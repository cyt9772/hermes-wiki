---
source_url: "/run/media/yutae/Data/퍼지_진화컴퓨팅 프로그래밍.pdf"
ingested: 2026-11-15
sha256: aec9a2276c20c9c174a9f42e84cc974abca01224fda2157909e3912c997784f2
type: raw-source
method: text-extract
---

# 퍼지_진화컴퓨팅 프로그래밍 (raw source)

> **출처:** USB 원본 PDF (`/run/media/yutae/Data/퍼지_진화컴퓨팅 프로그래밍.pdf`, 로컬 참고용 — git commit 불포함)
> **방법:** 내장 텍스트 레이어에서 `pdftotext -layout`로 추출 (OCR 불필요)
> **쪽수:** 212쪽 | **추출 텍스트:** 394 KB
> **주의:** 원고는 scan/레이어 추출로 영문·숫자·특수자 일부 아티팩트가 있을 수 있음. 해석 시 원본 PDF와 대조.
> OCR 추출 디렉터리 `raw/books/fuzzy-evolutionary-computing.ocr/`는 git-ignored (로컬 참고용만) — 본문은 아래에 내장.

## Book metadata
- **Title:** 퍼지_진화컴퓨팅 프로그래밍
- **Pages (PDF):** 212
- **Source:** 퍼지_진화컴퓨팅 프로그래밍.pdf
- **Ingested:** 2026-11-15

## Extracted text (all 212 pages)



===== PAGE 1 =====
                   ［매트랩 ]

퍼지,진화컴퓨팅 프로그래밍
Fuzzy, F加h血onary Coi珥)U血gi뇨恥amming
                            황희수


===== PAGE 2 =====
퍼지, 진화컴퓨팅 豆로그래밍
Fuzzy,.』 Evolutionary Computing Programming




                             w자＼V.naeha.co.kr


===== PAGE 3 =====
                       머리말
                          Fuzzy & Evolutionary Computing Programming




오늘날 공학기술의 핵심 트렌드는 고도의 전문성과 기술의 융합이라 할 수 있다. 과거와 다른
점은 그 어느 때 보다 융합이 강조되는 것이다. 아마도 변화가 빠르고 무한 경쟁의 시대에 생존
을 위해서는 기존에는 없는 새롭고 가치 있는 무언가를 창조해야 하는데, 융합이 새로운 돌파
구를 만들어 줄 수 있기 때문이 아닌가 싶다. 특정 분야에서 해결되지 못한 문제에 태해 다른
분야는 동일하지는 않지만 유사 문제의 해결책을 갖고 있을 수 있고 이를 활용하면 새롭고 혁
신적인 문제해결 방법을 찾을 수 있다. 또한 이미 존재하지만 이전에는 함께 사용되지 않았고
생각하지도 못했던 기술들이 융합되면 그 자체가 새로움을 만들어내는 힘을 갖는다．


이 책에서 다루고 있는 피지 시스템, 클러스터링 및 진화알고리즘은 퍼지 규칙（비선형 모델）을
만들기 위한 수단으로 이 분야를 공부하는 학생들에게 널리 알려져 있지만 저자가 이들을 융합
한 논문들 을 발표, 게재하던 1992년 전후만 해도 서로 독립적으로 발전해왔으며 동일한 목적
을 위해 함께 사용되지 않았다. 기존의 수식에 의한 최적화 방법으로는 퍼지 규칙의 전전부와
후건부 파라미터를 동시에 찾기 어려울 뿐만 아니라 찾는다 해도 국부수렴 문제로 전역 최적
해를 얻기 어려웠다. 진화알고리즘은 기존 최적화 방법 보다 계산 시간이 더 걸리지만 심지어
수식화가 불가능하더라도 컴퓨터 내에서 계산 할 수 있는 문제라면 전역 해를 찾을 수 있다.
클러스터링은 데이터 자체의 속성을 이용해 데이터를 분류하고 패턴을 찾는 분야에서 연구되
어 왔다. 특정한 데이터로부터 피지 규칙을 만들려면 그 구조어］ 대한 사전 정보（규칙의 수와
입출력 변수 및 그 퍼지 분할）를 필요로 한다. 이것을 알아야 최적화를 통해 규칙을 구성하는
파라미터를 찾을 수 있다. 그 당시에는 구조 정보를 가정하고 반복적인 시행착오를 통해 최적
의 피지 규칙을 찾으려 했다. 클러스터링은 바로 구조에 대한 사전 정보 없이도 데이터 특성만
으로 구조 정보를 얻을 수 있는 수단을 제공하기 때문에 반복적인 시행착오를 줄일 수 있게
해준다. 이처럼 3가지 서로 다른 이론들이 적절히 융합되면 서로의 장점을 살려 상승효과를
만들어 낼 수 있는 것이다．


이 책을 통해 독자는 피지 시스템, 피지 클러스터링 및 진화알고리즘仁｝분진화, 이진 및 실수형
유전알고리즘）의 매트랩 프로그래밍을 배우게 되며 5장에서 이들 이론이 결합되어 퍼지 규칙
（비선형 모델）을 효과적으로 만드는 방법을 배우게 될 것이다. 이 책의 핵심은 데이터가 주어지


===== PAGE 4 =====
iv
     면 그 뎨이터에 내재된 입출력 관계를 기술하는 최적의 퍼지 규칙을 자통으로 손쉽게 만드는
     것이다. 주어진 데이터가 이벤트 예측어］ 대한 것이면 생성된 퍼지 규칙은 예측 시스템으로, 패
     턴 분류어］ 대한 것이면 패턴 분류기로, 제어 통작어］ 대한 것이면 제어기로, 의사결정어］ 대한
     것이면 의사결정 시스템으로, 물체의 운동에 대한 것이면 거동 모델로 사용될 수 있다．


     이 책의 주제는 책 한 권으로 다루어질 수 없기 때문에 개별 주제어］ 대한 기본 이론들을 독자가
     알고 있다는 전제하어］ 이론척인 설명은 최소한으로 다루었으니 이 책을 공부하면서 기본 이론
     서를 참고하길 바란다. 이 책은 기본 이론을 프로그래밍하고 이를 토대로 자신의 요구에 맞는
     새로운 퍼지 규칙 생성 알고리즘을 연구하거나 데이터로부터 퍼지 규칙을 만들어 이를 이용하
     려는 학생들을 위한 책이다. 매트랩은 프로그래밍 방법도 쉽고 다양한 사용자 인터페이스 및
     그래픽 기능을 제공하기 때문어］ 일반적인 범용 언어（C, C++, Java 등） 보다 생산성이 뛰어나
     서 알고리즘을 설계, 분적하는 데는 최고이다. 범용 언어로 몇 십 줄어］ 해당하는 코드를 매트랩
     은 단 한 줄로 처리할 수 있다. 이 책에서 제공된 프로그래밍은 기본 매트랩 모듈에서 작동하며
     별도의 툴박스는 필요치 않다. 매트랩어］ 대한 사전 지식이 없는 독자는 이 책 부록의 '매트랩
     사용법' 부터 배우고 본문을 공부하기 바란다．


===== PAGE 5 =====
                            Fuzzy & Evolutionary Computing Programming




罐더장 퍼지 이론


 1. ] 퍼지 개요                                                     3
   1.1.1 역사                                                     3
    1.1.2 피지 대 비피지                                              3
 1.2 퍼지 집합                                                      4
    1.2.1 합집합, 교집합과 여집합                                         5
    1.2.2 十수준 집합                                                8
    1.2.3 동치관계                                                 10
    1.2.4 퍼지 변형자                                               10
    1.2.5 애매성의 증감                                              12
    1.2.6 다차원 멤버쉽함수                                            13
 1.3 퍼지 관계                                                     14
    1.3.1 합／교 관계                                               15
    1.3.2 합성 관계                                                16
 1.4 퍼지 추론                                                     17
    1.4.1 Mamdani형 퍼지 규칙에서의 추론                                 19
    1.4.2 Sugeno형 퍼지 규칙에서의 추론                                  36
    唾연습문제                                                      37
    唾 심화 학습 자료                                                 38




擊2장. 퍼지 클러스터링


  2.1 하드（Hard C-Mean引 클러스터링                                    41
  2.2 FCM(Fuzzy C-Means) 클러스터링                                 48
  2.3 분할의 타당성 평가                                               53
    好연습문제                                                      57
    專 심화 학습 자료                                                 57


===== PAGE 6 =====
vi




     宰 3장. 진화알고리즘m차분진화


       3.1 진화알고리즘의 개요           61
       3.2 진화알고리즘의 용도           63
       3.3 차분진화                 64
         難연습문제                  72
         茹 심화 학습 자료             73




     墩4장. 유전알고리즘


       4. ] 개체（하I)의 표현 및 초기화    78
       4.2 개체의 평가               83
      4.3 선택                    85
      4.4 유전 연산                 90
         4.4.1 이진 표현            90
         4.4.2 실수 표현            93
      4.5 종료조건                 100
      4.6 유전알고리즘의 처리           102
      4.7 유전알고리즘의 실행           111
         好연습문제                 125
         管 심화 학습 자료            126




     象5장. 퍼치 규칙의 생성


      5. ] 퍼지 모델               129
      5.2 퍼지 모델 인식             131
         5.2.1 구조 인식           132
         5.2.2 파라미터 인식         136
      5.3 퍼지 모델의 구축 및 평가       138
         5.3.1 모델의 구축          138


===== PAGE 7 =====
                                                               vii



    5.3.2 모델의 평가                                         155

   的연습문제                                                 158

    斗 심화 학습 자료                                           159




響부록. Matlab 사용법


 . 매트랩의 특징                                               163
    1) 매트랩의 실행 방법                                        164
    2) 매트랩 명령어                                           168
    3) 매트랩 기초                                            174
    4) 그래프 그리기                                           191
    5) 프로그래밍의 작성과 실행                                     196

    弊연습문제                                                204



  .찾아보기                                                  207



串 프로그램 코드 리스트



    孕 리스트 ］너 멤버쉽함수                                         4
    希 리스트卜2 합집합                                            6
    啼 리스트 ］田 교집합                                           7
    好 리스트卜4 여집합                                            8
    好 리스트 ］小 七수준                                           9
    豪 리스트 ］田 퍼지 변형자                                       11
    的 리스트卜7 애매성의 증감                                       12
    簪 리스트 ] 田 다차원 멤버쉽함수                                   13
    曲 리스트 ］四 최대m최소 합성                                     17
    好 리스트 卜］0 퍼지 변수 ser仇（石의 퍼지 집합 加or, good, excellent    19
    的 리스트 ］너 ] 퍼지 변수 /a河의 퍼지 집합 rancid, （抛仄放꺄S            21
    務리스트 卜］2 퍼지 변수 渤의 퍼지 집합 che口力， 口ver口ge, gene刃兀／S      22
    簪리스트 卜］3 봉사료 결정 규칙에서 퍼지화                              24
    簪리스트 卜］4 봉사료 결정 규칙에서 퍼지 연산자 적용                        26
    的 리스트卜15 봉사료 결정 규칙에 함의 연산자 적용                         28


===== PAGE 8 =====
Vu



     常 리스트 卜16 봉사료 결정 규칙에서 출력 퍼지 집합 합하기            29
     $ 리스트 卜］7 봉사료 결정 규칙에서 합하찐 출력 퍼지 집합의 비퍼지화      31
     斗 리스트 卜］8 봉사료 문제의 Mam扼ni형 퍼지 규칙에서 추론          33
     蜘 리스트 2너 나비 데이터의 하드 클러스터링                     44
     簪 리스트 2-2 FCM 클러스터링 코드                        49
     好 리스트 石3 평가척도 문V／了．,,,를 이용한 퍼지 분할 평가 코드       54
     學 리스트 于］ 차분 진화를 사용한 함수 최적화 코드                 66
     簪 리스트 午］ 이진 및 실수형의 초기 집단 생성, 초기화 및 평가         80
     務 리스트 午2 룰렛H휠 선택                              87
     管 리스트 4召 랭크 기반 선택                             88
     啼 리스트 午4 승자승 선택                               89
     嘴 리스트 午5 이진 돌연변이                              91
     心 리스트 午6 단순 교배（일점 교배）: 이진 및 실수 표현에 동일하게 사용    92
     的 리스트 午7 균일 돌연변이                              94
     斗 리스트 4田 비균일 돌연변이                             94
     啼 리스트 4四 멀티H비균일 돌연변이                          96
     啼 리스트 午］0 경계 돌연변이                             97
     毋 리스트 午］] 산술 교배1                              98
     學 리스트 午］2 휴리스틱 교배                             99
     簪 리스트 午］3 진화 세때1 수에 의한 종료                    100
     蜘 리스트 小］4 진화 세대 수와 목적함수 값어i 의한 종료            101
     好 리스트 午］5 유전알고리즘의 처리                         103
     母 리스트 午］6 유전알고리즘을 이용한 함수 최적화 사례              111
     孕 리스트 小17 이진 유전알고리즘어］ 의한 Rosenbrock 함수 최적화   119
     的 리스트 午］8 실수형 유전알고리즘에 의한 Rosenbrock 함수 최적화   122
     宙 리스트 5너 가스용광로 퍼지 모델의 구조 인식                  140
     a 리스트 5口 가스용광로 퍼지 모델 구축（차분진화 사용）             141
     a 리스트 5口 가즈느용광로 피지 모델 구축（유전알고리즘 사용）          152
     a 리스트 5召 가스H용꽝로 학습 및 평가용 데이터 분리              157


===== PAGE 9 =====
CHAPTER   퍼지 이론



          串 ] . ] 퍼지 개요
          水 1.2 퍼지 집합
          ：和 ] .3 퍼지 관7카
          永 ] .4 퍼지 추론


===== PAGE 10 =====
                                                       j장퍼지이론          口］
56 이 장어i서는퍼지 역사에대해간략히알아보，
                        고 퍼지집힙｛
                              fuzzy set), 멤버쉽함수（membership
   function), 小수준 집합（a-cut), 퍼지 관계（fuzzy relation), 퍼지 수（fuzzy number) 및 퍼지
   추론（fi.比zy inference）을 이해하고 이들을 매트랩으로 프로그래밍하는 것을 배운다. 이 책에서 사
  용된 매트랩 코드는 내하출판사（www.naeha.co.kr）의 자료실에 교재명의 압축 파일로 올려져 있
   으니 이를 다운로드 받아 사용하기 바란다（압축을 풀면 장별로 구분된 디렉토리가 만들어짐）.

                                                                      99


Fuzzy & Ev이utiona四
   Computing Programming   1.1 퍼지 개요


1.1.1 역사

 퍼지 이론은 미국 버클리태학 교수인 Zadeh가 1965년어］ 학술지어］발표한 퍼지 집합（fuzzy
sets）이란 논문에서 유래한다. 이 논문에서 피지 집합은 '큰 수의 집합’ 처럼 경계가불분명
한 집합이라 정의하고 있으며 인간 사고의 기본인 패턴인식 , 의미 정보의 전달과 추상화어］
커다란 역할을 한다고 적고 있다．




1.1.2 퍼지 대 비퍼지

 기존의 집합（crisp sets）은 '정수의 집합’ 처럼 집합에 대한 원소의 소속 여부가 명확한 반
면 '큰 수의 집합’ 처럼 피지 집합은 원소의 소속 여부가 단순히 가부로 확정될 수 없다. 여］
를 들어 "오늘 비가 올 것이다." 라고 확실히께 말하는 것은 참 또는 거짓 즉, 1 또는 0의
진리 값을 갖는다. 하지만 "오늘 비가 올 획률이 80％이다." 라고 말하면 이는 퍼지 논리
(fuzzy logic）를 사용한 것이다. 퍼지 논리는 0과 1 사이의 진리 값을 갖는 명제를 다룬다.
 퍼지 집합은 확신 정도를 다루는 것으로 확률（probabili缸）과는 다르다. 왜냐하면 확률에서
는 발생할지 모르는 불규칙성（randomness）어］ 기초한 가능성만을 취급하며 모든 발생 가능
한 사컨의 확률 합은 항상 1이다. 반면에 퍼지 집합에서 다루는 애매성（fuzziness）은 실제
발생하는 사컨에 대해서도 명확한（crisp) 판단을 내릴 수 없는 명제를 대상으로 한다. 가령，
 "친구가 내일 맛있는 저녁을 사줄까7" 라는 명제를 고려해 보자. 저녁을 사줄지는 확률 문


===== PAGE 11 =====
       퍼지, 진화컴퓨팅 프로그래밍



제로 내일이 되면 알 수 있지만, 사준 음식이 맛있을지 판단하는 것은 애매성을 다루는 퍼지
영역의 문제이다. 또한 퍼지 이론에서 애매성의 합이 반드시 1이 되어야 하는 것은 아니다．




 Fuzzy & Ev여Ut幻nary              睿
    Computing Programming            1.2 퍼지 집합


 보통 집합妃risp sets）에서는 어떤 원소가 집합 A에 속하면 그 소속 정도가 1, 속하지 않으
면 0이 된다. 퍼지 집합에서는 소속 정도를 1과 0 만이 아니라, 0 과 1 사이 값으로 표시할
수 있다. 퍼지 집합은 경계가 애매한 집합을 다룬다. 원소 工7} 퍼지집합 A에 속하는 정도는
멤버쉽함수（membership function) 바（功로 표시되며 0 과 1 사이의 값을 갖는다．

 리스트1-1은 피지 집합 'small number ' 와 ' about 5 ' 에 태한 멤버쉽함수를 정의하는 매트
랩 코드이다. 실행 결과가 그림1-1이다. 멤버쉽함수의 수평축은 universe of discourse로
불리며 피지 집합이 정의되는 변수 영역을 나타낸다. 수직축은 변수 영역의 값이 피지 집합어］
속하는 정도를 표시한다.                    그림에서      5가 퍼지 집합 'about   5 '에 속하는 정도는
1lAb。ut 5 (5) = 1.



    리스트 ］니 毋 멤버쉽함수

  % 파일명： fsets mu.m
  x=[0:0. l :101;
  muA = l./(l+0.8*x.A2); % fuzzy set 'Small number'
  muB = l./(I+5.*(x.5).八2); % fuzzy set 'About   5
                                                     '


  plot(x,muA,x,muB);
  title('Fuzzy sets: Small number, About 5');
  text( 1,0.7,'Small number');
  text(5,0.7,'About 5');
  xlabel('Universe of discourse');
  ylabel('Membership');


===== PAGE 12 =====
                                                               ］장 퍼지 이론   m

                           Fuzzy sets: Small number, About 5


                0    8


                          Small number    I 1 'out 5

              0     0
                    4
                    1
                     n0




             n三m뇨mnEm>




                    00        2        4         6              10
                                  Universe of discourse

           ［그림 1너］ 퍼지 집합 ' Small number'오I 'About 5' 의 멤버쉽함수




1.2.1 합집합, 교집합과 여집합

 피지집합 A와 B의 합집합(uni的은 A UB로 표시하며 합집합의 멤버쉽함수 값은 원소
工7} 퍼지집합 A와 B에 속하는 정도인 I'.A(X）와 nB（力의 최대값으로 한다．



   UAUB（兀）= max [1-lA（功 , 뱌m], \／工드x                                      (1.1)



 퍼지 집합 A와 B의 교집합（intersection)은 AflB로 표시하며 교집합의 멤버쉽함수 값
은 원소 工가 퍼지 집합 A와 B어］ 속하는 정도인 pd功와 1-'d功의 최소값（식（1.2)) 또는
곱（식（1.3)）으로 표시한다．


   比1flB（兀）= mmll [UA（兀）, UI了（兀）], V尤드x

   比1flB（工）= [llA（工） XIJB（兀）] , V尤드x


퍼지 집합 A의 여집합（complement）은 A "로 표기하며 식（1.4）와 같이 정의된다．


===== PAGE 13 =====
6        퍼지, 진화컴퓨팅 프로그래밍



         PA'- i H PA(x),VxeX                                                           (1.4)


    리스트 1-1어］ 정의된 두 개의 퍼지 집합어］ 대한 합집합 계산 코드가 리스트 1-2이며 그림
    1-2이 그 실행 결과이다．



       리스트卜2 心 합집합

     % 파일명： fsets union.m
     x=[0:0.l :10];
     muA = l./(l+0.8*x八2); % fuzzy set 'Small number'
     muB = 1.!(l+5.*(x-5).八2); % fuzzy set 'About 5'
     union = max(muA,muB);
     plot(x,union);
     title('Union of fuzzy sets: Small number, About 5');
     xlabel('Universe of discourse');
     ylabel('Membership');




                                     Union of fuzzy sets: Small number, About 5



                             0.8



                           0     0
                                 n
                                 O




                          Q三띤mnEm>
                                4




                               00         2         4         6        8          10
                                               Universe of discourse

                      ［그림卜2] 퍼지 집합 ' small number'오F 'about 5 ' 의 합집합



    리스트1-1어］ 정의퇸 두 개의 퍼지 집합에 대한 교집합 계산 코드가 리스트 1-3이며 실행
결과가 그림 1-3이다．


===== PAGE 14 =====
                                                                      '         1장퍼지 이론   ]m



   리스트］小 S 교집합

  % 파일명： fset乞intersection.m
  x=[0:O.1:10];
  muA = 1J(1+O.8*x.A2); % fuzzy set 'Small number'
  muD = 1J(1+5.*(x-5) 八2); % fuzzy set 'About 5'
  intersection! = min(muA,muB); % 최소값혀1 의한 계산
  intersection2 = muA.水muB; % 곱하기어］ 의한 졔산
  p!ot(x,intersection1,x,intersection2);
  axis([0,10,O,1});
  tit!e('Intersection of fuzzy sets: Small number, About 5');
  xlabel('Universe of discourse');
  ylabel('Membership');
  text(3,O.11,'minimum');
  text(5,0.08,'product');




                                 Intersection of fuzzy sets: Small number, About 5
                           I


                        0.8



                       0    0
                             八
                             b




                      Q三인mnEm>
                             4




                        0.2

                                         1깻 쁘世으」Ct                              .
                            q;            2        4         6            8      10
                                              Universe of discourse

                      ［그림卜3] 퍼지 집합 ' Small number ' 와 'About 5꾀 교집합



 기존의 이진 논리 연산 AND와 OR를 퍼지 논리 연산으로 확장한 것을 각각 于norm과
卜norm이라 부른다. 식（1.1) N 식（1.3）은 于norm과卜norm의 여러 연산 방식 가운데 대표
적으로 많이 사용되는 것이다. 퍼지집합 ' about 5' 어］ 대한 여집합 계산 코드가 리스트 1-4


===== PAGE 15 =====
:     1    퍼지， 진화컴퓨팅프로그래밍


    이고 실행 결과가 그림 1-4이다．


          리스트卜4 亡 여집합

      % 파일명： fsets_complement.m
      x=[O:O.1:10];
      muB = l./(I+5.*(x-5) 八2); % fuzzy set 'About 5'
      complement = 1 - muB;
      plot(x,complement);
      axis([O,10,0,1]);
      title('Complement of fuzzy set: About 5');
      xlabel('Universe of discourse');
      ylabel('Membership');
      text(5,0.7,'not About 5');




                                         Complement of fuzzy set: About 5




                           0     0
                                 n0




                          q三띤mnEm>
                                 4




                            0.2



                               00                  4         6        8     10
                                              Universe of discourse

                                      ［그림卜4] 퍼지 집합 'About 5'의 여집합




    1.2.2 a-수준 집합

     경계가 애매하지만 퍼지집합 A에 포함된 원소 가운데 멤버쉽함수 값이 a 이상이면 보통


===== PAGE 16 =====
                                                         ,   1장퍼지이론
                                                                       ]n
집합（crisp sets）으로 표시할 수 있는데, 이를 七수준（U-cuts) 집합이라 하며 다음 식（1.5)
과 같이 정의한다．


    凡＝｛尤드치1A(x)＞따                                                     (1.5)



 퍼지집합 'about 5 ' 에서 멤버쉽함수 값이 0.5 보다 큰 변수 영역을 구한다고 할 때 0.5가
七수준이 된다．
 十수준을 구하기 위한 코드가 리스트 1-5이며 결과가 그림 1-5이다. 리스트에서
mm1l_alpha_cut = 4.56와 max_alpha_cut = 5.55는 변수 x의 七수준을 결정하는 최소 및
최대값으로 이 범위에 속한 모든 x 값이 d '＞준이다. 리스트에서 alpha_cut = (muB >=
0.5）은 muB와 동일한 크기의 벡터를 만들어 muB가 0.5 이상인 점에는 1을, 그렇지 못한
점에는 0을 넣어서 alpha끄-it에 컨네준다. 또한 m1ld = find(muB >= 0.5）은 muB가 0.5 이상
인 muB의 인덱스를 짖0｝주며 x(min(ind)）와 x(max(ind力는 그 인덱스의 최소 및 최태값 위
치에 있는 x의 값을 결정한다. 이 최소값과 최대값 사이의 영역이 a 수준 집합인 것이다．


啣聯 리스트］小 1 h수준

  % 파일명： fsets_alpha_cuts.m
  x=[0:0.01:101;
  muB = 1.!(l+5.*(x-5)/\2); % fuzzy set 'About 5'
  alpha_cut = (muB >= 0.5);
  mild = find(muB >= 0.5);
  mmn_alpha_cut = x(min(ind)); % 키pha cut 벡터의 최소값
  max_alpha_cut = x(max(ind)); % alpha cut 벡터의 최대값
  ho너 on;
   plot(x,alpha_cut,'b-');
   plot([min_alpha_cut max_alpha_cutl,[0.0 0.0],'r+');
   axis({0,10,0, 11);
   title('Alpha cuts of fuzzy set: About 5');
   xlabel('Universe of discourse');
   ylabel('Membership');
   text(4.5,0.05,'alpha cut');


===== PAGE 17 =====
10      퍼지, 진화컴퓨팅 프로그래밍




                                         Alpha cuts of fuzzy set: About 5
                     1


                 0.9


                 0.8


                 0.7

                  6
                  0

                        4

                  b
                  =0    0

               口三em口Em>



                 0.3 나


                 02


                 0.1


                   0                               "" ' "
                                                   中’
                                                        므
                    0       1   2    3      4         5         6           7   10
                                            Universe of discourse




                            ［그림卜5] 퍼지 집합 ' about 5 ' 의 (1-수준 집합




 1.2.3 동치관겨1

     모든 원소 尤7} 피지 집합 A와 B어］ 속하는 정도가 같을 때 즉, 멤버쉽함수 값이 같을 때
 A와 B는 동치라 하고 식（1.6）와 같이 표시한다. 만약 어느 한 원소어］ 대해서도
 l노（尤）半UB（兀）이면 A半B이다．


       A= B ifandonlyif 11A（尤）= 'tB（功 , V工드x                                         (1.6)




1.2.4 퍼지 변형자

     퍼지 집합의 변형자 가운데 'very'는 퍼지 집합을 수축시키는 역할을 한다. 리스트1-1에서
퍼지 집합 ' small number'어］ 'very를 붇여 ' very small number'로 하면 이는 정량적으로
'small number'의 멤버쉽함수 값을 제곱한 것이다. 반대로 변형자 가운데 'more or less는


===== PAGE 18 =====
                                                             '       j장퍼지이론   ]m
피지 집합을 팽창시키는 역할을 하며 정량적으로는 멤버쉽함수 값어］ 제곱 근 을 취하는 것이
다. 리스트 1-6과 그림 1-6은 변형자어］ 대한 코드와 그 결과이다．


螂蹄 리스트 ］七 亡 퍼지 변형자

  % 파일명： fsets mo小fier.m
  x=[0:0. 1:10];
  muA = l./(1+0.8*x八2); % fuzzy set 'Small number'
  mu very = muA.A2;
  mu_moreorless = sqrt(muA);
  plot(x,muvery,x,mumoreorless);
  title('Fuzzy set modifier: Small number');
  text(l.5,0.2,'ve口 small number');
  text(l.5,0.7,'more or less small number');
  xlabel('Universe of discourse');
  ylab에'Membershi이；




                                  Fuzzy set modifier: Small number




                    0    0
                          n
                          O




                   으
                   ＝ 딴m쇼Em>
                          4
                          1




                                  very small numbe



                              0      2        4         6        8    10
                                         Universe of discourse
                                     ［그림卜6] 퍼지 집합의 변형자


===== PAGE 19 =====
U田口       퍼지, 진화컴퓨팅 프로그래밍




 1.2.5 애매성의 증감
  퍼지 집합의 애매성을 증가 또는 감소시킬 수가 있는데, 식（1.7）과 갇은 멤버쉽함수를 고려
 해보자. 멤버쉽함수를 구성하고 있는 파라미터의 값어］ 따라 퍼지 집합의 애매성이 증감된다．
 리스트 1-7에 파라미터의 영향을 알아보기 위한 코드가 주어지며 그 결과가 그림 1-7어］ 있다．



                                                   (1.7)
                          1
                          『         /
      "
          '
              "
                  "
                      『
                              （P2
      리스트卜7 蜘 애매성의 증감

  % 파일명： fsets intensification.m
  x = [0:1:100];
  pl = [5 10 100];
  p2 = 50;
  for i=1:Iength(pl)
          % fuzzy set 'Large number'
          muA(i,:) = 1水1+(x./p2)즈(-pl(i)));
  end
  p2 = [10 50 100];
  pl = 2.5;
  for i=1:length(p2)
          % fuzzy set 'Large number'
          muB(i,:) = 1./(1+(x./p2(i)).八(p1));
  end
  plot(x,muA,x,muB);
  title('Fuzzy set: Large! number');
  xlabel('Universe of discourse');
  ylabel('Membership');
  text(10,0.9,'pl=2.5, p2 =10');
  text(70,0.7,'pl=2.5, p2 =50');
  text(70,0.3,'pl=2.5, p2 =100');
  text(35,0.7,'pl=5, p2 =50');
  text(50,0.85,'pl=lO, p2 =50');
  text(75,0.9,'pl=lOO, p2 =50');


===== PAGE 20 =====
                                                                                               1장 퍼지 이론



                                                                Fuzzy set: Large number




                     0    0

                    Q三띤mnEm>




                                                         20           40         60       80   100
                                                                  Universe of discourse

                         ［그림卜7] 퍼지 집합 ' large number ' 의 애매성 증감




1.2.6 다차원 멤버쉽함수
 다차원인 입력 공간에서 멤버쉽함수를 정의해야 하는 경우에는 가우스 함수를 이용할 수
있다. 식（1.8）은 입력이 伊｝ y인 2차원 공간에서의 멤버쉽함수를 정의하고 있지만 고차원으
로 쉽게 확장할 수 있다. 이 식에서 파라미터（a, b, c, d, 力） 값에 따라 멤버쉽함수의 모양이 달
라진다. 식（1.8）에 의한 피지 집합 'x is near 2 and y is near 3' 어］ 대한 멤버쉽함수를 작성
하는 코드가 리스트1-8어］ 있고 그 결과가 그림 1-8어］ 보여진다．


                         [     4   (r-   h
                                             )   2
                                                     +『   (y-   d) 2   1
    P/?（尤, y) =    e     I                           力                 J                                  (1.8)



枷牡 리스트］田 難 다차원 멤버쉽함수

  % 파일명： fsets multi mu.m
  [x,y] = meshgrid(-5:0.5:10,-5:0.5: 10);
  p= 2; a= l; b= 3; c= 0.5; d= 2;
  multi mu = exp(-(a永（x-b)．八2 + 少（少마으）巾）;
  C아ormap(hsv); % surf 함수에서 사용할 색지도 지정


===== PAGE 21 =====
口m[ 퍼지
     ，진화컴퓨팅프로그래밍
    surf(x,y,multimu);
    view(45 ,45);
    title('Multi-dimensional fuzzy set');
    xlabel('x');
    ylabel('y');
    zlabel('Membership');




                                            M미作dimen引onal fuzzy set




                         0   二
                             U


                      Q三딴mnEm듣
                             0
                            5
                                                                      10



                                                    10           y
                                              x

                    ［그림卜8] 다차원 멤버쉽함수 ' x is near 2 and y is near 3'




  Fuzzy & Evolutionary
     Computing Programming            1.3 퍼지 관겨1                           ]
   일반적으로 집합 A와 B에 대해 A의 원소 尤와 B의 원소 y 사이에 관계（relation)가 있
  으면 이를 순서쌍 ( 兀, y）로 표시할 수 있다. 예를 들어 집합 A와 B 사이어］ 다음과 갇은 관계

  가 있다고 하자． A=｛幻 , 抑｝,B= {y1, y2, y3}. I？은 伊｝ y 사이의 관계를 정의하는 멤버쉽

  함수 값으로 여기서는 " 兀7} y와같은 정도를표시하는관계" 라하자. 차이 乃와갇은 정도


===== PAGE 22 =====
                                                                                              1장 퍼지 이론   ］
                                                                                                         口m


는 n （尤］ , Y2) = 0.2 이다． PR（兀', y1）은 0으로 이는 幻이 y1j2} 전혀 갇지 않음을，
llR（兀2, Yl）은 1로 兀2오｝ y1이 완전히 같음을 의미한다．



                                                   R                      Yi      Y2    y3

                                                   尤l                         0   0.2   1

                                                   兀2                         1   0.5   0.1

                                               工오｝ y의 관계를 정의하는 멤버쉽함수 값




1.3.1 합／교 관겨1

 퍼지 합 관계（fuzzy union relation)는 두 개의 퍼지 관계 /？과 Q의 합집합 /?UQ로 표시
하고, 합집합 관계의 멤버쉽함수는 식（1.9）과 같이 정의된다．


    /?={ （兀, y), ll/?（兀, y) 1（尤, y) 드x來 y}

    Q= {（兀 y), U Q（兀, y爪兀，y) 드x非 y}                                                                      (1.9)

    nRIJQ（尤，y) = max [11R(兀 y), IIQ（尤，y) ] = .1 R(兀 y) V如佃功



 위 식에서 串는 x와 Y 사이의 피지 관계를 나타내며 max 연산을 \／로 표기한다. 이를
刃개의 관계로 확장하면 식（1.10）과 같이 된다．



    1lR1J足                          (x,   y)   =   X    4凡   （/    ,y)
                                                                                                         (1.10)



퍼지 교 관계（fuzzy intersection relation)는 두 개의 피지 관계 /？과 Q의 교집합 RflQ로
표시하고, 교집합 관계의 멤버쉽함수는 식（1.11）와 같이 정의되며 이를 n개의 관계로 확장하
면 식（1.12）과 같이 된다. 여기서 n丘n 연산은 /＼로 표기한다．


     U 尺nQ（尤，y) = min[1R(x, y), 1.1d兀 y) ] = 1.1尺（尤，y) n知（尤，y)

     U R1flR2   .   ..   fl   R,   』(X,   Y)   =   쇼    UR   (x,         y)                              (1.12)


===== PAGE 23 =====
16       퍼지, 진화컴퓨팅 프로그라俚J




 1.3.2 합성 관겨1

     최대1최소합성（n追x小n血lcomposition) 관계를 알아보자. 두 개의 퍼지 관계 /？과 Q가
 다음과 같이 집합 x, Y와 z어］ 대해 정의되었다고 하자. 즉, 피지 관계 R은 집합 x와 Y
 사이의 관계를 정의하고, 퍼지 관계 Q는 집합 Y와 z 사이의 관계를 정의한다．


        /？드x永 Y, （工, y）드x半 Y

        Q드 }佯乙 (y, z）드 Y求z



     이 때 이들 두 개의 관계 /？과 Q의 합성 /?.Q는 집합 x와 z 사이의 관계를 정의할 수
 있다. 이 합성관계에 대한 멤버쉽함수는 식（1.13）어］ 의해 정의된다．



        11只』0（尤，2)
                z) = m릎즈 [min(UR（兀，y),UQ (y, 2) ]                                   (1.13)

                   = Y [UR(x,y)AU。(y,z)]
 여기서 집합 x, y, z를 사컨들의 집합이라 가정하자. 퍼지 관계 /？로부터 집합 X7} 발생
 하면 집합 Y가 발생할 가능성을 알 수 있으며 , Q로부터 집합 Y가 발생하면 집합 z가 발생
 할 가능성을 알 수 있다. 다시 말하1 집합 x의 원소인 사컨 抑이 발생하면 n （抑 , 的）에 의해

 집합 Y의 원소인 사건 刃이 발생할 가능성을 알 수 있고 식（1.13）의 피지 합성 관계

     llR , Q（尤l ,自）로부터 z1이 발생할 가능성을 알 수 있다． 이와 같은 규칙을 적용하여 새로운
 사실을 알아내는 것을 추론（耐erence）이라 한다．
     그림 1-9에서와 같이 （兀, y）의 관계 /？과 （兀, 2) 관계 Q가 주어질 때 최대 최소 합성 관계
 R. Q를 계산하는 코드가 리스트1-9이다．



        R     y1    Y2    y3     Q     z1    z2     z3    R. Q    z1    z2    之3

        尤l    1    0.7   0.4     y1   0.3   0.1     0.6    尤l     0.7   0.7   0.7
        兀2    0     1    0.6     Y2    1    0.7     1      兀2     1     0.7   1
        兀3   0.7    1    0.4     y3    1    0.6     1      2:,i   1     0.7   1

                   ［그림卜9] 관7朴 /?(:.,). Q (,.a) 및 합성 관:7카 ／小 Q (;. :)


===== PAGE 24 =====
                                                            ,   1장퍼지이론   ]m
   리스트 ] 四 作 최L十최소 합성

  % 파일명： fsets寸composition.m
  R = [1 0.7 0.4; 0 1 0.6; 0.7 1 0.4];
  Q = [0.3 0.1 0.6; 1 0.7 1; 1 0.6 1];
  [rr,rc] = size(R);
  [qr,qc] = size(Q);
  composition = zeros(rr,qc);
  for i=1:rr
        的r j=1:qc
              % 최다卜최소 합성
               composition(i工) = max(min(R(i,:),Q(:j)'));
        end
  end




Fuzzy & Evolutionary
   Computing Programming             1.4 퍼지 추론


 언어적 기술로 이루어진 퍼지 명제는 애매함을 포함하고 있는 것이 그 특징이다. 尤와 y가
각각 집합 x와 Y의 임의의 원소이고 A가 X, B가 Y의 퍼지 집합이라고 하면 다음과 같
은 퍼지 명제를 정의할 수 있다. 이런 명제 형식이 퍼지 논리를 다루는 기본이 된다．

 퍼지 명제 : P = 兀 is A, Q = y is B

 "P이면 Q이다." 라는 퍼지 조건 명제는 다음과 같이 표현될 수 있다. 여기서 ／곡三 퍼지 조
컨 명제의 전건부／조건부（antecedent）를, Q는 후건부／동작부（consequ이此）를 나타낸다．

 퍼지 조건 명제 : P- Q= If P then Q

 퍼지 추론（fuzzy in扼rence）은 몇 개의 퍼지 명제로부터 하나의 다른 퍼지 명제를 도출하는
것으로, 이를 근사 추론（approximate reasoning）이라 한다. 퍼지 추론은 아래에 보인 것처
럼 퍼지 조건 명제 "If 兀 is A then y is B"를 조컨으로 하고 퍼지 명제 " 兀 is A ' "를 전제하


===== PAGE 25 =====
U田口   퍼지, 진화컴퓨팅 프로그래밍



 여 이로부터 후건부 " y is B" 어］ 의미상 가까운 퍼지 명제 B"를 추론하는 것이다．


                         조건 : If 工 is A then y is B
                         전제 :     兀 is A'


                         결론 :     y is B'




  이 추론은 전제인 퍼지 명제（尸"）가 조컨의 전컨부 명제（끼와 달라서 결론 Q ' 도 조컨의 후
 컨부 명제（Q）와 다르지만 보통의 추론 규칙（跏dus pon帥5）을 따른다는 의미에서 일반화된
 추론 규칙（generalized modus pon帥S）이라 부른다．
  퍼지 추론에서는 이진 논리에서와 달리 다양한 해석이 존재하기 때문에 추론 방식이 다양
 하다. 피지 추론법으로는 합성 규칙을 기반으로 한 직접법, 언어적 진리값을 매개로 한 간접
 법이 있으며 직접법에는 크게 전건부와 후건부의 형태에 따라 Mamdani형과 Si.培eno형으로
 나뉜다. 八4amdani 형은 후건부가 피지 집합에 의하1 정의되는 반면 Sugeno형은 선형식이나
 상수（fuzzy sin멤eton이라 함）를 갖는다．
  퍼지 추론 합성 규칙은 퍼지 관계와 합성 연산어］ 의해 근사적 결론을 도출하는 방법이다．
 위에 보여진 Mamdarii형 규칙에서 결론 도출은 식（1.14）와 같이 기술할 수 있다. 이 때 최대
 1최소 합성 규칙이 사용된다면 퍼지 집합 B' 의 멤버쉽함수는 식（1.15）와 같이 계산된다．


      B =A   " R (P.Q)                                 (1.14)

      」B (y)= , 盖 [ 也4帥RCA.，仁y)1                       (1.15)


  . 입력 데이터를 퍼지 규칙에 적용하1 출력 데이터를 얻는 방법
  명확한 입력 데이터가 주어질 때 피지 규칙으로부터 명확한 출력을 추론하는 과정은 다음
 과 같이 5단계로 이루어진다．
  (D 입력의 피지화（fuzz汪ication)
  （易 피지 규칙의 전컨부에 퍼지 연산자 적용
  （多 함의（implication) 방법 적용
  @ 모튼 퍼지 규칙의 후컨부 퍼지 집합을 하나로 모음
  （旬 하나로 모아진 퍼지 집합으로부터 최종 출력을 계산個efuzzification)


===== PAGE 26 =====
                                                                   ］장 퍼지 이론   19



 이 과정을 Mamdani 및 Sugeno형 퍼지 규칙어］ 대해 적용해 보자．




1.4.1 Mamdani형 퍼지 규칙에서의 추론

 식당에서 종업원에게 줄 봉사료의 양을 결정할 때 아래 3가지 피지 규칙을 사용한다고 하
자. 피지 규칙어］ 사용될 입력 변수로는 서비스 질을 평가하기 위한 ser功ce와 음식의 맛을
평가하기 위한 /ood, 출력변수로는 팁의 앙을 결정하는 渤이 고려되었다．


 R1: If service is 加or or food is 及2nc河 then ／功 is che口力．

 R2: If service is good then tip is average.

 R3: If service is excellent and food is delicious then tip is generous.


 먼저 규칙어］ 사용된 입출력 퍼지 변수의 피지 집합이 정의되어야 한다. 리스트1-10은 입력
퍼지 변수 service에 대한 퍼지 집합 加or, good과 excelle耐의 멤버쉽함수를 정의하는 코드
이며 실행 결과가 그림1-10에 보여진다. 리스트1-11과 그림1-11은 입력 퍼지 변수 /rnood어］
대한 피지 집합 r口加河와 delic勿us어］ 대한 것이고 리스트1-12와 그림1-12는 출력 피지 변
수 渤어］ 대한 퍼지 집합 c力e口勿 口ver口ge와 gener（兀／5어］ 대한 것이다．


懈螂瑟 리스트卜］0 舜 퍼지 변수 ser沅ce의 퍼지 집합 加（7r, good, excellent

  % 파일명： fsets service.m
  service = 1:0.2:10:
  mu_poor = triangle(service,[0 1 41);
  mu_good =       triangle(service,[3 5 10]);
  mu excellent =       triangle(service,[5 10 111);
  plot(service,mu巾oor,'b-',service,mu_good,'k-',...   % ...는 줄 바꿈 명령어
  service,mu excellent,'r-');
  title('Fuzzy sets: poor, good, excellent');
  佃奴 1.乙0.9巾oor');
  text(4.75,0.9,'good');
  text(8.8,0.9,'excellent');
  xlabel('service');
  ylabel('membership');


===== PAGE 27 =====
20   퍼지, 진화컴퓨팅 프로그래밍




        function [mu] = triangle(x, parm);
        % 삼각형 모양의 멤버쉽함수
        % 사용법: [mu] = triangle(x, parm)
        %                      x: 논리영역의 입력변수 값
        %                      parm: 멤버쉽함수의 모양을 결정하는 파라미터
        %                      mu: 리턴되는 멤버쉽함수 값


        a = parm(1); b = parm(2); c = parm(3);
        mu = zeros(size(x));
        凡r i=1:向gth(지
               if (x(i) < a) mu(i) = 0;
               이se汗 (x(i) >= a & x(i) < b)
                        mu(i) = (x(i)-a)./(b-a);
               이se汪 似(i) >= b & x(i) <= c)
                      mu(i) = (x(i)-b)/(b-c) + 1;
              else
                      mu(i) = 0;
              end
        end




                                    Fuzzy sets: poor, good, excellent


                                                                          nt




                      0   0

                     으듦b口Em드




                                                   4             6   8   10
                                                       service
         ［그림 1너0] 퍼지 변수 serv匕e의 퍼지 집합 加（r, good, e冗cellent


===== PAGE 28 =====
                                                               ,      ］장퍼지이론   ]m
mm 리스트卜］1 ' 퍼지 변수 /-oo／의 퍼지 집합 及incid, delicious

  % 파일명： fsets_food.m
  food = 1:0.2:10;
  mu_rancid = trapezoidal(food,[0 1 2 4]);
  mu_delicious = trapezoidal(food,[5 9 10 11]) ;
  plot(food,mu_rancid,'b-',food,mu_delicious,'k-');
  title('Fuzzy sets: rancid, delicious');
  text(2,0.9,'rancid');
  佃奴＆0.9,'delicio四）;
  xlabel('food');
  ylabel('membership');


              function [mu] = trapezoida姙, parm);
              % 사다리꼴 모양의 멤버쉽함수
              % 사용법: [mu] = trapezoidal(x, parm)
              %                     x: 논리영역의 입력변수 값
              %                     parm: 멤버쉽함수의 모양을 결정하는 파라미터
              %                     mu: 리턴되는 멤버쉽함수 값
              %                     parm(1)<parm(2)<parm(3)<Par奴4）를 만족해야 함．


              a = parm(1);
              b = parm(2);
              c = parm(3);
              d = parm(4);
              mu = zeros(size(x));
              白r i=1:length（지
                    if (x(i) <= a) mu(i) = 0;
                    elseif (x(i) > a & x(i) < b)
                           mu(i) = (x(i)-a)./(b-a);
                    이se迂 (x(i) :>= b & x(i) < c)
                           mu(i) = 1;
                    elseif (x(i) >= c & x(i) < d)
                           mu(i) = (x(i)미如－d) + 1;
                    else
                           mu (i)    =   0;
                    end


===== PAGE 29 =====
.國口    퍼지, 진화컴퓨팅 프로그래밍



              end




                                        Fuzzy sets: rancid, delicious
                            1
                                         n이d                            de cious
                            毗



                           4
                      O
                      n
                      0    0

                     Q三띤mn드m드




                       0.2



                            00      2           4          6            8      10
                                                    food

                      ［그림 卜11] 퍼지 변수 /bod의 퍼지 집합 7七2ncid, delicious



      리스트卜］2 蜘 퍼지 변수 ／功의 퍼지 집합 C力e口力， 口ver口ge, ge刃ero끄S

  % 파일명： fsets_tip.m
  tip = 0:0.5:25;
  mu_cheap = bell(tip,[1 0]);
  mu_average = bell(tip,[1 10]);
  mu_generous = bell(tip,[0.5 25]);
  plot(tip,mucheap,'b-',tip,mu_average,'k-',tip,mu_generous,'r-');
  title('Fuzzy sets: cheap, average, generous');
  佃奴2,0.9,'cheap');
  text(12,0.9,'average');
  text(21,0.9,'generous');
  xlab이(ti可％)');
  ylabel('membership');


             function [mu] = bell(x,parm);


===== PAGE 30 =====
                                                         '        1장퍼지        이론   ］回
         % 종 모양의 멤버쉽함수
         % 사용법： [mu] = bell(x,parm)
         %        x: 논리영역의 입력 변수 값
         %        parm: 종의 모양을 결정하는 파라미터
         %        mu: 리턴되는 멤버쉽함수 값

         a = parm(I); b = parm(2);
         mu = 1.1(1 + a*(xb)/2);




                          Fuzzy sets: cheap, average, generous




                     4
                b
                八
                0    0

               쇼芝띤m口EmE




                                      10            15       20          25
                                           tip(%)
          ［그림 卜12] 퍼지 변수 渤의 퍼지 집합 C力e幼， 口ver口ge, ge冗ero瓦S



ci) 퍼지화（Fuzzificat向n)
 퍼지화는 명확한 입력변수 값을 퍼지 값（멤버쉽함수 값）으로 바꾸는 것을 말한다. 위의 서］
규칙에서 정의된 퍼지 입력 변수 service와 /bod는 각기 1 - 10 사이의 값으로 정량화 된다．
가령 , 음식을 먹은 후 service = 6, food = 6이라는 평가를 내렸다고 하자. 이 입력 값이 멤
버쉽함수를 통하1 퍼지 집합어］ 속하는 정도를 결정하는 것이 퍼지화이다. 즉, ser沅ce = 6인
값이 퍼지 집합 加or, good, excelle耐에, food = 6인 값이 피지 집합 rancid, delicious어］
속하는 정도를 계산하는 것이다. 이는 퍼지 집합의 멤버쉽함수에서 얻어지며 그 과정이 리스
트 卜13어］, 퍼지화 결과가 그림 1-13에 보인다．


===== PAGE 31 =====
           퍼지, 진화컴퓨팅 프로그래밍




-     리스트卜｝3 小 봉사료 결정 규칙에서 퍼天區1 蜘懈辯啣「懈驪娜빠娜娜麟恕

    % 파일명： fset乞血zz小cation.m
    % input = service 퍼지화
    fsets4service; % fsetsservice.m 호출 -> 멤버쉽함수 표시
    axis([1 10 0 1]);
    service = 6;
    mu_poor = triangle(service,[0 1 4]);
    mu_good = triangle(service,[3 5 10]);
    mu_excellent = triangle(service,[5 10 11]);
    h아d on;
    x = [service service];
    plot(x,[0,muegood],'k-',x,[O,mu_poor],'b-',x,[O,muexcellent],'r-');
    text(service+0.1,mu_poor+0.02,['mu(poor) = ' num2str(mu_poor)]);
    text(service+0.1,mu_good+0.01,['mu(good) = ' num2str(mu_good)]);
    text(service+0.1,mu_excellent+0.07,['mu(excellent) = '...
    num2str(mu_excellent)]);
    clear;
    pause;
    clf;
    % input = food 퍼지화
    fsets_food; % fsetsHfood.m 호출 -> 멤버쉽함수 표시
    axis([1 10 0 1]);
    food = 6;
    mu_rancid = trapezoidal(food,[0 1 2 4]);
    mu_delicious = trapezoidal(food,[5 9 10 11]) ;
    hold on;
    x = [food food];
    plot(x,[0,mu_rancid],'b-',x,[O,mudelicious],'k-');
    text(food+0.1,mu_rancid+0.02,['mu(rancid) = ' num2str(mu rancid)]);
    text(food+0.1,mu delicious+0.01,['mu(delicious) = '...
    num2str(mu_delicious)]);


===== PAGE 32 =====
                                                                 1장 퍼지 이론   ]m


                         Fuzzy sets: poor, good, excellent




           0    0
                 八
                 O




          쇼三띤m口EmE
                 d
                 1




                                           6                     10
                                      servi冶
                                    (a) ser仇ce


                           Fuzzy sets: rancid, delicious
               1
                     r ncid                            de 이ous
            0.8



           0    0
                 n
                 O




          Q三띤mnEmE
                 d
                 1




                                            mu(delicious) = 0.25
            0.2


               0
                     2          4           6          8           10
                                        food

                               (b) food
                     ［그림 卜13] service와 ／切d의 퍼지화



（多 퍼지 연산자 적용
모튼 입력의 퍼지화가 끝나면 피지 규칙의 각 전컨부가 어느 정도 만족되는지 알 수 있다．
규칙의 전건부가 둘 이상의 피지 변수로 구성되어 있으면 퍼지 연산자를 적용하여 각 전컨부
에 대한 만족도를 계산할 수 있다. 이렇게 계산된 만족도는 각 규칙의 후건부에 적용될 것이


===== PAGE 33 =====
26        퍼지, 진화컴퓨팅 프로그래밍



 다. 퍼지 연산자의 입력은 각 규칙의 전컨부를 구성하고 있는 입력의 퍼지화 값이고 출력은
 하나의 진리 값이다. 규칙의 전건부를 구성하고 있는 퍼지 변수들은 An）나 OR로 연결되어
 있다. Aln）와 (JR를 정의하는 퍼지 연산자는 다앙하지만 주로 Al寸D 연산자로는 최소값（II血）
 과 곱하기（product）를, OR 연산자로는 최대값（ma功을 사용한다．
     리스트 1-14와 그림 1-14는 팁 문제에 대한 퍼지 연산자 적용을 다루고 있다．


 mm 리스트卜］4 弊 봉사료 결정 규칙에서 퍼지 연산자 적용

     % 파일명： fsets_operation.m
     service = 6;
     mu_poor = triangle(service,[0 1 4]);
     mu_good =      triangle(service,[3 5 10]);
     mu_excellent =      triangle(service,[5 10 11]);
     food = 6;
     mu_rancid = trapezoidal(food,[0 1 2 4]);
     mu_delicious = trapezoidal(food,[5 9 10 11]) ;
     % Ri 규칙의 전거부에 퍼지 연산자 적용（OR -> max 연산）
     rule1_satisfaction = max(mu_poor,mu_rancid);
     rule2_satisfaction = mu_good;
     % R3 규칙의 전거부에 퍼지 연산자 적용｛AND -> mmtl 연산）
     rule3_satisfaction = min(mu_excellent,mu_delicious);
     x = [1 2 3]; % 규칙 번호
     bar width = 0.5;
     bar(x,[rule1_satisfaction ru1e2_satisfaction
     rule3_satisfaction],bar_width);
     axis([0 4 0 1]);
     text(0.8,rule l satisfaction+0.04,'Rule 1');
     text( 1.8,ru1e2_satisfaction+0.04,'Rule 2');
     text(2.8,ru1e3_satisfaction+0.04,'Rule 3');
     title('Fuzzy operation of the antecedent');
     xlabel('Rule number');
     ylabel('Degree of satisfaction in each antecedent');


===== PAGE 34 =====
                                                                                                        ］장 퍼지 이론   m

                                                                    Fuzzy operation of the antecedent




                                          O mm뇨口mD
                                                         4111




             H= mOmOmH= m =Omm 드 C으6m訪二mm H
                                                     0   8                        R미e2
                                                     1




                                                     0   八
                                                         0
                                                     1




                                                     0   d
                                                         1
                                                     1




                                                     0
                                                     ／
                                                     n                                        Ru旭 3
                                                     1   느



                                                         0            R미e ]
                                                                       1          2             3
                                                                              R미e number
                                                                ［그림 卜14] 봉사료 결정 규칙의 전건부 만족도




 이 그림은 음식을 먹은 고객이 service = 6, food = 6이라는 평가를 내렸을 때, 이 입력
데이터가 3개의 퍼지 규칙의 전건부를 만족시키는 정도（만족도）를 나타낸다．


(3) 함의(In）口lic計向n) 연산자 적용
 각 규칙어］ 서로 다른 가중치를 적용할 수 있는데 그 값은 0과 1 사이의 값을 갖는다. 함의
연산자를 적용하기에 앞서 규칙의 전건부 만족도어］ 가중치를 곱할 수 있다. 그러나 일반적으
로 가중치를 적용하지 않는뎨 이는 모든 규칙이 동일하게 중요하다고 생각하여 그 가중치를
1로 둔 것이다. 후건부의 퍼지 집합은 전건부 만족도에 의하1 그 모양이 변경된다. 함의 연산
자의 입력은 전건부 만족도인 수치이고 출력은 퍼지 집합이다. 함의 연산자는 모든 규칙에
적용된다. 함의 연산자로는 최소화（II丘n)와 곱하기（product）가 사용된다. 최소화는 전건부 규
칙의 만족도 값으로 후컨부 퍼지 집합을 잘라, 만족도 이하 부분의 후건부 퍼지 집합을 사용
한다. 곱하기는 후컨부 퍼지 집합에 만족도를 곱한 것으로 만족도가 1이면 변화가 없고 1 보
다 작으면 후컨부 퍼지 집합의 모양을 축소해서 사용하는 것이다．
 리스트 1-15와 그림 1-15는 봉사료 결정 규칙에서 함의 연산자를 적용하는 코드와 그 결
과를 보여준다. 여기서는 함의 연산자로 최소화를 사용하였다．


===== PAGE 35 =====
                                     率
     퍼지, 진화컴퓨팅 프로그래밍




mm 리스트卜］5. 봉사료 결정 규칙에 함의 연산자 적용 娜易璘娜驪蜘湃熙娜解

 % 파일명： fsets_implication.m
  service = 6;
 mu_poor = triangle(service,[0 1 4]);
 mu,good = triangle(service,[3 5 10]);
 mu_excellent = triangle(service,[5 10 111);
  food = 6;
 mu_rancid = trapezoidal(food,[0 1 2 4]);
 mu_delicious = trapezoidal(food,[5 9 10 11]) ;
 rule1_satisfaction = max(mu_poor,mu_rancid);
 ru1e2_satisfaction = mu_good;
 ru1e3_satisfaction = min(mu_excellent,mu_delicious);
 tip = 0:0.5:25;
 mu_cheap = bell(tip,[l 0]); % 규칙1의 후건부 피지 집합
 mu_average = bell(tip,[l 10]); % 규칙2의 후건부 퍼지 집합
 n世generous = bell(tip,[0.5 25]); % 규칙3의 후건부 퍼지 집합
 % 함의 연산자 적용如in 연산자 사용）
 mu_cheap = min(rule1_satisfaction,mu_cheap);
 mu_average = min(rule2_satisfaction,mu_average);
 mu_generous = min(rule3_satisfaction,mu_generous);
 plot(tip,mu_cheap,'b-',tip,mu_average,'k-',tip,mu_generous,'r-');
 axis([0 25 0 1]);
 title('Implied fuzzy sets: cheap, average, generous');
 text(1,0.1,'cheap');
 text(9,0.85,'average');
 text(2 l.5,0.1,'generous');
 xlabel('tip(%)');
 ylabel('membership');


===== PAGE 36 =====
                                                                                  1장 퍼지 이론   29



                                   Implied fuzzy sets: cheap, average, generous
                             1

                                                  average
                         0.8卜



                        0     0

                       으
                       ＝ m뇨mnEmE




                                   cheap

                                                   10            15   20          25
                                                        tip(%)
                         ［그림 1.15] 봉사료 결정 규칙에 함의 연산자 적용 결과



@) 출력 퍼지 집합 합하기（Aggregation)
 퍼지 추론 시스템에서는 모튼 규칙을 고려해서 최종 결정을 내리기 때문에 모든 규칙을 결
합하는 방법이 필요하게 된다. 출력 퍼지 집합을 합하는 것은 각 규칙의 후컨부에 함의 연산
자를 적용하여 얻어진 결과 즉, 전건부 만족도의해 변경된 후건부 퍼지 집합들을 합해서 하나
의 집합으로 만드는 것이다. 출력 변수가 하나가 아니면 합하기 과정은 출력 변수 별로 이루
어진다. 합하기 과정의 입력은 변경된 모든 후컨부 퍼지 집합들이고 출력은 이들을 합한 퍼지
집합이다. 합하는 순서는 상관이 없으며 합하기 연산자로는 최대화（n追功와 단순 더하기
(sum)가 주로 사용된다.
 리스트 1-16과 그림 1-16은 봉사료 결정 규칙에서 출력 퍼지 집합 합하기를 실행하는 코
드와 그 결과를 보여준다. 여기서는 max로 합하기를 하였다．


   리스트卜］6 毋 봉사료 결정 규칙에서 출력 퍼지 집합 합하71

  % 파일명： fsets_aggregation.m
  fsets_implication;
  % 함수      fsets_implication.m 실행 ->
                       퍼지 함의 연산자 적용
  % 퍼지 출력 변수 합하기（합하기 연산자 -> max 사용）
  mu中aggregation = max([mumcheap; mu_average; mu_generous]);
  plot(tip,muaggregation,'b-');


===== PAGE 37 =====
30         퍼지, 진화컴퓨팅 프로그래밍


       axis([0 25 0 1]);
       title('Aggregation of the implied output fuzzy sets');
       text(7,0.85,'the aggregated fuzzy set');
       xlabel('tip(%)');
       ylabel('membership');




                                     Aggregation of the implied output fuzzy sets
                                ]

                                               the aggregated fuzzy set
                             0.8



                            0    0
                                 八
                                 O




                           으듬bn드mE
                                 4




                            0.2



                                                    10            15                25
                                                         tip(%)
                       ［그림 1-16] 봉사료 결정 규칙에서 출력 퍼지 집합을 합한 결과



     (5) 비퍼지화（Defuzzification)
     비퍼지화의 입력은 출력 퍼지 집합을．합한 결과이고 출력은 이로부터 계산퇸 명확한 숫자
 이다. 합하기 결과로 얻어진 최종 퍼지 집합은 출력 변수 구간에 대해 정의되므로 출력으로
하나의 숫자를 얻기 위해서는 비피지화가 이루어져야 한다. 비피지화 방법에도 여러 가지가
있지만 가장 인기 있는 방법은 무게중심법（cen打아d）이다. 이 방법은 퍼지 집합의 무게중심어］
해당하는 변수 영역의 점（값）을 결정한다．
     무게중심을 구하기 위해서는 적분（출력 퍼지 집합의 면적 계산）을 해야 하지만 시간이 많이
걸리므로 출력 변수 영역에서 일정 간격으로 변수 값을 추출하여 사용한다. 출력 변수 영역에
서 추출된 모든 값어］ 대해 그 때의 출력 퍼지 변수 집합의 멤버쉽함수 값과 출력변수 값을
곱해서 더한 다음 이것을 멤버쉽함수 값의 합으로 나누어 계산한다. 가령, 출력 변수 영역이
0에서 25인데, 숫자 5 간격으로 추출했다고 하면 [0 5 10 15 20 25］가 추출된 변수 값이
된다. 이 변수 값어］ 대해 만족도어］ 의해 변경된 출력 퍼지 집합의 멤버쉽함수 값을 구한다．


===== PAGE 38 =====
                                                              ］장 퍼지 이론   m1
그 값이 [0.2 0.6 0.9 0.5 0］이라 하자. 이 때 무거］ 중심은 (0*0.2 + 5串0.5 + 10*0.9 +
20*0.5 + 25永0)/(0.2 + 0.6 + 0.9 + 0.5 + 0）으로 계산된다. 추출 간격을 작게 하면 적분에
의해 계산한 것과의 차이를 줄일 수 있다．
 리스트 1-17과 그림 1-17은 봉사료 결정 규칙에서 합해진 출력 퍼지 집합의 비퍼지화를
실행하는 코드와 그 결과를 보여준다．


    리스트卜］7 . 봉사료 결정 규칙에서 합해진 출력 퍼지 집합의 비퍼지화

  % 파일명： fse奴defuzz小cation.m
  fsets_aggregation;
  % 함수 fsets_aggregation.m 실행 -> 퍼지 출력 변수 합하기
  % 무게중심법에 의한 비퍼지화
  tip_value = centroid(tip,mu_aggregation);
  %ii如叩이曲on을 통한 自LV키此에서의 멥버쉽
  mu_tip_value = interp I (tip,mu_aggregation,tip_value)
  plot(tip,mu_aggregation,'b-',[tip_value tip_value],...
  [0 mu_tip_value],'r-');
  axis([0 25 0 1]);
  title('Defuzzification of the aggregated fuzzy set');
  text（먀느val出－2,mu먀_value+0.03,...
  ['tip = ' num2str(tip_value) '%']);
  text(tip_value-2.2,mu_tip_value-0.3,'center of area');
  xlabel('tip(%)');
  ylabel('membership');


              function [center] = centroid(x,y);
              % 무게 중심 계산
              % A]-용법: [center] = centroid(universe,grades)
              %             universe: 논리영역을 정의하는 행 벡터
              %             grades: 멤버쉽함수 값에 대응하는 행 벡터
              %             center: 무게 중심어］ 해당하는 명확한 값

              sun二느U = sum(y);
              if (sun그느U > 0)
                      center = (x*y')/sum(y);
              이se


===== PAGE 39 =====
m        퍼지, 진화컴퓨팅 프로그래밍



                   center = 0;
             end




                                Defuzzification of the aggregated fuzzy set
                         1


                      0.8


                           4
                      O
                      八
                      0    0

                     쇼三띤mnEmE


                       n
                       n

                                                             3.   2162

                                     5         10            15          20   25
                                                    tip(%)
                             ［그림 卜17] 봉사료 결정 규칙의 비퍼지화 결과



     위 그림에서 중앙 하단의 수직선이 출력 퍼지 집합의 무게중심에 해당하는 선이고 그 때의
    변수 값（tip=13.216）이 비피지화 즉, 퍼지 추론의 결과이다．
     입력과 출력 사이에 블랙박스가 있다고 하자. 즉, 블랙박스가 입력을 출력으로 변화시켜주
    는 기능을 한다고 하자. 블랙박스는 선형방정식（linear equation), 부분 선형방정식
    (piecewise linear equation), 비선형 방정식（noi亡linear equation) 또는 신경회로망
    (neural network）이나 퍼지 시스템（fuzzy system)과 같은 비선형 시스템으로 채울 수 있다．
    입력과 출력 사이의 변환 관계를 정의하는 시스템을 모델이라고도 한다. 위에 보인 봉사료
    문제에서 3개의 규칙이 바로 입력（service와 ／切d）과 출력（渤） 사이의 변환 관계를 정의하는
    블랙박스（모델）이라고 할 수 있다．
     리스트 1-18은 이 변환 관계를 보이기 위해 입력 변수 값들의 조합（매트랩의 mesh 형성）
    어］ 대해 출력을 계산하는 코드이고 그림1娼은 각 규칙의 만족도와 입출력 관계를 3차원으
    로 표시한 것이다．


===== PAGE 40 =====
                                                                        l장 퍼지 이론   4F=



雕珊豁 리스트卜］8 昏 봉사료 문저떽 Mamdani형 퍼지 규칙에서 추론

  % 파일명： fsets_tip_mamdani.m
  service = 1:0.2:10; % 입력 변수 설정
  food = service;
  tip = 0:0.5:25;% 출력 변수 설정
  % 전건부 멤버쉽 함수 값 계산
  mu_poor = triangle(service,[0 1 4]);
  mu_good =     triangle(service,[3 5 10]);
  mu excellent =    triangle(service,[5 10 11]);
  mu_rancid = trapezoidal(food,[0 1 2 4]);
  mu delicious = trapezoidal(food,[5 9 10 11]) ;
  % 후건부 멤버쉽 함수
  mu_cheap = bell(tip,[1 0]);
  mu_average = bell(tip,[1 10]);
  mu_generous = bell(tip,[0.5 25]);
  % 규칙의 전건부 만족도 계산
  [mesh_service,mesh_food] = meshgrid(service,food);
  [mesh_mu_poor,mesh_mu_rancid] = meshgrid(mu_poor,mu_rancid);
  rule1_satisfaction = max(mesh_mu_poor,mesh_mu_rancid);
  [mesh_mu_good,mesh_mu_goodc] = meshgrid(mu_good,mu_good);
  rule2_satisfaction = mesh_mu_good;
  [mesh mu excellent,mesh mu delicious] = meshgrid(mu_excellent,mu_delicious);
  rule3_satisfaction = min(mesh_mu_excellent,mesh_mu_delicious);
  % 후건부 멤버쉽 함수 값 계산
  [r,c] = size(mesh_service);
  tip_value = zeros(r,c);
  的r 卄l:r
       for j=1:（二
            % 규칙의 후건부에 함의 연산자 적용
            mu_im_cheap = min(rulel_satisfaction(ij),mu_cheap);
            mu_im_average = min(ru1e2_satisfaction(ij),mu_average);
            mu_im_generous = min(rule3_satisfaction(ij),mu_generous);
            % 후건부 퍼지 집합의 모음
            mu_aggregation = max([mu_im_cheap; mu_im_average;...
            mu_im_generous]);
            % 비퍼지화


===== PAGE 41 =====
口 ［ 퍼지， 진화컴퓨팅프로그래밍 ]
                tip_value(ij) = centroid(tip,mu_aggregation);
          end
    end
    surf(mesh_service,mesh food,tip value);
    axis([1 10 1 10 0 25]); view(235,60);
    title('Input-output relation');
    xlabel('service'); ylabel('food'); zlabel('tip(%)');




                                          Degree of satisfying the antecedent in rule 1




                          0
                                  d
                                  1 戶
                                    h
                                    U 0


                       Q三띤m스Em드                                                           10




                                                                            food
                                                service     10

                                                  (a) 규칙1의 전건부 만족도


                                          Degree of satisfying the antecedent in rule 2




                          0
                              d U 0
                              1 C
                              1

                       으듬늄쇼Em드                                                            10




                                               service

                                                  (b) 규칙2의 전건부 만족도


===== PAGE 42 =====
                                                                             j장 퍼지 이론



                             Degree of satisfying the antecedent in rule 3




                O
                    4
                    1
                    1=U 0
                      k

             q三띤mnEm드




                                                               food
                                  service      10

                                                           唾
                                     (c) 규칙3의 전건부

                                            tn
                                             0
                                             a
                                             e
                                             r
                                            tU
                                            P
                                            tU
                                             0
                                            t
                                            1
                                            DU
                                             n                               1




                   n<   0

                翁V읖
                  41
                        0


                  41
                        00




                                service                      food


                                  (d) 퍼지 규칙어］ 의한 입출력 관계
      ［그림 卜］8] 봉사료 문제의 Mamdani형 퍼지 규칙에서 입력 변수 값에 대한 추론 결과



 입력과 출력변수 사이의 비선형 관계를 기술하는 3개의 피지 규칙이 위 그림（d）와 갇은 비
선형 곡면을 정의한다. 이처럼 퍼지 시스템은 적은 수의 규칙을 가지고도 입출력 사이의 비선
형이고 복잡한 관계를 기술할 수 있기 때문어］ 비선형이고 복잡한 시스템을 모델링 할 때 유용
하다．


===== PAGE 43 =====
36        퍼지, 진화컴퓨팅 프로그래밍




 1.4.2 Sugeno형 퍼지 규칙에서의 추론
      앞서의 봉사료 결정을 위한 M帥idani형 퍼지 규칙에서 후건부는 퍼지 집합이지만 Sugeno
 형의 퍼지 규칙에서는 후컨부가 선형 방정식이다. 즉, Sugeno형 퍼지 집합은 아래와 같은
 형태를 취한다． 口，7는 선형 방정식을 결정하는 계수로 실수이며， ／는 규칙번호를 ／는 입력

 변수어］ 대한 인덱스이다. 후컨부에 계수 口, l만이 존재하고 나머지가 0이면 후건부가 퍼지 싱

 글톤佃ingle) 즉, 상수인 경우이다．


      R': If service iS 加or or food is rancid

                               then ／功＝口10+ 口11 · ser沅ce+ 口12 · food.

      R2: If service is good then 渤＝口20 + 口21 · service+ a22 · ／切（/.

      R3: If service is excellent and food is delicious

                                then tip = a3。+ a31 · service + a32 · food.



 이상과 같은 퍼지 규칙으로부터 추론 결과를 계산하는 방식어］ 대해 알아보자. 앞 절에서 설명
 한 (D 피지화, （今 퍼지 연산자 적용은 동일하며, 여기서는 차이가 나는 이후 단계만을 설명한
 다．
      （今 만족도의 정규화
      단계＠를 통해 얻어진 규칙의 전건부 만족도는 식（1.16）어］ 의해 정규화 된다．



                功r몸
                   Z
          功
                                                                              (1.16)   1




                   功




      여기서 Z抄，는 각 규칙의 전건부 만족도, ／는 규칙 번호, 1은 전체 규칙 수를 표시한다. 봉사
 료 결정 규칙에서 r= 3이다．


      @) 후건부 선형식 계산
      식（1.17）과 같이 각 규칙의 후컨부 선형식에 입력 값（抑，尤2' "·' 抑의 값）을 대입하여 선형


===== PAGE 44 =====
                                                      ］장 퍼지 이론     -F-

식 값을 계산한다．


   yi=   a刃＋口il ' 兀l + a i2 ' 尤2+ ' " + a旒 ' 父七                  (1.17)


／는 규칙 번호， 兀는 퍼지 규칙의 입력 변수， 七는 입력 변수의 수， 功는 i번째 규칙의 후건부

값이다. 봉사료 결정 규칙에서 입력 변수 自은 service이고 兀2는三 加d이므로 月는 2이고 y는

渤이다．


 (5) 최종 출력 계산
 최종 출력은 식（1.16）의 정규화한 만족도와 식（1.17）의 후컨부 선형식 값을 이용해서 식
(1.18）과 같은 산술 연산어］ 의해 계산된다．



          r2=
    片           功                                                (1.18)
                    yi




y는 최종 추론 값, yi는 i번째 규칙의 후건부 선형식 값, w，는 정규화퇸 ／번짜1 규칙의 전컨
부 만족도 값이다．




                                          연습문저1 書 ,




 [1] 본문어］ 제시된 봉사료 퍼지 규칙의 후건부를 Sugeno형의 선형식으로 변경한다. 이 때
   후건부 계수 a,0은 0에서 20 이내의 값을，규칙1의 떠-]- a2는 -1에서 1 사이의 값을，

   규칙2와 3의 a*15} a,2는三 0에서 1 사이의 값을 갖도록 임의로 정한다. 리스트 卜18어］

   서와 같이 입력 변수어］ 대한 봉사료를 추론하는 코드를 작성하고 퍼지 규칙이 기술하는
   입출력 관계를 알아보자．
 [2] 문제1에서 후건부를 퍼지 싱글톤（실수）로 변경한다. 유일한 후컨부 계수인 a0은 0에서

   25 사이에서 임의로 정한다. 리스트 1-18에서와 같이 입력 변수어］ 대한 봉사료를 추론
   하는 코드를 작성하고 퍼지 규칙이 기술하는 입출력 관계를 알아보자.


===== PAGE 45 =====
口m[ 퍼지
     ，진화컴퓨팅프로그래밍
                                簪 심화 학습 자료 轟


  'E. H. Mamdani, "Applications of fuzzy algorithms for control of simple dynamic
   plant," Proc. lEE Vol. 121, No. 12, pp. 1585-1588, 1974.
  'R. M. Tong, "The evaluation of fuzzy models derived from experimental data,"
   Fuzzy Sets and Systems, Vol. 13, pp. 1-12, 1980.
  'T. Takagi, and M. Sugeno, "Fuzzy identification of systems and its applications
   to modeling and control," IEEE Trans. on SMC, Vol. 15, No. 1, pp. 116-132,
   1985.
  'J. A. Bernard, "Use of rule-based system for process control," IEEE Control
   System Magazine, Vol. 8, No. 5, pp. 3-13, 1988.
  'X. T. Peng, S. M. Liu, T. Yamakawa, and P. Z. Wang, "Self-regulating fuzzy PID
   controllers and its application to a temperature controlling process," Fuzzy
   Computing, North-Holland, Amsterdam, 1987.


===== PAGE 46 =====
CHAPTER 2   퍼지 클러스터링




             守， 2.1 하드（Hard C-Means) 클러스터링
             堪｛; 2.2 FCM(Fuzzy C-Means) 클러스터링
             ：衣：2.3 분할의 타당성 평가


===== PAGE 47 =====
                                                 2장 퍼지 클러스터링   41




  多 클러스터링（clustering）은 적은 수의 파라미터를 가지면서도 데이터의 특성을 매우 빨리 파악할
  수 있게 해주기 때문어］ 패턴인식, 영상처리 , 데이터마이닝 등의 응용 분야에서 분류, 예측 또는
  제어 용도의 규칙을 유도하는데 널리 사용되고 있다. 이 장에서는 퍼지 클러스터링이 무엇인지 알
  아보고 이를 매트랩으로 프로그래밍 하는 것을 배운다. 5장의 퍼지 규칙 생성에서는 퍼지 규칙의
  구조를 파악’
        '陪 어떻게 퍼 ' ] 클러스터링 " ] 응용될 수 있는' ］를 "fi울 것' ］다" 99




Fuzzy & Evolutionary
   Computing Pro아帥ming   L 1
                          2.
                               하드
                                    （Hard
                                            아Means) 클러스터링


 클러스터링은 데이터에 존재하는 구조를 찾아내어 이들을 그룹화 하는 방법이다. 가장 흔
히 사용되는 클러스터링 방법은 유사한 데이터는 동일 클러스터어］, 유사하지 않은 뎨이터는
서로 다른 클러스터에 속하도록 데이터 집합을 몇 개의 클러스터（클래스）로 분할하는 것이다．
현실 문제에서는 분할된 클러스터들 사이의 경계가 분명치 않은 경우가 종종 발생하는데, 이
경우 퍼지 클러스터링이 적합하다. 퍼지 클러스터링은 0과 1 사이의 멤버쉽 값을 사용하여
데이터가 여러 클러스터에 속한 정도를 표시할 수 있다. 반면에 클러스터링은 데이터가 반드
시 하나의 클러스터에 속해야 한다. 속하면 멤버쉽이 1이고 속하지 않으면 0이다. 이는 전통
적인 집합 개념과 동일하다. 퍼지 클러스터링에 대비해 이를 하드 클러스터링이라 한다．


 다음 사례를 통해 클러스터링이 어떻게 활용되는지 보자. 아래와 같은 차량 데이터를 클러
스터링하면, 데이터어］ 내재된 구조에 따라 그림 }1과 같이 3개의 클러스터（클래스： 트럭，
중간 가격대 차량, 人平文 카）로 분할된다. 이로부터 특정한 차량의 무게와 최고 속도를 알면
이것이 어떤 클래스어］ 속하는지 판단할 수 있으며 , 역으로 특정 클래스를 규정하는 특성이
무엇인지도 알아낼 수 있다. 이런 정보는 패턴분류, 인식, 데이터마이닝 등의 분야에서 유용
하게 사용된다.


===== PAGE 48 =====
m       퍼지, 진화컴퓨팅 프로그래밍




                                                   차량 뎨이터

                             Vehicle   Top speed   Colour    Air          Weight
                                       kmlh                  resistance   Kg
                             VI        220         red       0.30         1300
                             V2        230         black     0.32         1400
                             V3        260         red       0.29         1500
                             V4        140         gray      0.35         800
                             V5        155         blue      0.33         950
                             V6        130         white     0.40         600
                             V7        100         black     0.50         3000
                             VS        105         red       0.60         2500
                             V9        110         gray      0.55         3500



                           3500


                           300


                           2500




                    弓巴曲m
                           2000


                           1500


                           1000


                            500
                               100           15'         200              250      300
                                                   최 고 속도 [km(h]


                           ［그림 午1] 차량 데이터의 하드 클러스터링 결과


     71개의 항목으로 구성된 데이터 집합 X=｛石,石,···,兀｝을 C개의 클러스터로 분할하고자 할
    때 하드 클러스터링은 식（2.1）의 목적함수를 최소화하는 분할（클러스터） 肛 伍i,曳,···,!,｝를

    찾는 것이 목적이다．



      'Jm(U, V: -7) = EZ ( k)mIIxk_ vHI2                                                           (2.1)



    이 식에서 L느 (v1, v2, ..., 阮）는 C개의 클러스터의 중심 벡터 집합이다. 즉, g는 0번째 클러
    스터의 중심 벡터（centroid）이다. 卄大, - V II 은 데이터 兀와 2번째 클러스터의 중심과의 기하
    학적個uclidean) 거리를 나타낸다.                     k와 m의 차원이 p이면                       q = (vj1,v뇨2,···,iJi力이고


===== PAGE 49 =====
                                                                           2장 퍼지 클러스터링     1=F=


瓜＝ 佃枷x枕，' " ,2枷）이다. 매개변수 m은 데이터가 클러스터어］ 속하는 정도를 조정하는

값으로 하드 클러스터링의 경우 1이다. /／旒는 데이터 丕가 클러스터 且어］ 대하여 속하는 정도

를 나타내는 것으로 0 또는 1 가운데 하나의 값을 가지며， (cx n) 크기의 분할 행렬 [/=［咽
의 원소로 식（2.2）의 조건을 만족한다. 특정한 데이터가 모든 클러스터에 속하는 정도를 합하
면 1이어야 하므로, 데이터는 하나의 클러스터에만 속해야 한다．


   PikE {O,1},)k= 1                                                                      (2.2)


하드 클러스터링 알고리즘을 정리하면 다음과 같다．

 d) 분할 수 c (2 드 c 드 n）와 분할 행렬（데이터가 각 클러스터어］ 속하는 정도） 口(t) - H的의
  초기값을 선택한다．
 (2) C개의 클러스터의 중심 벡터 V를 식（2.3）을 결정한다．

                                    X
                              "f)
                                                                                         (2.3)
                          (
        1)
                                        '                              c
   才+        =   k=   1
                                                           .   "




                      몸畔）
                                            i=   1,
                                                      2,           ,
 區） 식（2.4）를 사용해서 분할 행렬을 갱신한다．
   . 七+1) (v\ - fl if I 14- 六i 1 = 77li71l 드 i < . 1 I/ 寸大i 1
   尸士 나kJ Hl00坑ert尻se
   i= 1,".,c k= 1,.",n                                                                   (2.4)

 @) 1 少t+1) _(J(t) 1 < d을 만족하면 이 과정을 종료하고 그렇지 않으면 區） 단계로 복귀해서
  이 과정을 반복한다. 통상 o 값으로 1o3을 사용한다．


 단계（D에서 초기값으로 분할 행렬 값 대신 클러스터의 중심 벡터를 선택할 수 있다. 이 때
에는 단계＠와 단계＠의 순서가 바뀌면 된다. 이들의 초기값어］따라 클러스터링 결과가 달라
질 수 있기 때문어］ 효과적으로 초기값을 선정하는 방법은 클러스터링을 연구하는 분야 가운
더］ 하나이다．


표 2.1어］ 주어진 나비（Butterfly) 데이터 집합에 대해 하드 클러스터링을 수행해서 데이터를
어떻게 그룹화할 수 있는지 보자. 리스트 2.1은 이를 위한 매트랩 코드이다．


===== PAGE 50 =====
                                       琡
44       퍼지, 진화컴퓨팅 프로그래밍




                    ［표 2.1] 나비 데이터 집합

                        번호（k)       데이터 : 佃，y)    번호（肋   데이터 : 佃，y)

                            1          (0,0)       9        (4,2)
                            2          (0,2)       10       (5,1)
                            3          (0,4)       11       (5,2)
                            4          (1,1)       12       (5,3)
                            5          (1,2)       13       (6,0)
                            6          (1,3)       14       (6,2)
                            7          (2,2)       15       (6,4)
                            8          (3,2)




       리스트 2니 蜘 나비 데이터의 하드 클러스터링

     % 파일명： hcmc clustwer血g.m 하드 클러스터링 데모
     dlc; % 매트랩 코맨드뷰 화면 지우기
     elf; % 그림 창 내용 지우기
     eps = 1.e-3; % 종료조건
     C = 2; % 분할（클러스터） 수
     load butterfly.dat; % 데이터 파일（2 x15, 2 차원, 15 데이터） 읽기
     [n,d] = size(butterfly); % d: 차원， n: 뎨이터 수
     [UO] = initFcmc(c,butterfly); % 분할행렬의 초기치 설정
     % 하드 클러스터링 실행
     [U,V,iter] = hcmc(eps,UO,butterfly);
     x = 1:1:n; % 가로축 변수
     plot(x,U(1,:),'r-'); %
     h아d on;
     plot(x,U(2,:),'b-');
     xlabe!('Data number');
     ylabe!('Membership values');
     axis([1 n 0 1.1]);


                 function [UO] = initFcme(c,X);
                 % 함수명： initFcmc.m
                 % 하드 및 퍼지 클러스터링에서 분할 행렬의 초기화
                 % 사용법： RiO] = initFcmc(X);


===== PAGE 51 =====
                                            2장 퍼지 클러스터링   45



%             출력변수
%             U0: 분할행렬 초기 값
%             입력변수
%             C: 클러스터의 수
%             X: （뎨이터 수 nx 차원 d）인 뎨이터 행렬


[d,n] = size(X'); % d: 차원（입력변수 + 출력변수）,n: 데이터 수
% UO를 랜덤하게 초기화
tmp = rand(c,n); % [0,1] 사이의 랜덤 값
UO = zeros(size(tmp)); % U0를 0으로 초기화
for i=1:c
      UO(i,:) = tmp(i,:)./sum(tmp); % 정규화
end




% 하드 클러스터링： 이 함수는 종료조건 eps, 초기 분할 행렬 U0와
% 뎨이터 x를 인수로 벋아 데이터 x어］ 대해 C개의 분할을 수행한다．
% Aj용법: [U,V,iter]=hcmc(eps,UO,X)
%            UO: c x n 크기의 초기 분할 행렬
%             X: nxd 크기의 데이터 벡터（d: 뎨이터 차원）
%             U: cxn 크기의 최종 분할 행렬
%             V : dxc 크기의 클러스터 중심 벡터
%             iter: 종료조건을 만족할 때까지 반복 계산 횟수


tmp = X';
X = tmp; % d x n 크기의 데이터 벡터로 전치
% 초기화
[c,n] = size(UO); % 분할 클러스터의 수 C와 데이터 수 n의 계산
[d,nn] = size(X); % 데이터의 차원 d 계산, n과 nfl의 값은 동일
loop_cond = eps; % 종료 조건 확인에 사용
iter = 0;
U = UO;
VO = zeros(size(X)); % 분할 클러스티의 중심 벡터를 0으로 초기화
小st = zeros(c,n); % 거리 계산에 사용
while ( loop_cond >= eps )
      iter = iter + 1;


===== PAGE 52 =====
                                     求
.函口   퍼지, 진화컴퓨팅 프로그래밍



               Uo = U;
               tmp = sum(UO'); % 클러스터별로 모든 데이타의 분할 행렬 값의 합
               % 클러스터 중심 계산
               V = x시JO1;
               for i=1:c
                     V(:,i) = V(:,i)/tmp(i); % 클러스터 중심 계산
               end
               for i=1:c
                     for j=1:d
                           % 클러스터 중심벡터를 데이터 x와 동일 차원으로 만듦
                             VO(j,:) = V(j,i)*ones(1,n);
                       end
                       tmp2 = X - VO;
                       tmp2 = tmp2.*tmp2;
                       dist(i,:) = sum(tmp2); % 클러스터 중심과 데이터와 거리
               end
               % 새로운 분할 행렬 계산
               % mnd: 각 클러스터어］ 거리가 가장 가까운 데이터 인덱스를 찾음
               [minv,ind] = min(dist);
               U = zeros(c,n); % 모튼 소속 정도를 0으로 만듦
               for k=1:n
                      % 뎨이터가 가장 가까운 클러스터어］ 속하는 정도를 1로 바꿈
                      U(ind(k),k) = 1;
               end
               loop_cond = max(max(abs(U-UO))); % 종료조건 계산
         end
         % 종료조건이 만족 된 후 최종적인 클러스터 중심 계산
         tmp = sum(U');
         V = X*U1;
         for i=1:c
               V(:,i) = V(:,i)/tmp(i);
         end


===== PAGE 53 =====
                                                                                          2장 퍼지 클러스터링   m

 그림 }2는 나비 데이터의 하드 클러스터링 결과이다. 왼쪽 그림은 데이터의 분포를, 오른
쪽 그림은 데이터가 2개의 클러스터（그룹）로 분할된 것을 보여준다. 그림에서 중앙에 있는
데이터는 왼쪽 클러스터에 속한 것으로 되어 있다. 실제는 양 클러스터 중심까지의 거리가
같기 때문어］ 왼쪽과 오른쪽 클러스터 모두어］ 동일한 정도로 속해야 한다. 즉, 하드 클러스터
링은 데이터가 어느 한 클러스터어］ 완전히 속한 것으로 처리하기 때문에 특정 데이터가 어느
클러스터어］ 속해야 하는지 애매한 경우 이를 처리하지 못한다.


     (0.
      . 4)


             (1,3)                              (5,3)
              S                                  S
     (0.2    {1.2 J (2.2) (3.2) (4,2) (5.2) (6.2>
              S      S              S       S    1        S
             (1.1)                              { 5그 J
              S                                  1
                                                         (G. 01
                                                          S


                                 ［그림 午2] 나비 데이터의 하드 클러스터링 결과



 그림 2-3을 보면 1-7번까지의 데이터와 小15까지의 데이터가 서로 다른 클러스터어］ 속
함（소속정도가 1）을 알 수 있다．



                                4


                             8
                             0



                             6     4

                             0     0


                         m
                         m=m
                           m
                           ＞ 프二m늉스E山돋




                           0.2



                               0
                                        2         4           6         8       10   12   14
                                                                  Data number



 ［그림 十3] 나비 데이터의 하드 큘러스터링 결과（데이터가 클러스터에 속하는 정도, 멤버쉽 값）


===== PAGE 54 =====
m        퍼지, 진화컴퓨팅 프로그래밍




          蕃 Ev이Ut油na印
       Corn群.1妊n曾戶ro硏카nfl出lg    2.2 FCM(Fuzzy 口Means) 클러스터링



     일반척으로 퍼지 클러스터링은 데이터를 그룹화하기 위한 무감독 학습전략（uns叩ervised
    learning strategy）으로 사용되지만, 데이터로부터 피지 규칙（if N then -）을 생성할 때에도
    유용하게 사용된다（5장에서 다룸）. 퍼지 규칙의 구조는 사용한 데이터의 특성어］ 따라 달라진
    다. 가령 , 고장진단이나 패턴분류에서는 데이터가 어떤 클러스터（클래스）로 분류되어야 하는
    지를 결정하도록 퍼지 규칙이 만들어지고 퍼지 제어 , 시스템 인식이나 함수 근사화에서는 입
    출력 변수들 사이의 연속적인 관계를 기술할 수 있도록 만들어진다. 이미지 분석이나 인식어］
    서는 원이나 타원과 같은 공간상의 기하학적 형체를 감지하고 분리하는데 사용되며 , 이를 쉘
    (shell) 클러스터링 알고리즘이라 부른다.
     퍼지 클러스터링의 목적은 임의의 데이터 집합을 특정한 수의 퍼지 클러스터로 분할하는
    것이다. 현재까지 가장 널리 사용되고 있는 퍼지 클러스터링 방법은 F（弧4 알고리즘이다. 이
    알고리즘은 Ti개의 항목으로 구성된 데이터 집합 x=｛石, 大；, ···.. 大；,｝을 C개의 퍼지 클러스터로
    분할하고자 할 때 식（2.1）의 목적함수를 최소화하는 퍼지 분할 != ｛且, 良,. ·『．戶,｝를 찾는 것이

    목적이다. 하드 클러스터링과는 매개변수 m과 퍼지 분할 행렬의 값에 차이가 있다. 분할의
    애매함（fuzziness）을 표시하는 매개변수인 m은 1 보다 큰 값을 가질 수 있는데, 이 값이 클
    수록 모호함이 높아진다（Tn이 1인 경우는 애매하지 않는 명확한 하드 클러스터링을 표시）.
    m의 값은 일반적으로 1 25나 2가 좋은 결과를 제공하는 것으로 알려져 있지만, 응용 분야어］
    따라 적합한 m의 값을 선택할 수 있다. ／奴는 데이터 兀가 퍼지 클러스터 t，어］ 대하여 속하는

    정도를 나타내며， (c x n) 크기의 피지 분할 행렬 u= [mI의 원소로 식（2.5）의 조건을 만족한
    다. 특정한 데이터가 모튼 클러스터에 속하는 정도를 합하면 1이 되는 것은 하드 클러스터링
    의 경우와 동일하다．



       /1mE [0,1 ], ＞그／까k = 1                                 (2.5)



     FCM 클러스터링 알고리즘을 정리하면 다음과 같다．
     (D 분할 수 c (2 드 C 드 n）와 m의 값을 선택한다．


===== PAGE 55 =====
                                                                     2장 퍼지 클러스터링           49


（多 퍼지 분할 행렬 {y(t)의 초기값을 결정한다. 통상 식（2.5）를 만족시키는 랜덤 값을 사용한
   다．
（多 식（2.6）를 이용하여 클러스터의 중심 V를 계산한다．

                "
        才*，드 몸（""')" ,                                                             (2.6)
              Ei4
 E4) 식（2.7）을 사용해서 퍼지 분할 행렬을 갱신한다．
        m1
         尤
                        1             可 == 1. " ··下   H 1
                                                            k = 1,                 (2.7)
             寸'II 呼- T ', ) 1/(m-1)
             勺八 IA七尸1 匕 I ')

 (5) I [/{t+1) 中 (J{t) I <a을 만족하면 이 과정을 종료하고 그렇지 않으면 단계＠로 복귀해서
   이 과정을 반복한다. 통상 '5 값으로 iD-3을 사용한다．


이상의 알고리즘을 매트랩 코드로 만든 것이 리스트22이다. 퍼지 지수 m이 1.25와 2일
때의 클러스터링 결과를 그림으로 표시한 것이 그림 牙4- 그림 }6이다. 이 그림에서 보면
퍼지 지수 m이 증가할수록 분할된 클러스터의 애매함（중첩성）이 증가함을 알 수 있다．


mm 리스트卜2          4 FCM 클러스터링 코드


  % 파일명 fcme_clusiering.m 퍼지 클러스터링 데모
  dc; % 매트랩 코맨드 뷰 화면 지우기
  elf; % 그림 창 내용 지우기
 m = 1.25; % 퍼지 지수(m> 1)
  eps = 1.e-3; % 종료조건
  c = 2; % 퍼지 분할（클러스터） 수
  load butterfly.dat; % 데이터 파일（2 x15, 2 차원, 15 데이터） 읽기
  [n,d] = size(butterfiy); % d: 차원， n: 데이터 수
  [UO] = initFcmc(c,butterfly); % 분할행렬의 초기치 설정
  [1工V永en] = fcmc(m,eps,UO,butterfly); % 퍼지 클러스터링 실행
  x = l:1:n; % 그림의 가로축 변수
 plot(x,U(1,:),'r-');
 hold on;
 미叫＼U(2,:),'b-'上
  xlabel('Data number');


===== PAGE 56 =====
50       퍼지, 진화컴퓨팅 프로그래밍



     ylabel('Membership values');
     axis([1 fl 0 1.1]);


                function [U,V,iter] = fcmc(m,eps,U0,X)
                % FCM 클러스터링： 이 함수는 퍼지 인텍스 m, 종료조건 eps,
                % 초기 분할 행렬 U0와 데이터 x를 인수로 벋아 뎨이터 x어］
                % 대해 C개의 퍼지 분할을 수행한다．
                % AJ용법: [U,V,iter]=fcm(m,eps,U0,X)
                %             UO: c x n 크기의 초기 분할 행렬
                %             X: nxd 크기의 데이터 벡터（d: 데이터 차원）
                %             U: cxn 크기의 최종 분할 행렬
                %             V: dxc 크기의 클러스터 중심 벡터
                %             iter: 종료조건을 만족할 때까지 반복 계산 횟수


                tmp = X';
               X = tmp; % d x n 크기의 뎨이터 벡터로 전치
               % 초기화
                [c,n] = size(UO); % 분할 클러스터의 수 C와 데이터 수 n의 계산
                [d,nn] = size(X); % 데이터의 차원 d 계산, n과 nfl의 값은 동일
               mindist = 1.0e-50; % 클러스터 중심어써 데이터의 최소 거리
                loop_cond = eps;
               iter = 0;
               U = UO;
                VO = zeros(size(X));
               tmp = zeros(c,n);
               dist = tmp;
               tmp2 = VO;
                while ( loop cond >= eps )
                      iter = iter + 1;
                      UO = U;
                      tmp = U0．八m; % 분할 행렬 원소의 계승 쳬산
                      % 클러스터별로 모든 데이타의 분할 행렬 값의 합
                      ttmp = sum(tmp');
                      % 식（2.6）의 클러스터 중심 계산
                      \/ = X*tmp';
                      for i=1:c
                             V(:,i) = V(:,i)/ttmp(i); % 클러스터 중심 계산


===== PAGE 57 =====
                                                               2장 퍼지 큘러스터링



      end
      for i=1:c
             for j=1:d
                  % VO를 x와 차원이 같게 만듦
                         VO(j,:)=V(j,i)*ones(1,n);
             end
                   tmp2 = X - VO;
             tmp2 = tmp2.小tmp2;
      dist(i,:) = sum(tmp2); % 클러스터 중심과 뎨이터와 거리
      end
      % 클러스터 중심과 뎨이터와의 거리가 최소 거리 보다 작은 뎨이터를
      % 짖아 최소 거리로 설정， 이는 새로운 분할 행렬을 계산할 때
      %o으로 나누어지는 것을 방지
      i= find(dist < min_dist);
      dist(i) = dist(i) - dist(i) + mindist;
      % 식（2.7）의 새로운 분할 행렬 계산
      的r 卄1:c
            U(i,:) = 1.! ((dist(i,:)./sum(dist))八(1/(m-1)));
      end
      % 데이터가 모든 클러스터어］ 속하는 정도의 합을 l로 만듦
      sumU = sum(U);
      for i=1:c
            U(i,:) = U(i,:)./sumU;
      end
      loop_cond = max(max(abs(U-UO))); % 종료조건 졔산
end
% 종료조건이 만족 된 후 최종적인 클러스터 중심 계산
tmp = U．八nl;
仕nlp = sum(tmp');
\/ = x차mp';
白r i=1:c
      V(: ,i) = V(:,i)/ttmp(i);
end


===== PAGE 58 =====
                 퍼지, 진화컴퓨팅 프로그래밍




                   1                                               ()                             0                                            1
                   1                                               S                              S                                            .
                            1                            0                                                 ()                          1
                            .                            S                                                 .                           S
                   1        1         1    0.5    0      0         0                              0        0      0   0.5    1         1       1
                   S        S         S     S     I      0         S                              1        I      I    S     S         1       S
                            1                            0                                                 0                           1
                            S                            S                                                 S                           S
                   1                                               U                              0                                            1
                   I                                               S                              1                                            .

                       (a) 왼쪽 클러스터에 속한 정도                                                         (b) 오른쪽 클러스터어］ 속한 정도

                                          ［그림 午4] 나비 데이터의 퍼지 클러스터링(m = 1.25)


                  0.87                                            U. 13                       0.13                                            0.87
                   .                                               S                           I                                               1



                            01 l1
                                                        01 01
                                只口                           夕b
                                                                                                                                  0.
                                                                                                                                       . 95


                                                        0
                       恤
                                                                                                      띵5
                                     0.88 0.5 0.12       0        0.03                        0.03          01
                                                                                                            0    0.12 0.5 0.88         1l1    0.97
                   S        e         I    S   I         I         S                           1           .      I    1   1           1       .
                           0.95                         0.05                                          0.05                       0.95
                            .                            S                                             S                          S
                  0.87                                            0.13                        1).13                                           U.87
                   I                                               S                            S                                              S

                   (a) 왼쪽 클러스터에 속한 정도                                                             (b) 오른쪽 클러스터어］ 속한 정도

                                          ［그림 午5] 나비 데이터의 퍼지 클러스터링（m= 2)



하드 클러스터링 결과와 달리 위 그림에서는 정 가운데에 있는 뎨이터가 양쪽의 클러스터
어］ 반씩（소속정도 0.5) 속해 있음을 보인다. 이는 당연한 결과이다．




     8
     0
       1




     6      4




                                                                             g= 1
                                                                                m＞ 二三면띠스Em玉
     0      0
       1
                                                                                              吐




 召므m＞ 스三띤山스E山든
       1
                                                                                              M




    0.2




                                             8     10     12            14                                                   8     10          12    14
                                       Data nun止片r                                                                     Data number



                       (a) m= 1.25인 경우 멤버쉽 값                                                                    (b) m= 2인 경우 멤버쉽 값
                                              ［그림 午6] 나비 데이터의 퍼지 클러스터링


===== PAGE 59 =====
                                            2장 퍼지 클러스터링    m

 하드 클러스터링에서 언급한 것처럼 단계d）에서 초기값으로 분할 행렬 대신 클러스터의 중
심 벡터를 선택할 수 있으며, 이 때 단계＠과 단계＠의 순서가 바뀐다. 일반적으로 FCM 알고
리즘은 잘 동작하지만 클러스터 모양이 구형（spherical)으로 제한되기 때문어］ 뎨이터가 편중
되게 분포하거나 밀도가 다른 경우 문제를 일으킬 수 있다. 이런 문제를 해결한 것이
Gustafson-Kessel 알고리즘인뎨, 이는 데이터 특성어］ 따라 기하학적 모양이 서로 다른 클
러스터를 검출할 수 있도록 FCM 알고리즘을 확장한 것으로 자세한 것은 참고문헌을 보기
바란다．




 클러스터링 알고리즘은 퍼지 분할 행렬 또는 클러스터의 중심（centroid）의 초기 값을 설정
（둘 가운데 하나를 선택하1 사용하는데 본 책에서는 전자를 사용）하는 문제 때문에 최적의 분
할 결과를 얻는데 어려움이 있다. 대부분의 클러스터링 알고리즘은 퍼지 분할 행렬이나 클러
스터 중심에 대한 초기 값을 무작위로 선정하는데, 이런 초기 설정이 클러스터링 결과어］ 영향
을 미친다. 즉, 초기 설정을 변경하면 클러스터링 결과가 달라질 수 있다. 따라서 , 퍼지 클러
스터링의 결과로 분할이 이루어지면, 분할의 타당성을 측정하는 방법이 필요하게 된다. 측정
방법으로 타당성 평가척도佃alidity inde功가 사용된다. 미지의 데이터를 몇 개로 분할해야
할지 모르는 경우어］ 이 척도를 사용하면 최적의 분할 수（퍼지 클러스터의 수）를 구할 수 있다．
 지금까지 다양한 퍼지 클러스티 평가척도가 제안되어 왔다. Bezdek은 분할꼐수와 분할 엔
트로피를 이용하는 평가척도, Xie와 Beth는 클러스터의 조밀성（compactness）과 분리성
佃eparation)어］ 기초한 평가척도를（식（2.8)), Fukuyan追와 Sugeno는 클러스터 내부의 조밀
성과 클러스터 중심과의 거리를 이용하는 평가척도를（식（2.9)), Rezaee는 클러스터 내부의
분산과 거리 함수를 결합한 평가척도를, Zahid는 퍼지 합집합과 교집합을 이용하여 피지 조
밀성과 퍼지 분리성을 계산하는 평가척도를 제안하였다. 최적의 퍼지 클러스터링은 최종 클
러스터들이 조밀하고 이들의 분리성이 높아 서로 중첩되는 부분이 최소인 것을 말한다．


===== PAGE 60 =====
U區口    퍼지, 진화컴퓨팅 프로그래밍




             ZZ峨 1 兀_ 1二 I 2
      "",' 亡：；三，
              y k- H尸
                               m> 1   i 7Ej               (2.8)



  여기서 C는 클러스터 수, n은 데이터 수, m은 퍼지 지수이다．

      蜘In 宕完峨（나imk 1' H 1 mi1")                           (2.9)



 여기서 i는 x의 평균 벡터이다．
  식（2.8）의 평가척도에서 분자 항은 클러스터의 수가 증가함어］ 따라 단조감소하기 때문어］ 클
 러스터의 압축성을 평가하는데 문제가 있고, 분모 항은 클러스터 중심 간의 거리만을 사용하
 기 때문어］ 클러스터들의 분리성을 효과적으로 판정하지 못한다. 식（2.8）의 평가척도를 사용
 할 경우 척도의 값어］ 차이가 크지 않다면 보다 적은 클러스터 수를 최적 분할로 결정해도 된
 다. 식（2.9）도 식（2.8）과 유사한 특성을 보인다.
  리스트 23은 식（2.8）의 평가척도를 이용하여 나비 데이터의 최적 퍼지 분할을 결정하기 위
 한 코드이다. 클러스터 수를 2에서 10까지 1씩 증가시키면서 퍼지 클러스터링을 수행하고
 분할 평가척도를 계산한다. 그 결과가 그림 牙7이다. m= 1.25일 때 최적 퍼지 분할 수는
 2가 된다.


      리스트 2-3 亡 평가척도 5加．,，릍 이용한 퍼지 분할 평가 코드

   % 파일명： measure小Sxb.m, 피지 분할 평가 데모
   clear; % 변수 삭제
   dc; % 매트랩 코맨드뷰 화면 지우기
   cif; % 그림 창 내용 지우기
   cmax = 10; % 최대 퍼지 분할 수
   cmin = 2; % 최소 퍼지 분할 수
   m = 1.25; % 퍼지 지수（m > 1)
   eps = l.e-3; % 종료조건
   load butterfly.dat; % 뎨이터 파일（2 x15, 2 차원, 15 데이터） 읽기
   [n,d} = S切e(butterfly); % d: 차원， n: 뎨이터 수
   sxb = ones(cmax,1); % 퍼지 분할 평가 지수를 저장할 변수
   md = rand(cmax,n); % [0,1] 사이의 랜던 값


===== PAGE 61 =====
                                                                   2장 퍼지 클러스터링   m

for c = cmin:cmax
      [UO] = initFcmc(c,butterfly); % 분할행렬의 초기치 설정
      [U,V,iter] = fcmc(m,eps,UO,butterfly); % 퍼지 클러스터링 실행
      sxb(c) = Sxb(m,U,V,X);
end
% 최소 평가척도 값과 그 때의 분할 수
[min_sxb,opt_c] = min(sxb(cmin:cmax));
x = cmin:cmax; % 가로축 변수
plot偶sxb(cmin:cmax),'b小
xlabel('No. of fuzzy partition');
ylabel('Value of validity measure, Sxb');
text(4,O.9,['no. of optimal partion = ' num2str(opt_c+cmin-1)]);
axis([1 cmax 0 max(sxb)});


          血nction sxb = Sxb(m,U,V,X)
          % Xie와 Beni의 퍼지 분할 평가척도
          % 이 함수는 퍼지 지수 m, 분할 행렬 {J, 데이터 x와 클러스터 중심 V를
          % 인수로 벋아 퍼지 분할 평가척도를 계산한다．
          % 사용법： pi = Sxb(m,U,V,X)
          %            X    :nxd    크기의 뎨이터 벡터（d: 데이터 차원）
          %            U : cxn 크기의 최종 분할 행렬
          %            V    : dxc 크기의 클러스터 중심 벡터


           tmp = X';
          X = tmp; % d x n 크기의 데이터 벡터로 전치
          % 초기화
          [c,n] = size(U); % 분할 클러스터의 수 C오｝ 데이터 수 n의 계산
          [d,nn] = size(X);
          VO = zeros(d,n);
          dist = zeros(c,n);
          vdist = zeros(c,c);
          for i=1:c
                for j=1:d
                % 클러스터 중심벡터를 데이터 x와 동일 차원으로 만듦
                 VO(j,:)=＼岫'I）求ones(1,n);
                end
                tmp2 = X - VO;


===== PAGE 62 =====
56   퍼지, 진화컴퓨팅 프로그래밍




              tmp2 = tmp2.*tmp2;
              小st(U) = sum(tmp2); % 클러스터 중심과 뎨이터와 거리
        end
        sxb denom = sum(sum((U．八m)．水（list)); % 식（2.8）의 분자
        tmp3 = zeros(d,1);
        的r i=1:c
              for j=1:c
                                    if (i == j) vdist(ij) = 1.elO;
                                   이se
                                           % 클러스터 중심 간의 거리 계산
                                           tmp3 = V(:,i) - V(:,j);
                                           tmp3 = tmp3.*tmp3;
                                           vdist(ij) = sum(tmp3);
                                     end
              end
        end
        sxb numer =n水min(min(vdist)); % 식（2.8）의 분모
        sxb = sxb_denom/sxbnumer;




                            1
                        9
                        0
                                                      no. of optimal partion r 2




                8  7   6       4   3


                           V
                           二

                0  0   0   0   0   0   0
                                      {
                                      n




                 꿎m n
                    m뇨
                     ＝ m月mE＞ 亡
                             乙＝m
                               ＞ 늠띠三m>

                        1
                        0


                                01
                                                     4         5       6        7   8   9   10
                                                         No. of fuzzy partition



                  ［그림 十7] 평가척도 .S뇨m를 이용한 최적 퍼지 분할 수


===== PAGE 63 =====
                                                         2장 퍼지 클러스터링




                                   연습문저1


[1] 식（2.9）어］ 대한 평가척도 코드를 작성하고 나비 데이터에 대한 최적 퍼지 분할 수를 결
   정하라（나비 데이터는 다운로드한 파일의 '2장’ 디렉토리에 있는 butterfly.dat를 사

   용） .




[2] 정규분포로 3개의 데이터 집합을 만든다（매트랩 randn함수 이용）. 이 가운데 두 개 집
   합은 가까이 섞여 있고 나머지 하나는 떨어져 있게 한다. 이 데이터어］ 식（2.8）의 퍼지
   분할 평가척도를 적용해 보자．




                              壽 심화 학습 자료 蜘


'D. Gustafson and W. Kessel, "Fuzzy clustering with a fuzzy covariance matrix,"
 In Proc. IEEE CDC, pages 761-766, San Diego, 1979.
'J. C. Bezdek, and N. R. Pal, "Some new indexes of cluster validity," IEEE Trans.
 on SMC Part-B: Cybernetics, Vol. 28, No. 3, pp. 301-315, 1998.
'J. C. Bezdek, ／勿材em2 Re口7g7끄苡772 11北／i Fuz乙JTO自／e（吃加eF口fl'？苡7fl Algon功끄2,
 Plen끄22, NY, 1981.
M. R. Rezaee, B. F. P. Lelieveldt, and J. H. C. Reiber, "A new cluster validity
 index for the fuzzy c-mean," Pattern Recognition Letters, Vol. 19, pp. 237-246,
 1998.
1N. Zahid, M. Limouri, and A. Essaid, "A new cluster validity for fuzzy
 clustering," Pattern Recognition, Vol. 32, pp. 1089-1097, 1999.
'X. L. Xie, and G. Beni, "A validity measure for fuzzy clustering," IEEE Trans.
 on Pattern Analysis and Machine Intelligence, Vol. 13, No. 8, pp. 841-847, 1991.
'Y. Fukuyama, and M. Sugeno, "A new method of choosing the number of
 clusters for the fuzzy c-means method," Proceedings of 5th Fuzzy Systems
 Symposium, pp. 247-250, 1989.
'U. Kaymak, and M. Setnes, "Fuzzy clustering with volume prototypes and
 adaptive cluster merging," IEEE Trans. on Fuzzy Systems, Vol. 10, No. 6, pp.
 705-712, 2002.


===== PAGE 64 =====
CHAPTER 3   진화알고리즘 차분진화




              串 3. ] 진화알고리즘의 개요
              串 3.2 진화알고리즘의 용도
              永 3.3 차분진화


===== PAGE 65 =====
                                     3장 진화알고리즘小차분진화      61




66 자연 진회를 모방한 진화알고리즘은 비록 생물학적 진회를 간략화 시킨 것임어］도 불구하고 30
  여넌에 걸친 연구와 응용을 통해 매우 강력하고 강인한 탐색 기법으로 발전하였고, 다양한 학문
  분야에 관여하는 연구 분야로 성장하였다. 최근에는 최적화를 넘어 디자인 문제에 이를 적용하려
  는 연구' } 대단커
            ' 활”‘"하다· 99




 자연계에서는 생물학적으로 다양한 유기체가 탄생하고 한정된 자원을 이용하려고 다투면
서 보다 적합한 유기체가 생존해서 그들의 유전물질이 전파된다. 이런 자연 진화 원리를 바탕
으로 실세계의 다양하고 복잡한 문제를 해결하는데 사용할 목적으로 만든 것이 진화알고리즘
이다. 진화알고리즘은 자연계에서 볼 수 있는 무성생식과 유성생식을 모방한 것으로 무성생
식을 모방한 것은 부모 개체와 유전적으로 동일한 자식 개체를 낳는 반면 유성생식을 모방한
것은 부모 개체로부터 유전 정보를 교환하여 자식 개체를 낳는다. 유전정보의 교환을 위해
교바匠 알려진 재결합 연산자가 사용되며, 무작위 효과를 위해 돌연변이 연산도 사용된다．
유·무성생식 모두 부모개체의 선택이 필요하며, 이 선택은 개체의 적합도어］ 의존하기 때문어］
개체의 적합도를 측정할 수 있는 적함도 함수가 필요하게 된다. 적합도가 높 을수록 개체의
선택 확률이 높아지는 방식을 ' 적합도어］ 비례한 선택 '이라 한다. 작은 그룹에서 무작위로 몇
개의 개체를 선택하고 이들을 경쟁시켜 그 가운데 가장 우수한 것（적합도 값이 큰）을 선택하
는 방식도 있으며 이를 '승자승 선택'이라 한다. 진화알고리즘에서는 집단 내의 개체를 무작
위 값으로 초기화함으로써 초기 다양성을 확보하며 진화가 이루어지는 과정에서는 돌연변이
연산을 통해 다양성을 유지한다.
진화알고리즘은 문제해결을 위해 첫째, 집단이 처한 환경에서 보다 적합한 개체가 생존하
고 더 오래 존속하고 툴째, 유전자형으로 코딩 된 개체의 특성은 자손에게 유전되어 새로운
세대에 전파되고 셋짜1, 생식 과정에서 자손의 염색체는 부모의 염색체를 혼합한 것이며（유성
생식） 넷째, 자손의 특성은 부분적으로는 부모로부터 유전되지만 일부는 생식 과정에서 새로
이 획득된 유전자로부터 얻어진다는 진화 원리를 모방한 것이며 이를 컴퓨터 프로그램 모델


===== PAGE 66 =====
62      퍼지, 진화컴퓨팅 프로그래밍



 로 만든 것이다．
     진화알고리즘은 문제어］ 대한 해（적합도가 높은 개체）를 찾는 무작위 탐색이 아니라 확률적
 프로세스로 그 결과는 무작위한 것 보다 훨씬 우수하다. 진화알고리즘에서 다음 세대의 개체
 집단을 발생하기 위해서는
     (D 부모 개체가 선정되고 교배 풀이 만들어짐．
     （勿 교배 풀에서 선정된 부모 개체에 교배를 통해 동질의 염색체가 합쳐지고, 복제되고 유전
      적 물질을 교환（유성생식을 모방한 경우 교배 연산을 통하1, 무성생식을 모방한 경우 부
      모 염색체가 변경 없이 복제됨）.
     （匈 복제 과정에서 돌연변이를 적용.
     세대를 거치면서 이 서］ 과정의 반복을 통해 진화가 이루어지며, 이를 가상의 코드로 기술하
 면 아래 그림3-1과 같다.



           // 시간을 초기화
           t= o
           // 무작위 값으로 집단 초기화
           沇it尸印侃毗im2: P(t) . P(t) = 佃（t)，口2m, ···，a (t)}
           // 적합도 평가
           evalPopulation: P (t) , 少 (P(t)) = {P (a1 (t)),j (a2 (t)), " " " ,'P (a (t ))}
           // 종료 조건으로 세때1 수 또는 적합도 값을 사용
           wh可le (n야 terrninat加Ti c刃2dition)

           {
                // 재결합 적용 , r () : 재결합 연산자
                recombine: P' (t) = r (P(t))
                // 돌연변이 적용 , m ( : 돌연변이 연산자
                mutate: P ' (t) =m (P' (t))
                   // 적합도 평가
                   eva1Papulation: I ' " (t) ,
                                            j (P' (t)) = ｛少（n; (t)),j (q; (t))，···，j (O;(t))}

                   // 생존할 개체 선택 , sQ: 선택 메카니즘
                   sele（才： 尸（t+ 1) = 如（尸" (t)) （才 S（尸（t) u尸" (t))}
                   // 세대 수의 증가
                   t= t+ 1
            }
                                ［그림 3너］ 진화알고리즘의 계산 과정


===== PAGE 67 =====
                                              3장 진화알고리즘U차분진화          63




 Fuzzy & Evolutionary
    Computing Programming   3.2 진화알고리즘의 용도


 오늘날 진화알고리즘은 다양한 학문 분야의 사람들로부터 관심을 끌고 있다. 컴퓨터 과학
자는 기호 정보처리 , 학습, 적응시스템, 컴퓨터 프로그램의 자동생성 , 인공발생학에 의한 유
기체（인공생명）의 창조와 관련하여 진화알고리즘어］ 관심이 있으며 , 대규모 병렬 처리가 가능
한 진화알고리즘 하드웨어 개발에도 관심이 많다. 공학자는 다양한 분야에서 최적화나 디자
인 문제를 해결하는테 진화알고리즘을 활용한다 로보트 연구자는 사전어］ 작성된 지도를 사
용하지 않고 불확실한 환경에서 주행할 수 있는（시행착오를 통한 학습에 의해 주어진 환경어］
적응할 수 있고） 로보트를 만들기 위해 진화알고리즘어］ 관심을 가지며, 인지과학자는 분류시
스템을 사용하여 뇌의 사고 및 인지 모델을 묘사할 수 있는 도구를 만들려 할지 모른다. 물리
학자는 병렬처리가 가능한 진화알고리즘 컴퓨터를 사용하여 수천 개의 변수를 갖는 실제 문
제를 보다 쉽게 모델링 할 수 있을지 모른다. 생물학자는 유기체 집단의 실제 행동을 모델링
하거나 RNA 접이 경로를 찾는데 이를 사용할 수 있으며, 경제학자는 새로운 계량 경제 모델
을 만들거나 게임이론어］ 따른 새로운 게임전략（진화 게임）을 만드는데 이를 사용할 수 있다．
컴퓨터 음악가는 멜로디를 구성하거나 멜로디어］ 붙일 화음을 만드는데, 컴퓨터 그래픽 아티
스트는 새로운 이미지를 만드는데, 또 다른 컴퓨터 예술가는 가상의 조각공원, 가상의 유기체
환경 등을 만드는데 진화알고리즘을 사용하고 있다. 이상어］ 언급한 것처럼 진화알고리즘의
활용 분야는 매우 다양하다.
 진화 원리를 컴퓨터 모델로 만든 것을 진화알고리즘佃volutionary Algor此뇨n)이라 부르
며， 유전알고리즘（Genetic Algorithms), 진화전략（Evoli血on Strategy), 진화프로그래밍
(Evolutiona玎 Progranmiing), 분류시스템（Class出er System), 유전프로그래밍（Genetic
Programming）과 차분진화（Differential Ev아utionary Scheme）라는 6가지 알고리즘이 있
다. 이 책에서는 알고리즘이 매우 간단하면서도 파라미터 최적화에 효율적으로 사용할 수 있
는 차분진화（3.3절）와 다양한 분야에서 가장 널리 사용되고 있는 유전알고리즘（4장）을 소개
한다. 다른 알고리즘어］ 대해서 알고 싶은 분은 참고문헌을 활용하기 바란다．


===== PAGE 68 =====
64        퍼지, 진화컴퓨팅 프로그래밍




     Fuzzy & Ev이ut油！lary
        Computing Programming       3.3 차분진화


     이 절에서는 비선형이고 미분 불가능한 연속 공간 함수를 최적화하기 위한 차분진화（DE:
 Differential Ev아utionary Scheme）를 소개한다. 라이너와 케네스에 의해 제안된 이 방법은
 집단어］ 속한 개체 벡터의 거리와 방향 정보를 사용하는데 , 그 구조와 연산이 간단한 반면 수
 렴성이 뛰어나다. 차분진화의 응용 사례 및 다양한 언어의 코드（C , 八4at1ab, C++, Java,
 Scilab,     PSather, Fortran90,     I뇽thon,   Labview,   R）로 구현된   소스를 사이트
 (http://www.icsi.berkeley.edu/ '- storn/ code.html)에서 다운 받을 수 있다. 여기서 사용
 한 매트랩 극7亡두 이 사이트의 코드에 기초한 것이다. 차분진화는 목척변수에 해당하는 개체
 를 집단으로 사용하는 탐색 방법으로 집단의 크기는 진화 동안 변하지 않는다. 초기 집단은
 무작위로 구성하지만, 만약 우수한 해를 알고 있다면 이 해어］ 정규 분포의 무작위 변화를 주
 어 나머지 개체들을 생성할 수 있다. 차분진화의 핵심은 변화된 개체를 발생하는 체계에 있는
 더］, 두개의 개체의 차이에 가중치를 곱한 것을 서］ 번째 개체어］ 더해서 교배용 개체를 발생한
 다. 이 개체와 변경 대상 개체를 교배하여 새로운 개체가 얻어진다. 이 새로운 개체의 적합도
 가 변경 대상 개체의 것 보다 좋으면 이 개체로 변경 대상 개체를 대체한다. 즉, 교배로 만들
 어진 새 개체가 이전 것 보다 우수하면 새 개체가 살아남는다. 이는 현재 집단과 적어도 같거
 나 보다 우수한 개체들이 다음 세대에 유지될 수 있도록 해주기 때문어］ 표준 유전알고리즘어］
 서 종종 사용되는 엘리트주의와 유사한 효과를 거둘 수 있다. 교배용 개체를 생성하는 방식이
 몇 가지 존재하는데 여기서는 이 가운데 가장 기본적인 두 가지만을 소개한다．
     ni乂집단 크기）개로 구성된 변화 대상 개체 X，小 = 1.2, ·".np) 가운데 무작위로 선택된 서로
 다른 3개의 개체를 사용, 식（3.1）과 같이 교배용 개체를 생성한다．


         qnl= X,, . t + F. （兀，J -    'd)                                 (3.1)


     무작위로 선택된 rl , r2오｝r3는 0과 n刃 사이의 서로 다른 정수이고 변경 대상 개체의 인덱

 스 i 와도 다른 값이다．F (> 0）는 두 개체의 차이（兀，.t                     兀，.n를 조정하는 상수 파라미터로

 통상 0에서 2 사이의 값을 갖는다. t는 진화 세대 수를 표시한다. 차분 변화를 통해 새로이
 만들어질 개체가 식（3.2）에서와 같이 d 차원（탐색할 해의 차원）이라 하자. 식（3.3）은 식（3.1)


===== PAGE 69 =====
                                                3장 진화알고리즘e차분진화      ] 65
의 교배용 개체와 식（3.2）의 변경 대상 개체어］ 적용할 균일 교배 연산을 정의하고 있다．


   x.t =［比，比，···，x1,t}                                           (3.2)
   t
   T1aJ1i
            =n뇨，if rand 之 q, 4= ] 9 ... a
            l               +                                    (3.3)
                xh   otherwise   '   ' -,   W


 rar流는 구간 [0, 1］에서 무작위로 선택된 수이고 C，은 교배가 일어날 확률（교배율）이다. 교

배로 얻어진 개체가 자식 개체로 다음 세대에 살아남을 수 있는지를 결정하기 위해 Xh +1와

Xh의 적합도（목적함수 평가）를 비교한다． Xh +1의 적합도가 Xh의 적합도 보다 좋으면

t+ 1 세대에 石．t+1가 戈,릍 대신하며 반대인 경우에는 戈,t+1 = Xh가 된다. 교배용 개체

생성을 위해 식（3.1) 대신 식（3.4）를 사용할 수 있다. 이 식에서는 교배용 개체를 만들 때 현
재 세대까지 가장 우수한 개체를 기준 개체로 사용한다. 교배 연산 및 개체의 생존 여부는
앞의 경우와 동일하다.


   까，t+l= Xk:t,t + F · （兀d -兀,, t)                               (3.4)


 차분 진화를 사용할 때는 다음과 같은 규칙을 유념해야 한다．

 (D 초기 집단은 하1 공간어］ 골고루 분포되도록 해야 한다．
（勿 집단의 크기佃끼는 찾고자 하는 목적변수 숫자의 10배 정도로 한다．
（匈 교배율 （斗은 0과 1사이의 값으로 한다．
 (4) 가중치 F는 0.5와 1사이의 값으로 한다．
 (5) 가장 우수한 개체가 진화하면서 변화가 크면（특히 진화 초기에） 비록 적합도 값이 느리
   거］ 좋아져도 수렴할 가능성은 높다．
（旬 적합도 값이 일정 세대 동안 변하지 않아도 반드시 나쁜 것은 아니다（목적함수에 평탄면
   어］ 있는 경우）. 그러나 이는 최적화어］ 상당한 시간이 걸릴 수 있기 때문어］ 이 경우 집단
  크기를 증가하면 수렴어］ 도움이 된다．
 匣） 적합도 값이 너무 빠르거1 좋아지지 않는 것이 좋다. 이는 국부 수렴할 가능성이 크기
   때문이다. 국부 수렴이 발생하면 집단 크기를 크거］ 한다．
（匈 적합도 함수를 적절히 선택하는 것은 매우 중요하다. 문제어］ 대한 정보를 적합도 함수어］


===== PAGE 70 =====
66       퍼지, 진화컴퓨팅 프로그래밍



      많이 포함시킬수록 수렴할 가능성은 높아진다．


     진화알고리즘에서 적합도함수는 최대화를 목표로 한 것이기 때문에 최소화 문제인 경우 목
 적함수를 적합도함수로 그대로 사용할 수 없다. 즉, 최소화 문제의 목적함수를 최대화 문제의
 목적함수（적합도함수）로 변환하여야 한다. 그러나 다른 진화알고리즘과 달리 차분진화에서는
 단순한 선택 메커니즘으로 인해 목적함수를 적합도함수로 변화할 필요가 없다. 즉, 목적함수
 를 그대로 적합도함수로 사용하는데, 이는 새롭게 만들어진 개체의 적합도와 이전 개체의 적
 합도를 비교해서 생존할 개체의 선택이 이루어지기 때문이다. 최소화 문제에서는 적합도가
 작은 것이 생존하며, 최대화 문제에서는 그 반대이다．                                 1




     리스트 3.1은 차분진화를 사용해서 식（3.5) 함수의 최적 해를 찾는 코드이다．


      九，, ,而毗侮）=100 (寸m蜘)2+ (1_ xi)2                               (3.5)
                   - 2.048 드 파 드 2.048, 최소값：1切,, 昕岫（1,1) = 0



 mmm 리스트 3니 馨 차분 진화를 사용한 함수 최적화 코드

     % 파일명 flinco的mize.m: 차분 진화를 이용 목적함수를 최소로 하는 해를 구함
     % 목적함수를 정의하는 파일명 rosenFunc.m
     fname = 1r0SellFnllC'，·

     tix = 2; % 해의 수
     % 해의 탐색 범위 [ xl의 탐색범위·, x2의 탐색범위］
     xbound = [-2 2; -2 2];
     parm = [1; % 문저1 정의어］ 필요한 파라미터
     maxGen = 200; % 최대 진화 세대 수
     goal = 0; % 목표 목적함수 값
     epsFit = i.e母 % 목표 목적함수 값에 대한 허용오차
     np = 15; % 집단의 크기
     F = 0.5; % 차분 크기 조정 가중치
     Cr = 0.5; % 교배율
     ndisp = 10; % 중간 결과를 화면어T 표시하는 세대 간격
     nde = 1; % 교배용 개체 생성 방법 선택
     fType = 0; % 목적함수 유형 선택용으로 0 이면 최소화， 1 이면 최대화 문저］
     % 차분진화


===== PAGE 71 =====
                                                                       3장 진화알고리즘H차분진화   67


[x,obj,nobj,objhist] = de(thame,nx,xbound,parm,maxGen,...
                                 goal,epsFit,np,F,Cr,ndisp,nde,fType);
x % 최적 히；1
obj % 최적 해에 대한 목적함수 값
nobj % 최적 해를 얻을 때까지 실행된 목적함수 평가 횟수
plot(objhist);
xlabel('generation');
ylabel('objective function value');


           function [bestx,bestfit,nfeval,objhist] = de(fhame,nx,...
                  xbound,parm,maxGen,goal,epsFit,np,F,Cr,ndisp,nde,fType);
           % 차분 진화를 이용한 문저1 ' frosen'의 최적화
           % A용법 [bestx,bestfit,nfeval] = de(fname,nx,xbound,...
           %                     parm,maxGen,goal,np,F,Cr,ndisp,nde,fl'ype)
           % 출력 인수
           %      bestx: 진화를 통해 얻어진 좋은 해
           %      bestfit: 가장 좋은 해의 목적함수倒합도 함수） 값
           %      nfeval: 차분 진화가 종료될 때까지 실행된 적합도 함수 평가 횟수
           %       objhist: 각 세대에서 목적함수 값을 기록
           % 입력 인수
           %       fname: 목적함수가 정의된 파일명어］ 대한 문자열
           %      nx: 탐색할 해의 차원
           %       xbound: 탐색 범위， xbound(:, 1)＞최소값, xbound(:,2)＞최대값
           %      parm: 문제를 정위하는데 필요한 파라미터
           %      maxGen: 최대 진화 세대 수
           %      goal: 목표 적합도 값
           %      epsFit: 적합도 허용오차
           %      np: 집단의 크기로 문제의 복잡성어］ 따라 대개 10 \ 30 범위로 함．
           %      F: 차분 크기 조정 가중치
           %      Cr: 균일 교배의 교배율
           %      ndisp: 이 횟수만큼 진화한 후 중간 결과를 화면에 표시（정수）,
           %            이 값이 l 보다 작으면 표시하지 않음
           % nde: 교배용 개체 생성 방법 선택， 식（3.1) 또는 식（3.4)
           % fType: 목적함수 유형， 최소화 또는 최대화


           xbound = xbound'; % xbound를 전치시킴
           % 집단 초기화， 탐색 범위 내의 무작위 값으로 초기화 함


===== PAGE 72 =====
퍼지, 진화컴퓨팅 프로그래밍



   pop = zeros(np,nx);
   for i=1:np
    pop(i,:) = xbound(1,:) + rand(1,nx).*(xbound(2,:) -...
                       xbound(1,:));
   end
   ol如叩 = zeros(size(p이）)); % 이전 세대의 집단 보관
   加al = zeros(1,np); % 현재 세대의 목적함수（적합도） 값
   bestx = zeros(1,nx); % 현재까지 가장 좋은 해를 보관
   nfeval = 0; % 적합도 함수 평가 횟수
   objhist = zeros(1,maxGen);
   % 무작위로 만들어진 집단의 적합도 평가
   % [yl,..,yn] = feval(fhame,xl,...,x미， feval은 매트랩 함수
   [x obj] = 免val(fname,pop(1,:),parm); % 첫 번째 개체 평가
   fit(1) = obj;
   bestfit = fit(I); % 가장 좋은 적합도 값으로 설정
   bestp아） = 1; % 가장 좋은 개체 번호 저장
   nfeval = nfeval + 1; % 함수 평가 횟수 증가
   for i=2:np % 나머지 개체에 대한 평가
     [x obj] = feval(thame,pop(i,:),parm);
     fit(i) = obj;
     nfeval = nfeval + 1;
         if (fType =    0)
           % 최소화 문제에서 목적함수 값이 더 작으면
           if (fit(i) < bestfit)
                bestp아） = 1;
                bestfit = fit(i);
            end
      이se
            % 최대화 문제에서 목적함수 값이 더 크면
            if (fit(i) > bestfit)
                bestp야） = 1;
                bestfit = fit(i);
            end
         end
    end
   bestx = pop(bestpop,:);
   % 차분 진화


===== PAGE 73 =====
                                                         3장 진화알고리즘1차분진화   ] 69
crossarri = zeros(np,nx); % 교배용 개체 선정어］ 필요한 배열
crossarr2 = zeros(np,nx);
crossarr3 = zeros(np,nx);
rotate = (0:1:np-1); % 집단 크기의 순환 인덱스
indrotate = zeros(np); % 순환 인넥스
indarri     = zeros(np); % 인덱스 배열
indarr2     = zeros(np);
indarr3     = zeros(np);
mnd = zeros(2);
crossp이） = zeros(np,nx);      % 교배용 개체
cross = zeros(np,nx); % 교배에 사용될 유전물질의 위치
% 교배에서 부모 개체의 유전물질을 물려받는 위치
nocross = zeros(np,nx);
gen = 1;
% 종료조건
while ((gen <= maxGen) & (abs(bestfit - goal) > epsFit))
   이dp아） = pop; % 현재 집단 보관
   mlld = randperm(2); % 인덱스 포인터 배열
   indarri     = randperrn(np); % 개체 위치를 섞음
   % ind(l)만큼 위치를 변경， re呵m川은 rn/n의 나머지 계산
   indrotate = rem(rotate+ind(1),np);
   indarr2     = indarrl(indrotate + 1);
   indrotate = rem(rotate+ind(2),np);
   indarr3     = indarr2(indrotate + 1);
   % crossarri, crossarr2, crossarr3은 서로 다른 개체를 복제．
   crossarri = oldpop(indarrl,:);
   crossarr2 = oldpop(indarr2,:);
   crossarr3 = oldpop(indarr3,:);
   % 교배율에 의해 교배 대상 위치 결정
   % 교배율 보다 작은 값을 가지면 l로， 그렇지 않으면 0으로
   cross = rand(np,nx) < Cr;
   nocross = cross < 0.5; % cross와 0과 l으1 값을 반대로 가짐
   if (nde =      1) % 식（3.1)어］ 의한 교배
          % 교배용 개체 생성
          crosspop = crossarri + F*(crossarr2 - crossarr3);
   이se
           % nde = 2: 식（3.4）어］ 의한 교배


===== PAGE 74 =====
70   퍼지, 진화컴퓨팅 프로그래밍



           end
          % 교배 대상 pop이d와 교배용 벡터 crossp야）의 교배1 연산
           cross = oldpop.*nocross + crosspop.*cross;
          % 탐색범위를 벗어난 경우, 해당 변수의 경계 값으로 설정
           for i=1:np
              白r j=1:nx
                       if (cross(ij) < xbound(1j))
                          cross(ij) = xbound(lj) ;
                       elseif (cross(ij) > xbound(2j))
                             cross(ij) = xbound(2,j);
                       end
                 end
           end
           % 새로 만들어진 집단 cross의 적합도 평가
           for i=1:np
                 [x obj] = feval(thame,cross(i,:),parm);   % 개체 평가
                  tempfit = obj;
                 nfeval = nfeval + 1;
                 if (fType == 0)
                    if (tempfit <= fit(i)) % 이전 개체의 목적함수 값과 비교
                          % 더 작으면 새 개체를 다음 세대 개체（자식）로 인정
                          pop(i,:) = cross(i,:);
                             fit(i) = tempfit; % 목적함수 값 저장
                          if (tempfit < bestfit)
                                bestp아1 = I;
                                bestfit = fit(i); % 더 우수한 목적함수 값 저장
                             end
                       end
                  else
                       if (t口np血 :>= fit(i)) % 이전 개체의 목적함수 값과 비교
                          % 더 크면 새 개체를 다음 세대 개체（자식）로 인정
                          pop(i,:) = cross(i,:);
                             fit(i) = tempfit; % 목적함수 값 저장
                          if (tempfit > bestfit)
                                bestp아） = 1;
                                bestfit = fit(i); % 더 우수한 목적함수 값 저장
                             end


===== PAGE 75 =====
                                                                    3장 진화알고리즘1차분진화


                      end
                end
          end
          objhist(gen) = bestfit;
          bestx = pop(bestp이）,:); % 더 우수한 개체（해） 저장
          if (ndisp > 0)
              if (rem(gen,ndisp) == 0)
                  加rintf(1,'gen: %d, best_fit: %3.1e, neval: %d\n',...
                                    gen,bestfit,nfeval);
                      for j=1:nx
                            fPrintf(1,'best_X(%d) = %f\ 如',j,bestx(j));
                      end
                end
          end
          gen = gen + 1;
       end




      function [x, obj] = rosenFunc(x,parm);

      % 파일명： rosenFunc.m
      % 목적함수로 차분 진화에서는 적합도함수로 그대로 사용
      % A]용법 [x, obj] = rosenFunc(x,parm);
      %                 입력 벡터 x = [x(1) x(2)], x(1) = xl, x(2) = x2
      %                 parm: 파라미터 벡터로 이 문제에는 필요치 않음
      %                 叱j: 목적함수 값


      % Rosenbrock 의 목적함수
      obj = 100木（x(2)-x(1）八2）八2十（1-x(1)）八2;




그림 于1은 차분 진화어囚 식（3.5）의 목적함수 값이 감소해서 목표어］ 도달하는 과정이다．


===== PAGE 76 =====
1四口    퍼지, 진화컴퓨팅 프로그래밍




                        3.5




                m
                쿄m＞ 등g= ＝
                        卜山＞ g으g
                            二
                            V
                            n
                            {




                                  n
                                  {




                            二
                            V
                            1




                                  1




                                          50        100       150   200
                                                 generation


                                      ［그림 3-1] 진화 세대별 목적함수의 값



  다른 최적화 문제에 이 코드를 사용하기 위해서는 문제에 대한 목적함수 파일（여기서는
 rosenFunc.m)을 재정의해야 하고, 해의 수佃功, 해의 탐색 범위似bound), 목표 목적함수 값
 (goal) 및 최적화 유형（fype) 값을 문제에 맞게 변경해야 한다. 파라미터（parm)는 문제를
 기술하는데 필요한 경우에만 사용하며 , 나머지 차분진화 파라미터인 최대 진화 세대 수
 (maxGen) , 집단크기（np), 가중치（F), 교배율（Cr）은 실행해 보면서 적당한 값으로 변경할 수
 있다．




                                               [ 연습문저1
  [1] 리스트 31에서 교배용 개체 생성 부분의 코드에 식（3.4）를 위한 코드를 추가하고 식
      (3.1）과의 결과를 비교하라. 또한 F와 （十 값에 따라 차분진화의 성능이 어떻게 변화하
      는지 본다．
  [2] 차분진화를 사용하여 아래 함수를 최소로 만드는 해를 찾아라. 이를 10번 실행하고 최
      적 해를 찾는데 걸린 적합도함수의 평가 횟수에 대한 평균과 표준편차를 구하라．


===== PAGE 77 =====
                                                            3장 진화알고리즘小차분진화    m

                   凡蜘他 ) =
                                 20exp-.·出枷］
                                 20e2끄



                                  exp［去客.os(2irx,)］『20
                                                    『e
                                   30 드 ;ri 드 30,   n= 30

                              최소 값： fAct：加q (0, o, ·· ,0) =o




                               的 심화 학습 자료 醬



·황희수, 컴퓨터에 의한 진화계산 및 진화디자인, 내하출판사, 2002.
'K. Price and R. Stron, "Differential evolution: Numerical opti血ation made
 easy," Dr. Dobb's Journal, pp 18-24, April 1997.
·H. P. Schwefel, "Advantages and disadvantages of evolutiona玎 computation

 over other approaches," in Handbook of Evolutionary Computation, Oxford
 U小／ersity Press, New York, pp. A1.3:1-2, 1997.
'J. H. I如lland, Gene苡？ Alg口／1幼7끄S. S匕／e끄在万C 月끄始rican, pp. 66-72, 1992.

'M. J. French, Inve끄苡끄2an(/ 月volution.' Desi뇽72 끄21\色加re an(/ 万뇨印heering, 2nd
 Edition, Cambridge University Press, 1994.
'R. Storn and K. Price, "Differential Evolution: a simple and efficient heuristic
 for global optimization over continuous spaces," Journal of Global Optimization,
 Vol. 11, pp. 341-359, Kiuwer Academic Publisher, 1997.


===== PAGE 78 =====
孝 4.1 개체（해）의 표현 및 초기화
密 4. 2 개처떽 평가
永 4.3 선택
密 4.4 유전 연산
寧 4.5 종료조건
睿 4.6 유전알고리즘의 처리
孝 4.7 유전알고리즘의 실행


===== PAGE 79 =====
                                                     4장 유전알고리즘         m


66 탐색 과정에 자연 도태와 유전학의 원리를，陪한 최초의 알고리즘은 아니지만, 유전알고리즘
  (GAs: Genetic二 사gorit뇨ns）은 오늘날 가장 널리 사용되고 있다. 유전알고리즘은 다른 진화알고
  리즘에 비해 훨씬 자연 진화 원리에 가까우며, 많은 이론 및 실험적 연구가 수행되어 왔다. 유전알
  고리즘은 유연하고 강인한 능력으로 인해 불연속 함수 문제를 포함한 최적화 및 다양한 디자인
  문제를 해결할 수 있는 대안으로 각광 받고 있다. 비록 특정한 문제에 대해 어떤 알고리즘이 가장
  적합한지에 대해서는 논란의 여지가 있지만, 많은 연구자들이 유전알고리즘의 강인성에 동의하고
  있다. 즉, 어떤 한 가지 문제를 해결하기 위해 고안된 기존의 알고리즘이 유전알고리즘 보다 우수
  할 수 있지만, 유전알고리즘은 다양한 종류의 문제에 대해 우수한 해를 제공할 수 있다．
   골드베르그（G아dberg）는 개별적인 유전연산이 단순하고 그다지 매력적이지 못함에도 불구하고
  이들을 결합한 유전알고리즘이 유용한 탐색을 실행할 수 있는 이유를 '혁신직관（it끄iovation
  intuition)' 이라는 개념으로 설명하였다. 그의 설명에 따르면 선택과 돌연변이가 결합되면 언덕
  등반 메커니즘 역할을 한다. 즉, 돌연변이는 현재의 해 주변에 위치한 변화된 해를 발생하고 선택
  을 통하1 이 해를 받아들임으로써 더 우수한 해를 향해 등반한다는 것이다. 국부적 주변 환경에서
  실험을 계속하면 개선될 수는 있지만, 이는 엄연히 국부적인 환경에서 이루어지는 것이다. 국부적
  인 것에서 벗어나기 위해서는 해당 지역을 탈출할 수단이 있어야 하는데, 선택과 재결합 연산이
  이런 수단을 제공한다. 이는 우수한 해들을 결합시켜 더 우수한 새로운 해를 만들어 낼 수 있음을
  의미하는 것이다.
   유전알고리즘은 개체（해） 집단을 유지하면서 적자생존의 원칙에 따라 보다 적합한 개체를 탐색
  한다. 이 알고리즘은 내재적 병렬성(implicit parallelism)과 외적 병렬성（explicit parallelism)으
  로 인해 해를 동시어］ 전망이 좋은 다수의 영역에서 효율적으로 탐색할 수 있다. 내재적 병렬성은
  홀란드（Holland）어］ 의해 개발된 스키마 이론（schema theory）에 의한 것이며 , 외적 병렬성은 집
  단을 조작하는 방식에 연유한다. 가령 , 개체들（집단）의 적합도를 평가할 때 이를 병렬처리 할 수
  있으며 1三1 나아가 다양한 형태의 병렬화가 가능한데 이를 병렬 유전알고리즘이라 부른다．
   한 가지 형태의 탐색 알고리즘으로 최적화 및 디자인에 관련된 거의 모든 분야에서 사용되는
  것은 유전알고리즘이 유일하다. 유전알고리즘은 다음의 4가지 면에서 기존의 알고리즘과 다른 특
  성을 갖는다．
  . 유전알고리즘은 통상 파라미터 그 자체（표현형 : phen毗）me）가 아니라 파라메타의 코딩（유전
   자형 : genotype）을 갖고 동작한다．
  U 유전알고리즘은 해 공간에서 점이 아닌 점의 집단（populat如n)으로 동작한다．
  U 유전알고리즘은 미분 값이나 다른 보조 정보를 사용하지 않고, 목적함수 값에 대응하는 적합도
   (fitness) 값만을 사용한다．
  U 유전알고리즘은 결정론적（deterministic）이 아닌 확률적佃的chastic) 천이규칙을 사용한다．


===== PAGE 80 =====
m        퍼지, 진화컴퓨팅 프로그래밍


        유전알고리즘은 다음과 같이 동작한다. 전형적으로 개체 집단은 무작위（랜덤） 값으로 초기화 된
       다. 알고리즘이 시작되면 집단의 모든 개체가 평가되어 각 개체가 얼마나 적합한지 값으로 주어지
       며 , 이 적합도 값이 각 개체가 다음 세대를 위해 소위 교배 풀에 얼마나 많이 복제될지를 결정한다．
       적합도가 높으면 그 만큼 복제될 가능성이 뇽｝진다. 교배 풀에서 두개의 개체가 부모 개체로 선택
       되고, 부모로부터 자손에게 임의로 유전자를 할당하는 교배1 연산을 통해1 자손이 발생한다. 이때
       돌연변이가 매우 낮은 확률로 자손 개체에 적용되며 , 하나의 개체를 돌연변이 시킬 때 전형적으로
       단일 형질이 무작위로 변경되고, 우수한 유전 물질이 세대를 거쳐 물려진다. 평가와 생식（선택과
       유전연산） 과정은 만족할 만한 해가 나타나거나 유전알고리즘이 제한된 세대 수에 도달할 때까지
       계속된다．
        이 장에서 소개하는 유전알고리즘의 매트랩 코드는 GAOT(Genetic Algorithm Optimization
       Toolbox）에 ' ］초한것 ' ］다（참고문헌［21).,,




    Fuzzy & Evolutionary
       Computing Programming     4.1 개체（해）의 표현 및 초기화


     유전알고리즘에서 초기 집단을 구성하는 가장 일반적인 방법은 집단 전체를 무작위로 구성
    하는 것이지만, 기존어］ 알려진 해가 존재한다면 이를 활용해서 보다 우수한 초기 집단을 생성
    할 수 있다（알려진 해（개체）를 초기 집단에 도입하고 집단의 나머지는 무작위로 구성하거나
    또는 알려진 해와 이를 무작위로 변형시켜 집단을 구성할 수도 있다）.
     n차원 공간에서 정의된 목적변수（탐색해야 할 변수） x= ｛떠, 劣2' ···, 劣, ｝에 의해 정의된

    목적함수 F佃1' 蜘， ...,xfl）를 최대로 하는 문제를 유전알고리즘을 사용하여 해결한다고 생

    각하자. 유전알고리즘의 집단 P7} 식（4.1）과 같이 7叩개의 개체로 구성된다고 하자．


       P= { X1, x2, ·．., y ' }                                   (4.1)


    Xv는 k번째 개체로 Xk= {d, 硝, · ..,xk, ｝이다．

     코딩된 파라미터를 유전자但ene), 하나의 유전자가 취할 수 있는 값을 형질（allele), 하나의
    개체（individual)가 갖는 유전자 집합을 염색체（chromosome）라 한다. 한 개체（해）를 문자열


===== PAGE 81 =====
                                                             4장 유전알고리즘                             79



로 코딩한 것을 유전자형（genotype）이라 부르고 코딩된 파라미터가 정의（의미）하는 것을 표
현형（pheno切）이이라 한다. 문자열로는 이진 값, 실수, 정수, 기호 등이 사용될 수 있다. 이
진 문자열을 사용하면 유전자는 0과 1의 형질을 가진다. 入五chalewicz어］ 의하면 함수 최적화
와 같은 문제에서는 실수형 유전알고리즘이 더 효율적인 것으로 입증되었으며 , 이 경우에는
유전자형은 필요 없고 표현형만이 존재한다. 그림 }1의 경우를 보자.



    개체 』Yk           분절1                분절2                                 분절m
    유전자형
                                   b缶                                1                         l
  （이진 문자열）
                             b추i                   b츨／
                                                                砂，
              하l
                                                                                        n11k
   변수의 범위          ［耐“ ,
                      '"畔씨          ［硝“" "，耐씨                            k "," ,
                                                                              '"伊씨，
    표현형              d                  姑                                     劣k,




                           ［그림 午1] 개체（염색체）의 구조




 문자열은n개의 분절로구분되고, 각분절은목적변수xi 드 ［叫“" ", 畔""］에 대응하는 / 비

트의 이진 코드로 이루어져 있다. 염색체의 길이는 m = n · / 비트이다. 유전알고리즘에서
선택과 유전 연산（교배와 돌연변이）은 유전자형에 적용되지만 적합도를 평가하기 위해서는
유전자형이 식（4.2）에 의해 표현형으로 해독（decoding）되어야 한다. 물론, 실수형 유전알고
리즘에서는 표현형만이 존재하기 때문에 이 과정은 불필요하다．


. 코딩 및 해독
 (1) 코딩： 실수 표현형을 이진 문자열인 유전자형으로 변환하는 것을 말함．
    fl체: 3.273672 -> 11.0100011000001
 (2) 해독： 유전자형인 이진 문자열을 표현형으로 변환하는 것을 말함．
       11.0100011000001 -> 3.273672



   e, (b}1,b}2,··此）＝叫」in + 뼈
                           ，叫“"「如가尸1「         \/   工     /
                                                                                      (4.2)



 이 식은 개체 Xk의 i 번째 분절의 이진 문자열（유전자형）을 표현형으로 변환하는 식이다．


===== PAGE 82 =====
80       퍼지, 진화컴퓨팅 프로그래밍


 e는 분절 단위의 해독 함수이며, U개의 분절로 구성된 염색체를 해독하기 위한 함수를 식
 (4.3）과 같이 표시하자．


       e (x' ) =e1xe2x ·.. xe,                                            (4.3)


 리스트 午1은 초기 집단을 생성하고 이를 평가하는 매트랩 코드이다．



 mm 리스트 4니 弊 이진 및 실수형의 초기 집단 생성, 초기화 및 평가

     function [pop] = initializega(npop,bounds,evalFN,evalOpts,options)
     % 파일명： initializega.m
     % function [pop] = initializega(npop,variableBounds,...
     %                           ev키FN,evalOpts，야)ti0flS)
     %     무작위로 초기 집단 생성, 행의 수는 집단의 크기를
     %     열의 수는 변수 boun小의 행의 수 더하기 1,
     %     이 l은 eva1FN의 리턴 값인 목적함수 枷）의 값을 저장하기 위한 것임．
     %     출력변수
     %          pop: 무작위로 구성된 초기 집단으로 적합도 평가를 받음
     %     입력 변수
     %          npop: 집단의 크기 즉, 개체 수
     %          bounds: 개체를 구성하고 있는 목적변수의 최소， 최대값을 갖는 행렬로
     %                      행의 수 = 목적변수의 수, 열의 수 = 2（변수의 최대값과 최소값）
     %          evaIFN: 적합도 평가를 위한 함수의 매트랩 파일명
     %          evalOpts: 적합도 평가를 위해 설정할 부가적인 옵션， 디폴트는 []
     %          options: 초기화 함수에 대한 옵션으로 [eps type prec]
     %                        eps는 epsilon 欲목표어］ 대한 허용 오차）
     %                        type은 실수형 인 경우 l , 이진 유전알고리즘의 경우 0
     %                        prec는 변수의 정확도로 디폴트는 [l.0e-6 1]


     % 실수형 GA
     if options(2) == l
          % eval 함수로 실행할 명령문을 문자열로 만듦
          % 개체를 목적함수어］ 넘겨서 적합도를 계산하고， 그 결과를 다시 개체어］ 저장
           estr = [[pop(i,:) pop(i,xZomeLength)]=' evaIFN '...
                    (pop(i,:),evalOpts);'];


===== PAGE 83 =====
                                                                         4장 유전알고리즘


% 이진형 GA
이se
      estr = ['x = b2f(pop(i,:),bounds,bits);[x v]=' eva1FN '. .
               (x,evalOpts); pop(i,:)=[也b(x,bounds,bits) v];'];
end
numVars = size(boun小,1); % 목적변수의 수
range = (bounds(:,2) - bounds(:,1))'; % 목적변수의 범위（최대 . 최소）
if options(2)= 1 % 실수형 GA
      xZomeLength = numVars + 1; % 목적변수의 수 + 1(적합도 저장용）
      p야） = zeros(i叩아工xZo毗Length); % 초기 집단 생성
      % 목적변수 범위 내의 값으로 랜덤 초기화
      pop(:, 1:numVars) = (ones(npop,1)*range).*(rand(npop,numVars))...
                                  + (ones(npop,1)*bounds(:, 1)');
이se % 이진형 GA
      % 총비트 수 = 목적변수의 삳변수 당 비트 수
      bits = calcbits(bounds,options(1));
      xZomeLength = sum(bits) + 1; % 총 비트수 + 1（적합도 저장용）
      p아） = zeros(npop,xZomeLength); % 초기 집단 생성
      % 랜덤하게 0과 I로 초기화
      pop(:, 1:suni(bits)) = round(rand(npop,sum(bits)));
end
for i=1:叩야）
      % 적합도 계산
      eval(estr); % estr의 문자열 명령 실행
end


          血nction [bits] = calcbits(bounds,precision)

          % 파일명： calcbits.m
          % function [bits] = calcbits(bounds,precision)
          % 변수 precision어］ 의한 정확도를 유지하기 위해
          % 실수를 이진 값으로 변환하는뎨 필요한 비트 수를 계산
          % 출력변수
          %          bits:   변수 당 필요한 이진 비트 수
          %          bounds: 변수의 범위
          %          precision: 두 수를 구분하는데 필요한 최소한의 차이


          bits = ceil(log2((bounds(:,2) - bounds(:, 1))'./precision));


===== PAGE 84 =====
                                水
m   퍼지, 진화컴퓨팅 프로그래밍



       % ceil(x): x를 올림， 정수로 만듦




       function [如al] = b2gbva1,bounds,bits)
       % 파일명： b2f.m
       % function [fval] = b2gbval,bounds,bits)
       % 이진 표현 by키을 실수（유전자형을 표현형）로 변환하는 함수
       % 출력 변수
       %          如al: 실수로 변환된 값
       % 입력 변수
       %          bval: 이진수로 표시된 값
       %          t兀unds: 변수의 범위
       %          bits: 각 변수를 이진 값으로 표시하는데 사용된 비트 수


       % 변수의 범위
       scale = (bounds(:,2) - bounds(:, 1))'./(2八bits-1);
       numV = size(bounds,1); % 1兀Un小의 행의 수， 변수의 수
       cs = [0 cumsum(bits)]; % cumsum(bits): bits를 축적시키면 더한 합
       for i = 1:numV
             % by키은 개체에서 각 변수의 이진 문자열을 뽑아 a에 넣음
             a = bval((cs(i)+1):cs(i+1));
             % size(a,2): a의 열의 수（변수별 비트 수） 계산
             %l兀unds(i,1): 변수의 최소값
             fval(i) = sum(2八(size(a,2)_l:_1:0).*a)*sca1e(i) + ...
                            bounds(i,1);
             % stir可2.八G匕e(a刀-1:-1:0H旬는 a의 이진 문자열을
             % 10진수로 변환함
       end




       function [bval] = f2b(fval,bounds,bits)
       % 파일명： f'2b.m
       % function [bval] = f2b(fval,bounds,bits)
       % 십진수 h키을 이진수（표현형을 유전자형으로）로 변환하는 함수
       % 출력 변수
       %          bval: 이진수로 변환된 값


===== PAGE 85 =====
                                                                   4장 유전알고리즘       m

       % 입력 변수
       %            fval: 실수로 표시된 값
       %           bounds: 변수의 범위
       %           bits: 각 변수를 이진 값으로 표시하는뎨 사용된 비트 수


       % 변수의 범위
       scale = (2八bits 1)./(bounds(:,2) - bounds(:, 1))';
       numV = size(bounds,1); % bounds의 행의 수， 변수의 수
       % cumsum(bits): b如를 축적시켜 더한 합
       csr=[O cumsum(bits)];
       bval = [1; % null 변수 선언
       for i = 1:numV
             % 이진수를 십진수로 변환
             fval(i) = (fval(i) - bounds(i,1))* scale(i);
           % [bval ....]: bval로 시작， 변수들의 이진 문자열을 붙여 나감
           bval = [bval rem(floor(如al(i)*p0w2(1-bits(i):O)),2)];
             % pow2(e): 배열 e의 모튼 원소어］ 대해 伊(2.八 e）를 계산
           % floor(x): x를 내림하여 정수로 만듦．
             % rem(x,2）는 x를 2로 나눈 나머지
       end




식（4.3）으로 개체 x培 해독하여 얻은 표현형을 식（4.4）에 대입하여 적합도를 계산한다．


  少 (Xb= T(F(e (x丸))                                                           (4.4)


少는.적합도 함수， 戶는 목적함수， T는 비율조정 함수이다. 비율조정（scaling) 함수는


===== PAGE 86 =====
:       퍼지, 진화컴퓨팅 프로그래밍



    · 양의 적합도 값을 보장해야 한다．
     ' 초기어］ 적합도가 높은 소수의 개제가 세대를 거치면서 부모 개체로 더 많이 선택되고
      이들의 유전물질이 유전자 풀을 빠른 시간에 지배함으로써 집단의 다양성이 훼손되는뎨
      이러한 조기수렴（premature convergence）을 방지한다．
     ' 상당한 진화가 이루어지면 열등한 개체는 소멸하고 비교적 우수한 개체만이 존재하게
      되지만 가장 우수한 개체의 적합도가 전체 개체의 평균 적합도 보다 약간 높게 되므로
      우수한 개체가 높은 비율로 부모 개체로 선택되지 못해 집단의 적합도 개선이 늦어지게
      되는데 이를 방지하는 역할도 한다. 비율조정 함수는 가장 우수한 개체가 가장 큰 적합
      도 값을 할당 받도록 한다．


    비율조정 방식에도 여러 가지가 있지만 여기서는 본래의 적합도를 선형 변환하는 방식을
    설명한다．식（4.5）은 평균 적합도를 변경하지 않으면서 최대로 변환된 적합도가 평균 적합도
    의 배수가 되도록 한다（흔히 , 2배수가 사용된다）.


       TL (F(e (Xk))) = aX F (e (Xk)) + b              (4.5)

       a =：二
                F                    P뻔1二 ' 凡q)
               (c-i)-'夕「.9, b= 凡，. ' (Fm
                 111i工入   [WY       4 max   4 口vg




    乙은 적합도를 선형적으로 조정하는 함수， c는 최대 적합도 결정어］ 사용된 배수, 凡七

    본래 적합도의 평균， 且flax는 본래 적합도의 최대값이다. 식（4.5）에서 한 가지 문제의 소지가

    있는 것은 가끔 매우 작은 적합도 값이 음의 값으로 변환되는 것이다. 이를 방지하기 위해
    음의 값이 발생하면 식（4.6）의 기울기와 상수를 사용하여 최소 적합도가 0이 되게 하고 이
    때에도 평균 적합도는 변하지 않는다．



       a= r，弓"且，
               ,;;II ,b = 云：耳：:                        (4.6)



    여기서 只，in은 변환 전의 최소 적합도이다．


===== PAGE 87 =====
                                                   4장 유전알고리즘        m




     유전알고리즘에서 개체의 선택은 매우 중요한 역할을 하는뎨, 보다 우수한（적합도가 높은）
개체가 더 많이 선택되도록 하는 확률적 선택이 수행퇸다. 모튼 개체는 한 번 이상 선택될
수 있으며 다음 세대의 생존을 위해 선택 받을 기회를 부여받는다. 가장 일반적인 선택 방법
은 적합도어］ 기초해서 개체에 선택 확률（尸）을 할당하는 것이다. [0,1] 범위의 랜덤 수
(random number) R/＼二 (i= 1, 2, ", 꺄D를 집단 크기 인 np7ll 발생시킨 다음 식（4.7）과 같이
축적 확률을 계산한다．



        C = Z PJ                                                 (4.7)
            j= 1




     尸는 3번째 개체의 선택 확률, C' 는 처음부터 i 번째 개체까지의 축적 확률이다. 만약 i브I
째 랜덤 수가 식（4.8）을 만족하면 可 번째 개체는 선택되어 다음 세대를 위한 교배 풀로 복제된

다．
        CZ 1 <RA{: (0, 1) < C'                                   (4.8)


개체에 확률을 할당하는 방법에는 다음과 같은 방법들이 있다．


     . 룰렛（ruulette)-휠（wheel) 선택（비례 선택）:
     모튼 개체는 자신의 적합도어］ 비례하는 확률을 할당 받으며 이들을 다 더하면 1이 된다．
이는 룰렛휠을 회전시키는 놀이와 유사하다. 룰렛e휠 선택에서는 가장 높은 확률과 가장
낮은 확률 간에 차이가 크지 않도록 해야 하며 이 차이가 크면 뛰어난 소수의 개체가 집단
전체를 매우 빠르게 지배하게 된다. 이와 같은 조기수렴 문제는 식（4.5）와 (4.6）의 비율조정
(scaling) 기술로 해결할 수 있다. 번식을 위한 개체 Xk의 선택 확률은 식（4.9) --(4.11）에서
와 같이 개체의 상대적 적합도에 의해 결정된다. 식（4.9）는 실수형이며 적합도 비율조정을 적
용하지 않은 경우, 식（4.10）은 이진 문자열에 적합도 비율조정을 적용하지 않은 경우이다.


===== PAGE 88 =====
86       퍼지, 진화컴퓨팅 프로그래밍




                            F (Xk)                                        (4.9)
         少伍k) =

                       三：         노F        (Xa        )
                            F (O (XC))                                    (4.10)
        少伍k) =
                   ZF(e（刃）)
                  j= 1




      이 확률 값을 기초로 식（4.7）과 (4.8）을 사용하여 개체를 선택, 다음 세대의 부모 개체를
 구성한다. 적합도가 음인 경우는 앞에서 설명한 적합도 비율조정 기술을 사용 적합도 값을
 양의 범위로 변환해야 하며, 최소화 문제인 경우는 목적함수를 최대화 문제로 변환해야 한다．
 식（4.11）은 실수형에 적합도 비율조정을 적용한 경우, 식（4.12）는 이진 문자열에 적합도 비율
 조정을 적용한 경우이다．


                            T(F(X' ))
                                                                          (4.11)
                       Z기끼xi))
                  i= 1

                            T(F(e (xk)))                                  (4.12)

                  三：         노T        (F         (e       (x   "   )))

     . 랭크（rank) 기반 선택：
      모든 개체가 자신의 적합도어］ 따라서 정렬되고, 개체는 이 순서（자신의 위치）어］ 따라 정해
 진 확률을 할당 받아, 이 확률어］ 따라 선택이 이루어진다. 적합도의 순서가 중요하기 때문어］
     적합도가 음의 값을 갖는 것이 문제가 되지 않으며 , 최소화 문제（적합도가 커지는 순서로 정
     렬）의 경우도 최대화 문제（적합도가 작아지는 순서로 정렬）의 정렬 순서를 역순으로 바꾸면
     된다. 확률 尸k는 모든 개체가 적합도어］ 따라 정렬된 후 정렬 위치 즉, 랭크에 기초해서 결정
     된다. 정규화 기하학적 랭크（normalized geometric ranking) 방법은 이 확률을 식（4.13）과
 같이 결정한다.


        少佯k) = q' (1- q) " '                                              (4.13)


===== PAGE 89 =====
                                                   4장 유전알고리즘   m

 q는 가장 우수한 개체를 선택할 확률, r은 개체의 랭크（위치： 가장 좋은 것이 1),

 =       .q    . .,., 이다．
     1 - (1 - q)"尸



U 승자승(tournament) 선택：
이 선택은 랭크 선택처럼 적합도 값만을 필요로 하지만 확률을 할당하지는 않는다. 전체
집단 가운데 무작위로 선택된 하위 집단（토너먼트）어］ 기초해서 이루어진다. 토너먼트 크기가
S라면 무작위로 S개의 개체를 선택하고 그 중 적합도가 가장 좋은 것이 다음 세대를 위한
부모 개체로 선택되며, 이 과정이 집단 크기인 71끄번 이루어진다．
리스트 午2는 이상에서 설명한 선택 방식어］ 대한 매트랩 코드이다．


蜘螂 리스트卜2. 룰렛m훨 선택

 凡nc如可newPop] = roulette（아dP이）,options)
 % 파일명： roulette.m
'% function[newPop] = roulette(oldPop,options)
 % 개체의 적합도어］ 기초한 선택 방법
 % 출력 변수
 %            newP아X 다음 세대를 위해 oldP叩에서 선택된 집단
 %            oldP이3: 현재 집단
 %            options: 옵션 ［세대 수］


 % 이dP이）의 열 수 = 변수의 수 + 1(적합도 저장）
 numVars = size(oldPop,2);
 % 이dP아）의 행 수， 개체의 4X집단의 크기）
 numSols = size(oldPop,1);
 % 적합도에 기초해서 상대적인 선택 확률을 계산
 的伍叩it = sum(oldPop(:,numVars力； % 이dPop의 마지막 열（적합도 값）의 합
 % 확률 = 개체의 적합되집단의 적합도， 룰렛－휠에서 영역의 크기 결정
 prob = oldPop(:,numVars)/totalFit; % 식(4.9)
 pr이） = cumsum(prob); % 축적 확률 계산
 % rand(numSols,1): [0刀 범위의 무작위 값을 균일분포로 갖는
 % numSols행xl열의 행렬 만들고， 이를 정렬시켜서 룰렛－휠어］ 맞힌 값으로 사용
 rNums = sort(rand(numSols,1));
 % 룰렛훨 선택어］ 의해 새로운 집단을 생성


===== PAGE 90 =====
                                      水
U國口      퍼지, 진화컴퓨팅 프로그래밍



   fitln = 1;
   newln = 1;
   while newln<= numS이S % 모튼 개체에 대해
         if (r寸ums(newln) < prob(fitln)) % 룰렛－휠의 해당 영역 안어］ 맞힌 경우
               newPop(newln,:) = oldPop(fitln,:);
               newln = newln+1;
         이se % 룰렛－휠의 해당 영역을 벗어나면, 다음 영역 선택
               fitln = fitln + 1;
         end
   end




 mm 리스트 4小 好 랭크 기반 선택

   function[newPop] = normGeomSelect(oldPop,options)
  % 파일명： normGeomSelect.m
  % 정규화 된 기하학적 분포어］ 기초한 랭크 선택 방법
  % 凡nction[newPop] = normGeomSelect(oldPop,options)
  % 출력변수
  %        newPop: 아dPop어］서 선택된 집단
  %        이dP이y 현재 집단
  %        options: 옵션 ［세대 수 가장 좋은 것을 선택할 확률］


   q = options(2); % 가장 좋은 것을 선택할 확률
   e= s倪e（아叩咀2); % 변수의 수 + l（적합도）
  n = size(oldPop,1); % 집단내 개체의 수
   newP이） = zeros(n,e); % 새로운 집단을 위한 변수 공간 확보
   fit = zeros(n,1); % 개체별 선택 확률을 위한 변수 공간
   x = zeros(n,2); % 정렬된 랭크오｝ 아이디의 리스트
   x(:,1) = [n:-l:l]'; % 개체의 랭크（위치： 가장 좋은 것이 1)
  % [y,I1 = so氓지는 인덱스 행렬 I를 리턴， x가 벡터면 y = x(I)
   [y x(:,2)J = sort（아dP아）(:,e)); % x(:,2）는 정렬에 따른 인덱스를 가짐
  r = ql(1-(1-q）八ll); % 분포를 정규화， 식（4.13）의 q'
   fit(x(:,2)) = r*( _q).A(x(:,1)-i); % 식（4.13）의 선택 확률 계산
   fit = cumsum(fit); % 축적 선택 확률
   rNums = sort(rand(n,1)); % n개의 정렬된 무작위 수 발생
  % 이하 부분은 룰렛－휠의 경우와 동일


===== PAGE 91 =====
                                                             4장 유전알고리즘   : 89
fitln=1;
newln=1;
while newln <== n
      if(rNums(newln) < fit(fitln))
            newPop(newln,:) = oldP아珽itln,:); % 血In번째 개체 선택
            newln = newln+1;
      이se
            fitln = fitln + 1;
      end
end




 리스트 小4. 승자승 선택

function [newPop] = tournSelect(oldPop,options)
% 파일명： 的urnSelect.m
% 승자숭 선택 방법
% function [newPop] = tournSelect(oldPop,options)
% 출력 변수
%           newPop: 아dP叩에서 만들어진 새로운 집단
%           이dP야y 현재 집단
%           options: 옵션 ［세디；1 수 토너먼트 크기］


加un侶切e = options(2); % 토너먼트 크기를 얻음
e = size（아叩叱2); % 변수의 수 + l（적합도）
n= s吃可이曲op,l); % 개체의 수
newP叩 = zeros(n,e); % newP叩을 위한 기억 공간 할당
% floor(x): x를 내림한 정수로
的urns = floor(rand(tournSize,n）木n) + 1; % 승자승 대결 순서
% reshape(x,m,n): x에서 열 방향으로 취한 값을 m x n 행렬로 만들어 리턴
% max 연산을 통해 승자 결정， b가 숭자의 인덱스를 가짐
[c b] = max(reshape(oldPop(tourns,e),tournSize,n));
newP이） = oldPop(diag(tourns(b,:)),:); % 승자를 newPop에 복제


===== PAGE 92 =====
90    [   퍼지, 진화컴퓨팅 프로그래밍




     Fuzzy & Ev이Ut的nary
        Computing Programming        4.4 유전 연산


      유전알고리즘에서 기본적인 탐색 메커니즘을 제공하는 유전 연산자（genetic operat아S）는
 기존의 개체（부모）를 활용해 새로운 개체（자식）를 발생하는데 사용된다. 유전 연산자에는 교
 배（crossover）와 돌연변이（mutation）가 있다. 교배는 두 개의 개체를 사용해서 두개의 새로
 운 개체를 만들어내지만, 돌연변이는 한 개의 개체에 작용해서 한 개의 새로운 개체를 만든
 다. 이들 연산자의 형태는 개체의 염색체 표현 방식어］ 따라 달라진다．




     4.4.1 이진 표현

      집단에 m차원인 두 개의 개체 x垣｝X"가 있다고 하자. 이들 개체의 염색체가 이진 문자
     열이라면 다음과 같이 이진 돌연변이（binary mutation）와 단순 교배（simple crossover）를
 정의할 수 있다. 이진 돌연변이는 개체 Xk의 모든 비트의 값을 식（4.14）와 같이 변경한다．


            HJi        丁｝ if 冗刃（0, 1) < 끄m
                                             i= 1, 2,·", m    (4.14)
                  x}     otherwise




      Pm은 돌연변이 확률（돌연변이율）이고 m은 염색체의 총 비트 수이다．


     1 돌연변이 연산
      d) 돌연변이 점을 임의로 선택
          개체 Xk = 1010 （표현형 10)
     （易 돌연변이 점의 유전자 형질을 변경（1- 0)
          개체 X'k = 1000 （표현형 8)


     리스트 午5는 이진 돌연변이어］ 대한 매트랩 코드이다．


===== PAGE 93 =====
                                                            4장 유전알고리즘            91



mm 리스트 4小 S 이진 돌연변이

  function [child] = binaryMutate(parent,bounds,Ops)
  % 파일명： binary入4utate.m
  % 돌연변이 확률어］ 기초해서 부모 개체의 비트 값을 변경（1口＞0)
  % func如n [child] = binar外如tate(parent,bounds，아均
  %       출력변수
  %           child: parent어］ 돌연변이를 적용해서 만들어진 개체
  %       입력변수
  %                        ［개체 문자열 적합도 값］)
              parent: 부모 개체（
  %           bounds: 해의 탐색 공간（변수의 탐색 범위）
  %           Ops: 이진 돌연변이를 위한 옵션 ［세대 수 돌연변이 확률］


  pm = Ops(2); % 돌연변이율
  numVar = size(parent,2)-1; % 변수의 수
  % [0,1] 범위의 랜덤 수를 변수 수만큼 발생시키고 이를 돌연변이율과 비교
  % 돌연변이율 보다 작으면 해당（변수） 위치어］ l , 아니면 0
  rN = rand(1,numVar) <pm;
  % rN이 l인 위치에서 parent의 값을 0은 l로， l은 0으로 변경
  child = [abs(parent( l:numVar) - rN) parent(numVar+1)];




 단순 교배는 1에서 m의 범위에서 균일 분포로 랜덤 수 丑N(1, m)을 발생시킨 다음 식

(4.15）와 (4.16）어］ 의해 두 개의 새 개체 x '노｝ X '"를 만든다．



          n}, if.,才< 丑刀（1,川
          나ioinerwise
                                                                        (4.15)


      2   I畔 if 秀 < R꼬（1, m )         i= 1, 2, "· ,m                    (4.16)
          { x otherwise



 다음을 보면 이 교배 과정을 쉽게 이해할 수 있다（흔히 이를 일점 교배라 함）.


U 일점 교배佃ne나）이nt crossover) 연산
 (D 교배 지점을 임의로 선택하고 그 지점을 기준으로 유전자를 분할한다. 식（4J5）과 (4.16)


===== PAGE 94 =====
92         퍼지, 진화컴퓨팅 프로그래밍



        에서 교배지점은 冗N(1, m) 값어］ 의해 결정되며, 아래 예는 丑／\T(1, 15) 값이 5 보다
        크고 6 이하인 경우이다．

        부모 Xk = 11010 I 0011000001

        부모 X0 = 11001 I 0110001011

      區） 이진 문자열의 뒤쪽 분할 부분을 서로 교환한다．
        자식 X'k = 11010 I 0110001011

        자식 X " = 11001 I 0011000001


 리스트 午6은 단순 교배에 대한 매트랩 코드이다．


     mm 리스트 4七 嘉 단순 교배（일점 교배）: 이진 및 실수 표현에 동일하게 사용

       function [cl,c2] = simpleXover(pi,p2,bounds,Ops)
       % 파일명： sin叩ieXover.m
       % 부모 개체 p1과 p2를 이용 일점 교배를 수행
       % function [ci,c2] = simpieXover(p I ,p2,bounds,Ops)
       %      출력 변수
       %           ci, c2: 교배로 만들어진 자식 개체
       %      입력변수
       %                    ［개체 문자열 적합도 값］)
                   p1: 부모 개체（
       %                    ［개체 문자열 적합도 값］)
                   p2: 부모 개체（
       %           bounds: 해의 탐색 공간（변수의 탐색 범위）
       %           Ops: 단순 교배를 위한 옵션 ［세대 수 Ops(2)I
       %           Ops(2): 실수 표현에서는 교배 횟수를， 이진 표현에서는 교배율을 표시


       numVar = size(p1,2)-I; % 개체의 변수 수
       % 교배 지점 선택
       % round(x): x에 가까운 정수로 만듬, [0,변수 수-1] 범위의 수를 랜덤하게 선정
       %i을 더해 0이 선택되지 않도록 함
       cPoint = round(rand * (numVar-2)) + 1;
       % 교배를 통해 자식 개체 생성, cPoint 점 뒤의 문자열을 교환
       ci = [pl(1:cPoint) p2(cPoint+i:numVar+i)I; % 식(4.i5)
       c2 = [p2(1:cPoint) pl(cPoint+1:numVar+I)]; % 식(4.16)


===== PAGE 95 =====
                                                                                                 4장 유전알고리즘                93




4.4.2 실수 표현

 실수형 유전알고리즘에서는 돌연변이 연산자로 균일 돌연변이（山i1form mut帥아i), 비균일
돌연변이(n帥ni如rm mutation), 멀티H비균일 돌연변이（m毗i-non uniform mutation),
경계 돌연변이（boundary m毗毗幻n）가 있고 교배 연산자로는 단순 교배（simple crossover),
산술 교배（at砒hmetic crossover）와 휴리스틱 교배（heuristic crossover）가 있다.

 可 번째 변수인 따(i= 1, 2, "·,n)의 최소와 최대가 叫fin, Z艸이라 하자. 균일 돌연변이

연산은 식（4.17）과 같으며, 3는 무작위로 선택된 변수이고 冗／V（寸" ", 寸瞰）은 따의 최소와

최대 범위 내에서 균일분포로 선택된 랜덤 수이다．




   뇌‘=｛甲（"「'""尹" ) ':
                  ，二기，,,                                                                                         (4.17)



비균일 돌연변이 연산은 식（4.18）과 같으며, 3는 무작위로 선택퇸 변수이고 TI과 n는 무작위

랜덤 수 丑N(0, 1）이다．


                                                                                                             +
                                丸 k k
                                              （畔' " 口于）/(g) if r1 < 0.5
                     /
                                 2
                                 1 Z
                                   2
                                   1 21
                                              (x + X11ifl )f (g) if r1 2 0.5
         Z
                                 Z
         境
                         <11L
         2                                                                                                       (4.18)
                                                                                                                   H
                     1
                                                                                                             中
         1
                                                                                                                   1




                                                                 0坑erw可se




위식어］서／(g)                                 =          r2   (1   十，
                                                                    ))b,   g印재세대수小최대진화세대수이고b는모
양 결정 파라미터이다．

멀티e비균일 돌연변이 연산은 비균일 돌연변이 연산을 개체 Xk의 모튼 변수에 적용한다. 경
겨1 돌연변이 연산은 식（4.19）과 같으며, 3는 무작위로 선택된 변수이고 r = 冗／V(o, 1）인 랜
덤 수이다．


                                              if 可 = 工 1 < 0.5
             !:mm
                    1
   뇌k=
                                  2max
                                              if 可 = 工 r 2 0.5                                                   (4.19)
                    ［畔                        ot九e        「毗se


===== PAGE 96 =====
94       퍼지, 진화컴퓨팅 프로그래밍




 리스트 午7에서 午10까지는 위에서 설명한 돌연변이의 매트랩 코드이다．



      리스트 4刃 枷 균일 돌연변이

     function [child] = uni烋4utate(parent,bounds,Ops)
     % 파일명： unif入4utation.m
     % 균일 분포의 확률어］ 기초해서 부모 개체의 파라미터 가운데 하나를 변경
     % function [child] = unifMutation(parent,bounds,Ops)
     %      출력변수
     %           child: parent어］ 돌연변이를 적용해서 만들어진 개체
     %      입력변수
     %           parent: 부모 개체（
                              ［개체 문자열 적합도 값］)
     %           bounds: 해의 탐색 공간（변수의 탐색 범위）
     %           ops: 균일 돌연변이를 위한 옵션 ［세때1 수 균일 돌연변이 시행 횟수］


     df = boun小（:,2) - 1兀unds(:,1); % 변수의 탐색 범위의 크기
     numVar = size(parent,2）山 % 변수의 수
     % [1,numVar] 범위에서 돌연변이 지점의 선택
     mPoint = round(rand *(numVar. l)) + 1;
     % 돌연변이 값 = 변수의 최소값 + 변수 범위玎0,1] 사이의 랜덤 수
     newValue = bounds(mPoint,1) + rand*df(mPoint);
     % 돌연변이 된 자식 개체 생성， 식（4.17)
     child = parent;
     child(mPoint) = newValue;




 的싸｛「 리스트 午8 莎 비균일 돌연변0I

     function [child] = nonUniflvlutation(parent,bounds,Ops)
     % 파일명： nonUni外4utation.m
     % 비균일 분포의 확률어］ 기초해서 부모 개체의 파라미터 가운데 하나를 변경
     % 가우시안 분포를 넓게 시작해서, 세대 수가 최때1 세대 수어］ 근접함어］ 따라
     % 가우시안 분포를 점분포까지로 줄임
     % function [child] = nonUnifMutation(parent,bounds,Ops)
     %      출력변수
     %           child: parent에 돌연변이를 적용해서 만들어진 개체
     %      입력변수


===== PAGE 97 =====
                                                         率
                                                                      4장 유전알고리즘   95


%              parent: 부모 개체（
                            ［개체 문자열 적합도 값］)
%              bounds: 해의 탐색 공간（변수의 탐색 범위）
%              Ops: 비균일 돌연변이를 위한 옵션
%                 ［세대 수 비균일 돌연변이 시행 횟수 최때1 세대 수 모양 파라미터］


cg = Ops(l); % 현재 세대 수
mg = Ops(3); % 최디1 세대 수
b = Ops(4); % 가우시안 분포의 모양 파라미터
df = bounds(:,2) - bounds(:,1); % 변수 탐색 범위의 크기（최대－ 최소）
numVar = size(parent,2)-1; % 변수의 수
% [1,numVar] 범위에서 돌연변이 지점의 선택
mPoint = round(rand * (numVar-1)) + 1;
md = round(rand); % 돌연변이 방향 선택， md = 0 아니면 l
if md % 탐색 범위 상한선 쪽으로 돌연변이
      %l兀unds（艸이nt,가pare叫mP아nt): 상한 쪽으로 움직일 수 있는 양
      newValue = parent(mPoint) + ...
                    delta(cg,mg,bounds(mPoint,2)-parent(mPoint),b);
이se % 탐색 범위 하한선 쪽으로 돌연변이
      % parent(mP아nt)-l兀Un小佃P아nt,1): 하한 쪽으로 움직일 수 있는 양
      newValue = parent(mPoint) - ...
                    delta(cg,mg,parent(mPoint)-bounds(mPoint,1),b);
end
% 돌연변이된 개체 생성， 식（4.18)
child = parent;
child(mPoint) = newValue;


           function [change] = delta(ct,mt,y,b)
           % 파일명： delta.m
           % 비균일 분표의 함수로
            % 현재 세대 수， 최대 세대 수 및 가능한 편차의 양어］ 따라 변화랑을 리턴
           % 凡nction [change] = delta(ct,mt,y,b)
           %      출력변수
           %           change: 변화량
           %      입력변수
           %           Ct: 현재 세대 수
           %           mt: 최대 세대 수
           %           y: 최디1 변화량， 현재 위치에서 경계까지의 거리


===== PAGE 98 =====
U函1i    퍼지, 진화컴퓨팅 프로그라但J



            %               b: 모양 결정 파라미터


            % 식（4.18）에서 /(9) 값 계산
            r = ctlmt;
            if (r>1)
                   r=.99;
             end
             change = 少（rand*( l-r))小；




       리스트 4四 》 멀티m비균일 돌연변이

   function [child] = multiNonUnifMutation(parent,bounds,Ops)
   % 파일명： mu出NonUnif入4utation.m
   % 비균일 분포의 확률어］ 기초히써 부모 개체의 모튼 파라미터를 변경
   % 가우시안 분포를 넓게 시작해서, 세대 수가 최때1 세대 수어］ 근접함어］ 따라
   % 가우시안 분포를 점분포까지로 줄임
   % function [child] = multiNonUnifMutation(parent,bounds,Ops)
   %      출력변수
   %            child: parent에 돌연변이를 적용해서 만들어진 개체
   %      입력변수
   %                         ［개체 문자열 적합도 값］)
                parent: 부모 개체（
   %            bounds: 해의 탐색 공간（변수의 탐색 범위）
   %            Ops: 멀티－비균일 돌연변이를 위한 옵션
   %          ［세대 수 멀티－비균일 돌연변이 시행 횟수 최대 세대 수 모양 파라미터］


   cg = Ops(1); % 현재 세대 수
   mg = Ops(3); % 최대 세때1 수
   b = Ops(4); % 모양 결정 피라미터
   df = 1兀unds(:,2) - bounds(:,l); % 탐색 영역의 크기
   numVar = size(parent,2) - I; % 변수의 수
   % 모든 점에서 돌연변이 시행, 상한미냐 하한 쪽의 선택을 위해 랜덤 변수 이용
   md = round(rand(l,numVar));
   child = parent;
   for i = 1:numVar
        if md(i) % 경계 상한 쪽으로 delta 함수는 비균일 돌연변이 리스트 참조


===== PAGE 99 =====
                                                                                 4장 유전앞고리즘     ] 97
                  child(i) = parent(i) + delta(cg,mg,bounds(i,2)-parent(i),b);
            else % 경계 하한 쪽으로
                  child(i) = parent(i) - delta(cg,mg,parent(i)-bounds(i,1),b);
            end
  end




mm 리스트卜］0 管 경7카 돌연변0I

  func如n [child] = t兀unda口Mi丘ation(parent,bounds，이均
  % 파일명： t兀undary入4utation.m
  % 부모 개체의 파라미터 가운뎨 하나를 상한이나 하한 경계 값으로 변경
  % function [child] = boundaryMutation(parent,bounds,Ops)
  %           출력변수
  %                  child: parent에 돌연변이를 적용해서 만들어진 개체
  %           입력변수
  %                  parent: 부모 개체（
                                  ［개체 문자열 적합도 값］)
  %                  bounds: 해의 탐색 공간（변수의 탐색 범위）
  %                  Ops: 비균일 돌연변이를 위한 옵션 ［세대 수 경계 돌연변이 시행 횟수］


  numVar = size(parent,2)-1; % 변수의 수
  n甲이nt = round(rand 水 (numVar-l)) + 1; % 돌연변이 지점의 선택
  % 식（4.19）에 의한 돌연변이
  b = round(rand) + 1; % 어떤 쪽 경계를 이용할지 선택， b=1 -> 하한， b=2 -> 상한
  newValue = bounds(mP아nt,b); % 선택된 지점의 값을 돌연변이 시킴
  % 돌연변이 개체 생성
  child = parent;
  child(mPoint) = newValue;




 실수형 단순 교배 연산은 可 = 1, 2夕 ···7 n인 점을 빼면 식（4.15）와 (4.16）과 동일하다. 산술

교배 연산은 식（4.20), (4.21）과 같이 부모 개체를 선형 보간1inear interp아毗ion)어］ 의하1

결합하며, r＝丑叩(0, 1）이다．


        k         k
                   1       l       01
                   2
      Z                        r   T    12
                                    2        =1, 2, ·", n
        中
        2
                   r
                                                                                             (4a1)


===== PAGE 100 =====
98        퍼지, 진화컴퓨팅 프로그래밍



          r
          0 1
          Z 2
                    )
                    (
                    +        l   r
                                     丸     2
                                            01
                                             2
                    =                 工i
                                       1   r
                                                                     (4.21)
                                                 1
                1


                                                 2
     휴리스틱 교배는 두 개체를 선형 외삽（linear extrapolation）어］ 의해 결합한다. 이 연산자
 만이 교배 과정어］ 적합도 값을 이용한다. 교배에 의한 새로운 개체는 식（4.22）와 (4.23）어］ 의
 하1 생성된다（x丸의 적합도가 x " 보다 우수）. 만약 戶7} 실행가능하지 못하면（姃easible)
 즉, 식（4.24）의 값이 0이면 새로운 랜점 수 r = 冗N(0, 1）을 다시 발생하고, 식（4.22）를 이용
 새로운 개체를 생성한다. 정해진 횟수 이상으로 연속 실패하면 자식 개체를 부모 개체와 동일
 하게 설정한다.

          戈
          1i
           2
                         k
                         까
                                                 i= 1, 2, ", n   =


          b
          1
          n
           m
                        寸 江 1, 2, ·", n                          H

                                                                 1




        毗y극나. 寸＝可In, x} 드 x艸 Vi
       加，
                                      (, u oinerwise




 리스트 午11과 }12는 위에서 설명한 교배의 매트랩 코드이다．


       리스트卜］1.                       산술 교배

      function [ci,c2] = arithXover(p 1,p2,bounds,Ops)
      % 파일명： ar川lXover.m
      % 두 부모 개체들의 내삽을 통해 자식 개체 생성
      % function [ci,c2] = arithXover(p i ,p2,bounds,Ops)
      %                 출력 변수
      %                      ci, c2: 교배로 만들어진 자식 개체
      %                 입력변수
      %                      p1: 부모 개체
                                     （ ［개체 문자열 적합도 값］)
      %                      p2: 부모 개체
                                     （ ［개체 문자열 적합도 값］)
      %                      bounds: 해의 탐색 공간（변수의 탐색 범위）
      %                      Ops: 산술 교배를 위한 옵션 ［세때1 수 산술 교배 횟수］


      a = rand; % [0,1] 범위의 수를 랜덤하게 발생, 선형 보간 비율로 사용
      % 자식 개체 생성
      ci = pi*a + p2*(1-a); % 식(4.20)


===== PAGE 101 =====
                                                            4장 유전알고리즘    99


      c2 = p1斗（i-a) + p2半a; % 식（4.21)




mm 리스트卜］2. 휴리스틱 교배1

      function [cl,c2] = heuristicXover(p1,p2,bounds,Ops)
  % 파일명： heuristicXover.m
 % 부모 개체들의 외삽을 통해 자식 개체 생성（우수한 부모 개체의 방향으로 외삽）
  % function [ci,c2] = heuristicXover(p1,p2,bounds,Ops)
 %            출력 변수
 %              ' c1, c2: 교배로 만들어진 자식 개체
 %            입력변수
 %               p1: 부모 개체（
                          ［개체 문자열 적합도 값］)
 %               p2: 부모 개체（
                          ［개체 문자열 적합도 값］)
 %               1兀unds: 해의 탐색 공간（변수의 탐색 범위）
 %               Ops: 휴리스틱 교배를 위한 옵션 ［세때1 수 휴리스틱 교배 시행 횟니司


 retry = Ops(3); % 교배 재시행 횟수
 i=
         0;
 good = 0;
 bi = bounds(:,1)'; % 변수의 탐색영역에 대한 최소값 열 벡터
 b2 = bounds(:,2)'; % 변수의 탐색영역어］ 대한 최대값 열 벡터
 numVar = size(p1,2)-i; % 변수의 수
 % 적합도 비교를 통해 보다 우수한 부모 개체를 선택
 if (pi(numVar+i) > p2(numVar+1))
         bt = 하； % 우수 개체
         ＼자t = p2; % 열등 개체
 이se
         bt = p2;
         wt = pi;
 end
 while i<retry % 시행 횟수어］ 도달할 때까지
         a = rand; % [0,1] 범위의 수를 랜덤하게 발생， 외삽 비．율로 사용
         % 자식 개체 생성
         ci = a * (bt - wt) + bt; % 식
                                    （4.22)
         % 자식 개체가 탐색 영역 내어］ 존재하는 확인
         if (ci(1:numVar) <= b2 & (cl(i:numVar) >= bi)) % 탐색 영역 내에 있으면


===== PAGE 102 =====
100    [      퍼지, 진화컴퓨팅 프로그래밍



                    i= retry; % 교배 종료를 위해 i를 시행 횟수로 설정
                    good = 1;
              이se
                    i=   i + 1;
              end
        end
       if (good) % 자식 개체가 실행 가능하지 못하면(infeas삐e)
              ci = wt;
        end
        c2 = bt; % 식（4.23), 우수한 부모의 염색체를 자식에게 그대로 물려줌




      Fuzzy & Evolutionary
         Computing Programming
                                           71I-
                                    4.5 종료조:



      유전알고리즘은 종료조건을 만족할 때까지 매 세대에서 선택과 유전 연산을 통해 진화한
  다. 가장 흔히 사용되는 종료조컨은 최대 진화 세대수를 사전에 정해놓고 진화 세대 수가 이
  에 도달하면 알고리즘을 종료하는 것이다. 또 다른 종료조건으로는 알고리즘의 수렴성을 이
  용하는 것이다. 일반적으로 유전알고리즘은 전체 집단을 하나의 개체（최종 해）로 수렴시키며
  즉, 개체들 간의 편차 합을 감소시킨다. 따라서 편차의 합이 어떤 임계 값 이하로 줄어들면
  알고리즘을 종료할 수 있다. 사전에 정한 세대 동안 가장 우수한 개체가 개선되지 않을 때에
  도 알고리즘을 종료할 수 있다. 또는 적합도의 목표 값을 설정하고 가장 우수한 개체가 이
  목표를 달성하면 알고리즘을 종료할 수도 있다. 이상어］ 설명한 종료조건들을 결합해서 사용
  할 수도 있다．
  리스트 午13과 午14는 종료조건에 대한 매트랩 코드이다．


           리스트卜］3 各 진화 세대 수에 의한 종료

        function [done] = maxGenTerm(ops,bPop,endPop)
        % 파일명： maxGenTerm.m
        % function [done] = maxGenTerm(ops,bPop,endPop)


===== PAGE 103 =====
                                                                   4장 유전알고리즘   101


  % 최대 진화 세대 수어］ 도달하면 유전알고리즘을 종료시키기 위해 l을 리턴
  %          출력변수
  %            done: 정해진 진화 세대 수佃axGen）어］ 도달하면 l , 아니면 0.
  %          입력변수
  %            ops: 옵션 벡터 ［현재 진화 세대 수 최대 진화 세대］
  %            bPop: 가장 우수한 개체（해） 행렬 ［발견된 세대 수 해 관련 문자열］
  %            endPop: 현재 세대의 해


  currentGen = ops(l); % 현재 세대 수 얻음
  maxGen = ops(2); % 최대 진화 세대 수 얻음
  % currentGen >= maxGen이면 done = 1
  done = (currentGen >= maxGen);




mnm 리스트 小］4. 진화 세fl 수와 목적함수 값에 의한 종료

  function [done] = optMaxGenTerm(ops,bPop,endPop)
 % 파일명： op小4axGenTerm.m
 % function [done] = optMaxGenTerm(ops,bPop,endPop)
 % 최태1 진화 세대 수어］ 도달하거나 목표함수 값에 도달하면
 % 알고리즘 종료를 위해 l을 리턴
 %           입력변수
 %             ops: 옵션 벡터
 %                  ［현재 진화 세대 수 최대 진화 세대 목표 목적함수 값 허용오차］
 %             bP아y 가장 우수한 개체（해） 행렬 ［발견된 세대 수 해 관련 문자열］
 %             endPop: 현재 세대의 개체（해） 집단


  currentGen = ops(I); % 현재 세대 수 얻음
 maxGen = ops(2); % 최대 진화 세대 수 얻음
  optimal = ops(3); % 목표 적합도 함수 값
  epsilon = ops(4); % 허용오차
  fitlndex    = size(endPop,2); % endP이）의 열 수
  bestS아＼/al = max(endPop(:,fitlndex)); % 집단의 적합도 최대값
 % 최대 진화 세대 수에 도달 또는 허용오차 범위 내어써 목표 함수 값에 도달하면 l
  done = (currentGen >= maxGen) 1 (bestSolVal >= (optimal - epsilon));


===== PAGE 104 =====
102             퍼지, 진화컴퓨팅 프로그래밍




      Fuzzy & Ev이Ut幻nary
         Computing Programming        4.6 유전알고리즘의 처리


      이상어써 설명한 유전알고리즘의 계산 과정을 가상 코드 형태로 정리하면 다음과 같다．


      g= O;       /／시간（세태 수） 초기화
      in侊Popu厄仇아2P(t); // 초기 집단 구성

                     P(t) = {X1(g),X2 (g),"· ,X     (g)}

                     X' (g) = {x (g),x (g), ·..,x,(g)}

      ev毗尸bp工lation P(t); // 초기 집단의 적합도 평가
                      少 (xI) =T (F(e (xIv)) k= 1, 2, ···,np
      while (not termination condition)

      {
                 cross尸吻血仇on P(t); // 교배 적용

                     甘 (9) = 少（g) cross X" (g); II cross는 교배 연산자
                 mi虎毗e尸b끄'ula仇on 尸(t); // 돌연변이 적용

                     X"lc (g) =mu (X'k (g)); // 刃2U는 돌연변이 연산자
                 e刃毗尸切工厄仇on P" (g); // 새로운 집단의 적합도 평가

                     少（x"丸（9)) = T(F(e (x"七（9))) 丸＝ 1, 2, ···, np

                 select尸吻tl(比幻n 尸（g) fromP" (g); // 특정한 선택 메커니즘 적용

                 g= g+ 1; // 세태1 수 증가
      }   Use
                 best solution (individual) and its trace inforamtion;


      위의 가상 코드어］ 대한 매트랩 코드가 리스트4-15이다. 가상 코드에서는 설명되어 있지 않
  지만 매트랩 코드에서는 이진형 및 실수형 유전 연산자 모두를 다루고 있다. 따라서 교배와
  돌연변이 연산을 실행하기 전에 실수형인지 아닌지（이진형）를 먼저 확인한다. 실수형에서는
  연산자가 미리 정해진 횟수（함수의 인수）어］ 의하1 결정론적으로 적용되지만, 이진형에서는 횟
  수어］ 대한 파라미티가 확률（교배율, 돌연변이율）을 나타내며 연산자가 확률적으로 적용된다.


===== PAGE 105 =====
                                                                       4장 유전알고리즘   103


선택, 교배, 돌연변이 및 종료조건 판단어］ 대한 매트랩 코드 함수는 앞에서 설명하였고 여기

서는 이들 함수들이 호출되어 사용된다．



     리스트卜］5. 유전알고리즘의 처리

 function [x,endPop,bPop,tracelnfo]
       ga(bounds,evaIFN,evalOpts,startPop,options,termFN,...
       terinOpts,se1ectFN,se1ectOpts,xOverFNs,xOverOpts,mutFNs,mutOpts)
 % 파일명： ga.m
 % 유전알고리즘 실행
 % function [x,endPop,bPop,tracelnfo]=
 %      ga(bounds,evalFN,evalOpts,startPop,options,termFN,
 %      termOpts,selectF나,selectOpts,xOverFNs,xOverOpts,mutFNs,mutOpts)
 %      출력변수
 %           x: 유전알고리즘으로 찾은 가장 우수한 해（개체）
 %           endP이X 마지막 세대의 집단, 보조적으로 저장
 %           bP야L 가장 우수한 개체의 변화 기록（세대수와 개체）
 %           tracelnfo: 각 세대에서 유전알고리즘의 최우수 적합도와
 %                     평균 적합도 값을 갖는 행렬
 %      입력변수
 %           t兀unds: 변수의 상하한 값어］ 대한 행렬
 %           eva1FN: 평가함수로 .m 파일
 %           evalOpts: 평가함수에 건넬 옵션, 디폴트 값은 []
 %           star叩이y 초기 집단 행렬(initialize.m 파일에서 얻음）
 %           options: [epsilon pr아） ops display] 디폴트 값은 [le-6 1 01
 %                    epsilon: 두 해를 다른 것으로 판정하는뎨 필요한 변화량
 %                    prob_ops: 유전연산자를 확률적으로 적용할려면 0,
 %                              결정론적으로 적용 횟수를 지정할려면 1로 설정．
 %                    display: 진행 과정을 표시하려면 l , 아니면 0.
 %           termFN: 종료조건 함수어］ 대한 .m 파일， 여］: ['maxGenTerm']
 %           termO햐S: 종료조건 함수어］ 건네질 문자열 옵션， 예： [100].
 %           selectFN: 선택 함수의 .m 파일， 예 ['normGeomSelect']
 %           selectO少S: 선택함수어］ 건네질 문자열 옵션 , 여］: 따08]
 %           xOverfl寸S: 빈공간으로 분리된 Xover.m 파일명을 갖는 문자열,
 %                     여j: ['arithXover heuristicXover simpleXover']
 %       -   xOver伽ts: Xover.m 파일어］ 인수로 넘겨질 옵션 행렬로
 %                      실수형에서는 첫 열이 Xover의 횟수， 예： [2 0;2 3;2 0]


===== PAGE 106 =====
                                          率
104       퍼지, 진화컴퓨팅 프로그래밍



      %                       이진형에선 교배율
      %             mutFNs: 빈 공간으로 분리된 mutation.m 파일명을 갖는 문자열
      %                       예: ['boundaryMutation multiNonUnifMutation
                                   nonUni烋4utation unifMutation'])
      %             mutO아s: mutation.m 파일어］ 건녜질 옵션 행렬로
      %                       실수형에서는 첫 열이 mu伍tion의 횟수，
      %                       예： [4 0 0;6 100 3;4 100 3;4 0 0], 이진형에서는 돌연변이율


      if options(2) == l % 실수형 GA
            % [cl(xZomeLength) ci] = feval(evalFN,c 1,[gen eva1Opts])를
            % 문자열로 e1str에 저장
            e1str=['[c 1 ci (xZomeLength)]=' evalFN '(c 1,evalOpts);'];
            e2str=['[c2 c2(xZomeLength)]=' eva1FN '(c2,evalOpts);'];
      이se % 이진 GA
            eistr=['x = b2f(endPop(j,:),bounds,bits);[x v]=' evaI目
                 '(x,evalOpts); endPop(j,:)=[f2b(x,bounds,bits) v];'];
            bits=calcbits(bounds,options(1));
      end


      % 파라미터 설정
      % 교배 .m 파일 이름을 분할, 행렬어］ 넣음（한 행에 이름 하나）
      xOverFNs = parse(xOverFNs);
      mutFNs = parse(mutFNs);
      % 초기 집단의 열수 = 변수의 수 + 1(적합도）
      xZomeLength = size(startPop,2);
      numVar = xZon妃Length-1; % 변수의 수
      popSize = size（計毗P이）,1); % 집단내 개체의 수
      % 마지막 세디倒 집단을 저장하기 위한 행렬
      endPop = zeros(popSize,xZomeLength);
      ci = zeros(1,xZomeLength); % 71]체1
      c2 = zeros(1,xZomeLength); % 7J체2
      numXOvers = size似OverFNs,1); % 교배 연산자의 수
      numMuts = size(mutFNs,1); % 돌연변이 연산자의 수
      % 두 개의 적합도 값이 다른 것으로 판단하는데 필요한 잉｛차이）
      epsilon = options(1);
      % 초기 집단 startP叩에서 가장 좋은 적합도
      oval = max(startPop(:,xZomeLength));


===== PAGE 107 =====
                                                                        4장 유전알고리즘   105


bFoundln = 1; 9自 가장 우수한 것이 변경된 횟수
（如ne = 0; % 모의 진화 실행， l이면 종료
gen = 1; % 현재 세대 수
collectTrace = 1; % 1이면 매 세대에서 정보 수집
floatGA = (options(2) == 1); % 1이면 실수형
display = options(3); % 1이면 진행 과정 표시


whi1e(싸done)
    % 최우수 개체의 유지， bval: 최우수 적합도 bint奴： 최우수 개체 번호
    [bval,bindx} = max(startPop(:,xZomeLength));
    best = startPop(bindx,:); % 최우수 개체
    if collectTrace
          tracelnfo(gen,1) = gen; % Afl대
          % 최우수 개체의 적합도
          打acelnfo(gen,2) = startPop(bindx,xZomeLength);
          % 적합도 평균
          tracelnfo(gen,3) = mean(startPop(:,xZomeLength));
          % 적합도 표준편차
          tracelnfo(gen,4) = std(startPop(:,xZomeLength));
    end
   % 최우수 적합도어］ 변화가 있거나 세때1 수가 l 이면
   if ((abs(bval - oval) > epsilon) 1 (gen==1))
          if display
                 印rintf1,'＼出od %t\n',gen,bval); % 화면 표시
          end
          if floatGA
                 % 실수형
                 % 세대 수와 가장 우수한 개체를 bP야） 행렬어］ 저장
                 bPop(bFoundln,:) = [gen startPop(bindx,:)];
          else
                 % 이진， b2f 함수를 통해 이진 문자열을 실수로 변환하여 저장
                 bPop(bFoundln,:) = [gen b2gstartPop(bindx,l :numVar),...
                                      bounds,bits) startPop(bindx,xZomeLength)];
          end
          bFoundln = bFoundln + 1; % 최우 개체의 변화 횟수 증가
          % 이전 최우수 적합도 oval을 현재 최우수 개체의 적합도 값 bval로 대체
          oval = bval;


===== PAGE 108 =====
                                             率
106   [   퍼지, 진화컴퓨팅 프로그래밍



          이se % 최우수 적합도에 변화가 없으면
                if display
                      fprintf( 1,'%d ',gen); % 세대 수를 표시
                end
          end


          % 선택： 선택 함수 호출, 선택 결과로 만들어진 집단을 endPop에 저장
          %s이ectFN은 선택 함수의 .m 파일, 여卜 ['normGeomSelect']
          endPop = feval(selectFN,startPop,[gen selectOpts]);


          % 유전 연산
          if 加atGA % 실수형인 경우, 유전연산자를 결정론적으로 사용
                % 교배
                for i = I :numXOvers, % 모든 교배 연산자에 대해
                      % 교배 연산자의 실행 횟수， xOverOpts의 첫 열은 연산자 실행 횟수
                      for j = 1:xOver伽始(i,I),
                             % 부모 개체 번호 선택
                             a = round(rand*(popSizei) + I);
                             % 부모 개체 번호 선택
                             b = round(rand*(popSize-I) + 1);
                             % 교배 함수명 얻음, debiank(s): 문자열 5의 끝에 있는 공백 제거
                             xN = deblank(xOverFNs(i,:));
                             % fevai(fname,xl.....xn): fnan妃의 문자열과 동일한 .m파일어］
                             % 인수 xl.....xn을 주고 실행, ci, c2는 교배 결과， 자식 개체
                             [ci c2] = feval(xN,endPop(a,:),endPop(b,:),bounds,...
                                                    [gen xOverOpts(i,:)]);
                             % 교배 후 ci이 개체 a와 같으면
                             if ci (1:numVar) == endPop(a,(1:numVar))
                                   % a 개체의 적합도를 받음
                                   ci (xZomeLength) = endPop(a,xZomeLength);
                             %b와 같으면
                             이se仟 이（I :numVar) == endP야和,(i:numVar力
                                   이 似ZomeLength戶endP야)(b,xZomeLen맘h);
                             이se
                             % [ci (xZomeLength) ci ]=fevai(evaiFN,c 1,[gen eva山ptsfl를
                             % 실행
                                   eval(e I str);


===== PAGE 109 =====
                                                              率
                                                                    4장 유전암고리즘   107



               end
               if c2(l:numVar) == endPo乂a,(1:numVar))
                       c2(xZomeLength) = endPop(a,xZomeLength);
               elseif c2( l:numVar) == endPop(b,(l:numVar))
                       c2(xZomeLength) = endPop(b,xZomeLength);
              else
                      %[c2(xZomeLength) c2] =
                      % fey키（evaIFN,c2,[gen evalOpts]）를 실행
                      eval(e2str);
                      end
                      % 자식 개체 ci고｝ c2가 부모 개체 a와 b를 대체
                      endP아乂a,:) = ci;
                      endPop(b,:) = c2;
              end
        end
        % 돌연변이
        白r i=1:num入iluts, % 모든 돌연변이 연산자어］ 대해
              for j=i :mutOpt帥,1), % 돌연변이 시행 횟수
                    % 돌연변이 대상 개체 선정
                     a = round(rand*(popSizei) + 1);
                    % 돌연변이 실행
                     ci = feval(deblank(mutFNs(i,:)),endPop(a,:),bounds,...
                                       [gen mutOpts(i,:)]);
                    % 돌연변이 후 개체에 변화가 없으면
                    if 이（i :numVar) == endP아 (a,(1:numV缸力
                            % 적합도를 그대로 물려받음
                            ci(xZomeLength) = endPop(a,xZomeLength);
                    이se % 개체에 변화가 있으면 적합도 평가
                            % [ci(xZomeLength) ci] =
                            % 扼val(evalFN,c i ,[gen evalOpts]）를 실행
                            eval(e i str);
              end
              % 돌연변이 대상 개체를 돌연변이 된 개체로 교체
              endPop(a,:) = ci;
        end
  end
이se % 이진 문자열을 사용하는 경우， 유전연산자를 확률적으로 이용


===== PAGE 110 =====
                                       水
108   퍼지, 진화컴퓨팅 프로그래밍



            % 교배
            白r i = 1:numXOvers, % 모든 교배 연산자어］ 대해
                  % 교배1 연산자 함수명을 얻음
                  xN = deblank(xOverFNs(i,:));
                  % 집단 크기의 랜덤 수를 발생해 교배율 보다 작은 경우， 해당 개체
                  % 번호를 cp어］ 저장， 이진 표현에서 xO比tO야帥m는 교배율
                  cp = find(rand(popSize,1) < xOverOpts(i,1) =        1);
                  if rem(size(cp,I),2) % cp에 있는 개체 번호 수가 홀수이면
                        % cp에서 마지막 원소를 제거
                        cp = cp(1:(size(cp,1)-1));
                  end
                  % reshaep(cp,m,n): cp를 열 방향으로 읽어 m x n 행렬을 리턴
                  cp = reshape(cp,size(cp,1)12,2);
                  for j = 1:size(cp,1) % cp의 1 행부터 마지막 행까지
                        a = cp(j,1); % 교배 대상 개체 번호
                        b = cp(j,2); % 교배 대상 개체 번호
                        % 교빼1 실행
                  [endPop(a,:) endPop(b,:)] = feval(xN,endPop(a,:),...
                                       endPop(b,:),bounds,[gen xOverOpts(i,:)]);
                  end
            end
            % 돌연변이
            for i = 1:numMuts % 모든 돌연변이 연산자에 대해
                  mN = deblank(mu伊N帥,:)); % 돌연변이 함수명 얻음
                  for j =1:popSize
                        % 모든 개체어］ 대해 돌연변이 시행
                        endPop(j,:) = 免vat佃N,endP아心今，b이in小，...
                                                     [gen mutOpts(i,:)]);
                        eval(elstr); % 적합도 평가
                  end
            end
      end
      gen = gen + 1; % 세대 수 증가
      % 종료조건 만족 여부 확인, 面ne = 1 이면 종료
      done = feval(termFN,[gen termOpts],bPop,endPop);
      % 유전연산을 통해1 만들어진 자식 집단을 다음 세대의 부모로 만듦
      star四아） = endP야）;


===== PAGE 111 =====
                                                                        4장 유전알고리즘   109


      % 엘리트주의 적용： 최우수 개체는 다음 세대어］ 반드시 생존
       % 부모 개체에서 가장 열등한 개체를 최우수 개체로 대체
      % 가장 열등한 개체의 번호（bind자을 알아냄
       [bval,bindx} = min(startPop(:,xZomeLength));
      startPop(bindx,:) = best; % 개체 대체
end
% 알고리즘 종료 후 최우수 개체의 적합도（bval)와 해당 개체 번호（bind지를 알아냄
[bval,bindx] = max(startPop(:,xZomeLength));
if display
      巾rin氓1,'\n%d %f\n',gen,bv키）;
end
x = startPop(bindx,:); % 최우수 개체를 리턴
if options(2) ==O % 이진 표현의 경우
      x = b2f(x,bounds,bits); % 이진 문자열을 실수로 변환
      % 최우수 개체어］ 대한 정보［세대 수 개체 적합도］ 저장
      bPop(bFoundln,:) = [gen b2f(startPop(bindx,l:numVar),bounds,...
                                 bits) startPop(bindx,xZomeLength)];
이se
      bPop(bFoundln,:) = [gen startPop(bindx,:)];
end
if collectlrace
      % 현재 세대 수
      tracelnfo(gen,1) = gen;
      % 최우수 적합도
      tracelnfo(gen,2) = startPop(bindx,xZomeLength);
      % 적합도 평균
      tracelnfo(gen,3) = mean(startPop(:,xZomeLength));
end


             func如n ［日 = parse(inStr)
             % 함수명： parse.m
             % 빈칸으로 구분된 n개의 항목어］ 대한 문자열에서
             %n개의 문자열을 분리하여 n 항목의 행벡터를 만들어 리턴
           % function [x} = parse(inStr)
             %     출력변수
           %            x: 리턴 행 벡터
           %       입력변수


===== PAGE 112 =====
110   [   퍼지, 진화컴퓨팅 프로그래밍



             %               inStr: 빈칸으로 구분된 문자열


              sz = size(inStr); % 문자열 벡터의 행과 열 수
              strLen = sz(2); % 열의 4X문자열 크기）
              x = blanks(strLen); % strLen의 값만큼의 빈 공간으로 이루어진 문자열
              wordCount = 1;
              last = 0;
              for i=l:strLen,
                    if inStr(i) =     " % 빈칸이면
                          wordCount = wordCount + 1; % 다음 행
                          %x의 다음 행에 빈 문자열 생성
                          x(wordCount,:) = blanks(strLen);
                          last = i;
                    이se
                           %last에서 시작 i까지의 문자열을 x어］ 복사
                          x(wordCount,i - last) = inStr(i);
                    end

              end



              米 함수 ga의 다른 서브함수들은 앞의 리스트에서 설명되었음．




      ga.m 파일에서 호출한 서브e함수들을 정리하면 아래 그림 4.2와 같다. 평가함수의 경우
  문제어］ 따라 파일명을 다르게 작성하는 것이 편리하기 때문에 여기서는 구체적인 파일명을
  언급하지 않는다．


===== PAGE 113 =====
                                                                               4장 유전알고리즘




                                             ga . in



                                     실수 프
       roulette    .m
      normGeomSelect .m

       亡ournSelec亡 . in
                                                                                      조료조거
                                                                                      O  L


                               교바1                              형 변촨            maxGen Term, in

                                                                                （갸：此Mm心en Term, in
                        Si쨔끄e？幻ver. m                     - calcbits.   m

                        he口ris亡icXc기／er. m                卞 b2f. m

                        sri 亡hX이／er. in                     f2b. m



                                                                교바1


                                                         aim口］eX（그＼,er. In
                  口n i LM口 ta 亡ion-In

                  i끄,nUnifMuta 亡ion . m

                  In나1 亡iNonUnifMuta 亡ion . m                  돌연변이
                  bounds ryM口亡a亡ion, in                卄 bins ryM口亡ati（그n. m


                           ［그림 十2] ga.m 파일에서 호출되는 서브1함수




Fuzzy & Evolutionary
   （沁mputing Pro毋amming                 4.7 유전알고리즘의 실행1


 이상에서 설명한 유전알고리즘을 사용하여 식（4.25）의 / (x）를 최대로 하는 x의 값을 찾아
보자. 아래 리스트를 보면서 앞서 설명한 매트랩 함수들이 함수 최적화어］ 어떻게 사용되는지
알아본다．


   / （끼 = x + lOs航 (5끼 + 7（刃s (4끼, 0 드 x 드 9                                                      (425)


   리스트 十］o 茹 유전알고리즘을 이용한 함수 최적화 사려1

 % 파일명： gaTest.m
 % 목적함수 枷) = x+lOsin6지＋7cos(4지를 최대로 하는 x 구하기


===== PAGE 114 =====
1m띠［ 퍼지, 진화컴퓨팅 프로그래밍

     % 유전알고리즘의 파라미터 설정
     popSize = 10; % 집단 크기
     bounds = [0 9]; % 변수 x의 탐색 범위
     eva作N = 'testEval'; % 적합도 계산 함수명（testEval.m)
     evalO야5 = [I; % 적합도 평가어］ 필요한 부가적인 옵션
     epsFit = 1.口6; % 목적함수 값어］ 대한 허용오차
     galype = 1; % 1 이면 실수형， 0이면 이진형
     epsVar = 1; % 실수를 이진 문자열로 변환할 때의 허용오차
     options = [epsFit gaType epsVar];
     maxGen = 50; % 최대 진화 세대 수
     termFN = 'maxGenTerm'; % 종료조건 함수명
     termOpts = maxGen;
     selectFN = 'normGeomSelect'; % 선택 방법에 대한 함수명
     selectOpts = [0.08]; %
     xOverFNs = ['arithXover']; % 교배 연산 함수명
     nxOver = 2; % 교배 실행 횟수
     xOverOpts = [nxOver 0]; %
     mutFNs = 'nonUnifMutation'; % 돌연변이 연산 함수명
     nMut = 2; % 돌연변이 시행 횟수
     mutOpts = [nMut maxGen 3];


     % 초기 집단 구성
     initPop = initializega(popSize,bounds,evalFN,evalOpts,options);


     figure(1); % 그림 창
     % 초기 집단의 개체별 적합도
     barwidth = 0.2;
     bar([1 :popSize],initPop(:,2),barwidth);
     axis ([1 popSize -25 25]); % 그림의 축 법위 설정
     xlabel('initial population');
     ylabel('fitness: f(x)');


     % 유전알고리즘의 본체（ga.m) 실행
     [bestX endPop bPop tracelnfo] = ga(bounds,evalFN,evalOpts,initPop,options,termFNtermOpts,...
                                                selectFN,select야)ts,xOverFI'寸s,x아er야）ts,m姓Ns,mutOpts);
     bestX % 최 우수 개체（해）를 화면에 표시


===== PAGE 115 =====
                                                              4장 유전알고리즘   口Lm

pause; % 계속하려면 키를 침
elf; % 그림 창 지움


% 최종 집단의 개체별 적합도
barwidth = 0.5;
bar([1:popSize],endPop(:,2),barwidth);
axis ([ 1 popSize 0 25]);
xlabel('final population');
ylabel('fitness: f(x)');
pause;
elf,
如奴('x + 10水sin(5牛x)+7水cos(4水x)',[0 9]) % 목적함수 그림
axis ([1 popSize -25 25]); % 그림의 축 법위 설정
xlabel('x');
ylabel('f(x)');
hold on;
plot (bestX(1工bestX(2),'ro') % 최적 해의 표시
text(bestX(1),bestX(2)-5,num2str(bestX(1))); % 그림에 해 표시
pause;
elf;
% 세대 별 최우수 적합도의 변화
plot(tracelnfo(:, 1),tracelnfo(:,2),'b-');
axis ([1 maxGen 0 25]); % 그림의 축 법위 설정
xlabel('generation');
ylabel('fitness: f(x)');
hold on;
% 세대 별 평균 적합도의 변화
plot(traeelnfo(:, 1),traeelnfo(:,3),'k小


               function [sol, fit] = testEval(sol,options)
               % galest.m 파일어써 호출하는 적합도 평가 함수．
               % f(x) = x+ lOsin(5x)+7c0s(4x)
               % function [val,sol] = testEval(sol,options)
               %       fit: 해 x어］ 대한 적합도
               %       5아： 해（개체）
               %       options: 문제 관련 파라미터로 디폴트 []


===== PAGE 116 =====
口m[ 퍼지
     ，진화컴퓨팅프로그래밍
      x = sol(1);
      obj = x + l아sin(5奴戶꺄cos(4* 야
      % 최대화 문제이기 때문어］ 목적함수를 적합도 함수로 바로 사용 가능
      fit = obj;


       米 gaTest.m의 다른 서브－함수들은 앞에서 설명되었음．




                       25

                       20

                       15




                                    I
                      10
                           5



               숫口Ummm＝ 른
                                        I I
                                                               I
                                                                    I
                           0

                           占                            I



                                2   3   4         5       6     7   8   9    10
                                             initial population


                               ［그림 午3] 랜덤 초71 집단의 적합도


                25



                20




              5      0
              1      1

              小XV卜n留읕는




                                                5      6                    10
                                            final population


                               ［그림 小4] 진화 종료 후 집단의 적합도


===== PAGE 117 =====
                                                                                             4장 유전알고리즘   口Lm

위의 gaTest.m 파일의 실행 결과, 그림 午3은 초기 집단을 구성하는 10개의 개체들의 적합
도이고, 그림 士4은 최대 세대 수（50）까지 진화했을 때 집단의 적합도이다. 진화를 통하1 개체
들의 적합도가 전체적으로 개선되었음을 알 수 있다．

                  25

                  20                                                             8567




                  0
                   5

             g卜    0

                   1
                   占


              -10,

              -15

              -20

              끄5                                   1

                1                         3        4          5       6    7    8        9    1
                                                                  x

                                ［그림 午5] 목적함수와 최종 해


 그림 十5는 다수의 국부 수렴 첨두치를 갖는 함수인 식（4.25）와 유전알고리즘으로 찾은 하1
를 보인 것이다. 유전알고리즘이 전역 최적 해를 찾은 것을 볼 수 있다. 그림 壬6은 집단의
평균 적합도（아래 곡선）와 최우수 개체의 적합도가 진화를 통해 어떻게 변화하는지를 보인
것이다. 진화가 진행될수록 평균 적합도가 상승함을 볼 수 있기 때문어］, 유전알고리즘이 효과
적으로 동작한다고 볼 수 있다．


              25       -   1-
                                      -                ,     /
              20




                  0                                                        1
                           5     10           15       20      25     30   35   40      45   50
                                                            generation

                       ［그림 小6] 평균 및 최우수 적합도의 변화


===== PAGE 118 =====
116        퍼지, 진화컴퓨팅 프로그래밍



      유전알고리즘의 실행할 때 초기화（initializega.m) 및 본체（ga.m) 함수의 호출어］ 사용할 입
  출력 인수들의 사용법을 정리해 보자. 아래에 보인 파라미터 수치는 예를 보인 것으로 문제어］
  따라 변경되어야 한다．


      >[startPop] = initializega(popSize,bounds,eva1FN,evalOpts,options)
      卜[bestX,endPop,bPop,tracelnfo] = ga(bounds,eva1FN,evalOpts,startPop,options,
                          termFN,termOpts,selectFN,selectOpts,xOverFNs,xOverOpts,
                          mutFNs,mutOpts)


      . 입력인수
      .최대 진화 세대 수, 예） maxGen = 100
      .집단 크기, 예） popSize = 30
      .변수의 범위，
        예） 목적변수의 범위가 - 30 드 x1 드 30, 20 드 T2 드 40, 0 드 X3 드 10이면 bounds

            = [-30 30; 20 40; 0 101
      .적합도 함수파일명（문자열）(eva1FN) , 예） eva1FN = 'testEval' - testEval.m
      ．적합도 함수에 넘겨줄 부가적인 옵션（evalOpts), 예） evalOpts = []
      .ga 함수（ga.的에서 다음 문장을 이용 적합도 함수를 호출한다．
        [ci(xZomeLength) ci] = feval(eva1FN,c1,[gen evalOpts])
      .종료조건 함수명（termFN）과 옵션（termOpts)
        예) termFN = 'maxGenTerm', termOpts = [maxGen]
            ga 함수（ga.m)에서 진화 세대 수를 종료 조건으로 사용할 때 함수（maxGenTerm.m)
            를 호출하기 위해 다음 문장이 실행된다．
            done = feval(termFN,[gen termOpts] ,bPop,endFop);

        예） termFN = 'optMaxGenTerm',
            goalFit: 목표 적합도 값
            termOpts = [maxGen goalFit epsFit]
            ga 함수（ga.m)에서 진화 세대 수와 목적함수 값을 종료 조컨으로 사용할 때 함수
            (optMaxGenTerm.m)를 호출하기 위해 다음 문장이 실행된다．
            done = feval(term고N,[gen termOpts],bPop,endPop);


===== PAGE 119 =====
                                                           4장 유전알고리즘          mim
·유전알고리즘 옵션, options = [epsFit gaType epsVar]

  epsFit: 적합도어］ 태한 허용 오차로 디폴트 값은 1.可6이다．

  gaTi농rpe: 표현 체계에 따라 실수면 1, 이진 표현이면 0의 값을 갖는다．
  epsVar: 두 수를 구분하는데 필요한 차이로, 이 값어］ 의해 각 변수에 필요한 이진 비트
          수가 결정된다．

  예） options = [ 1.可6 11];
《선택 방법어］ 대한 함수명（selectFN）과 옵션（selectOpts)
  예) selectFN = 'roulette', selectOpts = []

  예） selectFN = 'normGeomSelect', selectOpts = [pBest]
     pBest: 최우수 개체가 선택될 확률, 예） pBest = 0.08

  예） selecti그N = ' 切1寸nSelect', select야亢S = [nSize]
     nSize: 토너먼트의 크기（개체의 수）, 예） nSize = 5
     ga 함수（ga.m)에서 다음의 문장을 통해 선택 함수를 호출한다．
     endPop = feval(selectFN,startPop,[gen selectOpts]);
.교배 방법에 대한 함수명位OverFNs）과 옵션位OverOpts)
  예） 실수 표현인 경우（gaType = 1)
     xOverFNs = 'arithXover heruristiXover simpleXover'
     xOverOpts = [nXover 0; nXover nTry; nXover 0]
     nXover: 교배 연산자의 적용 횟수, nXover = 2
     n'T놔： 재시행 횟수로 n'I놔 = 3, 0은 사용되지 않는 파라미터．
     위와 같이 정의하면 3개의 교배 연산자 모두가 사용되며, 특정 연산자를 사용할 때는
     xOverFNs = 'simpleXover' , xOverOpts = [nXover 0］과 같이 정의한다．
     ga 함수（ga.m)에서 다음의 문장을 통해 교배 함수를 호출한다．
     [endPop(a,:) endPop(b,:)] = feval(deblank(xOverFNs(i,:)),endPop(a,:),
                                       endPop(b,:),bounds ,[gen xOverOpts(i,:)]);
  예） 이진 표현인 경우（gaType = 0)
     xOverFNs = 님impleXover'
     xOver야亢S = [pCross]
     pCross: 교배 확률（교배율）, 예） pCross = 0.6


===== PAGE 120 =====
1mm[    퍼지, 진화컴퓨팅 프로그래밍



   .돌연변이 방법에 대한 함수명（mutFNs）과 옵션（mutO砒s)
       예） 실수 표현인 경우（gaType = 1)
         mutE기Ns = 'unifMutation nonUni小血tati아i multiN아Un迂Mut毗ion
                     boundaryMutation'
         mutOpts = linMut 0 0; nMut maxGen pShape;
                     nMut maxGen pShape; nMut 0 0]
         nMut: 교배 연산자의 적용 횟수, nMut = 2
         pShape: 모양 결정 파라미터 , pShape = 3
         mutOpts에서 0의 값은 의미 없는（사용되지 않는） 파라미터이다．
          위와 같이 정의하면 4개의 돌연변이 연산자 모두가 사용되며 , 특정 연산자를 사용할
          때는 mutFNs = 'unif入血tation', mutOpts = [nMut 0 0］과 같이 정의한다．
          ga 함수（ga.m)에서 다음의 문장을 통해 돌연변이 함수를 호출한다．
          endPop(j,:) = feval(deblank(mutFNs(i,:)), endPop(j,:),bounds,
                             [gen mutOpts(i,:)]);
       예） 이진 표현인 경우（gaType = 0)
          mutateFN = 'binaryMutation'
          mutateOpts = [pMut]
          pMut: 돌연변이 확률（돌연변이율）, 예） pMut = 0.01


   a출력인수
   ，최종 해（가장 우수한 개체）:bestX
       예） bestX(1:n): n개의 변수, bestX(n+1): 최우수 개체의 적합도
   ．마지막 집단어］ 대한 정보： endPop
       예） endi七p(1:popSize,1:n): popSize개의 개체, 개체는 n개의 변수를 가짐
       예） endPop(1:p아）Size,n+1): popSize개의 개체 적합도
   .최우수 개체의 변화를 기록： bPop
       예） bPop(:,1): 최우수 개체의 적합도가 향상된 세대 수
       예） bPop(:,2:n+1): 최우수 개체에 개선이 있을 때 그 개체의 정보를 저장
       예） bPop(:,n+2): 개선된 최우수 개체의 적합도 저장
   .서］대 증가어］ 따라 아래와 같은 정보를 저장： tracelnfo


===== PAGE 121 =====
                                                        4장 유전알고리즘   119


  예） 缸acelnfo(:,1): 세대 수 정보 저장

  예） tracelnfo(:,2): 최우수 적합도 저장

  예） tracel沚o(:,3): 집단의 적합도 평균 저장

  예） tracelnfo(:,4): 집단의 적합도 표준편차 저장



 3장의 식（3.5）의 해를 구하는 문제를 이진형 유전알고리즘과 실수형 유전알고리즘으로 처
리하는 코드가 리스트 午17과 全18이다．



 姦 리스트 小］7 小 이진 유전알고라즘에 의한 Rosenbrock 함수 최적화

 % 파일명： rosenBii俎ryGa.m
 % 이진형 유전알고리즘으로 Rosenbrock 함수의 최적해 찾기
 clear;
 dlc;
 rand('seed',0); % 비교 실험을 위해 랜덤 수 발생기를 초기 상태로 리셋


 % 파라미터 설정
 maxGen = 300; % 최대 진화 세대 수
 popSize = 30; % 집단 크기（>=20)
 epsFit = 1.e-6; % 두 적합도 값의 차를 구분할 수 있는 크71
 gaType = 0; % 이진 표현이면 0
 epsVar = 1; % 수를 구분하는뎨 필요한 크기로， 각 변수어］ 필요한 이진 비트 수를 결정．
 options = [epsFit gaType epsVar]; % 유전알고리즘 옵션
 t兀unds = ［그048 2.048; 그048 2.048]; % 변수의 범위
 evalFN = 'rosenEval'; % 적합도 함수명
 evalOpts = [1;


 % 종료： 아래1 (1）과 (2）중 선택, 현재1 (1)을 사용
 ten小N = 'maxGenTerm'; % (1)
 termOpts = [maxGen]; % (1)
 %termFN = 'opt入4axGenTerm'; % (2) 종료조건 함수명
 %goalFit = 4000; % (2) 적합도함수 목표 欲최대화 문제로 변형할 때 상수 이용）
 %termOpts = [maxGen goalFit epsFit]; % (2) 종료조건 파라미터


 % 선택： 아라1 (1), (2), (3）중 선택， 현재 (1）을 사용
 selec坦N = 'roulette'; % (1) 선택 방법어］ 대한 함수명


===== PAGE 122 =====
120   [          퍼지, 진화컴퓨팅 프로그래밍



      selectOpts = [1; % (1) 선택 방법의 파라미터
      %selectFN = 'normGeomSelect'; % (2)
      %pBest = 0.01; % (2) 최우수 개체가 선택될 확률
      %selectOpts = [pBest]; % (2)
      %selectFN = 'toumSelect'; % (3)
      %nSize = 2; % 토너먼트 크기 %(3)
      %s이凹山倂S = [nSize]; % (3)


      %교배
      xOverFNs = 'simpleXover'; % 교배 함수명
      pCross = 0.3; % 교배율
      xOverOpts = [pCross]; % 교배 관련 파라미터


      % 돌연변이
      mu作Ns = 'binaryMutation'; % 돌연변이 함수명
      pMut = 0.01; % 돌연변이율
      mutOpts = [pMut]; % 돌연변이 관련 파라미터


      % 집단 생성 및 초기화
      [startPop] = initializega(popSize,bounds,evaIFN,evalOpts,options);


      % 유전알고리즘 본체 실행
      [bestX,endPop,bPop,tracelnfo] = ga(bounds,evalFN,evalOpts,startPop,options,termFN,termOpts,...
                                                   selectFN,selectOpts,xOverF나s,xOverOpts,mutFNs,mutOpts);


      bestX % 최적해


      % 최종 집단의 개체별 적합도
      plotRosen;
      hold on;
      plot (bestX(1工bestX(2),'ro') % 최적 해의 표시
      pause;
      hold off;
          clf;
      % 세대 별 최우수 적합도의 변화
      plot(tracelnfo(:, 1),tracelnfo(:,2),'b-');
          axis ([1 maxGen goalFit-50 goalFit]); % 그림의 축 범위 설정


===== PAGE 123 =====
                                                                            4장 유전알고리즘   口國.

xlabel('generation');
ylabel('fitness: f(x)');
hold on;
% 서］다1 별 평균 적합도의 변화
plot(tracelnfo(:, 1),tracelnfo(:,3),'k-');


            function [so!, fit] = rosenEval(so!,options);
            % 파일명： rosenEva!.m
            % 목적함수로 차분 진화에서는 적합도 함수로 그대로 사용
            % 사용법 [so!, fit] = rosenEval(sol,options上
            %           입력변수
            %                 so!: 목적변수， 이 문제에서 so! = [so!(!) so!(2)]
            %                 options: 문제 콴련 파라미터 벡터
            %                 fit: 적합도 함수 값


           % Rosenbrock 의 목적함수
            obj = 100求（so!(2) - so!(1）八2）八2 + (1 - S아(1沙2;
           % 최소화 문제의 목적함수를 최대화 문제의 적합도함수로 변환
           const = 4000; % 최때1 문제로 변경하기 위한 상수（임의의 값을 사용）
           fit = const - obj;
           % 최대화 문제에서 叱j가 0이 되는 경우가 없다면 fit = 1允可를 사용．




           % 파일명： plotRosen.m
           % Rosenbrock 함수 그리기


           xl = -2.048:0.075:2.048;
           x2 = x!;
           sz = size(xl,2);
           z=zeros(sz,sz);
           const = 4000;
           gen = 0; % 세때1 수
           for i = 1: sz
                 for j = 1: sz
                      [sol, fit] = rosenEva!([x 1(i) x2(j)],[gen const]);
                      z(ij) = const - 血； % 본래 목적함수 값으로 환원


===== PAGE 124 =====
         퍼지, 진화컴퓨팅 프로그래밍



                  end
            end
            mesh(xi,x2,z); % 3차원 그림
            axis([-2.5 2.5 -2.5 2.5 0 4000]);
            view(40,60);
            grid on;
            xlabel('x 1');
            ylabel('x2');
             zlabel('F(x 1,x2)');




mm 리스트卜18 小 실수형 유전알고리즘에 의한 Rosenbrock 함수 최적화 無

  % 파일명： rosenFloatGa.m
  % 실수형 유전알고리즘으로 Rosenbrock 함수 최적해1 찾기
  clear;
  dlc;
  rand('seed',0); % 비교 실험을 위해 랜덤 수 발생기를 초기 상태로 리셋


  % 파라미터 설정
  maxGen = 300; % 최대 진화 세대 수
  popSize = 30; % 집단 크기（>=20)
  epsFit = i.e丘 % 두 적합도 값의 차를 구분할 수 있는 크기
  gaType = 1; % 실수 표현이면 l
  epsVar = 1; % 각 변수어］ 필요한 이진 비트 수를 결정．
  options = [epsFit gaType epsVar]; % 유전알고리즘 옵션
  bounds = ［그048 2.048; 그048 2.048]; % 변수의 범위
  eva作N = 'rosenEval'; % 적합도 함수명
  evalOpts = [1;


  % 종료： 아라1 (1）과 (2）중 선택， 현재 (2）가 사용．
  %termFN = 'maxGenlerm'; % (1)
  %termOpts = [maxGen]; % (1)
  termFN = 'O少MaxGenTerm'; % (2) 종료조건 함수명
  goaiFit = 4000; % (2) 적합도 함수 목표 값
  termOpts = [maxGen goaiFit epsFit]; % (2) 종료조건 파라미터


===== PAGE 125 =====
                                                                     4장 유전알고리즘


 % 선택： 아래 (1), (2), (3）중 선택， 현재 (3）이 사용．
 %selectFN = 'roulette';'% (1) 선택 방법에 대한 함수명
%seleetOpts = [1; % (1) 선택 방법의 파라미터
 %selectFN = 'normGeomSelect'; % (2)
%pBest = 0.01; % (2) 최우수 개체가 선택될 확률
%selectOpts = [pBest]; % (2)
selectFN = 'tournSelect'; % (3)
nSize = 2; % 토너먼트 크기 % (3)
selectOpts = [nSize]; % (3)


% 교배
xOverFNs = 'arithXover heuristicXover simpleXover'; % 교U1) 함수명
ftXOver = 1; % 교배 연산자의 적용 횟수
nTry = 3; % 재시행 횟수
xO妃rOpts = [nXover 0; nXover nTry; nXover 0]; % 교배 관련 파라미터


% 돌연변이
% 돌연변이 함수명
mutFNs = 'boundaryMutation multiNonUnifMutation nonUnifMutation unilMutation';
n入4ut = 1; % 교배 연산자의 적용 횟수
pShape = 3; % 모양 결정 파라미터
% 돌연변이 콴련 파라미터
mutOpts = [nMut 0 0; 刊Mut maxGen pShape; nMut maxGen pShape; nMut 0 0];


% 집단 생성 및 초기화
[startPop] = initializega(popSize,bounds,eva1FN,evalOpts,options);


% 유전알고리즘 본체 실행
[bestX,endPop,bPop,tracelnfo] = ga(bounds,eva1FN,evalOpts,startPop,options,termFN,termOpts,...
                                    selectFN,selectOpts,xOverF寸s,xOverOpts,mutF寸s,mutOpts);


bestX % 최적해


% 최종 집단의 개체별 적합도
히ot如sen;
hold on;
plot (bestX(1),bestX(2),'ro') % 최적 해의 표시


===== PAGE 126 =====
         퍼지, 진화컴퓨팅 프로그래밍



  pause;
  hold off
  cif,
  % 세대 별 최우수 적합도의 변화
  plot(tracelnfo(:,1),tracelnfo(:,2),'b-');
  axis ([ I maxGen goalFit-50 goalFit]); % 그림의 축 범위 설정
  xlabel('generation');
  ylabel('fitness: f(x)');
  hold on;
  % 세대 별 평균 적합도의 변화
  plot(tracelnfo(:, l),tracelnfo(:,3),'k-');




 그림 午7에서 午9까지가 실행 결과인데, 그림 壬7은 목적함수 평면 위에 유전알고리즘으
로 찾은 해를 표시한 것이고, 그림 午8과 午9는 이진형 및 실수형 유전알고리즘에서 진화를
거치면서 최우수 개체의 적합도와 집단의 평균 적합도의 변화를 보인 것이다. 이진형 유전알
고리즘에서는 선택 방법으로 'roulette'을, 실수형에서는 'tournSelect'을 채택하였다. 이 두
그림에서 최우수 개체의 적합도에는 별 차이가 없지만, 평균 적합도 측면에서는 실수형이 좋
아 보인다. 물론, 결과는 관련 파라미터를 어떻게 선택하느냐에 따라 달라질 수 있다．




                        4000



                   小N乂r즈且
                                0
                                0
                            n   0                                          牙文；泌：
                                                                          弩立恣；};．三
                            /
                                                                           ；스斗J5月




                                o   \,
                                                                             毛囊轟蠶焄芦
                                                                                         囊藝驀藿簧莽針 /q
                                              \:\\\

                                         -2
                                                      \\\           /\\
                                                            '   "          \,:\,,
                                                                                               '- '    0


                                                                                                      x2
                                                                                    xl

                                                        ［그림 小7] Rosenbrock 함수와 최적 히1


===== PAGE 127 =====
                                                                         4장유전알고리즘
                                                                                          m

                    r
             4000




             3990

                             4                    川
                        I
            39나
          ;3980-

          瓦，놔

                                 1
                        I
                                                        4,
                            50       100      150            200   250
                                           gene rat伯n


       ［그림 午8] 이진 유전알고리즘에서 최우수 적합도와 평균 적합도의 변화



            4000W

            3995

            3990

            3985

           -3980

          冒 3975
          山
          =
          는 3970

           3965

           3960

           3955

           3950
                        50       100          150       200        250              300
                                           generation


      ［그림 午9] 실수형 유전알고리즘에서 최우수 적합도와 평균 적합도의 변화




                                       연습문저1


[11 Rosenbrock 함수에 대해 아래 기술된 것처럼 유전알고리즘의 파라미터를 변경하면서
  최적화 결과를 확인한다. 이진형과 실수형 유전알고리즘 모두를 실행해 본다．


===== PAGE 128 =====
126       퍼지, 진화컴퓨팅 프로그래밍



         집단 크기： 30, 50, 100

         최대 세대 수： 500
         선택: 'roulette', 'normGeomSelect', 'tournSelect'
         교배： 이진형은 교배율의 변경

               실수형은 연산자를 모두 사용하는 것과 하나씩 사용하는 것
               'arithXover', 'heruristiXover', 'simpleXover'
         돌연변이： 이진형인 경우는 돌연변이율의 변경
               실수형은 연산자를 모두 사용하는 것과 하나씩 사용하는 것
               'unifMutation', 'nonUnifMutation'
               'multiNonUnifMutation', 'boundaryMutation'

      [2] 3장 연습문제 2번의 해를 유전알고리즘으로 찾아라．




                                      斗 심화 학습 자료 小


      [1] 황희수, 컴퓨터에 의한 진화계산 및 진화디자인, 내하출판사, 2002.
      [2] C. R. Houck, J. A. Joines, and M. G. Kay, "A genetic algorit노ll for function
         optimization:   A   matlab   implementation,"    NCSU-IE     Tecimical    Report

         95-09(http:II자ww.ie.ncsu. edu/mirage/GAToolBox/gaot/).
      [3] D. E. Goldberg, Genetic? 月／甘（끄亢加끄S 끄2 Search, Op勾）riiza苡2fl a끄d 兀台C／끄he
         Lear끄hg, Addison-Wesley, MA, 1989.
      [4] J. H. Holland, Adaptation in natural and artificial systems, The University of
         Michigan Press, 凡m Arbor, 1975.
      [5] J. H. Grefenstette and J. E. Baker, "How genetic algorithms work: A critical
         look at implicit parallelism," Proc. of the 3rd i1lt. conf. on genetic algorithms
         and their applications, pp. 20-27, Morgan Kaufmann Publishers, 1989.
      [6] Z. Michalewicz, "Genetic algorithms + Data structures = Evolution programs,"
         Springer-Verlag, New York, 1994.


===== PAGE 129 =====
CHAPTER 5   퍼지 규칙의 생성



             永 5. ] 퍼지 모델
             睿 5.2 퍼지 모델 인식
             密 5.3 퍼지 모델의 구축 및 평가


===== PAGE 130 =====
                                                    5장. 퍼지 규칙의 생성           129




 66 시스템의 특성과 거동을 표현한 것을흔히 모델이라부른다. 모델링이란 시스템의 특성과 거동
    을 잘 묘사하기 위해 시스템을 특성화하는 입력과 출력 변수를 정의하고, 이 입출력 변수들 사이의
    관계를 찾아내는 것이다. 이는 마치 아래 그림에서 블랙박스 안을 채우는 것과 같다. 블랙박스 안
    을 선형이나 비선형 방정식, 전문가시스템, 신경회로망 또는 퍼지 규칙 등으로 채울 수 있다．
      입출력 관계가 이벤트 예측을 기술하고 있으면 이 모델은 예측 시스템으로, 패턴 분류를 기술하
    고 있으면 패턴 분류기로, 제어 동작을 기술하고 있으면 제어기로, 의사결정을 기술하고 있으면
    의사결정 시스템으로, 물체의 운동을 기술하고 있으면 거동 모델 등으로 사용될 수 있다. 즉, 용도
    는 기술하려고 하는 입출력 사이의 관계에 의해1 결정되며 ，모델 형식은 그 관계를 기술하는 방법으
    로 수식, 신경회로망 또는 퍼지 규칙 등이 될 수 있다. 입출력 사이의 관계를 기술하는 퍼지 규칙
    （모델）을 생성하는 것을 흔히 퍼지 모델링이라 부른다．



                                    Black Box
                                        9




      시스템이 복잡하거나 정의하기 어렵거나 불확실해서 기존의 수학적 방법으로는 만족스런 결과
    를 얻기 힘든 경우에 퍼지 모델은 유용하게 사용될 수 있다 ．퍼지 모델은 크게 두 가지 유형 즉，
    퍼지 관계식（fuzzy relational equations）과 퍼지 규칙（fuzzy rules）이 있는데, 후자가 일반적이
    며 널리 사용되기 때문어T 본 책에서는 후자에 국한해서 퍼지 모델을 구성하는 퍼지 규칙을 자동으
    로 생성하는 절차와 과정을 소개한다. 이 장에서는 퍼지 규칙 생성（퍼지 모델링）을 위해 앞의 h4
    장 내용' ] 어떻게 결합돼";
                            陪되는' ］를 설벼"한다· 99




 Fuzzy & 드V이Ut油na口
    Computing Programming   5. ] 퍼지 모델


 퍼지 모델의 형식으로 식（5.1）과 같은 八41SO(Multiple Input Single Output）의 퍼지 규칙
으로 고려한다. MIMO(Mult螂e Input Multiple Output) 시스템의 경우에는 출력 수만큼의
MISO 모델을 이용할 수 있다．


===== PAGE 131 =====
130   [    퍼지, 진화컴퓨팅 프로그래밍



          R " : If x1isAi (x1) and ··· xkisAi(xk) thenyisH.                                              (5.1)


      /?"는 可 번째 규칙（1 드 可 드 r) , 幻(1 드 3 三 丸）는 입력변수，y는 출력변수， A} (幻）는 입

  력 멤버쉽함수로 식（5.2）와 같이 정의된다. 尸는 출력 퍼지변수로 일반적인 멤버쉽함수나 선
  형식을 사용할 수 있지만 여기서는 퍼지 싱글톤（실수） 값을 사용하기로 한다. 출력 퍼지 변수
  어］ 퍼지 싱글톤을 채용한 이유는 모델의 정확도어］ 손상을 거의 주지 않으면서 계산랑을 줄일
  수 있어 실용적이기 때문이다．


               1
               I   0         ifx. < (ct- dc已- d1二)_   .J   .   '   J :         J:   .   .1   '   .   .




               1 他＋叱＋叱- c)似二 if (c- dc- d1;）드xi드（c7- dc刃
                      3 （弓＋de)
          A＝任自＋叱＋叱＋c)府if     ．드x戶（弓十叱十．毗）                                                                (5.2)
               I             1                   if (c- dc) <x < (c+ dc)
               I             0                     0琉erwise


      위 식은 아래 그림 5-1과 같은 사다리꼴 멤버쉽함수이며，弓는 멤버쉽함수의 중심，叱가

  0 이면 삼각형 멤버쉽함수가 된다．




                                                       :i+ i               .        ;
                                          dli;        c1                 dr:

                                          ［그림 5-1] 멤버쉽함수



  식（5.1）을 벡터 형식으로 표시하면 식（5.3）과 같다．


          /Z ' :If Xis A' (X), yis B' .                                                                  (5.3)


  위 식에서 X= (xi, x2, ···, Xk）이고 A"= (A, A, ···,Ai）이다．

      식（5.2）와 같은 규칙이 r7fl 있을 때, 坦1째 입출력 데이터 （毗毗 ···，姝可）,
  (1 드 / 드 n）에 대한 피지 규칙의 추론 값은 다음과 갇은 단계를 거쳐 계산된다．


===== PAGE 132 =====
                                                                             5장. 퍼지 규칙의 생성



 (l:) 규칙에 대한 만족도 계산


     까        A            X   A     佃
                                     i
                                               X   X   A
                                                       12 七
                                                              ik
                                                              佃
                               2 n
                               1 乙
                       (x) xA (x1) x ...xA.(x'A.)
                               =
                                     n
                                     乙
                                                                                             (5.4)


乂는 곱하기나 최소값 계산 연산자를 의미하는데, 후건부가 선형식이나 싱글톤인 경우에는
주로 곱하기로 사용한다．


 區） 만족도의 정규화
                   凹
     切                                                              =
                   r
                                                                                             (5.5)

                   몸
 區） 후건부의 계산
   후건부가 선형식인 경우

    yi = a, + 可 · 可 + ．·· + 아， · 따，                                                          (5.6)

   후건부가 싱글톤인 경우 특별한 계산이 필요치 않음
   !/,   =   尸                                                                               (5.7)


 （孕 최종 출력의 계산

    yl = ＞二Wi X 夕
             / =       l
                                                                                             (5.8)




Fuzzy & Ev이Ut幻nary
   Computing Programming                 [5.       2 퍼지        모날       인식

 n개의 데이터 집합 x= ｛毗毗 ··U먀，們1 드 l 드n｝이 주어지면 퍼지 모델링 문제는
식（5.9）의 오차를 최소로 하는 퍼지 모델（퍼지 규칙들）을 인식하는 것이고 이를 위해 다음과
같이 두 단계를 거친다．


===== PAGE 133 =====
口m1 퍼지, 진화컴퓨팅 프로그래밍
   (] ) 구조 인식
   .피지 모델을 구성하는 규칙의 수
   4퍼지 규칙에 사용된 입출력 퍼지 변수의 공간 분할（멤버쉽함수의 형태）


   (2) 파라미터 인식
   .제한조컨을 가지며 식（5.9）를 최소로 만드는 최적화 문제를 구성
   .최적화 문제의 해결


    구조인식과 파라미터 인식이 서로 관련이 있기 때문에 원리적으로는 이 둘을 분리할 수 없
   지만 분리 수행할 수 있다면 계산상의 이점이 있다. 이 둘을 분리하지 않고 구조와 파라미터
   를 동시어］ 인식할 수도 있지만［참고문헌 3, 4] 여기서는 분리해서 퍼지 모델을 인식하는 방법
   을 소개한다［참고문헌 1, 2] . 물론, 구조（필요한 퍼지 규칙의 수, 사용할 입출력 변수 등）가
   알려진 경우에는 그 구조에 대해서 파라미터 인식만 수행해도 된다. 여기서는 앞에서 학습한
   내용(1- 4장） 모두를 종합적으로 활용한다는 차원에서 구조 인식과 파라미터 인식 모두를 다
   루기도 한다.


      万＝ 71寸，回可' )"                                       (5.9)
          [ /=1


   n은 모델링에 사용된 데이터 수, !/／은 실제 출력 뎨이터이고 !1' 는 피지 모델에서 추론된 출력
   값이다．


   5.2.1 구조 인식
    퍼지 규칙을 인식할 때 우선적으로 전건부어］ 주목하고 어떤 기준에 의해 최적의 퍼지 분할
   공간을 찾을 수도 있지만, 여기서는 전컨부와 후건부를 통시에 퍼지 분할하는 방법을 알아보
   자. 이를 위하1 2장에서 설명한 퍼지（只弧4) 클러스터링을 사용한다. 즉, 입출력 데이터
   x= ｛毗毗, ···, 毗, y111 드 1 드 n｝어］ 대해 퍼지 클러스터링을 수행해서 필요한 수의 퍼지

   클러스터를 찾아낸다. 하나의 피지 클러스터가 하나의 퍼지 규칙으로 매핑되기 때문어］ 피지
   클러스터의 수가 피지 규칙의 수가 된다.
    예로, 입력 변수가 둘인 데이터 집합 X= {x , 毗, !／口 드 / 드 n｝가 주어졌다고 하자. 입

   출력을 합쳐 크기 3Xn의 데이터에 대해 퍼지 클러스터링을 수행한 결과 클러스터 수가 2일


===== PAGE 134 =====
                                                                  5장. 퍼지 규칙의 생성     口m
때 식（2.8）의 클러스터링 평가척도가 최적（최소）이라 하자. 일부 클러스터 수에 있어 평가척
도 값어］ 차이가 별로 없는 경우에는 적은 수의 클러스터를 최적 분할로 보아도 된다. 그림
5-2는 이렇게 얻은 두 개의 클러스터를 입출력 공간으로 매핑한 것이다. 매핑에 있어 각 멤
버쉽함수의 중심은 해당 클러스터의 중심점 c1, c2（식（2.6）으로 계산）어］ 대응하며, 멤버쉽함

수는 퍼지 분할 행렬（식（27）으로 계산） 값어］ 의해 만들어진다. 클러스터의 중심점과 퍼지 분
할 행렬은 퍼지 클러스터링어］ 의해 얻어진 결과이다. 그림 5-2어］ 보인 퍼지 분할（멤버쉽함
수）을 그림 5-3과 같이 원하는 형태의 멤버쉽함수로 근사화시킬 수 있다.

                            ot毗0虎 斗：ace


                                               Centroid 町 cit工ster : C2
                                                        .




                                  autroid of duster: q :
                                           .



                                                                          卜
                                               A   '      ;      ill工砒如恥比
                                               i In町恥ng
                                x2




                                           A{             川
                           ［그림卜2] 퍼지 클러스터의 매핑



  ／간 : // x1 is 비 他 ) and x2 is 川 似 ), !/ is B'
                                                                                  (5.10)
   冗2 : // x] 可S 川回 ) and x2 is 川回）, !/ isB2


===== PAGE 135 =====
口m   퍼지, 진화컴퓨팅 프로그래밍



  이 책에서는 입력 멤버쉽함수는 사디리꼴, 출력은 싱글톤의 형태를 택했지만 삼각형이나
 종형의 멤버쉽함수를 선택해도 된다. 다음 단계는 그림 千3어］ 보인 멤버쉽함수들의 정확한
 모앙을 결정하기 위해 파라미터 인식 단계를 거친다. 독자들은 구조 인식에서 그림 5-2어］
 보인 것과 같이 퍼지 분할 행렬을 이용하여 퍼지 분할 형태를 알아낼 필요가 없다. 퍼지 클러
 스터링은 클러스터 중심과 데이터 사이의 거리어］ 기초하기 때문어］ 그림 5-2어］ 보인 것과 같
 은 퍼지 분할 형태를 가질 수밖어］ 없다. 따라서 그림 5-2의 과정을 거치지 않고 클러스터
 중심만을 이용해서 그림 5-3과 같은 구조로 매핑할 수 있다. 결과적으로 그림 5-3에서 식
 (5.10）에 보인 두 개의 퍼지 규칙을 유도할 수 있다．


                   y        out工a虎 斗ace
                   스

                                                auster C2: V2 = (vi, vg, v뭉)
             B2        V릎
             g         4         a哨ter (:; : V1 = （며.. t           二)


                                            A'                A2
                                                                        input space

                                           a好,roxirni流아1




                                            }            A쿠
                  ［그림 千3] 매핑된 퍼지 클러스터의 근사화


===== PAGE 136 =====
                                                                                  5장. 퍼지 규칙의 생성               口m
 구조 인식에서는 데이터 사이의 거리어］ 기초해서 입출력 데이터가 갖고 있는 고유의 구조
를 파악하고 클러스터들의 매핑 및 근사화를 통해 퍼지 규칙의 골격을 찾아낼 수 있다. 퍼지
클러스터링이 이를 가능하게 해주며 , 이 과정에서 퍼지 규칙의 전건부 및 후건부어］ 있는 파라
미터에는 관심을 둘 필요가 없다. 이는 결과적으로 구조 인식과 파라미터 인식을 분리해서
수행할 수 있도록 해준다．
구조 인식 과정을 정리하면 다음과 같다．

［단계1] 퍼지 클러스터의 최소 수（통상 2）를 정한다．
［단계2] 입출력 데이터에 대해 퍼지 클러스터링을 수행한다．
［단계3] 퍼지 클러스터링 평가척도를 계산한다．
［단계4] 클러스터 수를 하나 증가시키고 단계2로 복뀌. 최대 클러스터 수（통상 10）어］ 도달
     할 때까지 이 과정을 반복한다．
［단계5] 평가척도가 가장 낮은 클러스터 수를 찾고 이 때의 클러스터 중심 벡터를 얻는다．
     예로, 丸 입력 변수와 하나의 출력으로 구성된 依＋1) 차원의 데이터어］ 대해 nc7fl
     의 클러스터가 최적이라 하면 식（5.11）과 같은 중심 벡터가 얻어진다．


      V= { 1月, v2, ··．, V "} , 1戶 = （며，崎 ··．，可：, vi1)U
                                                                         1
                                                             1
                                                                                                          (5.11)
                                                                     7
                                                                                                      \
                                                         2
                                                                                                  J
                                                     加
                                                                                              /
                                                                 %
［단계6] 매핑을 통해 클러스터 중심 벡터에서 퍼지 규칙을 찾아낸다. 식（5.11）의 중심점을
     각 축으로 매핑하고 이를 크기 순으로 정렬하면 식（5.12）와 (5.13）으로 표현할 수
     있다．

                                        伊   m7
     vx = { 1戶i, T/ '2, ···， 少나，                 2
                                            丁
                                                                             ，畔
                                                                                  ‘ " "   )               (5.12)   1

                                                                                                                   나




    丁miJ " 과 畔"' 는 幻 축에서 정의된 최소와 최대값이고 心는 식（5.11）의 중심점 가운
    데 하나이다．


     ［月／= (! mm", !/i , ．··, !/ne, m씨                                                                     (5.13)


    !/"""" 과 !njm缸는 !/ 축에서 정의된 최소와 최대값이고 !/' 는 식（5.11）의 중심점 가운뎨
    하나이다．


===== PAGE 137 =====
=m      퍼지, 진화컴퓨팅 프로그래밍




 5.2.2 파라미터 인식

     구조 인식을 통하1 퍼지 규칙을 만들었지만 궁극적인 퍼지 모델은 식（5.9）로 정의퇸 실제 출
 력과 모델 출력 사이의 오차를 최소로 하는 것이어야 한다. 따라서 오차를 최소로 하는 전건
 부와 후컨부의 멤버쉽함수 파라미터를 찾는 것이 파라미터 인식의 목표이다．
     구조 인식의 결과로부터 파라미터 인식을 위한 문제를 정리해보자. 식（5.12）에서 畔는 전건

 부 멤버쉽함수의 중심인 식（5.2）의 弓에 해당한다 ．畔는 크기 순으로 정렬된 값이므로 퍼지

 규칙에서 사용한 인덱스 可 와는 다를 수 있다. 식（5.14）와 같이 제한조건을 두어 弓의 탐색범

 위를 좁힐 수 있다．


                    mj               4
                                     J       윽 그
       可 '" 드 c 드   T                                                           =

               Z 可
                                                          1
          1
          <口
                                                          凡
        d        드             +           2                          O乙   QU
                                                                                    C=
                                                                                     =

                                                                                                (5.14)
                                                                                            1
                                                                                    /=
                                                                                    n

       1
       2
       따 C野
                                                              ＝
                 d
                 J                         l r 7
                                                                                        n
                                                                                        H

                                                              丸
                 드Cn<
                                           1
                                                                  k                 <
                                                                                        1
                    1                                                               1
     이 때 寸'" 과 哮瞰의 값을 학습용 데이터에서 결정할 경우， 최소값은 데이터의 최소 보다
 더 작게, 최대값은 더 크거］ 여유를 줄 수 있다. 식（5.2）에서 다른 파라미터도 식（5J5）와 같이
 제한조건을 줄 수 있다．


       0 드dc 드 畔‘缸寸'" i= 1, 2, ···,ncj= 1, 2, · " ,k
                               TIC


       0 됴 dr
       O   dH             m町              Z jmm       可 = 1, 2, "·,ncj= 1, 2夕 ···夕 丸            (5.15)
                               TIC
                드                    -
                    xn炚
       0드d1드                                      "   i= 1, 2, ···,ncj= 1, 2, ···,k
                               ITH       C "』




     식（5.13）에서 !／는 퍼지 규칙의 후건부 싱글톤 尸 에 대응한다고 하면 ，식(5.16）과 같은 제

 한조컨을 두어서 H의 탐색 범위를 제한할 수 있다. 이 때의 i는 퍼지 규칙에서 사용한 인덱
 스 i와는 다르다（크기 순으로 정렬한 것임을 기억）.


===== PAGE 138 =====
                                          5장. 퍼지 규칙의 생성



    ymlfl < B'
    y" ' 드 B 드 y"+l i = 2, 3, ···, c- i                   (5.16)

    yC_ l < 月“ < ym"X


 식（5.14）에서 (5.16）까지의 제한범위를 두지 않아도 무방하지만 구조 인식의 결과물을 최대
한 활용해서 해의 탐색 범위를 줄이면 파라미터 인식어］ 걸리는 시간을 줄일 수 있다. 물론，
탐색 범위의 축소가 해를 국부적인 것으로 만들 위험도 있다. 최종 해가 만족스럽지 않다면
탐색 범위를 확장하囚 파라미터 인식을 수행한다．
 이제 파라미터 인식을 위해 해결해야 할 문제가 정립되었다. 이는 식（5.14), (5.15）와
(5.16）의 제한조컨을 만족시키면서 목적함수인 식（5.9）를 최소화하는 최적의 해（mc X k개의

c; , dc;, 叫와 叱를 mc개의 尸）를 찾는 것이다. 찾아야 할 파라미터의 총 수는
(4 X nc>< 丸 + nc）이다．

 이제 이 문제를 푸는 방법을 생각해보자. 최적화 문제를 해결하기 위한 방법들이 다수 있지
만, 여기서는 이 책의 3, 4장에서 설명한 진화알고리즘을 사용하는 방법을 설명한다. 이는
진화알고리즘이 다양한 문제어］ 적용하기 쉬우며, 퍼지 모델링에서 파라미터 인식만이 아니라
구조 인식과 파라미터 인식을 동시어］ 수행하는 경우에도 진화알고리즘이 유용하기 때문이다．
위에서 정립한 문제는 목적함수를 최소화하는 것인데, 이것이 차분진화에서는 문제가 되지
않지만, 유전알고리즘은 적합도가 최대가 되도록 작동하기 때문에 본래의 최소화 문제를 최
대화 문제로 변환해야 한다. 이를 위해 목적함수를 적합도 함수로 변환하는 식（5.17）이 사용
된다．


           1
    /；기
                                                          (5.17)
          I了


 E는 식（5.8）의 오차이며, 실제 데이터에서 오차가 0이 되는 경우는 없으므로 식（5.17）을
이용해 최소화 목적함수 月를 최대화 적합도 함수 F로 변환할 수 있다. 고려해야 할 또 다른
사항으로 모든 규칙어］ 대해 특정 뎨이터의 전건부 만족도（식（5.4)）가 0인 경우이다. 이는 해
당 데이터가 어떤 퍼지 규칙도 만족시키지 못함（퍼지 규칙어］ 속하지 않음）을 의미하는 것으로
이런 데이터가 존재해서는 안 된다. 따라서 이런 경우가 발생하면 벌칙을 가하1 진화 과정에서
이런 모델이 도태되도록 유도해야 한다. 이를 위해 식（5.18）과 같은 벌칙함수를 적합도 함수


===== PAGE 139 =====
口m         퍼지, 진화컴퓨팅 프로그래밍



 어］ 도입한다．



                                                                  (5.18)



      n는 1 번째 데이터어］ 대해 퍼지 모델의 전건부 적합도（wi i= 1, 2夕 ' " j r）가 0이면 가할 벌

 칙의 크기로 상수 값을 가지면, 적합도가 0이 아니면 I가 = 0이다. 식（5.18）을 식（5.17）에 포

 함시켜 식（5.19）를 만들면, 유전알고리즘에서 이 식이 적합도 함수로 사용된다. 戶를 최대로
 하는 것은 오차 月를 최소화 하고 벌칙을 통해 해（퍼지 모델）를 실행 가능한 것으로 만들어준

 다．
                                                                  (5.19)




      Fuzzy & Evolutionary
         Corn口uting Pro아amming   5.3 퍼지 모델의 구축 및 평가


 5.3.1 모델의 구축
      Box & Jet政in어］ 의하1 주어진 가스 용쾅로 데이터를 이용하여 가스 용광로 퍼지 모델을
 구축해 보자. 사용된 데이터는 佃（劤, U（川, 丸＝ 1, 2, ···,296｝의 296개인데, 이를 입력
 U（丸叫4）와 y（丸- 1) , 출력 y（丸）의 쌍으로 292개의 데이터를 만든다. 변수 U（丸）는 가스
 흐름 율 을 , 변수 y （丸）는 Co2 농도를 나타낸다. 292개의 데이터를 반으로 나누어 처음 반은

 모델 구축어］ 사용하고, 나머지 반은 구축된 모델의 평가어］ 사용하기 위해 다음과 같이 두 7fl
 의 데이터 집합을 만든다.


      학습용： Xtrain =｛兀，兀， ···，石b兀 = U（可 -4) , !/(i - 1), y (i)}

      평가용： 兀；t = 位佃，石54, ···，石H兀 = 2工(i -4) , y (i - 1), y (i)}


===== PAGE 140 =====
                                                                                 5장. 퍼지 규칙의 생성   139


 xtr口in 데이터를 퍼지 클러스터링하고 평가 척도를 이용, 클러스터의 수를 결정한다. 이 과

정에 대한 매트랩 코드가 리스트 5-1이다. 그림 5-4의 결과를 보면 퍼지 지수 m이 1.25와
2인 경우 모두 2개의 클러스터가 최적의 분할임을 보이고 있다. 퍼지 클러스터링을 반복해서
실행해 보면 결과어］ 있어 약간의 차이가 발생하는데, 이는 초기값 설정이 결과어］ 영향을 미치
기 때문이다. 따라서 평가척도 값어］ 큰 차이가 없으면 최종 분할 수를 작은 값으로 선택한다．
분할 수가 적어도 파라미터 인식을 통해 만들어진 분할 수 만큼의 퍼지 규칙은 필요한 입출력
관계를 충분히 기술할 수 있다．


                     9
                     0
                                                 n口 of optin倒 part伯n = 2




             8     6  5   4   3
                                                    m = 1.25




             0 r0  0  0   0   0 n0
                1


              꿎mm쁜금8E＞ 之乙言＞ 능山三m>{

                   ]
                   0



                                     2   3      4      5       6        7            10
                                                 No. of fuzzy partition

                                         (a) 퍼지 지수 刃2= 1.25

                       1
                   8
                   0
                                                no. of optimal partion = 2




            8  7
                              1




                  6 石 4
                                                    m =2



                           3   2
                              1




            0  0  0 0  0   0   0



             읒mn쁜금gEa三i＞ 능m三m>
                             尸



                             F




                  크
                  0


                      0
                       1             2   3     4       5      6        7     8   9   10
                                                No. of fuzzy partition

                                             (b) 퍼지 지수 m= 2
                ［그림 5-4] 가스 용광로 데이터의 최적 퍼지 분할


===== PAGE 141 =====
140      퍼지, 진화컴퓨팅 프로그래밍



  mm 리스트 5니 唾 가스1용광로 퍼지 모델의 구조 인식

       % 파일명： fiizmod_structure.m
       % 퍼지 클러스터링을 이용한 퍼지 모델의 구조 인식
       % Box-Jenkin의 가스 용쾅로 데이터 사용


       cmax = 10; % 최대 퍼지 분할 수
       cmin = 2; % 최소 퍼지 분할 수
       m = 2; % 퍼지 지수（m > I)
       eps = Le-4; % 종료조건


       load BoxJer血ins 1.tra; % 뎨이터 파일（146행 3열） 읽기
       Data = BoxJenkins 1;
       [d,n] = 計ze(Data); % d: 차원， n: 뎨이터 수
       sxb = ones(cmax,1); % 퍼지 분할 평가 지수를 저장할 변수
       md = rand(cmax,n); % [0,1] 사이의 랜던 값


       的r （二 = cmin:cmax
             [UO] = initFcmc(c,Data); % 분할행렬의 초기치 설정
             [U,V,iter] = fcmc(m,eps,UO,Data); % 퍼지 클러스터링 실행
             sxb(c) = Sxb(m,U,V,Data); % 평가척도 계산
       end


       {minmsxb,opt긔 = min(sxb(cmin:cmax)); % 최소 평가 지수 값과 그 때의 분할 수


       x = cmin:cmax; % 가로축 변수
       plot(x,sxb(cmin:cmax),'b-');
       xlabel('寸o. of fuzzy partition');
       ylabel('Value of validity measure, Sxb');
       text(4,0.9,['no. of optimal partion = '   num2str(opt_c+cmin-1)]);
       text(4.5,0.8, ['m = ' num2str(m)]);
       axis([1 emax 0 1]);




      결정된 피지 클러스터들을 이용 퍼지 모델의 구조를 인식하고, 차분진화를 이용 퍼지 모델
      의 파라미터를 인식한다. 이 과정어］ 대한 매트랩 코드가 리스트 5-2이고, 파라미터 인식어］
      실수형 유전알고리즘을 사용한 경우가 코드 5-3이다．


===== PAGE 142 =====
                                                          5장. 퍼지 규칙의 생성



的    리스트 5-2 斗 가스H용광로 퍼지 모델 구축（차분진화 사용）

    % 파일명： fuzmod build de.m
    % 퍼지 모델 구축
    % Box-Jenkin의 가스 용광로 데이터 사용
    이C;
    이ear;


    % 구조 인식 가운데 클러스터 중심 벡터 인식
    m = 2; % 퍼지 지수(m > 1)
    eps = 1.e-5; % 종료조건
    c = 2; % 퍼지 분할（클러스터） 수
    load BoxJenkinsHl .tra; % 데이터 파일（146행 3열） 읽기
    Data = BoxJenkins I;


    % 분할행렬의 초기치 설정
    [UO] = initFcmc(c,Data);


    % 퍼지 클러스터링 실행
    [U,V,iterl = fcmc(m,eps,UO,Data);


    % 파라미터 탐색 범위 설정
    [bounds] = setBounds(V,Data);


    % 파라미터 인식
    fname = 'fuzmodelFunc'; % 목적함수를 정의하는 파일명 fuzmodelFunc.m
    [nx nd] = size(bounds); % nx: 해의 수， nd = 2（최소， 최대I)
    parms = Data; % 문제 정의에 필요한 파라미터로 규칙 수와 데이터 행렬을 지정
    maxGen = 500; % 최대 진화 세대 수
    goal = 6.0; % 목표 적합도 = 1/목표 목적함수 값（l刀）
    epsFit = l .口5; % 목표 적합도 값어］ 대한 허용오차
    np = 30; % 집단의 크기
    F = 0.5; % 차분 크기 조정 가중치
    Cr = 0.5; % 교배율
    ndisp = 10; % 중간 결과를 화면에 표시하는 세대 간격
    nde = 1; % 교배용 개체 생성 방법 선택
    fType = 1; % 목적함수 유형 선택용으로 0 이면 최소화， l 이면 최대화 문저］


===== PAGE 143 =====
口m       퍼지, 진화컴퓨팅 프로그래밍


 % 차분진화
 [x,fit,nfit,fithist] = de(thame,nx,bounds,parms,maxGen,goal,epsFit,np,F,Cr,ndisp,nde,fType);
     x % 최적 해
     fit % 최적 해어］ 대한 적합도 값
 nfit % 최적 해를 얻을 때까지 실행된 적합도 함수 평가 횟수
     fid = fopen('gasFurnace.mod','w'); % 데이터 저장 파일 오픈
     如rintf(fid,'%10.5f               ',x); % 퍼지 모델 파라미터 저장
     fclose(fid); % 파일 닫기
     plot(fithist);
     xlabel('generation');
     ylabel('fitness function value');


     % 퍼지 모델의 학습 오차 계산
     load gasFurnac已mod; % 퍼지 모델 파라미터 로드
     load BoxJenkins 1.tra; % 학습용 뎨이터 로드
     Data = BoxJenkins 1;
     train_obj = fuzmod_test(Data,gasFumace);
     train_obj


     % 퍼지 모델의 검증
     load BoxJenkins 1.tst; % 평가용 뎨이터 로드
     Data = BoxJenkins 1;
     test_obj = fu기llod_test(Data,gasFurnace);
     test_obj




                      function [bounds] = setBounds(V,data);
                 % 파일명： setBounds.m
                 % 퍼지 클러스터의 중심 벡터를 이용해서
                  % 모델의 파라미터 인식을 위한 해의 탐색 범위 설정
                  % Box-Jenkin의 가스 용쾅로 뎨이터 사용
                  % 사용법 [bounds] = setBoun小（V,data)


                  % 클러스터 중심 벡터를 행： 클러스터 수（아 열： 차원（d）으로 변경
                  tmp    =   V   ';
                  V = tmp;
                  [nRule d] = size(V); % nRule: 클러스터 수， d: 차원（입력변수 + 출력변수）


===== PAGE 144 =====
                                                                5장. 퍼지 규칙의 생성   ] 143
 % 중심 벡터를 이용 해의 탐색 범위 결정
 % u(t-4), y(t-1), y(t)의 최소값 결정
 x_min = min(data);
 % u(t-4), y(t-1), y(t)의 최대값 결정
 x_max = max(data);
% 최대 - 최소： 크기
 x_del = xmax - xmin;
% 최대, 최소 여유 범위
毛mm = 毛mmll - 0.1求x del; % 10 피센트만큼 더 작거］
毛max = x max + 0.1平毛del; % 10 퍼센트만큼 더 크거1
% 열 단위로 오름차순으로 정렬
sortV = sort(V);


可 % 아래 본문 설명 참조
% 후건부 싱글톤의 탐색 범위， 식（5.1旬에서 B
bounds_Bi = zeros(nRule,2);
for i=1:nRule
      mlld = find(sortV(:,d) =    V(i,d));
      if (nRule == 1)
            bounds_Bi(i,:) = 匡皿奴d) x_max(d)];
      이se
            if (mnd == 1)
                  bounds卜Bi(i,:) = [x_min(d) sortV(ind+1,d)];
            elseif (mnd == nRule)
                  bounds_Bi(i,:) = [sortV(ind-1,d) x_max(d)];
            이Se
                  bounds_Bi(i,:) = [sortV(ind-1,d) sortV(ind+1,d)];
            end
      end
end
自




% 전건부 멤버쉽 함수의 탐색 범위
nx = d -1; % 입력 변수의 수
bounds_C = zeros(nRule永nx,2); % 식（5.14）어］서 q
bounds寸Dl = t兀undsHC; % 식（5.15）어］서 dl
bounds_Dc = bounds寸C; % 식（5.15）어］서 dC二


===== PAGE 145 =====
                                      水
144   퍼지, 진화컴퓨팅 프로그래밍



         bounds_Dr = boun小르 % 식（5.15）에서 dr

         % 전건부 멤버쉽함수의 거리에 대한 탐색 범위를
         % 해당 변수의 0 시 （최r作최소）/2］로 함
         白r i=1:nRule
               for j=1:nx
                     k = (i_1)*nx + j;
                     bounds_Dl(k,:) = [0      x_del(j)./nRule];
               end
         end
         bout岫I元 = bounds ［가；
         bounds Dr = bounds Dl;


         % 전건부 멤버쉽함수의 중심 값어］ 대한 탐색 범위， 식（5.14）에서 q
         白r 江1:nRule
               for j=1:nx
                     k = (i_1)*nx + j;
                     mlld = find(sortV(:}j) == V(i,j));
                     if (nRule =      1)
                           t兀unds_C(k,:) = [x_min(j) 毛ma씨月；
                     이se

                           if (mnd == 1)
                                  bounds_C(k,:) = [x_min(j) sortV(ind+1 j)];
                           else汀 (mnd == 1浪ule)
                                  bounds_C(k,:) = [sortV(ind-1j) x_max(j)];
                           else
                                  bounds_C(k,:) = [sortV(md-1 j) sortV(ind+1,j)];
                           end
                     end
               end
         end


         % 하나의 행렬로 만듬
         bounds = [bounds_Bi; bounds_C; bounds_DI; bounds_Dc; bounds_Dr];


===== PAGE 146 =====
                                                        5장． 퍼지 규칙의 생성   ］口m




 凡nction [x, fit] = fuzmodelFunc(x,parms);
 % 파일명： fuzmodelFunc.m
 % 목적함수로 차분 진화에서는 적합도 함수로 그대로 사용
 % 사용법 [x, obj] = fuzmodelFunc偶parms);
%               x: 입력 벡터
%               parms: 문제 관련 파라미터 벡터
%               fit: 적합도 = 1/（목적함수 값 + 벌칙 값）
% 퍼지 모델의 오차 계산


data = parms; % data 행렬
cPenalty = 10; % 벌칙 상수
[n,d] = size(data); % n: 뎨이터 수， d: （입력 + 출력）변수의 수
ninp = d - 1; % 입력변수의 수
[s,nx] = size(x); % nx: 해의 차원
nRule = round(nx/(1 + 伊而p)); % 퍼지 규칙의 수를 계산


% 퍼지 모델 추론 결과와 벌칙 인가 횟수를 리턴 값으로 받음
% 데이터의 입력변수 부분만 넘김
[infer nPenalty] = fuzlnfer(data(:, 1:ninp),nRule,x);
error = (data(:,d) - infer(:,1)).''2;
obj = suin(error)In; % 데이터 출력과 모델 출력 사이의 오차
penalty = nPenalty札Penalty; % 벌칙 계산， 식（5.18)
obj = obj + penalty; % 벌칙 부가
fit = l／아）LI; % 식（5.19)




function [infer, nPenalty] = f丑nfer(data,nRule,x);
% 파일명： fuzlnfer.m
%x（해）로부터 퍼지 모델을 구성하고 뎨이터어］ 대한 퍼지 출력 계산
% 사용법: infer = fuzlnfer(data,nRule,x);
%      출력변수：
%           infer: 퍼지 모델 출력 벡터（
                              ［데이터 수 xl］의 열벡터）
%           nPenalty: 벌칙 횟수
%      입력변수：


===== PAGE 147 =====
                                  水
口m[   퍼지, 진화컴퓨팅 프로그래밍



         [n,ninp] = 前ze(data); % n: 뎨이터 수， ninp: 입력변수의 수
         infer = zeros(n,1); % 퍼지 모델의 출력 저장
         Bi = x(1,1:nl之ule); % 해（x）에서 후건부 싱글톤 파라미터 저장
         mlld = nRule;
         Ci = x(1,(ind+1):(ind+nRule木ninp)); % 전건부 멤버쉽함수의 중앙 값 저장
         mlld = nRule + nRule*ninp;
         DI = x(1,(in小1):(mnd+nRule*ninp)); % 전건부 멤버쉽함수의 좌측 거리 저장
         mlld = nRule + 2*nRule*nmnp;
         Dc = x(1,(ind+1):(ind+nl之ule求ninp)); % 전건부 멤버쉽함수의 중앙 거리 저장
         mlld = nRule + 3*nRule*nmnp;
         I万 = x(1,(ind+1):(ind+nRule牛ninp)); % 전건부 멤버쉽함수의 우측 거리 저장
         wi = ones(n,nRule);
         mi = zeros(n,ninp);


          for j=1:nRule
                凡r k=1:ninp
                mlld = (j 1)*nmnp + k;
                       % 멤버쉽함수 호출
                parms = [Ci(ind) DI(ind) Dc(ind) Dr(ind)};
                       mi(:,k) = triangleTrapezoidal(data(:,k),parms);
                      %(1) 곱하기어］ 의한 전건부 규칙 만족도 계산
                       wi(:j) = wi(:j).*mi(:,k);
                end
                %wi(:1j) = min(mi')'; % (2) 최소값에 의한 전건부 규칙 만족도 계산
         end
          sumwi = sum(wi');
          for i=1:n
                白r j=1:nRule
                      if (sumwi(i) N= 0)
                         wi(ij) = wi(ij)/sumwi(i); % 만족도의 정규화
                      end
                end
                infer(i) = sum(wi(i,:).*Bi);
          end
         % 모든 규칙에 대한 만족도가 0인（멤버쉽함수어］ 공집합이 존지b
          % 횟수를 계산 np어］ 저장
         [r,nPenalty} = size(find(sumwi        0));


===== PAGE 148 =====
                                                 5장. 퍼지 규칙의 생성   ] 147

function [mu] = triangleTrapezoidal(x,parms);

% triangleTraperzoidal.m
% A]용법 mu = trianglelraperzoidal(c,dl,dc,dr);
%          출력변수：
%             mu: 멤버쉽함수 값, 소속정도
96         입력변수：
%             x: 입력 뎨이터
%             parms: 멤버쉽함수 파라미터로 [cp dl dc dr]
%             cp: 멤버쉽함수의 중심 값
%             dl, dc, dr: 멤버쉽함수의 좌측, 중앙 및 우측 거리


cp = parms(1);
dl = parms(2);
dc = parms(3);
dr = parms(4);
mu = zeros(size(x));


if (dc =     0 &dl= = 0 & dr ==0)
     % 멥버쉽함수가 존재하지 않음
    % mu = zeros(size(x)); 위어］서 정의
이se汪 (dc == 0 & dl 싸＝ 0 & dr N= 0)
     b = cp;
     a = b - dl;
     c = b + dr;
     mu = triangle(x,[a b c]); % 삼각형 멤버쉽함수 호출
elseif (dc -= 0 & dl == 0        & dr N= 0)
     a = cp - dc/2;
     b = cp + dc/2;
     c = b + dr;
     for i=너ength（지
           if (x(i) < a) mu(i) = 0;
           elseif (x(i) >= a & x(i) <= b)
                    mu(i) = 1;
           이Se汪 (x(i) > b & x(i) < c)
                    mu(i) = (x(i)七玖b미 + l;
           else


===== PAGE 149 =====
四   ［ 퍼지， 진화컴퓨팅 프로그래밍
                             mu(i) = 0;
                  end
               end
          elseif (de N= 0 & dl 시= 0       & dr =   0)
               b = cp - dc/2;
               a = b - dl;
               c = cp + dc/2;
               for i=1:Iength(x)
                  if (x(i) <= a) mu(i) = 0;
                  이se迂 (x(i) > a & x(i) < b)
                          mu(i) = 似(i)劫仄b-a) + 1;
                  이se汪 似(i) >= b & x(i) <= c)
                             mu(i) = 1;
                  else
                             mu(i) = 0;
                  end
               end
          이se汗 (dc == 0 & dl          0   &dr- =O)
               a = cp;
               b = a + dr;
               for i=1:佃喀h（자
                  if (x(i) < a) mu(i) = 0;
                  이se汪 似(i) >= a & x(i) < b)
                          mu(i) = 似(i)-a以十b) + 1;
                  이se
                             mu(i) = 0;
                  end
               end
          이se仟 (dc 시＝ 0 & dl == 0         & dr == 0)
               a = ep - dcl2;
               b = cp + dc/2;
               for i=l:length(x)
                  if (x(i) < a) mu(i) = 0;
                  elseif (x(i) > b)
                             mu(i) = 0;
                  else
                             mu(i) = 1;


===== PAGE 150 =====
                                                   水
                                                       5장. 퍼지 규칙의 생성   149


             end
        end
 elseif (dc =      0 & dl N= 0 & dr == 0)
       a = cp - dl;
       b = cp;
       for i=너en합h（지
          if (x(i) < a) mu(i) = 0;
          이se迂 (x(i) >= a & x(i) < b)
                     mu(i) = (x(i)-b)/(b-a) + 1;
          이se
                     mu(i) = 0;
          end
       end
else
       b = cp - dcl2;
       a = b - dl;
       c = cp + dc/2;
       d = c + dr;
       mu = trapez아dal(x,[a b c dl); % 사라디꼴 멤버쉽함수 호출
end




血nction [test_obj] = fuzmodtest(data,model);
% 파일명： fuzmod test.m
% 평가용 데이터를 사용하여 퍼지 모델의 오차 계산
% 사용법 [test_obj] = fuzmod_test(data,model);
%       출력변수
%               test_obj: 출력 오차
%       입력변수
%               data: 평가용 뎨이터 행렬
%               model: 퍼지 모델 파라미터


[n,d] = size(data); % n: 데이터 수， d: （입력 + 출력）변수의 수
ninp = d - 1; % 입력변수의 수
[s,nxl = size(model); % nx: 해의 차원
nRule = round(nx/(I + 4水ninp)); % 퍼지 규칙의 수 계산


===== PAGE 151 =====
150          퍼지, 진화컴퓨팅 프로그래밍



                     % 퍼지 모델 추론 결과와 벌칙 인가 횟수를 리턴 값으로 받음
                     % 데이터의 입력변수 부분만 넘김
                     [infer nPenalty] = fuzlnfer(data(:, 1:ninp),nRule,model);
                     error = (data(:,d) -   infer(:,l)).八2;
                     test_obj = sum(error)/n; % 데이터 출력과 모델 출력 사이의 오차




      1密 위의 코드에 표시된 부분

      setBounds.m어］서 식（5.16）에 해당하는 후건부 싱글톤의 탐색 범위를 계산하는 부분을 알
  아보자. 전건부의 경우 식（5.15）에 해당하는 멤버쉽함수의 중심 값의 범위는 후컨부 싱글톤
  과 동일한 방법을 사용하며, 식（5.16）어］ 하당하는 좌우측 및 중앙 거리의 범위는 데이터의
  최소, 최대값에 의해 쉽게 계산된다. 다음의 행렬 V는 클러스터링 결과인 클러스터 중심 벡터
  를 전치시킨 행렬이다. 따라서 행은 클러스터의 수（규칙의 수）를, 열은 변수를 나타닌仁｝. 첫
  열은 입력 u (t -4) , 둘째 열은 입력 y (t -1）을, 셋째 열은 출력 y (t）를 나타낸다. 乂m血I
  과 x max는 학습용 데이터에서 변수별 최소와 최태값을 나타낸다．


      V=
                                                              x m끄I =
            1.2513      56.9273       56.9300                     2.7160   45.6000   45.6000
           1.4391       48.6591      48.6479                  x max 二二

           0.3018       52.3293      52.3015                     2.8340    60.2000   60.2000


      sortV는 행렬 V를 열 단위로 크기 순으로 정렬한 것이다. 출력 y (t ）어］ 대한 싱글톤 彦 의
  탐색 범위를 결정하기 위해 V와 sortV의 3열만을 고려하자．


      sortV =
           -1.2513      48.6591       48.6479
           0.3018       52.3293      52.3015
           1.4391       56.9273      56.9300


      V의 첫 항목은 56.930이고 이것은 sortV에서 3（코드에서 ind=3）번째로 큰 값이고 이는 규


===== PAGE 152 =====
                                     1    5장. 퍼지 규칙의 생성
                                                          口國1

칙수와 같기 때문어］ 아래에 기술된 bounds의 回어］ 보인 것처럼 탐색 범위는 둘째로 큰 중심
값에서 변수의 최대값까지이다. 둘째 항목인 48.6479는 제일 작은（ind=1) 중심 값이므로 탐
색범위는 ＠에서처럼 변수의 최소값에서 둘째로 큰 중심 값까지이다. 셋째 항목인 52.3015는
제일 작지도, 크지도 않 O 口 쿠（ind=2) 탐색범위는 자신 보다 하나 작은（ind=1) 중심 값에서
자신 보다 하나 큰（ind=3) 중심 값까지이다（（今 참조）. bounds에서 （孕 N ＠까지는 전건부 멤
버쉽함수의 중심 값m）에 대한 탐색범위로 계산 과정은 후건부와 동일하다 ．차이는 입력 변
수가 2개이기 때문어］ 射2=6（규칙 삳변수 수）가 필요하며, ＠는 첫 규칙의 입력 n (t - 4),
＠는 입력 y (t -1) , ＠은 둘째 규칙의 입력 u (t -4）의 탐색범위, 이런 순서로 이어진다．

匈 N 的는 전건부 멤버쉽함수의 좌측 거리（m力에 대한 것이고, 그 다음 6개는 중앙 거리

(d타）, 나머지 6개는 우측 거리（dr}）어］ 대한 탐색범위이다. 그 순서는 전건부 멤버쉽함수의

중심 값의 경우와 동일하다.


bounds =
 侄）   52.3015   60.2000
(2)   45.6000   52.3015
（多    48.6479   56.9300
(4)   -2.7160    0.3018
@     52.3293   60.2000
（弓    0.3018     2.8340
(i)   45.6000   52.3293
匣）    -1.2513    1.4391
（今    48.6591   56.9273
匈          0     2.7750
區）         0     7.3000
匡｝         0     2.7750
4今         0     7.3000
d4)        0     2.7750
區）         0     7.3000
           0     2.7750


===== PAGE 153 =====
回   ［ 퍼지 진화컴퓨팅프로그래밍
                 ，




                     0   7.3000
                     0   2.7750
                     0   7.3000
                     0   2.7750
                     0   7.3000
                     0   2.7750
                     0   7.3000
                     0   2.7750
                     0   7.3000
                     0   2.7750
                     0   7.3000
    自




         리스트 千2 ' 가스1용광로 퍼지 모델 구축（유전알고리즘 사용）

        % 파일명： fuzmod_build_rga.m
        % 퍼지 모델 구축
        % Box-i enkin의 가스 용광로 데이터 사용
        dc;
        clear;


        % 구조 인식 가운데 클러스터 중심 벡터 인식
        m = 2; % 퍼지 지수（m > I)
        eps = l.e-5; % 종료조건
        c = 2; % 퍼지 분할（클러스터） 수
        load BoxJenkins I .tra; % 데이터 파일（146행 3열） 읽기
        Data = BoxJenkins I;


        % 분할행렬의 초기치 설정
        [UO] = initFcmc(c,Data);


        % 퍼지 클러스터링 실행
        [U,V,iter] = fcmc(m,eps,UO,Data);


        % 파라미터 탐색 범위 설정


===== PAGE 154 =====
                                                              5장. 퍼지 규칙의 생성       口m
[bounds] = setBounds(V,Data);


% 파라미터 인식
maxGen = 500; % 최때1 진화 세대 수
popSize = 30; % 집단 크기（>=20)
epsFit = 1.e-5; % 두 적합도 값의 차를 구분할 수 있는 크기
galype = 1; % 실수 표현이면 l
epsVar = 1; % 각 변수에 필요한 이진 비트 수를 결정．
options = [epsFit gaType epsVar]; % 유전알고리즘 옵션
eva作N = 'fuzmodelFunc'; % 적합도 함수명
evalOpts = Data;
% 종료： 아라1 (1）과 (2）중 선택
%termFN = 'maxGenTerm'; % (1)
%termOpts = [maxGen]; % (I)
termFN = 'opt人1axGenTerm'; % (2）종료조건 함수명
goalFit = 6.0; % (2) 적합도 함수 목표 값
termOpts = [maxGen goalFit epsFit]; % (2) 종료조건 파라미터
% 선택： 아라1 (1), (2), (3）중 선택
selectFN = 'roulette'; % (1) 선택 방법에 대한 함수명
selectOpts = []; % (1) 선택 방법의 파라미터
%selectFN = 'normGeomSelect'; % (2)
%pBest = 0.01; % (2) 최우수 개체가 선택될 확률
%selectOpts = [pBest]; % (2)
%selectFN = 'tournSelect'; % (3)
%nSize = 2; % 토너먼트 크기 % (3)
%selectOpts = [nSize]; % (3)
%교배
xOverFNs = 'arithXover heuristieXover 計mpleXover'; % 교배 함수명
nXover = 1; % 교배 연산자의 적용 횟수
nlry = 3; % 재시행 횟수
xOverOpts = [nXover 0; nXover nlry; nXover 0]; % 교배 관련 파라미터
% 돌연변이
% 돌연변이 힘수명
mutFNs = 'boundaryMutation multiNonUnil入4utation nonUnifMutation unifMutation';
n入4ut = 1; % 교배 연산자의 적용 횟수
pShape = 3; % 모양 결정 파라미터
% 돌연변이 관련 파라미터


===== PAGE 155 =====
四   ［ 퍼지 진화컴퓨팅프로그래밍
            ，                             ,




    mutOpts = [nMut 0 0; nMut maxGen pShape; nMut maxGen pShape; nMut 0 0];


    % 집단 생성 및 초기화
    [startPop] = initializega(popSize,bounds,evaI剛,evalOpts,options);


    % 유전알고리즘 본체 실행
    [bestX,endPop,bPop,甘acelnfo] = ga(bounds,eva1FN,evalOpts,startPop,options,termFN,termOpts,...
                                                 selectFN,selectOpts,xOverFNs,xOverOpts,mutFNs,mutOpts);


    bestX % 최적하1
    fid = fopen('gasFurnace.modI,!w?); % 뎨이터 저장 파일 오픈
    印rintf倬d,'%10.5f           ',bestX); % 퍼지 모델 파라미터 저장
    fclose(fid); % 파일 닫기


    % 세대 별 최우수 적합도의 변화
    plot(tracelnfo(:, 1),tracelnfo(:,2),'b-');
    axis ([1 maxGen 0 goalFit]); % 그림의 축 법위 설정
    xlabel('generation');
    ylabel('fitness: f(x)');


    % 퍼지 모델의 학습 오차 계산
    load gasFumace.mod; % 퍼지 모델 파라미터 로드
    load BoxJenkins l.tra; % 학습용 데이터 로드
    Data = BoxJei水11据 1;
    train_obj = fuzmod_test(Data,gasFumace);
    train_obj


    % 퍼지 모델의 검증
    load BoxJenkins_l .tst; % 평가용 데이터 로드
    Data = BoxJenkins 1;
    test_obj = fuzmod.btest(Data,gasFurnace);
    test_obj


===== PAGE 156 =====
                                                 5장. 퍼지 규칙의 생성   J=   m


5.3.2 모델의 평가

     구축된 모델의 타당성을 검증하는 과정에서는 모델링어］ 사용되었턴 데이터와는 별도의 평
가용 데이터를 사용해야 한다. 이를 모델의 검증佃alidation)이라 부르는데, 분할 검증, 교차
검증（cross-validati아1) 및 부드人트랩（bootstrap) 방법이 있다．
     일반적으로 데이터의 양이 충분하면 분할 검증을 사용해도 무방하지만, 데이터가 적은 경
우에는 교차 검증이나 너드人트랩 방법이 우수한 것으로 알려져 있다. 특히 , 데이터가 아주
적은 경우（대개 30개 이하）에는 leave-one-out 교차 검증이 가장 효과적이다．


     d) 분할 검증（Split Samp沌 또는 H이d尸叩t) 방법
     데이터를 학습용（모델링）과 검증용 두 집합으로 분할하여 사용하기 때문어］ 학습과 검증 사
이에 데이터 교차가 발생하지 않는다. 모델 구축 과정을 자동화하기 위해서 학습용 데이터를
두 개로 나누어 하나는 학습어］, 나머지는 시험에 사용할 수도 있다. 이 때 학습이 끝나면 시험
데이터로 모델 오차가 목표범위에 도달하는지를 확인해서 목표어］ 도달하면 모델링을 종료하
고, 그렇지 않으면 목표를 만족할 때까지 학습 뎨이터로 새로운 모델을 구축한다. 시험용 더］
이터에 대한 목표오차를 만족하면, 평가용 데이터를 사용해 구축된 모델의 타당성을 검증한
다．
     (2) 교차 검증（Cross-Validation)
     · k배 교차 검증（K-Fold Cross-Validation): 이 방법은 전체 데이터를 가능한 동일한 크기
      의 k개 집단으로 분할하고, k번 학습을 수행하는데, 이 때 순차적으로 1개의 데이터 집합
      을 모델링에 사용하지 않고 평가용으로 사용한다. k 값으로는 보통 10이 많이 사용된다．
     · 하나를 제외한 교차 검증（Leave-One-Out Cross-Validation): 교차 검증에서 k 값이 전
      체 데이터의 크기와 동일한 경우로, 전체 데이터 가운데 검증에 사용할 하나를 제외하고
      나머지를 학습에 사용한다. 이 과정은 데이터 수만큼 반복되어야 한다. 매번 하나가 아닌
      V개의 데이터를 제거하는 방법은 leave-v-out 교차 검증이라 부른다．
     · 잭 나이프 검증（Jack-Knife Validation): 데이터를 분할해서 학습과 평가어］ 사용하는 방
      법은 leave-one-out 교차 검증과 동일하기 때문어］ 교차 검증 방법의 하나로 볼 수 있다．
      하지만 교차 검증 방법이 일반적인 오차（오차 제곱）를 계산하는 반면, 잭＋나이프 검증은
      다앙한 통계적 수치를 활용한다. 예를 들면, 전체 데이터 집합에 대한 오차와 뎨이터의 부
      분 집합어］ 대한 오차의 평균 사이의 편차를 계산할 수 있다. 물론, 일반적인 오차를 계산하


===== PAGE 157 =====
156       퍼지, 진화컴퓨팅 프로그래밍



       는데 잭 나이프 검증을 사용했다면 leave-one-out 교차 검증과 다를 바 없다. 예로, 일
       반 오차를 졔산하는 50% 잭m나이프 검증은 분할U샘플 방법과 유사한데, 즈中나이프의 경
       우에는 학습 및 평가용으로 사용되었던 데이터가 다음에는 역으로 평가 및 학습용으로도
       사용된다．


      (3) 부트스트랩（Bootstrap) 방법
      여러 가지가 있지만, 가장 단순한 형태는 전체 Ti개의 데이터에서 차례로 Ti개의 샘플 데이
  터를 무작위로 선택해 이를 학습용으로 사용한다. 이 때 선택된 데이터는 원래 데이터 집합어］
  그대로 남아 있으며 그것의 복제 데이터를 추출한 것이다. 따라서 통일한 데이터가 여러 번
  추출될 수 있고 아예 추출되지 않을 수도 있다. 보통 분류기（classifier）에서 예측 오차를 추
  정하기 위해 식（5.20）과 같은 0.632 bootstrap 추정치를 이용한다. Ti개의 데이터에서 Ti번

  데이터 추출을 시도하였을 때 특정 데이터가 추출되지 않을 확률은 (1 - i/ n)" 七c_ i 之
  0.368이다. 이는 전체 데이터（평가용 데이터로 사용） 가운데 대략 63.2％가 학습용으로 사용
  됨을 의미한다. 따라서 평가용 오차어］ 대한 추정치는 비관적（63.2%만 포함）이며 데이터 크기
  가 아주 작으면 매우 비관적일 것이다. 너 드人E랩 샘플을 다수 만들어 식（5.20）으로 계산한
  추정 오차의 평균을 구해서 이를 최종 추정 오차로 간주한다．


        E0.632 = O.368E.QU, + O.632E,8t                        (5.20)


  耳, amn는 학습용 데이터에 대한 모델 오차이고 耳毗는 평가용 데이터어］ 대한 오차이다．

  이 방법은 일반 오차만이 아니라 신뢰 구간（car寸idence ii北ervals）을 추정하는데도 사용된다．


      리스트 5-3은 가스e용광로 데이터를 학습 및 평가용 뎨이터로 분할하는 코드이다. 여기서
  는 BoxJenkins.dat 파일의 데이터를 처음 반과 나머지로 나누어 이를 각각 학습（파일：
  BoxJenkins 1.tra) 및 평가용 데이터（파일： Bo兀Jenkins_i. tst）용으로 만드는 것과, 홀수 번
  째에 위치한 것과 짝수 번째에 위치한 것을 학습（파일： BoxJenkins그. tra) 및 평가용（파일：
  Bo乂Jenkins그.tra）으로 만드는 것을 기술한다．


===== PAGE 158 =====
                                                         5장. 퍼지 규칙의 생성   J1m
  리스트 5-3 蜘 가스H용광로 학습 및 평가용 데이터 분리

% 파일명： mkData-gasFumce.m


load BoxJenkins.dat; % 2 입력， l 출력의 292깨땍 데이터
[n,d] = size(floxienkins);


% 292 개의 뎨이터에서 처음 반은 모델용， 나중 반은 평가용 데이터로 만듦
half = round(n12);
x = BoxJenkins(1:half,:);
fid = fopen('BoxJenkins_l.tra','w'); % 모델용 뎨이터 저장 파일 오픈
加rintf(fid,'%lO.5f    %10.5f   %lO.5f\n',x'); % 데이터 저장
fclose(fid); % 파일 닫기
x = BoxJenkins((ha仟＋1):n,:);
fid = fopen('BoxJenkins_l.tst','w'); % 평가용 뎨이터 저장 파일 오픈
印rintf(fid,'%10.5f    %lO.5f   %I O.5f\n',x');
fclose(fid); % 파일 닫기


odd = (1:2:n)'; % 홀수열
even = (2:2:n)'; % 짝수열
x = BoxJenkins(odd,:);


% 292 개의 데이터에서 홀수 번째는 모델용， 짝수 번째는 평가용 데이터로 만듦
fid = fopen('BoxJenkins-.2.tra','w'); % 모델용 뎨이터 저장 파일 오픈
印rintf(fid,'%lO.5f    %10.5f   %lO.5f\n',x'); % 뎨이터 저장
fclose(fid); % 파일 닫기
x = BoxJenkins(even,:);
fid = fopen('BoxJenkinsH2.tst','w'); % 평가용 데이터 저장 파일 오픈
印rintf(fid,'%lO.5f    %lO.5f   %10.5f\n',x');
fclose(fid); % 파일 닫기


===== PAGE 159 =====
  퍼지, 진화컴퓨팅 프로그래밍




                              [ 연습문저1 ]
[1] 리스트 5-1과 5-2를 사용해서 10번의 실험을 수행해서 평균과 표준편차를 구해 아래
  표의 빈칸을 채워라. 이 때 집단 크기는 30, 최대 진화수는 500, 목표 적합도는 6이다．
  이상의 실험을 다음의 두 데이터 집합에 대해 실행해 보고 그 결과를 고찰해보자. 데이
  터 파일은 매트랩 코드 파일과 함께 제공된다．

  데이터 파일： Bo乂兀nkins 1.tra, Bo乂Jenkins그 .tst
              Bo兀Jenkins 2.tra, BoxJenkins_2.tst


                         가스U용광로의 퍼지 모델 평가




    \
                                 오차
                                                    적합도 평가 횟수
                         학습                평가
                    평균     표준편차       평균     표준편차   평균   표준편차
        차분진화
        실수형
      유전알고리즘




[2] 비선형 수식 데이터를 사용하여 입출과 관계를 기술하는 퍼지 모델을 만들어보자. 모델
  을 만들 때는 학습용 데이터 Sugeno.tra를, 모델을 평가할 때는 Sugeno.tst를 사용한
  다. 데이터 파일은 매트랩 코드 파일과 함께 제공된다．
  이 데이터는 다음의 비선형 수식에서 만들어진 것이며 , 데이터 파일에서 3, 4열은 불필
  요한個ummy) 입력 T3와 勺어］ 대한 것으로 임의의 값으로 주어졌다. 따라서 구조 인식

  에서 입력 心와 x4가 출력어］ 영향을 미치지 않음을 파악할 수 있다면 퍼지 규칙의 전컨

  부어］ 이들 변수가 포함될 필요가 없다. 불행히도 퍼지 클러스터링으로는 이를 확인하기
  어렵다（변수를 교체하면서 성능 비교를 통해 확인할 수는 있지만 변수가 많아지면 그
  조합수가 기하급수적으로 많아지므로 비현실적임）. 대신에 요인분석（FA: Factor
  Analysis）나 주성분 분석（PCA: Principal Component Analy前旬으로 입출력 변수들의
  상관관계를 알아내고 출력어］ 상관관계가 높은 변수들만을 입력으로 사용한다．
                    y = (1 + x尸 + 町비2 1 드 :l;l, x2 됴 5


===== PAGE 160 =====
                                                          5장. 퍼지 규칙의 생성           159


                               弗 심화 학습 자료 好


'H. S. Hwang and K. B. Woo, "Linguistic Fuzzy Model Identification," TEE
 Proceeding Part D.-Control Theory and Application, Vol. 142, No. 6, pp.
 537-544, November, 1995.
'Y. H. Joo, H. S. Hwang, K. B. Kim, K. B. Woo, "Fuzzy system modeling by fuzzy

 partition and GA hybrid scheme," Fuzzy Set and Systems, Vol. 86, pp. 279-288,
 1997.
'H. S. Hwang, "Automatic design of fuzzy rule base for modeling and control
 using evolutiona玎 programming," TEE Proceeding Part D.-Control Theory and

 Applications, Vol. 146, No. 1, pp. 9-16, January, 1999.
'S. J. Kang, C. H. Woo, H. S. Hwang, and K. B. Woo, "Evolutionary design of
 fuzzy rule base for nonlinear system modeling and control," IEEE Trans. on
 Fuzzy Systems, Vol. 8, No. 1, pp. 37-45, Febua玎 2000.
.U徊rth J. S. U., Co／刀刃끄ter Inte끄sive Statistica/ 끄ethods l乞／ida苡끄2, A勿del
 Selection, and Bootstrap, London: Chapman & Hall, 1994.
'Shao J. and Tu D., The Jac火nife and Bootstrap, New York: Springer- Verlag,

 1995.
·Sni.jders T. A. B., "On cross-validation for predictor evaluation in time series,"
 in Dijkstra, pp. 56-69, 1988.


===== PAGE 161 =====
부록   入4atlab 사용법



        客 1 매트랩의 특징
        串 l ) 매트랩의 실행 방법
        水 2) 매트랩 명령어
        ：恥 3) 매트랩 기초
        串 4) 그래프 그리기
        永 5) 프로그래밍의 작성과 실행


===== PAGE 162 =====
                                                부록. Matlab 사용법       163




"       매트랩（matlab）은 MATr奴 LABorat.玎의 줄임말로, 계산과 행렬과 벡터의 조작을 편리하고 효
      과적으로 처리해주는 인터프리터(interpreter）기반의 프로그래밍 언어이다. 인터프리터 기반이기
      때문어］ 컴파일러 언어 보다 실행 속도가 느린 단점이 있지만, 매트랩에서 사용하는 명령문은 프로
      그래밍 언어의 함수（function)와 같아서 복잡한 계산이 필요한 프로그램도 매트랩에서는 간단하
      거］ 작성, 그 결과를 빠르게 확인할 수 있는 장점이 있다. 이런 장점 때문에 매트랩은 과학기술 분야
      에서 널리 유용하게 쓰이고 있다. 또한 매트랩에는 많은 함수들이 기능별로 묶여 있는 툴 박스
      (ToolBox）들이 존재하는데, 여기에 있는 함수（.1ll 파일）를 활용하면 간단하고 쉽게 원하는 프로그
      래밍 결과를 얻을 수 있다. 툴 박스는 지속적으로 확장, 업그레이드가 되고 있다. 문자끼리의 계산
      을 가능하게 해주는 심볼 처리 툴 박스도 있다. 매트랩은 그래픽 기능이 우수하기 때문에 데이터의
      시각화 측면에서도 유용하며 , GUI 기능이 추가되어 임의의 사용자 인터페이스를 설계할 수 있고
      '] 를 통해 " 11트랩 함수를 실행시키고 그 결고屠 확인할 수 있다· ,,




Fuzzy & Ev이U如na四          難r                                     1

   Computing Pro아am曲ng
                           ,1 매트랩의 특징


·기본 데이터 요소는 차원의 제한이 없는 배열을 사용．
·벡터와 행렬 중심으로 프로그래밍．
·과학기술 분야 문제해결을 위한 다양한 툴 박스（tooll兀x）를 제공．
      Financing
      Communication

      Contr아

      I入izzy Logic

      Image Processing

    - Neural Network

      Optimization

      Power System

    - Signal Processing

    - Statistics


===== PAGE 163 =====
164    [   퍼지, 진화컴퓨팅 프로그래밍                         ]



      ·외부 프로그램（C, Fortran 등） 및 액셀과 링크해서 사용할 수 있음．




  1) 매트랩의 실행 방법

      윈도우의 매트랩 아이콘을 클릭하면 매트랩 6.x에서는 매트랩 실행 화면이, 매트랩 5.x에서
  는 실행 창이 만들어진다．


      (1 ) 실행 화면
      매트랩 6.x에서는 실행 화면어］ 실행 창, 워크스페이스, 경로설정기 창이 함께 만들어진다
  （그림1). 반면에 매트랩 5.x에서는 명령 실행 창만이 만들어진다（그림 2). 그림 1과 2에는
  File, Edit, View, Windows, H이p와 같은 메뉴가 있다. File 메뉴는 파일（함수, 그림 및 시뮬
  링크 관련 파일）과 워크스페이스에 태한 조작（열고, 닫고, 저장）을 위한 메뉴를 갖는다．


               『尸立 卜tAr匕／1日                                                                                        Nm口
                E陀     丘d茫    냄B나    We      뾰indow        닌HID

                [> 多              ！身孕 ,      (    碎      ?    Oma났야岫yr      C:I너yD四ornery針면구개亡m帥的中Stern
                                                                                                    ci娜Y굿내的on크 I
                                                                                                                            'C
                     寸MATLAS
                                                                       To get 針a,ted. select MATLA日 H이p" 什om the He巾 men나
                 f   小Commu毗枷os Toolbox
                 r   寸L Con甘미 System Toolbox
                 ,   寸Data Acqu引t向o To이box
                 +   小 Database Toolbox
                 +   小Dalafeed Too由ox
                 .   小Fillet De引go To미t山0
                 ,   寸L帥anc洽I Derivatives Tooll山X
                     小 Financial Time Series Toolbon
                     4印anc回 To이t山0
                     41 Fuzzy Logic Toolbox
                     寸IDA吼H To미L山X
                     dA rn口n口 口m尸口口+in+ Tn,rIhfl..
                          Lauscy Pad    wo,kxpace



                IC咐My D吼umentsW면구：JL크 匡그 e于 4自
                 朋斗as            小                     f消a 了 pe
                口cxc                                   Folder
                二jescGFCS                              F이der
                丘.4650日ULES                            F이den
               ；교escTFCS                               F이den
                ;i 口Id_glass                           F이den
               U固山如ting_tclass呵ng上治怡.m                 M-tile
                [i4 glass, dat
                Ill 미a＄帥ames




                                                                  =j
                          Command H1stor,+       Durrvnt Di,eotnry




                                             ［그림 1(a)] 매트랩 6.x의 실행 화면


===== PAGE 164 =====
                                                                                                       부록. Matlab 사용법   ]   165



       已) M.凸．TLAB                                                                                           目回口
       탸e         Ed比       냄ew        Web       fldow    bela
       ［그 多             ,     多牙口                        ? Carrsre r出啣卜 eevcon呻Sen／껸구개빔切sea印帥O
                                                                                             『m거ensue叱1玗늬 I
       驢：
        竄解蠱蕪難娜
        畔 日          芝麥       3 Sen出 1                                             ) ) an드 =
                                                                                     172 叩00   0 田37




       冬：므 三218 菲＄eoarr
       圈d
                    ann
                     三！                lxi                  B double array
       圈data_train                     214x10          1 7120 double array
       回fnamel                         lob                 10 char array

       歐" "                            咎                   ’喆，:.;：『
                                                                 『：誌
                   Lau,tch Pad           小／ark＄口ate
       C&]n , 4 0,rtslory                                                口口
         -7朴加DjLUrnenL3咐권구개달附lila引at，二J 山-I                       匡그 寸        J色


             glass_6_r6.cls
       ［그 이as乞已mC旭
       ［그 이as工丘思C怡
                                                                       業：;
                                                                       03日＝
       ［그 이as乞丘eC由                                                     03円1
       0. glass_ab.cls                                                 22日已
                                                                       凸n 口
       國 미ass上乳In

       ［그 미a的上訂J키rl, cljt                                              2＋小二
       固미ass小呵四．m                                     阡川e              22出｛



                                                                             ?
       固이as丘毗떼es,m                                    M寸ile            22-8-2
       [, j 이ass느norm dat                                              22七i
            result_aoalysls_ m    6.
                                                      M- file           "



        (1    和    Corrirnand卜4冶t口싸             Curs日St［汭rest口싸                                                l t
                                                                                                                "




       Ready


                                                ［그림 1(b)] 매트랩 6.x의 실행화면



 그림 2는 매트랩 5.x의 명령 실행 창에 있는 툴 바의 기능을 설명하고 있다. 매트랩 언어로
작성된 파일（.1ll 파일）을 열기 위해 그림 3에서 "New 八4 File" 아이콘을 클릭하면 그림 우측
에 보인 것처럼 m 파일 에디터가 열린다. 경로 설정을 위해서는 그림1의 파일 탐색기나 그림
4의 경로 설정기（Path Browser）를 이용하여 파일 경로를 설정할 수 있다. 그림 5는 시뮬링
크에서 새로운 파일을 오픈하는 경우를 나타닌仁｝.


===== PAGE 165 =====
四 ［ 퍼지 진화컴퓨팅프로그래밍 ，                                                        ］水
             3 I.i3T1 尸BC口mm arid 1／비ridow
             File      툐d卄     노to出 볜ndo놔 He巾                                                                                  Simulink Library        Browser

                                                                                                                                                   1
                                                                                                                                                 Pa 亡力 Browser
                       뚜：                       ：業 on, tipe tour or ulsit www.matllworks.com.
                                     二t
                                          Oil, t             ，山，        如，,.．如恥，如的加r-                                  n   .                卜
               ToF。r         : std 'uc    infer

                                                                                                                                 卜   Workspace Browser



                                                                                                                                                口ndo (C亡rl+Z)



                                                                                                                                                二fd
               adB                                                                                                                   Mi爪4         戶．



              V                                                                                                                                    V
                                                                                          'V
     New m file                           Open File                             C口亡 (C亡rl+X)                  Copy (Ctrl+ C)      Paste (Ctrl+ V)


                                            ［그림 2] 매트랩 5.x 명령 실행창
                                                                （（兀mmand Window)




            TL 日B : :rrirri,크nd 州Iii小：r町                                  N1ATLtB Editot!['日bugg므r- [Ijiti川edli                                            -l口i川
                                                                                                        1}ebug 工00怡 毖odo나 姓eIp                             -I酊즈J

                                                                                                              昌孕 1 囹同
                                                                        儺｝ d코 표i노 多甘                g1如k
            n, t      < t]   .=Fnd        t11n口     nnn 끼1         n1
                                                                   V1    니구     HH   니H        m1    ! m 미尸
            = = 1     =1 1 U " 1 느 H !    1) 1戶 느   끼＝ " 1

      For ! oduct inforuiiation, typ1




                                                                                Se亡／Clear                Break口oint              Clear 月11 Break下)Oiflt




    Ready


                                                                        只eady                                                           r[j4可F如艸m                戶

                                          ［그림 3] 매트랩 5.x에서 새로운 n} 파일 만들7但｝ 에디터


===== PAGE 166 =====
                                                                                                                        부록． Matlab사용법                       ]   167



莎 MATL月E Comm羽'1 쌔nd口小／                                                                        ！區口

瑟 ' "已弩“ 旨
         "：
          日. ,
    To get started, type one of these: helpuin, helpdesk, or demo.
                                                                                                           ,
    For product information, 四pe tour or vi亡1卜 니니니 m;i卜hUnrk亡 尸11m

                                    亨
                                                                          폴더 찾아보기                                                                  日口
U
         畔 Path Bran作er
                                                                            Current Path
         E沁        丘［카t   毖ew       Eath    Ia이S     He10

         늬 크최 星J                                                                               二 니

                                                                                                    =1 d
                                                                                                           m貳陋b
                                                                                                               현：卜잠치 최 적 설 계 화
                                                                                                                                               1
          Cu'rent
                                                                                                            口 이ustering
          F:       크＜二＞
                      「 i: 1】
                            」                             包丙g可ii.-                                      二j data an톄y틔S
          Pa出                                                                                   r    ,+ U nnet
                                                                     小                                 口 nnetl
J上             : : mM댜m山그：끄mX\rn日t-1-出그＼口p日                                                            ：그 ootimize
               : : \l吐kTLA0＼七0口ii그口x\rn日七I日l少1J.ong
               C:＼卜tATLAB\ t七口lb口x\ma七노B '忙끄na七
                                                                                                  下 ;J 巳vent_口redict
               C: \MATI小a\ t；叩Ibox\ ma七I日니 sHun                                                  壬 나 evoo
               C:＼卜WiLAB＼七0口lb口x\metl日B\ specfun                                                 ;＋二J 口attern class                                -J
               亡 : 나8AiLAB\ t；叩lbox\ one七I日늬m毗fun                                              느 二J oattern recogn川on
               C: \MATLAB\ 七口口Lbox\mm七I日b\ da七air Un
                                                                                                    口 이ustering
                                                                                                                                                   크
               C: \MATLAB＼七0口lb口x\ ina七I日b\ polyfun
               C: \MA吼AB＼七oolbox\ma七I日b\ funf on                                                  + 二J event D redictic나1
               C:＼川ATLAB＼七（nol上）（그x\rna亡lab\呂parfun
               C :\MuTLAB\ too.thox\rnmtlab\ graph2d
               C: \MITLAB\ tooJ.box\ rnmtLab\ graph3d
               C: \MATLAB\ too.thox\rnmtlab\ specgraph
                                                                                                                        확인                 취소           1
               C: \F吐&TLAB\ t；口口lb口x\ma七Iab\ graphi口呂
                                                                              國 abs七sp 1a
               C:＼卜PATLAB＼七oolbox\ ma七Iab\ ulto口I日
               C: \MATLAB\ tooth口o\n,a七Lab\ 呂卜．rfun                           因 rib日七口p 1.o
               : : 나IATLAB\ 七凸0] 口0nna亡 I크b\ l口fun                            國 rib七ype. Th
               4                                                              圓 rib up . to

         Ready                                                                                  7:15 PM


                          ［그림 4] 매트랩 5.x에서 경로설정과 파일 탐색을 위한 경로 설정기



已多 MAIl.明 con5ita川 州nd叫／
恥 트a rP叫 對ado.              帥
 二多                 恥      酊8
                                                 n 帥tnuliok
    10 get started, type one 0
                                             手. 只 comniunicario
    For product ynfornation, type tot         +, 只 Cant: 0Pen the 'Slrniulink' L巾rary
                                                   Dials
                                                 堪 DSP 텨ockoet
                                                 珽 日ned-Point Clock＄叭
                                                 舞 Fu2zy Lx吼 Toolbox
                                                  =NCD Blockoet

                                                                                           [=.} untitled
F陀        Ed作      Yow    Fotmat                                                                    툐dii       le나   lm미帥so   Formal 珏이5
                                                                                                    畔 日 旬二               葦"          亨     菰   H

    望，   「     「


                                        0匡trot.    Math     Fund口n Noni,flhl  S口na注
    읖aye                  CleluS                            & Tibits         & Sontnms
    Sane 全S山
                                         uiink Bin出 L山:a030
    ！如d이 Prope川89                       090.1的8 by Thn Math놔0帖．inn

    므riot．口               Ct.i. P
    Ptinter Se竝p..
                                                                                           1 100%
    C嫌卜PATLAC             Cteln(그



                    ［그림 5] 매트랩 5.x에서 시뮬링크怜imulink) 실행을 위한 새로운 파일 열기


===== PAGE 167 =====
168      퍼지, 진화컴퓨팅 프로그래밍



      (2) 작업 환경 설정
      매트랩 윈도에서 매트랩 프로그램을 실행하려면 해당 파일이 경로 설정기의 현재 디렉토리
  (current directory）에 있어야 한다. 그렇지 않으면 경로 설정기를 이용 해당 파일에 대한 경
  로를 현재 디렉토리에 추가해야 한다. 명령 실행 창에서 경로 설정을 위해서는 다음과 같은
  명령을 사용해야 한다．
      · pwd : 매트랩이 현재 어떤 디렉토리를 가리키는지 알고 싶을 때 사용．
      · cd : 작업 디렉토리를 변경하고자 할 때 사용．
      · dir : 현재 디렉토리에 있는 파일을 보고자 할 때 사용．




  2) 매트랩 명령어
      (] ) 기본적인 계산 방법
      매트랩은 인터프리터 언어이므로 명령 실행 창에서 변수를 선언하고 이를 이용하여 수식을
  치고 리턴 키를 치면 수식 계산 결과가 화면에 보인다. 수식 기호 또는 숫자 사이의 공란은
  계산 결과에 영향을 주지 않으며 , 계산 결과를 가질 변수를 지정하지 않으면 디폴트로 ' ans'
  가 변수로 지정되어 답이 저장되며, 한 줄어］ 여러 개의 수식을 실행할 수 있다．


      예） x=10, y= 20, 2半x + y回
         -.x=        10
             y=      20
             ans=         40


      명령문 뒤어］；를 붙이면 화면에 변수 값이 나타나지 않는다. 컴마 대신；를 사용해서 필요한
  변수 값만을 표시 할 수 있다. 위의 결과를 다시 실행해 보자．


      예） x=10; y= 20; 2뇨 + y回
         -   ans =        40


      수식을 실행하는 순서는 괄호 안이 우선적으로 계산되며, 제곱 계산, 곱셈과 나눗셈, 뺄셈
  과 덧셈 순이며 왼쪽에서 오른쪽으로 진행된다. 매트랩에서 사용한 모든 변수는 작업 영역


===== PAGE 168 =====
                                               부록. Matlab 사용법    169



佃orkspace）어］ 저장되며, 작업 영역을 파일로 저장하였다가 나중에 이를 복구할 수도 있다
(File>Save Workspace as 메뉴）. 매트랩은 대소문자를 구분하기（case sensitive) 때문에 x
와 x는 다른 변수이다．


(2) 프로그래밍 작업
 매트랩에서 프로그래밍은 두 가지가 있는데 하나는 앞에서 설명한 것처럼 명령 실행 창어］
서 명령문을 순차적으로 작성, 실행하는 것이고 다른 하나는 파일（파일명 .m)을 이용하는 것
이다. 첫 번째 방법은 간단한 프로그래밍을 작성할 때나 파일에 프로그래밍을 작성하는 과정
에서 부분적인 프로그램의 실행 및 검증이 필요할 때 주로 사용되며, 통상은 파일로 프로그래
밍 한다. 파일은 매트랩의 텍스트 에디터를 이용하여 작성되며（그림 3), 매트랩 에디터 대신
다른 아스키 텍스트 에디터를 사용해도 된다. 먼저 , 파일을 저장하고 실행하는 디렉토리를
현재 디렉토리어］ 지정하기 위해 매트랩의 경로 설정기를 이용하여 해당 경로를 추가한다
(Add to path 버튼과 save settings 버튼 이용）. 이렇게 추가된 디렉토리와 기존의 현재 디
렉토리K뇨rrent i:万rectoi了）어］ 존재하는 모든 디렉토리내의 매트랩 파일들이 서로 연계되어
사용될 수 있다. 매트랩 파일을 실행했는데 실행이 되지 않으면 경로 설정 창을 이용하여 해
당 파일의 디렉토리를 현재 디렉토리m出rent Direct아y）에 추가해야 한다．


(3) 키보드에서 명령에 조작
 키보드에서 명령에 조작을 편리하게 하기 위해 다음과 같은 명령어를 사용한다．
 .Ins : 명령문을 입력할 때 삽입／수정 모드의 전환．
 ·De1 : 커서 있던 자리의 글자를 지울 때 사용．
 ·Esc : 현재 행에 입력된 키보드 문자를 모두 무시할 때 사용．
 ·介／寸／ : 이전／이후어］ 입력한 실행 명령어들을 하나씩 열람할 때 사용．


(4) 변수 상태 점검
 현재 작업 영역(Workspace）에서 사용 중인 변수들은 작업 영역에 저장되며 , 변수명을 명
령 실행 창에 입력하고 리턴을 치면 해당 변수의 값이 화면에 출력된다. 작업 영역에 현재
저장된 변수를 파악하기 위해서 다음과 같은 명령어를 사용한다．
 · who : 이 명령은 작업 영역에 존재하는 변수를 보고자 할 때 사용．
 · whos : 이 명령은 변수의 크기 , 바이트 수 등의 정보를 알고자 할 때 人卜용．


===== PAGE 169 =====
170      퍼지, 진화컴퓨팅 프로그래밍



      예） who回
         -   Your variables are:
             ans       x           y


      예） whos回
         -   Name      Size            Bytes Class
             ans       lxi                8 double array
             x        lxi                 8 double array
             y        lxi                 8 double array
             Grand total is 3 elements using 24 bytes


      변수와 관련하여 다음의 명령도 자주 사용된다．
      ·c1ear : 작업 영역에 존재하는 모든 변수를 삭제할 때 사용．
      ·c1c : 변수어］ 영향을 주지 않고 명령 실행 창 화면에 표시된 내용을 지울 때 사용．


      (5) 출력 형식 지정
      format이라는 명령을 이용하여 화면에 표시되는 수치의 형식을 제어할 수 있다. 이는 데이
  터의 표시 양식만을 바꿀 뿐이며 계산의 정밀도와는 관계가 없다. 계산은 double 형으로 처
  리된다. 표시 형식 디폴트는 short와 동일하다．

  ·format short : 5（소수점 포함）자리의 고정 소수점 표시．
  ·format long : 15（소수점 포함）자리의 고정 소수점 표시．
  ·format short e : 5（소수점 포함）자리의 부동 소수점 표시．
  ·format long e : 15（소수점 포함）자리의 부동 소수점 표시．
  ·format short g : 5자리 고정 또는 부동 소수점 가운데 적합한 것으로 표시．
  ·format long g : 15자리 고정 또는 부동 소수점 가운데 적합한 것으로 표시．
  ·format hex : 16진수로 표시．
  ·format rat : 분수로 표시．
  ·format compact : 표시 데이터의 줄과 줄 사이에 빈 줄이 없음．
  ·format loose : 줄과 줄 사이에 여분의 빈 줄이 삽입됨．


===== PAGE 170 =====
                                                       부록. Matlab 사용법   J1日＝


(6) 데이터 저장과 읽기
 변수의 내용을 저장하기 위해 save 명령을 사용할 수 있다. 명령 실행 창에서 save를 치면
작업 영역의 모든 변수를 디폴트 파일명인 matlab.mat에 저장한다. 변수 x의 내용을 아스키
형태로 파일명 datafile.dat로 저장하기 위한 명령은 save datafile.dat x -ascii이다．


 예) a=[1 2 3]; b=[4 5 6]; x=[a; b], save sample.t砒 x 小ascii目
    -   x=    1     2        3
               4     5       6
    sample.t玭 파일어］ 변수 x의 데이터가 다음과 같이 저장된다．
        1.0000000e+000 2.0000000e+000 3.0000000e+000
        4.0000000e+000 5.0000000e+000 6.0000000e+000


 변수 뎨이터의 저장 형식을 행 단위로 지정하여 한 열씩 저장하기 위해서는 fprintf 명령을
사용한다. 이 때 주의할 것은 fprintf는 데이터를 열 단위로 저장한다는 것이다. 따라서 x의
행렬 형태 그대로 데이터를 저장하기 위해서는 전치시켜야 한다．
 다음 예는 데이터 변수 x의 전치 x'를 파일 sample2.奴t어］ 저장하기 위한 것으로, x'의 행이
3개이므로 fprintf안어］ 해당 행의 형식을 지정할 수 있다. 이 경우 파일의 열고, 닫기를 실행
해야 하며 fprintf는 변수 x' 의 데이터를 열 단위로 읽어 저장한다. fprintf에서 \n는 개행 문
자로 줄바꾸기를 한다. %3.lf은 변수 값은 3자로 적되 소수점 이하를 1자리로 표시하도록
지정한다. f는 실수, d는 정수, e는 지수를 나타낸다．


 예) a= [123];b= [456];x= [a; b];回
    fid = fopen('samp1e2.txt','w')；回
    fprintf(fid,'%3d %3.lf       %3.1e\n',x');回
    fclose(fid)；回
    -   sami月e2.奴t 파일어］ x의 데이터가 다음과 같이 저장된다．
        1 2.0 3.0e+000
        4 5.0 6.0e+000


 그림 파일을 저장할 때는 그림 창 메뉴 File의 하위H메뉴인 Save와 Save As를 이용하고


===== PAGE 171 =====
11m[    퍼지, 진화컴퓨팅 프로그래밍



  다른 응용 立로그램에 덧붙일 목적으로 복사할 때는 Edit 메뉴의 하위小메뉴인 Copy를 이용
  한다．
   파일 데이터를 읽기 위한 명령어로 load가 있다. 가령 , datafile.dat라는 파일이 있다고 하
  면, load datafile.dat라는 명령문은 datafile.dat 파일의 내용을 datafile라는 변수에 행렬
  로 읽어온다. load datafile.dat의 출력 변수를 지정하지 않으면 파일명（. 이하 제외）어］ 해당
  하는 변수가 자동으로 만들어진다．


   예） load sam하e.t砒日
        san叩扼目
        -sample =            1           2           3
                             4           5           6
        출력변수를 지정하지 않으면 파일 이름의 변수가 자동으로 생성된다．
        data = loadCsample.txt')回
        -   data =     1         2           3
                         4       5           6


  fscanf를 이용하여 데이터 파일을 읽을 수도 있는데 다음의 예를 보자．


   예) fid = fopen('samp1e2.txt','r');回
        data2 = fscanf(fid,'%g %g %g',[3 i沚])回
        fclose(fid上日
        尸＋ data2 =       1       4
                         2       5
                         3       6
        data2 = data2'
        -   data2=       1           2           3
                         4           5           6
        [3 inf］는 데이터를 읽어 들일 크기를 정하는 것으로 data2어］ 처장할 때는 행과 열을
        바꾸어 저장되기 때문어］ 파일어］ 저장된 형태를 유지하기 위해서는 읽은 데이터 행렬을
        전치시켜야 한다．


===== PAGE 172 =====
                                                        부록. Matlab 사용법   J1尿＝


(7) 도움말 이용
 매트랩 조작법과 내장 함수의 사용법을 익히는뎨 도움을 주기 위해 다음과 같은 명령어를
사용할 수 있다．

·he1p 'xyx' : 'xy才으로 된 매트랩 함수나 연산자를 찾아준다．
100kfor 'xyz' : 매트랩 함수의 첫 helj) 실행 문에서 ' xyz꾀 문자열을 갖는 함수를 찾아준
 다．
 heli) 명령어는 함수나 연산자의 사용법을 모를 경우에 helj) 다음어］ 사용법을 알고 싶은 함
수명이나 연산자를 입력하고 리턴 키를 치면 해당 사용법을 알 수 있다. 그냥 help만 치면
모든 명령어들이 화면에 표시된다. 예를 들어 sin이란 명령어（함수명）을 알고 있지만, 그 사
용법을 모를 경우 다음과 같이 helj) 명령어를 사용할 수 있다．


 예） he如 sin回
      -   SIN    Sine.
      H   SIN(X) is the sine of the elements of X.


loofkor ' X)皿'를 사용하면 m와 관련이 있는 모든 함수들을 찾아준다．


 예） lookfor sin回
      H+ SUBSI寸DEX Subscript index.
      -   ISINF True for infinite elements.
          ACOS    Inverse cosine.
          ACOSH Inverse hyperbolic cosine.
          GSVD    Generalized Singular Value Decompostion.
          SVD    Singular value decomposition.
      sin이란 문자열을 포함하는 모든 함수를 찾아 표시하며, 위에 표시한 것은 전체 결과
      가운데 일부임．


(8) 화면 출력
 문자열이나 벡터 , 행렬의 데이터를 화면에 표시할 때 disp라는 명령어를 사용한다, 변수 x


===== PAGE 173 =====
1區기   퍼지, 진화컴퓨팅 프로그래밍



 의 데이터를 표시하기 위하1disp（功를 치면 변수 x 없이 x의 내용만을 표시한다．


  예） x = 1:0.5:2；回
      disr巾c)回
      -   1.0000       1.5000       2.0000


      fprintf는 변수를 특정한 형식으로 표시할 때 사용한다. 다음의 예를 보자．


  예） x = 1:0.5:2；回
      如ri砒川%3.lf           %4.2f   % 4.2e',x）回
      H 1.0 1.50            2.00e+000?




 3) 매트랍1 기초

  (1 ) 일반 기호
  매트랩은 다양한 기호들을 여러 가지 용도로 사용하고 있는데, 주요 기호들의 기능은 다음
 과 같다．

 ·［ ] : 벡터나 행렬을 표시할 때 사용, 원소를 공란으로 분리하면서 벡터나 행렬의 원소를
  넣는다．
  예） x = [1 2 3; 4 5 6］回
          x=       1         2      3
                   4         5      6

 ·（ ) : 벡터 , 행렬 또는 다항식의 원소를 지정할 때 사용．
  예） x(2,3）回
      -   ans =        6
      x(2,3) =     1回
      -x=          1         2     3
                   4         5     -1


===== PAGE 174 =====
                                                                      부록. Matlab 사용법



·9b : 주석을 달 때 사용．


' : 벡터나 행렬을 전치시킬 때 사용．
 예） x = [1 2 3; 4 5 6］回
     x'回
     H+ ans =        1        4
                     2        5
                     3       -1

 "       : 문자열을 표시할 때 사용．
 예） x = '123h]jkkf'回
     H x =      123h]jkkf

... : 프로그램이 길어 여러 줄어］ 나누어 써야 할 때 이 기호를 사용. 줄 끝어］ 이 기호를
 붙이면 다음 줄과 연결되어 있음을 나타냄．
 예） x= [1 2 3 ...回
     45］回
     -    x =    1        2          3      4       5

.. : 벡터나 행렬에서는 행을 끝을 나타내며 수식 뒤에서는 결과 값을 화면에 표시하지 않도
 록 한다．
 예） x = [1 2; 3 4; 5 6］므


                 3       4
                 5       6
     x= [12; 34; 561; y= x(1,1)回
     -.y=        1
     x에 대한 결과를 표시하지 않음．

·：：벡터를 만들 때 사용．
 예） x =     1:0.5:1回
         x =    -1.0000           -0.5000       0       0.5000   1.0000


===== PAGE 175 =====
         퍼지, 진화컴퓨팅 프로그래밍



       -1에서 0.5씩 증가시키며 1까지의 행 벡터를 만든다. 중간 숫자를 제거하면 디폴트로
       1씩 증가한다. 즉, 1씩 증가하는 경우 x = -10:1:10을 줄여서 x = -10:10으로 쓸 수
       있다．
        x = -1:1回
                    1    0     1

· . : 이 점은 벡터나 행렬에서 원소끼리 계산할 때 사용．
     예） x= [1 2:3 4]; y = x. 米x, z = 냔x回
        -   y=      1    4
                  9     16
            z=      7   10
                 15     22


     (2) 수식 기호
     덧셈과 뺄셈을 제외한 행렬 및 벡터의 원소끼리의 연산에는 반드시 " ."을 넣어야 한다（.求
./ .쏘｝같이）. 점을 붙이지 않으면 이는 행렬 연산의 곱과 나누기를 의미한다. 벡터나 행렬의
덧셈과 뺄셈은 원소끼리의 계산이므로 " ."을 붙일 필요가 없다. 나누기에서 a/b는 b로 a를
나누는 것이지만, 小b는 a로 b를 나누는 것을 의미한다．
1+
      ：덧셈
      ：뺄셈
.*
     ：곱셈
·／ : 나눗셈
·八 : 지수

     예） a 벡터어］ 스칼라 5를 더하며
        b = a + 5回
        -   b=      6    7     8    9      10


     예） 벡터 a와 b를 더하면
        C = a + b回
        -= C=       7    9    11   13      15


===== PAGE 176 =====
                                   부록. Matlab 사용법   口m

예） 행렬 a의 제곱
    C = a"2回
    H+   C   =   30    36    42
                 66    81    96
                 102   126   150
    위의 결과는 c = a*a를 실행한 것과 같다．


예） 행렬 a의 원소를 제곱
    d = a. 八2目
    -    d=       1     4     9
                 16    25    36
                 49    64    81
    이 결과는 d= a.半a를 실행한 것과 같다．


(3) 관계 및 논리 연산자
매트랩은 다음과 같은 관겨］ 연산자를 사용한다．
·（ : 보다 작은
·＞ : 보다 큰
·（= : 보다 작거나 같은
·＞= : 보다 크거나 같은
·＝= : 같은
·N= : 같지 않은


매트랩에서 사용하는 논리 연산자는 다음과 같다．
·＆ : and（논리곱）
·1 : or（논리합）
·N : not(부정）
1xor : exclusive or
·any : 벡터에 0이 아닌 원소가 있으면 참．
·a11 : 벡터의 모든 원소가 0：기 아니면 참．


===== PAGE 177 =====
口m1 퍼지, 진화컴퓨팅 프로그래밍
    예） x = Ill 2 31!; an叭功回
       -   ans =      1
       x = 11 0 0; 2 3 0]; any(x)回
       -   ans =       1     1     0
       x가 행이나 열 벡터이고 벡터 원소에 0이 아닌 원소가 있으면 any는 1을 리턴하며 , x
       가 2개 이상의 행과 열을 가질 때 any는 열 단위로 벡터 원소를 점검하써 결과로 행
       벡터를 리턴한다．


    예） x = [1 1 1]; all(x)回
       -   ans ＝二      1
       x = [11 0; 2 0 0]; all（功回
       -   ans =       1    0     0


    예) x= 10; y= 4; cond= (x> 5& y>=4)回
       -cond=           1


   그 외에 비트 단위 연산자와 집합 연산자가 있다．


   (4) 매트랩의 지정 변수
    매트랩의 다음 변수들은 특정 용도로 지정되어 있다．
   ·i, j : 허수 V二i
   ·NaN : 숫자가 아님（Not a Number)
   .Inf : 무한대 이그
   .pi : 원주율 兀
   ·ans : 임시로 답을 보관하는 변수
   ·Z= a + bi : 복소수（a와 b는 실수） 표시 , 1대신 J를 사용해도 됨．
   ·rea1(기 : 복소수 z의 실수 값
   ·imag(z) : 복소수 z의 히수 값
    예） z = 1 + 2i回
       -   z =      1.0000 + 2.0000i


===== PAGE 178 =====
                                       부록. Matlab 사용법   179



    z = 1 + 2iE크
   Hz =           1.0000 + 2.0000i
    [real(기 imag(z刀回
   -       ans=       1     2


(5) 수식의 표현
매트랩은 수식을 표현하는데 사용될 함수를 내장하고 있으며 , 이들 함수의 입력 x는 상수나
벡터일 수 있다. 삼각함수의 경우 입력 x는 각도가 아닌 라디안 값을 사용해야 한다．

·abs（功 : x의 절대값을 리턴
·acos（功 : x의 아크 코사인 값을 리턴
·asi可功 : x의 아크 사인 값을 리턴
·atam功 : x의 아크 탄젠트 값을 리턴
.coI承功 : 복소수 x의 공액 복소수를 리턴
.cos（功 : x의 코사인 값을 리턴
·exp（功 : x의 지수함수 값을 리턴
 log（幻 : x의 자연 로그 값을 리턴
 logl0（功 : x의 상용 로그 값을 리턴
·round（功 : x어］ 가장 가까운 정수로 반올림 함．
·floor（功 : 음의 방향으로 x에 가장 가까운 정수로 만듦．
·ceil(功 : 양의 방향으로 x어］ 가장 가까운 정수로 만듦．
·fIM功 : 0의 방향으로 x어］ 가장 가까운 정수로 만듦．
·sqrt（幻 : x의 제곱근 값을 리턴
·tan（功 : x의 탄젠트 값을 리턴


 fl) [round(0.4) round(0.5)]日
   -ans=              0   1
       ceil(0.4）回
       -   ans=       1
       floor(0.6）回


===== PAGE 179 =====
180         퍼지, 진화컴퓨팅 프로그래밍



                m+ ans =          0
                [fix(0.6) fix（山.6)］回
                -    ans =        0        0



      예） 다음 수식의 값을 계산해 보자. x = 2, y = 1, z = 寸 (0.5 尸x) + e' 'sin (y)
        x = 2; y = 1; z = x八2米（0.千x) + exp(x"功노in(y）回
        -           z =   0.2177
        이 경우어］ x가 벡터나 행렬이면 z를 계산할 때 .을 사용해야 한다．
        x = [2 4; 3 5]; y = 1; z = x."2.*(0.5_x) + exp(x.八y).*sin(y)回
        -           z =   0.2177 -10.0572
                          5.5986          12.3854
      sqrt（功는 x."0.5와 동일한 계산 결과를 보이며 sqrtr可功는 x"0.5와 동일하다．


      예） x=[1 2; 3 4]；回
            sqrt（功回
            -       ans 二＝       1.0000        1.4142
                                 1.7321        2.0000
            sqrtn山()回
            Hans =           0.5537 + 0.4644i           0.8070 - 0.2124i
                             1.2104 - 0.3186i           1.7641 + 0.1458i


      (6) 벡터의 계산
      벡터는 [ ] 안에 원소를 빈 공간이나 콤마로 구분하여 입력하며 , [ ] 안어］ 수식이나 벡터가
  원소로 들어갈 수 있다．


      예） x = [ 123］回
        -x=                  1        2        3
        x = [1,2,3］回
        -.x=                 1        2        3


===== PAGE 180 =====
                                                            부록. Matlab 사용법   口國1

 예) x = [123]; y=[xx], z = [x;xI1回
    -   y=      1        2     3      1       2    3
        z   =   1        2     3
                1        2     3


 예） x = [ 1 2 3]；回
        x = [ sqrt（功 01］回
    1+ x =      1.0000       1.4142       1.7321       0   1.0000


벡터의 일부만을 꺼내 사용할 수도 있고 일부분의 값을 대체할 수도 있다. 다음 예를 보자．


 예) x= [123] ;y= [4561; z= y(1:2),w= x(2:3)'
    -z=         4        5
        ＼자 =    2
                3
   ( ）는 벡터의 출력을 나타낸다. a(1）는 a 벡터의 첫 번째 원소를, a(2:5）는 a의 둘째에서
   다섯째까지의 원소 벡터를 나타낸다. 벡터의 특정한 부분을 변경할 때에도 변경 부분을
   ( ）로 지정한다. a(2:4) = [1 2 釗는 a 벡터의 둘째에서 넷째까지의 원소를 [123］으로
   대체한다．


일정한 간격의 값을 갖는 벡터를 만드는 방법은 앞에서 설명하였다. x = a:b:c는 a에서 시작
해서 C까지 b씩 증가하는 행 벡터를 만들어준다. 매트랩에는 이와 같은 기능을 수행하는 명령
어로 血빠冶ce와 logspace가 있는데 이들의 사용법은 다음과 같다. logspace는 로그 값의
벡터를 만들어준다．

·linspace（시작 값, 종료 값, 원소 개수） : 시작 값에서 종료 값까지 원소 개수만큼의 행 벡터
 를 만듦．
logspace（시작 값, 종료 값, 원소 개수）: 10八' ］작 값에서 10八종료 값까지 원소 개수만큼의 행
 벡터를 만듦．


===== PAGE 181 =====
口m    퍼지, 진화컴퓨팅 프로그래밍



  예） x = 1:2:11을 linspace로 표현하면
     y = linspace(1,11,7); % 1에서 11까지 7개의 원소를 갖는 행 벡터
     z = logspace(1,2,5); % 101에서 1了까지 5개의 원소를 갖는 행 벡터


 벡터 계산에서 주의해야 할 점은 벡터의 차원［행의 수><열의 수］이다. 덧셈과 뺄셈의 경우 벡
 터의 차원이 통일해야 하며 , 벡터의 곱셈에서는 두 벡터의 차원이 전치 관계어］ 있어야 한다．
 즉, yb에서 a 벡터의 행의 수는 b 벡터의 열의 수와 같고 a 벡터의 열의 수는 b 벡터의 행의
 수와 같아야 한다. 벡터의 원소끼리의 곱하기와 나누기의 경우에는 덧셈과 뺄셈에서와 같이
 두 벡터의 차원이 동일해야 한다．


  예) x =[2916];yzz [234]; z= x+ y回
     -     z=       4    12      20
     x =[2916];y =[234] ; z= x- y回
     -z        ＝二   0    6       12
     x= [2916];y= [234]; z= x*y', w= x.*y回
     -     z=       95
           w=       4    27      64
     x= [2916];y= [234]; z =x.Iy, w =x.\y回
           z=       1        3     4
           w =      1.0000       0.3333   0.2500


 (7) 행렬의 연산
  매트랩에서 벡터의 동작 원리가 행렬에도 그대로 적용된다. 행렬의 일부만을 꺼내 사용할
 수도 있고 일부분의 값을 대체할 수도 있다. 다음 예를 보자．


  예) x = [1 23]; y = [456; 789]; z = y(l:2, :), w = [x(1:2); z'], q = y(:,2)回
     =H呼   z   =    4        5     6
                    7     8       9
           w        1     2
                    4     7


===== PAGE 182 =====
                                                        부록. Matlab 사용법



                 5      8
                 6      9
         q=      5
                 8
    z는 y의 첫 행과 둘째 행의 모든 데이터를 갖는다. x(1:2）는 x의 첫째와 둘째 원소를
    나타내며, q는 y의 둘째 열 데이터를 가진다. ( ）는 행렬의 출력을 나타낸다. a(1,1）은
    a 벡터의 첫 행 첫 열의 원소를, a(2,2:5）는 a의 둘째 행에서 둘째 열에서 다섯째 열까
    지의 원소 벡터를 나타낸다. 행렬의 특정한 부분을 변경할 때에도 변경 부분을 ( ）로
    지정한다. a(3,:) = [1 2 3］는 a 벡터의 셋째 행 벡터（3행어］ 있는 모든 열의 원소）를
    [1 2 3］으로 대체한다.


a(:,:）는 a의 모튼 행과 열 즉, 행렬 a 자체이다. 숫자 없이 괄호 안에 있는：는 '모든’ 을 의미
한다. 복소 벡터나 복소 행렬의 공액 전치를 구하는 경우에도 기호 " '를 사용한다．


 예） z = [ 1+i 2-2i ]巨꾜
     Hz = [1.0000 + 1.0000i         2.0000 - 2.0000i]
     z'回
     Hans =          1.0000 - 1.0000i
                 2.0000 + 2.0000i


z '에서 보면 행렬의 원소가 공액 복소수로 바뀌었는데, 이를 방지하키 위해서는 conj 명령어
를 사용해야 한다．


 예) z = [1.0000 + 1.0000i       2.0000 - 2.0000i1;
    co'承기回
     -   ans =       1.0000 + 1.0000i
                 2.0000 - 2.0000i


행렬의 덧셈, 뺄셈 및 곱셈은 벡터의 경우와 동일하다. 행렬의 나누기어］ 대하 알아보자. 행렬
식에서 해를 구하는 경우를 보자．


===== PAGE 183 =====
         퍼지, 진화컴퓨팅 프로그래밍



·Ax = b, x = 크＼b 또는 劣 = inv (A ）木 b)
·xA= b, x= A/b

.inv（功 : 행렬 x의 역행렬을 구할 때 사용．


 예） a = [11; 1 -11；回
     inv(a) E크
     -    ans =    0.5000       0.5000
                   0.5000      -0.5000


 예） Ax= b, A= [12; 3 11, b =[0.5; 1] 일 때 해 x를 구하라．
     A = [1 2; 3 1], b = [0.5; 1];回
     x = inv(A少b回
     -    x   =   0.3000
                  0.1000
     x = A伯드크
     -    x =     0.3000
                  0.1000


·eye(n) : 1l행 n열의 단위행렬을 만들 때 사용．
·det : 행렬식（determinant）을 구할 때 사용．


 예） a = eye(3）目
           a=      1       0     0
                   0       1     0
                   0       0     1


 예） b = [ 1 2; 3 4］回
     c = det(a)
     -     c=     1


===== PAGE 184 =====
                                          부록. Matlab 사용법   口:
'size : 행렬의 차원을 구할 때 사용, 티턴 값은 ［행의 수 열의 수］.
·ones(n,m) : 모든 원소가 1인 n행 n열의 행렬홀 만듦．
' zeros(n,m) : 모든 원소가 0인 n행 n열의 행렬을 만듦．
·eig : 행렬의 고유치（ei母ienvalue）를 구할 때 사용．
·dig : 벡터를 행렬의 대각선에 위치시킬 때 사용．
' length : 벡터의 크기（행의 수 또는 열의 수）를 알고자 할 때 사용．


 예) x = [1 2 3; 4 5 6]; dim = size(x)回
      -    dim=         2       3
      y = zeros(dim)回
      H+   y=
                    0       0       0
                    0       0       0
      z = ones(size位力日
  0

      -=z=        1         1       1
                    1       1       1
      w = diag(x(1,:))日
      -.   w =      1       0       0
                    0       2       0
                    0       0       3
      q = x(1,:）回
      -    q=       1       2       3
      size(q）回
      -    ans=         1       3
      length(q）日
      -ans=             3
      size(q'）回
      -=ans=            3       1
      lei培th(q'）回
      -=ans=            3


===== PAGE 185 =====
186   1   퍼지, 진화컴퓨팅 프로그래밍



      sum: 행렬 원소의 합을 구할 때 사용．
      mm : 행렬 원소의 최소값을 구할 때 사용．
      max 행렬 원소의 최대값을 구할 때 사용．
      이 때 열 단위로 계산되어, 그 결과는 열의 수어］ 해당하는 원소를 갖는 행 벡터로 주어진다．


      예) a = [5121; 3642; 237 8];回
          sum(a）回
          -=ans=         10        10       13       11
          sum(sum(a))回
          -+ ans =       44
          sum(sum(a)）는 열단위로 원소들의 합을 계산한 sum(a）의 결과로 생성된 행 벡터에서
          원소들의 합을 계산한다. 즉, 행렬의 모든 원소들의 값을 합한 결과이다．


      [Y, I] = ml可a）에서 Y는 a 행렬의 각 열에서 가장 작은 값의 원소로 이루어진 행벡터이고
  I는 각 열에서 해당 원소의 위치（행 번호）를 나타내는 행벡터이다. sum의 경우처럼 a 행렬의
  행과 열의 수가 모두 2 이상이면 행렬 a의 최소값은 ml可mln(a)）로 구할 수 있다. 최대값을
  구하는 max의 경우도 최소가 아닌 최대값을 찾는 점을 제외하면 mm과 사용법이 동일하다．


      예) a= [5121; 3642; 23 78];
          [Y, I] = mln(a)回
          -Y =       2         1        2        1
          -1=        3         1        1        1
          min(a）回
          -   ans=       2         1        2        1
          II血T1(mln(a)）回
          卞＋ ans =         1
      mln(a）에 출력 변수를 할당하지 않거나 하나만 할당하면 계산 결과는 최소 값의 원소를 갖
  는 행 벡터이다（위에서 출력 변수를 Y와 I . 두 개 할당한 결과에서 Y의 값만을 가짐）


===== PAGE 186 =====
                                                      부록. Matlab 사용법



  J) a= [5121; 3642; 23781;
    [Y, I] = max(a)回
    -'Y=          5       6        7          8
    -' I=         1       2        3          3
    max(a）回
                    5         6        7          8
    max(max(a))回
    -   ans =         8


·mean（功 : x의 평균을 구함．
·std（功 : x의 표준편차를 구함．
·media可功 : x의 대표 값을 계산．
·sort(x): 커지는 크기 순으로 x를 정렬할 때 사용．
·rand(m,n) : 균일분포의 랜덤 숫자를 원소로 갖는 m행 n열의 행렬을 만듦．
·randn(m,n) : 정규분포의 랜덤 숫자를 원소로 갖는 m행 n열의 행렬을 만듦．
.cov : 상호분샌covariance) 행렬을 만들 때 사용．
'rem(x,y) : x를 y로 나눈 나머지를 계산．
mean, std, median, sort 명령은 열 단위로 계산된다．


다음의 예들을 통하1 이들의 사용법을 알아보자．


 예） x = [1      0.1; 2    0.9; 3           0.3I;回
    mean(x）回
    H ans =        2.0000         0.4333
    std（功回
    나 ans =        1.0000         0.4163
    median(x)E크
    -   ans =      2.0000         0.3000
    sort(x）回
    H ans =        1.0000         0.1000


===== PAGE 187 =====
口m[    퍼지, 진화컴퓨팅 프로그래밍



                     2.0000      0.3000
                     3.0000      0.9000
       coy（功回
       -   ans =      1.0000      0.1000
                     0.1000      0.1733
       y = rand(size位力回
       -   y =      0.9501     0.4860
                   0.2311      0.8913
                   0.6068      0.7621
       z = ran面（size(y)）回
       -   z =     -0.4326      0.2877
                   小1.6656     小1.1465
                   0.1253      1.1909


  예） x = 7; y = 3; ren小（,y）回
       -ans =          1


  (7) 문자열의 처리
  문자열 처리를 위한 매트랩 명령어로 다음과 같은 것들이 있다．
  ·str2num( '문자열' ) : 문자열을 숫자로 변환할 때 사용．
  ·int2str（功 : 정수 x를 문자열로 변환할 때 사용．
  ·num2str（功 : 숫자 x를 문자열로 변환할 때 사용．
  ·strcmp(sl,s2) : 문자열 sl과 s2가 동일하면 1, 아니면 0을 리턴．
  ·eval( '문자열' ) : 문자열을 수식이나 문장으로 해석해서 수식이면 그 값을 리턴하고, 문장
      이면 이를 실행한다．
  'exist('的 : S는 변수나 파일명이며 , 해당 변수나 파일이 존재하면 0 이외의 값을 리턴．
  ·feva1C함수명 ' ,x1, ··r, Zn) : '함수명꽤 해당하는 함수어］ 입력 인수 x1, ' ' ' ,2n을 넘겨주며，

      함수를 실행해서 그 결과를 리턴. 출력 변수가 다수인 경우 [Yi, " " , Yrn] = feval('함수명' ,

      x1, ·..,x)와 같이 사용할 수 있다．


===== PAGE 188 =====
                                               부록. Matlab 사용법   i- F匹＝


·x = input( '문자열' ) :미 명령어는 화면어］ '문자열'을 표시하고 키보드로부터 입력을 기다
 린다. 자판을 치면 해당 문자를 받아들여 변수 x어］ 할당한다．


예) n = str2numC3.141592')回
   -   n =       3.1416


예） x = 10.35; s = num2str（功回
   1+ S = '10.35'


예) strcmp('yes','no')回
   -   ans =        0


예) s = '4*a+ai(1)'; pi = eva1(s)回
   H pi =        3.1416


예） for n=1:4回
       eval(['M' int2str(n) ' = magic(n)'])回
   end回
   -Ml       =     1
       M2=         1       3
                   4      2
       M3=         8       1    6
                   3      5    7
                   4      9    2
       M4=        16       2    3   13
                   5      11   10    8
                   9      7    6    12
                   4      14   15    1
   n追gic(n)은 n행 n열의 마술 행렬을 발생시키는 매트랩 함수이다. 마술 행렬은 n의 크
   기가 3 이상일 때 원소의 값이 1에서2
                        n2 범위 내에 있으면서 행과 열의 합이 모두 같은


===== PAGE 189 =====
190          퍼지, 진화컴퓨팅 프로그래밍



         행렬이다. n=4인 경우에 eval 함수의 실행은 매트랩 명령 실행 창에서 M4 = magic(4)
        를 실행시킨 것과 동일하다．


      예） k=O；回
         w址le 1回

              k=k+1;回

              datak = ['data' int2str(k)]回

              filename = [datak '.dat'];回

              if Nexist(fil이追me）回
                      break日

              end回

              eval(['load ' fil아追me])；回

              x = eva1(datak)回
         end回

         -    x   =      1
                         1     2
                         1     2   3
                         4     5   6
         이 예에서 k=1인 경우를 살펴보자. datak 변수는 문자열 'datal'을 저장하고，
         filename 변수는 datal의 문자열 뒤어］ '.dat'라는 문자열을 붙여서 'datal.dat'라는 문
         자열을 갖게 된다. 的dst(filenan始）함수는 현재 설정된 디렉토리에 변수 filenan始이
         갖는 문자열어］ 해당하는 파일이 존재하지 않으면 0을 리턴한다. --exist(filename）는
         해당 파일명이 존재하지 않으면 1이 되어 if 조컨을 만족시키므로 break 명령이 실행
         되어 루프（while N end）를 빠져나온다. 파일이 존재하면 eval 명령이 실행된다（명령
         실행 창에서 load datal.dat를 실행한 것과 동일, 이 명령어］ 의해 자동으로 생성된 변
        수 datal이 datal.dat 파일의 데이터를 저장한다）. 두 번째 eval 명령은 x = datal을
         실행한 것과 같다. 실행 결과는 현재 지정 디렉토리어］ 3개의 파일（datal.dat,
         data2.dat와 data3.dat）이 존재하며 각 파일어］ 다음과 같은 형태로 데이터가 저장되어
         있는 경우를 가정한 것이다.


===== PAGE 190 =====
                                             부록. Matlab 사용법



    datal.dat
    1
    data2.dat
    1      2
    data3.dat
    1      2     3
    4     5      6


 예） x = [1 2; 3 4]；回
    D = ['sui［可功' ; 'min(功' ; 'max(x)']；回
    n = input( ' 계산을 위한 번호를 선택하고 입력： ' )；回
    H 계산을 위한 번호 선택를 선택하고 입력： 1
    eval(D(n,:))回
    -   ans ＝二       4   6
    변수 D에서 문자열 길이（열의 수）는 동일해야 한다. 문자열 길이가 다른 경우에는 가장
    긴 문자열을 기준으로 해서 빈 공란을 삽입해서 문자열 길이를 맞춘다．


 예) x = [1 2; 3 4]; y = feva1('sum',x)回
    -   y=       4       6
    y = fevalCsum',x）은 y = Sm可功을 실행한 것과 동일하다．




4) 그래프 그리기

(1) 2차원 그래프
 그래프는 숫자 데이터를 가시화하써 데이터의 특성을 보다 쉽게 파악할 수 있도록 해준다．
매트랩은 매우 뛰어난 그래픽 및 사용자 인터페이스 기능을 가지고 있는데, 여기서는 2, 3차
원의 그래프를 그리는 방법어］ 대해서만 설명하기로 한다. 그래프를 그리기 위한 가장 기본적
인 명령어로 plot가 있다．


===== PAGE 191 =====
      퍼지, 진화컴퓨팅 프로그래밍



·plot : 이차원 데이터를 그릴 때 사용．
  ]) t = 0:0.5:10; tt = sin(t); p1ot(t,tt,'b+-')回
   변수 t의 데이터를 x축 값, tt를 y축 값으로 그래프를 그린다. b는 선의 색을 지정하는
   것으로 b(blue), c(cyan), k(black), m(magenta), r (red), g(green), w(white),
   y(yellow）의 색을 지정할 수 있다. 선 모양으로                   （실선）, :（점선）, 小（대쉬선）,   .（대쉬
    점선） 등을 지정할 수 있고, 뎨이터 위치를 표시하는 마커로 0, +, 米, x, . 등을 사용할
   수 있다．


명령 실행 창어］ helj) 히毗을 치면 plot과 관련된 세부 내용을 알 수 있다. plo妖t）하면 x축은
데이터 t의 번호, y축은 데이터 t의 값으로 그래프를 그린다．


 예) t = 0:0.5:10; tt = sin(t); z = cos(t);回
    p1ot(t,tt,'ro_ ',t,z,'b*:)回
    하毗은 위의 경우처럼 하나 이상의 곡선을 표시할 수 있다．


히毗을 이용 그림 창어］ 그려진 그래프에 축 이름, 그래프 제목, 문자열, 축의 범위를 표시하는
더］ 다음과 같은 명령어를 사용한다．

xlabel('문자열’) : '문자열' 에 해당하는 x축 이름을 표시．
·ylabel('문자열）' ) : '문자열' 어］ 해당하는 y축 이름을 표시．
·title('문자열’) : '문자열' 어］ 해당하는 그래프 제목을 표시．
·legend(’문자열’) : 그래프 안어］ '문자열' 로 표제를 붙임．
·text(x,y, '문자옐） : '문자열' 을 位，y) 좌표에 표시．
·gtext('문자옐） : 문자열이 표시될 위치를 마우스로 지정 , 마우스가 + 로 표시되며 마우스
 를 이동, 문자열을 표시할 위치에서 마우스 왼쪽 버튼을 클릭．
'axis([xmin xmax ymin 刃na刈） : x, y축 범위를 각각 xmin - 玎11缸과 ymin - 珥nax로
 설정
·axis square : 그래프를 정사각형으로 만듦．
·axis equal : x, y 축 눈금 크기를 동일하게 함．
·ax始 on : 그래프어］ 축 표시．


===== PAGE 192 =====
                                                     부록. Matlab 사용법   口m
·axis off : 그래프어］ 축을 표시하지 않음．
·axis( 'normal') : 그래프 설정을 디폴트 값으로 함．
'grid : 그래프어］ 격자선 표시, grid off 격자선 없앰．
·pause : 키 보드 입력이 있을 때까지 작업을 일시 중지．
'hold on : 현재 그래프어］ 다른 그래프를 추가로 그릴 때 사용．
·hold off : 현재 그래프 위어］ 다른 그래프를 그리는 것을 끝낼 때 사용．


 예) t = 0:0.5:10; y = sin(t); p1ot(t,y,'b+-');
     axis([0 10 -1 1]);回
     xlabel('t（라디안）' ); 列abel('si可t)')；回
     title( ' 싸인 곡선' ); text(3.14,0,'sin(pi)')回


 예) t = 0:0.5:10; tt = sin(t); ttt = cos(t);回
    하ot(t,tt,'ro-')；回
     hold on;回
     plot(t,ttt,'b抑 ' )；回
     hold off;回


 예) t = 0:0.5:10; tt = sin(t); ttt = cos(t);回
     plot(t,tt,t,ttt); legend('sin(t)','cos(t)');回
     legend안어］ 있는 문자열과 plot으로 그려지는 그래프의 순서가 맞아야 하며 , legend
     off 명령을 이용해서 표제 박스를 지울 수 있다．


'subplot : 하나의 그림 창어］ 여러 개의 하위 그래프를 그릴 경우 사용. 하위 그래프의 수어］
 따라 명령에 사용법이 달라짐．
' subplot(nr,nc,n): nr은 세로로 그릴 그래프 숫자, nc는 가로로 그릴 그래프 숫자, n은 그
 래프 번호．


===== PAGE 193 =====
194       퍼지, 진화컴퓨팅 프로그래밍



      예） subplot을 이용한 하위 그래프 위치 설정

                                         S口切：)1O亡 (211)
                                         S口bplo亡 (212)


                                         subplot (311)
                                         subplot (312)
                                         subplot (313)


                                sul丞江（9亡 (221)    St.山plo亡 (222)
                                subplot (223)     sul不江O亡 (224)


                                St.山I끄（) 亡 口2기    S口1不江C比 (322)
                                su杯끄（9亡 (323)     S口b下）lo亡 (324)
                                subplot (325)     S口上）下江O亡 (326)




      예) t = 0:0.5:10; y = sin(t); subplot(311); plot(t,y,'b+-')回
          axis([0 10 -1 1]);回
         덥abelCt（라디안）' ); ylabelCsin(t)')；回
          z = cos(t); subplot(312); plot(t,z,'r*:')回
          xlab에났라디안)'); ylabelCcos(t)')；回
          w = tan(t); subplot(313); plot(t,w,'ko-');回
         넜abelCt(라디안)'); ylabel('tan(tY）回


  상용로그 그래프용으로 다음과 같은 명령어가 있다．
  ·semilogx(t,tt) : 변수 t를 상용로그의 x축, 변수 tt를 y축으로 그린 그래프
  ·semilogy(t,tt) : 변수 t를 x축, 변수 tt를 상용로그의 y축으로 그린 그래프
      loglog(t,tt) : 변수 t를 x축, 변수 tt를 y축으로 상용로그 그래프를 그림


  그래프를 지우기 위한 명령으로 cif와 clg가 있다．
  ·clf : 그래픽 창의 그림을 지움

  ·clg : cif와 통일
  ·figure(h) : 새로운 그래픽 창을 염 . 예） figure( 1)


===== PAGE 194 =====
                                                                부록. Matlab 사용법     195



(2) 3차원 그래프
·plot3(t,tt,ttt) : 변수 t, tt, ttt의 데이터를 각각 x축, y축 및 z축 값으로 그린다. 기타 사용
 법은 히ot과 동일함．
·zlabel('문자열 ') :z축에 표제를 닮．
·axis([xmin 끄nax ymin 珥nax zmin zmax]) : z축을 포함한 축 범위 설정．


또 다른 명령어로 mesh와 surf가 있다．
·mesh(x,y,z,c) : x, y, z로 정의된 곡면에서 일정한 간격의 그리드를 선을 그린다. 이때 그
 리드 선의 색은 C 값에 의해 결정된다. mesh(x,y,z）으로 하면 c= z가 되어 색이 z의 값（3
 차원 곡면의 높이）에 따라 변한다．
·meshgrid(x,y) : 匡,y] = meshgrid(x,y）는 3차원 그림（mesh나 surface 그림）을 그리기
 위해 벡터 x와 y어］ 의해 규정된 영역을 행렬 x와 y로 변환한다．
·meshgrid（功 : [x,y] = meshgrid（功는 3차원 그림（mesh나 surface 그림）을 그리기 위해
 벡터 x에 의해 정의된 영역을 행렬 x와 y로 변환한다. 이는 匡,y] = meshgrid住,x）와 동일
 하다．
·surf(x,y,z,c) : x, y, z로 정의된 곡면을 그리며 면의 색은 C 값에 의해 결정된다．
 surf(x,y,z）으로 하면 c= z가 되어 색이 z의 값（3차원 곡면의 높이）어］ 따라 변한다．
·contour3(x,y,z)   :   co玭our(x,y,z）는      z의    값으로       등고선을        그리는       반면에
 contour3(x,y,z,n）는 n개의 3차원 등고선을 그린다.
·view([x,y,z]) : 3차원 그림의 시점（viewing an멤e）을 조정하기 위한 명령어로, 직각좌표
 계에서 각 축으로부터 시점까지의 각도를 정의한다. view(az,el)로 사용할 수도 있는데, 이
 때 az와 el은 각각 수평과 수직선으로부터 시점까지의 각도이다．


 예) t = 0:0.5:10; tt = sin(t); ttt = cos(t); p1ot3(t,tt,ttt)回


 예) [x,y] = meshgrid(-2:.2:2);回
     z = x. 米exp（吐.八2+y.八2)；回
     mesh(z）回 % 또는 mesh(x,y,z)
     pause；回
     meshc(x,y,z)回


===== PAGE 195 =====
196    L   퍼지, 진화컴퓨팅 프로그래밍



           pause；回

           meshz(x,y,z)回


      예) [x,y] = meshgrid(- 2:.2:2);回

           z = x. 米exp(-x.八24y.八2)；回
           surf佃乂回 % 또는 S出f(x,y,z)
           pause；回

           surfc(x,y,z)回


      예) x = -2:.2:2; y = -2:.2:3;回

           [x,y] = meshgrid(x,y);回

           z = x.米exp(-x.八2Hy.八2)；回
           contour(x,y,z)回
           pause；回

           contour3(x,y,z,20)回


      예) [x,y] = meshgrid(- 2:.2:2);回

           z = x. 米exp（놔x.八2 y.八2)；回
           mesh（기回

           view(30,60);
           xlabelCx'); ylab이行')；回
           zlabel('z = x.非exp(- x.八24/.八2)')；回




  5) 프로그래밍의 작성과 실행

      매트랩에서 프로그램 파일은 ' .1n'으로, 뎨이터 파일은 ' .mat'로 끝난다. 매트랩은 인터프리
  터 언어이기 때문에 명령 실행 창에서 직접 프로그램을 입력 실행시킬 수 있지만, 豆루그램이
  길거나 복잡한 경우 또는 나중에 수정이나 재사용이 필요한 경우에는 명령 창에서 실행하는
  것 보다 ' .lll' 파일로 만들어 실행하는 것이 유리하다. '.11l' 파일을 만들 때 매트랩의 에디터를
  사용하지만, 다른 텍스트 에디터를 사용해도 무방하다. 다만, 확장자를 ' .而으로 해야 매트랩


===== PAGE 196 =====
                                                                               '           부록. Mat冶b 사용법   ]   197



에서 실행이 된다. 아래 그림은 3차원 그림을 그리는 프로그램을 매트랩 에디터로 작성한 것
이다. 작성된 파일을 실행시키기 위해서는 해당 파일이 있는 디렉토리가 매트랩 경로 설정기
창의 현재 디렉토리어］ 있어야 한다. 이를 위해 경로 설정기를 이용하여 해당 파일의 위치를
설정한다. 실행（Run) 메뉴나 버튼을 클릭하면 해당 파일이 실행되고 오류가 있으면 오류 메
시지가 명령 실행 창어］ 나타난다. 파일에서 ％이 붙은 문장은 실행되지 않으며 , pause가 있으
면 거기서 정지한 상태로 키보드 입력을 기다린다. 키보드 입력이 있으면 그 다음 문장들이
실행된다. 문장이 ' ;'로 끝나는 경우 해당 문장의 실행 결과가 화면에 표시되지 않는다．


              「 卜IATLA8 Edit《나：／Debugger - [test.m卜 C出寸MNDOWSV寸바탐 山口目口
               客 F爬 丘tht )e'町 Debug IooIs Y녈ndow deID
               D 嚼묘               能 尋 땋                e 1台
                              Stack:   L                                 i
                    I[ x,yl = mestigrid(-2:.2:2);
                      z = x.+exp(-x八2)／八2).
                      meth(z)
                      너a나（30,60);
                      'dabel（才）; 너abeICy); 기ubelCz = 乂＋ex口（中＞< "2my. "' 2y);




            ［그림 6] 에디터를 이용한 프로그램 파일(test.m) 작성


               心 Path Brc'wser                                                          目回口
                好日 Ed梵 毖B낚 Eath
               스:1 크j 외
                C나汗ant                                             F카as in 바       t겨
                     nn小汕L寸 비 타 화 면                                  圃 Be已七 .rn
                                              '   B
                                                      『으쁘툐：   :]

                P
                 : : \l4且DLAE\ 七口口1k）口x\1na七I日b\ ,e, ee'
                 ::＼玉ml工Al＼七oolbox\ ma七I日b '＼口p呂         二
                 : :＼川ATLAB＼七口口lb口X\ lna七.1日b\ l, ,,g
                C : \14A끄JAl\ 七口olb口x\rna七lth\ e1knat
                .n :\p月ATL효B\ 七口口lb口）:\ma卜．上eb\ elf, ,r

                C:i:‘岩獸業：：
                         므:::::：芦： 器恥
               Ready                                                                4: 52 PM


            ［그림 7] 작성 파일의 디렉토리를 현재 디렉토리에 추가


===== PAGE 197 =====
   퍼지, 진화컴퓨팅 프로그래밍




             0

              g畦口닥尸XH
                                  小




                             ［그림 8] test.m 파일 실행 결과




(] ) 프로그램 제어 명령
매트랩에서는 프로그램의 흐름을 제어하기 위해 if. 丸r, while과 같은 명령문을 사용한다．

·for 문 : 이것은 특정한 꼐산을 반복해서 수행할 때 사용하며 그 형식은 다음과 같다. i 가
 a부터 시작하囚 문장을 반복해서 실행하는데 , 한 번 루프를 거칠 때마다 '1 는 b만큼 증가
 하며 i 가 C를 초과하지 않을 때까지 반복은 계속된다. b가 1이면 b 값을 생략한다. for
 루프 안에서 특정한 조건을 만족하면 해당 루프를 빠져나올 수 있게 하기 위해 if 문과
 함께 break 문을 사용한다. 아래 그림의 우측에서 if 조건을 만족하면 break 문어］ 의해
 이 문장이 속한 루프（for 루프）를 빠져나와 A 문장을 실행한다．


                                         如ri = a:b:c

                                             문장
              for i = a:b:c                  if조건
                        문장                         break;
              end                            end
                                         end
                                         A


===== PAGE 198 =====
                                                              부록. Matlab 사용법   199



 예） for i=1:2:6回
              如r j=1:2回
                 a(ij) = 1I(i + j -1);E크
              end回
      er넋回
      a回
      a   =     1.0000      0.5000
                0           0
                0.3333      0.2500
                0           0
                0.2000      0J667


·W址le 문 : 이것도 반복 실행을 위한 것으로 아래와 같은 형태로 쓰인다. 조건을 만족시키
 는 한（조건이 참인 한） 문장을 반복 실행하며, while 안의 조건 이외에 다른 조건어］ 의하1
 while 루프를 벗어나기 위해서는 아래 그림의 우측 형태를 취하며, break 문의 동작은 如r
 문장의 경우와 동일하다．

                                           while 조건
                                               문장
                      while 조건                 if 조건1
                          문장                         break;
                      end                      end
                                           end
                                           A


예） eps = 0.01; t = 1；回
      while (t > eps)回
              t = t/2；回
      end回
      t回
   m中t =        0.0078


===== PAGE 199 =====
200       퍼지, 진화컴퓨팅 프로그래밍



  .if 문 : 이것은 조컨의 만족 여부어］ 따른 실행을 처리하는뎨 다음과 같은 형식으로 사용한
      다. if의 조건부에는 ==, <. >, <=, >=, N＝와 같은 연산자를 사용해서 조컨의 진위를 판정
      하는 문장이 들어간다．


                                                   if 조건1
                                                     문장1
                            if조건                   elseif 조건2
                                  문장                 문장2
                             end                   이se
                                                         문장3
                                                   end



      예） a = 3; b = 5; x = [ 1 4 71;E크
           如r 卄1:length（功回
                   if 位（i) <= a）回
                           y(i) = a；回
                   elseif (a < x(i) & x(i) K b)回
                           y(i) = x(i乂回
                   이se回
                           y(i) = b；回
                   （표id回
           end回

           y   =      3       4        5


      (2) 함수(function) 작성
      자주 사용하는 프로그램이나 복잡한 豆쿠口램을 기능 별로 분할해서 이를 ' .1ll' 파일 형태로
  만들어 두면 프로그램 작업의 효율을 높일 수 있다化언어의 함수와 같은 역할을 함）. 이렇게
  작성된 ' .lll' 파일들을 사용자 정의 함수라 부르며 그 사용 형식은 다음과 같다．


===== PAGE 200 =====
                                         부록. Matlab 사용법   201



·function 출력인수 = fname（입력인수）
 사용자 정의 함수는 '.1n'로 작성되며, 파일명과 함수명이 동일해야 한다. 위의 경우 파일명
은 fname.m이어야 한다. 입출력 인수는 다수 일 수 있고 벡터나 행렬이 사용될 수 있다．
fn계l玲을 호출하는 파일에서 입력인수를 건네받아 fn帥e 함수에서 출력인수를 계산한 후 이
를 호출한 함수어］ 리턴한다. 평균과 표준편차를 계산하는 프로그램의 예를 보자．


 예） x = rand(30,2)；回
    [n,m] = size(x);E크
    avg = si-il可功/n回
    xavg = zeros(n,m);回
    如r i=1:n回
        xavg(i,:) = avg；回
    end回
    stdev = sqrt(sum((x - xavg).八2)In)
    -   avg =     0.4355    0.5153
        stdev =    0.2949    0.2992


    이 프로그램에서 평균과 표준편차를 계산하는 부분을 아래의 함수 stat로 만들 수 있
    고, 이 함수는 파일 stat.m으로 저장되어야 한다. x는 무작위 값을 할당받으므로 실행
    할 때마다 그 값이 달라진다．


    x = rand(30,2)；回
    [avg stdev] = stat（幻回
    -   avg =     0.5473    0.5771
        stdev =    0.2607    0.2463


===== PAGE 201 =====
202      퍼지, 진화컴퓨팅 프로그래밍




                             function [avg, stdev] = stat(x)
                                 % 함수 stat.m
                                 [n,m] = size(x);
                                 avg = sum(x)/n;
                                 xavg = zeros(n,m);
                                 for i=1:n
                                     xavg(i,:) = avg;
                                 end
                                 stdev = sqrt(sum((x - xavg).八2)/n);

                                             stat m으로 저장된 함수




      미분함수의 적분 값을 계산하는 프로그램을 작성하기 위해 다음과 같은 미분 방정식을 고
  려하자．
                                               !/ = sin (t )



      초기값이 !／小 시간 L에서 t／까지 위 식을 적분할 경우 다음과 같이 프로그램을 작성할 수

  있다（'integl.m'). 이 프로그램에서 적분을 위해 매트랩 내장 함수 ' ode23'를 사용하며, 이 때
  'ode23볘 초기 조건 L, tf, ％과 미분 식을 정의하는 함수명 ' der如1'이 입력인수로 건네진

  다. 아래 예에서 ' ode23'는 ' derivl.m' 파일의 함수를 호출해서 초기조건 yc를 가지고 시간
  to에서 tf까지 적분하고 그 결과로 t와 y를 출력변수어］ 넘긴다.


      예） % 파일명： integl.m
         yo = 0; tO = 0; tf = 2知1,回 % 초기 조건 설정
         % derivi 함수를 호출해서 적분
         [t,y] = ode23('derivl',[tO tf],yO);回
         plot(t,y,'b-');E크
         xlabel('t(sec)'); y1abe1('y(t)');回
         title(' sin의 적분')；回
         grid；回


===== PAGE 202 =====
                                                             부록. Matlab 사용법   i   203



             func如n yd야 = derivl(t,y)
             % 파일 derivl.m
             % 입력으로 시간 t를 받아 출력으로 미분값 yd야를 계산．
             ydot = sin(t);

                                   derivi m으로 저장된 함수


 또 다른 예로 Van der Pol 이차 미분 방정식을 고려해보자．

                                  a " + (x2 - 1 )a + x = 0

 이차 미분방정식이기 때문어］ 앞의 경우와 같이 적분하기 위해서는 일차미분방정식으로 변
환해야 한다（x = x2).

                                    펴 = x1 (1- x글 ) - x2

                                    x2 = 万1


 적분 계산을 위해 매트랩 내장 함수 ' ode45'를 사용한다. 'ode23'이 2차와 3차
Runge-Kutta 식을 사용해서 적분 계산을 하는 반면어］, 'ode45'는 보다 고차인 4차와 5차
Runge-Kutta 식을 사용하기 때문어］ 계산의 정확도가 더 높다. 아래 예에서 ' ode45'는
'deriv2.m' 파일의 함수를 호출해서 초기조건 X0를 가지고 시간 to에서 tf까지 적분하고 그
결과로 t와 x를 출력변수에 넘긴다．


 예） % 파일명： integ2.m
    to = 0; tf = 30;日
    xO = [0 0.25]；回 % 固의 초기값은 0, 万2의 초기값은 0.25

    % 함수 ' oder45 ' 어］ 의한 적분
    [t, xi = ode45('deriv2',[t0 tf],x0);回
    plot(t,x(:,1),'b-' ,t,x(:,2),'k:');回
    1egend('x1','x2');回
    title('Van der P아 방정식 ' )；回
    xlabelCt(secfl; y1abe1('x(t)');回
    grid；回


===== PAGE 203 =====
204   [   퍼지, 진화컴퓨팅 프로그래밍




                  function xdot = der加2(t,x)

                  % 파일 der如2.m
                  % 입 력으로 시간 t를 받아 출력으로 미분값 xd아를 계산．

                  xdot = zeros(2,1);

                  xdot(1) = x(1).*(1 - x(2) 八2) - x(2);

                  xdot(2) = x(1);

                                           deriv2.m으로 저장된 함수



                                                   Van der P이 방정 식




                                       5      10          15         30
                                                        t(sec)



                                                    실행 결과




                                               연습문저1


      [1] 행 구분을 위해 ' ;'를 사용하여 다음 데이터를 변수 x에 할당하시오．
          2   4    6   3
          3   7    8   1
          0 10     9    5
      [2] 문제1의 변수 x에서 2행 4열 원소를 변수 y어］ 할당하시오．
      [3] 문제1의 변수 x에서 3열 원소를 변수 z어］ 할당하시오．


===== PAGE 204 =====
                                               부록. Matlab 사용법     205



[4] 문제1의 변수 x에서 다음 데이터를 추출하여 변수 w에 할당하시오．
    3     7   1
    0     10 5
[5] x= [123],y= [1, 2, 3],z= [1; 2; 3] 일 때 x, y, z 사이의 차이를 설명하고 각각의
   차원을 구하시오．
[6] 문제5에서 x+ z를 실행하면 오류가 발생하는 이유를 설명하시오. 문제5의 변수 z의
   전치를 구하고 변수 x어］ 더하라．
[7] 문제5에서 x.求y, 寸y, 寸z, x.米z를 실행하고 오류가 발생하면 그 이유를 설명하시오．
[8] 문제5의 x를 x의 모든 원소의 합으로 나누시오．
[91 x= 0: 2: 10 일 때 다음 식의 값을 구하라.

        y= 2em ' (cos (/ 三) +sin (x2))

[10] x = 1 + i, y = 2 竹 3可 일 때 x+ y, x- y, xy, x屈를 구하라．
[11] 사인 30（도）의 3제곱과 탄젠트 0.5（라디안）의 제곱근 값을 구하시오．
[12] 직각 좌표계로 표시된 복소수 z = 2 - 2i 를 극좌표로 변환하고, 이를 다시 직각좌표
   계로 변환하라．

[131 e10의 상용로그와 자연로그 값을 구하시오．
[14] 모든 원소가 0인 10x5 크기의 행렬을 x를 만드시오.
[15] 문제14의 변수 x와 차원은 같지만, 모든 원소가 3인 행렬을 만드시오.
[16] 모든 원소가 무작위로 [-1,1] 범위의 값을 갖는 5x5 행렬을 만드시오．
[17] 매트랩의 heli) 기능을 이용해서 항등 행렬(identi缸 n追出功를 위한 함수를 찾고, 5x5
   크기의 항등 행렬을 만드시오．
[18] 다음 두 개의 이원 일차 방정식의 교점을 행렬을 이용하여 구하라．
    x+ y= 1
    x- y= 1
[19] 콜론（:) 연산자를 이용해서 0에서 30까지의 수에서 모든 홀수를 포함하는 벡터를 만드
   시오（만들어진 벡터는 크기 순서로 정렬되어야 함）.
[20] [1, 10］의 범위에서 일정한 간격으로 분포된 10개의 숫자를 갖는 벡터를 구하시오．
[211 [10, 1000］의 범위에서 로그 간격으로 분포된 10개의 숫자를 갖는 벡터를 구하시오．


===== PAGE 205 =====
206   [   퍼지, 진화컴퓨팅 프로그래밍



      [22] 0에서 0.1 간격으로 2知i까지 증가하는 원소를 갖는 벡터 t를 만들고 이 벡터의 코사
          인 값과 싸인 값을 각각 계산하여 변수 y와 z어］ 할당한다. 변수 t와 y, t와 z 사이의
          관계를 그래프로 표시하여라. 그래프어］ 축 이름과 제목을 붙이고 가로축의 범위를 [0,
          3], 세로축의 범위를 [-1,1]로 설정하고 각 곡선어］ 표제 붙여라. t와 y의 곡선은 붉은
          색의 실선에 데이터 표시 마커는 "+" 를, t와 z의 곡선은 파란색의 점선어］ 표시 마커
          "永" 를 사용하시오．
      [23] 문제18을 수행하는데 있어 먼저 변수 t와 y의 그래프를 그리고, 그리드를 표시한 다음
          어］ t와 z 사이의 그래프를 추가하라.


===== PAGE 206 =====
                                        INDEX
                                          Fuzzy & Evotu鈿n＆叩 Co汀｝               Pro莩帥imn穹




1 A1                                       fuzzification      18
Aggregation 29                             fuzziness     3
allele   78                                fuzzy inference         17
antecedent     17                          fuzzy intersection relation 15
approximate reasoning 17                   fuzzy union relation 15
arithmetic crossover          93
                                           1 G毋

1B 1                                       GAs: Genetic Algorithms            77
binary mutation 90                         gene     78
boundary mutation 93                       generalized modus ponens            18
                                           Genetic Algorithms            63
.C 好                                       genetic operators            90
centroid 42                                Genetic Programming 63
chromosome         78                      genotype      77
Classifier System 63                       Gustafson-Kessel 알고리즘 53
compactness        53
complement         5                       'H 巾

consequent     17                          heuristic crossover           93
crossover     90
a -cuts   9                                11   斗



                                           implication 18
1D 心                                       implicit parallelism 77
IDE: Differential Evolutionary Scheme      individual 78
  64                                       inference     16
Defuzzification         30                 innovation intuition 77
Differential Evolutionary Scheme   63      intersection       5


1 E巾                                       1K 心

Evolution Strategy           63            k배 교차 검증 155
Evolutionary Programming 63
explicit parallelism 77                    1L '
                                           leave卄one-out 교차 검증 155
1 F1

FCM 알고리즘 53                                1M 斗

FCM 클러스터링               48                 Mamdani형          18


===== PAGE 207 =====
                                                   率
208   [    퍼지, 진화컴퓨팅 프로그래밍




  membership function                   4                   S \/ 小


  multi-non uniform mutation                      93        validity index               53
  mutation          90
                                                            SW 小

  1N 毋                                                      wheel           85
  nonuniform mutation                   93
  normalized geometric ranking                     86       S 기 寸


                                                            가우스 함수                 13
  1o.                                                       가중치          65
  one-point crossover                   91                  간접법          18
                                                            강인성          77
  .P 毋                                                      개체 벡터                64
  phenotype            77                                   개체         78
  population           77                                   경계 돌연변이                    97
  premature convergence                      84             교배 풀 62, 78
  probability          3                                    교배1        62, 90
                                                            교배용 개체                64
  1R 骨                                                      교배율 65
  rank     86                                               교집합             5
  ruulette        85                                        교차 검증                155
                                                            구조 인식                132
  .s 小                                                      균일 교배 연산 65
  schema theory               77                            균일 돌연변이                    94
  separation           53                                   근사 추론                17
  simple crossover                 90                       기반 선택                86
  single     36
  s-norm        7
  Sugeno 형             18, 36                               나비 데이터                 44
                                                            내재적 병렬성                    77
  1T 每
  t- norm       7                                           .   ［二 S


  tournament             87                                 다차원 맴버쉽함수                         13
                                                            단순 교배                90
  .u 茹                                                      돌연변이 연산 61
  union     5                                               돌연변이                62, 90
  uniform mutation 93                                       돌연변이율 90
  unsupervised learning strategy                       48   동치         10


===== PAGE 208 =====
                                                            八DEX   ] 209
1 a     好                                비퍼지화 30
랭크 기반 선택 88
랭크 86                                    .   人 韶


룰렛 85                                    산술 교배 97
룰렛H휠 선택 87                               선택 85
                                         선형 보간 97
.   口   常                                선형 외삽 98
매핑          133                          口 1수준 9
멀티小비균일 돌연변이 96                           스키마 이론 77
멤버쉽함수 4                                  승자승 87
모델 32, 129                               승자승 선택 61, 89
모델링          129                         실수형 유전알고리즘        122

모델의 검증 155
목적변수 64, 78                              1o    好

목적함수 값어］ 의한 종료                     101

목적함수 42, 78                              애매성       3, 12
무감독 학습전략 48                              언덕 등반 메커니즘 77
무게중심법               30                   엘리트주의 64
무성생식              62                     여집합 5
                                         염색체 78
1 tJ 的                                   외적 병렬성 77
벌칙함수 137                                 유성생식  61
변수 영역 4                                  유전 연산자 90
변형자 10                                   유전알고리즘 63, 77, 103
부드人드랩                   155              유전자 78
분류시스템 63                                 유전자형        77
분리성           53                         이진 돌연변이 90
분할 검증 155                                이진 유전알고리즘 119
분할 엔트로피                       53         일점 교배 91
분할 행렬 43
분할계수 53                                  .x    蜘

분할의 타당성                       53         재결합 연산자 61
블랙박스 32                                  즈平나이프 검증 155
비균일 돌연변이 94                              적합도 함수 65, 83, 137
비례 선택 85                                 적합도 61, 83, 115
비율조정 함수 83                               적합도에 비례한 선택 61
비율조정               85                    적합도함수 66


===== PAGE 209 =====
210       1       퍼지, 진화컴퓨팅 프로그래밍



  전건부／조건부 17                                           퍼지 논리 연산 7
  전역 최적 해 115                                          퍼지 모델 구축 141, 152
  정규화 기하학적 랭크 86                                       퍼지 모델 129, 138
  조기수렴                 84                              퍼지 모델링          129
  종료조건 100                                             퍼지 변수 service의 퍼지 집합 poor, good,
  중심 벡터                 42                                 excellent   19
  직접법 18                                               퍼지 변수 19
  진화 세대 수어］ 의한 종료                                100   퍼지 변형자 11
  진화알고리즘 61                                            퍼지 분할 행렬 48
  진화전략 63                                              퍼지 분할 48
  진화프로그래밍 63                                           퍼지 싱글톤 36
  집단 크기                 64                             퍼지 연산자 18, 25
  집단 77                                                퍼지 조건 명제              17
                                                       퍼지 집합 3
  1   天       毋
                                                       퍼지 추론 17
  차분 진화 64                                             퍼지 추론법 18
  천이규칙                 77                              퍼지 클러스터 평가척도 53
  최대H최소 합성                        17                   퍼지 클러스터          48
  추론 규칙                 18                             퍼지 클러스터링              41, 132
  추론 16, 33                                            퍼지 합 관계          15
  출력 퍼지 집합 합하기                              29         퍼지（FCM) 클러스터링               132
                                                       퍼지 10
  .   디       好
                                                       퍼지화 18
  코딩              79                                   평가척도 54
  클러스터                 42                              표현형       77
  클러스터링                 41
  클러스터의 조밀성                            53              .   舌 好


  클러스터의 중심                        49                   하나를 제외한 교차 검증 155
                                                       하드 클러스터링              41
  .   드 好                                              함수 최적화 66, 111
  타당성 평가척도 53                                          함의 연산자 27
                                                       함의 18
  1   끄       雜
                                                       합성 관계 16
  파라미터 인식                    132                       합집합 5
  퍼지 관계                 14                             해독 79
  퍼지 교 관계                    15                        혁신직관 77
  피지 규칙                 18, 48                         형질 78


===== PAGE 210 =====
              INDEX   回L1

확률 3
후건부／동작부 17
후건부 36
휠 85
휴리스틱 교배1 98


===== PAGE 211 =====
저자소가I I 황회수

연세대학교 전기공학과 졸업, 동 대학에서 공학박사 취득. 한국고속철도 고속전철기술개발사업단 수석연구원
으로 프랑스 GecAisthom-SA 및 (3ec씨sthom Transport에서 KD( 고속전철 기술이전 수행, 차세대 한국형 고
속전철 개발 프로젝트（KBS 신화창조 방송） 수행． 기술신용보증기금 기술자문위원, 한국 퍼지 및 지능시스템학
 호J 이사를 지냈고, 한국철도시설공단 품질／환경／안전 자문위원으로 있다. Sc＞논문 11편을 포함 60편의 논문발
표와 저서 '컴퓨터에 의한 진화계산 및 진화디자인’ , '아이디어 발상 A To Z' , '나를 가두는 생각에 날개를
달자' 가 있다. 현재는 한라대학교 전자정보공학부 교수로 창의적 사고와 트리즈 관련 기고, 강의 등의 활동도
하고 있다．




                  ［매트랩］
퍼지, 진화컴퓨팅 프로그래밍

발행일 I 2006년 3월 1일

저 자 1 황힉수
발행인 1 모흥숙
편 집 1 박윤힉· 이경혜

발행처 1 내하출판사
등 록 1 제6-330호
주 소 1 서울 용산구 후암동 123너
      TEL : (02)775-3241'-'5
      FAX : (02)775-3246


ISBN 1 89-旬17너04-5
정가     12,000원



E-mail   1 naeha孕naeha.co,kr
Homepage I www,naeha.co,kr


· 책의 일부 혹은 전체 내용을 무단 복사， 복저L 전제하는 것은 저작권법에 저촉됩니다．
· 낙장 및 파본은 구입처나 출판사로 문의 주시면 교환해 드리겠습니다．


===== PAGE 212 =====
퍼지, 진화컴퓨팅 프로그래밍
Fuzzy, Evolutionary Computing Programming

1장 , 퍼지 이론
2장 . 퍼지 클러스터링
3장 . 진화알고리즘H차분진화
4장 . 유전알고리즘
5장 . 퍼지 규칙의 생성
  阜 . Ma姓ab 사용법
    쿠그램 코드 리스트




                         1S} N 89- 57 7- 04- 5




                                         1
                                         9356




                        788957 17 。42
                         ISBN 89 5717- 04 5
