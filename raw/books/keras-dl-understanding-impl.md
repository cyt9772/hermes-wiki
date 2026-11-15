---
source_url: "/run/media/yutae/Data/Keras 기반 딥러닝의 이해와 구현.pdf"
ingested: 2026-11-15
sha256: cf977bfb976cf3f957df59d7ff86cc8ec91c2a6ead4977887c58014259fbe218
type: raw-source
method: text-extract
---

# Keras 기반 딥러닝의 이해와 구현 (raw source)

> **출처:** USB 원본 PDF (`/run/media/yutae/Data/Keras 기반 딥러닝의 이해와 구현.pdf`, 로컬 참고용 — git commit 불포함)
> **방법:** 내장 텍스트 레이어에서 `pdftotext -layout`로 추출 (OCR 불필요)
> **쪽수:** 339쪽 | **추출 텍스트:** 494 KB
> **주의:** 원고는 scan/레이어 추출로 영문·숫자·특수자 일부 아티팩트가 있을 수 있음. 해석 시 원본 PDF와 대조.
> OCR 추출 디렉터리 `raw/books/keras-dl-understanding-impl.ocr/`는 git-ignored (로컬 참고용만) — 본문은 아래에 내장.

## Book metadata
- **Title:** Keras 기반 딥러닝의 이해와 구현
- **Pages (PDF):** 339
- **Source:** Keras 기반 딥러닝의 이해와 구현.pdf
- **Ingested:** 2026-11-15

## Extracted text (all 339 pages)



===== PAGE 1 =====
                     사외반출가능




       Lv.2 실무역량


Keras 기반 딥러닝의 이해와 구현




          Hachine
          Learning




       $ItM$UNG


===== PAGE 2 =====
파이썬과 Keras를 활용한 친절한 딥러닝 원리학습 및 활용


Keras 기반 딥러닝의 이해와 구현                ［제 3.02 판】


                         임베디드 전문가 그룹 윌텍 저




               CODEXPERT
               임베디드 전문가 그룹 윌텍



           임베디드 전문가 그룹 윌텍


===== PAGE 3 =====
Keras 기반 딥러닝의 이해와 구현                              L I3.02판I


簪 공인 강사 정 호채, hochae65@naver.com
管 전자공학 석사, 시DL연구소 대표이사, 삼성전자 및 다수의 기업체, 교육기관 출강
. 성균관대학교 겸임교수, 국제대학교 겸임교수 역임

● 공인 강사 깊 성호, james3302@naver.com
솔 전자공학 석사,
         （주）
           임베딕스 대표이사, 삼성전자 및 다수의 기업체, 교육기관 츌강
● 성균관대학교 겸임교수, 국제대학교 겸임교수 역임

● 공인 강사 송 화정，clance@naver.com
. 전자공학 석사,
         （주）
           행복한기술 대표이사, 삼성전자 및 다수의 기업체, 교육기관 출강
釀 성균관대학교 겸임교수, 삼성전자공과대학교 겸임교수 역임


. 공인 강사 김 태균, kimtglll@naver.com
* 전자공학 석사,
         （주）
           기쁜기술 개발실장, 삼성전자 및 다수의 기업체, 교육기관 출강
읗 성균관대학교 겸임교수，삼성SOS SCSA 전담교수, 국제대학교 강사 역임

e 공인 강사 기 호민, minisege@naver.com
參 전자공학 석사,《주）
            기쁜기술 대표이사！삼성전자 및 다수의 기업체, 교육기관 츨강
鬱 성균관대학교 겸임교수, 삼성전자공과대학교 겸임교수 역임

鬱 공인 강사 류 겊식, keyseek@naver.com
簪 전자공학 박사,
         （주）
           윌텍 대표이사, 삼성전자 및 다수의 기업체, 교육기관 출강
● 성균관대학교 겸임교수！용인송담대학 겸임교수，아주대，강남대 강사 역임

* 공인 강사 김 은경, m아rnio999@naver.com
* 컴퓨터교육학 석사,
           （주）
             에듀닉스 교육사업이사, 삼성전자 및 다수 기업체, 교육기관 출강
● 성균관대학교 겸임교수, 삼성SDS SCSA 전담교수, 직업훈련원 전임교수 역임




學 본 도서의 저작권은（주）윌텍 및 각 저자가 보유하고 있음
軫 저작권자의 허가 없이 무단으로 전재，  복제，  발췌, 디지털화 하는 것을 금합니다．
* 실습보드 구입 및 출강 문의：070-8740-2124
                              （주》윌텍 부설 codeXpert 연구소

●（주）윌텍 패밀리 기업：
             （주）
               행복한기술,《주）기쁜기술,（주）임베딕스,（주） 에듀닉스
好 윌텍 패밀리 부설 임베디드 시스템 소프트웨어 전문 연구소 codeXpert


===== PAGE 4 =====
차려I
1부. 머신러닝／딥리닝 개요                                               7
    1과. A.l, M.L, OeeI Learning 개요                            9

    2과. Machine Learning과 Percerflron                        21



2부. 머신리닝 기본                                                  29
    1과. Linear Regression                                    31

    2과. Logistic Regression(Binary Classification]           70

    3과. Softmax ClassificationEMultinomial Classification]   89



3부. 딥리닝 기본                                                   103
    l과. Multi Layer PerceDtron                               105

    2과. MNIST Dataset and Keras                              123


4부, CNN(C이lv이Uti에비 Neur비 Network)                            147
    1과. [;H" 개요                                              149

    2과. CNN 기본연산                                             158

    3과. CNN 기반 Classification                                183

    4과.〔刑N 발전 시키기                                            201


===== PAGE 5 =====
                                    차례
5부. RNNulecurrent Neural Network)   253
     l과. Time Series Forecasting    255

     2과. RNN Models                 266


6부, 부록                              293
     1과. N내끼列 라이브리리                 295

     2고k. lensorflo出 프로그래밍 기초       314

     3과. Keras 모델 생성, 저장 및 복원       325

     4과. Mat미Ut 라이브러리               338


===== PAGE 6 =====
1부. 머신러닝／딥러닝 개요


===== PAGE 7 =====
1부. 머신러닝／딥러닝 개요                  1과. A.I, M.L, Deep Learning 개요




             1부. 머신러닝／딥러닝 개요


              12F. AJ. M.L, Deep Learning 개요




@）임베디드 전문가 그룹 윌텍           9-    무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 8 =====
1부. 머신러닝／딥러닝 개요                      1과. A.I, M.L, Deep Learning 개요


 AI(Artificial Intelligence)                       임베디드 전문가 그룹 윌텍


  Q 시에 대한 다양한 정의
     ㄱr‘正*
      -I
                                     니쫠ㅎ


 ^John McCa뜨乫. .기'II를인갼행동의지식에서와같이행동하게만-I--
 uarrmoutn` I 닐＞이
                인간의 학습능력과 추론능력. 지각능력. 자연언어의 이해뇽력 등을 컴器터 IL
    두산백과
                로그램으로 실현한 기술
   컥퓨터이터너I
   IT喜어；LHA.珏   인간의사고과졍또는지적활동믈대신‘"階전기장치

  시사경제용어사전      고도의 문제해결 능력을 가진 인공적 지능

  천다사언기숙사저      짓싶골할의읕용기술에입각하여 컴퓨터로하여금인간의지식행동을대행시
  ---- '- ' -   기력고 ㅍH三 섯
   전자용어사전       컴퓨터로 인간의 지적 활동과 같은 처리를 대행하는 시스템

  생명과학대사전 AF쁠茫,
             ,i '추론" 뗀"언어"H'ㅐ등’"『조'능“율
                                    " 「’거프
                                       "로그래으
                                           "로
  매일경제사전        인간의 사고과정 또는 지적 활동을 대신하는 장치




＠임베디드 전문가 그룹 윌텍              -10 -   무단 전재, 복제, 발췌. 디지털화 금지


===== PAGE 9 =====
1부. 머신러닝／딥러닝 개요                                1과. A.I, M.L, Deep Learning 개요


 시 기술에 대한 접근방식의 변화                                                                엮베디드 전푼가 그룹 윌텍



      2옭 규斗걋］m 多，l스每ll      전문가들이 정립한 논리와 衫l에 따라 기계가 판단
      (1950년대 ∼）              : 개는 털이 있다. 꼬리가 있다. 짖는다 등
  Machine Learning(션경망）         인간이 만들어 놓은 지식을 기계에 학습
       0 980년대 "r         : 전문가들이 모델링한 규칙들을 데이터를 통해 기계가 학습
      莎發好弘 L發jffljfl!        인간의 사전작업 없이도 기계가 데이터를 학습 가능
      (2010년대 ∼）           : 모델링한 규칙 없이 스스로 학습하여 '개' 를 구분 가능
                                              Mad'ine learning

                                                         1뜨，/,／·직二7솥
                                                                                            Dog
                                               -+        t궁1ㅎ 今多-'S
                                                         .tr '   ∼＞1 " '     스*

                               Feat. e extraction             야漱misatlon




                                                Deep learning



                                        三콱쑈：::2三                                  -4
                                         Feature extraction + Optiutsation                 0utPuㅎ

                                                                           [Source: mmcventures.com]




 임베디드 전문가 그룹 윌텍
C）                            -"       -       무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 10 =====
1부. 머신러닝／딥러닝 개요                   1과. A.I, M.L, Deep Learning 개요




   J Machine Learning: 데이터를 이용해서 컴퓨터가 어떤 지식이나 璡턴을 학습
  露Deep Learning: 다층구조 형태의 신경망을 기반으로 하는 머신 러닝의 한 분야




@）임베디드 전문가 그룹 윌텍          -12 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 11 =====
1부. 머신러닝／딥러닝 개요                                              1과. A.I, M.L, Deep Learning 개요




        -               -               ,-               -              ∼   －
            CPU             (40        K40+ cuDNN1     M40+ CuDNN3      M40+ cuDNN4

            [Source: nvidia.com, AlexNet training throughput based on 20 iterations I




＠임베디드 전문가 그룹 윌텍                              -13-            무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 12 =====
1부. 머신러닝／딥러닝 개요           1과. A.I, M.L, Deep Learning 개요




＠임베디드 전문가 그룹 윌텍   -14 -   무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 13 =====
1부. 머신러닝／딥러닝 개요                                                     1과. A.l, M.L, Deep Learning 개요




  孕 딥러닝 알고리즘의 향상
  0 Better Activation Function
  0 Better optimization schemes
   0 Better weight-initialization
   0 Regularization




                                                                .
             2《〕12   2o］
                       크   2o]4   20巧   2이6   긔：57   2〔기8   I




＠임베디드 전문가 그룹 윌텍                                      -15 -          무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 14 =====
1부. 머신러닝／딥러닝 개요                                                            1과. A.I, M.L, Deep Learning 개요


  딥러닝이 주목 받는 이유
              （4)                                                                                          임베디드 전문가 그룹 윌텍

   卑 오픈소스 프레임워크 지원 ( Democratization of DL)
       〔）eep m8113m'1. PrOnle빎810 Sx-Mond` Gn｝
                                             빎th S
                                                《.r心 갔n9
                                                                          히似m11
                                                                          ● T胞·
                                                                              ｀可겯hmm        `4刃
                                                                            作∼｀心寸往          뱁出珊
                                                                          名 ㅄG七曲            1211.
                                                                            TE-+m什mm 贓     'I幽
                                                                          *18d '， 功7        5柳




 Source: https://towardsdatascience.com/which-deep-
 earning-framework-is-growing-fastest-3f77f14aa318]                                                 [Source: lensorFiow Summit
                   -    2010             2013              2014           的祗             2017        ㄻ18




                       α*W)
                       theano




                                                                                                 닙半→咆toT                 N아니寸k
                      아 N4occL xyU
                  卜℃ cm.
                       a니꿈이 Y？甘to'cc.,                            a텍슉능
                                           낙eV,4ㅇ六｀飇）




 임베디드 전문가 그룹 윌텍
C）                                                                -16 -   무단 전재. 복제, 발췌. 디지털화금지


===== PAGE 15 =====
1부. 머신러닝／딥러닝 개요                  1과. A.I, M.L, Deep Learning 개요




  Q 지능형 기기 :
  . 시를 탑재한 기기를 통해 인간의 일상적인 작업을 자동화
  . 자율주행 자동차. 로봇. 챗봇 등

  Q 지능형 시스템 :
   JAI를 기반으로 한 시스템을 구축하여 의사 결정. 문제 해결 등의 작업을
   0 의료 진단 시스템. 금융 투자 시스템. 생산 공정 최적화 시스템 등




＠임베디드 전문가 그룹 윌텍          -17 -   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 16 =====
1부. 머신러닝／딥러닝 개요                   1과. A.l, M.L, Deep Learning 개요




          샤 E   ＇녑m", q

          ＾灌 S1i”너t..k刪

            ｀뇨U日이 ^1 웃




＠임베디드 전문가 그룹 윌텍           -18 -   무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 17 =====
1부. 머신러닝／딥러닝 개요                                          1과. A.I, M.L, Deep Learning 개요




              2012         2013        2014            2015           2016           2017           Jan-Jun
                                                                                                     2018

            Source 皿꾜끄i쇼그〃
                         ＾工느“ －고d 르 - 乙 ㅈ＝‘立느꾜   尸   겹￡X htm1가胞d1읽d亡／ㄷDntPn1/`.mn.nen心apr27f1오n＆∼




＠임베디드 전문가 그룹 윌텍                        - 19 -           무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 18 =====
1부. 머신러닝／딥러닝 개요                   1과. A.I, M.L, Deep Learning 개요


 사람과 딥러닝 누가 더 잘 구별할까？                             CODEXPERT
                                                  임베디드 전문가 그룹 윌텍




                                             [ Source: Goo이e Image ]

           , 曲기어7t 絮自 "：无쾨1 斗，
                    三＞ 납分싸 仇늑 -상．
  많은 데이터를 활용한 반복적인 학습을 통하여. 정확한 결과를 도출하기 위한 체계를 구축해야 함




＠임베디드 전문가 그룹 윌텍          - 20 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 19 =====
1부. 머신러닝／딥러닝 개요                   24. Machine Learning F Perceptron




              1부. 머신러닝／딥러닝 개요

        I과* A,i, M.L. Deep Learning 걔2.
        2과. Machine Learning2F Perceptron




@）임베디드 전문가 그룹 윌텍             -21 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 20 =====
1부. 머신러닝／딥러닝 개요                                  2과. Machine Learning과 Perceptron


 고전적인 프로그래밍의 한계                                                   CODEXPERT
                                                                  임베디드 전문가 그룹 윌택


  @ Explicit Programming: 고전적인 프로그래밍 방식
   孕 기본 개념
    ＇小 문제 해결을 위한 R미e을 ㅍ로그래머가 직접 결정
    4. 프로그램은 프르그래어가 정한 문제 해결을 위한구칙
                                 （Rules)들을 기반으로 작성
   好 한계；난이도가 높음
    4. 예: Spam Filtering. Automatic Driving
    4. 다양한 상황에 따라 정해진 Rules. .만 해결할 수 없는 문群도 있을 수 있음
    4. 복잡하고 다양한 m겨e들을 적용해야 하며. 구현이 쉽지 않음
  .Explicit Programming 의 한계를 극복하려면？
    /' 프로그램이 직접 문제 해결 방법을 학습한다면？

  Q Machine Learning

  "명시적인 프로그래밍 없이 톄이터를 이용하여 컴퓨터가 어떤 지식이나 패턴
                                         （R미es）
                                              을
  학습하는 것' (Arthur Samuel, 1959)




                                                                                    I
＠임베디드 전문가 그룹 윌텍                         - 22 -    무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 21 =====
1부. 머신러닝／딥러닝 개요                             24. Machine Learning과 Perceptron


 Machine Learning                                             임베디드 전문가 그醫 윌텍


  孕 공학적 접근방법：T, P. E를 사용하여 정의
                        - 성능을 P. , 측즈
                                                          景찾”'서능"1’"삐
                                                                    '
                                     Task: Ma∥으I Spam 여부 분류




                                               二ㅍ＝」L= =


                              ,-    一∼   Performance『
                              ＼∼∼Mall의 Spam 분
               Label:                … 조청릉죵가곁괏
               Spam                    성능 평가
               or Not                                            x아g의之．
                                                                      비
                                                                    ` V" 盼，
                                                                          , ce
  Input：처리해야할Data, Output：연산을통해처리한결과，
                                    Label: Input에대한정답
                                                    （목표값） -




@）임베디드 전문가 그룹 윌텍                   - 23 -      무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 22 =====
1부. 머신러닝／딥러닝 개요             24. Machine Learning과 Perceptron




@）임베디드 전문가 그룹 윌텍   - 24 -     무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 23 =====
1부. 머신러닝／딥러닝 개요                              2과. Machine Learning과 Perceptron


 Supervised Learning                                              CODEXPERT
                                                                  임베디드 전문가 그醫 윌텍


                （회귀） i거컨이 욕갸- k--t는
     Q Regression                             '-l니 )
     . 특정 실수 값을 예측하는 문제              공부시간       10     20   30     40    50
       /' 예）공부 시간 대비 시험 점수           시험점수        52    65   77     85    92



     @ Classification
                    （분류）
     .Binary-class Classification    공부시간       10     20   30     40    50
       ／卜 0,1 예측
               （이분법적 분류）             시험점수 Fail(0) Fail(0) Pass(D Pass(D Pass(D
       ,1- 예）공부 시간 대비 합격 여부


     . M이ti-class 디assification
                                     공부시간       10     20   30     40     50
       #1' A, B, C. ft … 예측          시험점수        F     D    《＝     B      A
       /' 예）공부 시간 대비 학점



 [      실제로 대규모의 Input Data와 Labels(Dataset）
                                           을 사용하여 Machine Learning을 진행




@）딛J눼디드 전문가 그룹 윌텍                   - 25 -     무단 전재, 복제, 발췌, 디지털화 금지


===== PAGE 24 =====
1부. 머신러닝／딥러닝 개요                                                           2과. Machine Learning과 Perceptron
…m "                   스∼쓰心二茗堪角茗寸－m∼         …     『 …∼斗「      好呼拜… …呼發嚼姆촌撫鉀*헷射異包多軫瀜蠟鑽斗智重鱗弩驪婢｛撫樓窪경身多熙如辦戈｛釀照，
                                                                                                           交墨鄒甲轟꼴뾰駟無轍하




  Neuron과Perceptron                                                                                                       CODE,
                                                                                                                          ? HCIE   XPERT     1 t$


                      @ Sin이e Perceptron 구성
                               구분                                               설명
                       Input（입력）                 · 하나혹은그 이상의 Perceptron 입력
                       Activation Function       · Step function              . Sigmoid. ReLU 등
                                                               （특정 값기준으로0/1 구분）
                      （활성함수）                     · 입력에 가중치를곱한 값의 총 합을 입력 받아 정해진 출력을 내보내는 함수
                       Output
                           （출력）                  · 활성함수의 출력 결과




                      --輛，
                                                                     -
                                                                          Input weight                      ,   .                          output
                                                                     - "∼－ "'                      `iHo =2伊，
                                                                                                           a^＾즘／
                                                                                                               七*y-!
                         . Node
                           Ranvier
                            of麝
                             ji Output
                      -珥시맡七匹쓰띱了多쁜 ’녹
                                                                     -- " 1

                                                                     --
                                                                           ㅈ
                                                                            '          이i ,
                                                                                                   가穹→ 면一扼r:u샌
                                                                                                    '
                                                                                                                     L戶卉乙

                                                                                                        Activation Function
                                                                                                                                             y
                                                                                                                                              '




                      -
                                                                           工2



                        NucIus
                        鞭  ，脾Myinheath Schwann
                                           ceil
                                                                                               工
                                                                                 :w2
                                                                                                                    α（D
                       쑤，                                                  x3



                                                                                                                          ixi+ b)
                       Input
                                                                                                    a
                                                                                              Y=
                                                                                                        (
                                                                                              伊뺙m山‘




＠임베디드 전문가 그룹 윌텍                                                - 26 -           무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 25 =====
1부. 머신러닝／딥러닝 개요                                          2과. Machine Learning과 Perceptron


 Code: Perceptron 구현
                   （1)
  . ［예제 1] 다음 Perceptron 모델을 구현한 코드를 분석하라
                              [n Input / Weight / Bias




 # Element-wise multiply
 mu]. = W * X
 print( "mul = w * x : {}'.format(mul))

 # Summation array and Add 址as
 S =
            {} rmat )
       sum mu1) + B
     np.
 print    =(s
                 .f。
                        (s)          )
                              2i Multiply and
                               Summati。   n

    ctivation Function : Step Fuction
 y = np.f1oat32(s >10) . .                                mul = 贓 * X : 1 4 10 18]
 print( " y == tI " Jormat(y))                            s == 42
                                       [31 Activation     y = 1.o
                                         Function




@）임베디드 전문가 그룹 윌텍                               - 27 -      무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 26 =====
1부. 머신러닝／딥러닝 개요            2과. Machine Learning과 Perceptron




＠임베디드 전문가 그룹 윌텍   - 28 -     무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 27 =====
2부. 머신러닝 기본


===== PAGE 28 =====
2부. 머신러닝 기본                                      1과. Linear Regression




                    2부. 머신러닝 기본

         1과. Linear Regression
           Logistic Regression(Binary Clas崩ication)
         2과，
         3과，
           Softmax Classification(Multinomial Classification)




 임베디드 전문가 그룹 윌텍
C）                               -31 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 29 =====
2부. 머신러닝 기본                                    1과. Linear Regression

                                                     CODE兼PERT
 Machine Learning의 기본 프로세스                           임베다드 전문가 그룹 윌텍


  QStep 1: Hypothesis 설정
                       （문제해결을 위한 오델 수립）
   G Machine Learning은 학습하고자 하는 가설
                                 （모델）
                                    을 수학적 표현식으로 나타냄

  @ Step 2: Cost Function 설정
  色Cost Function: 가설의 성능을 평가할 수 있는 함수
    /' '설정한 가설을 통한 예축 값과 실계 값의 오차
                                （error)' 를 평가하는 함수
    ,$ Loss Function으로 불리기도 함


  @ Step 3: Learning Algorithm 적용하여 Training
  . 학습 알고리즘의 목적 + 일반적으로 cost의 최소화
                                （minimize)
    /2 Hypo出esis가 문제를 해결하기 위한 모델과 유사해지는 방향으로 학습 진행




 * Hypothesis
           （가설）
              : 일련의 현상
                     （상황）
                        울 설명하기 위해 설정된 가정
                                       （논리적 명제. 수식）




＠임베디드 전문가 그룹 윌텍                - 32 -   무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 30 =====
2부. 머신러닝 기본                                        1과. Linear Regression




  @ Regression(회귀): "Regression toward the mean"
    t2 예측 값은 '전체평균으로 되돌아 간다' 라는 의미의 통계학 용어
   〃 M.L에서 특정 값을 예측하는 문제에 활용


  @ Linear Regression
                    （선형 회귀）
   0 '가장 훌륭한 예측선 긋기'
   J Data를 가장 잘 표현하는 직선의 방정식을 찾는 것
    4. Data를 대표하는 Hypo功esi＄를 직선의 방정식으로 설정
    /2 수식에서 적절한 A
                （기울기）
                    . B(Y절편）값을 정하는 작업




 임베디드 전문가 그룹 윌텍
C）                              - 33 -   무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 31 =====
2부. 머신러닝 기본                                            1과. Linear Regression


 Example for Linear Regression                               c0DE,，本e트R,
                                                                      T
  回 다음과 같은 입력 x와 그에 대한 결과값 lab이이 주어져 있다면7
  . x에 대한 label 값을 나타낼 수 있는 적절한 함수의 형태7
   ＇小 x에 대한 1차 함수
                （직선방정식）
                      로 표현 가능


                                            x 1nPUt nabeI5

        x     labels
        1       3
        2       5
        3       7
        4       9
                                              心
        5      11
                                        쑤
        6      13
        7      15
        8      17
        9      19
       10      21
                                  2                          8   9   l.




＠임베디드 전문가 그룹 윌텍           -34 -       무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 32 =====
2부. 머신러닝 기본                       1과. Linear Regression




 임베디드 전문가 그룹 윌텍
C）                - 35 -   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 33 =====
2부. 머신러닝 기본                                   1과. Linear Regression


 Step2: Cost Function(1)
  @A-D의 직선 중 lab이들을 가장 잘 표현한 직선은7
  .직선C   -3
              label들과의차이가가장작음
                                    200L7.5
   鬱 실제 직선과 lab이의 차이 수치화 필요         15.。




                                                                      'I
C）
 임베디드 전문가 그룹 윌텍            - 36 -   무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 34 =====
2부. 머신러닝 기본                                            1과. Linear Regression




  @ Cost Function으로 ' Average Error"를 선택했을 경우의 문제점은？




   ● 결과 분석
    ,1- A가 abel＄에 가까운 결과를 내는 Hypothesis이지만 cost는 B가 더 작은 값으로 나옴
    4. 이를해결하려면？ 4 Error를제곱하여 평가！                  (      才 7凡      '-


   ·Mean             r(M9
                  Err。
            Squared
    4. Error 제곱의 평균
    4. Linear Regression의 Cost Function으로 많이 사용




                      小L 범D' d> Cc)
                       七：了t
                         （슨t쵸
      /7)             홴C· ,   .
      U(                  동面    가匈釀十ㄴ－串）4 t 9(

                               c 立 乂〔LU庠 十ㄴ귐. )


                      〃（:
                               = 쵸（山仗＋L－打
                           ,




      （互）             ＼ 뇨
                      《j勺




＠임베디드 전문가 그룹 윌텍                        - 37 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 35 =====
2부. 머신러닝 기본                                                        1과. Linear Regression


 Step3: Learning algorithm AI                                             CODEXPERT
                                                                          임베디드 전문가 그룹 윌텍


  9Machine Learning 기본 프로세스

     1.    Hypothesis설정   1   '   2.    Cost   Function설정   +   3. Learning algorithm 설1l
                                        Hypothesis으l 결과와
   데이터를 가장 잘 표현할 수 있는
       함수 H(x) 설겅                         label의 차이츌
                                       평가할 수 있는 항수 설정


  會 학습 알고리즘
  弊Cost Function의 결과
                   （=Cost, Error)
    t2- 입력에 대한 Hypothesis의 결과와 Label이 얼마나 다른 지 평가하는 함수
          x Cost가 클수록 Hypothesis의 결과와 Label의 차이가 큼을 의미
                                                     （封휼 今록 警용）
    4- Cost는 Hypothesis의 parameter(weight. bias）
                                               에 따라 달라짐
  .Learning Algorithm 사용 목적
    4- Cost가 최소가 되도록 Hypothesis의 parameter를 조정하는 것
    4. 조정된 Hypo卄1esis가 문제를 해결할 수 있는 함수에 가까워지도록 학습 진행




@）임베디드 전문가 그룹 윌텍                               - 38 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 36 =====
2부. 머신러닝 기본                                            1과. Linear Regression


                          （경사하강법） CODEXPERT
 Gradient Descent Algorithm                                      』＇`
                                                            임베디드 전문가 그룹 윌텍


 會 가장 많이 알려져 있는 곡선의 최저점 탐색 알고리즘
  . 다양한 minimization problem에서 사용되는 algorithm
  ● 곡선의 경사를 따라가며 최저점을 탐색

 孕 동작 과정
  ● 1. 임의의 parameter값에서 시작
  G 2. parameter룰조정
   .4 Cost갸 줄어들 수 있는 방향으로 변경
   /' 변경 기준 * gradient（기울기）
      x 해당 parameter께서의 (:ost function 기울기
  J 3. cost가 최저점에 도달할 때 까지 반복




C）
 임베디드 전문가 그룹 윌텍                        - 39 -   무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 37 =====
                                                              1과. Linear Regression


 Learning rate
             （학습율）                                                 CODEXPERT
                                                                   임베디드 전문가 그룹 월텍


  Q 성능향상을 위한 parameter 조정 시 변화 정도를 조절하는 상수
  J cost function의 기울기를 기준으로 parameter 조정
  .Learning rate 값의 설정：학습이 빨리 될 수 있도록크게 설정 한다면？
                  쀼 / Ca랒 釉nctm'1


                                            毗쁘브J7                   ming rate = 2
                                            I 'I景기＝10 j \\\




                                                  w가ㄷost가 점장커지는 형태로 변함
                                                 * w가《)ptimal한 營황으로부터 발산합

                                               [ 적철히작욘값읕선택하는 것이중요！
                                                  빽：
                                                   긺，,, )I)빙샤l..
   4- learning rate가 너무 작을 경우 어떤 문제가 있을까？




＠임베디드 전문가 그룹 윌텍                     -40 -   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 38 =====
2부. 머신러닝 기본                                                               i과. Linear Regression




  ?Parameter 조정 방법：Cost function의 기울기를 기준으로 조정
   G 기울기：미분을 통해서 얻어 냄：다수의 parameter 4 parameter별 편미분



  'Cost ' "" "" "":w,    C。   st functi。
                              bOll     n Cflj        花
                                                     C。             j) 11)2
                                                              parameter)
                                                                Ii(;  -




                    ,'               :          닌' ，구H거 +d"
                         크드쁘뵤스쏘：?                           맥 地’·0叫 기가S ,
     읒tI긔 졀ㅈ긱毛                b`D


     면켬）
       ':                     tZ )년 (「I 《 , 【
                                            '1 , ]

   準旦ㅛ 三씀斗 ！뿌
                        二 乂Hi) 乂먀小小 , 油，
                                       盼1甲尸니사             -=i5-

                              펫尸X孔－幻 · 仄


＠임베디드 전문가 그룹 윌텍                                     -41 -    무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 39 =====
2부. 머신러닝 기본                                          1과. Linear Regression




   唾 전제조건：Local minimum -     Global minimum
    ii- Local minimum != Global minimum 상황이 존재한다면？




@）임베디드 전문가 그룹 윌텍                  - 42 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 40 =====
2부. 머신러닝 기본                                                       14. Linear Regression




              [Source: suniIangirbIog.wordpress.com/2018/12/03/the-outIine-of-gradient-descent ]




    QT色 = g-kzk 戚f +L                Ar.




＠임베디드 전문가 그룹 윌텍                     - 43 -       무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 41 =====
2부. 머신러닝 기본                                                                                                           1과. Linear Regression

                                                                                                                           CODE A PERT
 Code: Optimize Hypothesis(1)                                                                                              임배디드 전문기 그룹 윌텍

  Q［예제 1] Gradient Descent 방식의 Training을 진행하는 코드 분석
  # Input and Labels..                                                 .
  x_input = np.arraytLl, 2, 3, 4, 5, 6, 7, 8, 9, 10J, dtype= np.f10at32)  .
  labels = np.array(p . 5. 7. 9. " , 13. 15, 17. 19, 2니. dtype= np.f1oat32)

  W, B =     np.          randorn. normalQ,            np.           random. normal              ()       I parameterW,      B   (randomvalue)
  # Hy枓o卄1esis : Linear Function
  def Uypothesis(x):
    return W*x + B

  # cost,    ;(
                   Mean           Squared Error
  def     (。
           stt)
        return np.mean( (Hypothesis(x_input) - labels)**2)

  def     Gradient    y)
        return np.mean`x*I.x*w-I-(I--y))), np.mean(W*x-y+b)) I
                            (x,  ,    :,   .   ,   .         ,   ,   .           ,   ,   .   .        .   .   .   l
        R"대 iii
                                                                                     n二；
            (？帥0,'）나，立(z,(xw+(b-y,)))
          :；「.                                                                       ' 方1cost(w.b)＝ㅉ                     r- y+ b)




＠임베디드 전문가 그룹 윌텍                                                          -44 -           무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 42 =====
2부. 머신러닝 기본                                                       14. Linear Regression

                                                                         COCE         T'ERT
 Code: Optimize Hypothesis(2)                                            임베디드 전문가 그룹 윌텍

  @ Training 진행단계에 따른 cost 및 parameter의 변화
  # Parameter Set                                                    느
  epodis = 5000                     epochs
                                         （학습회수）
                                              . 학습율
                                                  （걱당히 작은 값）
  learning_rate = 0.005




                                                              -
  #, 학습 (Training)         ,      .
  Tor즈flt 1P ranget),. .叩?cns+U=
     it cnt 乍,, 19?9chsll깼t- , , 0三 , , ,, , .     ..      ,.
       print(. "나 ncost=나／밂＝U ,8=n一 .tormat驛nt.(ost( J .w,BjJ

      grad_w, grad_b = Gradient( x_input, labels)                                8         .



                                                            w조정     TI' = w 가L- ---cost(L났）
                                                                                          )
      W -= learning_rate * grad_w                                              (7雄
      B -= learning_rate * grad_b


                                 쀼 쀼 쀼
  [     0] cost =      290.8,            -0.4783, B = -0.8653
                                                                     r"' Training진행중
                                               -




  [   2501 cost =     0.2772,              2.163, 8 = -0.1373
                                               -



                                                                         Weight I Bias I Cost
  [   500] cost =     0.1639,              2.126, B = 0.1254
                                               -



                                                                             변화 확인!


                                 恥 斟 닢
  [ 45001 cost =    3.673e-05,             2.002, 8 =
                                               -
                                                         0.9869
  [ 475이 cost =     2.172e-05,             2.001 , B =
                                               -

                                                         0.9899       '" 목표Weight I Bias
  [ 50001 cost =    1.285e-05,             2.001. 8 =
                                               -

                                                         0.9923       l   w= 2, b= 1     ,




＠임베디드 전문가 그룹 윌텍                            -45 -     무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 43 =====
2부. 머신러닝 기본                                                 1과. Linear Regression




  @ Gradient 동작을 수행하는 다른 유형의 다음 코드를 분석하라
  def Gradient(x, y):
      g1obal 甘. B
      pres_w, pres_b = W, B # W,B bac
      delta = 5e-7 ［刃 0얘가끄湛수C
     IN = nrne     뿌 -I-. tin14-,    ^,,「 ,,‘,

     h,;i“，
         eㅍw0t
           ，’;.三，
              l;;",
                lta" C。
                     和，
                      ,stfuncti。
                        w01ICHj
                              n
     costJII = t-ostl '
     grad_w = (cost_p-cost_.)I (2*delta)
     斗 = pres_w # w restore

      B        pres_b        delta
                             ()
                        +,
      c。st_ p =    C。   st
                   b
          =t
        st므res_         -




                st ()
                             delta
     c。   m =      C。
     grad_b = (cost_p-cost_m)I (2*delta)
     B = pres_b # b restore




＠임베디드 전문가 그룹 윌텍                             - 46 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 44 =====
2부. 머신러닝 기본                                                              1과. Linear Regression

                                                                                  CODEAPERT
 Linear Regression: 혈압 예측 Exam이e                                                  임베디드 전문가 그羈 윌텍




   나이
    （years)   혈압
               （mmHg)
      25        118
      25        125




      45        130
      55        122
      55        125




      65         130
      73        125.5

      73        138     F Source: https:f/nhiss.nhis.or.kr/bd/ab/bdabfO03cv.do]




＠임베디드 전문가 그룹 윌텍                          -47 -         무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 45 =====
2부. 머신러닝 기본                                                         12F. Linear Regression


                                                                                임베디드 진 문기 그룹 윌텍


  . ［예제 2] 혈압 예측 모델 설계 프로세스

  C 1.Hypothesis설정I1*12. CostFunction설정 Learning 3.Algorithm을
                                                      Training

 ［뺙"’聳潟，   驛‘下 , 1abe12.Hypothesis
                             l 2 '2f9.t                        적용하여
                                          Parameter w, b를Optimize

    # Input(AGE) and 1abels(BP)                                                 ,
    x_input=np.array([25,25,25,35,35,35, . ..65,65,73,73,73』,dtype=np.float32j
    labels=np. arrayn118,125,130,118,126      125.5,130,138j . dtype=np. float32)

    # Hypothesis : Linear Function
    def Hypothesis(x):
                                      [   H   (x)   =   wx+ b   ]
      return 닐*x + B

    4, Co莎 = ,1ean Squared Error
    aei- Cost` j :
       return np.mean((Hypothesis(x_input) - labels)**2)

   # Gradient
   def Gradient(x, y):,    .   ,..           ..         .,            w＝   秘，      〃乳ost   (w,   b)
     return np.mean(x*`x*m `B-yJ , J . np.meanuW*x-y-f-I) .1




 임베디드 전문가 그룹 윌텍
C）                                     -48 -            무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 46 =====
2부. 머신러닝 기본                                                       14. Linear Regression


  Code: Optimize Hypothesis(w, b)(1)                                       임베디드 전문가 그岳 윌텍

  @ Training 진행단계에 따른 cost 및 parameter의 변화
  # Parameter Set
  epomS = 100
  learning_rate = 0.01

  # 학습 (Training)
  for cnt in range(0, epochs+1》 ：
    if cnt % (epochsll20) = e:
      print( '[{)]cost={},W={},B={}',format(cnt,costQ,W,B))

    grad_w, grad_b = Gradient(x_input, labels)
    W -= learning_rate * grad_w
    B -= learning_rate * grad_b
      01 cost = 1.168e+04. W = 0.3765. B = -0.438
      51 cost = 1.706e+18, W = 493e+07, B = 4.516e+05    r∼
     101 cost =  2.84e+32. W = -3.e+14. B = -5.827e+12        Cost 값이 점점 커짐《즉. 최적화 안 됨）
     151 cost =       inf, 뽀 = 4.le+21. B = 7.518e+19                * 무엇 때문일까？
     201 cost =       inf. W = -5.e+28. B = -9.7e+26
     25j cost =       mnt. w =     mnt. B = 1.252e+34                                      …八
     30] cost =       nan, W =     nan, B =     nan           * inf: infinite. nan: not a number

    leo] cost =       nan, W =     nan, B =     nan


                                                                                                   쌔 크




 임베디드 전문가 그룹 윌텍
C）                                     - 49 -    무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 47 =====
2부. 머신러닝 기본                                                  1과. Linear Regression

     ＾. r, .`+:-:-` ．」. . ．∼｀'l∼一＝,J. ' . .'ti- ,
 rm^＇』                                                             CODEXPERT
 ㄴuuㄷ· JIJLIIIIILe nypULIIe)I>`VV, LI八U/
                                                                   임베다드 전문가 그룹 욀텍


  Q Training 완료 및 Prediction: 학습하는 이유 + 예측을 위해서
  I epochs = 200000, Jearning.j-ate = 0.0005 인 경우의 학습 결과
   n00001 cost =       541. 0. W =     1.469. 8 =    46.0
   [2000이 cost =       208 . 9. W =   0.9523. B =   74.51
   [3000이 cost =       87 . 34. W =   0.6398. B =   91. 76

   [190000] cost =      17.07. w =     0.161. B =    118.2
   [200000] cost =      17.01, W =    0.1609, B =    118.2   w 볍0.1609. b= 118.2



  . 나이가 50인 경우의 혈압 예측
                    （학습한 모델 사용）
   # Predict
   def Predict(x):
       return I-Iypothesis(x)

   age =, 50.0       . .     ,    .,        .         .. .   ..,
   printr" 나 Years : t :1/.4Jmmug "" .tormat(age, Prea1ctcage)))

   50.0 Years :    126.2mmHg




＠임베디드 전문가 그룹 윌텍                          - 50 -     무단 전재, 복제, 발췌, 디지털화 금지


===== PAGE 48 =====
2부. 머신러닝 기본                                                  1과. Linear Regression


 Code: TensorFiow I반 Linear Regression(1)                           임볘디드 전문가 그룝 훨텍

  @ [예제 3] lensorFiow 기반 Linear Regression: H(x), CostO
 import numpy as np
 import tensorfiow as tf        tensorfiow load만추가되었고. 나머지 코드 동일
                            `


 Drint("NumPv Version :{}".format(no. version 1)
 priat."" TensorFiow Version : U " . tormatltt._version_})

 # Input(A6E) and Labels《1W)
 x_input=tf.constant([25,25,25,35,35,35, . . .65,65,73,73,73],dtype=tf. t10at32)
 laDels=tt. constantun8,125,130,n8,126, . . . , 125.5,130. 138J , dtype=tt . tloat32夔


  #닐B
    Weights      ,                                           .  .      .
    = tf.Variabie(tf.random.normal(U), dtype=tf.f10at32) ㄴb蘇te 侈乂ol *2_ _
    =tf. Variable(tf.random.normal(()), dtype=tf.float32)-J,,－…뵤珖t',j e읠－ .

 def Hypothesis(x):                                    - H (x) = 切劣 + b     m
   return x*W + B # tf.add(tf.multiply(x, w), B)                   1
                                                        eost(w, b) = ,
                                                                    스＞ㅍ(H(x?) - yj)2
 def Cost():                                           ，∼
                                                                       i -- 1
                                                                       '-   工




   return tf.reduce_mean(tf.square(Hypothesis(x_input)-labels))

                d김헝긋형LL
                     '-U 古뱌




＠임베디드 전문가 그룹 윌텍                        - 51 -   무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 49 =====
2부. 머신러닝 기본                                                     1a-F. Linear Regression

                                                                      COO
  Code: TensorFiow J반 Linear Regression(2)                            임베다드 전문가 그룹 윌텍

  Q lensorFiow 기반 Linear Regression: Optimizer
   eModel을 Training하기 위해 사용하는 class
   .lensorFiow는 다양한 Optimizer 제공：ex) optimizers.SGD
    * Gradient Descent Algorithm 기반으로 최적화
                                        （Optimize）
                                                 를 진행하는 Optimizer
    fZ tf v2.17.0 부E1 keras 3 지원 - minimize method deprecated
       x tf_keras.optimizers -* keras 2.17 version
  .Optimizer의 사용 방법

              1. Optimzer쩍1            -       2. Optimzer唾이용하여최적화진행
      L0pt imizer의 Learning rate설정                     minimizeQ 이용

   ● Optimizer 생성


                                   # 학습상황OH 따라 조정
                                   # 학습상황에 따라 조정
                           . SGD( 1.earning_rate=learning_rate)




@）임베디드 전문가 그룹 윌텍                      - 52 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 50 =====
2부. 머신러닝 기본                                                                 14. Linear Regression


 Code: TensorFiow I반 Linear Regression(3)                                               임베더드 전문가 그룝 뭘텍


  磅TensorFiow 기J Linear Regression: Training
   for , cnt , in range(1, , epochs+i) :
                             鍔t,
       'F 드at , j ,, 주루
                     （． 們as'／   ==｀之 r,,,
         print`J1nC9Sr=iI7￦＝H中＝i ' · ',
                  rormdtlcnt,tostl.;,w.numpy`;        ,B.numpyQ))
                        2;＾갼 γdd`
       optimizer.minimiz하枋云r,[w,      B])
                               ',［뿌 . B])            f－귄ost를최소환하는봐할으로

                                      〃兀；  -J,,,
                                      ＇∼뉵r戶 '               variables 1W[B1츠i-
   0     inimize(Ioss, var_list)
          ·   느' ·     ，· 낟1     없어야하～' var_list는 최적화할 변수목록                  list또는tu이e『’ 전달

       4. 낸붓르르롯tf.GradientTape2f apply_gradients0量사욜
   [ 7500     cost =           589.8, W =      1.528, B =    42.71 1
   El59으9] cost                249.0, W ==     1.031. B =    70.17 <
   1225U
       （시 cost                 111.0, W =     0.7145, B =    87.64 \

   ！꼇5으與］ cost                  17.07, W =     0.162, B =     118.1 희
   11큔/쁘이 cost
   토Th0wuuJ cost
                                17.07, 쀼 볍＝
                                17.07, 맞 =
                                               0.162. B =
                                               0.162, B =
                                                              118.1 :
                                                              118.1     -     w=   0.   152.   b=   118.1




@）임베디드 전문가 그룹 윌텍                                 - 53 -      무단 전재, 복제. 발췌. 디지털화금지


===== PAGE 51 =====
2부. 머신러닝 기본                                                                          14. Linear Regression


깊。      de:       lens。     rFi。
                               w기반Linear           Regressi。               n   (4)    －「
                                                                                                   「三        '.
     @ lensorFiow 기반 Linear Regression: Prediction
     # Predici                                                                         ]
     def Predict(x:                                                                    i
       return Hypothesis(x, numpy)                                                     ㅣ

     aa =, '"ri
            50.        . .     .                              -
     DrintU tt! Year : { :>7·.4JlnmHg .rormatage., rreaictagn》

      50.0 Years :        126.2mmHg


     G NumPy 코드와 Tensorftow 코드 차이점
        구분                       Numpy                                     Tensorfiow
       Data,set                                                   .., Param: tf.Varia,             e
          &. '                   0」
                                  0「카
                                  「
                                                                  Input & label: tf.c。
                                                                                         ,b   ,l
                                                                                                        ()
                                                                                     nstant
                                                                                                             ()
                                 ndarray
       Param

       ..     '           np 연산자 및 np method 사용                tf method 사용  （np 연산자도 사용 가능）
              '               np.mean( ), *. +                     tf.reduce_meanO. tf.square()

       Training                  직접 구현                          제공되는 Optimizer, minimize 사용




 임베디드 전문가 그룹 윌텍
C）                                            - 54 -            무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 52 =====
2부. 머신러닝 기본                                                                         l과. Linear Regression

                                                                                                 DE 立 PERT
 Multi-variable Linear Regression                                                            임베디드 찬문기 그룹 묄텍


  ｛걍 더욱 정확한 혈압 예측을 위해 BMI
                        （체질량지수）입력을 추가한다면？
    나이       B1네    혈압
   (years)         (mmHg)                               나이. 체질량지수. 혈압의 관겨1
     25      22     118
     25      26     125
     25      30     130
     35      22     118
     35
     35
             26
             30
                    126
                    123
                                    鰲
                                                                                                        0
                                                                                                        3
     45      22     120
                                                                                                            튠m
                                                                                                        5
                                                                                                        2
     45      26     124                                J5
                                                                  45
     45      30     130                                                      5:
                                                                                        55
     55      22     122                                                                            '3

     55      26     125                                                 나이
     55      30     130
     65      22     127               覩 105-110 · i.io-iis   必 115-120 驪 120-12f   1125-130 1130-131 1135-140
     65      26     130
     65      30     130     일반적으로 BMI 1증가 시 혈압 0.8-1.7mmHg 상승 (170만명 대상 조사결과）
     73      22     125.5   [Source: medicaIxpress'com/news/2018-08-body-mass-index-bood-pressurehtmI I
     73      26      130
     73      30      138    [Source: https://nhiss.nhis.or.kr/bd/ab/bdabfO03cv.do I




＠임베디드 전문가 그룹 윌텍                                - 55 -          무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 53 =====
2부. 머신러닝 기본                       14. Linear Regression




＠임베디드 전문가 그룹 윌텍   - 56 -   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 54 =====
2부. 머신러닝 기본                        14. Linear Regression

                                        COD;KPERT
                                        임배디드 전문가 그룹 윌텍




@）임베디드 전문가 그룹 윌텍   - 57 -   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 55 =====
2부. 머신러닝 기본                                                                                     1과. Linear Regression

 Hypothesis of Multi-variable L.R.(3)                                                                CODEXPER
                                                                                                     임베디드 전문가 그룹 윌텍




                                          :{
  @ Matrix Shape
                                                    -I
                                  a:11         12
                              +                                                                   +b
                 H (X) =          劣21
                                                                       H2lWl 卞X22W2 +〃，
                                                                 bbb = I :r31끄柱 낙－ X32W2 十 O
                                                                        巨11w1          +X12W2
                                              Z22 - ,
                                              a:         w2
                                  石31
                                  -   -
                                              J=32

                                                                                        (3. 1 )
                                                                        夫의
                                                                       .(Batch Size
                                                                        （일괄처리 개수）




           31
                ;;
  . Matrix Shape Example: 다음 Matrix의 Shape은？
     ;ii
           21    Z
                 Z
                  12


                       X3
                         13
                         23
                                  102
                                          +
                                                b

                                                ,,b
                                                                                      x         w = H (X)
           41     42   X43                                                      -




                (4. 3)        (3.1)
                                                         +"
                                                          '


                                 일반화하면＋( 1 . m) · (m . k) = ( n , k)
   介 Matrix연산：(n, 3)·(3,2) =(n .2）
                                                                                    (5, 3) 9.!) (5,1)




 임베디드 전문가 그룹 윌텍
C）                                                            - 58 -    무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 56 =====
2부. 머신러닝 기본                                                      Linear Regression
                                                               1과．

                                                                   C各各瑟；
                                                                      4_ - --
                                                                          入弘瑟RT
                                                                              -.
 LAB: Muti-variable L.R.(TensorFow)(1)                             임배디드 전문가 그룹 웡텍


  @ [예제 4] Input(age, bmi) and Label(blood pressure)
 #Input(AGE) and Labe긔S佃바．.          .                                     .
 x_input=tf. constan妖LL25《2기[25'26JJ25,30]－…[7乳3011,dtype== tf. float32)
 1abe1s=tf. constant([[118L[125L[130], . .. . L1381],dtype== tf . float32)


   . 구현：Wei야，
            tand Bia` 생성
    ,4' x_input 과 matrix m미ti이ication 연산 결J뛰abet$ 가 나오도록 W. B의 $hape을 결정
    /' 아래 연산의 勍ape을 완성하라

                         b        xl1Wi + x12W2 + 6
                 松'
                         b   ==   客2ltz7l + X22W2 + 6
                  W2

                                       (   .   )

      쁘B = 난．
            yaria아e(tf.ranqom.nornia긔f!            )). dtype
        = tt. Var].a01e`tt. ranaom.norma趣츠         " . dtype




＠임베디드 전문가 그룹 윌텍                        - 59 -      무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 57 =====
2부. 머신러닝 기본                        1과. Linear Regression




@）임베디드 전문가 그룹 윌텍   - 60 -   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 58 =====
2부. 머신러닝 기본                                                               1과. Linear Regression




 training_ idx         np.     arange     1)
                                         (0,   epochs+   1,   1)
 c。 st_
      graph
             =   np.
                 =p
                             zer。s(ep。chs+

 for cnt in range(O, epochs+1):
   cost_grapt,flcnt.j =. .Co듕tU
   it cnt ! ,, 19〔l9cI'is/I찢t== , 覃：
                                   ,,,  ,. .,
     pt:int;.꾸 fl COSt=tJ,W＝너it U ，多＝  ,U", . ,    ....
     .tormat(cat,cost_graphb:ntL吼8,0』.引1-01-B.numpy(}"




＠임베디드 전문가 그룹 윌텍                                          - 61 -    무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 59 =====
2부. 머신러닝 기본                                                                            14. Linear Regression


  LAB: Multi-variable L.R.(TensorFlow)(4)                                                           익배디드 전 문7! :l룹 웠텍


  @ Training 결2F Test, Prediction
 H_x = Hypothesis(x4nput) .,                       , , , ,.                          . Training에ㅅ陪한data로검증
 Tar x,n, ,j., in . z1px_input,,,ii7x , .iaoeis;.
   pr1nt`
       ./..^ge .· it 'iL Ii'!' · t 了=jisr · i /【 .Laoei.=,'t n ,, r
                           .....u                                .rormat\
                                                                       - .i xr,
                                                                             U玎i ,XLr.I j ' .n r.
                                                                                               U:..1
                                                                                                 U ' -,
                                                                                                     ㅗ' '

 x_test..= tf,.constant([[50.0, 25.01], dtype= tf. float32)
                                                                 귑t盤 콰 예측
 11_x = Hypothes1sI,x_testJ
 print("Age:{},BMI: {}=>Bp: {}".format(x_test[e,ol,x_test[o,l],H_x[o,o]))

 eee
                                        B8B
        25.0, BUI :           22.e =>            116.8 [label => [118.]]
 gAg^
    g
                                          。
 A
                                          1
        25.8. B甘I :           26.e =>            121.8 [label => [125.]]
                                          p
                                          1
        25.0. B目I :           3e.e =>            126.8 [label => [130.]]
                                          。
                                          1
                 eeo
        3 3 nj
                       IgI目
                          I             P
                       K
                              2z.0 =>            125.2 label => [125.5]]
                                        B1B1B
 Age        ,
                                                                                                  Coot F Epocho GtoPh


                                         D
                                                          '


        7 7 7          8 BB                p
                                                                                 따
 Age        를                 26.0 =>             130.2 [label => 1130.1]
                                                          '

 Age        ·                 3o.e =>           !135. 2 [label => m8.]]
                                                          '




 [ Prediction by specific data ]
 Age : 50.0, BUI : 25.0 => BP : 124.9


                                                                                        ir目.{}0    기》
                                                                                                    .00(}     女好D(10    *好｛X0   mX｝
                                                                                                                                  허｝
                                                                                                        Ep.Ch5




＠임베디드 전문가 그룹 윌텍                                        - 62 -       무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 60 =====
2부. 머신러닝 기본                                                           1과. Linear Regression
 「빤
 「…“∼－…땀－륵생群∼－-                                    蜀多
 Code: Multi-variable L.R.(TF)(1)                                          임베디드 전문가 그룹 윌텍


  Q［예제 5] 학습효율 향상을 위한 Data의 Normalization(MinMaxScaler)
   S Cost 값의 발산으로 Learning Rate를 낮게 설정해야 하는 문제를 개선
   . x_input 값을 0-i 값으로 resc히e
     # Uin Max Scaler
     x_input_org = x_input,# 나중oil 원본[hIo'터 확인을 위해 백업．
     x_rnin, x_ma. x = np.min(x_ .nPut, axis=Oj( np.max(x_input, axis
     x_lnput = I. x_lnput-x_min)It.x_max-x_min)
   S epod,5= 5000, learning_rate = 0.01 4 Cost 발산 없이 학습 속도 개선




                                     l[[ ［蓼［
                                                               BB B
    [     0] cost   1.602e+04, * =        0.2148 -0.8582         = o. o5116
    [   25이 cost        151.9. W =         33.01   28.16         =    92. 86
    [   500] cost       65.39. 벌 =         25.04
                                               -
                                                   19.96              181, 9


                                                               BBB
    [ 4500] cost =      5.265, 멓 =             7.741
                                               -
                                                       8.426           118.0
    [ 47501 cost =      5.265, * =             7.733
                                               -
                                                       8.422           118. 0
    [ 50001 cost =      5.265, 쀼 =             7.729
                                               ㅡ
                                                        8.42           118.0
    Wall time: 6.27 s




@）임베디드 전문가 그룹 윌텍                         - 63 -        무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 61 =====
2부. 머신러닝 기본                                                                                                                                                       14. Linear Regression

                                                                                                                                                                       C0DE
                                                                                                                                                                       임베너드 자무가 그룹 윌ElI


  @［예제 5] Training 결과 Test
  . 입력 데이터와 Regression 결과 그리고 Lab이을 출력하여 결과 확인
  H_x = Hypothesis(x_input)                   , , , ,
  tar x,fl,.L, en 끗plx_1r)Put_or9《 ,H_x,,[a. 9+s);             . , . ,,, . , , ,,.
    prentt " Age= t } .I:1甘i = 나＝入；P= t nlabe1==2나 j " . tormat( xU시,xt1Lm町 , I. J J

  x_           input
                                         4 0-                     1값으로rescal.
                                                                                             한데이터，     xJnput_
                                                                                                                                     org* 원본데이터
                                                                                                                                              （출력을위해백업해놓은뎨이터）                      -

                                                          oo8oo                                                                                        →今→ →→
                                                                                I1 III

                                  m
                                  z `
                                    < 2 `j 갸J
                                                                                                       －溺고label


       디e e e e e e e e e e
                                          ( J ＜ 구 CJ `J
                                                                                         22.0 => OP
                              '

                              1




                                                                                         26.0 => BP              122.2 ilabel
                              .




                                                                                얘刪炚매昨
                              1




                                                                                         30.0 => 미：.             126.4 蠟label
                              1

                              .




                                                                                         22.0 => BP              119.6 ilabel
                              1

                              ·




                                         `J
                                                                                         26. e => OP             123.8 f label
                              ,

                              *




       忖勿勿勿勿 勿勿勿勿勿勿
                       : 65.0, OMI                                                       22.8 => OP              124.
                       : 65.0. 炚I
                       : 65.8. B甘I
                       : 73.o. 8肛
                                                                                         26.0 => OP
                                                                                         30.0 => 0p
                                                                                         22.0 => OP
                                                                                                                 128. 7
                                                                                                                     5哥label=
                                                                                                                 132. 9
                                                                                                                          =
                                                                                                                 125.7 label >
                                                                                                                                l(label
                                                                                                                                          label
                                                                                                                                                  =>
                                                                                                                                                  =>
                                                                                                                                                       >
                       : 73.8. B甘I                                                       26.0 => 0P
                       : 73.0. 얘I                                                        38.0 => 0P              槍聊｛label
                                                                                                                   41abe1 =;     [
                                                                                                                                -




＠임베디드 전문가 그룹 윌텍                                                                                                      -64 -                                 무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 62 =====
2부. 머신러닝 기본                                                1과. Linear Regression

                                                                 CODE，臂X꾸轍PERT
 Code: Multi-variable L.R.(TF)(3)                                 밈뻬口느 진너77! 그〔＝; 획텍


  @ E예1I 5] Prediction(MinMaxScaler)
   . 예측할 데이터를 Mmn Max Scaling 후 사용
  idef predict(x),: . .,   . . ,.        -
  L return Hypothes1sUx-x_min)/(x_max-x_min))
  x_test = tf. constant([[50.0, 25.01], dtype= tf. float32)
  H_x =. prec11cttx_test) ,        . , ,     ,,..
  print1:'nI 싸eg프tion, 型 듕Pec촌i-ic a9ta J "" ),    .         ,    ,     ,  ,..
  pr1ntU ""Age= 나,BNI: n=2BP: tJ" .tormat(x_testW,0j . x_test10, U . H_x[0,이Jj


  [Prediction by specific data I
  Age : 50.0. BMI : 25.0 = > BP =   125.2




C）
 임베디드 전문가 그룹 윌텍                       - 65 -   무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 63 =====
2부. 머신러닝 기본                                            14. Linear Regression


 Multi-variable Multi-output L.R.(TF)                       임畔디드 전문가 효룹 윌텍


  l'? 나이와 BMI를 입력하연. 수축기 혈압과 이완기 혈압 예측
                   수축기혈압 이완기혈압                          수축기혈압    이완기혈압
   （years)
  나이         BMI                       （years)
                                      나이         BMI
                   (mn꺼g) (mn汨이                         (mmHg)   (mmHg)
    25       22     118    72              55    22       122      78

    25       26     125    80              55    26       125      80

    25       30     130    80              55    30       130      81

    35       22     118    76              65    22       127      75

    35       26     126    75              65    26       130      79

    35       30     123    79              65    30       130      81

    45       22     120    80              73    22      125.5     80

    45       26     124    85              73    26       130      80

    45       30     130    83              73    30       138      82


  ● 여러 개의 입력에 따른 여러 개의 출력을 예측할 때 사용 가능




 임베디드 전문가 그룹 윌텍
C）                                - 66 -    무단 전재, 복제, 발췌, 디지털화 금지


===== PAGE 64 =====
2부. 머신러닝 기본                                               14. Linear Regression




   #Input(AGE, BMI) and Labels佃IGH, lo帥

   x_input=tf슨
   labels=tf .c。
               consta
                nstan盼125,22
                       118,72儡261
                               .8。1" " 173,30.
                                        [138,8211,
                                             1]j]dtype
                                                   dty謐f1oat32)
                                                        f f1。at32)




     = tf. Variable(tf.rando,n.normal( (2,. 2)), dtype=tf.f1oat32)
     == tt. VariaOiettt.ran《】om.normalu2, " . cltype=tt. tloat32)

   0 나머지 부분 이전코드와 동일




C）
 임베디드 전문가 그룹 윌텍                      - 67 .   무단 전재. 복제. 발췌, 디지털화금지


===== PAGE 65 =====
2부. 머신러닝 기본                                                                   1과. Linear Regression

                                                                                    O#E
 Code: N-variable, M-output L.R.(TF)(2)                                            임베다드 진：푸‘가 」룹 윌텍


  . ［예제 6] Training 결과 Test
   . 입력 데이터와 Regression 결과 그리고 Lab이을 출력하여 결과 확인
 H_x = Hypothesis(x_input)             . , . .
 b0r x,I1,.L in ziptx_iflut_.or9( ILx, iaoeis),=.,        . , . . . . . . , , , ,..
   pr1nt( "Age= 냐,BMI= U=2바｝=나 . U[laflel=,)나j "' . tormat(x〔Uj ，x
                                                                 【1 j 'Fn自U .hi 1 j ,1JJ

                           h18.J                                 ,o e b o
                                                                쨍＇8 8b   。8
 Age:25.0, BMI:22.0=>BP:            75.79 [label =>    1 t8.

                                                               ／
                                                               八        7
                                                                         ,




                                                                     '／
 Age:25.0, BMI:26.0=>BP:   122.2.   77.87 [label =>    125.              1




                                                                       쨍
 Age:25.0, BMI:30.0=>BP:   126.4,   79.96 [label =>    13o.              ·




 Age:35.0, BNI:22.0=>BP:   119.6,   76.34 [label =>    118.

                                                                     /
                                                                     , / `
                                                                         ,




 Age:35.0, BUI:26.0=>BP:   123.8,   78.42 [label =>    125.              1




 Age:35.0, BMI:30.0=>BP:   128.0,    80.5 [label =>    123.              ,




 Age:45.0, BMI:22.O=>BP:   121.2.   76.88 [label =>    120.              *




 Age:55.0, BNI:30.0=>BP:   131.3,    81.6 [label =>    130. 81. 1
 Age:65.8, BNI:22.0=>BP:   124.5,   77.98 [label =>    127. 75. ]
 Age:65.0, BMI:26.0=>BP:   128.7.   80.06 [label =>    130. 79. 1
 Age=65.e. BUI:30.0=>BP:   132.9.   82.14 [label =>    13o. 81. 1
 Age:73.0, BMI:22.0=>BP:   125.7,   78.42 [label =>    125.5 80. j]
 Age:73.O, BMI:26.0=>BP:   129.9,    80.5 [label =>    13o. 80. ]
 Age:73.0, BMI:30.0=>BP:   134.2.   82.58 [label =>    138. 82. 1




＠임베디드 전문가 그룹 윌텍                          - 68 -       무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 66 =====
2부. 머신러닝 기본                                                                                               1과. Linear Regression


 Code: N-variable, M-output L.R. (TF)(3)                                                                       임베디드 찬문가 그룹 윌텍


  《코［예제 6] Prediction
              G 예측할 데이터를 Mmn Max Scaling 후 사용

      defprecIict(x):- ' ·’·“' " 山" " "山"－…－-l
  i            return                  Hypothesis((x-          x_
                                                                    inin) /(x_max-    x_   min)
                                                                                                    )-i
      print( "\n[ Prediction by specific data 1")
      x_test = tf. constant([[50.0, 25.01], dtype= tf. float32)
      H_x
                                         {}              { }=>BP:{} {}"
                                              (x_
                          predict
                 =(
      print           (
                               "Age:           ,BMi:
                                                       test)          ,


               .f ormat( x_test[0,0], x_test[0,ii , H_x10,0]. H_x[0,1)))

      [ Prediction. by specific data I                                      ,M .           - -.
      ^ge . .17·u7 bH主 · z ·心 = / br .                                      괄L놀. z'        I6. /L




＠임베디드 전문가 그룹 윌텍                                                                - 69 .             무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 67 =====
2부. 머신러닝 기본                                       24. Logistic Regression




                    2부. 머신러닝 기본

        1邕 Linear Regression
        221. Logistic Regression(Binary Classification)
        32卜，Softmax ClassificatioMMuttinomial Cias尉ication)




 임베디드 전문가 그룹 윌텍
C）                             - 70 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 68 =====
2부. 머신러닝 기본                                       2과. Logistic Regression

                                                         CODE晟PERT
 Linear Regression vs Logistic Regression                임베디드 전문가 그룹 윌텍


  @ Linear Regression
   . 주어진 입력에 따라 Continuous한 결과 값을 예측                   //(.rj=   W.   V +   1
  口 나이에 따른 혈압. 공부시간에 따른 시험점수


  孕Logistic Regression(Binary Classification 동작 수행i
   . 주어진 입력에 따라 Discrete한 값
                          （일반적으로 (:lass）
                                       을 예측
   ) Binary Classification 예（특정 입력을 oil 로 구분）           Ji(.i:) E { O. I }
    4. 나이와 B卜川 수치에 따른 고혈압 여부：고혈압
                               （D / 고혈압 아님
                                         （0)
    /2- 메일의 스팸여부 구분：스팸 메일
                        （1) / 스팸 아닌 메일
                                     （0)
    4. 매입할 주식 종목 구분：오를 종목
                        （D / 떨어질 종목
                                  （0)
    '4. 신용카드 합법사용 여부：합법
                      （1) / 불법
                             （0)
    4- SNS 특정 내용 표시 여부：Show(1) / hide(0)
    '4. 영화감상 평：긍정
                （1) / 부정
                       （0)




@）임베디드 전문가 그룹 윌텍                  -71 -    무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 69 =====
2부. 머신러닝 기본                       2과. Logistic Regression




                               나이
                                （years)   .i혈압판정
                                  52      No40




C）
 임베디드 전문가 그룹 윌텍   - 72 -   무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 70 =====
2부. 머신러닝 기본                                      2과. Logistic Regression


 Linear Regression의 ! 1I                                  CODEXPERT
                                                          임베디드 전문기 그룹 왈텍


   唯 현재의 데이터를 기준으로 Linear Regression 모델링 * 선형으로 값 예측
   〃 고혈압 여부를 0.5 기준으로 판단한다면 50세 이상 이면 고혈압으로 판정



     以8



     .




          " 1i颯
   .Linear Regression의 가설 'H(x) =Wx+ b'의 결과 범위？ -OO- OO
    4. ' 나이와 고혈압 판정 여부"에서 예측해야 하는 결과값은？ 0/ 1 ( 또는 0- 1 사이의 값 )
    4. Linear Regression으로 0 또는 1인 데이터를 표현
                                         （결과값을 예측）
                                                 하는 것은 적절치 않음




＠임베디드 전문가 그룹 윌텍                 - 73 -   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 71 =====
2부. 머신러닝 기본                      2과. Logistic Regression




＠임베디드 전문가 그룹 윌텍   - 74 -   무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 72 =====
2부. 머신러닝 기본                                        2과. Logistic Regression


 Classification을 위한 Hypothesis
  Q 이상적인 Binary Classification
  . 나이가 특정 값
           （50) 이상일 때 1. 미만일 경우 0(step function)




   0 현실 데이터의 표현에 적합하지 않고. Gradient 적용이 부적절함
   0 위 모델의 특징을 가지면서 현실 데이터 표현에 적합한 Hypothesis
    4' Logistic Fun博on: Logistic Curve를 표현하는 함수




C）
 임베디드 전문가 그룹 윌텍                     - 75 .   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 73 =====
2부. 머신러닝 기본                                      24. Logistic Regression




  t Hypothesis로 Logistic Function(Curve）
                                       을 적용하여 regression 진행
  G Sigmoid Function(Standard Logistic Function의 표준적인 형태）
    4. 입력에 따라 0-1사이의 값을 출력
                         （확률에서도 사용：확률도 0-1사이의 값）




@）임베디드 전문가 그룹 윌텍               - 76 -   무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 74 =====
2부. 머신러닝 기본                      2과. Logistic Regression




＠임베디드 전문가 그룹 윌텍   - 77 ~   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 75 =====
2부. 머신러닝 기본                            2과. Logistic Regression


 Hypothesis of Logistic Regression           '11，
                                                "
  Q 데이터를 갸장 잘 표현할 수 있는 w와 b값을 학습
  0 학습：데이터를 통하여 Cost를 최소화 할 수 있는 W, b값으로 조정하는 과정




@）임베디드 전문가 그룹 윌텍        - 78 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 76 =====
2부. 머신러닝 기본                                                                                            2과. Logistic Regression

                                                                                                                            CODE ' PERT
 Decision Boundary and Logit                                                                                                임삐디드 전운가 그룹 윌텍


  @ Decision Boundary
  .Sigmoid Function의 결과를 0, 1 둘 중 하나로 판정하는 기준
                                            （경계）

               xiv + b     )C 느 〃 츠 X

                                         ∼I
                                              /-
                                                    () ＇二 77 5: 1
                                                                    y 2 a5
                                                                                      광7c {O. I }
                                                                                                           -     H    (X)        三0.  치
           CLinear-j                     Sigmoidl            뇩< feasion ,
               tquationj                J：
                                         쁘：브드므만lj                   ID므프
                                                                       【쁘쁘U


  會［참고］Probability, Odds, Logit과 Sigmoid 함수 관계
   ● 예를 들어. logit은 확률 를 구하기 위한 sigmoid함수의 입력으로 표현 가능
                    （p）
                自로                            Li-i             승뉵                 [ l。
                                                                                     g]                 釀윌짖                            季




  * Iogit(Io
                                                                        ,   . ,   .     .    . , . .    . . '.   _I   一＝     `   li
                                                                    ' prooii`prooaotit깡 十 unit). 왁曾巨 Ar
                                                                                                      '亡 냔于1                               牙




＠임베디드 전문가 그룹 윌텍                                               - 79 -                  무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 77 =====
2부. 머신러닝 기본                                                                                  22F. Logistic Regression


 Cost Function of Logistic Regression
  @ Cost Function of Linear Regression
                         r"                     H(.                                  )       " '

  r/ 'q/ L //   /n   -          (H(.x) - yi)2     r, )   =   ( l+   ,   .   WZ,+b)                             1                    , .




                                                              대입                         In곁        I +   e-   (" " ,+b)            " '/


  G Cost Function이 Non-convex 형태로 Gradient Descent 방법으로 최적화 힘듦
                                                         [Source: https://towardsdatascience.com/
                                                         introduction-to- ogistic-regression-66248243c148]




  0Sigmoid 함수를 Hypothesis로 사용하는 경우 다른 형태의 Cost Function 필요
      .4 Logistic Regression의 Cost Function 4 Cross Entropy Error AF
      ,4 Entropy: System내의 무질서도를 측정하는 척도          （Energy + tropy
                                                                （변형）
                                                                   )
         x Cross Entropy Error: 두 확를분포 p와 q의 차이 '                                                                              ,,




                                                                            cross entropy error =   m   >Dp,
                                                                                                        t==l
                                                                                                                   Iogq,
                                    t
                              雜一놔       c計이A "ㅣ 잃꺽                                                                         。
                                    0
     弗：
      乙                             i
                     盼＄\ 차누을                    c'oC 帥繃Y납




                                                                                                                                           -


＠임베디드 전문가 그룹 윌텍                                              - 80 -          무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 78 =====
2부. 머신러닝 기본                                    2과. Logistic Regression




  r걍 두 확률 분포 p, q의 차0（얼마나 일치하지 않는지）
                                  를 값으로 나타낸 개념
  臼Label(p）와 실제 Hypothesis(q) 값에 따른 Cost(CE E）
                                             값 비교
  fl -  C.E.E     『一 pl: IabeI이 1일획必 ' ㅍabel= y= pi, pO= l- pl=
  t    일반식 --J I. q1: H(x）   가 1알확률 . ` H(x) =qi, 畛＝1' qi = 1스




@）임베디드 전문가 그룹 윌텍               - 81 -   무단 전재, 복제, 발췌, 디지털화 금지


===== PAGE 79 =====
2부. 머신러닝 기본                      2과. Logistic Regression




＠임베디드 전문가 그룹 윌텍   - 82 -   무단 전재, 복제. 발췌. 디지털화금지


===== PAGE 80 =====
2부. 머신러닝 기본                                                                                                                                                                                                                                         2과. Logistic Regression

 ,-....j..· a - H =．·』．:〃口 1, ^ 'm'＾∼．
                                     . n` ·｀／ㅜ亡，
                                               /ㅓ ,                                                                                                                                                                                                           UUULA rLKI
  `-（〕 u ㅂ · LUU Ii LII...『｀eUI e> >IUI 꿸(I 【－ ' ' I '
   - - -        V - -        나           `    ' ` '                                                                                                                                                                                                            임베디드 전문가 그룹 윌텍

  Q E예제 7] Input, Labels, Weights, Hypothesis, Cost Function
   x_input=tf. constant( I [1. 1]. [2,1]. [1,21. lo. .5,4]                                                                                                                                                                                                    .

  1abe1s tf. m.
  l.          b.   t ([
              nstant
             c。,tㄻ    ［[01,
                        이
                       l,         =tf                   .                                          .
                                                                                                       E。
                                                                                                                 [4,
                                                                                                                       ], 1,dtype
                                                                                                                              [01,
                                                                                                                            1JIptf. tf. f1。
                                                                                                                                     f1oat32)
                                                                                                                                           at32)
                                                                                                                                          12.
                                                                                                                                                    [1]
                                                                                                                                                                     5,
                                                                                                                                                                          ,          [1]
                                                                                                                                                                                    2.     3JJ,
                                                                                                                                                                                                  ,       [1]
                                                                                                                                                                                                                    dtype
   W = tf.                                                                                     random. normal        ),dtype=tf.
                                                                                                         rmal((1, )),dtype=tf. fl。
                                                                                                                                                    (
                                                                                                                                                          (2,                       1)
                                        Variable                         (tf.
   B = tf.                              variable
                                                                         (tf.
                                                                                               raad。m.n。                         float32)
                                                                                                                                    at32)

             xli                    x12                                                                                .i:1I Wj + X12W2 + b
                                                                 tel
             X2i                    X22                                         『B                =                    X21Wl + X22W2 + b



      def,         ,   Hypothesis                                                                                                                                                                                                    I   l        LIIV   ,
                            i-f  infnnfr4(+
  L
             rM- iirn
             "_  -_ " "      一 "-－납                --, . f" mM-muil
                                    "' u --` Hf" ,mrItUi-          '- -(y
                                                            "'" - . ""
                                                                   (x)
                                                                       \"            :
                                                                                                                                                                                                                                  B) ) ! " `" 7
                                                                                                                                                                                                                                         ,,
                                                                                                                                                                                                                                                             1＋·－（仲’X b)


  -def Cost
     returnQtf.reduce_mean(
                   +(1-labels모els*tf
                            la *tf,math,l。
                                      math,g(1_
                                            log；므溫繼嗇；늪input))
                                                      nput)))
             cost                                                                                logH                       +
                            (W,                    b)       一츠
                                                                 772
                                                                                         (굴i
                                                                                                            (x
                                                                                                                       ')            (1
                                                                                                                                                -
                                                                                                                                                                y)
                                                                                                                                                                              log
                                                                                                                                                                                           (1         -         H
                                                                                                                                                                                                                            (x)
                                                                                                                                                                                                                                    ))        ,




＠임베디드 전문가 그룹 윌텍                                                                                                                                                      - 83 -                                                 무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 81 =====
2부. 머신러닝 기본                                                                               2과. Logistic Regression


 Code: Logistic Regression(TF)(2)                                                                 CODE7 PERT
                                                                                                  임베디드 전 문7F 그룹 욀텍


     . ［예제 7] Training
 epochs = 10000
 learning_rate = 0.1
 optimizer = optimizers .SGD(learning_rate=learning_rate)

 fDr cnt in range(0, epochs+1):
   cost araDhlcn미 = (ost()
   lr cnt 名 tenocnsi / LU I == U;
     Drint뜁 i i ' Icost=1 ' w=1 I I t 1ㅣI } t I b=I 1 I 1ㅣl
          . rormatKnt, cost_grapn[ cnt I , wIw,UJ ' Wt I, UJ,b[UJ) '



ㅣ
     optimizer.minimize(Cost, Lw, B])




                                                     n＂
                                                      ∥ H""小
                                    :！三三旦2, ":1.424]
                                             斗娑斟
                                             ：줅홰                                   BBB
                                                                                         IF 1.98511 l
     1。
      。。1
                                                  ㅣ   。-0.10
                                                        .966n]:
                                                                 -

              :，응，   :,   ;:
         0]                             4.
                                                                 -ㅡ
                                                                                         [[ -3.00기 j
      500]                                           [ 1.652]],  --
                                                                                            -5.528]]


                                             胃넓넓                                   BBB
 E 900
                ; ;;;:;;
              ；三三；
                                                           3.687]=ㅡ
                                                                        4.216]].            -14.96]]
 [ 950                                             = [[    3.745]=
                                                                        4.2821],             -15.2]]
 [   1。
      。。目！                     目；
                                                             3.8]=
                                                                        4.345Jj,
                                                                               －

                                                                               ㅡ

                                                                                            -15.43n     V




@）임베디드 전문가 그룹 윌텍                                               - 84 .      무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 82 =====
2부. 머신러닝 기본                                                                                                                                                                             2과. Logistic Regression


  Code: Logistic Regression(TF)(3)                                                                                                                                                                     GODEAPERT
                                                                                                                                                                                                       임베디드 전문가 그醫 윌텍

   每「［예제 71 Training 결과 Test, Prediction
 print( " (Traininq, Test]"),     ,.                                                                                                                                                    .Training에 사용한 data로 검증 -
 H-x = HypotflesisJx71nput).numpyU
 'l-x ' .14-x. ．·f르휀a. p빈｀-．쫠d' ,
 ㅐ = Lint(5t120.!U tor h in H_xj
 for idx in ranqe(x_input.shape[o]):

      print
       . rmat
           f。           (   "Inpt三；     (x_         input[         Label. {} idx]
                                                                [idx]          ,H
                                                                               ,   labels[          i.                    =>            .,   :{:>2}   H[      (H_x:
                                                                                                                                                           idxj.     H_   xEidx]
                                                                                                                                                                            {:>5.       2}   ))'
 print( '\n[ . Prediction. by specifi( data ]", )       ［…틀정값으로결과예측－ㅍ］
                                                          [
 x_test-.= tt,. con斗antuli·5, 31, .10.5, 2Jj, dtYPe= tt· t1oat32)       -
 브－x = .tlypotfles].돠x-test).nump놘hreshapeu-1,))                        -
 b｛》r lOx . in rang9`x_test.shapeL0j) :, .      .  .-. .      - - . ... -
   print,"Input U ＝새－x= t:25.2i'" . tormat(x_testLidxJ, H_자idx") -


                                                                                                                                                            ＞>>>＞一
                                                                                                                                                            玎


                                                                                 mm
   e. *··
            4 1




                                                                                                         芩→ →→→→               欲아이KKK
                                                ㅗ
                                                L
                                                                                                                                                                     ! Prediction bγ sp르iji드_ P2J



                                                                               喊
                                                                               mmm
                                                                     JJJㅕ a
                                                                          Jㅓ
                                                                                                               ㅐㅐ ㅐㅐ ㅐㅐ
                。
             J z`ㄴJ
                                                                                                                                  00 0
   - ，팔 ,
        1 八
          z    눼
               쬐                                                                         -




                                       ㅓ｀ j l
                                                                                                                                                             -




                                      1
                                      i
                ／
            ㄷ   ,                                            Label                                                                                                   !nput n.5 3. l 캉낸－x= (3.94 1

                                                                                         `jllJ11J
                                                                                                                                                           - 的*朽*明,
   n        04                                               Label                                                                                                    In以代 I 0 .5 z . i =); " x:                     u.uZ i

                                                                                                                                                                  l
                1                                                                                                                                                -




    .z 八14
                                                                                                                                                                   月月3
                                                                                                                                                                          "         -              =    '   `   -1       m1




                                                                                                                                  JxHJJJx
    I          z^   1                                        Label
                                                ]:
                                                                                                                                                                 -


    n



                                                                                                                                                                  ooo
   ,1 +
      , +
        L ,
          ` +  L ㅗ
             L ,  L                                          Label
                                      1곁1,
   auuuuuu
                                                                                                                                  ㅐㅐㅐㅐㅐㅐ
                                                                                                                                                           .
                                                                                                                                                           1
                                                                                                                                                                 -
                    1


                                                             Label
   竹 叩叩叩叩叩叩
                                                                                                                                                                 -
                    ·
                                                ,
                                                `
                                      ·                      Label                                                                                               -



                                                                                                                                                                 -                      -




C）
 임베디드 전문가 그룹 윌텍                                                                                                                 - 85 -                           무단 전재, 복제. 발췌. 디지털화금지


===== PAGE 83 =====
2부. 머신러닝 기본                      2과. Logistic Regression




⑥임베디드 전문가 그룹 윌텍   - 86 -   무단 전재, 복제, 발췌, 디지털화 금지


===== PAGE 84 =====
2부. 머신러닝 기본                                      2과. Logistic Regression

                                                       CODE
 LAB: 나이에 따른 고혈압 판정
                  （IF)                                  임베디드 진多가 上릎 휄텍


  @ 고혈압 여부의 판정은 Binary Classification
  . Labels + 0 또는 1
   9Linear Regression이 아닌 예측결과를 0 또는 1로 출력해야 함

    나이
     （years)   BMI    고혐압판정         나이
                                     （years)   BMI   고험압판정
               22     No40               55    22      No40
               26     No40               55    26      No40
               30     Yes 4 1            55    30      Yes 4 1
               22     No40               65    22      Yes41
                                         65    26      Yes41
                                         55    30      Yes41
                                         73    22      No40
               26     No40               73    26      Yes41
               30     Yes 4 1            73    30      Yes 4 1




C）
 임베디드 전문가 그룹 윌텍                 - 87 -    무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 85 =====
2부. 머신러닝 기본                                                                                                              24. Logistic Regression

                                                                                                                                    CODE힁 PERT
 LAB: BP Logistic Regression(TF)                                                                                                    김베디드 진 무가 그룹 윌텍


  Q E예제 81 lnput(age, bmi) and Label(O or 1)
   G x_input, Labels이 작성되어 있는 LAB 코드에서
    4' Hypothesis, Cost및 raining 부분을완성하세요
    4.［예제 7] Logistic Regression(TF) 참조하세요
     x_input = tf.constant([[2`221肛5,261,[25,3씬‘[35,22L
                                   d;
                                    113j 30JJ,[dtype tt.
                   nstant([[01  E8^
                                                                                                             t.
                                         :{,2bJj
     labels = tf. c。
     l.b.   1,              .                            loat32)
                                                          [   01   [   1]    ,   [01,        [11,     [01,        E01,    [O]   ,


                     , t } j ' 댜U , [1L " jj, atype= tt.rioat3Z)
     * = tf.                                                                ((2,) ),,dtype;tf.
                                                                                        1)
                                                   random.normal
                                                                            ((i,)), dtype tf. f1。
                 Variable         (tf.
     8 = tf.     Variable         (tf.
                                                   rand。m. n。
                                                            rmal                                f1oat32)
                                                                                                 at32)



     print("[ Hypothesis. test . 1")
     H-x = HypottlesisLx_input)              , . . .
     b0r x,n,tin 끗p브＝1叩U츠. .org, Hㅜxf , label키＝      ,,,,
       printVAge= U 걘NI = n=    《95딴k 零fllabel=)t 玎
                              .2！
            . tormat핏x댜U . xi1J . hU:U. IJ j




                                                                                                                                                      -


                                                                                                                                                      工




＠임베디드 전문가 그룹 윌텍                                                    - 88 .                           무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 86 =====
2부. 머신러닝 기본                                   3과. Softmax Classification




         2聲，
           Logistic Regression獅nary Classificatenj
         3과. Softmax Classification(Multinomial Classification)




@）임베디드 전문가 그룹 윌텍               - 89 -   무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 87 =====
2부. 머신러닝 기본                    32F. Softmax Classification




＠임베디드 전문가 그룹 윌텍   - 90 -   무단 전재. 복제, 발췌. 디지털화금지


===== PAGE 88 =====
2부. 머신러닝 기본                                           34. Softmax Classification

                                                                CO茫仄ERT
 Multinomial Classification                                     임배디드 전문가 그醫 윌텍

   G3개 이상의 다양한 Class의 구분
   〃 ex) 다음과 같은 좌표들을 세개의 dass로 구분 하기
           Data for MultinomLaLclassification




＠임베디드 전문가 그룹 윌텍                          - 91 -   무단 전재, 복제, 발췌. 디지털화금지


===== PAGE 89 =====
2부. 머신러닝 기본                                  3과.Softmax Classification




  督 다수의 Binary Classification을 이용한다면？
  臨Decision Boundary 직선 하나를 이용
   ／乍 특정 class와 나머지 class 구분 가능
   ／卜 3개의 클래스 구분 * 3개의 Decision Boundary?




@）임베디드 전문가 그룹 윌텍                - 92 -   무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 90 =====
2부. 머신러닝 기본                                                                            34. Softmax Classification


 Multinomial Classifier정의과정                                                                        엑DE,
                                                                                                    :E ;,,,PERT
   Q 다수의 Binary Classifier 사용 모델
                               （Activation Function 4 Sigmoid)

                                                                              . 해당모델에서 p0 pp1 pp2의 의미
                                  X
                                  ㅡ

                                      x什b + z기）


                                      ,Linear -
                                                    J
                                                   ' Sigmoid
                                                                         Po
                                                                                /1- 각각classO, class1, c1ass2일 확률


                                      tquati이i i   , runcu미1                  ● poppi ,P2 값이 가지게 鬱 특졍
                                                                               /' 각각은 확률이며 0-1사이의 값을 가짐

                                      XIV1 + b1
                                                                              ● 입력의 Class 판단 방법은？
                                                                    쓰i
                                                    -/-
   '     1 ,
                                         near              Sigmoid l           (2. p0 = 0.8, Pi =0.4, P2 = 0.6 일 경우
  it         1
                                         uation            -uflctIOnj
   밸
   乫｀
          츨'
        뇨r르      ,   --   ,   ,                                                ＇小 가장 높은 확률 선택 + class 0

                                                                    P2        - - .. ., -       -. - -.   .,
                                      入걔1'2 + b2                    －뺙        斗 Activation iUflCttOfl ygmom
                                                          -/-
                                       unear              Sigmoid
                                                                               ＇小 가장 높은 확률 구하는데 필수적일까？
                                       auation            Function l            '乍 Pa: 80%, Pi: 40% " ' 가능할까？




 임베디드 전문가 그룹 윌텍
C）                                                               - 93 -        무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 91 =====
2부. 머신러닝 기본                                                                    3과. Softmax Classification

                                                                                             COD
                                                                                             임버1디드 전문가 그醫 윌텍
                                                                                                             ,


                                     (   'U
                                                             x-
                                                                       』Y什h + b0 고으           J：으

                                                                                                    rn- i
                         J스          P1 꿎큭    ．.                                              Ii    V-' .-
                                    '   Z- P 芦 I              x        xH/l + h1      Softmax -     Z.J 予饉 = ㅗ
                                              n=0                                                   nr0
                              -r
                                    P2-
             xw2 + b2
                        」2
  入’   -
                                                                  x -- 大ㅠ2 + 6?
                              ./-
                                                         t
       . 확률은 양수이 I-／큰 확률차0                                    쓰,
                                                    위ㅎI1logit,，                       쁜；∼，사용
                                                                             대신Odds , ，
                                   ，∼ ' ?．寸j可） 쯔7 ^，∼r二낟J굔父夕\ A4
           〃확률차0l크면，
                   Lab이과Hypothesi｀의차이가커쳐Af희즙효율이향상됨∼             →諦＼길V
           f1 즉. Logit을 Sigmoid 4 p 4 odds. 보다 Logit에 지수를 취해 odd$ 계산
                                                                   （간단함）




 임베디드 전문가 그룹 윌텍
C）                                                    - 94 -          무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 92 =====
2부. 머신러닝 기본                                                                                                   3과. Softmax Classification

                                                                                                                          CODE晟 UERT
 Hypothesis of Softmax Classification                                                                                     임베디드 전문가 그醫 윌텍


  Q Hypothesis: y0, yl, y2
                         （각각의 class에 대한 확률）계산 과정

                                                                                               ,
                                                                                               t 11
                \


                        yo =             xwo
                                           『』）.눼2:. 치1J w。 + bo

                                       = xowoo + x1w01 + b0                                I

                    1        Yi:
                                             xw1 + b=       [1b2;
                                                                        1J   :::d 『b1          1수
                                                                                                      Softmax          S(！사 =
                                                                                                                                 e飾


                                                    /
                                        == low'0 + rrn'll + 이

                   'U9
                   ?J91I '- --  .      . 1fl,._1 ,                                             '
  x-     xw2 + i)2 =＋蜘 =XW+ b2 = l:r口I니「，  ∼ㄱ + b2
                    I                                                          L∼z1J
                    ;,
                    毛
                                        = 10w20 + fr1比＇21 + b2
                                                                                           기
                                        I
                        ,'         _



                                                                                                          `


                                               한번의 Matrix Multiplication으로 정리
   /-
        }' =x1'r + B = [T()
                                                」
                                                    fI
                                                           Woo          =lO      W20
                                                                                    I
                                                x1] I
                                                    ilw。
                                                    =
                                                                    i   L!1l     W21I  I
                                                                                       -



          = ［加 Yi
                                                    t.
                                       Y2]
                                                                                             …   Wei삵It Matrix의 Shape
                                                                                           =（입력 변수와수, 클래스의 수）(2,3)
                                                                                           `---）뇨넌스＝뱃스브小－
                                                                                                        －∼      小 /＼小느t옛스．
                                                                                                                         H孔寸




＠임베디드 전문가 그룹 윌텍                                                                - 95 -             무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 93 =====
2부. 머신러닝 기본                                   3과. Softmax Classification




  @ Cost Function: Cross Entropy Error를 사용함
  ● 가설의 결과가 사건의 확률이고. Label과의 차이를 계산
    f2 Logistic Regression과 동일




＠임베디드 전문가 그룹 윌텍                  - 96 =   무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 94 =====
2부. 머신러닝 기본                                    3과. Softmax Classification


  Softmax classification C.E.E 계산의 예                     임베디드 전문가 그푭 윌텍


  @3개의 Class를 구분하는 Softmax classification
   ●Class 0,1,2에 대해서 답이 class 1일［대. 다음 Hypothesis 결과들에 대한 ㄷost는？

      [ Label j:Hypothesis걸2f ; C。st(CEE) 1
          0         0.6                             분포가 비숫함수록 작아짐
         1          0.15      -log 0.15 幻 0.8239
          0         0.25

          0         0.05                                      -   1
          1         0.8       -logO.8 穴二 0.09691   c.E.E7 = - ? plogqi
          0         0.15                                          0


          0          0
          1          1        -log(1) = 0
          0          0




@）임베디드 전문가 그룹 윌텍               - 97 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 95 =====
2부. 머신러닝 기본                                                                                                        3과. Softmax Classification

                                                                                                                                            CODE盖PERT
  Code: Softmax Classification(TF)(1)                                                                                                       임베디드 젼 문 기 ．그룹 윌텍


            @ [예1I 9] Input, Hypothesis, Cost, Gradient
      x_input = tf. constant([[1, 1L , [2, 2.5] - [9` 4.,51], dtype=tf. float32)
      laDels = tt. constantuLl, U, UJ, ..., LU, U, lii, atype=tl-.tloat3z)

      n_var. n_class = 2. 3
      W = tf. Variabie(tf. random.normai( (n_var, n_class),dtype=tf. f10at32))
      B = Vt. Var1aD1eJtt . ranaom. normalun_class,) ,atype=tt. tloat3L))

 ri            logits                   n ---- -r7m:- --F---                  －…그츠
      def             (x)   .   ,   .   .
                                         !1 bgit.s 별도 졍의：cost_tunction에서 logits으류 c.E.E게
 i           return t1.matmul`x, WJ + B I        .       ' V"    一 팝｀/ ,/ `r
                                                                                "
                                                                                 - -
                                                                                    ^     /,              /,               4   /,   =r,   －小1   ／뇨   -   一｀



 `
                                                          '        岫斗흽犬찻加 거입 1
     def Hypathesis(x):                                                    /
       return tf. nn. softmax(logits(x))                                                                                             H(X) = S(XW + 끼
                                                                                                   ，군I-
                                                          III
     def Cost0:                                         I
       logit_value = logits( x inout)                 I
                             fr
       return tf. reduce meanitr. nfl. soTtmax_cross_entr야》   y_witn_iogits` i
                                            _   -------       --        -   -       -,.    -   -     -     -   -   -   -




                             I        1ogits=1og1t_value,     1abe1s=1abe1s)) I




                                                                                                                                                                1



＠임베디드 전문가 그룹 윌텍                                                - 98 -           무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 96 =====
2부. 머신러닝 기본                                             3과. Softmax Classification




 epodIs = 500e0
 learning_rate = 0.01
 optimizer = optimizers. SGD( learning_rate=learning_rate)

 for cnt in ranae(0. eDochs+1):
   cost oraonicnti = I_ostt J
   if cnt 읨； (enochs//20) = 0:
     printi. t i =2！쟈j cost = i ;21(J.4r .format(cnt, cost_grapnKnt j U



                    8.104
                   0.1371
                  0.06498
                 0.007014
                 0.006651
                 o. oo6324




@）임베디드 전문가 그룹 윌텍                       - 99 -   무단 전재. 복제, 발췌. 디지털화금지


===== PAGE 97 =====
2부. 머신러닝 기본                                                                3과. Softmax Classification

                                                                                                    COPE盈PERI
                                                                                                           R
 Code: Softmax CIassification(TF)(3)                                                                입베디드 자 믄가 4름 욋Eli


  e［예제 9] Training 결과Test, Prediction
  print(np.argmax佃ypothesis(x_input). axis=1))

  x_test = tf.constant([[3.5, 1.01, [5.0, 8.01. [9.0, .7.0], [5.0, 5.01]
                                                     ,cltype=tt . tloat32)
  1_x = Hypothesis(x_test)   , ,,
  tor 폰 깍， range，
                탠－test；돈haP兮！，아) :   .      ,.,
    printr1' 9 Group U= 나 "" .tormat( x_testLii ' np.argmax(ILx[i]), H_xlil) )
                                                                       Dath for Mu贓rjpizll磁 dassificat沁a
  [0 0 8 1 1 1 2 2 21
  [3.5 L]=> Group 0: [8.06e-01 3.490e-05 1.935e-01]
  [5. 8.1 =? Group 1: 므.21e-04 9.998e-01 1.994e-05j                                     C!ass
  19뇨－zㅢ－ㅌa．  虹멥口－乙：-1L｀ 驪t，  峰_k皿2"＝皿Jㄴ2罌루＝旦1．   』
  龜5. 5. j =? Group 1: 10.3248 0.3725    0.302』 ！·                    斗｀
  -     寸mmm戶－ m吃升”   -.   -----〃



  경계에 있는 경우 약간이라도 큰 값 기준으로 Group 선택
                                                      4           Class 0
  → 더 많은 데이터로 학습할 경우, 더 정밀하게 선택 가능                                    mm   ∼

                                                              /                    "`
                                                                                        ,
                                                          (
                                                                           紛

                                                                                            i
                                                                                    /
                                                      2
                                                          ＼…                   '
                                                           \ '
                                                                  1    견
                                                                           」 d*
                                                                                            3   ;




＠임베디드 전문가 그룹 윌텍                       -100 -    무단 전재. 복제, 발췌, 디지털화금지


===== PAGE 98 =====
2부. 머신러닝 기본                                                      34. Softmax Classification


 LAB·. BP Softmax 디assification(TF,                                         CODEAP
  -                                                     ,    '              입베디드 즈니구7} 꼬졉 윅텍


  @［예제 10] lnput(age, bmi) and Label(0: 정상. 1: 주의. 2: 경고）
      G X_input, Labels, Hypothesis Test 및 predict 함수만 존재하는 LAB 코드에서
       f1 Hypomesis, cost 및 Training 부분을 완성하세요
       ' 2'［예제 9] Softmax 디assification(TF) 참조하세요
        x_input =.tf. constant([[25,22],(25,26],[25,30],[35,22],
            . . . ,[73,22L173《2．트］,L73L3이I, 야ype= tf. f零oat32)
        labels 三tf. constant(【L1'0,0J,l9,1,0j,L0,0,1J,[1,0,이，
            . . . .10,1. 01,10,0, " ,[0.0, U j . dtype= tf . f1oat32)

        활 =
        8 =

        print("[ Hypothesis. test . ]" )
        H_x = Hypotfles1s(x-input)

        for x,h,1 ,in.zip(x-,inut. org, . tLx,. labels);. ,,,,
          pr.1nt( . 쑤9良弘밴，   읕 ' U 나duel.HJ-/CldSS ' U;, U           … , `,
          . Jormat`xU시' XE ' 』' np.argmax,i; ' np. arg,naxin. nuffipyl. ' 九 a)'




＠임베디드 전문가 그룹 윌텍                             - 101 -    무단 전재, 복제. 발췌, 디지털화 금지


===== PAGE 99 =====
2부. 머신러닝 기본                     34. Softmax Classification




＠임베디드 전문가 그룹 윌텍   - 102 -   무단 전재. 복제, 발췌. 디지털화금지


===== PAGE 100 =====
3부. 딥러닝 기본


===== PAGE 101 =====
3부. 딥러닝 기본                                   1과. Multi Layer Perceptron




               3부. Deep Learning 기본

         1과. Multi Layer Perceptron
         ∼. MNISI‘「 ;：多楓taset and Keras




@）임베디드 전문가 그룹 윌텍              - 105 -     무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 102 =====
3부. 딥러닝 기본                              1과. Multi Layer Perceptron


 2 Input Gate Logiㄷ 학습
  磅 씨 구현을 Gate Logiㄷ의 구현에서부터 출발：가장 Basic 한 소자로 정의
  . 두 개의 입력에 대한 출력을 생성하는 Perceptron




＠임베디드 전문가 그룹 윌텍           - 106 -   무단 전재, 복제, 발췌. 디지털화 금지


===== PAGE 103 =====
3부. 딥러닝 기본                     1과. Multi Layer Perceptron




@）임베디드 전문가 그룹 윌텍   -107 -   무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 104 =====
3부. 딥러닝 기본                                                                                                      1과. Multi Layer Perceptron


 Code:
  ,
       2
       7
         Innut
           r
               Gate
                -
                    Loaidl)
                    - 日 -` '                                                                                            7   임베디드 전문가그룹윌텍

     @ [예제 1] Inputs, Labels, Weights, Hypothesis, Cost Function
                                                                                                                   Weight Matrix의 Shape-
                                                                                                           " "변츠수．
                                                                                                          1『    ’．클래笠）
                                                                                                                    +2, " )
                                                                                                           r
     xo
     xl
                                                                                                           I        bidS Mairix디 》
                                                                                                                                 nape
                                                                                                           t,       《클래스수，     ）수
                                                                                                                                （L)

     x_input =tf. constant([[O, 01{ [O, ,i]r [i, .@1, [1, iJ1,dtype=tf. f1oat32)
     .iaDeis = ti-.constantlj[ JJ, t町 . [DI . " I 』. cltype=tt. t10at32) # liate= AND

 1甘= tf.Variable(tf.random.norma                                                                 iY.dtype=tf , f1oat32쟎n
 IB= tf,Variable(tf.random.norma                                                              ,),dtype=tf.f1oat32) ) i
 '

     def Hypothesis(x): .. ,       ,.    ...                                                      ,
       return tT.s1gmo1a1'tr. matmu上｀,x, · ) +                                                    )

 feps                          , #"" " "' 1石ceT艾∼
                                                "r"
                                                  'ute" .I1
       return -tf.reduce-mean(labels *. tf.ma功·log( Hypothesis( x_inPut)+!E
               + U - laDe!돠 * Vt.math.logU - Hypothesi돠x_lnput) + ep돠)
          (H(.
             c)   .   y)   =    -ylog   (H(x)) (I
                                             -
                                                    -
                                                        y)
                                                             o,   q(1   -   H   (』   ·))1
＠임베디드 전문가 그룹 윌텍                                                                             - 108 -   무단 전재. 복제. 발췌, 디지털화금지


===== PAGE 105 =====
3부. 딥러닝 기본                                                              1고F. Multi Layer Perceptron

                                                                                  COD
                                                                                  임베디드 전문가 그룹 윌텍

  孕［예제 1] Training
  epochs = 5000
  learning_rate = 0.1
  optimizer = optimizers.SGD( learning_rate=1.earning_rate)

  for cnt in range(0, epochs+1):
    cost_grapblcntJ = (.ostU
    if cnt%,,(eochs//20) = ,0: ,.,,. ,. . ,,,,,,,,
      printi. "'[qlcost=u, w＝니t iJIt i m1띈l t1jJ "" . , ...
        .tormatknt,cost_graph脾flt],W[t!),01. Wil . 0j . 하0J"

     optimizer.minimize(Cost, Ew, 81)


                                                       bbb
  [      0] cost = 0.5593. w = U 0.8338] [ 1.188]],
                                               -
                                                             [1    807
                                                             [1
                                                                  -0.
  [ 250이 cost = 0.2705. w = U !b '3J l 1.11111 -
                                                                   792
                                                                  -2.
  1 `(ftJtJ cost = U. j99Drn 떪 = U 2.3061 1 2.339JJ.
                                               -
                                                             [1 -3. 732

  t450+0] cost = G.03746,w = ,. 5.854, . 5.854]., b =    -8.959]
  1475001 cost = 0·03559*，뇨＝4ㅗ．.jㅗ옇吼4.－乞盟인恭．      車뇨＝..
  [50000 cost = e.0339,;w = u 6.059J L 6.059]]. b =
                                                       I    266   -9.     jj




＠임베디드 전문가 그룹 윌텍                            - 109 -      무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 106 =====
3부. 딥러닝 기본                                                                                                                                                                                             l과. Multi Layer Perceptron




                    Hypothesis                                                                                         numpy
                                                                                  ((-                                                              ()
        x=
                                                                      (x_
  H_
                                                                                   input)                          .
  H_    x =              H_   x.
                                         reshape
  H     =    [int
                               (h>
                                                  O.    5)                  f。    r                  1j)
                                                                                                     Ii     in         H_                 xJ
             idx:   ，·range,


                                                                                  {}                                                               {}                                    (H-x:
  for                         in·
                                                                            (x_             input.                     shape[
             print                                                                                   ,                                         :                :
                                                                                                                                                                                                                idx]))"
                                         'Input
                                     (                                                                     Label
                                                                                                                                                                    H.                                  {:>5.
                                                                                                                                                                         :{:>2}
                                                                                                                                                          =>,
                                                                                                     idx]                                                 idxl.                        idx]
                                                                                                                                                    oJ)
             .  rtnat
                    f。                            (x_        input[
                                                                                                                   ,            labels[                                           H[          .   H_   x[
                                                                                                                                                                                                                   2}
＠임베디드 전문가 그룹 윌텍                                                                                                                                           -110 -                        무단 전재, 복제, 발췌. 디지털화금지


===== PAGE 107 =====
3부. 딥러닝 기본                    1과. Multi Layer Perceptron




＠임베디드 전문가 그룹 윌텍   -111 -   무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 108 =====
3부. 딥러닝 기본                     14. Multi Layer Perceptron




＠임베디드 전문가 그룹 윌텍   -112 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 109 =====
3부. 딥러닝 기본                                       l과. Multi Layer Perceptron




  孕 여러 개의 Layer로 구성된 Perceptron 구조
   0 계층 구성 + Input Layer, Hidden Layer, Output Layer
   ● 아래의 Neural Network의 계층 수는？
    〃 2개 + 일반적으로 Input Layer를 제외하고 계충 수를 표현
   ● 아래의 구조로 x이之Gate 학습이 가능할까？




＠임베디드 전문가 그룹 윌텍                   -113 ,   무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 110 =====
3부. 딥러닝 기본                                       1과. Multi Layer Perceptron


 MLP로 구성한 XOR Gate 모델                                      CODE4'x` PERT
                                                           임베디드 전문가 그룹 욀텍


  孕 다음의 Neural Network에 모든 경우의 수 입력에 대한 결과를 계산해보자
                                          OutpUt,
             !Layer7-   -   -
                                           Layer 1




＠임베디드 전문가 그룹 윌텍                 -114 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 111 =====
3부. 딥러닝 기본                    1과. Multi Layer Perceptron




＠임베디드 전문가 그룹 윌텍   -115 -   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 112 =====
3부. 딥러닝 기본                                                       12F. Multi Layer Perceptron


 Code: 2 Input Gate Logic MLP(1)                                            임베디드 전문가 그룹 윌텍


  @ [예iI 2] Weights, Hypothesis, Cost
   ●Weights, Hypothesis 외의 다른 부분 동일




  즈_input = tf . constant([[0.0]'[0,1]'［芽‘이，     [1,1]I ,dtype'tf . float32)
  labels = tt. constanttL U기. " J . " 』. LII Latype=tt. t1oat3z) # Al.朕



                                                                             휘l니r―
  쁘= tf.Variabie(tf.random.normai((2,.2), .dtype= ,tf.f1oat32))                      壯殃den 녀yer
                                                                                      ight & Bias
  쁘 = 뜨·varia얏e,tr.ran甲)m.normai찧1三，  ):`uty,Pe=trJ[.L0dtiL싯＼,
  삣 = 竺· VariaDle낫T.ranoom.normal151, . ]), .atype=tI.110쯔폭I)                췹       山殃
                                                                                      itput iayeifl
  IS' = tr. variaDj.e튁，tT . ranoom.normai` t 1 ' ' ' otype=tr. ll0dtiLj j             ight & Bias     J



  "'照':：凞rnoid(tf.inatmul
          id(tf.matmul(x,,
                     (hidden,
                          we),wi)
                              +,+80)81,
  tp$, =. le;! . # prevent iog(0) => infinite
  uer 윗.osi` j.
                    .        , . .         , .    --
    return 4t . reduce=-neanI,I련bels*t苦·目？tll·坦gi Hypotne今is1x-in?ut)1-ep키
            + U - labels) * tt. lnath.logU - Hypothesi叭x_input) + eps)'




@）임베디드 전문가 그룹 윌텍                            -116 -       무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 113 =====
3부. 딥러닝 기본                                                1과. Multi Layer Perceptron




  Q [예제 2] Prediction 및 Decision Boundary
 ㅐ x = Hvoothesis(x inout) .nujnov(》
 'lx = tix .resnaDe` ` -1 } '
 ㅐ = [intlM>0.5J tor h in H_x]
 for idx in,.range(x_input,.shape[OJ):        . . ..      . .    .,
     printr'.npit U . ' ,Latei .: p , =2. H :1. 三)2flH_x: t:.？邑2, n "
     .tormat(x_].nputL lax j . label돠idx I . 川idx . H_x[idxjJ)




＠임베디드 전문가 그룹 윌텍                         -117 -     무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 114 =====
3부. 딥러닝 기본                                                       1과. M미ti Layer Perceptr아，




  @ "PerceDtrons: an introduction tocomDutational aeometrv"
   냉 iviarvin MinSky. >evmour vaoern I 늬b늬 ，』11
    4. Perceptron은 단순한 선형분류기 + XORGite 문제도 해결할 수 없음
    4. Multi Layer Perceptron을 사용해야 함
     No one on earth had found a viable way to train MLPs good enough to learn such simple function
    ＇小 단순한 기능 구현에도 많은 parameter 학습 필요 * 더욱 많은 연산
                                               （미분 듕) 필요
       x Parameter 개수(weight + bias) = (12+4) + (16+4) + (4+1) = 16 + 20 + 5 = 41개




@）임베디드 전문가 그룹 윌텍                            -118 -      무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 115 =====
3부 . 딥러닝 기본                   14. Multi Layer Perceptron




C）
 임베디드 전문가 그룹 윌텍   -119 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 116 =====
3부. 딥러닝 기본                                    l과. Multi Layer Perceptron


 Backpropagation
  @ MLP의 효율적 학습 방법：복잡한 신경망도 학습가능
   好Geoffrey Hinton, David Rumelart, Ronald Williams가 발표
                                                       （1980년대）
   孕 신경망의 0utput Layer로 부터 역방향으로 기울기 계산을 진행하는 방법
    /2- Feed Forward로 Loss구한 후 backward방향으로 전파시키면서 학습：연샨량 대폭 갛소




@）임베디드 전문가 그룹 윌텍                -12O .   무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 117 =====
3부. 딥러닝 기본                                                                      1과. Multi Layer Perceptron


 Backpropagation: Gradient 계산(1)                                                                       CODEXPERT
                                                                                                       잉베디드 전문가 그룹 윌텍

  i3三）함수 L 의 woㅔ대한 미분 계산：y=2x+1, Cost Function은 MSE 사용
   J Feed Forward 진행：w, x, b 현재 값에 따른 L 값을 계산（정답 y = 2x+1)
    tL,     1
                                                               forzt）
                                                                    α／r(/
            2
                            ^

                                ,'/
                                                                                                   L
                                                               /'= g + b ; 3
                                                                                                               n
                                                                                                       n



                                                                                                                   4
                                /
                                                                                                       ＇
                                                                                                           U
                                     ㅡ
                                                                                                               =
                                1
                                    ㅡ




                                              '                                 MSE
                                `
                                                                                                       〃   α
                                         ~


                                             *'
            1
                                                  /'
                                                                                               /
                                                  /
     z)
                                         /                                                 /
                                                           少
                                                                                      d'

                                                                                  /

                                                                               backward
                                                                                 I

                      生仇                           m"                     AT,
                                                  驪＝1                    方計2(f ！기｝
   aBackpropagation을 위해 알고 있는 수식
                               （연산）
                                  을 기준으로 gradient 수식을 도출
   〃 L 값으로부터 한 단계씩 backward 방향으로 전파하면서 기울기 계산
           x w 학습을 위해서 알아야 하는 값은 L의 woll 대한 미분

          DL       a5r Df DL                           .   .,      .
           ;:-=
          （八i7
                  ㅋ－ " ㅋ7 " ==7 == X " I ' 긱J - 9)
                  〔7ti7 （끄／ （긱／
                                                                                w = w - u · 2( I - u'ix
                                                                                －…－∼돌‘∼；      뇨 二1- 〕
                                                                                                                   h∥




@）임베디드 전문가 그룹 윌텍                                               -121 -    무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 118 =====
3부. 딥러닝 기본                      1과. Multi Layer Perceptron




＠임베디드 전문가 그룹 윌텍   - 122 -   무단 전재. 복제, 발췌. 디지털화금지


===== PAGE 119 =====
3부. 딥러닝 기본                                2 F. MNIST Dataset and Keras




         12蚤 Multi l 聲v袋r P錢rc移ntrnn
         2과. MNIST Dataset and Keras




@）임베디드 전문가 그룹 윌텍              - 123 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 120 =====
3부. 딥러닝 기본                                       2과. MNIST Dataset and Keras


 MNIST Database                                                CODEXPERT
                                        ,,       ,             임베디드 전문가 그룹 왈텍


  Q Modified National Institute of Standards and Technology database
   . 머신러닝 분야의 " Hello. World"
    4, 간단한 컴퓨터 비전 Dataset + 손으로 쓰여진 숫자 이미지로 구성
    ,1- Yann LeCun의 웹사이트0lttp://yann.Iecun.com/exdb/rnnist/）에 호스팅
   3MNIST 데이터의 구성
    /' 손으로 쓴 숫자와 그에 따른 레이블 데이터로 구성
    4' 55,000개의 학습 데이터
                     （Train Data)


                                                                            D/ ㅈ 3 v b 78 9
    4- 5.000개의 검증 데이터
                    （Validation Data)   / / , 3 9 f6 7 g
                                        ㅇlJ 侈 나5, ? 8
    4. 10.000개의 테스트 데이터
                      （Test Data)       D \ 工 J 4 `中 7J乙 랙
                                        ㅇ / 그 3 9 r, 9 ' 져
                                        〃 /己 b /5b 。g 익


                                                                            ㅇ / 2 3 'J
                                        〃 I ㅏ 5 7 戶b 7 f q


                                                                                      / , 7'9
                                        0 / 23 q5白 분r `
                                        。 / J 3 니 5S 걍 戚 q
                                        汐 l 夕 3 45ㄴ 그g


                                                                                     ＞
                                                                                     一
                                        ㅇ , 그 3 Y 礪, 그 ㅎ q


                                                                            α1a 3빅    ,, 7r q
                                        ㅇ 1그 3쟈    6 伊2q
                                        D I J 3 7J
                                                 .`, 7, ,
                                        0/ㅊ     나万   琿γ,
                                             쵸小      。
                                                                    q
                                                                        日
                                                                        1
                                                     ．
                                                                    1
@）임베디드 전문가 그룹 윌텍                   -124 -    무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 121 =====
3부. 딥러닝 기본                                           2과. MNIST Dataset and Keras


 Dataset I Underfitting, Overfitting                                 임베디드 전문가 그룹 욀텍


  孕Train Data vs Test Data
   J Train Data
    ／卜 모델의 최적 파라미터를 찾기위한 Training 과정에 사용하는 Data
   0Test Data
    ,4 Training이 잘 되었는지 확인 하기 위한 Test과정에 사용하는 Data

      I                   Train   data
                                                              Test   data
                                                                            I



  會Underfitting, Overfitting
   .Underfitting: 학습이 부족한 상황
    ' 1. 추가 학습 시 Train Data 탭
                            ［ Test DataO∥대한 Erro
                                               「 모두 개선될 수 있음
   G 0vert1tting:（특정 데이터에）과도하게 학습이 된 상황
    'I. 모델의 Parameter가 Train Data에게만 과도하게 맞춰진 상황
        x Train Data에 대한 정확도는 높으나. Test Data에 대한 정확도는 낯아지는 경향이 생김




＠임베디드 전문가 그룹 윌텍                          - 125 -   무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 122 =====
3부. 딥러닝 기본                   24. MNIST Dataset and Keras




＠임베디드 전문가 그룹 윌텍   -126 -   무단 전재. 복제. 발췌, 디지털화금지


===== PAGE 123 =====
3부. 딥러닝 기본                                                                   2과. MNIST Dataset and Keras
                                                                           1礬讐畔曄1凞蠟｝슥，
                                                                                     ＝뿟쥣心斗客驪多碧→ 一n낙確三秘Hm‘따小∼姓뿟斗섯n약씸磅群옜吟于
                                                                                     _



 `l_    I.
         1_J_   j_ ·. __
  VdIIUdUOfl L.JdLd
                           r% ...J1 ..                                                           CODEXPERT
                                                                                                 임베디드 천문7 그룹 윌텍


  @Validation data
       G Training에는 사용하지 않고. 0verfitting 여부의 확인을 위한 data

                                                                  Validation
                                         Train data                                Test data
                                                                    data


                                                      r
                                               Train data

                             Error
                                                          Validation Set
                                                                                                         u志궉

                                                                    Training Set


                                                                    Training Iteration




@）임베디드 전문가 그룹 윌텍                                          - 127 -      무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 124 =====
3부. 딥러닝 기본                    24. MNIST Dataset and Keras




 임베디드 전문가 그룹 윌텍
C）                - 128 -   무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 125 =====
3부. 딥러닝 기본                    24. MNIST Dataset and Keras




＠임베디드 전문가 그룹 윌텍   - 129 -   무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 126 =====
3부. 딥러닝 기본                                        2과. MNIST Dataset and Keras


 MNIST Classification(SLP)(2): Dataset                               임배디드 전문가 그醫 윌텍


 （꿍［예제 3] MNIST: tf.keras에서 제공하는 Handwriting Dataset
  (train_data,train_labels), (test_data,test_labels) = mnist,load_data(》
  睡nt(",Type: {}", .f으rmat(type(train_data))》．          Type : <class 'numpy,ndarray'>
  print("Shape:U" .tormat(train_data.shape} J
                                                    닐 Shape : (60000. 28, 28)
                                                      Type ; <class 'nu,npy.ndarray'>
  빠nt(",Type: {}" . .，꿴rmat(type(test_data)）》．          Shape : (10000, 28, 28)
  print( " Shape:" " ·tormat(test_data, shape))

  pr喜叫"Type：다”，.format(type( train_labels) ))’.
  print` >nape; U .Tormatttraln_ LaoeLs , snapeJ J      Type : <class 'numpy.ndarray'>
                                                     누 Shape : (6000〔〕
                                                                     .)
                                                       Type : <class 'numpy.pdarray'>
  pr勿t(:,'Type: {}", .fqrmat('ype(test_iabeis))).       Shape : (10000, )
  print(" Shape= " " .tormat(test_1abeIs. shapeJ)
  `                               一∼r∼∼∼留∼∼∼－ 떨Jm




@）임베디드 전문가 그룹 윌텍                  -130 -    무단 전재, 복제, 발췌. 디지털화 금지


===== PAGE 127 =====
3부. 딥러닝 기본                                                                                                                       2과. MNIST Dataset and Keras

                                                                                                                                                       CODE 蓋 PERT
  MNIST Classification(SLP)(3): Dataset                                                                                                                      建   騙돈

                                                                                                                                                       임베디드 진문가 그룝 윌텍




 llTh;K_show = np.arangeTh,'train_data.'sRapeT6lY
；미）..random. sh,1uttle(i.딴＝왠멘) R^vtk- 如기너 'r/ 1           random숫자출력
〔三照＝돈n맨 = 1ux_S쁘．         브; 쁘1---L皿쏴m刃」
                         Lw．              7`-----------戶     ,, !                ㄱ
 tig_train, ax_trair ,= pit. su미）   lot叭2,5,tigsizei1b, 차) - 2행5열＄ubplot l
 tig_train.supt1t3e(Jrain Data ") ---
 tor idx in mngeU0j:                    .                                          .
       ax_traintidx/I5, idx%51.imshow(train_data[idx=show1idx] j,cmap="binary")
       ax_trainlidx//5, idx능SJ,.set_title ( " train_data[ U I (label , : , t J 1
                  .tormat(i0x_snow1icix〕. train_laDel되icix_sno吼laxi UJ
                     0)

                          9
                                  9._OL.)2Sl3a) Ib&

                                            -
                                                         브
                                                      2) 《

                                                         。
                                                             a   dU)2S88SJ0.b.L 1) t, ,, at4) 2299I 1*91

                                                                                    91           -
                                                                                                           0)   r
                                                                                                                9
                                                                                                                    m dat*LUb1)II..S

                                                                                                                             -         9)
                                                                                                                                            rfri而ata。TrainLabel
                                                        1.

                                                        '`                                                                                       tram dat驢117751 0abel 帥
                                                        겸，
                                                                                                                                                 0
                                                        石
                云             0        ∥        由            .             m         .

   ．뿌町d蠟老a빼m쁘堡쁘多 'Fr90l_*0I009971)).b9) 9) J
                                           『' m2092.)29}0l 1)0009 01 出？m.doM9020e)n크b브
                                                                                    ［`} ｝겯？.4뱐철112901(192)
                                                                                                        0.


  i.

  1§

  珊


                                       i戚       円                                           `.       乂
                                                                                                                                                   0             沸




 임베디드 전문가 그룹 윌텍
C）                                                                                         -131 -                      무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 128 =====
3부. 딥러닝 기본                                                                 2과. MNIST Dataset and Keras


 MNIST Classification(SLP)(4)                                                              CODEA 》ERT
                                                                                           임볘디드 전문가 그룹 윌텍


  송[예제 3] Load and reshape MNIST Data for Training
                                                                                       train/test data load
  (train_data, train_labels), (test_data, test_labels) = mnist,load_data()
  train data = train data .astvne(no.f1oat32)/255 ,0          처i』p1
  test_data = test_data.astype(np. float32)/255.0       0.25540:i.0으로

  train_data = train_data.reshape((-i, 784))                               [j60000,28.28) + (60000,784)
  te얏_data = test_data·．reshape( (-1, 作4)) ..
  train_iaoeis = traln_laDels.resrlapeu-1, 1))                                    (60000j +(60000,1)
  test_labels = test_labels . reshape((-1, 1))


                     I reshape   (60000,    28,
                                              28)   +   (60000,            784)

                                                                     dI

                                                                     ^z




                                                    →                m
                                                                     i
                                                                     J




                                                                  783784




@）임베디드 전문가 그룹 윌텍                           -132 -                 무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 129 =====
3부. 딥러닝 기본                                             2과. MNIST Dataset and Keras


 MNIST Classification(SLP)(5)                                              CODEXPERT
                                                                           임베디드 전문가 그룹 윌텍

  @ [예제 31 Weights, Hypothesis, Cost, Accuracy
  categories = 10
  W = tf. Variable(tf. random.riormal( (784.」肆 gpries), dtype=tfjloat32) )
  ,0 = I. I· vdr1dLj1e`tT,.raflu0m:n0rffla1ncategories, I《 0type=tT.r1oatiL))
  iaoei_on = ti ,onejiot`train_iaDeis , categoriesj
                                                             )
  def .iogits(x):                                   룐꾸렉           k)
    return tf. matmul(x, w) + B          N, 784) @(784, 10                 -
  def Hypothesis(x):
    return tf . nn. softmax(logits(x))          h 1o개 중 1개 디assification 4 功卄max

  def costO:                                       I     cross entropy error AF*
                                                          cost:
    return tf.reduce_rnean(tf.nn. s.oftrnax_cross_entropy_with_logits(
                        10glts-J-ogits i train_oataJ . iaueis=iaoei_onj J

  def Accurac '(y_h, y):  ,,
    return np .meaninp.equau
                                                         Accuracy 계산 합수I
        np.argmax(y_h, axis=1).reshape( (-1, 1)), y).astype(np.float32))




@）임베디드 전문가 그룹 윌텍                       -133 -      무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 130 =====
3부. 딥러닝 기본                                          2과. MNIST Dataset and Keras


 MNIST Classification(SLP)(6)
  穹［예제 31 Training
  learning_rate = 0.1
  epod恪 = 1000
  optimizer = optimizers.SGD( 1earning_rate=learning_rate)
  training_idx = np.arange(0, epochs+1, 1)
  accu_graph = np.zeros(epochs+1)

  for cnt in ranae(0. eoochs+1):
    accu_graph[ciitJ = Accuracy(Hypothesis(test_data), test_labels)
    if cnt%(eDochs//20) = 0:
        print( "[{:>5}iaccuracy = {:>6.4}".format(cnt, accu_graph[cnt]))

     optimizer.minimize(Cost, Ew, B])




                              1
           ccuracy = 0.1221
 〔    501 accuracy = 0.2755
     10이 accuracy = 0.4544
     900j accuracy = 0.7961
  [ 9501 accuracy = 0.8005
  [ 1000j accuraq = 0.SfJ41       accuracy: 80%




＠임베디드 전문가 그룹 윌텍                          -134 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 131 =====
3부. 딥러닝 기본                    2과. MNIST Dataset and Keras




＠임베디드 전문가 그룹 윌텍   - 135 -   무단 전재, 복제. 발췌. 디지털화금지


===== PAGE 132 =====
3부. 딥러닝 기본                                                                                                 24. MNIST Dataset and Keras


 tf.keras 기반 코드 작성                                                                                                     CODEAPE
                                                                                                                       임베디드 전문가 그룹 왈텍


  @ Keras에서 제공하는 다양한 API를 이용. 비교적 쉽게 프로그램 개발 가능
  0Keras가 제공하는 Model 정의 방법
   /$ Sequential APIs, Functional APIs, Custom Model(Subclassing APIs)

                                                                                                               i




                                             彊淄

   1
                                                                                  -.-
                                                                                                                           '
                          r
                                  I-
   I tf.
       keras.
                Iayers.                Flatten I                          了「 tf Keras.layers.Dense ; 듀ㅔ斗 小M6c+a［粃r
                     咎    도   `

                                           m磁老蠟1뇨小ㅈ滋，
                                                    灌口漆앉∼／締표窮轍∼ ∼요표二뜨小t   云二繩小   md斗驪－ m닝七궉心m궁∼ 口   m牙多玉




＠임베디드 전문가 그룹 윌텍                                                             -136 -                  무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 133 =====
3부. 딥러닝 기본                                                   24. MNIST Dataset and Keras


 MNIST Classification(SLP): tf.keras AF용                                         임베디드 전문가 그룹 윌텍

  會［예제 4] tf.keras를 사용한 MNIST Classification
  from tensorflow.keras.datasets import mnist
  (x_train, y_train), (x_test, y_test) = mnist.load_data()                                 Dataset준n
  x_train, x_test = x_train I 255.0, x_test / 255,0

  model = tf.keras.models.Sequential.([ tf.keras.Input(shape=(28,28)),     Model 청의
                             tf.keras. layers.FlattenQ,
                             tf.keras. layers.Dense(10, activation='softmax')])

  model. compile(optimizer= 'SGD ' , 1,oss=       categorical_crossentropy'
  metrics= 'accuracy'])    -                                                      訂Model      compile

  model.fit (x_train, y_train, epochs=5)      뇨0m-Lo- 弘4rinin i
   그＼楙g꼿by多‘기 ）貌.- "깃 ' .
  model.eva'luate(x_test, y_test, ' verbose=2)                   Evaluate

 Epoch 1/5
 1875/1875                            35 2ms/step - accuracy: 0.7082 - loss: 1.1408

 Epoch 5/5
 1875/1875                      2s ims/step - accuracy: 0.90羽 - loss: 0.3595
 [0.3355335593223572, 0.9092000126838684]
                                                   accuracy: 90.7% 4 optimizer = 'adam' 사용 Al 92.7%




＠임베디드 전문가 그룹 윌텍                               - 137 -   무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 134 =====
I


===== PAGE 135 =====
3부. 딥러닝 기본                                                                  2과. MNIST Dataset and Keras



小긱：갸1:;;；」；ㅅ；‘』      ir…… C0DEXPERT
    Iassification(MLP)(2)      j t(
 model = tf.keras.models.Sequential([
     tf . keras.Input(shape=(28,28)),
     tf.keras.layers.FlattenO,
   r什－  ,ke「as.l：甘；y돋瓦. Deng5往琵7,｀託l式輾珊i;i;;rrgf4而쿄 ＇j:,.
   l tf.kerasJ르yers. Den5르． 5...Activation=' s1.gjnoid1뇨‘
     tf.keras.layers.Dense(10, activation='softmax')
 I)
 Model: " sequential"                                                                                                       '

   Layer (type)                              Output 轍ape                                              Param #

   flatten (Flatten)                         (           J   섭妃）                                                   a
                                                                                                                            트
   dense (Dense)                             C           ,   戶）   컨）                                  蔑0큰60                 立

                                                                                                                            量
   dense_i (uense)                           (                        ＞                                b5 ' 192
                                                                                                                            l
                                                             pn｛
                                                         J
                                                                  」
                                                 …




   dense_2 (Dense)                           (       ∼       三社》                                           , , 익 ？嚥




  Tot콘  params: 了千슥322 (i.03 舛D) --                                                               r' accuracy:97.8% -
  Tra1naOLe params: 漱浮十風：냥 (1.03 MB}                                                              `                         Y
                                                                                                                                          !
  Non-trainable par ms:, 0 (0.80 B)              3.13/313 - is - loss: 0.0771 - accuracy: 0, .9777                                        J

                                                 10.07707995921373367, 0.9776999950408936〕                                                {
                                                                                                                                          (
                                                                               >＂논町n걱뇨져m쑤＾ 휘너n…            r   乙                     1r

                                                                               쿄초旨金鍵挺珊孕響               …   싸           ……       ……            `




                                       珏難g肖騙稷手r心…




@）임베디드 전문가 그룹 윌텍                                 - 139 -                  무단 전재. 복제. 발췌, 디지털화금지


===== PAGE 136 =====
3부. 딥러닝 기본                                                              24. MNIST Dataset and Keras


                                                                                                  임베디드 전 문가 그룹 윌텍



 （르 더 많은 Layer를 쌓을수록 성능은 증가하는가？
   model. = tf.keras.model.s.Sequential([
       tf. keras.Input(shape=(28,28)),
       tf.keras. layers.Flattenfl.
     rtf .keras. layers.Dense(256, activation='sigmoid'),
       tf.keras. 1.ayers.Dense(256, activation='sigmoid'),
       tf.keras.layers.Dense(256, activation='sigmoid'),
       tf.keras.layers.Dense(256, activation='signtoid'),
       tf.keras. layers.Dense(256, activat ion='sigmoid' ),
       tf.keras.layers.Dense(10, activation='softmax')
   1)
   미3/313 - 澾 느 loss: 0 田35 - accuracy: 〔）.9696 于＝        .∼ ,,.. 一
                                                  dCCUrdCy· 珊 .y九 ' r
   ［□，
     m3459923138비847. 0. 9696000기83미시미

  G training 회수부족？ epochs = 20으로 증가
                                                       4
    313/313 - is - loss: 0. 1391 - accuracy: 0. 9785   크            1   ^   떼

                                                           ac`;ura`=y. ,' '. J汕
                                                                                .   른   驪 ＇




    [0. 13913984596729279, 0. 9785000085830588]

   ＇小 Layer 층수에 따라 epoch$ 조절 필요 할 수 있음
    4 Layer를 늘릴수록 성능이 증가하는 것만은 아님 + 원인 및 해결방안 추후 학습
                         「融… 堪r      4    ：…     ＼釀希팟                                         「   …




                                                                                                                    ,




                                                                                                                    녹




＠임베디드 전문가 그룹 윌텍                                - 140 -        무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 137 =====
3부. 딥러닝 기본                                24. MNIST Dataset and Keras


 Digit Sign Classification
  @ kag이e의 Dataset: 한 손으로 0-9를 표현하는 이미지 데이터
   017MB
       （압축파일）
            . Color(RGB), Size(100X100)




@）임베디드 전문가 그룹 윌텍             - 141 -   무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 138 =====
3부. 딥러닝 기본                                                                                                                                  2과. MNIST Dataset and Keras


     Digit Sign Classification                                                                         (SLP)          (1)             ---                                CODE         ;:ERT

                       !                                                                                                                                             j
     1MG_      64      =


     f。r md
         SIZEi
            in ran。
                  e                          1。 ii                      :
       도i尾百＝'f토i玉＝ii后茄“r"7ㅜT'g在Zi;iil丁＋ ' /*.*'                                                                                                 l        - path + Dataset/O/*.*
                                       (。
                                                                                                                                                             /                                            \




                                                                                                                       i
 -
 -      files =뽀坐皿쁘(path)                                                                                                                       J        - 枏e$ *해당폴더의 모든 파잎




-                                                                                                                                                                    -
                                                                                                                                                         ,                                                /
 1
               tmpx                  array   ([(v2.resize
                                                                                                                                            V
                           np,   .
                                                            cv2. cvtColor                          (
                                                                                                                (i;
                                                                                                                               caC\
                                                                                                                                                L
                                                               v2.                 imread
                                                                                                                (x,   cv2. IMREAD_
                                                                                   C0L0R_                                                           C0L0R)
                                                                                         BGR2RGB))
                                                                                                                                                                 ,
                                                                      v2.
                                                                                  SIZE,1MG_SIZE)
                                                        )
                                                             (1MG_                                                         ,
                                                                     r x
                                            ([                                                            es)))
                                                                                                       files]
                                                                                   in
                                                            f。
           tmpy        =   np.
                                     array       mndj                *      len             (fil
 -     'xtrain, xte도／rytrain, ytest                                                                            train_test_sp1!t(] - tmpx, tmpul train
                                                                                                                                                         /                                            ,

                                                                                                                                                                                      data2
 -     1          mp', 'mpy,                 ' st_ 'ize= ).Z , ranaom_state=123)                                                                     i   i
                                                                                                                                                         딪
                                                                                                                                                                 test data 'J   BFI
                                                                                                                                                                                              split
           -     )At
     1) cv2.imread(x. cv2.IMREAD_COLOR) ··· for x in files + 해당 폴더의 파일 1개 컬러로 Read
     2) cv2.cvtColor(·" . cv2.COLOR BGR2RGB) 4 익우 파익의 컥러 BGR읔 RGB로 변화
     3) cv2.resize( " . (IMG-SIZE,IMG_SIZE)) 4 0lOl417h'e'ize (100, FOO) 5 (64.64)
     4) np.array([ "] + 최종적으로 읽어서 변환한 이미지를 np.array로 tmpx에 저장




＠임베디드 전문가 그룹 윌텍                                                                                        - 142 -           무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 139 =====
3부. 딥러닝 기본                                                  2과. MNIST Dataset and Keras

                                                                        COD!人 'ERT
 Digit Sign Classification(SLP)(2)                                      임베디드 전문가 그룹 윌텍

  會［예제 5] 모델 정의 및 요약
   model = tf.keras.models.Sequential([
                tf.keras.Input(shape=(IMG_SIZE, IMG_SIZE,3)),
                tf.keras. layer苔. FlattenO,
                 tf.keras.layers.Dense(10, activation='softmax') 1)

   model. compile(optimizer= 'adam',
                  loss=' sparse_categorical_crossentropy',
                  metrics=[ 'accuracy'])

   model. summary()

  Model: " sequential"

    Layer (type)                           Output Shape                    Parm #

    flatten 0:jatten)                      (     J UZ88)                        8

    dense (Dense)                          （쟈뜬콰「［갸J 10)                    122,898

   Total params: }U1890 (480.84 KB)
   Trainable params: 22      (480.04 KB)
   Non-trainable paralts: l u.00 B)




@）임베디드 전문가 그룹 윌텍                           - 143 =        무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 140 =====
3부. 딥러닝 기본                                       24. MNIST Dataset and Keras




  history = model.fit (train_data, ,trainjabels, epochs=lGO, , ..
                       vaiioation_uata=` test_aata, test_iaoeisJJ




＠임베디드 전문가 그룹 윌텍                     - 144 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 141 =====
3부. 딥러닝 기본                    24. MNIST Dataset and Keras




＠임베디드 전문가 그룹 윌텍   - 145 -   무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 142 =====
3부. 딥러닝 기본                                           2과. MNIST Dataset and Keras

                                                                             CODEAPERT
 Digit Sign Classification(MLP)                                              임베디드 전문가 그룹 욀텍


  "model = tf.keras.models.Sequential([
      tf水eras.Input(shape=(IMG_SIZE, IM6_SIZE, 3)),
      tf.keras. layers.FlattenO,
      tf.keras. layers.Dense(256, activation= ' sigmoid'),
      tf.keras. layers.Dense(256, activation= ' sigmoid'),
      tf.keras. layers.Dense(10, activation=' softmaf)
  1)
  Epo사198/100                                                          r
  52/52                      0s 3ms/step - val_accuracy: 0.1007 ㅓ val-loss: 2.3032
  Epoch 99/100                                                         l
  52/52                      Os 3ms/step - val_accuracy: 0.1007 - val loss= 2. 3029
                                                                       .
  Epoch 100/100
                                                                             -




                                                                       1
  52/52                      Os 3mslstep - val_accuracy: 0.1007 ㅓ val. loss: 2.3029


  . 더 낮은 정확도가 나오거나. 심지어 학습이 거의 되지 않는 경우도 발생
   心 간단한 흑백 숫자에 비해 복잡한 이미지에서는 어떤 처리를 해야 할까？

                                                      c小r아이지 《 윙생q 桐斗
                                                             -)e   '       t力M I   「놔，




＠임베디드 전문가 그룹 윌텍                       -146 -     무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 143 =====
4부. CNN(Convolutional Neural Network)


===== PAGE 144 =====
4부. CNN                                 1과. 다lN 개요




＠임베디드 전문가 그룹 윌텍   - 149 -   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 145 =====
4부. CNN                                     1과. CNN 개요


  Convolutional Neural Network        -, CODEAPER,T
   G 고양이 실험：사물을 부분적으로 관찰하며 자극에 따라 뇌의 특정부분이 활성화




@）임베디드 전문가 그룹 윌텍       -150 -   무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 146 =====
4부. CNN                                                      1과. CNN 개요


  이미지 데이터                                                 CODEXPERT
                                                           임베디드 전문가 그룹 윌텍


  ,p，
    ' 이미지 데이터
            （image data)
   . 픽셀단위로 이미지를 직사각형 형태로 구성한 것
     4. 픽셀：디지털 이미지에서 표시할 수 있는 가장 작은 단위
     1- 전체 이미지의 크기를 표현 할 때는
                          （가로픽셀 수 * 세로픽셀 수）
                                          형식으로 표현
   密 색 공간
        （C이or space)
   臼 픽셀의 색을 숫자로 표현하는 방식
     4- Grayscale: 영도를 나타내는 숫자     로 표시
                             （0-255）
     4- RGB: Red(0-255). Green(0-255), Blue(0-255）
                                                 의 3가지 색의 명도로표시
     4- HSV: 색상
              （0-360). 채도（0-100). 명도
                                   （0-100）
                                         로 표시
                        z




                         ,,i,
                   '윗，
                                ./




                   RGB 색 공간                   HSV색공간




＠임베디드 전문가 그룹 윌텍                      -151 -   무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 147 =====
4부. CNN                                                        1과. CNN 개요


                                                             CODEXPERT
  이미지 데이터 특징                                                 임볘디드 전문가 그룹 윌텍

   . 픽셀데이터는 상하좌우의 픽셀 데이터와 연관 관계를 가지고 있음
   . 2차원 혹은 3차원 정보로 구성됨
                                         검은 픽셀이라고 전부 씨가 아님
                                          주변 픽셀과의 관계가 중요



          13




                               r긔미지데이터놉3ㅊ
                               L
                                               F ql이터1
                                  가로’:13 ' 섀로:13' 색：3 j
                    13


   3 분석 기준：주어진 이미지를 분석하여 미리 정의된 카테고리 중 하나로 분류
    '4' Fully Connected Layer만으로 구성된 모델은 1차원 형태로 한정
    4. 3차원 이미지 데이터를 1차원으로 평면화 시켜야 함
      'C 공간정보의 유실로 인한 정보부족 + 특징 추출 및 학습이 비효율적. 정확도를 높이는데 한계
      'C 어떻게 이미지의 공간정보를 유지한 채로 학습 시킬 것 인가？




@）임베디드 전문가 그룹 윌텍                -152 -     무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 148 =====
4부. CNN                                                             1과. CNN 개요


  Fully Connected 와 Convolution                       임베디드 전문가 그룹 윌텍


  @ Fully Connected Layer의 한계
   . 데이터의 형상 무시됨 + 원본이 이미지라면 평탄화 과정에서 공간적 정보 유실됨




                                                  口    「，   『   “    '" " "
                                                  l 인접한픽셀들간의 관계 등의
                                                     몬실석인 의미듈 가시는
                                                     패턴정보가 유실될 수 있다




       -   2Dimension "
       - UJ * 1J*치，

                                이"mens
                                  (507)巴
   QCony이ution 연산의 의미              十 V시叭e't 학인
   . 원본 data의 형태를 무너뜨리지 않으면서 연산을 진행
     4- Data가 가진 본연의 patterr, 정보를 찾기에 적합




@）임베디드 전문가 그룹 윌텍                -153 .     무단 전재, 복제, 발췌. 디지털화 금지


===== PAGE 149 =====
4부. CNN                                                                     1과. CNN 개요




   臼 이미지의 Cony이ution * 픽셀과 주변픽셀들의 Weighted Sum
  @ Why Convolution?
   3 의상의 스타일에 관한 차이점을 설명한다면）
    /2- 옷의 색. 상표의 엠블럼 등의 정보는 불필요
    ／卞 중요한 것은 옷의 윤곽. 모양 자체 + 블라우스는 셔츠. 재킷의 모양과는 다름
    ／乍 붊필요 정보를 제거하는 필터 설계 + 해당 요소에 의해 구분 되어지는 것 방지

  會 이미지 처리에서의 Cony이ution
   . 원본 이미지 * 필터 = 새로운 이미지
                         （feature map)


                                                                 ，돠綽7+ 빠知大' 각
                                                                            「' "之
     [Source: enwikipedia.org/wiki/KerneI_(mage_processing) ]
                            l스小，
                               .，及卜숴如，
                                     \                              수Q트er악 b＞畛 挻｛J팁．




@）임베디드 전문가 그룹 윌텍                                  -154 -        무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 150 =====
4부. CNN                                                                       1과. CNN 개요


  CNN     (Convolutional   Neural Network)                               CODEXPERT

   0Convolution Layer 추가 * 입력 데이터에 필터 적용 후 활성화 함수를 반영
   . 이미지를 추출하는 부분과 클래스를 분류하는 부분으로 구분
   ● 복수의 필터로 이미지 특징 추출 및 학습




                              Lonvolutional_neural_network#
                               니 그「치白스
                                               .           /media/File:Typical_cnn.pngl
                                                             (   -
                                                                     -   '\




                                           `/r1나" 딘 놔씽， ' (`"ㅍ1'" ( /




@）임베디드 전문가 그룹 윌텍              -155 -        무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 151 =====
4부. CNN                                                                         1과. CNN 개요




  @ Medical                乂P叫
   . 의료 영상 판독용 모니터 今 고가의 장비. 해상도나 명암 비. 휘도 등의 요소에 영향
   臼 한정된 시간 안에 검토해야 하는 많은 정보로 오진의 가능성


  @ Recommender Engine
   . 검색 키워드에 맞추어 해당 상품에 맞는 키워드를 일일이 입력
   呼CNN을 이용하여 입력된 이미지 훈련 + 패션 취향에 맞춰 상품 추천




                       완g 미미1i    包§ 甘4 J楓피   －麟깐뺘과갈召世이明챠彎4



              [Source: zdnetcokr/view/?no=20170318125505&re=R_20170629164620]




＠임베디드 전문가 그룹 윌텍                          -156 -     무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 152 =====
4부 . CNN                                              1과. CNN 개요


                                                    CODEAPERT
  CNN 활용
       （2)                                          임베디드 전문가 그룹 윌텍


  （孕Face Recognition
    臼 보안／감시. 신원 확인, 감정상태 파악 등에 활용
                                 （사람 97.5%, DeepFace 97.35%)
    臼DeepFace(2014): FACEBOOK에서 개발
                             （99.63％의 정확도）
    .FaceNet(2015): Goo이e에서 개발
    . 바이두 AI(2015): 99.77％의 정확도


   @ Mobility
    . 영상인식 기술이 자율 주행 자동차의 핵심기술
    .Tesla, 引VIW, Audi: NVIDIA가 CNN기반으로 개발한 PX-2드라이브 사용


  （季Fault Detection
    . 반도체 공정의 Wafer불량 검지
                                             「tㅉ乞처기처닝섯은
                                       甲 미이시 t）
    . 가동중인 기계설비의 이상징후 검출
                                           斗 사욜．




＠임베디드 전문가 그룹 윌텍               -157 -   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 153 =====
4부. CNN                                             2과. CNN 기본연산




          4부. CNN(Convolutional Neural Network)

            1* CNN 개요
            2과, CNN 기본연산
            32.F. CNN I뱐 Clas:
            4羈, CNN 쌀전 시키기




＠임베디드 전문가 그룹 윌텍                  -158 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 154 =====
4부. CNN                                                                            2과. CNN 기본연산




  @ Typical CNN Architecture
   J Convolution Layer: 2D Convolution
   ●Pooling Layer: Max pooling or Average pooling
   .Fully Connected Layer




               [Source: en,Wikipedia.org/wiki/Convolutional_neural_network#/media/File:Typical_cnn.png]




＠임베디드 전문가 그룹 윌텍                               -159 -        무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 155 =====
4부. CNN                                                            2과. CNN 기본연산


  Fully Connected 연산
                   （D
   . 출력 yo의 연산




                        Yo   =   wooxo+ Wi,,Xi   +W20X2   +W30X3              헤
                                                                      + W41JX4＋




@）임베디드 전문가 그룹 윌텍    -160 -          무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 156 =====
4부. CNN                                                 2과. CNN 기본연산


                   （2)
  Fully Connected 연산                                      CODEXPERT
                                                           임베디드 전문가 그룹 윌택


   口 출력 yl의 연산

       Input       Output
   r




                                 씰J
                                  （〕0：
                                     勿 + W10Xi + W2()勿 + W30X3 + W40X4 + b0




                            y1 = W0iXo + t011Xi + W21X2 + W31X3 + W4114 + z7i




@）임베디드 전문가 그룹 윌텍        -161 -      무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 157 =====
4부. CNN                               2과. CNN 기본연산




＠임베디드 전문가 그룹 윌텍   - 162 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 158 =====
4부. CNN                               2과. CNN 기본연산




@）임베디드 전문가 그룹 윌텍   -163 -   무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 159 =====
4부. CNN                               2과. CNN 기본연산




＠임베디드 전문가 그룹 윌텍   - 164 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 160 =====
4부. CNN                              2과. CNN 기본연산




@）임베디드 전문가 그룹 윌텍   -165 -   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 161 =====
4부. CNN                               2과. CNN 기본연산




@）임베디드 전문가 그룹 윌텍   - 166 -   무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 162 =====
4부. CNN                                                    2과. CNN 기본연산




   孕2D Cony이ution의 입력. 필터 크기와 출력 크기의 관계
   臼 입력이 M* M, 필터가 N*N 때. output의 크기가 L* L이라면）  (m>=n)
    4. 현재 P(padding)=0. S(stride)=1 이며. 추후에 학습       .
            r－→                    …，,    f∼.  --, 卞1十er
          L L= (M +2P- N)/S+1 J      _FL   L= M- N -'-l;   i




@）임베디드 전문가 그룹 윌텍                  -167 -   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 163 =====
4부. CNN                                                                                      2과. CNN 기본연산


  2D Convolution연산을위한준비                                                                       毖芝烈烈
  穹tf.nn.conv2d
  I            tf.nn.conv2d(input. filters=   None,
                                                       padding=   None,   data_    format=   'N   HWC
                                                                                                    ")   "




      .Arguments
             Name                                          Description
      input            Tensor, data_format parameter 설정에 맞는 shape을 입력해야 함
      ,.,,             shape [filter_height, filjej_width. in_channels, out_channels을 F진 4D Tensor
      riiter          닙뇩 f뉩흔峰屎흐토.j2l ]Oi6' f∼－                                    小7∼→－--－∼－
          ,.           "VALID": Padding을 하지 않음
      paaaing          'SAME"；입력크기와같은사이즈가되도록zero Padding합

                       input, output data의 format을 결정 함
      data_format      "NHWC": [batch, height, width, channels]
                       'NCHW": [batch, channels, height, width]

      .Return
         4 input과 동일 type을 가진 ㅜensor




＠임베디드 전문가 그룹 윌텍                                       -168 -        무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 164 =====
4부. CNN                                                                                            2과. CNN 기본연산


  2D Convolution 기본 연산 예제                                                                              임베디드 전문가 그룹 윌텍


  《코［예제 1] 2D Convolution 기본 연산
   . 입력 1채널 - 필터 1. 채널 1개
   而＝Input = np.arange(1.26.1,dtype=np.float32).reshaDe((r5-5可)
   'np_filter = np.array([l . 1.1.1],dtype=np.f10at32).reshape((2. 2. 1, `))
                                                                                                  ,7＼一／    ∼－   一∼－




    input_constant = tf.constant(np_input)
    '＝극 ] "^ `m 〃＾1,...`"   "
     IJㅗ L. j_ `.｀』II) LQII (.
                                 -
                                 -
                                     .4- = '．
                                            一－‘떼 』．m`1』
                                      L I .%.uII> LaIIL
                                                        ．
                                                        1. ..
                                                          lIp_   IJ. LLtL   /
                                                                                                         뇨甲
                                                                                                  鉀te「의 口．
                                                                                                 r -        - -       ＝」-



    cony = tf.nn.conv2d(input_constant, fi1ters=fi1ter_const'ht,      '"
                                                                                                          .（人J .      胛
                                                                                                                        ! `
                                                                                                                        -'    1
                                                                                                                                  L｀   ㅁ
                                                strides=l, padding='VALID')
    out = conv.numpy()
                                                         pad《拉珊흡차후에설멸l

      1     3 4 5
             2
                                                                   16 六그                   16 =1*1+2*1+6*1+7*1 1
      6     8 9 10
             7
                                                                                >4
                                                                                      ＞孑
                                      ⑧                    → 3(7 今 싸 4名
                                                1 1
      11 12 3 14 15
      16 17 18 19 20
                                                1 1                驪
      21 22 23 24 25




＠임베디드 전문가 그룹 윌텍                                              -169 -                  무단 전재, 복제, 발췌. 디지털화 금지


===== PAGE 165 =====
4부. CNN                                                                            2과. CNN 기본연산


  2D Cony이ution 연산                                                                  입볘디느 진 문가 그룝 욍텍

  匹》입력이 여러 채널일 경우의 연산
     l Input Data츳 2D 1「 Filter: 2D
     흴 5*5*3             2*2*3                                                 r
                                      斗殆 ㅣ     』시
                                                                    ~                         ＞ㅍㄱ
     image




                                                                                       lifR
                                                                                        ter
                     赴싸잽 졍什f.
  會 다 채널 입력일 경우 2D Cony이ution의 입력.필터 크기와 출력 크기의 관계
   . 입력이 M* M* C. 필터가 N* N* C 때. output의 크기가 L* L이라면？(m>=n)

                                      I   L=
                                                    M-
                                                           N+   1        l




＠임베디드 전문가 그룹 윌텍                                          -170 -         무단 전재. 복제, 발췌. 디지털화금지


===== PAGE 166 =====
4부. CNN                                                                                         2과. CNN 기본연산

                                                                                                              ERT
    2D Cony이ution 연산 예제
「兮혓1m卜H
                                                                                                    CGD
                                                                                                    임베디드 전문가 그룹 윌텍

          ·［예제1］입력3채널’ 르트3채널1개                                                                          -z2(。
                                                                                                            LwC12C-)3〕
             input'  np. arange   1.dtype= fl。   at32) reshape((1 5
          np_Tllter = np.arrayu〕J치L,atype=np. Tloat3L) .resnape니／, L .3,1))
          np_      =
                                     (116                 np   .                .           ,   .   5       万2
          input_constant = tf. constant(ip_input) .                                             自冗니耐i）
                                                                                                     寸I
          Tilter_constant = tt. constantInp_ti! ter)
                                                                                                        3
          cony = tf. nn.conv2d(input_constant, filters=filter_constant,                                          ,,,,. . , ,,,.
                                                                            strioes= i '   pduulflg= VMLILJ '




                        5*5*3    -          이미지와 필터의               2*2*3    ;               4*4*1
                       H* W* C              채널수가 같아야 함         H*W*C




 임베디드 전문가 그룹 윌텍
c）                                                       -171 -            무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 167 =====
                                                    1
4부. CNN                              2과. CNN 기본연산




＠임베디드 전문가 그룹 윌텍   -172 -   무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 168 =====
4부. CNN                                                                                                                         2과. CNN 기본연산


  2D Cony이ution 연산 예제                                                                                                            CODEXPERT
                                                                                                                                 잉베디드 전 문가 그룹 욀텍


   . ［예제 1] 입력 3채널 . 필터 3채널 6개
   np_온n?ut = np . arange(!.76Jfdtype=np. float갼2, ).reshape((1,5,5,3)),/n
   np_   lilter   =   np.
                            arraytjl       J*12*
                                               ,3*   t,   .   atype.   =np.   " ' "" ")
                                                                               T1oat32             .resflapeU1,                      ,3
                                                                                                                                           b)J)
   input_constant = tt. constantU3p_lnput) ,                                                                                               =.佈／
   tii.ter_constant = tt. constantInp_ti1ter)                                                                                              〃나' `'

   cony = tf nn. conv2d(          input_     constant, filters                  『filter_
                                                                                                  constant,
                                                                                           stridesl,                 padding=        '·   VALID   ")
                                                                                               -                  4.4.6
                                                                                                                                ㅒ
                                                     功 鱗b7L뉘 二十

                                                          一4乂4시，
                                                               . o                                                  o i4




＠임베디드 전문가 그룹 윌텍                                           -173 -              무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 169 =====
4부. CNN                                           2과. CNN 기본연산




  padding닐“5A쓰g/<
 mpuTv1J Lero raw기ng
  후 (onvolution항




                                石，>（기   ｀꺼
                                뉵닛숙－         ＞써
                                    社른싸 ￥                  <hr

                             i'샨 叫"
                                  「
                        =)
                                  孝t




@）임버1디드 전문가 그룹 윌텍      -174 -   무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 170 =====
4부. CNN                                                                                                                                                                      2과. CNN 기본연산


  2D Convolution: Padding 예제                                                                                                                                                           CODEXPERT
                                                                                                                                                                                       임베디드 전문가 그룹 윌텍

  曾［예제 21 2D Cony이ution의 Padding 사용 예제
                                                                                                                                                                  ((i,
                    input:
             arange   26,         f1oat32)
                                    ==

                   ([                                                                                                                                            ((3,                                 )》
   np_
                                         np.
                                                                    (1,                  1,
                                                                                              dtype=                               np.
                                                                                                                                                                             5,
                                                                                                                                                     .reshape
                                                                                                                                                                                       5,
   npfilter
                          dtype= f1。at32)
                                     =         np.
                                                     array
                                                                          11*       9,
                                                                                                                             np.
                                                                                                                                          ,reshape                      3,        1,        1)
                                                                                                                                                                                                 1)
                              constant,=                         tf. constant
                                                                        nstant(
    input_
                                                                                                       (np_
   filter_c。
           nstant                                            =    tf c。
                                                                     .                                        np_
                                                                                                                    input)
                                                                                                                             filter)
   cony = tf. nn.conv2d(input_constant. filters=filter constant




                  Input Data: 2D                                                 L!!!t!r; PJ
                             5* 5                                               「 3 * 3-1
                             平
              i              7*7         l                                                                                                                      Output: 2D -
                                                                                8                                                                                                 ㄱ
                                                                                                                                                                  5*5
   ㅣZero padding 卜｀,
                                               1
                                               1




@）임베디드 전문가 그룹 윌텍                                                                                                    -175 -               무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 171 =====
4부. CNN                                         2과. CNN 기본연산


  2D Convolution
    Conv이ution연산：-: 5tride5
                    Strides                       CODEXPERT
   J Cony이ution 연산 시 windows의 얼마만큼 sliding할지에 대한 설정 값




＠임베디드 전문가 그룹 윌텍             -176 -   무단 전재, 복제, 발췌. 디지털화 금지


===== PAGE 172 =====
4부.（갸卄J                                                              2과. CNN 기본연산


  2D Cony이ution: strides 예제                                                    coDEXPERT
                                                                               임베디드 전문가 그룹 윌텍


  Q［예제 3] 2D Cony이ution의 Stride 사용 예제
   npjnput " np.arangell,26,i, dtype=np.float32).reshape((1,5,5,1)),,.
   np-Tiiter = np. arrays I I ' 】' 1' I I 』type=np .rioatiL) .resnapet (z,L' 1' 1"

   input_constant = tf,.constant(np_input) .
   tiiter_ constant = tt, constantInp_1-i1ter)

   cony = tf. nn.conv2d(input_constant, filters=filter-constant,
                                        strides= i
                                               .         ,padding:
   c。nv2 = tf. ...
   .에，         .   c。
               nn. m.
                    nv2d
                      ,2d    t→ nstant, filters filter_ c。
                               c。：t帥t
                           (input_
                           《i.
                                     p.
                                                          nstant,    ;VALID"        ,   )
                                        strides=2,padding="VALID")

                   Strides = 2 * 각 차원 별 2씩 Sliding



          正易쿠                        ！多夕




@）임베디드 전문가 그룹 윌텍                          -177 -     무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 173 =====
4부. CNN                                          2과. CNN 기본연산

                                                  CODEXPERT
  Po이ing                                          임베디드 전문가 그룹 윌텍


  @ Neur비 Networl〔에서 특정 데이터를 샘플링하는 방법
   （各 대표적인 Po이ing 방식
    4- Average po이ing 4 Window 내부의 평균값으로 샘플링
    il- Max po이ing 4 Window 내의 최대값을 샘플링


   孕 특징
    4. 학습 할 parameter가 없음




@）임베디드 전문가 그룹 윌텍              -178 -   무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 174 =====
4부. CNN                                                                                                                          2과. CNN 기본연산


           （Max Po이ing)
  Po이ing연산예시                                                                                                                         CODEXP,
                                                                                                                                        1'?;J E ,,
                                                                                                                                               싸，
      .input data size = 4*4, kernel(=windows) size = 2*2 , strides = 2 01 AI황
                                                                                                                         -   舛 `



  ]     5   6   2           1l
                                     貞，
                                               :6             2   '.
                                                                                                 1        Sc   ,6:           2
  3     2   3   1           3              2       3          1        '
                                                                                                 3        2          3       1
  15    2   0   4           15             2       0          4                              15           2    ’     石 4
  3     2   3   5            3             2       3          5                                  3        2          3       5



                            1              5       6          2                                  4        5          6       2
                                                   3,                                            3        2          3       1
                                                              1
                        .   3,
                                     ‘구m
                                               -

                                                        ,




                    .
                        15 , 2   :
                                                   0    '녹｀
                                                                                    -
                                                                                    ,
                                                                                        `    15           2          0       4             .J   료寸
                                                                                                                                       t
                                                                                                                                       `
                                                                                            !`
                                                                                    -
                                                                                                                                                ,
                            3              2       3          5                     `            3
                                                                                                 /小       2          3 (     5   「




                    겡산 ㅟ屯弓比 0l그3으힁‘ 이궁너
                 → 互，




                켠’乍 州，Q\O E. r 'b'i                                                                   之
                 ^A《x 「m수斗 맨 "悟 ·




@）임베디드 전문가 그룹 윌텍                                                           -179 -   무단 전재, 복제. 발췌, 디지털화 금지


===== PAGE 175 =====
4부. CNN                                                                      2과. CNN 기본연산
      1           …           …                   …                                       …쩍斗∼쌩




  "  -.` ,，一.．.一八1` ，』                                                         CnrUYPcPT
  ti.nn.max-  Doolza
              1
                                                                               Y;，，쓰‘4쯔
                                                                               ，님예ㄴ
                                                                                         '=“，，닉,，쬔
                                                                                    浮신， 문가그룹冒，


  Q tf.nn.max_pool2d
                  tf.nn.max_pool2d(input, ksize, strides. data_format='NHWC', name)

      G arguments
          Name                                          Description
      input           Tensor, data_format parameter 설정에 맞는 shape을 입력해야 함
      ksize           mnt 혹은 길이 1.2.4 중 하나를 갖는 mnt list(window의 각 dimension size)
      strides         mnt 혹은 길이 1.2.4 중 하나를 갖는 mrt list
                                                     （각 dimension의 sliding window에 대한 stride)
                      input, output data의 format을 결정 함
      data_format     "NHWC": [batch, height, width, channels]
                      "NCHW": [batch, channels, height, width]


      .Returns
          4. Tensor
              x format: argument data_format에서 지정된 format
              x max pooling 된 output tensor




@）임베디드 전문가 그룹 윌텍                                  -180 -         무단 전재, 복제, 발췌, 디지털화 금지


===== PAGE 176 =====
4부. CNN                                                       2과. CNN 기본연산


  Max Po이ing 예제
              （D
  . ［예제 41 Pooling: Max Po이ing
   ● 1) Input Shape 4 (1,4,4,1), ksize = 2, strides = 2
  no innut = nn.arrav(111.562L13.231L115.2.EL4LF3.23.511.
                                  dtype=np. tloat32). reshapeU . 4. 4, U

  input. (onstant = tf , constant(np_input)

  pool = tf. nn.max7?ool2d(input_constant,ksize=2,strides=2,padding="VALID")
  out = pooi.numpyi '




                                   iksize ' 2. stride竺의




＠임베디드 전문가 그룹 윌텍                        - 181 -       무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 177 =====
4부. CNN                                                                            2과. CNN 기본연산




 pool_3 = tf.nn.max_pool2d(input_constant,ksize=3,str1des=3,padding="VALID")

 pool_2 = tf . nn .max_pool2d(input_constant,ksize=2,strides=2,padding="VALID")


   齒      驪＝
                    寸多       4    5          1 1       2 크틀 3        4        5
   I                                                       [
   r분5         7         8   9    10             6     7     8       9    ,   10
    →aa
                                                         꿱F               1
   軒午 42 :13                 14   15         i   ll   12 lI 13       141 15
                                                                          』
                                             1             ~I             】
    16         17   18       19   20         1 }5     17        18   i 9 - 20
                                                           ,              』


    21         22   23       24   25             21   22        23   24       25




＠임베디드 전문가 그룹 윌텍                        - 182 -        무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 178 =====
4부. CNN                                          3과. CNN 기반 Classification




          4부. CNN(Convolutional Neural Network)



            2과. CNN ?I뵨? 샨
             3과. CNN 기반 Classification
             4,,F, CNN 墅 j A15'I?I




@）임베디드 전문가 그룹 윌텍                     -183 -   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 179 =====
4부. CNN                             3과. CNN 기반 Classification




                  食

    미＞峰시쑥놔

    今 며꿩午

    이 V,\.沁柶 싸鹹e ·




＠임베디드 전문가 그룹 윌텍       - 184 -   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 180 =====
4부. CNN                                                3과. CNN 기반 Classification




   Q 학습해야 하는 Parameter
    0Convolution layer, Fully connected layer
                                                  Flatten      '     Fully connected layer
                                                20 * 32 9 10        input= 6272, output== m

    3 * 3 * 1 * 32 + 32                                            ( 6272 10+ 10
                                                                             *
  h * w * in_ch * out-ch + bias]                                     r




＠임베디드 전문가 그룹 윌텍                      - 185 .    무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 181 =====
4부. CNN                                                                  3과. CNN 기반 Classification


  1 Cony MNIST Classification 예jI(1)                                                                       cOD
                                                                                                           임베디드 잔문가 그룹 윌텍

  曾［예제 5] 단일 Cony이ution 계층을 가지는 (NN 예제
      0 Dataset준비 과정중            삯.t:rE ,       ] ,     1   `   -        I
                                                                             ---   _.._.           --__-
                                                                                                           7-=- ,       .....   ...   -
  ,       J ,           」 」,   /,   .   , , ,               .       .,             해낭코드실행사）                                               -
  train_oata =np.expa젯尹im糾train_uata, axis=긴工train_da7testdata화shape은？J
  test_uata ' np.expanu_uims(rest-uata, axis=-U   -   이과정이필요한이유？
    . 모델 정의
  model = tf. keras.model.s.Sequential()
  modeLadd(tf. keras.Input(shape=(28, 28, 1)))
  modeLadd(tf. keras. layers.Conv2D(filters=32, kernel_size=3,
  ｀싸考   亡／ -padding=',same’」a， 叫vation='sigmoid'))



                                                                                       小 견ㅇ E으m一q으憂ㅇ ＞
                                                                                                     COu
                                                                                                             解
  mooeL.aaa ttr. Keras. Layers.MaxI-'ooLzu(pooL_size=z,
                                                      strides=2))



                                                                                                           。ㄷ＝OO。 ×mE
  model. add(tf. keras. layers.FlattenO)
  model. add(tf. keras. layers. Dense(i0,
                   activation=' sot tmax ' ))




@）임베디드 전문가 그룹 윌텍                        -186 -                  무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 182 =====
4부. CNN                                                                                                 3과. CNN 기반 (:lassification
’沙쯔른옇野料브騙世∼
          「   「…             「                    心“
                                                   「…                                      熙’一 "小 ’ 多－ 吃‘牛辯￡∼－
                                                                                                             ' ；쫘 ∼「n翌j씬         ∼解多’"m∼m唾小－熙珊聊4싸∼傘




  ∼1 Cony MNIST Classification예제
                               （2)                                                                                         , 黑忿黑
      （孕［예제 5] 단일 Cony이ution 계층을 가지는 CNN 예제
       0 Model Summary 결과

       -



       -
        Model: ∥sequential"

           Layer (type)                                                Output Shape                                                  Paran1 #

           conv2d ( (Onv?D)                                           （… , 28, 28, 32) 弓人乙 乂꾸＋勿




                                                                                                                                                I
           max-p001ing2d (MaxPoo1ing2D)                                C」
                                                                        可첫
                                                                         「，'4, l4, 32)                         >Aft^，小或1r×                 0

           flatten (Flatten)                                                                                                               9
                                                                       (     『／   }   6272)                    G.
                                                                                                                    뇨
                                                                                                                    ;;)
           dense                                                        《：        ,   姆）
                                                                                                                                      6.,7珀

       -
                   (Dense)
           Total params:



        忖……… ∼ m…m →… " …"
                                 ', 050



       ㅣ- Non-LrdinsuLe pdrdII5; 스！三.쁘．ti)
                                          (246.
          I.rai므ao스e parses: 小 ’순” . 느쓴므' 仝
                                          . $.b)
                                                   29

                                                 m∼…
                                                        KB)   -   .




                                                                      m
                                                                                                r   .   的乂1.
                                                                                                `/I- " `u
                                                                                                       `
                                                                                                   移7「「「 口「「
                                                                                              ∼∼ 익丁，
                                                                                                                          *..
                                                                                                                           " '
                                                                                                                                                I
                                                                                                                                                --
                                                                                                                                                -




 唯－                              －…珊’




＠임베디드 전문가 그룹 윌텍                                                       -187 -               무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 183 =====
4부. CNN                         3과. CNN 기반 Classification




@）임베디드 전문가 그룹 윌텍   -188 .   무단 전재, 복제, 발췌. 디지털화 금지


===== PAGE 184 =====
4부. CNN                       3과. CNN 기반 Classification




＠임베디드 전문가 그룹 윌텍   -189 -   무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 185 =====
4부. CNN                                                                                                                                            3과. CNN 기반 Classification

                                                                                                                                                                             CODEAPERT
  3단 Cony이ution layer 사용
                       （D                                                                                                                                                    임베디드 전문가 그룹 윌텍

  《？ 다수의 Cony이ution Layer 사용한 CNN 구조
       .2D Cony이ution Layer 1개 + MAX Po이ing 1개 + 3단으로 구성
                                                         *》           Pooling 冶yer          *
  I  Cony이ution layer공통
                                                              2*2, strides = 2. Max pooling
  [Padding 'same', strides= 1
              ! Cony이Utiofl 佃yer                    Cony이utica layer                            Cony이utica layerj
                                                                                                               .                                   ㅣ    flatten _ J [:    Fplayer       ㅣ
                   3* 1 647 / j
                     3*
                                                        3*3*5464개                                   3*3*64647fl                J                   [ 2D * 64臭j, J [Input =576, output =10i
                                     (                       ㅗ                                                                                                                     1




                                                 。
                                                 匡ㅇ8
                                                   ×쁠             ㄷ으실므0＞ ㄷ
                                                                         ㅇu         。ㄷ＝ㅇㅇQ× m
                                                                                            ㅌ             ㄷㅇm섬石＞ ㄷ
                                                                                                                 ㅇU                     。ㄷ능ㅇ 。즘E
                                                                                                                                                               ㄷ四驪m=




                                               subsampling                        subs카Tipling                             I subsamphng
  `
          '
                                               14 * 14 * 64                        7 * 7 * 64                              F       3*              3*   64
                                                                              '                         /---
                                                              f                                 )
                                                                                                                      工－    －一－




      MNIST Image         rfeature            man             - feature map                                    feature map 「                                 Flatten feature map

       28 * 28 * 1                       28* 28*64 '          ' 14 , 14 * 54                                      7 * 7 * 54                                           576




@）임베디드 전문가 그룹 윌텍                                                                     -190 '                           무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 186 =====
4부. CNN                                                                                                                                3과. CNN 기반 (:lassification


  3단 Cony이ution 怡yer 사용
                      （2)                                                                                                                                   CODEXPERT
                                                                                                                                                            임베디느 전문가 그룹 윌텍

  百等 학습해야 하는 Parameter
   .3개의 Convolution layer, Fully connected layer

                                                     L_        Pooling layer        j#-
                                                     ri=i ,.strides : 2, Max pooling)


     Convolution layeD ! convolution layer                                    [ convolution layer                                                           m
                                                                                                                                                                            F.C layer

                                                                                                                                                     J - input
                                                                                                                                                       [-
        3 , 3 , 1 647 그 [ 3* 3* 64641                                                        3 * 3 * 6464걔                         l                                            output
                                                                                                                                       flatten                      =576,                        =10
     3 * 3 * l * 64+     3 ．了* 64 *"64"+'6司                                         3 * 3 * 64 * 64+ 64                            ,20 , 64 * i1〕 -              576* 10 十10
                                                                                                                                                〕
                          6지
                                                         쵸                                        쵸
                          1
                                                 r                    F                  ㄱ    F                                                  ,




                                  。ㄷ＝ㅇOn줌드                                  귿＝ 。。。X。 E                                   。ㄷ＝ㅇ8즘E
                                  －그
             ㄷㅇm싣으ㅇ ＞ㄷ8                                  ㄷㅇm분그苾＞ ㄷ8                                ㄷㅇm尸三ㅇ ＞ㄷㅇu
                                                                                                                                                                ."
                                                                                                                                                                一
                                                                                                                                                                u V
                                                                                                                                                                  mmㄷ씜                  xmEt0m
                                                                                                                                          Cm업즌
                                                                      --1                                        +   叫                                                          珊
                              논              卜




@）임베디드 전문가 그룹 윌텍                                                                             -191 -                  무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 187 =====
4부. CNN                                                   3과. CNN 기반《:Iassification

                                                                                CODEXPERT
  3 Cony MNIST Classification 예제
                               （1)                                              임베디드 전문가 그룹 윌텍


  〕［예제 히 Cony이ution Layer 3개 기반 MNIST Classification 예제
  目：
    model = tf.keras.models.Sequential()
    modeL ad빈도tf. keras.Input(shape=(28,= 28,. 1끄2                     -I
   rmodel. add(tf. keras.1;YerS.C0nV2D(f11.ters=64, kernel_size=3,
               padding= 'same' ,activation=' sigmoid'))
   1model.addtf . keras.layers.MaxPooi2Dpool size=2a strides=르22     ■·닉

    model..add(tf.keras. layers.Conv2D(fil.ters=64, kernel_size=3,
               padding='same' , activation=' sigmoid'))
    model..add(tf.keras.layers.MaxPool2D(pool size=2, strides=2))           I
    moaeL.aaa(,tT.Keras. Layers.LonvzLJj11ters=b4, Kernet_slze=i,
               padding=' same' ,activation='sigmoid'))
    model.add(tf.keras.layers.MaxPool2D(pool._size=2, strides=2))




                                              ；斗目:
                                               . .'..x.i!.H
                                                         E)c.I_51。<
    model.add(tf.keras.layers.FlattenQ)
    model.. add(tf. keras.layers.Dense(10,
    activation='softmax'))




＠임베디드 전문가 그룹 윌텍                          - 192 ·   무단 전재, 복제, 발췌, 디지털화 금지


===== PAGE 188 =====
4부. CNN                                                             3과. CNN 기반 Classification


  3 Cony MNIST Classification예제(2)                                                 CODr7PERT
                                                                                   1il E 1 Wt
  會［예제 6] Cony이ution Layer 3개 기반 MNIST Classification 예제
   口 Model summary 결과
    Model:   '
                 sequentia1
                          "                                                                       l
      Layer (type)                              Output Shape                           Param #    p
      conv2d αonv2D)                            (     1 z8, 28, 64) ',C (伊－
                                                                          -
                                                                              44
                                                                                   1




                                                                                                  -
      inax_pooling2d (MaxPooling2o)             C,      14, 14, 64)                          9

      conv2d 1 rL0nv2D,                         (     , 14, 14, 64)                     36,928

      max nooline2d 1 (MaxPo心ine2D)             t     } 7, 7, 64)                            0

      c0nv2d_2 α0nv2D)                          (    …’ 7} 7, 64)                       35,928

      Inax_pooling2d_2 (MaxPoo ling2D)          수e,e, 3, 3j 64)                              e

      flatten (Flatten)                         (. ae, 576)                                  8

      dense (Dense)                             (    」：「, 10)                            ’긴，77日

     Total params:  " > Th6 (313.54 KB)
     Trainable params: …      /, (313.54 KB)
     Non-trainable params:      (0.08 B)




＠임베디드 전문가 그룹 윌텍                                -193 -       무단 전재, 복제. 발췌, 디지털화 금지


===== PAGE 189 =====
4부. CNN                                           3과. CNN 기반 Classification


  3 Cony MNIST Classification 예제
                               （3)                              임베디드 전문가 그룹 윌텍


   孕 결과 분석 (Epoch 10회 training 기준）

  Epod18/10
  1875/1875 _         45 2mslstep - vat_accuracy: 0.9733 - val. loss: 0.0864
  Epoch 9/19
  1875/1875 _         Ss 2ms/step 尸 vat_accuracy: 0.9652 - vat loss: 0.1126
 蘇1och 10/10
 :1835/1875                       -val1a뜨브r르드yi0.9747 - vat再loss: 0.0848 1
                      6s 2ins/ste으．
                                                             1 cony layer
                                                               97.47%

 Epoch 8/1o
 1875/1875 _          45 2ms/step - vat_accuracy: 0.9889 - val_loss: 0.0331
 Epom 9/10
 1875/1875 _          45 2ms/step - vat_accuracy: 0.9897 - vat_ toss: 0.0321
                                        -                                    -.



 佰丙ch 10/10                                                                       !
 h875/1875            45 2ms/st르p-=_Y아m르뜨쁘쯔γ三 0.9867 - vat근oss: 0.04091

                                                              3 cony layer
                                                                98.67%




＠임베디드 전문가 그룹 윌텍                -194 -       무단 전재. 복제. 발췌, 디지털화 긍지


===== PAGE 190 =====
4부. CNN                                                                                                       3과. CNN 기반 Classification


  3 Cony MNIST Classification 예제(4)                                                                                                    CODEXPERT
                                                                                                                                           임베디드 전문가 그룹 윌텍



  密 결과 분석 (Epoch 10회 training 기준）
                                                                           ^f憁r Trainin9

    tent_datal0l (lab히 r7/ y:l7Il      in文detaIl](label = 2 싸 1211 tent data[21(label l! y : Lii)     t숀5idatlt卦 (bbel oly I이） test datal4l (lab쇠 d/ yr La])
   0                                  0                            0                                 0-                        0

    5



                                                                                                      巧
  It15
                                                                                                     珊
  괘）

                                                                                                     25 尸

      .        1〔〕        20             n      10        솖             0        l.      솖              b        1.       兀                 .        1.       2.
     testdatal5] (lab이 : l / y Ill)     te寸 datM6] nab이 : 4 ' y 【4])   tent data)?])hbe) 91yr 19])     test_datalol 作毗tel 5 / y (SI)       test_data]91(label 9/ yr (9])
    0                                 l1                             《                                                                 .




              I
                                       5

                                      l0

                                      15

                                      게

                                      乃




@）임베디드 전문가 그룹 윌텍                                                            - 195 -             무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 191 =====
4부. CNN                                                                3과. CNN 기반 Classification


  각 (onv Layer에서 얻은 결과에 대한 고찰                                                    CODExPERT
                                                                                 임베디드 전문가 그룹 윌텍


  每 첫 번째 Convolution Layer의 결과
   G low level Feature의 추출
     te 娥 dat혀잇 11db이 b(Y 193)
   . f




                                                                                  7
   9 和刊의                  .      t   [
        위hr 冬' l
                                                                                  7
                                         / 亡자m' 쩌
                                                「't 孰3
                                         \   뇌F笞，
                                                b'
                                              / :` " ㅣ
                                                          "
                                                              //




 임베디드 전문가 그룹 윌텍
C）                                                   - 196 -       무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 192 =====
                                                                                                                              ■月■ ＂口出· 日
                                                                                                                                                무단 전재, 복제. 발췌. 디지털화금지

3과. CNN 기반 Classification


                                                     임베디드 전문가 그룹 월텍




                                                                                                                              ·르目區區． 目驪
                                                                                                                              旺口■ H妃量目■
                            CODEJ&J
                                                                                                                              ·巨■ n目■ 。
                                                                                                                                      m
                                                                                                                              볍目日m ＇驪n.
                                                                                                                              m． 口日． ．月日
                                                                                                                              ■日． m· 口目目
                                                                                                                              田日巴日日딥떨．
                            각 Cony Layer에서 얻은 결과에 대한 고찰




                                                                                                                              在區口團匹目區目
                                                                                                                              n目■ ·ㅁ■豆■
                                                                                                                              日■ 텨a目圈m.
                                                                      @ 두 번째. 세 번째 (onv이ution Layer의 결과




                                                                                                                              ㅁ．．·．。區陌
                                                                                                                              口· ．區∥ 目貶口        -197 -
                                                                                                                              目뱝· ．■ㅁ區m
                                                                                                                              빼 目 驪 ． 驪· ■阿
                                                                                                                              口a日· 日日■ 口
                                                                                                                              ..．夕口． ㅡ    ＇
                                                                                                                                          .
                                                                                                                                               @）임베디드 전문가 그룹 윌텍




                                                                                                                              오ㅁ 夕 7 日 ． ..
                                                                                                                 .            ．目． －  野
                                                                                                                                     7 7。 口
                                                                                                                              . ＇ 口 夕夕ㅁ 7
                                                                                                          evel feature

                                                                                                                              口7 夕． ． 目 目 7
                                                                                                                              。 7 自 ． ．…오口ㅁ
4부. CNN
                                                                                                                              口   7. ．…7 7 7
                                                                                                                       Low)
                                                                                                                              口 ＇ 오 ． . ' 7ㅁ
                                                                                                                   ,


===== PAGE 193 =====
4부 . CNN                                                                  3과. CNN 기반 Classification


  3 Cony Digit Sign Classification예제(1)                                                                          CODEAPERT
                                                                                                                 ? ftrE .i
   e［예제 7] Cony이ution Layer 3개 기반 Digit Sign Classification 예제
     model = tf.keras.model.s.Sequential()
     modeLadd(tf.keras.Input( shape=(IMG_SIZE, 1MG_SIZE, 3)))
     麻梔rr5記z뀨謙斫弱：      1:i茹芮．   Conv2苡1i'E1irs=64, 下iFri6t＝§ize=3,
                             padding=' same' , activation=' sigmoid'))
     model. ad叭tf keras.j했ers. MaxPool2므｀2些j'.糟쯔:r巍 strides=끄2,
     modeLadd(tf.keras.layers.Conv2D(filters=64, kernel_size=3, i
                             padding='same , activation=' sigmoid' ) )I
     地湫．  L硼鍵（tt‘卜；em뇨」  ，翩蝦r驪쓰i眺￡QQLz以n.g1-}j工，      묘ㅗ쇼tr力t토돋三z川
     而a;e'raircr(ff工F5:Tiyers.〔0nv公又ffTf6   「§＝64∼k하而1.=3汪i百：츙－`
                             padding=' same' ,activation=' sigmoid'))
     model.ad빈侄t-keras. l ayers.MaxPool2D(eool4size=2』 strides=2)j

     model..add(tf.keras.layers.FlattenO)
     model.add(tf . keras.layers.Dense(10,
                      activation='softmax'))                                      9

                                                                                                                     h1;
                                                                .E
                                                      .2                      .
                                                  ,   .-.       _3                -
                                                                                           .
                                                                                           -




                                                      -    。         a.
                                                                     。        -   。    _




                                                           。                      p            a.   三        『
                                                           `[    ㄷ                `J           口        LI       ㄷ    -
                                                  …                       …
                                                                          …




＠임베디드 전문가 그룹 윌텍                        - 198 .    무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 194 =====
4부. CNN                                                                                               3과. CNN 기반 Classification
                    ……                     …∼        표            "   ∼恥
'   →＝    ……    "                                         1                                                    ∼   ∼   1    出「小    ∼        (




    3 Cony Digit Sign Classification예제(2)                                                                       CO三L느r'ERT
                                                                                                                 HjEE 1
         會［예제 7] Cony이ution Layer 3개 기반 Digit Sign Classification 예제
         ● Model summary 결과
           Model:         "   sequentiaF                      '                                                                        --
               Layer (type)                                                           Output Shape                         Par래｝#      ]
               conv2d Gorv2[))                                                        수… J 64J 64, 68)

               max_pooling2d (MaxPooling2D)                                           (    , 32, 32, 64)

               conv2d_1 (Conv2fJ)                                                     （써三쟈샀J 32, 32, 64)                    沁 }｀커筏：繁


               max oooline2d 1 (iaxPooline2D,
                    －■1                         `'   --       `            tJ   '
                                                                                      ＜「；느nn, 16, 16, 64)                         o

               c0nv2d-2 (C0nv20)                                                      (U느결亡＇ 16, 16, 68)                   36,928

               maxjooling2d_2 (MaxPooling20)                                          (ion0, 81 0, 64)                            0

               flatten (Flatten)                                                      (   1, 4O96)                                0

               dense (Dense)                                                          (   =, 10)                           40,970

               Total params: 1노 m『 (455.54 KB)
               Trainable params:
               Non-trainable params:
                                     … (455.54 KB)
                                      (0,00 B)                                                                                         -




＠임베디드 전문가 그룹 윌텍                                                                     - 199 -    무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 195 =====
4부. CNN                                           3과. CNN 기반 Classification

                                                               CODE蓋3ERT
  3 Cony Digit Sign Classification 예제(3)                       얌us'디드 전：르가 그룹 웡텍


  回 결과 분석 (Epoch 100회 training 기준）
 Epoch 98/100
 52/52             0s 7ms/step - val_accuracy: 0.7770 - vat_loss: 1.0982
 Epoch 99/100
 52/52             is J                 s11므r르fy= 0.7674 - vat-toss: 1.1296
                          J煞eA.-..y콰；．』뜨：
 lEpoch 100/100
 臣귑鰻Z              is 7.s鮮ep- - vat accuracy_쿄.7746m- V烈－loss:- 1..162조I:
                                                          1i cony layer

                                 1
 Epoch 98/100
 52/52             is 8n1s/step - vat_accuracy: 0.1007 - vat_loss: 乙3026
 Epoch 99/1脯
 52/52             is 鈿s/st_ee- y_aL`acc쁘:a_cx 0.1007 - val.,toss: 2.3026
 Epoch 100/1羽                                                                 경
 52/52             is ir 스tep- v아_raccu
                                      「acY: 0.1007 - vat toss: Z쿄熙희
                                                                      戈
                                                            cony hyer
                                                            10.07%
    G Layer를 증가시키면 학습이 진행되지 않는 이유는？




          긍깟 力心P了0/6n구그’




＠임베디드 전문가 그룹 윌텍                 - 200 -   무단 전재. 복제, 발췌. 디지털화금지


===== PAGE 196 =====
4부. CNN                                          4과. CNN 발전 시키기




          4부. CNN(Convolutional Neural Network)

            1 F. CNN 4&
             2과. CNN 기뵨현샨
             3* CNN 기빤 Classification
             4과, CNN 발전 시키기




@）임베디드 전문가 그룹 윌텍                - 201 -   무단 전재, 복제. 발췌, 디지털화 금지


===== PAGE 197 =====
4부. CNN                                                                                                           4과. CNN 발전 시키기


  주요 이JN 모델들의 발전                                                                                                                    CODE蓋弘發RT
                                                                                                                                    임베디드 전문가 그룹 윌텍



     1998                                                       2012                         2014 2015 2017



          飇L叫珊楙＼"연                                                               GoogLeNet                   -                     DenseNet
           M띠                                                                                VGGNet                   [actaINet]
                                                                            em 曦 ㅈ＼능치7긔
                                                                 碼
                                                     叫毗
                                  l16AY


            ,,
        1「 二二 - - = 二괘
                         , EIㅌ
                     ＇＝…섭一뇨
                                  I
                             ；J r延i三1
                                                      i1.7       !9 Lay仁rs



                                                                  =
                                                                      7.3

                                                                      ㅓ      m




      LSVRC
          「IO    ILSVRC"1I     IL.$VRCI2             L5VRC'I3    II,$VRC14                    ILSVRC'14      \ LSVRC'15 r              토LSVRC I6 1 ㅅ ,
                                                                   VGGN.4                     Gao'. .MM       \ 由轍比 /                  Enwnbl. t' ' '7
                                                                      기`                        「 r 一 ∼∼一 ㅎ 小 ∼1．떼－ . 」－. ' －一．
                                                                                                                              . 一ㄴ. ；ㅗ 一 .    小 m1 1

                                                                      l
                                                                                                 L Jou, Le- b니∥11L디LUIWVVCWILOJ                Itt 」
                   !,'   ,   …，,，뼈



                              SI,nC, "m                           包소 ’麓익 令易 …」닒,, .,\,J,i, ／吃
                              (   -   d)   七/   t7



                                                /




⑧임베디드 전문가 그룹 윌텍                                           - 202 -           무단 전재, 복제, 발췌, 디지털화 금지


===== PAGE 198 =====
4부. CNN                                                                                4과. CNN 발전 시키기

                                                                                              COD
  ImageNet and ILSVRC                                                                         임베디드 전문가 그룹 윌텍

  Q ILSVRC(lmageNet Large Scale Visual Recognition Challenge)
   ● 대용량의 이미지／비디오에서 객체를 분류／인식하는 알고리즘의 성능을 평가
   ● 이 대회에서 우승한 알고리즘들이 이미지 인식 분야 발전에 큰 역할을 함




  I Source: irnage-net.org/chailenges/ISVRC/2014/ and https://Iink,springer.com/article/101007/sl 1263-019-01247-41




 임베디드 전문가 그룹 윌텍
C）                                                   - 203 -        무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 199 =====
4부. CNN                                                                                                         4과. CNN 발전 시키기


  LeNet                                                                                                                 CODEXPERT
                                                                                                                           임배디드 전운가 그룹 윌텍

   .'Gradient-Based Learning Applied to Document Recognition' 논문(1998)
   各 모델 검증 위해 제작한 Dataset 4 MNIST Handwrite DB

                                             C3 ` maps 16@10*10
                        Ct feature maps                       S4: t. maps 16@5x5
                        6@28528
      32x32
         UT                                 S2「 maPS
                                                                                             layer P6: layer   OYTPUT
      臂，
                                            6@14x14                                                            10
                                                                                                    84




                                                                                            Full e nrectmn
                                                                                              7一                    -   Gaussian   connections
                 Convolutians             Subsar까rhng      Convolu6ons            Subsampling        Full connection
                                                                                                         ∼＼



           "Activate Functi。
                           n:                                       i-   :-   -

                                                                                  Pooling:         , .   "




           ,     Sigmoid                                           i.werage pooting

              [Source: Gradient-Based Learning Applied to Document Recognition(1998), Yann LeCun and others]




@）임베디드 전문가 그룹 윌텍                                           - 204 -                 무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 200 =====
4부. CNN                                                                                                                     4과. CNN 발전 시키기




  @口Architecture
     Activation i-unction 깍 KeLutKectiiiea iinear unit as non-linearity)
                                      . .   J,                ,   .   , .   ,       . . ..       .       .              ,      .   .



                                  .   .             \   ∼∼－           ，一
                                                                                --－∼－            －∼－    →＼∼－
                                                                                                               /----/
   .`'   h月．
         ■1 ■ H
                11+:
                 ~ `~
                      r;
                      ,d
                         1기
                         ~
                             1쿠 雰
                           `. m=- -`
                                     슈
                                     .




         瀋勿“학i；
              卜76A GTX 580 3GB GPUs, Memory문제해결. 연산시간줄임
   G Overlapping pooling
    4 Average p。。ling [ll !                  (Max                  。ling AF.
                                                                  p。                         .




         ,4. Window size: 3 X 3. strides: 2




@）임베디드 전문가 그룹 윌텍                                                                    - 205 -            무단 전재, 복제. 발췌. 디지털화금지


===== PAGE 201 =====
4부. CNN                                                                                                   4과. CNN 발전 시키기


  ReLU(1) 「 小4샌→                                                                                                         CODEXPERT
                                                                                                                          임베디드 전문가 그룹 윌텍


  Q DNN에서 Sigmoid Function의 문제점                                                                       St며n이d Fttn1ㄷtt이，
                                                                                                                      f(x` - l / 1 , erp《，
                                                                                                                                         z1
                                                                                                                                     ■ 기．叫



   . 미IN의 Optimization 방법                                                aa
                            '                                                                                             i
    4 Cost Function의 미분 값을 Backpropagation 해서 진행                     . '


      x Cost Function의 미분 값 + Gradient           즌

                                                                                                                                            1
   .Sigmoid Function 기울기 문제점＇
                            〃
                                                                                                                                            1
                                                                                                                                            1
    /2 x= 0 근처의 영역 * 기울기가매우큼                                                      `     -     -       -             L/ :m         -       』




    14- x < -5 혹은 x> 5 영역 + 기울기가 0에 가까움                                               .`.                           .                                       .        7     柶；
   ● 아주 깊은 DNN 신경망에서의 Back Propagation
                                                                                                                    0<                                                     Cost
    /$-0에 가까운 기울기가 계속 곱해간다면
                                                                                                                                                --



    4- 더 이상 기울기가 전달되ㅈ 못하는 상황 발생
                                                                                                                             n-       ----
                                                                                                                               ㅅP"JPdVdUUII
                                                                                                               ＜너
                                                                                                                             .d｀




                                                                                                               ㅡ 트mㄱ ，
      + Vanishing Gradient Problem
                                                                                                          -1
                                                                              ；닉m빽N                                                                  됴낙m乙           尸娑딱여    尸싣격．
                                                                                             ；닉mㄱ W                      ；닉m맥m         ；닉mㄱ m
                                                    +
                                                    *
                                                    *                                                                    r        斗                             今




    2e1L` - 甘V8冬kk' , 尸: _                              I-
                                                             -   -   -
                                                                         H-                 -－→           --


                                                                               m,           =m=       ..-           '




             -   '-
                      tX1
                                )vV   .




@）임베디드 전문가 그룹 윌텍                          - 206 -   무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 202 =====
4부. CNN                                                                              4과. CNN 발전 시키기


  ReLU(2)                                                                                  CODEAPERT
                                                                                            임베디드 전문가 그룹 윌텍



   넌    （   『，   「）   =   max   (0,   x)
   0 장점
                                                                                         只el u F un이」
                                                                                                    0【1
       ,4x가 양수인 영역에 대한 Gradient 4 1                              l.


                      x Backpropagation 구현 및 실행에 있어서 이득이 있음
                                                                                                                   1

                      x Sigmoid의 기울기 연산시에는 지수함수 연산 필요                                                              1
                                                                                                                   i


                      x Neural Network의 크기가 클 때는 학습속도의 차이가 큼
   .             단점
       ,4- x가 음수인 영역의 전 영역의 기울기 * 0
                      x 이를 극복하기 위해 Le訃
                                     （y ReLU 같은 함수도 사용할 수 있음
                                                                      -l(} 毛）   -7   .        . .    25   5.   7   0月

       〃 X가 0인 지점에서 미분 불가
                      xx가 0일 때만 특정 값으로 미분 값을 정의하여 해당 상황 극복
       今 이런 단점에도 불구하고 상대적으로 많은 장점으로 인해 DNN에서 많이 사용 됨




@）임베디드 전문가 그룹 윌텍                                  - 207 -     무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 203 =====
4부. CNN                                      4과. CNN 발저 시키기




  @ Overfitting을 방지하기위한ReguIarzation 뻗읜，
                                       읠登
   穹 일정 확률로 노드들을 사용하지 않게 만듦
                          （훈련 시 사용하지 않을 노드 무작위 선정）
    '4. 해당 뉴런과 연결된 모든 입출력 연결들이 끊어짐
   密 남은 뉴런들은 스스로 중요 특성 학습, 특정 뉴런에 의존하지 않게 만듦
    '4. 특정 뉴런과 지나치게 연계 * 다양한 뉴런과의 연계를 통한 학습 어려움
    /1' Overfitting될수있음              + 驍아？H기白t g吟 *Y'="｀쒸
                                                  수怪半｀.n赫「'0雜｀




@）임베디드 전문가 그룹 윌텍           - 208 .   무단 전재, 복제, 발췌. 디지털화 금지


===== PAGE 204 =====
4부. CNN                                       4과. CNN 발전 시키기


  Data Augmentation
  Q 이미지를 다양한 방법으로 변형하여 모델에 입력
   ● 데이터 수가 작아도 부풀려서 사용 가능
         섶늪의雙竺된ii Overfitting雙I횬.1!PF 있음
     CNN읜，
   . 시exNet 이후 거의 모든 모델들이 사용하는 보편적인 방법
   0 Data augmentation의 예




                                       흩흰) tL'      뉜 :t   '
           · 唵 , 치鮮． 2t,on' l i/QvT ．→




@）임베디드 전문가 그룹 윌텍            - 209 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 205 =====
4부. CNN                                                        4과.（그州 발전 시키기


  Digit Sign에 ReLU, Dropout 적용 (1/5)                               밈뼈디드 전문기 그룝 묄텍

  Q［예제 81 ReLU. Dropout을 적용한 예제
    model. = tf.keras.models.Sequential()
    # input 始yer
    model.. add(tf -keras.Input(就,ape=(IMG_SIZE, 1MG_SIZE, 3)))
    # cony 1
    modeL add(tf.keras layers.Conv2D(64,3,padding='same', activation=' relu'))
    modeL add(tf . keras.layers.Dropout( rate=0.4))
    modeL add(tf. keras.layers.MaxPool.2D(pool_size=2, strides=2))
    # cony 2
    model.add(tf .keras. layers.Conv2D(64, 3, padding='same', activation=' relu'))
    model.add(tf.keras. layers.Dropout(rate=0.4))
    model.add(tf.keras. layers.MaxPool2D(pool_size=2, strides=2))
    # cony 3
    model.add(tf.keras. layers.Conv2D(64, 3, padding=' same', activation=' relu'))
    modeLadd(tf.keras. layers.Dropout(rate=O. 4))
    model.add(tf.keras. layers.MaxPool2D(pool_size=2, strides=2))
    # dense layers
    model.add(tf.keras. layers.Flatten(name=' flatten'))
    model.add(tf.keras. l.ayers.Dense(10, activation=' softmax ' ))




＠임베디드 전문가 그룹 윌텍                      -210 -     무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 206 =====
4부, CNN                                                                   4과. CNN 발전 시키기

                                                                            CODE X PERT
  Digit Sign에 ReLU, Dropout 적용 (2/5)                                        임베디드 寸？기 그름 器텍


   G Model summary
          Layer (type)                          Dutput Shape                  Par出1 #

          convid (,,onv2D)                      (…낟－, 84…／닙 64)                 l 3 '9걋

          dropout (Dropout)                     (m1∥＝ , b졉＇ 亡4J 紬’;)

          max_pooling2d (MaxPoo1ing2D)          신… ， 弦，薑갸】 64)                          二〕



          conv2d_1 仁0nv20)                      (.1    , 驪，在，64)               >b m' `,

          dropout_i (Or아'out)                   (      J   긴」슭’ 크걋j 64)

          maxpooling2d_i (MaXPOming2fl)          (    「…hb j표, 64)

          conv2d_2 (ccnlvlD)                     和∼n」J 三＜} lb】64)              걋컨 , → ,,，已



          小opout_2 (Dropout)                     수ㅉ；, 16J 16, 64)

          max_pooling2d_2 (MaxPoo1ing2D)        （식」
                                                  ∥즌, g, 8, 64)

          flatten（차atten)                        甘 쩍눙 4096)
                                                （」

          dense (Des+)                          （立－J 10)

      Total params:           (455.54 KB)
      Trainable pararns;        6 (455.54 KB)
      Non-trainable pararlis;   (0.00 B)




@）임베디드 전문가 그룹 윌텍                                -211 -          무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 207 =====
4부. CNN                                                4과. CNN 발전 시키기


  Digit Sign에 ReLU, Dropout 적용 (3/5)
  Q 추가 적용한 내용
   J Cony이ution Layer의 Activation Function: ReLU로 변경
   mDropout 적용




＠임베디드 전문가 그룹 윌텍                  -212 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 208 =====
4부. CNN                                                4과. CNN 발전 시키기


  Digit Sign에 ReLU, Dropout 적용 (4/5)                        CODEXPERT
                                                            임베디드 전문가 그룹 윌텍


  Q 결과 분석 (Epoch 100회 training 기준）
   Epoch 98/i에              1 convolution layer 3 77.46%
   52/52            Os 7ms/step - val_accuracy: 0.7770 - vat그oss: 1.0982
   Epod199/i에
   52/52            is7 J. te.p.-y.힌：-jfsyr.cy 0.7674 - val.-loss:. 1.1296
  :Epoch 100/100
  臣ZL2                 7묘5／쟌르p뇨＝-y9l口크뜨뽀르드y으m吼zz艇－=-x아∼k？돋兌三．．工
                                                              「盤트蚣．
                                                                  i

   Epoch 98/100              3 convolution layer 3 10.07%
   52/52            is Thus/step - val_accuracy: 0.1007 - va1joss: 2.3026
   Epoch 99/1騁
   52/52            is 8m5/s    -vaLacc씬:a. cyF 0.1007 - val loss: 2.3026
                            tel-                                          곁
   Epo《余 100/100
   52/52
  / mmmmm                   盤 － val_accura드y요_立l塑z-=-x련흼．
                                                        士？트췬길궂r큐麒희

   Epoch 98/100     3 convolution layer + ReLu + Dropout 4 94.48%
   52/52             Os 4ms/step - val_accuracy: 0.9472 - val_loss: 0.1959
   Epoch 99/100
    2L52             Q읖·由隘z澈辦ㅍ」＝.＇카．
                                   』J=1;i1r긁｀;yj－奐949立＝,.yal-l. 돔듀요ㅃ乳．
                                                                     zl烈，
   Ep。ch 1。
          。/1。
             。
  ;s2i52             s_ Arp&1s.tep=-ya]._ac1=ucacyi∼夔盈鯤松＝보a.t-I끄됴됴．
                                                                  =－丸＇22.1郞




C）
 임베디드 전문가 그룹 윌텍               -213 .    무단 전재, 복제. 발췌, 디지털화 금지


===== PAGE 209 =====
4부. CNN                                                                                            4과. CNN 발전 시키기




          O/ y「｛OJ) t.stdataf80JfIat I 1/ y. I1J) 듬estdtat12甲fhb텨『2 / y - f21) 듬ect L't.i'1F0 hU




@）임베디드 전문가 그룹 윌텍                                        -214 -            무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 210 =====
4부．
  CNN                                                     4과. CNN 발전 시키기


 Regularization                                              cODE    PERT
                                                             임베디드 전문가 그룹 묄텍

 『？ 목적
  .Overfitting을 관리하여 학습의 효과를 높이는 것
  心｝ LJ I쇠드．
  `,= d ㅂ ㄹ

  . Data Augmentation
    Is. 같은 종류의 data를 늘리는 방법
  . Dropout
    4. 학습 시 model의 parameter 수를 조절하여 모든 parameter가 골고루 학습
  . Weight regularization
    ,2- 특정 parameter가 커지는 것을 직접 적으로 관리
  . Batch Normalization                       ∼   ,,\




    〃 층이 깊어지면서 발생하는 covariance에 대한 보정으노 학습 효과를 높임
         --－∼∼－   --        ，∼   ------－→∼－




＠임베디드 전문가 그룹 윌텍                  -215 -           무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 211 =====
4부. CNN                                                                                                                                              4과. CNN 발전 시키기


  L1/L2 Regularization (1/4)                                                                                                                           임볘디드 전문가 그룹 욀텍


  @ Weight 값의 분포를 제어함으로써 Overfitting을 방지하는 기법
   孕Cost function에 Regularization term을 더해줌
                                                           1         "
     Li Regularization: Cost = Cost。4 AD삐
                                                                     Jm긔
                                                                                      卜빠→ Regularization term

     L2 Regularization: Cost = Cost0 - A＞ㅍ w2                                                    Cost 4 Cost function
                                                                                                 Cost0 + 기존 Cost fun硼on
                                                                                                 ) 4 Regularization parameter

  警 동작 확인을 위해 단순한 Linear regression을 기준으로 분석
   今1. Hypothesis 설정 +                               H(x) = wx + b

   .2. Cost function 4 Mean squared error 적
     No   regularization: .硼《    （W,
                                            b)   ＝
                                                      楡>       ;(H
                                                                            (z)   ．   川'               2m
                                                                                                                 -
                                                                                                                     (7,
                                                                                                                                 ！나卜



     LI regularization: cost                         綸E 四＋b-                                                시뻐                                 i i
                                                                                       y)
                               (w,
                                                                      （工，
                                                                                            2-    1-
                                                                                                                           ；中－
                                       b)        ＝
                                                                                                                                  橫:
                                                                                                                                       J: =1

     L2 regularization: cost(w, b)：굶尤（=，粃，b-琇)2-iIAw2그
                                                 l         ＇ㅜi
                                                                                                            L




@）임베디드 전문가 그룹 윌텍                                                              -216 -                            무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 212 =====
4부. CNN                                                                      4과. CNN 발전 시키기


  L1/L2 Regularization (2/4)                                                       임베디드 전문가 그룝 윌텍


   03. Cost function의 w에 대한 미분
     N0 regularization:         (w, b) = 슬 x (xi(zw+ b-y))
                                           芒上 i




                                           읊＞D幟 明＋ii－的》＋A,ifw >0
                                              （z，
     L1regularization:
                                           슬＞如d我雉＋b－跳）}－入，ifW <0
                                                 1= l
                                            1탬

     L2 regularization= 읊coat    ,b) = 읊          跡(xw+b- 餉))+2Aw


   0 4. Weight 업데이트
                                                                   ''
                                                                             Ii 는 Learning rate
     No reguhrization: w,et· = 泌                        , b)＝功－슷 乞(zi(zw+b-〃))

                                    －슷＞걋，
                                        (:rm＋뇨挑）
                                               )F=^,if，
                                                      『 之o
     Li regularization: w,                                                啼畔： Wnew는 상수만큼 증감
                                          (xw+b- 號)fli- 入，ifv <U
                                      in＞玉，                                  깆；丁 U 孔小十i "
                                        i=i
                                                                              욍윈꺼／ +
     L2 reg표arization: W*ef         츨乞恪（我四+ b -轍）
                                                [r2A明                     琫心
                                                                           《wnew는 w에 비례하여 증감




@）임베디드 전문가 그룹 윌텍                                         - 217 -    무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 213 =====
4부. CNN                                                 4과. CNN 발전 시키기




    4- Cost function을 w로 편미분 하면 Regularization term은 상수가 됨
    Il- 따라서 Weight를 업데이트 할 때 Weight에서 상수 값을 빼거나 더하는 효과
    ／卜 결과적으로 작은 Weight들은 0으로 수렴되고 몇 개의 죵요한 weight들만 남게 됨
   G L2 regularization 4 Weight decay 로 불림




    4- Cost function을 w로 편미분 하면 Regularization term은 w의 1차식이 됨
    4. 따라서 Weight를 업데이트 할 때 Weight에 일정 비율로 영향을 줌
    4- Weigh마 101E00i 되시 않고 특정 Weight가 비이상적으로 커지는 것을 방지
    4- Weight들의 값이 2르'1I 분포하게 됨




@）임베디드 전문가 그룹 윌텍                  -218 -     무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 214 =====
4부. CNN                                                             4과. CNN 발전 시키기


  L1/L2 Regularization (4/4)                                            임베디드 전문가 그룹 윌텍


  @ Keras의 Li IL2 regularization 지원
   聾keras는 Dense. Convi D. Conv2D, Conv3D에서 Li IL2 Regularization을지원
    4- Dense layerOll Li regularization 적용 + O.01은 ).(Regularization parameter)
      model.add(Dense(1000, kernel_regularizer=tf.keras.regularizers.11(a.ei), .,,))
                                                  rm＼   ∼／＼→／ `/


     4- Conv2D layerOll L2 regularization 적* + O.01은 .(ReguIarization parameter)
      model. add(Conv2D(256, 3, kernel.jegularizer=tf.keras.regularizers.12(0.0D, .. ,))


                                                         小＄,,1t 二 C) . .이




@）임베디드 전문가 그룹 윌텍                        -219 -          무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 215 =====
4부. CNN                                                  4과. CNN 발전 시키기




  @ Internal Covariate Shift
                          （공변량 이동）
                     一，,/7→   ＼/,／入／     \-1
   ● 입출력 규칙은 Training, Testing 시 동일해야 좋음
    Is. 실제로는 입력의 분포가 변화되는 공변량 이동이 발생할 수 있음
   G Layer가 많아질수록 학습에 부정적인 영향을 줄 수 있음




＠임베디드 전문가 그룹 윌텍                        - 220 -   무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 216 =====
4부. CNN                                                                                                                                           4과. CNN 발전 시키기


  Batch Normalization(2)                                                                                                                                      임볘디드 전문가 그쭙 윌텍




    Input Layer                 Batch 嫩rmalization에 의히i
   평균0' 표준편차 1                 평균 0, 표준펀차 1의 분포로 복귀
                       1




                                                                                                           B                                                  ^/. ／꽂hmc: zt (U'Ttt (1



                                                                                                            n
                                                                                                            닐―珊
                                                                                                              r
                                                                                                               =   {Xp.                  .rn}


                                                                                                                          翔
                                                                                                               1   …STEPi:CakuateB的ch Stitistics

                                                                    ㅡ

                                                                                                             ？닉斗 暢＝!,，乶
                                                                                                               B
                                                                                                                          1
                                                                                                                          - m
                                                                                                                      （ - 功"              乞M    幻



                                                                                                                          STEP 2: Normalize Layer Inputs
                                                                                                                                                      ,r』     〃 什


                                                                                                                                                      V "i:   1       r


                                                                                                                                 STEP 3: Scaling and Shifting

                                                                                                                                                l/' = 갸J,' + 躬）
                                        ／二
    . 평균 = 0, 표준뿌차＝1로 만들뗏必쓰쁘드으Y카브르坐心唾줄일
                           "                 UU.
      '2.                                      .
                                                               ?I       i                                                                                1
                                                                            4:
                                  1tj
                                                                                                                                                                                               ,
                                                         7fl
            Training
                                                                                                                                                              t
                                                                                                                           :)CzbLcrtc                             (                       ':
                                                                             :.
                                                                                       "=
                                                                                  ""
                                        \                                                        -( e눠l)I- - 午쪄 7rAr4`' t9γ l'1．색，                    「녀디                            r '" '"



                                        1／스－-
                                                   ,-,                                           六八澄er’                           기乙1r            4                       r   ' ""

                                             \ I               \                                          ` '" /, I                      -VPA



                                  "-                                                  "「"］乂 .
                                                                            린凡＼ 弓叩 . a｝




        포처七 ＆枷珖＼小 앞펴 來노ㅟ＼ 삭윗




＠임베디드 전문가 그룹 윌텍                                                                        - 221 -            무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 217 =====
4부. CNN                                              4과. CNN 발전 시키기




  @ ImageNet으로 train된 model을 활용하여 문제 해결
   J Pretrain된 model의 Feature Extraction part를 사용
   好Classification part만 다시 training
   . Feature Extraction part도 train 한다면…




＠임베디드 전문가 그룹 윌텍                    - 222 -   무단 전재, 복제. 발췌, 디지털화 금지


===== PAGE 218 =====
4부. CNN                                                                        4과. CNN 발전 시키기

                                                                                       CODEAPERT
  적용 가능한 Pre-trained Model                                                             =；볘니노 친卜’기 그器 왑긱



          Documentation for individual modets
                 M0det         Size Top-i Accuracy Iop-5 Accuracy Parameters Depth
           Xception          88 MB           0.790          0.945 22,.910,480 126
           VGG16            528 MB           0.713          0.901138,357.544    23
           VGG19            549 MB           0.713          0.900143,667,240    26
           ResNet50          98MB            0.749          0.921 25,636.712
           ResNetlOl        171MB            0.764          0.928 44,707,176
           ResNet152        232 MB           0.766          0.931 60,419,944
           ResNet50V2        98 MB           0.760          0.930 25,613.800
           ResNet1O1V2      171MB            0.772          n938 44,675,560
            *esNet152V2     232 MB           0.780          0.942 60,380,648
           InceotionV3       92MB            0.779          0.937 23,851,784 159
           Ince. 's ResNetV2215MB            0.803          0,953 55,873.736 572
           Mot川eNet                          0.704          0.895 4,253.864     88
           劾6bUeNetV2        14 M8           0.713          0.901 쵸538,,984     88
，嘴鱗       :DenseNet121       33MB            0.750          0.923 8.062.504 121 :
           DenseNet169       57 MB           0.762          0.932 14,307.880 169
           DenseNet201       80 MB           0.773          0.936 20,242,984 201
           NASNetMobile      23 MB           0.744          0919 執326,716
           NASNetLarge      343 MB           0.825          0.960 88,949,818
                                                    I Source: https://keras.io/applications/ ]

                                        勿




(＼하숙
    -Er       .
                  .    "
                      ‘「" " cM\
                       畛"蝦 ct 3Mfr
                                  「Mk       "1,
                                              1    )1\   '*   ".   1,
                                                  ' Db" )\Z ).7/ 나「'"' '컥




@）임베디드 전문가 그룹 윌텍                            - 223 -           무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 219 =====
4부. CNN                                                                                     4과. CNN 발전 시키기


                                                                                                     임버1디느 전문가 그룹 윌텍


  @ 2014 ILSVRC에서 GoogLeNet에 밀려 2위 였지만 더 많은 관심을 받음
                                                                          CorwNet Configura,tion「
   . 간단한 구조와 훌륭한 성능                                          Ad→kN
                                                                                                     -
                                                                                                                            r         -   =
                                               蘆l weight   l 】weight     l3 weight  16 weight I I6 weight 1옇 】9 weight
   今 많은 연구의 기준 모델이 됨                             lavers       l avers      1비／ers     layers 1    layers   1 1avers
                                                                    input (224 x 224 ROB irna水)           1.
    4. 3만회 이상 참조됨                              c0nV] 64    eorrv3巧4    cons364      c0nV玉64 i conv, 64 1 c0nv玉64
                                                                                                              3-
                                                             LR,       eons3=64     coov3-64 1 e。nv3- 64 1 conv3-64
   啼CN!＼』망 깊이에 따른 성능 연 1                                                       tnaxpool       ·
                                                                                    co.w3-重28 1 conv3-I28 1i conv3i28
                                                                                                                       ;1
                                               conv3-128   runeS- l 28   conv3d28
    46가지 모델로 성능 비교                                                       convJl28 conv3d28 L conv3-I28 I 1 conv3-I2tt
                                                                                 rnaxpool        ;                     I;
                                               conv3-256   conv3-256     c.11v玉256      conv3-그56 1 conv3-256 .          256
   .19층
      （VGG-19）
             까지만 사용                            q가】v3-256   conv3-256     conv3-256      conv3256 i conv3-25(, . c。nv3- 256
                                                                                                                            ;conv3-
                                                                                        cons1-2쇳1 I eonv玉256 . 1 心》  nv3256
    4. 더 쌓아도 좋아지지 않음                                                                              i            ~ 최 co11v工256
                                                                                 maxpo이           i           '．최
                                               co∥v〕－512   c1ㄲ｝v3-512    cony3-5 ! 2    conv3-5i2 콰 eotw3-512 ~ 최 conv3-512
                                               coon3*512   .()nv玉5口      cony3-512      conv3-512    0WN子引2 ~            512:conv3-
                                                                                        C。 NVI-512: 口mv3-512 1 conv3- 5 12
                                                                                                              1 e。   nv3-512
                                                                                 r11axgo이         '           1`
                                               c｛겨1v3－引2
                                               eonv3-512
                                                           ccnv3-5l2
                                                           conv3-5i2
                                                                         eenv3-512
                                                                         eonv3-引2
                                                                                        conv3-시2【 cons
                                                                                        conv3-512 1 c。 ns，
                                                                                                         三：        ;:;:
                                                                                                                1 c{)nv3=q2
                                                                                                                i conv3-512
                                                                                        convl-512 . coflv3-5l2i i cony玉시？
                                                                                                  I-            i conv3-512
    [Source: Simonyan, K., & Zisserman. A.                                       maspo이           .          【i
    (2014). Very deep convolutional networks                                    FC-4096           ;           i;

                                                                                                 : VGG16[jTVGG19
    for large-scale image recognition. arXiv                                    FC-4096           :   ＝쩍 －ㄱi：    巴－ 毖m
    preprint arXiv:1409.1556.]                                                  PC- moo
                                                                                s。  ft-max                                   -



                                                                                                                   -


                                                 L乍N                                                  奴r1:,.1ㅈ낑흖t
                                                                                                     수＼




@）임베디드 전문가 그룹 윌텍                               - 224 -           무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 220 =====
                                                                                                                                                                                                                                                     무단 전재. 복제, 발췌. 디지털화 금지



4과. CNN 발전 시키기
                                                                                                                                                                                                               캭 순e긴 뷰블嗟 갓순穹 白f.，디 川숫 뇽차 .



                                                                                       O                                                                                                                                                                ^
                                                                                                                                                                                                                                                        ^
                 PERT                                            X
                                                                 m尸乞 一小8               ymF， ∼8                                                                                                                                                                         z
                                                                                                                                                                                                                                                                       Z
                         임베디드 전문가 그룹 윌텍


                                                                  。。。m u
                                                                       닙               。。H U
                                                                                           나
                 C0DE
                                                                  四小。 斗U "             山이口寸Uㄴ
                                                                                                           [Source: https://medium.com/coinmonks/paper-review-of-vggnet- 1 st-runner-up-of-ilsvlc-2014-image




                                                                 山잉4Y                  ．出口후口Y
                                                                                       g a 넓＂돋
                                                                  。。。 Xm>                ＞ ㄷ8
                                                                                      스m m
                                                                 八二小＞ ㄷ口U             스띠 띵ㄷ 。
                                                                                            U
                                                                 의변m> L
                                                                      。p              八H띠 Dㄷ 。
                                                                                             U
                                                                     >C
                                                                 의小． m O
                                                                       나，             八H띠 엥ㄷ 8                                                                                                                                                  놔）
                                                                                      a 麗 Xm>
                                                                                                                                                                                                                                                -7
                                                                  。。。ㅈm돌              스뱍m＞ ㄷ 8
                                                                                                                                                                                                                                             \?y!
                                                                 의쑹m> cQU             엌小m＞ 尸즈U
                                                                 었小小＞b 닢              가 나 깝 ＝O
                                                                                             U
                                                                             VGGd.6                V6G49
                                                                                                                                                                                                                                                     ㄷJ
                                                                                                                                                                                                                             ｛사℃∼岷느 쓸＋慨 ·



                                                                    >L
                                                                 스겨 m 。               `H뿌m> C
                                                                                            。U
                                                                      一니
                                                                                                           classification-d02355543a1 1 ]




                                                                                      石 요 蘿흩
                                                                  。。。 ×出＞             山小斗m＞ 尸5U
                                          @ VGG-16과 VGG-19의 구조




                                                                 。nN出＞ ㄷ。U            口띠현母ㄷ 0
                                                                                            U
                                                                 果히m＞ ㄷ。U             口띠斗母ㄷ 。
                                                                                            U
                                                                 累싼m＞ ㄷ。U             口mn丙＞ ㄷ。U
                                                                                                                                                                                                                                                     ＠임베디드 전문가 그룹 윌텍
                 VGGNet의 구조




                                                                 石 蠟 낫輜흩               。 읖 Xm姃
                                                                 m＂난잎ㄷ 。
                                                                       U              ㅁ엿 ＇
                                                                                         的＞ 尸5U
                                                                 m의H＞듀
                                                                     →U                스 出 ＞ ㄷ。U
                                                                  。gXm                丕 흩 xm휸
                                                                        z
                                                                        <
                                                                 q
                                                                 A일ㅆ ＞C。 U            寸
                                                                                      ．,＞ ㄷ。u
                                                                                        m
                                                                 寸 >r
                                                                 口 m 1
                                                                     OU               더山써＞ ㄷ。u
4부. CNN

                                                                  m驢f                  m軫ㅌ


===== PAGE 221 =====
4부. CNN                                       4과. CNN 발전 시키기




  @ Cony Filter를 3x3으로 고정
   .5x5, 7x7 대신 3x3을 여러 번 써도 같은 효과를 냄
   9P＃이 줄어들고. 이미지 크기의 감소가 적어 Layer 증가에 유리
   口 이후，
       캭큰fi艸改C뺏읜，
                칸봅인윳




          卄；乞 나 \》兀뼈, +k艇叭 키
                           "닒 料叫
          ( c1v 田m
                             寸枷＼"「'「"""1



@）임베디드 전문가 그룹 윌텍            - 226 -   무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 222 =====
4부. CNN                                                                             4과. CNN 발전 시키기




  @ ImageNet으로 학습된 모델이 제공됨
    tf . keras. applications, V6616(




    tf.
    :7inputtens   keras.   applical4。   然0   /   ns. VGG19   (.   1




@）임베디드 전문가 그룹 윌텍                                                  - 227 -   무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 223 =====
4부. CNN                                                                                                                                                                  4과. CNN 발전 시키기

  ;;．사． …．－「∼－,:：螂∼曳…
                6，   ∼∼出                                                                                                                     餌
                                                                                                                                                                                                               旨굻／/
  VGG-16 Fine                                                                                 (1/
                                                                                                                                                                                卞室코1；
                                                                                                                                                    「…    「∼…



                                                          Tunina
  孕［예제 91 Pretrain 된 VGG-16 모델을 디FAR10에 맞추어 Fine Tuning
   G Pretrain 된 VGG16 모델 로딩
    걔6_SIZE = n2                                                                                                                                                                                                      -
                        tensorflow.              keras.
                                                                               application
                                                                                                               ,   s    import              V6616
    froml VGG16
    m。  del
                           "imagenet
                                (weights=
                                                                                                          ",




    ,，』，include_top=
                    False,
              tensor=
               input_                                                               (shape=                            SIZE, 1MG_SIZE,                                 ))半ts J (.cs         \
                                                                                                                                                                                                                      >Y
                               ()
                                                                   Input                       (IMG_
    m。
                                                                                                                                                             3)
         summary
        del.
                                                                                                                                                                                                        e*
                                                                                                                                                                                        I^ ,      `` = .       → r . ＆니

    Layer (type)       Output Shape          Parai #                                                                                                              .      . ·
    －一－=----＝→－－一一－一－小＝=--=--=-=------=                                                                                          block4_coev2 (Coen28)                (None, 14, 14, 512)                  2359838
    Inputi 이ntutLayer) ](Ncee, 112, 112. 3)] .
                                                                                                                                 b1ock4_cenv3 (Coev2D)                            히12)
                                                                                                                                                                      (None, 닉．녀. 5                        俎ㄷnF1꺼
    blockl_conv( (Ccnv20(                       (None. 112. 112, 出）                                    783
               ---                                                                                                               비od<&DooI 여aXFb＜川ng2D(               (None. 7. 7, 히2)                     0
    벼odd.cony2 (Ccev20)                         (None. 112. 112. 64)                           泌望8
                                                                                                                                 비od5_convl (Ccqiv28)                 (None, 7, 7, 히2)                     23590818
    blockl..pool (Maut'ool in2t1)               (None, 56, 56, 64)                             0
                                                                                                                                 비od(5_coev2 (Cony乙）                  (None. ?. ?. 히2)                  刀56088
    b1ock2sony1 (Conv2U)                        (None. 56, 56, 28)                             7         6
                                                                                                                                 이ock5_conv3 (Coev28)                 (None. 7, 7, 512)                    2359568
    b1ok2_ccew2 (Conv28(                        (None, 56. 田. 128)                                     47564                             --         --
                                                                                                                                 blod&po이 (NoxPool 1ng20(             (None. 3. 3. 히2)                     0
                                            .                .             S                                                     ----－∼－         --－如∼－     ----－→＝m一－                  ==----=--=---                 l




＠임베디드 전문가 그룹 윌텍                                                                                         - 228 -                            무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 224 =====
4부. CNN                                                                                                4과. CNN 발전 시키기


       VGG-16 Fine Tuning (2/6)                                                                               CODEXPERT
 -m*      m∼           口－   卞논，
                                                                                                              임베디드 전문가 그룹 윌텍


        .0旦 t4Layer* FineTuning2롯AF '4(! F01츠J Layer은 *Oi 人 제
        for layer in model.layers[:-41:
            layer.trainable = False
        for    layer              (               model.
               print              (layer,
                                            iny
                                                      layer,
                                                               layers:
                                                                         trainable)
         <tensor시 o,.python.keras.englne. input_layer. InputLayer object at lJx7fb2b(Jlb939> F키se
         <tensornow. pyt h에.keras. layers.conyoluti예비 .Conv2D object at 0x7fb2b미eclYb0> F히se
         <tensorflow.python.keras. layers,conv이Uti에비 ,Conv2D object at 0x7fb2b미b9be0> False
         <tensorflow.python,keras. Iayers.pool lng.MaxPo이 ing21) object ab[lx7fbb0lede8l)> False
         <tensorflow.python,keras. layers.cony이utlon히 .Coiw2D object at Dx7tb 0la3& ]> F히se
         <tensorn ow python, karen. I ayers.conv이uti어繃 . Gonna) object at 0x7tb2bfllalctl>「키se
         <tensorflos.python.keras. layers,pool ing.MaePo이 inga) 아>j ect at 0x7fb2b01363g0> 「：키se
         <tensornow.python.keras. layers.conv이ution키 . Conea〕object at 0x7fb2b013bc18>「키se
         <tensorflo,.python.keras. layers.conv이Ut ion키 ,Conv2D object at 0x7fb2b0l3beb8> F히Se
         <tensorflow,pythoe上eras, layers. cony이utional ,Conva) object at 0x7fb2b1]l 495w:>「키se
         <tensorflow.python,keras. layers,po이 leg. MasPo이 h咀）object at 0x7fb2b1J1511471J> F비se
         <tensorfiow.python,keras. layers.cony이utice키 .Gonna) object at 0x7fb2b미53b38> F비se
         <tensorflow.pythne.keras. layers.conyolut ion키 .Cony2D object at 0n7fb2b00dc2e8> False
         <tensorflow.python.keras, layers.conv이Ut ion비 . Gonna) obj act at 0x7fb2bCl0e8438> False
         <tensorf low .python,keras. layers.po이 ing.MaxPo이 ing2[) object at 0x7fb2b(Ilee358> F비on
         <tensorn ow. python.keras, layers,cony이Ut i neal .Conv2D 야>ject at 0x7fb2bOJee
                                                                                                        瓷乞는            ∼
         <tensorflow.pytl'y3n.keras. layers.conyolutic4lal .Conv2f) object at 0x7fb2b1]Uf
         <tensor flow, python次eras. iayers.cony이U씨neal ; Gonna) object at 0x7fb2bC1마
         <teosorflow.python,keras. layers.po이 leg. MaxPo이 ing2D object at 0n7tb2b미U                    하쵯世－흐鑿




C）
 임베디드 전문가 그룹 윌텍                                                                       - 229 -   무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 225 =====
4부. CNN                                                                                    4과. CNN 발전 시키기


  VGG-16 Fine Tuning (3/6)                                                                   임베디드 전문가 그룹 윌택

   穹Layer를 추가하여 모델 완성
     model._fine = tf.keras.models. Sequential.()
     model_fine.add(Input(shape=(IMG_SIZE, 1146_SIZE, 3)))
     model_fine.add(model)
     model_fine.add( FlattenQ)
     model_fine.add(Dense(1024, activation='relu'))
     model._fine.add(BatchNormal.izationO) (，
                                            執3\)
     model._fine.add(Dense(10, activation=' $oftmax'))

     Layer (type)                            Output Shape                             -      Param #

                                                                                      --
                                                                                      -
     vgglc (functiona.D                      ∼                       「

                                                                                      -
                                                         .,,   .3,       .I2)
     flatten (Flatten)                               ，   4608)

                                                                                      -
                                              （…
     dense (Dense)

     batch normalization
     伊atchUormalizetlorD
                                             (
                                              「
                                                     ,   1024)

                                                         1024)                        -
     dense_i (Dense)                          (      ,   10)                          -
    Total params: 1乞44h, " (74.19 l8)
    Trainable parㄼns: 卜I ,얌三 . . n8 (45.06 MB)
    Non-trainable params: r      징7 … (29.13 MB)




＠임베디드 전문가 그룹 윌텍                                    - 230 -                      무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 226 =====
4부. CNN                                                         4과. CNN 발전 시키기




   . CIFAR沁 Data 로딩
    from tensorflow.keras.datasets imoort cifarlO
    (traindata. train,Label引. (testdata. test labels) = citarlO - Load data( 》
    orint(train data , shaDe. train labels.shaDe)
    print(test_data,shape, test_labels .shape)
    train_data = train_data.astype(np. doubi이
    train_data = train_data / 255.0

    test_data = test_data.astype(np.double)
    test_data = test_data / 255.0
     (50000. 32, 32, 3) (50000, 1)
     (10000, 32. 32, 3) (10000. 1)

   . 모델의 입력 크기와 동일하게 조정
    train..,.data = , 寸．
                       image,resize(train_data (1MG_SIZE,,.갯양興）       )
    resr_叩t可．    = tT.lma,e.resize`test_aata, `IM(j_,iLt, IMfj_SILL))
    prlnhl,'rraln_uata.snape, test_uata . snapeJ
    1 (50000, 112, 112, 3) (10000, 112, 112, 3)




@）임베디드 전문가 그룹 윌텍                              - 231 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 227 =====
4부. CNN                                                                  4과. CNN 발전 시키기


  VGG-16 Fine Tuning (5/6)
   'a 모델 컴파일
     model_fine.compile(optimizer=' adam'.
                  功＄$= ' sparse_categorical_crossentr이玎'.
                  metrics= t accuracy "
   . 학습 （Training)
    history = model_fine.fit (train..,data, train_labels, shuffle=True,
                    batch_size=500, epochs=,20,         . , , .,
                    va.Lidation_data=(test_data, test_label키＇



                                                                      4卦늬r르드X=；乞營뽀I sal_loss: 0.9111
                      u7s 395ais/step - accuracy: 0.9912갼oss: 0.0257 됴」




 임베디드 전문가 그룹 윌텍
C）                                       - 232 -       무단 건재. 복제. 발췌, 디지털화금지


===== PAGE 228 =====
4부. CNN                                                                                                                4과. CNN 발전 시키기


  VGG-16 Fine Tuning (6/6)                                                                                                    CODEXPERT
                                                                                                                              임베디드 전문가 그룹 윌텍

   唾 학습 후 상황
    !                                                                     ^fLer Train,,,q


        rot_datalo](label [31? y 151) 古rot_detaIl)(label -161/ y [8)) Ln答datal2ll)abel [OIly (Ill 紂t,,4d，츠빴y,a器J낍뇨甲 oot_datal4I[label「 [61/ y「 [6))




                                                                          즈       切         巧    꾜讓   .   즈   凹   구드   1Do     c    즈     切    拓    1m
                       ,) [611y. 161) 計0_datat6l (label bu/ y
        tost_data[5] lab,                                        I) Jest_detelfl'label 161? y 161) teot_data[83 (label I3lly. I I) 樗：
                                                                                                                                    ‘七b,Ig) ([a브＝:．쌌쓰 (11)




              石     so   石    m0       .    2`   so    7S   ｝瑯       .    즈       m         75   표川   .   石   卯   '5   lm       .    石    덧》   75   l며｝




@）임베디드 전문가 그룹 윌텍                                                         - 233 .                 무단 전재, 복제, 발췌, 디지털화 금지


===== PAGE 229 =====
4부. CNN                                                    4과. CNN 발전 시키기


  GoogLeNet                                                     CODEXPERT




                                    炸
                                                                임베디드 전문가 그룹 윌텍

  1A ,, '`   I .,`＇→ m1` rIt. lkl
  1汀 Lc LdyeI> uINI'l

  孕효율극대화시킨 "Inception Module" 제시                      한안갛허 驢紛
  會 차별화된 성적으로 ㄸSVRC14 우승




                                       졈∥     鮮注n珊뇨



                                                                 Corn,이ution
                                                                 Poolrng
                                                                 Seftmax
                                                                 c이icat/Normm




@）임베디드 전문가 그룹 윌텍                    - 234 -       무단 전재, 복제, 발췌, 디지털화 금지


===== PAGE 230 =====
4부. CNN                                              4과. CNN 발전 시키기


  Inception module                                       CODEXPERT
                                                         임베디드 전문가 그룹 윌텍


  字 구글이 주장하는 DNN의 문제점
   . 망이 깊어질수록. Layer가 넓을 수록 성능이 향상됨
    4. 대신 연산량이 증가하고 Overfitting 가능성이 높음
    4. 이러한 문제를 해결하기 위해 전체적으로는 망 내 연결을 줄이면서（Spa rsity), 세부적인
       행렬 연산에서는 dense하게 처리하면 효과적일 것이라고 주장
  @Inception module
   G Cony layer들을 Sparse 하게 연결, 행렬 연산 자체는 Dense하게 처리하는 구조
   ● 여러 개의 Con미ayer를 한 층으로 구성하는 형태

                                        Feature를 효과적으로 추출하기 위해
                                        lxi .'3x3. 5x5의 cony와 3x3의 max
                                        的이ing 사용 ◆ 그리고 이 결과를
                                        Channel-wise-concat(Feature map
                                        을 쌓는 것）+ 결과적으로 Feature 추
                                        숱食읜과성은 최대한 Sparse 하게        「핼
                                        열 연산 자체는 Ql들읔 합쳐 최대한
                                        Dense 하게 처리함




@）임베디드 전문가 그룹 윌텍              - 235 -   무단 전재, 복제. 발췌, 디지털화 금지


===== PAGE 231 =====
4부, CNN                                                                 4과. CNN 발전 시키기


  Inception module의 문제점                                                      CODEXPERT
                                                                             임베디드 전문가 그醫 윌텍


  ri} 계산량이 너무 많음
                         28x28x(128+192+96+256) = 28x28x672
                                           Filter    그
                                       concatenation
                                   L


    28x28x결 2B           8x28x1                          8x28x96         28x28x256

    lxi convolutions     3x3 convolutions        5x5 convolutions   3x3 max pooling
          "l 28               }:j亡




                                       Previous layer
                       28x28x256


    konv 연산량＞
    lxi cony. 128 -+ 1x1x28x28x256x128
    3x3 cony, 192 4 3x3x28x28x256x192
    5x5 cony, 96 3 5x5x28x28x256x96
    Total .3 854M ops




@）임베디드 전문가 그룹 윌텍                             - 236 -     무단 전재, 복제. 발췌, 디지털화 금지


===== PAGE 232 =====
4부. CNN                                                                            4과. CNN 발전 시키기

       ,iI r, ,,,,oI 트ㅈl                                                             CODEXPERT
   ,       ，口%J itv-    I   -, 《＞                                                    ^,,,.,-, 一 ==? . 二．.，미
            -           ~    1 ∼一                                                    딛t,ff디，드 잔문가 그룹 월텍


   I lx1 Conv(Bottlenecl빼0는 차원 축소.)imension reduction) 기능
      I ㄷU ＇fiP
   a- FP射         rv. 우 委본．
           LU I V III 0 I1'r==      --I - I - I 사욘도I치
                               0= ` 도I거나        "Ibd네r
                                                         악누 거득이 초채하
                                                       I I2` .= )` ㄹ ` I =='1I ㅂ


   G Bottleneck을 통과하면서 채널이 줄었다가 다시 늘어남
   0 Bottleneck은 채널을 크게 줄이지 않는 한 성능에 거의 영향을 미치지 않음
   ● 차원 축소를 통해 P＃이 감소됨




＠임베디드 전문가 그룹 윌텍                                     - 237 -       무단 전재. 복제. 발췌, 디지털화금지


===== PAGE 233 =====
4부. CNN                                                                      4과. CNN 발전 시키기
                                                                                                    璜흖




  Inception module의 개선                                                             CODEXPERT
                                                                                   임베디드 전문가 그룹 윌텍


  孕 기존 Inception module에 lxi Cony를 적용
                                         Filter               28x28x(128+192+96+64) = 28x28x480
                                     concatenation


                                            \b∼，                                 :.;.;
    lxi convolutions     3x3 convolutions           5x5 convolutions     lxi convolutions
          匡28                 192                         蠟7                   S4

                       28x28x641                   28x28x64

                                                                         3x3 max pooling
                         lxi co駿lutions ;           lxi convolutions
                                                          64




                       28x28x256 l
                       28x28X256     Previous layer

    <cony 연산량>                                       3x3 cony, 192 4 3x3x28x28x64x192
    lxi cony, 64 4 1x1x28x28x256x64                  5x5 cony, 96 3 5x5x28x28x64x96
    lxi cony, 64 4 1x1x28x28x256x64                  lxi cony, 64 4 lxi x28x28x256x64
    lxi cony, 1284 1x1x28x28x256x128                 Total 4 358M ops     g' iAct1 』’，l'
                                                                                      .'亡




@）임베디드 전문가 그룹 윌텍                            - 238 -            무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 234 =====
4부. CNN                                    4과. CNN 발전 시키기

                                              COD入弘ERT
  GoogLeNet의 Inception module                 임버I디드 전문가 그룹 윌텍


  孕 모델의 핵심인 9개의 Inception Module 존재




@）임베디드 전문가 그룹 윌텍          -239 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 235 =====
4부. CNN                                           4과. CNN 발전 시키기




                  은 일뱐짚잎모조
  孕 초가앞도嶝起m끄으tw으rk）
  ；孕 마지막은 Classifier
   學 F(＝를 대부분 제거했고. 파라미터가 줄어도 모델이 잘 동작함을 확인
  Ii? 보조 분류기
           （Auxiliary classifier)
   穹 추가적인 Gradient를 얻어 중간 Layer의 학습을 도움
   密 학습 후 제거




＠임베디드 전문가 그룹 윌텍                 - 240 -   무단 전재, 복제. 발췌, 디지털화 금지


===== PAGE 236 =====
4부. CNN                                              4과. CNN 발건 시키기


  지속적인 개선 작업                                            CODEXPERT
                                                        임버｝디드 전문가 그룹 윌텍


  @ GoogLeNet은 Inception.vl
  @ Inception.v221- Inception.v3
   0 5x5를 3x3 + 3x3으로 변경 + 연산량 28% 감소
   .nxn을 lxn + nxl로 변경 + 연산량 33% 감소
   . 보조 분류기1 제거
     1추 실험을 통해 성능에 영향을 주지 못하는 것으로 확인됨
   00ptimizer를 RMSProp로 변경
                                                    〃 d섶 乞뷘m’ㅈ｛ 창"이
   G Label sm石6函h5짜용4 Label을0. 1이 아L 라 0.1. 0.9와 같이 변형하여 사용
   G Fact。
         rized云74可
                 I- OF cl_FC。
                            ny 7x7흘C。
                                    ny 3x3 27ㅐ로 변경
   ●BN-auxiliary + 마지막 FC에 Batch normalization(BN）
                                                 을 적용
   彎Inception.v4
   臼Inception.v3를 변형하여 실험하여 얻은 좋은 결과를 적용




@）임베디드 전문가 그룹 윌텍                   - 241 -   무단 전재, 복제. 발췌, 디지털화 금지


===== PAGE 237 =====
4부. CNN                                                                                4과. CNN 발전 시키기


  망을깊게하면무조건성능이좋아질까？                                                                         叩DE PERT
  「걍 Cony 治yer들과 FC 怡yer들로 구성된 네트워크의 성능 테스트




     業나니ㅇ口 쓺 드 듬 b
                                                        小卞낙Hㅇ 놉U茁H
                                                                                            쯔aver
                                                                      ,：》∼－
                                                                                  L∼,,,→，
                                                                                        ,20-Iaver




                        iter. Oe4)                                            iter. ne4)
    [Source: Kaiming He, Xiangyu Zhang, Shaoqing Ren, Jian Sun. Deep Residual Learning for Image Recognition.]


   ● 더 깊은 구조인 56층 네트워크가 20층 네트워크 보다 성능이 나쁨
   . 망이 깊어질 수록 Gradient vanishin9L즈쁘브j끄으星젠生샐
                                           ［→
   0 망을 깊게 만들었을 때 효과를 볼 수 있는 방법은 없는가？




 임베디드 전문가 그룹 윌텍
C）                                                 - 242 -           무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 238 =====
4부. CNN                                                  4과. CNN 발전 시키기




   0 입력 값을 출력 값에 더해줄 수 있는 shortcut
                                （지름길）
                                    을 추가
    4. 勍ortcut은 보통 2∼3개 layer를 건너뜀
     4- x 입력 시 H(x) = F(x) + x 가 출력됨
    4- F(x) + x가 학습 대상 + x는 변합 수 없는 값이므로 겸국 Fix）   가 학습
    〃 F(x) = H(x) - x 이고 K(x) -x를 잔차
                                   （Residual）
                                            라고 함 *겯굴조브
     구m 이렇게 하면 Layer가 많아져도 최적화가 쉬워지고 정확도가 향상됨




@）딛Jl게디드 전문가 그룹 윌텍                     - 243 -   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 239 =====
聊쿠 , CNN                                                         4과. CNN 발전 시키기


  ResNet의 구조                                                        －…'－→贓《 훨쬐 毓－ , "
                                                                    임베디드 전문가 그룹 윌텍


  （걍ResNet은 VGG-19 구조를 뼈대로 합
   .VGG-19에 (onv layer들을 추가하고 다iortcut들을 연결한 것이 전부임
           VGG-19   34-layer plain   34-layer residual                    下
            m1離




                                                                              〔）綸
                                                                    伊솟穩 宖L0k V
                                                                                             l
                                                                         r   ｀스   小｀측；
                                                                                     거ㅟ갸




                                                                             J
                                                                     오？孔쟈唾W꺄
                                                                     旦乞｀l9c             '/       .




＠임베디드 전문가 그룹 윌텍                        - 244 .           무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 240 =====
4부. CNN                                                                  4과. CNN 발전 시키기


  ResNet의 성능                                                                  g；매디드 즈蝦’가 그竇 윅텍


  每 미air, 네트워크와 ResNet을 비교
                        굵은 선：validation error              굵은 선：validation error
                        가는 선：training error                가는 선：training error


    m
    口
    ， ㄴ요b




            1L1    2S        35   40   多0
                        目貫 nt4》                             it' n텨）

                  <Plain 네트워크＞                             <ResNet>


   G Plain 네트워크는 망이 깊어지면 오히려 error가 커짐
   .ResNet은 망이 깊어질 수록 error가 작아짐




C）
 임베디드 전문가 그룹 윌텍                                 - 245 -   무단 전재, 복제. 발췌. 디지털화금지


===== PAGE 241 =====
4부. CNN                                                   4과. CNN 발전 시키기




                   method                              topd err.   top-5e[T;
                   VGG 14이 (ILSVRC' 14)                   -          8.431
                   GoogLeNel [43](ILSVRC' 14)             m         7.89
                   VGG [4이 (v5)                          24.4       7.1
                   PReLLJ-net [l21                      21.59       5.71
                   BN-ince伊沁n  〔堈                       2l.99       5.8i
                   ResNet-34 B                          21.돈卜4      5.7}
                   ResNct-34 C                          21.53       5.60
                   ResNet-50                            20.74       5.25
                   kesNet-101
                   ResNet-l52                   /19.       87         蠶＼
                                                                      ，
@）임베디드 전문가 그룹 윌텍      - 246 -     무단 전재, 복제, 발췌. 디지털화 금지


===== PAGE 242 =====
4부. CNN                                                                                      4과. CNN 발전 시키기


  DenseNet (112)                                                                                    임베디드 전문가 그룹 웝텍


  @ Dense 비ock
   G Feed-forward 방식으로 각 Layer률 다른 모든 LayerOll
          Cony l rn * d 檄纛tnd
            6                                      <5 Layer Dense block with a growth rate of k = 4>
                 Ccciv 2 'nPUt〔hag청n이
                     5 추 4 玄 10

                                  oqw 3 input chanci礖
                                   6+4＋」=14


                                               c＜月1V 4 !nput chann倂
                                                6 +4 뿌4 ' 4 =18

                                                         Ttans而an Layrr input dian
                                                           6+4수4*4수4鷺22

                                                                               [Source: Densely Connected Convolutional
                                                                               Networks(2018). Gao Huang, Zhuang Liu,
                                                                               Laurens van der Maaten]



                                                                                     Den$e 테ock 3




                           「仇tH叱누                       比n缶하끼 〃l耳




＠임베디드 전문가 그룹 윌텍                                          - 247 -         무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 243 =====
4부. CNN                                                                4과. CNN 발전 시키기


                                                                            COO
  DenseNeti 21                                                              임볘디드 전운가 그룹 윌텍


  @ tf.keras.applications.densenet.DenseNetl 21
    tf.keras.applications.densenet.DenseNet121(include_top.True. weights='imagenet'.
           input_tensor=None, input_shape=None, pooling=None, classes=1000)
   密Arguments
       Name                                         Description
   include_top    R川y-connected layer(dense layer) 포함 여부 (True면 포함. False면 제외）
                  None: random initialization
   weights
                  'imagenet': pre-training on imageNet
   input_tensor   옵 크. 이미지 입력. Keras tensor（예를 들어 output of tf.keras.layers.lnput)
                  옵션. shape Tu이e, include_top=False인 경우만 지정 가능
   input_shape
                  높이와 너비가 32보다 작지 않아야 함




@）임베디드 전문가 그룹 윌텍                             - 248 -     무단 전재, 복제, 발췌. 디지털화 금지


===== PAGE 244 =====
4부. CNN                                                                                                                              4과. CNN 발전 시키기

                                                                                                                                          CODEXPERT
  Digit Sign에 DenseNet 적용 예제
                           （D                                                                                                             임베디뜨 전문가 그｛< 昱l E


  e［예제 10] pre-trained model인 DenseNet 을 적용한 예제
  model = tf . keras . models . Seauential()
  moclel.aacfltr.Keras.appiications Jlensenet . uensemetiLi (
      weights="imagenet".
           批lude_top=Fa1se,                                         #, dense,layer 01 뉵，
                                                                                       켄완m,,.                                                                    ..
           lnput_ tensor tT. Keras iayers . 1nput snape    .                                       '      =`IM
                                                                                                                 "_ siLt,            IMb_ 1Lt '                 i) )


  # Dense          layers
  model.                                                            Flatten                            flatten
                                                                                               24, activation ))relu;
                                                                                      (name=
                                                 layers.
                                             .
                                   keras
             add            (tf.
  model.                                                                                                                                                          1024
                                                                                                                                                                              ))
                                                                                                                                           'dense_
                                   keras                            Dense
                            (tf.
             add                                                               (i@
                                                 layers.
                                             .                                                                              ,name;
  m。                                                                                  rmalizati。
                                                                                                                                                                               )
             add
    del.                    (tf.             .
                                   keras          layers   .         BatchN。                                                                                             '
  m。del.     add            (tf.    keras.        layers   .Dense              (10,              nO) ' s。
                                                                                         activati。n=               ftmax    ',         name          'denselO            ')
  model. summary(》




＠임베디드 전문가 그룹 윌텍                                                                                - 249 -    무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 245 =====
4부. CNN                                                                                                                       4과. CNN 발전 시키기


  Digit Sign에 DenseNet 적용 예제
                           （2)                                                                                                      CODEXPERT
                                                                                                                                    임베디드 전문가 그룹 윌텍


  每［예제 10] pre-trained model인 DenseNet 을 적용한 예제
   臼Model summary 결과
                                                                                                                                                    -
                                                                                                                               ---－……，




          Layer (type)                                                                           Output Shape                            Parazn *

     -    densenetl2l                                            「tionai)                        (1   J 』，' 시 1.0)J)

     -
                                                          (Fun
          flatten                                                                                (
     -
                       (Flatten)
                                                                                                      j   …朴）



          dense 1024                           (Dense)                                           (    J 注汁立）

     I-   batch_
            (Batc
                     normalization
                    hNormailzatlon)
                                                                                                 (    J 1024)


          activation                                                  n)

                                                                                                                                                    -
     !
                                             (Activati。
                                                                                                 (    J 1024)

     - den5e 10                                                                                  (    ' 10)                               10, 250

                                                                                                                                                    !
                                   (Dense)
     -    otal params: 11,741,178                                           (42.   90 MB)   .




                              껀！,4111 (.421511 M빈．
     - lral!1ar)le Pa.rㄼ긺｀: i1，                                                                                                                     l
     -,Non-tralnaoLe par켁뺨＝J夕．꺅〕 (.334.,쑈즈믿∥ , .. :,∼…, ∼                                                         ,m ,…   …                ,니       I




⑥임베디드 전문가 그룹 윌텍                                                                                 - 250 -         무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 246 =====
4부. CNN                                                                                                                                                                          4과. CNN 발전 시키기
                                                                                                           蠟＝∼乙令啼츤留搏輾鱗찻好' -;                                      …＝蠟면mm… 료졈蠟……                           ……하ㅋ斗…              …－




  Digit Sign에ReLU, Dropout적용결과                                                                                                                                                                      EXP,E
                                                                                                                                                                                               엑딘),EE1-7 .a싸
   .결과분석                                                                                                                                                                                                                  ,
                                                        4   ___=           1_ I= .S! __            l_ _ '_ _    ' -                 1=                4 ^^,             `   ``              A '~SJ                        l
                                                        ~ WIIVUIUUQFI ia yei WPOCF1S= I UU) '                                                                               /I.
  Epoch 98/100
                   ∼，                                                                                                                                                                '07o                            'j
  52/52                                                     0s lrnslstep - vat_accuracy: 0 .3770 - val_loss: l. 0982
  Epoch 99/100
  52/52                                                     is 7m5/steD - val accuracy: 0.7674 - vat loss: 1.1296
  卄:pOCfl iuai八｝
               U                                                                                                 I
  巨Z｛丑                                                      is irnsJstep - vat accura드y三_吸꾜46-- vat∼loss: 그．
                                                                                                           .j憂2궂－l
                                                        , =-       ,                      ,   n_    I ll    ,   K                                 .                              4   .ts .       `
                                                                                                                                                                                                     沙'f''0 70
                                                                                                                                                                                                     na   Ann,
                        . ` UIIVUIULIUII IdyeI ㅜ fWLU ㅜ uiupuut ` epucrIs = I VU) '
                   -;     --   -   .   .   -.   .   .          -       -   .   .   一                                  _   _   ...   _    一.   .       -   -   -   -L-




   Epoch 98/100
   52/52                                                    0s 4.ns/step - val_accuracy: L9472 - vat그oss: 0.1959
   Epoch 99/100
  j2/52누                                                    - 楓4兆5乙＆姐狐二．
                                                                       보且又굽J(；拓』
                                                                               1a以jm乳949,-＝斗yal-l. 5읖뇨Q=,z15l,
  ]Epoch 100/100                                                                                             l
  益z즈5z                                                     拓． 4飇／5沈9-=-yal-aqa』
                                                                               CaCx：一，
                                                                                     公，요41松딨, v孔LI0S5．
                                                                                                     치，
                                                                                                      翩721닯
                   /                                                                                                                                                                                                      ,
                         n∼∼m kI. .4 *I- Q                                     1       fl ..s. _L &ㄴ一－..I: ..._...: .._ I_ _ - mL一 -                                             _t.%, _S ^^              .fl. flf

   Epo야I 18/2a
   Epoch 18/20           L,t=!I＞心I`eL                                      ㅜ 떼U..!I I'IJUIIdtILdLIUII `e )QI. JJ>                                                                LUJ '               =＇》.IQ70
   52/52                                                    5s 5&ns/step - vat_accuracy: 0.9233 - vaT-loss: 0.1947
   Epoch 19/20
   52/52                                                    3s Sims/step - vat_accuracy: 軌9784 - vat_loss: 0.0643
   Epo比 20/20
   52/52                                                    6s 64ms/step - vat_accuracy: 0.9976 - vat_toss: 毓0097




＠임베디드 전문가 그룹 윌텍                                                                               - 251 -                         무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 247 =====
4부. CNN                              4과. CNN 발전 시키기
                                        -=-     i塔걋』
                                                   轉智젯膏：




  MEMO                                  CODEXPERT
                                        임베디드 전문가 그룹 윌텍




@）임베디드 전문가 그룹 윌텍   - 252 -   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 248 =====
5부. RNN(Recurrent Neural Network)


===== PAGE 249 =====
5부. RNN                                      1 4. Time Series Forecasting




          li!F. Time Series Forecasting
          2羈. RNN M01.；每




@）임베디드 전문가 그룹 윌텍                - 255 -   무단 전재, 복제. 발췌, 디지털화 금지


===== PAGE 250 =====
5부. RNN                                                1과. Time Series Forecasting


  시계열 데이터
        （Time Series Data)                                        CODEXPERT
                                                                  임베디드 전문가 그룹 윌텍


   . 일정 시간 간격으로 배치된 같은 형태의 데이터들의 열
                                 （sequen떠
                                                                   米 C耐毛
   穹 시계열 해석
          （time series analysis)
                                                                    삽꺼끽蝦2包
    r乍 시계열 데이터들이 어떤 법칙에서 생성되어 나오는지 파악하는 수학 분야
   .Task
    f1 Forecasting
       x Series data를 통한 다음 발생 할 것에 대한 예측
       x ㄷ陪탈매출〃내일주식종가 ℃秀쟁촉汽，
                           )
    '4 Classification:
       x Series data에《:ategorical label을 구분
       x 사이트 방문자의 동작을 통한 bot 여부 판단
    '4 Event detection:
       'C 특정 Series data를 찾기
       'C ' 아
            （ Goo이 e"
    i4- Anomaly detection:
      ｀스맨쁘奭ta（연속적인 data stream)르보目와상유무판닫
      ' 생산공정관리                   Al,q드이 .直〔ㅔ스．
                                             ,           >1쵯




@）임베디드 전문가 그룹 윌텍                          - 256 -   무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 251 =====
5부. RNN                                                                                   1 F. Time Series Forecasting


  Weather archive Jena                                                                                                    CODEXPERT
                                                                                                                          임볘디드 전문가 그룹 윌텍



  @ Weather time series柚笏궉
   . Max Plan댄上rs쁘쁘ejtor Biogeqchemistry Uena, 녹일 )
    4. https://www.bgc-jena.mpg.de/wetter/
   0 14가지의날씨정보를.卄10분마다측정                                                               了八｀-.           j功m
   · 2003ii .E1善苕 A回 ∼나－
    〃수업에' I廷걘雨口琵如
                " ' 曙：Francois
                          （「이―e나"ㅐ구성
              jena_climat&2009-2016,csv                                                                         」눔
                                                                                                                              )

              Detad    c01l半1ct     C아umn                                                                   m 사15 . !Jmn` v


             O DSTh*           =    軫 Ptm出）           7    #nde901     1r    鶯！加nK}      多．   * ㅜd口나t0.40            F   *15141       l

            ..                                ㅅ 三 1                                               ▲
                                                                                                                                      i


             200*- 》1-01 2m7 》141   "14             `《）
                                                      외1   7〕          az3   2룐｝

             仔1 e1 2麗9 88 1e .e     99t, !z                m8 日2                               8 徒

             e! e 1 z에9 ．蝕2m ee     口아』 걀 /                .且41              los-el            4 28

             驪！ e} 2e的 ea 3m胛       Hb 5J                  B 5`              214.11            a :!

             eㅌ e1 2e.9 e* 4· 9.    rn恪 三                   근 1'             z65 12            1건3 댓

             단i .1 2弓·9 ea 羽 ·．     q午，V                   日 ??                                〕g4                       노4       B


                                              source:https://ww.kagqIe.com/datasets/pankrzysju/weather-archjve-jena




@）임베디드 전문가 그룹 윌텍                                                   - 257 -            무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 252 =====
5부. RNN                                                     1과. Time Series Forecasting


                                                                           임베디드 전문가 그룹 윌텍


  @ Download
   簿 From amazon
    4. ' ttps:J/s3 .a rnazonaws.com/keras-datasets/jena chmate 2009 2016.csv.zip
   .From kaggle
    4.


  @ Raw data
   . 측정 data: 14개 항목
    4. 'p (mbar)', 'T (degC)', 'Tpot (K)', 'Tdew (degC)', 'rh (%)', 'VPmax (mbar)', 'VPact
       (mbar)', 'VPdef (mbar)', 'sh (g/kg)', 'I-I20C (mmol/mol)', 'rho (g/m**3)', 'wv
       (mis)', ' max. wv (mis)', 'wd (deg)'
   .Shape: (420451, 14)




＠임베디드 전문가 그룹 윌텍                          - 258 -     무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 253 =====
5부. RNN                                                 1과. Time Series Forecasting


  시계열 데이터 기반 온도 예측
                 （1/7)                                            CODEXPERT
                                                                   임베디드 전문가 그룹 윌텍


  三：［예제 1] MLP 예측 모델로 Jena data의 처리방법과 결과 분석
  孕
   . Raw dataset
     /1' Validation & Test dataset 분aI
       x 최근의 온도 변화가 앞으로의 온도 변화에 영향이 큼
       x 실제 test와 학습 시 검중을 분리하여 진행
       x Train: 50%. Validation: 25%. Test: 25%
     4. Normalization
        x 14개 data가 서로 다른 scale -> 비슷한 scale로
       x Train dataset을 기준으로 norm키ization


          # Normalization
          mean = raw_data[:num_train_sample회.mean(axis=@)
          raw data -= mean
          std = raw_data[ :num_train_sample회. std(axis=O)
          raw data 1= std

                                                  珊 ,：卄,. 加，
                                                           4 餉］
                                                              『.
                                                              ‘




@）임베디드 전문가 그룹 윌텍                           - 259 -   무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 254 =====
5부. RNN                                                   l과. Time Series Forecasting


  시계열 데이터 기반 온도 예측 (2/7)                                               CODEXPERT
                                                                   M   임베디드 전문가 그룹 욀텍


   . Sequence dataset 생성
    / Parameters:
       x sampling_rate: 10 mmn * 6 -* 1 시간 단위의 온도 변화 측정
       x sequence_length: 120 <- 24*5 (- 5 일간의 온도 변화를 학습                        ,,
       x delay: sampling_rate * (sequence_length + 24- 1) e 'sequence의그다읕날같은시각의온도
       x Batch size: 256
                                                                   j&，신a1?z. )\21'叫
    tZ- Define function
       def create_dataset(data, targets, start_index, end_index, sequence_length,
                          sampling_rate):
           x, y = [3, [1
           start = start index
           if end index is None:        # for test data
               end_index = 1en(data) - delay
           for i in range(start, end_index, sampling_rate ):
               Xappend(data[i: i+seQuence lenqth*samplinq rate: samplinq ratel)
               y.append(targets[i + delay])
           return np.array(X), np.array(y)




@）임베디드 전문가 그룹 윌텍                       - 260 .    무단 전재, 복제. 발췌, 디지털화 금지


===== PAGE 255 =====
5부. RNN                                                      1과. Time Series Forecasting


  시계열 데이터 기반 온도 예측
                 （3/7)                                                    CODEJU'ERT
                                                                          임볘디드 전문가 그醫 윌텍

   臼 수치적 접근
    ／乍 현재 온도가 내일 같은 시간에 거의 같을 것이라고 예측 가능
    ,4 MAE(Mean Average Error）를 계산해 보면
       x Validation MAE: 2.44
       x Test MAE: 2.62

             del evaluate，∼naive-method(x, y):
                 total abs err = 0.
                 for samples, targets in zip(x, y):
                     preds = samples[-1, 13 * std[1] + mean[1J
                     tota1.-abs-err += np.sum(np.abs(preds - targets))
                 return totalabs_err / len(x)

             print(f"Validation MAE: {evaluate_naive_method(X_ val.. y_val.): . 2f}")
             print(f"Test MAE: {evaluate_naive_method(X_test, y_test): .2f}")

      Yalidat츠on,M스트
                  （근스
      1, .
             1e5I. n·AL : z e.z




@）임베디드 전문가 그룹 윌텍                            - 261 -    무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 256 =====
5부. RNN                                                14. Time Series Forecasting

                                                                    COD
  시계열 데이터 기반 온도 예측
                 （417)                                              잉뻬터드 찬딛가 ．그릅 월텍


   密MLP model

     l inouts = keras.Inout(shaoe=(seouence lenath. raw data.shaoel-1n》
     ; x = tayersJiar tenU(1flPUtS)
       x = 1.ayers.Dense(16, activation='relu")(x)
       outputs = layers.Dense(1)(x)
       model = keras.Model.(inputs, outputs)
       model_name = models_path + ' 1-jena_dense' + fx

      caithacks = [keras. caflbacks.ModelCheckpoint(model_name,
                                         save_best_only=True)]

      model.compile(optimizer=' rmsprop' ' loss= 'mse' 』metrics=
                                                               〔' mae' ])
      history = model.fit (X_train, y_train,
                          epochs=10,
                          validation_data=(X_val, y_val),
                          caflbacks=cal.lbacks)




@）임베디드 전문가 그룹 윌텍                      - 262 -   무단 전재. 복제. 발췌, 디지털화금지


===== PAGE 257 =====
5부. RNN                                                          1과. Time Series Forecasting

                                                                                 CODEAPERT
  시계열 데이터 기반 온도 예측
                 （517)                                                           임베디드 전문가 그룹 윌텍


   .Training result: MLP
    ' 1- 시계열 데이터를 MLP mod이로 예측하는 것은 무리

              Traning and validation Loss                    Trami四 and v비idation MAE
                             -        aInirs L-oss
                             *       Valkialon Loss




                                                      z6




                                                      24




                                                      2,2


                 `       1       ￡           1

                 2       4       6           B




＠임베디드 전문가 그룹 윌텍                                  - 263 -    무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 258 =====
5부. RNN                                             1과. Time Series Forecasting


  시계열 데이터 기반 온도 예측
                 （6/7)                                          cODE X PERT
                                                                밈베디드 전닌기 그룹 윌텍


  回［예제 2] 1DCNN 예측 모델 결과 분석

      inputs = keras.Input(shape=(sequence_lenqth, raw_data. shape〔-1]))
      x = layers.ConvlD(8, 24, activation="relu")(inputs)
      x = layers.MaxPoolinglD(2)(x)
      x = layers.ConvlD(8, 12, activation="relu")(x)
      x = layers.MaxPoolinglD(2)(x)
      x = layers.ConvlD(8, 6, activation="relu")(x)
      x = layers.Global.AveragePoolinglDQ(x)
      outputs = layers.Dense(1)(x)
      model = keras.Model(inputs, outputs)

      modeLcompiLe(optimizer=' rmsprop', loss='mse, metrics=[ 'mae'J)
      history = model.fit (X_train, y_train,
                          epod,s=10,
                          val.idation_data=(X_val, y_val.),
                          caUbacks=caUbacks)




＠임베디드 전문가 그룹 윌텍                    - 264 -   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 259 =====
5부. RNN                                                             1과. Time Series Forecasting


  시계열 데이터 기반 온도 예측
                 （7/7)                                                             CODEXPERT
                                                                                   임베디드 전문가 그룹 윌텍

   ' MLP vs CNN 결과 비교：MAE

                                     Naive                 MLP         CNN(1D)
              Validation             2.44                  2.61           2.88
                 Test                2.62                  2.70           3.07

                Wa}nInq and vabdation MAE                     Tra        lidation MAE
                              －一一 Yaiflin9 MAE                           -m 珊恥fling MAE
                              -m Vahd.hon MAE                            mm- V出1datI.n 姚A￡




          0       2




@）임베디드 전문가 그룹 윌텍                                 - 265 -    무단 전재, 복제, 발췌. 디지털화 금지


===== PAGE 260 =====
5부. RNN                                22F. RNN Models




@）임베디드 전문가 그룹 윌텍   - 266 .   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 261 =====
5부. RNN                                                                    2과. RNN Models

                                                                           CODEAPERT
  RNN(Recurrent Neural Network)                                            임베디드 전문가 그룹 윌텍

  孕 시계열 데이터의 복잡한 패턴을 해석하는데 RNN 구조 사용
   . 순환
      （Recurrent) 구조를 갖는 RNN의 동작
    ,2 1. 입력 데이터
               （xt）
                  는 시간 축에서 순차적으로 공급됨
    ／乍 2. 입력 데이터
               （xt）
                  와 이전에 기억된 정보를 사용하여 새로운 정보를 생성
     23. 새로 생성된 정보는 기억되고，
                        이것의 전체 또는 일부
                                   （h ）
                                      가 출력됨




               [ Source:〔이ah.github.io/posts/2015-08-Understanding-LSTM키




@）임베디드 전문가 그룹 윌텍                      - 267 -      무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 262 =====
5부. RNN                                                                                  221. RNN Models


  RNN의 다양한 형태：one to many                                                                CODEXPER「'

                                         …小ㅂ
                                           n
                                           …
                                                                                         임볘디드 전문가 그룹 윌텍




                           -U
                            스如
                  Mm니무戶…
    r   一一




        巴
        j念흉
          i一n
            vm니
                                                      *                   *




                                  U
                                  fnm
                                    一m     ▲
                                           r一∼
                                             비Yn
                                               山
                                                   [}
                                     r
                                     4
                                     i
                                     놔
                                                   LI L
                                     遼
                                     珏
                                     多
                                     巍
   [Source: CS231n Convolutional Neural Networks for Visual Recognition: tecturelO]


   . 활용사례1: 이미지 캡션 + 이미지로부터 문장을 생성
                                                          -
                                                                    A dog is running in the grass.

                                 ［이미지］                                            ［문장］

   ● 활용사례2: 노래 작곡 + 기본 멜로디로부터 노래를 작곡
                               事'"( . .-. fl.舜耳…:t1軫- --1-.= .="
                     4릎＝쿄 -*
     學학亨J -1딨 . j주士 l』         얇흰二， c J=-＝깝工쥬二1;f; '
                               癸＝=n .찧 客，     ,iJ7J그卄l兄견．      二
                                                                                  ［노래］




＠임베디드 전문가 그룹 윌텍                                       - 268 -      무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 263 =====
5부 . RNN                                                                                     22F. RNN Models
                                                                                             無걋「朴芝쭈媤擘꾼礬習象缸


  RNN의 다양한 형태：many to one                                                                    CODExPERT
                                                                                             임베디드 전문가 그룹 윌텍




                                                                        nnlㄴ 스
                                                                        …
                       rn緻ny t。
                              。ne                                      many to many

                                                                                 U,



       Ii             ［끄川            -I
    F Source: CS231n Convolutional Neural Networks for Visual Recognition: tecturelO I


    0 활용사례L 노래를 장르로 구분하기

           샅U j4jjjJJ'.J4 dUU사U]                               →                      디스코

                                                                                      ［장르］



    . 활용사례2: 영화 후기에 대한 감성 분석
                    남녀노소 다 눈묻 콧물 뼙니다
                    사람이연 다 보다 울어요
                                                                                      긍정

                          ［영화 후기］                                                     ［분석］




@）임베디드 전문가 그룹 윌텍                                       - 269 -        무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 264 =====
5부. RNN                                24. RNN Models




@）임베디드 전문가 그룹 윌텍   - 270 -   무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 265 =====
5부. RNN                                                                         22F. RNN Models




                    1件 챠斗 강川료괘 ㅉ＾4도1t ri삼 철40惻또）
          ·m的 =,균74*m.`＾최a.'.       주斗emi＝甘쿄5ㅎ ｀（므412`4i，緇




                   拓 －可－玉卄큐        ·   B   T    m    '   麗
                  nm1J141                      ,m口1·




@）딛간케디드 전문가 그룹 윌텍                                            - 271 -   무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 266 =====
5부. RNN                                                                           24. RNN Models


  Basic RNN의 구조                                                                    임베디드 전문가 그푭 윌텍




                                                                        h= tanh(Whhht-l + WxhXt + bh)
                                                                        h: 현재 hidden state 값
                                                                        ht.1 : 이전 hidden state 값
                                                                        xt : Ndden layer으』입력
                                                                        Whh. WXh : weight
    [Source: colah.github.io/posts/2015-08-Understanding-LSTMs I




＠임베디드 전문가 그룹 윌텍                                    - 272 -         무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 267 =====
5부. RNN                                                                                 2과. RNN Models

                                                                                                  ERT
  Basic RNN의 output 처리                                                                   임베미드 전문가 그醫 윌텍


                                                                         切
                             Yt
                                                                                   Yt: output
      「！      .
                             f,
                                   Why                                             Why: weight
                  Whh
      htij-
                                               Yt = Whht + %
                        L1         W,
                                                   h = tanh(1V,thht i + Whxt + 岫

      이,e 幻n恪fly                  m翩，
                                    y k) one       many to many     many to many
                                                                                   I
                                                                                   r．
                                                                                    뼈ㅊI2I7I갸甘／
                                                                                             「


                                         U
                                         수nㅂ
                                   싸
                                   니ul
                                                        스：－냥--.4탤    士스뻐소－』
                                               JTh{H"} U-!II{]
                                               수    수   수            亨   수   *

                                   f           口 ［〕      El




c）
 임베디드 전문가 그룹 윌텍                                         - 273 -     무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 268 =====
5부. RNN                                                                  2과. RNN Models




  @ Basic RNN이 activation function으로 tanh를 쓰는 이유
    * Vanishing gradient problem 방지에 tanh가 유리하기 때문
    ／小 아래 그링을 통해 sigmoid 보다 tanh21 미분 최대값이 상대적으로 큼을 알 수 있음




      [Source: https://towardsdatascience.com/why-data-should-be
       normalized-before-training-a-neural-network-c626b7f66c7d ]




＠임베디드 전문가 그룹 윌텍                                 - 274 -        무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 269 =====
5부. RNN                                                                          2과. RNN Models


  Basic RNN의 문제점                                                                  CODEXPERT
                                                                                  임볘디드 전문가 그룹 윌텍


  冬 장거리 의존성
          （Long-range dependency) 문제
   ."the clouds are in 柚e sky"에서 마지막 단어를 sky로 예측하는 것은 어렵지 않음
    /' 그러나 "I grew up in France ... I speak fluent French' 에서 마지막 단어 Frenc土 예측은7
     tl- FrencF，
               가 관련 정보인 France와 거리가 멀어 예측이 쉽지 않음 * 장거리 의존성 문제




   臼Basic RNN은 backpropagation 시 vanishing gradient 문제 발생
     4. 따라서 긴 시퀀스를 처리할 수 없고. 장거리 의존성 운제가 발생함 + tanh로는 해결 불가
               (8          (ii:}             也
                t           t                t                backpropagation
           A

                                   @[S。
                                          urce: http://c。
                                                       lah.
                                                                        sts/2。
                                                                      /p。
                                                              github.i。      15-。8-Understanding-LSTMs




@）임베디드 전문가 그룹 윌텍                          - 275 .      무단 전재, 복제, 발췌, 디지털화 금지


===== PAGE 270 =====
5부. RNN                                        2 F. RNN Models


  LSTM(Long short-term memory) J등장              CODEAPERT
                                                4 I:I
  @ LSTM은 Basic RNN에서 hidden state를 수정. C에 state를 추가한 구조
          孕         四l          區）




@）임베디드 전문가 그룹 윌텍           - 276 -   무단 전재, 복제. 발췌, 디지털화 금지


===== PAGE 271 =====
5부. RNN                                                                                          24. RNN Models
                                                                                                                         ∼之多




                                                                                                  CODE ' PERT
  LSTM의 구조
         （1)                                                                                      임베디드 전문가 그룹 뢸텍




      Neural Network
          Layer
                       Pointwite
                       Operati。n
                                    Vector
                                   Transfer
                                                           口py                               Output
                                                                                             (Hidden state)
                                                          βqe/
                                                         亡，

                                   F          et gate lnput gate
      Previous
      cell state               +                                                              Cell state

                                                                                        t gate

      Previous
                                                                                              Hidden state
      hidden state



                                                  nput
                                                    [Source: http://colah.githubio/posts/2015-08-Understanding-LSTMs I




 임베디드 전문가 그룹 윌텍
C）                                                        - 277 -       무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 272 =====
5부. RNN                                24. RNN Models




＠임베디드 전문가 그룹 윌텍   - 278 -   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 273 =====
5부. RNN                                                    2과. RNN Models


         （3)
  LSTM의 구조                                                     CODEXPERT
                                                               임베디드 전문가 그룹 윌텍


   . L갸)date C애 state + 기억할 정보를 수정

                            c




                                   (7f = /t * ct-I + 秀t * Ct




   .Update hidden state + 출력할 정보를 선택

                        t          ot = α（仍낚ha + w。
                                                  xt + b。
                                                        )
                                   ＇乙t = ot * tanhi(Ci)




@）임베디드 전문가 그룹 윌텍                - 279 -   무단 전재, 복제, 발췌, 디지털화 금지


===== PAGE 274 =====
5부. RNN                                                                                          2과. RNN Models
  赫磁횬                                                                                            孕器坪聲擘斗茗掛多
  GRU                                                                                            CODEKPERT
                                                                                                 임베다느 전문가 그룹 윌텍

  孕GRU는 LSTM의 장점을 유지하면서도 계산 복잡성을 낮춤



                                                  Zt = t7(Wh_i + W- x)

                                              '1, == 'TrIV.h. 4 + H/ P, ,
                                              ' I,    -.                                                        ) 昏rj
                                             瓦=       tanh     (   W             (rt*   h   '   ) ' wxV. /,’.
                                         ／乙＋ == " - zn * Ii.' 1『
                                                              므+ z4 '* 시；”「놓_ 〃 ' c\
                                                                                                                  '~L
                                        （돈二으7슨쓰：                       h4 1(jt；



                                                                       l）   汰｀
          I Source: Cho, Kyunghyun, et al. 'Learning phrase representations using RNN encoder-decoder
                             for statistical machine translation," arXi'vpreprint arXiv:1406. 7078(2014) 1




C）
 임베디드 전문가 그룹 윌텍                         - 280 -              무단 전재, 복제, 발췌. 디지털화 금지


===== PAGE 275 =====
5부. RNN                                                    2과. RNN Models


  RNN의parameter수계산                                       《「 ,jt1II'IE, a，
                                                                        텍
  @ Basic RNN c에
   （兀卄 H + 1) * /f＇三
                                  H.: hi.7jijstate의 길이
  @ LSTM C애
    ((Xe, + Hn + 1) * ／了＇l> * 4
  . GRU C에
    （兀1 + Hn + 2) * 珏瑋 * 3
    (




     di 찝asicRNNcell




＠임베디드 전문가 그룹 윌텍                   - 281 .   무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 276 =====
5부. RNN                                                       2과. RNN Models


                 （1/9)
  RNN：시계열데이터기반온도예측                                            CODEAPER,,
  Q［예제 키 기본 모델：카JN layer를 이용한 모델

    inputs = keras .Input(shape=(sequence_length, raw_data .shape[-1]))
    x, Ni = 1.ayers.LSTM(16)(inputs), ' 1stm'
    # x, m = layers.GRU(16)(inputs), ' gru'
    outputs = layers.Dense(1)(x)
    model = keras.Model(inputs, outputs)
    model_name = models_path + f '3_jena_{m}' + fx

    callbacks = [ keras . calibacks. ModelCheckpoint (model_name,
                                                      save_best_only=True)]

    model.compile(optimizer=' rmsprop ' J loss='mse', metric뇌' mae ' 〕）

    history = model.fit (X_train, y_train,
                        epochs=10,
                        validation_data=(X_val., y_vafl,
                        callbacks=callbacks)
                                                                              -J
＠임베디드 전문가 그룹 윌텍                    - 282 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 277 =====
5부. RNN                                2과. RNN Models




@）임베디드 전문가 그룹 윌텍   - 283 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 278 =====
5부. RNN                                                           2과. RNN Models


  RNN: 시계열 데이터 기반 온도 예측
                      （3/9)                                        밈升다드 전：」l가 죠룹 묄디，


  孕［예제 시 기본 RNN + Dropout 모델
                                                         十긱士，
                                               Lf 1너t 』（L＼
    inputs = keras,Input(s 'pe=(sequence_l.ength, raw_data. shape[-1]))
    x, m = l.ayers.LSTM(    r ecur ent_dro out=0.  (inputs), 'lstm'
    # x, m = iayers.GRU 2, recurrent_ r opou - .25)(inputs), ' gru'
    x = l.ayers.Dropout(B.5)(x)
    outputs = layers.Dense(1)(x)
    model. = keras.Model(inputs, outputs)
    model_name = models_path + f '4_jena_{m}_dropout ' + fx

    cailbacks = [keras.cafl.backs.Model.Checkpoint(model_name,
                                                   save_best_only=True)II

    model.. compile(optimizer=' rmsprop ' J l.oss='mse ' ) metrics=
                                                                  〔' mae ' 〕）
    history = model.fit (X_train, y_train,
                         epochs=20,
                         val.idation_data=(X_val, y_vafl,
                         caflbacks=cal.thacks)




 陌胥. : 社ㅐ뉜 뻬vC '\)" 기읠가흼 CGnH" fr. ia미




＠임베디드 전문가 그룹 윌텍                      - 284 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 279 =====
5부. 刪N                                                                      2과. RNN Models


 RNN: 시계열 데이터 기반 온도 예측
                     （4/9)                                                   CODEXPERT
                                                                             임베디드 전문가 그룹 윌텍


   0 기본 모델 + Dropout 결과
                               LSTM + DO              LSTM               Naive
          Validation                2.36 (‘駙色         2.41
             Test                   2.66 (거%i-)       2.60

              Training and validation MAE                Training and vaIidaton MAE
                                                                        -     季aming MAE
                                                                            ∼ VahdMun 跳AE




@）임베디드 전문가 그룹 윌텍                            - 285 -   무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 280 =====
5부. RNN                                                                                                                                 2과. RNN Models


  RNN: 시계열 데이터 기반 온도 예측
                      （5/9)                                                                                                             입베다느 젼문가 그를 윔텍


  Q［예제 5] Stacked RNN 모델
      inputs = keras.Input(shape=(sequence_length, raw_data.shape[-l]))
      x, m = layers.LSTM(16, recurrent dro
                                                    inputs), ' 1.stm'



      X# # #
             =
          七yers.LSTM(
          " ' /
               1wprc楡rer
                  一뺨
                      (7 ㄴ－n,
                         rriirrnf
                       ∼떼一 J
                               _.ropout=0
                                      drnnnii,UX',JJ. , . \V4
                             ' ' k' 一－U' 빅∼小．
                               `/ 1   M   → -   ' ` ∼
                                                              e eN\(,C 3fl27
                                                           , , ,
                                                        \ ｀〃수m J   '
                                                                       T t'I
                                                                       `m M *. .   1   `7 . ㅐ `   - ｀〃1      ｀〃`'
                                                                                                          1戶＇』      `*   `/   m `7 J


                              return-sequences= I rueㅆin恥』
                                                         ｛돠j                                                                           9ru   力
                                                                                                                                             「 /) ·
       x = layers.GRU(32) re繃rrent_dropout=0. 5乂x)
     x = layers.Dropout(0.5)(x)
     # x = layers.Qense(16)(x)
     # x = layers .Dropout《O.5)(x)
     outputs = layers.Dense(1)(x)
     model = keras.Model(inputs, outputs)

     calibacks =〔 keras.cailbacks.ModelCheckpoint(model_name,
                                                       save_best_on1y=True)]
     model.compile(optimizer=' rmsprop ' ' loss= 'mse', metrics=[mae' ])
     history = model.fit (X_train, y_train,
                         epo轍s=20,
                         validation_data=(X_val, y_val),
                         callbacks=callbacks)




＠임베디드 전문가 그룹 윌텍                                                                         - 286 -                     무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 281 =====
5부. RNN                                                                           14. RNN Models

  RNN: 시계열 데이터 기반 온도 예측
                      （6/9)                                                         CODEAPERT
                                                                                    임베디드 전문가 그룹 윌텍

   . Stacked RNN model 결과
                             Stacked LSTM              LSTM + D0                LSTM
           Validation                2.36                   z36                  2.41
              Test                  2.53                    2.66                 2.60

               Training and validation MAE                     Training and validation MAE




                                                       z4




＠임베디드 전문가 그룹 윌텍                              - 287 -        무단 전재, 복제, 발췌. 디지털화 금지


===== PAGE 282 =====
5부. RNN                                                                                       2과. RNN Models


      RNN: 시계열 데이터 기반 온도 예측
                          （7/9)                                                                CODEAPERT
叫喚枷
                                                                                               우］困디드 선문기 그룹 윌텍


      磅 F예제 히 미direction키 RNN 모덛l 겸과 걱토                                 . .               .
                                           ＝-, ,5/. ::3, ^r尸，
                                          二」                Uㅣ        (7!=H;l活℃           刊r기
                                     //      7 =＞        V닙   '   …   스ㅍ      －       -       I \r…
       inputs = keras.Input(shape=(sequence_length, raw_data .shape[-13))
                                                                                  '
                                                    珊I
       x , m = layers.Bidirecti(i al(layers.LSTM( 16) Vinout引, ' lstm'
       rx = tayers tsiairectionau tayers.帥nKlbj八in硏itS)) '9rir
       outputs = layers.Dense(1)(x)
       model = keras.Model(inputs, outputs)

       calibacks = [keras.callbacks.ModelCheckpoint(model_name,
                                                    save_best_only=True)J

       model.c0cnpile(optimizer= ' rmsprop ' J loss= ' mse ' J metrics=[ ' mae ' 〕）
       history = rnodel.fit (X_train, y_train,
                            epochs=i乞
                            validatioa_data=(X_val, y_val),
                            callba댜〔s=callbacks)

                                  （섬汕十 헌닥늰 의젼으 앗乞．




@）임베디드 전문가 그룹 윌텍                           - 288 -                무단 전제, 복제, 발췌. 디지털화 금지


===== PAGE 283 =====
5부. RNN                                            2과. RNN Models




                  -- 11aIn튠rg MAE
                  -－∼ V비idation MAE




 임베디드 전문가 그룹 윌텍
C）                             - 289 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 284 =====
5부. RNN                                                             2과. RNN Models


  RNN: 시계열 데이터 기반 온도 예측
                      （9/9)                                          CODEXPERT
                                                                     임볘디드 전문가 그룹 윌텍


  @ LSTM vs GRU 모델 결과 비교
   聾LSTM이 overfitting이 좀더 빨리 발생하고 있음
    l* tf version 2.17: (nnn) -* w/o Recurrent DO

                        BiD LSTM       S嫩 LSTM      LSTM+DO        LSTM
          Validation    2.38(2.40)    2 .36(2.37)   2.36(2.35)   2.41(2.36)
             Test       2.58(2.51)    2.53(2.56)    2.66(2.54)   2.60(2.55)
           Param#          4001          8289         6049         2001


                         BID GRU       Stk GRU       GRt卄DO        GRU
          Validation    2.42(2.32)    2.27(2.29)    2.29(2.32)   2.36(2.32)
             Test       2.50(2.44)    2.40(2.45)    2.43(2.45)   2.48(2.45)
           Param#          3105          6369         4641         1553




@）임베디드 전문가 그룹 윌텍                        - 290 -     무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 285 =====
5부. RNN                                                          24. RNN Models
                                                                 珊驪聽啣一쀼轝雕難難珊珊




  RNN model 개선 방안                                                 CODEXPERT
                                                                  임베디드 전문가 그룹 윌텍


  匹itAjj
             .Time sequence feature extraction up
             0 Dropout rate 조정 필요
   @T6ptim           izer
                                              나 三 b塊，
             口RNN layer 와 .utput layer 사이에 추가
             ● RNN layer 출력을 regression
             삡可ata닝 1ㄹL)
              TSequence size
             ● Sami川ng rate 조정
             S Fea
                                        한다




@）임베디드 전문가 그룹 윌텍                             - 291 -   무단 전재, 복제, 발췌, 디지털화 금지


===== PAGE 286 =====
5부. RNN                               2과. RNN Models




＠임베디드 전문가 그룹 윌텍   - 292 -   무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 287 =====
α 트맬 트브로
uㄱ『－· I-=1


===== PAGE 288 =====
6부. 부록                                 1과. Numpy 라이브러리




              3과. Keras 2델 섕청. 저장 및 興원
              4과, Matplot 라0浮1a




@）임베디드 전문가 그룹 윌텍      - 295 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 289 =====
6부. 부록                                                             1고F. Numpy 라이브러리


  NumPy(www.numpy.org)
  @ 2006년에 출시된Python순鞭峻曼라의부르」
                            괴
   會 머신러닝. 딥러닝에 필요한 다양한 기능들을 제공
   學NumPy2In브arraγ jimensi앤힌쁘臾yt
    ,1- An array object represents a multidimensional, homogeneous array of fixed-size items
    /2 과학적 계산을 위해 하드웨어가 효율적으로 처리할 수 있는 구조
    r+ C언어의 배열과 유사한 특징을 가짐
                         （연속적인 메모리 배치）




@）임베디드 전문가 그룹 윌텍                         - 296 -     무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 290 =====
6부. 부록                                                           1과. Numpy 라이브러리

                                                                     C0DEXPERT
  List2F NumPy Array                                                 김뺘디드 쟌눈：기 교每 封:11


  Q Import Numpy

               import numpy as np


  Q［예제 1] Python vs NumPy
            00-9999 까지 10000개의 숫자를 제곱 하는 연산

                               = range(10000)
  rL-rytiiuri
     fl. L_ .LISt
              =-1nJ       '=                 -   크｀
                               j**2 for i in u.:

                         －→［三晤편찬시갖측정I
                          뇨 = np . arange(10000)
   -NumPy        Array
                         4a**21
                                                                                     ㅈ   )




〔E                       쁘on ListOll I 1I NumPy Array갔뎅tIF. 켄첫롼箕




＠임베디드 전문가 그룹 윌텍                                  - 297 -   무단 전재. 복제, 발췌, 디지털화금지


===== PAGE 291 =====
6부. 부록                                                                                                         1과. Numpy 라이브러리
         ’「…       m…        …                                                                                 珊‘嚼媛季努渗坤毓塑璘耀驩難舞參輾灘옳蒜珊；難冬小3發柱




  np,ndarray                                                                                                          多P驢쁘싸「
  @ Attributes
           구분                                                                             설명
     arr.ndim           · 배열의 깊이
                               （차원）

    스rr",h'二，,.         ' 각차원 별요소걘숙정보를가진 배열의구조        （tu이e형태）정보
    " " " " HH느         . 2행 3열인 경우仁. 3))0쿠 표시되고. 1차원 구조는（5 ）와같이 표시됨
   -－…                                                     \   .       〃
                                                                       ．
                                                                                          -------                 n             →   ,   1




    arr.dtype           · 생성된배열의데6펴타입에대한정보                                                                     앗d介y느      D욉 놘J긴

    arr.itemsize        · item의 메모리 사용 byte 수                          ------                           ／〃｀\
                                      -             --~-           -




    arr.size            · 배열의 item 개수. 2행 3열인 경우＄izeF6 /)                                           \．∼y-
  Q Methods

          구분                                                                              설명
    arr.reshapeO        · Array를 주어진 shape우로 변경하여 return
                          ( ` "느/'.       .   \/'
    arr.transposeO      · Axis가 transpose 된 Ajjay를 return
                                                                   /`,/         \/\/ ,/
    arr.copyO           · Array를복사하여 return
                                   八／,/^/




＠임베디드 전문가 그룹 윌텍                                                            - 298 -        무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 292 =====
6부. 부록                                                                                                          1과. Numpy 라이브러리


  Create array: np.array()                                                                                                 임베디드 전문가 그룹 윌텍


                                                                     np.array(array-like)

      a궉'9·큰rray([o, 1, 2, 3])                                                                                    /
                                                                                                                                                                                 -
                                                                                                                                                    .                .    -\


      print} a) '. . ,
                                                                                                                                         -:
                                                                                                                  l                 a.
                                                                                                                                     ,naim                       =    I .
      print` a.nu끄하                                                                0        1       2       3     - a.snape =딴,) ㅣ
      print
                                                             )                                                                                                                   7
                       (a.
         print        (len
                                          shape)
                                                   (a)                                                            (,                Ien`a)='4

  - -b -.
        = IL
          np.array([[@, 1, 21, [3, 4, 51])
  1     prini                u)                    ',    .   ,
                                                                                            0       1       2                b.ndim = 2
  - print}::．·foul'L                                                                                                       b.shape =(2,3)
    prin다U, ，斗튼띳引                                                                           3       4       5                len(b) 2                       =

      print t i.enUU J                                                                                                                  夕

         np.array([F [1], [211/[[3], [41]I)
      註,nt(c)
                                                                                                                   /                          .. -T-Th

                              .
                                                                                                                  굼．
                                                                                                                  c.,C.fl( shap칼m                       =   (2,
                                                                                                                                                            (=       3
                                                                                                                                                                     2,     11
                                                                 )                                      4                                                            2
                                  ndim)
      print
                                                                     : 『乂1시
                     (듣，
                                  shave)
                                                                                                2                                                                                1
                                                                                                                   ，∼len
                                                                                                                                                            =
                                                                                                                                              (c)
      printI. Len`c J '

                 array-like: lists. lists of tupIes, tuples, tuples of tuples, tuples of lists and ndarrays




＠임베디드 전문가 그룹 윌텍                                                                  - 299 .        무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 293 =====
6부. 부록                                                                                                                               1과. Numpy 라이브러리


  Create array: 특정 형태의 array 생성                                                                                                                CODEXPERT
                                                                                                                                               임볘디드 전문가 그룹 윌텍



  l小
                         np.ones(出ape)                       t                                  np.onesJke(irray_Uke)

                                                             a            =   , . ,
                                                                                .   I .

       可＝叩.one5((3, 3))띄
                                                                                    [1,          2,        3,         41                              ,,                .         .        ,,



                                                             a－므K9 =. nP.Ones_J.iKeka) LP ㅣ - 니
                                                             print` a_liKe)
       print*   .a   '                 h.
                         np.zeros(shape)                                                        np.zeros_Iike(array_Iike)

                                                             b                      [[1,
       b = np.zeros((2, 2))                 [{0. 0.1                                                                        J                         [[,
                                                                                                                 3]        ,         s,
                                                                                                                               [4,
                                                                                                      2,
                                                                                                                 p. er。s_1ike                   (b)            0.
                                                                                                                                                                             D，       미，   ,,

       print(b)                              [0. 0,]]
                                                                          4ik
                                                                          =i                                                              6]
                                                             priflt(D_liKe)                                                                                LU u ujj
                                                                 b_
                         np.eye(N[,MLk1])                                                       np.empty_Iike(array_Iike)

                                      [[1. 0. 0.]            C = [[1,21,[3,4]1      . .
       C = np. eye(3)
       printt이
                                       [0. 1 . 0.1
                                       [0. 0. 1 .]]
                                                             c_          empty_like
                                                               like: like)
                                                                     l
                                                                 print                    (c_
                                                                                                           np.
                                                                                                                                                (c)
                                                                                                                                                           "        i       3 411
                                                                         arrayjike와 동일shape의 array 생성하는 항수
       shape올 가진 해당 형식의 array 생성하는 항수                                      (empty_like 9 uninitialized array 생성）




＠임베디드 전문가 그룹 윌텍                                         - 300 -                     무단 전재. 복제, 발췌. 디지털화금지


===== PAGE 294 =====
6부. 부록                                                                       1과. Numpy 라이브러리


…numpy의자료형                                                                          …*1jqE驪，J.;，「「
  @ numpy 자료형 분류
          자료형                                                      종류
                              …1




   부호 있는 정수형
           （int)    1nt8, intl6, int32, int64

   부호 없는 정수형
           （uint)   uint8, uintl6, uint32, uint64

   실수형(fIoat)       floati 6, float32, float64. floati 28

   복소수(compIex)     c0mp1ex64, comp1ex128, comp1ex256                               采 介le   ，吐乞
   부울형
     （bo이ean)       bo이                                                                 (P(너 \)／決小7Y1,
                                                                                                  71
   운자열              bytes_(byte string), str_(unicode string)

   객체               object, Container자료형들은object로 취급함


   ,！쁘쓰쁘찬르望르르妗*陪뻗쁘쓰쁘쁘float3？완乫丕擊呼형事*陪
                          ,        ' ,   /`/    \/ ，느낚→｀./   ,,/   ∼－   ∼∼   가 ‘-




C）
 임베디드 전문가 그룹 윌텍                                - 301 -       무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 295 =====
6부. 부록                                                                                    1과. Numpy 라이브러리

                                                                                                COD … ' ……'
  np.ndarray I dtype                                                                            임베디드 전문가 그룹 윌텍

   穹array 데이터의 요소타입에 맞게 결정
     a     =   np.
                           array   ([                                        parameter로 전달된     int64
                                                               )
                                        1,   2,
     print           (a.
                               dtypeT                     31
                                                                        array의 요소타입에 맞게 결정 됨    f oat 64
                                                                                                com Iex128
                           array   ([
                            dtype)1"              2   "             )                           bㅇ이
          rint(b
                                                               "]
     믐=        np.
                           .




     ( = np.array( I !t?i1 3+4j.-S+6*1_jJ)
     print.c .citype)
     d = nn.arrav(F True Fa1se Fa1se TrueD
     printUJ.cltype)

   已 생성 될 array의 요소 타입 직접 지정

     e = np.array(!1, 2, 3], dtypeㅌfloat)                                                      n oat
                                         parameter
     pr]ntL e. atype)                                                                          i nt ．궉
                                       dtype에 지정된
     f= 岬.array(!1., 乙，王1, dtype=int) type으로결정됨
     printIt.atype)




＠임베디드 전문가 그룹 윌텍                                                          - 302 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 296 =====
6부. 부록                              1과. Numpy 라이브러리




@）임베디드 전문가 그룹 윌텍   - 303 -   무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 297 =====
6부. 부록                                                            1과. Numpy 라이브러리


 Indexing of array
  @ Indexing: 배열 요소 접근
   . 1차 배열
    a       =,    (a了   range
                                 (10)   양수 ‘dx
                 np.
                             l
    print
    print         (a[   O}
    9LLfltld[引）
    print(a[                            음수idx




@）임베디드 전문가 그룹 윌텍                                 - 304 -   무단 전재, 복제, 발췌. 디지털화 금지


===== PAGE 298 =====
6부. 부록                                                     1과. Numpy 라이브러리


  Slicing of array(1)                                              CODEXPERT
                                                                   임베디드 전문가 그룝 윌텍


  孕 다음 결과를 예상해보자

                                0   1   2     3    4   5   5   7     8    9
    a = np.arange(10)
                            a   0   1   2     3    4   5   6   7     B    9
    print(a, '\n')

    print(a[2:9:3], '\n')

    prInt(aE :4J . '\n')

    print(a[1:3J, '\n')

    print(a[::2],'\n')

    print(a[3: J, '\a')




C）
 임베디드 전문가 그룹 윌텍                     - 305 -       무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 299 =====
6부. 부록                                                                       1과. Numpy 라이브러리


  Slicing of array(2)                                                                CODEXPERT
                                                                                     임베디드 진문가 그룝 윌텍


  俓｝다음 결과를 예상해보자

                                             0   1      2      3     4   5   6   7     8    9
    a = np.arange(10)                    a   0   l      2      3     4   5   6   7     8   9
    p근nt(a, 스nJ
    dID. ] =                W
    print(a. '\n')




    b = np.arange(5)                     b
    print(b, ,'\n'),,

    dID.                        '
                                         찰큉찬 겅우는
                          ?（而
    print   ](   (a   =             I\
                                             （多겨避 ei 'c )




@）임베디드 전문가 그룹 윌텍                                     - 306 -       무단 전재, 복제, 발췌. 디지털화 금지


===== PAGE 300 =====
6부. 부록                                                                              1과. Numpy 라이브러리


  Dimension reduction(1)                                                                      임베디드 전문가 그룹 윌텍


  @ Array의 차원을 감소시키는 연산

  Q np.sumO, np.ndarray.sum()                    r一
                                                 ; shape of array(ndim=N)
   . 합계를 구하는 함수
    x = np.array([i, 2, 3, 4])
                                                              (!i．기bJ 嵐切,，... ,!n)
                                             -                    il "`              "   -닒      "   "   -   , *

                                       axisO      axisi       ax1s2       ax1s3    axis(N-1)
    叫nt1끄p노斗煦）)                       axis(-N) axis(-N-i-1)axis(-N-i-2) axis(-N+3) axis(-1)
    printkx.s브띤．
               , /J


   . 특정 축을 기준으로 합계 구하기
    x = np.array([[孕, 1], [2, 2]])
                                                                   ㅇ 쓰× 띠
                                                                            1   1
    print(x. sum(ax1s=0)》                                                   2   2

    print(x.sum( axisl ) )
                                                                                                         「)
                                                                                              x.suni(axis=
                                                 '    /   '   一




                                      x 1sum axis＝이




＠임베디드 전문가 그룹 윌텍                      - 307 -              무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 301 =====
6부. 부록                                                                                         1과. Numpy 라이브러리




     x = np.array([i, 3, 21)

     叫nt(x.min())
     prlntLx . maxU J

     叫nt(x·argmin(n
     printtx . argmaxu '



     x =     np.
                       array   ([[9,   2,   io.
                                              ,6,   1J,   [5,    7,   3,   4,   81]   )
                                                                                           9   2   10   5        1
         .         ,           . .     . LJ,()
                                            . `
     隘緞x.          s1); 결과는？
         argmin(.(業s0)
       x argmax                                                                            5   7   3    4   （욘
.임베디드 전문가 그룹 윌텍                                                 - 308 -               무단 전재. 복제, 발췌. 디지털화금지


===== PAGE 302 =====
6부. 부록                                                                             1과. Numpy 라이브러리


  티
  Element-wise operation
    ement.Wi5eoperationandbroa-'(a5t
                          broaucast                                                          CODE P 「
                                                                                                    ，，
  @ Scaiar value와 array의 연산

    a = np.arraγ  (Ei,   2,   3,             1)
    謐nt'(n*")a)               跡畝「必七"是                       +     +    +     +




                                                                                                           )4
  Q Array간의 연산                                            `*`    lㅊ｀   弓t1    4디           ) ' 亡 >3

    ' a = np. arange(4)              talueError                                   Traceback (most recent cal - last)
      a + np.array([1, 2])         l 드ipymor-i nput -27-659bcd5U8c9e' in !:m)duI e>O
                                           I a m nt.arange(4)
                                     ---> 2 a + noarray([1,

                                   :ValueError: ooeran a could not be broadcast       ether with shaoes (4i (2, )
                                     r
                                     1
                                                  Broadcast: 서로 다른 寸tape을 가진 array의
                                     1
                                     毛
                                     , , l           산술 연산을 위해 NumPy가 가진 규칙




@）임베디드 전문가 그룹 윌텍                                    - 309 -       무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 303 =====
6부. 부록                            1과. Numpy 라이브러리




C）
 임베디드 전문가 그룹 윌텍   -310 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 304 =====
6부. 부록                                                1과. Numpy 라이브러리


  Broadcasting Rule(1)                                          임버I디드 전문가 그룝 윌텍


  @ array - scalar
         np.array([1, 2, 31)
         2
         a+ b

   [1 2 3] , a.shape = (3,)
   2, bshepe = O                                scalar 4 (3W)         (3, )
   [3 4 5] , o ,shape = (3,)

  孕array - array example 1




   [[1 2 3]
    [4 5 6]] , a.shape = (2, 3)
                                    (2, 3)     (3,)-}(2,3)            (2,3)
   [1 2 3] 』 b.shaDe = (3,)
   [[2 4 6]
    [5 7 9]] , cshape = (2, 3)                 cLe 耐如斗




@）임베디드 전문가 그룹 윌텍                  -311 -     무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 305 =====
6부. 부록                                                                         1과. Numpy 라이브러리


  Broadcasting Rule(2)                                                              CODEXPERT
                                                                                    임베디드 전문가 그룹 욀텍

  @ array - array example 2
   a = no.arrav(' [ i 2 3 41)
   0 = np.array`EL1J, [U』I,                                          stretch
   《＝ = a+ b                                            stretch -
  [1 2 3 4L a.shape = (4,)
  [[1J
   [2nJ b.shape 口 (2J 1)
  [[2 3 4 5]
  〔3456nJc. shape =《2, 4)                                           (2,1) 4 (2,4)

  @ array - array example 3




   [[1]                    n2 3 4]
    [2]                    [34 기
    [3]                     [4 5 6]
   〔4弦 a.shape = (4, 1) {567〕      L c.shape = (4, 3)
   [1 2 3], b.shape = (3,)




@）임베디드 전문가 그룹 윌텍                              -312 ~        무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 306 =====
6부. 부록                                                                       1과. Numpy 라이브러리


  Array Manipulation
  l等 티attening: 다차원 배열 춈 1차 배열로 전환
    4. np.ndarray.ravel() 4 flattened arrayf ai




  @Re닦iaping: 배열의 원하는 shape으로 변경
    4. np.ndarray.reshapeO O'IQ

   a = np.array([[1, 2, 3], [4, 5, 61])                          1

   b = a.reshape((6, 1))                                         2
   print (b)                                                     3
  〔 = a. reshape(櫓. 2)) - 다른shape정보                              4
   print(댜           .,1F n바탕으로자동결정
                             '       `                           J

   print(a.reshape((-1,3)))                                      ＇괵




                                               杆W
                                                         \
                     (? b "卜 ';!"넴
                                 「                       7
                                                                      쭈
                                             ㄱl니   C午＼
                                                                 L
                                                                 l
                         (               )
                                                             ＇
     α加
                                                             ㄴ
            '나   "   "       -   1   ,
     q，
      加qL9什 C니 )




@）임베디드 전문가 그룹 윌텍                             -313 -                   무단 전재, 복제. 발췌, 디지털화 금지


===== PAGE 307 =====
6부. 부록                      2과. Tensorfiow 프로그래밍 기초




＠임베디드 전문가 그룹 윌텍   -314 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 308 =====
6부. 부록                                                                    2과. Tensorflow 프로그래밍 기초


 lensorFiow                                                                                       CODEXPERT
                                                                                                  임베디드 전문가 그룹 윌텍

   臼Goo이e이 2015년 11월에 공개한 end to end 오픈소스 머신러닝 퓰랫폼
   .Tensor

            ＾ㅎF/nL斛         A tensor is a geometric object that maps in a multi-linear manner
            -v- il- -I- i             -   1=     ㅗ       i       1   1l    t       .    -
                            geomeuic vectors〃 scdiir毛 ano otner tensors to a resuiting tensor


                                           are muiti-dimensional arrays with a uniform type
     k05.
     Te
             nso
               『디애
                 rFlow
                            Tensors
                            4 If y。
                                  ure             iliarwit    m      eis。 are   (kind
                                                                                                    (dtype)
                                                                                         like np.arrays
                                                                                            。f)
   .Tensorflow
    tl' 텐서를 포함한 연산을 정의하고 실행하는 프레임워크
   ' TensorFlow를 사용하는 이유
                                                                                                     卞
                                                                                                  TensorFiow
    tl- 손쉬운 모델 빌드
            ’《 다양한 수준의 추상화를 제공 춈 사용자의 수준에 맞게 선택 사용가능
    4. 어디서든 강력한 Machine Learning 제작
            x Server나 edge device 또는 Web에서 언어 또는 플랫폼 별 M〔 모델을 쉽게 학습 및 배포 가능
            x TensorFlow Lite: Mobile. Embedded Device에 적용 가능한 경량화 된 library




@）임베디드 전문가 그룹 윌텍                                       -315 -        무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 309 =====
6부. 부록                                                                            2과. Tensorflow프로그래밍 기초
 「
 「
     …∼…                    「蜘’   如螂嚼姆一嶼群瀜娥嚼蜘烈斟巒蜘                           ‘蜘呻        「蜘幽姆娥鹽羽輾棘姆甲＝
     기본적인Tensor및생성방법 '                                                                                  , 客覡훑，
                                                                                                             므野「’
     @ tf.Tensor의 기본 속성
     (   dtype:      data
       ,4 Tensor 값의 Type
                                  塑)
      .4 Tensor 값의 각각의 element들은 모두 같은 data type을 가짐
     ● 퇘ape
       /s. 각 차원에 대한 크기를 가지고 있는 숫자들
      'I. 차원의 크기가 ' ?'인 경우：해당 크기는 runtime시 상황에 따라 달라질 수 있음을 의미
     @ Tensor 생성과 관련된 Class/Method
                  Name                   형식                                       Description

      tf.Variable                      Class    -                                                     에執닐 .H

      tf.constant                      Method   Creates a constant tensor




@）임베디드 전문가 그룹 윌텍                                           -316 -       무단 전재, 복제, 발췌. 디지털화 금지


===== PAGE 310 =====
6부. 부록                                                               2과. Tensorflow프로그래밍 기초


「 Constant: tf.constant                                                                           tE,:,, I;;，…
    0 Creates a constant tensor
   I`                 tf.constant(value, dtype= None, shape= None, name= 'Const')                                 7


    .Attribute                        잃받컥으t ㅔ0仄大22
               Name                                         Description
        value              A constant value(or list) of output type dtype
        dtype              The type of the elements of the resulting tensor.
        name               Optional name for the tensor

    0 Rank of value
        Rank                  Description                                 Example                      Shape
         0      Scalar(magnitude only)                    1 ,-4. .0.142                           ()
         1      Vector(magnitude and direction)           [1. , 2., 3.]                           (3. )
          2     Matrix(table of numbers)                  [[1.. 2., 3.], [4.. 5.. 6.]]       /
                                                                                                 _-4. 3)
                                                                                                       ,,/
                                                                                         /
          3      3-Tensor(cube of numbers)                [[[1..2..3.]], [[4., 5.. 6.]1Y          (2, 1, 3)
                                                                                    /
                                                                                  / U이긱咤 드＼叫꺼 21

                                                                                  \.
                                                                                   쓰가꾸＞h먀                    ㅍ＞




@）임베디드 전문가 그룹 윌텍                                   -317 -         무단 전재, 복제. 발췌. 디지털화금지


===== PAGE 311 =====
6부. 부록                                                                  2과. Tensor뛰ow 프로그래밍 기초


  tf.constant의 사용                                                                           CODEXPER
                                                                                            임배다드 전문가 그푭 윌텍



  《3.}！예제 2] tf.constant를 이용한 상수 tensor 생성 예제
       c_mnt = tf. constant(3)
       c floati = tf. constant(1.239)
       《＝ tloat2 = tt . constant( 3 . dtvDe= tt. tJ.0at32 )
       c_str = tt. constant("Hello. TensorFiow' . name= ' Const_String ' J

       list_constant = [c_mnt. c_floatl, c_f1oat2, c_str]

       for tensor in list constant:
         print(tensor, "value = {}" .format(tensor.numpyO))
                                                                 nstant는 value, shape. dtype의 순서로
                                                                              ==＝갸

       tf .Tensor(3, shape=O''. ype=int32) val
                                                                 ---     --




                                                                                     .J
       tf .Tensor(1 .239, shape#(), dtype=f Ioat32) value = 1 .2389999628067017
       tf．              dtype=f쁘르 2)싸aI』ue = 3:0. .
         工ensor(M식shape朴，                           V키ue
       tr rensoro i-iei io, ensori- low , 3r1HDe=c) ,（끄ype=stF ] ri刀             el lo, TensorFtow'
   /

                    · None: value따라자동설정，
        dtype
                    · 지정 시：지정 형태로 설정 （ value가 타입에 맞아야 함 ,아니면 'TypeError 발생）
   r            ㅣ
                    · tf.constant의 name은 생성 시 미설정 하면 기본 Const가 부여 됨
                '



        name
   \
                    · 동일 이름의 Tensor가 존재하면 '-n' 형태의 번호를 붙여 동일 이름의 Tensor 생성 회피




＠임베디드 전문가 그룹 윌텍                                      -318 -            무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 312 =====
6부. 부록                                                                 2과. Tensor-flow 프로그래밍 기초


「 tf.DType                                                                                                    스益區，
                                                                                                                 ，三；
                                                                                                                   ，구
  Q Tensor으1 요소 타입
                  Type                                             Description
    tf.float[16.32,641         [half, single, doublel-precision floating-point
    tf.bfloatl6                16-bit truncated floating-point                  e청，
                                                                                  pn`P戚k = e- c \):-i
                                                                                    -       ,                                   .    .       ,   I   ", \/
    tf.int[8,16,32,64]         Signed integer                                       +m*}0，
                                                                                         久 二 fl l= tJ
    tf.uint[8.16.32,641        Unsigned integer
    tf.bo이                     B 이ean
    tf.string                  String

  孕 각 type 별 표현 범위를 출력하는 코드
                                                   (
                                                               .
                                                       .   .       .   ..   .   .       .       ...   .   .   =1   .   ｀·   , . ．山   ,
                                                 ,-*i t . m1n= t 브i a. ra ?unatltl셔 쇠소｀{ 믄r뫈                                             訂

         Print` TFTTpe(tit1e.
    defnrint죙               ,. list:types): n
                 U 1 .Tormatttitie; '       !
                                              j..max:
                                                ．슭驪i1 t i'4data' 'JW길H
                                                                  typeOflAl
                                                                       ' I4醉1CfljI_
      [prini( "'{ :ie} .: {} ∼ {} " .forinat(t.nami-.1뇨쨘i工； ..jq8)) for t in list_typesi
                                                          ._t.
    list_types_float = [tf.floatl6, tf.f1oat32, tf.f1oat64]

    Print_TF_Type("Min.Max of tf.float[16,32,64]",list_types_float)




＠임베디드 전문가 그룹 윌텍                              -319 -                무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 313 =====
6부. 부록                                                                               2과. Tensorflow 프로그래밍 기초

                                                                                                                     COD
                                                                                                                     임베디드 전문가 그룹 윌텍


  Q lensorFiow convention$ 내의 Tensor의 [)imension에 대한 내용
    ●'lensorFiow code style guide'에 기술된 내용
         4' Batch operation의 Tensor 첫번째 dimension은 batch dimension으로 가정
         f2 마지막 dimension은 channel의 수로 사용 합
         4. 첫 번째와 마지막을 제외한 나머지 Dimension들은 space dimensions을 구성 합

  @Hi아，
      er rank of Tensor(image）
                             를정의한예제,., bat出，height. wid仇channel i
                                                                     '                                           `
        Datcn_images = ti. constant(u , I snape =(1U, 14U, 31I), 3)i
                                   -   -    ,_     r.                    』   →   -   -   -   -   -   -   -   `




   /m
          mann이：3
           (RGB)                                        batch size: 10 images
                                                                                                                                 +\
                                           1mage                             !maqe



                    width: 320px

                                                                 e       =




                                                                             閃b(（
                                                                                CL『＼小노                                乙h이 m七




＠임베디드 전문가 그룹 윌텍                                         . 320 -                  무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 314 =====
6부. 부록                                                                 2과. Tensorflow 프로그래밍 기초
灸聳狐妊孔m姚曲稷轝北柳않唯γ甘허渤토ㅊ聃木겼코캬出毖k∼，
                             嚼余얹쑈形一 e-   *pr*      －∼   -如一李的形月幽姸楓*形押獅騙藪嶼幽棚啣出凞뿟杉乞繫




    Variable: tf.Varia비e
    Variaㄴde:    Variable                                                                         9 ItEi 7l
                                                                                                  CODEXPERT
     @ tf.Variable: Class
       . operation 실행에 의해 값을 조정：Weights of Neural Network

     孕 변수의 생성
       $ tf.Variable Class의《:onstructor를 통해 만들 수 있음

     ㅣ1                     _init_(initial_value= Non(三inable= True, 今pe= None,")                         .「
                                                                                                           사等노
                                                                                                               -^
       --            －…                    「 --         '<=＝→         -<，
                                                                        ∼) '1 \      ' c   -   . '' 口｀'        '

              Name                                             Description
        initial_value        Variable I initial value
         trainable           True일 경우 Optimizer 사용시 해당 변수를 Training 함
         dtype               Variable의 type




@）임베디드 전문가 그룹 윌텍                                        - 321 .     무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 315 =====
6부. 부록                                                          2과. Tensorfiow프로그래밍 기초
                           〃          …        「   ……            「          mㅆ∼缸∼뜨→L



      r·n一a∼m `'- :,,1｀          ㄴ｀                                               rnn=p…r= …낙
      ㄴreatina
             1'
                variaDte                                             ,
                                                                                  一一 F『카
                                                                                       「 -
                                                                                  임베디드 전문가그룹 윌텍


      Q 상수를 초기값으로 하는 Varia비e 생성 예제
         var_i = tf.Variable(10) .    , ∼   . ∼ . －→
         var－르 = 브·Variable1外 므 YP：三rttJ三9 熙？, r type名i ,l
         var_i = tT.Var1aD1et3U, name=             YAK－떪eignt. L변수이륨정의 j

         list_ var = [var_i. var_2, var_31

         for tensor in list var:
           nrint( 'tensor = {}" .format(tensor))
           print( "" value = tJ ".tormat(tensor.numpyU))

        tensor = <tf , Variable ' Variable:0' shape=() dtype=int32, numpy=10>
        value = 10
        tensor = <tl .Variable 'Variable:0' shape=() dtype=110at64, numpy=20.0>
        value = 20.0
        tensor = <tf.Variable VAR_Welght:0' shape=() dtype=1nt32, numpy=30>
        value = 30




…肖乞
@）임베디드 전문가 그룹 윌텍                                - 322 -      무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 316 =====
6부. 부록                                                               2과. Tensorllow프로그래밍 기초


「 山nia비e의
  ；母1 --
         '초기
         "
            '값설정
             - -~ -
                    방법
                    - -
                                                                                      ∼！스一二：:.』』
                                                                                      임베디드전문가그룹윌텍


  Q 초기값 설정에 사용할 수 있는 함수
                        Name                                            Description
   tf.zeros(shape, dtype)                                  모든 원소가 0인 tensor 생성

    tf.ones(shape, dtype)                                  모든 원소가 1인 tensor 생성

    tf.eye(nurn_rows, num_columns, dtype)                  향등행렬 생성


  孕 특정 함수에 의해 만들어진 초기값을 사용하는 Variable 생성 예제

    var 1 = tf. Variable(tf .zeros( (2,3)))
    var 2 == tt. VariablettLones((i .5J))
    var_3 = tt. Variable(tt. eye(2,2j . name= " VAR_Weight " j

    list_ var = [var_i, var_2, var_31

    for tensor in list var:
         !   ' / $i 1     _   fl   "   L_ __. _._I 1_   ____\   ,
       pI-1, n뜨 ,, tensor - , V . ·. I 01Uld닷telisui I) ... ,
       printU"value = tJ . tormat`tensor.numpyIj))                       I 」각 변수에 대한 출력 내용은？




@）임베디드 전문가 그룹 윌텍                                        - 323 .     무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 317 =====
6부. 부록                                                            2과. Tensorflow 프로그래밍 기초
…→…"－   珌…           仁＝∼                                                   ……    느∼M     ∼n뇨    「헥뾔…위가姓쌩－侄꺄쁘孝1"뇨…「




  Variable의Random초기값설정방법                                                                              CODEXPERT
  《孕 초기값 설정에 사용할 수 있는 random 함수
                   Name                                                    Description

    tf.ra
    stdd썲om.normal(s.
          dtype, seed,hape,
                       name)mean,       헷으쯔씻istribution웃롯붕E1 Ra므브으므련7
    tf.random.truncated_normal
                              (shape,   a truncated normal distribution으로부                      E1의    Random값

    鷺·
    ；썼“잃歡；얍；’黑껜"'"'-                    a uniform distribution으로부터의Random값

             I
               / \, - norm비     -
                                         /
                                          / \\   `
                                                     truncated
                                                      nfl rrn 스1
                                                      1 1%J   1 ~ I   iJ    )
                                                                                           -Lunifo
                                                                                           1-
                                                                                                          'm.
     뇨締뇨MOII
 ,/，』，긔，
    var_i = tf. Variable(tf.random.normal((1,1))) , . . , , .   - ,.    ,, .   -
    var－三 = tr· variaine5tr.ranaom. truncat叩n雙niaxui,竗，j, uiean =, It),，吾tuuev = ti. I ' '
  - var_i = tr. var1ao1eItT.ranoom.un1Ton叭 t1,1J' minvai=o, maxvai=Iw"




@）임베디드 전문가 그룹 윌텍                         - 324 -          무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 318 =====
6부. 부록                            3과. Keras 모델 생성, 저강 및 복원




                    《 L샐 ㅂ 로－
                    '-i-i-. m i




              注!L Numpy aoj브aai
                Tensorflow 프盈J.2fl
              2과，
              3과. Keras모델생성, 저장및복원
              4p. M的궁4IQ aFOU!.21i




@）임베디드 전문가 그룹 윌텍        - 325 -   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 319 =====
6부. 부록                                                    3과. Keras 모델 생성. 저장 및 복원


  Mod비구성. 훈련및평가                                                              C叩),E 7LJ
                                                                                  EXPERTt
      Q [예제 3] keras model example: Sequential API 구조(basic)
      import tensorfiow as tf
      mnist = tf.keras.datasets.mnist
                                                                              1) Dataset
   似train, y_train),(x_test, y_test) = mnist.load_data{)
  'x._train, x_test = x_train / 155.t), x_test / zb518 51坐j그
   i而西－1＝珊f‘无F『＝百5F而而6珏＝56如面淺蘆百
       tf.keras. Input (shape=(28,28)
          tf.keras?t泊3".      {t6放r,
          tf.keras. 1.ayers.Dense(128) activation=' re1u'),            侖      2) Define
      ,   tf.keras.layers.Dense(10,
                                                                  汁－
                                      activation='softmpx.   ')                       ,

                                                                                      二
                                                                                          .4.
    I. name= >eauentia 1. rwaei i                `［斗，
                                                    ' ．一 ＇月U＞느＞
  ' m'        --1m-m--mi.．··－-'          :=::＝뾰쑈＝蚣－ m,'m
      model. compile(optimiz. - ' ,dam'                                ＾小力        '



                     loss=                                                    3) Compile
  '
                     metri ｀』스
                             ＇* accura
      model.fit ( x_tra. in, y'train, epochs
      mode.L.eva.Luate`x_test, y_test) 뉴
                                                    卜_                          4) Fit
                                                                              5) evaluate
                                          -I
          1모玉개요는tensorflow가이드참f [S사ce:https://www.t甲So世ow.
                                                        org/guide/keras/overview]
             的小…－，…－∼∼二∼？姦논쓰－…小∼
            匕，                 「
          Q1加*小「루） "'「":1 1




C）
 임베디드 전문가 그룹 윌텍                                - 326 -   무단 전재, 복제. 발췌, 디지털화 금지


===== PAGE 320 =====
6부. 부록                                                                                                        3과. Keras 모델 생성. 저장 및 복원


「
"   Functi。                          nal APr…                                                                    …                 …出     『l
                                                                                                                                               --   .   」    .-   .




                                                                                                                                        임베디드 전문가 그룹 월텍

              ● 함수 형태로 Layer 모델 정의 가능：Define 부분만 달라짐
                                                                                                                                                                                   -


              H"똬江，
                  밌keras.
                    .layers Flatten(
                          Input(shape=(
                                     )(i訊28))
                                          ts)                                                                                             - .Laye
                                                                                                                                              『정의1
              ,   xl堀
                  predicti。        tfker
                                      ns     "=   tf.
                                                  layers.
                                                     keras   Dense   layers   (128,    .   Dense   . activation=
                                                                                                        (l@  , activati。 n= ' s。
                                                                                                                     ;relu     ft mar)
                                                                                                                               '   )(x)                               (:  ,)
                                                                                                                                                                                   1


              !model. = tf,keras.Model.(lnputs=inputs,                                                                         E恥蟹：]
              -                                   d欌＝4 name=
                                                  CL4  outputs=
                                                            Functi。      del..)
                                                             ,predictions,
                                                                   nal._M。                                                                              -
                  Model: "Functional-Model"                          `’샤vt？十0씨盼mㅠ 瓦으p신 휑．                                                                                      皇
                              layer (type)                                                 Output Shape                                             Parair #

                              input_layer_i (InputLayeO                                    ( ［쿄씸슨， 28) 28)                                                            0        .


                              flatten_i (Flatten)                                          0. 8' 784)                                                                 e

                              dense-2 (Dense)                                              (. . w, 128)                                             100,480

                              dense_3 (Dense)                                              (3，
                                                                                             二lf3 l0)                                                       1 ,2아S




鞋璨轎攝轉韆幾薑參聲輧纛飜轉轟饔難蕣瑟潾辦蜘難料姓啣驪辦뇽磁岬鱗鬱料繫螂藝難冊蜘－                                                                                    轉翎畔鬱愍壑懈蘚礎璘雛                      iiii-

幽繃罐繃雌錨鹽蟲鹽驢轟磁發錢壅錢鹽轟雉磁鈿i楡雜嫡瑟鱗礪難灘轟礪- －攝i蜘                                                                          -衡崍蜘畔一繃補幽瀟－                                                    小




@）임베디드 전문가 그룹 윌텍                                                                      - 327 -                 무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 321 =====
    부
    부        쿄ㄱ
                                                          3과. Keras 모델 생성. 저강 및 복원
〃
b
    -    I         I
                                                                            CODEXPERT
    >uDciassing Pi-'I
                              -   -   1



                                                                            임베디드 전문가 그룹 윌텍


        口Class에서 기본적인 -_init_, call method 정의 후 model 객체 생성
        class MyModel(tf.keras.Model):
          祈芋＝ric= c§atf』name='! ii1r誌§y6dEr芍；                              사용할 Layer 정의
              super(MyModel, self).-_init__(name=name)                   _init__ : 생성 시 자동
              self.flatten = tf.keras. layers.Flatten()                  으로 호출되는 method
              self.dl == tf.keras.layers.Dense(128, activation=' relu')
              self.d2 = tf.keras.Lajers.DenseLl0 - activation=' soft!p ) j
         def call(self! , !)= , . l
                  x = seir.n』
                            ，atren(XI L d
                  x = self.dl (x2, .' 7- -     _lnit_ method 에서 정의한 Layer룹 사용
                  return se.Lr.oz`x)      I
                                          1


    !model = MyModelQ!                                  model instance 생성

                                                 유연성 증가
        G Subclassing API를사용 이유：伊속후customizing 장점，
        . 단. 복잡도가 증가하고 사용자 오류가 발생할 가능성이 높아지니 함수형 시：기 권고
          4 ten＄아ㅔow 홈페이지 가이드 참조




@）임베디드 전문가 그룹 윌텍                              - 328 -   무단 전재, 복제, 발췌. 디지털화금지


===== PAGE 322 =====
6부. 부록                                                                             3과. Kera$ 모델 생성. 저장 및 복원


                                                                                                   임베디드 전문가 그룹 윌텍


  Q Sequential model
     Model: "Sequential_Model '

         Layer (type)                                             Output Shape                        Param #

         flatten (natten)                                         .,        764)

         dense (Dense)                                               (   …, 128)                       無｝夕1乙 1

         dense_i (Dense)                                             (    } 10)                         1 ㅓ카日

       Total par． 驪s= 101,770 (397.54 KB)
       Trainable paras: U31,77C (397. 54 KB)
     ` N041-trainable par체.; 0     00            (9.    므；
                                                         》
  密Subdass model                                       /1仕안. 한 겆口！나厄                ㅅ，)7 j
     Model: 'subclass_Model"                                 -
                                                                                             A4   - " I i- ' 【?
         Layer                                                   - Output Shape                       Para. #

                                                                 -
                  (type)
         flatten 2                                                   》                            0 (unbuilt)

                                                                 ㅣ
                                     (Flatten)
                  4                                                  2                            0 (unbuilt)

                                                                 -
         dense_            (Dense)
         dense_   S        (Dense)
                                                                 - 2                               3 (unbuHt)

      Total params: r, (0.00 B)
      Trainable params:    他.00 B)
      Non-trainable paramst n ( (L00 B)




＠임베디드 전문가 그룹 윌텍                                                  - 329 -           무단 전재. 복제. 발췌. 디지털화금지


===== PAGE 323 =====
6부. 부록                                  3과. Keras모델 생성. 저장 및 복원


 모델의 저장과 복원                                        CODEXPE
                                                   임베디드 전문가 그룹 윌텍


  Q 학습 도중이나 학습이 끝난 후에 모델을 저장할 수 있음
   . 학습 도중 정기적으로 모델을 저장하는 경우
    /' 문제가 발생하여 작업이 중단되더라도 저장된 모델을 불러와 그 부분부터 다시 시작 가능함
    4. 최종 결과 대신 더 좋은 중간 결과를 선택해서 사용 가능
   . 저장된 모델을 다른 사람들과 공유할 수 있음
    '' 공유 받은 코드를 활용해 모델의 정확도를 향상시켜 더 좋은 모델로 발전시킬 수 있음
  ㅎ 모델 저장 시 저장할 대상
 下모델의학습된paramete：츠
  `,. 모델의 학습된 paramete"   모델을 만드는




C）
 임베디드 전문가 그룹 윌텍              - 330 -   무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 324 =====
6부. 부록                                          3과. Keras -델 생성. 저장 및 복원


 모델의 저장과복원 구현 _______________
            （1).---－…－ I IE   CODEXP,ERT
                                   7FI
  @［예제 4] MNIST 3단 Cony 모델을 기준으로 저장과 복원 방법을 이해하라
   0 저장경로 설정 今 모델을 저장하고 복원할 때 필요




   口 모델 정의 + 동일 모델을 여러 개 생성하므로 함수로 구현하였음
    def create-model():
      model = tf.keras.models.Sequential()



      model. compil이optimizer= ' adam' ,
                    loss= ' sparse..catego央cal_crossentropy ' ,
                    metrics= t accuracy 』'




         4A\J너닐은 P卜씨 학幻기 ' 綸




@）임베디드 전문가 그룹 윌텍                     - 331 -   무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 325 =====
6부. 부록                                                3과. Keras 모델 생성. 저장 및 복원


 모델의 저장과 복원 구현                                                    CODEXPERT
             （2)                                                  임베디드 전문가 그룝 욀텍


   . 모델 생성
    ;mo4el = createt
                  iTaode].( )
    - moaei.. summary` J

     Layer (type)               Output Shape           Param $/

     conv2d (Conv2D)            (None, 28, 28, 32)     320

     dropout (Dropout)          (None, 28, 28, 32)     0



     flatten (Flatten)          (None, 576)            0

     dense (Dense)              (None, 10)             5770

     Tot히 params: 비. 히4
     Trmnable params: 미. 히4
     llon-trainable params: U




＠임베디드 전문가 그룹 윌텍                          - 332 -     무단 전재, 복제, 발췌. 디지털화 금지


===== PAGE 326 =====
6부. 부록                                                                         3과. Keras모델 생성. 저강 및 복원


  모델의 저장과 복원 구현
              （3)                                                                               CODExPERT
                                                                                                임볘디드 전뿐가 그爵 윌텍


   . 학습하는 동안 체크포인트 파일 저장하기 今 Keras 2.xx
     r小 체크포인트 파일 이름 지정
    checkpoint_path = save_dir + " cp-{epoch:04아 . ck財"

    〃 체크포인트 콜백 만들기 +save_weights_only가 True이면 weight만 저장．
                                                        .False이면
      모델 전체를 저장 + 디폴트든한 epoch마다 저장，   . 옵션을 사용하여 저장 간격 설정 가능

    -cp_callback, ptf.
         checkp。   ath, save_
                   int_   = callbacks6
                              keras  。nly=
                                      .   weights_   ModelCheckpoint   True,      verb。
                                                                                      se
                                                                                      (    =D
    tl.학습* 학습시cp_callback을넘겨줌                        ￥u祭은 hTㄳ＄包 A죌，.
     history = model.fit (train_data, train_labels, shuffle=True,
                      batch_size=100, epodis=1이                    .   .
                    ,vi ii,r1ati on data= ." , , -' ,' , ,. test_labels;,
                      ca.L.LoacK5 = cp_ca.LLDaCKj)
     Ep。ch 00010: saying ifi。
                            d들f긺 /content/dr i ye/Mv Drive규iI es/save/c。 -00I 0. ckDt
     600/600 [--------------------------------I - 4s 7rHs/steP -valjoss: 00535 - val_accuracy: 0,9925




@）임베디드 전문가 그룹 윌텍                              - 333 -                  무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 327 =====
6부. 부록                                                                                                                     3과. Kera＄모델 생성. 저장 및복원


 모델의저장과복원구현
          （4)                                                                                                                                                    엑므),EE1XP
                                                                                                                                                                         7f:i트ER,
                                                                                                                                                                               'r
   〃 저장된 체크포인트 파일 확인＋ '../files/save/' 확인：한 세트는 여러 개의 파일로 구성됨
      x cp-0001.ckpt부터 cp-0010.ckpt까지 10개의 세트 생성됨
      ·   cp-0001 ckp1.data-OOOO0of-00002


      n   cp-OO01.ckp(.dta-OOO01-of-OOO02                                                 4- ; cp-0001.ckpt세트에해당하는파일들

      h   cP000Lckpt.indez


   ＇수 새 모델 만들기 * 학습 전이므로 성능은 당연히 낮음
    new_model = create7rnodel().                                                                             , , , , , .
    new_moaei . evaiuate(test_oata,                                                                          test_iaoeis J
     313/313 1- -   -   -   -   -   --   -   -   -   -   -   --   -   -   -
                                                                              -
                                                                                  -   -
                                                                                          -
                                                                                              --
                                                                                                   -]    -   is
                                                                                                                  2ms/
                                                                                                                         step   -   loss:   2.   3018   -   [
                                                                                                                                                                accuracy:   0,   i080｛   「




     [2. 3017983435584473. 0. m80000028미4183]

   〃 체크포인트 파일 적용 + cp-0008.ckpt 세트퓰 적용 * 저장했던 당시 성능이 그대로 나옴
    new_model. load_wei9hts(save_dir. + ,' cp-@008.ckpt')
    new_moaei . evaiuateijest_aata, test_ianeis'
    313/313 [---------------------.----.--=1 - is 2rns/step - loss: 0. 0558 -[accuracy: 0.9948I
    [0.05579540715314315. 0. 99479997158050541




C）
 임베디드 전문가 그룹 윌텍                                                                                         - 334 -          무단 전재. 복제. 발췌, 디지털화 금지


===== PAGE 328 =====
6부. 부록                                                        3과. Keras 모델 생성. 저장 및 복원


 모델의 저장과 복원 구현
             （5)                                                                                  CODEXPERT
                                                                                                  입버l디드 전문가 그룹 윌텍

   . 현재 상태를 체크포인트 파일로 저장하기
    ＇小 현재 상             ht릍 cp-curr.ckpt 세트에 저장
     mode    save_wei坐心(save_dir + ' cp-curr.ckpt' 》
    '' 새 모델 만듈기 * 학습 전이므로 성능은 당연히 낮음
     new_mode쟁 = create7rnodeln
     new_moaei.evaiuateitest_aata,
                                                           . , .,
                                                  test_labelsj

     313/313 [-------------------------------] - is 2ms/step - loss: 2,3049 -laccuracy: fljj
                                                                                              b                 1
     [2, 3048951625823975. 에0299997031698691

    'I. 쳬크포인트 파일 적：용            cp-curr.ckpt 세트를 적용 * 저장했던 당시 성눙이 그대로 나옴
     new_mo巾, .load_wei·hts(save_dir. + .' cp-curr.ckpt ' )
     new_moaei.ev, ua ' " st_aata, test_labelsJ

     313/313.[-------------------------------1 is
                                              -     2ms/   ster   -   loss:   0.   0534   -   accuracy:   0.   9925
     [。. 。5344429984688759, 9925。
                           。.      。。。715255741                                                                     -




@）임베디드 전문가 그룹 윌텍                            - 335 -         무단 전재, 복제, 발췌. 디지털화 금지


===== PAGE 329 =====
6부. 부록                                                 3과. Keras모델 생성. 저장 및복원


 모델의 저장과 복원 구현
             （6)                                                            CODEXPERT
                                                                            임베디드 전문가 그룹 윌텍


   . 모델ㅍ적철트저장하긴．
               :
   〃 모넬 섣쳇들 HDF5 포맷으로 저상                           " L:er心 " 궝장
    -model.save(save_dir + ' my. .model.h5')

    /' 저장된 모델을 로드하여 새로운 모델 생성 * 이미 학습된 상태로 로드됨 + summary를
       통해 저장된 모델과 동일한 구조임을 알 수 .
    new_mo력야 = tf·keras1models load_model save_dir + ' my_model.h5 ' )
    new_moaei , summary. '


    d' 저장했던 당시 성능이 그대로 나옴

    new: model. evaluate(tes견雙르 ,jst_ labe].s)
    313/313 [-----------------------------=I - is 2ms/steo - loss: 00534 -laccuracy: 099251
    [ft 05344429984688759. 0.99250000715255741




@）임베디드 전문가 그룹 윌텍                         - 336 -     무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 330 =====
6부. 부록                                       3과. Keras 모델 생성. 저장 및 복원



                                                          임베디드 전문가 그풉윌텍


  @ Weight 저장
   ·HDF5 format 으로 저장 -* .weights.h5
   ●.ckpt 지원 하지 않음
     checkpoint_path = save_dir + "cp-{epoch:04d}.weights.h5"


  @ Model 저장
   ..keras format우선 지원
    〃 .h5 (HDF5) -* .kera｀로변경추천     (2JD넥Z궉 匕ev口｀ 갛시 )
     ,1 tf format 은 지원하지 않음
   G Calibaci《 시 -* .keras format 만 지원




＠임베디드 전문가 그룹 윌텍                    - 337 -   무단 전재. 복제, 발췌. 디지털화 금지


===== PAGE 331 =====
6부. 부록                                    4과. Matplot 라이브러리




              124. Numpy 라햐雙2.j2J
              2과. Tensorfiow 프黨，J.래J 기，
                                      塾，
              324 Keras 2델 'i성, ;kl장 0-I 복蠶
              4과. Mat이ot 라이브러리




@）임베디드 전문가 그룹 윌텍        - 338 -   무단 전재, 복제. 발췌, 디지털화 금지


===== PAGE 332 =====
6부. 부록                                                     4과. Matplot 라이브러리


  Mat이otlib의 개요                                                 CODEAPERT
                                                                덛］베디드 전문가 그룝 윌텍


  @ Ma倒otlib는 』아in D. Hunter가 개발한그래프 그리기 라이브러리이다
   ' MATLAB처럼 동작하도록 하는 함수들의 모임이다
   .Py卄lon에 적당한 그래프 그리기 패키지가 없어 2003년에 직접 개발
   .Mat이otlib이 설치 되지 않았다면 다음 명령으로 설치한다
    4' pip install matplotlib
   ' matplotlib.pyplot
   Q matplotlib의 state-based interface이며. MATLAB과 같은 그리기 방법 제공
    /' 함수호출을 통해 다양한 상태가 유지됨 + 이를 통해 그림 그릴 객체.영역 그리기 방법 결정
   臼 자동으로 figure와 axis를 생성하므로 간단하게 정의된 이ot을 얻을 수 있다
   . 일반적으로 import mat이otlib.pypot as 이t 구문으로 import한다
  ｛多’ 본 과정에서는 기본적인 그래프 그리기에 대해 다룬다
   曄 자세한 내용은 아래의 링크에서 학습할 수 있다
    4. matplotlib tutorial
    4- https://matplotlib.org/tutorials/index.html




@）임베디드 전문가 그룹 윌텍                         - 339 -     무단 전재, 복제. 발췌. 디지털화 금지


===== PAGE 333 =====
6부. 부록                                           4과. Matplot 라이브러리


 그래프의 구성요소                                            CODEXPERT
                                                      임베디드 전문가 그룹 윌텍


  @Mat이ottib에서 그려지는 그래프의 기본 구성은 다음과 같다
        pyplot얘서 기본으로
        axes로 만드는 객체
       （기본으로 그래프 그릴 영역）




  모長이at e'ement의 최상위 container
 （그래프 그릴 도화지）


   axis, tick, Line2D, text등의
   그림요소가 대부분 포항된 좌표 겨i
  （도화지에 있는 그래프 그랄 영역）




@）임베디드 전문가 그룹 윌텍                 - 340 -   무단 전재, 복제, 발췌, 디지털화 금지


===== PAGE 334 =====
6부. 부록                                                                                       4과. Matplot 라이브러리

弓芦＼          ……1 ……… ……                                                 …                             성／發每쯔∼亨建和섭i奠醬
                                                                                                     璜；

    ,   '…          m-   ·                                                                       柄    임베디드전문가그驪윌텍


        @ y대 x를 선 또는 marker로 표시하는 함수
             plot (*args, scalex = True, scaley= True, data=None, **kwargs)
             .y대x를선또는marker로표시
                             = arra叫Ike or scalar로 보통 1차원 배열 전달
             y. x            · 1개의 argument전달 시 x축은 0부터 y와동일한 길 값을 자동 생성
                             ~ 2차원 배열 전달 시 열을 data set으로 선택하여 그래프를 그린다
             Sc히ex           · 그래프의 보이는 한계를 데이터의 한계 값으로자동 스케일링 할지 여부
             Sc히ey           · True : 데이터의 한계 값 사용. F計se : 미사용
                                                             （0-1.0사이 표시）
.            .. .,           ~ format string으로 색이나 marker, line에 관련되어있음. 사이트 참조
             iimti
                                                marker][line][color]                     순서무관
l
                             -   fmt
                                       =   '[                               '의형태로입력．
             data            1 label의 이름

             fmt는순서에 상관없이 서로조합하여 'b', 'or', '-g', '--', '^k' 등의 형태로사용가능하다
             marker              '.'(point), 'o'(circle), 'v', 'A', '<', )', 's'(square), *, x, 4- , -, I' 등등
             line            ~ '-'(solid), '--'(dashed), '-.'(dash-dot), ':'(dotted)
             c이or            ~ 'b', 'g', 'r', 'x', 'm', 'y', 'k'(black), 'w'
                                                          (-
                                                /-
                                                 '   ,_        「   ',




    ＠임베디드 전문가 그룹 윌텍                                                     - 341 -        무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 335 =====
6부. 부록                                                                                                                                    4과. Mat이ot 라이브러리

                                                                                                                                                  c0DE d; PERT
 예제 5. 이ot함수                                                                                                                                      임베디드 전문가 그룹 윌텍


    Q 다음 프로그램을 통해 이ot함수의 사용을 이해하라

                                                                                두 걔의 그래프를 한 axes에 그린다
                                                                                《현쟤 그림 그릴 영역에 plot 두 번）
  p t.出ow
  #
           乞蠟L比乞3‘있十…‘_ x, y좌표에그림
         [21
  야t.piOt
        （珏깅．
  pit.sliowu
  # 131
  p].t.plot([0.1, 0.2, 0.3, 41,[0.2, 0.3, 2.0, 0.91) ,    ,     ,       , ,
  pit,plot나0.1, 0.2, 0.乞 4],10.2, 0.3, 2.0, 0.9], scalexFalsLscaiy,== False.)
  pit.
                          ()
               show
  pit.plot([
                                                                                                                    maker만 주면 선은 그리자않응
  #141
         t ([
                                                      ,   [1,
                                  1,   2,   3,   4]             5,   3,
  pit.pl。                         1,   2,   3,   4]   ,   [t,   5,
                                                                     3,   9)
                                                                          91,
                                                                                ,   - '   。
                                                                                          r       ')
  pit.showu                                                                                                             2차원 배열은 열읊 data set으로 취급
  #151                .   .   .   ,               ,   ,              ,      .             .   .   .    .
                                                                                                           .    "   '
                                                                                                                                               로 3개의 그래프
                                                                                                                        [1,5,9], [2,4,3],L3.7,5］
  마t.plotHUzdJJ.Ld｀
                  끄고2‘乞j끄尸
  야t.snowU                                 . plotfll,41,[2,8]).,의 형태로 4개의 그래프
  #1 1                                   "

                                                -.3,2]1, 'ro-')
  plt.plot([[1,8,3,6], [4jL8,311J[[2,4,5,21,[8J9,
  pit.帥lowU




                                                                                                                                                                   I
＠임베디드 전문가 그룹 윌텍                                                                                                - 342 -        무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 336 =====
6부. 부록                                                                                                           4과. Matplot 라이브러리


 예제 5. title, label, legend                                                                                             CODExPERT
                                                                                                                        얌베디드 전문가 그醫 윌텍


  e 다음 프로그램을 통해 이ot함수의 사용법을 이해하라

  pit.piot([
  plt.pl。t ([
                   "Moon
                   "M。             。n ",
                                          ",
                                               "Song

                                               "S。
                                                       ng
                                                             ",


                                                             ",
                                                                      "Lew


                                                                      "Lew
                                                                             "l,
                                                                             "J,
                                                                                   I
                                                                                   80,70,
                                                                                   75,1。   )1)
                                                                                        。,8。
                                                                                            9,
                                                                                                 5)
                                                                                                           legend는 그래프 그린 순서에l 따랴 배정


  pit.titie (       '
                                     n_
   Dit.     (
          xiabei     )p'   'Name                       ='}        -
  pit.yiabei( ' Score')..                                                                             "
  pit.iegend( F "Kor", '
                       「Eng니，
                            》．
  아t . snows 〕               '

  이 개념이 $tate-based 이다
  이othng 하고
  title 만들고
  label 만들고
  legend 만들고
  show




＠임베디드 전문가 그룹 윌텍                                                                        - 343 -            무단 전재. 복제. 발췌. 디지털화 금지


===== PAGE 337 =====
6부. 부록                                                                                     4과. Mat이ot 라이브러리
                                                                                            느臂차



                                                                                                  CODEXPERT
 예제 5. sub이ot                                                                                     임베디드 전푼가 그흡 윌텍


  （身 다음 프로그램을 통해 sub이ot함수의 사용을 이해하라
   name.
          ==   [;Moon;               ,
                                            "Song
                                                    '   ,   "Lew


   sc。
     re    =             [8。   ,7。   ,951
                                                                   ''J


                                                                          인치단위 크기를 출수 있읗
   plt.figure(figsize=(12, 4) )--                                         기본 6.4. 4.8
   아t. SuD910t11,5,1) .
   아t.Dar(narne, 뜨oreJ
   아t. suDplotU , 5.刃      .
   아t.scat!er1na쁘e, . score)
   아t.suDp홍OtU,3,Z) .                                                     1행 3열 중 2번 인덱스
   p1t.p1ot`name, score)

                                                                         ----
   x = np.linspace(0, 2, ieo) .

   具g, ax .=.뺙.subp존ots(2, 3, f1gsize=(16, 9))
   I핀·suptir1e. test,',
   ror iux1 in八
             II-. . ,
                 rdnge쵸o).
                      。-.l . ..., !i,.i . fit! C   .I! .I
     ax[].ux;I5, 뀌x下킥·settitie ( iux . ' 'LI ·rormat`1ox;)
     ax[iaxiii, iax名3j.p1ot`x, x**1ax)




＠임베디드 전문가 그룹 윌텍                                                           - 344 -   무단 전재. 복제, 발췌, 디지털화 금지


===== PAGE 339 =====
S
