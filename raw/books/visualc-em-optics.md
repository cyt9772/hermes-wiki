---
source_url: /run/media/yutae/Data/visualc_정전기학_기하광학.pdf
ingested: 2026-10-22
sha256: 82d49f306fe0cc98925aee5cb3064f2f2cf96a9ed1e32b7abe0a8888d986c7fe
---

# C++ 6.0 으로 구현하는 정전기학·기하광학 (raw source)
> Text-layer PDF (poppler pdftotext -layout), Korean + C++ code, 336p, 2001.

## Book metadata
- title: C++ 6.0 으로 구현하는 정전기학·기하광학
- author: 최행진 (Choi Haeng-jin)
- publisher: 내하출판사 (Nae-ha Publishing), 발행인 모흥숙
- first edition: 2001-11-10
- ISBN: 89-88932-25-0
- price: 13,000원
- pages: 336
- note: "이 책은 필자의 두 번째 저서인 'Visual C++ 6.0으로 구현하는 기초적 물리현상 시뮬레이션'의 연장선상에 있는 책이다. 이 책은 전자기학의 한 분야인 **정전기학 (electrostatics)**과 광학의 한 분야인 **기하광학 (geometrical optics)**을 대상으로 한다." (저자서문)

## Chapter structure (from TOC)
| # | topic (이론 + Source Code + 실행결과) |
|---|------|
| 0 | MFC (Microsoft Foundation Classes) — 개론, 준비과정, Source Code |
| 1 | 전자기학 (Electromagnetism)의 기본 — 정전기학, 정자기학, Helmholtz 정리, 마당의 분류 (1~4종) |
| 2 | 등전위선 (Equipotential Line)과 전기마당의 역선 — 점전하, 쌍전하, 구면전하, 쌍극자, 사중극자, 도체구, 유전체구 |
| 3 | 전기다중극 (Electric Multipole) — 스칼라 퍼텐셜의 다중극 전개, 극/쌍극/사중극 |
| 4 | 영상법 (Method of Image) — 점전하+접지평면, 도체구, 유전체 |
| 5 | 변수분리법 (Separation of Variables) — 균일전기장 내 도체구/유전체구 |
| 6 | 전기마당의 역선 (재현, 쌍극자 마당) |
| 7 | 빛의 반사와 거울 (Mirror) — 볼록거울, 오목거울 |
| 8 | 빛의 굴절 (Refraction)과 렌즈 (Lens) — 오목렌즈, 볼록렌즈 |
| 9 | 3차원 입체의 구현 — 투영, 방위각 |
| 10 | 입체의 확대와 축소 |
| 11 | 입체의 회전 |
| 12 | 입체의 숨은선과 숨은면 |
| 13 | 이변수함수의 그림 — I/II |

## Extracted text (poppler pdftotext -layout)

C++ 6.0 으로 구현하는
＼入／
  ＼사＼入／.naeha.co.kr
nme ！口正 보기（r 도8mm
口斗U         1 t               쁨S骨     碧；




그림 1 단일 점전하佃46)               그림 2 단일 양전하와 단일 음전하伯54)



  닌已J 7면 月히＝ Y 月목1H U
n亡（E) !m日 브긔（r 도미             n1   mn 뵤가凹 드am
口畔U           1 t                    1 甘1 1

                                                 시 간＝15n미片nn主




叫



그림 5 균일한 구면 전하분포佃79)      '   그림 6 쌍극자마당（p92)



川t ham U가凹 Lu,며）                7 a1i1 브긔t出 us
Os므    r 1가 a ',              D 吃口나 工 因m r

                                                 川간d1土1711H主




川


그림 9 점전하와 접지된 도체구（口］23)       그림 ]0 점전하와 반무한평면 유전체 (키33)
l出띠 1口띠 뵤기凹 드11nn                        i1m 므＝七 보기侄 도目甲바
 Os 日    r 1 !                            D 낱日      凸 t

                       시 간d此1111m主                          그 r9? 5?n0n0 }




                                     \
                                                            / /



그림 3 두개의 양전하와 단일 음전하（p61)                그림 4 두개의 양전하와 두개의 음전하（p69)



1}1（日 ！三（目 ！거m 도11an
口 j 日       P 1 1

                       시 간11dJmmHi




                                         !a                                  m




그림 7 사중극자마당佃104)                         그림 8 점전하와 접지된 반무한평면 도체（p114)



n1띠 nmn ！가M 드11뗘｝                        口1e 11田 보月凹 도1m
0 呼口 「 也 e, ee                           Os口 { 每武1 !

                       시칸m117nn主




그림 ]] 균일한 전기마당 내의 접지된 도체구                그림 ]2 균일한 전기마당 내의 유전체구（p153)
      作)145)
저자서
學 餐 磁 鞋 湃 肆 離 難 聲 雄 雛 鞋




        이 책은 필자의 두 번째 저서인 "피sual C++ 6.0으로 구현하는 기초적 물리현상 시뮬레이
      션" 의 연장선상에 있는 책이라고 할 수 있다. "Visual C++ 6.0으로 구현하는 기초적 물리현
      상 시뮬레이션" 의 주된 내용은 수치해석（numerical analysis）을 이용하여 역학 현상을 시늉
      내기（S油ulation) 하는 것이었다. 이 책은 전자기학佃lectromagnetism) 의 한 분야인 정전기
      학（electrostatics）과 광학（optics）의 한 분야인 기하광학（geom아rical optics）을 대상으로
      한다．
        필자는 올해 3월달에 필자의 첫 번째 저서 "뀌sual C++ 6.0으로 구현하는 수치해석 "을 출
      간하였고, 5월달에 두 번째 저서 "Visual C++ 6.0으로 구현하는 기초적 물리현상 시뮬레이
      션”을 출간하였다. 2권의 책 출간 이후에, 몇몇 독자는 필자의 책에 대해 비판을 했다. 칭찬을
      한 독자도 있었고 쓴 소리를 한 독자도 있었다．
        그런데 쓴 소리를 한 독자들의 비판 내용은 대동소이했다. 그 내용은 프로그램의 대부분이
      보통의 C 언어로도 실행이 된다는 것이었다. 좀 더 구체적으로 말한다면, C 언어에는 없던 클
      래스 같은 것들을 사용하지 않았다는 것에 대해 불만이 있었던 것이다. 클래스를 사용하지 않
      았다는 비판은 맞는 말이다. 필자는 기본적으로 클래스를 만들어 사용하지 않았다. 하지만 대
      부분의 프로그램이 C 언어로 실행이 된다는 비판은 틀린 말이다. 필자는 MFC를 자주 사용하
      였는데 MFC를 사용한 프로그램은 절대로 C 언어에서 실행되지 않는다. 그 뿐 아니라 다른
      C+＋에서도 실행되지 않는다.
        필자에게 쓴 소리를 한 독자들은 필자의 저술 방향을 모르는 것 같다. 필자는 앞서 2권의
      책의 저자서문에서도 분명하게 저술 방향을 밝혔는데, 필자의 저술 방향은 어떻게 하면 쉽게
      수학이나 물리학을 프로그래밍 언어와 통합하느냐이다. 어려운 code를 사용하여 수학과 물리
      학을 구현하는 것이 아니다. 이 책의 저술 방향도 큰 차이는 없다. 다만 책 내용의 대상이 다
      를 뿐이다．
        요즘 대한수학회나 한국물리학회에서 외국의 전문 수학 용어나 물리학 용어에 대해 우리
      문화에 맞는 전문용어를 만들고 있다. 물론 그러한 작업의 목적은 사람들이 그러한 용어들을
      쓰는 것이다. 필자가 보기에 아직은 많은 사람들에게 영향을 미치지 못하고 있는 것 같은데，
      필자는 개인적으로 많은 과학도들이 우리 용어를 사용하려고 노력하기를 바란다. 얼마 전부터
iv 저자서문



   필자는 대한수학회나 한국물리학회에서 만든 우리 용어가 있으면 항상 그 용어를 쓰려고 노
   력하기 시작했고, 앞으로도 계속 그러려고 한다. 이 책을 포함하여 앞으로 출간될 필자의 저서
   에 쓰일 용어도 우선은 우리 용어를 사용할 것이다．
     많은 사람들이 우리 용어에 대하여 부정적인 시각을 가지고 있다. 어디까지나 필자 생각이
   긴 하지만, 0％라고 말할 수 있을 정도로 우리 나라에서 나온 과학 이론은 없다. 모든 전문용
   어에 대응하는 우리 용어를 만들기도 현실적으로 불가능할 것이다. 뜻 전달이 잘 되지 않거나
   좀 어색한 경우도 많다. 하지만 그렇다고 해서 계속 외국 용어만을 고집한다면 우리 나라는
   평생 외국의 뒤만 쫓게 될 것이다．
     노파심에서 말하는데, 이 책에 프로그래밍의 고급 기술 같은 것은 없다. 필자는 어떻게 하면
   어려운 과학의 분야를 컴퓨터를 사용하여 조금이라도 더 쉽게 구현할 수 있을 것인지를 항상
   고민한다. 이것은 수학과 물리학의 대중화를 꿈꾸는 필자의 수단이다. 컴퓨터를 통하여 많은
   사람들이 수학과 물리학에 좀 더 가까이 다가설 수 있기를 희망한다．
     책을 보다가 개선해야 할 점을 발견하거나 그 외 좋은 의견이 있으면 필자에게 알려주킬 바
   란다. 필자의 전자우편 주소는 kchongup（亘）dreamwiz.com이다．



                                                 저자 최행진
차려I
難 學 枷 轟 쪼 啼 簪 聽 黎 雄 彎 轟 蠱 學 學 儺 難 鞋 露 轟 難 勘 學 難 難 蜘 蜘
                                                      發 難 好 斗 a     卄 a   卞 a   .   小 4   斗 a   朴 a   斗 a   s   +   仁 儺 好 心 鴦




    0장 MFC（씨crosoft Foundation 이asse引                      1

         0. ] 개론     ]
         0.2 MFC      2
              0.2. ] 준비 과정 2
              0.2.2 Source Code     20




d：부 정전71학（Electrostatics)                           25

    1장 전자기학（Electromagnetism）의 기본0雇                            27

          ] . ] 정전기학（Electrostatics)       27
          ] .2 정자기핵Magnetostatics)          27
          1 .3 헬름홀쯔 정리（He帥h이仁 Theorem)                28
          1.4 마당의 분류 29
              1.4.1 제］종 마당 29
              1.4.2 제2종 마당 30
              1.4.3 제3종 마당 30
              1.4.4 제4종 마당 31

     2장 등전위선（Equipotential Line）과 전기마당의 역선                                33

          2.1 이론      33
          2.2 단일 점전하 38
              2.2.1 이론 38
              2.2.2 Source Code 40
              223 프로그램 실행 결과 46
   2.3 단일 양전하와 단일 음전하                  46
      2.3.1 이론     46
      2.3.2 Source Code 48
      233 프로그램 실행 결과 54
   2.4 두개의 양전하와 단일 음전하                  54
      2.4. ] 이론    54
      2.4.2 Source Code      55
      2.4.3 프로그램 실행 결과            61
   2.5 두개의 양전하와 두개의 음전하                     62
      2.5.1 이론     62
      2.5.2 Source Code
                      63
      2.5.3 프로그램 실행 결과 69
   2.6 균일한 구면 전하분포（Uniform Spherica' Charge 미stribution)   69
      2.6.1 이론     69
      2.6.2 Source Code 73
      2.6.3 프로그램 실행 결과 79


3장 전기다중극（Electric M미tipole)                  81

   3. ] 스칼라퍼텐셜의 여러겹극 전개                     81
   3.2 홀극    83
      3.2. ] 이론    83
   3.3 쌍극자마당（D巾이e 디이d)                 83
      3.3. ] 이론    83
      3.3.2 Source Code      86
      3.3.3 프로그램 실행 결과            92
   3.4 사중극자마당           92
      3.4.1 이론     92
      3.4.2 Source Code 98
      3.4.3 프로그램 실행 결과 ]04

4장 영상법（Method of Image)                105

   4. ] 개론   105
   4.2 점전하와 접지된 반무한평면 도체                         ]06
      4.2.1 이론     106
      4.2.2 Source Code
                      109
      4.2.3 프로그램 실행 결과 114
   4.3 점전하와 접지된 도체구                    ] 14
      4.3. ] 이론     ] 14
      4.3.2 Source Code          117
      4.3.3 프로그램 실행 결과             ] 23
   4.4 점전하와 반무한평면 유전체                         ] 23
      4.4. ] 이론     ] 23
      4.4.2 Source Code
                      127
      4.4.3 프로그램 실행 결과 ]33


5장 변수분리법（Separation of Variable引                        135

   5. ] 이론   ] 35
   5.2 균일한 전기마당 내의 접지된 도체구                            ]37
      5.2. ] 이론     137
      5.2.2 Source Code          140
      5.2.3 프로그램 실행 결과             ]45
   5.3 균일한 전기마당 내의 유전체구                         146
      5.3.1 이론      146
      5.3.2 Source Code          147
      533 프로그램 실행 결과               153

6장 전기마당의 역선                155

   6.1 이론    155
   6.2 단일 점전하         ] 56
   6.3 쌍극자 전기마당             156
      6.3.1 이론      156
      6.3.2 Source Code          157
      6.3.3 프로그램 실행 결과             162
   6.4 선형사중극자          162
      6.4. ] 이론     ]62
      6.4.2 Source Code 163
      6.4.3 프로그램 실행 결과 ]68
       기하광학（Geometrical Optics)                         169

     7장 빛의 반사와 거울（Mirror)               171

        7.1 이론    171
        7.2 볼록거울（Convex Mirror)          172
           7.2. ] 이론     ] 72
           7.2.2 Source Code      174
           7.2.3 프로그램 실행 결과           ]82
        7.3 오목거울（Concave Mirror)            ]83
           7.3. ] 이론     ]83
           7.3.2 Source Code      184
           7.3.3 프로그램 실행 결과           ]92

     8장 빛의 굴절（Refraction）과 렌즈（Lens)               193

        8. ] 이론   ] 93
        8.2 오목렌즈        194
           8.2.1 이론      ] 94
           8.2.2 Source Code      195
           8.2.3 프로그램 실행 결과           203
        8.3 볼록렌즈         203
           8.3.1 이론      203
           8.3.2 Source Code 204
           8.3.3 프로그램 실행 결과 212




       기초적인 3차원 컴퓨터 그래픽                            2化
（呼
     9장 3차원 입체의 구현              2佰

        9.1 개론    215
        9.2 이론    217
        9.3 Source Code         220
        9.4 프로그램 실행 결과            225
10장 입체의 확대와 축소             227

  10. ] 이론   227
  10.2 Source Code       228
     10.2. ] 입체의 확대와 축소피ew.h                228
     10.2.2 입체의 확대와 축소Vie넥.cpp                   230
  10.3 프로그램 실행 결과              237
     10.3.1 日key를 다섯 번, 圄key를 일곱 번 누른 경우                237
     10.3.2 띠key를 네 번, 圖key률 여덟 번 누른 경우                237
     10.3.3 日key를 네 번, 띠key를 여섯 번, 圄key를 세 번 누른 경우            238

11장 입체의 회전         239

  ] 1.1 이론   239
  11.2 Source Code       240
     11.2. ] 입체의 회전View.h            240
     11.2.2 입체의 회전View.cpp            242
  11.3 프로그램 실행 결과              249
     11.3.1 日 key를 누른 경우             249
     11.3.2 띠 key를 누른 경우             250
     11.3.3 圈 key를 누른 경우             252


12장 입체의 숨온선과 숨온면 제71                       255

  12.1 개론    255
  12.2 정육면체        255
     12.2.1 이론     255
     12.2.2 Source Code 256
     1223 프로그램 실행 결과 262
  12.3 지구본    262
     12.3. ] 이론    262
     12.3.2 Source Code 264
     12.3.3 프로그램 실행 결과 269

13장 이변수함수의 그리匹                 271

  13.1 개론    271
  13.2 이변수함수 I           271
x   차례



            13.2.1 이론    271
            13.2.2 Source Code 272
            13.2.3 프로그램 실행 결과 278
          13.3 이변수함수 ii        278
             13.3.1 이론   278
             13.3.2 SourceCode 279
             13.3.3 프로그램 실행 결과 283


     부록    285

          부록 A 대한수학회 제공 수학 용어집       287

          부록 B 한국물리학회 공식 물리학 용어집       309
A0,，眠(Mi.r姓F에曲11*
              씨asses),
0.1. 개론

 MFC (Microsoft Foundation Class Library）는 읜도우즈용 프로그램 개발을 보다 쉽게 하도록
도와준다. MFC에 대해 알기 위해서는 그 전에 먼저 API (Application Programming Interface)
에 대해 알아야 한다．
 API는 Application Program Interface의 頭文字語（acronym)로서 , 응용 프로그램이 컴퓨터의
운영 체제에 의해 수행되는 lower-level services를 요청하고 수행하기 위해 사용하는 명령어들
의 집합이다.
 MFC는 객체 지향 프로그래밍 기술의 적용과 cO(扼의 재사용을 위해서 윈도우즈 프로그래밍을
위한 API인 "硼n32 API"를 기능별로 구분해서 클래스로 작성해 놓은 것이다. MFC는 윈도우즈
운영 체제에서의 프로그래밍을 위한 "application fran祀work '이다. MFC는 \windows, 메뉴, 대화
상자에 필요한 code의 많은 부분을 제공한다. 독자는 fran祀work 안에 원하는 code를 더하면 된
다. MFC를 사용하면 개발 시간（dev이op毗nt time）을 줄일 수 있고, code를 다른 기종에 이식
하는 데 어려움을 줄이고, Windows Sockets을 통한 network 프로그래밍을 단순화시킨다．
 이 책에서 API와 MFC에 대해 자세하게 설명하는 것은 이 책의 범위를 벗어나는 일이므로 이
것들에 대한 구체적인 설명은 생략한다. 자세한 것이 궁금한 독자（reader）들은 "Visual C++
6.0 '이나 API, 또는 MFC에 관한 전문 서적을 참고하여라．
 참고로 제0장은 "Windows 2000”에서 설치한 "Visual C++ 6.아을 사용하였고, 그 이후부티
는 " Windows XP Professional 평가본" 에서 설치한 "Visual C++ 6.0"을 사용하였다. 모니터의
화면 해상도는 1024x768 픽셀로 설정하였다. 그리고, 이전의 저서에서도 그랬는데, 상황에 따라
서 필요하면 Mathematica를 사용하여 보충을 하였다．
2   제0장       MFC (Microsoft Foundat山n （기asses)




0.2. MFC

0.2.1. 준비 과정

    MFC를 사용하기 위해서 반드시 거쳐야 할 과정이 있다. 계속 이어지는 설명을 잘 읽고 그대로
따라하기를 바란다．
    아래의 화면


      E｝伯 丘dir y e나 !n弓00 Era作Cr 旦UI너 Isa's 蜘ad口놔 He巾
      固 才 뇨，. 今二              1'         已 囹 噴r 뫄i          片   !

                                                        그
      重                :.11                  i!
                              j쯔




     Ready




은 "뀌sual C++ 6.0"을 컴퓨터에 설치하고 난 후 처음으로 실행한 화면을 나타낸다．
                                                                 "To아SI,
 좌측 상단을 보면 "File", "Edit", "View ", "Insert", "Pr이ect", "Build",        , "硼ndow",
"H이p " 가 나열되어 있는 Menu Bar가 있다．
    마우스로 "File " 메뉴를 클릭하면 하위 메뉴（subn祀nu)가 나타난다. 이 중에서 "New " 명령을
선택하면 아래의 ''New" 대화 상자
                                                                   제0장 MFC (M匕rosoft Foundat山n （기asses) 3




   仍
    퍼日 트dit 'S伯빠 伯red 巳이ed1 目,Id Ira忖 獅ndow 브eID
                                   ;
   自 旨       小戶        (               n   丙穹       乳

                                           i    如




                      Files   다ojects i Workupoces F Other Docamento 1

                      ！封ATLCOMA1 Wizard                                   Project name:
                      玉｝Cm引目 Resource Type Wizard
                      壘Co如rn App쌔zard
                      i，磊Database F가이吼t
                                                                          1소cation:
                      汗受 DevSlodio Add-ia 놔注ard
                      自 巳＜tended Stored Proc 낵仁ard                        :D:쌔Proyram Flles쌔Hlcrauoft Vis
                      幽 田Al거 Exten引（1n 나注ard
                      oJMokelile
                      際MFC ActiveX ConitoiWizard
                        水 MFC Ann나注ard Idlil                               1; -Qeate oew wt泌帥lace
                      出 MFC App쌔znrd 佃＜ej                                  尹 口   口    口
                                                                                          口




                       Ti Utility Project
                      西W,n32 Al艸C씨0n
                          Win32 Coosole Application
                          Win32 Dynam ic-Link Libromy
                      혠W'i032 Static 山rory

                                                                           eta甘o,ms:
                                                                           zWln32




   1
가 나타난다．
 이 대화 상자에는 "Files", "Pr이ects", "Workspaces", "Other Documents" 의 네 개의 탭이 있
다. 별다른 조작을 하지 않았다면 "Pr이ects" 탭이 선택되어 있을 것이다．
 왼쪽 부분에는 우리가 만들 수 있는 여러 종류의 프로젝트의 목록이 있는데, default으로
"ATL COM AppWizard pr이ect "가 선택되어 있다．
 ATL은 ｝小cro soft의 Act如e Template Library를 말하는 것으로, "ATL COM AppWizard
pr이ect "는 ATL에 바탕을 두고 있는 프로젝트의 작성을 돕는다. 이것이 뭐하는 것인지는 전혀
몰라도 된다. 우리는 단지 우리의 목적에 맞는 프로젝트가 어떤 것인지 알고, 그것을 선택해 주면
될 뿐이다．
 믿에서 여섯 번째에 "Ml兀 AppWizard (exe）까 있다. 이 프로젝트는 단독으로 실행이 가능하
고 기본적인 MFC 응용 프로그램을 만들고자 할 때 사용하는 프로젝트로서 , 우리가 선택해야 할
프로젝트이다．
 목록에 나와 있는 여러 가지 프로젝트들 중에서 "MFC AppWizard (exe) "를 클릭하여 선택한다．
4 제O장 MFC (Microsoft Foundation Classes)



 "Pr이ect name''은 자신이 원하는 프로젝트 이름을 써넣는 곳이다. 만약 함수의 그래프를 그릴
거라면 ''Pr이ect name'쎄 "함수의 그래프嶝 입력하면 좋을 것이다．
 "Location"은 앞으로의 몇 단계의 과정을 거친 후에 생성될 프로젝트가 저장（save）될 위치를
말하는 것으로, 자신이 원하는 경로（path）를 지정해주면 된다. 필자의 경우 default 위치에 저장
한다. 다만, 하나의 프로젝트는 하나의 폴더에 저장하는 것이 좋으므로 새로운 폴더를 만들어 저
장할 것을 권장한다．
 "Location" 에 의해 생성되는 폴더는 프로젝트가 저장되는 한 단계 위의 상위 폴더이고，
"Pr이ect name " 에서 지정한 프로젝트의 이름과 동일한 이름의 하위 폴더가 이 폴더 아래에 만들
어지고 그 폴더에 프로젝트의 파일들이 모두 저장된다.
 그 아래쪽을 보면 "Create new workspace똬 " Win32까 선택되어 있다. 이것들은 건드리지
않는다.
 설명대로 한다면 아래의 화면


    殲裁轟難難蘿難客難難發難難轟＝礪難4難蹄曲群
     E加 툐dli iew j009,t r0忙ci 표U沁 I0U四 mnd(｝나 bmD

    由 潘 如｛，뇨夕 1        『1
                       三三             吃因 땀 殃

    !‘艸如             J！小H            ’小J
                       d心



                       Fne8   什可cc恬 1 밖oriropacco 1 Other Docum亡O18

                       卜好ATL Co卜A AppWiznrd                           Project name:

                       盞빻，．‘磊걺잎' "' Wizard                            함수의 그래프

                       無少브쁘斗Pro．拌느．                                   Location:
                       t彗日配oiled Stored Proc 낵仁ard                    三O：甘Program Files甘1小crosoft V注 1i

                       歇쌥，旱
                          , ' " sin, Wizard
                       七薛MFC ActiveX Coot,이쌔zord
                                                                      r; Cr亡ote no甘workspace
                       群謐瑞헒瑥］
                       丁jUtil仕y Project
                         Win32 Application
                         나in끄 Console Application

                       器：
                        ：擺黜껍芍 "ihr "미
                                                                      Eta打arm뵤




과 같다．
                                                              제0장 MF（二（Microsoft Foundat幻n （긔asses) 5



 이제 "0K" 버튼을 클릭하면 응용 프로그램 작성을 위한 기본적인 source code를 자동으로 생
성해 주는 MFC AppW匕ard가 실행된다. 우리는 MFC A叩＼?Vizard를 통하여 나중에 생성될 프로
젝트의 architecture, features, functions을 선택할 수 있다．
 "OK" 버튼을 클릭한다. 그러면 아래의 呱4FC AppWizard - Step 1" 태화 상자


                                                                                                               1 小 X
    E陀 트Al ＼柶C noert   ro四C! 目川d l印가5 땜tdow j甘D

    由 由寸 .':           針             n그 因 담   팎

                                        r


                                                  'What type of application suould you like itt create?

                                                        Single Uocuine,,t

                                                     " Multiple dar.un,ent5

                                                       Qialog bused

                                                     V Ooco,nent凹ew architecture support口




                                                  What language would you like your renniircen in?


                                                    巨卜 극 거 [A叩WZK아(.DLL1




                                                                                  [m i帥      !        Canc亡1




가 나타난다．
 이 대화 상자는 우리가 만들고자 하는 응용 프로그램의 기본적인 구조와 resource에서 사용할
언어를 결정하는 역할을 한다．
  "What type of application would you like to create?''라는 질문의 답에 서］ 가지의
architectures가 나열되어 있고, '八4u1tiple documents "가 default으로 선택되어 있다．
 "Single document "를 클릭하여 설정을 바꾸어 보아라. 또한, "D洌og based''로도 설정을 바꾸
어 보아라． "닯ngle document " 와 呱札出아e documents" , 그리고 "D洌og based''의 차이가 무엇
인지 대충 알 수 있을 것이다．
 서］ 번째의 "D洌og based"는 응용 프로그램이 메뉴와 document人妃w architecture를 갖지 않
6 제O장 MFC (Microsoft Foundation Classes)



는 하나의 대화 상자만을 가지도록 한다. 硼ndows의 보조 프로그램에 들어 있는 계산기 프로그
램은 "D洌og based" 유형의 응용 프로그램이다．


                                                                                                         -Si勻封
                          떤집低） 보7I()        도욤맏也）




                              加三크士           艸1뇝豈   11크늬士    1늬브豈크
                           rHeo    CS ｛泊C    root    C 태0




                                     늬늬늬a
                                                                          B配比口配·     1     CE     1      C   ]
                                                                  그그H듸그그二-J쓰U스U
                                                                  二-j二工므그＝그므-j스Li
                                                                  U그＝그그H그二시쓰Li
                                                                  =ULL그＝U=U므그
                                                                  上그＝-1J- J- J＝그

 우리의 목적에 적합한 유형은 SDI(Single Document Interface) 구조이다．
 서］ 가지의 architectures 중에서 아래의 화면


           Mew Insert er이8CC 旦U刈 Iso由 蜘너OW 브e巾




                                                      ?What t甲e of applic싸on would you like to create?




                                                       What language would you like your resources in?




    Re耐V
                                                                             제0장 MFC (Microsoft Foundat向11 （기asses) 7



처럼 "Single document "을 선택한다．
                                                                                                                                      毗
 "Single document " 유형의 응용 프로그램으로는 \Vindows의 보조 프로그램에 들어
八Vindows 탐색기까 있다. 이 유형의 응용 프로그램은 하나의 작업 창을 가진다．
 한편, 하나의 응용 프로그램에서 여러 개의 "source code 편집 창'을 제공하는 "Visual C++
6.0우 呱4u出이e documents" 유형의 응용 프로그램이다. 만약 "Visual C++ 6.0'미 SDI 구조라
면 매우 불편할 것이다. 왜냐하면 다른 파일을 편집하려면 현재 편집 중인 파일을 닫고 다른 파
일을 열어야 하기 때문이다. 계속 이런 작업을 반복해야 한다면 매우 불편할 수밖에 없다.
 아래쪽에는 "What language wou넌 you like your resources in?"이라는 질문에 "한국어 "가
default으로 되어 있다. " 한글판 뀌sual C++ 6.0"을 설치해서 그런 것이다. 이것 때문에 나중에
프로그램의 메뉴가 " 파일（F) ", “편집（E) " , "보기（V) " , "도움말（H) " 과 같이 한글로 나타난다. 또한，
메뉴 말고도 버튼 같은 다른 resource에서도 "확인 " , " 취소" 등과 같이 한글을 사용하게 된다．
 다음 단계로 넘어가기 위해서 "Next >" 버튼을 클릭한다. 그러면 아래의 "MFC AppWizard -
Step 2 of 6" 태화 상자

                                                                                                                          _J,4j. cJ
       E的 토dii Vi므w 1Sued 巳이oc! 旦wid louis 뽀odow feb

       固 哮 )               」1            口 因탐          i六！                           느    中1

   !                 -Jr


                                                             : 꿔hat database auppoui would you like to Indude?

                                                             【     序 系1오at

                                                                   1 Htader tiles oaiy

                                                                      Database,月e叫 낟Ithout lii亡 support

                                                                      Database view with tile support

                                                                 II you include a database view, you must select a
                                                                 data source




                                                                   No data 돠｝Urre 油 3亡1亡cted.




                                                                                                日ft油I,    }      Cancel
8 제0장 MF（二（Microso什 Foundation （기asses)



7} 나타난다．
 이 단계는 database를 지원하는 기능을 포함시킬 것인지의 여부를 결정하는 단계다．
 우리의 목적과 d砒abase는 전혀 콴계가 없다. dafault으로 선택되어 있는 "None!'을 그대로 놓
아 둔다．
  'Next >" 버튼을 클릭하여 다음 단계로 넘어간다. 그러면 아래의 "MFC AppWizard - Step
3 of 6" 대화 상자


    ！긔e 툐dit   lew Inn日n 므m忙Ct 昏川d l口'Is 뾰rdow H희口

    곧） 旨小，/              71            ［乙 囹 會   殃




                                                     What compound document cupportatould you like to
                                                     include?

                                                         Npne
                                                          Container
                                                         卜lini뗘 erVer
                                                          Fr,汁server
                                                          Both container and server




                                                     What other support would you like to include?


                                                        ' A出omatlon
                                                       \/ActivnX Cnnttoln



                                                                                   터niol,            Cancel

                                                                               轟難轟二難崖蹄融攝辨轟瑟纛轟




    Ready




7} 나타난다．
 이 단계는 복합문서（con叩ound document)를 지원하는 기능을 포함할 것인지 여부와 Act如eX
에 관한 code를 생성할 것인지 여부를 결정하는 단계이다. 복합문서는 그림 파일, 소리 파일 등
이 삽입되어 있는 워드프로세서 파일처럼 여러 종류의 데이터를 담고 있는 문서를 말한다．
 "What compound document support would you like to include?''라는 질문의 답에 default
으로 "None”이 선택되어 있다. 그대로 놓아둔다．
 한편, 아래 부분에는 "Aut毗ation꽈 "ActiveX Controls삐 있다. 이것들은 ActiveX에 속하는
                                                             제O장 MFC (Microsoft Foundation Classes) 9



기술이다．
 이전에는(form아ly) OLE Aut毗ation이라 알려졌던 automation은 한 응용 프로그램이 다른
응용 프로그램에서 구현된 objec始를 조작하는 것을 가능하게 한다. Exc이이나 피sual C++ 같
은 많은 상업적인 응용 프로그램들은 기능（functionality）의 많은 부분을 사용자가 automation할
수 있도록 허용한다. 예를 들어 , 피sual C+＋에서 , VBScript macros를 쓸 수 있다．
 default으로 선택되어 있는 ''ActiveX Contr이S'딴 ActiveX의 여러 가지 기술들 중 핵심 기술
이다. 요즈음에는 ActiveX를 Active technologies라 한다. Active techn이ogies는 소프트웨어
components7]-, 그들이 어떤 언어에서 생성되었는지에 개의치 않고, 네트워크화된 환경에서 다른
components와 서로 상호작용하는 것이 가능하게 하기 위해 Component Object Model (COM)
을 사용한다. Active techn이ogies는 데스크톱이나 인터넷에서 실행되는 응용 프로그램들을 생성
하는 데에 사용될 수 있다. 우리의 목적과 Act加eX와는 무관하다. 체크 표시를 클릭하여 선택을
해제하여라．
 다음 단계로 넘어가기 위해 "Next > " 버튼을 클릭한다. 그러면 아래 그림처럼 " MFC
AppWizard - Step 4 of 6 " 대화 상자

   難竄烏弑4寡如小뇨，       k盖m 1놔芯攝攝難輛灘難蘚y小必H
    lIe 目批 Me나 !tart Et이act 旦slId ISO忖 뾰ndow tints
    由 嗜 三，
         f/ 諍           秀缸          n因밈      叭！

    I              Ji                  ji




                                                      9 k1附at 且tatus h甘
                                                      戶 Erlndng and 列恤 恥tv拓甘
                                                      !m Costa朴$亡as附V亡 岫료巾
                                                       ' l D con打따S
                                                      尸 hI肴꺼 斛ease恥ag AF쩍
                                tm1小1m什 mm;d          I尸 螂ad呻$ Soc如ts
                                                     NOW 如 如U 늬ant 卯出 to曲如$1이的凹

                                                      了； 村minb1
                                                      尸 tnt旺rn亡tE川piers, RoBs四
]0   제0장   MFC (Microsoft 尸oundation 이asses)



가 나타난다．
 이 단계는 응용 프로그램의 사용자 인터페이스를 다양하게 조종하는 역할을 한다. 쉽게 말하면，
응용 프로그램을 어떤 모습으로 보이게 할 것인지 결정하는 것이다．
 "Docking to아bar''는 응용 프로그램이 명령어를 실행시킬 수 있는 버튼들이 들어 있는
docking toolbar를 가지도록 한다．
 "Initial Status Bar''은 main 창의 아래 부분에 상태 표시줄이 나타나게 한다．
 "Printing and print Preview"는 말 그대로 인쇄와 인쇄 미리보기 기능 설정에 관한 것이다．
 "Context-sensitive He如"를 선택하면 도움말 작성을 위해 도움말 프로젝트 파일（.hpj) 과 배
치 파일 MakeHelp.bat을 만든다．
 "3D con甘아5 ''는 응용 프로그램의 사용자 인터페이스에 3차원 모양을 넣는 code 작성 여부를
결정한다．
 "MAPI (Messag이ng API) "는 mail-enabled and mail-aware 응용 프로그램들이 mail
messages를 생성 , 조작, 저장하기 위해 사용하는 함수들의 집합이다. MAPI는 응용 프로그램 7下1
발자들이 underlying messaging system에 독립적인 mail-enabled and mail-aware 응용 프
로그램들을 생성하기 위해 사용할 수 있는 공통의 인터페이스를 제공한다．
 "Windows Sockets "는 socket 프로그래밍을 할 수 있도록 지원한다. socket은 통신의 종점
(communication endpoint)이다. Windows Sockets 응용 프로그램은 네트워크를 통하여 data의
packe始을 주고받는다. sockets에는 stream sockets와 datagram socke始이 있다. 사용자가 통
신의 양 끝에서 MFC를 사용할 때, MFC sockets을 사용하면 매우 좋다．
 그 밑으로 "How do you want your toolbars to look?"이라는 질문에 defau卄으로 선택되어
있는 "Normal"은 보통의 입체 버튼을 가진 도구바를 제공하고 "Internet Explorer Rebars"는
익스플로러의 도구바와 같은 모양의 도구바를 제공한다．
 하단에는 "How many files would you like on your recent file list?"라는 질문이 있다．
Windows의 레지스트리를 많이 편집해 본 사람들이라면 레지스트리 항목 중에 MRU (most
recently used) 항목을 알 것이다. MRU 항목에는 가장 최근어］ 사용한 파일 목록이 저장되어 있
는데 이 값에 따라 목록에 저장할 수 있는 파일 개수가 달라진다. 파일의 개수가 이 값을 넘게
되면 가장 오래된 파일 순서대로 삭제되고 새로운 파일로 갱신된다．
 "Advanced Options " 버튼이 있는데 여기에서 한 가지 설정해 줄 사항이 있다．
 "Advanced Options" 버튼을 누르면 아래
                                                                              제O장 MFC (Microsoft Foundation Classes) 11



   .E的 토d卄 Me놔 tflsot er아ccl 旦uuld lea怡 뾰ndow be巾
   油   滓 長寸瀯     >,   1 好      * 乙： nq3因땜                   殃r

                      J                    哮
                          d毖


                                                                                                            tI xl

                                           Document           T亡mplale Ste油go   1 Windo늬St넌亡＄ i
                                                      Nun-localized strings

                                                        File e넴ennion:           File type 10:
                                                        1                        }My. 加coment


                                                      1oca1i2ed St,iags

                                 tmd叫 i노
                                                       Lnngnage:                 Main frame 必Pt油n;
                                 匡 C11t1
                                                        한국어                      三함수의 그래프

                                                       Dec 押pecan妃：              ti仇rname:

                                                       ;My

                                                       File new name Ishart      Ff1亡 type cam亡 加ng
                                                       nam이：                     names
                                                        My                       Mv Document



                                                                                                     口one           Can,：亡1




와 같이 된다．
 "Document Template Strings" 탭과 " Window Styles" 탭이 있다．
 사용자는 " Window Styles " 탭에서 " main frame 창" 의 스타일을 바꿀 수 있다．
 frame 두께를 thick으로 할 것인지 thin으로 할 것인지 지정할 수 있다．
 창이 " 최소화 버튼(I\小nimize button) "이나 " 최태화 버튼（Maxin五ze button) "을 가질 것인지의
여부를 지정할 수 있다.
 창이 초기에 어떤 크기로 나타날 것인지의 여부를 지정할 수 있다. 창이 초기에 최대 크기로
나타날 것인지 , 최소 크기로 나타날 것인지 , 아니면 default으로 설정되어 있는 크기로 나타날 것
인지를 지정할 수 있다．
 SDI 응용 프로그램의 경우, framework에서 창의 스타일은 default으로 캡션（caption）과
border를 가지고 있으며 제목 표시줄에 "Con甘아기nenu box묵 가지고 있다．
 "Window Styles " 탭을 선택한다. 그러면 아래의 화면
]2   제0장       MFC (Microsoft Foundat山n （긔asses)




     E沁   d,I 냄므w 'flse1 日口已켜 旦U小J In'기S 好r,dow 匕甘口

     곧） 昏                              껀］ 丙 智 泌




                                             '   lJg! 卦빠냄nd쓰M

                                            卜da1n 和mist 500'地드
                                             17 Th노k home        '   System me

                                             !7 M1ntmtZe box         Miniinized

                                             ,7 !d斗dmze box          Mo넙m注ed




과 같이 된다．
 화면 중간 쯤에 "Main frame styles "가 있다. 몇 가지 옵션이 있는데 "Minimized똬
呱4aximized"은 프로그램을 실행시키면 생성되는 "main frame 창"을 기본적으로 어떤 크기로 시
작할 것인지 설정한다. "Max而zed"을 설정하여 주면 프로그램이 실행된 후에 최대 크기의
"main frame 창"이 만들어지고, "Minimized''을 설정하여 주면 프로그램이 실행된 후에 최소 크
기의 "main frame 창'이 만들어진다．
 呱4aximized''를 설정해 준 후 " Close " 버튼을 누른다. 그러면 다시 '爪4FC AppWizard 小 Step
4 of 6" 대화 상자로 되돌아온다．
 다음 단계로 진행하기 위해 "Next > " 버튼을 클릭한다. 그러면 아래의 ''MFC AppWizard -
Step 5 of 6" 대화상자
                                                                              제O장 MFC (Microsoft Foundation Classes) 13


   功
    E的 트d作 쯔ew !nu日fl Erolect 恥m 工00怡 批od口낵 tjeip

    匡｝ 潘 卄， ;11               ,    二） 口因탬                恥i

                    寸                        二j重




                                                                     Whnt ul너e of project would you like ?
                                  rd1 Ed11 y1t1 !1trt 肛Hd 卄ue
                                  1 1 I I , 1 I口그
                                                                        . MI- C Standard
                                                                           Wiadu나S 트op油rer


                                                                     Would you like to generate source tile otiruntents?

                                                                기       ' ouu. pleese
                                                                           No. thank you
                                                                     How would you like to use rite MFC library?

                                                                        1Au a uhared UtI

                                                                           An a gtatioolly linked library




                                                                    <80比          Next>               Finlub   三       Cnnr,el




   F七 a




7} 나타난다．
 이 단계는 사실상 프로젝트 생성을 위한 옵션 선택의 마지막 단계라 할 수 있다．
 "What style of pr이ect wou넌 you like?"라는 질문에 "MFC Standard까 default으로 선택
되어 있다. 이것은 응용 프로그램에 하나의 미ew를 보여 준다. "Windows Explorer "는 프로젝트
의 스타일이 \Vindows의 익스플로러와 매우 비슷해서 붙여진 이름이다. 이것은 "MFC Standard"
와는 달리 정적 분할 \window를 수직으로 나누어 view7} 별도로 나타나게 한다.
 두 번째로 " Wbu넌 you like to generate source file comments"라는 질문에 " Yes, 미ease"
가 default으로 선택되어 있다. 이 옵션은 source code에 주석문을 표시하는 기능을 한다. 주석
을 달면 AppWizard어］ 의해 만들어지는 함수 내부에 어떤 co（扼를 써 주어야 할지 알 수 있으므
로 co（五ng할 때 상당히 도움이 된다．
 세 번째 선택사항인 "How would you like to use the MFC library?"은 응용 프로그램이
MFC 라이브러리에 연결되는 방식을 선택하는 것이다. MFC 라이브러리를 프로그램에 연결하는
방법에는 정적인 연결과 통적인 연결의 두 가지가 있다. 정적으로 연결할 경우 프로그램의 단독
실행이 가능하지만 프로그램의 크기가 커진다. 동적으로 연결할 경우 프로그램의 크기가 줄어들
14 제O장 MFC (Microsoft Foundation Classes)



므로 보통은 동적으로 연결한다．
 이 단계에서도 변경할 것은 없다．
 다음 단계로 넘어가기 위해 "Next >" 버튼을 클릭한다. 그러면 아래의 "MFC AppWizard -
Step 6 of 6" 대화 상자


        E的 目lii 냄므닙r m드0,1 已0円亡t ＆川d ！口川＄ 竺qndC\Y 匕e油

    自 已；                                 口 回 돤r     泌                      中    的

    !                   小                   :j



                                                                        cc the I,내owing classes 化r


                                                          아lyApp
                                                          Cl,切inFrame
                                                          C卜才ylJoc




                                                          Class name:           leader file:

                                                          {C卜,4yVies/          함 4口 그래 프V沌V/

                                                          Base class:

                                                          (v沌닙




                                                        (Back




    Ready




7} 나타난다．
 이 탄계는 AppWizard가 생성할 클래스들에 대해, 각 클래스의 이름, base class, header 파
일, 구현 파일을 보여 준다. 위의 화면에 나타나 있는 것처럼 CMyView 클래스에 대해, base 클
래스는 CView 클래스이고, header 파일은 " 함수의 그래프뀌ew.h"이며, 구현 파일은 " 함수의 그
래프뀌ew.cpp''이다. 또한, C八4yView 클래스 아래에 있는 CMyApp 클래스에 대해, base 클래스
는 CWinApp 클래스이고, header 파일은 " 함수의 그래프．h"이며 , 구현 파일은 "함수의 그래
프．cpp "이다. （玉4yApp 클래스 아래에 있는 CMainFrame 클래스에 대해, base 클래스는
CFrameWnd 클래스이고, header 파일은 "入4ainFrm.h"이며 , 구현 파일은 " 八/IainFrm.cpp "이다．
마지막으로, CMainFrame 클래스 아래에 있는 CMyDoc 클래스에 대해, base 클래스는
                                                                        제O장 MFC (Microsoft Foundation Classes) 15


CDocurnent 클래스이고, header 파일은 " 함수의 그래프Doc.h"이며 , 구현 파일은 "함수의 그래프
Doc.cpp"이다． 사용자는 이 단계에서 응용 프로그램의 클래스들의 이름을 바꿀 수 있다．
 이 단계에서도 변경할 것이 없다．
 이제 모든 설정을 완료하기 위해 "Finish" 버튼을 누르면 아래의 "New Pr이ect Information '
대화 상자

   多磁，                                                                                                   표毋 즈
         In 툐dii Hiew 椰err E山忙Cl 旦ulld Iou奴 如nd口w Help

    匡




                                       AF甲냄如rd 닙川 亡lea忙 a ne낳 址如佃I PIO如ctw川tth亡 幻山8W的 spec枷硝ens:


                                       ;Applies如a type of 함수의 그래프：
                                          引ogle Oacu毗lit Interface A卯血曲m targeting:
                                             Wtn32

                                        Classes to be created:
                                          Ap畔口心an: Cfk艸卯 is 함수의 그래 프．h and 함수의 그래 프cpp
                                          Frame: CUalnFram亡 in MalaFrm.h and MainFrm.cpp

                                          (b:ournC裁咎罷븍蒙離畿黑馮壤陞筐猪詔p
                                          View:
                                        Features:
                                          C In川at 佃0由aria main frame
                                         + Initial status bar in main frame
                                         + Printing and Print Previe놔 noppo.t in view
                                         + 3D Controls
                                         + Uses shared OIL implementation PrlFC42.OIIJ
                                         + Localizable text in:
                                              한국어



                                       Pr이亡ct｛기ret才ory:
                                 mm    Dm什四ram Files卄lii油anott V注oat S仙di          可cc招卄함수의 그리促


                                                                                Li二二dk1二4



   Re




가 나타난다．
 이 대화 상자의 안에 있는 내용들을 천천히 살펴보아라. 무엇을 뜻하는지 잘은 몰라도 낯이 익
은 내용들이라는 것을 알 수 있다． 이 대화 상자는 지금까지 우리가 선택하였던 여러 가지 선택
사항들을 바탕으로 하여， 생성할 skeleton pr이ect의 spec而cations를 보여준다. 여러 가지 내용
들이 나타나 있다．
 위의 화면과 비교해 보고 이상이 없으면 " OK" 버튼을 클릭한다. 그러면 아래 화면
16   제O장          MFC (Microsoft Foundation Classes)



     '1 헒＋斗 그려프     !Q?icrr的良 \4g口놔 :41

      E陀 트it     teW insert Er이cc' 旨川d lool$ 뾰odow t如m

      由 潘 枷口                寸     二 5     ,   口因담    엮i        !;   小1

     小 ‘小m心Hn.          d卜，'tt U, " nn,n      心i er』
                                                   d1gm!{｝注   寸＼ !       쌉 芦   !   i1




     Ready




이 나타난다．
 처음 "Visual C++ 6.아을 실행시켰을 때와 비교하여 보아라．
 "ClassView", "ResourceView", "FileView " 의 서］ 가지 탭을 갖는 "Pr이ect Workspace 창"이
나타났다. " C坮弱Vi이VI'가 default으로 선택되어 있다．
 "ClassView "는 클래스들과 클래스들의 m이ithers을 보여준다. 클래스를 펼쳐서 그 클래스의
members을 표시하려면 클래스 아이콘을 더블클릭하거나 아이콘 아래의 ''+'' 기호를 클릭한다．
 "ResourceView"는 프로젝트에 포함되어 있는 resource 파일들을 표시한다. 폴더를 펼치면
resource 유형을 알 수 있다．
 'FileView'牛 프로젝트와 관련되어 있는 파일들을 표시한다. 우리는 "File View "를 통해 프로젝
트와 pr이ect workspace어］ 포함된 파일들의 관계를 알 수 있는데, 이 관계는 물리적인 관계가
아니라 논리적인 관계이다．
 下ileView "를 클릭한다. 그러면 " Pr이ect Workspace 창"이 아래의 그림
                                    제O장       MFC (Microsoft Foundation Classes)   17



                      咽낚／毗space '함수의 그래프':1 p5加叫司
                      莩 學함수의 그래프 lileo




                     ！虹Ia匙枷넜餐Re叩빤녠k多I無日1eV啣尸



처럼 바뀐다．
 "함수의 그래프 files " 앞에 " + " 기호가 있다. 이걸 클릭하여 트리 구조를 펼치면 아래의 그림


                      「겨 w아kspace '함수의 그래프':1 pro加eti司
                      多 擢함수의 그래프 tlleo
                         年 :.] Sours亡 flea
                         , .J Header Files
                         多 =J Resouru才 Files
                           重 ReadMe.txt




                     쓰Cl挺典핸i茹R쁘旦뽀堡姓以無F姓姓可H
18   제0장   MFC (Microso竹 Foundation （기asses)



처럼 " Source Files", "Header Files", "Resource Files", "ReadMe.txt" 의 네 가지 하위 항목이
나타난다．
 "ReadMe.txt "를 제외한 서］ 항목 앞에는 " + " 기호가 있다. "ReadMe.txt " 에는 응용 프로그램을
구성하는 여러 파일들에 관하여 간단한 설명이 들어 있다. 한 번쯤 이 파일을 읽어 보는 것도 좋
을 것이다．
 "Source Files " 앞에 있는 " + " 기호를 클릭한다. 그러면 아래의 그림


                               月 낚／orkspace ’함수의 그래프 ' :1 Pr미C'川司
                              i三1 番 함수의 그라巴 Ill亡S
                                  E ｛씌 Seurce Files
                                       自 卜.iulnFrm.cpp
                                       꾜 StdAfx.cpp
                                     尸 固 함수의 그래프띠｝P
                                     L塑 함수의 그래프.rc
                                       匈 함수의 그래프Dot.印p
                                       쓰 함수의 그래프V伯m印p
                                  1 니 Heoder Files
                                  主 口 lies,,山C亡 Flies
                                    邕 fleudMe．뇨t




                              H아的m川蜘駟塑斗恤d垂日枉撫可H


처럼 확장자가 rc인 파일 하나와 확장자가 cpp인 파일 몇 개가 보일 것이다．
 "함수의 그래프.cpp "는 CMyApp 클래스를 포함하는 main source 파일이다．
 "함수의 그래프．rc "는 프로그램이 사용하는 모든 윈도우즈 resources의 목록이다. 이 파일은
res 하위폴더에 저장되어 있는 아이콘, 비트맵, 커서를 포함한다. 뮈sual C+＋에서 직접 이 파일
을 편집할 수 있다. 참고로, res 하위폴더에 n함수의 그래프．rc2"7} 있는데, 이 파일은 Visual
C+＋에 의해 편집되지 않는 resources를 포함한다.
 呱4ainFrm.cpp”는 CM小nFrame frame 클래스를 포함한다．
 ”함수의 그래프Doc.cpp"는 CMyDoc 클래스를 포함한다．
 "함수의 그래프View.cpp"는 （弧/lyView 클래스를 포함한다．
 위의 파일들 중에서 우리가 최종적으로 선택하여야 할 파일은 처음에 입력했던 프로젝트 이름
인 " 함수의 그래프" 에 \Tjew7} 붙어 있고 확장자가 cpp인 파일, 즉, " 함수의 그래프View.cpp "이
                                                                               제0장 MFC (Microsoft Foundation Classes) 19



다．
     ”함수의 그래프뀌ew.cpp'딸 더블 클릭하여라. 그러면 아래의 화면


      曲    f加 丘d艮 y cw Insoil En加Ct 且slId In이＄ 邯ndow 甘e如

      詐管 畔日1 ，多 宅 1引 二小 !:＝나呵因曾 斗1                                                         네 "it 1
      JcIAyview 깁 (All clasS membe『司네f:!Jy\4械                                             크奴＋ 冷潘墨 ! 艱6!
                                                   t二i씌   // 좝수희 그래프Uien.cpp : 1.1呻lenentati이1nf the 口늉Vies. class
            Wnrkqonr. .한＝＞으1 기 ?II I工1· 1 nrniPr寸fqI      ii
          好 簪함수의 그라匡 tiles                                幷incluile " stdafu.h"
            多녀恣 Source Files                              hioclude " ‘함수의 그래프．h"
                 盈 MainFrin.cpp
                因 SIdAt乂.cpp                              口include " 함수의 그래프hoc小"
                固 함수의 그래프셔）p                              甘include " 함수의 그래프Uiew.h"'
                淘 함수의 그래프.rc
                由 함수의 그래프山乙cpp                            Iledef DEBUG
                                                          出lef inc flea DEBUG 旺H
                 川함수의 그래프吼w.cpp
                                                          Bonder THIS FILE
            泛 口 Head亡rFi노S                                static char THIS_FILE口 - _FILE_ ;
            汗m口 m印urce Files                              Dendif
              望 ReadMe.bcl
                                                          /////////////////////////////////////////////////////////////////////////////
                                                          // c！匈tien

                                                          ll1LEHtHl_DYlOBEDTE(CHijUiea, CUies.)

                                                          BECIN_旺SS肥E_1mP(ClHlUieo, CUiew)
                                                               lit t 0F5lnst_HDF(c札oiew)
                                                                     ii I 1TE - tIle ClassUizard 片ill add and reFa1ue mapping macrun here -
                                                                     ii     0h HUT CDII what ynn see in these hiocks of generated cnde!
                                                               //}}AFII lOG 14fF
                                                               ii Standard printing comuands
                                                               DHC0I*I小I( ID_FILE_PRINT 1 CUies. rBoFilePrint)
                                                               UN_C0卜R1III( ID_FILE_PRINT_DIRECT. Coiew: :0oFilepriot)
                                                               0H_C0I*111UI(ID_FILE_PRIHT_PREVIEV, CHico: :onrilePrintPreuiew)
                                                          E10I I在弧叩E_HUP()

                                                          liI/ il/ //lilill/     lfl/ ull/ l/ llllll/    lil/ lll/ ilill/     lllIllll/     /ilillll/     /lllill/   llli
                       狙鹿uourcV如미盈쯔쁘브


      萱
           41斗＼如社d乂on奴熙＼竹也In F姮呈l入只rid In艮U長之入R旦熟d匿／                                                                                                                        !1中
                                                                                                                                    [uii.     c.ii      .........廷珏:011面瓦而而




 과 같이 " source code 편집 창" 에 " 함수의 그래프View.cpp" 의 source code가 나타난다．
     드디어 우리에게 필요한 프로젝트가 생성되었고, 우리가 작업할 " source code 편집 창" 도 준비
되었다．
     main 메뉴 중 '1Build" 메뉴를 클릭한 다음 "Rebuild All'' 명령을 실행시켜라. 그러면 생성된 프
로젝트가 컴파일과 링크 과정을 거치게 되어 실행 파일이 만들어진다. "I之ebuild All'' 명령은 프로
 젝트의 모든 파일들을 building한다．
     참고로, 개발환경（development environment) 외부에서 프로그램을 building하려면, 명령 프롬
프트（co跏rnnd pron叩t)나 makefile에서 build 옵션을 지정한다. CL.EXE는 Microsoft C와
C++ compilers와 linker를 조정하는 32-bit 도구이다. compilers는 Common Object File
Format (C아下） object (.OBJ) 파일들을 생성하고, linker는 실행파일들이나 dynamic -link
libraries (DLLs）를 생성한다．
20 제0장 MFC (Microsoft Foundation Classes)



 파일을 실행시키기 위해서 "Build" 메뉴를 다시 클릭한 다음 "Execute 함수의 그래프. exe" 명
령을 실행시킨다. 그러면 " AppWizard" 에 의해 생성된 프로젝트의 실체（2）가 드러난다．
 아래의 화면

                                                           -III뇌
    파딜（E) 편집（D 보7Ky) 도旨닫但）
     [:) 4 日   1｝기 吼 毋   g




    준d1




처럼 되어야 한다．
 "source code 편집 창" 에 자동으로 작성된 source code는 다음과 같다. 중간 쯤에 OnDraw
함수가 있는데 이 함수 내부에 그림을 그리는 co(扼를 추가시키면 된다. OnDraw 함수가 main
함수라 생각하면 된다．


0.2.2. Source Code

// 함수의 그래프View.cpp : implementation of the CMyView class
III
                                                         제Oj MFC (Microsoft Foundation Classes) 21



#include "stdafx.h"
荊nclude " 함수의 그래프．h"


荊nclude " 함수의 그래프Doc.h'
荊nclude "함수의 그래프View.h '


#ifdef _DEBUG
#define new DEBUG_NEW
#undef THIS_FILE
static char THIS_FILE [I = _FILE_;
#endif


/////////////////////////////////////////////////////////////////////////////
II CMyView


IMPLEMENT_DYNCREATE (CMyView, CView)


BEGIN_MESSAGE_MAP (CMyView, CView)
           // { {AFX_MSG_MAP (CMyView)
                      II NOTE 中 the ClassWizard will add and remove mapping macros here.
                      II      DO NOT EDIT what you see in these blocks of generated code!
           //} } AFX_MSG_MAP
           II Standard printing comnands
           ON_COMMAND (ID_FILE_PRINT, CView::OnFjlePrint)
           ON_COMMAND (ID_FILE_PRINT_DIRECT, CView::OnFilePrint)
           ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView: :OnFilePrintPreview)
END_MESSAGE_MAP 0


/////////////////////////////////////////////////////////////////////////////
II CMyView construction/destruction


CMyView::CMy View 0
    22 제O장 MFC (Microsoft Foundation Classes)



     {
            1/ TODO: add construction code here


    }

    CMy View:: -CMyView 0
     {
    }

 BOOL CMyView::PreCreateWindow (CREATESTRUCT& cs)
    {
            7/ TODO: Modify the Window class or styles here by modifying
            // the CREATESTRUCT cs


            return CView::PreCreateWindow (cs);
}

/////////////////////////////////////////////////////////////////////////////
II CMyView drawing


void CMyView::QnDraw (CDC* pDC)
{
           CMyDoc* pDoc = GetDocument 0;
           ASSERT_VALID (pDoc) ;
           II TODO: add draw code for native data here
}

/////////////////////////////////////////////////////////////////////////////
1/ CMyView printing


BOOL CMyView::onPreparePrinting (CPrintlnfo* plnfo)
{
                                                          제0장 MFC (Microso竹 Foundation （기asses) 23



           1/ default preparation
           return DoPreparePrinting (plnfo) ;
}

void CMyView::OnBeginPrinting (CDC永 小pDC玎, CPrintlnfo水 /*이nfo木／)
{
           7/ TODO: add extra initialization before printing
}

void CMyView::OnEndPrinting (CDC半 小pDC玎, CPrintlnfo永 /*pli寸0率／)
{
           /7 TODO: add cleanup after printing
}

//////////,///////////////////////////////////////////////////////////////////
7/ CMyView diagnostics


荊fdef DEBUG
void CMyView::AssertValid 0 const
{
           CView::AssertValid0;
}

void CMyView::Dump (CDumpContext& dc) const
{
           CView: :Dump (dc);
}

CMyDoc* CMyView::GetDocument0 7/ non-debug version is inline
{
           ASSERT (m_pDocument ->1sKindOf (RUNTIME_CLASS (CMyDoc)));
           return (CMyDoc*) m_pDocument;
24 제O장          MFC (Microsoft Foundation Classes)



}
#endif I/_DEBUG


I/III/I//I/IIIII/II/I/III/I/III/IIIIII/III/I/IIIIIIIII/IIII///IIII/II/II/IIII
II CMyView message handlers
정전기학（Electrostatics)
                      저나
                                  1
                           n1J/
                                                 의7排
                                  非ectromagri베＄111）


1.1. 정전기학（Electrostatics)

 정전기학 또는 정전기마당（electrostatic Ii이d）은 아래의 세 가지


(1) 모든 전하（charge）는 공간적으로 고정되어 있다．
(2) 모든 전하밀도는 시간에 따라 변하지 않는다．
(3) 전하는 전기마당（e旭야nc field）의 원천（source）이다．


를 가정한다. 즉, 정전기마당은 시간에 따라 변하지 않는 전하분포에 의해 생기는 전기마당이다．
 독자는 전자기학 강의 시간에 정전기학 분야를 배웠을 때 임의의 점에서의 전위佃lectric
potential) , 임의의 점에서의 전기마당의 세기（electric field intensity) , 전하 상호간에 작용하는 힘
(force) , 전기마당 내에 축적되어 있는 에너지 등을 구하려고 했을 것이다. 이 책에서 필자와 독자
들은 전위와 전기마당벡터（electric field vector）를 프로그램으로 구현하여 볼 것이다．



1.2. 정자기학（Magn이ostatics)

 전자기학佃扼ctromagnetism)에서 정전기학(ele야rostatics）은 정지해 있는 전하들간의 관계를
다루는 분야이다. 전자기학（electromagnetism)에서 정전기학 다음으로 다루는 분야는 정자기학
 28 제］부 정전기학（Electrostatics)



     (magnetostatics）이다. 정자기학은 일정한 평균속도로 움직이는 전하들 사이의 힘과 관련이 있다．
      전하의 흐름을 전류（current)라고 한다. 정자기학에서 다루는 전류는 흐름의 속도가 변하지 않는
정상전류（stationary current) 이다．
      정자기마당을 배울 때 독자는 자기선속佃agnetic flux) , 자기선속밀도（magnetic flux density) ,
자기마당의 세기 등을 구하려고 했을 것이다. 이 책에서 정자기마당은 프로그램으로 구현하지 않는
다．
1,3. 헬름홀쯔 정리（Helmh이枉 Theorem)

  헬름홀쯔 정리는 어떤 유한영역 안의 모든 점에서 벡터 마당（field of vector）의 발산
(d汁ergence）과 회전（curl)을 알면 벡터 마당을 유일하게 결정할 수 있다는 것을 말한다．
     벡터 마당 F= F佃，y, 기 = F (r）에 대해서 발산 \7 · F= b (r）과 회전 \7 x F = c (r）이
유한영역 I/ 내의 모든 점에서 위치의 함수로 알려져 있다고 하자. 아래




                               少（『）:+,I 牛쩍
                               A(r)：슈／, 牛푸
와 같이 두 함수를 정의하면 헬름홀쯔 정리는 F(r）를


                           F (r) ＝小 口m (r) + V X A(r)


처럼 d）과 (2）로 나타낼 수 있다는 것이다. 여기에서 1卜r/ 1 은 상대위치벡터의 크기이다．
     少 (r）와 A(r）로부터 F(r）이 구해지기 때문에, \7j와 \7XA를 마당의 샘（source）이라고 한
다. 그리고, F (r）를 계산한 위치 r을 마당의 점이라고 하며 , 적분을 할 목적으로 샘이 계산된 위치
F,을 샘의 점이라고 한다. dr'은 샘의 점이 있는 부피요소（V이ume 이ement)이다．
     위 식의 미분은 마당의 점에 대한 것이다. c15(r）와 A(r）를 미분하여 F(r）를 얻으므로, 각각 스
칼라퍼텐셜（scalar potential) , 벡터퍼텐셜（vector po扼nt怡1)이라고 한다．
     샘이 무한대에 있어서 유한영역 내에 있지 않으면 헬름홀쯔 정리는 성립하지 않는다．
                                     제1장 전자기학（Electromagnetism）의 기본이론 29


 마지막으로 발산은 전하의 샘이고, 회전은 전류의 샘이라는 사실을 알아두어라．



1.4. 마당의 분류

 벡터 마당（field of ye야or）의 발산과 회전은 서로 독립인 연산이다. 그러므로, 두 가지 중 하나만
으로는 벡터 마당을 완전히 기술할 수 없다. 전자기학에서 공부하는 마당은 다음의 4가지 중 어느
한 가지에 속한다. 문제를 풀고자 하는 마당이 4가지 중 어디에 속하는지 아는 것은 중요하다. 왜냐
하면 그것은 문제를 푸는 과정을 알려주기 때문이다．


1.4.1. 제1종 마당

 벡터 마당 F(r）이 영역 내의 모든 점에서


                            V · F (r) = 0                             G)
                            V x F(r) = 0


을 만족하면 제1종 마당이다．
 그런데, 벡터의 회전이 0이면 이 벡터는 아래


                            F(r) =-Vm (r)                             @)


와 같이 스칼라함수의 기울기（gradient)로 표현할 수 있다. 위 식을 (3）에 대입하면


                           v · (- v中) =0
                            .'. V2cJ (r) =0


을 얻는다. 위 방정식은 라플라스 방정식（Laplace equation）이다．
 결론적으로, 제1종 마당 문제는 영역의 겅계에서의 조건을 만족시키는 라플라스 방정식을 푸는
것이다. 스칼라함수 少를 구하게 되면 벡터 마당 F (r）는 4）로부터 구할 수 있다．
 전하가 존재하지 않는 영역의 정전기마당（electrostatic field）이나 전류가 없는 영역의 자기마당
(magnetic field）은 제1종 마당에 속한다．
30 제］부 정전기학乍ectrostatics)




1.4.2, 제2종 마당

 벡터 마당 F (r）이 영역 내의 모든 점에서


                            V · F (r) ；亡 0                  (5)
                             V x F(r) = 0


을 만족하면 제2종 마당이다. 벡터 마당의 회전이 0인 사실은 제1종 마당과 같으나, 벡터 마당의 발
산이 0이 아니라는 사실은 제1종 마당과 다르다．
 벡터의 회전이 0이므로


                            F(r) =-V少 (r)                   6)


처럼 나타낼 수 있다. 위의 식을 (5）에 대입하면


                            V · （小 \7少）；亡 0
                             '   \72j (r) = (7


을 얻는다. 여기에서 (I는 0이 아닌 함수이다. 위 방정식은 푸아송 방정식（P이sson equation）이다．
 결론적으로, 제2종 마당 문제는 영역의 경계에서의 조건을 만족시키는 푸아송 방정식을 푸는 것
이다. 스칼라함수 j를 구하게 되면 벡터 마당 F(r）는 (6）으로부터 구할 수 있다．
 전하가 존재하는 영역의 정전기마당（electrostatic field）은 제2종 마당에 속한다．


1.4.3. 제3종 마당

 벡터 마당 F (r）이 영역 내의 모든 점에서


                             V · F (r) = 0
                             V )< F (r) 구드 0                @)

을 만족하면 제3종 마당이다. 벡터 마당의 발산이 0인 사실은 제1종 마당과 같으나, 벡터 마당의 회
                                      제］장 전자기학（E冶ctromagnetism）의 기본이론 31



전이 0이 아니라는 사실은 제1종 마당과 다르다．
 그런데, 벡터의 발산이 0이면 이 벡터는 아래


                           F(r) = \7xA (r)                            (8)


와 같이 다른 벡터의 회전으로 표현할 수 있다. 위 식을 ＠에 대입하면


                         v x (v x A(r)) = C(r)
                     '     v (v ·A) -v2A= C


을 얻는다． 여기에서 C(r）는 0이 아닌 벡터이다．
 헬름홀쯔 정리 (helmholtz theorem)에 의하여 A(r）가 유일한 벡터 마당이 되기 위해서는 A（미
의 발산이 정의되어야 한다. 특히，


                             V. A (r) =O


이라는 조건을 붙이면


                           v2A（미 =-c （미

을 얻는다. 이것은푸아송 벡터방정식이다．
 결론적으로, 제3종 마당 문제는 영역의 경계에서의 조건을 만족시키는 푸아송 벡터방정식을 푸는
것이다． A(r）를 구하게 되면 벡터 마당 F(r）는 ＠로부터 구할 수 있다．


1.4.4. 제4종 마당

 벡터 마당 F (r）이 영역 내의 모든 점에서


                             V · F (r) ；亡 0
                             V x F(r) ；亡 0


을 만족하면 제4종 마당이다．
32 제］부 정전기학（Electro없atics)



 다행스럽게도（?), 제4종 벡터 마당 F(r）은 아래


                                F(r) =G(r) +H(r)         Q)


와 같이 제3종 벡터 마당 G(r）과 제2종 벡터 마당 H (r）의 합으로 쓸 수 있다．
 G(r）은 제3종 마당이므로


                                 G(r) = V X A (r)


이고， H (r）은 제2종 마당이므로


                                            =-
                                      (r)
                                  H
이다. 위의 두 식을 匣）에 대입하면


                             F (r) = V X A (r) - v巾(r)


을 얻는다．
          )          （Eq印0tenlia山ne）과전71咐의백
                  등전위선
H八91                                   '「"’            「「小
                                                         「 小「

2.1, 이론

 정전기학은 쿨롱의 법칙（Coulo岫's law）에 기초를 두고 있다．
 전하（charge）를 나타내는 기호로 q를 사용하자. 아래의 그림




어］ 나타낸 것처럼 쿨롱의 법칙은 R만큼 떨어져 있는 두 점전하（p이nt charges) 사이의 힘을 나타
내는 법칙이다. 단, 전하들은 진공（vacuum) 속에 놓여 있다고 가정한다．
 q'이 q어］ 가하는 힘을 F可如로 표기하자． 즉 q '은 힘의 근원， 즉 샘（source）이다． 또한 q '이 놓여
34 제］부 정전기학（Electrostatics)



있는 위치 尸을 샘의 점이라 하고 q7} 놓여 있는 위치 r를 마당의 점이라고 한다．
 이것들을 이용하면 쿨롱의 법칙은


                                                       1   qq'j工．1J
                                                  =1       H1
                                                  4 兀Co ／코 二




으로 표시된다. 위의 공식에서 알 수 있듯이, 힘의 크기는 전하량의 곱에 비례하고 전하 사이의 거리
의 제곱에 반비례한다．
 비례상수 구－
       －七 어떤 단위계（
                'svstern of unit)'를 사용하느냐에 따라 그 값'이 달라진다.' 국제단
       '   47rE。 니   ' H 니 "   " ' H " H ' V" ' V1 나" " ' 口     ' U   '1
                                                                       누   ' "   "   H   나'   '   匕 1 니 " .'   나니

위계（system of international unit [=SII）를 사용하면


                                      1
                                           =8. 98755x 109m/F



이다． 여기에서 0는


                               E。=8.85x101'2C2/N. m2
                                  = 8.85x 104 '2F/m


이며 , 자유공간의 유전율（perm沚如仕y of free space）이라고 부른다．
 식 a）에서 두 전하의 부호가 같으면 힘은 척력이 되고, 전하의 부호가 다르면 힘은 인력이 된다．
즉 같은 부호의 전하들은 서로 밀어내고, 다른 부호의 전하들은 서로 당긴다．
 지금까지의 논의에서는 전하가 고정되어 있는 정적인 상태를 가정하였으므로, 어떤 역학적인 힘
F q, m이 있어 전하 q가 평형상태에 있다고 해야 한다．


                                          F了Hq+ Fq,m= 0


d에 대해서도 마찬가지이다．
 이제 q 이외에 N개의 점전하가 고정된 위치에 분포되어 있다고 하자. 각 전하를 吼로 표기하자．
이 상황이 아래의 그림
                                            제2장 등전위선（Equ巾아ential Line）과 전기마당의 역선 35




                                                qN



에 나타나 있다. 여기에서 단위벡터（unit vector) 瓦는 吼어］ 대한 q의 상대위치를 나타낸다．
 이들 각각의 전하는 q어］ 힘을 가한다. q어］ 가해지는 힘은


                       F        NZ山    F                                          白
                                                                                              쁘까
                                                             N
                                                                                                   )
                                                                                                   M
                                                             Z
                                                                      4
                                                                      H
                                                                                l
                                                                                1 冗
                                                                                     1
                                                                                                       =
                                                                                                        H


                                                             m
이다. 위 식에서


                           R=          r-       r!   ,                          小m       r2
이다．
 쿨롱의 법칙은 10 14m 정도 떨어져 있는 두 전하에 대해서 성립함이 증명되었다. 거리가 io '4
m보다 줄어들면 핵력（nuclear force）이 전기력 (electric force）보다 강해진다．
 스칼라퍼텐셜（scalar potential) 또는 정전기퍼텐셜（ele야rostatic potent洌）은 아래

                                                         N


                                中（「）        =        듣；          4{       ，且，
36 제］부 정전기학（Electrostatics)



와 같이 정의된다．
 만약, 모든 양이 직각좌표（rectangular coordinates）로 주어지면 위의 식은

                                                      N
                   (r ' == (L) (丁   'I,       夕＼ =   ＼기                   q1
              r5
              ""           ""       "           '    台' 4兀6. \/(！卄耐"+ (y小yy+ (z- 可"


가 된다．
 샘전하가 연속적으로 분포되어 있으면 스칼라퍼텐셜은


                                          ,               1   1    o (r')d丁'
                                        c (r) = 石기VI                   差1'

                                          , /             1   1   a (r')da'
                                        9 (rJ= 47；기,, 方1 '

                                         「卜 4 i7VE。fJ, 츠북므
                                        砂（
가 된다. 여기에서 적분은 샘전하를 포함하는 모든 부피, 곡면 또는 선분에 대한 것이다. 그런데, 전
하가 없는 곳의 전하밀도는 0이므로, 사실상 전 공간에 대하여 적분을 하는 것이라고 말할 수 있다．
 스칼라퍼텐셜이 일정한 곡면을 등전위면（eq岫otential surface）이라고 한다. 아래의 그림


                                                                   I
                                                                  I
                               제2장 등전위선（Eq비p아ent日 Line）과 전기마당의 역선 37



은 仍 > 仍 > &인 경우에 전기마당（electric field）의 방향을 점선으로, 등전위선을 실선으로 나타
낸 것이다. 각 점에서 전기마당의 방향에 접하는 선을 역선（line of force) 또는 전기마당의 역선이
라고 한다. 역선을 그릴 때에는 전기마당의 크기가 큰 곳의 선의 믿도를 높게 한다．
 그러면 단일 점전하 q71 r，어］ 있는 경우에 등전위선이 어떻게 되는지 알아보자. 이 경우에 전위는


                             d (r) = =J=
                                    r소 71t0fl




이다. 아래의 그림




                       \<1
                  0                             R




                        11
은 전위를 점전하에서의 거리의 함수로써 나타낸 것이다. 등전위면은 위의 식을 R어］ 대해서 풀면
얻을 수 있다. 그 결과는


                              R = 그1
                                  47rc04)



이고, 등전위면은 I？이 상수인, 즉 전하를 중심으로 하는 속이 비어 있는 공（sphere）이 된다. 양전
하（pos迂如e 이ectric charge）에 대해서 砂3> 向 > 하인 경우의 등전위면을 나타내어 보면 다음 그
림과 같다．
38 제］부 정전기학（Electrost帥cs)




2.2. 단일 점전하

2.2.1. 이론

 기본적으로 모니터 화면 좌표계에서 화면의 좌상단 모서리가 원점（origin）이다. 이 점에서 우측으
로 이동하면 x 값이 증가하고, 아래로 이동하면 y 값이 증가한다. 즉, 화면 좌표꼐는 우리가 일반적
으로 사용하는 수학적·물리적 좌표계와 다른 면이 있다. 화면 좌표계의 이러한 기본 설정을 바꾸는
code fragment


   CRecf rect;
   pDC->S야M叩Mode (MM工OMETRIC) ;
   GetClientRect (&rect);
   pDC->SetViewportOrg(rect.WidthO/2, rect.Height0/2);


이다．
 SetMapMode 함수는 mapping m이le를 설정하는 함수이다. mapping mode를 어떤 걸로 설정하
느냐에 따라서 , 논리 단위 (logical un迂旬를 장치 단위（device un仕S）로 변환하는 데에 사용되는 척
도 단위 (the unit of measure）와 장치의 x축과 y축의 orientation이 결정된다. GDI는 논리 좌표를
적절한 장치 좌표로 변환하기 위해 mapping mode를 사용한다. SetMapMode 함수의 원형은 다음
과 같다.
                                         제2장 등전위선（Eq미p아enti졔 Line）과 전기마당의 역선 39


   virtual m1lt SetMapMode ( m1lt nMapMode );


nMapMode parameter는 새로운 mapping mode를 지정하는데, 다음의 값들 중에서 어느 하나가
될 수 있다．


(1) MvLHIENGLISH: 각 논리 단위는 0.001 inch로 변환된다. 오른쪽으로 이동하면 x7} 증가하고，
  위로 올라가면 y가 증가한다．
(2) MMJ-IIMETRI(二 각 논리 단위는 0.01 ff111로 변환된다. 오른쪽으로 이동하면 x7} 증가하고, 위로
  올라가면 y가 증가한다．
(3) MItvLLOENGLISH: 각 논리 단위는 0.01 inch로 변환된다. 오른쪽으로 이동하면 x7} 증가하고，
  위로 올라가면 y가 증가한다．
(4) MMmLOMETRI(二 각 논리 단위는 0.1 mm로 변환된다. 오른쪽으로 이동하면 x7} 증가하고, 위로
  올라가면 y가 증가한다．
(5) MM. TWIPS: 각 논리 단위는 점 하나（ap아nt）의 솖로 변환된다· 점 하나는 쿠jinch이므로

  twip 하나는 1去可 油h이다·
(6) MMJSOTROPIC: 논리 단위들은 동일한 비율의 축들（axes）을 가지고 임의의 단위들로 변환된
  다. 즉, x축을 따른 1 단위는 y축을 따른 1 단위와 같다．
(7) M址ANISOTROPIC: 논리 단위들은 임의적인 비율의 축들（axes）을 가지고 임의의 단위들로
  변환된다. mapping mode를 이 mode로 설정하여도 현재의 window나 viewport 설정이 변하지
  않는다．


MMJ-IIENGLISH, MMJIIMETRIC, M｝江LOENGLISH, M｝兀LOMETR兀, 그리고 MMTWIPS
는 inch나 1111처럼 물리적으로 의미 있는 단위들로 그려야 할 때 사용한다. MMJSOTROPIC는
1 : 1 종횡비（aspect ratio）를 얻게 해 주므로, 油age의 정확한 모양을 유지해야 할 때 사용한다．
M加LANISOTROPIC는 x좌표들과 y좌표들을 독립적으로 조정할 수 있도록 한다．
 Set ViewportOrg 함수는 장치 context의 미ewport 원점을 설정한다. 이 함수의 원형으로는 다음
과 같이 2가지가 가능하다．


   virtual CPoint SetViewportOrg( mllt x, m1lt y );
   virtual CPoint SetViewportOrg( POINT point );
40 저Ii부 정전기학乍旭ctrost帥cs)



x parameter와 y parameter는 각각 미ewport의 원점의 x좌표와 y좌표를 지정한다. 이 두 값은 장
치 좌표계（device coordinate system) 의 범위 이내여야 한다．
     (0, 0）에 7nC의 점전하 하나가 있을 경우를 구현하여 보자．
 이 경우에 전위는



               砂（『）＝그귿百＝(8.98755x i09 )x " 二"' " = "" 二12"

가 된다. 전위는 점전하로부터 멀어질수록 작아진다. 전위의 최대값은 /?= 1 일 때 62 .9129이고, 최
소값은 화면의 꼭지점 (1500, -1000）에서


                    砂（:         =    /
                                     ,  62.9129
                                         .         .   ,   -        0000193578
                                    V1500'+ (- b 0uoy
                           )=                                  0.
                     (r)
이다．
 다음으로 최대값에서 시작하여 최소값까지 적당한 전위 간격으로 등전위선을 그린다. 이것은 여
러 가지 값에 대하여 일일이 실행해 보고 적당한 값을 찾아야 할 것이다．
     또한 어떤 전위값에 대해 등전위선을 그릴 때, 이 값을 기준으로 적당한 값을 더해주고 뺀 값의
범위 내에 있는 값들을 모두 하나의 전위값으로 취급해야 한다. 왜냐하면 우리가 등전위선을 그리고
자 하는 컴퓨터 모니터는 자연수로 된 점의 좌표를 가지고 있기 때문이다. 결코 이상적인 등전위선
을 그릴 수는 없는 것이다. 더해 주고 빼주는 값을 구하는 것도 역시 여러 번 시행착오를 거쳐야 할
것이다. 이 값을 너무 크게 잡으면 등전위선이 굵어지게 된다．
     프로그램이 실행되어 최종 결과가 나오기까지 걸린 시간을 측정하기 위해 시간 측정용 code를 추
가하였다. 왜 이런 code를 넣었는지 이해가 가지 않을 것이다. 아직은 프로그램 실행 시간이 별로
걸리지 않기 때문에 그런 생각이 들 것이다. 하지만, 나중에는 프로그램의 실행 시간이 매우 길어지
는 경우가 많이 나온다. 필자는 그런 경우에 과연 얼마만큼의 시간이 걸리는지 알고 싶어 시간 측정
을 위한 code를 추가한 것이다.


2.2.2. Source Code

// 단일 점전하View.cpp : implementation of the CMyView class
II
                                                        제2장 등전위선（Equip아ential Line）과 전기마당의 역선 41



#include 'stdafx.h"
荊nclude ”단일 점전하．h'


荊nclude "단일 점전하Doc.h"
荊nclude “단일 점전하뀌ew.h"


#include <math.h>


double phi [3001] [1901] ;
double potential(double x, double y, double xPrime, double yPrime, double charge);


荊fdef 卞DEBUG
#define new DEBUG_NEW
#undef THIS_FILE
static char THIS_FILE [1 = _FILE_;
#endif


/////////////////I////////////////////////////////////////////I//////////////
// CMyView


IMPLEMENT_DYNCREATE (CMyView, CView)


BEGIN_MESSAGE_MAP (CMyView, CView)
     II { {AFX_MSG_MAP (CMyView)
           II NOTE - the ClassWizard will add and remove mapping macros here.
           II     DO NOT EDIT what you see in these blocks of generated code!
     //} } AFX_MSG_MAP
     II Standard printing commands
     ON_COMMAND (ID_FILE_PRINT, CView::OnFilePrint)
     ON_COMMAND (ID_FILE_PRINT_DIRECT, CView::OnFilePrint)
     ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView::OnFilePrintPrevjew)
END_MESSAGE_MAP 0
42 제］부 정전기학（Electro없atics)



/////////////////////////////////////////////////////////////////////////////
/7 CMyView construction/destruction


CMyView: :CMyView 0
{
     7/ TODO: add construction code here


}

아打View:：兀MyView ()
{
}

BOOL CMyView::PreCreateWindow (CREATESTRUCT& cs)
{
     7/ TODO: Modify the Window class or styles here by modifying
     /7 the CREATESTRUCT cs


     return CView::PreCreateWindow (cs);
}

/////////////////////////////////////////////////////////////////////////////
II CMyView drawing


void CMyView::OnDraw (CDC* pDC)
{
     CMyDoc米 pDoc = GetDocument () ;
     ASSERT_VALID (pDoc) ;


     clock_t start, finish;
     dou바e y, x;
     doub1ie xPrime=0.0, yPrime=0.0, charge=7E-9;
                                       졔2장 등전위선（Equip아ential Line）과 전기마당의 역선 43



double interval, max=62.9129, min=0.0000193578;
double duration;
char str [1001! ;


CRect rect;
pDC->SetMapMode (MM_LOMETRIC);
GetClientRect (&rect);
pDC->SetViewportOrg (rect.Width 0/2, rect.Height 0/2) ;


CPen myPen(PS_SOLID, 5, RGB(0,0,0));
CPen來 p이dPen = pDC小＞SelectObject（邑myPen);
pDC->Rectangle (--1501, -1001, 1501, 901);
pDC->MoveTo ( mnt (xPrime) -20, mnt (yPrime) );
pDC->LineTo ( int (xPrime) +20, int (yPrime) );
pDC->MoveTo ( mnt (xPrime), mnt (yPrime) -20 );
pDC->LineTo ( int (xPrime), int (yPrime) +20 );
pDC->SelectObject (pOldPen);


start := clock 0;


for (y=-l000.O; y<901.0; y++)
     for (x=-1500.0; x<1501.0; x++)
     {
         if ( (x==xPrime)&&(y= =yPrime) )
              break;


         phi [int (x) + 15001 [int (y) + 10001 = potential( x, y, xPrime, yPrime, charge );
    }

for (interval=max; interval>=min; interval- = (max -mmn) /1100.0)
    for (y=-lOOO.O; y<901.O; y++)
          for (x=-1500.0; x<1501.0; x++)
44 제］부 정전기학（Electro없atics)



                 {
                      if ( (x==xPrime) &&(y==yPrime) )
                            break;


                      if ( (phi [m t (x) +1500] [mnt (y) +1000] >interval- (max-min)/150000.0)
                            && (phi [m t (x) +1500] [mnt (y) + 10001<interval+ (max -min)/150000.0) )
                            pDC->SetPixel(int (x), int (y), RGB(255, 0, 0));
                 }

     finish = clockO;


     duration = (double) (finish- start) /CLOCKS_PER..SEC;


     pDC->SetTextAlign (TA_CENTER+TA_TOP);
     sprintf ( s甘, "시간＝%11초", duration );
     pDC->TextOut (0, 1000, str);
}

/II///I/II/II/II/I/I/I/II/I/I/I/II/I///I/II//I/II//I///IIIII/I/I/I/I/I/I/I///
II CMyView printing


BOOL CMyView::OnPreparePrinting (CPrintlnfo* plnfo)
{
     II default preparation
     return DoPreparePrinting (plnfo);
}

void CMyView::OnBegmnPrmnting(CDC半 /*pDC玎, CPrintlnfo木 ／虹汀nfo半／)
{
     II TODO: add extra initialization before printing
                                                        제2장 등전위선（Equip아ential 니ne）과 전기마당의 역선 45



void CMyView::OnEndPrinting (CDC木 小pDC玎, CPrintlnfo水 小plnfo帛／)
{
     7/ TODO: add cleanup after printing
}

///////////////////////////////////////////////////////I/////////////////////
/7 CMyView diagnostics


#ifdef _DEBUG
void CMyView::AssertValidO const
{
     CView::Assert Valid 0;
}

void CMyView::Dump (CDumpContext& dc) const
{
     CView: :Dump (dc) ;
}

CMyDoc* CMyView::GetDocument0 /7 non-debug version is inline
{
     ASSERT (m_pDocument->IsKind0f (RUNTIME_CLASS (CMyDoc)));
     return (CMyDoc*) m_pDocument;
}
#endif I/_DEBUG


/////////////////////////////////////////////////////////////////////////////
/7 CMyView message handlers


double potential( double x, double y, double xPrime, double yPrime, double charge )
{
     double r;
46 제］부 정전기학（Electrostatics)



     r = sqrt ((x-xPrime) *(x-xPrime) + (y-yPrime)*(y-yPrime));
     return 8.98755E9* (charge/r);
1



223 프로그램 실행 결과


             따일（E)   므言L) 보7I(V)   도묩말出）
             1口 才 1            丹 寸
             尸
                                           4   1651.233000i




                                                                  山4小H4小
                                                                           MJM




2.3. 단일 양전하와 단일 음전하

2.3.1. 이론

    -8nC의 음전하와 5n（씌 양전하가 하나씩 있는 경우를 생각하여 보자．
    음전하의 좌표는 (400, 250）이고, 양전하의 좌표는 (740, 320）이다．
이전의 section과는 달리 화면 좌표꼐의 설정을 건드리지 않았다. mapping m아扼의 설정을 바꾸지
않았다는 말이다．
    일단 Mathematica에서 전위함수를 다음과 같이 정의한다．
                                                                제2장 등전위선（Equ巾아ential Line）과 전기마당의 역선 47




                                                                                                             1)
                                           /
                                           1                -8                            5
  phi[   x1   ,   y ]   :'   8.
                                  98755*   1  r
                                           \ V (X 4 400)
                                               V   (x   -
                                                            .          .

                                                               (y 1 250)
                                                    400) {2 ++ (y - 250) <2
                                                                            + /
                                                                                     740) <2+
                                                                             八／ (X 1 740)
                                                                             V   (x-            (y- 320) 2


 두 샘의 점을 제외한 곳에서 전위의 최소값과 최대값을 구하여 보자．
 우선 최소값을 구하기 위해 다음과 갇이 명령


  Min (Min 四ab1e (phi [x, y] , {x, 50, 1000) , {y, 50, 249) ]] r
   Min (Table (phi (x, 250] , {x, 50, 399) ]] , Min (Table[phi[ x, 250] , {x, 401, 1000) ]] ,
   Min[ Table[phi[ x, y] , {x, 50, 1000) , {y, 251, 319) ]) ,
   Min (Table (phi (x              320] , {x, 50, 739) ]] , 工in[Table[phi (x, 320] , {x, 741, 1000) ]] ,
   Min (Table[phi (x, y] , {x, 50, 1000} , {y, 321, 650) ]]]




하고 최대값을 구하기 위해 다음과 같이 명령


  Max[Max (Table (phi (x, y] , {x, 50, 1000) , {y, 50, 249) ]) ,
   Max (Table (phi (x, 250] , {x, 50, 399) ]] , Max (Table[phi (x, 250] r { x, 401, 1000) ]] ,
   Max (Table (phi (x, y] , {x, 50, 1000) , {y, 251, 319) ]] /
   Max (Table (pbi (x, 320] , {x, 50, 739) ]] , Hax (Table[phi (x, 320] r { x, 741, 1000) ]] ,
   Max[Table (phi (x, y] , {x, 50, 1000} , {y, 321, 650} ]]]




한다. 그러면 결과는 각각 -71.7713와 44.7312이다．
 다음으로는 최소값에서 시작하여 최대값까지 적당한 간격으로 등전위선을 그린다. 역시 적당한
값을 찾기 위해 여러 번의 시행착오를 겪을 것이다．
 또한 등전위선을 그리고자 하는 어떤 전위값에 대해 더해주고 빼주는 적당한 값을 구하는 것도 여
러 번 시행착오를 겪을 것이다．
 프로그램을 분석하여 보자．
 위치에 따라 전위값이 양수인 곳도 있고 음수인 곳도 있다. 물론 0인 곳도 있다. 전위값의 부호에
따라 색깔을 달리하여 등전위선을 그려주면 좋을 것이다. 아래의 code fragment


  if ( phi[int (x) -50] [int (y) -50] <0.0 )
         pDC->SetP怏el( int (x) , int (y), RGB(0, 0, 255) );
  이se if ( ph小nt (x) -的］[int (y）寸501>0.0 )
         pDC->SetPixel ( int (x), int (y), RGB(255, 0, 0) );
  이se
 48 제］부 정전7陣1乍lectrostatics)



            pDC->SetPixel ( int (x), int (y), RGB(255, 0, 255) );


 는 전위값의 부호에 따라 다른 색깔의 등전위선을 그린다. 전위값이 음수일 때 등전위선의 색깔은
 파랑이고, 전위값이 양수일 때 등전위선의 색깔은 빨강이다. 전위값이 0일 때의 등전위선의 색깔은
 다른 두 경우의 색깔을 혼합한 것이다．


 2.3.2. Source Code

 // 단일 양전하와 단일 음전하View.cpp : im이ementation of the CMyView class
 //

 #include "stdafx.h"
荊nclude "탄일 양전하와 단일 음전하．h'


荊nclude "단일 양전하와 단일 음전하Doc.h"
荊nclude "단일 양전하와 단일 음전하퍼ew.h"


#include <math.h>


double phi [9511 [6011;
double potential( double x, double y, double xPrime, double yPrime, double charge );


#ifdef _DEBUG
#define new DEBUG_NEW
#undef THIS_FILE
static char THIS놔FILE [] = HF凡且1
#endif


/////////////////////////////////////////////////////////////////////////////
/1 CMyView


IMPLEMENT_DYNCREATE (CMyView, CView)
                                                       제2장 등전위선（Eq비D아ential 니ne）과 전기마당의 역선 49



BEGIN_MESSAGE_MAP(CMyView, CView)
     II { {AFX_MSG_MAP (CMyView)
          II NOTE - the ClassWizard will add and remove mapping macros here,
          II      DO NOT EDIT what you see in these blocks of generated code!
     II) } AFX_MSG_MAP
     II Standard printing commands
     ON_COMMAND (ID_FILE_PRINT, CView::OnFjlePrjnt)
     ON_COMMAND (ID_FILE_PRINT_DIRECT, CView::OnFilePrint)
     ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView::OnFjlePrintPreview)
END_MESSAGE_MAP 0


/////////////////////////////////////////////////////////////////////////////
// CMyView construction/destruction


CMyView::CMyView0
{
     // TODO: add construction code here


}

CMy View:: -CMyView 0
{
}

BOOL CMyView::PreCreate Window (CREATESTRUCT& cs)
{
     /1 TODO: Modify the Window class or styles here by modifying
     // the CREATESTRUCT cs


     return CView::PreCreateWindow (cs);
}
50 제1부 정전기학（Electrostatics)



///////////////////////II////!////////I/II/II/I/////////////I//////////I/////
II CMyView drawing

void CMyView::OnDraw(CDC* pDC)
 {
      CMyDoc* pDoc = GetDocumentO;
      ASSERT_VALID (pDoc);


      clock_t start, finish;
      mnt i;
      double xPrime [21, yPrime [21, charge [21;
      double y, x;
      double interval, min==-71.7713, max=44.7312;
      double duration;
      char str[1001;


      pDC->Rectangle ( 49, 49, 1001, 651 );


      xPrime [01 =400.0; yPrime [01=250.0; charge [01 = -8E-9;
      xPrime [11 =740.0; yPrime [11=320.0; charge [11 =5E-9;


      start = clock 0;


      for (i=0; i<2; i++)
           if ( charge[il>0.0 )
            {
                 pDC->MoveTo ( m t (xPrime [ii) 5, mnt (yPrime [ii) );
                 pDC->LineTo ( mnt (xPrime [ii ) + 5, mnt (yPrime [ii) );
                 pDC->MoveTo ( mnt (xPrime [ii), m t (yPrime [ii ) -5 );
                 pDC->LineTo ( mnt (xPrime [ill), mnt (yPrime [ij) +5 );
           I
           이se
                                        제2장 등전위선（Eq비口아ential Line）과 전기마당의 역선      51




    {
        pDC->MoveTo ( 沁 (xPrime [ii ) -5, mnt (yPrime [ii) );
        pDC->LineTo ( mnt (xPrime [ill ) + 5, mnt (yPrime [ii) );




for (y=50.0; y<651.0; y++)
    for (x=50.0; x<1001.0; x++)
        for (i=0; i<2; i++)
        {
            if ( (x==xPrime [ii) && (y==yPrime [ii! ) )
                 break;


            phi [mnt (x) -50] [mnt (y) -501
                 += potential( x, y, xPrime[i], yPrime[i] , charge[i] );
        }

for (interval=min; interval@max; interval+ = (max-mmn)/i E3)
    for (y=50.0; y<651.O; y++)
        for (x=50.0; x<1001.0; x++)
        {
             for (i=0; i<2; i++)
                 if ( (x==xPrime [ii) &&(y= = yPrime [ii) )
                       break;


            if ( (phi [m t (x) -501 [mnt (y) -501! >interval- (max-min)/1E5)
                 && (phi [mnt (x) -soi [mnt (y) -501<interval+ (max-min)/1E5) )
                 if ( phi [int (x) -501 [int (y) -50] <0.0 )
                       pDC->SetPixel( int (x), int (y), RGB(0, 0, 255) );
                 이se if ( 야ii[int的H印］[int (y）中501>0.0 )
                       pDC->SetPixel( int (x), int (y), RGB(255, 0, 0) );
                 이se
                       pDC->SetPixel( int (x), int (y), RGB(255, 0, 255) );
52 제］부 정전기학（Electro없atics)




                 }

      finish = clockO;


      duration = (double) (finish-start) /CLOCKS_PER.SEC;


      pDC->SetTextAlign (TA_CENTER+TA_TOP);
      sprintf ( s打, "시간＝%lf초", duration );
      pDC->TextOut (512, 20, str);
}

I//I///////////////II//I/II/I//III/I////I/I/II///I//I//////I///////I//I///I//
II CMyView printing


BOOL CMyView::onpreparePrinting (CPrintlnfo* plnfo)
 {
     II default preparation
      return DoPreparePrinting (plnfo);
}

void CMyView::OnBeginPrinting (CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
 {
     1/ TODO: add extra initialization before printing
}

void CMyView::OnEndPrinting (CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
 {
     II TODO: add cleanup after printing
}

I/I///////I//I///////////////////I////////!I//////I////////////I/I///////I//I
II CMyView diagnostics
                                                        제2장 등전위선（Eq叫兀tential Line）과 전기마당의 역선 53



#ifdef DEBUG
void CMyView::AssertValid() const
{
     CView::AssertVal jd 0;
}

void CMyView::Dump (CDumpContext& dc) const
{
     CView::Dump (dc) ;
}

CMyDoc* CMyView::GetDocumerit () /7 non-debug version is inline
{
     ASSERT (m_pDocument- >IsKind0f (RUNTIMEeCLASS (CMyDoc) ));
     return (CMyDoc*) m_pDocument;
}
#endif /LDEBUG


/////////////////////////////////////////////////////////////////////////////
II CMyView message handlers


double potential ( double x, double y, double xPrime, double yPrime, double charge )
{
     double r;
     r = sqrt ( (x-xPrime) *(x-xPrime) + (y-yPrime) *(y-yPrime) );
     return 8.98755E9* (charge/r) ;
}
54 제］부 정전기학（Ele아rostatics)




2.3.3. 프로그램 실행 결과


                 파딜0D 딴집上） 보7H뇌 도묩달언）
                 D 4 나       r   凸 !

                                                            시간＝9乞町札00초




                 춘비




2.4. 두개의 양전하와 단일 음전하

2.4.1. 이론

 2nC, 5nC의 양전하와                        8nC의 음전하가 있는 경우를 구현하여 보자．
 2nC의 양전하의 좌표는 (420, 280), 5nC의 양전하의 좌표는 (810, 220), -8nC의 음전하의
좌표는 (640, 520）이다．
 우선 전위함수를 정의한다．




                      14
   phi[ x_ , y ] : 口


    8.   98755   *
                           (x-
                                       2

                                 420) 2+   (y- 280) 2
                                                        +


                                                            4   (x   -
                                                                              5

                                                                         810) 2 + (y   -   220) 2
                                                                                                    +


                                                                                                        4   (x-
                                                                                                                       -8

                                                                                                                  640) 2+   (y- 520) 2
                                                                                                                                         ]J
                                                제2장 등전위선（Equ巾아ential Line）과 전기마당의 역선 55



     세 샘의 점을 제외한 곳에서 전위의 최소값과 최태값을 구하여 보자．
 우선 최소값을 구하기 위해 다음과 같이 명령


      Min (Min (Table (phi (x, y] , {x, 50, 1000) , {y, 50, 219) ]] ,
       Min (Table[phi (x, 220] , {x, 50, 809} ]] , Mmi1 (Table (phi 江, 220] , {x, 811, 1000) ]] ,
       Min (Table[phi (x, y] , {x, 50, 1000) , {y, 221, 279} ]] r
       Min (Table (phi 江, 280] , { x, 50, 419) ]] , Min 四able (phi (x, 280] , {x, 421, 1000)1] ,
       Min (Table[phi[ x, y] , {x, 50, 1000) , {y, 281, 519} ]] /
       Min口able (phi (x, 520] , {x, 50, 639) ]] , Min (Table (phi (x, 520] , {x, 641, 1000) ]] ,
       Min (Table (phi (x, y] , {x, 50, 1000) , {y, 521, 650} ]]]




하고, 최대값을 구하기 위해 다음과 같이 명령


      Max (Max 口able (phi[ x, y] , {x, 50, 1000) , {y, 50, 219) ]],
       Max (lable (phi (x, 220] , {x, 50, 809) ]] , Ma工 (Table (phi (x, 220] , { x, 811, 1000) ]] ,
       Max[Table (phi (x, y] , {x, 50, 1000) , {y, 221, 279) ]] ,
       Max (Table (phi (x, 280] , {x, 50, 419) ]] , Max (Table (phi (x, 280] , {x, 421, 1000) ]] ,
       Max (Table (phi (x, y] , {x, 50, 1000) , {y, 281, 519) ]] ,
       Max (Table (phi (x, 520] , {x, 50, 639} ]] , Max (Table (phi (x, 520] , {x, 641, 1000) ]] ,
       Max (Table (phi (x, y] , {x, 50, 1000) , {y, 521, 650) ]]]




한다. 그러면 결과는 각각 - 71.7153와 44.7753이다．
     다음으로는 최소값에서 시작하여 최대값까지 적당한 간격으로 등전위선을 그린다. 역시 적당한
값을 찾기 위해 여러 번의 시행착오를 겪을 것이다．
     또한 등전위선을 그리고자 하는 어떤 전위값에 대해 더 해주고 빼주는 적당한 값을 구하는 것도 여
러 번 시행착오를 겪을 것이다．


2.4.2. Source Code

/12개의 양전하와 단일 음전하View.cpp : implementation of the CMy2View class
II

#include n stdafx.h11
荊nclude "2개의 양전하와 단일 음전하．h'


#include "2개의 양전하와 단일 음전하Doc.h"
56 저I1부 정전기학（Electrostatics)



荊nclude " 2개의 양전하와 단일 음전하뮈이V.h"


#include <math.h>


dou바e phi [951] [60比
double potential( double x, double y, double xPrime, double yPrime, double charge );


#ifdef _DEBUG
#define new DEBUG_NEW
#undef THIS_FILE
static char THIS_FILE[] = _FILE_;
#end汀


////////////////////////////////I////////////////////////////////////////////
II CMy2View

IMPLEMENTeDYNCREATE (CMy2View, CView)


BEGIN_MESSAGE_MAP (CMy2View, CView)
     II { {AFX_MSG_MAP (CMy2View)
           II NOTE - the ClassWizard will add and remove mapping macros here.
           II      DO NOT EDIT what you see in these blocks of generated code!
      //} } AFX_MSG_MAP
     II Standard printing commands
      ON_COMMAND (ID_FILE_PRINT, CView::OnFilePrint)
      ON_COMMAND (ID_FILE_PRINT_DIRECT, CView::OnFjlePrjnt)
      ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView::OnFilePrintPreview)
END_MESSAGE_MAP 0


/////////////////////////////////////////////////////////////////////////////
II CMy2View construction/destruction
                                                       제2장 등전위선（Equip아ential Line）과 전기마당의 역선 57



'CMy2View::CMy2View ()
 {
     /7 TODO: add construction code here


}

CMy2View::사CMy2View 0
{
}

BOOL CMy2View: :PreCreateWindow (CREATESTRUCT& cs)
 {
     I! TODO: Modify the Window class or styles here by modifying
     II the CREATESTRUCT cs


     return CView::PreCreateWindow (cs);
}

//////I////I//////////////////I//////////////////////////////////////////////
II CMy2View drawing


void CMy2View::OnDraw (CDC* pDC)
{
     CMy2Doc* pDoc = GetDocument 0;
     ASSERT_VALID (pDoc) ;


     clock_t start, finish;
     mrlt i, number=3;
     double xPrime [3], yPrime [31, charge [31;
     double y, x, interval, min=-71.7153, max=44.7753;
     double duration;
     char str[1001;
58 제］부 정전7陣 (티ectrostatics)



   pDC->Rectangle ( 49, 49, 1001, 651 );


   xPrime [01 = 420.0; yPrime [01 = 280.0; charge [0] =2E-9;
    xPrime [11 =810.0; yPrime [11=220.0; charge [11=5E-9;
    xPrime [21 =640.0; yPrime [21 =520.0; charge [21=-8E-9;


    start = clockO;


    for (i=0; i<number; i++)
       if ( charge [ii >0.0 )
        {
               pDC->MoveTo ( int(xPrime [i] ) 5, int(yPrime [ii) );
               pDC->LineTo ( mnt (xPrime [ii ) +5, mnt (yPrime [ii) );
               pDC- >MoveTo ( mnt (xPrime [ii), m t (yPrime [ii) -5 );
               pDC->LineTo ( mnt (xPrime [ii), m t (yPrime [ii ) +5 );
        }
        else
        {
               pDC->MoveTo ( 沁 (xPrime [i] ) 5, mnt (yPrime [ii) );
               pDC->LineTo ( mnt (xPrime [ii ) + 5, mnt (yPrime [ii) );
        }

    for (y=50.O; y<651.O; y++)
        for (x=50.0; x<1001.0; x++)
               for (i=0; i<number; j++)
               {
                   if ( (x==xPrime [ii) &&(y==yPrime [i]) )
                        break;


                   phi [int (x) -501 [int (y) -50]
                        += potential( x, y, xPrime [ii, yPrime [ii, charge [ii );
                                                       제2장 등전위선（Equipo旭nti히 Line）과 전기마당의 역선 59



      for (interval=min; interval<=max; interval+ = (max -mmn) /2E3)
           for (y=50.0; y<651.0; y++)
                 for (x=50.0; x<1001.0; x++)
                 {
                       for (i=0; i<number; i++)
                            if ( (x==xPrime [ii) &&(y==yPrime [ii) )
                                  break;


                      if ( (phi [m t (x) -501 [mnt (y) -501>interval- (max-mmn)I2E5)
                            && (phi [mnt (x) -501 [m t (y) -501<interval+ (max-mm ) /2E5) )
                            if ( phi[int (x) -501 [int (y) -50] <0.0 )
                                  pDC->SetPixel( int (x), int (y), RGB(0, 0, 255) );
                            else if ( phi[int (x) -501 [int (y) -501>0.0 )
                                  pDC->SetPixel( int (x), int (y), RGB(255, 0, 0) );
                            이se
                                  pDC->SetPixel( int (x) , int (y), RGB(255, 0, 255) );
                 }

      finish = clock();


      duration = (double) (finish-start)/CLOCKSePERSEC;


     pDC->SetTextAlign (TA_CENTER+TA_TOP);
      sprintf ( str, "A]간=%lf초' , duration );
     pDC->TextOut (512, 20, str);
}

I/II///II/////I/I//I//I/I//I/II//I//I//I/I/I/////III///////!//I/I/II/I/I/IIII
II CMy2View printing


BOOL CMy2View::OnPreparePrinting (CPrintlnfo* plnfo)
{
60 和부 정전기학乍旭ciro없atics)



     II default preparation
      return DoPreparePrinting (plnfo);
}

void CMy2View::OnBeginprinting (CDC米 八pDC玎, CPrintlnfo米 ／사汀nfo永／)
 {
     II TODO: add extra initialization before printing
}

void CMy2View::OnEndPrinting (CDC水 八pDC玎, CPrintlnfo永 /*이nfo半／)
 {
     II TODO: add cleanup after printing
}

II///I/I///I//IIIIII//////I/////////////////////I/IIII/I/I///I/I/III/II//II/I
II CMy2View diagnostics

#ifdef J1EBUG
void CMy2View::AssertValid 0 const
 {
      CView::AssertValid0;
}

void CMy2View::Dump (CDumpContext& dc) const
 {
      CView::Dump (dc);
}

CMy2Doc* CMy2View::GetDocumentO II non-debug version is inline
{
      ASSERT (mpDocument->IsKindOf (RUNTIME_CLASS (CMy2Doc)));
      return (CMy2Doc*) m_pDocument;
                                                        제2장 등전위선（Equi）아entia1 Line）과 전기마당의 역선 61



}
#endif I/_DEBUG


////I//////////II/////////////////I/////////I///////I///I/I////I/I/I/IIIIII/I
II CMy2View message handlers


double potential ( double x, double y, double xPrime, double yPrime, double charge )
{
     double r;
     r = sqrt ((x-xPrime) *(x-xPrime) + (y-yPrime) *(y-yPrime));
     return 8.98755E9* (charge/r);
}

243 프로그램 실행 결과


                  i｝일（E)   편집止） 보7Hy) 도묩말언）
                      D 4 日    \1 旨斗. 凸 寸
                 r느




                                                       시 간＝240.416000초
62 졔j부 정전기학（Electros怡tics)




2.5. 두개의 양전하와 두개의 음전하

2.5.1. 이론

 이전의 section을 마쳤는가2 그렇다면, 한개의 양전하와 두개의 음전하가 있는 경우를 프로그램
으로 구현하여 보아라. 이전의 section의 프로그램을 조금만 손보면 된다．
 그 다음으로는, 세개의 점전하가 있는데 모두 양전하들이거나 음전하들인 경우를 프로그램으로
구현하여 보아라．
 이 section에서는 전하의 개수가 세개에서 그보다 한개 늘어난 네개인 경우를 프로그램으로 구현
하여 보자．
 5nC, 12n（씌 양전하와 -6nC, -8nC의 음전하가 있다. 5n（겨 양전하의 좌표는 (330, 300),
12n（겨 양전하의 좌표는 (700, 300) , 小6nC의 음전하의 좌표는 (330, 400), -8nC의 음전하의
좌표는 (700, 400）이다．
 우선 전위함수를 정의한다．


   phi [x_ , y_ ]
                       (
                       I                      5                         12                            -6
    S   '
            98755*     1/ r     330) + (y
                       t V (X = 330) 42+
                           '\
                                (x-      (y-H 300)
                                              300) 12
                                              .       +. r
                                                           4   700) 12 +
                                                        V (X m 700)
                                                               (x   -
                                                                        .


                                                                       + (y  -
                                                                                  .


                                                                              300) 1
                                                                         (y m 300) 2
                                                                                     +
                                                                                       4 /            .


                                                                                                             400) 24
                                                                                                        (y m 400)
                                                                                                      + (y
                                                                                              330) 工2 +
                                                                                       V （工 m 330)
                                                                                             (x   -        -
                                                                                                                     +




             4   (x-
                                      -
                       700) 2+ (y- 400) 2
                                          8
                                                  1)
좀 길긴 한데, 조금도 어렵지 않을 것이다．
 전위의 최소값을 구하기 위해 아래


   Min[Hin (Table (phi[ x, y] , {x, 50, 1000} , {y, 50, 299} ]J,
    Hin (Table (phi[ x, 300] , {x, 50, 329} ]] , Min[ Table[phi (x, 300] , {x, 331, 699} ]] ,
    Min (Tab1e (phi (x, 300] , {x, 701, 1000} ]] /
    Min (Table (phi (x, y] , {x, 50, 1000} , {y, 301, 399} ]] ,
    Hin[ Table (phi[ x, 400] , {x, 50, 329} ]J , Min[ Tab1 (phi[ x, 400] , {x, 331, 699} ]] ,
    Min (Table (phi (x, 400] , {x, 701, 1000} ]] /
    Min[ Table[phi (x, yj , {x, 50, 1000} , {y, 401, 650} ]]]
                                                제2장 등전위선（Equ四아ential Line）과 전기마당의 역선 63


 와 같이 명령하고, 전위의 최대값을 구하기 위해 아래


      Max (Max (Table[phi (x, y] , {x, 50, 1000) , {y, 50, 299) ]] ,
       Max (Table (phi[ x, 300] , {x, 50, 329) ]] , Max (Table[phi (x, 300] , {x, 331,
                                                                                       699) ]] ,
       Max (Table (phi (x, 300] , {x, 701, 1000) ]] ,
       Max (Table (phi (兀 y] , {x, 50, 1000) , {y, 301, 399) ]] ,
       Max[Table[phi (x, 400] , {x, 50, 329) ]] , Max (Table[phi (x, 400] , {x, 331,
                                                                                     699) ]] r
       Max (Table (phi (x, 400] , {x, 701, 1000)1] ,
       Max[Table (phi[ x, y] , {x, 50, 1000) , {y, 401, 650) ]]]




와 같이 명령한다. 그러면 결과는 각각                       70.8611와 107.12이다．
     그 다음에는 어떻게 해야 할지 알 수 있으리라 믿는다. 필자가 더 이상 말을 하치 않아도 어떻게
해야 할 지 알 수 있을 것이다．


2.5.2. Source Code

II 2개의 양전하와 2개의 음전하뀌텨V.cpp : implementation of the （玉4y22View class
II

#include ustdafX.h!1
荊nclude "2개의 양전하와 2개의 음전하．h'


荊nclude "2개의 양전하와 2개의 음전하Doc.h"
荊nclude "2개의 양전하와 2개의 음전하View.h"


#include <math.h>


double phi [9511 [601] ;
double potential( double x, double y, double xPrime, double yPrime, double charge );


#ifdef _DEBUG
#define new DEBUGNEW
#undef THIS_FILE
static char THIS_FILE[] = _FILE_;
64 저Ii부 정전기학乍lectrostatics)



#endif


/////////////////////////////////////////////////////////////////////////////
II CMy22View

IMPLEMENT_DYNCREATE (CMy22View, CView)


BEGIN_MESSAGE_MAP (CMy22View, CView)
     II { {AFX_MSG_MAP (CMy22View)
           II NOTE - the ClassWizard will add and remove mapping macros here.
           II     DO NOT EDIT what you see in these blocks of generated code!
      //} } AFX_MSG_MAP
     II Standard printing commands
      ON_COMMAND (ID_FILE_PRINT, CView::OnFilePrint)
      ON_COMMAND (ID_FILE_PRINT_DIRECT, CView::OnFilePrint)
      ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView::OnFilePrintPreview)
END_MESSAGE_MAP 0


/////////////////////////////////////////////////////////////////////////////
II CMy22View construction/destruction


CMy22View::CMy22View 0
{
      // TODO: add construction code here


}

CMy22View::NCMy22View ()
{
}

BOOL CMy22View::PreCreateWindow (CREATESTRUCT& cs)
                                                       제2장 등전위선（Equ巾아entia1 Line）과 전기마당의 역선 65



{
     II TODO: Modify the Window class or styles here by modifying
     1/ the CREATESTRUCT cs


     return CView::preCreateWindow (cs);
}

//I//!///////////I//////////////I////////////////I/!/!III/I///I//////////////
II CMy22 View drawing


void CMy22View::OnDraw (CDC* pDC)
{
     CMy22Doc* pDoc = GetDocument 0;
     ASSERT_VALID (pDoc) ;


     clock_t start, finish;
     m1lt i, number=4;
     double xPrime [4], yPrime [4] , charge [41;
     double y, x, interval, min==-70.8611, max==107.12;
     double duration;
     char str[100] ;


     pDC->Rectangle ( 49, 49, 1001, 651 );


     xPrime [01 =330.0; yPrime [0] =300.0; charge [0] =5E-9;
     xPrime[1] =700.0; yPrime[11 = 300.0; charge [1] =12E-9;
     xPrime [2] =330.0; yPrime [2] =400.0; charge [21 = -6E-9;
     xPrime [3] = 700.0; yPrime [3] =400.0; charge [3] = -8E-9;


     start = clock 0;


     for (i=0; i<number; i++)
66 저Ii부 정전기학（Electrostatics)



        if ( charge [ii >0.0 )
        {
              pDC ->MoveTo ( m t (xPrime [ii) -5, mnt (yPrime [ii) );
              pDC->LineTo ( mnt (xPrime [ii) + 5, mnt (yPrime [ii) );
              pDC->MoveTo ( mnt (xPrime [ii), m t (yPrime [ii) -5 );
              pDC->LineTo ( mnt (xPrime [ii), mnt (yPrime [ii ) +5 );
       }
       else
        {
              pDC->MoveTo ( m t (xPrime [i] ) -5, mnt (yPrime [ii) );
              pDC ->LineTo ( mnt (xPrime {i] ) + 5, mnt (yPrime [ii) );



   for (y=50.0; y<651.0; y++)
       for (x=50.0; x<1001.0; x++)
              for (i=0; i<number; j++)
              {
                  if ( (x==xPrime[i] )&&(y==yPrime[ij) )
                       break;


                  phi [int (x) -501 [int (y) -50]
                       += potential( x, y, xPrime[i], yPrime[i], charge[i] );
            }

   for (interval=min; interval<=max; interval+ = (max -mmn) /4E3)
       for (y=50.0; y<651.O; y++)
            for (x=50.0; x<1001.0; x++)
            {
                  for (i 0; i<number; i++)
                      if ( (x==xPrime [ii) &&(y==yPrime [i] ) )
                           break;
                                                         제2장 등전위선（Eq미p아enti계 니ne）과 전기마당의 역선 67



                       if ( (phi [mlt (x) -50] [mnt (y) -501>interval- (max-min) /3E5)
                             && (phi [mnt (x) -50] [mnt (y) -50] <interval+ (max-min) /3E5) )
                             if ( phi [int(x) -501 [int(y) -50] <0.0 )
                                   pDC->SetPixel( int (x), int (y), RGB(0, 0, 255) );
                             else if ( phi[int (x) -50] [int (y) -50]>0.0 )
                                   pDC->SetPixel( int (x), int (y), RGB(255, 0, 0) );
                             이se
                                   pDC中>SetPixel( int (x), int (y), RGB(255, 0, 255) );
                 }

      finish = clock 0;


      duration = (double) (finish- start) /CLOCKS--PER. SEC;


     pDC->SetTextAlign (TA_CENTER+TATOP);
      sprintf( str, "시간＝%lf초", duration );
     pDC->TextOut (512, 20, str);
}

////////7////////////////////////////////////////////////////////////////////
II CMy22View printing


BOOL CMy22View::onPreparePrinting (CPrintlnfo* plnfo)
{
    II default preparation
     return DoPreparePrinting (plnfo);
}

void CMy22View::OnBeginPrinting (CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
    II TODO: add extra initialization before printing
}
68 제］부 정전기학（Eectrost計兀s)



void CMy22View::OnEndPrinting (CDC水 ／枉）DC町, CPrintlnfo永 八pInfo米／)
{
      /1 TODO: add cleanup after printing
}

II/IIIIIII/I/I/II/I//I//I//I//II///I/I/III/II/IIIII/I///I/I//I/I/I/I/I/////I/
II CMy22View diagnostics


#ifdef JDEBUG
void CMy22View::AssertValid 0 const
{
      CView::AssertValid 0;
}

void CMy22View::Dump (CDumpContext& dc) const
{
      CView::Dump (dc);
}

CMy22Doc* CMy22View::GetDocument0 II non-debug version is inline
{
      ASSERT (m.epDocument - >IsKindOf (RUNTIME_CLASS (CMy2 2Doc)));
      return (CMy22Doc*) nLpDocument;
}
#endif I/_DEBUG


II//I/////II/II/III/I///////I/I/III///II//I//////////I///I/I/I//II/II/III////
II CMy22View message handlers

double potential ( double x, double y, double xPrime, double yPrime, double charge )
 {
      double r;
                                               제2장 등전위선（Equip아ential Line）과 전기마당의 역선 69


     r = sqrt ( (x-xPrime) * (x-xPrime) + (y-yPrime) * (y-yPrime));
     return 8.98755E9* (chargelr);
}


253 프로그램 실행 켤과


             2. 7月의 맘전針엌 ？月의 믐 선針       川복얹믐
             파딤（LJ   판집止） 보기（多     도뇽맘咀）
              D 呼日         寸   凸    寸


                                               시 칸.792.5201M초




2.6. 균일한 구면 전하분포（Uni化rm Spherical Charge Distribution)

2.6.1. 이론

    지금까지는 한 7뀨 이상의 점전하가 있는 경우를 프로그램으로 구현하였다. 이번에는 점전하가 무
한히 많이 있는 경우를 구현하여 볼 것이다．
    총전하 Q를 가진 균일한 구면 전하분포가 있는 경우를 구현하여 보자．
    샘의 점을 구면좌표（spherical coordinates）로 표시하여 적분하는 것이 편리하다．
    전하분포가 만드는 구면의 반지름은 a이다. 마당의 점이 名축 위에 있으면 r＝虎이고 r' = rf '이
므로 R= 虎- rP이 된다．
70 제］부 정전기학（Electrostatics)



  아래의 그림




은 전하분포의     寺을
                 나타낸 것이다·
 아래의 그림




은 구면 전하분포를 다른 각도에서 본 모습을 나타낸다. 이 그림은 z축, r ', R을 포함하는 평면을 보
여준다．
                                               제2장 등전위선（Equip아ential 니ne）과 전기마당의 역선         71



  그림으로부터



                                 R2 = 22 + 구 -2名r七Os伊


임을 알 수 있다. 따라서



                 느슬，/,"" /," /," /，「
                                   ．‘巴‘臂
                                       ，少
                                        ，,*
로 된다．
  d砂 '에 대한 적분은 즉시 계산할 수 있으며 그 값은 2ii-이다. 따라서，



                          砂＝半J     ' / " .寸sin9'd尸d9'd砂'
                            乙to Jo
                                                v'z'+ r"- 2zr'cosO'


 dO '에 대해 적분하기 위해 새로운 변수 ／上= cosO‘를 도입한다. 그러면 d尸＝中 帥l9닢伊이므로




                  아붊／," /"可', 구亡毛＝                                                    (l)
 /i에 대한 적분은 적분표로부터


                              re
                                                                                      (2)
                  \/z2+
                                     小   2zr
                               zr'              ,=   去
                                                         （/
                                                              ＋『
                                                                   'H 卜   「 ')




 다음의 두 경우를 생각해야 한다．


(1) 공의 밖(z> a): 편의상 z를 양으로 가정하면 7J드 a이므로 z> 尸이 되어 (2）은



                            -1 [(z+
                               [(:+「9
                                    r- (z-
                                       (:m r:9] =-2
72 제］부 정전7陣 (Electrostatics)



가 된다. 따라서 d）은



                                               吃                   ／끄工3                                Q
                                                                   3E。z                          47rf。z
                                                      =




(2) 공의 안(z < 口）: 尸은 z보다 크거나 작을 수 있다. Z < 尸＜ a 일 때에 ＠는



                                         윽，[(:+ m+ (：小「,)] = 윽，

이 되고, 尸＜ z< a 일 때에 (2）는



                                             -1
                                              Zr' [(z+
                                                  [(:+ r9
                                                       r- (2
                                                          (z- r:9]J = -2Z

7} 된다. 따라서 , 공 안의 퍼텐셜은



                                                                                                               Q 叱
                                                                                                                              귀
                                        丑d            2
                                                      1                                   끄        d                              +=
                                                                                                           2
                                                                          n
                                    '
                                         r   r                                             r           r                 nd

                                                      2
                   므I/
                         260 L J0
                                                                          ／人
                                                                                                                     1
                                                                                                           二
                                                                          尸
                                                                                                                     \
 ＠과 위 식은      作쿄
                              구면 위에서 동일한                                                  47rf         a
                                                                                                           帥진다·
 지금까지 적분을 쉽게 하려고 마당의 점을 z축 위로 선택하였는데, 지금까지의 결과를 임의의 위
치로 일반화시킬 수 있다. 우리는 공의 중심에서의 거리 r로 지금까지의 결과를 쓸 수 있다. 그러므
로, 공의 안과 밖에서의 퍼텐셜에 대한 일반적 표현식은



                                                 中*       ＝        三모，         니3+                         }
                                                              吃＝                     ,   ,Q      ,,,
                                                          제2장 등전위선（Equip아ential Line）과 전기마당의 역선 73



 위의 두 식에서 r이 일정하면 砂 도 일정함을 알 수 있다. 즉, 등전위면은 공의 중심을 중심으로 하
는 동심구가 된다．
 프로그램으로 구현하여 보자．
 이번에는 mapping mode를 바꾸어 볼 것이다. 전하분포의 중심은 원점이고 반지름은 500이며 전
하량은 521nC이다．
 우선 전위함수를 다음과 같이 두 가지 경우로 나누어 정의한다．


      r (x_, y그 :=.I x2 +y2
                                              521
      phi ［工-,y그 : .8. 98755*                        /; r ［毛 y] 之 500
                                           r ［工ry]

                                          521         r江， y] 2
      phi (x_   ,
                         ] :.
                                     98755* 3。
                                             。         250000
                                8.
                    y_
                                          -      *
      phi[:．工］：·8.98755，릎능 (3 『,［
                               ，’볍,' ]I;【［毛！]45的
     공의 중심에서 전위는 최대가 되며 그 값을 구하기 위해 다음과 같이 명령


      phi[ 0, 0]



한다. 한편, 화면의 꼭지점 (-1500, 크000）이나 (1500, -1000）에서 전위는 최소가 되며 그 값
을 구하기 위해 다음과 같이 명령


      phi (1500, -1000]



한다. 최대값과 최소값을 구하기 위한 명령문에 대한 결과는 각각 14.0475와 2.59739이다．


2.6.2. Source Code

// 균일한 구면 전하분포뀌ew.cpp : implementation of the CMyView class
II

#include 'stdafx.h"
荊nclude "균일한 구면 전하분포.h
74 제］부 정전기학（帥ctrost帥cs)



荊nclude "균일한 구면 전하분포Doc.h"
荊nclude "균일한 구면 전하분포피ew.h"


#include <math.h>


dou바e 아ii [3001] [1901] ;


double potentialln( double radius, double charge, double r );
double potentialOut ( double r, double charge );


#ifdef _DEBUG
#define new DEBUG_NEW
#undef THIS_FILE
static char THIS_FILE {] = _FILE_;
#endif


I//////I/////I/I////////I/////////////////////II/////II////I/!/////////!//I/I
II CMyView

IMPLEMENT_DYNCREATE (CMyView, CView)


BEGIN_MESSAGE_MAP (CMyView, CView)
     II { {AFX_MSG_MAP (CMyView)
           II NOTE 1 the ClassWizard will add and remove mapping macros here.
           II      DO NOT EDIT what you see in these blocks of generated code!
      //} } AFX_MSG_MAP
     II Standard printing commands
      ON_COMMAND (ID_FILE_PRINT, CView::OnFilePrint)
      ON_COMMAND (ID_FILE_PRINT_DIRECT, CView::OnFilePrint)
      ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView::OnFilePrintPreview)
END_MESSAGE_MAP 0
                                                        제2장 등전위선（Equ巾아ential Line）과 전기마당의 역선 75



/////////////I///////////I/I////////////////I///////I/////////II//////I/I/I//
II CMyView construction/destruction


CMyView::CMy View 0
{
     /1 TODO: add construction code here


}

CMyView::사CMyView0
{
}

BOOL CMyView::PreCreateWindow (CREATESTRUCT& cs)
{
     II TODO: Modify the Window class or styles here by modifying
     II the CREATESTRUCT cs


     return CView::PreCreateWindow (cs);
}

/////////////////////////////////////////////////////////////////////////////
II CMyView drawing


void CMyView::onDraw (CDC* pDC)
{
     CMyDoc* pDoc = GetDocument0;
     ASSERT_VALID (pDoc);


     clockt start, finish;
     double xCenter=0.0, yCenter=0.0, radius=500.0, charge=521E-9;
     double y, x, r, interval, max=14.0475, min=2.59739;
76 제］부 정전7陣K日ectrostatics)



   double duration;
   char str{100] ;


   CRect rect;
   pDC卞冷出巾小lode (MM_LOMETRIC) ;
   GetClientRect (&rect);
   pDC - >SetViewportOrg (rect Width O/2, rect.Height O/2);


   CPen myPen (PS_SOLID, 5, RGB (0,0,0));
   CPen* pO넌Pen = pDC->SelectObject (&myPen);
   pDC->Rectangle(-1501, -1001, 1501, 901);
   pDC->SelectObject (pOldPen);
   CBrush Distribution (RGB (0,0,0));
   CBrush* pBrush;
   pBrush = pDC->SelectObject (&Distribution) ;
   pDC->Ellipse (- 500, 500, 500, -500);
   pDC->SelectObject (pBrush);


   start = clock 0;


   for (y=-l000.0; y<901.0; y++)
       for (x=-1500.0; x<1501.0; x++)
       {
           r = sqrt ( (x-xCenter) * (x-xCenter) + (y-yCenter) * (y-yCenter));


           if ( r<500.0 )
                 phi {int (x) +1500] [int (y) + 10001 = potentialln( radius, charge, r );
           이se
                 phi [mnt (x) +1500] [mnt (y) + 1000] = potentialOut ( r, charge );
       }

   for (interval=max; interval>=min; interval-= (max-min)/30.0)
                                                        제2장 등전위선（Equ巾아enti히 Line）과 전기마당의 역선 77


           for (y＝크000.0; y<901.0; y++)
                 for (x=-1500.0; x<1501.0; x++)
                      if ( (phi [m t (x) +1500] [mnt (y) + 10001>interval- (max-mmn) /4000.0)
                            && (phi [m t (x) + 15001 [mnt (y) + 10001<interval+ (max-min)/4000.0) )
                            pDC->SetPixel(int (x), int (y), RGB(255, 0, 0));


     finish = clockO;


     duration = (double) (finish - start) /CLOCKS_PER_SEC;


     pDC- >SetTextAlign (TA_CENTER+TA_TOP);
     sprintf ( str, "시간＝%lf초", （加ration );
     pDC->TextOut (0, 1000, str);
}

/////////////////////////////////////////////////////////////////////////////
II CMyView printing


BOOL CMyView::OnPreparePrinting (CPrintlnfo* plnfo)
{
     II default preparation
     return DoPreparePrinting (plnfo);
}

void CMyView::onBeginPrinting (CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     1/ TODO: add extra initialization before printing
}

void CMyView::OnEndPrinting (CDC* /*pDC*/, CPrintlnfo * /*plnfo水/)
{
     // TODO: add cleanup after printing
78 제］부 정전기학（Electrostatics)



}

////////////////////////////////////////////////////////////////I/I//////////
II CMyView diagnostics


#ifdef _DEBUG
void CMyView::AssertValid0 const
{
     CView::AssertValid 0;
}

void CMyView::Dump (CDumpContext& dc) const
{
     CView::Dump (dc);
}

CMyDoc米 CMyView::GetDocument0 1/ non-debug version is inline
{
     ASSERT (mpDocument->IsKind0f (RUNTIME_CLASS (CMyDoc)));
     return (CMyDoc*) nLpDocument;
}
#endif 力_DEBUG


///IIII/III//I///IIII/III/I/I///II///I/I/I/I//I/II/I//I//I//I///I///IIII/II//
II CMyView message handlers


double potentialln( double radius, double charge, double r )
{
     return 8.98755E9* (charge/(2.O*radius)) * (3.0- (r*r) / (radius*radius));



double potentialOut ( double r, double charge )
                                      제2장 등전위선（Equ巾아enti히 니ne）과 전기마당의 역선 79



{
    return 8.98755E9*
    retUrn   98755E9串（Char
                      (charge/r);
}

263 프로그램 실행 결과


            파말（E) 딴집（L) 보기（Y) 도욤맘出L
            D 哮日     노 融 4   !

                                      1I=4S.8920t01
                    전 廳극印毗씨加州：

3.1, 스칼라퍼텐셜의 여러겹극 전개

 어떤 부피 V，어］ N개의 점전하 ql, q2, q3, ···, qN 2, qN- 1 , 鈿7} 있다. 좌표계의 원점은 V'의 안
이나 근처로 선택한다. 전하들의 위치벡터（position vector）는 r1, r2, r3, ···， rN山 rN小 FN이다．
 위치벡터가 r인 마당의 점 P에서의 전위를 구해 보자．
 원점에서 r만큼 떨어진 곳에서 r의 방향을 가진 전위는


                                砂（r) = Z 4irE01引               qi
                                                                                          (l)
이다. 여기에서 /Zi= 1r- rI 이다. 乙와 r 사이의 각도를 Iii라 하면，


                                =   \   /r2+            ri2-        2rrcos0r
이므로 d）은

                                                                               吼
                     d(r)   =
                                                       \/r2+
                                                                                           (2)
                                               47rE。
                                                                          r2 H 2rrcosO,
82 제］부 정전기학（Electrostatics)



이 된다. 현재 상태에서 전하분포에 대하여 더 이상의 정보가 없으면 위 식에서 한 걸음도 더 나아
갈 수 없다．

 점 I汐｝ I戶에서 매우 멀리 떨어져 있다고 가정하자. 즉, 임의의 z어］ 대하여 r> r，이다. 그러면 그

는 항상 1보다 작으므로


                              1                        l1                           1
                   iJr2 + rj2 - 2rr1cos01              r         /     -          M2\+
                                                                                                  (3)
                                                                il-   2그 cosO.1 + 쓱   I.'
                                                                \                     )
                                                                I      an         - 石 1
                                                                        1         I




을 급수전개 시킬 수 있다．
 0에 가까운 t어］ 대하여 성립하는 다음의 거듭제곱 급수전개（power series expansion)

                                                            =                1} =
                                                                                              +
                                       l           3
                                  1         t + 二 t 2 1 걷＝. t 3 + n：娑m t4 Hn.           H 1




                                       可
                                                   百    lb       ' l28



을 이용하여 G）의 제곱근을 급수전캐 시켜 보자．
 과정은 생략하겠는데 정리한 후 (2）에 대입하면

                               l
                   ,. .       l1      N1
                                      :-'      ,       l1       v-'
                                                                 N
                   )\r) = 石구台 7'十石；;；唯寸 q2rcos r7
                                      끄       , m,2                                                     )
                                                                                                  侄）
                          + A_ .3＞그 뽁二（3cos201- 1) +...                d11



                            寸/Ito7    i= 1     1d




을 얻는다. 위의 식을 전위의 여러겹극 전개（multipole expansion）라고 한다. 위 식에서 첫째항을
홀극（跏nopole）항, 둘째항을 쌍극자m加이이항, 셋째항을 사중극（quadrupole）항이라고 한다．
 마당의 점이 전하분포에서 멀어질수록 전위의 여러겹극 전개에서 고차항의 중요성은 줄어든다．
 편의상 위의 식을


                          砂（미 = 加（미 + 加仕）+ 札（r) +...


로 쓰자．
                                                               제3장 전기다중극（E旭아nc M미ti）이e)   83




3.2. 홀극

3.2.1. 이론

 마당의 총전하량을 Q라고 하면 4）에서 홀극항은



                                  知（『） = 4글,:

가 된다．
 Q를 전하분포의 홀극모멘트（monopole m이ient)라고 부른다. 만약 전하가 이산적으로 분포되어
있는 것이 아니라 연속적으로 분포되어 있으면



                                     /,,   P
                                               「 ')
                                               （      d7   '
                             Q=
이 된다. 여기에서 적분은 샘전하가 분포된 부피 VI어］ 대하여 계산한다．



3.3. 쌍극자마당（Dip이e 디이d)

3.3.1. 이론

 匹）에서 cosoi는



                 cosO= "二니計 'CLxi+ lYy+ lZz                                               (5)
이다． 여기에서 /x, ill, lz는 점 P의 위치벡터 r의 방향코사인（direction cosine）이고, xi, yi, 릭는 전
하 吼의 위치를 나타내는 직각좌표 성분이다．
84 제］부 정전기학（Electrostatics)



 위 식을 ＠의 쌍극자항에 대입하면


                  N
                  Zm                    N
                    吼rcosOi = Z                吼（蜘‘＋切i+ 1z1)
                                                                                            N
                                                                                            Zm
                                       i= 1

                                                                       N
                                                                       Z山
                                        f N                      (
                                                                                    \
                                                                                                 ＼기如U
                               +
                          /
                                                                             肌
                                   c Zq2;                                                          吼
                                                                                    1
                          1
                          1
                                                                             吼      1
                                                                                        L
                               =                                                        乙
                                                                 11\
                          1
                                                   N
                                                   Z勻
                          \
                          {
                                        \ 1=   l        .
                                                                                    /




                               =   r    1
                                                       《山］



을 얻을 수 있다. 마지막 식에서 괄호 안은 마당의 점의 위치와는 무관하고, 단지 전하분포의 성질만
을 나타낸다. 이것을 전하분포의 쌍극자모멘트（d如아em이Tient)라고 정의하고, 기호로는 p을 쓴다．
즈




                                                   m        N
                                                            Z向                                          (6)
로 정의하면


                        N
                        Zm         m
                                               =r. p= 切卄 뇨) + lJ乙



으로 쓸 수 있다. 위의 식을 匹）에 대입하면 쌍극자항은


                               r / \                I그 1 r      I그 .r
                              C)n[ l= j =           -      n = 411
                              r 1/ \    /          d mm1n -乙           /4-口＝戶 m1J
                                                   寸It t01             寸lit0- ,




이 퇸다. 위의 식은 마당의 점의 위치와 전하분포의 형태에 의존하는 두 양의 스칼라곱의 형태를 하
고 있다．
 전하가 이산적으로 분포되어 있치 않고 연속적으로 분포되어 있으면 6）의 합은 부피 1戶에 대한
적분으로 바뀐다．
                                                                     제3장 전2江r중극（日ectric M미tipole) 85




                         p=           f,       p    (r   ') r 'dT'




 ＠은 쌍극자퍼텐셜（dipole potent洌）에 태한 식이고 총전하 Q가 Q= o이면 주된 전위가 된다．
우리는 처음에 마당의 점이 전하분포에서 멀리 떨어져 있다고 가정하였으나, 공간의 모든 점에서 이
러한 砂／77} 성립한다고 하면 편리할 것이다. 이런 전기마당을 쌍극자마당이라고 한다. Q= o이 되
는 가장 간단한 경우는 크기가 같고 부호가 반태인 두 점전하에 의해 생길 수 있다．
 특히 , 크기가 같고 부호가 반대인 두 점전하의 분리거리가 거의 0인 경우를 점쌍극자（PU沁
d如아e）라고 한다. 만약 구면좌표（spherical coordinates）를 사용하여 마당의 점 P의 위치를 나타
내고, 쌍극자모멘트 p의 방향이 z축이라면 ＠은



                        勃（       「）        =   :   ,"，“「   으                                      (8)


가 된다. 여기에서 0는 마당의 점이 z축과 이루는 각이다. 한편, 등전위면을 나타내는 방정식은



                        「" 小毛, ]cos0
가 된다．
 이제 점쌍극자의 등전위선을 구현하여 보자．
 그런데 위에서 우리는 쌍극자모멘트의 방향이 z축이라고 하였는데 이것은 어디까지나 구면좌표계
에서 그렇다는 것이고, 우리가 지금 컴퓨터 모니터 화면에 등전위선을 그리려면 쌍극자모멘트의 방
향이 y축이나 x축이라고 해야 한다. 무슨 말인지 이해가 가지 않는 독자가 있을지 모르겠는데, 이렇
게 하면 컴퓨터 화면 상에 쌍극자모멘트가 있는 것이다. 조금만 생각해 보면 무슨 말인지 알 수 있
을 것이다．
 이제 Mathematica에서 전위함수를 정의하자. 점쌍극자의 좌표는 화면의 중심 (512, 384）이다．

수식을 간략화시키기 위해 8에서 才쓸
                   . = 150 "］라고 하면， 전위는


                              i / \            , 尸,-' cos6
                         YD ( ' ') =           1JU11=
                                                    7'
86 제］부 정전기학乍旭ctro없atics)



가 된다. 모니터 화면좌표꼐에서 쌍극자모멘트의 방향이 x축이라면 cosO는


                                                                   x- 512
                                                         /(x_ 512)2+ (y- 384)2




                                                         (x- 512)2+ (y- 384) 2


이다. Mathematica에서 아래


                                        5l2)
                      ] ::                            (y_ 3B4) 2
                                        r                ]
   r
       (x_   ,
                 y_
                             'J   (x_
                                                 2+

                                            工’
                                                 512 ,
   pbi[ x_ , y_ ] :=50*
                                        1 1 L工 r yJ !    /




와 같이 전위함수를 정의한다．
 전위의 최대값을 구하기 위해 아래


   Max (Max (Table[phi (x, y] , {x, 50, 1000) , {y, 50, 383) ]],
       Max (Tab1e[phi (x, 384] , {x, 50, 511) ]] , Max (Table[phi [x, 384] , {x, 513, 1000) ]],
       Max[Table (phi (x, y] , {x, 50, 1000) , {y, 385, 650) ])]




와 같이 명령하고, 전위의 최소값을 구하기 위해 아래


   Min (Min (Tab1e (phi[ x, y) , {x, 50, 1000} , {y, 50, 383) ]],
       Min (Table (phi (x, 384] , {x, 50, 511} ]] , Min[ Table (phi 江, 384] , {x, 513, 1000) ]] ,
       Min[ Table (phi (x, y] , {x, 50, 1000) , {y, 385, 650) ]]]




와 같이 명령하면 결과는 각각 150과 - 150이다．


3.3.2. Source Code

// 점쌍극자뀌ew.cpp : implementation of the （玉4yView class
                                                                           제3장 전기다중극（E旭아nc M미tip이e) 87



1/

#include ustdafx.h11
荊nclude " 점쌍극자.h


荊nclude " 점쌍극자Doc.h '
荊nclude " 점쌍극자View.h"


#include <math.h>


double phi [95111 [6011;
double potential( double x, double y, double xPrime, double yPrime );


#ifdef _DEBUG
#define new DEBUG_NEW
#undef THIS_FILE
static char THIS_FILE [1 = _FILE_;
#endif


///I!//////I/////I//I//////I//II//////////////////I//////II//I/////////I///I/
II CMyView

IMPLEMENT_DYNCREATE (CMyView, CView)


BEGIN_MESSAGE_MAP (CMyView, CView)
     II { {AFX_MSG_MAP (CMyView)
           II NOTE H the ClassWizard will add and remove mapping macros here.
           II     DO NOT EDIT what you see in these blocks of generated code!
      //} } AFX_MSG_MAP
     II Standard printing commands
      ON_COMMAND (ID_FILE_PRINT, CView::OnFilePrint)
      ON_COMMAND (ID_FILE_PRINT_DIRECT, CView: :OnFilePrint)
88 제］부 정전기학（Electra없카（s)



     ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView::OnpilePrintPreview)
END_MESSAGE_MAP 0


/////////////////////////////////////////////////////////////////////////////
II CMyView construction/destruction


CMyView::CMy View 0
{
     II TODO: add construction code here


}

CMyView::사CMyView 0
{
}

BOOL CMyView::PreCreateWindow (CREATESTRUCT& cs)
{
     // TODO: Modify the Window class or styles here by modifying
     1/ the CREATESTRUCT cs


     return CView::preCreateWjndow (cs);
}

//////////////////////7//////////////////////////////////////////////////////
1/ CMyView drawing


void CMyView::OnDraw (CDC* pDC)
{
     CMyDoc* pDoc = GetDocument0;
     ASSERT_VALID (pDoc);
                                                       제3장 전기다중극（E旭아nc Multip이e) 89



c10ck. t start, finish;
double xPrime==512.0, yPrime=384.0;
double y, x, interval, max=150.0, min= -150.0;
double duration;
char str [1001;


pDC->Rectangle( 49, 49, 1001, 651 );
pDC->MoveTo ( m t (xPrime) -5, mnt (yPrime) );
pDC- >LineTo ( mnt (xPrime) + 5, mnt (yPrime) );
pDC->MoveTo ( mnt (xPrime) + 2, m t (yPrime) -3 );
pDC->LineTo( int (xPrime) +5, int(yPrime) );
pDC->LineTo( int (xPrime) +2, int (yPrime) +3 );


start = clock 0;


for (y=50.O; y<651.O; y++)
     for (x=50.0; x<1001.0; x++)
     {
         if ( (x==xPrime)&&(y==yPrime) )
              break;


         phi [int (x) -50] [int (y) -50] = potential ( x, y, xPrime, yPrime );
     }

for (interval=max; interval>=min; interval- = (max -mmn) /7000.0)
     for (y=50.O; y<651.O; y++)
          for (x=50.0; x<1001.0; x++)
          {
              if ( (x==xPrime）芯邑（y= =yPri毗） )
                   break;


              if ( (phi [mnt (x) -501 [mnt (y) -501>interval- (max-min)/700000.0)
    90 제］부 정전기학（印C打0없帥cs)




                              &&(phi [int (x) -50] [int (y) -501<interval+ (max-min)/700000.0) )
                             if ( phi[int (x) -50] [int(y) -50] >0.0 )
                                   pDC->SetPixel( int (x), int (y), RGB(255, 0, 0) );
                             이se if ( ph小nt的m印］[int (y) -50] <0.0 )
                                   pDC->SetPixel( int (x), int(y), RGB(0, 0, 255) );
                             이se
                                   pDC->SetPixel( int (x), int (y), RGB(255, 0, 255) );
                  }

      finish = clockO;


      duration = (double) (finish- start) /CLOCKS_PE艮SEC;


      pDC->SetTextAlign( TA_CENTER + TA_TOP);
      sprintf ( str, "A]간＝%lf초", duration );
      pDC->TextOut (512, 20, str);
}

II///II/I////////I///I/////////III/I/I/III///III//I/////////I//////////III///
II CMyView printing


BOOL CMyView::OnPreparePrinting (CPrintlnfo* plnfo)
{
      II default preparation
      return DoPreparePrinting (plnfo);
}

void CMyView::OnBeginPrinting (CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     II TODO: add extra initialization before printing
}
                                                                           제3장 전기다중극（F陀아nc M미如이e)   91




void CMyView::OnEndPrinting (CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     II TODO: add cleanup after printing
}

/////////////////////////////////////////////////////////////////////////////
/1 CMyView diagnostics


荊fdef DEBUG
void CMyView::AssertValid() const
{
     CView::AssertValidO;
}

void CMyView::Dump (CDumpContext& dc) const
{
     CView::Dump (dc) ;
}

CMyDoc* CMyView::GetDocumentO II non-debug version is inline
{
     ASSERT (m_pDocument->IsKindOf (RUNTIME_CLASS (CMyDoc) ));
     return (CMyDoc*) rn_pDocument;
}
#endif 仄DEBUG


/////////////////////////////////////////////////////////////////////////////
II CMyView message handlers


double potential( double x, double y, double xPrime, double yPrime )
{
     double r;
92 제］부 정전기학乍厄ctro없帥cs)



     r = sqrt ( (x-xPrime) * (x-xPrime) + (y-yPrime) * (y-yPrime) );
     return 150.0* ((x-xPrime)/(r*r*r));
}

333 프로그램 실행 결과


             毛 졈當극자     찌복앉믐
             파일（E)   편집上） 보게Y)     도욤말叱）
             ［그 心 1m           凸    !

                                               1 1 가 小59 996000 초




                                                   :
                                                   m口m
                                                     亡
                                                       11Jt告立j
                                                                    /
                                                                    /
                                                                    1
                                                                    \
              到                                                         N마너




3.4. 사韶자마당

3.4.1. 이론

    (5）를 이용하면


                      r2(3cos20i-1) = 3(i · ri)2-r2
                                           =3(奴＋蜘＋lz寸나六12 + l2 + 功


이 된다. 전개해서 정리하면
                                                         제3장 전기다중극（E旭아nc Mu作巾이e)   93




     寸 (3 cos20i小 1)
     = 取抛2 中r2) + y向i2 H 寸）+ 12個才                 r2) + 6的r跣＋吼切m+ 6址z伊뇨


을 얻는다．
 위 식의 우변에서 마지막 3개의 항을


                       61蜘yi = 3 l伊jy汁 31y切ixi,
                       吼切izi = 孔切izi + 잃zl戶y2,
                        6吼헉xi = 3 l) z; + 3 lT1따힉


와 같이 나누면 아래


      N
      Z日
                           N                              N             N
         吼r2 (3cos20i- 1) = i了＞그 吼伽？H寸）+lxl月 吼3x2y1+ 1l＞二 吼3따긱
                          i= 1                           i= 1          工= 1
                           N                      N                     N
                       +ly吃 吼3y;+ 1了＞二 吼（3y2- r12) + l,l즌二 吼3yzj                   (9)
                           2二＝1                  i= 1                  i= 1
                           N                       N             N
                       +lzl乞 吼3긱따+ lzl乞 吼3z2y뇨＋ j2z＞二 吼（3才 -r놓2)
                           2=1                    i= 1          i= 1




와 같이 대칭적인 형태로 쓸 수 있다．
 다음과 같이 사중극자모멘트 텐서의 성분 砥를 정의한다．


                                    N

                        Q｝丸＝ Z             吼（3j小i- r:2dj丸）
                                  i 二二二l




여기에서 3와 丸는 I, y, z 중 어느 한 가지를 나타낸다． 그리고， oj丸는 아래




                          jk=1,:：上‘，
와 같이 정의되는 크로네커 델타（Kronecker delta）이다. 그러면 아래
94 제］부 정전기학（E泡ctro없카ics)


                                   N
                                   Zm
                                                                                                                                             N
                                                                                                                                             Z勻
                                    %                                                                                                                                                         N
                                    吼        =                   吼    QU
                                                                                        9
                                                                                                        9
                                                                                    町
                                                                                                    寸
                                                                                                                                                        吼3따Ui, 吼＝ Z                                     吼3따zi,
                                                                                                                                                                                          i= 1
                                                       N                                                                      N                                                               N
                               Q恥＝ i=Z1 吼3yx, QW=: : 吼（3y2- r2), QW= Z
                                                  i= 1                                                                                                                                    i= 1
                                                       N                                                                      N                                             N
                                   Q:, = E qi3z2毛， Q,= Z q多ziyi, 吼＝ Z 吼（3z12 - r2)              H

                                                                                                1




                                         i=                1                                                              i= 1                                         i= 1




와 같이 9개의 Q七7} 있게 된다．
 전하가 연속적으로 분포되어 있으면



                                                                     Q3k=
                                                                                                            /,
                                                                                                                      p
                                                                                                                              『 ')
                                                                                                                              （
                                                                                                                                        (3j   '丸
                                                                                                                                                   '_
                                                                                                                                                         712万必）        dT
                                                                                                                                                                                 '




7} 된다. 구체적으로，




  Q끄= fVIp(r')(3x'2-r'2)dr', Qq,= fVIp(r')3x'y'dr', Q1                                                                                                                                            /,
                                                                                                                                                                                                           p (r')3x'z'dr',


                                             ') 3y노                                                                                                                                                        p (r')3y'z'dT',
  吼＝
                   /,,,
                               p
                                   (r
                                                           'd乙
                                                                            Qgy=
                                                                                                                 I,
                                                                                                                          p
                                                                                                                                  (r
                                                                                                                                       ')   (3y'2-        r
                                                                                                                                                              )
                                                                                                                                                                  d7
                                                                                                                                                                            ',       Q,
                                                                                                                                                                                          =       IV,
       吼=
                          f
                          VI       p    (r
                                             ')   3z
                                                       'x'dr ',                Q;
                                                                                            =
                                                                                                                  f,,VIp(r')3z'y'dr', Q:= f,, p(r')(3z'2-尸2)dr'
이다．
 Q必를 사용하면 ＠는

             N

            ＞그 吼r2 (3cos292- 1)
            i= 1

            = 毋吼＋吼Q四＋ 址吼日兀吼＋gQd 꾸刃d izi묘卄 Izi皿汁 z
                                               ,2r)
                                                  ' zz

            = j=Z        : YkQjk
                iy, z k= x, y, z
                                                                               제3장 전기다중극（E旭아nc MuRi口이e)   95



가 된다．
 이제 위의 식을 사중극항에 대입하면



                札（미三，右3 去，=; ,且，, 11kQ)k
을 얻는다．
 장의 점이 멀리 떨어져 있고 홀극모멘트와 쌍극자모멘트가 각각 Q= O, p= 0이면， Qj/.;7} 전하
분포의 주된 모습이 된다．
 한편, 위의 사중극항을


                丸仕）=                    ]
                                                          l
                                                                      Z
                                                                                   Z
                                                                                           J
                                                                                               아
                               47rEAr5
                                                                                       凡
                                                      可
                                                                  m
                                                                               却
와 같이 쓸 수 있다. 왜냐하면



                                            프 r                               三 r
                                   7
                                                  U
                                                  m
                                                              y           2                        1
                                                                                                   1

                                                                                                   +
                                                                                                   +




                                                              r
                               뇨
이기 때문이다．
 정의에 의하여 Q七 9깨 있다． 그러나，


                    （工戶 吼， 吼＝ 吼， 吼＝（兀y


이므로 9개의 Q丸어］서 독립성분은 6개이다．
 한편, 대각선 성분들을 모두 합하면


                         N
         吼＋ Q四＋ Q仁＝ Z                  吼［(3寸- r2) + (3y2H r2) + (3긱i2H pi2)]
                     i= 1



                             N
                             H卜m
                               =
                         1
                                                                                                          @
                                       吼［3 (x2 + yi2 + 才）- 3r기
                     i
                     1
                     0
96 제］부 정전기학乍lectro없atics)


이므로 독립성분은 다섯 개로 줄어든다．
 독립성분이 다섯 개임을 알게 되었으나 아직도 복잡하다. 문제를 좀 더 간단히 만들기 위해 전하
분포가 원통이나 원뿔과 같이 회전체를 이룬다고 하자. 대칭축은 z축이라고 하자. 또한, 대칭축에 대
해 서로 대응하는 한 쌍의 전하의 크기는 동일하다고 하자．
 그러면 佃', yl, zi）에 있는 전하 cj'에 대해서 (- xl, yl, zi）에 똑같은 크기의 전하가 있고 이와 같은
한 쌍의 전하가 Q伊 吼어］ 주는 기여는 각각


                                3q'x'y'+ 3q'(- x') y'= 0,
                                  3q／名／可＋ 3q／名／(- x') = 0


이다． 모든 전하들을 이렇게 짝을 지을 수 있으므로 결국 q戶 吼= 0이다． 마찬가지로
（乙 yl, zi）에 있는 전하 了어］ 대해서 （可, _y', z'）에 똑같은 크기의 전하가 있고 이와 같은 한 쌍
의 전하가 吼어］ 주는 기여는


                                  3q'y'z'+ 3q' (- y')z'= 0


이다． 모든 전하들을 이렇게 짝을 지을 수 있으므로 결국 Q恥＝ 0이다．
 이제 3개의 대각선 성분들만 남았다. 그런데 匈이 성립하므로 독립성분은 두개로 줄어든다．
 그럼 이제 더 이상 독립성분의 개수를 줄일 수 없는 것일까7
 그렇지 않다． 축대칭인 경우에는 x축과 y축의 구분이 무의미하므로 吼= Q9V7} 성립한다． 따라
서, 최종적으로 독립성분은 단 하나가 된다．
 이제 사중극항은 상당히 간단한 형태가 된다. 약간의 대수 계산을 하면


                            Q        3尸 -1        Q,2        3cos20- 1
                                                                         @
               札（r)
                            , 2

                      =
                          4ire0        4r3       4irE0          4r3


을 얻는다. 여기에서 9는 장의 점의 위치벡터 r와 대칭축 사이의 각도이다．
 아래의 두 전하분포는 사중극자모멘트（quadrup아em아rient)를 갖는다．
                                                                                         제3장 전기다중극（Ele아nc Mult巾이e) 97



                        q                 q



                     q                    n
                                                                            -        q       2q
                                                                                             片          3

                                          q
                    q


 프로그램으로 구현하여 보자．
 물리좌표계에서 화면좌표계로 변환할 때 주의한다. 지금까지 z축이 대칭축이라고 하였는데 이것
은 물리좌표계에서 그렇다는 것이고, 화면좌표계에서는 y축이 대칭축이라고 하자．
 우선 Mathematica에서 전위함수를 정의하자. 사중극자의 좌표는 화면의 중심 (512, 384）이다．

수식을 간략화시키기 위해 ＠에서 4ir。
                     ,                                   , ::,
                                                         Q
                                                                    =-
                                                                         200 이라고 하면， 전위는
                                                     4
                                                小 仟＼ - 50 (1 中3cos29)
                                                     /   (/ \ 1 /
                                                1/
                                                                                r3




가 된다. 화면좌표계에서 대칭축이 y축이므로 cos9는


                                                       384- v
                                               \/(x_ 512) 2+ (y- 384) 2


이다. 그리고, r3은



                                               小- 512)뇨 (y                       昭이午


이다. Mathematica에서 아래


   r
       (xe   ,   y J :=   \/(x_
                                  512)
                                         2+   (y_ 384) 2
     98 제］부 정전기학（Electrostatics)


                              384 -y
          eozine (x ,y ] : =
                   1  1      r ［毛 y]

                               50 (1 = 3 OO虹ne［毛 y] 2)
          plii[ x_ , y_ ] :=
                                      r[ x, y] 3




     와 같이 전위함수를 정의한다．
         전위의 최대값을 구하기 위해 아래


          Max (Max (Table (phi Cx, yj , {x, 50, 1000} , {y, 50, 383} ]] /
           Max (Tab1e (phi (x, 384] , {x, 50, 511} J] , Max (Table[phi 江, 384] r { x, 513, 1000} ]] r
           MaxLTab1e[phi (x, y] , {x, 50, 1000} , {y, 385, 650} J] J




 와 같이 명령하고, 전위의 최소값을 구하기 위해 아래


          Min (Min (Tab1e[phi[ x, y] , {x, 50, 1000} , {y, 50, 383} ]] ,
           Min[ Tab1e (phi (x, 384] , {x, 50, 511} ]] , M.tn (Tab1e[phi (x, 384] , {x, 513, 1000} ]J r
           Min (Table (phi (x, y] , {x, 50, 1000} , {y, 385, 650} )]]




와 같이 명령하면 결과는 각각 50 , 小100이다．
         앞 section의 프로그램에서도 그랬지만, 픽셀 하나가 물리좌표계의 1과 대응하는 이러한
mapping m아le에서는 보기에 좋은 결과가 나오지 않을 것이다. 쌍극자 주변에는 여러 개의 등퍼텐
셜선이 그려지지만 대부분의 영역에는 등퍼텐셜선이 그려지지 않는다. 그럼 어떻게 할까7 좀 더 보
기에 좋은 결과를 얻으려면 여러 개의 픽셀이 물리좌표계의 1과 대응하도록 하면 된다. 이것은 독자
7} 스스로 해결해 보아라．


3.4.2. Source Code

II 사중극 4View.cpp : implementation of the CMyView class
I,   '



 #include n stdafx.h"
荊nclude ”사중극자．h


荊nclude ”사중극자Doc.h"
                                                                           제3장 전기다중극（E旭아nc Multip이e) 99



荊nclude " 사중극자뀌ew.h"


#include <math.h>


double phi [951] [6011;
double potential( double x, double y, double xPrime, double yPrime );


荊fdef DEBUG
#define new DEBUG_NEW
#undef THIS_FILE
static char THIS_FILE [] = _FILE_;
#endif


/////////////////////////////////////////////////////////////////////////////
II CMyView

IMPLEMENT_DYNCREATE (CMyView, CView)


BEGIN_MESSAGE_MAP (CMyView, CView)
      // { {AFX_MSG_MAP (CMy View)
           II NOTE - the ClassWizard will add and remove mapping macros here,
           II      DO NOT EDIT what you see in these blocks of generated code!
     II) } AFX_MSG_MAP
     II Standard printing commands
      ON_COMMAND (ID_FILE_PRINT, CView::OnFjlePrint)
      ON_COMMAND (ID_FILE_PRINT_DIRECT, CView::OnFilePrint)
      ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView: OnFilePrintPreview)
END_MESSAGE_MAP 0


/////////////////////////////////////////////////////////////////////////////
// CMyView construction/destruction
100 제］부 정전기학乍lectrostatics)



CMyView::CMy View 0
{
     II TODO: add construction code here


}

CMyView::사CMyView 0
{
}

BOOL CMyView::PreCreateWindow (CREATESTRUCT& cs)
{
     II TODO: Modify the Window class or styles here by modifying
     II the CREATESTRUCT cs


      return CView::PreCreateWindow (cs);
}

I/IIIII/I/I/IIIIIII/III/!IIIIIIII/I/I/I//I/IIIIIII//IIII/III//II/II/III/I/I/I
// CMyView drawing


void CMyView::OnDraw (CDC* pDC)
{
      CMyDoc* pDoc = GetDocument0;
      ASSERT_VALID (pDoc);


      clock_t start, finish;
      double xPrime=512.0, yPrime=384.0;
      double y, x, interval, max=50.0, min=-100.0;
      double duration;
      char str[1001;
                                                         제3장 전기다중극（E旭아nc Mu'ti口o'e) 101



pDC->Rectangle (49, 49, 1001, 651) ;


start = clock 0;


for (y=50.0; y<651.O; y++)
    for (x=50.0; x<1001.0; x++)
    {
        if ( (x==xPrime) &&(y==yPrime) )
            break;


        phi[int (x) -501 [int (y) -501 = potential( x, y, xPrime, yPrime );
    }

for (interval=max; interval>min; interval- = (max -mmn) /900.0)
    for (y=50.O; y<651.O; y++)
        for (x==50.0; x<1001.0; x++)
        {
            if ( (x= =xPrime) &&(y==yPrime) )
                   break;


            if ( (phi [m t (x) -501 [mnt (y) -50] >interval- (max-min)/14000.0)
                   && (phi [mnt (x) -501 [mlt (y) -501<interval+ (max-min)/14000.0) )
                   if ( phi [int (x) -501 [int (y) -501>0.0 )
                       pDC->SetPixel( int (x), int (y), RGB(255, 0, 0) );
                   이se if ( ph小nt的H加］[int (y）巾50] <0.0 )
                       pDC->SetPixel( int (x), int (y), RGB(0, 0, 255) );
                   els（三
                       pDC->SetPixel( int (x), int (y), RGB(255, 0, 255) );
        }

finish = clockO;
102 제］부 정전기학（Electrostatics)



     duration = (double) (finish - start) /CLOCKS_PER..SEC;


     pDC->SetTextAlign( TPLCENTER + TA-TOP);
     sprintf ( str, "시간＝%lf초", duration );
     pDC->TextOut (512, 20, str);
}

/////////////////////////////////////////////I///////////////////////////////
/1 CMyView printing


BOOL CMyView::OnPreparePrinting (CPrintlnfo* plnfo)
{
     II default preparation
     return DoPreparePrinting (plnfo);
}

void CMyView::OnBeginPrinting (CDC卞 ／來pDC玎, CPrintlnfo半 小plnfo串／)
{
     II TODO: add extra initialization before printing
}

void CMyView::OnEndPrinting (CDC半 /*pDC町, CPrintlnfo米 /*이nfo來／)
{
     II TODO: add cleanup after printing
}

/////////////////////////////////////////////////////////////////////////////
7/ CMyView diagnostics


#ifdef _DEBUG
void CMyView::AssertValid0 const
{
                                                                          제3장 전기다중극（티ectric M미ti口이e) 103



         CView::AssertValid 0;
}

void CMyView: :Dump (CDumpContext& dc) const
     {
         CView::Dump (dc) ;
}

CMyDoc* CMyView::GetDocument0 II non-debug version is inline
     {
         ASSERT (m_pDocument寸 >IsKindOf (RUNTIME_CLASS (CMyDoc)));
         return (CMyDoc*) m_pDocument;
}
#endif 仄DEBUG


/////////////////////////////////////////////////////////////////////////////
II CMyView message handlers


double potential ( double x, double y, double xPrime, double yPrime )
 {
         double r, cosine;
         r = sqrt ( (x-xPrime) * (x-xPrime) + (y- yPrime) * (y-yPrime) );
         cosine = (yPrime-y)/r;
         return 50.아（(1.0田, 小co針ne札osine) /(r甘寸力；
I.
104 제］부 정전기학（Electrostatics)




3.4.3, 프로그램 실행 켤과


           따덜（E)   편집上） 보7Ky)   도묩말언）
           D 4 日         甘1 因    寸


                                        시 간円4.185000초




                                            壬
                  駙벱쌔ho川I a咐

4.1. 개론

 지금까지 우리는 주어진 영역 내에 전기마당에 영향을 줄 수 있는 어떤，것이 존재하지 않는 상황
만을 고려하였다. 하지만, 전하나 전하분포가 도체 가까이에 있는 경우가 흔히 있다. 이런 상황에서
는 도체 표면의 전하분포를 알아야 한다．
 전기쌍극자를 구성하는 한 전하에서 다른 전하까지의 변위（dis이acement)를 수직이등분하는 평
면 상의 모든 점에서 전위는 0이고, 전기력선（line of 이ec竹ic force）은 그 평면과 직각으로 만난
다. 즉, 그 평면은 평면 도체와 같은 역할을 한다. 다시 말하면, 그 평면 위치에 평면 도체를 삽입하
더라도 쌍극자에 의한 전기력선의 모양에는 변화가 없다. 만약 평면 도체를 삽입한 후 음전하를 제
거한다면 양전하가 있는 영역에서의 전기마당분포는 그태로이고 도체 표면에는 -q의 음전하가 유
도된다. 역으로 만약 우리가 무한평면 도체에서 d 만큼 떨어진 곳에 점전하 q를 놓으면, 무한평면
도체를 무시하고 무한평면 도체를 기준으로 점전하 q어］ 대칭인 곳에 -q의 점전하가 있다고 가정함
으로써 점전하 q가 있는 영역의 임의의 점에서 전위와 전기마당을 구할 수 있다. 이 때 가상적인 전
하 -q를 q의 영상帥age）이라고 한다．
 이처럼 영상법에서는 잠정적으로 평면 도체를 무시하고, 평면 도체를 기준으로 q와 서로 다른 영
역에 가상전하 -q를 놓는다. 가상전하는 실전하와 크기는 같고 부호는 반대이다. 주의할 것은 앞의
단락에서의 설명은 무한평면 도체인 경우에만 사실이라는 것이다．
 결론적으로 말하면, 영상법은 전위를




                         Ra + , 읖, 4ir！뇨
                 砂＝ 盈, 打！。a                                 (D
106 제］부 정전기학（Electrostatics)




의 형태로 쓸 수 있도록 한다．
 영상법을 적용할 때에는 다음의 두 가지를 만족시키도록 해야 한다．


(1) 영상전하는 도체가 있는 영역 내에 위치해야 한다．
(2) 도체 표면이 등전위면이 되도록 영상전하를 위치시켜야 한다．


조건 (1）은 푸아송 방정식（P이sson equation）을 만족시키기 위해 필요하고, 조컨 (2）는 경계조건을
만족시키기 위해 필요하다．
 모든 정전기적 문제에 영상법을 적용할 수는 없지만, 풀기 어려운 문제가 영상법에 의해 쉽게 풀
리는 경우가 많다. 절대온도눈금을 도입한 영국의 물리학자 켈빈（K이미n)이 영상법을 도입하였다．



4.2. 점전하와 접지된 반무횬뼝면 도체

4.2.1. 이론
                                                               제4장 영상법（Method of Image) 107



 위의 그림에서 보는 것처럼 , 점전하 q는 yz평면으로부터 d 만큼 떨어져 있다. 万 드 0인 공간은 도
체이고 y名평면은 이 도체의 표면이다. 도체가 아닌 공간은 진공이다. 도체의 표면은 등전위면이므로
경계조건은 x= O에서 砂는 상수이다. 문제를 간단하게 하기 위해 x= 0에서 砂 = 0이라고 하자. 만
약 도체 표면에서의 전위값이 0이 아니라면, 우리는 0이라고 가정하고 문제를 해결한 다음에 도체
의 표면의 전위값을 더해주면 된다．
 도체 표면으로부터 도체 내부 방향으로 d/ 만큼 떨어진 곳에 위치한 영상전하 d은 진공 영역에 대
하여 도체를 대체시킨다. q와 q'의 좌표는 각각 (d, 0,0), (- d', O, o）이므로 d）은


        未／m . . 사＼                 1     !          q        .         q'        ]       丙＼
        V kJ勺   y, ( j-           二＝=H {    /      入   .\  八 丁  尸＝ =111          卜       \e/
                                  仕lie() i V (x- d)'+ yz+ zZ   V(x+ df)z+ yz+ zz j


으로 쓸 수 있다．
 한편, 위의 식은 경계조건


                                             砂（0, y, z) =0


을 만족시켜야 하므로


                                      ,  q       + '    q'      =0
                                     /d2+ y2+ z2   /d'2+ y2+ z2


이 성립한다．
 명백히 d' = d이고 q'= -q이라면 위의 식은 항상 성립한다. 그러므로 q가 도체의 표면에서 떨어
져 있는 거리만큼，了도 도체의 표면에서 떨어져 있다. 물론 도체의 표면을 기준으로 q와 d은 서로
다른 영역에 놓여 있다．
 방금 구한 이들 값들을 (2）어］ 대입하면


                                                 1                    1          1
        砂（x,    y,   z   卜4시小d)                  2+   y2+ z2   Vm旴＋y2＋기
을 얻는다. 이것이 완전한 해이다. 위의 식은 x 之 0일 때에만 사용한다．
 도체의 내부에서의 전위는 도체의 표면의 전위값과 같다. 그런데, 우리는 처음에 도체 표면의 전
108 제］부 정전기학乍厄ctrostatics)



위값을 0이라고 가정하였으므로, 도체 내부에서의 전위는 0이다．
 x 立 0인 영역에서 등전위면을 나타내는 방정식은 위의 식에서 전위를 상수로 놓아 구할 수 있다．
xy평면에서의 등전위선을 구하려면 z= 0이라 놓아 구할 수 있다．
 참고로, q어］ 작용하는 힘을 구해보면


                                             ，거                02               스
                                             r =1              4             '\ X
                                                           47rE。(2d）乙


이다. 이것은 q와 영상전하 -q가 2d 만큼 떨어져 있을 때에 두 전하 사이의 인력에 대한 쿨롱의
법칙과 같다．
 프로그램으로 구현하여 보자．
 도체의 표면은 모니터 좌표계에서 x=100이다. 점전하의 크기는 9mC이고 점전하의 위치는
(500, 350）이다. 그러면 영상전하의 위치는 (-300, 350）이다．
 우선 Mathematica에서 다음과 같이 전위함수를 정의한다．


                                                                I

                                                                                       4
                                                                                                      1
                                                                                                                        1J
   phi【＝ -   ,   y-   )   :=   8加755   *9니
                                              4   (x   -   500) 2 + (y   -    350) 2       (x+
                                                                                                 300) 2+   (y- 350) 2


 전위의 최대값을 구하기 위해 아래


   Max (Max (Table (phi (x, y] , {x, 101, 1000) , {y, 50, 349) ]] r
    Max 口able (phi (x, 350] , {x, 101, 499) ]] , Uax (Table (phi (x, 350] , {x, 501, 1000) ]] ,
    Max (Table (phi (x, y] , {x, 101, 1000) , {y, 351, 650) ]]]




와 같이 명령하고, 전위의 최소값을 구하기 위해 아래


   Min (Min 四able[phi (x, y] , {x, 101, 1000) , {y, 50, 349} ]] r
    Min (Table (phi[ x, 350] , {x, 101, 499) ]],              Min (Table (phi[ x, 350) , {x, 501, 1000) ]] ,
    Min[ Table (phi Lx, y] / {x, 101, 1000} , {y, 351, 650) ]])




와 같이 명령하면, 결과는 각각 8.0787 x i07, 517.683이다．
                                                                                제4장 영상법（Meth이:1 of Image) 109




4.2.2. Source Code

// 점전하와 접지된 반무한평면 도체뀌ew.cpp : im이ementation of the CMyView class
II

#include "stdafx.h"
荊nclude " 점전하와 접지된 반무한평면 도체.h'


荊nclude " 점전하와 접지된 반무한평면 도체Doc.h"
荊nclude "점전하와 접지된 반무한평면 도체피이V.h"


#include <math.h>


double phi [9511 [6011;
double potential( double x, double y, double xPrime, double yPrime, double charge );


#ifdef _DEBUG
#define new DEBUG_NEW
#undef THIS_FILE
static char THIS_FILE[] = _-FILE_;
#endif


//////////I///////////////////!/////////!//////////////////////I//I/////////I
II CMyView

IMPLEMENT_DYNCREATE (CMyView, CView)


BEGIN_MESSAGE_MAP (CMyView, CView)
      /1{ {AFX_MSG_MAP (CMyView)
           II NOTE - the ClassWizard will add and remove mapping macros here.
           //      DO NOT EDIT what you see in these blocks of generated code!
    110 제］부 정전기학（Electrost카（s)



         //} } AFX_MSG_MAP
        II Standard printing commands
        ON_COMMAND (ID_FILE_PRINT, CView::OnFjlePrjnt)
        ON_COMMAND (ID_
                     FILE_PRINT_DIRECT, CView::OnFilePrint)
        ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView: :OnFilePrintPreview)
 END_MESSAGE_MAP 0


 /////////////////////////////////////////////////////////////////////////////
II CMyView construction/destruction


CMyView::CMyView0
    {
        // TODO: add construction code here


}

CMyView::NCMyView 0
 {
}

BOOL CMyView::PreCreate Window (CREATESTRUCT& cs)
{
        // TODO: Modify the Window class or styles here by modifying
        // the CREATESTRUCT cs


        return CView::PreCreateWindow (cs);
}

/////////////////////////////////////////////////////////////////////////////
/1 CMyView drawing


void CMyView::OnDraw (CDC* pDC)
                                                       제4장 영상법（Method of Image) 111




CMyDoc* pDoc = GetDocument 0;
ASSERT_VALID (pDoc);


clockj start, finish;
double xPrime=500.0, yPrime=350.0, charge=9E-3;
double y, x, interval, max=8.0787E7, min=517.683;
double duration;
char str[100] ;


pDC->Rectangle ( 49, 49, 1001, 651 );


CBrush Distribution (RGB (0,0,0) );
CBrush* pBrush;
pBrush = pDC- >Select0bject (&Distribution);
pDC->Rectangle (50, 50, 100, 650);
pDC- >SelectObject (pBrush);


start = clock 0;


for (y=50.O; y<651.0; y++)
     for (x=101.0; x<1001.0; x++)
     {
         if ( (x==xPrime) &&(y= =yPrime) )
              break;


         phi[int (x) -501 [int (y) -50] = potential ( x, y, xPrime, yPrime, charge );
     }

 for (interval=max; interval>min; interval-= (max-min) /900.0)
     for (y=50.0; y<651.O; y++)
          for (x=101.0; x<1001.0; x++)
112 제］부 정전7 i (EIectrostatics)



                 {
                      if ( (x==xPrime) &&(y==yPrime) )
                            break;


                      if ( (phi [m t (x) -501 [mnt (y) -501>interval- (max-mmn) /80000.0)
                            && (phi [mnt (x) -50] [mnt (y) -50] <interval+ (max-mmn) /80000.0) )
                            pDC->SetPixel( int (x), int (y), RGB(255, 0, 0) );
                 }

     finish = c1ock0;


     duration = (double) (finish-start)/CLOCKS_PER_SEC;


     pDC - >SetTextAlign (TA_CENTER+ TA_TOP);
     sprintf ( str, "시간＝%lf초" , duration );
     pDC->TextOut (512, 20, str);
}

/////////////////////////////////////////////////////////////////////////////
7/ CMyView printing


BOOL CMyView::OnPreparePrinting(CPrintlnfo* plnfo)
{
     7/ default preparation
     return DoPreparePrinting (plnfo);
}

void CMyView::OnBeginPrinting(CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     II TODO: add extra initialization before printing
}
                                                                                제4장 영상법（Method of Image) 113



void CMyView::OnEndPrinting (CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
 {
      // TODO: add cleanup after printing
}

/////I//////////////I///////////////I///////////////////////////////!////////
II CMyView diagnostics

#ifdef _DEBUG
void CMyView::AssertValidO const
 {
      CView::AssertValid 0;
}

void CMyView::Dump (CDumpContext& dc) const
 {
      CView::Dump (dc);
}

CMyDoc* CMyView::GetDocument0 II non-debug version is inline
 {
      ASSERT (mpDocument - >IsKind0f (RUNTIME_CLASS (CMyDoc)));
      return (CMyDoc*)m_pDocument;
}
#endif I/_DEBUG


///IIIIII/I/I//II/II//IIIIIIIII//II/IIIIII/III///I/IIIIII/I/////II/I/II//IIII
II CMyView message handlers

double potential ( double x, double y, double xPrime, double yPrime, double charge )
{
      dou바e r;
114 제］부 정전기학（Electrostatics)



     r = sqrt ( (x-xPrime) *(x-xPrime) + (y-yPrime) *(y-yPrime) );
     return 8.98755E9*charge
         * ( 1.O/r - 1.O/sqrt ( (x+300.O) * (x+300.O) + (y-yPrime) * (y-yPrime) ) );
}


423 프로그램 실행 결과


             i出n已 므口L   보기侄） 노8mtD
             0 아1        三受 1   ！匕

                                           시간＝5L.121000초




4.3, 점전하와 접지된 도체구

4.3.1. 이론

    반지름이 a인 도체구의 중심에 원점을 둔 구면좌표를 사용하자. 그리고, z축은 중심에서 거리 d
만큼 되는 곳에 있는 q를 지나도록 선택한다．
    중심에서 거리 d/ 떨어져 있는 곳에 하나의 영상전하 q'를 놓고 문제를 해결하고자 한다. 영상전하
7} 진공 영역이 아닌 곳에 있으려면 （尹 < a이어야 한다．
                                                              제4장 영상법（Method of Image) 115




 마당의 점 P에서의 전위는 0과 그림으로부터


                   . /.\ -           1 (q . q'
         vy,   '   甲／   m
                             47rf。
                                       （万丁
                                              7)

                               1 (          q           .           q'       \I
                                                                                       (3)
                             二小- I     1               커r  i      -
                             47T6o (i/ r2+ d2- 2rdcosO    sJr2+ d'2- 2rd'cosO)


이다．
 한편, 위의 식을 도체구의 표면에서 전위가 0이라는 경계조컨


                                             中（a, 0, 砂） = 0


와 결부시키면



                    /a2 + d2 -2, ,,
                    V,2,,q     adc。   s。+V,
                                    , ,.  /a22,
                                              + ,d'2q- ,,/
                                                      2ad'c。
                                                          ,, ,s9. =0
을 얻는다．
116 제］부 정전기학（Electrostatics)



]   위의 식은 0의 모든 값에 대해 성립함으로 어떤 특정한 값어］ 대해서 성립한다. 특히, 0= 0과
0= ir이면 분모의 제곱근이 사라진다．
    0= 0과 0= 7r를 위의 식에 대입하면 다음의 연립방정식


                                          q, + ,         q
                                                                                 =
                                   d
                                                             'd,
                                    d-     a     a-                     d   '            0,
                                   그＋      ,   + ,       了         'd           '=        0


을 얻는다. 이 연립방정식을 풀면

                                                                                     9
                                         了＝e으a. d'=                                  d
                                                                                     丁
                                            d
                                                                                     1
                                                 4   '




이다．
    이 결과를 (3）에 대입하면


                                                                                                       으d
       rJ) rr 月 ,JL, \ 二＝   q              1

                                                                                                  르尹                           r
                                                                                                                               1\
                                                                                                                                +
            "' ' '   '    4irE。                                                                                         l19H
                                  2+ d2- 2rdcos0
                                                                                                            쓰
                                                                                                                    ＼
                                                                                              O
                                                                                              乙         r
                                                                                              r
                                                                                                                S
                                                                                                                O
                                                                                                       n
                                                                                                       乙        C   이
                                                                                                            d
                                                                                                                    J
을 얻는다. 위 식이 도체구 외부에서의 전위를 나타낸다．
    프로그램으로 구현하여 보자．
    모니터 화면좌표계에서 도체구의 중심은 (600, 300）이고, 도체구의 반지름의 길이는 100이며，
점전하의 위치는 (889, 300）이고 점전하의 크기는 27nC이다．
    우선 Mathen追tica에서 전위함수를 정의해야 하는데 점전하와 도체구 내부를 정확히 제외한 영역
에서 전위함수를 정의하려면 상당히 까다로울 것이다. 그래서 필자는 전 영역에서 점전하와 도체구
에 외접하는 입방체 내부를 제외한 영역을 전위함수의 정의역（domain of definition）으로 하였다．
이렇게 하면 실제의 정의역보다 약간 줄어들긴 하지만 등전위선을 그리는 데에는 큰 영향을 미치지
않을 것이다. 프로그램에서는 실제의 정의역을 적용하였다. 프로그램에서는 도체 내부를 정확히 저］
외하는 것이 간단하기 때문이다．
                                                                                                                       제4장 영상법（Method of Image) 117



   r
       (x_   ,
                     y-        ] :=              J
                                                     (x_
                                                                 600)
                                                                               2+       (y_ 300) 2
                                                                     x - 600
   eosine                 (x   -         ,   y ]
                                             -             :=    r    [   y]
                                                                          x,
   phi[ x_ , y_ ] :=
       8. 98755 *27 *



                                                                                        1


             Vr (x, yJ2+ 2892 -2*r[x, y] *289* cozine[x, y]


                                                                                                      쁩
                 小                 【x,       y] 2+              （쀼）2                -   2*   小艸쁑小艸：                      , ！】




 전위의 최대값을 구하기 위해 아래


   Max (Max (lable (phi (x, y] , {x, 50, 1000) , {y, 50, 200) ]] ,
       Max[Tabl. [phi (x, y] , {x, 50, 500) , {y, 201, 399} ]] r
       Max (Tab1e (phi[ x, y] , {x, 700, 1000} , {y, 201, 299) ]] ,
       Max (Table (phi[ x, 300] , {x, 700, 888) ]],                                                       Max (Tab1e[phi (x, 300] , {x, 890, 1000) ]] /
       Max (Table[phi[ x, y] , {x, 700, 1000} , {y, 301, 399) ]] r
       Hax (Table[phi[ x, y] , {x, 50, 1000) , {y, 400, 650) ]]]




와 같이 명령하고, 전위의 최소값을 구하기 위해 아래


   Min[Min (Tabl. (phi (x, y] , {x, 50, 1000) , {y, 50, 200) ]] r
       Min (Tab1e (phi[ x, y] , {x, 50, 500} , {y, 201, 399) ]] ,
       Min[ Table (phi L毛 y] , {x, 700, 1000) , {y, 201, 299) ]] ,
       Min (Table (phi (x, 300] , {x, 700, 888} JJ, Min (Table (phi (x, 300] , {x, 890, 1000) ]] ,
       Min[ Tabl. (phi 江, y] , {x, 700, 1000} , {y, 301, 399) ]] ,
       Min[ Table (phi[ x, y] , {x, 50, 1000) , {y, 400, 650) ]]]




와 같이 명령하면, 그 결과는 각각 242.335, 0이다．


4.3.2. Source Code

// 점전하와 접지된 도체구뀌ew.cpp : implementation of the CMyView class
］化 저Ii부 정전기학（Electro없카（s)




 /1

 #include Hstdafx.hu
荊n伽de " 점전하와 접지된 도체구．h


荊nclude " 점전하와 접지된 도체구Doc.h"
荊nclude " 점전하와 접지된 도체구피ew.h"


#include <math.h>


double phi[9511 [601] ;
double potential( double x, double xCenter, double charge, double r );


#ifdef UDEBUG
#define new DEBUG_NEW
#undef THIS_FILE
static char THIS_FILE [] = _FILE_;
#endif


/////////////////////////////////////////////////////////////////////////////
II CMyView


IMPLEMENT_DYNCREATE (CMyView, CView)


BEGIN_MESSAGE_MAP (CMyView, CView)
      1/ { {AFX_MSG_MAP (CMyView)
          II NOTE - the ClassWizard will add and remove mapping macros here.
          II      DO NOT EDIT what you see in these blocks of generated code!
      //} } AFX_MSG_MAP
      II Standard printing commands
      ON_COMMAND (ID_FILE_PRINT, CView::OnFjlePrjnt)
      ON_COMMAND (ID_FILE_PRINT_DIRECT, CView::OnFilePrint)
                                                                                제4장 영상법（Method of Imag이 119



     0N_COMMAND (ID_FILEYRINT_PREVIEW, CView::OnFileprintPreview)
END_MESSAGE_MAP 0


//////I//////////////////////////////////////////////////////////////////////
II CMyView construction/destruction


CMyView::CMyView0
{
     1/ TODO: add construction code here




CMyView::사CMyViewO
{
}

BOOL CMyView::PreCreate Window (CREATESTRUCT& cs)
{
      /1 TODO: Modify the Window class or styles here by modifying
     1/ the CREATESTRUCT cs


      return CView::PreCreateWindow (cs);
}

//I//////////////////////////////////////////////////////////////////////////
II CMyView drawing

void CMyView::OnDraw(CDC* pDC)
{
      CMyDoc* pDoc = GetDocument 0;
      ASSERT_VALID (pDoc);
120 제］부 정전기학（Electrost카cs)



   clock_t start, finish;
   double y, x, r, interval, max=242.335, min=0.0;
   double xCenter= 600.0, yCenter= 300.0, charge= 27E- 9;
   double xPrime=889.0, yPrime=300.0;
   double duration;
   char str[100] ;


   pDC->Rectangle ( 49, 49, 1001, 651 );


   CBrush Distribution (RGB (0,0,0));
   CBrush* pBrush;
   pBrush = pDC->SelectObject (&Distribution);
   pDC->Ellipse (500, 200, 700, 400) ;
   pDC->SelectObject (pBrush);


   start = clock 0;


   for (y=50.O; y<651.O; y++)
       for (x=50.0; x<1001.0; x++)
       {
            r = sqrt ( (x-xCenter) * (x-xCenter) + (y- yCenter) * (y-yCenter) );


            if ( r<100.0 )
                break;


            if ( (x==xPrime) &&(y==yPrime) )
                break;


            phi[int (x) -50] [int (y) -50] = potential( x, xCenter, charge, r );
       }

   for (interval=max; interval>min; interval- = (max-mmn) /4000.0)
                                                                                제4장 영상법（M이hod of Image) 121



            for (y=50.0; y<651.0; y++)
                  for (x=50.0; x<1001.0; x++)
                  {
                       if (r<100.0)
                             break;


                       if ( (x==xPrime) &&(y==yPrime) )
                             break;


                       if ( (phi [m t (x) -50] [mnt (y) -501>interval-0.005)
                             && (phi [mnt (x) -50] [mnt (y) -50] <interval+0.005) )
                             pDC->SetPixel( int (x), int (y), RGB(255, 0, 0) );
                 }
      finish = clock 0;


      duration = (double) (finish-start) /CLOCKS_PERSEC;


     pDC->SetTextAlign (TAmCENTER+TA_TOP);
     sprintf( str, "A]간=%lf초", duration );
     pDC->TextOut(512, 20, str);
}

/////////////////////////////////////////////////////////////////////////////
/7 CMyView printing


BOOL CMyView::OnPreparePrinting (CPrintlnfo* plnfo)
{
    II default preparation
     return DoPreparePrinting (plnfo);
}

void CMyView::OnBeginPrinting (CDC* /*pDC*/, CPrintlnfo* /*pln fo木7)
122 제］부 정전기학乍lectrostatics)



{
     II TODO: add extra initialization before printing
}

V아d （玉4yView: :OnEndPrinting (CDC永 /*pDC玎, CPrintlnfo永 /*이nfo水／)
{
     II TODO: add cleanup after printing
}

////////////////I///////III/I//I//////////////I///I////I/I/////I//I///////I//
II CMyView diagnostics


#ifdef _DEBUG
void CMyView::AssertValid() const
{
     CView::AssertValidO;
}

void CMyView::Dump (CDumpContext& dc) const
{
     CView: :Dump (dc);
}

CMyDoc* CMyView::GetDocumentO II non-debug version is inline
{
     ASSERT (mpDocument- >IsKindOf (RUNTIME_CLASS (CMyDoc)));
     return (CMyDoc*)m_pDocument;
}
#end迂 仄DEBUG


///////////////////////////////I///////////////////////////I////////////I///!
II CMyView message handlers
                                                               제4장 영상법（Method of 1mage) 123



double potential( double x, double xCenter, double charge, double r )
{
     double cosine, a, d;
     cosine = (x-xCenter)/r;
     a=100.0; d=289.0;
     return 8.98755E9半charge半（ 1.0/sqrt (r半r+d串d-2.0永r求d半cosine)
         - (a/d)/sqrt (r水r+ (a木a木a永a)I (d*d) -2.0水r串（a非aid）水cosine) );
}

4.3.3,. 프로그램 실행 결과


             따빌（L1   뜨 십（L   보 n{ y)   도g할（甘
              二 나日                 多 甲


                                               시 간＝4掘仁8000 초




             죤Hr                                                            HJM




4.4. 점전하와 반무한평면 유전체

4.4.1. 이론

    x< O에 해당되는 영역은 선형 등방 균질 유전체로 채워져 있다. 지금까지와는 달리 전위는 미리
124 저Ii부 정전7陣爬旭ctros怡tics)
                                                          \




정해져 있지 않다．
 진공 영역에서의 전위를 계산하기 위해서 section 2에서 그랬던 것과 같이 영상전하를 배치한다．
이번에는 곧바로 /=d을 가정한다. 그러면


                                                                                                    m
                                  d
                                                                                                                                         4)
                                                  口
                                  +                                                                                   '
                                                      나
                                                  J                                                              q
            砂진공 =                +                                             2                        T
                                                                                   八 ／H

                                                                                                            d)             y2+ z2
                                 )            ）
                                                                  기 U J
                                 H            日
                                                                                          \/(x+                  2+
을 얻으며 이로부터 전기장은

                                         工            d   \
                                                          1J
                                 +   （昕d)q                          口
                                                                    1
                                                                               , +                          佃＋d) q'               ,]     O
           E.Lm,콧U , =＝구니
                                                                               /
                                                                                    1




                                                                                   3
                                                                                   e2
                                                                               (
                       q7Ten l       d   9日               n(              nd
                                                                          2
                                                                               二
                                                                                                    +                             二 r
                          ' ( [(x- d)2+ y2+ z2] 2     U
                                                      V
                                                                                           [(x+ d)2+ y2+ z2] 2 ]
                                     \
                                     \
           万진공，
                                     J
             ＝그쓸，
                !                +
                                              q                                브+                                     q'          n      @
                                                  0
                                                  J

                                                                                   3
                                                                                   12                                               3
                                                                                                                                    e2
                                                              D
                                                              口           9
                                                                          q
                                                                          2                             T   d9
                                                                                                             日   +
                          " I [(x- d)2+ y2+ z2] 2                                                 口나나
                                                      U
                                                      U
                                                                                            [(x+ d)2+ y2+
                                                                                                                              9
                                                                                                                 \1/
                                                                                                                              r
임을 쉽게 구할 수 있다．
 유전체 영역에서의 전위를 계산하기 위해서는 위와 같이 배치된 전하들을 사용할 수 없다. 왜냐하
면 위와 같이 배치된 전하들을 사용하면 영상전하가 유전체 안에 위치하게 되는데, 영상법에서 영상
전하는 전위를 구하고자 하는 영역이 아닌 곳에 위치해야 하기 때문이다. 이 경우에는 많은 행운을
기대하면서 아래의 그림




에서 보는 바와 같이 하나의 영상전하 q"이 q 자신의 위치에 있다고 가정하자. 그러면 이 영상전하
에 의해1 유전체 내부에 발생되는 전위는
                                                                제4장 영상법（Method of Imag이 ]25



                    d)
                          '\


                         " 寸신세
                               口1 :.1   二＝
                                                       q
                                                           "
                                                                                         (2)
                                             4冗E0\/(T- d)2 + y2 + z2


이다. 이로부터 전기장은


                                                   (x- d)q"
                  E유전체：=                                          3
                                         471f。[(x- d)2+ y2+ z2] 2

                                                      yq"
                  万뉴전체y=                                          3
                                         4冗f。[(x- d)2+ y2+ z2] 2


임을 쉽게 구할 수 있다．
 이제 전기장의 성분들을 경계조건에 대입한다．
 x= O인 평면에서의 경계조건은


           I] · (진공1；진공- E유전체1：유전체） = 0万뉼공：-E万뉴전체：= 0                                   匈
                                         月진공y= 万유전체y                                    @
                                         E진공：= E유전체：                                    回

이다. 경계조건 匈어］ (5）와 (8）을 대입하면


                                   f。(- q+ q') = c (- q")


을 얻고, 경켸조컨 ＠어］ (6）과 (9）을 대입하면


                                              q + q' = q"

을 얻는다．

 +, = 毛임을 상기“'｝면' ], 위의 두 식을 연립“"｝여 풀면
126 제］부 정전기학（Electrostatics)




                                                                       q       '=




이다. 이것은 우리가 이 문제를 완전히 풀었다는 것을 의미한다．
 위의 두 식을 @）와 匣）에 대입하면 진공에서의 전위


                                                                                                                        凡CH          '
                                                                                1                                       也＋ l
                       砂진공 = 4읖， \/(x_ d)2+ y2+ z2                                                         \/ (x+ d)2+ y2+ z2
                                                                                                                                                      !




와 유전체 내부에서의 전위


                                                                                                  2q
                                                                                                 凡e+ 1
                                            r力1 n n1 ,.1 =
                                            '寸신"1                              4兀E。\/(X- d)2+ y2+ 22


을 얻는다．
  프로그램으로 구현하여 보자．
  물리좌표계에서 모니터 화면좌표계로 변환할 때 주의한다．
  유전체의 상대유전율（r이ative di이飢甘ic constant)은 3.4이고 전하의 크기는 4nC이다．
  화면 좌표계에서 전하의 위치는 (512, 600）이다．
  전위함수를 정의한다．


                                                                                184
    phi (x_ , y_) : = 巳98755 出                                                                            / ; y 5 580
                                                                                    .
                                                     [
                                                 V   (x       -   512) 2 + (y               -   600) 2


    phi (x_   《
                  y_   ] :.   8.   98755*   4*
                                                                                        1                                                ｝去                  I;   y ,. 580

                                                          V       (x       -   512) 2 + (y        -   600) 2   V   (x         -   512) 2 + (y   _   560) 2



  전위의 최대값을 구하기 위해 아래
                                                                  제4장 영상법（Method of Image) 127



     Max 口1ax (Tablefphi (x, y] , {x, 50, 1000} , {y, 50, 599} ]],
      Max (Table (phi (x, 600] , {x, 50, 511} ]] , Ma工 (Table (phi (x, 600) , {x, 513, 1000} ]] ,
      Max[Table[phi (x, y] , {x, 50, 1000} , {y, 601, 650} J] ]




와 같이 명령하고 전위의 최소값을 구하기 위해 아래


     Min (Min (Table (phi (x, y] , {x, 50, 1000} , {y, 50, 599} ]] ,
      Min[ Table (phi (x, 600] , {x, 50, 511} ]] , Min (TableLphi (x, 600) , 仁, 513, 1000} ]] 《
      Min[ Table (phi 江, y] , {x, 50, 1000} , (y, 601, 650} ]]]




와 같이 명령하면, 결과는 각각 35.4719, 0.022224이다．


4.4.2. Source Code

// 점전하와 반무한평면 유전체View.cpp : implementation of the CMyView class
II

#include "stdafx.h"
荊nc山de " 점전하와 반무한평면 유전체.h'


荊nclude " 점전하와 반무한평면 유전체Doc.h"
荊nclude " 점전하와 반무한평면 유전체피ew.h"


#include "math.h"


double phi [9511 [601] ;
double potentialDielectric ( double relativeDielectricConstant, double charge, double r );
double potentialVacuum( double relativeDielectricConstant, double charge, double r, double x,
                            double y );


#ifdef _DEBUG
#define new DEBUG그日EW
#undef THIS_FILE
static char THIS_FILE [1 = _FILE_;
    128 제］부 정전기학（Electrostatics)



    #endif


    /////////////////////I///////////////////////////////////////////////////////
    // CMyView
IMPLEMENT_DYNCREATE (CMyView, CView)


BEG爪_MESSAGE小MAP (CMyView, CV沌的
         II { {AFX_MSG_MAP (CMyView)
              II NOTE - the ClassWizard will add and remove mapping macros here.
              II      DO NOT EDIT what you see in these blocks of generated code!
         //} } AFX소ISG小4AP
        II Standard printing commands
         ON_COMMAND (ID_FILE_PRINT, CView::OnFjlePrint)
         ON_COMMAND (ID_FILE_PRINT_DIRECT, CView::OnFjlePrint)
         ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView::OnFilePrintPreview)
END1MESSAGE_MAP 0


/////////////////////////////////////////////////////////////////////////////
// CMyView construction/destruction


CMyView::CMyView 0
{
        /1 TODO: add construction code here


}

CMyView::싸CMyViewQ
{
}

BOOL CMyView::PreCreateWjndow (CREATESTRUCT& cs)
{
                                                                                제4장 영상법（M이hod of Image) 129



     II TODO: Modify the Window class or styles here by modifying
     II the CREATESTRUCT cs


     return CView::PreCreateWindow (cs);
}

/////////////////////////////////////////////////////////////////////////////
II CMyView drawing


void CMyView::OnDraw (CDC* pDC)
{
     CMyDoc* pDoc = GetDocument 0;
     ASSERT_VALID (pDoc) ;


     clock_t start, finish;
     double y, x, r, interval, max=35.4719, min=0.022224;
     double xPrime=512.0, yPrime=600.0, charge=4E- 9;
     double relativeDielectricConstant=3.4;
     double duration;
     char str[100] ;


     pDC->Rectangle ( 49, 49, 1001, 651 );
     CBrush Distribution (RGB (0,0,0));
     CBrush* pBrush;
     pBrush = pDC->SelectObject (&Distribution);
     pDC- >Rectangle (50, 50, 1000, 580);
     pDC->SelectObject (pBrush);


     pDC->MoveTo ( 油(xPrime) -5, mnt (yPrime) );
     pDC->LineTo ( mnt (xPrime) + 5, mnt (yPrime) );
     pDC卞>MoveTo ( mnt (xPrime), 奴 (yPrime) 小 );
     pDC->LineTo ( mnt (xPrime), jot (yPrime) + 5 );
130 저Ii부 정전기학（Hectrostatics)




   start = clock 0;


    for (y=50.0; y<651.0; y++)
       for (x=50.0; x<1001.0; x++)
        {
            r = sqrt ( (x-xPrime) * (x-xPrime) + (y-yPrime) * (y-yPrime));


            if ( (y<581.0) )
                  phi [int (x) -501 [int(y) -50]
                  = potentialDielectric ( relativeDielectricConstant, charge, r );
            이se if ( (x== xPrime）邑邑（y== yPrime) )
                  break;
            이se
                  ph小nt的H印］[mnt (y) -50]
                  ==potentialVacuum( relativeDielectricConstant, charge, r, x, y );
       }

   for (interval=max; interval>min; interval- = (max-mmn) /4000.0)
       for (y=50.0; y<651.0; y++)
            for (x=50.0; x<1001.0; x++)
            {
                  if ( (x==xPrime) &&(y==yPrime) )
                      break;


                  if ( (phi [m t (x) -50] [mnt (y) -501>interval-0.001)
                      && (phi [mnt (x) -501 [mnt (y) -501<interval+0.001) )
                      pDC->SetPixel( int (x), int (y), RGB(255, 0, 0) );
            }

   finish = clockO;
                                                                                제4장 영상법（M아hod of Image) 131



     duration = (double) (finish小 start) /CLOCKS_PER_SEC;


     pDC->SetTextAlign( TA_CENTER + TA_TOP);
     sprintf ( 5甘, "시간＝%lf초", duration );
     pDC->TextOut (512, 20, str);
}

/////////////////////////////////////////////////////////////////////////////
II CMyView printing


BOOL CMyView::OnPreparePrinting (CPrintlnfo* plnfo)
{
     II default preparation
     return DoPreparePrinting (plnfo);
}

void CMyView::OnBeginPrinting (CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     II TODO: add extra initialization before printing
}

void CMyView::OnEndPrinting (CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     II TODO: add cleanup after printing
}

/////////////////////////////I/I/////I///////////////////////////I///!///////
II CMyView diagnostics


#ifdef _DEBUG
void CMyView::AssertValidO const
{
    132 제］부 정전기학（Electrostatics)



         CView::AssertValid 0;
    }

    void CMyView::Dump (CDumpContext& dc) const
    {
         CView::Dump (dc);
    }

CMyDoc* CMyView::GetDocument0 I! non-debug version is inline
    {
        ASSERT (n匕pDocument ->IsKindOf (RUNTIMEHCLASS (CMyDoc))) ;
        return (CMyDoc* )nupDocument;
}
#endif ILDEBUG


//!///!/////!/!!///!//!!//////!!!!///!!///!!!!!!/!!!I!/!!!!!!!!/!!!!!/////!!!
I! CMyView message handlers


double potentialDielectric ( double relativeDielectricConstant, double charge, double r )
{
        double qPrimePrime;
        qPrimePrime = (2.아charge)!(r이麵ye미이ectricConstant+ 1.0) ;
        return 8.98755E9* (qPrimePrime!r);
}

double potentialVacuum( double relativeDielectricConstant, double charge, double r,
                                 double x, double y )
{
        double qPrime;
        qPrime = - ( (relativeDielectricConstant -1.0)! (relativeDielectricConstant + 1.0) ) *charge;
        return 8.98755E9
            * ( cJarge/r+qPrime!sqrt ((x-512.Q) 米(x-512.0) + (y-560.O) * (y-560.O) ) );
                                                       제4장 영상법（Method of Image) 133



}

443 프로그램 실행 결과


      i｝앞（已   딴집（LJ   보긔（y)   도묩말出）
      D 4 日            n1 好 !

                                      시 칸口03.37E000초




      준dr                                                         艸’NUKt
                              너i
                       벼d뇨m
                                    =
                                    d느
                              人丁
                               小
                                      법（Se附帥ono싸캐刊困



5.1, 이론

 구면좌표계에서 라플라스 방정식은


           1 a (느9c           ,     1      8 n뇨na砂＼ ,           1
                                                                         辛   0   (l)
          r乙 (7r \    orj         們sine, （兀F \      （兀F)   尸sin'0
                                                                         =
와 같이 된다. 문제를 간단히 하기 위해 砂7} 砂어］ 독립이라고 하자. 즉


                                         砂 = 砂（r, 0)


이면 d）은


                     8 ( 986 '\ .          1     8 / . ,, 86\       』＼
                     ==1mI r甘m六1 1 十 已已r ＝之＝I S1fl (／커寸＝=I = U
                      or \    or)    sinu （兀r \       O1)




가 된다. 우리는 아래


                                  砂 (r, 0) =R (r) r (0)                          (3)
136 제］부 정전기학（Electrostatics)



와 같이 단일변수 함수들의 곱의 형태로 된 해를 가정하여 (2）를 풀고자 한다．
 (3）을 (2）에 대입하면


                a     9,,=/n\ dR (r)      .        1    a       . ,.-., . dT(O
                --   rHi (I)    ,'日m + HHm=r=== S1flUK (T) _'1                                      =U,
                or       ' "   ar       sint' （大／      "     （及／

                m/ n\ d    9dR (r ')         . n/ \     1             d           . ,dT(O ')
                i (t' 尸--- r=1a日1        十itiriH      U== sint'
                  ' 'ar        ar             ' 'sinuau                                       at
                                                                                               '



 양변을 砂（r, 0) = R (r) T (0）로 나누면


                1     d    9    fl       .         1        1         d                . ,,    fl
              r-.I11 ,    rH   ,'        十 r1기 / ,l \ 1= === sint'                            小 '    =
              凡 나Jar           ar          i (t/ J siriu at'                                  at
                                                                                               '
                                                                                                          0,
                11므 r2          ( ) =                1 ＝느브 sinG브 ｛쓰
               R (기 dr         dr                   T(0) sin0 dO d0
                                                                                                               4)


 위 식에서 좌변 (left side）은 r만의 함수이고 우변（right side）은 0만의 함수이다. 위 식은 서로
다른 독립변수인 T과 0의 모든 값에 대해 항상 같아야 한다. 이것은 양변이 동일한 상수와 같을 때
에만 가능하다. 이 상수를 丸己｝ 하면



                                1, drd r 2d-쑤，.1 = 自
                               R(r)
                               붉    「'        dr   ()   丸R      (r)       =       0,
                          2겯染1 + r2브塑I브
                                    dr二
                                                                      丸R(r) = 0,
                                                                              "



 위의 미분방정식을 풀기 위해서 R（기 = cr1 꼴의 해를 시도해 보자. 여기에서 i은 상수이다．
 R（기 = cr을 위의 미분방정식에 대입하면


                      2r（岫卜1) + r2[ 내卜 1)尸긔 나c r드 0,
                                 [1(1+ 1 ) 十 丸］／코（기 = 0


 豆（r) = 0이면 모든 곳에서 c= 0인데 우리는 이것을 바라지 않으므로
                                          제5장 변수분리법（Separation of Variables) 137



                               丸 = /(/ + 1 )


임을 알 수 있다．
 위의 식은 @）의 우변과 같으므로


                       1  1 d . ,,         ( )   , , ..
                      T回 盂万而 Sl1lU        d0 ' = 八1十 1)


 이 책의 범위를 넘어서므로 더 이상의 과정은 생략하고 최종 결과만을 기술하면



                      砂（「汨）= 客 ［凡「'『윽］P1(cos이                                 (5)
이다. 여기에서 P,(cosO）는 아래


                              P。(cosO) = 1,
                             P1(cosO) = cosO,

                           P2佃詔）글（3co汁1)

와 같이 르장드르 다항식（Legendre's polynom洌）이다. c5）가 축대칭인 경우의 라플라스 방정식의
일반해（general solution）이다．



5.2. 균일한 전기마당 내의 접지된 도처규

5.2.1. 이론

 균일한 전기마당 파인 영역에 반지름이 a인 도체구를 넣고 접지시킨다. 도체구의 중심을 원점으

로 선택하고, z축을 전기마당의 방향으로 선택하자. 그러면 瓦＝月如이다．

 이 상황은 축태칭이므로 전위는 (5）로 주어진다．
 도체구의 내부에서 中 = 0이라는 사실은 독자가 잘 알고 있을 것이므로, 우리는 r> a인 영역에
138 저Ii부 정전기학（Eiectro없atics)



서 전위를 구하면 된다. 목적을 달성하기 위해서는 경계조건을 활용해야 한다．
 도체구의 표면에서 砂 = 0이므로，


                                      砂 (a, 0 ) = 0


위 식을 (5）에 대입하면



                          客［如'『윽戶佃삐印
을 얻는다. 자세한 논의는 생략하겠는데 위 식에서 괄호 안은 0이다. 따라서，


                                    弓＝- a2+1A1


이고, (5）는

                               的                』m 끄＋ l \
                      口（7, 0) = Z Ai
                                               （力           1 7-) /   /) \
                                                  1. m      Il- it CUSU I
                                                mm1寸＝ i
                                                          )i     ' \     /
                                                                             (6)
                               1= 0             I




가 된다．
 한편, 우리는 도체구의 존재 때문에 원래의 균일한 전기마당이 변하지만, 도체구에서 멀어질수록
전기마당은 원래의 균일한 전기마당과 가까워질 것이라고 예상할 수 있다. 식으로 나타내면


                                tim E(r,0) = Ez
                               r-   co




이다. 그런데 E=-v砂이므로 위의 식을 전위를 사용하여 표현하면


                          urn 中 (r, 9) =-E。   rcos0
                                          z=-E。


이다. 위의 식을 6）에 적용하면
                                                                제5장 변수분리법（Se口aration of Variables) 139



                                    m
                                    Z山 凡尸Pt ( cos 0) =1 万brcos 0 =     月0rPi (cos0)



 자세한 논의는 생략하고 최종 결과를 말하면


                                                         0+ " "万 2
                                                                bcos0
                                            的，9) =e月rcos
                                                                       T




이다. 위 식에서 첫째항은 바로 원래의 균일한 전키장을 나타낸다．
 프로그램으로 구현하여 보자．
 도체구의 중심은 (500, 350）이고 반지름은 50이다．
 Mathematica어］서 아래


                                    500)            350) 2
   r
       (x_   ,
                 y_   ] :=   /(x_
                                           2+ (y_

                                    x -500
   co ine (x1 ,y
            -    - ] :'             r (x, y]
                                                             125000 出94 士 coline ［工ry]
  phi[ x_ , y_] : =-94r ［毛 y] 士口oBine［工ry] +
                                                                     r (x, y] 2




와 같이 전위함수를 정의한 후 최대값을 구하기 위해 아래


  Max (Max (Table [phi [x, y] , {x, 50, 1000) , {y, 50, 300) ]] r
       Max[Table (phi (x, y] , {x, 50, 450) , {y, 301, 399) ]],
       Max[Table (phi (x, y] , {x, 550, 1000} , {y, 301, 399) ]] ,
       Max[Table (phi (x, y] , {x, 50, 1000) , {y, 400, 650) ]]]




와 같이 명령하고, 최소값을 구하기 위해 아래


  Min (Min (Table[phi[ x, y] , {x, 50, 1000) , {y, 50, 300) ]] ,
       Min (Table (phi (毛 y] , {x, 50, 450} , {y, 301, 399} ]] /
       Min (Table (phi (x, y] , {x, 550, 1000} , {y, 301, 399) ]] ,
       Min (Table (phi (x, y] , {x, 50, 1000) , {y, 400, 650) ]]]




와 같이 명령하면 각각 42266.6, -46970.4이다．
140 제］부 정전기학（Electra없카cs)




5.2.2. Source Code

// 균일한 전기마당 내의 접지된 도체구피ew.cpp : implementation of the CMyView class
II

#include Hstdafx .hu
荊nc加de "균일한 전기마당 내의 접지된 도체구．h'


荊nclude "균일한 전기마당 내의 접지된 도체구Doc.h"
荊nclude "균일한 전기마당 내의 접지된 도체구피ew.h"


#include <math.h>


double phi [9511 [6011;
double potential( double x, double y, double xCenter, double yCenter, double r, double a );


#ifdef _DEBUG
#define new DEBUG_NEW
#undef THIS_FILE
static char THIS_FILE [1 = _FILE_;
#endif


////////////////////I/////////I//////////////I/////I////////////I////I!//////
II CMyView

IMPLEMENT_DYNCREATE (CMyView, CView)


BEGIN_MESSAGE_MAP (CMyView, CView)
      /1{ {AFX_MSG_MAP (CMyView)
           II NOTE - the ClassWizard will add and remove mapping macros here.
           II      DO NOT EDIT what you see in these blocks of generated code!
                                                                  제5장 변수분리법（Se口aration of Variables) 141


      //} } AFX_MSG_MAP
     II Standard printing commands
      ON_COMMAND (ID_FILE_PRINT, CView::OnFjlePrint)
      ON_COMMAND (ID_FILE_PRINT_DIRECT, CView: :OnFilePrint)
      ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView::OnFilePrintPreview)
END_MESSAGE_MAP 0


/////////////////////////////////////////////////////////////////////////////
II CMyView construction/destruction


CMyView::CMy View 0
{
     /1 TODO: add construction code here


}

CMyView::사CMyView 0
{
}

BOOL CMyView::PreCreateWindow (CREATESTRUCT& cs)
{
     // TODO: Modify the Window class or styles here by modifying
     // the CREATESTRUCT cs


     return CView::PreCreateWindow (cs);
}

/////////////////////////////////////////////////////////////////////////////
1/ CMyView drawing


void CMyView: :OnDraw (CDC* pDC)
142 제］부 정전기학（Electrost帥cs)



{
    CMyDoc* pDoc = GetDocument 0;
    ASSERT_VALID (pDoc);


    clock_t start, finish;
    double xCenter=500.0, yCenter=350.0, a=50.0;
    double y, x, r;
    double interval, max=42266.6, min= -46970.4;
    double duration;
    char str [100];


    pDC->Rectangle ( 49, 49, 1001, 651 );


    CBrush Distribution (RGB (0,0,0));
    CBrush* pBrush;
    pBrush = pDC->SelectObject (&Distribution) ;
    pDC->Ellipse (450, 300, 550, 400);
    pDC->SelectObject (pBrush);


    start = clock 0;


    for (y=50.0; y<651.O; y++)
        for (x=50.0; x<1001.0; x++)
        {
            r = sqrt ( (x-xCenter) * (x-xCenter) + (y-yCenter) * (y-yCenter) );


            if ( r<a )
                 break;


            phi[int (x) -50] [int (y) -50] = potential( x, y, xCenter, yCenter, r, a );
        }
                                                                           제5장 변수분리법（Se口aration of Variables) 143


       f。
            r (interval=max; int붉val>        min;
                                                    interval- =    (max-
                                                                                mm.
                                                                                      ) /40.。)
              for (y=50.0; y<651.0; y++)
                  for (x=50.0; x<1001.0; x++)
                      {
                          r = sqrt ( (x-xCenter) * (x-xCenter) + (y-yCenter) * (y-yCenter) );


                          if ( r<a )
                              break;


                          if ( (phi [int(x) -50] [int(y) -50] >interval- (max-min) /1000.0)
                              &&(phi [int (x) -501 [int(y) -501<interval+ (max-min) /1000.0) )
                              if ( phi[int (x) -50] [int (y) -50] >0.0 )
                                     pDC->SetPixel( int (x), int (y), RGB(255, 0, 0) );
                              else if ( phi[int (x) -501 [int (y) -50] <0.0 )
                                     pDC->SetPixel( int (x), int (y), RGB(0, 0, 255) );
                              else
                                     pDC->SetPixel( int (x), int (y), RGB(255, 0, 255) );
                  }

      finish = clockO;


      duration = (double) (finish- start)/CLOCKS.YER..SEC;


     pDC- >SetTextAlign (T凡CENTER+ TA. TOP);
      sprintf( str, "시간＝%lf초", duration );
     pDC->TextOut (512, 20, str);
}

/////////////////////////////////////////////////////////////////////////////
// CMyView printing


BOOL CMyView::onPreparePrinting (CPrintlnfo* plnfo)
144 제］부 정전기학（Electro없atics)



{
     II default preparation
     return DoPreparePrinting (plnfo);
}

void CMyView::OnBeginPrinting(CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     II TODO: add extra initialization before printing
}

v아d CMyView::OnEndPrinting (CDC來 /*pDC玎, CPrintlnfo水 八pInfo米／)
{
     II TODO: add cleanup after printing
}

/////////////////////////////////////////////////////////////////////////////
II CMyView diagnostics


#ifdef _DEBUG
void CMyView::AssertValid() const
{
     CView::AssertValidO;
}

void CMyView::Dump (CDumpContext& dc) const
{
     CView::Dump (dc);
}

CMyDoc* CMyView::GetDocumentO II non-debug version is inline
{
     ASSERT (mmpDocument- >IsKindOf (RUNTIME_CLASS (CMyDoc)));
                                                                    제5장 변수분리법（Se口aration of Variables) 145



     return (CMyDoc*)n匕pDocument;
}
#endiI I/_DEBUG


IIIIIII/IIIIII/IIIIIIII/IIIII/IIIIIII/I/IIIIIII//IIIIIII//IIIIIIII/I/I/II/III
II CMyView message handlers


double potential( double x, double y, double xCenter, double yCenter, double r, double a )
{
     double fie1d0=94.0, cosine;
     cosine = (x-xCenter)/r;
     return 小1.0木fieldO水r永cosine+ (a米a米a半fieldO木cosine) /(r水r);
}

5.2.3. 프로그램 실행 결과


                 二 쯔 HnHJ 나r의 첩지된 도 41 1]   川넥口믐
                    파밉（E) 편口止） 보7Ky)   도욜맙叱）




                                                              1
                    口 呼日    n 亡 醫三 日    !
                r
                                                       시칸＝&e7ooo초




                    到
                                                              U
146 제］부 정전기학乍lectrostatics)




5.3. 균일한 전기마당 내의 유전체구

5.3.1. 이론

 균일한 전기마당 E。인 영역에 반지름이 口이고 대전되지 않은 유전체구를 넣는다. 이 문제의 경우
에 유전체구는 일정한 전위를 가지고 있지 않으며 유전체구 내부의 전위도 반드시 일정할 필요가 없
다. r> a인 경우와 r ＜二 口인 경우로 나누어 생각한다．
 이전의 section에서처럼 유전체구에서 멀어질수록 전기마당은 원래의 균일한 전기마당에1 가까워
질 것이다. 식으로 나타내면，


                               jim       。(r, O) =-E。rcos6
                              r나＋q)




 유전체의 표면은 유전체와 진공 사이의 불연속면이다. 유전체의 표면에서 전기마당의 접선성분
(tangential component) 과 전기변위（electric dis이配이Tient) 의 법선성분（normal component)은
연속이다. 이 경계조건을 전위를 사용하여 표현하면



                         日肆]r=ad냐染L,,
                         口！므으i)                  =                1 a白'
                                                      /
                                                      1
                         ( r 羽)
                                                                                1




                                                                  r 80
                                                      1
                                          , =a
                                                      1
                                                      1
 마지막으로 또 하나의 조건이 있다. 가정에 의하여 유전체구 내부에는 자유점전하가 존재하지 않
으므로 r= 0에서 砂7} 유한하다．
 이 책의 범위를 넘어서므로 중간 과정은 생략하고 모든 경계조건을 만족시키는 최종 결과만을 기
술하면



                      仇＝－蜘cosO+口，+-12 " "包"'" ,
                                白＝   2     /     3E0 2)
                                               /ce+       卜cos0
                                                                                          제5장 변수분리법（Se口a日tion of Variables) 147



 이다．
     이전의 section과 다른 상황은 같고 尻 , = 3이라고 하자．
     우선 Mathematica에서 전위함수를 아래


      r
              (x_
                            ,   yj    :=    I
                                                (x_
                                                          500) 2+ (y_ 350) 2
                                                          x -500
      口osine［毛고 y_ ] : =
                                                          r ［毛 yl
                                                      .
                                                                                      2   8000000* 94* oosine
                                                                                                                      y]
                                                            .     .      .   .    .
          .         .   .             .

      Pfl1LX_ , y_ j
                                                  n

                                           "= -y4* ELX, YJ *cos. ne1x, yj + = *                      .
                                                                                                                           .     .    .
                                                                                                                (x,
                                                                                                          . D
                                                                                                                                           nn八
                                                                                                                           /;   ELX, yj   >LVV
                                                                            -                      EL工 r yJ 1

                                                      3 * 94
      phi［工H,
                                     之］『’             二-        *r (x, y] ' 口osine (x, y] /; r ［毛 Yl 5 200



와 같이 정의한 후, 최대값을 구하기 위해 아래


      Max (Max[Table (phi (x, y] , {x, 50, 1000) , {y, 50, 349} ]] ,
       Max[Table (phi[ x, 350] , { x, 50, 499) ]] , Max (Table (phi[ x, 350] , {x, 501, 1000) ]] r
       Max[Tab1e (phi (x, y] , {x, 50, 1000) , {y, 351, 650) ]]]



와 같이 명령하고, 최소값을 구하기 위해 아래


      Min[Min[Table[phi (x, y] , {x, 50, 1000) , {y, 50, 349) ]] ,
       Min (Table (phi[ x, 350] , {x, 50, 499) ]], Min (Table[phi (x, 350] , {x, 501, 1000) ]]
                                                                                               ,
       Min (Table (phi (x, y] , {x, 50, 1000) , {y, 351, 650) ]]]



와 같이 명령하면 각각 41444.3, -46241.4이다．


5.3.2. Source Code

// 균일한 전기마당 내의 유전체구뀌ew.cpp : implementation of the CMyView class
//

#include "stdafx.h'1
#inc山de "균일한 전기마당 내의 유전체구．h'
148 저Ii부 정전기학（Electrost帥cs)



荊nclude "균일한 전기마당 내의 유전체구Doc.h"
荊nclude "균일한 전기마당 내의 유전체구뀌e\미1"


#include <math.h>


double phi [9511 [6011;
double potentialOut ( double x, double xCenter, double r, double radius );
double potentialln( double x, double xCenter, double r, double radius );
double fie1d0=94.0, cosine;


#ifdef _DEBUG
#define new DEBUG_NEW
#undef THIS_FILE
static char THIS_FILE [1 = _FILE_;
#endif


II/////////////////////////////////I/I/I/I/I//I/IIII/!I/I///I//I/I//I////////
II CMyView

IMPLEMENT_DYNCREATE (CMyView, CView)


BEGIN_MESSAGE_MAP (CMyView, CView)
     II { {AFX_MSG_MAP (CMyView)
           II NOTE 1 the ClassWizard will add and remove mapping macros here.
           II     DO NOT EDIT what you see in these blocks of generated code!
      //} } AFX_MSG_MAP
     II Standard printing commands
     ON_COMMAND (ID_FILE_PRINT, CView::OnFilePrint)
     ON_COMMAND (ID_FILE_PRINT_DIRECT, CView::OnFilePrint)
     ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView::OnFileprintpreview)
END_MESSAGE_MAP 0
                                                                  제5장 변수분리법（Se口aration of Variables) 149



/////////////////////////////////////////////////////////////////////////////
II CMyView construction/destruction


CMyView::CMyViewO
{
     // TODO: add construction code here


}

CMyView::사CMyView0
{
}

BOOL CMyView::PreCreateWindow (CREATESTRUCT& cs)
{
     II TODO: Modify the Window class or styles here by modifying
     1/ the CREATESTRUCT cs


     return CView::PreCreateWindow (cs);
}

/////////////////////////////////////////////////////////////////////////////
// CMyView drawing


void CMyView: :OnDraw (CDC* pDC)
{
     CMyDoc* pDoc = GetDocument 0;
     ASSERT_VALID (pDoc) ;


     clock_t start, finish;
     double xCenter=500.0, yCenter=350.0, radius=200.0;
     double y, x, r;
150 제］부 정전기학（Electrostatics)



   double interval, max=41444.3, min=-46241.4;
   double duration;
   char str [1001;


   pDC->Rectangle ( 49, 49, 1001, 651 );


   CBrush Distribution (RGB (0,0,0));
   CBrush* pBrush;
   pBrush = pDC小＞SelectO히ect（缸万str蜘tion);
   pDC->Ellipse(300, 150, 700, 550);
   pDC->SelectObject (pBrush);


   start = clockO;


   for (y=50.0; y<651.O; y++)
       for (x=50.0; x<1001.0; x++)
       {
           if ( (x= =xCenter) && (y==yCenter) )
                 break;


           r = sqrt ( (x-xCenter) * (x-xCenter) + (y -yCenter) * (y- yCenter) );


           if ( r>radius )
                 phi[int (x) -50] [int (y) -50] = potentialOut ( x, xCenter, r, radius );
           이se
           이Se
                 phi [mnt (x) -501 [mnt (y) -50] = potentialln ( x, xCenter, r, radius );



  for (interval=max; interval> =mmn; interval - = (max - mmn) /20.0)
      for (y=SO.O; y<651.0; y++)
           for (x=50.0; x<1001.0; x++)
           {
                                                                  제5장 변수분리법（Se口arat向n of Variables) 151



                       if ( (x==xCenter)&&(y==yCenter) )
                            break;


                       if ( (phi [mnt (x) -50] [mnt (y) -50] >interval- (max-mmn) /900.0)
                            &&(phi [int(x) -50] [int (y) -50] <interval+ (max-min)/900.0) )
                            if ( phi [int (x) -50] [int (y) -50] >0.0 )
                                  pDC->SetPixel( int (x), int (y), RGB(255, 0, 0) );
                            이se if ( ph小nt的小加］[mnt (y) -501<0.0 )
                                  pDC->SetPixel( int (x), int (y), RGB(0, 0, 255) );
                            eh祀
                                  pDC->SetPixel( int (x), int (y), RGB(255, 0, 255) );
                 }

      finish = clockO;


     duration = (double) (finish - start) /CLOCKS_PER. SEC;


     pDC->SetTextAlign (TA_CENTER+TA_TOP);
      sprintf ( str, "시간＝%lf초", duration );
     pDC->TextOut (512, 20, str);
}

/////////////////////////////////////////////////////////////////////////////
1/ CMyView printing


BOOL CMyView::OnPreparePrinting (CPrintlnfo* plnfo)
{
     II default preparation
     return DoPreparePrinting (plnfo);
}

void OMyView::OnBeginprinting (CDC木 八pDC町, CPrintlnfo木 八plnfo永／)
152 제］부 정전기학（Electro없atics)



{
     1/ TODO: add extra initialization before printing
}

void CMyView::OnEndPrinting(CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     II TODO: add cleanup after printing
}

/////////////////////////////////////////////////////////////////////////////
II CMyView diagnostics


#ifdef 1DEBUG
void CMyView::AssertValid() const
{
     CView::AssertValid 0;
}

void CMyView::Dump (CDumpContext& dc) const
{
     CView::Dump (dc);
}

CMyDoc* CMyView::GetDocument0 II non-debug version is inline
{
      ASSERT (mpDocument->IsKind0f (RUNTIME_CLASS (CMyDoc)));
     return (CMyDoc*)m_pDocument;
}
#end江 仄DEBUG


/////////////////////////////////////////////////////////////////////////////
II CMyView message handlers
                                                                제5장 변수분리법（Separation of Variables) 1 53



double potentialOut ( double x, double xCenter, double r, double radius )
{
    cosine = (x-xCenter)/r;
    return -1.0섀eldO朴札們ine+0.恥（(radius*radius串radi毗섀이dO托的ne)/(r*r));
}

double potentialln( double x, double xCenter, double r, double radius )
{
    cosine = (x-xCenter)/r;
    return -0.6串fieldO半r半cosine;
}

5.3.3, 프로그램 실행 결과


            41 i/ '= 냔 선 기n!'. ! 내 뉴쳔出 H   제 빅置늠
            따3HE) 편깁止） 보게Y) 도gmtU
            D 4 日       也 凸 !

                                                   시칸＝乞00札00초
                  전71n땅의 역선



6.1. 이론

 전기마당의 역선은 그 점에서의 전기마당의 방향의 접선으로 정의되므로, 만약 由7} 전기마당의
역선 위에서의 조그마한 변위라면 이것은 그 점에서의 전기마당과 방향이 같다. 식으로는


                            ds = kE,


로 표현할 수 있다. 여기에서 丸는 적당한 차원을 가진 비례상수（proportional constant)이다．
 우리는 위의 식을 사용하여 전기마당의 역선을 나타내는 미분방정식을 얻을 수 있다. 직교좌표계
에서 성분을 사용하여 위의 식을 나타내면


                dxx+ 啣y + dzz = 丸（月芬＋ 民y＋且미


이다. 따라서 , 직교좌표계에서 전기마당의 역선의 미분방정식은


                          쁘=뾰 =쁘
                          ／乞 E 且


가 된다．
156 제］부 정전기학（Electra없計ics)



 역선을 그리는 것은 등전위선을 그리는 것에 비해 간단하다. 여기서 간단하다는 말은 code의 길
이가 짧고, 실행시간도 훨씬 짧다는 것을 의미한다. 단순히 수학 함수의 그래프를 그리는 것과 다름
없기 때문이다．



6.2. 단일 점전하

 직교좌표계에서 단일 점전하에 의한 전기마당은


                       E(r= H뜨1:= q(x＋渤
                       H\ 1 4兀白R " 婉，伊寸）32

이다. 그러므로, 전기마당의 역선을 결정하는 미분방정식은




이고, 이 방정식을 풀면


                                   y = cx


을 얻는다. 직관적으로도 위의 풀이가 맞다는 것을 알 수 있을 것이다．



6.3. 쌍극자 전기마당

6.3.1. 이론

 쌍극자 마당의 전위는


                                         工）cos9
                             Vi八r ) ＝二 ;         2
                                       （士7fe0 'f
                                                                      제6장 전기마당의 역선   ] 57



이므로, 전기마당의 성분은



                           耳＋染十쉬' “영" ,
                           平수響十쉬뽁目
                                      斗韶＝               .


이고, 역선에 대한 미분방정식은


                      쁘二 1- 브－              프 - 2cos0       d(2lnsinO)
                       dO   rd0             月0 小 sinO           dO     '
                              .       dlnr -     d(21nsin0)
                                  "    dO            （羽


이다．
     위의 미분방정식의 양변을 적분하면 역선에 태한 방정식을 얻을 수 있다．


                        lnr= 2lnsinO+ lnKD= ln (KDsin20) ,

                                      .'. r= KDsin20


여기에서 瓦七 양의 적분상수(integration constant)이다．


6.3.2. Source Code

// 점쌍극자의 역선피ew.cpp : implementation of the CMyView class
II

#include "stdafx.h"
荊nclude " 점쌍극자의 역선.h'
158 제］부 정전기학（Electrostatics)


荊nclude " 점쌍극자의 역선Doc.h '
荊nclude " 점쌍극자의 역선View.h"


#include <math.h>


double x ( double r, double theta );
double y ( double r, double theta );


#ifdef _DEBUG
#define new DEBUG_NEW
#undef THIS_FILE
static char THIS_FILE [II = _FILE_;
#endif


/////////////////////////////////////////////////////////////////////////////
II CMyView

IMPLEMENT_DYNCREATE (CMyView, CView)


BEGIN_MESSAGE_MAP (CMyView, CView)
     II { {AFX_MSG_MAP (CMyView)
           II NOTE - the ClassWizard will add and remove mapping macros here.
           II      DO NOT EDIT what you see in these blocks of generated code!
      //} } AFX_MSG_MAP
     II Standard printing commands
      ON_COMMAND (ID_FILE_PRINT, CView::OnFilePrjnt)
      ON_COMMAND (ID_FILE_PRINT_DIRECT, CView::OnFilePrint)
      ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView::OnFilePrintPrevjew)
END_MESSAGE_MAP 0


/////////////////////////////////////////////////////////////////////////////
II CMyView construction/destruction
                                                                                제6장 전기마당의 역선   159



CMyView::CMyView ()
{
     II TODO: add construction code here


}

CMyView::사CMyView 0
{
}

BOOL CMyView::PreCreateWindow (CREATESTRUCT& cs)
{
     II TODO: Modify the Window class or styles here by modifying
     II the CREATESTRUCT cs


     return CView::PreCreateWindow (cs);
}

/I/////////////////I//////I//I////////I///I/I///I///I//I//I/////////I/I//////
I! CMyView drawing


void CMyView::OnDraw (CDC* pDC)
{
     CMyDoc* pDoc = GetDocument0;
     ASSERT_VALID (pDoc);


     double k, theta, r;
     const double pi 3.1415926535;


     CRect rect;
     pDC->SetMapMode (MM_LOMETRIC);
     GetClientRect (&rect);
160 제］부 정전기학（Electra없atics)



     pDC->SetViewportOrg (rect.Width O/2, rect.Height O/2) ;


     CPen myPen(PS_SOLID, 3, RGB(0,0,0));
     CPen串 p아dPen = pDC今Se扼야O히ect（幽까Pen) ;


      for (k=0.0; k<51000.0; k+=200.0)
           for (theta=0.0; theta<2.0*pi; theta+=pi/2000.0)
            {
                 r = k*sin(theta) *sin(theta);
                 pDC->SetPixel(int (x (r, theta) ), mnt (y (r, theta) ), RGB (0,0,0));
           }

     pDC- 兆이ectO岫Ct (p이dPen) ;
}

//////////////////////////////////I///////!/////!///////I/II///I////////!/!//
II CMyView printing


BOOL CMyView::OnPreparePrinting (CPrintlnfo* plnfo)
{
     /1 default preparation
     return DoPreparePrinting (plnfo);
}

void CMyView::onBeginPrinting(CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     II TODO: add extra initialization before printing
}

void CMyView::OnEndPrinting (CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     /1 TODO: add cleanup after printing
                                                                                제6장 전기마당의 역선 161



}

/////////////////////////////////////////////////////////////////////////////
II CMyView diagnostics


荊fdef DEBUG
void CMyView::AssertValid() const
{
     CView::AssertValidO;
}

void CMyView::Dump (CDumpContext& dc) const
{
     CView: Dump (dc);
}

CMyDoc* CMyView::GetDocumentO II non-debug version is inline
{
     ASSERT (rnpDocument- >IsKindOf (RUNTIMEeCLASS (CMyDoc)));
     return (CMyDoc*) mpDocument;
}
#endif I/_DEBUG


/////////////////////////////////////////////////////////////////////////////
II CMyView message handlers


double x ( double r, double theta )
{
     return r*cos (theta);
}

double y ( double r, double theta )
162 제］부 정전기학乍lectrostatics)




           return r*sin (theta) ;
) 1 1 J




          3
          6 n
            J
                프로그램 실행 결과


                    J+ 찹썸극工H4 낵신   찌목멉믐
                    파딤（E) 띤집上） 보7Hy) 도욥닫（L)
                     D 才모




6.4. 선형사중극자

6.4.1. 이론

          선형사중극자의 전위는


                                              人       Q      3cos20- 1
                                              yo-   =1:1        . .2
                                                "   （士7[Eo     4r니




이므로 전기마당의 성분은
                                                                  제6장 전기마당의 역선 163



                                       I크오）3co計0 十 1
                                       L37rE0) 2r4   '
                                         cos的n0
                                 ／可, 나르오）
                                   7   (   87rE0)          V4


                                                    瓦= 0


이고, 전기마당의 역선을 나타내는 미분방정식은


                                 dr        Er         3cos20- 1
                                rdO        E9         2cos0sin0


이다．
     위의 미분방정식의 양변을 적분하면 역선에 대한 방정식을 얻을 수 있다．


                                   r2= KQsin28cos6


여기에서 KQ는 적분상수이다．



6.4.2. Source Code

// 사중극자의 역선View.cpp : implementation of the CMyView class
II

#include "stdafx.h"
荊nclude " 사중극자의 역선.h'


荊nclude " 사중극자의 역선Doc.h"
荊nclude " 사중극자의 역선View.h"


#include <math.h>


double x ( double r, double theta );
164 제］부 정전7陣K티ectrosta如s)



double y ( double r, double theta );


#ifdef _DEBUG
#define new DEBUG_NEW
#undef THIS_FILE
static char THIS_FILE [1 = _FILE_;
#endif


/////////////////////////////////////////////////////////////////////////////
II CMyView

IMPLEMENT_DYNCREATE (CMyView, CView)


BEGIN_MESSAGE_MAP (CMyView, CView)
     II { {AFX_MSG_MAP (CMy View)
           II NOTE 1 the ClassWizard will add and remove mapping macros here.
           II      DO NOT EDIT what you see in these blocks of generated code!
     II)) AFX_MSG_MAP
     II Standard printing commands
      ON_COMMAND (ID_FILE_PRINT, CView::OnFilePrint)
      ON_COMMAND (ID_FILE_PRINT_DIRECT, CView::OnFilePrint)
      ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView::OnFilePrintPreview)
END_MESSAGE_MAP 0


/////////////////////////////////////////////////////////////////////////////
II CMyView construction/destruction


CMy View::CMy View 0
{
     II TODO: add construction code here


}
                                                                                제6장 전기마당의 역선   ]65



CMyView::사CMyView0
 {
}

BOOL CMyView::PreCreate Window (CREATESTRUCT& cs)
{
     II TODO: Modify the Window class or styles here by modifying
     II the CREATESTRUCT cs


     return CView::PreCreateWindow (cs);
}

/////////////////////////////////////////////////////////////////////////////
II CMyView drawing


void CMyView::OnDraw (CDC* pDC)
{
     CMyDoc* pDoc = GetDocument 0;
     ASSERT_VALID (pDoc);


     double k, theta, pi 3.1415926535, r;


     CRect rect;
     pDC->SetMapMode (MM_LOMETRIC);
     GetClientRect (&rect);
     pDC->SetViewportOrg (rect.Width O/2, rect.Height O/2) ;


     CPen myPen (PS_SOLID, 3, RGB (0,0,0));
     CPen* pOldPen = pDC->SelectObject (&myPen);


     for (k=0.0; k<20000000.0; k+=1000000.0)
          for (theta=0.0; theta<2.0*pi; theta+=pi/4000.0)
166 제］부 정전기학（Electrostatics)



           {
                r = sqrt ( k*sin (theta) *sin (theta) *cos (theta) );
                 pDC->SetPixel(int (x (r, theta) ), mnt (y (r, theta)), RGB (0,0,0));
                 pDC->SetPixel(-int (x (r, theta) ), mnt (y (r, theta)), RGB (0,0,0) );
           }

     pDC->S이e아Ob忙ct (p이dPen) ;
}

/////////////////////////////////////////////////////////////////////////////
II CMyView printing


BOOL CMyView::OnPreparePrinting (CPrintlnfo* plnfo)
{
     II default preparation
     return 11兀PreparePrinti旽 (p可o);
}

void CMyView::OnBeginPrinting (CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     II TODO: add extra initialization before printing
}

void CMyView::OnEndPrinting (CDC米 ／枉）DC玎, CPrintlnfo半 小plnfo半／)
{
     II TODO: add cleanup after printing
}

///////////////////////////////////////////////////////////I/////////////////
II CMyView diagnostics


荊fdef DEBUG
                                                                                제6장 전기마당의 역선 ] 67



void CMyView::AssertValidO const
{
     CView::AssertValid 0;
}

void CMyView::Dump (CDumpContext& dc) const
{
     CView: Dump (dc);
}

CMyDoc半 CMyView::GetDocument () II non-debug version is inline
{
     ASSERT (mHpDocument- >IsKindOf (RUNTIME_CLASS (CMyDocfl);
     return (CMyDoc*) nLpDocument;
}
#end汀 仄DEBUG


/////////////////////////////////////////////////////////////////////////////
II CMyView message handlers


double x ( double r, double theta )
{
     return r*cos (theta);
}

double y ( double r, double theta )
{
     retLirn r*sin (theta);
}
168 저Ii부 정전기학（Electrost카ics)




    3
    4
n
0
         쿠기램 실행 결과


           4二 시줌극챠엌 텍신      川목얹믐      答驀蔽
            i}3f)   면집止） 보기坦） 도묩弓出）
            D j     日   1   客 凸 !
기하광학（Geometrical Optics)
7.1. 이론

 구면의 일부가 반사면으로 된 거울을 구면거울（spherical mirror）이라고 하며 , 볼록거울（convex
mirror）과 오목거울（concave m卄ror）이 있다. 아래의 두 그림




                                                                   > > >
                           ]a
             0S
에서 구면의 중심 0를 구심, 거울면의 중심 M을 거울중심（center of mirror) , 구심과 거울중심을
지나는 직선을 거울축（axis of mirror）이라고 한다．
 오목거울의 반사면은 오목하다. 위의 왼쪽 그림과 같이 거울축에 나란하게 입사한 빛은 한 점 F에
모인다. 이 점을 초점 (focus）이라 하고 거울중심과 초점 사이의 거리를 초점거리 (local length）라고
한다．
 볼록거울의 반사면은 볼록하다. 위의 오른쪽 그림과 같이 거울축에 나란하게 입사한 빛은 반사 후
172 제2부 기하광학（Geometrical 야川cs)


에 반사면 뒤의 한 점 F에서 나온 것처럼 진행한다. 이 점을 볼록거울의 허초점臼irtual focal
point）이라고 한다，
 구면거울에 의해 생긴 물체의 상을 작도하려면 다음의 녜 가지 중에서 임의의 두 가지를 이용하면
된다．


(1) 거울축에 나란하게 입사한 광선은 오목거울의 경우에 반사 후 초점을 지나고, 볼록거울의 경우에
  허초점에서 나온 것 같이 진행한다．
(2) 초점을 지나거나 향하는 입사광선은 반사 후 거울축에 나란하게 진행한다．
(3) 구심을 지나거나 향하는 입사광선은 반사 후 온 길을 되돌아간다．
(4) 거울중심에서 반사하는 광선은 반사 후 거울축에 대하여 같은 각을 이룬다．


 물체 및 상에서부터 거울중심까지의 거리 , 초점거리를 각각 （工, b , ／라 하면


                                 1+           三／
                                      l
                                 a    下
                                                           (l)


이 성립한다．



7.2. 볼록거울（Convex Mirror)

7.2.1. 이론

 볼록거울의 경우 물체가 어느 위치에 있더라도 상은 항상 허초점과 거울중심 사이에 생기고 정립
허상이다. 배율佃a帥涵cation）은 1보다 작다．
 프로그램으로 구현하여 보자．
 구간 [0, 3000］의 실수축을 생각하자. 거울중심의 좌표는 1800이고 초점거리는 300이다. 물체
의 좌표를 x라 하면 G）은

                                          l
                           1800- i        b
                                          工
                                                   300 '
                                 b=   300 (18oo出
                                         2100 - 7
                                                                                                  졔7장 빛의 반사와 거울（Mirror) 173



7下 되는데 허상이므로 b< 0이다. 따라서 허상의 좌표는



                                           1800 -뇨1800+ 30二幣으, ' )
이고 배율은


                                                          b                        300
                                                                                 2l00出
                                                                                 2100- x KU
                                                      m= a
                                                         -=


 키보드의 日 key를 누르면 물체는 왼쪽으로 이동하고, 日 key를 누르면 오른쪽으로 이동한다．
key를 한 번 누를 때마다 물체의 위치 x는 10만큼씩 증가하거나 감소한다. 이것을 구현한 것이 "볼
록거울View.cpp" file의 OnKeyDown 함수인데 이 함수를 coding할 때에는 그냥 입력하면 안 되고
다음과 같은 과정을 따라야 한다．
 일단 "볼록거울View.cpp" file의 가장 밑으로 내려간다．
 그 다음에 View 메뉴의 하위메뉴를 보면 가장 위에 " ClassWizard... "이 있다. 이것을 선택하면 아
래의 화면


         田日e Em 小너 mon er뎌Oct                   u1d 和이1 뾰k겨出J나 小如

           會   4 日口        ,   b   屯     二 , 1二    町m臂      씨往pm小“如m小如' m크

         fcMwte.                 i汭I do. mcmbersZjPmmmnJ                                느盈   r뇌 台
                                   Jd겯      }

         博咨品集斗
               兮 1凶 Source Pu      比＝ooq. Mop,     1 Me.eborV.nl1blco 1 加-"I哨口0I 岫nXEccot.
                                                                                                                        1
                    固 MoinFe,
                    固 SI.iMx.I     甘미Cut                                 口nOB끼me;                   Md CI......     ,


                    m 묠폭거          啣H                               j    ! CMy'fle거r
                    由 블폭거
                                   C,.....묠폭거 恥쁠폭거 읕너t叫．九 C也，.1흩폭7{ 읕010cC上下P
                    m 블폭거
                    山 붙폭거          O叫ect ID,:                            U      1 en:
               李 m比. do, F카        付幽H;                                  七.IcwI。  如叩Cd
               等 ;JI뇨1nm口          bDOW ABOUT                            ;                             dli C.dc
                 Ji RoaM亡S                                               ! Del나mnAcnut斗DC


                                                                         凝，難轟'
                                   iID EDIT COPY
                                 ：蹉評課兀
                                   ID EDIT UNDO
                                   Member 加no油n1:
                                     V OnBegioPnIetbog
                                   1:V OnOn.甘
                                   iV OnEndPtlflOng
                                   :v OnPrrp.reb가1nOn므
         叫C뇨‘．
             ］茹Re... IJ            iV PreC,r. IeWInd口w


         去                         DC.口1P如n:

                                                                                             OK           Conucnb




         뇨m.       ，妃／的 , , ＼如． , .. , ,            } ＼加 ‘, .. , , :\.    ,,,   耐, ; ;
                                                                                                       In 138. C川 1         크 i尸 기
174 제2부 기하광학（Geom아rical 야川cs)



과 같이 "MFC ClassWizard" 대화상자가 나타난다．
     대화상자의 중간에 있는 Messages에서 "WM_KEYDOWN"을 찾은 후 " WMeKEYDOWN"을 더
블 클릭하여라. 그러면 "Men小er functions " 에 OnKeyDown 함수가 추가된다．
     그 다음에 "Edit Code " 버튼을 눌러라. 그러면 아래의 화면


            目 E曲 Edo I陀나 !n88n 므rD1日Ct 旦oil 10어8 對nd아／ H帥）

           「可畔 日1       工 宅1      f2!            已田람        뫄和r                                1卜 10

            !CUV1ew        LIIAlI d. ..me n.ber. j    小0口Key1}1U1                          크王11今 凶薑； !



                                        }
                                               lSSER1(l. p00CUmflt- ) IsKindlu(flm I旺_CLRSS (C向001) ));
                                               r. t.u.. (C51J0.c. ).p0. c.忙nt ;                                                                               코
                                        tendif // ethIC

                                        /I/ ///I/ iI/ //1H/ ///I/ I/ I/ /I/ I/ f/ f/ I/ //flf/   I/ I/ I/ !///////1/   I/ I/ !/I/ (/ I/ I/ !/I/
                                        // CI*joi. 口 m S0491 Ijodipro

                                        tild    tltjUiew::tnkept..n (UINT oCUlar, hINT ntepCnt. hINT tF1a1s)
                                        {


                                               C0i.t: :Sl eflNT(. Ch甘. tttpCnt, nrlags) ;
                                        }




            \；五｝i,Bu妃乂D的四 \F小d虹타餓L\                    日也虹F姮＄之＼Res냅넙                    j. J                                                                OF
            肛1小V                                                                                                                    I山140. C이｝    n」1n1   n吼mii




1!} 같이 "볼록거울View.cpp" file의 마지막에 OnKeyDown 함수가 추가된다．
     검은색으로 나타난 부분을 읽어 보아라. message handler code를 추가하라고 친절하게 안내를
해 준다. 필요한 source code를 이 곳에 입력하면 된다．
     한편, 방향 key를 누를 때마다 값이 변하는 변수 x는 "볼록거울View.h" 에서 변수 선언을 하고， "
볼록거울뀌ew.cpp " 에서 초기값을 지정한다. x는 물체의 위치를 나타내는 변수이다．


7.2.2. Source Code

U 볼록거울피e叫.h


// 볼록거울피이w.h : interface of the CMyView class
II
                                                                                제7장 빛의 반사와 거울的따아） 175



///////////////////////////////////////////////////////////////!/////////////

#if ! defined (AFX_VIEW_H16A056D4B_56 18_4 186_931D_50E9F796FB8C_INCLUDED_)
#define AFX_VIEW_FU6A056D4B_56 18_4 186_93 1D_50E9F796FB8C_JNCLUDED_


#11 _MSC_VER > 1000
#pragma once
#endif II JVISC_VER> 1000



class CMyView : public CView
{
protected: II create from serialization only
     CMyView 0;
     DECLARE_DYNCREATE (CMyView)


II Attributes
public:
     CMyDoc* GetDocument 0;


     dou바e x;


II Operations
public:


II Overrides
     II ClassWizard generated virtual function overrides
     II { {AFX_VIRTUAL (CMyView)
     public:
     virtual void OnDraw (CDC* pDC) ; /1 overridden to draw this view
     virtual BOOL PreCreateWindow (CREATESTRUCT& c s);
     protected:
176 제2부 기하광학（Geometric졔 Optics)



     virtual BOOL OnPreparePrinting (CPrintlnfo* plnfo);
     virtual void OnBeginPrinting (CDC* pDC, CPrintlnfo* plnfo) ;
     virtual void OnEndPrinting (CDC* pDC, CPrintlnfo* plnfo);
     //} } AFX_VIRTUAL


I/ Implementation
public:
     미rtual -'CMyView ();
#ifdef _DEBUG
     virtual void AssertValidO const;
     virtual void Dump (CDumpContext& dc) const;
#endif


protected:


II Generated message map functions
protected:
     //{{AFX_MSG(CMyView)
     afxjiisg void OnKeyDown(UINT nChar, UINT nRepCnt, UINT nFlags) ;
     I/} } AFX_MSG
     DECLARE.MESSAGE_MAP 0
};

＃汀ndef _DEBUG // debug version in 볼록거울View.cpp
inline CMyDoc* CMyView::GetDocument0
     { return (CMyDoc*)mpDocument; }
#endif


/I/I/IIII/I//II///III/IIIIIIIIIII///II/IIIIIII/IIIIII//III/IIIIIIII/IIII/I/I/

II { {AFX_INSERT_LOCATION} }
II Microsoft Visual C++ will insert additional declarations immediately before the previous
                                                                                제7장 빛의 반사와 거울（Mirror) 177


line.


#endif                                                                                                 II
!defined (AFX_VIEW_H_16A056D4B_56 18_4 186_93 1D_50E9F796FB8CJNCLUDED_)


臼 볼록거울피e叫.cpp


II 볼록거울View.cpp : implementation of the CMyView class
II

#include "stdafx.h"
荊nclude " 볼록거울．h'


荊nclude "볼록거울Doc.h"
荊nclude "볼록거울View.h"


#include <math.h>


#ifdef _DEBUG
#define new DEBUG_NEW
#undef THIS_FILE
static char THIS_FILE [] = _..FILE_;
#endif


///////////I////////////////////////////////////////////I////////////////////
II CMyView

IMPLEMENT_DYNCREATE (CMyView, CView)


BEGIN_MESSAGE_MAP (CMyView, CView)
     II { {AFX_MSG_MAP (CMyView)
      ON_WM_KEYDOWN 0
178 제2부 기하광학（Geometric계 0帥cs)



      //} } AFX_MSG_MAP
     II Standard printing commands
      ON_COMMAND (ID_FILE_PRINT, CView::OnFilePrint)
      ON_COMMAND (ID_FILE_PRINT_DIRECT, CView::OnFilePrint)
      ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView::OnFilePrintPreview)
END_MESSAGE_MAP 0


///////////////I/////////////////////////////////////////////////////////////
II CMyView construction/destruction


CMyView::CMyView0
{
      x = 0.0;
}

CMyView::사CMyView 0
{
}

BOOL CMyView::PreCreateWindow (CREATESTRUCT& cs)
{
     1/ TODO: Modify the Window class or styles here by modifying
     /1 the CREATESTRUCT cs


     return CView::PreCreateWjndow (cs);
}

/////////////////////////////////////////////////////////////////////////////
1/ CMyView drawing


void CMyView::OnDraw (CDC* pDC)
{
                                                         제7장 빛의 반사와 거울（M町아） 179



const double pi 3.1415926535;
double theta, a, b, m;
char buffer[10] ;


pDC->SetMapMode (MM_LOMETRIC);
pDC->SetViewportOrg(23, 400);


CPen myPen (PS_SOLID, 5, RGB (0,0,0));
CPen* pOldPen = pDC->SelectObject (&myPen);
pDC->MoveTo (0, 0);
pDC->LineTo (3000, 0);


for (theta= 2.0*pi/3.0; theta<4.0*pi/3.0; theta+ =pi/1000.0)
    pDC->SetPixel (2400+int (600.0*cos (theta) ), mnt (600.0*sin (theta)), RGB (0,0,0));


pDC- 冷毗ct아）ject (p이dPen) ;


CPen myPen2 (PS_SOLID, 9, RGB(0,0,0));
CPen卞 p이dPen2 = pDC- 兆毗Ct아）ject (&myPen2);
pDC->MoveTo (mnt (x) ,0);
pDC->LineTo (mnt (x) ,550);


a = 1800.0-x;
b = - (300.0* (1800.0-x)/(2100.0-xfl;
m = -(300.0/(2100.0-x));
pDC寸乂vloveTo（沁（1800나）) ,0);
pDC->LineTo (m t (1800-b) ,int (- 550.0*m));
pDC->SelectObject (pOldPen2) ;


pDC中> SetTextAlign ( TA_CENTER+TA_TOP);
sprintf (buffer, "m=%lf ', m);
pDC->TextOut (油(1800-b), -2, buffer);
180 제2부 기하광학（Geometric줴 0帥cs)



}

/////////////////////////////////////////////////////////////////////////////
II CMyView printing


BOOL CMyView::OnPreparePrinting(CPrintlnfo* plnfo)
{
     II default preparation
     return DoPreparePrinting (plnfo);
}

void CMyView::OnBeginPrinting (CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     II TODO: add extra initialization before printing
}

void CMyView::OnEndPrinting (CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     II TODO: add cleanup after printing
}

////I///I//I/II//III/II/II/I/I!//////II//I/I///I////II///I/I/////II///I///II/
II CMyView diagnostics


#ifdef _DEBUG
void CMyView::AssertValidO const
{
      CView::AssertVal jd 0;
}

void CMyView::Dump (CDumpContext& dc) const
{
                                                                                 제7장 빛의 반사와 거울（Mftror) 181



     CView::11沁mp (d이 ;
}

CMyDoc* CMyView::GetDocument0 II non-debug version is inline
{
      ASSERT (mHpDocument - >IsKindOf (RUNTIMEmCLASS (CMyDoc)));
     return (CMyDoc*)m_pDocument;
}
#end汀 仄DEBUG


///////////////////////////////////////////////////////////////'//////////////
II CMyView message handlers


void CMyView::OnKeyDown(UINT nChar, UINT nRepCnt, UINT nFlags)
{
     switch ( nChar )
      {
           case VK_LEFT:
                 x 叫＝ 10.0;


                 if ( x<O.0 )
                       x = 0.0;


                 break;


           case VK_RIGHT:
                 x += 10.0;


                 if ( x>1800.0 )
                       x = 1800.0;


                 break;
182 제2부 기하광학（Geometric졔 Optics)



               case VICESCAPE:
                          巴毗（ 1 );
      }

     Invalidate 0;


     CView::OnKeyDown (nChar, nRepCnt, nFlags);
}

723 프로그램 실행 결과


                                           q} 8  三上   i
     J i 日                                 그 4 日 r




    듣d1
                                      mN



    Ui   므二＝   7 1l시    1로d
                                           客S분
                                                          긔凹 도'VS
    J 8 日         出 !                                     니1 1




                                                                    (
                                                                        7
                                                                제7장 빛의 반사와 거울（Mirr아） 183




7.3. 오목거울（Concave Mirror)

7.3.1. 이론

 오목거울의 경우에는 아래의 표에서 보는 바와 같이 물체의 위치에 따라 상의 종류와 위치가 다양
하게 나타난다．


            물체                     상
            위치                     종류                            위치
            口 == cx                점                             b= f
            （刃 >     a ::> r       축소된 도립 실상                     f< b< r
            口 == r                 같은 크기의 도립 실상                  b= r
            r> a> f                확대된 도립 실상                     / < b < 以＞
               f                   상이 생기지 않는다                    (X)

            口< /
            a=
                                   확대된 정립 허상                     b< 0


 프로그램으로 구현하여 보자．
 구간 [0, 3000］의 실수축을 생각하자. 거울중심의 좌표는 1800이고 초점거리는 300이다. 물체
의 좌표를 x라 하면 d）은


                                     1     . 1           1
                                                 l
                                   1800- x ' b          300 '
                                            나e
                                                 下
                                       b= 300 (18oo- Z)
                                            1500 - 丁


가 되므로 허상의 좌표는


                               1800卜b= 1800          300 (1800누丁）
                                                       1500卜 丁


이고 배율은
184 제2부 기하광학（Geometric졔 0［川cs)



                                                   b     300
                                               m= - a= 1500- x


    "오목거울피텨w.cpp " 에서도 가장 마지막의 OnKeyDown 함수를 입력하려면 이전의 section에서
설명한 방법대로 해야 한다．


7.3.2. Source Code

d 오목거울미e叫. h


// 오목거울View.h : interface of the CMyView class
II
//I///////////////////!//////////////I////II///I///I////////I//////I/////I///

#if ! defined (AFXUVIEW_HH6F5B346C_50B1_405F_9B16_0B280D1B92D0_INCLUDED_)
#define AFX_VIEW_1-L6F5B3 4 6C_5OB1_405F_9B16_0B2 80D1B92D0_INCLUDED_


#if _MSC_VER > 1000
#pragma once
#endif II _MSC_VER > 1000



class CMyView : public CView
{
protected: II create from serialization only
      CMy View 0;
     DECLARE_DYNCREATE (CMyView)


II Attributes
public:
      CMyDoc* GetDocument0;
     double x;
                                                              제7장 빛의 반사와 거울（Mirror) 185



II Operations
public:


II Overrides
        II ClassWizard generated virtual function overrides
        //{{AF)LVIRTUAL(CMyView)
        pu1小C.
        virtual void OnDraw (CDC* pDC) ; II overridden to draw this view
        virtual BOOL PreCreateWindow (CREATESTRUCT& cs);
        protected:
        virtual BOOL OnPreparePrinting (CPrintlnfo* plnfo);
        virtual void OnBeginPrinting (CDC* pDC, CPrintlnfo* plnfo);
        미rtual vo沁 OnEndPrinting (CDC非 pDC, CPrintlnfo非 이nfo);
        II) } AFX_VIRTUAL


I/ Implementation
public:
        미rtual 사CMyView ();
#ifdef _DEBUG
        virtual void AssertValidO const;
        virtual void Dump (CDumpContext& dc) const;
#endif


protected:


II Generated message map functions
protected:
        II { {AFX_MSG (CMyView)
        afx_msg void OnKeyDown (UINT nChar, UINT nRepCnt, UINT nFlags) ;
        //} } AFX_MSG
        DECLARE_MESSAGE_MAP 0
}   ,
186 제2부 기하광학（Geometrical 야川cs)



荊fndef _DEBUG // debug version in 오목거울피ew.cpp
inline CMyDoc* CMyView::GetDocumentO
     { return (CMyDoc*)m_pDocument; }
#endif


/////////////////////////////////////////////////////////////////////////////

II { {AFX_INSERT_LOCATION} }
II Microsoft Visual C++ will insert additional declarations immediately before the previous
line.


#endif                                                                                   II
!de伽ed (AF乂YIEW_T-U_6F5B346C_50B1_如肝'_9B16_0B28이끄B92D0그NCLUDED_)


臼 오목거울피e出.cpp


// 오목거울피ew.cpp : implementation of the CMyView class
II

#include "stdafx.h'1
#include 1'오목거울．h


荊nclude " 오목거울Doc.h"
荊nclude "오목거울View.h"


#include <math.h>


#ifdef _DEBUG
#define new DEBUG_NEW
#undef THIS_FILE
static char THIS_FILE [1 = _FILE_;
#endif
                                                                                제7장 빛의 반사와 거울（Mirror) 187




////////////////////////////////////////////////////////////I////////////////
II CMyView


IMPLEMENT_DYNCREATE (CMyView, CView)


BEGIN_MESSAGE_MAP (CMyView, CView)
     II { {AFX_MSG_MAP (CMyView)
     O乂WM上EYDOWN 0
     //} } AFX_MSG_MAP
     // Standard printing commands
     ON_COMMAND (ID_FILEPRINT, CView::OnFilePrint)
     ON_COMMAND (ID_FILEPRINT_DIRECT, CView::OnFilePrint)
     ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView::OnFilePrintPrevjew)
END_MESSAGE_MAP 0


/////////////////////////////////////////////////////////////////////////////
II CMyView construction/destruction


CMy View::CMy View 0
{
     x = 0.0;
}

CMy View::사CMyView 0
{
}

BOOL CMyView::PreCreate Window (CREATESTRUCT& cs)
{
     /1 TODO: Modify the Window class or styles here by modifying
     /1 the CREATESTRUCT cs
188 제2부 기하광학（Geometrical 야川cs)



     return CView::preCreateWjndow (cs);
}

/////!///////////////////////I//////////////I/I/I/I/////////I//I////I/I//II/I
II CMyView drawing


void CMyView::OnDraw (CDC* pDC)
{
     CMyDoc* pDoc = GetDocument 0;
     ASSERT_VALID (pDoc);


     const double pi 3.1415926535;
     double theta, a, b, m;
     char buffer[10] ;


     pDC->SetMapMode (MM_LOMETRIC);
     pDC->SetViewportOrg(23, 400);


     CPen myPen (PS_SOLID, 5, RGB (0,0,0));
     CPen* pOldPen = pDC->SelectObject (&myPen);
     pDC->MoveTo (0, 0);
     pDC->LineTo (3000, 0);


     for (theta= -pi/3.0; theta<pi/3.0; theta+=pi/1000.0)
           pDC->SetPixel (1200+int (600.0*cos (theta)), mnt (600.0*sin (theta)), RGB(0,0,0));


     pDC->S이e아Object (p이dPen) ;


     CPen myPen2 (PS_SOLID, 9, RGB(0,0,0));
     CPen永 p이dPen2 = pDC小＞SelectO히ect（邑myPen2) ;
     pDC->MoveTo (mnt (x) ,0);
     pDC->LineTo (mlt (x) ,300);
                                                                                제7장 빛의 반사와 거울（Mirror) 189



     a = 1800.0-x;
     b = 300.아(1800.아x)/(1500.아x) ;
     m = 300.0/(1500.0-x) ;
     pDC->MoveTo (int (1800-b) ,0);
     pDC->LineTo (mnt (1800-b) ,int (- 300.0*m));
     pDC->SelectObject (pO!dPen2) ;


     if ( m<0.0 )
      {
           pDC->SetTextAlign ( TA_CENTER+TAUTOP);
           sprintf (buffer, "m=%lf", m);
           pDC->TextOut (mnt (1800-b), -2, buffer);
     }
     이se
      {
           pDC - >SetTextA1ign ( TA_CENTER+ TAHBOTTOM);
           sprintf (buffer, "m=%!f", m);
           pDC->TextOut (int (1800-b), 2, buffer);
     }
}

///III//I//////////I//!////I/////////////////////I//I//I//I//////////II//!/I/
II CMyView printing


BOOL CMyView::OnPreparePrmnting (CPrintlnfo* plnfo)
{
     1/ default preparation
     return DoPreparePrinting (plnfo) ;
}

void CMyView::OnBeginPrinting(CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
190 제2부 기하광학（Geometrical 0口tics)



     II TODO: add extra initialization before printing
}

void CMyView::OnEndPrinting(CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     II TODO: add cleanup after printing
}

/////////////////////////////////////////////////////////////////////////////
II CMyView diagnostics


#ifdef _DEBUG
void CMyView::AssertValid() const
{
     CView::AssertValid 0;
}

void CMyView::Dump (CDumpContext& dc) const
{
     CView::Dump (dc) ;
}

CMyDoc* CMyView::GetDocument0 II non-debug version is inline
{
     ASSERT (n匕pDocument - >IsKindOf (RUNTIME_CLASS (CMyDoc)));
     return (CMyDoc*) m_pDocument;
}
#end任 力IDEBUG


////////////////////////////////I///////I////I///////I//////I//I/////////////
/1 CMyView message handlers
                                                   제7장 빛의 반사와 거울（Mir띠r)   191



void CMyView::OnKeyDown (UINT nChar, UINT nRepCnt, UINT nFlags)
{
    switch ( nChar )
    {
        case VK1LEFT:
             x -= 10.0;


             if (x<0.0)
                    x 二二 0.0;


             break;


        case VKRIGHT:
             x += 10.0;


             if ( x>1800.0 )
                    x = 1800.0;


             break;


        case VK_ESCAPE:
             exit ( 1 ) ;
    }

    Invalidate 0;


    CView::onKeyDown(nChar, nRepCnt, nFlags);
}
192 제2부 기하광학（Geom아配궤 Optics)




733 프로그램 실행 결과


   日二 : n : 1   코   D LII勺         日1:1 rt. j 工／m 노   耳
   二 4 u            a !            J 1 可｛ n 屯 a !




                                   \
                                   \\

                               /
                               /
   11t1 텬勻U i, ;力 i! im1           1卞七 탄Hr =7K口 드ltd
  ，으따日 ’느 = y느1 !                  口 寸日 :1 已 }} 1 1
                뾔 굴절（Refra에on）
                             과렌즈（Lens)


8.1. 이론

 렌즈는 폭넓게 사용되는 광학부품으로 두 7가 이상의 굴절면으로 구성된 광학계이며 적어도 한 면
은 곡면이다．
 볼록렌즈의 중심은 가장자리보다 두껍고, 오목렌즈의 중심은 가장자리보다 얇다．
 렌즈에 의해 생긴 물체의 상을 그릴 때에는 다음의 서］ 가지 중에서 두 가지를 선택한다．


(1) 렌즈의 축에 나란하게 입사한 빛은 굴절 후, 볼록렌즈의 경우 초점을 지나고 오목렌즈의 경우 초
 점에서 나온 것처럼 진행한다．
(2) 렌즈의 중심을 지나는 빛은 그대로 직친한다．
(3) 렌즈의 초점을 지나는 빛이나 초점을 향하는 빛은 굴절 후 광축에 평행하게 나아간다．


 렌즈의 중심에서 물체 및 상까지의 거리 , 초점거리를 각각 (z, b, ／라고 하면


                       三+       l/
                            l
                        a   下
                                                        (D


가 성립한다. 실물체와 실상의 경우에는 각각 a> O, b> O이고 허물체와 허상의 경우에는 각각
a< O, b< O이다. 또한, 볼록렌즈의 경우에는 />0이고, 오목렌즈의 경우에는 /<0이다．
194 제2부 기하광학（Geomet叱계 이川cs)



 굴절율(index of refraction）이 n인 물질로 만들어진 얇은 렌즈（thin lens）의 곡률반경（radius
of curvature）이 r1, r2이면 초점거리 (focal length）는


                                                1
                                             . J1          . 1'
                               f=
                                       I'n 叫 I 기 11 十 1e 1
                                               \, r1   T2)



이다. 여기에서 n과 r2의 부호는 렌즈의 단면 중심에서 보아 볼록하면 ' + ' , 오목하면 '1' 로 한다．



8.2. 오목렌즈

8.2.1. 이론

 n= 1.5이고 rl = r2 =- 600인 경우에 초점거리는


                                             1
                    I    . -        . \(     1         .   1      \
                                                                      =-600
                         卜I)匕600 十1而히
                        (l "

이다．
 렌즈의 중심의 좌표가 2400이면 d）은


                                 1       1                   1
                                                   l
                               2400- x 1 b                  600 '
                                             J1
                                                   下
                                    b=       600 (240tJ_-x)
                                                3000 - 丁


이다．
 배율은


                                                    600
                                     77t =
                                                  3000- x
                                                                    제8장 빛의 굴절（Ref a에On）과 렌즈（Lens) 195




 8.2.2. Source Code

 U 오목렌즈피이v.h


 // 오목렌즈View.h : interface of the （沮4yView class
II
////////III///////III/////////////I/////I////I/////I//II///II//I/II//////I//I

 #if ! defined (AF)LVJEW_H. C0FC211B_33E4_4E13_88C1_7EB583811B96_INCLUDED_)
 #define AFX_VJEW_I-LC0FC211B_33E4_4E13_88C1_7EB583811B96_INCLUDED_


 #if _MSC_VER > 1000
 #pragma once
 #endif II _MSC_VER > 1000



class CMyView : public CView
 {
protected: II create from serialization only
     CMyView 0;
     DECLARE_DYNCREATE (CMyView)


II Attributes
public:
     CMyDoc* GetDocument 0;


     double x;


II Operations
public:
196 제2부 기하광학（Geometric히 야川cs)



II Overrides
      II ClassWizard generated virtual function overrides
      II { {AFX_VIRTUAL (CMy View)
      put小C.
      virtual void OnDraw (CDC* pDC) ; II overridden to draw this view
      virtual BOOL PreCreateWindow (CREATESTRUCT& cs);
      protected:
      virtual BOOL OnPreparePrinting (CPrintlnfo* plnfo);
      미rtual vU沁 OnBeginPrinting (CDC串 pDC, CPrintlnfo半 이nfo);
      Virtual void OnEndPrinting (CDC* pDC, CPrintlnfo* plnfo);
      /I} } AFX_VIRTUAL


I/ Implementation
public:
      미rtual 시CMyView ();
荊fdef 叫DEBUG
      virtual void AssertValidO const;
      virtual void Dump (CDumpContext& dc) const;
 #endif


 protected:


II Generated message map functions
 protected:
       //{ {AFX小心이아fly피ew)
       afx_msg void OnKeyDown(UINT nChar, UINT nRepCnt, UINT nFlags) ;
       //}}AFX_MSG
       DECLARE_MESSAGE_MAP 0
 };

 荊fndef _DEBUG // debug version in 오목렌즈피ew.cpp
 inline CMyDoc木 아打뀌ew::Ge山ocum帥tO
                                                                    제8장 빛의 굴절（Ref a에on）과 렌즈（Lens) 197


     { return (CMyDoc*)m_pDocument; }
#endif


//IIII////////I//I/////////I//////I/I////I!I///////////I/II/!I/II/I/I////////

II { {AFX_INSERT_LOCATION} }
II Microsoft Visual C++ will insert additional declarations immediately before the previous
line.


#endif                                                                                             II
!defined (AF乂－VIEW_H__C0FC211B_33E4_4E13_88C1_7EB583811B96_INCLUDED_)


a 오목렌즈피e叫.cpp


// 오목렌즈뀌ew.cpp : implementation of the CMyView class
II

#include "stdafx.h"
荊nclude " 오목렌즈．h


荊nclude "오목렌즈Doc.h"
荊nclude " 오목렌즈피ew.h '


#include <math.h>


#ifdef _DEBUG
#define new DEBUG_NEW
#undef THIS_FILE
static char THIS_I江LE [] = H巾Fli卞1
#endif


///////////////////////////////////I/I////I/////!I//I////////I/II////////////
198 제2부 기햐광학（Geom아nc비 0帥cs)



II CMyView


IMPLEMENT_DYNCREATE (CMyView, CView)


BEGIN_MESSAGE_MAP (CMyView, CView)
     II { {AFX_MSG_MAP (CMyView)
     ONHWMHKEYDOWN 0
     II) } AFX소4SG_MAP
     II Standard printing commands
     ON_COMMAND (ID_FILE_PRINT, CView::OnFilePrjnt)
     ON_COMMAND (ID_FILE_PRINT_DIRECT, CView: :OnFilePrint)
     ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView::OnFilePrintPreview)
END_MESSAGE_MAP 0


/////////////////////////////I///////////////////////////////////////////////
II CMyView construction/destruction


CMyView::CMyView0
{
     x = 0.0;
}

CMyView::사CMyView0
{
}

BOOL CMyView::PreCreate Window (CREATESTRUCT& cs)
{
     /1 TODO: Modify the Window class or styles here by modifying
     1/ the CREATESTRUCT cs


     return CView::다eCreateWjndow (cs);
                                                                   제8장 빛의 굴절（Ref ra帥on）과 렌즈（Lens) 199



}

////////////I////////////////////////////////////////////////////////////////
II CMyView drawing


void CMyView::OnDraw (CDC* pDC)
{
     CMyDoc* pDoc = GetDocument 0;
     ASSERT_VALID (pDoc) ;


     const double pi=3.1415926535;
     double theta, a, b, m;
     char buffer[10] ;


     pDC->SetMapMode (MM_LOMETRIC);
     pDC->SetViewportOrg (23, 400);


     CPen myPen (PS_SOLID, 5, RGB (0,0,0));
     CPen* pOldPen = pDC->SelectObject (&myPen);
     pDC->MoveTo (0, 0);
     pDC->LineTo (3000, 0);


     for (theta= 2.0*pi/3.0; theta<4.0*pi/3.0; theta+ =pi/1000.0)
           pDC->SetPixel(3000+ mnt (600.0*cos (theta) ), mnt (600.0*sin (theta) ), RGB (0,0,0));


     for (theta= -pi/3.0; theta<pi/3.0; theta+ =pi/1000.0)
           pDC->SetPixel (1800+int (600.0*cos (theta)), mnt (600.0*sin(theta)), RGB (0,0,0));


     pDC->MoveTo (1800+int (600.0*cos (pi/3.0)), int (600.0*sin (pi/3.0) fl;
     pDC->LineTo (3000+int (600.0*cos (2.0*pi/3.0)), int (600.0*sin (2.0*pi/3.0) fl;
     pDC今MoveTo (1800쉬nt (600.아凹S（가)i/3.0)), int (600.0米sin(-pi/3.0)));
     pDC->LineTo (3000+int (600.0*cos (4,0*pi/3.0) ), mnt (600.0*sin (4.0*pi/3.0)));
200 제2부 기하광학（Geom아nc키 야川cs)



     pDC- 冷이e아Object (p이dPen) ;


     CPen myPen2 (PS_SOLID, 9, RGB(0,0,0fl;
     CPen米 p이dPen2 = pDC->SelectO可ect（邑myPen2) ;
     pDC->MoveTo (mnt (x) ,0);
     pDC->LineTo (mlt (x) ,550) ;
      a = 2400.0-x;
     b = -(600.0* (2400.0- x)/(3000.0-x));
     m = -(600.0/(3000.0-x));
     pDC->MoveTo (mnt (2400+b) ,0);
     pDC->LineTo (mnt (2400+b) ,int (- 550.0*m));
     pDC- 兆이e아O岫Ct (p이dPen2) ;


     pDC->SetTextAlign ( TAeCENTER+TAJOP);
     sprintf (buffer, "m=%lf", m);
     pDC->TextOut (mnt (2400+b), -2, buffer);
}

/I////////////////I!////////////I/////////////////////I/I////////////////I///
II CMyView printing


BOOL CMyView::OnPreparePrinting (CPrintlnfo* plnfo)
{
     // default preparation
     return DoPreparePrinting (plnfo);
}

void CMyView::OnBeginPrinting (CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     II TODO: add extra initialization before printing
}
                                                                    제8장 빛의 굴절（Refraction）과 렌즈（Lens) 201



void CMyView::OnEndPrinting(CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
 {
     II TODO: add cleanup after printing
}

///////////////////////////////////I/////////////////////////////////////////
II CMyView diagnostics


#ifdef _DEBUG
void CMyView::AssertValid() const
{
      CView::AssertValidO;
}

void CMyView::Dump (CDumpContext& dc) const
{
     CView::Dump (dc);
}

CMyDoc* CMyView::GetDocument () II non-debug version is inline
{
     ASSERT (mpDocument - >IsKindOf (RUNTIMEmCLASS (CMyDoc)));
     return (CMyDoc*)nLpDocument;
}
#endif I/_DEBUG


////////////////I//I//I////I/I////////////////////////I////I////I////I///////
II CMyView message handlers


void CMyView::OnKeyDown (UINT nChar, UINT nRepCnt, UINT nFlags)
{
     switch ( nChar )
202 제2부 기하광학（Geometric졔 0帥cs)




    {
        case VK_LEFT:
             x m= 10.0;


             if (x<0.0)
                    x = 0.0;


             break;


        case VK_RIGHT:
             x += 10.0;


             if ( x>2400.0 )
                    x = 2400.0;


             break;


        case VK_ESCAPE:
             ex奴 1 );
    }

    Invalidate 0;


    CView::OnKeyDown (nChar, nRepCnt, nFlags);
}
                                         제8장 빛의 굴절（Ref ra에on）과 렌즈（Lens) 203




8.2.3. 프로그램 실행 결과


    U                                      a,




8.3. 볼록렌즈

8.3.1. 이론

 n= 1.5이고 rl = r2 = 600인 경우에 초점거리는


                                  1
                                                  = 600
                   戶＝
                                / 1    』 1 '\
                        (1.5- 1) ＝二＝= 十 ==== 1
                                \\UuU    tDUU J
204 제2부 기하광학（Geom아肥al 야캐cs)



이다．
    렌즈의 중심의 좌표가 1800이면 d）은


                                           l801
                                           18。。-, 나나可）
                                           ／· 뇨 60＝嘴으Hx' )
이다．
    배율은


                                                          600
                                                  171 = 1200- i


8.3.2. Source Code

a 볼록렌즈피e出.h


// 볼록렌즈피ew.h : interface of the CMyView class
//
///////////////////////////////////////////I////////I//I///!//////////I//////

#if ! defined (AF) 中VIEW_FL]E414DB5_DCB6_4E7E_A2E8_5F781C766DFF_INCLUDED_)
#define AFX_VIEW_FL=7E4 14DB5_DCB6_4E7E_A2E8_5F78 1C766DFF_INCLUDED_


#if _MSC_VER > 1000
#pragma once
#end迂 // eMS（二VER > 1000



class CMyView : public CView
{
                                                 제8장 빛의 굴절（Refraction）과 렌즈（Lens) 205



protected: II create from serialization only
    CMyView0;
    DECLARE_DYNCREATE (CMyView)


// Attributes
public:
    CMyDoc* GetDocument 0;


    double x;


II Operations
public:


II Overrides
    II ClassWizard generated virtual function overrides
    II { {AFX_VIRTUAL (CMyView)
    public:
    virtual void OnDraw (CDC* pDC); II overridden to draw this view
    virtual BOOL PreCreateWindow (CREATESTRUCT& cs) ;
    protected:
    virtual BOOL OnPreparePrinting(CPrintlnfo* plnfo);
    virtual void OnBeginPrinting (CDC* pDC, CPrintlnfo* plnfo);
    virtual void OnEndPrinting (CDC* pDC, CPrintlnfo* plnfo);
    //} } AFX_VIRTUAL


I/ Implementation
public:
    미rtual 사CMyView ();
#ifdef _DEBUG
    virtual void AssertValidO const;
    미rtual void Dump (CDum可二ontext邑 dc) const;
#endif
206 제2부 기하광학（Geometric계 (:）口tics)



pr아ected:


II Generated message map functions
protected:
        II { {AFX_MSG (CMy View)
        afx_msg void OnKeyDown(UINT nChar, UINT nRepCnt, UINT nFlags);
        //} } AFX_MSG
        DECLARE_MESSAGE_MAP 0
};
荊fndef _DEBUG // debug version in 볼록렌즈View.cpp
inline CMyDoc* CMyView::GetDocument0
     { return (CMyDoc*)m_pDocument; }
#end江


////////////////////!///////I/I/////I/////I//////I//I/I/////I/!////////I/////

//{{AFX_INSERT_LOCATION} }
II Microsoft Visual C++ will insert additional declarations immediately before the previous
line.


#endif                                                                                   II
!defined (AFX_VIEW코_ 7E4 14DB5_DCB6_4E7E_A2E8_5F781C766DFF_INCLUDED_)


a 볼록렌즈피ew.c口口


// 볼록렌즈피ew.cpp : implementation of the CMyView class
II

#include 'stdafx.h1'
荊nclude "볼록렌즈.h
                                                                   제8장 빛의 굴절（Refraction）과 렌즈（Lens) 207



荊nclude " 볼록렌즈Doc.h"
#include "볼록렌즈뀌ew.h"


#include <math.h>


#ifdef _DEBUG
#define new DEBUG_NEW
#undef THIS FILE
static char THIS_FILE [I = _FILE__;
#endif


I/////////////////////////////////////////////////!//////////////////////////
II CMyView


IMPLEMENT_DYNCREATE (CMyView, CView)


BEGIN_MESSAGE_MAP (CMyView, CView)
     I! { {AFX_MSG_MAP (CMyView)
      ON_WM1KEYDOWN 0
      //} } AFX_MSG_MAP
     II Standard printing commands
      ON_COMMAND (ID_FILE_PRINT, CView::OnFjlePrint)
      ON_COMMAND (ID_FILE_PRINT_DIRECT, CView::OnFilePrint)
      ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView::OnFilePrjntPrevjew)
El町兀MESSAGE_MAP 0


/////////I//////////////!/////////!////!////////////////////I////////////////
II CMyView construction/destruction


CMyView::CMyView0
 {
      x = 0.0;
208 제2부 기하광학（GeometrcaI 야川cs)




}

CMyV妃＼V.：사CMyView 0
{
}

BOOL CMyView::PreCreateWindow (CREATESTRUCT& cs)
{
     II TODO: Modify the Window class or styles here by modifying
     II the CREATESTRUCT cs


      return CView::preCreateWindow (cs);
}

///II///I//I/I////I/I/I/I/IIII///I/////III/II//I/I/II/I/I/I/II/I/I////I//I//I
II CMyView drawing

void CMyView::OnDraw (CDC* pDC)
 {
      CMyDoc* pDoc = GetDocument 0;
      ASSERT_VALID (pDoc);


      const double pi 3.1415926535;
      double theta, a, b, m;
      char buffer[10] ;


      pDC->SetMapMode (MM_LOMETRIC);
      pDC->SetViewportOrg (23, 400);


      CPen myPen(PS_SOLID, 5, RGB(0,0,0));
      CPen* pOldPen = pDC->SelectObject (&myPen);
      pDC->MoveTo (0, 0);
                                                       제8장 빛의 굴절（Ref ra에on）과 렌즈（Lens) 209


    pDC->LineTo (3000, 0);


    for (theta=2.0*pi/3.0; theta<4.0*pi/3.0; theta+=pi/1000.0)
             pDC->SetPixel (2400+int (600.0*cos (theta)), mnt (600.0*sin (theta)), RGB(0,0,0fl;


    for (theta= -pil3.0; theta<pi/3.0; theta+ =pi/1000.0)
             pDC->SetPixel(1200+int (600.0*cos (theta)), mlt (600.0*sin (theta)), RGB (0,0,0));


    CPen myPen2(PS_SOLID, 9, RGB(0,0,0));
    CPen* p01dPen2 = pDC->SelectObject (&myPen2);
    pDC->MoveTo (mnt (x) ,0);
    pDC->LineTo (mnt (x) ,300);
    a = 1800.0-x;
    b == (600.아（1800.아x)/(1200.아x));
    m = 600.0I(1200.0-x);
    pDC->MoveTo (m t (1800-b) ,0);
    pDC- 乂ineTo（沁（1800나)) ,int (-300.아向）;
    pDC- 冷이ect（가永Ct (p이dPen2) ;


    if ( m<0.0 )
         {
             pDC->SetTextAlign( TA_CENTER+TA_TOP);
             sprintf (buffer, "m=%lf", m);
             pDC->TextOut (奴 (1800-b), -2, buffer);




             pDC- >SetTextA1ign ( TA_CENTER+ TA_BOTTOM);
             sprintf (buffer, "m %川, m);
             pDC->TextOut (mnt (1800-b), 2, buffer);
    ).
}
210 제2부 기하광학（Geome毗al 야川cs)



/////////////////////////////////////////////////////////////////////////////
// CMyView printing


BOOL CMyView::OnPreparePrinting (CPrintlnfo* plnfo)
{
     II default preparation
     return DoPreparePrinting (plnfo) ;
I

void CMyView::OnBeginPrinting (CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     II TODO: add extra initialization before printing
I

void 아/IyView::OnEndPrinting (CDC串 八pDC玎, CPrintlnfo木 小plnfo木／)
{
     II TODO: add cleanup after printing
I

/////////////////////////////////////////////////////////////////////////////
II CMyView diagnostics


#ifdef _DEBUG
void CMyView::AssertValid 0 const
{
      CView::AssertValid 0;
I

void CMyView::Dump (CDumpContext& dc) const
{
      CView::Dump (dc) ;
}
                                                                   제8장 빛의 굴절（Refraction）과 렌즈（Lens) 211



CMyDoc* CMyView::GetDocument0 1/ non-debug version is inline
{
     ASSERT (mHpDocument- >IsKindOf (RUNTIMEHCLASS (CMyDoc) fl ;
     return (CMyDoc*)m_pDocument;
}
#endif I/_DEBUG


////////////////////////////////////////////////////////////////////////I////
II CMyView message handlers


void CMyView::OnKeyDown(UINT nChar, UINT nRepCnt, UJNT nFlags)
{
     switch ( nChar )
      {
           case VK_LEFT:
                 x -= 10.0;


                 if (x<0.0)
                       x 二二 0.0;


                 break;


           case VK_RIGHT:
                 x += 10.0;


                 if ( x>1800.0 )
                      x = 1800.0;


                 break;


           case VK_ESCAPE:
                 exit ( 1 ) ;
212 제2부 기하광학（Geom아nc칡 0［川cs)



    }

    Invalidate 0;


    CView::OnKeyDown(nChar, nRepCnt, nFlags);
}

8.3.3. 프로그램 실행 결과


                                         므1:B r= L   !1士 노nmdJ
    口 畔U          1   T                  그 4 日        그 1 !




                          r
                              V

    1r二qr   r＝山 !J 小 i                   11i] 탄令U = 竹 5     4
                                         J 甘
                                             日t二스立 !




                              A
                                                                 少i如
기초적인 3차원 컴퓨터 그래떡
9.1, 개론

 기본적으로 컴퓨터 모니터는 2차원 평면이지만 실세계의 물체를 나타내기 위해서는 세 개의 좌표
가 필요하다. 따라서 서］ 개의 좌표를 어떻게 두 개의 좌표로 줄일 것인지가 관건이 된다. 사람들은
오래전부터 이것에 대해 연구하였다. 이렇게 3차원 입체를 평면상에 나타내는 것을 투영
(pr이ection）이라 한다．
 투영의 한 예로, 우리가 살고 있는 지구（earth）를 평면에 나타낸 지도를 생각해 볼 수 있다. 아래
의 두 그림들




     입 체투영 (stereographic
                            Trystan Edwards cylindrical 투
     pr이ection)
216 제3부 기초적인 3차원 컴퓨터 그래픽



은 다른 방법으로 투영한 지도를 나타낸다. 위의 그림들과 같이 동일한 입체라도 여러 가지 방법으
로 투영할 수 있고 결과적으로 우리가 보게 되는 것들은 다른 모습틀을 띤다．
 컴퓨터 그래픽에 사용되는 투영에는 평행투영（parallel pr이ection）과 원근투영（perspect如e
pr이ection）이 있다．
 평행투영은 투영의 중심（center of pr이ection）이 무한히 먼 곳에 위치해 있어 모든 투영선들이
서로 평행한 투영이고, 원근투영은 아래의 그림




과 같이 투영의 중심이 투영면으로부터 유한한 거리에 위치해 있는 투영이다．
 평행투영은 경사투영과 직교투영으로 나뉜다. 경사투영은 아래의 그림
                                          제9장 3차원 입체의 구현 217



과 같이 투영선들이 투영면（projection 이ane）에 대해 경사져 있는 것이고, 직교투영은 아래의 그림




과 같이 투영선들이 투영면에 대해 직교하는 것이다．
 우리가 이 책에서 3차원 컴퓨터 그래픽을 구현하기 위해서 공부할 것은 평행투영이다．
 독자는 이 책에서 공부하고자 하는 것들은 어디까지나 3차원 컴퓨터 그래픽에서 기초적인 단계라
는 것을 알아 두어라. 하지만 앞으로 공부할 것들만 익혀도 여러 곳에서 상당히 유용하게 사용할 수
있을 것이다．
 예를 들어 , 제2부 기하광학에서 공부하였던 프로그램들에서 물체는 모두 가느다란 선（line）이었
다. 제3부에서 공부할 내용들을 이용하면 가느다란 선을 간단한 모양의 입체로 바꾸어 볼 수 있다.
물체가 입체가 되면 프로그램은 훨씬 복잡해진다. 하지만, 시각적인 면에서나 기하광학의 이론적인
면에서, 그만큼 더 소득을 얻을 수 있을 것이다.



9.2. 이론

 평행투영을 사용하여 공간상의 점 佃，y, z）를 투영좌표 （邱，yp）로 변환하여 3차원 입체를 모니터
화면에 표현하여 보자．
 丁축과 y축은 모니터 화면의 좌표축과 방향이 같고 z축은 모니터 화면을 뚫고 들어가는 방향이다．
 공간상의 점 （毛 9, z）를 투영좌표 （邱，yp）로 변환하려면 두 개의 각도를 결정해야 한다．
 우선 （邱，佈）와 (x, y, 0）을 지나는 직선과 투영선이 이루는 투영각 (l이다．
218 제3부 기초적인 3차원 컴퓨터 그래픽




（邱，外）과 (x, y, 0) 사이의 거리를 ／이라고 하면


                             tana =   三／



이다. 아래의 그림들은 투영각에 따른 입체의 투영을 나타낸다．




          투영각 0
                             투영각 0.4冗


 그 다음 결정해야 할 각도는 (Il),     와 佃 y, 0）을 지나는 직선과 수평선에 의해 형성되는 방위
각 砂이다. 방위각이 클수록 입체의 윗부분이 더 많이 표시된다．
                                                                            제9장 3차원 입체의 구현 219




     방위각 0
                                                                  방위각 퓽


투영각과 방위각이 결정되면 （邱，yp）는 다음과 같이 계산된다．


                                   xp =    x+       icos色
                                    yP= y- lsin砂


그러면 아래의 그림



                                   (275,250,1000
                              (275,250,750)
                        (275,250,500
                                                       (450,400,1000)
                 (275,250,250)
                                                         0,750)
              (275,250,0
                                            \｛玉阿400.500
                                         .48J,400,250)

    (100,400,0)                                        (450,450,250)          450,650,1000)
                                                                   ////
                                                       450,100)

                                                             『650, 250)
                                                (A 仄n n二n ] nr\
    (100,650,0)       / /1 : r\ e C r\ r
                      ＼吐UU,UUU, U
                                                \l U\J ! \J1J\/ ! l \7\7/
220 제3부 기초적인 3차원 컴퓨터 그래픽



과 같은 좌표를 가친 집 (house）을 프로그램으로 구현하여 보자．



9.3. Source Code

II 3차원 입체뀌ew.cpp : implementation of the CMy3View class
II

#include "stdafx.h"
荊nclude "3차원 입체.h"


荊nclude "3차원 입체Doc.h"
#include "3차원 입체View.h"


#include <math.h>


const double pi 3.1415926535;


void figure ( CDC* pDC, double x, double y, double z, double alpha, double phi )
{
     double tanalpha, length, projectX, projectY;


     if ( (tanalpha=tan(alpha) ) !=0.0 )
            length = z/tanalpha;
     else
            length = 0.0;


     projectX = x+length*cos (phi);
     projectY = y-Iength*sin (phi);


     CPen myPen(PS_SOLID, 3, RGB(0,0,0));
     CPen* pO녑Pen = pDC->SelectObject (&myPen);
                                                                                제9장 3차원 입체의 구현 221



      pDC->LineTo (m t (projectX), m t (projectY));
      pDC->SelectObject (pOldPen);
}

void move ( CDC* pDC, double x, double y, double z, double alpha, double phi )
{
      double tanaipha, length, projectX, projectY;


      if ( (tanalpha=tan (alphafl!=0.0 )
            length = z/tanalpha;
      이se
            length = 0.0;


      projectX = x+length*cos (phi) ;
      pr이ectY = )'니engt小跏（phi) ;


      pDC->MoveTo (mnt (projectX), mnt (projectY));
}

#ifdeI _DEBUG
#define new DEBUG_NEW
#undef THIS小F瓦E
static char THIS_FILE [I = ...FILE_;
#endif


/I///////////////////I///I//I/II////I////I///////////////////////////////////
II CMy3View

IMPLEMENT_DYNCREATE (CMy3View, CView)

BEGIN_MESSAGE_MAP (CMy3View, CView)
   II { {AFX_MSG_MAP (CMy3View)
222 제3부 기초적인 3차원 컴퓨터 그래픽



           1/ NOTE - the ClassWizard will add and remove mapping macros here.
           II     DO NOT EDIT what you see in these blocks of generated code!
     //} } AFX_MSG_MAP
     II Standard printing commands
     ON_COMMAND (ID_FILEPRINT, CView::OnFilePrint)
     ON_COMMAND (ID_FILE_PRINT_DIRECT, CView: :OnFilePrint)
     ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView::OnFilePrintPreview)
END_MESSAGE_MAP 0


/////////////////////////////////////////////////////////////////////////////
II CMy3View construction/destruction


CMy鉀iew::CMy3뀌叫（)
{
     // TODO: add construction code here


}

CMy3 View:: -CMy3 View 0
{
}

BOOL CMy3View::PreCreateWindow (CREATESTRUCT& cs)
{
     // TODO: Modify the Window class or styles here by modifying
     // the CREATESTRUCT cs


     return CView::PreCreateWindow (cs);
}

/////////////////////////////////////////////////////////////////////////////
// CMy3View drawing
                                                                                제9장 3차원 입체의 구현 223



void CMy3View::OnDraw (CDC* pDC)
{
     CMy3Doc* pDoc = GetDocument 0;
     ASSERT_VALID (pDoc) ;


     static struct
      {
           double x, y, z;
           mnt option;
     } house [1 = { {450,650,0,0} , {100,650,0,1} , {100,400,0,1}, {450,400,0,1), {450,650,0,1} ,
      {450,650,1000,1} , {450,400,1000,1} , {450,400,0,1} , {275,250,0,1} , {100,400,0,1} ,
      {275,250,0,0} , {275,250,1000,1}, {450,400,1000,1}, {450,650,100,0), {450,450,100,1} ,
      {450,450,250,1} , {450,650,250,1} , {450,400,250,0} , {275,250,250,1} , {275,250,500,0} ,
      {450,400,500,1} , {450,400,750,0} , {275,250,750,1} };


     mlt i;


     for (江0; i<23; i++)
           if ( house{i].option==1 )
                  figure (pDC, house[iLx, house[i].y, house[i] .z, 0.35*pi, 0.15*pi);
           else
                  move (pDC, house [ii .x, house [ii .y, house [ii .z, 0.35*pi, 0.15*pi);
}

/////////////I////////////////////////////////////////I//////////////////////
II CMy3View printing


BOOL CMy3View::OnPreparePrinting (CPrintlnfo* plnfo)
{
     II default preparation
     return DoPreparePrinting (plnfo);
}
224 제3부 기초적인 3차원 컴퓨터 그래픽



void CMy3View::OnBeginPrinting (CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     1/ TODO: add extra initialization before printing
}

void CMy3View::OnEndPrinting (CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
      7/ TODO: add cleanup after printing
}

I///I/II!//I/I///////////////II/I//I/III/I/I////////////////II///I/I//II/III/
II CMy3View diagnostics


#ifdef .DEBUG
void CMy3View::AssertValid() const
{
      CView::AssertValid 0;
}

void CMy3View::Dump (CDumpContext& dc) const
{
      CView::Dump (dc);
}

CMy3Doc* CMy3View::GetDocument0 II non-debug version is inline
{
      ASSERT (rn4pDocument - >IsKindOf (RUNTIME_CLASS (CMy3Doc)));
     return (CMy3Doc*) m_pDocument;
}
#endif //JJEBUG


/////////////////////////////////////////////////////////////////////////////
                                        제9장 3차원 입체의 구현 225



/1 CMy3View message handlers


0
U   4
     프로그램 실행 결과



           파딛（t)   판口止｝ 보기d)   i뭄말（b)
           D 4 日        g' 凸   !
10:1. 이론

 원점에 중심을 가지고 있는 구（sphere）를 생각하여 보자. 이 구를 3배로 확대하고 싶다고 하자．
어떻게 하면 되겠는가7 반지름을 3배 해주면 된다．
 그러면 약간 관점을 달리하여 구를 이루는 모든 점들을 생각하여 보자． 원래의 구를 이루는 점들
과 확대된 구를 이루는 점들간에는 어떤 관계가 있는가7 확대된 구를 이루는 점들의 좌표는 원래의
구를 이루는 점들의 좌표를 3배 한 것이다．
 그러면 원점에 중심을 가지고 있지 않은 구를 확대하려면 어떻게 하면 되겠는가？ 구의 중심이 원
점이 되도록 이동한 후 배율을 곱한 후 새로 생긴 구의 중심이 원래의 구의 중심이 되도록 이동하면
된다.
 프로그램을 실행한 후에 團圄E｝巨小｝固 key를 누를 때마다 원래의 입체를 0.1배씩 확대하거나
축소한다. 방향 key를 누를 때마다 값이 변하는 서］ 변수들 zoomX, zoomY, zoon也는 " 입체의 확대
와 축소뀌ew.h" 에서 변수선언을 하고, " 입체의 확대와 축소View.cpp"에서 초기값을 지정한다.
228 제3부 기초적인 3차원 컴퓨터 그래픽




10.2. Source Code

10.2.1. 입체의 확대와 축소피이v.h

// 입체의 확대와 축소뀌ew.h : interface of the CMyView class
II
/!////////I//III////////////I/I//I/I///I////I/I/I/I////II/I////I/////I//II///

#if ! defined (AFX_VIEW_T-LC6 48B1EB_AA8E_4A 18_8 36 4_AE0E3AB1BE57_INCLUDED_)
#define AFX_VIEW_I-LC648B1EB_AA8E_4A18_8 3 64_AE0E3AB1BE5 7_INCLUDED_


#if _MSC_VER > 1000
#pragma once
#endif I! _MSC_VER > 1000



class CMyView : public CView
 {
protected: II create from serialization only
      CMyView 0;
      DECLARE_DYNCREATE (CMyView)


II Attributes
public:
      CMyDoc* GetDocument 0;
      double zoomX, zoomY, zoomZ;


/1 0perations
public:
                                                                저110장 입체의 확대와 축소 229



II Overrides
     II ClassWizard generated virtual function overrides
     II { {AFX1VIRTUAL (CMyView)
     public:
     virtual void OnDraw (CDC* pDC) ; II overridden to draw this view
     virtual BOOL PreCreateWindow (CREATESTRUCT& cs) ;
     protected:
     virtual BOOL OnPreparePrinting (CPrintlnfo* plnfo);
     virtual void OnBeginPrinting (CDC* pDC, CPrintlnfo* plnfo);
     virtual void OnEndPrinting(CDC* pDC, CPrintlnfo* plnfo);
     II) } AFX_VIRTUAL


I/ Implementation
public:
     미rtual 사CMyView ();
#ifdef _DEBUG
     virtual void AssertValidO const;
     virtual void Dump (CDumpContext& dc) const;
#endif


protected:


II Generated message map functions
protected:
     //{ {AFX소心G (CMy View)
     afx_msg void OnKeyDown(UINT nChar, UINT nRepCnt, UINT nFlags) ;
     II) } AFXMSG
     DECLARE_MESSAGE_MAP 0
};

荊fndef _DEBUG II debug version in 입체의 확대와 축소피ew.cpp
inline CMyDoc* CMyView: GetDocument 0
230 제3부 기초적인 3차원 컴퓨터 그래픽



     { return (CMyDoc*)nLpDocument; }
#end侄


////////I/////I/////////////////I////////////////////////////////////////////

II { {AFXJNSERT_LOCATION} }
II Microsoft Visual C++ will insert additional declarations immediately before the previous
line.


#endif                                                                                   1/
!defined (AF) 느VIEWJUC648B1EB_AA8E_4A18_8 364J1E0E3AB1BE57_INCLUDED_)


10.2.2. 입체의 확대와 축소피ew.cpp

// 입체의 확대와 축소View.cpp : implementation of the CMyView class
II

#include 'stdafx.h"
荊nclude " 입체의 확대와 축소．h'


荊nclude " 입체의 확태와 축소Doc.h"
荊nclude " 입체의 확대와 축소View.h"


#include <math.h>


const double pi 3.1415926535;


void figure ( CDC* pDC, double x, double y, double z, double alpha, double phi )
{
        double tanalpha, length, projectX, projectY;


        if ( (tanalpha=tan (alpha))! =0.0 )
                                                            저lb장 입체의 확대와 축소 231



          length = z/tanalpha;
    이se
          length = 0.0;


    projectX = x+length*cos(phi) ;
    pr이ectY = y나ength始in佃hi);
    CPen myPen(PS_SOLID, 3, RGB(0,0,0));
    CPen* pOldPen = pDC->SelectObject (&myPen);
    pDC中>LineTo (mnt (projectX), mnt (projectY));
    pDC中＞S이毗山히ect (p이dPen) ;
}

void move ( CDC* pDC, double x, double y, double z, double alpha, double phi )
{
    double tanalpha, length, projectX, projectY;


    if ( (tanalpha=tan(alpha))!=0.0 )
          length = z/tanalpha;
    이se
          length = 0.0;


    projectX = x+Iength*cos (phi);
    pr이ectY = y니engt小sin佃네；


    pDC->MoveTo (jot (projectX), mnt (projectY));
}

#ifdef JIEBUG
#define new DEBUGNEW
#undef THiS_FILE
static char THIS_FILE [1 = 1 FJLE_;
#endif
232 제3부 기초적인 3차원 컴퓨터 그래픽



/////////////I////I////////////////////////I//////////////I/I////////////////
II CMyView

IMPLEMENT_DYNCREATE (CMyView, CView)


BEGIN_MESSAGE_MAP (CMyView, CView)
     II { {AFX_MSG_MAP (CMyView)
      ONWM_KEYDOWN 0
      //} } AFX_MSG_MAP
     II Standard printing commands
      ON_COMMAND (ID_FILE_PRINT, CView::OnFilePrint)
      ON_COMMAND (ID_FILE_PRINT_DIRECT, CView::OnFilePrint)
      ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView::OnFjlePrjntPreview)
END_MESSAGEeMAP 0


///////////////////////////////////////////I/////////////////////////////////
II CMyView construction/destruction


CMyView::CMyView 0
 {
      zoomX=1.O, zoomY=1.O, zoomZ=1.O;


}

CMyView:：싸CMyView ()
{
}

BOOL CMyView::PreCreateWindow (CREATESTRUCT& cs)
 {
      // TODO: Modify the Window class or styles here by modifying
      // the CREATESTRUCT cs
                                                                                제］0장 입체의 확대와 축소 233


     return CView::PreCreateWindow (cs);
}

///I//////////////I////////////////I/////////////I////////////////I//////I///
II CMyView drawing


void CMyView::OnDraw (CDC* pDC)
{
     CMyDoc* pDoc = GetDocument 0;
     ASSERT_VALID (pDoc);


     static struct
      {
           double x, y, z;
           m1lt option;
     } house [I = { {450,650,0,0} , O00,650,0,1}, {100,400,0,1), {450,400,0,1), {450,650,0,1} ,
      {450,650,1000,1} , {450,400,1000,1} , {450,400,0,1} , {275,250,0,1} , {100,400,0,1} ,
      {275,250,0,0}, {275,250,1000,1}, {450,400,1000,1}, {450,650,100,0} , {450,450,100,1),
      {450,450,250,1} , {450,650,250,1), {450,400,250,0} , {275,250,250,1} , {275,250,500,0},
      {450,400,500,1} , {450,400,750,0} , {275,250,750,1} };


     mlt i;
     double x, centerX=275.0;
     double y, centerY=500.0;
     double z, centerZ=500.0;


     for (i=0; i<23; i++)
      {
           x = centerX-zoomX* (centerX-house [ii .x);
           y = centerY-zoomY* (centerY-house [ii .y);
           z = centerZ-zoomZ* (centerZ-house [ii .z);
234 제3부 기초적인 3차원 컴퓨터 그래픽



           if ( house[i] .option= =1 )
                  figure (pDC, x, y, z, 0.35*pi, 0.15*pi) ;
           이S（三

                 move (pDC, x, y, z, 0.35*pi, 0.15*pi) ;
     }
}

/////////////////////////////////////////////////////////////////////////////
II CMyView printing


BOOL CMyView::OnPreparePrinting (CPrintlnfo* plnfo)
{
     II default preparation
     return DoPreparePrinting(plnfo) ;
}

void CMyView::OnBeginPrinting (CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     II TODO: add extra initialization before printing
}

V아d CMyView: :OnEndPrinting (CDC永 ／虹）DC玎, CPrintlnfo水 /*plnfo永／)
{
     II TODO: add cleanup after printing
}

//////////////////////////I//////////////////////////////////////////////////
/7 CMyView diagnostics


荊fdef DEBUG
void CMyView::AssertValidO const
{
                                                                                제］0장 입체의 확대와 축소 235



      CView::AssertValid0;
}

void CMyView::Dump (CDumpContext& dc) const
 {
      CView::Dump (dc);
}

CMyDoc* CMyView::GetDocument () 7/ non-debug version is inline
 {
      ASSERT (rn. pDocument- >IsKindOf (RUNTIME_CLASS (CMyDoc)));
      return (CMyDoc*) m_pDocument;
}
#endif I/_DEBUG

/////I/II//I///////////I/III/II/II/II/I/II/II/IIII///II/I/III/I/I///I/I/II/I/
II CMyView message handlers

void CMyView::OnKeyDown(UINT nChar, UINT nRepCnt, UINT nFlags)
 {
      switch( nChar )
      {
           case VK_PRIOR:
                 zoomZ += 0.1;
                 break;


           case VK_NEXT:
                 if ( zoomZ>==0.1 )
                       zoomZ -== 0.1;


                 break;
236 제3부 기초적인 3차원 컴퓨터 그래픽



        case VK_LEFT:
             if ( zoomX>==0.1 )
                    zoomX -= 0.1;


             break;


        case VK--RIGHT:
             zoomX += 0.1;
             break;


        case VK_UP:
             zoomY += 0.1;
             break;


        case VK_DOWN:
             if ( zoomY>=0.1 )
                    zoomY -= 0.1;


             break;


        case VK_ESCAPE:
             exit (1) ;
    }

    Invalidate 0;


    CView::OnKeyDown(nChar, nRepCnt, nFlags) ;
}
                                        저lb장 입체의 확대와 축소 237




10,3. 프로그램 실행 결과

10요］. 三key를 다섯 번, 盈key를 일곱 번 누른 경우

        u= E)   딴집（L)   보기坦） 도움랖（b)
        二 才日              晉 孕




                                                  也



10.3.2. 匠key를 네 번, 圄key를 여덟 번 누른 경우

        皿일吃） 편찹（틔       보기d)   도뭄말（U)
        D 4 日           平 !    !




        副
238 제3부 기초적인 3차원 컴퓨터 그래픽




10.3.3, 三key를 네 번,                Jkey를 여섯 번, 쯔key를 세 번 누른 경우

         파일（E)   편집止） 보기吐） 도뭅말뉜
         D 哮L         甘뇨 甘   t




         副
                                                                NUM
11.1. 이론

 z축에 대하여 입체를 회전시키려면 아래의 code를 사용하면 된다．


  x = (object [ii .x-centerX) *cos (angleZ) 尸 (object [i] .y -centerY) *sin (angleZ) +centerX;
  y = (object [ii .卜centerX）永針n(an혭eZ) +(0비吼比］.少centerY）木cos (angleZ) +centerY;
  z = object [ii .z;


 y축에 태하여 입체를 회전시키려면 아래의 code를 사용하면 된다．


  x = (object [ii .x-centerX) *cos (angleY)中 (object [ii .z- centerZ) *sin (angleY) +centerX;
  z = (object [ii .x-centerX) *sjn (angleY) + (object [ii .z- centerZ) *cos (angleY) +centerZ;
  y = object[i].y;


 I축에 대하여 입체를 회전시키려면 아래의 code를 사용하면 된다．


  y = (object [ii .y -centerY) *cos (angleX) - (object [ii .z-centerZ) *sin (angleX) +centerY;
  z = (object [ii .y-centerY) *sin (angleX) + (object [ii .z-centerZ) *cos (angleX) +centerZ;
   x = object{i].x;
240 제3부 기초적인 3차원 컴퓨터 그래픽




11.2. Source Code

11.2.1, 입체의 화전View.h

// 입체의 회전View.h : interface of the CMyView class
II
//////////////////////////////I//I////I/////I///////////////I///////////////!

#if ! defined (AFX_VIEW_H_E1E8EE9 3_D170_4DA9_AC9B_0CAD9CC1A315_INCLUDEDi
#define AFX_VIEW_H_E1E8EE9 3_D170_4DA9_AC9B_0CAD9CC1A315_INCLUDED_


荊f eMS（二VER > 1000
#pragma once
#end迂 // mMS（二VER > 1000




class CMyView : public CView
{
protected: II create from serialization only
      CMyView 0;
      DECLARE_DYNCREATE (CMyView)


II Attributes
public:
      CMyDoc* GetDocument 0;
      double angleX, angleY, angleZ;


/7 0perations
public:
                                                                  제］］장 입체의 회전 241



// Overrides
     II ClassWizard generated virtual function overrides
     II { {AFX_VIRTUAL (CMyView)
     public:
     virtual void OnDraw (CDC* pDC); II overridden to draw this view
     virtual BOOL PreCreateWindow (CREATESTRUCT& cs);
     protected:
     virtual BOOL OnPreparePrinting (CPrintlnfo* plnfo);
     virtual void OnBeginPrinting(CDC* pDC, CPrintlnfo* plnfo);
     virtual void OnEndPrinting(CDC* pDC, CPrintlnfo* plnfo);
     //} } AFX_VIRTUAL


I/ Implementation
public:
     미rtual 사CMyView ();
#ifdef _DEBUG
     virtual void AssertValidO const;
     virtual void Dump (CDumpContext& dc) const;
#endif


protected:


II Generated message map functions
protected:
     II { {AFX_MSG (CMyView)
     afx_msg void OnKeyDown(UINT nChar, UINT nRepCnt, UINT nFlags);
     II) } AFX_MSG
     DECLARE_MESSAGE_MAP 0
};

荊fndef _DEBUG II debug version in 입체의 회전View.cpp
inline CMyDoc* CMyView: :GetDocumentO
242 제3부 기초적인 3차원 컴퓨터 그래픽



     { return (CMyDoc*)n pDocument; }
#endif


///////////////I/////////////////////////////////////////////////////////////

II { {AFXJNSERTLOCATION} }
II Microsoft Visual C++ will insert additional declarations immediately before the previous
line.


#endif                                                                                   II

!defined(AF)LVIEWJ-LE 1E8EE93D170_4DA9_AC9B_0CAD9CC1A315JNCLUDEDJ


11.2.2. 입체의 회전View.cpp

// 입체의 회전뮈ew.cpp : implementation of the CMyView class
II

#include "stdafx.h"
荊nclude " 입체의 회전.h'


荊nclude " 입체의 회전Doc.h"
荊nclude " 입체의 회전View.h"


 #include <math.h>


 const double pi=3.1415926535;


 void figure( CDC* pDC, double x, double y, double z, double alpha, double phi )
 {
        double tanaipha, length, projectX, projectY;


        if ( (tanalpha=tan(alpha) )!=O.O )
                                                                  제］l장 입체의 회전 243



          length = z/tanalpha;
    이se
          length = 0.0;


    projectX = x+length*cos(phi);
    pr이ectY = 少lengt小sin (phi);


    CPen myPen (PS_SOLID, 3, RGB (0,0,0));
    CPen串 p이dPen = pDC->Select아永Ct（邑myPen);
    pDC- >LineTo (mnt (projectX), mnt (projectY));
    pDC->SelectObject (pOldPen);
}

void move ( CDC* pDC, double x, double y, double z, double alpha, double phi )
{
    double tanaipha, length, projectX, projectY;


    if ( (tanalpha=tan (alpha))! =0.0 )
          length = z/tanalpha;
    이se
          length = 0.0;


    projectX = x+length*cos (phi);
    pr이ectY = y니engt小師（phi);


    pDC->MoveTo (mnt (projectX), mnt (projectY));
}

#ifdef _DEBUG
#define new DEBUG. .NEW
#undef THIS_FILE
static char THIS_FILE [1 = _FILE_;
244 제3부 기초적인 3차원 컴퓨터 그래픽



#end汀


/////////////////////////////////////////////////////////////////////////////
II CMyView


IMPLEMENT_DYNCREATE (CMyView, CView)


BEGIN_MESSAGE_MAP (CMyView, CView)
     //{ {AF乂MSG소4AP (CMyVie的
     ONWM_KEYDOWN 0
     //} } AFX小4SG소4AP
     II Standard printing commands
     ON_COMMAND (ID_FILE_PRINT, CView::OnFilePrjnt)
     ON_COMMAND (ID_FILE_PRINT_DIRECT, CView::OnFilePrint)
     ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView::OnFilePrjntPrevjew)
END1MESSAGE_MAP 0


/////////////////////////////////////////////////////////////////////////////
II CMyView construction/destruction


CMy View::CMy View 0
{
     ang1eX=O.O, ang1eY=O.O, angleZ=O.O;
}

CMy View::NCMyView ()
{
}


BOOL CMyView::PreCreateWindow (CREATESTRUCT& cs)
{
     // TODO: Modify the Window class or styles here by modifying
                                                                                제］］장 입체의 회전 245



     II the CREATESTRUCT cs


     return CView::PreCreateWindow (cs);
}

///////I//////////////////////////////////////////////////I///I//////////!///
II CMyView drawing


void CMyView::OnDraw (CDC* pDC)
{
     CMyDoc* PDOC = GetDocument 0;
     ASSERT_VALID (pDoc) ;


     static struct
      {
           double x, y, z;
           mlt option;
     }cuboid [I! = { {250,200,O,O} , {500,200,O,1} , {500,500,O,1), {250,500,O,1} ,
      {250,200,O,1} , {250,200,300,1} , {500,200,300,1}, {500,500,300,1} , {500,500,O,1),
      {500,200,O,O} , {500,200,300,1), {250,200,300,O} , {250,500,300,1}, {500,500,300,1} ,
      {250,500,300,O} , {250,500,O,1} };


     mnt 1;
     double x, centerX=375.O, newX;
     double y, centerY=350.O, newY;
     double z, centerZ=150.O;


     for (i=O; i<16; i++)
      {
           x = (cuboid [ii .x-centerX) *cos (angleZ)
                 - (cuboid [ii .y-centerY) *sin (angleZ) +centerX;
           y = (cuboid [ii .x-centerX) *sin (angleZ)
246 제3부 기초적인 3차원 컴퓨터 그래픽



                 +(cub아d[i] .少centerY）永cos (an합eZ) +centerY;
           newX = (x-centerX) *cos (angleY) + (cuboid [ii .z-centerZ) *sin (angleY) +centerX;
           z = (x-centerX) *sin (angleY) + (cuboid [ii .z-centerZ) *cos (angleY) +centerZ;
           x = newX;
           newY = (y-centerY) *cos (angleX) - (z-centerZ) *sin (angleX) +centerY;
           z = (y - centerY) *sin (angleX) + (z- centerZ) *cos (angleX) +centerZ;
           y = newY;


           if ( cuboid[il.option==1 )
                 figure (pDC, x, y, z, 0.35*pi, 0.15*pi);
           이se
                 move (pDC, x, y, z, 0.35*pi, 0.15*pi);
     }
}

/////////////////////////////////////////////////////////////////////////////
II CMyView printing


BOOL CMyView::OnPreparePrinting (CPrintlnfo* plnfo)
{
     II default preparation
     return DoPreparePrinting (plnfo);
}

void CMyView::OnBeginPrinting (CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     II TODO: add extra initialization before printing
}

void CMyView::OnEndPrinting (CDC木 戶pDC玎, CPrintlnfo米 小이nfo*/)
{
     II TODO: add cleanup after printing
                                                                                제11장 입체의 회전 247


 }

I/I//I//////////////I//////////i/II/I/iiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiii
II CMyView diagnostics

#ifdef JIEBUG
void CMyView::AssertValid 0 const
 {
      CView::AssertValid 0;
}

void CMyView::Dump (CDumpContext& dc) const
 {
      CView::Dump (dc);



CMyDoc* CMyView::GetDocumentO II non-debug version is inline
 {
      ASSERT (nipDocument->IsKindOf (RUNTIME_CLASS (CMyDoc)));
      return (CMyDoc*) m_pDocument;
}
#endif I/_DEBUG


I/////////////////////////I//I/I//////I///////I/I////I//////I/I////I////////I
II CMyView message handlers


void CMyView::OnKeyDown(UINT nChar, UJNT nRepCnt, UINT nFlags)
{
      switch( nChar )
      {
           case VK_PRIOR:
                 angleZ += O.1*pi;
248 제3부 기초적인 3차원 컴퓨터 그래픽



             break;


        case VK_NEXT:
             angleZ -= 0.1*pi;
             break;


        case VK_LEFT:
             angleX -= 0.1*pi;
             break;


        case VKRIGHT:
             angleX += 0.1*pi;
             break;


        case VK_UP:
             angleY += 0.1虹）i;
             break;


        case VKDOWN:
             angleY -= 0.l*pi;
             break;


        case VK_ESCAPE:
             exit (1);
    }

    Invalidate 0;


    CView::OnKeyDown(nChar, nRepCnt, nFlags) ;
}
                                                       제］］장 입체의 회전 249




11.3. 프로그램 실행 결과

11.3.1. 日 key를 누른 경우

  ri : 트！;   !   r    工！t1   11巴 E＝二 ！川r     i1
   그아w           a,          그 才U     !) 1   1




  한 번 누른 경우                  두 번 누른 경우
  1亡自 ！쩍U ！川力 도11꾜1          11!5 띤＝띠 工nd) i      1出
  D1 日  ' / i느a ,            그아므     b '1 . I
                             尸




  서］ 번 누른 경우                 네 번 누른 경우
250 제3부 기초적인 3차원 컴퓨터 그래픽



                                r可三 끄＝三   工川r i뮴1：
                                                 工
                                 그 아日       4 !




  다섯 번 누른 경우                    여섯 번 누른 경우



11.3.2. 田 key룔 누른 경우

  1心e 딴＝띠 ！긔凹 三뮴口d;
                            쩍   11七 콘＝U ！긔：r   도It,'
                                口 아日     U 1   !




                                 n




  한 번 누른 켱우                     두 번 누른 경우
  r1m1 r＝上： ! ) a4 三 1KdJ                 ！力Lr 도 工足d=
  口4 日           4 1                       모11 !




  서］ 번 누른 경우                    네 번 누른 경우
                                                          제］］장 입체의 회전 251



1m巴 凸느＝    !J i    m1 크           1m二 판V느   !/ r   크1rd
 그 i u         4   !




다섯 번 누른 경우                        여섯 번 누른 경우
口1 日      \ aa     !




im




일곱 번 누른 경우                        여덟 번 누른 경우
1甘5 깐잠＝; !nr       i11d           11J 므스已 ！기Y i1k1
J 呼U      iJ a      ?             3 아日     少 a,




                       4＝二二二二7才


E버




아홉 번 누른 경우                        열 번 누른 경우
252 제3부 기초적인 3차원 컴퓨터 그래픽




11.3.3. 團 key률 누른 경우

  n1d 므＝止： ！吐r ala         口1巴 IL ;   !1，刃 도1i=d
  口 나口     日 1 !           그 나日        尸 1 1




  t出




  한 번 누른 경우                두 번 누른 경우
  iit  rm目 ！川녑 i   3고工     11上 딴＝띠 !7曲 i11m
  口 才 日 ; r 好 a,           그 4 日    小 a ,




  H




  세 번 누른 경우                네 번 누른 경우
   어11 1 1] 니 1; 거 4 1                             1   J   k
  口it1 띤1띠 ! 'RD LIES      11巴 ！三띠 ！기凹 됴11rd
  a m日 1      尸'a    !     口才 S     i1 1 !




  다섯 번 누른 경우               여섯 번 누른 경우
                                           제］］장 입체의 회전 253



 거 r 1 ;1 끼 11 已！       n채 14尸 Jn ：겊
1二乞 L11L} !7m 노！r4    1}1正： 만LL ！서r i丘Iw
口心마            1 !    口i 1        a !




일곱 번 누른 경우            여덟 번 누른 경우
日1므 1n= !J r   工11d   11上 딴식目 ！川f 工11nd;
口 아日     ? 1   !       그 4 日  a 三 1 1




아홉 번 누른 경우            열 번 누른 경우
12.1. 개론

 우리가 입체를 모니터에 표현할 때 그 입체는 점과 직선과 곡선으로 표현된다. 이 경우 어떤 관찰
자가 입체를 바라볼 때 그 입체에서 보이지 않는 부분이 있는데 그 부분은 당연히 화면에 표시되어
서는 안 된다. 그러면 어떻게 해야 보이지 않는 부분을 없앨 수 있을 것인지가 문제가 된다. 이러한
문제를 가리켜서 숨은선 제거 , 숨은면 제거라 한다. 일반적으로 숨은선과 숨은면을 제거하는 알고리
즘은 꽤나 복잡하고 구현하는 것도 쉽지 않다. 물론 우리는 이 책에서 그러한 것을 공부하지 않는다．
그렇다고 3차원 컴퓨터 그래픽에서 숨은선과 숨은면 제거를 건너뛸 수는 없다．
 우리는 이 chapter에서 정육면체나 구면처럼 간단한 모양의 입체에 대해서 숨은선 제거를 해 볼
것이다. 입체가 조금이라도 더 복잡하면 숨은선 제거에 더 많은 노력을 들여야 하고 처리 시간도 상
당히 길어진다．



12.2, 정육면체

12.2.1. 이론

 바라보는 위치를 달리하면서 정육면체를 관찰하여 보아라. 결코 네 개의 면 이상을 볼 수는 없다．
이것을 이용하여 정육면체의 숨은선을 제거할 수 있다．
 회전하지 않은 정육면체를 정면에서 바라보아라. 그리고 눈 앞에 보이는 면과 그 면에 평행한 면
256 제3부 기초적인 3차원 컴퓨터 그래픽



을 머릿속에 그려 보아라. 우리는 이 두 평행한 면 중에서 어느 하나를 볼 수 있다. 그러면 우리가
볼 수 있는 면과 볼 수 없는 면을 어떻게 판별할 수 있을까7 두 면의 좌표를 생각하여 보면 쉽게 알
수 있다. 우리가 볼 수 있는 면의 z좌표는 볼 수 없는 면의 z좌표보다 작다. 이것을 프로그래밍하면
된다. 마찬가지로 다른 두 평행한 면, 즉 두 옆면에 대해서는 x좌표를 비교하고, 또 다른 두 평행한
면, 즉 윗면과 아랫면에 태해서는 y좌표를 비교한다．


12.2.2. Source Code

// 숨은선과 숨은면 제거View.cpp : implementation of the CMyView class
II

#include "stdafx.h"
荊nclude " 숨은선과 숨은면 제거 .h'


荊nclude "숨은선과 숨은면 제거Doc.h"
荊nclude "숨은선과 숨은면 제거피ew.h"


#include <math.h>


const double pi=3.1415926535;


struct 이ane
{
     double x, y, z;
     mlt option;
};

void figure ( CDC* pDC, double x, double y, double z, double alpha, double phi )
{
     double tanalpha, length, projectX, projectY;


     if ( (tanalpha=tan(alpha) ) !=0.O )
                                                      제］2장 입체의 숨은선과 숨은면 제거 257



           length = zltanalpha;
    이se
           length = 0.0;


    projectX = x+length*cos (phi);
    pr이ectY = 少lengt小針n(p川）;


    CPen myPen(PS_SOLID, 3, RGB(0,0,0));
    CPen* pOldPen = pDC->SelectObject (&myPen);
    pDC- >LineTo (mnt (projectX), mnt (projectY));
    pDC->S이ec山히ect (p이dPen) ;
}

void move ( CDC木 pDC, double x, double y, double z, double alpha, double phi )
{
    double tanalpha, length, projectX, projectY;


    if ( (tanalpha=tan(alpha)) !=0.0 )
           length = z/tanalpha;
    else
    elSe
           length = 0.0;


    projectX = x+length*cos (phi);
    pr이ectY = 出length半sin (phi);


    pDC->MoveTo (mnt (projectX), mnt (projectY));
}

void displayPlane ( CDC* pDC, struct plane line[], double offsetX, double offsetY )
{
    mlt m;
258 제3부 기초적인 3차원 컴퓨터 그래픽



     for ( 件0; i<6; i++ )
           if ( line[il.option==1 )
                 figure( pDC, line[i].x+offsetX, line[i] .y+offsetY, line[i] .z, 0.35*pi, 0.15*pi );
           이se
                 move( pDC, line[il.x+offsetX, line[il.y+offsetY, line[il.z, 0.35*pi, 0.15*pi );
}

#ifdef _DEBUG
#define new DEBUG_NEW
#undef THIS_FILE
static char THIS_FILE[1 = 1Jm且1
#endif


/////////////////////////////////////////////I//////////////I//////////////I/
// （玉如뀌이V



IMPLEMENT_DYNCREATE (CMyView, CView)


BEGIN_MESSAGE_MAP (CMyView, CView)
     //{{AFX_MSG_MAP(CMyView)
           II NOTE - the ClassWizard will add and remove mapping macros here.
           II     DO NOT EDIT what you see in these blocks of generated code!
     //} } AFX그dSG_MAP
     II Standard printing commands
     ON_COMMAND (ID_FILE_PRINT, CView::OnpilePrint)
     ON_COMMAND (ID_FILE_PRINT_ 파ECT, CView::OnFilePrint)
     ON_COM入AND (ID_FILE_PRINT_PREVIEW, CView::OnFilePrintPreview)
END_MESSAGE_
          MAP 0


/////////////////////////////////////////////////I///////////////////////////
II CMyView construction/destruction
                                                                          제俚장 입체의 숨은선과 숨은면 제거 259



CMyView::CMyViewO
{
     II TODO: add construction code here


}

CMyView:: -CMyView 0
{
}

BOOL CMyView::PreCreate Window (CREATESTRUCT& cs)
{
     II TODO: Modify the Window class or styles here by modifying
     II the CREATESTRUCT cs


     return CView::PreCreateWindow (cs);
}

/////////////////////////////////////////////////////////////////////////////
/1 CMyView drawing


void CMyView::OnDraw (CDC* pDC)
{
     CMyDoc* pDoc = GetDocument 0;
     ASSERTVALID (pDoc);


     static struct plane a[]={ {310,200,0,0} , {550,200,0,1} , {550,410,0,1} , {310,410,0,1} ,
      {310,200,0,1} };
     static struct plane b [1 = { {310,200,250,0} , {550,200,250,1}, {550,410,250,1} ,
      {310,410,250,1}, {310,200,250,1} };
     static struct plane c [1 = { {550,200,0,0}, {550,200,250,1}, {550,410,250,1},
      {550,410,0,1}, {550,200,0,1} };
260 제3부 기초적인 3차원 컴퓨터 그래픽



     static struct plane d [1 = { {310,200,0,0} , {310,200,250,1} , {310,410,250,1} ,
      {310,410,0,1} , {310,200,0,1} );
     static struct plane e[]={ {310,410,0,0}, {550,410,250,1} , {310,410,250,1} ,
     {310,410,0,1} , {550,410,0,1} };
     static struct plane f[Ik{ {550,200,0,0}, {550,200,250,1}, {310,200,250,1) ,
      {310,200,0,1}, {550,200,0,1} };


     double offsetX= 100.0, offsetY=50.0;


     if ( a[0].z<b[0I.z )
            displayPlane ( pDC, a, offsetX, offsetY );
     이se
     이Se
            displayPlane ( pDC, b, offsetX, offsetY );


     if ( c[0].x>d[0].x)
            displayPlane ( pDC, c, offsetX, offsetY );
     이se
     이Se
            displayPlane ( pDC, d, offsetX, offsetY );


     if ( e[0I.y<f[01.y )
            displayPlane ( pDC, e, offsetX, offsetY );
     else
     eiSe
            displayPlane ( pDC, 1, offsetX, offsetY );
}

////!//////I/II//III/I//I/I/I/I/IIII//I/III////I/III//II/IIIIIII/I/I/II/II//I
II CMyView printing


BOOL CMyView::OnPreparePrinting (CPrintlnfo* plnfo)
{
     II default preparation
     return DoPreparePrinting (plnfo);
                                                                          제］2장 입체의 숨은선과 숨은면 제거 261



}

void CMyView::OnBeginPrinting (CDC* /*pDC*/, Cprintlnfo* /*plnfo*/)
{
     II TODO: add extra initialization before printing
}

void CMyView::OnEndPrinting(CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     II TODO: add cleanup after printing
}

/////////////////////////////////////////////////////////////////////////////
II CMyView diagnostics


荊fdef DEBUG
void CMyView::AssertValidO const
{
     CView::AssertValid 0;
}

void CMyView::Dump (CDumpContext& dc) const
{
     CView::Dump (dc);
}

CMyDoc* CMyView::GetDocument0 II non-debug version is inline
{
     ASSERT(mpDocument->IsKindOf (RUNTIME_CLASS(CMyDoc)));
     return (CMyDoc*)nLpDocument;
}
#endif I/_DEBUG
262 제3부 기초적인 3차원 컴퓨터 그래픽



///////////////////////////////I////////////////////I!II//////II/////////////
II CMyView message handlers


12 2 3 프로그램 실행 켤과


                 =1 솜 픈 신 il1 솜 븐 낸 세 거       저1 "J; 없 g
                 파딜止） 판집低） 보기（보） 도뭅앞（d)
                  0 畔1          小 6       !




                  副
                                                                                NLJM




12.3. 지구본

12.3.1. 이론

  지구본을 제작0）하여 보자．
  프로그램은 3차원 구면을 y축, x축, z축에 대하여 순서대로 회전시킨 후에, 구면을 xy 평면에 투
영한다. 이 구면에는 실제의 지구본처럼 위도(latitude）와 경도(longitude）가 표시되어 있어 구면은
입체처럼 보인다. 숨은선은 우리에게 보이지 않는 위도와 경도이다．
  프로그램을 분석하여 보자．
  위도를 그리는 code fragn祀nt는 아래
                                                          제］2장 입체의 숨은선과 숨은면 제거 263



  for (theta=pi; theta> - pi; theta- =interval)
      for (phi 0.0; phi<=2.0*pi; phi+=pi/44000.0)
      {
           x = radius*cos(theta) *sin(phi);
           y = radius*sin (theta);
           z = radius*cos (theta) *cos (phi);


          rotate (xr, yr, zr, &x, &y, &z) ;


           if ( z<0.0 )


           else
                  pDC->SetPixel (mnt (x), mnt (y), RGB (0,0,0));
      }

인데 , 마지막의 if 문에서 조건에 해당하면 이것은 숨은선이 된다．
 그럼 아래의 code fragment


  for (phi 0.0; phi@pi; phi+=interval)
      for (theta=0.0; theta<= 2.0*pi; theta+=pi/44000.O )
      {
           x = radius*cos (theta) *sin(phi);
           y = radius*sin(theta);
           z = radius*cos(theta)*cos (phi);


          rotate (xr, yr, Zr, &x, &y, &z);


          if ( z<0.0 )


          이S（三

                  pDC->SetPixel (int (x), int (y), RGB (0,0,0));
      }
264 제3부 기초적인 3차원 컴퓨터 그래픽



가 무엇을 하는 부분인지 쉽게 알 수 있을 것이다．


12.3.2. Source Code

II 지구본View.cpp : implementation of the CMyView class
II

#include "stdafx.h"
荊nclude 1'지구본．h'


荊nclude "지구본Doc.h"
荊nclude ”지구본View.h"


#include <math.h>


void rotate ( double xr, double yr, double zr, double *px, double 永py, double *pz )
{
     double xl, yl, zi, x2, y2, z2, x3, y3, z3;


     xl = (*pz）串sin (yr) +（枉）x）非cos (yr);
     yl = 勺：)y;
     zi = (*pz）水cos (yr) -（木px）希sin(yr);
     x2 = xL
     y2 = zl*sin(xr) +yl*cos(xr);
     z2 = zl*cos(xr) -yl* sin(xr);
     x3 = x2*cos (zr) -y2*sin(zr);
     y3 = x2*sin(zr) +y2*cos(zr);
     z3 = z2;
     *px = x3;
     *py = y3;
     虹）z = z3;
}
                                                                          제］2장 입체의 숨은선과 숨은면 제거 265



const double radius=890.0;


#ifdef _DEBUG
#define new DEBUG_NEW
#undef THIS_FILE
static char THIS_FILE [1 = _FILE_;
#endif


/////////////////////////////////////////////////////////////////////////////
II CMyView

IMPLEMENT_DYNCREATE (CMyView, CView)


BEGIN_MESSAGE_MAP (CMyView, CView)
     II { {AFX_MSG_MAP (CMyView)
           II NOTE - the ClassWizard will add and remove mapping macros here.
           II      DO NOT EDIT what you see in these blocks of generated code!
     II) } AFX_MSG_MAP
     II Standard printing commands
      ON_COMMAND (ID_FILE_PRINT, CView::OnFilePrint)
      ON_COMMAND (ID_FILE_PRINT_DIRECT, CView::OnFilePrint)
      ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView::OnFilePrintPreview)
END_MESSAGE_MAP 0


/////////////////////////////////////////////////////////////////////////////
II CMyView construction/destruction


CMy View::CMy View 0
 {
      // TODO: add construction code here


 }
266 제3부 기초적인 3차원 컴퓨터 그래픽



CMyView::싸CMyView0
{
}                           "




BOOL CMyView::PreCreateWindow (CREATESTRUCT& cs)
 {
     II TODO: Modify the Window class or styles here by modifying
     II the CREATESTRUCT cs


     return CView::PreCreateWindow (cs);
}

////I///II///I////I///II//////I////////////////////I///////II//////////II/!/I
II CMyView drawing

void CMyView::OnDraw (CDC* pDC)
{
      CMyDoc* pDoc = GetDocument0;
      ASSERT_VALID (pDoc) ;


      double theta, phi;
      double x, y, z, xr, yr, zr;
      const double pi 3.1415926535, interval=pi/12.0;


     pDC->SetMapMode (M旺LOMETRIC);
     pDC->SetViewportOrg (512, 330);


      xr = -0.3枉）1,
      yr = pi/5.0;
      zr = -0.4*pi;


     pDC- >Ellipse (mnt (-radius), mnt (radius), mnt (radius), mnt (-radius));
                                                                           제］2장 입체의 숨은선과 숨은면 제거 267



      for (theta= pi; theta> - pi; theta- =interval)
            for (phi 0.0; phi@ 2.0*pi; phi+=pi/44000.0)
            {
                 x = radius*cos (theta) *sin(phi) ;
                 y = radius*sin(theta) ;
                 z = radius*cos (theta) *cos (phi) ;


                 rotate (xr, yr, zr, &x, &y, &z) ;


                 if ( z<0.0 )


                 이se
                       pDC->SetPixel(int (x), mnt (y), RGB (0,0,0) );
            }

      for (ph江0.0; phi<=pi; phi+=interva!)
            for (theta=0.0; theta<=2.0*pi; theta+=pi/44000.0 )
            {
                 x = radius*cos (theta) *sin(phi) ;
                 y = radius*sin (theta) ;
                 z = radius*cos (theta) *cos (phi) ;


                 rotate (xr, yr, zr, &x, &y, &z);


                 if ( z<0.0 )


                 이se
                       pDC->SetPixel (int (x), mnt (y), RGB (0,0,0) );
           }
}

IIIIIIIIIIIIIIIIIII!I!IIIIII!IIIII/IIIIIIIIIII/ull/III!IIIIIIIIIIIII!IIIIIIIII
268 제3부 기초적인 3차원 컴퓨터 그래픽



1/ CMyView printing


BOOL CMyView::OnPreparePrinting (CPrintlnfo* plnfo)
{
     1/ default preparation
     return DoPreparePrinting (plnfo);
}

vo沁 CMyView::OnBeginPrinting (CDC半 小pDC*/, CPrintlnfo米 A이nfo米／)
{
     II TODO: add extra initialization before printing
}

void CMyView::OnEndPrinting (CDC木 小pDC玎, CPrintlnfo米 A이nfo米／)
{
     II TODO: add cleanup after printing
}

//////////////////////////////////////////////////////////I//////////////////
II CMyView diagnostics


#ifdef _DEBUG
void CMyView::AssertValid 0 const
{
     CView::AssertValid 0;
}

void CMyView::Dump (CDumpContext& dc) const
{
     CView::Dump (dc) ;
}
                                                                          재］2쟝 입체의 숨은선과 숨은면 졔거 269



CMyDoc* CMyView::GetDocumentO II non-debug version is inline
{
      ASSERT (mpDocument今Is지nd아(RUNTIME놔CLASS ((玉如Doc) )) ;
      return (CMyDoc*)m1pDocument;
}
#endif I/_DEBUG

//I//I/I///IIII//I//III/IIII//II/I//I/I/I/IIIIII/I//I//II/II///I///I//I/////I
II CMyView message handlers


12 3 3 프로그램 실행 결과



                  파딜（E)   판집止） 보기（y)   도욤맣咆）
                  口才L           :?) 凸 !




                  副
                                                                                      N바d
  少翎率，, ., ,／「 0」，,0/
H匙
13.1. 개론

 드디어 마지막 chapter이다．
 이 chapter에서는 이변수함수 z = f (x, ,）의 함수를 간략하게 구현하여 볼 것이다．
 우선은 투영의 원리에 충실하게 그래프를 그릴 것이다. 좀 보기에 좋지 않더라도 일단은 이변수함
수의 그래프를 직접 우리의 손으로 구현하여 본다．
 그런 다음에는 위의 그래프에서 숨은선을 제거한다. 그러면 시각적으로 좀 더 보기에 좋은 모양이
된다．
 물론 여기에서도 간단한 방법으로 모든 문제를 해결할 것이다. 복잡한 알고리즘을 굳이 따질 필요
는 없다. 복잡한 알고리즘을 익히는 것보다 알고리즘을 잘 활용하는 것에 목적이 있다는 것을 잊지
말아라．



13.2, 이변수함수 i

13.2.1. 이론

 이변수함수
272 제3부 기초적인 3차원 컴퓨터 그래픽



                                         577
                            z = 16x+    0.1 付 + 切2)




의 그래프를 평행투영법으로 구현하여 보자．
 Mathematica 같은 소프트웨어에서 이변수함수의 그래프를 그리는 것이 아니라, 지금처럼 프로그
래밍 언어를 사용하여 직접 그래프를 그리는 것은 매우 어려운 일이다. 위의 식에서 16이나 577은
필자가 계수를 이란저런 값들로 바꿔 가면서 프로그램을 실행하여 출력 결과가 보기에 괜찮은 경우
를 찾은 것이다．
     Mathematica에서 z= f佃, y）의 그래프를 그려보면 다음과 같다．




프로그램 실행 결과와 비교하여 보아라．


13.2,2. Source Code

// 이변수함수피ew.cpp : implementation of the CMyView class
II

#include n stdafx.h"
#include "이변수함수．h


荊nclude "이변수함수Doc.h"
                                                               제］3장 이변수함수의 그래프 273



荊nclude "이변수함수View.h '


#include <math.h>


void move ( CDC* pDC, double x, double y, double z, double alpha, double phi )
{
    double projectX, projectY, length, tanalpha;


    if ( (tanalpha=tan(alphafl!=0.0 )
          length = z/tanalpha;
    이se
          length = 0.0;


    projectX = x + length*cos (phi) ;
    projectY = y - length*sin(phi) ;


    pDC- >MoveTo (mnt (projectX), mnt (projectYfl;
}

void graph( CDC* pDC, double x, double y, double z, double alpha, double phi
{
    double projectX, projectY, length, tanalpha;


    if ( (tanalpha=tan(alpha) )!=0.0 )
          length = z/tanalpha;
    이se
          length = 0.0;


    projectX = x + length*cos (phi) ;
    projectY = y - length*sin (phi) ;


    pDC->SetPixel (m t (projectX), mnt (projectY), RGB(255,0,255) );
274 제3부 기초적인 3차원 컴퓨터 그래픽



}

#ifdef _DEBUG
#define new DEBUG_NEW
#undef THIS_FILE
static char THIS_FILE [1 = _FILE_;
#endif


/////////////////////////////////////////////////////////////////////////////
// CMyView


IMPLEMENT_DYNCREATE (CMyView, CView)


BEGIN_MESSAGE_MAP (CMyView, CView)
     II { {AFX_MSG_MAP (CMyView)
           II NOTE - the ClassWizard will add and remove mapping macros here.
           II     DO NOT EDIT what you see in these blocks of generated code!
     //} } AFX小心G_MAP
     II Standard printing commands
     ON_COMMAND (ID_FILE_PRINT, CView::OnFilePrint)
     ON_COMMAND (ID_FILE_PRINT_DIRECT, CView: :OnFilePrint)
     ON_COMMAND (ID_FILE_PRINT_PREVIEW, CView::OnFilePrintPreview)
END_MESSAGE_MAP 0


/////////////////////////////////////////////////////////////////////////////
II CMyView construction/destruction


CMyView::CMyView0
{
     // TODO: add construction code here


}
                                                                                제］3장 이변수함수의 그래프 275



CMyView::사CMyView 0
{
}

BOOL CMyView::PreCreateWindow (CREATESTRUCT& cs)
{
     II TODO: Modify the Window class or styles here by modifying
     II the CREATESTRUCT cs


     return CView::preCreateWjndow (cs);
}

/////////////////////////////////////////////////////////////////////////////
II CMyView drawing


V아d CMyView::OnDra砥／(CDC水 pDC)
{
     CMyDoc* pDoc = GetDocument 0;
     ASSERT_VALID (pDoc);


     const double pi 3.1415926535;
     double x, xx, y, yy, z;


     pDC->SetMapMode (MM_LOMETRIC);
     pDC->SetViewportOrg(512, 350);


     for (x=-1000.0; x<1001.0; x+=100.0)
      {
           xx = xll0o.0;
           move (pDC, xx, -8.0, 0.0, 0.7*pi, 0.2*pi);


           for (y=-B00.0; y<B00.0; y+=1.0)
276 제3부 기초적인 3차원 컴퓨터 그래픽



           {
                yy = y/100.0;
                z = 16.0*xx+577.0*exp (_0.1* (xx*xx+2.0*yy*yy));
                graph(pDC, x, y, z , Q.7*pi, 0.2*pi);
           }
     }

     for (y= -800.0; y<80l.0; y+=lQQ.Q)
      {
           yy = y/ l00.0;
           move (pDC, -10.0, y, 0.0, 0.7*pi, 0.2*pi) ;


           for (x= -1000.0; x<1000.0; x+=1.0)
           {
                 xx = x/100.0;
                 z = 16.아xx+577 .아exp(- 0.卜（xx永xx+2.0米yy水yy) );
                 graph (pDC, x, y, z , 0.7*pi, 0.2*pi);
           }
     }
}

////////////////////////////////////////////////////////////////////////I////
II CMyView printing


BOOL CMyView::OnPreparePrinting (Cprintlnfo* plnfo)
{
     II default preparation
     return DoPreparePrinting (plnfo) ;
}

vo沁 CMyView::OnBeginPrinting (CDC米 小pDC玎, CPrintlnfo木 小plnfo米／)
{
                                                                                 제］3장 이변수함수의 그래프 277



     II TODO: add extra initialization before printing
}

void CMyView::OnEndPrinting(CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     II TODO: add cleanup after printing
}

III/////!//I/I///II///////I//////////////////////I///////I/!I/I//////I////II/
II CMyView diagnostics


#ifdef _DEBUG
void CMyView::AssertValidO const
{
      CView::AssertValid 0;
}

void CMyView::Dump (CDumpContext& dc) const
{
      CView::Dump (dc);
}

CMyDoc* CMyView::GetDocument0 II non-debug version is inline
{
      ASSERT (rnpDocument今IsKindOf (RUNTIME_CLASS (CMyDoc)));
      return (CMyDoc*) n니pDocument;
}
#endif I/_DEBUG


III/IIIIIIIIII/I/IIII/I/II1/IIIIIIIIII//I///IIIIIIII//IIII/IIIII/IIII/IIIIII/I
II CMyView message handlers
278 제3부 기초적인 3차원 컴퓨터 그래픽




13.2.3. 프로그램 실행 결과


         파일［E)   판집七） 보기吐） 도뭄및（d)
         口 才 1泣          凸   !



                                                          1叫



                                                               寸寸寸나寸寸寸규


                                                               나
                                                               aij




13.3. 이변수함수 n

13.3.1. 이론

 이 section에서는 이전의 scetion의 프로그램보다 짧은 길이의 code로 이변수함수를 구현한다．
 이변수함수


                             z= 120cos\/x2+ y2+ 7cos (11\/x2+ 9 2)



의 그래프를 그리는데 z축에 대해 회전을 시킨 후에, x축에 대해 회전을 시킨다. 두 번 회전시키고
나서는 화면에 투영한다．
 프로그램에서 rotateZ와 rotateX의 값을 여러 가지로 바꾸어 보아라. 두 변수의 역할을 금방 알게
될 것이다．
                                                                                제］3장 이변수함수의 그래프 279



     한편, for 문을 보면 변수 x의 증가치가 매우 작다는 것을 알 수 있는데, 이것은 그래프가 그려지
는 것을 우리가 제대로 볼 수 있도록 하기 위해서 필자가 적당한 값을 지정한 것이다. 독자의 컴퓨
터 속도에 따라 이 값을 적절히 지정하여라．


13.3.2. Source Code

// 이변수함수 iiView.cpp : im이帥entation of the CliView class
II

#include n stdafx.h"
荊nclude "이변수함수 ii.h"


荊nclude "이변수함수 iiDoc.h'
荊nclude "이변수함수 iiView.h"


#include <math.h>


#ifdef _DEBUG
#define new DEBUG_NEW
#undef THIS_FILE
static char THIS_FILE [1 = _FILE_;
#endif


///////////////////III/I/////II///II//II/II///II///I///I/////I/I////II////I//
II CliView

IMPLEMENTDYNCREATE (CliView, CView)


BEGIN_MESSAGE_MAP(CliView, CView)
      II { {AFX_MSG_MAP (CliView)
           II NOTE H the ClassWizard will add and remove mapping macros here.
           /7      DO NOT EDIT what you see in these blocks of generated code!
280 제3부 기초적인 3차원 컴퓨터 그래픽



     //} } AFX_MSG_MAP
     II Standard printing commands
     ON_COMMAND (TD_FILEPRINT, CView::OnFilePrjnt)
     ON_COMMAND (ID_FILE_PRINT_DIRECT, CView::OnFilePrint)
     ON_COMMAND (IDFILE_PRINT_PREVIEW, CView::OnFilePrintPreview)
END_MESSAGE_MAP 0


/////////////////////////////////////////////////////////////////////////////
II CliView construction/destruction


CliView: CliView 0
{
     /1 TODO: add construction code here


}

CliView:: -CIiView 0
{
}


BOOL CliView::PreCreateWjndow (CREATESTRUCT& cs)
{
     // TODO: Modify the Window class or styles here by modifying
     // the CREATESTRUCT cs


     return CView::preCreateWjndow (cs);
}

/////////////////////////////////////////////////////////////////////////////
// CliView drawing


void CliView::OnDraw (CDC* pDC)
                                                                                저13장 이변수함수의 그래프 281




{
     CliDoc* pDoc = GetDocumentO;
     ASSERT_VALID (pDoc);


     double y, x, z, xx, yy;
     const double pi=3.1415926535, radian=pi/180.0;
     double rotateZ=pi/10.0, rotateX=pi/4.0;


     pDC->S飢M叩Mode (！山江LOMETRIC) ;
     pDC- >SetViewportOrg (512, 350) ;


     for (y= -800.0; y<=800.0; y+=40.0)
           for (x= -800.0; x@800.0; x+=0.01)
           {
                 z = 120.0半cos (radian半sqrt (x來x+y半y) )+7.아cos (radian* 11.아sqrt (x*x+ y싹）);
                 xx = x*cos (rotateZ) -y*sin (rotateZ) ;
                 yy = z*cos (rotateX) - (- x*sin (rotateZ) -y*cos (rotateZ))半Sjn (rotateX);
                pDC->SetPixel (mnt (xx), mnt (yy), RGB (0,0,0));
           }
}

/////////////////////////////////////////////////////////////////////////////
II CliView printing


BOOL CliView::OnPreparePrinting (CPrintlnfo* plnfo)
{
     II default preparation
     return DoPreparePrinting (plnfo) ;
}

void CliView::OnBegmnPrmnting(CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
282 제3부 기초적인 3차원 컴퓨터 그래픽



     II TODO: add extra initialization before printing
}

void CliView::OnEndPrinting(CDC* /*pDC*/, CPrintlnfo* /*plnfo*/)
{
     II TODO: add cleanup after printing
}

///////////////////////////////////////////////////////I///III/////////////I/
II CliView diagnostics


#ifdef _DEBUG
void CliView::AssertValidO const
{
     CView::AssertValidO;
}

void CliView::Dump (CDumpContext& dc) const
{
     CView::Dump (dc);
}

CliDoc* CliView::GetDocument () II non-debug version is inline
{
      ASSERT (rnepDocument->IsKindOf (RUNTIME_CLASS (CliDocfl);
     return (CliDoc*)m_pDocument;
}
#end迂 仄DEBUG


//////////////////////////////////////I////I/////I/////I/II////II///I////I///
II CliView message handlers
                                       제］3장 이변수함수의 그래프 283




13.3.3. 프로그램 실행 결과


       二 아브i수맘수 h 니 꽤쩍엾善
       파딜（E)   편집（틔           도뭄말（d)
                                             髥題雙
                      보7Ky)
       口 畔日       > 難 凸       f
록 록
  A . 대한수학회 제공 수학 용어집
부 부
  B, 한국물리학회 공식 물리학 용어집
부록 A. 대한수학회 제공 수학 용어집




1-parameter group of transformations    algebraic differential equation
    1-매개변수변환군                               대수적 미분방정식
1-segment 1-선분                          싫gebraic singularity 대수적 특이점
午segment 于선분                            algebraically equivalent 대수적 동치（인）
a posteriori distribution 사후분포          싫most periodic function 거의 주기（적）함수
Abelian group 아벨 군, 가환군                 alternate interior angle 엇각
abs아ute differential calculus 절대미분학     alternating group 교대군
abs이ute differential 幻rm 절대미분형식         alternating multilinear mapping
accuracy 정확도                                 교태 다중선형사상, 교대 겹선형사상
action urn迂 처치한계                        alternating permutation 교대치환, 교대순열
action of a group 군의 작용                 analytic substitution 해석적 치환
additional sample 추가자료, 추가표본            angle bise아or 각의 이등분선
additive group 덧셈군, 가법군, 더하기군           ang蛇 of intersection 교각
adj이nt differential equation 수반미분방정식，   angle of segment 활꼴각
    딸림미분방정식                             angular 小splacement 각변위
admissible subgroup 허용가능 부분군            angular frequency 각진동수, 각주파수
affine chain 아핀사슬, 아핀연쇄                 annihilator differential operator
affine connection 아핀접속                      소멸미분작용소
affine coordinates 아핀좌표                 antiautomorphism 반자기동형사상
affine geometry 아핀기하학                   antiendomorphism 반자기준동형사상
affine group 아핀군                        antiperiodic function 반주기함수
affine mapping 아핀사상                     antipodal mapping 원점에 대칭인 사상
affine simplex 아핀단체                     aper幻dic state 비주기적 상태
affine space 아핀공간                       apothem of a regular polygon
affine transformation 아핀변환                  정다각형의 변심거리
affine 아핀                               approximate distribution 근사분포
age distribution 나이분포                   approximate integration 근사적분
키gebraic curve 대수곡선                     approximate solution 근사해
288 부록



approximation method 근사방법, 근사법        axiom of substitution 치환공리
approximation theorem 근사정리            back substiti川on 역대입법
approximation 근사, 어림셈                 backward d沮erence 후진차분
arc cosine 아크코사인, 역코사인                balanced sample 균형이 잡힌 표본, 균형표본
arc length 호의 길이                      Banach limit 바나흐 극한
arc 호                                 barycentric interpolation formula
Archimedian valuation 아르키메데스 부치           무게중심 보간공식
arcsecant 아크시컨트, 역시컨트                 base curve 밑곡선, 기저곡선
arcsine 아크사인, 역사인                     bell-shaped distribution 종모양분포
arctangent 아크탄젠트, 역탄젠트                Bessel equation 베셀 방정식
arcwise connected 호로 연결된, 호로 이어진      Bessel function 베셀 함수
arithmetic 小stribution 산술적 분포         Bessel interpolation 베셀 보간법
arithmetic of distribution function   Bessel's inequality 베셀 부등식
    분포함수의 계산                          best approximation 최적근사
arrow diagram 화살도표                    best linear approximation 최적선형근사
ascending difference 오름차분             Betti group 베티 군
associated Laguerre polynomial        between group 집단간
    부수된 라게르 다항식                       biadditive mapping 쌍가법사상, 겹덧셈사상
associated Legendre function          bicontinuous map1升ng 쌍연속사상, 겹연속사상
    부수된 르장드르 함수                       bicyclic group 쌍순환군
asymmetrical curve 비대칭곡선              bijective mapping 전단사사상, 일대일 대응사상
asymptotic curve 점근곡선                 bilateral exponential distribution
asymptotic distribution 점근적 분포            양방향 지수분포
autocatalytic curve 자기촉매곡선            binary search 이분탐색
automorphism 자기동형사상                   binomial coefficient 이항계수
auxiliary diagonal 보조대각선              binomial distribution 이항분포
auxiliary scale 보조자                   binom洌 equation 이항방정식
average extra defectives limit        binomial expansion 이항전개
    평균 여분불량수 한계                       binom洌 formula 이항공식
average of distribution 분포의 평균        binomial random variable 이항확률변수
average outgoing quality limit        binomial series 이항급수
    평균 출검품질 한계                        binomial theorem 이항정리
average sample number curve           binomial 이항（의）
    평균표본수 곡선                          bipolar coordinates 겹극좌표, 쌍극좌표
average sample number 평균표본수           bisection method 이분법
                                               부록 A . 대한수학회 제공 수학 용어집 289



bisector 이등분선                            cofactor 여인수
bivariate distrib的on 이변량분포               collinear p이nts 공선점, 동일 직선상의 점들
bivariate normal distribution 이변량 정규분포   co小near 동일 직선상（의）, 공선
Borel equivalence 보렐 동등                  collineation 공선사상
broken-line interpolation 굴절선 보간법，       column equilibration 열평형
    꺽은선 보간법                              column matr汶 열행렬
bulk sample 집단표본                         column vector 열벡터
Cantor diagonal process 칸토르 대각선 방법       column 열
cell frequency 칸 빈도                      combination 조합
central angle of a regular polygon       commensurable segment
    정다각형의 중심각                                같은 단위로 잴 수 있는 선분
central difference 중심차분                  common difference 공차
central limit theorem 중심극한정리             common factor 공통인수
characteristic base curve 특성기준곡선         common perpendicular 공통수선
characteristic curve 특성곡선                common tangent 공통접선
characteristic solution 특성해 , 고유해        commutative group 가환군
characteristic subgroup 특성부분군            commutator group 교환자군
check limit 감사한계                         commutator subgroup 교환자부분군
chi巾square distribution 카이제곱분포           complementary segment 여선분
circular arc 원호                          complete orthonormal set 완비 정규직교집합
circular permutation 원순열                 complete orthonormal system
circular truncated cone 원뿔대, 원추대             완비 정규직교계
circumscribed p이ygon 외접다각형               complete solution 완전해
class interval 계급구간                      completion 완비화
closed curve 닫힌 곡선, 폐곡선                  complex fraction 번분수
closed differential form 닫힌 미분형식，        composite mapping 합성사상
    폐미분형식                                composition series 조성열
closed interval 닫힌 구간, 폐구간               composition 합성
closed mapping 닫힌 사상, 폐사상                compound proposit幻n 합성명제
coefficient of correlation 상관계수          compressed limit 압축한계
coefficient of determination 결정계수        computer simul欲幻n 컴퓨터 모의실험，
coefficient of displacement 변위계수             컴퓨터 시뮬레이션
coefficient of variation 변동계수            computing machine 계산기
coefficient 계수                           concave p이ygon 오목다각형
cofactor expansion 여인수 전개                conceptual population 개념적 모집단
290 부록



concurrent lines 공점선                  contr이 limit 관리한계
concurrent 공점                         convergence in distribution 분포수렴
condition of congruence 합동조건          convex curve 볼록곡선
conditional distribution 조건부분포        convex polygon 볼록다각형
conditional proposition 조건명제          corrected trapezoid rule 수정된 사다리꼴 공식
confidence coefficient 신뢰계수           correlation coefficient 상관계수
confidence interval 신뢰구간              correlation factor 상관인자
confidence lim仕 신뢰한계                  cosine theorem 코사인정리
conformal mapping 등각사상                cosine 코사인
conforma伽 equivalent 등각동등한            cotangent bundle 공변접다발
congruence (mod m) 모듈 m에 관하여 합동       cotangent 코탄젠트
congruence class 합동류                  covariant differentiation 공변미분
congruence condition 합동조건             critical condition 임계조건
congruence criteria for triangles     critical length 임계길이
    삼각형의 합동조건                         critical p아nt 임계점
congruence ex可es前on 합동식               critical region 기각영역 , 기각역
congruence 합동                         critical rejection region 기각영역
congruent figure 합동도형                 critical value 임계값, 기각값
congruent figure 합동도형                 cube 삼승, 세제곱, 정육면체
congruent transformation 합동변환         cub이d 직육면체
congruent 합동（의）                       cumulative distribution function 누적분포함수
con如gate arc 켤레호, 공액호                 cumulative frequency distribution polygon
con如gate prior distribution 켤레 사전분포       누적도수분포 다각형
conjugate subgroup 켤레부분군, 공액부분군       cumulative frequency distribution table
constant of integration 적분상수              누적도수분포표
contingency coefficient 분할계수          cumulative frequency graph 누적도수그래프
continued fraction 연분수                cumulative frequency table 누적도수표
continuous distribution 연속분포          cumulative frequency 누적도수
continuous group 연속군                  cumulative relative frequency 누적상태도수
continuous mapping 연속사상               curve fitting 곡선 맞추기
continuous population 연속모집단           curve of constant breadth 폭이 일정한 곡선
continuous sample space 연속표본공간        curve of constant 引ope 기울기가 일정한 곡선
continuously differentiable 연속미분가능    curve segment 곡선분
contractive mapping theorem 축약사상정리    curve tracing 곡선의 추적
contraposition 대우                     curve 곡선
                                         부록 A . 대한수학회 제공 수학 용어집 291



curv小near p이ygon 굽은 다각형           difference equation 차분방정식
cycle decomposition 순환마디 분할       difference mod따e 차모듈
cyclic group 순환군                  difference operator 차분작용소
cyclic permutation 순환치환           difference quotient 차분몫
cyclic subgroup 순환부분군             difference set 차집합
damping coefficient 감쇠계수          difference 차, 차분, 차집합
damping factor 감쇠인자               differentiable function 미분가능 함수
data fitting 자료맞추기                differentiable manif이（:1 미분가능한 다양체
decimal part 소수부                  differentiable 미분가능한
decomposable measure 분해가능（한）측도    differential calculus 미분법, 미분학
decon巾osit向n 분해, 분할               differential coefficient 미분계수
defective s帥叩旭 불량표본               differential equation 미분방정식
definite form 정부호형식               differential form 미분형식
definite integral 정적분             differential geometry 미분기하학
definite quadratic form 정부호이차형식   differential of higher order 고계미분，
degenerate conic section 퇴화원뿔곡선       고차미분
degenerate distribution 퇴화분포      differential operator 미분작용소
degenerate eigenvalue 퇴화（된）고유치    differential quotient 미분몫
degenerate system 퇴화방정식계          differential 미분
degenerate 퇴화                     differentiation 미분
degree of scattering 산포도          dihedral group 정이면체군
delta singularity 델타 톡이성          direct indecomposable 직접기약
descending difference 내림차분        direct limit 귀납적 극한
development figure 전개도            direct motion 정향합동변환
diagonal 이e毗nt 대각선원소              directed distance 유향거리
diagonal line 대각선                 directed line segment 유향선분
diagonal matrix 대각선행렬             directed segment 유향선분
diagonal point 대각점                direction coefficient 방향계수
小agonal process 대각화 과정            direction cosine 방향코사인
diagonal subset 대각부분집합            directional coefficient 방향계수
diagonal triangle 대각삼각형           director curve 도선
diagonalizable 대각화 가능한            discontinuous group 불연속군
diagonalization 대각화               discrete distribution 이산분포
diffeomorphism 미분동형사상             discrete population 이산모집단
difference calculus 차분법           discrete random distribution 이산확률분포
292 부록



discrete time interval 이산시간구간        面uble sequence 이중수열
dispersion 산포, 흗어진                   double series 이중급수
displacen祀nt 변위                      面uble 針gn 겹부호, 복부호
distance 거리                          面ublet function 이중함수, 쌍극함수
distribution curve 분포곡선              面ubly periodic function 이중주기함수
distribution form 분포형                duplicating the cube
distribution function 분포함수               정육면체의 부피를 두배하기
distribution polygon 분포다각형           dynamic equilibrium 동력학적 평형
distribution table 분포표               edge of regress幻n 반퀴곡선
distribution 분포, 초함수                 efficiency factor 효율인자
distribution-free method             이ec甘ic displacement    전기변위
    분포에 의존하지 않는 방법                   elementary row and column operation
distribution-作ee 분포에 의존하지 않는             기본 행 및 열연산
divergence differential expression   이ementary solution 기본해
    발산미분식                            elimination method 소거법
divided difference 차분상               elimination 소거
division into equal parts 등분         endomorphism 자기준동형사상
面decagon 십이각형                        epimorphism 전사준동형사상，
double coset 이중잉여류                       위로의 준동형사상
面uble 이ement 이중원소                    equiangular triangle 정삼각형
double exponential distribution      equiareal transform 등적변형
    이중지수분포                           equicontinuity 동등연속（성）
double Fourier series 이중 푸리에 급수      equicontinuous family 동등연속함수의 모임
double integral 이중적분                 equicontinuous 동등연속인
double layer 이중층                     equ泊油ensional equation 등차원방정식
double line 이중선                      equidistant curve 등거리곡선
double 하ane 이중평면                     equilateral hyperb이a 직각쌍곡선
double p이nt 이중점                      equilateral p이ygon 등변다각형
double precision 배정밀도                equilateral trapez아d 등변사다리꼴
double product 이중곱                   equilateral triangle 정삼각형
double radical sign 이중근호             equ小bration 평형
double root 이중근                      equ小brium distribution 평형분포
double sampling inspection plan      equ小brium 평형
    이중추출검사법                          equimeasure transformation 등측도변환
double sampling 이중추출법                equipotent 대등
                                           부록 A . 대한수학회 제공 수학 용어집 293



equipotential curve 등위곡선            factorial experiment 요인분석법 , 요인실험
equipotential line 등위선              factorial moment generating function
equipotential surface 등위곡면              계승모멘트 생성함수
equipotential 등위의                   factorial moment 계승모멘트
equiscalar surface 등스칼라면            factorial 계승, 차례곱
equivalence class 동치류, 동등류          factorization in prime factors 소인수분해
equivalence relation 동치관계, 동등관계     factorization into primes 소인수분해
equivalence 동치 , 동등                 factorization 인수분해
equivalent event 동등사건, 동치사건         false 거짓
equivalent fraction 동치분수            family of curves 곡선족, 곡선의 모임
equivalent 동치인, 동등한                 family of distributions 확률분포의 모임
error of the first kind 제일종의 과오     fam泗 of functions 함수족, 함수의 모임
essential singular point 본질적 특이점，   fam加 of sets 집합족, 집합의 모임
    진성 특이점                          fam蜘 모임, 족
essential singul카ity 본질적 특이성        feasible solution 실현가능 해
evaluation homomorphism 부치준동형사상     fiber-preserving map 파이버보존사상
even permutation 짝순열, 짝치환           Fibonacci numbers 피보나치 수
exact d沮erential equation 완전미분방정식   fiduc洌 interval 신뢰구간
exact differential form 완전미분형식      fiducial limit 신뢰한계
exact differential 완전미분             figure 도형, 그림
expected cell frequency 평균셀도수       finer composition series 더 세분된 조성열
explicit s이ut向n 양함수해1, 양적인 해        finite d消erence 유한차분
exponential distribution 지수분포       finite group 유한군
exponential growth 지수적 증가           finite intersection property 유한교차성
exponential mapping 지수적 사상          finite interval 유한구간
extended기recision 확대된 정밀도           finite part 유한부분
的ter幻r common tangent 공통외접선         finite population correction 유한모집단 수정
extreme displacement 극대 변이          finite population 유한모집단
F-distribution F 분포                 finite simple continued fraction
factor analysis 인자분석（법）                  유한단순연분수
factor group 인자군                    finitely generated abelian group
 factor level 인자 수준                      유한생성 아벨 군
factor ring 잉여환                      finitely generated group 유한생성군
 factor set 인자집합                     first axiom of countability 제1가산공리
 factor 인자, 인수                       first category 제1범주
294 부록



first countable axiom 제1가산공리             frequency distribution 도수분포
first derivative test 일계도함수판정법           frequency of occurrence 출현도수
first fundamental form 제1기본형식            frequency of vibration 진동수
first kind 제1종                           frequency p이ygon 도수다각형
first passage time 첫통과시간                 frequency 도수, 진동수, 주파수
first term 초항, 첫째항                       full pivoting 전추축
first -order approximation 일차근사          functional scale 함수자
first-order differential equation        fundamental group 기본군
    일계 미분방정식                             fundamental solution 기본해
Fisher -Neyman factorization criterion   fundamental system of solutions
    피셔H네이만의 인수분해법                            해의 기본체계
focal distance 초점거리                      fuzzy coefficient 피지계수
foot of perpendicular 수선의 발              Galois group 갈루아 군
forward difference 전진차분                  gamma distribution 감마분포
forward elimination 전진소거                 Gaussian curve 가우스 곡선
forward substitution 전진대입                Gaussian 小stribution 가우스 분포
four group 사원군                           general angle 일반각
four vertex theorem 네꼭지점정리               general 5이ution 일반해
fraction defective 불량률                   general term 일반항
fract幻n 분수                               generalized Cantor set
fractional equation 분수방정식                    일반화된 칸토르 집합
fractional express向n 분수식                 generalized factorial function
fractional function 분수함수                     일반화된 계승함수
fractional inequality 분수부등식              generalized function 초함수
fractional part 분수부분                     geometric Brownian motion
fractional power 분수거듭제곱                      기하적 브라운 운동
fractional replication 부분실시법             geometric distribution 기하분포
fractional transformation 분수변환           glide reflection 미끄럼 반사변환
free Abelian group 자유 아벨 군               帥bal random search 대역적 우연탐색
free group 자유군                           g이den rectangle 황금비율 직사각형
frequency curve 도수곡선                     goodness of fit test 적합도검정
frequency distribution curve 도수분포곡선      goodness of fit 적합도
frequency distribution polygon           graded group 차수 붙은 군
    도수분포다각형                              graphical s이ut幻n 그래프풀이
frequency distrit乂ition tab地 도수분포표       greatest common divisor 최대공약수
                                              부록 A. 대한수학회 제공 수학 용어집 295



greatest comm이lfactor 최대공약수           horneomorphism 위상동형사상
greatest common measure 최대공약수         homogeneous condition 동차조건, 동질조건
greatest 이ement 최대원소                  homogeneous coordinates 동차좌표
                                          니




greatest integer function 가우스 정수함수，   homogeneous equation 동차방정식
    최대 정수함수                           homogeneous expression 동차식
greatest lower bound 하한, 최대하계         homogeneous function 동차함수
greatest monomial factor 최대단항인수       homogeneous p이ynomial 동차다항식
                                          니




group action 군의 작용                    homogeneous solution 동차해1
group algebra 군대수                     homogeneous surface 동차곡면, 동질곡면
group index 군지표                       homogeneous system of algebraic equations
group of h이onomy 홀로노미군                    동차대수방정식계
group of transformations 변환군          homogeneous system of linear equations
group representation 군의 표현                동차연립일차방정식
group ring 군환                         homogeneous 동차의, 동질의
group velocity 군속도                    horn이ogy group 호몰로지군
gr oup 군                              homomorphism 준동형사상
grouped data 집단화된 자료                  homotopy group 호모토피군, 연속변형군
grouped sequential inspection         hyperbolic cosine 쌍곡코사인
    집단 축차 추출검사                        hyperbolic sine 쌍곡사인
grouping 편가름                          hyperbolic tangent 쌍곡탄젠트
groupo沁 버금군, 준군                       hypergeometric distribution 초기하분포
growth 성장, 증가                         identity mapping 항등사상
half closod interval 반 닫힌 구간, 반폐구간    imaginary part 허수부분
half infinite interval 반무한구간          implicit d沮erentiation 음함수미분법
half open interval topology           implicit solution 음적인 해
    반 열린 구간 위상                        imprimitive group 비원시군
half open interval 반 열린 구간, 반개구간      improper fraction 가분수
half turn 반회전                         inclusion mapping 포함사상
Herm仕e interp이ation 에르미트 보간법          incongruent 합동이 아닌
hexagon 육각형                           indecomposable group 분해불가능 군
hexahedron 육면체                        indefinite equation 부정방정식
川erarch治1 subdivision 계층별 분류          indefinite integral 부정적분
higher commutator subgroup            indefinite quadratic form 부정부호 이차형식
    고차의 교환자부분군                        independent samples 독립표본
h이onomy group 홀로노미군                   index of dispers幻n 산포지표
296 부록



indexed fam蜘 of 이asses 지표가 주어진        interquartile range 사분위 범위
     유들의 모임 , 첨수된 유들의 모임              intersection angle 교각
inductive limit 귀납적 극한                intersection chart 공점도표
infer幻r arc 열호                        intersection number 만남의 수
infinite group 무한군                    intersection point 교점 , 만난점
infinite limit 무한극한                   intersection 만남, 교집합, 공통집합
infinite population 무한모집단             interval estimation 구간 추정
infinitely divisible distribution     interval function 구간함수
     무한 번 분해가능한 분포                    interval of convergence 수렴구간
inhomogeneous coordinates 비동차좌표       interval 구간
inhomogeneous 비동차의 , 비동질의             into mapping 안으로의 사상
initial segment 앞 절편                  intransitive group 비추이적 군
injective mapping 단사사상                intrinsic accuracy 내재정밀도
inner automorphism 내부자기동형사상           invariant subgroup 불변부분군
integer part 정수부분                     inverse interpolation 역보간법
integral part 정수부분                    inverse limit 역극한
integrand 적분될 함수, 피적분함수               inverse mapping 역사상
integration by parts 부분적분             involutive distribution 대합적 분포
integration by substitution 치환적분      irrational fraction 무리분수식
integration constant 적분상수             irreducible fraction 기약분수
integration 적분                        irreducible fractional expression 기악분수식
integrodifferential equation 미적분방정식   irregular singular point 비정칙 특이점
interior angle 내각, 안각                 irregular singularity 비정칙 특이성
interior angles on the same side      isogonal mapping 등각사상
     동측내각, 같은쪽 안각                     isolated essential singularity 고립된 본질적
interior 面main 내부영역                       특이점 , 고립된 진성 특이점
interior extremum theorem 내부극값정리      is아欲ed singular point 고립된 특이점
inter幻r point 내점 , 안점                 is아ated singularity 고립된 특이점
interior product 내부곱                  isometric mapping 등거리사상
interior 내부, 안의                       isometry 등거리변환
internal common tangent 공통내접선         isomorphic group 동형군
internal tangent 내접선                  isomorphism 동형사상
interpenetrating sample 상호관입표본        isosceles right triangle 직각이등변삼각형
interpolation function 보간함수           isosceles trapezoid 등변사다리꼴
interp이ation 보간법                      isosceles triangle 이등변삼각형
                                                 부록 /\. 대한수학회 제공 수학 용어집 297



isotropy group 등방군, 부동군                  least square estimate 최소제곱 추정값
iso甘opy subgroup 등방부분군, 부동부분군            least square estim砒or 최소제곱 추정량
iterated linear interpolation 반복된선형보간법   least square method 최소제곱법
卜shaped distribution卜형분포                 least upper bound 최소상계, 상한
Jacobi identity 야코비 항등식                  left side differential coefficient
Jacobi's syn由이 야코비 기호                         좌방미분계수, 왼쪽 미분계수
Jacobian determinant 야코비의 행렬식            left side limit 좌극한, 왼쪽 극한
Jacobian matr汶 야코비의 행렬                   left-hand tim仕 좌극한, 왼쪽 극한
Jacobian 야코비안, 야코비 행렬식                   Legendre's p아ynom洌 르장드르 다항식
佃nt conditional distribut由n 결합조건부분포      Legendre's syn由이 르장드르의 기호
何nt distribution function 결합분포함수         Legendre's transformation 르장드르 변환
佃nt 小stribution 결합분포                     legs of isosceles triangle
何nt frequency 결합도수                            이등변삼각형의 등변
兀rdan curve 조르당 곡선                       teptokurtic distribution 폭이 좁은 분포
judgment sample 유의표본, 판단추출법              Lie group 리군
 juxtaposition 병렬, 이음                    lifetime distribution 수명분포
K-sample K 표본                            lifting of map 사상의 올림
kurtos治 뾰족한 정도                           limit comparison test 극한비교판정법
 lack of fit 적합성 결여                      limit function 극한함수
Lagrange mutt巾tier method 라그랑즈 승수법       lim迂 inferior 하극한
Lagrange multiplier 라그랑즈 승수              limit of error 오차의 한계
 Lagrange's parenthesis 라그랑즈의 괄호         limit of filterbase 필터기저의 극한
 Laguerre's p이ynom洌 라게르 다항식              limit of integration 적분한계
 large sample approximation 대표본근사        limit ordinal number 극한순서수
 large sample 대표본                        lim仕 point 집적점 , 쌓인점 , 극한점
 lattice distribution 격자분포               limit superior 상극한
 lattice group 격자군                       limit 극한, 한계, 극한（값）
 leading diagonal 주대각선                   limiting circle 극한원
 least common denominator 최소공분모          limiting distribution 극한분포
 least common multiple 최소공배수             limiting moment generating function
 least 이ement 최소원소                             극한모멘트생성함수
 least positive residue 최소양의 잉여           limiting probability 극한확률
 least splitting field 최소분해체              line of 이ectric displacement 전기변위선
 least square approximation 최소제곱근사        line of intersection 교선
 least square criterion 최소제곱판정법           tine of regression 회귀선
298 부록



line segment 선분                         marginal of sample 표본의 주변
linear approximation 일차근사, 선형근사         marginal probability function 주변확률함수
linear combination 일차결합                 marginal revenue 한계수익
linear congruence 일차합동                  marginal value 한계값
linear d沮erential operator 선형미분작용소      market research 시장조사
linear fractional transformation        master sample 마스터표본
     선형（일차）분수변환                         matr汶 diagonalization 행렬의 대각화
linear mapping 선형사상                     maximal commutative group 극대가환군
linear ordinary differential equation   maximal normal subgroup 극대정규부분군
     선형상미분방정식                           maximum sample value 최대표본값
linear partial differential equation    mean dispersion 평균산포도
     선형편미분방정식                           mean square approximation 평균제곱근사
linear regression analysis 선형회귀분석       measuration by parts 구분구적법
linear regression 선형회귀 , 직선회귀           measure of dispersion 산포도, 분산도
linear span 선형생성 부분공간                   med治n line 중선
linear T-approximation                  median 중앙값
     선형卜근사, 일차卜근사                       meromorphi帥l 준준동형사상, 유리형사상
local s이ut幻n 국소해                        meta-Abelian group 메타아벨 군
local truncation error 국소 절단오차          method of equivalence 등치법
locally one-to-one mapping              method of least squares 최소제곱법
    국소 일대일 사상                           method of substitution 대입법
logarithmic differentiation 로그미분법       method of successive approximation
logistic distribution 로지스틱분포                축차근사법
lognormal distribution 로그정규분포           method of successive substitution
lower differential coefficient 하미분계수        축차대입법
lower lim仕 아래 끝, 하단                     method of undetermined coefficients
lower triangular 하부삼각（행렬）,                  미정계수법
    아래 삼각（행렬）                           metric coefficient 계량계수
magic square 마방진                        middle quartile 중앙사분위
main diagonal 주대각선                      minimax approximation 최대최소근사값
main scale 어미자                          m而mum san叩地 value 최소표본값
mapping 사상                              minor angle 열각
marginal cost 한계비용                      minor arc 열호
marginal density function 주변밀도함수        minor axis 단축, 짧은 축
marmnal distribution 주변분포               minor defect 작은 결점
                                                    부록 A . 대한수학회 제공 수학 용어집 299



minor determinant 소행렬식                       negative definite 음의 정부호
minor diameter 짧은지름                          negative semidefinite 음의 준정부호
minor premise 소전제                            nested interval 축소구간
minor segmemt 열활꼴, 작은쪽 활꼴                    nested intervals 可operty 축소구간 성질
minor submatr怏 소부분행렬                         nilpotent group 거듭제곱이 영인 군
minor 소행렬식                                   non-differentiable function 미분불가능 함수
m汶ed fraction 대분수                            non-normal population 비정규모집단，
m汶ed scalar product 혼합된 스칼라적，                    정규가 아닌 모집단
    혼합된 내적                                   non-parametric confidence interval
modified Bessel function of the first kind       비모수적 신뢰구간
    제1종 변형 베셀 함수                             non-parametric inference 비모수적 추론，
mod小ed regula falsi 수정된 오차조정법                non-parametric test 비모수적 검정
monomorphi師1 단사준동형사상                         non-parametric 모수에 의존하지 않는，
monotone convergence theorem                     비모수적
    단조수렴정리                                   nondegenerate conic 정상적 원뿔곡선
mon야one decreasing 단조감소                      nondegenerate critical 呵nt 정상적인 임계점
mon아one function 단조함수                        nondegenerate matr汶 정상적 행렬，
mon아one increasing 단조증가                          퇴화되지 않은 행렬
monotone sequence 단조수열                       nondegenerate 정상적인, 퇴화되지 않은
monotone 단조                                  nonhomogeneous boundary condition
morphism 사상                                      비동차경계조건
motion 합동변환, 운동                              nonhomogeneous coordinate 비동차좌표
moving singularity 움직이는 특이점                  nonhomogeneous differential equation
multinomial distribution 다항분포                    비동차 미분방정식
mult巾licative group 곱셈군                      nonhomogeneous linear differential equation
multivariate normal distribution                 비동차 선형 미분방정식
    다변량정규분포                                  nonhomogeneous Poisson process
n-ply transitive group n중 추이군                    비동질 포아송 과정
n-th potential resi加en제곱잉여                   nonhomogeneous problem 비동차 문제
natural map 표준사상, 자연사상                       nonisolated singularity
negative binomial random variable                고립되지 않은 특이성 , 비고립 특이점
    음의 이항확률변수                                nonlinear interaction 비선형 상호작용
negative definite form 음의 정부호형식              nonlinear 비선형
negative definite quadratic form             nonlinearity 비선형성
    음의 정부호 이차형식                              nonnegative definite 음이 아닌 정부호
300 부록



nonsingular matrix 정칙행렬                number of samples 표본의 수
nonsingular 정칙                         numerical calculation 수치계산법
nontrivial solution 자명하지 않은 해          numerical differentiation 수치미분
nontrivial subgroup 자명하지 않은 부분군        numerical equation 수치방정식
norm 노름                                numerical expression 수치적 표현
normal acceleration 법선가속도              numerical instability 수치적 불안정（성）
normal approximation to binomial       numerical integration 수치적분
    이항의 정규근사                           numerical method 수치계산법
normal approximation 정규근사              numerical quadrature 수치구적법
normal coefficient 표준계수                numerical solution 수치해
normal dispersion 정규산포도                numerical 수치（의）
normal distribution curve 정규분포곡선       oblique cube 빗육면체
normal distribution table 정규분포표        odd permutation 홀치환, 기치환
normal distribution 정규분포               one-sided confidence interval
normal fam泗 정규족                            한쪽 신뢰구간, 단측신뢰구간
normal population 정규모집단                one-sided limit 한쪽 극한
normal subgroup 정규부분군                  one나0-one map 일대일 사상
normal 법선, 표준, 정규                      one나于one mapping 일대일 사상
normalization of freciuencv function   onto map 위로의 사상, 전사사상
    도수분포의 정규화                          open interval 열린 구간, 개구간
normalized floating-ooint number       open mapping theorem 열린 사상정리
    정규화된 부동소수                          open maj珂ng 열린 사상
normalized 싱卄화뇐                        operator automorphism 작용소동형사상
normalizer 정규화부분군                      operator homomorphism 작용소준동형사상
nowhere differentiable function        opposite motion 역향합동변환
    어디에서도 미분불가능한 함수                    optimal solution 최적해
null event 공사건                         orbital mar河ng 궤도사상
null function 영함수                      ordered triple 순서있는 서］ 짝
null hypothesis 귀무가설                   ordinary differential equation 상미분방정식
null set 공집합                           ordinary point 보통점
null space 영공간                         orientated intersection number
null system 영체계                            방향（을 고려한） 교차수
null vector 영벡터                        orientation preserving isometry
null-horn아opic 아호모토픽, 아연속변형의               향 보존 등거리사상
nullity 영공간의 차원, 핵공간의 차원               oriented segment 유향선분
                                          부록 A . 대한수학회 제공 수학 용어집 301



orthocenter 수심                     partial correlation 편상관
orthogonal array 직교배열              partial derivative 편도함수
orthogonal comj코ement 직교여공간        partial 小fferentiable 편미분가능
orthogonal component 직교성분          partial differential equation 편미분방정식
orthogonal coordinates 직교좌표        partial d沮erential 편미분
orthogonal function 직교함수           partial d沮erentiation 편미분
orthogonal group 직교군               partial dispersi이1 부분산포도
orthogonal matrix 직교행렬             partial enumeration 부분조사
orthogonal pr이ection 정사영           partial fraction 부분분수
orthogonal set 직교집합                partial inspection 일부조사
orthogonal squares 직교방격            partial integration 부분적분
orthogonal system 직교체계             partial order 부분순서
orthogonal trajectory 직교절선         partial ordering 부분순서
orthogonal transformation 직교변환     partial pivoting 부분적 추축
orthogonal 직교                      partial product 부분곱
orthogonality relation 직교관계        partial sequence 부분（수）열
orthogonality 직교성                  partial sum 부분합
orthogonalization 직교화              partial velocity 편속도
orthonormal has治 정규직교기저            partial wave expansion 부분파동 전개
orthonormal set 정규직교집합             partially ordered class
orthonormal system 정규직교체계              부분순서가 있는 모임（류）
orthonormalization 정규직교화           partially ordered set 부분순서가 있는 집합
osculatory interp이ation 접촉보간법      partiar denominator 부분분모
outer automorphism 외부자기동형사상        particular solution 특수해1
outer con甘이 limit 외측관리한계           partition of unity subordinated to a covering
少group p군                               한 덮개에 종속된 단위분할
p-quartile p분위수                    partition of unity 단위분할
parallel displacement 평행이동         partition 분할, 가름
parallelopiped 평행육면체               perfect 얍oup 완전군
parametric curve 매개（변수）곡선          periodic decimal 순환소수
parametric equation 매개（변수）방정식      periodic extens幻n 주기 확장
parametric function 모수함수           periodic function 주기함수
parametric representation 매개변수표현   periodic motion 주기운동
paried difference 짝의 차             periodic point 주기점
partial correlation ratio 편상관비     periodicity modulus 주기모수
302 부록



periodicity 주기성                         p아ar form 극형식
permutation group 치환군                   p이ar line 극선
permutation 순열, 치환                      p이ar 하ane 극평면
perpendicular bisector 수직이등분선           polar tangential coordinates 접선극좌표
perpendicular 미ane 수직평면                 p이ar vector 극벡터
perpendicular 수직, 수선, 직교                polar 극
Pfaffian differential equation          p이ygon 다각형
    파피안 미분방정식                           p이ygonal approximation 다각형근사
Pfaffian d沮erential form 파피안 미분형식       polygonal function 다각형함수
Picard successive approximation         polygonal line 꺾은선
    피카드의 계속적 근사                         p이ynomial approximation 다항식근사
piecewise cubic interpolation           p이ynomial distribution 다항분포
    구분적 삼차보간법                           p이yno而al interp이ation 다항식보간법
piecewise differentiability 조각적 미분가능성   p이ynom洌 regression 다항회귀
piecewise polynomial interpolation      pooled estimate of variance
    조각적 다항식보간법                              분산의 합동 추정값
p如야 entry 피보트성분                         population 小stribution 모집단분포
pivot 선회축, 추축, 피보트                      population mean 모평균
pivotal 이en祀nt 중심원소                     population parameter 모집단의 모수
pivotal equation 중심방정식                  population ratio 모비율
pivoting strategy 추축연산 전략               1兀pulation standard deviation 모표준편차
pivoting 추축연산                           population variance 모분산
하anar p이ygon 평면다각형                      population 모집단
하ane figure 평면도형                        position of 帥nilarity 닮음의 위치
하ane of regression 회귀평면                 position vector 위치벡터
하ane wave 평면파동                          position 위치
Poincare group 기본군                      positive definite form 양의 정부호형식
Poisson approximation to binomial       positive definite quadratic form
    이항의 푸아송근사                               양의 정부호 이차형식
Poisson distribution 푸아송분포              positive definite 양의 정부호
polar axis 기선, 극축                       positive part of a function 함수의 양의 부분
polar coordinate system 극좌표계            1兀엷tive semidefinite 양의 준정부호
p아ar coordinates 극좌표                    precision attained 달성될 정밀도
p이ar curve 극곡선                          precision prescribed 요구되는 정밀도
polar equation 극방정식                     precision reached 도달되는 정밀도
                                            부록 A . 대한수학회 제공 수학 용어집 303



precision 정밀도                        pseudo-vector 유사벡터
primitive group 원시군                  purposive sample 유의표본
primitive mapping 원시사상               Pythagoras theorem 피타고라스 정리
principal composition series 주조성렬    quadrant test 사분원 검정
principal diagonal 주대각선              quadrant 사분면
principal part 주요 부분, 으뜸 부분          quadratic approximation 이차근사
principle of least action 최소작용의 원리   quadratic residue 제곱잉여
princi히e of superposition 중첩의 원리     quartile deviation 사분위편차
prior distribution 사전분포              quartile 사분위수
probability distrib岫on 확률분포          quasi니nterp이ation operator 준보간작용소
probability limit 확률극한, 확률한계         quatern幻n group 사원수군
probability sample 확률표본              quotient group 상군, 몫군
product of proposition 명제의 곱         random interval 확률구간
可ogre ssion of d泌erences 계차수열        random sample 확률표본, 임의 표본
pr이ected figure 투영도                  rational fraction 유리분수
pr이ected scale 투영자                   reciprocal difference 역차분
projective coordinate ax恰 사영좌표축      reciprocal dispersion 역분산
pr이ective coordinates 사영좌표           rectangle graph 직사각형 그래프
pr이ective mapping 사영사상               rectangle 직사각형
proper coordinate patch 고유 좌표조각      rectangular coordinate system 직교좌표계
proper fraction 진분수                  rectangular coordinates 직교좌표
proper map 고유사상                      rectangular distribution 직사각형분포
proper subgroup 진부분군                 rectangular parallelopiped 직육면체
proper (map) 적절한                     rectified sine wave 정류 사인 파동
proportional distribution 비례배분       recursion 幻rmula 점화식
proposition 명제                       recursion 반복, 되풀이
propositional function 명제함수          recursive definit向n 귀납적 정의
pseudo- 유사의                          recursive function 귀납적 함수
pseudo-code 유사부호                     recursive 되풀이하는, 귀납적
pseudo니nverse 유사역원                   recursively enumerable set
pseudo-metric 유사거리                       귀납적으로 셀 수 있는 집합
pseudo-norm 유사노름                     reduced row-eche幻n form 기약 행 사다리꼴
pseudo-random number 유사난수            reduced scale 축척
pseudo-scalar 유사스칼라                  reduc而地 fraction 약분가능 분수
pseudo-sphere 의구, 유사구면               reduction of fraction 귀류법
304 부록



reference scale 참고자                    residue class 잉여류
refraction 굴절                          residue theorem 유수（의） 정리
regression analysis 회귀분석               residue 유수, 나머지 , 잉여
regression coefficient 회귀계수            res이ution 분해
regression curve 회귀곡선                  rhombus 마름모
regression equation 회귀방정식              right differentiable 오른쪽 미분 가능
regression estimate 회퀴추정값              right differential coefficient
regression line 회귀직선                        우미분계수, 오른쪽 미분계수
regression 회귀                          right hand limit 우극한, 오른쪽 극한
regular falsi 오차조정（법）                  right handed coordinate system
regular hexagon 정육각형                        오른손 좌표계
regular hexahedron 정육면체                right side differential coefficient
regular mapping 정칙사상                        오른쪽 미분계수, 우방미분계수
regular n-p이ygon 정n각형                  right side limit 우극한, 오른쪽 극한
regular parametric representation      right-handed coordinate frame
    정칙매개변수표현                                오른손 좌표틀
regular polygon 정다각형                   rotational group 회전군
regular singular point 정칙특이점           row vector 행벡터
regular singularity 정칙특이점              row 행
reg山ar truncated pyramid 정각뿔대          row-echelon form 행 사다리꼴
relative coordinates 상대좌표              san叩旭 design 표본설계
relative dispersion 상대산포도              sample distribution 표본분포
relative hom이ogy group 상태호몰로지군         sample inspection 추출검사
removable singular point 없앨 수 있는 특이점   sample ma川mum value 표본최대값
removable singularity 없앨 수 있는 특이점      sample mean 표본평균
repeated combination 중복조합              sample rate 표본비율
repeated permutation 중복순열              sample 針ze 표본의 크기
reproductive property of binomial      sample space 표본공간
    이항분포의 재생성                          sample standard deviation 표본표준편차
residual correction 나머지 수정             sample survey 표본조사
residual set 나머지 집합, 잉여 집합             sample variance 표본분산
residual sum of squares 잔차의 제곱합        sample 표본
residual 잉여의， 잉여 , 잔차                  sam1小ng distribution 표본분포
residue class field 잉여류체               sampling fract向n 추출비 , 추출율
residue class ring 잉여류환                samj小ng interval 표본추출간격
                                               부록 A. 대한수학회 제공 수학 용어집 305



saw나ooth wave 톱니모양 파동                   simplicial partition 단체분할
scalar curvature 스칼라곡률                  Simpson's formula 심프슨의 공식
scalar density 스칼라밀도                    Simpson's rule 심프슨의 법칙
scalar function 스칼라함수                   엷mutation 모의 실험 , 시뮬레이션
scalar mult巾le 스칼라배                     simultaneous confidence interval
scalar mutt巾lication 스칼라곱                   동시신뢰구간
scalar product 스칼라적 , 내적                simultaneous differential equation
scalar 스칼라                                  연립미분방정식
scale of notation 기수법                   simultaneous distribution 동시분포
scale 눈금, 축척                            sine curve 사인곡선
scalene triangle 부등변 삼각형                sine law 사인법칙
scatter diagram 점도표                     sine rule 사인법칙
segment of a circle 활꼴                  sine theorem 사인정리
segment 선분, 활꼴                          針ne 사인
self니ntersec如n number 자기 교차수            single precision 단순정밀도
self-orthogonal family of curves        singular c아lom이ogy 특이 코호몰로지
    자기직교곡선모임                            singular curve 특이곡선
semi-definite quadratic form            섧ngular horn이ogy 특이 호몰로지
    준정부호 이차형식                           singular solution 특이해
semi-positive definiteness 준정부호성        skew position 꼬인 위치
semigroup representation 반군표현           skewness 일그러짐, 비틀림
semigroup 반군                            slicing map 조각사상
separable differential equation         없ope of regression line 회귀직선의 기울기
    분해가능한 미분방정식                         small sample 소표본
separating family of gauges             solid figure 입체도형
    게이지의 분리모임                           solution set 해집합
series solution 급수해                     solution space 해공간
set of the first category 제1범주의 집합      solution 해, 풀이
shear 전단응력 , 층밀림변환                      solvable group 가해군
signed measure 부호가 붙은 측도                space figure 공간도형
針gned rank test 부호순위검정                  span 생성, 펼침
師riilar figure 닮은 도형                     spanned 생성된
simple correlation coefficient 단순상관계수    spec而ed limit 지정한계
前n叩旭 group 단순군                           spectial linear group 특수선형군
simple proposition 단순명제                  spectral resolution 스펙트럼 분해
306 부록



spherical coordinates 구면좌표           symmetric d沮erence 대칭차
spherical figure 구면도형                symmetric figure 幻r a line 선대칭도형
spherical p이ar coordinate 구면극좌표      symmetric figure 幻r a plane 면대칭도형
spherical p이ygon 구면다각형               symmetric figure 幻rap아nt 점대칭도형
spherical segment 구면대                symmetric figure 대칭도형
standard Brownian motion 표준 브라운 운동   symmetric group 대칭군
standard normal 小stribution 표준정규분포   svmn祀tr兀 law 대칭률
statistical probab小ty 통계적 확률         symmetric matrix 대칭행렬
statistical series 통계계열              symmetric operator 대칭작용소
statistical table 통계표                S恥nmetr兀 point 대칭점
statistics of attributes 속성통계        symmetric polyhedron 대칭다면체
statistics of variable 변수통계          symmetric polynomial 대칭다항식
statistics of variates 변량통계          symmetric relation 대칭관계
statistics 통계학                       symmetric tensor 대칭텐서
stochastics 확률론                      symmetric transformation 태칭변환
student's distribution 학생의 분포        symmetric transposition 대칭이동
student's卜statistic 학생 t통계량          symmetrical 小叩lacement 대칭이동
subgroup 부분군                         symmetrical distribution 대칭분포
subsequential urn仕 부분수열 극한           symmetrical figure 대칭도형
substitution 대입, 치환                  symmetrical test 대칭검정
successive approximation method      symplectic group 사교군, 심플렉틱군
    축차근사법                            system of coordinates 좌표계
successive differentiation 축차미분법     system of orthogonal functions
successive displacement 축차변위             직교함수체계
sufficient statistic 충분통계량           system of orthonormal function
sum of prof兀엷tions 명제의 합                 정규직교함수체계
summation by parts 부분합               system of residues 잉여계
superior arc 우월호                     table of differences 차분표
superposition 겹침, 중첩                 tabular 小fference 표차
supers아vable group 초가해군              tangent bundle 접다발, 접속
surface fitting 곡면 맞추기               tangent circle 접원
surface wave 곡면파동                    tangent line 접선
surjection 전사함수, 전사, 위로의 함수          tangent 히ane 접평면
Sylow group 실로우군                     tangent point 접점
Sylow subgroup 실로우부분군                tangent space 접공간
                                             부록 A. 대한수학회 제공 수학 용어집 307



 tangent vector 접벡터                   transposition matrix 호환행렬
 tangent 탄젠트, 접선                      transposition 호환, 자리바꿈, 이항
 tangential component 접성분             transversal ' intersection 횡단교차
 tangential i고ane 접평면                 trapezoid rule 사다리꼴공식
 target population 목적 모집단             trapezoid 사다리꼴
 tempered distribution 조절된 초함수        trapezoidal rule 사다리꼴공식
 term-by-term integration 항별적분        triangular 幻rm 삼각꼴
 termwise differentiation 항별미분        triangular ma甘汶 삼각꼴행렬
 termwise integration 항별적분            triangul可 number 삼각수
 test of statistical hypothesis       triangular prism 삼각기둥
     통계적 가설검정                         triangular pyramid 삼각뿔
test statistic 검정통계량                 triangular survey 삼각측량
tetracyclic coordinates 사원좌표         triangularization 삼각형화
the greatest 최대                      tridiagonal matr汶 삼중 대각행렬
the least 최소                         tr小near coordinates 삼선좌표
theorem of three perpendiculars      triple integral 삼중적분
     삼수선의 정리                         trip旭 interaction 삼인자 교호작용
theory of groups 군론                  triple product 삼중적 , 혼합적
t이erance interval 허용구간               triple ratio 세제곱비
t이erance limits 허용한계                 triple root 삼중근
topological group 위상군                triple scalar product 스칼라 삼중적
topological mapping 위상사상             triple 세짝
torsion coefficient 꼬임계수             trivial subgroup 자명한 부분군
torsion free group 꼬임이 없는 군          truncate 절단하다
torsion group 꼬임군                    truncated circular cone 원뿔대
tors幻n subgroup 꼬임 부분군               truncated distribution 절단된 분포
的tal differential equation 전미분방정식    truncated pyramid with square bases
total differential form 전미분형식            정사각뿔대
total differential 전미분               trunc欲ed pyramid 각뿔대
total pivoting 전추축                   truncation error 단절오차
transfinite recursion 초한반복           unbiased estimate of population variance
transformation group 변환군                 모분산의 불편추정값
transformation of coordinates 좌표변환   undetermined coefficient 미정계수
transition map 추이사상                  uniform d沮erentiab小ty 고른 미분가능성
transitive group 추이군                 uniform distribution 고른 분포, 균등분포
308 부록



uniform equivalent 고르게 동등한
uniform homeomorphism 고른 위상동형사상
uniform isomorphism 고른 동형사상 '
unimodal dist曲ution 단봉분포
unique solution 유일한 해
unit cube 단위정육면체
unit distance 단위거리
unital homomorphism 단위적 준동형사상
upper d沮erential coefficient 위 미분계수
upper urn仕 위끝, 상극한
variable of integration 적분변수
vector difference 벡터의 차
vertex 꼭지점
waiting time 小stribution 기다리는 시간분포
wave equation 파동방정식
wave front 파면
wave function 파동함수
wei帥ted average 가중평균
wei帥ted mean 가중평균
working mean 가평균
zone of indifference 검사속행역
부록 B. 한국물리학회 공식 물리학 용어집



absolute differential calculus 절대미분학   angle of deviation 편향각
abs아ute 이ectromagnetic un迂             ang蛇 of minimum deviation 최소 편향각
    절대전자기단위                            angle of reflection 반사각
absolute motion 절대운동                   angular acceleration 각가속도
absolute system of units 절대단위계         angular frequency 각진동수
absolute unit system 절대단위계             angular momentum 각운동량
abs이ute zero point 절대영도점               angular   momentum operator   각운동량연산자
absolute zero potential 절대영전위          angular momentum operator 각운동량작용소
absorptive power 흡수능                   angular momentum quantum number
accelerated motion 가속도운동                   각운동량 으弘｝수
acceleration 가속도                       angular momentum quantum number
acoustical vibration 소리떨기                  부양자수
acoustical vibration 음향떨기              anharmonic oscillation 비조화 진동
AC power source 교류전기샘                  anode 양극
AC power source 교류전원                   anode 플러스극［전지의］
action integral 작용적분                   ano（扼 glow 양극 글로
AC v아tage 교류전압                         anode ray 양극선
adiabatic potential 단열퍼텐셜              antinode loop 배고리［파동의］
adiabatic potential 열끊음퍼텐셜             antireflection film 반사방지막
air column 공기기둥                        司丑anatic point 구면수차 지움점
air column resonance apparatus         applied physics 응용물리
    공기기둥 공명장치                          applied physics 응용물리학
air column resonance apparatus         Archimedes'principle 아르키메데스의 원리
    공기기둥 껴울림장치                         arm of moment 모멘트의 팔
air table 공기부상대                        articulation point 마디점
alternating current voltage 교류전압       astrophysics 천체물리학
analog- digital converter              atmospheric barometer 기압계
     아날로그m디지탈 변환기                      就omic dip이e 원자쌍극
aner아d barometer 아네로이드 기압계             atomic dip이e 원자쌍극자
引0 부록



欲omic 이ectron 원자내 전자                   barrier permeability 가로막이 투과율
atomic 이ectron shell 원자의 전자 껍질         barrier permeability 장벽 투과율
카omic mass unit [=amu] 원자 질량 단위        Bartlett's exchange operator
atomic physics 원자물리학                       바틀레의 교환연산자
atomic un仕 원자단위                        Bartlett's exchange operator
砒omic vibration 원자떨기                       바틀레의 바꿈연산자
audio frequency [=AF] 가청진동수            Bartlett force 바틀레 힘
audio frequency [=AF] 들림진동수            Bartlett interaction 바틀레 상호작용
aud幻 frequency amplifier 가청진동수 증폭기     Bartlett interaction 바틀레 서로작용
audio frequency oscillator 가청진동수 발진기   barycenter 무게중심
Auger 이ectron 오제 전자                    barycenter 질량중심
average acceleration 평균가속도             baryon 바리온
average deviation 평균편차                 baryon 중입자
average power 평균일률                     baryon number 바리온수
axial vector 축성벡터                      baryon number 중입자수
axis of precession 세차축                 bending moment 휨 모멘트
back reflection method 뒷쪽되비침법          betatron oscillation 베타트론 진동
back reflection method 뒷쪽반사법           bias voltage 바이어스 전압
ballistic pendulum 충격흔들이               bicritical p아nt 겹고비점
ballistic pendulum 탄동흔들이               bicritical point 쌍임계점
bar 바아［기압단위］                           bimolecular recombination 두 분자 재결합
bare mass 맨질량                          biophysics 생물물리학
bar magnet 막대자석                        bo小ng p이nt 끓는점
barn 바안［단면적의 단위］                       bo小ng-point 이evation 끓는점 오름
barometer 기압계                          bombarded particle 맞음알갱이
barometer 기압재개                         bombarded particle 피격입자
barometric distribution 기압분포           bombarding particle 두들김알갱이
barometric pressure 기압［단위］             bombarding particle 포격입자
barrel di飢아tion 통모양 일그러짐               bombardment 두들김
barrier 가로막이                           bombardment 포격
barrier 장벽                             bonding molecular orbital
barrier height 가로막이 높이                     결합성 분자 궤도함수
barrier height 장벽 높이                   Borda's pendulum 보르다의 흔들이
barrier penetration 가로막이 투과            bound 이ec甘on 속박된 전자
barrier penetration 장벽투과               bound 이ectron 얽매인 전자
                                          부록 B. 한국물리학회 공식 물리학 용어집 311



bound motion 속박운동                      Celsius temperature 섭찌온도
bound motion 얽매인 운동                    Celsius temperature scale 섭씨온도눈금
bound motion 유한구간운동                    center of mass motion 질량중심 운동
Bragg reflection 브래그 되비춤               center of oscillation 진동중심
Bragg reflection 브래그 반사                central potential 중심퍼텐셜
bra vector 브라벡터                        centrifugal barrier 원심힘 가로막이
bridge circuit 다리흐름길                   centrifugal governor 원심 속도 조절기
bridge circuit 브리지 회로                  centripetal acceleration 구심가속도
British thermal un仕 [=BTU] 영국 열단위      CGS 이ec甘omagnetic unit
Brownian motion [=Brownian movement]       시지에스 전자기단위
    브라운 운동                             CGS system of unit 시지에스 단위계
bulk 덩치                                CGS unit 시지에스 단위
bulk 부피                                characteristic frequency 특성 진동수
bulk 체적                                chemical physics 화학물리학
bulk effect 덩치효과                       chemical potential 화학퍼텐셜
bulk expansion coefficient 부피불음곁수      circular arc 원호
bulk modulus 부피 튐성률                    circular birefringence 원편광 겹꺾임
bulk modulus 체적 탄성율                    circular conical surface 원뿔면
bulk motion 통째운동                       circular 小chr이sm 원편광이색성
bulk sample 덩치시료                       circular double refraction 원편광 두 번꺾임
Burger's vector 버거의 벡터                 circular duplex 원형 이중나사선
can（끄e power 광도                        circular fringe 원형무늬
candle power 촉광［단위］                    circular motion 원운동
canonically conjugate momentum         circular oscillation 원떨기
    바른틀 켤레운동량                          circular oscillation 원진동
canonically conjugate momentum         circular p이ar切ation 원편광
    정준공액 운동량                           circular p이arized light 원편광
capacitor 들이                           circular pulse 원형펄스
capacitor 전기들이                         circular truncated cone 원뿔대
capacitor 축전기                          circular wave guide 둥근 파동길잡이
cardinal point (s) 방위 기점               circular wave guide 원형도파관
cardinal point (s) 주요점                 circun迂erence 원둘레
celestial mechanics 천체역학               circumference 원주
Celsius degree 섭씨도                     circumscr巾tion 바깥접함
Celsius scale 섭씨눈금                     circumscription 외접
312 부록



classical hypothesis 고전가설                  configuration integral 배위적분
classical mechanics 고전역학                   configuration integral 짜임새 적분
classical physics 고전물리학                    conical helix 원뿔 나사선
closed 이ec甘on shell 닫힌 전자껍질                conical pendulum 원뿔흔들이
closed mercury column manometer            conical refraction 원뿔꺽임
    폐관 수은압력계                               conical refraction 원추굴절
cloud 하lysics 구름 물리학                       conical section [=conic section] 원뿔곡선
coefficient of electrostatic potential     conical symmetry 원뿔 대칭
    정전기전위곁수                                conservation of angular momentum
coefficient of reflection 되비침곁수                각운동량보존
coefficient of reflection 반사곁수             conservation of momentum 운동량보존
coherent-light source 결맞는 빛샘               constant acceleration 등가속도
coherent potential approximation           constant current source 일정 전류샘
    결맞는 퍼텐셜 어림법                            constant of motion 운동의 상수
collective angular momentum 집단 각운동량        constrained motion 구속된 운동
collective motion 집단운동                     contact point 접점
column 기둥                                  contact potential difference 접촉전위차
column 열                                   continuous oscillation 연속진동
column vector 세로줄 벡터                       contravariant vector 반대바뀜벡터
completeness 완전성                           core 이ectron 속전자
complete orthogonal system 완전직교계           Coriolis' acceleration 코리올리의 가속도
complete set 완전집합                          Coulomb's law 쿨롱의 법칙
complex potential 복소 퍼텐셜                   Coulomb's theorem 쿨롱의 정리
component of vector 벡터의 성분                 Coulomb's tors幻n balance 쿨롱의 비틀림저울
component vector 성분벡터                      coulomb [=C] 쿨롱［단위］
composition of vector 벡터의 합성               Cou幻mb barrier 쿨롱 가로막이
comi兀und pendulum 겹흔들이                     Coulomb barrier 쿨롱 장벽
computer simulated experiment              Coulomb energy 쿨롱 에너지
    셈틀 시늉내기실험                              Coulomb excitation 쿨롱 들뜸
computer simulated experiment              Coulomb factor 쿨롱 인자
    컴퓨터 시늉실험                               Coulomb force 쿨롱힘
computer simulational molecular dynamics   Coulomb 幻rce law 쿨롱힘 법칙
    컴퓨터 시늉 분자동역학                           Coulomb potential 쿨롱퍼텐셜
condensation point 서림점                     Coulomb scattering 쿨롱 산란
conduction 이ectron 전도전자                    Coulomb scattering 쿨롱 흩뜨림
                                           부록 B . 한국물리학회 공식 물리학 용어집 313



coupled oscillation 결합된 진동              derived unit 파생단위
covariant differntiation 공변미분           deviation 벗어나기
covariant d浚erntiation 껴바뀜 미분           deviation 편차
covariant vector 공변 벡터                  deviation angle 벗어나기 각
covariant vector 껴바뀜 벡티                 dew p아nt 이슬점
coverage 덮임율                            dew-point hygrometer 이슬점누기재개
critical end point 고비끝점                 dew-point hygrometer 이슬점습도계
critical end point 임계끝점                 dew-point temperature 이슬점 온도
critical point 고비점                      diaphragm 진동판
critical point 임계점                      difference 계차
crossover 교차                            小fference 뺌
cross-over 교차                           difference 차
crossover 교차이동                          difference 차분
crossover exponent 교차지수                 difference -differential equation
crossover scaling 교차 눈금잡기                   계차미분방정식
crossover scaling 교차축척                  d沮erence-d沮erential equation
crystal momentum 결정운동량                      뺌미분방정식
cubic un迂 cell 입방단위세포                   小fference equation 계차방정식
Curie p이nt 퀴리점                          difference equation 차분방정식
Curie unit 퀴리단위                         d消erence tone 뺌소리
cutoff potential 끊어버림 퍼텐셜               d沮erence tone 차음
cycloidal pendulum 사이클로이드 흔들이           differential 미분
cyclotron frequency 사이클로트론 진동수          小fferential calculus 미분법
cylindrical capacitor 원기둥형 전기들이         differential calculus 미분법학
damped oscillation 감쇠진동                 differential coefficient 미분곁수
Debye un托 데바이단위                         differential cross section 미분자름넓이
decimal point 소수점                       differential 이ectrometer 차동전위계
decrease of melting point 녹는점 내림        小fferential equation 미분방정식
deep well potential 깊은 우물퍼텐셜            differential galvanometer 차동검류계
definite integral 정적분                   differential gear 차동기어
delay-differential equation 늦어짐 미분방정식   d河erential geometry 미분기하학
delta function 델타함수                     differential n祀thod 차등법
delta singularity 델타 특이성                d沮erential operator 미분연산자
derived unit 유도단위                       differential pulley 차동도르래
derived unit 이끎단위                       小fferential screw 차동나사
314 부록



differential spectrometry 시차분광법           effective differential cross section
diffuse reflection 퍼진 되비침                     유효 미분자름넓이
diffuse reflection 퍼진 반사                  effective 이ectron mass 유효 전자질량
diffusion potential 퍼짐퍼텐셜                 effective magnetic moment 유효 자기모멘트
digital 디지탈                               effective potential 유효퍼텐셜
digital 수치형                               eigenvector 고유벡터
dip이e 쌍극자                                 elastic oscillation 탄성진동
dip이e broadening 쌍극 넓히기                   이ec汀ic dipole 전기쌍극
dip아e小d巾이e interaction 쌍극자 상호작용           이ectric dipole 전기쌍극자
d巾이e-d巾이e interaction 쌍극자 서로작용            이ec甘ic d巾아e moment 전기 쌍극자모멘트
dip이e field 쌍극자마당                         이ectric field barrier 전기마당가로막이
dip이e 엎ass 쌍극자유리                          electric field intens蜘 전기마당의 세기
dip이e interaction 쌍극자 상호작용                이ec甘ic field strength 전기마당의 세기
dip아e interaction 쌍극자 서로작용                이ec甘ic field vector 전기마당벡터
dipole moment 쌍극자모멘트                      이ec汀ic insulator 전기절연체
dip이e movement 쌍극자 운동                     이ectric moment 전기모멘트
dip이e orientation 쌍극자 배향                  electric monopole 전기홀극
小pole potential 쌍극자퍼텐셜                    이ectric multip아e 전기다중극
dipole radiation 쌍극자내비침                   이ec甘ic mu出p이e 전기다중극자
dip아e radiation 쌍극자 복사                    이ec甘ic multip아e moment 전기다중극모멘트
dipole strength 쌍극자 세기                    이ec甘ic mu出p이e moment 전기다중극자모멘트
dip아e-sum rule 쌍극자합법칙                     이ec甘ic mu川p아e radiation 전기다중극 내비침
dip아e transition 쌍극자 전이                   이ec甘ic mu川p아e radiation 전기다중극 복사
Dirac's 이ectron theory 디락의 전자이론           이ectric musical instrument 전기악기
direct integral 직접적분                      electric octup이e 전기팔중극자
direction vector 방향벡터                     이ectric pendulum 전기흔들이
dispersive power 분산능력                     이ec甘ic permittivity 유전율
displacen祀nt vector 변위벡터［전기］              electric potential 전기퍼텐셜
disp怡cement vector 옮김벡터                   이ec甘ic potential 전위
double pendulum 겹흔들이                      electric potential difference 전위차
doublet 겹샘                                이ectric power 전력
drift motion 표류운동                         이ectric power line 전력선
dynamics of material point 질점동역학          electric power transmission 전력수송
effective centrifugal potential 유효원심퍼텐셜   electric quadrup이e 전기사중극
                                                 부록 B . 한국물리학회 공식 물리학 용어집 315



 이ec甘ic quadrup이e 전기사중극자                     이ec甘on ionization 전자이온화
 이ectroche而cal potential 전기화학퍼텐셜             electron microscope 전자현미경
 이ec甘ode potential 전극전위                      이ectron mob小ty 전자이동도
 elec甘이ytic capacitor 전해질축전기                 이ec甘on mult巾her 전자증배관
 이ec汀帥agnetic mo毗ntum 전자기운동량                 이ectron neutrino 전자중성미자
 이ectromagnetic oscillation 전자기진동            이ectron optics 전자광학
 이ec比帥agnetic potential 전자기퍼텐셜               이ectron orbit 전자자리길
 이ectromagnetic system of unit 전자기단위계        이ectron pair 전자짝
 이ectromagnetic un仕 [=emu] 전자기단위             이ectron pair annihilation 전자짝 소멸
이ectron 전자                                   이ectron pair bond 전자짝 결합
이ectron affinity 전자친화성                      이ectron pair creation 전자짝 생성
 elec甘on affin蜘 전자친화성도                      이ectron寸pair production 전자짝 생김
 elec甘이I capture 전자잡힘                       이ectron-pair production 전자짝 생성
electron capture 전자포획                       이ec甘on 히asma wave 전자 플라스마 파동
이ec甘on cloud 전자구름                            electron-positron pair formation
이ectron collision 전자충돌                           전자卞양전자 짝형성
이ectron diffraction 전자에돌이                   이ectron ray 전자선
이ectronegativity 전기옴성도                      이ec甘이i scattering 전자 홑뜨림
electron -elec汀on co小sion 전자e전자 부딪침         이ectron screening 전자 가리기
이ectron-이ec甘on co小針이1 전자小전자 충돌              이ec甘이i spin 전자스핀
electron gun 枷｝총                            elec甘on spin moment 전자스핀모멘트
이ec甘on h이e 전자4구멍                            이ec甘on spin relaxation 전자스핀완화
이ec甘on卞h이e pair 전자卞구멍 짝                     이ectron spin relaxation 전자스핀풀림
electron-hole recombination                 elec甘on spin resonance 전자스핀공명
    전자H구멍 재결합                               이ectron spin resonance 전자스핀껴울림
electronic clock 전자시계                       electron synchrotron 전자싱크로트론
이ectronic computer 전자계산기                    electron temperature 전자온도
이ectronic configuration 전자짜임새               elec甘on theory of metals 금속 전자이론
electronic data processing system [=EDPSJ   electron tube 전자관
    전산자료처리장치                                electron wave 전자파동
이ectronic energy 전자에너지                      electroreflectance 전기반사율
이ec汀onics 전자공학                              이ectrostatic field 정전기마당
이ectronic spec沮c heat 전자견줌열                 이ectrostatic potential 정전기퍼텐셜
이ectronic state 전자상태                        이ectrostatics 정전기학
이ectron impact 전자충격                         이ectros'tatic unit {=esu] 정전기단위
316 부록



이ectrostatic Un迂 system 정전기단위계       equipotential surface 등전위면
이ementary particle physics 소립자물리학    equipotential surface 등퍼텐셜면
e川PS아d of inertia 관성타원체              equivalent 이ec作on 같은값 전자
elliptically p아arized light 긴원극나뉨빛   equiv키ent 이ectron 등가전자
elliptically polarized light 타원편광    equivalent 이ectron 맞먹이 전자
elliptic coordinate 긴원자리표            equivalent simple pendulum
elliptic coordinate 타원좌표                 같은값 단순흔들이
에巾tic double refraction 긴원겹꺽임        equivalent 帥iiple pendulum 등가 단순흔들이
e小ptic double refraction 타원복굴절       equivalent simple pendulum
elliptic function 긴원함수                   맞먹이 단순흔들이
e小ptic function 타원함수                 error bar 오차 막대
e小ptic integral 긴원적분                 Euler's equation of motion
elliptic integral 타원적분                   오일러의 운동방정식
에巾tic motion 긴원운동                    eutectic point 공융점
elliptic motion 타원운동                 eutectic point 함께 녹음점
e小ptic orbit 긴원자리길                   exact differential 완전미분
elliptic orbit 타원궤도                  exact d沮erential equation 완전미분방정식
elliptic oscillation 긴원떨기            excess 이ec甘on 과잉전자
elliptic oscillation 타원진동            exchange frequency 교환진동수
elliptic polarization 긴원극나뉨          exchange integral 바꿈적분
elliptic polarization 타원편극           excitation potential 들뜸퍼텐셜
emissive power 방출능                   excitonic insulator 엑시톤 절연체
end p아nt 끝점                          experimental physics 실험물리학
end point energy 끝점에너지               external reflection 바깥되비침
energy integral 에너지 적분               external reflection 외부반사
energy-momentum tensor               extraction 추출
     에너지1운동량 텐서                      extraneous root 무연근
energy source 에너지샘                   extraordinary ray 이상광선
 equation of motion 운동방정식            extraordinary ray 이상 빛살
 equation of vibration 떨기방정식         extraordinary wave 예외파동
 equilibrium point 비김점               extraordinary wave 특수파동
 equilibrium point 평형점                extrap이ated method 바깥늘림법
 equipotential line 등전위선              extrapolated range 바깥늘림 범위
 equipotential line 둥퍼텐셜선             extrem이y high frequency 초 고진동수
                                              부록 B. 한국물리학회 공식 물리학 용어집 317



farad 패럿［전기용량의 단위］                         focusing anode 모음양극
Faraday뇨 Ia＼자 of elec甘이ys始                 forced 미bration 강제떨기
    패러데이의 전기분해 법칙                          幻rce of inert治 관성력
Faraday's law of electromagnetic inducti   force of inertia 관성힘
    패러데이의 전자기유도법칙                          Foucault's pendulum 푸코의 흔들이
Faraday's law of electromagnetic inducti   Fourier analysis 푸리에 해석
    패러데이의 전자기 이끎법칙                         Fourier-Bessel expansion 푸리에小베셀 전개
Faraday constant 패러데이 상수                   Fourier expansion 푸리에 전개
Faraday dark space 패러데이 암흑부                Fourier integral 푸리에 적분
Faraday dark space 패러데이 어둠부분               Fourier integral theorem 푸리에 적분정리
Faraday effect 패러데이 효과                     Fourier series 푸리에 급수
Faraday rotation 패러데이 돌기                   Fourier space 푸리에 공간
Faraday rotation 패러데이 회전                   Fourier transform 푸리에 변환
far from equ小brium 평형에서 먼                  four potential 사차원 퍼텐셜
far infrared 먼 넘빨강                         four vector 사차원 벡터
far infrared 원 적외선                         Frank-Read source 프랑크m리드 샘
far point 먼 점                              free 이ec甘on 자유전자
far point 원점                               free 이ectron model 자유전자모형
far 針ghtness 멀리보기                          free 미bration 자유떨기
far sightness 원시                           freezing point 어는점
Fermi momentum 페르미 운동량                     freezing point 응결점
Fermi wave vector 페르미 파수벡터                 freezing point depression 어는점 내림
field momentum 마당운동량                       frequency 진동수
field of vector 벡터 마당                      frequency band 진동수띠
finite-difference method 유한차 방법            frequency condition 진동수조건
fixed c카）acitor 고정축전기                      frequency doubling 진동수배가
fixed capacitor 붙박이전기들이                    frequency gap 진동수간격
fixed point 고정점                            frequency meter 진동수계
 fixed point 붙박이점                          frequency modulated cyclotron
 fixed point of temperature 온도의 고정점            진동수변조 사이클로트론
 fixed point of temperature 온도의 붙박이점       frequency modulation 진동수변조
加ating point 떠돔점                           frequency sh沮 진동수이동
加ating point 이동소숫점                         frequency sweep 진동수쓸기
 focal point 모암점                           Friedel oscillation 프리델 진동
 focal point 초점                            frost point 서리점
318 부록



fundamental unit 기본단위                    grid potential 그리드 퍼텐셜
fundamental vector 기본벡터                  gyrosc야光 자이로스코프
fundamental vibration 기본떨기               Hamilton's canonical equation
Galilei's inertial law 갈릴레이의 관성법칙             해밀턴의 바른틀방정식
gap voltage 간격전압                         Hamilton's canonical equation
gap voltage 틈전압                              해밀턴의 정준방정식
gauss 가우스［단위］                            H跏ilton's function 해밀턴의 함수
Gauss distribution law 가우스 분포법칙          Hamilton's principle 해밀턴의 원리
Gauss divergence theorem 가우스 발산정리        Hamiltonian 해밀토니안
Gauss error function 가우스 오차함수            Hamiltonian operator 해밀토니안 연산자
Gauss eye-piece 가우스 눈쪽렌즈                 harmonic motion 어울림운동
Gaussian distribution 가우스 분포             harmonic motion 조화운동
Gaussian model 가우스 모형                    harmonic oscillator potential
Gaussian process 가우스 과정                      어울림떨개퍼텐셜
Gaussian unit 가우스 단위                     harmonic oscillator potential 조화떨개퍼텐셜
Gaussian well 가우스 우물                     harmonic overtone 어울림배음
Gauss lens formula 가우스 렌즈 공식             harmonic overtone 조화배음
Gauss theorem 가우스 정리                     health physics 보건물리학
generalized momentum 일반화 운동량             heat effect of 이ec甘on current 전류의 열효과
generation of hydroelectric power 수력발전   heat insulator 열절연처］
geocentric motion 지구중심운동                 heat source 열샘
geocentric rectangular coordinates       heliocentric motion 태양중심운동
    지구중심 직교자리표                           hertz [=H기 헤르츠［진동수의 단위］
geocentric rectangular coordinates       heteroclinic point 다른 모임점
    지구중심 직교좌표                            high energy 이ectron 고에너지 전자
geometrical 이ec甘on optics 기하전자광학         high-frequency 고진동수
geophysics 지구물리학                         high-frequency ampl派er 고진동수 증폭기
giant dipole resonance 거대쌍극자공명           high-frequency circuit 고진동수 회로
曾ant 小p아e resonance 큰쌍극자껴울림              high-丘equency circuit 높은 진동수 흐름길
gram molecular weight 그램분자량              high-frequency furnace 고진동수 도가니
gravitational acceleration 중력가속도         high-frequency heating 고진동수 가열
gravitational potential 중력퍼텐셜            high-frequency insulator 고진동수 절연물
gravitational un仕 of force 힘의 중력단위       high -frequency wave 고진동수 파동
gravitational-unit system 중력단위계          high resolving power 고분해능
grid bias voltage 그리드 바이어스 전압            hon均clinic p이nt 같은 모임점
                                       부록 B; 한국물리학회 공식 물리학 용어집 319



homologous point 대응점                inertial force 관성력
horizontal pendulum 수평 흔들이          inertial force 관성힘
horsepower 마력                       inertial mass 관성질량
horsepower hour 마력시                 inertial resistance 관성저항
h야 이ectron 뜨거운 전자                   inertial system 관성계
h야 이ectron 열전자                      inertial wave 관성파동
Hubbard model 허바드 모형                inertia tensor 관성텐서
hybrid frequency 복합진동수              inexact differential 불완전미분
hydroelectric power station 수력발전소   inflection point 변곡점
hyperuniversality 초보편성              infrared lattice 미bration 넘빨강 살창떨기
ice point 얼음점                       infrared lattice 미bration 적외선 살창떨기
ideal insulator 이상절연체               infrared reflectivity 넘빨강 되비춤율
ignition point 발화점                  infrared reflectivity 적외선반사도
ignition p이nt 불붙음점                  nitial point 시초점
image point 상점                      initial point 처음점
image point 영상점                     inner point 내부점
imaginary point 허점                  inner p아nt 안쪽 점
imaginary un仕 허수단위                  inscribe 내접
impedance bridge 온저항 브리지            inscribe 내접하다
impedance bridge 임피던스 브리지           instantaneous acceleration 순간가속도
impedance vector 온저항 벡터             ins甘ument 계기
impedance vector 임피던스 벡터            instrument 기구
impedance voltage 온저항 전압            instrument 도구
impedance v이tage 임피던스 전압            instrument 장치
impressed voltage 인가전압              instrument 재개
improper integral 특이적분              instrumental error 계기오차
incident point 입사점                  instrumental error 기구오차
indefinite integral 부정적분            instrument gauge 재개
index of a critical point 고비점의 지표   insulator 부도체
induced dip아e 유도 쌍극자                insulator 절연체
induced d巾이e 이끌린 쌍극자                integral 적분
inductance bridge 인덕턴스 브리지          integral calculus 적분법
inert治 관성                           integral calculus 적분학
inertia ellipsoid 관성타원체             integral constant 적분상수
inertial balance 관성저울               integral denominator 적분분모
320 부록



integral divisor 옹근나눔수                 internal conical refraction 속원뿔꺽임
integral equation 적분방정식                internal conversion 이ec甘on 내부전환전자
integral factor 적분인자                   internal convers幻n 이ectron 속전환전자
integral network 적분그물                  internal linear momentum 내부선운동량
integral network 적분그물얼개                internal linear momentum 속선운동량
integral path 적분경로                     internal motion 내부운동
integral path 적분길                      internal motion 속운동
integral path 적분행로                     internal p아ential 내부퍼텐셜
integral variable 적분변수                 internal potential 속퍼텐셜
intermediate frequency [=1F] 중간진동수     internal reflection 내부반사
intermediate frequency amplifier       internal reflection 속되비침
    중간진동수 증폭기                          interpolation 내삽법
intermediate frequency trans的rmer      interpolation 사이채움
    중간진동수 변압기                          interpolation 속채우기
interm아ecular 분자간                      interpolation method 내삽법
interm이ecular 분자사이                     interpolation meth叱 보간법
interm이ecular 幻rce 분자간 힘               interpolation method 속채우기법
m t町m아ecular force 분자사이 힘              intrinsic angular momentum 고유각운동량
intermolecular interaction 분자간 상호작용    intrinsic angular mon祀ntum 배내각운동량
intermolecular interaction 분자사이 서로작용   intrinsic magnetic moment 고유자기모멘트
m t町m아ecular potential 분자간퍼텐셜          intrinsic magnetic moment 배내자기모멘트
interm이ecular potential 분자사이 퍼텐셜       ion bombardment 이온 두둘김
intermolecular reaction 분자간 반응         ion bombardment 이온 충격
intermolecular reaction 분자사이 반응        ion-dipole bond 이온 쌍극자 결합
intermolecular rearrangement           ionization extrapolated range
     분자간 자리옮김                               이온화바깥늘림범위
intermolecular rearrangement           向nization p아ential 이온화퍼텐셜
     분자간 자리옮김반응                        ionization power 이온화능력
intermolecular rearrangement           幻nization voltage 이온화전압
     분자사이 자리옮김                         向n source 이온샘
intermolecular rearrangement            irrational system of units 무리수꼴 단위계
     분자사이 자리옮김반응                        irrational unit system 무리수꼴 단위계
 internal angular momentum 내부각운동량       irregular reflection 난반사
 internal angular momentum 속각운동량        irregular reflection 막 되비침
 internal conical refraction 내부원뿔굴절     isobar 동중원소
                                        부록 B. 한국물리학회 공식 물리학 용어집 321



isobar 동중원자핵                         Lagrange's method of undetermined mu川p
isobar 동중핵                               라그랑지의 미정계수법
isobar 등압선                           Lagrange's method of undetermined multip
isobar 일정압력선                             라그랑지의 미정곱수법
isobaric change 동중원자핵변화              Lagrange multiplier 라그랑지 곱수
isobaric change 동중핵변화                lambda point 람다 점
isobaric change 등압변화                 Larmor frequency 라모 진동수
isobaric change 일정압력변화               lateral motion 가로운동
isobaric expansion 등압팽창              lattice column 살창기둥
isobaric expansion 일정압력불음            lattice p이nt 살창마디
isobaric 마ocess 동중핵과정                lattice point 살창점
isobaric process 등압과정                lattice reflection 살창되비침
isobaric process 일정압력과정              lattice reflection 살창반사
isobaric surface 등압면                 lattice 미bration 살창떨기
isobaric surface 일정압력면               law of conservation of momentum
isobaric transformation 동중핵 사이의 변환       운동량보존법칙
is이ated p아nt 고립점                     law of inert治 관성의 법칙
isolated p이nt 외떨어진 점                 law of momentum conservation
isovector 돌벡터                            운동량보존법칙
isovector 아이소벡터                      law of motion 운동 법칙
iterated integral 반복적분               law of motion 운동의 법칙
junct幻n potential 접점전위               law of reflection 되비침 법칙
卜inction potential 접점퍼텐셜             law of reflection 반사의 법칙
Kater's pendulum 케이터의 흔들이            law of universal gravitation 만유인력의 법칙
Kater's reversible pendulum          leakage factor 샘인자
    케이터의 되짚기흔들이                      Lennard-Jones potential 르나드U존스퍼텐샬
Kepler's law 케플러의 법칙                 light-gathering power 집광력
Ke히er's law of areas 케플러의 넓이법칙       light point 광점
Kepler's law of planetary motion     light point 빛점
    케플러의 떠돌이별 운동법칙                   light soL甘ce 빛샘
Kepler's telescope 케플러의 망원경          light source for illumination 비침용 빛샘
ket vector 켓벡터                       limiting point 극한점
Kohlrausch bridge 콜라우시 다리            linear acc이erat幻n 선가속도
Kronecker delta 크로네커 델타              linear difference equation 선형계차방정식
Lagrange's equation 라그랑지의 방정식        linear differential equation 선형미분방정식
 322 부록



 linear n珣mentum 선운동량                     magnetic dipole radiation 자기쌍극자 내비침
 linear ordinary differential equation    magnetic flux 자기선속
      선형상미분방정식                            magnetic flux density 자기선속밀도
 linear partial differential equation     magnetic moment 자기모멘트
      선형편미분방정식                            magnetic monop이e 자기홀극
 linear vector space 선형벡터공간               magnetic north pole [=N] 자기북극
 line integral 선적분                        magnetic p이e 자기극
 line of force 역선                         magnetic potential 자기퍼텐셜
 line of tni히e points 삼중점의 선              magnetic quadrup이e 자기사중극
 line of triple points 세겹점의 선            magnetic quadrup이e 자기사중극자
 line source 선샘                          magnetic southern p이e 자기남극
 liquid column thermometer 액체기둥온도계       magneto plasma frequency
Lissajous figure 리사주 그림                       자기플라스마 진동수
localized moment 국소모멘트                   magnetos怡tic potential 정자기퍼텐셜
localized moment 한곳 모멘트                  magnifying power 배율
locked-phase source 위상고정 샘               magni如ing power 확대능
longitudinal 미bration 세로 떨기              mass point pendulum 질점흔들이
low energy electron diffraction          mass unit 질량단위
     낮은 에너지 전자 에돌이                       material point 질점
low energy electron diffraction          mathematical physics 수리물리학
     저에너지 전자에돌이                          matrix mechanics 행렬역학
low frequency 낮은 진동수                     mean deviation 평균편차
low power i川e 저출력 원자로                    mean spherical approximation 평균 공어림법
low v이tage 낮은 전압                         mechanics 역학
low voltage 저전압                          mechanics of a system of material points
magnetic dip이e 자기쌍극                           질점계역학
magnetic dip이e 자기쌍극자                     mechanics of particle 질점역학
magnetic dip이e interaction 자기쌍극 상호작용     mechanics of rigid body 강체역학
magnetic dip이e interaction 자기쌍극 서로작용     melting point 그l二그二二처
                                                       中 14 1그

magnetic dipole interaction              melting point 융해점
    자기쌍극자 상호작용                           m이ting point depression 녹는점 내림
magnetic dipole interaction              mercury barometer 수은기압계
    자기쌍극자 서로작용                           mercury column 수은기둥
magnetic dip이e moment 자기쌍극자모멘트           mercury column 수은주
magnetic dip아e radiation 자기쌍극 내비침        metastable 준안정
                                                부록 B . 한국물리학회 공식 물리학 용어집 323



 metastable level 준안정준위                      molecular heat at constant volume
 metastable phase 준안정상                           정적분자열
 metastable state 준안정상태                      m이ecular kinetic energy 분자운동에너지
 micro-Brownian motion 미소m브라운 운동             molecular kinetic theory 분자운동론
 migration p야ential 이동전위                     molecular mass 분자질량
 minimum deviation 최소편향                      m이ecular model of a gas 기체의 분자모형
 mirror reflection 거울되비침                     m이ecular motion 분자운동
 mirror reflection 거울반사                     m이ecular orbital 분자궤도상태
 MKS system of unit [=meter-kilogram-seco   molecular orbital 분자궤도함수
     엠케이에스 단위계                              molecular reorientation 분자 되방향잡기
 mode of 미bration 떨기의 방식                    molecular spec汀oscopy 분자분광학
modern physics 현대물리학                        m이ecular 미scosity 분자속쓸림
m이ecular beam 분자살                           m이ecular wei帥t 분자량
molecular-beam experiment 분자살 실험            moment 모멘트
molecular binding 분자결합                      moment of force 힘능률
m이ecular bin如g 분자묶음                         moment of force 힘의 모멘트
m이ecular chaos 분자혼돈                         moment of inertia 관성모멘트
molecular clock 분자시계                        momentum 운동량
molecular crystal 분자결정                      momentum balance 운동량 균형
m이ecular current 분자전류                       momentum balance 운동량 차이
m이ecular dynamics 분자동역학                     momentum conservation law 운동량보존법칙
molecular dynamics ensemble                 momentum density 운동량 밀도
    분자동역학 모듬                                momentum operator 운동량 연산자
molecular dynamics ensemble                 momentum operator 운동량 작용소
    분자동역학 앙상블                               momentum representation 운동량 나툼
m이ecular excitation 분자들뜸                    momentum representation 운동량 표시
m이ecular field 분자마당                         momentum representation 운동량 표현
m이ecular force 분자력                          momentum transfer 운동량 전달
molecular force 분자힘                         monochromatic light source 한색빛샘
molecular heat at constant pressure         monomolecular layer 단분자층
    일정압력분자열                                 monom이ecular layer 한분자켜
molecular heat at constant pressure         monopole 홀극
    정압분자열                                   Monte Carlo simul謫on 몬테칼로 시늉내기
molecular heat at constant volume           motion 운동
    일정부피분자열                                 motional narrowing 운동 좁아지기
324 부록



motion of falling body 낙체운동                near point 근점
motion of falling body 낙하운동                negative deviation 음의 편차
motion of pr이ectile 포물선운동                  negative 이ectron 음전자
motion of pr이ectile 포물체운동                  neoclassical diffus由n 새고전 퍼짐
motion of straight line 직선운동               neu甘on physics 중성자물리학
movable point 동점                           neutron source 중성자샘
movable point 움직점                          Newton's first law 뉴턴의 제일법칙
moving point 움직점                           Newton's first law 뉴턴의 첫째법칙
moving p이nt 이동점                            Newton's law of cooling 뉴턴의 냉각법칙
multichannel differential pulse height s   Newton's law of motion 뉴턴의 운동법칙
    뭇겹 펄스높이 선택기                            Ne＼砒on's ring 뉴턴의 원
multichannel differential pulse height s   Ne＼毗on's ring 뉴턴의 원무늬
    여러 펄스높이 고르개                            Ne＼砒on's second la＼人／뉴턴의 둘째법칙
multiple integral 뭇겹적분                     Newton's second law 뉴턴의 제이법칙
multiple integral 여러겹 적분                   Ne＼砒on's third law 뉴턴의 세째법칙
multiple reflection 뭇겹반사                   Newton's third law 뉴턴의 제삼법칙
multiple reflection 여러겹 되비침                newton 뉴턴［단위］
multiplication table 곱셈표                   newtonian mechanics 뉴턴역학
multiply periodic motion 뭇겹주기운동            Ne＼砒이ian telescope 뉴턴 망원경
multi히y periodic motion 여러 주기 운동           Newtonian viscos卄y 뉴튼 속쓸림
multip이e 뭇겹극                               nodal point 마디점
multip이e 여러겹극                              node 교점
multip이e expansion 뭇겹극 전개                  node 마디
mul如이e expansion 여러겹극 전개                   node 절
multip이e ma比汶 element 뭇겹극 행렬요소             non니ocal potential 한곳아닌 퍼텐셜
mu川p이e ma甘汶 이e毗nt 여러겹극 행렬요소                non-Newtonian 미scos蜘 비뉴튼 속쓸림도
multip이e moment 뭇겹극 모멘트                    nonrationalized unit system 비유리화 단위계
multipole moment 여러겹극 모멘트                  nonuniform velocity motion 안고른속도운동
multipole radiation 뭇겹극복사                  normal acceleration 법선가속도
multip이e radiation 여러겹극 내비침                normalization integral 틀맞춤적분
natural frequency 자연진동수                    normal mode of 너bration 떨기의 기준방식
natural time unit 자연시간단위                   normal North pole 기준 북극
nearly free electron model                 normal 미bration 기준떨기
    거의 자유로운 전자모형                           north pole 북극
near p이nt 가까운점                             north p이e 엔극
                                         부록 B. 한국물리학회 공식 물리학 용어집 325



Nose-Hoover oscillation 노제1후버 떨기      optical reflectivity 빛 되비침도
nuclear magnetic moment 핵자기모멘트        optical rotatory power 빛회오리성
nuclear moment 핵 모멘트                  optical rotatory power 선광성
nuclear physics 핵물리학                  opto-electronic integrated circuit [=0E11
nuclear power 원자력                         광전집적회로
nuclear power 핵에너지                    optoelectronics 광전자공학
nuclear power 히ant 원자력발전소             orbital angular momentum 궤도각운동량
nuclear power 히ant 핵발전소               orbital angular momentum 자리길각운동량
nuclear power station 원자력발전소          orbital 이ec甘on 궤도전자
nuclear power station 핵발전소            orbital 이ec甘on 자리길전자
nuclear quadrupole moment             orbital 이ec甘on capture 궤도전자 포획
    핵 사중극자모멘트                         orbital 이ectron capture 자리길전자 잡힘
nuclear quadrupole resonance          overall rotation 전체회전
    핵 사중극자껴울림                         overall yield 전체거둠율
nuclear vibration 핵떨기                 overcharge 과충전
numerical aperture 조리개수               overhang 튀어나옴
numerical method 수치계산법                Overhauser effect 오버하우저 효과
numerical weather prediction 수치예보     overlap 겹치기
n-vector model 엔벡터모형                  overlap integral 겹치기적분
oceanophysics 해양물리학                   overpotential 과전위
octup이e 팔중극                           overtone 배떨기
octup이e 팔중극자                          overtone 배음
octup이e moment 팔중극 모멘트                overvoltage 과전압
octupole moment 팔중극자 모멘트              oxidation potential 산화전위
octupole radiation 팔중극 내비침            oxidizing power 산화력
octupole radiation 팔중극 복사             paper capacitor 종이 축전기
omega point 마지막 점                     parallel plate capacitor 평행판 축전기
one-electron bond 단일전자 결합             partial reflection 부분되비침
one-pion exchange potential [=OPEP]   partial reflection 부분반사
    단일파이온 바꿈퍼텐셜                       particle mechanics 질점역학
optical instrument 광학기기               particle physics 입자물리학
optical path d浪erence 광행로차            path d沮erence 길거리차
optical point 광점                      path difference 행로차
optical potential 광학퍼텐셜               peak potential 봉우리 전위
optical reflectivity 광 반사도            pendulum 흔들이
326 부록



penetrating power 투과능               1기anck's quantum theory 플랑크의 양자이론
periodic motion 주기운동                Planck's radiation formula
per幻dic table 주기율표                      플랑크의 내비침 공식
permanent dip이e 영구쌍극자               Planck's radiation formula
permittivity 유전율                        플랑크의 복사공식
permittivity constant 유전율상수         I기anck constant 플랑크상수
perpetual motion 영구운동               Planck distribution function 플랑크 분포함수
phase difference 위상차                하ane of reflection 되비침면
phase integral 위상적분                 1丑ane of reflection 반사면
phase vector 위상벡터                   1丑anetary motion 떠돌이별 운동
phonon momentum 소리알 운동량             히anetary motion 행성운동
帥onon momentum 포논 운동량               이asma frequency 플라스마 진동수
photo이ectric thresh이d 광전문턱          이asma oscillation 플라스마 진동
photo이ectric thresh이d 빛전자문턱         point 점
하ioto이吼比on 광전자                      p이nt charge 점전하
ph아oelectron 빛전자                    point contact transistor 점접촉 트랜지스터
physical atomic weight 물리적원자량       point defect 점결함
physical change 물리적 변화              point discharge 끝점방전
physical chem活甘y 물리화학               p이nter 가리키개
physical constant 물리상수              pointer 바늘
physical mass unit 물리질량단위           p이nt groups 결정군
physical metall出gy 물리야금학            point groups 점군
physical model 물리적 모형               point group symbol 점군기호
physical oceanography 해양물리학         p아nt image 점상
physical property 물리적 성질            point니on model 점이온 모형
physical quantity 물리량               p이nt light source 점광원
physical science 물상과학               point light source 점빛샘
physical un仕 물리단위                   pointlike particle 점같은 알갱이
physical universe 물리적 우주            pointlike particle 점같은 입자
physical variable star 물리적 변광성      p아ntlike target 점같은 과녁
physics 물리학                         point magnetic p이e 점자기극
physics of crystals 결정 물리학          p이nt mass pendulum 질점흔들이
picofarad 피코패럿                      point of application 작용점［힘의］
1기anck's action quantum 플랑크의 작용양자   p이nt source 점샘
I기anck's constant 플랑크의 상수           point source 점원
                                    부록 B . 한국물리학회 공식 물리학 용어집 327



 p이arization vector 쏠림벡터        power reactor 동력핵반응로
 polarization vector 편광벡터       power series 멱급수
 p이ar vector 극성벡터               power series 지수급수
 p이e 극                          power source 전력샘
 p이e 히ate 극판                    power source 전원
 position vector 위치벡터           Poynting vector 포인팅 벡터
 position vector 자리벡터           practical unit 실용단위
 positive column 양극 기둥          precession 옆돌기
 positive c이umn 양극 빛기둥         precessional motion 옆돌기운동
 potential 퍼텐셜                 precolumn 앞엣기둥
p아ential barrier 퍼텐셜 가로막이      prewetting critical point 미리젖음고비점
p아ential barrier 퍼텐셜 장벽        primary 이ectron 일차전자
potential difference 전위차       primary voltage 일차전압
potential difference 퍼텐셜 차이    principal axis of inertia 관성주축
potential drop 전위떨어짐           principal lattice vector 기본살창벡터
potential drop 퍼텐셜 떨어짐         principal moment of inertia 주관성모멘트
potential energy 위치에너지         principal point 주점
potential energy 퍼텐셜에너지        product of inertia 관성의 곱
potential flow 퍼텐셜 흐름          pr이ectile motion 팔매선운동
potential gradient 전위 물매       pr이ectile motion 팔매선운동포물체운동
potential gradient 퍼텐셜 물매      pr아ectile motion 포물선운동
potential hill 퍼텐셜 언덕          propagation vector 전파벡터
potential scattering 퍼텐셜 산란    propagation vector 퍼져나감벡터
potential scattering 퍼텐셜 흩뜨림   proper oscillation 고유진동
potential step 퍼텐셜 계단          proper vibration 고유떨기
potential well 퍼텐셜 우물          可oper 미bration 참떨기
power 능력                       proton-electron hypothesis of the nucleu
P0＼入／er 동력                         원자핵의 양성자H전자가설
power 일률                       pseudopotential 유사퍼텐셜
power 전력                       pseudovector 유사벡터
power dissipation 전력흗어지기       psychophysics 마음 물리학
power寸factor 전력인자              pure physics 순수물리학
power generator 발전기            quadrille de미at幻n 사분편차
power line 동력선                 quadrupole 사중극
power of lens 렌즈의 능력           quadrup이e 사중극자
328 부록



quadrupole cou1小ng constant 사중극 결합상수   reducing power 환원력
quadrup이e interaction 사중극 서로작용         reduction p아ential 환원 퍼텐셜
quadrup이e lens 사중극렌즈                   reflectance 되비침율
quadrup이e matr汶 이ement 사중극 행렬요소        reflectance 반사율
quadrupole moment 사중극자모멘트              reflected light 되비침빛
quadrup아e radiation 사중극내비침             reflected light 반사광
quadrup이e radiation 사중극복사              reflected pulse 반사펄스
quadrup이e relaxation 사중극 완화            reflected ray 되비침빛살
quadrup이e relaxation 사중극풂              reflected ray 되비침살
quantum 이ec甘onics 양자전자공학               reflected ray 반사광선
quantum mechanics 양자역학                 reflected ray 반사선
quantum physics 양자물리학                  reflected wave 되비침파동
quantum statistical mechanics 양자통계역학   reflected wave 반사파동
quasiperiodic motion 준주기운동             reflecting mirror 되비춤거울
radial acceleration 지름가속도              reflecting telescope 되비춤망원경
radiation source 내비침샘                  reflecting telescope 반사망원경
radiation source 방사선샘                  reflection 되비침
radius vector 반지름 벡터                   reflection 반사
ramp voltage 경사전압                      reflection angle 되비침각
ramp voltage generator 경사 전압 발생기       reflection angle 반사각
random motion 마구잡이 운동                  r出ection coefficient 되비침곁수
random motion 막운동                      reflection coefficient 반사곁수
rationalized unit system 유리화된 단위계      reflection grating 되비침 에돌이발
rational unit system 유리화된 단위계          reflection grating 반사 에돌이발
reactor physics 원자로물리학                 reflection of X-ray 엑스선의 되비침
reactor power 원자로 출력                   reflection of 千ray 엑스선의 반사
reciprocal lattice point 역살창점          reflective law 되비침 법칙
reciprocal lattice vector 역살창벡터        reflective law 반사법칙
rec아l 이ec甘on 되튐전자                      reflectivity 되비침율
rectangular coordinates 직각자리표          reflectivity 반사율
rectangular coordinates 직각좌표           reflector 되비추개
rectangular prism 직각프리즘                reflector 반사경
rectangular pulse 장방형파                 refroreflection 뒷되비침
rectangular wave guide 장방형 도파관         refroreflection 후방반사
reduced unit 축약단위                      relative motion 상대운동
                                             부록 B . 한국물리학회 공식 물리학 용어집 329



relative stopping power 상대저지능             saddle point 안장점
relativistic mechanics 상대론적 역학            Sagdeev potential 사그데프 퍼텐셜
relativistic quantum mechanics            saw tooth voltage 톱니 전압
    상대론적 양자역학                             scalar point function 스칼라 점함수
repetive motion 되풀이 운동                    scalar potential 스칼라퍼텐셜
representative point 대표점                  scattered reflection 난반사
repulsive potential 밀기퍼텐셜                 scattered reflection 흗뜨러진 되비침
repulsive potential 반발피텐셜                 scattering power 산란능
resistance type potential divider 저항분압기   scattering power 흩뜨림능력
resistance unit 저항소자                      scattering spherical wave 산란구면파
resolution of vector 벡터의 나눔               scattering spherical wave 흩뜨림구면파동
res이ution of vector 벡터의 분해                scattering vector 산란벡터
resolving power 분리능                       scattering vector 홑뜨림벡터
resolving power 분해능                       Schottky barrier 쇼트키 가로막이
resolving power of microscope             scissoring 미bration 가위질 떨기
    현미경의 분해능                              screened Coulomb potential
resonance frequency 공명진동수                     가려진 쿨롱퍼텐셜
resonance oscillation 공명진동                sealed source 봉한샘
resonance potential 공명퍼텐셜                 seat of 이ectromotive 如rce 기전력샘
resonance potential 껴울림퍼텐셜                secondary 이ectron 이차전자
resultant vector 합벡터                      selective reflection 선택반사
retarded potential 뒤처진 퍼텐셜                separative power 분해능
retarded-vector potential 뒤처진 벡터퍼텐셜       separative power 분해력
retarding potential 뒤처진 퍼텐셜               series capacitor 곧추축전기
retrograde motion 역행운동                    series capacitor 직렬축전기
reverberation 뒤울림                         shared 이ec甘이1 공유전자
reverberation 잔향                          simple harmonic motion 단순조화운동
reversible pendulum 되짚기흔들이                simple harmonic motion 홑어울림운동
ripple voltage 잔결 전압                      simple pendulum 홑흔들이
rolling motion 굴림운동                       simulation 시늉
rotational frequency 회전진동수                simulation 시늉내기
rotational motion 돌기운동                    엷ngle 이ectron tunneling 단일전자터널링
rotational motion 회전운동                    singlet potential 단일항퍼텐셜
row vector 행벡터                            singlet potential 홑겹퍼텐셜
runaway 이ectron 고삐풀린 전자                   singular point 특이점
330 부록



sinusoidal 사인꼴                          specular reflection 거울반사
sinusoidal 사인 모양                        specular reflect幻n 바른 되비침
sinusoidal AC electromotive force       speed governor 속력조절기
    사인꼴 교류기전력                           spherical aberration 구면벗어남
sinusoidal AC electromotive force       spherical angle 구면각
    사인모양 교류기전력                          spherical Bessel function 구면베셀함수
針nusoidal alternating current 사인꼴 교류    spherical condenser 공모양 전기들이
針nusoidal alternating current 사인모양 교류   spherical condenser 구면축전기
skewness 비대칭도                           spherical coordinates 구면자리표
skewness 비틀림                            spherical coordinates 구면좌표
slide wire bridge 미닫이 브리지               spherical curvature 구면곡률

slowing down power 감속능                  spherical curve 구면곡선
引owing down power 감속능력                  spherical Hankel function 구면항켈함수
small oscillation 미소진동                  spherical harmonic function 구면 어울림함수
softening point 무름점                     spherical harmonic function 구면조화함수
softening point 연화점                     spherical harmonics 구면 어울림함수
solar physics 태양물리학                     spherical harmonics 구면조화함수
solid angle 입체각                         spherical harmonic tensor 구면 어울림텐서
solidifying point 굳기점                   spherical harmonic tensor 구면조화텐서
solidifying point 응고점                   spherically symmetric field 구면대칭마당
solidifying point depression 굳기점 내림     spherical mirror 구면거울
solidifying point depression 응고점 내림     spherical model 구면모형
solid state physics 고체물리학               spherical Neumann function 구면노이만함수
solvent extraction 용매 추출                spherical pendulum 구면흔들이
sound barrier 소리 가로막이                   spherical polar coordinate 구면극자리표
sound barrier 소리 장벽                     spherical polar coordinate 구면극좌표
sound source 소리샘                        spherical shell 구면껍질
source 샘                                spherical surface 구면
south p이e 남극                            spherical symmetry 공대칭
south p이e 에스극                           spherical symmetry 구대칭
space motion 공간운동                       spherical wave 구면파동
 spatial frequency 공간진동수                 spin angular momentum 스핀각운동량
special unitary group 특수 유니터리 군         spin magnetic moment 스핀자기모멘트
special unitary group 특수 유니터리 무리         spin precession 스핀 옆돌기
 specific rotatory power 고유광회전도          spin precession 스핀 옆돌기운동
                                              부록 B . 한국물리학회 공식 물리학 용어집 331



 spring pendulum 용수철흔들이                   system of 이ectrostatic unit 정전기단위계
 square-well nuclear potential            system of international un仕 [=sI] 국제단위계
     네모우물핵포텐셜                             system of material point 질점계
 square-well potential 네모우물포텐셜            system of unit 단위계
 stable equilibrium 안정비김                  tab노 표
 stable equilibrium 안정평형                  tableau 타블로
 stable nuclide 안정 핵종                     tadp이e diagram 올챙이 그림
 stable orbit 안정궤도                       tangential acceleration 닿이선가속도
 stable orbit 안정자리길                      tangential acceleration 접선가속도
 standard deviation 표준편차                 tangential motion 닿이선운동
standard p이nt 기준점                        tangential motion 접선운동
standard point 정점                        terminal voltage 단자전압
standard source 표준샘                      theoretical physics 이론물리학
standing wave 서있는 파동                     theory of differential equation 미분방정식이론
standing wave 정상파동                       theory of electron 전자이론
statistical mechanics 통계역학               theory of potential 퍼텐셜이론
statistical physics 통계물리학                thermal 이ectron 열전자
stopping power 멈춤능력                      thermal 이ectron emission 열전자내쏘기
straight line motion 직선운동                thermal motion 열운동
strength of magnetic p아e 자기극 세기          thermal power generation 화력발전 .
stretching 미bration 늘어남떨기                thermal power station 화력발전소
stretching vibration 신축떨기                thermal 미bration 열떨기
string instrument 현악기                    thermodynamic potential 열역학포텐셜
subun仕 소단위                               thermoelectron 열전자
surface integral 면적분                     three 이ec汀on bond 세전자 결합
surface potential 겉면퍼텐셜                  three 이ectron bond 세전자 묶음
s-止face potential 표면전위                   three- scale- factor universality
surface potential 표면퍼텐셜                      세눈금인자 보편성
survey instrument 측량기                    thresh이d 문턱
survey instrument 탐사기                    thresh이d energy 문턱에너지
symmetrical point 대칭점                    thresh이d frequency 문턱떨기수
system of absolute unit 절대단위계            thresh이d frequency 문턱진동수
system of complete orthogonal function   thresh이d value 문턱값
    완전직교함수계                              thresh이d wavelength 문턱파길이
system of 이ec甘omagnetic unit 전자기단위계      torsion pendulum 비틀림흔들이
332 부록



torsion 미bration 비틀림떨기                  uniform motion 등속도운동
total differential 온미분                  uniform motion 등속운동
total differential 전미분                  unit 단위
total reflection 온되비침                   unitarity 유니타리성
total reflection 전반사                    unitary matr汶 유니타리 행렬
total reflection prism 온되비침프리즘          unitary operator 유니타리 연산자
total reflection prism 전반사프리즘           unitary space 유니타리 공간
transition point 전이온도                   unitary transformation 유니타리 변환
transition point 전이점                    unit cell 단위낱칸
translational motion 나란한운동              unit cell 단위세포
translational motion 병진운동               unit charge 단위전하
translation vector 나란히 옮김벡터             un比 charge 전기씨량
translation vector 병진벡터                 un吐 circle 단위원
transversal vibration 가로떨기              unit 이en祀nt 단위요소
transverse acceleration 가로가속도           unit lattice 단위살창
transverse acceleration 수평가속도           unit length 단위길이
trapped 이ectron 잡힌 전자                   unit line 단위선
triangulation point 삼각점                 unit mass 단위질량
tricritical point 세겹고비점                 unit matr汶 단위행렬
tricritical point 세겹임계점                 unit operator 단위연산자
trigonometric table 삼각함수표               un仕 tensor 단위텐서
triple point 삼중점                        unit vector 단위벡터
triple point 세겹점                        universal amplitude ratio 보편너비 비
triplet potential 삼중항 퍼텐셜               universal amplitude ratio 보편너비 비율
triplet potential 세겹항 퍼텐셜               universal conductance fluctuation
turt川ent motion 난류운동                        보편 전도율 요동
turbulent motion 막흐름운동                  universal Fermi interaction
turning p이nt 되돌이점                           보편 페르미 상호작용
two- scale- factor universality         universal gas constant 보편기체상수
    두눈금인자 보편성                           universal gravitation constant 만유인력의 상수
uniform circular motion 고른원운동           universal gravitation constant 보편중력상수
uniform circular motion 등속원운동           universal instalt川ity 보편 불안정성
uniformly accelerated motion 고른 가속도운동   universality 보편성
uniformly accelerated motion 등가속도운동     universality 이ass 보편성 부류
uniform motion 고른운동                     universal scaling form 보편 눈금잡기꼴
                                            부록 B . 한국물리학회 공식 물리학 용어집 333



 universal scaling form 보편 축척형태         미brational-rotational band 떨기회전띠
 universal shunt 만능가름개                  너brational-rotational band 떨돌기띠
 unstable 불안정                           미brational spectrum 떨기빛띠
 unstable equilibrium 불안정비김             미brational state 떨기상태
 unstable equ小brium 불안정평형               미bration galvanometer 떨기검류계
 unstable equ小brium state 불안정 비김상태      vibration of string 줄떨기
 unstable equilibrium state             미bration of string 현떨기
     안정하지 못한 비김상태                       미br欲or 진동기
 unstable is아ope 불안정동위원소                미bronic coupling 진동전자 결합
 unstable nucleus 불안정핵                  피bronic interaction 진동H전자 상호작용
 unstable nuclide 불안정핵종                 미bronic transition 진동寸전자 전이
 valence 이ec汀on 바깥전자                    미rtual 幻cal point 허초점
 valence 이ec甘on 원자가전자                   미rtual image point 허상점
 van der Waals potential 반데발스 퍼텐셜       voltage 전압
vapo (u)r p아nt 증기점                      voltage adjustment 전압조정
variable capacitor 가변축전기                voltage amplification 전압증폭
variable capacitor 더덜기전기들이              voltage amplifier 전압증폭기
vector 벡터                               voltage drop 전압강하
vector addition 벡터 가법                   V이tage drop 전압내림
vector addit幻n 벡터 더하기                   voltage mu川plier 전압증배기
vector analysis 벡터해석학                   voltage regulator 전압 고르개
vector-coupling coefficient 벡터 결합곁수     v이tage regulator 전압조정기
vector equation 벡터방정식                   vortex motion 소용돌이 운동
vector operator 벡터연산자                   watteless power 무효전력
vector potential 벡터퍼텐셜                  wave mechanics 파동역학
vector product 벡터곱                      wave motion 파동운동
vector space 벡터공간                       wave source 파동샘
vector spin model 벡터 스핀 모형              wave source separation 파동샘 분리
velocity governor 속도조절기                 wave vector 파수벡터
velocity potential 속도퍼텐셜                Wheatstone bridge 휘트스톤 다리
velocity vector 속도벡터                    Wheatstone bridge 휘트스톤 다리흐름길
미bration 떨기                             Wheatstone bridge 휘트스톤 브리지
미brational energy 떨기 에너지                Wien뇽 displac帥ent law 빈의 변위법칙
vibrational mode 떨기 방식                  Wien's displacement law 빈의 자리옮김법칙
미brational partition function 떨기 분배함수   wor川ng voltage 절연내압
334 부록



world point 세계점
world vector 세계벡터
斗ray unit 엑스선 단위
千unit 엑스 단위
yield point 항복점
Young뇽 experiment 영의 실험
Young's modulus 영률
Yukawa potential 유가와 퍼텐셜
zero p아nt 영점
zero point energy 영점에너지
zero-point entropy 영점엔트로피
zero point fluctuation 영점요동
zero point 미bration 영점 떨개
zero power 영출력
저서
 1. 디지탈 사운드와 디지탈 음악 구현에 중점을 둔 八4athematica 4: 放）01. 10.
 2. Visual C++ 6.0으로 구현하는，기초적 물리현상 시뮬레이션： 2001. 5.
 3. Visual C++ 6.0으로 구현하는 수치해석： 2001. 3.




     Visual C++ 6.0으로 구현하는
     정전기학（electrostatics) ·
     기하광학（geometrical o口tics) ·
     기초적인 3차원 컴퓨El 그래픽

     ］판1쇄1 발행   2001년 11월 10일
     저자     최행진
     발행인    모흥숙
     발행처   내하출판사
     주소    서울 성북구 정릉1동 16-12 （우） 136-101
     전화    (02)941-0584/5
     팩스    (02)941-0586
     정가    13,000원


     ISBN 89-88932-25-0
