---
source_url: "/run/media/yutae/Data/엣지있게 설명한 텐서플로우.pdf"
ingested: 2026-11-15
sha256: f9aa2e7b044c22ec3848cb90802cbe657da7b5e63864b7c599ac38c24108a9bc
type: raw-source
method: text-extract
---

# 엣지있게 설명한 텐서플로우 (raw source)

> **출처:** USB 원본 PDF (`/run/media/yutae/Data/엣지있게 설명한 텐서플로우.pdf`, 로컬 참고용 — git commit 불포함)
> **방법:** 내장 텍스트 레이어에서 `pdftotext -layout`로 추출 (OCR 불필요)
> **쪽수:** 300쪽 | **추출 텍스트:** 533 KB
> **주의:** 원고는 scan/레이어 추출로 영문·숫자·특수자 일부 아티팩트가 있을 수 있음. 해석 시 원본 PDF와 대조.
> OCR 추출 디렉터리 `raw/books/tensorflow-explained.ocr/`는 git-ignored (로컬 참고용만) — 본문은 아래에 내장.

## Book metadata
- **Title:** 엣지있게 설명한 텐서플로우
- **Pages (PDF):** 300
- **Source:** 엣지있게 설명한 텐서플로우.pdf
- **Domain:** Programming · 프로그래밍 (예상)
- **Ingested:** 2026-11-15

## Extracted text (all 300 pages)


===== PAGE 1 =====
                 TENSORFLOW
             FOR MACHINE INTELLIGENCE

                엣지있게 설명한




    戶／   /

今




                            Sam Abrahams ' Danijar Hafner
                               Erik Erwitt ' Ariel Scarpinelli 공저
                                                    정기철       역


===== PAGE 2 =====
             TENSORFLOW
         FOR MACHINE INTELLIGENCE

            엣지있게 설명한




    戶／
9




                        Sam Abrahams ' Danijar Hafner
                           Erik Erwitt ' Ariel Scarpinelli 공저
                                                정기철       역


===== PAGE 3 =====
TENSORFLOW
 FOR MACHINE INThLLIGENCE

                             by Sam Abrahams· Danijar Hafner ' Erik Erwitt ' Mel Scarpinelli




Copyright @)2016 Bleeding Edge Press.


All Rights Reserved.


First published in the English language under the title "TensorFiow for Machine Intelligence" By
: Sam Abrabams, Dat펴ar Haftner, Erik Erwitt, Mel Scarpinelli by Bleeding Edge 'Press, an
imprint of Backstop Media.

KOREAN language edition published by, Copyright @) 2017 Hongreung Science Publishing
Company

The Korean edition was published by arrangement with Bleeding Edge Press, an imprint of
Backstop Media LLC, Santa Rosa through Agency-One, Seoul.




    이 책의 한국어판 저작권은 에이전시 원을 통해 저작권자의 독점 계약으로 홍룽
    과학출판사에 있습니다. 저작권법에 의해 한국 내에서 보호를 받는 저작물이므로
    무단전재와 무단복제를 금합니다．


===== PAGE 4 =====
환영합니다

텐서플로우TensorEtow는 2015년 11월에 오픈 소스로 공개된 이후에, 현재 사용할 수 있

는 가장흥미로운 머신 러닝machine Learning 라이브러리 중의 하나로써，
                                            연구， 교육
                                              개발，

분야에서 점점 더 많이 사용되고 있으며, 계속적으로 업그레이드, 추가, 최적화되면서
                          텐서플로우를 이용한 딥러닝Deep
텐서플로우 커뮤니티는 빠른 속도로 성장하고 있다．
                          초보자나숙련자들이 텐서플로우로 각자의능력을향상시키
Learning with Tensorflow으로，
고, 이막강한라이브러리를 최대한 이용할수 있게 되기를바란다.



이 책의 구조

섹션 1: 텐서플로우 API, 기초, 실습

이 첫 번째 섹션은 " 텐서플로우 기초" 로 시작하는데, 자신의 컴퓨터어］텐서플로우를 설

치한후,많은머신 러닝machine learning의 개념들 없이 텐서플로우API의 기본을살펴본
다. 이 섹션의 목표는 " 텐서플로우 공부"와 " 텐서플로우를 이용한 머신 러닝 수행 방법
공부" 를분리하는 것으로써, 이 섹션에서는텐서플로우 API의 가장중요한부분들을 깊
이살펴볼 것이다．

핵심 API 개념을 배운 후에, 텐서플로우에서 제공되는 선형 회귀 분적linear regression,

로지스틱 회귀분적〔ogistic regression, 클러스터링clustering과 같은 간단한 머신 러닝 모델
을 만듦으로써 " 머신 러닝 기초"를 다룬다. 또한 각 머신 러닝 모델을 어떻게 시각적인
그래프 표현으로만드는 지를 배우고, 그것을 텐서플로우 코드로 변환하는방법과텐서


===== PAGE 5 =====
         보드TensorBoard를통해서 우리의 그래프가 정확하게 모델링되었음을 검증한다．

              " 실습" 에서 한걸음 뒤로 물러나서 좋은 구현습관에 대해서 논의할 것이다．
         마지막으로，
         여기에서는코드를적절하게 조직하는 법, 프로젝트구성법，
                                     파이썬Python 언어의 특성
         들을 효과적으로 사용하는 법, 그리고 부가적인 텐서플로우의 특성들을 최대한 이용하
         는법을다룬다．


         섹션 2: 텐서플로우로 고급 딥 모델
                            （deep models）
                                        을 구현하는 법

         이 두 번째 섹션은 3개의 장으로 구성되는데, 각장은 각각다른 복잡한 딥 러닝 모델에
         집중한다. 각장는 해당하는모델을설명하고, 우리가 만들려고 하는모델의 시각적 그
         래프 표현을 먼저 소개한다. 각 모델이 왜 그런 식으로 구성되는지 살펴보고, 수학적인
         표현, 그리고 텐서플로우로 효과적으로구성하는 법을살펴본다．

         우리가 살펴볼 첫 번째 모델은 물체 인식과분류object recognition and classification에서의
         컨볼루셔널 신경망convolutional neural network: CNN인데，이미지 데이테mage data로 텐서
         플로우 모델을 학습하는 법을 다룬다. 수학적인 내용, 컨볼루션convolution 연산의 목적，

         원래의 이미지 데이터「aw image data를 텐서플로우에서 사용할수 있는 형태로 변환하는
         방법, 최종적인 결과물을테스트하는방법을포함한다.

         " 회귀 신경망과 자연 언어
                       （Recurrent Neural Networks and Natural Language)"
         장에서 텐서플로우를 이용하여 순환 신경망
                              「ecurrent neural network: RNN을 만드는 방법

         을살펴본다．
              다양한자연어 처리natural language processing: NLP 작업을 고려해서，
                                                                Long
                                   를활용하는 방법과사용하는 모델에 미리 학습된단
         Short-Term Memory(networks）
         어벡터word vectors들을 병합하는방법을살펴본다．




iv
     -


===== PAGE 6 =====
다른 머신 러닝 라이브러리들

텐서플로우가유일한오픈소스 머신 러닝 라이브러리는 아니다. 아래에 딥러닝을 위한
다양한 라이브러리들을 간단하게 정리하였다．

 · Caffee는c+＋로작성된 컨볼루션 신경망과 영상처라mage processing에 집중

      한다．
 . Chainer는 하나의 컴퓨터에서 여러 개의 GPU를활용할수 있는유연한flexible
      Python 기반머신 러닝 라이브러리다．
 · CNTK는Microsoft의 머신 러닝 라이브러리 게임으로써 선언적declaratively으로
      분산모델을만들수 있는고유의모델정의 언어modeldefinition language를사용한다．
 · Deeplearning4j는신경망에특화된자바기반라이브러이다．
                                   Spark, Hadoop,
      그리고다른자바 기반의 분산소프트웨어와 결합되어서 활용될수 있다．
 . Nervana Neon은하나의 컴퓨터에서 여러 개의 GPU를사용할수 있는Python
      기반의 머신 러닝 라이브러리이다.
 .    Theano는아주유연한Python머신 러닝 라이브러리로써 Python으로작성되
      었다. 복잡한 모델을 아주 쉽게 정의할 수 있고, 사용자 친화적인 특성으로 인하
      여 연구에 많이 사용된다. 텐서플로우시？I는ㄲieano와아주 비슷하다．
  .   Torch는Lua로 작성된 GPU상의 구현에 집중한 머신 러닝 라이브러리로써 여
      러 대형 회사에서 지원을받고 있다．


이러한모든라이브러리들의 장점을깊이 토론하는것은이 책의 범위를벗어나지만, 시
간이 있다면 각자 한번 살펴볼 필요가 있는 라이브러리들이다. 텐서플로우 제작자들은
자신의 프레임워크를디자인할때 이들로부터 많은 영감을 받았었다．




                                                            -


===== PAGE 7 =====
         필요한 기반 지식

         이 책은텐서플로우 API에 집중하는데, 이를 위해서 독자들이 미리 알았으면 하는수학
         과프로그래밍 관련 개념들을 아래에 정리하였다：

           ·   미분계수derivative calculus：단알－변수single-variable와다－변수multi-variable
           ·   행렬 연산
                   （특히 행렬의 곱）
           ·   프로그래밍 원리에 대한기본적 이해

          ·    머신 러닝 기본개념


         위의 사항에 더해서, 독자들이 다음의 지식이 있다면 이 책에서 더 많은 것을배울수 있
         을것이다：

          ·    Python언어와모듈module작성 경험

          ·    Numpy라이브러리 경험

          ·    matplothb라이브러리 경험
          ·    고급 머신 러닝 개념에 대한 지식, 특히 피드포워드 신경망feed-forward neural
               networks, 컨볼루션 신경망convolutional neural networks, 순환신경망
                                                                    「ecurrent neural
               networks에 대한 지식


         가능하다면 우리는 이 책에서도수학과Python에 대한 개념들의 이해에 필요한 내용들
         을독자들에게 제공할 것이다．


         이 책에서 공부할 내용들

         이 책을 읽은후에 당신은 아래의 사항을 알게 된다．

          ·    핵심 텐서플로우API의 깊은이해
          ·    텐서플로우워크플로우-workflow：그래프정의와그래프실행
          · 다양한기기에 텐서플로우설치 방법
          ·    각자의 코드와프로젝트를진행하는가장좋은실습




vi   I


===== PAGE 8 =====
  ·   텐서플로우로핵심적인머신러닝 모델을만드는방법
  · 텐서플로우로RNN, CNN을구현하는방법

  · 분산환경에서 컴퓨터들을연결하는방법
  · 텐서플로우서빙으로코드를활용하는방법
  · 텐서보드를최대한활용하는핵심 원리


이 책을본후에 텐서플로우를 더 깊이 공부하고 싶다면 아래의 자료들을참고하자．

  .   The official TensorFiow website: 최신의문서, 시〕
                                               I , 튜토리얼이 있다．
  .   The TensorFiow GitHub repository: 텐서플로우오픈 소스 구현에 기여할수
      있고다른 소스 코드들을살펴볼수 있다．
  · 텐서플로우로 구현된 공식적으로 공개된 머신 러닝 모델듈：이러한모델들을그

      대로 사용하거나자신의 목적에맞게 수정해서 사용할수 있다．
  ·   The Goo이e Research테og：텐서플로우응용프로그램과수정사항관련구글
      의 최신소식을 접할수 있다．

  ·   Kag이e: 공개된 데이터셋을 찾고 이를 이용한다른 사람들과의 성능 비교를 할

      수 있다．
  ·   Data.gov: 미국 전역의 공개 데이터셋을찾을수 있는미국 정부의 포탈사이트


이제 텐서플로우를 이용한 인공 지능TensorFtow for Machine InteLligence어I 대해서 시작
해보자！


===== PAGE 9 =====
대apter 1    텐서플로우 설치하기                                    1
            설치 환경 선택하기                                     2
            Jupyter NotebookZ Matplotlib                   4
            Virtualenv 환경 생성                              6
            간단한 텐서플로우 설치                                   7
            소스를 사용한 설치 예： 64－비트 ㅃuntu Linux with GPU 지원    9
            의존성 설치                                         9
            Bazel 설치                                      9
               CUDA 소프트웨어 설치
                           （NVIDIA CUDA CPU만 가능）          12
               텐서플로우를 소스 코드로부터 빌드해서 설치하기                  15

            Jupyter Notebook 설치하기                         17
            matplotlib 설치하기                               18
            텐서플로우, Jupyter Notebo아〔, matplotlib 테스트하기     19
            결론                                            23



Chapter 2   서론                                            25

            모든 곳에서 넘쳐나는 데이터                               26
               （deep learning)
            딥 러닝                                          26


===== PAGE 10 =====
            TensorFlow: 최신의 머신 러닝 라이브러리        28
            텐서플로우：기술적인 개괄                      28
              구글의 딥러닝 관련 간단한 역사                28
            텐서플로우란 무엇인가？                       29
              한 문장으로 이해하기                      29
              조금 더 자세한 설명                      32
            텐서플로우는 이런 경우에 사용하자                 34
            텐서플로우의 강점                          35
              사용성
                （usability)                    35
              유연성
                （flexibility)                  35
              효율성
                （efficiency)                   35
              지원
               （support)                       36
              기타 특징들                           36
            텐서플로우를 사용할 때 어려운 점                 36
              분산 지원은 아직 진행형                    36
            앞으로 그리고 위로！                        37



Chapter 3   텐서플로우 기본                           39

            계산 그래프
                 （computation graph) 소개        40
              그래프 기본                           40
              의존성
                （Dependencies)                 45
            텐서플로우에서 계산 그래프 정의하기                49
              첫 번째 텐서플로우 그래프 만들기               50
              텐서가 무엇일까？                        59
              파애선 기본 자료형
                       （Python native types)   60
              NumPy 배열                         63
              텐서 모양
                  （Tensor shape)               64
              텐서플로우 오퍼레이션                      66
              텐서플로우 그래프                        70


===== PAGE 11 =====
              FETCHES                                           74
              FEED 딕셔너리
                      （dictionary)                              75
              플레이스홀더로 입력 사용하기                                   77
              변수                                                79
            그래프를 name scope로 구성하기                               84
              그래프 만들기                                           93
              그래프 실행                                            97

            결론                                                 104



Chapter 4   머신 러닝 기초                                           105

               （Supervised Learning) 기초
            지도학습                                               106
            학습 체크포인트 저장하기                                      109
                （Linear Regression)
            선형 회귀                                              111
                  （Logistic Regression)
            로지스틱 회귀                                            115
            소프트맥ㅅ 분류
                   （Softmax Classification)                    122
                 （Multi-Layer Neural Networks)
            다층 신경망                                             127
            기울기 하강법과 역전파
                       （Gradient Descent and Backpr아〕
                                                    agation) 132



Chapter 5   실습                                                 141

            코드 구조와 유틸리티 함수들                                    142
              LAZY PROPERTY DECORATOR                          142
              DOWNLOAD FUNCTION                                142
              DISK CACHING DECORATOR                           143
              속성 사전
                  （Attribute Dictiona이                         146
              그래프 데코레이터 덮어 쓰기                                  147



아iapter 6            （0bject Recognition and Classification)
            물체 인식 및 분류                                         151

                   （Convolutional Neural Networks)
            컨볼루션 신경망                                           154


===== PAGE 12 =====
   （Convolution)
컨볼루션                            158
  입력과 커널(Input and Kernel)      159
  스트라이드
      （Strides, 큰 걸음 걷기）        161
  패딩
   （Padding)                    164

  데이터 형식                        165
  KERNELS IN DEPTH              165
Common Layers                   169
  컨볼루션 레이어                      170
  활성화 함수
       （activation functions)   171
  POOUNG LAYER                  174
    （normalization)
  정규화                           178
                （고차원 레이어）
  네gh Level Layers              179
  냐＼YER INPUT                   182

이미지와 텐서플로우                      182
  이미지 로딩                        183

  이미지 형식                        184

  JPEG와 PNG                     185
   TFRECORD                     186
  이미지 조작                        190
   CROPI긔NG                     191
   PADDING                      192
   FUF긔：DING                    194
    （Saturation）
   채도             （Balance)
               과 균형             196

   색상                           198
   GRAYSCALE                    198
   HSV                          199

   RGB                          200

   LAB                          200
   이미지 값의 변경                    200

CNN 구현                          201


===== PAGE 13 =====
               Stanford Dogs 데이터셋                              202
               이미지를 TFRecords로 변환하기                            202
               이미지 불러오기                                        207
               모델                                              208
               학습                                              212
               텐서보드로 필터 디버깅하기                                  213

            계속 진행                                              215



Chapter 7   회귀 신경망과 자연 언어
            (Recurrent Neural Networks and Natural Language)   217

            회귀 신경망 소개                                          218
               우리는 시간적인 세계에 살고 있다．                             218
               임의의 프로그램을 학습하기                                  219
               시간에 따른 역전파
                        （Backpropagation)                      221
               우리의 첫 번째 순환 신경망 만들기                             222
               사라지거나 폭발하는 기울기                                  224
               Long-Short Term Memory                          226
               구조에 변화를 주자                                      228
               다중 순환 레이어                                       229

            단어 벡터 임베딩                                          230
               Wikipedia 말뭉치 준비하기                              232
               모델 구조                                           238
               NOISE CONTRASTIVE CLASSIFIER                    239
               모델 학습하기                                         240
            시퀀스 분류                                             241
               Imdb Movie 비평 데이터셋                              242
               단어 임베딩 사용하기                                     243
               시퀀스 레이블링 모델                                     244
               냐＼ST RELEVANT ACTIVATION에서 소프트맥스                246


===== PAGE 14 =====
                     （gradient clipping)
               기울기 자르기                                       248
               모델 학습                                         249

            시퀀스 레이블링                                         251
                      （optical character recognition) 데이터셋
               광학 문자 인식                                      252
               타임 스텝 사이에서 공유되는 소프ㅌ맥ㅅ                         254

               모델을 학습시키기                                     259

               양 방향 RNNs(Bidirectional RNNs)                 261

            Predictive Coding                                265
               문자 단위 언어 모델링                                  266

               ArXiv 초록 Api                                  266
                     （Preprocessing the Data)
               데이터 전처리                                       270

               Predictive Coding Model                       271

               모델 학습하기                                       277

               유사한 시퀀스를 생성하기                                 281



Chapter 8   실제 사용하기                                          285

            학습된 모델                                           286


===== PAGE 15 =====
텐서플로우 설치하기




堺橡枉(
 。#므斗示뿌* 。 ／V,'- ,1。


===== PAGE 16 =====
                                  다행스럽게됴 공식적인 텐
    텐서플로우를 사용하기 전에 이를 컴퓨터에 설치해야 한다．
    서플로우 웹사이트에 Linux와Max OS X 컴퓨터 상에서의 완벽한단계별 설치 방법이
    있다. 이 장은 설치할 때의 다양한 옵션들 중에서 추천 사항을 설명하고, 텐서플로우와
    잘 맞는 써드．                               또한CPU를 이용한
           파티third-party 소프트웨어에 대한 정보도 제공한다．
    텐서플로우 설치를 위해서 소스 코드를 이용한 설치 방법도 제공한다．

                            소스 코드를 이용한 설치법 등에 익숙하다면，
    독자들중에 이미 Pip/Conda, 가상환경，
    아래의 공식적인 가이드 정보를 사용하는 것도 좋다．

         https://www.tensorfiow.org/versions/master/ge乙started/os_setup.html




    설치 환경 선택하기

    소프트웨어들은독립적으로 관리되는많은 라이브러리library와 패키지package들을사용

    한다. 이러한 방법들은 개발자들에게는 코드를 재사용할 수 있고, 이미 사용 가능한 코
    드들을다시 작성할 필요없이 새로운 기능들의구현에만 집중할수 있게 하기 때문에 편

    리하다. 그러나장점만 있는 것은 아니다. 하나의 프로그램이 정상적으로동작하기 위해
    서 다른 라이브러리에 의존한다면, 해당하는 라이브러리가 사전에 설치되어 있어야 한
    다. 이것을 쉽게 생각하면, 해당하는 소프트웨어를 설치하면 되는 간단한 문제인 것 같
    지만, 불행하게도 그렇지 않다. 이 문제는 원하지 않는 결과를 종종 초래하기도 하기 때

    문이다.

    다음과 같은 시나리오를 생각해보자. 당신이 멋진 소프트웨어 A를발견해서, 다운로드
    하고 설치했다．
           설치 스크립트script의 일부에서 소프트웨어 A가 지금 당신의 컴퓨터에
    설치되어 있지 않은다른 소프트웨어를 찾는다. 해당 소프트웨어가 설치되어 있지 않다
    면，
     그것을 설치한다．
             이러한 상황을 소프트웨어 의존성dependency이라고 하자．
                                              현재는
                                그래서 소프트웨어 A는1.0 버전을설치
    dependency 버전1.0이 필요하다고 가정하자．
    하고자신의 설치를종료한다. 현재까지는 모든 것이 정상이다．




CHAPTER 1 텐서플로우 설치하기


===== PAGE 17 =====
그런데 나중에 소프트웨어 B라는 다른 프로그램이 필요한데, 이 소프트웨어 B는 버전
2.0이 필요하다. 소프트웨어가 배포되는 방식 때문에 1.0과 2.0을 모두 사용할 수 없다．

둘다 설치되면 어느 버전을 사용해야 할지 모호하기 때문이다. 소프트웨어 B는 버전
2.0을 덮어 쓰고 자신의 설치를 종료한다. 그런데 소프트웨어 A가 버전 2.0과는 호환이

되지 않는다는 것을 알게 되었다. 문제가발생한 것이다．

어떻게 하면 하나의 컴퓨터에서 소프트웨어 A와 소프트웨어 B를 같이 사용할 수 있을
까？텐서플로우는 여러 오픈 소스를 사용하기 때문이 이것은 중요한 문제이다. 이러한
소프트웨어 의존성dependency 문제를 우회하는 몇 가지 방법이 Python
                                           （텐서플로우를
                 에 있다．
패키징packaging하는 언어）

  1. 코드싱K게서의 패키지package 의존성；시스템 레벨에서의 패키지나 라이브러리를
    사용하는 대신, 개발자들은 자신의 코드 내에 라이브러리의 정확한 버전을 포함
    하고 지역적으로Locally 참조
                     「eference할수 있다．
                                   이 방식은 소프트웨어가 필요로
    하는모든코드를사용할수 있고, 외부의 변화에 영향을받지 않는다. 그러나 이
    에 따른 단점도 있다. 첫 번째로, 이 방식의 소프트웨어를 설치하기 위한 디스크
    공간이 더 필요해진다. 이로 인해서 설치 시간이 길어지고 비용이 더들수 있다．
    두 번째로，
         사용자는 어깼든 전역적으로 소프트웨어의 의존성을 가진다. 로컬버
    전은중복이며 공간을 더 사용한다. 마지막으로, 소프트웨어 의존성이 심각한 보
    안 침해를 고치는 업데이트를 할수 없게 된다. 사용자가 패키지 관리자를 통해
    서 업데이트하는 대신 소프트웨어 개발자가 코드 기반으로 의존성을 업데이트
    해야하는데, 불행하게도 소프트웨어의 최종사용자는 별로할 일이 없고, 언제
    직접적으로 의존정을 포함할 지를 개발자가 결정하기 때문이다. 텐서플로우는
    각의존성을포함하지 않기 때문에, 각각별도로 설치되어야한다.

  2. 의존 관계 환경dependency environments 사용：몇몇 패키지 배포 관리 소프트웨어
    는 다른 환경과 상관없이 특정 버전의 소프트웨어를 사용할 수 있게 해주는 환
    경을 구성해주는 소프트웨어를 가지고 있다. 파이썬의 경우에 몇 가지 옵션이
    있다. 파이썬의 표준 배포에는 Virtualenv가 있다. Anaconda를 사용한다면



                                                   설치 환경 선택하기   -   3


===== PAGE 18 =====
        Vfrtua1env는 패키지 관리자인 Conda와함께 기본 환경으로 제공된다. 잠시 후
        에 이두 개를 사용해서 텐서플로우를 설치하는 법을살펴보자．

      3. 컨테이너containe「사용：Docker와같은 컨테이너는 소프트웨어의 실행 환경
        과 의존 관계를 포함해서 전체 파일 시스템을 포함하는 환경을 패키징하는 간
        편한 방법이다. 그렇기 때문에 컨테이너를 실행할 수 있는 어떤 컴퓨터
                                             （가상 머
        신 포함）
            라도 그 컨테이너를 실행하는 다른 컴퓨터와 동일하게 실행할 수 있다．
        Docker 컨테이너로 텐서플로우를 시작하는 것은 단순히 Virtualenv나 Conda
        환경을 실행하는 것보다 해야 할 일이 조금은 더 많다. 그러나 실행 환경 전체에
        서의 일관성consistency은 인스턴스를 여러 개 실행할 때 그 가치는 충분하다아
        상머신이든실제 물리적인 서버이든）
                         . 우리는Docker를설치하는방법, 텐서플
        로우 컨테이너를 만드는 방법
                      （공식적인 텐서플로우 이미지를 사용하는 방법 포
        함）
         들을아래에서 살펴볼 것이다．


    일반적으로，
         우리는 하나의 컴퓨터에 텐서플로우를 설치할 때는 Virtualenv나 Conda
    환경을사용하기를 권한다. 이 방법들은상대적으로 적은 오버헤드overhead로 의존성을
    해결할수 있는데, 설치하기 쉽고, 만든후에는 거의 생각할 필요가 없다. 그와달리, 텐
    서플로우 코드를 하나 이상의 서버에서 실행하려면, Docker 컨테이너 이미지를 생성하
    는 것이 좋다. 절차가조금더많지만많은 서버에 설치할때는충분히 가치가 있다. 우리
    는 환경environment이나 컨테이너containe를사용하지 않는 텐서플로우 설치는추천하고
    싶지는않다．




    Jupyter Notebook2I Matptottib

    데이터 사이언스 워크플로우data science workftow에서 최근에 통합된 두 개의 멋진 소프
                                       이 두 개의 소프트웨어들은 수년
    트웨어가바로Jupyter Notebook과matplotlib이다．
    동안Numpy와같이 사용되었으며，
                     Numpy와 텐서플로우가 밀접하게 연관되어 있어
    서 사용자들이 익숙한 작업 패턴을 그대로 활용할수 있도록 해준다. 이 둘다 오픈 소스



애APTER 1 텐서플로우 설치하기


===== PAGE 19 =====
이고 " permissive BSD라이선스"이다．

Jupyter Notebook
               （예전에는 iPython Notebook）
                                     은 사용자가 코드, 텍스트, 출력，
LaTeX, 그 외의 시각적 출력visualization을 포함하는 문서를 인터랙티브하게 작성할 수
있도록 해준다．
       이 소프트웨어는 차트chart에서 시각적인 결과 바로 옆에 코드를 붙임
으로써，
   실험분적 보고서를 작성할 때 놀랍도록 유용하다. 또한 특별한 연구 방법에 대

한당신의 통찰력insight을공유하기 위해서 RFlrichly formatted text를 제공하는 설명을포
함할 수 있다．
       또한Jupyter Notebook은 자신의 코드의 어디로든 되돌아가서 수정하
거나 바로 실행해볼 수 있기 때문에，
                   생각을 구체화idea prototyping할 때 환상적이다. 당
신의 코드를 한 줄씩 실행해야 하는 다른 인터랙티브한 파이썬 환경과 달리Jupyter

Notebook은 스크립트의 특정 부분을 디버깅하기 쉽도록 당신의 코드를 논리적인 덩
어리로 작성할 수 있도록 해준다．
                 보통의 텐서플로우 프로그램은 " 그래프 정의graph
definition" 와 " 그래프 실행graph running" 부분이 분리되어 있기 때문에 이 기능은상당히
유용하다．

Mat이otlib는 사용자가 파이썬으로 동적인 시각 출력 결과를 만드는 차트 라이브러

리charting Library로써，Numpy와 확실하게 결합된다．
                                    또한 작성된 그래프는 Jupyter
Notebook에서 바로 출력할수 있다．
                     Matplothb는 영상 인식 결과를 검증하거나 신경
망의 내부 요소를 시각화할 때 사용될 수 있는 숫자 데이터의 이미지 출력에도 사용될

수 있다．Seaborn과같은 ma如lotlib의 부가적인 레이어를사용해서 기능을확장할수
도 있다．




        ∼ 』.- - 一 . : ∼－ ,,.-,. . ., →－n n. - . , . . 一 .- - → -．」袋變蓼爵轟珊뺄饑蛋姆뿐攝舞씽
        딘므I들도뉴＝ 실지슬 ㅟ해시긍 ｀가匕＂느시 ㅌ눙／늬 ㅅ 비브놀 슨f,．므0rㅅr.

        httPs://www.tensortlow.org/versions!rO. 10/geLstarted/os-setuP.html#overview


        윈도우 운영체제를 사용하는 경우라면 Docker를 사용해보자．
        价tp:/!www.netinstructions.com/how-to-instal뇨7nd-run-tensomow-on-a-windows-pc!




                                                                         Jupyter Notebook과 Matplotlib   -   5


===== PAGE 20 =====
            VirtuaLenv 환경 생성

            소프트웨어 사이의 의존 관계를 멋지고 명확하게 유지하기 위해서, 가상 파이썬 환
            勘rtuat Python environment을 만들기 위해서 virtualenv를 사용할 것이다．먼저，
            virtualenv가pip            와같이 설치되었는지 확인하자· 자신의 운
                         （파이썬의 패키지 매니저）
            영체제에 따라서 다음의 명령어를 실행해보자：

             Linux 64-bit



             $ sudo apt-get install python-pip python-dev python-virtualenv
             # Pyth아구 3
             $ sudo apt-get install python3-pip python3-dev python3- virtualenv



             Mac OS X
             $ sudo easy_install pip
             $ sudo pip install - - upgrade virtualenv


            이제 나중에 사용할 환경뿐만아니라이 환경을 저장할 디렉터리를만들자．

             $ sudo mkdir -/env



            다음으로 virtualenv 명령어로 환경을 만들 것이다. 이 예제에서는 ∼/env/terisorflow
            폴더를사용한다．

             $ virtualenv --system-site-packages -/env/tensorf1ow


            환경을 생성한후에는 source 명령어로 그 환경을 실행할수 있다．

             $ source ` /env/tensorfiow/bin/activate
             # Notice that your prompt noLJ has α ' (tensorfiow夕 ' indicator
             (tensorflow)$




6   -   CHAPTER 1 텐서플로우 설치하기


===== PAGE 21 =====
pip로무엇인가를설치할때，
             그환경이 활성화active 상태인지를 체크해야한다．
                                        왜냐하
면 virtualenv가다양한 의존관계를추적하는방식과관련있기 때문이다．

환경을다사용한후에 deactivate 명령어로 종료할수 있다．

 (tensorflow)$ deactivate



가상환경을자주사용할경우에는, 전체 source.. . 명령어를 일일이 입력할필요없이
단축 명령어shortcut를 사용할 수 있다. 다음의 명령어는 ∼/.bachrc 파일에 bash alias를
추가한다. 이로써 환경을 시작하고 싶을때 마다tensorfiow를 입력하기만하면 된다．

 $ sudo printf ' \nalias tensorflow="source -/env/tensorflow/bin/
 activate" ' >> -./.bashrc


이것을테스트하려면bash 터미널을재 실행하고 tensorfiow를 입력하자：

 $ tensorfiow
 # The prompt shouLd change, α5 before
 (tensorf]ow)$




간단한 텐서플로우 설치

GPU에 상관없이 튜토리얼을 가능한빨리따라하고 싶다면, 텐서플로우의 공식 실행 파
                            이전 섹션에서 설명한Virtualenv 환경이 액티브한
일pre-buiLt binaries를 설치하면 된다．
지, 그리고 다음의 명령어를운영체제와파이썬 버전에 맞게 실행했는지 만을 체크하면
된다．




                                                              간단한 텐서플로우설치   -   7


===== PAGE 22 =====
Linux 64-bit installation

# Linux, Python 2.7
(tensorflow)$ pip install --upgrade
https:I/storage.googleapis.com/tensorflow/linux/cpu/tensorflow-0.9.0- cp27-none-linux_
x86 64.whl


# LtnUX 64-t)it' Python 3.4
(tensorflow)$ p1p3 install - -upgrade
https://storage.googleapis.com/tensorflow/linux/cpu/tensor-Flow-0.9.0-cp34-cp34m-
linux x86 64.whl


# LLnux 64-bLt, Python 크．5
(tensorfiow)$ p1p3 install --upgrade
https:I/ storage.googleapis.corn/tensor-flowllinux/cpu/tensorflow-0.9.0-cp35-cp35m-
linux x86 64.whl


Mac OS X installation

# 川αt 05 X』 Python 2. 7:
(tensorflow)$ pip install - -upgrade
https://storage.googleapis. com/tensorf]ow/mac/tensorflow-0.9.0-py2-none-any.whl


# Mac OS XJ Python 3. 4+
(tensorflow)$ pip3 install --upgrade
https : //storage.googleapis.corn/tensorflow/mac/tensorflow-0.9.0-py3-none-any.whl




                기술적으로, GPU를 지원하는 텐서플로우 실행 파일도 있다. 그러나 특정 버전의
                NVIDIA 소프트웨어가 필요하고, 향후 버전과는 호환되지 않는다．




  8   -   애APTER 1 텐서플로우 설치하기


===== PAGE 23 =====
소스를 사용한 설치 예： 64－비트 Ubuntu Linux with GPU 지원

CPU를 사용하고 싶다면 소스로부터 빌드buiLd하는 것이 좋다. 아래에 텐서플로우를

斗용하기 위해 필요한 모든 것을 한 단계씩 설치하는 예를 포함하였다. 아래의 예제는

Ubuntu Linux 64비트이기 때문에 특별한 명령어는 바꿔야 할 수도 있다
                                           （예를 들어

apt-get). Max OS x에서 소스로부터 빌드하고 싶다면 텐서플로우 웹사이트의 공식 사

용 가이드를 추천한다．

     https://www.tensorflow.org/versions/master/get_started/
     os_setup.html#installation-for-mac-os-x



의존성 설치

 여기서는 Virtualenv 설치와 관련된 이전 섹션에서 python-pip, python-dev,
 python-virtualenv가 이미 설치되어 있다고 가정한다．



텐서플로우를 빌드할 때 몇 개의 다른 의존성이 필요하다. 파이썬 버전에 맞게 다음의

명령어를 실행하자：


Python 2.7

 $ sudo apt-get install python-numpy python-wheel python-imaging swig


Python 3

 $ sudo apt-get install python3-numpy python3-wheel python3-imaging swig




Bazel 설치

Bazel은 Google의 내부 소프트웨어 Bazel에 기반한 오픈 소스 빌드 툴open source buiLd

tool이다. 책을 쓰는 지금 시점에, 텐서플로우는 소스로부터 빌드하기 위해서는 Bazel이




                                    소스를 사용한 설치 예： 64 비트 Ubuntu Linux with GPU 지원   -   9


===== PAGE 24 =====
             필요하기 때문에, 이를 직접 설치해야한다. Bazel 웹사이트에 전체 설치 방법이 있지만，
             여기에서 기본척인단계를 설명한다．

             먼저 Java Development Kit 8이 설치되었는지 확인하자．
                                                   아래의 명령어들은 0rade
             JDK 8 repository를apt의다운로드 위치로추가하고，
                                              그것을설치할것이다．

              $ sudo apt-get install software-properties-common
              $ sudo add-apt-repository ppa:webupd8team/ java
              $ sudo apt-get update
              $ sudo apt-get install oracle-java8-installer



              Ubntu 버전 15.10과 이후의 버전은 0racle JDK 대신에 OperkJDK 8를 설치할 수 있
              다. 이것이 더 쉽고 추천되는 방식이다. 0perdDl
                                          （를 설치하기 위해서는 위의 명령어
              말고 아래의 명령어를 사용하자．

              # Ub（』ntu l5. 그0
              $ sudo apt-get install openjdk-8- jdk
              # Ubuntu 그6. e4
              $ sudo apt-get install default-jdk



             다음단계 이전에 Java가 정확하게 설치되었는지 확인하자：

              $ Java -version
              # 5h0uL (/ 5ee 5tmiLαr output as beL0w
              java version "l. 8.0_91'
              그ava (TM) SE Runtime Environment (build 1.8.0_91-b14)
              Java HotSpot(TM) 64-Bit Server VM (build 25.91-b14, mixed mode)



             Java 설치 후에 설치할몇 개의 의존성이 더 있다．

              $ sudo apt-get install pkg-config zip g++ zliblg-dev unzip




10   -   CHAPTER 1 텐서플로우설치하기


===== PAGE 25 =====
다음으로，
    Bazel 설치 스크립트Bazel installation script를 다운로드하자. 이를 위해

서 GitHub에서 Bazel releases page로 가거나，
                                   다음의 wget 명령어를 사용하자．
Ubuntu에서는"bazel-installer-linux-x86 64.sh":


 # Down LoadS 8azeL o. 3. o
 $ wget https://github.com/bazelbuild/bazel/releases/download/0. 3.0/
 bazel-8. 3.0-installer-linux-x86 64. sh



이제 스크립트를 실행 가능하게 해서 실행할 것이다．


 $ chmod +x bazel-<version>-installer-linux-x86 64.sh
 $ ./bazel-<version>-installer-linux-x86 64. sh --user



--user flag을사용함으로써 Bazel이 사용자를 위한／bin 디렉터리에 설치된다．
                                                당신의
PATH에 추가되게 하려면 당신의 /.bashrc를 업데이트하기 위해서 다음의 명령어를 실

행하자．


 $ sudo printf '\nexport PATH="$PATH:$HOME/bin" ' >> '/ .bashrc


bash 터미널을 재 시작하고, 모든 것이 정확하게 작동하는지 테스트하기 위해서 bazel
을 실행하자．


 $ bazel version
 # You shouLd see some output Like the foL Lowing
 Build label: 0.3.0
 Build target:




멋지다1.다음으로CPU 지원을 위한올바른 의존성을 설치하자．




                                  소스를 사용한 설치 예： 64－비트 Ubuntu Linux with GPU 지원   - 11


===== PAGE 26 =====
   CUDA 소프트웨어 설치
               （NVIDIA CUDA GPU만 가능）

                 IA GPU를 가지고 있다면, GPU가 지원되는 텐서플로우를
   CUDA를 지원하는 NV끄〕
   설치할수 있다. 아래에 CUDA가 가능한 비디오 카드의 목록이 있다．

        hnps刃developer.nvidia.com/cuda-야)US

                             당신의 카드와 관련된 " Compute
   당신의 GPU가 이 리스트에 있는지 확인한 후에，
                             GeForce GTX 1080은 6.1의 compute
   Capability" 숫자를 적어두자．예를 들어，
               GeForce GTX TiTAN X는5.2의 compute capability를 가지고 있다·
   capabffity이고，
   텐서플로우를 컴파일할 때 이 숫자가 필요하다. 일단 CUDA를 사용하기로 결정했으
   면NVIDIA의 " Accelerated Computer Developer Program" 에 가입하자．
                                                            CUDA와
   cuDNN을 설치하기 위해 필요한 모든 파일을 다운로드하려면 필요하다. 아래에 링크
   가 있다：

        h村p勁developer.nvidia.com/accelerated-comPuting-developer

    가입을마쳤으면, CUDA를다운로드하자. 아래의 링크에 가서 설치 방법을따르자：

        hnPs://developer.nvidia.corn/cudα downloadS




                                                 非뇨
                                  0

         c
         【．C1 .n 盼｀e 9reen bu'mns that 뺘tscrrbe your tar9et ptat化rrn 〔〕n1y tapperted ptart미ㅜn` m1
                                                                                                【 be thOr.rt
                                                                                                               l

                                                                  ■ .

            ver51.n
                                                                  m
            lestattet rype.




         0oartttead Target 油htatter 幻터．
                                      tree bbtanlrt 14,84 工86)4


         ,eda-r.poubante1604-7-5-tttat75-l8atttdtt dab ttrd5retrt: 5d6568139d70270d9234d511td697t71




         1n`ta
             【lah.n 1n5trUㄷh.ㅔ노
            !   tttdo dpkg -, tt,da-r叩o-eborttalhrt4-7-5-toeat 75-18 atttd64deb
            z eado apt-get ,pdate
            J   sudoapt-get,astattteda


         "r 山nmnnf.n11ah.n. 뵤e 1h큔 nS'J4m' ∼ 二 :r 」               ' and nm




대APTER 1 텐서플로우 설치하기


===== PAGE 27 =====
  1.   "Select Target Platform"아래에아래의옵션을선택하자：




       · 14.04115.04
                   （당신이 사용하는버전）
       · deb(local)
  2.
       "Download" 버튼을클릭하고 컴퓨터의 어딘가에 저장하자. 이 파일은용량이
       커서 시간이 조금 걸린다．
  3.
       다운로드한파일이 있는 디렉터리로 가서 아래의 명령어들을 실행하자：
       $ sudo dpkg -i cuda-repo-ubuntu1404-7-5-local_7.5-18_amd64.deb
       $ sudo apt-get update
       $ sudo apt-get install cuda


이것은CUDA를 /usr/local/cuda 디렉터리에 설치할 것이다．

다음으로 cuDNN을 다운로드하자. 이는 딥 신경망을 설계하기 위한 CUDA의 별도의
add-on이다. 아래의 페이지에서 ''Download" 버튼을클릭하자．

       hnps刃developer.nvidia.com/cudnn

위에서 만든 계정으로 들어가면 간단한 서베이를 한다. 서베이를 기입하면 다운로드
        "I Agree to the Terms..." 을클릭하면 각자의 다운로드옵션으
페이지로들어간다．
로 넘어간다. 위에서 CUDA 7.5 이상의 버전을 설치하였기 때문에, CUDA 7.5를 위한
           （지금 시점에는cuDNN 버전 5.0을 가정한다）
cuDNN을다운로드하자                         .

"Download cuDNN vS for CUDA 7.5" 를클릭하면다운로 三 옵션이 펼쳐진다：




                                     소스를 사용한 설치 예： 64비트 Ubuntu Unux with GPU 지원   - 13


===== PAGE 28 =====
          cuDNN Download

                                 , 5PU.accelsca1H bbrary 이Pr隅，
                                                             n"e` '. dnp n.u,aI ".I*o,1ts

          ' m9r·t k 1fl. ㅜ卄n멥mIt.. (UDNㅒ鈿rt1날．
                                             m ㄴt손n仕 ^q "m뀀nt
          Pleass check 50cc, t,a,,eec,rlc dccc,n, tahocc m determne he mt.mmem.ed 쟁er，
                                                                                     띠n m〔냐
                                                                                          ［〕1댐N
          lfyOcace cscflgcu마SN clh a Pascal 1018 m며｝610 m7이 ''r듸m Sedate,,. mqu1red


                山nm.川 oaOeSNe5.lRC LO.,e 19. ㄻ1t.L See CODA 80 吼


            ｛눕mn甘.出 OtOOtON eSl AC Ike.. it.. 201st 財 CODA 7S


                以7weSead cUDNN .7 似．
                                   y27. 201H」
                                            α .J《〕
                                                 ＾ 8. Rc

                                                                                                  므, 뺘i「“"-－一 1
                'te*
                       ,chaA cccDISN sOIl'S. 1→   ‘∥口W1667 7  〕
                加*＋쨋·써【니｀)N"ak [n枸 m ati'1 he C1'n^ 7 . 거너 tJ1甘
                                                                                                         ：쓰＝:：玄？'
          ^'r1`m,ed 山O∥ n커ea5￡
                             ｀




    "cuDNN v5 Library for Lmux" 를클릭하고 압축된zipped cuDNN 파일들을 다운로드

    하자：



          cuDNN Download

                                  GP盼dccetetalcd t,b,aty 이 Prmα'on 눈S deep stUeat Setw.rk5

          J ^9re' 1. the TIKm1口
                              ＇nm
                                【u【）
                                   숴ㅐ駟f
                                      ＇별．
                                        r' Ure1”七 ^9
                                                   『eemen뺨
          PLe걍5e〔heL1 y0Ur 'rameW.rk 曲cumemah.n t. deteeet,,cethe,ecottt,e,endedaers,oncfcc0NN
          tydcc arecS,flgccDi새 00,11a Padcs나SIX m8미 GTX m701. cerstonl estate, tfloeqccteed


                Doee'tdad cc0NN .7 1 유c 盼』
                                         1.
                                          . Ii 2이헤* 10r cUD^ · . nC


                leoactcoac硼NNot I m=IO,.ceit. 201此 岫 CODA I 5
                                                                                                  GPu c.mP的nq           r F이mo
                .1.'rn，
                      여id Cuoi∥ 닐引May z7 zn1시．
                                             句＇O1끄）
                                                  ^ `. Rc


                QDAmAaa coal거4써 읠드 IHa, ', 찌1a~ i『 1긺
                                                    ［      7=                                      3ㅁ
                                                                                                           nㅗ尸－
                                                                                                                              至
                                                                                                  mK .m 뇨∼너掛E寸떼f` KJ ＇小 ·뜅m
                cU마1N 나s1？ㅜ 伽엥e                                                                   '1嵋1甘r` , 山 cmm甘月d1mm= m
                                                                                                  d1*幽꿸 em口m＜口甲m t"` `
                (U［卜卜1N h5柏d Gccd

                  etooncotcc. rarlrn..t)




                                                                                                  疏
                                  -
          (c.
                cu.＇널r1 75 L心m사 "r bnu` IDA寸 P- m

                cUONNctL,SeaytQ( w啣-5,

                t`d거叫4 sO L쎄
                           ＇a1y 1nr 빎＝mI.1m, 10

                coDNNe5Llb,,eyi,eOSt

                  cONH OS cme `a〃”m"

                esc）
                   ㅐO a§ Re1e1｀』“예，

                m      NH v5 RoOd,片 Lka가 tee       1oal

                (U마‘ㅐ힁｀0e驪1叩甘 1」
                               m "Y 1酵 LmUi 1功td

                oilx1`Y5 C08.65mm`첩녑 -p 0.a'1ID.뻐




CHAPTER 1 텐서플로우 설치하기


===== PAGE 29 =====
.tgz 파일이 다운로드된 디렉터리로 가서 아래의 명령어로 /usr/locallcuda 디렉터리에
정확한 파일들을 넣자：


 $ tar xvzf cudnn-7. 5-linux-x64-v5.0-ga.tgz
 $ sudo cp cuda/include/cudnn.h /usr/local/cuda/include
 $ sudo cp cuda/1ib64/libcudnn* /usr/local/cuda/1ib64
 $ sudo chmod a+r /usr/local/cuda/include/cudnn.h /usr/local/cuda/11b64/libcudnn*



여기까지가（그JDA를 설치 과정 끝이다！이제까지의 의존성에 대한 고려를 바탕으로
이제 텐서플로우를 설치해보자．



텐서플로우를 소스 코드로부터 빌드해서 설치하기

GitHub에서 텐서플로우 리파지토리를복제해서, 그 디렉터리로 들어가자：


 $ git clone --recurse-submodules https ://github.com/tensorflow/tensorfiow
 $ cd tensorfiow


                                     이는 Bazel에서 사용할 컴파
그 디렉터리에서 .Iconfigure script 명령어를 실행하자．
일러, CUDA의 버전 등을 알려준다. 이전에 설명하였던 본인의 GPU 카드와 관련된
"compute capability'" 숫자를알고있어야한다：


 $ ./configure
 Please specify the location of python. [Default is /usr/bin/python]: /usr/bin/
 python
 # NOTE: For Python 3, sped力／ /usr/bth/python3 thstead
 Do you wish to build lensorFlow with Google Cloud Platform support? [y/N] N


 Do you wish to build TensorFlow with GPU support? [yIN] y


 Please specify which gcc nvcc should use as the host compiler. [Default is/usr/bin/
 gcc]: /usr/bin/gcc




                                 소스를 사용한 설치 예： 64 비트 Ubuntu Linux with GPU 지원   - 15


===== PAGE 30 =====
Please specify the Cuda SDK version you want to use, e.g.7.0. [Leave empty to use
system default]: 7.5


Please specify the Cudnn version you want to use. [Leave empty to use system
default]: 5.0.5


Please specify the location where cuDNN 5.0.5 library is installed. Refer to
README.md for more details. [Defaultis /usr/local/cuda]: /usr/local/cuda


Please specify a list of comma-separated Cuda computecapabilities you want to build
wi차1.
You can find the compute capability of your device at:
https :1/developer.nvidia. com/cuda -gpus.
Please note that each additional compute capability significantly increases your
build time and binary size.
[Default is: "3.5,5.2"]: <YOUR-COMPUTE-CAPABILITY-NUMBERHERE>


Setting up Cuda include
Setting up Cuda 11b64
Setting up Cuda bin
Setting up Cuda nvvm
Setting up CUPTI include
Setting up CUPTI 1ib64
Configuration finished




                  구글의 클라우드 플랫폼
                             （Google Cloud Platform）
                                                   은 현재 closed alpha 단계이다. 그
                  프로그램에 접근할 수 있다면 Google Cloud Platform support 질문에 yes라고 답해
                  도 된다．



               설정이 끝나면 파이썬 이진 파일을 생성할 실행 파일을 만들기 위해서 Bazel을 사용할

              수 있다：




  16 -   CHAPTER 1 텐서플로우 설치하기


===== PAGE 31 =====
 $ bazel build -c opt --conf9g=cuda
 //tensorflow/tools/pippackage: build_pip_package



이단계는 사용하는 컴퓨터의 성능에 따라서 시간이 좀 걸릴수 있다. Bazel 수행을마치
면, 출력된 실행 파일을 실행하고 파이썬 휠Python wheel을 저장하기 위해서 위치를 넘겨
주자：


 $ bazel-bin/tensorflow/tools/pip_package/build_pip_package -'/tensorflow/bin

위의 명령문이 파이썬의 .whi 파일을∼/tensorflow/bin/ 내부에 생성한다. 이때 텐서플
로우의 Virtualenv가 액티브한지 확인하자．
                          그리고 wheel을 pip로 설치하자
                                             （실행 파
일의 정확한 이름은 설치된텐서플로우의 버전, 운영체제의 종류, 파이썬의 버전에따라
다를수 있다）
      .


 $ tensorfiow
 (tensorflow)$ sudo pip install ` /tensorfiow/bin/tensorf1ow-0.9.0-py2-none-any.whl



비슷한하드웨어를 가진 여러 대의 컴퓨터가 있다면, 모든 컴퓨터에 텐서플로우를 설치
하기 위해서 이 wheel을사용할수 있다．

이제 Jupyter Notebook과matplothb를 설치해보자．




Jupyter Notebook 설치하기

  iPython을 설치하기 위해서 다음의 명령어들을 입력하자．
먼저，                               iPython은 놀랍도록
                                        우리는 파이썬 2
유용한 인터랙티브 파이썬 커널이며Jupyter Notebook의 핵심이다．
와파이썬3 커널 모두를설치하기를 권장하다. 더많은옵션을사용할수 있기 때문이다
（따라서 아래의 명령에 모두를 실행하자）
                     :




                                                            Jupyter Notebook설치하기   - 17


===== PAGE 32 =====
            # Pyt加n 2. 7
            $ sudo python2 -m pip install ipykernel
            $ sudo python2 -m ipykernel install
            # Python 3
            $ sudo python3 -m pip install jupyterhub notebook ipykernel
            $ sudo python3 -m ipykernel install


           다음으로, 두 개의 간단한 명령어를 실행해야 한다. 먼저 build-essential 의존성을 설치
           하자：

            $ sudo apt-get install build-essential



           그런 후에，
                pip를 이용해서 Jupyter Notebook을 설치하자
                                               （파이썬 3을 사용하는 경우
           에는pip3):

            # For Pyt/1
                      《가〕 2. 7
            $ sudo pip install jupyter
            # For Python 3
            $ sudo pip3 install jupyter



           공식적인 설치 방법은Jupyter 웹사이트에 있다．

                 加p功upyter.readthedocs.io/en/Iatest/instalLhtml



           matplottib 설치하기

           Linw/lJbuntu에 matplotlib를 설치하기는 쉽다．
                                             다음을 따라하자：

            # Python 2. 7
            $ sudo apt-get build-dep python-matplotlib python-tk
            # Python 3
            $ sudo apt-get build-dep python3-matplotlib python3-tk




18 -   CHAPTER 1 텐서플로우 설치하기


===== PAGE 33 =====
텐서플로우，Jupyter Notebook, matptotlib 테스트하기

모든 것이 정상적으로 작동하는지 다시 한번체크하기 위해서 몇 개의 더미 코뜨-dummy
code를 실행해보자. "if-notebooks" 라는 디렉터리를 만들자. 그 디렉터리에 들어가서
                               텐서플로우환경이 액티브한지 확
jupyter notebook을실행하자 다시 한번강조한다．
실히하자．

(tensorflow)$ mkdir tf-notebooks
(tensorf]ow)$ cd t-F-notebooks
(tensorflow)$ jupyter notebook



Jupyter Notebook 서버가 시작되고 웹 브라우저에 소프트웨어가 실행될 것이다．
tf-notebook 디렉터리에 지금은 파일이 하나도 없다고 가정하자. "Notebook list
is empty" 라는 메시지를 가진 텅 빈 워크스페이스workspace를 볼 것이다．새로운
notebook을만들기 위해서 페이지의 우측상단의 "New" 버튼을클릭하자. 그리고 텐
서플로우를설치할때사용한파이썬버전에따라" Python 2" 또는" Python 3" 중하나
를 선택하자．



                                            Upkad

                                   Text File
                                   Folder
                                   Terminal


                                   Notebo가s




                                   텐서플로우．Jupyter Notebook, matplotlib 테스트하기   - 19


===== PAGE 34 =====
    새로운 notebook이 자동으로 열리고 작업하기 위한 빈 판이 보일 것이다. notebook에
    새로운 이름을 지정하자. 화면의 상단에''Untitled" 를클릭하자：

         =jupyter                          .넌－       첵 ".   W｀·｀qd` 끼戶 ("ma형目1d떪’ ．히




          .       +   *   色   .   +   +   H 1    .     vN뇬




              -




    notebook의 이름을변경하는팝업창이 열릴것이다．
                               이는확장자가 .ipynb인notebook
                이 예제에서 우리는"My First Notebook" 으로 이름지었다．
    파일의 이름도 변경한다．


                                          Re1mn紀 N여ebook


                                          Em∥1 mm 一小           mm


                                          ; 나r Fh' ｀뻐aX슭



                                                                                       -C-
    이제 실질적인 인터페이스를살펴보자．
                      In[ 〕옆에 빈 셀cel〔이 있다. 여기에 파이썬 코
    드를 입력할수 있다．
              여러 줄의 입력도 가능하다．TensorFiow, NumPy, matplotllb의
    pyplot모듈을notebook으로 임포트하자：

     import tensorfiow as tf
     import numpy as np
     import matpiotiib.pypiot as pit




애APTER 1 텐서플로우 설치하기


===== PAGE 35 =====
      =Jupyter MyF'rStNmeb에kLa口C뺨以k－∼，
                                     m四凹이.『啣．
                                            d:－뢰

      巴   *    }   ?     1`   ◆   *   H   ■   0           '   口   ·叫낙小』
                                                                      뇨U




              1n［】
                 L       i■戶rt 'ensoflth닐 륩｀ tf
                         ｀口md n뻐1y a` nP
                         U "rt 1 .tpthtlib. 뻐
                                            ＇Pt야 11 pt'



      -       1n [ ㅣ =




셀을 실행하기 위해서 shift-enter를 입력하면, 코드가 실행되고 새로운 셀이 아래에 생
성된다．
   왼쪽에 In[1}：이라고 변경된부분을볼수 있는데, 이는 커널에서 실행할코드의
첫 번째 블록b〔ock을 의미한다．
                  다음의 코드를 적당한 개수의 셀
                                  （많거나 적거나 상관없
다）
 로 notebook에 입력하자. 관련된 코드를자연스럽게 묶기 위해서 셀 안에서 줄을 띄
워도 된다．


%matplotlib inline
 a = tf. random_normai([2,20])
 sess = tf. Session()
out = sess. run(a)
 x, y = out


plt. scatter(x, y)
pit. show()




                                                                           텐서플로우, Jupyter Notebook, matplotlib 테스트하기   - 21


===== PAGE 36 =====
          ＝〕UpyteI My Fi,st Notebook｀』om'.'.
                                                  느nm叫      "

          巴    +    1   ?    r,   수   .   ㅒ   1   .   L』
                                                       ）夔       '   디 〔뻣lT窈加茁




                   in lt 1   J   r ' ttHSOrflO닐 11 it
                             ㅗ뻐衿rt n너떼가 *1 nP
                             `1m
                               『1 .tp1. 1tlb. PyPmt .` Ptt




           -

    아래 줄은특별하기 때문에 자세히 설명하자．


     %matplotlib inline



    이 명령어는notebook이 브라우저의 내부에 직접 matplotlib 차트를 출력하라는 명령
    어다．

    나머지 코드를한줄씩 설명하자. 아래 설명에서 모르는용어가 있더라도 걱정하지말자
    이 책에서 모두 설명할 것이다：

      1. 랜덤숫자로2 x 20매트릭스를정의하기 위해서TensorFiow를사용하고변수a

          를할당하자．
      2. TensorFiow Session을시작하고，
                                이를sess라고하자．
      3. sess.run( ) 메소드로실행하고，
                             출력NumPy array을out라고하자．
      4. 2x20매트릭스를2개’의1x10벡터로나누J긱각각을x와y라고하자．

      5. pyplot으로x와y를이용해서산점도scatter plot를그리자．




애APTER 1 텐서플로우 설치하기


===== PAGE 37 =====
모든 설치가 성공적이라면 위와 유사한 결과를 볼 수 있을 것이다. 간단한 샘플이지만
이제 본격적으로 진행할수 있을 것이다．

Jupyter Notebook의 자세한튜토리얼은아래의 페이지를참고하자：

     http://jupyter-notebook.readthedocs.io/en/Iatest/examples/
     Notebook/examPles_index.html




결론

축하한다. 이제 바로 사용할 수 있는 TensorFiow를 가지고 있다. 다음 장에서 중요한
TensorFiow 개념을 배우고 라이브러리를 이용해서 당신의 첫 번째 모델을 만들 것이
다. TensorFiow 설치에 문제가 있으면공식 설치 방법을참고하자：

     https//www.tensorflow.org/versions/master/get_started/os_setup.htm!




                                                                           결론   - 23


===== PAGE 38 =====
        서론




         느뻥J口k」i-玎그
     ·＾1-，三，
           ,a石衲b囚 '1坪ㅂ



琳w
               --   r
                    。   o


===== PAGE 39 =====
             모든 곳에서 넘쳐나는 데이터

             우리는 지금 " 정보화 시대" 에살고 있다. 요즘, 모든곳에서 데이터들이 흘러가고flow 있
             다：스마트폰, 시계, 자동차, 주차요금 미터기, 집안의 가전 제품들. 이름을 말할수 있는
             거의 모든 기술들이 요즘은클라우드 어딘가에 있는 데이터베이스와통신하고 있다. 거
             의 한계가 없는 메모리 용량으로 개발자들은 점점 데이터 웨어하우징data warehousing과
             그들의 제품과 고객으로 부터의 수 페타베이트petabytes어］달하는 데이터에 " more-is-
                 （많을수록좋다）
             better     " 접근을하고있다．

             동시에, 컴퓨터의 계산능력은 점점 더 향상되고 있다. CPU 속도 향상은 느려지고 있지
             만 병렬 처리 구조가폭발적으로 향상되고 있다. 처음에는주로 컴퓨터 게임에 사용되었
             던 GPUGraphic Processing Units는 이제 일반적인 연산general purpose computing에도 사용
             되고 있고，
                  머신 러닝의붐을 열었다．

             머신 러닝Machine Learning: ML은 데이터를 사용해서 특정 질문에 대답하기 위해서 일반
             적인 목적의 수학적인 모델을 사용한다. 머신 러닝은 스팸 메일을 식별하거나, 고객을
             위한 제품을 추천하거나, 여러 해 동안의 상품의 가치를 예측하기 위해 사용되고 있다．
             최근에는 특별한종류의 머신 러닝 기법이 다양한분야에서 믿을수 없는속도로 성공하
             고 있다．
                 이를딥 러닝dee이earning이라고한다．




             딥 러닝
                （deep Learning)

             " 딥 러닝"은다층 신경망multi-Layer neural networks의 처리 과정을 기술하기 위해 사용되
             는용어가 되었다. 다층 신경망은 아주 많은다양성을 활용할수 있고, 많은수학적 기법
             들을 결합해서 사용할 수 있는 아주 플렉서블한flexible 개념으로써 아주 강력하다. 그러
             나 신경망을 이용해서 큰 성공을 거둔 것은 상대적으로 최근의 현상이다. 그 이유는 최
             근에야 다른 머신 러닝 기법을 능가하기 위한 엄청난 양의 데이터와 계산 능력을 가질
             수 있게 되었기 때문이다．




26   -   CHAPTER 2 서론


===== PAGE 40 =====
딥러닝의 파워는 최대의 효과를내기 위해서 데이터를 사용하는방식을 결정할때 더많
은유연성을 모델에 제공해주기 때문이다. 어떤 입력이 고려할 가치가 있는지 사람이 대
략적으로 추측하는 대신에，
             잘 조절된 딥 러닝 모델이 모든 파라미터parameters를 가지
고 유용한그리고 입력 값들의 고차원higher-order 조합을자동으로 결정할수 있다. 이로
써 훨씬 더 정교한 결정 판단decision-making 프로세스가 가능해졌고, 컴퓨터가 훨씬 더
지능적이 되었다. 딥러닝으로 우리는자율주행 차량과 우리의 말을 이해하는 전화기를
만들수 있다．
      딥러닝으로 인하여 기계 번역，
                     얼굴 인식，
                          예측분석predictive analytics, 자동
작곡 등, 셀 수도 없이 많은 인공지능 작업들이 가능해지고 있고 그것들의 능력이 향상
되고 있다．

딥러닝 뒤에 숨겨진 수학적 개념들이 수 십넌 동안 개발되어 왔지만, 이러한 딥 모델
들을 만들고 학습시키는 프로그래밍 라이브러리들은 최근에야 사용 가능하게 되었
다．
 불행히도 대부분의 이러한 라이브러리들은 유연성flexibility과 생산 가치성production-
worthines＄에 장단점trade-off이 있다. 유연한 라이브러리들은새로운모델 구조를찾을때
아주중요하다. 그러나종종 너무 느리거나 실제 제품에 사용되지 못하곤 한다. 반면에,
분산 환경에서 실행 가능한 빠르고 효율적인 라이브러리들은 특정한 형태의 신경망에
최적화되어 있어서 새롭게 더 좋은모델에는 적합하지 않을수 있다. 이런 상황이 어떤
결정을 내릴때 딜레마에 빠지게 한다. 조금은덜유연한 라이브러리들을사용／연구해서
코드를새로 만들 필요가 없는 방법을사용할 지, 연구를 위해서 특정 라이브러리를사
용하고 실제 제품을 위해서는 완전히 다른 라이브러리를 사용할까를 고민해야 한다. 첫
번째 방법을 사용한다면 다양한 형태의 신경망 모델을 테스트할 수 없을 수도 있다. 두
번째 방법을사용한다면완전히 다른 API를가지는코드를사용해야한다. 이를 위한자
원을 가질 수는 있을까？

TensorFiow는 이러한 딜레마를 해결하는 것을목표로한다．




                                               딥 러닝
                                                  （deep learning)   - 27


===== PAGE 41 =====
    TensorFlow: 최신의 머신 러닝 라이브러리

    텐서플로우는 2015년 11월에 Google에 의해서 공개된 오픈소스로써 DistBelief라는
    이전모델을만들고 사용함으로써 배운 수년 동안의 경험을바탕으로 만들어졌다. 유연

    하고，
      효율적이며, 확장성이 있고, 휴대성을 가질 수 있게 만들어져서, 스마트폰부터 대
    형 컴퓨터 클러스터까지 어떤 형태나 크기의 컴퓨터에서도수행 가능하다. 학습된 모델
    을 금방 실제 제품어］사용할 수 있도록 하는 경량 소프트웨어가 제공되고, 모델들을 새
    로 만들 필요가 없다. 텐서플로우는 오픈 소스의 혁신과 협동을 채택하고 있지만, 큰 회
    사의 지원，
         도움，
           안정성 또한가지고 있어서，
                        스타트업부터 Google처럼 큰 회사에 이르
    기까지 개인이나 기업 모두사용 가능하다.

    당신이나당신의 동료가 데이터, 궁금한 질문, 수행 가능한 컴퓨터가 있다면, 텐서플로
    우는당신이 찾는남아 있는마지막부품일수 있다．




    텐서플로우： 기술적인 개괄

    이 섹션은 텐서플로우 라이브러리에 대한 개론적인 정보를 제공한다. 텐서플로우가 무
    엇이고, 텐서플로우의 개발과정의 역사, 사용된 사례, 그리고 경쟁 제품들과 대적할수
    있었던 이유들을 알아본다. 결정을 해야 하는 사람, 이해 관계자, 텐서플로우의 배경 지
    식을 이해하고 싶은사람은이 섹션에서 도움을받을수 있을 것이다．



    구글의 딥러닝 관련 간단한 역사

    Google의 첫 대규모 딥러닝 툴은 Google Brain 팀에서 개발한 DistBelief였다．
    DistBelief는딥 신경망deep neural network을 사용하는 셀 수 없이 많은프로젝트를 위해
    서 수십 개의 팀에 의해서 사용되었다. 그러나많은 첫 번째 프로젝트들 처럼 DistBelief
    의 사용성과 유연성을 제약하는 설계상의 실수가 있었다. DistBelief를 만든 후에，
    Google-은DistBelief의 사용으로 배운 경험을 바탕으로 그 후계자를 만들기 시작했다．




CHAPTER 2 서론


===== PAGE 42 =====
이 프로젝트가2015년 11월에 공개된 텐서플로우인데, 금방머신 러닝을 위한대중적인
라이브러리가 되었으며 자연어 처리，
                  인공지능，
                      예측 분석predictive analytics 등에 사용되
고 있다．




텐서플로우란 무엇인가？

텐서플로우가 어떤 문제를 해결하려고 하는 것인지 이해하기 위해서 텐서플로우를 전
체적으로살펴보자．



한 문장으로 이해하기

텐서플로우 웹사이트를 보면방문자에게 보이는 첫 번째 문장은 아래와같다：

  lensorFiow is   an Open Source Software Library for Machine
  Intelligence


그밑에 " About TensorFiow" 밑의 첫문단에 아래의 설명을찾을수있다．

  TensorFlow'" is an open source software library for numerical
  computation using data flow graphs.


이 두 번째 정의는 조금 더 구체적이기는 하지만, 수학이나 기술적인 배경 지식이 적은
사람에게 최적의 설명은 아닐 것 같다. 이제 세부적인단위로 나누어서 각각을 이해해
보자．

오픈 소스

Google이 만든 텐서플로우는 처음에는 구글 내부의 머신 러닝 툴이었다．
                                        그러나 구현
된 결과물이 2015년 11월에 Apache 2.0 라이선스로오픈소스로공개되었으며，
                                             누구나
    수정, 사용이 가능한 오픈 소스 소프트웨어이다. 오픈 소스 개발자들은 이 코
다운로드，
드에 추가하거나 개량할수 있고，
                향후의 버전에 자신의 수정 사항이 포함되기를 제안할




                                                      텐서플로우란무엇인가？   - 29


===== PAGE 43 =====
          수 있다．
              텐서플로우가가진 대중성으로 인해서 Google이나third-party 개발자들에 의
          해서 매일매일라이브러리가향상되고 있다．


           "텐서플로우"라고 하지 않고 ' 구현된 결과물"이 오픈 소스로 공개되었다는 점에 주
           의하자. 기술적으로 말하면, 텐서플로우는 텐서플로우 wme paper에 기술된 수학적
           인 계산을 위한 인터페이스이다. 그리고 Goo이e은 여전히 자신의 내부 구현물을 가
           지고 있다. 그러나, 오픈 소스 구현 결과물과 Goo이e 내부의 구현물의 차이점은 다른
           내부 소프트웨어들과의 연결이지, Go刈e이 좋은 것들을 몰래 간직한다는 것은 아니
           다. Goo이e은 내부적인 혁신들을 대중에게 공개하고 있고, Google의 내부 버전과 동
           일한 성능으로 계속 오픈 소스는 공개되고 있다．

           이 책에서 "텐서플로우' 라고 하면 이는 오픈 소스 결과물을 의미한다．



          수치 계산을 위한 라이브러리

          "머신 러닝을위한라이브러리" 라고하지 않고조금더 넓은범위의 " 수치 계산numerical
                              텐서플로우는 " learn"("Scikit Flow" 라고도 알려진）패키지
          computation" 이라고 하였다．
          를 포함하고 있다．
                   이는 Scikit-LearnI 한줄 모델링 기능one-line modeling functionality을
          에뮬레이트한다emulate. 텐서플로우의 주된 목적이 기성품out-of-the-box 머신 러닝 솔루
          션을 제공하는 것이 아니라는 점에 유의하자. 텐서플로우는 사용자가 수학적인 초창기
          표현에서 모델을 정의할 수 있도록 해주는 함수들과 클래스들의 모음이다. 이로써 사용
          자들은 적절한 기술적인 배경 지식을 바탕으로 커스터마이즈customized되고 유연한 모
          델을 직관적이고 빠르게 만들수 있도록 한다. 또한, 텐서플로우는 머신 러닝에 특화된
          함수를 많이 제공하기 때문에, 복잡한 수학 계산을 수행하기에 적합하다. 그러나 이 책
                （그중쇄서도 딥 러닝）
          은 머신 러닝          에 집중하기 때문에, 우리는 '머신 러닝 모델'을만들
          기 위한텐서플로우에 대해서 이야기할 것이다.

          테이터 플로우 그래프
                    （data flow gra山s)

          텐서플로우를 위한 계산모델은 노드nodes
                               （보통 원이나 박스로표시）
                                            가 함수functions／계




30 - CHAPTER 2 서론


===== PAGE 44 =====
                     a
               - '   .   ,   `
           7                     \

          r -input l
          t                      I

              ,＼느d/




               / 戶 - , `



          { input :
          `                      '
               S. - --


                     b                      I




산computations를 의미하고，
                   에지edges
                        （보통 화살표나 선으로 표시）
                                       는숫자，
                                          매트릭스，
                                              텐
서를 의미하는방향성 그래프directed graph이다．

이유는 여러 가지인데, 첫 번째로 신경망과같은많은 머신 러닝 모델들이 머신 러닝 전
문가들이 구현할 때 훨씬 편리한방향성 그래프로 이미 사용되고 있기 때문이다. 두 번
째로，
  계산들을 쉽거］미분 가능differentiable한 조각
                                （텐서플로우）
                                      으로 나눔으로써, 첫 번
째 노드의 출력 결과에 영향을줄수 있는다른 노드에 대해서 특정 노드
                                    （텐서플로우에
서는 연산operation이라고 부르는）
                     의 도함수derivative를 자동으로 계산할 수 있기 때문
이다. 출력 노드를 포함해서 어떤 노드의 도함수／기울기를 계산할 수 있다는 것은 머신

러닝 모델을 만들 때 필수적이다. 마지막으로, 계산을 분할함으로써 여러 대의 CPU,
CPU, 또는 다른 컴퓨터에서 분산 작업이 쉬워진다는 점이다. 큰 전체의 그래프를 작은
여러 개가 그래프로 나누고, 각 디바이스에게 분할된 그래프의 일부를 맡기는 것이다

（분산되어 있는 디바이스를 조율하기 위해서 정보를공유하는로직을포함해서）
                                      .




                                                텐서플로우란무엇인가？   - 31


===== PAGE 45 =====
                     짧은 고찰：텐서
                            （tensor）
                                   란 무엇인가？

    텐서는 간단하게 말하는 n차원 매트릭스이다. 2차원 텐서는 일반적인 매트릭스인 셈이
    다. m Xm 매트릭스
               （높이 m, 너비 m）
                          를 숫자들의 정방행렬
                                    （square matrix）
                                                  로 본다면，
    m Xm Xm 텐서는 숫자들의 큐브 행렬
                         （높이 m, 너비 m, 깊이 m）
                                          로볼 수 있다. 일반적으로，
    매트릭스 연산들에 대해서 익숙하다면텐서를 매트릭스와유사하게 생각할 수 있다．




    조금 더 자세한 설명

    "테이터 플로우그래프를 이용한수치 계산을 위한오픈 소스 라이브러리" 라는 말은 인
    상적인 표현이기는 하지만, 텐서플로우를 머신 러닝 라이브러리 중에서 돋보이게 할수
    있는몇 가지를놓치고 있다. 텐서플로우의 몇 가지 장점을자세하게 이야기해보자．


    분산
     （distributed)

    위에서 데이터 플로우그래프를 설명할때 언급된 것과같이, 텐서플로우는하나의 컴퓨
    터 내부의 여러 cpu, GPU 뿐만 아니라 여러 대의 컴퓨터 상에서 스케일러블scalable하
    도록 디자인되었다. 처음의 오픈 소스 구현은 분산 기능이 없었지만, 0.8.0 버전은 분산
    실행환경이 텐서플로우의 내장된b비〔t-in 라이브러리의 일부로 포함되어 있다. 이 초기
    의 분산API는 약간은 귀찮은 면이 있지만 놀랍도록 강력하다. 대부분의 다른 머신 러
    닝 라이브러리들은그러한 기능이 없는데, Kubernetes와같은클러스터 관리자cluster
    manager와의 호환성도추진되고 있다．


    소프트웨어들의 묶음

    텐서플로우는 머신 러닝 모델을만들고 학습시키기 위한API로 주로 불리고 있지만, 실
    제로텐서플로우는 연관된 소프트웨어들의 묶음이다：

       · 텐서플로우TensorFiow: 머신 러닝 모델을정의하ㅍ긱 데이터를학습시키고, 향후의



CHAPTER 2 서론


===== PAGE 46 =====
      사용을 위해서 엑스포트.export하기 위한API이다．
                                   실제 계산은C+＋로구현되었

      지만, 주된 API는 파이썬으로 사용 가능하다．
                               이로써，
                                  실제의 계산은 빠른 C++
      코드로 작성되어 있지만, 파이썬으로 데이터 사이언티스트data scientist나 공학

      자들이 더 친근한 환경에서 사용할 수 있다. 텐서플로우 모델을 실행할 수 있는
      C++ API도 있지만, 지금 현재는 제한적이어서 대부분의 사용자에게 추천되지

      는않는다．
 ·    텐서보드TensorBoard: 표준 텐서플로우 설치에 포함된 그래프 시각화graph
      visualization 소프트웨어이다. 텐서플로우의 특정 텐서보드와관련된 연산이 포함
      하면, 텐서보드는 텐서플로우 그래프에서 엑스포트된 파일을 읽어서 모델의 동

      작을살펴볼수 있도록해준다. 이는통계 요약, 학습분석, 텐서플로우코드의 디
      버깅에 도움된다. 처음부터 텐서보드의 사용법을 배운다면 텐서플로우를 이용
      한작업이 훨씬즐거워지고생산성을높일수있을것이다.                  -
                                             -
  .   텐서플로우서빙TensorFiow Serving：학습된텐서플로우모델을쉽 四       수있
      게 하는 소프트웨어이다. 내장된built-in 텐서플로우 함수를 사용해서 자신의 모
      델을 엑스포트하고, 이를 텐서플로우 서빙에서 바로 사용할 수 있다. 이렇게 해
                          입력 데이터를 받고，
      서, 간편하게 고성능 서버를 실행하고，         모델로부터의 결과

      를사용할수 있다. 또한, 텐서플로우 서빙은 예전 모델에서 새로운모델로 최종
      사용자end-users들이 쉽게 교체할 수 있다. 텐서플로우 서빙은 텐서플로우 생태
                                     텐서플로우의 경쟁력의 한
      계eco-system에서 가장주목 받지 못하는 부분이지만，
      부분이다. 서빙을 제품 생산에 사용하면 사용자들이 자신의 모델을 새로 구현할
      필요가 없고, 대신텐서플로우 엑스포트export를따라서 진행하면 된다．
                                            텐서플로

      우서빙은전부C++로작성되었으며, 해당API들은모두C卄로만사용할수
      있다.


텐서플로우의 전체 기능을 사용하는 것은 위에서 설명한 것들을 결합해서 사용하는
방법을 안다는 것을 의미한다. 그렇기 때문에 위의 세 부분 모두를 이 책에서 살펴볼 것

이다．




                                             텐서플로우란무엇인가？   - 33


===== PAGE 47 =====
    텐서플로우는 이런 경우에 사용하자


    텐서플로우를 사용한 예를몇 개 살펴보자. 일반적으로，
                                텐서플로우는 대부분의 머신 러
    닝 목적에 활용하기 좋다. 다음은텐서플로우를 사용한목록이다．

    새로운 머신 러닝 구조에 대한 연구, 개발, 반복 작업. 텐서플로우는 믿을수 없을 정도로
    유연하기 때문에, 새롭고 많이 테스트되지 않는 모델을 만들 때 솎용하다. 다른 어떤 라
    이브러리들은 변경하기 힘들고 미리 만들어진모델을 사용하기 때문에 프로토타이핑에

    는좋지만수정이 힘들다．

    학습에서 실전 배치까지 쉽게 활용. 이전에 설명한 바와 같이 텐서플로우 서빙은 사용

    자가 빨리 학습에서 실전 배치까지 할수 있도록 해준다. 모델을 만들고 돌려보는 작업            I
    을 훨씬 빠르게 반복적으로 할수 있도록 해준다. 당신의 팀이 빨리 운영되어야 하거나

    c+＋나Java 등으로 모델을다시 구현할충분한 리소스가 없다면，
                                      텐서플로우는당신의
    제품이 쉽게 시작할수 있도록 해준다．

    현존하는 복잡한 구조를 구현하기. 일단 텐서플로우에서 그래프를 만들고 시각화된 그
    래프를 보는 법을 배우면, 최근의 연구 논문에 소개된 모델을 텐서플로우로 구현할 수
    있다．
      이렇게 하면 새로운 모델을 만들 때 필요한 통찰력insight이 생길 수 있고，
                                                 각자의
    현재의 모델을향상시킬수 있다．

    대규모 분산 모델. 텐서플로우는 많은 디바이스에서 아주 쉽게 스케일 업scale-up을 할

    수 있다．  Google에서는 이미 많은 프로젝트에서 DistBelief를 대체하고 있다．
        그리고，
    최근의 분산 실행환경distributed runtime에서 클라우드 상의 가상머신 뿐만 아니라 많은
    하드웨어 서버에서 수행되는텐서플로우를 더 많이볼수 있다．

    모바일／임베디드 시스템을 만들고 학습시키기. 대부분의 경우에 텐서플로우는 스케일－
    업 능력에 초점이 모아지지만, 스케일－다운scale-down도 마찬가지이다. 텐서플로우의 유
    연성은 적은 계산 능력을 지닌 시스템까지도 확장된다．
                                Raspberry P1와 같은 미니 컴
    퓨터뿐만 아니라 안드로이드 디바이스에서도 수행될 수 있다. 텐서플로우 리파지토리
    repository에는 안드로이드에서 학습된모델을 실행하는 예제도 있다．



CHAPTER 2 서론


===== PAGE 48 =====
텐서플로우의 강점


사용성
  （usability)

  · 텐서플로우의 일관된API는새로운모델을만들때에도동일한방법을사용할
     수 있도록 해준다．
  · 텐서플로우의 API는안정적이다. 그래서 변경되더라도 호환성이 유지되게 하려
     고한다．
  · 텐서플로우는Numpy 라이브러리와 밀접하게 결합됨으로써 대부분의 파이썬
     기반의 데이터 사이언티스트가 편하게 사용할수 있다．
  · 다른 라이브러리와다르게 텐서플로우는 컴파일 타임이 없기 때문에, 사용자가
     더빨리 자신의 아이디어를반복적으로수행해 볼수 있다．
  · 텐서플로우의 상단에 Keras나SkFlow와같은 여러 개의 더 높은 레벨의 인터페
     이스들이 이미 있다. 사용자가 손으로 전체 모델을만들지 않고서도 텐서플로우
     의장점을사용할수 있게 해준다．


유연성
  （flexibility)

  · 텐서플로우는모든모양과크기의 컴퓨터에서 작동된다. 수퍼 컴퓨터부터 임베
     디드시스템, 그리고그사이의 모든종류의 컴퓨터에서 사용할수 있다．
  · 분산구조는 적정한 시간 안에 대량의 데이터를 모델의 학습에 사용할수 있게
     해준다．
  · 텐서플로우는CPU와CPU를동시에 사용할수있다．


효율성
  （efficiency)

  · 텐서플로우가처음나왔을 때, 유명 머신 러닝 벤치마킹에서 아주느렸었다. 그
     뒤로 개발팀은 아주 많은 시간과 노력을 들여서 텐서플로우의 코드를 향장시켰
     다. 지금은오픈 소스 머신 러닝 프레임워크 중에서 최고의 속도를 겨루는 정도



                                           텐서플로우의 강점   - 35


===== PAGE 49 =====
                에 이르렀다．
              · 텐서플로우의 효율성은아직도향상되고있다．


           지원
            （support)

                            Google은텐서플로우가머신 러닝 연구원들과개발자들어］
              · Google이 지원한다．
                 게 국제 표준이 되기를 원하기 때문에 텐서플로우에 아주 많은 자원을 지원하고
                 있다． Google은텐서플로우를자신의 작업에도사용하고 있다·
                   또한，
              · 텐서플로우를사용하는많은커뮤니티와GitHub상의 커뮤니티와개발자들의
                 응답을받기 쉽다．
              · Goog1e은텐서플로우를사용한여러개의학습된머신러닝모델을공개하였다·
                 무료로 사용할수 있으며 프로토타입이 많은 데이터 파이프라인 없이 실행할 수
                 있도록해준다．


           기타 특징들

              · 텐서보드는모델을디버깅하고 시각화하기 좋다. 다른머신 러닝 라이브러리어］
                 는 없는 기능이다．
              · 텐서플로우 서빙은 더 많은 스타트업 기업들이 자신들의 서비스와 리소스를 머
                 신 러닝에 쏟을 수 있도록 해주는 소프트웨어가 될 것이다. 모델을 사용하기 위
                 해서 코드를새로구현하는비용을 고려해야 하기 때문이다．



           텐서플로우를 사용할 때 어려운 점


           분산 지원은 아직 진행형

           공식적으로 공개되기는 했지만 텐서플로우에서의 분산특징을 사용하는 것은 기대하는
           것 만큼부드럽지는 않다. 이 책을 쓰는 지금, 각 디바이스의 역할을수작업으로 정의해




36 -   CHAPTER 2 서론


===== PAGE 50 =====
야 하는데，
     이 작업은 지루하고，
               실수하기 쉽다．
                      계속적으로 氷 되어야 하지만, 새로운
내용이라서 참고할 예제가 많지 않다. 이전에 Kubemetes를 위한 지원은 현재 개발되
고 있다고말했지만, 그러나 현재도 여전히 개발중이다．


커스텀 코드
     （custom code) 개발이 쉽지 않다．

텐서플로우로 자신의 연산.peration을 만드는공식적인 방법이 있다. 그러나 텐서플로우
에 최적화된 코드를 만드는 것은 꽤 많은오버헤드overhead를 필요로 한다. 만약 마스터
리파지토리master repository에 기여하고 싶다면，
                                Google 개발 팀이 당신의 질문에 즉시
도와줄것이다．


몇몇 기능
    （특징）
       은 여전히 없다．

다양한 프레임워크 상에서 머신 러닝에 대한 전문가라면 작지만 유용한 기능들이 아직
텐서플로우에는구현되지 않았다는 것을 알것이다. 종종돌아가는 길이 있지만 " 왜 이
러한 기능들이 원래 제공되지 않았지？" 라는 질문을하게 된다．




앞으로 그리고 위로！


말할 필요도 없이 우리는 텐서프로우의 미래에 대해서 아주흥분되어 있다. 당신에게 그
러한 강력한 툴을 소개하려고 하니 떨린다. 다음 장에서 당신은 텐서플로우를 설치하고
핵심적인텐서플로우라이브러리, 기본적인사용패턴과환경들을배울것이다．




                                                앞으로그리고위뢰   - 37


===== PAGE 51 =====
功吟茗t：  彼은 兮
    §i쐰，

텍專騫略옇
   1.   -'   -   _   :!   -   -   ,`   ';   -



         J督鷺□娑旦
             「'.1示芦


===== PAGE 52 =====
             계산 그래프
                  （computation gra뱌0 소개


              이 섹션은 텐서플로우와 별개로 계산 그래프의 기본적인 내용을 소개한다. 노드
              (node), 에지           （dependency) 개념들을 살펴보고, 여러 예제를 통해
                       （edge), 종속 관계
              중요한 원리를 살펴본다. 계산 그래프에 익숙한 독자는 이 섹션을 건너 뛰어도 무방
              하다．


             그래프 기본

             모든텐서플로우프로그램의 핵심에는텐서플로우시3J를사용하는 코드에 기술된 계산

             그래프computation graph가 있다．
                                     계산 그래프는 계산구조computational structure를 정의하
             기 위해 사용되는 특별한 형태의 방향성 그래프directed graph이다．
                                                      텐서플로우에서는자
             신의출력 결과를0개 이상
                         （0개, 1개，
                                그 이상）
                                    전달하는함수들의 연속적인 연결이다. 이
             러한방식으로 사용자는 더 작고 쉽게 이해할수 있는수학적인함수들을사용해서, 데

             이터에 복잡한 변형을 구현할수 있다. 단순한 예를살펴보자．




                                               －3
                                  b●
             위의 예에서 우리는 기본적인 addition 그래프를 살펴보자. 원으로 표현되는 함수는 화
             살표로 표시되는2개의 입력을받는다. 해당함수의 출력은 1과2를 더한 결과3을함수
             에서 밖으로향하는 화살표에 표시한다. 이 결과는또다른함수에게 전달되거나 사용자
             에게 전달될수도 있다．




40   -   대APTER 3 텐서플로우 기본


===== PAGE 53 =====
이 그래프를 간단한 식으로 생각할수도 있다．


            f (1,2) = 1+ 2= 3

위의 그림은 그래프의 두 개의 기본 빌딩 블록인 노드와 에지들이 계산 그래프를 만들

때 어떻게 사용되는지를보인다. 이제 세부사항을 설명하자．

  ·   노드nodes: 일반적으로원, 타원, 박스등으로표현하며, 그래프안허］
                                           서 데이터에
      적용될 계산computation이나액션action을나타낸다. 위의 예에서 " add" 오퍼레이
      션이 노드이다．

  ·   에지edges: 노드들사이에 전달되는 실제 값으로써 일반적으로 화살표로 표시한
      다. 위의 " add" 에서 입력 1과 입력 2는노드로향하는 에지이고, 출력 3은노드로
      부터 나오는 에지이다. 개념적으로 에지는 노드들 사이의 정보를 운반하는 역
      할을 하기 때문에，
               에지를 다른 노드
                       （오퍼레이션）사이의 연결“nk로 생각할 수
      있다.

다음은 조금더 흥미로운 예제이다：




        5


                                                  23

                     F 戶m `   \
                 F                S
        3
                :input ;

                        b


이 그래프에서는 조금 더 많은 내용이 소개된다. 데이터는 에지의 방향이 의미하는 것

처럼 왼쪽에서 오른쪽으로 흘러간다. 그래서 왼쪽에서 출발해서 그래프를 하나씩 살펴

보자．




                                         계산그래프＜computation graph）소개   - 41


===== PAGE 54 =====
          1.
               시작부분에 그래프 속으로 입력되는 두 개의 값5와3이 있다. 이러한 값들은다
               른그래프로부터 올수도 있고，
                             파일이나사용자에 의해서 입력될수도 있다．
          2. 이 초기값들은두개의 " input" 노드a, b로전달된다．
                                            "input" 노드들은자신이
               입력받은 이 값들을 전달한다. 노드 a는 5를 받아서 같은 값을 다음 단계의 c, d
               노드로 각각 전달하며, 노드b는동일한 일을 값3어］대해서 수행한다．

          3. 노드C는곱셈multipLication 연산을수행한다．
                                         5와3을노드a와b로부터 받아서 곱
               셈 결과인15를 노드 e로 전달한다. 한편 노드 d는 같은 입력값에 대해서 덧셈을
               수행하고，
                   그 결과인8을 노드 e에 전달한다．
          4. 마지막으로그래프의마지막노드인e는또다른" add" 노드이다. 15와8을벋아

               서, 더한 결과인 23을그래프의 출력 결과로 제출한다.


        아래는 위의 그래프를수식으로 적어보았다．


                  α＝ 1꺄m/l; b = input2

                  c= a 'b; d= a+ b

                  e= c+ d


        a =5이고 b= 3인상황쩨서 e를 구하고 싶다면, 아래와 같이 e로부터 역순으로 계산하
        면 된다．


                  a= 5; b= 3

                  e = (a ' b) + (a + b)

                  e= (5 '3) + (5+ 3)

                  e= 15+ 8= 23


        이로써 모든 계산이 완료되었다！여기서 강조해야 할 개념들이 몇 개 있다：

               "input" 노드를사용하는 것이 편리하다．
                                      왜냐하면 " input" 노드는 하나의 입력



!   애APTER 3 텐서플로우 기본


===== PAGE 55 =====
     값을향후에 아주많은 노드들로 전달할수 있기 때문이다．
                                 "input" 노드를사
     용하지 않는다면, 사용자들이 직접 입력값을 그래프 안의 다수의 노드들에게
     모두명시적으로 입력값을전달해야하기 때문이다．
                            "input" 노드를사용함으
     로써 사용자는 한 번만 값을 전달하기만 하면 된다. 이와 같은 그래프의 추상화
     abstracting는나중에 조금 더 살펴볼 것이다．
 ·   Pop Quiz: 곱셈 노드 C와 덧셈 노드 d 중에 어느 것이 먼저 수행될까？지금은 알
     수 없다. 이 그래프로는 어느 노드가 먼저 수행될 지 알수 없다. 어떤 이는 그래
     프를 왼쪽에서 오른쪽으로, 그리고 위에서 아래로 읽어서, 노드 C가 먼저 계산될

     것이라고 생각할수도 있다. 그러나 그래프를 그릴때반대로 노드 C 위에 노드 d
     를 그릴 수도 있다．
               어떤 사람은 이 두 개의 노드가 병행concurrently 처리될수 있
     다고 생각할수도 있다. 그러나다양한구현상의 세부 사항이나 하드웨어 제약으
     로 인해서 언제나 그렇지 않을수도 있다. 실제로는 그 두 개의 노드가 서로 무관

     하게independently 수행된다고생각하는 것이 최상이다. 노드C는노드 d로부터 어
     떤 정보도 필요로 하지 않기 때문에,자신의 연산을종료하기 위해서 노드 d가어

     떤 일을하기를 기다릴 필요가 없기 때문이다. 노드 d도 동일하다. 노드 d도 노드
     C로부터 어떤 정보도 필요로 하지 않는다．
                           이 장의 후반부에 의존성dependency에
     대해서 더 살펴볼 것이다．


다음으로，
    아래에 그래프를조금수정하였다．




                                              26




                                      계산그래프
                                          （computation graph）소개   - 43


===== PAGE 56 =====
    여기에는두 가지의큰 변화가 있다·．

      1. 노드b로부터의 " input" 값3이노드e에전달된다．
       2. 노드e의 " add" 함수가 " sum" 으로교체되었는데, 이는두개 이상의 값을더한

         다는 것을 암시하기 위해서이다．


    노드들사이의 에지를 더하는 방식을 눈여겨보자. 일반적으로, 모든노드는 그 사이에

    얼마나많은 연산이 실행되는지에 상관없이, 그래프 안의 다음의 노드에 값을 전달할수
    있다. 그래프는다음처럼 그릴 수 있는데, 여전히 이그래프는완벽하게 유효하다：



         -－」    )i input ;




                     I        ,

                 ; input ;
                          I




    이 그래프들로부터 우리는 그래프의 입력을추상화하는 것의장점을볼수 있다. 우리는

    그래프 내부에서 어떤 일이 벌어지는지 자세한 내용을 조작할수 있다. 그러나 사용자는
    두 개의 입력 노드에 정보를 전달하기만 하면 된다. 우리는 이러한 추상화를 더욱 심화
    해서 아래와같은 그림을 그릴수 있다．




                         transformatj on


    이렇게 함a로 서，
             노드들의 전체 시퀀스를 입력과출력 집합을 가지는독립적인빌딩 블



CHAPTER 3 텐서플로우 기본


===== PAGE 57 =====
록들로 생각할 수 있다．
            각 조각들의 구체적인 사항들에 대해서 걱정하는 것보다, 여러
계산들을묶는 것으로 시각화하는 것이 더 쉽다．



  （Dependencies)
의존성

노드 사이에 허용되지 않는 연결 형태들이 있다. 대표적인 경우가 해결되지 않는 순환
의존성circular dependencγ을만드는 경우이다．
                               순환 의존성을 설명하기 위해서 의존정이
라는 것이 무엇인지 이야기해보자. 아래의 그래프를다시 보자＝




순환 의존성이란 개념은 명확하다：A라는 노드가 B라는 노드의 계산 결과를 필요로 할
때，
 노드 A는 노드 B에 의존정이 있다고 한다．
                        노드 A, B가 서로에게서 어떤 정보도 필
요로 하지 않을 때 독립적independent이라고 한다．
                               이것을 시각적으로 이해하기 위해서，
아래의 그림에서 mul노드C가계산을종료할수 없다면
                          （어떠한 이류로든）
                                   무슨 일이발
생할지 살펴보자．




    -;'_
                         ,___,




                                        35
           3
               )
                                 ,;/3
                   ;u:
                                             계산그래프
                                                 （computation graph）소개   - 45


===== PAGE 58 =====
             노드e는노드C의 출력 결과가필요하기 때문에, 노드C의 데이터가도착할때까지는 계

             산을수행할수 없고，
                      노드 C의 데이터가도착하기를무작정 기다려야한다. 노드 c, d의
             결과가 직접적으로 최종 add 노드에 사용되기 때문에 노드 e의 의존물이다는 것은명확
             하다．
               그러나 노드 a,b가 노드e의 의존물이라는것은약간불명확할 수 있다. 입력 노드
             중에 하나가그래프의다음함수로 값을 전달하지 못한다면 어떤 일이 발생할까？


                                      a                               c

                         1,
                     5
                                                            ,'\
                                          `,            '         첩
                                                    ,

                              '1`
                     3              mput ; "
                                               』／
                                      b                               d



             그림에서 확인할수 있듯이 input노드중 하나를 제거하면 향후의 모든 연산이 동작하

             지 않는다．
                  이를 의존정의 전이성transitivity of dependency이라고 한다. A가 B에 의존하고，
             B가C에 의존하면 A는 C에 의존한다. 위의 그림에서 마지막 노드 e는 노드 C와 d의 의
             존한다．
                그리고노드C와d가모두input 노드b에 의존한다．
                                          그렇기 때문에마지막노드
             e는 input 노드 b에 의존한다．
                                동일한 방식으로 노드 e가 노드 a에도 의존한다는 것을
             확인할 수 있다. 또한 노드 e가 가지는 의존성들 중에서 구별할 수 있는 차이점이 있

             는데：

               1. 노드 e는노드 C와 d에 직접 의존directly dependent한다．이 말은노드 e가 실행하
                   기 위해서는 노드 C와 d로부터 직접적으로 데이터가 입력되어야 한다는 의미

                   이다．
               2. 노드e는노드a와b에 간접 의존ndirectly dependent한다. 이말은노드a와b의 출
                   력이 직접적으로 노드 e에 입력되지 않J긱 중간에 있는 노드들캥＝드 e에 직접 또
                   는 간접 의존하는）
                            에 입력된다. 이 말은 하나의 노드는 중간에 많은 레이어의 연
                   결 노드들을가지는어떤노드에 간접 의존할수 있다는말이다．



46   -   CHAPTER 3 텐서플로우 기본


===== PAGE 59 =====
마지막으로, 그래프의 출력을 다시 그래프의 앞부분으로 연결하면 어떤 일이 발생하는

살펴보자：


                  a

        5
            : -input :




        3




                           우리는 지금 노드 e의 출력을 노드 b
음, 불행하게도 이 모델은 작동하지 않을 것 같다．
로 거꾸로 연결하려고 하고 있다．
                 이로써 그래프는 사이클cycle이 생겼다．
                                       이로써 노드b
              동시에, 노드 e는노드 b에 간접 의존한다. 이로써 노드 b와
는노드 e에 직접 의존하고，

e는 실행될수 없다. 왜냐하면두 개모두서로의 계산이 끝나기를 기다리기 때문이다．

똑똑한 사람은 노드b와e에 초기값nitial value를 주면 어떨까라고 생각할수 있다 ．그래
프의노드 e의출력에 초기값으로 1을 줘보자．


              a

        5

            谷  {3, 69, . . .
                                                1,23,419, . . .



        3                              ad


                               .   .   }d




처음 몇 단계의 그래프의 반복 과정을 살펴보자. 그래프는 끝이 없는 피드백 순환을 보
인다. 그래프의 대부분의 에지들은무한대로 증가한다. 그러나 텐서플로우와같은 소프



                                            계산그래프
                                                （computation graph）소개   - 47


===== PAGE 60 =====
             트웨어는 이런 식의 무한루프infinite loop를좋아하지 않는다：

               1. 무한루프이기 때문에프로그램의종료가멋지지 않다．

               2. 의존성이 무한개가된다. 각각의반복이 모든 이전의 반복에 의존하기 때문이다．
                  불행하게도 각 노드가한 개의 의존정을 가지는 것이 아니라，
                                                 반복에서 출력값이
                  변경될 때마다 의존성이 늘어난다. 이로써 의존 정보를 추적하는 것을 불가능하
                  게한다．
               3. 이런 시나리오와 같은상횡미 실제 종종 나타나는데, 값이 아주큰 양수 값으로
                  폭발하거나
                      （결과적으로는오버플로우overflow), 아주큰음수값
                                                  （결과적으로는
                  언더플로우underflow), 또는 0에 가까워지는
                                             （각반복이 의미 없어지는）경우가발
                  생한다.


             이런이유로순환의존성circular dependency은 텐서플로우로표현할수 없다. 실제로 이와
             같은모델을사용하는 경우에, 이러한종류의 의존정은유한한 개수의 그래프를복사함
             으로써 흉내simulate낼 수 있다. 각 그래프를 옆으로 나열해서 하나의 출력을 다음의 그
             래프의 입력으로 제공하는방식이다. 이런방식을 보통 그래프를 펼친다unroll라고 한다．

             이를순환 신경망recurrent neural network에서 살펴볼 것이다. 그래프의 펼침을 그림으로
             보기 위해서 순환 의존을5번 펼치면 어떻게 될지 보자：




             이 그래프를 보면, 그래프의 노드와 에지의 시퀀스가 이전의 그래프를 5번 반복하는 것

             과 동일하다는 것을 알 수 있다．
                              원래의 입력값
                                    （그림의 위와 아래에서 각 그래프를 뛰
             어 넘는 긴 화살표）
                       이 각 복사본에게 전달되는 것을 확인하자. 각 그래프의 복사본도
             입력값이 필요하기 때문이다. 이와 같이 그래프를 펼침으로써 명확한 계산deterministic
             computation을보장하면서 그래프의 순환의존성을흉내낼수 있다．




48   -   CHAPTER 3 텐서플로우기본


===== PAGE 61 =====
이제 의존정을 이해하고 있으니까, 의존성을 고려하는 이유를 알아보자. 이전의 예제
                                            노드 C와무관한노드 d
multiplication node어］서 노드 C의 출력만 필요하다고 가정해보자．
와 그래프에서 노드 C 이후에 있는 노드 e도 현재의 그래프에는 포함되어 있다. 그렇다

면노드 d와 e의 출력값이 필요없는 상황에서 그래프의 모든 노드를 계산해야만 할까？
그렇지 않다！노드 C의 출력만 필요한 경우에 모든 노드를 계산하는 것은 시간 낭비라

는 것을 알 수 있다. 그렇다면 문제는, 직접 사람이 말해주는 대신 필요한 노드만을 컴
퓨터가 계산하게 만들려면 어떻게 해야 할까？ 그 대답은 바로 의존성을 사용하라는

것이다！

이 뒤에 숨어있는 생각은아주 간단하다. 우리가 확실하게 해야하는 것은, 각노드가직
접
（간접은 빼고）의존하는 노드들의 리스트를 가지게 해야 한다는 점이다. 최종적으로
우리가 계산해야 하는 노드들을 보관하게 될 현재는 빈 스택stack으로 시작하자. 출력을
계산할노드들로 시작하자. 그 노드들은반드시 계산해야 하니까스택에 추가한다. 출력
노드들의 의존정 리스트를 살펴서, 그들 모두를 스택에 추가한다. 이제 그 노드들을 모
두 살펴보고，
      그들의 직접 의존 노드들을 스택에 추가한다. 이런 패턴을 그래프를 거꾸

로 가면서 의존성이 없어질 때까지 수행한다. 이런 방식으로 우리가 수행해야 하는
                                           （그
리고 수행할 필요가 있는 노드들만）
                  노드들을 구할수 있다．
                             또한 스택은 우리가 반복해
서 수행할 때 스택에 있는 순서로 실행하면 가능하도록 정렬되어 있다. 주의해야 하는
사항은 이미 계산된노드의 값을메모리에 저장하는 것이다. 이런방식으로 같은노드를
여러 번 계산하지 않아도 된다. 이런방식으로 우리의 계산을 가능한 가볍게 함으로써，
큰그래프의 계산 시간을줄일수 있다．




텐서플로우에서 계산 그래프 정의하기


이 책에서 우리는 다양하고 상당히 복잡한 머신 러닝 모델들을 살펴볼 것이다. 그러나，
텐서플로우에서 이런다양한 모델들을 정의하는방법은 비슷한 패턴이 있다. 다양한 수
학적인 개념과구현 방법을 배우는 과정에서, 텐서플로우가 작동하는 핵심 패턴을 이해




                                       텐서플로우에서 계산그래프정의하기   - 4'


===== PAGE 62 =====
           하는것이 어려울것이다. 다행스럽게도 이러한워크플로우는2단계로단순하다：

             1. 계산그래프정의하기
             2. 그래프를데이터로실행하기


           그래프가존재하지 않는다면, 그래프를실행할수조차 없다. 명확하다. 텐서플로우에서

           제공하는 거대한 기능들은 실제 코드를작성할때 아주 부담되는 일이 될수 있다. 이 워
           크플로우의 한부분씩나누어서 생각함으로써, 당신의 코드를 더욱잘구조화할수 있을
           뿐만아니라작업한다음단계로나아가는 것을도와줄 것이다．

           이 섹션은 그래프의 정의에 집중하고, 다음섹션에서 그래프의 실행을살펴보자. 마지막
                           여러 번 실행하면서 변화되는 그래프를 생성하는 법과
           에서는 이 두 단계를 결합하고，
           다른데이터를 사용하는방법을살펴보자．



           첫 번째 텐서플로우 그래프 만들기

           아래의 그래프는 이전섹션에서 보았었다：


                       (

                                              -   23.-*


                   3




           텐서플로우 코드는다음과같이 표현된다．




50 -   CHAPTER 3 텐서플로우 기본


===== PAGE 63 =====
import tensorfiow as tf
a = t-F.constant(5, name= 'input_a")
 b = t-F.constant(3, name="input_b")
 c = t-f.mul(a,b, name="mul_c")    WJ＼나峀
d = tf. add(a,b, name="add_d")
 e = tf. add(c,d, name="add_e")



이 코드를한줄씩 살펴보자．
             첫 번째 줄에 import문장이 있다．

import tensorfiow as tf



이 문장은 텐서플로우 라이브러리를 임포트하고 이름alias을 if라고 한다. 여러 번 사용
할것이기 때문에 " tensorfiow" 라고하는것보다 " tf'라고하는것이 훨씬 쉽다．

다음으로，
    처음의두 변수 대입문을 보자：

 a = tf. constant(5, name="input a ')
 b = tf. constant(3, name="input-b ')



여기서 " input" 노드a,b를정의한다．
                       이줄들은텐서플로우오퍼레이션tf.constantq
를 사용한다．
      텐서플로우에서 그래프 상의 계산 노드를 오퍼레이션Operation/Op이라고
  op는 0개 이상의 텐서 객체를 입력으로 받아서，
한다．                         0개 이상의 텐서 객체를 출력한
다. 오퍼레이션을 생성하기 위해서 연관된 파이썬 생성자constructo를 호출한다. 여기
서는tf.constant(）
              가 " 상수constant"를생성하는데, 하나의 텐서 값을벋아서 연결된
노드에 같은 값을 출력한다. 편리하게도 이 함수는 스칼라값 5와3을 텐서 객체로 자동
으로 변경해준다. 우리가 생성하는 노드에 식별자identifie를 부여하기 위해서 문자열인
name 파라미터를 적을수도 있다．


 오퍼레이션이나 텐서 객처를 지금 이해하지 못한다고 해서 걱정하지 말자. 이 장의

 후반부에 자세하게 살펴볼 것이다．




                                           텐서플로우에서 계산그래프 정의하기   - 51


===== PAGE 64 =====
          c = t-F.mul(a,b, name='mul_c')
          d = tf.add(a,b, name="add_d")


         이제 그래프의 다음 두 노드를 보자. 이전에 정의했었던 노드들을 사용한다. 노드 C는
         tf.mul 오퍼레이션을사용하는데, 두 개의 입력을 받아서 그들의 곱을출력한다. 비슷
         하게 노드 d는 t-f.add 오퍼레이션을 사용해서 두 개의 입력값을 더한다. 이 두 오퍼레
         이션에도name을부여하자. 노드와 별개로 그래프의 에지를 정의할 필요가 없다. 텐서
         플로우에서 노드를만들때, 그오퍼레이션이 필요로하는모든 입력을포함하기 때문에

         소프트웨어가알아서 연결을만들어준다．

          e = tF.add(c,d, name="add_e")


         이 마지막 줄은 그래프의 마지막 노드를 정의한다. 노드 e는 tf. add를 node d와 비슷
         한방법으로 사용한다. 그러나 이번에는 노드 C와d를 입력으로 사용한다．

         이로써 작기는 하지만 우리의 첫 번째 그래프를완벽히 정의하였다！파이썬스크립트나
         쉘에서 위를 실행한다면, 실행은 되지만 실제로는 어떤 일도 하지 않는다. 기억하자！이
         것은단순히 프로세스에서의 정의definition이다. 그래프를 실행한다는 것이 어떤 것인지

         잠깐살펴보기 위해서 다음의두줄을 추가하자．

          sess = t-F.Session()
          sess.run(e)


         이것을 파이썬 쉘이나Jupyter/iPython Notebook과 같은 인터랙티브 환경에서 실행
         한다면, 아래의 출력을볼것이다．

          >>> sess = tf.Session()
          >>> sess.run(e)
          23


         이 정도면충분할 것이다. 실제로 이를 실행해보자！




52 - CHAPTER 3 텐서퓰로우 기본


===== PAGE 65 =====
           연습문제： 텐서플로우에서 기본 그래프 만들기

이제 실전이다！이 연습문제에서 처음으로 텐서플로우 그래프를 작성하고 실행해 보자．
그리고 蛋 jAi보느라는 아주유용한툴을 접하게 된다．
                            이 부 분 을 마치면 기본적인 텐서플
로우 그래프를만들고 실험하는데 조금은 편안함을느낄 것이다．

이제 텐서플로우로 정말 그래프를 정의해보자. 텐서플로우를 설치하고 자신이 사용하

는 파이썬 사용 환경
          （Virtualenv. Conda, Docker) 중에서 사용하는 환경을 시작하자．
텐서플로우를 소스 코드를 통해서 설치하였다면, 현재 본인의 콘솔에서 현재 작업하는

디렉터리가 텐서플로우 소스 폴더가 아니어야 한다는 것에 주의하자. 그렇지 않으면 파
이썬이 라이브러리를 임포트할 때 동작하지 않을 수 있다. 이제, 인터랙티브 파이썬 세

      쉘에서 Jupyter notebook 명령어로 Jupyter Notebook을 사용하거나，
션을시작하자．
                    본인이 편하게 사용하는 인터랙티브 파이썬 환경이
python으로 파이썬 쉘을 시작하자．
있다면 어떤 것이든 사용해도 된다．


  파이썬 파일로 작성하고, 인터랙티브하지 않게 실행할 수도 있다. 그러나 이렇게 하면 그
  래프의 실행결과가 자동으로 출력되지는 않는다. 그래프의 결과를 보고 즉시 피드백을 받
  고, (Jupyter Notebook의 경우에는）에러를 수정하고, 순간 순간 코드를 변경할 수 있으려
  면, 인터랙티브 환경에서 실행하기를 강력히 추천한다. 또한 인터랙티브 텐서플로우는 재
  미있다！


먼저，
  텐서플로우 라이브러리를 로드한다．
                   아래와같이 import 문장을 적자：

  import tensorfiow as tf

몇 초 후에 임포팅을마치고 코드의 다음 줄이 시작될 것이다. GPU 사용 가능한 텐서플
로우를 설치했으면 CIJDA 라이브러리도 임포트 되었다는 공지를볼 것이다．

아래와 같은 에러를 보면：

 ImportError: cannot import name pywrap-tensorflow




                                                 텐서플로우에서 계산그래프 정의하기   - 53


===== PAGE 66 =====
           텐서플로우 소스 폴더에서 인터랙티브 환경을 시작하지 않았다는 것을 확실히 하자，

           아래와같은 에러는：

             ImportError: No module named tensorfiow

           텐서플로우가 정확히 설치되었는지 다시 한 번 확인하자. Virtualenv나 Conda를 사용
           한다면, 인터랙티브 파이썬 추ㅍㅌ웨어를 시작할 때 텐서플로우 환경이 액티브한지 확
           인하자. 여러 개의 터미널termifla｛을 사용할 때, 하나의 터미널은 액티브한 환경을 가지
           고,다른 터미널은 그렇지 않을수도 있다．

           임포트가정상적으로 되었으면, 다음문장으로가자：

             a = tf. constant(5, name="input_a")
             b = tf. constant(3, name="input_b")


           위에서 사용한 것과 같은 코드이다. 값이나name 파라미터를 원한다면 바꿔보자. 이 책

           에서는 일관성을 위해서 같은값을 사용할 것이다．

             c = t-F.mul(a,b, name="mul-c')
             d = tf. add(a,b, name="add_d")


           이제 실제적인 수학적 함수를 실행하는 첫 번째 Ups를 보자 tf.mul이나tf.add에 싫

                                       （각각뺄셈, 나눗셈，
           증나면tf.sub, tf. div, tf. mod 등         나머지 연산）
                                                       으로 바꿔보자．


             {tf . di v](https://www.tensorflow.org/versions/master/ap댜iocs/python/rnath_ops.
             htrnl#div＞는 사용되는 입력값의 타입에 따라서 정수 나눗셈이나 실수 나눗셈을 수행한다，
             확실하게 실수 나눗셈을 원한다면 t-F .truediv를 사용하자．



           아제 마지막 코드이다：

             e = tf. add(c,d, name="add_e' )


           이제까지의 오퍼레이션들은 출력이 없었다．
                                단순히 그래프에 Ups를 추가했을 뿐이다．




54 -   CHAPTER 3 텐서플로우 기본


===== PAGE 67 =====
                       珊꺅斟凞呼鞋馨驪꾼和多


실제로 계산은 일어나지 않는다. 그래프를 실행하기 위해서 텐서플로우 Session이 필요

하다．

 sess = tF.Session()

Session 객체는 실행될 때 그래프 감독을 책임지며, 그래프를 실행하기 위한 기본적인
인터페이스이다. Session 객체에 대해서는 이 연습문제 후에 깊이 살펴본다. 그 전에는
텐서플로우에서는 코드를 실행하기 위해서는 Session이 필요하다는 정도로만 알고 넘
어가자. Session을 ses$ 변수에 할당하고, 나중에 사용할수 있다．

  InteractiveSession: t-F.Session의 약간 변형된 tf. InteractiveSession이
  있다. 인터랙티브 파이썬 소프트웨어에서 사용할 목적으로 만들어져서 코드를 실행하는
  조금은 간편한 방법을 제공한다. 나쁜 점으로는, 파이썬 파일로 텐서플로우를 쓸 때는 조
  금 불편하다. 그리고 텐서플로우의 초보자가 알아OF 하는 사항을 보이지 않게 한다. 또한
  마지막으로, 많은 키 입력을 저장하지 않는다. 이 책에서는 t-F. Session을 사용할 것이다．


 sess.run(e)

이 줄을 통해서 마침내 결과를 확인할 수 있다.
                        ＇이 코드를 실행하면 그래프의 출력 결과
를 볼 수 있다. 이 예제 그래프에서의 출력은 23이다. 만약 함수를 변경하였다면 사용한

함수에 따라서 달라질수 있다. 여기가끝이 아니다. 그래프의 다른 노드를 sess.run( )
으로 실행해보자．

 sess.run(c)

이 문장을 실행하면 C의 중간 결과를 확인할 수 있다
                            （이 코드 예제에서는 15). 텐서플로
우는 당신이 만든 그래프에 대해서 어떠한 가정도 하지 않는다. 실제로 그래프의 어떤
오퍼레이션에서도「un( ）을사용할수있다．
                     op를＄ession· run( ）에게 전달할때，
                                                                           三
실제로 텐서플로우에게 말하는 것은 " 여기에 내가출력하고 싶은 노드가 있다. 이 노드
를 실행하기 위해서 필요한 모든 오퍼레이션들을 실행해줘" 라는 것이다. 여기서 각자                             !
시간을들여 다양한노드들의 값을출력해보자．




                                             텐서플로우에서 계산그래프 정의하기     - 55


===== PAGE 68 =====
    훌륭하다！이제 우리는 Session이 활성화되어 있고 그래프를 정의했다. 우리가 처음 그
    래프를 그렸던 것과 동일한지 그래프를 시각적으로 그려보자. 텐서플로우와 같이 설치
    된 렌서보드TerisorBoard가 이 역할을 한다. 텐서보드를 사용하기 위해서 아래와 같이 한
    줄을추가한다· k-c. 如，   「" J"*c' A晧，
                   ，. m
                  M펴
      writer = tf . train.SumniaryWriteN ' ./my_graph' J sess.graph)

    이 코드를 분석해보자. 텐서플로우의 SumniaryWrite
                                    「라는 텐서플로우 객체를 생성하
    고, 이것을write
              「 변수에 할당한다. 이 연습문제에서는 Sunimarywrite
                                                「에서는 더 이

    상의 일은 하지 않는다. 그러나 향후에는 이를 데이터를 저장하고 그래프를 통계값들을
    요약하는용도로 사용할 것이다. 그래서 변수에 할당한 것이다. SummaryWrite
                                                 「를 초

    기화하기 위해서 두 개의 파라미터를 전달한다. 첫 번째는 그래프 명세graph description
    가 저장될 디스크의 디렉터리 문자열이다. 이 예제에서는 파일들이 파이썬을 실행되는

    디렉터리 내부에 "mygraph" 디렉터리에 저장될 것이다. 두 번째는 Session의 gra肉
    속성이다. 텐서플로우에서 정의된 그래프의 매니저로써 tf. Session 객체는 그들이 추
    적하는 그래프의 레퍼런스reference인 graph 속성을 가진다. 이것을 SummaryWriter

    에 전달함으로써 " my_graph" 디렉터리에 그래프의 명세를 출력하는 것이다．
    SummaryWriter 객체는 초기화될 때 그 즉시 이 데이터를 출력한다. 그래서 코드의 이
    줄을 실행하만 바로 텐서보드를 시작할수 있다．

    터미널에서 다음의 명령어를 입력하자 현재 작업 디렉터리working directory가파이썬 코
    드를실행한곳과동일해야한다
                （"my_graph" 디렉터리가 리스트에 있는 것을볼수 있
    어야한다）
        .

      $ tensorboard --logdir="my_graph"

    콘솔에 어떤로그 정보가출력될 것이다．
                       그리고 'Stailing TensorBoard on port 6006"
              "my_graph" 디렉터리에 있는데이터를이용해서 텐서보드
    이라는메시지가나온다．
    서버를 실행한 것이다. 디폴트로 서버는 텐서보드에 접속하기 위해서 포트 6006으로 시
       브라우저를 실행해서 http://localhost:6006을 입력하자 오렌지 색과 흰색으로
    작한다．




CHAPTER 3 텐서플로우 기본


===== PAGE 69 =====
이루어진 화면이 나타날 것이다．




                         ㅒ. ·驪＝．■山 나m fm1贓

                         m며月ㅂ* .1"11臘

                           ' ＇에r나뉘·n ■11口1n .1 .C/.r m뱁a 1.叩빼〃*'．
                                                                겨卜m
                           . Tr－物｀  dLm h닙邪．      nm1m1

                         ' 烟 m m썲1.U8叫 Tm·y如  ＇d ·M H돈m m f．
                                                           넌.U' m빎t口叱d d'.
                         翩d 1m 驢 朴M月닒m nm1 ChaC노 에∥柚 8f^n1在 ·nd .1m叩a 胞
                         7m디HHnmH 치mㄱ‘ㅢ


     =                   ' 柳 mn* T1r翩物·쾨｀mn
                         楢 旺月DML口nm驢盤』  y，
                                          「m'1d여－把 m" " ~m m 出，   m며
                                                 惻·二i1너C1m·거汁 `mm . m｀
                                         욧홰也 랑1工1』                   떫




"No scalar data was found" 라는 경고 메시지에 놀라지 말자. 이것은 단지 텐서보드
를 위한 어떤 정리된 통계 정보도 저장하지 않았다는 것을 의미한다. 이 화면은 우리가
SummaryWriter를통해서 텐서플로우에게 저장하라고말한정보를보여준다．
                                        다른 정

보를 저장하지 않았기 때문에 이 이상출력할 것이 없다．
                             페이지의 상단에 " Graphs" 링
크를 클릭하자. 아래와 같은 화면을볼수 있다．




     ∼                add_e
     솝느 ● 戶』
           →
         .-




                                            J一




                                                                      dd_d
                                         nput_a
                                        input_b 0




그래프가 너무 작다면 마우스 휠을 움직여서 텐서보드에서 확대할 수 있다. name 파라




                                                                             텐서플로우에서 계산그래프정의하기   - 57


===== PAGE 70 =====
           미터에 의해서 부여된 이름을 확인할 수도 있다. 노드를 클릭하면 연결된 다른 노드와
                          input 노드 a와b가 복제되어 있는 것처럼 보인다．
           같은 정보를 확인할 수 있다．                            그러나

           "input a" 레이블위로마우스를움직이거나클릭하면둘다함께표시되는것을알수
           있다．
             이 그래프는우리가그렸던 그래프와똑같아보이지는 않지만，
                                         input 노드가두 번
           보이는 것 빼고는동일한 그래프이다．

           당신의 첫 번째 텐서플로우 그래프를 작성하고 실행해보았다. 그리고 몇 줄 안되는 코드
           로 텐서보드로 확인하였다．

           연습 삼아서, 몇 개의 노드를 추가하거나, 다른 수학 연산을 사용하거나, 더 많은
           tf. constant 노드를 추가 해보자. 당신이 추가한 노드를 실행해보고, 그래프 상에서

           데이터가흘러가는 원리를 본인이 정확히 이해하고 있는지 확인해보자．

           그래프를그린후에 세션을닫자：

             sess.close()

           기술적으로는, session 객체는 프로그램이 종료되면
                                        （인터랙티브한 경우에는 파이썬
                        ) 자동으로 닫힌다. 그러나 명시적으로 $ession을 닫아주
           커널을 닫거나에 시작하면）
           는 것이 좋다．

           아래는 예제에서 사용하는 값을 이용한 튜토리얼의 전체 코드이다：

             import tensorfiow as tf

             a = t-f.constant(5, name="input_a')
             b = tf.constant(3, name="input_b')
             c = tf.mul(a,b, name="mul_c")
             d = t-F.add(a,b, name="add_d")
             e = tf.add(c,d, name='add_e")

             sess = tf.Session()
             output = sess.run(e)
             writer = tF.train .SummaryWriter( ' ./my_graph ' , sess .graph)
             sess.close( )
             져 Y, rf一 / p ,




58 ㅣ   CHAPTER 3 텐서플로우 기본


===== PAGE 71 =====
텐서가 무엇일까？

계산그래프의 기본을 공부할 때는 스칼라숫자가 적당하다. 이제 우리는 플로우flow의
개념을대략적으로 알고 있기 때문에 이제 텐서tenso
                            「를 이해해보자．

텐서는 단순하게 매트릭스matrix의 n－차원 추상화이다. 그래서 1차원 텐서는 벡터와 동
일하고, 2차원텐서는매트릭스와동일할것이다. 그리고그이상은 "N차원텐서" 라고

할수 있다. 이를 염두에 두고우리의 위의 예제를텐서를사용해서 수정할수 있다．




       r   input




       H
두 개의 별도의 input노드를가지는 대신，
                       우리는 이제 숫자들의 벡터
                                    （1차원텐서）
                                          를가
지는하나의 노드를사용한다. 이 그래프는이전의 예제에 비해서 몇개의 장점이 있다：

  1. 사용자는하나의 노드에 입력을전달함으로써 그래프사용을간단하게 한다．
  2. 입력 노드에 직접적으로의존하는노드들은이제 두개가아니라하나의 의존성

    만을고려하면 된다．
  3. 원한다면그래프를 어떠한 길이의 벡터를 입력받을수 있도록수정할수 있다．

    이것은 그래프를 더 융통성있게 사용할수 있게 해준다. 반대로 우리는 그래프에
    엄격한 요구사항을강제할 수 있는데 입력이 길이 2
                             （또는 원한다면 어떠한 길이
    라도）
      로 제한할수도 있다．


위의 코드를수정하면텐서플로우에서 다음과같이 수정할수 있다．




                                  텐서플로우에서 계산그래프정의하기   - 59


===== PAGE 72 =====
     import tensorfiow as tf


     a = t-F.constant([5,3], name="input_a')
     b = tf.reduce_prod(a, name="pr0d_b")
     c = tf.reduce_suni(a, name= 'sum_c")
     d = t-f.add(b, c, name="add_d")



    변수 이름을수정한것 이외에 두 개의 큰 변화가 있다：

      1. 별개의 노드인 a와b를 결합된하나의 노드
                              （a）
                                로 교체하였다. 숫자들의 리스트를
         전달하는데 tf. constant는 이제 1차원텐서로 변환될수 있다．
      2. 스칼라 값을 입력받기 위해서 사용된 곱셈과 덧셈 오퍼레이션은, 이제
         tf. reduce_prod( ）와tf.reduce_sum( ）이다. 이 함수들은텐서를 입력받으
         면, 모든값을입력벋하서 그값들을모두곱하거나더한다．


    텐서플로우에서 노드 사이에 전달되는 모든 데이터는 텐서 객체이다. 텐서플로우 오퍼
    레이션은 표준 파이썬 자료형
                  （integers, st血1gs 등）
                                     을자동으로 텐서로 변환한다．
                                                   텐서
    객체를 수동으로 생성하는다양한 방법이 있다
                          （즉，
                            외부의 데이터 소스로부터 읽어들일
    필요없이）
        . 몇 가지 사항을 조금 더 살펴보자．



    파이썬 기본 자료형
             （Python native types)

    텐서플로우는 파이썬의 숫자numbers, 불리언booleans, 문자열strings, 이들의 리스트 모
    두를 사용할수 있다．
              하나의 값은 0－차원텐서
                          （스칼라）
                              로 변환되고, 값들의 리스트list of
    values는 1－차원 텐서
                  （벡터）
                     로 변환되고, 값들의 리스트의 리스트list of list는 2．
                                                        차원 텐서
   （매트릭스）
        로 변환되는 식이다. 이를 설명하는 예를다음에서 보자．




애APTER 3 텐서플로우 기본


===== PAGE 73 =====
t-0 = 50                             # Treated as .－【） Tensor, or "scaLar"


t-i = ["apple", "peach", "grape"]    # Treated as ㅏ   Tensor, or "vector "


t_2 = [[True, False, False],         # 了reated α5 2-z) Tensor, 0r "matrLx"
      [False, False, True],
      [False, True, Falsen


t-3 = [[ [0, 0], [0, 1], [0, 2] ]J   1 Treated as 3-D Tensor
     〔 [1, 0], [1, 1], [1, 2] ]J
     [ [2, 0], [2, 1], [2, 2] ］〕




파이썬 자료형을 사용해서 텐서 객체를 지정하는 것은 쉽고 빠르다. 그리고 또한 아이
디어를 구체화할 때1 좋다. 그러나 여기에 중요한단점 또한 존재한다. 텐서플로우는마
음대로 사용할 수 있는 아주 많은 자료형이 있지만, 파이썬의 기본 자료형은 당신이 사
용하려는 자료형을 명확하기 표현하기에는 부족하다. 그래서 텐서플로우는 당신이 사
              문자열string과같은자료형은 명확한데，
용하려는자료형을유추해야한다．                    그러나다른
자료형에서는 유추가 불가능할수도 있다．
                    예를 들어，
                         파이썬에서는 모든 integer는 동
일한자료형이다．
       그러나 텐서플로우는 8－비트，
                      16．
                        비트，
                          32－비트，
                               64－비트 integer 형을
사용할수 있다. 데이터를 텐서플로우에게 전달할때 데이터를 적절한 자료형으로 변환
하는 방법들이 있다．
          그러나 복소수comptex numbers와 같은 자료형은 여전히 정확하게
선언하기 어려울 수도 있다. 이런 이유로 인하여 Tensor 객체를 iumPy 배열로 생각하
는것이 일반적이다.




                                                텐서플로우에서 계산그래프정의하기            - 61


===== PAGE 74 =====
                         텐서플로우 데이터 형
                                   （TensorFiow data types)

                             （불리언）
                우리는 아직 boolean   이나 string
                                         （문자열）형은 보지 않았지만, 텐서를 어떤 데이
                터든지 구조화된 형식으로 저장할 수 있는 수단으로 생각할 수 있다. 수학에 사용되는 함
                수
                （function）
                         들은 문자열에는 작동하지 않으며, 문자열의 파싱
                                                  （parsing) 함수들은 숫자에
                                             （numerics) 이상을 다룰 수 있
                는 당연하게 작동하지 않는다. 그러나 텐서플로우는 숫자
                다는 것을 알아야 한다. 아래는 텐서플로우에서 사용할 수 있는 모든자료형이다．




  Data type (dtype)          Description

                             32-bit floating point

                             64-bit floating point

                             8-bit signed integer

                             16-bit signed integer

                             32-bit signed integer

                             64-bit signed integer

                             8-bit unsigned integer

  tf. string                 String (as bytes array, not Unicode)

                             Boolean

  ti. comp1ex64              Complex number, with 32-bit floating point real portion.
                             and 32-bit floating point imaginary portion

  tf. qint8                  8-bit signed integer (used in quantized Operations)

  ti. q1rit32                32-bit signed integer (used in quantized Operations)

  tf. quint8                 8-bit unsigned integer (used in quantized Operations)




62 -   CHAPTER 3 텐서플로우 기본


===== PAGE 75 =====
NumPy 배열

텐서플로우는 N차원 배열을 다루기 위해 제작된 과학 계산용 패키지인 NumPy와 아주

            그래서 NumPy에 대한 경험이 없는 사람은 관련된 튜토리얼
밀접하게 결합되어 있다．
                           NumPy는 이제 데이터 사이언스
이나 다양한 관련 지식을 접하기를 강력하게 권한다．
data science의 실질적인 표준이 되었기 때문이다．
                               텐서플로우의 자료형도 NumPy의 자
료형에 기반을두고 있다. 실제로 np.int32 == tf. int32는True이대. 모든 종류의

NumPy 배열은 어떤 텐서플로우 op에도 전달될 수 있다．이렇게 함으로써 필요로 하
는 자료형을 최소한의 노력으로 지정할수 있다는장점이 있다．


 문자열 데이터 형
         （String data types)
 숫자와 불리언 자료형에 대해서는 텐서플로우와 NumPy 자료형이 정확히 일치한
 다. 그러나 문자열 자료형에는 문제가 있다. tf. string은 NumPy가 문자열을 다루
 는 방법으로 인해서 NumPy에는 정확히 일치하는 자료형이 없다. 그러나 텐서플로
 우는 NumPy의 문자열 배열을 정확하게 임포트.mport）
                                 할 수 있다. 단지 NumPy에서
 dtype을 명시하지만 않으면 된다．



보너스로，
    그래프를 실행하기 전 또는 후에，
                     numpy 라이브러리의 기능 들 을 사용할 수
있다．
  왜냐하면 Session, run이 반환하는 텐서들은 NumPy 배열들이기 때문이다．
                                               아
                       （위와동일한 예제이다）
래는 NumPy 배열들을 생성하는방법을보인다          .


import numpy as np # Don』t forget to import NumPy/


# e-D Tensor with 32-bit integer data tyPe
t_0 = np.array(50, dtype=np.int32)


# 1-D Tensor with byte string data tyPe
# Note: don't e쟈,Licit勻／ speciJy dtype when using strings in NumPy
t_1 = np.array(["apple", "peach", "grape"])


# 1-D Tensor with bo九ean data type




                                                 텐서플로우에서 계산그래프 정의하기   - 63


===== PAGE 76 =====
     t_2 = np.array([[True, False, False],
                     [False, False, True],
                     [False, True, False]],
                      dtype=np. bool)


     # 3-D Tensor with 64-bit integer data type
     치3 = np.array([[ [0, 0], [0, 1], [0, 2] 〕J
                     [ [1, 0], [1, 1], [1, 2] ],
                     [ [2, 0], [2, 1], [2, 2] ]],
                     dtype=np . int64)




     텐서플로우는 NumPy 자료형을 이해할 수 있도록 디자인되었지만, 그 반대는 참
          이 아니다. 따라서 실수로라도 NumPy의 배열을 t-f.int32로 초기화하려고 하
     (true）
     지 말라！



    e·     기술적으로는NuniPy 또한자료형을자동으로감지할수 있다．
                                         그러나텐서 객쳬가 가
           질 숫자형에 대해서는 명확하게 정의하는 버릇을 가지는 것이 좋다. 거대한 그래프를
           다룰 때 어떤 객체가 TypeMismatchErro
                                      「를 발생하는지 찾아야 하는 불낭사를 원하
           지는 않을 것이기 때문이다. 하나의 예외는 문자열을 다룰 때이다. 문자열 텐서를 생성
           할때 dtype을사용하지 말라．

                        衫．
    텐서 모양
        （Tensor shape)
                   乙   ＼∼－




    텐서플로우 라이브러리에서 텐서의 모양shape을 참조하는 함수나 오퍼레이션을 자주
    보게 될 것이다．
            텐서플로우에서 모양이라는단어는텐서의 차원과각차원의 크기를나
    타낸다. 텐서 모양은 파이썬 리스트일 수도 있고, 정수들의 정렬된 집합을 포함하는 튜

    플tuples일수도 있다. 차원의 개수만큼의 숫자들이 리스트 안에 있을수도 있는데, 리스
    트 안의 각숫자는 각차원의 크기를 나타낸다. 예를들어, 리스트 [2, 3］
                                            은 첫 번째 차
    원이 크기가2이며, 두 번째 차원은 길이가3인 2차원텐서를 의미한다. 괄호 ( ）로 감싸
    진각 튜플이나 대괄호 [ ］로 감싸진 리스트들이 텐서의 모양을 정의하기 위해 사용된



CHAPTER 3 텐서플로우 기본


===== PAGE 77 =====
다. 자세한 설명은 아래를 참고하자：


# Shapes that specify α O-D Tensor (scαLor)
# e.g. any singLe number: 7J 工J 3J 4J etc.
s_0_iist = [1
s_0_tupie = 0


# Shape that describes α vector of Length 3
# e.g. [1, 2, 刃
s_i = [3]


# Shape that describes α 3-by-2 matrix
# e.g rfl J2力
#       r3, 47J
#       f5, 6刀
s_2 = (3, 2)


각 차원에 고정된 길이를 명시할 수 있을 뿐만 아니라, 각 차원의 값으로 None를 넘겨
줌으로써 가변적인 길이를 지정할 수도 있다. 뿐만 아니라, None을 포함하는 리스트나
튜플을 사용하는 대신 None 값을 모양으로 전달하면, 텐서플로우는 어떤 모양의 텐서
도만들수 있다. 즉, 몇 차원이든또한각차원의 길이가 어떤 것이든만들수 있다．


# Shape for α vector （〕
                      f αny Length:
s_i_flex = [None]


# Shape for α matrix 枋at is any amount af rows taLL' and 3 coLumns wide:
 s_2_flex = (None, 3)


# Shape 0f α 3-D Tensor with Length 2 in its first dimension, and variabLe-
# Length in its second and third dimensions:
s_3_flex = [2, None, None]


# 5hape thαt c《기兀d be αny Tensor
s_any = None




                                                 텐서플로우에서 계산 그래프 정의하기          - 65


===== PAGE 78 =====
    그래프의 중간에서 텐서의 모양을 보고 싶다면, tf. shape 오퍼레이션을 사용하면 된

   다. 이 오퍼레이션은텐서 객체를벋아서 1nt32 벡터로 반환해준다．


     import tensorfiow as tF

     # . . . creote some sort of mystery tensor


     # Find the shape of the 끼／5tery tensor
     shape = tf. shape(mystery_tensor, name="mystery_shape')


    tf. shape 오퍼레이션 또한다른 오퍼레이션 처럼 Session의 내부에서 실행되어야 동
    작한다．

    REMINDER: 텐서는매트릭스의 수퍼셋
                         （superset）
                                  일뿐이다！



    텐서플로우 오퍼레이션

    텐서景로우 오퍼레이션TensorFiow Operations: 0ps은 텐서 객체에
                                                （또는 텐서 객체를 사용

    하여서）계산을수행하는노드이다. UPs는 계산후의 결과로써 그래프의 이후단계에서
                                  오퍼레이션을 생성하기 위해
    다른ops에 의해서 사용될 0개 이상의 텐서를 반환한다．
                               이때 생성자는 input으로 계산을 위해 필
    서 파이썬에서 생성자constructo를 호출한다．
    요한 텐서 파라미터parameters를 받J긱 또한오퍼레이션을 정확하게 생성하는데 필요한
    부가적인 정보인 속성attributes이 필요하다. 그러면 파이썬 생성자는 오퍼레이션의 출력
    (0개 이상의 텐서 객체）                    이 출력은다른오퍼레이
                 을다룰수 있는 핸들handLe을반환한다．
    션이나 Session,run에 전달될수 있다．


     import tensorflow as tf
     import numpy as np

          （九ize some tensors to u5e in C《〕爪βutαtton
     # mnitt
     a = np. array([2, 3], dtype=np.int32)
     b = np.array([4, 5], dtype=np. int32)




CHAPTER 3 텐서플로우 기본


===== PAGE 79 =====
# Use 'tf.add()' to tniti （冗ize an "add" Operation
# The variabLe ' C ' WiLL be α ham九e to the Tensor output of this Op
c = tf.add(a, b)



 0개의 입력, 0개의 출력 오퍼레이션
 입력이 0개 그리고 출력도 0개인 오퍼레이션이 있다. 0ps는 단순한 수학적인 계산
 이상으로써, 상태를 초기화하는 등과 같은 일에 사용된다. 이 장에서는 이러한 수학
 적 오퍼레이션 이외의 오퍼레이션을 살펴볼 것인데, 당분간은 모든 노드들이 다른 노
 드들과 꼭 연결될 필요는 없다라는 점을 기억하자．



input과 attribute와 더불어，
                     각오퍼레이션의 생성자는문자열 파라미터인 name을 입
력으로 벋빠들인다. 위의 예제에서 본 것처럼, name 파라미터를 사용함으로써 문자열
로특정 op를참조할수 있는장점이 있다．

c = tf. add(a, b, name="niy_add_op")


이 예제에서 " my_add_op" 이라는문자열을add 오퍼레이션에 붙였다．
                                         이 이름은 텐서
보드와같은툴에서 사용할수 있다．


 그래프 안의 다른 오퍼레이션에 동일한 name을 사용하고 싶은 경우도 있을 것이다．
               （prefix）
 이러한 경우에 일일이 접두사      나 접미사〈posttix）
                                   를 붙일 필요없이, 프로그래밍
 을 하는 것처럼 오퍼레이션들을 뭉치기 위해서 name_scope를 사용할 수 있다. 이
 장 끝부분의 연습 문제에서 name scope 사용법을 배워보자．




                                                 텐서플로우에서 계산그래프정의하기     - 67


===== PAGE 80 =====
                               연산자 오버로딩
                                      （overloaded operators)

              텐서플로우도 일반적인 수학 연산자들을 오버로딩함으로써 곱셈, 덧셈, 뺄셈 둥의 일반
              적인 연산들을 더욱 간결하게 만들어준다. 연산자의 하나 이상의 아규먼트
                                                    （argument）
                                                             가
              텐서 객체라면, 텐서플로우오퍼레이션이 호출되고그래프에 추가된다. 예를들어, 아래
              와 같이 두 개의 텐서를 쉽게 더할 수 있다．


              # Assume that ' α ' and ' b ' are ' Tensor ' obJects viLth matching shapes
              c= a+ b

              아래는 텐서에 대한 연산자 오버로딩의 목록이다：


  단항 연산자
       （unary operators)

  오퍼레이터                    텐서 오퍼레이션              설명

  -   x                    tF.neg()               x의 각 요소의 음수화된 값을 반환

  ∼X                       tf. logical_not()      x의 각 요소의 논리 연산 NOT 결과를 반환．
                                                  tf. bool의 dtype을 가진 텐서 객체에만 사용할
                                                 수 있음．

  abs(x)                   tf. abs()              x의 각 요소의 절대값을 반환．



  이항 연산자
       （binary operators)

  오퍼레이터                    텐서 오퍼레이션              설명

  x+ y                     tf. add()              x와 y의 요소간 덧셈

  x- y                     tF.sub()               x에서 y의 요소간 뺄셈

  x*      y                tF.mul()               x와 y의 요소간 곱셈

  x / y (Python 2)         tf. div()             정수형 텐서인 경우에는 요소간 정수 나눗셈．
                                                 실수 텐서인 경우에는 실수 나눗셈

  x / y (Python 3)         tf. truediv()         요소간 실수 나눗셈
                                                          （정수 포함）




68 - 대APTER 3 텐서플로우 기본


===== PAGE 81 =====
오퍼레이터                    텐서 오퍼레이션              설명

x1/ y (Python 2)         t-F. floordiv()       요소간 floor 나눗셍, 나머지는 반환하지 않음．

x% y                     tf. mod()             요소간 나머지

x *才 y           "
                         tf. pow()             요소간 지수 승

x      <v                tF. less()            요소간 x <y를 계산한 진리표
                                                               （truth table)

x          <=        y   tf. lessmequal()      요소간 x <= y를 계산한 진리표
                                                                 （truth table)

x> v                     tf. greater()         요소간 x> y를 계산한 진리표
                                                               （truth table)

x     >=             y   t-F.greater_equal()   요소간 x >= y를 계산한 진리표
                                                                 （truth table)

x&                   y   tf. logical_and()     요소간 x& y를 계산한 진리표
                                                               （truth table).
                                               dtype은 if.bool이어야함．

xly
                         tf. logical_or()      요소간 x Iy를 계산한 진리표
                                                               （truth table)
                                               dtype은 if.bool이어야함．

x, y        ..
                         tf. logical_xor( )    요소간 x...'y를 계산한 진리표
                                                                 （truth table)
                                               dtype은 if.bool이어야함．




이러한오버로딩된 연산자들을 통해서 쉽게 코드들을 연결할 수 있다. 그러나 이런 각오

퍼레이션에 name 값을 부여할 수 없다. op에 name을 부여하려면, 텐서플로우 오퍼레이

션을 직접적으로 호출하라．




기술적으로 === 연산자도 오버로딩된다. 그러나 이 연산자는 불리언 값의 텐서를 반환하지는 않는다. 대
신 두 개의 텐서가 같은 객체이면 True를 반환하고, 그 반대의 경우는 False를 반환한다. 이 연산자는
내부 목적으로 주로 사용된다. 객체들이 같은지 다른지를 체크하고 싶으면 tf. equal( ）이나 tf. not_
equal( ）을 사용하자．




                                                      텐서플로우에서 계산그래프정의하기          - 69


===== PAGE 82 =====
    텐서플로우 그래프

    이제까지 우리는 '그래프' 라는 것을 텐서플로우 안에서 추상적이면서 언제나 존재하는
    어떤 것으로 생각했다. 또한 이제까지 우리는 코딩을 시작할 때, 각 오퍼레이션들이 그
    래프에 어떻게 자동으로 연결되는지 질문조차 하지 않았다. 이제 우리는몇 개의 예제가

    있으니까，
        텐서플로우 그래프 객체TensorRow Graph object를 살펴보고，
                                                여러 개의 그래프
    를생성해서, 서로 연결하여 사용하는방법을공부하자．

    그래프를 생성하는 것은 간단하다
                    （생성자는 어떠한매개 변수도 필요없다）
                                        .


     import tensorfiow as tf


     # Create α new graph:
     g = t-F.Graph()


    Graph가 초기화되면，
                컨텍스트 매니저content manage
                                     「에 접근하기 위해서 Graph. as_
    default() 메소드를 이용해서 오퍼레이션을추가할수 있다. 컨텍스트매니저를with

    문장과함께 사용해서, 우리가 지금특정한 그래프에 오퍼레이션을 추가하려는 한다는
    것을텐서플로우가 알도록할수 있다．

     with as_defaultO:
         # Create OperatLons as usua야 they wLLL be added to graph 'g '
         a = t-f.mu1(2』 3)




    당신은 이전 예제에서는왜 우리가ops를추가하려는 그래프를 명시할 필요가 없었는

    지 의아해 할 것이다. 편의를 위해서 텐서플로우는 라이브러리가 로딩될 때 자동으로
    53raph를생성하고 이를 디폴트로 할당한다．
                            이를통해서 (5raph . as_default( ) 콘텍
    스트 매니저 외부에 정의된 어떤 오퍼레이션이나 텐서들은 자동으로 디폴트 그래프에
    위치시킨다．




CHAPTER 3 텐서플로우 기본


===== PAGE 83 =====
# F叱aced in th슨 defauLt graph
 in_default_graph = tf. add(l, 2)


 # PLaced in graPh ' g'
 with g.as_defaultO:
 in_graph_g = tf. mul(2,3)


 # We are no Longer in the ' with ' bLock, so this is pLaced in the
 defauLt 9rαPh
 also_in_default_graph = tf. sub(5,l)


디폴트 그래프의 핸들이 필요하면, tf . get_defaultgraph( ) 함수를사용하라：


 default_graph = tf. get_default_graph 0


대부분의 텐서플로우 ㅍ쿠 ㄱ램에서는 대부분 디폴트 그래프만을 다룰 것이다. 그러나
서로 관련이 없는 여러 개의 모델을 사용하려면 다수의 그래프를 만드는 것이 편하다．
다수의 그래프를 하나의 파일에 정의할 때는, 디폴트 그래프를 사용하지 않거나 디폴트
그래프에게 핸들을 즉시 할당하는 것이 가장 좋은 방법이다. 이렇게 하면 각 노드들은
동일한방식으로 각 그래프에 추가될 수 있기 때문이다．


Correct - Create new graphs, ignore default graph:

 import tensorfiow as tf


 gi = tf. Graph()
 g2 = tf. Graph()


 with gl.as_defaultQ:
     # Define gi（功erations, tensors, etc.




 with g2.as'defau1tO:




                                                     텐서플로우에서 계산그래프 정의하기   - 71


===== PAGE 84 =====
                # Define g2 0perations, tensors, etc.




           Correct - Get handle to default graph

            import terisorfiow as tf


            gi = tf.get_default_graph()
            g2 = tf.Graph()


            with gl.as_defaultQ:
                # Define gi Operations, tensors, etc.



            with g2.as_defaultQ:
                # Define g2 0perations, tensors, etc.




           Incorrect: Mix default graph and user-created graph styles

            import tensorfiow as tf


            g2 = tf.Graph()


            # Define defOuLt graph 印erations, tensors, etc를



            with g2.as_defaultQ:
            # Define g2 0perations, tensors, etc.




           또한, 다른 텐서플로우 스크립트에서 정의된 모델을 로딩해서，
                                           그 모델들을Gr햐）
                                                    h .as_

           graph_def( ）와tf. import_graph_def( ) 함수를결합해서 사용해서 Graph 객
           체에 할당할 수 있다. 이와 같이 사용자는 여러 다른 모델들의 결과를 하나의 파이썬 파



72 -   CHAPTER 3 텐서플로우 기본


===== PAGE 85 =====
일에서 계산하고 사용할수 있다．
                이 책의 후반부에 그래프를 임포팅importing 또는 엑스
포팅exporting하는 것을살펴보자．


텐서플로우 세션
       （TensorFiow sessions)

이전 연습문제에서 설명한바와같이，
                 세션（session)은 그래프의 실행을 책임진다．
                                           .생성
잔h-https://wwwtensorfloworg/versions/master/apLdocs/pythonlclient.htm!#Session.
init[tf.Session( )］은3개의선택적인optiona
                                 ［파라미터를가진다．

   . ,:target은사용할실행 엔진을지정한다. 대부분의 응용에서는디폴트인빈문자
       열로 남겨둔다. 세션을 분산환경에서 사용할 경우에 이 파라미터는 tf.train.
       server 인스턴스instance에 연결하기 위해서 사용된다側 책의 후반부에서 언급
       된다）
         .
   · graph는Session에서 실행될 Graph 객체를 지정한다. 디폴트값인None은 현
       재의 디폴트 그래프가 사용됨을 나타낸다. 여러 개의 그래프를 사용하는 경우에
       는실행하고자 하는(raph를 명시적으로 전달하는 것이 좋다
                                      （with 블록 안에서
       Session을생성하는대신에）
                      .
   ·   config는사용자가세션을구성할때 옵션들을지정할수 있도록해준다. 옵션들
       은 사용할 CPU나 GPU의 개수를 제한하거나, 그래프들의 최적 파라미터 설정，
       로깅 옵 크들이 있다．


전형적인 텐서플로우 프로그램에서 Session 객체는 보통 디폴트 생성자 파라미터를
변경하지 않고 생성될 것이다．

 import tensorfiow as tf

 # Create 0Perattons, Tensors, etc (using the defauLt graph)
 a = t-f.add(2, 5)
 b = tf·mu1(a, 3)卜따t;d넘
 # Start Uβ α 'Session ' using the defαuLt graph
 sess = tf. Session()




                                                       텐서플로우에서 계산그래프정의하기          - 73


===== PAGE 86 =====
     아래의 두함수 호출은동일하다·．

      sess = tf.Session()
      sess = tf.Session(graph=tf.get_default_graphQ)


     일단Session이 열리면, 원하는 텐서 출력값을 계산하기 위해서 가장중요한 메소드인
     run( ）을사용할수있다．

      sess.run(b) # Returns 21
       0吐＝c心．   fAv (心 누> 얀ㅆt (Dㄵt)
     Session.run( ）은 필수 파라미터 fetches 하나와 세 개의 옵션 파라미터 feed-
     dict, options, run_metadata를받아들인다. feed--dict 파라미터는중요하기 때
     문에 살펴보고 넘어가자．
                 그러나 나머지 두 개의 선택적인 파라미터 options와「Un-
     metadata는 변경될 가능성도 있고，
                          지금은별로 사용할 필요가 없어서 그냥 넘어가자.



     FETCHES

     fetche＄는오퍼레이션이든텐서이든 사용자가 실행시키고자 하는 어떠한 그래프 구성
     요소든지 받아들일 수 있다．
                   요청된 객체가 텐서라면「un( ）의 출력은NuniPy 배열이
     될 것이고，
          객체가오퍼레이션이라면출력은None일 것이다．

     위의예에서，우리는『etches를텐           .f.
                                           mul오퍼레이션의결踞）로정했다．   이것
    은 텐서플로우에게 Session이 b 값을 계산하기 위해서 필요한 모든 노드를찾아서, 순
     서대로 그것들을 실행하고갼）값을 출력해야 한다는 것을말해준다. 또한 우리는 그래프
    항목들의 리스트를 전달할수도 있다．

      sess·run([a, b]) # returns r7, 217


     fetches가 리스트를 사용하면, run( ）의 출력은 요청된 항목들의 출력에 해당하는 값
    들의 리스트가될 것이다. 이 예제에서 a와b의 값을순서대로요청했다. a와b는텐서이




（거시DTER 3 텐서플로우 기본


===== PAGE 87 =====
기 때문에, 그들의 값을출력으로받게된다．

텐서 객체를 얻기 위해서 fetches를 사용할수 있을뿐만 아니라, 실행할 때 " 유용핸'
부작용＄ide-effect이 있는오퍼레이션의 핸들handle을fetches에게 주는예제를볼수 있을
것이다. 이 예제는tf.initialize_all_variable引 ）라고하는모든 텐서플로우의
Variable 객체를사용하는 예제이다
                    （Variable 객체는 이장의 후반부에서 다룬다）
                                               .

op를fetches 파라미터로써 전달하더라도，Session.run( ）의 결과는 None일 것
이다.


 # Performs the computations needed to initiaLize VariabLes,but returns 'None '
 sess .run(tf. initialize-all-variables ( ) )




FEED 딕셔너리
        （dictionary)

. feed_dict 파라미터는그래프에서 텐서 값을오버라이드override할 때 사용되며，
                                                 파이
썬의 딕셔너리dictionary 객체를 입력으로 기대한다．
                               딕셔너리의 key는오버라이드 되어
야하는 텐서 객체의 핸들인데，
               그 값들은숫자，
                      문자열，
                         리스트 또는NumPy 배열이 될
수 있다
   （이전에 설명되었다）
             . 그 값들은 텐서 key와 같은 자료형
                                  （또는 같은 자료형으로
변경 가능）
     이어야 한다．
           이전의 그래프의 값을 덮어쓰기overwrite 위해서 feed_dict를
쓰는법을알아보자.


 import tensorfiow as tf


 # Create Operations, Tensors, etc (using the def01北t grap!D
 a = t-F.add(2, 5)
 b = t-F.mul(a, 3)


 # Start up α 'Session ' usin9 the defauLt 9rαPh
 sess = t-F.Session()




                                                   텐서플로우에서 계산그래프정의하기              - 75


===== PAGE 88 =====
# Define α dictionary that says to repLace the vaLue（〕
                                                     f ' α ' with 15
replace_dict = {a: 15}

# Run the session, passing in 'repLace_dict ' as the vaLue to 'feed_dict '
sess. run(b, -Feed_dict=replace_dict) # returns 45



              a의 값이 7이되더라욱 우리가feed dict로 전달하는 dictionary는 그 값을 15로 대체
              한다. feed_dict는 많은 상황에서 유용하다. 텐서의 값이 바로 제공되기 때문에, 그래
              프는 더 이상 텐서의 일반적인 의존 관계를 계산할 필요가 없다. 만약 그래프가 아주 크
               더미 값dummy vaLue으로 그 그래프의 일부를 테스트하려는 상황인 경우에，
              고，                                          텐서플로

              우는 불필요한 계산으로 시간을 낭비하지 않는다는 것을 의미한다. feed_dict는 입력
              값을 지정할 때 편한데, 이는 바로 다음에 오는 플레이스홀더ptaceholde
                                                        「 섹션에서 알아

              보자．

              Session을 마친후에,더 이상사용하지 않는자원을 해제하기 위해서 그것의 close( )
              메소드를호출하자．

               # Open Session
               sess = tf. Session()

               # ＇紬n the graph, write summary statistics, etc.



               # CLose the graph, reLease its resources
               sess . close( )


              또 다른 방법으로는 Session을 컨텍스트 매니저로 사용할 수 있다. 이렇게 하면 코드가

              범위scope를 벗어날때 자동으로 dose된다．

               with 더: sessjofl() as sess:
                   # Run graph, write summary statistics, etc.


               # The Session cLoses automaticaLLy




  76 -   CHAPTER 3 텐서플로우 기본


===== PAGE 89 =====
이제 그래프를 실행하는 것을 잘 이해할 수 있을 것이다. 이제는 입력 노드를 지정하는
방법과그들과 feed_dict를 연결해서 사용하는방법을배워보자．



플레이스홀더로 입력 사용하기

웃리가 이전왜 사용하였던 그래프는 진짜 'input'을 사용하지 않고 언제나 동일한 값 5
와3을 사용한다는 점을 눈치챘을 것이다. 지금부터는 다양한 값에 대해서 연산을 수
행하기 위해서 사용자로부터 값을 입력받도록 할 것이다. 이를 위해서 " 플레이스홀더
ptacehoLder" 라는 것을 이용한다．이름이 의미하듯이 플레이스홀더는 텐서 객체인 것처
럼 행동가지맏二岬될 때 값을가지지는않는다 대싣실핼A]Ofl箕렬量．iA1量크함자
                                      플레이스홀더를생
리plac9量l그닌프브姓있다．이로써 'input' 노드가되는효과가있다．
성하는 것은 tf.placeholde
                   「 오퍼레이션을 사용하면 된다.

 import tensorflow as tf
 import numpy as np


 # Creates α pLacehoLder vector o王 Length 2 with data type 1nt32
 a = tf. placeholder(t-F.1nt32, shape=[2], name="my∼input")


 # Use the PLacehoLder as if Lt were αny other Tensor object
 b = tf. reduce_prod(a, name="prod_b")
 c = t-f.reduce_sum(a, name="sum_c")


 # FinLsh of王 the qrαβh
 d = tf. add(b, C, name="add-d")


t-F. placeholder는 파라미터로 dtype이 필요하며，
                                   선택적으로 모양shape 파라미터를
필요로 한다：

   · dtype은플레이스홀더로 전달될 값의 자료형이다．
                               자료형 불일치type mismatch
     오류를막기 위해서 이 파라미터는꼭 필요하다．




                                                   텐서플로우어I, 계산그래프 정의하기   - 77


===== PAGE 90 =====
             . shape은 입력될 텐서 객체의 모양을 정한다＜위의 텐서 shape에 대한논의를참
                 고하자）
                    . shape의 디폴트 값은 None이다. 이는 어떤 shape의 텐서도 받아들인

                 다는 것을 의미한다．


           다른 오퍼레이션과동일하게 tf. placeholde
                                      「에도 name 식별자를 지정할수 있다．

           플레이스홀더에게 값을 전달하기 위해서 Session. run( ）에서 feed_dict 파라미터
           를 사용할 것이다．
                    플레이스홀더의 출력에 대한 핸들을 dictionary에 대한 key로 사용
           핸다
            （위의 코드에서는 변수 a), 그리고 우리가 전달하고자 하는 텐서 객체를 그것의 값
           으로 사용한다．


            # Open α TensorFtow Session
            sess = tf. Session()


            # Create α dictionary to pass into 'feed_dLct '
            # Key: ' α ' , the han‘九e to the placeholder's output Tensor
            # VaLue: A vector with vaLue r5, 37 and int32 data type
            input_dict = {a: np.array([5, 3], dtype=np.1nt32)}


            # Fetch the vaLue of 'd' J feeding the vaLues （〕f ' input vector ' into ' α'
            sess. run(d, feed_dict=input_dict)


           fetch된 출력에 의존성을 가진 각 플레이스홀더마다 feed_dict에 키값key-vaLue 쌍을
           반드시 포함해야한다. 위의 예에서는, 우리가fetch하는 d는 a의 출력에 의존한다. 만약
           d가 의존하지 않는 또 다른 플레이스홀더를 정의했었다면, feed_dict에 그것을 포함
           할 필요가 없을 것이다．


            플레이스홀더의 값을 fetch할 수 없다. Sessioin . run( ）에 어떤 값을 넣으려고 하

            면 에러exception가 발생할 것이다．




78 -   CHAPTER 3 텐서플로우 기본


===== PAGE 91 =====
변수


변수 생성

텐서와오퍼레이션 객체는 변경할수 없다. 그러나 머신 러닝은속성상 시간에 따라 변
경되는값을 저장할수 있는방법이 필요하다. 텐서플로우에서는 이를 위해서 여러 번의

Session.run( ）호출동안유지되면서畛졍r7怜한텐서값을보관하기 위해서변今
,VariabLe 객체를사용한다．
                 t-F.Variable( ) 생성자를사용해서 변수 객체를 생성할수
있다．

 import tensorfiow as tf


 # Pass in α starting V(北ue of three for the variabLe
 my_var = tf. Variable( 』, name= 'my_variable")


변수는텐서를사용할수 있는 어떤 텐서플로우 함수／오퍼레이션에서도 사용할수 있다．
변수의 현재값은 그것을사용하는오퍼레이션에게 전달된다．

 add = tf. add(5, my_var)
 mul = t-F.mul(8, my_var)


변수의 초기값은 보통 많은 0, 1 또는 랜덤값들로 이루어진 큰 텐서large tensors들이다．
이런 일반적으로 많이 사용되는 값들을 생성하기 쉽게 하기 위해서 텐서플로우는 다
음과같은다양한오퍼레이션을제공한다. tf. zeros( ),tf.one引 ), tf. random_
normal( ),tf.random_uniform( ). 이들은 원하는 텐서의 차원을 지정하는 shape

파라미터를받는다．


 # 2x2 matrix 0f zeros
 zeros = t-F. zeros([2, 2])


 # vector （그f Length 6 af ones
 ones = tf. ones([ ])




                                                  텐서플로우에서 계산그래프정의하기   - 79


===== PAGE 92 =====
# 3x3x3 Tensor of random uniform vaLues between o and 그o
uniform = tf. random_uniform([3, 3, 3], minval=0, maxval=10)


# 3x3x3 Tensor of normaL Ly（九stributed numbers; mean 0 and standard deviation 2
normal = tf. random_normal([3, 3, 3], mean=0.0, stddev=2.0)



               t-f. random-normal( ）을사용하는대신, tf. truncated_normal( ）을사용하는것
               을종종볼 것이다. 이것은 평균mean에서 표준 편차standard deviation 2배 이상인 값은 생
               성하지 않기 때문에, 텐서 내부의 한두 개의 값이 다른 값들과많은 차이가나는 가능성
               을막아준다．

                # No vaLues beL이｀/ 3. e or above 7. 9 wiLL be returned in this Tensor
                trunc = tf. truncated_normal({2, 2], mean=5.0, stddev=1.0)



               이러한오퍼레이션을텐서를만들때 변수의초기값으로 넘겨줄수 있다．

                # DefαuLt vaLue 0f mean=0. 0
                # DefauLt VaLue of 5tddev=1.0
                random_var = tf. Variable(tf. truncated_normal([2, 2]))



               변수 초기화

               변수 객체는 텐서플로우의 다른 객체들 처럼 Graph 내부에 존재한다. 그러니：生三의상 ,
               태는 Session에 의해서 관리된다. 이 때
                                       ［문에 변수들을 사용할 때는 한단계가 더 필요

                                     （촌Z嫂肄츠학다는점' 따 .o1 게하면5" " " "
                kt11, Sessio" 내부에서변수들을
               이 변수의 현재의 값들을 추적하기 시작하게 한다. 이는 보통 tf. initialize_a11_
               variable竅 ) 오퍼레이션을SeSsion.run( ）에 전달함으로써 일어난다．

                mnit = tf. initialize all variables()
                sess = tf. Session()
                sess. run(init)




  80   -   CHAPTER 3 텐서플로우 기본


===== PAGE 93 =====
그래프에서 정의된 변수들의 일부분subset만을 초기화하려면, tf. initialize_
variables( ）를사용하면 된다. 이는초기화될 변수들의 리스트를받아들인다．


van1 = t-F.Variable(e, name="initialize_me")
var2 = tf. Vaniable(1, name="rio_initialization")
mnit = tf. mnitialize_variables([varl], name="init_vari")
sess = 더궉Session()
sess .run(init)



변수값 변경

변수의 값을 변경하기 위해서, Variable.assign( ) 메소드를사용해서 변수에 새로
운값을부여할수 있다. Variable.assign( ）은오퍼레이션이기 때문에 Session에

서 실행되어야효과가발생한다．


# Create varLabLe with starting vaLue af 그
my_var = t-F.Variable(1)


# Create αn operation that mu!.ttpLies the 以7尸tαz兀e by 2 each time it is run
my_var_times_two = my_var.assign(my_van * 2)


# Intt-iaLization operation
mnit = tf. initialize_all_vaniables()


# Start α sesst아？
sess = tf Session()


# 1nitiα［.tze vartabLe
sess. run(init)


# 세冗ttβLy Vαrtαt)Le by t14／
                          《） and return it
sess . run(my_van_times_two)
## OUT: 2




                                                    텐서플로우에서 계산그래프 정의하기         - 81


===== PAGE 94 =====
# MuLtLpb/ αgαtn
sess.run(my_var_times_two)
## OUT' 4


# MuLtipLy again
sess.run(my_var_times_two)
## OUT: 8



               변수의 값을 편하게 증가／감소시키기 위해서, 텐서플로우는Variable.assign_add( )
               와Variable.assign sub( ) 메소드를사용한다．


                   # Increment by l
                   sess. run(my_var. assign_add(1))


                   # Decrement 勻／ 그
                   sess . run(my_var.assign_sub(1))


               Session들은 변수들의 값을 독립적으로 관리하기 때문에, 각 Session은 그래프에 정
               의된 변수들의 자신의 현재값을 가진다．


# Create Ops
my_var = tf. Variable(0)
mnit = tf. initialize_all_variables()


# Start Sesstons
sessi = tf. Session()
sess2 = tf. Session()


# InitiaLize VariabLe in sessi, and increment vaLue（萃 my_ var in that Session
sessi. run(init)
sessi. run(my_var. assign_add( 5))
## 0U7: ,


# Do the same with sess2, but use α different increment vaLue




  82 -   CHAPTER 3 텐서플로우 기본


===== PAGE 95 =====
sess2.run(init)
sess2.run(my_var.assign_add(2))
## OUT: 2


# Can increment the VariabLe vaLues in each Session independentLy


 sessl.run(my_var.assign_add(5))
## OUT: 10


 sess2.run(rny_var.assign_add(2))
## OUT: 4



변수들을 각각의 시작값으로 리셋하려면, tf. initialize_ all_ variables( )

           （또는 변수들의 부분 집합만을 리셋하려면 tf. initialize_
를 다시 호출하면 된다

variables):


 # Create 야'5
 my_var = tf. Variable(0)
 iriit = tf. initialize_all_variables()


 # Start Sessi아구
 sess = tf. Session()


 # 工ntttαt.tze VαrtαbLes
 sess.run(init)


 # Change the Vα尸iαbLe
 sess . run(my_var . assign(10))


 # Reset the VariabLe to 0, its initiaL vaLue
 sess . run(init)




                                                 텐서플로우에서 계산그래프 정의하기   - 83


===== PAGE 96 =====
    학습 가능
        （trainable)

    이 책의 후반부에서, 머신 러닝 모델을자동으로 학습시키는 다양한종류의 Optimizer
    클래스를볼수 있다. 이들은 변수 객체의 값을 명시적으로물어보지 않고 수정한다. 대

    부분의 경우에 이런 상황은 사용자가 원하는 것이기는 하지만, 만약 그래프 안의 어떤
    변수가수작업으로만 변경되어야하고Optimize
                            「에 의해서는변경되면안되는상황이
    라면, 변수들을생성할때 그들의 trainable 파라미터를 False로해야한다．


     not_trainable = tf.Variable(0, trainable=False)


    이것은 보통 스텝 카운터＄tep counte
                          「나 머신 러닝 모델의 계산과 연관이 없는 것들에 사
    용된다．




    그래프를 name scope로 구성하기


    이제까지 텐서플로우 그래프를 만드는데 필요한 핵심은 이미 살펴보았다. 이제까지 서
    너 개의 노드와작은 텐서들을 가진작은 그래프만사용했었다. 그러나 실제의 모델들은
    수 백 개의 노드와 수 백만 개의 파라미터를 사용한다. 이렇게 큰 복잡도를다루기 위해
    서 텐서플로우는네임 스코프name scope라는 개념을사용한다．

    네임 스코프는 사용하기 아주 간단하면서도 텐서보드에서 그래프를 시각화할 때 아주
    좋다. 네임 스코프는 오퍼레이션을 더 큰 블록bLock으로 만들수 있게 해준다. 그리고 텐
    서보드에서 그래프를 실행할때，
                   각네임 스코프는자신의 오퍼레이션을묶어encapsulate
    준다. 이를 통해서 그래프의 시각화가 쉬워진다. 기본적인 네임 스코프 사용법으로
    with tf. name_scope( <name> )블록내부에 오퍼레이션을추가해보자．


     import tensorflow as tf


     with tf. nanie_scope( 'Scope_A") :
         a = tf. add(1, 2, name="A_add")




애APTER 3 텐서플로우 기본


===== PAGE 97 =====
    b = tF.mul(a, 3, name="A-mul")


with tf.name_scope( "Scope_B"):
    c = t-F.add(4, 5, name="B_add")
    d = t-F.mul(c, 6, name="B_mul")


e = t-F.add(b, d, name="output")


텐서보드에서 네임 스코프의 효과를 보기 위해서 SummaryWrite
                                     「로 그래프를 디스크

에써보자．


writer = tf. train.SummaryWriter( ' ./name_scope_1 ', graph=t-f.get_de-fault_graphQ)
writer.close()


SummaryWrite
           「는그래프를즉시 엑ㅅ平ㅌ하기 때문에, 위의 코드를 실행한후에 텐서

보드를금방시작할수 있다. 당신이 실행한 이전 스크립트로 가서 텐서보드를 시작하자．
                                             l "


$ tensorboard --1ogdir=' 鬱narne_scope_1少


이전과 같이, 위의 문장은 로컬 컴퓨터의 포트 6006에서 텐서보드 서버를 실행할 것이
대 브라우저를 열어서 URL 바에 localhost:6006을 입력하자．
                                       Graph 탭을 보면 아
래와같은 것을볼수 있다：


      iU-.--
                                    output

      ＝翼，      :




                                        (∼         Scope_   B   "
                               A1
                     Scope_
                                                                그래프를 name scope로구성하기   - 85


===== PAGE 98 =====
           우리가 그래프에 추가한 add와 mu]. 오퍼레이션은 바로 보이지 않고, 대신 오퍼레이션

           들을 둘러싸고 있는 네임 스코프를 볼 수 있다. 네임 스코프 박스의 오른쪽 상단의 + 아

           이콘을 클릭하면 네임 스코프 상자를 열수 있다．



                   H


              -




           각 스코프 안에서 그래프에 추가한 각 오퍼레이션을 볼 수 있다. 하나의 네임 스코프 안

           에다른 네임 스코프를중첩할수도 있다：


            graph = 杆.Gra뱐，
                          ()


            with graph.as_defaultQ:
                  in_i = t-F.piacehoider(tf. fl0at32, shape=[], name="input_a")
                  in_2 = tf. piaceholder(tf. f]0at32, shape=[], name="input_b")
                  const = t-F.constant(3, dtype=tf. float32, name='static_vaiue' )


                  with t-F.name_scope("Transformation '):


                       with tf. name_scope( "A") :
                           A_mu]
                               . = tf. mui(in_i, const)
                           A_out = tf. sub(A_mui, in_i)


                       with tf. name_scope("B") :
                           B_mui = tf. mui(1n-2, const)




86 -   CHAPTER 3 텐서플로우 기본


===== PAGE 99 =====
            A_out = tf.sub(B_mul, in_2) /:'＼』4.
                                            h'mt…
        with tf. name_scope("C") :
            C_div = tf. div(A_out, B_out)
            C_out = tf. add(C_div, const)


        with tf. name_scope( "D") :
            D_div = tf. div(B_out, A_out)
            D_out = tf. add(D_div, const)
    out = t-F.maximum(C_out, D_out)


writer = t-F.train.SummaryWriter( ' ./name_scope_2', graph=graph)
writer.close()


이 코드는 디폴트 그래프를 사용하지 않고 tf. Gra한，
                               객체를 명시적으로 만들고 있다．

코드를 보고 정획뼈 코드가 어떤 구조인지 확인하기 위해서 네임 스코프에 집중하자．


graph = t-F.Graph()


with graph.as_defaultQ:
    in_i = tf. piacehoider(. . .)
    in_2 = tf. piacehoider(. . .)
    const = tf. constant(. . .)


    with tf. name_scope("Transformation") :


        with tf. name_scope( "A") :
            # Takes tn_i, ㅇUtPuts some vaLue



        with tf. narne_scope("B") :
            # Takes Ln_2, outputs some v九ue



        with t-F.name_scope("C") :




                                                     그래프를name scope로구성하기   - 87


===== PAGE 100 =====
                   # Takes the output of A and B, outputs some `/（끄ue




               with t-f.namescope("D") :
                   # Takes the output of A and BJ outputs some `／αLue




         # Takes the output of C and p
         out = tf. maximum(. . . )


    이제 코드를 분해해서 보기 더 쉬워졌다. 이 모델은 입력으로 두 개의 스칼라 플레이스

    홀더, 텐서플로우상수, 가운데에 위치한' Transformation" 이라는부분, 그리고오퍼레
    이션으로tf . maximum( ）을사용하는 최종출력 노드로구성된다. 이를 텐서보드의 상

    위단계에서 개략적인내용을볼수 있다：


     # Start up TensorBoard in α ternrina니 Loading in our previous graph
     $ tensorboard --logdir= ' ./name_scope_2'




               蓼                                      Maximum

                                                           듀＞
                                                                C
                                                                8!
                                                                m




                                     Transformation
                                                i     F·
                                                                     inp
                                                                       '   b
          :F
    Transform 네임 스코프 내부에는 2 레이어［aye
                                  「으로 배치된 4개의 네임 스코프가 더 있
    다. 첫 번째 레이어에 있는스코프 " A" 와''B" 는그들의 출력값을다음레이어인 " C"와
    "D" 로 넘겨준다. 마지막 노드는 이 마지막 레이어의 출력값을 입력값으로 사용한다. 턴l



CHAPTER 3 텐서플로우 기본


===== PAGE 101 =====
서보드에서 Transformation 네임 스코프를 펼쳐보면 아래와 같이 확인할 수 있을 것

이다．




               차
                                        ＝蔘
               …
               …
                              共央


이 그림에서 텐서보드의 또다른특징을볼수 있다. 위 그림에서 네임 스코프 " A"와" B"
는파란색이고，
      "C"와" D" 는녹색이다．
                    이 네임 스코프들은동일한형태configuration에서
설정된동일한오퍼레이션을가지기 때문이다．
                    즉，"A"와" B" 는둘다tf.sub( ) Op로
데이터를전달하는tf.mul( )Op를가지고 있고，
                          "C"와" D"는tf.add( )Op로데이
터를전달하는tf.div( ) Op를가지고 있다．
                         오퍼레얘크들을반복적인순서로만들
때 편리한기능이다．



      U
      m
      ,
      一

      뻐*m              .叫mm
      d．
       口·          -
                                        山m．
                                          ·




          就             －
          !
                        缸
          八，            骨
                                     그래프를 name scope로구성하기   - 89


===== PAGE 102 =====
    이 그림을 보면, 텐서보드에서 출력될때 奸．
                           constant 객체는다른텐서나 오퍼레이션
    과는다르게 동작한다는 것을볼수 있다. 어떤네임 스코프 외부에 $tatic_value를 선
    언하더라도，
         그 값은 여전히 그 내부에 위치한다. 또한 static_value는 하나의 아이콘
    이 아니라사용될때마다아이콘이 만들어진다. 이와관련된 기본적인아이디어는상수
    는 언제든지 사용될수 있고 어떤특정한 순서로 사용될 필요가 없다는 점이다. 한곳에
    서 그래프의 여러 곳으로 화살표를 그리는 것을방지하기 위해서 상수가 사용될 때마다
    표기하는 것이다．




CHAPTER 3 텐서플로우 기본


===== PAGE 103 =====
                  연습문제：모두 합치기

이제까지 소개한 모든 요소들을 사용하는 연습문제를 다루면서 이 장를 마치자. 이제까
지 우리는 텐서, 그래프, 오퍼레이션, 변수, 플레이스홀더, 세션, 네임 ㅅㅋㅍ를 배웠다．
텐서보드를 통해서 그래프의 실행 상황을 추적해볼 수도 있다. 이제 기본적인 텐서플로
우 그래프를만들고 텐서보드상에서 실행해보기 바란다．

가장 핵심적인 사항은 우리의 첫 번째 모델과유사할 것이다．



        5




        3




그러나 이번에는텐서플로우의 기능을 더욱잘 사용하기 위해서 중요한 몇 가지 다른 점

이 있다．

      입력은 tf. constant 노드 대신에 플레이스홀더를 사용한다．

  · 두 개의 이산스칼라discrete scala
                          「 입력을 사용하는 대신, 가변 길이의 하나의 벡
      터를사용한다．
  ·   그래프를사용하는동안의 시간에 따른모든출력값을누적할것이다．
  ·   그래프를네임 ㅅㅋㅍ무 깔끔하게분할할것이다．
  ·   각각의 실행 후에, 그래프의 출력, 모든출력 결과의 누적, 모든출력 결과의 평균
      을 텐서보드에서 사용하기 위해서 디스크에 저장할 것이다．


다음은 우리가만들 그래프의 개괄을 보이는 그림이다：




                                       그래프를 name scope로구성하기   - 91


===== PAGE 104 =====
                                                           Transf。
                                                                 rmati 。n,




                        / TensorBoard summJ7T --"

                              output Summary
                                                    'r
                                                                             [1
                                                         Varㄱab〕eS




             이 모델을 읽을 때 주의할 점이다：

               · 각에지에 [None] 또는 [ ] 아이콘이 배치된 이유를알자．
                                                  이는에지를타고흐

                  르는텐서의 형태를의미하는데, None는가변 길이의 벡터를,〔 ］는스칼라를의
                  미한다．
                · 노드 d의 출력이 " update" 섹션으로 흘러 들어간다．
                                                  이 섹션은TensorBoard

                  Summaries로 데이터를 전송하고, 변수를 업데이트하기 위해 필요한 오퍼레이
                  션을 가진다．
                · 두 개의 변수를 저장하기 위해서 별도의 네임 스코프를 가진다. 하나는출력값의
                  누적 합을 저장하고, 다른 하나는 그래프의 수행 횟수를 저장한다. 이 두 개의 변
                  수는 우리의 중요 트랜스포메이션transformation의 외부에서 작동하기 때문에, 별
                  도의 스페이스에 할당하는 것이 합리적이다．

                · tf. scalar_summary오퍼레이션을가지는텐서보드요약에 네임 스코프를할
                     이를 " update" 섹션 뒤에 배치함으로써 요약들이 변수를 업데이트한후
                  당한다．
                  추가되는 것을 확실히 한다. 그렇지 않으면순서가 엉클어질 수도 있다．




92   -   CHAPTER 3 텐서플로우 기본


===== PAGE 105 =====
이제 시작하자！코드 에디터를 열거나 인터랙티브 파이썬 환경을 시작하자．



그래프 만들기

언제나 처럼 가장 먼저 해야 하는 일은텐서플로우 라이브러리를 임포트하는 것이다．

import tensorfiow as tf


디폴트그래프를사용하지 않고그래프를명시적으로만들기 위해서, tf.graph( ）를
사용하자．

   graph = tf. Graph()


이제부터 우리의 모델을만드는동안은이새로운그래프를 디폴트로 사용할 것이다．

   with graph. as_default Q:


                               첫 번째는 " global_step" 인데 모델
우리 모델에는 " global" 스타일의 변수가2개 있다．
을실행한횟수를 기억하는 변수이다. 이는텐서플로우에서 일반적인방법인데, API 전
                           두 번째는 " total_output" 으로써 시
반을 걸쳐서 이것이 사용되는 것을 보게 될 것이다．
간에 따라서 이 모델에서 실행된 모든 출력 결과의 합을 기록한다. 이 변수들은 속성상
               그래프의 나머지 노드들과는 별개로 선언하고 그들 자신의 네
전역적globa［이기 때문에，
임 스페이스에 배치한다.


 with graph.as_defaultQ:

    with t-f.name_scope( 'variables") :
         # Var1a帆e to keep track of how mαny times the graph hα5 been run
         global_step = t-f.Variable( , dtype=tf. int32, trainable=False, name="global_step")
        # VariabLe that keeps track of the sum of aLL output vaLues over time:
        total_output = tf. Variable(      , dtype=t-F.float32, trainable=False,
                                     name="total_output")




                                                         그래프를name scope로구성하기          - 93


===== PAGE 106 =====
              지금은 trainable=False라고 설정하였다. 지금은 학습을 시키고 있지 않기 때문에 아

              무런 효과가 없지만, 이 설정을 통해서 이 변수들이 수작업으로 세팅될 것이라는 것을

              명확하게 해준다．

              다음으로, 이 모델의 핵심 연산 부분을작성하자. "transformation" 이라는 네임 스코

                              그리고 이 네임 스코프는 " input", "intermediate
              프에서 전체 연산부분을작성하자．

              layer","output" 네임 스코프들로다시 세부적으로나뉜다：



with graph. as_de-faultQ:
    with tf. name_scope( "variables"):



   with" tt=name_scope( 'transformation"):


        # Separate input（αyer
        with tf. name_scope( "input"):
            # Create input pLacehoLder- takes in α Vector
            a = tf. placeholder(t-F.fl0at32, shape=[Nonej, name="iriput_placeholder_a")


        # Separate mtdc北e Lαyer
        with tf. name_scope( "intermediate_layer"):
            b = tf. reduce_prod(a, name="product_b")
            c = tf. reduce_sum(a, name="sum_c")


        # Separate output Layer
        with tf. name_scope( "output"):
            output = t-f.add(b, c, name="output")



              이 코드는 이전모델의 코드와몇 개의 차이점만 있을 뿐 매우 유사하다．

                    입력 노드가 모든 길이의 벡터를 받아들이는 tf. placeholde
                                                         「이다
                                                           （shape
                    =[None])




 94 -   CHAPTER 3 텐서플로우 기본


===== PAGE 107 =====
  · tf.mul( ),t-F.add( ）를 사용하는 대신, 각각 tf . reduce_prod( ）와
     tf. reduce_sum( ）을사용한다．이전의 ops는 정확히 2개의 스칼라 입력만을
     벋아들이는데, 이들은 전체 입력 벡터를곱하거나더할수 있기 때문이다．


Transformation 연산을마친 후에, 위의 두 개의 변수를 업데이트해야 한다. 이를 위해
서 "update'" 네임스코프를만들자：


 with graph. as_default Q:
     with tf. name_scope("variables") :




     with tf. name_scope("transformation") :




     with tf. name_scope("update") :
         # 力？crements the totaL_output VariabLe by the Latest output
         update_total = total_output.assign_add(output)


         # Increments the above ' gLobaL_step ' VariabLe, 功ouLd be run ihenever the
graph ts run
         increment_step = global_step. assign_add(l)



total_output과global_step을증가시키기 위해서 Variable,assign_add( ) 오
퍼레이션을사용한다．
         시간에 따른모든출력값을누적해서 더하기 위해서 output의 값
을total_output에 더하고, global_ste〕
                              은단순하게 1씩 증가시킨다．

변수들을 업데이트한후에 이제 텐서보드요약을만들어보자. 이를 " summaries" 네임
스코프에서 코딩하자．


 with graph.as_defaultQ:


         with tf. name_scope( 'update' ):




                                                       그래프를 name scope로구성하기    - 95


===== PAGE 108 =====
         with t-F.name_scope( "summaries"):
             avg = tf.div(update_total, t-F.cast(increment_step, t-F.flOat32), name="average")


             # Creates summaries for output node
             tf.scalar_summary(b'Output', output, name="output_summary")
             t-F.scalar_summary(b'Sum of outputs over time', update_total,
         name="total_summary")
             tf.scalar_summary(b'Average of outputs over time', avg,
         name="average_summary")



               이 섹션 내부에서 할 첫 번째 일은 시간에 따른 평균 출력값을 계산하는 것이다. 다행
               스럽게도, total_output 변수에 모든 출력값의 합이 있다
                                                  （avg를 계산하기 전에 업
               데이트를 한다는 것을 확실히 하기 위해서 update_total의 출력을 사용한다）
                                                            .또

                                                （동일하게 우리는 그래프가
               한 global_step은 그래프를 실행한 총 횟수를 저장한다
               순서대로 실행된다는 것을 보장하기 위해서 increment_step의 결과를 사용한다）
                                                              .

                            별도의 tf. scalar_summary 객체를 가지고 output, update_
               average를구한후에는，
               total, avg를저장한다．

               그래프를마치기 위해서, 변수초기화오퍼레이션과모든요약을합치기 위한도우미 노

                                         이를 " glob쿄ops" 네임스코프에두자．
               드heLper node를하나의오퍼레이션으로만들고，


                with graph.as_defau1t() :


                    with t-F.name_scope( "summaries") :


                     with tf. name_scope("global_ops") :
                         # InitiaLization Op
                         mnit = tf. initialize_all_variables()
                         # t'lerge aLL summaries into one Operation
                         merged_summaries = t-F.merge_all_summaries 0




96   -   CHAPT티국3 텐서플로우 기본


===== PAGE 109 =====
왜tf.merge_all_summaries( ) Op를" summary" 네임스코프대신여기에배치하

는지 의아할 것이다．
          이 경우에는 큰 차이가 없지만, merge_all_summaris( ）를 다른
전역 오퍼레이션global operation과 같이 두는 것이 일반적으로 가장좋은 방법이다. 이 그
래프는 summary를 위해서 하나의 섹션만을 사용하지만，
                               변수，
                                 오퍼레이션，
                                      네임 스코
프들을위해서 다양한요약이 필요한그래프를상상해보자. merge_all_summarie軾 )

를따로보관하는것은 " summary" 코드블록을 어디에 두었는지 기억할필요없이 오
퍼레이션을찾을수 있게 보장해준다．

여기까지가그래프를생성하는모든내용이다. 이제 그래프 실행으로 넘어가보자．



그래프 실행

Session을 열고，
           방금 만든 Graph를 가동하자．
                            요약을 저장하기 위해서 사용할
t-F.trairi.SumaryWrite
                     「도 열자．
                          여기서 swnmary가저장될폴더로써 ./improved_
graph를 사용하자．

sess = tf .Session(graph=graph)
writer = tf.train.SummaryWriter(' ./improved graph', graph)


Session이 시작하고，
             먼저 변수들을초기화하자．

 sess.run(init)


실제로그래프를실행하기 위해서, 도우미 함수「un_graph( ）를만들자. 이 함수는 계
속 같은 일을 반복하지 않게 해준다. 우리가 하고자 하는 것은 입력 벡터를 그래프를 실
행할함수에게 넘겨주고summary를 저장하는 것이다．

def run_graph(input_tensor):
    feed_dict = {a: input_tensor)
    _, step, summary = sess.run([output, increment_step, merged_
summaries], feed_dict=feed_dict)
    writer.add_summary(summary, global_step=step)




                                                    그래프를name scope로구성하기   - 97


===== PAGE 110 =====
    아래는「un_graph ) 함수의 각라인별 설명이다：

      1. 첫번째로，
             Session. run( ）에시 -Feed_dict로사용할dictionary를생성한다．
          이는핸들a를사용하는t-f. placeholde
                                  「노드와연관있다．

       2. 다음에는feed_dict를 사용해서 우리의 Session이 그래프를실행하도록하
          자．
           그리고 output, increment_step, merged_summaries Ops를 실행한다

          는 것을 확실히하자. summary를 출력하기 위해서 g1obal_ste）
                                                  과 merged_
          summaries 값을 저장해야 한다. 이를 위해서 파이썬 변수 step과 summary에
          저장한다. 언더스코어 - 문자를 사용해서 output 값을저장할 필요는 없다는 것
          을보이고 있다.

       3. 마지막으로，
               S네inary를SummaryWrite
                                  「에 더한다. global_step 파라미터는
          중요한데, 이것이 텐서보드가시간에 따라그래프를그리도록하기 때문이다．


    이제 정말 사용해보자！아래와 같이 다양한 길이의 벡터를 이용해서 여러 번「Un-
    graph를호출하자：


     run_gra帥 （ [2,8])
     run_gra ph( [ 3,1,3,3])
     run_graph( [8])
     run_gra ph( [1,2, 3])
     run_graph([ll, 4])
     run_gra ph( [4,1])
     run_gra ph( [ 7, 3,1])
     run_graph( [6, 3])
     run_graph( [0, 2])
     run_graph([4,5,6])


    원하는만큼 여러 번 해본후에, 요약을 Summary1Jriter .flush( ）를 이용해서 디스크
    에 쓰자：


     writer.flush()




CHAPTER 3 텐서플로우 기본


===== PAGE 111 =====
마지막으로, SumaryWrite
                 「와Session을닫자：


writer.c].ose()
sess.close()


여기가 우리의 텐서플로우 코드의 끝이다！지난번 그래프보다 조금 길었지만 그렇게나
쁘지만은 않았다. 이제 텐서보 크를 열어보자. 터미널 쉘을 열어서 방금 실행한 코드가

          （"improved_graph" 라는 이름의 디렉터리가 있어야 한다）
있는 디렉터리로 가자                                    . 그리
고다음을실행하자：

 $ tensorboard --logdir='improved_graph"


텐서보드 서버의 포트 6006을 열고，
                    "improved_graph" 안에 저장된 데이터를 사용할
것이다. 이제 웹 브라우저에 " localhost:6006" 을 입력하고 어떤 결과가화면에 나오는지
보자．
  먼저 " Graph" 탭을보자．


      a         ．·－
       !        驪．H*m




                          "    summariesj
     ‘饉닙＝

                                 update



           H=




           ；■       ㅡ季毛
                              transformation   l variables

이 그래프가 처음에 다이어그램으로 그렸던 것과 일치하는 것을 확인할 수 있다．

transformation 오퍼레이션이 update 블록으로 흘러가서 summaiy와variable 네임
ㅅ구ㅍ무 들어간다. 다이어그램과의 차이점은 주된 트랜스포메이션 계산과는 관련이

없는오퍼레이션을포함하는 " 얹obal_ops" 네임스코프이다．




                                                             그래프를name scope로구성하기   - 99


===== PAGE 112 =====
    각블록을 확장해서 좀더 자세하게 확인할수도 있다．



                                         〔 쁘쁘1쁘8 ．ㅣ


                                          (   0date     l    "



                                          transformation 놓




                                         r- Othp1t



                                         l 1탤1md.1쳔쓰／
                                                i




                                         이런작은예에서는너무과
    이제 input, intermediate 레이어와출력을확인할수 있다．
    하다고 생각할 수도 있지만, 이렇게 부분들로 나누는 방법이 좋다. 그래프의 나머지 블
    록도펼쳐보자. 이제준비되었으면" Events" 페이지로넘어가보자．


            ‘
         ·1끼已            `   七m.'－ ·－-
         ㅁ．m. `-             m·

         ㅁm－뻐뻐－              -


         －뻐

         -      －∼   -




         =
                                         ∼∼－            →／       "   '   \/-－∼＼ . /




    "Events" 페이지를 열면，
                    우리가 위에서 scalar_summary 객체에서 부여한 이름에 따
    른3개의 탭을볼수 있다. 그중에 하나의 탭을클릭하면, 시간에 따라 저장된값들이 꺽
    은선 차트로 보인다. 차트의 좌측 하단의 파란 사각형을 클릭하면 위와 같은 그림을 볼
    수 있다．



CHAPTER 3 텐서플로우 기본


===== PAGE 113 =====
summary의 결과들을 확인하고 비교해서 적합한 결과인지 확실히 살펴보자．
                                         여기까지
하면서 다이어그램에서부터 텐서플로우 그래프를 만드는 법과 텐서보드에서 기본적인
요약을살펴보는 법을 배웠다．

이 연습문제를 위한 전체 코 三는 아래와 같다：


import tensorfiow as t-F


# ExpLicitLy create α Graph object
graph = tF.Gra아1()


with graph.as_de-Fault():


    with t-F.name_scope( "variables") :
        # VariabLe to keep track of hoi many times the graph has been run
        global_step = t-F.Variable(0, dtype=tf. int32, trainable=False, narne="global_step")


        # VariabLe that keeps track （〕
                                     f the sum of aLL output vaLues over time:
        total_output = tf. Variable(0.0, dtype=tf. fl0at32, trainable=False,
    name="total_output")


        # Primary transformation Operations
        with t-F.name_scope("trans-Formation") :


             # Separate input Layer
             with t-F.name_scope( "input") :
                 # Create input pLacehoLder-takes in α Vector
                 a = tF.placeholder(t-F.fl0at32, shape=[None], name="inputplaceholder_a")


             # Separate mid
                          （九e Lαyer
             with t-F.name_scope( "intermediate_layer' ):
                 b = tf. reduce_prod(a, name="product_b")
                 c = tF.reduce_sum(a, name= 'sum_c")


               # Separate output 功yer




                                                        그래프를name scope로구성하기           - 101


===== PAGE 114 =====
             with tf.name_scope("output"):
                 output = tf.add(b, c, name="output")


             with tf.name_scope( "update"):
                 # Increments the totaL_output VariabLe 妙 the Latest output
                 update_total = total_output. assign_add(output)


                 # Increments the above 'gLobaL_step ' VariabLe, shouLd be run whenever
             the graPh is run
                 increment_step = global_step.assign_add(l)


         # Summary Operations
         with tf. name_scope( "summaries"):
             avg = tf. div(update_total, tf. cast(increment_step, tf. flOat32),
         name="average")


             # creates summaries for output node
             tf. scalar_summary(b 'Output', output, name="output_summary")
             tf. scalar_sunuflary(b 'Sum of outputs over time', update_total,
         name="total_summary")
             tf. scalar_summary(b 'Average of outputs over time', avg,
         name="average_summary")


         # GLobaL `／αriαbLes and Operations
         with tf. name_scope( "global_ops"):
             # 끄珏ti(쿄ization Op
             mnit = tf. initialize_all_variables()
               # Merge αLL summaries into one Operati아1
               merged_summaries = tf. merge_afl_summaries()


# Start α Session, using the expLicitLy created Graph
sess = 터LSession(graph=gra뱐D
# Open α SummaryWriter to save summaries
writer = tf. train.SummaryWriter( ' ./improvedgraph', graph)




 102 -   CHAPTER3 텐서플로우 기본


===== PAGE 115 =====
# In-LtLl九ize VariaLn.es
sess. run(init)


def run_graph(input_tensor):


    Helper function; runs the graph with given input tensor and saves summaries


    feed_dict = {a: input_tensor)
    -, step, summary = sess.run([output, increment_step,
    merged_summaries], feed_dict=feed_dict)
    writer. add_summary( summary, global_step=step)


# Run the graph with various inputs
run_graph( [2,8])
run_graph([3,1,3, 3])
run_graph( [8])
run_graph([1,2, 3])
run_graph( [11,4])
run_graph( [4,1])
run_graph( [7,3,1])
run_graph( [6,3])
run_graph( [0,2])
run_graph( [4,5,6])


# Write the summaries to disk
writer.flush()


# cLose the SummaryWriter
writer. close()


# α．05e the sessiz가1
sess. close()




                                                      그래프를name scope로구성하기    - 103


===== PAGE 116 =====
    결론

    알아야 하는 많은 내용들이 있었다. 원리를 이해하려면 텐서플로우로많은 실습을 해봐
    야한다．                                         머릿속에 그래프를만
       Operations, Variables, Sessions어］익숙해지도록 하고，
    들고 실행하는방법을잘새겨 넣자．

    어떤사람에게는 간단한수학문제를텐서플로우로 푸는 것이 재미있을수 있다．
                                         그러나

    우리는 아직까지 머신 러닝과 같은 라이브러리는 사용해보지 않았다. 다음장에서 머신
    러닝의 기본 개념과 기술들, 그리고 텐서플로우에서 사용하는 법을 소개할 것이다．




CHAPTER 3 텐서플로우 기본


===== PAGE 117 =====
跡뵤出＝ 。


===== PAGE 118 =====
    이제 우리는 텐서플로우가 작동하는 기본방식을 알고 있다. 이제는 텐서플로우의 중요
    한사용목적인머신 러닝machine [earning을 이야기할준비가 되었다．

    이제부터 기본적인머신 러닝의 개념들을 소개하고 텐서플로우에서 어떻게 구현하는지
    소개할것이다．




    지도학습
       （Supervised Learning) 기초

                                                지도학습이란 입력
    이 책에서 우리는 지도학습supervised learning 문제에 집중할것이다．
    데이터 집합과 그 집합의 각 예제 샘플에 대한 실제 또는 기대하는 결과값을 가지고 추
    론 모델inference mode
                     ［을 학습시키는 것을말한다. 이 모델은 초기의 학습데이터 집합에
    는존재하지 않는 새로운 입력에 대한 결과값을 예측할수 있다．

    추론 모델은 데이터에 적용되는 일련의 수학적인 오퍼레이션이다. 각단계는 코드에 의
    해만들어지고 주어진문제를풀기 위해 우리가사용하는 모델에 의해서 결정된다. 우리
    의 모델을 구성하는 오퍼레이션은 고정되어 있다．
                             각 오퍼레이션 내부에는 " multiply
                                   이러한 값들은 학습 과정 동안에 모델
    by 3", "add 2" 와 같은 임의의 값들이 있는데，
    이 출력 결과를 학습하고 조절하기 위해서 변경되는데 이들을 그 모델의 파라미터
          「라고한다.
    paramete

    추론모델은사용되는오퍼레이션의 개수，
                      결합되는방식, 사용되는파라미터의 개수등
    에 따라 다양하게 변경될 수 있지만, 학습을 위해서는 언제나 동일한 일반적인 구조를
    적용한다．


                                            Training loop


          Initiakze
                                                Execute 1nference
          modei        hput training data                                Compute loss
                                                mode] on training data
          parameters



                                              Adjust model parameters




CHAPTER 4 머신 러닝 기초


===== PAGE 119 =====
계산그래프는다음과같은반복적인학습과정training loop을 거친다：

  ·   처음에 모델 파라미터를초기화한다. 대부분 이를 위해서 랜덤값을사용하는데，
      d-          ---1




      단순한모델인 경우에는0으로 초기화하기도 한다．
  ·   각샘플에 대해서 학습데이터와원하는출력값을 읽어 들인다. 여기서 대부분의
      오퍼레이션은 데이터의 순서를 랜덤하게 바꾸어서 모델에 입력되는 데이터의
      순서를다르게 한다．
  · 학습 데이터를 이용해서 추론모델을 실행한다. 이 단계에서 모델 현재의 파라미
      터를 이용해서 각학습 입력 예제에 대한출력을 계산한다．
  ·   손실〔oss값을계산한다. 손실값이란학습데이터에 있는목표출력값으로부터 방
      금 계산된 값이 얼마나 다른 지를 의미한다. 다양한손실 함수들이 이 책에서 소
      개될 것이다．
  · 모델 파라미터를조절한다. 여기서 실제적인학습이 수행된다. 주어진 손실함수
      를 이용해서 여러 번의 학습단계를 통해서 손실값을 최소화하기 위해서 파라미
      터를 수정하는 것을 의미한다．
                     일반적으로 우리는 기울기 하강 알고리즘gradient
      descent algorithm을사용하는데，
                             다음절에서 설명할 것이다．


이러한반복 과정은 학습률learning rate, 사용하는 모델과 입력 데이터에 따라서 여러 번
반복수행된다．

학습후에는예상 결과값이 있는다른데이터에 대해서 추론 모델을 실행해보는 평가단
계evaluation phase를 실행한다．
                       학습과정 중에 모델에게 전해지지 않은학습데이터를사
용해서 학습을 넘어서 얼마나잘 예측하는지를 판별하는작업이다. 보통은 초창기의 데
이터셋을70％는학습에, 나머지 30％를 평가단계에 사용한다．

학습모델의 코드는 보통다음과 같은구조를 가지게 된다．




                                       지도학습
                                          （Supervised Learning) 기초   - 107


===== PAGE 120 =====
          import tensorfiow as tf


          # Lflttt(九ize variabLes/modeL parameters


          # define the training Loop operations
          def in-Ference(X):
              # compute inference modeL over data x and return the resuLt


          def loss(X, Y) :
              # compute Loss over training data x and expected outputs V


          def inputsQ:
              # read/generate input training data x and expected outputs V


          def train(total_loss):
              # train / adjust modeL parameters according to computed totaL Loss


          def evaluate(sess, X, Y) :
              # evaLuate the resuLting trained modeL


          # Launch the graph in α sessionJ setup boiLerpLate
          with tF.Session() as sess:


              tF.initialize_all_variables() .run()


              X, V = inputs()


              total_loss = 1oss(XJ Y)
              train_op = train(total_loss)


              coord = t-F.train.Coordinator()
              threads = tf. train.start_queue_runners(sess=sess, coord=coord)


              # actuaL training Loop
              training_steps = 1000




1081 CHAPTER4 머신 러닝 기초


===== PAGE 121 =====
    for step in range(training steps):
        sess.run([trainop])
        # for debugging and Learning purposes, see how the Loss gets
          decremented thru training steps
        i-f step % 10 == 0:
            print "'loss: ", sess.run([total loss])


    evaluate(sess, X, Y)


    coord .request_stop()
    coord.join(threads)
    sess.close( )



위의 코드가 추론 모델 코드의 기본적인 형식이다．
                          먼저 모델 파라미터를 초기화하고，
반복학습과정을 정의한다．
            입력 학습 데이터를 읽. .input method, 추론모델을 계산하고
inference method, 예상출력값과의 비교를통해서 손실을 계산하고toss method, 모델 파라
미터를 갱신하고train method, 결과 모델을 평가한다evaluate method. 그 이후에는 세션을
시작하고반복학습을 실행하는 코드이다. 다음 섹션에서 위의 비어 있는메소드들을채
워 넣자．

모델의 전반에 대한 이해가 되면, 작업하고자하는데이터에 실제로 적용해볼수 있다．




학습 체크포인트 저장하기

위에서 이야기한 바와 같이 학습이라는 것은 텐서플로우에서 사용하는 용어로는 많은
학습 사이클을 통해서 파라미터 또는 변수들을 갱신하는 과정을 의미한다. 변수는 메
모리에 저장된다. 그래서 몇 시간동안의 학습후에 전기가끊기면, 모든 결과물을 잃어
      이를 해결하기 위해서 이진 파일binary file로 그래프의 변수들을 저장하는
버릴 것이다．
tf.train.Save
            「라는 클래스가 있다. 주기적으로 변수들을 저장하고 체크포인트 파일
을만들어서, 필요한경우에 원하는지점부터 다시 학습을 시작할수 있다．




                                                         학습체크포인트저짇빠기   - 109


===== PAGE 122 =====
    Saver를사용하기 위해서 반복학습과정을 조금 수정해야한다．


     # modeL defin{Hon code . . .
     # Creαte α saver.
     saver = t-f.train.Saver()


     # Lαunch the graPh in α 5es5tor), setup boLLerpLate
     with t-1.Session() as sess:


         # modeL setup. . . .


         # actuaL traLnLng Loop
         for step in range(training_steps) :
             sess.run([train_op])


             if step % n…
                  saver. save(sess, 'my-model', global_step=step)


         # em九uati아7. . .


         saver. save(sess, ' my-rnDde1', global-step=training steps)


         sess . close()


    위의 코드에서 세션을 열기 전에 saver의 인스턴스를만든다. 그리고반복학습 중에매
    1000 스텝마다, 그리고 학습을 종료할 때 tf . train.Saver, save 메소드를 호출한다．
                           과 같은 형식으로，
    각 함수 호출은 my-model-{step｝        예를 들면 my-model-1000, my-
    model-2000, 체크포인트 파일을 생성한다. 이 파일에는 각 변수들의 현재 값이 저장된

    다. 디폴트로 saver는 가장 최근의 5파일만보관하고 나머지는 지운다．

                      tf .train.get_checkpoint state 메소드
    특정 지점에서 학습과정을재개하려면，
         이메소드는저장된 체크포인트가 있는지를 검증하고，
    를사용한다．                        tf.train.Saver.
    restore 메소드를통해서 변수값을복구한다．




CHAPTER 4 머신 러닝 기초


===== PAGE 123 =====
with tf.Session() as sess:


   # modeL setup....


    initial_step = 0


   # yeni力／ if we don't have α checkpoint saved aLready
    ckpt = tf. train.get_checkpoint_state(os.path.dirname(_ file_ ))
   if ckpt and ckpt.model_checkpoint_path:
        # Restores from checkpoint
        saver. restore(sess, ckpt.model_checkpoint_path)
        initial_step = int(ckpt.model_checkpoint_path.rsplit( ' -', l) [1J)


    #actuaL tr《九fling LooP
    for step in range(initial_step, training_steps):




위의 코드에서는 체크포인트 파일이 있는지 먼저 검사하고, 반복 학습을 시작하기 전

에 변수값을 복구한다. 체크포인트 파일 이름으로부터 전역 변수인 반복 횟수도 복구

한다．

이제 지도 학습의 개괄적인 이해와 학습 과정을 저장하는 법을 배웠으니까, 추론 모델을
배워보자．




선형 회귀
    （Linear Regression)

선형 회퀴는 지도 학습문제를모델링하는 가장 단순한 형식이다. 학습 데이터로써 데이
터 집합이 주어진다면, 그 학습 데이터에 가장 잘 맞는 선형 함수Unear function를 찾을 수
있다. 2차원데이터 집합에서 그러한함수는 직선으로 표현된다．




                                                           선형 회귀
                                                               （니near Regression)   - lii


===== PAGE 124 =====
                                 Linear regression
                                                                                   ●        *
                                                                          ●                     Training
                           400                                                                  dataset
                                                                                                p이n1
                                                                                            ■■Model


            8으섧＝    8
                    =0
                           300                                                                premdi아｀




                ＞m＝
                                      S



                  尸
                           200 ●



                           100



                            0
                                 20         30              40                50       60

                                                     input variable (X》




    위는 2차원상의 선형 회귀 모델의 그림이다. 파란 점은 학습 데이터이고, 붉은 선은 모
    델이 추론할 대상이다．

    선형 회귀 모델을 설명히끼 위해서 약간의 수학으로 시작하자. 선형 함수의 일반적인 형
    식은아래와같다：


                    y(x1, x2,...,xk) = w1x1+ w2x2+ ...+ wrk+ b


    위의 식을 행렬
           （또는 텐서）
                 형식으로 나타내면：


                         Y= XWT+ b where X= (x1, ...,x1jW= 佃1' …，Wk)

       ·   γ는예측
              （추론）
                 하고자하는값이다．
       . X;, …，兀는 새로운 값을 예측하기 위해서 모델을 사용할 때 제공하는 값으로써
           서로 독립independent 변수이다．
                                행렬의 형태로 주어지면 한 줄당 하나로써 여러
           개의 예를동시에 제공할수 있다．
       ·   WI, ..., Wh는학습 데이터로부터 학습해야하는모델의 파라미터로써, 각 변수에
           주어지는 웨이트weight라고도한다．



애APTER 6 머신 러닝 기초


===== PAGE 125 =====
                        모델의바이어스bias로알려진선형함수
     · ,b도또한학습해야하는파라미터로써，
         의상수이다．

이 모델을 코드로 표현해보자．
               .웨이트의 전치 행렬tranposing을 구하는 대신 열 벡터
cotunin vecto
           「로 표현하자．


# initiaLize.variabLes/modeL para,meters
                                        t
 W =     tf.Variab1e   (tf.   zer。
                                 s      2,
                                        '          1]        ), name=     "weights       "   )
 b   =   tf. Variable 0.      name=
                                  ,"bias



                              fI)   b
                                            %OO-
                                                        ")
                                                              令，
                                                                   diJi
                                                                                     :
                                                                                             ,:.,,,，忙았       :1
 def inference(X) :
                                                                           얜식
         return t-f.matmul(X, W) + b



이제 우리는 손실을 계산할 방법을 정의해야 한다. 이러한 간단한 모델에서 우리는 각
학습 샘플의 목표값과 계산된 값
                （추정값）
                    의 차이의 제곱，
                            즉 제곱 에러squared erro를 사
용한다. 이 값은수학적으로는목표값 벡터와추정값 벡터의 유클리디언 거리euclidean
distance이다. 2차원 데이터셋에서 그림으로 생각하면 예측된 값에서 선형 함수 그래프
로 향하는 수직선의 길이를 의미한다. 이는L2 norm 또는L2 손실 함수라고 한다．
                                              제곱
근 계산을 피하기 위해서 이 값을 제곱한다. 이렇게 하더라도 손실을 최소화하는 것은
달라지는 것이 없이 계산단계를줄일수 있기 때문이다．


               loss = Z (yi- y_predicted1)2


戚는각 예제 데이터를 의미하는데, 전체 i를통해서 합산한다. 코드상으로는：

 def loss(X, V) :
         V_predicted = in-ference(X)
         return tf. reducesum(t-F. squared_dif-ference(Y, V_predicted))


O]7fl데' 떠를 ' 1*해서우리의모델을실제로학습시킬시｛1-O1다 -r
                                     '定》  쁘뜨
                                         pyears-'-r
                                                e1 11'-i-겐
                        （hnP仰e0P'"
戶峻〔깟완혈르크火섶붙콴읜沓峰젖르：曼聖브뾰브쁘塑

                                                                                                         선형 회귀
                                                                                                             （니near Regression)   1113


===== PAGE 126 =====
                 sc.fsu.edu/-jburkardt/datasets/regression/x09.txt).

                 크기가크기 않기 때문에, 코드 속에 이 데이터를삽입하자. 다음 섹션에서는 파일에서
                 학습데이터를 읽어 들이는 법을사용할 것이다．


def inputs() :
    weight_age = [[84, 46], [73, 20], [65, 52], [70, 30], [76, 57], [69, 25],
[63, 28], [72, 36], [79, 57], [75, 44], [27, 24], [89, 31], [65, 52], [57, 23],
[59, 60], [69, 48], [60, 34], [79, 51], [75, 50], [82, 34], [59, 46], [67, 23],
[85, 37], [55, 40], [63, 30]]


    blood_fat_content = [354, 190, 405, 263, 451, 302, 288, 385, 402, 365, 209, 290,
346, 254, 395, 434, 220, 374, 308, 220, 311, 181, 274, 303, 244]


    return tf. to_float(weight_age), tf. to_fioat(blood_fat_content)



                 이제는모델의 학습오퍼레이션을 정의하자. 기울기 하강 알고리즘을사용해서 모델의

                 파라미터를 최적화한다. 이 내용은다음 섹션에서 설명한다．


def train(total_loss) :
    learning_rate = 0.0008001
    return tf. train.GradientDescentOptimizer(learning-rate) .minimize(total_loss)



                 실행할때, 각학습단계마다손실이 어떻게 작아지는지 출력된다．

                 이제 모델의 학습을 마쳤으니 모델을 평가할 시간이다. 몸무게가 80킬로그램인 25살의
                 혈중 지방 성분의 예상치를 계산해보자. 이 데이터는 원래의 학습 데이터에 있지 않았
                 다. 그러나 같은나이의 65킬로그램의 다른사람과 비교해보자．

                  def evaluate(sess, X, Y):
                       print sess. run(inferen ce([[80. J 2 5 1])) # , 303
                       print sess. run(in-Feren ce([[65., 25 ]])) # N 256




 11띠     CHAPTER 4 머신 러닝 기초


===== PAGE 127 =====
간단한 평가를 통해서 모델이 몸무게에 따라서 혈중 지방 성분이 어떻게 줄어드는지를
체크하였다. 그리고 출력값들이 원래의 학습 데이터들의 경계 사이에 위치함을 알 수
있다．




로지스틱 회귀
      （Logistic Regression)

선형 회귀 모델은 연속continuous적인 값또는 실수값
                               「eal numbe읕 예측한다. 이제 우리
는 " 이 이메일은스팸입니까？" 와같은yes-no 형태의 질문에 답할수 있는모델을 제시
한다．

머신 러닝에서 자주 사용되는 로지스틱 함수〔ogistic function가 있다．
                                            이 함수는 모양이
                이기때문에시그모이드sigmoid향I＝라고한다．
S(Sigma는S의그리스문자다）


                         1
                J
                 (x) =1 + e-x

      l力




      0. 5




                           甲   1
                               r   1
                                   。   "
                                       r   ·
                                           H   m   寸   n    山   卜   m       。
                                                                            ㅐ
      0.   0유
                  甲   '}
                                                                        이




위의 그림이 모양이 " S" 인로지스틱／시그모이드함수의 그래프이다．



                                                           로지스틱 회귀
                                                                 （Logistic Regression)   - 115


===== PAGE 128 =====
    로지스틱 함수는 특정한 입력값이 주어지면 출력값이 success일 확률을 계산하는 확률
    분포함수probability distribution function이다．즉질문에 대한대답이 " yes" 일 확률을출
    력한다．

    이 함수는 하나의 입력값을 받는데, 우리의 학습 데이터와 같은 다차원공간 또는 다차
    원특징값들을 사용하기 위해서는 이들을 하나의 값으로 결합해야한다. 이를 위해서 위
    에서 소개했던 선형 회귀 모델 식을사용할수 있다．

    선형 모델의 코드를 재사용할 수 있는데 시그모이드를 적용하기 위해서 약간의 수정이
    필요하다．

     # same 尸arams αnd var1abLes initiα LLzati아〕as Log reg.
     W = t-f.Variable(t-F. zeros([5, 1]), name="weights ')
     b = t-f.Variable(0. , name="bias")


     # former inference is now used for combLnthg thputs
     def combine_inputs(X):
         return tf. matmul(X, W) + b


     # new inferred 以孔ue is the 51gm01d appt1ed to the former
     def in-ference(X):
         return tf. sigmoid(combine_inputs(X) )




    이제 이 모델을 위한손실 함수에 집중해보자. 제곱 에러squared erro
                                             「를 사용할 수 있었
    다．
     ‘로지스틱 함수는'노es" 라고 답할 확률을 계산한다．
                                  학습 샘플에서 " yes" 라는 대달寸
    또는1의 출력값은 100％의 확률을 의미한다. 여기서 손실 값은 그 샘플에 대하여 모델
    이 제시한1보다작은값의 제곱값을의미한다. 따라서, "no" 라는답은확률0을의미하
    며, 그래서 손실값은그모델이 예제에 대하여 제시한확률값의 제곱값을 의미한다．

    기대되는대답이 " yes" 이고모델이0에 가까운아주작은확률값을제시하는경우를고
    려해보자. 이것은그대답이 "no" 일 가능성이 100％라는것을의미한다．




CHAPTER 4 머신 러닝 기초


===== PAGE 129 =====
이러한문제에 더 잘동작하는크로스 엔트로파cross entropy라는손실함수가 있다．


loss = - Z (yi' log(y_predicted1) + (1- yi) ' log(1- y_predicted1))


"yes" 라는 예측 결과값에따른이 두손실함수의 행동을 시각적으로 비교할수 있다．

            5



                                             L2
                                             L에istic....

            3




            2




            ㅇ

                                                       口
                                                       qH
                        .N1 。                                           。。· 。




위의 그림은 크로스 엔트로피와 제곱 에러
                     （L2) 함수의 그림이다. 크로스 엔트로피는 출
력값이 원하는 값보다 훨씬멀기 때문에 훨씬큰 값을출력한다
                              （"penalizes").

크로스 엔트로피는 예상확률값이 " yes" 예제에 대해서는 0에 가까이 가는 경우에，
                                              페
널티는 무한대에 가까이 증가한다. 이것은모델이 학습 이후에 잘못된 예측을 하는 것을
불가능하게 만든다. 이런 점이 크로스 엔트로피가 이 모델을 위한 손실 함수로써 더 적
당한 이유가 된다．




                                                 로지스틱 회귀
                                                       （Logistic Regression)    1117


===== PAGE 130 =====
                  텐서플로우에는한 번의 최적화된단계로 시그모이드 함수를 위한 ㅋ쿠ㅅ 엔트로피를

                  직접 계산하는 방법이 있다．


def loss(X, Y):
    return tf.reduce_mean(tf.nn. sigmoid_cross_entropy_with_logits(combineinputs(x),Y))




                                         ㅋ 쿠 ㅅ 엔트로피의 의미

                  정보 이론
                      （information theory）
                                         에서 새넌 엔트로피
                                                  （Shannon entropy）
                                                                  는 심볼들의 문자
                  열에서 심볼 Si를 인코딩하기 위해서 필요한 최소 평균 비트수를 그 문자열에 나타나는 각
                  심볼들의 확률값
                         （/',）에 의해서 추정할 수 있도록 해준다．



                        H= - Z (p1.1og2(p1))
                                  z




                  이 엔트로피 개념을 엔트로피의 열역학 개념과 연결해서 수학적인 표현으로 유사하게
                  사용할 수 있다．

                  예를들어, 단어 "HELLO"를위한 엔트로피를계산해보자．


                        p("H") = P("f " ) = p("O") = 1/5 = 0 . 2

                        P(" t " )= 2/5 = 0 . 4

                        H= _3* o.2* 10g2(0.2) _0.4* 1og2(0. 4) = 1. 92193


                  그래서 최적의 인코딩으로''HELLO"를 인코딩 하기 위해서 심볼들마다 2비틔 필요하다．

                  만약 실제의 확률값／’가 아니라 q1라는 확률값을 사용한다면，
                                                   각 심볼의 인코딩을 위해서
                  더 많은 비트가 필요할 수도 있다. 이것이 크로스 엔트로피를사용해야 하는 이유이다．




    1181 CHAPTER4 머신 러닝 기초


===== PAGE 131 =====
         //=- Z (p1. log2(q1)

예를 들어서，
      ASCII 코드에서 q, = 1/256의 동일한 확률로 모든 심볼에게 확률값을 부여한다고 하자．
이 경우에 "HELLO" 단어의 크로스 엔트로피를계산해보가．


         q("H") = q("E") = q("L") = q("O") =1/256
         H= _3* o.2* 10g2(1/256) _0.4* 1og2(1/256) =8
                                                U 녑盤
                                                口乙，D

그래서 예상하는 대로 HELLO 단어를ASCII 인코딩에서 표현하려면 8비트가 필요하다．

손실 함수에서，
       β를 학습 목표치와 분포 함수
                      （인코딩）
                          라고 할 때，
                                실제값은 100％이며 0이 아
니다. 그리고 q를 모델이 계산한 결과값이라고 생각하자. 시그모이드 함수가 확률을 계산한
다는 점을 기억하자．

크로스 엔트로피는／'＝α인 경우에 최소값이 된다. 그래서 크로스 엔트로피를분포
                                          （distribution)
들간의 비교 방법으로 사용할 수 있다. 크로스 엔트로피가 엔트로피에 가까울수록，
                                           q가／洲
더 근사해진다. 그렇게 되면, 크로스 엔트로피는 모델이 추정치를 더 잘 샘플링 할수록 감소
하게 된다．

엔트로피를 최소화하기 위해서 log2를 log로 바꿀 수 있다. 로그의 밑
                                        （base) 값의 변화를 곱
해주면 되기 때문이다．




이제 그 모델을특정 데이터에 적용해보자．
                     https://www.kaggle.com/c/titanic/datα에서

Titanic survivor Kaggle contest 데이터를사용할 것이다．

이 모델은 승객의 나이, 성별, 티켓 종류어］따라서 그 사람이 구조되었는지 아니었는지

를유추할것이다．

문제를좀 더 흥미롭게 만들기 위해서, 이번에는 파일에서 데이터를 입력받자. train.



                                               로지스틱 회귀
                                                     （Logistic Regression)   - 119


===== PAGE 132 =====
               csv 파일을 다운받자．

               아래는 파일을 입력받기 위한 코드이다. 로드해서 파싱할수 있고 추론 과정을 효율적으
               로 하기 위해서 하나의 텐서 안에 있는 여러 줄을 읽어 들이도록 배치batch를 구성할 수

               있다．


def read_csv(batch_size, file_name, record_defaults) :
    filename_queue = tf. train. string_input_producer([os .path.dirname(_ flle_ ) +
"I " + file_name])
    reader = tf. TextLineReader(skip_header_lines=1)
    key, value = reader.read(filename_queue)


    # decode_csv wiL〔 convert α Tensor from type string (the text Lmne) in
    # α tupLe 0f tensor coLumns with the specified defauLts, which aLso
    # sets the data type fOr each coLumn
    decoded = tf. decode_csv(value, record_defaults=record_defaults)


    # batch actu쑈Ly reads the fiLe and Loads "batch_size" rows in α singLe tensor
    return t-F.train. shuffle_batch(decoded, batch_size=batch_size,
capacity=batch_size * 50, min_after_dequeue=batch_size)



               이 데이터셋에서 카테고리 데이터categoricaL data를 사용해야한다. 티켓 종류와 성별은
               사용할수 있는 미리 정해진 가능한 값들을 가진 문자열이다. 추론 모델에서 이들을 사
               용하기 위해서는, 이 값들을숫자값으로 叩직야 한다. 가장 쉬운 방법은 각 가능한 값에

               숫자를 할당하는 것이다. 예를 들어, 1등급 티켓 종류에 " 1" 을 할당하고, 2등급 티켓에
               "2"를, 3등급에는 " 3" 을할당하는 방식이다. 그러나 이 방식은 값들 사이에 실제로는존
               재하지 않는 선형적tinea「인 의미를 강요하게 된다. 실제로 " 3등급 티켓이 1등급 티켓의
               3배" 라고 할 수는 없다. 이와달리 각각의 카테고리 특징값을 N개의 불리언특징값으로
               확장해서 원래 값이 가능한 값들 중에 하나를 가지도록 해야 한다. 이렇게 하면 모델이
               각각의 가능한 값들을 서로 독립적으로 학습할 수 있게 된다. 우리의 예제 데이터에서
               "1등급 티켓" 은다른 것들보다 더 큰 생존자 확률을 가져야 한다．




 120 -   CHAPTER4 머신 러닝 기초


===== PAGE 133 =====
종류 데이터를 사용할 때는, 각 가능한 값마다 하나씩 부여해서 여러 개의 불리언 특징
값으로 바꿔야 한다. 이렇게 하면 모델이 각 가능한 값의 가중치를 별개로 부여할 수 있
게 된다．

위의 데이터 집합에서 성별과 같이 단지 두 개의 가능한 값을 가지는 카테고리인 경우에
는, 변수하나를가져도 된다. 값들사이의 선형적인관계를표현할수 있기 때문이다. 예
를들어서 female =1이고 male=0이라면, male = 1 - female로구할수 있고, 하나의
웨이트만으로 두 개의 가능한상태를 표현할수 있다．


 def inputsQ:
    passenger_id, survived, pclass, name, sex, age, sibsp, parch, ticket, fare,
 cabin, embarked = \
     read_csv(100, "train.csv", 〔[0.0], [0.0], [0], [" " ]J [" " ]J [0.0]) [0.0]' [0.0],
["] , [0.0], ["1 ' ["] ])


    # convert categoricaL data
    is_first_class = tf. to_float(tf. equal(pclass, [1]))
    is_second_class = tf. to_float(tf. equal(pclass, [2]))
    is_third_class = tf. to_float(tf. equal(pclass, [3]))


     gender = tf. to_float(tf. equal(sex, ["female"]))


    # FinaLLy we pack αLL the features in α singLe matrix;
    # We then transpose to have α matrix with one exampLe per row and one feature
per coLumn.                           和＆ 벼겅
     features = tf. transpose(tf. j)ac.k([is_first_class, is_second_class, is_third_class,
                                  `   ∼




 gender, age]))
     survived = t-F.reshape(survived, [100, 1])


     return features, survived


위의 코드에서 입력을 위해서 read_csv를 호출하고 데이터를 변환하였다. 불리언으로
변환하기 위해서 우리는 특정 상수값과동일힌씨 비교하는 일에 tf.equal 메소드를사




                                                         로지스틱 회귀
                                                               （Logistic Regression)   - 121


===== PAGE 134 =====
              용한다．
                 또한불리언 값을숫자값으로 되돌리기 위해서 tf. to-float를 사용한다. 그런
              후모든불리언값을tf.pack로 하나의 텐서로 묶는다．

              마침내 이제 우리의 모델을학습시키자．


def train(total_loss):
    learning_rate = 0.01
    return tf. trairi.GradientDescentOptimizer(learning_rate) .minimize(total_loss)



              결과를 평가하기 위해서, 추론을 학습 세트에 대해서 수행하고 정확하게 예측된 예제의
              개수를셀 것이다．
                      이것을 정확도accuracy라고한다．


def evaluate(sess, X, Y) :

    predicted = t-f.cast(in-ference(X) > 0.5, tf. float32)

    print sess.run(tf. reduce_mean(tf. cast(tf. equal(predicted, Y), t-F.float32)))



              이 모델이 답이 " yes" 가 될 확률을 계산하기 때문에，
                                              예제의 출력값이 0.5보다 크면긍
              정적인답안으로 변환해야 한다. 그리고 tf.equal을 이용해서 실제값과의 동일성을비
              교한다. 마지막으로 정답의 비율을 계산하기 위해서 정답의 개수를 세고，
                                                    배치 작업에서
              모든샘플의 개수로나누는tf. reduce_mean을사용한다．

              위의 코드를 실행하면 80％의 정확도를 얻을 것이다. 이 정도면모델의단순성을 고려하
              면좋은수치이다．



              소프트맥스 분류
                     （Softmax CLassification)

              로지스틱 회귀로yes-no문제에 답할수 있는모델을만들수 있었다．
                                                이제는 "당신은보
              스톤，
                런던, 시드니 중에 어디서 태어났나요？" 와같은 다중 선택형에 답할수 있는 모델
              을 원한다．




  i2a -   CHAPTER4 머신 러닝 기초


===== PAGE 135 =====
이런 경우를 위해서 소프트맥스＄oftmax 함수가 있다. 이는C 개의다른값들에 대한로지
스틱 회귀를 일반화한 것이다．

           功
           只      ㅡ

                                  一 forc= O. . . C- i
                              1       j
                          ,
                      一
                      乙
                      ，
                          ．
                                  "       '




                          尸
위의 식은C개의 요소component를 가지는확률벡터를돌려주는데, 각각은각출력 클래
스와 연관된 확률값이다. 이것이 확률값이기 때문에 C개의 값의 합은 언제나 1이다. 위
의 식 자체가 가능한 예제들을 100% 포함하기 위해서 모든 가능한 입력 예제가꼭 하나
의 출력 클래스에 속해야하기 때문이다. 따라서, 만약그 합이 1보다작다면, 숨어있는
클래스가 있음을 암시하는 것일수 있다. 1보다크다면,각예제가 하나 이상의 클래스에
속한다는 것을의미할수도 있다．

클래스가 2개인 경우는 결과 출력 확률값이 로지스틱 회귀 모델과 동일하다는 것을 증
명할수 있다．

이제 이 모델을코딩하기 위해서, 변수초기화에서 이전 모델을 약간수정할 것이다. 우
리의 모델이 하나가 아닌 C개의 출력값을 계산하기 위해서는，
                                각 출력값마다 하나씩해
서 C개의 다른 웨이트 그룹이 필요하다．
                     그래서 우리는 웨이트 벡터weight vecto
                                             「대신 웨
이트 행렬weight matrix을사용할것이다. 이 행렬은각 입력 특징값마다하나의 행을가지
고, 각출력 클쾌스마다 하나의 칼럼을 차지한다．

우리는 httpsi/archive.ics.uci.edu/ml/datasets/Iris에서 다운받은 고전적인Iris 꽃 데이
터 집합을 이용해서 소프트맥ㅅ를 실험할 것이다. 이 데이터는4개의특징값을 가지고3
개의 가능한출력 클래스가 있어서, 웨이트 매트릭스는4x3 차원이다．

변수초기화코드 부분은 아래와같다：

 # this time weights form α matrix, not α vector, with one "feature
 weights coLumn" per output cLass.




                                                    소프트맥스분류
                                                          （Softmax Classification)   - 123


===== PAGE 136 =====
            W = tf.Variable(tf.zeros([4, 3]), name="weights' )
            # so do the bthses, one per output cLoss.
            b = tf.Variable(tf.zeros([3]), name= "bias")


           또한당신이 예상하는바와같이, 텐서플로우는소프트맥스함수의 구현을제공한다．

            def in-ference(X):
                return tf. nn. softmax(combine_inputs(X))



           손실 계산과 관련해서는 여기서의 출력도 확률값이기 때문에 로지스틱 회귀를 위한 동
           일한 고려 사항이 후보 손실 함수를 맞춰갈 때도 필요하다. 그래서 계산된 확률값에서
           여러 개의 클래스에 맞추어서 크로스 엔트로피를다시 사용할 것이다．

           하나의 학습 예제／를 위해서 크로스 엔트로피는아래와같다．


                      loss1= - Z U/c·log(y. predicted))

           모든 학습 예제에 대해서 각 출력 클래스의 손실을 더한다. γ,는 학습 예제의 예정된 클
           래스를 위해서는1의 값을, 그리고 그 외의 클쾌스를 위해서는 0이 될 것이다. 그래서단
           지 하나의 손실 값만이 실제로는 합해진다. 이는 그 모델이 예측한 확률값이 실제 클래
           스에서 얼마나 멀리 떨어져있는지를 의미한다．

           모든학습 집합에 대해서 손실 합계를 계산하기 위해서 모든학습 샘플들의 손실을통합
           하자．

           코드에서 소프트맥스 크로스 엔트로피 함수를, 텐서플로우에서 구현한 두 가지 버전이
           있다：하나는 예제마다 하나의 클래스 값을 가지는 학습 샘플을 위해 최적화된 것이다．
           예를들어，
               우리의 학습데이터는 " dog", "person", "tree" 중에 하나의 클래스값을가
           지는경우에는tf.nn. sparse_so-Ftmax cross entropy-with logits함수를사용
           하자．




1241   CHAPTER4 머신 러닝 기초


===== PAGE 137 =====
def loss(X, Y):
    return tf.reduce_mean(t-f.nn.sparse_so-Ftmax_cross_entropy_with_logits
(combine_inputs(X),Y))
L耐ㅍ：:                            斌棺
다른 하나는 각 예제의 확률값이 모든 클래스에 속하는 학습 샘플에 동작하는 경우이
다．    " 질문을 받은 사람의 60％가 이 그림은 dog에 대한 그림이고，
 예를 들어，                                   25％의 사
                                         이를 위해서 t-F.nn.
람은tree, 나머지는 " person" 이라고 생각한다" 와같은 경우이다．
softmax_c ross_entropy_with_logit s 함수를 사용하자. 실제 문제에 이러한 함수
를 사용할 수도 있다．
           그러나 이 책의 간단한 문제에서는 필요하지 않다．
                                     sparse 버전이
빠르기 때문에 더 선호된다. 모델의 최종출력은 언제는 하나클래스 값이다. 이 버전은

더욱 융통성있는학습 데이터를 지원하기 위한 것이다.

입력 방법에 대한 이야기를 하자. 로지스틱 회귀 예제에서 사용했던「ead_csv 함수를
다시 사용할 것이다. 모두 숫자로 이루어진 이번 데이터셋에 대해서 디폴트 값으로 호출

하자．


 def inputsO:                                       ,／乃 딨 두즌'ㅣ "인 기"'"ㅣ "｝
                                                                         幻 e的" 나牢 .

     sepal_        length,       sepa1_   wi9   '   h,   petal_   length,   petal_      width,     label   =\
    read_csv(Uc3, ""iris.c1ta'", LL ' ' Uj, LU " U」，L던 " U」）LE} ' U」， L "' "'ii)

    # convert cLass names to α o based cLass index.                                              d따∼
    label number =t-F.to int32(tf. argmax(t-F.to_int32(t-f.pack([
             tf. equal(label, ["Iris-setosa"]),
             t-F.equal(label, ["Iris-versicolor"]),
             tf. equal(label, ["Iris-virginica"])
     II))J    0)
                             )

 # Pack aLL the features that we care about in α singLe matrix;
     # We then transpose to have α matrix with one exampLe per row and one feature
Per coLumn.




                                                                                     소프트맥ㅅ 분류
                                                                                            （Softmax Classification)   - 125


===== PAGE 138 =====
    features = tf.transpose(tf. pack([sepal length, sepal-width, petal_length,
petal_width]))


    return -features, label number



              spa rse_softmax-c ross_entropy_with_logits를사용하기 위해서 각클래스를 해
              당하는 변수로바꿀 필요는 없다. 그러나 그값들이 O..2 사이의 값이어야 한다. 왜냐하면
              우리가 지금 3개의 가능한 클래스를 가지고 있기 때문이다. 데이터셋 파일에서 클래스
              는" Iris-setosa", "Iris-versicolor", "Iris-virginica" 중의 하나의 문자열 값을가진다．
                                                                                   이
              를 변환하기 위해서 t-F.pack으로 텐서를 생성하고, tf.equal을 이용해서 파일 입력과
              가능한 값을 비교한다. 그 다음에 tf. argmax로 참인 값을 가지는 텐서의 위치를 찾는
              다. 이로써 효과적으로클래스들을O..2 사이의 정수값으로 변환한다．

              학습함수는동일하다．

              정확도를평가하기 위해서, 시그모이드버전을조금고쳐야한다：


def evaluate(sess, X, Y) :
    predicted = tf. cast(tf. arg-max(inference(x), ]), tf. int32)
    print sess.run(tf. reduce_mean(tf. cast(t-f.equall(predicted, Y), tf. f]0at32)))



              추론은 테스트 예제에 대한 각 출력 클래스의 확률을 계산한다. t-F.argmax 함수가
              예측된 출력 값에서 가장 큰 확률값을 가진 것을 찾기 위해서 사용된다. 마지막으로，
              tf.equal로 목표 클래스와 비교하고, 시그모이드 예제와동일하게 tf. reduce_mean
            ' 을적용한다．

              코드를 실행하면 정확도 95％가나올 것이다．




        아｛APTER 4 머신 러닝 기초


===== PAGE 139 =====
     （MuLti-Layer NeuraL Networks)
다층 신경망

이제까지 우리는 언급하지는 않았지만 간단한 신경망을 사용했었다. 선형과 로지스틱
회귀 모델은아래의 관점에서 하나의 뉴런이다：

  ·     입력 값들의 가중치 합을 구한다. 바이어스bia＄는 모든 예제 샘플에 1의 값을
        가지는 입력 특징값의 웨이트로 간주한다. 이를 특징값들의 선형 조합〔 near
        combination이라고한다．

  ·     그런 후에, 출력값을 계산하기 위해서 활성화activation 또는 전송transfe
                                                      「 함수를

        적용한다. 선형 회귀의 경우에 활성화함수는 항등 함수identity function
                                                    （즉，같은
        값）
         을，로지스틱 회귀는 시그모이드함수를사용한다．


다음그림은각뉴런의 입력, 연산, 출력을보인다．




       x1


       x2                                                          outPUt
       x3           \\…
                           w2
               t-
                           w3-
        1           →｀…          ',




      inputs           weight         sum   transfer
                     multiplication         function



소프트맥스 분류softmax classification의 경우에 각 가능한 출력 클래스마다 하나씩 총 C

개의 뉴런을사용하는 신경망을사용한다；




                                                  다층 신경망
                                                       （Multi-Layer Neural Networks) 1127


===== PAGE 140 =====
                                                    outputl
                  xl


                                                    output2


                  1
                                                    output3




          이제 손으로 쓴 숫자 인식，
                        또는 이미지에서 고양이나 개를 식별하는 문제와 같은 더욱
          복잡한문제를해결하기 위해서,좀더 향상된 모델이 필요할 것이다．

          간단한 예제로 시작하자. XOReXdusive 0R 불리언 연산을 학습할 신경망을 만든다고 가
          정하자．

          표 4-1 XOR 연산의 진리표

         陌put 1        Input 2   0utput
         0             0         0
         0             1         1
         1             0         1
         1             1         0


          입력값중의 하나가1이면1을출력하고，
                            둘다0이거나1이면 0을출력해야 한다．

          이제까지 우리가도전했던 문제들보다 훨씬 간단한문제처럼 보이지만, 이제껏 사용했
          던다른모델들은 이 문제를 풀지 못한다．

          그 이유는 시그모이드 형태의 뉴런은데이터가 선형 분리 가늉inea n y separabLe한 경우에
          잘동작하기 때문이다. 이말은다음그림과같이 2차원데이터인 경우에는면의 한쪽에
          하나의 클래스에 속하는 모든 데이터가 배치되는 직선
                                     （고차원 데이터의 경우는 하이퍼



128 - CHAPTER4 머신 러닝 기초


===== PAGE 141 =====
플레인hyperplarie이 존재해야한다는것을의미한다．




                                        S        S


                       4"
                   .                    S                S
                            \
                                `
                   S
                                    ,
                                            ^
                                            `

                   .                            4'

                                                     \




이 그림에서는 예제 데이터가 자신이 속한클래스에따른 색상의 점으로나타난다. 빨간
점과파란점을완전하게 분리하는노란선을찾을수 있다면, 시그모이드뉴런은잘동
작할것이다．

XOR 게이트 함수를살펴보자：



          1




          0
              0




모든1
  （빨간 점）
       을한 면에，
            그리고모든0    을다른 면으로구분하는하나의 직선
                 （파란 점）
을찾을수 없다. XOR 함수출력은 선형 분리가 가능하지 않기 때문이다．



                                                         다층 신경망
                                                              （Multi-Layer Neural Networks)   1129


===== PAGE 142 =====
    이 문제는 실제로 1970년대에 십 여년 동안 신경망 연구가 침쩨기가 되게 만든 원인이
    었다. 그래서 그들은 신경망을 계속 사용하려고 선형 분리성의 부족을 어떻게 극복했을
    까？그들은 아래의 그림과 같이 신경망의 입력과출력 사이에 더 많은 뉴런을 삽입함으
    로써 극복했다．




                                                      output




          input layer   hidden layer   output layer



    이것을 입력 레이어와출력 레이어 사이에 뉴런들의 은닉 레이어hidden tayer을추가했다
    라고 말한다. 이것이 신경망이 입력 데이터에 다수의 질문을 할 수 있게 만든다고 생각
    할수 있다. 은닉 레이어의 뉴런 하나가 하나의 질문에 해당한다. 출력 결과는 이러한 질
    문들에 대한대답들에 기반한다．

    그림으로 나타내면, 이것은 신경망미 하나 이상의 분리선을 그리는 것을 허용하는 것을
    의미한다．




CHAPTER 4 머신 러닝 기초


===== PAGE 143 =====
           iS




                                  S




                                               S44
           0
               0     S                    1
                         S
                             S



위의 그림에서 볼 수 있듯이 각 직선은 입력 데이터에 대한 질문에 따라서 화면을 나
눈다．

당신은 이제 딥 러닝deep learning에서의 딥deep의 의미를추측할수 있다．
                                             우리는 더 많은
은닉 레이어를 추가함으로써 더 깊은 신경망을 만들 수 있다. 우리는 레이어들 사이를
다양한 형태로 연결할 수 있고, 심지어는 각 레이어에 다양한 활성화 함수를 사용할 수
도 있다．

이 책의 후반부에 우리는 다양한 사용 용도를 가지는 다양한 형태의 딥 신경망을 소개
한다．




                                   다층 신경밍KMuIh-Layer Neural Networks)   - 131


===== PAGE 144 =====
    기올기 하강법과 역전파
               （Gradient Descent and Backpropagation)

    우리가 지금 사용하는 학습 알고리즘의 동작방식을 설명하는 것으로 이장를마치려고
    한다．

    기울기 하강법은 함수가 최소값을 가지는 지점을 찾는 알고리즘이다. 우리는학습을수
    많은 단계를 거치면서 손실을 최소화하기 위해 모델의 파라미터를 조절해가는 과정이
    라고 정의했다는 것을 기억하자. 이 생각을 바탕으로, 모델의 손실 함수를 최소화하기
    위해서 기울기 하강법을 사용하는 것이 입력 데이터로부터 모델을 학습하게 되는 것
    이다．

    기울기가무엇인지 정의하자. 기울기는 일반적으로 V으로 표현되는 수학적 연산이다．
    미분derivative과유사한데, 기울기는우리가사용하는손실 함수와같이 벡터를 입력으로
    받고 하나의 값을출력하는함수에 적용된다．

    기울기의출력은함수의 입력 벡터 위치마다의 편미문partial derivative의 벡터이다．


            -
            V
              r a
              1=           .
                                     a   .   .   .   .   .
                                                                  a ,I
                   ` cw1' 《71472 "                           《7H7〃7
                                                             :-
                     =--       =--
    편미분은 함수가단지 하나의 변수만을 가지고 있고, 다른 변수들은 모두 상수로 생각해
    서 일반적인 미분을수행하면 된다．

    편미분은 특정한 입력 변수 하나에 대한 함수의 출력의 변화율을 측정한다. 이 말은 우
    리가특정 입력 변수값을증가하면출력값이 얼마나증가하는지를 의미한다．

    손실 함수의 입력 변수에 대해 말할 때, 이는 모델의 웨이트를 말하는 것이다. 실제적인
    입력 데이터의 특징값이 아니라는 것에 유의하자. 입력 데이터의 특징값들은 데이터 집
    합에 의해서 고정되는 것이지 최적화되는 것이 아니기 때문이다. 우리가 계산하는 편미
    분은추론모델에서 각각의 웨이트와관계된것이다．




CHAPTER 4 머신 러닝 기초


===== PAGE 145 =====
                  기울기의출력 벡터가손실 함수가 가장 커지는방
기울기라는 정보를 사용하는 이유는，
향을 가리키기 때문이다. 기울기는함수의 모든 지점에서 그 값을증가시키기 위해서 움
직여야하는 위치를 의미하는작은 화살표라고 생각할수 있다．




위의 그림이 손실 함수라고 생각해보자. 빨간 점은 당신이 지금 서있는 현재의 웨이트

값을 나타낸다. 기울기는당신이 손실을 크게 하는 오른쪽으로 가라고말한다. 또한, 화
살표의 길이는 개념적으로 그방향으로 움직이면 얼마나 이익을 얻을수 있는지를나타

낸다．

이제 기울기의 반대방향으로 간다면손실 또한반대로 줄어들 것이다．




                    기울기 하강법과 역전파
                               （Gradient Descent and Backpropagation)   -133


===== PAGE 146 =====
    그림에서 기울기의 반대 방향      으로움직인다면손실을줄이는방향으로움
                  （파란 화살표）

    직일 것이다．

    이제, 그 방향으로움직여서, 기울기를다시 계산해보자. 그리고 그과정을 기울기의 크
    기가0이 될 때까지 반복하자. 그러면 손실이 최소가 된다. 그것이 우리의 목표이다. 그
    림으로는 아래와같을 것이다．




애APTER 4 머신 러닝 기초


===== PAGE 147 =====
이제 끝이다. 기울기 하강 알고리즘을 아래와같이 나타낼 수 있다．


        weightsstep i + 1 = weightsstep i-'1" Vloss(weights5t.p i)

기울기 값의 크기를조절하기 위해서 n 값을추가하였다．
                            이를 학습률〔earning rate이라고
한다．
  기울기 벡터의 크기가실제로는 " 웨이트단위weight units" 가아니라 "손실함수단
위［oss function units" 로 측정되기 때문이다. 그래서 웨이트에 추가할수 있도록 기울기의
크기를조절할 필요가 있다．

학습 률은 모델이 추론을 통해서 얻는 값이 아니다. 그것은 우리의 모델에서 수작업으로
값을 조절하는 하이퍼 파라미터hyper paramete「이다．
                                 그래서 어떤 값이 적절한지 알아야
한다. 이 값이 너무 작으면 최소의 손실값을 찾기 위해서 많은 학습 사이클을 수행해야
한다．
  반대로 너무 크다면 최소값을 건너 뛰어서 찾지 못할 수도 있다. 또는반복적으로
건너뛸수도 있다．
        이를오버 슈팅overshooting이라고 한다．
                                 우리의손실함수 예제에서는
아래와같을것이다．




                             기울기 하강법과 역전파
                                        （Gradient Descent and Backpropagation)   1135


===== PAGE 148 =====
    실제로는 변수가 많아서 손실함수를 시각적으로 그리기 어렵다. 오버 슈팅 상황인지를
    알기 위해서 시간에 따른총손실값의 그림을봐야한다. 텐서보드에서는손실에 대해서
    tf. scalar_sumary를사용해서 얻을수 있다．

    아래는좋은 학습률 을 의미하는 시간에 따라손실값이 감소되는 경우를 보인다．




                α히
                 ＂   Ia         21n*     3. 1I      4a      l.fl     Ia     I』
                                                                             （1C    ta   .a    mm1




    파란선이 텐서보드그림이다．
                 붉은 선은손실의 추세선tendency line이다．

    오버슈팅은 아래와같이 나타난다．




                na        m〃》      1mO       13l0        ax노0      2텨）
                                                                     i)   ax10     刪.0   4n0   식刃끄   텨
                                                                                                     ＂끄




    오버슈팅이 발생하지 않게 충분히 작은 값이 되도록, 그리고 또한 반복 횟수를 줄여서
    더 빨리 학습을수행하도록충분히 크게 학습 률 을 조절해야한다．




CHAPTER 4 머신 러닝 기초


===== PAGE 149 =====
학습률 뿐만 아니라 기울기 하강 알고리즘에 영향을 끼치는다른 요인도 있다. 손실함수
에서의 지역 최적값locaL optima이다．                    아래의 그
                        손실 향수 그림의 쉬운 예로 돌아가보자．
림은초기 웨이트 값이 손실함수의 계곡valley의 오른편 근처에서 시작할때 알고리즘이
어떻게 동작할지를 나타낸다：




알고리즘은 그곳이 최적의 값이 아니라는 것을알방법이 없기 때문에 계곡을찾고 멈춘
다. 그곳에서의 기울기는 모든 지역 최적값에서 0이기 때문이다. 우리의 알고리즘은 전
역 최소값global minimum인지 지역 최소＜hocal minimum인지 구별할수 없다．
                                                   지역 최소값
은 해당하는근처에서 최적인값을 의미한다．

초기 웨이트 값을 랜덤값으로 함으로써 이런상황을극복하려고한다. 초기 웨이트 값은
수작업으로 정해진다는 점을 기억하자．

다음장에서 볼 예와같은딥 신경망문제에서, 이러한 지역 최적값은 아주 빈번히 일어
난다. 다행스럽게도많은 연구논문에서 이러한 지역 최적값들은손실 면에서는 전역 최
적값과유사하고 전역 최적값에 비해서 그렇게 많이 나쁘지 않다는 점이다．




                        기울기 하강법과 역전ㅍKGradient Descent and Backpropagation)   - 137


===== PAGE 150 =====
            이제까지 우리는미분값을 실제로 계산하지 않았다. 또 계산할 필요도 없었다. 텐서플로
            우는 지정한 그래프의 기울기를 계산해서 텐서로출력해주는 tf.gradients 메소드를
            제공한다. 사실은 심지어 기울기를 계산하는 이 메소드를 호출할 필요도 없다. 기울기
            하강 알고리즘 전체를 제공해주기 때문이다. 인공 지능 알고리즘의 세부 구현사항과수
            학에 깊이 들어가지 않는 이유가바로 여기에 있다．

            그렇기는 하지만 계산 그래프에서 기울기를 효율적으로 계산하기 위해서 사용되는 기
            법인 역전파backpropagation를간단하게 소개해보자．

            입력 레이어 1개, 출력 레이어 1개, 하나의 뉴런을 가진은닉 레이어 2개를 가진 아주 간
            단한 신경망을 생각해보자. 은닉 레이어와출력 레이어의 뉴런들은 시그모이드이고, 손
            실은 크로스 엔트로피를 이용해서 계산된다. 이런 네트워크는 아래와같을 것이다．




                                                          output


                                 LI             L2   13


            q을 첫 번째 은닉 레이어의 출력,L2를 두 번째 은닉 레이어의 출력,L3를출력 레이어의
            출력 값이라고 하자．


                     Li = sigmoid(w1·x)

                     L2 = sigmoid(w2·Li)

                     L3 = sig,noid(w3 ·L2)

            네트워크의 손실은아래와같이 기술할 수 있다．


                     loss   =   cross entropy



            기울기 하강법을 한스텝 실행하기 위해서, 손실 함수를 신경망의 3개의 웨이트에 대해



138 -   CHAPTER4 머신 러닝 기초


===== PAGE 151 =====
서 각각 편미분해야한다. 체인룰chain rule을 이용해서출력레이어 웨이트부터 시작한다．


     aloss
                   = cross_entropy'(L3,yexpected) ' sigmoid' (w3 ' L2) ' L2
      adP3

L2는 W3과는 상관없기 때문에 상수constant이다．위의 식을 간단히 하면다음과 같이 적
을수 있다．


         loss' = cross_entropy'(L3' Yexpecred)

         L3' = siginoid'(w3·L2)


편미분의 최종 결과는아래와같다．


         gloss          , .       .
                      = loss' ·L.5' · Lz
          aw3

이제 두 번째 은닉 레이어의 미분값을구해보자．


         L2' = sigmoid' (w2 ·Li)

         aloss           .   .     .     .    .
                      = loss' · Li ' · LZ' · LI
          aw2

WI에 대한 미분값은


         L1' = sigmoid'(w1·x)

         aloss           ,   .    -'. ' ,-.   ..
                      = loss' ·L.5' · Lz' · LI ' · x
             aw,
위의 계산에는 특정한 반복적인 패턴이 있다. 각 레이어의 미분값은 그 다음 레이어의




                                       기울기 하강법과 역전파
                                                  （Gradient Descent and Backpropagation)   1139


===== PAGE 152 =====
         미분값과그 전레이어의 출력값의 곱이다．

         입력 레이어에서 시작해서, 각은닉 레이어의출력 결과를 계산해서 출력 레이어까지 순
         차적으로forward 계산한다. 그다음에은 레이어를거쳐서 역방향backward으로미분값
         을 계산한다. 이렇게 함으로써 이미 계산된값을 재 사용함으로써 계산량을줄이기 위해
         서 그 결과를 전파한다propagate. 이러한 연유로 이름을 역전파backpropagation라고한다．

         시그모이드나 크로스 엔트로피 미분에 대한 정의는 아직 하지 않았다. 다른미분함수나
         손실값을쓰더라도 결과는같을 것이다．

         이 예제는 아주 간단하다. 그러나 동일한 알고리즘으로 미분값을 계산하는데 수천 개의
         웨이트를 가진 신경망인 경우에는학습 시간을 훨씬줄일수 있다．

         텐서플로우에는 몇 개의 다른 최적화 알고리즘들이 있는데, 모두 기울기를 계산하는방
         법을사용한다. 차이점은 입력 데이터의 모양과풀고자 하는문제에 따라서 성능의 차이
         가조금 있을수 있다．

         시그모이드은닉 레이어, 소프트맥스출력 레이어, 그리고 역전파기울기 하강법은다음
         장에서 보게 될보다복잡한모델을 위해 사용될 가장 기본적인 요소이다．




140ㅣ CHAPTER4 머신 러닝 기초


===== PAGE 153 =====
         ㅅ】Z=
         ㄹ 】：d




曳@   :      j。   *   4Ld
                     r   。   LIJ   O


===== PAGE 154 =====
            코드 구조와 유틸리티 함수들



            LAZY PROPERTY DECORATOR

             import functools


             def lazy_property(function):
                  attribute = "      + function,   name


                  @property
                  @functools .wraps(function)


                 def wrapper(self):
                       if not hasattr(self, attribute):
                             setattr(self, attribute, -Function(self))
                         return getattr(self, attribute)
                  return wrapper




            DOWNLOAD FUNCTION

             import shutil
              from urllib.request import urlopen


             def download(url, directory, filename=None):


                  Download a file and return its filename on the local file system.
              I-F the file is already there, it will not be downloaded again.
              The filename is derived from the url i-F not provided. Return the
             filepath.


                  if not filename:
                       -, filename = os.path.split(url)




142 -   CHAPTER 5 실습


===== PAGE 155 =====
         directory = os. path.expanduser(directory)
         ensure_directory(directory)
         filepath = os.path.join(directory, filename)


         if os.path.isfile(filepath):
             return filepath
         print( 'Download ' J 191epa꺄D
         with urlopen(url) as response, open(fllepath, ' wb') as flle_:
             shutil.copyflleobj(response, flle_)
         return filepath




DISK CACHING DECORATOR

데이터 사이언스와머신 러닝에서는，
                 학습 모델을 변경할 때마다매번전처리를다시 하
는 것을 원하지 않는 거대한 데이터셋을 사용한다. 그래서, 디스크에 데이터 처리의 중
간과정의 결과물을 저장하는 것이 좋다．

이 섹션에서는 캐싱caching과 로딩loading을 도와주는 데코레이터 함수decorator function
를 살펴보자. 데코레이터 함수의 반환값을 시리얼라이즈serialize 또는 디시리얼라이즈
deserialize하기 위해서 파이썬의 pickle 함수를사용하자. 그러나, 이 경우는 데이터셋
이 주기억장치에 로딩될 수 있을 때 가능하다. 더 큰 데이터셋을 위해서는 HDF5와같
은과학데이터셋 포맷을살펴보자．

이를 위해 먼저 필요한 세부 사항을 먼저 살펴보자. 파일을 저장하기 위해서 파일 시스
템에 디렉터리를 만들어야 한다．
                파이썬은 자동으로 만들어주지 않기 때문에，
                                      경로path
상에 디렉터리가 이미 존재하는 경우도잘다루어주는 아래의 함수를 사용하자．

 import errno
 impo吐 Os


 def ensure_directory(directory):




                                                          코드巧1조와유틸리티 함수들   - 143


===== PAGE 156 =====
                       Create the directories along the provided directory path that do
                   not exist.


                       directory = os.path.expanduser(directory)
                       try:
                           Os.makedirs(directory)
                       except OSError as e:
                           i-F e.errno !== errno.EEXIST:
                                raise e


                 @disk_cache 데코레이터를 작성하기 위해서 이 함수를 사용하자. 이것은 함수의 아규
                 먼트argument를 데코레이트 함수로 전달한다．
                                           함수 아규먼트는 이 아규먼트를 위한 캐
                 쉬된 결과가 있는지를 결정할 때도 사용된다. 이를 위해서 파일 이름에 연결된 하나의
                 숫자로 해쉬hash되어야 한다．


import functools
import Os
import pickle


def disk_cache(basename, directory, method=False):


     Function decorator for caching pickleable return values on disk. Uses a hash
computed from the function arguments for invalidation. If          ' method ' , skip the first
argument, usually being self or cls. The cache filepath is ' directory/basename-hash.
pickle' .


    directory = os. path. expanduser(directory)
    ensure_directory(directory)


    def wrapper(func) :
          @functools .wraps(Func)
            def wrapped(*args, **kwargs) :
                key = (tuple(args), tuple(kwargs.items()))




  144 -     CHAPTER 5 실습


===== PAGE 157 =====
            # Don't use seLf or cLS fOr the tnvaLLdation hash.
            if method and key:
                  key = key[l:]
            filename = '{}-{}.pickle'.format(basename, hash(key))
            filepath = os.path.join(directory, filename)
            if os.path.isfile(filepath):
                  with open(filepath, 'rb ') as handle:
                      return pickle.load(handle)
            result = func(*args, **kwargs)
            with open(filepath, 'wb') as handle:
                  pickle.dump(result, handle)
            return result
        return wrapped


    return wrapper


데이터를 처리하는 파이프라인을 저장하기 위한 디스크 캐쉬 데코레이터의 사용 예제

가 아래에 있다．


@disk_cache( ' dataset', '/home/user/dataset/')
def get_dataset(one_hot=True):
    dataset = Dataset( ' http://example.com/dataset.bz2')
    dataset = Tokenize(dataset)
    if one hot:
        dataset = OneHotEncoding(dataset)
    return dataset


method=False라는 아규먼트는 데코테이터에서 첫 번째 아규먼트를 무시할지 말지를

말해준다. 메소드나 클래스 메소드의 첫 번째 아규먼트는 수행되는 모든 프로그램들마

다 다른 객체의 인스턴스인 self이다. 그래서 사용 가능한 캐쉬가 있는지를 결정하지

못한다. 클래스 밖에 있는 스태틱static 메소드와 함수들에게는 이 아규먼트가 False여

야한다．




                                                            코드구조와유틸리티 함수들   - 145


===== PAGE 158 =====
            속성 사전
                （Attribute Dictionary)

            아래의 간단한 클래스는 컨패구레이션 객체configuration object를 사용할 때 편리

            하다．파이썬 딕셔너리dictionary에 컨피규레이션을 완벽하게 저장할 수는 있지만，
             config[ 'key' ］를통해서 각요소를접근하기는불편하다．

              class AttrDict(dict):


                  def _getattr_(self, key):
                       if key not in self:
                           raise AttributeError
                       return self[key]


                  def _setattr_ (self, key, value):
                       if key not in self:
                           raise AttributeError
                       self[key] = value


            빌트인buiLt-in dict에서 상속받은 이 클래스는 config. key와 ㄷon-Fig. key=value와같
            이 요소를 접근하거나 변경시킬 수 있다. 표준 딕셔너리에 키워드 아규먼트를 넘겨주거

            나**locals( ）를사용해서 속성 사전attribute dictionaㄸ를생성할수 있다．


              parmas = AttrDict({
                  'key' : value,
             })

              params = AttrDict(
                  key=value,
              )

              def get_paramsQ:
                  key = value
                  return AttrDict(**localsQ)




146 -   CHAPTER 5 실습


===== PAGE 159 =====
locals( ）는스코프scope 내의 모든 지역 변수 이름의 각각의 값으로의 매핑mapping을

반환한다. 파이썬에 익숙하지 않은 사람은 너무 복잡하다고 생각할 수 있다. 그렇지만
바로 전의 엔트리에 의존하는 컨I1 레이션 엔트리를 가지는 경우에는 이점이 있다．


 def get_paramsQ:
    learning_rate = 0.003
    optimizer = t-f.train.AdamOptimizer(learning_rate)
    return AttrDict(**localsQ)


이 함수는 learning_rate와optimize
                           「를 포함하는 속성 사전attribute dictionary을 반
환한다. 이것은 딕셔너리의 선언 내부에서는불가능하다. 자신에게 적합한방법을 찾가
야한다．



그래프 데코레이터 덮어 쓰기

이 함수 데코레이터는 텐서플로우를Jupyter notebook과같은 인터랙티브한방식으로
사용하는 경우에 유용하다. 일반적으로, 텐서플로우는 명시적으로 다른 것을 사용한다
고 말하지 않는 경우에는 디폴트 그래프를 사용한다．
                           그러나Jupyter notebook에서 인
터프리터의 상태는 모든 셀cet〔을 수행하는 중간 중간에 보관된다. 그래서 처음의 디폴
트그래프는 여전히 존재한다．


       勻upyter orc-sequence-abeIIingL.引C－幽L.:`sWmym12札PM{mm，
                                                           出.h－〕
        F4e       〔m         ·E시v    "`e【     Ce1     K아nt'1   H＇』4》

       目      *    1《   色      ．느   4'   .1   ㅒ   ■    mEr띠미              1   ce1lT.머ba
                                                                                      『
                                                      Res(a^
                                                      Re딧.n 8 이ear（〕
                                                                   ｀npu
                                                                      【
                                                      Re렸리1 & Run ^k
                              .cR $equenc             Re[Unnect

                              ￡沁出．
                                 t= hn口//騶 코uill이
                                                      q`a에e k日n叫

                  In F1] :    늬atptotUb tfll.iflfl

                              i1P.rt lmp.『tIib
                              i싸mrt fit 'llty
                              i. porttib. rnlo.d(&tiUty)

                              뇨Port flu떽1y ·1 np
                              1.port tnfl&orfto& ·～ tf
                              ㅓ '`r* 口．t..1..tlih ,..flt.,t 月4 ..lt




                                                                                          코드구조와유틸리티 함수들   - 147


===== PAGE 160 =====
            그래프 오퍼레이션을 정의하는 셀을 다시 수행하면 그것을 미리 존재하는 디폴트 그래
                                  텐서플로우는 이런 경우에 에러를 발생시킨
            프에 추가하려고 할 것이다. 다행스럽게도，
            다throw an error. 간단한 해결 방법은 커널을 재 시작하고 모든 셀을 다시 수행하는 것

            이다．

               더 좋은 방법이 있다. 커스텀 그래프custom graph를 만들고 그것을 디폴트로 선
            그러나，
            언하면 된다. 이렇게 하면 모든 오퍼레이션이 그 그래프에 추가되고, 셀을 다시 실행하
            면 새로운 그래프가 생성될 것이다. 그러면 예전의 그래프는 더 이상 참조하지 않기 때
            문에 자동으로 지워진다．


             def mainO:
                 # Define your PLacehoLders, modeL' etc.
                 data = t-F. placeholder(. . . )
                 target = t-1.placeholder(.. . . )
                 model = Model()


             with tf. Graph( ) . as_defaultO :
                 main()



                      아래와같이 데코레이터 안에서 그래프를 생성하고，
            더욱 편한방법으로는，                        그것과함께

            main 함수를 데코레이트하면 된다. 이 man' 함수는 플레이스홀더나 모델을 생성하기
            위한다른함수 전체 그래프를 정의해야한다．


             import functools
             import tensorfiow as t-F


             def overwrite_graph(function):
                 @functools .wraps(function)
                 def wrapper(*args, **kwargs) :
                       with tf. Graph() .as-default( ):
                           return function(*args, **kwargs)
                 return wrapper




148 -   CHAPTER 5 실습


===== PAGE 161 =====
이렇게 하면 위의 예제는 조금 쉬워진다．

@overwrite_graph
def mairiQ:
    # Define your βLacehoLders, modeLJ etc.
     data = tf. placeholder(. . .)
     target = tf. placeholder(. . .)
    model = Model()


main()




                                              코드구조와유틸리티 함수들   - 149


===== PAGE 162 =====
             물체 인식 및 분류
(Object Recognition and Classification)




     嶝   O     I   '   _   o   go   .
                                    J   * r% 。
                                          。      A   O


===== PAGE 163 =====
    텐서플로우의 기본을 이해하고 있고 실습도 해보았다. 이제 우리는 물체 인식과분류를
    위한모델을만들면서 이제까지의 실습 경험을활용할 것이다. 이 모델을만들면서 컴퓨
    터 비전computer vision의 새로운용어，
                              기법，
                                기본 원리들을 추가할 것이다. 이 모델을 학
    습시키는 기법은 정확도의 이점으로 인해서 최근에 유명해졌다．

   JmageNet은 레이블이 있는 이미지 데이터베이스로써, 컴퓨터 비전과 딥러닝이 최근에
    붐을 일으킨 대상이다．
               매년ImageNet의 데이터베이스에 있는 이미지들을분류하거나
    물체를 인식하는대회인 ILSVRC이 개최된다. 2012년에 Supervision이라는 팀은 새로
    운 신경망 구조를 이용한 해결책을 제출했다. ILSVRC의 제출 시스템들은 종종 창의적
    이었지만，
        SuperVision은 이미지 분류의 정확도에서 특출났다．
                                       SuperVision은 컴퓨터
    비전 정확도의 새로운표준을 정했고，
                      컨벌루션 신경망convolution neuraL network이라는딥
    러닝 기술의흥미를유발했다．

    컨벌루션 신경망Convolutional Neural Networks: CNNs은 점점 대중성을 얻었다. 처음에는 컴
    퓨터 비전관련된 일에 주로 사용되었지만, 이미지를 다루는 영역에만 국한되지는 않았
    다．
     CNN은그리드grid 상에서 연관된 값들이 순서대로나열된텐서로 표현되는 어떤데
    이터에도 사용될 수 있다. Microsoft Research는 2014년에 음성 인식을 위해서 CNN
    을사용하였는데, 입력 텐서는녹음된 순서대로 정렬된 소리로 구성된 1줄짜리 그리드
    였다. 이미지에 대해서는텐서의 값들은 이미지의 폭과높이에따른 그리드로 정렬된 픽
    셀이다．

    이 장는 텐서플로우에서 CNN과 이미지를 사용한다．
                               우리는 ImageNet 데이터베이스
    의 일부를 분류하는 CNN 모델을 텐서플로우를 이용해서 만들 것이다. CNN 모델을
    학습시키기 위해서는 텐서플로우에서 이미지를 사용할수 있어야 하고, CNN의 동작
    방식을 이해해야 한다. 이장의 대부분은텐서플로우를 이용한 컴퓨터 비전의 개념을 소
    개하는데 집중한다．

    CNN을 훈련시키는데 사용하는 데이터는Stanford's Dogs Dataset라고 이름이 붙은
    ImageNet의 이미지의 일부이다. 이름이 의미하듯이 이 데이터베이스는다양한종류의




CHAPTER 6 물체 인식 및 분류


===== PAGE 164 =====
개 이미지가품종에 따라서 레이블이 붙어있다. 모델의 목표는 이미지를 입력 벋아서 이
미지 안에 있는 개의 품종을 정확하게 추측하는 것이다．




                 7   n   1n ^   ㅕ ㅕ^ 쨍 口 ㄷ   체 4 口.   in ^   n ^ .   4ㅓ^ 쎄 . 「
                                         -'* 1(JqP닝                        . J *l「JJ'
                                                                                   . . ;- ∼
                                                                                       JP9



     Stanford's Dog Datbase에서 "Sberian Husky"라고 태깅된 예제 이미지



이 모델에 위의 이미지 중의 하나를 입력하면 ' 시베리안허스키' 레이블을출력해야한
다. 이 이미지들은학습과정에서 사용되었기 때문에 모델의 정확도 테스트를 위해서는
공정한 이미지는 아니다. 모델의 정확도 측정에 공정한 기준을 찾기 위해서 레이블링은
되어 있지만학습과정에 사용되지 않는많은 이미지가 필요하다. 이러한 이미지가 별도
의테스트 데이터셋으로 사용될 것이다．

모델의 정확도를 테스트하기 위한공정한 이미지 이야기를 하는 이유는 테스트, 학습，
크로스－밸리데이션cross-validation 데이터셋을 별도로 유지해야 하기 때문이다. 입력을
처리할때 신경망을학습하기 위해서 많은 비율의 데이터를 별도로괸리해야한다. 학습
에 사용했던 입력으로 모델을테스트하면 이미 보았던 입력은 정확하게 맞추는 모델을
생성하겠지만, 새로운 입력에는 잘 동작하지 않을 것이기 때문이다. 그때 테스트 데이
터셋을 사용함으로써 보지 않은 데이터에 대해서 모델이 얼마나 잘 작동하는지 확인할
수 있다. 여러 번반복 학습함으로써 테스트 데이터셋에 잘 적응하는 모델을 만들수 있
지만, 반면에 실제 응용에서는 잘동작하지 않을 수도 있다. ㅋ쿠ㅅ－밸리데이션 데이터
셋을사용하여 최종모델을 점검하고 정확도를조금 더 정확하게 측정하자. 이미지를사
용할때는 모든 데이터셋어］대해서 입력 절차를 유지하면서 전처리
                                 （색상 보정이나 영상
자르기）
   등은 해두면서 원래의 이미지를구분해두는 것이좋다．




                                                                                              1153


===== PAGE 165 =====
    컨볼루션 신경망
           （ConvoLutionaL NeuraL Networks)

    컨볼루션 신경망은 입력／와커널 g사이의 컨볼루션convolution 연산을수행해서 출력을
    생성하는 최소한 하나 이상의 레이어
                      （t-F. nfl. conv2d）
                                       를 포함하는 신경망을 의미한다．
    단순하게 말하면 컨볼루션의 목표는 필터링된 결과를 출력히끼 위해서 이미지의 모든
    픽셀에 커널
         （필터）
            을 적용하는 것이다．

    아래의 필터링된 결과물의 예는 이미지 내의 에지edge 검출이다．
                                       특별한 커널이 이미지
    의 모든 픽셀에 적용되어서 에지를 표시하는새로운 이미지가출력된다. 이 경우에, 입
    력 텐서는 이미지이고，
               텐서의 각 점이 red, green, blue 값을 지니는 픽셀이 된다．
                                                      커널
    이 이미지의 모든 픽셀에 대해서 미끄러지듯이 적용되면서 컬러들 사이에 에지가 있으
    면출력값이 커진다.



                                            -1 -1 -1
                                   g(t) =   -1 8  -1
                                            -1 -1 -1




                       (f* g)(t)




        입력이 이미지이고 출력이 이미지 내의 수펑선 에지인 간단한 컨볼루션 레이어 예




CHAPTER 6 물체 인식 및 분류


===== PAGE 166 =====
이 장의 후반부에서 실습하기 전까지는，컨볼루션이 어떻게 출력을 만들어내는지 또는
커널이 정확히 무엇을 말하는지 이해하는 것은 중요하지 않다. 큰 맥락에서 CNN이 무
엇인지 그리고 기술적인구현을 이룬생물학적인 영감을 이해하자．

1968년에 원숭이의 striate cortex
                         （줄무늬 피질, 시각적인 입력을 처리하는 것으로 알려
진 뇌의 부분）
       의 세포 구조에 대한 새로운 발견이 소개되었다. 수직으로 확장된 세포들
의 그룹이 특정한 시각적인특성을 보인다는 사실이었는데, 이러한 영장류의 뇌에 대한
연구는 머신 러닝과관련 없어 보일수 있지만, 이것이 CNN을 이용한 딥러닝의 개발의
단초가되었다．

CNN은 원숭이의 줄무늬 피질의 세포 구조와유사한구조로 정보를 연결하는단순화된
절차를 따른다. 신호가 원숭이의 줄무늬 피질을 거쳐갈 때, 어떤 레이어는 특정한 시각
적인 패턴이 표시될때 신호를낸다. 예를들어, 어떤세포 레이어는수평 선이 지나갈때
활성화된다
    （출력 신호가 커진다）
               .CNN이 학습을 통해서 획득된 패턴들에 기반해서 뉴
런들의 군집이 비슷한행동을보이는 것을확인할수 있을 것이다. 예를들어, 학습한후
에, CNN이 수평선이 지나갈때 특정 레이어가활성화되는 것처럼．

수평선을 확인하는 일은 유용한 신경망 구조이다. 그리고 cNN은 복잡한 패턴을 식별
하기 위해서 다수의 간단한 패턴들을 쌓음으로써 한단계 더 향상시켰다. CNN에서는
이러한패턴들을 필터filte
              「 또는 커널kerne
                         ［이라고 한다. 그리고 학습 데이터에 정확하게
매칭될 때까지 커널의 웨이트를조절하는 것이 목표이다. 이러한 필터들을학습시키는
것은여러 레이어를 결합하고 기울기 하강법으로 웨이트를학습함으로써 이루어진다．

단순한 CNN 구조는 컨볼루션 레이어
                   （t-F.nn.conv2d), 비선형non-linearity 레이어
(tf.nn.relu), 풀링pooling 레이어
                          （tf.nn.max_pool), 그리고 완전 연결fully connected
레이어
  （t-F.matmul）
             로 구성된다. 이러한 레이어가 없다면, 신경망이 너무 많은 정보
information로 채워질수 있어서 복잡한 패턴을매칭하기 어렵다. 잘 설계된 CNN 구조는
노이즈는무시하면서 중요한 정보를 부각한다. 우리는다음 장에서 이러한 여러 레이어
들이작동하는방식을자세히 살펴볼 것이다．




                                        컨볼루션 신경망
                                               （Convolutional Neural Networks)   - 155


===== PAGE 167 =====
                                                                                                   batchl
                                                                                 fimage_
                                                                                               I
                                     jnlage            IUP叫
                                              a-
                                                              -




                   Convolutional
                                                                  La er]  y     [tf.nn.conv2d
                                                   I                                 I
             [Re                   ctified Linear                  Unit
                                                                                           tf.nn.relu
                                                   1                                 I
                                    Pooling Laye"                               玗nn.rnax.poo기
                                                   I               -      )          I_
             Fully Connected Layer                                            kf.matmul(x, W)＋이

    이 구조에서는 배치batch 이미지를 입력받기 위해서 입력 이미지의 구조가 조금 복잡
    해진다．
       여러 이미지를 로딩
                ［oading한다는 것은 다수의 이미지를동시에 계산할수 있다
    는 의미이다. 이를 위해서는 조금 더 복잡한 자료 구조가 필요하다. 이를 위해서 사용되
    는자료 구조는배치 이미지를 컨볼브convotve하기 위해 필요한모든 정보를 포함하는 랭
    크「ank 4의 텐서이다. 텐서플로우의 입력 파이프라인
                                 （파일을 읽고 해석하기 위해 사용
    되는）
      은이미지에 대한필요한정보
                  （[image_batch_size, image_hei帥t, image_
    width, image_channels]）를포함해서 배치로동작하기 위한특별한형식을지닌다．
    예제코드에서, 텐서플로우에서 이미지를 사용하면서 사용되는 입력의 구조를살펴볼

    수 있다．

     image_batch = t-f.constant([
             [ # First Image
                                   [[0, 255, 0], [0, 255, 0], [0, 255, 0]],
                                   [[0, 255, 0], [0, 255, 0], [0, 255, 0]]
             L
             [ # Second Image
                                   [[0, 0, 255], [0, 0, 255], [0, 0, 255]],
                                   [[0, 0, 255], [0, 0, 255]』 [0, 0, 255]]




CHAPTER 6 물체 인식 및 분류


===== PAGE 168 =====
           I
     1)
image_batch.get_shape()


예제 코드의 출력은다음과같다．


TensorShape([Dimension(씬), Dimension( ), Dimension( ),Dimension(3)])

                  391익【"「"l甲        }    y   二）             D{""_
각주     이 예제 코드를 포함한향후의 예제들은텐서플로우코드를 실행하기 위한 일반적인코
       드는포함하지 않았다. 예를들어, 텐서플로우임포트，
                                 텐서플로우세션생성, 변수의 초
          기화，
            스레드 러너
                 （仕Lread runner) 시작등은 표시하지 않았다. 이러한과정 없이 실행
       하면Undefined variable error 같은메시지가출력될수도 있다．

예제 코드에서, 두 개의 이미지를포함하는 배치 이미지가생성된다. 각 이미지는RGB

색상값을 가지는 높이 2픽셀, 폭 3픽셀이다. 예제 코드는 이미지의 양을 첫 번째 차원
Dimension(2), 각이미지의 높이를두 번째 차원 Dimension(2), 각 이미지의 너비를
                                                으로 출력
세 번째 차원 Dimension(3), 컬러 채널의 크기를 마지막 Dimension(3）

한다．

각 픽셀이 이미지의 높이와폭에 해당한다는 점이 중요하다. 첫 번째 이미지의 첫 번째
픽셀의 색상은아래와같이 접근 가능하다．

 sess . run(image_batch)[0][0J[0]


예제 코드의 출력은아래와같다．


 array([ 0, 255, 0], dtype=1nt32)


디스크에서 이미지를 로딩하는 대신, image_batch 변수가 입력 파이프라인의 부분으
로 로드된 이미지처럼 동작한다. 입력 파이프라인을 사용해서 디스크에서 로드된 이미
지도 같은 형식을 가지고 동일하게 동작한다. CNN의 입력과 출력을 테스트하기 위해
                                            단순화된
서, 위의 image-batch 예제와유사한 가상의 데이터를 만드는 것이 편하다．



                                         컨볼루션 신경망
                                                （Convolutional Neural Networks)   - 1 57


===== PAGE 169 =====
    입력은 디버깅이 쉽도록 해준다. cNN은 굉장히 복잡하고 학습에 여러 날이 필요할 수
    있기 때문에, 디버깅 과정을단순하게 하는 것이 중요하다．

    CNN을 사용할 때 첫 번째 복잡한 것은 컨볼루션 레이어의 동작방식을 이해하는 것이
    다. 이미지 로딩과조작후에, 보통 컨볼루션 레이어가 신경망의 첫 번째 레이어가 되는
    데, 첫 번째 컨볼루션레이어는 신경망의 이후의 작업을 간단하게 할수 있고，
                                            디버깅에
    사용되기 때문에 중요하다. 다음 섹션에서는 컨볼루션 레이어의 작동 방식과 텐서플로
    우의 사용법에 집중한다．




    컨볼루션
       （ConvoLution)

    컨볼루션 연산은 이름이 의미하듯이 컨볼루션 신경망의 중요한부분이다. CNN이다양
    한 패턴에 정확히 매칭할수 있는 능력은 컨볼루션 연산 덕분이다. 이런 연산들은 이전
    섹션에서 봤던 것처럼 복잡한 입력을 필요로한다. 이 섹션에서 우리는 컨볼루션 연산과
    파라미터 튜닝 관련 실험을 해보자．




          두 개의 입력 텐서(input과 kernel）
                                  를 컨볼브해서 각 입력으로부터의 정보
          를 표현하는 하나의 출력 텐서를 생성하는 컨볼루션 연산




CHAPTER 6 물체 인식 및 분류


===== PAGE 170 =====
입력과 커널0nput and Kernel)

일반적인 상황쩨서 텐서플로우의 컨벌루션 오퍼레이션은 tf.nn. conv2d를 사용한다．
텐서플로우에는 특별한 용도로 사용할 수 있는 다른 컨벌루션 오퍼레이션들도 있지만，
tf.nn.conv2d는 처음 실험할 때 많이 사용되는 컨벌루션 오퍼레이션이다. 예를들어
두 개의 텐서를 서로 컨볼빙convolving하는 실험을할수 있다．

 input_batch = t-1. constant([

                       炒 First Inpu
                   (    /




            「
             「L
                   K                    4; ,;
                                                긱꺅q    中楙4叫 어3ㅅ
                                                                                         繃N
                                                                                 CU&'U쿄ㅆt；        '




                                                 甘n；忠
                                                      n ,       ㄱ
   少，
    돋，
    돈d Iipij
                                                            ,
                                                            '       ㄴ   C0   ,   0〕
                                                「；
 ('     L4.ejj,    ,L.L.' 'r:"
 ""'\   '          LtD.     "j,   [8.    ejj
                  ])

 kernel = tf. constant([
                       [

                       ]
                  ])

이 예제 코드는 두 개의 텐서를 생성한다. input_batch 텐서는 이전 섹션에서 사용했
던 image_batch 텐서와 비슷한 모양이다. 이것이 컨벌루션되는 첫 번째 텐서이고, 두
번째 텐서는 kernel이다．
               kernel은weights,filter, convolz成on matrix, mask라고도불리
는 중요한단어이다．
         이 단어들 중에서，
                  지금은 컴퓨터 비전과 관련된작업이기 때문에，
image kernel처럼 kernel이라는 단어를사용하는 것이 좋을 것 같다．
                                           텐서플로우에는
기능상 위의 용어들 사이의 차이점은 없다. 이것을 텐서플로우에서 파라미터에서는 필
터filter라고 불리며，
             학습을 통해서 얻게 되는 웨이트의 집합이다. 커널
                                       （필터 파라미터）
에 포함된다양한 웨이트들이 학습될 커널을 의미한다．




                                                                                      컨볼루션
                                                                                         （Convolution)   - 159


===== PAGE 171 =====
                이 예제 코드에서, kernel 변수의 첫 번째 차원인 하나의 커널이 있다. 커널은 하나의
                채널은 원래의 입력을 가지고，
                               다른 채널은 입력값의 2배를 가지는 텐서를 반환하기 위
                해 사용된다．
                      여기서 채널channe
                                 ［은 랭크rank 1 텐서
                                              （벡터）
                                                 를 표현하기 위해서 사용된다．
                채널은 컴퓨터 비전에서 출력 벡터를 표현하기 위해서 사용되는 용어인데, 예를들어
                RGB 이미지는하나의 랭크 1 텐서 [red, green, blue〕
                                                     로써 표현되는3개의 채널을
                가지고 있다. 나중에 소개될 stride＄와 padding 파라미터는 지금은 고려하지 말고 컨
              볼루션
                （tf.nn.con2d) 출력에만 집중하자．


conv2d = tf. nn.conv2d(input-batch, kernel, strides=[1, 1, 1,1], padding= 'SAME')


sess. run(conv2d)



              이 예제 코드의출력은 아래와같다：


               array([[40. , 0.},
                   [ 1., 2.]],
                    [[ 2., 4.],
                    〔 3., 6.]]],
                    [[[ 2., 4.],
                    [ 4., 8.]],
                    [[ 6., 12.],
                    [ 8., 16.]]]], dtype=fl0at32)


              출력은 1먀)ut_batch와동일한 랭크인 또 다른 텐서인데, 커널의 차원과 동일하다．
              input_batd，
                        가 하나의 이미지라고 생각해보자. 그렇다면 그 이미지는 하나의 채널
              일 수 있다．
                    이러한 경우에는 그레이 스케일grayscale 이미지인 경우이대
                                                      （Working with
              Co'ors 참고）
                       . 텐서의 각요소가 이미지의 하나의 픽셀이며, 오른쪽 아래의 픽셀의 색상
              값은3.0일 것이다．

              tF.nfl. conv2d 컨벌루션 오퍼레이션을 이미지input_batch와kernel 텐서와의 결합이라
              고 생각해보자．
                     이 두 개의 텐서의 컨벌루션은 피처맵feature map을 생성한다．피처맵은




 160 -   CHAPTER6 물체 인식 및 분류


===== PAGE 172 =====
컴퓨터 비전에서 이미지 커널을 사용한오퍼레이션의 출력 결과와관련된 일반적인용
어인데, 여기서의 피처맵은출력 결과에 새로운 레이어를 더함으로써 이런 텐서들사이
의 컨벌루션을 의미한다．

입력 이미지와출력 피처맵 사이의 관계를코드로살펴보자. 입력 배치와피처맵의 요소
들을 접근하는 것은 동일한 인덱스로 이루어진다. 입력과 피처맵의 같은 픽셀을 접근함
으로써, 입력이 kernel과 컨볼브되면 어떻게 변하는지를 보여준다. 아래의 경우에 이
미지의 우측 하단의 픽셀이 3.0*1.0과 3.0*2.0을 곱한 값을 출력한다. 이 값들은 픽셀값
과 kernel에 있는 픽셀값에 해당하는 값이다．

lower_right_image_pixel = sess.run(input_batch)[0][l][1]
lower_right_kernel_pixel = sess.run(conv2d)[0][l][l}
lower_right_image_pixel, lower_right_kernel_pixel


예제 코드의출력은아래와같다．

 (arrav(1 3.1. dtvoe=float32). arrav(1 3 .   1. dtvoe=f1oat32n

        ＼의              Z
이 간단한 예제에서，
          이미지의 각 픽셀은 커널의 연관된 값으로 곱해진 후，
                                      피처맵의 연
관된 레이어에 더해진다．
            여기서 레이어Laye는출력에서의 새로운차원을 의미한다. 이
예제에서는 컨볼루션 연산에서 그 값을보기는 쉽지 않다．



스트라이드
    （Strides, 큰 걸음 걷기）

컴퓨터 비전에서 컨볼루션의 중요성은 입력
                     （이 경우에는 이미지）
                                의 차원을줄이는능력
에 있다. 2차원 이미지의 차원은 이미지의 폭, 높이, 채널의 개수와관련 있다. 이미지의
차원이 커지면 그에 따라 신경망이 모든 픽셀을 처리하고 어느 픽셀이 중요한지 판단하
는데 기하급수적으로 많은 시간이 필요하다. 컨볼루션으로 이미지의 차원을 줄이는 것
은 커널의 스트라이드＄tride를 변경함으로써 가능하다．




                                                                 컨볼루션
                                                                    （Convolution)   - 161


===== PAGE 173 =====
                                                       모든
              츤ㅌ라이드 파라미터는 이미지의 픽셀들을 건너뛰고 출력에 포함되지 않게 한다．
               픽셀들이 출력에 영향을 미칠수 있기 때문에 픽셀들을 건너뛴다는 것은합당해 보이지
              않는다. 스트라이드파라미터는큰이미지와복잡한커널을사용하는경우에, 컨볼루션
               연산이 커널에 의해서 수행되는방법을더욱뚜렷하게 보인다. 컨볼루션이 입력 위를 커
              널을움직일 때, 입력 위를움직이는방법을바꿀 때 스트라이드파라미터를사용한다．
               입력의 모든요소를살펴보는 대신, 스트라이드 파라미터는 어떤 요소는 건너뛰도록 할
              수 있다.

              조금 더 큰 이미지와 커널을 컨볼루션에 사용하는 경우를 보자. 아래는 높이, 폭, 채널의
               개수가6x6x1인이미지와3x3x1크기의 커널 사이의 컨볼루션이다．


input_batch = t-F.constant
         [ # /=tr5t 工nput
             [[0.0], [1.0], [2.0], [3.0], [4.0], [5.0]],
             [[0.1], [1.1], [2.1], [3.1], [4.1], [5.1]],
             [[0.2], [L2], [212], [3.2], [4.2], [5.2]],
             [[0.3], [1.3], [2.3], [3: ]-; [4.3], ts.3]1,
             [[0.4], [1.4], [2.4], [3.4], [4.4], [5.4]],
             [[gj] , [1.5], [2.5], [3.5], [4.5], [5.5]],
                              →   一   -




kernel = t-F.constant([ # KerneL
             [[t0.(=}]], [[0.-5]], [[ ;bfl],
             [[[0.0]], [[1.0]], [[0.0]]],
             [[[0.0]], [[0.5]], [[0.0]]]
    1)


#NOTE: =.
conv20    tt.nn.
         the change     the 보' " of the '                                  乙二，
                .c0nv20
                      ( lnput- batch, kernel, str1des= 1, 3, 3,1j, paddiflg=e竺)
                     !"   .                可ides   parameter.   '   -   .   .   .   .
                                                                                    .
sess. runiconvLu)




 16기     CHAPTER 6 물체 인식 및 분류


===== PAGE 174 =====
예제 코드의출력은 아래와같다：


      ［山 2. 20000005],
 array(
    [ 8.19999981]],
                                  (＝諦 ×2 xI죠
    [[ 2.79999995],
    [ 8. 80000019]]]], dtype=fl0at32)


kernel을 input_batch 위에서 일정한요소들을 건너뛰며
                                   （striding, skipping) 움직
이면서 input_batch가 kernel과 결합한다. kernel이 움직일 때 마다 input_batch
의 한요소에 중심을 맞춘다. 겹쳐진 값들을 곱해서 모두 더한 결과가출력 결과이다. 아

래 그림은 '항목간의 곱셈point-wise multiplication' 이라고 하는두 값들사이의 컨볼루션결
합방법을보인다．




                          b刀그璜궁           ／蠟卄舞
                              1
                              n 44444 4
                t 2222 22
                叩刀그2345                          －츤rn이 g
                              沈刀그八굽345
                n l llll 1                       100.501
                I 0l234 5                        j0 1 0j
                              a 33 。333
                                                 L 0 0.5 0 」
                  o0 000 1




           (fo* go+ .·.+fn* g)
       (0.0 * 0+ 1.0 * 0.5 +2.0 *0,                          output
       ㅣ 0.1* 0+ 1.1* 1+ 2.1* 0 1                      싸2.     2 8.2
                                                             2.8 8.
        \0.2* 0+ 1.2* 0.5+ 2.2* 0J                                8]
ㅇ．]그림에서，
       코드에서 보았던 것과 같은 로직이 수행된다．
                              두 개의 텐서가 입력 위를 건
                      스트라이드는출력의 차원을 줄이고，
너뛰면서striding 함께 컨볼루션된다．                커널은 모든

입력값을 사용해서 컨볼루션할수 있도록 해준다. 스트라이딩 때문에 입력값중어떤 것
도완전히 제거되지는않으며, 이제 입력은더 작은텐서인셈이 된다．




                                                                       컨볼루션
                                                                          （Convolution)   - 163


===== PAGE 175 =====
    스트라이딩은 입력 데이터의 차원을 조절하는방식이다. 차원을 줄이면 연산량이 줄어
    들고 완전히 겹쳐지는 receptive field가 발생하는 것을 막아준다．
                                             스트라이드 파라미
    터는 입력 텐서와동일한형식이다 [image_batch_size_stride, image_hei帥t-
    stride, image_width_stride, image_channel_stride]. 스트라이드파라미터의
    첫 번째 요소와마지막요소는 거의 변경하지 않는다. 변경한다는말은tf.nn.conv2d
    연산에서 데이터를 건너 뛰어서 아예 고려하지 않는다는 말이기 때문이다. i mage_
   ,hei帥t_stride와image_width_stride는 입력의 차원을줄이는데 유용하다．

    스트라이딩에서 입력의 가장자리에서 문제점이 있다. 이미지와 커널의 크기가맞지 않
    는 경우인데，
          이미지 크기，
                커널 크기，
                     스트라이드가 변경될 수 없다면，
                                     패딩padding을 해
    서맞출수 있다．



    패딩
     （Padding)

    커널이 이미지에 겹쳐질 때 이미지의 경계 안에서 이루어져야한다. 경우에 따라서 크
    기가맞지 않아서 이미지에 모자라는부분을 채워야하는 경우가 있다．
                                      이를 패딩padding
    이라고한다. 텐서플로우는 이미지를0으로 패딩하거나, 커널이 이미지의 경계를 넘어
    서지 않고서는 스트라이드할 수 없는 경우는 에러를 발생시킨다. 0의 개수나 tf. nn.
    conv2d의 에러 메시지는padding 파라미터
                              （'VALID' 또는 ' SAME' 값을 가진다）
                                                        에
    의해서 조절된다．

      , SAME: 컨볼루션 출력은 입력과 SAME 크기이다．
                                    이미지 위에서 스트라이드할때 필
    터의 크기를 고려하지 않는다. 경계를 넘어서 없는 값들을 0으로 패딩하는 경우에는 이
    미지의 경계를넘어서서 스트라이딩할수도 있다．

      VAUD: 이미지를 스트라이드할 때 필터의 크기를 고려한다. 이 방법은 커널을 가능
    한이미지의 경계 내부에 두려고 노력할 것이다．


    입력의 크기를 고려하는 것이 가장 좋다. 그러나 패딩이 필요하다면 텐서플로우는 내
    장된 옵션이 있다. 가장 간단한 시나리오로 SAME이 좋은 선택이다. VALID는 입력



CHAPTER 6 물체 인식 및 분류


===== PAGE 176 =====
과 커널이 스트라이드와 잘 작동한다면 사용하는 것도 좋다. 더 많은 정보를 위해서

convolution documentation을참고하자．

                                                i1,4 報빈t   스）   6\   ev
                                                                      'CU-   LM 7    뙤
데이터 형식

tf. nn. conv2d에는 아직 설명하지 않는 data_-Format 파라미터가 있다. tf.nn.conv2d

설명서는 입력, 커널, 스트라이드가 이제까지 사용하던 형식과 다른 형식을 사용할

수 있도록 데이터 형식을 변경하는 방법을 설명한다. 입력 텐서가 [batch size,
height, width, channel〕표준형식과다른경우에유용한데, 입력을수정하는대신

     -Format 파라미터를 변경하면 된다．
data-

   데이터형식：" NHWc ', "NCHW'에서 선택해서사용할수있다. "l얀Iwc" 가디폴트이다.
   입력과출력 데이터의 형식을지정해야한다．
                       디폴트 형식인 "NHWC"은데이터가 [batch,
   in_height, in_width, in_channels] 순서로저장된다．
                                            "NCHW'' 형식은데이터가［batch,
   in_channels, in_hei함1t, in_width]순서로 저장된다．

   데이터 형식             정의
      N               배치의 텐서의 개수, batch_size
      H               각 배치의 텐서의 높이
      w               각 배치의 텐서의 너비
      C               각 배치의 텐서의 채널




KERNELS IN DEPTH

텐서플로우에서 필터 파라미터는 입력에 컨볼루션되는 커널을 명시하기 위해서 사용된

다. 필터는 카메리'의 렌즈에 도달하는 빛의 양과 같이 사진의 특성들을 조절하기 위해

사용되는용어인데, 사진에서 필터는사진사가사진에 아주극명한 변화를줄때 사용된

다．
 사진사가 필터를 이용해서 그림을 수정할 수 있는 이유는, 필터가 렌즈에 도달하는

빛의 속정을 인지할수 있기 때문이다. 예를들어, 빨강 렌즈 필터는빨간색만 필터를통

과시키고 그 이외의 색은 흡수
               （차단）
                  한다．



                                                            컨볼루션
                                                               （Convolution)        - 165


===== PAGE 177 =====
                 Before and after applying a minor red fi lter to n02088466_3184.jpg




          컴퓨터 비전에서 커널
                    （필터）
                       은 디지털 이미지의 중요한속성을 인지하기 위해서 사용된
          다. 이미지에 어떤특징값들이 존재할때 이를부각시키기 위해서 특정한 패턴을사용함
          으로써 이루어지는데, 빨강 필터 예제를흉내내는 커널은빨간색 이외의 색상값들을 감
          소시킴으로써 구현된다. 이 예제에서 빨간색은 그대로 유지되지만다른 색상들은 감소
          된다．

          이 장의 시작 부분의 예제는 에지 검출을 위한 커널을 사용하였다. 에지 검출 커널은 컴
          퓨터 비전 응용에서는 일반적으로 사용되며, 기본적인 텐서플로우 오퍼레이션과 하나
          의 t-f.nn.conv2d 오퍼레이션으로구현될수 있다．

           kernel = tf. constant({

                   II
                        [[ -1. , 0., 0.], [ 0., -1.., 0.], [ 0., 0., -1.]],
                        [[ -1. , 0., 0.], [ 0., -1., 0.], [ 0., 0., -1.]],
                        [[ -1., 0., 0.], [ 0., -1. , 0.], [ 0., 0., -1.]]
                   ],
                   [
                        [[ *1. J 0. J 0. ]J [ 0. J -1. J 0. ]J〔 0. J 0., -' n,
                        [[ 8., 0., 0.], [ 0., 8., 0.], [ 0., 0., 8.]],
                        [[ -1. , 0., 0.], [ 0., -1. , 0.], [ 0., 0., -1.]]




                        [[ -1. , 0., 0.], [ 0., -1., 0.], [ 0., 0., -1.]],




16히   CHAPTER 6 물체 인식 및 분류


===== PAGE 178 =====
            [II -1., 0., 0.], [ 0., -1., 0.1, [ 0., 0., -1.]],
           [[ -1., 0., 0.], [ 0., -1., 0.], [ 0., 0., -1.]]




conv2d = t-f.nn.conv2d(image-batch, kernel, [1, 1, 1, 1], padding="SAME")
activation_map = sess.run(tf.minimum(tf.nn.relu(conv2d), 255))




              0
            50
           100
           150
           200
           250
           300
           350
               0      100    200     300    400     500



위의 이미지는 이미지와 에지 검출 커널과의 컨볼루션 결과 이미지이다. 이 코드는 디
스크에서 로딩된 배치 이미지가 있다는 것을 가정한다
                           （image_batdD. 이 예제에서
의 이미지는 Stanford Dogs Dataset의 예제 이미지이다．커널은 3개의 입력과 3개
의 출력 채널이 있다．
           채널들은 RGB 값이 0에서 255
                             （가장 밝은값）
                                    까지의 값을 가진다．
tf.minimum과tf.nn.relu는 컨볼루션 값이 0에서 255사이의 RGB값의 범위를 유지
하기 위해서 사용된다．

이 예제에서 사용할수 있는 여러 커널들이 있다. 각 커널은 이미지의 다른 패턴들을 강
조하는데, 아래의 커널은 색상 변화의 정도를 증가시킴으로써 이미지를 더욱 선명하게
한다．



                                                             컨볼루션
                                                                （Convolution)   - 167


===== PAGE 179 =====
kernel = t-F.constant([

         [
             〔〔 0. J 0. J 0. ]J [ 0. J 0. J 0. ]J [ 0. J 0. J 0. ]]}
             {[ -1. , 0., 0.], [ 0., -1., 0.], [ 0., 0., -1.]],
             [[ 0. J 0. J 0. ]J [ 0. J 0., 0. ]J [ 0. J 0. J 0. ]]




             [[ -1. , 0., 0.), [ 0., -1., 0.], [ 0., 0., -1.]],
             [[ 5. J 0., 0.]J [ 0. J 5. J 0. ]J [ 0. J 0. J 5. ]],
             [[ -1. , 0., 0.], [ 0., -1., 0.], [ 0., 0., -1.]]




             [ [ 0. J 0. J 0. 〕J [ 0. J 0. J 0. ]J [ 0. J 0. J 0. ]]J
             [ [ -1.' 0., 0. L   [ 0., -l. J 0. ]J [ 0., 0., -l. ]]J
             [ [ 0J 0. J 0. ]J [ 0. J 0. J 0. ]J [ 0. J 0. J 0. ］〕




conv2d = t-F.nn.conv2d(image_batch, kernel, [1, 1, 1, 1], padding="SANE")
activation_map = sess.run(tf. minimum(tf. nn.relu(conv2d), 255))




                                  0
                                 50
                               100
                              150
                               200
                               250
                               300
                               350
                                      0    100      200      300        400   500




 168 -   CHAPTER 6 물체 인식 및 분류


===== PAGE 180 =====
앞의 커널은, 커널의 중심은 밝기를증가시키j긱 커널 둘레의 값은밝기를줄인다. 이 커
널은 시각적으로 선명해지는 이미지를 출력하게 된다. 커널 구석의 값은 0이어서 덧셈
기호 모양의 패턴으로작동하는출력은 영향을미치지 않는다．

이러한 커널들은 기초적인 레벨에서 이미지의 패턴과 일치된다. 컨볼루션 신경망은 학
습 을 통해서 배운 복잡한 커널을 사용해서 에지뿐만 아니다 다른 것들과매칭될수 있
는데, 커널의 초기값은 랜덤값에서 시작해서 CNN의 학습 과정 동안에 최적화된다．
CNN이 완성되면, 각 이미지가 컨볼루션되고, 예측값이 이미지의 레이블과 일치하는
지 여부에 따라서 값들이 수정된다．
                  예를 들어，
                       Sheepdog 그림이 학습된 CNN에 의
해서 Pit Bull로 인식된다면，Sheepdog 그림을 더 잘 인식할 수 있도록 필터값을 조
금수정한다．

CNN으로 복잡한 패턴을 학습하려면 하나 이상의 컨볼루션 레이어가 필요하다. 예제
코드도출력을 시각화하기 위해서 tf.nn.relu 레이어를 사용한다. 컨볼루션 레이어는
CNN에서 보통 한 번 이상사용되며, 다른 형태의 레이어도 포함할수 있다. 이러한 레
이어들은 성공적인 CNN 구조를 위해서 결합된다．




Common Layers

CNN 신경망은 최소한 하나의 컨볼루션 레이어
                        （tf.nn.conv2d）
                                     가 있어야 한다. 에지
검출을 위해서 싱글 레이어 CNN이 주로 사용되고，
                           이미지 인식image recognition이나분
류categorization를 위해서는 다양한 형태의 컨볼루션 레이어를 사용한다. 이 레이어들은
오버 피팅over-fitting
               （과적합）
                   을줄이고，
                       학습속도를빨리하며, 메모리 사용을줄인다．

이 장에서 소개되는 레이어들은 CNN 구조에서 자주 사용되는 레이어에 집중했다．
CNN이 이러한레이어만사용할수 있는것은아니며, 다른신경망구조를위해서 이러
한레이어를 섞어서 사용할수도 있다．




                                                Common Layers   1 169


===== PAGE 181 =====
    컨볼루션 레이어

    컨볼루션레이어의한종류인tf.nn. conv2d는자세하게살펴보았는데, 이외에도고급
    사용자를 위한 몇 가지 자세한 설명이 남았다. 텐서플로우의 컨볼루션 레이어는 완전한
    컨볼루션을수행하지 않는다
                （자세한 내용은 텐서플로우 API 설명을 참고하자）
                                           . 실제의
    컨볼루션과텐서플로우에서 사용하는오퍼레이션의 차이는 성능이다. 텐서플로우는다
    양한 형태의 컨볼루션 레이어에서 사용하는 컨볼루션 오퍼레이션의 속도를 향상 시킬
    수 있는 기법을사용하기 때문이다．

    각 컨볼루션 레이어의 사용 예제들이 있지만 t-F. nn. conv2d가 시작하기에 편하다. 다
    른종류의 컨볼루션도유용하기는하지만, 물체 인식과분류를 위해서는 필요하지 않다．
    각각에 대한간단한요약을 샬펴보자．


    TF.NN.DEPTHWISE CONV2D

    컫볼루션의 출력을 다른 컨볼루션의 입력으로 연결할 때 사용된다．고급 사용자는
    inception architecture를 따르는 신경망을 구성할 때 tf. nn.depthwise_conv2d를
    사용할수 있다．

    이 컨볼루션은tf.nn.con2d와유사하지만동일하지는 않은데, 큰 모델인 경우에는 정
    확도를 줄이지 않고 학습 속도를 올릴 수 있다. 작은 모델인 경우에는 정확도는 떨어지
    지만빨리 수렴한다．
                                               1 ,1,,, ,, ,낢 門，.0 1\   의 34얘
                                ...      d),^\/D`｀欠，
                                                   `U一’ V ' ㅣ        U
    ㄱ－「 ㄴ1`. ^^`" ',,1, -,^`U一∼，
    TF.NN.CONV2D        TRANSPOSE     /) ㄴ〃" '               "

    각 영역이 커널과 같은 값으로 채워진 피천맵에 커널을 적용한다．커널이 새로운 이미
    지 위를 스트라이드할 때 겹쳐지는 영역은 함께 합해진다. Stanford's CS231n Winter
    2016: Lecture 13에 tf. nn. conv2d_transpose에 대한자세한 설명이 있다．




CHAPTER 6 물체 인식 및 분류


===== PAGE 182 =====
     （activation functions)
활성화 함수

활성화함수는다른레이어의 결과와 결합되어서 피처맵을만들때사용된다. 이들은특
정한오퍼레이션의 결과를 평탄화＄mooth 또는 미분differentiate하기 위해서 사용된다. 활
성화 함수의 목적은 신경망에 비 선형성non-linearity을 부여하기 위해서인데，
                                              비 선형성
이란 입력이 직선이 아닌 곡선이라는 의미이다. 곡선은 입력에서 더 복잡한 변화를 표
현할수 있다는 것을 의미한다. 예를들어, 비 선형 입력이란 대부분의 시간에는작은 값
이면서, 주기적으로극단적인 값을가지는경우를표현할수 있음을의미한다. 신경망에
비 선형성을추가함으로써, 데이터의복잡한패턴을학습시킬수 있게 된다．

텐서플로우는 여러 가지의 활성화함수가 있다. CNN에는 정보 손실이 조금 있지만 성
                             처음 시작할때는tf.nn. relu를추
능이 좋기 때문에 %f.nn.relu가주로 사용되는데，
천한다. 고급 사용자는 자신의 활성화 함수를만들 수도 있다. 활성화함수 선택에는다
음을고려하자．

  1. 함수가단조 증가monotonic인 경우：출력이 입력에 따라서 증가되거나감소된다．
     기울기 하강법은 지역 최적값에 다다를수 있다．
  2. 함수가미분 가능differentiable한경우：함수의 정의 구역의 모든값에 대해서 미분
     값derivatives이 있다. 기울기 하강 최적화방법이 적절하게 작동할수 있다．


이러한 조건을만족하는 어떠한 함수도 활성화함수로 사용될 수 있다. 텐서플로우에서
CNN에서 자주 사용되는 것을 살펴보자. 각각의 간단한 설명은사용 예제와 함께 샘플
코드가포함되어 있다．


TF.NN.RELU

램프 함수                                                      는 그림으로 그
    「amp function라고불리는rectifier(rectified linear unit: ReLU）
리면 스케이트 보드의 램프와 비슷하다. ReLU는 선형이며, 응수값은 0으로 만들고 모
든 양수값은동일한값을유지한다．
               기울기 소멸gradient vanishing의 문제가 없고 [0, +삐




                                                            Common Layers 1171


===== PAGE 183 =====
    까지의 값을 가진다는 장점이 있다. ReLU의 단점은 학습률이 너무 크면 뉴런이 포화
    'saturated될 수 오끄斗는 점이다．

     features = tf. range(-2, 3)
     # Keep note ()f the uatue fb尸 negative features
     sess. run([features, tf. nn.relu(features)])


    예제 코드의 출력은 아래와같다：


     [array([-2, -1, 0, 1, 2],        dtype=1nt32),   array([0, 0, 0, 1,2],
     dtype=1nt32)]


                                      （벡터）
    이 예제에서 입력은정수값［-2, 3】사이를 가지는 랭크 1 텐서  이다．
                                           tf. rin. rellu

    는0보다작은값은0으로만들고，
                  다른값들은변화되지 않는다．


    TF.SIGMOID

    시그모이드 함수는 [0.0, 1.0] 사이의 값을돌려준다. 큰 값들은 t-F. sigmoid가 1.0에 가
          작은 값은 0.0에 가까운 값으로 변화된다．
    까운 값으로，                      시그모이드가[0.0, 1.0] 사이의

    값을유지 한다는 점은[0.0, 1.0]사이의 확률값에 따라학습되는 신경망에 유용하다．
                                                  출
    력값의 범위가 줄어드는 것은 입력이 포화되거나 입력에서의 변화가 과장되는 경우에
    문제가 될수도 있다．


     # Note, tf. sLgmoLd (tf.nn.sLgmoLd) is currentLy UinLted to 月Oat vaLues
     features = t-F. to_f]oat(tf. range(- ,   ))
     sess. run([-features, tf. sigmoid(features)])



    위의 예제 코드의 출력은아래와같다：

     [array([-1.,    0., 1.,   2.], dtype=float32),array([ 0.26894143, 0. 5,
     0.7310586, 0.88079703], dtype=float32)]




CHAPTER 6 물체 인식 및 분류


===== PAGE 184 =====
이 예에서，                              1이 1.0이 된다）
     정수값ntege「의 범위가실수값ifoat으로 변환된후＜즉，         ,시그모
이드 함수가 적용된다. 값 0.0이 시그모이드 함수어］주어지면, 결과는 시그모이드 정의
구역의 중간인 0.5가 된다. 0.5가 시그모이드의 중간이라는 점은 음수값도 시그모이드
에는 입력으로 사용될수 있다는 것을 의미한다．


TF.TANF

        （하이퍼볼릭，
Hyperbolic       탄젠트 함수는 tf. sigmoid 함수와유사해서 장단점
              쌍곡선）
도 유사하다．
      둘 사이의 큰 차이점은 tf.tanh는 [-1.0, 1.0] 범위를 사용한다는 점이다．
음수를출력하는장점은특정 신경망구조에 유용할수 있다．

 # Note, tf. tanh (tf. nn. tanh) is currentLy LLmited to float vaLues
 -Features = tf. to_f1oat(tf. range(- ,   ))
 sess.run([-features, tf. tanh(-Features)])



이 예제의 출력 결과는아래와같다：

 [array({-1. , 0. , 1.,   2. ], dtype=float32), array([-0.76159418, 0. ,
 0.76159418, 0.96402758], dtype=float32)]



이 예제에서, 모든셋업은tf. sigmoid 예제와동일하고출력만다르다. tf.tanh의 출
력에서 중간 위치는0.0이고음수값을 가진다. 신경망의 다음 레이어가음수나 0.0에 대
한대비가 없다면 문제가 될수 있다．


TF.NN.DROPOUT

조절이 가능한확률값에 따라서 출력을 0.0으로 설정할수 있다. 이 레이어는 약간의 랜
덤성이 학습을도울수 있는시나리오상에서 잘동작한다. 예를들어, 학습할어떤 패턴
이 이웃특징값에 강하게 연결되어 있는 경우라면, 이 레이어는학습된 출력에 약간의
노이즈를 추가할 것이다．

각주      잇 레이어는학습과정에서만사용되어야한다· 추가할 랜덤 노이즈가테스트과정 중
        에 오류를발생시킬수도 있기 때문이다．



                                                                    Common Layers   1173


===== PAGE 185 =====
     -features = t-f.constant([-0.1, 0.0, 0.1, 0.:])
     # Note, the output shouLd be dLfferent 아7 aLmost ever execution.
     Your numbers won't match this output.
     sess. run(Ifeatures, tf. nn.dropout(features, keep_prob=0.5)])

                                                             -v '' - O9乙
    예제 코드의출력은아래와같다．
                  .


     [array([-0.1, 0., 0.1, 0.2], dtype=float32), array([-0., 0., 0.2,
     0.40000001], dtype=float32)]



    이 예제에서, 출력은50%의 확률로유지된다. 이 레이어의 실행 결과는매번다른 결과
       （랜덤한결과）
    를보인다     , 출력이떨어지면결과는0.0으로세팅된다．



    POOLING LAYER

    풀링 레이어는 과적합over-fitting을 줄이고 입력을 크기를 줄임으로써 성능을 향상시킨
    다. 풀링 레이어는다음 레이어를 위해서 중요한 정보는유지하면서 입력의 크기를줄이
    기 위해서 사용된다. 입력의 크기는tf.nn.conv2d로줄일수도 있다．
                                           그러나풀링 레이

    어가더욱빠르다．


    TF.NN.MAX POOL

    텐서 위를 스트라이딩하면서 커널 크기 안에서의 최대값을 선택한다．
                                       입력 데이터의밝
    기가 이미지의 중요도와유관할때 유용하다．




CHAPTER 6 물체 인식 및 분류


===== PAGE 186 =====
같은 예제에 대한코드가 아래에 있다. 텐서 내부에서 가장큰 값을 찾는 것이 목표이다．



# UsuaLLy the input wouLd be output from α previous Layer and not an image directLy.
batch size=1
input_height = 3
input_width = 3
input_channels = 1


layer_input = tf. constant([
         [
             [[1.0], [0.2], [1. 5]],
               [[0.1], [1.2], [1.4]],
               [[1.1], [0.4], [8.4]]




# The strides wILL Look at the entire input 勻／ using the image_height and image_width
kernel = [batch_size, input_height, input_width, input_channels]
max_pool = t-f.nn.max_pool(layer_input, kernel, [1, 1, 1, lb   "VALID")
 sess. run(max_pool)




                                                                  Common Layers   1 175


===== PAGE 187 =====
    예제 코드의 출력은아래와같다．

     array([[[[   1]]], dtype=fl0at32)


    layer_input은 tf. nn. conv2d의 출력 또는 활성화 함수와 비슷한 모양의 텐서이다．
    목표는 텐서에서의 가장 큰 값을 하나만 추출하는 것이다. 이 예제에서, 텐서의 가장 큰
    값은1.5인데, 입력과동일한형식으로 반환된다. kernel이 더 작은값이라면, 이미지 위
    를스트라이드하면서 각 커널에서의 가장큰값을 선택할 것이다．

                                                 이는보통 " 2 X 2 max-
    ,max-pooling은2x2수용 영역「eceptive field이 주로 사용된다．
                        2x2수용 영역을사용하는 이유는한단계에서 수
    pooling오퍼레이션" 이라고불린다．
    행될수 있는 가장작은 다운 샘플링인데, lxi 수용 영역은 동일한 출력 결과를 보이기
    때문이다．


    TF.NN.AVG POOL

    텐서 위를 스트라이드하고 커널 크기 내부의 각 깊이depth의 모든 값들을 평균한다．커
    널 전체가중요한 경우, 예를 들어서 큰 폭과높이를 가지면서 깊이가 얕은 텐서의 값을
    줄일때 유용하다．




                                回回回
                                              ㄱ
                   1.0                   1.0 -
                                                  -
                   1.0
                                         0.   0   H■
                   0.0                   6끼
                                                  7




CHAPTER 6 물체 인식 및 분류


===== PAGE 188 =====
동일한 예에 대한 코드는 아래와 같다. 목표는 텐서 내부의 모든 값의 평균을 구하는 것
이다．


batd1 size=l
input_height = 3
input_width = 3
input_channels = 1


layer_input = t-F.constant([
        {
               [[1.0], [1.0], [1.0]],
               [[1.0]J [e, 5]J [0.0]]J
               [[0.0]J 〔e.0]J [0.0]]




# The strides wiLL Look at the entire input 勻／ using the image_height and image_width
kernel = [batch_size., input_height, input_width, input_channels]
max_pool = t-f.nn.avg_pool(layer_input, kernel, [1, 1, 1, 1],"VALID')
sess. run(max_pool)




출력 결과는 아래와 같다：

array([[[[ 0.5]]]], dtype=float32)


텐서 내부의 모든 값을 더하고, 텐서 내부의 스칼라 값들의 개수로 나눈다．


    1.0+ 1. 0+ 1. 0+ 1. 0 +0. 5 +0.0+ 0.0 +0.0 +0.0
                            9. 0


커널의 크기만 다르고 나머지 부 분 은 위의 예제 코드와동일하다. 출력의 크기를조절하

는 것도 가능하다．




                                                                  Common Layers   - 177


===== PAGE 189 =====
            정규화
              （normalization)

            茹干화 레이어는 CNN에서만 사용되는 것은 아니고, 또자주 사용되지는 않는다. tf.
            nfl.relu를사용할 때 출력을 정규화하는 것을 고려할 필요가 있다. ReLU가 값의 제한
            ' 作i기 때문에고주파high-frequency특징값들을식별하려면엔旦칫멨콘是콧j培를할
            필요가 있다．

            tf.nn.locaL_response_normalization(tt.nn.lrn)

            Local response normalization은 텐서플로우문서에 가장 잘 설명되어 있는 덧셈 오퍼
            레이션에 기반해서 출력 모양을 정하는함수이다．

                  …Within a given vector, each component is divided by the weighted, squared
                  sum of inputs within depth radius.


            정규화의 목적은 입력을志丸홴쁘交녕照慰학는 것' 따· 예를들어，
                                             [0.0,
            1.0] 범위로 입력을 茹子화하면, 모든 입력은 0.0 이상1.0 이하의 값으로 표현된다．
                                                             local
            response normalization은각값을중요도를고려하면서 제干화한다．

                           （그gN 구조에서 local response normalization을사용하면유
            Cuda-Convnet에 어떤
            용한지 그 이유에 대한자세한 설명이 있다. ImageNet은tf. nn. relu의출력을 정규화
            하기 위해서 이 레이어를사용한다．

             # Create α range 0f 3 floats.
             # TensorShape(fbatchJ image_height. image_t'idth, image_channeL57夕
             layer_input = t-F.constant([
                      [[[    ]], [[     ]], [[    ]]]
                      ])
             lrn = t-F. nn. local_response_normalization( layer_input)
             sess. run([layer_iriput, lrn])




178 -   CHAPTER6 물체 인식 및 분류


===== PAGE 190 =====
이 예제의 출력은 아래와 같다：


[array([[[[ 1.]],
    [[   2.   ]],
    [[ 3.]]]], dtype=fioat32), array([[[[ 0.70710677]],
    [[ 8. 89442718]],
    [[ 0.94868326]]]], dtype=float32)]



이 예제 코드에서, layer_input은 [batch, image－力ei미it, image_width, image_
channel외 형식이다. 稍干화는출력을 [-1.0, 1.0] 범위로 만든다. tf.nn.relu를 위해
서 이 레이어는 제한이 없는출력값이 동일한 범위로만들어질 것이다．



               （고차원 레이어）
네gh Level Layers

텐서플로우는 표준 레이어를 쉽게 만들기 위해서 고차원 레이어를 도입하였는데, 꼭사
용할 필요는 없지만, 중복된 코드를 제거할 수 있도록 해주기 때문이다. 이 레이어들은
그래프에 필수적이지는 않는 노드들을 추가한다. 이 레이어를 사용하기 전에 기본척인
사항들이 익숙해질 때까지 기다리자．


TF.CONTRBLAYERS.CONVOLUTION2D

convolution2d 레이어는 웨이트 초기화, 바이어스 초기화，
                                    학습할 변수 출력, 바이어
스 덧셈, 활성화함수를추가하는 것을 포함해서 tf.nn.conv2d와동일한 로직으로 동
                                         －∼·
                                               ∼∼？   ,=＇∼V~\   /.V一∼*     1，   군1,


작한다. 이런단계들은CNN에서 소개되지는 않았지만눈에 익숙할 것이다. 커널은 학
습해야 하는 변수들이다                          . 웨이트 초
           （CNN의 목표가 바로 이 변수를 학습하는 것이다）
                             （tf. truncated_normal). 나
기화는 첫 번째 학습 시에 커널을 값들로 채우는과정이다
머지 파라미터들은축약된 버전이라는 차이점만 있을뿐, 이전에 사용한 것과유사하다.
완전한 커널을 선언하는대신단순하게 (1,1) 크기의 커널을사용해보자．




                                                                        Common Layers   I 179


===== PAGE 191 =====
image_input = tf.constant([
         [
             [[0., 0., 0.], [255., 255., 255.], [254.,0., 0.]],
             [[0., 191., 0.], [3., 108., 233.], [0.,191., 0.]],
             [[254., 0., 0.], [255., 255., 255.], [0.,0., 0.]]




conv2d = t-f.contrib.layers.convolution2d(image_input, num_output_channels=4,
kernel_size=(1,1), # It눙 on勻／ the fiLter height and width.
activation_fn=tF.nn. relu,
stride=(1, 1), # Skips the stride vaLues for image_batch and input_channeLs.
trainable=True)


# It눙 required to initi（요ize the variabLes used in convoLution2d성 setup.
sess. run(tf. initialize_ a11_variab1es() )
sess . run(conv2d)



               예제 코드의 출력은 아래와 같다．


                array([[[[ 0., 0., 0., 0.],
                     [ 166.44549561, 0. , 0., 0.],
                     [ 171.00466919, 0. , 0., 0. 〕］J
                     [[ 28. 54177475, 0., 59.9046936, 0.],
                     [ 0., 124.69891357, 0., 0.],
                     [ 28. 54177475, 0., 59.9046936, 0.]],
                     [[ 171.00466919, 0., 0., 0.],
                     [ 166.44549561, 8. , 0., 0.],
                     [ 0., 0., 0., 0.]]]], dtype=fl0at32)



               이 예제는 이미지 하나의 배치에 대해서 완전환 컨볼루션을 수행한다. 모든 파라미터는
               이 장에서 소개된 내용이다. 차이점은 tf. contrib.layers. convolution2d가 다시
               작성할 필요없이 많은 양의 셋업을 수행한다는 것이다. 고급 사용자에게는 시간을 절약
               할수 있는방법이다．



 180 -   CHAPTER6 물체 인식 및 분류


===== PAGE 192 =====
각주        tf. to_float는 입력이 이미지라면 사용해서는 안된다．
                                           대신 tf. image. convert_
          image_dtype을 사용해서 값들이 색상을 표현하는데 적합하도록 하자. 이 예제 코드
          에서 텐서플로우는 색상의 범위가〔0, 1]사이의 실수값으로 표현되어야한다．



TF.CONTRIB.LAYERS.FULLY CONNECTED

완전 연결 레이어fuRy connected taye七 모든 입력이 모든 출력에 연결된다．
                                                이것은 많은
신경망구조에 일반적인 연결 형태' 凶만，
                     CNN에서는그렇지 않다·￡씬妗U毛므브
         O1된늦뎃，tf.contrib.layers.fully_connected를 O1*
브聖rj간定롯璧르，
해서만들수 있다．

일반적으로 텐서플로우에서의 완전 연결 레이어는tf.matmul(features, wei助t)
+ bias 형식으로사용하는데, feature, weight, bias는모두 텐서이다. 이 방법은

weight와bias 텐서와관련된복잡한 내용을다루어주면서 동일한 일을 처리할수 있게
해준다．

features = tf. constant({
           [[1.2], [3.4]]
     〕)
 fc = tf. contrib.layers .fullyconnected(-Features, num_output_units= )
 # 工t눙 requLred to inittatLze αLL the variabtes first or 柚ere그L be
 αn error about precondLtLon fαitures.
 sess .run(tf. initialize--all-.variablesO)
 sess. run(fc)



출력은아래와같다．

 array([[[-0. 53210509, @.74457598].,[-1. 50763106, 2.10963178]]],
   dtype=f10at32)


이 예제는 완전 연결 레이어를 만들고 입력 텐서를 출력의 각 뉴런들과 연결한다. 다른
완전 연결 레이어를 미세 조정하기 위한많은파라미터들이 있다．




                                                                     Common Layers   - 181


===== PAGE 193 =====
            LAY티：之 隅PUT

                                               （최소한）
            각 레이어는 CNN 구조에서 특정 기능을담당한다. 추상적으로 윗단   에서 각각
            을 이해하는 것이 중요한데, 실제로 실습을 하지 않으면 잊기 쉽다. 신경망에서 필수적
            인레이어는 입력이 학습과 테스트를 위해서 제공되는 입력 레이어이다. 물체 인식과분
            류를 위해서 입력 레이어는 f!nn. conv2d를통해서 이미지를 입력 받는다. 다음단계
            는 tf. constant나 tf.range 변수의 형식으로 예제 입력 대신에 실제 이미지를 학습
            에 사용하는 것이다．




            이미지와 텐서플로우


            텐서플로우는 신경망의 입력으로 이미지를 사용할 수 있도록 설계되었다. 텐서플로우
            는 일반적인파일 형식
                      （IPG, PNG）          다양한색 공간
                               들의 로딩을 지원하고，     （RGB, RGBA)
            과 일반적인 이미지 조작 기능을 제공한다. 텐서플로우는 이미지를 사용하기 쉽게 해주
            지만, 어려운부분도 있다. 가장큰 어려운 점은로딩된 텐서의 크기이다. 모든 이미지는
                                                           채널들은 각채
            이미지의 height * width * channels의 크기와동일한 텐서가 필요하다．
                           「ank 1의텐서를 표현한다．
            널당 색의 개수에 해당하는랭크

            빨강RGB 픽셀은 텐츠 It       우            은텐서로표현된다．

             red = tf. constant([255, 0, 0])



            각 스칼라 값은 다른 색상을 표현하거나 색상들을 혼합하기 위해서 변경될 수 있다. 픽
            셀의 랭크 1 텐서는RGB 색 공간에서 [red, green, blue] 형식이다. 이미지의 모든
            픽셀은 디스크의 파일에 저장되어 있고，
                                텐서플로우가 斗용하기 위해서는 메모리로 읽
            혀져야한다．




182,!   CHAPTER6 물체 인식 및 분류


===== PAGE 194 =====
이미지 로딩

텐서플로우는 디스크에서 파일을빨리 로딩할 수 있도록 설계되었다. 이미지 로딩은 파
일의 내용물을 디코딩decoding하기 전에는 다른 이진 파일binary file을 로딩하는 것과동
일하다．
   아래의 3x3 픽셀의 RGB JFG 파일을 로딩하는 것은 다른 형식의 파일을 로딩
하는것과유사한과정을수행한다．




                           H
 # The match_fiLename흰－once wtLt accept α regex but there Ls no need for thLs exampLe.
 image_filename = " . /images/chapter-05-object-recognition-andclassification/
 working-with-images/test4nput- image .jpg '
 filename_queue = tf. train .string_input_producer(
 t-F .train .match_filenames_once(image_fllename))


 image- reader = tf. WholeFileReader()
 -J image file = image_reader.read(fllename-queue)
 image = tf. image.decode_jpeg(image_file)


이 코드가 있는 곳에서 상대 주소 디렉터리에 있는 이미지가 수행된다. t-F.train.
string_inputproduce
                  「는 그 파일을 찾고 로딩을 위한큐queue에 추가한다. 이미지
로딩은 전체 파일을 로딩하기 위해 필요한 메모리가 필요하고
                               （tf.WholeFileReader).
파일이 읽혀지면
       （image_reader. read) 결과 이미지가 디코딩된다
                                        （tf. image,
decode_jpeg).

이제 그 이름으로는 오직 하나의 파일이 있기 때문에, 큐는 언제나동일한 이미지를반

환한다．




                                                                 이미지와텐서플로우       - 183


===== PAGE 195 =====
             sess.run(image)


            그출력은아래와같다：

             array([［〔 0, 0, 01J
                [255, 255, 255],
                [254, 0, 0]］』
                [[ 0, 191, 01,
                 [ 3, 108, 233],
                 [ 0, 191, 0]]J
                [[254, 0, 0],
                [255, 255, 255],
                 [ 0, 0, 0]]], dtype=uint8)



            로딩된 이미지의 출력을 조사해보면, 단순한 랭크 3의 텐서라는 것을 확인할수 있을 것
            이다. RGB 값은9개의 랭크1텐서에 있다. 메모리에 로딩된 이미지의 형태는 [batch_
            size, image_height, image_width, channels]0]다.

            이 예제에서의 batch_size는 1인데, 실제로는배치 작업이 이루어지지 않기 때문이다．
            입력을 배치 처리하는부분은 텐서플로우 문서에 자세하게 설명되어 있다. 이미지를다
            룰때는 원래의 이미지를로딩하기에 필요한메모리의 양에 유의하자. 이미지가너무크
            거나너무많으면 시스템이 멈출수도 있다．



            이미지 형식

            이미지가 어떻게 우리의 모델에 영향을 끼치는지 아는 것은 중요하다. RED Weapon
                            （이 책을 쓰는 지금은 6144 x 3160 크기이다）
            Camera로부터 하나의 프레임                            으로 신경
            망을 학습시키면 어떤 일이 일어날지 고려해보자. 이 프레임은 3차원 색상값을 가진
            19,415,040 랭크인하나의 텐서이다．

            실제로，
               그 정도 크기의 입력은 엄청난 메모리가 필요하다. CNN을학습시키는 것은많




184 -   CHAPTER6 물체 인식 및 분류


===== PAGE 196 =====
은 시간이 필요한데, 매우 큰 파일을 로딩하는 것은 속도를 느리게 만든다. 시간이 느려
지는 것은 참을수 있다고 하더라도，
                  이 정도 크기의 이미지는 지금 대부분의 GPU에맞
지 않을 것이다．

큰 입력 이미지는 대부분의 CNN을 학습시킬 때 비 생산적이다. CNN은 이미지 내부
의 고유의특성을찾으려고 하기 때문에, 큰 입력을 사용하면모델을 일반화하기에는너
무많은관련 없는 정보로넘치게 된다．

Stanford Dogs Dataset에서 Pug로 인식되어야하는 같은품종이면서 아주 다른 이미
지들이 있다. 이 이미지들에는 학습과정을 어렵게 하는 불필요한 정보들이 너무 많다．
예를들어, 아래 그림에서의 모자는불필요한 정보이다．




       n02110958 2410.jpg       n02110958 4030.jpg



이미지에서 중요한 정보를 부각시키는 작업은 그것들을 적절한 파일 형식으로 저장하
고 사용함으로써 가능하다. 다양한 형태들을 사용함으로써 다양한 문제를 해결할 수 있
을것이다．



JPEG와 PNG

텐서플로우는 이미지 데이터를 디코딩하기 위해서 2가지 종류의 파일 형식을 사용한다．
하나는tf. image. decode_jpeg이고,다른하나는tf.image.decode_png이다. 이 파
일 형식들은 컫퓨터 비전분야에서는 일반적인파일 형식이다．




                                                     이미지와텐서플로우   - 185


===== PAGE 197 =====
             PNG 파일은 알파alpha 채널을 저장하지만, JPEG는 저장하지 않는다．
                                                      만약 알파 정보
            （투명도）                           이미지의 특정 부분을 잘
                를 학습에 사용하려면 중요한 사항이다. 예를 들어서，
              라서, 그 부분을 알파 값을 0으로 해서 투명하게 보관하는 것이 도움이 될수 있기 때문
              이다．

                              이미지에 너무 많은 수정을 하지 않는 것이 좋다．
              JPEG 이미지를 사용할 때는，                         필요하
                                            그리고 학습 시간을줄이기 위해서，
              다면 원래의 이미지「aw image를사용하는 것이 좋다．
              이미지를로딩하기 전에 이미지 수정을미리 해두는 것이 좋다．

              PNG 이미지는 필요한 경우에 수정을 해도 무방하다. PNG 이미지는 무손실lossless 압
              축이기 때문에 원래의 정보를모두 보관한다．



              TFRECORD

              텐서플로우는 하나의 파일어I 이진 데이터와 레이블 데이터를 보관할 수 있는 내장된
              built-in 파일 포맷인 TFRecord 포맷이 있다. 학습 단계 이전에 이미지들을 이 포맷으로
              미리 변환해야 하는 전처리 단계가 있다. 이 포맷의 가장 큰 장점은 이미지와 레이블을
              같미 보관할수 있다는 점이다．

              기술적으로는，TFRecord 파일은protobuf 파일 포맷이다．
                                                 이 파일은 압축되지 않아서
              바로 메모리에 로딩될 수 있기 때문에 빠르다. 이 예제에서 이미지는 TFRecord 포맷으
              로 적혀 있고, 레이블도 저장되어 있다．


# Reuse the image fram earLier and giye it α faIe LabeL
image_label = b' \x0l' # Assume the LabeL data is in α onehot representation (eee0OOe쟈
# Convert the tensor into bytes, notice that this wiLL Load the entire image fiLe
image_loaded = sess.run(image)
image_bytes = image_loaded .tobytes ()
image_height, image_width, image_channels = image_loaded.shape




        CHAPTER 6 물체 인식 및 분류


===== PAGE 198 =====
# ExPort TFRecord
writer = t-F .python_io.lFRecordWriter("./output/trainingimage.tfrecord")


# Don't store the wtdt枋 height or image channeLs in this ExampLe ／江e to save space
but not required.
example =
tf .train .Example (-Features=t-F .train.Features (feature={'label' :
t-f.train.Feature(bytes_list=tf. train.BytesList (value=[image_label])),'image' :
tf. train.Feature(bytes_list=t-F.train.BytesList (value=[image_bytes]))}
 ))

# This wiLL save the exampLe to α text fiLe 勺Frecord
writer .write (example .SerializeloString())
writer .close()


레이블은 멀티－클래스 데이터의 분류를 위해서 일반적으로 사용되는 one-hot 인코딩으

로 저장된다．                                  실제로는 개의 품종
      Stanford Dogs Dataset는 멀티－클래스 데이터이다．

인식을 위해서는 멀티레이블이 더 좋을 것이다. 혼혈 품종이 있을수 있기 때문이다．

                                        이바이트들
예제 코드에서 이미지가메모리에 로딩되고 바이트byte들의 배열로 변환된다．
                            디스크에 저장되기 전에 SerializeloString
이 t-F.train.Example 파일에 더해지고，

으로 시리얼라이즈serialze된다. 시리얼라이즈는 메모리에 있는 것을 파일로 전송하기

위해서 안전한 포맷으로 변환하는 작업이다. 시리얼라이즈된 예제는 로딩될 수 있는 포

맷으로 저장되고, 예제 포맷으로 다시 역으로 역－시리얼라이즈된다de-seriatized.

TFRecord 포맷으로 저장되어 있어서, 이제 TFRecord 파일에서 로딩될 수 있다. 학습

을 위해서 이미지와 레이블을 로딩하는 것이다. 이미지와 레이블을 따로 로딩하는 것보
다 시간을줄일 수 있다．




                                                                        이미지와 텐서플로우   - 187


===== PAGE 199 =====
# z.oad rFRecord
tF_record_filename_queue = tf.train.string_input_producer(
tf.train.match_filenames_once( "./output/trainingimage.tfrecord"))


# Notice the different record reader, this one -is designed to work with TFRecord
fiLes which may have more than one exampLe in them.
tf_record_reader = tf.TFRecordReader()
-, t-f_record_serialized = tf_record_reader.read(t-F_record_filename_queue)


# The LabeL and image are stored as bytes but couLd be
stored as int64 or fl0at64 vaLues in α seriaLized tf.ExampLe protobuf.
tf_record_features = t-f. parse_single_example(
    tf_record_serialized,
    features={
          'label': tf.FixedLenFeature([], tf.string),
          'image': tf.FixedLenFeature([], t-F.string),
    })

# Using tf.uint8 because aLL of the channeL inf0rmation is between 0-255
tF_record_image = tf.decode_raw(t-f_record_features[ ' image'], t-f. uint8)


# Reshape the image to Look Like the image saved, not required
t-F_record_image = tf.reshape(tf_record_image, [image_height, image_width, image_
channels])


# Use reaL vaLues for the height, width and channeLs af the
image because it눙 required to reshape the input.
tf_record_label = tf. cast(t-F_record_features[ 'label'], tf. string)


               먼저, 다른파일과동일한방식으로로딩된다. 가장큰차이점은파일이 TFRecordReader

               로 읽혀진다는 점이다. 이미지를 디코딩하는 대신, TFRecord는 t-F. parse_single_

               example로파싱되고, 이미지는원래의 raw 바이트로 읽혀진다
                                                 （tf. decode_raw).


               파일이 로딩된 후, tf. nn . conv2d가사용하는 [imageJieight, image_width,

                              와 같은 형식으로 보관하기 위해서 tf. reshape을 사용한다．
               image_channnels］




  188 -   CHAPTER 6 물체 인식 및분류


===== PAGE 200 =====
batch_size 차원을 input_batd，
                         로 추가하기 위해서 tf. expand를 이용해서 차원을
확장할수 있다．

위의 경우에는 이미지 하나가TFRecord에 있었지만, 이 레코드 파일들은 여러 예제가
포함되어도 된다. 전체 학습 셋트를 하나의 TFRecord 파일에 보관해도 되고 ，여러 개
의 파일로 나누어도 무방하다．

아래의 코드는 디스크에 저장될 파일이 텐서플로우에 로딩된 이미지와 동일한지 체크
한다．

sess.run(tf.equal(image, tf_record_image))


예제의출력은아래와같다：

 array([[[ True, True, True],
     [ True, True, True],
     [ True, True, True]],
     [[ True, True, True],
     [ True, True, True],
     [ True, True, True]],
     [[ True, True, True],
     [ True, True, True],
     [ True, True, True]]], dtype=bool)



원래 이미지의 모든 특성과 TFRecord 파일에서 로딩된 이미지는 동일하다. 확실히
하기 위해서 TFRecord 파일에서 레이블을 로딩하고 원래 저장된 것과 동일한지 체
크하자．

 # Check that the LabeL Ls 5tiLL 0b0000000그．
 sess . run(tf_ record_iabel)




                                                이미지와 텐서플로우   - 189


===== PAGE 201 =====
    출력은 아래와 같다：

     b' \xel1


    원래의 raw 이미지 데이터와출력 레이블을 함께 저장하는 파일을 만듦으로써 학습 동
    안의 일을줄일수 있다. 이미지를다룰때는TFRecord 파일을사용하는 것을추천한다．
    최소한 학습 전에 전처리를 미리 하는 것도 좋다. 로딩할 때마다 이미지를 수정하는 것
    은좋은방법이 아니다．



    이미지 조작

    CNN은 아주 많은 다양한 품질의 학습 데이터가 있을 때 잘 작동한다．
                                          Stanford Dogs
    Dataset에서 이미지들은 그림 속의 개를 강조한다. 중앙에 명확하게 개를 포함한 그림
    은배경 쪽에 개를가진그림보다 더 좋다．

    모든 데이터셋이 가장 좋은 이미지들은 아니다. Stanford Dogs Dataset의 아래의 두
    이미지를 보자．
           왼쪽의 이미지는 전형적인 Mexican Hairless Dog이1긱 오른쪽의 이미
    지는Mexican Hairless Dog으로 놀라는파티 장면이다．
                                       오른쪽의 그림은파티에 참석
    한사람들의 얼굴을 학습시킬지도 모를 정도로 불필요한 정보를 포함하고 있다. 이러한
    그림은사람대신 개를 강조하기 위해서 조금수정될 필요가 있다．




                n02113978_3480.jpg   n02113978_1030.jpg



CHAPTER 6 물체 인식 및 분류


===== PAGE 202 =====
이미지 조작은 대부분의 경우에 전처리 작업으로 이루어져야 한다. 이미지는 필요한 부
                      「esize, 색상 레벨을 조절할 수 있다. 또한 이미
분을 잘라내거나crop, 크기를 변경하거나
지가 로딩된 후에，
         ffip되거나 네트워크에 다양한 입력 정보를주기 위해서 변형distorted
이 가해질수도 있다．
          이단계는 더 많은 처리 시간이 필요하지만오버피팅overtitting을막
는데 도움이 될수 있다．

텐서플로우는 이미지 조작 프레임워크가 아니다. 텐서플로우보다 이미지 조작을 위해
서는 다양한 파이썬 라이브러리가 있다
                   （PIL, OpenCV). 텐서플로우에서는 CNN 학습
과관련된몇 가지 유용한 기능을요약해보자．



CROPPING

                            크로핑은 전체 텐서에서 텐서의 일
크로핑cropping은불필요한 영역을삭제하는 것이다．
부분을삭제하는tf. slice와유사하다. CNN을 위해서 입력 이미지를크로핑하는 것
은불필요한차원이 있는 경우에 유용한다. 예를들어, 개가중앙에 있는 이미지를크로
핑하면 입력의 크기를줄일수 있다．

 sess. run(tf. image.central_crop(image, 0.1))


위의 출력은 아래와 같다：

 array([[[ 3, 108, 233]]], dtype=uint8)


t-F. image. central_crop은 이미지의 10％를잘라내고반환한다. 이방법은 언제나 이
미지의중앙이 사용된다는 것을 가정한다．

크로핑은 일반적으로 전처리 단계에서 수행되지만，
                         배경background이 유용할 경우에는
학습동안에서 사용될 수 있다. 배경이 유용한 경우에는 크로핑이 시작되는 시점을랜덤
하게 정해서 수행된다．




                                                 이미지와 텐서플로우   - 191


===== PAGE 203 =====
# This cr이〕method onLy vorks on reaL vaLue input.
real_image = sess.run(image)


bounding_crop = t-F. image. crop_to_bounding_box(
    real_image, of fset_height=0, offset_width=0, target_height=2, target_width=l)


sess . run(bounding_crop)



                  수행 결과는 아래와 같다：


                   array([[[ 0, 0, 0]], [[ 0, 191, 0]]], dtype=uint8)


                  예제 코드는 tf. image. crop_to_bounding_box를 이용해서 이미지의 (0, 0) 좌표에

                  서 시작해서 이미지를 잘라낸다．
                                  이 함수는 정의된 형태shape의 텐서에 잘작동한다．



                  PADDING

                  패딩padding은 이미지를 원하는 크기와 맞추기 위해서 0으로 채우는 작업이다. tf. pad
                  를 이용할 수 있는데, 텐서플로우는 아주 크거나 아주 작은 이미지의 크기를 바꾸기 위

                  해서 다른 함수를 제공한다. 이 함수는 이미지의 가장자리에 0을 포함하는 아주 작은 이
                  미지를 패딩한다. 종종 다른 함수는 이미지의 크기를 변경할 때 이미지를 왜곡시키기도
                  하기 때문에 이 함수를 사용한다．


# This padding method on勻／ Wor朽 on reaL V(孔ue input.
real_image = sess.run(image)


pad = tf. image. pad_to_bounding_box(
    real_image, offset_height=0, offset_width=0, target_height=4, target_width=4)


sess . run(pad)




 192 -   CHAPTER6 물체 인식 및 분류


===== PAGE 204 =====
이 예제의 출력은 아래와 같다：


array (〔［[ 0, 0, 0],
    [255, 255, 255]'
    [254, 0, 01,
    [ 0, e, 0]]J
    [[ 0J 191J 0],
    [ 3, 108, 233],
    [ 0, 191, 0],
    [ 0J 0J 0]]J
    [[254, 0, 0],
    [255, 255, 255],
    [ 0J 0J 01J
    [ 0J 0J 01]J
    [[ 0J 0J 0],
    [ 0J 0J 0]J
    [ 0, 0J 0]J
    [ 0J 0J 0]]]J dtype=uint8)



이 예제 코드는 이미지의 높이와폭을 1 픽셀 키운다. 새로운 픽셀의 값은0이다. 이런방
식의 패딩은 아주 작은 이미지의 크기를 키울 때 유용하다. 학습 중에 이미지의 가로 세
로 비율이 섞인 데이터를다룰때도 용이하다. 텐서플로우는 pad와 crop 함수를 결합해

서 해결할 수 있다．


# TIrLs paddthg method onLy works on reaL vaLue input.
real_image = sess.run(image)


crop_or_pad = tf. image.resize_image_with_crop_or_pad(real_image, target_height=2,
    target_width=5)


sess . run(crop_or_pad)




                                                             이미지와 텐서플로우       - 193


===== PAGE 205 =====
    이 예제의 출력은아래와같다：


     array([［〔 0, 0, 0],
         [ 0, 0, 0]J
         [255, 255, 255],
         [254, 0, 0],
         [ 0J 0, 0]]J
         [[ 0, 0, 0]J
         [ 0, 191, 0],
         [ 3, 108, 233],
         [ 8, 191, 0],
         [ 0, 0, 0]]], dtype=ulnt8)


    real_image는높이가2픽셀 줄어들고 폭은0을 패딩해서 늘어난다. 이 함수는 입력 이
    미지의중앙을 기준으로 이루어진다．



    F니PPING

                                각 픽셀의 위치가수평 또는수직으로
    이미지를플리핑flipping하는 것은단어 뜻 그대로，
    뒤집어지는 것이다. 플리핑을 하면 학습을 위해서 동일한 이미지를 다양한 관점에서 학
    습할수있도록해준다. 예를들어, 오른쪽귀가굽은개 사진을플리핑함으로써, 왼쪽귀
    가굽은 이미지를학습할수 있도록 해주는등이다．

    텐서플로우는 이미지를 수평 또는 수직으로 랜덤하게 플리핑하는 함수가 있다. 랜덤한
    이미지 플리핑은 모델이 플리핑된 이미지에 오버피팅되는 것을막아준다．

     top_left_pixels = tf. slice(image, [0, 0, 0], [2, 2, 3])


     flip horizon = tf. iniage.flipleft_ right(top_le-Ft_pixels)
     flip_vertical = tf. image.flipup_down(flip_horizon)


     sess. run([top_left_pixels, flip_vertical])




CHAPTER 6 물체 인식 및 분류


===== PAGE 206 =====
예제 코드의 출력 결과는 아래와 같다：


[array([[[ 0, 0, 0],
     [255, 255, 255]]J
    [[ 0, 191, 01,
    [ 3, 108, 233]]], dtype=uint8), array([[[ 3, 108, 233],
     [ 0, 191J 01]J
    [[255, 255, 255],
    [ 0, 0, 0]]], dtype=uint8) J


이 예제 코드는 이미지의 일부를수평으로 그리고 수직으로 플리핑한다. 이미지들의 일

부만t-F. slice를사용하는데, 플립된 원래의 이미지가동일한 이미지를 반환하기 때

문이다
  （이 예제에만 해당）
            . 픽셀들의 일부는 이미지가플립되었을 때의 차이를 보인다．
tf. image.flip_left_ri帥t와 tf. image. flop_up_down 이 두 함수는 이미지의 크기

에 제한되지 않는다. 이들은한 번만에 이미지를플립하는데, 이미지를 랜덤하게 플립하
는 것은 별도의 함수들에 의해서 수행된다．


 top_left_pixels = tf. slice(image, [0, 0, 0], [2, 2, 3])


 random_flip_horizon = tf. image. random_flip_left_right(top_left_pixels)
 random_flip_vertical = tf. image. random_flip_up_down( random_flip_horizon)


 sess. run(random_flip_vertical)


예제 코드의 출력은 아래와 같다：


 array([[[ 3, 108, 233],
     [ 0, 191, 0]]J
     [[255, 255, 255],
     [ 0, 0, 0]]], dtype=uint8)




                                                                   이미지와 텐서플로우   - 195


===== PAGE 207 =====
              이 예제는출력이 랜덤이란 것만다르고 이전 예제와동일하다. 따라서 매 번다른출력
              이 나온다. seed라는파라미터가랜덤성을조절한다．



              채도
               （Saturation）
                          과 균형
                             （Balance)

              인터넷에서 구할 수 있는 이미지들은 종종 미리 수정되어 있다. 예를 들어, Stanford
              Dogs Dataset의 이미지들중많은 이미지들은채도가높다tots of Co[or. 이렇게 수정된 이
              미지들을 학습에 사용하면 CNN 모델이 이런 수정된 이미지에 많이 반응하고, 이미지
              의 내용물에 반응하지 않을수도 있다．

              텐서플로우는 채도，
                       색상hue, 대조contrast, 명도brightness 등을 변경하는 함수를 제공한
              다．
               이 함수들은 이러한 이미지의 속정값을 바꾸거나 랜덤하게 변경할 수도 있다. 랜덤
              하게 변경하는 이유는플리핑을 랜덤하게 하는 이유와동일하다．


example_red_pixel = tf. constant([254., 2., 15.])
adjust_brightness = tf. image. adjust brightness(example-red-pixel,


sess.run(adjust_brightness)



              예제 코드의 출력 결과는 아래와같다：


array([ 254.19999695, 2.20000005, 15.19999981], dtype=fl0at32)



              이 예제는 하나의 red 픽셀을 delta 값 0.2로 밝게 한다. 그렇지만 현재의 텐서플로우
              0.8 버전은tF.u1nt8 입력과는잘작동하지 않는다．


adjust_contrast = tf. image.adjust-contrast(image, - .5)


sess.run(tf. slice(adjust-contrast, [1, 0, 0], [1, 3, 3]))




 19히    CHAPTER 6 물체 인식 및분류


===== PAGE 208 =====
예제 코드의 출력 결과는 아래와같다：

array([[[170, 71, 124],
    [168, 112, 7],
    [170, 71, 124]]], dtype=uint8)



이 예제 코드는 대조contrast를 -0.5만큼 바꿔서 잘 알아보지 못하게 이미지를 수정한다．
대조를 수정하는 것은 조금씩 하는 것이 좋다. 많이 변경하면 뉴런을 포화시켜서saturate
최대값이 되게 하면복구할수 없게 된다．

tf. slice 오퍼레이션은 변경된 픽셀들중하나를빨리 강조하는 기능을 한다．

 adjust_hue = tf. image. adjust_hue(image, 0.7)


 sess.run(tf. slice(adjust_hue, [1, 0, 0], [1, 3, 3]))



이 예제 코드의 출력은 아래와 같다：

 array([[[191, 38, 0],
     [ 62, 233, 3],
     [191, 38, 0]]], dtype=uint8)



예제 코드는 이미지의 색상hue 값을 수정해서 더욱색감을높인다. 이함수의 delta 파라
미터는 조절할 색상값의 정도를나타낸다．

 adjust_saturation = tf. image. adjust_saturation(image, 0.4)


 sess. run(t-f. slice(adjust_saturation, [1, 0, 0], [1, 3, 3]))




                                                                  이미지와 텐서플로우   - 作7


===== PAGE 209 =====
    이 예제 코드의 출력은 아래와 같다：

     array([[[114, 191, 11d],
         [141, 183, 233],
         [114, 191, 114]]), dtype=uint8)



    이 코드는 대조contrast를수정하는 것과유사하다. 채도를높이면 색의 변화가 강조되기
    때문에 에지를 식별하기 위해서 이미지의 채도를많이 높이는작업을자주사용한다．



    색상

    일반적으로 CNN은 하나의 색상을 가진 이미지를 사용한다. 이런 경우의 이미지를 그
    레이스케일 색 공간grayscale color space이라 하고，
                                        하나의 색 채널을 가지는 것을 의미한
    다. 대부분의 컴퓨터 비전 관련 작업에서 그레이스케일이면 충분한데, 이미지의 형태는
    색상정보 없이도 판별 가능하기 때문이다. 색상정보를줄이면 이미지의 학습도빨라진
    다. 랭크1 텐서를3개 가지는대신그레이스케일 이미지는 랭크 1 텐서 1개면 되기 때문
    이다．

    그레이스케일이 장점도 있지만, 색상을 이용해서 식별할 필요가 있는분야도 있다는 점
    을 알아두자. 컴퓨터 비전에서 색상을 다루는 것은 쉽지 않다. 왜냐하면 수학적으로 두
    개의 RGB 색깔의 유사성을 정의하기 어렵기 때문이다. CNN 학습에서 색상을 사용하
    기 위해서는 이미지의 색 공간을 변환할 필요가 있다．



    GRAYSCALE

    그레이스케일은RGB[O, 255] 사이의 값을가진하나의 컴포넌트를가진다．

     gray = tf. iniage. rgbto-grayscale(image)

     sess.run(t-f.slice(gray, [ , 0, 0], [1, 3, 1]))




CHAPTER 6 물체 인식 및 분류


===== PAGE 210 =====
출력 결과는 아래와같다；

array([[[ 0],
      [255],
      [ 76]]], dtype=uint8)



이 예제는RGB 이미지를 그레이스케일로 변경한다. tf.slice 오퍼레이션은색이 어
떻게 변경되었는지 확인하기 위해서 첫 줄을잘라낸다. 그레이스케일 변환은 한 픽셀의
모든 색상값의 평균을 사용한다．



HSV

색슈Hue, 채도Saturation, 명도Value가｛sv 색 공간이다. 이 색 공간은 RGB와유사하
게 랭크 1 텐서 3개가 필요하다．
                  Hsv는RGB에 비해서 인간의 색 감각에 더 유사하며，
HSB라고불리기도한다．
           이때 B는밝기Brightness를 의미한다．


hsv = tf. image. rgb_tohsv(tf. image .convert_imagedtype(iniage, tf .float32) )


 sess.run(tf. slice(hsv, [0, 0, 0], [3, 3, 3]))



예제 코 三의 출력은 아래와같다：

array([[[ 0., 0., 0.],
      [ 0. J 0. J 1. ]J
    【 0., 1., 0.99607849]],
      [[ 0.33333334, 1., 0.74901962],
      [ 0.59057975, 0.98712444, 0.91372555],
      [ 0.33333334, 1. J0. 74901962]]J
      [[ 0., 1., 0.99607849],
      [ 0. J 0. J 1. ],
      [ 0., 0., 0.]]], dtype=f]oat32)




                                                                  이미지와텐서플로우       - 199


===== PAGE 211 =====
    RGB

    RGB는 이제까지 모든 예제 코드에서 사용한 색 공간이다．
                                   red[O, 255], green[O, 255],
    Hue[O, 255］
              로써 랭크 1인 텐서 3개로 구성된다. 대부분의 이미지는 보통 원래 RGB 색
    공간으로 표현되는데, 텐서플로우는다른 색 공간으로 표현된 이미지를 위한 빌트인함

    수가있다．


     rgb_hsv = t-F.image.hsv_to_ rgb(hsv)
     rgbgrayscale = tf.image.grayscale_to_rgb(gray)


    예제 코드는 그레이스케일에서 RGB로 변환하는 말이 안되는 부분 빼고는 명확하다．

    RGB는3개의 색상값이 필요한데, 그레이스케일은 1개 밖에 없기 때문에, 이 변환부분
    에서는RGB 값이 모두동일한그레이스케일 값으로 채워진다．



    LAB

    Lab는 텐서플로우가 지원하지 않는 색 공간이다. 그러나Lab는RGB에 비해서 인지 가
    능한 더 넓은 색을 표현할 수 있다. 텐서플로우가 기본적으로는 지원하지 않지만, 전문
    적으로 설정을 하면 사용할 수 있다. python-co1ormath와 같은 파이썬 라이브러리는
    Lab 뿐만아니라다른색 공간도 지원한다．

    Lab 색 공간을 사용하면 RGB나 HSV 보다 색상 차이를 인간에 더 유사하게 매핑할 수

    있는 장점이 있다. Lab 색 공간에서의 두 색상의 유클리디언차이는 다른 색 공간에 비
    해서 더 뚜렷하다．



    이미지 값의 변경

    이 예제에서 tf.to_float는 이미지 타입을 다른 형태로 바꾸는 것을 설명할 때 사용된
    다．
     이렇게 해도 되지만, 텐서플로우는 값의 타입을 변경할 때 값들의 범위를 적절하게
    조절해주는빌트인함수가있다. tf. image. convert_image_dtype(image, dtype,



CHAPTER 6 물체 인식 및 분류


===== PAGE 212 =====
saturate=False) 함수는 이미지의 타입을tf.uint8에서 tf.fioat로 변경해준다．




CNN 구현

텐서플로우를 이용한 물체 인식과 분류는 컨볼루션
                         （（그JN 신경망에서의）
                                     , 일반층

          （즉，
common layer non-linearity, pooling, fc), 이미지 로딩，     색 공간에 대
                                                이미지 조작，
한 이해가 필요하다. 그런 후에, 텐서플로우를 이용해서 영상 인식이나 분류를 위한
CNN 모델을 만들수 있다. 여기서는 모델이 개의 이미지와 개의 품종 이름을 포함하는
Stanford 데이터셋을 이용하여 학습해서, 입력 그림에 따른 개의 품종 이름을맞추는 문
제이다.

신경망의 구조는 Alex Krizhevsky의 AlexNet 모델에서 모든 AlexNet의 레이어를 없
앤 간단한 버젼이다. 이 구조는 ILSVRC'12 대회에서 우승한 네트워크으로 앞부분에서
소개되었다. 이 신경망은CNN의 튜토리얼에서 제공되는 텐서플로우와유사한 레이어
들과 테크닉들을 사용한다．


                                 ]
         Stanford
       Dogs Dataset
        (250 151 1 )
                        convta




                        pool layer 1
                                       ;Ea쁘
                                                   “   '
                                              pool byer 2
                                                           "y푠   『「；

                                                                       ■■
                        (3 63 38 32)          ( 3 32 19 64 )



          Larger                                                            Smaller
       Dimensionality                                                  ' Dimensionality



이 섹션에서 설명되는 네트워크는 각 층의 TensorShape 출력을 포함한다. 레이어들은 왼

쪽에서 오른쪽. 그리고 위에서 아래로 진행하고, 관련된 레이어들이 뭉쳐 있다. 입력이 네트

워크 속에서 흘러감에 따라 깊이는 증가하고 폭과 높이는 감소한다, 깊이에서의 증가는 네

크워크를 사용하기 위해서 필요한 계산량을 줄여준다．




                                                                                          CNN 구현   - 201


===== PAGE 213 =====
    Stanford Dogs 데이터셋

    이 모델을 학습시키기 위한 뎨이터셋은 Stanford의 컴퓨터비전 사이트 /)t切:1/vision.
    stonford.edu/ad1tya86/imageNetDogs／에서 구할 수 있다．
                                                 모델을 학습시키기 위해서
    관련데이터를다운로드해야하J긱모든이미지의 Zip 압축을다운로드한후에，
                                        모델을
    만드는 코드가 있는 동일한 디렉터리 안에 imagenet - dogs라는 새로운 디렉터리에 압
    축을풀자．

    Stanford에 의해 제공되는Zip 파일은120개의 품종으로구성되는개의 이미지이다．
                                                  이
                          나머지 20％로 테스트하는 것이다. 더 엄밀한
    모델의 목표는 80％의 이미지로 학습하고，
    검증을 위해서는 원 데이터의 일부를 교차 검증crass-validation을 위해 남겨두어야 한다．
    교차 검증은모델의 정확도를 검증하기 위한중요한단계이지만,우리는지금 시합을 위
    한 것이 아니라 개발과정을 설명하기 위한 것이기 때문에 이를생략한다．

    데이터의 구조는 ImageNet의 일반적인 방법을따른다．
                                  각 개의 품종이 디렉터리의 이
    름이다. 예를 들면 n02085620-Chihuahua처럼 디렉터리 이름의 뒷부분은 영어로 된
    품종 이름
        （Chihuahua）
                  이다. 각 디렉터리에는 각 품종의 개의 이미지가 있고，
                                               폴더마다
    그 숫자는 일정하지는 않다. 각 이미지는JPEG 형태   이고 크기는 다를 수 있는데，
                                （RGB）
    텐서플로우는 동일한 차원의 텐서를 사용하기 때문에 이미지의 크기가 다른 문제도 해
    결해야한다．



    이미지를 TFRecords로 변환하기

    디렉터리 내부의 원이미지는같은 크기가아니고 품종 이름이 파일에 포함되어 있지 않
    기 때문에 학습에 사용하기 어렵다. 그래서 이미지들을TFRecord 파일로 변환함으로써
    학습올빨리하고 이미지의 레이블을매칭하는과정을단순화할수 있다. 또다른장점은
    이미지와관련된 학습과 테스트 과정을 미리 분리함으로써, 체크 포인트 파일을 이용해
    서 학습하는 도중에 계속적으로테스트를할수 있다는 점이다．

    이미지 변환은 컬러 이미지를그레이스케일로 변환하고, 크기를동일하게 맞추고,각 이



CHAPTER 6 물체 인식 및 분류


===== PAGE 214 =====
미지에 레이블을 붙이는 과정으로써, 학습 과정 이전에 한번만 수행하면 되고, 꽤 오랜

시간이 걸린다．


import glob


image_filenames = glob .glob( " . /imagenet-dogs/n02*/* .jpg")
image_filenames[0:2]


위의 예제 코드의 출력 결과는 아래와같다：


[' . /imagenet-dogs/n02085620-Chihuahua/n02085620_10074. jpg ' ,
 ' ./imagenet-dogs/n02085620-Chihuahua/n02085620_10131. jpg ' ]



데이터셋이 어떻게 구성되었는지의 예이다．
                     glob 모듈은 데이터셋에 존재하는 파일
들의 구조를 보이는 디렉터리의 리스트를 보인다．8자리 숫자는 ImageNet에서 사용

하는 각 종류별 WordNet ID이다．
                     ImageNet은 WordNet ID를 통해서 이미지를 검
색하는 브라우저가 있다．
            예를 들어，
                 Chihuahua 예제는 http://www.image-net.org/
synset?wnid=n02085620를통해서 검색할수 있다．


from itertools import groupby
from collections import de-faultdict


training_dataset = defaultdict(list)
testing_dataset = de-Faultdict (list)


# SpLit up the fiLename into its breed and corresponding fiLename. The breed is f0und
by taking the directory name
image_filename_with_breed = map(lambda filename: (filename.split("/")[2],
filename), image_filenames)


# Group each image by the breed which is the 0th eLement in the tupLe returned above
for dog_breed, breed_images in groupby(image_filename_with_breed, lambda x: x[0]):




                                                                       CNN 구현   口03


===== PAGE 215 =====
   # Enumerate each breed눔 image and send -20% af the images to α testing set
    -For i, breed_image in enumerate(breed_images):
          if j. % 5 볍＝ e :
              testing_dataset{dog_breed]. append(breed_image[l] )
          else:
              training_dataset[dog_breed] .append(breed_image[l] )


    # Check that each breed incLudes at Least 18% of the images fOr testing
    breed_training_count = len(training_dataset[dog_breed])
    breed_testing_count = len(testing_dataset[dog_breed])


    assert round(breed_testing_count I (breed_training_count+
breed_testing_count), 2) > 0.18, "Not enough testing images."



                  이 예제 코드는 디렉터리와 이미지들
                                    （t./imagenetdogs/n02085620-Chihuahua/
                  n02085620_10131.jpg'）을 각 품종과 그 품종의 모든 이미지들，
                                                            이 두 개의 딕셔너리
                  dictionary로 조직한다. 이제 각 딕셔너리는 아래의 포맷으로（그교iuahua 이미지를 포함

                  한다．

                  training_dataset{"n02085620-Chihuahua"] = ["n02085620_10131. jpg", .. .]


                  품종들 을 이러한 딕셔너리로 구성하는 것은 각 형태의 이미지를 선택하거나 나누는 과
                  정을 간단하게 해준다. 전처리 동안모든 이미지들이 반복적으로 사용되고, 각 이미지들
                  은 리스트에 있는 파일 이름에따라 열린다．


def write_records-file(dataset, record_location) :


    Fill a TFRecords file with the images -Found in 'dataset ' and include their category.
    Parameters


    dataset : dict(list)
          Dictionary with each key being a label -For the list of image filenames of
its value.




  204 -   CHAPTER 6 물체 인식 및 분류


===== PAGE 216 =====
    record location : str
        Location to store the TFRecord output.


    writer = None


   # Enumerating the dataset because the current index is used to breakup the fiLes
1f they get over 100
   # images to avoid α 뵤owdown in writing.
    current index == 0
    for breed, images_filenames in dataset.itemsQ:
        for image_filename in images_filenames:
            if current index % 100 == 0:
                if writer:
                       writer.close()


                record_filename = "{record_location}-{current-index}.tfrecords' .format(
record_location=record_location, current_index=current-index)


                writer = tf . python_io.TFRecordWriter(record_filename)
                current index += i


                image_file = tf . read_file(image_filename)
                # In ImageNet dogs, there are α few images which TensorFLow doesn 't
recognize as JPE65. Thi5
                # tryIcatch wiLL ignore those images.
                try:
                       image = tf . image .decode_jpeg(image_file)
                except:
                    print (image_filename)
                       continue


                # Converting to grayscaLe saves processing and memory but isn't
required.
                grayscale_image = tf. image. rgb_to_grayscale(image)
                resized_image = tf. image.resize_images(grayscale_image, 250, 151)




                                                                          CNN 구현   - 205


===== PAGE 217 =====
                    # tf.cast is used here because the resized images are floats but
haven't been converted into
                    # image floats where an RGB vaLue is between r9,1工
                    image_bytes = sess .run(tf. cast(resized_image, tf. uint8)) .tobytes()


                    # Instead of using the LabeL as α string, it 'd be more efficient to
turn it into either an
                    # integer index or α one-hot encoded rank one tensor.
                    # https:1/en. wikipedia.org/wiki/One-hot
                    image_label = breed.encode( "utf-8")


                    example =
                    tf . train.Example(features=t-F . train.Features(feature={ ' label' :
                    tf. train.Feature(bytes_list=tf. train.BytesList(value=
             [image_label])), ' image' :
                    tf. train.Feature(bytes-list=tf. train.BytesList(value=[image-bytes]))
             }) )

                    writer .write(example . SerializeloStringQ)
    writer .close 0


write_records_file(testing_dataset, "./output/testing-images/testing-image")


write_records_file(training_dataset, "./output/trainingimages/training-iniage")


               이 예제 코드는 각 이미지를 열고, 그레이스케일로 변환하고, 이를 TFRecord 파일에 추
               가한다. 전체적인 로직은 앞의 예와동일하다. 다만tf.image. resize_images를사용
               한다는 점만 다르다. 영상의 크기를 맞추는 작업으로 인해서 영상이 조금 왜곡distortion
               될 수는 있다. 예를 들어서 세로 방향으로 긴 이미지와 가로 방향으로 긴 이미지가 모두
               이 코드로 크기가 맞춰진다면, 가로 방향으로 긴 이미지는 왜곡될 수 있다. 이러한 왜곡

               은 tf. image. resize_images가 이미지의 가로 세로 비율을 고려하지 않기 때문이다．
               조금 더 정확하게 이미지의 크기를 맞추려면 이미지의 외곽을잘라내거나cropping, 필요

               한부분에 덧붙이는padding 작업이 필요할수도 있다．



 206 -   CHAPTER 6 물체 인식 및 분류


===== PAGE 218 =====
이미지 불러오기

데이터가TFRecord 형식으로 준비되어있기 때문에 JPEG 이미지 대신 TFRecord로 읽
어들이면 된다. 아래는 이미지 몇 개와 레이블값을동시에 입력 받는다．


filename_queue = tf. train. string_input_producer
(tf. train.match_filenames_once( " ./output/training-images/*.tfrecords"))
reader = tf. TFRecordReader()
_, serialized = reader.read(filename_queue)


features = tf. parse_single_example(
     serialized,
     features={
         'label' : tf. FixedLenFeature([], tf. string),
         'image' : tf. FixedLenFeature([], tf. string),
    })

record_image = tf. decode_raw(features[ 'image '], tf. uint8)


# Changing the image into this shape heLps train and visuaLize the output by
converting it to
# be organized Ltke an imαge.
 image = tf. reshape(record_image, [258, 151, 1])


label = tf. cast(features[ ' label'], t-f.string)
min_after_dequeue = 18
batch size = 3
capacity = min_a-fter_dequeue + 3 * batch_size
 image_batch, label_batch = tf. train.shuffle_batch([image, label], batch_size=
batch_size, capacity=capacity, min_after_dequeue=min_after_dequeue)



이 예제 코드는 학습 디렉터리에 있는 모든 TFRecord 파일을 사용함으로써 학습 이
미지들을 로드한다. 각TFRecord는 여러 개의 이미지를 포함하고 있지만 tf . parse_
single_example은 하나의 이미지만 사용한다. 이전에 소개된 배치 오퍼레이션은 여




                                                                        CNN 구현    - 207


===== PAGE 219 =====
               러 이미지를동시에 학습시킬 때 사용된다. 이러한오퍼레이션들은 여러 이미지를하나
               의 이미지처럼 동작하도록 만들어졌기 때문에 여러 이미지를 배치 처리하는 것이 효과
               적이다. 이를 위해서는 시스템의 메모리가 충분해야 한다．

              메모리에 이미지를두고, 이제 학습과 테스트를 위한모델을만들어야한다．



              모델

              사용하는 모델은 텐서플로우에서 회귀 신경망convoLutionaL neuraL network을 설명하는 튜
                                                           이 모델의 구조가
               토리얼에 자주 사용되는 mnist convolution example과 유사하다．
               간단하기는 하지만, 영상 분류와 인식에 사용되는 다양한 기법들을 설명하기에는 충
               분하다. 조금 더 진보된 모델은 더 많은 컨볼루션 레이어를 가지는 /\Iex Krizhevsky's
               P;exNe'에서 참고하자．


# Converting the images to α float of r0,1) to match the expected input to convoLutLon2d
float_image_batch = tf. image. convert_image_dtype(image_batch, tf. f10at32)


conv2d_layer_one = tf. contrib. layers. convolution2d( float_image_batch,
    num_output_channels=32, # The number af fiLters to generate
    kernel_size=(5, 5), # It 's onLy the βLterheight and vrLdth.
    activation_-Fn=t-F. nn. relu,
    weight_init=t-F. random_normal,
    stride=(2, 2),
    trainable=True)
    pool_layer_one = t-F.nn.max_pool(conv2d_layer_one, ksize=[l, 2, 2, 1],
strides=[l, 2, 2, 1], padding= 'SAME')


# Note, the first and Last 《九mension 0f the convoLution output hasn忙 changed but the
# middLe hvo dtmen5t아구5 hαVe.
conv2d_layer_one. get_shape(), pool_layer_one. get_shape()




  208 -   CHAPTER6 물체 인식 및 분류


===== PAGE 220 =====
출력은다음과같다：


 (TensorShape([Dimension(3), Dimension(125), Dimension(76), Dimension(32)]),
 TensorShape([Dimension(3), Dimension(63), Dimension(38), Dimension(32)]))



이 모델의 첫 번째 레이어는 tf. cont rib,layers. convolution2d로 생성한다．
weight_mnit는 random_normal로 세팅된다는 점이 중요하다. 이것은 첫 번째 필터

셋이 稍予분포normaL distribution를 따르는 랜덤값으로 채워진다는 점이다
                                              （이 파라미터
는 TensorFiow 0.9에서는 weights_initialize
                                     「로 이름이 변경되었다）
                                                 . 필터들은
trainable로 정해져서 네트워크에 정보를 입력하면서 모델의 정확도를 향상시키기 위
해서 조절된다．

이미지에 건볼루션이 적용된 후에, 출력은 max_pool 오퍼레이션으로 크기를 축소한다．
그 오퍼레이션 이후에는 건볼루션의 출력 결과가 반으로 줄어드는데, 이것은 풀링에서

사용되는 size와 strides의 영향이다．
                        출력 크기의 축소가 필터
                                    （출력 채널）
                                          들의 개수나
이미지 배치의 개수를 변경하는 것은 아니다. 줄어드는 것은 이미지
                                   （필터）
                                      의 높이와폭
이다．


 conv2d_layer_two = t-F. contrib. layers. convolution2d(pool_layer_one,
      num_output_channels=64, # More output channeLs means an increase in the number
 0f /7Lters
     kernel_size=(5, 5),
     activation_-Fn=tf. nn. relu,
     weight_init=tf. random-normal,
     stride=(1, 1),
     trainable=True)


 pool_layer_two = t-F.nn.max_pool(conv2d_layer_two, ksize={1, 2, 2, 1], strides=[1, 2,
 2, 1], padding='SNE')


 conv2d_layer_two.get_shapeQ, pool_layer_two.get_shape()




                                                                          CNN 구현   - 209


===== PAGE 221 =====
             이 코드의 출력은：


(TensorShape([Dimension(3), Dimension(63), Dimension(38), Diniension(64)]),
TensorShape([Dimension(3), Dimension(32), Dimension(19), Dimension(64)]))



             두 번째 레이어는 필터들의 깊이를 제외하고는 첫 번째에 비해 약간만 변경되었다. 필터
             들의 개수는두 배가 되고，
                          이미지의 높이와폭은또 다시 줄어든다. 여러 번의 컨볼루션
             과풀 레이어가 깊이는더하면서 입력의 높이와폭을줄이기 위해서 반복된다．

             여기서 더 많은 컨볼루션과풀링 단계가수행될수도 있다. 많은 구조들에서는 5개 이상
             의 다양한 컨볼루션과풀링 레이어가 있다. 가장발전된구조들은 더 많이 사용함으로써
             학습과 디버깅에 시간이 많이 소요되기는 하지만, 더욱복잡한 패턴들을매칭할수 있게
             된다. 이 예제에서, 두 개의 컨볼루션과풀링 레이어들은 전체적인메커니즘을 설명하기
             에충분하다．

             작업을수행하는 텐서는 여전히 꽤나복잡한텐서이다. 다음단계는 이미지의 모든 점을
             출력 뉴런에 모두 완전 연결fully-connected하는 것이다．
                                                 이 예제는 나중에softmax를 사
             용하기 때문에 완전 연결된 레이어는 랭크가2인 텐서로 변경되어야 한다. 텐서의 첫 번
             째 차원은 각 이미지를 구별하기 위해서 사용되고，
                                       두 번째 차원은 각 입력 텐서의 랭크
             1텐서이다．

              flattened_layer_two = tf. reshape(
                  pool_layer_two,
                  [
                       batch_size, # Each image in the image_batch
                       -l           # Every other dimension of the input
                  ])
              flattened_layer_two. get_shape()




 21미 대APTER 6 물체 인식 및 분류


===== PAGE 222 =====
출력은아래와같다：


TensorShape([Dimension(3), Dimension(38912)])


tf. reshape은남은 모든차원을 사용하기 위해 사용될 수 있는특별한 값이다. 이 예제
코드에서 -1은 마지막 풀링 레이어를 거대한 하나의 랭크 1 텐서로 변경「eshape하기 위
해 사용된다. 풀링 레이어를 통해서 현재의 네트워크의 상태를 개 품종 예측에 연결하는
두 개의 완전 연결 레이어와 결합될 수 있다．


# The weight_mnit parameter can aLso accept α caLLabLe, α Lambda is used here
returning α truncated normaL
# i,iith α stddev specified.
hidden_layer_three = tf. contrib. layers.fully_connected(
     flattened_layer_two,
     512,
     weight_init=lambda i, dtype: tf. truncated_normal([38912, 512], stddev=0.1),
     activation fn=tf. nn. relu
 )

# Dropout some （〕
                f the neurons, reducing their importance in the modeL
hidden_layer_three = tf. nn.dropout(hidden_layer_three, 0.1)


# The output of this are aLL the connections between the previous Layers and the
120 different dog breeds
# αVαiLab{,e t0 trαtn 0n.
final_fully_connected = tf. contrib. layers.fully_connected(
     hidden_layer_three,
     120, # Number （〕
                    f dog breeds in the ImageNet Dogs dataset
     weight_init=lambda i, dtype: tf. truncated_normal([512,120], stddev=0.1)
 )

이 예제는 모든 픽셀이 모드 개 품종에 연결되는 마지막의 완전 연결 레이어를 만든다．
이 네트워크의 모든 단계는 모든 이미지를 필터들로 변환함으로써 입력 이미지의 크기




                                                                       CNN 구현       - 211


===== PAGE 223 =====
              를 줄이고，
                   개 품종
                      （레이블）
                          과 매칭시킨다．
                                 이런 기법은 출력을 일반화generaLize하면서
              학습과 테스트 과정에 처리 능력을줄여준다．



              학습

              이제 모델을 학습시킬 차례이다. 이 마지막단계는 이 책의 앞 장에서 소개된 것과 동일
              한 과정을 따른다. 각 층의 웨이트를 업데이트하는 학습기에 학습 이미지를 입력한 후，
              네트워크의 결과가 얼마나 정확한지에 따라모델의 손실을 계산한다. 이 과정은각단계
              의 정확도를향상 시키면서 한 번에 한 과정iteration씩 반복한다．

                                                （tf.nn. softmax）
              이 모델에서 중요한 점은, 학습 과정 동안 대부분의 분류 함수들              은

              숫자로 된 레이블을 필요로 한다는 점이다. 이것은 TFRecords에서 이미지를 불러오
              는 부분에서 강조했었다. 각 레이블은 n02085620-Chihuahua와 유사한 문자열이다．
              tf. nfl. softmax에서 이 문자열을 사용하는 대신, 각 레이블마다 고유의 숫자로 바꿔야

              한다. 이러한 변환작업은 전치리 단계에서 수행되어야 한다．

              이 데이터셋에서 각 레이블은 모든 개의 품종을 포함하는 리스트에서 각 이름들의 인
              덱스를 의미하는 숫자로 바꾼다. 다양한 방법으로 처리할 수 있지만, 이 예제에서는
              tf . map_fn이라는 새로운 텐서플로우 오퍼레이션을 사용해보자．


import glob


# Find every directory name in the imagenet-dogs directory(n02085620-Chihuahua, . . .)
labels = list (map(lambda C: c.split( "/")[-l], g1ob.glob(". /imagenet-dogs/*")))


# Match every LabeL from LabeL_batch and return the LndexL. 'here they exist in the
Lt5tof cLasses
train_labels = tF.map_fn(lambda 1: tf. where(t-F.equal(labels,l) )[0,0:l][0],
label_batch, dtype=tf. int64)




 212 -   애APTER 6 물체 인식 및 분류


===== PAGE 224 =====
이 예제 코드는2개의 다른 형태의 map 오퍼레이션을사용한다．
                                 첫 번째는 디렉터리의
리스트에 있는 개 품종 이름의 리스트를 만든다. 두 번째는 그래프에서 텐서에 함수를
맵핑하는텐서플로우오퍼레이션인tf.map_fn이다. 이것은정수 인덱스만을포함하는
랭크1인텐서를생성하는데, 각레이블은모든클쾌스 레이블의 리스트에 위치한다. 이
러한고유의 정수값들은 tF.nn. softmax와같은 함수에서 사용할수 있다．



텐서보드로 필터 디버깅하기

CNN은 학습 동안에 정확도를 떨어뜨릴 수 있는 여러 움직이는 부분들이 있다. CNN
에서 디버깅 문제는반복과정 중에 필터filte叩｀ernel) 들이 어떻게 변화하는지를 조사하
는 것에서 시작한다. 필터에서 사용되는 각 웨이트들은 네트워크가 학습방법에 따라서
가장 정확한 웨이트 세트를 학습하려고 시도하면서 계속적으로 변경된다．

잘 설계된 CNN에서는 첫 번째 컨볼루션 레이어가 작동할때, 초기화된 입력 웨이트들
은 랜덤한값으로 정해진다
            （이 예에서는weight_init=tf. random_normal). 이 웨이
트들이 이미지 위에서 작동하면서 활성화 값
                      （피처맵feature map）
                                     도 랜덤한 값이 된다．
                                                피
처맵을 이미지와 같은 형식으로 출력하면, 그 출력값은 입력 이미지에 잡음이 추가된
것 처럼 보인다. 이 잡음은 랜덤한 웨이트 때문이다. 여러 번반복 과정을 거치면서 각
필터는 점점 균일화uniform되는데, 웨이트가 학습 과정에서 조절되기 때문이다. 네트
워크가 수렴함에 따라 필터들은 이미지에서 발견될 수 있는 각각의 작은 패턴을 닮아
가게된다.




                                                     CNN구현   - 213


===== PAGE 225 =====
                               0




                              5o




                             100




                             150




                             200




                               0   20 40   60   80 100 120 140




                첫 번째 컨볼루션 레이어를 통과하기 전인 원래의 그레이스케일 입력 이미지




                               0   10   20 30   40   50   a〕 70




                   출력의 랜덤성을 보여주는 첫 번째 컨볼루션 레이어의 출력 피처맵




2141   CHAPTER6 물체 인식 및 분류


===== PAGE 226 =====
CNN을 디버깅하는 과정에서 이러한 필터들에 익숙해져：畦한다. 현재 텐서플로우에는
필터나피처맵을출력ㅎH三내장함수는없떳f. image_su끄쁘y를 " 陪해서생성된
피처맵이나학습된 필터들을볼수 있다. 그래프에 이미지 요약출력을추가하면사용하
는 필터들과 이 필터들을 입력 이미지에 적용해서 생성되는 피처맵의 개괄을 살펴보는
데도움된다．

지금 진행되고 있는 TensorDebugger라는jupyter notebook extension은 현재 개발
초기 단계이다．
       이 익스텐션extension은반복 과정 중에 필터들을 애니메이션 gif 파일로
변화하는 과정을볼수 있도록 해준다．




계속 진행

CNN은 텐서플로우에서 약간의 코드로 구현할 수 있는 아주 유용한 네트워크이다. 이
미지를 염두에 두고 만들어진 것이기는 하지만, CNN은 이미지 입력만 사용할수 있는
것은아니다. 컨볼루션은음악, 의학등에서도사용되고 있다. 그래서 CNN도유사한방
법으로 적용될 수 있다. 현재 텐서플로우는 2차원 컨볼루션이지만, 텐서플로우를 이용
해서 더 고차원 입력에도 적용할수 있다．

CNN은 이론적으로는 자연어 데이터text에도 적용할수 있다. 텍스트 입력은 보통 다수
                            CNN은모든 입력이 중요하고다수의 입력
의 입력값이 0인 Sparselensor에 저장된다．
                                       텍스트 데이터에 적용
이 0이 아닌 소밀한 입력dense input에 동작하도록 디자인되었다．
하는것은다음장 "Recurrent Neural Networks and Natural language Processing"
에서 살펴보자．




                                                                 계속 진행   - 215


===== PAGE 227 =====
                      놔
회귀 신경망과 자연 언어


              唾
(Recurrent Neural Networks and




                              發蚣
      Natural Language)


                                   漆莎
                      照mM瞰界
    d         自
                                       ＝辦卜
    r
    菲的            兮
        L
        ,
        〃

                                      〃 1 h`
                                    .last
                                       .-.
       ant。
          U




       必
                         0


===== PAGE 228 =====
     이전 장에서 우리는 정적인 이미지를 분류하는 방법을 배웠다. 이 분야는 머신 러닝의
     커다란 응용 분야이다. 그러나 다른 분야들도 많다. 이 장에서 우리는 연속적인 모델
                             이러한모델들은 연속적인 입력을분류하거나，
     sequential mode〔을살펴볼 것이다．                    문자열
     을출력하거나，
           하나의 입력 시퀀스를다른 것으로번역translate하는등의 일을할수 있다．

     여기서 다루는 내용들이 정적인 분류, 회귀 분석 등과다르지 않다. 대신 회귀 신경망은
     완전 연결된 그리고 컨볼루션레이어의툴 키트와작동하는빌딩 블록을 제공한다．




     회귀 신경망 소개



     우리는 시간적인 세계에 살고 있다．

     많은 실 세계의 문제들은 속성상 연속적sequentia［이다．자연어 처리natural language
     processing: NLP도동일하다．          문장은단어들의 연속이며，
                         문단은문장의 연속이고，           단어는
     글자들의 연속이다. 이와유사하게 오디오나 비디오 클립도 시간에 따라 변하는 프레임
     들의 연속이다. 심지어 주식 시장의 가격들도 시간에 따라서 분석될때에 의미가 있다．

     이러한모든분야에서 관측observation의 순서가중요하다. 예를들어, "I had cleaned
                                                  당신이 누군가를 시켜
     my car" 라는 문장을 " I had my car cleaned" 라고 바꾸면，
     서 일을 시킨 것이 된다. 이러한 시간적인 의존성은 여러 단어가 아주 유사한 발음을
     공유하는구어spoken language에서 더 심해진다．   "wreck a nice beach" 는
                                   예를들어，
                               단어들은 문맥에 따라서 만이 인식될 수 있기 때문
     "recognize speech" 처럼 들리는데，
     이다．

     이런 관점에서 당신이 αonvnets을 포함하는 피드포워드 신경망을 생각하고 있다면, 그
     신경망은 아주 제한적이다. 그러한 신경망은 reflex와 같은 하나의 포워딩을 통해서 입
     력값을 처리한다. 이러한 신경망은 모든 입력이 독립적이라고 간주한다. 동일한 길이의
     입력을 패딩하여서 신경망에 전체 시퀀스를 입력하는방법도 있지만, 이방법은 연속이




CHAPTER 7 회귀 신경망과 자연 언어
                      （Recurrent Neural Networks and Natural Language)


===== PAGE 229 =====
라는속성을잘사용하지는못한다．

회귀 신경망Recurrent NeuraL Network: RNN은 명시적으로 시간을 모델링하는 신경망이다．
RNN은다른뉴런으로부터 입력들의 가중합을 계산하는동일한뉴런을사용한다. 그러
나뉴런들은다음 단계의 레이어로 연결되거나, 이전 레이어로 연결되거나사이클을 형
성할수도 있다. 신경망의 히든 액티베이션hidden activation들은 같은 시퀀스의 입력 사이
에서 기억된다．

RNN의 많은 변종들이 1980년대 이후에 제안되었지만 계산 성능의 부족과 학습의 어
려움으로 인해서 최근까지 널리 사용되지 못했다. 그러나2006년에 LSTM과 같은 구조
의 발명으로 이제 RNN의 아주 좋은사용 예가 되었다. 이들은많은분야에서 연속적인
작업에 잘동작하고 있는데, 예를들어 음성 인식, 음성 합성, 연속문자 인식, 일기 예보，
이미지 캡션 생성, 기계 번역 등의 분야가 이에 해당한다．

이 장의 다음 섹션에서 RNN을 깊이 살펴보고, 최적화하는방법과 이를 위해 필요한 수
학적인 배경 지식을 배워보자. 그런 후에 하나씩 단점들을 해결한RNN의 변형들을 소
개한다. 이를바탕으로 4개의 자연어 처리 작업을수행하기 위해서 RNN을사용하는데，
데이터정리작업,모델디자인,구현,그리고텐서플로우를이용한학습과정을다룬다．



임의의 프로그램을 학습하기

RNN을 직관적으로 먼저 이해해보자. 이전에 소개된 피드 포워드 신경망은 고정된 크
기의 벡터에 동작한다. 예를들어, 28 x 28 픽셀 이미지를 10개의 가능한클래스들의 확
률로맵핑한다. 계산은 고정된 횟수의단계
                    （레이어의 개수）
                            로수행된다. 반대로，
                                      회귀 신
경망은 가변적인 길이의 벡터 시퀀스
                  （입력, 출력 또는모두）
                              에 동작한다．

RNN는 기본적으로는 임의의 방향으로 연결된뉴런과 웨이트의 방향성 그래프이다. 그
러나 입력 데이터에 의해서 활성화되는 입력 뉴런은 입력과 연결되고，
                                    출력 뉴런은 인식
된 결과를 읽는 미리 지정된 뉴런의 집합이다. 그래프에서의 다른 모든 뉴런들은 은닉
뉴런hidden neuron이라고 한다．




                                                    회귀 신경망소개   - 219


===== PAGE 230 =====
                                             OE
                                             ○〈
                                             Q＜三

                             피드 포워드 신경망과 회귀 신경망



     RNN의 연산은 일반적인 신경망과유사하다. 각 단계에서 신경망에게 입력 시퀀스의
     다음 프레임을 입력한다. 그러나 포워드 신경망과다르게 은닉 뉴런의 결과를 버리지 않
     는다. 그것들을 다음 단계의 뉴런에 입력으로 사용될수 있기 때문이다. 현재의 히든 액
     티베이션hidden activation을상태state라고 한다．
                                       각시퀀스의 시작부분에서，
                                                   빈상태empty
     state,즉0에서 시작한다．



               mH
                           Short Notation of FFNN and RNN


     RNN의 상태는 현재의 입력과 이전상태
                         （차례로 이전의 입력과상태에 의존한다）
                                             에따
     라달라진다. 그렇기 때문에 상태는 모든 이전의 입력 시퀀스에 간접적으로 접근하고 있
     고，
      작업 메모리working memory라고생각할수 있다．

     컴퓨터 프로그램에 비유해서 설명해보자. 사람이 쓴 글씨를 이미지로 입력받아서 인식
                                  조건문들을 사용해서 만들 수도 있
     하려고 한다. 이 문제를 파이썬 언어로 변수, 반복문，
     다. 이렇게 직접만들어도 된다. 그렇지만안정적인 인식률을 얻기는 쉽지 않을 것이다．

     이에 비해서 RNN은 예제 데이터로 학습시킬 수 있다는 점이 좋은 점이다. 변수에 중간
     결과를 저장하는 것처럼,RNN은중간 결과를상태state로 저장한다. RNN의 웨이트매




CHAPTER 7 회귀 신경망과 자연 언어
                      （Recurrent Neural Networks and Natural Language)


===== PAGE 231 =====
트릭스는수행하고자하는프로그램을 정의하는셈이다. 이것은 히든 액티베이션에 어
떤 입력을 저장할지, 액티베이션을 새로운 액티베이션과 출력으로 결합하는 방법 등을
의미한다．

실제로 시그모이드 활성화함수를 가진RNN은 2006년에 Schafer과Zimmermann에
                            적당한 웨이트가주어진다면 어떠한 계산
의해서 Turing-complete라고 증명되었으며，
가능한문제도 계산할수 있다는 의미이다. 이것은 이론척인 특성이기는하다. 즉，
                                         각업
무에 적합한완벽한 웨이트를찾을수 있는방법이 없기 때문이다．

RNN을 최적화하는 복잡한 내용 이전에 파이썬 프로그램을 작성할 수 있다면 왜 우리
가RNN을 필요로 하는지에 대한답을 해보자. 가능한 웨이트 매트리스 공간이 가능한
C 프로그램의 공간보다자동으로탐색하기 훨씬 쉽기 때문이다．



시간에 따른 역전파
         （Backpropagation)

이제 RNN이 무엇이고，
            왜 좋은지를 알고 있으니까，
                          좋은 웨이트매트릭스를찾는방법，
즉 웨이트를 최적화하는 방법을 알아보자. 포워드 네트워크에서 가장 대중적인 최적화
방법은 기울기 하강법을 이용하는 방법이다. 그러나 이와 같은 다이나믹 시스템에서는
에러를 역전파하는방법이 쉽지 않다．




               회귀 신경망을 시간에 따라 펼치기


RNN을 최적화하는 기법은 최적화하기 위해서 시간에 따라서 RNN을 펼쳐서 포워딩
신경망을 최적화하는 것과동일한방법을 사용한다. 길이 10인 시퀀스를 사용하는 경우




                                             회귀 신경망소개 口21


===== PAGE 232 =====
     를 보자. 히든 뉴런을10번복사해서 그들사이를 연결해서 펼치면 된다. 이를통해서 계

     산과정의 의미를 변경하지 않고 회귀 연결
                          「ecurrent connection흘 없앤다. 이로써 포워드
     신경망이 되기 때문에 각타임 스텝 사이의 연결 웨이트가같은 연결 강도로 연결된다．




                                          w,
                                                 wh
                                                       밋-         wh




                                    RNN을 시간에 따라서 펼치기



     이제 웨이트에 대해서 에러의 기울기를 계산하기 위해서 펼쳐진RNN에서 표준 역전파
     알고리즘을 적용할수 있다．
                  이 알고리즘을Back-Propagation Through Time(BPTT)
     라고 한다. 이는 서로 연결된 것들을 포함해서 시간에 따른 각 웨이트의 도함수derivative
     를 제공해준다. 연결된 웨이트를 같은 값으로 유지하기 위해서, 각 기울기를 합해서 사
     용한다. 이런방법은 컨볼루션 필터의 경우와동일하다．

               Sequence             Sequence          Sequence         Sequence
              Classification        Generation        Labelling        Translation



                               i棉      ＇
                               회귀 신경망에서의 일반적인 맵핑




     우리의 첫 번째 순환 신경망 만들기

     이제까지 배운 것을 구현해보자. 텐서플로우는 다양한 종류의 RNN을 제공하는데
     tensorfiow. models. mnn. mnn-cell 모듈에서 찾을수 있다. tensorflow.model. mnn




CHAPTER 7 회귀 신경망과 자연 언어(Recurrent Neural Networks and Natural Language)


===== PAGE 233 =====
에서의 mn 오퍼레이션으로 텐서플로우는 우리를 위해서 시간에 따른 RNN 펼침을 수

행한다. 우리가 입력 시퀀스에 대한 각 타임 스텝에 대한 텐서들의 리스트를 제공하면，
RNN이 이 함수를 수행한다. RNN은 펼쳐진 계산 그래프의 계산을 수행하고 출력과각
타임 스텝에서의 히든 스테이트를 가지는 텐서들의 리스트를 반환한다．


import tensor-flow as tf
from tensorflow.models.rnn import mnn_cell
from tensorflow.models.rnn import mnn


# The input data has dimensions batch_size * sequence_Length * frame_sLze.
# To not restrict ourseLves to α fixed batch size, we use None as size of
# the first dimension.
 sequence_length
frame size = . .
data = tf. placeholder(tf. fl0at32, [None, sequence_length,-Frame_size])


num neurons = 200
network = mnn_cell. BasicRNNCell(num_neurons)


# UnfoLd the network in time fOr sequence_Length time steps.Since we do not
# provide initiaL states to the function here, we have to manuaL勻／ speci力／ the
# data type of the neurons.
outputs, states = rnn(network, unpack_sequence(data),dtype=tf. float32)
output = pack_sequence(outputs)
state = pack_sequence(states)


텐서플로우는 원래의 파이썬 리스트를사용한다. 시퀀스 데이터, 출력, 스테이트state들

을 하나의 텐서로 만들려고 한다. 우리는 하나의 텐서를 첫 번째 축을 따르는 텐서들의
리스트로 나누기 위해서 tf. unpack( ）를 사용한다. 시간 단계에 따라 나누기 위해서，

우리는 미리 데이터 텐서의 전치transpose 행렬을구한다. 이와유사하게 tf. pack( ）은
텐서들의 리스트를 하나의 큰 텐서로 합쳐준다. 우리는 입력과 동일한 형식으로 만들기

위해서 전치 행렬을구한다．




                                                                   회귀 신경망 소개   - 223


===== PAGE 234 =====
def unpack_sequence(tensor):
    "Split the single tensor of a sequence into a list of frames."
    return t-f.unpack(tf.transpose(tensor, perm={l, 0, 2]))


def pack_sequence(sequence):
    "Combine a list of the frames into a single tensor of the sequence."
    return t-f.transpose(tf.pack(sequence), perm=[l, 0, 2])




                                 ○篒
                                 O篒
                                  ○＜
                                             출력을 표시한 RNN


               이제 RNN이 있고 시간축으로 펼쳐져 있기 때문에, 데이터를 로드하고 tf. train.
               RMSPropOptimizer나 tf. train.AdamOptimize
                                                      「와 같은 텐서플로우의 최적화 함수
               를 사용해서 신경망을학습시킬 수 있다. 이 장의 후반부에 예제를살펴볼 것이다．

                  ·   dynamic m1n
                  ·   Variable sequence lengths


               사라지거나 폭발하는 기울기

               마지막 섹션에서 】NN을 정의하고 에러를 역전파하고 기울기 하강법을 적용하기 위해
               서 시간축으로 펼쳤었다. 그러나 이 모델은 그렇게 잘 작동하지 않을수 있다. 예를 들어
               NLP와 같은 입력 프레임 사이의 장기간thng-term의 의존 관계dependency를 잘 파악하지
               못할수 있기 때문이다．




  224 -   CHAPTER7 회귀 신경망과 자연 언어
                               （Recurrent Neural Networks and Natural Language)


===== PAGE 235 =====
아래는 RNN이 입력 시퀀스가 주어진 문법에 맞는 지 틀린 지를 구별해야 하는 장기간
의 의존 관계를 포함하는 문제이다. 이 작업을 수행하기 위해서 신경망은 그 시퀀스의
첫 번째 프레임과 그 이후의 관련 없는 많은 프레임들을 모두 기억해야 한다. 왜 이것이
지금껏 우리가 보아온 전통적인RNN의문제일까？




                        장기간 의존관계를 가지는 문법



RNN이 그러한 장기간의 의존성을 학습하기 힘든 이유는 최적화하는 동안에 신경망
을통해서 에러가 어떻게 전파되는 지에 담겨있다. 기울기를 계산하기 위해서 펼쳐진
RNN을 통해서 에러가 전파된다는 점을 기억하자. 긴 시퀀스를 위해서 펼쳐진 신경망
은매우 깊어진다. 따라서 많은 레이어를 가지게 된다. 각 레이어마다 역전파 알고리즘
은 신경망의상위레이어에서 에러의 크기를지역 미분값에 의해서 조절한다．

대부분의 지역 미분값은 1보다 아주 작기 때문에, 기울기는 모든 레이어에서 작아지는
데 지수적exponentially으로 작아지며 결국에서 없어지게vanish된다．이와유사하게, 1보다
큰많은 지역 미분값들은 기울기가폭발expLode
                         （아주 커지게）
                                하게 된다．

이 문제를 쉽게 이해하기 위해서, 레이어에 하나의 히든 뉴런이 있는 예를 통해서 기울

기를계산해보자．
       각레이어＇에대해서지역미분값 /'(in1) * Wf은서로곱해진다．



    3C = 흐으* 츠n3* 쓰'2:= ac 面"i3 * am3 0ut2 * a""2 坐스
   am, 1   am刃3   "2    'a"h   aout3 aub     out2 131712   130Ut1 ifl "

   = cost'(f(out3)) * f '(1n3) * W ' * f '(in2) * W ' * f '(in1)




                                                                          회귀 신경망소개   - 225


===== PAGE 236 =====
                              딥 신경망에서 불안정한 기울기



     이 문제는 순환 신경망 이외에 실제로다른 어떤딥 신경망에도 존재한다. 그러나RNN
     에서는타임 스텝 사이의 연결이 각각 연결되어 있기 때문에, 각 웨이트의 지역 미분값
     이 1보다 모두작거나 또는모두 커서 기울기가 언제나 같은방향으로 조절된다. 그래서
     기울기 값이 사라지거나폭발하는문제가포워드 신경망보다 더욱극명하게 발생한다．

     아주작거나큰 기울기와관련된문제가 몇 가지 더 있다. 0이나무한대에 가까운 기울기
     값은 학습이 각각 지연되거나 발산한다. 더군다나 수치적으로 최적화하고 있기 때문에
     부동소수점의 정밀도가 기울기를 왜곡하게 된다. '딥러닝의 근본적인 문제'로 알려진
     이 문제는 지난 수년 동안많은 연구자들에 의해서 연구되어 왔다. 가장 유명한 해결책
                                           이라고 불리는RNN 구
     은다음섹션에서 살펴볼Long-Short Term Memory(LSTM）
     조이다．



     Long-Short Term Memory

     1997년에 Hochreiter와 Schmidhuber에 의해 제안된 LSTM은 기울기가 사라지거나
     폭발하는 문제를 극복하기 위해서 특별히 제안된RNN 구조이다. 장기간의 의존 관계
     를학습하는데 뚜렷이 향상된능력이 있고 현재 사실상의 RNN의 표준이 되었다. 그 이
     후에 LSTM의 여러 변종들이 제안되었고 텐서플로우에도 구현되어 있다. 이 섹션에서
     살펴보자．

     사라지거나폭발하는 기울기의 문제를극복하기 위해서, LSTM 구조는RNN의 일반적
     인뉴런들을 내부에 작은 메모리를 가진 LSTM 셀ce1로 교체한다. 이 셀들은 일반적인
     RNN과같이 연결되어 있어서, 내부의 상태가 여러 스텝에 걸친 에러를 기억하는 것을
     돕는다．




CHAPTER 7 朝닉 신경망과 자연 언어
                      （Recurrent Neural Networks and Natural Language)


===== PAGE 237 =====
LSTM의 트릭은 이 내부 상태가1로 고정된 웨이트와 선형 활성화함수와 연결되어 있
어서, 지역 미분값은 언제나1이다. 역전파동안, 이것은상수 에러 회전목마constant error
carouse〔라고불리는데, 기울기가사라지거나폭발하지 않고 여러 스텝동안 에러를 전송
할수 있다．


         톼= f '(in) * w * et+ 1 = 1.0

내부 상태의 목적이 여러 타임 스텝에 걸친 에러를 전송하는 것인 반면, LSTM 구조는
비 선형
   （일반적으로 시그모이드）활성화함수를 가지는 주변의 게이트surrounding gates
에게 학습을 위임한다. 원래의 LSTM 셀에서는 2개의 게이트가 있다. 하나는 들어오는
액티베이션을스케일하는 것을학습하고, 다른 하나는 나가는 액티베이션을스케일하
는 것을 학습한다. 그래서 셀은 언제 새로운 입력을 벋아들일지 아니면 무시할지를, 그
리고 언제 자신이 표현하는 특징값을다른 셀들쩨게 줄지를학습한다. 셀로의 입력은 개
별적인 웨이트를 이용해서 모든 게이트 속으로 주어진다．

순환 신경망을 레이어들로 생각할 수 있다. 왜냐하면순환 신경망을 더 큰 구조의 한부
분으로 사용할수 있기 때문이다. 예를들어, 처음에는 여러 개의 컨볼루션과풀링 레이
어를 이용해서 몇 단계를 거치고, 그 다음에 이것들의 출력을 LSTM 레이어로 처리하
고,마지막단계에서 LSTM의 가장상단에 소프트맥스 레이어를더하는 것이다．

            녹 * 괏


                    Output Gate

                    Output
                    Non'inearity




                    Input Gate
                    Input
                    Nonlinearity

            / - \
                                             「口
                         Long Short-Ternㄱ 메모리
                                            （LSTM)




                                                     회귀 신경망소개   - 227


===== PAGE 238 =====
     텐서플로우는 그런 LSTM 네트워크에 BasicRNNCe11을 교체할 수 있고 ，부가적인 스
     위치를 제공하는 LSTMCe11 클래스를 제공한다. 이름뿐만 아니라, 이 클래스는 LSTM
     레이어 전체를 제공한다. 마지막 섹션에서 더 큰 구조를 만들기 위해서LSTM 레이어들
     을다른네트워크에 연결하는방법을살펴볼 것이다．



     구조에 변화를 주자

     LSTM의 확장의 일반적인 것은 포겟 게이트forget gate를 더해서 내부적인 순환 연결
     recurrent connection을 스케일링scaling하는 것이다．
                                            이를 통해서 네트워크는 잊어버리
     는forget 기능을 학습한다
                    （Gers, Felix A., Jurgen Schmidhuber, and Fred Cummins,
     "Learning to forget: Continual prediction with LSTM," Neural Computation
     12,10(2000): 2451-2471.). 내부의 순환 연결의 미분값은 이제 포겟 게이트의 활성화값
     activation이 되고，
                   이 값은 1이 아니다. 이 네트워크은 문맥 정보가중요한 경우에는 포겟
     게이트를닫힌상태로 두는 것을학습할수 있다．

     포겟 게이트를 1로 초기화하는 것이 중요하다．
                             그러면 셀은 기억 상태「emembering state
     에서 출발한다. 포겟 게이트는 이제 대부분의 구현에서 필수적인 사항이다. 텐서플로우
     에서 forget_bias 파라미터를 LSTM 레이어로 명시함으로써, 포겟 게이트의 바이어
     스값을초기화할수 있다. 디폴트 값은1이고대부분 이러한방식으로사용하는 것이 최
     선의 방식이다．



                                 Ott螂』
                                     t Gate

                                 Output
                                 No川1neanty


                                 State
              ForgGa븐，

                                 Input Gate

                                 Input
                                 Nonlinearity




                         Forget Gate와 Gated Recurrent Unit(GRU）
                                                              를 가진 LSTM




CHAPTER 7 회귀 신경망과 자연 언어
                      （Recurrent Neural Networks and Natural Language)


===== PAGE 239 =====
또 다른 확장 방식은 게이트들이 셀의 상태를 볼 수 있도록 하는 방식인데, 보통 핍
홀peephole 연결이라고 불리운다
                   （Gers, Felix A., Nicol N. Schraudolph, and Jurgen
Schmidhuber. "Learning precise timing with LSTM recurrent networks." The Journalqf
Machine Learning Research 3(2003): 115-1143.). 이논문의 저자들은 핍홀 연결이 정교한
시간 정합timing과 시간 간격interva［이 필요한 일에 효과적이라고 주장한다．
                                              텐서플로우
의 LSThI 레이어는 이 핍홀 연결을 지원한다. 이 연결은 use_peepholes=True 파라미
터를LSTM 레이어에 전달함으로써 활성화될수 있다．

LSTM의 아이디어에 따라서, Gated Recurrent Unit(GRU）
                                         이라고 불리는 또 다른메
모리 셀이 2014년도에 제안되었다
                  （Chung, Junyoung, et al. "Empirical evaluation of
gated recurrent neural networks on sequence modeling." arXiv preprint arXiv:1412.3555
(2014).). LSTM과 비교해서，              비슷한 결과를 보이면서도
                    GRU는 조금 단순한구조로써，
계산량은 적다. GRU는 출력 게이트가 없고 입력과 포겟 게이트들을 하나의 업데이트
update 게이트로 결합한다．

이 업데이트 게이트는 내부의 상태가 후보 활성화 값과 얼마나 섞일지blended를 결정
한다. 후보 활성화값은 리셋reset 게이트와 새로운 입력에 의해서 결정되는 은닉 상태
hidden state의 부분fraction으로부터 계산된다. 텐서플로우의 GRU 레이어는 GRUCell이
라고 불리는데，
       그 레이어의 셀의 개수 파라미터만 가진다．
                             더 궁금한사람은Jozefwicz
등이 발표한 2015년도 논문을 참고하기 바란다
                         （Jozefowicz, Rafal, Wojciech Zaremba,
and /z그／α Sutskever. "An empirical exploration of recurrent network architectures."
Proceedings of the 32nd International Conference on Machine Learning(ICML-15).
2015.).



다중 순환 레이어

LSTM 네트워크는보통 서로완전 연결fully connected된많은셀들로 이루어진다．
                                               하나의
네트워크를 다른 네트워크의 상단에 쌓음으로써 다중 LSTM을 만드는 것도 가능하다．
성능은더 좋은데, 그 이유를 알고 있지는못하지만, 일반적으로 성능이 더 좋다．



                                                                             회귀 신경망소개   - 229


===== PAGE 240 =====
                                                   '        V\/5
                                               ■
                                               w
                                                       w4   ■ VV4+     w   "




                                                            w3
                                                                      ' *, 그쁘3
                                                                 w, ;T1



                              회구 신경망어나4의 다중 레이어




     단어 벡터 임베딩

     이 섹 크에서는 워드 임베딩word embedding을 학습할 모델을 만들 것이다．이는
     NLPNaturaL Language Processing     를 위한단어들을 표현하는 강력한 방법이
                                 （자연어 처리）
     다. 최근에 대량의 텍스트를 사용할 수 있도록 충분히 효율적인 방법인 워드 벡터 임베
     딩이 인기를 얻고 있다. 이것을 위해서 우리가 RNN을사용하지는 않지만, 향후의 다른
     일들에는사용할것이다. 워드 벡터 개념과word2vec과같은툴too〔에 익숙하지만, 직접
     구현하는데는 관심이 없다면 편하게 다음섹션으로 넘어가도 된다．

     단어들을 왜 벡터들로 표현할까？단어들을학습 시스템에 입력하는 가장 직접적인방법
     은 one-hot 인코딩이다．
                    이는 단어 사전 크기vocabulary size의 벡터인데，
                                                    해당 단어 위치
     에는 1을, 그리고 나머지 부분에는 모두 0인 값을 가지게 표현하는방식이다. 그런데 이
     방법은 두 가지 문제점이 있다. 자연어에는 아주 많은 단어들이 있기 때문에 실제 응용
     에서는 벡터가 너무 커진다는 점, 두 번째 단점은 이 one-hot 표현은 단어들 사이에 존
     재하는 의미의 유사성을 표현할수 없다는 점이다.




CHAPTER 7 회귀 신경망과 자연 언어
                      （Recurrent Neural Networks and Natural Language)


===== PAGE 241 =====
                                                            0     King
      1       0   0

          0   1   0     0        0          0         0     0     Queen

                                                  1
          0   0   1     0        0          0         0     0     Princess


                   0ne-hot 인코딩으로 표현된 단어들



단어들 사이의 의미의 유사성 문제의 해결책으로 단어들의 함께－출현co-occurrence 방
법이 오랫동안 연구되어 왔다．
               기본 개념을 소개해보자．
                           대량의단어 뭉치corpus가 있다．
각단어마다 특정 거리
          （여］
            를들어 5) 안에 있는주위의단어들의 개수를 센다. 각단어는
주위단어들의 정규화normalized된숫자들로 표현된다. 이를 출현 벡터occurrence vector라
고 하자. 이 방법의 기본 아이디어는 유사한 컨텍스트context에서 사용되는단어들은 유
사한 의미를 가진다는 것이다. 출현벡터는PCA 등의방법으로차원을줄일수 있다. 이
방법은 성능이 더 좋기는 하지만, 전체 단어 개수의 2차원 매트릭스 크기의 함께－사용
정보를관리해야한다는단점이 있다．

                  Age   Sex Wealth
                                                             m
                  0.8   0,8     0.9         0.1       0.3   0.3   King


                  0.7   0.1 0.8             0.2       0.1   0.5   Queen
                         一－     -m-   －叫一


                         -    mm뻔
                                「k욘寸繃1m』
                                       可巧二」 向h긋




                  0.3   0.1     0.6         0.5       0.3   0.9   Princess


                              단어의 분산 표현




                                                                             단어 벡터 임베딩   - 231


===== PAGE 242 =====
                2013년에 入lik이ov 등이 문맥에서 단어들을 표현하는 실용적이고 효과적인 방법을 제
                안했다．
                   Mikolov, Tomas, etαL "Efficient estimationqfword representations in vector
                space." arXiv preprint arXiv:130L3781(2013). 이 skip-gram 모델은 랜덤한값에서 시
                작해서, 현재의 단어에서 문맥 단어context word를 예측하는 간단한 분류기를 가지고 있
                다. 오류값은 분류기의 웨이트와단어 표현을 통해서 전파된다. 그리고 예측 오류를 줄
                이기 위해서 값들을 조절한다. 큰말뭉치에 대해서 이 모델을 학습하는 것은그 표현벡
                터가 압축된 함께－출현co-occurrence 벡터의근사치를만들어준다는 것이 밝혀졌다. 이제
                부터 텐서플로우를 이용해서 skip-gram 모델을만들어보자．



                Wikipedia 말뭉치 준비하기

                skip-gram 모델을 자세히 살펴보기 전에，
                                         영어 Wikipedia 덤프로부터 데이터셋을만
                들자. 기본적인 데이터는모든 페이지의 수정 기록을 포함하고 있다. 그러나 우리는 현
                재 버전에서도 100GB의 텍스트로 충분한 데이터를 가지고 있다. 이 예제는 다른 언어
                에도 적용할 수 있고，
                           Wikimedia Download 웹 사이트 /ittps://dumps.wikimedia.org/
                backup-index.htm／에서 사용가능한 데이터 뭉치의 개괄을살펴볼수 있다．


import bz2
import collections
import os
import re


class Wikipedia:


    def _init_     (self, un1, cache-dir, vocabulary size=      3) :
         pass
    def - iter- (self):
         ' " " Iterate over pages represented as lists of word indices. " "
         pass


   @property




 232 -   CHAPTER 7 회귀 신경망과 자연 언어
                               （Recurrent Neural Networks and Natural Language)


===== PAGE 243 =====
   def vocabulary_size(self):
       pass


   def encode(self) word):
       "Get the vocabulary index of a string word."""
       pa弱


   def decode(self, index):
       ' ' 'Get back the string word from a vocabulary index." " "
       pass


   def _read_pages(self, un1):
       .1∥ "




       Extract plain words from a Wikipedia dump and store them to the pages
       file. Each page will be a line with words separated by spaces.


       pass


   def _build_vocabulary(sel-f, vocabulary_size):
       1 ~ 11 ~ ·




       Count words in the pages file and write a list of the most frequent
       words to the vocabulary file.


       pass


   @classmethod
   def _tokenize(cls, page) :
       pass



데이터를 정확한 형식으로 만들기 위해서 몇 차례 절차를 거쳐야 한다. 이 책의 앞에서
본 적이 있었던 것 처럼, 데이터 수집과 정리 작업은 손이 많이 가고 중요한 작업이다．
one-hot 인코딩된 단어들로 표현되는 Wikipedia 페이지들을 반복적으로 작업해야

한다．

 1. 뭉치 데이터를다운로드하고페이지와단어들을추출한다．



                                                                     단어 벡터 임베딩   - 233


===== PAGE 244 =====
                 2. 가장빈번하게사용되는단어들의모음
                                   （단어집）
                                       을만들기 위해서단어수를센다．
                  3. 단어집을이용해서 추출된 페이지를인코딩한다．


               모든말뭉치가메인 메모리에 맞게 로딩되지는 않는다. 그래서 우리는 이 연산들을파일
               에서 한줄 한줄 읽으면서, 중간 결과를 디스크에 써가는, 즉 데이터 스트림에 수행해야

               한다. 이 방식은 스텝 사이에 점검할 수 있기 때문에 중간에 문제가 생기더라도 전체 과
               정을모두 다시 수행할 필요가 없다．
                                 Wikipedia를 처리하기 위해서 아래의 클래스를 사
               용한다. _init_ ( ）에서 파일이 있는지 체크함으로써 중간 과정의 완료를 점검하는
               것을알수 있다．


def _init_   (sel-F, unl, cache_dir, vocabulary_size=10000):
    sel-F._cache_dir = os.path.expanduser(cache_dir)
   self._pages_path = os. path. join(selF._cache_dir, 'pages .bz2')
   self._vocabulary_path = os.path. join(self._cache_dir, 'vocabulary.bz2')


   if not os.path.isfile(self._pages_path) :
         print( 'Read pages')
         self. _read_pages(unl)
   if not os. path. isfile(self._vocabulary_path):
         print('Build vocabulary')
         self._build_vocabulary(vocabulary_size)
   with bz2.open(self._vocabulary_path, 'rt ') as vocabulary:
         print( 'Read vocabulary')
         sel-F._vocabulary = [x.strip() for x in vocabulary]
    sel-F._indices = {x: I for I, x in enumerate(sel-F._vocabulary)}


def _iter_ (self):
    "Iterate    over pages represented as lists of word indices." " "
    with bz2.open(self._pages_path, 'rt ') as pages:
         for page in pages:
             words = page.stripQ.split()
             words = [self.encode(x) for x in words]
             yield words




 234 -                        （Recurrent Neural Networks and Natural Language)
         CHAPTER7 회귀 신경망과 자연 언어


===== PAGE 245 =====
@property
def vocabulary_size(self):
    return len(self._vocabulary)


def encode(self, word):
    "Get the vocabulary index of a string word.
    return self._indices.get(word, 0)


def decode(self, index):
    " 'Get back the string word from a vocabulary index."
    return self._vocabulary[index]



이 Wclass에서 2개의 중요한 함수를 구현해야 한다. _read_pages( ）는 압축된 XML

파일 형식의 Wikipedia 뭉치를 다운로드하고，
                           각 페이지마다 포매팅 정보를 제거하기
위해서 보통의 단어들을 추출하는 작업을 반복한다. 압축 파일을 읽기 위해서 파일을
스티리밍streaming하면서도 압축과 압축 해제 모두가 가능한 open( ) 함수를 제공하는
bz2 모듈이 필요하다. 디스크 공간을 절약하기 위해서 중간 결과 파일에도 압축을수행

한다. 어떤 연속된 글자들이라든지, 특별한문자들의 각각의 사용 정보를 파악할수도

있다．


TOKEN_REGEX = re.compile(r '[A-Za-z]+I[!?.:,Q]')
def _read_pages(self, unl):


    Extract plain words from a Wikipedia dump and store them to the pages fUe.
    Each page will be a line with words separated by spaces.


    wikipedia_path = download(url, self._cache_dir)
    with bz2.open(wikipedia_path) as wikipedia, \
        bz2.open(self._pages_path, 'wt') as pages:
        for _, element in etree.iterparse(wikipedia, tag='{*}page') :
            if element.find( ' ./{*}redirect') is not None:
                continue
            page = element.findtext( ' ./{*}revision/{*}text')




                                                                 단어 벡터 임베딩   - 235


===== PAGE 246 =====
                words = self._tokenize(page)
                pages.write( " .join(words) + '\n ' )
                element.clear()


@= lassmethod
    def _tokenize(cls, page):
          words = cis.TOKEN_REGEX.findall(page)
          words = [x.lower() -For x in words]
          return words



                 one-hot 인코딩을 위해서 사용할 단어집vocabuLary of words이 필요하다．그래야만 그 단
                 어집 안의 인덱스로 각 단어를 인코딩할 수 있기 때문이다. 오타나 자주 사용하지 않는
                 단어들을삭제하기 위해서, 단어집은 vocabulary - 1 개수의 가장자주 사용하는 단
                 어들을 포함하고, <unk> 토큰은단어집에 없는 모든단어를 위해서 사용된다. 이 토큰은

                 나중에 처음 접하는단어의 단어 벡터를 위해서 사용할 것이다．


def _build_vocabulary(self, vocabulary_size):


    Count words in the pages file and write a list of the most frequent
    words to the vocabulary file.


    counter = collections.Counter()
    with bz2.open(self._pages_path, 'rt ') as pages:
                    for page in pages:
                         words = page.stripO.split()
                        counter. update(words)
          common = ['<unk> '] + counter.most_common(vocabulary_size-1)
          common = [x[8] for x in common]
          with bz2.open(self._vocabulary_path, ' wt ') as vocabulary:
                    for word in comon:
                         vocabulary.write(word + ' \n ' )




  236 -                         （Recurrent Neural Networks and Natural Language)
          CHAPTER 7 회귀 신경망과 자연 언어


===== PAGE 247 =====
보통의 텍스트를 추출하고 단어들을 인코딩했기 때문에 학습 예제를 쉽게 만들 수 있다．

예제를 저장하는 것은 많은 저장 용량을 필요로 한다. 어쨌든 대부분의 시간은 학습을
위해서 사용되기 때문에 이것은 성능에 별 문제가 되지 않는다. 좀 더 효율적으로 학습
시키기 위해서 결과 예제를 배치batch로 그룹을 만들자. 분류기는 많은 메모리를 필요로
하지 않기 때문이, 이 모델로 아주큰 배치를 사용할수 있을 것이다．

그래서，
   어떻게 학습 샘플 들을 만들 수 있을까？ skip-gram 모델이 현재의 단어들로부
터 문맥에 적합한 단어들을 예측한다는 점을 기억하자. 텍스트를 반복하면서 현재의 단
어를 데이터로 하고 그 주위의 단어들을 타겟으로 하는 학습 샘플을 만든다. 문맥 크기
R=5인 경우에, 단어마다좌측으로5단어, 우측으로5단어를사용해서 학습샘플을10개
생성한다. 가까운 이웃이 멋 이웃보다 의미상으로 더욱 중요하다고 생각할 수도 있다．
그래서 문맥의 크기를 랜덤하게 설정하고, 멀리 있는단어는 적은 개수를 사용하였다．


def skipgrams(pages, max_context):
    ' " "Form training pairs according to the skip-gram model." " "
   for words in pages:
        for index, current in enumerate(words) :
            context = random.randint(l, max_context)
            for target in words[max(0, index - context):index]:
                  yield current, target
            for target in words[index + 1: index + context + 1]:
                  yield current, target


def batched(iterator, batch_size):
    " 'Group a numerical stream into batches and yield them as Numpy arrays."
    while True:
    data = np. zeros(batch_size)
    target = np. zeros(batch_size)
   for index in range(batch_size):
        data[index], target[index] = next(iterator)
        yield data, target




                                                                      단어 벡터 임베딩   - 237


===== PAGE 248 =====
     모델 구조

     이제 우리는 Wikipedia 말뭉치가 있으니까단어 임베딩을 계산할 모델을 정의할 수
     있다．

      class EmbeddingModel:
           def _init_   (self, data, target, params):
               self.data = data
               self.target = target
               self. params = paranis
               self. embeddings
               self. cost
               self. optimize


      @lazy-property
      def embeddings(self):
           pass


      @lazy_property
      def optimize(self):
           pass


      @lazy_property
      def cost(self):
           pass



     각단어는랜덤 벡터로 표현되는 것으로 시작한다. 단어의중간상태의 표현으로부터 분
     류기는 그것의 문맥 단어 중의 하나의 현재 표현을 여］측하려고 할 것이다. 그 다음에웨
     이트와 입력 단어의 표현을조절하기 위해서 에러를 전파할 것이다. 단어 표현을 위해서
     tf.Variable을사용한다．


      @lazy_property
      def embeddings(self):
           initial = tf. random-uniform(




                      （Recurrent Neural Networks and Natural Language)
CHAPTER 7 회귀 신경망과 자연 언어


===== PAGE 249 =====
        [self.params.vocabulary_size, sel-F.params.embedding_size], -1.0, 1.0)
     return tf.Variable(initial)



우리는 똑똑하지는 않지만 아주 빠르다는 장점이 있는 MomentumOptimize
                                            「를 사용한
다．
 이것은 우리의 큰 Wikipedia 말뭉치와잘 작동한다．
                               그리고 좋은 알고리즘 보다 더
많은 데이터를 선호한다는skip-gram에 숨겨진아이디어와도 잘맞다．


@lazy_property
 def optimize(self):
     optimizer = t-F.train.MomentumOptimizer(
         self .params.learning_rate,sel-F.params.momentum)
     return optimizer.minimize(self.cost)



우리의 모델에서 빠진 부 분 은 분류기이다．
                       성공적인 skip-gram모델의 핵심인 이 부분을
이제부터 살펴볼 것이다．



NOISE CONTRASTIVE CLASSIFIER

skip-gram 모델을 위한 비용 함수cost function는 여러 가지가 있다．
                                              그 중에서 noise-
contrastive estimation loss가 아주잘 작동한다고 알려져 있다. 이상적으로는, 예측이 타

겟에 가까워야할 뿐만 아니라, 현재 단어를 위한 타겟이 아닌 단어들로부터는 멀어야
한다. 이것은 소프트맥ㅅ 분류기로 잘 모델링될 수 있다. 그러나 매번 알파벳에 있는 모
든 단어들을 계산하고 학습하고 싶지는 않다. 우리의 아이디어는 '대조 예제contrastive

examples'라고 불리는 negative example로 새로운 랜덤 벡터를 사용하는 것이다. 충분
한 반복 학습을 통해서 10개의 클래스를 필요로 하면서 평균적으로 소프트맥ㅅ 분류기
에 근접하게 된다. 텐서플로우는 이를 위한 편리한tf. nn. nce_loss 함수를 제공한다．




                                                               단어 벡터 임베딩         - 239


===== PAGE 250 =====
@lazy_property
def cost(self):
      embedded = tf.nn.embeddingjookup(self.embeddings,self.data)
      weight = tf.Variable(tf.truncated_normal([sel-f.params.vocabulary_size,
            self.params.embeddingsize], stddev=l.0 I
            self.params.embedding_size ** 0.5))
      bias = tf.Variable(tf.zeros([self.params.vocabulary_size]))
      target = tf.expand_dims(self.target, 1)
      return tf.reduce_mean(tf.nn.nce_loss(weight, bias, embedded, target,
            self.params.contrastive_examples,
            self.params.vocabulary-size))




                 모델 학습하기

                 이제 말뭉치와 모델이 있다. 이제 모든 것을 합치기 위한 나머지 코드를 보자. 학습 후
                 에 최종적인 임베딩을 다른 파일에 저장한다. 아래의 예는 보통의 (:pu에서 5시간 동안
                 학습한 Wikipedia 의 부분 집합을 사용한다．
                                            모든 말뭉치를 사용하기 위해서는 unl을
                 다음으로 변경하자：https://durnps.wikimedia.org/enwiki/20160501/enwiki-20160501-
                 pages-rneta-current.xmLbz2.


params = AttrDict(
      vocabulary_size=10000,
      max_context=10,
      embedding_size=200,
      contrastive_examples=100,
      learning_rate=0. 5,
      momentum=0. 5,
      batch_size=1000,
)

data = tf. placeholder(tf. int32, [None])
target = tf. placeholder(t-f.int32, [None])
model = EmbeddingModel(data, target, params)




    240 -   CHAPTER 7 회귀 신경망과 자연 언어
                                  （Recurrent Neural Networks and Natural Language)


===== PAGE 251 =====
corpus = Wikipedia(
    " https:1/dumps.wikimedia.org/enwiki/20160501/ ' \
    'enwiki- 20160501- pages-meta- currenti.xm1p000000010p000030303.bz2' J
    '/home/user/wikipedia', params.vocabulary_size)


examples = skipgrams(corpus, params.max_context)
batches = batched(examples, params.batch_size)


sess = tf.Session()
sess.run(tf.initialize_all_variables Q)
average = collections.deque(maxlen=100)
for index, batch in enumerate(batches):
    feed_dict = {data: batch[0], target: batch[1]}
    cost, - = sess.run([model.cost, model.optimize], feed_dict)
    average,append(cost)
    print('{}: {:5.lf}'.format(index + 1, sum(average) I len(average)))
    embeddings = sess.run(model.embeddings)
    np.save( '/home/user/wikipedia/embeddings.npy', embeddings)




시퀀스 분류


시퀀스 분 류 는 전체 입력 시퀀스를 위한클래스를 예측하기 위한 문제 셋팅이다. 이런

문제는 유전학genomics과 재정finance을 포함하는 많은 분야에서 일반적인 문제이다．
NLP에서는 감정 분석이 유명한 문제이다. 사용자가 작성한 텍스트에서 주어진 주제에

대한 성향 예측과 같은 문제가 있다. 예를 들어 선거에서 특정한 후보를 언급하는 트윗
의 감정을 예측한 결과를 선거 결과를 전망하기 위해 사용할 수 있다. 다른 예제는 작성
된 비평들로부터 제품이나 영화의 품평을 예측하는 것이 있을 수 있다. 비평은 보통 타
겟 값으로 사용하기 편리한숫자로 되어 있어서 NLP 커뮤니티에서 벤치마크 작업으로
사용된다．




                                                                       시퀀스 분류   - 241


===== PAGE 252 =====
                 우리는 International Movie Database에서 2개의 대답，
                                                          즉 positive 또는 negative 로
                 구성되는 영화 비평 데이터셋을 사용한다. 이 데이터셋에서 단어들의 존재 유 무 를 살펴
                 보는 단순한 방법은 일반적으로 언어에 있는 부정, 아이러니, 모호성 등 때문에 실패하

                 곤 한다. 그래서 우리는 이전 섹션에서의 단어 벡터에서 동작하는 순환 모델을 만들 것
                 이다. 순환네트워크는한단어씩 비평을보면서, 마지막단어의 액티베이션activation of

                 the last word으로부터 분류기가 전체 비평의 감정을 예측하도록 훈련할 것이다. 전체 구
                 조를 끝에서 끝까지 학습시키기 때문에 RNN은 향후의 분류 작업에 가장 가치 있을 것
                 같은단어들로부터 유용한 정보를수집하고 인코딩할 것이다．



                 Imdb Movie 비평 데이터셋

                 Stanford University의 AT 학과：http://ai.stanford.edu/-amaas/data/sentiment／에
                 서 제공되는 영화 비평 데이터셋을 사용하자. 2개의 관련된 폴더 안에 텍스트 파일로
                 positive 또는 negative 비평을 담은 압축된 tar 파일이다．
                                                         지난 섹션에서 芍구식「egular
                 expression을 이용한 평이한 단어plain word 추출과 소문자로의 변환 과정에서 텍스트의
                 전처리 과정과동일한 과정을 수행한다．


import tarfile
import re


class ImdbMovieReviews:
DEFAULT-URL = 'http://ai.stanford.edu/-.amaas/data/sentiment/acllmdb_vl. tar.gz '
TOKEN_REGEX = re.compile(r '[A-Za-z]+I[!?.:,O]')


def _init_   (self, cache_dir, url=None):
    self, cache dir = cache dir
    self._url = url or type(self).DEFAULT_URL


def _iter_ (self):
    filepath = download(self._url, self._cache_dir)




  242 I   CHAPTER 7 회귀 신경망과 자연 언어
                                （Recurrent Neural Networks and Natural Language)


===== PAGE 253 =====
    with tarfile.open(filepath) as archive:
        for filename in archive.getnames():
            if filename.startswith( 'acllmdb/train/pos/'):
                  yield self._read(archive, filename), True
            elif filename.startswith( 'acllmdb/train/neg/'):
                  yield self._read(archive, filename), False


def _read(sel-F, archive, filename):
    with archive.extractfile(filename) as file_:
        data = file_.readQ.decode( 'ut-F-8')
        data = type(sel-f).TOKEN_REGEX.findall(data)
        data = [x.lower() for x in data]
    return data




단어 임베딩 사용하기

단어 벡터 임베딩 섹션에서 설명한 바와 같이, 임베딩은 one-hot 인코딩된 단어보다 의
미상으로 더욱 풍부하며, 우리의 RNN이 one-hot 인코딩된단어들보다 영화 비평의 임
베딩된 단어들에게 동작하도록 도울 것이다. 이를 위해서 참고 섹션
                                   「eference section에서
계산하였던단어집과 임베딩을사용할 것이다. 코드는 쉽게 알아볼수 있을텐데, 단어의
인덱스를 결정하기 위해서 단어집을사용하고, 적합한 小ㅔ딩 벡터를 찾기 위해서 그 인
덱스를 사용한다. 다음의 클래스는 다루기 쉽게 하기 위해서 시퀀스들을 같은 길이로맞
추기 위해서 데이터를 덧붙인다padding.




                                                               시퀀스분류   - 243


===== PAGE 254 =====
import bz2
import numpy as np


class Embedding:
   def _init_(self, vocabulary_path, embedding_path,length):
        self._embedding = np.load(embedding_path)
        with bz2.open(vocabulary_path, 'rt ') as file_:
             self._vocabulary = {k.strip(): i for 1, k in enumerate(file_)}
             self._length = length


   def _call_(sel-F, sequence):
        data = np.zeros((self._length, self._embedding.shape[l]))
        indices = [self._vocabulary.get(x, 0) for x in sequence]
        embedded = self._embedding[indices]
        data[:len(sequence)] = embedded
        return data


   @property
    def dimensions(sel-F):
        return self._embedding.shape[l]




               시퀀스 레이블링 모델


               텍스트 시퀀스의 감정을 분류하고자 한다. 지도 학습이기 때문에 그 모델에 2개의 플

               레이스홀더를 전달한다. 하나는 입력으로써 data 또는 시퀀스, 다른 하나는 target

               값 또는 감정이다．
                        순환 층「ecurrent [aye
                                         「의 크기，
                                              셀 구조           , 사용할 최적
                                                 （LSTM, GRU 등）

               화 함수와 같은 파라미터를 가지는 params 객체도 전달한다. 우리는 지금 그 프라퍼티

               property를 구현하고 상세하게 살펴볼 것이다．




                          （Recurrent Neural Networks and Natural Language)
 24시 애APTER 7 회귀 신경망과 자연 언어


===== PAGE 255 =====
class SequenceClassificationModel:


    def _init_(sel-F, data, target, params):
        self.data = data
        self.target = target
        self.pa rams = params
        self.prediction
        self,cost
        self.error
        self.optimize


   @lazy_property
    deF length(self):
        pass


   @lazy_property
    de'F prediction(self):
        pass


   @lazy_property
    def cost(self):
        pass


   @lazy_property
    def error(sel-F):
        pa5S


   @lazy_property
    def optimize(self):
        pass


   @staticmethod
    def _last_relevant(output, length):
        pass




                                               시퀀스분류   - 245


===== PAGE 256 =====
              먼저，
                현재의 데이터 배치에서 시퀀스의 길이를 구한다. 데이터가 가장 긴 비평 길이에
              맞춰서 0 벡터가 패딩된 하나의 텐서로 들어오기 때문에 시퀀스의 길이가 필요하다. 모
              든 비평의 시퀀스 길이를 저장하는 대신에 텐서플로우에서는 이것을 동적으로 계산한
              다. 시퀀스마다의 길이를 구하기 위해서 단어 벡터를 절대값의 최대값을 이용해서 단어
              벡터를줄인다collapse. 그 결과스칼라값은0 벡터를 위해서는0이, 다른 실제단어 벡터
              를위해서는0보다큰 값을가진다. 이 값을tf.sign( ）을 이용해서 0 또는 1로 이산화
              discretize하고，각 시퀀스의 길이를 구하기 위해서 타임 스텝을 따라서 결과값을 합한다.
              그 결과 텐서는배치 크기의 길이를 가지고 각시퀀스의 스칼라 길이를 가진다．


@lazy. property
de-F length(self):
    used = t-F. sign(t-f. reducemax(t-f. abs(sel-f.data), reduction indices= ))
    length = t-f.reduce-sum(used, reduction indices= )
    length = t-f.cast(length, tf. int32)
    return length




              냐＼ST RELEVANT ACTIVATION에서 소프트맥ㅅ

              예측을 위해서 보통 때처럼 RNN을 정의하자. 그러나 이번에 우리는 RNN의 마지막
              액티베이션 위에 소프트맥스 레이어를 쌓음으로써 RNN을 확장한다. RNN을 위해서

              params 객체에 정의된cell type과ce끄 count를사용한다．
                                                    RNN에 배치batch의 줄수를
              알기 위해서 이미 정의된 length 프라퍼티를 사용한다. 각 시퀀스의 마지막 출력 활성
              값을 소프트맥스 레이어에 입력한다. 소프트맥스 레이어를 정의하는 것은 이 책의 지금
              까지를따르면 쉽게 할수 있을 것이다．

              RNN의 마지막 relevant 출력 활성값은 학습 배치에서 각 시퀀스의 다른 인덱스를 가
              진다. 왜냐하면 각 비평은 다른 길이를 가지기 때문이다. 우리는 이미 각 시퀀스의 길
              이를 알고 있다. 그래서 마지막 활성값을 선택하기 위해서 그것을 어떻게 사용할 수 있
              을까？우리의 문제는 타임 스텝의 차원에서의 인덱스를 원한다는 것이다. 이 차원은



 246 I   CHAPTER 7 회귀 신경망과 자연 언어
                               （Recurrent Neural Networks and Natural Language)


===== PAGE 257 =====
1   1-
         -   'r---




             sequences * time_steps * word_vectors 형태의 배치에서 2번째 차원이다．


             @lazy_property
             def prediction(sel-F) :
                     # Recurrent network.
                     output, _ = rnn.dynamic_rnn( self.params. rnn_cell(sel-F.params.rnn_hidden),
                         self.data, dtype=tf. fl0at32, sequence_lertgth=self.length, )
                     last = selF._iast_relevant(output, self.length)
                     # Softmax Layer.
                     num_classes = int(self.target.get_shapeQ[i])
                     weight = tf. Variabie(tf. truncated_normal(
                         [sel-F.params. mnn_hidden) num_classes], stddev=0.01))
                     bias = t-f.Variable(t-f.constant(@.1, shape=[num_ciasses]))
                     prediction = tf. nn.softmax(t-F.matmul(last, weight) + bias)
                     return prediction


             지금 텐서플로우는 t-F.gatheN ）를 통해서 첫 번째 차원을 따라서만 인덱싱을 지원
         한다. 그래서 sequences * time_steps * word_vectors 형태에서 첫 번째 2개의 차
             원을 평탄화한다ifatten. 그리고 이 텐서에 인덱스를 생성한다. 인덱스는 평탄화된 텐서
             의 각 시퀀스에 대한 시작 인덱스를 고려해서, 시퀀스의 길이를 더한다. 실제로 우리는
             length-i을더한다. 이렇게 마지막타임 스텝을 선택할수 있다．


             @staticmethod
              def _last_relevant(output, length) :
                     batch_size = t-F. shape(output)[8]
                     max_length = int(output .get_shapeQ[l] )
                     output_size = int(output.get_shapeQ[2])
                     index = t-F.range(0, batch_size) * max_length + (length       1)
                     flat = t-1.reshape(output, [-1, output_size])
                     relevant = tf. gather(flat, index)
                     return relevant




                                                                                         시퀀스분류      - 247


===== PAGE 258 =====
              소프트맥스 층과】
                      之NN의 타임 스텝을 통해서 텐서플로우가 에러를 전파하면서 전체 모

              델을학습시킬 수 있다. 이제 비용함수만 남았다．



              기울기 자르기
                    （gradient clipping)

              시퀀스 분류를 위해서, 모델의 출력값은 가능한 클래스 상의 확률 분포이기 때문에, 분
              류에 합당한 어떤 비용 함수든지 사용할 수 있다．
                                        우리 예제에서 두 클래스는 positive와
                           그리고 우리는 물체 인식과 분류에서 사용했던 표준 크로스 엔트로
              negative 감정이다．
              피 비용cross entropy cost을사용한다．

              비용 함수를 최소화하기 위해서 설정에서 정의된 최적화기를 사용한다. 그러나 기울기
              자르기를추가함으로써 이제까지 배운 것을향상 시킬것이다. RNN은학습시키기 매우
              어렵고 웨이트는 하이퍼 파라미터들이 서로 잘 조율되지 않으면 발산하는 경향이 있다．

              기울기 자르기 아이디어는 기울기 값이 특정 범위의 값이 되도록 제한하는 것이다. 이런
              방식으로 웨이트 변화량의 최대치를 제한할수 있다．


@lazy_property
def cost(self):
    cross_entropy = -tf.reduce_sum(self.target * tf. log(self.prediction))
    return cross_entropy


@lazy_property
def optimize(self):
    gradient = self.params .optimizer.compute_gradients(self.cost)
    if self.params.gradient_clipping:
         limit = self.params .gradient_clipping
         gradient = [(tf. clip_by_value(g, -limit, limit) , v)
             if g is not None else (None, v)
             for g, v in gradient]
         optimize = self.params .optimizer.apply_gradients(gradient)
         return optimize




 2L8 I   CHAPTER 7 회귀 신경망과 자연 언어
                               （Recurrent Neural Networks and Natural Language)


===== PAGE 259 =====
@lazy_property
def error(self):
    mistakes=t-F.not_equal(tf.argmax(sel-f.target, l),tf.argmax(self.prediction,   ))
    return tf.reduce-mean(tf.cast(mistakes, tf.fl0at32))



텐서플로우는 각 최적화기 인스턴스가 제공하는 compute_gradient쐬 ) 함수로 이
시나리오를지원한다. 그리고apply_gradient引 ）로기울기를수정하고웨이트변화
                               이 값보다작으면 -limit으
를 적용할수 있다. 기울기 자르기를 위해서 값을 설정하고，
로，
 이 값보다 크면 limit으로 설정한다. 텐서플로우에서의 미분값은 변수와 비용 함수

사이에 관계가 없는 경우에는None을 가지도록 하였다. 수학적으로 그러한 미분값은 0
벡터이어야 한다. 그러나 None을 사용함으로써 내부적인 성능 최적화를할수 있다. 그
런 경우는None 값을튜플로 되돌려 전달함으로써 제어한다.



모델 학습

위에서 정의한 개량된 모델을 트레이닝하자. 우리가 말한 바와 같이 단어 단위로 순환
신경망에 영화 비평을 입력한다. 그러면 각 타임 스텝은 단어 벡터들의 배치이다. 단어
벡터를찾기 위해서 지난섹션의 batched( ) 함수를사용한다. 그리고모든 시퀀스들
을같은 길이로 패딩한다．


deF preprocess_batched(iterator, length, embedding, batch_size):
    iterator = iter (iterator)
    while True:
        data = np. zeros((batch size, length, embedding.dimensions) )
        target = np. zeros((batch_size,     ))
        for index in r'ange(batch_size) :
            text, label = next(iterator)
            data[index] = embedding(text)
            target[index] = [ ,   I if label else
        yield data, target




                                                                        시퀀스 분류   - 249


===== PAGE 260 =====
                 이제 모델을 쉽게 트레이닝할수 있다. 하이퍼 파라미터들을 정의하고, 데이터셋과 임베
                 딩을로딩하고, 전처리된학습배치로모델을실행한다．


params = AttrDict(
      rnn_cell=GRUCell,
      mnnJ山Jden=300,
      optimizer=tf. train.RMSPropOptimizer(0. 0e2),
      batch_size=20,
)

reviews = ImdbMovieReviews( '/home/user/imdb')
length = max(len(x[0]) for x in reviews)


embedding = Embedding('/home/user/wikipedia/vocabulary.bz2',
      '/home/user/wikipedia/embedding,npy', length)
batches = preprocess_batched(reviews, length, embedding, params.batch_size)


data = t-F.placeholder(tf. fl0at32, [None, length, embedding.dimensions])
target = tf. placeholder(t-f.fl0at32, [None, 2])
model = SequenceClassificationModel(data, target, params)


sess = t-F.Session()
sess. run(tF.initialize_all_variables 0)
for index, batch in enumerate(batches):
      feed = {data: batch[0], target: batch[1]}
      error, - = sess.run([model.error, model.optirnize], feed)
      print( '{}: {:3.lf} %'.format(index + 1, 100 * error))


                 이 모델의 학습 성공은 네트워크의 구조와 하이퍼 파라미터뿐만 아니라 단어 임베딩
                 의 품질에도 영향을 받는다. 지난 섹션에서 기술된 단어 임베딩을 학습시키지 않는다면
                 word2vec 프로젝트에서 skip-gram 모델을 구현해서 이미 학습된 임베딩을 로딩해서
                 사용할 수 있다：skip-gram 모델의 구현：https://code.google.com/archive/p/word2vec.
                 또는 Stanford NLP 그룹의 매우 유사한 Glove 모델：加p://nlp.stanford.edu/pr可ects/




    250 -                         （Recurrent Neural Networks and Natural Language)
            CHAPTER 7 회귀 신경망과 자연 언어


===== PAGE 261 =====
glove／를사용할수 있다. 위의 두경우모두웹 상의 파이썬로더를찾을수 있을것이다．

이제 이런 멋진모델이 있다. 이것으로 무엇을할수 있을까？데이터 사이언스 경기를 호
스팅하는 유명한 웹 사이트인 Kaggle에 오픈 러닝 대결이 있다．
                                    이 섹션에서 우리가 한
것과 같은 IMDB 영화 비평을 사용한다. 그래서 만약 당신의 결과를 다른 사람의 결과
와 비교해보고 싶다면 당신의 모델을 그들의 테스트셋으로 테스트하고 그 결과를 다음
사이트에 업로드하라 https://www.kaggle.com/c/word2vec-nlp-tutorial. 지금 이 책을
쓰는 시점에는 그 데이터셋을 해결한 0.99259의 AUC 점수가 최고이다. AUC는 Area
Under the receiver operating Curve라는뜻으로 precision과reca끄을 결합한숫자값
이다．




시퀀스 레이블링

지난 섹션에서 ISTM 네트워크와마지막 액티베이션 위에 소프트맥스 레이어를 쌓은
시퀀스분류모델을만들었다. 이제는시퀀스 레이블링의 조금 더 어려운문제에 도전해
보자. 이 문제는 입력 시퀀스의 각 프레임에 대해서 각각의 클래스를 예측한다는 점에서
시퀀스분류와조금다르다．

예를 들어, 필기체 글자를 인식하는 경우를 생각해보자. 한단어의 각각의 문자는 개별
적으로 인식할수 있으며，
            단어는 이러한 문자들의 시퀀스이다．
                              또한 언에anguage에는
문자들의 순서 관계에 강한 구조적 정보가 있다. 작성된 샘플 문자를 보면 해당 글자만
으로는 읽기 힘든경우가있다. 예를들어 "n" , "irt", "ii" 와같은문자들이 해당되는데，
이런 문자들은 주위의 글자를 보면 인식될 수 있다. 이 섹션에서 우리는 문자들간의 의
존정을사용하기 위해서 RNN을사용해서 더욱강건한OcROptical Character Recognition
시스템을만들 것이다．




                                                            시퀀스 레이블링   - 251


===== PAGE 262 =====
                     （optical character recognition) 데이터셋
              광학 문자 인식

              시퀀스 레이블링 문제의 예제로 Mif의 Spoken Language Systems Group의 Rob
              Kassel이 수집하고 Stanford Al 그룹의 Ben Taskar에 의해 전처리된 OCR 데이터셋을
              살펴보자．
                  이 데이터셋은 각각의 글자가 16X8 크기의 이진 이미지binary image이다．각
              글자들은단어를구성하기 위해서 시퀀스로 나열되어 있다. 전체 데이터셋에는 대략 길
              이가14까지되는6800개의단어들이 있다．

              아래는3개의 단어 예제이다．
                            단어들은 cafeteria, puzzlement, unexpected이다．
                                                                    첫글
              자들은 대문자라서 데이터셋에 포함되지 않았다. 모든 시퀀스는 길이가 최대 14가 되도
              록 패딩되었다. 문제를 조금 쉽게 만들기 위해서 소문자만 포함되어 있다. 그래서 어떤
              단어들은 첫글자가빠진 경우도 있다．



                     叭
                          N e［恨n                .
                                                    氏

                            군 t노idt )NL
                                   '

                     나1
                          2.
                     14   P/ 巴αI Pi/
                                   /)
import gzip
impo吐 csv
import numpy as np


class OcrDataset:


   Dataset of handwritten words collected by Rob Kassel at the MIT Spoken
    Language Systems Group. Each example contains the normalized letters of the
    word, padded to the maximum word length. Only contains lower case letter,




 252 -   CHAPTER7 회귀 신경망과 자연 언어
                              （Recurrent Neural Networks and Natural Language)


===== PAGE 263 =====
capitalized letters were removed.
From: http:IIai.stanford.edu/-btaskar/ocr/




URL = 'http://ai.stanford.edu/-btaskar/ocr/letter.data.gz'


def _init_(self, cache_dir):
    path = download(type(self).URL, cache_dir)
    lines = self._read(path)
    data, target = self. parse(lines)
    self.data, self.target = self._pad(data, target)


@staticmethod
def _read(filepath):
    with gzip.open(filepath, ' rt') as file_:
        reader = csv.reader(lile_, delimiter='\t ' )
        lines = list(reader)
        return lines


@staticmethod
def - parse(lines):
    lines = sorted(lines, key=lambda x: int(x[e]))
    data, target = [1J [I
    next   = None
    for line in lines:
        if not next :
            data.append([])
            target.append([])
        else:
            assert next_ == int(line[0])
             next_ = int(line[2]) if int(line[2]) > -1 else None
             pixels = np.array([int(x) for x in line[6:134]])
             pixels = pixels.reshape((16, 8))
            data[-1].append(pixels)
            target[-l].append(line[1])




                                                             시퀀스 레이블링   - 253


===== PAGE 264 =====
         return data, target


  自staticmethod
  def     pad(data, target):
         max_length = max(len(x) for x in target)
         padding = np. zeros((16, 8) )
         data = [x + ([padding] * (max_length - len(xfl) for x in data]
         target = [x + ([ ' ] * (max_length - len(xfl) for x in target]
         return np. array(data), np.array(target)


                                                             파이썬의 csv 모듈로 읽을 수
               데이터셋은 http.J/ai.stanford.edu/-btaskar/ocr/에 있다．
               있는，
                 탭으로 구분되는 텍스트 파일이 gzip으로 압축되어 있다．
                                                각 줄은 데이터셋의 하
              나의 글자를표현하며 id,타겟 글자，
                                 픽셀 값, 단어에서의다음글자id 등을 포함한다．

              id 값으로 정렬해서 각단어들을 정확한순서로 문자들을 읽을수 있다. 그 다음에, 다음
              id가 없을 때까지 계속 글자들을 수집한다. 타겟 글자와 픽셀값을 읽은 다음, 그 시퀀스
              를zero 이미지로 패딩해서 타겟 글자와 픽셀값을가진두 개의큰Numpy 배열에맞도
              록한다．



               타임 스텝 사이에서 공유되는 소프ㅌ맥ㅅ

               이번에는 데이터뿐만아니라타겟도 시퀀스인 경우이다. 즉, 각 이미지 프레임마다하나
               의 타겟 문자가 있다. 각 프레임에 대한 예측을 얻는 가장 쉬운 방법은 우리의 RNN을
               확장하는 것인데, 각글자의 출력에 소프트맥스 분류기를올린다. 이것은 마지막에 한
               번만 하지 않고매 프레임마다 평가한다는 점을 제외하면 지난섹션의 시퀀스 분류 모델
               과아주유사하다．

                class SequenceLabellin핸odel:


                    def _init_   (sei-F, data, target, params) :
                         self.data = data




,,b4 -                        （Recurrent Neural Networks and Natural Language)
         CHAPTER7 회귀 신경망과 자연 언어


===== PAGE 265 =====
        self.target = target
        sel-F.params = params
        self.prediction
        self.cost
        self.error
        self.optimize


   @lazy_property
    def length(self):
        pass


   @lazy_property
    def prediction(self):
        pa5S


   @lazy_property
    def cost(self):
        pass


   @lazy_property
    def error(self):
        pass


   @lazy_property
   def optimize(self):
        pass



우리의 시퀀스 레이블링 모드의 메소드들을 구현하자. 먼저 시퀀스의 길이를 계산할 필

요가 있는데, 지난 섹션에서 이미 했었기 때문에 여기서 추가할 것은많지 않다．



@lazy_property
def length(self):
    used = t-F.sign(tf. reduce_max(tf. abs(self.data), reduction_indices=2))
    length = tf. reduce_sum(used, reduction_indices=l)




                                                                  시퀀스 레이블링     - 255


===== PAGE 266 =====
                     length = tf.cast(length, tf.int32)
                     return length


              이제 예측부분을 구현해야 한다. 시퀀스 인식 모델과의 가장 큰다른 점이 이 부분이다．
              소프트맥스 레이어를 모든 프레임에 추가하는 두 가지 방법이 있다. 다양한 여러 개의
              분류기를 추가하거나 모든 프레임이 같은 분류기를 공유할수 있다. 3번째 문자를 분류
              하는 것이 8번째 문자를 분류하는 것과많이 다를 수 없기 때문에 2번째 방법이 합당해
              보인다. 이런방식으로 분류기의 웨이트들은단어의 각 문자가 그들을 학습하는데 영향
              을미치기 때문에 더자주 학습된다．

              텐서플로우에서 공유 레이어shared Laye를 구현하기 위해서 작은 트릭trick을 써야 한다．
              완전 연결 레이어의 웨이트 매트릭스는 언제나 batch_size x in_size x out_size
              차원이다. 그러나 이제 우리는 매트릭스를 적용하고자 하는 두 개의 입력 차원을 가진
              다: batch_size와 sequence_steps.

              이 문제를 회피하기 위해서 우리가할수 있는 것은 입력을 레이어로 평탄화
                                                    （natten）
                                                           하
              는 것이다. 이 경우에 RNN의 출력 액티베이션은 batch_size x sequence_steps x
              in_size이다. 물론우리는다시unflatten하기 위해서 결과의 모양을바꿔야한다．


@lazy_property
def prediction(self):
    output, - = rnn.dynamic_rnn(
        GRUCell(self. params . mnn_hidden),
        self.data,
        dtype=tf. fioat32,
        sequence_length=self. length,
    )

    # Softmax Layer.
    max_length = int(self.target.get_shapeQ[l] )
    num_classes = int(self.target.get_shapeQ[2])
    weight = tf . Var'iable(tf. truncated_normal(




 2561   CHAPTER7 회귀 신경망과 자연 언어
                             （Recurrent Neural Networks and Natural Language)


===== PAGE 267 =====
       [sel-F.params_rnn_hidden, num_classes], stddev=0.01))
    bias = t-F.Variable(tf.constant(0.1, shape=[num_classes]))


   # FLatten to αPPLy same weights to aLL time stePS.
   output = tf.reshape(output, [-1, self.params.rrtn_hidden])
    prediction = t-F.nn.softmax(t-F.matmul(output, weight) + bias)
    prediction = tf.reshape(prediction, [-1, max-length, num_classes])
    return prediction


비용 함수와 에러 함수는 우리가 시퀀스 분류를 위해 했던 것으로 조금 바뀐다. 즉, 시퀀
스의 각 프레임은 예측－타겟 쌍이 있다. 그래서 우리는 그 차원 또한 평균을 구해야한
다. 그러나tf. reduce_mean( ）은 시퀀스의 최대 길이인 텐서 길이로 정규화하기 때문

에 동작하지 않는다. 대신 우리는 이전에 계산된 실제의 시퀀스 길이로 棚구화해야 한
다. 이를위해서, 우리는수작업으로t-F. reduce_sum( ）을사용하고 정확한평균을구

하기 위해서 나눗셈을 사용한다.


@lazy_property
def cost(self):
    # Compute cross entropy fOr each frame.
    cross_entropy = self.target * t-F.log(self.prediction)
    cross_entropy = -t-F.reduce_sum(cross_entropy, reduction_indices=2)
    mask = tf. sign(t-F.reduce_max(t-F.abs(self.target),reduction_indices=2))
    cross_entropy *= mask
    # 겨vera9e over αctuαL sequence Lengths.
    cross_entropy = tf. reduce_sum(cross_entropy, reduction_indices=1)
    cross_entropy 1= tF.cast(self.length, tf. fl0at32)
    return tf. reduce_mean(cross_entropy)


비용과 비슷하게 에러 함수를 조정해야 한다. t-F.argmax( ）가 수행되는 축은 이제 축
1이 아니라 축 2이다. 그리고 패딩 프레임을 매스크하고 실제 시퀀스의 길이로 평균을
구한다. 마지막의 tf. reduce_mean( ）은 배치 데이터에서 단어들의 평균이다．




                                                                  시퀀스 레이블링      - 257


===== PAGE 268 =====
@lazy_property
def error(self):
    mistakes=tf.not_equal(tf.argmax(self.target, 2),tf.argmax(self.prediction.,2))
    mistakes = tf.cast(mistakes, t-F.fi0at32)
    mask = tf.sign(t-f.reduce_max(tf.abs(sel-F.target),reduction_indices=2))
    mist訃ces *= ma針
                  （
    # Averaqe over actu요 sequence Lengths.
    mistakes = tf. reduce_sum(mistakes, reduction_indices=l)
    mistakes 1= tf. cast(self.length, tf. fl0at32)
    return t-F. reduce_mean(mistakes)



               텐서플로우의 자동 기울기 계산의 좋은 점은 비용 함수만 새로운 것으로 바꾸고 시퀀스
               분류를 위해 사용한 것과 동일한 최적화 연산을 사용할 수 있다는 점이다. 우리는 지금
               부터 모든 RNN에 기울기 자르기gradient cLipping를 할 것이다．
                                                         왜냐하면 부정적인 영향
               은 없으면서 학습동안발산을방지할수 있기 때문이다．


@lazy_property
def optimize(self):
    gradient = self. params.optimizer. compute_gradients(sel-F. cost)
    if self. params . gradient_clipping:
          limit = self. params.gradient_clipping
          gradient = [
              (t-F.clip_by_value(g, -limit, limit), v)
              if g is not None else (None, v)
              for g, v in gradient]
    optimize = self.params .optimizer.apply_gradients(gradient)
    return optimize




  258 -                        （Recurrent Neural Networks and Natural Language)
          CHAPTER7 회귀 신경망과 자연 언어


===== PAGE 269 =====
모델을 학습시키기


import random
from tensorfiow.mode1s.rnn import mnn
from terisorflow.models.rnn import mnn_cell


params = AttrDict(
    rnn_cell=rnn_cell .GRUCell,
    rnn_hidden=300,
    optimizer=t-f. train.RMSPropOptimizer(8. 882),
    gradient_clipping=5,
    batch_size=10,
    epoc갸is=20,
    epoch_size=50,
)

def get_datasetO:
    dataset = OcrDataset( '=/.dataset/booklocr')
    # FLatten images into vectors.
    dataset.data = dataset.data.reshape(dataset.data.shape[:2] + (-1,))
    # One-hot encode tar9ets.
    target = np. zeros(dataset.target. shape + (26,))
    for index, letter in np.ndenumerate(dataset.target):
        if letter:
            target[index][ord(letter) - ord( 'a')] = 1
    dataset.target = target
    # Shuffle order af exampLes.
    order = np. random.permutation(len(dataset.data))
    dataset.data = dataset.data[order]
    dataset.target = dataset.target[order]
    return dataset


# 치묘it into training and test data.
dataset = get_dataset()
split = int(0.66 * len(dataset.data))




                                                                시퀀스 레이블링   - 259


===== PAGE 270 =====
train_data, test_data = dataset.data[:split], dataset.data[split:]
train_target, test_target = dataset.target[:split], dataset.target[split:]


# Compute gra尸h.
-J length, image_size = train_data.shape
num_classes = train_target.shape[2]
data = t-F.placeholder(tf. fl0at32, [None, length, image_size])
target = tf. placeholder(tf. float32, [None, length, num_classes])
model = SequenceLabellingModel(data, target, params)



                                           LSTM Error on OCR Dataset
                       100%




                        10%




                         1%
                                     200         400       600         800   1000




              1000 단어를 학습한 후에 우리 모델은 테스트셋의 모든 문자 중 9％의 오분류를 보였다．
              그렇게 나쁜 결과는 아니다. 그러나 향상시킬 여지가 있다. 우리의 현재 모델은 시퀀스
              분류 모델과 아주 유사하다. 이것은 여러분이 지금의 모델을 새로운 작업에 적용할 때
              해야 하는 일을 확인할 수 있게 의도된 것이다. 다른 문제에 작동했던 방법이 대략적인
              추측을통해서 만들어진방법보다 새로운문제에 더 잘작동할 것이기 때문이다. 그러나
              더 좋은 시스템을 만들 수도 있다.
                               ＇다음 섹션에서 우리는 더 향상된 순환 구조로 우리의
              결과를 향상시킬 것이다．




 260 I   CHAPTER 7 회귀 신경망과 자연 언어
                               （Recurrent Neural Networks and Natural Language)


===== PAGE 271 =====
양 방향 RNNs(Bidirectional RNNs)

RNN과소프트맥스 구조를 이용한OCR 데이터셋 결과를 어떻게 향상시킬 수 있을까？
RNN을 사용하게 된 동기를 생각해보자. OCR 데이터셋에 RNN을 선택한 이유는 한
단어 속의 글자들사이에 의존정, 즉상호 연관된 정보가 있기 때문이다.RNN은자신의
히든 액티베이션에 같은단어의모든 과거 입력에 대한정보를 저장한다．

이 점을 생각하면, 우리 모델의 순환성은단어의 초반 몇 글자의 분류에는 그렇게 도움
되지 않는다. 왜냐하면 네트워크는 추론에 필요한 많은 입력을 아직 가지고 있지 않기
때문이다. 시퀀스분류에서는 네트워크가 결정을 내리기 전에 모든 프레임을 보기 때문
에 문제가 되지 않았다. 시퀀스 레이블링에서는 여러 분류문제에서 최신의 기법인 양방
향】NNbidirectiona1RNNs을사용함으로써 이단점을극복할수 있다．

양방향 RNN의 아이디어는 간단하다. 입력 시퀀스를 살펴보는 두 개의 RNN이 있다．
그 중에 하나는 왼쪽에서 오른쪽으로 읽고，
                      다른 하나는 반대로 읽는다. 각 타임 스텝에
공유 소프트맥스 레이어로 올리기 전에 이 두 개의 출력 액티베이션을 연결한다. 이 구
조를 이용한분류기는 각글자에서 전체 단어의 정보를 접근할수 있다．



                                                        w6
                                                   w3
                                              w6
                                         w3
                                    w6
                                w




                          양방향 RNN




                                                             시퀀스 레이블링   - 261


===== PAGE 272 =====
              텐서플로우에서 양방향 RNN을 어떻게 만들 수 있을까？ tf. model. mnn.
              bidirectional_mnn에 구현된 모델이 있다. 그러나 우리가 직접 복잡한 모델을 만드

              는방법을공부해보자．
                       단계별로 설명할 것이다．
                                   먼저 prediction 프라퍼티를두 개의 함
              수로 나누어서 살펴보자．


               @lazy_property
               def prediction(self):
                    output = sel-F._bidirectional_rnn(sel-F.data, sel-F.length)
                    num_classes = int(sel-F.target.get_shape()[2])
                    prediction = self._shared_softmax(output, num_classes)
                    return prediction


               def _bidirectional_rnn(self, data, length) :
                    pass


               def _shared_soFtmax(self, data, out_size):
                    pass



              _shared_softmax( ) 함수는쉽다．
                                      이전의 prediction프라퍼티에서 사용했었다．
                                                                차이
              점은 입력 크기를 함수에 주어지는 data 텐서에서 구한다는 점이다. 이런 방식으로, 필
              요하다면 다른 구조의 함수를 재사용할 수 있다. 그런 다음에 전체 타임 스텝 동안에 같
              은소프트맥스 레이어를공유하기 위해서 flattening 트릭을사용한다．


def _shared_softmax(sel-F, data, out_size):
    max_length = int(data.get_shapeQ[1])
    in_size = int(data.get_shape()[2])
    weight = t-F.Variable(t-F.truncated_normal([in_size, out_size], stddev=0.01))
    bias = t-F.Variable(t-f.constant(0.1, shape=[out_size]))
    # FLatten to app勻／ same weights to aLL time steps.
    flat = tf. reshape(data, [-1, in_size])
    output = tf. nn. so-Ftmax(tf. matmul(flat, weight) + bias)
    output = t-F.reshape(output, [-1, max_length, out_size])
    return output




 2621   CHAPTER7 회귀 신경망과 자연 언어
                             （Recurrent Neural Networks and Natural Language)


===== PAGE 273 =====
이제 흥미로운 양방향 RNN 구현 부분이다. mnn . dynamic_mnn으로 두 개의 RNN을
만든다. 전방향forward 네트워크는 익숙할 것이다. 역방향Ijackward 네트워크는 새로운 것

이다．

역방향 RNN으로 데이터를 단순히 입력하는 대신 시퀀스를 먼저 거꾸로 뒤집는다. 역
방향으로 움직이는 RNN 오퍼레이션을 작성하는 것보다 이 방법이 더 쉽다. 텐서플로
우는tf. reverse_sequence( ) 함수로사용한프레임들을 sequence_length까지
뒤집을 수 있다．
        함수는 길이가 64．
                  비트 정수형ntege
                            「 텐서라고 생각하지만，
                                        32．
                                          비트 텐
서에도 작동할 것이다. 단지 self,length만 전달하면 된다．


def _bidirectional_rnn(self, data, length):
    length_64 = tf. cast(length, tf. 1nt64)
    forward, - = rnn.dynamic_rnn(
        cell=self.params .rnn_cell(self.params .rnn_hidden),
        inputs=data,
        dtype=tf . float32,
        sequence_length=length,
        scope=' mnn-forward')
    ba아:ward, - = mnn . dynamic_mnn(
        cell=self params .rnn_cell(self.params .rnn_hidden),
        inputs=tf. reverse_sequence(data, length_64, seq_dim=1),
        dtype=tf. float32,
        sequence_length=self.length,
        scope=' mnn-backward')
    backward = tf. reverse_sequence(backward, length_64,seq_dim=1)
    output = tf. concat(2, [forward, backward])
    return output


                    왜 필요할까？3장 " 텐서플로우 기본" 에서 설명한
이번에 scope 파라미터를 사용한다．
바와 같이 계산 그래프의 노드는 이름을 가진다．
                         scope는 mnn · dynamic_cell에 의해

서 사용되는 변수 scope의 이름이다．
                     이번에 우리는 서로 다른 파라미터를 가진두 개의
RNN을사용하기 때문에, 그들은다른스코프에 있어야한다．




                                                                   시퀀스 레이블링   - 263


===== PAGE 274 =====
     역방향 RNN에 뒤집힌 시퀀스를 입력한후에, 출력 결과도 뒤집어서 전방향 네트워크
     의 결과와 맞춘다. RNN의 출력 뉴런의 차원을 따라서 두 개의 텐서를 붙인후 이를 출
     력한다. 예를들어, 배치 크기가50, RNN 마다300개의 히든유닛, 14개의 글자를 가진
     단어들이 있으면텐서의 크기는 50 x 14 x 600이 된다．

     여러 개의 RNN으로 구성된 첫 번째 구조를 완성했다. 지난 섹션의 학습 코드를 이용해
     서 어떻게 작동하는지 보자. 그래프를 비교해보면 양방향 모델이 조금 더 좋은 것을 알
     수 있다. 100개의단어를본후에, 테스트에서 4％만오분류가 있었다．


                         Bidirectional LSTM Error on OCR Dataset
              100%




               10%




                1%




     정리하면, 이번 섹션에서 우리는 시퀀스 레이블링을 위한 RNN 사용법과 시퀀스 분류
     와의 다른 점을 배웠다. RNN 출력을벋아서 전체 타임 스텝동안 공유되는분류기가 필

     요하다．

     이 구조는 역방향으로 진행되는 두 번째 RNN을 추가함으로써 확연하게 향상되었다．
     이것은 전체 시퀀스의 정보가 각글자의분류 과정에서 모두사용될수 있기 때문이다．

     다음 섹션에서 우리는 언어를학습하기 위해서 비지도unsupervised 형식으로 RNN을학
     습시킬 것이다．




CHAPTER 7 회귀 신경망과 자연 언어
                      （Recurrent Neural Networks and Natural Language)


===== PAGE 275 =====
Predictive Coding

우리는 이미 RNN을 이용하여 영화 비평의 감정을 분류하고, 필기체 단어를 인식하
는방법을 배웠다．
        이런 것들은 레이블링된 데이터셋을 사용하는 지도 학습supervised
learning이다．또다른 재미있는분야는predictive coding이라는 것으로써，
                                               많은 시퀀스
를RNN에게 보여주고 시퀀스의 다음프레임을 예측하게 학습시키는 것을말한다．

텍스트를 예를 들면, 한문장 안의 다음단어의 가능성LikeLihood을 예측하는 것을 언어 모
델링language modeling이라고 한다．
                         문장 속의 다음 단어를 예측하는 것이 왜 필요할까？
하나의 응용분야는 언어 인식〔anguage recognition이다．입력된 필기체를스캔해서 번역하
는 필기체 인식기를 만든다고 생각해보자. 입력에서 모든 단어들을 복원할 때, 다음단
어로올수 있는후보를 알수 있다면 문제가 훨씬 쉬워질 것이다．

자연어를 포함하는 일에서 성능을 향상시키는 것 이외에도 문장을 생성하기 위해서 네
트워크가 생각하는 다음단어의 분포를 샘플링할 수도 있다. 학습한 후에 RNN에 시드
seed 단어를 주고 다음 예측단어를 살펴보자. 그리고 가장 유망한단어를 RNN에게 다
음 입력으로 주고，
         그다음 번의 예측을 살펴보자. 이 과정을반복함으로써 학습 데이터
와유사한새로운 컨텐츠를 생성할수 있다．

         (is)   we    walked   down     the    street   <eos>




                       we      walked   down    the     street

        That    day

                회귀 언어 모델에서 시드를 이용한 샘플링




                                                                 Predictive Coding   I 265


===== PAGE 276 =====
     훙미로운 점은predictive coding은 신경망이 입력 시퀀스의 모든중요한 정보를 압축
     할수 있다는 점이다. 문장에서의 다음 단어는 일반적으로 이전의 단어들 그리고 그 단
     어들사이의 순서나관계에 의존한다. 자연어에서 다음글자를 정확하게 예측할수 있는
     신경망은문법과 언어의 특성을 파악해야한다．



     문자 단위 언어 모델링

     이제 우리는 RNN을 이용하여 predictive coding 언어 모델을 만들 것이다．
                                                     단어 단위
     로 작동하는 기존의 방법 대신에 우리는RNN이 개개의 글자단위로 동작하게 할 것이
     다. 그래서 입력으로단어 임베딩 대신에 알파벳, 마침표，
                                   빈칸등을포함하여 26보다약
     간많은 one-hot 인코딩된문자들을 가진다．

     단어 단위 언어 모델링이 글자단위보다 좋은방법으로 알려져 있다. 그런데, 문자단위
     의 좋은 점은 네트워크가 단어들을 조합하는 방법도 배우지만 단어의 스펠링도 배운다
     는 점이다. 또한, 우리의 신경망의 입력은 크기가300이거나 심지어 one-hot 인코딩 단
     어들을 사용하는 경우에 비해서 낮은 차원이다. 보너스로 이제 우리는 더 이상 모르는
     단어를 신경쓸 필요가 없다. 그 단어들도 신경망이 이미 알고 있는 글자들로 구성해 주
     기 때문이다. 이론적으로 이것은 네트워크가새로운단어도만들수 있도록 해준다.

     Andrew Karpathy는 2015년에 RNN의 글자단위 실험에서 놀랍게도 세익스피어 대
     본의 멋진 샘플들과 리눅스 커널과 드라이버 코드，
                               마크업 문법까지 정확한 위키피디아
     글을 생성하였다．
             이 프로젝트는 Github http://github.com/karpathy/char-rnn에 있다．
     우리는 이와 비슷한모델을 머신 러닝 논문들의 초록에 적용해서 그럴듯한 새로운 초록
     을생성할수 있는지 볼 것이다．



     ArXiv 초록 Api

     ArXiv.org는 컴퓨터 사이언스， 물리학，
                        수학，  생물학 분야의 많은 연구 논문을 호스팅
     하는온라인 도서관이다. 머신 러닝 연구를공부한다면 들어봤을수도 있을 것이다. 다



CHAPTER 7 회 갸 신경망과 자연 언어
                       （Recurrent Neural Networks and Natural Language)


===== PAGE 277 =====
행스럽게도 이 플랫폼은논문검색을위해서 웹 기반시'I를 제공한다．
                                  특정 쿼리query어I
대해서 Arxiv에서 초록을 가져오는클쾌스를작성하자．


import requests
import os
from bs4 import Beauti-fulSoup


class ArxivAbstracts:


    def _init_    (self, cache_dir, categories, keywords, amount=None):
        pass


    def _fetch_ali (self, amount) :
        pass


    def _fet야i_page(self, amount, offset) :
        paSS


    def -fetch-count(self):
        pass


    def _build_url (self, amount, offset):
        pass



생성자부분에서 사용 가능한초록의 이전 덤프가 이미 있는지 체크해서, 있다면 API를
사용하는 대신 그것을 사용할 것이다. 존재하는 파일이 새로운 카테고리나 키워드와매
칭되는지 체크하는 좀 더 복잡한 로직을 생각할 수도 있다. 그러나 지금 당장은 새로운

쿼리를 수행하기 위해서 예전의 덤프를 지우거나 옮기는 것만으로도 충분하다. 덤프
가 존재하지 않는다면 -fetch-all ( ) 메소드를 호출하고 제공받는 줄 들 을 디스크
에쓴다．




                                                                 Predictive Coding   I 267


===== PAGE 278 =====
                 def - mnit-(self, cache_dir, categories, keywords, amount=None):
                    self.categories = categories
                    selfJ:eywords = keywords
                    cache_dir = os. path.expanduser(cache_dir)
                    ensure_directory(cache_dir)
                    filename = os.path.join(cache_dir, 'abstracts.txt')
                    if not os.path.isfile(filename):
                        with open(filename, 'w') as file_:
                              for abstract in self._fetch_all(amount):
                                   file_.write(abstract + ' \n')
                    with open(filename) as file_:
                           self.data = file_.readlines()



              우리는 머신 러닝 논문에 관심이 있기 때문에 ^4achine Learning, Neural and

              Evolutionary Computing, Optimization and Control 카테고리에서 검색할 것이다．
                                                                             이

              결과에서도 메타 데이터에 'ieural, network, deep 단어를 포함한 결과를 사용하자．
                                                                   이렇

              게 해서 하나의 간단한RNN 언어 모델을 학습하기에 적당한 7 MB의 텍스트를 구할수
              있었다. 더 많은 데이터를 사용해서 더 좋은 결과를 얻을수 있을 것이다. 그러나 어떤 결
              과를 눈으로 보기 전에 너무 많은 시간을 기다리고 싶지 않았다. 더 많은 쿼리를 사용해
              보고 그다음에 더 많은데이터로 학습시켜보자．


ENDPOINT = 'http://export.arxiv.org/api/query'


def _build_url(self, amount, offset):
    categories = ' OR ' .join( 'cat: ' + x for x in self.categories)
    keywords = ' OR ' .join( 'all: ' + x for x in self.keywords)
    un1 = type(self).ENDPOINT
    url += '?search_query=(({}) AND ({})) ' .format(categonies, keywords)
    unl += '&max_results={}&offset={}' .format(amount, offset)
    return url


def _-Fetch_count(self):
    url = self._build_url(0, 0)




  2681                        （Recurrent Neural Networks and Natural Language)
         CHAPTER7 회귀 신경망과 자연 언어


===== PAGE 279 =====
     response = requests.get(url)
    soup = BeautifulSoup(response.text, ' lxrnl')
     count = int(soup.find( 'opensearch:totalresults').string)
     print(count, 'papers -found')
     return count


_-Fetch_all( ) 메소드는 기본적으로 pagination을 수행한다．API는 각 요청「equest

에 대해서 정해진 양의 abstract를 제공해주고 두 번째，
                                 세 번째，
                                     기타 " page" 결과를 얻
기 위해 걸릴 시간의 차이offset를 정할수 있다．
                            이론적으로 페이지 크기page size를 아주
큰 숫자로 정해서 모든 결과를 한 번에 얻으려고 할 수도 있다. 그러나 실제로는 이러한

방법은 요청을 매우 느리게 한다．
                 페이지를 페칭fetching하는 것은 더욱 오류가 적고fault
tolerant, 가장중요한 점은 Arxiv API에 스트레스를많이 주지 않는다는장점이 있다．


 PAGE SIZE = 100


def _fetch_all (self, amount):
    page_size = type(self).PAGE_SIZE
     count = self._fetch_count()
    if amount:
         count = min(count, amount)
    for offset in range(0, count, page_size):
        print( 'Fetch papers {}/{}' .format(offset + page_size, count))
         yield from self._fetch_page(page_size, count)


여기서 실제적인 페칭을 해보자. 결과는XML 형식으로 나오는데, 초록을 추출하기 위
해서 많이 사용하며 강력한 기능의 BeautifulSoup 라이브러리를 사용한다．
                                            이미 설치
되어 있지 않다면아래와같이 설치하자．

  sudo -H p1p3 install beautifulsoup4

BeautifulSoup은 )(ML을 파싱해서 우리가 관심있는 태그tag에 대해서 쉽게 반복적으
로 수행할 수 있게 한다. 출판물과 연관된 <entry> 태그를 찾아서 각 아이템마다 초록
을 포함하고 있는 <summary> 태그를 읽는다．



                                                                 Predictive Coding   - 269


===== PAGE 280 =====
                 def _fetch_page(self, amount, offset):
                     un1 = self._build_url(amount, offset)
                     response = requests.get(unl)
                     soup = BeautifulSoup(response.text)
                     for entry in soup.findAll( 'entry'):
                         text = entry.find( 'summary').text
                         text = text.stnipQ.replace( '\n',      ')
                         yield text




                데이터 전처리
                      （Preprocessing the Data)


import random
import numpy as np


class Preprocessing:


    VOCABULARY = \
        " $%' 0-i-, - ./0123456789: ;=?ABCDEFGHIJKLMNOPQRSTUVlJXYZ" \
        "\ \A-abcdefghijklmnopqrstuvwxyz{ I


    def _init_    (self, texts, length, batch_size):
        self.texts = texts
        self.length = length
        self.batch size = batch size
        self.lookup = {x: i for i, x in enumerate(self.VOCABULARY)}


    def __call_(self, texts):
        batch = np.zeros((len(texts), self.length, len(self.VOCABULARY)))
        for index, text in enumerate(texts):
            text = [x for x in text if x in self.lookup]
            assert 2 <= len(text) <= self.length
            for offset, character in enumerate(text):
                  code = self.lookup[character]




 2701   CHAPTER7 회귀 신경망과 자연 언어
                             （Recurrent Neural Networks and Natural Language)


===== PAGE 281 =====
                 batch[index, offset, code] = 1
         return batch


     def _iter_(self):
         windows = []
         for text in self.texts:
             for i in range(0, len(text) - self.length + 1,self.length II 2):
                 windows.append(text[i: i + self.length])
         assert all(len(x) == len(windows[0]) for x in windows)
         while True:
             random.shuffle(windows)
             for i in range(e, len(windows), self.batch_size):
                 batch = windows{i: i + self.batch_size]
                 yield self(batch)




Predictive Coding Model

이제 우리는 전체 과정을 알고 있다. 우리의 작업을 정의하고, 데이터셋을 얻기 위한 파
서를 작성하고，
       텐서플로우에서 신경망 모델을 구현할 것이다．
                              predictive coding을 위
해서 우리는 입력 시퀀스의 다음 문자를 예측하기 때문에, 모델에의 입력은 생성자의

sequence 파라미터 뿐이다．

생성자는 중간 부분에서 옵션을 수정하기 위해서 파라미터 오브젝트를 받아서 우리의
실험을 재 반복할수 있게 한다. 세 번째 파라미터 initial=None은순환 레이어의 초기
inner activation이다. 텐서플로우가 은닉 상태를 zero 덴서로 초기화하면서, 학습된 언
어 모델에서 샘플을만들때 다루기 쉽게 해준다．

 import tenso에ow as tf
 from tensorflow.models.rnn import mnn
 from tensorflow.models.rnn import mnn_cell
 from utility import lazy_property




                                                                  Predictive Coding   I 271


===== PAGE 282 =====
               class PredictiveCodingModel:


                   def _init_(self, params, sequence, initial=None):
                       self.pararns = params
                       self.sequence = sequence
                       self.initial = initial
                       self.prediction
                       self.state
                       self.cost
                       self.error
                       self.logprob
                       self.optimize


                   @lazy_property
                   def data(self):
                       pass


                   @lazy_property
                   def target(self):
                       pass


                   @lazy_property
                   d이＝ mask(self):
                       pass


                   @lazy_property
                   def length(self):
                       pass


                   @lazy_property
                   def prediction(self):
                       pass


                   @lazy_property
                   def state(self):
                       pass




272 I   CHAPTER 7 회귀 신경망과 자연 언어
                              （Recurrent Neural Networks and Natural Language)


===== PAGE 283 =====
   @lazy_property
   def forward(selF):
       pa55


   @lazy_property
   def cost(self):
       pass


   @lazy_property
   def error(self):
       pass


   @1azy_p roperty
   def logprob(self):
       paS5


   @lazy_property
   def optimize(self):
       pa弱


   def _average(self, data) :
       pass



위의 예제 코드에서 우리 모델이 구현할 함수들의 개괄을 살펴볼 수 있다. 첫눈에 너무

부담을 가지지 않아도 된다. 먼저 입력 데이터를 생성하고 그것으로부터 타겟 시퀀스
를 만들자. 타임 스텝 t에서 모델은 문자 SI를 입력으로 st+1을 타겟으로 가진다．
                                               data와

target을 얻는 쉬운 방법은 제공된 시퀀스를 조각 내서 첫 번째나마지막 프레임을잘

라버리는것이다．

tf. slice( ）는 시퀀스，
                 각차원에 대한시작 인덱스, 각차원을 위한크기를받아서 슬
라이스를 낸다. sizes-i은그 차원에서 시작 인덱스에서 끝까지의 모든 요소를 포함하
     , 프레임 단위로슬라이스하기 위해서 2차원만고려한다．
기 때문어］




                                              Predictive Coding   273


===== PAGE 284 =====
@lazy_property
def data(self):
    max_length = int(self.sequence.get-shapeQ[1])
    return tf.slice(sel-F.sequence, (0, 0, 0), (-1, max_length


@lazy_property
def target(self):
    return tf.slice(self.sequence, (0, 1, 0), (-1, -1, - ))


@lazy_property
deF mask(self):
    return tf.reduce_max(t-F.abs(sel-f.target), reduction_indices= )


@lazy_property
def length(self):
    return tf.reduce_sum(self.mask, reductlon_indices=1)


             타겟 시퀀스의 프라퍼티를2개 정의한다. mask는 크기가 batch_size x max_length
             인텐서인데 respective 프레임이 사용되는지 패딩 프레임이 사용되는지에 따라서 0 또
             는 1값을 가진다. length 프라퍼티는 각 시퀀스의 길이를 구하기 위해서 시간축 상의
             마스크를합한다．

                                            개념적으로는타겟 시퀀스와동
             mask와length 프라퍼티는 데이터 시퀀스에 유효한데，
             일한 길이이기 때문이다. 그러나 예측할다음문자가 없는마지막프레임을포함하고 있
             기 때문에, 데이터 시퀀스어］대해서 계산할수 없다. 데이터 텐서의 마지막프레임을삭
             제했기 때문에 대부분의 시퀀스의 실제적인 마지막 프레임이 없다. 이것이 우리가 아래
             에서 mask를 사용하는 이유이다．

             우리는 순환 네트워크와 공유되는 softmax 레이어를 가지는 실제적인 네트워크를 정
             의할 것이다. 이전섹션에서 시퀀스 레이블링을 위해서 사용했던 것과동일한구조이다．
             공유 소프트맥스 레이어의 코드는 소개하지 않을 것이다. 필요하다면 이전 섹션에서 찾
             아보자．




 27시    CHAPTER 7   H'1 신경망과 자연 언어
                                 （Recurrent Neural Networks and Natural Language)


===== PAGE 285 =====
@lazy_property
def prediction(self):
    prediction, - = sel-F.forward
    return prediction


@lazy_property
def state(self):
   -, state = self.forward
    return state


@lazy_property
def forward(self):
    cell = self. pararns.rnn_cell(sel-f.params. mnn_hidden)
    cell = rnn_cell.MultiRNNCell([cell] * self. params. mnn_layers)
    hidden, state = rnn.dynamic_rnn(
        inputs=self.data,
        cell=cell,
        dtype=tf.float32,
        initial_state=self.initial,
        sequence_length=self.length)
    vocabulary_size = int(self.target.get_shapeQ[2])
    prediction = self._shared_softmax(hidden,vocabulary_size)
    return prediction, state


위의 신경망 코드의 새로운 부분은 예측과 마지막 순환 액티베이션을 구한다는 것이다．

이전에 우리는 예측만 구했었다. 그러나 마지막 액티베이션은 이후에 시퀀스를 더욱 효
과적으로 만들 수 있도록 해준다. 한 번만에 순환 네트워크의 그래프를 만들고 싶기 때
문에 텐서와prediction, state을반환하는forward 프라퍼티가 있다．

우리 모델의 다음 부분은 cost와 evaluation 함수이다. 각 타임 스텝에서 모델은 단어
집의 다음 문자를 예측한다. 이것은 분류 문제이고 따라서 크로스 엔트로피 비용cross
                 문자 예측의 에러율을 쉽게 구할수 있다．
entropy cost을사용한다．

logprob 프라퍼티는 새로운 것으로써，       （logarithmic) 공간에서 정확한
                      우리 모델이 로그




                                                                Predictive Coding   I 275


===== PAGE 286 =====
              다음문자를 예측할확률을 제공한다. 이것은 기본적으로는 로그 공간에서 평균을구한
                                      그 결과를 선형 공간으로 변경한 것이 perplexity이다．
              negative cross entropy이다．                                이
              는 언어 모델의 성능을 평가하기 위한 일반적인 기준measure이다．

              직관적으로 perplexity는 큰 말뭉치에서 다음 문자를 얼마나 잘 예측하는지를 보여준
               perplexity가 1이면 정확한 것이고，
              다．                                         perplexity
                                      더 큰 값은 성능이 나빠지는 것이다．
              는 다음 문자의 확률에 0을 제시하면 심지어 무한대nfinity일 수 있다．
                                                       예측 확률을 매우
              작은 양수와1 사이의 값으로 제한함으로써 이런 극단적인 경우를 방지한다．


@lazy_property
def cost(self):
    prediction = tf. clip_by_value(sel-F.prediction, le-10, 1.0)
    cost = self.target * tf. log(prediction)
    cost = -t-f.reduce_sum(cost, reduction_indices=2)
    return self._average(cost)


@lazy_property
    def error(self):
        error = tF.not_equal(t-F.argmax(self.prediction, 2),t-F.argmax(self.target,   2)   )
        error = tf. cast(error, tf. float32)
        return sel-F._average(error)

@lazy_property
def logprob(self):
    logprob = tf. mul(selF.prediction, sel-F.target)
    logprob = t-F. reduce_max(logprob, reduction_indices=2)
    logprob = tf. log(tf. clip_by_value(logprob, le-lO, 1.0)) I t-F.log(2.0)
    return sel-f._average(logprob)

def _average(self, data) :
    data *= self.mask
    length = t-F.reduce_sum(self.length, 1)
    data = t-F.reduce_sum(data, reduction_indices=l) I length
    data = t-F. reduce_mean(data)
    return data




 27이                          （Recurrent Neural Networks and Natural Language)
        CHAPTER 7 회귀 신경망과 자연 언어


===== PAGE 287 =====
앞의 3개의 프라퍼티 모두가 모든 시퀀스의 프레임에 대해서 평균을 구한다. 고정 길이
fixed-Length의 시퀀스에서는한 번의 tf. reduce_mean( ）으로 구할수 있지만，
                                                     가변 길
이variable-length에 대해서는 조금 더 주의해야 한다．
                                   첫째，
                                     패딩 프레임에 매스크를 곱하
고, 프레임 사이즈에 대해서 합친다 ．위의 3 함수는 모두 타켓과 곱하기 때문에 각 프레
임은 하나의 요소만 가지고 있고, tf. reduce_sum( ）으로 각 프레임을 하나의 스칼라
값으로만들수 있다．

다음으로，
    각 시퀀스의 프레임을따라 실제 시퀀스 길이를 이용해서 평균을구하려고한
다. 빈시퀀스인 경우에 0으로 나누는 것을방지하기 위해서 시퀀스 길이와1 중의큰값
을사용한다. 결론적으로 tf. reduce mean( ）을 사용함으로써 배치로 예제들의 평균
을구할수 있다．

이제 바로 이 모델을학습하는 이야기로 넘어가보자．
                          아직 optimize 오퍼레이션을 정의
하지 않았는데, 이 장의 앞 부분에 시퀀스 분류나 시퀀스 레이블링에 사용된 것과 동일
하다．



모델 학습하기

우리의 언어 모델에서 샘플링하기 전에，
                    우리가 방금 만든 블록들
                                （데이터셋，
                                     전처리
단계，
  신경망）
     을 모두 합쳐야 한다．
                이런 단계들을 합치고，
                           새롭게 소개된 perplexity
measure를출력하고, 정기적으로학습 진행 정도를 저장하는클래스를작성하자. 이러
한방법은 학습을 계속할 때 유용하며, 샘플링을 위해서 학습된 모델을 시작할 때도 편
리하다．


 import os


 class Training:


    @overwrite_graph
    def _init_     (selF, params) :




                                                   Predictive Coding   I 277


===== PAGE 288 =====
        self.params = params
        self.texts = ArxivAbstracts( '/home/user/dataset/arxiv')()
        self.prep = Preprocessing(
        self.texts, self. params.max_length,self. params.batch_size)
        self.sequence = tf.placeholder( tf.float32, [None,
        self. params.max_length, len(self. prep.VOCABULARY)])
        self.model = PredictiveCodingModel(self. params, self.sequence)
        self.-mnit-or-load-session( )


  def _call_(self):
        print( 'Start training')
        self.logprobs = [1
        batches = iter(self.prep)
        for epoch in range(self.epoch, self.params.epochs + 1):
            self.epoch = epoch
            for - in range(self.params.epoch_size):
                self._optimization(next(batches))
            self._evaluation()
        return np.array(self.logprobs)


  def _optimization(self, batch):
        logprob, - = self.sess.run((self.model.logprob, self.model.optimize),
           {self.sequence: batch})
        if np.isnan(logprob):
            raise Exception( 'training diverged')
        self.logprobs.append(logprob)


  def _evaluation(sel-F):
        self.saver.save(self.sess, os.path.join(
        self.params.checkpoint_dir, 'model'), self.epoch)
        self.saver.save(self.sess, os.path.jomn(
        self.params.checkpoint_dir, 'model'), self.epoch)
        perplexity = 2 ** -(sum(self.logprobs[-self.params.epoch_size:]) I
        self.params.epoch_size)
        print( 'Epoch {:2d} perplexity {:5.lf}'.format(self.epoch, perplexity))




278 -   CHAPTER 7 회귀 신경망과 자연 언어
                              （Recurrent Neural Networks and Natural Language)


===== PAGE 289 =====
    def _init_or_load_session(self):
        self.sess = 奸．
                     Session()
        sel-F. saver = t-f.train.Saver()
        checkpoint = tf. train.get_checkpoint_state(self.params. checkpoint_dir)
       if checkpoint and checkpoint,model_checkpoint_path:
            path = checkpoint,model_checkpoint_path
            print( 'Load checkpoint', path)
            self.saver. restore(self.sess, patD
            self.epoch = int(re.search(r'-(\d+)$',path).group(l) ) + 1
        else:
            ensure_directory(self.params . checkpoint_dir)
            print( 'Randomly initialize variables')
            self. sess. run(tf. initialize_afl_variablesQ)
            seh믹이Doch = 1



생성자－call_( ), _optimization( ), _evaluation( ）은이해하기 쉽다. 데이터
셋을로드하고 그래프를 계산할 입력을 정의하고, 전처리된 데이터셋을 학습하고, 로그

 ［ogarithmic probabiLity을 추적한대 ㅁㅐ 학습 단계에서 perplexity를 계산하고 출력하
확률
기 위해서 평가 시점에 이것들을사용한다．

_init_or_load-session( ）에서 그래프에서 모든tf.Variable( ）의 현재값을 저

장하는t-F.train.SaveN ）를소개한다. 실제의 체크포인팅은－evaluation( ）에

서 수행되지만, 여기서 클래스를 만들고 로딩할 체크포인트를 찾는다. tf.train.get-
래eckpoint_state( ）는체크포인트 디렉터리에서 텐서플로우의 메타 데이터 파일을

찾는다. 책을 쓰는 시점에 가장 덜 최근에［east recent사용된 체크포인트 파일을 보관
한다．

체크포인트 파일은우리가 지정할수 있는숫자에 의해서 정해진다. 우리의 경우는반복

세대epoch 숫자이다．
            체크포인트를 로딩할 때 반복 횟수를 추출하기 위해서 파이썬의 re

패키지의 정규식                       체크포인트를 위한로직을만들고 학습을
       「egular expression을 적용한다．
시작할수 있다. 다음은 이를 위한환경 설정이다．




                                                                Predictive Coding   - 279


===== PAGE 290 =====
              def get_paramsO:
                  checkpoint_dir = ' /home/user/rnodel/arxiv-predictivecoding'
                  max_length = 50
                  sampling_temperature = 0.7
                  mnn cell = GRUCell
                  mnn hidden = 200
                  mnn_layers = 2
                  learning_rate = 0.002
                  optimizer = tf.train.AdamOptimizer
                  gradient_clipping = 5
                  batch size = 100
                  epochs = 20
                  epoch_size = 200
                  return AttrDict(**localsO)


            이 코드를 실행하기 위해서 Training(get_pa rams ( ))( ）를 호출하자. 나의 노트북
            에서 20번 반복에 1시간이 걸렸다. 이 학습 동안 모델은 20번 반복 × 200 배치 × 100

            예제 × 50문자 = 20M문자를보았다．


                                 ArXiv Predictive Coding Perplexity




                                500   1000 1500 2000 2500 3000 3500 4000



            그래프에서 볼 수 있는 바와 같이 모델은 문자당 약 1.5의 perplexity로 수렴한다．
                                                              이말
            은우리 모델은문자당 평균 1.5비트로 압축할수 있다는 것을 의미한다．




2801   CHAPTER7 회귀 신경망과 자연 언어
                            （Recurrent Neural Networks and Natural Language)


===== PAGE 291 =====
단어단위 언어 모델과 비교하여 문자 갯수보다단어 갯수로 평균을 해보자. 대략적으로
계산하면, 단어당 평균 문자 갯수로 곱해서 구할수 있다．



유사한 시퀀스를 생성하기

이제 우리는학습된 모델을사용해서 새로운시퀀스를만들수 있다．
                               Training 클래스와
유사한작은클래스를만들 것이다. 이 클래스는 디스크에서 가장 최근의 모델 체크포인
트를로드하고，
      데이터를 계산그래프에 입력하기 위해서 플레이스홀더placeholde틀 정
의한다. 물론 지금은 모델을 학습시키지 않고 새로운 데이터를 생성하기 위해서 사용하
는것이다．

class Sampling:


   @overwrite_gra아1
    def    init_ (self, params) :
          pass


    def - call- (self, seed, length):
          pass


    clef _sample(self, dist) :
          paSS



생성자에서는 현재 생성된 시퀀스를 그래프에 입력할 Numpy 벡터로 변환하기 위한
전처리 클래스의 인스턴스를 생성한다. 이를 위한 시퀀스 플레이스홀더는 동시에 여러
개의 시퀀스를 생성하지는 않기 때문에 배치batch 마다 하나의 시퀀스만가지면 된다．

모델은 입력 데이터의 마지막글자만빼고 모두 사용하며, 타겟으로는 첫 글자만 제외하
고 모두 사용한다. 현재 텍스트의 마지막 글자와 두 번째 글자를 시퀀스로 입력한다. 네
트워크는 첫글자를 위한타겟을 예측하는데, 두 번째 글자가타겟으로사용된다．




                                           Predictive Coding   - 281


===== PAGE 292 =====
               현재 텍스트의 마지막글자를 네트워크에 어떻게 전해줄지 의아할 것이다. 회귀 신경망
               의 마지막 액티베이션 값을 얻고, 이를 다음 번실행에서 상태를 초기화하는데 사용하는
               방식으로 해결한다. 이를 위해서 모델의 초기 상태 파라미터를 사용한다. GRUCell에서
               상태는「nfl_layers * mnn_units 크기의 벡터이다．


@overwrite_graph
def __init_ (self, params, length) :
    self.params = params
    self.prep = Preprocessing([], 2, self.params.batch_size)
    self.sequence = tf. placeholder(tf. fl0at32, [1, 2, len(self.prep.VOCABULARY)])
    self.state = tf. placeholder(tf. fl0at32) [1, self.params.mnn_hidden *
         self.params . mnn_layers])
    self.model = PredictiveCodingModel(self params, self.sequence, self.state)
    self.sess = tf. Session()
    checkpoint = tf. train.get_checkpoint_state(self.params .checkpoint_dir)
    if checkpoint and checkpoint .model_checkpoint_path:
         tf. train.Saver() . restore(
             self. sess, checkpoint .model_checkpoint_path)
    else:
         print( 'Sampling from untrained model. ' )
    print( 'Sampling temperature ' , self.params .sampling_temperature)


               _call_ ( ) 함수는 여러 문자들의 샘플링 시퀀스를 위한논리를 정의한다. 우리 모델

               은 배치 데이터에 작동하도록 정의되기 때문에 여러 시퀀스를 동시에 생성할 수 있다．
               현재의 텍스트들을 패딩된 Numpy 블록으로 변환하고 이를 네트워크에 입력하는동일
               한 전처리 클래스를 사용하자. 배치에서 하나의 출력 프레임에 하나의 시퀀스가 있기 때
                           에서만 예측한다. 그리고－sample( ) 함수를사용해서 소프트맥ㅅ
               문에 인덱스 [0, 0］
               출력에서 샘플을만들어낸다．




 282 -   CHAPTER 7 회귀 신경망과 자연 언어
                               （Recurrent Neural Networks and Natural Language)


===== PAGE 293 =====
def ---call-(self, seed, length=100):
   text = seed
   state = np.zeros(( , self.params.rnn_hidden * sel-f.params.rnn_layers))
   for - in range(length):
       feed = {self.state: state}
       -Feed{self.sequence] = self.prep([text[- ] +   '   ? ])
        prediction, state = selF.sess.run([self.model.prediction,
           self.model.state], feed)
       text += self._sample(prediction[ ,   〕）
   return text



네크워크 출력에서 어떻게 샘플을만들수 있을까？이전에 가장 좋은 예측값을 다음프
레임의 입력으로 넣음으로써 시퀀스를 생성할 수 있다고 했었다. 실제로는 가장 그럴듯
한다음 프레임을 선택하는 것이 아니라，
                    RNN의출력 결과인 확률 분포에서 랜덤하게
샘플링한다. 이런방식으로 높은출력 확률값이 많이 선택되기는 하지만, 적은확률값의
출력도 여전히 선택될 가능성이 있게 된다. 이를 통해서 결과 시퀀스가 좀 더 다이나믹
                  동일한 평균적인 시퀀스만 계속 반복적으로 생성될 것
dynamic해진다．그렇지 않으면，
이다．

이러한 생성 프로세스가 얼마나 도움이 되는지를 수작업으로 조절하는 간단한 메커니
즘이 있다．
     예를 들어，
          다음 단어를 언제나 랜덤하게 선택한다면
                              （네트워크의 출력값을
완전히 무시하고）
        , 완전히 새롭고 독특한문장을 얻을 것이다. 그렇지만 이는 의미가 없
는 문장일 수도 있다. 만약 네트워크의 가장 높은 출력값만 언제나 선택한다면, 가장자
주나타나지만별의미가없는" the" ,''a" 와같은단어만얻을수도있다．

                                        소프트맥스 레이어
"temperature 7"'라는 파라미터를 사용함으로써 이를 조절해보자．
에서 출력 분포의 예측값을 더욱 비슷하게 또는더욱 급진적으로만들 파라미터이다. 이
를통해서 스펙트럼의 한편에서는흥미롭지만 랜덤 시퀀스가생성되거나, 다른 한편에
서는그럴듯 하지만 지루한 시퀀스를 얻을 수 있다．
                          이 방법은 선형 공간linear space에서
출력값을 크기를 조절하는 것이다．
                 이 값들을 지수 공간exponential space으로 옮겨서 정




                                                                 Predictive Coding   - 283


===== PAGE 294 =====
             규화normaUze를 다시 한다：




                        끄
                        （차）=        ',
                                   27『（ IT



             네트워크가 이미 소프트맥스 분포를 출력하기 때문에，
                                        자연 로그natural togarithm을 적용

             해서 이를 되돌린다. 출력 결과를다시 정규화할 것이라서 斗干화를 다시 되돌릴 필요는

               각 값을 설정된 temperature 값으로 나누고 추ㅍㅌ맥ㅅ 함수를다시 적용한다．
             없다．


              def _sample(self, dist):
                   dist = np.log(dist) I self.params. sampling_temperature
                   dist = np. exp(dist) I np.exp(dist).sum()
                   choice = np. random.choice(len(dist), p=dist)
                   choice = self. prep.VOCABULARY[choice]
                   return choice



             Sampling(get_params( ) )( 'We', 500) ）을호출해서 네크워크가새로운초록을

             생성하도록 실행해보자．

                We study nonconvex encoder in the networks (RFNs) hasding
                configurations wi洲
                non-convex large-layers of images, each directions literatic
                for layers. More
                recent results competitive strategy, in which data at
                training and more
                difficult to parallelize. Recent Newutic systems, the
                desirmally parametrically
                in the DNNs improves optimization technique, we extend their
                important and
                subset of theidesteding and dast and scale in recent
                advances in sparse
                recovery to complicated patterns of the $L-p$




284 -   CHAPTER7 회귀 신경망과 자연 언어
                             （Recurrent Neural Networks and Natural Language)


===== PAGE 295 =====
실제 사용하기


                 ' 'V.嚆未 .Co4
 移冬也□聊쓰
 ㅈ，■■■ . 四 -1 ia@ 盞，I I




”聲韆_-掛
  'w   -   z二」   r'


===== PAGE 296 =====
              이제까지 우리는 텐서플로우를 이용해서 기본적인 머신 러닝 모델부터 복잡한 딥 러닝
              네트워크까지의 모델을 만들고 학습시키는방법을 살펴보았다. 이 장에서는 학습된 모
              델을 실제로다른 앱에서 사용할수 있는방법에 집중해보자．

              우리의 목표는 간단한 웹앱webapp을 만들어서 사용자가 이미지를 업로드하면 분류를
              위해서 우리의 학습된 모델을수행하는 것이다．




              학습된 모델

              모델의학습과평가가끝나면，
                          사용하기 위해서 모델의 그래프와값들을출력export한다．

              모델의 그래프는학습 버전에서 조금수정을 해야하는데, 입력 값을플레이스홀더에 보
              관하고 결과를 계산하기 위해서 추론 과정을한스텝 수행한다. 일반적으로 이미지 인식
              작업에서 입력값은IPEG 인코딩된 이미지를 의미하는 하나의 문자열로 표현된다．
                                                        이렇
              게 하면 실제의 사용 앱에서 데이터를 쉽게 전달할 수 있다. 이 과정이 TFRecords 파일
              에서 입력을벋아들이는학습단계와다른점이다．

              입력을 위한코드는아래와같다·．


def inference(x):
    # frα刃 the originaL ＇刃
                         《棘eL. . .


def convert_external_inputs(external_x):
    # transform the externaL input to the input format required on inference
    external_x = t-F. placeholder(tf. string)
    x = convert_external_inputs(x)
    y = inference(x)


              위의 코드에서 입력을 위한플레이스홀더를 정의하였다. 플레이스홀더에의 입력값을
              원래의 추론모델어I 필요한 형태로 바꾸는함수를 호출한다．
                                            예를 들어, JPEG 문자열을
              추론에 필요한 이미지 형태로바꾸는 것이다. 마지막으로，
                                           변환된 입력으로 원래의 추론




 286 -   CRAPTER8 실제 사용하기


===== PAGE 297 =====
모델을수행한다．

추론모델은 파라미터를 위한값이 필요하다. 이 값들은 학습 체크포인트에서 구할수

있다. 학습 동안에 중간 중간에 모델의 파라미터들을 체크포인트 파일에 저장해두었기

때문이다. 이 파일에는 그 당시의 파라미터들의 값이 포함되어 있기 때문에, 사고가발

생하더라고 학습내용을 잃어버리지 않게 된다．

학습이 끝나면, 마지막의 체크포인트 파일에 가장 최근의 모델 파라미터가 있고, 이를

실전에 사용한다．

체크포인트에서 정보를 가져오기 위한 코드는 아래와 같다：


 saver = tf.train.Saver()


 with tf.Session() as sess:
     # Restore varLabLes fr아r) tra-LnLng checkpoints.
     ckpt = tf.train.get_checkpoint_state(os.path.dirname(jile_ ))
     if ckpt and ckpt.model_checkpoint_path:
         saver. restore(sess, ckpt.model_checkpoint_path)
     else:
         print("Checkpoint file not found")
         return


추론모델은 아래에서 미리 학습된 체크포인트를다운로드할수 있다；httpi/download.

tenso胛ow.org/models/image/imagenet/inception-v3-2016-03-01.tar.gz

마지막으로, tensorflow_serving. session_bundle. exporter. Exporte
                                                           「 클래

스로 엑스포트한다. saver 인스턴스를 전달해서 인스턴스를 만들 수 있다. 그리고

exporter. classification--signature 메추ㄷ 쿠 모델의 시그니처signature를 만들어

야한다. 시그니처는 어느 것이 input_tenso
                           「인지, 어느 것이 output_tenso
                                                 「인지를

정의한다. 출력은출력 클래스 이름의 리스트를담고 있는 classes_tenso
                                          「와 각클래

                               「에 의해서 조합된다. 많은 클래스
스에 할당된 점수／확률값을 보관하는 scores_tenso

가 있는 모델에서는 tf. nn .top_k로 선택된 클래스들만 반환하도록 하는게 보통이다．




                                                                     학습된모델   - 287


===== PAGE 298 =====
              이는 모델에서 가장 높은 점수를받은K개의 클래스를 의미한다．

              마지막 단계는 exporter. Exporter. mnit 메소드를 호출하는 시그니처를 적용하고

                                        export 메소드는 출력 패스path, 모델의
              export 메소드로 엑ㅅ平ㅌ를 실행하는 것이다．

              버전숫자와세션이 필요하다．



scores, classes = t-F.nn.top_k(y, NUM_CLASSES_TO_RETURN)


model_exporter = exporter. Exporter(saver)
signature = exporter. classifkation_signature(input_tensor=x, classes_tensor=classes,
scores_tensor=scores)
model_exporter. init (de-Fault_graph_signature=signature)
model_exporter.export(os.path.dirname(_ file_ ),t-F.constant(time.timeQ), sess)



              이 모든 것을 합치고, JPEG 문자열을 추론 모델을 위한 형태로 바꾸면 코드는 아래와

              같다：



def in-Ference(x):
    # from the originaL modeL. . .


def convert_external_inputs(external_x):
    # transform the externaL input to the input fOrmat required on inference


external_x = t-F. placeholder(tf. string)
x = convert_external_inputs(x)
y = in-Ference(x)


scores, classes = tf. nn.top_k(y, NUM--CLASSES_TO_RETURN)


model_exporter = exporter. Exporter(saver)
signature = exporter. classification_signature(input_tensor=x,
classes_tensor=classes, scores_tensor=scores)
model_exporter. init (de-Fault_graph_signature=signature)
model_exporter.export(os.path.dirname(_ file_ ),tf. constant(time.timeQ), sess)




  288 -   CHAPTER 8 실제 사용하기


===== PAGE 299 =====
                                              정가 25,000원


엣지있게 설명한 텐서플로우

 2017년 l월 3일 초판 인쇄
 2017년 1월 10일 초판 발행
 저 4: Abrahams· Hafner· ErWitt· Scarpinelli
 역 자：정기철
 발행자：우명찬．        송 준
 발행처 : 홍릉과학출판사
 주 소：서울시 강북구 인수동 455-에
          回［긔［미［의 ［工
 등 록：1976년 10월 21일 제5-66호
  전
      화: (02) 999-2274--5, 903-7037
 팩 스：(02) 905-6729
 e-mail: hongpub(@hongpub.co.kr
 http://www.hongpub.co.kr
 ISBN: 979-11-5600-476-9

낙장 및 파본은 구입처나 본사에서 교환하여 드립니다．
판권 소유에 위배되는 사항
             （인쇄，복제，제본）은 법에 저촉됩니다．


===== PAGE 300 =====
엣지있게 설명한

텐서플로우


     GoogLe
      C++
     Python
 Data Row Graph
     Tensor
   Operation
    Session
    VariabLes
Machine Learning
 Deep Learning
