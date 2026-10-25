---
source_url: /run/media/yutae/Data/MPEG_비디오.pdf (USB, 2026-10-25 확인)
ingested: 2026-10-25
sha256: 54dc5758274896e1ff85f9e8a4b82cf5593d7d93431b6b36a88970c5ddb2ca1f
---

# MPEG 비디오 (raw source)
> text-layer PDF → `pdftotext -layout` 전체 추출. 일부 토큰은 원서 원형과 미묘히 다름 (인식 오류 아님, text-layer 원본). 원문 PDF(`/work/wiki/raw/books/MPEG_비디오.pdf`, 로컬) 대조 권장.

## Book metadata
- title: MPEG 비디오
- authors: 대우전자 영상연구소 (지은이명 원서 표기)
- pages: 308 (pdfinfo)
- source file: `MPEG_비디오.pdf` (sha256: `54dc5758274896e1…`, 344 MB)
- extract: `pdftotext -layout` @ 2026-10-25, 593,821 chars

## Original text (all 308 pages)

              ＝七中41HH4斗11mH1




대우천자 영상연구소 지음




     MPEG은 이제 전자공학을 전공하지 않은 사람들에게도
                               친근한 용어가 되었다．
           이렇게 널리 알려진 MPEG이지만 실제로 그
          기술적인 내용을 알고 있는 사람은 많지 않다．
따라서 0I 책은 MPEG을 알고자 하는 사람들을 위해 민틀었으며
       다양하고 쉽게 접근할 수 있는 방법을 제시하고 있다．
머리 말
   MPEG은 디지털 화상 및 음성의 압축표준화를 위한 국제기구의 약식명

 칭으로 1988년부터 회의가 시작되었으나       11끄）TV연구가 활발하困 90년태
 초반에도 入4PEG는 일부 극소수 전문가만이 알고 있는 용어였다. 그러나

 이제는 MPEG영상압축방식을 이용한 CD Video, Video on Demand, 무궁화위

 성 등이 현실화되면서 일반 신문에서도 자주 볼 수 있는 용어가 되었고

 떨티미디어 시대가 도래하면서 이 분야에 약간이라도 관심이 있는 사람이

 라면 귀에 익숙한 용어가 되었다. 그만큼 이제 MPEG은 널리 알려진 국제

 표준이 되었고 음성보다도 특히 화상어］ 있어서 획기적인 성공을 거두었다．

 벌써 MPEG신호를 복호할 수 있는 단일칩이 나오는가 하면 앞으로 영상

 신호의 보급어］ 있어서도 入4PEG방식을 이용하여 압축저장시킨 매체들이

 쏟아질 예정이다．



   이렇게 널리 알려진 八1PEG이지만 전문가들도 이해하기 어려운 표준규

 격서만 나와 있는 상황이고 기술적인 내용이 체계적으로 정리되어 있지

 않아서 실제로 그 표준의 세세한 부분까지 정확히 알고 있는 사람은 드문

 것 같다. 이는 전문가들의 능력이 모자라서가 아니고 그만큼 MPEG이 전

 공지식만으로는 이해하기 어려운 부분을 많이 가지고 있기 때문이다.             특
 히m氾G은 부호기 쪽은 언급하지 않고 복호기 쪽만의 표준을 정했기 때

 문어］ 더욱 어렵게 보일 수 있다. 이 책은 그러한 답답함을 풀어주기 위하

 여 入兀PEG표준 중 영상압축 부분을 나름대로 소화한 후, 쉽게 풀어서 설명

 했다. MPE(끄은 MPEG2의 부분집합으로서 완전 호환성을 갖고 있기 때문

 어］ I'띠PEG2를 이해하면 MPEG!은 자연스럽게 이아할 수 있다．



  이 책은 M까好을 기술적으로 이해하고자 하는 사람들을 위한 것이다．

 따라서 혼동을 피하기 위하여 八WEG에서 정의한 용어나 매개변수들은 그

 대로 영어로 썼으며, 표들도 入4PEG 표준어］ 있는 표를 그태로 이용하였다．
 또한 MPEG표준을 참고하고자 하는 사람들을 위하여 MPEG표준에서의

표나 그림들의 번호를 따로 표시하여 참고에 편리하도록 하였다．



 이 책이 MPEG을 이해하고자 하는 사람들에게 많은 도움이 되기를 바

라며, 그 동안 영상연구소의 연구지원을 아끼지 않으신 대우전자의 배순훈

회장님과 양재열 사장님께 깊은 감사를 드리고 또한 이 책의 출간을 위해

도움을 주신 연암책만들기의 유정룡 주간님께도 감사를 드린다．




                                 1995년 7월

                           대우전자 유시룡 상무
                                                       MPEG
                                                       VIDE0   3


                                          드므    iJ..
                                          1m기   /\ 1




목        只／
          .                                                           3



1.서콘                                                            10


2. 용어정의                                                        16


3. 약자와 기호                                                      36
3.1. 연산자
                                                                     36
 3.1.1. 산술연산자
                                                                     36
 3.1.2. 논리연산자
                                                                     37
 3.1.3. 관계연산자
                                                                     37
 3.1.4. 비트 연산자
                                                                     38
 3.1.5. 할당연산자（Assi聊卿t)
                                                                     38
 3.1.6. 간략기호(Mnemonics)
                                                                     38
3.2. 복호과정 기술을 위한 통려］
                                                                     40
 3.2.1. bitstream syntax 기술을 위한 방법
                                                                     40
 3.2.2. 함수의 정의
                                                                     41
 3.2.3. Reserved, forbidden, marker_bit                              41
 3.2.4. 정세도
                                                                     42



4.베트스트럼 신택스와 의미                                                44
4.1. 부호화된 화상데이터의 구조
                                                               44
 4.1.1. 비디오 sequence
                                                               '14
   I노略ress加e sequence와 Interlaced Sequence                     44
4



                                                  45
     Picture
     Chmminance format                            45
                                                  49
4.1.2. 움직임 예측과 Dcl'
                                                  51
 4.1.3. Picture type과 GOP
                                                  54
 4.1.4. 슬라이스（Slice)
 4.1.5. 매크로 블록(Macrobli乂k)                        55
                                                  57
 4.1.6. 블록（Block)

                                                  58
4.2. 부호화과정과 비트스트림 신택스
                                                  58
 42.1. 부호화과정과 버퍼제어
                                                  63
    4.2.2. Low delay 모드
                                                  64
    4.2.3. 계위（Scalab小ty)
                                                  65
    4.2.4. Syntax변수들의 내용
                                                  67
    4.2.5. Synt炚구조

4.3. 비트스트림의 각 변수의 의미와 조건들                         81

                                                  81
    4.3.1. Sequence Header
                                                  87
    4.3.2. User Data
                                                  88
    4.3.3. Sequence Ex妃nsion
                                                  92
    4.3.4. Sequence Display Ex把nsion
                                                   96
    4.3.5. Sequence Scalable Ex妃nsion
                                                  101
    4.3.6. Group of Picture Header
                                                  103
    4.3.7. Picture H叫1der
                                                  107
    4.3.8. Picture Coding Ex把nsion
                                                  123
    4.3.9. Quant卜4a1r1：乂Ex把ns幻n
                                                  125
    4.3.10. Picture Display Extension
                                                  127
    4.3.11. Picture Temporal Scalable Extension
                                                  128
    4.3.12. Picture Spatial Scalable Extension
                                                  132
     4.3.13. Copyright Extension
                                                  133
     4.3.14. Slice
                                                  140
     4.3.15. Macro block
                                                  145
     4.3.16. Macroblock Modes
 4.3.17. Motion Vectors                          154
 4.3.18. Motion Vector                           155
 4.3.19. Coded Block Pattern                    157
 4.3.20. Block                                  160



5. 복호화과정                                        ]64
5.1. 역양자화와 역 DCT                                164
 5.1.1. 가변장복호화臼ariable len帥decoding)            164
    intra bli乂k에서의 DC 계수들 (c（玘術cients)          165
   다른 계수들 (coefficients)                        168
 5.1.2. 역스캔（hwerse Scan)                        177
 5.1.3. 역양자화（佃erse（加antization)                 177
    역양자화 연산 (Inverse quantization arithmetic)   178
   포화처리 (Saturation)                            182
   불일치 제어 (Mismatch coi血에                       182
 5.1.4. 역 DCT(Inverse D크)                       184

5.2. 움직임 보상                                     184
 5.2.1. Pred蜘on field 와 frame 선택（selection)     186
   Field prediction                             186
   Frame 예측                                     189
 5.2.2. Frame 메모리에의 저장（Fr跏est아e addres跏g)       190
 5.2.3. 入4otion vector 디코딩                      191
 5.2.4. 벡타예측기（Vec奴Predic帥s)                     201
   motion vector predictor으1 갱신방법               201
   motion vect아predictor의 리셋방법                  202
 5.2.5. 추가 Du고prime 계산（Anti毗tic)                203
 5.2.6. Color components 의 Scaling              205
 5.2.7. 반화소예측을 위한 필터링                           205
 5.2.8. 예측값들의 평균（co岫II妃predicti毗）               207
6



                                          207
     단순 丘ame 예측
                                          207
     단순 field 예측
                                          207
     16x8 motion compensation
                                          208
     Dual prime
                                          208
 5.2.9. 합산과 포화（Addi如n and sa恤ation)
                                          209
 5.2.10. Skipped macroblock
                                          209
     P field picture
                                          209
     P frame picture
                                          209
     B field picture
                                          210
     Bframepicture
                                          210
5.3. 공간적 계위（Spatial Scalabffity)
                                          211
    5.3.1. 공간예측（Spati仰redic如n)
                                          212
     reference fr如le의 선택
                                          213
     resampling 과정
                                          217
      Deinterlacing
                                          218
      Vertical resampling
                                          219
      Horizont訌 resampling
                                           219
      Reinterlacing
                                           220
    5.3.2. 시간예측（Te呻oral pre小ction)
                                           225
    5.3.3. 공간예측과 시간예측의 선택과 조합
                                           228
    5.3.4. Skipped macroblocks
                                          228
5.4. SNR 겨1위 (SNR scalabifity)
                                           229
    5.4.1. 변경되는 신택스 구조
                                           233
    5.4.2. 入Iacrobh乂k
                                           233
      dctjype
                                           233
       Skipped Macroblocks
                                           234
    5.4.3. Block
                                           234
       가변장복호 (Variable length decoding)
       역스캔 (lnverse scan)                  234
                                           234
       역양자화 (Inver記 quantisation)
    두 레이어의 계수들의 합산                    234

5.5. 시간적계위 (Temporal scalabffity)    235
  5.5.1. 변경되는 신택스 구조                  237
  5.5.2. 시간적꼐위에 대한 권고사항               239

5.6. Data paritioning                240

5.7. 복합졔위(Hybrid s에abffity)          242

5.8. 복호화된 출력의 형태                     244



6. 프로파얻과 레뻗                          250
6.1. MPEG1 과의 호환성                    252

6.2. 프로파일들 간의 관겨］                    252
  6.2.1. rei光at_first_field의 사용      254

6.3. 레벨 간의 관겨］                       255

6.4. 계위층 (Scalable layers)           257
  6.4.1. 허용가능한 layer들의 조합            258

6.5. 프로파일！ 레벨과 레이어에서의 변수값            260

6.6. 각 프로파일과 레벨에서의 제한조건들             266



부콕 I : 챰고문헌과 국제규격                    299


부목 2: MPEG2의 이ementary stream 의 에I   301
IJ
      \   MP日｝VIDEO

          서론




이 책은 MPEG을 기술적 입장에서 얄고
자 하는 사람矗 위메서 쓴 것이다. 그
런 사림들이라면 MPEG2 IS를 ！콰도 되지
만, MPEG2 IS는 보기가 그렇게 쉬운 권
고안은 아니다. 행간의 뜻을 읽어야 하
口］ 뒷이야기를 얄아야 힌다. 이 책은 그
런 사람들이 MEPG을 좀 뎌 이해하기
쉽게 돕기 위힌 책이다．
     MPEG
10   VIDE0




 1．서론

        MPEG（엠펙）은     入4oving Picture Experts Group의 약자로 정식명칭은 ISO/IEC

      JTC1/SC29/WG11이다.   즉   국제표준기관인        ISO와   mc의       Joint   Technical

      Comm血ee어］서 SubComni血ee 29의 \Vorking Group 11이다.   MPEG은 1988년에 설

      립되어 15명 정도로 시작하였으나 나중에는 그 20배가 넘는 인원으로 불어났다．

      처음에는     저장매체를       근간으로     하는    1.外化PS급       이상의    入4IPE(끄（공식명

      칭:ISO/IEC 1172）으로 시작하였으나 入4PEG1이 끝날 즈음인 1990년 9월 미국 산

      타클라라 회의부터 5Mbps급 이상의 MPEG2어］ 대한 논의가 시작되어 1994년 싱

      가폴 회의에서 入4PEG2 IS（국제표준沁口na如nal Stand征d）가 만들어지게 되었다．

      MPEG2는 시스템, 비디오, 오디오 등의 작은 그룹들로 이루어져 있으며 현재

      IS로 된 이 3개 표준의 공식명칭은 시스템이 ISO肛iC 13818-1, 비디오가

      ISO/IEC 13818-2, 오디오가 ISO/IEC 13818-3이다.   현재 MPEG2는 화상압축분야

      에서 거의 세계공통표준이 되다시피 하고 있는더］, 入I1PEG2가 이렇게 널리 쓰이

      거］ 된 이유는 다음과 같이 2가지를 꼽을 수 있을 것이다.                   첫째로 압축부호화

      의 기술이 거의 최고수준어］ 달했고 또한 비디오의 디지털 세계표준이 요망되고

      있던 시점에서 세계 각국 대표들이 같이 모여 최고의 기술을 위하1 서로 경쟁했

      으며 또 각국 대표들이 정하困 기술에 대해서 동의했다는 것이다.                               둘찌臣

      MPE好의 신택스부분에서 찾아볼 수 있는더］ MPE(｝은 어떤 특정한 응용분야만

      을 목표로 해서 만든 것이 아니고 화상압축을 필요로 하는 모든 분야에 쓰일

      수 있도록 유연성을 주어 제작되었다는 것이다.



        MPEG2 비디오표준은 h血oduction을 포함하여 총 8개의 Chapter오干 부록으로

      되어 있다. I川的duction과 Chapter 1은 MPEG의 화상압축기술에 대한 소개， 범위

      등의 개괄적인 설명에 관한 것으로 뒤에서 자세히 설명되기 11n문에 이 책에서

      는 따로 구성하지 않았다. Chapter 2는 MPEG 표준에서 언급한 국제표준들이며
                                                   S
                                                    MPEG
                                                    미DE0        11
                                                       ；日1
이 책에서는 참고문헌과 함께 맨 뒤에 기술한다. Chap妃r3은 용어들에 대한 정

의 또는 뜻을 설명하1 놓은 것으로 이 책에서는 2장에서 기술한다.                        확상압축기

술에 어느 정도 익숙한 사람이라면 먼저 읽어보는 것도 도움이 되리라 생각한

다.   또한 Chapter 4와 Chap虹5는 뒷장에서 사용될 기호나 약자, 용어들에 대한

설명으로 이루어졌는더1 이 책에서는 묶어서 3장에서 기술하였다.                          이중 상당수

는 대부분의 엔지니어들에게 이미 알려져 있는 것이고, 또 필요하면 언제든지

찾아볼 수 있지만 미리 익혀두면 이해에 도움이 되리라 생각한다.                           시간이 없

는 사람이라도 3장 중에서 간략기호（n끄iemonics）는 한번 보고 넘어가면 좋다．



 入4PEG 표준의 Chapter 6은 入4PEG2 신택스（syntax）에 관한 것이다.             즉 데이터

를 보내기 위해서 붙이는 header들, bits仕earn의 흐름을 결정하는 데이터 내부의

조건들, bit毗earn의 순서 등어］ 관한 내용을 담고 있다.          MPEG2로 부호화된 영

상데이터는 움직임 벡터와 DCT계수들로 이루어져 있다.                  이러한 데이터들은

Chapter 7의 복호과정을 설명함으로써 알 수 있는 것이지만 Chapter 6의 신택스

부분에서 이러한 데이터요소의 명칭이 먼저 나오게 된다. 이것은 먼저 bits甘earn

의 신택스를 명확히 설명하기 위함인데, Chapter 7의 복호화과정 부분에서 충분

한 설명이 나오지만 본 책에서는 장의 분리를 위하여 4장에서 신택스부분을 기

술하면서 이러한 요소들을 간단히 설명을 한 후 5장에서 복호과정율자세히 기

술하겠다.    6장의 대부분의 변수（parameter）들은 화상부호화에 어느 정도 경험이

있는 사람이라면 충분히 이하빨 수 있는 내용이다.                처음 읽는 사람이라면 4, 5

장을 다 읽어야 완전히 이해하겠지만 전문가가 된 후에는 4장의 신택스만 보고

도 MPEG2 bit缸earn을 이하빨 수 있도록 4장을 구성하겠다.              MPEG표준의

Chapter 8은 profile과 level어］ 관한 내용이다.   여기서 pr而le이란 MPEG2의 신택

스 내의 모든 경우를 전체집합이라 했을 I , 이 중에서 몇 개씩 묶어서 정한

일종의 부분집합이다. 즉 어떤 pr曲le에서는 어떠한 것들만을 허용한다든가 하

는 그러한 규정이다.        또한 1ev이이란 bits仕earn의 변수（parameter）에 부가되는 저］
12




     한조건들이다. 入'IPEG에서 이와 같이 profile과 1ev이을 규정하고 있는 이유는 편

     리함 때문도 있겠지만 MPEG 방법이 앞에서 언급했듯이 유연성이 있다는 데에

     있다.   원래 MPEG에서는 어떤 특수한 응용분야를 목표로 해서 방법을 선정하

     지 않았다.    II긔1문어］ 응용분야에   따라서 전송률이나 색신호 표현방법 등 여러

     가지 변수（parameter）나 방식 등을 바꿀 수 있고 이를 신택스에서 표시하도록 하

     고 있다.    이렇게 유연성이 있다는 것은 좋은 점도 되지만 너무 가변적인 경우

     에는 오히려 혼동을 가져올 수 있다. 따라서 어느 정도의 굵은 선을 그어주어

     야 할 필요성이 생기게 되는더］ 이 t대문어］ 만든 것이 profile과 level이다.   이에

     대해서는 6장에서 다시 설명한다.        본 책에서는 설명 순서를 Is의 순서를 따르

     나 세세한 부분의 구성은 설명어］ 유리한 순서로 재구성하였다.          또한 본 책의

     표나 그림 중에서 入4PEG 표준어］ 있는 표나 그림은 MPEG IS에서의 번호를 뒤

     어］ 표시함으로써 이 번호를 이용하여 IS를 참조할 수 있도록 하였으며 이해의

     편의를 위해서 같은 표나 그림이라도 설명되는 부분에 중복해서 표시하였다．

     IS에서 사용하는 변수들은 혼돈을 피하기 위하여 영어 그대로 이용했으며 여기

     서의 설명을 위해서 불가피하게 만든 변수는 이 책에서 만든 것임을 분명히 언

     급하겠다. 入WEG에서의 부록은 표준의 보조설명이므로 따로 구성하지 않고 본

     문의 해당 부분에서 같이 설명하도록 하겠다．



      참고로 八4PEG2 표준사양은 복호기규격이라는 점을 밝혀둔다. MPEG2에서는

     특별히 부호화과정을 규정하지 않고 있으므로, 부호화는 어떻게 해도 관계가

     없으며 bit缸earn이 신택스어］ 맞기만 하면 복호가 가능하다.     이러한 규정에 익

     숙하지 않은 사람은 이상하게 들릴지 모르지만 이러한 이유로 入'IPEG2에는 부

     호기가 어떠한 것이 되더라도 복호가 가능하도록 보호장치들이 되어 있다.              뒤

     에서 이러한 것을 언급할 필요가 있으면 그따1 그때 언급하도록 하겠다.             또한

     MPEG2 IS에서는 보통의 상식으로는 잘 이해가 가지 않는 부분들이 많다.           효

     율성을 위해서 그렇게 된 부분도 있고 다른 역사적인 또는 하드웨어상의 이유

     로 그렇게 된 부분도 있다. 이러한 것들은 권고안에서 설명되어 있지 않기 U뀨
                                       匣13
문어］ 읽는 이가 혼란스러울 수 있다.     또 어떤 부분에서는 자서同 설명되어야

할 부분들이 프로그래밍 언어로 간단히 압축되어 있기 I대문어］ 여기서는 그러한

부분을 자세히 설명하고 복잡한 과정은 설명을 덧붙여서 부호화과정까지 설명

하도록 하겠다．



 이 책은 入IPEG을 기술적 입장에서 알고자 하는 사람들을 위해서 쓴 것이다．

그런 사람들이라면 MPEG2 IS를 봐도 되지만, MPEG2 IS는 보기가 그렇게 쉬운

권고안은 아니다. 행간의 뜻을 읽어야 하며 뒷이야기를 알아야 한다. 이 책은

그런 사람들이 MEPG을：좀 더 이해하기 쉽게 돕기 위한 책이다.         마지막으로

덧붇이고 싶은 말은 入4IPEG은 전세계의   전문가들이 모여서 수년 간 만든 것이

다. 따라서 어떻게 보면 단순할지 모르지만 막상 프로그램을 짜려고 한다든가

특수한 경우어］ 태해서 入IlPEG을 해석할 때는 만만한 문제들이 한두 가지가 아

니다.   따라서 이 책을 소설을 읽듯이 읽어도 되겠지만．그랬을 때 뒷부분으로

가면 갈수록 앞에서 나온 변수들이 혼동되고 뜻도 더 모호해지게 된다.         따라

서 저자는 4장의 신택스 부분에서 설명되는 변수들은 되도록 의미를 정확히 파

악하고 그띠1 그따1 그 이름과 뜻을 외우면서 나갈 것을 권하는 바이다.
frame:

호｛상신호의 공간 정보를 이루는 line들의
집합. 아ogressive신호인 경우 이 라인
들은 시간상의 힌 점에서 시작해서
卄ame의 맨 끝 라인까지 연속된다．
in也rlaced신호인 경우는 top field와加ttom
field로 이루어지는데 이중 힌게의 field는
다른 것보다 하나의 fie넌기간만큼 늦게
시작힌F{.
16




 2. 용어정의

     AC coefficient
       2차원 DCF계수 중에서 양쪽 차원 중 한쪽이라도 주파수가 0이 아닌 계수．



     big p妃ture
       VBV b咐er의 underfiow를 유발시킬 수 있는 coded picture. 이 big picture는

       low_delay가 1인 경우에만 발생할 수 있다. big picture가 발생하면 伽ture를

       건너뛰게（skip) 되는더］, 그래서 가끔 "skipped picture" 가 같은 개념을 설명하

       기 위하여 쓰인다．



     B-field picture
       Field siructure를 갖는 B-picture.



     B-frame picture
       Frame s仕ucture를 갖는 B-picture.



     B-picture
       과거와 미래의 reference field 또는 frame으로부터의 움직임 보상을 통해서

       얻어지는 picture.



     back사ard compatibility                               "
       기존의 표준이 있는 상태에서 새로운 표준이 정해졌을 1대, 만약 기존의 표

       준이 새로운 표준의 일부 또는 전부를 이용하囚 계속 동작할 수 있을 I대

       새로운 표준을 "backward compatible" 하다고 한다．
                                                      17



backward motion vector

  디스플레이 순서에 따라서 더 늦은 fran配이나 fie넌를（미래의 ft如配이나

  field) 참고로 해서 움직임 보상할 1대 쓰이는 motion vector.



backward prediction

  미래의 fra끄叱이나 field를 참고로 해서 하는 예측．



base layer

  Scalab皿口에서의 각 layer 중 독립적으로 부호화될 수 있는 layer.



bitstream : stream
  Data가 부호화됐을 때의 bit열．



bitrate
  부호화된 bit缸earn이 디코더에 입력되는 bit율．



비ock
  8열과 8행으로 이루어진 샘플들의 행렬 또는 64개의 DCI계수들．



bottom field
  Frame을 이루고 있는 2 field 중 위치적으로 밑에 있는 field. Bottom field의

  각 l血e은 的p field의 각 line 바로 밑에 존재한다．



切rte align風1
  Bit가 bitstream에서의 첫 bit로 부터 8b畑단위로 위치할 I대 byte 십igned되었

  다고 한다．
18




     byte

      8 bits.



     channel

      이 표준어］ 따라서 만들어진 bits仕earn을 저장하거나 전송하기 위한 디지털

      매체．



     chrominance 化rn伯t

      Macroblock에서의 ci寸ominance block 개수를 나타낸다．



     chroma simulcast

      SNR scalabil幻의 한 종류로서 enhancement layer어］ 해상도가 높은 색신호

      (ii血a-DC계수와 모든 AC계수）를 보낸다．



     chrominance component

      Bitstream어］서 정의된 대로의 primary color와 관계되고 2개의 차이 색신호

      Cb, Cr의 matrix, block 또는 하나의 화소．



     Coded B-frame

      B-frame picture나 B-field pi아出e의 쌍．



     coded frame

      Coded I七arne 또는 coded P－加끄ne 또는 coded B-frame.



     coded I-frame

      I-frame picture 또는 I小eld picture의 쌍. 여기서 첫 번째1 field picture는 I-

       pictt止e이고 2번째 field picture는 I-picture 또는 P-I加ture이다．
                                                          r小.
coded P-frame

  P-fra끄lie picture 또는 P-field picture의 쌍．



coded picture
  Coded丘ame 또는 coded field, 이 coded picture는 picture header와 extension들

  또 picture data로 이루어진다．



COded videO;bitstream
  이 표준에서 정의한 대로의 하나 또는 둘 이상의 picture들이 연속적으로

  부호화된 bit열．



coded order
 Picture가 전송되거나 복호되는 순서. 이는 꼭 디스플레이되는 순서와 같을

  필요는 없다．



coded representation
 부호화된 형태의 데이터 요소（d玭a element).



coding parameters
 Bit毗earn을 특징지어 주기 위해서 사용자가 정하1 주는 변수의 집합．




component
 Picture를 구성하는 휘도신호와 두 개의 색신호의 matr奴, block 또는 한 개

 의 샘플．
     MPEG
20   V山EQ




       compression
            어떤 data를 나타내기 위하1 사용되는 bit를 줄이는 일．



       constant bitrate coded video
            일정한 bit율을 갖는 부호화된 vid的bits仕earn.



       constant bitrate
            부호화된 bits仕earn의 bit율이 처음부터 끝까지 일정한 것．



       data element
            부호화 전이나 부호화된 후의 상타땍 데이터（data) 항목들．



        data partitioning
            Chai기riel error 등어］ 대비하여 bitstream을 2개로 나누는 방법.           이 두 개의

            bi始仕earn은 복호화하기 전에 합쳐져야 한다．



       口picture
            入4PEG1어］서 사용한다．



        DC coefficient
            2차원 D(크된 계수 중에서 양쪽 차원 모두 주파수가 0인 계수．



        DCT coefficient
            Dcr계수：cosine basis 함수의 진폭．



        decoder input buffer
            Video buffe血ig verifier에서의 FIFO(first in丘rst out)bu什er.
                                              21




decoder
  복호과정을 행하는 장치．



decoding process
  부호화된 bi始甘earn을 받아서 복호된 picture나 음성을 내주기 위하여 이 표
  준에서 정해진 과정．



dequantisation
  양자화된 DC[계수들을 다시 원래의 크기로 만들어주는 작업．



dig作키 針orage me비a: DSM
  디지털로 전송하거나 저장하는 장치나 시스템．



d治crete co引ne tran針orm : DCT
  DCT 또는 inverse DCT.



display aspect ratio    t Ae
  디스플레이하고자 하는 화상의 높이／폭의 비율．



display order
  복호화된 picture가 디스플레이되는 순서. 보통 이 순서는 디코더에서 출력
 되는 순서와 동일하다．



display process
 복원된 fran配을 디스플레이하는 작업．
22




     dual巾r油e pred托蜘D自
       두 개의 forward field 예측이 평균되어지는 예측모드. 여기서 예측블록 크기

       는 16X16이고 이 모드는 U恥riaced P-pic加妃에서만 사용된다．



     editing
       하나 또는 2개 이상의 bi始仕earn을 이용하여 새로운 하나의 bitstream을 만드

       는 작업. 새롭거］ 구성된 bi侄甘earn도 이 표준어］ 맞아야 한다．



     encoder
       부호화과정을 행하는 장치．



     encoding process
       Picture나 음성을 받아서 이 표준어］ 맞는 부호화된 bits甘earn을 만드는 과정．

       이 표준에서는 부호화과정은 언급하지 않고 있다．



     enhancement layer
       Sc出ab小ty에서 base layer 위에 있는 상태적인 참고 layer.




     fast for사ard playback
       하나의 sequence나 그 일부분을 실시간보다 빠르게 디스플레이하는 작업．



     fast reverse playback
       하나의 sequence나 그 일부분을 역으로 실시간보다 빠르게 디스플레이하는

       작업．
                                                                         23



field
  Frame에서 하나 컬러씩의 라인들의 집합．



field_based prediction
  Reference fra끄叱의 한 fie닢만을 이용하나a 예측하는 모드.                         예측크기는 16X
  16이며 皿四ressive丘arne에서는 이용되지 않는다．



field period
  Frame rate의 역수의 반．



field picture : field structure picture
  Picture structure가 "top field" 나 " 比ttom f祀id" 인 C에ed picture.



flag
  이 표준에서 가질 수 있는 값이 단 두 개밖에 안 되는 변수．



化rbidden
  절다1 사용되어서는 안 되는 값．



forced updating
  인코더와 디코더 사이의 DCT 불일치（mismatch）가 과도하게 커지는 것을

  방지하기 위하여 帥대로 macroblock이 血ira-codii堪되는 과정．



forward compatibility
  기존의 표준이 있는 상태에서 새로운 표준이 정해졌을 경우 만약 새로운

 표준이 기존의 표준을 계속 복호할 수 있을 t대1 새로운 표준을 "forward
24




      con叩atible"하다고 한다．



     forward motion vector
      디스플레이순서로 따져서 더 빠른 frame이나 field（과거의 fran叱이나 field)를

       참고로 해서 움직임 보상할 TI가 쓰이는 motion vector.



     化rward pre버야or
       과거의 允ime이나 fie닢를 reference로 삼아서 하는 예측．



     frame
       화상신호의 공간정보를 이루는 l血e들의 집합.                       皿魄res없ye신호인 경우 이

       라인들은 시간상의 한 점에서 시작해서 丘ame의 맨 끝 라인까지 연속된다．

       hlterlaced신호인 경우는 的p field와 m如m field로 이루어지는더］ 이중 한 개

       의 field는 다른 컷보다 하나의 field 기간만큼 늦게 시작한다．



     frame_based predictor
       Referei此ft加配의 양 field를 이용하는 예측모드．



     frame period
       frame rate의 역수．



     frame picture : frame structure picture
       Picture structure7l- "frame" 인 coded picture.



      frame rate
        복호 후어］ 출력되는 {1加配율．
                                                          25




fL血ire reference fram이伽Id)

   디스플레이 순서로 현재 fran配보다 늦은 reference frame (field).



아oup 아 picture
  入4PEG1에서만 정의한다. 그러나 이 표준에서는 얍oup可picture header를 삽

   입함으로써 비슷한 개념을 만들 수 있다．



header

  Bi떼ream에서 header 다음에 따라오는 부호화된 데이터의 성질을 나타내주

  는 데이터의 군．



hybrid scalibility
  두 가지 형태 이상의 scalab小ty의 조합．



interlace

  Ft砒ne을 구성하는 lit妃들이 한 血le씩 건너뛰며 다른 시간의 신호를 나타내

  는 특성. 현행 TV가 채택하고 있다.          두 개의 field 중 첫 번째로 디스플레
  이하고자 하는 fle너를 打rst field라 하고 다른 fie닢를 second field라 하는데，

  first field는 的p field가 될 수도 있고 b야torn field가 될 수 도있다．



I-field picture
  Field s打ucture인 I-picture.



I-frame picture

  Fr工ne stmcture인 I-picture.
26




     I-picture: intra-coded picture
       그 picture 자신의 정보만을 이용하여 부호화된 picture.



     intra coding

       그 자신의 macrobli乂k 또는 picture의 정보만을 이용하여 macroblock 또는

       picture를 부호화하는 것．



     level

       특정 profile 내에서 이 표준의 변수들이 가질 수 있는 값들에 태한 제한조

       건들의 집합. 하나의 profile은 하나 또는 그 이상의 level들을 가질 수 있다．

       pr而le과 level 이외의 다른 문맥에서는 1ev이은 0이 아닌 계수의 절대값을

       뜻한다．



     layer

        Scalabili口를 이용하는 곳에서 순위가 매겨진 bitstream 중의 하나를 가리킨

        다．
      layer bitstream
        특정 layer에 연관된 하나의 bitstream. " enhancement layer bitstream" 처 럼 항상

        layer를 특정지어 주는 말콰 같이 쓰인다．



      lower layer
         layer으1 계수 중 enhancement layer 바로 밑의 layer.



      luminance component

             Bitstream에서 정의된 대로의 primary c이or어］ 맞는 흑백신호를 표시하는 휘

             도신호（Y）의 ma打奴block 또는 한 개의 샘플．
                                                   MPEG
                                                   VIDE0   27



Mbit
  1000 000 bits.



macr아)IOCk

  휘도신호의 8X8 block     4개와 그 lun血ance신호의 같은 위치（크기＝l6X16)

  로부터의 색신호 8X8block 2개, 4개, 또는 8개．



motion compensation

  예측의 효율을 향상시키기 위하여 motion vect야를 사용하는 것. motion vector

  는 복원된 과거 또는 미래의 reference field나 fran叱으로부터의 0岱et을 나타

  낸다．



motion estimation
  부호화과정에서 motion ye아아를 예측하는 작업．



motion vector

  움직임 보상을 위해서, 현재의 picture나 fie닢의 좌표로부터 referen代丘如配이

  나 field의 좌표의 0什S아을 나타내주는 2차원 벡터．



non-intra coding
  그 자신뿐만 아니라 다른 시간의 macroblock 또는 picture의 정보를 이용해1

  서 macr的뇨：k 또는 picture를 부호화하는것．



opposite parity
  Top의 반대 parity는 比帥l이고, 比ttom의 반대 parity는 的p이다．
     MPEG
28   피DEO
     ;H므




           P-field picture

             Field s仕icture인 P-picture.



           P-frame picture

             Frame structure인 P-picture.



           P-picture: predictive-coded picture

             과거의 field나 frame을 referen凹로 삼아서 움직임 보상을 하는 picture.



           parameter

             이 표준에서의 syntax 내의 변수．



           parity (of field)

             Field의 parity는 t아） 또는 比如m 중의 한 가지 값을 갖는다．



           past reference frame (field)

              디스플레이 순서상 한개의 picture보다 빨리 발생한 reference 丘ame 또는

              field.



            p把ture

              Luminance와 두개의 chrom血ance신호를 나타내는 8bit로 된 숫자들의 행렬

              3개로 이루어진 신호Gource）나 부호화된 데이터 또는 복원된 화상 떼이터．



            picture data

              VB\/ 동작에서 부호화된 picture의 모든 데이터와 그 전의 모든 header, user

              data, 또 만약 picture data 뒤쪽으로 그 다음의 start code 바로 직전까지

              stu節璡이 있다면 그 stuffmg data까지 모두 포함한다. 이띠1 그 다음의 stait
                                                     29



  code는 포함시키지 않는더］ sequence end code는 예외적으로 포함시킨다．



prediction
  지금 현재 부호화되고 있는 샘플값이나 데이터의 추정치를 제공해주기 위

  해서 사용된다．



prediction error
  어떤 샘플값이나 데이터의 실제값과 predict아값의 차이．


pred七t아
  이전어］ 부호화된 샘플값이나 데이터들의 선형결합．



profile
  이 표준의 syntax에서 미리 정해진 부분집합．



progressive
  한 卄ame의 모든 화소들이 시간적으로 같은 것을 나타낸다．



quantization matrix
  역양자화기에 의해서 사용되는 64개의 8bit 값들



quantized DCT coefficients
  역양자화 전의 DCT겨］수들．



quantiser scale
 역양자화 과정에서 양자화 크기를 나타내주는 Sc沁e factor.
30




     random access
      Bitstream의 임의의 위치에서 읽어서 복호화하는 작업．



     reconstructed frame
      휘도신호와 두개의 색신호를 나타내는 8b畑로 된 숫자들의 행렬 3개로 이

       루어진 복원된 frame.



     reconstructed picture
       복원된 fran妃중의 한 field.



     reference 竹이d
       복원된 如irne의 한 field로서 P-picture나 B-1뇨cture의 복호시 순방향이나 역방

       향 예측을 위해서 쓰인다．



     reference frame
       I-丘an肥이나 P-丘ame의 형태의 복원된 丘ame. P-1朮ture나 B巾icture의 복호시

       순방향이나 역방향 예측을 위해서 쓰인다．



     reordering delay
       Frame 재배치때문어j 발생되는 지연．



     reserved
       미래의 사용을 위해서 확보해놓은 것．



      sample asp엮）t rati0     91FL

        샘플 사이 간격을 나타내는 더］ 血le간의 간격을 샘플간의 간격으로 나눈값

       을 사용한다．
                                                         31



scalable hierachy
  한개 이상의 순서가 매겨진 vid的bitstream에서의 부호화된 화상뎨이터．



scalability
  순서가 매겨진 bitstream에서 그 부분집합을 이용해서 복호할수 있는 능력．

  자체적으로 복호될수 있는 가장 작은 부분집합을 base layer라 한다． 그외에

  다른 bitstream들의 각각을 enhancement layer라 한다. 또 lower layer는 어떤

  enhancement layer의 바로 아래에 있는 layer를 뜻한다．



side information
  Bitstream 에서 복호기를 조정하기 위하여 필요한 정보．



16 x 8 pred把t아

  Fie넌단위 예측과 비슷하지만 예측블록크기가 16X8인 예측．



run
  주사(scanning）순서로 0이 아닌 계수앞의 0의 갯수. 0이 아닌 계수의 절대값

  은 1ev이이라 한다．



saturation
 정하困 최대치나 최소치를 넘어가는 값을 제한하는 것．



引dpped macro이ock
 부호화할 데이터가 하나도 없는 macrobl어：k.
     MPEG
32   피DEO
     日d




          引把e
            연속적인 macr아）lock 들．



          SNR scalability

            Enhancement layer가 lower layer보다 DCT계수를 더욱 세밀하게 보내주는

            scalab小ty 의 한 종류．



          source: input
            부호화하기전의 비디오물이나 그것의 속성을 표시해주는 말．



          spatial prediction
            Spatial scalab小口에서 lower layer의 복원된 frame으로 부터의 예측．



          spatial scalability
            Enhancen目it layer가 같은 layer로부터 뿐만아니라 lower layer의 복원된 丘ame
            으로부터의 예측하는 scalability.           각 layer는 丘ame크기, 包ime율, chroi恤iance

            format이 디를수 있다．



          St카t code [system and 너de이
            Bi떼ream내에서 S戶flax의 특정한 구조를 나타내주기 위하여 사용되는 32b社

             code.



           stuffing(bits) : stuffing(bytes)
             복호화 과정에서 버려질 것이지만, 데이터 발생량이 적을띠P bit율을 높여주

             기 위하꺼 bitstream에 채워주는 것．
                                                      33




temporal prediction

   Spatial prediction에서 정의된 이외의 reference蜘ne이나 加id을 이용하여 하
  는 예측．



temporal scalability

  Enhancement layer가 lower layer로부터 얻어진 샘플로 부터의 움직임 보상을

  이용하는 형태의 Sc고ability. 각 layer들은 동일한 frame크기, chrominance

  format읖L 같지만 frame율은 다를 수 있다．



如pf伯Id

  하나의 frame을 이루는 2개의 field중 하나.     T叩 field의 각 line은 蜘如m
  field의 각 line 바로 위에 존재한다．



如p layer
  Sc出ab小ty어］서 가장 위에 있는 layer. 뇨yer코값이 가장크다．



variable bitrate
  Bit毗earn의 복호시 시간어］ 따라 bit율이 변하는 동작．



variable length coding ; VLC;
  자주 발생하는 데이터에는 짧은 부호를 할당하고, 별로 발생하지 않는 더1

  이터에 대해서는 긴 부호를 할당하는 것으로서 복호가 가능하햐 한다．



video buffering verifier: VBV
 Encoder뒤에 개념적으로 붙어 있는 가상적인 디코더． 이는 인코더가 발생

  시키는 가변적인 데이터에 제한을 가하기 위하여 사용된다．
MPEG
VIDEO




   video sequence
        Bitstream의 가장 높은 계위의 신택스구조.         이는 하나 또는 그 이상의 부

        호화 된 丘ame을 포함한다．



   xxx profile decoder
                                                               bi慨呻m을
        To미ayer가 소위 xxx profile을 따르는 하나 또는 계위（scalable）의

        복호할 수 있는 디코더．



    xxx profile scalable hierachy

        To이ayer가 소위 xxx pr而le을 따르는 bits仕earn들의 집합．




    xxx profile bitstream
        Pr而Ic이 xxx인 scalable계위의 bitstream. 이 bits仕earn은 모든 lower layer의

        bits仕earn이 있어야 복호될 수 있다任f base layer bits仕earn은 제외）.



    zigzag scanning order
        가장 낮은 주파수부터 가장 높은 주파수까지 DCI꼐수들을 일렬로 세우기

        위한 특정한 나열방식．
r <b

Z只i)   I를 a부터 b-i까지 변회시
i= n


       켰을 때 쩨의 합
  MPEG
  VIDE0




3. 약자와 기호

     이 표준을 기술하는 더］ 쓰이는 약자와 기호들을 다음과 같이 정의한다．



3.1. 연산자
3, ] , ] . 산술연산자
     +




     ++



      x*




              제곱승巾ower)
     /        결과를 0 쪽으로 만들어주는 정수나누기. 예를 들어 7/4와 －刀-4

              의 결과는 1이고, -7/4와 刀-4의 결과는 -1이다．



      //      결과를 가까운 정수 쪽으로 만들어주는 정수나누기. 단, 중간인 경

              우는 특별한 언급이 없는 한 0에서 먼 쪽으로 올림한다.     예를들

              어 3112의 결과는 2이 고 -3112의 결과는 -2이다．



     DI\/     결과를 마이너스 무한대 쪽으로 만들어주는 정수나누끼.       예를 들

              어 3D1\口의 결과는 1이고 -3D1＼口는 그이다．



      +       절단이나 반올림을 하지 않는 수학적인 의미의 나눗셈．



      %       나머지 연산（양수에 대해서만 정의됨）.
                                                          37



     Zf (i)           i를 a부터 b-i까지 변화시켰을 때 f(i）의 합

                                           i    x> 0
     Sign()           Sign(x) = " 0             x==0
                                           -1   x< 0
      .   ,   .   .   .   .   .   .   fx        x>   =0
     IWS()            /\ OSIX) :=)                 r\
                                  t,-x          Xczu




3.1.2, 논리연산자


     II               논리적 OR



     &&               논리적             AND



     !                논리적 NOT




3, ] .3 , 관계언산자


                      큰
38




                        같은



                        같지     않은



         rnax[,....,]   [］안의    값 중 최대값



         n血l[,....,]    I］안의    값 중 최소값




     3.1.4, 비트 언산자


         &              bit별   AND



         I              bit별   OR



         >>             八4SB가 왼쪽이라고 가정했을 1대I shift right.

                        侮gn bit는 그냥 연장시킨다．)



         <<             MSB가 왼쪽이라고 가정했을따1 shift left.

                        (LSB 쪽은 0으로 채운다．)




     3.1 .5, 할당언산자（廊닯gnment)


                        할당
                                                                   39



3.1.6. 간략기호小佃떼Tlonics)


    加lbf: 川帥ing le丘bit 丘rst

          여기서 left bit란 이 표준에서 쓰여진 bitstring 그대로 보아서 왼쪽이란

         뜻      이며, 이 le丘bit가 먼저 전송됨을 뜻한다. bits枉ing은 ' 10000001'고｝

         같이         single아iote mark로 둘러쳐서 표시한다．



    岫nsbf: Unsigned血把ger, most sign血cant bit小4SB）가 먼저 전송됨을 뜻한다．



    simsbf: Signed血妃ger, 2's complement 형태로 표시되며 入LSB bit(sign bit）가 먼저

             전송됨을 뜻한다．



    vlclbf: Variable length code, 여기서 left bit란 VLC C에e가 표어］ 쓰여진 형태 그

         대로 보아서 왼쪽이란 뜻이며left bit가 먼저 전송됨을 뜻한다. 또한 byte

         끼    리의 순서로 most sign而cant b外e가 왼쪽에 위치한다．
       MPEG
40     V山E0




     3.2. 복호과정 기술을 위한 통려1
     3.2.1. bit計ream syn伯x기술을 위한 방법
         Synt炚의 각 山姐항은 굵은 문자로 표시되고, 각 항목마다 이름, bit수가 나와

        있다. 또한 전송순서와 형태는 간략기호（mnemonics）로 나타내고 있다. 다음은

        이 표준에서 쓰이는 문장의 예를 표시한 것이다．


         while(condifion){data_element. . .   }                  만약 조건이 참이면 뒤의 d趾a element가
                                                                 실행된다. 이는 조건이 참이 아닐 때까지
                                                                 반복된다．


         面｛data_element.．小小le佃nd地on)                             data ele瞰沁가 적어도 한 번은 일어난다．


                                                                 이 조건이 참이 아닐 때까지 이 data
                                                                 e佃Tient는 반복된다


          if(condition) (data_element. . . }else{data_element)   만약 조건이 참이면 첫 번째I data element
                                                                 가 실행된다．


                                                                 만약 조건이 거짓이면 두 번째1 data
                                                                 element가 실행된다．


          如r(i=O;i＜心＋+)                                          data elen妃nt가 n번 실행된다．

          (data_element. . .)

         ／닉＜（刃mn妃nt 치                                            설명을 위한 부분으로 지워도 된다．
                                                           41



3.2.2. 함수의 정의


      bytealigned()
        현재의 위치가 byte의 가장자리에 있을 때 즉 bi始甘earn의 바로 디음 bit가

        한 byte의 처음 bit면 1을 나타내고 아니면 0을 나타낸다．



      nextb心（)
        Bits甘earn어］서 바로 다음 bit와의 비교를 의미한다．



      next_start_code()
        0으로 된 bit나 byte의 stiif五ng을 제거한 후의 그 다음 S恤t code를 나타낸다．




3.2.3. Reserved, forbidden, markeL bit


      reserved
       미래의 사용을 위하여 특별한 정의를 하지 않은 값．



     化rbidden
       이 표준에서 사용되어서는 안되는 값（start code와 같은 값을 피하기 위한

       이유 등으로）.



     marker bit
       Start code와 같은 값을 피하기 위하여 syntax상어］ 강제로 값이 " 1"인 한 bit

       를 집어넣은 것．
42




     3.2.4, 정세도
          정세도가 특별히 언급되지 않으면 마지막 정수 자리어四 큰 에러가 나치 않

        을 정도로 유지하면 된다．

          범위를 말할 때는   [, >, < 등을 이용하는더］, 예를 들어 [a: b＞는 a는 포힘하

        고 b는 포함하지 않는다는 것을 말한다．
                     VIDEO


              신택 스 와
              의미



Pic加re는 부호회하는 단위로 frame과는
다른 게념이다.             口C加re에는 frame
口C加re와 field picture, 2가지가 있다. 즉
卄ame단위로 부호호｛하면 frame 口伽re라
하고, field단위로 부호회하면 fie너 口cture
a｛ 힌다．
4.비트스트림 신택스와 의미

4.1. 부호화된 화상데이터의 구조
4.1.1. 비디2 sequence
 N    Progressive sequence와 Interlaced Sequence
      카메라로 영상을 얻는 더］는 두 가지 방법이 있다. 하나는 progressive scanning

     이고 다른 하나는 interlaced scanning이다.              그림 4-1에서 보는 바와 같이

   pro酊es前ye scannn堤은 순차적으로 주사하는 것이고, interlaced scanning은 한 line

     씩 건너서 주사하는 것이다．




                                                             1




             (a) progressive scanning             (b) in旭而ced scanning


                                                         汁（)P fi이d
                                                         :bo卄om field




             누   누    누         누   누   느m


             卜   누    누         누   누   卜




                          (c)
                     그림 4-1 pr지ress卜／e scanning과 intedaced scanning
                                                       MPEG
                                                       피DE0   45




     그림 午1에서 보듯이 progres없ye나 interlaced 모두 한 장의 화면이 같은 수의

    scanning 血ie으로 이루어짐을 알 수 있는더］ 이를 丘an妃이라 한다. 그러나

    interlaced scan恤唯에서는 인접한 두 血le간어］ 시간차가 있으므로 이를 2개의

    field로 나누는더］ 그림 午1 (c）는 이렇게 top field와 比ttom field 두 개로 나눈 것을

    나타낸다. top field는 위쪽 field를 bottom field는 아래쪽 field를 나타내지만

    入WEG2에서 이것은 디스플레이순서와는 콴계없다.              즉 top field가 먼저 디스플

    레이될 수도 있고 比仗om field가 먼저 디스플레이될 수도 있다. T아）, 蜘ttom field

    와는 관계없이 먼저 디스플레이되는 field를 first field라 하고 나중에 디스플레이

    되는 field를 second field라고 한다． 이와 같이 pr唯ressive scann血g어］ 의해서 얻은

    화상의 열을 pro얍essive sequence라 하고 interlaced sc而ng어］ 의해서 얻은 화상의

    열을 interlaced s叩ence라고 한다．



N    月C九ire

     Picli표e는 부호화하는 단위로 frame과는 다른 개념이다. picture에는 frame picture

    와 field pic山re, 2가지가 있다． 즉 fran配단위로 부호화하면 frame picture라하고，

    field단위로 부호화하면 field picture라 한다. 그림 千1에서 scan血垠방식과 무관하

    거］ (a）와 (b) 같은 frame단위로 부호화하면 丘a끄ie picture가 되며 (b）를 (c）와같이

    field로 분리하여 따로 부호화하면 field picture가 된다.        따라서 pro肛essive

    sequen凹에서는 field picture가 있을 수 없다．



N    C加아7功力nce. format
     색（chrom血an此）신호는 휘도（iwn血ance）신호어］ 비해서 해상도가 낮기 때문어］ 샘

    플수가 적어도 된다. 따라서 색신호의 표본화방법에 따라 chrominance format이

    다르게 되는더］ MPEG에서는 4:2:0, 4:2:2, 4:4:4的nnai을 규정하고 있다．
46




      (a)     4:2:0 format

      中2:0 format에서의 색신호와 휘도신호 화소들의 위치는 그림 午2와 같다.                                 여

     기서 색신호 화소의 위치가 수직축에서 휘도신호 화소들의 사이에 있는 것은

     색신호를 얻을 때 위치적으로 그 위치의 색신호값을 얻거나 또는 계산하여 써

     O} 한다는 것이다.            수평축으로는 중간위치를 잡지 않고 왼쪽 화소에 맞추었는

     더］ 원래 MPEG1에서는 중간위치어］ 있었다.                          그러나 ITU-R에서 권고한 CIR601

     화상들이 왼쪽으로 맞추어져 있기 I대문어］ 상호변환을 용이하게 하기 위하여

     入4PEG2에서는 이와 같이 변경했다. 따라서 휘도신호는 수직, 수평축으로 짝수

     이어야 한다.         시간축（把叫叩raldi爬ction）으로 본 샘플들의 위치는 그림 4-3, 4-4와

     같은더］ 그림 4-3에서 top-加idH血st=1이라는 것은 그림 4-1에서 top field가 시간적

     으로 먼저 디스플레이됨을 의미한다．



                       X         X    I    X     X   1   X    X     X      X
                                      I              I
                       O              ' O          ' O              O
                                      I            I
                       ><        乂    1 乂        乂 I X        X     ')<    乂


                       ><        X    1 X        X i     X    ><    )<     )<
                                      I              I
                       O              I   Q        1 O              O
                       )<        X    I   X      X I 乂        X     >(     X


                       ><        X    1 X        乂 1 X        X     )<     )<
                                      1              1
                       O              I C)          I Q             O
                       X         ><   I )<       >< i X       X     乂.     X

                             X            Represent lumin（그nce 5（그n耳)les
                             0            Represent chromonance samples

            그림 4-2 The position of luminance and chrominance samples. 4:2:0 data
                                     (MPEG IS: Figure &1)
                                                             47



                          T아）          Bottom
                         Field          Field

                           XO

                                        x

                          x
                                        0
                                        X

                         乂
                         O
                                        x

                         乂
                                        O

                                 虹no


그림 4-3 Verlic이（가d temporalP(＞엷加ns아san갸DIes in an inte的ced什ame咐h
             topji이dHflrst= ]     (MPEG IS : 日g내e 6-2)



                        Bottom           Top
                         Field          Field

                                         )<
                                         O
                          x

                                         )<
                         O
                         X

                                        乂
                                        O
                         x

                                         x
                         O

                                 切1e


그림 4-4 Vert奴批Dnd ten갸＞아계IDOS敞)flS of san갸이es in an싸e的ced的m帥府h
            topJ冷dH砒t= 0          (MPEGIS :日g내e 6-3)
                                  恥a皿e

                                   乂
                                   O
                                   ><

                                   )<
                                   O
                                   ><

                                   x
                                   O
                                   乂

                                   )<
                                   O
                                   乂

                                   加ne



그림 4-5 Verlic긔and ten가＞or긔pos敞＞ns of san갸긔es in（그progress爪／e frame (MPEG
                            IS: Figure o-4)



 (b) 4:2:2 format

 이 format에서의 화소위치는 그림 午6, 午7과 같다．


                            I            I        1
                    因    X I 因      >< 1 因     >< 1 因     :<

                    （己   乂 : 8      乂 : 8      乂 : 因      乂
                            r            r        r
                            1            1         1
                    0    )< i O     乂 i 0      >< 1 因     ><
                            1            I         I
                            i=
                                         r         r


                    0    >( 1 웅     X 1 웅      X I 因       X

                    0    X ' 8      'X I t8)   X r 8       乂

                    0    X i 0    >< i 8      X i 8    )<
                     X     Represent luminance s그mples
                     O     Represent chromonance samples

    그림 4-    The posiflon of luminance and chrominance samples. 4:2:2 d아a
                               (MPEG IS :日g내e 6-5)
                                                                                 49



                                                 Top          Bottom
                               Frame             Field         Field
                                0                  0

                                0                                  0

                                因                  因


                                0                                  0

                                0                  0

                                0                                  0

                                0                  0

                                0                                  8
       그림 4-7 Verflc（캬兀帥onsofsam口es w的4:2:2and4:4:4d아a
                       (MPEG IS :日gureo句



(c).4:4:4 format

이 如nn砒에서의 화소위치는 그림 4-8과 같다．



                   因       因           옹     8           因    因        因    옹

                   8)      因           召）    0           0    0        因    （因

                   0       因           (8)   亡8)         亡g   8)       因    0

                   0       因           0     0           召）   0        （豹   召）

                   0       因           0     0           0    0        0    0

                   0       0       0    邀）     返）   0    因     0
                       X         Represent luminance samples
                       0         Represent chromonance s아nples

   그림 4-8 The口osftion of un出）ance and chron出）ance san耳)1es4:4:4d（寸（그
                           (MPE（引S : 디gureo-7)
4.1.2, 움직임 예측과 DOT
    시간에 따라 변화하는 video sequence를 효율적으로 압축하기 위해서는 영상

   데이터가 갖고 있는 2차원 공간상의 중복성（redun由ncy）뿐만 아니라 시간축의

   중복성 제거가 절대적으로 필요하다.       MPEG에서는 2차원 공간상의 중복성을

   줄이기 위하여 殊釘（discrete cosine甘ansform）를 이용하며, 시간축외 중복성제거를

   위하여 움직임 보상방법을 이용한다．

    DCT는 2차원 축변환을 통하囚 데이터의 상관성을 제거하는 방법으로 picture

   를 bli乂k단위로 나눈 후 나뉘어진 각각의 block을 5장에서 소개될 DCT식에 따

   라 축변환시킨다. 이렇게 축변환된 데이터들은 한쪽 방항（저역 쪽）으로 몰리는

   경향이 있는더］ 이렇게 몰려진 데이터들만을 양자화해서 전송하게 된다.

    시간축으로 연속된 picture들은 주로 화면의 중앙부분에서 사람이나 물체의

   움직임이 있기 때문어］ 움직임 보상방법에서는 이러한 성질을 이용하여 시간축

   의 중복성제거를 행한다. 즉 화면의 변하지 않은 부분이나 움직였다 하더라도

   비슷한 부분을 바로 전 picture에서 가져와서 채움으로써 전송하햐 할 데이터량

   을 큰 폭으로 줄일 수 있다. 이렇게4血Lure 즈낟1에서 가장 비슷한 블록을 찾는

         예측(motion es山na如n）이라 하며， 엎마만큼 움직였는가 하는 변위를
   일을 움착암』

   낙타내는 것을.II婚血取如戒m라 한다. MPEG에서는 이 두 방법을 결합한 움직임

   보상-DCT(MCD-CT:mo如n compensated DCI）방법을 이용하고 있는더］ 이는 먼저

   움직임 보상만을 이용하囚 picture를 복원한 후에 그 복원된 picture와 원래의

   picture를 뺀 후 그 차이를 DCI를 이용, 코딩하는 기법이다. 그러나 뒤에 설명

   하겠지만 화면의 변화가 심한 picture나 macr아）뇨：k 등은움직임 보상을 이용하

   직,‘않고 단순히 DCI만을 이용하여 코딩한다.      이러한 경우를 加tra코뎡이라 하

   며 움직임 보상을 이용하는 경우를 茁噴코팅이라 한다. 움직임 보상은 휘도신호

   어］ 대해서만 행하며 움직임 예측방법들은 5장에서 설명한다．
                                                                       MPEG
                                                                       VIDE0    51




4.1 ,3. 디cture 加口e과 (:
                     7아＞
      MPEG2어］서 규정하는 picture 형태에는 I, P, B-picture의 서］ 가지가 있다．

   I(In甘a coded)-picture는 움직임 보상을 이용하지 않고 단순히 그 picture만을 DCI

   해서 부호화하는 것이고, P(Predic妃d coded卜picture에서는 I 또는 다른 P-I加tu托를

   reference로 삼아 움직임             보상을 한 후 나머지             차분을 D（了F한다.           또한

   B(Bidirection出ly pre小아ed coded卜picture에서는 P-picture처럼 움직임 보상을 사용하

   지만 P們cture와는 달리 시간축상에서 앞뒤에 있는 두 개의 frame으로부터 움직

    임 보상을 한다. 움직임 보상의 방향을 그려보면 그림 千9와 같다．


                        Bidirection出 Inte叩olation




                     그림 4-9 Exart耳)Ie of ten耳）on引 F永寸ure structure
                                 (MPEG IS 日gure卜］)



     따라서 入4PEG2의 Picture sequen此는 . . . . , B, B, I, B, B, P, B,B,P, B, B, . . .．와 같

   은 구조를 갖게 되는더］ 여키서 I-picture 전전의 B汭cture로부터， 그 다음 I-

   pictui   전의   P拉cture까지를 GOP(Gr叫p of pic恤回라 한다． 또한 그림 4-10과

   같이 GOP 내의 picture의 개수를 N이라 하고, I와 P-picture 사이 혹은 P와 P-

   까跏re 사이의 picture 개수를 M이라 한다．
52




                                     N
              //
                                 N
          BBIBBPBBPBBPBBPBBPBBIBBP. . . .
                   \    /               \   /
                     入4                   M


                                     그림 4-10 GOP구조



      위의 예는 N=18, M=3인 （刃P구조이다. 그러나 이제 B拉cture에서의 움직임

     보상을 생각하1 보면 B-picture는 시간적으로 뒤에 나오는 P 또는 I-picture를 이

     용하햐 디코딩（d凹od血g）할 수 있다. 예를 들면 그림 午11과 같은 구조에서 2번

     B-picture를 디코딩하기 위해서는 먼저 4번의 P-帥加re를 디코딩해야 한다． 따라

     서 송신측에서는 IPBBPBB . . . . 의 순서로 전송해 주어야 4번의 P肛ctu肥를 먼저

     디코딩할 수 있다.            디코더측에서는 이 순서를 원래의 순서로 되돌려서 디스플

     레이해야 한다． 따라서 入4PEG2에서는 B-picture 때문에 디스플레이되는 순서와

     전송되는 순서가 다르게 되며 디스플레이되는 순서를 "display order", 전송되는

     순서를 "transmission order"라 한다．



         At the enc에er mp此
              1 2 3 4 5             6    7   8   9    10 11 12 13
             I     B   B   P   B    B    P   B B      I B B P

         At the encoder output, in the coded bitstream, and at the dec에er input,
              1 4 2 3 7 5 6 10 8 9 13 11 12
             I     P   B   B   P    B    B I      B B      P   B    B

         At the dec어er output,
              1 2 3 4 5             6    7   8    9   10 11 12 13

                           그림 4-1 ] 如nsri宿敬＞n（가der오｝ d的回 order



       일반적으로는 그림 4-10과 같이 GOP구조를 설명하지만                                     入4PEG에서 규정하

     는 GOP구조는 이와 같이 N과 M값어］ 따라 고정된 것은 아니다.                                         N과 M은
일반적으로 개략적인 것을 표시하기 위하여 나타내는 파라메타이고 이                                                                               N과
M값이 하나의 s叩ence에서 불변인 것은 아니다. 예를 들어 그림 午12와 같이

羽叩en配가 시작하는 경우를 살펴보자．



   1 2      3   4   5   6   7   8    9   10   11 12     13   14   15   16   17   18   19
                                                                                                卜   dirplay
                                                                                            _
                                                                                                    。rder
   I   B    B P B       B   P B B        I    B    B    P    B     B   P     B   B      I


   1 4      2   3   7   5   6   10 8     9    13   11   12   16   14   15
                                                                            19   17   18 +                         "
   I   P B B P B            B    I   B B      P    B    B    P    B    B    I
                                                                                                    黔岫
                                                                                 B
                                                                                                              '幻
                                                                                      B

           fix밗 GOP                           羽corid GOP                    third GOP

                            그림 4-12 GC平에서 N과 M값이 달라지는 예



  GOP는 岫nsmis없on ordei를 기준으로 하면 I-拉cture에서 그 다음 I-picture 전까

지가 된다． 따라서                      d招히ay ord町로는 BBI로 시작하써 EBP로 끝나게 된다.                                                    이
와 같이 잡을 때 위에서 알 수 있는 바와 같이 sequence 중에서 first OC叩는 구

성이 약간 틀리게 된다.                            그러나 GOP구조가 다르더라도                               入4PEG으로 코딩된
bits仕earn에서 각 picture의                   종류를 알려주기 때문어］ 디코딩에 지장을 주지는
않는다.        또한 장면전환 같은 것이 일어나서 움직임 보상을 해도 소용이 없을

때는 P-I加ture가 와야할 자리에 강제로 I-picture를 집어넣어 intra coding을 할수

있는더］, 이런 경우에도 GOP의 N값이 변하게 된다.                                               따라서 M과 N, 또 G아）
구조는 편의상 설명하기 위한 것이지, 반드시 그와 같은 구조를 고정해서 사용

할 필요는 없다.               더 나아가 MPEG2에서는 P-picture 내에서도能螂瀜且毗에 따

라 어떤 ma口oblock은 I-翊pe으로 코딩할 수 있으며, B-picture에서도 macroblock마

다 I-翊pe이나 I九type, B－翊凹을 자유롭거］ 선택하여 코딩할 수 있는 유연성이 허용

된다. 왜냐하면 움직임 보상을 해도 오히려 I-type으로 코딩하는 경우보다 나쁜

경우는 picture 竝pe어］ 관계없이 ma町的lock별로 코딩 형태를 선택할 수 있기 11뀨

문이다．
1
    MPEG
    VIDE0
        V




4.1.4. 슬라이스（왜Ce)
        Slice의 정의는 원문 그대로의 표현을 빌자면 " a series of arb虹ary num比rof

      n追crobloc넌이다.   Slice는 적어도 한 개 이상의 m町oblock을 가져야 하며 slice

      끼리 서로 겹쳐지면 안 된다.              또한 slice구조는 매우 유연하여 매 picture마다

      구조를 달리할 수도 있다.           또한 그림 4-13과 같이 화면 전체를 다 메울 필요도

      없다.   그림 午13과 갇은 구조를 " general slice structure"라 한다．




                 勿     勿




               그림 4-13 The most gener이slice stru（寸ure (MPEG IS: 디gureo-8)



        그러나 이와 같은 Slice구조는 仕ick（확인을 위한 목적）mode에서 fast forward나

      fast reverse와 같이 slice를 건너띄어야 하는 경우어Ji.+ 특수한 목적을 위하여 주

      로 쓰인다. 보통은 그림 4-14와 같이 모든 macr的l(乂k을 다 포함하는 구조가

      많이 사용되는더］ 이를 "restiicted slice 誼ucture" 라고 한다.           이 그림에서 보듯이

      하나의 Slice는 다음 줄까지 꺾여서 이어지지 못한다.                       즉 Slice의 처음과 끝의

      m肛아加ck은 같은 수평열 내에 있어야 한다.                   Gener刻 slice구조에서 빈공간의 처

      리는 어떻게 해도 되며 MPEG표준에서는 정의되지 않았다．
                                                                  MPEG
                                                                  피DE0   55




             그림 4-14 Rest叱ted 引匕es打ucture (MPEG IS : 디gure 6-9)




4.1.5. 매크로 블록（Ma（걋야이oc目
    入4acroblock은 휘도신호와 그어］ 대응되는 색신호로 이루어지는더］ 디음 절에

   설명할 block을 하부구조로 갖는다.           chrominance format어］ 따라 macr아如ck의 구

   조가 달라지며 각 向rmat어］ 따른 ma町oblock의 구조는 그림 午15 시 17과 같다．

   이 그림에서 블록 내의 번호는 bh乂k nur沚er를 가리킨다. 入4acr小k乂k의 휘도신

   호를 DCT할 때는 frame DCT방법과 field DCI방법이 있는더］ 丘ame DCT 는 그림

   午18처럼 너］ 개의 block으로 쪼갠 다음 각 8 X 8 block어］ 대하여 DCI를 하는 것

   이고   fie닢DCI는 그림 4－四와 같이 각 field별로 서로              나눈 후 각각 2깨匠 쪼

   개서 DCI하는 방법이다.         ·한편 색신호는 chrominance 如m毗어］ 따라 다른더］

   4:2:2과 4:4:4凡nnat은 색신호의 수직쪽 해상도가 휘도신호와 같으므로 휘도신호

   와 같은 방법을 채택한다.         그러나 4:2:0 format에서는 색신호가 8X8밖에                  안

   되기 때문에                     ． 여기서 유념할 점은 이후에 설명
             丘ame DC'F방법만을 사용한다

   할 움직임 보상에서의 field나 frame prediction과 이 DCI에서의             field 또는 frame

                  . 따라서 움직임 보상을 field별로 했다 해서 DCI
   竝PC과는 무관하다는 것이다．
56




     도 field type으로 해야 하고 움직임 보상을 frame으로 했다 해서 DCT도 frame

     ty四으로 해야만 하는 것은 아니다.                그러므로 이 4:2:0 format에서 색신호의

     DCT를 包如叱口pe으로 고정했다 해서 움직임 검출에서도 加me竝pe만이 허용되

     는 것은 아니다．




                                      ［그            ［그
                               Y         Cb            Cr

             그림 4-154:2:0 Macroblock 針ruc仙re (MPE（引＆ 디g네e6-1 )




                        0
                            口             4
                                                    目
                     目口                   6
                                                    日
                            l: r         Cb            Cr

             그림 4-164:2:2 Macr丈)IOCk 針ructure (MPEG IS : 日gure6-11)




                       0
                           口         4        8
                                                  目9
                    目目               6    10      日口
                           Y             Cb           Cr

             그림 4-174:4:4 Macroblock 針ruc仙re (MPE（引S : Fig내eo-12)
                                                                  1

                                                                  MPEG
                                                                  피DEC   57




            그림 4-18 Luminance macroblock structure in frame DOT coding
                             (MPEG IS: Figure 6-13)




            그림 4-19 Luminance ri自아oblock s卄ucture in field DOT coding
                            (MPEG IS: Figure 6-14)



4.1.6. 블록（師Ok)
    미ock은     원화상의 복원된          데이터의 단위, DCT처리단위, 또는 그에 해당하

   는 "coded data element"를 의미한다.       MPEG2에서는 8乂8로 한다（sample수지血e

   수）   .
58




     4.2. 부호화과정과 비트스트림 신택스
         Syntax는 코딩된 뎨이터 （움직임 벡터와      DCT겨］수）를 전송하기 위하여 붇이는

        he耐江와 조건, bi曲ealn의 순서 등어］ 관한 것이다. 즉 데이터를 일정한 형태에 맞추

        어 운반하1 주는 운반수단이라 할 수 있는더］,t'띠？EG2 synt炚는 유연한 구조로 되어 있

        어서 조건이 많고 그어］ 따른 ex把nsion들이 많은더］ MPEG2 디코더는 어떠한 bitstiam

        이라도 入띠PEG2 syntax어］ 맞기만 하면 디코딩할 수 있다. 즉 syntax어］ 맞는다면 그 부

        분에 어떠한 떼이터를 넣더라도 디코더는 디코딩을 할 수 있다（물론 화면에 복원된

        그림은 아무 의미도 없겠지민）. 이러한 h띠PEG2 syntax를 많이 다루어 본 사람은 어렵

        지 않지만 이러한 구조를 처음 대하는 사람은 약간 어리둥절할지 모른다. 매개변수

        伽ran妃奴）들이 많이 나오고 그어］ 따라 디코딩하는 방법이 달라지게 되는더］ 마치 프

        로그래밍 언어식으로 되어 있다.      또한 읽다보면 도대체 왜 이런 것들이 필요할까

        하는 의문이 많이 들고 어떤 것들은 전문가어］거］ 물어보지 않으면 그런 응용여屠 생

        각하1 내기 쉽지 않은 것들도 있다. 그러나 몇 번 보면 이런 데에 익숙해지고 나중

        에는 syntax를 자유자재로 쓸 수 있으므로 변수 하나하나의 뜻을 짚고 넘어가는 것이

        필요하다.




     4.2.1 , 부호화과정과 버퍼제어
         Syntax어］ 나오는 변쉬pan毗r）들을 쉽게 이해하기 위해서는 부호화과정을 설명하

        고 넘어갈 필요성이 있다.     여기서는 그 중어］서도 버퍼제어부분을 상세하게 살펴보

        기로 한다. 그림 牛20에 入4PEG2의 부호화과정을 나타냈다. 그림에서 볼 수 있듯이

        Dcr블록의 입력은 쇼an可기 그대로 들어갈 수도 있고 움직임 보상된 加nt과 II게ltj斗

       中의짜이가 들어갈 수도 있다
                     ； 전자는 如蚣co如唯을 위한 것이고 후잔늪if坦9如g읖

        위한 것이다.   MP日｝에서의 움직임 보상은 앞에서도 설명했듯이 P四件과 B勺恥이

        있으며 또한 fie넌별로 움직임 보상을 할 수도 있고 flame별로 움직임 보상을 할 수도

        있다. 또한 P勺pe에서는 dual prime이라는 독특한 방법을 이용하기도 한다.
                                                                                        59




                                                    4                               1
                                                            1 ｛二二니 I3uife【卜
  frame input
                                  DCI
                                          니    Q啣       《


                \',r     "   et
                                                             니崙" F니 IDCT
                                                                              +

                                                    [
                                               Prediction
                              MV

                             motion
                                                              rame Stores
                             estimation

                                        그림 4-20 Enc的ing 블록도



 움직임 벡터의 탐색영역을 어디까지 하느냐에 따라서4冬9弗라는 변순가 결

정되는톄 찾아진 움직임 벡터를 그냥 전송하는 것이 아니고 이 f_code를 이용

하여 mo如皿co(妃와 mo如n邸k加al로 나누어 부호화한다. 또한 dua印血ne방식에

서는 ｛奴Mt的蟠＋는 움직임 벡터변위가 추가로 전송된다． DCr블록의 입력은

DCT된     후에            양자화佃uantisation）되는더］ 이                양자화에는          weigh山ig mati奴와

quantizer _sc심e呵把가 이용된다. Weighting m的奴는 각 DCT계수의 가중치를 나

타내는 것이고 quanti配r-－凹欲1code는 양자화 스텝을 결정한다. 이렇게 양자화된

후의 각 계수는 가변장부호화（VLC:variable len맘hc에ing）되는더］ intra bk乂k의 DC

계수와 그 외의 나머지 계수들로 분리되어 코딩된다. II血a block의 DC계수들은

dct_dc_size와 dc dct di卄erential의 둘로 나뉘어져 코딩되고 나머지 계수들은

MPEG2어］서 정하困 ＼兀C table을 이용하꺼 코딩된다.                                  위의 weighting m的奴는

sequence header나 quantizer matrix extension 부분에서 전송되고 quantizer_scale

Hc어妃는 slice와 macroblock어］서 선택적으로 전송된다． 이 움직임 보상과 DCT

ty［玘, 양자화등의 과정은 fl acro嫌坤（단위로 이루어지며 h出c札bloc蛇勺｛玘이라는 변

수를 통하1 이러한 코딩 형태를 알려준다.                                      즉 macroblock_口恥만 보면 그
60




     macr的lock이 어떠한 움직임 보상을 했는지, DCT계수가 전송되는지 아닌지，

     quan屯erH蜘e町妃가 전송되는지 아닌지 등을 알 수 있다.              또한 inter coding어］

     서 전송해야 할 계수가 없는 경우 이를 S뺘恥d macr的1o求이라 하는더］

     macr아）li乂k_addressjncrement는 이러한 skipped macr的ic兀k이 몇 개가 계속되는지

     를 나타내 준다. 또한 각 macr的ic乂k은 block별로 부호화 되는더］ macroblock에

     속하1 있는 b1兀k들이 코딩이 됐는가 skip됐는가를 나타내는 더］ 쓰이는 것이
            ChP
     鈿柯tibb托堪pa恥rhO이다. 이후 이러한 데이터들은 각종 header와 ex妃nsion, user

     data들과 묶여서 하나의 synt炚를 이루어 bu卄er를 통하1 디코더로 전송된다.               한

     picture당 발생 bit수는 가변적으로 b咐er의 충만도어］ 따라서 제어되는더1 이

     bu卄er가 underfiow나 overflow가 나지 않게 하기 위해서 인코더에서는 bu什er상타1

     를 항상 감시하고 있어야 하며 이에 따라서 다음 picture의 비트발생량을 조절

     하1 주어야 한다. 이러한 발생량 조절에 대해서는 入4PEG2어］ 기술되어 있지 않다．

     인코더에서 bu卄er를 10(刃분의 1초마다 조사하든 아니면 매 picture마다 조사하

     든 그것은 인코더의 자유이며, 만들기 나름이다. 결과적으로 주어진 b岫屯r량에

     대해서 underfiow나 overflow만 나지 않도록 해주면 된다. 그러나 이 작용이 최

     적화되지 않으면 정보량이 많은 picture어］ 비트할당을 많이 해주지 못하는 경우

     가 생기며 또 그 반대의 경우도 발생할 수 있다. 실제로 bu什er저1어를 어떻게

     하는가어］ 따라서 화질이 약 2-3dB 정도 차이가 나게 된다．

      入'IPEG2에서는 실제의 bu什er체계와는 관계없이 하나의 가상 buffer system어］

     대해서 언급하고 있는더1 이것이 바로加B欺叭d的bu地ring verifier）이다. VBV는 원

     래 virtu심bu什&ing verifier였다가 vi此ual이 video로 바뀐 것인데 이 처음의 virtual

     이 의미하듯이 이 VBV bu什er란 인코더가 실제로 갖고 있지는 않지만 인코딩을

     할 tt뀨 dec에er bu卄er의 상태를 똑같이 따라가기 위해서 인코더가 생각하고 있는

     가상 bu什er system을 말한다.    물론 디코더는 실제의 bu什er를 가지고 있으며

     bu侄er의 상태는 가상의 encoder bu什er상타따 동일하게 유지된다. Bu什er으1 동작

     을 나타내면 그림 4-21고干 같다．
                                    b
                               ，浪                      ,




             q口
                               "        LI.    -   >   I   '   )/.
                                                                                      61
                                                                     ( [ e (7




       그림 4-21 VBV Buff아 Occ叩ancy -（力耐an卄澍寸아e operation
                        (MPEG IS: Figure C-i)



 그림 牛21의 디코더에서는 기본적으로 일정한 시간간격마다 한4加u:i茹분외

LI第a尋 한꺼번에 VBV bu卄er에서 뽑아간다.                  이 양이 그림에서 山으로 표시되어

있다.   이 VBV 모델에서 디코딩하는 더］ 걸리는 시간은 없다고 가정한다.                                             따

라서 t=n일 U긔 ＼떠V buffer에서 제거된 n번째 pie加re data는 순식간에 디코딩되어

역시 느n일 U긔 디스플레이된다고 가정하는 것이다. 여기서 마P picture data를 뽑

아가는 시간간격（뇨l -Q은 보통 pro얍essive s叩ence의 경우 frame油宛의］曾수이며

T로 표시한다. 이 시간간격（뇨1 -Q은 경우어］ 따라 달라질 수 있는더］ 이는 뒤의

rei玘at_ 油t_field변수를 설명할 1대같이 설명한다.                 또한 B는 VBV bu什er의 크기이

며 각 시간간격 내에서의 직선의 기울기는 hi曲te인 R이 된다.                                            그러므로 bu拜er

의 입력단에는 매초당」Rb吐씩의 data가 계속 들어오고 출력단어］서는 T간격으로

口Hpi啣re의 data를 한꺼번에 뽑아가서 디코딩하고 디스플레이까지 한다. 그러나

디코딩을 맨 처음 시작할 때는 buffer 내에 아무 data도 없기 때문어］ bu卄er가

어느 정도 차는 것을 기다려야 하며 이렇게 bu什er를 채우는 테까지 디코더가

기다려야 하는 시간을 V枷Hd貞取퐈 한다. 이 vbv_delay는 MPEG!의 system clock
62




     인 90k1也의 주기로 나타내며 뒤에 나오지만 vbv_delay＝어好的B求7R로 표시된다．

     여기서 B木, 이란 그림 4-21에서 알 수 있듯이 t=n일 a뀨 VBV bu什er가 얼마나 차

     있는가伊］트 수）를 나타내는더］, 이띠1 picture의 시작을 알려주는 picture_start_code

     를 포함하Al 그 앞쪽의 header나 user data 등은 빼고 계산한다. 그림 4-21에서

     빗금친 직사각형으로 표시한 부분이 바로 이 header나 user data 등어］ 해당하는

     부분이다.    Vbv_delay식을 살펴보면 9000은 90KHz의 주기로 표현하기 위한 숫

     자이고 跣을 R로 나누어주므로 이 vbv_ delay는 디코더가 처음 시작할 a뀨

     buffer의 상태를 인코더의 bu珏er상태 즉 B水, 까지 끌어올려 주기 위해서 걸리는

     시간임을 알 수 있다. 이 V加코elay의 시간이 지나면 얻코더；의／加嫌才상태와 디

     코더의 bu拜er상태가 B木, 으로 동일하게 되고 디코더는 이때에 口H T초마다 그때

     의 picture data를 뽑아 디코딩할 수 있게 되는 것이다. 디코딩 준비를 언제라도

     할 수 있도록 하기 위하여 이 vbv_delay는 U긔I picture마다 필요하다. 이

     vbv_delay를 초로 계산하면 (vbvm由lay/90(刃0）초가 된다．

      디코더에서는 디코딩을 처음 시작할 따1 들어오는 sequence를 계속 감시하다

     가 어떤 pictur口start_c어把가 감지되면 그 pictu肥5恤IC에e의 마지막 byte가 지나

     간 바로 다음부터 V蜘_delay만큼 기다렸다가 미만큼의 data량을 뽑아가게 된다．

     얼마만큼을 뽑아가야 할 것인가는 디코더에서 바로 전의 n-i번째 picture_

     start_code를 찾으면 알 수 있는더］ 띠은 n번째 picture의 data와 그 앞의 picture

     header로 구성되며 또한 그 전어］ GOP header나 sequence header, extension 등이 있

     으면 그것까지 모두 포함된다.          이러한 과정에서 만약 buffer 내의 bit량이 B를

     넘어가면 overflow가 발생하고 또 d, 을 가져올 1대 buffer 내에 가져올 data가 모

     자라면 underfiow가 발생한다． 보통의 경우에서는 인코더의 buffer coi出아로 인

     해 underfiow나 overflow가 절대 발생할 수 없지만 다음에 설명할 low delay mode

     에서는 underfiow가 발생할 수 있다.      결론적으로 특정한 bits打earn은 특정크기의

     bu卄er를 가진 디코더를 가정하囚 코딩된 것이므로 디코더가 그 b畑仕earn에서 규

     정한 vbv_bu卄이1Si配보다 작은 bu卄er를 가졌다면 그 bit毗earn을 디코딩할 수 없
   거］ 된다. 이와 같은 이유로 뒤에서 설명하겠지만 sequence he川er어］서 최소한의

   ybv加抒er敬四를 표시하고 있다．




4.2.2. Lo＼사d이ay 모드
     MPEG2에는 low delay n均de라는 것이 있다. low_delay=1이면 low delay mode로

   들어가는더］ 이 如wd이ay변수는 配q畔n四e乂ten前on어］ 있다.                 I刃w delay mode에서

   는 B牡cture가 없다． 따라서 frame 재배열（reordering）이 필요 없고 그어］ 따른 지

   연이 없다． 이 low delay mode는 원래 visual telephony, video conference, monitoring

   등과 같이 지연시간이 짧아야 하는 응용에 쓰인다.                       I力刊delay m넜e에서는 I와

   P-picture밖에 없기 때문에 들어오늪.그대로 디코딩해서 디스플레이하면 된다．

   그러나 이러한 low delay mode에서 bu珏er의 unde出ow가 발생할 수 있는더］ 이는

   big picture가 발생할 It가 일어난다.      Big pi伽re는 코딩해야 할 데이터가 너무 많

   아서 뇨n일 I대 마어］ 해당하는 양이 bu卄er에 없는 경우 발생한다.                       즉 P-pictuire

   는 B-picture보다 움직임 보상이 좋지 않기 때문어］ P-pi曲re로만 계속 이루어지

   는 경우에 어떤 picture에서는 비트발생량이 너무 많아지는 경우가 발생한다．

   '] 와 같이 브］트발생량이 너무 많은 picture를戶培磁爵呼라 하는더I, 이 big picture

   가 발생하면 그 다음의 picture는 이 big picture 때문어］ 보낼 수 없게 된다.                    결

   국 big picture 바로 뒤의 picture들을 건너뛰게 되는톄 이를 skippedi心曲e라 한다．

   이렇게 picture의 건너뜀이 일어나면 picture의 temporal_reference는 건너뛴 picture

   수만큼 증가하게 되는더1 temporal-reference어］ 대해서는 뒤에서 다시 설명한다．

   간단하게 이 temporal_reference는 앞의 video sequence 부분에서 설명했듯이

   display order로 따져서 pi啣re의 순서를 나타낸다．
 MPEG
 VIDE0
 HJ




4.2.3. 계위（Sc（批그b附y)

        어떤 bits仕earn이 scalable하다는 것은 간단하게 말해서 코딩된 결과가 여러 개

      읜 브y트로 되어 있고 그중 몇 개의 layer를 이용해서 디코딩하느냐에 따라서 화

      상의 화질을 다르게 할 수 있는 기법이다. 일반적으로 연속된 2개의 layer를 생

      각했을 따1 아래쪽의 layer를 lower layer, 위쪽의 layer를 enhan凹ment layer라 한다．
                          b口弓e
      또한 가장 아래쪽어］ 있는 layer흩 base layer라 한다. 보통은 layer가 2개인 경우

      가 많으며 이 경우 base layer와 lower layer는 같게 된다． 따라서 표준에서는

      base layer와 lower layer를 혼동해서 쓰는 경우가 많다． 보통 base layer는 그 단독

      으로 디코딩이 가능하다. Enhanc이nent layer는 lower layer가 없이는 디코딩이 불

      가능하며 따라서 보통은 lower layer에서 reference frame의 디코딩이 끝난 후에

      또는 lower layer와 동시에 디코팅을 해야 한다.             이렇게 bits仕earn을 여러 개로

      나누는 이유는 뒤에 나오는 scalab小口의 종류를 보면 알겠지만 주로 lower layer

      에서는 낮은 해상도를 유지하는 대신 bit rate가 낮고 enhancement layer는 bit 수

      를 더해서 lower layer의 해상도를 높여주는 역할을 하기 때문이다．

        入4PEG2에서 언급하고 있는 scalabili口는 8pa叫 scalability, te｝甘伊）ralscalab小ty,

      冶l扼뇨刻a씨ity, 如a 們itition血g, hybrid scalabili口등이 있다． Spatial scalabilaty는

      er血ancement layer를 더해서 공간해상도를 높여주는 것이다． T由np이a1 scalability

      는 enhan此ment layer를 더해서 시간해상도를 높여주는 것인데 간단히 말하면

      base layer는 보통보다 낮은 frame rate를 갖기 때문에 enhancement layer에서 디코

      딩된 picture들을 base layer picture들 사이에 끼워 넣어줌으로써 시간해상도를 높

      이는 것이다.      SNR scalab小勺는 enhancement layer를 더해서 SNR을 높여주는 것

      이다.    또한 data partitionning은 채널상의 에러 등에 대비하기 위하여 코딩된

      data를 2개의 partition으로 나누어 bitstream을 구성하는 것이고 hybrid scalabili口는

      서로 다른 두개의 scalab皿口를 결합한 형태를 말한다．
                                                                   65




4.2.4. Syn幻x변수들의 내용
     入作EG2의 synt炚의 구성은 그림 午22와 같다.            중요한 정보는 주로 header에
   포함되어 있다.           한 sequen此에서 전체적으로 필요한 정보는 sequence header어］,

   편집을 위한 정보는 G아） header어］, 또 매 picture마다 필요한 정보는 picture

   header에 들어간다.        DCT계수와 m아ion vect아는 picture data에서 전송되고 또한

   여러 가지 ex把n前on들이 따로 전송된다． 먼저 嘲嗔ut針犯明軒에서는 화면의 毗e,,                       \




  코하咨s,Ct ratQ, 如me       砥已此V,h咀虹毗e, qu鈿四rmatrix 등 디코딩을 위하여 없
   어서는 안 되는 중요한 정보들이 들어간다. 그리고 G硏） head町에는 편집을 위
                                                                              뇨e寸x
   해서 이 GOP가 단독으로 쓰일 수 있느냐 없느냐 하는 것을 판단하기 위한 정

   보가 들어간다． 또한 芦q民恥如der어］는 temporaJ匕reference, picture_coding.jy件，
                                                                  vbv
  _delay 등과 같은 정보가 들어가는데 이는 대부분 이제까지 언급된 것들로서

  매 picture마다의 코딩에 관계되는 것들이다． Ek佃寸曲岩 강제적으로 항상 들어

  가는 嘲畔oce ex妃n駐on과 們蜘ec에呼e啣材c$n이 있고， 그 외 선택적으로 들어

  가는 여러 가지 ex妃nsion들이 있다．Sequence ex蜘sion에는 sequence header의 변수

  들의 값이 너무 클 때의 extension bit들이 주로 들어간다.              또한 picture c（뇌ing
  extension에는 한 picture를 디코딩할 U뀨 필요하지만 비교적 덜 중요한加tl之11(乙

  莎er竝on, t叩玉eld 血st, re倂at耐field，弦伊蜘1竝pe, 甲妃rn毗scan 등과 같은 변수

  들이 들어간다. 선택적으로 들어가는 ex佃通on중 se4配uce뇨輛毋自y 崩鈿喊on은
                                                                              e寸＼陟' 」『
                                                                                     "'
  video format이나 색신호，小splay size어］ 관한 것이다. 8啣呼＄油b柶e砥ension은

  scalab小ty를 이용할 I대 쓰여지는 변수와 scalable mode어］ 콴한 것이다.             伽ant
  mab奴e本旭flSi(月l은 quan血er mati奴가 색신호까지 필요할 I대 다운로딩（download岫）

  하기 위해 이용되며，pita埠小S타ay楙鉀雌on은 pan/scan을 지원하기 위한 것이다．

  Picture temporal scalable ex啣喊on은 tempoi川 sc싶ab小口를 쓸때 이용되는 변수들에

  관한 것이고, picture spati고sc싶able ex啣慽on은 spatial sc코ability를 이용할 때 이용되

  는 변수들에 관한 것이다.             마지막으로 copy right ex妃nsion은 코딩된 bit雜earn의

  소유권을 표시하기 위한 부분이다. Repe攷ed sequ이堆e으1 .각 羽叩ence he征匕r의 내용 /

  은 qual仙虹m毗奴 부분을 제외하고는 다른 변수들은 모두 같아야 한다．
66




                    'Sc）江EC 11172그




              * After a GOP the first picture shall be an 1-picture

           그림 4-22 High 1ev이 b什S打earn org아仁a如n (MPEG IS : 日gureo-巧）



      入WEG2 bit缸earn으로 동영상의 열을 코딩하려면 일단 picture들을 sequence로

     나누고 그 sequence 내에서 다시戶OP단위로 나눈다． 이렇게 나눈후에 S叫uence

     처음에 sequence header를 붙이고 다시 GOP단위로 GOP header를 붙인다． 그리

     고 각 pic如re마다 picture header를 붙인다. 그런뎨 MPEG2에서 이 G0P header는

     선택사항으로서 붙여도 되고 안 붙여도 된다. 또한 각 picture마다 picture header

     를 붙이는더］ 이 picture의 순서는 甘ansrnission order순서와 같다. 이 sequence

     header에는 앞에서도 설명했듯이 전체 sequence를 디코딩하는 더］ 필요한 정보들

     이 포함된다. 그러나 GOP header에는 closed召叩, broken_如k등과 같은 bit雜earn의

     편집과 관련된 정보들이 실린다. 여기서 우리는 sequence와 GOP의 관계를 살펴

     볼 필요가 있는더］, 한마디로 GOP는 편집을 위한 것이다. 처음에                            羽叩ence는

     방송의 한 프로그램, 또는 한 프로그램에서 광고와 광고사이 정도의 상당히 긴

     pic加re열을 생각하囚 만든 단위였다. 그러나 羽叩ence가 그렇게 길어지면

     sequence 중간에서 전원을 킨 디코더는 이미 지나간 羽叩ence header으｝ 정보를

     받을 수 없기 1대문에 다음 sequence header가 나올 때까지 기다려야 하며 ，복원

     어］ 필요한 정보를 받아보는 I카 상당한 시간이 걸리게 된다. 따라서 이와 같은

     문제점을 해결하기 위해서는 瓷quence를 짧게（해서 sequence header를 모두 같거1
                                                               I口        旬



    주면 되는데， 이러한 header 부분이 같은 sequence를 repeated sequence라고 한다．

    그림    午22의    孝는    이러한     repea把d   sequence구조를    나타내고      있다.    즉
    sequen凹end刃de가 나오기 전의 모든 sequence들은 repeated羽叩ence가 된다．

      그러나 이와 같이 Sc'：世ence길이를 짧게 하다 보면 이제는 하나의 sequence 내

    어］ GOP가 몇 개밖에 들어가지 않게 된다. 따라서 이와 같은 경우에는 a아）

    header를 없애고 그냥 羽叩毗e로만 대치하게 되었다. 그런데 \ICR 같은 응용예

    에서는 테이프를 중간부터 보지는 않으므로 羽叫ence길이를 짧게 할 필요는 없

    는 대신에 편집（editing）은 자주 필요하게 된다. 이러한 경우는 羽따ience길이는

    길거］ 하고 GOP는 자주 집어넣을 필요가 있다. 이러한 이유로 入4PEG2에서는

    GOP를 선택사항으로 두어 응용환경에 대처하게 하였다． Repeated sequence의

    header는 I나 P-I加ture의 앞에 오며 B-picture 앞에는 올 수 없다.               또한 field
    picture에서 한 &ime을 이루는 first오｝ second field picture, 중 두 번째 field picture

    앞에도 올 수 없다. Sequence_就심abi乞라啣通on과 sequence코ispla兄炚把nsion은

    repeated sequence에서 첫 번째 sequence header가 나오면 그 뒤에 sequence header

    뒤어匠 꼭 있어야 하며 만약 처음어］ 없었다면 그 뒤에도 나와서는 안 된다．



4.2.5. Syntax구조
     Syntax구조는 표 午1부터 표 4-24까지의 모든 표를 순서대로 살펴보면 알 수

   있다. 표午1이 synt炚의 전체구조를 나타내는더］, 이해를 돕기위해 이 표들을 한

   눈어］ 볼 수 있도록 그림 半23과 같은 흐름도를 그려보았다. 이 흐름도의 각 블

   록은 위의 표들과 대응되는더］ 각 표들에 대해서는 4.3절에서 설명한다. 각 표들

   은 프로그래밍 언어와 유사한 언어로 짜여져서 이해하는 더］ 큰 어려움은 없을

   것이지만 모르는 기호가 있을 때는 앞의 3장을 참조하기 바란다. 이 표들에서

   No. of b如가 표시되어 있는 곳만이 bit가 전송되는 부분이다. 따라서 뒷절에서

   의미를 설명할 때도 이 부분에 대해서만 설명하겠고, 또 그러한 것들은 표에서

   고딕체로 표시되어 있어서 눈어］ 잘 띈다. 단 유의할 점은 No. of bits가 1-11 (bits)
68




     로 표시된 경우는 가변장 부호화（variable length coding）를 사용하는 경우이다． 간

     략기호(Mn帥onics）에 나오는 기호들은 각 비트의 전송순서나 data type 등을 나

     타내는더］ program을 짜서 bitstream을 만드는 경우 자주 참조되는 부분이다． 간

     략기호（Mnemonic）으로부터 간단하게 많은 정보를 얻을 수 있으므로 필요한 경

     우 이 부분을 참조하기 바란다. 이곳에서 쓰이는 약자들은 3장어］ 있지만 다시

     써보면 다음과 같다．


      b引bp :t朮string, lef나朮伽St
      uimsbf : unsigned integer, most significant bit first
      simsbf : signed integer (twos complement), most significant bit first
      vlclbf : variable length code, left bit first



      참고로 MPEG2바stream의 예를 부록 2어］ 나타냈다．


                                               표4-1 Video Sequence
     video_sequenceO {                                                               No. of bits   Mnemonic
          next吼art下Od的
           sequence_headerO
           if ( nextbits() == extension_start_code) {
                 sequence_extensionO
                 do {
                 extens幻n and use乙da삐 0 )
                 do {
                       if (nextbits() == ：乂ip小start_c에e) {
                                 gr乂lp_of_pictures_headerO
                                 extension_and_ 上；er_data( 1)
                       }
                    picture_header()
                    picture_coding_extensionO
                 \\                    extensions_and_user_data( 2)
                      N.                    picture_datao)
                           \\.         加bile ( (nextb油0 == picture_sta恥어le) II
                                                  (nextbits0 == g乂lp_start_code) )
                                       if ( nextbits0 != sequence_end_code) {
                                              sequence_header()
                                              sequence_extension()
                                       }
                                   while (nextbit.s0 != sequence_end_code)
                 }else{
                                 ／串 ISO/IEC 11172그 永／
                  }
恥蜘-t            《                                               .
                                                                                                                @ 口Y[8A：品rE-5命仕H白／L
                                                      .



                                                                                          乂1B3: ce每5忘（t中岫S
            쿄                           '1比
                                    d
                    t附t尸凶少e,                                                囹
回 oxR'O : 1가t十나化尸 '
                                                                            @ 0乂t\3q : Q芦t,4d9忖寸（Me            E? 0치［3 ,3 : 伊仇m尸．th5才H
@ O川吐 : 弓t-leE戶 脚"叭， gtaar1                                                                JM小臼de
                g1｝比小ny卜 弓뇨rt                                               ＠八1Bn .· q%                                              .   d0口色
匈0乂1AR .,
                                                                          回 0乂 [e平 : 白叩．如『t- &,旋                                69
@ O乂I 13그： utCer qfts汁， Me
                                                                          9 아 [3e ., 工的小eM尸C心rIle

                                    sequence_end_code                                                   32             bslbf
                }



                                                                       표 4-2 日den引on and user d（그ta
                extension_and_user dala( i)                                                             No. of bits    Mnem이uc
                      while ( ( (i != 1) && ( nextbits0== extension_start_c넜e) ) II
                                    (nex由出I== user_缸之曲凡町le) ) {
                            甘(n以ti血sl戶＝extens幻n夕ait code )
                                                     extension_data( i)
                                              if ( nextbits()== user_data_start_code)
                                                     user data()
                            }
                }



                                                                             표 4-3 日dension d아（그
                    extension_thta( i) {                                                                 No. of bits    Mnemonic
                             while (nextbitsO== ex妃nsion_start_code) {
                                                extension start code                                     32             bslbf
                                                if (i == O) {／샤에ow朴因呻毗_extenslon() 치
                                                     if ( nextbitsO== "Sequence Display Extension표）")
                                                           sequence_display_extensiono
                            else                    else
                                                           sequence_scalable_extensiono
                                                }
                    /* Note: extension never follows a g oup_of_pictures_headen) *1
                         if (i == 2) { /半 follows picture_co五ng_extensiono *1
                                if ( nextbits()== "Quant Matrix Ex妃nsion ID")
                                       quant_matnx_extension()
                                else if ( nextbitsO== "Copyright Extension ID")
                                       copyright_extensiono
                                else if ( nextbitsO== "Picture Display Extension ID")
                                       picture_display_ex妃nsiono
                                else if ( nextbitsO== "Picture Spatial Scalable Extension ID")
                                       picture_spatial_sc띠able_extensionO
                                else
                                       picture_temporal_scalable_extension()
                                }
                        }
                    }
70




                                           표 4-4 Sequence he（了Jer
     sequence_header() {                                            No.（寸t吼S           Mnemonic
                   sequence_header_code                             32                 bslbf
                   hoi屯이北alsi配 value                                12                 uimsbf
                   vertic십 St配 value                                12                 uimsbf
                   aSPeCU沁ow匈nna由n                                  4                  uimsbf
                   framne rate code                                 4                  uimsbf
                   bit rate value                                   18                 uimsbf
                   marker bit                                       l                  bslbf
                   vbv buffer 自ze value                             10                 uimsbf
                   凹ns伽wed下缸게neters_flag                            1
                   load_intra_quantiser_mairix                      1
                   if ( load_infra_quantiser_matrix)
                               intra_quantiser_matrixl64]           甲64                urn咨bf
                   load_non_infra_quanti光r_niatrix                  l
                   if ( load_non_intra_quantiser_matrix)
                               'H札hitra 和antiser_m出ix[64]           附64                uinishf
                   next_start_code0
     }


                                                 표 4-5 User dat그
         user_data() {                                                   No. of bits     Mnemonic
             user data start code                                        극n              hslhf
             while( nex由itsO !=000000000000000000000001') {
                   U配rdata                                               8夾Cvt
             }
             next_stait_code0
         }


                                          표 4-6 Sequence e汁ension
         sequence_extension {                                            ！如. of bits     Mm叫叩m뉵
            extension start code                                         32              bslbf
            extension start code identifier                              4               uimsbf
             proflle_andJevel_indication                                 8               uimsbf
             profl鈿加e昶叩ence                                               l              uimsbf
             chroma format                                               2               uimsbf
             horizontal 寸ze extension                                    乃
                                                                                         uinisbf
             vertical 寸ze extension                                      2               uinisbf
             bit rate extension                                          12              uimsbf
             maker bit                                                   l               bslbf
             vbv buffer si：及三 exten前이l                                   8               uimsbf
             low delat                                                   l               uimsbf
             frame,크te extens加nfl                                         )              uimsbf
             frame rate extension d                                       \              uimsbf
             next_start_code()
         }
                                                                                                71
                                                                                        묘




                                  표4-7 Sequence display extension
sequence_(五splay_ex妃ns幻nO {                                              No.（寸bits     入1n1nonk
           extension start code identifier                               4             uimsbf
           video format                                                  3             uimsbf
           colour_d心cription                                             l             uimsbf
           if (colour_description)(
                       c어ourptimaries                                    8             uimsbf
                       transfer characteristics                          8             uimsbf
                       matrix coefficients                               8             uimsbf
            }
           d却lay_hon끄)ntal夕ze                                            14            uimsbf
           marker bit                                                     1            bslbf
           display_vei七（:alm尉；ie                                          '4           uimsbf
           next_st町tc以妃0
1




                                  표． 4-8 Sequence sc이야긔e exten엷on
sequence_scalable_extension() {                                          No. of bits   Mnemonic
           extension start code identifier                               4             uimsbf
           scalable mode                                                 2             uimsbf
           layer id                                                      4             uimsbf
           if (scalable_mode =="spatial sc出ability') {
                       lower_layer_pred批rnn上orizontalk_si肥               14            uimsbf
                       marker bit                                        l             bslbf
                       lower_layer꾸1氾毗lion寸妃rh洌寸i七                       14            岫ilsbf
                       horizontal_suhsamplin꿀_factor_m                   5             uimsbf
                       hI川zont吐subsan叩曲rig_fac加口l                        5             uimsbf
                       verhical_subsamp血g趾岫m                             5             uimsbf
                       vert岫Is山SalnP血姓fa由rn                              5             uimsbf
           }
           if (scalable mode =="temporal scalability")
                       pict띠e_mu乂enable                                  l             uimsbf
                       if (pict口re_mux_enable)
                                 mux_to_pn名代S前ye_sequence                l             umisbf
                       picture_mux_order                                 3             uimsbf
                       1出：t口re1mux f出：h才                                 3             uimsbf
           }
           next_start_code()
}


                                      표 4-9（갉oupofr이ctures he（그der

gm叩O댜,ictures上eader() {                                              No. of bits        八nemonic
       gr川lp_start_code                                              극）                 bslbf
       血ne code                                                      7S                 bslbf
       (：岫ed召op                                                      l                 岫sbf
           bn出en link                                                l                 미m由f
           next_start_code()
}
72




                                        표 4-10 디ctu爬）he（그der

     picture_headerO {                                                      No. of bits   Mnemonic
                picture_start_code                                          32            bslbf
                 tempor沚reference                                           I0            uimsbf
               picture codin邕tyF比                                           3             uim.sbf
               vbv_delay                                                    16            uln暾寸
               if (picture_coding_type == 211 picture_coding_type == 3) {
                           I吐-l났如rward_ve梵or                                1
                            forward f code                                  3             uinisbf
                }
               寸（picture_c（넘加gtype==3 ) {
                          f川니Pel_backward_vector                            l
                          backward f code                                   각             uimsbf
                }
               while (nextbits() == '1' ) {
                           extra b吐picture       『iththev田ue "1" 承／
                                              ／水＼人                          l             uimshf
                           extra in伽mation_pict出e                           8
                }
               extra_bit_ 耐ure         /* with the value '0" 木/             l             uim.sbf
               next_start_code()
     }


                                   표 4-1 ] 다cture coding exten듸on
     picture_coding_extension() (                                           No. of bits   Mnemonic
                 extension start code                                       32            bslbf
                 extension start code identifier                            4             uim.sbf
                 f_code(O][O]         ／샤brward hoi切川al 串／                   4             uimsbf
                 f_code[O][1J          幷fo'가 『ard ver伽川 永／                  4             uim.sbf
               f_code[11[O]           /* backward horizontal永1              4             uimsbf
               乙：ode[1][l]                   『缸d ver七c키 치
                                      戶 back14                              4             uinisbf
               intra_dc_precision                                           2             uimsbf
               picture_structure                                            2             uimsbf
               top_field_flu暾                                               l             uimsbf
               frame_pred_frame_dct                                         l             uiinsbf
               concealment motion vectors                                   1             uln咨bf
               q_scale_ty：比                                                 1             uimsbf
               intra vlc format                                             l             uimsbf
               alternate scan                                               1             uimsbf
               repeat_first_field                                           l             uimsbf
               chroma_420_ty比                                               l             uin咨bf
               progressive_frame                                            l             uimsbf
               composite_display_flag                                       ]             uim.sbf
               if ( composite_display_flag) {
                            va航s4                                           l             uimsbf
                           field_sequence                                   극             uimsbf
                           sub carrier                                      l             uim.sbf
                           burst_amplitude                                  7             uin咨bf
                           sub_carrier_phase                                8             uim.sbf
                }
                                                                                MPEG
                                                                                피DE0         73




          nextH' start codeo
}


                                표 4-12 Quant mc그十rix extension

quant_matrix_extension() C                                        No. of bits     Mnemon乂
           extension start code identifier                        4               uim.sbf
           load_intra_qua北ser_matrix                              l               uimsbf
           if (load_in岫르uantiser matrix )
                       II吐r2匕quanhis町luau奴［64]                    8 永（놔           uim.sbf
           load_non_intra_quantiser_malrix                        l               uini.shf
           if ( load_non_intra_quantiser_matrix)
                        non_intra_quantiser_mat敬[64]              8 永 64          uimsbf
           load下hrom也毗1包quanliser_mati缸                           l               uim.sbf
           if ( load_chroma_intra_quantiser_matnx)
                       chrom艮intra시uantiser.皿ati뇨西4]              8 木 64          mm屯f
           load_chroma_non_intr匕quanliser_matrix                   1              uimsbf
           if ( load_chmma_non_intra_quantiser_matrix)
                       chroma_non_intra_quantiser_matrix[641      K 卞 64          uimsbf
           next start code()
}


                               표 4-13 F기cture disF이（그y exten없on

미ctur口毗play_ex妃nsion() {                                          No. of bits     Mnemonic
        extension start code identifier                           4               uimsbf
        的r ( i=0; izriumber_of_frame小此ntr口硝配ts; i++ ) {
                      frame centr三 horizontal offset              16              sim.sbf
                      m別rker bit                                  l               bslbf
                       frame centre vertical offset               16              sinisbf
                       marker bit                                 1               bslbf
           }
           next_start_code()
}



                     표 4-14 Picture十en갸＞or싯Sc이야여e extension
pictun_tempora1_sca1ab1e_extension() {                            No. of bits     Mnemornc
          extension start code identifier                         4               uimsbf
           reference select code                                  2               uimsbf
           forward tern rai reference                             10              uim.sbf
           01刈rker bit                                            l               bslbf
           backward_temporal_reference                            10              uimsbf
           next_start_code()
}
     S
         MPEG
74       피DE0




                                      표 4-15 미cture斗刃ti이SC(水그ble exten引on

                pictur口_spatial_scalable_extensionO {                                 No. of bits    入4nemonic
                            e쩍tension start code identi丘er                            4              uimsbf
                           lower_layer_temporal_reference                             10             uimsbf
                           m町ker bit                                                  l              bslbf
                           lower_layerho寸끄）ntal offset                                15             simsbf
                           marker bit                                                 l              bslbf
                           lower layer vertical offset                                15             simsbf
                           spatial_temporal_weight_code_table_index                   2              uimsbf
                           Ii）恥r_layer_ 吐어꾸心5加e士ame                                   l              uimsbf
                           lower_layer_deinterlaced_fleld_select                      l              uimsbf
                           next_sta凡code()
                }


                                               표 4-16 C야Dyri아卄exten삶on
                copyright_extensionQ{cop                                              No..of bits    人lnemomc
                           extension start code identiflerextestart code identifier   4              unim.sbf
                           co巾yright_flagc叩川帥t_flag                                   1              bslbfbslbf
                           copyright_identiflercopyright_idenhi丘er                    8              Un加i.sbf
                           original_or_copyoriginal_or_copy                           1              bslbfbslbf
                           reservedreserved                                           7              unimsbf
                           marker bitmarker bit                                       1              bslbfbslbf
                           copyright_number_lcopyright_n네mher_1                       20             unimsbf
                           marker bitinarker bit                                      l              bslbfbslbf
                           copyright_number_2copyright_number_2                       22             unimsbf
                           marker bitmarker bit                                       l              hslbtbslbf
                           copyright_number_3copyright_number_3                       22             unimsbf
                           next_start code( )next_start codel)
                }}


                                                    표 4-17 다cture d아a
                picture_data() {                                                      ！늬o. of bits   Mnemonic
                            do {
                                       sliceO
                           }w川le ( nexthits() == slice_start_code)
                           next_start_codeO
                }
                                                                                                MPEG
                                                                                                니DE0        75




                                                   표． 4-18    왜ce

sliceo) {                                                                         No. of bits     Mnemonic
                出ce start code                                                    32              bslbf
            if (vertical_size >2800)
                      slii叱yerfic심_ K好ition_extension                             3               urn咨bf
            if ( csequence_scalable_extension() ispresent in the bitstream> )
                      if (scalable_mode == "d毗a partitioning")
                            F1如'it兄breakpoint                                     7               uirn的f
            quanliser_scale_code                                                  5               uimsbf
            il (nexthitsO=='l ') {
                    slice_extension_flag                                          l               bslbf
                    intra slice                                                   l               uimsbf
                    slice下如山e id en的le                                            l               uimsbf
                    slice_picture_id                                              6               uimsbf
                    while (nextbits() == 'I' ) {
                            extra bit slice           ／永 with ti比 value "! " 水／   1               uim.shf
                            extra information sli氾                                8
                    }
            }
            extra bit 到ice ／水 \vith 山cv고ue "0" 半／                                 l               uimsbf
            do (
                    macrobl어：kO
            }while ( nexthitsO != ' )00 0000 0000 0000 0000 0000')
            next_start_code()
}



                                            표 4-19       M아才（)block

ma（江ob!야：kO {                                                                     No. of b此；      八/lnemornc
       꿔hile (nexthits() == '000000아 以刃9
                     macroblock_escape                                            II              bslhf
            macroblock address rncresnent                                             I-   Il     vlclhf
            macmb!ock_modesO
            if ( macroblock_quant)
                     quantiser_scale_code                                         5               urn사寸
            if (m孤an뱌乂kmo由兀拓IW毗 n
                     (rnacmblockmtra && conceahnent1motion vect이旬)
                     motion_vectors( 0)
            if ( rnacmb!ock_motion_backward)
                     motion_vectors( 1)
            if ( macroblock_intra && conce田ment_motion_vectors)
                     marker bit                                                   l               hslbf
            以 macrobli乂k_pattern )
                   0넜ed上뇨：k_r帥帥0
            如r ( 느0; i小奴놔玔nt; i++) {
                    block( i)
             }
 }
     MPEG
76   니DEO




                                            표 4-20 Macroblo아（modes
            macn刑吼뇨呱des0 {                                                          No. of bits   Mriemornc
                       macroblo出_type                                               1-9           미clhf
                       if ( (spatial_temporal_weight_code_flag == 1) &&
                               ( spati出ten好刑wei帥下（)de I址此_index != '00') ) {
                               SpaliL娩mporal_weightcode                             )             uimsbf
                        }
                       if ( macmblock_motion_forward II
                               macmblock_motion_backward) {
                               if ( picture_st끄cture == 'flame') {
                                   if ( fmme_pred_frame_dct == 0)
                                               frame_motion_type                    2             uimsbf
                               }else {
                                                field. motion_type                  2             uimsbf
                               }
                        }
                       if ( (picture_stnlcture == "Frame pict山e") &&
                                (frame_r月e也鈿ne dct==0 ) &&
                                ( maCm바乂k ii出a Ii macobli乂k_patt帥) ){
                               dcl type                                             l             uim.sbf
                        }
            }



                                                표4-21 Motion vectors
            motion_vecto八 ( s) {                                                    No. of bits   Mnemonic
                       if ( motion_vector_count == 1) {
                                   if (( mv_format == field) && (dmv != 1))
                                               motion_vertical_field_select[0][s]   l             uirn.sbf
                                   motion_vector( 0. s)
                        }else{
                                   motionyertic川_fie1d_select[01[sj                 l             uimsbf
                                   motion小vec幻r( 0, s )
                                   molion_verlical_field_select[11[s]               l             uimsbf
                                   inotion_vector( 1, s)
                        }
            }
                                                                                         MPEG
                                                                                         미DE0




                                       표 4-22       M아ion vec幻r

motion_vector ( r, s) {                                                  No. of bits       Mnemonic
            motion_code[r][sjtO]                                          11
                                                                         1-
                                                                                           vlclbf
            if ( (f프넜e[s][0] != l) &&(moti이L프xle[r]圄［0] != 0) )
                       m此on r心恤ialft][s][O]                              卜8                uimsbf
            if (drnv== 1)
                        drnvector[O]                                     1-         2      미clbf
            mofion_code[r][s][1]                                         1-11              vlclbf
            if ( (f_code[s][1] != 1) && (motion_code[r][s][ I] !=0) )
                         molion_residual[r][sl[1]                         1-        8      uimsbf
            if (drnv == 1)
                          drnvector[1]                                    1-        2      미clbf
}


                                   표 4-23 Coded block p그卄em

coded_block_pattern 0 {                                                  卜幻．of bits        Mnemonic
          coded_bl乂k_pattem_420                                          3-9               미clbf
          if ( chroma幻rmat==4:2그）
                          coded_I必ock_patt巴n1                            )                 uimsbf
            if ( chroma_format == 4:4:4)
                        C에ed bi어：kpa如rn2                                 6                 uimsbf
}


                                             표 4-24 日（Dck

block( i) {                                                              No. of bits       Mnem이끄c
      if ( pattem_code[i] ) {
             if ( macroblock_intra)      {
                         if ( i<4) {
                                       dct dc 前ze lumllinance             2-9              vlclbf
                                       if(dct_dc_size_luminance !=0)
                                                   dct dc differential         I-   il     uimsbf
                          }else{
                                       dct dc size chrominance             2-10            vlclbf
                                       if(dct_dc_size_chrominance !=0)
                                                   dct dc 血derential           1-   il     L山nsbf
                          }
             } 타se {
                          Fi八t DCI' coefficient                               3-24
             }
             while ( nextbits() != End of block)
                         Subsequent DCI' coefficients                         2-24
             End of늬ock                                                       2 or 4       vlclhf
       }
 }
78




                                                                 그림 4-23 Syntax의 흐름도




                                                                         sequence_header()
                                                                              포E 4-4


                                                                        sequence_extension()
                                                                              포[. 4-6




                                                                                                         f( iclure_starl_code)
                                                   if(extensio       I_code)


                                                                                                                                                 em기




                                          extension_start_code()                            if(user_da      start_code)
                                              oo00 이 B5(H)

             if (sequence_display                                                                                         if (user_
                                                          sequence_scalahle_
              ex妃nsion_ident汗 I.)                                                                                             山ita
                                                        ex , ision_identilicr)


                                 sequence                 sequence_
                                                                                                                              點
                                                                                                               user.dataO
                                 display                  scalable
                                 extenson()               exlenson( )
                                                                                                                 표 小S
                                  포[ 4刀                    王E 小8



                                쿠
         L
                                                                                          가往lensi아l
                                                                                           start_code)         if(grcup
       if(extension.            .jtart_   c。
                                           de)          if(user)_data_start_co山)                               starl나 ;ode)




                1111111111111
                                                                      if(group_slazl_code)


                                                                                                                                      if(piclui e
                                                                                                              GOP_headerO             start_ccile)
                                                                                                                포[ 小9
                                                                                                     if(user (Ja(a \\            If
                                                                                                                                   (p油ureb
                                                                                                      start_c以Je)                start_C八Je)

        Extension
            &
       User 부분                                                                                                 user_daia()
     ( 표 小2, 표 4-3 )                                                                                             표 4呑
                                                                                                                    ＼七皿少町 ata
                                                                                                                      start_code)
                                                                 if(picture_start_code)



                                                                                                             까ctur（乙header()
                                                                                                                표 4-10
                                                                                                                                                      79



                                                                그림 4-23 계속




                                                                picture_coding_extension()
                                                                         표 4-11


                                                                                                              ice_start_code)



                                             +
                                    if(extensio             ,    _c어｝   e)      if(user.    _由ta_          art_c。
                                                                                                                de)
                                               if(extension_start code)                                                                    Extension
r
                                        f
                                                                                _
                        +--
                                    -                                                                                                          =＆느1
                                                                                                                                                      mh




                    ex妃nsionU亂缸t_code( )                                                                                                   User 부분
                       0000 01B5(H)                                                                                                         ( 표 中2,
                                                                                                                                              포1 4-3 )


                                              if(picture_                           if(picture_
      if(Quant          if(copy
      matrix                                  S ' L                                 佃aporaL
                        eXtens nigh'韶：           alab                               scalable
      exteflstjO                                  ;-
                        idetifi )   eXtIjSon_ cx son                                     nson
      identif )
                                    ident     identi   r)
                                                                                    1denS
      Quant_                                picture_                    picture_               picture_
      matrlx_           copyright_          display_                    spatiaL                temporal.
     extenstion()       extenson()          extenson()                                                                                user_data()
                                                                        scalahle_              scalahle_
                                                                        exlenson()             extenson()                              표    中-s
      표     4-12              표 4-16         표 4-13                      표 4-15                 표 4-14




if(extension_start_code)
                                                                        if(user_data_stai-t_code)



                                                                                                            if(sli " _       _code)
                                            if(slice_st                 code)




                    尸
                                                                                      ! !                   Picture Data 부분（표                中17)
                              if(slice_start _code)                          없ice()

                                                                          표 4-18




                                                                                                                                            0D0D
                                                                                                    if(sequence_斗eader_c에e)

                    L                                                                               if(group_star_code)

                                                                        if(sequence_                if(user_data_start_code)
                                                                          end_
                                                                               ;ode)                if
                                                                                                         (picture_start code)
                                                                                                                         _
                                                                 sequence_end_code()
                                                                    00000 B7(lI)
                  그림 4-23 계속 딕cture d아a（引匕eQ）부분




sliceO: picture da呵motion ye아아S 十 DCT 꼐수）를 전송하는 부분（표 午18)
   do (
          macroblok() : 한 macr야）lock의 data를 전송하는 부분 （표 4-19)
              macr야ilock_modes() : 한 macr아）lock의 type을 전송하는 부분
                    macroblock_quant, macroblock_motion_forward,
                    macr야)lOC뇨motion_backw町d, macr야加ck_intra,
                  macr아寸ock_patter등이 여기서 결정된다．（표 午20)
             if(macr야加味_motion_forward II
                  (macroblock_intra && concealment_motion_vectors)) {
                    motion_vectors(s) : forward m아ion vectors(s=0）를 전송 （표 牛기）
                        if(motion_vector_count==1) (
                             motion_vector(0,s) : motion ye아아가 하나인 경우
                                                  first motion vec恤를 전송 （표 +22)
                         }
                        else {
                             motion_vector(0,s) : motion ye아아가 두개인 경우
                                               first mo如n 比아아를 전송 （표 小끄）
                             motion_vector(1,s) : m아ion ye아아가 두개인 경우
                                              second motion ye아아를 전송（표牛끄）
                         }
              }
              if(macr아加昧mo如n_backward) {
                    motion_vectors(s) : backward motion vector(s=l)를 전송 (A 4-2 1)
                         상동
              }
              if(macrohlock_pattern) {
                     coded_block小pattern() : 한 macr아）lock 내의 블록들의
                                             coding 여부를 전송 （표 +23)
              }
              for(i=0; i<hlock_count; i++) {
                     닒ock(i) : macr的lock내의 각 블록(i)에 대해서
                               DCT 꼐수를 전송 （표 午24)
              }
    } while(nexthits0!='000 (1000 (1O00 0000 0000 0000')
                                                                                         81



4.3. 비트스트림의 각 변수의 의미와 조건들
4.3.1. Sequence Header
      sequence_header() {                                         No. of bits   Mnem이MC
                 sequel砒j固der_code                                32            bslbf
                 horm只lal 前：配 value                               12            uimsbf
                 vertical 茁：四V曲le                                 12            uimsbf
                 a斗心幻a由如formati（月l                                4             uimsbf
                frame rate code                                   4             uimsbf
                bit_rate_value                                    18            uimsbf
                marker bit                                        l             bslbf
                 vbv buffer 自：配 value                             10            uimsbf
                （刃nstraine吐下aran 吐豆flag                           l
                ba也inti也qua批iserinatrix                           l
                寸（岫也iiilra_quan出er_mafl奴 )
                            int日_quantiser_matrix[64]             甲64           uimsbf
                boad_non_intra_quanliser_matrix                   l
                if ( l대ad_non_intr뇨quantiser_matiix)
                            non_intra_quantiser_matr1x164]        附64           uimsbf
                next_start_codeO
      )



     sequence_header_code : 32 bits

          -00001B3 (H)（여기서 (H）는 hexa妃ciinal을 나타낸다．)



     horizontal size value: 12 bits

          - 화면에 小splay하는 영상에서 휘도 신호（Y coi珥兀I妃nt)의 horizontal_

            size(14 bits)의 LSB 12 bits.

          - 반드시 macrobkx火의 배수가 될 필요는 없지만 12비트 모두 0이 되는것

            을 방지하기 위하여 horizont川j配는 싻)96의 배수는 될 수 없다．

          - 이 값은 macr아六乂k의 배수가 아닐 수도 있기 I대문에 가로 방향의

            macrobli乂k 개수를 나타내는 macro뱌乂k wid血伽b_width）는 다음과 같이

            계산된다．



                               mb_width=(honzontal_size+15)/i 6
82




        （이 경우 그림 午24와 같이 왼쪽으로 정렬시킨다．)


                left 田igi比d
                     '" ,.
                         "'




                                                      thspla3娘ble pe工t

                              그림 4-24 mb wid十h



     vertical size value: 12 bits

        . 화면에 display하는 영상에서 휘도신호（Y component)의 verticalmsize(14

          b畑）의 LSB l2bits

         - 그림 4-25와 같이 위로 정렬시키며 progerssive sequence인 경우에는

           mb如坦ht를 아래 식과 같이 꼐산하고 progressive sequence가 아닌 경우

           에는 frame picture인지 field picture인지에 따라서 각각 그림 午25와 같이

           계산한다.



             mb_height=(vertica匕size+15)/i 6 (for progressive sequence)
                                                                                             MPEG
                                                                                             니DE0     83
                                                                                               1그




                                                top 띠ig工出（l
                                         /../



                                 .//"




                       J/
                            "




    nib加培lit = 2게＜(1/artica1_s끄e + 31 : 32                    mb_lieight= ( 'ertica.1_size + 3l)/32

             (a) fra끄e pictuxe                                           (b) fi三id picti끄E

                                        그림 4-25 mt兀height



    - veritc카jze가 4096의 배수가 되지 말아야 한다．



Aspect_ratiojnformation : 4 bits

    - DAR(di旦pl y pectrati이는 디스플레이되는 화면의 세로 다L가로 비를 말

      한다．

    - SAR(sam히e aspect rati이는 한 화소의 세로 대 가로 빈릎 말한다．
   1 표 4-25와 같다．


             표 4-25 as口ect了켸OJfl幻rmation (MPEG IS : Ic刈e 6-3)

 aspecLratio_information                  Sample Aspect                                DAR
                                             Ratio
           0000                               如rbidden                              forbiddeen
           0001                         1.0 (Squ缸e Sample)
           ()（끄0                                                                       3三 4
           0011                                                                       9 三 I6
          아00                                                                         I --2.21
          0101                                                                       reserved

           1111                                                                      reserved
frame rate c에e :4 bits

   -fran妃1ra妃는 원칙적으로 다음 식과 같이 결정된다．



              戶ame나ate＝戶口me나口teX (/7i7刃2e小r口te小e工tensjonHn+1)
                                 (frame_ r口te e工tensii刃l d+ ]\



     （여기서          fram乞rat乞炚把nsion_n과    fran妃1ra虹ex把nsion크는       sequence

     eX妃ns幻n에서 전송된다．)

    = 그러나 frame rate val出가 표 午26과 같이 정하쪄 있으면 그때의 丘ame

      rate는   frame_rate_val出가   되고      frame rate炚出ision工과      frame1rateH

      extension_d는 0이 되어야한다（표 午26어］ 보면 각 경우가 모두 정해져

      있기 때문에 위 식은 현재까지는 사용할 필요가 없으며 미래를 위한

      것이다）.

    - field批妃는 frameHra妃의 2배이다．


                표 4-26 的me ra怡 V이ue (MPEG IS : T그ble 6匈

  丘帥ne rate code                         丘ame rate v出ue
  0000                                   如rbidden
  0001                                   24 000 + 1001 (23.976)
  0010                                   24
  0011                                   25
  아00                                    30000 + 1001 (29.97)
  0101                                   30
  0110                                   50
  0111                                   60 000+ l001 (59.94)
   1000                                  60
                                         reserved
   1111                                  reserved
bit rate value          : 18 bits
   - bit_ ate(30 bits)의 LSB l8bits.

   띤 多bits!毗단위로 계신如unded upw可dj （즉 예를 들어 32*400 +25이면
           33永400으로 계산해서 33을 bit_rn妃값으로 전송한다）.

   - 이 값은 실제전송률 R과 다르다佃)Uflded 따叭ward시켰으므로）. 이 값은

           VBV bu卄er 작용에서의 최태 bit rate가 되며 따라서 단순한 상한값만읔

           젠골해H歪단二 톺정小油如am은 특정전송률을 가정히弘a 부호화된 것이

           기 I대문어］ 전송률읖＋정한최 않은 상태에서 bu珏er크기를 정할 수 없다．

           따라서 전송률의 상한값을 알고 있으면 buffer크기가 정해져 있을 U뀨

           그 bits仕earn이 복호화 가능한지 아닌치를 알 수 있다．

   = 0값 H 사용불가．



marker bit          : 1 bit

   -   H   l   11




   . 이런 marke乙bit는 아래위의 변수 중 0만 계속 나올 가능성이 있는 곳

           어］ 삽입하게 된다
                    （ 0 이 계속 나오면 없art c어妃와 혼동될 염려가 있다．).



vbv buffer size value               : 10 bits
   - vbv_buffer_size (18 bits)의 LSB lObits.

   - 최소 vbv bu什er size B를 다음과 같이 계산한다．



                              B=16*1024*vbv_buffer_size(bits)


   - 앞의 4.2.1절에서도 언급했듯이 bitstream은 특정한 buffer를 가정해서 부

           호화한 것이기 U뀨문에 그 bit毗凹m을 복호할 수 있는 최소 vbv bu卄er크

           기를 정하1 주어야 한다.                만약 디코더의 bu打er크기가 이보다 작으면

           그 bitstream은 복호할 수 없게 된다．
constraine&parameters_flag: 1 bit


    - 아무 뜻도 없다．


load_intra_quantiser_matrix: 1 bit
    - if ("1") ==>quantiserm北奴를 다운로드함을 의미．

    = 주로 中2:0 format어］ 대해서는 여기서 다운로드

      倖2:2인 경우나 4:4:4인 경우는 색신호어］ 대한 mati奴를 따로 다운로드

      해야 하므로 quan山蚣mati奴extension에서 해주면 편하다）.

    - zig-zag scanni!병순서로 다운로드

    - if ("0") ==> quantiz町m的奴를 그대로 유지, 그러나 만약                   sequence header

      에서 "0" 이면 그림 午26의           default mati奴를 이용．



                   8    16   19   22   26   27   29   34

                   16   16   22   24   27   29   34   37

                   19   22   26   27   29   34   34   38

                   22   22   26   27   29   34   37   40

                   22   26   27   29   32   35   40   48

                   26   27   29   32   35   40   48   58

                   26   27   29   34   38   46   56   69

                   27   29   35   38   46   56   69   83



             그림 4-26 Defauft quanfizer matrix for intra coding



intra_quantizer_matrix[64] : 8* 64 bits
    -z培呪ag scani血埋된 값들을 8 bit로 차례로 전송．
                                                                                           MPEG
                                                                                           VIDE0   87




      load小on_intra寸quan血아Hmatr次 : 1 bit
            - load_rn曲긔uantizer_ma出x와 내용이 동일．

            - default mati奴는 그림 4-27과 같다．


                                16     16     16    16    16      16   16   16

                                16     16     16    16    16      16   16   16

                                16     16     16    16    16      16   16   16

                                16     16     16    16    16      16   16   16

                                16     16     16    16    16      16   16   16

                                16     16     16    16    16      16   16   16

                                16     16     16    16    16      16   16   16

                                16     16     16    16    16      16   16   16


                         그림 4-27 Def汕什quan恤이 ma州x幻m t이c的ng




4.3.2. User Data
        user data() {                                                            No. of bits   Mnemonic
           userdata_startcode                                                    32            bslbf
            while( nextbitsO !=10000 0000 0000 0000 0000 0001')
                  user data                                                      8恥nL
            }
            next_start_codeO
        }


      user data start code : 32 bits

            - 000001B2 (H)

      user data : 8* n bits
            - dcc에er와 encoder 사이에서 user da呵n byte）를 전송．

            - 모든 start code들은 (X)0叩1(1刃로 시작되므로 이 C（넜e가 나오기 전까지는
             MPEG
             피DEO




                            모두 user data로 간주한다．

                          -23개 이상의 zero b出는 금지．




          4.3.3. Sequence Extension
                 sequence_ex把ns幻n {                                          No.（寸bits   入4'好nonw
                    exten駐on start code                                      32          bslbf
                    exte,心이s start code id巴stifler                           4           uimsbf
                    proflle_andJevel_indicafion                              8           uimsbf
                    Pr,必的ye旴弘en（光                                            l           uimsbf
                    chroma fonnat                                            2           uimsbf
                    horizoi北al 葫：配 ext印帥on                                   2           uimsbf
                    vertical si配 extension                                   2           uixnsbf
              >     bit rate extension                                       12          uimsbf


 츠：X:
              '꺼    maker bit                                                l           bslbf
                    vbv buffer si配 extension                                 8           uimsbf
                    low del叫                                                 l           uimsbf
                    frame_rateextension_n                                    2           uimsbf
능늣川      寸 d욜
      却 t。          色ame rate exten幽［川l d                                    5           uimsbf
                    next_start_codeO
                      }



                   extension start code : 32 bits
                          - 000001B5 (H)

                                                                                 )
                   extension start code identifier: 4 bits

                          - II 0001"

                          - 참고적으로 다른 ex奴ision들의 identifier는 표 午27과 갑斗．



                   profile_and_level_indication : 8 bits

                          - 다음의 표 午28, 4-29, 午30, 4-31고干 같다．

                          - if (escape bit = "0") ==> 표 午28, 표 4-29, 표 午30

                          -if (escapebit= "l") ==> 표 4-31

                          - profile과 level에 대해서는 6장에서 자세히 설명한다．
                                                                                 MPEG
                                                                                 피DE0        89




         표 4-27 exten羽n針art_codejden키伯codes (MPE（引S : T야扼 o-2)
extension start code identifier                  Name
00(刃                                             reserved
0001                                             Sequence Extension ID
(）아0                                             Sequence Display Extension ID
0011                                             Quant Matrix Extension ID
0100                                             Copyright Extension ID
0101                                             Sequence Scalable Extension ID
0110                                             reserved
0111                                             Picture Display Extension ID
1000                                             Pict山'e Coding I次tens幻nIP
1001                                             Picture Spatial Scalable Ex妃nsion ID
1010                                             Picture Temp月al Scalable Extension ID
 1011                                            reserved
 1100                                            reserved

1111                                             re心＼ed



              표 4-28卜朮心nning of bit引n pro뛔e and그eveL indication
                           (MPEG IS : Table 8-1)
Bits            Filed Size (bits)   Meaning
 [7:7]           l                  Es曲伊bit
 [6:4]           3                  Profile identification
 [3:0]           4                  Level identification




                     표 4-29 다애e indic아ion (MPEG IS : Table 8-2)
 Pr띠川e identi血ation                                  Profile
 IlOtoll]                                                                           (reserved)
 101                                                 Simple
 100                                                 Main
 011                                                 SNR Scalable
 010                                                 Spatially Scalable
 001                                                 1小gh
 000                                                                                (reserved)
                    표 4-30 Level indica作＞n (MPE（引S : Table 8-3)
 I七vet idnl枷叫伯川1                              I七vet




        표． 4-31 Esc야冷 口n：川eandleveUndication (MPEG IS : Table 8-4)
  profile.andJevelJndication                  Name
  10000000to 11111111                                             (reserved)




progressive_sequence: 1 bit
    - if (" lii) ==> 한 sequence 내에 pro얍ess如e frame만 있을 I대．

    可 （1011) ==> 그 sequence 내에            interlaced picu此를 하나라도 포함한다（즉

       field picture와 fran妃picture(progressive or not)가 섞여있는 경우도 포함）.



chroma 化rn怡t : 2b心
                                                             1
    - 표 4-32와 같이 chrominance format을 결정한다．


            표 4-32 Meanning 아chrom工form아 (MPE（引S : T야긔e o-5)
                           chroma f丑mat     Meaning
                                 00         leS心-V的
                                 01         4:2:0
                                 10         4:2:2
                                 11         4:4:4




horizontal size extension : 2 bits

   －如rizontal_s切e의 入4SB 2 bits
vertical 이ze exten引on : 2b心
   - vertical_s加의 八4SB2bits



marker bit: 1 bit




vbv buffer size extension : 8 bits
   －此v buf佃size의 MSB 8 bits



low_delay: 1 bit
   - if ("1") ==>B fra끄配이 없다. 따라서 재배열（re에ering）하는 지연이 없으며

     buffer가 und出low상태로 들어갈 수 있다.（앞의 4.2.2절에서 설명）

   - ii ("0") ==> B frame이 있다．

   - 미리 sequence structn肥가 정해져 있다면 디코딩중에는 이 flag은 필요

      없기 때문어］ 무시할 수 있다（단지 low delay mode에서 검증용으로 쓰인

     다） .




   - 이 low delay mode에서는 B-picture가 없으므로 picture data를 디코딩한 후
     곧바로 디스플레이하게 된다．



frame rate extension n : 2 bits
   -4.3.1절의 丘ame_rate 계산어］ 이용된다．



frame rate extension d : 5 bits
   -4.3.1절의 frame_rate 계산어］ 이용된다．
      .
          MPEG
92        VIDEO




     4.3.4. Sequence Display Extension
              sequence_display_extension() I                                No. of bits   入nemonic
                         extension start code identifier                    4             uim.sbf
                         %ideo format                                       3             uimsbf
                         colour_d哨cription                                  l             uimsbf
                         if (colour_descnption){
                                     colour_primaries                       8             uim的f
                                     transf針 characteri出心                   8             uim.sbf
                                    matrix coefficients                     8             umisbf
                         }
                         display_horizontal_size                            14            uimsbf
                         marker bit                                         1             bslbf
                         display_vertical_size                              14            uimsbf
                         next_start_code()
              }



              extension start code identifier : 4 bits
                   - n 0（月1 ''



              미deo 化rmat : 3 bits

                   - 표 牛33과 같이 video format을 나타내주는더］ 미리 化rmat이 약속되어 있

                       으면 관계없지만 그렇지 않은 경우 이 sequence di叩lay extension이 없으

                      면 표 중에서 unspe出led vid的向rmat으로 한다．


                              표 4-33 Meannig of기deof아m아 (MPEG IS : Table 6句
                                             vid刃 format    Meaning
                                                   000      co'끼ponent
                                                   001      PAL
                                                   010      NTSC
                                                   011      SECAM
                                                   100      MAC
                                                   101      Unst比cifiedvid凹 format
                                                   110      reserved
                                                   Ill      m氾rved
                                                                           93
                                                                      U




color_巾＄cription : lb吐
                      C可（7r_ prinu玎ies
     - if ( 1") ==>   transfer_ c方aricteristics     가 존재한다．
                      刃iatri工1Co功icients

     - if (11011) ==> 존재하지 않는다．



C아or下Fin伯ries : 8 bits

     - 표 4-34와 같이 색신호의 색도겨］ 위치를 나타낸다. .

     - 만약 sequen氾1di叩lay_e亂ension이               존재하지           않거나, 위에서 color

         description이 "0" 이면 각 응용에서 정한 값으로 한다．




                  표 4-34 C이ou나川manes (MPEG IS : Table o-7)
 Value                       P1血nai心
 0                           (forbidden)
 l                           Recommendation 玎U-R BT.709
                             pnmaly x y
                             green 0.300 0.600
                             blue 0.150 0.060
                             red 0.640 0.330
                             whith D65 0.3127 0.32卯
 2                           Unsp比坵edVk奴）
                             Image ch게a｛丸口istics are unknown.

 3                           res口ved
 4                           Recommendation ITU-R BT 470-2 SystemM
                             pnmaly x y
                             green 0.21 0.71
                             blue 0.14 0.08
                             red 0.67 033
                             white C 0.310 0.316
 5                           Rec아no妃nda如n ITU-1之 BT.470-2 Sys蜘iB.G
                             pnmaiy x y
                             留eenO.290．   的
                             blue 0.15 0.06
                             red 0.64 0.33
                             white D65 0.313 0.329
 6                           針vIE玎E 170M
                             primaly x y
                             留een 0.310 0.595
                             blue 0.155 0.070
                             red 0.630 0.340
                              white D65 0.31270.3290
 7                       S卜vLPTE 240入1(1987)
                         prlnlaiy x y
                         留een 0.310 0.595
                         blue 0.155 0.070
                         red 0.6300.340
                         white D65 0.3127 03291
 8-255                   reserved




transfer char七ter治tics : 8b吐5
     - 표 牛35와 같이 신호의 광전기적 특성을 나타낸다．

         만약 sequent氾H小叩lay_ex把nsion이 존재하지 않거나, 위에서                       color

         desc如tion이 " 0'' 이면 각 응용에서 정한 값으로 한다．


             표． 4-351乙哨厄rCha띠Ct이帥Cs (MPEG키S : I야)Ie o-8)
 \／帥ue                    Trans也rCh壯玭tensile
 0                        伽rbidden)
 l                        Recommendation IT나R BT.709
                          V= i.099L0·45띠.099
                                   的r12L 之0.아8
                          V= 4.500L
                                   如r0.018>1（之0
 2                        Unspecified Video
                                     Image Charact口istics are unknown.
 3                        reserved
 4                        Recommendation I口U-R BT.470-2 System M
                                     Assumd display gamma 22
 5                        Recommendation ITU-R BT.470-2 System B.G
                                     Assumed display gamma 2.8
 6                        SMPTE 170M
                          V = 1.099 L0.45-0.099
                                     如rl k20.018
                          V= 4500L
                                     for 0.018 2 L20
 7                        SMPTE 240M (1987)
                          V= 1.l1l5L0·45-0.1115
                                      forL.c之0.0228
                          V= 4.0Lc
                                      for 0.0228 > L
 8                        Linear transfer Charact口istics
                          i.e. V= 1(
 9-255                    reserved
                                                                            MPEG
                                                                            피DE0    95




matrix coefficients : 8 bits

     - 표 午36과 같이,且丘丑신호와 乂'I珉PR신호사이의 관계를 나타낸다．

         만약 sequenc乞display卞cx把nsion이             존재하지           않거나, 위에서          colorU

         description이   " 0" 이면 각 응용에서 정한 값으로 한다．


                  표 4-36M아淑 coefficients (MPEG IS : I야兆 6-9)
 V키ue                        Mafrix
 0                           (forbidden)
 l                           Rec이ml妃ndation ITO-I之 BT7(刃
                             E'y=07154E'G+00721E'B+02125E'R
                             E'田＝-0386E뇨＋0500E'5-0115E뇨
                             E'1lr=4454E'G-0046EB+0500E뇨
 2                           Unsr比C小ed 꺼den
                                       Image characteristics are unknown.
 3                           res心ved
 4                           FCC
                             E'y=0.59E'G-4-01lE뇨+030E'g
                             E'田＝-033E뇨＋0500E'B-0169E뇨
                             E'm=-0421E노4079E뇨+0500E'R
 5                           Recomn玘nda如nm卜R BT 470-2 Sys帥江iG
                             E'y=0587E'G+0114E'B+0299E뇨
                             E' =-0.331E'G+0500E'BM169E뇨
                             Em=M419E'0-0081E＼汁05（刃E뇨
 6                           SMPTE 170M
                             E'y=0587끄u+0114E'B+0299E'R
                             E' =4331E'G+0500E노M169E뇨
                             파衣＝:-t)419E'口0081EB+0500E뇨
 7                           SMPTE 240M (1987)
                             E'y=0.701E'a+0087E'B+0212E'R
                             E娩=-0384E'0+0500E'5-01l6E뇨
                             E'm=-0445E'c-0055E뇨+0500E'R
 8-255                       res口ved




display_horizontaLsize: 14 bits
     1 실제로 디스플레이하고자 하는 부분의 加rizontal size.

     - if (display_size <encoded ft跏e size) ==＞그림 4-28과 같이 enc에ed frame 중

         의 일부만 디스플레이한다．

     -if（반曲＝=> 그림 +29와 같이 dec（쿄edfra끄配이 화면의 일부밖에는 되지

         못한다．
96




          decoded
          fi
                                                                                                           화면


                                                                                          肖   ，“‘넌，
                                                                                                  ."
                                   그림 4-28                                 그림 4-29



            marker bit: 1 bit




            display_verticaLsize: 14 bits
                    - 디스플레이하고자 하는 부분의 수직쪽 크기．

                    －曲p1町h아izontal血配와 뜻이 같다．




     4.3.5. Sequence Scalable E)cfension
         sequence_scalable_extensiono {                                          No. of bits           Mnemonic
                    extension start code identifier                              4                     uimsbf
                    s沮lable mode                                                 스
                                                                                                       uim.sbf
                    layer id                                                     4                     uim.sbf
                    if (scalable_mode ==' spatial scalability ') {
                                 lower_layer_prediclion_horizontalk_size             14                uim.sbf
                                 m別由er bit                                           l                 bslbf
                                 10吼r_layer_prediction_verlix川H毗a                    14                uimsbf
                               horzontal_subsampling_factor_m                        5                 uimsbf
                               horizontal_subsampling_factor_n                       5                 uimsbf
                               vex七cal subsam ［沚ngjac奴m                              S                 uimsbf
                               vertical_subsamplin흩_factor_n                         S                 uimsbf
                     }
                     if (scalable_mode ==temporal scalabiity") {
                                  picture中mux_enable                                 l                 uimsbf
                                  if (picture_mux_enable)
                                               mu乂to下rogres啣e_sequence               l                 uim.sbf
                                  picture_mux_order                                  1                 uimsbf
                                  picture_mux_factor                                 국                 uimsbf
                                                                      97



         }
        next_start_codeO
)



    이 sequence sc沁able ex妃nsion은 한번 나오면 그 뒤의 repe毗d sequence에서도

항상 나와야 한다.                 즉 하나의 bit毗earn이 scalable하다가 안 하다가 할 수는 없

다. 또한 하나의 羽叫ence 내에서도 scalable하다가 안 하다가 할 수는 없다． 또

만약 bitstream어］ sequence scalable extension이 존재하지 않는다면 그 bitstream은

scalab血口를 사용하지 않은 것으로 간주한다.                   Data -如恤埋을 제외하고 base

layer에서는 sequence scalable extension을 보내지 않는다（5장에서 다시 설명한다）.



    extension start code identifier: 4 bits
       口 "0101"



    scalable mode : 2 bits

       - 표 午37과 같이 scalab小口의 翊四을 표시하1 주며 이에 따른 macr아）lock

             1type의 표들도 달라진다（이 표들은 4.3.16절의 Macroblock mode에서 설

             명됨）.

       - Sequence scalable exten없on이 존재하더라도 spatial scalability의 경우에서는

             아래 표 午37어］서 나타낸 대로 picture_spatial쪼alab뇨아帥如nO가 존재

             하지     않는      picture어］ 대해서만은   non卞scalable   mode로   디코딩한

             다．(scalab皿y어］ 대해서는 5장에서 설명함）.
     MPEG
98   VIDE0




                        표． 4-37 De作내on 아 Sc이able_n似把 (MPEG IS Table o-10)
             scalable mode   Meaning                  pictum_叩姐吐乳出고如e肌的0   macroblock_ty比
                                                      n0                   tables
             sequence_scalabie ex帥S幻n0 n야present                           午52, 4-53, and 4-54
             00                d毗a paititioning                            午52, 午53, and 4-54
             01                spatial sc出ab小ty       P1eSent              午55, 午56, and 4-57
                                                      not present          4-52, 牛53, and 4-54
             10              SNR sc띠小ility                                 4-58
             11              把mpr표al scalability                           牛5가1-53, and 4-54




         layer id : 4 bits
                  -b餐e layer인 경우 0이며 layer가 높은 순으로 순서다로 1, 2, 3,...순이다．



         lower_layer_prediction_horizontal_size: 14 bits
                  - lower layer쇼ame의 horizontal_size.

                  . 그림 午30 참조（자세한 것은 5장에서 설명）.



         IowerJayer_prediction_verticaLsize: 14 bits
                  - lower layer frame의      vertical_size

                  - 그림 牛30 참조（자세한 것은 5장에서 설명）.



         horizontal_subsampling_factor_m : 5 bits
                  - lower layer와 enhanc이nent layer의 sampling 비율．
                  - 그림 4-30 참조（자세한 것은 5장에서 설명）.



         horizontaL subsam川ng_fact이m : 5b心
                  - lower layer와 et血a毗ment layer의 sampling 비율．
                  - 그림 4-30 참조（자세한 것은 5장에서 설명）.
verticaLsubsampling_factor_ m : 5 bits
          - lower layer와 enhan氾n妃nt layer의 sampling 비율．
          - 그림 牛30 참조（자세한 것은 5장에서 설명）.



verticaLsubsamplingjactor_n : 5 bits
         - lower layer와 enhancement layer의 samlpling 비율．
         - 그림 牛30 참조（자세한 것은 5장에서 설명）.


                                   幻叩라J口yer下rethctic功vertwalm引ze半 叱rae吐缸samj丑ingjact아1月 /
                                                                        ye此IC出그弘小sampli月gJ뇨t까少
                                        勿恥乙la e乙horiz口月tal1功set




  i口）ver_layer小ye斤IC口｛40／丙et
 ＝
 1



    m
    心m 芦H七뿟
                                                                                                  A

                                                               Up드ampi心d I.o1Vd
                                                                  少小
  으乞侮쁜뎌＼ m奇비뇨土요
                       I.心1斗er La＼七t
                          Frame
                                    H
                                                                 LavCi Frame
                                                                                                  V

 幻거ierlayerprethction加rizontal下任e
                                                      lower layerpredz CCI on_horizontal_sIze *
                                                            方orizo月tal訊如口月刎ingJ뇨切乙月 /
                                                             加rizo月talsu加ampli月g乖C切乙月i
그림 4-30 Formation (＞什he spa恢抑xe뎨C化n by inte巾olalion O什he lower layer
                     帥寸내e (MPEGIS : 日gure 7-14)



picture_mux_enab旭: 1 bit

       - ii ('1') ==>        Temporal sc띠abili口에서 복호된 picture가 디스플레이되기 전

                  어］ remultiple幻ng될 필요가 있으면 아래의 picture_mux_order와 picture_

              mux_factor를 이용한다（Te呻曲I scalab小勺에서는 base layer의 decoded

              picture와 enhancen妃nt layer의 decoded pi啣re를 서로 사이사이에 끼워서

              완전한 pictt配rate를 얻는더］ 이를 remultiple恤ig이라 한다）.

      - if ("0") ==> 필요성이 없는 경우
100




      n仙乂如下ro뎬笛帥尼_sequence : 1 bit

         - if ("1") ==> pro母essive di叩l町를 할 필요가 있을 때 두 개의 layer에 해당

           하는 decoded picture를 섞어서， 잠정적인 pn）留邙前ye pi力ire를 얻는다．

         - if("O") ==> 섞은 후 interlaced sequ帥（:e를 얻고자 할 때（progressive

           Hse（弘ence가 " 1" 인데 mu兀的pro얍ess加乞鋸叩ence가 "0" 이 될 수는 없

           다)    .




                      鈿
      p七ture_rnux-－이1er : 3b卜冷

         - Ten叩아alscal的血y어］서 remultiplexii垠할 때，enhanc이I妃nt layer어］서 얻어진

           decoded picture를 base layer의 첫 번째 picture 앞에 몇 장 끼워넣느냐 하

           는 개수를 나타낸다. 즉 enhancen妃nt layer picture들과 base layer picture들

           의 O什set을 나타낸다고 할 수 있다（그림 4-31 참조）.

                      전처＼州上＼
      picture_rnux_tactor: 3 bits

          - Temp丑Bi scalab血ty어］서 remultiple汕嘔할 때，base layer에서 얻어진 picture

            들 사이어］ enhancement layer의 deco妃d picture를 몇 장씩 끼워넣느냐 하

            는 숫자를 가리킨다．

          - Decoder에서 remultiplexing된 후의 picture열을 나타내면 그림 午끄과 같

            다．
                                                                                          1MPEG
                                                                                           VIDE0     101



                       /      picture_muxmorde느1
                                                              r       pict旺e_mux_factor=2
                   /           ,    .       1   1         I       I
                   1           I    U                     I       U
                   I           U    I                     U       U
                   1           U    U                     I       1
                   1           U    I                     I       1
                   1           U    I       1   I         I       I
                   1           U    U       1   U         1       1



                                        base layer pictures
                                        enhance ment layer pictures

                           그림 4-3] 디cture_mux_아der오I- picture_mux如ctor




4.3.6.（計ou口 (>f 미ct내eHe（그der
     莎에m吐少巾瑯上凹曲0 {                                                          No. of bits     Mnemomc
                group_start_code                                            32              bslbf
                血tie code                                                   25              bslbf
                di哨ed 叩                                                     l               uimsbf
                brt六en link                                                 l               uimsbf
                next_start_code()
     }



     아oup多怡凡code : 32 b心

         -000001B8 (H)



     time code : 25 bits

         . 특히 digital VCR 등에서 reference로서 중요하다. 표 4-38과 같이                                           구성

           된다．

         m 이 time code는 표 午38과 같이 시각을 나타내며 이 시각은 GOP header

          바로 다음에 나오는 picture(tempoi赴reference 가 0임）의 시각을 나타낸

           다．
         - 표 午38의 time code拉cture는 1초 내의 picture의 숫자이며 이 값은 다
102




              음과 같이 dr아)_frame_flag어］ 따라 달라진다．

           -if (dr아) 加In乞flag="0") ==> (picture per second）값을 가까운 정수값으로 고

              쳐서 picture갯수를 계산한다（예를 들어 pic加re per second값이 29.971七인

              경우는 3아也로 고쳐서 1초어］ 30장의 picture가 발생하는 컷처럼 꼐산하

             면 된다）.

           - if (drop什ame_flag = "1") ==> 이 flag가 1로 sethi略되는 경우는 29.97Hz일

              U귀 만인데 이 때는 1초에 30장씩 나온다고 가정한 후 Ii'［妃 code

             n血lutes가 0, 10, 20, 30, 40, 50인 경우를 제외하고 매분마다의 처음 두

             picture (time_c0de_pit珀ure=0,1)는 갯수에 넣지 않는다（즉 그때는 timee

              c에e_ picture가 2 부터 시작한다）.


                           표． 4-38卄me code (MPE（引S: I야)Ie-1])
       lime_code                 II range of value     No. oft由四   Mnemonic
       dmp_frame_flag                                  l
       time code h에rs              0-23                5           uimsbf
       血ne code minutes            0-59                6           uimsbf
       marker bit                  l                   l           "l   "

       time code seconds           0-59                6           uimsbf
       tin也code 加恤es               0-59                6           uimsbf




      closed_gop: 1 bit
           - GOP는 그림 4-32와 같이 구성되는더］ 이때1 孝1고｝ 韋2 frame은 전 GOP의

             煎）가 없으면 복원할 수 없다.                       편집은 GOP단위로 하므로 편집과정어］

              서 앞의 GOP가 없어지면 和允如rte이 없으므로 #1,孝2丘a끄ie을 복원할 수

              없다.      그런더］ 예를 들어 孝1, 韋2丘ame을 backward motion vect아만을 사용

             한다면 앞의 GOP가 없어도 현 (3OP를 완벽하게 복원할 수 있게 된다．

             이와 같이 closed4叩가               " 1" 이라는 것은 이 孝1，韋2 B picture가 단지

             backward m呱on vect야만을 이용하거나 또는 in仕a coding을 이용하씨 코

             딩되었다는 것을 가리킨다．
                                                                                                       103



                                                         GOP
                                                1                       1
                                     BBP BBIBBP. ..BBP
                                      叛） i幸1抱

                                                     그림 4-32


      broken link: 1 bit

            - Closed_gop가 "0" 인 경우는 위에서 설명한 바와 같이 앞의 GOP와 관

               계되는더］ 이때 앞의 （刃P가 없어지면 孝1，宰2 frame을 만들 수 없게 된

               다.      따라서 코딩이나 편집작업 시 이와 같은 경우가 발생하면 그

               GOP의 header어］ broken_li耿를 " 1" 로 해주거］ 된다．

            - Broken_血k가 "1" 이면 decoder에서는 backward motion vect아만을 이용하

             中거‘난1또는 孝1，宰2丘ame을 sk如하고 디스플레이하지 않을 수 도있다（재량

               권은 디코더에 있음）.




4.3.7. 디cture He（그der
       picture_headero (                                                       No. of bits   入4nemonic
                  picture_st町t_code                                            32            bslbf
                  岫TI恥l丑_ 싸bren(氾                                              10            uin咨bf
                  picWi七cod加g帥1e                                               3             uixnsbf
                  vbv_delay                                                    16            uimsbf
                  if ( picture_coding_type == 211 picture_coding_ty比 == 3) {
                                f네．下el＋匈rward批由r                               l
                                forward f code                                 3             uimsbf
                  }
                  if ( pictul乞cO五11且먀比 ==3 ) {
                                fi皿下el누backward_vec切r                          l
                               backward_f_code                                 3             urn肖bf
                  }
                  while (nextbits0=='l' ){
                             extrambit_
                                     I沁ure       ／水＼with the v심ue "1" 水／       l             uirnsbf
                             e虹ra_infonnalion_pictw七                           8
                  }
                  extra_bit_I沁ure        ／木＼with the v出［ue "O" 半／              l             uirnsbf
                  next_start_code0
      I
      1
          MPEG
104       VIDEO




              p妃ture_sta凡code : 32 b心
                  -00000100 (H)



              temporaLreference: 10 bits
                  - 각 d匙dpi山re의 순서를 나타내는 unsigned integer.

                  - 이 temporal reference가 같다는 것은 기본적으로 시간축상에서 같은 시

                    간＜네 있다는 것을 뜻한다．

                  - 寸（low_delay = '0" ) ==> 이때는 B picture가 있는 경우로 小splay order에

                    맞추어 口겨1 丘nme마다 1씩 증가한다（단 10 b抽이므로 modulo 1024연샨）.

                    그러나 field picture구조로서 한 fran叱이 두 개의 field로 코딩되는 경

                    우 그 두 pi伽re의 picture header어］ 있는 tem兀ral reference는 같다（이는

                    한 fran配을 field별로 코딩했다 하더라도 두 field어］ 같은 temporal

                    reference를 줌으로 디스플레이를 합쳐서 伽me단위로 한다는 뜻이 내포

                    되어 있다）. 또 GOP 1蜘der 바로 뒤 pi啣re의 temporal re佃mice는 0으로

                  ．초기화 된다．

                    if (low_delay = "1") ==> Low_delay가 1인 경우에서는 4.2.2절의 설명과

                     같이 big picture가 발생할 수 있는더］ 이와 같이 big picture 바로 다음에

                    므오늪洹cture의 temporal reference는 N+1(modulo 1024）이 된다． 여기서

                     N은 coded picture data를 VBV bu卄er로 부터 제거하기 전에 VBV buffer

                     를 몇 번 검사했나 하는 횟수이다（4.2.2절의                 설명에서 ,N은 결국

                     skipped pictu珥의 개수가 된다）. Big pict配가 GOP 바로 전에 발생하면

                     GOP 바로 다음 pic加re의 ten격？oral reference는 N이 된다． Big picture가

                     아닌 picture 뒤를 따르는 picture의 temporal_reference는 low_delay="0" 인

                     경우와 같다（즉 temporal reference는 1씩 증가하고 한 frame을 이루는

                     두 丘eld의 temporal_refernce는 갇다.    또한 GOP 바로 다음 加ture의

                     temporal_ reference값은 0이 된다）.
                                                       105




   - 한 frame이 두 개의 field pic加re로 구성되고 그 첫 번째 field가 big

    picture인 경우 이   두 field의 把mporal妃ference는 같지 않다．



p油ure_coding_type : 3b心
   - 표 4-39와 같이 pi伽re의 코딩타입을 나타낸다．
ic石




                          표 4-39 picture_coding小t叩e ( MPEG IS : T야)Ie6-12 )
       甘ctu八＝conf吐帥比                                 （刃fifigme吐md
       000                                           如巾姓妃n
       001                                           intra-coded (I)
       010                                           pi乂1icfive-col已d (P)
       011                                           bi血eclionally們毗ctive깹毗曲ve-刃de姙D
       100                                            n야used
       101                                            reserved
       110                                            res口ved
       111                                            reserved




      V自牙띠e怡弘：16 bits
         - 처음 빈 상태에서 VBV bu卄er를 일정수준으로 메우는 더］ 이용한다．

         - 4.2.1절에서 설명한 바와 같이 vbv尸delay는 다음과 같이 계산된다．

                           vbv_d이ay=90,000 B*r/R(B*n고｝ R은 4.2.1절 참조）



      ft川HpeL幻rw카d_vect아 : 1 bit
         -       Ito, ,



         小4PEG1에서 쓰인다．



      forwardj_code : 3 bits
             - 모두 II l tI

         －八叩EG1에서 쓰인다．



      ft川小peLbackward_比Ct아 : 1 bit
             -    11011



             小作EG1에서 쓰인다．



      backwardf code : 3 bits
             - 모두 " ill

             小4PEG1에서 쓰인다．
                                                                                          107




      extra_bit_picture: 1 bit

          －寸（" it) ==> 뒤어］ ex甘a mi이mation_picture가 따르는 것을 의미．

           - if (1100) ==> 뒤에 extra mi이mat on_pictL玎e가 없다는 것을 의미．

               (4 '1', extra_infor 的on_picture(8bits), "1", extra information_.picture(8 bits),

                     , " 0"     끝）.

           - MPEG2에서는 미래의 사용을 위하여 남겨졌으므로 항상 extra bit

               _picture를 0으로 하면 된다．



      extra_information_picture: 8 bits
               ' 미래의 사용을 위해서 남겨짐．




43.8. Picture Coding Extension
      picture_coding_extensiono {                            No. of bits    Miiemonic
            extension start code                             크2             bslbf
           extens加nstart (：에eident出er                        4              uimsbf
           心ode[OJ[O] 片 forw町d ho巾ontal 차                    4              uimsbf
           f_code[O][1J／水 forw出xl vertical 半／                4              uimsbf
           fc에eFlilfil／시坮吐wt끄汪I hon끄)ntal 永／                 4              uimsbf
           fc어le[1][1] 幷 b岫ward vertical 呵                  4               uimsbf
           intra_dc_precision                               2               uimsbf
           picture_structure                                2               uin的f
           top_加Id fit吼                                      l              uimsbf
           frame下red加me_dct                                  l              uimsbf
           concehuent motion vectors                         l              uimsbf
           (L乳毗t叩e                                           l             uimsbf
           intra sic format                                 l              uimsbf
           alternate scan                                    l             uimsbf
           repeat_first_field                               l              uimsbf
           chroma_420_type                                  l              uimsbf
           progressive_frame                                l              uirn.sbf
          con甲妓t已d柳奴y뗘ag                                    l              uimsbf
          if (composite_display_flag) {
                v axis
                     1


                                                            1              uim.sbf
                field_sequence                              ;              uimsbf
                sub carrier                                 l              네m咨bf
                but吼긔n바tude                                 7              uini.sbf
                sub_carrier_phase                           8              wmsbf
           }
          next_start_code()
108




        }



       extension start code : 32 bits
            -000001B5 (H)



       extension start code identifier :4 bits




       f_code (s][t] : 각 4 bits씩
            . 표 中40콰 같이 motion vect아의 用；쌕영역을 나타낸다．
             -1- 9까지의 범위, 안 쓰면 " 1111", 0은 금지．

             -s가 0이면 的rward, 1이면 backw可d, t0이면 horizontal, 1이면 vertical.

             - if (concealment_motion_vect이s = h10H && I-picture) ==> "1111"

       - if (I or P picture) ==> f_code [1][t] = "1111" （왜나하면 I 나 P-I竝cture에서는

      backward moti이i vec恤는 쓰이지 않기 때문이다）.




               표 小40 시아시ble n狗化n vector range（그sa 仙ncflon 아 f_code(s) (t)
                               (MPEG IS : I야)Ie 7的
            ／끄S勿Es皿］    Verfical c且nponents (t=1) of field             Ali戎her 螂
                        vectors in frame pi才11re
                    0                                    (fothidden)
                    l                    [-4:+3.5]                           [-8:+7.5]
                    2                    [-8:+7.5]                        卜16:+15.5]
                    3                  [-16:+15.5]                         [-32:+31.51
                    4                  [-32:+31.5]                         [-64:+63.5]
                    5                 ［而4:+63.51                         [-128:+1275]
                    6                [-128:+127.51                       [-256:+255.51
                    7                [-256:+255.5]                       [-512:+511.51
                    8               卜512:+511.5]                       [-1024:+1023.5]
                    9              [-1024:+10235]                      [-2048:+2047.51
                10-15                                     (reseived)
                                                                1
                                                                    MPEG
                                                                    피DE0   109




intra_dc_precision : 2 bits
    - 표 午41고｝ 같이 intra block DC계수의 코딩 bit 수를 나타낸다．
                                             8八    i\ \oit,

              표4-41 Intra DC precision (MPEG IS : Table 6-13)
                  intra dc_precision       Precision (bits)
                         00                        8
                         01                        9
                         10                       I0
                         11                       11




picture_structure : 2 bits

     이 변수는 표 4-42와 같이 그 picture의 구조를 나타낸다．


        표 4-42 Meanning 아 口cture_計uc加re (MPEGIS 化비e6-14)
                     picture_structure    Meami理
                              00           reserved
                              01          孔pF妃Id
                              10         Bottom Field
                              11         Fmrne picture




    - Fra工ne으로 이루어진 field picture에서 한 fr如叱의 두 개의 m넌는 코딩타

      입이 같아야 하지만 first fie넌가 I-type이고 두 번째 field가 p－翊pe인 경

      우는 있을 수 있다. 한 frame에서 두 개의 field picture의 각 변수 중에

      서 다른 값을 가질 수 있는 것들은 다음과 같은 것들뿐이다．



          f_code［이［이， f_code[0] 기

          f_code[1][0], f_code[1][1]

          intra_dc_precision, concealment motion vectors, q_scale_type

          intra ＼기c 幻rmat, 졔也mate scan




    - First field가 top이면 그 다음 fie넌는 的如m이어야 하고 first field가
110




            1兀如m이면 그 다음 field는 幻p이어야 한다．



      top_field_first: 1 bit

          - 원칙적으로 field picture에서는 먼저 전송되어온 fie닢가 먼저 디스플레이

            된다. 즉 들어오는 순서대로 디스플레이한다. 그러나 field구조로 되어

            있는 frame picture에서는 fran配단위로 전송하기 때문에 어떤 field를 먼

            저 디스플레이할 것인지를 선택할 수 있다. 또한 丘ame구조로 되어 있

            는 丘ame picture에서는 쇼ame 자체를 단순히 반복시켜 주어야 하는 경

            우가 있다. 이와 같은 경우에서 picture_str끄cture, progressive中 S叫uence,

            repeat_first_field등에1 따라서 결과를 달리할 수 있는더］ 이들을 경우별로

            따져보면 다음과 같다.



        (a) field picture어］서

                이때는 top-如追血St는 "0" 이 되어야 하며, 출력은 그 시간어］

                디코딩된 field가 된다．



        (b) field 구조로 된 frame picture어］서

                if (t아Lfle通玉rst = "1") ==> top field가 먼저 디스플레이된다．

                if (top_field_first = "0") ==> bot幻m field가 먼저 디스플레이된다．



          다음부터는 뒤에 설명될 l롸玘趾뇨first如ld와 관계되는 것이다. 따라서

        repeat_first_field를 먼저 참조하고 보기를 바란다．



        (c) progressive_sequence = "1" 이고 repeat_first_field 가 "0" 인 경우
                이때는 t아느fle님f뇨st는 " 0" 이 되어야 하며 출력은 그 시간어］

                디코딩된 progress加efra끄叱이 된다．
                                                                 "
                                                                     111




  (d) progressive_sequence = lii" 이고 repeat_first_field가 " 1" 인 경우
          if (t아LfieldH如St = 1101!) ==> 출력은 두 개의 pro얍essive伽me이 된다．

                                （전송된 fran配의 단순한 반복이다．)

          if (top_field_first = 1111) ==> 출력은 서］ 개의 皿O曾essive f뇨曲配이 된다．

                                （전송된 伽me의 단순한 반복이다．)

     이 的n如通fi心t의 활용예는 뒤의 rei玘at fi搭t_field에서 설명한다．



frame_pred_frame_dct: 1 bit
   - 迂（lilt) ==> 그 picture에서는 frameH玭？r와 쇼an配 prediction만이 이용되었

      음을 뜻함（progress如乞sequence=" 1" 이면 이 flag이 "1" 임）.
   - if ("O") ==> 그렇지 않은 경우．



concealment motion vecto四: 1 bit
   - if ("l") ==＞七l仕a macr的1(乂k의 motion vec奴를 보낸다는 뜻（예를들면 채널

      이 나쁜 곳에서 inirablock의 데이터가 깨지면 임시방편으로 그 전

      fran妃에서 moti이lv凹toi를 이용하여 가져오게 하기 위한 일종의 에러대

      책 장치이다）.



cscaIe_type: 1 bit
      = 표 午43과 같이 양자화 스텝을 바꿔준다．
      MPEG
112   VIDE0




              표 4-43 R이allon between quantiseLsc（긔e and qu（그ntisersc이e_code
                                   (MPEG IS : Table 7句
                                               quanliser_s月lelq_scalejypel
              quanlisersca1e_code   q_scale_type = U                 q_scale_type = 1
                      0                                (forbidden)
                       l                   2                                l
                      2                    4                                2
                      3                    6                                긔
                      4                    8                                4
                      5                   10                                5
                      6                   12                                6
                      7                   14                                7
                       8                  16                                8
                      9                   18                               10
                      10                  20                               12
                      11                  22                               14
                      12                  24                               16
                      13                  26                               18
                      14                  28                               20
                      15                  30                               22
                      16                  32                               24
                      17                  34                               28
                      18                  36                               32
                      19                  38                               36
                      20                  40                               40
                      21                  42                               44
                      22                  44                               48
                      23                  46                               52
                      24                  48                               56
                      25                  50                               64
                      26                  52                               72
                      27                  54                               80
                      28                  56                               88
                      29                  58                               96
                      30                  60                               104
                      31                  62                               112
                                                                        113




intra 미C 化rn伯t : 1 bit

   - 표 中44와 같이 intrabi어永의 DC계수를 제외한 DCF꼐수들을 디코딩하

     는 더］ 쓰이는 표를 선택하는 데에 쓰인다．

      5장에서 자세히 설명．


     표． 小44S이ecu아）of DCI coefficient VLC table (MPE（引S : Table 7匈
                        inti크 Vi口font田t        0                l
                            intra blocks   table 5-6        table 5-7
                   (macroblo出_intra = 1)
                        nc旺l寸flU沮 bk겨出뀨    table 5-6        table 5-6
                   (ma口obl어：k_intra = 0)




a仕ernate scan: 1 bit
  -if CV)＝볍＞al妃'Ii毗scanning（그림 4-31)

  - jf (fl0U) ==> 74恥g scanning（그림 千32)


                                                        U

                   0   1    2     3    4   5       6    7
               0   0   1    5     6    14 15 27 28
               1   2   4    7     13 16 26 29 42
               2   3   8    12 17 25 30 41 43
               3   9   11 18 24 31 40 44 53
                                                   4
                                                   二    弘
               4   10 19 23 32 39 45               <
                                                   1V




                                                        印 旬 臼
                                                   <J
               5   20 22 33 38 46 51               <1
                                                    V

                                                   0/
               6   21 34 37 47 50 56               <
                                                   1V

                                                   八
                                                   乙
           v   7   35 36 48 49 57 58               6




         그림 4-31 Defin壯＞n of scan(0) (v)(u) ( MPEG IS:日gure 工2 )
114




                                                        U

                        0   1     2   3    4   5   6    7
                    0   0   4     6   20 22 36 38 52
                    1   1   5     7   21 23 37 39 53
                    2   2   8     19 24 34 4.0 50 54
                    3   3   9     18 25 35 41 51 55
                    4   10 17 26 30 42 46 56 60
                    5   11 16 27 31 43 47 57 61
                    6   12 15 28 32 44 48 58 62
                v   7   13 14 29 33 45 49 59 63

                 그림 4-32 Defir咐ion of scan(1)(v)(u) (MPE이S :日g내e7匈



      repeat_first_field: 1 bit
          - 이 변수는 241七의 영화를 301七의 interlace TV신호나 또는 601七의

            progressive 牙V신호로 만를 畔이용되는 것이다. 먼저 24Hz의 영화를

            3아七의 interlace TV신호로 바꿀 때는 그림牛33과 같은 針o2p띠idown방

            법이 쓰여진다.         이 방법은 그림에서도 볼 수 있듯이 film의 한 丘ame

            씩 건너서 3 fields - 2 fields - 3 fields 식으로 번갈아 가면서 뽑아내는 것

            이다. 이따1 자세히 살펴보면 3장의 field를 쓸 때는 첫 번째 field가 반

            복되는 것을 알 수 있다. 따라서 인코더에서는 241七의 ifim을 그대로

            코딩해서 보내고 디코더에서 打o 2 pulldown을 이용하꺼 디스플레이할

            수   있다면 bit발생량을               줄일   수   있다.      이U뀨   쓰는    것이   이

            repeat first侃ld이다.    따라서 이 변수를 이용하기 위해서는 전송하는

            丘an妃이 꼭 "pro軍essive"이어야 한다.                그러므로 field구조로 된 f始me

            picture나 또는 field picture어］서 rej光at_first_field의 값은 항상 0이 되어야

            한다. 각 경우를 살펴보면 다음과 같다．



        (a) progressive_sequence = "0" 이고 progressive寸f切me = "0" 인 경우
                repeat_first小eld 는 " 0" 이어야 한다．
                                                                            115




(b) progressive_sequence = "0" 이고 progressive玉ame= "1'' 인 경우

         if (repeat_first_field =1'0") ==> 출력은 鈿o fields

         if (repeat_first_field ='1") ==> 출력은 three fields

(c) progressive_sequence = "1'

         if (repeat_first_field ="0") ==> 출력은 복원된 one丘ame

         if (repeat_first_field ="1') ==> 출력은 two or山ree frames (top_field_first

                                      참조, 단순한 쇼ame의 반복）



     이러한 3的2P山idown방법은 결국 幻p玉eld_flrst와 repe丸缸芷玉eld를 이

    용하면 될 수 있다.              그림 4-33어］서 두 변수의 값을 생각하1 보면 다음

    과 같다．



(a) 1 加me에서

         여기서는 的p field가 먼저 디스플레이되고 첫 번째 尿4d를 반복시

         켜        야 한다. 따라서 top_field_first = "1", re玘at니first_field =" 1"

(b) 2frame에서

         여기서는 field를 반복시키지는 않지만 比如n field가 먼저 디스플레

         이돼야 한다. 따라서 的p-－丘eld_flrst = "0", repeat_flrst_丘eld ="0"

(c) 3 frame어］서

         Bo如m field가 먼저 디스플레이되고 첫번째 field를 반복시켜야 한

         다． 따라서 的p－五eld血St = "0" , repeat_first_field =1"

(d) 4 frame 에서

         Field를 반복시키지는 않지만 top field가 먼저 디스플레이되어야

         한다. 따라서 top_field_first= 1" , rej玘at first玉eld ="0"




      이들 변수를 이용하면 24Hz의                      영화필름을 디코더에서 601也의
      MPEG
116   VIDEO




                  progressive TV신호로도 만들어 줄 수 있는더］ 이것이 바로 progressive

                  小sequence가 " 1" 인 경우이다.             이경우 위의 1,2,3,4 丘ame에서의 t아）m

                  fiel&.first오｝ iepeatjirsL如id값은 다음과 같이 된다．



              (a) lfra끄［ie에서

                       여기서는 똑 같은 fran配을 3장 연속해서 디스플레이시켜야 한다．

                       따라서 的c느field．皿St = "1", repeat_first_field =" 1"

              (b) 2 fi＝如［le어］서

                       여기서는 똑 같은 frame을 2장 연속하써 디스플레이시켜야 한다．

                       따라서 top_field_first = "0", repeat_first_field =11
                                                                                                                                        117




                                                                戶人
                                                                     INTERLACED                         PROGRESSIVE SCAN
                                     디LM FRAMES                          니DEO                                 피DEO
                                    24 FRAMES/SEC                    60 디ELD듸SEC                          24 FRAMES/SEC




     0 000 00 000 00 000 00 000 0
                                                 0                                                  2
1
                                           中
                                           m                             1

                                           H
                                           m                             m                          뇨
                                           H
                                           1                             m

                                           小
                                           4                             H




                                                          如的m
                                                                                                    U
                                                           m
                                                           e             m




2
                                                           m
                                                           H             小

                                                           m
                                                           U
                                                           e             中

                                                           小
                                                           H             小
                                                                                  =m       m       h1   1寸   卜

                                                                                  ///
                                                    C                m
                                                                     H   =

                                                                     中
                                                                     m   尸

                                                                     H
                                                                     e
                                                                     m   H



3                                                                    1   尸




                                                                                                                                韜轟拙鹽醬
                                                                                       1
                                                                                       m
                                                                                       中



                                                                                               娜
                                                                                               懈
                                                                                       小
                                                                                       e
                                                                                       m




                                                                                                                                驪
                                                                                       m
                                                                                       e
                                                                                       1
                                                                                       1



                                                    0
                                                                                                                      解
                                                                                                                      艸H
                                                                                       H
                                                                                       나
                                                                                       H




4                                                                                                                          渤礬



                                                                                                             ar
                                                                                                                  m
                                                                                                                  =
                                                                                                                  1


                                                                                                                  H
                                                                                                                  m
                                                                                                                  m
                                                                                                                  H

                                                                                                                  烈礪烈4無喜琉：
                                                                                                                  e
                                                                                                                  H
                                                                                                                  中
                                                                                                                  n      姓i
                                                                                                                  擘蟹旨；『；
                                                                                                                  H
                                                                                                                  1
                                                                                                                  e
                                                                                                                      翼羅難發；트


                                                        그림 4-333 to 2 pulldo＼八／
                                                                              n



(c) 3 쇼ame어］서

                                    마찬가지로 top_field_first = "1', rej玘at_first_field ='1'

(d) 4 frame어］서

                                    마찬가지로 top_field_first = "0", re1光at小first_field =01"



    앞의 4.2.1절에서 설명했듯이 vbv bu珏er의 동작에서 b咐er를 체크하는

    시간간격(t 1 山）은 이 repeat_缸st_field와 的p-加님1血St값에 따라서 달라

    질 수 있는더］ 이 이유는 3 to 2 puildown을 하면 디스플레이되는 간격이

    달라지기 때문이다． 따라서 buffer에서 coded picture를 가져오는 시간

    （즉 buffer를 체크하는 시간）도 그에 따라 보통의 2바1 또는 3바區 조정
118




         이 되어야 하는데 이 조정되는 시간은 pro얍essive小sequence, low_delay,

         的p_配닢_flrst, repeaLfi搭t_fleld값어］ 따라서 달라치게 된다.              이는 또 어

         떤 翊PC의 picture냐에 따라서 달라지는더］ 각 경우를 살펴보면 다음과

         같다.    여기서 I는 frame rate의 역수, 즉 frame 간의 간격이다. 따라서

         field 간의 간격은 1/2가 된다．



      (a) progressive_sequence =" 1" 이고 lo뾰_delay =D" 인 경우

         -t= n일 때의 伽ture의 repeat寸first_field = " 0" 인B－加艾ure의 경우

                                    tfl+l tHl= T

         -t= n일 때의 picture의 rei玘at_first_field = "1" 이고

             的p_fleld_缸St = " 0" 인 B-picture의 경우

                                    뇨i-tn = 2T

         -t= n일 때의 picture의 rej玘at_first_field = ' 1" 이고

             的p_field_first =" 1" 인 B-pi曲re의 경우

                                    뇨i-tn= 3T

         -t= n일 때의 picture가 P 또는 I-picture이고，

             그전에 있던 P나 I-picture의 rei玘at_first玉叱＝"0" 인 경우

                                    tn+1-tn= T

         -t= n일 때의 picture가 P또는 I-picture이고 그 전어］ 있던 P나 I-picture의

                     repeat_first_field = "1" 이고 的p_fleld_缸St = " 0" 인 경우

                                    뇨l 山＝ 2T
         -t= n일 때의 picture가 P또는 I-picture이고 그 전에 있던 P나 I-picture의

                     r디光at_first_field ="l " 이고 幻p小field_flu亂＝ " 1" 인 경우

                                    tn+1-t= 3T
                                                                119




(b) progressive_sequence = "1" 이고 low_delay = "1" 인 경우

  -t= n일 때의 picture의 repe缸Jmt_field = " 0" 인 P나 I-picture의 경우

                                 tn+l-t= T

  -t= n일 때의 pi（艾ure의 repeat_first_field = 111" 이고

        的p_丘eld血就= 110" 인 P나 I-picture의 경우

                                t+i-tn= 21

   -t= n일 때의 picture의 repeat나first_field = II 1" 이고

        top_field_first ="l " 인 P나 I-picture의 경우

                                tn+1-tn= 3T



(c) progressive卞sequence = II 0" 이고 low_delay = II 0" 인 경우

   -t= n일 I대의 picture가 field s仕ucture인 B-j加ture의 경우

                               t11+1-t   =T/2

   -t= n일 때의 picture가 frame structure인 B七ame이고

        re꺄at fi搭t_field = " 0" 의 경우

                               tn+l =tn = T

   -t= n일 때의 picture가 frame S仕ucture인 B七ame이고

        repeat_first_field = "1" 의 경우

                              t［什1-t, =31/2

   -t= n일 때의 picture가 加me s仕ucture인 P나 I frame이고，

        그 전어］ 있던 P나 I frame의 re倂at fi於t玉e넌＝ '0'떽 경우

                               tn+1 寸n = I

   -t= n일 때의 picture가 frame structure인 P나 Ifr跏e이고，

        그전어］ 있던 P나 Ifran配의 re꺄at니fi搭t_field = "1" 의 경우

                             tn+l 4n = 31/2
120




          -t= n일 때의 picture가 field structure인 P나 I丘an配의 첫 번째 field인 경

                -r
                                         tn+l 山 = T/2

           - t= n일 때의 picture가 fields仕ucture인 P나 Ifran配의 두 번째 field이고，

                그 전에 있는 P나 Ifra끄配이 field structure이거나 re1玘at_first_field =

                     "0”의 경우

                                         tn+l -tn = T/2

           -t= n일 때의 picture가 field structure인 P나 I frame의 두 번째 field이고，

                 그 전에 있던 p나 I frame이 frame structure이거나 rer光at_first_field =

                 Ill,,의 경우

                                          t1}+1 =tfi = T



      (d) progressive_sequence = " 0" 이고 low_delay = "1" 인 경우

            -t= n일 It뀨의 picture가 field s甘ucture인 P나 I丘ame의 경우

                                         뇨l -tn = T/2

            -t= n일 때의 picture가 餉毗structure인 P나 Iframe이고

                     re恥at first毓ld = "0" 의 경우

                                           tn+l 止n = T

            -t= n일 때의 picture가 什知ie structure인 P나 I frame이고

                     repeat_first_field =" 1" 의 경우

                                          tn+l -tdn = 3T/2



      chroma_420_type: 1 bit

          - 단지 역사적인 이유 I대문에 존재．

           - 만약 색신호가 4:2:0이면 progressive_frame 변수값과 무조건 값을 같게

             한다. 그렇지 않으면 " 0".
                                                                  121




progressive_frame: 1 bit
   - jf ("1n) ==> progressive scanning을 해서 얻은 血an［妃을 뜻하며， 이때는

      frame_j玭d鈿i_i乞dct를 " 1"로 해야 한다．

   - if ("0") ==>      progressive frame이 아니라는 의미임．



composite_display_flag: 1 bit
    - if ("1") ==> Con叩osi把신호로 이미 되었기 때문어］ RGB가 완벽하지 않은

      신호를 다시 휘도신호와 색신호로 분리 코딩할 II뀨                          그러한 사실을 알

      려준다．

    - jf (U0ll) ==> 원래부터 분리된 신호인 경우
                        m   v          ax奴

                            fi    sequence
                                eld_
   - ll ("l") ==> 뒤에        sub_ carrier          가 존재한다．
                            burst_ amplitude
                            sub_ carrier_ phase

   - if ("O")   ==>   존재하지 않는다．



va川S : 1 bit
   - if (11") ==> 그전에 PAL로 됐던 신호라는 것을 가리킨다．

   征（11011) ==> 그렇지 않은 경우．



field_sequence : 3 bits
   - PAL에서의 field를 1부터 8까지로 나타내기 위하여．

   小TSC에서의 field를 1부터 4까지로 나타내기 위하여．
    4 표 午45
122




               표4-45 Definition of field_sequence (MPEG IS Table 6-15)
                               fi'山1           fia1ne         fl1d
                              照iuen伐
                               000               l             l
                               001               l             2
                               010               2             3
                               011               2             4
                               100               3             5
                               101               3             6
                               110               4             7
                               111               4             8




      sub carrier   : 1 bit
         - 寸（U0I) ==> sul乂artier와 l血e 丘equency 관계가 卜TSC 또는 PAL의 규정과

            같다는 것을 뜻한다．

         - if ("1") ==> su比artier와 血le frequency 관계가 규격어］ 맞지 않다는 것을
           뜻한다．



      burst_amplitude : 7 bits
            - PAL과 NTSC인 경우에 burst신호의 진폭을 정하기 위하여．

            - 1TU-R 601 기준으로 해서 subcarri町의 진폭을 양자화한 후 전송．



      sub_carrier_phase : 8 bits
            - ITU-R BT.470에 의한 subcarrier으4 위상（phase）을 나타내기 위한 변수
            = 표 4-46


              표． 4띠6D帥n什ion of sub_cariier_財X그羽 (MPE（引S : T야)le 6-16)

                          此b_can佃J由a配           I斗）｛料e
                                                0
                                 0          ([3印 + 256]*0)
                                                0
                                 l          ([360 + 2561*1)

                                               0
                                255        ([3的 +256什256)
                                                                              MPEG
                                                                              니DE0      123



4.3.9, G汕（기卄 r＼月（그trix 日<ten싫on
       quant_m山lx_extension0 {                                  No. of bits    Mnen札IMC
            extension start code identifier                     4             uimsbf
            load_intra叫antiser_mati奴                            1             uimsbf
            if ( load_intra_quantiser_matnx)
                  rntra 恥an出町m毗攷西4]                             S 卞 64        uimsbf
            load_non_intra_quanti眺r_matrix                      l             uimsbf
            if ( load_non_intm_quantiser_matiix)
                 non_intra_quantiser_mat缸［64J                   8 率 64        uimsbf
            Ioad_chromajntra_quantiser_matrix                   l             uin咨bf
            if ( load_chmma_intra_quantiser_matnx)
                 chroma_1ntr2匕quan出ermati奴［641                  8 半 64        uimsbf
            load_c뇨on心non i曲-aquanti斑r_matrix                   l             uirnsbf
            寸（1oad_chrom나on Intra叩antiser_mati奴 )
                 chroma_non小．intra_quantiser_matrix[64]         8 水 64        uimsbf
            next_start_code0

       }



      extension start code identifier                : 4 bits
            H0011'



     IoadJntra_quantiser_matrix: 1 bit
           －迂（"1") ==> quan山：er m毗奴를 다운로드한다는 것을 의미（주로 4:2:2인 경

             우나 4:4:4인 경우에 대해서 여기서 다운로드하며 zig-zag scanning순서

             로 다운로드）.

           －寸("0") ==> quan由er m缸奴를 그대로 유지．



     intra_quantizer_ matrix[64] : 8 x 64 bits
           - zig-zag scanning된 값들을 8 bit로 차례로 전송．
124




      load_non_intra_quantizer_matrix: 1 bit
         - load_intr乞叩an血er_ma虹奴와 내용이 동일．



      non_intra_quantizer_matrix[64] : 8 x 64 bits
         -z地呪ag scan恤띵된 값들을 8 bit로 차려匡 전송．


      load_chroma_intra_quantiser_matrix: 1 bit
         - if ("1") ==> chroma quanlizer mali奴를 다운로드 한다는 것을 의미（주로

            4:2:2인 경우나 4:4:4인 경우에 대해서 여기서 다운로드하며 zig-zag
            scai끄rung순서로 다운로드）.
         - f (11011) ==> chr아na quan山：er nu毗奴를 그다區 유지．



      chromaJntra_quantizer_matrix(64] : 8 x 64 bits
         -z坦呪ag scan恤培된 값들을 8 bit로 차려］로 전송．


      load_chron伯_non_intra_quan血이ma打汶 : 1 bit
         - load_chroma누intra_quan屯er_mali奴와 내용이 동일．


      chroma_non_intra_quantizer_matrix[64] : 8 x 64 bits
         - zig呪ag scannii평된 값들을 8 bit로 차례로 전송．
                                                                                                      125




4.3. ] 0. 디（나ure Display Exten敬＞n
     picture_display_extensionO {                                         No.（寸bits        Mnemonic
           extension start code identifier                                4                山msbf
           的r (i印小:nu趾目＝可fran思centi트硝謫s; i-t-+) {
                 framl}e centre horizontal offset                         16               simsbf
                 marker bit                                               l                bslbf
                 frame centre vertical offset                             16               simsbf
                 marker bit                                               l                bslbf
           }
           next尸甑ai下od的
     }



         이 picture display ex啣臧on은 picture마다 디스플레이 위치를 달리하1 주는 경우

    어］ 이용되는더］ 이러한 예로 pan/scan이 있다. Display size는 sequence display

    exten計on에서 정하1 주는더］ 羽qu이ice display exten舡on이 앞에 존재하지 않으면 이

    picture小叩lay exten없on을 쓸 수 없다．



         extension_start_codejdentifier : 4 bits
               -"0111"



         아래의          frame_center_horizontal_offset,      marker_bit,        丘ame_center_vertic카moffset,

    marker寸 bit의 총 34 b畑는                    num比r可frame下en姓卄set만큼 되풀이되는더1 이

    mui仙町fi枷ne_cen把ro卄set은 다음과 같이 결정된다．



           什 ((progressive_sequence = 1) 11 (pi支ure_structure = "field")) {

                       number_of_frame_center_offset = 1

           } else {

                       汗( repeat_first_field = n1")

                                    number of frame center offset =3

                       이se
126




                        number_of_famecenteroffset =2

       }


       여기서 repeat_first_field = "1" 인 경우에 number_of -丘ame_center_o什set이 3이 되

      는 경우는 반복된 picture어］ 대해서도 오프셋은 달라야 하기 때문이다．



       frame center horizontal off set       : 16 bits
           - 그림 午34에서 보듯이 이 O卄set은 "display rectan멤d의 중심으로부터

             "reconstructed frame" 의 중심까지의 변위를 나타낸다．

           - 변위는 1/16 pixel 단위이며부호는 그림 午34 참조（signed血eger로 표시）.

           . 만약 picture display extension이 존재하지 않으면 바로 이전 값을 그다匠

            이용한다．

           - picture display ex啣sjon을 쓰되 이 오프셋을 이용하지 않는 경우는 0으로

            해야 한다．




                                                                       e十 1由
                                  ;1 fr쏘lle centre - :111         卜
                                                                  e        +
                                                                           4
                               :: i:: horizontal offset : 11




                                                                dis刈ay--
                                                                vei奴Cal size




                                       而야加L加月zonta! size

             그림 4-34 F띠me cent아 O倫et p아ameters ( MPEG I& 日g내eo-16)
                                                                              MPEG
                                                                              니DE0      127




      marker bit : 1 bit




      frame center vertici offset                   : 16 bits

           - 의미는 丘ame center honzont吐O卄set과 동일．

                 1/16 p奴el단위， 부호는 그림 4-34참조（旽ned mteger로 표시）.



      marker bit : 1 bit




4,3.1 ] . Pi(升ure Ten갸JOIC기 Scal（긔ble 日dension
       picture_temporal_scalable_extensiono) {                  No. of bits    Mnemonic
             extension start code identifier                    4              uimsbf
             reference select code                              2              uimsbf
             forward_temporal_reference                         11)            uimsbf
            111別rker bit                                        1              bslbf
             backward_temporal_reference                        jo             U"咨bf
             next_st町_
                     tcode()

       }



      extension start code identifier : 4 bits
             H   1() I0n



      reference select code                    : 2 bits

             啣叩아al sc심ab血ty에서 움직임 보상의 reference를 선택하는 더］ 쓰는 코드．

           - 표 4-47（자세한 것은 5장에서 설명）.
128




                               표4-47 Prediction references selection in P-pictures
                                           ( MPEG IS : T걋이e 工28 )
                              reference select code        forward predic如n reference

                                                  (X)      Most recent decoded enhancement picture(s)
                                                  01       Most recent lower layer frame in display order
                                                      10   Next lower layer frame in display order
                                                           如巾idden




            化rward_旭mporal_reference                            : lOb心

                 - forward prediction을 위한 lower layer reference frame의 tempor出_reference.



            marker bit : 1 bit




            back사ard_temporal_reference                             : 10 bits

                 - backward prediction을 위한 lo＼化r layer reference fran肥의 tempor띠referenc已




      4.3. ] 2. 디（삿ure Spa卄（계 Soak그ble 日den얽（Dn
             picture_spatial_scalable_extension() {                                           No. of bits   Mnemonic
                   exten前on start code identifier                                             4             uimsbf
                   lower_layer_佃nporal_reference                                               10           uimsbf
                   marker bit                                                                  1            bslbf
                   加wer_laver_li山nan砒al offset                                                 15           simsbf
                   marker bit                                                                  1            bslbf
                   lower layer vertical offset                                                 15           simsbf
                   spati；沚ten耳以심J代坦ht c（넋et的le_index                                           2            uimsbf
                   lower_layer下r어甲ess加之frame                                                   l            uim北f
                   lower layer deinterlaced field select                                       l            uimsbf
                   next_start_code(,)

             }
                                                                                            MPEG
                                                                                            피DE0        129




 extension start code identifier : 4 bits
                       -"1001"



 lowerJayer_temporaLreference : 10 bits
                       -l才e小ction을 위한 lower layer reference frame의 temporal_reference.



 marker bit : 1 bit




 lower_layer_h아注ont키HO什set                                : 15b卜冷

                       - spatial scalabilityfl서 enhancement 1ayer의 horizontal offset.

                       - 그림 4-35 참조．


                                           lower I口.yer_pred妃tb月vertle그L針ze幸＼坦忙IC口i고功S그月叩lingfact口乙月 /
                                                                             ye此IC口iJ姓?Sa月IplIngfac切乙月i
                                               IC가ver I따升m加riz口nm小功抑t
                                                               >


  i아verkye乙Ye忙IC缸H功3et




   亡OHHU븅쁜뎌L爰寸끼늠三요
                     山N目 겅m之m>   L小.er Lay心r
                                   Frame



  i口）verlayerpredlctl口月h口rlzo／
                             了taIslze
                                                              low마mlayer_predbcti on-－加riz口月tal s妃8 半
                                                                   加가z이忙al고功＄a川下寸bngfa吐or n /
                                                                   加rizo肋i고功S口刃I)小咽J뇨tor少

그림 4-35 F아mation of the斗＞a枇캬)redk州（)n by m t이p이아ion of lower layer帥：ture
                         (MPEG IS: Figure 7-14)
130




      marker bit : 1 bit




      IowerJayer_verticaLoffset : 15 bits
         .spati띠scalability에서 enhancement layer의 vertical o什set.

         1 그림 午35 참조．



      spatial_temporaLweight_code_table_index : 2 bits
         －妃mporal pre小ction과 spatial I江ediction의 섞는 비율．
         - 표 4-48 참조（자세한 것은 5장에서 설명）.



      IowerJayerprogressive_frame: 1 bit
         - if ("1) ==> lower layer7l- progressive.

         - if ("0") ==> lower layer7l- interlace.
                                                                              口
                                                                               MPEG
                                                                               니DE0          131



 표 4-48 spatial小temporaL weights（그nd s口a恢兀ten기porc止weight_ 永兆計아the
叩에aL teri和아Lweig바_code士珣e_index 아d 叩에a나empor：          止w쉬ght_codes
                         (MPEG IS : Table 7-21 )
   spatial_temporal         spalial_          spa1ia1            spatial           spatial
   wei았1t_code_table       temporal          ten叩oral          temporal           temp긔ral
         index            weight_code        weight (s)        weight class    inte只er_ weight
          (0水
                                               (0.5)                l                 0
          01                  00               (0; 1)               3                 l
                              01              (0; 0.5)              l                 0
                              10              (0.5; 1)              3                0
                              11             (0.5; 0.5)             l                0
          10                  00               (1; 0)               7                 l
                              01              (0.5; 0)              l                0
                              10              (1; 0.5              2                 0
                              11             (0.5;0旬                l                0
          Ii                  00               (1; 0)              2                  l
                              01              仕, 0.5)              2                 0
                              10              (0.5; 1)             3                 0
                              11             (0.5; 0.5)             l                0
           For spati띠_temporal_weight_code_table_index == 00 no spa曲_tempo可weight_c넜e is
           tansmitted.




lower_layer_deinterlaced field select: 1 bit

    - lower layer의 res帥叩血g과정에서 deinterlace시킨 후에 다시 mterlace로 만
       들려고 할 때, 어떤 field를 선택할 것인가를 나타내는 변수．

    - if (lower_layer_deinterlaced_field_select = "1") ==> lower           layer어서        bottom
       field였던 부분을 선택．

    - if (lower_layer_deinterlaced_field_select = "0") ==> lower layer어꺼 top field

       였던 부분을 선택．
132




      4.3.13. O야가畇ht 태ension
           copynghLex妃nsionO{                            No.（寸1:航5   Mnemonic

                exten毖Dn start code iden血ier             4           uimsbf

                cop州ght flag                             l           bslbf

                a坪1yl11g出It山id4巴'Ii出er                   8           1血nsbf

                0I如aal야_copy                             l           bslbf

                re配rved                                  7           uimsbf

                marker bit                               l           bslbf

                copyright_nu岫er_i                        20          uimsbf

                marker bit                               l           bslbf

                (：叩州小t_number_2                          22          uimsbf

                marker bit                               l           bs1bf

                C叩州小t nw的er 3                            22          山nsbf

                ne虹쿄a此code0
            }




           extension start code identifier : 4 bits
                - "0100"



           copyright_flag: 1 bit
                - if (" 1") ==> copyright가 있음을 뜻하며 뒤의 C叩yi帥t nul油er가 이를 구
                  별해준다．

                - if ("0") ==> copyright가 있거나 없을 수도 있으며 이때는 뒤의

                  cop戶휑fl number 1, H2, +3이 모두 0 이 되어야 한다．



           original_or_copy: 1 bit
                - in:" m==> orig血al bit打earn이란 것을 의미．

                - if ("0") => copy된 bitstream이란 것을 의미．
                                                                             133




reserved : 7 bits
    = 미래를 위해서 남겨놓은 bits.

    = 모두 0이 되어야 한다．



marker bit: 1 bit




copyright_num比r_i : 20 bits

    - copyri帥t flu!油er(64bi더의 상위 63부터 44까지의 bit를 나타낸다．



marker bit: 1 bit




copyr也ht_nun伯er그 : 22 b心

    - copyri帥t nur油er(64bi回의 상위 43부터 22까지의 bit를 나타낸다．



marker bit: 1 bit
    -   Hilt.
copyright_number_3 : 22 bits
    - copyright_num比r(64bi비의 상위 21부터 0까지의 bit를 나타낸다．



Cop戶i帥t nul仙er는 다음과 같이 구해지며 그 의미는 MPEG에서 정한다．



  copyright_number = (copyright_number_i <<44) + (c어：)ynght_number_2 <<22)

                     + (copynght_number_3)
134




      4.3.14. Slice
              slice() {                                                                         No. of bits   Mnemonic
                                   slice start code                                             32            bslbf
                          if (veitical_size >2800)
                                       si咀verti川1P心岱an_exten自an                                 3             uimsbf
                          寸（<cequence_sca姃）乞extensio川后present加 the b加工ream.)
                                       if (scalable_m너e == "data parti由ning")
                                               pnon勺Hhi七akpoint                                 7             uimsbf
                          quan仕光r多沁e따le                                                         5             uimsbf
                          if ( nextbits() == '1')
                                       sli氾_extension_flag                                      l             bslbf
                                       inti丑 slice                                              l             uimsbf
                                       引icej加恤e id ens川e                                        l             uimsbf
                                       dk氾mpictui之id                                            6             uimsbf
                                       ＼材tile ( nex山itsO== '1' ) {
                                               extra bit slice       ／半 \V忖i the v汕ie "1" 늬＜/   l             uimsbf
                                               extra infonnation slice                          8
                                       }
                               }
                          exti沮 bit 旦H氾 ／木 \.'iththeva1ue ' {)" 卞／                              l             uimsbf
                          do {
                                       macmbl어：kO
                           }w川e ( nextbitsO 느 '000 0000 0000 0000 어00 0000')
                          next_start_code()

              }



            slice start code : 32 bits

                   - 00000101仕) - 000001AF (H)

                   - 여기서는 slice s恤t cot妃 의 마지막 8 bit가 slic乞yertical_pos抽DII을 가리킨

                          다．
                   - 같은 열（horizont川ro＼끼에 있는 slice_veritc띠_position은 같다．



            slice_vertical_position_extension                                   : 3 bits

                  －丘ame의 line 수가 2800이 넘는 경우의 slic氾HV口tical_position의 八4SB 3 bits
                                                                          135




    - slice_vertic고_position 은 l부터 시작, 그런톄 mb_row는 0부터 시작하므로

      l小row는 다음과 같이 계산한다．



                      mb_row = slice_vertical_position - 1


        slice比r떼_position의       최대값은         AF(H）이므로       175이지만       만약

      slice_v이tical니Pos也on少ten駐on이 존재하면 [1:128］까지의 범위로 제한시

      켜야 한다. 따라서 이렇게 exten舡on이 존재하는 경우의 n通row는 다음

      과 같이 꼐산한다．



 mb_row = (slice_vertic刻_position_extension <<7) + slice_vertical_position - 1


priority_breakpoint : 7 bits
    -da伍partitio恤培에서 데이터를 나누는 기준에 이용된다．

    - sequence scalable extens幻n의 scalable m넜e가 data partition血g일 때만 존재

      한다．

    1 표 4-49
136
      L日1




                          표 4-49 P的向나的kpoint V이ues and assoda怡d seman卄Cs
                                      (MPEG IS : Table 7-30)
            Pt如rity_bi七出叩     S弘itax elements mdud이I in paii山m 配ro
                  omt

                  0           This value is irs心ved f（且 F用rtition 1. 시［si心汁叩耐tion 1 sh세1 have a priority_brealqx月nt
                              equal to 0.
                   l          削I data at the sequence, GOP, pi앉ore and s11ce0 d이wn to 耐rab兀si奴血 吐ceO.
                  2           All data included above, plus macrubl어：k syntax elemen四 up to and including
                              maci刃lit乂k a&L［鈿 mc'꾀nent.
                  3           All d比a included above, plus macmblock syntax elements up to but not including
                              coded_block_p毗帥0.
                4 ...63       Res心ved.
                  64          削［ syntax elements up to and including coded_block...pat1em0 or DC coefficient
                              (dct_dc_diffe七n亡al), and the first (run, level) DOT c比fficient pair (or EOB).t
                  65          사 sy孔ax elements above, plus up to 2 (run, level) DCT coefficient pai요


                 63+]         朋syntax elements above, plus up幻j(mn向에DCT ci玘fficien印面匹．


                 127          All syntax elements above, plus up to 64 (run, level) DCI coefficient pai心.




            quantizer_scale_code: 5 bits
                - 呱ce나 macr아寸ock(）에 다른 叩an血吼Sc出乞C어妃가 존재할 때까지 기존값

                  을 그대로 유지한다．

                - [1:31] 범위에서의 정수값을 가지며 0은 금지．

               1 표 午50
                                                                           137



     표4-50 R이a如n bets사een quan掘이Sc이e and qu아내昑小C이釘ode
                        (MPEG IS : Table 7- )
                                   quantiser中scalelq_scale_typej
 quantiser_scale_code   吼Sc毗_type = 0                   q_scale_type = 1
          0                                 如rbidden)
          l                  2                                 i
          2                  4                                 2
          3                  6                                 3
          4                   8                                4
          5                  10                                5
          6                  12                                6
          7                  14                                7
          8                  16                                8
          9                  18                                10
         10                  20                                12
         11                  22                                14
         12                  24                                16
         13                  26                                18
         14                  28                                20
         15                  30                                22
         16                  32                                24
         17                  34                                28
         18                  36                                32
         19                  38                                36
         20                  40                                40
         21                  42                                44
         22                  44                                48
         23                  46                                52
         24                  48                                56
         25                  50                                64
         26                  52                                72
         27                  54                                80
         28                  56                                88
         29                  58                                96
         30                  60                               104
) r>
5b       31                  62                               112




                                    PCT
                                                 乙
                                                Qci。 ,         .

       ＜프步                                  '




                    小
                    ' "抄斗
                                          9넛乙8六ce7, 了C小／{
138




      slice_extension_flag : 1 bit
          - if (" 1") ==> intra_slice, slice_picture_id_enable, slice_picture_id, ex仕a_bit_slice7f

            다음에 있다는 것을 표시．



      intra 引七e      : 1 bit

          -if（나 " )==> 그 slice 내의 모든 macr的k乂k이 血m라는 것을 표시．

          - 정해진값은 " on, 없어도 " on.

         . 이 변수는 vid印에서 보다는 DS入4-CC 쪽에서 쓰인다．



      slice_picture_id_enable: 1 bits

          - if (tl()II) ==> slice_p奴ure_id가 0이며 의미가 없다．

          - if (11") ==> slice_picture_id가 0이 아닌 값을 갖는다．

          - 디코딩과정에서는 쓰이지 않지만 slice 내의 모든 slice_picture_id小enable

            값은 모두 같아야 한다．



      slice_picturejd          : 6 bits

          -if（나 " ) ==> slice_pic恤eid가 0이 아닌 값을 갖는다.                       이 6bit는 응용예에

            따라서 각자 정할 수 있는더］ 예를 들어 버스트에러가 나는 환경에서

            한 picture마다 sli（氾_picturQ쿄를 같게 줌으로써                        그 slice가 어떤 pic加re

            어］ 속하는가를 알 수 있다．

         . 디코딩과정에서는 쓰이지 않지만 slice 내의 모든 slice_picture_id_enable

            값은 모두 같아야 한다．



      extra bit slice : 1 bit
          - jf (lIlI) ==> 뒤에 ex仕a_informa如n_slice가 존재한다는 것을 의미．

          m 현재는 쓰지 않는다. 따라서 "on.
                                                                            139




extra小information 引把e               : 8b心
   - reserved, 현재는 쓰지 않는다．

   -ex的小追曲ce가 " 1" 이 계속되는 한은 extra_i苾onnation_slice는 계속된다

     (4 "l", exfra_information_slice(8bits), "1", extra_information_slice(8bits),

     .   .   .   .   , Ilnhl   끝）
                                .




macroblock ()

   - 다음에 어떤 start code가 나오지 않는 한 한 slice 내의 macroblock(）이

     계속 전송된다．
140




      4.3.15. Macro block
            macmblockQ {                                                No. of bits   짜In小ionic

                 while ( nex虹IsO == 伽（．肌J01000')
                       inacrobi어水m心cape                                 11            bslbf

                 macroblock add因 increment                              1-11          vlclbf

                 macmblock 'modesO
                 if ( macmblock_quant)
                       quantiser_scale_code                             5             uimsbf

                 if (n皿口小lock_motion_foi批niH
                       ( 蜘Co兆1(姓느岫ra && conce汕nent_mo由n_vec的l引 )
                       motion_vectors( 0)
                 if ( mac仄）block_motion_backward)
                       m曲on_vecto奴 l )
                 if (m出江oblo<永Ii血a && concealment_n均lion_v凹to匈
                       1na1斗［er bit                                     l             bslbf

                 if ( macmblock_pattem)
                       code也蜘出-p川em()
                 for ( i=0; iblock_count; i++) {
                       block( i)

                  }
             }



            macro비ock_escape                  : 11 b心

                 -"0000 0001 000"

                 - macroblock address increment가 33이 넘는 경우에 사용．

                 - 만약 n追croblock_escape가 있으면 address di卄erence는 다음과 같이 계산

                      한다．

                       address difference = 33 + macroblock_address_increment

                 (macroblock_escape가 2개 연달아 있으면 33 대신 66을 더한다）



            macroblock address increment                 : 1 -11 bits

                 - address difference를 코딩하기 위하여 표千釘의 가변장부호 채택．

                 - macroblock 중에서 보내야 힐· 데이터가 없는 경우를 sk巾ped macro砥乂k
                                                                                         141




             이라하고 테이터가 있는 경우를 nonskipped macr小lock이라 하는더］, 이

             address di卄erence는 현 macroblock이 nonskipped인 경우 다음 식과 같이

             이전의 nonskipped macr的1c改과의 어드레스차이를 나타낸다. address

             difference = previous_macrobl어：k_address - current_macroblock_address

            - macr的1O味_address는 그림 午36에서처럼 왼쪽위의 macr아加ck부터 0, 1, 2,

             3, 4순으로 증가한다．




             표 4-51＼幻的ble length codes f아 11띠아야永＞c匕그ddress increment
                                (MPEG IS : I야)le 탸］)
macroblock address        increment value      macrobi어：k addr啣        increment value
m口七ment VI乂二 code                              increment VLC code
l                         l                    0000010101               18
011                       2                    0000010100               19
010                       3                    0000010011               20
0011                      4                    0000010010               21
0010                      5                    00000100011              22
00011                     6                    以000 아00010              23
0001 0                    7                    00000100001              24
0000111                   8                    00000100000              25
0000 110                  9                    00000011111              26
0000 1011                 10                   （刃仄00011110              27
0000 1010                 11                   00000011 101             28
0000 1001                 12                   00000011 100             29
0000 1000                 13                   （刃佚) (刃11011             30
00000111                  14                   以朕00011 아0               31
00000110                  15                   00000011001              32
0000010111                16                   00000011 000             33
0000010110                17                   00000001 000             macmblock_escape
142




           macrob1ock e1dress =0            mecrobi口ck 계Id比弱 = 23


           0   l   2   3   4    5   6   7   8   91   /0 11 12 13           mb xo甲＝ 0
           14 15 16 17 18 19 20 21 22                戶                     0：由 iov= 1
                                                                           mb so斗r= 2




                                            腸易笏物               '      pie vi口us_maciobl그ck_
                                                                      add工ess for slice A.
                                                出妃eA




       mb c。unm= 。

                               그림 4-3o 卜爪丑갓（>1긔（xk（그ddress



      - 보통은 previous_macro比兀k_address는 바로 전의 non skipped macrobli乂k

       의       macrobk兀k address오｝ 같다. 그러나                         slice의 첫 macroblock에서는

       다음과 같이 계산한다．



            pre너ous_macr야加欲크ddress = ( mb_row ' mb_width ) -1



        （설명 : 보통은 address_di什erence를 slice단위로 하는 것이 좋겠지만

       slice구조가 4.1.2절에서 설명했듯이 丘ar配마다 가변적일 수 있기 때문

        어］ slice시작에서는 previous_macr小1O(火_address를 그림 午36어］ 나타난

       것과 같이 그전 열（hod加ntal row）의 끝으로 한다. )



      - 여기서 mb row는 그림 午36과 같이 macroblo火의 row를 위에서부터

       0,1,2,3,4....로 정한 것이며, l小jol山nfl은 macroblock의 column을 왼쪽부

       터 0,1,2,3,4. . .으로 정한 것이다．
                                                                              143




               mb column = macroblock address % mb width



   - slice의 시작에서는 slice_start_co把가 전송되므로 그 start code로부터의 수

     직쪽       위치를     알       수   있으며,      slice의   수평쪽       위치는          그때의

     macr아六乂k_address_increment로 알 수 있다（slice의 첫 번째 macr的뇨：k은

     절대 skip될 수 없기 때문어ii).



   . 다음과 같은 경우에는 macr的lock이 skip되지 못한다．



     a)     I-pi比ure에서는       picture_spatial_scalable_ex把nsiolm이       현picture의

          picture_header() 뒤에1 존재하는 경우나, bits仕earn 내에 sequence_scalable

          1 ex妃nsion()이 존재하면서 scalable_n好把가 SNR             scalab皿ty인 경우를

          제외하고는 절대 skip되지 않는다．

     b) slice의 처음과 끝의 macrobli乂k은 절대 skip되지 않는다．

     c) B-picture에서 in甘a로 코딩되는（즉 macr的1어永_intra=" 1') macrob뇨火바

          로 뒤의 macr的k兀k은 절대 skip되지 않는다．



macroblock_modeO
   - 뒤에 설명할 macrobli乂k_rnode()에서 전송되는 n始croblock_勺恥을 디코딩

     하1     보면    macr아寸ock_quant,     macr아丑ock_motion_f아ward,        macrobl(乂k

     motion_backward, macroblock_pattem, macroblock_intra,          spatial_temporal

     _weight_code－丑ag들이 0인지 1인지를 알 수 있는더］ 이 값들에 따라 다

     음과 같은 변수들이 존재한다．



quantizer_scale_code      :   5 bits

   - iI(macroblock_quant = "1") ==> 이 변수가 존재한다．

   - 이 변수의 뜻은 앞의 표 4-50에서와 동일하다．
144




      motion_vectors(O)
         - forward mot沁n vec幻r 전송을 위한 부분．



      motionmvectors(1)
         - backward motion vector 전송을 위한 부분．



      marker bit : 1 bit




      coded_block_pattern0
         - macroblock 내의 bi以：k들이 코딩되었는가 아닌가를 나타내주는 부분．



      비ockO
         - macr아）lock 내의 모든 블록어］ 대해서 전송（즉 block의 개수（bli兀k叩unt)

           만큼 전송）.

         -DCT계수들을 보내는 부분．
                                                                                           145




4.3' ] 6. 卜月（그（가（>block Modes
      macmblock--modesO {                                           No. of bits   짜Fnenu岫r

           mal거）hi어出；--1;ype                                        1-9           vlcibf

           if ( ( sp毗町tei珥101刻1吼蜘tel넜eflag == 1 ) &&
                (span叱恤fl01川mwei小냐od탸缸e ndex != '00') ) {
                spafialj巴nporai_we自ght_code                         2             uimsbf

           }
           if ( macmbl乂k_motion_forward II
                macmbl며：k_motion_backward) {
                if (pi艾ure下帥啣妃＝= '쇼ame' ) {
                      if ( 丘ame1pred_frame_dct == 0)
                            fram탸no如III叩e                           2             uimsbf
                 }eise{
                      丘eld_motion_ty比                               2             uimsbf

                 }
           }
           if ( (pictuie_stmcture=='Frame picture")&&
               (frame그)fed玉me面t==0)&&
                (macn力岫노蜘비tmacrn뱌)ck_pattem)){
                d& type                                             1             uimsbf

           }
      }



      macroblock누type               :卜9b仕S
            - 표 4-52부터 午58을 살펴보면 다음과 같은 변수들이 등장하는더］ 이들

               표에서는, macroblock type의                   VLC code어］ 따라서     이들 변수들의 값

               이 0 또는 1로 표시되어 있다. 이들 변수에서의 0과 1이 뜻하는 바를

               살펴보면 다음과 같다．



          (a) macr毗寸어永긔uant

            - jf (111") ==> 그 macr的it兀k을 위한 quan血ci－多cale_c넜e가 존재한다．



          (b) macroblock_motion_forward

            -ifm ' ) ==> 그 macroblock의 的rward仙的나ect아가 존재한다．
146




      (c) macroblock_motion_backward

        - if ('1") ==> 그 macr的lock의 backward m曲on ye아아가 존재한다．



      (d) macroblock_pattem

        - if ("1") ==> coded_bk兀kJ坦如m이 존재한다．



      (e) macr야加以intra

        - jf (" 1") ==> 그 macro比乂k이 intra coding된 것을 나타낸다．



      (f) spatial_t巳mporal_weight_code_flag

        - if ( 'O") ==> spatial_ten叩oral_we培ht_code가 존재하지 않는다. 또 spatial_

               temporal_weight_class를 표 4-55시午57에서 찾는다．

        - if ('l ") ==> spati띠卞聊OI刻_weig址下어把가 존재한다. spatial_temi兀ml1

               weight_class를 표 午59에서 찾는다．
                                                                                               147




           표 4-52 V애able 1en아h codes for n띠croblockJ叩em 卜pictures
                             (MPEG IS : Table B-2)
macr川)J어：k_tyj比 VLC code
                    macrobtockquant
                           macroblock motion forward
                               macn由加ck motion backw町d
                                   macroblockpattern
                                        macr야加ck intra
                                            spatiaLtemporal_weightcode_flag
                                                           permitted spat洌如mpoi川_weight_classes
                                                              Description

1                   0      0   0   0    ]   0                    Intra                        0
01                   l     0   0   0    l   0                 Intra, 加ant                     0




          표 4-53 V애able len아h code計아 macroblock_ty口e in P-pi（사ures
                            (MPEG IS : Table B匈
macrobl乂k_type VLC code
                    macroblock_quant
                           macroblock motion forward
                               macroblock motion backward
                                   macroblock_pattem
                                        macroblock mtra
                                            spatial_temporal_weight_code_flag
                                                           permitted spatial_temporal_weight_classes
                                                              D心en的이l

l                   0      1   0   l    0   0                 MC, Coded                       0
01                  0      0   0   l    0   0               No MC, Coded                      0
001                 0      l   0   0    0   0               入4C,卜奴Coded                       0
00011               0      0   0   0    1   0                    Intra                        0
0001 0               l     l   0    l   0   0              ｝너［C, COded, Qu川lt                 0
otx刃 l               l     0   0    1   0   0             No MC, COded, Quant                 0
000001               1     0   0   0    l   0                 Intra, Quant                    0
      MPEG
148   피DE0




                  표 4-54＼八川야1e 陀ngth codes for macroblock_押口e in B-r乂寸ures
                                   (MPEG IS : Table B-4)
        macroblock_type VLC code
                            macro汕乂k叫ant
                                   macrobl어：
                                           k motion forward
                                       macroblock motion backward
                                            macro川ock_pa如rn
                                                 macroblock intra
                                                      spatial_temporaLweight_code_flag
                                                                    permitted spatiat_恤叩or카weight_classes
                                                                       Description

        10                  1)     i   1    1)   I)   0              Interp, Not Coded             0
        11                  (1     1   l    l    0    0                Inteip, Coded               0
        010                 (I     0   1    0    0    0              Bwd, Not Coded                0
        011                 1)     0   1    1    0    0                Bwd. Coded                  0
        0010                0      1   0    0    0    0              Fwd, Not COded                0
        001!                0      l   0    l    0    0                Fwd, Coded                  0
        0001 1              0      0   0    0    l    0                    Intra                   0
        00010                l     l   l    l    0    0             Jnte叩，Coded,（沁ant              0
        00001!               l     1   1)   1    0    0             Fwd,（뇨Intl加ant                 0
        0000 10              l     0   1    l    0    0             Bwd, Coded, Quant              0
        000001               l     0   0    0    l    0                 Tntra, Quaiit              0
                                                                                    匣           149


표 4-55＼八川abl이ength codes for macroblock_押口e in 나)ic仙res with s口（그쉬（싯 sc이야페fy
                           (MPEG IS : T야여eB句
macroblock_type VLC code
                    macroblock_quant
                           macroblock motion forward
                               macrobl어：
                                       k motion backward
                                   niacroblock_pattern
                                               k intra
                                       macrobl어：
                                            spatial_temporal_weight_code_flag
                                                            permitted spatial_temporal_weight_classes
                                                               Description

l                   0      0   0   l   0    0               Coded, Compatible                  4
01                  l      0   0   l   0    0            COded, Compatible, Quant              4
0011                0      0   0   0    l   0                     Intra                        0
0010                 l     0   0   0    1   0                  Inira, Quant                    0
0001                0      0   0   0   0    0             Not COded, Compatible                4
150




             표 4-5o Variable len아h codes for m그아야긔（Dck_iy口e in P-pictures \A／附）sp에이
                                 scalab咐v (너P日3IS : 伯ble B- )
      macr야如k自恥 VL(노ode
                         macroblock_quant
                             macrobl어：k motion forward
                                 macrobl어：k motion backward
                                     macroblock pattern
                                            macroblock mtra
                                                spatial_temporal_weight_code_flag
                                                                permitted spatialtempora1_weightc1asses
                                                                   Description
      10                 0   l   0    l     0   0                  MC, COded                     0
      011                0   l   0    l     0   l             MC, Coded, Compatible             1,2,3
      00(刃 100           0   0   0    1     0   0                No MC, Coded                    0
      000111             0   0   0    l     0   l          No MC, Coded, Compatible             1,2,3
      (）아0               0   l   0    0     0   0                MC,N아Coded                      0
      0000111            0   0   0    0     l   0                     Intra                      0
      0011               0   l   0    0     0   1          入'IC小奴 C（넜ed, Compatible             1.2,3
      010                l   1   0    1     0   0               MC, Coded, Quant                 0
      00(끄 어0            1   0   0    l     0   0             No MC, Coded. Quant                0
      0000 110           l   0   0    0     l   0                  Intra,（加ant                   0
      11                 l   1   0    l     0   l        MC, Coded, Compatible, Quant           1,2,3
      0001 01            l   0   0    1     0   l      No MC, Coded, Compatible, Quant          1,2,3
      00(끄 10            0   0   0    0     0   l        No MC, Not Coded, Compatible           1,2,3
      0000 101           0   0   0    l     0   0               Coded, Compatible                4
      0000 010           l   0   0    l     0   0          Coded, Compatible, Quane              4
      0000 011           0   0   0    0     0   0             卜幻eC（넜ed, C帥patible                4
                                                                                          區              佰，


       표 4-57 Va的ble length codes for macro炚兀Uype in B-pictures \A／附싸刃ti이
                           sc（그labilily (MPEG IS : T야1e B力
macroblock type VLC code
                        m批roblock_叫ant
                           macroblock motion forward
                               macrobl어：k motion backward
                                       macr이Iockp毗eml
                                               macroblock intra
                                                   spatialHtempora1weightc에e_flag
                                                                  permitted 斗atial temporal weightclasses
                                                                      Description
10                  0      l       l   1)      0   0               lnterp, Not coded               0
11                  0      1       l       1   0   0                 Interp, Coded                 0
010                 0      0       l   0       0   0                Back, Not coded                0
011                 0      0       l       l   0   0                 Back, Coded                   0
0010                0      l   0       0       0   0                For, Not coded                 0
0011                0      l   0           l   0   0                  For, Coded                   0
0001 10             0      0   1       0       0   l        Back, Not Coded. Compatible          1,2,3
00(끄 II             0      0   l       1       0   l          Back, Coded, Compatible            1,2,3
000100              0      1   C)      0       0   l         For, Not Coded, Compatible          1,2,3
000101              0      l   C)      l       0   1          For, Coded, Compatible             1,2,3
0000 110           0       0   0       0       l   0                     liTha                    0
0000111             1      t   t       l       0   0              In妃叩，Cod呱 伽mt                   0
0000100             l      l   0       l       0   0              For. C에ed. Qu出lt                0
0000 101            l      0   l       l       0   0              Back. Coded, Quant              0
0000 0100           l      0   0       0       l   0                 Inlia, Quant                 0
0000 0101           l      1   0       l       0   1       恥r, Coded, Co呻atible, Quant           1,2,3
000001100           1      0   l       l       0   l      Back, Coded, Compatible, Quant         1,2,3
000001110          0       0   0       0       0   0          ｝的tC（넜ed, Con꾸atible                4
00(刃 01101          [     0    0       l       0   0         Coded, Compatible, Quant             4
000001111          0      0    0       ]       0   0              Coded, Compatible               4
152




              표 4-58 VaabIe Ien步h code計아 macroblock加p이n 나Dict내es, P- 이cture, 먀永少ure
                                w的 SNRsc（킷ab附y (MPE（引S : T야扼 B-8)
          macr斛叱k帥肥 VLC code
                                     macroblock_quant
                                          macroblock motion forward
                                                macrobl어：
                                                        k motion backward
                                                     macroblo出-f毗eml
                                                                  k intra
                                                          macrobl어：
                                                                spat珌尸tempol川wei小t_code_flag
                                                                                 Pe1lm伽d spatial_t帥poral_wei小tdasses
                                                                                    D心cnption

          l                          0     0    0     l    0    0                        Coded                        0
          01                         l     0    0     l    0    0                  Coded, Quant                       0
          (）아                        0     0    0     0    0    0                   Not Coded                         0



                     표 4-59 Intended 佃Ilowed) sp카K게HtemPt系그L낚后ightcode_tablejndex
                                           (MPEG IS 汗able 工20)
                                                    Lower layer format     Enhancem心蛇            spatial temporal weight
                                                                           layer format          code table index

                                               Progro渭we or in缸比ed         Progressive           00
                Progressive coincident with e川L}ancement layer top fiel玉   Interlaced            10 (00; 01; 11)
      Pmogressive coincident with enhancement layer from bottom fields     Interlaced            01 (00; 10: 11)
                         Interlaced (picture stmct山e == Frame-Picture)     Interlaced            어0orll (01; 101
                          Interlaced (picture st끄cture 뇨 Frame-Picture)    Interlaced            00




                spatiaLtemporaLweight_code                            : 2 bits

                      - spati심scalab小ty인 경우 사용．

                      - spati出prediction과 temporal prediction의 섞는 비율을 나타낸다（5장에서 설

                         땅）   .




                아래 두 丘ame小motion叫type 과 field_mo如n口恥은 macrobli乂k_motion_forward

              나 macroblock_m曲on_backward가 둘 중어］ 하나라도 1인 경우어］ 존재한다．
 frame_motion_type : 2 bits
        - fra끄叱picture인 경우 존재한다．
       1 표 午60


           표 4七乂）M的nning of 的me_rn에on I'叩e (MPEG & Table 6-口）

code       spatial_temporal   prediction ty比    motion vector   my 白mast     dinv
             weight_class                           count
 00                              reserved
 01              0,1            Field-based          2            field       0
 01              2,3           Field-based            1           斤1d         0
 10             0,1,23         Frame-based            l           frame       0
 11             0,2,3          Dual-Prime                         field       l



field_motion_type : 2 bits
      - field picture인 경우 존재한다．
      1 표 午61


           표． 4亡］ Meanning of fi터drl）아ion_iy口e (MPEG IS : T야)le 6-18)

code      spatial_temporal    prediction t키：比   motion vector   my formnat   dmv
             weight_class                           count
00                               reserved
01               0,1           Field-based            l            field      0
10               0.1            16昭 入4C               2            field      0
11               0             Dual-Prin妃             l            field      l




dct_type      : 1 bit
       -f油d DCT인가 丘an妃DCT인가를 나타내기 위하1 사용．

       －迂（"1') ==>macro늬ock이 field DCT 코딩됨．

       - dct type이 없는 경우의 dctUpe은 표 午62와 같이 결정된다．
154




                           표 4-62 V（미ue 아dct押口e 仟 dot押口e 恰 n(＞什卄he bit針ream
                                          (MPEG IS : Table 6-19)
                                                        Condition     dct_type

                                       picture_structure == "field"   unused because there is no framelfield distinction in a field
                                                                      picture.

                                       frame_i胱d鈿ne dct== 1           0 ("frame")
                        !(macroblc乂k_intra 恤mm뱌姚_patt帥） unused - macrobl어k is not coded
                                            ma（江obli乂k is skipped     unused - macmbl어永 is n야 coded




      4.3, ] 7 , 入爪＞tion Vect아S
              motion_vectors ( s) {                                                                 No. of bits      Mnemonic

                   if (motion_vector_count == 1) {
                           if ((mv_format==field) &&( 山mv !=1))
                                                ［上eld刻吐t(0}[s]
                                  rn［川ion vertic刻                                                   l                uimsbf

                           motion_vec幻r( 0, s)
                    }else {
                           rnotion_vertical_field_select[0]lsl                                      l                uimsbf

                           mot幻n_vector( 0, s)
                           motion_vertical_field_select[1][sl                                       l                uimsbf

                           motion_vector(1, s)

                    }
              }



             m아1O口vert七al_f ield_select[r]［司                               : 1 bit

                   - if ("0") ==> top reference field가 움직임 예측어］ 쓰인다．

                  －迂（'1") ==>b아抑ii reference field가 움직임 예측어］ 쓰인다．

                   -r고干 S의 뜻은 다음과 같다．

                          r -->    0     first motion vector

                           -->     1     second motion vector

                          s -->    0     forw缸d motion vector

                           -->     1     backw町d motion vector
                                                                                           MPEG
                                                                                           VIDE0         155
                                                                                           1




            - motion_vector_count, mv_format, dmv는 표 460, 461어1.



      m야ion_vect아化히

            -m아ion_code와 m아加n爬Si(加al을 보내는 부분

             (motior나帥아는 mo如n_code와 n姓ion r田油ml로 나뉘어 전송된다）.




4.3.18. Motion Vector
       motion_vector ( r, s) {                                          No. of bits            Mnemonic
             molion_codetr][s][0]                                            1-
                                                                                      11       vlclbf
             if ( (f_code[s][0] != 1) && (motion_code[r][sj[0] !=0) )
                   m아加n_residu叫r][s][0]                                 I 8       -
                                                                                               uinisbf
             if (dmv== 1)
                   dmvector[0]                                           1-
                                                                                      2        vlclbf
            molion_code[r][s]11I                                        卜］l                    vlclbf
            if ( (f_code[sl[1] != l) &&(motion_code[rl[s][1] '= 0) )
                   mo由n_residual[r][sl[1]                               1-
                                                                                      8        uin咨bf
            if (dmv== 1)
                   dmvector[1I                                          1-
                                                                                      2        vlclbf
       }



     motion_code[r][s][t] : 1 - 11 bits
           1 표 午63

           - 의미는 5장에서 설명．
156




          표 4-o3 Va的ble len아h codes f아 m아ion小code (MPE（引S Table 田0)
                   Variable lei埋1h刃de    moti月_
                                              lcode[r][s][tl

                   00000011 001          -16
                   00000011011           -15
                   00000011 101          -14
                   00000011 111          -13
                   00000100001                12
                   00(刃 01(刃 011         -11
                   0000010011            -10
                   0000010101            -9
                   00000101 11           -8
                   0000 0111                  7
                   00001001              -6
                   00001011                   5
                   0000111               -4
                   00011                 -3
                   0011                  -2
                   011                   -    1
                    l                    0
                   010                   l
                   0010                  2
                   00010                 3
                   0000 110              4
                   0000 1010             5
                   00001000              6
                   0x刃0110               7
                   00000101 10           8
                   000001아 ()0           9
                   0000010010            10
                   00000100010           11
                   00000100000           12
                   00000011 110          13
                   00000011 100          14
                   （刃000011010           15
                   0000刃11 000           16




      n伯tion_residua巾］[s][t] : 1 = 8b心
         - 의미는 5장에서 설명．
                                                                                                                 157




     dmvector: 1 -2 bits
          1 표 4-64

          - 의미는 5장에서 설명．


            표 小64 Variable len尹h codes 向rdrr叭ecto巾）(MPEG IS : Table B-il)
                                 code                       value
                                   11                        -   1
                                   0                             0
                                   10                            l




4.3, ] 9 （兀ded 텨ock Pa卄em
      (X너e& block_patt帥 () {                                                              No. of bits   Mnemonic
           coded_blo吐pa仙吐기m420                                                            玉9            vlclbf
           if ( chroma_fotmat == 4:2:2)
                coded川ock恥伽ml                                                             2             uimsbf
           if ( chroma_fomiat == 4:4:4)
                coded_block_j帥岫n2                                                         6             uimsbf

      }



     codedJ이ock巾a如rn _420 : 3 = 9b心
          1 표 4-65

            이 표에서 각 \/LC code어］ 따라서 cbp값을 얻을 수 있다. 이 cbp값은

             macroblock 내의 block number가 i (i= 0,1,2,3 ...）인 bi以k이 코딩되면（그림

             4-15, 4-16, 4-17 참조） 그때의 pattern._code[i]를 1로 하고 그렇지 않으면

             0으로 해서 다음과 같이 계산된 값이다．


                                            5

                                   cbp =   2
                                           i=O
                                                 pattern_            code[ij   x2   (5D
158




                  표 小55 ＼八川able len아h codes f아coded_blocKp咐em)
                               (MPEG IS: Table B-9)
      code&blo&pattem VLC     cbp             code&蜘吐-p硝em VI兀   cbp
      code                                    （甘川Je

      111                     d)              00011100           35
      1101                    4               00011011           13
      1100                    8               0001 1010          49
      1011                    16              0001 1001          21
      1010                    32              0001 1(刃0          41
      10011                   12              00010111           14
      10010                   48              00010110           50
      1(刃01                   20              0001 0101          22
      10000                   40              0001 0100          42
      0111 1                  28              00010011           15
      01110                   44              0001 0010          51
      01101                   52              0001 0001          23
      01100                   56               0001 0000         43
      0101 1                  l                00001111          25
      0101 0                  61               0000 1110         37
      0100 1                  2                00001101          26
      01000                   62               0000 1100         38
      001111                  24               0000 1011         29
      001110                  36               0000 1010         45
      001101                  3                0000 1001         53
      001100                  63               0000 1000         57
      0010 111                5                00(刃 0111         30
      0010 110                9                00(刃 0110         46
      0010 101                17               00000101          54
      0010 100                33               00000100          58
      仗11이끄 l                 6                000000111         31
      0010010                 10               0000 00110        47
      m아0001                  18               0000 0010 1       55
      0010000                 34               000000100         59
      0001 1111               7                000000011         27
      0001 1110               11               000000010         39
      0001 1101               19               000000001         0 (NOTE)
      NOTE - This ently shah姓be used w沚따:2:야hn加inance S如cture
                                                                             MPEG
                                                                             피DE0   159




   - b1乂k下ount는 macroblock 내의 블록의 개수이며                                     표 午66과 같이

       chrominance form欲어］ 따라 다르지만 如rmat어］ 관계없이 block I仙仙er가

       5인 block까지의 pattern_c넜eiJ는 여기서 구한다．



coded上1O比_patternJ : 2b心

            chrom血ance 如rmat이 4:2:2인 경우어］ 있어서는 pattern_c어le[i]가 2개 더

       필요한데 i= 6, 7일 때의 pattern_code[i]를 나타내는 bit를 표시한다．



coded上lo比_pattern그 : 6b心

   -        chron伽ance 白rmat이 4：牛4인 경우에 있어서는 pattern_code田가 6개 더

       필요한테 i = 6, 7, 8, 9, 10, 11일 때의 pattem_codeli]를 나타내는 bit를 표

       시한다.           종합적으로 decoder에서는 pattet兀code田를 다음과 같이 구한

       다．
   奴乍U;K12;i卄）

       if(macr야加ck_intra)

             pattern_code[il = 1;

       터se

             pattern code[i] = 0;




  氓macr야旭水＋帥em)

       幻r乍0;k釘＋+)

             if(cbp&(1<<(5-i))) paattem_code[i] = 1;

             什(chroma卞format == "4:2:2")

              for乍6；
                   卜田奸＋)

                 if(coded_blocL冶ttem_1 & (1<<(7-i))) pattem_codejj] = 1;

       if(chrom之幻m欲 牛 '4:4:4")
160




                            佃r(i=6；
                                  卜＜12;i-H-)

                               作(c여ed_blo水 汨ttem_2 & (1*z(11-i))) pattem_codeti] =1;


                   }


            예를 들어 4:2:2인 경우 cbp값이 14이고 q넜吐bic以恥tt心ie1이 2인 경우는

          bkx火num比r가 2, 3, 4, 6인 블록이 코딩되었다는 것을 가리킨다．


                               표 4-65 block count as a function 아 ch幻ma forn心t
                                            (MPEG IS : Table 6-20)
                                         chroma format                           ［c只m1t
                                                                             bi［거出

                                               4:20                              6
                                               中2:2                              8
                                               4:4:4                             12




      4.3.20. Block
            block(i) {                                                                    No. of bits   入4n口11 刃ic
                  if ( pattem_c닙e[il ) {
                         if ( ma그iblock_intra)   {
                                    if (i<4) {
                                                 dct dc 毗配 luminance                      2-9           vlclbf
                                                 if(dct_dc_size卞luminance !=0)
                                                             dctdcdiff끼叫ifial             1-11          비m的f
                                     }else{
                                                 ti吐 dc 寸配 （出on血日nee                      2-10          vlclbf
                                                 if(dct녀C毗仁曲m恤Ian凹 !=0)
                                                          dct dc differendal              1-11          uimsbf
                                     }
                        }else{
                                    First DCF Ct比ifici口It                                 玉24
                        }
                        wh扼 ( nextb心0 != End可比乂k)
                                   效小S띠出nt DCT Ct玘侄icients                                2-24
                        End of block                                                      2or4          vlclbf
                  }
            }
                                                    MPEG
                                                    피DE0   161




 위에서 구한 pattern_c（넜아i]=1이면 그 블록은 skip하지 않으므로 계수를 디코

딩 한다．



 dct dc size luminance      :   2- 9 bits



 dct dc d附이ent治1 : 1- 11 bits

    - pattern_cod可i]=1이면서 macrobli乂k이 intra mode인 경우에는 휘도신호에

        대해서 U血aDC만을 따로 dct_dc_size_lum血ance와 d아1dc1di打erential을

        이용해서 코딩한다（5장에서 자세히 설명）.



 dct dc size chrominance        :2- 10 bits



 dct dc differential   : 1 -11 bits

        pattern_cod아ii = 1이면서 macr아加ck이 inira mode인 색신호어］ 대해서

        intra_DC만을 따로 dct面S汰下hn町iinance와 dct血코咐erential을 이용하1

        서 coding한다（5장에서 자세히 설명）.



 other dct coefficients
     -in仕a block의 DC를 제외한 다른 DCT계수들은 모두 VLC table을 이용해

        서 코딩한다（5장에서 자세히 설명）.
n=O이면 DC계수이고 아니면 그
뒤의 AC계수를 나타낸다.     보통
intra Co네四에서의 DC계수는 크
기가 보통계수외는 守, 매우 크
기 때문에 VLC table을 이용하는
보통의 계수들과는 다른 방법올
이용하여 코딩힌다．
164    堪흐

 5. 복호화과정

          복호화과정을 블록별로 그려보면 그림 5-1고｝ 같다. 여기서 움직임 보상

        (motion com玘nsation) 부분은 5.2절에서 따로 다루고 있다．




                                   Val始川e           Inverse
                                    Length            Scan
                                   Decoding
            C음dedata+
                                         Inverse                           Motion        Decoded


                                                                                    \
                                                              Inverse     Compen
                                         Quantis-                                       卜謚砥；
                              1卜
                                                                DCT        sation
                                           ation

                                                                         ［玎
                                                                        力］
                        2림 5-1 Simplified Video Decoding Process (MPEG IS: Figure 7-1)



            이제부터 이 블록별로 하나하나 살펴보기로 한다．



      5.1. 역양자화와 역DCI
      5.1.'] . 가변장복호호如그rk그ble len아h deco에n助
            이 과정은 bit馳earn으로부터 가변장부호화된 Dcr계수를 뽑아서 그 역과정을

         거쳐 QFS[n］을 얻는 것이다. n =0이면 DC계수이고 아니면 그 뒤의 AC계수를

         나타낸다.             보통 intra coding에서의             DC계수는 크기가 보통꼐수와는 달리 매윈

         큰가 때昰에 VLC table읔 이용하는 보통의 꼐수들과는 다른 방법을 이용하여

         르딩한다H또한 절대 크기를 전송하는 것이 아니고 전 블록의 해당되는 값과

         비교해써 그 차아만을＋，송 }                                다. 따라서 pred奴or를 이용하게 되는더］ 이

         prod奴아는 바로 전 블록의 계수값을 갖게 된다. 여기서 표기를 편하게 하기 위

         하여 C이or component를 CC라 표기하고 cc=0이면 휘도신호를, Cb component의 CC
                                                                        165




    를 1로 Cr component 의 cc를 2로 표시한다. 따라서 한 macro b뇨火에서의 block

    flu!小er와 그어］ 따른 cc값을 표시해보면 표 5-1콰 같다．


         표 5-1 Defir們on아cc, C이（汕component index (MPEG IS : Table 7-1)




N    /／功a block에져의DC계수들 (coe厥兆n勾

     lntrabl어火의 DC차이값을 그대로 가변장부호화하기에는 너무 많은 값들이 있

    기 때문어］ VLC table을 이용하지 않고 d아1dc小S也와 dct_dc_ differential 의 두 부분

    으로 나누어서 코딩한다. dct_dc_size는 표 5-2와 5-3과 같이 휘도신호와 색신호

    어］ 대한 것이 있고， 그 variable leng血匈妃가 2bit- 10 bit까지 할당되어 있다．
166




                표 5-2 V（孤그ble len아hcodesf아dct_dc_size_lumin아兀e
                               (MPEG IS : Table B-12)
                Variable length code   dct dc size luminance

                100                    0
               00                      l
                01                     2
                101                    ;
                110                    4
                1110                   S
                11110                  6
                1111 10                7
                1111 110               8
                1111 1110              9
                1111 11110             10
                111! 1111 1            11



               표 5-3 ＼八개able len아h codesf아dct_dc_s比 나ominance
                                (MPEG IS : Table B-13)
                Variable length code   dct dc size chrominance

                00                     0
                01                     l
                10                     2
                110                    3
                1110                   4
                11110                  5
                111110                 6
                1111 110               7
                1111 1110              8
                111111110              9
                1111 1111 10           10
                1111 1111 11           11




      표의 오른쪽 항에는 dct 叱size값이 표시되어 있는더］ 이것이 바로 dct dc--

      di卄erentiaI의 bit 수가 된다. dct_dc없ze가 0이면 그냥 dct_th乙size의 code만 전송되

      고 0이 아니면 그 뒤에 dct dcHSi配의 bit 수만큼 dct.dc-, di侄erential으｝ 값을 전송

      한다. Decoder에서는 dct_dc코迂ferential값을 이용해서 d아코湃를 구한 다음 이 값
                                                                                 167




을 pred奴아값에 더한다. Pred奴아는 cc= 0, 1, 2인 서］ 개의 경우어］ 한 개씩 도합

3개가 있는더］ 이 각각의 pred奴아의 값을 dct_dc_p妃d[cc］라 한다. dct d湃값을 같

은 cc값을 갖는 d아_dcj胱d[cc］어］ 더한 다음 그 더한 값을 다시 predictor어］ 저장

한다． 즉 dct_dc_pred[cc］값을 새로운 값으로 갱신시킨다. 이 predi아아의 값은 다

음과 같은 경우에 표 5-4와                       같이 intradc皿ecision ( picture_coding_ex妃nsion어］

있음）에 따라 리셋시킨다.



      a) slice의 시작에서

      b) non_u血a macrobl(乂k이 디코딩될 때마다

      c) macro뱌乂k이       skip될 때마t衣즉 macr的1(乂k_address_increment> !인 경우）


     표 5-4 Relation b帥ween in椒工dc_precision and 卄冷 pred匕for reset v（계ue (MPEG IS :
                                    化ble 7-2)                           "
             虹ra_dc_pre小ion            Bits of precision         reset value
                     0                        8                      128
                     1                        9                      256
                     2                        10                     512
                     3                        11                     1024



      Dct山乙differential은 unsigned integer이고 dct_dc_size로 dct dc di抒erential의 bit수

를 지정해 주기 때문어］ 다음과 같이 d아d咐를 계산하꺼 pred奴아의 값에 더한

다．
         什 ( dctj丸_size = 0)
         {
            dctd附＝0;
        ｝이se{
            ha足J帥ge= 2사dct+dc싫ze - ] );         Note A denotes power (not XOR)
            卄（dct_dc_diffe囹出al >= h帥_range )
            dct_d澍 = dct_dc_d咐erentiai;
           터se
            dct d咐＝( (k兀出J캐ferenti졔 + 价 (2* half_range);
        }
        QFS[0] = dct_dc_pred[cc] + dct_d附
        dctdcj爬마떠 = QFS［이；
168   塑
         예를 들어 휘도신호의 경우를 살펴보면 표 5-2에서 variable length c어妃가

       1110011이면 dct_dc_size=0이 된다. 또한 d아1dcd咐erential=0이 된다. 따라서 dct_diff

       도 0이 된다. 반면 variable len맘he어妃가 "00" 이면 d야Hdc小缸ze는 1이 되며 따라서

       뒤따라오는 d아1dc1小卄erenlial은 1 bit가 된다. 이때 h띠f_range = 2八0= 1이 된다. 따

       라서    뒤따라오는           d아코cdi卄erential이         " 1" 이면   위의       d吐－di拜＝1이   되며

       d아1dcdi卄erential이     "0" 이면      dct_di卄＝ -1이 된다. 또한 var始ble leng由code가 "

       01" 이면 h띠f_range가 2가 되며 그따I d야4dc1di卄erential이 2 bit가 된다． 그때의 값

       이 0,1,2,3이면 그따1 대응되는 dct di什값은 각각 -3, -2, 2, 3이 된다.                    이따1 士 1값

       이 생기지 않는 것은 바로 위의 variable length c에e가 (110011인 부분에서 cover하기

       때문이다. 이와 같은 방법으로 디코딩이 꼐속 진행된다.



      N 다른 계수들 moe所den均
         표 5-5와 같이 표 5-6과             5-7에 의해서 VLC 코딩된다.              이 표5-6과 표5-7을

       자세히 살펴보면 약간씩 틀린것을 알 수 있는더］ 인코더에서는 두 VLC table중

       bit수를 적게 발생하는것을 선택하Al 코딩하면 되고 이를 ii血之vlc_format을 통

       해서 표5-5와 같이 디코더에 알려준다．




              표 5-5 Selec竹＞n of DOT coefficient V匕二tables (MPEG IS: Table工3)
                                infravlc_fonnat        0             1
                                     intra blocks
                                                    t삯加 5毛       table 5-7
                           (macroblockintra = 1)
                                non-inira blo永s
                                                    table 5-6    t삯,le 5-6
                           (macroblockJntra = 0)
                                                                                            169



              표 5-o DOT coefficients T야DIe zero (MP日; is : T야Die B-14)
Variable length code (寸OTE1)                 mn                                 1ev（毋
10 (NOTE 2)                                  End of Block
1 s (NOTE3)                                  0                                  l
11 s (寸OTE 4)                                0                                  l
0ils                                         l                                  l
OlOOs                                        0                                  2
0101 S                                       2                                  l
仄110 is                                      0                                  3
00iiis                                        3                                 l
0011 0s                                      4                                  l
0001 lOs                                     1                                  2
ocx끄 Us                                      5                                  l
0001 01 S                                    6                                  l
0001 00 s                                    7                                  l
0000 ilOs                                    0                                  4
0000 lOOs                                    2                                  7
0000 ills                                    8                                   l
0000 101 S                                 9                                     l
000001                                     Escape
(）아00U0s                                   0                                     5
0010 0001 s                                0                                     6
0010 0lOls                                 l                                     3
0010 0100 s                                3                                     2
(）아00llls                                  10                                    l
(）아00011 S                                 11                                    l
0010 0010 s                                12                                    l
0010 01300 s                               13                                    l
00000010 lOs                               0                                     7
000000l100s                                l                                     4
0000001011 S                               2                                     3
00000011 u ls                              4                                     2
0000 0010 01 s                             5                                     2
00000011 10 S                              14                                    l
0000（刃1101 S                               15                                    l
000000l000s                                16                                    l
NOTE! - The last bit 's' deno妃s the sign of the level, '0' for positive '1' for negative.
NOTE2 - "End of Block" sh沚 not be the only code oft he block.
NOTE3 - This code shall比 used for the first (DC) coefficient in the block
NOTE4 - This c에e sh沚比이珞ed for 訌比血er coe佈cients
170




              표 5-a（겨i속）DOT coef依始nts 伯ble zero (MPEG IS : I야긔e B-14)

      Variable len멧h code (NOTE)      fin                      level

      000000011101 S                  0                        8
      어300 IX刃1 1000s                 0                        9
      000000010011 S                  0                        10
      00000001 0000s                  0                        11
      00000001 1011                   l                        5
      0000 00010100 S                 2                        4
      00000001 il凹s                   3                        3
      0000 00010010 S                 4                        3
      00000001 lil0s                  6                        2
      000000010101 S                  7                        2
      00000001 00끄                    8                        2
      00000001 1111                   17                       l
      000000끄 l0l0s                   18                       1
      000000끄 1001 S                  19                       l
      04그000(刃10111s                  20                       l
      0000 00010110 S                 21                       l
      00000000 li0l0s                 0                        12
      0000000011001 S                 0                        13
      0000 0000 11000 S               0                        14
      00000000 1011 is                0                        15
      0000 0000 10110 s                l                       6
      00000000 1010 is                 l                       7
      00000000 l0l00s                 2                        5
      0000 0000 l00lis                3                        4
      0000 0000 10010 s               5                        3
      000000001000 is                 9                        2
      00000000 10000s                 10                       2
      0000 0000 11111 S               22                       l
      0000 0000 11110s                23                       i
      000000001110 Is                 24                       l
      00000000 ill00s                 25                       l
      000000001101 is                 26                       l

      NOTE - The last bit 'Sr denotes the sign of the level, '0' for positive, '1' for
      negative.
                                                                                           171



           표 5-a（계속）DOT coefficients T（갔)Ie zero (MPEG IS: T（갔)Ie B-14)
Variable length code (NOTE)                   nun                                level
00(刃 (xx刃 0111 11 S                           0                                  16
000000000111 l0s                              0                                  17
00(刃 (xx刃 011101 S                            0                                  18
0000 0000 011100 S                            0                                  19
0000 00刃011011                                0                                  20
0刃000000110 l0s                               0                                  21
00000刃0011001 S                               0                                  22
0000 0000 0110 00 S                           0                                  23
000000000101 u s                              0                                  24
000000000101 l0s                              0                                  25
0刃00000010101 S                               0                                  26
00000000010100s                               0                                  27
00000000010011 S                              0                                  28
000000000100 l0s                              0                                  29
00000000010001 $                              0                                  30
0000 0000 0100 00 g                           0                                  31
0000 0000 0011000 S                           0                                  32
000000000010 ills                             0                                  33
以以刃 0仄刃 0010 ll0s                             0                                  34
以00000000010 101 s                            0                                  35
000000000010 l00s                             0                                  36
000000000010011                               0                                  37
00000000 0010 0l0s                            0                                  38
0000 0000 0010 001 S                          0                                  39
0000 0000 0010 000 s                          0                                  40
000000000011 h lis                            l                                  8
000000000011 li0s                             l                                  9
0000 0000 00II 101 s                          l                                  10
00000어：00011 l00s                             1                                  11
000000000011011 S                             1                                  12
0000 0000 00 11010 s                          l                                  13
000000000011001 S                             l                                  14
NOTE - The last bit s denotes the sign of the level, '0' for positive, '1' for negative.
172




            표 5-o에속） DCI Co可ficients Table z이（>                              (MPEG IS: I야시eB-14)
      Variable length code 們OTE)                  nm1l                              level
      000000000001 0011 s                         l                                 15
      000000000001 0010s                          l                                 16
      000000000001 0001 S                         l                                 17
      000000000001 0000s                          l                                 18
      000000000001 0l00s                          6                                 3
      000000000001 l0l0s                          11                                2
      0000000000011001 s                          12                                2
      000000000001 1000s                          13                                2
      0000 0000 0001 0111 s                       14                                2
      0000 0000 00010110 s                        15                                2
      0000000000010101 s                          16                                2
      000000000001 1111 s                         27                                l
      000000000001 lil0s                          28                                l
      000000000001 1101 s                         29                                l
      000000000001 il00s                          30                                l
      000000000001 1011 S                         31                                l
      NOTE - The last bit 's' denotes the sign of the level, '0' for p面山e, '1' for negative.
                                                                                        區   ，兀


           표5-7 DOT coefficients Table one (MPEG IS : Table B -15)
Variable length code (NOTEI)              rim                              level

0110 NOTI끄                                End of Bk乂k
l0s                                       0                                l
0l0s                                       l                               l
il0s                                      0                                2
0010 1 S                                   2                               l
0111 S                                    0                                3
00llls                                     극                               l
0001 l0s                                   4                               l
00ll0s                                     l                               2
0X끄 u s                                    5                               l
0000 il0s                                  6                               l
0000 100s                                  7                               l
ill00s                                     0                               4
0000 ills                                  2                               2
0000 101 S                                 8                               l
1111 000                                   9                               l
000001                                    Escape
1110 1 S                                   0                               5
00(月 01 5                                  0                               6
1111001 S                                  l                               3
0010 0110 s                                극                               2
liii 0l0s                                  10                              l
00100001 S                                 11                              l
0010 0l0is                                 12                              l
0010 0100                                  13                              ]
000100s                                    0                               7
0010 0lUs                                  l                               4
1111 il00s                                 2                               극
1111 1101 S                                4                               D

0000 00100 S                               5                               2
00000010 is                                14                              l
00000011 is                                15                              l
0000001101 S                               16                              l
NOTE1 - The last bit s deno把s the sign of the level, '0 for positive 1' for negative.
NOTE 2- "End of Block" sha끄 not occur as the only code of a block.
      1
          MPEG
174       VIDE0
      ：나      ；




                          표 5-7（겨1속）DCI coefficien朽Tab冶one (MPEG IS: Table B-15)
                  Variahie length code (NOTE)                 nm11                              level
                  1111011s                                    0                                 8
                  1111 l00s                                   0                                 9
                  （刃l000lls                                   0                                 10
                  仗아00010 s                                   0                                 11
                  0010 0000 S                                  l                                5
                  0000 001100 s                               2                                 4
                  00000001 il00s                              3                                 3
                  0000 00010010 s                             4                                 3
                  00000001 lil0s                              6                                 2
                  000000010101 S                              7                                 2
                  00000001 0001 S                             8                                 2
                  00000001 1111 S                             17                                l
                  00000001 l0l0s                              18                                l
                  000000011001 s                              19                                l
                  000000010111 S                              20                                l
                  0000 00010110 s                             21                                l
                  1111 l0l0s                                  0                                 12
                  1111 1011 S                                 0                                 13
                  1111 ill0s                                  0                                 14
                  1111 1111                                   0                                 15
                  00000000 l0ll0s                              l                                6
                  000000001010 is                              l                                7
                  00000000 l0l00s                             2                                 5
                  0000000010011 S                             3                                 4
                  以D0(이刃00 1001 0s                            5                                 3
                  000000001000 is                             9                                 2
                  00000000 i刃00s                               10                               2
                  0000 0000 11111 S                           22                                l
                  00000000 ilil0s                             23                                l
                  000000001110 Is                             24                                l
                  00000000 lli00s                             25                                l
                  0000 0000 il0lls                            26                                l
                  NOTE - The last bit 's' deno妃S the sign of寸比 level, '0' for p玲itive, '1' for negative.
                                                                                           175



         표 5-7（겨1속）DCT coefficients Ta眺 one (MPEG & Table B 而）
Variable length code (NOTE)                       run                             level

0000 00刃 0111 Us                                  0                                16
000000000111 l0s                                  0                                17
000000000lll0l s                                  0                                18
以000 0000 011100 S                                0                                19
00000000011011 S                                  0                                20
000000000110 l0s                                  1)                               21
어000000011001 S                                   (I                              22
0000 0000 0110 00 S                               1)                               23
0000 0000 010! u ls                               0                               24
000000000101 l0s                                  0                               25
00000000010101 S                                  0                               26
0000 0000 010100 S                                0                               27
00000000010011 S                                  0                               28
000000刃0100 l0s                                   0                               29
00000000010001                                    0                               30
00000000010000 s                                  0                               31
0000 0000 0011000 S                               0                               32
000000000010 ills                                 0                               33
0000 어：000010 110s                                0                               34
000000000010 l0ls                                 0                               35
0000 어：)000010 l00s                               0                               36
000000000010011 s                                 1)                              37
0X)(Xn刃 0이0010s                                   1)                              38
0000 0000 0010 001s                               1)                              39
0000 0000 0010 000 S                              (1                              40
0000 0000 00I I I lls                              l                              8
00000000001 1 Il0s                                 l                              9
0000 0000 0011 101 S                               1                               10
000000000011 l00s                                  l                               II
0000 0000 00 11011 S                               1                               12
0000 0000 0011010 S                                l                              13
0000000000110아                                     1                              14
NOTE - The last bit s denotes the sign of the level, '0' for positive, '1' for negative.
176




                 표5-7 (겨I속) DOT coefficients Table one (MPEG IS : Table B -15)
         Variabl이en伊h code (NOT꽈                   fin                            level
         0000 0000 0001 0끄1 s                      l                              15
         000000000刃1 0010s                         l                              16
         000000000001 0001 s                       l                              17
         000000000001 0000s                        l                              18
         0000 0000 0001 0100 s                     6                              3
         0000 000아）(）아 l0l0s                       11                             2
         0000000000011001 s                        12                             2
         0000 000아刃아 1000s                         13                             2
         0000000000010111 s                        14                             2
         0000 0000 00010110 s                      15                             2
         00X只xx刃 (x刃l 이01 S                        16                             2
         000000000001 1111 s                       27                              l
         000000000001 lil0s                        28                              l
         000000000001 il0ls                        29                              l
         000000000001 il00s                        30                              l
         000000000001 1011                         31                              l
         l吼玎E - The last bit낳 deno妃S 山e sign of the level, '0' 的rp（竝five, '1' for negativ已




       표 5-6에서 N町'E2는 non ii出a bi以火의 DC계수어］ 대한 것이고, 다른 계수어씨

      는 모두 NOTE3 부분을 이용, 코딩한다. 또한 위에서 escape에 해당되는 것은

      표 5-6과 5-7에서 해당되는 코드가 없을 때 esca恥코드를 사용한 후 표 5-8과 같

      이 mn과 level을 고정킬이（fixed length) 코드로 따로따로 코딩한다. 즉 다음과 같

      이 코딩한다．

                   escape code ( " 0000 01") + run (6 bits) + signed_level ( 12 bits)
                                                                                                 177



                   표 5-8日兀oding of run and leve나에owing an ESCAPE code
                                 (MPEG IS : Table 8-16)
        flxedl日曜th code      1lln                           fixed length code    signedlevel
        000000               0                              100000000000        reserved
        000001               l                              1000 0000 0001      -2047
        0000 10              2                              1000 0000 0010      -2046


                                                            1111 1111 1111      -
                                                                                     1
                                                            0000 0000 0000      的由idden
                                                            0000 0000 0001      +1
        1111 11              63
                                                            0111 1111 1111      +2047




5.1.2. 억스캔(Inverse Scan)
      이 rever配scan 작업은 QFS[n］인 일차원 DCF겨］수를 scan曲培방법에 따라서 다

    시 2차원으로 바꿔주는 작업이다. 기존어］ 정해진 것은 zig－工ag scan과 alternate

    scan 두 가지가 있고 임의의 scanning방식을 다운로드할 수 있다. inverse scan어］

    의해서 2차원으로 바꾸는 것을 식으로 써보면 아리斟 같다．



                  幻r ( v=0;v8;v卄）

                   幻r( u=0;小8시＋+)

                                  QF[v][uJ = QFS[scan[刻ternate_scan][v][u]I




     alternat乞印an값이         "0" 이면       zig寸zag     scanning을       나타내고,           "1" 이면 alternate
    scam血培을 나타낸다（그림 午31, 4-32 참조）.




5.1.3. 역양자화(Inverse Quc玎）tization)
       Inverse quantization의 과정은 그림 5그와 같다．
      MPEG
178   VIDEO




                                         F伽］
                                           ［기              町日［끼


                           Inverse                             A肛smatch
                         Quantisation        Saturation         Coi如ol
                          Arithmetic




                                        quant_scale_code

                                     刃加］[v][日
                    그림 5-2 Inverse quanilsaflon process (MPEG IS: Figure 7궉)



           윗그림에서 inverse quan由ation은 we培hting mati奴＼V와 qual丑뉴Sc심e_code를 이용

        해서 실제의 DCT꼐수값을 복원하는 작업이며, saturation은 [-2048 : +2047] 이상

        벗어나는 값을 막아 주어 ID口에서 에러가 발생하지 않도록 해주는 작업이다．

        이는 원래 인코딩을 제대로 해주고 채널상에서 에러가 발생하지 않는다면 이렇

          거］ 범위를 넘어가는 경우가 없겠지만 入'IPEG은 디코딩만 규정하고 있기 T대문어］

          어떤 경우라도 대비해서 에러는 나지 않게 하기 위하여 이러한 saturation과정을

          규정한다. 또한 불일치 제어(mismatch contr에도 역시 마찬가지로 MPEG이 디코

          딩만 규정하기 1대문어］ 인코더의 DCF와 디코더의 끄：x7r가 맞지 않는 경우에 어］

        러가 계속 누적되는 컷을 막기 위한 장치이다.



      N       역먕자화 면스／(Inverse quantization a片／hmetic)
              여기서도 intraDC계수와 다른 계수들 간의 처리과정이 다르다．

               (a) In打a DC계수佃effici毗）

                     F"[O][O］는 다음과 같이 구한다．

                                   F"[O][O] = QF[0][O] * intra_dc_mu仕
                 여기서 II血a dc malt는 표 도9와 같이 정해진다．
                                                                                  179



    표． 5-9 R이a加n bets肥en intro_dc_precision and in打（工dc ri피什
                     (MPEG IS : lable7-4)
                  lntra_dcj江由如fi               Bits of preci虹on   I,功U '初 刃zuit

                               0                      8                8
                               l                      9                4
                               2                     10                2
                               3                     11                l




(b) 다른 쳬수들

             이따1 weightii堪m的奴는 4:2:0인 경우는 2가L 4:2:2와 4:4:4인 경우

             는 4개가 있다. 그 종류는 앞에서 설명했듯이 다음과 같다．




   4:
        2:
             0    r
                  Lm   non-intra
                       nn1l日］1l1n}
                       intra
                                   .   (w=
                                             0)
                                             (w=1)
                                             [\




   4:2:2          =m   intra luminance            (w=0)

        or             non-intra luminance (w=1)

  4:4:4                mtra chrominance (w=2)

                       non-intra chrominance              (w=3)



             이It뀨 이 m的奴의 종류를 표시하는 것이 \V[w][vi미에서 加dex w이

             다.    w는 0 부터 3까지의 값을 갖는더1, 그 값과 matrix 종류와의

             관계는 표 5-10에 표시한 바와 같다．
180




                          표 5-10 Seleclion아w (MPEG IS : I야긔e7句
                                                   4:2:0                         4:2:2 and 4:4:4
                                    h!min和114쩍）       由rnm柶귀ng뽀        1i1min1가11i늬＞       (hrn1枾fiance

                                        (cc = 0)           (cc_ 0)       佃＝0)                    (cc_ 0)

                     intra blo出S
                                           0                 0              0                        2
           (macroblock_intra = 1)
                 non寸ritra bbx出S
                                           l                  l              l                       3
           (macrobIo出已intra = 0)




       Quantizer_scal乞code는 정수이고 quanti配r_scale과의 관꼐는 표 5-11과 같다. 이

      두 개의 파라메타를 이용하써 F"[v]［비를 구하는 방법은 다음과 같다．



              F" [v][u] = ((2*QF[vl[ul + k) * W[w][v][u] * quantizer_scale) /32;
                                                                                       '    十，   .




                 , . ..                        10                    (intra blocks)
                여기서                 k     = { . . n，  거． ,. ,, .            . .   , ,
                                              S뇽可QF[
                                             L zgn(1/r   %町町）
                                                       / 1       (7i(Jri'- intra
                                                          711U1) (non             blocks)
                                                                           iri1rq i7L
                                                                         e
                                                                          MPEG
                                                                          미DE0     181
                                                                              H1




표 5-1 ]   R쉬아ion between qu아）撫e乙Sc이e and quantis이sc데e_code
                      (MPEG IS : Table 7亡)
                                   qua1l ser_scale[q느scalejypel
      quantisersca1e_code   q+sca1e_type = 0                 qscale_type =1
              0                                (forbidden)
               l                   2                               l
              2                    4                               2
              3                    6                               3
              4                    8                               4
              5                   10                               5
              6                   12                               6
              7                   14                              7
              8                   16                               8
              9                   18                              10
              10                  20                              12
              11                  22                              14
              12                  24                              16
              13                  26                              18
              14                  28                              20
             15                   30                              22
             16                   32                              24
             17                   34                              28
             18                   36                              32
             19                   38                              36
             20                   40                              40
             21                  42                               44
             22                  44                               48
             23                  46                               52
             24                  48                              56
             25                  50                              64
             26                  52                              72
             27                  54                              80
             28                  56                              88
             29                  58                              96
             30                  60                              104
             31                  62                              112
182




      ft    포화자리 位加仄7灰加）


                                         12047,
                                                                  F
                                                                      "     [v]
                                                                                    [u] > 2047
            F   '
                    [v]
                          [uj   =   1F
                                                   ' '[      F
                                                          vliu]
                                                                          ,-2048드
                                                                                             ' '[   vjtuj
                                                                                                            2047
                                         [-0248, F" tivliu] < -2048



      N     불읠大y 邢어 (I＼俯nc力ch contr이）

            이것은 앞에서도 설명했듯이 encoder의 DCT와 디코더의 Dcc가 맞지않아서

           에러가 꼐속 누적되는 것을 방지하는 것으로 일단 한 블록내의 F［네미의 모든

           계수를 다음과 같이 모두 더해 본다．


                                                                                       v<8   u<8

                                                                          sum=Z Z尸［「［］미v=O   u＝二0




            그후 이 더한 값이 홀수냐 짝수냐에 따라서 조정을 하는더］ 홀수인 경우는 그

           냥 놔두고 짝수인 경우만 다음과 같이 조정한다．



                                                  F[町町 = 尸加／／町和ral/ 川excej玎 U = V = 7
                                                           F' [7][7] if sum is odd
                                                  F／刀／71   F'[ 7][7] - 1 if F' [71[7] is odd
                                                           F' [7][7] + 1 (f F' [7][7] is even                      )   i/sum is even




            이 이유는 원래 DCf는 실수연산으로서 결콰는 정수가 나와야 하는더］ 예를

           들어 DCI된 결과가 （정수 +0.5）가 되는 경우 정세도를 아무리 올려도 반올림

           I대문어］ 1만큼이나 차이가 나는 확률이 1/2 정도나 된다. 그런더］ 이렇게 반올림

           의 방법을 규정하囚 이런 문제를 피하는 것도 가능하지만 H.261에서 위와 같이

           홀수로 만드는 방법을 규정했고 이미 H.261의 칩이 시판되고 있기 때문어］

           MPEG2에서도 이와같은 방법을 취했다. 그래도 불일치（mismatch) 오차가 누적되
                                                                                                        183




    는 것을 막기위해서 MPEG2의 부록 A에서는 P－翊四의 macr的1(乂k이 132번 반복

    되기 전어］ 그 macr的1(乂k을 I-竝四으로 바꿔주는 것을 권하고 있다． 여기서 B-

    竝畔은 콴계없는더］ B－勺I玘은 에러를 누적시키지 않기 때문이다． 역양자화 과정

    을 정리해 보면 다음과 같다．


for (v=0; vd亡旴＋) {
       for (u=0; u8;u-s-+) {
             侄（(u==0) && (i느＝0) && (macn力뇨火j曲비 ) {
                   尸'[v]回 = 加ra_dc_mu!t * Q外回；
              }else{
                   if ( macmbl乂k_intra) {
                         尸'[vi回 = (QF[너回 永 M刈[v]回 水 們i,nise乙韶毗 牛 2) / 32;
                    }else{
                          尸'[v][u] = ( ( ( QFIv][u] * 2) + Sign(QF[v][u])) * W[w][vj[u}
                                                                               非 qu口n九貂兀sc口le ) / 32;
                   }
             }
      }
}
sum = 0;
如r（乍0; v4늑따＋) {
     for (u=O; u<8;u++) {
           if ( F"[vj[u] >2047) {
                  F'[v][uj = 2047;
            }else{
                  if (F"[v][u] <-2048) {
                        F'[v][u] = -2048;
                   }else{
                         F'[v][u] = /7 'h][ii];
                    }
             }
      sum = sum + F'[v][u];
      기피回 = F'n][ii];
       }
}
if ((su九& 1) =0) {
       if ((F[7][7] & 1) !=0) {
              F[7][7] = P[7][7] - 1;
        }else{
              F17][7] = P[7][7] + 1;
       }
}
184




      5.1.4. 억 DCT(Inverse DOD
            Inverse DC1'는 다음 식에 의해서 행해진다. 이 IDCT된 결과는 9b如로 표시되

          고 범위는 卜256 : 255］이다. 물론 skipped macroblock어］서는 IDCT결콰는 모두 0이

         되어야 한다
              （ 강제적 setting 방법 동원）.

                                                                   m2向
                        n
                        t                                                                       \              (.            (2x+ 1)uK   , (2 y + 1)v 刀
                                                                   2eN                      (.)C(,
                                                                                               =
                                                                                                                                ,
                                                                                                                    ,,)..,
                                             V
                                                                                                          )F
                                                                                 IC
                                                                            N-
                                                                                 山
                                             /
                                                                                                                                乙 J시              乙l 거




                  with                                    u, v, x, y= O, l, 2, ...N-l
                  where                                   x, y are spatial coordinates in the sample domain
                          u, v are coordinates in the transform domain
                  .( ,           1
                                      for u,v= 0
                                                                       1
                                                              )=
                                 ),.(,
                  C(u) C(v)              ,                         =

                                 l     otherwise                       t.
            참고적으로 入4PEG의 부록어］ 나와 있는 NxN 블록 DCT는 다음과 같다．

            「「？
              F   (u,
                  （         v)     )＝            =   -
                                                     급.   -         (O).(? x i。 N-
                                                                   C(u)C(v)     y。 f(x,y) cos (2x+
                                                                                      )N-        2N1)u r cos8
                                                                                                   i佃m8                                    (2y+    2N
                                                                                                                                                    l)   v
  5.2. 움직임 보상
            움직임 보상작업은 그림 5-3과 같다. 이 작업은 기존의 반화소단위의 움직임

          보상작업과 같지만 MPEG2에서는 dual巾rime이 들어가는 것이 차이점이다． 그

          외 入4PEG2에서는 field단위 또는 fran妃단위의 움직임 보상이 가능하다. 따라서

          丘eld picture에서는 field prediction을 하고 fran叱 pictt配에서는 frame prediction이나

          field prediction                                             두 가지를 이용할 수 있다.                                              Sin叩le丘ame pre小ction에서는 16X 16

          macrob!어火당 P勺pe어］서는 1개의 motion vector가，B-翊畔에서는 如rward, backward

          두 개의 motion vector가 필요하다. 또한 단순한 field prediction인 경우는 16X16

          macr面li乂k당 P-tx四에서는 t아）, 比ttom 두 field로부터 각각 하나씩 두개，B-翊四의

          경우는 幻p, bottom, backward, forward까지 도합 4개의 n刃tion ye야or가 필요하다．
                                                                                                                  185




                   Prediction
                                         Fram朗tore
                  Field下rame
                                         Addressing                    Framesto
                    Selection

                      vect口,fr][s]［日      A
                                    \..h.

                  Additional              Scaling                      Half-pel
                  Dual-Prime             for Colour                   Prediction
                  Ar咐irnetic            Uomponents                     Filtering

                      A             vectol[r][s][t]


                                             Hal卜Pel
                    Vector                                             Combine
   下：                                           Info
                   Decoding                                           Predictions
         뗀U
                  土
  " ' "' " " 帥J

                                                             d " '/

                                                       風川키                '         H
                                                                                    口
                                                                                                                      d

                                                                                    Hm늉늉m
                                                                                                            D P
                                                                                    O
                                                                                                                  e
                                Vector                                                                            0
                                                                                                                  d
                                                                                                                  d
                                                                                            1111t1111
                                                                                                        r
                                Predictors


                                                                                                        曲   工


       그림 5-3Sirr耳獅ed mo枷＞n compens（카ion process (MPEG IS: Fig내e7句



 또한 MPEG2에서는 field picture에서 16怒 predict幻n mode를, P-picture에서 dual

prime mode를 규정하고 있는더I dual_prime에서는 송신측에서 하나의 motion

vect아와 하나의 differential n奴ion v凹恤를 보내고                                  decoder에서 이것을 이용하여

도합 4개의            的rward motion vect야를 계산해 낸다. 이 n均de는 P-I丘cture에서만 이

용한다. 이는 뒤에서 자세히 설명된다. 16x8 pre小ction mode는 하나의 field picture

에서의 16x16 macr的lock을 그림 5-4와 같이 아래위의 16X8블록으로 나누어서

아래위 각각의 블록어］ 대해서 1개씩의 motion ye야or를 전송한다.                                                   이와같이 하

는 이유는 field picture에서의 vertical distance는 frame picture에서의 두 배이므로

16X16 macr아加ck을 그냥 움직임 보상하기에는 수직축 길이가 너무 킬어서 움

직임 보상이 제대로 되지 않는 경우가 생기기 때문이다．
186




                 /
                                            虹       M
                 /
                 /
                 +
                                                                     16




                                                                     16


                                       그림 5-4 l6x8 predicflon mode



             이제 그림 5-3의 각 블록을 차례대로 설명하면 다음과 같다．




      5.2.1 . 다ed匕tion fi이d와 的me 선택（selec作＞n)
        I    尸ek力 'redk刃幻n

             앞에서도 언급했듯이 field prediction은 field picture나 frame picture에서 모두 이

            용될 수 있기 때문에 이제부터 언급되는 top이나 比ttom field는 각 field라도 되

            고 한 frame 내에서의 top field나 比仗om fle녑를 가리킬 수도 있다. 또한 아래의

            first나 second field라는 것은 디스플레이되는 순서태로 앞의 것이 first, 뒤의 것이

            second field이다. 그런더］ MPEG2에서는 바로 그 field가                 的p인가 bottom인가를

            지정하게 되어 있기 때문어］ 꼭 first field가 top field로 된다는 보장은 없다. 결론

            적으로 지적하고 싶은 것은 入4PEG에서의 field prediction은 가장 최근어］ 복원된

            field들에 의해서 행해진다는 것이다．



             (a) P-picture어］A- 의 field prediction

               1) frame picture어］서 field별로 예측하는 경우

                그림 5-5와 같이 전 frame의 top이나 比ttom field로부터 예측한다．
                                                            187




                                 Possible
                               Intervening
                                B巾ictures
                             (Not yet decoded)
      그림 5-5다edic化n ofthefi田t field predic加nina什ame이C十ure
                     (MPEG IS :日（)ure 7句



2) fie닢picture에서 field별로 예측하는 경우

 i) first field를 예측하는 경우

   이 경우는 그림 도5와 동일하다．



 ii) second field를 예측하는 경우

   이 경우는 그림 5-6, 그림 5-7과 같이 2가지로 나뉜다. 그림 5-6은 second

   field가 比ttom field인 경우이고 그림 5-7은 second field가 幻p field인 경우이

   다. 이 두 개의 그림은 언뜻 보면 잘 이하까 안 되지만 기본적인 원칙은

   같다. 즉 움직임 예측을 가장 최근에 복원된 field                2개로부터 한다는 것

   이다． 그림 三6에서는 first field와 second fie닢가 的P－比如m의 순서인 경우

   이다. 그런데 first field와 second field의 순서가 比ttom-t叩인 경우에서는 그

   림5-8과 같이 孝4 field를 디코딩하려고 할따1 가장 최근어］ 복원된 field 2개

   는 韋2와 粥 field이다. 그림 5-7어］ 나타난 2개의 field가 바로 이 韋2, 彦3 field

   이다．
188




                                   Possible
                                 Intervening
                                  B-pictures
                              (Not yet decoded)
      그림 5-6다e네cflon 아the second fi이d下)icture '巾en it is卄）e bo卄om field
                          (MPEG IS : 日gure 7刃




                                   Intervening
                                    B-pictures
                                 (Not yet decoded)
       그림 5-7 Predk새on 아The second fleld-pic仙re 낚小en 什 is the t＞口 field
                          (MPEG IS :日gure 7的



                          전 frame        현 打게ne

                        bottom - top    bottom - top

                          孝1    舵        韋3     孝4

                                                     티스플레이 순서

                                    그림 5-8
                                                                                            189




     (b) B-picture어］서의 field prediction

                  B-picture에서는 frame prediction 또는 field prediction을 쓸 수 있다. 그러나

                  움직임 추정은 그림 5-9와 같이 항상 가장 최근어］ 복원된 "丘ame" 2개로

                  부터 한다. 위의 그림 三6이나 그림 5-7과 같은 방법은 이용하지 않는다

                 （원래 B肛cti.此를 "reference'로 쓰는 일은 없다．).




                                     C                            ( )
                  T叩                                                              (    Top \
               Reference                                                            Reference 1
                                                                                 戶j
                 Field                                                            \. Field /

     (Bottom
                                                                                     Bottom
     I Reference                                                                    Reference
      \＼느 Fi    /  eld
                         ./
                         .
                                                                                      Field
                                       Possible                      Possible
                                      Intervening                     Intervening
                                       B-pictures                      B-pictures
                                  (Already decoded)                 (Not yet decoded)
                              그림 5-9 Fiek抑)redk加n of B fiek캬긔cturE羚or B f띠me口ctures
                                                  (MPEG IS : 日gure 7功



N       Fr（그／7)e r砂추

      이때의 frame prediction에서도 reference frame이 2개의 field picture로 이루어졌

    든 하나의 fra끄配picture로 이루어졌든 상관이 없다．



               (a) P-picture어］서의 frame prediction

                   그림 5-10과 같이 가장 최근어］ 복원된 丘ame 1개로부터 행해진다．
190




                    /1                                         /r1
                         Reference
                          Frame
                    ＼뇨           /            \\b     ./       ＼뇨          /
                                              Possible
                                            Intervening
                                             B-pictures
                                          (Not yet decoded)
                   그림 5-10다an）今pied匕flon幻ri下永寸ures and Pj：北仙res
                               (MPE（引S :日gure 7-10)



            (b) B-pictui洲서의 fran配prediction

              그림 5-11과 같이 가장 최근어］ 복원된 丘an叱2개로부터 행해진다．




           느）
                            /r        \                                           /11\
                                                                                         Reference
                                                                                          Frame
                                                                     ＼뇨   J       ＼뇨             /
                                Possible                          Possible
                              Intervening                       Intervening
                               B-pictures                        B-pictures
                          (Already decoded)                   (Not yet decoded)
                그림 5-1 ] Fr酊）今pred비on 幻r 먀ycture (MPE（引S : 日（7ure 7-1 ])




      5.2.2. Frame 메모리에의 저장（F띠mestore addressin助
          fra끄配m아I均ry를 억세스하기 위한 부분으로 하드웨어와 관련된 부분이기 때문

         어］ 표준에서는 언급이 없다．
                                                                                                         191



5.2.3.卜爪쇄on vect아 디코딩
    入4otion ye아or는 한 macr的뇨火당 최대 4개까지 나올 수 있는더］ 이를 그냥 보

   내면 너무 bit량이 많으므로 바로 전 m批ro뱌乂k의 motion ye아or와의 차이만을

   VLC 코딩하여 전송한다.                         MPEG에서는 이 차이를 구하기 위해서 이전

   ma的1(兀k의 motion ye아야값을                    motion vector predictor어］ 저장하는데                        이 값을

   PMV[r][s]［下｝ 표시한다. 즉 I爪4V의 값은 바로 이전                                    macr小1(乂k의 m아ion vector

   가 되고        encoder에서 코딩하는 값은 vector[rJ[s][tJ - I小4V[r］同띠가 된다. 여기서

   r,s,t의 의미는 표 5-12과 같다.


       표 5-12卜月eanning of indice引n 아,IV(r) (s) (此 vecto巾 (s) (t) and vector(r) (s) (t)
                                (MPEG IS : Table 7-7)
                                      0                                             1
           r          F小tn均tion vec的r m Ma口oblock                  Second motion vector in Macmblock
           S               Forward m야幻n Vector                           Back＼자ardsmot幻ri Vector
                           Horizontal Component                             Vertical Component

    N아e:          r 汕to takes 仕比 values 2 and 3 的rderi比d mo由nv帥ors used w捉h dua印血ne 畔如t由n.
                  Since these motion vecto心 are derived they do not themselves have motion vec幻r predictors.




    이 motion ye야아의 차이를 이 책에서 DMV라 정의한다. 이 DMV를 디코딩하

   는 방법을 설명하는 것보다는 인코딩하는 방법을 설명하는 것이 훨씬 더 쉽게

   이해할 수 있기 1대문어］ 먼저 부호화과정을 설명한 후 복호과정을 설명하기로

   하겠다. 인코더에서 움직임 추정을 할 때는 먼저 m아ion vect아를 구해야 한다．

   보통은 b1乂k matching 방법을 이용하는더］ 이러한 방법을 위해서는 미리 탐색영

   역（search r出ige）을 정해야 한다. 이러한 탐색영역을 인코더에서는 f_code로 디코

   더에 알려주며 decoder는 이 fc어扼만 보면 표 5-13과 같은 탐색영역을 알아낼

   수 있다.
192




            표． 5-13 Allo＼사야긔en）에（)n vect아 range as a funcflon of f_code(s) (t)
                                 (MPEG IS : Table 7的
                                 Vertical c月llponents (l=1) of
                   f_co毗［s][t]   丘eld ve出)rs in frame pictui心             A끄 other cas心
                            0                              伽thidden)
                            l                나：+3,5]                         [-8: +7,51
                            2               卜8: +7,5]                       [-16: +15,5]
                            3               [-16: +15,5]                    [-32: +31,5]
                            4               [-32: +31,5]                    [-64: +63,5]
                            5               [-64: +63,5]                   [-128: +127,5]
                            6              [-128: +127,5]                  [-256: +255,51
                            7              [-256: +255,5]                  [-512: +511,51
                            8             卜512: +511,5]                   [-1024: +1023,5]
                            9            [-1024: +1023,5]                 [-2048: +2047司
                        10-15                                (reseived)




       이 표에 나타나 있는 영역은 반화소단위로 표시한 것이며 이를 정수화하기

      위해서는 이 영역에 2를 곱하면 된다 ．인코딩은 이렇게 2를 곱해서 정수로 만

      든 후에 하게 된다. 다음에 설명하는 인코딩과정에서는 수평축의 motion vector

      에 대해서만 설명하도록 하겠다 ．예를 들어 f_code가 1인 경우의 최대 변위인

      址gh는 15가되고 최소 변위 low =-16이 된다. 따라서 탐색영역 range = 32가 된다

      (0까지 포함해서）. 이때 DMV는 卜31,+31]의 영역에 있게 된다. 이 MV는 f변수

      （뒤에 설명함）로 나누었을 때 몫어］ 해당히는 n均tio兀C(넜e와 나머지어］ 해당하는

      motion_residual로 나누어서 코딩하게 되는더I f_ct넜e가                             1인 경우는 f=1 이기 I대1

      문어］ moti이1_residual은 없고 mo如nc어妃만 있게 된다.                              이 mo如n_code는 표 5-

      14로 전송하는더］ 이 VLC table은 -16부터 +16까지의 값밖에 없으므로 [-31 : +31]

      범위를 卜16: 15] 범위로 좁혀서 만들 수 있어야 한다. 따라서 위의 [-31 : +31]까

      지의 값 중 [-16: +15］까지의 값은 그냥 그 값을 mo如n_code로 하고 [-31:-17］까

      지의 값은 range값 32를 더해서 [1 : 15］으로 만든 후 그 값을 motion _code로 한

      다. 또 [16: 31]까지의 값은 range값 32를 빼서 [-16: -1］까지의 값으로 만든 후

      그 값을 motion下어妃로 한다.              이렇게 [-16 : +15] 사이의 값으로 조정된 값을
                                                  MPEG
                                                  VIDE0   193




delta라 한다. 위와 같이 delta를 [-16: +15］까지 강제적으로 만들면 디코더에서 진

짜 motion vector 차이인 DMV를 어떻게 알 수 있나 생각하겠지만 이것은 명확

히 구분된다.     Decoder에서는 위에서 구해진 [-16: 15］까지의 delta를 PMV에 더

하게 되는더］ 이때      delta+ PMV값을 살펴보자. 여기서 v는 motion ye아아를 나타

낸다．



   1) DM\／가 [-16 :+15］인 경우

        d이怡 + PMV = V = PMV + PMV = V

      따라서 이 경우 -16 톺 delta + PMV 各15（왜냐하면 -16 드 v 드 15 이므로）

      이 되고 delta + PMV = v 가 된다．



   2) D入'I\／가 [-31 :-17］인 경우

        delta + PMV = v 느 PMV +32 + PMV = v +32

      따라서 이 경우 16 드 delta + PMV 드 47이 되고 delta + I小4V가 16 이상

      이 되며 이 경우 delta + PM\／에서 32를 빼줘야 원래의 ff0如n妃ct아인 V

      를 얻을 수 있다는 것을 알 수 있다．



   3) DMV가 [ 16: 31］인 경우

        delta+ PMV= v- PMV-32+ PMV= v-32

      따라서 이 경우 delta + PMV는 [ -48 : -17］까지의 값을 가지며 이 경우

      delta + PMV에 32를 더해줘야 원래의 motion ye야or인 V를 얻을 수 있다．
194




      표5-14 Variable length codes for motion_code (MPEG IS: Table B-b )
                   Variable length code   mot如n_code(r][s][t]

                  어0000011001             -16
                   00000011011            -15
                   00000011 101           -14
                   00000011111            -13
                   0000 0100001           -12
                   00000100011            -11
                   0000010011             -10
                   0000010101                  9
                   00000101 11            -8
                   0000 0111                   7
                   0000 iC刃l              -6
                   0000 1011                   5
                  어000111                 -4
                   00011                  -3
                  0(기 l                   -2
                  011                          l
                   l                      0
                  010                     l
                  0010                    2
                  （刃01 0                  3
                  0000 110                4
                  어00 1010                5
                  어刃0 1000                6
                  어刃00110                 7
                  00000101 10             8
                  0X刃 0101 以0             9
                  0000010010              10
                  00000100010             11
                  0000 0100 000           12
                  00000011 110            13
                  00000011 100            14
                  00000011 010            15
                  00000011 000            16
                                                                 195




  예를 들어 v= 14이고 PMV= -16인 경우 DMV= 30이 되며 delta = -2가 된다．

따라서    decoder어］서의   delta +PMV =-18이 된다. 그런데 이 값이 low(= -16）보
다 작으므로 32름 더해서 원래 ye아아값 14L= -18 +32）를 복원할 수 있다．

 Moti이residu싶을 설명하기 위해서 f_code가 2인 경우를 살펴본다. f 변수값

은 (1 <<(f_code -1)）로 구한다. 따라서 bma玎로       " 10''이 되며 f= 2가 된다（예를
들어 f_code가 4면 f= ' 1000" 즉 f= 8이 된다）. 이띠1 high = (16米f) -l =31이며 low

= (16*f) = -32이다. 또한 range = (32均＝64가 된다. 따라서 DMV는 [-63 : 63］의

범위에 있게된다. 이것을 앞에서 설명한 방법을 이용하囚                      [ low : high］범위값
즉 [-32 : 31］까지의 범위값（= delta）으로 만든다. 그러나 표5-14의           motion _code
VLC table은 [-16: 16］까지의 값이므로 [-32: 31］까지의 delta값을 f를 이용해서

[ -16 : 15 ] 범위의 몫어］ 해당하는       motion_code 부분과    나머지에 해딩方｝는
motion叫residual 부분으로 다시 나눈다. 나누는 방법은 다음과 같다.

     1) delta가 0이면 motion_code는 무조건 0이다.

     2) delta가 0이 아니면 음수는 부호를 1덴 후 1을 빼고 양수는 그대로 1을

       뺀다. 그러면 양수는 [0: 30］의 범위에 있고 음수는 [0 : 31］의 범위에

       있게 된다.     그 후에 f값인 2로 나눠주거］ 된다. 2로 나누면 몫은 [0:

       15］의 범위에, 나머지는 0 또는 1이 된다. 이렇게 l을 빼는 이유는 나

       머지가 1부터 시작하는 것보다 0부터 시작해서 010101. . .이 나오게끔

       하는 이유도 있고 하드웨어적으로 음수는 2's c아nplement로 표시하는데

       이를 부호를 떼고 양수로 만드는 과정에서                다시    2's complement를 취
       해야 하므로 이II뀨 1을 아여］ 빼버리면 단지 bit幻gg血평만 하면 되므로

       편리하1 진다.      이렇게 구한 몫은 [0: 15］이므로 몫이 0인 경우 원래

      delta가 0인 경우와 구별이 되지 않는다. 즉 원래               delta가 0이라서 몫
      이 0인지 delta가 +d,+-2라서 몫이 0인지는 나머지를 봐야 알게 되며

      더욱이 delta가 +-l인 경우는 위에서 부호를 떼고 1을 빼는 과정에서

      그 값도 0이 되므로 delta가 원래 0인 경우 구분을 할 수 없게 된다．

      따라서 위에서 구한 몫에 l을 더해서 [ 1: 16］까지로 올린후에 다시 원
196




             래의 부호를 붙여서 이를 mo如n困le라 하고 표 5-14를 이용하써

             VLC 코딩한다. 표 5－나에서 +16에 대한 C에e가 있는 것도 이 때문이

             다. 또한 motion_res恤ial은 나머지에 해당하는 부분인데 여기서는 0과

             l이 된다. 따라서 ibit이면 충분히 보낼 수 있다. 이 motion뇨 residual은

             고정길이      코딩（fixed   length   coding）을   한다.   즉   f를   구하면

             motion residual이 몇 bit로 전송되는지를 알 수 있다. 이와 같이 delta가

             0인 경우와 0이 아닌 경우를 분리해서 코딩하는 것은 JPEG과 MPEG1

             에서도 볼 수 있는더］ delta가 0인 경우와 아닌 경우를 나누어 생각하

             는 더］에서 출발한 것이다．



       Motion vect아의 수는 엄청나게 많으며 이를 직접 코딩하는 ＼兀C table을 만들

      수는 없다. 따라서 그룹으로 나누어야 하는더］ 보통 motion vector들을 살펴보면

      어떤 picture에서는 물체의 움직임들이 커서 motion ye心or값이 대체로 크고 어

      떤 pictt끄e에서는 움직임이 작아서 motion vect야들이 작거］ 된다. 따라서 그

      picture의 motion ye야아들의 크기에 맞게 어떤 값（여기서는 f 값）으로 나누어주면

      그 몫 중에서 특히 많小발생하는 값이 있게 되는더］ 이들 분포는 거의 비슷하

      므로 같은 ＼兀C table을 이용해서 코딩하면 효율적일 수 있다. 그러나 나머지는

      불규칙하며 따라서 VLC 코딩하지 않고 f 값어］ 따라 고정길이 코딩을 한다. 즉

      f=2이면 motion_residual을 ibit로 코딩하고 f=3이면 motion_residual은 2bits. . . 등

      등으로 코딩된다. 따라서 motion resi(加al은 그I대 그때의                bit수를 계산하PAl

      bitstream에서 뽑아 쓰면 된다. 결과적으로 delta, vec加r[r][sIt], PMV[r][s] 띠는 모두

      口ow : high］영역어］ 있게 된다．

       이제 복호과정을 생각해1 본다. 이 복호과정은 지금까지의 역과정으로, 프로그

      래밍 언어로 나타내면 다음과 같다. 여기서의 변수는 앞에서 사용했던 변수들

      과 동일하다. 먼저 인코딩과정에서 했던 것처럼 r針ze, f, high, low, range 등과 같

      은 변수값을 구한다. 그 후 mo如n띠妃가 0이거나 f=1이면 delta를 motion뇨C어le
                                                                                      197




로 하고 그렇지 않으면 앞에서의 과정의 역순으로 delta를 구한다. 그 후 delta가

mw:high］영역 밖에 있으면 delta에서 range를 더하거나 빼서 값을 조정한다．


      r_size = f_code囹[t] -1
      f= 1ozr size
      세gh = ( 16사）- 1;
      l에= (( 16)*f);
      range =(32*t);

      if ((f = 1)Il( rnotion_code[r][s][t] = 0)
             de恒 = n杓如n cc由떼테寸
      else {
               delta = (( Ab히m的（가'cc져可r][司［小 1)*f) + Ii｝에onHre섧dua巾][s][t] + 1;
               作（m얘에下여印[s坰 < 0)
                    delta = -이ta;
           }
     prediction = PMV[rl[s][t];
     if ( (mv_format = 坪回d") && (t=1) && (pi才Ure_structure = "Frame picture"))    pred七伽Dn
= PMV[r][鉦t] 미V2;

      vector'[r][s][t] = prediction + de卄a;
      if ( vector'[r][s][t] <low)
           vector'[r][s][t] = vec幻r[r][s][t] + range;
      if ( vector'[r][s][t] > high)
           ye（加r[r]同띠 = vecto巾］Es]［小 range;
      什（(my幻miat =섀e뇌') &&(t=＝너）&＆佃cture_stnjcture =" 日'ame pk支ur甘');             PMV띠b批］
= vector[r][s][tr2;
      else
           PMV[r][s][t] = vector[r][s][t];



  Mv1如m切t은 표 5-16, 표 5-17에서 구할 수 있다. 여기서 frame picture에서

field prediction을 할 따1 vertical con叩onent의 값을 2로 나누었다가 후에 원상타匠

2를 곱하1 주며 새로운 motion vector yEnl司띠가 구해지면 그 값을 PMV[r][s]띠에

대입해서 motion vect야pred奴야값을 갱신하게 된다. 이 PMV田同띠값은 r, s, t 값

에 따라서 8개가 되는더］ sequence중간에서는 LPB拉山re들이 번갈아 나올 수

있으므로 이 8개가 항상 전송되지는 않는다. 따라서 이 전송되지 않은 I爪lv들

은 어떤 법칙을 세워서 갱신을 시켜주든가 또는 이 I呱IV값들을 모두 reset시켜

주든가 해야 하는더1 이에 대해서는 다음의 ye乂：tor predictors 부분에서 설명한다．
      MPEG
198   니DEC




                    표5-15 Meanning of frame_motion_lype (MPEG IS : Table 6-17)
          code      spatial temporal        predict沁iity比     motion vector    mY format   dmv

                      weight_clai心                                count

             00                                reserved

             01               0,1             Field-based              7          field     0
             01                2,3            Field-based              l          field     0

              10         0,1,2,3             Frame-based               l         frame      0

              11              0,2,3           Du出下rime                 l          field         l




                      표 5-16 Me（그nning of field_motion巾ty'口e (MPEGIS : T（火)1e6-恪）
         code      spatk止te叫NM川            prediction type   motion vector    my 白I-n咀t    dmv

                     weight_class                               （刃unt

         (X)                                  reserved

          01             0,
                               1             Field-based           1            field       0

                         0,1                  16x8 MC              7            field       0
          10
          11                  0              Du寸P由Tie              l             fi이d       l




             Field picture와           fra끄ne picture에서의 예측과 전송되는 motion vect야를 살펴보면

        각각 표 5-17과 표 5-18과 같다
                                                                                                                             199



                                     표 5-17 다edic거on amd m아ion vectors in field 口ctures
                                                  (MPEG IS Table 7-13)
   field                                               macro-
  motion             macroblock motion -               block -
    t1．꾸e           白rward          backward            intra             Motion ve出才      Prediction formed for

Fieldhased牛                                                1         vecto,1[0}[0][l:0]X   None (mo如n        vector     is   如r
                                                                                           conce拙rnent)
Field-based              l               l                0          vector'[O][0][1:0]    whole field, forward
                                                                     vector'[O][l][l:OJ    whole field, backward
Field-based              l               0                0          vector'[O][O][l:O]    whole 丘eld, 如rward
Field-based             0                                 0          vecto,'[O][l][l:O]    whole field, backward

Field-basedt            0                0                0          vec切40][OI[1:0］蜂      whole field, forward

l6x8MC                  l                l                0          1坦（크or'{O][O][l:O]    upper 16x8 field, forward
                                                                     vec幻nm0][L이           lower 16x8 field, forward
                                                                     vector'[O][l][l:O]    upper 16x8 丘1日d, backw出xl
                                                                     vec勿7乍皿皿：0]           lower 16x8 field, backward
16x8MC                   l               0                0          rector'[O][O][l:O]    up比r 16x8 field, forward
                                                                     vecto4l][0][1:0]      lower 16x8 field, forward
16x8MC                  0                l                0          vector'[O][l][l:O]    up比r 16x8 field, backward
                                                                     vectoi'[1][1][1:0}    lower 16x8 field, backward
Du띠 1가Tie                1               0                0          vector'[O][O][l:O]    whole field, fmm S쾨I妃 p缸ity,
                                                                                           forward

                                                                     vecto尸［2][0][l:0］싸    whole field, 血m opposite parity,
                                                                                           如rward
Note:         Motion vectors are listed in the order they appear in the bitstream

           X the motion vector is only present if conceahnent_motion_vectors is one

           聿 f녑也mofi（月山I比isn啣螂ent in小eb油帥but is assum叱to he Field-based

           * These motion vectors are not present in the bi臼tream

        中 These motion vecto心are derived如m vect까'田］[0]［쌔as desc네晦1in7.63.6

           蚤 The motion vec幻r is切ken幻be (zem, z的as exp岫1的in 7.6.3.5.
200




                                  표 5-18 P尼dic州on and motion vect이引n 依그me 口ctures
                                                (MPEG IS : I야兆 工14)


                        macroblock motion -
                       forward       backward                      Moti（月lve幻r             Prediction fonned for

  Frame-basedt                                            l        vector'[O][O][l:of<     None (motion          vector   is   for
                                                                                           conce拙ment)
  Frame七ased               l               l              0        vector'[O][O][l:O]      frame, forward
                                                                   vector'[O][l][l:O]      frame, backward
  Fr끄ne-based              l              0               0        vector'[O][O][l:O]      frame, forward
  Frame-based              0              l               0        vector'[O][lJ[l:O]      framae, backward

  Fran妃－t日sed聿             0              0               0        vecto尸[0][0][1:O]*      frame, forward

  Field-based              l               l              0        vecto,'[O][OJ[l:O}      top field, forward
                                                                   1坦ct刃／[1][0][l:0]       bottom field, forward
                                                                   vecto40][l][1:0]        的p field, backward
                                                                   vector'[l][l][l:O]      bottom field, backward
  Fi이d-based               l              0               0        vecto40][0][1:0]        top field, forward
                                                                   vector'[l] [O][l :0]    比的m field, 的iward
  Field-based              0               l              0        vector'[O][l][l :0]     top field, backward
                                                                   vector'[l][l][l:O]      bottom field, backward
  Dual prime               l              0               0        vector'[O][O][l :0]     top field, 加m same 凹ity, for吼iii
                                                                   vector'[O][O][l:O]      bottom field, fmm same parity,
                                                                                           for＼入／a工xi

                                                                   vecn）尸［2][0][1:0］싸      top field, fmm opposit已 parity,
                                                                                           向rward

                                                                   vector[3][0][1:O]*t     b乂幻m field, from opposite parity,
                                                                                           白rward
                M的on vec幻Is 毗 lis妃曲i the order毗y appear in the bitst叱am

                the mot由fl vec幻ris only 口tsent if c月1侊ala目也mofion_vec加rs is one

                framne_motion_type is not伊sent in the bitstream but is assumed to be Frame-based

                These motion vectors art not present in the bitstream

                These motion vecto心 are derived 丘Om vector'[O][OI[l:O] as described in 7.63.6

                The mc比由n vec奴is 姚en 的 比 (zero, 配向 as explaine的x7.的．5
                                                                                                                       201




 5.2.4. 벡타예측기（Vect이Pre네ct아s)
                 앞 절에서도 설명했듯이 이 vec的r predi比ors는 전 macr小lock의 n均tion vect아값

        PMV를 저장하고 있는 곳이며 총 4개의 pred奴아가 있다. vertical, horiz呱al

            component까지 따지면 8개의 값이 있는뎨 마Ima的뇨永당 8개가 항상 이용되지

            않으므로 빠진 부분은 어떤 법칙을 세워서 갱신을 해주어야 한다. 또 어떤 더］

            에서는 완전히 리셋을 해주어야 하는 부분도 있는뎨 이를 살펴보면 다음과 같

            다．
        M        m에On vec幻rpre아bt아의 갱잔방뼙

                 각 경우어］ 대해서 표 5-19와 5-20과 같이 갱신한다．


                             표 5-19Upd아ing of molion＼爬1<寸O나)redict(兆 in 的me pictures
                                              (MPEG S: T的le 工9)
  frame motion -                  macr出lock motion -            macroblock -

        type                    forward         backward             hitra          Predictors to Update

Fram三‘basedt                                                           l            PMV{1][0][1:0] = PMV[0][0][1:of<
Fran好based                          l                l                 0           ／꺼IV[11[0][1:0] = 尸冗IV[0][0][1:0]
                                                                                    PMV[1][1][1:0] =PMV[0][1][1:0]
Frame-based                         l                0                 0            PMVI1][0][1:0] = PMVI0][0][1:0]
Frame-based                        0                 l                 0            PMV[1][1][1:0] = PMV[0][1][1:0]

Frame-based享                       0                 0                 0            PMV[r][s][1] = 0g
Field-based                         l                l                 0            (none)
Field-based                         l                0                 0            (none)
Field-based                        0                 l                 0            (none)
Dual prime                          l                0                 0            PMV[1][0][1:0] = PMV[0][0][1:0]
Note:            PMV[r][s][1:0] = PMV[u][v] 1:0] means that;
                            PMV[r][s][1] = PMV[u][v][1] and PMVlr][s][0] = PMV[u][v][0]

        )( 珏 concealmlent_motion_vectors is zero then PMV[r][s][t] is set to zero (for all r, sand t).

        土 frame_motion_type is not present in the bitstream but is assumed to be Frame-based

        효 (Only心呻inP肛C毗）尸MV帥l小s set to zero (for曲，sand t). See 7.6.3.4
202




                              표 5-20 Upda거ng of mo札n vector pre（계cto四 infi이d pictures
                                              (MPEG IS : Table 7-10)
      field n札lion -              macroblock motion -          macroblock -
          type               知rward           backward             inti묘         Predictors to Update

 Fie1d,based未                                                        l           PMV[1][0][1:0I = PMVE0I[0][1:0?<
 Field-based                       l              l                  0           PMV[1I[01[l:01= PMVI0][0][1:0]
                                                                                 PMV[1][1It1:0] = PMVI0][l][l:0I
 Fiel小切sed                         l              0                  0           PMVI1][0][l:0] = PMV[0][0][1:0}
 Field-based                       0              l                  0           PMV[1][1I[1:0] = P才V[0I[1J[1:0}

 Fie1d-based聿                      0              0                  0           PMV[r][sJ[t]印蚤

 16x8MC                            l              l                  0           (none)
 16x8MC                            l              0                  0           (none)
 16x8MC                            0              l                  0           (none)
 Dual pi土［l妃                       l              0                  0           PM141][0][1:0J = PMVI0J[0][l:0]
 Note:         PMV[rl[s][l:0] =PMV[u][v][ :0] meansthat;
                          PMV[r][s][1] = PMV[u][v][l] and PMV[rj[s][01= PMV[u][v][0]

           )< If col毗吐nenLm心on寸ye巾心iszemth口l尸MVIrI[s][t} is set t끄跏(f아al나, sand t).

           聿 II叫幻枷呱lq跏no냐肥sent in山ebitstream but is assur油tot小配based

           효 (Only毗呻inP們毗川M14r伽川呼山zero（缸曲，san由小cc 7.6.3.4




          N      mo／幻n vec幻r尸m寸C／아의 리셋방뼙

                 다음 같은 경우어］ PMV값을 0으로 리셋한다．

                       - slice의        시작에서

                       - concealment motion vectol를 갖지 않는 in打a macroblock마다

                       - macro바姚_motion加rward가 0인 P-picture의 non-intra macrobk乂k에서

                       - P-picture어］서 macr아丑ock이 skip될 때
                                                                                          203




5.2.5. 추가 Du이 prime 계산（Arithmetic)
       Du出 伊ime prediction은 P-picture에서만 쓰이는더Ivec的라O][O][1:O］와 dr四ect아로

   부터 한 field당 motion vec奴 2개씩, 쇼ame당 도합 4개의 motion vect야를 구하는

   것이다． 여기서 편의상 pa血y라는 말을 쓰게 되는더］ 이는 &id를 구분하기 위한

   것으로 啣 叱가 parity 0, 比tt呻飼d가 p .ty l이 된다．

                                  v[21[01[0:11
                            -lx                           Deny叱 Vectors
                          .05 1         -lx                      0
                           ox          皿5 勿
                                                                      v[3][0][0:1]




                                   ／升 卑
                          35 m=-                                         Field Vector
                                          3X
                                                                         from bitstream
                           4            3,5 難
                          4,5 移          4X                     0
                                        4.5 好
                            Top          Bottom     Top       Bottom
                            Reference Pict出e          Picture Being
                                                       Predicted
              그림 5-12 Scalingofm에on vectors for du（거F川me pre계ction
                             (MPEG IS : Figure 7-12)



       그림 5-12는 dual prime에서 2개의 vectos를 계산하1 내는 과정을 그림으로 설명

   한 것이다. 이 그림에서 굵은 실선으로 표시한 것이 인코더에서 전송한 vector

   인    v[0][0][0:1J이다.     이      v[0][0][0:1］과   dmvector[0:1]로부터       그림에        표시한
  v[2][0J[0町과 v[3][0][0:l］을 구하1 낸다． 즉 decoder에서는 pari口가 같은 field로부

  터의 motion vect町로부터 parity가 서로 다른 field로부터의 motion vect아를 구하1

  내게 된다. 이렇게 한 field어］ 대해서 각각 2개씩（한 개는 전송된 것, 또 하나는
      1
          MPEG
204       VIDE0




            디코더에서 계산된 것）을 구해서 그 2개의 motion vect아를 갖고 한 fie닢를 움직

            임 보정한다. 결국 평균을 취하는것인데 자세한 방법은 combine predictions 부분

            에서 설명한다. 이 v[2][O][O: 1］과 v[3][O][O:1]을 구하는 방법은 다음과 같다．



                  vecto巾］[0]［이＝((ye如巾］[O][0] ' m[paiity什re吼Pahty나）re司）112) +dmvector[0]; vector[r][O][1]

                              = ((vector[O][0][O] * m[parity_ref][parity_pred])//2)

                                       + e巾ality_ref]巾a向pre미 + dmvecto巾］;



              여기서 dm叱ctor[O］와 dm比ctor[1］은 각각 differential motion vect아의 수평과 수

            직 성분이다. 이는 표 5-21의 \/LC table을 이용해서 코딩하며 값은 -1,O,+1이다．

            이 값은 그림 도21어］ 표시한 바와 같다．


                     표． 5-21 \／애야)le len아h codes for dmvect＞巾） (MPEG IS : I야扼 B-i ])
                                                 n小e                   value
                                                  11                     -   1
                                                  0                      0
                                                  10                         l




              m[parityref][parity_pred］는 predicted field와 reference field 사이의 field 간 거리
            (distance）로 표 三22와 같다. 여기서 pan口ref는 reference field의 panty이고

            pan口H皿ed는 predi아ed field의 pan口이다．


                    표 5-22 De仰佈on of ri乂pa向ref）自咐y_pred) (MPE（今 IS : I야)1e7-1])
                                                                                 m[j欠'I亥y_re月[paritypred]
                         pictut七sthactan七         切p_field血絨            n可1][O)                  m[O][1]
                         11        (Frame)               l                       l                  3
                         11        (Frame)               0                       3                  l
                         01     (Fop Field)                                      l
                         10 (Bottom Field)                                                          l
                                                                             205




     또한   e[pa血y-爬fl[parit兄恥ed］는 top field와 加如m field의 血e 사이에 0.5만큼

   의 간격차이가 나는 것을 보상해 주기 위한 것이며 표 5－乃과 같게된다．




          표5-23 DefinElion of e(partty rel)(F刃脚jred) (MPEG IS: Table 7-12)
               까旽口可                  I月U玄ypred         네p口r勿J明蜘7幻J7ra1
                   0                       l                 +1
                    l                     0                   -1
5.2.6. C이or con）口onents의 Sc이ing
     이는 색신호가 휘도신호어］ 비해서 해상도가 반이 되는 chrom血ance format이

   있기 때문에 이를 보상하기 위한 것으로 3개의 chrominance format에 따라서 다

   음과 같이 Sc曲ng한다．



       (a) 4: 2: 0 format의 경우

              vector[r][s][0] = vector'[r][s] [OJI2;

              vector[r] s][1] = vector'[r][sj[1]/2;

       (b) 4: 2: 2f아in毗의 경우

               vector[r][sj[0J = vector'[rj[s][0]I2;

              vector[r][s][l I = vector'[r][s][l];

       (c) 4: 4: 4 format의 경우

               vector[r]Es][0] = vector'[r][s][O];

              vector[r][s][1] = vector'[rj[s][l];



5.2.7, 반화소예측을 위한 필터링
     디코딩된 motion vec恤는 반화소단위이므로 이를 반으로 나누면（즉 vector[r]

   [s][t] DiV 2 = int_vector[t] ) 이 mt妃Ct띠가 （정수＋0.5）와 같이 화소중간어］ 위치하
2（冷




      거］ 되는 경우가 발생한다. 따라서 이와 같은 경우는 양쪽으로 인접한 화소의

      평균값을 움직임 보상값으로 해야 하는더］ 이의 표시를 위하여 h띠ffl明띠를 1로

      set仕略한다.    h삼f_flag[0］은 수평 쪽의 움직임벡터 mt妃ct[0］가 （정수＋0.5）로 된

      경우 1로 되고, h띠f_flag[1］은 수직 쪽의 움직임벡터 虹vect[1]이 （정수＋0.5）로 된

      경우 1로 된다. 움직임벡터 (mt_vect[0], mt_vect[1]）이 （정수,정수）,（정수,정수＋0.5),

      （정수＋0.5,정수）,（정수＋0.5,정수＋0.5）인 4가지 경우에 움직임 보정값 1玘1皿ed를 살

      펴보면 다음과 같다．



          (a)   （정수, 정수）인 경우

                  pel_pred[y][xj
                  PeL-Pred         pel_reffy+int_vec[1]J[x+int_vec[0]];
                          [y][X] = Pel1ref

          (b)   （정수, 정수＋0.5）인 경우

                  pel_pred[y][xl = (pe1_refTy+int_vec[1]][x+int_vec[0I]

                                   + pel_refly.i-int_vec[1J + 1J[x+mt_vec[0]])//2;

          (c)   （정수 +0.5, 정수）인 경우

                   pel_pred[y][x] = (pe1_reffy+int_vec[1]][x+int_vec[0jI

                                   + pe1_re玎y+int_vec[1I][x+mt_vec[0] + fl)//2;

         (d)     ( 정수 +0.5, 정수 +0.5）인 경우

                   pe1_predIy}[xI = (pel_refly+int_vec[ 1II1[x+int_vec[0I1]

                                   + pelH呵［y＋沁4妃c[1]][x＋奴_vec[0] + 1]

                                   + pel_refly+int_vec[1I + 1][x+int_vec[0]]

                                   + pel_ref[y+mt_vec[1j + 1][x+int_vec[0] + 11)刀4;



        여기서 pe냐妃d[y］因와 p吐自珝因는 각각 predicted picture와 reference picture의

       화소값이다．
                                                                                        207
                                                                             나    1 너




5.2.8. 예측값들의 평균（combine predic卄ons)
        이것은 예측된 것이 두 개 이상 있을 trfl 그 2개를 macr面lock당 평균해서 최

      종적인 움직임 보상을 하는 과정으로 B-picture인 경우와, P-picture에서는 dual

      p'1끄叱인 경우에서만 이용된다．



 1      단순 斤C刃冶 t功추

        이때는 B-j呱cture인 경우밖에 없으며 최종적인 움직임 보상값 呻_pred[y][시는

      다음과 같다．



          pel_pred[yftx] = (pel_pred_forward[y][x] + peLpre&backward[y][x])//2;



        색신호에서의 위의 계산크기는 4:2:0, 4:2:2, 4:4:4 的rmat에서 각각 8X8, 8X16,

      16X 16 (samplexline）이다．



  S     단둔＝ 万eld r可추

        이 경우는 field prediction인 경우로 크기는 16x8이다. peL皿ed[y][시는 윗식과

      같다. Chrominance 白rmat어］ 따른 크기는 다음과 같이 丘ame picture인가 field

      picture인가 따라서 다음과 같이 달라진다．

          a) framepicture: 8X4, 8X8, 16X8 (s如plexline)

          b) fieldpicture: 8X8, 8X16, l6X16 (samplexime)



 N      16x8m이ion compens（그／幻n

       Field picture어］서 위아래 각각의 16X8 block어］ 태해서 따로 만들면 된다．

      Chrominance format어］ 따른 크기는 각각 8X4, 8X8, l6X8이다．
       MPEG
208    니DEO




       M    Dualprime

            같은 pa血y로부터의 prediction과 다른 pan口로부터의 예측을 다음과 같이 평균

           한다．

              洲_pred[y似卜 巾吐恥ed寸啣le中an口［y][시 + pel_pred＋叩osi也par幻［y］因)11 2;



            Chron血mnce format어］ U｝른 크기는 field picture인가 丘ame p奴ure인가어］ 따라서

           다음과 같이 달라진다．



              a) frame picture: 8 X 4. 8 X 8, 16 X 8 ( sample x line)

              b) field picture: 8 X 8, 8 X 16, 16 X 16 (sample x line)




      5.2.9, 합산과 포호KAd배on and s（카내ation)
            이것은 움직임 보상에서 얻은 p[ylllxl( = 阿e皿ed[y正xl)와                     IDCT한 결과인

           tlyl[지를 다음과 같이 블록별로 더하는 것이다．



              化r(y田y<8駙＋) {

                        for(x=O;x. 8;x++) {

                                   d[y][x] = fWJ[x] + p[y][x];

                                   if(d[y][x]<O) d[y][x] =0;

                                   if(d[y][xI>255) d[yl[x] =255;
                                                                    MPEG
                                                                    피DE0    209




5.2.10. Skipped macroblock
        어떤 data도 전송되지 않은 macr小l(乂k을 sk巾ped macr的lock이라 한다. 이러한

      skipped ma아的lock은 macro바兀k_address_il乂rement를 보면 알 수 있다. 즉 앞에서

      도 설명했듯이 slice의 시작을 제외하고는 macrobl어：k_address_increment가 1 이상

      되면 skipj光d macr的k乂k이 있는 것을 뜻한다. 이러한 skipped macrobk乂k에서는

      motion ye아아도 없기 때문어］ 앞에서와 같은 과정을 할 수가 없다. 따라서 어떤

      방법을 이용하써 그 전 fran叱으로부터 data를 가져와야 하는더］ 이는 다음과 같

      이 B-picture, P-picture에 따라 틀리고, 또 field picture, frame picture어］ 따라 틀리게

      된다.     I-picture에서는    picture_spati出_ scalable_ex把ns而n(）이   현   picture의
      picture_header 뒤어］ 존재하는 경우나, bitstream 내에 sequence_scalable寸extension()

      이 존재하면서 sc십able mode가 SNRsc出ability인 경우를 제외하고는 skipped

      macr아如ck은 없다．



  s     Pflek了尸厄加／e

       예측은 field끄均如n口pe이 'II妃姓base寸인 것으로 가정하고, 예측되는 field와

      같은 pa血y의 field로부터 보상된다.           入4otion vec的r는 (0,0）으로 가정되고 入4otion

      vec的r pred奴아는 0로 초기화된다．



 '     p欣그／7冶尸幻加re

       예측은 fran妃Hn刃tion_type이 "Frame-based" 인 것으로 가정하고， Motion vector

      는 (0,0）으로 가정한다. 八1o如n vector pred奴아는 0로 초기화된다．



 1     B展汨p/c加／e

       예측은 field小n姓幻n口pe이 "Field-base寸인 것으로 가정하고, 예측되는 field와

      같은 pa血y의 field로부터 보상된다. 예측의 방힝寸orward, backward, bi＜血吼如n심）

      은 이전 매크로블록과 같이 하고, Motion ye아아는 이전 매크로블록의 해당 vector

      와 같은 값을 갖는다. Motion ye아아pred奴아는 아무 변화가 없다．
210




      N    助TC肋이)iC／나e

           예측은 frame_motion寸竝pe이 "Frame-bas以1" 인 것으로 가정하고, 예측의 방향

          (foi꾀ard, backward, bi네rectional）은 이전 매크로블록과 같게 한다.     Motion vector

          는 이전 매크로블록의 해당 vect아와 같은 값을 갖는다. Motion vect야pred奴아는

          아무 변화가 없다．




  5.3. 공간적 계위（S먀卄떼Scalab咐y)
           Spatial sc심ab小口는 그림 5 -13과 같이 lo＼比r layer와   enhancmei止layer로 구성되

          어 있다. I乂）wer layer는 해상도가 낮거나 크기가 작은 기본적인 bits打earn이며

          enhancment layer는 추가적으로 붇여서 해상도나 크기를 크게 해줄 수 있는 bit

          S甘earn이다. 원칙적으로 lower layer는 독립적으로 디코딩이 가능하기 때문어］ 어

          떤 형태로 코딩을 해도 enhancment layer와 결합할 수 있치만 여기서는 MPEG2

          나 MPEG1규격을 따르는 것으로 규정하며 slice구조도 restricted slice 없ructure를

          가져야 하는 것으로 한다．
                                                                                                              MPEG
                                                                                                              피DE0              211




                  Lower Layer
                    Bitstr由m 卜




              Prediction
             FieldJFram小m+ Framestors
              S日ection     Addressing                                          Framesto


                 vec幻巾］[s］屆］            I                                                                       d加1陀｛
                                                                                                                    日岡
                                M1니＼
                                       ＼니




                                                                 1
                                                                                                     I!
             Additional              Sc꾜ing


                          1三
                                                                                  pcI
             Dual-Prime             for Colour
                                                                       Half-
                               >                               片 1Prediction                Upsampl巴
             An山n妃tic              C口mpon口its                     卜끄t帥g
                                                                 I.
                土             vectos[r][s}[t]



      From    Vect（可                   比if-Pel
                                                     /                 Combine
                                                         ,/"
                                            inso
  Bitstrmm   Decoding                                                 Predictions
                                                                                                 \
             솥
                               戶口／-Pr口d_temy巾] [x]                                                              姻
                                                                                                          J
                                                                                                          地     如           뇌
                                                                                             V
                                                                                                                        J
                          Vec加r                                                                               Decoded
                          Predictors                                                                          samples


                                                               加］［目                                  却］［日

      그림 5-13 Simplified motion con）口ens（寸ion process for sp그ti이 sc이야Dility
                             (MPEG IS : Figure 7-13)
                                                                                          4 毛 ＼용뚜，
                                                                                          나＞ ; 나C.
  Spati카 scalab小口에서는 그림에서도 알 수 있듯이 기존의 temporal prediction뿐

만 아니라 lower layer에서 가져오는 spatial prediction을 하는 것이 보통과 다르다．

따라서 pred奴ed fran妃은 이 temporally predicted 丘ame과 spatially predicted frame의

가중합佃eighted sum)으로 구해지며, 다른 과정은 동일하다. 여기서는 spatial

prediction과 telT叩oral i玭diction과정 그리고 이 둘을 가중합（wei帥妃d sum)하는 과

정으로 나누어 설명한다．
212




      5.3.1 , 공간예측（Sp에이 predic卄on)
                                                                                        일
             Spatial prediction은 lower layer에서 pre小ction을 위한 reference frame을 고르는
         과 그 고른 丘an配의 크기를 그림 5-14와 같이 enhancement layer어］ 맞도록

         resamp血唯하는 작업의 두 부분으로 나뉘어진다. Resampi血g작업은 reference frame

            전체에 대해서 하지만 한 macro뱌乂k의 디코딩을 위해서는 resam미ed된 frame 중

            그 위치어］ 대응하는 macroblock 부분만 필요하다．

                                                                                    叱柳,1
                                  加叱rlqyerpr口dn才10七ye)伽刎1s,zd卞 Vm才,cal_sijbs口7꺄？in坦J；
                                                                vertica匕功S口7？窄枷료facto乙거
                                                                          \\,.,
                                      lower 1凹'er_ho月no刃t口？Uq力3et
                                                       卜



              加wer1la叩L1꾀寸icalc力3et



                 뀝口 冬h七m二




              士Oh늠芯mK띠늉童1늄兮요

              加叩erk 'erj片edic打0之加月no月t그L닯ze
                                                       lower_I毋er_predic枷L加r汪on姻S坦e京
                                                             加陀on奴-功5口7끼口渤已fa曲乙Jy
                                                              h아.IZ口ntal꾀加m叩枷gfi密加Tm2

              그림 5-14 比n1아ion of the 'spa作긔' pre네ction b미nterp(긔베on o什he lower layer
                                   F긔ct내e (MPEG IS : 日gure 7-14)



        N     reference斤ame의 즈／택

             I刃wer layer어］서의 !eference frame은 lower_layer_ten叩아심_referenc르어］ 의해서 주

            어진다. 즉 디코더는 이 lower_layer_t印lpor吐reference에서 표시된대로 re也rence

            丘ame을 고르면 되지만 인코더에서는 아래와 같은 picture들 중에서 reference

            picture을 골라야 한다. 그러나 기본적인 원칙은 enhancement layer의 picture가 디

            스플레이되는 시간이 같은 lower layer의 fran配을 reference frame으로 삼는 것이

            제일 좋다．
                                                                        213
                                                                   H1




 a) 시간이 동일하거나 또는 가장 최근어］ 디코딩된 lower layer의 picture

 b) 시간이 동일하거나 가장 최근어］ 디코딩된 lower layer의 I 또는 P picture

 c) lower layer으-1 low_delay가 "1'' 이 아닐 t대 가장 최근 바로 이전어］ 디코딩된

   lower layer의 1나 P picture



 resat기pling과졍

 Resamp血lg은 lower layer으1 丘ame크기를 enhancn妃nt layer에서 상응하는 부분의

크기로 재조정하는 과정이다. 보통 enhancment layer의 화면이 크기 때문어］ 이

과정은 주로 화면크기를 키우는 과정이다. 이 resampling과정은 fran妃을 기본으

로 하고 그 frame이 field picture이건 아니건 상관하지 않는다. 따라서 frame

picture인 경우에는 단순하게 화면크기만 맞춰주면 되지만 field picture인 경우어］

는 하나의 fie닢를 demterlace시키고 화면크기를 맞춰준 다음에 다시 field를 만들

어주기 위하여 rein把rlacing시키는 과정이 들어가거］ 된다. 이것을 경우별로 정리

하1 보면 다음과 같다. 멈코m훤도신호어］ 대하여 살펴보자．



   a) lower layer reference丘a끄配이 pro앉essive인 경우

            (lower_layer_progressive_frame =" 1")
 이 경우는 그림 5－巧와 같이 단순히 수평 수직축으로 res跏叩ling만 한다．



  Lower
   layer
 Refemece
  Frame
            1H+
                     Vertical
                    Resampling
                       과정
                                         Resampling
                             '" \ ' ""“芬몰‘
                                           \
                                          Horzontal

                                            과정
                                                       . U$s帥ripled
                                                        "
                                                            "
                                                                "跏 "


                                     L_ verl_pic      L hor_pic
                             그림 5-15 resampling
      1
          MPEG
214       V山EQ




             이 최종 叩sam미edfran叱은 enhan凹ment layer의 progressive_丘ame = "l " 이면
                                                                  간주한다． 이때
            progressive로 간주하고 progressive frame = "아이면 interlace로

            lowerjayer코曲lterlaced_field_select는 무조건 "1" 이 되어야 한다．



              b) lower layer의 reference丘ame이 interlace인 경우

                            (lower_layer_progressive_frame = "0")

                    i) enhancement layer의 progi七銘ive士ame = "0" 인 경우

                       이      경우는      그림     5-16과     같이     lower    layer의   reference    丘a끄ae을

                       dein把rlacir唯시킨 후에 resamp血堪을 하고 다시 remterla血培을 시킨다．

                       이때도 lower_layer_deinterlaced_field_select는 무조건 1이 되어야 한다．



                    ii) enhancement layer의 progressive士anie=" 1" 인 경우

                       이 경우는 그림 5-17과 같이 de血terlacing과 resam미血g 과정만을 이용

                       하여 최종적으로 progressive한 upsampled frame을 얻는다．



                  Lower                                        Vertical
                                      Deinterlace



                                                       V
                   layer
                                         과정                  resampling
                 Refemece
                                                                과정
                  Frame

                                                         \   prog_pic              veil_plc

                                       Horizantal            Reinterlacing
                                       resampliiig               과정
                                          과정

                                                             hor_pic


                                                     그림 5-16
                                                                                                               MPEG
                                                                                                               VIDE0         215




   Lower Layer                  deinterlacmg                      A                / "썲스.rjayer_
  Reference Frame       卜           과정                    j나
                                                                                                dem妃nlaced玉라d1
     Top Field
                                                                       \/ 尹 \
                                                                      k\                    .
                                                                                          Sel比．Lr)
                                                                                                「이띤＝            "0
                                                                                                                .
                                                                                                                    ")
                                             prog_pic -                    /\       \＼뇨
                                                                                                아nerw哨e

   L叭Ver Layer
  Reference Frame
                                de血르na.
                                            과정
                                                 血g       1
                                                          j寸
   B아幻m Field

                                             prog_pic -




            /           Vertical
                       Resampi血g
                          과정
                                                 ＝나
                                                                I如rzontal
                                                               Resamp丘［lg
                                                                  과정
                                                                                         커［斗 UI跏np血g
                                                                                               Fmmt


                                          veil_plc -                        hor_pic -

                                                  그림 5-17



      위 그림들의 upsampling 과정을 정리하1 보면 표 5-23과 같다．


                  표 5-23 냐＞sam디峽7process (MPE（引S: T（가扼7-15)
  lower_layer_        lower_layer_                     pr（准r幽ye小                 Apply                       Entity used
  (I川毗erI ' 'I      pro伊心sly已加me                         fr nip                 deinterbe                   for prediction
   field select                                                                  proc珊

        0                   0                              l                       yes                 tOpti잊d
        l                   0                              l                       yes                 bottom field
        l                   l                              l                       no
        l                   l                              0                       no                  fr
        l                   0                              0                       yes                 both fields




 색신호는 원칙적으로 휘도신호와 비슷한 과정을 거치지만 C뇨ominance 白rnlat

어］ 따라 다를 수 있고 또 lower layer와 enhancement layer의 chrom血ance format이

다를 수 있기 때문어］ 앞으로 설명할 deinterlace, resampling 등에서 설명하는 더］

쓰일 표 5-24와 같은 변수들은 표 5-24, 5-25, 5-26에서처럼 chrominance format 각
216




      각어］ 대해서 그 값을 달리하고 있다. 그러므로 색신호에 대해서는 표 5-24에서

      정의한 대로의 값을 그태로 대입하면 색신호일 때의 처리과정이 된다.                                                                  위의

      그림에서 블록으로 표시한 각각의 과정들을 다음 절부터 살펴보기로 한다．


                  표5-24 Local vaabIes used in 5.3.1.1. to 5.3.1,o. (MPEG IS : Table 7-l6)
      vanable              value for luminance pmcessing                 value for chn)minance pmcessing

      II h size           10吼r_layer나：,iediction_hori끄汕町毗e               lower_layer_p帥ctionjiorizont出_size
                                                                         I chmma_ratio_horizont고flowerj
      II V size           lower_layer下）rediction_vertical_size           k六wer_layer_p肥如t由兀妃mc叱毗e
                                                                         / chmma_ratio_vertical[lowerj
      II h offset         lower_layer_horizontal_offset                  lower_layer_horizontal_offset
                                                                         / chmma_ratio_horizontal[enhance]
      II v offset         k月자町jayer_vemi：키10甘set                         lower_layer_vertic띠_offset
                                                                         / chroma_ratio_vertical[enhancel
      h subs m            hoiizont毗subsarnpling卜factor_m                 hoiizont고subsani山1lg- factor_m
      h subs n            horizontal_subsarnpling_factor_n               hoiizontal_subsamp1ingfactor_n
                                                                         * format ratio horizontal
      v subs rn            vertical_subsarnpling_factor_m                vertical_subsamp血且factor_rn
      v subs n             vei如可刈bsam的昭1facti兀n                          vertic띠_subsamp血lg_factor_n
                                                                         * format ratio vertical




                     표 5-25 chrominance sari刈ing r예Os 幻lay이 = 如＼WE兀 enhance}
                                        (MPEG IS : Table 7-17)
                          chi工가ninance 向mat           chroma ratio          c如oma ratio
                              lower layer            horizontalflayerl      veiticalUayerl

                                 4:2:0                       2                     2
                                 4:2:2                       2                     l
                                 4:4:4                       l                     l
                                                                          無目 :17
              표 5-26 chrominance 向rm아 ra卄Os (MPEG IS Table 7-18)
          chrominan此 如miat   chmminance fomiat        的imat ratio    如Imat ratio
             lower layer     enhancement layer         horizontal      vertical

               4:2:0               4:2:0                   l              l
                4:2:0              4:2:2                   l              2
                4:2:0              4:4:4                   2              2
                4:2:2              4:2:2                   ]              l
                4:2:2              七t4                     2              l
                4:4:4              4:4:4                   l              1




D    De幻／er/acing

     D帥出rlacmg은 fran肥의 각 field에서 그림 5-比과 같이 빠진 곳似로 표시）을 0

    으로 채운 뒤 표 三27과 같은 필터를 이용하여 보간(in自pola如n)한다．




                                    0            x

                                     x           0
                                    0            x

                                     x           0
                                    0            ><
                                                        b temporal
                                      t         T         axis
                                    first    second
                                    field     field


                                     그림 5-18
      1
          MPEG
218       VIDE0
          H?




                                       표． 5-27 Deintedacing Fitter (MPEG IS : Table 7-19)
                                                                  two field aperture                   one field apertu七
                    Ten叩OI丑l   Verti川           Filter for first field       Filter for second field   Filter (both fiel小)
                       -   1               2              0                                l                   0
                       -   1          0                   0                            2                       0
                           l           2                  0                            -   l                   0
                       0                   l                 8                         8                       8
                       0              0                  16                            16                      16
                       0                   l                 8                         8                       8
                           l          -2
                                                          -   1                        0                       0
                           l           0                     2                         0                       0
                           l     +2                      -    l                        0                       0




                    이따1 ：휘도신호로서 picture_structure가 frame picture이면 표 5-27의 two field

               따玘rture filter를 이용하고 그 외에 휘도신호와 색신호는 one fi이d 可玘rturef血er를

               이용한다. 이후에 정규화를 위해서 필터링된 sum값을 다음과 같이 16으로 나눈

               다．
                                                      prog_pic[y]{x] = sum//i 6
                    그 후 [0: 255］의 범위를 넘어가는 것은 이 범위 내로 한정시킨다. 또한 필터

               의 구경（aperture）이 picture의 경계를 넘어가는 경우는 picture의 경계를 확장한

               값들을 이용한다．



          N         Vertical resampling

                    이 과정은 1O＼比r layer丘ame이 enhancement layer의 상응하는 부분에 맞도록 재

               조정（즉 lower layer의 그리드와 enhancemei止layer의 그리드를 맞추는 일）하는 것

               으로 이때의 frame은 원래 lower layer가 frame picture이거나 또는 field picture를

               앞에서의 deii佃rlacing과정을 거쳐서 frame stur아ure로 만든 것이거나 상관이 없다．

               이렇게 크기를 변경하는 일을 入WEG2에서는 다음과 같이 거리에 비례해서

               inter兀lation해 내는 과정을 통해서 하고 있다．
                                                                                       219




   ve&.pic[yh + lLv_offset][x] = (16- phase)*prog_pic[yl][x]+phase*prog_pic[y2][x]

   여기서
   蜘+ II V 0卄＄et            =          0U巾Ut san,叱co0세nate in vert_pic

   yl                       =          (Yh * v_subs_rn) / v_subs_n

   y2                       =           yl + 1   if (yl <Il_v_size - 1)

                                       yl            아herb너se

   phase = (16 * ((Yh * v_subs_m)%v_subs_n)) 11 v_subs_n



N Horizontal resampllng
   이 과정은 수평방향에 대해서 하는 것으로 방법은 다음과 같다．

   hor_pic[y][x, + lLh_off set] = ((16- phase)*ver下啣j[xl]+phase*ve比pic[y][x2]) 11256

   여기서

   Xh + ILh_offset          =          0바四tsamF가e Ca-이네nate in hor_pic

   xl                       =          (x1, * h_subs_m)/h_subs_n

   x2                       =          xl +1      什 (xl <Il_h_size-i)

                                       xl              otherw怡e

   phase = (16 * (()q * h_subs_rn) % h_subs_n)) 11 h_subs_n



N Reinterlacing
   이는 resam히血g된 fra끄配을 enhancement layer가 field struc恤e인 경우 다시 field

 로 만드는 과정으로 만약                       h아-pic가 원래 lower layer의 top field로부터 만들어

 졌다면 hor-pic의 even血e이 spat_皿ed_pic의 even ffi妃으로 된다（즉 以Id lii妃을 빼버

 린다）. 또한 반대로 h아pic가 원래 lower layer의 b아恤Ti伽ld로부터 만들어 졌다

 면 hor_pic으lodd 血e이 spat_皿ed_pic의 odd line으로 된다（즉 even lii妃은 빼버린

 다） .
220 出믐뚫


  5.3.2. 시간예측（lempor이 prediction)
       Temporal prediction은 앞의 motion comi玘nsation 부분에서 언급한 것과 동일하

     다． 다만 이 spatial Sc심ab小口에서는 예측이 시간예측（tempor如redic如n）과 공간여］

     측（spati出 predic如n）의 두 부분으로 나뉘어져 있기 때문어］ 만약 공간예측（spatial

     prdic如n）만 가지고 완벽한 예측을 이룰 수 있다면 구태여 시간예측을 사용하지

     않아도 되며 따라서 motion ye아아를 보낼 필요가 없다. 그러므로 scalab小勻가 없

     는 경우어］ 비해서 기존의 motion vect아를 보내지 않아도 되는 경우가 생기는더］

     이따I motion vect아predictor PMV를 갱신시키는 방법이 틀려지게 된다. 이를 위한

     표가 표 5-28과 5-29이며 spatial scalab小ty가 있을 IT긔1field picture와 行ame picture어］

     서의 예측방법과 전송되는 motion ye야아를 살펴보면 각각 표 5-30, 5-31과 같다．
                                                                                                .
                                                                                                    MPEG
                                                                                                    미DE0   221



                표． 5-28 Upd그卄ng of motion vector predictors in Field Pictures
                                 (MPEG IS : Table 7-22)
fi긔me moth［月lJy1比
                     macrobl어：
                             k motion forward
                           macrobl어：
                                   k motion backward
                                macroblock intra
                                     spatialjemporal吼It虹크出S
                                                   Pre小C恤s to update

Field-based聿                     l            0    尸凡f1411[0j[1:0] =／꺼v1140J[0][1:01<
Field-based           l     l   0             0    PM141][0][1:0] = P才V[0I[0I[1:0]
                                                   PAIVIJI[1I[1:0I = PMV[0][l][1:O]
Field-based           l    0    0        0.   1    PMV[lJ[0][1:0J = PMV[0I[0][l:0]
Field-based           0     l   0        0,   1    川4V[1][1][1:0] =／개才V[0][11[1:0]

Field-ba,sedt         0    0    0       0,1,4      尸MV[r][s]［小＝ 0 흐

16x8MC                l     l   0             0     (none)
16x8 MC               l    0    0        0,   1     (none)
16x8MC                0     l   0        0,1        (none)
Dual prime            l    0    0             0    ／꺼／V[1][0][1:0I = 尸MV[0I[0][1:이
Note:         PMV[rjtsl[1:0] =PMV[ul[v] j1:O] meansthat;
                          PA'!Vlr][sl[1] =／꺼／V如］[vIE!] and PMV[게sj[0I = 川'!V[u伽][0]

         X If啣毗汕nent十m얘ony出이.Sis配ro then PMV[r][s][小S set t毗帥侄아네r, s and t).

         + field_motion_type is not present in the bitstream but is assumed to be Field-based

         효 PMVIr][s][t] is set to zem (for십l r, sandr). See 7.6.3.4.
      MPEG
222   피DE0




                          표 5-29Updalingofm아ion vec幻나)redicto四 in Frame F가ctures
                                          (MPEG IS : Table 7-23)
      fram仁m瓜)nty比
                            macroblock motion forward
                                   macroblock motion backward
                                         macroblock intra
                                              spati皿如mporal岫小tclass
                                                             Predicto心 to update

      Frame-based                        l         0         PMV11I[0I[1:0] = PMV[0110][1:0Ix
      Fram口based             l      l    0         0         PMV[1][0J[1:0] = PMV'[OJ[O][l:이
                                                             PM1'[lI[lI[l:OI = PM140][1][1:0]
      Frame-based            l      0    0      0,1,2,3      PMV[1][0]tl:0] = PMl40][0][1:0J
      Frame-based            0      l    0      0,1,2,3     ／꺼IV[1][1][1:0] = 尸a才V[0][1][1:0]

      Fi코me-based土           0      0    0     0,1,2,3,4     尸MV[rl[sl[tl = 0蚤

      Field-based            l      l    0         0         (none)
      Field-based            l      0    0        0,1        (none)
      Field-based            l      0    0         2         PMV[1][0][1:0j = PiW%'[O][O][l:O]
      Field-based            l      0    0         3         PA'IV[lI[OI[l:O] = PMVIO][0I[1:0I
      Field-based            0      l    0        0.1        (none)
      Field-based            0      l    0         2         PM'VIl][l][l:OI= PMV[0J[1J[l:0]
      Field-based            0      l    0         3         PMV[l] [1][1:0] = PMV[0I[1][1:0]
      I沁al 叫11e（包            l      0    0       0.2.3       PMV[1][0][1:O] =PMVl0I[0][1:0]
      Note:         PMV[rj[sj[1:0] = PMV[u][vl[l:0] means that;
                                 PMV[r][s][1] = PMV[u][vj[1 j and PMV1rI[s][0I = PMV[ul[v][0]

              X If conce키ment_motion_vectors is zero then PMV[rl[s][tl is set to zero (for出l r, s and t).

              土 frame_motion_勺꺄is not ptsent in由e bitstream but is ass山町Ito be Fi刊［ise-based

              효 PMV1r][sj[t] is set to zero (for a끄［r, sand 1). See 7.6.3.4.

              @ [油1prime can no奴used when斗ati카止畔oral_in啞町weight = "0".
                                                                                                                 223



                     표． 5-30 다edic作＞ns and ma卄an vectars in field F긔ctures
                                   (MPEG IS : Table 7-24)
field_inotion勺1比

                       macroblock motion forward

                             macrobk乂km成油i backward

                                  macroblock intra

                                        spali고te叫lot沚weight dass

                                                       Motion vector                P11삐iciion fi기口a巴d for

Fie1d'based土                       l         0         vector'[O][OJ[l:O]><         None (motion vector is for
                                                                                    concea노玘nt)
Field-based            l     l    0          0         vector'[O][O][l:O]           whole field, forward
                                                       vecto尸[O][l][l:Q]            whole field, backward
Field-加sed             l     0    0         0,1        vector'[OJ[01[1:01           whole field, forward
Field-based            0     l    0         0,1        vector'[O][l][l:O]           whole field, back자ard

Field.based牛           0     0    0        0,1,4       vect）尸［0][0I[l:0］蜂           w加妃 field, forward

16x8 MC                l     l    0          0         vecto尸[01[0I[1:OJ            1料比r 16昭 field, forwa川
                                                       vector'[l][O][l:OI           lower 16x8 field, forward
                                                       vector'[O][l][l:O]           upper 16x8 field, backward
                                                       vector'[ ll[ fl[l:O]         lower 16x8 field, backward
16x8 MC                l     0    0         0,1        vecto尸[OI[OI[l:OI            upper 16x8 field, forward
                                                       vector'LIJ[O][l:OI           lower 16x8 field, forward
16昭 MC                 0     l    0         0,1        vector'[OI[l][l:O]           upper 16x8 field, backward
                                                       vector'[l][l][l:O]           lower 16x8 field, backward
Du심 piime              1     0    0          0         vector'[O][O][l :0]          whole field,    same     parity,
                                                                                    如rward

                                                       vecto尸［2][0][l :0］싸          whole field, opposite parity,
                                                                                    向rward
Note:         Motion vectors are listed in the order they appear in the bitstream

        X the motion vector is only pre記nt if concealment_motion_vectors is one

        卞 field_mo如山恥跏啣re配ntin山e bitstream but is assumed to be飼d加sed

        * These motion vectors are not present in the bitstream
        十 These n刃lion vecto心毗derived加m vector'[O][OI[l:OJ as descri毗in 7.6.3.6

        효 The motion vec幻r is趾帥毗e (zem, rem) as explained in 7.6.3.5
224




                          표 5-31 Predic寸ions and m아ion vect이引n frame口ctures
                                          (MPEG IS 汁（그ble 7-25)
      frame_n批jo也蜘e
                         macrobl어：k motion forward
                              macroblock_motion_backward
                                  macroblo出i intra
                                       spatial_temporal_weight_class
                                                   Motion vector                      Prediction formed for
                                       l          0                                   None (motion vector is for
      Fram己－based享                                         vector[O][OjT1:OIX
                                                                                      con兀alment)
      Frame-based         1    l       0          0        vector'[0I[0][1:0I         fi 配, 如iward
                                                           vector'[0] 1][1:0]         frame, backward
      Frame-based         l    0       0        0,1,2,3    vector'[O][OI[l:O]         frame, for入／ard
      Frame-based         0    l       0        0,1,2,3    vector'[O][l][l:O]         丘ame, b出永＼ward
                          0    0       0       0,1,2,3,4                              framle, forward
      Frame-based4                                         vecto尸［0][0}[1:0］蜂
      Field-based         l     l      0          0        vector'[O][0][1:0]         top field, forward
                                                           vecto4l][0}[1:0]           bottom field, forward
                                                           vector'[O][l][l:O]         top field, backward
                                                           vector'[l][l][l:O]         bottom field, backw끄
      Field-based         l    0       0          0,1      vecto40][0][1:0]           top field, forward
                                                           vector'[l][O][l:O]         bottom field, forward
      Field-based         l    0       0           2                                  top field, spatial
                                                           vect040][0][l:0]           bottom field. forward
      Field-based         l     0      0           3       vect040][0I[l:0]            top field, forward
                                                                                      的ttom 如姓 spatial
      Field-based         0        l       0      0,1      vector'[O][l][l:O]          top field, backward
                                                           vector'[l][l][l:O]         的如m fie姓 backward
      Field-based         0        l       0       2                                   top field, spatial
                                                           vector'[O][l][l:O]          bottom field, backw出
      Field-based         0        l       0       3       vecto40][1][1:0]            top field, backward
                                                                                       bottom field, spatial
                          1        0       0     0,2,3     vector'[O][0][1:0]          top field, same p계：ity, forward
      Dual prime@
                                                                                      b야torn field, same parity, f아w町d
                                                           vecto,1[0][0][l:0]*
                                                            vecto尸［2][0][l:0］싸         top field, opposi妃 p계由：y, forw게xl
                                                                                      bottom fid.,      opposite   parity,
                                                            vecto尸［3][0][l:0]' 卞
                                                                                      forward
       Note:        M야由n比如心arel出ted in the아der血ey ap休缸in由eb抽出am
               < the motion vector is only present if concealment_motion_vectors is one
               牛 fransemm（肛on勺pe is notp旺e配nt血the bi四trearn but is assumed to be Frame-i:日sed
               * These motion vectors are not present in the bitst叱am
               十 hi毗mo由n vec幻rs毗曲ved fmm vec切r'[O][O][l:O] as described in 7.6.3.6
               흐 The motion vector is切ken to be (zero, zem) as explained in 7.6.3.5
               @ Dual prime can not be used when spatial_temporal_in妃ger_weight = "0".
                                                                    225




   또한 5.2.4.2절（non spatial scalable m毗）에서 언급한 경우 이외에 spatial

  scalab小ty에서 m出on vect야pred奴아를 리셋시켜야 할 때는 다음과 같다．



      a) maci小lock이 오로지 sp毗al pie小ction만을 사용하는 P-picture에서

            (spatial_temporal_weight_class == 4)
      b) macr的lock이 오로지 spatial prediction만을 사용하는 B-picture에서

            (spatial_妃mpol可_weigh냐lass == 4)



   Field-based prediction이 사용되는 frame pi伽re에서 spatial_啣npor吐weight_class

  ==2이면, 전송된 ye아or는 bottom field어］서 사용된다（표 5-끄）. 그러나 이 vector

  [0］圄［1:0］는 PMV[0］同［1:0］으로부터 예측되고 I丕iIV[0］同［1:0］은 표 5-29와 같이갱

  신된다．




5.3.3, 공간예측과 시간예측의 선택과 조합
   어디서 어떻게 예측을 하느냐에 따라서 예측의 class가 다음과 같이 5가지로

  구분된다. 이 class번호는 spati심ten叩or심Hwei帥tc始ss의 값이 된다．



     Class 0: 把n叩oral-only prediction인 경우

     Class 1: 어느 field도 spatial田nly prediction이 아닌 경우

     Class 2: 的p fle닢가 spatial-only prediction인 경우

     Class 3: 加ttom field가 spatial自nly prediction인 경우

     Class 4: spati出－only prediction인 경우



   I, P, B-I加ture어］ 따라 각 class에서의 모드는 다음과 같다．
226




         (a) I-picture

            class 0--> normal inira coding

            class 1, 2, 3 ,4-->spafial만 쓰인다．

         (b) P-picture or B-picture

            class 0--> tempora只｝ 쓰인다．

            class 1, 2, 3 --> spati出과 temporal이                   모두 쓰인다．

            class 4--> spatial만 쓰인다．



         이 공간예측과 시간예측을 어떻게 섞느냐 하는 것도 \weight table어］ 의해서 정

      해지는톄 이 \weight table도, 표 5-32와 같이 spatial_temporal_weight_code_table寸

      index가 '以）II, " 01", " 10", "11" 인 경우의 4가지가 있다. 이 spatial_t이叩or고J比培ht

      下od口table_index는 picture spatial sc심able ex把nsion (）에서 전송된다．


          표 5-32 Intended（에owed) 斗）:1作艾ten耳兀口U사eight_code_tablejndex v이ues
                                  (MPEG IS : Table 7-20)
                                                  Lower layer formnat      1nhiqCement    SPafialtem目且a1w톄咐mC
                                                                           layer fonnat   ode table index

                                              Progressive or in把rlaced     Progressive    00
             Progressive coincident with enhancement layer top fields      Interlaced     10 (00; 01; 11)
      Pr叱res鉀e coincic妃nt with enhancer配nt layer加m 比如m 加L血                 Interlaced     01 (00; 10; 11)
                      Interlaced (picture_structure == Frame-Picture)      Interlaced     00or 11 (01; 10)
                         Interlaced (picture_structure != Frame-Picture)   In妃rlaced      00




         정확한 weight는 macrobk乂k_mode(）에서 전송되는 spati町卞mpor심                                              \veight_code

       에 의해서 표 5-33과 같이 결정된다．
                                                                                                        227



   표 5-33 Sp예아ten不好aLweights and S口에아tern口 （加山叩ht拍sses f아 the
  斗X캐al怡rnpo띠Lweight_code_t야兆jndex and sp아aL
                                             tern口아아w이gh工odes
                        (MPE（引S : I야)Ie 7끼）
    spat洌ten甲n刈                spati玭               spatial_         spati沚               spati沚
   weight_code_table_         tempoi川             ten叩oral          tempol까              temporal.m
         index               weight_oxte          weight (s)       weight class        integer_weight
          a）求
                                                     他5)                       l                    0
          01                     00                  (0; 1)                3                        l
                                 01                 (0;05)                 l                    0
                                 10                (05; 1)                 3                    0
                                 11               他5; 05)                  l                    0
          10                     00          /'     (1; 0)              2                       l
                                 01                (0.5; 0)             l                       0
                                 10                (1; 0.5)            2                        0
                                 11               他5; 0.5)             l                    0
          11                    00                  (1; 0)             2                        l
                                01                 (1; 0.5)            2                    0
                                10                (0.5; 1)             3                    0
                                11                (0.5; 0.5)           l                    0
         For spatial_temporal_weight_code_table_index == 00
                                                            no spatial_temp이al_weight_code is
         甘ansn血ted.




  표 三33에서 spatial_佃np이a1_weight尙가 섞는 비율을
                                                                           가리키는더］ 이 값은 전
체를 I로 보았을 때 spatial pre小ction의 섞는 비율을
                                                                  표시한 것이다. 그런데 (a, b)
로 표시한 경우 a는               top field의 섞는 비율을 말하고 b는 bottom field의
                                                      섞는 비
율을 말한다. 예를 들어 spati吐卞mporal_weight_
                                   code가 0, 1, 0.5인 경우의 pel_
pred[y兀시를 구하1 보면 다음과 같다．



   因中red[y}[xJ = p이中red_temply][xj (for spatial_旭n巾아쉐的帥t
                                                                   _code = 0)

   pe냐）red[yJ[x} =pe냐升ect多pat[y][x] (f아spatiaLtempor줴we
                                                        ight_code = ])

   p아下redly][x] = ( pe나）red_temp[y]［지 + pe냐片ed[yj[xl )I/2

                                              (for spatiaLtemporaLweight_code = 0.5)
228




      5,3.4. S뺘和edri日가oblocks
             앞의 5.2.10절에 더해서 디음과 같은 경우가 추가된다．


                                                        경우．
           a) 1-pictu妃에서 spatial predi沮on만을 이용하는
                                                            이용하는 경우．
           b) P-picture와 B-j攷cture에서 tei坤야a! pre小ction만을
                                                         ma口oblock뒤의 ma口oblo出은
           c) B-picture에서 spatial p肥diction만을 이용하는

              skip될 수 없다．




      5.4. SNR계위（SNR scakib咐y)
                                                                 정에서 孔C 코딩, inverse
            SNR scalab小ty는 그림 도19에서 볼 수 있듯이 복호과
                                                                layer로 나뉘어 있는 것으로
          scan, 血vrese quantisation이 loM肥r layer와 enhancement
                                                                   layer어］ 더해주면 high
          결국 DCT계수를 enhanceri玘nt layer로 더 보내면서 lower
                                                                  enhancen妃nt layer가 서로
          SNR을 얻을 수 있다. 이 SNR scalabili口는 lower layer와
                                                                    나가야 한다. 이러한
          밀접한 연관성을 이루고 있기 I대문어］ 디코딩을 같이하1
                                                                     동시방송帥毗ast）에
          SNR scalab小ty는 단순히 SNR뿐만이 아니라 chroma format
                                                                           format이 4:2:0
          도 적용할 수 있다. 이와 같은 경우에 원래 lower layer의 c뇨oma
                                                                     의 해상도를 높일 수
          인 경우 enhancement layer어］ 4:2:2 foi끄垠t을 전송하囚 색신호
                                                                   값만 빼고는 모두 버린
           있는더］ 이따1 lo＼比r layer에서 디코딩된 색신호는 intra-I乂
                                                                이용하게 된다．
           후에 enhancement layer에서 전송된 색신호 데이타를
                                                                                                   229



                                   QFS［비             Q町네미                        Fe?owg小小미

                       Variable                                   Inverse
      C으dedH      _                   Inverse        P                ati。
                                                                         n
                                                                         tis-
                        Leng出
       Data       尸                     Scan
                                                              Quan,
                      Decoding
                                                         소11出n比tic

              Lower Layer

       Enhancement Layer           QFS［비             Q비네미

                     Variable                                     Inverse
     （加ded        -                   Inverse        >                ati。
                                                                         ntis
                                                                                       F小小미
      Data        Pr Length             Scan
                                                          Quan,
                      Decoding
                                                         凡lthmetic
                                                                                      Frbn方ance[ v][u




                      ／小小비          ／小m미


                        Mismatch                                        Motion
                                           Inverse                                            Decoded


                                                                                 \
     Saturation                                          P             Compen
                         Control             DCT
                                                                        sation         卜盜珏；

                                                                                     d{y]［기


                  그림 5-19 Illu琡州on아decoding r가oces計아SNRsc이야켸啣
                                (MPE（引S : 日gure 7-15)




5.4.1 , 빈경되는 신택스 구조
    이는 SNR scalab皿ty를 이용할 경우 enhancement layer bits仕earn이 제한적으로 가

   지는 변수값들이다．



    (a) Sequence header

      다음의 값들은 load_u也之叩an小er m壯rix가 0일 때를 제외하면 lower layer

      와 다른 값들을 가질 수 있다．

                  bit_rate, vbv_bu拜er1s奴e, loadi址ra_quan小er寸ma虹1凡
230




                   in甘a_quantiser_ma甘ix, load_non_intra_quantiser_matrix,

                   non_intra_quantiser_matri乂



       (b) Sequence extension

          다음의 값들은 lo毗r layer와 다른 값들을 가질 수 있다．

                   profile_and_level_indication, c뇨oma_format,

                   bit rate extension.     vbv buffer size extension



       Layer마다 chrom乞白rmat이 다르면 chr아na_simulcast_flag는 표 5-34와 같은 값

      이 된다. Enhancement layer으-1 chroma_forinat은 lower layer보다 낮을 수 없다．


                   표 5-34 ChromaH計Ti내ca針_fiag (MPEG IS :T（그ble 7-26)
                      chroma format            （寸ir(川na fonnat      chronia simulcast
                       如wer layer)            (enhancement layer)
                          4:2:0                      4:2:0                 0
                          中2:0                       4:2:2                  l
                          4:2:0                      4:4:4                  l
                          4:2:2                      4:2:2                 0
                           4:2:2                     4:4:4                  l
                          4:4:4                      4:4:4                 0




       Lower layer bits打earn이 入4PEG1을 따르는 경우에는 sequence_炚帥sion이 lower

      layer어］ 존재하지 않으므로 디코딩을 위하여 sequence extension어］서 필요한 변수

      들이 다음과 같은 값들로 가정된다．



          progressive_sequence           =1

          chroma 白rn皿t                   = "4: 2: 0"

          horizontal size extension      =0

          vertical size extension        =0
                                                                  231




    bit rate extension            =0

    vbv bu卄er s也eex把n前on = 0

   low_delay                      =0

    frame rate extension n        =0

    frame rate extension d        =0



(c) Sequence display extension

     Enhancement layer만을 따로 디스플레이하지는 않으므로 이 ex啣臧on은 존

     재하지 않는다．



(d) Sequence scalable extension

     Scalable_n好把가 " SNR scalability " 이면 이 ex佃ision은 나타나게 된다．



(e) GOP_header

     Lower layer와 동일하다. 각 layer으1 ten叩oral爬ference가 같은 frame에서 초

     기화되도록 GOP header는 한 layer에만 있어서는 안된다．



(f) Picture header

     Vbv_delay를 제외하면 lower layer와 동일하다．



(g) Picture coding extension

    吼scale1口pe4 a1把mat口凹an을 제외하면 lower layer와 동일하다. 만약

    cli的m乞誼nulcast가        1이되면 chrom之似0勺I玘은 0이된다． Lower         layer
    bitstream이 入4PEG1을 따르는 경우에는 picture_c(넜血＆炚妃ns幻n이 lower

    layer어］ 존재하지 않으므로 디코딩을 위하여 picture_codin且ex把nsion어洲

    필요한 변수들이 다음과 같은 값들로 가정된다．
232




      f_code[0J[0]             lower layer의 동일한 코드 혹은 15

      f_code[0][1]             lower layer의 동일한 코드 혹은 15

      f_code[1][O]             lower layer의 동일한 코드 혹은 15

      f_code[1][1]             lower layer의 동일한 코드 혹은 15

                     intra_dc_precision =0

                     picture_structure       = "Frame Picture"

                     top_field_first         =0

                     frame_pred_frme_dct     =1

                     concealment motion vecto느 0

                     intra vlc format        =0

                  repeat_first_field         =0

                  chroma_420_type            =1

                  progressive_frame          =1

                  composite_display_flag     =0
          Lower layer의 q_scale_竝PC이나 심temate_scan은 0으로 가정된다. 이 값들은

          enhancen日it layer에서 독자적인 값을 갖는다．



      (h) Quant matrix extension

          이 extension은 필수적이진 않다. Load_intraj恥antiser_mati奴와 oad_chroma_

          岫乞叩antiser_matrix는 0이된다．
                                                                            233
                                                                        d




       (i) Picture 小splay extension

           Enhancement layer만 독자적으로 디스플레이되지는 않으므로 있을 필요가

            없다. 만약 pan-scan이 사용되면 lower layer의 정보를 이용한다．



       (j) Slice header
           （加antiser-scal乞code만을 제외하고는 lower layer와 동일하다．




5.4.2. r＼爪그croblock
        Scalable_mode가 " SNR scalability" 일 따I er血an啣nent layer의 데이타는 lower layer

      의 데이타의 정세도를 높이는 데이타일 뿐이므로 macr아六姚J끄玘 중 macr的1o火

      _inira, macrobk乂k_motion_f야ward, macrobli乂k_moti이i_backward flag는 0만 허용된다．



  S     dctjype
        Syntax의 변수 dct_type은 어느 layer의 macroblock_m녔e( ）에도 나올 수 있다．

      만약 동시에 두 layer어］ 나타나면 두 변수값은 같아야 한다．



  S     Skipped Macroblocks

        Macrobli乂k은 다른 layer의 해당 macrobl아：k의 skip 여부에 관계없이 독자적으

      로 skip될 수 있다．
234
       世브
      5.4.3, 텨ock


        N     7／끈／장복호 (Va／幻ble Ien刃h decodi,切

              5.1.1에서와 같이 디코딩된다．



        I     역스캔 (Inverse scan)

              5.1.1에서와 같이 디코딩된다．



        I     역양사화 (Inverse quar坑刃加n)

              Non intra bic乂k어］ 대해서는 5.1.3에서와 같이 디코딩한다. 만약 佃wer layer가

            入4PEG1을 따르는 bitstream이면 F"lo比rtv][미를 얻기 위한 " mverse quantisation

            arithmetic " 은 入'IPEGi어］ 규정된 불일치제어帥smatch con甘ol)를 따른다．



        I     두 可刃꺼의 계수들의 합샨

              각 ]ayer의 벼ock들이 더해져 c（玘ificients F" 를 만든다．



                            尸［v]［비 = F"lower[v][u] + 尸enhance[v]［비，    幻rafl 나V


             만약 chroma _simulcast가 사용되면 luminance bl（乂k만이 위에서처럼 사용되고

            chrominance 비ock어］ 대해서는 base layer으IDC값이 enh出icement layer의 DC값을

            예측하기 위하여 사용된다. 반면에 AC값은 base layer의                             AC값을 버리고
            enhancement layer으1 값만으로 구성된다．



             尸'{O]{O]   =         F"lower[O][O} + F"enhance[OJ[O]
             尸［v]［비     =        F''enhance[v][u],

                                                               幻rail 나 v except u=v=O
                                                                                   235




    Chr아nas油毗ast bk兀k은 chrom血ance non-inira m汕奴를 사용하여 마치 non七l甘a

   bk乂k인 것처럼 역양자화된다． 표 5-35는 그 block의 DC값이 enhancement layer의

   DC값을 예측하기 위해서 사용되는 lo＼比r layer chrominance block의 mdex를 나타

   낸다．


         표5-35 block index used to predict DC coefficient (MPEG IS : Table 7-27)
                                                 bli岫index
             chi기月na format     4   5      6      7     8      9      10    11
                base: 4:2:0     4   5      4      5
                 upper: 4:2:2
                base: 4:2:0     4   5      4      S     4      5      4      S
                 up休r: 4:4:4
                base: 4:2:2     4   5      6      7     4      5      6      7
                 upper 4:4:4




5.5. 시간적계위 (Tempor이＄calab咐y)
    Tempor띠scak由小ty는 그림 도20과 같으나 언뜻 봐서는 잘 이해가 가지 않는다．

   이 tempor고 scalab血ty는 말뜻 그대로 ei血a毗ment layer를 추가해써 시간해상도를

   높여주는 것이다. 즉 lower layer와 enhancement layer의 공간해상도는 같다．

   Enhancement layer의 디코딩과정은 reference 什ame을 어디서 가져오는가 하는 문

   제만 빼고는 기존의 디코딩과정과 동일하다. 즉 temporal Sc키ab小ty에서는

   reference frame은 이血ancement layer 내에서 가져올 수도 있지만 lo毗r layer에서도

   가져올 수 있다. 이는 reference_select_c에e어］ 의해 달라지는테 P-picture와 B-

   picu止e에서의 referenc乞＆en乞配lection은 표 5-36, 5-37과 같다. 여기서 한 가지 유

   념하뱌 할 것은 B-picture에서 backward prediction의 reference frame은 enhanement

   layer에서 가져오지 않는다는 것이다. 즉 lower layer나 enhancement layer으1 전

   (previous) fran妃에서 가져온다. 따라서 enhancement layer에서의 B牡跏re는 P.
      MPEG
236   川DEO




        picture처럼 동작하며 enhancemant layer에서 fran叱을 재배열할 필요는 없다． I-

        picture에서는 예측을 사용하지 않기 때문어］ 이것을 표시하기 위해서 I-picture의

        reference_select_code를 "11" 로 한다．


                         표 5-3o 다e<永少ion references s이e베on in P利ctures
                                    (MPEG IS : I야)Ie 工28)
                        refei꾀we 眺佃：tcode      forward pred油on i七蛇rei孔e

                                         00    入4哨trec止d町月ed enhanc口nent picture6)
                                         01    Most recent lower layer frame mdisplayoiiler
                                         10    Next lower layer frame in display order
                                         11    forbidden




                         표 5-37 다e<계c加n references selection in 먀)ictures
                                     (MPEG IS : I야긔e 7-2)
                          forward predi出on re佃ence                       ha（永wardr毗diction I七佃ence




                   00     白由idden                                        白由idden
                   01     Most此cent deco出 enhan(氾毗nt pi山呵s)              Most recent lower layer picture in
                                                                         display order
                   10     Most re七nt dec뇌ed enhancement picture(s)       Next lower layer picture in display
                                                                         order
                   11     Most recent lower layer pict띠e in display      Next lower layer picture   in display
                          red町                                           order
                                                                                       237




                     Lo니／er Lay竺 1. -
                        Bitstrmm)r




                 Prediction
                Field石ram台＋
                 Selection
                            Framestore
                            Addressing                  "帥 "
                                                                \
                                                               tore51J
                     i'ec加巾］[s］固              A
                                   \\\\




                Additional                   Sc꾜ing
                Dual-Prime       >         for Colour
                An出metsc                  Component:

                    A            vec加）中作l玎


                                             Haif-Pel
         Fr·쁘－니    Vector
                                                Info.
      itstr田m r 1 Decod끄ig




                 솥           Vec切r
                             Predictors                                  \
                                                                                Deco（妃d
                                                                             > ;=a乙
                                                                                 LiLpLC"
                                                                                 d.
   그림 5-20 Simplified motion compensation process for the enhancement layer u섧ng
                      ten갸兀n계sc（게야네作y (MPEG IS: 디（jure 7-16)




5.5.1 . 변경되는 신택스 구조
     이는 把mporal scalab小ty를 이용한 경우 enhancement layer에서 가지는 제한값들

   을 정리한 것이다.           Sequence_scalableHex妃nsion의 layerjd를 읽어서 두 layer간의

   구분을 한다. 만약 두 bit打earn이 연속적인 layer-id를 가지면 id값이 큰 쪽이

   enhancement layer이다．
238




      (a) Sequence header

          Horizont키_size_value, vertical_size_v出ue, asp凹tT帥O血formation을 제외하면

          lower layer와 다른 값을 가질 수 있다．

      (b) Sequence extension

          Profile and level indication, bit rate extension, vbv buffer size extension,   low

           delay, I始m乞rat乞炚把nsion_n, frame_ra妃exten計on4d을 제외한 값들은 lower

          layer와 동일한 값을 갖는다.                 Pro얍es鈿乞sequence는 enhancement layer의

          Sc跏rung 凡mruat만을 나타내고 remultiple疝增한 후에 출력되는 video의 scan

          format을 나내는 것은 아니다. Remultiplexing 후의 출력 如mruat은 sequence

          scalable extension의 mux to까ogressiv乞sequence로 알 수 있다．

      (c) Sequence display extension

          Enhancen妃nt layer만을 따로 디스플레이하지는 않으므로 이 ex佃sion은 존

          재하지 않는다．

      (d) Sequence Scalable extension

           이 extension의 sc따的le中n好le가 "Temporal scalabiity'로 된다. I斗ogressive

            sequence=0이고，       mux_to_progressive_sequence=0일        t대    top_fl叱小rst오｝

          pic恤之m以fa아아는 허용된 어떤 값도 다 갖는다. I거rogressive_sequence = 0

          이고, mux_to_progressive_sequence = I일 1대 top_field_first는 lower layer의

          tOp五eld小fir眺의 보수가 되고 picture_muc_fa아아는 l이 된다. I거rogressive_

          sequence = 0이고，mux_to_progressive_sequence = 1일 t대 top_field_first는 0이

          되고, pictur乞muc_fa아야는 허용된 어떤 값도 다 갖는다．

      (e) GOP header

          GOP header에 대한 어떠한 제한도 없다．

      (1) Picture header

          Picture header에 대한 어떠한 제한도 없다．
                                                                    MPEG
                                                                    피DE0     239




   (g) Picture coding extension

        Top_field_first, concealment_motion_vectors, chroma_420_type, progressive

       frame을 제외한 모든 값은 lower layer 와 다른 값을 갖을 수 있다. I叩

       1 fie넌上rst는 progres啣e記quence와 mux to皿四ressive_s텍U毗叫］ 따라 결

        정되고 conce심ment _m曲on v毗아는 0이 되어야 하고, Chrom之仁0口PC은

       lower layer와 같아야 하고 pr魄ressive玉ame은 pro얍es如乞sequence와 같은

       값을 갖는다．

   (h) Picture temporal scalable extension

        각 picture어］ 대해서 존재해야 한다．

   (i) Quant matr奴 炚帥駐이l

        존재할 수 없다．




5.5.2, 시간적계위에 대한 권고사항
   Temporal reference는 lower layer와 enhancement layer어］ 관꼐없이 가장 최근어］

  디코딩된 layer로부터 하는 것이 좋다. 또 만약 GOP header가 자주 있어서

  ten叩oral reference가 혼동될 염려가 있을 때는 system layer의 타이밍 정보를 이용

  하면 좋다．
      MPEG
240   VIDE0




  5.6. D아a pariti아ting
          Data partitior血평은 vid的bitstream을 partition해서 두 개의 layer로 나누는 기법이

        다. 그림 三21처럼 어떤 pnority breakp여nt어］ 의해서 데이타를 partilion 0 （또는

        high p加血y partition)과 partition 1（또는 low priority pai奴如n)로 나누는더1 이러한 기

        준인 prio血yb妃akpo血는 표 5-38과 같은 것들이 있다．Partiti이ii에서의 sequence,

        GOP, picture header는 에러발생시 회복을 위해서 pail址on 0와 동일한 값을 이용

        하고 역시 sequen凹end c넘e도 들어간다. 또한 partition 1의 모든 field도 역시

        partition 0의 것과 동일한 값이 들어간다. 한편 pail的on 1에서 허용되는 extension

        들은sequence_extensionO, picture_coding_extensionO, sequence_曲lable_ extensionO뿐

        이다. VBV의 개념은 전과 동일한데, 한 개의 partition만이 아니고 두 개의

        bitstream을 합쳐서 생각한다. 즉 bit_rn妃, vbv_bu什erHS切e, vbv_ delay는 두 개의

        partition에서 동일한 값을 가지며 위에서 언급했듯이 2개의 paIl的on을 합한 값을

        이용한다（즉 data pail虹on을 쓰지 않을 경우와 동일하게 한다）. 복호과정은 다음

        과 같이 변경된다．



          (a) Current_partition을 0으로 하고 partition 0 (sequence乳ala川乞以啣Ision을 포함

              함）의 디코딩을 시작한다．



          (b) Curr口1tI坦rtition이 0이면 현재 디코딩하려는 부분이 priority breakpou止인지

              조사해서 참이면 partition 1에서의 다음 뎨이터를 디코딩하고 만약 거짓이

              면 part沁on 0의 디코딩을 계속한다．



          (c) Current_partition이 1이면 현재 디코딩하려는 부분이 priority breakpoint인지

              조사해서 참이면 partition 0에서의 다음 데이터를 디코딩하고 만약 거짓이

              면 1用rtition 1으1 디코딩을 꼐속한다．
                                                                      S
                                                                       MPEG
                                                                       피DE0     241




                      Quarit   DC     DCT                DCT
                                                                  I：님I七tion 0
                                               ID口
                      Scale    coeff coeff 1   1coeff
                                                        coeff 1




                                                                  Partition 1




그림 5-21 A segment from가y怡tream with two p帥tions, 니尉나)riOrity bre아4:X加tset
              幻 64 ( one（띠n,level）口（升 ). 小e Iwo F刃巾的ns are shown,
wiTh arrows indicating how the decoder needs to swftch bet八／een partitions (MPEG
                                  IS: Figure 7-17)
242




                     표 5-38 P的rity bre야（口oint v이ues and as鉤ci아ed semantics
                                      (MPEG IS 汁（그ble 7-30)
      pn이祉y_breakpoint     Syntax elements induded in partition zero

             0             This value is 肥Served for partition 1. All slices in partition 1 sh出l have a
                           pn어幻b代akpoint텍ual to 0.
              l            All data at the sequence, GOP, picture and sliceO down to extra_bit_slice in sliceO.
             2             All data included above, plus macrobl乂k syntax elements up to and including
                           macroblock address increment
             3             All data included above, plus macrobl乂k syntax elements up to but not including
                           a넜ed b!以：k나：,at出mO.
           4 ...63         Reserved.
             64            All syntax elements up to and including coded_block_pattem() or DC coefficient
                           (dct_d口d出毗ntial), and the 丘匹t (nin, l四래 1X그 c（比fflcient pair (or EOB).
             65            시isynt缸 elements a蜘ye, p加sup to 2 (ron, le比!)DCTc沛ci帥 pal八．


            63+j           All synt炚 elements above, plus up toj (run, level) DCI
                                                                                ' coefficient paha.


            127            세 syntax eleme毗 above, plus up to 64 (run, 1ev에 DCI' coe術c把ntpairs.




  5.7. 복합계위（Hybrid scalab咐y)
       Hybrid scalab小ty는 앞에서 언급한 것 중 2개의 서로 다른 sccalab小ty를 결합하

      는 것을 말한다. 따라서 이렇게 2개의 scalability가 결합될 It가 layer는 표 5-39와

      같이 3개가 된다．


                          표 5-39 卜k그mes of Iaye匹 (MPEG IS : table 7-31)
                                         layer_id           name

                                             0              base layer
                                             l               enhancem三nt layer 1
                                             2               enhancement layer 2
                                                                 243




     助hanc帥ent layer 2개를 가지고 볼 1'11 enhance毗nt layer 1이 lower layer이고

enhancement layer 2가 enhancement layer가 된다. 어떻게 디코딩하느냐 하는 것은

어떤 Sc띠ab小ty들이 결합되었냐에 따라 다른더1 여기어］ 2개의 예를 들어 설명한

다．
        CASE! :

           base layer

              <spatial or t巴mporal scalab小ty>

               enhancement layer 1

                         < 針恨 seal的ffity >

              enhancement layer 2



       CASE 2:

            base layer

                         <SNR scalab小ty>

              enhancement layer 1

                         <spatial or temporal scalability>

              enhancement layer 2



     CASE 1에서는 base layer를 먼저 디코딩하고 er血anc아rient layer 2개를 동시에 디

코딩한다． 또한 CASE 2에서는 base layer와 enhancement layrer 1을 동시에 디코딩

한 후 enhancement layer 2를 디코딩한다．
244




  5.8. 복호화된 출력의 형태
           디코딩과정을 거쳐 최종적으로 출력되는 형태는 progressive_frame, rei玘at_first

      _field, t아Lfield fi胤어］ 따라서 달라진다. 이들 각 경우어］ 대한 출력형태를 알아보

      자．
           (a) pn）얍essive_sequen凹＝ 1인 경우

             예를 들어 chroma_format이 4:2:0인 경우는 그림 5-刃와 같다．




                                                        XUX 乂OX XUX 乂OX   XU乂 M
                                                                              A口乂 XUX XUX


                                      냐1 竹aree period
                                         =1/丹띠ne rate

                   그림 5-22 progres섧ve_sequence == 1 (MPEG IS: Figure 7-18)
                                                                                                                                                  245




(b) pro留essive_sequence = 1이고                                     le件叱鈿t_field =1인 경우 Chroma的nnat이
    4:2:0인 경우 그림 5-23과 같다．




                                                                                       n
                                                                                       nn口
                                                                                        旒me period
                                                                                       =1/frame rate




                        Xn乂 Xn又 XO又 乂n又         乂O乂 Xn又 XO又 XO乂
                                                                        丙
                                                                                                                                              貢
                                                                                                                                          X
                                                                   XO又 X 8 O 乂 ＝              乂n又 呑 又 肖 乂 뇨
                                                                    乂
                                                                                                                                      9
                                                                                                                                  X
                                                                                                                              O
                                                                                                                          乂
                                                                                                                      貢
                  ＼나＼
                                          YH/
      top_fl日d.1丘rst:                     0
                                                                                                                  H
                                                                                   1                          0

        그림 5-23 progressive_昑quence== ]. repe아fi田tfield=]
                       (MPE（引S :日（그ure 7-19)



(c) progress加乞記quence =0인 경우

  II如riaced羽叩ence인 경우의 휘도신호는 그림 5-24와 같이 출력되는더］ 색신

  호는 pro얍essive_fran妃값어］ 따라 그림 5-25와 그림 5-26과 같이 달라진다．
246




                                 ><                 ><                    ><
                                           ><                 ><                   ><
                                 >(                 >(                    X
                                                              x                    x
                                                                          ><
                                                                                   x
                                                                           x
                                                                                   x




                                                          且可ne pthocl
                                                         =1/frame rate


                그림 5-24 progressive_sequence =0                         (MPEG IS: Figure 7-20)



       그림 5-25, 5-26에서 보듯이 pro얍eS鈿e卞丘an妃이 l인 경우의 색신호는 휘도신호

      의 첫 번째 field가 출력되는 시간어］ 모두 출력된다．




                       5              乂         즈        x
                                                                   )<
                                                                               9
                                                                                        ><
                                                                                                      5
                       >(
                                                     ：乂

                       25             ><                 ><
                                                                   ><
                                                                               딪
                                                                                        ><
                                                                                             ><
                                                                                                      25
                       乂
                                  딪             즈        x         乂           딪 「           9        '
                      뇨1J                   뇨-       Y1U                    뇨Yq'             뇨＼1
        progressive.-.fr缸ne: 0                           1                         1              0


                 그림 5-25口rogress卜／e_sequence ==0\A／什h 4:2:0 chromin（그nce
                                  小/IPE（引S :日gure 7-21)
                                                                      MPEG
                                                                      피DE0   247




                            gggg=
                                               O 酌 因 O 8O 욘
                                  ><


                                   x




                                                  O
                                                  1
                                   X
                                                                      因
                                           乂



                                   X Yl
                                           나
                                                                  1
pro greSsive_竹ame: 0                                          l


    그림 5-26 progressive_昑quence == 0 with 4:2:2 or 4:4:4 chrominance
                        (MPEG IS: Figure 7-22)
6
    MPEG VID日p

    H I " 파일 과
    레벨
250




 6. 프로파일과 레벨

       入4PEG2어］서 정의하는 prof끄e과 level의 의미는 일반적으로 우리가 생각하는

      의미와는 차이가 있다. 入'IPEG2에서는 매우 다양하고 융통성 있는 video bitstream

      의 synt炚를 정의하고 있다. 이 다양성과 융통성은 header, extens幻n 등과 기타

      부가정보에 의해 이루어지는더］, 이 전체 syntax의 일부로 정의되는 syntax를

      profile이라고 한다.   한편 각 profile에서는 최대 영상의 크기, 최태 bit-rate 등

      bitstream에서의 변수어］ 대한 제한치들에도 차이가 날 수 있는더］, 이 제한치들의

      정의된 집합을 1ev이이라 한다．

       MPEG2에서는 적합성（con伽伽nce) 여부를 이 pr可끄e과 level의 형태로 정의하

      는더1, 그 결과 서로 다른 응용분야에서 bitstre카n을 교환하여 사용할 수 있다.

      따라서 이 MPEG표준에서 정의하는 bits仕earn synt砥를 구현하고자 하는 이들은，

      같은 profile/level에서 생성된 bits甘earn은 서로 다른 응용분야라 해도 교환이 가

      능하도록 하여야 한다. 이 표준에서 정의한 profile과 1ev이이 모든 제한치들을

      정의하는 것은 아니므로, 정의되지 않은 값들은 허용된 범위 내에서 어떠한 값

      을 사용하여도 무방하다. 일반적으로 어떤 profile/level에서 허용하는 모든 변수

      들의 모든 제한치들을 디코딩할 수 있는 디코더는 그 profile/level어］ 적합

      (conformant)하다고 한다. 하나의 예외가 존재하기는 하는더］, Simple profile 入4am

      level의 디코더는 Mam profile U叭v 1ev이의 bits甘earn을 디코딩할 수 있어야 한다．

      따라서, 허용된 값의 범위를 넘지 않고, 허용되지 않는 변수들을 포함하지 않은

      bitstream은 적합（con的rmant)하다고 한다.   Pr而le과   level을 나타내는 변수는

      sequence_炚妃ns幻n어］ 있는 profile_and_level血넌ication이다． 이 변수내의 비트들의

      의미는 표 6-1어］ 정의되어 있다.       Esca꺄Hbit가 0인 경우는 profile과 1ev이이 표

      6-2와 표 6-3어］ 기술된 것과 같은 의미를 갖는더］, identification 번호가 작은 것이

      큰 것을 포함한다. Escape_bit가 1인 경우는 profile과 1ev이이 표 6-4어］ 보인 것처

      럼 proffi乞and_le比1_mdic的on이 Escape_bit가 0인 경우와는 달리 계층적인 구조
                                                                                  251




를 갖지 않아, profile과 level이 반드시 다른 것들의 부분집합은 아니다．


               표 6-1 Meanning of b汁引n pro셰e_andJeveLindk갓카ion
                             (MPEG IS : Table 8-1)
  Bus     FieldSi；配（bits)           入lean加g
  [7:7]   1                         Escape bit
  [6:4]   3                         Pmflle identification
  [3：이    4                         I尤ye! ident而cation



                  표 6-2다애e identifica如n (MPEG IS: Tc그ble 8-2)
          Profile dentifii'iton

                                                                     (reserved)
                                                  Simple
                                                  入'lain
                                                  SNR Sc沚的le
                                                  Spati세y Scalable
                                                  High
                                                                     (reserved)



                  표 6-3 Level iden桁匕에（Dn （卜기PEG IS : Table 8匈
          I七vel identifies岱Dfl                    I尤vel




          표 6-4 Esc（그口e口R＞톄e_andJeveLindk刃化n identification
                         (MPEG IS : Table 8-4)
              proflleandJevel_indication           Name
              10000刃0 to 11111111                                    佃sei叱d)
252




  6.1. MPEG］과의 호환성
       MPEG1에서는 영상의 크기나 picture rate 등 몇 개의 변수들이 정해진 값보다

      작은 경우, 그 bits仕earn을 제한된 변수（con血汕edp啣neter) bitstream이라 부르고，

      constrained_i刃rame把rs寸fi明를 1로 놓는다.     入iIPEG2의 모든 皿ofile과 level에서는

      入IPEGi의 제한된 변수((刃nslra血ed parameter) bit缸earn을 디코딩할 수 있어야 한다．

      入4PE(끄의 제한된 변수 코딩에 적합(conformant)한 bitstream이 생성될 때는

      羽叩en凹上eader에 있는 constraii妃d.j刃rameters_flag를 1로 셋팅한다. 또 入作EG2의

      모든 profile에 해당하는 디코더는 MPEG!의 D拉cture만이 존재하는 bitstream이

      디코더의 level 제한치 내에 있는 bit毗earn이라면 디코딩할 수 있어야 한다．




  6.2. 프로파일들 간의 관겨1
       MPEG2의 모든 proffle들 간어］는 계층적인 구조가 존재하여, 상위계층의

      proffle을 갖는 디코더는 하위계층의 pr而le을 갖는 디코더가 생성한 bitstream을

      level어］ 콴계없이 디코딩할 수 있어야 한다. 같은 proffle 내에서는 level어］ 관꼐

      없이 같은 syntax 집합을 갖는다. 계층의 순서는 표 6-2에 있다． 각 pr而le에서

      변수들은 표 6-5와 같은 범위에 한정되는더］ 이를 간단히 살펴보기로 한다. 모든

      profile에서 chroma_f아mat 4:2:0를 허용하고,     4:2:2는 I五gh proffle에서만 허용되며

      모든    pr而Ic에서     加me_rate_ex妃的on_n,    framlle_rate_ext己nsion小d,   asi玘Ct ratio

      i址ormation의 제한 범위는 동일하다. I万CtU肥下odin且竝꺄은 simple皿而Ic에서는 I, P

      만 허용하고, 나머지는 I, P, B 모두 허용한다. R다玘at first侃id는 罰mple profile과

      入4am1l prof配에서는    제한을 두지만 SNR proffle            이상에서는             제한이     없고

      sequen此_scalable小cx把ns油i()은 SNR profile 이상에서만 존재한다． 또한 SNR proffle

      은 scalable_mode로 SNR 한 가지만 가질 수 있지만, spatial profile과 high皿而Ic은

      SNR과 spatial 두 가지를 모두 갖는다. 따라서, pictur口叩a寸斗alable _extension()
   은 spalial prof끄e과 highpr而le만이 갖게 된다. hi曲dc下recision은 모두 8, 9, 10의

   값을 가질 수 있고,               high profile은 11의 값을 가질 수도 있다. 그리고, 모든

   proffle의 sli凹_structure는 res出cted이다．


                   표 6-5 Syntacflc consir이nlS of pro쇄es (MPE（引S：化ble 8- )
                                                               I뇨疝Ic
      S弘a c mm姓it             Sim艸e            A1ain           SNR           Spalial           碼典
chro也1 format                  4:2:0            4:2:0          4:2:0          4:2:0        4:2:2 or 4:2:0
framct긔此e ext印sion n             0                 0             0              0                0
framei긔此ee光tei岫［乂id              0                 0             0              0                0
呵心tra由Jnfonna毖咀l            0001, 0아0,       0001, 0010,    0001, 0010,    0001, 0010,      0001, 仄아0,
                               0011             0011           0011           0011             0011
I由比ure cod뇨g－勺I比               I. P            L P. B         I,P, B         L P. B           I,P, B
l却cati岫L羽d                            ConatnhTh너                           Unconstrained
田끼出毛駐月lable                     No                 No          Yes            Yes               Yes
exten立片10
恥川a汕e mode                                                     SNR           SNR or        SNR or Spatial
                                                                             S-
［由：hllt卞SFmdalHS（田lable         No                 No           No            Yes               Y哨

日tel岫［)nO
自titra_dcj耐i如l                8, 9, 10         8, 9, 10       8, 9, 10       8, 9, 10       8,9, 10, 11
g作十 帥1기C佃1七                                                  Restricted
                                                             S（配 6.1.2.2




      모든 pr曲le들에서 한 macroblock어］ 대한 비트랑에는 표 6-6에 정한 것과 같

   은 제한이 있다. 이 값은 DCT 후 각 계수를 12비트로 표현했을 11가, block의 수

   와 block 내의 계수의 수를 고려하여 정한 것이다（예를 들어, 4,608 = 12x8x8x6).

   그러나, 한 slice에서 최대 두 개의 macr的1(兀k의 비트량은 이 값을 초과할 수

   있다. 한 macr아加ck은 macr的k兀k ...adcl心乞in口ement의 첫 비트로 시작하고, 마지

   막 coded bli乂k의 "End of Bk乂k' syr毗oI의 마지막 비트나, coded b뇨火이 없을 경우，

   coded小1(乂k中attemO의         마지막           비트로            끝나는         것으로       간주된다.           따라서

   macr的kx永의 앞에 있는 slice(）를 나타내는 더］ 쓰이는 어떠한 비트도 macro bk兀k
254




         의 일부로 간주되지 않는다. High pr而le은 표 6-5어］ 보인 것 외에도 luminance

         sample ra把, maximum bit ra把, VBV bu珏er size 등에서도 다른 proffle들과는 차이를

         보인다．


              표． o-o卜爪그川mum number of b汁引n a macroblock (MPEG IS : T야)Ie 8句
                            chroma fonnat        入aximum number of bits

                                4:2:0                    未刃8
                                4:2:2                    6144
                                4:4:4                    9216




          자세한 것은 표 6-12, 6-13, 6-14를 참조하키 바란다. sP＠八ilL의 디코더는

         MP@LL의 bit毗eam을 dec어妃할 수 있어야 한다．




      6.2.1. repe아＋佈St섀이d의 사용
          罰mple profile과 Main proffle의 bits甘earn어］서는 repeat_f的field가 표 6-7어］ 보인

         것처럼 제한을 갖는다.         MP@h孔과 SP@ML에서는 다음과 같은 부가적인 제한

         이 있다．

            (a) vertical寸釘ze가 480보다 큰 B-1丘cture에서는 repeat_first_field가 0이다．

            (b) vertical_si配가 480보다 크면 fran妃rate는 251也가 되어야한다．
                                                                             255



           표 6-7 Cons枳ints on use of repe아first fi이df아 Sin耳긔e and Main 다애e
                                  (MPEG IS : Table 8刃
                                                 pn增 鈿ye        Pr'名1捕1Ye
                                                 se(私en（肛네1     就quenc作＝1

    fran肥 rate (X넘e   丘a끄配mte value              re心也I岫LfieId   rep凹t丘鹵小日d

                      fothidden
                      24000/ 1001     (23.976)   0              0
    0010              24                         0              0
    0011              25                         0orl           0
    아00               30000 / 1001    (29.97)    0 or 1         0
    0101              30                         0（兀 l          0
    0110              50                         0 or 1         0
    0111              60000/ 1001     (59.94)    0 or 1         0orl
                      60                         0 or 1         0orl


    1111              reseived




6.3, 레벨 간의 관겨1
    I刃w, 入4am1l, High-1440, High level들 간에는 계층적인 관계가 있다． 따라서 상위

   level의 parameter 제한치들은 하위level의 parame也r 제한치들보다 큰 값을 갖는

   다. 예를 들어, MP@ML의 디코더는 MP@LL의 bit없ream을 디코딩할 수 있어야

   한다. 계층의 순서는 표 6-3에 나타나 있다. 각 level에서의 변수들의 제한치들

   은 표 6-8어］ 보인 것과 같다. 이중 유의할 점만 살펴본다．
      MPEG
256   V山E0




                          표 6-8 Part了re怡rcon計raints for levels ( MPEG IS : Table 8-8 )
                                                                                         I士vel
                        Syntactic El帥ent                      I刃w             Main           Hi小-1440            H帥1
        f_code[0][0] (forward hori끼川al)                       [1:7]            [1:8]               [1:9]         [1:9]

        f_code[1][0]*(ba吐ward hori기Xltal)                     [1:7]            [1:8]               [1:9]         [1:9]

        Frame picture
        f_code刈[1] (forw띠d vertical)                          [1:4]            [1:5]               [1:5]         [1:5]

        f_code[1][1］京（ha永ward veili（沁）                        [1:4]            [1:5]               [1:51         [1:5]

        verti(月lv仗b)r range十                                [-64:63,5]     [-128:127,5]      [-128:127司       [-128:127,51

        Field picture
        fc넜d이［1]（白rward vei岱川）                                [1:3]            [1:4]               [1:4]         [1:4]

        f_code[1]L1J*(backward vertical)                      [1:3]            [1:4]               [1:4]         [1:4]

        vertical v炚tor i日uge卞                               [-32:31,5]      [-64:63,5]           [-64:63,5]   凹中63,5]

        frame rate code                                       [1:5]            [1:5]               [1:8]         [1:8]

        San긔？le Den曲137                                                          Seelable 6-11
        Luminance Sa째le Rate                                                     Seelable 6-12
        Maximum Bit Rate                                                         See Table 6-13
        Bul脆r Si配                                                                SeeTable 6-14

                               民r Simple pmflle bits出amswh岫 面 n아mc뇨de B-pie吐es,
                           backw川mhorizon目 f c넋e and b玭wanlverlicalf_code sh出l be set to 15 (not used).

                           十    This restnction applies to the final 代consinicted motion vector, In the case of dual prime
                           motion vec幻rs it由is restnction applies to a끄 the following values:
        vector'[O][O][I]
        ((vect까'[0110111/ 串 刃伽art力口爬fit凹'it）냐批刃i2)
        伽edi마'[0110)11/ 水 刃tip口ri砂J（刃／까mb냐7red]上尼)-i-e[parit)乙r可끄p口月DJ批dl
        ((vector'[01[01[1] * m[parisy_ref][parizyj,red])/12)+d[小｝ivector[1]
        伽ec切'[0)10끄1] 水 m[j싸it)乙r明／pa月D나才ed川끼杷加antyr可끄j九汁口批dJ＋功加配沙／11




          f_code[l][O］과 f_code[1][1]은 backward motion vector어］ 관계되는 f_code인뎨，

       Simple pr而le에서는 B肛cture가 없어 backward motion이 없다. 따라서, simple

       pr而le에서는 f_code[1J[O],                   f_c（넜e[1][l]의 값이 모두 15로 se出ng된다促code 15는

       그 f_code가 사용되지 않는 것을 의미한다）. 1亐cture구조가 frame picture인지, field

       picture인지에 따라 vertical motion vect아의 범위가 달라진다. Field picture의 motion

       크기는 &ame picture의 motion 크기의 반이므로 표6-8어］ 보인 것처럼 motion

       vector range가 frame picture의 반이다. 그리고, 이 제한범위들은 마지막 복원
                                                                               257




   motion vect야들에 대해 적용된다. 한편 dual pi如ie motion收毗아에서는 주의할 것

   이 하나 더 있다. 이는 （如nV가 더해지기 전에 mot幻n比아아의 스케일링이 필요하

   기 때문이다. 그러므로 스케일링（Sc띠血g）을 하기 전과, 하고 난 후 dr四가 더해

   진 후에 표에서 정한 대로 vect야의 범위에 제한을 두어야 한다．




6.4. 계위층 (Scalable laye向
     Scalab皿勺는 하나의 복원 video sequence를 만들기 위하1 두 개 이상의 bi始仕earn

   을 사용하는 것을 말한다. 따라서, SNR scalable pr而Ic과 spatial scalalbie profile,

   high profile에서는 하나의 video sequence어］ 두 개 이상의 bitstream을 만든다． 이는

   bitstream이 layer구조를 갖는 것을 의미하며, 하나의 layer어］ 의해1 얻어지는 복원

   화질보다 좋은 화질을 얻을 수 있다. Profile별로 가질 수 있는 최대 layer의 수

   가 표 6-9에 나타나 있다．


    표． -9 U口口er bounds for scal(泌)le laye囚inSNRSc이able, Spatial Sc이（士)le（그nd H납）
                              ofile (MPEG IS : Table 8-9
                                                            I뇨嗣［e
       I尤vel          Maximum Number of               없나R     Spatial    ffigh

        H自帥                시l 切口s (base + enh.)                           3
                        Spalial enhancement layers                         l
                         SNR enhancement layers                            l
      H帥-1440              All layers (base + enh.)             3         3
                        Spa出al enhancement layers                l         l
                         S寸R enhancement layers                 1          l
        八laln              사I layers (base + ei血．)     2                  3
                        Spatial en떠ncement layers      0                   l
                         SNR enhancement layers        l                   l
        I力w                 A끄［layers (base + enh.)    2
                        Spatial enhancement layers     0
                         S卜R en떠ncement layers         l
258




           Spatial scalable profile과 노gh proffle은 SNR scalable pr而le을 포함하기 1대문에

         SNR er血an凹ment layer를 가질 수 있지만，SNR scalable pr曲le은 spatial enhancement

         layer를 가질 수 없다. 그러므로，SNR scalable pr而le에서는 최대 layer의 수가 2이

         지만 Spatial sc심able prof配과 I五ghpr可配은 3이다．




      6.4.1. 허용가능한 layer들의 조합
           Scalabili口를 사용하는 pr曲le에서 scalabili口의 조합은 다음과 같은 규칙에1 의

         해 이루어지므로, 허용되는 조합이 있으며, 이는 표 6-10에 잘 나타나 있다．
                                                                                           259



               표 6-10 Perry宿솨ble layer combina恢＞ns (M昨G IS:I야扼＆10)
                                                                           Prt寸lie/ level
                                   S（늬11升ble mode                      （寸曲mm昑tba配切yer
                                                                               d텨oder
pn刈le                  Ba舵lay町      Enh. layer 1      Enh. layer 2     (level z娥.1伽layer) 方
      SNR               4:2:0        SNR, 4:2:0                           MP@凹me level
 S-                     4:2:0        SNR, 中2:0                            MP@凹me level
 Spatial                4:2:0       Spatial, 4:2:0                        MP@(level- 1)
 Spatial                4:2:0       sr旺（4:2:0         Spatial, 4:2:0      MP@(level- 1)
 Spatial                4:2:0       Spatial, 4:2:0     sy旺（4:2:0          MP@(level- 1)
      Fligh             中2:0                                              HP@same level
      I五gh              4:2:2                                             HP@same level
      I五gh              4:2:0        SNR, 4:2:0                           HP@sa玘 level
      I-五gh             4:2:0        sy寸R, 4:2:2                          HP@same level
      I五gh              4:2:2        sr寸R, 4:2:2                          HP(＠町ne level
      F五gh              4:2:0       Spatial, 4:2:0                        HP@(level- 1)
      High              中2:0        Sp刊ial, 4:2:2                         HP@(level- 1)
      High              4:2:2       Spatial, 4:2:2                       HP＠伽妃1- 1) 十
      I五gh              4:2:0        SNR, 4:2:0       Spatial, 4:2:0      HP@(level- 1)
      High              4:2:0        SNR, 4:2:0       Spatial, 4:2:2      HP@(level- 1)
      High              4:2:0        SNR,4:2:2        Spatial, 4:2:2     HP@(level- 1) 十
      High              4:2:2        sr旺（4:2:2        Spatial, 4:2:2     HP@(level- 1) t
      Hi帥               4:2:0       Spatial, 4:2:0     SN艮4:2:0           HP@(level- 1)
      High              4:2:0       Spatial, 4:2:0     sr寸R, 4:2:2        HP@(level- 1)
      I五gh              4:2:0       Spatial, 4:2:2     SNR, 4:2:2         HP@(level- 1)
      I五gh              4:2:2       Spatial, 4:2:2     SNR, 4:2:2        HP@(level- l) t




(a)           SNR scalable pr而le은 최대 layer 수가 2, Spati띠 scalable pr可끄e과 HIgh

              pr曲le은 최대 layer의 수가 3이다．

(b)           3-layer 조합에서 SNR enhancement layer와 spatial enhan啣nent layer는 하나

              씩만 허용되며, S卜JR/spatial 또는 spatial/SNR의 순서가 허용된다．

(c)            Lower   layer의    c뇨oma니如rmt이         4:2:0인     경우, enhancement layer의

              chrom乞format이 4:2:2라면 SNR scalable pr而le과 spatical scalable proffle중

              어느것이라도 SNR enhancement를 허용하는 것이라 간주한다．

(d)           I乂）wer layer의 chroma_f이mat이 4:2:2인 경우, enhancement layer의 c뇨on俎

              format은 4:2:0이 될 수 없다．
260




        표 6-10을 간단히 설명한다. 표의 최우측단은 가장 간단한 형태의 base layer

      dec어ler의 profile月ev이을 나타내고, enhancement layer 1이 enhancement layer 2보다

      lower layer이다. Base layer는 scalab血ty를 사용할 수 없으므로, base layer의 profile은

      main profile이거나, scalab小勺를 포함하지 않는 high pr而le이다. 이 base layer

      decoder는 표의 최우측단어］ 기술된 profile月eve!에서 허용하는 어떠한 synt炚나 어

      떠한 paran났er값을 가질 수 있다. HP＠入4L spati십ly scaled bits仕earn에서 base layer

      decod町의 형태가 HP@(level-1）이라 함은 MP@(level-l)과 같다. 이는 base layer에

      서는 scalab小口가 없고, HP@ML보다 낮은 level은 그 level에서의 main profil고干 같

      기 때문이다. 만일 base layer에서 허용되는 변수보다 적은 변수를 사용하고， 변

      수들의 범위도 줄여서 사용한다면 base layer의 proffle이 전체 bits仕earn의 profile

      보다 낮은 pr吐配이 된다. 한편, HP@M工의 layer 수가 3인 경우, enhancement layer

      1이 spatial layer이면 이 layer에서는 中2:2 c뇨oma的rmat은 지원되지 않는다． 이것

      은 enhancement layer 2가 SNR layer이기 때문인뎨, enhancement layer 1이 4:2:0

      chr이na format을 갖고 SNR layer가 4:2:2 C뇨oma format을 갖는 경우，SNR layer에서

      lo＼肥r layer의 해당 bli乂k이 없으면 그 bli乂k의 coded data가 없는 것으로 생각하고

      SNR layer에서 향상시켜주면 되지만, 그 반대의 경우는 syntax상 lower layer에는

      있고 SNR layer어］ 없는 bk兀k들（7, 8번）은 디코딩하지 않기 때문이다．




  6.5. 프로파일, 레벨과 레이어에서의 변수값
        이 표 6-11은 표본밀도에 태한 상한UPI玘r bounds）을 나타낸 것인뎨， 다음 서］

      변수에 대한 것이 나타나 있다．

          samples/line : horizont出_size

          lines/frame : vertical size

          frames/sec : frame rate
                                                                                                          MPEG
                                                                                                          피DE0        261



                  표 b] ] . U口per bounds f아 釵그n）口Ung den엷ty ( MPEG IS I야)Ie &] ] )
                      Spatial
                                                                                    Pro川C
                    r心이ution
 I七vet                 layer                            Simple          Main           SNR         Spat洌           Iligh

  Iligh           Enhancement          samples/line                     1920                                       1920
                                        lines/flame                     1152                                       1152
                                        frames/sec                        60                                        60
                      1,ower           samples/line                                                                9（刃
                                        lines/flame                                                                576
                                        frames/sec                                                                  30
                  Enhancement          samples/line                     1440                        1440           1440
 楹：
                                        lines/frame                     1152                        1152           1152
                                         frames/sec                       a)                         a)            （刃
                      Lower            samples/line                                                 720            720
                                        lines/flame                                                 576            576
                                        flames/s（戈                                                   30             30
 Main             Enhancement          samples/line       720            720           720                         720
                                        lines/frame       576            576           576                         576
                                        frames/sec         30             30            30                          30
                      Lower            samples/line                                                                352
                                        lines/frame                                                                288
                                        nama小cc                                                                     30
      I刃1下        Enhaia无m口it          samples/line                      352           352
                                        lines/frame                      288           288
                                        frames/sec                        30            30
                      Lower            samples/line
                                        lines/flame
                                        fi仙aes/sec

Note:        In the case of single layer or SNR scaled c어：ing, the limits specified by 'Enhancement layer' apply




      Frame rate어］ 대한 상한은 progress加乞記quence가 0인 경우와 l인 경우 모두어］

해당한다． 단일 layer오｝ SNR scaled coding의 경우는 enhancement layer어］ 대한 상

한이 적용된다． 표 6-11에서 각 profile/lev이에는 서］ 개의 상한값이 있는더1, 이 서］

개의 상한값을 동시에 가질 수 있다는 것을 의미하는 것은 아니다. 예를 들어，

MP@Hl의 경우 加nzont4_si配가 1,920이고, 丘ame rate가 30이라면 vertical size는

1,152까지 값을 가질 수 있고, horizont川size가 1,920이고, 卄ame rate가 60이라면

verti沁 없ze는 576까지 값을 가질 수 있다．
262




                     표． 6-12 U口口e사）ounds for luri기n（그nce sample rate ( samples/sec )
                                        (MPEG IS : Table 8-12)
                         Spatial
                                                                 Proffle
                        resolution
         Level            layer       Simple      Main        없町t           Spatial         High

                       Enha乂ement                62668800                             62668800 (4:2:2)
         High
                                                                                      83558400 (4:2:0)

                          lA小ver                                                      14745600 (4:2:2)
                                                                                      19660800 (4:2:0)

                       Enhancement               47001 600                 47001600   47001 텨，)0 倖2:2)
       IJigh-1440
                                                                                      62668800 (4:2:0)

                          Lower                                            10368000   11059200 (4:2:2)
                                                                                      14745600 (4:2:0)

                        Enhancement   10368（丸0   10368 000   10368000                 11059200 (4:2:2)
          八lain
                                                                                      14745600 (4:2:0)

                          I乂）＼사er
                                                                                       3041280 (4:2:0)

          L們V           Enhancement              3041280     3041280


                           Lower



      Note: In如case of srngle layer or SNR sc沚edc어如g由elm此斗心小edby 'E血ancement layer' apply




           이 표 6-12에는 휘도신호의 sam하e rate(san叩les/sec）의 상한이 나와 있다． 휘도

         신호의 S如叩le rate를 P라 하면 표어］ 있는 수치들은 다음 식어］ 의해 구해진다．



                  P = horizont刻 이ze va山e * vert匕al size va山e* frame rate
                                                                                              263




 (a) progressive_sequence가 1인 경우

              horizontal_size_value = 16*((honzont섧_size+15)/i 6)

                     vertical_size_value = 16*((vertcaLsize+15)/i6)

 (b)progressive_sequence가 0인 경우

               horizont刻1size va山e = 16士((honzontal_size+15）서6)

                     vertica匕size_va山e = 32*((vert七켸小size+31)/32)


          표 今］3 Uppert兀undsf아바ra怡S（卜毗咐／s)                     (MPEGIS: TabIe8-13)
                                            Profile
 Simple        Mate             SNR                    Spatial                   H培h
                                                                             l00 시llayers
                80                                                       80m斌lie + base lay町
                                                                              25 base layer
                                                      60a끄 layers             80 all layers
               （刃                              40 middle + base layers   60 middle + base layers
                                                      15base1ay町              20 base layer
                                                                              20 all layers
   15           15          15 b乂h layers                                15 middle + base layer
                            10 base layer                                     4 base layer


                4           4 both layers
                             3 base layer




 이 표 6-13에는 b也rate의 상한이 Mbits/s의 단위로 나와 있는더］, 주어진

profile과 level의 coded bitstream어］ 대한 VBV의 동작을 위한 최대 전송율을 정의

한다. 표에 있는 전송율은 그 layer까지의 누계를 이야기하며， 각 layer의 최다1

전송율은 lower layer의 전송율과의 합이 표에 있는 값이 될 때까지 허용된다．

예를 들어, HP@M山에서 base layer는 4r띠b꺄까지 허용되고，middle layer는 (15Mbps

- base layer rate）까지 허용되며, 모든 layer의 전송율을 합한 것이 20Mbps가 될 때

까지 최상위 layer의 rate를 허용한다．
264




                표o-14 VBV Buffer size requiremenlS (bts) (MPEG IS : Table 8-14)
                                                         Proffle
          Level        Layer      Simple      Mab         SNR       Spalial        Hgh
          Hgh          I加h. 2                                                  12222464
                       I加h. 1                                                  9781248
                       Base                 9781248                               3047424
        111小·1440      Enh. 2                                      7340032     9781248
                       Enh.i                                       4882432     7340032
                       Base                 7340032                1 835 008      2441216
          人lab         Enh. 2                                                     2441216
                       Enh.i                            1 835008                  1 835008
                       Base      1 835008   1 835 어据    1212416                   475 136
          I刃w          Enh. 2
                       Enh. 1                           475 136
                       Base                  475 136    360448




        표 6-14는 VBV bu侄er S吃e어］ 대한 필요량을 b出단위로 나타내고 있는더］, 최대

      허용 bit율에 비례해서 꼐산된다. 이 값은 16시,024의 배수어］ 가장 가까운 정수

      어］ 반내림(rounded down)되어 구해진다. 표에 있는 값들은 MP@ML의 size

      requirement를 기준치로 해서 구해진 값들이다. 예를 들어， MP@H-14에서 최대

      bit율이 6呱化PS이고 MP@ML의 최대 bit율이 1外小PS이므로小4P@H-나의 요구되

      는 크기는 16사，024*(((60115少1,835,008)/(16사，024))=7,340,032이다. 표어］ 있는 값

      은 그 layer까지의 누꼐를 이야기하며, 각 layer의 砒e는 lower layer의 SI配와의

      합이 표에 있는 값이 되도록 해야 한다. 예를 들어, HP@MI』
                                         에서 base layer의

      buffer size는 475,136(bits）를 요구하며, middle layer와 base layer의 bu표er size 합은

      1,835,008(bit旬가 요구되고, 모든 layer를 합쳤을 경우는 2,441,216(bit旬의 Si配가

      되도록 하여야 한다．
                                                                                                            265



          표 6-15 Forward compafib咐yb帥ween d附이ent pro꿰es and 向/els
                             ( MPEG IS 汀야兆＆巧 )
                                                              1k쩍쩍xler
                       HP      HP      HP     Spatial 없旺t        針汀t     A11>    八IP      MP      人'P       SP
   Pr刈e & Level         @       @       @        @        @       @       @       @        @       @         @
    indication in      HI     H-14     ML      H-14      ML      LL      HL      H-14    ML       LL        ML
      t埴tata坪귀m
 ILP@HL                 x
 I표@H-14                x       x
 HP@ML                  x       x       x
 Spatial@H-14           x       x                x
 SNR @ML                x       x       x        x        x
 SNR@LL                 x       x       x        x        x       x
 MP@HL                  x                                                  x
 MP@H-14                x       x                x                         x       x
 八IP@ML                 x       x       x        x        x                x       x       x
 MP@LL                  x       x       x        x        x       x        x       x       x       x        x*
 SP@ML                  x       x       x        x        x                x       x       x                     x
 IS lEC 11172           x       x       x        x        x       x        x       x       x       x             x
           X indicates the dec에＝r sha나比 able to decod已 the bitstream including all relevant lower layers.
           半 Note that SP@ 너L decoders are卿uired to decode MP@LL bitstreams.




 표 6-15는 서로 다른 profile과 level 간의 白rward co呻alib皿ty를 나타낸다. x는

주어진 profile과 level의 디코더가 디코딩할 수 있는 bits打earn의 profile과 level을

나타낸다. 예를 들어, HP@Ml쇠 디코더는 HP@ML, SNR@ML, SNR@LL,

MP@ML, MP（飢1, SP@ML, MPEG1의 bitstream을 디코딩한다. 또, SP@ML의 디

코더는 MP@LL의 bit引ream을 디코딩할 수 있어야 한다.
      MPEG
266   V山E0




  6.6. 각 프로파일과 레벨에서의 제한조건들
           다음 표들은 각 프로파일과 레벨에서의 제한조건을 나타낸다. 또 표 6-拓은

          이 표들어써 쓰이는 용어의 뜻을 설명해 놓은 것이고 표 6-17에서 6-34까지는

          S푀ltax의 header, ex把nsion 등에서의 변수들에 대한 조건을 나타내고 표 6-35에서

          6-61까지는 pr而le과 level에 따른 변수들의 제한치를 나타낸다．


                     표o-lo Abbreviations used in the Tables of 6.6( MPEG IS : Table E-1)
      Abbreviation            Used in            入leaning
      x                       Stafl］只            must be supported by the decoder
      0                       Status             need not be supported by the decoder
      D                       Type               it巳m with Level-dependent parameters
      1                       Type               item independent of the Level in the Pmfile
      p                       Type               item for post-pmcessing after decoding; the decoder must be
                                                 capable of decoding bitstreams which contain these items, but
                                                 their use is beyond the scope of 出is Recommendation I
                                                 Internation出 Standani
                                                                                        MPEG
                                                                                       쌉또              267




                                      표 6-17 Sequence header ( MP日; is : T（카이e 타 2)
     Status                                                                     Type
     HIGH
     SPATIAL
     SNIR
     MAIN
     SIMPI上
#    Syntactic elements                                                                comments
01   horizontal size value                              x    x    乂    X   x    D      see Table 8-7
02   vertical size value                                x    x    x   x    x    D      see Table 8-7
03   aspect_ratio_information                           X    x    x    x   x    P
04   frame rate code                                    K    x    x    x   x    D      see Tables 8-7 and
                                                                                       8-6
05   呼Irate)                                                                    D      see Table 8-8; pcI
     Note: this is not a syntactic element                                             rate is a product of
                                                                                       pels/line,
                                                                                       lines/frame     and
                                                                                       fran妃s/sec
06   bit rate value                                     x    X    x    x   x    D      see T的Ic 8-9
07   vbv buffer size value                              X    x    x    x   x    D      see Table 8-10
08   constrained_par川lleters_flag                       x    x    x    x   x    1      set to '1' if MPEG-
                                                                                       1 constrained,
                                                                                       set to '0' if MPEG
                                                                                       2
09   load_intra_quantiser_matrix                        x    乂    x    K   K    1
10              intra_quantiser_matr1x164]              x    K    K    x   x    1
11   load_non_intra_quantiser_matrix                    x    K    x    K   K    1
12             non_intra_quan出er_mat씨64l                x    x    x    K   K    1
13   sequence_extensionO                                x    K    x    K   x    1      always present if
                                                                                       入4PEG-2
14   sequence_display_extensionO                        K    K    K    K   x    P
15   sequence_scalable_extensiono                       0    ()   K    乂   x    1      see Table 8-11 for
                                                                                       maximum number
                                                                                       of scalable laye八
16   user data()                                        x    K    x    x   K    1      d就에er may skip
                                                                                       this data
268




                                   표 -18 Sequence exten엷아）( MPEG IS : T야)Ie E - 3)
                                                                             Status TT比
                                                                             HIGH
                                                                   SPATIAL
                                                                   없나R
                                                            MAIN
                                                  S끄 'LPLE
#     Syntactic elements                                                                  Comments

01    proffle_andJeveLindication                       x      x     x    x     x    D     proffle: one of 8 values
                                                                                          level: one of 16 values
                                                                                          esca比 bit: one of 2
                                                                                          valu（冬
02    progressive_sequence                             x      x     x    x     x    1

03    chroma format                                    x      x     x    x     x    1     see Table 8-5
04    horizontal 毗e exten前on                           x      x     x    x     x    D     input picture size
                                                                                          related
05    vertical 前ze extension                           x      x     X    x     x    D     血Pu印icture 5끄e
                                                                                          related
06    bit rate exten寸on                                x      x     X    x     x    D     input pi｛艾ore s끄e
                                                                                          related
07    vbv buffer size exten鈿n                          x      x     x    x     x    D     l叩Ut P1Cmm size
                                                                                          related
08    low_delay                                        x      x     x    x     x    1

09    frame rate extension n                           x      x     x    x     x    I     set to 0 for all defined
                                                                                          profiles

10    frame rate extension d                           Ii     x     x    x     x    1     set to 0 for all defined
                                                                                          profiles
                                                                                    MPEG
                                                                                    뮈DE0         269



                      표 6-19 Sequenced恰口ay exten訊＞n elements ( MPEG IS Table 타 4)
                                                                      Sh卄1伊 Type
                                                                      HIGH
                                                            SPATIAL
                                                            SNR
                                                     MAIN
                                            SIMI兀E
#    Syntactic elements                                                            Comments

01   video format                                x     x     x    x     x    P
02   colour_description                          x     x     x    X     x    p     血1乂it format related
03        colour_primaries                       x     x     x    x     x    P
04        transfer characteri鹹cs                 x     x     x    x     x    P
05        matrix coefficien臼                     x     x     x    x     x    P
06    isplay horizontal si乙e                     x     x     x    x     X    p     input format related
07   display_verti沚size                          x     x     x    x     x    P     input format related
270




                           표6-20 Sequence scalable extensions ( MPEG IS Table E -5)
      Status                                                             Type
      1끄GH
      SPATIAL
      SNR
      八4AIN
      SIMPLE
#     Syntactic elements                                                        C아nments
01    sealable mode                               0    0   x    x    x   1      SNR      Profile:  SNR
                                                                                Scalab丑ity
                                                                                Spatial and High Profile:
                                                                                SNR         or    Spatial
                                                                                Scalability
02    layer_id                                    0    0    x   x    x   1
      寸（spatial sc出able)
03               lo1枇ri町er_predic由n               0    0   0    x    x   D      see    table   8-8   for
                 horizontal size                                                luminance       sampling
                                                                                density
04               lower_layer_prediction           0    0   0    x    x   D      see    table   8-8   for
                 vertical size                                                  luminance       sampling
                                                                                density
05               horizont出_subsampling            0    0   0    x    x   1
                 factor m
06               horizont出_subsampling            0    0   0    x    x   1
                 factor n
07                verti沁크山sam［山略                  0    0   0    x    x    1
                  f加tor m
08                vertical_s山san耳汕唯               0    0   0    x    x    1
                  factor n
      if(temporal scalable)
09                picture_mux_enable              0    0    0   0    0    I
10                mi姓加下rogr哨S加e馳quence            0    0    0   0    0    1
11                picture_mux_order               0    0    0   0    0    I
12                picture_mux_factor              0    0    0   0    0    I
                                                                                   1그         ::,


                          표 6-21（갉ou口 of pictures header ( MPEG lS: T야)Ie F - 6)

                                                                     Status Type
                                                                     HIGH
                                                           SPATIAL
                                                           SNR
                                                     MA[
                                            SIMPLE
#    Syntaclic elements
                                                                                   Comments
01   血ne code                                    x     x    x    x     x    1
02   c1冷ed召아）                                    x    x    x     x     x    I
03   broken 娃nk                                  x    x    x     x     x    1
272




                                      표6-22 Picture header    (MPEG IS : Table E -7)
                                                                              Status Tyi光

                                                                              HIGH

                                                                    SPATIAL

                                                                    SNR

                                                             MALN

                                                    SIMPLE
                                                                                            Comments
#     Syntactic elements

                                                        x      x     x    x      x     1
01    temporal_reference
                                                        x      x     x    x      x    1     Simple P기0file: I, P
02    picture_coding_ty比
                                                                                            at Main level.
                                                                                                        I. P. B
                                                                                            at Low level
                                                                                            Main, SNR, Spatial
                                                                                            & High Profile: I,
                                                                                            P. B

                                                        x      x     x    x      x     1
03    vbv_delay
                                                        x      K     X    x      x     1    "0" for MPEG-2
04          f毗Lpe1如rward_v毗or
                                                               x     x    x      x     1    '111" 凡rJ뇨4PEG-2
05          白rward f code                               x

                                                                     x    x      X     I    '0' for MPEG-2
06          ftillpeI上岫M町d ye如r                           X     x

                                                               x     X    K      x     1    ' 111" forMPEG-2
07          backward f code                              x


            extra_information_picture                    x     x     x    x      x     1
08
                                                                     x    K      x     1
09    picture_coding_extension()                         x     x

                                                         x     x     x    x      x     1
10    quant_matrix_extension()
                                                               x      x   x      x     P
11    picture_display_extension()                        x

                                                                     0    K      x     [
12     picture_spatial_scalable_extension0               0     0

                                                                          0      0     1
13    picture_temporal_scalable_extension()              0     0     0
                                                                                              273



                                표 &23디cture coding 태旭哨on (MPEG IS :I야)Ie E召）
     Status
                                                                         Type
     HIGH
     SPATIAL
     SNR
     入{All寸
     SIMPLE
#    Syntactic elements                                                         Comments
01   f_code[O][O] (forward horizon切l)        x   x       x   x   x   D           I乂)W I尤ye! [1:71
                                                                                入4am I七ye! [1:8]
                                                                                High-1440 & High
                                                                                Level [1:9]
02   f_code[01[1J (forward vertical)         x   x    x      x   x   D          I乂)W I尤vel [1:41
                                                                                Main, Fligh-1440 &
                                                                                I五ghl尤ye! [1:5]
03   f_code[1][O] (backw壯d ho屯ontal)         x   x    x      x   x   D          I刃＼vi尤vel [1:7]
                                                                                M曲l 1尤vel [1:8]
                                                                                High-1440 & High
                                                                                Level [1:9]
04   fc에e[1][1] (ba吐ward ver伽刻 )             x   x    x      x   x   D          Low level [1:41
                                                                                Main, H-14 & High
                                                                                Level [1:5]
05   in佃jkJ吐ec奴on                            x   x    x      x   x   i          Simple, Main, SNR &
                                                                                Spatial
                                                                                Profile: [8:10]
                                                                                High Profile: [8:111
06   picture_structure                       x   x    x      x   x   I
07   t叩J념dfii吼                               x   x    x      x   x   I
08   frame_pred_fraine_dct                   x   x    x      x   x   1
09   conce拙ment_moti이i vectors               x   x    x      x   x   I
10   qs（月Iety比                               x   x    x      x   x   I
11   intra vie format                        x   x    x      x   x   I
12   alternate scan                         x    x    x      x   x   I
13   repeat_first_field                     x    x    x      x   x   I
14   chroma_420_type                        x    x    x      x   x   P
15   pri埋res前ye玉ame                         x    x    x      x   x   P
16   composite_display_flag                 x    x   x       x   x   P
17              v axis                      x    x   x       x   x   P
18              field_sequence              x    x   x       x   x   P
19              sub carrier                 x    x   x       x   x   P
20              burst_amplitude             x    x   x       x   x   P
21              sub_carrier_phase           x    x   x       x   x   P
274




                                 표 6-24 Qu（그nt matrix exten引on ( MPE（引S : T(걋긔eE ' 9)
                                                                             Status   Type
                                                                             HIGH

                                                                   SPATIAL
                                                                   SNR
                                                            MAIN
                                                   SIMPLE
                                                                                             Comments
#       Syntactic elements
                                                        x     x     X    x      X      1
01      load_intraquantiser_matrix
             intraquantiser_matrix[64J                  X     x     x    x      x      1
02
                                                              x     x    x      X      1
03      佃ad_non_intr之叩antiser끄atiix                     x

                                                        x     x     x    x      x      1
04           nonintra_quantiser_
                   ma1ri4641
                                                        0     0     0    0       x     1
05      load_chroma_intra_quantiser
                   niahix
                                                        0     0     0    0       x     I
06            chroma_intra_quantiser
                   matrixt64]
                                                        0     0     0    0       x      1
07      load chroma non intra
                   quantiser_matrix
                                                        0     0     0    0       x      1
08            chroma_non_intra_quantiser
                   matrix[64]




                                표 6-25 니아내e dis이ay extension ( MPEG IS Table E - 10)
                                                                             Status   T印e
                                                                             HIGH
                                                                   SPATIAL
                                                                   읾놔R
                                                            MAIN
                                                   SIMPLE
                                                                                             Comments
    #    Syntactic elements
                                                              K     x    x      x      P     input format related
 01      frame centre horizontal offset                 K

                                                        K     K     K    K      x      p     input format related
 02      frame centre vertic出 offset
                                                                                                              L 1            275



                           표 6-26 아寸ure tempor이 scalable exten엷on ( MP日; is : I（그ble E ] ])

                                                                                           Status Ty比
                                                                                           HIGH
                                                                             SPATIAL
                                                                         SNR
                                                               A1An놔
                                                   S끄江P1氾
 韋    Syntactic elements                                                                                      Comments
01    reference select code                               0          0        0       0         0       1
02    fon平ard ten耳沁ral reference                          0          0        0       0         0       1
03   backward_temporal_reference                          0          0        0       0         0       1



                            표 6-27 디cture斗）ati이sc이able extension (MPEG IS 幻ble E -12)

                                                                                          Status Ty比
                                                                                          HIGH
                                                                         SPATIAL
                                                                         SNR
                                                              l녑［AIN
                                                  SINPLE
#    Syntactic elements                                                                                     Comments
01   Lower_layer_temporal_reference                   0          0        0       x         x       1
02   lower layer horizontal offset                    0          0        0       x         x       D       input format related
03   lower_layer_vertical_offset                      0                                             D
                                                                 0       0        x         x               input format related
04   spatial_temporal_weight_code                     0          0       0        x         x       1
          table index
05   Lo吼r_layei그：
                1rogressive_如me                       0          0       0        x         x       1
06   lower_layer_deinterlaced_tield                   0          0       0        x         x       1
          select
276




                                       표 6-28 톄ce layer (MPE（引S : I（求긔eE - 13)
                                                                              St가tu뀨 Ty11e

                                                                              HIGH

                                                                    SPATIAL

                                                                    SNR

                                                             入t N

                                                    SI旺PI皿

#     Syntactic el巴llents                                                                    Comments

01    slice_vertical_po前tion_                            x     x     x    x      x    D      input format selated
           exten葫On

02         priority_breakpoint                           0     0     0    0      0    1      only requi七d for data
                                                                                             partitioning

03    quantiser_scale_code                               x     x     x    x      x     I

04         intra slice                                   x     x     x    x      x    1

05         extra information slice                       x     x     x    x      x    1      da:0(l巳r may skip 仕dS
                                                                                             data

06    macmblockO                                         x     x     x    x      x     I




                                     표 6-29 Mc그crc丈)lOC川ayer ( MPEG IS : Table E - 14)
                                                                              Status Ty比
                                                                              HIGH
                                                                    SPATIAL
                                                                    SNR
                                                             MMN
                                                    SIMPI코
#     Syntactic elements                                                                     Comments
01          macrobl어：
                    k_escape                             x     x     x    x      x    1
02    macroblock address inc日nent                        x     x     x    x      x    1
03    macroblock_modesO                                  x     x     x    x      x    1
04          quantiser_scale_code                         x     x     x    x      x    1
05          motion_vectors(0)                            x     x     x    x      x    1      forward motion vector
06          motion_vectors(1)                            0     x     x    x      x    1      backward motion
                                                                                             vector
07          coded_block_pattemO                          x     x     x    x      x    1
08          block(i)                                     x     x     x    x      x    1
                                                                                                         277



                                 표6-30 Macroblock modes (MPEG IS : Table E - 15)
                                                                             Status Type
                                                                             HIGH
                                                                   SPATIAL
                                                                   SNR
                                                           MAIN
                                                   SIMPLE
 #    Syntactic elements                                                                    Comments

01    macroblock_ty比                                   x      x     x    x      x    1
02         spati키_tempora1weight_code                  0     0      0    x      x    1
03         frame_motion_ty比                            x     x      x    x      x    1      01: Field-based
                                                                                            prediction
                                                                                            10: Frame-based
                                                                                            prediction
                                                                                            11: Dual-prime
04         field_mot向U勺pe                              x      x     x    x      x    1      01: Field-based
                                                                                            pre小ction
                                                                                            10: l6x8MC
                                                                                            11: Dual-prime
05         dct_tyj比                                    x      x     x    x      x    1




                                     표 6-3] 卜加枇＞n vec幻rs    ( MPEG IS 汁able E - 16)

                                                                              Status Tyj光
                                                                              HIGH
                                                                    SPATIAL
                                                                   없旺t
                                                            MAIN
                                                   SIMPLE
 #    馱Titac如 elements                                                                      Comments

 01   motion vertical field select                     x      x     x    x      x     1
 02   motion_vector()                                  x      x     x    x      x     1
         MPEG
278      피DE0




                                   표6-32 Motion vector (MPEG IS : Table E - 7)
                                                                              Status Type
                                                                              HIGH
                                                                   SPATIAL
                                                                  SNR
                                                          MAIN
                                                 SIMPLE
#     Syntactic elements                                                                      Commen朽

01    motion horizontal code                         x      x       x     x     x     1
02         motion horizontal r                       x      x       x     x     x     1
03         dmv horizontal                            x      X       x     x     x     1
04    motion vertical code                           x      x       x     x     x     1
05         mo岱아i vertical r                          x      x       x     x     x     1
06         dmv vertical                              x      x       x     X     x     1




                                 표 6-33 Coded 텨（>ckPa卄em        ( MP日; is : T（그ble E - ] 8)
                                                                              Status Ty1比
                                                                              HIGH
                                                                   SPATIAL
                                                                  SNR
                                                         l너［AIN
                                                 SIMPLE
#     Syntactic elements                                                                      Comments

01    c에ed_blockpattern_420                          x      x       x     x     x     1
02         c에e&blockpatternj                         0      0      0      0     x     1       4:2:2
03         coded_blockpattern_2                      0      0      0      0     0     1       4:4:4
                                                                                                                         MPEG
                                                                                                                         뮈DE0          279
                                                                                                                           1   모




                                                표6-34 Block layer (MPEG IS : Table E - 19)
                                                                                                 Status T11e
                                                                                                 HIGH
                                                                                      SPATIAL
                                                                                      SNR
                                                                            A1A1N
                                                              SI入IPLI亡
 #       Syntaclic elements                                                                                          Comments
 01      DCT coefficients                                               x      x       x     x       x          1
 02      End of block                                                   x      x       x     x       x          I




                                           표 6-35 Abbre崍批Dns幻나＞rc州e an비evel names
                                                      (MPEG IS : Table E - 20)
                                                   <profile                                              <level
                            Proffle                abbreviation>              Level                      abbreviation>

                            Simple                  Sp                        Low                        IL
                            Main                   八4p                        入4am
                            SNR Scalable            SNR                       I五gh-1440                  H-14
                            Spatia끄y Scalable       Spt                                                  FII
                            High                   HP
                            LSO/IEC 11172-1 constrained parameters                                       ISO 11172




                                      표6-36 Simple profile @ Main level (MPEG IS : Table E -21)
No. of       layer id         S叫山가h1        Maximum sample         入'I규ximum           Maximum             Maximum                 Profile and
layers                         In'겨仰            density            Sam1이e rate         切talbiti沮te         total VBV                  level
                                                 (lilY/F)                               /1000000             but扼r                 indication

  l             0              Base             720/576/30           10368000               15                 1 835 008            SP@ML



                                      표 6-37     M이n 口ro꿰e @ 山＼사 1ev이                 ( MPE（引S : T야DIe E - 22)

No. of       layer id         Scalable      Maximlum sample          Maximum           八1aximum            Maximum             Pr(）川e and
layers                         mode             den前ty               s別1llple rate     加切1bit rate         切talVBV                level
                                                 (B/V/F)                                11000000            bu甘er              indication

  l             0              Base             352/288/30            3041280               4                  475 136               fl기＠IL
 280




                               표 6-38 M이n prc洌e @ Main I今tel (MPEG IS : T야긔eE -23)
No. of   layer id   Scalable      Maximwn sample   Maximum       lV1nYi11끼im 切切l   Maximum       Profile and
layers               mode             density      sample rate        bit rate     total VBV   level indication
                                      (H/V/F)                        /1000000        buffer

  1         0        Base            720/576/30     10368000           15          1 835 008     MP@ML




                            표． o-39 卜爪Jin口r애e@ High-i 44이今同（MP日; is: T야兆E- 24)
No. of   layer id   Sc川able       Maximum sample   Maximum       八aximum total     八aximum       Profile and
layers               mode             density      sample rate      bit rate       切talVBV     level indication
                                      (H/V/F)                      /1000000         bu卄er

  l         0        B田e            1440/1152/的     47001 600          d)          7340032       MP@H-14




                               표． 6-4CM이n 口rofile @ High level ( MPEG IS 汗야DIe E - 25)
No. of   layer id   Scalable      Maximum sample   Ma가imum       Maximum total     짜[a너mum       Pn）川e and
layers               mode             density      sample rate      biti크te        加t出 VBV     level indication
                                      (WV/F)                       /10(朕KK)          I川1付er

  l         0        Base           1920/1152印      62668800           80          9781 248       MP@HL




                                표 o-4i SNP pr州e @ Lo＼八／level ( MPE（引S : T求긔e 탸 26)
No. of   layer id   Scalable      Maximum sample   人aximum       Maximum total     Maximum       Pn姻［e and
layers               mode             density      sa叫1e rate       bit rate       切talVBV     level indication
                                      (WV/F)                       /1000(朕）         buffer

  2         0        Base            352/288/30     2534400           1.8564        327 680      Iso 11172
            l        SNR             352/288/30     2534400                         475 136      SNR@LL
  2         0,                       352/288/30     3041280                         360448        SP@ML
                     BaseSNR         352/288/30     3041280                         475 136      SNR@LL
  2         0,       Base            352/288/30     3041280                         3＆나48         MP@LL
                     SNR             352/288/30     3041280             43          475 136      SNR@LL
                                                                                                       281




                                 표6-42 SNR profile @ Main level ( MPEG IS : Table E - 27)
No. of   layer id   Sc川able        Maximum sample    Maximum        入如ximum 切tal    1小牡in뀌mi      Pn刈te and
layers               1111겨'p           den葫ty        S刊Laple i沮te     bit rate      加tal VBV    level indicat和n
                                       (H/V/p)                       I1(K川XK1         buffer

  2         0        B孤C              720/57仍0        2534400           1.856        327 680      Iso 11172
            l        SNR              720/576/30      2534400            15         1 835 008     SNR@ML
  2         0        Base             720/57日30       10368000           10         1212416        SP@ML
            l        SNR              720/57日30       10368000           15         1 835008      SNR@ML
  2         0,       Base             3521288/30      3041280            4           475 136       MP@I工
                     SNR              3521288/30      3041280            15         1 835008      SNR@ML
  2         0,       Base             720/57日30       10368000           10         1212416       MP@ML
                     SNR              720/576/30      10368 000          15         1 835008      SNR@ML



                                표． 小43Spafl이 口n＞셰e @ High-144(기evel (Base Layer + SNR)
                                               ( MPEG IS : Ta兆 E 口8)
No. of   layer id   Scalable       Maximum sample    Maximum        Maximum total   Ma너mum        Pro川e and
layers               n기겨仰              density       sample rate       bit rate     切talVBV     level 뇨小cation
                                       (H八1/F)                        f1000X刃        buffer

  2         0        Base             3521288/30      2534400           1.856        327 680      Iso 11172
            l        SNR              3521288/30      2534400            d)         7340032       Spt@H-14
  2         0,                        720/57日30       10368000           15         1 835 어据       SP@ML
                     ’，業              720/57日30       10368 000          （刃         7340032       Spt@H-14


                                                                         二
  2         0,                        352/288/30      3041280                        475 136       MP@LL
                      BaseSNR         352/288/30      3041280                       7340032       Spt（孕H-14


                                                                         늠
  2         0        Base             720/576/30      10368 000                     1 835008       MP@ML
            l         SNR             720/576/30      10368000                      7340032       Spt@H-14


                    ：焄
  2         0                        1440/1152/60     47001 600          40         4882432       MP@H-14
            l                        1440/1152/60     47001600           d)         7340032       Spt@H-14
 282




                          표． 小44Spa이口rofile @ High-144이今向 (B小e Layer + S口（내이）
                                        ( MPEG IS : I야兆 E口9)
No. of   layer id   Scalable     人Ia목unum       짜Ia沖叫In'       Maximum        人laximum t毗al     I뇨姻le and
layers               mode      sample density   sample rate   t야al bit rate    VBV bu什er      level in小cation
                                  (H/V/F)                      /1000000

  2         0        Base       768/576/30       2534400         1.856           327 680        15O11172
            l        Spatial   1440/1152/30     47001 텨IX)         60           7340032         Spt@H-14
  2         0        Base       720/576/30      10368000           15           1 835008         SP@ML
            l        Spatial   1440/1152/30     47001 600          60           7340032         Spt@H-14
  2         0        Base        352口88/30       3041280           4             475 136         MP@I工
            l        Spatial   1440/1152/30     47001600           60           7340032         Spt@H-14
  2         0        Base       720/576/30      10368000           15           1 835008        MP@ML
            l        Sr用hal    1440/1152/30     47 仄아 600          6            7340032         Spt@H-14
  2         0        B出e       1440/1152/印      47001 600          40           4882432         MP@H-14
            l        Spatial   1440/1152印       47001 600          d)           7340032         Spt@H-14
                                                                                                           283




                            표 6-45 Spati이 口rofile @ High-i MO level (Base 山yer + SNR + Spati이）
                                                  (MPEG IS I Table E -30)

                          Scalable      Maximum        Maximum       Ma巾llum        Maximum total     Pro川e and
No. of        lager Id
                           mode       sample density   sample rate   加切1 bit rate    VBV bu侄er      level indication
lagers
                                                                      /1000000
                                         (H/V/F)

  I                        Base         352/288/30      2534400         1.856          327 680        ISO 11172
                 0
                           SNR          352/288/30      2534400           4            475 136        SNR@LL
                 l
                 乃         Spatial     1440/1152130    47001600           60          7 340032        Spt@H-14

                 0          Base        352/288/30      3041280           3            360448          SP@ML
  3
                            SNR         352/288/30      3041280           4            475 136         SNR@LL
                 l
                 n         Spatial     1440/1152/30    47001 600          60          7340032          Spt@H-14

   극                        Base        352/288/30      3041280           3            360448          MP@LL
                 0
                  l         SNR         352/288/30      3041280           4            475 136         SNR@LL

                 2         Spatial     1440/1152/30    47001 600          60           7340032         Spt（孕H-14

                            B出e         720/576/30      25344에           1.856         327 680         ISO 11172
      ;          0
                  l         SNR         720/576/30      2534400           15           1 835008        SNR@ML

                  )        Spatial     1440/1152130     47001600          （刃           7340032         Spt（孕H-14

                            Base        720/576/30      10368000          10           l 끄2416          SPt0ML
      3           0
                     l      SNR         720/576/30      10368000          15           1835008         SNR@ML

                           Spati고      1440/1152/30     47001 600         d0           7340032         Spt@H-14
                     2
                            Base        352/288/30      3041280            4            475 136         MP@LL
      3              0
                            SNR         352/288/30       3041280          15           1835008         SNR@ML
                      l
                     스      Spatial    1440/1152/30     47001600          60           7 34O032        Spt（孕11-14

      극                                 720/576/30      10368 000         10           l 끄2416          MP@ML
                     0      Base
                             SNR         720/576/30     10368000           15          1 835008        SNR@ML
                      l
                      2     Spatial     1440/1152/30    47001600           60          7 34O032        Spt（孕H-14

          三                  Base       1440/1152/60    10368000           15          1 835008        MP@H-14
                      0
                      l      SNR        1440/1152/60    10368000           40          4882432          Spt@H-14

                      2     Spatial     1440/1152/60    47001 600          60          7340032          Spt@H-14
         284




                                         표 6-46 Spa卄이 口r아가e @ Hig八］440 level (Base 山yer + Spati（기 + SNR)
                                                            (MPEG IS : Table E -31)
      No. of          layer Id      Scalable              Maximum             Maximum            Ma姓mum          Maximum total        Pro丘leand
      layers                         mode               sample density        sample rate       total bit rate    VBV buffer        level indication
                                                           (HJVIF)                                /1000에0

         3               0              Base             768/576/30            2534 400            1.856              327 680         ISO 11172
                         1          Spati띠              1440/1152/30          47001 600              40              4882432          Spt（孕H-14
                         2              SNR             1440/1152/30          47001600               60              734O032          Spt（包H-14
         I               0              Base             720/576/30           10368 000              15              1 835008          SP@ML
                         1          Spatial             1440/1152/30          47001 600              40              4882432          Spt（孕H-14
                         )
                                        SNR             1440/1152/30          47001 600              d)              7340032          Spt（孕H-14
         3              0               Base             352/288/30           3041280                4               475 136          MP@LL
                        l           Spatial             1440'1152130          47001 600             40               4882432          Spt（孕H-14
                        2               SNR             1440/1152/30          47001 600             60               73中0032          Spt@H-14
         3              0               Base             720/576/30           10368000              15               1 835008         MP@ML
                        l           Spatial             1440/1152/30          47001 텨)0             40               4882432         Spt（包H-14
                        2               SNR             1440/1152/30          47001 600             60               734O032         Spt@H-14
         국              0               Base             720/576/30           10368（刃0              15               1 835008        MP@H-14
                        1           Spa丘al              1440/1152/60          47001600              40               4882432         Spt@H-14
                        2               SNR             1440/1152/30          47001 600             60               7340032         Spt@H-14



                                    표6-47 High profile @ Main level (Base Layer) (MPEG IS : Table F - 32)
No. of         layer id      Scalabl           Chroma          Maximum            Maximum             Maximum           Maximum        Profile and
layers                       e mode            Format        sample density       sample rate        total I血 rate      total VBV         level
                                                                (H/V/F)                                /1000000           bu熙｝r        indication
  l               0              B沓e            4:2:0          720/576/30         14745600                 20           2441216         HP@ML
  ]               0              Base           4:2:2          720/576/30         11 059200                20           2441216         HP@ML
                                                                                                    MPEG
                                                                                                    피DE0      285




                                     표o-48 High profile @ Main level (Base Layer + SNR)
                                                 (MPEG IS : Table E - 33)
                         Sc汕able     Chroma        M1斗쩍iinum     M和XH卞urn       Maximum       Maximum      Profile and
No. of     layer id
                                     Format         sample       sample rate     切tal bit     切talVBV         level
layers                    mode
                                                    density                       rate         buf比r       indication
                                                                                Ii伉朋（H:1
                                                    (H/V/F)
                                      4:2:0        720/576/30    10368000          15         1 835 008     SP@ML
  2           0,          Base
                          SNR         中2:0         720/576/30    10368 000         20         2441216       HP@ML

                                      4:2:0        720/576/30    10368000          15         1 835008      SP@ML
  2           0           Base
                                      4:2:2        720/576/30    10368 000         20         2441 216      HP＠入'IL
              l           SNR
                                      中2:0         352/288/30     3041280           4          475 136      MP@LL
  2           0           Base
                                      4:2:0        352/288/30     3041280          20         2441216       HP@N兀
               l          SNR
                                      4:2:0        352/288/30     3041280           4          475 136      MP@I工
  2           0           Base
                           SNR        4:2:2        352/288/30     3041280           20        2441216       HP@ML
               l
                                      4:2:0        720/57日30      10368000          15         1 835 008    入'IP@ML
   2           0,
                                      4:2:0        720/576/30     10368000          20        2441216       HP@ML
                           ’，業
                           B出e        4:2:0        720/576/30     10368 000         15         1835008      MP@ML
   2           0
                           SNR        4:2:2        720/576/30     10368 000         20         2441 216     HP@ML
               l
                           Base       牛2:0         720/576/30     14745600          15         1 835008     HP@1vlL
   2           0,
                           SNR        4:2:0        720/576/30     14745600          20         2441216      HP@ML

                                       4:2:2       720/576/30     11 059200         15         1 835008      HP@ML
   2           0           Base
                           SNR        中2:2         720/576/30     11059200          20         2441 216      HP@ML
                   l


                                     표 6-49 High pr：川e @ M이n level (Base Layer + Spati이）
                                                    ( MPEG IS : T야긔eE - 34)
                         Scalable    Chroma         八4기xunum      Ma卄mum         Ma柶1um       Maximum       Profile and
 No. of    layer id
                                     Format          sample       sample rate      切切I bit    切ta1VBV          level
 layers                   mode
                                                     den前ty                         rate       buffer       indi(吐1伽祉l
                                                                                  /1000000
                                                         F)
                                                     (H/V/

                           Base        4:2:0        352/288/30     2534400         1.856        327 680     ISO 11172
   2              0
                          Spatial      4:2:0        720/576/30    14745600          20         2441216       HP@ML
                   l
                           Base        4:2:0        352/288/30     2534400         1.856        327 680     ISO 11172
      2            0,
                          Spatial      4:2:2        720/576/30     11059200         20         2441216       HP@ML

                           Base        4:2:0        352/288/30     3041280                      475 136       SP@ML
      2            0,
                           Spatial     4:2:0        720/576/30     14745600          24。        2441216      HP@ML

                                       4:2:0        352/288/30     3041 280             4       475 136       SP@ML
      2            0,      Base
                           Spatial     4:2:2        720/576/30     11 059200         20         2441216      HP@ML

                            Base             2:     352/288/30     3041280                       475 136      MP@LL
      2            0,                   4:
                           Spatial             。
                                             :40
                                             2:
                                                    720/576/30     14745600          24。        2441216       HP（包ML

                                        4:2:0       352/288/30      3041280                      475 136      入4P@I工
       2            0,      Base
                           Spatial       4:2:2      720/576/30     11059200             41。     2441 216      HP@ML
      286




                                 표6-50 High profile @ Main level (Base Layer + SNR + Spatia
                                                                                            l)
                                                   ( MPE（引S : Table 타 3)
No. of      layer id   Sealable     Chl叫41      入I升帥mum        Maximum       Maximum         umum    I뇨岷le and
layers                  mode        Format    sample density   sample rate    total bit   切ta1VBV       level
                                                  II八7/目                        rate       buffer     i刈cali이I
                                                                             /1000000
  3               0     Base          4:2:0     352/288/30      3041280          3         360 448   SP@ML
                  l     SNR          4:2:0      3521288/30      3041280          4         475 136   SNR@I工
              2        Spatial       4:2:0      720/576/30     14745600         20        2441 216   HP@ML
 3            0         Base         4:2:0      352/288/30     3041280           3         3（又）448   SP@ML
              l         SNR          4:2:0      352尼88/30      3041280          4          475 136   SNR@LL
              2.       Spati끄        4:2:2      720/576/30     11 059200        20        2441216    HP@ML
 3            0         Base         4:2:0     3521288/30      3041280          3         360448     MP@LL
              l         SNR          4:2:0     352尼88/30       3041280          4         475 136    SNR@LL
              2        Spatial       中2:0      720/576/30      14745600         20        2441216    HI기孕A4L
 3            0         Base         4:2:0     352尼88/30       3041280          3         360448     MP@I工
              l        SNR           4:2:0     352/288/30      3041280          4         475 136    SNR@LL
              2        Spatial       4:2:2     720/576/30      11 059200       20         2441216    HP@ML
                                                                                                     287



                               표6-51 High profile @ Main level (Base Layer + Spatial + SNR)
                                                 (MPEg IS : Table E - 36)
No.（寸    layer id   Scalable      clamma     Maximum      Maximum       Ma쩍imum     人aximum     I뇨堀le and
layers               mode         Format      sample      sample rate    t毗al bit   t毗出 VBV         level
                                              den前EN                       1크te       bu依m       indic耐on
                                              (WV/F)                    /1ooK卜凹

  3         0        Base           4:2:0    3521288/30    2534400        1.856      327 680    15O11172
            l        Spatial        4:2:0    720/576/30   14745600         15       1 835 008   HP@ML
            2        SNR            4:2:0    720/576/30   14745600         20       2441216     HP@ML
  3         0        B沓e            4:2:0    352/288/30    2534400        1.856      327 680    ISO 11172
            l        Spatial        4:2:0    720/576/30   11059200         15       1 835008     HP@ML
            2        SNR            4:2:2    720/576/30   11 059200        20       2441216     HP@ML
  3         0        Base           4:2:0    352/288/30    2534400        1.856      327 680    ISO 11172
            l        Spatial        4:2:2    720/57日30    11 059 200       15       1 835008    HP@ML
            2        SNR            4:2:2    720/576/30   11059200         20       2441216     HP@ML
  3         0        Base           4:2:0    352/288/30    3041280          4        475 136     SP＠入4L
            l        Spatial        4:2:0    720/576/30   14745600         15       1 835 0(据    HP@ML
            2        SNR            4:2:0    720/576/30   14745600         20       2441216      HP@ML
  3         0        Base           4:2:0    352/288/30    3041280          4        475 136     SP@ML
            l        Spatial        4:2:0    720/576/30   11059200         15       1 835008    FIP@ML
            2        SNR            4:2:2    720/576/30   11 059 200       20       2441216      HP@ML
  3         0        Base           4:2:0    352/288/30    3041280          4        475 136     SP@ML
            l        Spatial        4:2:2    720/57日30    11059200         15       1 835008     HP@ML
            2        SNR            4:2:2    720/576/30   11059200         20       2441 끄6     HP@ML
  3         0        Base           4:2:0    352/288/30    3041280          4        475 136     MP@LL
            l        Spatial        4:2:0    720/576/30   14745600         15       1 835008     HP@ML
            2         SNR           4:2:0    720/576/30   14745600         20       2441216      HP@ML
  3         0        Base           4:2:0    352/288/30    3041280          4        475 136     八'IP@LL
            l        Spatial        4:2:0    720/576/30   11059200         15       1 835008     HP@ML
            2         SNR           4:2:2    720/576/30   11059200         20       2441216      HP@ML
  3         0        Base           4:2:0    352/288/30    3041280          4        475 136     MP@I工
            l        Spatial        4:2:2    720/576/30   11059200         15       1 835008     HP@ML
            2         SNR           4:2:2    720/57日30    11059200         20       2441216      HP@ML
      288




                                   표 -52 High profile @ 네gh-t44이evel [ Base 山yer)
                                               (MPEG IS : Table E -37)
No. of      layer Id   Scalable   Chroma   Maximum        Ma虹mum        Maximum     Ma姓mum      Pro川e and
layers                  mode      Format    sample        sample rate    的tal bit   total VBV      level
                                            density                        rate       buffer    indication
                                             (11八UF)                    /1000000

  l            0        Base       辛2:0    1440/1152/60   62668800         80       9781 248    HP@H-14
  l            0        Base       4:2:2   1440/1152/60   47001 600        80       9781 248    l-LP@H-14
                                                                                                               289



                                  표 &53 네gh prc）꿰e@ Hi아下］44이今ieI ( Ba昑Layer+ SNR)
                                                (MPEG Is : Table E - 38)
No. of   layer沁   Scalable         Chroma       Maximum        Maximum         三namiim      k印ximum      Profile and
layers            mode             Fonnat        sample        sample rate   total    bit   total VBV    level
                                                 density                     rate           buffer       indication
                                                  (H/V/F)                    /1000000

  2         0                        4:2:0       720/576/30    10368 000         15          1 835 008     SP@ML
            l       BaseSNR          4:2:0      720/576/30     10368 000         80         9781 248      HP@H-14
  2         0,      Base             4:2:0       720/576/30    10368 000         15         1 835008       SP@ML
                    SNR              4:2:2       720/576/30    10368 000         80         9781 248      HP@H-14
  2         0,      B出e              4:2:0       352t288/30     3041280               4      475 136       MP@LL
                    SNR              4:2:0       352/288/30     3041280          80         9781 248      HP@H-14


                              蓋
  2         0                        4:   2:     352/288/30     3041280               4      475 136       入4P@LL
            l        “，                   :40
                                          2:2    352/288/30     3041280          80         9781 248      HP@H-14
  2         0,      Base             4:2:0      720/576/30     10368 000         15         1 835008      MP＠入4L
                    SNR              4:2:0      720/576/30     10368 000         80         9781 248      HP（回H-14
  2         0       Base             4:2:0      720/576/30     10368000          15          1 835008     MP@ML
            l       SNR              4:2:2      720/576/30     10368000          80         9781 248      HP@H-14


                                                                                 몲
  2         0        Base            4:2:0      1440/1152/60   47001 600                    7340032       MP@H-14
            l       SNR              4:2:0      1440/1152/60   47001 600                    9781 248      HP@H-14
  2         0       Base             4:2:0      1440/1152/60   47001 600                    7340032       MP@H-14
                                                                                 60g。
            l       SNR              4:2:2      1440/1152/60   47001 600                    9781 248      HP@H-14
  2         0       Base             4:2:0      72아57日30       14745 600         20          1 835008     HP@ML
            l       SNR              4:2:0      720/576/30     14745600          80         9781 248      FIP@H-14


                                                                                 二응
  2         0,      Base             4:2:0      720/576/30     14745 仗10                     1835008      HP＠入4L
                    SNR              4:2:2       720/576/30    14745600                     9781 248      HP@H-14
  2         0       Base             4:2:2      720/576/30     11 059200         20         1 835008      HP@ML
            l       SNR              4:2:2       720/576/30    11 059200         80         9781 248      HP@H-14
  2         0,      Base             4:2:0      1440/11521的    62 的8800          60         7340032       1-IP@H-14
                    SNR              4:2:0      1440/1152印     62668800          80          9781 248     FIP@H-14
  2         0                        4:2:0      1440/1152/凹    47001600          60          7340032      HP@H-14
            l       BaseSNR          4:2:2      1440/1152/的    47001 600         80         9781 248      HP@H-14


                   ：業
  2         0,                       4: 2 2:
                                                1440/1152/60   47001 600                    7340032       HP@H-14
                                     4: 2 2:    1440/1152的     47001 600         y,          9781 248     FIP@H-14
   290




                             표&54 High profile @ High-1440 level ( Base Layer + Spatial)
                                             ( MPE（引S : 化ble 타 39)
No. of   layer沁   Scalable      Chroma             Ma너mum        M귀ximwn         Maximum    1小1Yi11게ni   Profile and
layers             mode         Format               sample      san기그1le rate    切切1bit    匈切IVBV          level
                                                    den茁ty                          rate     bu心er       indication
                                                    (H/V/F)                      /1000000
  2        0,      B沓e           4:2:0             3521288/30     2534400          1.856     327 680     Iso 11172
                  Spatial        中2:0             1440/1152160   62668800           80      9781 248     HP@H-14
  2        0       Base          4:2:0             352尼88/30      2534400          1.856     327680      ISO 11172
           l      Spatial        4:2:2            1440/1152/印    47001 600          80      9781 248     HP@H-14


                                                                                    二：
  2        0       Base          4:2:0             720/576/30    10368000                   1 835 008     SP@ML
           l      Spatial        4:2:0            1440/1152印     62668 800                  9781 248     HP@H-14
  2        0,      Base          4:         2:    720/576/30     10368000           15      1 835 어沼      SP@ML
                  Spatial             :40
                                        2   2:
                                                  1440/1152印     47001600           80      9781248      HP@H-14
  2        0       Base          4:2:0             3521288/30     3041280           4        475 136      MP@LL
           l      Spatial        4:2:0            1440/1152/印    62668 800          80      9781248      HP@H-14
  2        0       Base          中2:0              352/288/30     3041280           4        475 136      MP@LL
           l      Spatial        4:2:2            1440/1152印     47001日Jo           80      9781248      HP@H-14
  2        0,      Base          4:2:0             720/576/30    10368000           15      1 835008     MP@ML
                  Spatial        4:2:0            1440/1152/的    62668800           80      9781248      I표）@H-14
  2        0       Base          4:2:0             720/576/30    10368 000          15      1 835008     MP@ML
           l      Spatial        4:2:2            1440/1152印     47001600           8。      9781248      HP@H-14
  2        0       B餐e           4:2:0             720/576/30    14745600           20      2 441 216    MP@H-14
           l      Spatial        4:2:0            1440/1152印     62668800           80      9781248      HP@H-14
  2        0,      B出e           4:2:0             720/57日30     14745600           20      2441216      MP@H-14
                  Spatial        中2:2             1440/1152印     47001600           80      9781 248     1-IP@H-14


                                                                                   二：
  2        0,      Base          4:
                                            2:    720/57日30      14745 600                  2441 216     HP(카vIL
                  Spatial             :40
                                        。   2:
                                                  1440/1152/印    62668800                   9781248      I표）@H-14
  2        0,      B田e           4:         2:     720/576/30    14745600           20      2441216       HP@ML
                  Spatial             :40
                                        2   2:
                                                  1440/1152印     47001 600          80      9781248      FIP@H-14
  2                Base          4:         2:    720/576/30     11 059200                  2441216      HP@ML
           01     Spatial             :42
                                            2:2   1440/1152/印    47001 600          208。    9781248      HP@H-14
                                                                                                       291



                         표 6-55 High pr아卄e @ 네아下］44이evel (Base Layer + SNR + S的化［)
                                            (MPEG IS : Table E - 40)
No.（寸    layerid   Scalable   C omo       l比axin께m     入小牡unum         人1aximum    Maximum      I뇨刈노 and
layers              mode      F이inst        sample     sample rate      加tal bit   切tal VBV         level
                                            density                      rate       buffer       indication
                                           (H/V/F)                     /1어X川刃
  3         0        Base      4:2:0      352/288乃0      3041280           3          360 448      SP@ML
             l       SNR       4:2:0      352/288/30     3041280           4          475 136     SNR@LL
             2      s-         中2:0     1440/1152印      62668800          80         9781248     HP@H-14
  3         0        Base      4:2:0      352/288/30     3041280           3          360448       SP@ML
             l       SNR       4:2:0      352/288/30     3041280           4          475 136     SNR@LL
            2       Spatial    4:2:2    1440/1152印      47001 600         80        9781248      HP@H-14
  3         0        Base      中2:0       720/576/30    10368000          10         1212416       SP@ML
             l       SNR       4:2:0      720/576/30    10368 000         15         1 835008    SNR@ML
            2       Spatial    4:2:0    1440/1152／印     62668800          80        9781248      HP@H-14
 3         0         Base      4:2:0     720/57日30      10 368 000 ·      10        1212416        SP@ML
            l        SNR       4:2:0     720/576/30     10368000          15        1 835008    SNR@ML
            2      Spatial     4:2:2    1440/1152/60    47001 600         80        9781248      '-'P（包H-14
 3         0         Base      4:2:0     3521288/30     3041280            3         360448       MP@LL
            l       SNR        4:2:0     352/288/30     3041280            4         475 136     SNR@I工
           2       Spatial     4:2:0    1440/1152印     62668800           80        9781248     HP@H-14
 3         0        Base       4:2:0     352/288/30     3041280           3          360448       MP@LL
            l       SNR       4:2:0      352/288/30     3041280           4          475 136     SNR@I工
           2       Spatial    4:2:2    1440/1152/60    47001 600          80       9781248      HP@H-14
 3        0         Base      4:2:0      720/576/30    10368000          10        1212416       入作色小4L
           l        SNR       4:2:0      720/576/30    10368000          15        1 835008     SNR@ML
          2        S-         4:2:0    1440/1152／印     62668800          80        9781248      HP@H-14
 3        0         Base      4:2:0      720/57日30     10368 000         10         l 끄2416      MP@ML
           l        SNR       4:2:0      720/57日30     10368000          15        1 835008     SNR@ML
          2        Spat표      4:2:2    1440/1152印      47001 600         80        9781248      HP@H-14
 3        0         Base      4:2:0      720/576/30    10368 000         15        1 835008     MP@ML
           l        SNR       4:2:2      720/576/30    10368 000         20        2441216       HP@ML
          2        5-         4:2:2    1440/1152/60    47001 600         80        9781248      HP@H-14
 3        0         Base      4:2:0      720/57日30     14745600          15        1 835008      HP@ML
          l         SNR       中2:0       720/576/30    14745600          20        2441216       HP@ML
          2        Spatial    4:2:2    1440/1152印      47001 600         80        9781248      HP@H-14
 3        0         Base      4:2:0     720/576/30     11 059 200        15        1 835（刃8     HP@ML
          l         SNR       4:2:2     720/57日30      11 059200         20        2441216       HP＠入4L
          2        5-         牛2:2     1440/1152/印     47001 600         80        9781248      HP@H-14
 3        0         Base      4:2:2     720/576/30     11059200          15        1 835008     HP@ML
          l         SNR       4:2:2     720/576/30     11059200          20        2441216      HP@ML
          2        5-         4:2:2    144O/1152印      47001 600         80        9781248      HP@H-14
                 (MPEG
        292       V山E0




                               표 小56 네gh 口田꿰e @ High-1441기ev이 作ase Layer + 部XJ作게 + SNR)
                                               (MPEG기S : I야긔eE-41)

                         Scalable     Chroma     Msa鈿mm         入la긔：imum       入4aximu       Maximum        Profile    and
No. of        layer id
                         mode         Fonnat     sample         sample rate     m total bit   total VBV      level
layers
                                                 density                        rate          buffer         indication
                                                 (H/V/F)                        /1000000
                         Base         4:2:0      352/288/30      2534400        1.856         327 680        ISO 11172
3             0
                         Spatial      4:2:0      1440/11521印     47001（又10      d0            7340032        Spt@H-14
              l
                         SNR          4:2:0      1440/1152/60    4701끄 (ioo     80            9781 248       HP@H-14
              2
                         B出e          4:2:0      352/288/30      2534400        1.856         327 680        ISO 11172
3             0
                         Spatial      4:2:0      1440/1152印      47001 600      60            7 340032        Spt@H-14
              l
                         SNR          4:2:2      1440/1152/的     47001600       80            9781 248       FIP@H-14
              2
                         Base         4:2:0      352/288/30      2534400        1.856         327 680         ISO 11172
3             0
                         Spatial      4:2:0      1440/1152/印 626688（刃           60            7 340 032       HP@H-14
               l
                         SNR          4:2:0      1440/1152/的 62 668 800         80            9781 248        HP@H-14
              2
                         B田e          4:2:0      352/288/30      2534 400       1.856         327 680         ISO 11172
3             0
                         Spatial      中2:2       1440/11521印     47001 텨11O     60            734O032         HP@H-14
               l
                         SNR          4:2:2       1440/1152/60   47001 600      80            9781248         HP@H-14
               2
                         Base         4:2:0      720/576/30      10368000       15            1835008          SP@ML
3             0
                         Spatial      4:2:0       1440/1152印     47001 600      a)            7 340032         Spt@H-14
                l
                          SNR         4:2:0       1440/11521印     47 以Dl 600     80           9781 248         HP@H-14
               2
                                       4:2:0      720/576/30      10368 000      15            1 835008        SP＠入'11.
3              0          Base
                          Spati出       4:2:0      1440/1152／印 47001 600          60            7 34O032        Spt@H-14
                l
                          SNR          4:2:2      1440/1152/的 47001600           80            9781248         HP@H-14
               2
                          Base         4:2:0      720/576/30      10368 000      15            1 835008        SP@ML
3              0
                          Spatial     中2:0        1440/11521的     62668800       a)            734O032         HP@H-14
                 l
                          SNR          4:2:0      1440/1152印      62668800       80            9781 248        HP@H-14
                2
                          Base         中2:0       720/576/30      10368000       15            1835008         SP@ML
3               0
                          Spatial      4:2:2      1440/1152/的 47001 600          60            7340032         HP@H-14
                 l
                          SNR          4:2:2      1440/1152/印 47001 600          80            9781 248        HP@H-14
                 2
                          Base         4:2:0      352/288/30      3041280        4             475 136         MP@LL
3               0
                          Spatial      4:2:0      1440/1152/印 47001 600          60            7 340032        Spt@H-14
                  l
                          SNR          4:2:0       1440/11521的    47001 600      80            9781 248        HP@H-14
                 2
                          Base         4:2:0       352/288/30      3041280       4              475 136        MP@LL
    3            0
                          Spatial      4:2:0       1440/11521的     47001 600      60            7340032         Spt@H- 14
                  l
                          SNR          4:2:2       14.40/1152/60   47001 600      80           9781 248        HP@H-14
                  2
                          Base          4:2:0      3521288/30      3041280        4             475 136         MP@LL
    3             0
                           Spati심       4:2:0      1440/1152160    62668800       60            7 340032        HP@H-14
                   l
                           SNR          4:2:0      1440/1152印      62 668 800     80            9781 248        I-IP@H-14
                  2
                                        4:2:0      352/288/30      3041280        4             475 136         MP@I工
    3             0        Base
                           Spati띠       4:2:2      14.40/1152/60   47001 600      60            7 340032        HP@H-14
                   l
                           SNR          拿2:2       1440/1152／的     47001 600      80            9781248         HP@H-14
                   2
                           Base         4:2:0      720/576/30      10368000       15            1835008         MP@ML
    3              0
                           Spatial      4:2:0      1440/1152/的     47001 600      60            7 340 032        Spt@H-14
                   l
                           SNR          4:2:0      1440/1152的      47001 600      80            9781 248        HP@H-14
                   2
                           Base         4:2:0      720/576/30      10368000       15            1 835008         MP@ML
    3              0
                           Spatial      4:2:0       1440/1152/60   47001600       a0            7 340032         Spt@H-14
                    l
                           SNR          4:2:2       1440/1152/60   47001 600      80            9781248          HP@H-14
                   2
                           Base         4:2:0       720/576/30      10368000       15            1835008         MP@ML
    3              0
                           Spatial      中2:0        1440/1152/60   62668800       60             7 340032        HP@H-14
                    l
                           SNR          中2:0        1440/1152／印 62668800           80            9781248         HP@H-14
                    2
                           Base          4:2:0      720/576/30      10368 000      15            1835008         MP@ML
    3               0
                            Spatial      4:2:2      1440/1152/的     47001 600      60            7 340 032       HP@H-14
                     l
                            SNR          4:2:2      1440/1152160    47001 600      80            9781 248        1-IP@H-14
                     2
                                                                                                                   293



3        0          Base       4:2:0          720/576/30     14745600           20             2441216     HP@ML
         l          Spati出     中2:0           1440/11521印    62668800           60             7340032     HP@H-14
         2          SNR        4:2:0          1440/1152/印    62668800           80             9781 248    HP@H-14
3        0          Base       4:2:0          720/576/30     14745600           20             2441216     HP@ML
         l          Spatial    4:2:0          1440/1152/ 刃   47001 600          60             7340032     HP@H-14
         2          SNR        4:2:2          1440/1152印     47001 600          80             9781 248    HP@H-14
3        0          Base       4:2:0          720/576/30     14745600           20             2441216     HP@ML
         l          Spatial    4:2:2          1440/1152/60   47001600           60             7340032     HP@H-14
         2          SNR        4:2:2          1440/1152/60   47001 600          80             9781248     HP@H-14
3        0          B沓e        4:2:2          720/576/30     11 059 200         20             2441216     HP@ML
         l          Spatial    4:2:2          1440/1152/60   47001 600          60             7340032     HP@H-14
         2          SNR        4:2:2          1440/1152/60   47001 600          80             9781248     FLP@H-14




                        표6-57 High profile @ High level (Base Layer) (MPEG IS : Table E -42)
No. of   layer id   Sc拙小Ic     Chroma         Maximum        Maximum            Maximu         Maximum     Profile    and
layers              mode       Format         sample         sax叩le rate        m total bit    total VBV   level
                                              density                           rate           buffer      indication
                                              (H/V/F)                           /1000000
l        0          Base       4:2:0          1920/1152/印    83558400           100            12222464    HP@HL
l        0          Base       4:2:2          1920/1152/60   62668800           100            12222464    HP@HL



                                    표6-58 High profile @ High level ( Base Layer + SNP)
                                                 MPEG IS : Table E -43
No. of   layer id   Scalable   Chroma         Maximum        Max血皿'In      Maximum            Maximum      Profile    and
layers              mode       Format         sample         sample rate   幻tal bit           的tal VBV     level
                                              density                      rate               buffer       indication
                                              (WV/I今                       /1000000
2
         으          蠶                    0。
                                              720/576/30
                                              720/576/30
                                                             10368000
                                                             10368 000     品                  1 835008
                                                                                              12222464
                                                                                                           SP@ML
                                                                                                           HP@1丑‘

         으          蠶          撰                                           儡
                               岩：
2                                             720/576/30     10368000                         1 835008     SP@ML
                                              720/576/30     10368000                         12222464     HP@HL
2
         으          謐          榴              352/288/30
                                              352/288/30
                                                             3041280
                                                             3041280       41。。
                                                                                              475 136
                                                                                              12222464
                                                                                                           MP@LL
                                                                                                           HP@HL
2
         으          蠶          擢              352/288/30
                                              352/288/30
                                                             3041280
                                                             3041280       41。。
                                                                                              475 136
                                                                                              12222464
                                                                                                           MP@LL
                                                                                                           HP@HL
2
         으          蠶          4:
                                  0
                               4: 。
                                    2:
                                              720/576/30
                                              720/576/30
                                                             10368 000
                                                             10368000      1늚                 1 835008
                                                                                              12222464
                                                                                                           MP@ML
                                                                                                           HP@HL

         으          蠶                                                      協
                                    2:
2                                             720/576/30     10368000                         1 835008     N[P＠入41J
                                         02   720/576/30     10368 000                        12222464     HP@HL

         으          謐
                               岩：
2                              4:   2:
                                              1440/1152印     47001 600                        7340032      入'IP@H-14
                                    :40
                                     2:。      1440/1152/60   47001 600                        12222464     HP@HL

         으          盜          撰
                                                                           쀼0
2                                             1440/1152/60   47001 600                        7340032      MP@H-14
                                              t440/l152/ 刃   47001 600                        12222464     HP@HL

         으          謐          ：썲
                                                                           잃0
2                                             1920/1152/60   62668800                         9781248      MP@HL
                                              1920/1152/ 刃   62668800                         12222 464    HP@HL

         으          蠶
                                                                           쁨0
2                                             1920/1152/60   62668800                         9781 248     MP@HL
                                         02   1920/1152/60   62668800                         12222 464    HP@HL

         으          謐                    응
                               岩：
                                                                           쁨0
2                                             720/576/30     14745600                         1 835008     HP@ML
                                              720/576/30     14745600                         12222464     HP@HL

         으          謐
                               岩：
                                                                           꼲0
2                                             720/576/30     14745600                         1 835008     HP@ML
                               茗：        02   720/576/30     14745600      끊0                 12222 464    HP@HL
              MPEG
    294       VIDE0




2
          우           謐          :：를:
                                                        2
                                                             720/576乃0
                                                             720/57的0
                                                                            11059200
                                                                            11059200
                                                                                                           1 835008
                                                                                                           12222 464
                                                                                                                        HP@ML
                                                                                                                        HP@I-IL

          우           蠶          擢
                                                   :2
                                                                                          끊0
2                                                            1440/1152160   62668 800                      9781 248     HP@H-14
                                                             1440/1152/60   62668 800                      12222 464    HP@HL

          으           蠶
                                                                                          器0
2                                :：를：                        1440/1152/60   62668 800                      9781248      HP@H-14
                                                        02   1440/1152/60   62668800                       12222464     HP@HL

          으           蠶          ：믈：
                                  二
                                                                                          器0
2                                                            1440/1152印     47001 600                      9781 248     I표@H-14
                                                             1440/1152印     47001 600                      12222464     HP@HL

          으           蠶
                                                                                          器0
2                                4:2:                        1920/1152印     83558400                       9781 248     HP@HL
                                     。                       1920/1152印     83558400                       12222 464    HP@HL

          으           蠶
                                        :40   2:                                          쀼0
2                                :：二：
                                                             1920/1152/60   62668800                       9781248      HP@HL
                                                        02   1920/1152/60   62668 800                      12222464     HP@HL

          으           蠶                             를
                                                                                          器0
2                                                            1920/1152印     62668800                       9781 248     HP@HL
                                 :：를：
                                                             1920/1152印     62668800      쀼0
                                                                                                           12222 464    HP@HL



                                 표6-59 High profile @ High level ( B그se Layer + SpatiaD
                                              (MPEG IS : Table E - 44)
No. of    layer Id    Scalable   C뇨1丑na                      Madmum         Ma虹mum        Ma虹mum            Maximum     Pmfile     and
layers                mode       Format                      sample         sample rate   total bit rate    tot日 VBV    level
                                                             density                      /1000000          buffer      indication
                                                             (H/V/F)
2
          우           Base
                      Spatial    擺                           352/288/30
                                                             1920/1152/印
                                                                            2534400
                                                                            83558400
                                                                                                            327 680
                                                                                                            12222 464
                                                                                                                        ISO 11172
                                                                                                                        HP@HL

          오                      擢
                                                                                            當6
2                     Base                                   352/288/30     2534400                         327 680     ISO 11172
                      Spatial                                1920/11521印    62668800                        12222464    HP@HL

          으                      擺                                                        品
                                                                                            崙6
2                     Base                                   720/576/30     10368000                        1 835 以08   SP@ML
                      Spatial                                1920/11521印    83558400                        12222464    HP@HL
2
          우           Base
                      Spatial
                                 :：를：
                                                        02
                                                             720/576/30
                                                             1920/1152/印
                                                                            10368000
                                                                            62668800      儡                 1 835008
                                                                                                            12222 464
                                                                                                                        SP@ML
                                                                                                                        HP@HL
2
          으           Base
                      Spatial
                                 :：를：                   0。   3521288/30
                                                             1920/1152160
                                                                            3041 280
                                                                            83558400
                                                                                                            475 136
                                                                                                            12222464
                                                                                                                        MP@LL
                                                                                                                        HP@HL

          으
                                                                                          寸00
2                     Base                                   3521288/30     3041280                         475 136     MP@LL
                      Spatial                           02   1920/11521印    62668800      41。。              12222464    HP@HL

          오                      擺                                                        儡
                                 岩：
2                     Base                                   720/576/30     10368000                        1 835008    MP@ML
                      Spatial                                1920/1152/60   83558400                        12222464    HP@HL
2
          으           Base
                      Spatial    擢                           720/576/30
                                                             1920/1152160
                                                                            10368000
                                                                            62 的8800      1듦                1 835008
                                                                                                            12222464
                                                                                                                        MP@ML
                                                                                                                        HP@HL
2
          오           Base
                      Spatial     응                          9日)/57日30
                                                             1920/11521的
                                                                            19 660 800
                                                                            83558400
                                                                                                            3047424
                                                                                                            12222464
                                                                                                                        MP@H-14
                                                                                                                        HP@HL

          으
                                                                                          료）
                                 :：를：
2                     Base       :：弓：                        960/576/30     196（刃 800                       3047424     MP@H-14
                      Spatial                           02   1920/11521的    62668800                        12222 464   HP@HL

          우                      擺
                                                                                          往）
2                     Base                                   720/576/30     14745600                        2441216     HP@ML
                      Spatial                                1920/11521印    83558400                        12222464    HP@HL

          으
                                                                                          꼲0
2                     Base                                   720/57日30      14745600                        2441216     HP＠入4L
                      Spatial                           02   1920/11521的    62668800                        12222464    HP@HL

          으                      撰
                                                                                          쀼0
                                 岩：
2                     Base                                   720/57日30      11 059200                       2441216     HP@ML
                      Spati키                                 1920/11521的    626688어：}                       12222464    HP@HL

          으
                                                                                          쁩0
2                     Base       4:
                                              2:             960/576/30     19660800                        3047424     HP@H-14
                      Spati고            :40
                                          。                  1920/1152/60   83558400                        12222464    HP@HL

          우                      擢
                                                                                          往）
                                              2:
2                     Base                                   960/576/30     19660800                        3047424     HP@H-14
                      Spati심                                 1920/1152/60   62668800      往）                12222464    HP@HL
2         0           Base       4:2:2                       960/576/30     14745600      25                3047424     HP@H-14
                                                                                                                             295



                     l         I Spatial    1 4:2:2   I 1920/1152160 I 62 668 800 I 100                I 12222464 1 FIP@HL            1

                                           표 白的 High profile @ 네gh level (Base 山yer + SNR + Sp（州이）
                                                            (MPEG IS: Table E -45)
    No. of          layer id    Scalable     Chroma    Maximum          入laximum       Ma川mum           Maxunum       Profile   and
    layers                      mode         Format    sample           sample rate    tot日 bit rate    tot고 VBV      level
                                                       density                         /1     刃         buffer        mdication
                                                       (H/V/E)
    3                0           Base         4:2:0     352/288/30       3041280        3                3仗）恥8         SP@ML
                      l          SNR         中2:0       352/288/30       3041280        4                475 136       SNR(@I工
                     2           Spatial      4:2:0     1920/11521的      83558400       100              12222 464    HP@HL
    3                0           Base         4:2:0     352/288/30       3041280        3                3＆나48         SP@ML
                     l           SNR          4:2:0     352/288乃0       3041280         4               475 136       SNR@I工
                     2           Spati심       4:2:2     1920/1152/60    83558400        100             12222464      HP@HL
    3               0           Base         中2:0       720/576/30      10368000        10              1212416       SP@ML
                     l          SNR          4:2:0     720/576/30       10368000        15              1 835 어猪      SNR@ML
                     2          Spati出       4:2:0      1920/1152/60    83558 400       100             12222464      HP@HL
    3               0           Base         中2:0      720/576/30       10368000        10              1212416       SP@ML
                     l          SNR          4:2:0     720/576/30       10368000       15               1 835008      SNR@ML
                    2           Spat洌        4:2:2     1920/1152/60     62668800       100              12222 464     HP@HL
3                  0            B朗e          中2:0      720/576/30       10368000       15               1 835008      SP@ML
                    l           SNR          4:2:2     720/57日30        10 368 000     20               2441216       HP＠入4L
                    2           Spatial      4:2:2     1920/1152/60     62668800       100              12222 464     HP@HL
3                  0            Base         4:2:0     352/288/30       3041280        3                3日：1448       入4P@LL
                    l           SNR          4:2:0     3521288/30       3041280        4                475 136       SNR@LL
                   2            Spatial      中2:0      1920/1152/60     83558400       100              12222464      HP@HL
3                  0            Base         4:2:0     352/288/30       3041280        3                3＆나48         MP@LL
                   l            SNR          4:2:0     352/288/30       3041280        4                475 136       SNR@LL
                   2            Spatial      4:2:2     1920/1152/60     62668800       100              12222464      HP@HL
3                 0             Base         4:2:0     720/576/30       10368000       10               1212416       MP@ML
                  1             SNR          4:2:0     72아576/30        10368000       15               1 835008      SNR@ML
                  2             Spatial      4:2:0     1920/1152160     83558400       100              12222464     HP@HL
3                 0            Base          4:2:0     720/57日30        10368000       10               1212416      N下＠N1L
                   l           SNR          中2:0       720/576/30      10368000        15              1 835008       SNR@ML
                  2            Spatial      4:2:2      1920/1152/60    62668800       100              12222 464     HP@HL
3                 0            Base         4:2:0     720/576/30       10368000        15              1 835008      MP@ML
                  l            SNR          4:2:2     720/576/30       10368000       20               2441216       HP@ML
                  2            Spatial      4:2:2      1920/1152160    62668800       100              12222 464     HP@HL
3                0             Base         4:2:0     960/576/30       196（刃 800      20               2441216       MP@H-14
             _
                  1            SNR          4:2:0     9（刃／576/30       19660800       25               3047424       Spt@H-14
                 2             Spatial      4:2:0     1920/1152/60     83558 400      100              12222464      HP@HL
3                0             Base         4:2:0     960/576/30       19660800       20               2441216       MP@H-14
                  l            SNR          中2:0      960/576/30       19660800       25               3047424       Spt@H-14
                 2             Spatial      4:2:2     1920/1152/60     62668800       100              12222 464     HP@HL
3                0             Base         4:2:0     960/576/30       14745600       20               2441216       入IP@H-14
                 l             SNR          4:2:2     960/576/30       14745600       25               3047424       HP@H-14
                 2             Spatial      中2:2      1920/1152/60     62668800       100              12222464      HP@HL
3                0             Base         4:2:0     720/576/30       14745600       15               1 835008      HP@ML
                 l             SNR          4:2:0     720/576/30       14745600       20               2441216       HP@ML
                 2             Spatial      中2:0      1920/1152/60     83558 400      100              12222464      HP@HL
3                0             Base         中2:0      720/576/30       14745600       15               1 835 以）8     HP@ML
                 l             SNR          4:2:0     720/576/30       14745600       20               2441216       HP@ML
                 2             Spatial      4:2:2     1920/11521印      62668800       100              12222464      HP@HL
3                0             Base         4:2:0     720/576/30       11 059200      15               1 835008      HP＠小4L
3
         二
         0
                    SNR
                    Spatial
                    Base
                                  4:
                                  4: 2
                                  4:2:2
                                       2:
                                       2:
                                            2   720/576/30
                                                1920/1152./的
                                                               11 059 200
                                                               62668 800     꼼0
                                                                                              2441 216
                                                                                              12222 464
                                                                                                          HP＠入4L
                                                                                                          FIP@HL
                                                                                                          I-il기孕N1L
                                                720/576/30     11 059200     15               1 835008
         l          SNR           4:2:2         720/57日30      11 059200     20               2441 216    HP@ML
         2          Spatial       4:2:2         1920/1152／的    62668 800     100              12222 464   HP@HL
3        0          Base          4:2:0         960/576/30     19660800      20               2441216     HP@H-14
         l          SNR           4:2:0         9（刃／576/30     19660800      25               3047424     HP@H-14
         2          Spatial       4:2:0         1920/1152/60   83558400      100              12222 464   HP@HL
3        0          B小e           4:2:0         960/576/30     196（刃 800     20               2441216     HP@H-14
         l          SNR           4:2:0         960/576/30     19660800      25               3047424     HP@H-14
         2          Spatial       4:2:2         1920/11521印    62668800      100              12222 464   HP@HL
3        0          Base          4:2:0         960/576/30     14745600      20               2441216     HP@H-14
         l          SNR           4:2:2         960/576/30     14745600      25               3047424     HP@H-14
         2          Spatial       4:2:2         1920/1152/的    62668800      100              12222464    HP@HL
3        0          Base          4:2:2         960/576/30     14745600      20               2441216     HP@H-14
         l          SNR           4:2:2         아刃巧76/30       14745600      25               3047424     HP@H-14
         2          Spatial       4:2:2         1920/1152/印    62668 800     100              12222464    HP@HL



                               표 a 句 High pro셰e @ High level ( Base Layer + Spa旅미 + SNR)
                                              (MPEG IS : Table E - 46)
No. of   layer id   Scalable      C노oma         Maximum        Maximum       卜4aximum         Maximum     Profile    and
layers              mode          Fonnat        sample         sample rate   total bit rate   total VBV   level
                                                density                      /1000000         buffer      indication
                                                (H/V/I乃
3        0          Base         中2:0           352/288/30     2534400       1.856            327 680     ISO 11172
         l          Spatial      4:2:0          1440/1152/印    47001 텨X)     60               7 340032    Spt@H-14
         2          SNR          4:2:0          1440/1152/印    47001日Jo      100              12222 464   HP@HL
3        0          Base         4:2:0          352/288/30     2534400       1.856            327 680     ISO 11172
         l          Spatial      4:2:0          1440/11521的    47001 600     60               7 340032    Spt（孕H-14
         2          SNIR         4:2:2          1440/1152/的    47001600      100              12222 464   HP@HL
3        0          Base         4:2:0          352/288/30     2534400       1.856            327 680     ISO 11172
         l          Spatial      4:2:0          720/576/30     14745600      20               2441216     HP（카vIL
         2          SNR          4:2:0          720/576/30     14745 텨Jo     100              12222464    HP@HL
3        0          Base         4:2:0          352/288/30     2534400       1.856            327 680     ISO 11172
         l          Spatial      4:2:0          720/576/30     14745600      20               2441216     HP@ML
         2          SNR          4:2:2          720/576/30     14745600      100              12222464    HP@HL
3        0          Base         4:2:0          352/288/30     2534400       1.856            327 680     ISO 11172
         l          Spatial      4:2:2          720/576/30     11 059200     20               2441216     HP@ML
         2          SNR          4:2:2          720/576/30     11 059200     100              12222 464   HP@HL
3        0          Base         中2:0           352/288/30     2534 400      1.856            327 680     ISO 11172
         l          Spatial      中2:0           1440/1152/60   62668800      80               9781 248    HP@H-14
         2          SNR          4:2:0          1440/1152160   62668800      100              12222 464   HP（孕HL
3        0          B小e          4:2:0          352/288/30     2534400       1.856            327 680     ISO 11172
         l          Spatial      4:2:0          14.40/11521印   62668800      80               9781 248    HP@H-14
         2          SNR          4:2:2          1440/1152印     62668800      100              12222464    HP@HL
3        0          Base         中2:0           352/288/30     2534400       1.856            327 680     ISO 11172
         l          Spatial      4:2:2          1440/1152印     47001 600     80               9781 248    FIP@H-14
         2          SNR          4:2:2          1440/1152印     47001 600     100              12222464    HP@HL
3        0          Base         4:2:0          352/288/30     2534400       1.856            327 680     ISO 11172
         l          Spatial      4:2:0          1920/1152/60   83558400      80               9781 248    HP@HL
         2          SNR          4:2:0          1920/1152160   83558400      100              12222464    HP@HL
3
         우          Base
                    Spatial
                                  4:   2:
                                       :40
                                       2:。
                                                352/288/30
                                                1920/1152/60
                                                               2534400
                                                               62668800       喆56
                                                                                              327 680
                                                                                              9781 248
                                                                                                          ISO 11172
                                                                                                          HP@HL
                                                                                    297



    2    SNR        中2:2    1920/1152/60    62668 800     100     12222464    HP@HL
3   0    Base       4:2:0   352/288/30      2534400       1.856   327 680     ISO 11172
    l    Spatial    4:2:2   1920/1152印      62668800      80      9781248     HP@HL
    2    SNR        4:2:2   1920/1152/印     626688（刃      100     12222 464   HP@HL
3   0    Base       4:2:0   720/576/30      10368000      15      1 835008    SP@ML
    l    Spatial    中2:0    1440/1152/60    47 cx끄 600    60      7340032     Spt（包H-14
    2    SNR        4:2:0   1440/1152/的     47001 600     100     12222 464   HP@HL
3   0    Base       4:2:0   720/576/30      10368000      15      1835008     SP@ML
    l    Spati심     4:2:0   1440/11521印     47001 600     8)      7340032     Spt@H-14
    2    SNR        4:2:2   14.40/1152/60   47001600      100     12222 464   HP@HL
3   0    Base       4:2:0   720/576/30      10368000      15      1 835008     SP@ML
    l    Spatial    4:2:0   1440/1152／印     62668800      80      9781 248    HP@H-14
    2    SNR        4:2:0   1440/1L52/60    62668800      100     12222464    HP@HL
3   0    Base       4:2:0   720/576/30      10368 000     15      1 835008     SP@ML
    l    Spatial    4:2:0   1440/11521的     62668800      80      9781 248    HP@H-14
    2    SNR        4:2:2   1440/1152/的     62668800      100     12222464    HP@HL
3   0    Base       4:2:0   720/576/30      10368000      15      1 835008     SP@ML
    l    Spatial    4:2:2   1440/1152/60    47 (）아 600    80      9781 248    HP@H-14
    2    SNR        4:2:2   1440/1152/的     47001 600 '   100     12222464    HP@HL
3   0    Base       4:2:0   720/576/30      10368000      15      1 835008     SP@ML
    l    Spatial    4:2:0   1920/1152/60    83558400      80      9781 248    HP@HL
    2    SNR        4:2:0   1920/1152/印     83558400      100     12222 464    HP@HL
3   0    Base       4:2:0   720/576/30      10368000      15      1 835008     SP@ML
    l    Spatial    4:2:0   1920/1152印      62668800      80      9781248     HP@HL
    2    SNR        中2:2    1920/1152/60    62668800      100     12222464    HP@HL
3   0    Base       4:2:0   720/576/30      10368000      15      1 835008     SP@ML
    l    Spatial    4:2:2   1920/1152/60    62668800      80      9781 248     HP@FIL
    2    SNR        4:2:2   1920/1152/60    62668800      100     12222464     HF@HL
3   0    B沓e        中2:0    352/288/30      3041280       4       475 136      MP@LL
    l    Spatial    4:2:0   1440/1152/60    47001600      60      7340032      Spt@H-14
    2    SNR        4:2:0   1440/1152/60    47001 600     100     12222464     HP@HL
3   0    Base       4:2:0   352/288/30      3041280       4       475 136      MP@LL
     l   Spat洌      4:2:0   1440/1152/的     47001600      60      7 340032     Spt@H-14
    2    SNR        4:2:2   1440/1152/60    47001600      100     12222 464    HP@HL
3   0    Base       4:2:0   352/288/30      3041280       4       475 136      MP@LL
    l    Spatial    4:2:0   720/576/30      14745600      20      2441216      HP@ML
    2    SNR        4:2:0   720/576/30      14745600      100     12222464     HP@HL
3   0    Base       4:2:0   352/288/30      3041 280      4       475 136      MP@LL
     l   Spatial    4:2:0   720/576/30      14745600      20      2441 216     HP@ML
    2    SNR        4:2:2   720/576/30      14745 600     100     12222 464    HP@HL
3   0    Base       4:2:0   352/288/30      3041280       4       475 136      MP@LL
     l   Spatial    4:2:2   720/576/30      11 059200     20      2441 216     HP@ML
    2    SNR        4:2:2   720/576/30      11 059200     100     12222464     HP@HL
3   0    Base       4:2:0   352/288/30      3041280       4       475 136      MP@I工
     l   Spatial    4:2:0   1440/1152/60    62668800      80      9781 248     HP@H-14
    2    SNR        4:2:0   1440/1152/印     62668800      100     12222464     HP@HL
3   0    Base       中2:0    352/288/30      3041280       4       475 136      MP@I工
     l   5-         4:2:0   1440/1152/60    62668800      80      9781 248     HP@H-14
    2    SNR        4:2:2   1440/1152/的     62668800      100     12222464     HP@HL
3   0    Base       4:2:0   352/288/30      3041280       4       475 136      MP@LL
     l   Spatial    4:2:2    1440/1152/60   47001 600     80      9781248      HP@H-14
     2   SNR        中2:2    1440/1152/60    62668800      100      12222464    HP@HL
3    0   Base       4:2:0   352/288/30       3041280      4       475 136      MP@LL
     l    Spatial   4:2:0    1920/1152/的     83558400     80      9781248      HP@HL
     2    SNR       4:2:0    1920/1152/60    83558400     100     12222464     HP@HL
3   0    Base       4:2:0   352/288/30       3041280      4       475 136      MP@LL
    298




3
           二0
                  Spatial
                  SNR
                  Base
                            擢          1920/1152/60
                                       1920/1152/60
                                                       62 的8800
                                                       62668 舡10     쁨
                                                                         ［)
                                                                               9781 248
                                                                               12222464
                                                                                            HP@HL
                                                                                            HP@HL
                             4:2:0    352/288/30       3041280       4         475 136      MP@I工
             l    Spati고     4:2:2     1920/1152/60    62 的8800      80        9781 248     HP@HL
            2     SNR        4:2:2    1920/1152印       62668800      100       12222464     HP@HL
3           0     Base       4:2:0    720/57日30        10368000      15        1 835008     MP@ML
             l    Spatial    4:2:0    1440/1152印       47 어：11600    a)        7340032      Spt@H-14
            2     SNR        4:2:0    1440/1152印       47001 600     100       12222 464    HP@HL
3           0     Base       4:2:0    720/576/30       10368000      15        1 835008     MP@ML
             l    Spati出     4:2:0    1440/1152印       47001 600     a)        7340032      Spt@H-14
            2     SNR        4:2:2    1440/1152/60     47001 600     100       12222464     HP@HL
3          0      Base       4:2:0    720/576/30       10368000      15        1 835008    MP@ML
            l     Spatial   中2:0      1440/1152印       62668800      80        9781 248     HP@H-14
           2      SNR        4:2:0    1440/1152印       62668800      100       12222464    HP@HL
3          0     Base        4:2:0    720/576/30       10368 000     15        1 835008    MP@ML
            l     Spatial    4:2:0    1440/1152/60     62668800      80        9781 248    HP@H-14
           2     SNR        4:2:2     1440/1152印       62668800      100       12222464    HP@HL
3         0      Base       4:2:0     720/576/30       10368000      15       1 835008     MP@ML
            l    Spatial     4:2:2    1440/1152印      47001 600      80       9781 248     HP@H-14
           2     SNR        4:2:2     1440/1152印      47001 600      100      12222464     HP@HL
3         0      Base       4:2:0     720/576/30      10368000       15       1 835008     MP@ML
           l     Spatial    4:2:0     1920/1152/印     83558400      80        9781248      HP@HL
           2     SNR        4:2:0     1920/1152/60    83558400      100       12222 464    HP@HL
3         0      Base       4:2:0    720/576/30       10368000      15        1 835008     MP@ML
           l     Spatial    4:2:0     1920/1152/的     62668800      80        9781 248     HP@HL
          2      SNR        4:2:2     1920/1152/60    62668800      100       12222 464    HP@HL
3         0      Base       4:2:0    720/57日30        10368000      15        1 835008     MP@ML
          1      Spatial    4:2:2    1920/1152/印      62668 800     80        9781248      HP@HL
          2      SNR        4:2:2    1920/1152/印      62668800      100       12222 464    HP@HL
3         0      Base       中2:0     960/57日30        196印 800      25        3047424      HP@H-14
          l      Spatial    4:2:0    1920/1152/60     83558400      80        9781 248     HP@HL
          2      SNR        4:2:0    1920/1152/印      83558400      100       12222 464    HP@HL
3         0      Base       4:2:0    9（刃／576/30       19660800      25        3047424      HP@H-14
          l      Spa丘a!     4:2:0    1920/1152印       62668800      80        9781 248     HP@HL
          2      SNR        4:2:2    1920/1152印       62668 800     100       12222464     HP@HL
3         0      Base       4:2:0    9（又)/576/30      19660800      25        3047424      HP@H-14
          l      Spatial    中2:2     1920/1152/60     62668800      80        9781 248     HP@HL
          2      SNR        4:2:2    1920/1152印       62668800      100       12222464     HP@HL
3         0      Base       4:2:2    960/576/30       14745600      25        3047424      HP@1玉14
          l      Spatial    4:2:2    1920/1152/60     62668800      80        9781248      HP@HL
          2      SNR        4:2:2    1920/1152/60     62668800      100       12222464     HP@HL
     부록 1 : 참고문헌과 국제규격

1     Arun N. Ne仕avali & Barry G. Haskell "Digital Pictures, representation and
      compression" Plenum Press, 1988
2     Didier Le Gall "入PEG: A Video Compression Standard for Multimedia Applications"
      Trans. ACM, April 1991
3     C Loeffler, A Ligtenberg, G S Moschytz "Practical fast 1-D DCT algori仕1ms with 11
      multiplications" Proceedings IEEE ICASSP-89, Vol. 2, pp 988-991, Feb. 1989
4     See the Normative Reference for Recommendation IT工R BT.601
5     See the Normative Reference for JEC Stand町d Publica如n 461
6     See the Normative Reference for Recommendation 1T工T H.261
7     See the Normative reference for IEEE Stan由rd Specification P1180-1990
8     ISO/IEC 10918-li 1TU-T T.81 (JPEG)
9     E Viscito and C Gon乙ales "A Video Compression Algorithm with Adaptive Bit
      Allocation and Quantization", Proc SPIE Visual Communications and Image Proc '91
      Boston MA November 10-15 Vol. 1605 205, 1991
10    A Puri and R Aravind "Motion Compensated Video Coding with Adaptive Perceptual
      Quantization", IEEE Trans. on Circuits and Systems for Video Tec노lology, Vol. 1 pp
      351 Dec. 1991.
11    C. Gonzales and E. Viscito, "Flexibly scalable digital video coding". Image
      Communications, Vol. 5, Nos. 1-2, February 1993
12    A.W.Johnson, T.Sikora and T.K. Tan, "Filters for Drift Reduction in Frequency
      Scalable Video Coding Schemes" ＜乃ansmittedfor까I疵C口加2加夙ec加毗I石玎ers.>
13    R.Mokry and D.Anastassiou, "八inimal Error Drift in Frequency Scalability for
      Motion-Compensated DCT Coding". IEEE Transactions on Circuits and Systems for
      Video Technology, <acceptedfor publication>
14    K.N. Ngan, J. Arnold, T. Sikora, T.K. Tan and A.W. Johnson. "Frequency Scalability
      Experiments for 入PEG-2 Standard". Asia-Pacific Conference on Communications,
      Korea, August 1993.
15    T. Sikora, T.K. Tan and K.N. Ngan, "A Performance Comparison of Frequency
      Domain Pyramid Scalable Coding Schemes Within the MPEG Framework". Proc.
      PCS, Picture Coding Symposium, Lausan此 pp. 16.1 - 16.2, Switzerland March 1993.
16    Masahiro Iwahashi, "Motion Compensation Technique for 2:1 Scaled-down Moving
      Pictures". 8-14, Picture Coding Symposium '93.
 300




17     Sikora, T. and Pang, K., "Expe血ents with O加mal Blo出Overlapping Filters for Cell
       Loss Conce汕ment in Packet Video", Proc I日E Visual Signal Processing and
       Com 毗cations Workshop, Melbourne, 21-22 Sept. 1993, pp. 247-250.
18     A. Pun "Video Coding Using the 入4PEG-2 Compression Standard", <to appear> Proc
       SPIE Visual Communications and Image Proc '93 Boston MA November,1993.
19     A. Pun and A. Wong "Spatial Do曲in Resolution Scalable Video Coding", <to
       appear> Proc SPIE Visual Communications and Image Pr乂 '93 Boston 入A
       November,1993.
                                                                                                    區
                                                                                                    MPEG
                                                                                                    뮈DE0
                                                                                                            301



   부록 2: MPEG2의 이ementary stream의 예
MPEG-2 SAMPLE BIT STREAM
[beginning of sequence]

SEQUENCE- HEA［가三日＜LODE            : len=16, \／刻＝=    0                                '0000000000000000]
                                  : Ien=16, val=                      435             '0000000110110011]
horizontal-size-value             : len=12, val=                      704             '001011000000']
vertical-size-value               : len=12, va느                       480             '000111100000]
aspect-rat山니n幻rmation             닉en= 4, v졔＝        2                                '0010']
frame寸카e-code                     : len= 4, V줴＝      4                                 '0100']
b作ra也－v졔ue                        : Ien=18, v졔＝            10000                       '어）0010011100010000]
marker-b吐                          : len= 1, v졔＝     ]                                네］
vbv-buffer-size-value              : len=10, val=                     112             '00011100001


                                                                                       0 n U
                                                                                         U n
constrained-parameter-flag        : len= 1, val=     0
load-intra-quantizer-matrix        : len= 1, val=    0
 幻ad-no口intra띠uantizer-matrix      : len= 1, v졔＝     0

SEQUENCE EXTENSION                : len=16, val=     0                                '0000000000000000']
 . . EXTENSION START CODE         : len=16, val=                      437             '0000000110110101']
extension-id-sequence-extension   : len= 4, val=     ]                                '000川




                                                                              在이叫叫叫
                                  : len= 8, va느                                        010（거 ()00']
profile-and-level-indication




                                                         0]000]0000
progressive-sequence              : len= 1, va느
chroma-format                     : len= 2, val=
honzonta卜size-exten引on            : 陀n= 2, va느
vertica卜삶ze＝터dens山n               : len= 2, v례＝
b牛ra也－exten섧on                    : 冶n=12, \／刻＝                         000000000000']
marker-bit                         : len= 1, val=                      '1
                                                                             ']
vbv-b마他n引ze．이dension               : len= 8, V졔＝                        00000000]
lo小尸d쉬ay                           : len= 1, va느                                       0    ']
frame-rate-extension-n             : len= 2, val=                           00'1
frame-rate-extension-d             : len= 5, va느                            00000']

 GROUP-START-CODE                  : len=16, val=  0 '00000000000000000]
                                   : len=16, va느       440      '00000001101111000']
 time-code                         : len=25, val=  5246976
                                   '0010100000001000000000000']
 closed-gop                        : Ien= 1, val=[ 0                                    0
                                                                                               ']
 broken-link                       : len= 1, v졔=[   0 '0]
 {byte-align)                      : len= 5, val=[ 0 '00000']

 PICTURE-START-CODE                : len=16, val=[       0            '0000000000000000']
                                   : Ien=16, val=[           256      '0000000100000000']
 temporal-reference                : len=10, va느[        0 '0000000000]
 口cture-cc乂小ng-type                : Ien= 3, \／계＝[       ]    00기
                                   : len=16, val=[         30877      '0111100010011101']
 vbv-delay
 extra-bit                         : len= 1, val=[       0             '0']
 { byte-align }                    : len= 2, val=[       0 '00]

 PICTURE CODING EXTENSION          : Ien=16, val=[        0             '0000000000000000']
 . . . EXTEN듸O사STA日T-CODE          : len=16, va느［                       437        '00000001101］이0川
 extension-id-picture-coding       : len= 4, val=[         8                       '1000']
 幻八vard-horizont졔＋code             : len= 4, \／졔놔                        15        너］11']
 幻rwan弘厄rtica卜寸（ode                : 陀n= 4, va느［                         15        '1111]
 backward七orizonta나（ode            : len= 4, v궤＝[                        15        너］11']
 backward-vertica卜卜code            : len= 2, \／싫놔                        15        녀111]
     302




                                                                              0버삐이이이삐
  intra-dc-precision                          : Ien= 2,      val=
                                                                    U
                                                                    Q                        00']
 picture-structure                            : len= 1,      va느
 加p十터小伽St                                                               ]
                                              : len= 1,      V졔＝
 frame甘的七ame-dct                                                    U
                                                                    n
                                              : len= 1,      V졔＝

                                                                    0 0 j
 conce례ment寸了）0的n-vectors                     ., Ien= ] ,   va느
 qsc刻e却pe                                    : len= 1,      V톄＝
 intra-vic-徊rmat                             : len= ] ,     \／졔＝二
 졔也mate-scan                                                        1
                                                                    J
                                             : len= 1,      \／톄＝



                                                                             이이이이
 repeat-first-field                                                 0
                                                                                        네］
                                             : len= 1,      val=
 chroma-420-type                                                    U
                                                                    n
                                             : len= 1,      val=

                                                                    0 0 0
 아四ressive升ame                               : len= 1,      V졔＝
 C아npos在e-display-flag                       : len= 1,      va느
 { byte-align)                               : len= 6,      val=            '000000]
 듸J0E-START-CODE                             .· 厄n=16, va느          0        '00000000000000000']
                                             : len=16, val=                 257         '00000001000000001']
 quantizer-scale-code                        : len= 5 val=                    10        '01010]
 extra-bit                                   : Ien= 1 va노           0       '0']
 PMV1 =PMV2 = PMV3 = PMV4 = (0 , 0)
 [
     0]
 macroblock-address-increment                    : len= 1 VLC=[{        1}             '1]
 macroblock-type                                 : len= 2 VLC=[{      17)              '01']
 dct-type                                        : len= 1, val=[  0 '0']
 quantizer-scale-code                            : Ien= 5, val=[  6 '00110]
 dct-dc-size-lumanance                           : len= 4, val={         5}            1110']
 d竺d口d咐erenti졔                                  : len= 5, va느［           26            11010']
    runlengtWamplitude codeword                 : len= 4, [{ 0 /      -3)             '01111']
    runlength/amplitude codeword                : len= 4, [{ 0 /       3) '01110']
    runlength'amplitude codeword                : Ien= 5, [{ 0/        4)            '111000']
    runlengtWamplitude codeword                 : len= 6, [{ 4/       -1}            '0001101']
    runlengtWamplitude codeword                 : len= 3, [{ 1 /      -1)            '0101']
    runlength'amplitude codeword                : Ien= 2, [{ 0 /      -1)            '101']
 end-of-block                                   : len= 4, VLC=[{        0)           '0110']
 dct-dc-size-lumtnance                          : len= 2, VLC=[{         2)          '01]
dct-dc-differential                             : len= 2, val=[  0 '00]
   runlingth/amplitude codeword        : len= 7,        [{ 1 /     3) '11110010']
   runlingtWamplitude codeword         : len= 4,       [{ 0 /      3) '01110']
   runlingth/amplitude codeword       : len= 2,         [{ 0/      1) 네00']
   runlingth/amplitude codeword       : len= 2,         [{ 0/    -1} '101']
   runlingth/amplitude codeword       : len= 5,         {{ 3 /     1) '001110']
   runlingth/amplitude codeword          len= 3,       [{ 0 /    -2) 녀101']
   runlingffilamplitude codeword      : len= 2,        [{ 0 /    -1) '101']
   runlingth/amplitude codeword                : len= 3, [{ 1 /         1}          '0100']
   runlingtb/amplitude codeword       : len= 5,        [{ 3 /    -1} '001111']
   runlingtli/amplitude codeword      : len= 2,        [{ 0 /    -1) '101']
  runlingth/amplitude codeword        : len= 7,        [{ 7 /      1)              '00001000']
                                                                            아와
end-of-block                                   : len= 4, VLC=[{         0)          '0110']
dct-dc-size-luminance                            !en= 2, VLC=[{         2)          '01']
dct-dc-d附erenti계                              : len= 2, v졔놔      ]                 '01']
                                                                            와아
  runlength(amplitude codeword                : len= 3, [{ 0 /          2}         '1100']
  runlength/amplitude codeword                : len= 4, {{ 0 /          3)         '0111']
  runlengthlamplitude codeword                : len= 2, [{ 0/         -1)          '101']
  runlength/amplitude codeword                : len= 7, [{ 1 /         3}          '11110010']
  runlength/amplitude codeword                : len= 3, [{ 1 /        -1)         '0101']
  runlength'amplitude codeword                : len= 2, [{ 0/         -1) '101']
  runlengtWamplitude codeword                : len= 2, [{ 0/          -1) '101']
  띠nlengthlamplitude codeword                : len= 2, [{ 0/           1) '101']
                                                                                                                                 303



  runlength/amplitude codeword          : len= 3, [{       1/                                          '0100']
  ninlengthlamplitude codeword          : len= 5, [{    2/
                                                                                                      q셔0］끼
  runlengthfamplitude codeword           .' len= 2, [{ 0/                                             녀01']
  runlengtWamplitude codeword            : len= 2, [{   0/
                                                                                                       녀00']
  runlength/amplitude codeword           : len= 2, [{ 0/                                               너00]
  띠nlength/amplitude codeword             '. len= 7, [{ 8/
                                                                                                       '00001010']
  runlengtWamplitude codeword           .1 len= 2, [{ 0/                                              녀0川
  띠nlength/amplitude codeword           : len= 3, [{ 1/                                                        '010씨
end-o卜벼ock                               : len= 4, VLC=[{                                                      '0110']
dct-dc-size-Iuminance                    : len= 3, VLC=[{                                          4}          녀10']
m斗dc-d附erential                          : len= 4, val=[  9                                        녀00끼
  runlength/amplitude codeword          : len= 5, [{                                              -4} 녀11001']
                                         .1 len= 7, [{
                                                           0/
  runlength'amplitude codeword                             2/                                     -2) '000011111']
  runlengthlamplit냐de codeword           : len= 2, [{      0/
                                                                                                  -1} '101]
  runlen아hlamplitude codeword            : len= 5, [{ 2/                                           1} '001010]
  rurilength'amplitude codeword          : len= 2, [{ 0/                                           l} 녀00']



MPEG-2 SAMPLE B汗 ST日EAM
{B-Frame }
PICTURE-START-CODE                       : len＝怜, va느                  0             '0000000000000000]
                                   : len=16, val=[                     256 '0000000100000000']
temporal-reference                       : len=10, \／刻＝                1 '0000000001']
picture-coding-type                      : len= 3, \／켸＝=               3 '011]




                                                                                                           斗쀼이叫
vbv-d이ay                                 : len=16, va느                   22598 '01011000010000110']




                                                                            0 70 700
f마pe小化rward시ec幻r                         : len= 1, \／톄＝;
幻rward-f-code                            : len= 3, V졔＝
fu作pe卜backward-vector                    : len= 1, \／졔＝二
backward-f-code                          : len= 3, va느
extra-bit                                : Ien= 1, va느
{ byte-align }                           : len= 2, va느
                                                                             0
PICTURE CO［긔NG EXTEN듸O卜J                  : len=16, val=                0                                   0000000000000000그
. . .EXTEBSUIB-START-CODE                 '. len=16, val=                                         437 '0000000110110101']




                                                                8n
                                                                 <n<2 2 0 ] 0 0 0 ] ] 0 0 0 0 0
extension-id-picture-
                    coding                : len= 4, val=                8                         네000]
幻rward巾orizonta卜卜code                     : len= 4, v졔＝                 2                          '0010']
幻rward-vertica卜f-code                     : len= 4, v졔＝                 2                          '0010']
backward-horizontal-f-code                '. len= 4, va느                2                           0010']
backward-vertical-f-code                  : len= 4, va느                 2                           0010']
intra-dc-precision                 : len= 2,      val=[                 0                           00']
picture-structure                  : len= 2,      val=[                 3                          '11']
top-field-first                   : len= 1,       val=[                 ]




                                                                         U
                                                                         Q
                                                                                                           ']
                                                                                                  '1
frame-pred-frame-dct                      : len= 1, val=                0                              0   ']
conce톄ment-mo如n-vect）田                    : len= 1, v졔＝                 0



                                                                                                  n
                                                                                                  Jn J n  ]n
                                                                                                        J n 1
                                                                                                            JnJnJ 0
                                                                                                                       0   ']
qscale却pe                                 : len= 1, va느                 0
intra小／Ic寸ormat                           : len= ] , V례＝                ]
졔伯rn카e-scan                               : len= ] , ＼尼느


                                                                                                  0 J1 41 0 0 0 0 0
repeat-first-field                        : len= ] , va느
chroma-420-type                           : len= 1, \／톄＝
아四res삶ye十ame                              : len＝二1, va느
                                                                                                  1  1  1 1 1 r 1
c아liposite-dis히ay쥐ag                      : len= ] , V졔＝                                                         0
                                                                                                                 0nU

{byte-align }                             : len= 6, val=                                                         0

SLICE-START-CODE                         : Ien=16, val=                  0                         '0000000000000000']
                                         : len＝怡, V졔＝=                                            257         '000000이0000000끼
quantizer-scale-code                     : len= 5, V졔＝                                              12 '01100']
ex打a-b仕                                  : len= 1, val=                                              0   0']
    304



PMV1 =PMV2 = PMV3 = PMV4 = (0, 0)

         '
                                                                  D斟
    0
[
macroblock-address-increment               : len= 1, VLC=[{                   네］
macrob幻ck-type                             : Ien= 6, VLC=[{                  '000011]
frame-mo如n寸叩e                       : len= 2,     val=[      2               녀0'1
dct-type                                   : len= 1, val=[   0                0     ']
quantizer-scale-code                       : len= 5, v졔놔     7               '00111]




                                                                   但삐冊끽D아D
frame m아向n vec幻r horizontal                : pmvl x= 0, val=                 '000010001
frame motion vector vertical               : pmvly= 0, va느 0
coded-block-pattem                         : len= 5, VLC=[{                  녀0010']
   runlengthlamplitude codeword            : len= 8, [{ 3/                   '001001001']
   runlength/amplitude codeword            : len= 6, [{ 7/                   '0001000']
end-o卜비ock                                 : len= 2, VLC={{                  녀0']
   runlengtWamplitude codeword             : len= 3, [{ 1/                    0110']
   runlengthlamplitude codeword            : len= 3, [{ 1/       -1}          0111']
   runlength/amplitude codeword            : len= 6, [{ 7/        1}         '0001000']
end-of-block                               : Ien= 2, VLC=[{       0}         '10]

[   1]
macr야加아c-ad야ess냐ncrement                 : len= 1, VLC=[{    1)              네］
macroblock-type                          : Ien= 2, VLC=[    12}              너0']
frame-motion-type                        : len= 2, val=[  2                  녀0']
frame motion vector horizontal           :pmvlx= 12, val=[                   9    '00110']
fran冶 mo如n ye아아 vertical                 :pmvly= 0, val=[                    0    녀 '1
backward frame motion vector hor         :pmv3x= 0, val=[ -18                '00000101011']
backward frame motion vector ver         :pmv3y= 0, val=[                    2 '0101']

    2]
                                                                  D叫
[
macroblock-address-increment             : len= 1, VLC=[{    1)          '1']
macroblock-type                          : Ien= 5, VLC=[{   30}          '00010']
frame-motion-type                        : len= 2, val=[  1              '01']

                                                                  이H이
dct-type                                 : len= 1, val=[  0
quantizer-scale-code                     : len= 5, val=[     11         '01011']
m애on-vertica나ield                        : Ien= 1, v졔놔    0
field 1 motion vector horizontal         :pmvlx= 9, val= 3 '000111']
field 1 motion vector vertical           : pmvly= 0, \／켸＝ 0 네］
mo如n八／ert七a네eld-s이ect                    : len= 1, val=[  0 '0']
field 2 motion vector horizontal         :pmv2x= 9. val=     20         'OOooloooO'I
field 2 mo的n vec幻r ver키cal               :pmv2y= 0, val= 0                   'l    'I
moti이下vertica卜fielc卞select               : len= 1, val=[  0 '0]
backward field 1 motion vector h         :pmv3x= -18, va느 -30 '000010011']
backward field 1 motion vector v         : pmv3y= 1, v졔＝                  j    네’]
mo如n시ertica卜fiek卞S쉬ect                   : len= 1, v졔놔    0 '0']
backv咀川 field 2 m（光on vec幻rh             :pmv4x= -18, val= -19 '0110]
backward field 2 motion vector v         :pmv4y= 1, val=                2 '0100']
coded-block-pattem                       : len= 5, VLC=[{   44}         '01110']
   runlen아hlamplitude codeword           : len= 4, [{ 2/    -1} '01011]
   runlength'amplitude codeword          : len= 6, [{ 7/     1} '0001000']
   runlength'amplitude codeword          : len= 2, [{ 0/    -1} '111']
end-of寸기ock                              : len= 2, VLC=[{     0}        '10']
   runlengtlt/amplitude codeword         : Ien= 3, [{ 1/     1) '0110']
   runlength/amplitude codeword          : Ien= 7, [{ 8/     1} '00001110']
   runlength'amplitude codeword          : len= 2, [{ 0/    -1}         네］]]
   띠nlength/amplitude codeword           : len= 2, [{ 0/     ]}         녀］0']
en小0卜b幻ck                                : len= 2, VLC=[{    0}         '10']
   runlengtlVamplitude codeword          : Ien= 8, [{ 10/    1}         '001001110']
                                                                                區     .弱


  runlen아r/amplitude codeword       : len= 2, [{   0/    -1}          '111']
end-of缸ock                            len= 2, [{   2/     0}           10']

[   3]
macroblock-address-increment         : len= 1, VLC=[             1}   녀 ']
macroblock-type                      : len= 5, VLC=[            30}   '00010]
vrame-motion-type                    : len= 2, val=[      1 '01]
dct-type                             : len= 1, va느[       0           '0]
quantizer-scale-code                 : len= 5, val=[           12     '01100']
mo的n-ye加졔쥐eld                        : len= 1, v졔＝[-S이ect             0     '0']
field 1 motion vecto                 : pmvl x= 3, val=         14     '000010000']
field 1 mo如n vecto                   : 口mvly= O, va느                  0     '1]
mo的n-vert七a내eld-s毗Ct                 : len=1, V졔＝[        0           '0']
field 2 motion ve아or horizontal      : pmv2x= 20, val=         19     '0110']
field2mot向n vec幻r vertical           : pmv2y= O, va느                  0 네’]
mc川on-vert1ca나回d-s이ect               : len= ], va느［ j 네’]
backward field 1 motion vector h     : pmv3x= -30, val= -32 '0111']
                                                                      0이
backward fi텨d ] mo如n vect아V          : pmv3y= 1, v졔＝                  0    '0110']
motion-vertic졔十eld-s이ect             : len= 1, V싫놔        0
backward field 2 motion vector h     : pmv4x= -19, va느 -19
backward field 2 motion vector v     : pmv4y= 2, val=                 2 '1]
coded-block-pattem                   : len= 8, VLC=[{         58}     '00000100]
   runlength/amplitude codeword      : len= 5, val=[{ 3 /     1}      '001110']
   runlength/amplitude codeword      : len= 6, val=[{ 6 /     1}      '0001010']
end-o卜block                          니en= 2, VLC=[{            0}     녀0']
   wnlength/amplitude codeword       : len= 8, val=[{ 10 / 1}         '0010001110']
   runlength/amplitude codeword      : len= 3, val=[{ 1 / -1}         '0111']
end-of-block                           len= 2, VLC=[{ 0}              '10']
   runlength/amplitude codeword    : len= 4,[{ 2 /         -1} '01
306




엮은0/

      유시룡    1972 년 서울대학교 전자공학과 졸업
             현 대우전자 상무（TV 사업부장）

      장규환    1977 년 서울대학교 전자공학과 졸업
             현 대우전자 이사（영상연구소 담당）

      이병욱    1979 년 서울디獐｝교 전자공학과 졸업
             1981 년 KAIST 전기 및 전자공학과 졸업（석사）
             1991 년 Stai面i1Univers卿（박사）
             현 대우전자 영상현구소 수석연구원

      정해묵    1985 년 서울디獐r교 전자공학과 졸업
             1987 년 서울대학원 전자공학과 졸업（석사）
             1992 년 서울대학원 전자공학과 졸업（박사）
             현 대우전자 영상연구소 선임연구원

      김종락    1988 년 서울디樟f교 전자공학과 졸업
             1990 년 서울대학원 전자공학과 졸업（석사）
             1993 년 서울대학원 전자공학과 박사수료
             현 대우전자 영상연구소 주임연구원

      황덕동    1989 년 연세대학교 전자공학과 졸업
             1993 년 연세대학원 전자공학과 졸업（석사）
             현 대우전자 영상현구소 연구원

      이민섭    1989 년 서강대학교 전자공학과 졸업
             1991 년 KAIST 전기및 전자공학과 졸업（석사）
             현 대우전자 영상연구소 주임연구원

      김진헌    1992 년 한국과학 기술디掛 전자공학과 졸업
             1994 넌 서울대학원 전자공학과 졸업（석사）
             현 대우전자 영상연구소 연구원

      임종타1   1989 년 서울대학교 전자공학과 졸업
             1991 년 서울대학원 전자공학콰 졸업（석사）
             현 대우전자 영샹연구소 주임연구원

      김종일    1988 년 연세대학교 전자공학과 졸업
             19卯 년 연세대학원 전자공학과 졸업（석사）
             현 대우전자 영상연구소 주임연구원
        연암츈판사의 '연암셈岳71획'은 올바른 셈簧문화의 정립과 발전에 밑7俉0I 되'1 위하여
                   늘 신선한 기획, 충만한 내용, 세밀한 편집으로
                 독자 여러분을 찾아갑니Cl. 연암을 지켜봐 주십시오．


      라 PC 2"                                이제 컴맹이 아니Ct,
                                                                            1


     훈 저／ 750쪽／ 10. 000원                     꿜 조형진／ 전2권 860쪽／ 15, 000원 （초보를 위한 필수 디스켓 제공）


  컴퓨터를 배우고 싶으십니까？ 이 책 한 권이면 학원에          PC 초보자 6백여 명의 요구 사항을 조사 · 분석해 기획된 이
다닐 필요가 없습니다. 이미 수많은 아버지들, 어머니들，                    책을 '수박 겉 핥기'식의 얇은 입문서와 비교
           학생들이 이 책으로 쉽고도 재미있게 컴                   하지 마십시오 초보자인 당신은 이 책으로
           퓨터를 배웠습니다. PC 초보자를 '컴퓨                  초보를 탈출할 수 있을 뿐만 아니라 초보의
           터 도사'로 만드는 책 . 초보자가 꼭 알아                단계를 벗어났을 즈음에서 각종 시스템 사용
           야 가장 다양한 내용, 가장 최신 바전의                  에 욕심을 부리게 되어도 아무 탈 없도록 옆
           프로그램과 사용법을 소설보다 재미있                     에서 코우치를 알뜰히 해 드릴 것입니다. 쉽
           게 , 그 어떤 책보다 알기 쉽게 설명하고      고도 내용이 꽉 찬 입문서 e 바로 여기 있습니다. .PC는 무엇
있습니다. 뿐만 아니라 독자들의 이해를 돕기 위해1 필요하        이며 PC로 무얼 하나9 0하드웨어 , 소프트웨어의 원리와 구조
다고 생각된 부분에는 상세한 그림을 곁들여 설명했습니           I도스 6.2의 사용법과 메모리 관리 I워드프로세서 （한글） S
다. S컴퓨터의 구조 및 사용법 .도스의 기초（DOS 6.0,      NC보다 뛰어난 한국형 파일 관리 프로그램 MDIR皿 I화려
6.2) S프로그램 설치법 I마우스와 노턴 코맨더 사용법         한 연인 윈도우즈 IPC 통신의 세계（하이텔, 천리안） I노턴
I아래 한글 2.11 활용법 S메모리 관리와 노턴 유틸리티        유틸리티 I압축1해제 방법과 바이러스 퇴치법 1 PC의 고장
I압축 및 디스크 뻥튀기 유틸리티 I바이러스의 예방과           시 응급 조치법 I초보자를 겁에 질리게 만드는 컴퓨터 고장，
치료 I컴퓨터 통신（이야기） I윈도우즈와 멀티미디어            그 수리 비법 !



      엽의 페모리 관리"
       天｛/ 69］쪽／ ]2. 000원                      외 공저／ 632쪽／ 12, 000원



 386을 386답게 , 486을 486답게 쓰려면 메모리 관리 문     당신의 컴퓨터를 노래방으로, 신디사이저로 , 오케스트라
제를 정복해야 합니다. 메모리 관리를 할 수 없다면 '초보        로 만들 수 있습니다. 초보자를 위한 PC 음악의 모든 것을
자 딱지 ' 를 결코 떼지 못 합니다. 이 책 한 권이면 메모리                 다룬 책 . PC가 있으면서도 음악 이론을
            관리는 쉽게 해결됩니다. 노력하는 저자                   잘 모르는 분, 또 음악 카드로 노래방 활
            송세엽은 독자들을 위해 좋은 책 , 꼭 필                 용밖에 못하는 분들을 위한 컴퓨터 음악
            요한 책을 펴내기 위해1 오늘도 끊임없이                  입문서입니다. 'PC 음악과 음악 이론
            노력하고 있으며 , 그 결실의 하나로 이                  의 기초 I애드립 카드와 비주얼 컴포저
            책에선 독자 여러분의 요청에 부응, 윈도                  사용법 I옥소리와 응용 프로그램（옥피
            우즈의 메모리 관리 및 최적화 방법을 새      리 , 가요방 등） S사운드블래스터의 모든 것 S미디의 이
롭게 추가하는 등 그 광역을 넓혀가고 있습니다．              해와 응용의 실제
               은 올바른 셈틀문화익 정립과 발전에 밑거름이 되가 위하여 늘 선선한 기획， 중만한 내용， 세밀한 핀집으로 독자 여력분을 찾아갑니1
                                                                                                   1
；연암셈틀기획，
           커들의 해킹 기UI,,
                   너                                   라 한글 2.1+2.5"
           j스4 외 공저／ 496쪽／ 10. 000원                    외 공저／ 615쪽／ 10.000원 (.醍서식', '타차 프로그럽' 디스켓 끼공）

           영국 해커 침입！ 이것으로 끝나지 않습니다. 순             '한글'로 막대 그래프나 꺾은선 그래프를 그려 본 적이 9
           망치한（脣亡齒寒）이란 고사를 생각해 볼 때 , 입
           술을 무너뜨린 그들은 이제 곧 이빨을 무너뜨리             는가9 이 책에는 '한글'로 불가능하다고 생각됐던 많은 I
           기 위해 다가올 것입니다. 유선상의 외세 침공／                       들이 담겨 있다. 이 책은 '한글' 설명서드
           그것을 막기 위한 길은 우리도 해킹 방법을 연                        내용만으로는 어려워서 잘 활용을 못 돋
           구해 해커가 되는 길뿐입니다. 시스템 해킹 및                        는 초보자들, '한글'을 더 완벽히 사용i
           락 해제와 파일 에디트 등에 관한한 국내의 일
                                                            고자 하는 기왕의 사용자들을 위해 쓰＜
           인자를 자처하는 대표적 해커들의 해킹 기법．
0파일과 디스크 에디트를 위한 PC-TOOLS, NDE, DEBUG 완                     졌다. '한글'의 기초는 물론이고 도표 2
벽 해설 I락을 풀기 위한 이론과 실제, UNPROTECT의 예제 다                      성 , 그림 , 수식 , 책 만들기 등 다양한 I
수 포함 I게임 섹터 에디트 4 내 마음대로 게임 조작하기1 1 '트로          크닉과 팁을 이용한 고급 사용법을 쉽게 배울 수 있도록 1
이의 목마'를 이용한 '호롱불' 해킹에서 UNIX, INTERNET까지
                                                 들었다．
I해커의 윤리와 해킹 사례



            자 ANSI"                                      라이브러리의 모든 것"
           호 저／ 312쪽／ 8. 500원 （몌斗 디스켓 포함）             재 저／ 667쪽／ 15. 000원 （몌川 디스켓 포합）

           단지 몇 개의 ANSI 코드만 갖고도 통                 C 언어용 한글 라이브러리의 삼총사라 할 수 있는 '허
          신을 이용해1 애인에게 장미꽃을 보낼 수                           미 한글 라이브러리 ' , '한글 라이브러
          도 있고, 친구에게 생일 축하 카드를 보                           프로' , '한글 라이브러리 （한）'을 중심
          낼 수도 있다. 문자 위주의 통신 환경이                           로 컴퓨터에서의 한글 구현 문제를 실
          무지개보다 아름다운 색의 환경으로 바                             위주로 기술한 역작. 유용하게 쓸 수
          뀐다. 또한 자신의 BBS를 화려한 로고                           는 각종 테크닉과 예제들이 다수 실려
와 메뉴로 장식할 수도 있다. 'DOS & 이야기 ANSI 코                         다. Ii부 한글 라이브러리 기초 '2
드 완벽 해설 I통신 동호회와 BBS의 로고 제작 기법 .                 라이브러리 활용 예제 .3부 마우스 커서 , 내장 아이콘，
게시판과 채팅실에서의 ANSI.이야기 ANSI를 이용한                   자형 등록 및 예제 응용 루틴 .4부 라이브러리 함수 I
그래픽                                              로．
             엽 도스"                                          과디럭스 패인트"
            엽 저／ 912쪽／ 16. 000원                              공저／ 468쪽／ 8. 000원

  PC의 작동은 도스가 한다. 디스켓을 포맷하고 , 파일을                 '디럭스 페인트'는 문자 그대로 페인팅 프로그램이다. 亐
복사하고, 옮기고 , 없애고 , 지워진 파일 다시 살리는 법들               순히 페인팅 흉내내기가 아닌 실제로 예술가가 붓과 팔코
에서부터 하드디스크를 두 배로 쓰는 법까지 . A/S 신고의                          트를 가지고 물감을 섞어가며 작품을 2
50%는 도스를 잘 몰라서이다. 이 책은 원래 '초보자용'과                          작하는 것과 같은 효과를 얻게 해준디
             '중급자용' 두 권으로 출간하려 했으나                         이 책의 특징은 동종 책들의 메뉴 설므
             저자 특유의 친절한 설명이면 이내 누구                         방식을 탈피하고, 메뉴 구성과 사용 설1{
             나 중급자가 돼버린다는 이유 때문에 합                         을 실례를 들어 설명함으로써 학습자으
             권으로 묶은 것이다. 이 책은 도스와 메                        자연스러운 창작 행위를 유도한다. 개으
             모리 관리에 관한 한 국니：1 최고의 책이라            용 컴퓨터의 중요한 활용 분야로 부상한 ' 컴퓨터 그래픽 ' 히
             할 수 있다. 저자는 현재 공인회계사로서              평소 관심을 가졌던 일반인들과 미술 학도들에게 많은 3
국내 회계 업무의 전산화에 공헌하고 있으며 , HiTEL 내                움이 되리라 확신한다. I컴퓨터 그래픽의 개요 I컴퓨t
'OS 동우회' 의 시삽으로 '도스란'을 맡아 강좌하고 있다．               그래픽의 분야와 활용 12차원 그래픽의 소개 I디럭스 피
P（그 유력지 'PC-Lil寸E'은 그를 '컴퓨터 시대를 여는 전문            인트의 분석과 응용 I윈도우용 그래픽 프로그램의 소개호
인' 으로 선정한 바 있다．                                  활용 I다양한 그래픽 장비 소개
“연암셈틀기획’은 올바른 셈틀문화의 정립과 발전에 밑거름이 되기 위하여 늘 산선한 기획 , 충만한 내용 , 세밀한 핀집으로 독자 여력분을 찾아갑니다．




         엽의 필수 유틜리El 대활8"                             와함月하는게임 만들기"
     엽 저／ 550쪽／ 12. 000원 （유므리티 프로그百 디스켓 포함）        드4 저／ 642쪽／ 13. 000원 （예川 디스켓포합）

 누구나 쉽게 구할 수 있어서 대개는 몇 개씩 가지고 있는               이 책은 업소용으로 대단히 인기를 누렸던 'SF-2'를
유틸리티 , 하지만 제대로 쓰질 못해서 손도 못댄 채 자신의             PC용으로 개조하는 데 성공한 저자가 그 제작 과정을 처
    八十
           컴퓨티 공간만을 차지하고 있다면, 겉치
         어녀 티1 :
         여口 리1 회크
                                              음부터 조목조목 설명하면서 쓴 것으로 기존에 나와 있는
          장만 요란한 멍텅구리에 지나지 않습니
    띠a
         세n 타a 대
         八古 0n                                게임에 관한 매뉴얼이나 팁 정도를 소개한 책들과는 비교
          다. 이 책으로 마음껏 활용해 보십시오．                        가 되지 않는다. 게임을 만들어 보려고
          꼭 필요한 최신 버전의 유틸리티들만올                          하신 분이면 누구나 느끼는 게 국내엔 게
           모았습니다. 이 책에 수록된 다양한 유틸                       임 제작을 위해 참고할 만한 책이 거의
          리티들이 여러분의 컴퓨터 환경을 개선，                         없다는 것이다. 저자가 그러한 독자들의
증진시켜 주고 독자 여러분의 컴퓨터 실력을 더욱 향상시                          심중을 혜아려 쓰게 된 이 책은 독자들이
켜 줄 것입니다．                                               게임 제작을 함에 있어서 꼭 알아야 할
                                              내용을 실무자의 차원에서 상술함으로써 저자가 들여야 했
                                              던 시간과 고충을 절감시켜 드리고저 했다．

     이크웍 프로 2.00"
     훙 저／/ 355쪽／ 10. 000원 （예제 디스켓 포합）                  있는게임 만들기"
                                                       / 232쪽／ 8.000원
  윈도우즈용 케이크웍은 키존의 미디 프로그램들이 가지 !
고 있는 특성들을 고루 갖추고 있는 프로그램으로 윈도우                 게임 제작 , 초보라고요2 미리 겁먹지 마십시오. '완전 초
             즈의 특성인 다양한 화면 구성과 기능，            보'도 게임을 제작할 수 있는 길이 열렸습니다. 왜냐면 중
             손쉬운 표현 방식으로 누구나 쉽게 컴퓨            학교 2학년인 저자가 쓴 이 책은 베이식까지는 아는데 , 게
             터 음악의 진수를 느낄 수 있게 해드립니           임 제작 하면 도망가는 r완전 초보J , 베이식도 알고 게임도
             다. 이는 P（二 음악용 소프트웨어 패키지                     어느 정도 다루고 이해하지만 게임 제작
             가운데 가장 널리 사용되고 있는 프로그                       하면 힘들어 하는 F초보J , 그리고 국산
             램이며 . 성능 또한 여타의 추종을 불허합                     스트리트 파이터 개조법과 좀더 나은 게
니다. 특별한 장비나 입력 도구를 필요로 하는 것도 아니                          임 제작 기법을 알려고 하는 F가짜 초보J
며 , 일반 386DX 이상의 시스템과 미디 인터페이스와 미                        가 대상이니까요. 필자의 발자국만 좇으
디 케이블, 미디 악기 및 마스터 키보드만 있으면 누구나                          면 누구나 게임을 만들 수 있게 될 것입
사용할 수 있습니다．                                   니다. 자, 게임 제작의 세계로 들어오십시오．




           튜디오 R3"                                   배우는 UNIX와 C"
     스1 저／ 789쪽／ 20. 000원                          므J 天｛/ 480쪽／ ]0.000원

 '3D 스튜디오'는 386DX 이상의 시스템과 코프로세서，              컴퓨터 환경은 점차적으로 기존의 호스트 중심과 수직형
8MB 이상의 메모리만 있으면 누구나 돌릴 수 있는 대중적                        전산구조 , 메인 프레임 중심의 하드웨어
인 그래픽 프로그램으로 그 성능면에선 웍스테이션에 견줄                          둥에서 탈피하여 클라이언트 서버 중심
           만하다. 이 책은 저자가 컴퓨터 그래픽                        의 수평구조 아래 웍스테이션. PC 둥의
           디자이너로 일하며 , 평소 '31) 스튜디오'                    하드웨어 차원으로 변하고 있기 때문에
           를 사용하면서 느낀 많은 문제점과 기존                        UNIX. X-WINDOW. C 언어 등의 애
           설명서들의 미홉한 점 , 보충할 점들을 충                      플리케이션이 더욱 비중있게 평가되고
           분히 감안하여 썼기 때문에 차근차근 따              있다. 이에 많은 컴퓨터 전문가들은 UNIX가 미래의 표준
           라만 하면 누구나 '3') 스튜디오' 의 사용          운영체제가 될 것이라고 하나같이 말하고 있다. 그 운영체
법을 익히고 응용할 수 있을 것이다．                          제를 초보자도 능히 익힐 수 있도록 쉽게 설명하고 있다．
     ‘연암셈틀가획’은 올바른 셈틀문화의 정립과 발전에 밑가름이 되가 위하여 늘 신선한 기획 , 충만한 내융 , 세밀한 편집으로 독자 여력분을 찾아갑니




           립 , PC수리 , PC업그레이드"
         I연구모임 저／ 775쪽／ 15,000원 （보너스 디스갓 포甘）            저／ 537쪽／ 10.000원

  이 책은 초보자에서 중급자에 이르기까지 모든 PC 활용                  한글워드는 현재 최고의 워드프로세서임과 동시에 7｝즈
자들이 PC를 조립하거나 활용 중에 겪는 간단한 에러나                  미래가 밝은 워드프로세서임을 어떤 전문가도 부인할 수
             고장을 처치하고자 할 때 또는 시스템을              없을 것입니다. 처음 워드프로세서를 대하는 사람들은 우
             업그레이드할 때 흔히 겪는 곤란을 쉽게              드프로세서로 무엇을 할 수 있는지 잘 모르기 때문에 겉上
             해결할 수 있도록 그 방면의 지식과 정보             기 몇 가지 기능으로 판단하려 합니다. 한글워드는 첫눈O
             를 풍부히 제공합니다. 제명에서 알 수                        반할 만한 깔끔하고 훌륭可외양은 물론1
             있듯 비단 조립 뿐만 아니라 조립에 앞서                       익히면 익힐수록 놀라운 기능들을 7｝겨
             좋은 부품의 구입과 조립 후의 자가 진단                       고 있는 워드프로세서입니다· 한글워셔
및 사고 조치 요령 , 그리고 자신의 PC를 멀티미디어 PC                         를 충분히 활용할 수 았는 단계에 이르쩍
로 개조하는 방법 둥을 친절하고도 상세하게 담고 있습니                            다른 워드프로세서와한글워드가 어떻기
다. . 제1부 rpC 조립"fi- 컴퓨터의 부품에 대한 기본 지                      다른지 실감케 될 것이며 , 스스로 한글켜
식과 최상의 시스템을 구축하는 방법과 조립 후 점검 사항                 드를 선택한 것에 대한 안도감을 느끼게 될 것입니다. 미
0 제2부 r고장 진단과 수리J 부팅과 작동 과정상의 고장                제1부 r워드다운 워드프로세싱J - 처음 시작하는 분들0
에 대한 진단 및 수리 절차 . 제3부 r업그레이드J 1 지금              워드답게 워드를 사용할 수 있도록 워드의 기본적인 7］남
사용하고 있는 PC를 자신이 사용하는 용도에 가장 적합하                 들을 설명합니다. 0 제2부 r생각하는 워드프로세싱J . 1
게 스스로 업그레이드할 수 있는 방법 및 절차 . 제4부                 준 높은 워드프로세싱을 위한 편집디자인의 기본 개념들놔
r컴퓨터 부품 정보J- IBM PC의 기본적인 지식과 용어                문서를 이루는 각 부분을 워드에서 구현하는 방법을 실才
풀이를 필두로 각종 부품 정보에 대한 상세 설명 0r부록                 예를 통해 설명합니다. I 제3부 r효율적인 워드프로세싱1
편J- (l) 보너스 디스켓 안에 들어 있는 진단 프로그램인               - 작업 능률의 극대화를 위한 워드의 자동화 기능올 설d
QAPlus, Snooper,"· 등의 설치 방법과 사용법 @ 제조           합니다. 워드의 가장 차별적인 기능인 필드와 워드 베이4
회사별 하드디스크 사양 및 점퍼 조정법 區）서울 지역과 지                의 응용에 대해서도깊이 있게 설명합니다.           1
방 대도시의 컴퓨터 관련 상가 주소록




          중 저／ 706쪽／ 15, 000원 （소스 디스켓 포합）


 이 책은 기존의 C로 프로그래밍한 사람이 \uisual
C+＋로 윈도우즈 어플리케이션을 만드는 경우 C와
C+＋의 차이 , 도스 프로그래밍과 윈도우즈 프로그래밍의
             차이 , C로 윈도우즈 프로그램을 작성하
             는 것과 \Tisual C +＋로 윈도우즈 프로
             그램을 작성하는 차이에 대해1 쉽게 이해
             할 수 있도록 각각을 비교 설명합니다．
             C와 SDK로 만든 프로그램이 \Tisual
             C+＋의 환경에서는 어떻게 만들어지는
가를 초보자를 위해 단계별 , 도식적으로 쉽게 설명하고 있
습니다. 뭐니뭐니 해도 Visual C+＋를 잘 이용하는 가장
빠른 길은 제공되는 툴（AppWizard. Class Wizard,
App Studio 등）보다 MFC의 계층 구조（Hierarhy）에
있는 클래스의 기능들을 얼마 만큼 파악하느냐에 달려 있
다．
