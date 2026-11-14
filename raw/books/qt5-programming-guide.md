---
source_url: "/run/media/yutae/Data/QT5 프로그래밍 가이드.pdf"
ingested: 2026-11-15
sha256: 042d8dc4a7ef10d595b8f22007988d20b565b8b2c0d9e5757a782e4b99432a34
type: raw-source
method: text-extract
---

# QT5 프로그래밍 가이드 (raw source)

> **출처:** USB 원본 PDF (`/run/media/yutae/Data/QT5 프로그래밍 가이드.pdf`, 로컬 참고용 — git commit 불포함)
> **방법:** 내장 텍스트 레이어에서 `pdftotext -layout`로 추출 (OCR 불필요)
> **쪽수:** 623쪽 | **추출 텍스트:** 1300 KB
> **주의:** 원고는 scan/레이어 추출로 영문·숫자·특수자 일부 아티팩트가 있을 수 있음. 해석 시 원본 PDF와 대조.
> OCR 추출 디렉터리 `raw/books/qt5-programming-guide.ocr/`는 git-ignored (로컬 참고용만) — 본문은 아래에 내장.

## Book metadata
- **Title:** QT5 프로그래밍 가이드
- **Pages (PDF):** 623
- **Source:** QT5 프로그래밍 가이드.pdf
- **Domain:** Programming · 프로그래밍 (예상)
- **Ingested:** 2026-11-15

## Extracted text (all 623 pages)


===== PAGE 1 =====
           小1m斗＋   +1ih尸Hm니小느卞4m中




                                                                              소스 코드 다운로드
                                                                        http://www.cyber.co.kr




                          5
                                       예저1 중심의 애플리케이션 개발을 위한



                                      프로그래밍
                                      가이드 I [fl
                                                           上寸
LU   qe
                                          =
                                              =
                                                                =
                                                                ＝口
                                                                            肛
｛그 OA 匣 亨 邕＼



                                    X, Windows, Linux, Android, QNX. MeeGo, WebOS 등 다양한
           플랫폼을 지원해야 할 때
          8 고급 G니와 야羌nGL 및 OpenGL ES를 사용한 3D 그래픽 애플리케이션을 개발할 때
          8 멀티스레드. 멀티미디어．네트워크， XML JavaScript 지원 애플리케이션을 개발할 때
          0 오픈 소스 웹 브라우저 엔진인 WebK曙 이용하1 인터넷 응용 애플리케이션을 개발할
                                                           때
          0 Back田nd 시스템 관리를 위한 애플리케이션을 개발할 때



                      E乙규성안당


===== PAGE 2 =====
t5
     예제 중심의 애플리케이션 개발을 위한


     프 쿠 그래빙
     가이드 吐，:,.




 성안당


===== PAGE 3 =====
／小＼         예제 중심의 애플리케이션 개발을 위한

V
닌t5 프로그래밍 가이드
2014.   5. 29. 1판 j솨1 발행
                                            저자와의
2015.   3. 9. 1판 2쇄 발행
                                            협의하에
2017.   2. 17. ］판 3쇄 발행
                                            검인생략

지은이 1 김대진
펴낸이     이종춘
펴낸곳 1 匣可주식희사성안당
츠人 04032서울시마포구양화로127첨단빌딩5층（출판기획R&D센터）
' 小 10881 경기도 파주시 문발로 112 출판문화정보산업단지（제작 및 물류）

전화曜漆응娑
팩스 I 031) 955-0510
등록 1 1973. 2. 1. 저406-2005-000046호
출판사홈페이지 1 www.cyber.co.kr
ISBN I 978-89-315-5319-2 (13000)
정가 1 28,000원

이 책을 만든 사람들
기획 ' 진행 1 최옥현
본문 디자인 1 김인환
                                                         女 女 女
표지 디자인 1 박원석
홍보 1 박연주
                                            WW.cyber.CO.k
                                           성안당 Web 사0匡
국제부   이선민, 조혜란, 고운채, 김해영, 킴필호
마케팅 1 구본철, 차정욱. 나진호，0동후. 강호묵
제작 1 김유석


01 책의 어느 부분도 저작권자나 區回주식회사성안당 발행인의 승인 문서 없이 일부 또는 전부를 사진 복사나
디스크 복사 및 기타 정보 재생 시스템을 비롯하여 현재 알려지거나 향후 발명될 어떤 전기적， 기계적 또는
다른 수단을 통해 복사하거나 재생하거나 이용할 수 없음．

米 잘못된 책은 바꾸어 드립니다．


===== PAGE 4 =====
 머리말



Qt는 Embedded Linux, Mac OS X, Windows, Linux, Android, QNX, MeeGo,
WebOS, Symbian 등 다양한 플랫폼을 지원하는 크로스 플랫폼 프레임워크입니다. 예를 들
어 Embedded Linux에서 개발한 애플리케이션 소스 코드를 \Vindows, Andr아d, QNX와
같은 다양한 플랫폼에서 플랫폼의 종속적인 부분을 제외하면 소스 코드 변경 없이 그대로 사
용할 수 있습니다．

또한 Qt는 c++ 이외에 파이선, 루비 등 다양한 언어를 지원하며 전 세계 약 50만 명 이상
Qt 개발자가 다양한 컴퓨팅 환경에서 수많은 소프트웨어를 개발하고 있습니다. 따라서 일반
사용자 애플리케이션, 멀티미디어, 시스템 관리를 Back-end, 자동차, 국방, 가전, 모바일어］
이르기까지 다양한 분야에서 Qt를 활용하고 있습니다．

요즘과 갇이 다양한 플랫폼이 난무하는 개발환경에서 여러 플랫폼을 지원하는 애플리케이션
을 개발하는 것은 쉽지 않은 과제입니다. 예를 들어 안드로이드, 아이폰과 같은 이기종간의
모바일 플랫폼에서 동작하는 동일한 애플리케이션을 개발하는 것은 개발에 많은 시간을 투자
해야 합니다．

하지만 Qt 프레임워크를 사용하면 소스 코드의 변경 없이 다양한 플랫폼을 지원하는 애플리
케이션 개발이 가능하므로 애플리케이션 개발 시간을 단축할 수 있습니다. 그러므로 Qt는 급
변하는 시장에서 강쟁력을 확보할 수 있는 적합한 개발 프레임워크라 생각합니다．

마지막으로 부모의 사랑이 훌륭한 아이를 키울 수 있는 밑거름이 되는 것처럼 많은 관심을 가
져준 독자분들에게 더없는 감사를 드립니다. 그리고 이 책이 Qt 개발프레임워크에 관심 있는
모든 독자분들에게 조금이나마 도움이 되킬 바랍니다. 또한 이 책이 출판될 수 있도록 도와준
출판사 관계자 분들에게도 감사드립니다．


                                                         김대진 드림




                                                               머리말 3


===== PAGE 5 =====
            차려］

CHAPTER 01
0verview                                  9

CHAPTER 02
유용한 툴과 qmake                             17
  ]. 유용한 툴과 qmake                        18
     1.1 Of Creator IDE Tool             18
     1.2 Of Assistant                    26
     1.3_at Designer Tool                28
    1.4_qmake                            29


CHAPTER 03
GUI 설계와 제작                               30

  1 Basic Widget                         30
    1.1_OCheckBox2F OButtonGroup         37
    1.2 OComboBox                        40
    1.3OCommandLinkButton                41
    1.4_ODate 클래스와 ODateEdit 위젯          42
    1.5 O기me 클래스와 O기meEdit 위젯            46
    ]. 旬ODateTime 클래스와 ODateTimeEd仕 위젯   50
    1.7 OD回                              51
    1.8_田pinBox와 ODoubleSpinBox          53
    1.9 OPushButton과 QFocusFrame         55
    1.10 OFontComboBox                   58
    1.11 OLabe꽈 OLCDNumber               60
    1.12 O［그neEd仕                        62
    1.13 OMenu와 OMenuBar                 64
    1.14_OProgressBar                    67
    1.15 ORadioButton                    68
    1.16 OScrollArea                     70
    1.17 OScrolIBar                       71
    1.18_OSizeGrip                       72
    1.19 OSlider                         74
    1.20_OTabWidget                      76
    1.21 OToolB可와 OAction                78
    1.22아呱均et                            80
    1.23 OlabBar                         85
    1.24 OToolBox                        87
    1.25 OToolButton                     88
  2. 레이아웃                                90



4 차려1


===== PAGE 6 =====
 3. Advanced Widget                  94
   3.1 QColumnView                   95
   3.2_ODataWidgetMapper             96
   3.3_QDesktopWidget                98
   3.4_OCalendarWidget              100
 4. Designer를 이용한 GUI 폼 제작          ]03
   4. ] 위젯과 시그널 슬롯을 사용한 예제          ]06
   4.2 Calculator Form 예제           108
 5. 다이얼로그                           111
   5.1일반 다이얼로그                      ]11
    5.2사용자 정의 다이얼로그                 ]21
 6. Main Window                     123
 7. 卜加del/View 아키텍처와 데이터 바인딩 위젯     ]27
    7.1_Mod이/Vi이V 아키텍처              ]27
    7.2_Mod터 클래스와 \hiew 위젯의 활용      ]29
 8. 사용자 정의 커스텀 위젯과 플러그인             ]34
    8.1 사용자 정의 커스텀 위젯 구현            136
    8．乙플러그인 제작과 배포                  147

CHAPTER 04
시그널과 슬롯                             157
  ] . 시그널과 슬롯                       ]58

CHAPTER 05
데이터 타입과 유용한 데이터 조작 클래스              ]61
  ]. 데이터 타입과 유용한 데이터 조작 클래스         ]62
     1.1변수 비교／판단 함수                 ]65
     ] .乙데이터 클래스                    167
     1.3_Container 클래스              ]87
     1.4문자열 클래스                     ]93

CHAPTER 06
파일 입출력                              197
  ] . 파일 입출력                        ]98
      1.1_SIMPLE 파일 \flEW 예제        202

CHAPTER 07
그래픽스                                207
 1. QPainter 클래스를 이용한 그래프           208
    1.1_QPainter으I Basic Drawing    210


                                   차려 5


===== PAGE 7 =====
        차려］



   1.2 Gradients                          217
   1.3 Trans幻曲at山n                        220
   1.4_Composition                        222
  2. （計a아기cs View 다amew아k                 224
   2.1_Graphics View Architecture         227
   2.2_Graphics View의 좌표                  230
   2.3_Gra아）ics View의 주요 특징               231
   2.4 이벤트 처리                             233
   2.5사용자 정의 QGr야巾ic引也m                   235
   2.6_QGraphicsEffect                    238
  3. Of OpenGL 모듈을 이용한 3D 그래픽             243
    3工3D 그래픽 렌더링을 위한 QGLWidget 클래스        245
    3.2_Hello OpenGL 예제                   248
    3.3 HW 가속기를 이용한 2[) 그래픽 렌더링           255
    3.4 OPainter 클래스의 Over Painting       261
  4. Scalable Vec幻r Gra아기cs               269

CHAPTER 08
Animation Framework과 State Machine        273
  1. Animation Framework과 State Machine   274
     1.1 Animation 아키텍처와 클래스              275
   1.2_Animation과 State Machine           283

CHAPTER 09
Thread                                    287
  1. Thread                               288
     1.1 QThread 클래스                      292
     1.2 멀티 쓰레드 프로그래밍                     295
   1.3_Thread Wait Condition              298
   1.4_Sema아iore률 이용한 동기화                 301
   1.5 아Concurrent를 이용한 멀티 쓰레드            303

CHAPTER 10
（兀ntainer 클래스와 Iterator 클래스               307
  ] . Container 클래스와 Iterator 클래스         308
      ].] Java 스타일의 Iterator 방식· ·        309
      1.2_STt, 스타일의 Iterator 방식           312
      1.3 foreach 키워드를 이용한 1terat가 접근     313

CHAPTER 숴
XML                                       315


6 차려1


===== PAGE 8 =====
 1. XML                                               316
    ] .］즈트림을 이용한 XML 데이터 핸들링                          3侶
    1.之Document Object 卜加del                          321
    1.3_Sim이e Al기 幻r XML                              325

CHAPTER 12
데이터 커뮤니케이션과 인터넷 프로그래밍                                 329
 ]. 네트워크                                              330
   1.1_QTc口Socket고｝ QTcpServer를 사용한 TCP 프로토콜 프로그래삥    335
   l .之oUdpSock아을 사용한 UDP 프로토콜                        344
    j 旬호스트 네임과 DNS 검색                                 350
   1.4_HTTP(HyperText Transfer Protoc이） 프로토콜          358
   1.5_Bearer Management                              368
   ] .q서버／클라이언트 기반 채팅 예제                              370
 2. 0싸VebK仕                                           378
   2.LOtWebkit 모듈에서 제공하는 클래스                          381
   2.2_DOM(Document O히ect Model) 검색                   388
    2.3_QtWebKit 모듈 환경에서 JQuery 활용                    391
    2.4_QtWebK仕과 OO히ect 卜加d이 간의 Bridge                396
    2.5_Hybrid 클라이언트 어플리케이션 예제                        403
 3. Inter-Process Communication                       407
   3.1 TCP/IP                                         408
   3.2_Shared Memo四                                   409
   3.：王D-Bus Pro佃c이                                   415
   3.4아가ocess                                         423

CHAPTER 13
멀티미디어                                                 425
  ]. 멀티미디어                                            426
     1.1오디오 컴포넌트                                      427
     ].乙비디오 컴포넌트                                      431
     ].旬카메라 컴포넌트                                      434
     1.4＝라디오 컴포넌트                                     436

CHAPTER 14
데이터베이스                                                439
  ]. 데이터베이스                                           440
     1.1 데이터베이스와 SQL 이해                               442
     l .乙데이터베이스 연결과 지원하는 드라이버                         445
     ].乙S（그L 구문을 사용한 데이터베이스 질의                        454
     1.4 卜,lod이 클래스                                   461



                                                     차례 7


===== PAGE 9 =====
        차려］



    1.乞Table View의 활용               464
    1.6_SQL- 레코드 필드와 GUI 위젯 매핑      466
    ].乙Cached 테이블 예제                471
    1.8_Drill Dow,) 예제              474

CHAPTER 15
Of Test Framework                   487
  1. Qt Test Framework              488
     1.LUnit Test                   492
     ].之데이터 주도 테스트                  494
     ].乙GUI 이벤트 시뮬레이션               496
     1.4_GUI 이벤트 Replay 테스트         497
     ] .乞벤치마크 테스트                   499

CHAPTER 16
O1O내ck과 QML                         503
  ]. （가 Quick과 QML                  504
     1.1_Qt Quick 프로젝트 생성과 유용한 툴    505
     1.2 기본 타입과 확장된 데이터 타입          508
     ].｛아이템                          514
     1.4사용자 입력과 이벤트 처리              526
     1.邑아이템 Positioning             532
     1.6요ate와 Transition            535
     1.7_Animation                  539
     ].＆데이터의 표현                     546
     ]. q모듈화 프로그래밍                  551
     1.10_Graphic Effects           557
     1. 任유용한 QML- 타입                581
     1.12 Canvas                    584
     1.l3lntegrating QMLaF C++      587
     1.14 卜巾기timed治                 593

CHAPTER 17
Of 어플리케이션 배포                        597
  ]. 다양한 플랫폼에서 （코 어플리케이션 배포         598
     1.1_Un以와 니nux                  599
     1.2 Windows                    600
     1.3 Mac OS X                   601
    1.4_Andr이d 플랫폼에서 （값 어플리케이션 배포   602

찾아보기                                618




8 차려1


===== PAGE 10 =====
CHAPTER




   Overview


===== PAGE 11 =====
0t 5 Programming




r i 'Overview
              어플리케이션 개발을 위한 （코 개발 프레임워크에 대하1 알아보자．




Qt는 개발자에게 현대적인 GUI 인터페이스를 쉽게 설계하기 위한 API뿐만 아니라 응용 어플리케이션 개
발에 필요한 다양하고 방대한 API를 제공한다. Qt는 c++ 기반의 응용 어플리케이션 개발과 Qt Quick을
이용해 어플리케이션 개발이 가능하다. Qt 鈿ick은 QML 언어를 사용한다. QML은 인터프리터 언어로써
c+＋를 알지 못하더라도 QML를 사용해 응용 어플리케이션 GI끄를 디자인 및 설계할 수 있다．

QML은 declarative 언어이며 （절차 언어） 자바스크립트가 확장된 스타일의 문법구조를 가지고 있다．
QML은 JavaScript와 같은 절차 언어를 해석하는 Declarative 모듈이 있으며, c+＋을 사용해 소스 코
드를 작성하면 컴파일러가 실행 바이너리를 생성하는 것과 같이 Declarative 모듈은 QML로 작성한 코
드를 실행할 수 있는 어플리케이션으로 변환하는 작업을 한다. 또한 QML 어플리케이션 내에서 C＋十
API를 사용할 수 있다．


風mainq빤‘ 管昏壽磁的：; :::m나珏堪抵混m磁難蠶瑟繫聲饔藝鑿罌難難難驪發                                                                     1白
 蔑缸느各套烏心纛諱婉建磁唾轟努H竄났球蚤器各無蚣拉煎好曲唾解弑證磁磁弦낢泣二七＝已髥瓷轟轟多瑟熬瑟難箋薛瑟蘿器g器蘇發
       Proi白：t;  ! 묘. 包 日＋ 夕 宰 呻 ri-I日LI그nil 匹 TeHt    寸  二
  J／日ice rr日 4 如 H出刈似玭d                            1        imj그（그rt QtQuick 2 . 0                                  스
    ＝三匍          隘 HelloWorld.pro                  L
二 0.名t口n       4 hqtq미比2applic欲由nviewer            3 4 Rectangle
重 幽bt,口             颱 qtq내ck2applicat幻n너們ver.pr    4       width: 360
冒 尸roj日C노            h Headers
큼    打，lyzo          C..   Sources
                                                   5
                                                   6 '
                                                           height:
                                                           Text {I
                                                                     360

旨  H日｛1그        4 CH Sources                       7           text:   qsTr ( "Hello                     World")
i 마: : :            드：크 main.cpp
                                                   S                  anchors               centerln:    工그크ren亡    量
                4 딴已 QML
                                                                                        -

f    -                                                           }                                                  :.


                  4 缸 qml/Hello＼幷orid
                                                   드5
亘    ; "                                          IC- '         MouseArea {                                         /
클 갸b四                      圓 ma1n,qm1             ll                카-I-｛닸lors , fill:                paren亡
貫                                                 J 八   J             r\ Y) r시 }   jIZlr그r4   =   1                 !


（그림） QML 프로젝트




10    CHAPTER 01_ Overview


===== PAGE 12 =====
Qt 鈿ick과 QML을 사용해 응용 어플리케이션을 구현하는 경우 Qt 帥ick과 QML로 완벽한 응용 어플
리케이션을 구현할 수 없다. 예를 들어 녜트워크 Traffic 사용량을 확인하기 위한 어플리케이션을 구현
하기 위해 시스템 레벨의 네트워크 Traffic을 제어하기 위해 Native 라이브러리 사용이 필요하다. 따라
                                                        네트워크
서 사용자에게 제공하는 GUI 단은 Qt Quick을 사용해 네트워크 사용량을 그래프로 표시하고
Traffic을 측정하는 실제 구현 API는 전통적인 Qt API 혹은 시스템 레벨의 API를 사용해 구현하는 것
이 가장 바람직하다．

따라서 Qt Quick으로는 GI끄를 구현하고 실제 기능이 동작하는 모듈은 전통적인 Qt API를 사용해 구현
할 수 있다. 이러한 방식은 HTML5를 이용해 응용 어플리케이션의 구조와 흡사하다. 즉, 사용자에게 제
공하는 GI끄는 HTML5를 사용하고 실제 동작을 담당하는 모듈은 Native API를 사용해 HTML5 기반의
응용 어플리케이션을 구현한다．

Qt 帥ick을 사용하면 디자인 로직과 프로그램 로직을 분리할 수 있는 장점이 있다. 즉 C+＋와 같은 프로
그래밍 언어의 지식 없이 QML만 이해하고 있다면 GUI를 디자인 할 수 있다. QML은 HTML5와 유사하
며 직관적이고 이해하기 쉽다. 그리고 전통적인 C十＋에서 제공했던 기능을 모두 지원한다. 예를 들어
QtWebKit, Animation, 멀티미디어 등을 QML에 사용이 가능하다．

또한 Qt는 다양한 멀티 플랫폼을 지원한다. 예를 들어 MS Windows, Linux/Un奴, Mac OS 뿐만 아니
라 모바일 및 임베디드 디바이스 플랫폼과 같은 Android, iOS, Windows 8(WinRT), BlackBerry 10,
QNX, VxWorks, Embedded Linux 플랫폼도 지원한다. 즉 플랫폼의 종속적인 기능을 제외하고 소스
코드를 다시 작성하지 않고도 다양한 플랫폼어］ 동일한 기능을 적용할 수 있다．

Qt는 네트워크, 그래픽스, 데이터베이스, OpenGL/ES, WebKit, HTML5, 멀티미디어 등과 같은 다양
한 API를 사용해 구현한 응용 어플리케이션을 다양한 플랫폼에 적용할 수 있으며 각 플랫폼에 동일한
IDE 툴을 사용해 적용할 수 있다. Qt는 공식 IDE 툴로 Qt Creator 툴을 제공한다. Qt Creator는 Qt
Designer와 Help 기능이 Assistant 기능이 통합된 환경을 제공한다. 따라서 개발 시 Qt API 중 좀더
자세한 정보를 원한다면 해당 클래스 혹은 함수에 커서를 위치하1 놓은 상태에서 團을 클릭하면 해당 API
어］ 대한 자세한 정보를 쉽게 찾을 수 있다.




                                                               1 0verview 11


===== PAGE 13 =====
    'n 口echarih - chapt蛇．n,eth叱5. （간 口的tar
      F加   Ed仕   Build   Deb시g   Are肛e   1刈5    Wirx幻기Y
                                                                                        <Setect S戶nbol>
                 d E chapter2-methods
                     圃 chapter2-rnethodcpre                  tifndef    PIECBIART H
                   J j,, Headers
                                                             !define    PIECHART H
                        曲 piecha比h
                   1 E. 鈿urces                               tinclude <QtQuickfQQuickPaj.ntedltem>
                        凸 rnan.cpp                           tiruclude <QCo]工그r>
                         츠 마echartcpp
                 d n 叩瞰油ness
                                                            I/ f (0]
                     匠ipostttonfSpr口                      d class pieChar七 : 口t上i표ic QQujCicpain七edltem
                   d e. S에rces
                                                             {
                         包 m哥n-cPp
                                                            If! [0]
                     m Resources                                  Q OHJECT
                         E C:/QtJQ好02八0刀cue,                      Q PROPERTY JQString n카ne READ name WRITE setName)
                          回 shared.qrc                            Q PROPERTY (QCOlor color READ color WRITE 드etColor)
                        Ip야出one八甲C
                                                             II! [1]
                                                             pub! 工C:
                                                             I/ tEl]

                                                                 PieChart (QQuickltem 丹parent = 0) ;

                                                                 QString n丑始 () corust;
                                                                 void oetName (const QString Ename) ;

                                                                 QColor color) )      -orust;
                                                                 void setColort        : st QColor 됴color) ;



                                                  回卜＄Sues田S日arch 日S＄吐＄日Applicalior Output四Corn呻 Ou匈Ut月OM나iS Coos이e


（그림）（가 Cre計or IDE 툴



Qt에서 제공하는 API는 다양한 분야에서 활용할 수 있도록 방대한 API를 제공하며 구현하기 쉽고 직관
적인 구조의 라이브러리로 제공되므로 소스 코드 작성이 쉬울 뿐 아니라 직관이므로 어플리케아션 개발
어］ 소요되는 시간을 단축할 수 있다．


I （가에서 제공한 GUI 위젯
=
       e Case sensitive                        됴t너so                                   Pack自ge selet［口n
                                                          쓰ar믹no

                                                                                        YUpdat兮 $y就em
       . Search from the cursor                  브．eadirsq
                                                                                          Jpdate applications
                                               斗 므ara했’aph
     Enter your name                                                                      뱌）date 如cumerl伯t山Sr
                                                 LISt



                                                                                        口
     (art 14. 2005 4:19:00 PM                    F口otn口Ia
                                                                                                                245自


    Bitstream＼旭ra San놔               V              Br口叫Sc n        Cancel




12 CHAPTER 01_ Overview


===== PAGE 14 =====
小 0口enGL을 이용한 그래픽스
Qt는 2D 및 3D Painting 뿐만 아니라 0penGL과 같은 그래픽 API와 SVG API와 멀티미디어 기능을
쉽게 구현할 수 있는 API를 제공한다．




（그림） OpenGL을 이용한 3D 그래픽 프로그래밍



모바일 및 임베디드 디바이스 환경에서는 3D 그래픽스를 적용하기 위해서는 3D 그래픽 가속기를 지원한
다. Qt는 3D 그래픽뿐만 아니라 21) 그래픽을 311) 그래픽 가속기를 적용할 수 있다. 따라서 Qt는 2D와
3D 그래픽 모두 하드웨어 그래픽 가속기를 사용할 수 있다．


eWebK什을 이용한 웹 응용 어플리케이션
Qt는 WebK此을 지원한다. 따라서 인터넷 웹 브라우저 및 인터넷 콘텐츠를 이용해 응용 어플리케이션 구
현이 가능하며 HTML5를 사용할 수 있다．

                    쁘竺 匕        H1中1 뽀쓰 ＞旨J브크 느二멤 二므    1                                    뇨吐m 1 心1
                            카




                    Got셍C ＝뇨m呻，,,,,,, ,,,
                                                                               滋好易m,       브口U1쓰t皿n

                                                            方［母나ci好 i

                     HmhH1            Hy H 11m                          n   기目1 匹王 }U1d H m1 1口 n11


                    中；：茗．,
                      M1\        ;U1;E t11 d K:
        小
                      h1m
                      f1nhri-   1a1 1

                      m1



                     已1寸
r기斗쿠"
                      1나1mH       m



                      蜘堈
                                                   .

                      斗mmn月L m1r口1 t姓 目甘甲，
                                         口i山바
                      畔＝




 "      戶m

                i   ':1 涵：琺每芬三＝ =
                                                  ak去늠카- mm呻． .4出1...m.,mr노욘 :


（그림） WebK什을 이용한 월J 응용 어플리케이션 실행 화면


                                                                                                        1 0verview 13


===== PAGE 15 =====
 好 WebK作을 이용한 웹 응용 어플리케이션
 Qt는 UI 디자인 설계를 위해 기본적으로 제공한 위젯 혹은 컴포넌트 이외에도 사용자 정의 위젯과 帥ilL
 을 이용해 사용자가 직접 위젯을 디자인 할 수 있다．




（그림） 위젯 커스터마이징



 蜘（코5에서 새롭게 추가된 기능
Qt5는 가장 최신 버전이다. Qt5에서는 QML과 JavaScript를 사용할 수 있을 뿐만 아니라 HTML5와
같은 웹 응용 어플리케이션이 개발이 가능하다. Qt5에서는 OpenGL을 이용한 다양한 애니메이션 효과
가 추가되 었다．




（그림） 이미지에 Shader Effect 적용



Qt 帥ick은 Qt4에서부터 지원하였다. Qt5에서는 Qt Quick 버전 2.0을 사용하며 HT入4L5와 비슷한
Canvas 기능이 추가되었으며 다양한 2D 그래픽 Effect 기능이 추가되었다．




14 CHAPTER 01_ Overview


===== PAGE 16 =====
（그림） 2D 그래픽 Effect



또한 Qt Quick에서 Graphical Effects 모듈을 사용해 Soft dr아） shadow, Blur, Glow 그리고
C아orize 등과 같은 다양한 Effect를 사용할 수 있다．




（그림） Graphical Effect



Qt5에서 Qt Quick 2.0을 사용할 경우 OpenGL/ES 2.0 기반의 Qt Quick Graphic Scene 그래프를
사용할 수 있다. 그리고 애니메이션에서 SpriteSequence 타입이 새로 추가되었다．
그리고 Qt5에서는 C++ 뿐만 아니라 Qt Quick과 같은 QML에서 멀티미디어 모듈을 사용할 수 있다. 여］
를 들어 Qt Quick에서 컴포넌트를 통해 멀티미디어 영상 출력이 가능하다. 그리고 Camera와 Radio 기
능은 API를 통해1 접근할 수 있다．




（그림） 01 Quick을 이용한 멀티미디어 영상 출력


                                                              1 Overview 15


===== PAGE 17 =====
1


===== PAGE 18 =====
CHAPTER




  유용한 툴과
    qmake


===== PAGE 19 =====
Qt 5 Programming




I尸꺼 유용한 툴과 qmake
瑟
驀

           어플리케이션 개발을 위해 （가7F 제공하는 유용한 개발 툴에 대해 알아보도록 하자．




Qt는 개발에 필요한 IDE(Integrated Devel아)ment Environment) 툴인 Qt Creator, Help
Docum아此인 Assistant, 또한 GUI를 디자인 하기 위해 Designer 툴을 사용해 쉽게 GI끄를 설계할 수
있다．

그리고 Qt로 작성한 응용 어플리케이션 소스 코드를 바이너리 실행 파일로 컴파일을 지원하기 위한
qmake를 제공한다．

 Tool              설명
 Qt Creator        IDE 툴로서 Qt 응용 어플리케이션 개발을 위한 툴
 Qt Assistant      Ot A믹에 대한 He巾 Document 툴
 Ot Designer       소스 코드를 작성하지 않고 GU를 쉽게 설계하거나 위젯을 배치할 수 있는 툴
 Qmake             （거로 작성한 예제 코드를 컴파일을 쉽게 할 수 있도록 지원하는 툴



이번 단원에서는 Qt 응용 어플리케이션 개발을 위해1 제공되는 툴과 qmake어］ 대해 살펴보도록 하자．


          1 Qt Creator IDE Tool

 Qt Creat아는 Qt Framework를 사용해 응용 어플리케이션 개발을 지원하기 위한 IDE(Integrated
 Development Environment)이다. Qt는 Unix/Linux, Windows, Mac OS X, Android, Black-
 berry, QNX 등 다양한 플랫폼을 지원한다. 상이한 플랫폼상에서 Qt Cre毗아는 동일한 개발환경을 제
 공한다. 그리고 Qt Creator IDE 툴을 사용해 구현한 응용 어플리케이션을 개발 타깃 플랫폼에
 Deployment 기능을 제공한다．

 예를 들어 Embedded 디바이스와 같은 모바일, 태블릿, 임베디드 리눅스 등과 같이 원격어］ 떨어진 개발
 타깃에 응용 어플리케이션을 직접 실행할 수 있다. 즉, 컴파일이 완료된 Qt 응용 어플리케이션을 실제 디
 바이스상에 실행시켜 보므로 편리하게 디버깅 할 수 있다．




 18 CHAPTER 02_ 유용한 툴과 qmake


===== PAGE 20 =====
II p.ec9a5 1- chapter2-methods - Qt C "eator
                             사油肛       b09     tedsd메          He巾
                                                 小      中               ["nh,批 h             -   [S.ledSyntboI[
               ti '4日pte52-0닢0yX1S                                  \   /
                 昴 thopt甘2-methods 며0                                   #ifod日f PIECHART H
               1 is' ！忙eden                                             tdodine PIECHART H
                     匹 呻oh布th
               1 t느 toureR                           巨3                 finC끄ode <Q七a口工CE力；놔戶 :kPaintedltem>
                     qe mam 다까J                      44                 $iso1ud. HQColor>
                     므 P吐ha凡'Pp                      d=
             C r 的5作mner1                             46   II! (0)
                  配 四m0呻5 丁D                          47 J ci크so Piechar七 : pat: i亡 QQuichPa工ntedltem
               1 th SOureR                            40    4
                     t中 m라horn                        49   (14 (0)
               a . 七巧｛yJrreg                          SC        Q OBJECT
                  1j. C (Q口Qt.0.2/5.O-2/snnat         51        3 PROPERTY ( QItring 0帥｝e R旦互0 name WRITE so七Na皿e)
                        固 5hared qr(                  52        3_PROPERTY )口Color color R旦AD color WRITE setColor)
                     立 叩see',甘5 甲
                                                      升
                                   （
                                                  1
                                                  r                     (Il (1)


                                                     끼 亡m q     m
                                                                        pub100t
                                                                        /11 (1)


                                                              나
                                                              n n
                                                            n:口
                                                      二 r 5y
                                                                             PioChart (QQuickttem 什parent = 0) ;
        가牛

                                                              亡
                                                                             Qstring name) ) Bon 亡;
                                                                             Void setName)conat OString Afl카ne) ;
    卜
                                                                             UColor color) ) const;
                                                                             void setColor) oonst OColor Acolor) ;



             U                                    口1 Ue 日Se仙 日esulls月Hp的如的나HumCov呻 I; '口Ut目叩나Js C口n5미巳


（그림） 01 Creator I［正 툴 실행 화면


또한 Qt Cre毗야는 Qt Designer와 H이p 기능이 Assistant 기능이 통합된 환경을 제공한다. 따라서 개
발 시 Qt API 중 좀더 자세한 정보를 원한다면 해당 클래스 혹은 함수에 커서를 위치해 놓은 상태에서
團을 클릭하면 해당 API어］ 대한 자세한 정보를 쉽게 찾을 수 있다．

개발을 하다 보면 여러 명과 함께 개발을 하는 경우가 있다. 여러 사람이 함께 개발을 하기 위해서는 Git,
CvS 등과 같은 소스 형상관리 툴을 사용하는 경우가 많다. Qt Cre毗町는 이리한 형상관리 툴과 연동해
Qt 프로젝트를 관리할 수 있는 기능을 제공한다. 그리고 Qt 응용 어플리케이션을 디버깅하기 위해 GNU
Symbolic Debugger(GDB), Microsoft Console Debugger(CDB), QML/JavaScript Debugger를
지원한다. 또한 소스 코드상에서 메모리 누수와 같은 문제점을 찾아내고 분석하기 위한 툴을 지원한다．
지금까지 언급한 Qt Cre毗야의 기능에 대해 자세히 살펴보도록 하자．


巾 ot 프로젝트 생성
Qt Creator에서 개발할 새로운 프로젝트를 설정하는 방법은 프로젝트 생성 과정에 따라 Step 단위로 단
계별 가이드어］ 따라 프로젝트 \Wizard를 사용해 프로젝트를 생성한다. Qt Creator는 프로젝트 \Wizard
어］ 의해 프로젝트를 생성하기 위해 Qt Build to아인 qmake를 사용한다. qmake어］ 대해서는 추후 자세
히 설명할 것이다．

Qt 프로젝트 \Wizard를 생성해 프로젝트를 생성할 수 있지만 qmake 만을 사용해 메모장과 같은 에디 터
상에서 프로젝트를 생성할 수 있다. 이러한 방법은 추후 설명하기로 하고 이번 장에서는 프로젝트
Wizard를 사용해 프로젝트를 생성해 보도록 하자．

Qt는 다양한 플랫폼을 지원하며 동일한 개발 환경(IDE）인 Qt Creator 인터페이스를 사용한다. 따라서
플랫폼이 다르더라도 동일한 방법을 사용해 프로젝트를 생성할 수 있다．

다음 그림에서 보는 것과 같이 새로운 프로젝트 생성을 위한 프로젝트 Wizard를 실행한다. 프로젝트를


                                                                                                                      ] 유용한 툴과 qmake 19


===== PAGE 21 =====
생성하기 위해서는 Qt Creator의 [File] 메뉴를 선택하거나 區피＋［苞을 눌러 실행할 수 있다．


 Choose a totra미Orn                                                                                                   Desktop Templates 1

   m胎05                                      口   Qt Gut立附］Ca的n                                 Creates a Ut a마川colon for 5Pme dust如다．
  m                                              a 伽以 1 Appbc000e IOU小tn 딤arrests)             Includes a 마 On引gnem나rased main wind口1V
   Libraries                                 +u크 Qt Quick 2 appltcatleer touilt-jn 目e1rsnt5j   Pres이acts a deslit마1 그ttom bull비ng the
                                                                                               a마내cat向nlieu玔ab咆
   otf臣r Pr이eQ                               피 a Qusk 1 4먀）hr計心n lInen, E出500gQ卜CL F


                                                쁘，’，客『，
                                                      :：「
                                                        ,"'"' "口""" ' "" "
                                                                                               Supported 미atfoeros: Do크en凸二

                                             i二「，
   사criaQt Pr이ml
   Import Project
  F加sand Cl冬5e5                             呵    FIT卜月L5A y口eat心n
   C,+                                       <   Qt Quick jut
  （겯L                                        렵 QtQth改 do'
  ｛꾜 SI
   5尸floral


                                                                                                                                   Cane이




（그림） Ot Creator의 프로젝트 Wizard 실행 화면



Wizard 첫 번째 화면에서는 구현하고자 하는 Qt 응용 어플리케이션 종류에 따라 프로젝트를 선택할 수
있다. 예를 들어 위젯 기반의 GUI 응용 어플리케이션, Mobile 기반의 어플리케이션, 시스템 기반의 어
플리케이션 등과 같이 종류어］ 따라 프로젝트를 선택할 수 있다. 여기서는 GUI 기반의 어플리케이션 걔발
을 위한 프로젝트를 생성하기 위해 [Pr이ects] 탭에서 [Applications］를 선택하고 중앙에 위치한 리스트
에서는 [Qt Gui Application］을 선택하고, 하단의 [Choose] 버튼을 클릭하면 다음 \Wizard 화면을 선
택한다．

두 번째 \Vizard는 Class Wizard 화면이다. 이 Step에서는 C++ 소스 파일과 혜더 파일명을 지정하고
생성할 프로젝트 Base 클래스를 지정한다. Base 클래스는 帥ilainWindow, QDialog, 印Widget 중 하
나를 선택할 수 있다. 여기서는 邸Widget을 선택하고 （끄ass 이름으로 MyWidget으로 입력한다．

아래 하단의 [Generate form] 항목의 체크박스는 프로젝트 Designer를 사용해 포함할 UI를 지정할 수
있다. Designer는 GUI 컴포넌트들을 마우스로 드래그하여 1끄를 배치할 수 있다．




@ 已Qt          Gui Application


                           Class 1nFormaton
        Location
        K附                 Specify basic information about the classes for which you want to generate skeleton source code
                           files
  4Detailo

         Sumnmo四           口ass name:       卜dy바너get
                           日ase 이coo        唯쌔如et

                           Header file r    rnywidget.

                           Source file:     ri가lwidg日t C［叩
                           Generate form:
                           Form tile:       mywfdgelui




                                                                                                                 N已；at    ]   ,   Canc미     ]

（그림）（긔ass Wizard 화면


20 CHAPTER 02_ 유용한 툴과 qmake


===== PAGE 22 =====
（끄ass Wizard 화면에서 보는 것과 같이 [Next] 버튼을 클릭해 다음 화면을 실행한다. 다음 화면은 지금
까지 프로젝트 Wizard로 생성한 결과를 Summary 내용을 보여주는 화면이며 , 아래 [Finish] 버튼을 클
릭해 프로젝트 생성을 완료한다．

프로젝트 생성을 완료하면 프로젝트 파일 중 확장자가 . pro 파일이 생성되었을 것이다. 이 파일은 프로젝
트 컴파일어］ 필요한 라이브러리 및 모듈을 지정한다. 예를 들어 개발하려는 Qt 응용 어플리케이션이
Network 모듈을 사용한다면 . pro 파일어］ network 모듈을 다음과 같이 추가해야 한다．

 n ：朴t口
     『小：巴t- Qt Creator=                            1                         찌麝1i轟量                            믹回出늬
    tie      Ed忙   guild      Debug       At引yze   配4뇌5 ＼사ndow   He巾
                   Pruiects           !   묘 包 日＋ X      中 中      18就마0                  1              Line: 1tC미 23   zr


    ,，』注
         크11
                   '           印，
                       1 =h HeadEr5
                       「亂，                                   ;
                                                        「 甘 Pro그eCt Crea七ud by 야Crea七口r 2013-05-12T10r11: 1了
                                                                                                                            '


                             1, roy느心idgth              口 i
!                      a C _ SOurtos                     三 3
i                            （戶 mam CDn                  』1
i " " "" '                  三rrryzidgetrpp              了 QT         -'-=czrc gui
「 P，品Ct됴               J / 陌rm드                          프
 !                            댑 nrytvrdget ui            드’ gr日a七orThaniQT OSAJOR V呂1之0I（乂寸『 4) : QT += widgee므
     二    ]r; i日                                         U

                                                        ,只 } 0갚act只밋 = test
          'dD                                            L三 쪼뫄lb江』A낏8 = ai：匹1
                                                           3
        油                                                l長
      : 甘』'                                              55 80｛狂亡C묘S += maim旺'F'
!    D8bU口                                               l弓           mywidge七．口pp
i                                                        i싸
i    卜                                                   蚣18므AD쯔155 *= roywidge七．l寸
                                                         三 ‘多
                                                        3d P018188     *= mywidget.ui
                                                         묘:


                   1그 ) J                           /        口冷sues田Search日es岫日App沁刻0恤如Ut心帥曲帥us.

（그림） Qt Creator 프로젝트 실행 화면



Qt Creator에서 제공하는 프로젝트 Wizard는 Qt 응용 어플리케이션 이외에 Qt 라이브러리 개발을 위
한 \Wizard 등 다양한 종류의 프로젝트를 생성할 수 있다．


D 프로젝트 버전 관리／형상 관리
Qt Creat아는 프로젝트 버전 관리／형상 관리를 통합할 수 있도록 다양한 버전 관리 시스템을 지원한다．

    종류                            URL                                                                              비고
    Bazaar                       http://bazaar.canonical.com/                                                     （값 Creat그r 2.2 이후 버전
（기earCase                        h뺘)://www-01 !bm.corn/so伽陷re伯岫to毗／이earcase/                                      （거 Creator 2.6 에서 플러그인 설치
    Cvs                                     ＼사. cvshon冶.0四
                                 http:II니／＼八／
（引t                              h먀刃Ig十scm.com/
    Mercurial                    http://mercuriaI.seIenic.com/                                                     Qt Crea伯r 2.0 이후 버전
    Perforce                     http://www.pertorce.com                                                           Server 2006.1 이후 버전
    Subversion                   http://subversion.apache.org/




                                                                                                                                L유용한 툴과 qmake 21


===== PAGE 23 =====
Qt Creator에서 버전 관리 시스템을 사용하기 위해 클라이언트 PC에 버전 관리 시스템에서 다운로드
받을 디렉토리를 지정해야 한다. 클라이언트가 지정한 디렉토리 PATH를 지정하기 위해 Qt Creator 메
뉴에서 [Tools] + 四ptions] -                                     [Version］을 선택해 사용할 버전 관리 시스템을 설정하면 된다．


                       Version Control

                       3ener히     日i: J카      i      三亡rn1   dn Un 키   1，
                                                                        山 jrS.Sfl    P巳rt口CH   C吃

                       / 붜ra口 eubmit m已 1］日 크1        亡 h키 玎1



                       B止mn message check script

                       Jser/allae conlguralon tie

                       hluerSe너드 二onhtggret口r file

                       SSV prompt commgedl

                       Patch command:




                                                                                                                      App山




（그림） Qt Creator의 버전 관리 시스템 설정 화면


$ 프로젝트 日川d 및 Run 설정
Qt Cre毗야는 개발하려는 플랫폼에 따라 Build와 실행을 지정할 수 있다. 예를 들어 안드로이드, QNX
혹은 임베디드 리눅스와 같이 물리적으로 분리된 개발 플랫폼에 개발환경을 맞춰 빌드와 실행할 플랫폼
을 지정할 수 있다. 현재 프로젝트에써 설정을 수정하키 위해 L西 ＋흐를 누르면 Build 및 Run 설정을
할 수 있다. 또한 메뉴에서 [To아s] -o [Options] -. [Build & Run]나［Kits］를 실행하면 된다．

r    te;t orc - :e;t - Qt Creator

    Fl陌   Ed比   a山너     Debug           An키yze          自이5       Window            He巾
                                                                                                                      m
    We凡m ,        Bu妃 a: 日口ri                     Ed如r             Code Style                  De口endencies   ：區毒，n
      目
      Ed吐
                   Add Kit       !

                Manage K姑



（그림） B내Id & Run 화면



好 Qt 응용 어플리케이션 디버깅
Qt Cre毗아는 디버깅 키능을 지원한다. 현재 컴파일된 실행 바이너리를 GDB와 CDB를 사용해 어플리
케이션 디버깅이 가능하다. 메뉴에서 [Tools] - [Options] - [Debugger] 메뉴를 선택하면 GDB와
CDB를 설정할 수 있다．




22 CHAPTER 02_ 유용한 툴과 qmake


===== PAGE 24 =====
        iOptions                                N     口kd+}t二e



                                                                  Debugger
                                                                      3已n已r키 나므四-i크DC                 L口cc區 &Eap氾esiona
                                                                          Beha너or
          mEnvironment
          匿                 花났E由t아                                        回 Use 키也mnating ro니／ C이0四 in debug 너e叫S                                口Debugyerfoot !

          繇                 F如／im
                                                                          口 Use 切0川ps in main e비幻rwh扼 d아싸gging
                                                                          國 Close temporary buffers on debugger exit
                                                                                                                                                 國 Populate sourc
                                                                                                                                                 口 닯vitch to 口revi
                                                                          團 Bring （코 Creator to foreground 바hen a口베ca如ninterrupts                國 Sho叫 UML obj

          0
            8Help
                            c+   +
                                                                          明 마ea印曲ts ft川 path by default                                          回 Use Ut Crea加r
                                                                          Ma川mum s相ck de口th: 20            ｝취
              上4dQt Quick

           好                B」妃 帥Un
                                                                          Source Paths Mapping

                                                                           Source path      佃get path
                 斗          Debugger


（그림） Debugger 설정 화면




이외에도 Qt Cre毗야는 GUI 환경에서 디버깅 기능을 제공한다. Qt Creator의 [Debug] 메뉴에서 C++
기반 혹은 QML로 개발한 어플리케이션 디버깅을 위한 옵션을 실행한다．


    i山出                                                               !    X

        LeY甘 FUndmn                            1,1.              Lne
         U               T&E dm小脆dF4也tadm뱌 iL注1                                                                                                         Q1ntC나r1t1r
         1               1t+F+de, 1i)tF1nder   t的枷+ e,           52                                                                                     0k蚣＄0t1m
                                                                                 mPU1F뀨甘   n／呻吼口r                                                       51*
         2               5M.,                  n니m工m         7
                                                                                 h.        HQl         目m伯E51口01卜小1t化n1\ (0n노P却妃m四rted de. topner0 en   5모m因
                                               C丹＝aFfL六t恥工pp l3l
                                                                               >Th心        H TytFinde.' Oe22f.友1                                        kdFmder




                                                                               山山如帥m口月 心蘭資也屯Jr쁘 心咆브브


（그림） GUI 환경의 디버깅


디버깅을 시작하기 위해 圈를 실행하면 된다. 그리고 Qt Creator의 Break Poir此를 지정하기 위해 어］
디터의 라인에 마우스를 클릭하면 Break Point를 설정할 수 있다．




目黑뇨뇨r
（그림） 마eak P（기nt 지정 화면
                                                                                                엽盜                      "   '   " ",          Ignur      iaB
                                                                                                                                                         Ph           !
   Qt Cre毗야는 Debug 모드의 Short Key를 사용해 다음과 같은 디버깅을 지정할 수 있다．

         Short Key                                               설명
                  Sh附 + F5                                       디버깅 모드를 종료

         디0                                                      전체 코드에서 라인 단위로 실행

         Fl1                                                     코드상에서 함수 단위로 실행

         F5                                                      디버깅 모드를 실행

                     Shift + f        j                          가장 근접한 함수로 실행을 넘길 때 사용




                                                                                                                                                                          L유용한 툴과 qmake 23


===== PAGE 25 =====
 希 에디터 기능
 Qt Creator 에디터 기능은 내비게이션과 코드 에디터로 분류됩니다. 내비게이션은 헤더 파일, 소스 파
 일, 리소스 파일, 프로젝트 파일 및 프로젝트별 내비게이션을 제공한다. 내비게이션은 프로젝트
                                                     단위의
 트리 구조로 검색할 수 있다. 화면의 오른쪽은 직접 코드를 작성할 수 있는 에디터로써 C+＋과
                                                      QML
 (QtQuick) 코드를 에디터 할 수 있다．

 r.: connect由n.h - rejationaltablemodel · Qt C
        Ed作    Eu叱    Debug     Ana卜yze 自이S      WInS佃Y
                                                              connection h
                 f. reIaSionaItab!emode1
                   岫 r쉬ation키tablernoc旭 pro
                 1 j5 Headers                                 Eifndef      CONNECTION 珏
                        i, C:/QtJ才500/5 00/                   年define      CONNECTI（汁uSE
                           쓰j connection.h
                    a 500江e5                                  tiocci끄de <QMe므日aceB（그X>
                       tH r曲t口rc默ablemodeic                   tinclude <Qoqivetebase>
                                                              tiesolude <QSqltrror>J
                                                              tincicide <Q0qiQuery>

                                                    e9    d   / 山

                                                    三｛:             Thi日       bile      크efjr. e므    a   helper       func乞i口n   勺D    그C
                                                    51              in-   memory         SQLIn咆      cia乞abase     and    七0   Cr已自乞e   a
                                                    52
                                                    53              If    y口ii    Want     to u日e a1l0乞her da七abase.              simp
                                                    之心              hn ] m뇨1      九] ]   卜1m月 =＝긔r 스m11 ] Hr1 ; !1 卜k = =1 戶d; 竹＝n卜 八七1


（그림） 내비게이션과 에디터 영역



메뉴 바 하단에 에디터 툴바는 현재 위치한 소스 파일에 포함된 Symb아을 통하1 멤버변수와 멤버함수
                                                                                                                                             등
을 검색할 수 있다．


                                    ', QPushbutton
                                    더$ OTeotEd仕
                                                                                                                   舞
         ItiFndef DIALU百 14
         甘deFine DIALOC II
                                    qr [）帥四
                                        夕 吼checkJar꾜OBJECT山拍叩（D口not T &) 4
                                                                             恥
                                        甲 staticMetaObject: coost 마'10伯0바吼t
         Itinclude 促Diahiq>             夕 meta［가,ject() cane
                                       甲 qt.m日tacant(const char 女）
         QT_RECIH_NAMESPACE             伊 tr(const char.. canst char t = 먀
         class QAction;                夕 trU冊（C口not char 士. c500t char 士 = 0)
         class Qttialogttuttonttox;    夕 tr(caaot char 士. C（그not char *. jot)
         class QGroupBox;              夕 trUtftt(canst char 士. conot char t. jot)
         class QLabel;                 中  吼me伯C케（가aletaUb旭ct::CaII, jot. vajd 士十）
         class qline[dit;              伊 [)i帥］8).)
         class Q卜1enu;                唯 createMenut)
         class QMenuBar;               在 createHorjzontaIGrnuDBoo()
         class QPushttutton;           I툐 crea拍Grjdl카ouo日0虹）
         class Qlextfdit;              作  createFormGroupfloo()
         QT_END NANESPACE           日 營 anonymoas
                                         艀 蜘mGrjd日own

（그림） 에디터 툴바



메뉴 툴바 왼쪽에 위치한 口P} 日버튼은 현재 열려있는 파일의 Hi毗ory가 저장되어 이전 파일과 다음
파일로 이동할 수 있다. 현재 파일과 Symb이의 오른쪽 아래방향 화살표는 열려 있는 파일 목록 및 심볼
목록을 Dr아느Down 메뉴로 펼쳐진 상태에서 더블클릭하여 이동할 수 있다. 그리고 Split 기능을 이용하
면 Qt Creator 에디터를 여러 개로 나누어 여러 파일을 동시어］ 볼 수 있다．




24 CHAPTER 02_ 유용한 툴과 qmake


===== PAGE 26 =====
                                      rr七n b C.기abi      =, <S日已亡！ S   =    r그                                             C口nfl日C作그n h   甘 吃미0- b g




                                                                                            3456789          l23月
                                                                                     스
                       l
                                                   山出山古出斗＋山山出山山山 山山山山山山山出山山山山
                                                                                                                       essageBox: :critical    (0, qApp->t4
                                                                                                                         q스pp->tr ( "Una上）le 七（> e5七al그ii:
              0             11        ／出山＋
              1
              仕
              l
              4
              =
                                      tinclude <QtWidgets>                                                                          "This example needE=
                                                                                                                                    "the Qt SQL driver F
              2
                                      tin｛그ii上（le <（汁Sql>
              月
              느

                                                                                                                                    1' 七o build i七 = \ll\ ll11
              3




                                                                                                         니n口
              4
              +

                                                                                                                                    1'Click Cancel to e工
              4
                                      菲include " . . /connection. h"
              1
              仕

                                                                                                                       turn false;
              5
              J
              느




                                                                                            尸
                                                                                            匕 戶
                                                                                              b ／
              5




                                                                                                勺 戶
                                                                                                  b 少
                                                                                                    b 戶
                                                                                                      b 尸
                                                                                                        b
                            d void initializeModel                     (QSqlRela



                                                                                                              口
                                                                                                              1 小
                                                                                                                ／ m
              4
              m
              7                                                                            r
                                                                                           小
              J
              吐
              只
              H                        {
              4
              m
                                      II!       [0]                                                                    ery query;
                                                                                                                                                 table person (id   r
              q
              J
              r
              브
                                                m口del->setTable ( ' employee r                                         exec ( "create
                                                                                                                      F너


                                      C DCC河卄n, h                          1뇨回나 Svr的［巾                                                    「   L! nl브   드1   1L


           41                         tifndef          CONNEC땃ION 珏
           42
           唾 :3
                                      tdefine          CONNECTION H
                                                                                                                                                                    I
                                      tinclude          <QMes呂ag巳Box>


（그림） 에디터 Split 기능


작성한 코드를 함수 단위 혹은 丸r문과 같은 소스 코드의 영역을 I五ghlighting 기능과 특정 영역을 펼치
거나 감출 수 있다．

                            uoui Dia1og: :create目srizontalCroupBox()
                            {
                                horizuota]GroupBox - n 'n, gcraupl3ox(tr ( "uorizontal 1a(iout") );
                                QHBoxLa9out 'layout - new QH8oata3out;

                                             Fi比 (jet I = I; I < 卜IumuttOn朴 ++1) {
                                                 butt口ns(i} - new QPushButt卜n(tr ( "Button tl ') .arg(i                                       + 1) );
                                                 la如毗-)addvldgPt(button町ij) ;
                                             )
                                             加rizuntalCrou叩매->setLayout(1케PO以）;
! 立｝i                       }

隍                           //!              [7)

（그림） 에디터 F키ghlighting 기능




에디터 영역을 Highlighting 기능을 사용하기 위해서는 메뉴에서 [Tools] - [Options] - [Text
Edit야］H[Display] -. [Highlight blocks] 체크 박스를 활성화 하면 이 기능을 사용할 수 있다. 소스
코드 작성 시 문법（Synta功이 잘못된 부분을 자동으로 표기하는 기능과 잘못된 영역상어］ 마우스 포인터
를 위치하면 ToolTip을 이용해 문법이 잘못된 부분을 지적해 주는 기능을 제공한다．




   q1   3 45
                                 甘include <gApplication)




   14 4 4 4 4 岫 町 杵 的 印 더
                                 甘include "dialog小 "

                     日lot                     nain(int     argc, char 斗argu[ ])
                                 '1
                                              qApplication app (arqc,            argu)            -    ;    I
                                              Dialog Dialog J    ..                expectea token ; got app 1
                                              return dialog. execo;
                                 }

（그림） 문법 오류 검사




                                                                                                                                                                        L유용한 툴과 qmake 25


===== PAGE 27 =====
잘못된 문법을 지적해 주는 기능과 Semantic error와 warnii培을 표시하는 기능을 제공한다．

   'iii   //flinclude <OAnolication>
 . i1Z1   /／퓨lnC1U0e "a1a1oq.n"
   '43
   lou1 日 mnt nain(int argc. char .argu[ ])
   'uc    (
   J46          QApplication app(arac. arou) :
   i1/          pialoq dia1oq ;      'QADolication ' in not a tone name I
   '48          return dia1og.execQ;「' "
  149     }
 너51

（그림） Semantic error와 warning 표시



Symbols 상에서 본 여러 아이콘은 어떤 타입인지 표시를 함으로써 소스 코드의 가독성을 높여주므로 아
이콘이 가리키는 타입이 무엇인지 알아두면 유용하다．




      他團圄夕命슝夕命丘令
 아이콘               타입                                 아이콘         타입

                   클래스
                                                      r           슬롯（SLOT)
                   ENUM
                                                      出           P대VATE SLOT

                   ENUMERATOR(ENUM의 값)            」   亡           PROTECT SLOT
                   FUNC기ON                              9         C++ 키워드

                   다귀＼/ATE FUNC지ON                      0         C++ 코드 조각（snip四I)

                   PROTECT FUNC기이q                      n         QML element
                   VALUEABLE                            N         OME- 코드 조각（snip口et)

                   F캬귀VATE VALUEABLE                   口          매크로

                   PROTECT VALUEABLE                              네임스페이스
                                                        a.

                   시그널（SIGNAL)


헤더 파일의 소스 코드 파일로 이동할 때 圃를 이용하면 해당 소스 코드 파일로 이동한다. 그리고 소스
코드 파일 상에서 멤버함수나 멤버변수에 커서를 위치한 다음 ［鈿日＋區를 누르면 소스 파일상에 멤버변
수나 멤버함수가 위치한 라인으로 이동할 수 있다．



                    Of Assistant
Qt Assi毗ai此는 Qt API어］ 대한 HELP 문서뿐만 아니라 각 모듈의 예제 어플리케이션에 대한 설명도 포
함하고 있다. 그리고 키워드를 통해 도움말을 찾아볼 수 있다. 그리고 Qt Assistant는 Bookmark
                                                         기능
을 지원하며 자주 참조하는 문서를 따로 보관할 수 있으며 , index를 통해 찾고자 하는 도움말을 쉽고 빠
르게 찾을 수 있다．




26 CHAPTER 02_ 유용한 툴과 qmake


===== PAGE 28 =====
                                                                                                                         k=4：匣F1啣   '
nQt Assistant
    파딜（F)   편집（E)    보7115)    미듐（6)    책걀피（마      도움달（HI

     수 , <; ，命 1딥                 ，님 立＼ 斗（ 日丸 4
  내용 1잭한 L착갇피 1 찾기
 내욤                                    序 X    Active Qt
        AnISe at
    d St AS$latent Man나키
            Fuamples
         J 卜伯flu引                             그rs ActroeX and C（가너 su꺄｝U艮 계心邸S ：교C for             Conten始
    卜 dl Concurrent                           NIfldOWS den타야比mSt口
    C dl Core                                                                                       rArtic唯s and Guano
    ? St Do帥和or Manu키                               Access and use ActiveX contr이s and COM
    !}015,0 Relerence Documentation
                                                                                                    口Seterence
     > Qt6r히川ccl Ellen佃
                                                    objects provided by ary ActiYeX server in
                                                    their （거 ap미Cal山Cs                              出 Eram口lOs
    C Ut GUI
    H St He巾
     H St Image Formats
                                                     Make trmeirot applications available as
        Ut Unguist Manuel                            COM servers, 낚AIt any number old!
        St Mu出n祀비a                                   05呼Is and帥age始 as CO！내 obeC恕 and AC如end rontr아S.
        口I Network
        St 0pen0t
        0r Print Duppnrt                      For mate utormatton about using ACtIveX with at, see Building ActiveX somers iv Ot
      )0101a5
        St 口미ck                               Toe AChy以그ttramew아K cons好朽 Ott벼o mod네es
        （거 Sen口t
         Sr SQL
         St 056                                      Toe aArCont라net nodule Is a static library implementing aOblect and QWidget
        St Teal                                      subclasses QAnOb1ect and Q.eaWidget. teat act as containers tor COM Objects
         St Ut Ton匕                                  and AcliveX controls
         0r 빠abC汪

                                                                                                                   Am山
（그림） Qt Assistant 실행 화면



Qt Assi毗ar式의 왼쪽 메뉴는 각 모듈별 검색을 위한 내용 탭과 색인별 특정 단어를 사용해 해당 기능에
대한 HELP 문서를 찾을 수 있다. 책갈피 메뉴 탭은 자주 검색되는 HELP 메뉴를 즐겨찾기와 같이 등록
해 Bookmark할 수 있다．
/                                                                                                                        口   回
    nQt Assistant
     파밀（F)       편집（E)        보21(V)    미돔(a)       책랄피（B)        도움말（H)

       수 , d7 , 令 EJ                         ：勿 立L琶1 e1 C1
    I亘亘1 색민                 책칼피        찾기
     책갈피                                          5 x     QAxServer C++ C冶Sses
     필터 :

                                                         The           （그AXS斛＼er           Contents
              도구 모믐 메뉴                                   mod네e is a 小IlfldO나S
                  [:m：口re 5, 0: Sema먀町日s Exa                                                申 Class匕느
                                                          아가y static 比ra四 that
                  (-II山血k 5,0: Dl 0uick 0卜alL T-                                            中 Deta作ed Description
                                                          you can use to turn a
            密* 책걀피 메뉴
                                                          standard     ｛그I    Bin카＼r          + 니cense Intormat山n
                                                          Into a COM server
                                                          知tore



                        [     춘갼1 1냐竺也그 （긔asses


 （그림） （코 Assistant의 Bookmark 기능


                                                                                                                                                 변경하기
    Qt Assistant는 도움말에서 표시되는 폰트를 변경할 수 있다. Qt Assi毗ar此가 지정한 폰트를
    위해서 ［편집］H ［환경설정］메뉴를 선택하면 폰트를 변경할 수 있다．




                                                                                                                                        L유용한 툴과 qmake 27


===== PAGE 29 =====
                        글꼴 설정       브라무저
                i       口 사욤자 점의 설정 사욤


               d 문자j朴계
               사
                      （叫）
                        ！근F틔
                        날솰 솜듀（F) 1냘딤


               ] 스EF말 ) 쁘
                r
                            “S
                        글꼴 크기（F) 9
                              '
                         Aa4ZZ



                                               r否自二）i
（그림） 폰트 설정 화면




                                     Qt Designer Tool
             Qt Designer는 Qt에서 제공되는 컴포넌트나 사용자 정의 컴포넌트들을 배치 및 설계, 디자인하기 위해
             제공되는 툴이다. Qt Creator IDE 툴에서 통합된 형식으로 제공하지만 Qt Designer To아을 따로 실행
  할 수 있다．

 이 툴의 가장 큰 장점은 개발하려는 어플리케이션의 사용자 인터페이스（GUI)상에 위젯 혹은 컴포넌트들
을 마우스로 드래그하여 폼의 원하는 위치어］ 배치할 수 있다．

즉 하드 코딩 방법을 이용하여 폼에 위젯들을 배치하는 작업은 상당한 시간이 필요할 뿐만 아니라 직관적
으로 바로 확인할 수 없기 때문어］ 폼을 설계하거나 디자인하기 위해 많은 시간이 소요되지만 Qt Desig-
ner 툴을 이용하면 개발자의 수고를 덜 수 있다．



                                           3   ! i岫母 目 區i n] 目 k&   稍 器 斗目
             WI的et BOO
                                                                    06忙RI 出pact아
                                                                    OH忙＜I          Class
                         Layouts                                        rest F口rn} 勿 OW心蚌t
             名 Vertic켸 Ltylut                                           aogjot     口 QLineEd吐
             回I Horizontal LaW乂jt                                       aog pbl d Qpushwutson
                                                                        eng_Ibi    心 QLabel
降Grid너V어Jt
                                                                        cog_ Vt    社 （거ioekd仕
! 目 FortH Lay에t                                                         如rJhi      吟 gLobe'
1          Spa（七1묘  小

                                                                    Pnepetty beEBe
  - flOflzOntal Spacer
             iVertlcalSpacer                                        瑞讓巴                             '
                       Hobtons                                      Pr야始my        Va汕e
1回 Push Ru比0n                                                        ) 9e0ii1e... hO. 0). 40703001
汨e 化이 山tone                                                          口 듸eePOlicy (PrefomBd. Preforrod. 0. 01
巴 Radio autoon                                                       S mlnirnu.. 000
        1Check Box                                                   口 rnaxlmu. 167772150 06777215
       OCommand Link Button                                          口 듸1010cr.. 000
                                                                     5.00됴므幻7n n 보n
       프 But帥 帥X
        比前nV而而訂蘭5玉i蕩示ad)                                            0BSCURe ato匹er
  iList View
  1 3Tree View
                                                                      <resource motH
  捕 Tat놔eVie밖
［고 C伽Inn VIew
               t帥1W心p已上르쯔BOSOnJ
LI List Widget
* 3 Tree Widget
旴 -i      's끄如1毗                                                    Signal/Slot Editor Act,on Editor Resource Browser




（그림） Qt Designer Too 실행 화면


28 CHAPTER 02_ 유용한 툴과 qmake


                                                                                                                        1


===== PAGE 30 =====
그림에서 보는 것과 같이 오른쪽 부분의 \Uidget Box는 Qt에서 제공되는 위젯을 마우스로 드래그해 폼
어］ 배치할 수 있다. 오른쪽의 Object Inspector에서는 폼에 배치한 위젯을 선택하면 해당 위젯에 대한
속성을 변경할 수 있다. 속성에는 class명 , size, font, focus position 등 컴포넌트의 모든 속성을 변경
할 수 있다. Designer 툴어］ 대한 자세한 설명과 예제는 추후 단원에서 다룰 것이다．



（玉；4j叩ake
qmake는 Qt를 이용해 구현한 응용 어플리케이션 컴파일을 지원하기 위한 툴이다. Qt는 Linux/Un奴，
Windows, 八4ac OS X, Android 등 다양한 플랫폼에서 동일한 문법을 사용해 컴파일을 위한 과정을 쉽
게 할 수 있도록 지원하는 툴이다．

예를 들어 리눅스 플랫폼에서 gcc와 같은 툴을 이용해 응용 어플리케이션을 컴파일 할 때 소스 파일이 여
러 개 혹은 수십 개로 작성되고 또한 Qt 이외에 다른 라이브러리를 사용할 때 gcc를 이용해 컴파일 한다
면 복잡한 구조의 makefile을 작성해야 한다. 하지만 qmake를 이용하면 makefile 작성을 하지 않고도
qmake를 이용해 쉽게 n追kefile을 작성해 준다. 다음과 같이 소스 파일이 있다고 가정해 보자．

  1addressbook.h
  ·addressbook. cpp
  1main. cpp

위와 같이 Qt로 작성된 소스 파일이 위치한 해당 디렉토리로 이동해 qmake 파일을 실행하면 확장자가
.pro 파일인 프로젝트 파일이 생성된다. qmake를 이용해 프로젝트 파일（.pr이을 생성하기 위해 소스가
위치한 디렉토리어］ 위치한 다음 다음과 같이 터미널상에 입력하면 된다．

! 1느＼Q七5\usefule\ ad（뇨ess>
                               qmake   -projec七
                                                                       그
qmake 실행 파일은 Qt가 설치된 하위 디렉토리인 bin 디렉토리에 위치해 있다. 만약 이 디렉토리
PATH가 설정되어 있지 않다면 qmake 실행 파일을 찾을 수 없을 것이다．

 5.02
 上 MSVC 2010
    따 A鄒始nt
    旴 Designer
    寸 Linguist
    四Qt5쇼2幻rDesk啣（MSVC 2010)
匕IsSrn忙h
 eK卜4F기ayer
 tal Commander

       뒤로




（그림） Qt 터미널 실행 화면




                                                         L유용한 툴과 qmake 29


===== PAGE 31 =====
         명령 프롬프트에서 qmake를 실행하기 위해서 Qt를 설치하면 관리자 설정 명령 프롬프트가 있다. 이 명
         령 프롬프트에서 다음과 같이 qmake를 실행한다．

           四 단크 二 :/ 三 =
            目13니日5-14               노 "슨 I目：羽   <DIR>
            日13 日5-14               오전 I日：3目    <DI丑）
            013 目5中日3               오전 11：  日8           乳81王 addressbook.cpp
          i日13-05-日3                오전 11：目8             二428 a山lresshi乂｝k , 11
          i日13놔05 日3                오전 11＝日8             2.285 main.cpp
          I                             3가1 파일              ?.524 바이트
          I                            2) H 디렉터리 87. 965 .6日9.984 바이트 남옴

          1：
               的比吼：
                              吐. iRaddress >qma如                Proj毗
          1
          1 ＝竹Qt5卄Useful卄address >dir
          ID 드라이브의 볼흄어는 이릍이 없．습니다．
          1 볼튬 일련 번호： 6A16小7DA2
          1
          ID：出Qt5楙朽.fu1呻addres: 디렉El리
          1
         ！日13-05叫14                오전 10:35                 .
         ！日13-05-14                오전 :1日：35 <DIR>
         ！日13中日5-14                오전 I日：35             3크5 a1dress.pro
         1目13 日5-日3                오전 11:08           2.811 addressbook.cpp
         ！目13卄日5尸03                오전 11:08           2.428 addressbool.h
         p013-日5-03                2전 11:08           2.285 nain.cpp
         I                           4가1 파일              7.859 바이트
         I                           2)H 디렉터리 87. 965 .6日9.984 바이트 남믐

          II                亡．.f , , ]1小二‘1a, .n交 , 노



         （그림） qmake 실행 화면



         qmake로 생성된 프로젝트 파일（.pr이의 내용은 다음과 같다．

          TEMPLATE = app
          TARGET = address
          INCLUDEPATH +=


         孝 Input
         HEADERS += addressbook.h
          SOURCES += addressbook.cpp main.cpp



         HEADERS 키워드는 소스 헤더 파일을 명시하고 SOURCE 키워드에서는 소스 파일을 명시하면 된다．
         TARGET 이름은 자동으로 설정되는 실행 파일명이며 , 프로젝트 파일명과 동일하다. TARGET에서 정해
         진 이름이 어플리케이션 컴파일 후 실행 바이너리 파일명이 된다. 예를 들어 윈도우 플랫폼에서 address
         .exe 명으로 실행 파일이 지정된다．

     qmake로 생성한 프로젝트 파일（.pro）을 이용해 八4akefile을 생성하기 위해서는 다음과 같이 명령을 프
  롬프트 상어］ 실행한다．

         qmake -o Makef lie                             address.pro


만약 \Tjsual Studio를 사용한다면 다음과 같이 사용한다．

!qmake
                      -tp
                                   vc address.            pro
30 CHAPTER 02_ 유용한 둘과 qmake


===== PAGE 32 =====
     簪 디버깅 모드
Qt로 구현한 응용 어플리케이션이 Release 버전인 경우 디버깅 Symb아5가 포함되지 않는다. 만약 어플
리케이션 개발 시 디버깅 버전으로 컴파일 하기 위해서 프로젝트 파일에 다음과 같이 디버깅을 지정한다．

!CONFIG += debua
!HEADERS += aclciressbooic. fl
! SOURCES += aciclressbooic.cpp
三 SOURCES += main.cpp
\




     黎 특정 플랫폼에 소스 포함시키기
Qt는 다수의 플랫폼을 인식한다. 따라서 특정 플랫폼에서 지정한 소스 파일을 컴파일에 포함시키기 위해
다음과 같이 사용할 수 있다．

     win32 {
!,             " " '『   ' " 缸' " ' 岫   "" ' "   ' ""




만약 Unix/Linux와 같은 플랫폼에서 특정 옵션 및 소스 파일을 지정하기 위해 다음과 같이 사용한다．

     win32 {
         SOURCES += addressbookWin.cpp
     }
     Unix {
         SOURCES += addressbookUnix.cpp
     }


     簪 특정 파일이 존재하지 않는 경우
     qmake는 Makefile을 동작하기 전에 특정 소스 파일이 존재하지 않는지 다음과 같은 옵션을 사용한다．
만약 지정한 파일이 존재하지 않는다면 八'lakefile을 생성하지 않는다．

     CONFIG += debug
     HEADERS += addressbook.h
     SOURCES += addressbook.cpp
     SOURCES += main.cpp
     win32 {
         SOURCES += addressbookWin.cpp


     Unix {
         SOURCES += addressbookUnix.cpp
     }
     !exists ( main.cpp ) {
         error ( "No main. cpp file             found"   )




                                                             1 유용한 툴과 qmake 31


===== PAGE 33 =====
/＼八2VH乙）


===== PAGE 34 =====
 CHAPTER




GUI 설계와 제작


===== PAGE 35 =====
Qt 5 Programming




f               1 Basic Widget
                이번 장에서 배울 내용은 어플리케이션 GUI 인터페이스를 개발하기 위해 필요한 위젯에 대해 알아보도
                록 하자. 위젯은 데이터 및 정보를 표시하고 어플리케이션 사용자로부터 입력을 받을 수 있다．




QOr。u08。  x -     Appointment Detads
parent wIdget                                              O0針eEdit
                                                           야ii町 似dget
                                                            limeEdit
                                                           child widget
OLabel                                                     OLinehdil
child w!dgets                                              child widget
                  Developer meeting
                  A brief meeting to check the status
                  of each project in the development
                  department
OTextEdd
child 나dget




（그림） 위젯과 레이아웃


위젯을 배치할 때, setGeometry( ) 멤버함수를 사용할 수 있다. 이 방법은 윈도우 창의 크기가 변경되더
라도 위젯의 위치와 크기가 변경되지 않는 단점이 있다．
위젯을 배치할 때 , 레이아웃을 사용하면 윈도우 창이 변할 때, 동적으로 위젯의 크기를 변경하거나 배치
할 수 있다. 레이아웃은 다음 장에서 다룰 예정이다．


           One                                          One        1
                  Three                                 Two        1
                             티ye                        Three      I      I
（그림） 레이아웃




 사용할 위젯은 QStyle 클래스를 사용해 위젯의 스타일을 변경할 수 있다. 예를 들어 윈도우 혹은 리눅스
 Os의 테마를 변경함으로써 전체적인 스타일을 변경할 수 있는 것처럼 어플리케이션상어］ QStyle을 사용
 해 전체 UI 스타일로 변경할 수 있다．


 34 CHAF汗ER 03_ GUI 설계와 제작


===== PAGE 36 =====
                                                            昱t냇es            Mar                                                fStyles

                                                            O Heading                                                        Q Heading
                                                            t孕 earagraph                                                     8Paragraph
                                                                                                                             Q List
                                                            (：그 List                                                         Q Footnote
                                                            （乙 印otnote



（그림） Os'니e을 이용한 UI 스타일 변경



QStyle은 기본으로 제공하는 스타일 이외에 사용자가 직접 UI의 스타일을 커스터마이징 할 수 있는 메
커니즘을 제공한다. 커스터마이징을 하기 위해 Qt Style Sheet를 사용하며 , 이 방법은 HTML Cas
cading Style Sheet(CSS）를 사용해 위젯에 척용할 수 있다. 예를 들어 QLineEdit와 QCheckBox,
QPushButton 위젯에 CSS를 적용하는 방법은 다음과 같다．


}QLineEdit { background:                       yellow           }
iQCheckBox { color: red  }

    QPushButton *btn = new QPushButton( "Click! ", this) ;


    btn->setStyleSheet ( "background-image: url ( : /img/ a.png) ;\n "
           "font-weight: 600; \n border: opx; color:white; text-align:center; ") ;



                                                                                                      Style Slonnt
                                                                       肛            (51

                                                                                     N카Re    A미sander

            Nmm:                                        니                          Gender:    Male        Female
            Ama甘： Cl 汁虹 r       Fan出단
                                                                                      Age    2S
              Age:   25
                                                                              Pass나아d
       Pa$$VY아d.

                                                                                   Country   France
        C아mbY;       다aKe

      Pro他5듸on:       yV甘耳）g
                                                                             Profess山n       Des딥야乂r
                     :554口才                                                                  Studrnt
                     日sherman                                                                FaIre 나nrc




                                                                             口 I acce口tthe tern恬 and cond:trons
      口 I acne口'5袒 납yes and C마,dboes
                                                                                                               Cancel   OK
                                        c(   Cancel


    Ready                                                                  Ready
/



（그림） Windows XP 스타일과 Mac O5 x 스타일



위젯, 레이아웃 더불어 위젯에 적용할 수 있는 Qt Style어］ 대해 간단히 알아보았다. 이외에 사용자가 직
접 UI 스타일과 기능을 적용한 커스텀（Custom) 위젯을 만들 수 있으며 커스텀 위젯을 다루는 것은 추후
다른 단원에서 다루도록 하겠다．

다음 표를 참고해1 어플리케이션 개발에 활용하면 유용하다. Qt에서 제공하는 위젯은 QCheckBox,
QPushButton 등과 QListView, QCalendarWidget과 같은 고급위젯, QButtonGroup, QGroupBox


                                                                                                                                          1_Basic Widget 35


===== PAGE 37 =====
와 같은 동일한 속성의 집합 형태와 같은 위젯 그리고 추상화 위젯으로 분류할 수 있다．

Basic Widget
Button, Combo Box, Scr에과 같이 직접 사용할 수 있는 Widget

QCheckBox            체크박스 위젯（Text Label 포함）
QComboBox            버튼을 클릭하면 팝업리스 중 하나를 선택
QCommandLinkButton   쌔ndows Vista 스타일 Command 링크 버튼
Q기meEdit             QTime巨dit 위젯 상에서 Date를 편집하거나 표시하71 위한 위젯
ODateEdit            QDateEd仕 위젯 상에서 Da也를 편집하거나 표시하71 위한 위젯
0먀射eTimeEdit         Date와 기me을 편집하거나 표시하71 위한 위젯
ODial                원형 스타일의 니를 제공하며 범위를 지정하는 데 사용
OSpinBox             스핀박스 위젯
QDoubleSpinBox       Doub冶 데이터 타입을 사용할 수 있는 Spin B（그x
QPushButton          일반적인 버튼 위젯
QFocusFrame          위젯의 Painter 영역 바깥쪽 영역을 지원하는 프레임
QFon兀omb旺幻x          선택한 폰트를 사용할 수 있는 Combo Box 위젯
QLCDNumber           미야al LCD 스타일의 숫자를 표시하기 위한 위젯
OLabel               텍스트 혹은 이미지를 표시하기 위한 위젯
（긔JneEdit            Sin이e Line 텍스트박스 위젯
OMenu                Menu Bar에서 사용하기 위한 Menu 위젯, Context 그리고 팝업 메뉴에서 사용할 수 있는 위젯
QProgressBar         Horizontal 혹은 vertical Progress Bar
QRadioButton         라디오 버튼 위젯（Text Label 포함）
QScr에Area            다른 위젯의 니ew 상에 Add-on 할 수 있는 스크롤 위젯
QScr에Bar             Vertical 혹은 horizontal Scroll Bar
QSizeGri口            T야） Leve 윈도우 크기를 변경하기 위한 핸들링
QSlider              Vertical 혹은 horizontal slider
OTabBar              Tab Bar 위젯（탭 다이얼로그에서 사용하기 위한 위젯）
oTabWidget           Tab 위젯
OTo이Box              C이umn 형태로 된 탭 위젯
OToolButton          OToolBox 위젯 안에서 사용되며 옵션이나 명령에 기반과 같이 빠른 접근을 제공하71 위한 버튼 위젯
OWidget              모든 0b忙아의 Base 이ass



아ganizer 빠dget
S아tter, Tab Bar, Button Grou口 등과 같이 Grou口Ing된 위젯


                                        Package selection
 好 Hea凶nq
 唾 Paraga的                               團 U口date systeri
｛雙年Li呂t
                                         ,H U口date a口口hcatons
的 Fc'olr꺾攷e
                                         [：二 U口date（把currentation




36 CHAPTER 03_ GUI 설계와 제작


===== PAGE 38 =====
    OButtonGr（그U口                             버튼 위젯 집합 Container
    OGroupBox                                 Title을 표시할 수 있는 (3rou口 Box 다ame
    Os이附er                                    Splitter 기능을 구현한 위젯
    OSplitterHandle                           햐케tter 기능을 제어하기 위한 위젯
    OStacked Widget                           하나의 위젯이 아닌 여러 개의 위젯을 스크린상에 동시에 표시하기 위한 기능을 제공하는
                                              위젯
    QTabWidget                                Tab 위젯




    Abstract Widget Class
    위젯의 Base C冶ss이며. 예를 들어 QPush日utton은 QAbstra이But幻n으로부터 상속받은 Sub （긔ass를 사용

    QAbstractButton                            일반적인 버튼의 기능을 제공하기 위한 추상화 클래스
    QAbstractScrol lArea                       Scr에 Bar에서 필요한 기능을 제공하는 추상화 클래스
    QAbstra아테der                               정해진 범위 내의 nteger 값을 사용하71 위하1 제공하는 추상화 클래스
    QAbstract5pinBox                           Spinbox와 Line 탸川에서 값을 표시하기 위한 추상화 클래스
    oDialog                                    ［거alog 때ndows의 Base （기ass
（가가ame                                         프레임을 내장할 수 있는 기능을 제공하는 Base Class




    ：上』l. 1, QCheckBox F QButtonGroup
Qt에서 제공하는 QCheckBox 위젯의 특징은 여러 항목을 선택할 수 있는 유저 인터페이스를 제공한다．

    #include <QCheckBox>



QCheckBox는 스위치와 같이 Check(On) 혹은 Un Check(off）된 두 가지 중 하나를 선택할 수 있다．
첫 번째 인자는 체크박스 항목 텍스트이다. 두 번짜1 인자는 부모 클래스를 선언할 수 있다．

i
         ckBox   *chk   =   new   QCheckBox            (   "P&
                                                                 rogramming " ,   this) ;



    " & " 문자는 체크박스의 Short-Cu仄단축키）을 사용할 수 있으며 , 단축키는 區 +［亘를 누르면 체크박스
를 활성화 혹은 비활성화 시킬 수 있다．
어플리케이션 상에서 체크박스를 사용할 때, 여러 그룹으로 분리할 때, QButtonGroup을 사용하면 그룹
으로 분리할 수 있다．

    QButtonGroup * group = new QButtonGroup( this) ;



첫 번째 인자는 부모 클래스를 지정한다. QButtonGroup 클래스에 구현된 addButton( ) 멤버함수를
이용해1 체크박스를 그룹에 포함시킬 수 있다．

체크박스의 특징은 여러 항목 중 다중 선택할 수 있는 특징이 있지만 QButtonGroup 클래스의 set-
Exclusive( ) 함수를 사용하면 단일 항목만 선택할 수 있도록 체크박스의 성질을 변경할 수 있다．


                                                                                            1_Basic Widget 37


===== PAGE 39 =====
QString strl[ 3] = {"Game ", "Office", "Develop"} ;
QString str2[ 3] = {"P&rogramming ", "Q&t ", "O&S "} ;


 mnt xpos = 30;
 mnt ypos = 30;


 chk_group[ 0] = new QButtonGroup (this) ;
 chk.mgroup[ 1] = new QButtonGroup (this) ;


 for (int i = 0 ; i < 3 ; i++)
 {
      exclusive[ i] = new QCheckBox(strl[ i] , this) ;
      exclusive[ i] ->setGeometry (xpos, ypos, 100, 30) ;
     Vchk_group [ 0］巾＞addBu七七on ( excli坮ive[ i] ); I/ 첫 번째 그룹

      non exclusive[ i] = new QCheckBox (str2[ i] , this) ;
      non exclusive[ i] ->setGeometry (xpos + 120, ypos, 100, 30) ;
     ＼厄hk_group [ 1] ->addBu七七on(exclusive[ i] ); // 두 번째 그룹

       connect (exclusive[ i] , SIGNAL (clicked() ), this,
                                SLOT (chkChanged() ) );
       ypos += 40;
 }
 chk group[ 0] ->setExclusive (false) ;
 chk group[ 1] ->setExciusive (true) ;




=


     口淆誦百i        口마四ramming

     [:：그0州ce     ［그 [:)t

     ［그 0ev미0口    口 0旦



（그림） QCheckBox


 exclusive[ i] = new QCheckBox(strl[ ij, this) ;
 exclusive[ i] ->setGeometry (xpos, ypos, 100, 30) ;
 chk_group[ 0] ->addButton(exclusive[ i] );


QCheckBox 첫 번째 인자는 체크박스의 텍스트를 선언하고 두 번째 인자는 부모 위젯을 선언할 수 있
다. 세 번째 라인은 체크 박스를 포함할 그룹을 지정하였다. 그룹으로 지정했기 때문어］ Programming,
Qt, OS 체크박스의 선택에는 영향을 주지 않는다．

Game, Office, Develop는 첫 번째 그룹으로 분리하고 Programming, Qt, OS는 두 번째 그룹으로 분리
했다. 첫 번째 그룹의 특징은 하나만 선택할 수 있도록 했고, 두 번째 그룹은 하나 이상을 선택할 수 있다．


38 CHAPTER 03_ GUI 설계와 제작


===== PAGE 40 =====
 chkmgroup [0] ->setExclusive (false) ;
 ch卞느group[ l] ->se七Exclusive ( 七rue) ;



어플리케이션상에서 체크박스가 사용자에 의해 활성화 되거나 비활성화 될 때1, connect( ) 함수를 사용
해 확인할 수 있다．

 connect (exclusive[ i] , SIGNAL(clickedO) , this,        SLOT (chkChangedQ) );


첫 번째 그룹의 체크박스가 선택되거나 비활성화 되면 슬롯（SL0T) 함수에 연결된 멤버함수인 chk나
Changed( ) 함수가 실행한다．

1void Widget: :chkChanged()
 {
      for (int i        = 0 ; i < 3 ; i++)
      {
            if (exclusive[ i] ->checkState ( ))
            {
                    qDebug ( "checkbox %d selected ", i+ l) ;
            }
       }
 }

checkState( ) 함수는 체크박스가 활성화 되어 있으면 TRUE , 그렇지 않으면 FALSE를 리턴한다．
QCheckBox는 텍스트가 위치한 곳에 이미지를 사용할 수 있다. 이미지 리소스 파일을 QCheckBox 위
젯에서 사용하기 위해서 QAbstractButton 클래스로부터 상속받은 setlcon( ) 멤버함수를 사용하면
QCheckBox 위젯에 이미지를 사용할 수 있다．

 exclusive[ O] ->setlcon(Qlcon( "resources/browser.png") );
 exclusive[ l] ->setlcon(Q工con ( "resources/calendar.png") );
 exclusive[ 2] ->setlcon(Qlcon( "resources/chat.png") );


 non1exclusive[ 0] ->setlcon(Qlcon( "resources/editor. png") );
 non exclusive[ l] ->setlcon(Qlcon( "resources/mail.png") );
 non_exclusive[ 2 }->setlcon (Qlcon ( 'resources/users .png") );



 =                                口回因

     匣] \d Game     :   ［그 ;．마0아ammi

     ［그 互 0州C日           回   01

     ［그    Dcv미0口       ［그 七 0昱



（그림） 아이콘을 사용한 QCheckB（그x




                                                                                  1_Basic Widget 39


===== PAGE 41 =====
 (1i.
               i I QComboBox
 사용자가 위젯을 클릭하면 팝업메뉴가 나타나고 등록된 항목 중 하나를 선택할 수 있는 GUI 인터페이스
 를 제공한다．

        헤더 파일 : 孝include <QComboBox>


 QComboBox 위젯상어］ 아이템을 등록하기 위해 텍스트를 사용해 아이템을 등록하거나 이미지와 텍스트
를 같이 사용할 수 있다．

        口 OComboBox




              尸1正dn：刊口口




（그림） QComboBox



                 new QC（丑的出아이thi引 ;
                 etGeometry (50, 50, 200, 30) ;



        combo->addltem( "Application") ;
        combo->addltem( "Graphics ") ;
        combo->addltem( "Database") ;
        cornbo->addltem( "Network ") ;


addltem( ) 함수는 QComboBox 상에 아이템을 등록할 때 사용한다. 아이템상에 아이콘을 사용하기 위
해서는 오버라이딩된 addltem( ) 함수를 다음과 같이 사용할 수 있다．

됴In加如毗帥陣的川螂毗呻伽呻er.                        png") , "Applic.七io可，);
con由o->addltem(Qlcon( "resources/ calendar.png") , "Graphics ") ;




                                                  \Y6rphics
                                                  Databas（크
                                                  Network
（그림） QCombo8ox 이미지 사용




40 CHAPTER 03_ GUI 설계와 제작


===== PAGE 42 =====
QComboBox는 아이템이 변경될 때 , 선택한 아이템의 Index를 리턴하는 시그널을 제공한다．

         combo, SIGNAL (currentlndexChanged(int) ), this,
                        SLOT (valueChanged() ));


currentlndex（그hanged(int) 시그널 함수를 사용하면 아이템이 변경되었을 때 , 변경된 아이템 Index를
리턴한다．

void Widget: :valueChanged()
{
     mnt current_index = combo->currentlndexU;
     qDebug ( "Current ComboBox index : %d", current index) ;




사용자가 선택한 아이템 Index를 받기 위해서는 currentlndex( ) 멤버함수를 사용하면 현재 Combo
Box 위젯의 선택된 아이템 인덱스를 리턴한다．

등록된 아이템의 Index를 이용해 아이템을 삭제하거나 전체 아이템 개수를 리턴함수를 제공한다. 그리
고 Index 이외에 선택한 아이템에 대한 텍스트를 리턴하는 멤버함수가 제공된다．

QString str;
str = con幻o->curren七Tex七（) ;


qDebug( "Total Items ", coinbo->count () );
combo->removeltem( 3)




    t1.3, QCommandLinkButton
이 위젯은 QPushButton 위젯과 동일한 기능을 제공하는 위젯이다. 특징으로 이 위젯은 MS Windows
에서 제공하는 Link B毗ton과 같은 스타일을 제공한다．

헤더 파일： 半ii兀lude <QComman（江inkBu七七on>
                                                                                          j
버튼에 표시할 텍스를 입력하고 두 번째 인자인 Description을 추가하면 다음 그림과 같이 버튼 아래에
Description이 표시된다．

cinrnBtn = new gCommandLinkButton( "Vision'1 ,
                                     n＼八到On Projec七" r
                                     七hi引 ;

connect (cinmBtn, SIGNAL(clicked(fl,    this,    SLOT (clickFunc () ));




                                                                          1_Basic Widget 41


===== PAGE 43 =====
     Vision
     Vision Pr미日Ct




（그림） QCommandLinkButton



두 번째 인자의 Description을 사용하지 않길 원한다면 다음과 같이 오버라이딩된 생성자 함수를 사용
할 수 있다．

 QCommandLinkButton: :QComrnandLinkButton ( const QString & text, QWidget * parent = 0


QCommandLinkButton 위젯은 QPushBu仇on 부모 클래스로부터 상속받아 구현된 위젯이다. 따라서
QPushButton 위젯 클래스에서 구현된 함수를 사용할 수 있다．

                                                              小
                                                              艸
             QDa也 클래스와 QDateEdit 위젯
                                                              打
                                                              口
QDateEdit는 날짜를 표시하거나 변경할 수 있는 GUI 인터페이스를 제공한다. QDateEdit는 QDate 클
래스로부터 제공하는 기능을 이용해 날짜를 표시할 수 있다. QDate 클래스는 년, 월, 일을 표시하기 위
해 제공되는 클래스이며 , 날짜를 표시하기 위한 함수 이외에도 날짜를 계산식을 이용해 변경할 수 있는
다양한 멤버함수를 제공한다．

 헤더 파일 :
 判nc1ude <QDa七e>
 孝include <QDateEdi七＞



QDate의 생성자 함수는 년, 월, 일을 지정하거나 현재 시간을 시스템 시간으로부터 얻어와 QDateEdit
위젯어］ 연결해 표시할 수 있다．

 QDate dtl = QDate (2013, 11, 7) ;
 QDate dt2 = QDate: :currentDate ( );
 da七eEdi七［0] = new QDa七eEdi七（
                            （蛇l. addYears (2) r 七his) ;
 da七eEdi土［0] ->se七（把帥e七ry(10, 10, 140, 40) ;
 da七eEdi七［1] = new QDa七eEdit ( dtl . addNon七hs (3) r 七hi引 ;
 dateEdit[ 1] ->setGeometry (160, 10, 140, 40) ;
 dateEdit[ 2] = new QDateEdit (dtl .addDays ( 10) , this) ;
 dateEdit[ 2] ->setGeometry (310, 10, 140, 40) ;
 da七eEdj土［3] = new QDa七eEdi七（dt2, thi引 ;
 dateEdit[ 3] ->setGeometry(10, 60, 140, 40) ;




42   CHAPTER 03_ GUI 설계와 제작


===== PAGE 44 =====
（그림） ODate와 QDateEd仕롤 이용한 날짜 표시



QDate 클래스는 날짜를 얻어오거나 요일의 Index를 리턴하는 멤버함수를 이용해 현재 설정된 날짜의
요일이 무슨 요일인지 알 수 있는 멤버함수를 제공한다．

i // 1：월r 2：화 ' 3：수' 4：목 ' 5：금, 6：토 ' 7：일
  switch(dt2. dayOfWeek () )
 {
 case 1:
     qDebug ( "卜幻nday ' ) ;
     break;
 case 2:
     qDebug ( " Tuesday ") ;
     break;
 case 3:
     qDebug ( "Wednesday " ) ;
     break;
 case 4:
     qDebug ( " Thursday ") ;
     break;
 case 5:
     qDebug ( " Friday " ) ;
     break;
 case 6:
     qDebug ( "Saturday ") ;
     break;
 case 7:
     qDebug ( "Sunday ") ;
     break;




 dtl 인스턴스어］ 설정된 날짜에서 그 해로부터 며칠이 지났는지 알기 위해 day아'Year( ) 멤버변수를 사
 용하면 지난 날짜를 m1lt로 리턴한다. 비슷한 멤버함수로 설정한 날짜의 해당 월의 마지막 일이 며칠인지，
 해당 년에 마지막 일은 며칠까지 있는지 다음과 같은 멤버함수를 이용하면 결과를 얻을 수 있다．

 qDebug( "Day of year : %d", dtl. dayOfYear (fl;
 qDebug ( "End Day : %d", dtl. dayslnMonth (fl;
 qDebug ( "End Day : %d", dtl. dayslnYearQ) ;




                                                    1_Ba듸C ＼八／idget 43


===== PAGE 45 =====
 QDate 클래스는 설정한 날짜를 표시하기 위한 방법으로 QString 데이터 타입을 리턴하는 멤버함수를
 이용하면 날짜를 다양하게 표현할 수 있다．

 Expression          Output
 d                   卜31 표시 (1'- '31)
 dd              , 1"31 표시하되 2자리로 표시 (01-'-31)
 ddd                 3자리 문자로 요일을 표시 (Mon N Sun)
 dddd                완전한 문자로 요일을 표시 （卜加nday N Sunday)
 M                   ]Nj2 숫자로 표시 (]N但）
                 a




 MM                  卜］2 숫자로 표시하되 2자리로 표시 (01'-'-'但）
 MMM                 월을 3자리 문자로 표시 (Jan N Dec)
 MMMM                월을 완전한 문자로 표시 (January " December)
 yy                  년을 2자리로 표시 (00,-,99)
 yyyy            ! 년을 4자리로 표시 (2002)




 QDate dt3 = QDate: :fromString ( "2002. 06. 26 ",             "yyyy.MM.dd ") ;
 QDate dt4 = QDate: :fromString ( "06. 26 ",              "MM.dd") ;

 lbl[ 0] = new QLabel (dt3.toString() , this) ;
 lbl[ 0] ->setGeometry(10,110, 150, 30) ;
 1b1[1] = new QLabel (dt4.toString( ), this) ;
 lbl[ 1] ->setGeometry (10,150, 150, 30) ;




                                                 드：j回匡1
 喇t0키 07               a기4 꾜 n7   三珽難恁2미＋11-17


     2013-0卜］4


  수 6262匹0


  화 5 26 円［10



（그림） QDate::fromStrin（그



QDate로 설정한 날짜가 유효한 날짜인지 확인하기 위해 isValid( ) 멤버함수를 이용할 수 있다．

 if (QDate: :isValid (2011, 6, 27) )
 {
          qDebug ( "2013. 6. 27 true") ; II       2013. 6. 27 true
 }
 else
 {
          qDebug( "2013. 6. 27 false") ; II        2013. 6.27 false
 }




44 CHAPTER 03_ GU 설계와 제작


===== PAGE 46 =====
요일을 표시하기 위해 dayOfWeek( ) 함수는 요일을 h7까지 숫자로 리턴한다. 이 함수로 받은 리턴값
을 QString 타입의 문자열로 리턴받기 위해서 longDayName( ) 멤버함수를 이용하면 요일을 문자로 리
턴 받을 수 있다．

이와 비슷한 멤버함수로 101培MonthName( ) 멤버함수를 이용하면 숫자로 표시된 월을 완전한 문자로
리턴 받을 수 있다．

완전한 문자열 이외에 짧은 문자열로 리턴하는 멤버함수로써 shortDayName( ）와 shortMonth
Name( ) 멤버함수를 제공한다．

QDate dt5 = QDate (2012, 4, 26) ;


 QString LongWeek = dt5 . longDayNaine (dt5 .dayOfWeek () );
 QString LongMonth = dt5 . longMonthName (dt5 .month() );
 QString strDateLong = QString( "%l                 %21' ) .arg(LongWeek) .arg(LongMonth) ;


 QString ShortWeek = dt5 . shortDayName (dt5 .dayOfWeek (fl;
 OString ShortMonth = dt5. shortMonthName(dt5 .nionth() );
 QString strDateShort = QString( "% l                %21' ) . arg(ShortWeek) . arg(ShortMonth) ;



 lbl[ 2] = new QLabel(QString( "Long: %1 , Short : %2 ") .arg(strDateLong)
                                                      .arg(strDateShort) , this) ;
 lbl[ 2] ->setGeoinetry (10,190, 250, 30) ;




                 A                 A
  ':lI3니卜0긔           2O12니J2니J0       2011-11-17
                 기r                Y




                 1
 nn1 극 01-14
                 Y




 수 525 252

 화 626 四00


 Long: 목a밀 4퓔 . Shorl 목 4



（그림） 문자열 날짜 표시



날짜를 다루는 QDate 클래스는 표시하는 스타일을 표현하는 표준 타입을 변경할 수 있다．

 Enum                                  Va山e            Descri口t泊n
（가：:Te川Date                            0               디폴트 타입 표시
Qt::ISODa也                             ]               1SO860] 확장된 포맷으로 표시
Qt::SystemLocateDate                                   국가의 표현 방식으로 표시




                                                                                                   1_Basic Widget 45


===== PAGE 47 =====
! QDate dt6 = QDate (2012, 7, 26) ;
    lbl[ 3] = new QLabel(dt6 .toString (Qt: :TextDate) , thi引 ;
    ibi [3] ->setGeometry (10, 240, 250, 30) ;


    lbl[ 4] = new QLabel(dt6 .toString (Qt: :ISODate) , this) ;
    lbl[ 4卜>setGeometry(10, 270, 250, 30) ;


    ibi [5] = new QLabel(dt6．七OS七ring (Q七：: SysteinLocaleDa七e) / 七hi引 ;
    lbl[ 5] ->setGeometry (10, 300, 250, 30) ;



                                                         口回因

                                       m的小目口
    201크-11-07            2012-02-37


    加14니기 니 4


    수 020 2[}D2


    화 6261丑｝0


    L口no 목8밀 4뉠 , Oh口rt ; 목 4




（그림） 날짜 표시 표준 타입




    寸Li百jQ기me 클래스와 QTimeEd什 위젯
QTime 클래스는 시간을 hour, minutes, seconds, millisecond로 처리할 수 있는 기능을 제공한다．
현재 시스템 설정 시간과 현재 시간으로부터 특정 시간까지의 경과 시간을 표시하거나 시간을 비교하는
등 어플리케이션 개발에 필요한 다양한 시간관련 기능을 QTime 클래스의 멤버함수를 통해 쉽게 구현할
수 있는 인터페이스를 제공한다．

    헤더 파일 :
    #include <QTime>
    #include <Qtwidgets /QTimeEdit>



QTimeEdit는 QTime 클래스로부터 얻어온 시간을 GUI 인터페이스 상어］ 표시할 수 있는 기능을 제공하
는 위젯이다. QTimeEdit 생성자 함수의 첫 번째 인자는 QTime 클래스로부터 얻어온 시간을 지정하면
QTimeEdit 위젯에 시간을 표시한다．

!QTime til           = QTime (6, 24, 55, 432) ; /1 hour, mmn, sec, millisecond
    QTimeEdi七 出qte;


    qte = new QTimeEdit (til,                  this) ;
    q七e小＞setGe（丑［1e七ry (10, 30, 150, 30) ;
{


46 CHAPTER 03_ GU手 설계와 제작


===== PAGE 48 =====
                                     口            口回因                     口回因
                                                         八
                                                                모전 日24國




（그림） QTimeEdit



그림에서 보는 것과 같이 hour, minute, second 표시 위치어］ 커서를 위치하고 오른쪽 스핀 버튼을 클
릭하면 시간을 변경할 수 있는 GUI 인터페이스를 제공한다．

QTime 클래스는 시간을 계산하는 다양하고 유용한 멤버함수를 통해1 기능을 제공한다. 그럼 실제 예제
코드를 통해 QTime 클래스의 멤버함수에 대해 살펴보자．

    qte[ 1] = new QTimeEclit (til.   addMSecs (200) , this) ;
    qte[ 1] ->setGeometry (10, 30, 150, 30) ;


    qte[ 2] = new QT初陀Edi土（til .addSecs (2) r 七his) ;
    qte[ 2] ->setGeometry (10, 30, 150, 30) ;




현재 시간에 millisecond와 second어］ 지정한 값만큼 더하기 위해서 addMSecs(）와 addSecs( ) 멤버함
수를 이용하면 원하는 결과를 얻을 수 있다．




（그림） addMSecs(）와 addSecs() 멤버함수


C

    QTime ti2 = QTime: :currentTime () ;
    qte[ 4] = new QTimeEdi七（七i2 .curren七Time ( ) r 七hi引 ;
    哄e [4卜＞SE比Geome七ry (10, 30, 150, 30) ;




                                                                            1_Basic Widget 47


===== PAGE 49 =====
         currentTime( ) 멤버함수는 설정된 시스템의 현재 시간을 얻어오는 멤버함수이다．


         a


             모젼 回：24:55
                                            V




（그림） currentTime( ) 멤버함수


         QTirne t13;


         ti3. start () ;


         for (int           i = 0 ; I < 100000 ; i++)
         {
               for (int          j = 0 ;        j < 100000 ;    j++)
               {
               }


iaDebua ( "Elaosed Time : %d" . ti3. elansed(fl;


!ulime
                   ti   '    =   (jrlme:   :rrombtrlng   (   ui: i '   ,   nfl: mrn   );

         QLabel *lbl   fromString = new QLabel (ti4. toString() , this) ;
         lbl   fromString->setGeometry (10, 30, 150, 30) ;




start( ) 멤버함수가 선언된 시점부터 elapsed( ) 멤버함수가 호출된 소스 코드 라인까지 처리하는 데 경
과된 시간을 얻어오는 함수로 사용할 수 있으며 , fromString( ) 멤버함수를 이용하면 다양한 방법으로
시간을 표시할 수 있다．




（그림） from앉ring() 멤버함수




48 CHAPTER 03_ GUI 설계와 제작


===== PAGE 50 =====
 Expression         Description
 h                  Hour를 0八J23 숫자로 표시
 hh                 Ho바를 00"23 숫자로 표시 （항상 2자리로 표시）
 m                 卜川nu也를 0-'- 59로 표시
 mm                卜川flu冶를 OO'-'59로 표시
 S                  Second를 小／59로 표시
 ss                 Second를 0oN59로 표시
 z                  밀리 츠를 표시 0' 999로 표시
 zzz                밀리 초를 표시 000'999로 표시
 AP                 오전／오후를 표시하는 AM/PM 문자를 대문자로 표시

 ap                 오전／오후를 표시하는 AM/PM 문자를 소문자로 표시



현재 설정된 Time에서 시간（0N出）을 얻어오기 위해 hour( ) 멤버함수를 사용하면 ii此로 시간을 리턴한
다. 그리고 분과 초도 마찬가지로 minuteC, second( ) 멤버함수를 사용한다．


 QTime t15 = QTime (6, 25, 34, 323) ;
 qDebug ( "Hour : %d", ti5. hour ( ) );
 qDebug( "Min : %d", ti5. minute() );
 qDebug( "Sec : %d", t15. second() );
 qDebug( '1Msec : %d", ti5. insec () );


［결과］
Hour: 6
入川n: 25
Sec: 34
Msec: 323

 QTime ti6 = QTime (7, 10, 23, 122) ;
 QLabel *lbl1toString = new QLabel (t16. toString( 'AP hh:mm: ss: zzzu) , this) ;
 lbl1toString- >setceometry ( 10, 30, 150, 30) ;



시간을 표시하는 방법으로 toString( ) 멤버함수를 이용하면 다양한 방법으로 시간을 표시할 수 있다．


口                 ；回因
     川＼it IJ710꾼3:122


（그림） toString( ) 멤버함수




                                                                               1 Basic Widget 49


===== PAGE 51 =====
    珷I흐 QD的毗 클래스와 OD的m曲t 위젯
    QDateTime 클래스는 날짜와 시간을 다루기 위해 제공되는 클래스로, QDateTime으로 얻은 날짜와 시
    간을 QDateT油eEdit를 통해 표시할 수 있는 GUI 인터페이스를 제공한다．

     헤더 파일：
     #include <QDateTime>
     #include <QDateTimeEdit>



QDateTimeEdit 위젯은 QDateTime 클래스 이외에 QDate와 QTime 클래스를 사용해 날짜와 시간을
표시할 수 있다．

    QDateTirneEdit *qdel;
    qdel = new QDateTimeEdit (QDateTiine: :currentDateTiine () , thi引 ;
    qdel->setDispiayFormat (1' yyyy-DD-dd hh:mm: ss: zzz ") ;
i
         >setGeometry (10, 30, 250, 50) ;
         1-
QDateTime 클래스로부터 시스템 시간을 얻어와 QDateTimeEdit 위젯에 날짜와 시간을 표시한다．
setDisplayFormat( ) 멤버함수는 Qt에서 제공하는 표현 포맷에 따라 날짜와 시간을 표시할 수 있다．

    口




     r
               1 1 38:18:704
                 :
（그림） QD計eTimeEd仕



QDateTimeEdit는 위젯에 표시된 날짜와 시간을 스핀박스 버튼으로 변경할 수 있으며, 날짜와 시간을
변경할 때 범위를 지정할 수 있다．

    qde[ 0] = new QDateTimeEdit (QDate: :currentDate () , this) ;
    qde[ 0] ->setMinimumDate (QDate: :currentDate () .addYears (- 3fl;
    qde [ 0] ->setMaximumDate (QDate: : currentDate () . addYears (3) );
    qde[ 0] ->setDisplayFormat ( "yyyy ") ;
    qde[ 0] ->setGeometry (10, 90, 100, 50) ;


    qde[ 1] = new QDateTimeEdit (QDate: :currentDate ( ), this) ;
    qde[ 1卜＞Se目linimumDa七e (QDa七e: :curren七Da七e ( ) . addNonths ( -2 ) ) ;
    qde [ 1] ->setMaximumDate ( QDate: : currentDate ( ) . addNonths (2) );
    qde[ 1] ->setDisplayForinat ( "r4M") ;
    qde[ 1J->setGeometry (110, 90, 100, 50) ;


qde[ 2] = new QDateTimeEdit (QDate: :currentDate () , this) ;
                                                                              O


50 CHAPTER 03_ GUI 설계와 제작


===== PAGE 52 =====
 qde[ 2] ->setMinimumDate (QDate: :currentDate ( ) .addDays (- 20fl;
 qde [2 ]->setMaximu山ate (QDate: : currentDate ( ) . addDays (20) );
 qde[ 2] ->setDisplayFormat ( 'dd ' ) ;
 qde[ 2] ->setGeometry (210, 90, 100, 50) ;



setMinirnumDate( ）와 setMaxin끄imDate( ) 멤버함수는 QDateTimeEdit 위젯에서 제공하는 스핀 버
튼으로 날짜를 변경할 때 , 범위를 자정하여 설정된 범위 내에서만 날짜를 변경할 수 있다．


.                                                        口同國

                                                     A
    됴-          。1- 14 11:41 吼日5
                               :
                                                     Y




         2013
                       止


                       甘
                           1
                                   01     '   1[14
                                                          :U
（그림） 0DateTimeEd仕 범위 설정




          富 1.7 QD洌

QDia1 위젯은 원 형태의 볼륨 조절기와 같은 GUI 인터페이스를 제공하며 멤버함수를 이용해 범위를 지
정할 수 있다．

 헤더 파일 :
 #include <QDial>


QAbstractS1ider로부터 상속받은 QiDial 위젯 클래스는 슬라이더 위젯과 비슷하며 시그널과 슬롯을 이
용해 QDia1 범위를 설정하거나 설정된 값을 변경할 수 있다．

 in七 자)OS = 30;
    for (int         i = 0 ; i < 3 ; i++, xpos += 110)
    {
                dial[ i]           = new QDial(this) ;
                dial[ i] ->setRange(0, 100) ;
                dial[ i] ->setGeometry (xpos, 30, 100, 100) ;



 dial [0] ->setNotchesVisible (true) ;




                                                                       1 Basic Widqet 51


===== PAGE 53 =====
=                                         回團團




（그림） CD톄



setRange( ) 멤버함수는 QDia1 위젯의 범위를 지정할 수 있다. setNotchesVisible( ) 멤버함수를 사용
하면 QDial 위젯에 눈금을 표시할 수 있다. 사용자가 QDia1 위젯을 마우스로 값을 변경하면 value
Changed(int) 시그널을 등록해 변경한 QDia1의 현재 값을 얻어올 수 있다．

 private slots:
            void changedData () ;


widget.h 헤더 파일어］ changeData( ) 슬롯함수를 선언하고 w沁get. cpp 소스 파일어］ 슬롯함수가 시그
널어］ 의해 호출되면 QDia1 위젯의 현재 값을 리턴하는 멤버함수를 다음과 같이 작성한다．

rvoid Widget: :changedData()
 {                                                                  1
            qDebug( "QDial 1 value : %d ' , dial[ O] ->value (fl;
 }


QDia1 위젯의 값이 변경되면 changeData( ) 슬롯함수가 호출될 수 있도록 connect( ) 함수를 사용한
다. 시그널 연결을 위해 생성자 함수에 다음과 같이 소스 코드를 추가한다．




 Q미쉬口 1


                      q 6 q 3 2 l D 8
ODial 1 val끄亡
QDial 1 value




                      7   7 7   7   6
QDiai 1 value
ODial 1 value




                        1
                        口     1
                              口   1
                                  口
QDi已1 1 val끄e
QDI及l i v日lu日
QDial 1 value
QDial 1 value
ODial 1 value
nr1 4   ]   寸   l        仄仄



（그림） 시그널과 슬롯을 이용한 0미al 이벤트 처리




52 CHAPTER 03_ GUI 설계와 제작


===== PAGE 54 =====
置：
 王         ,（그S口inBox와QDoubleSpin日ox
QSpinBox는 ii此형 데이터 타입의 정수 값을 상하버튼을 이용해 변경할 수 있는 GUI 인터페이스를 제
공한다. mllt형 데이터 타입 이외에 double 데이터 타입을 사용하기 위해서 QDoubleSpinBox 위젯을 제
공한다. 이 두 위젯은 11此형 혹은 double형 데이터 타입의 차이만 있을 뿐 제공하는 기능은 동일하다．

헤더 파일 :
#include <QSpinBox>
孝mnci끄de <QDoubleSpinBox>



QSpinBox와 QDoubleSpinBox 위젯은 GUI 사용자가 변경하는 값의 범위를 제한할 수 있으며 , 숫자가
표시되는 Pref奴와 Suffix 부분에 특정 문자 혹은 단위를 가리키는 문자를 사용할 수 있다. 예를 들어 화
폐를 가리키는 단위를 표시할 수 있다．

jot xpos = 10;
lot   ypos = 30;
mnt val[ 3] = {50, 100, 200} ;
double doubleHval[ 3] = {50. 5, 127. 32, 171. 342} ;


for (int   i = 0 ; i   < 3 ; i++)
{
      spin[ i]   = new QSpinBox (this) ;
      spmn[ i] ->setMmnlmum( 10) ;
      spin[ i] ->setMaxlmum(300) ;
      spin[ lI- >setValue (val[ i] );
      spin[ i] ->setGeometry (xpos, ypos, 100, 30) ;


      doublespin[ i]   = new QDoubleSpinBox (thls) ;
      doublespin[ i] ->setMinimum( 10. 0) ;
      doublespin[ i] ->setMaximum( 300. 0) ;
      doublespin[1] ->setValue (doubleHval [i] );
      doublespmn[ i] ->setGeometry (xpos + 110, ypos, 100, 30) ;


      ypos += 40;
}


setMinimum(）와 set入4aximum(）는 위젯의 최소값과 최대값을 설정하기 위한 멤버함수이다．
setValue(）는 위젯상어］ 표시할 값을 디폴트로 지정하기 위해 사용하는 멤버함수이며 , 최때毆 보다 큰 값
을 setValue( ) 멤버함수로 지정하면 디폴트 값은 최대값으로 설정된다．




                                                                   1 Basic Widqet 53


===== PAGE 55 =====
（그림） OS미nBox와 ODoubleSpinBox 위젯



 spin[ i] ->setPrefix ( "$ " );
 doublespin[ i卜>setSuffix ( " mm" ) ;



QSpinBox와 QDoubleSpinBox 위젯은 Pref奴와 Suffix 부분에 특정 문자를 지정할 수 있다．
setPrefix( ) 멤버함수는 Prefix 부분에 특정 문자를 지정할 수 있고, setSuffix( ) 멤버함수는 Suffix
부분에 특정 문자를 지정할 수 있다．




（그림） F가ef ix와 Suffix



QSpinBox와 QDoubleSpinBox 위젯은 상하버튼을 이용해 디폴트 값을 변경하면 이벤트를 처리하기
위한 시그널과 슬롯을 제공한다. 값이 변경되었을 때, 처리하기 위해 다음과 같이 헤더 파일에 소스 코드
를 추가한다．

 private slots:
      void valueChange ( ) ;
      void double_valueChange () ;



valueChange( ）는 QSpinBox 위젯의 디폴트 값이 변경되었을 때 호출할 슬롯함수이며 , double value
Change( ）는 QDoubleSpinBox 위젯의 시그널 이벤트가 발생했을 때 호출하는 슬롯함수이다．




54 CHAPTER 03_ GUI 설계와 제작


===== PAGE 56 =====
           void Widget: :valueChange()


               qDebug ( "Change value : %d", spin[ Oj->value (fl;



           void Widget: :double valueChange ()


               qDebug ( "Change double value : %3 . 2f ", doublespin[ O] ->value ( ) );




위젯의 상하 버튼을 클릭했을 때 , 변경된 디폴트 설정 값을 디버깅 창어］ 출력한다. 작성한 슬롯함수가 시
그널 이벤트가 발생했을 때 호출할 수 있도록 다음과 같이 소스 코드어］ 추가한다．

r尸삐




iconnect          (spin[               O] ,       SIGNAL                (valueChanged
                                                                                                      (int) ), this


!                   bJ. U"v
   nneCt (doublespin[
!ConneCt (d(DdbleSP끄lL UO]] ,r
                           .   ,   .          .


                                                                SIGNAL
                                                                bl (jNAL (Va上UeChanqed
                                                                쁘eLnanget      )H."'
                                                                         (valueChanged(double)
                                                                                       (dOUb上e ),                     this,
                                                                SLOT (double中valueChange () ));




           a미計口            as미出매꾜
    Change value :                     56
    Change value :
    Change value =
                                       59
                                       5日
                                                   됴百艸                                  :   5口5口rn nr       :

    Change value =                     57
    Change value :                     56               $ 103                               133.32 rn rn    :
    C hang已 valu日 :                    55
    Chan甘日 value :                     54
                                                         2口그                                171. 34 rnirn
    Ch已nge V巴lu巴 :                     55
                                                   i$
    Chan다已 value :                     56
    Change value :                     57


（그림） 시그널과 슬롯




               1.9 QPushButton과 QFocusFrame

 QPushButton 위젯은 버튼 기능을 제공하는 위젯이다. 그리고 QFocusFrame은 다른 위젯의 바깥쪽
Paintable 영역을 제어할 수 있는 기능을 제공한다. 예를 들어 버튼의 바깥쪽어］ Outer Line을 사용해야
할 경우 QFocusFrame을 사용하면 유용하다. 이 외에도 QFocusFrame은 QStyle과 같은 위젯을 사용
할 때 자주 사용된다．

 QPushButton 위젯 바깥쪽에 Outer Line을 그리기 위해1QFocusFrame를 사용하는 방법은 다음과
같다．

           헤더 파일 :
           #include <QPushButton>
           #inc lude <QFocusFrame>




                                                                                                                              lBasic Widget 55


===== PAGE 57 =====
QPushButton 위젯은 Qt 어플리케이션어써 Apply, Cancel, Yes, No와 같은 버튼을 클릭했을 때, 이
벤트를 처리하기 위한 GUI 인터페이스를 제공한다．

1QPushBu七七on 싸光n[ 3} ;


    jnt ypos = 30;


 for (int   i   = 0 ; i < 3 ; i++)
 {
       t亢n[ i] = ne＼寸 QPushBu七七on (QString( " Frame's but七on 뚬1" ) .arg(i) , 七his) ;
       btn[ i] ->setGeometry(10, ypos, 300, 40) ;


       ypos += 50;




QPushButton( ) 생성자 함수의 첫 번째 인자는 버튼어］ 표시할 텍스트를 입력하고 두 번째 인자로
QPushBu就on의 Parent Class를 지정한다. QPushButton 위젯은 Click 외에 버튼이 Pressed（버튼
이 눌려진 상태 이벤트 발생）되었을 때, Released（버튼을 누른 상태에서 마우스 버튼을 떼었을 때 이벤
트 발생）되었을 때 발생하는 시그널 이벤트를 제공한다．

지금까지 설명한 3가지 타입의 마우스 이벤트를 발생시킨 후 버튼에서 때었을 때, 이벤트 발생 순서가 어
떻게 되는지 알아보도록 하자．

widget.h

 private slots:
       void btn click ( ) ;
       void btnpressed ( ) ;
       void btn released() ;



widget.cpp

 void Widget: :btn_click ()
 {
       qDebug ( "Button Click ") ;
 }

void Widget: :btn_pressed()
 {
       qDebug( "Button Pressed") ;
 }

void Widget: :btn released()
{
       qDebug ( "Button Relased ' ) ;
}



56 CHAPTER 03_ GUI 설계와 제작


===== PAGE 58 =====
추가한 소스 코드는 버튼의 시그널이 발생했을 때 호출되는 슬롯함수이다. 시그널이 발생했을 때1 이벤트
를 처리하기 위한 슬롯함수를 연결하기 위해 생성자 함수에 다음과 같은 코드를 추가한다．

 connect (btri[ O] , SIGNJ\L (clicked(fl,   this,   SLOT (btnclick () fl ;
 connect (btn[ O] , SIGNAL (pressed(fl,     this,   SLOT (btn_pressedU) );
 connect (btn[ 0] , SIGNAL (released() ), this,      SLOT (btnreleased() fl ;



버튼을 마우스로 클릭했을 때 가장 먼저 실행되는 슬롯함수는 Pressed 이벤트가 먼저 발생한다. 그리고
마우스에서 버튼을 떼었을 때 Release 이벤트가 발생한다. Click 시그널 이벤트는 Pressed와 Release
이벤트가 처리된 후, 시그널을 처리한다．


!UpushButton_OFocusF

Starting D: \QtPro
D日가ig\d吐ng\QPu呂

콘Ut七on 中e55ed




（그림） QPushButton



이번에는 QFocusFrame을 이용해 QPushButton 위젯 바깥쪽에 Outer Line을 그리기 위해 다음과 같
이 소스 코드를 추가한다．

 QFocusFrame 出btn frame = new QF（그미娼Frame（七hi引 ;


 btn frame->setWidget (btn [0] );
 btn fra王［胞->setAutorillaackground(true) ;


setWidget( ）은 우리가 이전에 선언한 QPushButton 위젯을 QFocusFrame에 포함시키기 위한 멤버
함수이다. QF뇨shBut切n 위젯 뿐만 아니라 다른 위젯도 QFocus所跏e어］포함시킬 수 있다．




                 Fr；크me ‘드 bu枷：山 U



                 탸台I'始뇹 butt口ni



                 Frames button 2




（그림） QFocusFrame


                                                                                1_Basic Widget 57


===== PAGE 59 =====
        .10 QFontComboBox
 QFontComboBox 위젯은 G1끄상에 폰트를 선택하기 위한 GUI 인터페이스를 제공한다. 어플리케이션
 사용자어꺼 폰트를 선택하는 인터페이스를 제공해야 한다면, QFontComboBox를 이용해 폰트 리스트를
 제공할 수 있다. 이 위젯은 폰트가 알파벳 순서로 나열되고, 폰트의 모양도 확인할 수 있다．

 헤더 파일 :
 半include <QForitCoi址珣Box>



QFont（그omboBox 위젯 상에서 사용자가 새로운 폰트를 선택하면 currentFontChanged( ) 시그널 이
벤트가 호출된다. 비슷한 시그널로 QFontComBox 위젯에 등록된 폰트의 Index를 리턴하는 시그널 이
벤트를 제공한다．

 QFontCornboBox *fontcombo[ 5] ;


 for (int   I   = 0 ; I    < 5 ; i++)
 {
      此毗con由o[ i]         = new QFon七CornboBox（七his) ;



 如ntco岫o[ 0 ] 수se七FontFilters (QFon七CorthoBox: :AllFon七5 ) ;
 fon七con山이 l] ->se七For比Fil七ers (QFontCon由oBox: : ScalableFon七S ) ;
 f on七con由아 2卜＞setFontFil七ers (QFontCoirtboBox: : NonScalableFon七S ) ;
 fontconibo [3] ->setFontFilters (QFontCornboBox: :MonospacedFonts) ;
 f on七con由o[ 4] ->se七Fon七Fil七ers (QFontComboBox: : Pr아均此ionalFon七5 ) ;


 mnt ypos = 30;
 for (int   I   = 0 ; i   < 5 ; i++)
 {
      此毗con山0d1-犯e七Geometry (10, ypos, 300, 30) ;
      ypos 十＝ 40;




setFontFilters( ）는 QFontComboBox 위젯상어］ 나열할 폰트 목록을 상수를 통해 특정 폰트만을 표시
하기 위해 사용하는 타입이다．

상수                                        값       설명
QFontComboBox::AllFonts                   0       모든 폰트
QFontComboBox::Sca冶비eFon怡                 Ox]    확대 및 축소와 같은 동적 자동 변환이 가능한 폰트
QFontComboBox::NonSca冶비eFonts             0x2    동적 자동 변환이 제공되지 않는 폰트
QFontComboBox::MonospacedFon怡             0x3    일정한 문자 넓이 형태를 제공하는 폰트
QFontComboBox사가oportion톄Fon恰              0x4    넓이와 폭의 균형이 잡힌 폰트




58   CHAPTER 03_ GUI 설계와 제작


===== PAGE 60 =====
      i3                     [ 口 回 Ii叫 "


                굴림1                      .

                굴림                            ,

                                              可     Courier
                                                   ·크 Courier
                                                   ·크 日xeds s


                                                   a MS Serif

                                              量    a Small Fonts


I..                                      立艸
                                              !     ·크 System
                                                  -a Terminal

（그림） QFontComboBox 위젯



QFontComboBox 위젯을 사용하는 목적은 어플리케이션 사용자가 선택한 폰트를 특정 텍스트를 표시하
기 위해 사용하는 경우가 많다. 예를 들어 선택한 폰트를 QLabel의 폰트로 변경하기 위해서 QFont（그om
boBox 위젯의 시그널을 사용한다．

QFontComboBox 위젯상에서 폰트를 선택하면 폰트의 인덱스를 리턴하는 currentlndexChanged(int)
시그널 함수가 선택한 폰트의 QFont를 리턴하는 currentFontChanged(QFont) 시그널 함수를 제공
한다．

그럼 실제 예제를 통해 QLabel 위젯의 폰트를 QFontComboBox 위젯에서 선택한 폰트로 변경하기 위
해 다음과 같이 소스 코드를 작성해 보자．

widget.h

      private          slots:
                  void changedlndex (int idx) ;
                  void changedFont (const QFont &f) ;


widget.cpp

      ibi         = new QLabel ( " I   love Q七 progra끄rming", thi引 ; // lbl 추가
      lbl- >se七Geometry (l0, ypos, 200, 30) ; 7/ lbl               위젯 위치


      // 선택한 폰트 인덱스 리턴 시그널
      connect (fontcombo[ 0] , SIGNAL (current工ndexChanged(int) ), this,
                                        SLOT (changedlndex (int) ));


      // 선택한 폰트 리턴 시그널
      connect (fontcoxnbo[ 0} , SIGNAL (currentFontChanged(QFont) ), this,
                                        SLOT ( changedFont (const QFont &)));




                                                                                 1_Basic Widget 59


===== PAGE 61 =====
                                   Berlin Sans F日 Den기


                                   Vrinda


                                   Terminal


                                   Consolas


                                   굴림


                                  11口ue Qt 才口亨口1n1如q




（그림） OLabel 폰트를 OFoniComboBox에서 선택한 폰트로 변경



첫 번째 QFont（그omboBox 위젯을 변경하면 발생한 시그널 이벤트가 changedFont( ) 슬롯함수를 호출
할 수 있도록 connect( ) 함수를 이용해 시그널과 슬롯을 연결한다. 이 함수는 QLabel의 setFont( ) 멤
버함수를 이용하면 기존 폰트 QFontC아nboBox에서 리턴한 폰트로 변경할 수 있다．



            QLabe꽈 QLCDNumber
QLabel 위젯은 어플리케 ' ］션 상에 텔슨튼曳안민싻曼프신괏玎l늅을 제공하는 위젯'］다砒CD-
Number 위젯 또한 어플리케이션 상에 텍스트를 출력할 수 있다. 문자는 표현할 수 없고 숫자만 표시할
革a3tl1.숙丙百느侖可슐횬늉菲7:萍g翁俺 수 있는 GUI 인터페이스를 제공한다. 그리고
QLCDNumber는 시간을 표시할 때 사용하는 ":" 문자를 함께 사용할 수 있다．

 헤더 파일 :
 #include <QLabel>
 孝include <QLCDNun由er>



0QLabel
QLabel은 텍스트 혹은 이미지를 GUI어T 표시하는 위젯이다. 또한 QMov扼를 통해1 출력되는 영상을
QLabel 위젯과 연결해 멀티미디어 영상을 실시간으로 출력할 수 있다. 예를 들어 동영상 혹은 캠으로부
터 출력되는 데이터를 QByteArray 데이터 타입어］ 저장하여 QLabel 위젯상어］ 영상을 출력할 수 있다．

 QLabel   *lbl[ 2] ;

lbl[ 0] = new QLabel ( "I love Qt prograinn'ing", this) ;
lbl[ 0J->setGeometry (10, 30, 200, 40) ;


QPixmap pix = QPixmap ( '느resources/ browser.png ") ;

lbl[ l} 口 new QLabel（七hi引 ;
lbl 口 ] ->se七i山map (pi지 ;
lbl[ 1] ->setGeometry (10, 70, 100, 100) ;



60 CHAPTER 03_ GUI 설계와 제작


===== PAGE 62 =====
QPixmap 클래스는 이미지를 GUI상어］ 렌더링하기 위해 제공되는 API이다. QPixmap을 이용해 렌더링
한 이미지를 QLabel 위젯의 setPixmap( ) 멤버함수를 이용하면 Gt月상어］ 표시할 수 있다．

  可    匕
       Q   口
                回       h


  1 伯V日 Ot programm岫




  (i
（그림） QLabel Widget



小QLCDNumber
QLCDNumber는 디지털 시계와 같은 스타일로 숫자를 표시할 수 있는 기능을 제공하는 위젯이다．

 QLCDNumber *lcd[ 2] ;
 lcd[ 0] = new QLCDNurnber (2, this) ;
 lcd[ 0] ->display (24) ;
 lcd[ 0] ->setGeometry (150, 30, 200, 100) ;


 lcd[ 1] = new QLCDNUII幻er (5, 七hi引 ;
 lcd[ 1] ->display ( " 10: 34 ") ;
 lcd[ 1} ->setGeometry (150, 140, 200, 100) ;



QLCDNumber 생성자 함수의 첫 번째 인자는 표시할 숫자의 개수이다. display( ) 멤버함수에 표시할
숫자 혹은 텍스트를 입력하면 디지털 시계와 같은 스타일로 GUI상에 표시할 수 있다．


 U그 QLab이 and QLCDNuniber ＼사idget        1叫    1




                                               /


（그림） QLCDNumber 위젯


                                                       1 Basic Widget 61


===== PAGE 63 =====
            예제에서 사용한 QLCDNumber 위젯은 상수 타입을 사용해 숫자 안쪽이 칠해질 때 , 윈도우 Back
            ground 색과 동일한 컬러로 채우거나 혹은 외각선의 표시 스타일을 다음과 같이 변경할 수 있다．

            상수                                                             값            설명
            QLCDNumber::Outline                                                         윈도우 Background 색과 동일하게 표시
            QLCDNumber::Filled                                             ]            폰트 컬러와 동일한 색으로 표시
            QLCDNumber:下冶t                                                              외과선이 나타나지 않는 스타일


            lcd [0 ]->setSegmentStyle (QLCDNumber: : Outline) ;
            lcd[ l] ->se七Segmen七Style (QLCDN王끄r由er: :Filled) ;
    ilcd[
                 2]   ->setSegmentStyle
                                                                                   (QLCDNu由er: :Flat) ;




              出 크니
              出 : 크나
    （그림） QLCDNumber 스타일




            王m曲eEdit
    QLineEdit 위젯은 사용자가 텍스트를 입력하기 위한 GUI 인터페이스를 제공하는 위젯이다. 텍스트가
    변경될 때 시그널을 제공하며 변경된 QLineEdit 위젯의 텍스트를 QString 문자열을 슬롯함수에게 인자
    로 전달한다．

    ! 헤더 파일：
    ! 半include <QLineEdit>

    워드프로세서 혹은 윈도우 메모장과 같은 어플리케이션어써 특정 블록을 복사, 붙여넣기, 자르기 등의 기
능을 제공한다．

    widget.h
    private:
                 QLineEdit; 火edi幻
                 QLabel *lbl;


!
                  e                       ,   slots:
                                                       .   ,   .   ,   .       .
                                                                                    .
                                                                                         .   .




!                 1O textUnangeo (12atr工ng SEE) ;



62 CHAPTER 03_ GUI 설계와 제작


===== PAGE 64 =====
txchChanged( ）는 QLineEdit상에서 텍스트를 입력 , 수정 등과 같이 변화가 있을 때 시그널이 발생되
면 호출되는 슬롯함수이다．

widget.cpp

 edit = new QLineEdit ( n ", this) ;
 ibi     = new QLabe1( "Q1ineEdit Text : ", this) ;


 connect ( edi七, SI（批A디比砒Changed ( QS七ring) ), 七hi旬
                         SLOT (textChanged(QString) ));



QLineEdit 생성자 함수의 첫 번째 인자는 위젯에 표시할 텍스트이며 , QLineEdit상어］ 텍스트를 입력，
수정, 삭제 등이 일어나면 시그널이 발생한다. 발생한 시그널을 슬롯함수가 호출될 수 있도록 connect()
함수를 이용해 등록한다. 따라서 QLineEdit 위젯의 텍스트가 변경되면 QLabel 위젯에 표시된다．


                                         叫

     ' I love （計 口r口gn크mmin미


      lineEdit Text : I love Ot programming   m

                                              月

                                              n

                                              니

                                              1




（그림） OLineEdit



QLineEdit는 입력한 텍스트를 보이지 않게 하거나 패스워드 처리가 가능하다. 이와 같은 처리를 하기
위해 setEchoMode( ) 멤버함수에 인자로 다음과 같은 상수를 사용해야 한다. 상수를 사용하면 어떤 변
화가 있는지 확인하기 위해 디폴트로 "I love Qt programming" 텍스트가 위젯에 입력된 상태이다．

 상수                                           값   설 명
（긔JneE뎨口Normal                                    디폴트와 동일한 스타일
a니fleE베二NoEcho                                    입력한 테스트가 보이지 않으며 커서의 위치도 변경되지
                                                  않는 스타일
（값JneEd比：Password                                 텍스트가 "士" 문자로 표시
QLineEdit::PasswordEchoOnEdit                     텍스트가 변경되면 디폴트 스타일과 동일하지만 포커스가
                                                  이동되면 "士 ' 표시



 mnt ypos = 120;
 for (int i = 1 ; i < 5 ; i++)
 {
         edit[ i]     = new QLineEdit ( "I love MeeGo. ", this) ;
         edit[ i] ->setGeometry (l0, ypos, 200, 40) ;
          ypos += 50;
 }                                                                                        O


                                                                             1_Basic Widget 63


===== PAGE 65 =====
edit [ l] ->setEchoMode ( QLineEdit: : Normal) ;
 edit[ 2] ->setEchoMode(QLineEdit: :NoEcho) ;
 edit[ 3] ->setEchoMode (QLineEdit: :Password) ;
 edit[ 4] ->setEchoMode (QLineEdit: :PasswordEchoOnEdit) ;




 1 I[ 'e qt.




 e1e10 01111


 11 1 e101 11 1


（그림）（긔ineEd作 위젯 스타일




     t          QMenu와 QMenuBar
QM이Ilu와 QMenuBar 클래스 위젯은 어플리케이션 상어］ 메뉴의 GUI 기능을 제공하기 위해 사용되는
클래스이다．

 헤더 파일：
 #include <QMenu>
 #inc lude <QMenuBar>



QMenu 위젯은 메뉴를 만들기 위해1 제공하는 위젯으로써 addAction(）과 add八4enu( ) 멤버함수를 제공
한다. addAction(）은 하위 메뉴가 없이 바로 실행할 기능을 연결하기 위해 사용되고, addM帥u(）는 하
위 메뉴를 연결할 때 사용하는 멤버함수이다. QM아lU로 생성한 위젯을 QMenuBar와 연결해 메뉴를 완
성할 수 있다．

 menu[ 0] = new QMenu( "File ") ;
 menu[ 0] ->addAction ( "Edit ") ;
 menu [ 01 ->addAction ( "View' );
 menu [ 01 ->addAction ( "Tools ") ;


 ac七［0] = new QAc七ion( " Ne可' r 七hi引 ;
 ac七［0] ->se七Shor七Cu七（Q七：:C쏘RL 1 Q七：: Key_A) ;
 缸比［0] ->setS七a七usTip ( "This is a New menu. " ) ;


 a（北［1] = new QA（그七ion( " Open", 七hi引 ;
 act[ l] ->setCheckable (true) ;


 menu[ l]      = new QMenu( "Save") ;
 menu[ l] ->addAction(act[ 0] );                               O



64 CHAPTER 03_ GUI 설계와 제작


===== PAGE 66 =====
menu [ 1卜＞addAc七ion(ac七 [ 1 ] ) ;


menu[ 2] = new QMenu ( "Print ") ;
menu[ 2] ->ad아＼ction ( "Page Setup'! );
rnenu[ 2] ->adclMenu (menu[ 1] );


menuBar->addNenu (menu[ O] );
menuBar->addMenu (menu [2] );



帥4enu 클래스 위젯은 위젯으로 생성한 "File", "Save" 그리고 "Print" 상위 메뉴이다. 그리고
QAction 클래스로 생성한 메뉴는 하위 메뉴로 추가하는 클래스 위젯이다. 최종 하위 메뉴는 QAction
위젯을 연결해야 하지만 하위 트리구조와 같이 여러 Depth의 메뉴 트리를 작성하기 위해 Qt는 QMenu
를 하위 메뉴로 위치할 수 있다. 이 예제에서는 Save 메뉴를 Print 하위 메뉴어］ 위치시키기 위해
帥4enu 클래스의 addMenu( ) 함수를 사용하면 된다.




           Selected Menu : Page Setup
뇨



（그림） QMenu와 OMenuBar



QAction( ) 함수를 사용하면 하위 메뉴를 추가할 수 있으며, setShortcut( ) 멤버함수는 메뉴의 단축키
를 사용할 수 있다. 그리고 setStatusT巾() 멤버함수는 메뉴 ToolTip 기능을 추가할 수 있다．

    ac七［0] = nei寸 QAc七ion( "New",                        thi引 ;
    a（北［0卜＞setShor七Cu七（Q七：:CTRL ! Q七：:Key A) ;
    a（比［0卜＞setS七a七邸Tip ( ' This is a Ne＼寸 menu. " ) ;


                                                                  口   1i刃

    'Fle
               Ii [[iI
                         Page Setup
                         Save         卜   New    CtrkA
                                          0口en




（그림） 메뉴의 단축키


                                                                            1_Basic Widget 65


===== PAGE 67 =====
 act[ O] = new QAction( "Audio", this) ;
 a（北［0] ->se七Shor七Cu七（Q七：:CTRL 1 Q七：: Key_A) ;
 act[ 0] ->setStatusTip ( "This is a Audio menu. '1 ) ;


 act[ 1] = new QAction ( "Video", this) ;
 act[ 1] ->setCheckable(true) ;


 menu[ 1} = new QMenu ( "Gstreamer ") ;
 menu[ 1] ->addAction (act[ O] );
 menu[ 1] ->addAction(act[ 1] );


setCheckable( ）는 메뉴상에 체크 기능을 추가할 수 있으며 , 인자로 true를 설정하면 메뉴상에 체크 기
능이 활성화 된다．




（그림） 체크 기능



선택한 메뉴를 실행하기 위해 connect( ) 함수를 사용하여 시그널과 슬롯을 연결해야 한다. 선택한 메뉴
가 실행되면 triggered( ) 시그널 이벤트가 발생한다. 이 시그널을 작성한 슬롯함수와 연걸한다．


 ibi   = new QLabel ( " ", this) ;


 conneCt (menuBar, SIGNAL(triggered(QAction* )), this,
                   SLOT ( 七rigerMenu (QAc七ion士 ) ) ) ;


메뉴 시그널 이벤트가 발생하면 실행된 메뉴명을 QLabel 위젯에 출력하기 위해 슬롯함수를 다음과 같이
작성한다．

 void Widget: :trigerMenu (QAction *act)
 {
       QString str = QString( "Selected Menu : %1") .arg(act->text (fl;
       lbi- >setText (str) ;




                                     （그림） 메뉴 이벤트 처리


66 CHAPTER 03_ GUI 설계와 제작


===== PAGE 68 =====
     1.14 QProgressBar
프로그램을 설치하거나 인터넷을 통해 파일을 다운로드 받을 때 진행사항을 표시하기 위한 위젯으로，
QProgressBar 위젯을 활용할 수 있으며 가로와 세로 방향으로 위젯을 표시할 수 있는 GUI 인터페이스
를 제공한다．

 헤더 파일：
 #inc lude <QProgressBar>



QProgressBar 위젯은 가로 방향으로 배치할 경우 왼쪽에서 오른쪽으로, 오른쪽에서 왼쪽으로 진행 방
향을 변경할 수 있다. 반대로 세로 방향으로 배치할 경우 아래에서 위로, 위에서 아래로 진행 방향을 표시
할 수 있다．

 QProgressBar *progress [21;


 progress[ O] = new QProgressBar (this) ;
 progress [0 ]->setMinimum( 0) ;
 progress[ 0} ->setMaximuxn( 100) ;
 progress[ 0} ->setValue (50) ;
 progress[ 0} ->setOrientation(Qt: :Horizontal) ;


 progress[ 1] = new QProgressBar (this) ;
 progress [ 1] ->setMinimuni( 0) ;
 progress[ 1} ->setMaximum( 100) ;
 progress[ 1]->setvalue(70) ;
 progress[ 1} ->setOrientation(Qt: :Horizontal) ;
 progress [ 1]->setlnvertedAppearance (true) ;



setMinimum( ）와 set入4aximum( ) 함수를 이용해 QProgressBar의 최소값과 최대값을 설정할 수 있
으며 , setRange( ) 멤버함수를 이용하면 최소값과 최대값을 함께 설정할 수 있다. setValue( ）는 QPro-
gressBar의 최소값과 최대값 사이의 진행값을 설정하기 위해1 사용하는 멤버함수이며 , setOrienta-
tion( ) 함수는 가로 혹은 세로 방향으로 표시할 지 설정할 수 있다．
그리고 setlnvertedAppearance( ) 멤버함수는 진행 방향을 설정하기 위한 멤버함수이다. 인자로 true
를 설정하면 디폴트 설정의 반대 방향으로 바꿀 수 있다.




                                    50拓

                                    70鬼
                                難



（그림） QProgressBar



                                                         1_Basic Widget 67


===== PAGE 69 =====
     progress [2] ->setValue (50) ;
     progress [ 2] ->se七Orieri七a七ion(Q七：: Ver七ical) ;


     progress [3] ->setValue (70) ;
     progress [ 3] ->se七Orien七a七ion(Q七 : :Ver七ical) ;
     progress [ 3 ] ->setlnvertedAppearance (true) ;



setOrientation( ) 멤버함수의 인자로 Qt::Vertjcal 상수를 사용하면 QProgressBar를 세로 방향으로
변경할 수 있으며, seth나ertedAppearance( ) 멤버함수의 인자를 true로 설정하면 진행 방향을 반대로
변경할 수 있다．




（그림） QProgressBar




                  QRadioBu卄on

QRadioButton 위젯은 사용자에게 여러 항목 중 하나를 선택할 수 있는 인터페이스를 제공한다．

1 헤더파일：
1#
         include <QRadioButton>


On(checked) 혹은 Off (unchecked）와 같이 둘 중 하나를 선택하기 위해 사용하며 QCheckBox 위젯과
달리 여러 항목 중 하나만 선택할 수 있다．

     QString strl[ 3] = { 'NetBook ", "Handset ", "Tablet"} ;


     m1lt ypos = 30;
     for (int i = 0 ; i < 3 ; i++)
     {
           radiol[ i] = new QRadioButton(strl[ i] , this) ;
           radiol[ i] ->setGeometry (10, ypos, 150, 30) ;


            ypos += 40;
     }



68 CHAPTER 03_ GUI 설계와 제작


===== PAGE 70 =====
 QString str2[ 3] = {"In- Vehicle", "Smart TV", "Media Phone "} ;


 ypos = 30;
 for (int i = 0       i < 3 ; i++)
                  1
                  l
 {
        radio2 [i] = new QRadioBu七ton(s七r2 [ii,   七hi引 ;
        if (i == 2)
             radio2 [1] .->setChecked (true) ;
        radio2[ i] ->setGeometry (180, ypos, 150, 30) ;


        ypos += 40;
 }

QRadioButton 위젯 중 선택된 상태를 설정하기 위해 setChecked( ) 멤버함수를 사용할 수 있다．

                                         回 k回


     戶JNet日口마（              ln-Veh比伯


       Handset              SmartTV


       Tablet            仙 Med治 Phone




（그림） QRadioBu卄on



만약 6개 항목에서 왼쪽 3개 항목을 그룹으로 지정함으로써 오른쪽 QRadioButton과 분리할 수 있다．

 QButtonGroup *groupl = new QButtonGroup(this) ;
 QButtonGroup *gr0up2 = new QButtonGroup (this) ;
 groupl->addButton (radio1[ 0] );
 groupl->addButton(radiol[ 1] );
 groupl->addButton(radiol[ 2] );
 group2->addButton (radio2[ 0] );
 group2->addButton(radio2[ 1] );
 group2->addButton(radio2[ 2] );




      J Net800k          戶l In-Vehicle


     多． Handset           J Sma八TV


      」 Tablet            a」卜4ed治 Phone




（그림） QRad向跏tton과 QBu如nGroup


                                                                    1 Basic Widget 69


===== PAGE 71 =====
                 QScr이lArea
 QScrollArea는 위젯 혹은 레이아웃을 포함시켜 하나의 읜도우를 여러 개로 분리할 수 있다．

     헤더 파일．:
 !
          jude <vscroi上／\rea>



 리스트 박스 기능의 커스텀 위젯으로 구현할 때 QScrollArea 위젯을 사용하면 리스트 박스상어］ 표시된
 항목이 많을 때 리스트 항목을 상하 조절할 수 있는 기능을 제공한다. 그리고 이미지를 QLab이을 이용해
 렌더링 한 다음, 이미지가 큰 경우 QScrollArea에 포함시켜 이미지 \[jew Port 영역을 스크롤 바로 이
 동할 수 있다．

     QLabel 士ibi = new QLabel作hi引 ;
     Qlmage image ( " :resources/ dj . jpg") ;

     lbl- >setpi지nap (QPixmap: :fromlmage (image) );

     area = new QScrollArea (this) ;
     area->setwidget ( ibi) ;
     area->setBackgroundRole ( QPaiette: : Dark) ;


     area->setGeometry(0, 0, image.width( ), iniage.height () - 60) ;



Qlmage 클래스를 이용해 로딩한 이미지를 QLabel 위젯 상어］ seti万xmap( ) 멤버함수를 이용해 렌더링
한다. 렌더링 한 이미지는 QLabel 위젯 상에 표시된다．

QScrollArea 위젯의 setWidget( ) 멤버함수를 이용하면 QLabel 위젯을 QScrollArea 위젯 영역에 포
함시킬 수 있다. 만약 이미지가 QScrollArea 위젯보다 큰 경우 자동으로 스크롤 바가 활성화 된다．




（그림） QScr이'I놔ea 위젯


70 CHAPTER 03_ GU! 설계와 제작


===== PAGE 72 =====
     tii           QScrollBar
QScrollBar는 위젯에 표시할 수 없는 영역을 보여주기 위해 제공되는 GUI 인터페이스이다. 슬라이더
위젯의 모양과 비슷하지만 QScrollBar 위젯은 아래 혹은 오른쪽에 Add-On 시킬 수 있다. 윈도우 영역
을 모두 보여주기 어려운 GUI상에 QScrollBar 위젯을 사용해 특정 영역 위치로 이동시킬 수 있는 인터
페이스를 제공한다．

 헤더 파일 :
I #include <QScrollArea>

QScrollBar는 위젯의 좌우 혹은 상하 위치에 Add-On 시킬 때 세로 방향 혹은 가로 방향으로 배치할 수
있는 기능을 제공한다．

 mnt xpos = 10;
 mnt ypos = 50;
 for (int i        = 0 ; i < 3 ; i++)
 {
         vscrollbar[ i]             = new QScrollBar (Qt: :Vertical,   this) ;
         vscrollbar[ i] ->setRange(0, 100) ;
         vscrollbar[ i] ->setGeometry (xpos, 30, 20, 200) ;


         lbl[ i]   = new QLabel (QString ( "%l ' ) .arg(vscrollbar[ i] ->value () ), this) ;
         lbl[ i] ->setGeometry (xpos + 2, 220, 30, 30) ;
         xpos += 50;


         hscrollbar[ i]              = new QScrollBar (Qt: :Horizontal, this) ;
         hscrollbar[ i] ->setRange (0, 100) ;
         hscrollbar[ i} ->setGeometry (150, ypos, 200, 20) ;
         ypos += 30;
 }


E                                               口r回1叫


                                          區
           ！多

                                   匕
                                   小 匕
                                     小
                                                         卜




     0      0            0


                    n   n蚣nm口口n出m毖蚣蚣艾｛m




（그림） QScr에Bar 위젯



                                                                                          1 Ba미C Wid（그et 71


===== PAGE 73 =====
수직 방향으로 배치한 QScrollBar 위젯의 눈금을 변경해 SIGNAL 이벤트를 슬롯함수와 연결해 값을 변
경하면 그림에서 보는 것과 같이 라벨과 가로 방향 QScrollBar 위젯의 눈금을 변경하기 위해 value-
Changed( ) 시그널 이벤트 함수를 사용할 수 있다．

    connect (vscrollbar[ OI, SIGNAL (valueChanged(int) ), this,
                             SLOT (valueChangedl (int) ));



value（그hanged( ) 시그널은 QAbstractS1ider 클래스로부터 상속 받도록 구현되었기 때문어］ QScroll-
Bar 위젯에서 사용할 수 있다．

    void Widget: :valueChangedl (mnt value)
    {
         lbl 四卜相e七Te＞比 ( QS七ring( "%l " ) .arg(value) );
         hscrollbar [0] ->se七＼冶lue ( vscrol끄冶r[ 0卜＞value ( ) ) ;




슬롯함수는 세로 방향의 QScrollBar 위젯 눈금이 위치한 값을 QLabel 텍스트상어］ 표시하고 setValue()
멤버함수를 이용해 가로 방향의 QScrollBar 위젯의 값을 동일하게 변경한다．




（그림） QScr에Bar 위젯 시그널과 슬롯




        多打祠Q帥的ri口

                         「“'「" "'「］
器黑磊器器瓷群少蚣곕'］다꼐를드"어 """""' 윈
1 헤더 파일．’         .     .
[        jude <Ubizeurip>




72 CHAPTER 03_ GU1 설계와 제작


===== PAGE 74 =====
QSizeGrip 위젯은 한정된 크기의 윈도우 영역 안에 위젯의 크기를 조절할 수 있다. 예를 들어 윈도 탐색
기와 같이 왼쪽에는 트리 영역 , 오른쪽은 파일 및 디렉토리 속성을 보여주는 GUI 상에서 트리 영역의 경
계선을 마우스로 드래그하여 줄이거나 늘릴 수 있는 것처럼 QSizeGr如을 이용하면 Splitter와 같은
GUI 인터페이스를 구현할 수 있다．

widget.h

class SubWindow : public Qwidget
 {
   Q OBJECT
public:
          Subwindow (QWidget *parent = 0) : QWidget (parent, Qt: :SubWindow)
          {
                  QSizeGrip *sizegrip = new QSizeGrip(this) ;
                  sizegrip->setFixedSize ( sizegrip->sizeHint () );


                  七his->setLayou七（ne1寸 QVBoxLayou七）; II Su小吐ndow의 레이아웃을 선언
                  七his->layou七（卜＞se七Margin(0) ;        // 여백설정
                  layout ( )->addWidget (new QTextEdit) ;


                  sizegrip->setWindowFlags (Qt: : WindowStaysOnTopHint) ;
                  sizegrip->raise () ;
              }

          QSize sizeHint () const
          {
                  return QSize(200, 100) ;
          }
 };

 class Widget : public Qwidget
 {
          Q OBJECT

 public:
          Widget (oWidget *parent = 0) ;
          -Widget U;
     };
m톄n.Cpp

 QApplication a (argc, argv) ;
 Widget w;
 w.resize(400, 300) ;


     SubWindow subWindow( &w) ;         ，뇨J j' ta
                                       뇨／           itt, L
     subWindow.move (200, 180) ;


     w. show() ;
     return a.exec ( );


                                                                               1_Basic Widget 73


===== PAGE 75 =====
 예제에서 Widget 클래스는 부모 윈도우로 선언하고 SubWindow 클래스는 \Widget 윈도우의 Child 윈
 도우이다. Sub\硝ndow 클래스 선언 시, 첫 번째 인자를 \Widget 클래스로 선언한 Widget을 명시하면
 Widget 클래스의 Sub 윈도우로 선언할 수 있다．

작성한 소스 코드상에 QVBoxLayout은 수직 방향의 레이아웃을 이용해 위젯을 배치하기 위한 위젯으로
 써 추후 자세히 다룰 것이므로 여기서는 Sub Window의 레이아웃으로 선언한다는 정도만 알고 넘어가
도록 하자. QTextEdit 위젯은 메모장과 같이 텍스트를 편집하기 위해 제공되는 위젯이다. 인터페이스는
QLineEdit와 동일하다. QLineEdit와 달리 QTextEdit는 여러 텍스트 라인을 편집할 수 있다．

예제에서 선언한 QTextEdit 위젯은 SubWindow 영역의 전체 영역 크기로 설정해I Sub 윈도우 크기를
변경할 때, QTextEdit로 변경하기 위해1QVBoxLayout으로 동적으로 크기가 변경할 수 있도록 작성한
예제이다．


                                             1m




                       OTextEd仕 뻐dget... ,




           小m恥好朴亥 tn




（그림） QSizeGri을 이용한 Child Window SIZE 변경



그림에서 보는 것과 같이 Child Window 왼쪽 상단 영역을 마우스로 드래그하여 크기를 조절할 수 있다．



           QSlider

욘雙蛇是겔율떤솟塑1-떤；迅造쯔르쁘戈赳心쳔쨘是好孚 수 있는 GUI 인터페 "］스를 제
공한다．

헤더 파일：
#include <QSlider>


일전에 다루었던 QScrollBar와 상당히 유사하다. set入Iinimum( ）과 setMaximum( ) 멤버함수를 사용
해 최소값과 최태값을 설정할 수 있다. 최소값과 최대값을 설정하기 위해 setl之ange( ) 멤버함수를 사용
하면 QSlider 위젯의 Minimum 값과 Maximum 값을 설정할 수 있다．



74 CHAPTER 03_ GUI 설계와 제작


===== PAGE 76 =====
if (i <= 2)
     {
           slider[ i]   = new QSlider (Qt: :Vertical,   this) ;
           slider[ i] ->setGeometry (xpos, 20, 30, 80) ;
           xpos += 30;
     }
     else if (i >= 3)
     {
           slider[ i]   = new QSlider (Qt: :Horizontal, this) ;
           slider[ i] -.>setGeometry (130, ypos, 80, 30) ;
           ypos += 30;
     }

     slider[ i] ->setRange(0, 100) ;
     slider[ i] ->setValue (50) ;
}


QSlider 위젯은 수평 방향과 수직 방향의 GUI 인터페이스를 제공하고, QSlider의 생성자 함수의 첫 번째
인자어］ Qt::Vertjcal(수직）혹은 Qt: :Horjzontal(수평）상수를 사용하면 위젯의 방향을 변경할 수 있다．

xpos = 20;
for (int   i = 0 ; i < 3 ; i++)
{
     lbl[ i]   = new QLabel(QString( "%l ") .arg(slider[ i} ->valueW, this) ;
     lbl[ i] ->setGeometry (xpos+10, 100, 30, 40) ;
     자均S += 30;
}


QLabel 위젯은 수직 방향의 QSlider의 눈금이 위치한 값을 표시하기 위해 사용한 위젯이다. 그리고
QSlider의 눈금의 위치가 변경될 때 , 시그널 이벤트를 발생해 QLabel 위젯의 텍스트를 QSlider의 현재
값으로 변경한다. QSlider의 값이 변경될 때, 시그널 이벤트를 슬롯함수를 연결하기 위해 다음과 같이
소스 코드를 추가한다．

connect (slider[ 0] , SIGNAL (valueChanged(int) ), this,
                         SLOT(valueChangedl (int) ));


시그널이 발생하면 슬롯함수에서 QLabel의 텍스트 값을 변경하고 수평 방향의 QSlider의 위치를 수직
방향의 QSlider의 현재 값과 동일하게 변경하기 위해 다음과 같이 슬롯함수를 작성한다．

void Widget: :valueChangedl (int value)
 {
     lbl四卜＞se七Te比（QS七ring ( " 돔1" ) .arg(value) );
     slider[ 3] ->setValue (slider[ 0] ->value () );
 }




                                                                                1_Basic Widget 75


===== PAGE 77 =====
引




    72   22   74




（그림） 0Slider 위젯




   fT.20 ' QTabWidget
괄르쁘곌曼哭進世쁘돛쁘므끄쁘크일 때 탭을 사용하면 유용가다· 어플리케'］션 개발 시，
QTabWidget은 제한된 크기에 모든 탭을 표시할 수 없을 경우 동적으로 페이지를 이동할 수 있는 기능
을 제공한다．

 헤더 파일 :
 #include <QTabWidget>




（그림） QTabWidget GUI 인터페이스



QT카)Widget상어］탭을 배치하기 위해서는 addTab( ) 멤버함수를 이용해 탭을 연결할 수 있다．

 QTabWidget *tab = new QTabWidget (this) ;


 QWidget *browserHtab = new QWidget;
 QWidget *usersHtab = new QWidget;


 tab->addTab(browser-1tab, Qlcon( " 1 /resources/browser.png") ,    "Browser ") ;
 tab->addTab(users_tab, Qlcon( " . /resources/users .png") ,   "Users ") ;



QWidget으로 선언한 위젯을 tab 인스턴스 위젯상어］ 배치하기 위해 addTab( ) 멤버함수를 사용할 수 있
으며 탭의 왼쪽어］ 아이콘을 배치할 수 있다．

각 탭 상에 위젯을 배치하는 방법은 지금까지 위젯을 배치하기 위해 부모 클래스를 인자로 명시한 것처럼
부모 클래스를 탭 위젯으로 명시하면 탭 상어］ 위젯을 배치할 수 있다．




76 CHAPTER 03_ GUI 설계와 제작


===== PAGE 78 =====
     QS七ring 1此l느str[ 3] = { " Bu七七on 1 ",                  "Bu七七on 2 ",   " Bu七七（)n 3 " };
     QPushBu七ton 싸光n[ 3 ] ;


     mnt ypos = 30;
     for (int   i = 0 ; i < 3 ; i++)
     {
         l：此n[ i]   = new QPushBu七七on (btn_str [ ii,               browser－小七ab) ;
         t亢n[ i卜＞se七Geome七ry (10, ypos, 100, 40) ;
         ypos += 50;
     }




（그림） 탭 상에 QPushButton 배치



browse乙tab 인스턴스어］ QPushButton 위젯을 배치하기 위해 QPushButton 생성자 함수의 두 번째
인자어］ 부모 클래스를 지정할 수 있다. 두 번째 인자에 browser tab을 선언하면 QPushButton을
browser_tab 상에 위젯을 배치할 수 있다．

QTabWidget은 탭이 변경되었을 때 , 시그널 이벤트를 처리할 수 있는 인터페이스를 제공한다．

widget.h

          a七e slots :
          \/Oid currentTab ( mnt index) ;
          void CUrre


widget.cp口

11       ""“七（tab, 땅쁘(currentC．卿艸in디）
                       bLU'
                          l'   (  )J;
                                      , 七his,
                               (current’   上’
                                                aL) lilt)



currentChanged(int) 시그널 이벤트 함수는 탭이 변경되었을 때, 발생하는 시그널 이벤트이다. 탭이 변
경되면 connect( ) 함수를 사용해 연결한 슬롯함수는 전달받은 m1lt 값을 참조해 몇 번째1 탭으로 변경되었
는지 확인할 수 있다．


                                                                                              1_Basic Widget 77


===== PAGE 79 =====
  void Widget: :currentTab (int index)
  {
       qDebug( 1'Current Tab : %d", index) ;
  }




                              丘甘 마owser

               QTab뻐的et 口
  Current Tab : l
  Current Tab : D
  D : \Qtproje그t\ QTa刑idget
  e工ited 늬ith code 0
                                 Button 2
  Starting  D: \QtProject\
  \QTabWidget .e工e. . .
  Current Tab = 1
                                 Button 3
  Current Tab : 0
  口｝rrent  Tab : 1
  Current Tab : 0


（그림） QlabWk均et 시그널 이벤트 처리




      自i面UQTo이Bar와 （그Action
QTo「小町위젯은윈도우상에 톡먼也브왓르르으쏘편껜交揖 "카공한다·

 헤더 파일 :
 #include <QToolBar>
 孝include <QAc七ion>



QToolBar 위젯은 addAction( ) 멤버함수를 이용해 툴바 메뉴 버튼을 배치할 수 있다. 그리고 사용자가
단축키를 이용해 툴바 메뉴 버튼을 실행할 수 있는 인터페이스를 위해 setShortcut( ) 멤버함수를 제공
하며 짧은 설명과 같은 툴팁 기능도 제공한다．

 QToolBar *toolbar = new QToolBar (this) ;


 QA（그七ion 士a（北［2 ] ;


 act[ O} = new QAction(Qlcon( " :resources/ browser.png ") , "Browser ", this) ;
 act[ 1] = new QAction(Qlcon ( " :resources/ calendar.png") , "calendar ", this) ;


 act[ O] ->setShortcut (Qt: :Key1Control I Qt: :KeymE) ;
 act[ O] ->setToolTip ( "This is a ToolTip. ") ;


 for (int i = 0 ; i < 2 ; i-t-+)
     toolbar->ad姐ction(act[ i] );


QAction 위젯은 QToolBar에 배치할 툴바 메뉴 버튼이다． QAction 위젯을 QToolBar 위젯에 등록하
기 위해 addAction( ) 멤버함수를 사용할 수 있다．


78 CHAPTER 03_ GU1 설계와 제작


===== PAGE 80 =====
                                                      口 回心



                1 editcr !




（그림） QTooIBar 위젯



그림에서 보는 것과 같이 QAction 메뉴 버튼의 아이콘만 보이게 하거나 아이콘과 버튼명을 같이 표시할
수 있도록 다음과 같은 상수 값을 제공한다．


（가：:To이跏ttorilcon아기y                         0            아이콘만 표시
Qt::ToolButtonTextOnly                       ]            버튼명만 표시
O口T이引B미tonTextBesid이con                      2            아이콘을 텍스트 안쪽에 표시
Qt::Tool ButtonTextUndericon                 3            아이콘을 텍스트 아래에 표시



표에서 명시한 스타일을 적용하기 위해서는 QToolBar 위젯의 setToolButtonStyle( ) 멤버함수를 사용
하면 된다．

 toolbar->setToolButtonStyle ( Qt: : ToolButtonTextBesidelcon) ;




  나／日r口wser   五姚ndar           >7 chat   ;       edit口r    j m訓

                                             i edtcr 1




（그림） QTo이Bar 위젯 스타일



 connect (act[ O] , SIGNAL(triggered() ), this,
                       SLOT (triggerl () ));


QToolBar 위젯은 툴바 상에 배치한 메뉴 버튼을 실행하기 위한 인터페이스로 triggered( ) 시그널 이벤
트를 제공한다. connect( ) 함수를 이용해 시그널 이벤트를 처리할 수 있다．




                                                                            1_Basic Widget 79


===== PAGE 81 =====
  void Widget: :triggerl ()
  {
          qDebug( "Tool Button 1 click. ") ;
  }



  却plicoti口n1그utput   ,'i + 中 b      "了H
   OSUder     1 QTabWidgei
                                           Bro나Ser   烈 ：引Inda:       mail
                                                                 加
                                                                 回
                                                                 ＝
  Startieg 0: \QtProject\ QTOOI$
  'a 어）11뇨r .exe. . .            }
  a舛indo나aKimBo出 : setSeometry =
  Reaulting geometry:     116x30+
  Tool Butt （코l 2 click ,        三
  Too]. But亡口｝l 3 ci工Ok.         !
  Tool Button 4 Click.
  T口O1 Butt口n 5 Click.
  Tool Bietton 4 click.




 （그림） QToolBar 시그널 이벤트 처리




斗4 幻.221 QWidget

 지금까지 살펴본 위젯은욘쁘쁘얀署붓貝쏘솔밭안크迎，型이다． 예를 들어 마우스， 키보드 혹은
 윈도우로부터 받은 이벤트를 QPus｝떠毗ton과 같은 위젯에서 사용할 수 있는 것도 QWidget으로부터
 상속받았기 때문어］ 가능하다．

 커스텀 위젯을 구현할 때에도 QWidget 클래스로부터 상속받아 구현할 수 있다. QWidget은 부모 윈도
 우인 동시에 Child 윈도일 수 있다. 헤더 파일상어］ 邸Vidget이 부모 윈도우인지, 혹은 자식 윈도우인지
 명시할 수 있다．

  半include <QtGui/Q寸idge七＞


  class Widge七 : pubi뇨그 QWidge七
  {
          Q OBJECT

  public:
          Widge七（QWidget; 虹厄rent = 0) ;
          -Widget () ;
      ;



 쁘쁘뜨그쁘르些二으괏孕안곡a匙깐갔交坦분毛윌돗呈완只뜨L았브恥剋剋읜으팟好겯엎된
 다. 여기서는 Parei此를 0으로 명시했지만 명시하지 않을 경우 0값이 디폴트로 설정된다．




 80 CHAPTER 03_ GUI 설계와 제작


===== PAGE 82 =====
                     玉1m n n1 nh11 Jm r41 fl il卜m,L

 O日roupBox
 pa,ent widget -                                                        --   QDateEdit
                   나Qate1          [21 Sep 2005                 ＝주r
                                                                             child widget

                   d1蜘e:          ] 01 3000円4                   4令＋叫HH O키meEd仕
                                                                             Chi넙 widget
 0Labei            ILocation:I Meeting room 1                         4-Hm 아JneEd什
 thiId 岫dn蹴S                                                                 i11七二1尸1 11 mH八八冬
                                                                             납1 H艮J !11\J납口t

                     Developer meeting
                     A brief meeting to check the status
                     肝 each pr이ect a the deve佃pme！比                    !


                     department.
 OTex匹dit
 짢川d widget


                                                                        三

                                                                 -J
（그림） QWidg이의 Parent Widget2F Child Widget



그림에서 보는 것과 같이 QGrol叩Box는 Parent Widget이며 QLabel, QTextEdit 등은 Parent 위젯
의 Child 위젯이다. 이와 같이 印Widget으로부터 상속받아 구현된 위젯들은 Parent 혹은 Child인지 구
분할 수 있도록 Parent의 값을 통해 구분할 수 있다．

QWidget은 이벤트 처리와 Pair此를 이용하기 위해1 다음과 같은 헤더 파일을 include 해야 한다．

 헤더 파일 :
 孝mlci나de <QPain七er>
 #include <QtEvents>



. .,.ow，的，,::,,나，
                Event(Q미，
                        ntE. 幣甘m．茫，印rotectedI
마우스나 키보드 등 이벤트가 발생했을 때 , 邸Widget 영역을 Paint 하거나 Repaint 이벤트가 발생 시
호출할 수 있는 기능을 제공하는 함수이다. 이 함수는 Virtual 함수로써 邸Widget 클래스의 멤버함수로
구현되어 있으므로 재정의해 사용할 수 있다．


  헤더 파일
 protected:
       virtual      void pairitEvent (QPaintEvent *event) ;

  소스 파일

 void Widget: :paintEvent (OPaintEvent *event)
 {
       Q UNUSED (event) ;
       QString img full                   name;


       QPainter painter (this) ;


       img full       name = gString ( ' %1/ %2 " ).arg(uresourcesfl)
                                                                 .arg( '1browser.png") ;


       Qilnage image (img full                        name) ;


                                                                                                 1_Basic Widget 81


===== PAGE 83 =====
     painter. drawPixmap (0, 0,
               QPixmap: :fromlmage (i咀ge. scaled(100, 100,
                                   Qt: : IgnoreAspectRatio,
                                   Qt: :SmoothTransformation) ));


     painter. end() ;
 }




（그림） QWidg이의 paintEvent



그림에서 보는 것과 같이 QWidget 클래스 기반의 윈도우가 생성되면 paintEvent( ) 이벤트를 호출한
다. 邸Widget 영역을 다시 그려야 하는 경우 paint( ）와 repaint( ) 멤버함수를 사용하면 paintEvent()
함수가 호출된다. QUNUSED( ) 함수는 선언한 함수나 데이터 변수를 사용하지 않으면 \Warning 메시
지를 출력하지 않도록 처리하기 위해1 사용하는 함수이다．


1void QWidget::resizeEvent(QResizeEvent *event) [virtual protected]
QWidget의 크기를 조절할 때 사용하는 멤버함수이며 , resize( ) 멤버함수를 호출하면 resizeEver此가
호출된다. 이 함수는 virtual 함수로써 재정의 할 수 있다．


 헤더 파일
 pro七ec七ed:
     virtual   void resizeEvent (QResizeEvent *event) .

 소스 파일

 void Widget: :resizeEvent (QResizeEvent *event)
 {
     QtJNtJSED(event) ;


     qDebug( " [Resize Event call] ") ;
     qDebug( "width : %d, height : %d", this-'>widthU, this- >height () );
 }




82 CHAPTER 03_ GUI 설계와 제작


===== PAGE 84 =====
 且p口licati口p ')ijtpijt

 嗔靴磁姦才，蒲， a배dget 口
 width : 300, height : 200
 (Resize Event calli
 width : 300, height : 200
 (Mouse Pressi x, y : 64 , 43
 (Mouse Relea日e] 묘r y : 64 , 43
 (Mouse Presal x, y : 51 , 63
 (Mou日e Release] 乂r y : 51 , 6?
 Key Press Event.
 Key Press 心pen七 .


（그림） QWidg이의 resizeEvent



0mousePressEvent, mouseReeaseEvent, moveEvent, mouseDoubleClickEvent
帥Widget 상에서 마우스의 Press, Release, Move 이벤트가 발생하면 구현된 Virtual 멤버함수를 통해1
이벤트를 재정의 할 수 있다．

mousel노essEver此는 마우스 버튼이 눌러졌을 때1 발생하고, mousel扼leaseEvei此는 마우스를 눌렀다
떼었을 때1 발생한다. 그리고 moveEve砒는 마우스를 누른 상태에서 움직였을 때 발생하는 이벤트 멤버
함수이다．

 헤더 파일
 br。
   tected'
        virtual          void mousePressEven七（QMouse丑yen七 出even七）;
                                                                             !\




        virtual          void mouseReleaseEvent (QMouseEvent *event) ;
        virtual          void mouseDoubleClickEvent (QMouseEvent *event) ;
        virtual          void mouseMoveEvent (QMouseEvent * event) ;

 소스 파일

 void Widget: :mousePressEvent (QMouseEvent *event)
 {
        Q UNUSED(event) ;


        qDebug ( " [Mouse Press] x, y : %d , %d ", this- >x () , this- >y () );
 I

 void Widget: :mouseReleaseEvent (QMouseEvent *event)
 {
        Q UNUSED(event) ;
        qDebug ( " [Mouse Release] x, y : %d , %d ", this- >x ( ), this- >y () );
 I

 void Widget: :mouseDoubleClickEvent (QMouseEvent *event)
 {
        Q UNUSED(event) ;
        qDebug( " [Mouse Double Click] x, y : %d , %d ", this- >xU, this- >y () );
 I                                                                                               0


                                                                                    1 Basic Widget 83


===== PAGE 85 =====
void Widget: :mouseMoveEvent ( QMouseEvent *event)
{
     QUNUSED(event) ;
     qDebug( n[ Mouse Move] x, y : %d , %d " r this- >x ( ), this- >y () );




이외어炡 마우스의 휠(WHELL) 이벤트가 발생했을 때, 처리하기 위해 whee出vent( ) 멤버함수를 제공
한다. 마우스의 위치가 邸7/idget 영역 안으로 들어올 때 , 혹은 영역 밖으로 위치가 변경되면 enter-
Event(), leaveEvent( ) 멤버함수를 사용할 수 있다．

그리고 QWidget이 close( ) 멤버함수에 의해 닫힐 때 , closeEvent( ) 멤버함수를 통해 재정의 할 수 있다．


1KeyPressEvent( ), KeyReleaseEvent( ), focuslnEvent( ), focus0utEvent( )
QWidget 영역에서 키보드 이벤트가 발생하면 KeyPressEvent( ) 멤버함수를 재정의해 키보드 이벤트
를 처리할 수 있다. 如cuslnEvent( ）는 QWidget상에 키보드 포커스를 얻을 때 발생하는 이벤트이고
focusOutEvent( ）는 키보드 포커스를 잃었을 때 발생하는 함수이다．


 헤더 파일

protected:
     virtual    void keyPressEvent (QKeyEvent *event) ;
     virtual    void keyReleaseEvent (QKeyEvent *event) ;
     virtual    void focuslnEvent (QFocusEvent *event) ;
     virtual    void focusOutEvent (QFocusEvent *event) ;

 소스 파일

void Widget: :keyPressEvent (QKeyEvent *event)
 {
     QUNUSED(event) ;
     qDebug( "Key Press Event. ") ;


     switch(event->key () )
     {
     case Qt: :KeyA :


         if (event->modifiers () == true)
             qDebug ( "A") ;
         else
                qDebug( " a") ;


         qDebug ( " %x ", event->key () );


     break;


     default:
     break;
     }                                                                        O

84 CHAPTER 03_ GUI 설계와 제작


===== PAGE 86 =====
}

void Widget: :keyReleaseEvent (QKeyEvent *event)
{
    Q UNUSED (event) ;
    qDebug( "Key Release Event. " ) ;
}

void Widget: :focuslnEvent (QFocusEvent *event)
{
    Q UNUSED (event) ;
    qDebug ( "focus InEvent Event. ") ;
}

void Widget: :focusoutEvent (QFocusEvent *event)
{
    Q UNUSED (event) ;
    qDebug( " focusOutEvent Event. ") ;
}


키보드 이벤트가 발생하면 키보드에서 어떤 키 이벤트가 발생했는지 혹은 區拉｝동시에 눌러진 키가 있
는지 확인하기 위해서 Qt::key 상수를 제공한다. Qt::key 상수에 정의된 값은 Qt Online 도움말이나
Qt Creator의 도움말 기능을 통해 자세히 살펴볼 수 있다．

지금까지 살펴본 멤버함수 이외에도 QWidget은 다양한 함수를 제공한다. 어플리케이션 개발 시 필요한
기능을 추가해야 한다면 커스텀 위젯을 통해 새로운 기능을 추가할 수 있다．



           QTabBar

       旦l望크廻론긋쁘센샷量也t쁘甦브컨竺］다· QTabBa『는 사용가기
映些姮坐번찢르，
간단하며 미리 정의된 도형 중 하나를 사용해 탭을 그릴 수 있으며 탭을 선택했을 때 시그널 이벤트를 발
생시킬 수 있다. 또한 Qt는 QTabBar와 비슷한 기능으로 QTabWidget을 제공한다．

헤더 파일 :
孝mnci끄de <QTabBar>


각 탭은 텍스트를 표현할 수 있으며 탭에 사용할 아이콘을 옵션으로 사용할 수 있다. 탭의 텍스트는
setTabText( ) 함수를 이용해 텍스트를 설정하고 아이콘은 setTablcon( ) 함수를 사용하면 된다. 그리
고 탭어］ 대한 툴팁 기눙을 제공하기 위해 setTabToolTip( ) 함수를 사용할 수 있다．

각 탭에 표시되는 텍스트가 구별되게 컬러 지정이 가능하다. 탭의 텍스트를 지정하기 위해 setTabText
C아or( ) 함수를 사용하면 된다．

QTabBar는 이미 정의된 도형을 이용하여 탭의 모양을 변경할 수 있는 기능을 제공한다. 예를 들어 모서


                                                         ] 日a미c Widget 85


===== PAGE 87 =====
리가 둥근 형태의 탭이나 탭의 왼쪽 모서리만 둥글게 표현한 도형을 이용할 수 있는 기능을 제공하며
setShape( ) 함수를 이용해 지정할 수 있다. enum 타입으로 정의된 탭 모양은 다음과 같다．

Constant                          Value   Description
QTabBar::RoundedNorth             0       디폴트 모양
QTabBar::RoundedSouth             ]       페이지 아래쪽이 둥근 형태
QTabBar::RoundedWest              2       페이지의 왼쪽 부분이 둥근 형태
QTabBar::RoundedEast              3       페이지의 오른쪽 부분이 둥근 형태
QTabBar::TriangularNorth          4       삼각형 모양
QTabBar::Triangu冶rSo미h            5       엑셀 스프레드시트에서 사용하는 형태와 비슷한 삼각형
QTabBar::Triangu冶r\사est           6       페이지의 왼쪽 부분이 삼각형 모양
QTabBar::TriangularEast           7       페이지의 오른쪽 부분이 삼각형 모양


QTabBar 위젯은 QTabWidget과 사용 방법이 유사하다. addTab( ) 함수를 통해 탭을 추가할 수 있다．

 QTabBar *tab = new QTabBar (this) ;


 tab->add.Tab ( 'Browser '1 ) ;
 tab->addTab ( "User ") ;
 tab->addTab( "Application") ;



사용자가 선택한 탭을 클릭했을 때, 시그널 이벤트를 발생시키기 위해 currentChanged( ) 시그널 함수
를 사용하면 된다．

 connect (tab, SIGN스L (currentChanged(int) ), this,
               SLOT (currentTab (int) ));




     日n그뇨'1日Br   User   ! 却帥:ation 1




（그림） OTabBar 위젯




86 CHAPTER 03_ GUI 설계와 제작


===== PAGE 88 =====
      1.24 QToolBox
QToolbox 클래스 위젯은 위젯 아이템들을 탭 기반 컬럼 형태로 GI끄를 제공하는 위젯이다. 여러 개의 세
로 방향의 탭들을 배치할 수 있으며 사용자가 특정 탭을 선택하면 해당 탭에 속한 위젯이 나타나게 된다．

 헤더 파일：
 #include <QToolBox>



각 탭의 아이템은 텍스트를 지정할 수 있으며 옵션으로 아이콘을 사용할 수 있다. 아이템의 텍스트는
itemText( ) 함수를 이용해 QString 타입으로 리턴값을 얻을 수 있으며 itemlcon( ) 함수를 이용해
Qlcon을 리턴받을 수 있다．

QToolBox 위젯상에 탭 아이템을 추가하기 위해 addltem( ) 함수를 사용하면 된다. addltem어］ 아이템
을 추가하기 위해 위젯을 추가할 수 있다．

   =new QTc均iBox（比i引 ;
   =new QHB炚Layou七（thi引 ;


上乂l七1=new QE七shBut；七on( "Da七aBase 놔 1 '' r七hi引 ;
but2=nei寸 QPushButton ( 'Ne七M江k 小 2 '' r七hi히 ;
but3=new QPushButton ( "Graphics - 3 ", this) ;


box->addltem(butl, "DataBase ") ;
box->addltem(but2, "Network ") ;
box->addltern(but3, "Graphics " ) ;


lay- >addwidget (box) ;
setLayout (lay) ;


탭에 등록한 아이템을 추가하거나 제거할 수 있는 함수를 제공한다. 아이템을 추가하기 위해서는
insertltem( ) 함수를 사용하면 된다. 반대로 아이템을 제거하기 위해 removeltem( ) 함수를 사용할 수
있다．

현재 아이템 위젯의 인덱스를 리턴받기 위해 currentlndex( ) 함수를 사용할 수 있다. 그리고 사용자가
탭을 알 수 있도록 시그널 이벤트를 제공한다. 사용자가 선택한 탭의 인덱스를 얻어오기 위해 current
Changed( ) 시그널 함수를 사용하면 된다．

connect (box, SIGNAL (currentChanged(int) ), this,
                 SLOT (changedTab (int) fl ;




                                                       1_Basic Widget 87


===== PAGE 89 =====
  Dat크Bas日

        Data日ase - ]



                                                            Crap비Cs日   }
  Net心巾

  Grap비CS



（그림） OToolBox 위젯




              QTo이Button
QToolButton 클래스는 사용자에 빠른 GUI 인터페이스를 제공하기 위한 목적으로 제공하는 위젯이다．
일반적으로 QToolBar 위젯상에서 사용된다．

 헤더 파일 :
 #include <QToolButton>


QToolButton 위젯은 텍스트로 표시할 수 있지만 일반적으로 아이콘을 사용해 위젯을 표시한다．


            好 kr       ,，今 武 也 확 !:1
（그림） QTooIBu卄on 위젯



QToo出毗ton의 아이콘은 Qlcon 클래스를 이용해 지정할 수 있다. 아이콘은 State어］ 따라 활성화된 상
태 혹은 비활성화된 상태로 표시할 수 있다. 만약 비활성화 상태에서는 버튼을 사용할 수 없다．

QToo出毗的n의 스타일을 지정할 수 있다. setToolButtonStyle( ) 함수를 이용하면 버튼의 스타일을
지정할 수 있다. 또한 setlConSize( ) 함수를 이용하면 아이콘의 크기를 지정할 수 있다．

 QToolBar *tool = new QToolBar (this) ;


 QToo] Button *button = new QToolButton;
 button->setlcon(Qlcon( '1 :resources/browser.png") );


 QToolButton *buttonl = new QToolButton;
 buttonl- >setlcon(Qlcon( 1' :resources/calendar.png") );


 QToolBut七on 火bu七七（Dn2 = new QToolBut土on;
 button2->setlcon(Qlcon( n :resources/chat.png") );


 tool- >addWidget (button) ;
 tool- >addwidget (buttoni) ;
 tool- >addSeparator ( );
 tool- >addWidget (button2) ;



88 CHAPTER 03. GUI 설계와 제작


===== PAGE 90 =====
QToolBar어］ QToolButton 위젯을 추가하기 위해 addWidget( ) 함수를 이용하면 아이템을 추가할 수
있다. 그리고 QToolButton 위젯 사이에 Separ毗아를 사용하고자 한다. addSeparator( ) 함수를 사용
하면 된다．

                         .口 回 m



（그림） OToolButton 위젯




                                                        1_Basic Widget 89


===== PAGE 91 =====
Qt 5 Programming




          2· 레이아웃

   難繫瑟 레이아웃은 윈도우 크기가 변경됨에 따라 배치한 위젯의 위치 또는 크기가 동적으로 변경될 수 있는 :71
          능을 제공한다. 이번 장에서는 아에서 제공하는 레이아웃 관련 AP를 사용하는 방법에 대해 알아보도
          록 하자．




지금까지 GI끄상에 위젯을 배치하기 위해 setGeometry( ）를 사용했다. 이 함수는 GUI상어］ 절대좌표를
이용해 위젯을 배치할 수 있다. 그러나 윈도우의 크기가 사용자에 의해1 동적으로 변경된다면 절대좌표로
배치한 위젯의 크기는 동적으로 변하지 않기 때문에 문제가 된다．

따라서 배치한 위젯의 윈도우 크기가 변경되면 동적으로 크기가 변경될 수 있도록 레이아웃을 제공한다．
레이아웃은 윈도우 크기에 따라 동적으로 위젯의 크기를 변경할 수 있는 것 이외에 레이아웃을 감추거나
표시하게 되면 레이아웃에 포함된 모든 위젯을 감추거나 표시할 수 있다．

이번 장에서는 레이아웃 클래스를 이용해 위젯을 배치하는 방법에 대해 살펴보도록 하자. 레이아웃은 위
젯을 세로 방향으로 배치 , 가로 방향으로 배치 혹은 바둑판과 같이 그리드 형태로 배치할 수 있는 인터페
이스를 제공한다．

레이아웃               설명
QHBoxLayout        위젯을 가로 방향으로 배치
QVBoxLayout        위젯을 세로 방향으로 배치
QGridLayout        위젯을 그리드 형태 스타일로 배치
QBoxLayout         위젯을 가로 방향으로 배치 혹은 세로 방향으로 배치할 수 있는 클래스로써 옵션을
                   사용하1 배치 방향을 결정할 수 있다．



표에서 나열한 레이아웃은 중첩해 사용할 수 있다. 예를 들어 상단은 가로 방향으로 위젯을 배치하고, 하
단은 배치할 경우 QVBoxLayout 상에 QHBoxLayout과 QVBoxLayout을 포함시 킬 수 있다．


0QHBoxLayout
QHBoxLayout은 위젯들을 가로 방향으로 배치할 수 있다. 윈도우의 크기가 변하면 위젯의 크기가 동적
으로 변경된다．




90 CHAPTER 03_ GUI 설계와 제작


===== PAGE 92 =====
 QHBoxLayout *hboxLayout = new QHBoxLayout (this) ;
 QPushBut七（>n 싸亢n[ 6] ;


 QS七ring b七nS七r[ 6] = eNe七Book ' ,              'Table七",         "Handse七1' r
                               1' Genivi" , "Smart人／'1 ,          "Vechile" };


 for (int     i   = 0 ; i < 6 ; i++)
 {
      l此nEil = new QPushBl그七七on (b七nS七r[ i} ) ;
      hboxLayou七->addWidge七 (b七n[ i ] ) ;



 setLayout ( hboxLayout) ;



                                                                  [ 口 1回 m
     N化nday        Tuesday   따日dnesday1   Thursday   1   Friday     [
（그림） QHBoxLayout



addWidget( ）는 위젯을 레이아웃에 추가하기 위한 멤버함수이다. 예제 코드에서 보는 것과 같이
QPushButton 위젯을 addWidget( ) 멤버함수를 이용해 추가할 수 있다. 레이아웃을 윈도우 상에 배치
하기 위해 QWidget의 setLayout( ) 멤버함수를 사용하면 위젯의 디폴트 레이아웃으로 지정할 수 있다．


簪QVBoxLayout
QVBoxLayot此을 사용하면 위젯을 세로 방향으로 배치할 수 있다. 사용방법은 앞서 다룬 QHBox
Layout과 동일하다．

 QVBoxLayout *vboxLayout = new QVBoxLayout (this) ;
 QPushBut七on 士＼ib七n[ 6 ] ;


 QString vbtnStr[ 3} = {"Movie",              "Drama",       "Animation"} ;


 for (int i       = 0 ; I < 3 ; i++)
 {
      vb七rs[ i]     = new QPushBut七on (vb七nS七r[ i] );
      vboxLayout->addWidget (vbtn[I] );
 }
 setLayout (vboxLayout) ;




                                                                                 2 레이아웃 91


===== PAGE 93 =====
（그림） QVBoxLayout



    eQGridLayout
 釵｝ridLayout은 바둑판과 같이 위젯을 그리드와 같은 스타일로 배치할 수 있다. 예를 들어 배치하고자
하는 위젯을 표와 같이 배치할 수 있으며 특정 행을 여러 셀로 나누거나 병합할 수 있다．

     QGridLayou七 火gridLayou七 口 new QGridLayou七（this) ;
     QPushBu七ton 火야此n[ 5] ;


     QString btnStr[ 6] = {"Monday ",         "Tuesday ", "Wednesday",
                                   "Thursday", "Friday ", "Saturday" };

     for (int i   = 0 ; i < 5 ; i++)
     {
         야此n[ i]     = ne＼寸 QPushBu七七on(gb七nStr[ i] ) ;



     gridLayout->addWidget (gbtn[ O] , 0, 0) ;
     gric江ayou七수addWidge七（gb七n[ 1} , 0, 1) ;
     gridLayot此수addWidge七（야光n[ 2] , 1, 0, 1, 2) ;
     gridLayout->addWidget (gbtn[ 3} , 2, 0) ;
     gridLayout->addWidget ( gbtn[4] , 2, 1) ;


     setLayout ( gridLayout) ;




'I크                         ｛口 回 km'
          卜4c,nday               Tues（抽1/

                     Wednesday              !

1         Thursday               Friday

t=                                              j


（그림） QGridLayout



QGridLayout을 이용해 위젯을 배치하기 위해 addWidget( ) 멤버함수를 사용한다. 첫 번째 인자는 행
(row）이고, 두 번째 인자는 열（col)이다. 그리고 오버라이딩된 addWidget( ) 멤버함수의 세 번째 인자는
병합할 행을, 네 번째 인자는 병합할 열을 지정할 수 있다．


92 CHAPTER 03_ GUI 설계와 제작


===== PAGE 94 =====
0 중첩 레이아웃 사용
위젯을 배치할 때 상단은 가로 방향으로, 중간은 세로 방향으로, 하단은 그리드 스타일로 배치해야 한다
면 한 가지 레이아웃만 사용해 표시할 수 없다. 따라서 지금까지 살펴본 QHBoxLayout,
QVBoxLayout 그리고 QGridLayout을 중첩해 사용할 수 있다．

레이아웃을 중첩해 사용하기 위해서는 Pare砒와 Child 클래스와 같이 윈도우에 등록할 디폴트 레이아웃
을 선언하고 디폴트 레이아웃의 addLayout( ) 멤버함수를 이용해 레이아웃을 중첩해 사용할 수 있다．

［而oxLayou七 *hboxLayou七 = new QHBoxLayou七（);
I     QVBoxLayout        new            () ;        *vboxLayout                           =                QVBoxLayout
!QGrlciLayout *gr1(Layout = new QurlciLayouto;


      QVBoxLayout *defaultLayout = new QVBoxLayout () ;


      defaultLayout->addLayout ( hboxLayout) ;
      defaultLayout->addLayout (vboxLayout) ;
      defaultLayout->addLayout ( gridLayout) ;


             setLayout ( defaultLayout) ;



뇨                                                                             :                                                             ［늬回甘叫

「                       Monday                 Tuesday 陟塑뜨쁘뇨 [ Thursday j L叫                                                                  ] i Saturday
                                                                                          Mo너e
 ;                                                                                        Drama
                                                                                       出슈nm訓on

                    I                          Monday                                                                              Tuesday
                                                                                        누iednes day
                                               Thursday                                                                            Friday
 七小                     m! m     h山   小   如H    +                 m   小   如小m4a小小mm=          ,   ,   n艸                 山   小n寸        1心a                  /




（그림） 중첩 레이아웃



이전 레이아웃은 레이아웃 클래스 선언 시 생성자 함수에 this를 사용해 부모 클래스를 명시했지만 인자
가 없는 오버라이딩된 생성자 함수를 사용할 수 있다. 이 생성자 함수는 addLayout( ) 멤버함수를 사용
 해 레이아웃을 추가할 때 사용하면 중첩된 레이아웃을 구성할 수 있다．

 윈도우 크기가 변경되면 동적으로 위젯의 크기가 변경될 수 있도록 레이아웃을 사용하는 방법에 대해 살
 펴보았다. 어플리케이션 개발 시 레이아웃은 예제와 달리 소스 코드가 상당히 복잡해질 수 있다. 하지만
 이번 장에서 살펴본 레이아웃을 사용함으로써 어플리케이션 사용자에게는 동적인 크기 변환에 따른 인터
 렉티브한 GUI 인터페이스를 제공할 수 있다．




                                                                                                                                                                 2 레이아웃 93


                                                                                                                                                                             1


===== PAGE 95 =====
                           n
    Qt 5 Programming




                                  3// Advanced Widget
    嚮難熙照蘚難韓難小
                                  0는 GU를 설계 또는 디자인하기 위해 QPushBu卄on, OLabel 등과 같은 단순한 위젯을 제공할 뿐만
                                  아니라 여러 위젯의 기능이 하나의 위젯으로 동작할 수 있는 Advanced Widget 클래스를 제공한다. 예
                                  를 들어 달력을 표시하기 위한 00졔endarWidget과 하나의 위젯에 여러 위젯 기능이 통합된 위젯을 저f
                                  공한다. 따라서 이번 단원에서 아에서 제공하는 Advanced Widget（川 대해 살펴보도록 하자．




    Advanced Widget 클래스는 Qt에서 제공하는 여러 가지의 Basic Widget들을 하나의 복합된 위젯으로
                                                                                              ＼八U뇨小小느八．/＼入／ \bd／八J

    제공하는 위젯을 말한다．


                         Name 1                                 FebruaryV 2009




          申
          ；田i
            田i田
              ：由 田 由 由 ＜
                     Ii:그묘나CKo..                           Sun Mon Tue Wed Thu    Fri   Sat
                     口 cdrc                   F拒
                                              F拒      5     25 26 27 28 29        30    31
                     口 由aruge瓦．
                     口 database               F拒      6     1   2   3   4   5     6      7
                     口 南C妃心奴                  File                   10   11   12D14
                   口 eve                      File     8   15   16   17   18   19 20 21
                     口 fon也                   File
                                                       9   22   23   24   25   26 27 28
                       11＝그1 卄1<fmn口r         Pu口 쯔
                                        小 ‘

                                                >     10   1     2    3    4   5   6  7

    （그림） Advanced Widget



        위젯                                    설명
    00이umnVk키사                                卜加del/View 기반으로 구현한 컬럼뷰 위젯
    oDataWidgetMapper                         위젯과 卜加de 데이터를 연결하여 제공하기 위한 Ma口ping 클래스 위젯
    （긔_ist View                               리스트 형태의 뷰 위젯
    OTableView                                Model/View 기반으로 구현된 테이블뷰 위젯
    OTreeView                                 Model/View 기반으로 구현된 트리뷰 위젯
    QDeskto이Vidget                              하나의 그래픽 카드로 가상의 여러 711 데스크탑 화면을 활용하기 위해 제공
                                              ? 되는 위젯
    QUndoVi아V                                 Undo stack의 내용을 리스트 형태의 위젯에 표시하1 출력하는 기능을 제공
                                              하는 위젯
    OCalendarWidget                           사용자가 선택한 날짜（Month 단위）를 달력 형태로 표시하는 위젯
    QMacCocoa＼기ewCon怡iner                     Cocoa 미ew와 같은 클래스를 Wr야갸기ng하7! 위하1 사용하는 Mac OS x
                                              룰 위한 위젯
    QMacNativeWidget                          ot 구성 방식에 따라 Cocoa 계층구조에 （기 위젯을 넣는 방법을 제공하는
                                              위젯




    94 CHAPTER 03_ GUI 설계와 제작


卜


===== PAGE 96 =====
            Qc이umn＼기ew
QColumnView 클래스는 Model/View 데이터 기반으로 컬럼 단위 리스트 위젯을 제공한다. 컬럼 단위
로 리스트를 제공하는 QC아umnView 클래스는 Qt어］서 제공하는요些얀껸쁘｝쁘쁘쁘르랫스엔坐旦
졀브哭쁘긴스量크共竺므땐쁘M四민是랫슨롯분貝丑샐是꼿으翅낏；塑月쁘量푠신가기 위
한 구현 방법을 제공한다．

 헤더 파일：
 #include <QColurnnView>




  Name                        上 F侄St Name       r 小 Sri기th
  Ad山e5S                 ,      La攷 Name        +




（그림） OO이umn＼기이V 위젯



그림에서 보는 것과 같이 QC아umnView 클래스는 model人扼w 기반의 클래스 위젯이다. 그렇기 때문
에 model 관련 클래스로 데이터를 가공하고 QC이umnView 클래스의 setModel( ) 함수를 이용해
Model 인스턴스를 지정하면 된다．

 QStandardlternNodel *model = new QStandardltemModel;


 QStandardltem *name = new QStandardltem( "Name ") ;
 QStandardltem *fjrstName = new QStandardltem( "First Name") ;
 QStandardltem *lastName = new QStandardltem( "Last Name ") ;


 name->appendRow(firstName) ;
 name->appendRow ( lastName) ;
 model->appendRow ( name) ;


QStandardltemModel 클래스는 model 기반의 데이터를 가공하는데 사용한다. model 인스턴스에 데
이터를 삽입 시 생성자를 사용할 수 있다. firstName과 lastName은 name 인스턴스의 하위에 등록하
면 그림에서 보는 것과 같이 name 인스턴스 하위 데이터 항목으로 삽입된다．

 QStandardltem *john = new QStandard工tem( "John") ;
 QStandardltem *smjth = new QStandardltem( "Smith") ;


 firstN帥e수appendRow ( j야in) ;
 lastName->appendRow(smith) ;



                                                                 3_Advanced Widget   95


===== PAGE 97 =====
加hn 인스턴스는 firstName 인스턴스 하위에， smith 인스턴스는 lastName 인스턴스 하위에 삽입한다．

QStandardltem *address = new QStandardltem( "Address ") ;
QStandardltem * street = new QStandard工tem( "Street ") ;
QStandardltem *city = new QStandardltem( "City ") ;
QStandardltem *state = new QStandardltem( "State ") ;
QStandardltem *country = new QStandardltem( "Country") ;


address->appendRow( Street) ;
address->appendRow(city) ;
address->appendRow ( state) ;
address->appen娘ow(country) ;
model->appendRow ( address) ;


QColumnView *colulpjlVjew = new QColumnView;
co1UmnView->setMode1(model) ;



Street, City, State 그리고 Cou砒ry는 address 인스턴스에 등록하고, 마지막에 model 기반 데이터
최상위 항목에 위치할 수 있도록 model 인스턴스에 appendRow( ) 함수를 이용해 등록한 다음 column
小View 클래스의 setModel을 이용해 등록하면 그림에서 보는 것과 같은 구조로 위젯을 사용할 수 있다．



     3.2 j QDataWidgetMapper

QDataWidgetMapper는 model 데이터와 위젯 사이를 Mapping 할 수 있는 기능을 제공한다. 예를 들
어 QCombox나 QListView의 mod이에 있는 데이터를 Mapping 시켜 놓은 상태에서 model에서 제공
하는 pervious와 next 관련 함수를 이용해 데이터를 이동하면 위젯에 표시한 데이터도 자동으로 위치가
변환된다．

헤더 파일：
#include <QDataWidgetMapper>


model은 모든 데이터에 현재 인펙스를 가지고 있다. 따라서 인덱스를 기반으로 각 위젯에 표시된 데이터를
변환시키기 위해1model 데이터에 인텍스가 이동되면 시그널 이벤트를 사용해 데이터를 이동할 수 있다．

QStringList items;
items << tr ( 'Home") << tr ( "Work") << tr ( "Other ") ;
typeModel = new QStringListModel (items, this) ;


model = new QStandardltemModel(5, 3, this) ;
QStringList names;
names << "Alice " << "Bob" << "Carol" << "Donald" << "Emma";
QStringList addresses;
addresses << "<qt>123 Main Street<br/ >Market Town</qt>"
        << "<qt>PO Box 32<br/ >Mail Handling Service "
           "<brl>Service City</qt>"                               0

96 CHAPTER 03_ GUI 설계와 제작


===== PAGE 98 =====
          << "<qt>The Lighthouse<br/ >Remote Island</qt>n
          << "<qt>47338 Park Avenue<br/ >Big City< /qt>"
          << "<qt>Research Station<br/>Base Camp<br/ >Big Mountain</qt> ";
 QStringList types;
 types << "0 " << " 1" << "2 ' << "0 '1 << "2 '1 ;



코드에서 보는 것과 같이 model 인스턴스어］ 데이터를 삽입한다. 데이터 삽입이 완료되면 setltem( ) 함
수를 이용해 열, 행 , 그리고 데이터를 인자로 지정한다．

 mapper = new QDataWidgetMapper (this) ;
 mapper->setModel (model) ;
 mapper->addNapping(nanteEdit, 0) ;
 mapper->addNapping(addressEdit, 1) ;
 mapper->addMapping (typeComboBox, 2, "currentlndex1' ) ;

 connect (previousButton, SIGNAL (clicked() ),
          mapper, SLOT (toPrevious () ));
 connect (nextButton, SIGNAL(clicked() ),
          mapper, SLOT (toNext () ));
 connect (mapper, SIGNAL (currentlndexChanged(int) ),
          this, SLOT ( updateButtons ( int) ));



nameEdit 위젯은 QLineEdit 위젯, addressEdit는 QTextEdit 위젯 그리고 typeComboBox는
QComboBox 위젯에 데이터 Mappir培을 한다. addMapping( ) 함수를 이용해 위젯 八4apping이 완료
되면 시그널을 발생시켜 model 데이터의 현재 index가 변환 시 위젯 데이터가 변환될 수 있도록 시그널
어］ toPrevious( ) 슬롯함수와 toNext( ) 슬롯함수를 연결한다．

 刃 D이텍；ate＼幀dget Mapper                卜＝ 1回 km
  Name:    B먀1

  Address: P0 Box 32                         Next
           Mail Handling Service
           Ser너ce City




  Type:    ／幻rk


（그림） QDataWidgetMapper 클래스 위젯




                                                                        3_Advanced Widget 97


===== PAGE 99 =====
           ODesktopWidget
 QDesktopWidget 클래스는 스크린의 정보를 액세스하기 위한 기능을 제공한다. 어플리케이션을 개발하
는 시스템의 디스플레이스의 물리적인 그래픽카드와 같은 층을 가상의 멀티 디스플레이로 구성하여 하나
 의 가상 디스플레이를 구성할 수 있다. 또한 여러 개의 디스플레이를 논리적인 영역으로 구분할 수 있다．
따라사욘匙브雙0쁘뵨翌르쁘슷立간살읜뽀크昱므슨置叱遇쳔본量몬긴운竺갓늪量 제공한다·
 헤더 파일 :
 #include <QDesktopWidget>


QDesktopWidget 클래스는 Qt를 사용하여 어플리케이션 위젯이 위치한 디스플레이상의 위치 정보를
얻기 위채 screenGeometry( ) 함수를 제공한다． 또한
                       안퓰쁘띤塑多坐矣二느쓰L쁘크스플
덴，"］를 사용O生브쁘 단스量坐造二쓰곳多七그쁘熙뜨쁘雙三론丑틴員二世할 수 있다·
screenCount 프로피티는 스크린의 개수가 변경될 때 screen（그ountChanged( ) 시그널 함수에 의해 리
턴값을 screenCount어］ 저장한다. 또한 위젯이 위치한 스크린 번호를 얻어오기 위해 screenNumber()
함수를 사용할 수 있다. 그리고 스크린상에 특정 위치 영역에 위젯을 배치할 수 있는지 정보를 얻기 위해
availableGeometry( ) 함수를 사용할 수 있다．

이번에 살펴볼 예제는 위젯상에 드로잉 기능을 제공하는 QPainter 클래스를 이용해 이미지를 렌더링하
고 QDesktopWidget 클래스를 이용해 위젯의 크기를 참조해1 이미지를 확대／축소 기능을 제공하는 방법
어］ 대해 알아보도록 하자．




（그림） QDeskto口Widget을 이용한 확대／축소 예제



그림에서 보는 것과 같이 이미지를 위젯상에 렌더링 하여 오른쪽 QSlider 위젯의 값이 변경될 때 , 위젯
의 크기를 변경하는 어플리케이션 위젯이다．




98 CHAPTER 03_ GUI 설계와 제작


===== PAGE 100 =====
QHBOXLayOU七 出layou七 = new QHBoxLayou七；


canvas = new gwidget;
slider = new QSlider;
slider- >setMinimum( 0) ;
slider- >setMaximum( 100) ;
slider- >setValue(50) ;


layout->addWidget (canvas) ;
layout->addwidget (slider) ;


setLayout (layout) ;


if (! pixmap.load( " :/resources/ fish. png") )


     qDebug( ) << "Fatal error: Unable to load image ";
     e幼上 (- 1 ) ;



connect (slider,    SIGNAL (valueChanged(int) ),
          SLOT (setZoom(int) fl ;



slider 인스턴스는 QSlider 위젯이며 , slider 인스턴스의 값이 변경될 때 valueChanged( ) 시그널 함수
이벤트가 뱝생한다. 시그널을 발생하면 이미지의 확대 축소 기능을 처리하는 setZoom( ) 슬롯함수가 이
벤트를 처리한다．

zoom = (qreal) (50+new zoom) I      50;
pixels = pi玎陋p.wid比（) 出 zoom;


QDesktopWidget desk;
p足width = desk.width() I pixels;
p乂 height = desk. heigh七（ ) / pixel司
mm width = pxwidth * 17. 9;
mm height = p乂血eight; 火 17. 9;


qDebug() << "Zoom: " << zoom;
qDebug() << "desk.width外｛:" << desk.widthMN() ;
qoebug() << "pxwidth:       " << pxwidth;
qDebu引 ) << "p乂上eight: '1 << p乂上eight;
qDebug() << "mm_width: " << mm_width;
qDebug() << "mm_height: " << mm_height;


repaint () ;



확대／축소에 따라 이미지를 렌더링 하기 위한 비율을 꼐산하기 위해 px_widget, pxheight, mm
w奴th 그리고 mm height 프로퍼티에 확대／축소 비율 크기를 계산해 볼 수 있다. zoom 프로퍼티에 이
미지 확대／축소에 대한 비율을 계산하고 마지막 豆；
                           ;;;t( ) 함수를 호출한다． 이 함수를 호출하면


                                                          3_Advanced Widget   99


===== PAGE 101 =====
QPainter 클래스의 재정의 함수인 paintEvent( ) 함수가 실행된다．

paintEvent( ) 함수에서 scale( ) 함수를 사용해 이미지 크기 비율을 참조한다. drawPixmap( ) 함수가
호출되면 비율이 적용된 이미지를 위젯에 렌더링한다．




     乙QDaa놔녑g叭Ma마mr
    Zoom:    a 口 44
    de4k. wtdbhMMe 544
    pxwidthe        5. 78923
    p工 heighb:       1. 00644
    mmw工dbhe        32. 0272
    n皿 hehghb:       16.01已




（그림） 이미지 확대／축소에 따른 디버깅 메시지




                           QCalenda rWidget

QCalendarWidget 위젯은 시스템 시간의 현재艮慢 브깐爻깁建읏롯          력 스타일의 （표JI 인터페이스
를 제공하는 위젯이다. 현재 시간을 기반으로 달력횰立치하거나 멤버함수를 이용해 표시할 년／월을 설정
할 수 있다．

1     카더 파익：
    莎inc上uce <（求a上enclarw끄3get>




        일 뒬 화 수 목 금 토
      1 30 31 1 2 3 4 5
      2 6 7 8 9 10 11 12
    t
      3 13 14 15 16 17 18 19
      4 20922 23 24 25 26
      5 2728293031 1 2
      6 3 4 5 6 7 8 c


（그림） OCalendarWidget



이 위젯은 날짜를 마우스와 키보드로 이동할 수 있으며 위젯에서 선택한 날짜의 정보를 얻어오기 위해
selectedDate( ) 멤버함수를 사용할 수 있다. 그리고 현재 표시된 월의 시작일과 마지막 일의 정보를
minimumDate(）와 ma虹mumDate( ) 프로퍼티를 이용해 정보를 얻어올 수 있다．

그림에서 보는 것과 같이 일을 표시하는 셀의 경계가 없지만 Border Line을 표시할 수 있는 멤버함수를


100          CHAPTER 03_ GUI 설계와 제작


===== PAGE 102 =====
제공한다. 이 밖에도 사용자 이벤트를 처리하기 위한 시그널 이벤트를 제공하며 , 달력 GUI 인터페이스어］
필요한 다양한 멤버함수와 프로피티를 제공한다．

 QCalendarWidget *calendar = new QCalendarWidget (this) ;
 calendar->setGridVisible (true) ;




                   r= l 回 m凸너"

                        목 금 토
      :1       1    2   3 4 5
           7   8    9 10 11 i:
      13 14 15 16 17 18 19
      20 回122 23 24 25 16
      27 28 29 30 31 1
         乙 5 . 6 7 8


（그림） Qc졔endarWidget


QCalendarWidget을 선언하면 현재 날짜의 년／월 정보를 얻어와 GUI 인터페이스를 제공한다. 그림과
같이 시작일은 1일부터 29일까지 표시하거나 특정 범위의 시작일과 마지막 일을 다음 그림과 같이 표시
할 수 있다．

 calendar->setMinhi씨nDate (QDate (2014孕夕4, 18) )
 calendar->setMaxim끄jlDate (QDate (2014, 4, 22) );




    일 뉠 호｝ 수 목 금 토                  일 쉴 화 수 목 금 토
  1 3031 1 2 3 4 5               14 30 31 1 2 3 4 5
  2   6    7   8    9 10 11 12   15 6   7   8   9 10 11 12
  3 13 14 15 16 17 18 19         16 13 14 15 16 17919
  4 20922 23 24 25 26            1720212223242526
  5 2728 29 30 31 1 2            1827282930 1           2   3
  6 3 二 5 6 7 8 1                19 2   5   r   叫   8   9 10


（그림） 범위 지정



setMinimumDate( ）와 set八4aximumDate( ）는 시작일과 마지막 일을 설정할 수 있으며 , 현재 설정된
시작일과 마지막 일의 날짜 정보를 얻어오기 위해 minimumDate( ）와 maximumDate( ) 멤버함수를
사용할 수 있다．

사용자가 QCalendarWidget 영역에서 Click 시그널 이벤트를 처리할 수 있으며 , 날짜가 선택되면
selectionChanged( ) 시그널 이벤트 함수를 슬롯함수와 연결할 수 있다. QCalendarWidget의 헤더라
인 표시 스타일을 반경하기 위해 다음과 같은 상수를 제공한다．



                                                                3_Advanced Widget 101


===== PAGE 103 =====
enum QCalendarWidget::HorizontalHeaderFormat
상수                                        값    설명
QCalendarWidget::SingleLetterDayNames     ]    요일을 ］문자로 표시한다．
                                               (예 Monday -> M)
QCaiendarWidget::ShortDayNames            2    짧은 요일은 표시 스타일로 표시한다．
                                               (（계 Monday 寸二＞ Mon)
oCalendarWidget::LongDayNames             3    요일을 완전한 단어 스타일로 표시한다．
                                               （예 Monday)
QCalendarWidget::NoHorizontalHeader       0    가로 헤더라인을 표시하지 않는다．


앞의 표에서 명시한 상수값을 setHorizontalHeaderFormat( ) 멤버함수를 통해 사용할 수 있다. 그리
고 사용자가 달력의 날짜를 선택할 수 없도록 하거나, 선택할 수 있도록 설정할 수 있는 상수값을 제공
한다．

enum oCalendarWidget::SelectionMode
상수                                    값   설명
QC졔endarWidget::NoSelection           0   날짜를 선택할 수 없도록 설정하기 위한 상수이다．
QC졔endarWi均이二SingleSelection          1   날짜를 선택할 수 있도록 설정하기 위한 상수이다．


날짜를 선택할 수 없도록 하기 위해1 setSelectionMode( ) 멤버함수를 사용할 수 있다．



 +     4돨！ 2014     +
    일 뮐 화 수 목 금 토
 14 30 31 1 2 3 4 5
 15 6 7 8 9 10 11 12 .
 16 13 14 15 16 17田19 多
 17 20 21 22 23 24 25 26
 1827282930 1 2 3
 19 4 5 6 7 8 9 10 二

（그림） OO계endarW幽이二NoSelection




1O2 CHAPTER 03... GUI 설계와 제작


===== PAGE 104 =====
（그t5F가（:)gramming




F尸4 ' Designer를 이용한 GUI 폼 제작
                     GUI 상에 위젯을 배치하고 시그널 슬롯 기능을 구현하기 위해 직접 소스 코드를 작성하였다. 아에서
                     제공하는 Designer 툴을 사용하면 소스 코드를 작성하지 않고 GU를 설계할 수 있다. Designer 툴
                    로 배치한 위젯을 시그널과 슬롯을 연결할 수 있는 기능도 제공한다．




      叫m싸eW                                                                      日네沁d
                                                                                 g曲,Ht,y
                                                                                                岡
                                                                                                 (to. 0fl 493 0S
      目         Db片Ve나
                                                                                 5口eflodtv       [m甘tote 마目
      （고 C이Umn V匹나                                                               nnnn1Un15Ze     0X0
        J          tern a匈心 了mmB州）                                               ma지mUmSCe       l67772l5 1 lb
      itot如字t
                                                                                 52目mmmenr       a 工0
                                                                                 bodizo          POX
      乞BfleX 벼dget
                                                                                 n키口nE           Hmm色j
      咽         臼b忙 나000
                        Cmtmm三
                                         4d山n 드11기   외qna匕 3 引0作 Ed如［
                    B們
                ／工 小1／ 」j ，니4乂       口姑＄Ue＄口＄ torch flea매5日却P比的onE呻녀口Corn이e0呻m




（그림） Qt Designer 실행 화면



 원리는，受愍쁘昱彭世으므즈乂느是웍프쁘르한옛웃翌프是：世횃스슨롯                                                                                  ] 변환하여 컴파일
 한다．

   Designer                                               자동 생성 코든J                            컴파일


  widget.ui                                                 U 小／dqet.h                         Make川e



（그림） Qt De引gner의 코드 자동 생성 과정




                                                                                                  4_Designer를 이용한 GUI 폼 제작 103


===== PAGE 105 =====
0Editing 卜加de
Qt Designer는 GUI 설계 기능을 제공하기 위해 \Widget Editing Mode, Signal and Slot Editing
Mode, Buddy Editing Mode 그리고 Tab Order Editing Mode의 네 가지 Editing Mode를 제공한다．

Mode                      Description
Widget Editing            GTh낮F았里흐엣耀프쁘므堡旦立따과翼픕릍悉重文르하는 기능
Signal and Slot Editing   叭突운翅읕A哮숀社旦쿡하는 기능
Buddy Editing             Label 위젯에 포함된 단축키를 통개絮天픗.1匕毛明차
                                                       "는 기능
Tab Order Editing         탭에 따라 위젯에 포커스를 순서대로 이동시킬 수 있는 기능



8Layout 기능
Designer는 GUI 설계 시 절대좌표를 이용해 마우스로 위젯을 배치할 수 있는 기능뿐만 아니라 레이아
웃을 사용할 수 있다．


                             gAdjust size
                             mJ Lay OutHonzonta如
                             目 L하r加W色八隧酬y
                             趙 Lay Out in a 垂id
                             洲 Lay Out Honzorlta却 in＄닙虹er




（그림） Layout을 사용


小 미리보기 기능과 GUI 프린트 기능
설계한 GI끄를 정확한 결과를 확인할 수 있도록 미리보기 기능을 지원한다. 이 기능을 활용하면
Designer를 이용해 GI끄를 설계하는 동안 미리보기를 통해 GI汀를 설계할 수 있다. 미리보기를 하기 위
한 단축키는 西町＋園 이다. 정확히 말하면 어플리케이션을 실행하기 위한 단축키이지만, Designer로 설
계한 GUI 확인을 위해 사용할 수 있다．

또한 설계한 GUI는 프린트를 통해1 출력할 수 있는 기능을 제공한다. GI끄를 프린트하기 위해 四ile] a
[Print］를 선택하면 된다．


心 Container 위젯 사용
Designer를 이용해 Qt에서 제공하는 Container 위젯을 사용할 수 있는 기능을 제공한다. 예를 들어 그
룹박스에서 QCheckBox 위젯을 포함시키는 GUI를 설계할 수 있다．




104 CHAPTER 03_ GUI 설계와 제작


===== PAGE 106 =====
[i小，
!
         ;


  Iext j치1gnment
               U   .




   @)Left ahgned
   0 Right aligned
   Q Centered



（그림） Cont졔ner 위젯



0Main Window 설계
Designer 툴을 사용하면 단일 위젯으로 GI끄를 설계하는 것 이외에 다중 GUI 인터페이스를 제공하는            ' \/   \hH/ ＼느／＼니小1니／ 八H／   八m= m小＝ 八1


入4amll Window 설계가 가능하다. Main Window어］메뉴를 추가하거나 특정 위젯을 메뉴어］ 추가하는 것
도 가능하다．




（그림） Main Window의 메뉴 기능 추가



0Custom Widget F기ug니n
Qt에서 제공하는 위젯 이외에 개발한 위젯인 커스텀 위젯을 Designer의 위젯 상자로 추가히1Designer
툴에서 사용할 수 있는 기능을 제공한다．

      汭幻rid Time Ck乂k - exan叩les/de引gne由心Ii巾lii


             update d(QTime)
                                                                                                                !




                                             mEF0石E日팎
                               Current tim              2 :00 :00 AM
                                                                                                                八




                   c
             setTimeZonelint
                               Set time zo           !n      L소j
                                                   -v히ueChanged(int




（그림） De引gner에서 Cus幻m Widget 등록




                                                                         4_Designer를 이용한 GUI 폼 제작 105


===== PAGE 107 =====
  畜如．1 1 위젯과 시그널 슬롯을 사용한 예제
 Qt Designer 기능을 이용해 GUI를 설계하기 위해 다음과 같이 프로젝트를 생성한다．




      口 Qt Gui Applicatr아l


                        Class Information
      Location
      K油                却Sc的 ban比 in幻rmatiOn 的out the classes for which you 놔ant to generate 5k미e伯nsource code tiles.

  中 Details
                        디ass name:         뻐的et
      Summary
                        Base class         요越4get ？小

                        ffeaderflle:       widget,h
                        Source file:       내dget cpp
                        Generate 佃m 團
                        Form tile          내的吼at




                                                                                                               Cancel



（그림） 프로젝트 클래스 정보 입력



"Generate form" 항목을 체크하고 화면에서 보는 것과 같이 프로젝트를 생성한다. 프로젝트 생성이 완
료되면 Qt Creator 프로젝트 내비게이션의 Forms 항목에 widget.ui 파일이 추가된다．



 F沌    Ed作       B山Id      Debug           As日肛e       自이S ＼사in（卞m
                 Projec始               !    됴7. 包 日＋ )<      +
                 4 h iDe却ner
                     瞬 1_Designer.pro
                   1> 。h Headers
                   4 奴 SOUrCeS
                       깐：二 maln.cpp
                      巴 wid哄cpp
                   4 芦 Forms
                      之, Wi. . - 山

（그림） UI 파일 선택



w奴get.ui 파일을 더블 클릭하면 Qt Designer를 이용해 폼을 디자인 할 수 있는 인터페이스가 제공된
다. 여기서 위젯과 레이아웃을 이용해 어플리케이션을 작성해 보자．

마우스로 [Horizontal Layout］을 Drag하여 배치하고 QSinBox 위젯과 QSlider 위젯을 배치한 레이아
웃 상에 포함될 수 있도록 배치한다. 동일한 방법으로 레이아웃과 위젯을 다음 화면과 같이 배치한다．




106 CHAPTER 03_ GUI 설계와 제작


===== PAGE 108 =====
宙 s,dgetu            그85心net - QE Cleat口r                                                                         ，二＋厚hm"三mm

    F卜e   661    Blild     D.6tg    邱mbm    自이5   m的汁   F+HP



    1兀n ：「‘『                  回m,           므 '                     "             已"'峯쌔的.                     就m的．,             '



    ;,';: 뇨m：烏恣百 닙小m                                           1i             ;      m盤쁘心繫望쁘
三         i ＼柚吼깐印丑뜨
                                                                                  口L                                O   +   卞   "
    " " " 匐瓦i客臂                                                                   刈dUel     n咐deli

                       加    BUd0n                                                 Pr아enty                Ut山e                   1
                咽




                   Sil。
                    ；戶
                 e      Rad匕 BtJtt0n



            中Uted中      峙                                                                 멉批             41                     나
: 强冬二
                                                                                    end아咐odaity          lonModa
                                                                                    ena벼Cl               團
                                                                                     qeeteetry            ((0. 0). 33911 1661
                                                                                     5注16帥CS             .1966미Te4 口referred




/ " 弘乞：ni-il 뇨亡缸姓小』,.,．』
                                                                                     n기nmUmS口e           0X0
                                                                                    maaeeumSlze          167772151116777215     -

                                                                                  口C口nip的0UmUt       =




（그림） 레이아웃과 위젯 배치


그림과 같이 위젯을 배치하고 QSpinBox와 QSlider의 프로피티 창을 통해 minimum, maximum 값과
오브젝트명을 다음과 같이 변경한다．

OSpinBox Object Name                                    QSlider Object Name       minimum                    maximum
하기nBoxl                                                 sliderl                                              99
S口nBox2                                                 slider2                                              99
하기nBox3                                                 slider3                                              99


소스 코드를 작성할 수 있도록 Qt Creator 왼쪽 탭 중 [Ed川를 클릭한다. 배치한 QSlider 위젯의 시그
널 이벤트를 연결할 슬롯함수를 다음과 같이 작성한다．

widget.h

    private slots:
                void sliderlmvaluechanged(int value) ;
                void slider21valuechanged(int value) ;
                void slider3mvaluechanged(irxt value) ;


widget.cpp
    void Widget: :sliderl1 valuechanged(int value)
    {
            ui- >spinBoxl->setValue (value) ;



    void Widget: :slider2 valuechanged(int value)
    {
                u戶＞spinBox2牛＞se七Value (value) ;
    }

    void Widget: :slider3Hvaluechanged(int value)
    {
            ui- >spinBox3->setValue (value) ;




                                                                                                                  4_Designer를 이용한 GUI 폼 제작 107


===== PAGE 109 =====
QSlider 위젯의 시그널 이벤트와 슬롯함수를 연결하기 위해 connect( ) 함수를 다음과 같이 클래스 생성
자에 코드를 추가한다．

 connect (ui- >sliderl,        SIGNAL (valueChanged(int) ), this,
              SLOT (sliderlmvaluechanged(intfl)    ;


 connect (ui- >slider2, SIGNAL (valueChanged(int) ), this,
              SLOT (slider2mvaluechanged(int) ));


 connect (ui- >slider3, SIGNAL (valueChanged(int) ), this,
              SLOT (slider3_valuechanged(int) ));



QSlider 위젯상의 눈금을 변경하면 QSpinBox 위젯의 값이 변경될 수 있도록 슬롯함수에서 QSpinBox
위젯 클래스의 setValue( ) 멤버함수를 이용해 값을 변경할 수 있다．

 I그 ＼사idget




（그림）（거 Designer를 이용한 예제



Qt Designer 툴은 제공하는 위젯 이외에 커스텀 위젯을 플러그인 기능을 통해 위젯 탭을 등록할 수 있
다. 이 방법은 추후 커스텀 위젯을 다루는 단원에서 살펴보도록 하겠다．



    如？Calculator Form 예제

C叱a史｝으뜨연雙쁘乏延之匙哭뜨브量也t쁘르쁘쓰한다· 생성한 어플리케 "］션 상에 다음 그
림과 같이 QWidget의 Sub 클래스로 등록한 위젯상에 숫자를 표시하고 첫 번째 입력 값과 두 번째 입력
값을 더해 출력 위젯에 값을 표시하는 기능을 작성해 보자．

「匡그 Calculator Form                1叫
   Input 1      Input 2   Output
    6   :        텨 名＞     !   I4




（그림） C톄C미ator Form 예저1




108 CHAPTER 03_ GUI 설계와 제작


===== PAGE 110 =====
생성한 어플리케이션의 Pr이ect 파일어］ 다음과 같이 코드를 추가한다．

            FORMS           = calculatorform.ui



 프로젝트를 빌드하면 uiC가 ui calculatorform.h 헤더 파일을 생성한다. calculatorform.ui 파일에 의
해 생성된 ui calculatorform.h 파일을 calculatorform.h 헤더 파일을 추가한다．

[#include
                         노i calculat。
                                    rf。rm.    h   "




  QWidget을 상속받은 CalculatorForm 클래스에 Designer로 생성한 UI 파일을 사용하기 위해 다음과
같이 코드를 추가한다．

            class CalculatorForm : public QWidget
            {
                   Q OBJECT

            public:
                   CalculatorForm(QWidget *parent = 0) ;


            private slots:
                   void on inputSpinBoxlmvalueChanged(int value) ;
                   void on inputSpinBox2HValueChanged(int value) ;


            private:
                   Ui: :CalculatorForm Ui;
            };
 Ui는 Designer어］ 의해 생성된 GUI를 연결하기 위한 인터페이스이다. 따라서 GUI 상어］ 생성된 위젯에
      접근하기 위해 Ui를 다음과 같이 사용하면 된다．

            CalculatorForm: :CalculatorForm(QWidget *parent)
                   : QWidget (parent)
            {
                   Ui 小etupUi(thi引 ;
            }


     GUI 인터페이스를 설정하기 위해1 setupUl( ) 함수를 사용한다. 스핀 박스로부터 시그널을 자동으로 연
        결하기 위해 각각의 슬롯함수를 구현해야 한다．

            void CalculatorForm: :on_inputSpinBoxl_valueChanged(int value)
            {
                 ui . outputWidget->setText ( QString: : number (value
                                                      + ui. inputSpinBox2->value () ));
            }

            void CalculatorForm: :on inputSpinBox2_valueChanged(int value)                                   0


                                                                                    4_Designer를 이용한 GUI 폼 제작 109


===== PAGE 111 =====
  {
      ui . outputWidget->setText (QString: : number (value
                                      + ui. inputSpinBoxl->value () ));
  }



 첫 번째 스핀 박스 값이 변경되거나 두 번째 스핀 박스의 값이 변경되면 각 슬롯함수가 실행된다. 따라서
 첫 번째 스핀 박스의 값과 두 번째 스핀 박스의 값을 더해1outp毗＼Widget의 출력 값이 표시된다．




110 CHAPTER 03_ GUI 설계와 제작


===== PAGE 112 =====
Qt 5 Programming




r口n5 다이얼로그

             단0愕론극트쁘쁘쁘‘코｛呈蜚크뽀L윔활旦간曼견嶝한다· 예를 들면 메인 윈도우 또는 싱글 윈
             도우 기반의 어플리케이션상에서 새로운 다이얼로그를 생성하여 값을 입력받을 수 있는 기능을 제공한
             다. 이번 장에서는 （기에서 제공하는 다이얼로그 타입에 대해 알아보도록 하자．




다이얼로그는 사용자로부터 입력을 받거나 여러 개 중 하나를 선택할 수 있는 GUI 인터페이스를 제공한
다. 메인 윈도우 이외에 다른 태화상자와 같은 다이얼로그를 통해 사용자로부터 입력을 받을 수 있도록
Qt에서는 GUI 기반 다이 얼로그를 제공한다．

새로운 프로젝트를 생성하는 과정에서 프로젝트명을 입력하거나 클래스명을 입력하는 것도 다이얼로그
중 하나이다. Qt는 사용자 입력으로부터 값을 입력하거나 원하는 것 중 하나를 선택하는 다이얼로그, 메
시지 다이얼로그, 파일 다이얼로그 등과 같은 다이얼로그 이외에 사용자 정의 다이얼로그를 제공한다. 따
라서 특정 조건에 맞는 다이얼로그는 커스터마이징이 가능하다．



          5. ] 일반 다이얼로그

Qt에서 제공하는 다이얼로그는 파일, 폰트, 컬러 선택 등의 다양한 형태의 다이얼로그 클래스 위젯을 제
공한다．

    종류             설명

（긔n口utDialog       사용자로부터 값을 입력 받을 수 있는 다이얼로그

    OColorDialog   특정 컬러를 선택할 수 있는 다이얼로그

    OFileDialog    파일 혹은 디렉토리를 선택하는 GUI 인터페이스를 제공하는 다이얼로그
    QFontDialog    폰트를 선택하기 위한 다이얼로그
    QMessageBox    모달 방식의 다이얼로그OloL 사용자가 선택한 항목（여를 들어 확인／취소）의 리턴 값을
                   메인 윈노우로 전달할 수 있다．

    아rogress미졔og   퍼센트와 같은 진행사항을 보여주기 위한 다이얼로그



. （긔npu山回og
r
    헤더 파일 :
    #include <QlnputDialog>




                                                                  5 다이얼로그 111


===== PAGE 113 =====
QlnputDialog는 사용자로부터 값을 입력 받을 수 있는 기능을 제공하는 다이얼로그이다. 입력값은 정
수, 실수, 문자열 QStrii培을 입력값으로 받을 수 있다．

 bool retValue;
 m1lt i        = QlnputDialog: :getlnt (this,   tr ( "QlnputDialog: :getlnteger () ") ,
                                        tr ( "Percentage: ") , 25, 0, 100, 1, &retValue) ;
 if     (retValue)
         qDebug( ''true,    %d", i) ;
 else
         qDebug( "false, %d", i) ;



getlnt( ) 멤버함수는 사용자로부터 정수값을 입력 받을 수 있는 다이얼로그 기능을 제공한다. 첫 번째
인자는 부모 클래스를 지정하고, 두 번째 인자는 윈도우의 타이틀 바 제목이다. 세 번째 인자는 입력값 위
젯 항목의 라벨이다. 네 번째 인자는 설정값이며, 다섯 번째 위젯과 여섯 번째1 위젯은 위젯의 입력값의 범
위이고 다음 인자는 다이얼로그의 스핀 박스의 STEP이다．

마지막 인자는 다이얼로그에서 [OK] 또는 [Cancel] 버튼을 클릭했는지 확인할 수 있는 변수를 지정한다．


 i그QlnputDialog4ge t        甘叫斗




（그림）（긔nputDialog 정수값 입력 다이얼로그



 bool Ok;
 double d = QlnputDialog: :getDouble (this,            tr ( "QlnputDialog: :getDouble ( ) U) ,
                                                tr ( "linount: ' ) , 48. 56, -100, 100, 2, &ok) ;
 if     (ok)
         edit- >setText (QString( "$%l" ) .arg(d) );


getDouble( ) 멤버함수의 7번째 인자는 소수점을 표현할 자릿수를 지정하는 인자이다．


 互3QtnputDi引og::ge.. 秘：m
      Amount:
      48: 56

                0K       Cent；미



（그림）（긔nputDis幻g Doub冶 값 입력 다이얼로그




112 CHAPTER 03m 0니 설계와 제작


===== PAGE 114 =====
        石St三ingList i七ems;                                                                                        n
            items << tr ( "Spring") << tr ( 'Summer ") << tr ( "Fall ") << tr ( 'rWinter ") ;


         bool Ok;
         QString item = QlnputDialog: :getltem(this,                 tr ( "QlnputDialog: :getltem() ") ,
                                                             tr ( "Season: ") , items, 0, false, &ok) ;
         if     (ok && !item. isEmpty () )
                 edi七->se七Te）比 ( 3土em) ;




    '勤帥呻帥的e [ 秘／」m
              Season :                              Season
              Spring                   !
                                                    C口ring
                         OK   Cancel
                                                    Summer
  \                                    小nn   /      Fall
                                                    쌔nter
（그림）（긔np며［기alog 아이템 선택 다이얼로그



ibool
                  Ok;
        QString text = QlnputDialog: :getText (this,                 tr ( "QlnputDialog: :getText () ") ,
                                                             tr ( "User name: ") , QLineEdit: :Normal,
                                                             QDir: :home ( ) .dirNaxne () , &ok) ;
        if      (ok && !text. isEmpty () )
                 edit- >setText (text) ;
                                                                                                                      /




  心 00이orD回og

        헤더 파일 :
        #include <QColorDialog>



QColorDialog는 사용자가 색상을 선택하기 위해 제공되는 다이얼로그이다．

        QColor color;


        color = QColorDialog: :getColor (Qt: :green, this,
                                         "Select Color ",
                                                 QColorDialog: : DontUseNativeDialog) ;

        if     (color. isValid () ) {
                edit- >setText (color. name () );
                edit- >setPalette (QPalette (color) );
                edit- >setAutoFillBackground(true) ;
        }




                                                                                                        5 다이얼로그 113


===== PAGE 115 =====
getColor( ) 멤버함수의 첫 번째 인자는 Q（그아on1万alog의 디폴트 색상을 지정하고 세 번째 위젯은 다이
얼로그의 타이틀바 제목을 입력할 수 있다. 마지막 인자는 옵션값을 상수로 지정할 수 있다．

상수                                     값                설명
QColorDaIog::ShowAIphaChannel              Ox00000001   알파 값을 선택할 수 있는 기능 제공
QColorDialog::NoButtons                    0x00000002   0K, CANCEL 버튼을 표시하지 않음



     nSelect C미cr




             戶ld to Cus地mC帥가S


                                                                 /



（그림） QC이orDialog



0QFontDialog

        파일 :
       dlude <QnontDialog>



QFontDialog는 사용자로부터 폰트를 선택할 수 있는 다이 얼로그이다．

 bool Ok;
 QFont font = QFontoialog: :getFont (&ok, QFont ( "Courier 10 Pitch' ) , this) ;


 if     (ok) {
         edit- >setText (font. key () );
         edit- >se七Fon七 ( f on七 ) ;
 }




114 CHAPTER 03_ GLM 설계와 제작


===== PAGE 116 =====
' U그 Select F。nt                             1                                       k叫 '
    } Font                                       Font style                   Size            1
    1 旺目mii                                日미d                                12              1
    rAg!匹y FB                            , B이d                                6           ,   1
    1 Aharon                         口           a벼dltalic                    7       +       1
    1 시gerian                                                                 B       三       1
    1 Andalus                                                                 9               1
    1 Angsana New                                                             10      -




    1 AngsanaUPC                                                              11              1
    1 Aparajita                                                               12              1
    1 Arabic Typesetting                                                      14              }
    I Anal                               !                                    16          7
                                                                                              !
                                                                                              !
               E加出                                S訂叩厄
                                                                                              !
j
             口 Strike。ut
               口Und        “계
                              「“
                      iting System
                                                                     幻曲YyZz                   1
                                     1
        Wr
         Any
                                                          ,1Canca,                            2


（그림） oFontDialog



첫 번째 인자는 사용자가 다이얼로그 상에서 [OK] 또는 [Cancel] 버튼을 클릭했는지 확인하기 위한 변수
를 지정한다. 두 번째 인자는 폰트 다이얼로그 상에서 디폴트 선택으로 지정할 수 있는 폰트를 지정한다．


1OF陀D回og

    헤더 파일：
    #include <QFileDialog>



QFileDialog는 사용자가 파일을 OPEN, SAVE, 디렉토리 선택 등과 같은 파일 처리를 위한 다이얼로그
이다. 기존의 존재하는 파일을 선택하기 위해 get야)enFilename( ) 멤버함수를 사용할 수 있으며 지정
한 확장자, 텍스트 파일만을 파일 다이얼로그 상어］ 필터링하여 사용자에게 보여줄 수 있다．

get야)enFileNames( ) 멤버함수는 디렉토리 내에 존재하는 파일을 다중 선택할 수 있는 기능을 제공한
다. getExistingDirectory( ) 멤버함수는 사용자로부터 디렉토리를 선택할 수 있으며 , getSave
FileName( ) 멤버함수는 사용자가 저장할 파일을 지정할 수 있는 다이 얼로그 기능을 제공한다．

    QFileDialog: :Options options;
    options = QFileDialog: :DontResolveSymlinks 1 QFileDialog: :ShowDirsOnly;


    options 1= QFileDialog: :DontUseNativeDialog;
    QString directory = QFileDialog: :getExistingDirectory (this,
                                tr ( "QFileDialog: :getExistingDirectory () ") ,
                                                 HIhome " r
                                                 options) ;




                                                                                                  5 다이얼로그 115


===== PAGE 117 =====
get且xistingDirectory( ) 멤버함수는 사용자로부터 디렉토리를 선택할 수 있는 기능을 제공하는 멤버함
수이다. 첫 번째 인자는 부모 클래스를 지정하고, 두 번째 인자는 파일 다이얼로그의 타이틀바 제목이다．

세 번째 인자는 지정한 디렉토리가 디폴트로 지정하기 위해 사용하는 인자이다. 마지막 인자는 파일 다이
얼로그의 상수 값을 이용해 필터 링하기 위한 옵션이다．

상수                                       값                설명
아키eD回四::ShowDirs아기y                       0x00000001      디렉토리만 표시
QFiIeDiaog::DontResoIveSymIinks           0x00000002      심볼릭 링크를 표시하지 않기 위해 사용
QFiI印治Iog::DontContirm아erwrite            0x00000004      기존 파일을 덮어쓰기 할 때 묻는 경고 메시
                                                          지를 표시하지 않기 위하1 사용
QFiIe미alog::［兀ntUseNativeD治幻g             0x0000 0010     시스템 기본 파일 다이얼로그를 사용하지 않
                                                          7I 위하1 사용
QFileDialog::ReadOnly                     0x00000020      읽기 모드로 파일 다이얼로그를 사용
oFileDialog::HideNameFilterDetails        0x00000040      필터를 이용하1 파일을 감추21 위해 사용



到QFileDiaIog::getopennileNamel

 Look in           ，士 D附師*파딜처리*듸m미BF地                      rjO a O 降 回［司 1

  쑈깠小冬，單籌「「
                        已 듸畔舵테epro




  F陀 home

  Files of type:   ［越
                                                                  m되
（그림） 파일 다이얼로그 디렉토리 선택



 QI그ileDialog:：야比如ns Options;
 Options 1= oFileDialog: :DontUseNativeDialog;


 QString selectedFilter;
 QString fileName = QFileDialog: :getOpenFileName(this,
                                        tr ( n QFileDialog: :getOpenFileName ( ) 1' ) ,
                                        ft In
                                           /  I
                                        tr ( 'All Files (* );;Text Files (* .txt) ") ,
                                        &selectedFilter,
                                        Options) ;




116 CHAPTER03_ GUI 설계와 제작


===== PAGE 118 =====
QFileDialog 클래스의 get야）en까leName( ) 함수의 다섯 번째 인자는 사용자가 선택한 필터 옵션을 확
인하기 위한 옵션이다．




  구셤 !       川 1더                                                                            缸츠 m
    .幷 다운로드                         O匹                                 수정한 날짜             유림                크7)
    a    바뭉 호｝면
                                    多 d出rug                            2013-01-22 오阜      파할 II큭
    鹽 촤근 워치
                                    缸 release                          2013七1-22 오阜n      파일 I더
                                    口 Mak可陀                            2013-01-22 오阜      따일
                                    나 卜내akef11e0e0u9                   2013-01口2 오享       SE마凡 파덜
                                      MakefileRelease                  2013-01-22 오享m     RELEASE 파멀
                                    뼝 吼100                             2013七l끄 오莩m        Progeam S曲J9
                                a
                                크
                                쏘
                                m
                                m
                                m
   汗 킴퓨터
                                多
                                重
                                肖
    包 로겉 디스勻：C)
                                勇
                                a
    LJ 로겉 디스크 (0:)



                    파일 이룝（5):                                              r   1    1e5




（그림） 파일 다이얼로그 4 파일 열기



 QString selectedFilter;
 QStringList files = QFileDialog: :getOpenFileNames (
                             this, tr ( "QFileDialog: :getOpenFileNames ( ) ") ,
                                                        n   / r,
                                                                   r

                                                        tr ( "All Files (* );;Text Files (* .tx七) ") ,
                                                        &sele（그tedFil七er,
                                                        options ) ;



 刃QFiieDialog::getOpenrilerkamesO

  Look in            D附0馬W파밑처리W텨S耳油F旽                                              (> a ;> 窟｛自［目
    友My Computer 鳳 ma口三EF느
                 客 main빠n寸S쁘Fi?P/
    反 dejin匕m     1노 mainwin由叫h
                 ; S咽pleFile伊O




  F陀 name         "Simpi可陀pr丁 main. 耳耳）" "mamna미ndow. h"                                            Opgn

   Files of typo M日l s (*                                                                          Canpel



（그림） 파일 다이얼로그 다중 선택




                                                                                                                  5 다이얼로그 117


===== PAGE 119 =====
/                                                                                              卜

    QFileDialog:：야亢如ns 아此ions;
    options 1= QFileDialog: :DontUseNativeDialog;


    QString selectedFilter;
    QString fileName = QFileDialog: :getSaveFileName (this,
                                tr ( "QFileDialog: :getSaveFileName () ") ,
                                           "test. txt ",
                                           tr ( "All Files (* ); ;Text Files (* .txt) ") ,
                                           &selectedFilter, options) ;



    亘3 QfileDialog::getSaveFleNameU

     Lank in:     1 和，D：勺呱蝴叩治由g勺비工口mmonD卜MSVC2叩쿄b兀SOK山ebug 니 ＼孕    任） 됴） 娩 1田 ［司

           My Computer    和 debug
                          L r미ease
           de小nkir,)        卜Aakef lie
                          나UMakefi陀Debug
                          口 Makef陀R미ease
                          영 oct00머lb




     File name     姐陋

     Files at type: 쇄 Files                                               Cancel



（그림） 파일 다이얼로그 파일 저장


    今OMessageBox

    헤더 파일：
    #inc lude <QMes sageBox>


帥/lessageBox는 모달 다이얼로그를 제공하는 클래스이다. 사용자로부터 메시지를 보여주고 다음과 같
은 버튼을 입력 받을 수 있다．

    QMessageBox: : StandardButton reply;
    reply = QMessageBox; :critical          (this,    tr ( "QMessageBox: :critical   () ") ,
                                                  "There is no a disk. ",
                                                QMessageBox: :Abort 1 QMessageBox: :Retry 1
                                                QMessageBox: :Ignore) ;


    if    (reply == QMessageBox: :Abort)
           edit- >setText (tr ( " 스bort ") );
    else if     (reply == QMessageBox: :Retry)
           edit- >setText (tr ( "Retry ") );
    else
           edit- >setText (tr ( " Ignore ' ) );



    118 CHAPTER 03叫 GUI 설계와 제작


===== PAGE 120 =====
critical( ）는 경고 창 메시지 다이얼로그를 사용하기 위해 제공하는 모달 다이얼로그이다. 첫 번째 인자
는 부모 클래스를 지정하고 두 번째 인자는 메시지 박스의 타이틀바 제목이다．

세 번째 인자는 메시지 다이얼로그의 내용을 입력할 수 있다. 마지막 인자는 다이얼로그상어］ 배치할 버튼
이며 , 상수 값으로 다음과 같은 버튼을 다이얼로그상어］ 배치할 수 있다．

    상수                                         값            설명
    QMessageBox::Ok                            0x00000400   0K 버튼
    QMessageBox::Open                          0x00002000   파일 열기 버튼
    QMessageBox::Save                          0x00000800   저장 버튼
    QMessageBox::Cancel                        0x00400000   취소 버튼
    QMessageBox::Close                         0x00200000   닫기 버튼
                                          H나




    QMessageBox::Discard                       0x00800000   저장하지 않고 버리;71 버튼
    QMessageBox::A口히y                          0x02000000   APPLY 버튼
    QMessageBox::Reset                         0x04000000   RESET 버튼
    QMessageBox::RestoreDefaults               0x08000000   다시 저장하71 버튼
    QMessageBox::Help                          0x01000000   도움말 버튼
    QMessageBox::SaveAU                        0x00001000   모두 저장하기 버튼
    aMessageBox::Yes                           0x00004000   YES 버튼
    QMessageBox::YesToAll                      0x00008000   모두 YES 적용하기 버튼
    QMessageBox::No                            0x00010000   N0 버튼
    QMessageBox::NoToAll                       0x00020000   모두 N0 적용하기 버튼
    QMessageBox::Abort                         0x00040000   중지 버튼
    QMessageBox::Retry                         0x00080000   재시도 버튼
    QMessageBox::lgnore                        0x00100000   gnore（무시） 버튼
    QMessageBox::NoButton                      Ox00000000   An invalid button



'刃QMessageBo乂：critic키0               m

     0       There is no a   dis
         m            Ign어e        Ab여t
\                                              J




（그림） Critical 메시지 모달 다이얼로그



    QMessageBox: : StandardButton reply;
    reply = OMessageBox: :information(this, tr ( "QMessageBox: : information ( )") ,
                                      "I am a Qt Devel아尼r. <br> ' \
                                      "I love Qt '1 ) ;


    if (reply == QMessageBox: :ok)
        edit- >setText (tr ( "OK ' ) );
    else
        edi卜＞se七Te＞比（tr 「 Escape " ) ) ;



                                                                                       5 다이얼로그 ］伶


===== PAGE 121 =====
    箋3QMessageBox::informa   山          '




（그림） Inform졔山n 메시지 모달 다이얼로그



    QMessageBox: : StandardButton reply;
    reply = QMessageBox: :question(this,                       tr ( "QMessageBox: :question() ") ,
                                                         "Do you save this file? ",
                                                         QMessageBox: :Yes 1 QMessageBox: :No 1
                                                         QMessageBox: :Cancel) ;


    if   (reply == QMessageBox: :Yes)
         edit- >setText ( tr ( "Yes ") );
    else if    (reply == QMessageBox: :No)
         edit- >setText (tr ( "No") );
    else
         edi卜＞se四e）代 作r ( "Cancel기 ) ) ;



'I그QM巴珀恥B。
         x::que:ti。
                  nO               b叫                '




으"＝니
\                       1nm小mdm며m小口n口       444』 』       7




（그림） Question 메시지 모달 다이얼로그



    QMessageBox msgBox (QMessageBox: :Warning, tr ( "QMessageBox: :warning() ") ,
                         "you save this file                    ?", 0, this) ;
    msgBox. addButton(tr ( "Save &Again") , QMessageBox: :AcceptRole) ;
    rnsgBox. addButton(tr ( "&Continue ") , QMessageflox: :RejectRole) ;


    if   (msgBox. exec () == QMessageBox: :AcceptRole)
           edi七수se七Te砒 (t丁（H 鈿ye Again" ) ) ;
    else
           edit- >setText (tr ( "Continue") );




120 CHAPTER 03小 GUI 설계와 제작


===== PAGE 122 =====
첫 번째 인자는 QMessageBox 상에 표시할 아이콘을 선택할 수 있으며 다음과 같은 상수 값을 사용할
수 있다．

상수                                                   값          설명
QMessageBox::Nolcon                                             아이콘을 사용하지 않기 위한 상수
QMessageBox::Question                                     4     Question 아이콘 사용
QMessageBox기n幻曲at山n                                       ]     In幻rm졔ion 아이콘 사용
QMessageBox::Warning                                      2     Warning 아이콘 사용
QMessageBox::Critical                                     3     Critical 아이콘 사용



 刃 QMessageBox: '／亂．냠m
                      you &ave this file 7
           I
   !Save          Again          Con加iue
                                                     .1
（그림） Warning 메시지 모달 다이얼로그



                 2 사용자 정의 다이얼로그

지금까지 기본척인 다이얼로그를 다루는 방법을 살펴보았다. 기본적인 다이얼로그어囚 제공하지 않은 기
능을 사용자에게 제공하기 위해 QDialog 클래스를 상속받아 사용자 정의 다이얼로그를 구현할 수 있는
방법을 제공한다. 이번 장에서는 QDialog를 이용해 사용자 정의 다이얼로그를 구현하는 방법에 대해 살
펴보도록 하자．

 헤더 파일 :
 #include <QDialog>




 @ 口 Qt         Gui A口口＜anion


                           Class Information
           Location
           K炳               S口ec加 has妃 in佃rmation about the 이ass日S 佃r 寸,hioh you 뇨cant t口 generate sketet口n
                            5口urce C口de tiles
  中 Details
           Summary          디ass name:       Main쌔ndow

                            Base class:      roMainwindow
                            Header tile:     m계nwind口W上

                            Source tile:     m히n나indo比C［耳
                            Generate form:
                            Form 꿰5:         m刮n넥ind口叱Ui




                                                                                      Nest        Canoe




（그림） 프로젝트 생성 시 （기ass In幻rm計山n 창


                                                                                                              5 다이얼로그 121


===== PAGE 123 =====
프로젝트 생성 시 [Class Information] 창의 Base class 항목에서 "QDialog" 항목을 선택한다. 프로젝
트 생성을 완료하면 clialog.h 혜더 파일에 사용자로부터 값을 입력 받을 수 있는 QLineEdit 위젯과
QPushButton 위젯을 배치하기 위해 다음과 같이 코드를 추가한다．

 priva七e :
       QLabel *lbl;
       QLineEdi七 出edi七；
       QPushBut；七on 士okb七n;
       QPushButton *cancelbtn;



혜더 파일에 선언한 위젯을 배치하기 위해 레이아웃을 사용하였다. dialog. cpp 파일에 다음과 같이 소스
파일을 추가한다．

 setWindowTitle ( "Custom Dialog't ) ;


 ibi   = new QLabel ( "Name ") ;
 edit = new QLineEdit ( " ") ;


 okbtn = new QPushButton ( "OK ") ;
 cancelbtn = new QPushButton ( "CANCEL") ;


 QHBoxLayout *hlayl = new QHBoxLayout () ;
hlayl- >addWidget ( ibi) ;
hlayl- >addwidget (edit) ;


 QHBoxLayout *h1ay2 = new QHBoxLayout () ;
 h1ay2->addWidget ( okbtn) ;
h1ay2->addwidget ( cancelbtn) ;


QVBoxLayout *vlay = new QVBoxLayout () ;
 vlay->addLayout (hlayl) ;
 vlay->addLayout ( hlay2) ;


 setLayout (vlay) ;




끄 Cus帥 D녜09           『芬尋，:：了「？C.「，,

  Name

  ,      OK    !    CANCEL



사용자 정의 다이얼로그




122 C니APTER 03_ GUI 설계와 제작


===== PAGE 124 =====
Qt 5 Programming




F尸 6 Main 쌔ndow
                     이번 장에서는 QMainWindow 클래스를 이용하1 어플리케이션 메인 윈도우 사용자 인터페이스를 개발
                     하는 방법에 대해 다루어 보도록 하자. 메인 윈도우는 메뉴바, 툴바, 상태바, Dock Widget, Central
                     Widget을 메인 윈도우의 레이아웃에 배치할 수 있는 유저 인터페이스를 설계할 수 있다．




（그림） 메인 윈도우 GUI 인터페이스



메인 윈도우는 SDI와 MDI 방식으로 분류할 수 있다손므르브蟹엿雙팟史翅心뺏샤자로 메
인 윈도우는 하나의 서브 윈도우가 포함된 형식이다. MDI는 메인 윈도우상에 여러 개의 서브 윈도우를
                                                                \．小／ \/\/\/\=,/＼小／   \H/   \/\／八七／   \=／八，／八小r

포함할 수 있다．

                            README 5D1

 E加    Ed口   He1P


     口 多｝口 矢 三：
              } 的
 시 me 듸and꾜d fea山remfa列＜abm mammnd0W5 出e 皿n너ded 하 QL

 Ham mnd0甘5（帥 haYe PUn d0nn nmnU5 md b카5. Mddot* ,nd0나'p祀5e
 5텨jar出e rmm5 이 U5er 1n1)m 可e m艇d,,,anmt.며카edacbon 升gernth긔
 리505upnomke1tO카d 5 ho,1c, tt 凹dacce出m0f he好 m n比nU mm5
 1
 p忙 eX키n叱 1aUnd比r m0너d叱 eith Pt (m be a Led 伯 eX머0t,atheIthe
 examples m 甘e d taerb

 DeCUmexaeeeler*比5e eXam呻5Can be (0USd 녀a 片円 TCee거 emdEeacm的町
 hnk n d기e m기n Q1 如rUmem帥0n




（그림） SDI와 MDI




                                                                                                6 Main Window 123


===== PAGE 125 =====
簪 메뉴바 생성
메인 윈도우에 메뉴를 생성하기 위해 帥4enu와 帥4enuBar 클래스를 사용한다. QAction 클래스로 생
성한 메뉴 아이템을 帥/lenu 위젯의 addAction( ) 멤버함수를 사용해 등록한다．

QMenu *fileMenu;
QAc七ion 央newAct;
QAc七ion 卉openAc七；


newAct = new QAction(Qlcon( " . /images/new.png") , tr ( "&New") , this) ;
newAct->setShortcuts (QKeySequence: : New) ;
newAct->setStatusTip(tr ( "Create a new file ") );
connect (newAct, SIGNAL(triggered() ), this,      SLOT (newFile () ));


 openAct = new QAction(Qlcon( " . /images/open.png") , tr ( " &Open. ..") , this) ;
openAct->setShortcuts (QKeySequence: : Open) ;
openAct->setStatusTip(tr ( "Open an existing file ") );
connect (openAct, SIGNAL(triggered() ), this,      SLOT (open() ));


 fileMenu = menuBar (卜＞ad沁帥미七r ( "&File " ) ) ;
 fileMenu->addAction ( newAct) ;
 fileMenu->addAction (openAct) ;




（그림） 메인 윈도우 메뉴바



客 툴바 생성
툴바는 QToolBar 클래스의 addToolBar( ) 멤버함수를 이용해 메인 메뉴에 툴바를 추가할 수 있다．

 QToolBar * fileToolBar;
 fileToolBar = addToolBar (tr ( "File ") );
 fileToolBar->addAction ( newAct) ;
 fiieToolBar->addAction ( openAct) ;




（그림） 메인 윈도우 툴바




124 CHAPTER 03_ GUI 설7引외 제작


===== PAGE 126 =====
0Dock Widget 추가
Dock Widget은 메인 윈도우 상에 배치하거나 윈도우 영역 밖에 배치할 수 있는 위젯이다. addDock
Widget( ) 멤버함수를 사용해 메인 윈도우어］ Dock Widget을 추가할 수 있다．

 QDockWidget *dock = new QDockWidget (tr ( "Target ") , this) ;
 dock->setAllowedAreas (Qt: :LeftDockWidgetArea 1 Qt: :RightDockWidgetArea) ;


 QListWidget *customerList = new QListWidget (dock) ;
 customerList->addltems (QStringList ()
          << 'One"
          << "rwo"
          <<   "Three"
          <<   "Four "
          <<   "Five") ;
 dock->setWidget (customerList) ;
 addDockWidget (Qt: : RightDockWidgetArea, 面ck) ;




 Target                      序 >＜三


 OneTw。
 汀柑ee
  Four
n 디ye

（그림） 메인 윈도우 Dock Widget



0Central Widget 추가
setCentralWidget( ) 멤버함수를 사용해 메인 윈도우 상에 Central Widget을 추가할 수 있다．

 QTextEdit *textEdit = new QTextEdit;
 setcentraiwidget (textEdit) ;




                                 Target
                                 （그ne
                                 Two
                                 Three
                                 Four
                                 디ye




（그림） 메인 윈도우 Central Widget




                                                                           6 Main Window 125


===== PAGE 127 =====
 S Status Bar 추가
 Status Bar는 사용자에게 메인 윈도우의 정보를 표시하기 위한 목적으로 사용할 수 있으며 QStatus-
 Bar 위젯을 메인 윈도우상에 배치할 수 있다. Status Bar를 추가하기 위해서는 setStatusBar( ) 멤버
 함수를 사용해야 한다．

 S七atusBar (卜＞show卜陀ssage (tr ( "脆ady" ) ) ;




  F昶




                               （그ne
                               Two
                               Three
                               Four
                               日ye




（그림） 메인 윈도우 Status Bar




126 CHAPTER 03_ GUI 설계와 제작


===== PAGE 128 =====
01 5 Programming




       '7 卜加del/View 아키텍처와
          데이터 바인딩 위젯
              이번 장에서는 Model/View 아키텍처 구조를 살펴보고 QTreeView, QListView, OTab厄니ew 위젯
              상에 데이터 리스트 아이템을 표시하고 핸들링 하71 위한 방법에 대해 살펴보도록 하자．




위젯                 설명
 QList View        데이터 리스트 스타일로 표시하기 위한 위젯
 QTable View       Tab匕 피ew를 구현하기 위한 mo（拍I'미이V
 OTreeView         가ee View를 구현하기 위한 model!피ew




                卜加del/니이V 아키텍처

Model/View는 데이터를 다루는 Model과 사용자에게 GUI 인터페이스를 제공하는 \[jew를 말한다. 데
"］터를 GUI로부터 분리가는 일종의 아키텍처이며，,M乂잇妥으赳쓰쁘多0多브뺏라고 부른다·

MVC는 3가지의 오브젝트로 구성되어 있다. 첫 번째는 파일 및 데이터베이스와 같이 Qt를 이용하기 위
한 데이터를 가공하지 않은 상태이고, 두 번째는 Model Container로써 데이티로부터 읽어온 데이터를
담는 Container이다. Mod이은 GUI 인터페이스 상에 표시할 데이터를 \[jew에 표시하지 않고 Model
로 접근해 데이터를 표시한다. 마지막 View는 Mod이로부터 읽어온 데이터를 위젯을 통해 표시하거나
핸들링 할 수 있는 GUI 인터페이스를 제공한다．


         Data




（그림）卜化deH니이v Architecture




                                                 7 卜加del!View 아키텍처와 데이터 바인딩 위젯 127


===== PAGE 129 =====
墩交三三三旦曳雹퇘'］며 "11O1터륵핸들링 할수있는QListVi「也 QTabelVi「也 디렉토리 그
리고 트리와 같은 QTreeView 등과 같은 다양한 위젯을 제공한다．

Model/View를 왜 사용해야 할까? QListView와 QTableView 같은 위젯을 통해1 데이터를 표시할 때，
Model/View를 사용하지 않는다고 가정해 보자. 만약 그렇다면 QListView로 데이터를 표시하고 핸들
링 할 때와 QTableView를 통해 데이터를 표시하거나 핸들링 하기 위해서 두 개의 위젯은 서로 다른 구
조의 형태를 제공하게 된다．

그리고 QTableView와 QListView상어］ 렌더링된 데이터를 정렬하기 위한 인터페이스는 다를 수 있다．
즉 Model/View는 위젯과 뎨이터를 분류함으로써 개발자어］ 많은 수고를 덛 수 있다. Delegate는 위임이
라는 사전척 의미와 같이 뎨이터를 수정하거나 삭제와 같은 핸들링을 위한 인터페이스를 제공한다．
Model/View의 아키텍처가 어떤 형태의 클래스로 구현되어 있는지 살펴보도록 하자．


I Model
眺怏其旦q逃與M으翅是랫스늄믄是꼬으廻르괜슷읫곤욧望르괜수이다· 데이터를 액세스하거나 관리
하기 위한 인터페이스를 제공하며 데이터의 구조체, 파일, 데이터베이스와 다른 어플리케이션으로부터
읽어온 데이터를 저장할 수 있는 인터페이스를 제공한다．



QStringListModel           OString 데이터 타입의 단순한 데이터 리스트를 저장하기 위한 클래스
QStandardltemModel         임의의 데이터로부터 읽어온 데이터를 트리 형태와 같은 아이템으로 제공할 수 있는 클래스
QFileSystemModel           파일 시스템으로부터 얻어온 파일과 디렉토리에 관한 정보를 제공하71 위한 클래스
QSqlQueryModel
oSqlTableModel             데이터베이스상에 액세스하여 얻어온 정보를 Model 클래스로 구현하기 위한 클래스
oSqlRelationalTebleModel


（표＞에서 소개한 Model이 원하는 기능을 제공하지 않는다면 QAbstractltemModel 클래스를 Base 클
래스로 상속받아 커스텀 Model을 구현할 수 있다．


I View
프쁘爻덴앗브트으뜨쓰앗프쓰巴번多크콴量' ］다· 리스트 형태로 표시할 수 있는왓嶢也뜨 테 " ]
븍과 갇우 스타익로 데이터름 표시학 수 O］누 GTihIeVi .M/ 두卜 다얏하 좃류의 위젠읔 제곳하다 이 위젯
들은 QAbstractltemView 클래스로부터 상속받아 구현된 위젯이며 , 이외의 추가 기능이 필요하다면
QAbstractltemView 클래스로부터 상속받아 커스텀 View 위젯을 구현할 수 있다．


I Delegates
델리게 "］트는근欠定넷겻흐된：是多쓰:t.므쁘曼브안탓量근빳足多楚엣브쁘한쓰坦：브룐世르
赳건叉哭走又文］며 Qt 4.4 O1상 버전부터 ' i］공된 기능" j다· 클래스는 QStyledltemDele-
gate와 QltemDelegate가 제공된다. 부모 클래스는 QAbstractltemDelegate 클래스이다．



128 CHAPTER 03_ GUI 설계와 제작


===== PAGE 130 =====
QStyledltemDelegate 클래스는 View 위젯으로 데이터를 렌더링 할 때 아이템 리스트를 표시하는 스
타일을 정의할 수 있다. 예를 들어 특정 리스트 아이템 상어］ 아이콘 혹은 페인트를 사용해 도형을 그릴
                                                               수
있는 기능을 제공한다. Qlten山elegate는 Model/View어］ 뎨이터를 핸들링하기 위한 기능을 제공한다．



      7.2 Model 클래스와 \h1ew 위젯의 활용

Model 클래스의 인스턴스로부터 읽어온 데이터를 QListView 위젯과 QTreeView 위젯상어］ 표시하기
위해 다음과 같이 사용할 수 있다．

I resize(600, 300) ;
 QSplit土er 士split土er = new QSp1i七ter（七hi引 ;


 // Model 클래스
 QFileSystemModel *model = new QFileSystemModel;
 model->setRootPath(QDir: :currentPath() );


 // View 위젯 - QTreeView
 QTreeView *tree = new QTreeView ( splitter) ;
 tree->setModel (model) ;
 tree->setRootlndex (model->index (QDir: :currentPath() ));


7/ View 위젯 - QListView
QListView *list = new QListView(splitter) ;
list- >setModel (model) ;
list- >setRootlndex (model->index (QDir: :currentPath() ));


QVBoxLayout * layout = new QVBoxLayout () ;
layout->addWidget (splitter) ;
setLayout (layout) ;



선언한 QFileSystemModel은 Model 클래스로의 인스턴스로써 파일 시스템으로부터 디렉토리와 파일
정보 데이터가 매핑된 Model 클래스이다．

Model 클래스로부터 QTreeView와 QList View 위젯상어］ 렌더링하기 위해 setModel( ) 멤버함수를 사
용할 수 있다. setRootPath( ) 멤버함수는 QFileSystemModel 클래스가 현재 가리키고 있는 디렉토리
를 설정하기 위해 setRootPath( ) 멤버함수를 사용할 수 있다．

QTreeView와 QListView 위젯은 setRootlndex( ) 멤버함수를 제공한다. 이 함수는 Model로부터
Root PATH를 설정할 수 있으며, PATH를 변경하기 위해1 rootPathChanged( ) 멤버함수를 사용할 수
있다．




                                                     7 Mode1/Vie\A/ 아키텍처와 데이터 바인딩 위젯 129


===== PAGE 131 =====
a                                                                                                                      口回因
     Name                              Size                         A               뇨교 debug



                                                                                     昏區區回
                                                                                            r미已日Se




                                                               田田北m作냐m
                                                                근
         旨 器：崙盟.cpp
               .。bj                                                                 區 Makefile
                                                                                    ［蚤 Mak帥咆叱山g
         r벼 ModeL낚e叫_ConceotU.
         i1 Mod미J小e＼肱Conceot 山                                                      ［云 Makefile；日elease
                                                                                    匹 vclOO.pdb
          쩨 Mod미-v油a_C口nceot. 口4
         네 Mod이. View_Conceot ··4
         刈 ！너ode匕Vie叫_Concept.以
         염 Mode나／ew_Conce口t, 口
          ’口 州dg飢的j



                                                               口田四呻
    : 高 竿，界：,
     k盛 Makefil已Debu口

     默標e,Heleaoe
        db                                                               V




（그림） Mod이／View를 이용한 예저1




QSplitter 위젯은 위젯의 크기를 조절할 수 있는 GUI 인터페이스를 제공한다. QTreeView와 QList
View 가운데에 배치되어 있으며 위젯의 크기를 조절할 수 있다．

왼쪽은 QTreeView 위젯으로 디렉토리와 파일 정보를 트리 스타일로 표시할 수 있으며, QListView 위
젯은 디렉토리와 파일을 리스트 아이템 형태로 표시할 수 있다．

View 위젯상어］ Model 데이터를 렌더링하기 방식으로 리스트, 테이블, 트리 스타일로 분류해 볼 수 있
다. QListView는 행 단위로 Model을 렌더링하기 척합한 구조로 되어 있고 QTableView는 Model을 행
과 열을 표시하기 적합한 구조로 구현되어 있다. 그리고 QTreeView는 행 단위의 데이터를 트리 형태로
표시하기 적합하다．

     L油t 似odel                                    Table Model                                                       丁ree Model

1기 ／初O!tern               11R。
                             。titem                                                                         i       月0｛가岫m
     J
                                                                                                                1
1                          1       1


              row ;= 0         1                                                                  to나 = 0               row = 0

                                                                                                  row = 1
               ow = I                                                                                                            row = 0
                                                                                                  to刊 三＝2
              row = 2                                                                                                            row = l
                                                                                                  to나 = 3




                                                    n8三크＝ nJ             U8E3그 nN
                                         8三크그nO                                         n8三크＝ 卄
                                                                                              m
                                                                                                                        row == I


                                                                                                                        row = 2


（그림） Model 데이터 구조




130 CHAPTER 03_ GUI 설계와 제작


===== PAGE 132 =====
 D Q니st\기ew
QAbstractltemModel 클래스로부터 상속받아 구현된 QStrii垠ListModel은 QString 데이터 타입을
매핑할 수 있는 클래스이다．
r小
     QStringList strList;
     strList   << "Monday ' << "Tuesday " << "Wednedav" << "Thurdav" << "Friday ":


     QAbstractltemModel *model = new QStringListModel(strList) ;


     QListView *vjew = new QListView() ;
     view->setModel (model) ;


     QModellndex index = model->index (3, 0) ;
     QString text = model->data(index, Qt: :DisplayRole) .toString () ;


     QLabel *lbl   = new QLabel ( " ") ;
     lbl- >setText (text) ;


     QVB그xLayout *lay = new QVBoxLayout () ;
     lay->addWidget (view) ;
     lay->addWidget ( lbl) ;


     se七Layou七 ( lay) ;



QString 타입의 리스트 아이템을 QStringListModel 클래스를 이용해 매핑할 수 있다. 매핑된 Model
은 생성자 함수 첫 번째 인자로 명시하면 된다. 실제 데이터와 매핑된 mod이은 QListView 위젯상에 렌
더링하기 위해 setModel( ) 멤버함수를 사용할 수 있다．

     QModellndex index = model->index (3, 0) ;
     QString text = model->data(index, Qt: :DisplayRole) .toString () ;


 QStringListMod이로부터 리턴받은 QModellndex를 QString 데이터 타입으로 변환하기 위해 data()
멤버함수를 사용할 수 있다. QLabel 위젯은 QString 데이터 타입으로 변환한 model 데이터를 표시하
 기 위해 사용했다．




（그림）（가娼tView


                                                          7 Model/View 아키텍처와 데이터 바인딩 위젯 131


===== PAGE 133 =====
0 QTa비eView
QTableView 위젯은 행과 열이 있는 테이블 스타일과 같은 Model을 렌더 링 할 수 있는 위젯이다．
             Tab伯 m岫的
     月口아加rn

                                                  rc哨 心 0

                                                  fc哨 口 1

                                                  rc脚 = 2
                            1
                                                  rc哨 = 3



       n8쯔身二口凸
                            小
                            1




                                8E身a1的   8芝a二1m
                 8甘a心甘二 4

（그림）卜加d이 구조



QStandardltemModel 클래스는 吼lumn의 Header를 정의할 수 있는 setHeaderData( ) 멤버함수를
제공한다. 이 함수를 통해 각 C아umn별 헤더를 지정할 수 있다. setVerticalHeaderltem( ) 멤버함수
는 Row의 Header를 정의할 수 있다．

 model->setHeaderData(0, Qt: :Horizontal, Qcbject: :tr ( "Subject ") );
 model->setHeaderData (l, Qt: :Horizontal, QObject: :tr ( 1'Description") );
 it口del->se七HeaderDa七a(2, Q七：:HOriZOntal , QObject: 比r ( "Da七 e" ) ) ;


 model->setVerticalHeaderltem(0, new QStandardltem( "Col 1 ") );
 model나＞setVerticalHeaderltem(1, new QStandardltem( "Col 2 ") );
 model->setVerticalHeaderltem(2, new QStandardltem( "Col 3 ") );



setHeaderData( ) 멤버함수의 첫 번째 인자는 Column의 index이고 두 번째 인자는 상수이다．
Qt: :Orientatjon 상수이며 세 번째 함수는 Header어］ 들어갈 텍스트를 명시한다. setVertical-
Headerltem( ) 멤버함수는 열（row）의 Header를 지정할 수 있다. 첫 번째 인자는 열의 index이고 두 번
째 인자는 헤더에 표시할 텍스트이다．
헤더 라인을 지정하고 Model어］ 실제 데이터를 저장하기 위해 setData( ) 멤버함수를 사용할 수 있다．


 model->setData (model->index (0, 0) , "Monitor ") ;
 model->setData (model->index (0, 1) , "LCD 24 inch") ;
 model->setData(inodel->index ( 0, 2) , QDateTime (QDate (2011, 10, 4) ));


 model->setData(model->index ( 1, 0) , "CPU") ;
 model->setData(model_>index (l, 1) , "Intel core 2 duo") ;
 model->setData(model->index ( 1, 2) , QDateTime (QDate (2011, 12, 5) ));


 model->setData(model->index ( 2, 0) , "Keyboard") ;
 model->setData(model->index ( 2, 1) , "104 key USH Keyboard") ;
 model->setData (model->index (2, 2) , QDateTime (QDate (2011, 12, 6) ));



132 CHAPTER 03... G네 설계와 제작


===== PAGE 134 =====
setData( ) 멤버함수의 첫 번째 인자는 QModellndex로 데이터가 저장될 Row와 C아umn을 지정하고，
두 번째 인자는 QVariant 타입을 지정한다. QVariant 타입은 다양한 데이터 타입을 지정할 수 있다．

n

               Su늬ect          Descript佃n                Da伯
    C미 1 加佃n的r          LCD 24 inch            2013-10-04 오젼 12:00:00

    C미 2 CPU            Intel core 2 duo       20日니＋05 오전 12:00:00

    Col 3 Keyboard      104 key USO Keyboard   20日-1즈06 모전 12:00:00




（그림） QTableView



지금까지 살펴본 QTreeView, QListView, QTableView 이외에도 QC아umnView, QListWidget 등
Model/View 아키텍처를 사용할 수 있는 다양한 위젯들을 제공한다．




                                                                        7 Model/View 아키텍처와 데이터 바인딩 위젯 133


===== PAGE 135 =====
01 5 Programming




F尸8 ' 사용자 정의 커스텀 위젯과 플러그인
          이번 장에서는 사용자 정의 커스텀 위젯을 제작하는 방법과 플러그인을 제작하고 배포하는 방법에 대
          하1 살펴보자. 사용자 정의 커스텀 위젯을 만드는 이유는 다음과 같이 요약해 볼 수 있다．




S 제공하는 위젯이 없을 때
어플리케이션의 GUI 인터페이스를 설계하다 보면 Qt에서 제공하는 기본 위젯으로 처리할 수 없는 위젯
이 있기 마련이다. 예를 들어 어플리케이션 사용자에게 Cpu의 사용 양을 그래픽 요소를 사용해 표시해
야 하는 경우, 자동차 계기판과 같은 아날로그 속도계를 표시하는 위젯이 필요한 경우와 같이 제공하는
위젯이 없을 때 QObject 및 帥widget 등과 같은 클래스를 상속받아 사용자 정의 커스텀 위젯을 구현할
수 있다．




（그림） 사용자 정의 커스텀 위젯


. 경량의 가벼운 위젯이 필요한 경우
자원이 부족한 시스템의 한정된 리소스를 사용해 GUI 인터페이스를 설계해야 하는 경우 시스템 자원을
절약할 수 있도록 최적화된 사용자 정의 커스텀 위젯을 작성해 사용해야 한다. 예를 들어 임베디드 디바
이스에서 고화질 멀티미디어 영상 및 음성 데이터를 항상 출력하햐 하는 경우 물리적인 시스템 자원의
90% 이상을 사용한다고 가정해보자．



134 CHAPTER 03_ GUI 설계와 제작


===== PAGE 136 =====
이러한 열악한 상황에서 사용자로부터 키 입력을 받을 수 있는 \lirtual 키보드 GUI 인터페이스를 제공
해야 한다면 시스템의 남은 자원 중 활용 가능한 리소스를 최소한 절약할 수 있는 경량의 사용자 정의 커
스텀 위젯을 구현해야 한다．

芦公心恥心社心社畇a口汕泣汕I口艮比呼蜘斗社心 社心丘去仁냐＝무
目 "U日口月日口I日I 'll口月！ = 口口目口口U匹
口口口U口口口口口口口口       ［月II 口口目口口口口
四띠口口口口口U口口月口伊m1斗                 口口U口
mm口口口口口口口月口fl             口      口口nm
             m1匹           三m1a 口따

（그림） 가상 키보드 구현 GUI



그림에서 보는 것과 같이 키보드 버튼을 표시할 QPushButton, 텍스트를 표시할 QLabel 위젯, 사용자
로부터 입력을 받을 QLineEdit 위젯을 사용해 가상의 키보드 GUI 인터페이스를 설계하기 위해 상당히
많은 위젯을 사용해야 한다．

QPushButton, QLineEdit, QLabel 위젯과 같은 클래스는 帥肌dget과 다른 Base 클래스로부터 상속
받아 다양한 API를 제공하기 때문어］ 필요한 API만 제공하는 사용자 정의 커스텀 위젯에 비해 시스템 자
원을 많이 소모한다．

너무 많은 위젯을 사용해 시스템 자원이 한계에 이른다면 사용자에게 빠른 반응을 제공하기 위한 GI끄를
설계할 수 없다. 따라서 시스템 자원을 고려해 최소한의 사용자 정의 위젯만으로도 가상의 키보드 위젯을
구현할 수 있다．


S 커스텀 위젯 재사용
지금까지 언급한 기능은 사용자 정의 위젯을 사용하지 않고 클래스를 이용해 구현할 수 있지만 어플리케
이션 상에서 재사용해야 하는 경우가 있다. 예를 들어 사용자로부티 입력을 받기 위해 가상 키보드를 재
사용해야 하는 경우가 많기 때문어］ 사용자 정의 위젯을 제작한다면 필요한 곳에서 재사용할 수 있다. 이
번 단원에서 직접 소스 코드를 작성해 사용자 정의 위젯으로 제작해1 보도록 하자．
                   1人 Ta右1 三d프j   묘由

h- custom_widget - Qt Creator




키四clock
 arsalogclockpro
 Headers
브analogclockh
 Sot卄ces
쓰artalogclock.cpp
쓰 malrs.cpp
stomwdget
 cu攷om_widg心PU USED

齬諡叫驩Pet
小jcus的m_slider_wdqet.h
쓰j V삐dgeth
Sources         SLIDER
（그림） 구현할 사용자 정의 위젯



                                             ＆사용자 정의 커스텀 위젯과 플러그인 135


===== PAGE 137 =====
직접 구현한 사용자 정의 위젯을 플러그인으로 배포해 Qt Designer상에서 쉽고 빠르게 GUI 인터페이스
상어］ 배치할 수 있는 프레임워크를 제공한다．


    /                Custom
                                  CPU Widget Plug-   in        "
                                                                   . "”
                                                                          컴 파일로 생성된
                                                                          Custom Widget
    (   '   Custom
                                  Slider Widget Plug-     in   .   '"
                                                                            라이브러리


r
                                                                                +
                                          Ct Designer Integration

（그림） 사용자 정의 위젯 플러그인 제작과 Ct Designer Export



구현한 CPU USED와 SLIDER 사용자 정의 위젯을 플러그인으로 작성해 Qt Designer 상에서 익스포
트（Export）하기 위한 방법에 대해 살펴보자．


                              "      D冶材하 出k姐ets
                              스 1ae1
                                                                                    m尸H
                                   Text Bi'그wser
                                                                                          =
                                                                                          1
                                                                                    H
                                                                                          1 1
                                                                                    三

                                   Gr可小K冷 VI陋w                                      中     =




                                   Calend斗
                                   LCD N山Tiber
                                   Pr畦re$s ear
                                   Honzontal Une
                              a    \／目I比秘 Une

                              回 QDed카蜘너ew




（그림） Qt Designer룰 이용하1 사용자 정의 위젯을 G네상에 배치



                                   사용자 정의 커스텀 위젯 구현

사용자 정의 커스텀 위젯을 구현하기 위해 CPU USED 위젯과 SLIDER 위젯은 별도의 클래스로 작성하
고 제작한 커스텀 위젯을 사용하여 어플리케이션을 작성해 보도록 하자．




136 CHAPTER 03_ GUI 설계와 제작


===== PAGE 138 =====
                            Source Tree
                  (CPU USED Widget]         [Slider Widget]
                          .cpu widget.h
                    custom』                  Custom slider widget.h
                    Custom_cpu widget.cpp    Custom slider widget.cpp


                  [Application Program]
                            widget.h
                            widget.cpp
                  11        main.cpp



（그림） 소스 구성도




프로젝트 생성 시 Base 클래스로 QWidget을 선택한다. 프로젝트를 생성하고 구현할 Cpu와 Slider 커
스텀 위젯 클래스 헤더 파일과 소스 파일을 프로젝트어］ 추가한다. Qt Creator의 내비게이션 창에서 프로
젝트명에 마우스 포인터를 위치한 후 오른쪽 버튼을 클릭하면 단축 메뉴가 실행된다. 단축 메뉴에서
[Add New］를 선택해 커스텀 위젯의 헤더 파일과 소스 파일을 추가한다．

어플리케이션 프로그램의 Background로 사용할 이미지와 Slider 커스텀 위젯에서 사용할 눈금 이미지
파일을 리소스 파일어］ 등록하기 위해 프로젝트어］ 리소스를 추가한다. 리소스를 추가하는 방법은 해더 파
일과 리소스 파일을 등록했던 방법과 동일하며 [New File] 다이얼로그에서 다음 화면과 같이 추가한다．




（그림） 리소스 추가




그림에서 보는 것과 같이 [Qt]-[Qt Resource file］을 선택한다. 다음은 추가한 리소스명을 "resources
.qrc" 를 입력하고 리소스 파일 추가를 완료한다．




                   Choose the Location
  斗 Location
     b urnrnarv    Name: rca口urce히

                   Path   附exam미esW베的미sWwidgetsWan키叩이口ck



（그림） 리소스명 입력




                                                                        ＆사용자 정의 커스텀 위젯과 플러그인 137


===== PAGE 139 =====
리소스를 프로젝트어］ 추가하고 어플리케이션 백그라운드 이미지와 슬라이더 커스텀 위젯에서 사용할 이
미지를 리소스 파일을 다음 화면과 같이 등록한다．


口 res叩rce됴平口custcm_widg叭，Qt Creator                                       '=      ‘「    季 「「n
    Fit且Ed作     Bt1妃     De駟9     却也tyze   b拈   벼柄出M   l科和
                Pr미cc枳                     甲 드7. 唾츠 日十 乂   + 中      resource邕 마C
L        i\ , 4 趣 q1鈿sn_widget                               a'
:        1깐｛     颱custom_widget.pro                           I resourceslbackground.png
    Y/e比아玎8        d      니nnJ4i3rr                             小 resources/slider-handle.png


          啣-              ,h 느viugetn
                  4    c_ 5（긔니rces
                         .包 C냐stom工pu_widget.cpp
重                        므custom_slider_widgetcpp
旨         「              下乞 malncpp
旨       的bUq             므 出idgetcpp
旨        느        d 』m Resources
目        턱           固 re蛤urces.qrc
（그림） 사용할 이미지 파일을 리소스상에 등록



S CPU USED 커스텀 위젯 헤더 파일과 소스 코드 작성

    class custom_cpu_widget : public QWidget
    {
           Q OBJECT
    public:
           custoincpuwidge七（QWidge七 火paren七 = 0) ; /7 CPU USED 위젯 클래스 생성자
           void cpu setHwidge七 level (int level) ;                  /7 CPU 사용 레벨을 설정할 멤버함수


    private:
             in七 w width;                  // 위젯의 가로크기 멤버변수
           mnt 叱height;                    // 위젯의 세로크기 멤버변수
             mnt cp뜨used level; 7/ CI刃 사용 율을 변수에 저장하기 위한 멤버변수


    protected:
             vir七ual void paintEven七（QPain七丑yen七 出even七）; 7/ CPU 사용 율을 그리는 함수
    };


소스 코드는 CPU USED 위젯 클래스의 혜더 파일이며 클래스명은 Cu毗毗1叩u_widget으로 선언한다．
PUBLIC으로 선언한 cu毗om_cpu_widget 생성자는 위젯의 가로와 세로 크기를 멤버변수어］ 저장하고
resize( ）와 setFixedSize( ) 멤버함수로 위젯의 크기를 설정한다. 그리고 CPU 사용 레벨을 Cpu_
used_level 멤버변수에 디폴트 값을 설정한다．




138 CHAPTER 03_ GUI 설계와 제작


===== PAGE 140 =====
custom_cpu_widget: : custom_cpu_widget (Owidget *parent) : oWidget (parent)
{
    this- >w width = 80;
    this- >w height = 100;
    resize (QSize (this- >w width, this- >w height) );
    setFixedSize (this- >w width, this- >w height) ;
    this- >cpu used level = 10;




resize( ）와 setF奴edSize( ) 위젯 영역의 크기를 설정하는 기능은 동일하지만 x, y 좌표의 시작 좌표를
절대값 좌표 0, 0으로 설정하기 위해 setFixedSize( ) 함수를 사용해야 한다．

cpu_set_widgetjevel( ) 멤버함수는 첫 번째 인자 값을 CPU 사용 레벨 멤버변수어］ 저장하고 邸Widget
으로부터 상속받은 repaint( ) 멤버함수를 호출한다．

void custom_cpu_widget: : cpu_set_widget_level (mnt level)
{
    this- >cpu used level = level;
    this- >repaint () ;




repaint( ) 함수를 호출하면 PaintEvent( ) 멤버함수가 호출된다. 이 멤버함수는 repaint( ) 함수와 마
찬가지로 邸Widget 클래스로부터 상속받았으며 구현할 CPU USED 클래스에서 재정의 할 수 있다．

void custom_cpu_widget: : paintEvent (QPaintEvent *event)
{
    Q_UNUSED(event) ;

    QPainter painter (this) ;


    pain七er. se七Pen (QColor (0, 0, 0) );  // 드로잉 외곽선 컬러
    pain七er. se七Brush(QColor (0, 0, 0) ); // 드로잉 내부를 채울 컬러
    painter.drawRect (0, 0, this- >w_width, this- >wheight) ;


              八
              Z   l   1r
                           1
                               0
                           l
        if (this- >cpu used level > i) {
            painter. setBrush(QColor (153, 255, 0) ); 7/ used color
        }else{
            painter. setBrush(QColor (51, 102, 0) );     /7 free color
        }

        painter.drawRect (6, (this- >w height - 8) - (i* 4) , 30, 3) ;
        painter.drawRect (43, (this- >w height - 8) - (i* 4) , 30, 3) ;
    }
}


                                                               ＆사용자 정의 커스텀 위젯과 플러그인 139


===== PAGE 141 =====
drawRect( ) 함수는 x, y 좌표로부터 width, height 크기 영역을 지정한 setPen( ）과 setBrush( ) 멤
버함수로 사각형을 그린다．

凡r문에서는 Cpu의 사용 양을 표시할 색상은 녹색으로 사각형 영역을 그리고 사용하지 않은 Free 영역
은 어두운 녹색으로 사각형을 그린다. 생성자 함수에서 디폴트 값으로 10의 값을 Cpu-끄sed_level 멤버
변수에 선언하였으므로 좌우 10개의 사각형을 밝은 녹색으로 지정하고 나머지 사각형은 어두운 녹색으로
칠하게 된다．




                        RGB 51, 102, 0



                          GB 153, 255, 0




（그림） CPU USED 커스텀 위젯 Paint 영역



구현할 Slider 커스텀 위젯의 눈금이 변경되면 시그널 이벤트를 발생하며 슬롯함수에서 CPU USED 커
스텀 위젯 클래스의 PUBLI(그 멤버함수로 선언한 cpu_set_widget七vel( ) 함수를 호출한다. CPU
USED 위젯 클래스의 Paint 영역은 repaint( ) 함수가 Mappii乷된 paintEvent( ) 함수를 호출해 다시
그려지게 된다．


密 Slider 커스텀 위젯 헤더 파일과 소스 코드 작성

 class custom sliderHwidget : public QWidget
 {
     Q OBJECT


 public:
     custom_slider_widget (QWidget *parent = 0) ;
     void slider_ set widge七小r的ize (in七 wid七h, in七 height) ;
     void sliderHset max value (float value) ;
     void slidermset中mmn value (float value) ;
     void slidermsetHcurrent1value(float value) ;


     mnt slider_ get_current_value () ;


 signals:
     void valuchanged(int value) ;


 private:
     mnt 1寸 wid七h; // 위젯의 넓이
     in七 wheight; // 위젯의 높이
                                                                         O


140 CHAPTER 03_ GUI 설계와 제작


===== PAGE 142 =====
     float max value; /7 max 값
     float mmn value; /7 mmn 값
     float curren七 value; // 현재 값


     float slide二y1均S;
     float slider width, slidermheight;


protected:
     virtual void paintEvent (QPaintEvent *event) ;
     virtual void mouseMoveEvent (QMouseEvent* event) ;




소스 코드는 Slider 위젯의 헤더 파일이다. 클래스명은 custon匕slider_widget 이름으로 선언하고
QWidget 클래스를 부모 클래스로 선언한다. slider set十widget_resize( ) 멤버함수는 Slider 커스텀
위젯의 가로와 세로 크기를 멤버변수에 저장하고 邸Widget으로부터 상속받은resize( ) 함수와 setFixed
Size( ) 멤버함수를 이용해 Slider 위젯의 크기를 설정한다．

slider_set_max_value( ）와 slider_set_min_value( ）는 Slider 커스텀 위젯의 최소값과 최대값을 멤버
변수에 저장하기 위한 멤버함수이다．

void custom slider widget: :sliderHset,widgetmresize(int width, mnt height)
 {
     七his->w width = wid七h;
     this- >w height = height;


     resize (QSize (width, height) );
     setFixedSize (width, height) ; // mouse absolute x,y position
     七his->slider니-ypos = 0;
     七his-＞釘ider毗d七h = 24;
     this- >slider height = 16;



 void custom_slider_widget: :sliderHset max value(float value)
 {
     this- >max value = value;



 void custom_slider_widget: :slider中setm.mmn value(float value)
 {
      this- >min value = value;




slider set current value( ）는 Slider 위젯의 눈금이 위치한 값을 current_value 멤버변수에 저장하
고 눈금이 위치한 Y좌표를 계산하기 위해 피센트로 환산하여 slider_ypos 멤버변수에 저장한다. m1lt형
멤버함수 slider_g毗_current_value(）는 현재 설정된 current value 멤버변수를 리턴한다．



                                                             ＆사용자 정의 커스텀 위젯과 플러그인 141


===== PAGE 143 =====
 Void custom_slider_widget: :slider_set_current_value(float value)
      {
          this- >current value = value;


          float percent2 = (100 I this- >max_value) ;
          this- >slider스／pos = percent2 * value;
          this- >slider_ypos = abs (this- >slider_ypos - this- >w_height)
                                    - (this- >sllder_height/ 2) ;
 I

 mnt custom slider widget: :slider get_current value ()
 {
     return this- >current value;
 I.
valueChanged( ) 시그널 함수는 사용자가 Slider 위젯의 눈금을 마우스로 드래그（Drag）하면 emit를
이용해 시그널 이벤트를 발생한다. 이 시그널은 슬라이더 눈금 위치를 피센트로 계산하여 슬롯함수의 인
자로 전달한다. 이 시그널이 발생하면 커스텀 위젯을 배치한 어플리케이션 소스 코드에서 작성할 슬롯함
수와 연결하기 위한 시그널 함수이다．

Slider 위젯 클래스에서 재정의된 paintEvent( ) 멤버함수는 사용자가 눈금의 위치를 변경하면 변경된
좌표로 눈금을 이동시키기 위해 Slider 위젯 Paint 영역을 다시 그린다．

 void custom_slider_widget: :paintEvent (QPaintEvent *event)
 {
          QUNUSED (event) ;
          QPainter painter (this) ;


          painter. setPen(gColor (255, 255, 255) );
          painter. setBrush(QColor (255, 255, 255) );
          painter.drawRect (12, 0, 0, this- >wheight) ;


          Qlmage image ( n : /resources/ slider-handle.png") ;
          painter. drawlmage(0, this- >slider了pos, image) ;




mouseMoveEvent( ）는 사용자로부터 마우스 이벤트를 처리하기 위해 선언한 멤버함수이다. 이 멤버함
수는 마우스 이벤트 중 마우스 왼쪽 버튼을 누른 상태에서 드래그하면 자동으로 호출된다. 마우스의 드래
그 영역은 위젯의 영역상에서만 적용되며 위젯의 눈금 영역을 마우스로 드래그하면 눈금의 Y좌표를 계산
하고 value（그hanged( ) 시그널 이벤트를 emit 한다．

변경된 눈금의 Y좌표를 위젯에 반영하기 위해 repaint( ) 함수를 호출한다. repaint( ) 함수는 入4apping
된 paintEvent ( ) 함수를 호출한다．




142 CHAPTER 03_ GUI 설계와 제작


===== PAGE 144 =====
 void custom_slider_widget: :mouseMoveEvent (QMouseEvent *event)
 {
     QUNUS丑D (even七 ) ;


     if ( (event->buttons () & Qt: :LeftButton) )
     {
         if ( event->pos () .x () >= 0 && event->pos () .x () <= this- >w width &&
              event->pos () .y () >= 0 && event->pos () .y () <= this- >w_height )


              if ( (event->pos () .y () -   (this- >slider놔height / 2) ) >= 0 &&
                  (event->pos ( ) .y ( )+(this- >sliderHheight I   2) ) <= this- >w height)
              {
                     this- >slider_ypos = event->pos ( ) .y ( )-(this- >sliderheight/ 2) ;
                     float percentl = this- >slider ypos / 84 * 100;
                     float percent2 = (100 / this- >max value) ;
                     mllt percent3 = percentl / percent2;
                     percent3 = abs (percent3 - this- >max value) ;


                     emit this- >valuchanged(percerit3) ;
                     this- >repaint () ;




           drawl之ect (12, 0/ 0, 乞his-＞叫 heigh乞｝;


            Q끄nage image ( ' : /resources/ slider- handle .png") :
            painter. drawlmage (0, this- >sliderjrpos, image) ;


（그림） Slider 커스텀 위젯 Paint 영역



지금까지 CPU USED와 Slider 커스텀 위젯을 작성하였고, 두 커스텀 위젯을 어플리케이션 프로그램
GUI 상에 배치와 Slider 커스텀 위젯의 눈금을 변경하면 CPU USED 커스텀 위젯의 레벨을 변경할 수
있도록 두 위젯을 연동할 수 있는 소스 코드를 작성하1 보도록 하자．


好 작성한 커스텀 위젯 배치와 사용 예저1
CPU USED와 Slider 커스텀 위젯을 사용하기 위해 widget.h 헤더 파일과 widget. cpp 파일에 소스 코
드를 추가해 보도록 하자. 커스텀 위젯을 GUI상어］ 배치하고 Slider 위젯의 핸들 영역인 눈금을 마우스로
드래그하면 Slider 위젯에서 시그널 이벤트가 발생한다．




                                                                       8 사용지 정의 커스텀 위젯과 플러그인 143


===== PAGE 145 =====
 CPU USED Widget                       Slider 出沁get




                     Slider뮈젯 匐gnal 과 연동




（그림） CPU USED와 Slider 커스텀 위젯간 기능 연동



시그널 이벤트가 발생하면 Cpu USED 커스텀 위젯 클래스에서 구현한 cpu_set_widgetjevel( ) 멤버
함수를 호출해 Cpu USE 사용 레벨을 변경할 수 있도록 작성하고 QWidget 클래스로부터 상속받은
set八Iask( ) 멤버함수를 이용해 윈도우의 모양을 리소스어］ 등록한 백그라운드 이미지로 변경할 수 있도
록 MASK 기능을 사용해보도록 코드를 작성한다．




                     1m=   1日H




                     MASK 롤 사용혀1
                     뮌 도우 모양 변 경




（그림） 윈도우 모양 변경



 孝include <Q七Widgets>
 #include "custom'ecpuwidget.h"
 #include H custom_slider_widget. h'


 class Widget : public QWidget
 {
     Q OBJECT


 public:
     Widget (QWidget *parent = 0) ;
     -Widget ( ) ;


 public slots:
     II Slider 시그널 이벤트와 연결할 슬롯함수
     void mvaluechanged(int value) ;


 private:                                                     0


144 CHAPTER 03_ GUI 설계와 제작


===== PAGE 146 =====
    cus七omcpuwidge七 火cp또J寸idge七； 7/ CPU USED 위젯 선언
    cus七omslider_widge七 火sliderm widge七； /7 Slider 위젯 선언


private:
    bool m embedded;
    QPixmap m．나device; // 윈도우 영역을 MASK할 백그라운드 이미지 리소스


protected:
    void update_background ( ); // 윈도우 모양을 변경


protected:
    virtual   void paintEvent (QPaintEvent* event) ;




소스 코드는 커스텀 위젯을 사용할 \A/idget 클래스의 헤더 파일이다. Widget 클래스 생성자의 Base 클
래스에서 Qt::FramelessWindowHint 상수 옵션을 사용하면 윈도우의 타이틀 바를 표시하지 않는다．

리소스에 등록한 백그라운드 이미지를 QPixmap으로 렌더링하고 윈도우 모양을 MASK하기 위해 구현
한 update_background( ) 멤버함수를 호출한다. 구현한 커스텀 위젯을 어플리케이션 윈도우 영역에 배
치하고 커스텀 위젯 멤버함수를 사용해 위젯의 초기값을 설정한다．

Widget: :Widget (QWidget *parent)
    : QWidget (0, Qt: :FramelessWindowHint) , membedded(false)
{
    Q皿USED(parent) ;


    upda七ebackground( ); I/ 윈도우 모양을 변경하:7 ' 위한 함수 호출
    setWindowTitle (tr ( "Custom Widget ' ));


    slider_widget = new custom slider_widget (this) ;             /7 CI刃 USED 위젯 선언
    slider1-widget->sllder set widget resize(24, 100) ;           7/ CI七 USED 위젯 크기
    slider widget->slider set_max value (22) ;                    /／최대값
    slider widget->sliderm set mmn value ( 0) ;                   /／최소값
    slider-nwidget->sliderHset_current_value ( 12) ;              // 눈금 위치의 디폴트 값


    cp뜨widget = new cus如m아世widget ( thi引 ;                        7/ Slider 위젯 선언
    cpu-widget->cpuHsetHwidgetmlevel
                    作liderwidget- >sliderge七놔curren七1value() ); // 레벨 디폴트값
    cpu widget->setGeometry (40, 100, 80, 100) ;
    slider widget->setGeometry (130, 100, 24, 100) ;


    /7 Slider 위젯 시그널 이벤트와 슬롯함수 연결
    connect (slider_ widget, SIGNAL (valuchanged(int) ), this,
                              SLOT (mvaluechanged(int) ));
}




                                                                 已사용자 정의 커스텀 위젯과 플러그인 145


===== PAGE 147 =====
connect( ) 함수는 Slider 위젯의 눈금이 마우스 드래그에 의해 시그널 이벤트가 발생하면 mvalue-
changed( ) 슬롯함수와 연결하기 위해 작성한다．

void Widget: :mvaluechanged(int value)
{
     cpu widget->cpu set widget level ( value) ;




슬롯함수에서는 Cpu USED 위젯 클래스의 cpu_set_widget_level( ) 멤버함수를 호출한다. 이 함수는
CPU 사용율을 변경하기 위한 기능이 구현되어 있다．

void Widget: : update_background ()
 {
     rn_device = QPixrnap ( " : /resources/background.png", n png") ;
     Qaitmap bitmap = rn_device. createHeuristicNask ( ) ;
     se七FixedSize (m device. size() ); I/ 절대좌표로 변환하71 위하1 사용하는 함
     setMask (bitmap) ;
     update ( ) ;




update background( ) 멤버함수에서 사용한 createHeuristicMask( ) 함수는 QPixmap을 MASK 하
기 위해 QBitmap을 생성하고 리턴하는 함수이다. 帥Widget 클래스로부터 상속받은 setMask( ）는
QBitmap 이미지를 위젯에 MASK를 하기 위한 멤버함수이다. update( ）는 repaint( ) 함수와 기능은
동일하지만 repaint( ) 함수에 보다 빠르게 렌더 링할 수 있도록 옵티마이징된 함수이며 paintEvent( ）를
한번만 호출할 수 있다．


                    CPU USED Widegt


                    SLIDER Widget




（그림） 사용자 정의 커스텀 위젯을 사용한 예저1



작성한 예제를 실행해 보고 Slider 커스텀 위젯의 눈금을 마우스로 드래그해 CPU USED 커스텀 위젯의
사용율이 변경되는 것을 확인해 보자. 지금까지 사용자 정의 위젯을 구현하고 사용하는 방법에 대해 살펴
보았다. 다음 장에서는 구현한 사용자 정의 커스텀 위젯을 배포할 수 있는 플러그인으로 제작하기 위한
방법을 살펴보자．




146 CHAPTER 03_ GUI 설계와 제작


===== PAGE 148 =====
         8.2 플러그인 제작과 배포

이전 장에서 구현한 커스텀 위젯을 플러그인으로 제작하고 Qt Designer에서 커스텀 위젯을 GUI 인터페
이스 상어］ 배치하고 사용할 수 있는 방법에 대해 살펴보도록 하자．




（그림） 커스텀 위젯 플러그인 Add-On과 GUI 배치



Qt에서는 커스텀 위젯을 Qt Designer의 플러그인으로 제작하고 그림에서 보는 것과 같이 사용할 수 있
도록 기능을 제공한다. 이번 장에서는 두 가지 예제를 다룰 것이다. 첫 번째 예제는 Cpu USED와
Slider 커스텀 위젯을 플러그인으로 제작 및 배포할 수 있는 예제를 구현하고, 두 번째 예제에서 제작한
플러그인을 Qt Designer어］ Add-On하고 GUI 인터페이스에 배치하는 예제를 다루어 보도록 하자．


e （값 De이gner에서 사용할 커스텀 위젯 플러그인 제작과 배포

(File] .> (New File or Project...]



  如m1 nh mn이代Ln
  01片n Am 쁘Rh山
                                                1申


                                艮               斗肖
                                                nfl甘11（느口m8   二二系m kr寸二긔tt工mt1e01札0,.口a,
                                                                                      ."
                                   缸tire ,      C..             n4 伽mt긔nCML C工1m呻1Pk中t
  Seseo.r                   >          -        Qi              1口 0,0,.,,., ,디.r.

  Se勺e                 cw.s 川카8                                     Cm幽e크 日 Cr 口J5mm D們巴mr W
                                                                    CU5te1n 나 - C이mdKm
  S. , 塑0                       TI.
                                    小cm烈아
  鈿e蚣             口n ' 텨겨51*5   鈿m啼出녑R니

                                口01501 eQS （二




（그림） 커스텀 위젯 플러그인 프로젝트 생성 ］단겨1



프로젝트를 생성하기 위해 왼쪽 탭에서 [Other Project] 탭을 선택하고 오른쪽의 리스트 중 [QtCustom
Designer Widget] 항목을 선택한다．




                                                                                               ＆사용자 정의 커스텀 위젯과 플러그인 147


===== PAGE 149 =====
                  I.寸e0由址好曲 a忖 p.升1m 1此1dm

                  1m1 nU미d 1日寸小1 1 m4 마1뿌r出t C山好n 났心m m a 며4 마m好n目山日4口C- -口Xm
                  呻




                                                               Pr이ect 1기rectory Nan犯

                                                                             Parent Directory of Project




                                                                        山mW

                     Um mmn1二 1月마미三 mm=m




（그림） 커스텀 위젯 플러그인 프로젝트 생성 2단7카



Name 항목에 "custom_cpu_widget" 을 입력하고 [Next] 버튼을 클릭해 다음 화면으로 넘어간다．

                        弔多m料凞蚤m饗缸小m：
                                   玉뇩4出心吐H

                        Custom Wdget List
     岫1

 +   Cu료예1 낵H垠eiS       S口mry t蜘 h코 0( 口后bn nq1et5 미넙 ftn   미呼似丘

                                                                                           Widget Class Name to create
                        w心m口a占油 唯1              ‘로J1在r
                         CU디어기 q노J nK］云                                 im   岐거a,
                         ! Ne川 C附＄5>
                                                                    1   1뇌me 며아哨
                                                                                          Custom Widget headerfile and
                                                                                          source file
                                                  w띠p.. 며아出土


                                                  w心p.. 唾出沁'C

                                                  Wr녑m qm 虹E f11e


                  多塑匈 쁘心get5                      나1叩이 므aCtual. SWM芼e(
                                                                              尸戶才 custom wiaget nase ciass
                                                                        ,m,, 尸．
     乙    Label




                                                                                        Class name and file name
                                                                                        化r Qt Dc引gnerF기t崎in
                                                                        口m
                      C小tmj 나任吼小




（그림） 커스텀 위젯 플러그인 프로젝트 생성 3단겨1



Custom Widget 그림에서 [+] 아이콘 버튼을 클릭하고 "custom_cpu_widget" 항목을 입력한다. 그림
에서 보는 것과 같이 입력할 수 있는 필드가 활성화 되면 다음 표와 같이 값을 입력한다．

항목                                            필드 입력값

Widget Project tile                           custom_cpu_widget.pri
쌔dget header 꿰e                               custom_cpu_widget.h
Widget source tile                            custom_cpu_widget.cpp
Widget base class                             oWidget
Plugin header file                            custom_cpu_widget plugin
F기ugin source file                            custom （가乂i_widget이ugin.h
F기ugin source 川e                              Custom_c口u小／dget引ugln.Cpp




148 CHAPTER 03_ GUI 설계와 제작


===== PAGE 150 =====
그림의 마지막 Icon file 항목은 Qt Designer의 위젯 탭에서 플러그인 위젯을 표시할 아이콘을 지정할
수 있다. 아이콘을 지정하지 않으면 Qt Creator에서 기본으로 제공하는 디폴트 아이콘을 사용한다．


                                                              Qt CustGrn De＞出ner Wkhit


                                        Plugln and Co如Ct沁n 이ass Informat沁n
                     Locati어）
                     Cu客torn Wi叱ets     Sc比아y the 아叩미如＄ cit the ph堰in hbca가 and the cc琳ection dass.

                   牛 P的魯fl Det며悴
                                        C어旭coon C總55:
                      늬 Jd 1   묘n " r


                                        C어沌cc山nh也81ef lile: ;


                                        Cc出ection 吼照玗｛갸，多 寸小小： ;


                                        F가ugn name:                mrmm口丕二工及
                                        Reso4i旺老 fi晦：              心거15.(恥




（그림） 커스텀 위젯 플러그인 프로젝트 생성 4단겨1




Plugin name 항목의 입력 필드에서 "custom_cpu_widgetplu얹n" 을 입력한 후 [Next] 버튼을 클릭하
면 프로젝트 생성이 완료된다. 프로젝트 생성이 완료되면 Qt Designer가 인식할 수 있는 플러그인 클래
스와 CPU USED 커스텀 위젯을 구현할 클래스가 생성된다．


                  P佃g巾1 허1더 파일고｝ 소스파일


                  [Qdeslgner Custom Widget Interface]
                          CI怡tom_cp吐叫idgetpl四in.h
                          custom_cpu_wldgetplugin.cpp

1Custom出idget헤더                             파일과소스파일                    ]
                  [Custom CPU Widget]
                          custom_cpu_wldget.b
                          CI心tom_cF川i_widget．
                                            印P4

（그림） 플러그인 클래스와 커스텀 위젯 클래스




플러그인 클래스는 Qt Designer 상어］ Export할 기능을 담당하는 클래스이며 Qt Designer 상에서 배
치할 위젯 그룹명 , 위젯명 등과 같은 정보를 Qt Designer와 통신하기 위한 인터페이스를 제공한다．
CPU 커스텀 위젯 클래스는 이전 장에서 작성한 소스 코드와 같이 기능을 구현할 클래스이다. 플러그인
클래스 구현에 필요한 멤버함수를 살펴보자．




                                                                                                      ＆사용자 정의 커스텀 위젯과 플러그인 149


===== PAGE 151 =====
class custorncpuwidgetPlugin :
          public QObject, public QDesignerCustomWidgetlnterface
 {
      Q OBJECT
      Q INTERFACES (QDesignerCustornwidgetlnterf ace)


public:
      custorn_cpu_widgetPlugin(QObject *parent = 0) ;

      bool isContainer () const;
      bool islnitialized () const;
      Qlcon icon() const;
      QString dornXml() const;
      QString group() const;
      QString includeFile() const;
      QString name () const;
      QString toolTip() const;
      QString whatsThis () const;
      QWidget *createWidget (QWidget *parent) ;
      void initialize (QDesignerFormEditorlnterface *core) ;

private:
      I均（>1 rn inj土ialized;
 };
플러그인 클래스 QObject 클래스와 QDeB培n餌沁stomWi1getInterface클래스를 상솎 받는다．
QObject는 Qt 클래스에서 기본이 되는 클래스이며, QDesignerCustomWidgetlnterface 클래스는
Qt Designer가 접근할 수 있도록 \Widget Interface가 정의된 클래스이다. Q끄寸TERFACES( ）는 Qt
Designer와 통합하기 위해 작성된 소스 코드이다.

다음 라인의 플러그인 클래스의 생성자는 QObject를 호출하고 rn_initialized의 값을 FALSE로 지정하
여 초기화 되지 않은 플러그인이 초기화 되지 않은 상태로 설정한다．

cus七orn그p뜨widge七Plugin: :cus七orn叩뜨widgetPlugin ( QObjec七 出parent)
    : QObject (paren七)
 {
      mHinitialized = false;
 }


다음 라인의 bool 값을 리턴하는 isContainer( ）는 커스텀 위젯이 Child 위젯을 포함하고 있는지 여부를
Qt Des培ner에게 알려주기 위한 멤버함수이다. False를 리턴하면 커스텀 위젯 내에 다른 Child 위젯을
사용할 수 없다. Ti'ue릍 리턴하면커스텀 위젯 내에 Child 위젯을포함할 수 있다. 따라서 구현할 커스
텀 위젯에 Child 위젯을 포함한다면 true를 리턴하도록 구현해야 한다．




150 CHAPTER 03_ GUI 설계와 제작


===== PAGE 152 =====
1bool cus的IT느cp뜨widge七Plugin: :isCon七amner ( ) cons七
i {
                    return false;
 }

islnitialized( ) 함수는 Qt Designer가 커스텀 위젯을 사용할 준비가 되었는지 판단하기 위한 멤버함수
이다．

 b（그ol custort느叩uwidge七P1끄gin: :islnit江alized ( ) cons七
 {
                    return m initialized;
 }


Icon( ) 함수는 Qt Designer의 위젯 박스에 나타날 아이콘을 지정하는 멤버함수이다. 지정하지 않으면
Q묘L기본으로 제공하는 아이콘을 사용한다．

 Qlcon custom_cpu_widgetPlugin: : icon() const
 {
                    return Qlcon ( );




田 QDec治rat押eView
Q
三：'
         QWebView
                          탸an冽e Cust먀n Widget

四 cu歌町啣ymm
                                                小二｝
回 cu없om죄曲－나唾et

（그림） 플러그인 위젯 아이콘



 面Xm1( ) 함수는 커스텀 위젯의 클래스명, 커스텀 위젯의 이름, x좌표와 Y좌표, 위젯의 크기 , 플러그인
 위젯의 위젯 박스에서 마우스 포인터를 올려놓으면 표시할 툴팁 메시지 등의 정보를 Qt Design아에게
 QString 타입으로 리턴하기 위한 멤버함수이다．

  QString custom cpum widgetPlugin: :domXml() const
     {
                     return QLatinlString( "<widget class=\" custom_cpu widget\ " "
                                           "name=\" custom_cpu_widget\ " >\n</widget>\n") ;
                     ／士
                     return '1<ui language=\" c++\" >\n"
                             ' <widget class=\"customcpuwidget\ " "
                            " name=\" custom下r乂I T姓dg毗＼1' >\n"
                                    <property name=\" geometry\ " >\n"
                                n


                                     <rect>\n"
                                n
                                      <x>O<Ix> <y>O< /y>\n"
                                n
                                      <width>80</width> <height>100</height>\n"                        0

                                                                                  ＆사용자 정의 커스텀 위젯과 플러그인 151


===== PAGE 153 =====
                          </rect>\n"
                        </pr아氾r切놔nfl
                        <property name=\"toolTip\ " >\n"
                         <string>Custom CPU Widget<I string>\n"
                        </pr아尼rty> \n"
                        <property nanie=\ "whatsThis\ " >\n"
                         <string>This is a Custom CPU Widget.</string>\n"
                        </pr아冶rty> \n"
                       </widget>\n ";
      火／
 grouj乂 ) 함수는 커스텀 위젯이 포함될 위젯 박스 그룹을 Qt Designer에거，1리턴하는 함수이다． 지정한
 그룹이 위젯 박스에 없으면 새로운 그룹이 생성된다. includeFile( ）은 커스텀 위젯의 헤더 파일을 명시
하고 name( ) 함수는 위젯 박스상에 표시될 커스텀 위젯의 이름을 Qt Design町에게 리턴하기 위한 멤
버함수이다．

 QString custom_cpu_widgetPlugin: :group ( ) const
 {
      // 커스텀위젯이 포함될 그룹 명을 리턴, 없으면 새로운 그룹이 생성
      return QLatinlString( "Exaniple Custom Widgets ") ;
 }

 QString custom cpu-widgetPlugin: :includeFile ( ) const
 {
           return QLa七mniS七ring ( "custom.cpuwidget.h") ; // 커스텀 위젯의 헤더파일




                       텨a'꺄陀 Cu없ml 出k坦et
                   1
               ｛沁S打）mmc아j WIC妊et


            回   Cu없町帥der_             wfdget
（그림） 커스텀 위젯이 포함될 그룹명



 QString custom_cpu_widgetPlugin: :naxne ( ) const
 {
     re七urn QLa七iniString( "custom_cp뜨widget") ; // 커스텀 위젯명
 }




                                               뇨
           qr 12weov田

              C나stOm_c叩나I(坦et

           回 Cust帥쏴er毗get
               J>r 乙口會 to !Cfl二薛tE三


（그림） 커스텀 위젯 이름


152 CHAPTER 03_ GUI 설계와 제작


===== PAGE 154 =====
toolTip( ) 함수는 커스텀 위젯 위에 마우스 포인터가 위치하면 툴팁（To아Ti히을 표시하기 위해 Qt
Designer 에게 메시지를 리턴하고, whatThis( ）는 위젯에 대한 긴 설명이 필요한 메시지를 리턴하기 위
해 구현된 멤버함수이다．

 QString custom_cpu_widgetPlugin: :toolTip () const
 {
      return QLatinlString( "Custom CPU Widget ") ;
 }

 QString custom cpu-widgetPlugin: :whatsThis () conat
 {
      return QLatinlString( "This is a CPU USED Custom Widget. ") ;
 }


           Q QWebVtew
                 Ex이꺄杷 C嶠t엔 世
           回 cu없帥工叩艸恥t
           心尸叩프畦뇨torn C뎌3卿et
               j工 Ty口e to (光ate

（그림） 커스텀 위젯 툴팁



印Widget을 리턴하는 createWidget( ）는 플러그인 커스텀 위젯 구현을 단순화 하기 위해 구현된 함수이
고, 커스텀 위젯의 Parent 클래스를 리턴한다．

 QWidget *customcpuwH1寸idgetPlugin: : createWidget (QWidget *parent)
 {
      return new custom_cpu_widget (parent) ;
 }

마지막으로 initialize( ) 함수는 Qt Designer가 커스텀 위젯을 초기화 할 때 호출하는 멤버함수이다．
이 함수는 커스텀 위젯을 초기화시키기 위해 PRIVATE으로 선언한 rn_initialized 변수를 true로 변경
한다．

 void custom cpu widgetPlugin: :initialize   (QDesignerForntEditorlnterface *
 {
      if    (minitialized)
            return;


      m initialized     = true;




지금까지 살펴본 플러그인 클래스는 커스텀 위젯을 Qt Designer가 커스텀 위젯을 Export 하고. GUI
상에 커스텀 위젯을 배치하거나 프로퍼티 정보를 제공하기 위해 구현한 클래스이다．


                                                               已사용자 정의 커스텀 위젯과 플러그인 153


===== PAGE 155 =====
다음으로 살펴볼 Cpu 커스텀 위젯 클래스의 헤더 파일과 소스 파일은 이전 장에서 구현한 컨슨뵤윈젯과
다른 점은 클래스 선언 시 QDESIGNER_WIDGETEXPORT키워드를 클래스명 앞에 명시해야 한다．

#include <QtDesigner/QDesignerExportWidget>


class QDESIGNER_WIDGET_EXPORT custom_cpu_widget : public Qwidget
 {
        Q OBJECT


public :
        cus七이tF9느widget (QWidget 火parent = 0) ; // CI七 위젯 클래스 생성자
        void cpu_se七J吐dget_level (int level) ;             II CPU 사용레벨을 설정




이전 장에서 작성한 커스텀 위젯 헤더 파일을 앞의 예제와 같이 수정하고 프로젝트를 발튿화면 libcus
tom_cpu_widge삐ugin. SO 동적 라이브러리 파일을 Qt가 설치된 디자이너 하위 플러그인 디렉토리어］
복사한다．


     Custom CPU Widget Plug-in             컴파일로 생성된
                                           Custom Widget
     Custom Slider Widget Plug-in            라이브러리


                                                 1
                      Qt Designer Integration

（그림） 생성된 동적 라이브러리 복사



작성한 라이브러리는 STATIC과 DYNAMI(그 방식으로 분류된다. 플러그인을 빌드（Build）해 생성된 동적
라이브러리는 어플리케이션 개발 시 실행 바이너리에 포함되지 않는다．

따라서 CPU와 Slider 커스텀 위젯의 동적 라이브러리는 어플리케이션이 동작하는 파일 시스템 상어］ 참
조할 수 있는 디렉토리에 존재해야 한다. 커스텀 위젯의 동적 라이브러리가 위치한 디렉토리를 명시하기
위해서는 project 파일어］ 명시해야 한다．

지금까지 Qt Designer상에서 사용할 커스텀 위젯 플러그인 제작과 배포 방법은 CPU 커스텀 위젯을 위
주로 살펴보았다．


. 커스텀 플러그인 위젯을 이용한 어플리케이션 작성
이전에 다룬 커스텀 위젯을 어플리케이션 GUI상어］ 배치하고 Slider 커스텀 위젯의 눈금을 변경하면
CPU 커스텀 위젯의 사용 레벨이 변경되도록 소스 코드를 작성해보자. 프로젝트 생성 시 Qt Designer를
사용해 커스텀 위젯을 배치할 수 있도록 [Generate form] 항목의 체크박스를 체크하고 프로젝트를 생성
한다．


154 CHAPT타긋 03尸 GUI 설계와 제작


===== PAGE 156 =====
      Class name:           Wi叱et

      孕se dass:            ; QWN*et
                 ／戶                        'dn



      He    rf        Generate form 향목의 又II
                      스 활성 화
      鈿t丑（a fi
                                맣
                      f이m: 'f
       如
      Fonn N. :
 I；
                            Wdget.Ut


（그림） 프로젝트 생성 마법사 （기ass Inf아m計山n 다이얼로그



프로젝트 생성이 완료되면 Qt Creator 프로젝트 내비게이션상에 w姓get.ui 파일을 더블 클릭해 Qt
Designer로 전환한다. 다음 화면과 같이 GUI상어］ 이전 예제에서 Export한 커스텀 위젯을 마우스로 드
래그해 배치한다．



                                                                                ClOb. Wbt甲C   Cu引o.e_ Cpumw띠get
                                                                                引心or wotget   CustOfll_引心er 出K坦a




                                                                     /1H


                                                                      ［주의사朗

                                                                       커 스텀 위 젯 귿4스 명과 인 스텬스
                                                                       멓이 동일하지 않도폭주의
                                        커 스텀 위 젯율 마우스로 드래 그
                                        하여 t月상0$ 뼈치                    Wldget    Q
                                    \                                  Port比八y




（그림） GUI 상에 커스텀 위젯 배치와 인스턴스 이름 변경



화면에서 보는 것과 같이 커스텀 위젯을 UI상에 배치하고 widget.h 헤더 파일어］ 다음과 같이 소스 코드
를 추가한다．

 public slots:
           void mvaluechanged(int value) ;



Slider 커스텀 위젯의 크기 , 슬라이더의 최소값과 최대값, 눈금이 위치할 디폴트 값을 Slider 커스텀 위
젯 클래스의 멤버함수를 사용해 설정할 수 있다．

Slider 커스텀 위젯의 눈금을 마우스로 드래그하면 시그널 이벤트가 발생하고, connect( ) 함수를 이용
해 mvaluechanged( ) 슬롯함수와 연결할 수 있도록 생성자어］ 다음과 같이 소스 코드를 추가한다．


 ui- >slider_widget->slider_set_widget_resize (24, 100) ;                                                     // 위젯 크71
 ui- >sliderwidget- >slider_set_max_value (22) ;                                                              /／최대값
 ui- >slider1widget->slidermset-mmn value ( 0) ;                                                              /／최소값
 ui- >slider widget->slider set current value ( 12) ;                                                         // 눈금위치의 디폴트 값


  // 시그널과 슬롯함수 연결
  connect (ui- >slider widget, SIGNAL (valuchanged(int) ), this,
                                                      SLOT (rnvaluechanged(int) ));



                                                                                                          ＆싸용자 정의 커스텀 위젯과 플러그인 155


===== PAGE 157 =====
connect( ) 함수를 이용해 연결한 mvaluechanged( ) 슬롯함수는 Slider 위젯의 눈금이 변경되면 CPU
커스텀 위젯의 CPU 사용율을 변경할 수 있도록 다음과 같이 소스 코드를 작성한다．

 void Widget: :mvaluechanged(int value)
 {
         ui- >cpu widget->cpu set widget level(value) ;




커스텀 위젯의 동적 라이브러리 헤더 파일을 참조할 수 있도록 프로젝트 상에 헤더 파일을 추가한다．

          d口 八八키 r丁a4n;m
                                          C口nfl日ct (ui- ＞드1
          DC吐 甘岫曲i exan出K

          expo凡we坦供_exam이e．口ro
     '7 庚i Headers
          h Custom c머JWI(坦et.h
          !   CUS的m引IC地r 쌔dget.h
          h 베喀吼h                          Ui戶＞cpu-w끄jn
     口 圍 鈿urtes
          國 marn.cpp       1   커스텀위젯라이브러리헤더과일 추사
         國 나K坦etc텍｝
     口 曲 Forms                            delete ui :
          寸／ w,姐映JJ


（그림） 커스텀 위젯 동적 라이브러리 헤더 파일 추가



프로젝트의 속성이 저장된 pr이ect 파일어］ 다음과 같이 LIB 옵션을 추가한다．

 LIBS += Irooti libcustom cpu widgetplugin. so
 LIBS += /root/ libcustom_sliderwidgetplugin. so


예제를 빌드하면 프로젝트 속성 파일을 참조해1Makefile을 생성한다. Makefile은 커스텀 위젯 동적 라
이브러리가 포함된 PATH이므로 Build한 예제를 실행할 파일 시스템 상의 PATH에 커스텀 위젯 동적
라이브러리가 존재해야 한다. 그리고 프로젝트 파일에 명시한 LIBS 옵션 PATH와 동일해뺘 한다．




（그림） 카스텀 위젯 예제 실행 화면



빌드가 완료되면 화면에서 보는 것과 같이 예제 어플리케이션을 실행해 보고 GUI 상에 배치한 Slider 커
스텀 위젯의 눈금을 마우스로 드래그해 CPU 커스텀 위젯의 사용율 값이 변경된다．

지금까지 커스텀 위젯을 구현하는 방법과 구현한 커스텀 위젯을 플러인으로 제작하고 배포할 수 있는 방
법에 대해 살펴보았다. 플러그인 제작과 배포는 API를 모듈로 분리하거나 Qt가 제공하는 API 외에 다른
API를 Qt API 모듈로 추가할 수 있는 프레임워크를 제공한다. 예를 들어 JPEG, FREETYPE 등과 같
은 라이브러리를 Qt API로 추가할 수 있다．


156 CHAPTER 03_ GUI 설계와 제작


===== PAGE 158 =====
CHAPTER




시그널과 슬롯


===== PAGE 159 =====
（그t5F가（jgramming




I尸러 시그널고F슬록
             객체 간의 통신 혹은 이벤트를 처리하기 위해 시그널과 슬롯을 제공한다. GUI 상에서 발생한 이벤트를
             처리할 수 있는 방법뿐만 아니라 객체 간의 데이터 통신을 위한 방법으로 사용할 수 있다. 따라서 이번
             에 다루는 내용을 꼭 숙지하도록 하자．




客雙受땠多횬친힛多世e븐矩갇읜兵多邑윈j比堤好'］다· GUI 프로그래밍어］서 버튼 위
젯을 사용자가 클릭했을 때 지정한 함수를 실행하기 위해서 시그널과 슬롯을 사용하면 원하는 함수를 실
행할 수 있는 매커니즘을 제공한다. 시그널과 슬롯은 사용자의 다양한 이벤트를 처리하기 위해 다양한
Callback 함수를 제공한다．

Qt에서 제공되는 모든 위젯은 미리 정해진 다양한 시그널을 가지고 있다. 예를 들어 QPushB毗ton의
click, double click, mouse over 등과 같이 다양한 시그널이 정의되어 있다. 슬롯도 기본으로 제공하
                                     r\   /   \/\/   \/V    ＼尸 기／ \/   \n／   八m八느／느d八느尸戶＼

庭上壁르足史밋．     多1炅戈됨다· 예를 들어 valueChanged( ）와 같' ] 값을 변경가기 위해 기본으로
제공되는 Virtual 함수이며 재정의해 사용할 수 있다.

인뽀튼갼是졀쁘쁘므曳견쓰므쁘］라면色츠彭뽀星쁘，브르是斐冕전곗할함수를 "］정
해주는 함수이다. 시그널과 슬롯은 하나의 파이프라인과 같이 생각하면 된다．

시그널과슬롯은항상 1: 1 ufi칭되는 것은 ' ｝니다· 하나완二프쁘브-r읫흐츠관坐交哭曼수 있
다. 슬롯도 마찬가지로 여러 개의 시그널 입력을 하나의 슬롯을 통해 연결할 수 있다．


   Objec12         Object3    Objecti                      Object2

    引gnall                                                 signall




（그림） 시그널과 슬롯


마우스 클릭의 이벤트 발생 시 특정 함수가 실행되는 슬롯을 연결하기 위해서는 connect 함수를 사용하
면 된다．




158 CHAPTER 04_ 시그널과 슬롯


===== PAGE 160 =====
bool QObject: :connect ( const QObject * sender,
                     const char * signal,
                     const char * method,
                     Qt: :ConnectionType type = Qt: :AutoConnection ) corist


bool QObject: :disconnect ( const QObject * sender,
                     const char * signal,
                     const QObject * receiver,
                     C（끄lS七 char 火 method ) [5七a七i（그］



connect 함수는 시그널과 슬롯을 연결하는 함수이며 , 마우스 click 이벤트 이외에 직접 용도어］ 맞는 시
그널과 슬롯을 정의해 사용할 수 있다．

class SignalSiot : public QObject
{
     Q OBJECT
public:
     SignalSlot () { mvalue = 0; }
     mnt value () const { return m.mvalue; }


public slots:
     void setValue (int value) ;


signals:
      void valueChanged(int newValue) ;


private:
      mnt m value;
};


駐gnalSlot 클래스는 駁gnals 함수로 value（그hanged(int newValue) 함수를 선언했다. 이 함수는
private으로 선언된 클래스 멤버변수 m value 값을 newValue 값으로 변경하는 함수이다. 그리고 Si毗
함수로 setValue 함수를 선언하였으며, 이 함수를 사용하면 시그널 함수로 선언한 value（그hanged(int
newValue) 함수가 시그널로 연결된 슬롯함수를 실행한다．

void SignalSiot: :setValue (int value)
{
     m value = value;
     emit valueChanged (mvalue) ;




emit은 시그널 함수를 수행하끼 위해 사용하는 키워드이다. 코드에서 보는 것과 같이 수행할 시그널을
em此으로 지정하면 connect 함수로 지정된 시그널 이벤트가 발생한다．




                                                                               ] 시그널과 슬롯 159


===== PAGE 161 =====
Lb1 = new Qlabel ( " ", this) ;
 ibl- >setGeometry (10, 10, 100, 40) ;


 SignaiSlot si,   s2;
 QObject: :connect (& si,    SIGNAL (vaiueChanged(int) ),
                            &s2, SLOT (setValue (int) ));


 si. setVaiue (50) ; /7 sl. value = 50, s2.vaiue = 50
 ibl- >setText (QString ( "%i " ).arg(s2.value ( )fl;



si 클래스의 값을 50으로 변경하면 시그널이 발생한다. 이 시그널과 연결된 슬롯함수는 s2 클래스의 set
-Value 함수와 연결한다. 따라서 si 클래스와 s2 클래스의 멤버변수 m value의 값은 동일한 값으로 변
경된다．

=Custom Signal Slot

 50




（그림） Cu없om Sign졔과 Slot 실행 화면




                                                                  >



160 CHAPTER 04_ 시그널과 슬롯


===== PAGE 162 =====
    CHAPTER




데이터 타입과 유용한
 데이터 조작 클래스


===== PAGE 163 =====
Qt 5 Programming




            1 // 데이터 타입과 유용한
                 데이터 조작 클래스
            0+＋에서 제공하는 기본적인 데이터 타입 이외에 아는 개발자7F 유용하게 사용할 수 있는 다양한 데이
            터 타입을 제공한다. 아는 제공하는 데이터 타입을 기본 데이터 타입과 클래스 형태의 데이터 타입을
            제공한다. 따라서 이번 장에서 （가가 제공하는 데이터 타입에 대해 알아보도록 하자．




 Qt는 다양한 플랫폼을 지원한다. 작성한 어플리케이션이 다양한 플랫폼어］ 동일한 크기를 갖는 데이터 타
 입이 필요하다. 예를 들어 어플리케이션 작성 시 quintl6, quint32와 같이 정수형 데이터 타입의 플랫폼
 이 달라도 작성한 어플리케이션에서 데이터 타입은 동일한 크기를 갖는 것이 중요하다. Qt에서는 정확한
 크기를 지정할 수 있도록 다음과 같은 데이터 타입과 클래스를 지원한다．


 . 기본 데이터 타입

 타입                 크기        설명
  bool              8 bit     true / false
 （기nt8              8 bit     signed char
  대ntl6            ! 16 bit   signed short
  qint32            32 bit    signed mnt
  이nt64             64 bit    long long nt
  qu1n18            8 bit     unsigned char
  quintl6           16 bit    unsigned short
  quint32           32 bit    unsigned mnt
  quint64           64 bit    unsigned long long mnt
  加at                32 bit   IEEE 754 포맷을 사용하는 floating 口이nt number
 （幻ub冶               64 bit   IEEE 754 포맷을 사용하는 floating p이nt number
  const char*        32 bit   문자열 상수를 가리키는 포인터, 마지막에 0 제외



  . 데이터 클래스
  클래스                설명
  QBitArray          비트 연산（AND, OR, X아？, NOT）을 제공하기 위한 bit Array
  OBrush             QPainter에서 그려지는 도헝의 칠하기 타입을 정의하기 위한 타입
  QBy也Array          Byte 단위 Array를 지원하는 클래스. 만약 Array가 Null이면 0xFFFFFFFF (quint32)
  OC이or              RGB, HSV 그리고 CMYK 값 기반으로 C이or를 제공하71 위한 클래스
  OCursor            마우스 커서의 도형을 정의하기 위해 제공하는 클래스


  162 CHAPTER 05尸 데이터 타입과 유용한 데이터 조작 클래스


===== PAGE 164 =====
클래스                설명
QDa伯               날짜 Function을 제공하기 위한 클래스
QDateTime          날짜와 시간 Function을 제공하기 위한 클래스
QEasingCurve       GUI 상에 Animat山n의 움직임 패턴을 제어하기 위한 데이터 클래스
QFont              테스트를 표현하기 위하1 폰트를 설정하는 클래스
（긔con              모드와 상태7F 다른 아이콘을 제공하기 위한 클래스
（긔mage             이미지를 표시하기 위한 클래스
QKeySequence       Shortcut 키를 지정하기 위해 제공하는 클래스
QMar이ns            left (int), to口 (int), right (int), bo卄om (int) 사각형의 각 Mann을 처리하71 위한 클래스
QM計rix             2D를 변형하기 위해 정의된 클래스
QMatrix4x4         3D 4x4의 변형을 위하1 정의된 클래스
OPalette           각 위젯 상태의 컬러 그룹을 포함하는 클래스
OPen               그려지는 Line의 스타일, 두께, 컬러를 제공하71 위해 제공하는 클래스
OPicture           F기cture 이미지의 포맷을 처리하기 위하1 제공하는 클래스
아거xmap             PNG와 같은 포맷의 이미지를 처리하기 위해 제공하는 클래스
QPoint             X, V. Z 값을 처리하기 위하1 제공하는 클래스
OQuafernion        벡터 및 스칼라로 구성된 Quatern山n을 처리하기 위한 클래스．Quatern山n는 3D 공간에서 회
                   전을 대표하고, x. y 및 z 좌표와 회전 각도를 대표하는 스칼라에 의해 지정된 3D 회전 축으로
                   구성하는 데 사용된다．
ORect              사각형의 left (qint32), 幻口 呵nt32), right (qint32), bot幻m (qint32)
QRegExp            정규화 표현식을 처리하기 위한 클래스
0Reg미arExpres듸on   정규화 표현식을 처리하71 위한 클래스
QRegion            Painter 상에서 클립보드 영역을 정의하71 위해 사용하는 클래스
OSize              넓이와 높이를 사용하먀 하는 목적의 클래스． wi아h (qint32), height (qint32)
oSlring            문자열 처리를 위하1 제공하는 클래스． 문자열이 Null인 경우 0xFFFFFFFF (quint32),
QTime              시간， 분， 초, 卜川Ilisecond를 다루기 위한 클래스
QTransform         크71, 전단（shear), 회전, 좌표 등을 그래픽 렌더링하31 위하1 사용되는 클래스
QUrl               URL 주소 (QString)
QVaniant           다양한 종류의 데이터 타입을 저장할 수 있는 union 형태의 클래스
QVector2D          2차원 공간에서 Vector 또는 ＼尼rtex를 나타내기 위한 클래스
QVector3D          x, y, z 3개의 좌표를 사용해 3D 그래픽을 Drawing 하거나 표현할 때 사용하는 클래스
QVector4D          4차원 공간에서 \/ector 또는 vertex를 나타내71 위한 클래스




                                                                  l 데이터 타입과 유용한 데이터 조작 클래스 163


===== PAGE 165 =====
S Container 클래스

클리倭                    설명
QHash(Key, T)         Hash 테이블 기반의 ［거ctionary를 제공하71 위한 템플릿 클래스
OMap(Key, T)          텨na四 Search tree 기반 E기ct山nary를 제공하기 위한 템플릿 클래스
QPairKT1, T2)         쌍으로 존재하는 아이템 데이터를 처리하기 위한 템플릿 클래스
QList(T)              List 형태의 값을 다루기 위하1 제공하는 템플릿 클래스
OLin kedListT)        링크 리스트를 제공하기 위한 템플릿 클래스
QVector(T)            동적인 OVector 배열을 다루기 위하1 제공되는 클래스
QStackCD              口ush(), 口opO, top(）을 이용한 앉ack을 사용하71 위하1 제공되는 클래스
QQueue(T)             enqueue(), dequeue( ) 그리고 head(）를 이용하1 디FO 구조의 데이터 조작을
                      위해 제공되는 클래스
OSetKT)               해시 기반의 빠른 검색을 위하1 제공되는 클래스
QMap(Key, T)          Key 값에 의해 Mapping 되는 데이터를 하나의 조합으로 연결되어 미ctiona四를
                      제공하고, QMap 클래스는 키 순서로 데이터를 저장할 수 있다．
0卜爪기tiMa口（Key, T)     QMa口으로부터 상속받은 클래스로, 다중 M햐가기ng 값을 이용할 수 있다．
QMultiHash(Key, T)    QHash 로부터 상속받은 클래스로， 다중 Ma口口ing 값을 이용하1 해시를 사용할 수
                      있다．




斗 문자열 클래스

큘래스                     설명
OByteArray              바01드 다우1의 바1역윽 지워하71 의云f 큭라1人 쿠 네 드의크 파익 저솟콰 갇0I 데01
                        E 스트림 구현 시 사용하면 유용함                nM7V＼       八／勺＼N\ /
OByteArrayMatcher       OByteArray로 구현된 바이트 단위의 배열의 index를 이용하1 매칭되는 문자열
                        이 있는지 찾71 위해 사용되는 클래스
QChar                   l6bit 유니코드 Chara이아를 지원하기 위한 클래스
OLatiniChar
                        US-ASCII/Latin너 인코딩 문자열을 지원하71 위하1 제공되는 클래스
oLatinlString
OLocale                 숫자 표시 방식 혹은 문자 표시 방식을 다양한 언어의 표현 방식에 맞도록 변환
                        하는 클래스입니다．
QString                 유니코드 문자열 캐릭터를 지원하는 클래스
OStrin아ist              String 리스트의 집합 클래스
OString Matcher         유니코드 스트링 문자열상에 매칭되는 문자열을 찾71 위해 제공되는 클래스
QString Ref             듸ze(), 口ositionLt, toString(）과 같은 서브 스트링 Wrap口er 클래스
QTextBoundaryFinder     스트링 문자열과 일치하는 모든 문자열을 찾71 위하1 제공되는 클래스로， 검색된
                        문자열의 NEXT/PREV 기능을 제공함
QTextStream             테스트를 쓰거나 읽어들이71 위해 제공되는 클래스로, 파일상에서 데이터를 읽거
                        나 쏠 때 사용하면 유용함




164 CHAPTER 05m 데이터 타입과 유용한 데이터 조작 클래스


===== PAGE 166 =====
          乞1.1 변수 비교／판단 함수
  Qt는 데이터 타입의 값을 판단／비교하기 위한 일반 함수와 템플릿 함수를 제공한다. 예를 들어 절대값을
 사용하기 위한 qAbs(), 최대／최소 사이의 값을 구하기 위한 qBound(), 최소값을 구하기 위한 qMin(),
 최대값을 구하기 위한 qMax( ) 함수 등을 제공한다．


  DT qAbs(const T & value)
  절대값을 사용하기 위한 함수이다．

1mnt absoluteValue;
      mnt myValue = -4;


      absoluteValue = qAbs (myValue) ;

L쓰的so加teValue 『＝ 4
1const T & qBound(const T & mm , const T & value, const T & max)
 최대／최소 사이의 값을 구하기 위한 함수이다．

      mnt myValue = 10;
      mnt minValue = 2;
      jot maxValue = 6;


      mnt boundedValue = qBound(minValue, myValue, maxValue) ;
      II boundedValue == 6



      0void qCritical(const char * msg, ...)
 Critical 메시지를 핸들링하기 위한 함수이다．
m.m＝戶／＼尸十？        m/           /\m/         m七m1小／




      void load(const QString &fiieName)
      {
             QFi1e file (fileName) ;
             if              (! file. exists () )
                              qCritical ( "File '%s ' does not exist! n, qPrintabie (fileName) );
      }

      0void qDebug(const char * msg, ...)
디버깅 메시지를 출력하기 위한 함수이다．

1ug               (   'I七.       ins   in     ii. 七： 욤d느   myLi毗．   size   () ) ;




                                                                                    ] 데이터 타입과 유용한 데이터 조작 클래스 165


===== PAGE 167 =====
evoid qFatal(const char * msg, ...)
오류 메시 지를 핸들링하기 위한 함수이다．
戶＼／小／    k/   \/\/＼小느／         小，


 mnt divide(int               a, mnt b)
 {
         if     (b == 0) /I program error
                 qFatal( "divide: cannot divide by zero '' ) ;
         return a / b;
 }


0 bool qFuzzyCompare(double p1, double p2) [static]
Floating point 값을 비교하기 위해1 사용하는 함수이다．

i II 0. 0과 비교
 qFuzzyCompare (0. 0,1.0e-200) ; II return false
 qFuzzyCompare           (1    + 0.   0,   1 + 1.   oe-
                                                          200) ;   // return   true




小bool qFuzzyCompare(float p1, float p2) [static]
float형 값을 비교하기 위해 제공되는 함수로, 값이 같으면 true, 그렇지 않으면 false를 리턴한다．

0QtMsgHandler qlnstallMsgHandler(otMsgHandier handler)
                   旽迂쓰므咬史짯多흐曳社간匙之造잣突見쏘숫"1다·
Qt에서 정의되어 있는 P.叭및쁘쁘；

 void myMessageOutput (QtMsgType type, const char *msg)
     {
         sw土ch 作ype) {
         case QtDebugMsg:
             fprintf (stderr, "Debug: %s\n", msg) ;
             break;
         case QtWarningMsg:
                 fprintf (stderr, "Warning: %s\n", msg) ;
                 break;
         case QtCri七i（그alMsg:
                 fprintf (stderr, "Critical:                   %s\n", msg) ;
                 break;
         case QtFatalMsg:
                 fprintf (stderr, "Fatal: %s\n", msg) ;
                 abort ( );
         }
     }

     mnt main(int argc, char **argv)
     {
         qlnstallMsgHandler (myMessageoutput) ;
         QApplication app(argc, argv) ;

         return app.exec ( );




166 CHAPTER 05.. 데이터 타입과 유용한 데이터 조작 클래스


===== PAGE 168 =====
孕 const T & qMax(const T & valuel, const T & va1ue2)
둘 중 八/laximum 값을 리턴하는 함수이다．

m1lt myValue = 6, yourValue = 4;

mnt maxValue = qMax (myValue, yourValue) ;
 // maxValue == myValue



簪const T & qMin(const T & valuel, const T & va1ue2)
둘 중 Minumum 값을 리턴하는 함수이다．

mnt myValue = 6, yourValue = 4;

mnt minValue = qMin(myValue, yourValue) ;
II minValue == yourValue



蜘q1nt64 qRound64(qreal value)
64b1t mnt형 반올림 함수이다．

qreal valueA = 42949672960. 3;
qreal valueB = 42949672960. 7;


mllt roundedValueA = qRound(valueA) ; /7 roundedValueA = 42949672960
m1lt roundedValueB = qRourid(valueB) ; /7 roundedValueB = 42949672961



醫mnt qRound(qreal value)
mnt형 반올림 함수이다．

qreal valueA = 2.3;
qreal valueB = 2. 7;


mnt roundedValueA = qRound(valueA) ; If roundedValueA = 2
mnt roundedValueB = qRound(valueB) ; /7 roundedvalueB = 3




 :tL2 데이터 클래스
제공하는 Basic Data type과 더불어 Qt는 어플리케이션 개발 시 , 유연한 데이터 조작을 위해 다양한 클
래스를 제공한다. 예를 들어 Bit 단위의 데이터를 다루기 위한 QBitArray, Byte 단위의 데이터를
Array 형태로 다루기 위해 QByteArray 등과 같이 데이터 조작에 편리한 클래스를 제공한다. 여기서는
데이터를 다루는데 유용한 클래스에 대해 알아보도록 하자．




                                                      ] 데이터 타입과 유용한 데이터 조작 클래스 167


===== PAGE 169 =====
 S QBitArray
 QBitArray 클래스는 Bit를 Array로 제공하는 클래스로, AND, OR, XOR 그리고 NOT 연산을 통해
Bit 연산 기능을 제공한다. 또한 Bit 데이터 복사로 인한 불필요한 메모리 낭비를 줄일 수 있고，
 QBitArray 클래스는 데이터 초기화를 위해 다음과 같이 초기화 코드를 작성할 수 있다．

 QBitArray ba(200) ;


또한 QBitArray는 Array 크기를 재조정할 수 있다．

 QBitArray ba;
 ba.resize (3) ;
 ba[ O] = true;
 ba[ l]   = false;
 ba[ 2] = true;



QBitArray는 & (AND), 1 (OR), 八 (XOR), - (NOT) 연산과 더불어 &=, 1=, 八＝ 등과 같은 연산자를 사
용할 수 있다．

 QBitArray x (5) ;
 x. setBit (3, true) ;
 // x: [ 0, 0, 0, 1, 0 1


 QEitArray y (5) ;
 y. setBit (4, true) ;
 /7 y: [ 0, 0, 0, 0, 1 ]

       y [
  X刀   卜 出   0
                 0, 0, 1, 1 1



QBitArray 클래스 Array의 특정 위치에 Null과 비어 있는（Empty) 배열 변수를 구분하기 위한 멤버함
수를 제공한다．

 QBitArray() .isNull ( );       // returns true
 QBi土Array ( ) .1毗m1此y ( ) ;    // returns true

 QBitArray (0) .isNull () ;     7/ returns false
 QBitArray ( 0) . isEmpty 0;    // returns true

 QBitArray (3) .isNull () ;     7/ returns false
 QBitArray (3) . isEmpty ( );   /7 returns false



모든 QBitArray 클래스로 선언된 Array를 false 혹은 true로 이용해 일괄 적용할 수 있는 멤버함수를
제공한다．




168 CHAPTER 05_ 데이터 타입과 유용한 데이터 조작 클래스


===== PAGE 170 =====
 QBitArray ba (8) ;
 ba. fill (true) ;
 // ba: [ 1, 1, 1, 1, 1, 1, 1, 1 1


 ba. fill (faise, 2) ;
 /7 ba: [ 0, 0 ]




G泛，:.QPainterOllk]                       .1-1F,
           ,,.,, ,,471, 7,F71,, 4*1 fl,，。1cF.
 Brush는 Style, Color, Gradient 그리고 texture를 표현할 수 있다．

 QPainter painter (this) ;


 painter. setBrush(Qt: :cyan) ;
 painter. setPen ( Qt: : darkCyan) ;
 painter.drawRect (0, 0, 100,100) ;


 painter. setBrush(Qt: :NoBrush) ;
 painter. setPen(Qt: :darkGreen) ;
 painter.drawRect (40, 40, 100, 100) ;




   （그t::S에dPattern       Qt::Densel Pattern   Qt::Dense2Pattern




   Qt::Dense3Pattern     Qt::Dense4Pattern    Qt::Dense5Pattern


 S QByteArray
 QByteArray 클래스는 문자열 데이터를 Byte 단위로 Array어］ 저장할 수 있어 유용하다. Raw 데이터
 뿐만 아니라 String 형태（마지막 '\O' 이 포함）의 Byte를 저장할 수 있다. const char과 같은 상수보다
 사용하기 쉽다. 또한 QByteArray는 동일한 메모리 영역의 문자열을 복사하는 동안 다른 프로세서가 접
 근하여 메모리 사용의 증가를 감소시켜 주기 때문에 메모리 사용이 효율적이다.

 그렇기 때문어］ 임베디드 리눅스 플랫폼에서 사용하면 메모리 효율성을 높일 수 있다. 그리고 QByte
 Array 문자열 데이터를 저장하는 QString 클래스에 저장된 문자열과 같은 non-ASCII / non-Latin-
 1 문자를 저장하기 쉽다．

 QByteArray 클래스는 생성자에 문자열을 저장할 수 있다．

 QByteArray ba ( "flello ") ;



                                                                  L데이터 타입과 유용한 데이터 조작 클래스 169


===== PAGE 171 =====
생성자를 통해 문자열을 저장하는 방법 이외에 resize( ) 함수를 사용해 QByteArray의 크기를 동적 할
당이 가능하다．

QByteArray ba;
ba.resize (5) ;
ba[ O] = 0x3c;
ba[ 1] = 0xb8;
ba[ 2] = 0x64;
ba[ 3] = 0x18;
ba[ 4] = Oxca;



그리고 Array 상어］ 특정 위치의 데이터를 읽기 위해 at( ) 함수를 사용해 접근할 수 있다．

for (mnt j = O; i < ba. size() ; ++i) {
     if   (ba.at (i) >= 'a' && ba.at (i) <= 1 f ' )
           cout << "Found character in range [a-f] " << endi;
}


QByteArray는 문자열의 '\O' 을 포함시킬 수 있다. 이 경우에 array 문자열의 전체 크기를 size( ) 함수
로 리턴하면 ' \O'은 크기어］ 포함되지 않는다．

QByteArray bal ( "ca\ Or\ Ot ") ;
bal. size() ;                              7/ Returns 2.
bal. constData() ;                         7/ Returns "ca" with terminating \O.


QByteArray ba2 ( "ca\ Or\ Ot ", 3) ;
ba2. size() ;                              7/ Returns 3.
ba2.constData() ;                          7/ Returns "ca\ O " with terminating \O.


QByteArray ba3 ( "ca\ Or\ Ot ", 4) ;
ba3. size ( );                             7/ Returns 4.
ba2.constData );                           7/ Returns "ca\ Or " with terminating \O.


const char cart[ ] = {'c ' , 'a' , '\ O ' , 'r ' , '\ O ' , 't ' };
QByteArray ba4 (QByteArray: : fromRawData(cart, 6) );
ba4. size() ;                      7/ Returns 6.
ba4.constData() ;                  7/ Returns "ca\ Or\ Ot " without terminating \O.



QByteArray는 문자열의 앞부분 또는 뒷부분에 문자 및 문자열을 추가할 수 있으며, 특정 위치의 데이티
를 교체할 수 있는 멤버함수를 제공한다．

QByteArray x ( "and") ;
x. prepend( " rock ") ;             7/ x      "rock and"
x.append ( "roll ") ;               7/ x      "rock and roll "
x.replace (5, 3, "& " );            7/ x      "rock & roll "




170 CHAPTER 05.. 데이터 타입과 유용한 데이터 조작 클래스


===== PAGE 172 =====
저장된 문자열 Array어］서 특정 문자열이 발견되는 위치를 찾기 위한 방법으로 indexOf( ) 함수를 사용
할 수 있다. indexOf( ) 함수는 처음부티 검색을 시작한다. 이와 반대로 lastlndexOf( ) 함수를 사용하
면 문자열 끝에서부터 검색을 시작한다．


QayteArray ba ( 'We must be <b>bold</b>, very <b>bold</b> ") ;
mnt j = 0;
while ( (j = ba.indexof ( "<b>",         j) ) 1= -1) {
      cout << "Found <b> tag at index position " << j << endl;
      ++j;




QByteArray는 operator<O, operator乍（), operator==(), oper毗町戶（) 등과 같은 연산자를 사용
해 문자열을 비교할 수 있다. QByteArray어］ 저장된 데이터가 Null 또는 Empty 상태인지 구분하기 위
해 isNull( ) 함수와 isEmpty( ) 함수를 이용할 수 있다．

QByteArray ( ) .isNull        );           // returns true
QByteArray ( ) . isEmpty () ;              // returns true


QByteArray ( " " ).isNull () ;             II returns false
QByteArray ( " " ) .isEmpty () ;           7/ returns true


QByteArray ( "abc " ) .isNull () ;         7/ returns false
QayteArray ( "abc " ) .isEmpty () ;        7/ returns false



문자열이 저장된 문자열의 마지막을 나타내는 ' \r'과 ' \n'을 제거하기 위해 chop( ) 함수를 사용하며 , 이
함수의 Argument인 m1lt 값은 문자열 마지막의 길이를 의미한다．


OByteArray ba ( "STARTTLS\r\ n") ;
ba.chop(2) ;            II ba == "STARTTLS "



Array어］ 저장된 문자열의 개수를 특정 문자로 대체할 수 있는 멤버함수를 제공한다. Fill( ) 멤버함수를
사용하면 Array어］ 저장된 개수만큼 Argum아此로 지정한 문자로 모두 대체된다．

 QBy七eArray ba ( "Is七an止）ul " ) ;
 ba. fill   ( 'o ' );
 II   ba == "OOOOOOOO "


 ba. fill   ( 'X ' , 2) ;
 II   ba == "XX "



QByteArray는 Base64 포맷의 데이터를 Decode 할 수 있는 기능을 제공한다. fromBase64( ) 멤버함
수를 사용하면 Decode가 가능하다．




                                                              1 데이터 타입과 유용한 데이터 조작 클래스 171


===== PAGE 173 =====
    QByteArray text = QByteArray: : fromBase64 ( n UXQgaXMgZ3JlYXQh") ;
    text. data() ;               7/ returns "Qt is great! "



Base64 기반의 encoded된 데이터를 사용하기 위한 알고리즘은 RFC2045를 사용한다. 이 외에도 Hex
로 저장된 데이터를 변환할 수 있고 URL/URI 스타일의 입력된 Encoding된 데이터를 변환할 수 있는
기능을 제공한다．

    QBy七eArray 七ext = QByteArray: :fromHex ( "517420697320677265617421") ;
    text. data() ;               7/ returns "Qt is great! "


    QEyteArray text = QEyteArray: :froinPercentEncoding( "Qt%20is%20great%33 ") ;
    text. data () ;              /7 returns "Qt is great! "



문자열이 저장된 Array에서 왼쪽부터 지정한 위치만큼 데이터를 반환할 수 있다. left( ) 함수를 지정한
크기 만큼을（mlt 값） Argume砒로 전달할 수 있다．

r
    QByteArray x ( "Pineapple") ;
    QByteArray y = x.left (4) ;
    /7 y == "Pine"



왼쪽 이외에 right( ) 함수와 mid(）를 사용해 오른쪽부터 또는 중간부터 지정한 크기만큼의 문자열 길이
를 반환할 수 있다. 그리고 leftJustified( ) 함수를 사용하면 특정 위치의 문자열 이후부터 지정한 문자
를 사용할 수 있다．

    QEyteArray x ( "apple ") ;
    QByteArray y = x.leftjustified      (8, ' . ' );
    II y == "apple. .."


QByteArray는 저장된 톄이터에서 특정 문자를 제거하거나 대체하기 위한 기능을 제공한다. replace()
함수를 사용하면 특정 위치의 문자열로 변경할 수 있고, remove( ) 멤버함수를 사용해 제거할 수 있다．

    QByteArray x ( "Say yes! ") ;
    QByteArray y ( "no") ;
    x.replace (4, 3, y) ; /7 x == "Say no! "



QByteArray는 저장된 문자열 데이터를 int, float, long과 같은 데이터 타입의 데이터를 변환하여 저
장힐 수 있는 기능을 제공한다．

    QByteArray str ( "FF") ;
    bool ok;
    mnt hex = str. tolnt (&ok, 16) ;         7/ hex    255, ok == true
    mllt dec = str. tolnt (&ok, 10) ;        7/ dec    0, ok == false




172 CHAPTER 05如 데이터 타입과 유용한 데이터 조작 클래스


===== PAGE 174 =====
    QByteArray str2 ( "FF") ;
    bool ok;
    long hex = str2. toLong (&ok, 16) ;                                   7/ hex   255, ok == true
    long dec = str2. toLong(&ok, 10) ;                                    7/ dec   0, ok == false



저장된 문자열의 알파벳이 대문자인 경우 소문자로 변경할 수 있다. 的Lower( ) 멤버함수를 사용하면 문
자열 Array에 저장된 데이터를 모두 소문자로 변경할 수 있다．

    QByteArray x ( "Qt by DIGIA") ;
    QByteArray y = x.toLower () ;
    II y == "qt by digia"
1




    小 Qc이or
QC아or 클래스는 RGB, HSV 혹은 CMYK 값 기반의 컬러를 제공하기 위한 클래스이다. 즉, RGB（빨강，
녹색 , 파랑） 구성 이외에 HSV（색조, 채도, 그리고 Value）와 CMYK를 지정할 구성요소로 사용할 수 있다．

                                                                                                                                    (0, 0, 1, 0)




     (0, L 0} )V\      \    I      ,.-"W ' (10, 0)      (120/360, 1, 1)                               (1, 0, 1, 0) r '   \＼뇨    I    ._-r '        \ (0, 1, 1, 0)


     (0, I I) \，八 //        1     \＼뇨        i) 1山，1)   (t0야360, 1                 (300/360, 1, 1)    (1, 0. 0, 0) \八 //        I    \\        J (0, l, 0, 0)




                                 (0, 0. I)

                           ROB                                              HSV                                                CMYK


QColor는 기본으로 RGB 값을 사용한다. HSV 또는 CMYK를 사용하기 위해 toHsv( ) 함수와
的Cmyk( ) 함수를 이용해 변환할 수 있는 기능을 제공한다．

r7/ Specify semi-transparent red
    painter. setBrush(QColor (255, 0, 0, 127) );
    painter.drawRect (0, 0, width( )/2, height (fl;


    /7 Specify semi-transparent blue
    painter. setBrush(QColor (0, 0, 255, 127) );
    painter.drawRect (0, 0, width() , height () /2) ;



    S QCursor
QCursor 클래스는 마우스 커서를 임의의 모양으로 지정할 수 있는 기능을 제공한다. 이 클래스는 주로
특정 위젯상에 마우스 커서를 생성하고 마우스 커서의 위치를 설정하는 데 사용한다. 표준 마우스 커서
모양 이외에 QBitmap, 八flask, I如tspot을 기반으로 사용자 정의 커서 모양을 만들 수 있는 기능을 제공
한다．




                                                                                                     ] 데이터 타입과 유용한 데이터 조작 클래스 173


===== PAGE 175 =====
II Specify semi-transparent red
painter. setBrush(QColor (255, 0, 0, 127) );
painter.drawRect (0, 0, width( )I2, height ( ));


II Specify semi-transparent blue
painter. setBrush(QColor (0, 0, 255, 127) );
painter.drawRect (0, 0, width() , height ( )I2) ;



Shape Qt::CursorShape Value                  Cursor Name        Shape Qt::CursorShape Value Cursor Name

       臣Qt:                 :ArrowCursor     let t_ptr
                                                                 l                Qt::SizeVerCursor     이ze ver


       I              Qt::UpArrowCursor      up_arrow
                                                                卜+                Qt::SizeHorCursor     size hor




                                                                  / \ 小 + 小 抑 功
 -{-                  Qt:   :CrossCursor     cross                                Qt::SizeBDiagCursor   이ze_bdiag

                      （그r사BeamCursor         仕兀am                                 Qt::SizeFDiagCursor   size_fdiag

                      아：:W帥Cursor            wait                                 0仁SizeAliCursor       引ze all

                      Qt::BusyCursor         Iett_ptr_watch                       （값：:S이itVCursor       5이it \/




              0 枷
                니 胛
                                                                                  O   QU
                                                                                           C
                                                                                           m   r
                                                                                               0
                                                                                               r
                      Qt::ForbiddenCursor    幻rbidden                                          U
                                                                                               八뇨U
                                                                                                        S이仕小

                      Qt::PointingHandCursor pointing_hand                        Ot::OpenHandCursor    openhand

                      Qt::WhatslhisCursor    whats this                           （거：:ClosedHandCurs（가 이osedhand

                      Qt::DragMoveCursor     dnd-move or move                     Qt::DragCopyCursor    dnd-copy or copy

                      Qt::DragLinkCursor     dnd-link or link



I QDate
이 클래스는 날짜와 날짜를 비교하는 기능을 제공한다. 년, 월, 일 등과 같이 시스템 이ock을 이용해 현
재 날짜를 읽을 수 있다. QDate는 currentDate( ) 함수를 이용해 현재 날짜를 읽을 수 있다. 그리고
fromString( ) 함수를 이용해 문자어꺼 날짜를 해석할 수 있다．

또한 yearO, month( ) 그리고 day( ) 함수를 통해 각 년, 월, 일을 읽을 수 있다. 그리고 날짜어］ 대한 요
약된 이름과 완벽한 날짜 이름을 알파벳으로 읽을 수 있다. 그리고 m1lt형에 숫자를 더하는 것과 같이 해
당 날짜어］ 년, 월, 일을 addYears( ), addMoi此k( ) 그리고 addDays( ) 함수를 사용해 해당 날짜에
Argument 값을 더할 수 있는 기능을 제공한다．

QDate dl (1995, 5, 17) ;                    II May 17, 1995
QDate d2 (1995, 5, 20) ;                    II May 20, 1995
dl. daysTo (d2) ;                           7/ returns 3
d2. daysTo (dl) ;                           /7 returns -3




174 CHAPTER 05_ 데이터 타입과 유용한 데이터 조작 클래스


===== PAGE 176 =====
QDate는 Strii乷의 특정 패턴 방식 표현으로 날짜의 자릿수에 맞게 표시할 수 있는 기능을 제공한다. 예
를 들어 1-31일까지 표시하는데 있어 10일 이하인 경우 앞에 0을 사용하는 것과 같이 Day를 두 자리로
표시할 수 있다．

    표현               설명
    d                앞에 0이 붙지 않는 숫자로 표시 (1N31)
    dd               앞에 0이 붙는 숫자로 표시 (01N31)
    ddd              3자리의 요약으로 요일 표시 （예 "Mon' to 'Sun'). OD計e::shortDayName().
    dddd             요일 이름을 모두 표시 （예 ‘卜加nday' to sunday' ). QDate::IongDayNameO.
    M                앞에 001 붙지 않는 숫자로 표시 (1'31)
    MM               앞에 0이 붙는 숫자로 표시 (01N31)
    MM卜A             월을 3자리의 요약으로 요일 표시 (011 'Jan' N 'Dec' ). Uses QD計아shorth加nthNam& ).
    MMMM             월 이름을 모두 표시 （예 'January' N 'December' ). Uses QDa博：幻ngMon卄Name().

    yy               년을 두 자리 숫자로 표시 (00N99)

    yyyy             년을 4자리 숫자로 표시



QDate 클래스는 모든 입력 문자를 텍스트로 표시한다. 그렇기 때문어］ 날짜를 표시하는 패턴의 문자는
따옴표로 묶어서 입력해야 한다．


    QDate dl = QDate: :fromString( '02. 25 ' ,     "MM. dd" ) ;
    QDate d2 = QDate: :fromString( "2013. 02. 25 ",      "yyyy.MM. dd") ;
    /7 Sun Feb 25 1900
    7/ Sun Feb 25 2013



QDate는 현재 날짜를 얻어오기 위한 멤버함수를 제공한다. currentDate( ) 함수를 이용해 현재 날짜를
얻어올 수 있다．

    QDate dl = QDate: :currentDate() ;
    QLabel *labell = new QLabel(dl. toString(fl;


현재 날짜의 요일을 얻어오기 위해 해당 요일의 Enum 타입의 숫자를 리턴하는 기능을 제공한다．

    QDate dl = QDate: :currentDate () ;


    //enum: 월（1) , 화（2) , 수（3) , 목（4) , 금（5) , 토（6) , 일（7)
t
           day
                 =   dl.   dayOfweek   ( );


Year를 기준으로 현재 날짜에서 며칠이 지났는지 얻어오는 기능을 제공한다. dayOfYear( ) 함수를 이
용하면 해당 년에서 며칠이 경과했는지 얻어올 수 있다．

    QDate dl = QDate: :currentDate () ;
    m1lt day = dl. dayOfYear ( );




                                                                   l 데이터 타입과 유용한 데이터 조작 클래스 175


===== PAGE 177 =====
또한 dayOfYear( ) 함수와 같이 해당 월에서 며칠째 인지 얻어오는 기능을 제공한다. dayslnM아此ho )
함수를 이용하면 며칠이 경과하였는지 알 수 있는 멤버함수를 제공한다．

 ODate dl = QDate: : currentDate( ) ;
 mnt day = dl. days工nNonthQ;



현재 날짜와 설정한 날짜로부터 해당 년에서 며칠이 남았는지 알 수 있다. dayslnYear( ) 함수를 이용하
면 그 해의 넌이 며칠인지 얻어올 수 있다. （범위 365- -366) 날짜를 표기하는 방식은 디폴트로 Qt의 기본
적인 타입으로 표기하는 것과 ISO8601 방식으로 표기 또는 운영체제의 설정된 지역의 포맷으로 날짜를
표현하는 방식으로 표기 방법을 선택할 수 있다．

상수               값      설명
Qt::TextDate            아의 기본적인 디폴트 타입
Qt::ISODate             IS0860] 표준에 정의된 방식으로 날짜를 표현
Qt::LocalDate           0s가 설정된 지역의 포맷0로 날짜를 표현



S ODateTime
QDate 클래스는 날짜를 표시하기 위한 클래스라면 QDateTime 클래스는 날짜와 시간을 함께 처리할
수 있는 기능을 제공한다. QDate 클래스와 동작하는 방식은 거의 동일하다. 예를 들어 시간을 문자 포맷
으로 표시할 때 0을 앞에 사용할 경우 'h', 그렇지 않은 경우 'hh' 를 포맷으로 사용할 수 있다．

표현              출력
h               小23, 만약 AM/PM의 경우卜］2
hh              00'-'23, 만약 AM/PM의 경우 0N]2
H               0N23시로 표시
HH              OO"23시로 표시
m               분을 O"59로 표시
mm              분을 표시, 앞에 '0'을 사용하는 방식으로 00-"59로 표시
S               초를 小59로 표시
ss              초를 표시， 앞에 '0'을 사용하는 방식으로 00N59로 표시
z               MiHisecond를 표시, 앞에 '0'을 사용하지 않는 방식（0'999)
zzz             Millisecond를 표시, 앞에 '0'을 사용하는 방식（000八J999)
AP or A         AP/PM으로 표시
ap or a         am巾m으로 표시




176 CHAPTER 05... 데이터 타입과 유용한 데이터 조작 클래스


===== PAGE 178 =====
fromString( ) 함수는 문자를 표시하기 위한 방식으로 따옴표를 사용해야 한다. 그렇지 않으면 삽입한
문자가 그대로 출력된다．

    QTime timel = QTime: :fromString( "131",                                "HHh") ;
    7/ timel is 13: 00: 00
    QTime timel = QTime: :fromString ( "lapA",                                "larnA卜1") ;
    7/ timel is 01: 00: 00


    QDateTime dateTime2 = QDateTime: :fromString( "M1d1y9800 :01: 02 ",
                                                                                   ' 'M'M'd 'd 'y 'yyhh:mm: ss ' ) ;
    7/ dateTirne is 1 January 1998 00: 01: 02



露 QEasingCurve
QEasingCurve 클래스는 애니메이션 프레임워크에서 움직임에 대해 Alpha 값을 적용해 다양한 Effect
효과를 표시할 수 있다. 즉, 움직이는 오브젝트가 목적지까지 이동하는데 있어 선형 (Linear) 방식으로 이
동하는 것이 아니라, 목적지까지 이동하는데 시간과 속도를 특정 패턴에 따라 다양하게 변화시킬 수
있다．

예를 들어 1.0초의 소요시간을 설정하고 팝업의 크기를 커지게 하는 경우 0.5초까지 빠르게 커지고, 나머
지 0.5초 동안은 서서히 커지는 것과 같은 Effect를 정의한 것이 QEasingCurve이다．

    value                             (1 1)
                                       .      value
                                                                  (1, 1)   value                    value




                       progress                                 progress               progress                 progress

                  Linear                              InQuad                       OutQuad                  OutinQuart


Qt 애니메이션에 효과를 지정하기 위해 40가지의 지정된 방식을 제공한다. 또한 사용자가 Effect를 추
가할 수 있는 Custom 타입을 제공한다．



f   animati：per      三므： :::：忿
                           :::::：믄：                      " '"

ianim“七ion. a"쁘“dv卵叩，000.);
년nimation ' set브asingUurve（닙브as ingLurve: :inout닙ua（그j "


    心 QFont
QFont 객체는 글꼴어］ 대한 속성을 지정하는 기능을 제공한다. 글자의 크기 , 색상, B아d, 밑줄 기능, 기
울기 등 폰트가 가지는 특성을 사용할 수 있다．

    QFont serifFont ( "Times ", 10, QFont: :Bold) ;                                                                        艸1
    QFont sansFont ( "Helvetica [Cronyx] ", 12) ;
                                                                                                                                J

                                                                                              j 데이터 타입과 유용한 데이터 조작 클래스 177


===== PAGE 179 =====
       小（긔con
 Qlcon 클래스는 툴 메뉴상에서 아이콘을 사용하거나 버튼에 아이콘을 추가하기 위한 기능을 제공한다．
가장 간단한 방법은 QPixmap을 사용해 아이콘을 표시할 수 있다．

fQT。
   。iBu七七on *bu七七on = new QToo1Bu七七On;
}button-            >setlcon (Qlcon   (   "open.        xpm   "   ) );


  Qlcon은 QToolButton 클래스에서 사용할 때 아이콘이 표시되는 상태에 따라 표시하는 아이콘을 다르
   게 표시할 수 있다. 예를 들어 Normal인 상태, 버튼이 선택되었을 때 , on/off 상태에서 아이콘을 다르
   게 표시하는 것이 가능하다．

           void MyWidget: :drawlcon(QPainter *painter, QPoint pos)
            {
                QPi刃nap pixmap = icon.pixmap(QSize (22, 22) ,
                                                                     isEnabled() ? Qlcon: :Normal : Qlcon: :Disabied,
                                                                     isChecked() ? Qlcon: :On : Qlcon: :Off) ;
                painter->drawPixmap(pos, pixmap) ;




   Qlcon은 Enum 타입으로 아이콘 모드를 다음과 같이 지정할 수 있다．

           상수                 값                    설명
       （긔con::N아mal                                사용자가 아이콘을 표시하는 Normal 한 상태의 기본 모드
       （긔c0n::［기sabled        1                    기능상 미sab旭 모드
           （긔cc가l::Active     2                    사용자에 의해 활성화된 모드
       （긔con::Selected        3                    아이콘이 체크된 모드



 또한 Qlcon 클래스는 아이콘의 On과 Off 상태에 따라 Pixmap 상태를 변경할 수 있는 State를 제공한다．

           상수                 값                    설명
      （긔con::Off              0                    다xmap이 위젯상에서 off 상Ej]
      （긔con::On                                    Pixmap이 위젯상에서 on 상태


           好（긔mage
Qlmage 클래스는 이미지와 같은 픽셀 데이터를 액세스 할 수 있고, 하드웨어와 독립적으로 이미지를 표
현하는 기능을 제공한다. Qlmage 클래스와 같은 기능을 제공하는 클래스로 Qt는 QPixmap,
QBitmap, QPicture 클래스를 사용할 수 있다．

이 녜 가지 중 QPixmap 클래스는 이미지를 조작해 표시하는 경우 최적화 되어 있고, Qlmage 클래스는
직접 픽셀을 조작할 수 있으며 I/O와 연결하여 사용하므로 성능어］ 최적화 되어 있다．

Qlmage는 QPaintDevice 클래스의 하위 클래스이다. QPainter 상에서 Qlmage를 사용할 경우 GUI
의 다른 Thread에서 수행된다. Qlmage는 enum 타입으로 여러 가지 이미지 형식을 지원한다. 예를 들


178 CHAPTER 05_ 데이터 타입과 유용한 데이터 조작 클래스


===== PAGE 180 =====
  어 흑백, 8비트, 32비트 및 알파가 혼합된 이미지를 포함해 사용할 수 있다. Qlmage는 다음과 같은 포
맷을 지원한다．

          포맷                   설명                                                 지원
          BMP                  윈도우 Bitma口                                         Read/write
          （引F                  （計aphic Interchange 포맷 (or川anal)                   Read
          JPG                  J이nt Photogra口hic Experts Grou口                    Read!＼사rite
          JPEG                 Joint Photographic Experts Group                   Read/write
          PNG                  Portab冶 Network G田아iics                            Read!＼사rite
          PBM                  Portable Bitmap                                    Read
          PGM                  Portable Graymap                                   Read
          마가너                  Portable Pixmap                                    Read/write
          XBM                  Xli Bitmap                                         Read/write
          XPM                  xii 거xma口                                          Read/write


이미지 픽셀은 조작하는 형식에 따라 달라진다. 그 이유는 32비트 이미지를 직접 ARGB 값을 저장하는
동안 인덱스 기반의 乎bit 이미지와 흑백 색상 Lookup Table 기반이기 때문이다. 32-bit 이미지의 경
우에는 setPixel( ）을 이용해 ARGB를 조작할 수 있다. 그리고 QRgb 값을 만들려면 qRgb( ) 함수를 사
용할 수 있다．




                                                                                                                                  ;
                                    (3,                                                                                           1

                                                                                                   P尸［戶
                                                                                                     1 [1
          Qlmage       image
                                          3,
                                                    Qlmage:
                                                              :FormatRGB32)   ;
          QRgb value;

          value = qRgb(189, 149, 39) ; /1 0xffbd9527
          image. setPixel (l,  value) ;        1,
                                                                                                             H




                                                                                                    0xfl7aa327   0xffedba 1
!value    qRgb(122, 163, 39) ; // 0xff7aa327
                   =




                                                                                                   1 P尸P尸
iimage. setPixel (O,   value) ;                1,
1image. setPixel(l, 0, value) ;
1
  value = qRgb (237, 187, 51) ; // 0xffedba31
                                                                                                             .
!iinage. setPixel(2, 1, value) ;
                                                                                                                              1
      S OKeySequence
QKeySequence 클래스는 메뉴의 단축키를 지정해 빠른 실행을 위한 사용자 인터페이스를 제공하기 위한
 기능이다. 가장 일반적으로 사용하는 Key는 ［區끄 과 알파벳을 조합한 형태로 단축키를 지정할 수 있다．

          QKeySequence ( QKeySequence: : Print) ;
          QKeySequence (tr ( "Ctrl+P") );
          QKeySequence(tr ( "Ctrl+p") );
          QKeySequence(Qt: :CTRL + Qt: :Key_P) ;




                                                                                                ] 데이터 타입과 유용한 데이터 조작 클래스 179


===== PAGE 181 =====
1QMargins
QMargins 클래스는 사각형 4개 영역의 Margin 값을 지정하기 위해1 제공되는 기능이다. 즉 Left, Top,
Right 그리고 Bot的m을 설정할 수 있다．

Margin 값 설정은 setLeft( ), setRight( ), setTop( ) 그리고 setBottom 함수를 이용해 설정할 수 있
다. 만약 八4argin 값이 0인지 확인하기 위한 방법으로 isNull( ）로 확인할 수 있다. 0인 경우 isNull( )
함수는 true를 리턴한다．


1QMatrix 클래스와 QMatrix 4x4 클래스
QMatr奴 클래스는 2D의 오브젝트에 확대 및 축소와 같은 Scale, 회전 혹은 이동을 조작할 수 있는 기능
을 제공한다, 또한 3차원 공간에 缸4 Matr奴를 표현하기 위한 클래스로 QMatrix 缸4 클래스를 제공
한다．

void SimpleTransformation: :paintEvent (QPaintEvent *)
 {
      QPainter painter (this) ;
      painter. setPen (QPen(Qt: :blue, 1, Qt: :DashLine) );
      painter. drawRect (0, 0, 100, 100) ;                                   戈乞
      pain七er . ro七ate ( 45 ) ;


      painter. setFont (QFont ( "Helvetica", 24) );
      painter. setPen(QPen(Qt: :black, 1) );
      painter. drawText (20, 10, "QMatrix ") ;
 }


eop톄ette
QPalette 클래스는 각 위젯의 상태를 위한 색상 그룹을 포함하는 클래스이다. 하나의 Palette는 3가지
의 컬러 그룹을 가지고 있다. Active, Disabled 그리고 Inactive이다. Palette를 포함하는 모든 위젯은
스스로 위젯을 Drawing하기 위해 사용한다．

활성화 그룹은 키보드 포커스가 있는 창어］ 사용하고 비활성화 그룹은 다른 창에 사용된다. 그리고
Disabled 그룹은 비 활성화된 위젯에서 사용된다．


0OPen
QPen 클래스는 라인과 도헝의 윤곽선을 그리는데 사용한다. QPen은 속성으로 스타일, 선의 넓이, 브러
쉬, CapStyle 그리고 Joir侶tyle을 사용할 수 있다．

QPainter painter (this) ;
QPen pen(Qt: :green, 3, Qt: :DashDotLine, Qt: :RoundCap, Qt: :RoundJoin) ;
pain七er. se七Pen (pen) ;




180 CHAPTER 05_ 데이터 타입과 유용한 데이터 조작 클래스


===== PAGE 182 =====
Pen 스타일로 지정되어 있는 Enum 타입으로 6가지의 타입을 지정할 수 있다．

                               /
                           ,                                       d毛



                                                                  弔




      Qt::S이1미Jne                  Qt::DashLine                            Qt::D이니ne



 如




                           :   小     \L
                                          (   蜘    ,   ,   /                   너也




     Qt::DashDotLine           Qt::DashD아D아니ne                          Qt::CustomDashLine


Cap Style은 QPair此er를 사용하여 라인을 그릴 때 라인의 마지막 부분을 어떤 스타일을 사용할지 결정
하기 위한 방식이다．




Qt::SquaneCap              Qt::FlatCap                         Qt::RoundCap


Join Style은 QPair此er를 사용해 라인이 만나는 부분과 모서리 부분은 enum 타입을 이용해 다음과 같
은 스타일을 지정할 수 있다．




 （값::BevelJoin             Qt::卜川terJ이n                        Qt::RoundJoin


00 Picture
QPicture 클래스 플랫폼의 독립적인 IO 장치를 사용하여 직렬화 형태도 사용한다. 이미지는 바이너리
방식의 포맷이며 Qt에서 이미지와 위젯상어］ 사용할 수 있다．

QPainter painter;
painter.begin(&picture) ;                         II paint in picture
painter.drawEllipse(10, 20, 80, 70) ;             7/ draw an ellipse
painter.end() ;                                   II painting done
picture .save ( '1 drawing.pic1' ) ;              // save picture




                                                                        ] 데이터 타입과 유용한 데이터 조작 클래스 181


===== PAGE 183 =====
QPicture 클래스는 QPainter어］ 의해 Drawing한 데이터를 파일에 저장하고 로딩하기 위해 save( ) 함
수와 load( ) 함수를 사용할 수 있다．

    QPicture picture;
    pic七l그re. load( " dras寸ing.pic " ) ;                     II load picture
    QPainter painter;
    painter, begin ( &mylmage) ;                            /7 paint in mylmage
    painter. drawPicture (0, 0, picture) ;                  7/ draw the picture at (0, 0)
    painter. end() ;                                        // pain七ing d（그ne




    0QPixmap
QPixmap 클래스는 페인트 디바이스를 사용할 수 있는 Off-screen 이미지로 처리할 수 있다. 예를 들
어 QPainter에 의해I Drawing된 요소를 I기xmap에 바로 그릴 수 있으며 화면에 보이지 않는 영역을 포
함하여 이미지를 표시할 수 있다．




                     Igno冶Aspec杆크at幻          KeepAs아兀們atio Kee口A히）ec卄극atioByExpanding


    S OP이nt
QPoint 클래스는 정수 정밀도를 사용하여 좌표 지점을 표시하기 위해 사용되는 기능을 제공한다. x와 Y
모두 0인 경우 isNull( ) 함수는 true를 반환한다. 좌표 설정을 위한 함수는 setX( ) 함수와 setY( ) 함수
를 사용한다．

    QPoint p;


    p. setX (p.x () + 1) ;
    p += QPoint (l, 0) ;
    p.rx ( )++;



QPointer는 operator를 통해 연산이 가능하다．

    QPoint p ( 3, 7) ;
1         七q
               (-   l,     4) ;
1
          q;             /7 p becomes   (2,
                                               11)
小 OQu計err기on
QQuaternion 클래스는 백터 및 스칼라로 구성된 Quaternion을 나타낸다. Quaternion은 3D 공간어］
서 x,Y 그리고 z 좌표와 회전과 같은 각도를 3D에 사용되는 기능을 제공한다．

    宓旭C七自茗3D resu此 = (q 出 QQua七ernion(O, vector) 士 q. con jug社e ( )}.v以比or ( );



182 CHAPTER 05_ 데이터 타입과 유용한 데이터 조작 클래스


===== PAGE 184 =====
S QRect
QRect 클래스는 정수(Integer）를 사용해 사각형을 정의하기 위해 사용된다. 사각형의 x, y 좌표 그리고
Width, Height의 좌표 정보를 나타내는데 사용한다．

QRect rl (100, 200, 11, 16) ;
QRect r2 (QPoint (100, 200) , QSize(11, 16) );



S QRegExp2F ORegularExpression
QRegExp 클래스는 정규식 표현을 이용해 패턴 매칭 기능을 제공한다. 정규식 표현 방식은 수많은 문자
열 혹은 특정 문자열에서 패턴을 적용해 매칭되는 단어를 찾을 수 있다. 예를 들어 문자열에서 'ABCD'
가 반복되는 문자열을 찾고자 하는 경우 유용하다. 문자열에서 0 N 99 사이의 숫자가 포함되는 것을 확
인하기 위해 다음과 같이 QRegExp 클래스를 활용할 수 있다．

QReg助叩 rX ( n 八＼\d\\d? $,, ) ;     If match integers 0 to 99
rx. indexln( " 123 ") ;            If returns -1 (no match)
rx. indexln( "- 6 ") ;             // returns -1 (no match)
rx. indexln( "6 ") ;               II returns 0 (matched as position 0)



S QRegion
QRegion 클래스는 Painter 영역에서 특정 영역 중 일부를 클립보드 영역으로 정의하기 위해 사용된다．
QRegion은 QPainter: :setClipRegion( ) 함수와 함께 사용한다. Painter 상에서 사각형 내부의 특정
영 역을 사각형으로 클립보드로 사용하기 위해 다음과 같이 사용할 수 있다．

void Mywidget: :paintEvent (QPaintEvent *)
{
     QRegion rl (QRect (100, 100, 200, 80) ,     II rl:   elliptic   region
                   QRegion: :Ellipse) ;
     QRegion r2 (QRect (100, 120, 90, 30) );     II r2: rectangular region
     QRegion r3 = rl. intersected(r2) ;           // r3: intersection


     QPainter painter (this) ;
     painter. setClipRegion ( r3) ;
                                                  /7 paint clipped graphics
}


S QSize
QSize 클래스는 mllt 값을 이용해 width(int), height(int）을 정의하기 위해 사용되는 클래스이다．
width와 height 값을 설정하기 위해 setWidth( ）와 setHeight( ) 함수를 사용하며 width와 height를
참조하기 위해 width( ）와 height( ) 함수를 사용할 수 있다．

QSize size (loo, 10) ;
size.rwidth( ) += 20;
7/ size becomes (120,10)



                                                            ] 데이터 타입과 유용한 데이터 조작 클래스 183


===== PAGE 185 =====
QSize 클래스는 Qt: : AspectRationMode와 같이 width와 height 값에 sacle을 적용할 수 있는 기능을
제공한다．

           QSize tl (10, 12) ;
           tl. scale(60, 60, Qt: :IgnoreAspectRatio) ; II tl         is (60, 60)


           QSize t2 (10, 12) ;
           t2. scale (60, 60, Qt: :KeepAspectRatio) ; 7/ t2 is (50, 60)


           QSize t3 (10, 12) ;
           t3. scale(60, 60, Qt: :KeepAspectRatioByExpanding) ; 7/ t3 is (60, 72)




1QString
QStrii培은 16-bit Q（그har의 문자열을 저장할 수 있다. QChar은 Unicode 4.0 character와 일치한다．
Unicode는 컴퓨터에서 가장 많이 사용하는 국제 표준 포맷 중 하나이다. QStrii乷은 사용자 편의를 위
해 쉽게 사용할 수 있고, 초기화하는 방법으로 다음과 같이 사용할 수 있다．

1OString
                         str   =   "Hello            "   ;



  QStrii培은 const char와 같은 상수를 fromUtf8( ) 함수를 사용해1 대체할 수 있다．

           static Oonst QChar data[ 4] = { 0x0055, 0x006e, 0x10e3, 0x03a3 };
           QString str (data, 4) ;



    QStrii培의 array의 특정 위치어］ QChar을 저장할 수 있다．

  QString str;
三 S七r. resize ( 4) ;


 ,
           str[ 0]   =    QChar (     'U    '   );
   QStrii培은 if문을 이용해 다음과 같이 문자열 비교가 가능하다．

           QString str;

           if   (S七r == 'au七0"         L S七r == " e）代emn"
                         L     S七r == "S七atic " 1 1 5七r == "regis七er ' ) {
                II




 184 CHAPTER 05_ 데이터 타입과 유용한 데이터 조작 클래스


===== PAGE 186 =====
QString어］ 저장된 문자열을 조작하기 위한 방법으로 추가하는 기능은 append( ) 함수를 사용할 수 있
다. 그리고 QString의 앞쪽어］ 문자를 추가하는 방식으로 prepend( ) 함수를 사용할 수 있으며，
replace( ) 함수를 이용해 특정 위치의 문자 및 문자열을 변경할 수 있다. 또한 특정 위치의 문자열을 제
거하기 위해 remove( ) 함수를 이용할 수 있다．

QString str = "and";
str. prepend ( "rock ' ) ;    // str     "rock and"
str. append( " roll ") ;      // str     "rock and roll "
str. replace (5, 3, "& " );   II str     "rock & roll "



만약 찾고자 하는 특정 문자열의 위치를 알고 싶다면 indexOf( ) 함수를 사용해 찾고자 하는 문자열의 위
치를 찾을 수 있다．


QString str = "We must be <b>bold</b>, very <b>bold</b>";
mnt j = 0;


while ( (j = str. indexOf ( '1<b>",
                                 j) ) != -1) {
     qDebug( ) << "Found <b> tag  at index position"        <<   그;
     ++j;




0OTime
QTime 클래스는 시 , 분, 초, 그리고 millisecond를 포함하는 Clock Time을 제공한다. 그리고 시간을
표기하는 다양한 방법을 제공한다. AM/PM과 같은 방식으로 시간을 표시할 수 있으며, 현재 시간을
currentTime( ) 함수를 이용해 얻어올 수 있다．

QTime n(14, 0, 0) ;                    II n == 14: 00: 00
QTime t;
t = n.addSecs (70) ;                   // t == 14: 01: 10
t = n.addSecs (- 70) ;                 /7 t == 13: 58: 50
t = n.addSecs (10 * 60 * 60 + 5) ;     I! t == 00: 00: 05
七 = n.addSecs (- 15 出 60 士 60) ;       II t == 23: 00: 00


hourO, minuteO, second(), 그리고 msec( ) 함수를 이용해 각 시간에 대한 정보를 얻어올 수 있으며
문자열 포맷으로 변환하여 얻어오기 위에 切String(）을 이용할 수 있다. 문자열로 변환하기 위한 방법으
로 다음과 같은 포맷을 사용할 수 있다．




                                                             j 데이터 타입과 유용한 데이터 조작 클래스 185


===== PAGE 187 =====
표현            설명
h              0 N 23, 만약 AM/PM의 경우 ] N 12
hh             00 八J23, 만약 AM/PM의 경우 0 N 12
m              분을 0 八／ 59로 표시
mm             분을 표시, 앞에 '0'을 사용하는 방식으로 00 "' 59로 표시
S              초를 0 N 59로 표시
ss             초를 표시， 앞에 ' 0'을 사용하는 방식으로 00 N 59로 표시
z             卜川Ilisecond를 표시， 앞에 可을 사용하지 않는 방식 (0 " 999)
zzz            M베second를 표시， 앞에 '0을 사용하는 방식 (000 "-' 999)
AP             대문자 'AM', 'PM’으로 표시
a口             소문자 'am', 'pm’으로 표시


S QTrans幻rm
QTransform 클래스는 2D 환경에서 이동, 확대／축소, 회전과 같은 속성을 정의하는데 사용되는 클래스
이다．

void SimpleTransforniation: : paintEvent (QPaintEvent *)
 {
       QPainter pain七er作hi引 ;
       painter. setPen(QPen(Qt: :blue, 1, Qt: :DashLine) );
       painter. drawRect (0, 0, 100, 100) ;


       painter. rotate (45) ;


       painter. setFont (QFont ( "Helvetica", 24) );
       painter. setPen(QPen(Qt: :black, 1) );
       painter. drawText (20, 10, "QTransforrn") ;
 }


S QUrI
QUrl 클래스는 URL을 사용하는 인터페이스에서 편리하게 사용할 수 있다. 인코딩된 주소와 그렇지 않
은 URL을 처리하고 조작하기 위한 다양한 기능을 제공한다．

QUrl url ( "http: I/ www. exarnple.com/List of holidays. xml ") ;
II    url. toEncoded( ) == "http: //www. example.com/List%200f%20h011days. xml "



Encodi1培된 문자열로부터 URL을 구성하기 위해 fromEncoded( ) 함수를 사용할 수 있다．

QUrl unl = QUrl: :froiriEncoded( " http: //qt. nokia.com/List%200f%20h011days. xml ") ;




186 CHAPTER 05_ 데이터 타입과 유용한 데이터 조작 클래스


===== PAGE 188 =====
I QVariant
QVariant 클래스는 일반적으로 사용되는 Qt 데이터 타입들을 union과 같은 기능을 제공한다．

QDataStream out (. ..);
QVariant v (123) ;                 // The variant now contains an mllt
mnt x = v.tolnt () ;               /7 x = 123
out << v;                          7/ Writes a type tag and an mnt to out
v = QVariant ( "hello11 ) ;        /7 The variant now contains a QByteArray
V = QVariant (tr ( "hello") );     7/ The variant now contains a QString
in七 y = V. tom1l七（ ) ;             // y = 0 since v cannot be converted to an mnt
QString s = v.toString() ;         7/ s = tr ( "hello '1 ) (see Q0bject: :tr ( ))
out << v;                          7/ Writes a type tag and a QString to out

QDataStream in (. . .);            7/ (opening the previously written stream)
in >> v;                           /7 Reads an mnt variant
mnt z = v.tolnt () ;               /7 z = 123
qDebug( " Tyf氾 is 둠5 "             7/ prints "Type is mnt '
        v. typeNanle ( ));
V = v.tolnt () + 100;              7/ The variant now hold the value 223
v = QVariant (QStringList ( ) );



I QVector2D, QVector3D 그리고 QVector4D
QVec的r2D는 2D 공간에서 Vect아와 Vertex를 표시하기 위해 사용되는 클래스이다. QVec的r3D는
x, y에 z가 추가된 클래스이다. 그리고 QVector4D 클래스는 w가 추가된 기능을 제공한다．



伉仁 由曲er 클래스
Qt 라이브러리는 범용 템플릿 기반 클래스들을 제공한다. Container 클래스는 특정 유형의 데이터 항목
들을 저장하는데 사용할 수 있다. 예를 들어 QStrir培으로 저장해야 할 항목이 여러 개 있다면 QVector
<QString泣｝같은 배열인 경우 Container 클래스를 이용하면 유용하다．

Qt에서 제공하는 Container 클래스들은 STL에서 제공하는 Container들보다 사용하기 쉽고 안전하다．
또한 경량화 되어 있다. 그러므로 Qt에서 제공하는 Container는 STL에서 제공하는 Container를 대체
해 사용할 수 있다．




                                                        ] 데이터 타입과 유용한 데0떠 조작 클래스 187


===== PAGE 189 =====
     S Cont테ner 클래스

         타입                            설명
         QHash(Key, T)                 Hash 테이블 기반의 ［기ctionary를 제공하기 위한 템플릿 클래스
         QMap(Key, T)                  Binary Search tree 기반 ［기ctionary룔 제공하기 위한 템플릿 클래스
         QPair(T1, T2)                 쌍으로 존재하는 아이템 데이터를 처리하기 위한 템플릿 클래스
         QList(T)                      니St 형태의 값을 다루71 위해 제공하는 템플릿 클래스
    （가JnkedL巴tT>                       링크 리스트를 제공하기 위한 템플릿 클래스
         QVector(T)                    동적인 0 Vector 배열을 다루기 위하1 제공되는 클래스
         QStack(T)                     push( ), pop( ), top( ）을 이용한 Stack을 사용하71 위해 제공되는 클래스
         QQueue(T)                     enqueue( ), dequeue( ) 그리고 head( ）를 이용하1 디FO 구조의 데이터 조작을 위해 제공되는
                                       클래스
         QSetKT)                       해시 기반의 빠른 검색을 위해 제공되는 클래스
         QMap(Key, T)                  Key 값에 의해 Mapping 되는 데이터를 하나의 조합으로 연결되어 ［기ctionary를 제공하고，
                                       QMap 클래스는 키 순서로 데이터를 저장할 수 있다．
         QMultiMap(Key, T)             OMap으로부터 상속받은 클래스이다. 다중 Ma口ping 값을 이용할 수 있다．
         QMultiHash(Key, T)            OHash로부터 상속받은 클래스이다. 다중 Ma口口ir四 값을 이용해 해시를 사용할 수 있다．



         0QHash(Key, T)
 QHash 클래스는 해시 테이블 기반의 Dicti아追ry를 제공한다. 데이터를 저장하는 방식은 Key, V키ue
가 Pair（쌍）로 저장 된다. Key로 찾고자 하는 데이터를 매우 빠르게 검색할 수 있는 기능을 제공한다．
 QHash는 帥flap과 매우 비슷한 기능을 제공하지만 내부 알고리즘은 帥flap어］ 비해 상당히 빠르게 검색
할 수 있다．

 QStrii培을 Key 값으로 사용하고 mllt Value를 저장하기 위해 다음과 같이 선언하여 방법을 사용할 수
 있다．

         QHash<QString, int> hash;


 QHash에 데이터를 저장하기 위해 Key와 Value를 같이 할당하기 원한다면 다음과 같은 방식을 사용할
수 있다．

         hash[ "one"] = 1;
         hash[ 'three"] = 3;
         hash[ "seven"] = 7;



QHash에 Key, Value를 삽입하기 위한 방법으로 insert( ) 함수를 사용할 수 있다. 그리고 value 값을
알기 위해 opera的r（연산자）를 사용하는 방법과 value( ) 함수를 사용할 수 있다．

                         (                          12)
1小
1hash.
               insert
                             "twelve    "   ,   .               ,;
H-nt numi = hash[ "thirteen' ] ;
!mnt num2 = hash. value                         (   "thirteen        "   );




188 CHAPTER 05. 데이터 타입과 유용한 데이터 조작 클래스


===== PAGE 190 =====
磁 QMultiHashKKey, T)
QMultiHash 클래스는 QHash 클래스로부터 상속받은 클래스이다. 다중의 Hash 값을 저장하기 위해
QHash보다 적합하다. QHash는 다중의 동일한 값을 허용하지 않지만 QMultiHash는 동일한 다중의
값을 허용하는 특징이 있다. 따라서 帥'lultiHash는 QHash의 확장한 형태의 클래스 기능을 제공한다．

QMultiuash<QString, jot> hashi, hash2, hash3;


hashl.insert ( "plenty", 100) ;
hashl.insert ( "plenty" , 2000) ;
// hashl. size () == 2


hash2.insert ( "plenty", 5000) ;
/7 hash2. size () == 1


hash3 = hashl + hash2;
7/ hash3. size () == 3



QMultiHash는 다중 값으로 저장된 아이템을 QList에 아이템으로 반환해 저장할 수 있다．

QList<int> values = hash.values ( "plenty ") ;


for (jot   j = 0; i < values. size () ; ++i)
     cout << values.at (i)    << endl;



S QMapKKey, T)
QMap의 사용 방법은 QHash와 매우 유사하며 제공하는 기능도 유사하다. 다음 예는 QString을 Key
로 사용하고 mllt를 Value로 선언하는 예이다．

QNap<QString, int> map;



Key와 Value를 帥'lap어］ 삽입하기 위해 operator[］와 insert( ) 함수를 제공한다．

map[ "one"] = 1;
map[ "three"] = 3
map[ "seven"] = 7


map.insert ( "twelve", 12) ;



만약 Key 값을 이용해 value 값을 얻어오기 위한 방법으로 contains( ) 함수를 사용할 수 있다．

 in七 七imeout; 口 30;


if   (map.contains ( "TThI日OUT ") )
     timeout = map. value ( "TIMEOUT") ;




                                                 1 데이터 타입과 유용한 데이터 조작 클래스 189


===== PAGE 191 =====
簪QMuItiMapKKey, T)
QMap 클래스로부티 상속받은 클래스이다. 다중 Mapping 값을 사용할 수 있는 기능을 제공한다. 따라
서 帥4ap을 확장해1 사용할 수 있다．

QMultiMap<QString, int> mapi, map2, map3;


inapl.insert ( "plenty ", 100) ;
mapl.insert ( "plenty ", 2000) ;
// mapl. size ( ) == 2


map2.insert ( "p1entyn, 5000) ;
// map2. size () == 1


map3 = mapi + map2;
/7 map3. size () == 3



蜘QPair(T1, T2)
QPa卄 클래스는 두 개의 아이템을 하나로 구성된 Pa卄로 저장할 수 있는 기능을 제공한다. 만약 STL 기
반의 pail를 활용하지 않는다면 QPair 함수를 사용할 수 있다. QPair 클래스는 다음과 같이 선언하여
사용할 수 있다．

QPair<QString, double> pair;


pair. first   = " pin;
pair. second = 3.14159265358979323846;



莎 0니st(T)
QList<T＞는 값을 저장하여 리스트 형태로 관리할 수 있다. 그리고 빠른 인덱스 기반의 액세스가 가능할
뿐만 아니라 저장된 데이터 삭제도 매우 빠르다. QList 클래스의 사용법은 QLinkedList, QVector 클
래스와 사용방법이 유사하다．

QList는 인덱스 기반의 클래스로, QLinkedList의 Iteratorr 기반보다 사용하기 편리하며 , 데이터 저장
시 메모리 할당하는 속도에서 QVector 보다 빠르다．

QList<int> integerList;
QList<QDate> dateList;


QList는 리스트 상에 아이템을 추가하기 위해 oper毗아를 사용할 수 있다．

QList<QString> list;
list   << 'one" << "two" << "three ";
// lis七： [ 노ne '' , " 七wo",   " 七hreeH ]



QList는 비교 연산자를 통해 리턴 값을 참조할 수 있다．


190 CHA口TER 05_ 데이터 타입과 유용한 데이터 조작 클래스


===== PAGE 192 =====
if     (uis七［0] == " 助b '1 )
       uis七［0] = " Rober七n ;



QList는 포인터 배열로 구현되어 있어 빠르게 연산자를 통해 QList어］ 저장된 값을 참조할 수 있다. 그리
고 at( ) 함수를 이용하면 리스트 상어］ 저장된 위치를 쉽게 참조할 수 있다．

for (mnt i      = 0; i < list. size () ; ++i) {
       if   (list. at (i)   == "Jane ")
             cout << "Found Jane at position " << i   << endi;
}


心 O니nkedList<T)
QLinkedList 클래스는 iterator 기반으로, 리스트의 아이템을 삽입하고 삭제하는 기능을 제공하는 클
래스이다. QLinkedList는 다음과 같이 선언할 수 있다．

QLinkedList<int> integerList;
QLinkedList<QTiine> timeList;



리스트 상에 아이템을 추가하기 위해 다음 예와 같이 operat야를 사용할 수 있다．

QLinkedList<QString> list;
list     << "one" << "two" << "three ";
// uis七： n oneH , 11七＼寸o ",      "three " ]



0QVector(T)
QVect야는 컨테이너 클래스 중 하나로, 메모리 위치어］ 해당 항목을 저장하고 빠른 인덱스 기반의 액세
스를 제공한다．

QVector<int> integerVector;
QVector<QString> stringVector;


QVe毗야는 Vec的r어］ 아이템을 저장한다. 일반적으로 Vector 크기는 선언 시 할당한다. 예를 들어 200
개의 저장 공간을 가지는 Vect아를 선언하기 위해 다음과 같이 작성할 수 있다．

QVector<QString> vector (200) ;



만약 200개의 저장 공간어］ Default 아이템으로 초기화가 가능하다．

QVector<QString> vector (200, "Pass ") ;


Vector에 저장된 아이템을 비교하거나 할당하기 위한 방법으로 Q＼旭毗야는 opera的r（연산자）를 사용할
수 있다．


                                                           1 데이터 타입과 유용한 데이터 不작 클래스 191


===== PAGE 193 =====
1if
               r[ O]
          (vect。              ==   "Liz   ")
            vector[ O] = "Elizabeth";



또한 at( ) 함수를 사용해 아이템을 검색할 수 있는 기능을 졔공한다．

      for (mnt i      = 0; i < vector.sizeO; ++i) {
            if   (vector.at (i)           == "Alfonso")
                  C（그Ut << "I그ound Alfonso a七 F刃siti아l " << i << endi;




 . Os怡ck(T)
QStack은 Stack 알고리즘을 제공하기 위한 클래스로, 맨 나중에 삽입된 데이터가 먼저 나오는 구조
 (LIF이이다．

      QStack<int> stack;
      S七ack . 1乂ish ( 1 ) ;
      stack.push(2) ;
      stack.push(3) ;


      while (! stack. isEmpty ( ))
            cout << stack.pop() << endi;



      eQOueueKT)
QQueue는 伽cue 알고리즘을 제공하기 위한 클래스로, 먼저 삽입된 데이터가 먼저 나오는 구조（FIF이
이며 Stack과는 반대의 개념이다．

      QQueue<int> queue;
      queue. enqueue ( 1) ;
      queue. enqueue (2) ;




                                                                         1
      queue. enqueue (3) ;


      while ( ! queue.isEmpty () )
            cout << queue.dequeue () << endl;



      S QSet(T)
QSet은 Qt의 Container 클래스의 하나이며 순서가 지정되지 않은 구조로 저장하므로 검색 시 속도가
매우 빠르다. QSet의 내부구조는 QHash로 구현되었다. QStrir培을 저장하기 위한 방법으로 다음과 같
이 초기화 할 수 있다．

      QSe七＜QS七ring> set;




192 CHAPTER 05_ 데이터 타입과 유용한 데이터 조작 클래스


===== PAGE 194 =====
데이터를 삽입하기 위해 다음과 같이 insert( ) 함수를 사용할 수 있다．

 set.insert ( "one") ;
 set.insert ( "three") ;
 set.insert ( "seven") ;



또한 데이터 삽입 시 , insert( ) 함수를 사용하는 방법 이외에 operator <<0를 사용할 수
                                                                           있다．

 set << "twelve " <c "fifteen " << "nineteen";




   毛J4J 문자열 클래스
문자열 클래스는 단순한 문자열을 표시하기 위한 경우 외에도 데이터 스트림 , 멀티 바이트 캐릭터 형태의
유니코드 4.O(Unicode Standard Version) 캐릭터를 지원하는 다양한 클래스를 지원한다．


0QByteArray
QByteArray 클래스는 바이트（8如t) 단위의 배열을 제공하는 클래스이며 문자 배열을 QByteArray에
저장하기 위한 방법은 다음과 같다．

QByteArray ba( "Hello Qt ") ;


size( ) 멤버함수를 이용해 "Qt" 문자 배열의 크기를 구할 수 있다. 문자 배열의 크기는 2를 리턴하지만
이 문자 배열은 추가로 '\O' 문자를 포함한다．
QByteArray에 저장된 문자 배열에 추가 및 변경을 하기 위해 append( ), prepen( ), insert( ),
replace( ) 그리고 지정한 위치부터 길이만큼 지우기 위해 remove( ) 멤버함수를 제공한다．


QByteArray x ( "Q") ;
x.prepend( "I love ") ;      II x == "I love Q "
x.append( "t _八八* ") ;       If x == "I love Qt U "k "
x.replace (13, 1, " 士 ") ;   II x == "I love Qt *"k "


remove( ) 멤버함수는 지우고자 하는 배열의 위치를 첫 번째 인자로 지정하고 위치부터 지우고자 하는
길이를 지정한다．

QByteArray x ( "I love Qt -八八出1' ) ;
x.remove (13, 4) ; II x == "I love Qt "


0QByteArrayMatcher
QByteArrayMatcher 클래스는 바이트 배열에서 매칭되는 바이트 배열 패턴을 찾기 위해1 제공되는 클
래스이다．


                                                         1 데이터 타입과 유용한 데이터 조작 클래스 193


===== PAGE 195 =====
QByteArray x ( "hello Qt, nice to meet you. ") ; II 전 I QByteArray
QBy七eArray y ( "Q七 '! ); // X에서 찾고자 하는 문자열

QByteArrayMatcher matcher (y) ;
in七 index = rnatcher.indexln(x, 0) ; /／문자열이 시작되는 위치 index 변수에 저장


qDebug ( '1index : %d'1 , index) ;
qDebug( "QByte : %c%c ",     x.at (index) , x.at (index+lfl;



I QChar
l6bit 유니코드 Character를 지원하기 위한 클래스이다．


QLabel *lbl = new QLabel ( " ", this) ;


QString str = "Hello Qt ";
QChar *data = str. data() ;
QString strHdisplay;

while ( !data->isNull() )
 {
     str_display. append(data->unicode () );
     ++data;
 }

 lbl- >setText (str display) ; II Hello Qt



0QLatinlString
US-ASCII/Latin-i 인코딩 문자열을 지원하기 위해 제공되는 클래스이다．

 QLatinlString latin ( "Qt ") ;
 QString str = QString ( "Qt ") ;

 if (str == latin)
      qDebug ( " Equal. " ) ;
 else
      qDebug ( "Not equal. ") ;

 bool is_equal = latin. operator ==(str) ;

 if (is equal)
      qDebug ( " Equal. ") ;
 else
        qDebug ( "Not equal. ") ;


 0QLocale
 QLocale 클래스는 숫자와 문자를 다양한 언어로 변환하기 위해 사용된다．


 194 CHAPTER 05_ 데이터 타입과 유용한 데이터 조작 클래스


===== PAGE 196 =====
bool Ok;
double d;


QLocale: :setDefault (QLocale: :C) ;


d = QString( "1234, 56 ") .toDouble (&ok) ;             7/ ok : false
if (ok) qDebug( "TRUE") ;
else qDebug ( "FALSE") ;


d = QString( "1234. 56 " ) .toDouble (&ok) ;            7/ Ok : true, d == 1234. 56
if (ok) qDebug( "TRUE") ;
else qDebug( "FALSE") ;


QLocale: :setDefault (QLocale: :German) ;
d = QString( "1234, 56 ") .toDouble (&ok) ;             7/ ok == true, d == 1234. 56
if (ok) qDebug( "TRUE") ;
else qDebug( " FALSE") ;

d = QString( "1234. 56 ") .toDouble (&ok) ;             /7 ok == true, d == 1234. 56
if (ok) qDebug ( "TRUE") ;
else qDebug ( "FALSE") ;



介 QString
QString 클래스는 유니코드 캐릭터의 문자열을 지원하는 클래스로, l6bit QChar를 저장할 수 있다．

QString str = "Hello";



QStrii培은 다양한 멤버함수를 이용해 비교, 문자열 길이, 문자열 위치 리턴 그리고 문자열을 비교할 수
있다．

QString str;

for (mnt i = 0; i < str. size() ; ++i)
{
      if        (str. at (i) >= QChar ( 'a' ) && str. at (i) <= QChar ( 'f ' ))
                 qDebug ( ) << "Found character in range [a-f] ";
}

QString compare_str;
if (compare str == "auto"              1 1 compare str == "extern")
{
      /7.   .   .




}


Null 문자열이거나 문자열이 빈 경우 확인하기 위해1 다음과 같은 멤버함수를 제공한다．




                                                                      L데이터 타입과 유용한 데이터 조작 클래스 195


===== PAGE 197 =====
QString() .isNull     );                7/ returns true
QString( ) .isEmpty () ;                7/ returns true


QString( " " ) .isNull () ;              /7 returns false
QString( " " ) .isEmpty () ;             /7 returns true


QString( "abc " ) .isNull () ;           // returns false
QString( "abc ") . isEinpty () ;         7/ returns false



QString은 %1, %2- %99까지 Argument를 이용해 문자열을 표시하거나 저장할 수 있는 기능을 제공한다．


QString i = "10 ";
QString total = "25 ";
QString fileName = "test. cpp";


QString status = QString ( "Processing file      %1 of %2: %3 ")
                 .arg(i) .arg(total) .arg(fileName) ;



0QStringList
QStringList 클래스는 QList<QString＞으로부터 상속받은 클래스로, Operation 연산이 가능하고
append(), prepend(), insert( ) 등의 멤버함수를 제공한다．

QStringList strList;
strList   << "Monday " << "Tuesday " << "Wednesday ";


QString str;
str = strList. join ( ", ") ; II   str == " Monday, Tuesday,Wednesday "



0QStringMatcher
QStringMatcher 클래스는 QString 문자열을 비교해 매칭되는 문자를 찾기 위한 기능을 제공한다．


QString x ( "hello Qt, nice to meet you. ") ; II 전체 QString
QString y ( "Q七") ; 7/ x에서 찾고자 하는 문자열


QStringMatcher matcher (y) ;


in七 index = ma七cher.indexln(x, 0) ; /／문자열이 시작되는 위치 index 변수에 저장
qDebug ( "index : %d", index) ; /7 index : 6




196 CHAPTER 05_ 데이터 타입과 유용한 데이터 조작 클래스


===== PAGE 198 =====
CHAPTER




  파일 입출력


===== PAGE 199 =====
（코 5 F가ogramming




r         i ' 파일 입출력
           플랫폼 상에서 파일 생성／수정／삭제 등과 같은 파일을 제어할 수 있는 API에 대해 알아보도록 하자．




Qt에서는 파일을 입·출력하기 위해 QFi1e 클래스를 사용한다. QFi1e은 I/O 디바이스를 통해 파일어］ 기
록된 바이너리와 텍스트, 리소스와 같은 파일의 내용을 읽거나 쓰기를 할 수 있는 기능을 제공한다．
또한 효율적인 데이터 스트림을 통해 데이터를 읽고 쓰는데 있어 QTextStream과 QDataStream 클래
스를 제공한다. 즉, 이 두 클래스는 파일어］ 직접 뎨이터를 기록하지 않고 파이프와 같은 인터페이스를 통
해 파일어］ 데이터를 읽고 쓰는 데 쉬운 인터페이스를 제공한다．

QTextStream 클래스를 사용한 0카

 QFi1e data ( 노U七Pu七．比t,, ) ;
 if   (data.open(QFile: :WriteOnly 1 QFile: :Truncate) ) {
      QTextStream out (&data) ;
      out << "Result: " << qSetFieldWidth(10) << left        << 3.14 << 2. 7;
       // writes "Result: 3. 14        2. 7




QFi1e 클래스는 QFileDev扼 클래스로부터 상속받은 클래스이다. QFileDevice 클래스는 OPEN된 파일
에 데이터를 READ 하거나 \URITE 하는 인터페이스를 제공한다 ．그리고 파일의 현재 위치 ，파일 크기，
Flush 등의 기능이 구현되어 있다．

OF陀 클래스를 이용해 직접 파일에 데이터 기록

 QFi1e file ( "in. txt ") ;
 if   (! file. open(QloDevice: :ReadOnly I QlODevice: :Text) )
      return;


         (! file. atEnd() ) {
         teArray line = file. readLine () ;
          'ess line (line) ;




             드R 06_ 파일 입출력


===== PAGE 200 =====
QFi1e 클래스는 파일 이름을 설정하기 위해 생성자 클래스에서 지정할 수 있지만 멤버함수인 setFile-
Name( ) 함수를 이용하면 특정 이름의 파일을 설정할 수 있다．
그리고 절대경로, 상대경로를 지정하기 위해 디렉토리를 파일명과 함께 표시할 수 있다. 디렉토리를 구분
하기 위해 Qt에서는 운영체제 플랫폼과 관계없이 ' /' 구분자를 사용한다. 그렇기 때문에 구분자로 ' \' 구
분자는 지원하지 않는다．

QFile 클래스를 이용해 직접 파일에 데이터를 기록하는 예제에서 보는 것과 같이 QFi1e 클래스는 file을
처리하기 위해 파일명은 생성자를 통해 설정한다. 그런 다음 파일을 열기 위한 멤버함수인 open( ) 함수
를 사용한다. 인자로 지정한 Argument는 파일을 열기 위한 옵션으로 파일을 어떤 모드로 Open 할지
결정한다．

예에서는 ReadOnly 방식으로 파일을 열고 디불어 텍스트 모드로 파일을 열 수 있다. 이와 반대로 파일
을 기록하기 위해서는 Write 모드를 사용할 수 있으며 印ODevice 클래스의 enum을 이용해 파일을 읽
기 모드, 쓰기 모드, 추가 모드 등을 지정할 수 있다．

Constant                 Va山e                    Descri口lion
이ODe미ce::No山pen         0x0000                   파일을 열지 않을 때 사용
QlODevice::ReadOnly     0x0001                   읽기 전용 모드로 사용
OlODevice::WriteOnly    0x0002                   쓰:7 ' 전용 모드로 사용
QIODevice::ReadWrite    ReadOnlylWriteOnly       읽기 전용 모드와 쓰기 전용 모드를 함께 사용
QlODevice::Append       0x0004                   파일 끝에 추가하기 위하1 사용
QlODevice::Truncate     0x0008                   만약 이전에 Open된 디바이스가 있다면 새로운 연결을 위
                                                 하1 이전에 사용된 디바이스는 삭제하기를 원할 때 사용
QlODevice::Text         0x00l0                   텍스트 모드로 파일을 읽을 때 마지막에 \n’을 사용하고，
                                                 Win32 경우 '\r\n을 마지막에 사용，
                              小              h




（기ODevice::Unbu卄ered    0x0020                   버퍼를 사용하지 않고 디바이스를 바로 사용



스트림을 이용해 파일의 내용 읽71

 QFile file ( 'in. txtn) ;
 if   ( ! file. open(QlODevice: :ReadOnly I QlODevice: :Text) )
      re七urn;


 QTextStreain in (& file) ;
 while ( !in. atEndU) {
      QString line = in. readLine () ;
      process line (line) ;




QTextStream 클래스는 파일로부터 저장된 8bit 데이터를 l6bit 유니코드 방식의 QString 데이터 타
입으로 변환하여 다루기 위한 기능을 가지고 있다．

attend( ) 멤버함수는 파일의 끝인지 판단하기 위해 사용되며 readLine( ) 함수를 이용해 파일어］ 기록된
데이터를 스트림을 사용해 읽어 들일 수 있다．


                                                                             ] 파일 입출력 199


===== PAGE 201 =====
 텍스트 스트림을 이용하면 <＜와 같은 오퍼레이터 연산을 통해 파일어］ 데이터를 Write 할 수 있는 기능
 을 제공한다．


 (( 연산을 사용한 파일에 데이터 기록

     QFile file ( "out.txt ") ;
 if     (! file. open(QloDevice: :Writeonly    QlODevice: :Text) )
         return;


 QTextStream out (& file) ;
 out << "The magic number is:        " << 49 << "\ n";


QDataStream도 QTextStream과 비슷해서 (( 연산자와 力 연산자를 사용할 수 있다. QFi1e 클래스 외
에도 QFilelnfo 클래스와 QDir 클래스를 사용해 운영체제의 플랫폼의 파일 시스템에 접근할 수 있다．

운영체제의 플랫폼의 특성에 따라 파일의 이름은 8bit encodii培으로 저장된다. 유닉스와 같은 방식은
파일 이름을 저장할 때 8b1t 방식으로 저장한다．
이러한 경우 QFi1e 클래스에서 제공하는 encode Name( ）와 decodeName( ) 함수를 이용해 8bit 방식
의 파일 이름을 디코딩 하거나 인코딩할 수 있다．

그리고 리눅스와 유닉스 계열의 /proc와 같은 하위 파일은 메모리상에 존재하는 파일 시스템이며 시스템
의 정보를 기록하는 뎨 메모리 공간을 사용한다. 이러한 파일은 size( ) 함수로 파일의 크기를 반환할 때，
0을 반환한다．

따라서 이러한 경우 /proc 하위의 파일의 내용을 읽기 위해 attend( ) 함수를 사용할 수 없다. 그러므로
파일을 읽기 위해 다음과 같이 isNull( ) 함수를 사용할 수 있다．


 QFile file ( "/ proc/modules ") ;                                   1
 if     (! file. open(QlODevice: :ReadOnly 1 QlODevice: :Text) )
         re七urn;


 QTextStream in ( &file) ;
 QString line = in. readLineO;
 while (! line. isNull () ) {
        process_line (line) ;
        line = in. readLine () ;
 }


그리고 파일에 기록되는 데이터가 리눅스와 유닉스 계열의 운영체제에서는 UTF-8을 Default로 설정되
는 경우 QTextCodec: :codeForLocale( ) 함수를 사용해 데이터를 처리할 수 있다．




200 CHAPTER 06_ 파일 입출력


===== PAGE 202 =====
. 파일 시그널과 슬롯 이벤트
QFi1e 클래스는 印Oflevice 클래스를 상속받은 클래스이다. 아ODevice 클래스는 다음과 같은 시그널
이벤트를 처리할 수 있다. 따라서 印ODevice를 상속받은 QFi1e 클래스에서 다음과 같은 클래스를 사용
할 수 있다．

（긔ODevice 시그널                              설명
void QlODevice::aboutToClose( )            디바이스가 닫혔을 때 발생
void （긔ODevice::bmesWritten（뎨nt64 bytes)   데이터가 w대TE되면 발생
void （긔ODevice::readChann이日nished( )       입력 스트림이 CLOSE되면 발생
void （긔ODevice::readyRead( )               데이터가 READ되면 발생



1 예외 처리
QFi1e 클래스를 이용해1 파일을 열기 , 읽기, 쓰기 , 삭제, 파일명 변경 , 복사 등과 같은 멤버함수를 사용해
예외사항이 발생되면 error( ) 멤버함수를 통해 발생한 예외사항을 확인할 수 있다．

enum QFi1e: :FileError


error( ) 멤버함수는 발생한 예외사항을 Qt에서 정의된 상수 값을 리턴한다. 예외사항으로 정의한 상수
는 다음과 같다．

상수                             값    설명
OF陀::NoError                        예외사항이 발생하지 않음
O디色:ReadE口or                   ]    파일로부터 데이터를 읽을 때 에러 발생
OFile::WriteError              2    파일（게 데이터를 쓸 때 에러 발생
O테e::F졔톄Error                  3    치명적인 에러 발생
OFile::ResourceError           4    파일을 열 수 없음
OFile::OpenError               5    파일을 열 수 없을 때 에러 발생
QFiPe::AbortError              6    실행이 중지되었을 때 에러 발생
QFiIe::TimeOutError            7    기meO마되었을 때 에러 발생
oFile::UnspecifiedError        8    듸冶E다or에 정의되지 않은 에러
QFiIe::RemoveError             9    파일을 제거할 수 없을 때 에러 발생
QFile::RenameError             10   파일의 이름을 바꿀 수 없을 때
OF陀：:PositionErr(가             11   파일의 위치를 변경할 수 없을 때 에러 발생
OF陀：:R(카引zeError               12   파일의 크기를 변경할 수 없을 때 에러 발생
OFiIe::PermissionsError        13   파일에 접근할 수 없을 때 에러 발생
OFile::CopyError               14   파일 복사를 실패했을 때 에러 발생




                                                                ] 파일 입출력 201


===== PAGE 203 =====
t；缸1 SIMPLE 파일 VIEW 예저1
이번에 다룰 예제는 QFile 클래스를 이용해 텍스트 파일을 읽어와 QPlainTextEdit 클래스 위젯에 출력
하는 예제를 다루어보도록 하겠다. QPlainText且dit 위젯은 텍스트 Viewer와 Edit 기능을 제공한다．
또한 상당히 큰 파일의 Docum아此를 처리할 수 있어 에디터 어플리케이션 개발에 유용하다．

QPlainTextEdit 클래스는 QTextEdit와 유사하다. 하지만 텍스트 기반의 데이터를 에디트하는데 고급
기능을 제공한다. 예를 들어 폰트와 컬러를 핸들링 할 수 있으며 문서 편집에 필요한 다양한 기능을 제공
한다. 그리고 QSyntaxl五ghlighter 클래스를 함께 사용해 에디트 상에 특정 단어는 High Light 표시
가 가능하다．

町MPLE 파일 \/IEM/ 어플리케이션은 텍스트 파일을 읽어오는 기능만 제공된다. 따라서 이외에 수정된
파일을 수정하는 기능은 추가해 완성해 보도록 하자．

class MainWindow : public QMainWindow
{
     Q OBJECT


public:
     MainWindow (QWidget *parent = 0) ;
     -MainWindow() ;


private:
     void createActions ( ) ;
     void createNenus Q;
     void loadFile(const QString &fileName) ;


     QMenu *file4enu;
     QAction *opeflAct;
     QHBoxLayout * layout;
     QPlainTextEdit *textEdjt;
     QString fileName;


private slots:
     void open() ;



createActions( ) 함수는 어플리케이션 메뉴에서 이벤트를 처리하기 위한 함수이며 , create八4enu( ) 함
수는 田lie] 메뉴 아이템을 Menu Bar어］ 등록하기 위한 함수이다. 사용자가 八ilenu 상에서 File을 클릭하
면 connection( ) 함수에서 등록한 시그널／슬롯 이벤트가 발생한다．

void MainWindow: :createActions ()
{
     openAct = new QAction(tr ( "&Open. ..") , this) ;
     openAct->setShortcuts (QKeySequence: : Open) ;
     connect (open如t, SIGNAL (triggered() ), this,    SLOT (open() ));
 }


202 CHAPTER 06_ 파일 입출력


===== PAGE 204 =====
QAction 클래스의 인스턴스 openAct는 사용자가 메뉴상에 [Open］을 클릭하면 connect( ) 함수의 네
번째 인자인 open( ) 함수를 호출하는 이벤트가 발생한다. setShortcuts( ) 함수는 Define된 항목 중
Open어］ 매칭된 단축키(百L ＋立）를 사용할 수 있다. 또한 QKeySequence는 단축키 지정이 가능하다．

QKeySequence ( QKeySequence: : Print) ;
QKeySequence(tr ( "Ctrl+P") );
QKeySequence(tr ( "Ctrl+p") );
QKeySequence (Qt: :CTRL + Qt: :KeyP) ;



QKeySequence 오브젝트에 등록된 표준 단축키는 운영체제에 따라 키의 Mappii培이 다르다. 예를 들
어 \Windows, Mac OS X에 따라 단축키의 玉4eta 값이 다르게 Define되어 있다．

StandardKey         Windows                              Mac OS X                KDE                                   GN아따E
HelpContents         Fi                                  01,1 41 ?i                                                    瓦
WhatsTh巴             Shift 十 Fl'                         S旴L+ Fli                                                      Shift +i1

Open                 Clil '+ 0                           CAt + 0                                                       CS口＋ 0


이ose                 Cirl 十F4         Clii 十w,           Ctri +W,      攷L+ f4]                                         ott

Save                 Girl -1- S                          竺匕＋立                                                          cst + S

Quit                                                     Clii +［萱                                                      （코H + （工

SaveAs                                                   Clii +   Shift 汁 Si                                           Clii +   Shift +5

New                 匣口＋團                                 Girl + N1               051 + N                                Girl + N

Delete              匣丑                                   DeL, Meta+LPI           四 r마n＋立                               Del      Cir + 口

Cut                 1可＋因 ,            Sh1iI +   Datr     CS 十 S」                 Ct小＋ 乂           F2口，                 CSI +    X

                                                                                 Shift -4- Da                          F2S      Shift +        CS


Copy                 弛＋르 051+ j『틔                        16姓＋立                   Ch1 i+ C,        F16                  051+ C

                                                                                 051 + Ins                             F個       GIrl +         nS

Paste                cw+ v , 旦쁘+ fnsr                    Ctrl +V                 CAt 十 \/         FIB                  Clii +V

                                                                                 Shift '+ Ins                          F侶       55咐 +          nS

F가efe円nces
Undo                4U+[i' , ［越j＋蜘姻                                              05 나- z.         了l4


Redo                 CtrL+ y,         sAt!.:+:e- l+ Z}   Ctrl i+ Shilt i+ ZJ     Gill +    Shift + Z                    Cli口十 Shift 十7

                     Alt +   SOft＋曲孤굽

Back                 /＼仕 + L 拓占恥
Forward                                                                                                                 A卄 +




Refresh                                                                          F5                                     CS口 + R


Zoomln                                                                                                                  0th 4

ZoomOut                                                                          Clii+ 크                                C甘卜 +


FuliScreen          Fif . AS +cAr!:                           +Meta+ F           Fft .    Ctrl ＋恒區If＋了］                 Ott +F作

Print                CVI+ P                              051 + P                 Ciii + P                               Ct寸 + P


AddTab               Ctrl +T                             dill -4- r              （가n 나 Sh出 + 卜1             （기n + T     Ohi+ T

NexfChild            .ct,l + nbJ Forward.                ct, + 1 , Forward,      Girl + Feb, F（기＼A罔川，                   Clii +J카가，

                     Ctrl 나 Fb                           Cl,! + Tebi              051 + Cteirri                        Forward
Pre\／幻usChild        C吼十Shift + TsblJ                    C枉1+ 0,       B琴日，      Ciii +    Shift -F- Tab.   Back        Chi +   54-It    -I-
                     Back         Clii +   Shif卜＋ FAt    Ctil i+ Shift :+ Tab    Ciii +                                 Back




                                                                                                                      ] 파일 입출력 203


===== PAGE 205 =====
디nd                           Cbll+ Fl                 흐피＋區                              Ct키+ 下j              Cot +     F


FindNext             圓 , 巫그＋回                                                            亘                    Ctrl+ G
                                                                                                                            !
                                                                                                                                  F3


듸ndF가ev山us           至咽＋回，                             面心回＋回                             ShIft + F3           CIrI +    ShIll +        C 1

                     Ch1 +區回＋回                                                                                Sh出 + Ft


Re히ace                        Ctrl + 田                 (none)                            Cot i+ B             CII +     H


SelectAll                     Ctrl + 可                                                   Cttl +A              Clnl +    A


B이d                           CIrI +    B              Cot +           B                 Chi +     B          GIrl + 日


It키IC                         CII +     1              Chi +           .                 Ctrl +    I          Clnl -f


Underline                     CE口 +     U              CDI +           U                 Ct,f +    U          Ctrl -I- U


MoveToNextChar                                             1

MoveT아가eviousChar
MoveToNext Word               Ctrl +                   Alt +                                                  CII +


MoveT아가eviou訓Vord             CII +                    Alt +                                                  CII +


MoveToNextLine
Mo＼尼ToPr今iiousLine
MoveToNextPage                                         匈   ［）어m    .




                                                       Ab 十型뽀，

                                                       Meta十亘匣i,
                                                       Meta＋ 由D（川n
MoveT아가eviousPage    匣回                                內Up ,               쁘t + F勺U口 .   F勺Up!                F勺U口

                                                       M이a十 브p .

                                                       Meta+               F勺U口


MoveT破光artO山ne                H어ne                     CS ＋늬，                            Home,

                                                       Meta十크
MoveToEndC가니ne                                         C벼＋크，                             End                  End I

                                                       Me冶＋크
MoveToS怡rtOf마)ck                                       Alt + Up              Meta+ A     (none)               (none)
MoveToEnd（거텨ock      (n。
                       ne)
                     (none)
                                                       A作 十 Down , Meta+ El              (none)               (none)
卜爪：)veToStartOf                                         CSI + Up              Home       CII + Hornml         CII + Home

Document
MoveToEndOf                                            흐피＋區回, ！呵                         Cot +     End        CIrI＋七誌

Document
SelectNextChar                                          ShIft +                          Shift +              Shift 4


Sele이Prey山usChar              S世ft + 니                 Shift +                           Shift 4              ShIft ＋二


SelectNextWord                Ct,I +    Shrft -1       A忙 + Sbrft +                      C뉘 + Shrtt +         Cot + 口 ＋日
S터ecU가今기ousWord               CInl +    ShIft +    -   씨t + SIr出 + -                     CII l+ Sh出 +         아r-f 旦匣)IJ ［크
S이ectNex止m e                  Sh,lt + Down              Shrft + Down                     Shift + Down         Sh滋 + Down


S쉬ec仟가evious니ne               Shift + Up               Shift + U口                        ShIft + U口           Shrf卜 + U口


SelectNextPage                ShIft + tqD。
                                         wrr               St汗t + 肉a川n                   Sf111 + 다；DOnI       Shift + 印D（川n


Selec作가eviousPage             ShIft +       F勺U口           Shift + 內U口                   ShIft +       F勺U口   S斗ft + PqU口


SelectStartOtLine             Shift + How包                 Cot +       Shift +           Shift + Home         SOdS + 加me


SelectEndOf Line              ShIft +       En（工           Cot +       Shift +           Sh附 +         Em工    Shift +       End


Selec侄計artO伯lock     (none)                            A比 + SbItt + U口                   (none)               (none)
                                                       Meta+ ShIft + A
Sek크ctEndOtB幻ck                                        AU + Shift + Down.                (none)               (none)
                                                       Meta+ ShIft + E



204 CHAPTER 06_ 파일 입출력


===== PAGE 206 =====
SelectS怡rt아                區圈＋基蚤麓＋匡瑚                 Ctrlj +百而n十U口         Cirl + Sdift + Home1     Ci, 十Sh푸t글＋Ho而j
Document                                            囹回十區回

Sele아EndOf                 匹因＋零蚤瑟＋區瑟                陋ii 1+ Sh浚二쉬SoonL      6打1 . 十Shot+ End         CtTt + SUit + End

Document                                            1Sb浪 !+ End三

DeleteStart（가W（가（J         L巫기＋晦                    忿藍＋團磁                 二그＋區延                     ctnl + 쁘竺多甘

D이eteEnd（거Word             흐固＋啼                     (none)                 Cid+ Del                 Ct,I + De[
DeleteEndOfLine            (none)                   (none)                 드빠＋ K                    nm + 乂
InsertParagraph            肛丑                       臘1Enter                                        Enter
O凸 r入凸 r凸 he,



Insert니neSeparator         匣回뛰亘匣3                   Meta+                  Shift + Enter            Shmft 十 Enter




open( ) 함수는 파일 다이얼로그 박스를 실행해 선택한 파일의 파일명을 QString 변수인 fileName 변
수에 저장한다. 만약 파일 선택이 정상적으로 되었다면 loadFile( ) 함수에 인자로 파일명을 전달한다．

void MainWindow: :open()
 {
        QString fileName = QFileDialog: :getOpenFileName(this) ;
        if      (! fileName.isEmpty ( ))
                loadEile (fileName) ;




loadFile( ) 함수는 파일 다이얼로그에서 선택한 파일을 QFi1e 클래스를 이용해 파일의 내용을 읽어들인
다. 만약 파일 Open시 예외가 발생하면 帥/lessageBox를 이용해 경고 메시지 박스에 에러 메시지를 출
력한다．

void MainWindow: :loadFile (const QString &fileName)
 {
        QFi1e file (fileName) ;
        if      (! file. open(QFile: :ReadOnly 1 QFile: :Text) ) {
                QMessageBox: :warning(this,      tr ( "Application") ,
                                           tr ( "Cannot read file    %l: \n%2. ")
                                           .arg(fileName) .arg(file. errorString() fl ;
                re七urn;
        }
        QTextStream in (& file) ;
        textEdit- >setPlainText (in. readAll() );
 }


QFi1e로부터 읽어들인 파일 데이터를 QTextStream 클래스를 이용해 스트림으로 처리할 수 있으며, 마
지막 라인에 읽어들인 파일의 텍스트를 QPlainTextEdit 클래스의 인스턴스에 출력한다．

QFileDialog 클래스는 파일을 선택할 수 있는 사용자 인터페이스를 제공한다. 이 클래스를 이용하면 파
일 필터링을 통해1 특정 파일의 확장자만 선택하는 것이 가능하다. 그리고 최근 열어본 파일의 디렉토리를
검사하여 디폴트 디렉토리를 설정할 수 있다．


                                                                                                  ] 파일 입출력 205


===== PAGE 207 =====
帥4essageBox 클래스는 사용자에게 경고 메시지 등 다양한 메시지를 사용자에게 전달할 수 있는 인터
페이스를 제공한다. 이 메시지 박스에는 Question, Information, Warning 그리고 Critical 아이콘을
사용해 표현할 수 있다. 그리고 메시지 박스에 버튼을 배치할 수 있으며, 메시지 박스 타이틀도 변경이 가
능하다．




206 CHAPTER 06_ 파일 입출력


===== PAGE 208 =====
CHAPTER




      그래픽스


===== PAGE 209 =====
Ot 5 Programming




          1 QPainter 클래스를 이용한 그래프

        느 QPainter를 이용하I GUI 상에 그래프를 표시할 수 있는 방법에 대하1 알아본다．




QPainter는 그래프（Line, Shape, Gradient 등）, 텍스트 그리고 이미지를 GUI 혹은 Qlmage, QOpen
GLPaintDevice, 帥Widget 및 QPrinter와 같은 QPaintDevice어］ 표시하기 위한 API를 제공한다．

여기서 QPaintDevice는 물리적인 디스플레이 화면에 직접 그리지 않고 논리적인 인터페이스의 중간 매
개체를 이용한다. 예를 들어 사각형의 도형을 그릴 때 , 렌더링하기 위한 대상이 邸Widget, QGLPixe1-
Buffer, Qlmage, QPixmap, QPicture 등 다양한 인터페이스에 그리기 위해 중간에 QPaintDevice
를 필요로 하기 때문이다．

QPainter는 그래프를 G1끄상에 표시하기 위해1 소프트웨어 기반의 rasterizer를 사용해 그래프를 표현
하는 방법과 OpenGL 및 OpenGL ES의 Back-end 시스템을 사용할 수 있다. 소프트웨어 기반의
rasterizer는 화면상에 점을 찍어 표현하고, OpenGL 및 Open（孔 ES 방식은 선을 이용해 그래프를 표
현하는 방식 이다．

QPair此er를 이용해 그래프를 그리기 위해 OpenGL Back-end를 사용할 수 있다는 것은 매우 큰 장점
중에 하나이다. 그 이유는 그래프를 표현할 때 3D 하드웨어 가속기 즉, 그래프카드에 내장된 3DHW 가
속기를 사용할 수 있기 때문에 그래픽 렌더링 속도는 매우 빠르게 표현할 수 있다．

또한 Qt Embedded Linux를 이용해 임베디드 디바이스 어플리케이션 작성 시, 사용하는 임베디드 디바
이스가 3D HW 가속기 모듈이 내장되어 있다면 QPainter를 이용해 2D 그래프를 그릴 때 3D HW 가속
기를 사용할 수 있다．




208 CHAPTER 07,.. 그래픽스


===== PAGE 210 =====
DQPainter를 이용한 렌더링 방식

종류                  설명

（긔mage             하드웨어의 독립적인 렌더링 방식으로 픽셀에 직접 접근하여 그래프를 표현할
                   수 있는 방식이다. QPainter상에 （긔mage를 이용하1 그래프를 표현할 때
                   （긔mage 인스턴스에 소프트웨어 기반의 rasterizer 방식을 사용한다．

아가xmap              이미지를 화면상에 표시할 때 적합하다 ．소프트웨어 기반의 rastenzer 방식을
                    사용해 이미지를 표현한다．

QOpenGLPain山e니ce    OpenGL 및 Open（孔 ES와 같은 하드웨어 기반의 가속기를 사용해 그래프률
                    표현하71 위한 방식이다．

0Bac시ngSt아e         QBackingStore는 OWindow를 위한 클래스로, 가장 상위 윈도우의 드로잉 영
                    역에 그래프를 표현하기 위해 사용된다. QBackingStore는 소프트웨어 기반의
                    rasterizer 방식뿐만 아니라 0口enGL 기반의 HW 가속기를 사용할 수 있다．

QWidget             QWidget 클래스는 위젯 영역에 그래프를 표현하기 위한 방식이다．



지금까지 살펴본 방식은 QPainter 클래스를 이용해 2D 그래프를 표현하는 방법이다. 311) 그래프를 사용
해 화면상어］ 렌더링하기 위한 방식은 추후 0penGL 장에서 다룰 것이다. 또한 UI 상에 그래프를 표현하
는 방식으로 Qt Quick을 사용하며 , 자세한 설명은 16장 Qt Quick을 참조하기 바란다．



다룰내용               설명
QPainter2I basic   기초적인 드로잉을 표현하7! 위하1 점, 선, 도형을 그리기 위한 0Pen, 도형 내부의
drawing            색을 칠하71 위한 0마ush를 설명
Gra（기en怡           0먀ush률 이용해 특정 기울71 방향으로 그레디언트를 표현




                     아inearGra뎨ent      0RadialGradient   OConicalOradient
Trans幻rn伺tion      확대와 축소（Scaling)
                   회전（R아計ion)
                   원근 표현（Perspective)
ComF兀sition        여러 레이어를 합성하기 위해 제공되는 기능




                                                               1 0Painter 클래스를 이용한 그래프 209


===== PAGE 211 =====
     1.1 QPainter2I Basic Drawing
이번 장에서는 QPaii此er를 이용해 점 , 선, 도형과 같은 기초적인 드로잉을 하기 위한 QPen과 QBrush
클래스어］ 대해 살펴보도록 하자．

어플리케이션 GUI상어］ QPaii式er를 이용해 드로잉하기 위해서는 paintEvent( ) 재정의 함수를 사용한
다. 이 멤버함수는 윈도우 영역이 업데이트되거나 다시 그려져야 하는 경우에 호출되며, repaint( ）와
update( ) 멤버함수를 사용하면 paintEvent( ) 함수가 호출된다. 예를 들어 윈도우 영역이 다른 윈도우
어］ 가려진 상태에서 다시 보여질 때 , paintEvent( ) 멤버함수가 자동으로 호출된다．

그럼 간단한 예제를 통해 paintEvent( ) 멤버함수를 사용하는 방법에 태해 살펴보기 위해1Qt Creat야로
프로젝트를 생성하고 헤더 파일과 소스 파일어］ 다음과 같이 코드를 추가한다．

幸mnci叱甘＜Qt（把i/QWidget>
#inciude <QPainter>


class Widget : public QWidget
{
     Q OBJECT


public:
     Widget (QWidget; 枉沮ren七 = 0) ;
     -Widget () ;


protected:
     void paintEvent (QPaintEvent *event) ;
};


헤더 파일어］ 선언한 paintEvent( ）는 GI끄상에 드로잉하기 위해 선언한 멤버함수이며 , update( ）와
repaint( ) 함수를 사용하면 paintEvent( ) 멤버함수가 호출된다．

void Widget: :paintEvent (QPaintEvent *event)
{
     QUNUSED (event) ;


     QPainter painter;
     painter.begin(this) ;


     painter. setPen(Qt: :blue) ;
     painter. drawLine (10, 10, 100, 40) ; II 선
     pain七er . drawRec七（120, 10, 80, 80) ; // 사각형


     QRectF rect (230. 0, 10. 0, 80. 0, 80. 0) ;
     pain七er . drawRol끄ldedRec七（rect, 20, 20) ; I/ 둥근 사각형


     QPointF pl[ 3] = {



210 CHAPTE只 071 그래픽스


===== PAGE 212 =====
                        QPointF(10. 0, 110. 0) ,
                        QPointF(110.O, 110.0) ,
                        QPointF(110. 0, 190. 0)
                    };
    pain七er.drawPolyline(pl,      3) ; // 포인트 지점을 선으로 그리기


    QPointF p2[ 3] = {
                        QPointF (120. 0, 110. 0) ,
                        QPointF (220. 0, 110. 0) ,
                        QPointF (220. 0, 190. 0)
                     };
    painter. drawPolygon(p2, 3) ; I/ 포인트 지점으로 도형그리71


    painter. se七Fon七（QFon七（"Anial1',      20) ) ; // 폰트지정
    painter. setPen(Qt: :black) ;
    QRect font乙rect (10, 150, 220, 180) ; // 텍스트를 표시할 영역
    painter .drawText ( font_rect, Qt: :AlignCenter, "I love Qt. ") ;


    painter. end ( );
}



begin( ) 함수는 드로잉을 시작하는 함수이며 마지막 라인의 end( ) 함수는 Paint 디바이스를 닫기 위한
멤버함수이다. begin( ) 함수는 인자가 없지만 이미지나 위젯을 명시할 수 있다．

begin(）과 end( ) 함수는 버퍼에 드로잉한 다음 end( ) 함수를 호출하면 페인트 디바이스에 드로잉을 하
게 된다. 따라서 더블 버피링과 같이 상황에 따라 그려지는게 시각적으로 보여지는 것을 방지할 수 있다．
그리고 begin( ) 함수의 인자로 위젯을 명시하면 특정 위젯상어］ 드로잉을 할 수 있다．


painter->begin(0) ;


QPixmap image(0, 0) ;
painter->begin( & image) ;


painter->begin ( myWidget) ;
painter2->begin (rnyWidget) ;


drawLine( ）는 선을 드로잉하기 위한 멤버함수로써 xl, yl 좌표부터 x2, y2까지 선을 드로잉하며
drawRect(）는 사각형을 표시하기 위한 멤버함수이다．

drawRoundedRect( ) 멤버함수는 모서리가 둥근 사각형을 드로잉하는 멤버함수이며 두 번째 인자는 x
축 기울기이고, 세 번째 인자는 y축 기울기이다．

drawPolyline( ) 함수는 QPointF로 선언한 좌표를 순서대로 선을 드로잉하는 함수이며 draw-
Polygon( ) 함수는 좌표로 도형을 표시하는 멤버함수이다. 이 두개 함수의 두 번째 인자는 QPointF로
선언한 좌표의 개수를 명시하면 된다．


                                                              1 0Painter 클래스를 이용한 그래프 211


===== PAGE 213 =====
     I가




                                  I love （값．

（그림） OPainter를 이용한 드로잉



0OPen
QPen 클래스는 QPainter를 이용해 드로잉할 때, 선과 도형 윤곽의 컬러 , 두께, 스타일을 다양하게 표현
할 수 있도록 제공하는 클래스이다．

r小
     QP
                 ‘뇨ter                      ,
                                                pai
                                                             「『；
                                                           " 七     .




   /QPen pen(Qt: :blue,                                                 3, Qt: :SolidLine, Qt: :RoundCap, Qt: :RoundJoin) ;
1 쓰2ren  Pe민．닙t:,:D上U.e '
  QPen pen(Qt: :blue) ;
1 Pe1l setWidth(4)
  pen. :5eLVV上（그tn ;; '                                    (qJ
     painter. setPen(pen) ;
     QRect rectl (10.0, 20. 0, 80. 0, 50) ;
     painter. drawEllipse ( recti) ;


      pen. setStyle (Qt: :DashLine) ;
      painter. setPen(pen) ;
      QRectrect2 (110.0, 20. 0, 80. 0, 50. 0) ;
      painter.drawEllipse (rect2) ;



     setWidth(）는 선의 두께를 지정할 수 있는 멤버함수이다. setStyle( ) 멤버함수는 선을 드로잉하는 패턴
     을 지정할 수 있다．




          （二＞
           /'/            '       누         '   \
                                                      (:
                                                                 :::)
            '\
                  .           -       /,J
                                                                                      /


     （그림） setStyle( ) 함수를 이용한 드로잉


     212 CHAPTER 07_ 그래픽스


===== PAGE 214 =====
상수                      값        설명
（가：:N아七n                0        선을 드로잉 하지 않을 때 사용
Qt::S이b니ne              l        직선 패턴
Qt::Dash니ne             2        긴 점선 패턴
01::［兀tLine             3        점선 패턴
아1DashDot니ne            4        긴 점선, 점선 패턴
Qt::DashDotD아Line       5        긴 점선, 점선, 점선 패턴
（거::(加없omDash口ne        6        사용자 정의 패턴



capStyle( ) 함수를 이용하면 드로잉하는 선의 끝부분을 Flat, SquareCap과 둥근 원형의 RoundCap
스타일을 지정할 수 있다．

 pen. setCapStyle (0t: :FlatCap) ;
 painter. setPen (pen) ;
 painter.drawLine (30, 30, 200, 30) ;


 pen. setCapStyle (Qt: :SquareCap) ;
 painter. setPen (pen) ;
 painter.drawLine (30, 70, 200, 70) ;


 pen. setCapStyle (Qt: :RoundCap) ;
 painter. setPen (pen) ;
 painter.drawLine (30, 110, 200, 110) ;



                                                     01. FlatCap


                                                     01::SquareCap


                                                     Qt::RoundCap
   H

（그림） setCapStyle()


 상수              값          설명
 Qt::FlatCap     Ox00       티at 스타일
 Qt::SquareCap   Ox0]       끝 좌표에 사각형이 확장된 스타일
 ot::RoundCap    0x02       끝 좌표에 둥근 사각형이 확장된 스타일



각 좌표에 따라 선 ，도형을 연결하는 모서리의 스타일을 지정할 수 있도록 Joix侶tyle을 제공한다．




                                                     1 QPainter 클래스를 이용한 그래프 213


===== PAGE 215 =====
 QPointF pl[ 3] = {
     QPointF (30. 0, 80. 0) ,QPointF (20. 0, 40. 0) , QPointF (80.0, 60. 0) };
 pen. setJoinStyle ( Qt: : BeveiJoin) ;
 painter. setPen(pen) ;
 painter.drawPolyline(pl, 3) ;


 QPointF p2[ 3] = {
      QPointF (130.0, 80. 0) , QPointF (120. 0, 40. 0) , QPointF(180. 0, 60. 0) };
 pen. setJoinStyle (Qt: :MiterJoin) ;
 painter. setPen(pen) ;
 painter. drawPolyline (p2, 3) ;


 QPointF p3[ 3] = {
      QPointF(230.0, 80. 0) , QPointF (220. 0, 40. 0) , QPointF (280. 0, 60. 0) };
 pen. setJoinStyie (Qt: : RoundJoin) ;
 painter. setPen(pen) ;
 painter.drawPolyline (p3, 3) ;



 恥                          1口 回




卜 卜 卜
（그림） setJoinSt小（)



 상수             값        설명
Qt:: M什er幻In     OxOO    선이 만나는 좌표의 모서리를 삼각형으로 표시
Ot:: BeveLJ（川    0x40    끝 좌표를 채우는 스타일
Qt:: Roun山oin    0x80    끝 좌표를 둥근 형태로 채우는 스타일



S QBrush
QBrush 클래스는 QPainter어］ 의해 드로잉된 도형을 지정한 컬러로 채울 수 있는 기능을 제공한다．
QBrush 클래스의 setStyle( ) 멤버함수는 enum 값으로 정의된 값을 인자로 지정하면 내부를 칠할 때
패턴을 지정할 수 있으며 , 제공하는 패턴은 다음과 같다．




214 CHAPTER 07_ 그래픽스


===== PAGE 216 =====
=     Qt::S에dPattern       Qt::DenselPattern        Qt::Dense2Pattern




=  0t::Dense3Pattern       Qt::Dense4Pattern
                                                   mQt::Dense5Pattern




   Qt::Dense6Pattern       Ot: Dense7Pattern           Qt::NoBrush




      Qt::H아Pattern          Qt::VerPattern          Qt :0 ossPattern




    0仁B미agPattern           Qt::F미agPattern       （가：:［거ag아ossPattern

（그림） QBrush Style



QBrush는 그레디 언트 패턴을 이용해 도형 내부를 칠할 수 있는 기능을 제공한다．




（거1Unead카羽ientPattern
                                              口山
                        （孔Ra비톄臼a비en甲attern     이1C帥（訓뇨的ientPattern
（그림） OBrush Style



 painter. setBrush(QBrush(Qt: : green, Qt: :Dense3Pattern) );
 painter. setPen(Qt: :blue) ;
 painter. drawEllipse (10, 10, 100, 100) ;


 painter. setBrush(Qt: :NoBrush) ;
 painter. setPen(Qt: :blue) ;
 painter. drawEllipse(80, 10, 100, 100) ;

  刃
                                    QPainter 클래스의 setBi끄sh( ) 멤버함수는 QBi끄sh를 지정할 수 있
                                    다. QBrush의 첫 번째 인자는 도형 내부에 칠해질 색의 컬러를 지정할
                                    수 있으며 , 두 번째 인자는 패턴을 지정할 수 있다．




（그림） QB山sh의 패턴


                                                                        1 QPainter 클래스를 이용한 그래프 215


===== PAGE 217 =====
QPixmap pixmap ( n : resources/qtblog.png") ;
mnt w = pixmap.width( );
mnt h = pixr咀p.hei야此（) ;
pixmap. scaled(w, h, Qt: : IgnoreAspectRatio, Qt: :SmoothTransforination) ;

QBrush brush(pixmap) ;
painter. setBrush (brush) ;
painter. setPen(Qt: :blue) ;
painter.drawRect (O, 0, w, h) ;



QBrush 클래스 생성자의 첫 번째 인자에 QI芍xmap을 인자로 선언하면 도형의 내부를 이미지로 채울 수
있다. QPixmap 클래스의 scaled( ）는 이미지의 크기를 변경하기 위해 사용하는 멤버함수이다. 세 번째
인자는 이미지를 스케일링하기 위한 옵션이며 제공하는 종류는 다음과 같다．



                                 比
              岫烈粱
             IgnoreA히：冶ctRatio   KeepAspec日at幻 KeepA햐冶Ct由如ByExpanc｝汭g

（그림） 스케일링 옵션



네 번째 인자는 필터링 방식을 지정할 수 있으며 Qt::SmoothTransformation는 bilinear 필터링 기법
을 사용해 이미지를 QPixmap 인스턴스에 렌더링한다．




                    Code less.
                    Create more.
                    Dep佃yevery1八／here.

（그림） QB띠sh의 이미지 패턴



 QRadialGradient gradient (50, 50, 50, 50, 50) ;
 gradient.setColorAt (0, QColor: :fromRgbF (O, 1, 0, 1) );
 gradient. setCoiorAt (1, QColor: :from之gbF (O, 0, 0, 0) );
 QBrush brush(gradient) ;


painter. setBrush (brush) ;
painter.drawRect (0, 0, 100, 100) ;




216 CHAPTER 07_ 그래픽스


===== PAGE 218 =====
QBrush는 도형의 내부를 칠하기 위한 패턴으로 그레디언트를 지정할 수 있다. QRadialgradient 클래
스로 선언된 인스턴스를 QBrush 생성자의 첫 번째 인자로 지정하면 drawRect( ) 함수로 드로잉한 사각
형 내부의 패턴으로 사용할 수 있다．


          回mm




（그림） QBrush의 그레디언트 패턴




   t1Gradien恰
그레디언트는 다른 말로 '기울기' 라는 사전적 의미가 있다. 벡터 미적분학을 이용해 기울기를 나타내는
벡터장을 증가율의 크기에 따라 그래프로 표시하기 위해 제공하는 기능으로 다음과 같은 그레디언트를
사용할 수 있다．

（打a미ent            설명
（긔inearGra비ent     시작 좌표에서부터 마지막 좌표까지 선형 그레디언트를 사용해 표시




                                          ’也
                                          x2, y2


QRadial(計adient    cx, cy 좌표를 중심으로 원형 형태로 그레디언트를 표시




OConicaiGradient   cx,cy 좌표에서 각도를 중심으로 그래디언트를 표시




                                                      1 QPainter 클래스를 이용한 그래프 217


===== PAGE 219 =====
00니nearGra비ent
QLinearGradient는 시작점에서 마지막점까지 그레디 언트를 표시할 수 있는 기능을 제공한다．


                        xl,      yl
                          " ' ·．,.




                                      " " " ’뇨

                                          x2, y2


（그림） 아inearGraient



 QLinearGradient ling (QPointF(70, 70) , QPoint ( 140, 140 ) );
 ling. setColorAt (O, Qt: :blue) ;
 ling. setColorAt (1, Qt: :green) ;


 ling. setSpread( QGradient: :PadSpread );
 //linGrad. setSpread( QGradient: :RepeatSpread );
 //linGrad. setSpread( QGradient: :ReflectSpread );
 QBrush brush(ling) ;
 painter. setBrush (brush) ;
 painter. drawRect (0, 0, 200, 200) ;




QLinearGradient 클래스 생성자의 첫 번째 인자에 시작점을 지정하고 두 번째 인자에 마지막점을 지정
해 그레디언트를 표시할 수 있다. setColorAt( ) 멤버함수는 시작점부터 마지막 지점까지 표시할 색상을
지정할 수 있으며 , setSpread( ) 멤버함수를 이용해 시작점에서 마지막 지점 밖의 영역을 표시하기 위한
패턴을 지정할 수 있다．

                                       r           口
                                                       回




                                                                \


 QGradient::PadSpread                 QGradient::RepeatSpread   QGradient::RefIectSpread

（그림） QLinearGra（引ent




2侶 CHAPTER 07叫 그래픽스


===== PAGE 220 =====
0QRa비aiGra비ent
QRadialGradient 클래스는 원을 중심으로 그레디언트를 표시하기 위한 기능을 제공한다. cx, cy는 중심
점이고 radius는 중심점으로부터 원의 반지름이다. 그리고 fx, fy는 그레디언트를 표시할 시작점이다．




（그림） QRadialGra（기ent



    QRadialGradient radg(100, 100, 50, 120, 120) ;


    radg. setSpread ( QGradient: : PadSpread) ;
    radg.setColorAt ( 0, Qt: :biack );
    radg.setColorAt ( 1, Qt: :white ) ;


    QBrush brush(radg) ;
    painter. setBrush (brush) ;
    painter. drawRect (0, 0, 200, 200) ;



QRadialGradient 클래스 생성자의 첫 번째 인자와 두 번째 인자는 cx, cy 좌표이고 세 번째 인자는
radius이다. 네 번째와 다섯 번째 인자는 fx, fy 좌표를 지정할 수 있다．

              m匹m




\


    QGradient::PadSpread       QGradient::RepeatSpread   QGradient::ReflectSpread

（그림） QRadialGradient



1QConicalGradient




                             戶
                                                  QConicalGradient 클래스는 cx, cy 좌표에서 an멤e（각
                                                  도）을 중심으로 그레디 언트를 표시할 수 있는 기능을 제공
                                                  한다．




（그림） oc（그nicaiGradient


                                                                     1 （가治inter 클래스를 이용한 그래프 219


===== PAGE 221 =====
r
    QConicalGradient cong( 100, 100, 45. 0 );
    cong. setColorAt ( 0, Qt: :black );
    cong. setColorAt ( 1, Qt: :white );


    QBrush brush(cong) ;
    painter. setBrush (brush) ;
    painter. drawRect (0, 0, 200, 200) ;



QConicalGradient 클래스 생성자의 첫 번째 인자와 두 번째 인자는 cx, cy 좌표이며 세 번째 인자는 각
도를 지정할 수 있다．




（그림） OC(：가기caiGradient




      t        가ans幻rmation
QTransform 클래스를 이용하면 Scaling（확대／축소）, Rotation（회전）, Perspective（원근 표현） 기법을
QPaii此er 인스턴스에 적용할 수 있다．


          ＄어北（:eIm的a               Scaling             Rotation   Perspective

                                  Qt
     여難河，
（그림） OTrans幻rm을 이용한 Sc졔ing, Rotat山n, Perspective 기법



    Qlmage image ( " :/resources/qtblog.png") ;


    QPainter painter (this) ;
    painter. setPen(QPen(Qt: :blue, 1, Qt: :DashLine) );
    painter. drawRect (0, 0, 100, 100) ;


    QTransform transform;                                                       0


    220 CHAPTER O7_ 그래팍스


===== PAGE 222 =====
 transform.translate (50, 50) ;
 transform. rotate ( 45 ) ;
 transform. scale(0.5, 0. 5) ;


 painter. setTransform(transform) ;
 painter. drawlmage (0, 0, image) ;



QTransform 클래스의 translate(）는 원점 좌표를 지 정한 x, y 좌표로 변경할 수 있다. 소스 코드에서
보는 것과 갇이 translate( ) 멤버함수를 이용해 0, 0 원점 좌표를 50, 50 원점 좌표로 변경할 수 있다．

  Painterdrawtmage(O, 0, image);
(0川                                                 r   ==1111=   =1=   ==1=   =1=   =====1=   ====1=   ==1=




                                  Tran割a始（晟）, 5口｝                       (50,5아
                                  H

 L                            J


（그림） translate( ) 함수를 이용한 원점 좌표 변경



rotate( ）는 렌더링한 이미지를 45도 회전할 수 있으며 , scale( ）는 렌더링한 이미지를 확대하거나 축소
할 수 있다．




（그림） 확대와 축소



 painter. drawRect (0, 0, 100, 100) ;


 QTransform transform;
 transform.transiate (50, 50) ;
 transform.rotate (70, Qt: :YAxis) ;


 painter. setTransform( transform) ;
 painter. drawlmage (0, 0, image) ;




                                                                                                               1 QPainter 클래스를 이용한 그래프 221


===== PAGE 223 =====
（그림） 확대와 축소



rotate( ) 멤버함수는 Perspective 기법을 이용해 원근을 표현할 수 있다. 두 번째 인자어］ Perspective
상수 값을 지정하면 x축, Y축, z축 원근 기법을 표현할 수 있다．

상수                         값             설명
 Qt::XAxis                 0             x축 이동
 Qt::YAxis                 ]             Y축 이동
Qt::ZAxis                  2             z축 이동




                                Translate. rotate (50, Qt: :XAxis)


                                          Trarisla七e. rotate (50, Q七 : : YAxi引

                                            （그림） Perspective 기법



    t          Composition
QPai砒er를 이용해1 도형 혹은 이미지를 사용했을 때 , 중첩된 영역을 Composition mode（중첩 모드）로
사용할 수 있다. 페인트 디바이스상에서 Qlmage를 Composition 모드로 사용할 경우 Format
ARGB32_Pr이flu比印lied 혹은 Format ARGB32 포맷 중 하나를 사용해야 한다．




                                         月                  !              'V
    S。   u                                Destinationover       Sourcein        Desthiationln




         d卜
   SourceOut   DestinationOut


（그림） Comsition 모드
                                         기 卜d
                                          DesthiationAtop        Clear              Xor




222 CHAPTER 07 그래픽스


===== PAGE 224 =====
painter. drawlmage(O, 0, destinationlmage) ;
painter. setCompositionNode (QPainter: : CompositionNodeDestinationOver) ;
painter. drawlmage (0, 0, sourcelmage) ;


Painter::CompositionModeDestinationOver 상수 값을 set（拍mpositionMode( ) 함수의 인자로
전달하면 Destin毗ion의 알파 값이 Source 픽셀 위에 블렌딩된다．




                                                            1 QPainter 클래스를 이용한 그래프 223


===== PAGE 225 =====
Qt 5 Programming




r         2「／（計a아기cs View 다amewo水

          수많은 그래떡 요소를 GUI 상에 표시, 확대, 축소 등과 같은 수많은 그래삑 요소를 효과적으로 표시하
          거나 관리할 수 있는 AP뻬 대해 살펴보도록 하자．




QPushButton, QLabel, Q（그heckBox, QListWidget과 같은 GI끄를 구성하는 위젯 혹은 커스터마이징
된 그래픽 아이템을 사용해 어플리케이션을 개발하는 것은 상당히 유연하고 개발하기 쉬우며 사용자에게
좋은 User Experience GI끄를 설계할 수 있다. 하지만 GUI상어］ 그래픽 아이템을 작게는 수십 개 혹은
수백 개를 사용해 사용자에게 보여지는 스크린을 완벽하계 제어하는데 많은 제약이 있다．

어플리케이션 상어］ 사용자에게 보여지는 Surface를 관리하고 개발자가 커스터마이징 한 2D그래픽 요소
들을 렌더링 , 줌을 이용한 확대 축소, 회전과 같이 어플리케이션상에서 상호 작용할 수 있는 인터페이스
를 제공한다．

Graphics View Framework는 BSP(Binary Space Partitioning) Tree 알고리즘을 사용한다. BSP
는 공간을 2개로 분할하는 알고리즘이다. 큰 지형을 이진（Binary) 트리 형태로 분석해 Node 정보를 구
성한다. 그리고 이를 참조해 렌더링할 대상을 찾아내는 원리이다．


                                     Space Root




                                     2진（Binary) 트리


（그림） 텨nary Space Partitioning 알고리즘


BSP 알고리즘을 사용하는 Graphics View는 그래픽 아이템을 매우 빠르게 발견할 수 있다. 따라서
Graphics View를 Surface로 사용해 그래픽 아이템을 GUI상에 렌더링하는 경우 매우 빠르다. 심지어
수백 개의 아이템을 매우 빠른 속도로 렌더링 할 수 있다．



224 CHAPTER 07_ 그래픽스


===== PAGE 226 =====
1 (카aphics View 다amewo水 기본 요소
Graphics View Fran始work를 기반으로 어플리케이션을 작성하기 위해 다음과 같은 클래스를 제공한다．


[QGraphicsViewl
QGraphicsView는 스크린상어］ 위젯을 표시 혹은 디스플레이 하기 위해 제공되는 클래스이다. 위젯이
View상에 보여지는 영역과 큰 스크린을 사용자에게 모두 보여주기 위해1 사용하는 화면 스크롤 바 영역이
QGraphicsView어］ 포함된다. View는 사용자가 화면으로부터 버튼을 클릭하거나 터치를 이용해 입력
이벤트를 받을 수 있으며 , 사용자에게 보여지는 View 영역에서 발생하는 입력 이벤트를 보내기 전에 스
크린 이벤트를 제어할 수 있다．


[QGraphicsScene]
QGraphicsScene은 위젯을 저장하고 키보드나 터치로부터 생겨나는 이벤트를 처리할 수 있으며, 또한
아이템들이 포커스 또는 선택된 것과 같은 아이템들의 상태를 관리하기 위한 목적으로 제공되는 클래스
이다．


[QGra아기C帥em]
QGraphicsltem은 Graphics View 상의 그래픽 아이템을 구현하기 위해 제공되는 클래스이다. 또한
QGr町血icsltem은 그래픽 아이템을 그룹으로 관리할 수 있는 인터페이스를 제공한다. 그래픽 아이템으
로써 , 사각헝 모양과 같은 전형적인 도형 아이템을 위해 QGraphicsR吼tltem을 타원과 같은 아이템을
위해 GRaphicsEllipseltem을 제공하고 텍스트를 렌더링하는 아이템을 구현하기 위해 QGra하iics
Textltem 클래스를 제공한다.


           QGraphicsView    QGraphicsScene




                      \ /
                  0（計a口hicsltem

（그림） Graphics View 다amework




                                             2Gm아기Cs View 다amework 225


===== PAGE 227 =====
 S Graphics View 다amework 이하를 위한 간단한 예제

 #include <QApplication>
 半include " widge七．h'
 #include <QGraphicsView>
 #include <QGraphicsScene>
 #include <QGraphicsltem>


 in七 main(in七 argc, char 出argv[ ] )
 {
      QApplication a (argc, argv) ;
      QGraphicsScene scene;
      scene. addText ( "I love Qt programming. "
                           r QFont ( "Times ", 22, QFont: :Boldfl;


      QGraphicsView view(& scene) ;
      view. show () ;
      return a. exec () ;c
 }


                                  口 回 hm


     I love Qt programming

（그림） G田아기Cs \/e小／ 예제



 QGraphicsScene scene;


 QPainterPath path;
 path.moveTo (30, 120) ;
 path.cubicTo (80, 0, 50, 50, 80, 80) ;


 scene. addPath(path, QPen(Qt: :black) , QBrush(Qt: :green) );
 scene. addText ( "I love Qt programming. ", QFont ( "Times ", 15, QFont: :Bold) );


 QGraphicsView view(& scene) ;
 view. show() ;



                   ［回

 I love Qt programming.



     I
（그림） Graph心 \/ew 예제


226 CHAPTER 07 그래픽스


===== PAGE 228 =====
     2.1 , Graphics View Architecture
Graphics View는 Model/View 프로그래밍에서 아이템 기반으로 구현할 수 있다. 예를 들어 QTable
\／扼w, QTreeView 그리고 QListView와 같은 편리한 클래스를 통해 Graphics View어］ 아이템을 렌더
링 할 수 있으며 다양한 기하학적 도형을 Scene어］ 포함할 수 있다. QGraphicsScene은 Graphics
View scene을 제공하며 다음과 같은 기능을 포함하고 있다．

 · 많은 아이템을 빠르게 제공하고 관리
 · 각 아이템어］ 이벤트를 전달
 · 아이템의 선택 혹은 포커스 핸들링과 같은 아이템 상태를 관리
 .U砒ransformed 렌더링 기능을 제공한다（주로 프린트 기능에서 사용）.

Scene은 QGraphicsltem 오브젝트를 위한 Container를 제공한다. 아이템을 추가하기 위해
QGraphicsScene 클래스의 addltem( ) 함수를 제공하고 items( ) 함수를 이용해 많은 아이템 중 하나
를 검색할 수 있으며 items( ）의 오버로드 된 함수를 이용해 Rectangle, Point, Polygon과 일반적인
Vector path를 포함한 모든 아이템을 리턴할 수 있다．

QGraphicsScene 클래스는 x, Y 좌표를 이용해 가장 근접한 아이템을 리턴하기 위해 itemAt( ) 함수를
사용할 수 있다．

QGraphicsScene scene;
QGraphicsRectltem *rect = scene. addRect (QRectF(0, 0, 100, 100) );


QGraphicsltem *item = scene.iternAt (50, 50) ;
II item == rect



QGraphicsScene의 이벤트 전달 아키텍처는 아이템에서 발생하는 이벤트를 위해 scene이 Schedule
할 뿐만 아니라 아이템 사이의 이벤트도 관리하는 기능을 제공한다. 또한 각 아이템의 상태를 관리하며
set SelectionArea( ) 함수를 사용하면 선택한 임의의 도형을 전달할 수 있다. 또한 이 함수는 고무밴드
와 같이 모양이 변하는 아이템을 QGraphicsView에서 사용할 수 있다．

아이템에 키보드와 포커스를 사용할 수 있다. setFocusltem( ) 함수를 사용하면 선택한 아이템에 포커
스를 이동할 수 있다. 또한 동일한 기능으로 setFocus( ) 함수를 사용할 수 있다．

마지막으로 QGraphicsScene은 paint device로부터 QGraphicsScene 클래스의 render( ) 함수를 통
해 scene 일부분 렌더링을 허용한다．


1View
QGraphicsView 클래스는 scene어］ 포함된 아이템을 표현하기 위한 View 위젯을 제공한다. 그리고 같은
scene에서 다른 view어］ 접근할 수 있으며 view 위젯은 표시되는 영역에 스크롤 바 기능을 제공한다. 또한
view 위젯은 QWidget 클래스로부터 파생된 QGLWidget 상에 setViewport( ) 함수를 이용할 수 있다．


                                                              乙Grap볘Cs View 다amework 227


===== PAGE 229 =====
QGraphicsScene scene;
myPopulateScene ( & scene) ;


QGraphicsView view (& scene) ;
view. show) ) ;




0Item
QGraphicsltem은 scene에서 그래픽 아이템을 위한 상위 클래스로, Graphics View는 일반적인 표준
도형을 위한 다음과 같은 클래스를 지 원한다．

아이템               .        클래스
Rectangle                  QGraphicsRectltem
E川口se                      QG田아기csElli口seltem
Text item                  (QGraphicsTextltem)



위에서 제공하는 클래스보다 가장 많이 사용하는 클래스는 QGraphicsltem 클래스이다. 이 클래스는 사
용자가 지정한 아이템을 사용할 수 있다. 즉 작성한 커스텀 모양의 아이템을 사용할 수 있다. QGraphics
Item은 다음과 같은 기능을 제공한다．

  · 마우스 press, move, release 그리고 double click을 제공한다. 뿐만 아니라 마우스 Wheel 이벤
   트와 hover 이벤트를 지원하고 마우스가 위치한 곳에 context menu 이벤트를 사용할 수 있다．
  · 키보드 입력 이벤트와 Key 이벤트를 제공한다．
  · 드래그（Drag）와 드랍（Drop) 기능을 지원한다．
  ·Parei此와 Child의 Relationships 그룹 기능을 지원한다（QGraphicsltemGroup).
  ·Collision detection 기능을 지원한다．

QGraphicsView와 같이 아이템은 Local 좌표 시스템을 사용한다. 또한 아이템과 scene 사이에 좌표를
八4appii培하기 위한 많은 함수를 제공한다. 만약 Matr奴를 사용한다면 아이템의 위치를 이동／회전 등의
기능을 사용할 수 있다．




                                                               Li
                                                                            口
                                                                    ]




                                                               pc'
                                                     '   ""뇨   .




                                                                            1!
                                                                            ]
                  口
                                     ACith p4 ten,
                                                                            1
                                     Wrh 小41er1r出＄
                       1             'C캬1 1 出야｝m J




                      1
                                     M 蒸丘：     苾


                                                                        /
                                      川ef a h끼

                                                           1   (,
                  \\   7            나1

（그림） OGra아기C引tern 클래스의 Shape




228 CHAPTER 07느 그래픽스


===== PAGE 230 =====
아이템은 Child 아이템 개넘과 같이 특정 아이템들이 하나의 아이템에 Grouping 될 수 있다. 이러한
Grouping 기능은 Child로 Groupir乷된 아이템들을 일괄적으로 변형시키거나 이동시킬 수 있다. 아이
템을 Groupir培하기 위해 QGraphicsltem의 contains( ) 함수와 boundingRect( ) 함수 그리고
coll姓esW此h( ) 함수를 사용할 수 있다. QGraphicsltem 클래스는 shape( ) 함수를 통해 Collision
Detection 기능을 지원한다.

클래스                              설명
QGraphicsEffect                  모든 그래픽 타旭아의 부모 클래스
QGraphicsAnchorLayout            Gra아기cs View에서 위젯들을 배치하기 위한 Layout을 제공
QGraphicsAnchor                  QGra아iicsAnchorLayo미에서 아이템 사이의 Anchor（공백 등）를 표현
QGrap비csGridLayout               Graph心 피ew에서 위젯을 관리하기 위한 Grid 기반의 Layout
OGra아기csltem                     I OGra口hicsScene에서 모든 그래픽 아이템의 부모 클래스
OGraphic없珣ect                    모든 그래픽 아이템의 시그널, 슬롯 그리고 프로퍼티의 부모 클래스
QAbstractGraphicsShapeltem       모든 Path 아이템을 위한 공통 부모 클래스
OGrapt기csPathltern               QGrap볘弱Scene에 추가할 수 있는 Path 아이템 클래스
QGraphicsRectltem                QGra아기csScene에 추가할 수 있는 Rec伯n이e 아이템 클래스
QGra아icsEIIipseltem              QGraphicsScene에 추가할 수 있는 Elli口se 아이템 클래스
QGraphicsP이ygo톄怡m                 QGraphicsScene에 추가할 수 있는 P이ygon 아이템 클래스
OGra아기Cs니n레em                     QG田p볘csScene에 추가할 수 있는 Line 아이템 클래스
QGraphi四미xrn햐川em                  QGraphicsScene에 추가할 수 있는 Pixmap 아이템 클래스
QG떠p비csTextltern                  텍스트를 화면에 출력하기 위해 QGraphicsScene에 추가할 수 있는 Text 아이템 클래스
QGrap비csSim이eTextitem             QGraphicsScene에 추가할 수 있는 Simple test 아이템 클래스
QGra아）允sltemGro바1                 아이템을 그룹으로 처리할 수 있는 Container 클래스
QGraphicsltemAnim帥on              QGraphic引tern을 위한 단순한 애니메이션 기능을 지원하기 위한 클래스
OGra아기csLayout                    Graphics View 상에서 모든 Layout의 부모 클래스
OGrap비csLayoutltern               사용자 정의 아이템이 Layout (게 의하1 관리할 수 있도록 상속할 수 있는 클래스
OGra아iCs니nearLayout               Gra아）允S View에서 위젯을 관리하기 위한 Horizontal(수평） 혹은 Vertical Layout
QGra아기csProxyWidget               QGraphicsScene에서 a小써get을 내장하71 위한 Proxy Layer
QGra아iicsScene                    많은 2D 그래픽 아이템을 관리하기 위한 Surface
QGraphicsSceneEvent               이벤트와 관련된 모든 Gra아. iCs 너ew를 위한 부모 클래스
0（카aphicsSceneMouseEvent         （計a아）匕s view framework에서 마우스 이벤트 클래스
OGra아icsSceneWheelEvent           Graphics view framework에서 마우스 Whe이 이벤트 클래스
QGraphicsSceneContextMenuEvent    Gra아ics view frarnewo水에서 마우스 Context menu 이벤트 클래스
QGraphicsSceneHoverEvent          Gra口hics 피e小／ 什amework에서 Hover 이벤트 클래스
QGraphicsSceneHelpEvent           Toolti口 기능이 필요할 때 사용되는 이벤트 클래스
QGra아iicsSceneDragDropEvent       Graphics view 什arnewo水에서 마우스 먀ag와 Dro口 이벤트 클래스
oGraphicsSceneResizeEvent        （計aphics ＼기ew framework에서 위젯 크:7롤 변경하21 위한 이벤트 클래스
0Gra하iicsSceneMoveEvent           Gra하ics view framewo水에서 위젯 이동을 위한 이벤트 클래스
OGra이기csTranstorrn                QGraphicsltem을 변형시키거나 이동시키기 위한 부모 클래스
OGra이기csView                      QGra이기csScene의 모든 객체를 표시하기 위한 위젯 클래스
QGraphicsWi均et                    QGra아기csScene에서 모든 위젯 아이템의 부모 클래스
OSt니eQ이山m針러出吃sitem                OGrap볘四Item을 그리21 위해 필요한 파라미터를 서술하기 위해 사용




                                                                    乙Gr叩hics View 다amework 229


===== PAGE 231 =====
     2.2 Gra아기cs View의 좌표
Graphics View는 교차하는 축에 태한 위치어］ 의해서 위치가 결정되어 있는 2차원 혹은 3차원 상의 위
치인 데카르트 좌표（Cartesian coordinate）를 사용한다. x축（가로축）,Y축（세로축） 두 개의 좌표를 이
용하며 위치를 표시한다．

Graphics View에는 Item 좌표, scene 좌표 그리고 \／扼w 좌표를 사용한다. 언급한 3개의 좌표를 사용
하기 위해 Graphics View는 편리한 함수를 제공한다. 그래픽 요소들이 표시될 때 Graphics View 좌
표는 QPainter의 논리적인 좌표와 일치한다. 논리적인 좌표와 디바이스의 좌표 사이의 관계와 관련해
정보를 얻어올 수 있다．




（그림）（計aphics View의 좌표



1 아이템의 좌표
각 Item은 자신의 좌표를 가지고 있다. 이러한 좌표는 0,0 위가 중심이다. 이러한 좌표는 모든 움직일 때
중심 좌표（0,0）가 중심이 된다. 사용자 정의 Item을 생성할 때와 QGraphicsScene과 QGraphicsView
상에 이동과 변형이 일어날 때 Item 좌표어］ 대해 고려해야 한다. 예를 들어 마우스 클릭과 드래그 이벤트
로 인해 Item의 좌표가 변할 수 있다．

QGraphicsltem 클래스의 contains( ) 함수는 Item 안으로 이동할 경우 유효한 좌표면 True를 리턴한
다. 반대로 False인 경우는 아이템의 좌표 안에 아이템이 Boundii培되지 않은 상태를 말한다. 아이템의
좌표는 부모 좌표의 중심 좌표를 기반으로 사용한다．


0scene 좌표
scene은 모든 Item 좌표의 중심（0,0）이 된다. 가장 상위 레벨에 있는 아이템은 scene 좌표를 참조한다．
또한 view로부터 모든 scene을 이동하기 위한 좌표로 사용한다. scene은 좌표와 Boun恤培된 사각형 영
역을 가지고 있다. scene의 위치는 scenePos( ) 함수를 통해 얻어올 수 있으며 sceneBoundingRect()
함수를 사용해 사각형 영역의 정보를 얻어올 수 있다．


1 니ew 좌표
View 좌표는 위젯의 좌표이다. 각 Un仇은 \[jew어］ 포함되고 하나의 픽셀과 일치한다. 그리고 View 좌표
는 위젯, 叭ewport와 view에 포함된 scene과 밀접한 관련이 있다. 가장 상위의 위치와 왼쪽이 좌표의


230 CHAPTER 07_ 그래픽스


===== PAGE 232 =====
중심（0,0）이 된다. View 포트의 가장 아래와 오른쪽은 叭ewport의 width와 height가 된다. 모든 마우
스 이벤트는 \[jew 좌표와 관련이 있다．


. 좌표 Mapping
scene에서 Item을 다룰 때 아이템을 좌표로 아이템 안의 좌표상에 아이템을 배치할 때 유용하다. 예를
들어 QGraphicsView의 \Tiewport 안에서 마우스를 클릭할 때 즉, 아이템이 속한 scene을 요구할 때
mapToScene( ) 함수를 사용할 수 있다. mapToScene( ) 함수는 scene 좌표에서 Mapping된
viewport 좌표를 리턴한다. 만약 viewport 상에 위치한 Item을 얻고자 한다면 itemAt( ) 함수를 사용
할 수 있다．



      f H . Graphics View의 주요 특징
S 확대／축소와 회전
Affine transformation은 도형이나 이미지를 그릴 때 Ve毗아를 이용해 변화를 주는 것을 의미한다. 변
화의 성질은 Translate, Scale, Rotate가 있다. QGraphicsView는 setMatrix( ) 함수를 통해 QPain
  ter와 같이 Affine transformation을 지원한다．

View에서 변형（Tran計아m毗珀n）을 적용한다면 확대／축소（Zooming), 회전（r毗毗ion）과 같은 기능을
쉽게 사용할 수 있다. 아래 예제는 QGrap址csView 클래스를 상속받은 클래스에서 구현한 예제이다．

class View :public   QGraphicsView
{
Q OBJECT

public slots:
    void zoomln() { scale(1. 2, 1. 2) ; }
    void zoomOut () { scale(1 I 1.2, 1 I 1. 2) ; }
    void rotateLeft () { rotate(-10) ; }
    void rotateRight () { rotate(10) ; }


 };
S QPrinter를 이용한 출력
Graphics View는 QGraphicsV扼w 클래스의 render( ) 함수와 GraphicsScene 클래스의 render( )
함수를 통해 출력 기능을 제공한다. 이 API는 동일한 기능이며 다른 Paint device로 QPainter 클래스
를 통해 렌더링 할 수 있다. QPrinter 상에 QPair式er를 이용해 드로잉이 가능하다．




                                                     乙Gr叩hics ＼기ew 다amewc玎K   231


===== PAGE 233 =====
QGraphicsScene scene;
scene. addRect (QRectF (0, 0, 100, 200) , QPen(Qt: :black) , QBrush (Qt: :green) );


QPrinter printer;
if (QPrintoialog(&printer) .exec () == QDialog: :Accepted) {
    QPainter painter (&printer) ;
    painter. setRenderHint (QPainter: :Antialiasing) ;
    scene. render ( &painter) ;




scene과 V扼w의 기능 중 차이점은 사용하는 좌표가 scene 좌표 혹은 V扼w 좌표를 사용한다．
QGraphicsScene 클래스의 render( ) 함수는 전체 중에 scene의 일부분을 printii培하기 위해 사용된
다. 다른 하나인 可柯aphicsView 클래스의 render( ) 함수는 전체를 Screen Sh毗을 가져오기 위해 사
용된다．

QGraphicsScene scene;
scene.addRect (QRectF(0, 0, 100, 200) , QPen(Qt: :black) , QBrush(Qt: :green) );


QPi沁nap pixmap;
QPainter painter (&pixmap) ;
painter. setRenderHint (QPainter: :Antialiasing) ;
scene. render ( &painter) ;
painter.end() ;


pixmap. save ( "scene.png") ;



S［가ag와 Drop
QGraphicsView 클래스는 QWidget을 간접적으로 상속받았다. 따라서 邸Widget에서 제공하는 Drag
와 Drop을 QGraphicsView에서 쉽게 추가하1 사용할 수 있다. Graphics View Framework는 scene
과 각각의 모든 Item에서 Drag와 Drop을 지원한다. 즉 Drag와 Drop을 이용한 변환을 위해
QGraphicsSceneDragDropEvent 클래스를 사용할 수 있다．

Item을 마우스로 드래그하기 위해 QDrag 오브젝트를 생성한다. 드래그를 시작한 위젯에서 포인터를 반
환한다. Item은 동시에 여러 \hiew를 관찰할 수 있다. 하지만 단지 마우스를 움직이거나 버튼을 누르는
것과 같이 시작되는 하나의 View에서 Drag와 Drop을 처리할 수 있다．

void Customltem: :mousePressEvent ( QGraphicsSceneMouseEvent *event)
 {
     QMimeData *data = new QMimeData;
     data->setColor (Qt: :green) ;


     QDrag *drag = new QDrag(event->widget () );
     drag->setMimeData (data) ;
     drag->start () ;
 }


232 CHAPTER 07_ 그래픽스


===== PAGE 234 =====
0Cursor오F Tooltip
QWidget, QGraphicsltem 클래스와 같이 QGraphicsltem 클래스의 setCursor( ) 함수를 사용하면
Cursor를 지원한다. 그리고 setToolTip( ) 함수를 사용하면 Tooltip 기능을 사용할 수 있다. 만약 마우
스 커서가 Item의 영역어］ 들어가는 것과 같이 QGraphicsView에 의해 （뇨rsor와 Toolt巾을 활성화한
다. View 상에서 setCursor( ) 함수를 호출하면 디폴트 커서를 설정할 수 있다．


0Animation
Graphics View는 Anim毗ion을 지원한다. Animation Framework를 사용해 Animation을 적용할
수 있다. QGraphics아力ect 클래스로부터 상속받은 Item을 QPropertyAnimation으로 연결해1 사용할
수 있다. QPropertyAnimation은 QObject 프로피티를 애니메이션 기능 추가가 가능하다．


0OpenG[ 렌더링
QGraphicsView 클래스의 setViewport( ) 함수를 호출에 의해 QGraphicsView의 叭ewport와 같이
QGLWidget어］ OpenGL 상에 렌더링할 수 있다. OpenGL에 Antialiasing을 사용하길 원한다면
sample buffer를 사용할 수 있다．

QGraphicsView view (& scene) ;
view. setViewport (new QGLWidget (QGLFormat (QGL: :SampleBuffers) ));


0Item 그룹
다른 Child Item들을 하나의 Item으로 만들 수 있다. Item의 그룹은 가장 필수적인 기능이며 그룹화된
Item은 함께 이동（Move）할 수 있다. 그룹화 기능은 QGraphicsltemGr이叩을 사용해 Item을 그룹화
할 수 있다．


lWic杓et과 Layout
QGraphicsWidget을 통해 Item들을 배치하고 레이아웃을 위한 기능을 지원한다. 이것은 QWidget과
비슷하지만 QWidget과 동일하지는 않다. QGraphicsWidget은 QPaintDevice로부터 상속되지 않
는다．


           이벤트 처리

QGraphicsView는 마우스, 키보드, 터치 등과 같은 이벤트 처리가 가능하며 이벤트를 담당하는 QGra-
phicsScene 클래스를 이용하면 사용자 이벤트를 처리할 수 있다．

void rnousePressEvent (QGraphicsSceneNouseEvent *event) ;
void mouseReleaseEvent (QGraphicsSceneMouseEvent *event) ;
void mouseMoveEvent (QGraphicsSceneMouseEvent *event) ;
void mouseDoubleClickEvent (QGraphicsSceneMouseEvent * event) ;




                                                                 2_Graphics View Framework 233


===== PAGE 235 =====
QGraphicsView에서 마우스 이벤트 처리를 위해 QGraphicsSceneMouseEvent 클래스를 제공하며
可｝raphicsView에서만 사용이 가능하다．

 void Myltem: :mousePressEvent (QGraphicsSceneMouseEvent *event) {
      qDebug( "Mouse button clicked") ;
 }

 void Myltem: :mouseReleaseEvent (QGraphicsSceneMouseEvent *event) {
      qDebug( "Mouse released clicked") ;
 }

 void Myltem: :mouseMoveEvent (QGraphicsSceneMouseEvent *event) {
      qDebug( "Mouse move") ;
 }

 void Myltem: :mouseDoubleClickEvent (QGraphicsSceneMouseEvent *event) {
      qDebug ( "Mouse double clicked") ;




mousePressEvent( ）는 마우스가 눌러질 때 발생하는 이벤트이며, mouseReleaseEvent(）는 마우스가
눌러진 상태가 해제되었을 때 발생하는 이벤트이다. mouse卜iloveEvent( ) 이벤트는 마우스가 눌러진 상
태에서 좌표가 변경되면 이벤트가 발생하며 , mouseDoubleClickEvent( ) 이벤트 함수는 마우스를
Double Click했을 때 발생한다．

 void keyPressEvent (QKeyEvent *event) ;
 void keyReleaseEvent (QKeyEvent *event) ;




（카aphi出加畦陀nt 口

Starting D: \Qt5\ Graphi그
Desktop Qt 5 0 0 MSVC20t
Mouse bu亡亡on clicked
Mouse released clicked ;
Mouse but乞口n clicked      三
Mouse released clicked




（그림） Gra아기Cs ＼기ew 이벤트 처리



키보드 이벤트를 처리하기 위해 keyPressEvent( ）와 keyReleaseEvent( ) 함수를 사용할 수 있다．




234 CHAPTER 07_ 그래픽스


===== PAGE 236 =====
哮t흩互 사용자 정의 QGraphicsltem
이번 장에서는 QGraphicsltem을 이용해 사용자 정의 아이템을 구현해 보도록 하자. 구현할 사용자 정
의 QGraphicsltem은 QPushButton과 같이 마우스 이벤트가 발생하면 버튼이 클릭된 이미지로 변경되
도록 페인트를 이용해 구현해 보도록 하자．

파일                   설명
CustomItem. h        사용자 정의 QGraph七읽也rn 헤더 파일
Customltem.cpp       사용자 정의 QGraph七引tern 소스 파일
rnain.cpp            프로그램 메인 소스 파일


표에서 보는 것과 같이 헤더 파일과 소스 파일을 생성하고 Customltem.h 파일어］ 다음과 같이 소스 코
드를 작성한다．

#include <QGraphicsltem>
#include <QObject>
#include <QPainter>
#include <QGraphicsSceneMouseEvent>


class Customltem : public QObject, public Qcraphicsltem
{
     Q OBJECT
     Q INTERFACES (QGraphicsItem)

public:
     Customltem(QGraphicsltem *parent = 0) ;
     Customltem(const QString normal,
                       const QString pressed = " ", QGraphicsltem *parent = 0) ;


     // 페인트 영역
     QRectF boundingRect ( ) const;


     // 버튼 이미지를 렌더링하기 위한 함수
     void paint (QPain七er 枉沮in七er,
                 const QStyleOptionGraphicsltem *option,
                 Qwidget; 火widge七 = 0) ;


     // 이미지 로딩
     void setPixmap(const QString normal,
                      const QString pressed = H n ) ;


signals:
     void clicked( ) ; // 시그널

protected:
     /／이벤트
     void mousePressEvent (QGraphicsSceneMouseEvent *event) ;
     void mouseMoveEvent (QGraphicsSceneMouseEvent *event) ;
     void mouseReleaseEvent (QGraphicsSceneMouseEvent *event) ;                            O

                                                                  2_Graphics View Framework 235


===== PAGE 237 =====
private:
      QPixmap in끄（Drmal;     // 버튼 이미지
      QPixmap rn_pressed; // 버튼이 눌러진 상태 이미지
      bool m isPressed; // 버튼이 클릭된 상태인지 확인하기 위한 변수
 };


Q_INTERFACES(QGraphicsltem)는 구현할 클래스가 어떤 인터페이스로 구성되었는지 알리기 위한
매크로이다. 생성자에서는 이미지를 로딩하는 클래스의 setPixmap( ) 멤버함수를 호출한다．

Customltem: :Customltern(const QString normal,
                             const QString pressed,
                             QGraphicsItem *parent)
                      : QGraphicsltern(parent) , misPressed(false)


      setPixmap(normal, pressed) ;




setP奴map( ) 함수는 Private 멤버로 선언한 QPixmap 인스턴스를 초기화하고 지정한 버튼 이미지 파
일을 QPixmap 인스턴스어j 저장한다．

void Customltem: :setPixmap(QString normal, QString pressed)
 {
      if   (! mnornial.isNull () )
       {
       1
           rn normal.detach() ;
           rn_pressed.detach() ;
      }

      rn_normal, load (normal) ;
      n_pressed. load(pressed) ;
 }


QPixmap 클래스의 detach( ) 멤버함수는 QPixmap 인스턴스에 공유된 p奴map 데이터를 제거하기 위
해 사용하는 멤버함수이며, load( ）는 함수로 넘겨 받은 파일명을 QPixmap 인스턴스어］ 저장하기 위한
QPixmap 클래스의 멤버함수이다．

void Customltern: :mousePressEvent (QGraphicsSceneMouseEvent *event)
{
      if   (event->bu七ton( ) == Qt: :Lef七Bu七七on)
      {
           if   (contains (event->pos () ))
                m isPressed = true;


           update ( ) ;
      }



236 CHAPTER 07... 그래픽스


===== PAGE 238 =====
마우스 오른쪽 버튼이 클릭된 상태일 때 발생하는 이벤트로써 bool 타입의 rn_i sPressed 변수는 true 값
을 저장하고 update( ) 함수를 호출한다. update( ) 함수를 호출하면 구현할 paint( ) 함수가 호출된다．

void Customltem: :paint (QPainter *painter,
               const QStyleoptioncraphicsltem *option, QWidget *widget)
 {
     QUNUSED（아此如n) ;
     QU]寸口SED(widget) ;


     if   (m isPressed)
         painter->drawPi刃nap(O, 0, rn_pressed) ;
     else
          painter->drawPixmap(O, 0, rn_normal) ;
 }


update( ) 함수를 호출하면 Mappii培된 paint( ) 함수를 호출한다. paint( ) 함수에서는 QPixmap에 저
장된 이미지를 QGraphicsScene에 렌더링한다. m isPressed 변수가 true이면 마우스가 눌러진 상태
를 표시하는 이미지를 렌더링한다．


void Customltem: :rnouseReleaseEvent (QGraphicsSceneMouseEvent *event)
 {
     if   (event->button() == Qt: :LeftButton) {
           m isPressed = false;
           update() ;


          if   (contains (event->pos () ))
                emit clicked( );
     }
 }




（그림） 사용자 정의 OGra口hicsltem 실행 화면



mouseReleaseEvent( ）는 마우스가 눌러진 상태가 해제되는 이벤트이며 , update( ) 함수를 호출해 매
핑된 paint( ) 함수를 실행한다. 그리고 헤더 파일에서 선언한 clicked( ) 시그널 emit을 통해 이벤트가
발생한다．



                                                              之아a아)iCS View 다amework 237


===== PAGE 239 =====
                  QGra아기csE卄ect
이번 장에서는 QGraphicsEffect를 이용해 렌더링 그래픽 요소에 Blur, DropShadow, Colorize,
Opacity Effect를 사용해 그래픽 효과를 사용하는 방법에 대해 알아보도록 하자．

QGraphicsEffect는 모든 Effect 클래스의 부모 클래스이다. 원본 이미지와 최종으로 이미지를 출력하
는 디바이스（예를 들어 QGraphicsView의 Viewport) 사이의 렌더링 파이프라인을 Hookit瑠하여 효과
(Effect）를 사용한다．

그리고 QGraphicsltem에 효과를 추가하기 위해 다음과 같은 효과 중 하나를 선택해 사용할 수 있으며
QPai砒er를 이용한 드로잉 , QGraphicsView Viewport 상에 렌더링 한 QGraphicsltem에서 효과를
사용할 수 있다．

                                      원본사진




    Blur Effect       Drop Shadow Effect     Colorize Effect   Opacity Effect
     흐림효과                 그림자효과               색상변환효과             투명효과




（그림） 원본 사진과 타m아를 적용한 사진



Etfect                             설명
QGraphicsBlurEffect                흐림 효과
QGraphicsDropShadowEftect          그림자 효과
QGraphicsColorizeEffect            tint를 사용한 C이orize 효과
O아톄가기cs야冶레yE卄ect                   투명 효과




0QGraphicsBlurEffect
Blur Effect는 흐림 효과로 정의할 수 있으며 이미지나 도형이 렌더링 되는 영역을 흐리게 할 수 있다．
Blur Effect는 포커스가 아웃 포커싱 효과를 사용하고자 할 때 유용하다．

렌더링 할 이미지나 도형에 Blur Effect는 디폴트로 5 픽셀 값이 설정되어 있으며 , setBlurRadius()
멤버함수를 이용해 Blur Effect의 레벨을 조절할 수 있고, Blur 힌트를 선택하기 위해 setBlurHints( )
멤버함수를 사용할 수 있다．


238 CHAPTER 07_ 그래픽스


===== PAGE 240 =====
 QPixrnap pi刃nap ( " :/resources/lena.png") ;
 QcraphicsPixrnapltern *bg = rn scene.addPixrnap (pixrnap) ;
bg->setParentltern( parent) ;
bg->setZValue(1) ;


rn_effect = new QGraphicsBlurEffect;
也effec七->se七BlurRadi꾜s (10) ; // 흐림 효과 레벨
rn effect- >setEnabled (true) ;
parent->setGraphicsEffect (rn effect) ;



                                                               쁜뼈
                                     쯔 QGr캬m<5E




（그림） 원본 실행 화면과 Blur Ef伯ci를 사용한 실행 화면



0QGraphicsDropShadowEffect
Dr아） Shadow Effect는 그림자 효과를 표현하기 위한 Effect이다. setColor( ）는 그림자의 컬러를 설
정하기 위한 멤버함수이며 첫 번째 인자로 QC아or를 지정할 수 있다．

setBlurRadius( ) 멤버함수는 그림자 효과가 표시되는 영역에 투명 효과를 설정할 수 있으며 설정하지
않은 경우 디폴트 값은 1로 설정된다. setOffset( ) 멤버함수는 그림자가 표시되는 크기와 방향을 설정할
수 있으며 인자로 x좌표 값과 Y좌표 값을 설정할 수 있다．

x좌표의 값이 양수이면 오른쪽 방향으로 그림자가 표시되고, 음수이면 왼쪽 방향으로 그림자가 설정된
다. 또한 Y좌표의 값이 양수이면 아래 방향, 음수이면 위 방향으로 그림자가 표시된다．

 QGraphicsRectltern *parent = rn scene.addRect (O, 0, 700, 360) ;
 parent->setPen(Qt: :NoPen) ;
 parent->setZValue ( 0) ;


 QGraphicsPixrnapltem *bg[ 7] ;
 qreal x = 40. 0, y = 30. 0;


 for (int i   = 0, j = 0 ; i < 7 ; i++, j++)
 {
     bg[ i]   = rn scene.addPi刃nap (QPixrnap ( " :/resources/lena.png") );
     bg[ i卜＞se七Paren七I七ern(paren七）; // 부모 그래픽스 뷰 아이템 지정                                     0

                                                                      乙아a아iics View 다amework 239


===== PAGE 241 =====
    bg [ i卜＞moveBy (x, y) ; // 좌표 설정
    bg[ i ] ->se七ZVa1끄e(1 ) ;

     x += 160;

     if (i == 3) {
          x = 200;
          y 十＝ 170;
     }
}
rn.Heffect[ 0] = new QGraphicsDropShadowEffect;
// 民G,B, Alpha - Alpha값을 지정하지 않으면 1로 설정
m1effect[ 0] ->setColor (QColor (63, 63, 63, 180) );
bg[ 1] ->se七GraphicsEffec七（rn_effec七［0] ); /7 Drop Shadow Effect를 지정할 아이템

rn_effect[ 1] = new QGraphicsDropShadowEffect;
rn effect[ 1]수setColor (QColor (63, 63, 63, 180) );
// 그림자 영역 투명 효과 설정, 사용하지 않으면 디폴트 값 1이 설정됨
rn-1effect[ 1] ->setBlurRadius (15. 0) ;
IT느effec七［1] ->se七丑nabled( 七rue) ;
bg [2 ] ->setGraphicsEffect (rn_effect [1] );

rn effect[ 2] = new QGraphicsDropShadowEffect;
rn effect[ 2] ->setColor (QColor (63, 63, 63, 180) );
rn_effect [2] ->setBlurRadius ( 15. 0) ;
// 그림자가 표시될 방향, X7f 양수이면 오른쪽, 음수이면 왼쪽, Y 'F 양수이면 아래， 음수이면 위쪽
 // 지정하지 않으면 디폴트 값 X=8, Y=8
IT느effect[ 2］少＞se七Offse七（20, 20) ;
rn.meffect[ 1] ->setEnabled(true) ;
bg[ 3] ->setGraphicsEffect (rneffect[ 2] );

m_effect[ 3] = new QGraphicsDropShadowEffect;
rn-1effect[ 3] ->setColor (QColor (63, 63, 63, 180) );
rn effect[ 3卜>setBlurRadius ( 15. 0) ;
rn-4effect[ 3] ->setOffset (- 20, 20) ;
IT느effec七 [ 1] ->se七Enabled(true) ;
bg [4 ]->setGraphicsEffect (rn_effect [3] );

rn-1effect[ 4] = new QGraphicsDropShadowEffect;
rn'effect[ 4} ->setColor (QColor (63, 63, 63, 180) );
rn_effect [4] ->setBlurRadius (15. 0) ;
rn-eeffect[ 4] ->setOffset (- 20, -20) ;
mjffe （北 [ 1卜＞se七Enabled (true) ;
bg[ 5] ->setGraphicsEffect (rn effect[ 4] );

rn effect[ 5] = new QGraphicsDropShadowEffect;
rn effect[ 5] ->setColor (QColor (63, 63, 63, 180) );
rn effect [5] ->setBlurRadius ( 15. 0) ;
rn 4effect[ 5] ->setOffset (20, -20) ;
rn_effect [ 1] ->setEnabled( true) ;
bg[ 6] ->setGraphicsEffect (rn_effect[ 5} );



240 CHAPTER 07_ 그래픽스


===== PAGE 242 =====
 ij QGraphicsE ec                                     小 呻m




                    U
（그림） OGraphics［가opShadowEf厄아를 사용한 예제



0QGra아기csC이아注eE卄ect
Colorize Effect는 C아or 값의 tint를 사용해 원본 이미지를 렌더링하는 효과이며 setC아or( ) 멤버함수
를 이용해 Effect를 사용할 수 있다．

 rn_effect = new QGraphicsColorizeEffect;
 rn'effect- >setColor (QColor (O, 0, 192) ); II RGB의 LIGHT BLUE


 rn_effect->setStrength( 1) ;
 m'effect- >setEnabled (true) ;


 parent->setGraphicsEffect (rn_effect) ;



                                  ri1Q3,aFh口寸E:t




（그림） 원본과 C이orized Effect




                                                                  乙（針a아ics View 다amewo가（ 241


===== PAGE 243 =====
1QGraphicsOpacityEffect
Opacity Effect는 투명 효과를 사용해 이미지 혹은 도형을 렌더링 할 수 있다. Effect를 사용하기 위해
setOpacity( ) 멤버함수를 사용할 수 있으며 디폴트로 0.7값이 설정되어 있다. set야垠ci打로 투명 효과
를 사용하는 범위는 0. 小1.0 값의 범위를 사용할 수 있다．


 rn_effect = new oGraphics0pacityEffect;
 rn_effec七->se七0pa（그j土y (0.3) ; // 투명 효과 범위 설정 값
 rn小effect->setEnabled(true) ;
 parent->setGraphicsEffect (rn_effect) ;




（그림） 원본과 Opac啣 Effect




242 CHAPTER 07_ 그래픽스


===== PAGE 244 =====
（그t5 Pr（그gramming




             3 Qt OpenGL 모듈을 이용한
               3D 그래픽
             OpenGL과 OpenGL ES를 이용하I 3D 그래픽스를 사용하기 위하1 아에서 제공하는 AP뻬 대해 살펴
             본다．




OpenGL은 1992년 실리콘 그래픽스에서 개발한 3D 그래픽 표준 API이며 약 250개의 함수를 제공한다．
 기초적인 기하도형에서 복잡한 3D 그래픽스를 표현할 수 있다. OpenGL은 311) 그래픽이 필요한 3D 가
상 모델링 시뮬레이션, 게임 , 네트워크 Traffic 시각화, 건축설계 등 다양한 분야에서 널리 활용되고 있
다. OpenGL은 두 가지로 분류된다．

 종류                 설명
 Open（孔             긔쿠누人 그룹이 정의한 3D 그래픽스 표준 API
 O口enGL ES          임베디드 시스템과 같이 자원0I 제한된 개발환경에서 3D 그래픽스를 사용하71 위
                    해 사용된다. 예를 들어 M야川e, Tablet, SmartTV 등과 같은 임베디드 디바이스
                    환경에서 작은 메모리 자원에서 동작할 수 있도록 명령의 수나 동작에 필요한 메
                    모리 소모량을 줄인 경량의 버전이다. ES는 Embedded Sys也m의 약자이다．


 Qt를 사용해 OpenGL 기반 3D 그래픽스 어플리케이션을 개발하기 위해서 QGLWidget을 사용할 수 있
다. 또한 임베디드 리눅스상에서도 별도의 수정작업 없이 QGLWidget을 사용해 3D 그래픽스 어플리케
 이션을 개발할 수 있다. 八'IS윈도우, Mac OS X 플랫폼 등 다양한 플랫폼에서 QGLWidget을 사용해
 OpenGL 기반의 어플리케이션 개발이 가능하다．

 Qt에서 제공하는 OpenGL 모듈을 사용하여 3D 그래픽스 어플리케이션을 개발 시, OpenGL을 쉽게 구
 현할 수 있도록 QGLWidget을 제공한다. 또한 QPaii此er를 이용한 2D 그래픽을 렌더링하기 위해
 QGLWidget을 Mappii培할 수 있다．
       A口口妃ation 化r2D Graphics
                                                 A口口i出at幻n 幻r3D 白a口tiics
           U여ng OPainter
                                  QGLWidget Class
                    口月尸／(0(2口／3D Gra例放？S ｛好加口 丑7 口店口加CS 日C口e旭／旨／口r

 ＆切口月以10力era加7口 旬썲旬77

   Embedded Linux MS Windows Mac OS x            텨ackberry    Sym bian    QNX

  月뇨侄卉V日／口
                    CPU     Memo斗     S的rage            3D Graphics Accelerator

（그림） HW 3D Gra아iics Acc이아졔아를 활용한 2D/3D 그래픽 어폴리케이션 구조


                                                                         {（가 OpenGL 모듈을 이용한 3D 그래픽 243


===== PAGE 245 =====
이는 2D 그래픽을 OpenGL 기반 렌더링을 사용하기 위해 HW에서 제공하는 3D 가속기 모듈（3D
Graphics HW Accelera的r）을 사용하므로 CPU와 같은 자원을 절약할 수 있다. 또한 임베디드 디바이
스와 같은 제한된 자원에서 HW3D 가속기 모듈을 사용하므로 Anim毗ion Framework, QGrap-
hicsEffect, QGraphicsView 등 풍부한 UX(User Experience）를 설계할 수 있다．

Qt에서 Qt OpenGL 모듈을 사용하기 위해서는 qmake 프로젝트（.pro) 파일어］ "opengi" 을 추가한다．

QT += opengi



소스 파일어］ QtOpenGL을 include 하기 위해 다음과 같이 추가한다．

#include <QtOpenGL>


S （값 OpenGL 클래스

종류             설명
QGLW,dget      OpenGL 그래픽을 렌더링하기 위한 위젯
QGLFormat      OpenGL 롄더링 conte았의 포맷 디스플레이를 지정
QGLContext     OpenGL 렌더링 context 캡슐화 클래스



S QGLWidget
QGLWidget은 Qt 어플리케이션에 OpenGL 그래픽을 통합하여 화면상에 3D 그래픽을 렌더링하기 위
해 제공한다. 사용하기 매우 쉽게 구현되어 있다. 帥Widget 클래스가 부모 클래스이다. 따라서 QGL
Widget 클래스에서 QPainter를 사용해 2D 그래픽을 함께 사용할 수 있다．


0QGLFormat
QGLFormat 클래스는 Double 혹은 Single Buffer, Depth buffer, RGBA(or color) index mode
등 OpenGL 렌더링 context의 디스플레이 포맷을 지정할 수 있는 기능을 제공한다．

QGLFormat fmt;
fmt. setDoubleBuffer (false) ;              II single buffer
fmt. setDirectRendering (false) ;           II software rendering



0QGLContext
QGLContext는 OpenGL 렌더링 context를 캡슐화된 클래스이다. 렌더링 context의 포맷은 클래스 생
성자에서 설정할 수 있다. 또한 생성자에서 설정하지 않더라도 setFormat( ) 함수를 사용해 추후
context의 포맷을 설정할 수 있다．




244 CHAPTER 07_ 그래픽스


===== PAGE 246 =====
             3D 그래픽 렌더링을 위한 QG네Vidget 클래스

QGLWidget은 Qt 어플리케이션에 0penGL 그래픽 기능을 추가하기 위해 제공하는 클래스이다. 사용하
기 쉽게 구현되어 있다. QGLWidget은 QWidget 클래스를 상속받았으며 QPainter를 사용할 수 있다．
QGLWidget은 일반적인 0penGL 프로그래밍 구조를 편리하게 구현할 수 있도록 다음과 같은 3개의
Virtual 함수를 제공한다．


DpaintGL( )
0penGL scene을 렌더링한다. 위젯（QGLWidget）의 업데이트가 필요하면 호출된다．


0resizeGL( )
0penGL의 viewport, project 등을 설정한다. 위젯의 크기가 변경（resize）될 때 자동으로 호출하며 위
젯（QGLWidget）이 처음 실행될 때 resize 이벤트가 자동으로 호출된다．


S initializeGL( )
0penGL 렌더링 context를 설정한다. resizeGLO, paintGL( ) 함수가 호출되기 전 최초 한번만 호출
된다．

class MyGLDrawer : public QGLWidget
 {
      Q OBJECT         // 시그널 슬롯을 사용하면 항상 포함

public:
      MyGLDrawer ( Qwid.get; 枉冶ren七）
          : QGL'寸idge七（paren七） {}

pro七ec七ed:


      void initializeGL ( )
      {
          7/ Set up the rendering context, define display lists   etc. :


          glClearColor (O. 0, 0.0, 0.0, 0.0) ;
          glEnable(GL_DEPTH TEST) ;


      }

      void resizeGL (int w, mnt h)
      {
          // setup viewi均r七rprojec七ion e七C. :
          glViewport (0, 0, (GLint)w, (GLint)h) ;

          glFrustum(. ..);
                                                                                    O


                                                        3 (코 C）口enGL 모듈을 이용한 3D 그래픽 245


===== PAGE 247 =====
      }

     void paintGL (      )
      {
           /7 draw the scene:


           glRotatef (. ..);
           glaaterialfv (. ..);
           glBegin(GL_QUADS) ;
           g1Vertex3f (. ..);
           g1Vertex3f (. ..);


           glEnd( );


      }

};
0penGL이 포함된 어플리케이션상어꺼 paintGL( ) 함수보다 먼저 repaii此가 수행할 필요가 있다면 코
드상에서 updateGL( ) 함수를 사용해야 한다. updateGL( ) 함수를 호출하면 glDraw( ) 함수가 호출되
고 최종 paintGL( ) 함수가 호출된다．

위젯상에 OpenGL 렌더링 context가 화면상어］ 표시하기 위해 pair此GL( ), resizeGL( ) 혹은
initializeGL( ) 함수를 호출한다. 만약 다른 위치（위젯의 생성자 혹은 Paint 함수）로부터 표준 OpenGL
API를 호출해야 한다면 makeCurrent( ) 함수를 호출해햐 한다．


eOverlays
시스템상에서 오버레이를 지원한다면 QGLWidget은 일반적인 main context어］ 추가로 GL overlay
context를 생성할 수 있다. 또한 QGLWidget은 다음과 같은 3개의 오버레이 함수를 지원한다．

종류                           설명
paintOverlayGL               paintGL( ) 함수와 동일하다. 위젯의 main con旭났를 대신해 위젯의 오버레이 연
                             산을 위하1 사용하는 재정의（Virtual) 함수이다．
resizeOverlayGL( )           paintGL( ) 함수와 동일하다. 위젯의 main con也）d를 대신해 위젯의 오버레이 연
                             산을 위해 사용하는 \/irtual 함수이며 새로운 크7를 전달한다．
initializeOverlay（孔（ )       이 함수는 initializeGL( ) 함수와 동일하다. 위젯의 m계n context를 대신하1 위젯의
                             오버러삐 연산을 사용하는 재정의（Virtual) 함수이다. 이 함수는 paintOverlayGL()
                             혹은 resizeOverlayGL( ) 함수를 호출하기 전 한번만 호출한다. 이 함수는 Open
                             GL의 context 렌더링 플래그를 설정하기 위해 사용해야 한다．



살펴본 3개의 재정의（Virtual) 함수는 paintGL( ) 함수와 동일한 방법으로 동작한다. 다른 특징은 오버
레이 con扼砒를 구성할 때 사용한다．

QGLWidget 클래스어］ 구현된 initializeGL( ）과 resize（孔（) 함수는 OpenGL 상태와 3D로 예상되는
변경사항을 설정하기 위해 사용된다. paintGL( ) 함수 3D scene을 Painting하기 위한 함수이며 위젯상


246 CHAPTER 07小 그래픽스


===== PAGE 248 =====
에서 드로잉이 필요할 때 호출된다．
이전 2D 그래픽스 단원에서 언급하였듯이 QGL砥往dget의 하위 클래스를 이용해 2D 그래픽 드로잉이 가
능하다. 2D 그래픽을 드로잉하기 위해 paintEvent( ) 함수를 다음과 같이 사용할 수 있다．

 ·QPainter 오브젝트 생성자
 ·QPainter::begin( ) 함수를 사용해 위젯상에서 초기화 할 수 있다．
 ·QPainter의 멤버함수를 사용한 드로잉
 · 페인트가 끝나면 QPainter::end( ) 함수를 호출


3D 그래픽 Contents 상어］ 2D 그래픽 Contents를 Over Painting이 가능하다. 또한 이 단원 후반부에
서 3D 그래픽스와 2D 그래픽을 함께 사용하는 방법은 예제를 통해서 다룰 것이다．


0Threading
Qt에서는 OpenGL 렌더링을 위해 Thread를 지원한다. Double Bu珏er에서 버피를 스왑（Swap) 기능
을 위해 버퍼를 동기화 할 경우가 있다. 특별하게 임베디드 디바이스에서 GPU(Graphic Process Unit)
가 버퍼를 스왑하는 동안 CPU가 유휴(idling）하지 않도록 하기 위해 T뇨ead를 활용할 수 있다. 이러한
경우 분리된 Thread에서 버퍼 스왑을 진행하고 주恤amn) Thread에서 렌더링이 가능하며 다음과 같은
순서로 Thread를 사용할 수 있다．


1Thread를 이용한 Buffer 스왑 수행 순서
 1. 렌더링을 완료할 때 주 Thread에서 doneCurrent( ) 함수를 호출한다．
  2. 스왑 Thread어꺼 소유하고 있는 context를 이동하기 위해 moveToThread( ) 함수를 호출한다．
  3. 스왑 Thread를 Notify하고 con扼砒를 Grab 할 수 있다．
  4. II垠keCi玎rent(）를 사용해 스왑 Thread에서 현재 co砒炚t를 구성하고 swapB沚fer(）를 호출한다．
  5. 스왑 Thread에서 doneCurrent( ) 함수를 호출한다．
  6. moveToThread(qApp- > thread()) 함수를 호출하고 스왑이 완료된 주 Thread를 Notify한다．


0Thread에서 Texture 업로드
포토 갤러리 어플리케이션에서와 같이 많은 이미지를 사용하는 Texture 업로드를 위해 Thread를 사용
하는 것은 매우 유용하며 존재하는 bindTexture( ) 함수를 Qt에서 지원한다. QGLWidget의 주 GUI
Thread에서 화면을 구성하고 다른 Thread에서 Texture를 업로드 하도록 구현할 수 있다．


0Thread에서 QGLWidget 상에서 드로잉하기 위해 OPainter를 사용
QGLWidget 상에서 QPaii此er를 사용하는 것은 Qt 4.8 버전 이상에서만 지원되는 기능이다. Thread
를 분리해 QPair此er를 사용할 수 있다. 또한 QGLP奴이Buffers와 QGLFramebufferObject를 사용할
수 있다. 이 기능은 OpenGL 2.0 이상의 paint engine에서만 지원한다．




                                               {（값 야兀nGL 모듈을 이용한 3D 그래픽 247


===== PAGE 249 =====
QGLWidget은 단지 주 GUI Thread에서만 생성할 수 있다. 그렇기 때문어］ 주 Thread로부터 OpenGL
의 context를 Release하기 위해서 done（그urrent( ) 함수가 필요하다. 위젯이 다른 Thread로부터 드로
잉되기 전에 QGLConte玭1moveToThread( ) 함수 호출이 필요하다. 위젯의 크기가 변경되면 주 GUI
Thread가 크기 변경 이벤트를 QGLWidget에게 이벤트를 통보한다．



            Hello OpenGL- 예제
이번 예제는 Qt에서 제공하는 QGLWidget 클래스를 이용한 예제이다. QGLWidget 클래스는 OpenGL
기반의 3D 그래픽을 화면상어］ 렌더링하기 위한 기능을 제공한다. 이 예제에서는 3D scenes의 렌더링 구
현 방법과 QGLWidget의 시그널 슬롯을 사용하는 방법에 대해 살펴볼 것이다．




（그림） QGLWidg이을 이용한 3D 그래픽 예저1



0GLWidget 클래스 정의
GLWidget 클래스는 생성자, 소멸자（destruct야）, sizeHint( ) 그리고 minimumSizeHint( ) 함수 기
능이 포함된다．

 class GLWidget : public QGLWidget
 {
   Q OBJECT
public:
     GLWidget (QWidget *parent = 0) ;
     -GLWidget () ;


     QSize minimuxnSizeHint () const;
     QSize sizeHin七（) （兀弱t;



소멸자는 위젯이 더 이상 필요하지 않을 때 OpenGL을 정의한 뎨이터 구조를 메모리로부터 반환하기 위
한 기능을 구현하면 된다．


248 CHAPTER 07_ 그래픽스


===== PAGE 250 =====
public slots:
   void setXRotation(int angle) ;
   void setYRotation(int angle) ;
   void setZRotation(int angle) ;


signals:
    void xRotationChanged(int angle) ;
    void yRotationChanged(int angle) ;
    void zRotationChanged(int angle) ;



시그널과 슬롯은 3D scene 상에서 발생하는 이벤트를 처리하기 위해 사용한다．

protected:
     void initializeGL() ;
     void paintGL() ;
     void resizeGL (int width, mnt height) ;
     void mousePressEvent (QMouseEvent *e\'ent) ;
     void mouseMoveEvent (QMouseEvent * event) ;



OpenGL 초기화, viewport 크기 변경 그리고 드로잉하기 위한 작업은 initializeGLO, resizeGL( ) 그리
고 paintGL( ) 재정의（Virtual) 함수에서 구현할 수 있다. 사용자가 마우스로 발생하는 이벤트를 처리하기
위해 mousePressEvei此（）와 mouseMoveEvent( ) 재정의 함수를 사용해 기능을 구현할 수 있다．


private:
     QtLogo *logo;
     mnt xRot, yRot, zRot;
     QPoint lastPos;
     QColor qtGreen;
     QColor qtPurple;
};
logo 변수는 QtLogo 오브젝트의 geometry 포인터를 지정하기 위한 변수이다．


S GLWidget 클래스 구현
예제에서는 QGLWidget을 사용하는 위젯과 Native 위젯（QWidget과 QFrame）을 사용하는 클래스로
분리하였다. 생성자에서는 scene을 위한 각도를 회전하기 위해 사용하는 변수를 디폴트 값인 0의 값으로
변수를 설정하고 QtLogo 오브젝트 포인터에는 초기화되지 않은 상태이므로 포인터는 null 상태이다．




                                                    旬Ot OpenGL 모듈을 이용한 3D 그래픽 249


===== PAGE 251 =====
     GLWidget: :GLWidget (QWidget *parent)
        : QGLWidget (QGLFormat (QGL: : SampleBuffers) , parent)
     {
             logo = 0;
             xR(＞七 = 0;
             yRot = 0;
             zRot = 0;


          qtGreen = QColor: :fromCmykF(0. 40, 0.0, 1.0, 0. 0) ;
          qtPurple = QColor: :fromCmykF(0.39, 0. 39, 0. 0, 0. 0) ;
     }


또한 소멸자에는 위젯이 삭제될 때 OpenGL과 관련된 리소스를 해제할 수 있도록 구현하면 된다．

 GLwidge七 : h吼Widget ( )
 {
 }


위젯이 적절한 크기로 표시될 수 있도록 前ze hint 기능을 제공한다．

 QSize GLWidget: :minimumSizeHint () const
 {
         return QSize (50, 50) ;
 }

 QSize GLWidget: :sizeHint () const
 {
         return QSize (400, 400) ;
 }


위젯이 scene의 방향을 변경할 수 있는 구성 요소로 슬롯 기능을 구현한다．

 void GLWidget: :setXRotation(int angle)
 {
         qNormalizeAngle (angle) ;
         if    (angle != xRot) {
                xRot = angle;
                emit xRotationChanged (angle) ;
                updateGL() ;
         }
 }


angle의 이전 값이 xRot 값과 다르면 xRot 변수에 angle 변수 값으로 변경하고 xR毗ationchanged()
시그널을 발생（emit）하고 updateGL( ) 함수를 호출한다. updateGL( ) 함수를 호출하면 Mappii培된
paintGL( ) 재정의 함수가 호출된다．




250 CHAPTER 07_ 그래픽스


===== PAGE 252 =====
1OpenGL 초기화
initializeGL( ) 함수는 3D scene을 렌더링하기 위해 필요한 초기화 과정을 수행한다. 주로 컬러와
OpenGL 요소를 정의하는 기능을 포함한다. 렌더링 과정은 커스터마이징과 프로퍼티들을 설정하고, 렌
더링 플래그 값을 설정한다．

    void GLWidget: :initializeGL ()
    {
        qglClearColor (qtPurple.dark (fl;


        logo = new QtLogo (this,      64) ;
        logo->setColor (qtGreen.dark () );


        glEnable ( GL_DEPTH_TEST) ;
        glEnable ( GLCULL FACE) ;
        glShadeModel (GLSMOOTH) ;
        glEnable (GL-1LIGHTING) ;
        glEnable (GL_LIGHT0) ;
        glEnable (GL_MULTISAMPLE) ;
        sta七a亡 GLfloa七 ligh七Posi上ion[ 4] = { 0. 5, 5. 0, 7.0, 1. 0 };
        glLightfv (GL_LIGHT0, GL1POSITION, lightPosition) ;
    }

예제에서는 배경색 설정과 QtLogo 오브젝트의 인스턴스를 생성하고, 각각의 shading 모듈 및 렌더링
플래그를 설정한다．


1Viewport 변경
위젯의 크기와 매칭되는 viewport로부터 scene의 렌더링되는 크기가 변경되면 resizeGL( ) 함수가 자
동으로 호출된다. 따라서 위젯의 크기가 변경되면 이 함수가 자동으로 호출된다．

    void GLWidget: :resizeGL (int width, mnt height)
    {
        m1lt side = qMin(width, height) ;
        glViewport ( (width - side) / 2, (height - side) I     2, side, side) ;


        glMatri必ode (GL PROJECTION) ;
        glLoadldentity () ;
    #ifdef QT OPENGL ES 1
        glOrthof (- 0.5, +0. 5, -0. 5, +0. 5, 4. 0, 15. 0) ;
    孝else
        glOrtho(- 0. 5, +0. 5, -0. 5, +0. 5, 4. 0, 15. 0) ;
    孝endif
1
        glMatrixMode ( GL_MODELVIEW) ;




                                                               3꾜t0pen（孔 모듈을 이용한 3D 그래픽 251


===== PAGE 253 =====
IScene2I Painting
paintGL( ) 함수는 위젯으로부터 scene의 드로잉을 하기 위해 사용하는 함수이다. QWidget의 paint
Event( ) 재정의 함수 대신 QGLWidget 클래스의 paintGL( ) 함수를 재정의해 사용한다．

    void GLWidget: :paintGL()
    {
        giClear (GL_COLOR BUFFER_BIT 1 GL'.DEPTH寸BUFFER-BIT) ;
        glLoadldentity () ;
        glTranslatef (0.0, 0.0, -10.0) ;
        glRotatef (xRot / 16. 0, 1. 0, 0.0, 0. 0) ;
        cilRotatef (vRot / 16. 0, 0. 0, 1.0. 0. 0) :
I           lRotatef (zRot / 16. 0, 0. 0. 0.0. 1. 0) :
i
            ogo-
                    >draw() ;




위의 소스 코드에서는 initializeGL( ) 함수에서 정의한 배경 컬러를 이용해 위젯을 Clear하는 기능 함수
이다. Scene어］ 렌더링되는 QtLogo 오브젝트를 드로잉하기 위해 geometry를 참조해 프레임을 설정한다．


    . 마우스 이벤트 처리
QGLWidget의 Native 클래스인 邸Vidget의 mousePressEvent( ）와 mouseMoveEvent( ) 함수를
재정의해 사용한다. mousePressEvent( ) 함수는 단순히 마우스의 위치를 기록한다．

    void GLWidget: :mousePressEvent (QMouseEvent *event)
    {
        las七Pos = even七->1均S ( ) ;
    }


mouseMoveEve砒（) 함수는 마우스 커서의 이전 위치 값을 사용해 scene의 오브젝트 방향과 각도를 결
정하기 위해 사용한다．

    void GLWidget: :mouseMoveEverit ( QMouseEvent *event)
    {
        mnt dx = event->x () - lastPos. x ( );
        mnt dy = event->y () - lastPos.y () ;


        if         (event->buttons () & Qt: :LeftButton) {
                   setXRotatiori(xRot + 8 * dy) ;
                   setYRotation(yRot + 8 * dx) ;
        } else if         (event->buttons () & Qt: :RightButton) {
                   setXRo七a七ion(xRot + 8 士 dy) ;
                   setZRotation(zRot + 8 * dx) ;
        }
        lastPos = event->pos () ;
    }




    252 CHA口TER 07_ 그래픽스


===== PAGE 254 =====
마우스 이벤트가 발생하는 순간마다 커서의 위치를 업데이트 하고 오브젝트의 회전을 드래그 또는 마우
스 버튼 이벤트를 참조한다．


0o止ogo 클래스
Open（孔 geometry 데이터 값이 3D scene에서 렌디링하기 위해 캡슐화된 클래스이다．

class QtLogo : public QObject
{
public:
         explicit   QtLogo (QObject *parent, mnt d = 64, qreal s = 1. 0) ;
         시QtLogo ( );
         void setColor (QColor C) ;
         void draw() const;
private:
         void buildGeometry (int d, qreal s) ;


         QList<Patch 出> parts;
         Geometry *geom;
};

Geometry는 여러 가지 방법으로 렌더링하기 위한 리스트 항목으로 나누어진다. 데이터는 vertices로부
터 포함하는 Geometry 구조체를 포함한다．

5七ruct Geome七ry
{
         QVector<GLushort> faces;
         QVector<QVector3D> vertices;
         QVector<QVector3D> normals;
         void appendSmooth(const QVector3D &a, const QVector3D &n, mnt from) ;
         void appendFaceted(const QVector3D &a, const QVector3D &n) ;
         void finalize () ;
         void loadArrays () const;
     ;



Geometry 클래스에서 데이터는 QVector <QVector3D> 멤버에 저장된다. 즉, constData( ) 함수를 경
유하는 raw 형태의 연속된 floating 포인트 값을 내보내기 때문어］ QVector<QVector3D）에 저장한다．

class Pa七ch
 {
public:
         enum Smoothing { Faceted, Smooth    };
         Pa七ch (Geometry 出 ) ;
         void setSmoothing(Smoothing 5) { sm = 5; }
         void translate (const QVector3D &t) ;
         void rotate (greal deg, QVector3D axis) ;
         void dra叫 ) cons七；
         void addTri(const QVector3D &a, const QVector3D &b, const QVector3D &c,          O


                                                               3 (거 OpenGL 모듈을 이용한 3D 그래픽 253


===== PAGE 255 =====
 const QVector3D &n) ;
       void addQuad(const QVector3D &a, const QVector3D &b,        const QVector3D &c,
 const QVector3D &d) ;


      GLushort start;
      GLushort count;
      GLushort initv;


      GLfloat faceColor[ 4] ;
      QMatrix4x4 mat;
      Smoothing Sm;
      Georne七ry 士geom;
 };
높은 수준의 Patch 클래스는 한번에 하나의 face 형상을 축적하기 위한 메소드를 가지고 있다. 그리고
서로 다른 색상을 적용하거나 부드럽게 처리하기 위해 face 변경을 위한 collection을 가지고 있다．

 void Patch: :draw() const
 {
      glPushNatrix () ;
      glMultMatrixf (mat.constData () );
      glMaterialfv ( GL_FRONT_AND BACK, GL_AMBIENT_A旺）_DIFFUSE, faceColor) ;


      const GLuShort *indices = geom->faces.constData() ;
      glDrawElements (GLTRIANGLES, count, GL_UNSIG卜ED_SHORT
                                           r indices + start) ;
      glPopMatrix () ;
 }


Patch 클래스는 단순히 어떤 변화된 scene을 적용한다. 그리고 model View Matr奴는 저장 및 변환이
다음 부분에 영향을 미치지 않도록 변환한다．

 void QtLogo: :buildGeometry (int divisions, greal scale)
 {
      qreal cw = cross width * scale;
      qreal b七 = barm七hickness 士 scale;
      qreal ld = logo_depth * scale;
      qreal th = tee_height *scale;


      RectPrism cross (geom, cw, bt, ld) ;
      RectPrism stern(geom, bt, th, ld) ;


      QVector3D z (0. 0, 0.0, 1. 0) ;
      cross.rotate (45. 0, z) ;
      眺em.r毗ate (45.0, z) ;


      qreal stem_downshift = (th + bt) / 2.0;
      stem. translate(QVector3D(0 .0, -stem.mdo寸nshift, 0. 0) );
                                                                                         O



254 CHAPTER 07_ 그래픽스


===== PAGE 256 =====
      RectTorus body (geom, 0. 20, 0. 30, 0.1, divisions) ;


      parts << stem.parts << cross.parts << body.parts;


      geom->finalize ( ) ;




      沮3; HW 가속기를 이용한 2D 그래픽 렌더링
2D 그래픽을 화면상에 렌더링하기 위해 QWidget 하위 클래스어］ 포함된 QPainter 클래스를 사용하였
다. 이러한 방법은 화면상어］ 21) 그래픽 요소를 렌더링하기 위한 연산을 CPU에서 처리한다．

그래픽을 렌더링하는 것은 CPU와 같은 시스템의 많은 자원을 소모한다. 데스크탑 컴퓨터의 경우 그래픽
카드 인터페이스어］ 내장된 GPU(Graphic Process Unit）를 사용한다. 임베디드 디바이스와 같은 시스
템은 OpenGL 3D 그래픽을 처리하기 위해 하드웨어 가속 칩을 사용한다．

Qt에서는 2D 그래픽을 처리하기 위해 하드웨어 기반의 3D 가속기를 사용할 수 있다. 따라서 복잡한 2D
그래픽을 렌더링 할 경우 3D 하드웨어 가속기를 통해 2D 그래픽을 렌더링 할 수 있다．


                  Qt Applicatkn   ba羽d   2D Gra하                      )
  I     QPainter class       ）켜卜H/         QGLWdge1 class      ')
                                                   +
  (                   HW Graphic Accelerator                  "   '


（그림） HW 가속기를 사용한 2D 그래픽 어플리케이션 클래스 구조



QGLWidget 클래스는 邸Widget의 하위 클래스이다. 화면에 2D 그래픽 요소를 그리기 위해 QPainter
를 사용하고 paintEvent( ) 함수를 재정의할 수 있다. QPainter 클래스는 QWidget의 하위 클래스이므
로 QGLWidget 클래스상에서 QPainter 클래스를 이용해 Drawing 한 2D 그래픽을 Q（訌Widget의
3D Scene상에 렌더링이 가능하다．

이번 예제에서는 邸Widget 클래스를 이용해 2D 그래픽을 렌더링 한 결과와 QGLWidget 클래스를 이용
해 2D 그래픽의 렌더링 결과를 비교해 볼 수 있다. 각각의 2D 그래픽 드로잉은 QPainter 클래스를 상속
받아 구현한 Helper 클래스를 사용한다．




                                                              3_Ot OpenGL 모듈을 이용한 3D 그래픽 255


===== PAGE 257 =====
  12C 七nting 0八 N計P므r숀 ar二 OF｝므nG_ 砥'dgets




               Native                        OpenGL



（그림） HW 가속기를 이용한 2D Painting 예제



0Helper 클래스 정의
예제에서 H이per 클래스에 의해 구현된 드로잉 한 2D Painting 결과를 각각의 위젯（QWidget과 QGL
Widget）에 렌더링한다．

 class Helper
 {
 public:
         Helper () ;


 public:
         void paint (QPainter *pajnter, QPaintEvent *event, mnt elapsed) ;


 private:
         QBrush background;
         QBrush circleBrush;
         QFon七 textFon七；
         QPen circiePen;
         QPen 七e＞比Pen;
     ;



생성자 다음에 위치한 paint( ) 함수는 단지 각 위젯에 드로잉을 위해 구현한 함수이다．


0Helper 클래스의 구현
위젯에서 2D 그래픽은 드로잉이 필요하다. Helper 클래스 생성자는 리소스를 설정한다．

 Helper: :Helper ()
 {
         QLinearGradient gradient (QPointF(50, -20) , QPointF(80, 20) );
         gradient. setColorAt (0. 0, Qt: :white) ;
         gradient. setColorAt (l .0, QColor (0xa6, Oxce, 0x39) );


         background = QBrush(QColor (64, 32, 64) );
         circieBrush = QBrush (gradient) ;                                   O


256 CHAPTER 07_ 그래픽스


===== PAGE 258 =====
         circlepen = QPen(Qt: :black) ;
         circlepen. setWidth( 1) ;
         textPen = QPen(Qt: :white) ;
         textFont. setPixelSize (50) ;




실제 그래픽이 그려지는 것은 paint( ) 함수에서 수행한다. 페인트 디바이스로부터 Painter를 설정하고
드로잉（Paint) 될 영역을 지정한다. 드로잉 영역에 관한 정보를 제공하는 QPaii此Ever此는 페인트 디바
이스상에 마지막 업데이트된 경과 시간을 측정한다．

    void Helper: :paint (QPainter *painter, QPairitEvent *event, mnt elapsed)
    {
         painter->fillRect (event->rect () , background) ;
         painter->translate (100, 100) ;



Paint Device의 중심（원점）으로부터 변위되는 좌표계의 원점을 해석하기 위해 Paint 이벤트어］ 포함된
영역을 작성하여 드로잉한다．

    painter->save () ;
         painter->setBrush ( circleBrush) ;
         painter->setPen ( circlePen) ;
         painter->rotate (elapsed * 0. 030) ;


         qreal r = elapsed/ 1000. 0;
         mnt n = 30;
         for (mnt i = 0; i < n; ++i) {
             painter->rotate ( 30) ;
             qreal radius = 0 + 120. 0* ( (i+r) /n) ;
             qreal circleRadius = 1 + ( (i+r) /n) *20;
             painter->drawEllipse ( QRectF (radius, -circleRadius,
                                              circleRadius*2, circleRadius* 2) );
         }
        painter->restore () ;



드로잉 좌표계는 이 과정에서 회전이 여러 번 동작하는 동안 QPaii此er의 상태를 저장하고 복원하기
                                                                                            위
해1restore( ) 함수를 사용한다．


r       pairiter->setPen ( textPen) ;
        painter->setFont (textFont) ;
        painter->drawText (QRect (- 50, -50, 100, 100) , Qt: :AlignCenter, "Qt ") ;




효과（Effect）를 완료하기 위해 원점에서 일부 텍스트를 드로잉한다．




                                                                3 (거 OpenGL 모듈을 이용한 3D 그래픽 257


===== PAGE 259 =====
0Widget 클래스 정의
Widget 클래스는 Helper 클래스어］ 의해 드로잉（Paint）한 단순한 애니메이션을 위젯에 렌더링하기 위해
구현한 커스텀 위젯 클래스이다．

class Helper;
class QPaintEvent;


class Widget : public QWidget
{
        Q OBJECT


public:
        Widget (Helper *helper, QWidget *parent) ;


public slots:
        void aniinate () ;


protected:
        void paintEvent (QPaintEvent *event) ;


priva七e:
        Helper *helper;
        mnt elapsed;
 };


생성자에는 단지 paintEvent( ) 함수, 그리고 그 내용을 애니메이션 효과를 사용하는 드로잉을 호출할
수 있는 슬롯이 포함되어 있다. 하나의 멤버변수는 위젯의 내용, 그리고 업데이트된 경과시간을 디버깅하
는데 사용한다．


1Widget 클래스 구현
생성자는 단지 멤버변수를 초기화, Helper 오브젝트를 저장하고 클래스의 기본 생성자를 호출한다．

 Widget: :Widget (Helper *helper, QWidget *parent)
     : QWidget (parent) , helper (helper)


        elapsed = 0;
        setFixedSize (200, 200) ;




animate( ) 슬롯 함수는 타임아웃이 발생하면 호출된다．

    void Widget: :animate ()
    {
         elapsed = (elapsed + qobjectcast<QTimer*>(sender () )_>interval() )
                                                                      % 1000;
         repaint () ;
    }


 258 CHAPTER 07= 그래픽스


===== PAGE 260 =====
마지막 타임아웃이 발생한 이래로 경과시간의 interval 값을 결정한다. 그리고 위젯을 repainting하기
전에 이미 존재하는 값을 추가한다. 매초마다 Helper 클래스에서 사용한 애니메이션이 동작하는 이래로
항상 1000 보다 작은 경과시간을 보장하기 위한 연산을 사용한다．
H이per 클래스가 실제로 모든 요소를 Paintir培한 이후로 위젯상에 QPainter를 설정하기 위한 paint
이벤트를 구현해야 하며 paint( ) 함수를 호출한다．

void Widget: :paintEvent (QPaintEvent *eJent)
{
     QPainter painter;
     pain七er.begin (thi引 ;
     painter. setRenderHint (QPainter: : Antialiasing) ;
     helper->paint (&painter, event, elapsed) ;
     painter. end() ;




0GLWidget 클래스 정의
GLWidget 클래스 정의는 기본적으로 \/idget 클래스와 같다. 다른 점은 QGLWidget 클래스로부터 파
생된다．

class Helper;
class QPaintEvent;
class QWidget;

class GLWidget : public QGLwidget
{
     Q OBJECT

public:
     GLWidget (Helper *helper, QWidget *parent) ;


public slots:
    void animate ( ) ;


protected:
     void paintEvent (QPaintEvent *event) ;

private:
     Helper *helper;
     mnt elapsed;
};


다시 한번 elapsed 멤버변수는 위젯의 이전 업데이트 이후 경과 시간을 측정하여 드로잉 하는데 참조되
는 값을 기록한다．


0GLWidget 클래스 구현
생성자는 \Vidget 클래스의 생성자와 대부분 비슷하다．


                                                           3 0t 0口enGL 모듈을 이용한 3D 그라땍 259


===== PAGE 261 =====
GLWidget: :GLWidget (Helper *helper, QWidget *parent)
     : QGLWidget (QGLFormat (QGL: : SainpleBuffers) , parent) , helper (helper)


     elapsed = 0;
     setFixedSize (200, 200) ;
     setAutoFillBackground(false) ;




경과된 시간을 측정하기 위한 이apsed 멤버변수 초기화뿐만 아니라 위젯상어］ 드로잉하기 위해 사용하는
Helper 클래스의 오브젝트를 저장한다. 그리고 클래스의 생성자는 OpenGL 포맷으로 QGL: :Sample
Buffers 플래그를 지정하기 위해 호출한다. 이 포맷은 시스템의 OpenGL 드라이버에서 지원하는 Anti
-aliasii培을 활성화한다．

void GLWidget: :animate ()                                                          1
{
     elapsed = (elapsed + qobject cast<QTimer*>(sender () )_>interval() ) % 1000;
     repaint ( ) ;
}


paintEvent( ) 함수는 Widget 클래스의 paintEvent( ) 함수와 대부분 동일하다．

void GLWidget: : paintEvent ( QPaintEvent *event)
{
     QPainter painter;
     painter, begin (this) ;
     painter. setRenderHint (QPainter: :Antialiasing) ;
     helper->pairit (&painter, event, elapsed) ;
     painter. end() ;
}


anti-aliasing이 활성화된 이후로 위젯상어］ QPaii此er 설정이 필요하고 위젯의 Contents를 화면상에
렌더링하기 위해 Helper 클래스의 paint( ) 함수를 호출한다．


0Windc汭사 클래스 정의
Window 클래스는 기본적인 최소한의 기능을 구현하기 위한 것만 정의한다．

class Window : public QWidget
{
   Q OBJECT
public:
    Window ( ) ;
private:
     Helper helper;
};



260 CHAPTER 07_ 그래픽스


===== PAGE 262 =====
이 클래스는 모든 위젯 사이에서 공유하기 위한 하나의 Helper 오브젝트를 포함한다．


S Window 클래스 구현
생성자는 각각의 위젯을 생성하고 레이아웃상어］ 위젯을 삽입하고 배치한다．

f Window: :Window()
      : Qwidget ()
 {
      Widget *native = new Widget (&helper, this) ;
      GLWidget *openGL = new GLWidget (&helper, this) ;
      QLabel *natjveLabel = new QLabel (tr ( "Native ") );
      nativeLabel->setAlignment ( Qt: : AlignHCenter) ;
      QLabel *openGLLabel = new QLabel(tr ( "OpenGL") );
      openGLLabel->setAlignment (Qt: :AlignHCenter) ;


      QGridLayout *layout = new QGridLayout;
      layout->addWidget (native, 0, 0) ;
      layou七->addWidget（아冶nGL, 0, 1) ;
                                             0
      layout->addWidget ( nativeLabel, 1,
      layout->addWidget ( openGLLabel, 1, 1
      setLayout ( layout) ;


      QTimer *timer = new QTimer (this) ;
      connect (tixrter, SIGNAL(timeout () ), native, SLOT (animate () ))
      connect (timer, SIGNAL(timeoutU) , openGL, SLOT (animate () ));
      timer->start (50) ;


      setWindowTitle (tr ( "2O Painting on Native and OpenGL Widgets ") );
 }


50 millisecond의 타임아웃을 발생하는 타이머는 애니메이션을 구현하는 목적으로 필요하다. Widget
과 GLWidget 오브젝트의 슬롯과 연결되어 있다. 어플리케이션이 시작되면 초당 20 frame을 업데이트
한다．



      3.4 QPainter 클래스의 Over Painting

QGLWidget 클래스는 일반적인 Op이GL을 사용해 3D 그래픽을 화면상어］ 렌더링하고 QPainter 클래1
스를 이용해 Over Paintii培（3D가 렌더링된 화면에 QPainter를 이용한 그래픽 요소를 동일한 화면에
렌더링）을 할 수 있는 기능을 제공한다. 또한 Over Painting을 사용한 위젯은 시그널 슬롯 그리고 프로
퍼 티를 지원하는 표준 Qt 위젯과 동일하다．

QGLWidget은 3D scene을 화면상에 디스플레이 하기 위한 클래스이다. 개발자는 초기화해야 하는 리
소스를 initializeGL( ) 함수를 사용해 재정의해 구현한다. resizeGL( ）은 viewport와 pr이ection을 설
정하고 Opei好L을 수행하는 paintGL( ) 함수는 scene을 렌더링하기 위해 사용되는 함수이다．


                                                              3 （그t0pen（孔 모듈을 이용한 3D 그래픽 261


===== PAGE 263 =====
QGLWidget의 하위 클래스인 QPainter 클래스를 사용해 3D scene상어］ 2D 그래픽을 렌더링 할 수 있다．

이 예제에서는 3D scene상에 Hello GL 예제를 통해 얻은 결과물어］ 21) 그래픽을 0ver Pair此ing 할 수
있는 결과를 보여주기 위한 예제이다．




（그림） Over Painting （계저1



的 GLWidget 클래스 정의
GLWidget 클래스는 Hello GL 예제에서 사용했던 클래스를 기반으로 한다. 클래스의 첫 번째 몇 라인
과 나머지 변경된 내용을 설명한 것이다．

 class GLWidget : public QGLWidget
 {
      Q OBJECT


 public:
      GLWidget (QWidget *parent = 0) ;
      사GLWidget ( ) ;


 protected:
      void initializeGL ( ) ;
      void paintEvent (QPaintEvent *event) ;
      void resizeGL(int width, m1lt height) ;
      void mousePressEvent (QMouseEvent *event) ;
      void mouseMoveEvent (QMouseEvent *event) ;
      void showEvent (QShowEvent *event) ;


 private slots:
      void animate () ;




262 CHAPTER OT 그래팍스


===== PAGE 264 =====
priva七e :
      void createBubbles (int number) ;
      void drawlnstructions (QPainter *pajnter) ;


      QtLog（그 火log（그；
      QList<Bubble*> bubbles;
      QTimer aninlationTimer;



                                          위한 과정을 수행하기 위해 initializeGL()
위젯은 scene을 위한 geometry 설정과 OpenGL을 초기화하기
                                             2D Viewport어］올바르게 변환되는 것
함수를 사용한다. resizeGL( ) 함수는 311) 그래픽 위젯상에 표시되는
을 보장하기 위해 사용한다．

                                        는 대신해 QWidget 클래스의 paint
위젯에서 업데이트 핸들링을 하기 위해 paintGL( ) 함수를 구현하
                                         showEvent( ) 함수를 구현해 사용
Event( ) 함수를 구현한다. 또한 2D 그래픽의 초기화를 돕기 위해
한다．
                                                   관계가 있다. animation( ) 슬롯 함
새로운 Private 멤버함수와 변수는 2D 그래픽과 애니메이션에서만
                                               일정 시간 간격으로 호출한다. create
수는 위젯을 업데이트하기 위해 animationTimer어］ 의해
                                                    r 클래스를 대신하기 위한 Bubble
Bubbles( ) 함수는 애니메이션을 드로잉하기 위해 사용하는 helpe
                                                  ］ over painted 된 반투명 처리를 책
ii毗를 초기화한다. drawlnstructions( ) 함수는 OpenGL scene어
임진다．


DGLWidget 클래스 구현
                                     이션을 제어할 수 있는 QTimer를 초기
이 예제와 관련된 GLWidget의 구현 부분은 생성자어囚 애니메
화한다．

  GLWidge七：:GLWidget (QWidge七 사沮rent)
       : QGLwidget (QGLFormat (QGL: :SampleBuffers)
                                                    , parent)
                                                                                                         1
  {
       QTime midnight (O, 0, 0) ;
                                                    e () ) ) ;
       qsrand (midnight. secsTo (QTime: :currentTim

                   0
        O 七 七 七
        八늬 O O O
                   0

        O R R R
                   0

        l X y Z    n
                   U


                                                                      )
                                                                     0 0
                                                             nU
                                                                           r
                                                                           1
                                                     1. 0,
        qtGreen = QColor: :fromCmykF (0. 40, 0. 0,
                                                                 1

                                                             0             U
                                                                           n
                   QColo r: :fromc mykF( 0. 39, 0. 39,  0.   1        口

        qtPurple =


        animationTimer. setSingleshot (false) ;
                                                       this,                   SLOT (aniniate ( )));
        connect (&animationTimer, SIGNL (timeout () ),
        animationTin ier. start (25) ;




                                                                               3 (가 OpenGL 모듈을 이용한 3D 그래픽 263


===== PAGE 265 =====
      setAutoFillBackground( false) ;
      setMinimuxnSize (200, 200) ;
      setWindowTitle(tr ( "Overpainting a Scene ' ) );
 }


QPainter 클래스의 begin( ) 멤버함수가 호출될 때 OpenGL이 위젯의 Background를 paint 하지 않
도록 지시하기 위해 위젯의 autoFillBackground 프로퍼티를 해제한다．

다른 예제에서와 같이 소멸자（destruc切r）는 OpenGL이 사용한 시스템 리소스를 해제하기 위해 구현
한다．

 GLWidget: :-GLWidget ( )
 {



initializeGL( ) 함수는 단지 QtLogo 오브젝트를 설정하기 위한 최소한의 기능을 구현한다. QtLogo 오
브젝트에 대한 상세 설명은 이전 예제를 참고하면 된다．

 void GLWidget: :initializeGL ()
 {
     glEnable ( GLM兀TISANPLE) ;


     log（그 = now QtLogo作hi引 ;
     logo->setColor (qtGreen.dark ( ) );
 }


QPainter 클래스로 over paintil培의 기능을 완벽히 구현하기 위해1 위젯이 업데이트 될 때까지 속성과
Matrix stack 연산을 연끼한다. 이 예제에서는 scene을 렌더링하기 위해 paintGL( ) 보다 먼저
paintEvent( ) 함수를 구현한다．

QGLWidget 상에 드로잉 될 때 , QPaix此er가 사용하는 Paint 엔진은 OpenGL의 구현해야 하는 부분의
Matr奴와 프로퍼티 Stack의 상태 변경에 관련된 정확한 연산을 수행한다. 그러므로 2D 오버레이를 드
로잉하는 QPainter 설계 이전에 3D 그래픽을 화면상에 표시하기 위한 모든 OpenGL을 호출할 수 있도
록 만들 필요가 있다．

모델과 프로젝션 변환 및 기타 속성을 설정하여 3D scene을 렌더링한다. 나중에 원래의 상태로 복구할
수 있도록 원래의 八4atrix 상태를 유지하기 위해 OpenGL의 Stack을 사용한다．

     glMa七ri朴伯de (GLM0DELVIEW) ;
     glPushNatrix ( );


위젯의 Background어］지정한 컬러를 사용하고 렌더링이 될 scene 상의 다양한 속성을 설정한다．



264 CHAPTER 07_ 그래픽스


===== PAGE 266 =====
    qglClearColor (qtPurple.dark () );
    giShade卜幻del (GL卞SMOOTH) ;
    glEnable (GL DEPTHHTEST) ;
    glEnable (GL CULL. FACE) ;
    glEnable (GLLIGHTING) ;
    glEnable ( GL-mLIGHT0) ;
    glEnable ( GL-MULTISANPLE) ;
    static GLfloat lightPosition[ 4] = { 0. 5, 5. 0, 7. 0, 1. 0 };
    glLightfv (GLmLIGHT0, GL_POSITION, lightPosition) ;


    setupViewport (width ( ), height () );



Scene의 사용하는 프로젝션을 설정하기 위해 S毗upViewport( ) 비공개（private) 멤버함수를 호출한다．
OpenGL 예제에서 pail孔GL( ) 함수를 구현하는 것은 불필요하다. 그 이유는 Matrix stack이 일반적으
로 resizeGL( ) 함수와 paintGL( ) 함수가 호출되는 사이의 수정이 없기 때문이다．

위젯의 Background가 시스템과 Qt어］ 의해 그려지지 않은 상태 이래로 이전 scene어］ 정의된 객체를 위
치하기 전어］ OpenGL은 드로잉 하기 위해 사용한다．

r   giClear (GL_COLOR_BUFFER_BIT 1 GL_DEPTH_BUFFER_BIT) ;
    glLoadldentity () ;
    giTranslatef (0. 0, 0. 0, -10. 0) ;
    glRotatef (xRot / 16. 0, 1. 0, 0.0, 0. 0) ;
    glRotatef (yRot / 16. 0, 0. 0, 1. 0, 0. 0) ;
    glRotatef (zRot / 16. 0, 0. 0, 0.0, 1. 0) ;
    logo->draw ( );



QtLogo 객체의 그리기 메소드가 실행되면 Over Painting을 시작하기 전에 入4atrix stack이 함수의 시
작 부분의 원래 상태로 복원해야 한다．

    giShadeModel (GL_FLAT) ;
    glDisable (GL-1CULL---FACE) ;
    giDisable ( GL_DEPTH_TEST) ;
    glDisable(GL LIGHTING) ;
    glMatrix卜ode ( GLHMODELVIEW) ;
    glPopMatrix () ;



3D 그래픽 렌더링과 함께 위젯상에 사용되는 2D 그래픽이 위젯을 Over Paintir培을 사용하기 위해
QPair此er를 설계한다. 이 경우 위젯에 반투명 Bubble을 그리기 위해 helper 클래스를 사용하여 오버레
이 drawlnstructions( ) 함수를 호출한다．




                                                          3 (코 OpenGL 모듈을 이용한 3D 그라땍 265


===== PAGE 267 =====
    QPainter painter (this) ;
    painter. setRenderHint ( QPainter: : Antialiasing) ;
    foreach (Bubble *bubble, bubbles) {
         if   (bubble->rect ( ) . intersects (event->rect (fl)
              bubble->drawBubble ( &painter) ;
    }
    drawlnstructions ( &painter) ;
    painter. end( ) ;
}


QPainter 클래스의 end( ) 함수가 호출되었을 때 , 적절한 OpenGL을 정의한 호출이 scene을 위젯상어］
작성하기 위해1 만들어진다. resizeGL( ) 함수의 구현은 Vie叫）ort의 넓이를 설정하고 pr이ect 변환을 정
의한다．

void GLWidget: :resizeGL(int width, mnt height)
{
    setupViewport (width, height) ;
}


가장 이상적으로 위젯의 넓이（dimension）를 적합하게 2D 그래픽을 정렬하기 원한다. 이러한 목적을 달
성하기 위해 showEvent( ) 핸들러 함수, 그리고 만약 위젯에 위치를 접근하기 위해 필요하다면 새로운
그래픽 요소（B따力le）들을 생성하도록 구현한다．

void GLwidget: : showEvent (QShowEvent *event)


    QUNUSED(event) ;
    createBubbles (20 - bubbles.count () );




이 함수는 20개 미만의 bubble이 이미 생성된 상태라면 효과적이다．
animate( ) 슬롯함수는 timeout( ) 함수 시그널이 발생하면 위젯의 animationTimer가 매번 호출된다．

void GLWidget: :animate ()
{
    QMutableListlterator<Bubble*> iter (bubbles) ;


    while (iter. hasNext () ) {
         Bubble 싸沁比le = j土er. ne砒（ ) ;
         bubble->move (rect () );
    }
    update() ;
I


단순히 bubble list에서 bubble이 각각 이동하면서 반복된다. setupViewport( ) 함수는 paintEvent()
함수와 resizeGL( ) 함수로부터 호출된다．


266 CHAPTER 07_ 그래픽스


===== PAGE 268 =====
void GLWidget: :setupViewport (int width, mnt height)
{
         mnt side = qMin(width, height) ;
         glViewport ( (width - side) / 2, (height - side) / 2, side, side) ;

    glMatrixaode ( GL_PROJECT ION) ;
    giL（그adldenti七y ( ) ;
#ifdef QT OPENGL ES
    glOrthof (- 0. 5, +0. 5, -0. 5, 0. 5, 4.0, 15. 0) ;
#else
   giOrtho (- 0. 5, +0. 5, -0. 5, 0. 5, 4. 0, 15. 0) ;
#endif
   glMatrixMode (GL MODELVIEW) ;
}


drawlnstructions( ) 함수는 3D scene 상어］ 2D 그래픽으로 드로잉하는 기본 instruction을 준비하기
위해 사용한다．

void GLWidget: :drawlnstructions (QPainter *painter)
{
         QString text = tr ( "Click and drag with the left mouse button 1'
                             "to rotate the Qt logo. ") ;
         QFontMetrics metrics = QFontMetrics (font (fl;
         mnt border = qMax (4, metrics.leading ( ));


         QRect rect = metrics.boundingRect (0, 0,
                                     width() - 2*border, mnt (height ( * 0.125) ,
                                            Qt: :AlignCeriter 1 Qt: : TextWordWrap, text) ;
         painter->setRenderHint (QPainter: : TextAntialiasing) ;
         painter->fillRect (QRect (0, 0, width() , rect. height () + 2*border) ,
                           QColor (0, 0, 0, 127) );
         painter->setPen(Qt: :white) ;
         painter->fillRect (QRect (0, 0, width() , rect. height () + 2싸珣rder) r
                            QColor (0, 0, 0, 127) );
         painter->dra刃？ext ( (width() - rect. width( ))I2, border,
                             rect. width( ), rect. height () ,
                             Q七：:AlignCen七er 1 Q七：:Tex七1幻rdWrap, 七ext) ;
    }



3D 콘텐츠에 2D 콘텐츠를 Over Painting 할 때 , 원하는 효과를 만들기 위해 OpenGL을 호출하도록 만
들어야 한다. QGLWidget 하위 클래스에서 사용할 때 QPainter 자체가 OpenGL을 호출하여 사용하기
때문어］ 다음과 같은 방법을 사용해 OpenGL의 Stack 상태를 보존할 필요가 있다．

        ·QGLWidget 클래스의 initializeGL( ) 함수를 재정의해 구현한다. 하지만 최소한의 기능만 구현하
         도록 한다. QPaii此er가 초기화 과정을 수행하며, 八ilatr奴와 프로퍼티를 수정하고 3D scene을 렌더
         링하기 직전까지 초기화 과정을 미루는 것이 더 좋은 방법이다．

                                                               乙（거 OpenGL 모듈을 이용한 3D 그래픽 267


===== PAGE 269 =====
  · 순수하게 Open（孔 3D의 경우에서와 같이 QGLWidget 클래스의 resizeGL( ) 함수를 재정의해 구
   현한다．
  ·2D와 3D 그래픽 모두 드로잉하기 위해 paintEvent( ) 함수를 재정의해 구현한다．


paintEvent( ) 함수를 구현하는 과정에서 다음과 같이 구현한다．
  · Stack 상어］ OpenGL modelview m毗rix를 삽입한다．
  · in代坮lizeGL( ) 함수에서 초기화 과정을 수행한다．
  · 정확한 예상 변환을 설정하는 것은 위젯의 resizeGL( ) 함수에서 위치를 지정하도록 코드를 수행하
   고 viewport를 설정한다．
  ·OpenGL을 호출해1 사용하도록 scene을 렌더 링한다．
  ·OpenGL modelview matr奴를 stack에서 꺼낸다．
  ·QPainter object를 설꼐한다．
  ·QPainter 클래스의 begin( ) 함수로 시작해 초기화한다.
  ·QPainter의 멤버함수를 사용해 원형을 드로잉한다．
  · 페인팅이 끝나면 QPainter 클래스의 end( ) 함수를 호출한다．




268 CHAPTER 07．느 그래픽스


===== PAGE 270 =====
01 5 Programming




r          4 Scalable Vector Graphics
        1 아는 SVG를 처리할 수 있는 아Svg 모듈을 제공한다. 따라서 아Svg를 통하I SVG를 핸들링하:7 ' 위한
          방법에 대해 알아보도록 하자．




SVG(Scalable Vector Graphics）는 \Tector Graph를 표시하기 위한 방법으로 XML 기반으로 정의되
어 있다. Qt는 SVG를 지원하며 QtSvg 모듈을 사용해 SVG를 Qt 응용 어플리케이션 상에 Rendering
할 수 있다. QtSvg 모듈을 사용하기 위해서는 다음과 같이 iflClU(扼를 사용해 QtSvg 모듈을 선언해야
한다．

 #include <QtSvg>


또한 QtSvg 모듈을 사용하기 위해 qmake 프로젝트 파일（.pro 파일）에 SVG 모듈을 다음과 같이 추가해1
야 한다．

iQT += svg


Qt에서는 SVG 이미지를 핸들링하기 위해 다음과 같은 클래스를 제공한다．

 클래스                설명
 QGraphicsSv이也m     XML 기반의 SVG 파일을 이미지로 Rendering 할 수 있는 기능을 제공
 oSvgGenerator      SVG를 이용해 드로잉하기 위한 Paint Device
 QSvgRenderer       Paint Device 상에서 SVG 파일을 드로잉하71 위해 사용
 QSv이Vidget         Sca冶ble Vector Graphics 파일의 XML 콘텐츠를 위젯상에 디스플러回 하기 위한 기능을 제공



0QGraphicsSvgltem 클래스
QGraphicsSvgltem 클래스는 SVG 파일의 콘텐츠를 렌더링하기 위한 QGraphicsltem이며
QGraphicsView 상에서 SVG 파일을 렌더링하기 위한 방법을 제공한다. 이 클래스의 setElementld()
멤버함수어］ 전달된 인자 값인 아이디(ID）를 통해 SVG 파일 일부분을 렌더링할 수 있다. 이 방법은 큰
SVG 파일의 콘텐츠를 Element로 나누어 렌더링하기어］ 적합하다．




                                                            4 Sc졔able Vec幻r Gra아기os 269


===== PAGE 271 =====
 QSvgRenderer *renderer =
                            new QSvgRenderer (QLatinlString( " SvgCardDeck. svg") );

 QGraphicsSvgltem *black = new QGraphicsSvgltem( );
 QGraphicsSvgltem *red   = new QGraphicsSvgltem( );

 black->setShare妊enderer ( renderer) ;
 black->setElementld (QLatinlString( " black joker ") );

 red->setSharedRenderer (renderer) ;
 red->setElement工d(QLatinlString( "red_joker ' ));




이 클래스는 SVG 아이템의 크기 값을 얻기 위해 setSize( ) 멤버함수를 사용할 수 있다. 기본적으로
SVG 파일의 렌더링 성능을 높이기 위해 QGraphicsltem: :Device（그oordinateCache 모드를 사용할 수
있다. Cache를 사용하지 않기 위해서는 QGraphicsltem: :NoCache 모드를 사용할 수 있다. 모드어］ 대
한 변경은 QGraphicsltem::setCache入化de( ) 함수를 사용해 인자로 지정할 수 있다．


0OSvgGenera幻r 클래스
QSvgGenerator 클래스는 SVG를 드로잉 할 Paint Device를 제공한다. 즉 QPainter와 같은 동일한
방식을 사용한다．

 QSvgGenerator generator;
 generator. setFileName (path) ;
 generator. setSize (QSize (200, 200) );
 generator. setViewBox (QRect (0, 0, 200, 200) );
 generator. setTitle (tr ( "SVG Generator Example Drawing") );
 generator. setDescription(tr ( "An SVG drawing created by the SVG Generator     n


                                "Example provided with Qt. ") );



또한 이 클래스의 인스턴스를 QPainter 오브젝트로 사용할 수 있으며 QPainter 클래스의 begin( ）과
end( ) 함수를 사용해 SVG상어］ 드로잉 요소를 추가할 수 있다．

 QPainter painter;

painter,begin ( &generator) ;

painter.end ( );




1QSvgRenderer 클래스
QSvgRenderer 클래스는 Paint 디바이스 상에서 SVG 파일 콘텐츠를 드로잉하기 위한 기능을 제공한
다. QSvgRenderer 클래스를 사용하기 위해서는 QPaintDevice의 하위 클래스로 렌더링 할 수 있다．
따라서 QSvgRenderer 클래스를 사용하면 邸Widget, Qimage 그리고 QGLWidget어］ SVG 파일의 콘


270 CHAPTER 07_ 그래픽스


===== PAGE 272 =====
텐츠를 Rendering 할 수 있다．


S QSvgWidget 클래스
QSvgWidget 클래스는 QWidget과 QGLWidget 상에서 이미지 혹은 기본적인 드로잉을 표시할 수 있
는 것과 같이 SVG 파일의 콘텐츠를 표시할 수 있는 위젯을 제공한다. 이 클래스는 QWidget과 QObject
클래스를 상속받았기 때문어］ QWidget과 QObj ect의 멤버함수를 사용할 수 있다．

이 클래스는 생성자로 부모 위젯을 지정할 수 있으며 문자열 형태의 SVG 파일명을 지정할 수 있는 생성
자를 제공한다．

QSvgWidget (QWidget * parent = 0)
QSvgwidget (const QString & file,   Qwidget * parent = 0)




                                                            4_Sc톄ab咆 Vector G田아기cs 271


===== PAGE 273 =====
MQvv1乙）


===== PAGE 274 =====
          CHAPTER




Animation Framework과
         State Machine


===== PAGE 275 =====
Qt 5 Programming



          1 · Animation 다amewo水과
二n
              State Machine
瑟發轟鱗藝 이동， 확대I, 축소 등 애니메이션 요소를 사용하는 방법과 State Machine를 처리하71 위한 방법에 대
      해 알아보도록 하자．




Animation Framework는 부드러운 화면 전환과 애니메이션 요소를 추가한 GUI 인터페이스를 쉽게
작성할 수 있도록 제공하기 위한 프레임워크이다. Qt에서 제공하는 위젯, QOb把Ct로부터 파생된 클래스
위젯 등과 같은 요소에 애니메이션 효과를 사용할 수 있다．

그리고 State Machine이란 Finite State Machine을 뜻하며 상태들 사이에 움직임을 정의하기 위해
사용하는 개념이다. 예를 들어 스위치의 행동 동작을 보면 ON/OFF의 두 가지 경우가 있으며 , 행위에 의
해 ON 또는 OFF로 변경된다. State Machine을 사용하면 Animation 요소를 사용해 요소 간의 행위
를 그룹화 하여 간단하고 쉽게 구현할 수 있다．

또한 Animation Framework는 c++ 기반의 GI끄를 작성하는 프레임워크 이외에 Qt 鈿ick에서도 활
용할 수 있는 프레임워크도 제공한다．

후반부에서 QState를 사용해 Animation 요소가 행위에 의해 변경되는 상태를 구현하는 방법에 대해 다
룰 것이며, 여기서는 Anim毗如n Framework과 State 玉4achine을 살펴보고 예제를 통해 직접 구현해
보도록 하자．




 274 CHAPTER 08_ Animation Framework과 State Machine


===== PAGE 276 =====
0Easing Curves
Animation 아이템이 시작 좌표부터 마지막 좌표까지 이동하는 경로를 진행 속도를 조절하여 움직임의
패턴을 변경할 수 있다．


1QAnimationGroup
Animation 아이템을 그룹화하기 위한 방법으로 병렬 형태의 QParallelAnim毗ionGroup과 QSe-
quentialAnimationGroup 클래스를 제공하며 QAnimationGroui) 클래스를 상속하도록 구현한다．


1AnimationZ State
State 入/lachine는 Finite State Machine이라고 하며 , ON/OFF 스위치와 같이 상태가 ON 또는 OFF
인 상태를 State, ON에서 OFF로 뱌뀌는 것을 행동 및 Transition이라 정의할 수 있다．
State Machine 모델링 기법을 구현할 수 있도록 QState, QSignalTrans代幻n 그리고 QEvent
Transition 클래스를 제공한다．



          1.1 Animation 아키텍처와 클라쓰

Anim毗ion Framework의 부모 클래스는 QtAbstractAnim毗ion이며, QVariantAnim毗ion과
QAnim毗ion(打아叩은 QtAbstractAnim毗ion 클래스를 상속받는다．
QPropertyAnim毗ion 클래스는 QVariantAnimation 클래스로부터 상속받는다. QOb昶ct와 같은 프
로퍼티와 QPropertyAnimation을 연결하므로 Anim毗ion 효과를 사용할 수 있다．



       01『
       QTransition
           0땐少 '1-I. addAnimationO
           玉1
                                              QAbctractA汕ilation    그
                I addTrancitionO
            .   1
         Qstate                    Animation計oup                    QVariantAnimation

                                        A


                                                                    『opertyAnima如n

                                                                                       111中
                                                            巨
                                                                         Qobject
                                                                I
                                                                ;    QGr카）hicsObject           ;

\
    QParallelAnimationGroup        QSecuenti出A川mat泊nGroup       I                  ·

                                                                                              II

（그림） Animation 다amew가k




                                                                                                   ] A미n冶lion 다ame小八rk과 S冶旭 Machine 275


===== PAGE 277 =====
1Anim졔ion 클래스

 함수                              설명
 QAbstractAnimation              모든 Animation 클래스의 부모 클래스
 QAnimationGroup                 Animation 그룹을 위한 추상화 클래스
 QEasingCurve                    Animation을 제어하71 위한 Easing curves
 QPar訓이AnimationGr이Jp            여러 Animation 그룹을 병렬로 처리
 OPauseAnimation                 QSequentialAnimation아ou口 중지 기능
 QPropertyAnimation              OO히ect 아이템에 Animation 기능을 추가
 QSequenti졔Anim帥onGroup          Sequential Anim계向n 그룹
 QVariantAnimation               Anim計ion을 위한 추상화 클래스
 OTim이mne                        애니메이션 진행 속도를 제어하기 위한 타임라인



0QAbstractAnimation
Timer와 TimeEvei此가 완벽하게 추상화되어 현재 시간, 애니메이션이 지속되는 시간, 애니메이션 효과
가 반복되는 Loop 카운트와 Animation의 상태를 위한 인터페이스를 제공하며 Animation의 start,
st아）, resume, pause 기능을 제공한다．

start( ), stop( ), resume( ), pause( ）는 Anin追tion을 시작, 일시 중지 그리고 중지를 하기 위한 함수
이고 duration( ) 멤버함수는 애니메이션이 지속되는 시간을 리턴한다. 지속 시간을 설정하는 set
I九ration( ) 함수는 QVariantAnimation 클래스에 구현되어 있다．

loopCount( ) 함수는 반복되는 Loop 카운트 값을 리턴하고 setLoopCount( ) 함수는 반복되는 Loop
카운트를 설정할 수 있다．

direction( ) 함수는 Anim毗ion의 현재 진행 시간이 증가하고 있을 때 0을 리턴하며, 그렇지 않고 현재
진행 시간이 감소하고 있을 때 1을 리턴한다. direction( ) 함수가 리턴하는 Direction 상수는 다음과
같다．

 상수                                값      설명
 QAbstractAnimation::Forward              Anim계ion의 현재 진행 시간이 증가하고 있을 때 0을 리턴
 QAbstra아Animation::E治ckward        ]     현재 진행 시간이 감소하고 있을 때 ］을 리턴


setDirection( ) 함수는 진행 방향을 설정할 수 있다．
  0 （呂tart)
                                                  duration (end)
                                                                   >   七I코te


                                                    ]
  4L
                        loop 4
（그림） Time Line



currentTime( ) 함수는 Animation의 현재 진행 시간을 리턴하고 setCurrentTime( ) 함수는 현재 진
행 시간을 설정할 수 있으며 단위는 밀리세컨드를 인자로 지정할 수 있다．



276 CHAPTER 08小 Animation 다amewo水과 텨a也 Machine


===== PAGE 278 =====
彷QVariantAnimation
QVariantAnim毗ion 클래스는 Animation을 위한 추상화 클래스로써 Animation 아이템과 속성을 위
한 Base 클래스이다. Anim毗ion 요소로 지정된 QObject 아이템 등과 같은 Anim毗ion의 시작 지점과
Animation의 마지막 지점을 setStartValue( ）와 setEndValue( ) 함수를 통해 지정할 수 있는 기능을
제공한다. 좌표값이 변경되었을 때 이벤트를 발생하기 위해 valueChanged( ) 시그널 이벤트가 제공
된다．

Anim毗幻a 아이템의 easingCurve 설정값을 리턴하거나 설정하는 기능이 구현되어 있다. 이 기능은 시작
좌표부터 마지막 좌표까지 이동하는 패턴（또는 보간법）으로 easingCurve(）는 현재 설정된 보간법을 리턴
하고, setEasingCurve( ) 함수는 시작 좌표부터 마지막 좌표까지 이동하는 보간법을 설정할 수 있다．




       Linear             InQuad
（그림） easingCurve



그림에서 보는 것 이외에도 다양한 보간법을 제공한다．


0OPropertyAnimation
QPropertyAnimation 클래스는 타깃이 되는 QObject 아이템과 클래스의 생성자를 이용해 타깃과 프
로퍼티를 지정할 수 있다．

 QPushButton *btn = new QPushButton ( "Buttori", this) ;
 btn->setGeometry (10, 10, 100, 30) ;


 QPropertyAnimation * animation;
 II Aninia七ion 의 타겟이 될 버튼 지정
 animation = new QPropertyAnimatiom(btn, nge（그me七ry", thi引 ;


 anima七如n->setDuration (3000) ; // 3초（단위 밀리세컨드）
 animation->setStartValue (QRect (10, 10, 100, 30) ); // 시작 좌표
 animation->setEmdValue (QRect (200, 150, 100, 30) ); I/ 끝나는 좌표


 amimation->start () ;



setDuration( ) 함수는 Anim毗ion 아이템이 시작하囚 끝나는 지점까지 이동할 때까지의 시간을 지정하
며, 단위는 밀리세컨드이다. setDuration( ) 함수를 사용하지 않으면 디폴트 값으로 250 밀리세컨드 값
이 설정된다．


                                                       1_Animation Framework과 State Machine 277


===== PAGE 279 =====
setStartValue( ) 함수는 Animation의 시작 좌표를 설정하며 setEndValue( ) 함수는 Animation이
이동하는 마지막 좌표를 설정할 수 있다. 마지막 라인의 start( ) 함수는 시작 좌표부티 마지막 좌표까지
지 정한 시간 동안 Animation을 시작하기 위한 함수이다．




（그림） Anim計向n 타깃 QPushButton 이동



簪QEasingCurve
QEasingCurve 클래스는 Anim毗ion의 easing curve를 제어하기 위해 제공되는 클래스이다．
QVariantAnim毗ion 클래스의 프로퍼티로 제공하기 위한 목적으로 주로 사용되며 , Anim毗ion 아이템이
시작 좌표부터 마지막 좌표까지 이동하는 경로 진행 속도를 보간하여 움직 임의 패턴을 변경할 수 있다．

valueForProgress( ) 함수는 小1 사이의 범위에서 움직임의 진행 시간을 리턴할 수 있다. 시간 t를 첫
번째 인자로 넘겨주면 setDuration( ) 함수에 의해 지정한 시간을 t어］ 해당하는 진행 시간을 밀리세컨드
로 리턴한다．

 QEasingCurve easing(QEasingCurve: :InOutQuad) ;

 for (qreal t = 0.0; t < 1.0; t+=0.1)
 {
      qDebug() << n Effective progress " << t << " is "
               << easing.valueForprogress (t) ;
 }
 // ［켤과］
 // Effective progress 0 is 0
 // Effective progress 0.1 is 0. 02
 II Effective progress 0. 2 is 0. 08
 II Effective progress 0. 3 is 0.18
 II Effective progress 0. 4 is 0. 32
 I! Effective progress 0. 5 is 0. 5
 // Effective progress 0. 6 is 0. 68
 I! Effective progress 0. 7 is 0. 82
 II Effective progress 0. 8 is 0. 92
 II Effective progress 0. 9 is 0. 98
 II Effective progress 1 is 1




278 CHAPTER 08_ A미ma的n 다amework과 State Machine


===== PAGE 280 =====
valueForProgress( ) 함수의 첫 번째 인자의 값은 小1 범위의 qreal 데이터 타입값을 인자로 설정해야
한다．

QPropertyAnimation *anirnation = new QPropertyAnimation(item, "opacity ' ) ;
animation->setEasingCurve (QEasingCurve: : InOutSine) ;



Animation 아이템이 움직이는 진행 STEP 小1 사이의 값과 시간을 보간하여 움직임을 변경할 수 있는
패턴을 setEasingCurve( ) 함수를 이용해 지정할 수 있다．

QEasingCurve: :InOutSine 상수값 이외에도 Qt에서는 다양한 패턴을 지정할 수 있으며 , 상수값으로
제공하는 보간된 패턴은 다음과 같다．

value             (1, 1)    value   1             (1 1)     value   1                 (1 1)    value




             progress               I           progress                            口rogress                  progress

        InCubic                             OutCubic                    InC山tCubic                        OL川nCub吃


value             (1, 1)    value                 (1 1)     value 1                   (1 1)    value             (1 1)




             口rog ress                          口rog ress                           progress                   F가ogress

        InQuad                              OutQuad                         lnOutQuad                     OutlnQuad


                  (l, ])    vs山el                 (1 ])     \／톄ue                     (1, 1)   value             (1 1)
                                                                               ／그
             口rog ress                          口rogress                            口rogress                   progress

        InQuart                             0내Quart                         ln0utQuart                     OutinQuart


                   (1 1)     value                 (1 1)     value 1                   (1 1)     value           (1 1)




              progress                           progress                            口rc그gress                 미ogress

        InBounce                            OutBounce                       mO마Bounce                     OutlnBounce


                    (1 1)    value      1          (1, 1)    value      1              (1 1)     value            (1, 1)




              口rog ress                          口rogress                            口rogress                  口rogress

        lnOut(그미nt                          OutlnQuint                      InOutO내nt                     OL川nQuint




                                                                                                         1 Animation 다ame叭幻水과 State Machine 279


===== PAGE 281 =====
 value               (1 1)    value                                           (] ])    va山e               (1 1)




                  口rogress                                                  口rogress
         InSine

 va山e                (1. 1)   \／졔ue                                           (1 1)    value




                  progress                                                  progress



 value               (1. 1)   value                                           (1 1)    value




                  progress                   progress                       progress                   progress
         lnCirc                       OutCirc                                                  OL川n（긔rc


 value              (1, 1)    value 1/ \ 4      (1 1) value I           A     (1 1)    value
                                                                                               1



                     gress                   progress           I     V progress                       progress
         InElastic                    Out日astic                     InO내日astic                     Outln티astic

＼罔山e               (1. 1)     value             ] 1)    value                 ] 1)     value




              口rogress                       progress                       progress                   progress
         InBack                       OutBack                       InOutBack                  OutlnBack


setEasingCurve( ) 함수로 easing curve를 지정하지 않으면 디폴트 QEasingCurve::Linear가 설정
된다．

 Widget: :Widget ( QWidget *parent) : QWidget (parent)
 {
       resize (300, 220) ;
       QPushButton *btn = new QPushButton ( "Button", this) ;
       btn->setGeometry (10, 10, 100, 30) ;


       II Animation 의 타겟이 될 ｝北n 지정
       animation = new QPropertyAnimation (btn, "geometry", this) ;


       anima七i이卜＞se七D吐a七ion(2000) ; /1 2초（단위 밀리세컨드）
                                                                                                                  0


280 CHAPTER 08_ Animation Framework과 State Machine


===== PAGE 282 =====
                animation->se七S七ar七Value (QRec七（10, 10, 100, 30) );               // 시작 좌표
                animati이i->setEndValue (QRec七（200, 150, 100, 30) ); I/ 끝나는 좌표


                QEasingCurve easing(QEasingCurve: :In0utQuad) ;
                for (qreal t = 0.0; t < 1. 0; t+=0.1)
                {
                       qDebug() << "Effective progress " << t << " is "
                                   << easing. valueForPr야拉ess (t) ; II Mapping 되는 시간 리턴
                }
                anilnati이卜＞se七EasingCurve (easing) ; // easing curve 설정
                connect (btn, SIGNAL (clickedU) , this,          SLOT (btneclicked() ));
         }

         void Widget: :btnclicked ()
         {
                animation->start () ;
         }


QEasingCurve 생성자의 인자로 easing curve를 지정하고 setEasing（노rve( ) 함수를 사용해 easing
curve를 설정할 수 있다．




（그림）（正asingCurve를 사용한 예제 실행 화면



I QAnimationGroup
QAnimationGroup은 Animation 아이템을 그룹화하기 위해 제공되는 추상화된 클래스이다．
Anim毗ion 아이템을 그룹화하기 위한 방법으로 병렬 형태의 QParallelAnim毗幻n(打아叩과 QSequen
-tialAnimationGroup 클래스를 제공하며, QAnimationGroup 클래스를 상속하도록 구현되어 있다．

/6Seq.              帥ti히Animati帥Gro叩

                                       QparallelAnimationGroup
                                         Animation 아아템            Anima卄on 아이 템
             An油at油n 아이 템      나
                                         Anirnat沁nO卜：)i 털1
\\
（그림） OPar쉐回AnimationGroup과 QSequenti졔Anim欲山n（計ou口 클래스


                                                                           1_Animation Framework과 State Machine 281


===== PAGE 283 =====
  Widget: :Widget (QWidget *parent) : QWidget (parent)
  {
      resize (320, 270) ;
      QPushButton *btnl = new QPushButton ( "First ", this) ;
      btnl- >setGeometry (10, 10, 100, 30) ;


      QPushButton *btn2 = new QPushButton ( "Second", this) ;
      btn2->setGeometry (10, 45, 100, 30) ;


      animi = new QPropertyAnimation( btnl, "geometry") ;
      animl->se七1沁ra七ion (2000) ; // 2초（단위 밀리세컨드）
      animl->setStartValue(QRect (10, 10, 100, 30) ); II AI작 좌표
      animl->setEndValue(QRect (200, 150, 100, 30) ); I/ 끝나는 좌표


      anim2 = new QPropertyAnimation (btn2, "geometry ") ;
      anim2->se七Dura七ion(2000) ; II 2초（단위 밀리세컨드）
      anim2->setS七ar七Value (QRect (10, 45, 100, 30) ); // 시작 좌표
      anim2->setEndValue (QRect (200, 195, 100, 30) ); I/ 끝나는 좌표


      sGroup = new QSequentialAnimationGroup; II Sequential Group
      sGroup->addAnimation ( animi) ;
      sGroup->addAnimation ( anim2) ;


      //pGroup = new QParallelAnimationGroup; // Parallel Group
      /IpGroup->addAniniation(animl) ;
      //pGroup->addAnimation(anim2) ;

      connect (btnl, SIGNAL(clickedO) , this, SLOT (btnclicked ( ) ));
      connect (btn2, SIGNAL(clickedO) , this, SLOT (btnclicked ( ) ));



 void Widget: :btn_clicked()
 {
      sGroup->start ( QPropertyAnimation: : DeleteWhenStopped) ;
      I /pGroup->start ( QPropertyAnimation: : DeleteWhenStopped) ;




소스 코드에서 두 개의 QPushButton 위젯을 GUI 상에 배치하고, addAnimation( ) 멤버함수를 이용
해 Anim毗ion 아이템을 그룹에 등록한 후 버튼을 클릭하면 start( ) 함수가 호출된다. Sequential
Group으로 지정된 첫 번째 QPushB毗ton의 Animation이 동작한다. 동작이 완료된 다음에 두 번째
QPushButton의 An油ation이 동작한다．

주석 처리된 소스 코드는 Parallel Group（병렬 그룹）으로 설정된 애니메이션 아이템을 동작시킨다，
Sequential은 순차대로 Anim毗ion 아이템이 실행되지만 Parallel Group어］ 등록된 QPushBut切n의
Animation이 동시에 실행된다．




282 CHAPTER 08_ Animation FrameworkF State Machine


===== PAGE 284 =====
QSequenu川Anim玔onGroup                                      QparaflelAnimotionGroup
!j


     !    Ffrst   1   ,   .


                                \.
         Second




                  "
                      "，      李차싶행   ' "'   \.   .   (1)




                                            ' 뇨까‘" J姓芬＝訂
（그림） Sequential Group과 Parall이 （計oup



이전 예제와 달리 start( ) 함수에서 Policy를 사용할 수 있는데, Animation 인스턴스가 생성될 때 메모
리를 사용하게 된다. 따라서 start( ) 함수의 인자로 Deletion Policy 상수값을 지정하면 Animation이
완료되었을 때 메모리에서 자동으로 소거할 수 있다．

 상수                                                                  값      설명
 QAbstra아Anim訓on::KeepWhenStop口ed                                           Animation 아이템의 동작이 완료되어도 메모리를 남아있도록 설정
 QAbs卄a아A데mation::D이eteWhenStopped                                          Anim計ion 아이템의 동작이 완료되면 메모리에서 자동으로 소거됨




         tj十 Animation과 State Machine
Animation 아이템을 setStartValue( ）와 setEndValue( ）를 이용해 시작 좌표와 마지막 좌표를 설정
하는 방식으로 Animation 동작을 구현했다. 만약 ON/OFF와 같이 디폴트가 ON 상태에서 OFF로 바뀌
게 되면 QPushButton 아이템을 setStartValue( ) 함수로 지정한 좌표에서 setEndValue( ) 함수로 지
점한 좌표까지 Animation을 동작시키고, 다시 OFF/ON 상태로 바뀌면 QPushButton을 마지막 좌표
에서 시작 좌표로 Animation을 동작시켜야 한다면, 이전에 배운 것과 같이 QPropertyAnimation을
사용해 구현하거나 QAnimationGroup을 이용해 구현할 수 있다．

하지만 구현해야 하는 Animation 아이템이 하나 이상 또는 수십 개의 Animation 아이템이 있다고 가
정했을 때 구현 난이도가 매우 복잡해질 수 있다. 예를 들어 수십 개의 메뉴 아이템 중 하나의 아이템을
애니메이션을 처리한다고 가정해 볼 수 있다. 하나의 아이템이 활성화되었을 때 이전어｝ 활성화된 아이템
을 배치된 수십 개의 아이템과 같이 비활성화 상태로 복퀴시키도록 상태를 변경해야 한다. 따라서 구현이
매우 복잡해 질 수 있다．

예를 들어 설명한 것과 같이 아이템을 순차적으로 Animation 아이템이 동작하는 방식이 아닌 Anima-
tion 아이템을 State Machine 모델링 기법을 적용하면 매우 쉽게 구현할 수 있다．




                                                                                     ] Animation 다amev四rk과 S怡怡 Machine 283


===== PAGE 285 =====
                                  행동（Transition) 혹은 이벤트




              （가뇌                                           liFE
                    Fj                                    IS TAT 타




                                  행동（Transition) 혹은 이벤트
    （그림） State Machine 모델링 기법



    State Machine을 좀더 정확하게 말해 Finite State 八4achine으로, ON/OFF 스위치와 같이 ON 또는
    OFF인 상태를 State, ON에서 OFF로 바뀌는 것을 행동 또는 Transition이라 정의할 수 있다．

    지금까지 설명한 State Machine 모델링 기법을 구현할 수 있도록 QState, QSignalTransition 그리
    고 QEventTransition 클래스를 제공한다．



       QI『낀땐브－} """' "'" '띤
                          ：可 QAbst『耐A.岫ation
          r
                                                                     r                   11




                                                                          QPropertyAnimation
                                                                                         1
                                                                                         1
               addTransition()                                                          立
                                                                         r1 1 1
                                                                                                    \1111/
          上                                                                          Qobject

                         1 11 J
                                                                                  QGraphicsObject
        Qstate                                                           1

（그림） QTransition 클래스와 QAbstra아A이m帥on 클래스 관)카



    버튼의 시작 위치를 state-i , 버튼을 클릭해 Anim毗ion 동작이 완료된 상태를 state-2라고 정의하고
    버튼이 state-i에서 state-2로 바뀌는 행동을 transition-i, state-2에서 state-i로 바뀌는 행동을
    trai娼iti이느2라고 정의했을 때 제공하는 QState와 Q罰얍ia1Transition을 사용해 구현할 수 있다．


    resize (360, 290) ;

i   QI七shBu七七on 火bu七七（Dn = new QPushBu七ton ( " Bu七ton", this) ;
    button->setGeometry (10, 10, 100, 30) ;


!QStateMachine *machine = new QStateMachine;
!
1QS七a七e 出sta七el = new QS七ate (machine) ; // S七a七e-1
!statel- >assignProperty (button, "geometry ", QRect (10, 10, 100, 30) );
 machine->se七InitialS七a七e          ;         (sta七el)
                                                                                                             0

284 CHAPTER 08_ Animation Framework과 State Machine


===== PAGE 286 =====
QState *state2 = new QState (machine) ; II state-2
 state2->assignProperty (button, "geometry ", QRect (250, 250, 100, 30) );


QSignalTransition *transitioni                      = statel- >acldTransition(button,
 SIGNL(c1icked() ), state2) ; // transition- i
 transitioni- >addAnimation(new QPropertyAnirnation(button, "geometry") );


QSignalTransition *transition2 = state2->addTransition(button,
 SIGNAL (ciicked(fl,                   statei) ; // transition- 2
 transition2- >addAnimation(new QPropertyAnimation(button, "geometry ") );


machine->startt ) ;



QStateMachine 클래스의 State 八4achine 모델링 기법을 적용하기 위한 인스턴스이며 QState 클래스
생성자어］ 첫 번째 인자로 지정한다. QState 인스턴스 state卜1인 타깃 QPushB毗on을 assign
Property( ) 함수를 이용해 지정할 수 있다．

assignProperty( ) 함수 첫 번째 인자는 QPushB毗ton의 인스턴스를 지정하고 서］ 번째 인자에 QPush
Button 좌표와 크기를 QRect( ) 함수를 통해 등록한다. state띱 또한 state-i과 같은 방식으로 등록할
수 있다．

state-i에서 state-2로 바뀔 때 Transition을 등록하기 위해 addTransition( ) 함수를 사용할 수 있
다. addTransition( ) 함수의 첫 번째 인자로 버튼 위젯을 명시하고, 두 번째 인자는 버튼 클릭 시그널
을, 세 번째1 인자는 변경할 State를 지정할 수 있다. 동일한 방식으로 두 번째 Transition을 소스 코드어］
서 보는 것과 같이 구현할 수 있다．



     Bu如n          State - 1
               \
               1
               \
               1




                    "' .   " . Tran쉬t向n -1


         Transition - 2 N




                               ＄奴te-        2!   跏如n    1   J




（그림） State Machine 모델링 기법을 사용한 예제



지금까지 State Machine 모델 기법을 Anim毗ion Framework에 적용하기 위한 방법에 대해 살펴보았
으며 제공하는 Animation Framework를 사용해 어플리케이션을 작성하는 경우 State Machine도 함
께 사용한다. 그만큼 Animation을 제어하기 위한 구현의 복잡성을 단순화시킬 수 있다．


                                                                         1 Animation Framework과 State Machine 285


===== PAGE 287 =====
        노       노J
            1
            )   ,    '1   i   }   1   A   )   ft


M2vio
            /


===== PAGE 288 =====
CHAPTER




          Thread


===== PAGE 289 =====
01 5 Programming




r尸1 ' Thread
          （값는 Thread를 제공하기 위한 AP로 QThread를 사용한다. 따라서 QThread가 제공하는 API 사용
          법에 대해 알아보도록 하자．




Qt에서는 멀티 태스킹을 위해 QThread 클래스를 제공한다. Qt에서 제공하는 쓰레드는 멀티 태스킹과
같이 하나의 프로세스가 하지 못하는 일을 대신해출 수 있다. 예를 들어 네트워크 어플리케이션에서 다중
접속자를 처리하기 위해 쓰레드를 사용할 수 있다．

QThread는 QObject 클래스로부터 상속받아 구현되어 있으며 동기화를 위해 QMutex 클래스를 제공한
다. 쓰레드와프로세스가 공유하는 글로벌 변수에 값이 변경되는 것을 동기화 하기 위해 뮤텍스小血te功
를 사용할 수 있다. 예를 들어 채팅 프로그램에서 새로운 접속자가 생기거나 연결이 닫히는 경우 접속된
사용자 카운트 값을 변경하는 순간에 다른 프로세스가 카운트 값을 참조하게 되면 네트워크 접속 사용자
간에 잘못된 데이터를 전달할 수 있다. 따라서 글로벌 데이터를 변경해야 하는 경우 M毗ex를 사용해 다
른 프로세스가 값을 변경하지 못하거나 참조할 수 없도록 동기화할 수 있다．


1QThread 생성과 시작

 class MyThread : public QThread
 {
      Q OBJECT
 protected:
      void run( );
 };

 void MyThread: :run( )
 {

 }


예제 소스 코드에서 보는 것과 같이 쓰레드를 생성하기 위해 QThread 클래스로부터 상속받아야 하며
八4yThread는 run( ) 멤버함수를 이용해1 쓰레드를 구현할 수 있다．




288 CHAPTER 09_ Thread


===== PAGE 290 =====
I （값에서 제공하는 쓰레드 클래스

클래스                   설명
QAtomi이ft             Integer 상에서 플랫폼의 독립적인 /\tomic 연산을 제공
QAtomicPointer        포인터 상에서 Atom允 연산을 제공하71 위한 템플릿 클래스
QFuture               비동기 계산 결과를 나타내는 클래스
QFutureSynchronizer   QFuture 클래스는 동기화를 단순화하71 위해 제공되는 클래스
QFutur이Natcher        시그널과 슬롯을 사용해 QFu山re의 모니터링을 허용하는 클래스
QMutex                클래스 사이의 동기화에 접근
QMutexLocker          Lock과 Unlock 叭flex를 단순화하71 위한 클래스
QReadWriteLock        Read와 Write를 제어하71 위한 클래스
QReadLocker           Read 접근을 위해 Read-Write Lock과 Unlock을 간단하게 사용하71 위한 클래스
QWriteLocker          Write 접근을 위해 Read-Wri伯 Lock과 Unlock을 간단하게 사용하71 위한 쿨래스
QRunnab陀              동작하고 있는 모든 오브젝트를 위한 부모 클래스이며 \,irtual 함수인 run( ) 함수가 정의되어 있음
QSemaphore            일반적인 Count 뮤텍스 클래스
Qihread               플랫폼의 독립적인 쓰레드 기능을 제공하는 클래스
QlhreadPo이            쓰레드들을 관리하71 위한 클래스
QThreadStorage        쓰레드당 스토리지 영역을 제공하는 클래스
OW톄tCondition         쓰레드들간 동기화를 위한 클래스 상태 값을 확인하기 위한 클래스



I QThread 동기화를 위한 클래스
Qt에서는 쓰레드 동기화를 위해 QM毗ex, QReadWriteLock, QSemaphore 그리고 邸VaitCondition
클래스를 제공한다. 주요 쓰레드가 다른 쓰레드로부터 중단을 기다리는 상황에서 동기화가 필요하다. 여］
를 들어 두 개의 쓰레드가 동시어］ 공용변수를 Access 한다면 예상할 수 있는 결과를 얻지 못할 것이다．
따라서 두 개의 쓰레드가 공용변수를 사용해야 한다면 동기화가 필요하다．

QM毗ox는 하나의 쓰레드가 특정 공용변수를 Access 하는 동안 다른 쓰레드가 접근할 수 없도록 잠금
장치와 같은 기능을 제공한다. 공용변수에 M毗ex가 활성화된 상태에서는 쓰레드들이 동시에 접근할 수
없으며 먼저 접근한 쓰레드가 공용변수 Access 작업이 완료되면 다른 쓰레드가 접근할 수 있다．
만약 하나의 쓰레드가 M毗ex로 잠금 장치가 걸려 있는 공용변수에 Access가 하고 있는 동안 다른 쓰레
드가 동일한 공용변수에 접근하면 Access가 완료될 때까지 Sleep하게 된다. 이것은 Thread safety라
고 한다．

QReadWriteLock은 帥血tex와 동일하다. 차이점은 Read와 Wri扼를 구분해 데이터어］ Access 할 수
있다. 많은 쓰레드가 공용변수 Access가 빈번히 발생할 때 帥ilutex 대신 QReadWr此eLock을 사용하
면 유용하다．

QSemaphore는 정확한 숫자어］ 의해 식별이 된 여러 개의 리소스를 QM毗ex와 같은 동기화 기능을 제
공한다. QM毗ex는 정확히 하나의 리소스를 관리하지만 QSemaphore를 이용하면 번호로 식별화된 여
러 개의 리소스를 관리할 수 있다．

QWaitCondition은 조건에 부합할 때, 쓰레드가 Wake-Up 될 수 있도록 허용한다. 예를 들어 여러 개


                                                                          1 Thread 289


===== PAGE 291 =====
 의 쓰레드 중 하나가 Blockir培된 상태에서 QWaitCondition 클래스가 제공하는 wakeOne( ) 함수 및
 wakeAll(）을 통해1 블로킹된 쓰레드를 Wake-Up 할 수 있다．


 S Reentrancy2F Thread-Safety
Reentrar兀y 두 개 이상의 쓰레드가 병렬로 접근했을 때 호출될 순서어］ 상관없이 실행 코드가 겹쳐서 실행
 되더라도 결과는 보장되어야 한다는 것을 의미한다. Thread-Safety는 병렬로 쓰레드가 동작하는 상황에
 서 프로그램이 정상적으로 동작할 수 있는 결과를 보장하지만 정적 공간（static）이나 공유（heap과 같은 메
모리 객체） 객체들을 접근할 때 뮤텍스（M毗ex）와 같은 매커니즘을 사용해 보장하는 것을 의미하다．
Reentrancy는 C++ 클래스와 비슷하다. 단지 자신이 소유한 데이터 변수 영역만 Access하기 때문어］ 두
개 이상의 쓰레드가 접근하더라도 안전성을 보장한다．

1class Counter
  {
 publi（그:
      （幻un七er ( ) { n = 0;   }

      void increnient () { ++n; }
      void decrement () { --n; }
      mnt value() const { return n; }


 private:
      mnt n;
 };


소스 코드에서 선언한 n 변수는 Counter에서만 접근할 수 있는 변수이며 increment ( ) 함수와
decrement( ) 함수를 통해서만 n 변수에 접근할 수 있다. 이 클래스의 II은 공용변수 영역이 아니므로 두
개 이상의 쓰레드가 접근하더라도 안전성을 보장한다．

Thread寸Safety는 두 개 이상의 쓰레드가 공용변수에 병렬로 접근하더라도 안전성을 보장하는 것을 의
미한다. 앞의 예에서 살펴본 Counter 클래스의 n 변수가 공용변수라면 두 개 이상의 변수가 접근했을
때 안전성을 보장하기 위해 QM毗ex를 사용해야 한다．

 class Counter
 {
 恥blic:
      Counter () { n = 0; }


      void increment () { QMutexLocker locker (&mutex) ; ++fl; }
      void decrernent ( ) { QMutexLocker locker (&mutex) ; --n; }
      mnt value () const { QMutexLocker locker (&mutex) ; return n; }

private:
      mutable QMutex mutex;
      mnt n;
 };


290 CHAPTER 09_ Thread


===== PAGE 292 =====
帥4utexLock 클래스는 八4utex의 Lock을 생성자에서 자동으로 설정하고 함수 마지막인 소멸자가 호출
되면 자동으로 UnLock 된다．


0QThread와 QObjec怡
QThread는 QObject 클래스로부터 상속받은 클래스이다. 그렇기 때문어］ 쓰레드가 시작하거나 종료되었
을 때 Emit 시그널 이벤트를 발생하는 기능을 제공한다. 시그널 슬롯 기능은 QThread가 QObject 클래
스로부터 상속받은 기능이며 시작과 종료 등과 같은 처리를 시그널 슬롯으로 처리가 가능하므로 멀티 쓰
레드 구현이 가능하다. QObject는 QTimer, QTcpSocket, QUdpSocket 그리고 QProcess와 같은
non-GUI 기반의 하위 클래스이다．

non-GUI 기반의 하위 클래스는 쓰레드가 없이 동작한다. 단일 클래스가 어떤 기능을 실행하기 위해서
는 쓰레드가 필요하지 않다. 하지만 단일 클래스의 오브젝트를 실행하는 상위 기능은 쓰레드로 구현해야
한다．

예를 들어 사용자의 종료 이벤트가 발생하기 전까지 어플리케이션이 종료가 안된다면 어플리케이션의 메
인 부분은 쓰레드 이벤트 루프가 필요하다. 따라서 어플리케이션 메인 부분은 쓰레드 이벤트 루프를 통해
사용자 이벤트를 기다리도록 다음과 같이 설계해야 한다．

                                                                 /;1尸／   H叫＼   \




       Thread A              Main Thread
                                        回口
                        回a
       <：   二：
      a什road::e肥아）
                  ::>         ＜二：      >
                            QA야川C帥On 0000{ ,
                                                                                   0th tO


                 （쯔 그   ［璽乙                    ..   a   (;   .
                                                                   回미

（그림） 메인 Thread



 in七 rnain(int argc, char 火arg町 ] )
 {
      QApplication a (argc, argv) ;
      Widget w;
      w. show ( );


      return a. exec ( );




소스 코드는 GUI 기반의 Qt 어플리케이션의 메인 부분이다. 사용자의 종료 이벤트가 발생하기 전까지
어플리케이션은 Thread Event Loop를 통해 계속 동작한다. 이와 마찬가지로 쓰레드 기능을 추가할 때
별도의 쓰레드 매커니즘을 통해1 메인 부분과 분리될 수 있도록 쓰레드 기능을 추가해야 한다．

그렇다면 메인 쓰레드는 어떻게 정의할 것인가의 문제가 남는다. 메인 쓰레드는 그림에서 보는 것과 같이
Thread A와 Thread B 인스턴스를 초기화하거나 시작하는 클래스가 메인 쓰레드가 되도록 설꼐해야
한다．

그리고 메인 Thread A와 Thread B가 종료되지 않은 상황에서 메인 쓰레드 이벤트 루프가 종료되지 않


                                                                                            1 Thread 291


===== PAGE 293 =====
도록 설계해야 한다. 예를 들어 Thread A가 쓰레드를 종료되기 전에 메인 쓰레드 이벤트 루프가 종료되
면 Thread A와 Thread B가 처리하는 루틴의 안전성은 보장할 수 없다. 따라서 메인 쓰레드 루프는 하
위의 모든 쓰레드가 종료되고 마지막에 종료될 수 있는 견고한 멀티 쓰레드가 필요하다．

또한 예상하지 않은 결과로 인해 Thread A가 종료되지 않아 메인 쓰레드 루프가 종료되지 않는다면 어
플리케이션 전체 안전성은 보장할 수 없다. 따라서 쓰레드가 일정 시간 이내에 종료되지 않는 예외상황에
대해 처리할 수 있도록 안전성을 보장해따 한다．


S Thread 처리를 위한 시그널 슬롯의 타입
Qt는 쓰레드 환경에서 적합한 이벤트 처리를 위해 시그널 슬롯 타입을 결정할 수 있는 enum 타입을 지
원한다．

Constant                      Value Description
Qt::Aut000nnection            0     만약 시그녈이 다른 쓰레드에서 발생하면 시그널은 Queue에 삽입되며
                                    QueuedConnection과 같다. 그렇지 않으면 [)irectConnection과 같이 즉
                                    시 슬롯이 처리된다． Connection 타입은 시그널이 발생할 때 결정된다．
Qt::DirectConnedt ion         ]     시그널 이벤트가 발생하면 바로 슬롯이 응답한다．
Qt::QueuedConnection          2     받는 쓰레드의 이벤트 루프가 리턴될 때 슬롯이 발생한다. 슬롯은 받는 쓰레
                                    드에서 실행된다．
Qt::B幻ckingQueuedConnection         QueuedConnection과 같다. 슬롯이 리턴할 때까지 쓰레드가 미ocking 된
                                    다. 01 Conne에on 타입은 이벤트7F 발생하는 곳에서 사용하길 권장한다．


I 아Concurrent 클래스를 이용한 Concurrent 프로그래밍
QtConcurrent 클래스는 M毗ex, read-write locks, wait condition, semaphores 등과 같이 Low-
level 쓰레드를 사용하지 않고 멀티 쓰레드 기능을 제공한다. QtConcurrent를 사용해 작성한 프로그램
은 프로세스 수에 따라 사용하는 쓰레드의 수를 자동으로 조절한다. QtConcurrei此는 멀티코어 시스템
에서 동작하는 Qt 응용 프로그램 배포 시 확장하기 위한 목적으로 사용한다．

QtConcurrent 클래스는 공유 메모리（Shared-memory) 시스템의 MapReduce와 Filterl亡educe 구현
이 포함된 병렬 처리 스타일의 API와 GUI 기반의 어플리케이션에서 비동기 방식의 계산을 Mappir培하
기 위한 클래스가 포함되어 있다．



       ].] 0Thread 클래스

QThread 클래스는 플랫폼에 독립적이며 쓰레드를 구현할 수 있는 기능을 제공한다. QThread는 프로
그램 내에서 쓰레드를 관리하고 제어할 수 있는 다양한 멤버함수와 시그널 슬롯을 제공한다. QThread
클래스의 start( ) 멤버함수를 통해 쓰레드를 시작할 수 있다．




292 CHAPTER 09_ Thread


===== PAGE 294 =====
class Worker : public QObject
{
     Q OBJECT


public slots:
     void doWork () {


     }
};
void MyObject: :putWorkerlnAThread()
{
     Worker *worker = new Worker;
     QThread *workerThread = new QThread(this) ;


     connect (workerThread, &QThread: : started, worker, &Worker: :doWork) ;
     connect (workerThread, &QThread: :firiished
                                             r worker, &Worker: :deleteLater) ;
     worker->moveToThread (workerThread) ;


     II   Starts an event loop, and emits workerThread->started( )
     workerThread->start () ;




위의 코드 상에서 \Worker 클래스의 슬롯은 분리된 쓰레드가 시작할 때 발생하는 시그널과 쓰레드가 종
료되었을 때 발생하는 시그널과 연결되어 있다. 쓰레드가 시작하면 Worker 클래스의 doWork( ) 슬롯함
수가 호출된다．

즉, putWorkerlnAThread( ）의 start( ) 함수가 실행되면 쓰레드의 시작（QThread: :started) 시그널이
발생하고 connect( ) 함수에 의해 연결된 Worker 클래스의 doWork( ) 슬롯함수가 호출된다．
쓰레드가 종료되면 QThread::fjnjshed 시그널이 자동으로 발생한다. 이 시그널이 발생하면 Worker어］
서 사용했던 쓰레드 메모리 영역을 바로 해제한다．

QThread는 started(）와 如ished( ) 시그널 함수를 통해 시작되어 종료되는 것을 공지할 수 있고, 쓰레
드의 상태를 확인할 수 있다. isFinished( ) 함수를 사용해 쓰레드가 종료된 상태인지 , isRunning( ) 함
수를 사용해 쓰레드가 동작 중인지 확인할 수 있다. 또한 exit(), quit( ) 함수를 이용해 쓰레드를 종료할
수 있다．

Qt 4.8 버전부터 finished( ) 시그널 함수가 QObject: :deleteLater( ) 슬롯과 연결되어 있으면 쓰레드
가 종료되면 쓰레드가 할당한 메모리 영역을 해제한다．

멀티 쓰레드를 사용하면 모든 쓰레드가 종료될 때까지 기다려야 하는 경우가 있다. 호출한 쓰레드가 종료
될 때까지 기다리기 위해 wait( ) 함수를 사용하면 된다. 그리고 쓰레드 내어써 쓰레드를 second, milli
second 혹은 microsecond 단위로 쓰레드를 일시 중지시키기 위해서 sleep( ), msleep( ) 그리고
usleep( ) 멤버함수를 사용할 수 있다．


                                                                                  1 Thread 293


===== PAGE 295 =====
 QThread 클래스는 쓰레드에서 수행하길 원하는 동작을 위해 virtual 함수로 제공하는 run( ) 함수를 통
 해 재정의 할 수 있다. run( ) 함수 내에 쓰레드에서 동작하길 원하는 기능을 추가하면 된다. run( ) 함수
 내에 코드를 수행하기 위해서 start( ) 함수를 실행하면 자동으로 run( ) 함수가 호출된다．

  class AdvancedThread奴nager : public QThread
  {
 protected:
          void run()
          {
              /士 . . . other code to initialize      thread. .. 出／
              /7 Begin event handling
              execQ;
          }
      ;



위의 소스 코드에서 exec( ) 함수는 exit( ) 함수가 호출될 때까지 쓰레드가 종료되지 않고 대기 상태가
된다. 만약 quit( ) 함수를 경유해 exit( ) 함수가 호출되면 0을 리턴하고 쓰레드가 종료된다．

QThread는 사용하는 메모리 영역으로 쓰레드 내부 영역과 공유 메모리 영역으로 분리된다. 쓰레드의 내
부에서 사용하는 Register 영역은 쓰레드 내부에서만 공유할 수 있다. 그리고 공유 데이터 영역은 다른
쓰레드에서 접근할 수 있다．

                                            \                 \       //
                                                                                         \\


                               A Thread         B Thread                   C Thread
                               쓰레드 내부            쓰레드 내부                     쓰러匹 내부
                              Register 염역       Register 영역                Re口iSter 영역




  쁩胃          騶 騁                醫冒                醫                          醫
                                                                  \                      1




（그림） 쓰레드 Register오FStack 영역



위의 그림은 쓰레드 내부에서 사용하는 Re廓ster와 Stack 영역을 도시화한 그림이다. 쓰레드 내부에서
공유하는 영역은 다른 쓰레드에서 접근할 수 없지만 Stack 영역은 쓰레드간 공유할 수 있다. 따라서 다
중 쓰레드 구현 시 Stack 영역을 접근할 경우 M毗ex, Read-Write Lock 등과 같은 Thread-safety를
고려해야 한다．




294 CHAPTER 09_ Thread


===== PAGE 296 =====
      t1      멀티 쓰레드 프로그래밍
QThread는 단일 쓰레드 뿐만 아니라 멀티 쓰레드를 쉽게 구현할 수 있는 API를 제공한다. 쓰레드를 시
작하기 위해 run( ) 멤버함수를 제공한다. isRunning( ) 함수와 isFinished( ) 함수를 통해 쓰레드 동작
과 정지 상태를 확인할 수 있다．

class MyThread : public QThread
 {
      0 0BJECT
public:
      MyThread(int      num) ;


private:
      b（그（그1 threadStop;
      in七 nun山er;


public:
      void stop ( ) ;


protected:
      void run ( ) ;
 };


QThread 클래스로부터 파생된 MyThread 클래스 생성자의 num 변수는 현재 동작하고 있는 쓰레드를
확인하기 위해 선언한 변수이다．




                                                                   그
1NyThread: :MyThread( mnt num)
 {
      number = num;
 }


number 변수는 MyThread 클래스의 멤버변수로 선언되어 있으며 쓰레드를 확인하기 위한 매개체이다．

 void MyThread: :stop ()
 {
      七hreadS七아） = 七rue;
      qDebug ( "[ %d] Thread stop ", number) ;
 }


I뇨blic의 stop( ) 함수는 쓰레드를 정지하기 위한 함수이며 Thread를 정지하기 위해 threadSt야）변수
어］ true 값을 설정한다．




                                                            1 Thread 295


===== PAGE 297 =====
 void MyThread: :run()
 {
     threadStop = false;
     mnt i = 0;


     while ( 代hreadS如p)
     {
            qDebug( "[ %d] MyThread %d", number, i) ;
            i++;
            sleep ( 1) ;
     }
 }


쓰레드를 동작시키기 위한 run(）는 virtual 함수로써 start( ) 함수를 실행하면 run( ) 함수가 호출된다．

 void Widget: :btn_start ()
 {
     七hreadl->s七ar七（) ;
     thread2->start () ;




현재 쓰레드가 동작하거나 동작이 멈춘 상태를 확인하기 위해 QThread는 isRunning( ) 멤버함수와
isFinished( ) 멤버함수를 제공한다. 이 함수를 이용하면 현재 쓰레드의 상태를 확인할 수 있다．

 void Widget: : btn_isRunning()
 {
     if (threadl->isRunning() )
            qDebug( "[ l]   Thread is running") ;
     else
            qDebug( "[ lJ Thread is not running") ;




 void Widget: :btnisFinished ()
 {
     if (threadl->isFinished() )
         gDebug ( "[ l]     Thread Finish'1 ) ;
     else
         qDebug( "[ l}      Thread not Finish") ;




296 CHAPTER 09_ Thread


===== PAGE 298 =====
! Thread_Ex訂0이e口


渭
1
         MyThread 0
         Mymread 0
    [ 11 MyThread 1
    [2] MyThread 1
    [2] MyThread 2
    (1] MyThread 2
    (1] Thread stop
    [2] Thread stop
    [1] Thread is not running
    [2] Thread is not running
    [1] Thread Finish
'
    [2] Thread Finish

（그림） 멀티쓰레드 실행 화면



    小 QThread 시그널과 슬롯
QThread는 쓰레드가 시작되거나 끝날 때 , 시그널과 슬롯을 제공한다．

1QThread 시그널
    \／이d tinished( )         쓰레드 인스턴스가 수행이 종료되면 시그널을 발생
    void started( )          쓰레드 인스턴스가 시작되면 시그널을 발생
    void termin計ed( }        쓰레드 인스턴스가 끝나면 시그널을 발생


[9Thread 슬롯
    \／이d quitO                                        쓰레드 수행 종료 SLOT
    void start (Priori如 priority = InheritPriority)   쓰레드 시작 SLOT
    void terminate()                                  쓰레드 종료 SLOT



     Widget: :Widget (QWidget *parent) : QWidget (parent)
     {
          threadi = new MyThread(1) ;
           thread2 = new MyThread(2) ;


           connect (threadl, SIGNAL(stop() ), this, SLOT (slot stoped) );
     }

     void Widget: :slot_ stoped()
     {
           qDebug( "Thread started") ;
     }



     [11 MyThread 2
     [2] MyThread 2
     [2] MyThread 3
     [1] MyThread 3
     [1] Thread stop
     [2} Thread s乞아）


（그림） sto口（) 시그널과 슬롯 예제 화면


                                                                            1 Thread 297


===== PAGE 299 =====
 S QThread 우선순위
 QThread는 멀티쓰레드간 set田or此y (Priority priority) 함수를 통해 우선순위를 부여할 수 있다．

 상수
 QThread::ldlePriority
                                   값   설명
                                       쓰레드가 동작하지 않고 있을 때의 상Efi
                                                                   1
 QThread::LowestPriority               LowPriority 보다 낮은 우선 순위
 0Th read::LowPriority             2   Norm톄Priority 보다 낮은 우선 순위
 QThread::NormalPriority           3   네ghPriority 보다 낮은 우선 순위
 Qlhread::H ighPriority            4   네ghes卄거ority 보다 낮은 우선 순위
 QThread::HighestPriority          5   가장 우선 순위가 높은 상태
 QThread::TimeCriticalPriority     6   플랫폼 상태에 따라 가능한 한 스케줄 상태
 olhread::InheritPriority          7   쓰레드 생성시 디폴트 값 우선 순위




               Thread Wait Condition
이전 예제에서 멀티 쓰레드를 사용하는 방법을 살펴보았다. 이번 장은 쓰레드 \Wait Condition을 구현하
는 방법에 대해 살펴볼 것이다. 어플리케이션에서 여러 개의 멀티 쓰레드가 실행될 때, 어떤 쓰레드가 먼저
실행되고 나중어］ 실행되는지 보증할 수 없다. Wait Condition은 쓰레드간 동기화를 목적으로 사용된다．

예를 들어 어플리케이션에서 두 개의 쓰레드가 동시에 실행된다고 가정해 보자. 첫 번째 쓰레드는 1초 간
격으로 1씩 증가한다. 두 번째 쓰레드는 첫 번째 쓰레드가 1씩 증가할 때까지 대기한다. 즉, 첫 번째 쓰레
드가 1씩 증가하고 이벤트를 두 번째 쓰레드에게 전달할 때까지 두 번째 쓰레드는 대기한다. 만약 첫
                                                                       번
째 쓰레드에서 1을 증가하고 두 번째 쓰레드에게 이벤트를 공지하면 증가한 값을 화면상에 출력한다．

위와 같이 쓰레드 간의 동기화를 위한 목적으로 \Wait Condition을 사용한다. Qt에서는 \Wait Condi-
tion을 제공하기 위해 QWaitCond此ion 클래스를 제공한다．

印WaitC아iditi아I 클래스는 쓰레드가 다른 쓰레드에게 특정 조건이 부합될 때까지 Block Waiting 모드
로 진입하기 위해 wait( ) 함수를 사용할 수 있다. 그리고 미ock Waiting 상태로부터 깨어나기 위해
waitOne( ) 혹은 waitAll( ) 함수를 사용하면 된다．

邸WaitCondition은 쓰레드에서 뮤텍스（Mu扼功와 함께 사용한다. 예를 들어 어플리케이션이 동작 중어］
사용자 특정 키를 입력했을 때 대기중인 쓰레드가 동작하도록 하기 위해 쓰레드 run( ) 함수에 다음과 같
이 소스 코드를 작성할 수 있다．

 如rever {
    mutex.lock () ;
      keyPressed.wait (&mutex) ;
      do_something() ;
      mutex.unlock () ;




298 CHAPTER 09_ Thread


===== PAGE 300 =====
이번 장에서는 QWaitCondition을 쉽게 이해할 수 있도록 다음과 같은 예제를 살펴보도록 하자. 두 개
의 쓰레드를 작성한다. 첫 번째 쓰레드는 Producer 쓰레드이고 두 번째 쓰레드는 Consumer 쓰레드이
다. Producer 쓰레드는 1초 간격으로 공용변수 numUsed에 1씩 값을 증가한다. 1씩 증가할 때마다
邸WaitCondition어］ 의해 대기하고 있는 Consumer 쓰레드의 상태를 wakeAll( ) 함수를 사용해 태기
모드를 해제한다．

邸WaitCondition어］ 의해 引ock Waiting 상태에 있는 Consumer 쓰레드는 Producer 쓰레드어］ 의해
깨어나고 공용변수 numUsed의 값을 화면상에 출력한다．

    QMutex mutex;         1
    QWaitCondition incNumber;
    mnt numused;
L


incNun小er는 QWaitConditi아I 클래스의 인스턴스이다. Producer와 Consumer 쓰레드간 동기화를
위해 사용한다. I끄imUsed는 Producer와 Consumer가 사용하는 공용변수이다．
Producer 쓰레드의 run( ) 함수에 공용변수 numUsed 값을 1초 간격으로 1씩 증가한다. 1씩 증가하고
Consumer 쓰레드가 QWaitCondition에 의해 미ock Waiting 모드 상태를 \Uake 모드로 전환하기 위
해 wakeAll( ) 함수를 사용한다．

    class Producer : public QThread
    {
    public:
          Producer ( )
          {
          }

    pr아；e（北ed:
        void run()
          {
               for (int i = 0 ; l < 10 ; i++){
                    sleep(l) ;
                    mutex.lock );
                    ++numtJsed;

                    incNuxnber.wakeAllU;
                    mutex.unlock () ;
               }
          }
     };


    Producer 쓰레드에서 사용한 incNumber는 邸WaitCondition의 인스턴스이다. Consumer 쓰레드와
    공용으로 사용하며 뮤텍스와 함께 사용한다. 소스 코드에서 보는 것과 같이 wakeAll( ) 함수를 호출하면
    incNumber어］ 의해 미ock Waiting 상태가 Wake中Up 상태로 전환된다．



                                                              1 Thread 299


===== PAGE 301 =====
class Consumer :public        QThread
 {
public:
      Consumer ()
      {
      }

protected:
      void run()
      {
           for (int   i = 0 ; i   < 10 ; i++)
           {
               mutex. lock () ;
                incNumber .wait (&mutex) ;
               mutex.unlock () ;


                qDebug (un그mUsed : %d", nuinUsed) ;
           }
      }
 };


Consumer 쓰레드는 邸WaitCondition 클래스의 인스턴스 incNumber어］ 의해 대기 상태로 진입하게
된다. Consumer 쓰레드는 Producer 쓰레드에서 wakeAll( ) 함수가 호출될 때까지 引ock Waiting 상
태가 된다. wait( ) 함수는 두 번째 인자를 사용할 수 있다．

bool QWaitCondition: :wait ( QReadWriteLock * locke妊之eadWriteLock
                                          r unsigned long time = ULONG-.，卜4AX)



두 번째 인자는 미ock Waiting 모드가 일정시간 동안 입력이 없을 때 Timeout을 위한 인자 값이다. 단
위는 millisecond이다. 지정한 millisecond 동안 응답이 없으면 邸A[aitCondition은 Timeout을 발생
하고 미ock Waiting 모드를 해제시킨다．

mnt main(int argc, char *argv[ ])
 {
      QCoreApplication a(argc, arg기;


      Producer producer;
      Consumer consumer;
      producer. s七ar七 ( ) ;
      consumer, start () ;


      return a.exec () ;




작성한 producer와 consumer 쓰레드를 메인함수에서 QThread의 start( ) 함수를 실행한다. start( )
함수를 실행하면 쓰레드의 run( ) 함수가 호출된다．


300 CHAPTER 09_ Thread


===== PAGE 302 =====
                       目
 unUsed
 unUsed
 unUsed
 unUsed




          l 234 56? 89 l
 unUsed
 unUsed
 unUsed
 unUsed
 unUsed
 unUsed




（그림）（콰NaitCondition 예제 실행 화면




  :tm Semaphore를 이용한 동기화
세마포어（Semaphore）는 멀티 프로그래밍 환경에서 공유 자원에 대한 접근을 제한하는 방법으로 사용된
다. 세마포어는 뮤텍스와 동일하다. 차이점으로 뮤텍스는 공유 리소스어］ 대한 접근을 제한하기 위해
Lock과 UnLock을 사용한다. 여러 개의 개체 간의 동시어］ 사용할 수 없도록 한다. 세마포어는 프로세스
간 메시지를 전송하거나 공유 메모리 영역의 접근을 동기화하는데 비교적 긴 시간을 확보해야 하는 경우
세마포어를 주로 사용한다．

세마포어는 공유 메모리 동기화를 하기 위한 목척으로 뮤텍스 보다 높은 수준의 동시성 접근 레벨을 제공
한다. 프로세스가 세마포어를 사용해 공유 메모리 영역을 사용하고 있을 때 다른 프로세스가 접근하면 먼
저 사용하고 있는 프로세스가 공유 메모리를 사용 완료할 때까지 대기한다．

                                                                      위
Qt에서는 세마포어를 사용하기 위해 QSemaphore 클래스를 제공한다. 세마포어의 연산을 제공하기
                                                                      사
해 acquire( ) 함수와 release( ) 함수를 제공한다. acquire(n) 함수는 n번째 리소스를 획득하기 위해
용하는 인자이다. 만약 리소스를 활용하지 못하면 Blocking 된다. release(n) 함수는 n번째 리소스를 해
 제한다．

  QSemaphore sem( 5) ;     7/ sem. available ( ) == 5


  sem.ac아1虹e (3 ) ;        /7 sem.available()       2
  sem.acquire (2) ;        /7 sem. available()      0
  sem.release (5) ;        7/ sem. available()      5
  sein.release (5) ;       /7 serrt. available()    10


  sem. tryAcquire (1) ;    /7 sem.available() == 9, returns true
  sem.tryAcq口ire (250) ;   7/ sem. available ( ) == 9, returns false



 또한 QSemaphore 클래스는 tryAcquire(n) 함수를 사용해1 n번째 리소스를 획득하기 위해 시도한다．
 만약 n번째 리소스가 활용 가능한지 확인하기 위해 available( ) 함수를 사용하면 된다．

                                                                       1 Thread 301


===== PAGE 303 =====
 QSemaphore 클래스를 이해하기 위한 예제를 위해 Producer 쓰레드와 Consumer 쓰레드를 작성한다．

  QSemaphore incNu山er;
     jnt numUsed;


 QSemaphore 클래스의 incNumber 인스턴스는 쓰레드간 동기화를 위해 사용한다. numUsed 변수는
 쓰레드간 사용하는 공용변수이다．

  class Producer : public QThread
  {
 public:
              Producer ( ) {}
 prote（北ed:
              void run()
              {
                  for (int   i = 0 ; i   < 10 ; i++){
                       sleep(l) ;
                       ++numUsed;
                       qDebug( "[ Producer] nuxnUsed : %d", numUsed) ;
                       incNumber. releaseO;
                  }

      ;



Producer 쓰레드는 numUsed 공용변수를 1초 간격으로 1씩 증가한다. 1씩 증가할 때마다 numUsed
값을 화면에 출력하고 release( ) 함수를 호출해 Consumer 쓰레드의 대기 모드를 해제한다．

 class Consumer : public QThread
 {
 public:
     Consumer () {}
 protected:
          void run()
          {
                  for (int I = 0 ; I < 10 ; i++){
                       IncNumber.acquire ( );
                      qDebug ( " [Consumer] numUsed : %d", numUsed) ;
                  }
          }
 };


Consumer 쓰레드는 QSemaphore 클래스의 acquire( ) 멤버함수에 의해 쓰레드가 Block Waitir培된
상태이다. Producer 쓰레드에서 release( ) 함수를 실행하면 Block Waiting 모드가 해제된다．




302 CHAPTER 09_ Thread


===== PAGE 304 =====
mnt main(irit argc, char *argv[ ])
 {
       QcoreApplication a(argc, arg기;
       Producer producer;
       Consumer consumer;
       producer. start () ;
       consumer. start ( ) ;
       return a.exec ( ) ;
 }


작성한 producer와 consumer 쓰레드를 메인함수에서 QThread의 start( ) 함수를 실행한다. start( )
함수를 실행하면 쓰레드의 run( ) 함수가 호출된다．




                          l l2 2 3 3 4 4 5 5 6 6 7 ? 8 8 9 9
 [Producer] numUsed
 [Consumer] numUsed
 [Producer] nunUsed
 [Consumer] numUsed
 [Producer] numUsed
 [Consumer] numUsed
 [F'川｝ducet口 nunflsed
 [Consumer] nunUsed
 [Producer] numUsed
 [Consumer] numUsed
 [Producer] numUsed
 [Consumer] oumUsed
 [Producer] nunUsed
 [Consumer] numUsed
 I Producer] numUsed
 [Consumer] numUsed
   nroducer] numUsed
     1 osumer] nunlJeed




（그림） oSemaphore 예제 실행 화면



QSemaphore는 印NaitCondition과 QMutex를 함께 사용한 것과 같이 쓰레드간 메시지 교환과 동기
화가 가능하다．


                  QtConcurrent를 이용한 멀티 쓰레드

QtConcurrent 클래스는 M毗ex, read-write locks, wait condition, semaphores 등과 같이 Low-
level 쓰레드를 사용하지 않고 멀티 쓰레드 기능을 제공한다. QtConcurrent를 사용해1 작성한 프로그램
은 프로세스 수어］ 따라 사용하는 쓰레드의 수를 자동으로 조절한다. QtConcurrent는 멀티코어 시스템
에서 동작하는 Qt 응용 프로그램 배포 시 확장하기 위한 목적으로 사용한다．

QtConcurrent 클래스는 공유 메모리（Shared中m아nory) 시스템의 MapReduce와 Filterl扼duce 구현
이 포함된 병렬 치리 스타일의 API와 GUI 기반의 어플리케이션에서 비동기 방식의 계산을 八ilappii培하
기 위한 클래스가 포함되어 있다．




                                                                    1 Thread 303


===== PAGE 305 =====
 0QtConcurrent::map( )
 모든 아이템에 함수를 container어］ 적용하거나 적절하게 아이템을 수정한다．


 0QtConcurrent::mapped( )
map(）과 같으나 다른 점으로 수정된 새로운 container를 리턴한다．


 DQtConcurrent::mappedReduced( )
mapped( ）과 동일하다. 다른 점으로 수정된 리턴값이 감소하거나 하나의 결과로 통합한다．


 0QtConcurrent::filter(
필터 함수의 결과어］ 따라 cor此amner로부터 모든 아이템을 제거한다．


0QtConcurrent::filtered( )
filter(）와 같으나 다른 점으로 필터 링된 결과와 함께 새로운 container를 리턴한다．


1QtConcurrent::filteredReduced( )
filtered( ）와 같으나 필터링된 결과가 감소하거나 하나의 아이템으로 통합한다．


1QtConcurrent::run( )
지정한 함수를 쓰레드에서 동작시킨다．


QtConcurrent::run( ) 함수를 사용해 작성한 함수를 쓰레드로 동작시켜 보는 예제를 다루어 보도록 하
자. 쓰레드로 동작할 함수를 다음과 같이 작성한다．

 void hello (QString name)
 {
     qDebug(    ) << "Hello" << name << "from" << QThread: :currentThread() ;


     for (int   i = 0 ; i < 10 ; i++)
     {
         QThread: :sleep(l) ;
         qDebug ( "[ %s] i = %d", name. data ( ) , i) ;
     }



QThread 클래스의 currentThread( ) 함수는 현재 수행되는 쓰레드의 포인터를 리턴한다. Name은 추
후 QFuture 클래스의 인자로 전달받은 QString 값을 출력한다．




304 CHAPTER 09_ Thread


===== PAGE 306 =====
 m1lt main(int argc, char *argv[ ])
 {
       QCoreApplication a (argc, argv) ;


       QFuture<void> U            = QtConcurrent: :run(hello, QStririg( "Alice ") );
       QFuture<void> f2 = QtConcurrent: :run(hello, QString( "Bob") );


       fl. waitForFinished( );
       f2 .waitForFinished( );


       return a.exec ( );
 }


QFuture 클래스는 다른 비동기화된 쓰레드로부터 수행한 결과를 표현하기 위해 사용한다. waitFor
Fin坮hed( ) 함수는 쓰레드가 결과를 리턴할 때까지 Blocking 된다．

QtConcurrent는 여러 STL 호환 container와 iter毗or 타입을 지원한다. 하지만 QList 또는 QVector
와 같이 랜덤 액세스 iterator를 가지는 Qt container를 사용하는 것이 성능 면에서 유리하다．

QFuture 외에도 QFutureiterator, QFutureWatcher 그리고 비동기화 방식인 여러 QFuture를 자동
으로 동기화를 지원하기 위해 QFutureSynchronizer 클래스를 지원한다．


    1 La "Bob11 fi 'on Q1hl'ead（目xd598 d尸 none - 'lln 'ead (pen
 , lbO "Alice " Iron QThread(目xd59ie吼 none = "Thread (p
汪B:i i == 日
U口 1. = 目
1石］ 1 == l
U口 I = l
[B] 1 = 2
 [[1 i 古 2
 !1] 1 = 3
 Ill 1 = 3
 Ii] I = 4
  ii i = 4
 [[1 1 = 5
 [II I = S
 II] i = A
 [I II 1 = 6
 [[1 i = 2
 냐] a = ?
  [1 i. = 8
  [1 1 = 8
 II] I = 9
 [[1 1 = 9




（그림）（거Concurrent 예제 실행 화면




                                                                                       1 Thread 305


===== PAGE 307 =====
M@viw


===== PAGE 308 =====
    CHAPTER




Container 클래스와
   Iterator 클래스


===== PAGE 309 =====
Qt 5 Programming




r미 Container클래스오나erat아 클래스
            데이터 수정, 삭제, 삽입, 저장하기 위해 （값는 유용한 Container와 Iterator 클래匹를 제공한다. （값에
            서 제공하는 Container와 Iterator 클래스에 대해 알아보도록 하자．




Container 클래스와 Iterator 클래스는 데이터 수정 , 삭제, 삽입, 저장 등을 위한 기능을 제공한다. 이
클래스들은 여러 타입들로 구성된 데이터들을 아이템 단위로 저장할 수 있다. 예를 들어 QString 타입의
데이터들을 배열에 저장하고 싶다면 몇 개의 배열을 사용할 지 미리 알고 있어야 한다. Container 클래
스는 가변 크기의 배열에 QString 데이터를 저장할 때 QVer切r<QString）의 （兀ntainer 클래스를 사
용하여 삽입 , 수정, 삭제를 할 수 있다.

Container 클래스들은 STL Container 클래스보다 가볍고 사용하기 쉬우며 안전하게 구현되었다. 그리
고 Qt는 如reach라는 키워드를 제공한다. 이 키워드는 Container 클래스와 같은 저장된 아이템을 쉽게
접근할 수 있도록 해준다. 다음의 표는 Qt어］ 제공하는 Container 클래스이다．

클래스                 설명
QList(T>            QList(T) 클래스는 가장 일반적으로 사용하는 클래스이다. 데이터 간의 인덱스를 사용해 접근할 수 있
                    으며 특정 타입（I）으로 이루어진 배열 데이터를 저장할 수 있다. 뿐만 아니라 인덱스 기반이므로 접근이
                    상당히 빠르다． O니St 클래스는 QList::append( ) 함수, QList::prepend( ) 함수와 Q니St::insert( ) 함
                    수를 사용해 데이터를 삽입할 수 있다．
O匕nkedL暾仟)          이 클래스는 （값-I없와 비슷하다. 차이점은 이 클래스는 데이터에 접근하기 위해 integer 기반의 인덱스보
                    다 iter計or률 사용한다. 거대한 데이터 중간에 데이터를 삽입할 때 O니St보다 더 빠른 성능을 제공한다．
QVector(T)          이 클래스는 메모리에 인접한 위치에 특정 타입의 데이터의 배열을 저장한다. Vec幻r의 맨 앞과 뒤에
                    데이터를 삽입하는 것은 상당히 느리다. 왜냐하면 메모리의 특정 번지에 의하1 거대한 데이터를 이동할
                    수 있기 때문이다．
QStack(T)           니FO 방식을 제공하는 QVertor으1 편리한 하위 클래스이다．
QQueue仟）            O니없의 디FO 방식의 편리한 하위 클래스이다．
QSet(T)             빠른 검색을 위한 단일 값으로 된 수학적인 방식을 제공한다．
QMap(Key, T)        데이터에 대응하는 하나의 Map 방식의 Key 값, 그리고 Key가 가리키는 T 타입의 데이터가 조합된 방
                    식, 즉 사전과 같은 방식을 제공한다. OMap은 Key 값에 따라 데이터를 저장한다. 만약 OMap 대신
                    다른 클래스를 사용해도 된다면 OHash를 사용하는 것을 권장한다．
QMu出Map(Key, T)     OMa口에서 제공하는 단일 Ma口의 Key 방식 형태를 멀티 map 기반의 인터페이스를 제공하는 편리한
                    하위 클래스0따．
QHash(Key, T)       OMap과 상당히 비슷하지만 저장된 데이터 상에서 검색 속도는 훨씬 빠르다. OHash는 저장할 데이터
                    를 랜덤하게 저장한다．
QM미tiHash(Key, T)   이 클래스는 멀티 키 방식의 OHash의 하위 클래스이다．



308   CHAPTER 10卞 （力ntainer 클래스와 Iterator 클래스


===== PAGE 310 =====
Coi此am er 클래스들은 여러 데이터를 하나의 집합으로 만들 수 있다. 예를 들어 QMap <QString,QList
<mnt力를 사용하는 것은 가능하다. QStrii培의 Key 타입의 값과 QList <m1lt> 타입의 데이터 값을 사용할
수 있다．

다른 데이터 타입이 할당된 데이터를 Qt에서 제공하는 다양한 Contatiner 클래스를 사용해 저장할 수
있다. 데이터를 복사하거나 할당 연산에 의한 데이터 타입은 QString, QDate, QTime과 같은 데이터
타입을 사용할 수 있다. 하지만 QObject 혹은 다른 QOb昶ct의 클래스（QWidget, QDialog, QTimer）는
동시에 사용할 수 없다 ．만약 Container 클래스어］ 다른 종류의 오브젝트를 저장해야 한다면 포인터 연산
을 사용하면 된다. 예를 들어 QList <Q＼航dget 朴와 같이 사용하면 된다．


      ]. ] Java 스타일의 Iterator 빙"식

Container 클래스 외에 Iterator 클래스는 Container어］ 저장된 특정 아이템에 접근하기 위한 통합된 방
식을 제공하며 Iter毗아를 사용하는 방식으로는 JAVA 스타일 방식과 STL 스타일 방식을 사용할 수 있다．

JAVA 스타일의 iterator 방식은 STL 방식을 사용하는 것보다 편리하다. 각（兀ntainer 클래스에 대해
JAVA 스타일 방식의 iterat야는 두 가지 데이터 타입이 있다. 하나는 read尸only 접근 방식과 read-
write 접근 방식을 제공한다．

Container                             Read-only iterator        Read-write iterator

 QList<T). QQueue(T)                   QListlterator(T)         OMutab陀니訓tera伯r<T)

 QLinkedListKT>                        0니nkedListlter계or(T)     QMutableLinkedListlterator(T)

 QVectorT). QStack<T>                  QVectorlterator(T)       QM마計)IeVectorIterator(T)

 QSet(T)                               0SetlteratcrKT)          QMu怡비eSetlterator(T)

 QMapKKey, T), QMu出Map(Key, T)         oMap仕eratorKKey, T1      oMutableMaplterator(Key, T)

 QHash(Key, T), QMultiHash(Key, T)     QHashlterator (Key, T)   QMutableHash仕erator(Key, T)



QLinkedList, QVector 그리고 QSet은 QList의 iter毗아와 비슷하며 QHash는 QMap의 Iter毗아와
비슷하다. STL 스타일 방식의 iterator와 달리 JAVA 스타일의 Iterator는 아이템 상에서 데이터 사이
를 구분하기 위해 포인터를 사용한다．


      ABCD        i
                       EFGH          HIJK
                                                   ;;;：그
                  1r
                              1               4

                              '1

（그림） Iterator를 구분하기 위한 포인터


 앞의 그림에서 보는 것과 같이 모든 요소들 사이에 QList <QString）를 다음과 같이 사용할 수 있다．




                                                                         ] Container 클래스와 terator 클래스 309


===== PAGE 311 =====
  QList<QString> list;
  list << "ABCD' << "EFGH" << '1HIJK " << "LMNO";

 QListlterator<QString> i (list) ;
 while (i. hasNext () )
      qDebug() << i. next () ;



 QListlterator 생성자는 list어］ 저장된 아이템을 반복해서 포인트를 이동시킨다. hasNext( ) 멤버함수는
다음 iter毗야의 다음 아이템이 존재하는지 검사한다. 만약 존재하면 다음 위치로 포인터를 위치시킨다. 만
약 위의 코드와 반대로 이전 아이템을 검색하고자 한다면 previous( ) 멤버함수를 사용하면 된다．

 QListlterator<QString> i (list) ;
 i. toBack ( );
 while (i. hasPreviousQ)
         qDebug( ) << i. previous ( );



Iterator가 가리키고 있는 현재 포인터의 이전 포인터로 이동하는 예제이다. 다음 그림은 next( ) 함수와
previous( ) 함수를 사용해1 이동 시 포인터 위치를 설명하기 위한 그림이다．


     ABCD           EFGH          HIJK       LMNO



                  느品1뇨／'
                 ，「
（그림） terator으1 口rev幻us(）와 next( ) 함수를 이용한 포인터 이동



QListlterator 클래스는 previous( ）와 next( ) 멤버함수 이외에도 다음 표와 같은 멤버함수를 사용할
수 있다．

함수                 설명
伯다ont()            리스트의 처음 위치로 Iterator를 이동시킨다．
toBack()           리스트의 마지막 itera幻r로 이동시킨다．
hasNext()          다음 iterator가 존재하는지 검사한다. 참일 경우 true를 리턴한다．
next()             가리키고 있는 iterato四1 위치Oil Al 다음 iterator와 아이템을 리턴한다．
peekNext()         iter計아의 이동 없이 다음 아이템을 리턴한다．
hasF가e너ous()      가리키고 있는 iterator 위치에서 이전의 iterator가 있는지 검사한다. 참일 경우 true를 리턴한다．
pre너ous()         Iterator으J 위치를 이전의 iterator로 한 단계 이동한 다음 이전 데이터를 리턴한다．
peekPrevious()    Iterator으1 이동 없이 이전 iterator 이전 아이템을 리턴한다．


QListlterator에서 제공하는 함수들은 데이터를 삽입 , 삭제하는 등의 멤버함수는 제공하지 않는다. 만약
저장된 아이템을 제거하기 위해 Q入4utableListIterator 클래스를 사용한다．




310 CHAPTER 10_ （力nt테ner 클래스와 陀ra幻r 클래스


===== PAGE 312 =====
QMutableListlterator<int> i ( list) ;


while (i. hasNext () ) {
     if (i. nex七（) 통 2 != 0)
          i . remove U;
}


앞의 소스 코드와 표어꺼 설명한 것과 같이 QLinkedList, QVec的r 그리고 QSet의 iterator에서도 동
일한 기능과 멤버함수를 제공한다. 다음 예제는 각 나라의 수도와 국가를 나타내는 아이템을 QMap을 사
용해 보도록 하자．

QMap<QString, QString> map;
map.insert ( "Paris ", "France ") ;
map.insert ( "Paris", "France ") ;
map. insert ( "Moscow", "Russia") ;


QMutableMaplterator<QString, QString> i (map) ;

while (i. hasNext () ) {
     if (i. next () .key() .endsWith ( "City ") )
          i . remove 0;
}


다음 예제는 QMap어］ 저장된 아이템들을 QHash에 저장하는 방법을 설명하기 위한 예제이다．

QMap<int, QWidget '> map;
QHash<int, QWidget 士 > hash;


QMaplterator<int, oWidget 士> i (map) ;
while (i. hasNext ( )) {
     i. next () ;
     hash.insert (i. key () , i. value ( ));
 }


만약 동일한 값으로 모든 아이템을 iterat야를 반복하고자 한다면 findNext( ) 함수 혹은 findPre-
미ous( ) 함수를 사용할 수 있다．

QMutableMap工terator<int, QWidget 士> i (map ; ;
while (i. findNext (widget) )
     i. removeO;




                                                    ] Container 클래스와 Iterator 클래스 311


===== PAGE 313 =====
       1.2 STL 스타일의 I te rato r 방식
 JAVA 스타일의 방식과 마찬가지로 STL 스타일 Iterator는 두 가지 데이터 타입이 있다. 하나는 read
 only 접근 방식과 read-w毗e 접근 방식을 제공한다. 다음 표는 STL 스타일의 Iterator 타입이다．

 Containers                          Read-only iterator               Read-write iterator
 QList(T), QQueue(T)                 QList<T)::constjterator          QList(T)::iterator
 OLin kedList(T)                     QLinkedList(T)::const_iterator   아inkedList仟):: jterator
 QVector(T>, QStack<T>               QVectorKp::const iterator        QVector(T)::iterator
 OSet(T)                             OSetKT)::const iterator          OSet<T>::iterator
 QMap(Key, T>, QMultiMap(Key, T)     QMap(Key, T)::constjterator      QMap<Key, T)::iterator
 QHash<Key, T), OMultiHash(Key, T)   OHash(Key, T)::const_iterator    QHash(Key, T)::iterator


STL 스타일의 Iter毗町는 배열에서 포인터를 사용하는 방식을 사용한다. 예를 들어 ++ 연산자, 火 연산
자는 Iter毗야의 아이템을 리턴하기 위해 사용한다. JAVA 스타일의 iterator 방식과 마찬가지로 QList
는 QLinkedList, QVector 그리고 QSet과 동일한 인터페이스를 제공하고 QHash는 QMap과 동일하
다. 아래 소스 코드는 QList <QString＞을 사용한 예이다．

 QList<QString> list;
 list << "ABCD" << "EFGH" << "IJKL'1 << '卜N0P";

 QList<QString>: :iterator i;
 for (i = list. begin() ; i != list. end( ); ++i)
 {
       出i = di) 止oLower ( ) ;
 }


JAVA 스타일의 Iterator와 달리 STL 스타일의 Iterator는 아이템의 포인터를 가리키도록 되어 있다．
begin( ) 함수는 iter毗아의 첫 번째 아이템의 포인터를 리턴한다. end( ) 함수는 iter毗or의 마지막 포
인터를 가리키며 실제 존재하지 않는 아이템의 포인터를 가리키도록 되어 있다．


     ABCD          EFGH      IJKL        MNOP           END




（그림） STL 스타일의 Iterator 포인터
                                          I
앞의 그림에서 보는 것과 같이 STL 스타일의 iterator 방식으로 이전 iterator의 포인터를 지정하기 위
해서 다음과 같은 방식을 사용한다．




312 CHAPTER 101（力nt졔ner 클래스와 陀ra幻r 클래스


===== PAGE 314 =====
QList<QString> list;
list << "ABCD" << '也FGH" << "IJKL" << "M正OP ";


QList<QString>::iterator i = list. end( );
while (i != list. begin( )) {
       --1;




       *i = (* j) . toLower () ;
}


만약 read-only 접근 방식을 사용하기 위해서는 const iter毗町를 사용할 수 있으며 Iterator의 첫 번
째 포인터를 가리키는 constBegin( ) 함수와 마지막 포인터를 가리키는 constEnd( ) 함수를 사용하면
된다．

QList<QString> : :const1iterator 1;
for (i = list. constBegin( ); i != list. cor'stEnd ( ); ++i)
     qDebug( ) << *i;



QMap과 QHash는 key( ) 함수와 value( ) 함수를 사용해 Iterator의 아이템에 접근할 수 있다．

QMap<int,     irit> map;


QMap<int, int> : :const iterator i;
for (1 = rnap.constBegin() ; i != map.const.End ( ) ; ++i)
     qDebug ( ) << i. key () << n : n << i. value () ;




    多t1.3 幻reach 키워드를 이용한 I te rator 접근

Iterator어］ 저장된 모든 아이템을 순서대로 반복하기 위해 Qt는 如reach 키워드를 제공한다. 이 키워드
는 c++ 언어에서 제공되는 키워드는 아니며 Qt에서 제공하는 추가된 키워드이며 전처리기（Preproce-
ssor）를 사용해 구현되었다. Syntax는 如reach(variable, container) 구문을 사용한다．

QLinkedList<QString> list;

QString str;
此reach 佃tr, uis七）
      qDebug() << str;


丸reach 키워드를 사용한 방식은 다른 반복 구문 방식보다 소스 코드가 간단 명료하다．

QLinkedList<QString> list;


QLinkedListlterator<QString> i (list) ;
while (i. hasNext ( ))
    qDebug() << i. next ( );



                                                               ] Con回ner 클래스와 Iterator 클래스 313


===== PAGE 315 =====
 콤마（comma）를 사용하는 데이터 타입（예를 들어 QPair<int, m t力과 달리 Iterator를 사용해 데이터 값
 을 사용하는 변수를 foreach 구문에 포함한다．

     QLinkedList<QString> list;


     foreach (const QString &str, list)
         qDebug() << str;



 일반적인 0++ 반복 구문에서 루프(loop）를 빠져 나오기 위해 break 구문을 사용하는 것과 같이
 foreach에서도 break 구문을 사용해 반복문에서 빠져나올 수 있다. 그리고 앞의 소스 코드에서 보는 것
과 같이 str 변수가 iterator의 값을 참조한다. 따라서 if문을 사용해 Iterator어］ 저장된 각 아이템 값을
참조할 수 있다．

 QLinkedList<QString> list;


 foreach (const QString &str, list)       {
     if (str. isEmpty () )
            break;
        qDebug() << str;




QMap과 QHash는 사용할 때 foreach는 (key, value) 쌍（pair）을 함께 접근할 수 있다．

 QMap<QString, int> map;

 foreach (const QString &str, map.keys ( ))
        qDebug() << str << ": " << map.value(str) ;



QMultiMap을 사용하여 Key와 Value를 다음과 같이 사용할 수 있다．

 QMultiMap<QString, int> map;

 foreach (const QString &str, map.uniqueKeys ))
 {
        foreach (mnt i, map.values (str) )
            qDebug() << str << ": " << i;
 }




314 CHAPTER 10_ Coni톄ner 클래스와 Iterator 클래스


===== PAGE 316 =====
CHAPTER




          XML


===== PAGE 317 =====
（그t5 Pro아amming




r미 XML
          XM匕 문서를 핸들링 하기 위한 방법으로 （값에서 제공하는 API에 대하1 살펴보도록 하자．




XML(eXtensible Markup Language）은 수많은 종류의 데이터를 기술하는 더］ 사용하기 위한 마크업
언어이다. XML을 사용하는 이유는 여러 가지 이유가 있지만, XML을 사용해 수많은 종류의 문서를 읽
기 쉬운 형태로 정의할 수 있기 때문에 사용자가 읽기 쉽다. 그리고 다른 어플리케이션과 다른 시스템에
서 XML 사용해 데이터를 쉽게 주고받을 수 있다．

Qt는 XML을 모듈 형태로 제공한다. 모듈의 클래스를 혜더 파일에 포함하기 위해 다음과 같이 QtXML
해더를 소스 코드에 추가한다．

 孝include <Q七Xml>


그리고 qmake의 .pro 파일에 다음과 같이 XML 모듈을 추가한다．

 QT += xml


Qt는 XML을 접근하기 위한 방법으로 DOM과 SAX 방식을 제공한다. SAX는 DOM 방식어］ 비해 간단하
게 구현이 가능하다. 그리고 XML 파일을 분석하면서 읽어 들이는 방식이다. DOM 방식은 XML 파일 전
체를 메모리에 트리 형태로 저장한 다음 읽어 들인다．

SAX는 XML 데이터를 수정하는 것이 어렵다. 반면에 DOM에 비해 작은 메모리를 소모한다. 그렇기 때1
문에 작은 메모리를 사용해야 한다면 SAX 방식이 유리하다．

DOM은 XML 문서 전체를 메모리에 유지하므로 많은 메모리를 사용한다. 또한 메모리 상에 존재하므로
수정과 같은 작업이 빈번히 이루어질 때 유용하게 사용할 수 있다. 그리고 파일로부터 읽어 메모리 상에
상주해햐 하는 경우 DOM 방식이 SAX 방식에 비해 빈번히 사용된다．

파일 입출력을 다룬 단원에서 우리는 파일을 직접 읽는 방법과 스트림을 읽는 방법을 사용하였다. 마찬가
지로 XML을 접근하는 방식은 두 가지로 분류할 수 있다. 첫 번째는 Qt가 제공하는 API를 사용해 접근
하기 보다는 QXmlStrean氓eader와 QXmlStreamWri扼r 클래스를 사용하는 것이 성능상 유리하다．
이 클래스들은 XML의 스트림을 통해 매우 빠르게 분석（Parser）할 수 있는 기능을 제공한다．


316 CHAPTER 11_ XML


===== PAGE 318 =====
QXmlStreamReader 클래스는 SAX Parser를 위한 QXmlSimpleReader 클래스 보다 어플리케이션
상에서 더 빠르고 쉽게 사용할 수 있다. QXmlStreamReader 클래스는 데이터를 읽기 위한 방식으로
印ODevice 또는 QByteArray로부터 Raw 데이터를 읽어 들일 수 있다．

QXmlS七rean氓eader 坦Ti';


while (！玎nl. a七End( ) ) {
      xml.readNext () ;
          . . . II do processing
 }
if     佯ml. hasErr吐（ ) ) {
         . . . // do error handling
 }


QXmlStreamWriter 클래스는 단순한 스트림을 경유하여 XML 데이터를 Write 할 수 있는 기능을 제
공한다. 이 클래스는 setDevice( ) 멤버함수로 지정된 印ODevice를 통해 동작한다．

 QxrnlStreamWriter stream( &output) ;
 stream. setAutoFormatting (true) ;
 strearn.writeStartDocunlentU;

 strearn.writeStartElement ( 1'bookmark") ;
 streanhwriteAttribute ( "href ", "http: //gt. digia.com/ ") ;
 St丁earn. writeTex七Elemen七（ntd土leu r IIQ七 Home" ) ;
 stream.writeEndElement () ; // bookmark

 stream.writeEndDocument () ;



Qt는 XML을 다루기 위해 다음과 같은 다양한 클래스를 제공한다．

 클래스                        설명
 QDomAttr                   ODom티ement 중 하나의 attribu也를 나타낸다．
 QDomCDATASection           XML CDATA sect向n을 나타낸다．
 QDomCharacterData          DOM에서 일반적인 String올 나타낸다．
 QDomComment                 XML 컴포넌트를 나타낸다．
 QDomDocument               XML document를 나타낸다．
 Q［兀mDocu men卄가agment       일반적으로 완벽한 QDomDocument가 아닌 a［兀mNodes의 Tree를 나타낸다．
 QDomDocumentType           도큐먼트 Tree에 DTD의 표시
 QDom티ement                  DOM Tree에서 하나의 이ement를 나타낸다，
 QDomEntity                  XML의 Enti印를 나타낸다．
 QDomEntityReference         XML의 Entity 레퍼런스를 나타낸다．
 QDomlmplementation          D아vi 구현의 특징에 관한 정보
 ODomNamedNodeMap            이름으로 접근할 수 있는 Node들의 집합을 포함
     QDomNode                D아／ tree에서 모든 Node의 부모 클래스
     0［兀mNode口st             0［兀mNode 오브젝트 리스트



                                                                            1 XML 317


===== PAGE 319 =====
  클   ／뇨
                               설명
  QDomN이at山n                   XM[ 표기법을 나타낸다．
  QDomProcessinglnstruction    XML 미ocessing instruct口n을 나타낸다．
  QDomlext                     분석된（Parsed) XML docurr祀nt에서 텍스트 데이터를 나타낸다．
  QXm!Attributes               XML attributes를 나타낸따．
  QXmlContentHandler           XML 데이터의 논리적인 내용을 리포트하기 위한 인터페이스
  QXmIDTDHandIer               XML data의 DTD Con旭nt를 리포트하기 위한 인터페이스
  QXmlDeclHandler              XML 데이터 선언（declar帥on) 내용을 리포트하기 위한 인터페이스
  QXm山可au仕Handler              모든 XML 핸들러 클래스의 기본 구현 클래스
  QXmlEntityResolver           XML 데이터에 포함된 외부 엔티티들을 해석하기 위한 인터페이스
  QXmlErrorHandler             XML 데이터에서 에러를 리포트하71 위한 인터페이스
  QXmllnputSource              QXmlReader 하위 클래스를 위한 입력 데이터
 QXmlLex七쉐Han미er               XML 데이터의 어휘 내용을 리포트하71 위한 인터페이스
 QXm止ocator                    파일 내에 파싱 위치와 관련한 정보를 제어하기 위한 XML 핸들러 클래스
 QXmlNamespaceSupport          네임스페이스 지원을 포함하7릍 원하는 XML 리더를 위한 He巾er 클래스
 QXmlParseException            QXmlErrorHandler 인터페이스를 사용해 에러를 리포트하71 위하1 사용
 ox씨Reader                     XML 리더를 위한 인터페이스
 QXmlSimpleReader              간단한 XML 파싱을 위해 구현된 클래스




           ]. ] 스트림을 이용한 XML- 데이터 핸들링

데이터 및 파일로부터 XML 데이터를 Read, Wri扼하기 위해 스트림을 사용할 수 있다. 스트림 API를
경유하여 XML을 빠르고 쉽게 Parsii培하는 것이 가능하다. Qt에서는 XML에서 스트림 기능을 제공하
기 위해 QXmlStreamReader와 QXmlStreamWri扼r 클래스를 제공한다. 이번 장에서는 이 클래스를
이용해 스트림으로부터 XML 테이터를 읽어오고 저장하는 방법에 대해 알아보도록 하자．


S QXmlStreamReader 클래스
QXmlStreamReader 클래스는 단순한 스트림 기능을 제공하는 API이다. 스트림 API를 경유해 읽어온
XML 데이터를 파싱하는 기능을 제공한다. QXmlStreamReader 클래스의 기본 개념은 SAX와 비슷하
며 코튼 단위로 스트림으로부터 데이터를 파싱한다. 토큰 단위로 스트림을 통해 데이터를 읽어오기 위해
readNext( ) 멤버함수를 사용한다．

 QXmlStreamReader xml;


 while (! 沁nl. atEnd ( ) ) {
       xinl.readNext () ;
           . . . // do processing
 1
 J


 if   (xinl.hasError () ) {
          . . . // do error handling




318 CHAPTER 11_ XML


===== PAGE 320 =====
QXmlStreamReader 클래스는 외부 파싱을 포함하지 않는 XML 1.0 기반 Parser를 제공한다. XML
문서로부터 데이터를 읽어오기 위해 readNext( ) 함수를 사용한다. 이 함수는 토큰 단위로 이동해 데이
터를 스트림으로부터 읽어 온다．

만약 스트림으로부터 데이터를 읽어오는 과정에서 에러가 발생하면 hasError( ) 함수를 사용할 수 있다．
이 함수는 다음 토큰에서 데이터를 읽어올 때 발생한 에러를 Detecting이 가능하다．


S QXmlStreamWriter 클래스
QXmlStreamWriter 클래스는 스트림을 사용해 \writing 할 수 있는 스트림 API를 제공한다. XML 데
이터를 Writing하기 위해 setDevice( ) 함수로 지정된 QlODevice를 통해1XML 데이터를 Writii培하게
된다．

QXmlStreainWriter stream( &output) ;
stream. setAutoFormatting (true) ;
streain.writeStartDocument () ;


 stream. writeStartElement ( "bookmark") ;
 stream.writeAttribute( "href ", "http: //www.qt-dev.com/ ") ;
 stream.writeTextElement ( "title ", "Qt Home") ;
 stream.writeEndElement () ; II bookmark


 stream.writeEndDocument () ;



QXmlStreamWriter 클래스는 Elements와 Attributes를 Write할 때 namespaceUri를 지정해야 한
다. 그리고 스트림 기반으로 XML의 데이터를 Wri扼하기 위한 포맷을 자동으로 지정한다．


0QXmlStreamReader오｝ QXmI앉reamWriter 클래스를 이용한 예제
QFile 클래스를 이용해 XML 문서가 저장된 파일을 QXmlStreamReader 클래스로 읽어와 GI끄상에
결과를 출력하고 다시 QXmlStreamWriter 클래스를 이용해 결과를 저장하는 예제를 살펴보도록 하자．

 QString inputFilePath =
    QFileDialog: :getOpenFileName(this, tr ( "Open XML File ") ,
                                  QDir: :currentPath() ,
                                  tr ( "XML Files (*．刃nl) ") );


 QFile inputFile (inputFilePath) ;



QFi1eI万alog 클래스는 사용자로부터 파일 시스템에 저장된 파일을 선택할 수 있는 다이얼로그를 제공한
다. 사용자가 선택한 파일명（파일 PATH 포함） ii叩utFilePath에 리턴 값으로 저장한다．

 inputFilePath어］ 저장된 파일명은 QFile을 이용해 파일을 읽어온다. 이 예제에서는 읽어온 파일을 직접
 다루지 않고 QXmlStrean氓eader를 이용해 스트림 방식을 사용한다．


                                                                   1 XML 319


===== PAGE 321 =====
  OFile inputFile ( inputFilePath) ;


  if ( !QFi1e: :exists(inputFilePath) ){
      edt->setText ( "File does not exist. ") ;
  }
 else if ( ! inputFile.open(QlODevice: :ReadOnly) ) {
     edt->setText ( "Failed to open file. ") ;



 QFile outputFile ( " s出npleOutput.xml") ;
 outputFile . open ( QlODevice: : WriteOnly) ;



QFi1e 클래스의 open( ) 함수를 이용해 사용자가 선택한 파일을 읽기 모드로 선택한다. 읽기 모드로 선
택한 파일의 QFi1e 클래스 인스턴스를 QXmlStreamReader 클래스 인스턴스 생성 시 첫 번째 인자로
지정한다. 파일을 저장하기 위해 동일한 방식으로 QXmlStreamWriter 클래스 인스턴스 생성 시 첫 번
째 인자로 지정한다．

 QXmlStreaxflReader reader ( &inputFile) ;
 QXmlStreaniWriter writer ( &outputFile) ;


 QString inputData;
 while( !reader.atEnd( ))
 {
      reader.readNext () ;

      if ( !reader. text ( ) .isEmpty ( ))
           inputData.append(reader.text ( )) .append ( "<br> ' ) ;

      writer .writeCurrentToken (reader) ;
 }

 edt->setText ( inputData) ;



reader 인스턴스는 파일로 읽어온 뎨이터를 스트림을 통해1XML 문서 뎨이터를 읽어올 수 있는 기능을
제공한다. atEnd( ) 함수는 스트림으로부터 읽어온 XML 문서 내용을 마지막인지 판단하기 위해1 제공하
는 함수이다. readNext( ) 함수는 XML 문서의 내용을 토큰 단위로 읽어올 수 있다. 토큰 단위로 분리된
XML 문서의 내용은 포인터를 이동할 수 있는 기능을 제공한다．

토큰 단위로 읽어온 XML 포맷의 데이터를 wri扼r 인스턴스를 이용해 스트림을 경유하여 파일어］ 저장할
수 있다. 현재 XML 토큰 위치의 내용은 wri扼CurrentToken( ) 함수를 사용하여 파일어］ 저장한다．




320 CHAPTER 11_ XML


===== PAGE 322 =====
     Literate Programming: Propaganda and Tools


     Literate Programming by Henrik Turbell


     Literate Programming Library


（그림） 스트림을 이용한 예제 실행 화면




（t2Document
言           0히ect 卜加der
Qt는 XML 문서를 핸들링하기 위한 방법으로 DOM과 SAX 방식을 사용할 수 있다. DOM 방식과 SAX
방식의 차이점 중 하나는 XML 문서를 읽어와 메모리에 저장하고 XML 문서의 내용을 액세스하는 방식
을 사용한다. 그렇기 때문에 SAX 방식보다 메모리 자원을 많이 사용하지만 XML 문서의 데이터를 수정
하는 것은 SAX 방식보다 용이하다. 이번 장에서는 DOM 방식을 이용해 읽어온 XML 파일을 핸들링하는
방법에 태해 살펴보도록 하자．

예제의 mainwindow.h와 mainwindow. cpp 소스 코드 파일은 어플리케이션의 GUI를 구현한 소스 파
일이다. 이 예제에서는 QTreeWidget 클래스를 사용한 XML 데이터로부터 읽어온 데이터를 트리 구조
형태로 GUI상어］ 출력하기 위한 위젯으로 사용한다. xbeltree.h와 xbeltree. cpp 파일은 XbelTree 클래
스를 구현한 소스 파일이다. XbelTree 클래스는 QTreeWidget 클래스를 상속 받는다．

 <?xxnl version=" 1. 0 " encoding="UTF-B "?>
 <!DOCTYPE xbel>
 <xbel version=" 1.0 ">
        <folder fo1ded="yes ">
            <title> Literate Prograxnming</title>
            <bookmark href=" http: //www.vivtek.com/litprog. html">
                   <title> Synopsis of Literate Programming</title>
               </bookmark>




QTreeWidget 클래스를 상속받은 XbelTree 클래스는 QDomElement 클래스로부터 XML 문서를 읽
어와 파싱한다. 파싱한 Eleme砒의 tag를 QTreeWidget어］출력한다．

 class XbelTree : public QTreeWidget
 {
    Q OBJECT
 publi（그:
         XbelTree (QWidget; 枉沮rem七 = 0) ;

        bool read(QlOoevice *devjce) ;                                      O

                                                                      1 XML 321


===== PAGE 323 =====
     bool write (QloDevice *devjce) ;


private slots:
     void updateDomElement (QTreeWidgetltem *item, mnt column) ;

private:
     void parseFolderElement ( const QDomElement &element,
                               QTreeWidgetl七텨n 出parentl七em = 0) ;
     QTreeWidgetltem *createltem( const QDomElement &element,
                                    QTreeWidgetltem *parentltem = 0) ;

     QDomDocument domDocument;
     QHash<QTreewidgetltem 火, QDoinElement> domElementForltem;
     Qlcon folderlcon;
     Qlcon bookmarklcon;
};
XbelTree 클래스의 생성자에서는 상속받은 QTreeWidget 클래스의 헤더를 설정한다. QTreeWidget
상어］ 헤더를 설정하기 위해서는 setHeaderLabels( ) 멤버함수를 사용한다. QTreeWidget은 등록한 아
이템에 아이콘을 사용할 수 있다. 이 예제에서는 Qt에서 디폴트로 제공하는 아이콘을 사용한다．

XbelTree: : XbelTree ( QWidget *parent)
     : QTreeWidget (parent)
{
     QStringLis七 label引
     labels << tr ( "Title ") << tr ( "Location") ;
     header ( ) ->setSectionResizeMode (QHeaderView: : Stretch) ;
     setHeaderLabels (labels) ;


     如lderlcon. addi山an叩作七yle (卜＞standard1山unap(QStyle: :SP口DirClosedlcon) ,
                           Qlcon: :Normal, Qlcon: :Off) ;
     folderlcon.add山map(style( )->standardPixmap(QStyle: :SP_DirOpenlcon) ,
                           Qlcon: :Normal, Qlcon: :On) ;
     bookmarklcon. addPixmap( style ( ) .->standardPixmap(QStyle: : SP_Filelcon) );
}


XbelTree 클래스의 read( ) 함수는 XML 문서로부터 읽어온 데이터를 파싱한다. QDomElement 클래
스의 root 인스턴스는 XML의 DOCTYPE의 Tag를 읽어온다．

그리고 root Element의 하위 Elem이此를 파싱한다. parseFolderElement( ) 멤버함수는 하위 Tag를
파싱하기 위해 구현한 함수이다. while문에서 사용한 isNull( ) 함수는 root Element 하위에 포함된
child Elem이此가 마지막인지 bool 타입으로 결과를 리턴한다. while문에 포함된 다음 child Element
를 읽어오기 위해 nextSiblingElement( ) 함수를 사용하면 된다.




322 CHAPTER 11느 XML


===== PAGE 324 =====
    QDomElement root = domDocument. documentElernent () ;
    if (root. tagName () 1= "xbel '' ) {


    }

    clear ( ) ;

    disconnect (this,                SIGNZL (itemChanged(QTreeWidgetItem* , int) ),
                this,                SLOT (updateDo田lement (QTreeWidgetltem* , mnt) ))7

    QDomElement child = root. firstChild日lement ( "folder ") ;
    while (! child. isNull ( )) {
        parseFolderElement (child) ;
        child = child. nextSiblingElement ( "folder ") ;



i
        nnec七   （七hiS,
                                  SIGNAL ( itemChanged ( QTreehidge七I七e耐，        in七）  ),
[
                         trils,   bLUT   (upc1ateDo   毗1ement   (QTreeW1QgetItern* , int) ));


read( ) 멤버함수에서 사용한 clear( ) 함수는 QTreeWidget 클래스의 멤버함수이다. 이 함수를 사용하
면 QTreeWidget에 등록된 모든 아이템을 삭제한다 ．그리고 disconnect( ) 함수는 기존의 QTree
Widget어］ 등록된 아이템의 시그널 슬롯을 disconnect하기 위한 함수이다. 이 예제에서는 파일 메뉴를
통해 다른 XML 문서 파일을 읽어온다. 읽어온 X八4L 문서를 QTreeWidget을 업데이트 한다. 따라서 기존
어］ 있던 아이템을 삭제하고 연결되어 있던 시그널 슬롯 이벤트를 삭제해야 한다.

    connect( ) 함수는 QTreeWidget어］ 새로 업데이트된 아이템을 시그널 슬롯을 통해 연결한다. 이 예제어］
서는 QTreeWidget어］ 등록한 아이템을 수정할 수 있는 기능을 제공한다. 사용자가 GUI상에서 QTree
    Widget어］ 아이템을 선택하면 수정할 수 있는 GUI 인터페이스를 제공한다. 수정이 완료되면 시그널／슬
롯 이벤트가 연결된 updateDomElement( ) 슬롯함수를 호출한다．


    void XbelTree: :updateDomElement (QTreewidgetltem *item, mnt column)
    {
          QDomElement element = domElementForltem.value (item) ;

          if    (! element.isNull () ) {
                 if (column == 0) {
                      QDomElement oldTitleElement -= element. firstChildElement ( "title            ") ;
                      QDoinElement newTitleElement = domDocument.createElement ( "title             ") ;

                             QDomText newTitleText = dor山ocument.createTextNode (
                                                                                item->text (0) );
                             newTitleElement. appendChild ( newTitleText) ;
                             elemen七．replaceChild (new꺼土leElemen七r olc汀j土leElemen七）;
                         } else {
                             if (element. tagName () == "bookmark")
                                  element.setAttribute ( "href", item->text (l) );
                         }
          }
    }

                                                                                                           1 XML 323


===== PAGE 325 =====
 updateDomElement( ) 함수는 슬롯함수이다. GUI상에서 QTreeWidget 아이템을 수정하면 수정된 아
 이템을 QTreeWidgetltem 인스턴스를 첫 번째 인자로 넘겨준다. 넘겨 받은 인자를 setAttribute( ) 함
 수를 이용해 수정한다. wri扼（) 멤버함수는 메모리에 저장된 XML 문서를 파일에 저장한다. 파일에 저장
 하기 위해1QDomDocument 클래스의 save( ) 함수를 사용하면 파일에 저장할 수 있다．

  bool XbelTree: :write (QlODevice *devjce)
  {
              const mnt IndentSize = 4;


              QTe＞比S七ream ou七（device) ;
              domDocument. save (out, IndentSize) ;
              return true;
  }


 createltem( ) 멤버함수는 QTreeWidget 상에 새로운 아이템을 등록하기 위한 함수이다. 또한 새로 등
록한 아이템은 XML의 Elemer此로 추가한다．

  QTreeWidgetltem *XbelTree: :createltem(const QDomElement &element,
                                                                            QTreeWidgetltem *parentltem)
  {
             QTreewidge七I七em 士item;
             if    (parentltem) {
                   item = new QTreeWidgetltem(parentltem) ;
              } else {
                   3土em = new QTreeWidgetl七em作hi引 ;
             }
             domElementForltem.insert (item, element) ;
             return item;
 }


! 亘크 DO入I Bookmarks
  F陀         He巾
 Title                                                     Lou苡口n
         J   1 Qt
                幽 Qt 4.7 Reference                         httpi/q卜project.oug/doc/qt-4.7/
                回 Qt 4.8 Reference                         ht如-i/ q卜po才out어gfdoc/ql卜4.8/
               國 Qt 5.0 Reference                          httpj/qt-projectorgfdoc/q卜5.0/
               回 Qt Home陀Re                                httpi/qtnok汨．Com/
         P Jg lOSreams
         I' j$ gdb
            嚼Classes and Constructors
            Software Documentation or System Documentat.
            TX Res어Jrces
  d
            Portable Document Format (PDF)
            圃Adobe - The po引script and PDF standards       http://snuwadobe.corn/
            回Reference Manual Portable Document Format     http://partners.ad야）e.com/asrvdeveloper/technotes/acro
            回Ad야）e Acrobat Software Development Kit        http://partners.a야珀.com/asrrJdeveIopec/acrosdk/main
            니teratUre 듸tes




（그림） D（가＼,1 방식의 예제 실행 화면




324 CHART타긋 11. XML


===== PAGE 326 =====
        1.3 Simple API for XML
SAX(Sin叩le API for XML）는 XML 문서를 나타내는 표준인터페이스이다. 이전 장에서 다룬 DOM과 달
리 SAX는 XML 문서로부터 파싱한 모든 객체들을 메모리에 올리지 않는다. SAX는 XML을 하나의 긴 문
자열로 인식하며 앞에서부터 차례로 읽어 가면서 요소 및 속성이 인식될 때마다 이벤트를 발생시킨다. 즉，
SAX는 XML의 파싱한 모든 결과를 메모리에 올리지 않기 때문에 DOM어］ 비해 메모리를 작게 사용한다．

하지만 SAX는 차례로 읽어 가면서 XML 핸들러를 구현하는 방식이므로 XML 문서의 특정 요소를 수정
하는 것이 불가능하다. DOM은 XML 문서에 대한 구조적 접근이 필요하거나 XML 문서 구조를 쉽게 파
악하기 위해 주로 사용된다. 또한 XML 요소를 수정하는 경우에도 DOM 방식이 주로 사용된다. SAX는
문서의 일부분만 읽어와 유효성을 판단 또는 파싱해야 하는 XML 문서가 많거나 큰 경우에 적합하다. Qt
에서는 QXmlDefaultHandler 클래스를 사용해 SAX 방식으로 XML 문서를 파싱할 수 있다. XML 문
서는 SAX 방식을 사용하기 위해 다음과 같은 이벤트 핸들러를 작성할 수 있다．

  estartElement
 1endElement
 1characters


                                                                          卜 嗽artE匕m미 t
 (7xn,l vers油n= l .0 encodkig=.UTF-8.?>              '
 ＜江刃C丁YPE books>       ====11nmm111111mm411기기1Hm====＝·                    =＞吼artElem帥t
 \                                                  /

 <books vs囹on＝녀 .丁＞                                                        > 制晤代E泊ment
     <bern>                                                  ：뇨．.m           + 吼계tElement
           <bookmark urI='ttltp:f/. . ./qt-4.8/'></bookmark> H4              ) 毗artElement
           ＜甘te>
           Of 4.8 Reference                                          --------卜characters
           <／撤旭＞                                                     nHmH仁 endE佃1겨知t
     <Iitem>
     <item>                                             ．노m1d             午 S怡rt日ement
          <bookma水 urI=mhtt口；//.../qtH5.0/ ' ></b어味m帥（> 1·끼11巾1m          卞 St미炬1剖TI日nt
           <tiUe>
           Ot 5.0 Reference        ' 1=" ' 11             口1' m'         > charac泊田
          <Itit1e>                                        m1' ==1        卜 end티em이｝t
     <fdem>

 </books>                                                                  >endElem머）t


（그림） SAX 방식을 이용한 이벤트 핸들러 처리 함수



앞의 그림에서 보는 것과 같이 XML 문서를 SAX 방식으로 파싱하기 위해 startElement, characters
그리고 endElement 이벤트 핸들러 함수를 작성해야 한다. 구현해야 할 이벤트 핸들러 함수는 QXml
DefaultHandler 클래스에서 제공하는 재정의 함수（Virtual function)를 사용하면 된다．

QXmlDefaultHandler 클래스에서 제공하는 재정의 함수를 통해 XML 문서를 파싱하며 Bool 타입의
리턴 값을 반환한다．




                                                                                             1 XML 325


===== PAGE 327 =====
class saxParser : public QXmlDefaultHandler
{
public:
     saxParser (QTreeWidget *treeWidget) ;
     bool startElement (const QString &namespaceURl, const QString &localName,
                     const QString &qName, const QxmlAttributes &atts) ;
     bool endElement (const QString &namespaceuRl,
                      const QString &localName, const QString &qName) ;
     bool characters (const QString &str) ;

private:
     QTreeWidgetltem *createchildltem(const QString &tagName) ;
     QTreeWidge七 士treewidge七；
     QTreewidge七I七em 士1七em;
     QString currentText;
 ;



startElement( ) 함수는 파싱해햐 하는 XML 문서로부터 books 태그와 version 속성을 질의한다. 그
리고 bookmark 태그의 unl 속성을 질의한다. bookmark 태그가 발견되면 QTreeWidget의 상위 트리
아이템으로 등록한다．

characters( ) 함수는 title의 Element 값을 얻어오며 동시에 endElement( ) 함수가 호출되어 title 태
그 이벤트가 발생하면 QTreeWidget의 하위 트리 아이템으로 등록한다．

bool saxParser: :startElement (const QString &/* namespaceuRl */,
                               const QString &/* localName */,
                               const QString &qName, const QXmlAttributes &atts)


     if (qName == "books ' ) {
          if (atts. value ( "version" ) != n l .0 " ) {
               return false;
           }
     }else if (qNaxne == 1'bookmark") {
         item = createChildltem(qName) ;
         item->setText (l, atts .value( "url ") );
     }
     return true;




앞의 코드는 startElement 이벤트 핸들러 함수이다. XML 문서에서 books 태그와 bookmark 태그를
qName 변수에 저장된 태그 값을 이용하여 유효성을 검사한다. bookmark 태그에서는 unl 속성 값을
읽어 QTreeWidget의 상위 트리 아이템으로 등록한다. 트리 아이템으로 등록하기 위해 구현한 create
Childltem( ) 함수를 호출한다. 인자는 태그명을 넘겨주면 QTreeWidget 클래스의 QTreeWidget
Item 인스턴스를 리턴한다．




326 CHAPTER 11_ XML


===== PAGE 328 =====
1QTreewidgetltem *saxparser: :createChildltem(const QString &tagName)
! {
1                QTreeWidgetltem *childltem;
                 if (tagName == "title ")
                       childltem = new QTreeWidgetltem(treeWidget) ;
                 else
                       childltem = new QTreeWidgetltem(item) ;


                 childltem->setData ( 0, Qt: : userRole, tagName) ;
                 return childltem;




앞의 소스 코드에서 보는 것과 같이 태그명이 title이면 QTreeWidget의 상위 아이템을 생성하고 그렇지
않으면 title의 하위 아이템으로 등록한다. startElement( ) 함수에서는 bookmark 태그가 발견되면
createChildltem( ) 함수를 호출해 title 태그의 하위 아이템으로 등록한다．

  bool saxParser: :endElement (const QString &/* namespaceURl */,
                               （兀ns七 QString &／火 localName 出／,
                                                    const QString &qNaine)
  {
                 if (qName == "title" ")){{
                      j土em = Oreat;eChild
                      item                  ltem(qNanie) ;
                               createChild1t;em(qNa工ne)
                      item->setTe
                      it; eme>Set;TeXt (0, currentTex
                                    xt;(0r             ;) ;
                                           Cdrrent;TeXtt)
                 }
                 re七nrn trne;
                 return true;
      }


 endElement( ) 이벤트 핸들러 함수는 title 태그가 발견되면 QTreeWidget의 상위 아이템으로 등록하
 기 위해 create（그hildltem( ) 함수를 호출한다. 만약 title 태그가 발견되면 동시에 title 태그의
 Element 값을 얻어오기 위한 characters( ) 이벤트 핸들러 함수가 호출된다．

 characters( ) 함수는 title 태그의 Element 값을 currentTe玭 멤버변수에 저장한다. currentText 변
 수에 저장된 값은 endElement( ) 함수에 의해 아이템 텍스트로 설정된다．

      bool
                     saxParser:   :characters   (const
                                                          QString &str)


                  if ( Lstr. isEmpty () )
                        currentText = str;
                  return true;
             }


  지금까지 살펴본 XML 문서 파싱 이벤트 핸들러 함수는 saxParser 클래스로 구현한다. saxParser 클
  래스의 인스턴스 widget.h와 widget. cpp 소스 코드의 Widget 클래스에서 인스턴스를 생성한다. 인스
  턴스 생성이 완료하면 파일 다이얼로그로부터 지정한 XML 문서 파일을 QXm1Sin叩leReader 클래스를

                                                                             1 XML 327


===== PAGE 329 =====
 이용해 XML 문서 내용을 읽어 들인다．


 void Widget: :createSAXParser (QString fileName)
 {
         saxParser handler (treeWidget) ;
         QxmlSimpleReader reader;
         reader. setContentHandler (&handler) ;


         QFile file (fileName) ;
         if (! file. open( (QFile: :ReadOnly 1 QFile: :Text) )){
               QMessageBox: :warning(this, tr ( "SAX Bookmarks ") ,
                                        tr ( "Cannot read file     %l: \n%2. ")
                                        . arg (fileName)
                                        .arg(file. errorString() fl ;
               return;
         }

         QXmllnputSource xxnllnputSource (& file) ;
         if (reader.parse ( xnillnputSource) )




앞의 예제 소스 코드에서 reader는 구현한 saxParser 클래스의 인스턴스이다. QXmllnputSot크ce 클
래스가 파일로부터 읽어온 XML 문서의 인스턴스를 reader 인스턴스의 인자로 넘겨준다. parse( ) 함수
가 호출되면 XML 문서의 태그가 발견되면 startElement, endElement, characters 이벤트 핸들러
함수가 자동으로 호출된다．


                                                   m 回1m
     I出e                       L어默山n
      4 Qt 4,8 Reference
                               http://qt-projectorg/doc/qt-4.8/
     4 Qt 5.0 Reference
                               http://qt-project.org/doc/qt-5.0/
     4 Qt developer communty
                               http://ww나.qt-dev.com/




（그림） SAX 방식의 예제 실행 화면




328 CHAPTER 11 XML


===== PAGE 330 =====
    CHAPTER




데이터 커뮤니케이션과
  인터넷 프로그래밍


===== PAGE 331 =====
Qt 5 Programming




F 1 」／네트워크
            아에서 제공하는 Socket AP를 이용해 네트워크 어플리케이션을 개발하는 방법에 대하1 알아보도록
            하자．




Qt에서 제공하는 Network 모듈은 TCP/II) 프로토콜 기반의 클라이언트와 서버 어플리케이션을 작성하
는 클래스를 제공한다. Low 레벨의 네트워크 접근을 위해 QTcpSocket, QTcpServer, QUdp
                                                    Socket
과 같은 클래스를 이용해 Low 레벨의 네트워크 클래스를 제공하여 일반적인 프로토콜을 사용해1 네트워
크 동작을 수행하기 위한 QNetworkRequest, QNetworkReply, QNetworkAccess 八4anager 클래스
를 제공한다．

표준 네트워크 라이브러리를 사용하는 것보다 쉽고 빠르게 네트워크 응용 어플리케이션을 작성할 수 있다．


心 （가에서 제공하는 Network 클래스

클라낱                       설명
QAbstractNetworkCache     Cache 구현을 위한 인터페이스 제공 클래스
OAbstractSocket           모든 Socket 타입에 제공되는 BASE 클래스
QAuthenticator            인증 오브젝트
QDnsDomainNameRecord      도메인 네임 레코드와 관련된 정보를 저장하는 클래스
QDnsHostAddressRecord     호스트 어드레스 레코드와 관련된 정보를 저장하는 클래스
QDnsLooku口                DNS looku口 클래스
oDnsMailExchangeRecord    DNS MX 레코드 정보를 저장하는 클래스
QDnsServiceRecord         DNS SRV 레코드 정보를 저장하는 클래스
QDnsTextRecord           DNS TXT 레코드 정보를 저장하는 클래스
QHostAddress             IF) 어드레스 관련 클래스
QHostln幻                 Looku口을 위한 호스트 네임 기능
QHtto卜爪거tiPart           HTTP 상에서 전송하는 MIME multipart 메시지와 유사한 클래스
QHttpPart                HTTP m네ti口art t川ME 메시지 내부에서 사용하는 B（그dy 부분을 지정하는 클래스
QLocalServer             ' 서버 기반의 로컬 소켓을 위한 클래스
QLocalSocket             로컬 소켓을 지원하기 위한 클래스
QNetworkAccessManager    네트워크로부터 데이터를 송／수신 응답 처리를 위한 클래스
QNetworkAddressEntry     作：>, Netmask 등 네트워크 정보를 저장
QNetworkCacheMetaData    Cache information


330 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 332 =====
클래스                            설명
QNetworkContiguration          네트워크 액세스 포인트 설정을 위한 클래스

QNetworkContigurationManager   시스템의 네트워크 설정을 관리하71 위한 클래스

QNetworkCookie                 네트워크 Co아de를 사용하71 위한 클래스
QNetworkCookieJar              QNet幻rkCookie 오브젝트의 단순 Jar 구현 클래스
QNetworkDiskCache              기본적인 디스크 Cache

ONetworkintert ace             호스트 네트워크 'P와 네트워크 인터페이스 리스트

QNetworkProxy                  네트워크 Layer 아oxy

QNetworkProxyFactory           ON이workProxy를 확장한 클래스

QNetworkProxyQuery             소켓에서 Proxy S아ting을 쿼리하기 위해 사용하는 클래스

QNetworkReply                  ONetworkAccessManager를 이용해 데이터와 헤더가 포함된 메시지를 전송하기
                               위한 클래스

QNetworkRequest                QNet\사orkAccessManager를 이용하1 데이터를 전송하71 위한 클래스
QNetworkSession                네트워크가 접근 가능한 액세스 포인터부터 플랫폼의 액세스 포인터를 관리하71 위
                               한 클래스
QSocketNotifier                네트워크부터 알림 메시지를 모니터링 하기 위한 클래스
Os읾Certifica伯                  X509 인증 API
OSsiCertificateExten듸on        X509 Certific欲e의 확장 AP를 제공하71 위한 클래스

OSsiCipher                     SSL 암호인증 Cipher(열쇠） 지원을 위한 클래스
OSsiConfiguration              SSL 연결 상태와 설정을 지정하기 위한 클래스
Os引Error                       SSL 에러 처리

 QSslKey                       Pri始m과 Public keys 인터페이스

 Os引Socket                     클라이언트와 서버 간의 Ss匕 암호화된 소켓 지원 클래스

 QTcpServer
 QTcpSocket                    TCP socket

 QUdpSocket                    UDP socket

 QUrl                          URL로 동작하는 인터페이스를 지원하기 위한 클래스




Bearer Management를 위한 QNetworkConfiguration, QNetworkConfigurationManager,
                                                                      사이
QNetworkSession과 같은 클래스를 제공한다. Bearer Manageme砒는 네트워크 Access 포인트
의 데이터를 전송하는 데이티의 전송 경로 혹은 네트워크 디바이스 장치어］ 대한 Start와 St아） 인터페이
스를 사용할 수 있다. 따라서 Bearer 八/1anagem아d는 네트워크 시스템의 Contr아과 연결
 (Connectivity) 상태를 관리할 수 있다．




                                                                             1 네트워크 331


===== PAGE 333 =====
 0Bearer Management의 Mapping Type

 aearerType              Va山e
 BearerUnknown           Unknown type
 BearerEthernet          타hernet
 BearerWLAN              쌔r이的S LAN
 Bearer2G                2G
 BearerCDMA2OOO          CDMA2000
 BearerWCDtvlA           WCDMA
 BearerHSPA              HSPA
 BearerBluetooth         미ueto아h
 BearerWiMAX             WIMAX



. at 네트워크 모듈을 사용하기 위한 헤더 파일과 프로젝트 추가사항
Qt에서 제공하는 네트워크 모듈을 사용하기 위해 다음과 같이 혜더 파일을 추가한다．

 孝include <Q七Nets了ork>


qmake의 프로젝트（.pr이 파일어］ 다음과 같이 네트워크 모듈을 추가해야 한다．

 QT += network



0QTcpSocket고1QTc口Server 클래스를 사용한 TOP 프로토콜 기반 프로그래밍
TCP(Tran町ni弱幻II（幻ntr아 Pr毗ocol)는 일반적으로 가장 많이 사용하는 인터넷 프로토콜 중 하나이
며 Low 레벨 네트워크 프로토콜을 사용해 서버와 클라이언트 간의 신뢰성 있는 네트워크 어플리케이션
을 구현할 수 있다．

QTcpSocket 클래스는 TCP 프로토콜을 지원하기 위해 제공하는 클래스이며 POP3, SMTP, NNTP와
같은 표준 네트워크 프로토콜 기반 어플리케이션을 구현할 수 있다. 뿐만 아니라 QTcpSocket 클래스는
사용자가 정의한 커스텀 프로토콜을 구현할 수 있다．

TCP 연결은 원격지 상에 존재하는 호스트와 네트워크를 경유하여 신뢰성이 보장된 데이터를 전송할 수
있는 녜트워크 연결을 보장한다. TCP는 원격지 상어］ 존재하는 Peer간 네트워크 연결을 위해 II) 어드레
스와 Port를 사용한다. QTcpSocket 클래스에서는 peerAddress( ）와 peerPort( ) 멤버함수를 사용할
수 있다．

QTcpSocket 클래스는 현재 네트워크 상태와 에러가 발생하는 경우 시그널 이벤트를 통해 비동기
(Asynchronous) 방식으로 동작한다. 그리고 TCP 프로토콜을 이용하여 데이터 송수신을 위해
QTcpSocket 클래스는 wri扼（）와 read( ) 함수를 제공한다. QTcpSocket 클래스는 印ODevice 클래스
로부터 상속받은 클래스이다. 따라서 QTextStream과 QDataStream 클래스를 사용해 데이터의 스트
림 처리가 가능하다. QTcpSocket 클래스는 원격지 호스트에서 데이터를 수신받으면 byteAvailable()
멤버함수가 미리 호출되며 수신받은 데이터를 처리할 수 있는지 검증한다．


332 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 334 =====
만약 TCP 연결을 핸들링하기 위한 서버 어플리케이션을 구현하기 위해 QTcpServer 클래스를 제공한
다. TCP 연결을 위한 서버가 준비되면 listen( ) 함수를 사용해 클라이언트 연결을 기다린다. 클라이언트
가 서버어］ 연결을 시도하면 newConn吼ti아l( ) 시그널 이벤트 함수가 호출된다. 이 시그널과 연결된 슬
롯함수는 모든 클라이언트가 새로운 연결을 시도하면 단 한번만 호출되는 시그널이다. 클라이언트와 연
결이 허용되면 nextPendingConnection( ) 시그널 이벤트가 호출되고 클라이언트와 데이터 송수신을
위한 준비가 완료된다．

QTcpSocket은 비동기 방식아지만 미ockiT培을 통해 동기화（Synchronous) 방식으로 사용할 수 있다．
동기화 방식을 위해서는 waitFor 구문으로 시작하는 멤버함수를 사용할 수 있다．

waitForByteswritten(int)    : bool
wai七m그rConnec七ed(int)   : bool
waitForDisconnected(irit)   : bool
waitForReadyRead(int)   : bool




waitFor 구문으로 시작하는 함수를 사용해 클라이언트 Connection 연결을 기다리는 동기화 방식으로
구현하면 어플리케이션의 GUI 인터페이스를 Blocking 할 수 있다. 즉 사용자의 Connection 연결을 동
기화 방식으로 구현하기 위해서는 GI끄와 분리될 수 있도록 쓰레드를 사용해야 한다．


1QUdpSocket 클래스를 사용한 UDP 프로토콜 기반 프로그래밍
UDP(User Datagram Pr毗oc아）는 경량화된 네트워크 프로토콜이다. TCP와 달리 비신뢰성 기반의 연
결 프로토콜이다. 그렇기 때문에 데이터 송수신 시, 신뢰성이 보장되지 않아도 되는 멀티미디어 기반의
데이터 송수신을 위한 어플리케이션을 구현하는 데 사용한다. Qt에서는 UDP 프로토콜을 지원하기 위해
QUdpSocket 클래스를 지원한다．

QUdpSocket 클래스는 IPv4 브로드케스팅을 지원한다. 브로드케스팅은 호스트를 검색하는 것과 같은
어플리케이션 구현 시 용이하다. QUdpSocket 클래스는 로컬상에 존재하는 녜트워크 호스트 브로드케
스팅을 위해 Broadcast(255. 255. 255. 255) 함수를 사용하면 된다．

UDP 프로토콜을 사용해 데이터를 수신하기 위한 준비 단꼐로 QUdpSocket 클래스의 bind( ) 함수를
사용할 수 있다. 이 함수는 TCP 연결을 위한 QTcpServer 클래스의 listen( ) 함수와 비슷하다. QUdp
Socket은 Datagram이 도착하면 readyRead( ) 시그널 이벤트가 발생한다. 그리고 호스트로부터 들어
오는 데이터를 수신하기 위해1 readDatagram( ) 함수를 사용할 수 있다．


0QHostln幻 클래스를 사용한 호스트 네임 Res이미ng
네트워크 연결을 완료하기 전에 QTcpSocket과 QUdpSocket은 II) 어드레스로부터 연결할 수 있는 호
스트 네임을 Lookup하는 과정을 수행한다. 이러한 과정은 DNS(Domain Name Service) 프로토콜을
사용해 수행한다．

Qt에서 제공하는 네트워크 모듈은 호스트 네임을 얻어오기 위해 QHostlnfo 클래스를 제공한다．


                                                         ] 네트워크 333


===== PAGE 335 =====
 QHostlnfo 클래스에서 제공하는 1ookl叩Host( ) 함수를 사용해 호스트의 네임을 얻어올 수 있다. 이 클
래스는 호스트의 이름을 Lookup하고 호스트 네임의 결과의 Lookup이 완료되면 시그널／슬롯을
                                                                              통해 이
벤트를 발생한다．

또한 이 클래스에서 제공하는 fromN跏e( ) 함수의 인자로 QString 타입의 호스트 네임을 사용해 호스
트의 'P어드레스를 질의할 수 있다．


的 Network 마oxy 지원
Qt는 로컬과 원격지상에 존재하는 호스트와의 네트워크 트래픽（Traffic）을 필터링하거나 직접 연결하기
위해 프락시（Proxy）를 지원한다. Qt에서 프락시 기능을 구현하기 위해 QNetworkProxy 클래스를 제공
한다. SCOK5로 Low 레벨상에서 녜트워크 프락시 히용을 지원하고 HTTP와 FTP 프락시가 프로토콜
레벨에서 동작할 수 있도록 지원한다．

                                벼日'Il-   i '四q町nn可In
 QNetv四rk마oxy::N아가oxy           2        프락시를 사용하지 않는다．
 QNet\사orkProxy::Defau바가oxy     0        set!＼口이（帥onProxy( ) 함수를 사용해 어풀리케이션
                                         프락시 설정을 결정하71 위한 디폴트 값
 0NetworkProxy::Socks5Proxy     ]        Socks5 프락시 사용
 ONetworkProxy::HttpProxy       3        HTTP trans口arent 프락시 사용
 ON이wo水마oxy::H螂兀配비四마oxy         4        HTTP Request만을 위한 프락시
 ONet사orkProxy::F巾Caching마oxy   5        FTP Reque없만을 위한 프락시



eBearer Management 지원
Bearer Management는 네트워크 액세스 포인트 간의 데이터 송수신과 네트워크 디바이스의 인터페이
스를 시작하거나 중지하는 것과 같은 디바이스 상태를 제어할 수 있는 기능을 지원한다. QNetwork
ConfigurationManager 클래스는 네트워크 디바이스의 연결 리스트를 관리하는 기능을 제공하며
QNetworkConfiguration 클래스는 네트워크 인터페이스를 사용해 연결을 시작하는데 사용한다．
QNetworkConfigurationManager 클래스로부터 얻어온 네트워크 연결 정보를 이 클래스의 파라미터
로 사용한다.

네트워크 연결 정보를 이용해 QNetworkSession을 사용하여 네트워크 세션을 시작할 수 있다. 이 클래
스는 네트워크 세션을 만드는데 적합하며 QNetworkConfigurati아小ilanager 클래스가 제공하는
defaultConfiguration( ) 함수에 의해 연결 구성을 리턴한다. 어떤 플랫폼에서는 네트워크 동작을 수행
하기 전에 네트워크 세션을 요구하여 사용하기도 한다．




334 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 336 =====
         ].] QTcpSock이과 QT야）Server를 사용한 TOP 프로토콜 프로그래밍

네트워크 TCP 프로토콜 기반의 클라이언트 서버 어플리케이션을 구현하기 위해 QTcpSocket과
QTcpServer 클래스를 사용한다. 이번 장에서는 TCP 프로토콜을 사용해 구현된 Forturne C1ie1此와
Forturne Server 예제를 살펴보도록 하자. 이 예제는 Qt를 설치하면 기본으로 제공하는 네트워크 예제
에 포함되어 있다．


0Fortune Server 예제 어플리케이션
이 예제 어플리케이션은 클라이언트와의 연결을 위해 QTcpServer 클래스를 사용하며 클라이언트와 더］
이터 송수신을 위해1QDataStream 클래스를 사용해 데이터를 스트림으로 송수신한다．


I가 Fortune Serve口                        1   뇜


     The server is running on
  IP: 1
  口ort: 텨905
  日un the Fortune Client example now.

                                  Quit


（그림） Fortune Server 실행 화면



 class Server : public QDialog
 {
         Q OBJECT

 public:
          Server (QWidget *parent = 0) ;


 private slots:
     void sessionOpened( );
     void sendFortune () ;

 private:
          QLabel *statusLabel;
          QPushButton *quitButtofl.
          QTcpServer *tcpserver;
          QStringList fortunes;
          QNetworkSession *networksessjon;
  };


 클라이언트 호스트로부터 연결 요청이 발생하면 핸들링하기 위해 단지 하나의 슬롯을 사용한 단순하게
 구현된 서버이다．



                                                        1 네트워크 335


===== PAGE 337 =====
    tcpServer = new QTcpServer (this) ;
    if      (! tcpServer->listen () ) {
             QMessageBox: :critical (this,                    tr ( "Fortune Server ") ,
                                                      tr ( "Unable to start the server: %1. ")
                                                      .arg(tcpServer->errorString () ));
            close () ;
            return;
    }
    QString ipAddress;
    QList<QHostAddress> ipAddressesList = QNetworklnterface: :allAddresses () ;
    // use the firs七 non叫1（그calhos七 IPv4 address
    for (mnt i = 0; i < ipAddressesList. size () ; ++i) {
         if (ipAddressesList.at (i) 1= QHostAddress: :LocalHost &&
             ipAddressesList. at (i) .toIPv4Address () ) {
             ipAddress = ipAddressesList.at (i) .toString () ;
             break;
            }
    }
    /7 if       we did not find one, use IPv4 localhost
    if   (ipAddress. isEmpty () )
        ipAddress = QHostAddress (QHostAddress: :LocalHost) .toString () ;
    statusLabel->setText (tr ( "The server is running on\n\nIP: %1\nport: %2\n\n"
                               "Run the Fortune Client example now. ")
                               .arg(ipAddress) .arg(tcpServer->serverPort () ));



소스 코드에서 보는 것과 같이 생성자에서는 QTcpServer 클래스의 listen( ) 함수를 사용해 클라이언트
호스트로부터 연결 요청을 기다리는 Listen 대기 모드로 진입한다. 그리고 클라이언트가 서버의 II) 어드
레스와 PORT 정보를 어플리케이션 GUI 상의 라벨 위젯에 출력한다．

클라이언트와 새로운 연결이 완료되면 서버는 클라이언트에게 다음과 같은 메시지를 차례대로 전송한다．

    fortunes << tr ( "You've been leading a dog's life. Stay off the furniture. ")
              << tr ( "You've got to think about tomorrow. ")
              < < tr ( "You will be surprised by a loud noise.
                                                               ")
              << tr ( "You will feel hungry again in another hour.
                                                                   ")
                   << tr ( "You might have mail. ")
                   << tr ( "You cann毗 kill 七ime wi七hou七 injuring e七erni七y. ', )
                   << tr ( "Computers are not intelligent. They only think they are. ") ;


Fortunes에 저장된 메시지는 랜덤하게 연결된 클라이언트에게 전송한다．

F
connect (tcpServer,         SIGN2L   (newConnection
                                                                  () ), this,   SLOT   (sendFortune
                                                                                                      () ));

새로운 연결이 발생하면 newConnection( ) 시그널 이벤트가 sendFortune( ) 슬롯함수와 연결된다.
                                                        따
라서 새로운 클라이언트가 연결 요청이 들어오면 new（兀nne毗mn 시그널이 발생하며 이 시그널과 연결
된 sendFortune( ) 슬롯함수가 호출된다．



336 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 338 =====
void Server: :sendFortune()
{
     QByteArray block;
     QDataStrean Out (&block, QlODevice: :Writeonly) ;
     out. setVersion(QDataStream: :Qt 5 2) ;



如rtunes 변수에 저장된 리스로부터 랜덤하게 클라이언트에게 메시지를 전달하려는 목적으로 QByte
Array 데이터를 QDataStream 클래스의 스트림을 통해 Encode된다. 이러한 방법은 소켓어］ 연결된 호
스트에게 데이터를 전송하기 위한 방법이다. 여기서 클라이언트와 통신하기 위한 버전으로 QData
Stream의 Qt_5그 프로토콜 버전을 설정한다. 설치한 Qt 버전에 따라 프로토콜 버전이 달라진다. 따라
서 QDataStream: :version을 참조해 사용해야 한다．

    out << (quintl6) 0;
    out << fortunes .at (qrand() % fortunes. size ( ) );
    out.device ( 尸>seek (0) ;
    out << (quintl6) (block. size () - sizeof (quintl6) );



QByteArray의 시작 부분에 전송할 데이터의 전체 사이즈를 포함하는 l6bit Integer를 포함한다. 이러
한 방식은 클라이언트가 전체 데이터를 전송받기 전에 데이터의 전체 사이즈를 미리 알 수 있는 기능을
제공한다．

    QTcpSocket *cljentconnectjon = tcpServer->nextPendingConnection( ) ;
    connect (clientConnection, SIGNAL (disconnected( )),
              clientConnection, SLOT (deleteLater ( )));



nextPendingConnection( ) 함수를 사용해 연결된 클라이언트가 연결이 종료되면 disconnected( ) 시
그널 이벤트 함수가 호출할 수 있는 기능을 제공한다. 예제와 같이 discoonected( ) 시그널이 발생하면
deleteLater( ) 슬롯함수가 호출된다．

    clien七Connec七ion->.寸ri土e(block) ;
    clientConnection->disconnectFrornHost ( );
}


write( ) 함수를 사용해 연결된 클라이언트에게 Ei乂ode된 데이터를 전송하고 클라이언트 연결을 종료한
다. 연결을 종료하기 위하1disconnectFromHost( ) 함수를 사용한다. 이 함수가 사용되면 connect( )
함수에 연결된 시그널과 슬롯함수가 호출된다．


0Fortune Client 예제 어플리케이션
이 예제는 QTcpSocket 클래스를 사용하며 이전의 Fortune Client 서버와 접속해 서버로부터 메시지를
수신받는다．




                                                                           1 네트워크 337


===== PAGE 339 =====
 自Fortune Client                                             ［因唯m
     Server name: locaihost
     Server port:
                61905
     Th冶 exam미es requires that 90U run the Fortune S日rver exam미e as 叫a比
                                               Get Fortune     Quit


（그림） Fortune Client 실행 화면


이 예제에서는 서버로부터 전달받은 메시지 데이터를 QDataStream을 사용해 데이터를 처리한다．
Client는 Server에게 연결을 요청하고 연결이 완료되면 서버에서 메시지를 Client에게 전달한다．
Client는 Server에게 텍스트를 요청한다. 요청한 텍스트에는 l6bit의 Integer 값이 포함되어 있다. 이
값은 서버로부터 수신한 메시지의 전체 사이즈가 포함된다. QTcpSocket은 네트워크 프로그래밍에서 다
음과 같은 두 가지 방식을 지원한다．


. 비동기（Asynchronous 혹은 non-Blocking) 방식의 접근
이 방식은 비동기 방식으로 스케줄화된 방식으로 동작하며 Qt의 Event loop에서 제어한다. 비동기 방식
은 QTcpSocket에서 제공하는 시그널／슬롯을 통해 제공한다. 예를 들어 QTcpSocket 클래스에서 제공
하는 connected( ) 시그널을 제공한다. 이 시그널은 호스트와 연결 요청이 들어오면 시그널 이벤트가 호
출된다．


0 동기（Synchronous 혹은 테ocking) 방식의 접근
이 방식은 동기화 방식으로 non-GI끄와 같은 어플리케이션과 멀티 쓰레드 기반의 어플리케이션에서 사
용한다. 호스트로부터 연결 요청이 있을 때까지 미ocking 할 수 있는 기능을 제공한다. Blockir培을 하
기 위해 QTcpSocket 클래스의 waitForConnectecl( ) 함수를 사용하면 된다. 만약 GI끄를 사용하는 어
플리케이션에서 引ocking을 사용하면 사용자 GUI 이벤트로부터 발생하는 모든 처리 이벤트가
미ocking 되므로 GUI 루틴과 분리해야 한다．

이번 예제에서는 비동기 방식의 접근하는 방식에 대해서 먼저 살펴보도록 하자. 클래스의 혜더 파일은 다
음과 같다．

 class Client : public ODialog
 {
        Q OBJECT

public:
        Client (QWidget *parent = 0) ;


private slots:
        void requestNewFortune () ;
        void readFortune ( ) ;
        void displayError (QAbstractSocket: :SocketError socketError) ;
        void enableGetFortuneButton 1 1;
                                                                          0

338 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 340 =====
         void sessionopened() ;


    priva七e:
         QLabel *hostLabel;
         QLabel 枉均r七Label;
         QComboBox 士hostCon由O;
         QLineEdit 柱刃r比ineEdit;
         QLabel * statusLabel;
         QPushButton * getFortuneButton;
         QPushButton *quitButton;
         QDialogButtonBox *buttonBox;


         QTcpSocket *tcpsocket;
         QString currentFortune;
         quint16 blockSize;


         QNetworkSession *networkSession;

    };
.
이 클래스에서는 QTcpSocket 포인터가 포함된 데이터 멤버와 GUI상어］ 사용할 위젯 포인터가 정의되어
있다. Socket은 이 클래스의 생성자에서 초기화 과정이 구현되어 있다．

    Client: :Client (QWidget *parent) : QDialog(parent) , networkSession(O)
    {

         tcpSocket = new QTcpSocket (this) ;



이 예제에서는 단순히 QTcpSocket 시그널로 호스트로부터 메시지 수신이 들어오면 시그널 이벤트가 발
생하도록 구현되어 있다. 그리고 error( ) 시그널은 서버와 연결된 Connection이 에러가 발생하는 예외
처리를 위한 시그널이다．


         connect (tcpSocket, SIGNAL (readyRead() ), this,   SLOT (readFortune () ));
         connect (tcpSocket, SIGNAL (error (QAbstractSocket: :SocketError) ),


    }


이 예제의 GUI 상에서 [Get Fortune] 버튼을 클릭하면 requestNewFortune( ) 슬롯함수가 호출된다．

    void Client: :requestNewFortune ()
    {
         getFortuneButton->setEnabled(false) ;
         blockSize = 0;
         tcpSocket->abort () ;
         tcpSocket->connectToHost ( hostCombo->currentText () ,
                                    portLineEdit->text ( ) .tolnt () );

巳
                                                                                       1 네트워크 339


===== PAGE 341 =====
이 슬롯함수는 호스트로부터 수신받는 새로운 블록 데이터를 읽어 들이기 위해 0의 값으로 설정한다. 왜
냐하면 Connection이 종료되고 사용자가 [Get Fortune] 버튼을 클릭할 수 있도록 허용하기 위함이다．
QTcpSocket 클래스의 ConnectT아｛ost( ) 함수가 호출되면 凡rtune server에 연결 과정이 수행하기
전에 [JI상어］ 서버의 호스트 네임과 PORT 번호를 참조해 서버에 연결을 요청한다．

connectToHost( ) 함수가 호출된 결과로 다음과 같은 두 가지 중 하나가 발생한다．


. 연결（Connection)
이 경우 如rtune server와 연결이 완료되고 서버로부터 메시 지를 수신 받으므로 QTcpSocket 클래스의
readyRead( ) 시그널 이벤트가 발생한다．


. 에러 발생
이 경우 如rtune server와 연결을 실패하는 경우이다. 서버와의 연결을 실패하면 QTcpSocket 클래스
의 error( ) 시그널 이벤트 함수가 호출되고 이 시그널과 연결된 displayError( ) 슬롯함수가 실행된다．

void Client: :displayError (QAbstractSocket: :SocketError socketError)
{
     switch (socketError) {
     case QAbstractSocket: :RemoteHostClosedError:
         break;
     case QAbstractSocket: :HostNotFoundError:
         QMessageBox: :information(this,     tr ( "Fortune Client ") ,
                                                                                      n
                                    tr ( "The host was not found. Please check the
                                       "host name and port settings. ") );
         break;
     case QlthstractSocket: :ConnectionRefusedError:
         QMessageBox: :information(this,     tr ( "Fortune Client ") ,
                                    tr ( "The connection was refused by the peer. '
                                       "Make sure the fortune server is running,
                                       "and check that the host name and port !1
                                       "settings are correct. ") );
         break;
     default:
         QMessageBox: : information(this,    tr ( "Fortune Client ") ,
                                    tr ( "The following error occurred: %1. ")
                                    .arg(tcpSocket->errorString() ));
     }

     getFortuneButton->setEnabled( true) ;
 }



소스 코드에서 보는 것과 같이 error( ) 시그널 이벤트가 발생하면 displayError( ) 함수가 발생한다．
QMessageBox: nj寸orm毗ion( ) 함수를 사용해 다이얼로그에 발생한 에러를 표시한다 ．다이얼로그가
화면상에 출력되고 다이얼로그 GUI 상에 [OK] 버튼을 클릭하면 [Get Fortune] 버튼이 활성화 된다．


340 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 342 =====
r
洹3Fortune Client

                 The connection was refused by the peer. Make sure the fc戊une server is
                 running, and check that the host name and 四rt settings are correct




（그림） error() 이벤트 시그널이 호출되면 다이얼로그에 에러 로그가 출력



이와 반대로 서버와 연결이 정상적으로 완료되면 fortune server로부터 메시지를 수신받는다. 메시지를
수신받으면 readyRead( ) 시그널 이벤트 함수가 발생한다. 이 시그널이 발생하면 연결된 read
Fortune( ) 슬롯함수가 호출된다．

    void Client: : readFortune ()
    {
            QDataStream in (tcpSocket) ;
            in. setVersion(QDataStream: :Qt_5_2) ;


            if     (blockSize == 0) {
                    if (tcpSocket->bytesAvailable () < (int) sizeof (quintl6) )
                           return;


                     in >> blockSize;
            }

            if      (tcpSocket->bytesAvailable() < blockSize)
                     return;



    이 예제에서 TCP 프로토콜은 QDataStream을 경유해 데이터를 처리한다. 이 스트림으로부터 데이터
    스트림의 버전을 설정하기 위해 setVersion( ) 함수를 사용한다. 이 함수에서 사용하는 QDataStream::
    Qt戶그 인자는 스트림 버전이며 클라이언트와 서버가 같은 버전을 사용해야 한다. 현재 이 예제에서
    T（刃 프로토콜을 사용해 경유하는 데이터 스트림 기반으로 데이터를 전송한다．
    readyRead( ) 함수는 새로운 데이터가 도착하면 네트워크를 통해1 들어오는 데이터를 QTcpSocket 클래
    스의 버퍼어］ 저장한다. 그리고 작은 사이즈로 나누어진 Fragment 단위로 데이터를 수신받는다．

    [6giring flex七For七une;
            in >> nextFortune;

             if     (ne:＜七For七une == curren七For七une) {
                     OTimer: :singleShot (O, this, SLOT (requestNewFortune () ));
                      return;
             }

             currentFortune = nextFortune;
             statusLabel->setText (currentFortune) ;
             getFortuneButton->setEnabled (true) ;
        }

                                                                                          ] 네트워크 341


===== PAGE 343 =====
 예제의 소스 코드에서 보는 것과 같이 QDataStream은 스트림 데이터를 처리하기 위한 과정이다. 서버
로부터 읽어온 데이터는 라벨 위젯의 setText( ) 함수를 사용해 GUI 상어］ 출력한다．

     I크 F아tune Client

         Server name: localhost
         Server 口orl     텨905
         You will feel hungry again in another hour.
                                                       Get Fortune   Quit


（그림） 서버로부터 수신받은 메시지를 UI 상에 출력



. 동기화（Blocking) 방식을 사용하는 Fortune Client 예제
이번 예제는 이전 예제에서 다루었던 비동기 방식의 如rtune client와 동일한 GUI 구조이다. 다른 점은
이번 예제에서는 미ockit培을 통한 동기화 방식을 사용한다. 동기화 방식으로 클라이언트서버 어플리케
이션을 구현할 때 멀티 쓰레드 기반으로 구현해야 한다．

동기화 방식은 호스트로부터 응답을 받을 때까지 Blocking 된다. 만약 호스트로 응답 이외에 다른 처리
과정으로 이벤트가 처리된다면 호스트가 응답할 때까지 어플리케이션 전체가 Blockit培의 영향을 받는
다. 예를 들어 GUI 기반의 어플리케이션에서 QTcpSocket의 Blockir培으로 인해 GI끄가 응답을 받지
못한다. 그렇기 때문에 Blocking이 포함된 처리과정은 쓰레드를 이용해 처리해巾乍 한다．

이번 예제에서 사용한 동기화 방식의 처리는 QThread를 사용한다. 구현할 클래스의 헤더 구조는 다음과
같다．

     class FortuneThread : public QThread
     {
            Q OBJECT

public:
            For七uneThread ( Qobj ec七 柱冶rent = 0) ;
            -FortuneThread() ;


            void requestNewFortune (const QString &hostName, quintl6 port) ;
            void run() ;


 signals:
            void newFortune(const QString &fortune) ;
            void error (int socketError, const QString &message) ;

priva七e:
            OString hostName;
           quint16 port;
           QMutex mutex;
           QWaitCondition cond;
           bool quit;
};
342 CHAPT타212_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 344 =====
구현한 FortuneThread 클래스는 서버로부터 요청을 처리하기 위한 API로 구성되며 QThread 클래스
를 상속받았다. 어플리케이션에서 [Get Fortune] 버튼을 클릭하면 requestNewFortune( ) 함수가 수
행된다. 이 함수는 구현한 FortuneThread 클래스의 requestNewFortune( ) 멤버함수를 호출한다．
requestNewFortune( ) 함수에서 서버의 호스트명과 포트 번호가 동시에 변경되지 않도록 QM毗ex를
사용해 동기화 처리하였다．

void FortuneThread: :requestNewFortune (const OString &hostN帥［le, quintl6 port)
{
    QMutexLocker locker (&mutex) ;
    七his->hos七Name = 뇨＞S七Name;
    七his->port = por七；
    if   ( ! isRunning( ))
           start () ;
    else
          cond.wakeOne () ;
}


requestNewFortune( ) 함수가 수행되면 GUI 쓰레드에서 구현한 Fortune 클래스의 쓰레드가 실행된다．

void FortuneThread: :run()
{
    mutex. lock() ;
    QString serverName = hostName;
    quintl6 serverPort = port;
    mutex.unlock ( );


    while ( ! quit)       {
          const mnt Timeout = 5 * 1000;


          QTcpSocket socket;
              socket.connectToHost (serverName, serverPort) ;



run( ) 함수에서는 다시 한번 멤버변수를 동기화한다. while 구문의 루프는 서버로부터 Connection 연
결을 요청하기 위해 connectToHost( ) 함수를 수행한다. 서버로부터 요청이 있을 때까지 Blocking될
수 있도록 waitForConnected( ) 함수를 호출한다. 이 함수는 서버로부터 응답을 받을 때까지 Blocking
한다. 이 함수의 첫 번짜1 인자는 millisecond이다. 지정한 millisecond 만큼 서버로부터 연결 응답을 기
다린다. 지정한 시간을 초과하면 에러를 리턴한다．

         if       ( !socke七．wai七ForConne（北ed ( Timeou七）) {
                    emit error (socket.error () , socket.errorString() );
                    return;
              }




                                                                             1 네트워크 343


===== PAGE 345 =====
 예제의 소스 코드에서 보는 것과 같이 인자로 지정한 Timeout millisecond만큼 서버로 연결 요청을 받
을 때까지 Blocking 된다. 이후 서버로부터 메시지 응답을 받을 때까지 Blocking 처리가 가능하다. 메
시지를 받을 때까지 틔ocking 하기 위해서는 waitForReadyRead( ) 함수를 사용하면 된다．

       while (socket.bytesAvailable () < (int) sizeof (quintl6) ) {
                  if ( ! socket.waitForReadyRead(Timeout) ) {
                       emit error (socket.error ( ) , socket.errorString() );
                       return;
                   }
        }




            QUdpSocke욜 사용한 UDP 프로토콜

QUdpSocket 클래스는 UDP(User Datagram Pr毗ocol) 소켓을 사용해 네트워크 어플리케이션을 구
현하기 위한 기능을 제공한다. UDP는 호스트로부터 송／수신한 데이터 패킷의 전송이 제대로 되었는지
보장하지 않는다．

TCP는연결 ' ］향프로토콜어］ "］해UDP는 " 1연결 ' ］향프로토콜이다· 따라"I UDP프로토콜은패킷을                    I
송수신하는호스트간데이터 신뢰성읔보장하지 않는 " 1디오 "가 ' 1터를 기
                                        '리가기 위흐I-     프로토콜로주로                   I
활용된다· 예를들어 멀티 " 1디어 "11O1터를 "II트워크를통 '개 송수신하는 경우 일부 패킷 ' 1 손실되 " 忙十도            I
멀티 " 1디어 "가 ' 1터를 4
                  '리가는 " 11 又］장' ] 없기 때문' ］다· 따라서 UDP프로토콜은대량의 " 가 " 1터를수신       I
하는 프로토콜로 활용한다.
                                                                                I
또한 UDP 프로토콜은 비연결 지향이므로 TCP 프로토콜어］ 비해 구현이 간단하며 비연결 지향이므로 녜
트워크를 경유해 대량의 데이터를 전송하는 TCP 보다 빠르게 패킷을 처리할 수 있다．

Qt에서는 UDP 프로토콜을 구현하기 위해 QUdpSocket 클래스를 제공한다. QUdpSocket 클래스는
QAbstractSocket 클래스의 하위 클래스이며 UDP 프로토콜을 사용해 Datagram을 전달할 수 있다．
UDP를 사용해 특정 호스트로 데이터를 송수신하기 위히1QUdpSocket 클래스의 bind( ) 함수를 사용한
다. Datagram을 전송하기 위해 wri扼Datagram( ) 함수를 제공한다. 반대로 데이터를 수신받기 위해
서는 readDatagram( ) 함수를 제공한다.

만약 QUdpSocket을 사용해 특정 호스트와 연결하기 위해1 connectToHost( ) 함수를 사용해 직접 연결
할 수 있다. 만약 네트워크상에 특정 호스트에게 Datagram을 전송하는 경우 bind( ) 함수를 사용하지
않고 bytesWritten( ) 함수를 사용해 직접 Datagram을 전송할 수 있다．

특정 호스트로부터 데이터를 수신받는 경우 QUdpSocket은 비동기화 방식으로 Datagram을 수신받을
수 있도록 readyRead( ) 시그널 이벤트 함수를 제공한다. 이 시그널을 사용하면 네트워크 상에
Datagram이 수신되면 시그널 이벤트가 발생한다．




344 CHAPTER 12.. 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 346 =====
void Server: :initSocket ()
{
        udpSocket = new QudpSocket (this) ;
        udpSocket->bind(QHostAddress: :LocalHost, 7755) ;


        connect (udpSocket, SIGNAL (readyRead1 )),
                 this, SLOT (readPendingDatagrams ( ) ));
}

void Server: :readPendingDatagrams ()
{
        while (udpSocket->hasPendingDatagrarns () ) {
            QByteArray datagram;
            datagram.resize (udpSocket->pendingDatagramSize () );
            QllostAddress sender;
            quint16 senderPort;


            udpSocket->readDatagram(datagram.data() , datagram. size () ,
                                    & sender, &senderPort) ;


             processTheDatagram( datagram) ;
        }
    }


또한 QUdpSocket 클래스는 멀티케스트（multicast）를 지원한다. 운영체제 플랫폼에서 사용하는 네트워
크 디바이스에서 설정된 네트워크 그룹을 지정해 멀티케스트 메시지를 전달할 수 있다. 로컬 녜트워크상
그룹어］ 메시지를 전달하기 위해 如inMulticastGroup( ）와 leaveMulticastGroup( ) 함수를 사용할 수
있다．

그리고 QUdpSocket 클래스는 connectToHost( ) 함수를 사용해 UDP 서버로 접속하여 데이터의 송수
                                                                송
신이 가능하다. 데이터 송수신을 하기 위해서 read( ）와 wri扼（) 함수를 통히1UDP 서버로 메시지를
수신할 수 있다．

QUdpSocket 클래스는 UDP 서버로부터 연결을 끊기 위해서 disconnectFromHost( ) 함수를 제공한
                                                                 방
다. 이 함수를 사용하면 연결된 UDP 서버로부터 연결을 끊을 수 있다. 또한 연결을 끊기 위해 동기화
식을 사용할 수 있다．

    socket->disconnectFrornHost () ;
        if (socke七->sta七e ( ) == 아山S七rac七Socke七：: iJnconnec tedS七a七e H
            socket->waitForDisconnected( 1000) }
              qDebug ( "Disconnected! ") ;



예제의 소스 코드에서 보는 것과 같이 waitF야Disconnected( ) 멤버함수를 사용하면 UDP 서버로부터
                                                           . 지정한
연결을 끊을 때까지 Blocking 할 수 있다. 이 함수는 인자로 TIMEOUT 시간을 지정할 수 있다
    인자의 시간 동안 UDP 서버와 연결을 끊기 위해 Blocking 한다．

                                                                            1 네트워크 345


===== PAGE 347 =====
 bool QAbstractSocket: :waitForDisconnected(int msecs = 30000) [virtual]



 . 브로드케스트를 이용한 메시지 송수신 예제
 브로드케스트를 이용한 예제는 Broadcast Sender와 Broadcast Receiver 예제를 살펴보도록 하자. 이
 예저］ 어플리케이션은 Qt가 설치되면 기본으로 제공하는 Example 어플리케이션에 포함되어 있다．
Broadcast Sender는 UDP 프로토콜을 이용해 메시지를 전송하고 Broadcast Rece加er는 메시 지를 수
신한다．




     Now broadcasting datagrarn 19           9eceived datagram: 'Broadcast message 19"

                                     Quit                      Quit


（그림） 마oadcast Sender오fBroadcast Receiver 어플리케이션 실행 화면



그림에서 보는 것과 같이 왼쪽 어플리케이션은 Broadcast Sender이고 오른쪽은 Receiver이다．
Sender 어플리케이션에서 [Start] 버튼을 클릭하면 시그널 이벤트와 연결된 startBroadcasting( ) 슬
롯함수가 실행된다. 이 함수는 l000millisecond 단위로 timer를 호출한다．

timer가 l000milisecond 단위로 시그널 이벤트가 발생하면 broadcastDatagram( ) 슬롯함수를 반복
해 호출한다．

 Sender: : Sender ( QWidget *parent) : QWidget (parent)
 {
        statusLabel = new QLabel (tr ( n Ready to broadcast
                                            datagrams on port 45454 ") );

        startButton = new QPushButton (tr ( "&Start ") );


       timer = new QTimer (this) ;
       udpSocket = new QUdpSocket (this) ;
       messageNo = 1;


       connect (startButton, SIGNAL (clicked() ), this, SLOT (startBroadcasting()
                                                                                  ));
       connect (quitButton, SIGNAL(clicked( ) ), this, SLOT (close () ));
       connect (timer, SIGNPL(timeoutU) , this,             SLOT (broadcastDatagram(fl) ;


구현한 Sender 클래스의 생성자에서 [Start] 버튼을 클릭하면 startBroadcasting( ) 슬롯함수가 수행
될 수 있도록 connect( ) 함수를 통해1 연결하였다．




                                                                                            r
346 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 348 =====
void Sender: :startBroadcasting()
{
        star七But亢on수set氾nabled(false ) ;
        timer->start (1000) ;




startBroadcasting( ) 슬롯함수는 timer를 1초 단위로 반복해 시그널 이벤트가 발생한다. 생성자에서 선
언한 connect( ) 함수어써 timer 시그널 이벤트가 발생하면 broadcastDatagram( ) 함수가 호출된다．

void Sender: :broadcastDatagram( )


        statusLabel->setText (tr ( "Now broadcasting
                                         datagra끄 듬1" ) .arg(messageN이 ) ;


        QByteArray datagram = "Broadcast message " + QByteArray: :nuniber (messageNo) ;
        udpSocket->writeDatagrain(datagram. data () , datagram. size () ,
                                  QHostAddress: :Broadcast, 45454) ;


        ++messageNo;




이 슬롯함수에서는 45454 포트를 사용해 메시지를 Receiver 어플리케이션이 동작하고 있는 모든 로컬
네트워크 호스트에게 Datagram 메시지를 wri扼Datagram( ) 함수를 사용해 전송한다. Broadcast
Receiver 어플리케이션은 Sender가 보낸 멀티케스트 메시지를 수신한다．

!Receiver: :Receiver (QWidget *parent) : QWidget (parent)
    {
        statusLabel = new QLabel (tr ( "Listenirtg for broadcasted messages ") );
        5七a七usLabei->se七i妃rdWrap ( 七rue) ;
        quitButton = new QPushButton (tr ( "&Quit "fl;


        udpSocket = new QUdpSocket (this) ;
        udpSocket->bind(45454, QUdpSocket: :St.areAddress) ;


        connect (udpSocket, SIGNIL (readyRead ( )),
                 this, SLOT (processPendingDatagrams (fl) ;
        connect (quitButton, SIGNAL(clicked(fl, this, SLOT (close (fl) ;




예제의 소스 코드는 Broadcast Rece如er의 생성자이다. QUdpSocket 클래스의 bind(）를 이용해 호스
트와 연결한다. Sender로부티 브로드케스트 메시지를 전달받으면 readyRead( ) 시그널 이벤트 함수가
호출되고 이 시그널과 연결된 processPendingDatagrams( ) 슬롯함수를 수행한다．




                                                                                    l 네트워크 347


===== PAGE 349 =====
                  void Receiver: :processPendingDatagrams ()
                   {
                         while (udpSocket->hasPendingDatagrams () ) {
                              QByteArray datagram;
                                 datagram.resize (udpSocket->pendingDatagraxnSize() );
                                 udpSocket->readDatagram(datagram.data() , datagram. size() );
                                 statusLabel->setText (tr (n Received datagram: \" %1V' ")
                                                                             .arg(datagram.data(fl) ;                                     U
                          }




                  processPendingDatagrams( ) 슬롯함수가 수행되면 readDatagram( ) 멤버함수가 브로드케스트 메
                  시지를 GUI상에 출력한다．


                  S 멀티케스트를 이용한 메시지 송수신 예제
                  QUdpSocket 클래스는 로컬 호스트상어］ 존재하는 호스트들에게 멀티케스트 메시지를 전달할 수 있는
                  기능을 지원한다. 송신자와 수신자 관점에서 나누어보면 유니케스트, 브로드케스트, 멀티케스트로 구분
             할 수 있다. 유니케스트 전송 방식은 하나의 송신자가 다른 하나의 수신자에게만 메시지를 전달하는 방식
             이다．




                                                                ：卞
                              유니케스트                                      브로드케스트                                 멀E케스트

브로드케스트 전송 방식은 하나의 송신자가 모든 수신자에게 메시지를 전달할 수 있는 방식이다.
                                                   멀티케
스트 전송 방식은 하나이상의 사용자가 하나이상의 송신자에게 데이터를 전송하는 방식이다. 멀티케스트
방식은 데이터 송수신 과정이 특정 그룹에게 속한 수신자에게만 메시지를 전달한다. Qt에서 제공하는
QUdpSocket 클래스는 그룹어］ 속한 호스트에게 멀티케스트 메시지를 전송할 수 있다．

    '刃Multicast
                              Sender                                 ！
                                                                         딥   珏     )1그Pd叫「：止『1   datagram:                           川‘
                   Now sending datagram 44
                   TTL Per multicast datagrams:                                       Received                Mullicast message 44
                                                  g                          i:q
                                                                                                         :,




                                                      1而訂］ 的融鈿凡니                                               QLtR
\m二出느小mmm=
                              Hmmm겅小H크＝           mt比1m거mmmm구                      1= 1111口二；                         ;+=1




멀티케스트 예제는 메시지를 전송하는 Multicast Ser姓er와 수신하는 Multicast Receiver로 구성된다．
Multicast Sender는 메시지를 수신하는 하나이상의 Rece如er에게 멀티케스트 메시지를 전송할 수 있다．




348 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 350 =====
Sender: :Sender (QWidget; 枉冶ren七）
    : QDialog(parent)
{
        groupAddress = QHostAddress ( n127. 0. 0.1u) ;
        statusLabel = new QLabel (tr ( 'Ready to multicast datagrams to group %1
                                 on port 45454n ).arg(groupAddress. toString() fl ;


        startButton = new QPushButton (tr ( "&Start ") );


        timer = new QTimer (this) ;
        udpSocket = new QUdpSocket作his) ;
        messageNo = 1;


        connect (startButton, SIGNAL(clicked() ), this, SLOT (startSending() ));
         connect (꾸litButton, SIGNAL(clicked() ), this, SLOT (close () ));
         connect (timer, SIGNAL(timeout () ), this, SLOT (sendDatagram() ));




Sender 클래스의 생성자는 예제의 소스 코드에서 보는 것과 같이 [Start] 버튼을 클릭하면 시그널 이벤
트 함수와 연결된 startSending( ) 슬롯함수가 호출된다．

void Sender: :startSending()
{
         startButton->setEnabled (false) ;
         tixner->start ( 1000) ;
}


startSending( ) 슬롯함수는 timer 인스턴스를 시작한다. timer 인스턴스는 l000millisecond 단위로
타임아웃 이벤트를 발생한다. timer가 타임아웃 이벤트를 발생하면 timeout( ) 시그널 이벤트 함수가 실
행되고 최종 연결된 sendDatagram( ) 슬롯함수가 호출된다．

    void Sender: :sendDatagram()
    {
         statusLabel->setText (tr ( '1 Now sending datagram %1" ) .arg(messageNo) );
         QByteArray datagram = "Multicast message " +
                                               QByteArray: :nu曲er (messageNo) ;
         udpSocket->writeDatagrain(datagram.da七a( ), datagram. size () ,
                                   groupAddress, 45454) ;
         ++messageNo;
    }


sendDatagram( ) 슬롯함수는 그룹어］ 등록된 모든 호스트에게 wri扼Datagram( ) 멤버함수를 이용해
메시지를 전송한다．

Multicast Receiver는 Sender에서 전송한 멀티케스트를 수신받는다．


                                                                                       1 네트워크 349


===== PAGE 351 =====
                  {
                      H小




                                                                               Qoialog (parent)
    C十小
 1Receiver:
                                 :Receiver   (QWidget   *parent)
                                                                           :



i1                         叩빠m螂，      S 켁呼쁘dreS
                            roupAddress = QHostAddress ( "127. O. O. 1 ") ;
                                                    「(n기！
                           statusLabel = new QLabel (tr          니“n .. .
                                                         'Listening for multicasted messages ") );

                           udpSocket = new QlJdpSocket (this) ;
                           udpSocket->bind (QHostAddress: :AnyIPv4, 45454, QtJdpSocket: : ShareAddress) ;
                           udpSocket->joinMulticastGroup(groupAddress) ;


                           connect (udpSocket, SIGNAL (readyRead(fl,
                                                    this, SLOT (processPendingDatagrams () ));
                           connect (quitButton, SIGNAL(clicked(fl, this, SLOT (close () ));



예제의 소스 코드는 구현한 Receiver 클래스의 생성자이다. groupAddress에 Sender 호스트 II) 어드
레스를 지정한다. bind( ) 함수는 45454 포트를 통해 Sender와 Binding 한다．

일전에 설명했던 것과 같이 멀티케스트를 수신받기 위해서 로컬 네트워크 그룹을 설정해야 한다. 따라서
예제의 소스 코드에서 보는 것과 같이 加inMulticastGroup( ) 함수를 사용해 그룹에 등록한다. 이 함수
의 인자는 QHostAddress 인스턴스를 지정하면 된다．

Broadcast Sender로부터 수신받은 Datagram을 비동기 방식으로 수신받기 위해서 시그널 슬롯을 사
용한다. Sender로부터 수신받으면 readyRead( ) 시그널 이벤트가 호출되고 이 시그널과 연결된
processPendingDatagrams( ) 슬롯함수가 실행된다. 이 함수에서는 Sender로부터 수신받은
Datagram 메시지를 Broadcast Receiver 어플리케이션 GUI어］ 메시지를 출력한다．

              void Receiver: :processPendingDatagrams ()
              {
                           while (udpSocket->hasPendingDatagraxns () ) {
                               QByteArray datagram;
                               datagram. resize (udpSocket->pendingDatagramSize () );
                               udpSocket->readDatagram(datagraxn.data() , datagram. size () );
                               statusLabel->setText (tr ( "Received datagram: \" %1\ " ")
                                                                   .arg(datagram.data() ));
                           }




                      t1.3: 호스트 네임과 DNS 검색
DQHo訓n幻 클래스를 이용한 호스트 네임 검색
Qt에서 제공하는 Network 모듈은 호스트 녜임 Res아叭ng하기 위해 QHostl沚0 클래스와 DNS를 검색
하기 위해 QDnsLookup 클래스를 제공한다. QHostlnfo 클래스는 호스트 녜임으로 II) 어드레스를 쿼
리하거나 II) 어드레스로 호스트 네임을 쿼리할 수 있는 기능을 제공한다. 이 클래스는 Static 함수를 제
공하며 비동기 방식을 사용한다. 호스트를 발견하면 비동기 방식으로 시그널 이벤트가 발생한다．


350 CHAPTER 12= 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 352 =====
II) 어드레스를 비동기 방식으로 찾기 위해서 lookupHost( ) 함수를 사용하면 된다. 이 함수는 검색하고
자 하는 호스트를 IF) 어드레스와 호스트 네임으로 검색할 수 있다. 그리고 호스트 녜임과 H) 어드레스를
발견하면 시그널 이벤트 함수와 연결된 슬롯함수가 호출된다．

/7 q七-dev. corn 호스트 네임으로 'p 어드레스 검색
QHostlnfo: :lookupHost ( "qt- dev.corn",
                             this,   SLOT (printResults (QHostlnfo) fl ;


7/ 'p 어드레스로 호스트 네임 검색
QHostlnfo: :lookupHost ( "4. 2. 2. l ",
                             this,   SLOT (printResults (Quostlnfo) ));




printResults( ) 함수는 슬롯함수이다. 호스트 네임 혹은 II) 어드레스가 검색되면 시그널과 연결된 슬롯함
수를 작성해 등록할 수 있다. 만약 호스트 네임 검색이 실패하면 error( ) 멤버함수를 호출한다. error( )
함수상에 errorString( ) 함수를 사용해 실패한 상세 설명을 참조할 수 있다．

QHostlnfo 클래스는 IDNA와 I뇨nycode 표준을 통하 국제 도메인 네임（岫ernationalized Domain
Names）을 지원한다. 로컬 호스트의 네임을 검색하기 위해 QHostlnfo 클래스의 Static 함수인 local
HostName( ) 함수를 사용하면 된다. 그리고 QHostlnfo 클래스는 호스트 네임을 사용해 등록된 II) 어
드레스 리스트를 얻어오기 위해 hostName( ) 멤버함수를 사용할 수 있다．

     Os七Info inf아


if    (! info. addresses () .isErnpty () ) {
      QHostAddress address = info. addresses ( ) . first () ;
      7/ use the first     IP address
}


호스트를 검색하면 결과로 에러를 리턴하는 경우가 있다. 이런 경우 error( ) 멤버함수를 통해 리턴된 어］
러를 다음과 같은 방법으로 참조할 수 있다．

void MyWidget: :lookedtJp(const QHostlnfo &host)
{
      if   (host.error () != QHostlnfo: :N그Error) {
           qDebug() << "Lookup failed: " << host.errorString( );
           return;
       }

       foreach (const QHostAddress &address, host. addresses () )
           qDebug() << "Found address: " << address.toString() ;
 }




                                                                           ] 네트워크 351


===== PAGE 353 =====
 0QDnsLo아（up 클래스를 이용한 DNS 검색
QDnsLookup 클래스는 DNS 검색을 수행하기 위한 기능을 제공한다. name과 type을 지정해야 한다．
다음 소스 코드는 XMPP 채팅에서 클라이언트 서버를 검색하기 위한 예제 코드이다．

 void MyObject: :lookupServers ()
     {
         II Create a DNS lookup.
         dns = new QDnsLookup(this) ;
         connect (dns, SIGNAL (finished() ),
                    this,   SLOT (handleServers () ));


         // Find the 耶PP servers for 이mail.com
         dns->setType (QDnsLookup: :SRV) ;
         dns->setNanie ( " U'xmpp中client. tcp. gmail.com") ;
         dns->lookup() ;
 }


예제의 소스 코드에서 보는 것과 같이 DNS 검색을 완료하면 finished( ) 시그널 이벤트가 발생하며 연결
된 handleServers( ) 슬롯함수가 호출된다. 이 함수에서는 검색된 서버의 DNS 결과를 참조할 수 있다．
그리고 DNS 검색 도중 발생한 에러를 참조할 수 있다．

 void MyObject: :handleServers ()
 {
         // Check the lookup succeeded.
         if   (dns->error () != QDnsLookup: :NoError)    {
               qWarning( "DNS lookup failed ' ) ;
               山ls->dele七eLa七er ( ) ;
               re七urn;
         }


         II   Handle the results.
         foreach (const QDnsServiceRecord &record, dns->serviceRecords () ) {


         }
         dns->deleteLater () ;
 }


QDnsLookup 클래스는 에러가 발생하면 다음과 같은 에러 처리를 위한 Enum 타입을 제공한다．




352 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 354 =====
Constant                                 Value   Descnption
QDnsLookup::NoError                              DNS 검색 중 에러가 발생하지 않음．
QDnsLookup::ResolverError                1       시스템의 DNS Res이ver으1 초기화 에러
QDnsLookup:：야冶rationCance陀dError         2       검색 도중 abort( ) 함수가 사용으로 중지
QDnsLookup::lnvalidRequestError          3       유효하지 않은 DNS
QDnsLookup::InvaIidRepIyError            4       검색한 서버의 리턴 값이 유효하지 않는 에러
QDnsLookup::ServerFailureError                   DNS 요청 검색 서버의 처리 도중에 내부 실패가 발생
QDnsLookup::ServerRetusedError           6       보안과 정책에 의하1 요청이 실패된 경우
QDnsLookup::NotFoundError                7       요청한 도메인 네임이 존재하지 않는 경우



0QDnsLo아（up 클래스의 DNS 레코드 타입 지정
DNS는 하나의 II) 어드레스와 Mapping 할 수 있는 레코드 타입을 존재한다. 예를 들어 qt-dev. corn 도
메인 주소 서버의 하위 서버로 존재하는 Mail 서버가 존재할 수 있다. 이러한 방식으로 하나의 도메인은
여러 개의 도메인 레코드 타입을 설정할 수 있다. QDnsLookup 클래스는 DNS를 검색하는 레코드 타입
을 지정할 수 있는 기능을 제공한다．

Const카lt               Va山e       Descri口hon
QDnsLookup::A               l     도메인 주소를 IF그 어드레스에 연결하기 위한 레코드이다. 예를 들어 ]0.11.12.13의 1P
                                  어드레스를 야-dev.com에 연결하:
                                                      71 위한 레코드를 설정할 수 있다．
QDnsLookup::AAAA         28       lPv6를 도메인과 연결하기 위한 레코드 타입이다．
QDnsLookup::ANY         255       ANY 레코드
QDnsLookup::CNAME           5     CNAME 레코드는 별칭이라 하며 다른 정규 도메인 이름과 연결하기 위해1 사용할 수
                                  있다. 예를 들어 帥as.q卜dev.com은 q卜dev.com과 연결할 수 있다．
QDnsLookup::MX           15       MX 레코드는 Mail Exchange라 하며 메일을 도메인의 메일 주소 서버에 전달하기
                                  위한 목적의 레코드 타입이다．
QDrisLookup::NS                   네임 서버（Name Server) 레코드0뼈 도메인 주소 정보를 어떤 서버가 전달할지 결정
                                  한다. NS 레코드는 도메인 이름을 식별하기 위한 서버를 지정하는 레코드이다．
QDnsLookup::PTR          12       PTR 레코드（Pc기nTer Record）는 DNS의 역방향 조회를 실행하기 위한 레코드 타입
                                  이다．
QDnsLookup::SRV          33       SRV는 서비스 DNS의 호스트와 특정 포트 번호가 정의된 서비스 위치를 지정하:11 위
                                  한 레코드 타입이다. 예를 들어 SRV 타입은 부하를 분산시키고 백업을 위한 목적을
                                  위하1 사용한다．
QDnsLookup::TXT          16       TXT 레코드는 텍스트 레코드라고도 하며 임의의 텍스트를 포함할 수 있다. TXT 레코
                                  드는 텍스트를 포함시킬 수 있지만 기계가 읽을 수 있는 텍스트를 정의할 목적으로도
                                  사용되며 도메인의 소유권을 확인하기 위하1 사용되곤 한다．




QDnsLookup 클래스는 DNS의 레코드 타입을 설정할 수 있는 기능을 지원한다. 예를 들어 QDns
Lookun:A와 같은 enurn 타입을 제공한다．




                                                                              ] 네트워크 353


===== PAGE 355 =====
     void DnsManager: :execute ()
     {
           QStringList args = QCoreApplication: : instance( )->arguments () ;
           args .takeFirst () ;
           dns->setType (QDnsLookup: :A) ;


           if   (args. size ( ) > 1 && args. first () == "- t ") {
                 args.takeFirst () ;
                const QString type = args.takeFirst () .toLower () ;
                if (type == "a")
                    dns->setType(QflnsLookup: :A) ;
                else if (type == "aaaa")
                        dns->setType (QDnsLookup: :AAAA) ;




I DNS 프로토콜을 이용한 예제 어플리케이션
DNS 프로토콜은 도메인 정보의 검색과 응답을 위한 프로토콜이다. DNS 프로토콜은 OSI 7 Layer에서
7계층인 Application 계층에 속해 있는 프로토콜이다. DNS 프로토콜은 네트워크를 경유하여 DNS 질
의山NS query）와 응답（DNS response）을 수행하기 위한 서버 클라이언트 모델 개념의 어플리케이션
계층 프로토콜이다．


         A口p比ation            내P           DNS        SMTP     RPC   F丁P

         Presentation          ILS         SSL

           Session

          가ans口아t                    TcP                     UDP


                                                 'P

          Datalink

          Physical

（그림） 0읽 7 Layer 앉ack



이번 예제에서는 QDnsLookup 클래스를 사용해 도메인 네임을 검색하는 예제를 살펴보자．

 class DnsManager : public QObject
 {
          Q OBJECT

publ如：
          DnsManager () ;

public slots:
                                                                                0

354 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 356 =====
     void execute () ;
     void showResults () ;


private:
     QDnsLookup *dns;

L1
예제의 소스 코드에서 execute( ) 함수는 QTimer 인스턴스에서 호출할 슬롯함수가 있다. QTimer가 수
행되면 execute 함수가 수행된다. showResults( ) 함수는 DNS 서버로부터 요청이 완료되면 응답을 받
으면 finished( ) 시그널 이벤트 함수가 호출한다. 이 시그널 이벤트는 showResults( ) 슬롯함수와 연결
되어 있다．

이번 예제 어플리케이션은 GUI가 존재하지 않는다. 커맨드 명령에 창 또는 터미널에서 도메인 타입과 도
메인 주소를 인자로 전달받는다．

dnslookup.exe -t ns google.com



첫 번째 인자는 검색할 DNS 타입을 설정한다. 그리고 두 번째 인자는 검색하고자 하는 레코드 타입을 명
시한다. 마지막 세 번째 인자는 도메인 주소를 입력한다．

in七 main(in七 argc, char 士argv[ ] )
{
     QCoreApplication app (argc, argv) ;


     DnsManager manager;
     QTimer: :singleShot (O, &manager, SLOT (execute () ));




QTimer 클래스는 정해진 시간의 주기어］ 따라 계속 반복한다. singleShot( ) 멤버함수는 한번만 실행되
도록 실행할 수 있는 기능을 제공한다. singleShot( ) 함수에서 두 번째1 인자는 구현한 DnsManager 클
래스의 인스턴스를 지정하고, 세 번째 인자에서는 DnsManager 클래스의 슬롯함수를 지정한다．

in七 main(iri七 argc, char 士argv[ ] )
{
     QCoreApplication app(argc, argv) ;


     DnsNanager manager;
     QTimer: : singleShot (O, &manager, SLOT (execute () ));


     return app. exec () ;
}




                                                               1 네트워크 355


===== PAGE 357 =====
DnsManager 클래스의 생성자에서는 QDnsLookup 클래스의 인스턴스를 초기화하고 도메인 서버로부터
요청을 완료하면 finished( ) 시그널 이벤트를 발생한다. finished( ) 시그널 이벤트는 showResults( ) 함
수와 연결되어 finished( ) 시그널 이벤트가 발생하면 showResults( ) 슬롯함수가 호출된다．

void DnsManager: :execute()
{
    QStringList args = QCoreApplication: :iristance () ->arguments ( );
    args .takeFirst () ;



args는 Command 명령에 창 또는 터미널로부터 사용자가 입력한 인자（Arguments）를 저장한다. 그리
고 instance( ) 함수는 QCoreApplication 인스턴스의 포인터를 리턴하며 arguments( ) 함수는 사용
자가 입력한 인자를 리턴한다．

    II lookup type
    dns->setType (QDnsLookup: :A) ;
    if   (args. size () > 1 && args. first () == "- t ") {
         args . takeFirst U;
         const QString type = args.takeFirst ( ).toLowerU;
         if   (type == "a")
              dns->setType (QDnsLookup: :A) ;
         else if   (type == "aaaa")
              dns->setType(QDnsLookup: :AMA) ;
         else if  (type == "any ")
              dns->setType (QDnsLookup: :ANY) ;
         else if   (ty冶 == "cname")
              dns->setType (QDnsLookup: :CNM4E) ;


         else {
              printf ( "Bad record type: %s\n", qPrintable (type) );
              QCoreApplication: :instance (卜>quit ( );
              return;
          }
     }


args는 사용자가 입력한 인자를 QStringList 타입으로 저장되어 있다. size( ) 함수를 사용해 저장한 인
자의 개수를 리턴한다. first( ) 함수는 args 인자어］ 저장된 첫 번째 인자를 리턴한다. QStringList 클래
스가 제공하는 takeFirst( ) 함수는 args 인스턴스에 저장된 첫 번째 아이템을 제거한다．

첫 번째 인자를 제거하면 사용자가 입력한 두 번째円l 리소스 레코드 타입이 첫 번째 인자가 된다. 리소스
타입에 따라 dns 인스턴스의 도메인 검색 레코드 타입을 설정한다．




356 CHAPTER 12. 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 358 =====
   if    (args.isEmpty () ) {
          usage () ;
          QCoreAppli（그a七ion: : instance (卜＞quj土 ( ) ;
          return;
    }
    dns->setName (args.takeFirst () );
    dns->1ookup ( );




dns 인스턴스의 검색하고자 하는 도메인 네임을 setName( ) 함수를 사용해 설정하고 lookup( ) 함수를
실행해 지정한 DNS 주소를 DNS 서버로부터 요청한다. DNS 서버로부터 검색하고자 하는 DNS 검색 결
과 요청을 받으면 생성자에서 설정한 finished( ) 시그널 이벤트가 발생하고 연결된 showResu比s( ) 슬
롯함수를 호출한다．

void DnsManager: :showResults ()


    if   (dns->error ( ) !== QDnsLookup: :NoError)
          printf ( "Error: 돔i 作引＼n'' , dns小＞err（그r ( ) r
                                         qPrintable (dns->errorString() ) );


    II CNM1E records
    foreach ( const QDnsDomainNameRecord & record,
                                                  dns->canonicalNameRecords () )
          printf ( " %s\ t%i\ tIN\ tCNANE\ t%s\n", qPrintable(record.name () ),
                                                  record.timeToLive() ,
                                                  qPrintable (record.value() ));


    /1 MX records
    foreach (const QDnsMailExchangeRecord &record,
                                                  dns->mailExchangeRecords () )
          printf ( "%s\ t%i\ tIN\ tMX\ t%u %s\n", qPrintable (record.name () ),
                                                  record.timeToLive () ,
                                                  record.preference () ,
                                                  qPrintable (record.exchange() ));




검색 결과가 에러가 발생하면 QDi始Lookup 클래스의 error( ) 함수를 통해 에러가 발생했는지 확인할
수 있다. QDnsLookup에서 제공하는 enum 타입과 비교해 에러가 발생한다면 errorString( ) 함수를
통해 에러에 태한 상세 내용이 저장된 내용을 문자열로 리턴한다．

foreach 구문을 사용한 이유는 검색한 타입의 리소스 레코드는 하나 이상이 될 수 있다. 따라서 여러 개
의 리소스 레코드 타입을 참조하기 위해서 凡reach 구문을 사용하면 용이하다. recode 인스턴스는
QDnsDomainNameRecord 클래스의 인스턴스이다. DNS 서버로부터 응답 받은 레코드 정보를 이 클
래스의 인스턴스로 결과를 리턴한다．




                                                                                      ] 네트워크 357


===== PAGE 359 =====
 텍          귄리 쟈 Qt 5 D n f，그rt冶5k＋그D   드＼/0 2010)


 DrIKt5甘Net小川）rk卄dne1ooJnp- b,ti tdkIcIJng>rtnr. 1ooInL1p -eXe    t nS google. eon
   S 4. Ffoog1e.eom 86368 IN          A         216. 239. 38. 1日
 nfl .goo므le .con         IN                    216. 239. 32. 1日
  ns2.google. con 86368   IN                    216 .2 39 . 34. 1日
   s3. qooqie , ,on 86368 IN          AAA       216. 239. 36. 1目
                                /
   angle . con      86368 IN         NI         nsl. google. con
 늬 oogle .cOi까      86368 IN         NI         net .google .com
 니 (J1玎jie .com     86368 IN         NI         ns2 .google .com
 4oogle .Com        86368 IN         NI         ns3 - go og le . con

 1:明QtSWNetHo-In卄dne1ooknp-boi1dWdebag>dne1ookup.exe -t mx google. com
  1t2. .aepmx.1. google. con 269  IN      A        71. 126. 14日.27
  1t4. aepnx.1. goog1e.c기4 269    IN      A        173. 194. 75. 27
  1t3 느aepmx.1. google. coe 269   IN      A        173. 194. 74. 27
  epnx. 1. gooqle. com       269  IN      A        173. 194. 79. 27
  王tl. xepmx. 1. google. com 269  IN      A        74. 125. 142. 27
  oogle. con        269      IN   11%     1日 eepnx. 1. google. com

 :::：亡：
 느ooqle.com
                  ::269
                             를듬： :=
                             IN
                                  Mt
                                  Mt
                                  MX
                                          20 e1tl 1oepnx. 1. goog1e日con
                                          3日 alt2. anpnx. 1. google. com
                                          40 alt3. eopmx.1. google. con
  oogle. com        269      IN   MX      5日 alt4. oepnx. 1. google. con

     1 :wgts l汁1e t, ,o .-k旴tns looknp- hnild好debng)_




（그림） 도메인 네임의 검색 어플리케이션 예제 실행 화면




            t1E11 HTTP(Hy口erText Transfer Protoc이） 프루토콜
Qt에서 제공하는 녜트워크 모듈은 HTTP 프로토콜 기반의 어플리케이션을 구현할 수 있는 API를 제공
한다. Qt는 HTTP 프로토콜뿐만 아니라 OSI 7 Layer에서 7계층인 Application Layer 계층에 위치한
FTP, DNS, SNMP 등 다양한 프로토콜 기반의 어플리케이션을 구현할 수 있는 기능을 제공한다．

   Ap口比ation Layer             NNTP SIP SSI DNS FTP I-hIP NFS NIP SMPP SMTP DHCP SNMP...

Presentation Layer             MIME XDR TLS SSL...

          Session Layer        Named미pe N비미OS SAP SIP ...

          Trans口ort L톄／er      TCP UDP SCTP DCCP...

          Network Layer        'P 吃MP 作＞sec IGMP IPX A口이eTa水 ...

          Datalink Layer       A日P CS니PS니P 타hernet 日ame re冶y ITU나 (3.hn DLL L2TP PPP PPTP ...

                               RS-232 RS-449 V.35 V.34 1.430 1.431 Ti El POTS SONET/SDH OTN
          Phy덟C례 Layer
                               DSL 802.hla/b/g/n PHY ITU寸 13.hn PHY 타hemet USB 태U아的th

（그림） 0텨 7계층



Qt 4. x 버전은 HTTP와 FTP 프로토콜을 지원하기 위해 QHttp와 QFtp 클래스를 제공하였다. Qt 5.0
버전부터는 QHttp와 QFtp 클래스는 삭제되었다. QNetworkAccessManager, QNetworkRequest,
QNetworkReply 클래스를 통해1HTTP와 FTP 프로토콜 기반의 어플리케이션을 구현할 수 있는 기능을
제공한다. 이 클래스는 HTTP와 FTP 프로토콜 이외에 I끄gh Level(OSI 7계층에서 상위 계층） 네트워크
어플리케이션을 구현할 수 있다．

네트워크를 경유하여 Request를 요청할 경우 QNetworkRequest 클래스를 제공한다. 또한 헤더 정보
와 Encryption된 헤더 정보를 포함해 요청할 수 있다. QNetworkRequest 클래스는 HTTP, FTP 그리
고 로컬 파일을 URL을 통해 업로드 및 다운로드 할 수 있는 기능을 지원한다．


358            CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 360 =====
HTTP와 FTP 프로토콜을 이용해 네트워크상의 수행 과정을 관리하기 위한 목적으로 Qt 네트워크 모듈
은 QNetworkAccessManager 클래스를 제공한다. 이 클래스는 네트워크 요청과 응답을 처리할 수 있
는 기능을 제공한다. 클라이언트가 새로운 요청을 생성할 때 요청어］ 대한 진행과정（Progress）을 리포트
할 수 있는 기능과 요청에 따른 시그널 이벤트를 사용할 수 있는 기능을 제어하고 관리한다. 그리고
QNetworkAccessManager 클래스는 클라이언트상에 Cookie를 저장하기 인증 요청을 사용하거나 프
락시를 설정할 수 있다．

QNetworkRe히y 클래스는 네트워크상에서 응답을 처리하기 위해 제공하는 클래스이다. 요청이 도착할
때 QNetworkAccessManager 클래스에 의해 생성된다. QNetworkRe히y 클래스는 각각의 요청에 대
한 응답을 모니터링이 가능한 시그널을 제공한다. QNetworkRe히y 클래스는 印ODevice 클래스의 하
위 클래스이며 동기화와 비동기 방식 모두 지원한다. 이번 장에서 HTTP와 FTP 같은 상위 계층 네트워
크 응용 어플리케이션을 개발할 수 있는 API어］ 대해 살펴보도록 하자.


1QNetw아kAccessManager, QNetworkRequest 그리고 QNetw아kRepm 클래스
QNetworkAccessManager 클래스는 네트워크 요청과 응답을 관리하기 위해 제공되는 클래스이다. 네트
워크상에서 요청 및 응답하기 위한 설정을 관리하며 프락시와 캐시를 사용할 수 있으며 네트워크 요청과
응답과정에서 발생한 시그널을 처리할 수 있는 기능을 제공한다. 아래 예제의 소스 코드는 QNetwork
Acces帥血nager 클래스를 사용하였다．

QNetworkAccessManager *manager = new QNetworkAccessManager (this) ;
connect (manager, SIGNAL(finished(QNetworkReply* )),
         this, SLOT (replyFinished(QNetworkRep1y* )));


manager->get (QNetworkReq口est (QUr1( "http: //qt- dev.com") ));



예제의 소스 코드는 QNetworkAccessManager를 비동기 방식으로 사용한 예제이다. 다운로드가 완료되면
QNetworkReply 오브젝트를 가져온다. QNetworkAccessManager 클래스는 받은 요청을 큐（Queue）를
사용해 저장한다. 따라서 프로토콜상의 요청（Request）은 병렬 형태와 같이 차례대로 수행한다．

QNetworkRequest req口est;


request. seturl (QiJr1( "http: //qt- dev.com") );
request. setRawHeader ( "User-Agent ", "MyOwnBrowser 1.0 ") ;


QNetworkReply *reply = manager->get (request) ;

connect (reply, SIGNAL (readyRead() ), this, SLOT(slotReadyRead() ));

connect (reply, SIGNAL (error (QNetworkReply: :NetworkError) ),
         this, SLOT (slotError (QNetworkReply: :NetworkError) ));

connect (reply, SIGNAL(sslErrors (QList<QSslError> )),
         this, SLOT(slotSslErrors (QList<QSslError> )));



                                                                        L네트워크 359


===== PAGE 361 =====
0QHttpPart 클래스와 QHttpM네tiPart 클래스
HTTP 프로토콜은 상호간 통신을 위해1TCP 세션 연결을 시작한다. 일단 HTTP를 요청하는 클라이언트
는 HTTP Request 혜더와 Body어］ URL과 요청 데이터를 포함하여 전달한다. 이때 응답하는 서버（예를
들어 웹 서버） 클라이언트 요청의 유효성을 검증한 후 이상이 없다면 HTTP Response Header 및 Res-
ponse Body에 문서를 만들어 클라이언트에게 전달하게 된다．

클라이언트가 HTTP 프로토콜을 이용해 Request를 요청하기 위한 Message를 전달한다. HTTP 프로
토콜 八ilessage는 요청과 응답 메시지로 구분된다. 또한 버전에 따라 지원 가능한 Method가 존재한다．
HTTP/1. 0 이하 버전일 때 GET 요청만 가능하며 응답 또한 text 타입으로 제한된다．

 Vers山ri           Descri口tion
 HTTP/0.9          "GET"
 HTTP/1.0          "GET", "POST", "HEAD"
 HTTP/1.1          "GET", "POST", "HEAD", "OPTIONS", "PUT", "DELETE", "TRACE", "CONNECT"



HTTP 메시지는 크게 라인, 헤더 , 바디 영역으로 구분되며, 또 여기서 헤더와 바디 영역 사이는 공백으로
구분된다. 또한 Body 영역을 제외한 나머지 영역（요청 , 헤더）의 각 라인은 연속된 CR/LF(\r\n) 문자로
구분된다．

                           요청 人I HTTP 메시지 구성               웅답 시 HTTP 메시지 구성
                           /                           \   /                        \
      Start Une                      Request Une                     Status Une
                           \\                          I


                                일반에더 (Gener테 Header)           일반헤더 (General Header)
       Header                   요청에더 (Reque鐵 H明d帥              응답에더 （日es口onse Header)
                                 객체에더 (Entry Header)            객체에더 (Entry Header)

     A 벼ank line
                      I
                           (         빈공벡라인         : :               빈공백라인          )
                                요청에 필요한 데이터 내용                 요청 데이터의 용답 메시지외
        Body                          기슬                            HTML문서


（그림） Hill그 Request/Response Message 구성


일반 혜더는 요청과 응답 모두 사용할 수 있는 헤더이며 요청（Request), 응답（Response) 헤더는 요청과
응답 시 사용되는 헤더이다. 객체（Ent仇y) 헤더는 파일의 인코딩 방식, 최종 수정 일자와 같은 외형적인
정보를 나타내기 위해 쓰이는 헤더이다．

Qt에서 제공하는 QHttpPart 클래스는 HTTP의 Multipart MIME message 내에 사용할 수 있는 Body
를 지정할 수 있는 기능을 제공한다. QHttpPart 클래스는 헤더 Block과 Data Block으로 구성된다．




360 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 362 =====
1Con七en七-Type: 七e）代／plain
rmm
 Conten七-DisE均sition: 如rm-data; name= '노e就n


      here goes the body



QHttpPart 클래스는 헤더를 설정하기 위해 setHeader( ) 멤버함수, setRawHeader( ) 멤버함수를 제
공한다. 즉 QNetworkRequest 클래스의 set}-Ieader(）와 setRawHeader( ) 함수와 같이 동작한다. 여］
를 들어 setBody( ) 함수를 사용해 일부를 읽어 들이거나 이미지와 같은 데이터 영역을 읽기 위해
 setBodyDevice( ) 함수를 사용한다．

문자열 메소드는 떼이터를 즉시 복사하지 않고 메모리에 저장할 뿐만 아니라 파일로부터 직접 읽어 들인
다. QHttpPart 클래스를 사용해 Body를 구성하는 방법은 다음과 같다．

      QHttpPart textPart;


      textPart. setHeader ( QNetworkRequest: : ContentTypeHeader,
                                              QVariant ( "text/ plain") );
      textPart. setHeader (QNetworkRequest: :ContentDispositionHeader,
                                                QVariant ( "form-data; name=\" text\ " ") );


      textPart.setBody ( "here goes the body ") ;



 QHttp 클래스는 파일로부터 읽어와 구성하는 방법은 다음과 같이 사용한다．

      QHttpPart imagePart;


      imagePart. setHeader (QNetworkRequest: : ContentTypeHeader,
                                                QVariant ( "image/ jpeg") );
      imagePart. setHeader ( QNetworkRequest: : ContentDispositionHeader,
                                              QVariant ( "form-data; name=\" image\ " ") );
      imagePart. setRawHeader ( "Content-ID", "my@content.id ") ;

      QFile *file   = new QFi1e ( "image. jpg") ;
      file- >open (Q工oDevice: :ReadOnly) ;
      imagePart. setBodyDevice (file) ;



  QHttpPart 클래스는 HTTP의 메시지의 특정 부분을 지정하거나 저장할 수 있다. 또한 Qt는 여러 개로
 나누어진 메시지를 하나로 나타낼 수 있는 QHttpMultiPart 클래스를 제공한다. 즉 이 클래스는 HTTP
상에서 전송할 MIME 타입의 메시지를 통합할 수 있는 기능을 제공한다．




                                                                                           ] 네트워크 361


===== PAGE 363 =====
  QHttpMultiPart *multiPart = new
                                                           QHttpMultiPart (QHttpMultiPart: : Fori山ataType) ;

  QH七七pPar七 te）比Part;
  textPart. setHeader (QNetworkRequest: : ContentDispositionHeader,
                                                           QVariant ( "form-data; name=\ " text\ " ") );
  textPart. setBody ( "my text ") ;


 QHttpPart imagePart;
 imagePart. setHeader ( QNetworkRequest: : CoritentTypeHeader,
                                          QVariant ( "image/ jpeg") );
 imagePart. setHeader (QNetwork之equest: : ContentDispositionHeader,
                                                           QVariant ( "form-data; nanie=\" ixnage\ '1 ") );

 QFile *file   = new QFile ( "image. jpg") ;
 file- >open (Q工ODevice: : ReadOnly) ;
 imagePart. setBodyDevice (file) ;
 file- >set下aren七 (mu그上iPart) ;
 multiPart->append ( textPart) ;
 multiPart->append ( imagePart) ;


 Qurl url ( "http: //my. server.tld ") ;
 QNetworkRequest request (url) ;


 QNetworkAccessManager manager;
 QNetworkReply *reply = manager.post (request, multiPart) ;
 multiPart->setParent (reply) ;




S HTTP 클라이언트 예제
이번 예제 HTTP 클라이언트 어플리케이션은 웹 서버어］ 접속해 해당 URL을 파일로 저장하는 예제이다．
이 예제에서는 QN毗workAccessManager, QNetworkRequest, QN毗workRe히y 클래스를 사용해
웹 서버에 위치한 파일을 다운로드 하는 방법에 대해 살펴보도록 하자．

二刃 HT갸）

  UAL: http://qt-dev. com/

  Please enter the URL of a file y ou want to download.

                                               1Download      Quit


（그림） HTTP 예제 실행 화면



그림에서 보는 것과 같이 다운로드 할 파일의 URL을 입력하고 [Download] 버튼을 클릭하면 웹 서버상
어］ 존재하는 URL을 경유해 파일로 저장한다．




362 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 364 =====
class Httpwindow : public QDialog
{
    Q OBJECT


public:
    HttpWindow ( QWidget *parent = 0) ;
    void startRequest (QUrl url) ;


private slots:
    void downloadFile () ;
    void cancelDownload() ;
    void httpFinished() ;
    void httpReadyRead() ;
    void updateDataReadProgress (qirit64 bytesRead, qint64 totalBytes) ;
    void enableDownloadButton() ;




예제의 소스 코드는 구현할 HttmWindow 클래스의 헤더 소스 파일이다. 슬롯함수로 명시한 download
File( ) 슬롯함수는 GUI 상에서 [Download] 버튼을 클릭하면 호출되는 슬롯함수이다. 이 슬롯함수에서는
저장할 파일을 지정하고 다운로드 준비가 완료되면 startRequest( ) 함수를 호출한다. 이 함수는 URL을
인자로 전달 받으며 QNetworkRequest 클래스의 인스턴스가 설정된 URL을 인자로 전달한다．

void HttpWindow: :startRequest (QUrl url)
{
    reply = qnani. get (QNetworkRequest (url) );
    connect (reply, SIGN公L(finished() ), this,      SLOT (httpFinished() ));
    connect (reply, SIGNAL (readyRead() ), this,     SLoT (httpReadyRead() ))


    connect (reply, SIGNAL (downloadProgress (qint64,qint64) ),
               this,   SLOT (updateoataReadProgress (qint64 ,qint64) ));
}


QNetworkAccess八ilanager 클래스의 qnam 인스턴스는 QN毗workRequest 클래스의 생성자를 인자
로 사용하여 요청하기 위해 QNetworkAccessManager 클래스의 get( ) 멤버함수를 사용한다．

reply는 QNetworkReply 클래스의 인스턴스이다. 웹 서버로부터 응답이 완료되면 finished( ) 시그널
이벤트가 발생하고 이 시그널과 연결된 httpFinished( ) 슬롯함수가 호출된다. 그리고 웹 서버로부터 데
이터를 읽을 때마다 readyRead( ) 시그널 이벤트가 발생하고 이 시그널과 연결된 httpReadyRead()
슬롯함수가 호출된다．

마지막 시그널은 다운로드 되는 과정을 다이얼로그박스 상에 진행사항을 Progress Bar 형태로 나타내
기 위해 downloadProgress( ) 시그널 이벤트를 제공한다. 이 시그널 이벤트가 발생하면 연결된 up
dateDataReadProgress( ) 슬롯함수를 호출하게 된다．




                                                                                ] 네트워크 363


===== PAGE 365 =====
 void HttpWindow: :httpReadyRead()
 {
         if   (file)
               file- >write (reply->readAll( ));
 }


httpReadyRead( ) 슬롯함수가 호출되면 HTTP 웹 서버로부터 읽어온 데이터를 파일어］ 저장한다．
reply는 QNetworkRe히y 클래스의 인스턴스이다．

 void HttpWindow: :httpFinished()
 {
      if      (httpRequestAborted) {
               if (file) {
                       file- >close() ;
                       file- >remove() ;
                   delete file;
                       file   = 0;
               }
               reply->deleteLater () ;
               progressDialog->hide () ;
               return;
      }

     progressDialog->hide () ;
     file- >flush() ;
     file- >close () ;



httpFinished( ) 슬롯함수는 다운로드가 완료되면 호출된다. 이 슬롯함수에서 만약 파일 다운로드가 실
패하면 파일을 닫고 현재 파일을 삭제한다. 그리고 생성한 QFile 클래스의 file 인스턴스를 메모리로부터
해제한다. 만약 정상적으로 파일을 다운로드 받으면 진행다이얼로그를 숨기고 flush( ) 함수를 사용해 버
퍼에 남아있는 파일 내용을 실제 파일어］ 적용한다．

     QVariant redirectionTarget =
                  reply->attribute (QNetworkRequest: : RedirectionTargetAttribute) ;
     if       (reply->error () ) {
               file- >remove() ;
              QMessageBox: :information(this,      tr ( "HTTP") ,
                                           tr ( "Download failed: %l. ")
                                       .arg(reply->errorString() ));
              downloadButton->setEnabled (true) ;
     }


만약 다운로드 중어］ 에러가 발생하면 QFile 클래스의 remove( ) 멤버함수를 사용해 파일을 삭제하고 발
생한 에러를 帥/IessageBox에 표시한다．



364 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 366 =====
    else if      ( !redirectionTarget.isNull () ) {
                QUrl newUrl = url .resolved(redirectionTarget.toUrl (fl;
                if   (QMessageBox: :question(this,           tr ( "HTTP") ,
                              tr ( "Redirect to %1 ?" ) .arg(newUrl. toString(fl,
                         QMessageBox: :Yes 1 QMessageBox: :No) == QMessageBox: : Yes)   {
                      unl = newlJrl;
                      reply->deleteLater () ;
                      file- >open(QlODevice: :WriteOnly) ;
                       file- >resize (O) ;
                      startRequest (url) ;
                      re七urn;
                 }
      }


만약 다운로드 받는 파일이 끝이 아니면 파일을 다시 쓰기 모드로 지정하고 startRequest( ) 함수를 호
출한다．


S ON아workAccessManager 클래스를 이용한 파일 다운로드 예저1
이번 예제 어플리케이션은 GI끄가 포함되지 않은 예제이다. （兀mmand 창 또는 터미널 상에서 입력한
URL을 인자로 읽어와 파일을 로컬 디스크어］ 파일로 저장한다．

download.exe http: //qt- dev.com/index.htrnl



다운로드 받을 웹 서버의 URL과 파일을 첫 번째 인자로 명시하면 다음 그림에서 보는 것과 같이 웹 서버
어］ 접속해 파일을 다운로드 받는다．

圃 관리자：Qt 5요a 向rDesktop (！너5VC i二


 ：卜冷比帥妃too바泄Ihoild瞰Iebu中doon1oad. exe http: //qt- doo con/index.htp,1
 oon1oad of http: //qt- doo.con/index.htnl succeeded <sa ed to indsx.htnl>

 ) : 什3t5WHetuo. hWdbui1dWdebug)dir
  1) 드라이 브의 불튬에는 이 픔이 없습니다．
   롤튬 일 련 번호： 6fl16-?DA2

 B：뽀Qt5卄NetoorkRdbaild竹de｝川9 디렉터 리

小13田3硅3      오후 日9: 43   <DIR>
．日13-日3-13   오후 99:13    <DIR>
 目13 日3-13   오후 日9:37          62.464 doonload.exe
!5t3 日3-13   오후 99:43             586 index.I,tol
              2개1파일               62.9？日 바이 트
              2)11 디 렉터 리 89,665.839. 912 바이트 남 ;




（그림） 파일 다운로드 예제 실행 화면




                                                                                            ] 네트워크 365


===== PAGE 367 =====
  class DownloadNanager: public QObject
      {
          Q OBJECT
          QNetworkAccessManager manager;
          QList<QNetworkReply 出> currentDownloads;


 public:
          DownloadNanager () ;
          void doDownload(const Qurl &url) ;
          QString saveFileName (const Qurl &url) ;
          bool saveToDisk (const QString &filename, QlODevice *data) ;


 public slots:
          void execute () ;
          void downloadFinished(QNetworkReply *reply) ;
          void sslErrors (const QList<QSslError> &errors) ;
 };
예제의 소스 코드는 구현한 Downloa（江4anager 클래스의 헤더 파일 소스 코드이다. execute( ) 슬롯함
수는 QTimer 인스턴스에 의해1 최초 한번만 호출한다. QTimer 클래스는 인자로 지정한 시간만큼 주기
적 인 반복을 하지만 QTimer 클래스의 singleShot( ) 멤버함수를 사용하면 최초 한번만 호출한다．

 in七 main(int argc, char 出出arg미
 {
          QCoreApplication app(argc, arg기;


          Do寸nloadManager manager;
          QTimer: : singleShot (O, &manager, SLOT (execute () ));


          app.exec () ;
 }



QTimer 클래스의 singleShot( ）는 Static 멤버함수이다. 따라서 인스턴스를 사용하지 않아도 사용할
수 있다. 첫 번째 인자는 구현한 DownloadManager 클래스 execute( ) 함수가 실행될 Interval 타임
을 지정한다．

여기서는 0을 인자로 지정했기 때문에 singleShot( ) 함수를 실행하면 execute( ) 함수를 바로 호출한
다. 두 번째 인자는 DownloadManager 클래스의 인스턴스를 지정하고 세 번째 인자는 호출할 슬롯함
수를 지정한다．




366 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 368 =====
!void               oownloa   曲anager:         :execute   ()

            QStringList args = QCoreApplication: : instance ( )->arguments () ;
            args.takeFirst ( );
            if        (args.isEmpty () )
            {
                       printf ( "Qt Download example - downloads all URLs in parallel\ n"
                                         "Usage: download urli     [ur12. . . urlN] \n"
                                          "differentiate. \n") ;
                       OCoreApplication: :instance ( )->quit () ;
                       re七urn;
                }

            foreach(QString arg, args)
            {
                       QUrl url = QUrl: : froinEncoded(arg.toLocal8Bit () );
                       doDownload(url) ;
                }
        }


    execute( ) 슬롯함수는 Command 명령어 창과 터미널에서 사용자가 어플리케이션을 실행할 때 인자를
    입력했는지 확인한다. takeFirst( ) 함수는 args어］ 저장된 인자 중 처음에 저장된 아이템을 제거한다．
    args어］ 저장된 첫 번째 인자는 실행한 어플리케이션의 파일명이다. 따라서 takeFirst( ) 함수로 처음 아
  이템을 제거했을 때 다음 인자가 존재하지 않으면 에리를 리턴한다．

  如reach 구문에서 args어］ 저장된 인자를 QURL 클래스의 unl 인스턴스어］ 저장하고 doDownload( ) 함
  수를 수행한다．

        void DownloadManager: :doDownload(const QUrl &url)
        {
            QNetworkRequest request (url) ;
            QNetworkReply *reply = manager.get (request) ;


        #ifndef QT NO SSL
            connect (reply, SIGNAL(sslErrors (QList<QSslError> )),
                                                                     SLOT (sslErrors (QList<QSslError> )));
        幸endif


            currentDownloads .append(reply) ;
        }


        doDownload( ) 함수는 QNetworkRequest 클래스의 인스턴스에 전달받은 un을 첫 번째 인자로 설정
        해 다운로드 할 URL을 설정한다. manager는 QNetworkAccessManager 클래스의 인스턴스이다．
        get( ) 함수를 통해 다운로드 받는다．




                                                                                                              ] 네트워크 367


===== PAGE 369 =====
Downloa丑4anager: :DownloadNanager ()
{
    connect (&manager, SIGNAL (finished(QNetworkReply* )),
                  SLOT (downloadFinished(QNetworkReply* )));




DownloadManager 클래스의 생성자에서는 다운로드가 완료되면 finished( ) 시그널 이벤트가 발생하
며 연결된 downloadFinished( ) 슬롯함수가 호출된다. downloadFinished( ) 슬롯함수는 다운로드 도
중 실꽤하면 에러를 문자열로 리턴하고, 그렇지 않고 다운로드가 완료되면 다운로드를 위해 임시로 생성
한 파일을 실제 파일명으로 변경한다．

void DownloadManager: :downloadFiriished(QNetworkReply *reply)
{
    QUrl unl = reply->unl() ;
    if   (reply->error () ) {
          fprintf (stderr, "Download of %s failed:        %s\n",
                      url. toEncoded( ) .constData ( ),
                      qPrintable(reply->errorString() ));
    } else    {
         QString filename = saveFileName (url) ;
         if   (saveToDisk (filenaxne, reply) )
                  prin七f ( '너：)ownload of 통s succeeded 作aved 七（> 돔s) \n" r
                         url. toEncoded() .constData ( ), qPrintable (filename) );
    }

    currentDownloads . removeAll (reply) ;
    reply->deleteLater () ;


    if   (currentDownloads.isEmpty () )
          7/ all    downloads finished
         QCoreApplication: :instance ( )->和it ( );
}


downloadFinished( ) 슬롯함수는 다운로드가 완료되면 saveFile( ) 함수를 수행한다. 이 함수는 실제
파일어］ 저장한다. 그리고 버퍼어］ 저장된 currer此Downloads의 내용을 removeAll( ) 함수를 사용해 제
거한다．



武l.5Bearer Management
컴퓨터 시스템은 Ethernet과 같은 네트워크 디바이스 인터페이스를 내장하고 있다. Ethernet 이외에도
WiFi와 같은 무선 인터넷 인터페이스, Bluetooth, 2G, WCDMA, HSPA, M乃MAX 등 다양한 네트워크
디바이스를 지원한다. 이러한 수많은 네트워크 디바이스는 인터넷에 접속하기 위해 설정과 인터페이스의
시작과 종료를 위한 처리과정 그리고 특정 디바이스마다 인터넷 연결 세션을 관리하는 등을 지원하는 설
정과 인터페이스를 관리하는 다양한 종류의 API를 사용해야 한다．


368 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 370 =====
예를 들어 다양한 네트워크 디바이스 인터페이스를 내장하고 있는 시스템으로 스마트 핸드폰, 태블릿, 스
마트 TV 등이 있다. 이러한 다양한 네트워크 디바이스를 지원하는 시스템에서 인터넷 네트워크어］ 접속해
원하는 정보를 다운로드 받거나 데이터를 송수신하기 위한 Connectivity 어플리케이션을 구현하는 것은
매우 힘든 사항이다．

Qt는 이러한 다양한 네트워크 디바이스를 제어하고 연결 세션을 관리하기 위해 표준화된 API를 제공하
는 목적으로 Bearer Manageme玭를 제공한다. Bearer Manageme玭는 다양한 네트워크 디바이스 인
터페이스의 데이터 송수신을 위한 연결 세션을 시작과 중지하는 표준화된 클래스를 제공할 뿐만 아니라
다양한 네트워크 디바이스 인터페이스를 설정하기 위한 표준화된 클래스를 제공한다．

QNetworkCor寸培urationManager 클래스는 네트워크 디바이스의 연결 리스트를 관리하는 기능을 제
공하며 QNetworkConfiguration 클래스는 녜트워크 인터페이스를 사용해 연결을 시작하는뎨 사용한
다. QNetworkConfigurati아小/lanager 클래스로부터 얻어온 네트워크 연결 정보를 이 클래스의 파라
미터로 사용한다．

BearerTy口e                       Va山e
BearerUnknown                    Unknown type
BearerEthernet                   타hernet
BearerWLAN                       Wireless LAN
Bearer2G                         2G
BearerCDMA2000                   CDMA2000
BearerWCDMA                      WCDMA
BearerHSPA                       HSPA
BearerBluetooth                  텨uetooth
BearerWiMAX                      WIMAX



네트워크 연결 정보를 이용해 QNetworkSession을 사용하여 네트워크 세션을 시작할 수 있다. 이 클래1
스는 네트워크 세션을 만드는데 적합하며 QNetworkConfigurationManager 클래스가 제공하는
defaultConfiguration( ) 함수에 의해 연결 구성을 리턴한다. 어떤 플랫폼에서는 네트워크 동작을 수행
하기 전에 네트워크 세션을 요구하여 사용하기도 한다．

Interface management                        Session management
QNetworkSession::stop()                     QNetworkSess山n::open()
QNetworkSession::interface()                QNetworkSession::close()
QNetworkSession::state()                    QNetworkSes듸on긔sO口en( )
QNetworkSess山n::bytesWritten()              QNetworkSession::migrate()
QNetworkSession::bytesReceived()            oNetworkSession::ignoreO
QNetworkSession::activeTime()               QNetworkSession::accept()
QNetworkSession::stateChanged()             QNetworkSession::reject()
                                            QNetworkSess山n::opened()
                                            QNetworkSess幻n::closed()



                                                                         1 네트워크 369


===== PAGE 371 =====
（南百 서버／클라이언투 咐 채팅 예제
QTcpSocket 클래스는 TCP 기반 서버／클라이언트 어플리켸이션을 개발하는 데 표준 API를 사용하는
것보다 많은 부분이 간편화되어 있으며 짧은 소스 코드로 구현이 가능하다는 장점이 있다. 이번 장에서는
QTcpSocket 클래스를 사용해 서버／클라이언트 채팅 어플리케이션을 구현해 보는 방법에 대해 살펴보도
록 하자．


  . 채팅 서버 예제 어플리케이션
ChatServer 예제 어플리케이션은 클라이언트가 접속 혹은 클라이언트가 서버로 메시지를 전송하면
QTcpSocket 클래스를 이용해 서버에 연결되어 있는 클라이언트에게 데이터를 전송한다．

           새로운 i라이언트 접속                                           클라이언트71 보낸 메시지
ri그Cha：             鈿싸en            「 “「    [m
                                                 《4   口   '   1 '. C已三t노昨.         뇨向m)
1[ 珏뇨小                                                        !




                                                          1
                                                          二1
1i斛澍群，嚮UI



          Clients    ,         ::   ' 「，
                                       「" ' " ' " '


（그림） ChatSer尼r 예제 실행 화면



 그림에서 보는 것과 같이 [Server Start] 버튼을 클릭하면 서버가 시작되고 클라이언트가 접속하면 클라
이언트의 유저명과 관련한 로그를 출력한다. 그리고 클라이언트가 메시지를 전송하면 유저명과 메시지를
출력한다．

 서버 어플리케이션은 네트워크 관련 기능이 구현된 ChatServer와 GUI와 관련한 w奴get 클래스로 구
 현되어 있으며 ChatServer 클래스부터 살펴보도록 하자．

          class chatServer : public QTcpServer
          {
                    0 0BJECT

          public:
                    chatServer (QObject *parent=O) ;

          private slots:
              void readyRead() ;
              void disconnectedO;
              void sendUserList () ;                                                      O



370 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 372 =====
     signals:
         void clients signal(int users) ;
         void message signal (QString msg) ;


 protected:
        void incomingConnection(int     socke七fd) ;

 private:
        QSe七＜QTcpSocket；出＞ clien七S;
        QMap<QTcpSocket* ,QString> users;
 };


incomingConnection( ）는 QTcpServer 클래스의 재정의된 virtual 함수이며 새로운 클라이언트가 접
속했을 때 , 호출되는 함수이다．

 void chatServer: :incomingConnection(int        socketfd)
 {
        QTcpSocket *client = new QTcpSocket (this) ;
        client- >setSocketDescriptor (socketfd) ;
        clients, insert (client) ;


        emit clients signal(clients. count () );


        QString str;
        str = QString( "New client  from: %l ")
                 .arg(client- >peerAddress ( ) .toString () );


        emi七 messa먀乞signal(s七r) ;


        connect (client,   SIGNAL (readyRead() ), this,
                           SLOT (readyRead() ));
        connect (client,   SIGNAL (disconnected() ), this,
                           SLOT (disconnected( ) ));
 }


코드에서 보는 것과 같이 새로운 클라이언트7} 접속하면 QTcpSocket 클래스의 client 인스턴스를 생성
하고 incomingConnection( ) 함수 인자의 socketfd를 setSocketDescriptor( ) 함수를 이용해
Socket File Description을 설정한다．

die砒S培nal(）은 GUI 클래스와 통신하기 위한 시그널 이벤트이며 새로운 클라이언트 소켓이 생성되면
사용자 정보를 GI끄상에 표시하기 위해 발생하는 시그널이다．

QTcpSocket은 클라이언트로부터 새로운 메시지를 받으면 QTcpSocket의 reaclyRead( ) 시그널 이벤
트가 발생하며, readyRead( ) 시그널은 readyRead( ) 슬롯함수와 연결되어 클라이언트로부터 전송받은
메시지를 처리한다．



                                                                 ] 네트워크 371


===== PAGE 373 =====
void chatServer: :readyRead()
{
    QTcpSocket *client = (QTcpSocket* )sender () ;
    while(client- >canReadLine () )
    {
        QString line = QString: : fromUtf8 (client- >readLine () ) .trimmed( );


        QString str;
        str = QString( "Read line: %l") .arg(line) ;

        emit message_signal ( str) ;


        QRegExp meRegex ( " 八Ime: (. *)$") ;

        if (meRegex. indexln(line) != -1)
        {
            QString user = meRegex.cap(1) ;
            users[ client] = user;
            foreach (QTcpSocket *client, clients)
             {
                 client- >write (QString( "Server: %1 connect ")
                                 .arg(user) .toUtf8 ( ));
             }

            sendUserList ( );
        }
        else if (users.contains (client) )
        {
            QString message = line;
            QString user = users[ client] ;


            QString str;
            str = QString ( "User: %1, Message: %2 ")
                    .arg(user) .arg(message) ;
            emit message signal(str) ;


             foreach ( QTcpSocket *otherClient, clients)
                 otherClient->write (QString(user+" : "+message+" \n")
                                           .toUtf8 ( ));
        }

    }
}


readyRead( ) 슬롯함수는 클라이언트로부터 메시지를 전송받을 때까지 대기하고 있으며 , 메시지를 전송
받으면 readLine( ) 멤버함수를 이용해 메시지를 QString 데이터 타입 변수에 저장한다. QString어］ 저
장된 메시지는 서버어］ 접속한 모든 사용자 클라이언트로 전송한다．

入4essage_signal( ) 시그널은 GUI 클래스와 통신하기 위한 시그널이며 , QTextEdit 위젯에 로그를 출력


372 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 374 =====
하기 위한 시그널 이벤트이다．

void chatServer: :disconnected()
 {
     QTcpSocket *client = (QTcpSocket* )sender () ;


     QString str;
      str = QString ( "Client disconnected: : %l ")
             .arg(client- >peerAddress ( ) .toString( ));


      emit message_signal(str) ;


     clients, remove (client) ;

      emit clients signal(clients. count () );


     QString user = users[ client] ;
     users. remove (client) ;


      sendUserList () ;
      foreach(QTcpSocket *client, clients)
          client- >write(QString( " Server: %1 disconnect " ) .arg(user) .toUtf8 () );


 }


disconnected( ) 슬롯함수는 클라이언트가 서버로부터 접속이 종료되면 발생하는 슬롯함수이며, 접속
시 생성한 클라이언트의 QTcpSocket 클래스의 client 인스턴스를 제거한다．


              incomingConnection(int socketfd
                 새로운 클라이언트 인스턴스 생성




        readyReadO                     disconnected()
     클라이언트 메시지 처리를                  클라이언트 접속 종료
        위한 슬롯함수                        슬롯함수

（그림） chatServer 클래스 구조



그림어꺼 보는 것과 같이 readyRead( ) 슬롯과 disconnected( ) 함수에서 클라이언트 접속 유저 수와
메시지 및 로그 정보를 GUI상에 표시하기 위해 clients_signal( ）과 message_signal( ) 시그널 이벤트
를 사용한다. 이 두 개의 시그널은 widget 클래스의 slots_btnStart( ）와 slot clients( ) 슬롯함수와 연
결되어 있다．




                                                                                     ] 네트워크 373


===== PAGE 375 =====
            void Widget: :slotsbtnStart ()
            {
                    bool success = server->listen (QHostAddress: :Any, 9999) ;
                    if (success) {
                               U卜갸e＞代Edi七1相ppend( "Cha七 Server start " ) ;
                     }else{
                               ui- 比이比Ed此수append ( "Chat Server error " ) ;
                     }
            }

        void Widget: :slot                     clients (int       users)
            {
                    QString str = QString( "Clients : %1") .arg(users) ;
                    ui- >label->setText ( str) ;
            }


slot邑btnStart(）는 GUI의 textEdit 위젯에 메시지를 출력하기 위한 슬롯함수이고, si毗下lients( ) 함
수는 GUI 하단의 클라이언트 수를 label 위젯에 표시하기 위한 슬롯함수이다．

'亘jChatServer                            :1,                       I口 匣l臼
                                                            QTe났Ed往
                Server Statt口                               /
                               「汗J                      g
                Chat Sep.喀f 馱art
                New client from: I27.t1al
                Re自d line: /me:eddy




 (Clients
                         : 1         )          QL3m1
（그림） Chat Server 예제 실행 화면



. 채팅 클라이언트 예제 어플리케이션
chatClient 어플리케이션은 ChatServer 어플리케이션에 접속하여 서버어］ 접속한 클라이언트어］ 메시지
를 전송하거나 서버로부터 메시지를 전송받기 위한 어플리케이션이다. chat（개ent의 GUI 인터페이스는
다음과 같다．




374 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 376 =====
  큐라이언트 로그인 GUI                        景라이언트 메시지 전송 GUI
                             陌呼回    iiChat三hent        各，』i系；i

                                       Sero口rdorothy oonn.CUU,.thd口r口
                                       dn,oIhy: F4&Io Eddy




                                                                        ［垂回


（그림） chatClient 예제 실행 화면



첫 번째 로그인 UI에서 서버 주소와 유저명을 입력하고 [LOGIN] 버튼을 클릭하면 서버 어플리케이션에
접속을 시도하며 접속이 완료되면 두 번째 {-II가 활성화된다．



 class MainWindow : public QMainWindow
 {
      Q OBJECT


 public:
      explicit    MainWindow (QWidget *parent = 0) ;
      -MainWindow() ;


 private:
      Ui: :MainWindow *Ui;


 private slots:
      void oneloginButtonclicked() ;
      void on sayBu七七O1느clicked( ) ;
      void readyRead() ;
      void connected() ;


 private:
      QTcpSocket; 火socke七；
 };


서버와 같이 chatClient 어플리케이션도 [LOGIN] 버튼을 클릭해 서버와 연결하기 위해1QTcpSocket
클래스의 socket 인스턴스를 생성자에서 선언한다．




                                                                              ] 네트워크 375


===== PAGE 377 =====
 void MainWindow: :on loginButtonclicked()
    {
            socket->connectToHost (ui- >serverLineEdit->text () , 9999) ;




[LOGIN] 버튼을 클릭하면 on_loginButton_clicked( ) 슬롯함수가 호출되며 생성자에서 초기화한
QTcpSocket 클래스의 socket 인스턴스를 이용해 서버로 접속을 시도한다. connectToHost( ) 함수의
첫 번째 인자는 서버의 호스트 정보를 지정하고 두 번째 인자는 서버의 포트를 지정한다．

 MainWindow: :MainWindow ( QWidget *parent) :
     QMainWindow(parent) ,ui (new Ui: :MainWindow)
 {
        ui- >se七upUi ( 七hi引 ;
            ui- >stackedWidget->setCurrentWidget (ui- >loginPage) ;
            socke七 = new QTcpSocke디thi引 ;


        connect (socket, SIGNAL (readyRead() ), this,            SLOT (readyRead() ));
        connect (socket, SIGNAL (connected() ), this,             SLOT (connected() ));
 }


클래스 생성자에서는 클라이언트 소켓을 위한 socket 인스턴스를 초기화하며 socket 인스턴스를 이용해
메시지를 서버로부터 전송받기 위해 readyRead( ) 시그널을 readyRead( ) 슬롯함수와 연결하고 서버로
부터 접속 결과를 받기 위해 connected( ) 시그널을 connected( ) 슬롯함수와 연결한다．

 void MainWindow: :readyRead()
 {
        while (socket->canReadLine () )
        {
                QString line = QString: : fromUtf8 (socket->readLine ( ) ) .triittmed() ;
                QRegExp messageRegex ( " 八 ([ 느]+):(. *)$") ;


                if (messageRegex.indexln(line)      != -1)
               {
                    QString user = messageRegex.cap(1) ;
                    QString message = messageRegex.cap(2) ;
                    ui- >roomTextEdit->append( '<b> '' +user+" </b>: "+message) ;




void MainWindow: :connected()
{
        ui- >stackedWidget->setCurrentWidget ( ui- >chatPage) ;
        socket->write(QString( " /me: "+ui- >userLineEdit->text ()
                                           + '! \n', )．七아凡f8 ( ) ) ;




376 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 378 =====
readyRead( ）는 서버 어플리케이션에서 메시지를 전송받기 위한 슬롯함수이며 서버로부터 메시지를 전
송받을 때까지 대기한다. connected( ）는 on_loginB毗的n_clicked( ) 슬롯함수에서 서버에 접속하고
서버로부터 연결된 정보를 받기 위한 슬롯함수이다．

                                                             \

 socket=new QTcpSocket(this); C={> connectToHost(server,port);
생성자에서 socket 인스턴스 초기화                       서버접속
                                                             I


                                               8
            readyRead()               connected()
        서버로부터 메시지 처리룰               클라이언트 접속 종료
           위한 슬롯함수                     슬롯함수
                                                      7


（그림） chatClient 어플리케이션 구조



그림에서 보는 것과 같이 socket 클래스 인스턴스를 초기화하고 connectT아如st( ) 함수를 이용해 서버로
접속을 시도한다. readyRead( ）는 서버로부터 메시지를 전송받기 위한 슬롯함수이고 connected( ）는
connectToHost( ) 함수어］ 의해 접속을 시도하고 서버로부터 접속 결과를 처 리하기 위한 슬롯함수이다．




                                                                 L네트워크 377


===== PAGE 379 =====
01 5 Programming




F尸 2 ' Q t＼사ebK仕
        1 아는 웹 브라우저를 사용해 어플리케이션 개발이 가능하도록 WebKit 오픈소스 프레임워크를 제공한
          다. 이번 장0似怯 （카에서 제공하는 QtWebKit 모듈을 사용해 웹 어플리케이션을 개발하는 방법에 대
          해 알아보도록 하자．




WebKit은 웹 브라우저를 만드는데 사용하는 오픈 소스 프레임워크이다. KDE 프로젝트의 일환으로 1I
발되었으며 지금은 아이폰, 안드로이드 플랫폼과 같은 모바일, 임베디드 디바이스에서의 웹 브라우저를
제공하기 위한 목적으로도 사용되고 있다．

Qt에서 제공하는 QtWebKit 모듈은 \WebKit 오픈 소스 엔진 기반이다. QtWebKit 모듈은 HTML
(HyperText Markup Language), XHTML(eXtensible HyperText Markup Language), CSS
(Cascading Style Sheets), SVG(Scalable Vector Graphics), HTML5, JavaScript **   위젯 상에
렌더링 기능을 제공한다．

Qt에서 제공하는 QtWebKit 모듈은 JavaScript와 Qt 오브젝트간의 통신이 가능하다. 이는 매우 유용
하다. 예를 들어 QtWebKit 상에서 동작하는 웹 어플리케이션을 시스템 미들웨어와 통신하기 위해1 IPC
(Inter Process Communication), RPC 등과 같은 방법을 사용해야 한다. 하지만 Qt에서는 제공하는
QtWebKit Bridge를 사용해 시스템 미들웨어 또는 플랫폼 커널과 통신할 수 있는 모듈을 쉽게 구현할
수 있다．

QtWebKit 모듈에서 제공하는 클래스를 사용하기 위해 다음과 같이 헤더 파일을 소스 코드에 추가해야
한다．

      ude <Q蜘陀bkit>


또한 qmake 프로젝트 파일（.pr이에 다음과 같이 추가해야 한다．

QT +== webkit


많은 플랫폼에서 Debugging Symb아을 포함해 WebK比을 함께 빌드하는 것은 \JebKit 엔진의 크기 문
제로 인해 많은 문제가 있다. 그렇기 때문에 임베디드 플랫폼상에서는 Release Mode에서 Build하기 권
장한다. 그리고 gcc를 사용할 때 Debugging Symb이을 제거하고 컴파일하는 것을 권장한다．



378 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 380 =====
0o싸VebKit 아키텍처
QtWebKit 모듈을 사용해 Contents 렌더링을 구현하는 방법 중 가장 쉬운 방법은 邸WebView 클래스
를 사용하는 방법이다. 이 클래스는 위젯과 같이 GUI Form 및 Graphics View 상에 내장된 형태로
URL 다운로드와 Web Site 렌더 링을 쉽게 구현할 수 있다．

QWebView *vjew = new QWebView(parent) ;
view->load(QUrl( "http: //www.qt-dev. com/ ") ) ;
view->show () ;



邸WebView 클래스는 \Web Page를 Rendering하는 기능을 제공한다. QWebView 인스턴스는 한 개의
QWebPage를 가지고 있다. QWebPage는 웹 페이지에서 문서 구조를 접근하기 위한 기능을 제공한다．
Frame과 같은 구조를 서술, Web page의 I끄毗아y를 탐색 및 수정을 위한 Undo/Redo Stack을 포함
하고 있다．

HTML 문서는 중첩된 Frame을 사용할 수 있다. Qt는 HTML 문서 내에서 중첩된 Frame을 구성할 수
있도록 邸WebFrame 클래스를 제공한다. 이 클래스는 JavaScrij亢 window 오브젝트와 브리지 기능을
포함하고 있다. 따라서 邸WebFrame은 QPaii此아를 사용할 수 있다. 각각의 邸WebPage 클래스는
八4am1l Frame과 같이 한 7귀 이상의 QWebFra표m을 가지고 있으며 Main Frame은 여러 개의 Child
frame을 가지고 있다．

HTML Docum아此의 각 Elem이孔는 웹 페이지 ．내에 D0M JavaScript를 경유해 접근할 수 있다．
QWebK此은 QWebElen回此가 제공하는 Element를 경유해 각 HTML 문서의 El帥ient를 접근할 수
있다. 邸WebElement 오브젝트는 CSS를 사용해 QWebFrame 클래스 findAllElements( ) 함수와
findFirstElemetns( ) 함수를 사용해 각 Elem아此를 획득할 수 있다. 일반적인 웹 브라우저의 각 특징
(Feature）은 QWebSettir培S 클래스를 통해 설정이 가능하다. 이 클래스는 QWebPage의 모든 인스턴
스의 기본설정을 조작할 수 있다．


1Netscape 플러그인 지원
Webkit이 Netscape 플러그인 API를 지원한 이래로 QtWebKit 모듈 또한 Netscape 플러그인 기능을
지원한다. Netscape 플러그인 기능은 플랫폼 상에서 지원해야만 사용할 수 있다. 만약 플랫폼 상에서
Netscape 플러그인 기능을 지원한다면 邸WebSetti始S 클래스의 PluginsEnabled 속성을 활성화해야
만 QtWebKit 모듈에서 Netscape 플러그인 기능을 사용할 수 있다．


Linux/Unix 플랫폼

 · .mozilla/plugins in the user " s home directory
 · .mozilla/plugins in the user' s home directory
 · .netscape/plugins in the user' s home directory
 1System locations, such as
   - /usr/lib/ browser/plugins
   - /usr/local/ lib/ mozilla/plugins                              O

                                                         2 （거WebK什 379


===== PAGE 381 =====
  - /usr/lib/ firefox/ plugins
  - /usr/11b64 /browser-plugins
  中 /usr/lib/ browser-plugins
  中 /usr/lib/ mozilla/plugins
  - /usr/local/ netscape/plugins
  - /opt/mozilla/plugins
  小 /opt/netscape/plugins
  - /opt/netscape/communicator/plugins
  - /usr/lib/ netscape/plugins
  -   /usr/lib/ netscape/plugins-1ibc5
  -   /usr/lib/ netscape/plugins-1ibc6
  -   /usr/1ib64/netscape/plugins
  -   /usr/1ib64/mozilla/plugins
 ·Locations specified by environment variables:
  - $MOZ ILLAeHO卜E /plugins
  - $MOZ PLUGIN PATH
  - $QTWEBKIT PLUGIN PATH



윈도우 플랫폼

 ·The user' s Application Data\Mozilla\plugins directory
 ·Standard system locations of plugins for Quicktime, Flash, etc.


Mac OS X 플랫폼

 .Library/ Internet Plug-Ins in the user's home directory
 ·The system /Library/Internet Plug-Ins directory




S WebK仕 라이선스
QtWebkit 모듈은 \WebKit 오픈 소스 엔진을 기반으로 제공하는 모듈이다. Qt에서 지원하는 WebKit
모듈의 버전을 확인하기 위해 Qt 디렉토리의 src/3rdparty/webkit/ VERSION 파일을 통해 확인할 수
있다. Qt는 Commercial Edition과 Open Source Edition으로 나눠진다．

Qt Commercial Edition은 QtWebKit 모듈이 필요한 경우 LGPL(GNU Library General I뇨blic
License）을 따라야 한다. Qt Open Source Edition을 사용하는 경우 GNU LGPL의 버전어］ 따라 모듈
을 재배포해야 한다．

WebKit은 GNU Library General I뇨blic License를 따른다. 따라서 QtWebl（此을 사용하는 경우 소
스 코드상에 배포자 이름과（兀pyright를 명시해야 한다. Free Software Foundation에서 제공하는 라
이선스의 규칙하에 수정하거나 재배포가 가능하다．




380 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 382 =====
      2.1 QtWebkit 모듈에서 제공하는 클래스

Qt에서 제공하는 QtWebKit 모듈은 웹 응용 어플리케이션을 구현할 수 있도록 다양한 클래스를 제공한
다. 예를 들어 웹 브라우저 상에 렌더링된 페이지의 DOM 트리 분석과 제어를 위한 QWebElement 클래
스를 제공하고 웹 페이지의 Frame과 His的ry를 사용해 다양한 형태의 웹 응용 어플리케이션을 구현할
수 있다．

뿐만 아니라 QtWebKit 모듈에서는 JavaScript를 통해 웹 페이지를 조작할 수 있도록 0++ 바인딩 기
능을 제공한다. 이번 장에서는 QtWebK此에서 제공하는 다양한 클래스어］ 대해 알아보도록 하자．


S QtWebK仕 모듈에서 제공하는 클래스

클래스                     설명

QWebDatabase            JavaScri아를 사용해 HTML5 WebDatabase에 접근하기 위한 기능을 제공하는
                        클래스

QWeb티emerit             QWebFrame 내에서 D아VI 티emen怡를 편리하게 접근할 수 있는 클래스
QWebElemerit(二에ection   웹 요소의 컬렉션을 나타내71 위하1 사용하는 클래스
QWebFrame               웹 페이지 내에서 다ame 표시

QWebHistory             웹 페이지의 History 정보를 제공
QWebHistor닌nterf ace    링크 네5幻ry를 구현하기 위한 인터페이스
oWebHistoryltem         QWebPage 클래스의 History 내에서 하나의 아이템을 표시하71 위한 클래스
QWebH仕TestResult        테스트를 위해 선택한 월j 페이지에 관련한 정보를 제공

QWeblnspector           ioWebPage의 Inspecto四J 제어와 배치를 위한 클래스． Ins口ector는 페이지의
                          계층 구조의 로딩 통7카 및 개별 요소의 현재 상태를 표시할 수 있다．
                          대부분 웹 페이지 개발자에 의해 사용된다．

 oWebPage                View의 오브젝트와 Web 문서의 수정을 위한 클래스

 QWebP山ginFactory        웹 페이지에서 Embed custom 데이터 타입을 사용
 QWebSecurityOrigin      웹 사이트를 위한 보안 Boundary를 정의

 QWebSettings            QWebPage와 QWebFrame에 의해 사용되는 설정을 저장하71 위한 클래스
 QWebView                View를 사용하고 웹 문서를 수정하기 위한 위젯




S OWebDatabase 클라쓰
HTML5 표준은 웹 사이트를 생성하고 JavaScript를 통해 로컬에 존재하는 SQL 데이터베이스에 대해
액세스할 수 있는 지원이 포함되어 있다. 邸WebDatabase 클래스는 데이터베이스를 조작할 수 있는
c++ 기반의 인터페이스를 제공한다．

각 데이터베이스는 각 데이터베이스를 구분하기 위한 데이터베이스 이름을 가지고 있다. 데이터베이스를
 얻기 위해 name( ) 멤버함수를 사용할 수 있다．

 Webi（仇은 로컬상어］ 존재하는 SQL 데이터베이스를 생성하고 접근하기 위해 SQLite를 사용한다. 로컬
 파일 시스템에 존재하는 데이터베이스 파일의 위치는 邸VebDatabase 클래스의 filename( ) 멤버함수
를 통해 리턴받을 수 있다．

                                                                           乙아WebK作 381


===== PAGE 383 =====
 QWebDatabase webdb =
 QSqloatabase sqldb = QSqlDatabase: :addDatabase ( "QSQLITE",   "myconnection") ;
 sqldb. setDatabaseName (webdb. fileName ( ) ) ;
 if   (sqldb.open ( ) ) {                                                    1
       QStringList tables = sqldb.tables () ;                            1       1




 0QWeb다ame 클래匹
邸A/ebFrame 클래스 웹 페이스 내부에 존재하는 Frame을 표시하기 위해 제공되는 클래스이다．
邸AlebFrame 클래스는 웹 페이지 내에 포함된 모든 Frame을 표시한다. 邸VebPage 오브젝트는 척어
도 하나이상의 Frame을 포함한다. 帥A[ebPage 클래스의 mainframe( ）을 사용해 메인 Frame을 획득
할 수 있다．

Frame은 load( ) 함수와 setUrl( ) 함수를 사용해 로딩할 수 있다. 또 다른 방법으로 HTML의 Content
를 활용하기 위해서 setHtml( ) 함수를 대신 사용할 수 있다. page( ) 함수는 웹 페이지 오브젝트의 포인
터를 리턴한다．

QWebFrame 클래스는 현재 Frame어］ 의해 로딩된 URL뿐만 아니라 원래의 Request URL 모두 검색
할 수 있는 방법을 제공한다. 이러한 방법은 로딩되는 과정 동안 발생한 Redirection과 DNS를 검색할
수 있도록 히용한다. requestedUrl( ) 함수는 Frame History에서 추가된 URL과 매칭할 수 있다．

HTML frame의 제목은 title( ) 함수를 통해1 접근할 수 있다. 추가로 frame은 아이콘을 지정할 수 있다．
frame에서 지정한 아이콘어］ 접근하기 위해서 icon( ) 함수를 사용할 수 있다. 만약 제목과 아이콘을 변
경하면 titleChanged( ）와 icon（그hanged( ) 시그널 이벤트가 발생한다. zoomFactor ( ）는 frame에서
표시될 내용의 전체 크기가 변경하기 위해 사용할 수 있다．

QWebFrame 오브젝트는 웹 페이지를 생성하고 제어할 수 있는 기능을 제공하고 새로운 frame을 생성하
기 위해 공지하는 시그널인 frameCreated( ）과 연결할 수 있다. frame의 내용을 구현하기 위한 테스트
목적으로 사용할 수 있는 여러 가지 방법이 있다. hitTestContent( ) 함수는 위치어］ 의해 배치된 Element
를 찾기로 사용할 수 있다. 또한 DOM의 트리 구조상에서 접근하기 위해 documentElement( ),
findAllElements( ) 그리고 findFirstElement( ) 함수를 사용할 수 있다．

QWebFrame 클래스는 print( ) 함수를 사용해 QPrinter 상에서 프린트할 수 있는 기능을 제공하며
QPrir此PreviewDialog 클래스의 paintRequested( ) 시그널과 연결할 수 있다．


0QWebElement 클래스
邸VebElement 클래스는 邸A[ebFrame에서 DOM Element어］ 접근하기 위한 기능을 제공한다. 이 클래
스는 Document model어］ 쉽게 접근할 수 있는 기능을 제공한다. DOM Tree의 root는 Document ele
 meat를 호출하고 QWebFrame::documentElem帥t( ) 함수를 사용해 접근할 수 있다．



382 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 384 =====
특정 Element를 findAll( ）과 findFirst( ) 함수를 사용해 접근할 수 있다. 이러한 Eleme毗는 css
select아를 사용해 고유한 식별자를 제공한다. 아래는 findAll( ) 함수의 사용 방법이다．

QWebEl回陀nt document = frame->documentElement () ;
／出
     <p class=intro>
       <span>Intro</ span>
       <span>Snippets< /span>
     </p>
     <p>
       <span>Content</ span>
       <span>Here</ span>
     </p>
士／
QWebElementCollection allSpans = document. findAll ( "span") ;
QWebElementCollection introSpans = document. findAll ( "p.intro span") ;



첫 번째 리스트 Docum아此에서 모든 span 피eme砒를 포함한다. 두 번째 리스트는 intro가 속한 p의
Child Elem아此를 포함한다. 그리고 리스트에서 첫 번째 Element를 리턴하기 위해 제공하는 find
First( ) 함수는 findAll( ) 함수를 사용하는 것보다 효과적이다. 또한 findChild( ) 함수와 nex侶illing( )
함수를 사용해 수동으로 Docum아此를 탐색할 수 있다．

 frame->setHtml( "<html><body><p>First Paragraph</p>
                               <p>Second Paragraph</p></body></html>") ;

QWebElement doc = frame->documentElementU;
QWebElement body = doc. firstChild () ;
QWebElement firstParagraph = body. firstChild ( );
QWebElement secondParagraph = firstParagraph.nextSibling() ;



각 Elem이此는 attribute( ) 혹은 setAttribute( ) 함수와 같은 메소드를 사용해 속성을 변경하거나 탐색
할 수 있다. 예를 들어 텍스트 필드에 사용자가 입력한 값을 얻기 위해 다음과 같이 사용할 수 있다．

QWebElemen七 firs七Te>＜七Inpu七 = documen七．findFirs七（" inpu七［七ype＝七ex七］" ) ;
QString storedText = firstTextlnput.attribute ( "value") ;



그리고 사용자가 입력한 필드의 값을 수정하기 위해 입력 Element의 속성을 setAttribute( ) 함수를 사
용해 다음과 같이 변경할 수 있다．

QWebElemen七 firstTe＞比Inpu七 = document. findFirs七（"inpu七［七ype＝七ext] " ) ;
textlnput.setAttribute ( "value", storeciText) ;



에뮬레이터를 수행하는 방법과 같이 특정 Elem이式의 이벤트를 수행할 수 있다. 다음 예제의 소스 코드
는 Submit 버튼의 JavaScript DOM click( ) 메소드를 호출하는 방법이다．


                                                                           2 QtWebKit 383


===== PAGE 385 =====
 QWebElement document = franie->documentElement () ;
 ／士
     <form name= " myforin" action=" submit_form. asp" method= " get ">
           <input type=" text " na끄［1e="myfield">
               <input type=" submit " value=" Submit">
          <If orm>



 QWebElernen七 bu七七on = 面cunient. fin姐irs七( '녈마)Ut［七ype=submi七］" ) ;
 button. evaluateJavaScript ( "clickQ ") ;




1QWebH暾ory와 QWebHistorylnterf ace 클래스
邸VebHist야y 클래스는 印WebPage의 His切ry를 다루기 위해 제공되는 클래스이다. 각각의 邸Veb
Page 인스턴스는 QWebPage: :hi毗야y( ) 함수에 의해 방문했던 웹 페이지의 II五story를 접근할 수 있
다. Hi毗ory는 현재 페이지를 기준으로 이전에 방문했던 페이지와 현재 페이지에서 앞에 방문했던 페이
지를 back(）과 如rward( ) 함수를 사용해 History 정보를 얻을 수 있다．

현재의 페이지와 이전에 방문했던 페이지를 아이템으로 간주했을 때 backltems( ) 함수는 이전에 방문
했던 아이템을 호출해 얻을 수 있다．

그리고 현재 페이지 아이템을 기준으로 Back 페이지 아이템이 존재하는지 확인하기 위해서 canGo
Back( ) 함수를 사용해 리턴 값을 얻을 수 있다. 만약 참이면 true를 리턴한다. 또한 Forward 페이지 아
이템이 존재하는지 확인하기 위해I canGoForward( ) 함수를 사용하면 된다．

帥WebHistorylr此erface 클래스는 링크 His的ry를 구현하기 위해 제공되는 클래스이다. 이 클래스는
방문했던 링크를 유지하기 위해 사용할 수 있으며 \WebKit 엔진에 의해 호출되는 순수한 \lirtual
method를 포함하고 있다. AddHis的ry( ) 함수는 방문했던 URL을 추가하기 위해1 사용한다. 그리고 사
용자가 방문했던 URL을 검색하기 위해 historyContains( ) 함수를 사용할 수 있다．


兮 QWeb네S幻ryltem 클래스
邸A[ebHistoryltem 클래스는 QWebPage의 His切ry 중어］ 한 개의 Item을 표시하기 위해 제공되는 클
래스이다. 이 클래스의 인스턴스는 웹 페이지의 His的ry 스택에서 Entry 정보를 얻을 수 있으며 해당 페
이지가 포함하는 정보 및 마지막에 방문했던 페이지의 정보를 얻을 수 있다. 다음 표는 I五毗町y Item에
의해 제공되는 페이지의 속성을 보여준다. 각 함수들은 아이템을 접근할 수 있다．

함수                   설명
title()              페이지의 제목
url()                페이지의 위치
origin톄Url()         페이지를 접근하71 위해 사용하는 URL
IastVisited()        사용자가 마지막에 방문했던 페이지에 대한 날짜와 시간 정보
icon()               서버가 제공하는 페이지의 아이콘
userData()           History 아이템을 사용하1 저장된 데이터


384 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 386 =====
S QWebHitTestResu仕 클래낱느
印WebHitTestResult 클래스는 테스트 목적으로 사용하는 클래스이다. 이 클래스는 특정 웹 페이지를
클릭한 다음 방문한 페이지에 대한 정보를 제공한다. QWebHitTestResult 클래스는 특정 위치의 웹 페
이지 내용과 관련한 정보를 제공하기 위해 邸WebFrame: :h此TestContent( ) 함수가 제공하는 정보를
리턴한다．


S QWeblnspector 클래스
QWeblnspe毗or 클래스는 QWebPage 검사의 위치와 제어 기능을 제공하는 클래스이다. 이 클래스는
개발자가 페이지를 상하 구조로 표시할 수 있으며 각 Elem町此의 상태를 검사할 수 있다. 검사할 페이지
는 setPage( ) 함수를 사용해 다음과 같이 지정해야 한다．

II . . .
QWebPaqe *page = new QwebPage;
II . . .


QWeblnspector *inspector = new QWeblnspector;
inspector->setPage (page) ;



eQWebPage 클래스
QWebPage 클래스는 View와 Edit Document 페이지 오브젝트를 제공한다. 印AlebPage는 웹
Content, Setting, History link 그리고 Action을 구현하기 위한 메인 frame을 지정할 수 있다. 그리
고 이와 함께 邸WebFrame을 사용하며 위젯이 없는 환경에서 印WebView와 같은 기능을 제공하는 클래
스이다．

印WebPage의 API는 QWebView 클래스와 유사하다. Action( ）과 같은 일반적인 기능을 제공하며
trigerAction(), findText(), settings( ) 함수를 제공한다. 邸WebView와 달리 QWebPage 클래스는
위젯을 제공하지 않는 환경에서 사용하는 목적으로 제공한다. 다음은 QWebPage 클래스를 사용해
Thumbnail 클래스를 구현한 예이다．

class Thumbnailer : public QObject
{
   Q OBJECT
public:
   Thumbnailer (const QtJrl &url) ;

Q SIGNALS:
    void finished() ;

private Q SLOTS:
    void render ( ) ;

private:
     QWebPage page;
};


                                                                2 QtWebKit 385


===== PAGE 387 =====
Thumbnail 클래스의 생성자는 URL의 정보를 얻어온다. 邸?VebPage의 오브젝트를 render( ) 슬롯함
수와 연결한다. render( ) 함수는 QWebPage 오브젝트를 사용해 thumbnail을 드로잉 할 수 있다．

void Thumbnailer: : render ()
{
    page. setViewportSize(page.mainFraine ( )->contentsSizeQ) ;
    Qlmage image(page.viewportSize ( ), Qlmage: :Format_ARGB32) ;
    QPainter painter (&image) ;


    page.mainFrame ( )->render (&painter) ;
    painter.end() ;
    Qlmage thumbnail = image. scaled(400, 400) ;
    thumbnail. save ( "thumbnail.png") ;

    emit finished( ) ;
}


viewportSize를 설정하고 viewportSize와 같은 크기로 Qlmage 오브젝트를 초기화한다. 이미지는 페
이지 인자로 보낸다. 다음으로 메인 frame어］ Drawing한 이미지 Pal:式er를 Renderii培한다. 마지막으
로 이미지 Scaling을 처리하여 thumbnail.png에 저장한다．


0QWebP山qnFactory 클래스
QWebPlugix伊ac的ry 클래스는 웹 페이지에 사용자 정의 데이터를 내장하기 위해 제공하는 클래스이
다. 웹 페이지상어］ 임의의 데이터를 내장하기 위해 HTML의 佃bject>를 다음과 같이 사용한다．

<object type=" application/x-pdf "
         data＝샤比tp: /／啣吼qt-dev. Co可docuine毗 .pdf "
         width=" 500 " height=" 400 " ><Iobject>



QtWebKit은 기본적으로 text/html과 image/jpeg과 같은 데이터 타입을 Handling할 수 있다． 하지
만 사용자 정의 데이터 타입을 Handling할 수 없다. 따라서 邸WebPlugir巾ac的ry 클래스는 邸Web
Page상에서 I가ugin을 생성할 수 있는 기능을 제공한다. 하나의 Plugin을 만들기 위해 邸A[ebPage: :set
PluginFactory( ) 함수를 사용해 邸WebPage 상에 설치할 수 있다．


0QWebSecurityOr呵n 클래스
邸WebSecur此yOrimn 클래스는 웹 페이지의 Security Boundary를 정의할 수 있는 기능을 제공한다．
즉 邸WebSecur此yOrigin 클래스는 웹 사이트에 의해1 정의된 Security domain어］ 접근하기 위한 기능
을 제공한다. 예를 들어 같은 데이터베이스를 공유하는 같은 도메인에 존재하는 공유 도메인만 접근할 수
있도록 하기 위해 제공되는 클래스이다．

Security origin 내어］ 정의된 뎨이터베이스에 접근하기 위해 databases( ）를 사용하며, 현재 제한된 디
스크 사용량을 제한하거나 참조하기 위해 setDatabaseQuota( ), databaseQuota( ), database


386 CHAPTER 12= 데이터 커뮤니케이션과 인터넷 프로그라俚J


===== PAGE 388 =====
Usage( ) 함수를 사용할 수 있다．


I OWebSettings 클래스
邸WebSetti叩S 클래스는 邸AlebPage와 邸WebFrame에서 사용한 설정 정보를 저장하기 위한 오브젝트
를 제공한다. 각 邸WebPage 오브젝트는 페이지의 설정 정보를 저장할 수 있는 소유의 印WebSettings
오브젝트를 가지고 있다. 만약 설정을 사용하지 않는다면 Global 설정 오브젝트를 검색해야 하며
（丑obal 설정은 멎oba好ettings( ) 함수를 사용해 접근할 수 있다．

帥VebSettings는 브라우저의 프로피티 설정을 저장할 수 있다. 예를 들어 폰트 Family와 폰트 크기가
같은 정보는 설정어］ 저장할 수 있다. 그리고 Custom style sheet의 위치, JavaScript 및 I가ugin과 같
은 속성을 저장할 수 있다．


心 0WebView 클래스
QWebView 클래스는 웹 문서를 수정하거나 \[jew를 사용하기 위한 위젯을 제공하는 클래스이다. 이 클
래스는 웹 브라우저 모듈을 위젯에 표시하기 위한 컴포넌트를 제공한다 ．예를 들어 인터넷으로부터 웹
Contents를 표시할 수 있는 응용 어플리케이션에 다양한 목적으로 웹 페이지를 렌더링할 수 있는 위젯
을 제공한다．

 QWebView *vjew = new Qwebview(parent) ;
 view->load(QUr1( "http: //www.qt_dev.com/ '' ) );
 view->show() ;



load( ) 함수를 사용해 Qt에서 제공하는 위젯과 같은 형태의 위젯상에 인터넷 웹 사이트를 로딩할 수 있
다. 또한 SetUrl( ) 함수를 통해 특정 웹 사이트를 지정할 수 있다．

邸WebView에서 웹 사이트 로딩이 시작되면 loadStarted( ) 시그널 이벤트가 발생한다. 그리고 로딩이
완료될 때까지 현재 로딩 진행 상태를 제공하기 위한 목적으로 loadProgress( ) 시그널 이벤트를 제공한
다. 로딩이 완료되면 loadFinished( ) 시그널 이벤트가 발생한다．

page( ) 함수는 웹 페이지의 포인터를 리턴한다. 웹 페이지 \[jew의 설정을 수정하기 위해 邸WebSet-
tings 오브젝트어］ 접근할 수 있다. QWebSettii培S 오브젝트어］ 접근하기 위해서 settings( ) 함수를 사
용하면 된다. QWebSettings 클래스는 디폴트 폰트를 변경할 수 있으며 , JavaScript 및 Plugin과 같은
Feature들을 활성화하거나 비활성화 할 수 있다．

HTML 문서의 제목어］ 접근하기 위해서는 title( ) 프로피티를 사용하고, 웹 페이지에서 사용한 아이콘에
접근하기 위해서는 icon( ) 프로퍼티를 사용할 수 있다. 만약 아이콘과 제목을 변경하면 titleChanged()
와 icon（그hanged( ) 시그널 이벤트가 발생한다. 만약 Custom context 메뉴 이벤트를 사용하기 위해서
는 context八4enuEvent( ) 함수를 사용할 수 있다. 그리고 pageAction( ) 함수로부터 획득한 Actions
를 사용해 帥4enu를 채울 수 있다.




                                                             2 QtWebKit 387


===== PAGE 389 =====
邸WebView 클래스는 QPrinter 상에서 print( ) 함수를 이용해 프린트할 수 있는 기능을 제공한다. 이
러한 프린트 기능은 QPrintPreviewl五alog 클래스의 paintRequested( ) 시그널을 사용하면 편리하게
구현할 수 있다. 새로운 윈도우를 허용하는 웹 사이트에서 지원을 목적으로 팝업과 같은 새로운 윈도를
Open할 수 있는 기능을 제공한다. 이 기능은 createWindow( ) 함수를 사용하면 된다．

邸WebView 클래스는 帥WebFrame과 QWebPage와 같은 다른 오브젝트들로 구성된다. 다음 그림은 오
브젝트의 구성도를 도식화한 그림이다．


            QWebView


                 1                         ,/ QWebView::page() 함수를 사용해
                             //               웹페이지를31져온다·
            oWebpage



                                                 / QWebView::m톄nFrame() 함수를 사용해
            QWebFrame              ///             메인Frame늘가져온다·

  1
        1

（그림） 0Web View 클래스의 오브젝트 구성




                       DOM(Document Object 卜加del) 검색

이번 장에서 다룰 예제는 Qt를 설치하면 기본 예제로 포함된 DOM 邸WebElement Traversal 예제이
다. 이 예제는 특정 웹 페이지의 DOM 인터페이스를 통해 DOM Tree 구조를 분석하기 위한 웹 응용 어
플리케이션 예제이다．

      neD 닙 e뗘En L兀｝

 Document Structure
  J HEAD
       META
                          出 Qt 개발자 커뮤니티
       M日A                                          http刃나W比qt-dev.com
       M日A                  HOME             클래스        다문로드         커뮤Li8
       TITLE
       STYLE               ｝初me          공지人H甘   주요뉴스 & 뉴스aEl     Or 싣젼 프로그래밈
       SCRIPT
       SCRIPT
  d 日SITS                 그H그 U
                                                     곰지사함
       아V                 비딜벋＝
       마V                         세밀빈호 거덕             지빙a서 St 스터Ci 진행
       SCRIPT                                        口 Ut En口CV 3rou口 없udy 모밈 커己큘럼
                             회뭔돋록         비번분실
       STYLE
       gCRn가                                         亡 Ut 개먈자 스터디 모밈 곰지
       D짜




（그림） Web 티ement D아너 Traversal 예제 실행 화면



邸A[ebElement 클래스는 Document Object Model 인터페이스를 경유해 웹 페이지의 내용과 구조를
사용할 수 있는 API를 제공하며 Document의 구조를 탐색할 수 있다. 이 예제는 웹 페이지를 표시하기
위해 QWebView 위젯을 사용한다. 그리고 DOM 트리 구조를 표시하기 위하1QTreeWidget을 사용하였
다. 왼쪽에 위치한 QTreeWidget은 Dock 위젯이므로 윈도우에서 분리할 수 있다．



388 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 390 =====
0000,BBBB SOBOt m       i크 Web 티INtent 0口＼.1 TnawocS'

       Dlv
     1 TABLE
        d 08000                     Qt 개발자 커뮤니 티
            S TB                                        hBtp//w나놔.ql-d日VJmm
     J TAPII
                              HOME            콜해스           U운로 드        커뮤나日
        1 18000
           d TB                                                       01 희전 프로그H咽
                                              !     추요뉴스 & 杵스격터
               :> 10
               t TO
                S TO                                     공지사항
                그 TD
               : T［그               비밀변호 가걱               口 지방메서 m 스터口 진햄
                1 T［그
                              휘윕듕묘       비번분실             ！거 巳叩ant Orou口 닦sly 모밈 커리큘럼 l
                  -ID
       TPBLE                                              그1 겨달자 스E卄그 모임 공지
                                                                                          寸
        Sc町PT
                                                                                     1
       TABLE
        TABLE




（그림） Dock Widg이의 분리된 화면



S Window 클래스 정의
Window 클래스는 帥4ain硝ndow와 분리되고 Qt Designer를 사용해 생성한 GI끄를 생성하였다. 따
라서 이 클래스는 UIC(User Interface Compiler）에 의해 생성된 GUI와 분리된다．

 #include 'ui window.h"


 class Window : public QMainWindow, private Ui: :Window
 {
          Q OBJ丑CT


 public:
           Window (QWidget *parent = 0) ;
           void setUrl (const QUrl &url) ;


 public slots:
     void on_webView_loadFinished() ;


 private:
           void exaniineChildElements (const QwebElement &parentElement,
                                       QTreeWidgetltem 柱沮ren七I七em) ;
  };


 이 예제에서 중요한 함수는 onwebViewloadFinished( ) 슬롯함수와 examineChildElements( ) 함수
 이다. QWebView 위젯은 웹 페이지 로딩이 완료될 때 자동으로 구성된다. examineChildElements( ) 함
 수는 QTreeWidget에 아이템을 추가하고 Document 구조를 탐색할 수 있도록 기능을 제공한다．


 0Window 클래스 구현
 Window 클래스의 생성자에서 setupUi( ) 함수를 window.ui 파일에서 정의한 GUI를 설정한다．

   Window: :Window ( QWidget *parent)
       : QMainWindow (parent)
     {
             se七upUi (thi引 ;




                                                                                              2 QtWebKit 389


===== PAGE 391 =====
 웹 페이지가 로딩될 때 , 0皿w的View_loadFinished( ) 슬롯함수가 호출된다. 여기서 Tree 위젯을
 Clear하고 웹 페이지의 메인 Fran始으로부터 Document Elem아此를 얻기 위해 Document를 검사하기
시작한다．

    void Window: :on webView loadFinished()
    {
         treeWidget->clear () ;


        QWebFrarne *frame = webView_>page ( _>mainFrame ( );
        QWebElement document = frame->documentElemerit () ;
        examineChildElements (document, treeWidget->invisibleRootltem() );




Docume砒를 검색하기 위해 examineChildElements( ) 함수를 호출하는 시점에서 Elem이此의 첫 번
째 Eleme玭를 firstChild( ) 함수를 사용해 얻어온다. 얻어온 첫 번째 Elem이此의 Child Element를 검
사하기 시작한다. 유효한（Null이 아닌 Element) Element를 얻어오기 위해 isNull( ) 함수를 사용한다．
QTreeWidgetltem 인스턴스를 생성하고 Parent 아이템을 여기에 추가한다．

 void Window: :examineChildElements (const QWebElement &parentElement,
                                     QTreeWidgetltem 枉沮ren七I七em)

        QWebElement element = parentElement. firstChild () ;
        while (! elemerit.isNull () ) {


            QTreeWidgetltem * item = new QTreeWidgetltem() ;
            item->setText (0, element. tagName (fl;
            parentltem->addChild(item) ;


            examineChildElements (elernent, item) ;
            element = element.nextSibling() ;
        }



여기서 새로 생성한 아이템과 현재 Elem이此를 등록하기 위해 examine（걋iildElements( ) 함수를 재퀴
적으로 호출해1 각 Eleme玭를 Child Element로 등록한다. Document 내에서 Child Element인지 같
은 레벨의 다음 Element인지 구분하기 위해 nextSibling( ) 함수를 사용한다．

재퀴적 호출을 사용하는 방법은 트리 위젯에 Document 구조를 단순하게 표시할 수 있도록 해준다. 예
제의 main( ) 함수에서 Document URL을 설정하기 위해 setUrl( ) 함수를 호출한다．

void Window: :seturl (const QUrl &url)
{
        webView->setUrl (url) ;




390 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 392 =====
                   QtWebK什 모듈 환경에서 JQue四 활용

이번 장에서는 QtWebkit 모듈을 사용해 Effect와 콘텐츠 조작 기능이 추가된 웹 브라우저 상에서
JQuery를 사용하는 방법에 대해 알아보도록 하자．

'可Qt牲자커뮤니티                                                               山四畔놔］
 V昭w     Effect   1的뇹

              『d口h口口board=
  0 4) 0 C. 'b口크      kkkmairlcoEarn］
                                    口b=sk.iri_ir＼日tOe:尸 h＝：帥board} _horne

 目            Qt 개발자 커뮤니티
                                     http叭心ww.qt-始VJ沁m

       HIME               클래스            나문로드            커뮤L卄크        비즈니스

       t化me       곤지사뷸F          주 . 뉴스 ; 뉴스기 El       C 실견 프로그d =-

 4 I                       1ri                     I


（그림） 예제 실행 화면



그림에서 보는 것과 같이 JQuery JavaScrij亢 코드를 사용하기 위해 QWebFrame 클래스에서 제공하
는 evaluateJavaScript( ) 멤버함수를 사용하였다. 이 함수는 Frame상에서 사용할 자바스크립트를 인
자로 지정한다．

끄otj코발자켜뮤니El                                                「     「 「        口 回mm
 View     杆ect     To놔S

  Q 0 0 () 'bcard.php先oardrkkkmair1&
                                  comrnand=skiri_irisert&exe늬ns日rt_
                                                                iboardI_home

  '日；荏筐"뇨루肛lb田                                                                  :
       He卜IE              클켜스            L卄， 나 =         커뮤니El        버즈니스

       Ho汗尼       곤지사함           주요뉴스 & 뉴스레El          01 솰전 프로그래！-

 { !


（그림） Effe아의 Turn image u口side down 기능을 실행한 화면



파일 메뉴에서 \／扼w는 렌더링한 웹 페이지 소스의 \[jew 기능을 제공한다. Effect 메뉴는 웹 페이지 상
에서 링크 Tag의 I七ghlight 기능과 이미지를 반대로 회전시키는 기능을 제공한다．

To아S 메뉴는 웹 페이지 상에서 GIF 이미지 , inline frame, object element, embedded element를
제거하는 기능을 제공한다．


0M졔nWindow 클래낱느 정의
MainWindow 클래스는 QMainWindow 클래스를 상속받았으며 어플리케이션과 웹 콘텐츠 상에서 동
작시키기 위한 이벤트 시그널을 처리하기 위한 슬롯이 구현되어 있다．



                                                                                     2 （거WebK作 391


===== PAGE 393 =====
 class MainWindow : public QMainWindow
     {
    Q OBJECT
 public:
         MainWindow (const QUrl& url) ;

 pro七ec七ed slots:
         void adjustLocation() ;
         void changeLocation() ;
         void adjustTitle () ;
         void setProgress (int p) ;
         void firiishLoading(bool) ;


         void viewSource () ;
         void slotSourceDownloaded() ;


         void highlightAllLinks () ;
         void rotatelmages (bool invert) ;
         void removeGif Images ( ) ;
         void removelnlineFrames () ;
         void removeObjectElements () ;
         void removeEmbeddedElements () ;

 private:
         QString jQuery;
         QWebView * view;
         QLineEdit *locationEdit.
         QAction 士ro七ateAc七ion;
         mnt progress;




jQuery QString 타입의 변수에 jQuery 콘텐츠를 지정한다. 웹 콘텐츠를 디스플레이하기 위해 印Veb
View 클래스를 사용하고, 웹 주소를 조작하고 표시하기 위해 QLineEdit 위젯을 사용하였다．


0 M톄nWindow 클래스 구현
八4ainWindow 클래스의 생성자는 jQuery의 저장된 파일로부터 읽어와 QString 타입의 변수에 저장
한다．

MainWindow: :MainWindow (const QUrl& unl)
 {
         progress = 0;


         QFile file;
         file. setFileName ( " :!jquery.min. js ' ) ;
         file. open(QloDevice: :ReadOnly) ;
         jQuery = file. readAllU;
         file. close() ;




392 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 394 =====
생성자의 첫 번째 라인의 progress는 0의 값을 할당한다. 이 변수는 웹 페이지의 로딩 진행상황을 피센
트로 사용자에게 보여주기 위한 변수이다. 다음으로 파일로부터 jQuery 콘텐츠를 읽어와 QString 변수
에 저장한다. jQuery 라이브러리는 웹 페이지상의 HTML을 조작하기 위해 사용한다．

   vie'寸 = new QWebVie叫七hi引 ;
   view->load(url) ;
   connect (view, SIGNAL (1oadFinished(boo1) ), SLOT (adjustLocation() fl ;
   connect (view, SIGNAL(titleChanged(QString) ), SLOT (adjustTitle (fl) ;
   connect (view, SIGNAL (loadProgress (int) ), SLOT (setProgress (int) fl ;
   connect (view, SIGNPL (loadFinished(bool) ), SLOT (finishLoading(bool) fl ;


   locationEdit = new QLineEdit (this) ;
   locationEdit->setSizePolicy(QSizePoticy: :Expanding,
                                 locationEdit->sizePolicy() .verticalPolicy (fl;
   connect (locationEdit, SIGNAL (returnPressed() ), SLOT (changeLocation() ));


   QToolBar *toolBar = addToolBar (tr ( "Navigation") );
   toolBar->addAction (view->pageAction ( QWebPage: : Back) );
   toolBar->addAction ( view->pageAction ( QWebPage: : Forward) );
   toolBar->addAction(view->pageAction(QWebPage: :Reloadfl;
   toolBar->addAction (view->pageAction ( QwebPage: : Stop) );
   toolBar->addwidget ( locationEdit) ;



帥?VebView 오브젝트를 생성하고 View에서 발생한 시그널을 처리하기 위해 connect( ) 함수를 사용해
슬롯함수와 연결한다. 그리고 웹 브라우저에서 사용할 주소 Bar를 위한 QLineEdit 위젯을 생성한다. 동
시에 웹 브라우저를 활용 가능한 영역을 채우기 위해 Horizontal QSizePolicy를 설정한다. QToolBar
어］ 주소 입력 위젯을 추가하고 배치된 버튼의 Action을 지정한다．

                                                                n
   QMenu *effec七Nenu = menuBar ( )->addNenu(tr ( "&Effec            ));
   effectMenu->addAction ( "Highlight all    links ",
                                                      七his, SL(刃（highligh七Al珏ink引 ) ) ) ;
   rotateAction = nei寸 QActio미七hi引 ;
   rotateAction->setlcon (style ( ) ->standardlcon
                                       (QStyle: :SP尸FileDialogDetailedView) );
   rotateAction->setCheckable (true) ;
   rotateAction->setText (tr ( "Turn images upside down") );
   connect (rotateAction, SIGNAL(toggled(bool) ),
                                             this,    SLOT (rotatelmages (bool) ));
   effectMenu->addAction ( rotateAction) ;
   QMenu *toolsMenu = menuBar ( )->ad沁enu(tr ( "&Tools ") );
   toolsMenu->addAction(tr ( "Remove GIF images ") ,
                                             this,    SLOT (removeGiflmages () ));
   toolsNenu->addAction(tr ( "Remove all     inline     frames ") ,
                                             this,    SLOT ( removelnlineFrames () ));
   toolsMenu->addAction(tr ( "Remove all     object elements ") ,
                                             this,    SLOT (removeObjectElements () ));
   toolsMenu->addAction(tr ( "Remove all     embedded elements ") ,



                                                                                      2 QtWebKit 393


===== PAGE 395 =====
                                                this, SLOT (removeEmbeddedElements () ));
             setcentraiwidget (view) ;
             setunifiedTitleAndToolBaronMac (true) ;
        }


    effectMenu와 toolsM帥U어］ 대한 구현 부분이다. 두 개의 QM이m의 Action을 처리할 슬롯함수를 지
정하고 帥/lainWindow의 중앙에 邸WebView 위젯을 배치한다．

    void MainWindow: :adjustLocation()
    {
            locationEdit->setText (view->url( ) .toString( ));
    }

    void MainWindow: :changeLocation()
    {
            QUrl unl = QUrl: : fromUsenlnput (locationEdit->text (fl;
            view->load(url) ;
            view->setFocus () ;
    }
L



웹 페이지가 로딩될 때 주소 입력 위젯을 업데이트하고, 帥WebView에서 웹 페이지 로딩이 완료되면
loadFinished( ) 시그널 이벤트가 발생하며 이 시그널과 연결된 adjustLocation( ) 슬롯함수가 호출된
다. adjustLocation( ) 슬롯함수는 Address Bar의 주소를 업데이트한다．

    void MainWindow: :adjustTitle()
    {
            if (progress <= 0 I I progress >= 100)
                 setWindowTitle (view->title () );
            else
                 setWindowTitle (QString( "%l   (%2% )")
                                                .arg(view->title ( ) ) .arg(progress) );
    }

    void MainWindow: :setProgress (int p)
    {
            progress = P;
            adjustTitle () ;
    }


adjustTitle( ) 슬롯함수는 로딩되는 진행 상황을 퍼센트로 환산해1 윈도우 타이틀 영역에 출력한다. 이
슬롯은 邸WebView의 titleChanged( ) 시그널에 의해 호출된다．




394 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 396 =====
void MainWindow: :finishLoading(bool)
{
     progress = 100;
     ad j us七Tj土le ( ) ;
     view->page ( )->mainFraxne ( )->evaluatejavaScript (jQuery) ;


     rotatelmages (rotateAction->isChecked () );
}


웹 페이지 로딩이 완료되면 loadFinished( ) 시그널 이벤트가 발생하며 finishLoading( ) 슬롯함수를
호출한다. 이 슬롯함수는 웹 페이지 로딩 진행상황을 퍼센트로 환산해1 윈도우 제목 영역을 표시한다. 웹
페이지 로딩 진행 상황을 업데이트 하고 JQuery 라이브러리를 사용하기 위해 evaluateJavaScript()
함수를 호출한다．

JQuery 라이브러리는 邸VebView에 Rendering된 웹 페이지의 콘텐츠를 조작하기 위해 사용한다．
rotatelmages( ) 함수가 호출되면 새로 로딩된 페이지상에 이미지 Toggle action 상태를 확인하기 위
해 호출한다．

void MainWindow: :highlightAllLinks ()
{
     OString code = "$ ( 'a' ) .each ( function ()
                  { $(this) .css ( 1background-color ' , 'yellow ' ) } ); undefined";
     view->page ( ) ->mainFraine ( ) ->evaluateJavaScript (code) ;
}


highlightAllLinks( ）는 jQuery 기반 함수이다. 현재 웹 페이지의 링크를 역상（H培hlight) 시킨다. 각
Elem아此의 Hyperlink된 Tag 이름을 검색하며 css를 사용해 Yellow 컬러로 Background를 설정한다．


void MainWindow: : rotatelmages (bool invert)
{
     QString code;
     if (invert)
         code = "$ ( 'img' ).each ( function () {
                   $ (thi引 .css ( '- webkit十七r帥sj土的n' , '- webki七m七ransform 2可 ) ;
                   $(this) .css ( ' -webkit-transform' , 'rotate (lBOdeg) ' ) } );
                   undefined";
     else
         code = "$ ( 'img' ).each( function () {
                  $(this) .css ( ' -webkit-transition' , , -webkit-transform 2s ' ) ;
                  $(this) .css ( ' -webkit-transform' , 'rotate (odeg) ' ) } );
                  undefined";


     view->page ( ) ->mainFrame ( ) ->evaluateJavaScript (code) ;
 }




                                                                                   2 QtWebKit 395


===== PAGE 397 =====
rotatelmage( ) 함수는 현재 웹 페이지에 로딩된 이미지를 회전시킨다. Webi（此은 CSS transforms를
지원하며 JavaScript 코드는 웹 페이지에 로딩된 이미지를 찾아 180도 회전시킨다．

void MainWindow: :removeGiflmages ()
{
     QString code = t'$ ( 1 [src*=gif] ' ).removeO ";
     view->page ( ) ->mainFr帥e ( ) ->evaluateJavaScript (code) ;
}

void MainWindow: :removelnhineFrames ( )
{
     QString code = '$ ( 'iframe ' ) .removeU ' ;
     view->page ( ) ->mainFraine ( ) ->evaiuateJavaScript (code) ;
}

void MainWindow: :removeobjectEiements ( )
 {
     QString code = "$ ( 'object ' ) .remove ( ) ";
     view->page ( ) ->inainFrame ( ) ->evaiuateJavaScript (code) ;
}

void MainWindow: :removeEmbeddedElernents ( )
 {
     QString code = "$ ( 'embed' ) .removeU ' ;
     view->page ( ) ->rnainFrame ( ) ->evaluateJavaScript (code) ;
 }


removeGiflmages( ) 함수는 JQuery 라이브러리를 이용해 웹 페이지에 로딩된 GIF 포맷의 이미지 파
일을 졔거한다. removelnlineFrames( ）는 웹 페이지상어］ inline frame을 제거한다．

removeObjectElements(), removeEmbeddedElements( ) 함수도 동일한 방법을 사용해 웹 페이지
의 object elements와 plugins embedded elements를 제거한다．



            0싸VebKit과 00히ect 卜／odel 간의 Bridge

QtWebKit 모듈은 QObject와 같은 c++ 기반의 Nat如e Object 간의 접근을 위해 \VebK抗의 Java
Script를 확장한 메커니즘을 제공한다. 즉 웹 페이지의 DOM 객체를 통해 QObject와 통신이 가능하다．

예를 들어 JavaScript를 발생한 이벤트를 처리하기 위해 C+＋로 작성된 슬롯함수를 완결할 수 있다. 이
러한 매커니즘은 QtWebKit 모듈에서 동작하는 웹 페이지의 Elemei此와 연결할 수 있다. 따라서 시스템
레벨의 미들웨어 소프트웨어와 통신을 쉽게 할 수 있다．

0Native 어플리케이션에서의 웹 콘텐츠
예를 들어 Qt를 사용해 Music Player와 같은 전통적으로 응용 어플리케이션을 구현한다고 가정하자．
소프트웨어 디자인 패턴을 적용해 어플리케이션을 구현할 때 미디어를 플레이하고 사용자 인터페이스를


396 CHAPTER 12_ 뎨이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 398 =====
제공하는 모듈, 플레이 리스트 제공 모듈, 음악 파일이 저장된 스토어 관리 모듈로 분리해 응용 어플리케
이션을 설계하고 구현한다．

어플리케이션의 사용자 인터페이스를 제공하는 모듈을 구현할 때 Qt에서 제공하는 邸Widget과 같은
Native 위젯을 사용하거나 Graphics View 파'amework를 사용한다. 그리고 QtDeclarative 모듈과
같은 QML(QtQuick）을 사용해 사용자 인터페이스를 구현할 수도 있다. 또 다른 방법으로 Qt에서 제공
하는 QtWebKit 모듈을 사용해 GI끄를 구현할 수도 있다．

QtWebKit 모듈을 사용하면 HTML, HTML5, JavaScrii亢, Css를 사용해 GUI를 구현할 수 있다. 플
레이 리스트 모듈을 구현하기 위해 플랫폼어］ 존재하는 파일 시스템에 접근해야 한다．
따라서 QtWebKit 상에서 동작하는 HTML5와 시스템 레벨에서 동작하는 Native 모듈 간의 통신이 필
요하다．


 SQO히e아의 접근
기본적으로 보안상의 이유 때문어］ 웹 환경을 통해1QObject어］ 접근할 수 없다. 웹 기반의 응용 어플리케
이션이 QObject어］ 접근해야 한다면 다음과 같은 방법을 사용해 QObject 접근 권한을 획득할 수 있다．


j '台굶：뇨恤帥n叫*的Pa叩－汕鈿如）;
1   rame- >aclctToJavabcrlptWlnclowubJect   (   soIreN帥e"orMyOtJJect   ,   myOo eCt) ;




. 시그널과 슬롯을 사용한 Bridge
QtWebK比과 QObject 간의 통신을 위한 방법으로 시그널과 슬롯을 사용한다. 시그널과 슬롯을 연결하
는 방법은 다음과 같이 3가지 형태로 분류된다．
     · Hybrid C++ 슬롯과 스크립트
      C++ 어플리케이션 소스 코드는 스크립트 함수에 시그널을 연결할 수 있다. 이 접근 방법은
      QObject를 사용할 경우 유용하지만 스크립트 환경에서 오브젝트가 노출되지 않는다. 단지 C+＋어］
      서 이벤트가 발생하면 스크립트에서 응답 처리만 가능한 방식이다. 어플리케이션 측면에서 C＋十 시
      그널과 JavaScr巾t 슬롯 연결만 가능하다.
     · Hybrid 스크립트와 C++
      스크립트는 스크립트 환경어］ 접근할 수 있는 미리 정의된 어플리케이션 오브젝트어］ 시그널과 슬롯
      을 연결할 수 있다. 하지만 이러한 방법도 슬롯은 C+＋에서만 작성할 수 있다．
     · 완전한 스크립트 방식
       스크립트 시그널 Handler 함수는 스크립트로 작성된 슬롯과 연결이 가능하다. 예를 들어 스크립트
      는 QLineEdit::returnPressed( ) 시그널을 조작할 수 있으며 스크립트 함수에 발생한 시그널 이
      벤트를 연결할 수 있다．




                                                                                         2꾜tWebKit 397


===== PAGE 399 =====
   Funct山n에 시그널 연결

 function mylnterestingScriptFunction() { . . . }


 myQObject. somethingChanged.connect (myInterestingScriptFunction) ;



somethingChanged 시그널과 mylnterestingScriptFunction 슬롯은 connection( ) 함수를 사용해
시그널과 슬롯을 연결할 수 있다. somethingChanged 시그널 이벤트가 발생하면 자동으로 mylnteres
-tingScriptFunction 슬롯이 호출된다. Connect( ) 함수의 인자는 JavaScript 함수와 QOb把ct의 슬
롯을 사용할 수 있다．

 myQObj察拉. somethingChanged . connect (myOtherQObject . doSomething) ;


시그널과 슬롯의 연결을 해제하기 위해 시그널의 disconnect( ) 함수를 호출한다. 이 함수의 인자는 슬롯
을 지정한다．

 myQObject. somethingChanged.disconnect (mylnterestingFunction) ;
 myQobj ec七 . some七hingChanged.disconne（北 (myO七herQObjec七.doS帥e七hing) ;




  멤버함수에 시그널 연결

 myQObject. somethingChanged.connect (thisObject, function)



connect( ) 함수 호출은 somethingChanged 시그널과 슬롯 함수를 연결한다. 오브젝트인 my아)ject
는 somethingChanged 시그널을 발생시키고 thisObject의 슬롯 function은 예제에서 설명했던 것과
같이 자동으로 호출된다．

만약 GUI Form상에 myBut切n이 존재한다고 가정할 때1 이 버튼의 clicked 시그널에 응답하도록 처리
해야 한다. connect( ) 함수는 버튼이 clicked 시그널 이벤트를 처리하도록 처리할 수 있다. 다음 예제는
on（그licked( ) 슬롯함수는 GUI Form의 x좌표 값을 출력한다．

var form = { x: 123 };
var onClicked = function() { print (this. x) ; };
myButton.clicked.connect (form, onClicked) ;



시그널로부터 슬롯의 연결을 해제하기 위해써 connect( ) 함수 인자로 사용했던 인자를 disconnect( )
함수에 같은 인자를 사용한다．

myQObject. somethingChanged . disconnect (thisObject, function) ;




398 CHAPTER 12= 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 400 =====
I 정해진 이름의 멤버함수에 시그널 연결

myQObject. somethingChanged.connect (thisobject, "functionName")



함수 functionName은 시그널 something（그hanged어］ 응답할 때 여기 속한 thisObject 인자는 첫 번
째 인자로 설정한다. 두 번째 인자 functionName은 시그널에 연결된 함수 이름을 지정한다. 이러한 방
법은 오브젝트의 멤버함수를 참조한다．

var obj = { x: 123, fun: function() { print (this. x) ; } };
myQObject. somethingChanged.connect (objr'fun1' ) ;



시그널과 연결을 해제하기 위해 connect( ) 함수에서 사용했던 같은 인자를 사용한다．
myQObject. somethingChanged. disconnect(thisObject, "functionName");


I 에러 핸들링
connect( ) 혹은 disconnect( ) 함수가 수행될 때 undefined가 발생하는 상황에서 스크립트 예외 처리
를 통해 발생하는 오브젝트를 리턴하도록 다음과 같이 예외 처리할 수 있다．

try {
    myQObject. somethingChanged.connect (myQObject, "slotThatDoesntExist ") ;
 }
Ca七（샀1 (e)
 {
     print (e) ;
 }


I 스크립트에서 시그널 발생
스크립트 코드로부터 시그널을 발생시키기 위해 시그널 함수를 관련된 인자를 지정하여 시그널을 발생시
킬 수 있다．

myQObject. somethingChanged( "hello") ;



I 시그널 슬롯의 다양성（
             （加erload)
Overload된 시그널과 슬롯을 지원하기 위해 QtWebkit 모듈의 Bridge는 호출되는 QSscriptValue 인
자의 타입을 기반으로 Overload된 함수를 지원한다. 예를 들어 I好OverloadeSlot(int）과 myOver
loadedSlot(QString) 함수와 같이 Overload된 함수를 사용할 수 있다．

myQObject.myOverloadedSlot (l0) ;     7/ wail call the mnt overload
myQObject.myOverloadedSlot ( "l0 ") ; 7/ will call the QString overload



만약 프로퍼티 이름과 같이 C十＋ 함수의 정규화 방식의 시그너처를 접근할 수 있는 방법을 제공한다．


                                                                                2 QlWebKiI 399


===== PAGE 401 =====
 myQobjec七［' myOverloadedSlo七（mnt) 1 J (t 10 ") ;     // 인자를 mnt 타입으로변환
 myQObj ec七［' myOverloadedSlot (QString) 1 ] (10) ;   // 인자를 S七ring 타입으로 변환



 小 Invokable 메소드
기본척으로 스크립트로부터 시그널과 슬롯을 호출할 수 있다. 또한 스크립트부터 호출할 메소드가 시그
널과 슬롯이 아니더라도 메소드를 호출하도록 정의할 수 있다. Invokable 메소드로 정의하기 위해 다음
과 같이 리턴 타입으로 QJNVOKABLE 매크로를 지정해야 한다．

 class MyObject : public QObject
 {
         O OBJECT


 public:
         Q I卜VOKABLE void thisMethodlslnvokablelnJavaScript () ;
         void thisMethodlsNotlnvokable工nJavaScript ( ) ;



     ;



Q(北昶ct의 프로퍼티는 JavaScrij亢 오브젝트와 일치하는 프로피티를 활용할 수 있다. 스크립트 코드어］
서 프로퍼티를 조작하기 위해 프로퍼티를 위한 C+＋의 get/set 메소드는 자동으로 호출한다. 다음 예제
는 C++ 클래스에서 프로퍼티를 다음과 같이 사용한다．

 QPROPERTY(bool enabled R且AD enabled WRITE setEnabled)



다음 예제는 스크립트 코드에서 사용하는 예이다．

myQObject.enabled = true;


myQObject. enabled = !myQObject .enabled;



QObject의 child 오브젝트는 JavaScript 래퍼（wrapper) 오브젝트의 프로퍼티와 같이 활용할 수 있다．
예를 들어 QDialog상어］ "okButton" child 오브젝트가 있다면 다음과 같이 스크립트 코드에서 오브젝트
를 접근할 수 있다．

myDialog.okButton



스크립트 코드에서 오브젝트의 이름을 다음과 같이 변경하는 것이 가능하다．

myDialog. okButton
myDialog. okautton.objectName = "cancelButton";
// from now on, myDialog.cancelButton references the button




400 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 402 =====
0 데이터 타입
슬롯을 호출할 때 시그널 혹은 슬롯을 받기 위해 일반적으로 사용하는 데이터 타입을 고려해야 한다．
QWebKit Bridge는 JavaScrii亢의 데이터 타입과 Qt 타입의 데이터 타입을 변환할 수 있는 기능이 포
함되어 있다. 따라서 데이터 타입을 일치하기 위해 Qt의 톄이터 타입과 JavaScript의 사용 가능 데이터
타입을 일치하도록 코드상에서 정의해야 한다．

모든 Qt의 Number 타입은 JavaScrij凡 number 타입으로 일치하도록 타입을 지정해야 한다. int,
short, float, double과 Qt에서 정의한 타입（qreal, qint 등）이 포함하도록 일치시켜야 한다. 특별하게
QtWebKit 상에서 Unicode 값을 사용한다. 이때 특별하게 QChar을 슬롯으로 지정해야 한다．

JavaScript 코드가 QStrir乷과 대응하는 메소드 혹은 프로퍼티를 접근할 때 QtWebKit bridge는 자동
으로 값을 string 값으로 변환한다. JavaScript Date 오브젝트를 변환하기 위해 QData, QTime 그리
고 QDateTime으로 데이터 변환 작업이 자동으로 이루어진다．

QtWebKit은 JavaScrij元에서 사용한 정규표현（RegExp) 오브젝트를 QRegExp로 변경한다．

QtWebKit bridge는 특별한 방법으로 리스트 타입의 변환 작업을 처리한다. QVariantList, QString
List, QObjectList 그리고 QList와 같은 리스트 타입을 변환하기 위해I JavaScri1亢의 Array 타입으로
변환한다．

JavaScript는 JSON 오브젝트와 같은 혼합 형태 데이터 타입을 사용한다. Key와 Value가 쌍으로 존재
하는 타입을 지정하기 위해 QtWebKit 모듈은 QVariai此Map으로 변환한다．

QtWebKit bridge는 특별한 방법을 사용해 QPixmap과 Qlmage를 조작할 수 있다. QtWebK此은
HTML 이미지로 QPixmap을 저장하고 QPixmap은 WebKit 내부에서 바로 사용할 수 있다. 따라서
Qlmage와 QPixmap은 JavaScrij亢 오브젝트로 변경할 수 있다．


c++ 예저1 코드

class MyObject : QObject {
          Q OBJECT
          Q PROPERTY (QPixmap myPixmap READ getPixmap)


public:
          QPixmap getPi刃nap() const;
 };
／士    .   .   .   士／/


MyObject myObject;
myWebPage .mainFrame ( )->acIdToJavaScriptVindowObject ( "rnyObject ",   &myObject) ;




                                                                                    2 0t小／ebK什 401


===== PAGE 403 =====
HTM匕 예제 코드

 <h七ml>
          <head>
                 <script>
                              function loadlmage()
                              {
                                  myObject .myPixmap . assignToHTMLlmageElement (document.
                                                                  getElementByld( "imageElement ") );
                                  var context =
                                     document.getElementByld( "canvasElement " ) .getContext ( "2d") ;
                                     con七ex七 . Pu七ImageDa七a (myObject .myPixmap 比olmageDa七a ( ) ) ;
                              }
                 </script>
     </head>
     <body onload= "loadlmage () ">
         <img id=" imageElement " width=" 300 " height=" 200 " I>
         <canvas id="canvasElement " width=" 300 " height=" 200 " I>
     <Ibody>
 </html>



시그널과 슬롯은 프로피티를 사용해 邸VebE1ement 리턴 타입으로 리턴할 수 있으며, 반대로 Java
Script에서 야WebKit bridge의 타입으로 리턴할 수 있다. JavaScript 환경에서는 D0M Elemer此를 선
택하고 QWebElement 타입으로 다음과 같은 예제와 같이 전달할 수 있다．

0++ 예제 코드

 class MyObject : QObject {
         Q OBJECT
     public Q_SLOTS:
                 void doSomethingWithWebElement (const QWebElement& );
     };
    ／出       .   .   .   火／
    MyObject myObject;
    myWebPage.mainFrame ( )->addToJavaScriptWindo的bject ( "myObject ", &rnyObject) ;




HTML 예제 코드

<html>
          <head>
                     <script>
                              function runExample () {
                                 myObject . doSomethingWithWebElement (
                                                  document. getElementByld( "someEleinent ") );
                              }
             </script>
          </head>
          <body onload= " runExample ( )">                                                               O

402 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 404 =====
              <span id=' someElement " >Text< /span>
     </body>
</html>




    ; 2.5 Hybrid 클라이언트 어플리케이션 예저1
이전 장에서 QtWebKit 모듈에서 동작하는 웹 환경의 JavaScript와 Qt Native 오브젝트（QObj吼t) 간
의 이벤트와 데이터 간의 전달을 위한 QtWebKit Bridge 사용 방법에 대해 알아보았다．

이번 장에서는 QtWebKit 상에서 동작하는 웹 페이지와 C)++ 기반의 어플리케이션간 Bridge를 활용한
예제를 통해 실제 사용하는 방법에 대해 알아보도록 하자. 이 예제 소스 코드는 Qt를 설치하면 기본적으
로 제공하는 QtWebKit 어플리케이션 예제이다．

다음 그림에서 보는 것과 같이 오른쪽 상단의 빈 리스트 항목이 있다. 이 리스트 항목은 아래의 이미지를
클릭하면 이 리스트 항목에 등록된다．


                Image Analyzer
                                                    hnage5 m 뇨an小工ed:

                      Ssafl,S: Idle


                     L1te1t 1tE5n1n:
                        1ttd n a
                       Gmen: n a
                        1i1口e n/1



     Click on images below to select for analysis




（그림）（그tWebKit Bridge 예제 실행 화면



왼쪽은 각 이미지의 평균 RGB 값을 보여준다. 앞의 예제 실행 화면에서 보는 것과 같이 이미지를 선택했
다면 [Analyze] 버튼을 클릭한다. 이 버튼을 클릭하면 왼쪽 상단에 위치한 이미지어］ 대한 RGB 정보가
출력될 것이다．


                 Image Analyzer
                                                     mv, nIn..*s.d:
                      StaIns, I띠e

                      L1tdt Rt3nlt1:
                      RJ: 5lSI 口n
                      (;r卄1: F490 4自
                       B1ai: 5且（14 q毛



     Click on Images below to select foe analysis


（그림） [Analyze] 버튼 실행 후 이미지에 대한 ROB 정보를 출력한 실행 화면 일부



어플리케이션의 메인 윈도우는 0++ 언어로 정의되어 있다. QNetworkDiskCache와 QWebView를 생
성하고 처음 로딩할 웹 페이지를 帥VebView예게 알려준다．



                                                                        2 QtWebKit 403


===== PAGE 405 =====
 MainWin: :MainWin(QWidget * parent) : QWebView(parent)
     {
          rn_network = new QNetworkAccessManager (this) ;
         in ca（그he = new QNe七workD始kCache (thi引 ;
         mcache->setCacheDirectory (QStandardPaths: :writableLocation(
                               QStandardPaths: :CacheLocation) + "/ irnageanalyzer ' ) ;
         rn_cache->setMaxirnumCacheSize (1000000) ; I/ set the cache to l0rnegs
         rn network->setCache (rncache) ;
         page (卜>setNetworkAccessManager (rn network) ;


         屯analyzer = nes寸 IrnageAnalyzer (in-4（그ache, 七hi引 ;


         II Signal is ernitted before frame loads any web content:
         QObject: :connect (page ( )->mainFrame () ,
                          SIGNAL ( javaScriptWindowObjectCleared() ),
                             this,   SLOT (addJSObject (fl) ;


         QUrl startU之L = QUrl ( 'qrc: /index.htrnl") ;
         setUrl(startURL) ; /7 Load web content now!
 }


이 예제에서 사용한 웹 페이지 샘플은 qrc:/index.html 파일을 URL 주소로 사용하였다. 이 URL은 Qt
resource에 쩌장된 파일이다. 웹 폐이지와 더불어 Qt resource에는 웹 페이지에시 사용한 이미지로 함
께 저장되어 있다．

javaScr印tWindowObjectCleared( ) 시그널과 addJS아玎ect( ) 슬롯을 QObject: :connect( ) 함수를
사용해 연결한다. javaScr印tWindowObjectCleared( ) 시그널 이벤트는 새로운 페이지가 로딩되기 전
에 JavaScript의 윈도우 오브젝트를 초기화한다．

void MainWin: :addJSObject () {
page ( ) ->rnainFr帥e ( ) ->addToJavaScriptwindowObject (
                         QString ( "imageAnalyzer ") , rn_analyzer) ;
 }


ImageAnalyzer 오브젝트가 생성되고 addToJavaScriptWindowObject( ) 함수와 함께 웹 페이지의
mainFrame상에 JavaScript 오브젝트가 추가된다. Index.html 페이지의 (div> 영역에 이미지를 클릭
하면 addlmage( ) 함수가 호출된다．

<div id=irnagediv style=Hclear:both; text- align: center "> <hr/>
    <irng src=" images/rntRainier. jpg' height=150px
                                     onclick=' return addlrnage (this) ; 1 I>
         <irng src=" irnages/bellaCoola . jpg" height=150px
                                     onclick=' return addlmage (this) ;' I>
         <irng src=1! images/ seaShell. jpg11 height=150px
                                      on（그lick=' re七urn addlmage作hi히 ; ' />




404 CHA口TER 12如 데이Ed 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 406 =====
이미지 중 하나를 클릭하면 addlmage( ) 함수가 호출되고 이미지 리스트 항목에 추가한다．

function addlmage(newimg) {
    var imglist = document.getElementByld( 'imglist ' ) ;
    var curChildren = imglist. childNodes;
    var newline = document.createElement ( 'option' ) ;
    newline. innerHTML = newimg. src . substring(newimg. src
                                                       .lastlndexOf ( ' I ' )+l) ;
     newline.value = newimg. src;
     imglist. appendChild (newline) ;




이미지 리스트 항목에 정상적으로 등록되었다면 [Analyze] 버튼을 클릭해 이미지 분석을 시작한다．

<div style="float: right; width: 50%; border-left: solid lpx black ">
    <div id=" listdiv " align="center ">
        <h5>Images to be analyzed:</h5>
        <select multiple size=10 id=imglist style="width: B0% "></select>
          <br I>
          <input type=" button " id=" evalbutton"
                                 value="Analyze" onclick=" analyzelmages () " I>
     </div>
 </div>


[Analyze] 버튼을 클릭하면 analyzelmage( ) 함수가 호출된다．
여가서 이미지 리스트 항목에 등록된 이미지를 ImageAnalyzer 클래스의 startAnalysis( ) 슬롯함수를
호출한다．

 class ImageAnalyzer : public QObject
 {
    Q OBJECT
 public:
      ImageAnalyzer ( QNetworkDiskCache * netcache, QObject * parent=0) ;


      QRgb lastResults () ;
      float lastRed() ;
      float lastGreen() ;
      float lastBlue() ;
      bool isBusy () ;
      QPROPERTY (bool busy R月AD isBusy) ;
      QPROPERTY (float red READ lastRed) ;
      QPROPERTY (float green READ lastGreen) ;
      QPROPERTY (float blue READ lastBiue) ;
      -ImageAnalyzer () ;


 public slots:
    1* ! initiates analysis of all the urls in the list        */
     void startAnalysis (const QStringList & urls) ;



                                                                                     2 아WebK什 405


===== PAGE 407 =====
     signals:
        void finishedAnalysis () ;
        void updateProgress (int completed, mnt total) ;


 priva七e:
 QNetworkAccess14anager* rn_network;
 QNe七workDiskCache出 m ca（그he;
 QStringList rn URLQueue;
 QList<Qlmage> mmimageQueue;
 m1lt mmoutstandingFetches;
 QFutureWatcher<QRgb> * rn_watcher;



대부분의 멤버가 클래스 생성자에서 설정된다．




connectSlots( ) 함수는 JavaScript 함수에 imageAnalyzer 오브젝트 시그널을 연결하기 위한 함수이
다. c++ 측면에서 진행상황을 확인하기 위해 사용된다．

startAnalysis( ) 함수는 public 슬롯함수이다. 이 함수는 분석할 이미지를 가져오기 위해 호출되는 함
수이다. imageAnalyzer의 QtCondurrent 처리 Queue어］ URL 목록을 가져온다．

 void ImageAnalyzer: :startAnalysis (const QStringList & urls)
 {
       in URLQueue = urls;
        fetchURLsO;
 }




406 CHAPTER 12_ 데이터 커뮤니케0 L크과 인터넷 프로그래밍


===== PAGE 408 =====
01 5 Programming



          3 Inter-Process Communication

          프로세스 혹은 어플리케이션간 데이터 통신을 위한 방법으로 'PC를 사용한다. 따라서 아에서 제공하는
          II그C AP를 이용해 프로세스 혹은 어플리케이션간 통신하는 방법에 대해 알아보도록 하자．




IPC(Inter-Process Communication）란 독립된 프로세스 혹은 어플리케이션간 데이터를 교환하기 위
한 통신 방법으로 사용한다. 독립된 프로세스 객체 간의 통신이 가능하다. 예를 들어 운영체제 플랫폼과
연결된 하드웨어 디바이스 및 프로세스 또는 어플리케이션과 통신을 하거나 독립된 프로세스와 어플리케
이션간 통신을 위한 매커니즘을 제공한다．


               다ocess    P幻cess
                                    呼三
                   Inter-Pr以；ess Communic歐to-i in （값
       TCP／下       Shared Mem어y
                                  1 小師帥。口              0Process




（그림） Inter냐가ocess Communication Overview


IPC를 사용하면 완전히 독립된 어플리케이션은 프로세스 간의 영향을 받지 않고 데이터를 교환할 수 있
는 장점이 있다. 또한 IF毛는 어플리케이션상의 내부 프로세스 간의 통신으로 활용할 수 있다. 따라서 내
부 프로세스간과 외부 프로세스간의 통신은 영향을 주지 않는다. IPC에는 두 가지 표준이 있다．
System V 기반의 II毛와 POSIX 기반의 叩C가 있다. System V IP（그 보다 POSIX II毛는 좀더 직관적
인 API 구조로 되어 있어 구현하기 쉬운 장점이 있다．

Qt에서는 II兀를 지원하기 위해 TCP/IP, Shared Memory, 小Bus, QProcess를 제공한다．
QProcess는 Windows CE 플랫폼에서는 지원하지 않는다. 그리고 小Bus는 단지 Un奴와 Linux 플랫
폼에서만 지원한다．




                                                                  3 Inter-Process Communication 407


===== PAGE 409 =====
 0TCP川＞
TCP/IP는 모든 운영체제 플랫폼어］ 상관없이 프로세스간 통신을 위한 방법으로 사용할 수 있으며 QtNet
work 모듈을 사용해 쉽게 구현이 가능하다. 예를 들어 QtNetwork 모듈에서 제공하는 QTcpSocke
                                                                         t,
QTcpServer, QSslSocket, QLocalSocket 등의 클래스를 사용해 I五gh-Level과 Low-Level 단위의
구현이 가능하다．


1Shared Memory
Shared Memory는 모든 플랫폼에서 사용할 수 있으며 Qt에서 제공하는 QShared入4emory 클래스를
사용해 접근할 수 있다. 멀티 쓰레드와 프로세스에 의해 공유 메모리 영역에 접근이 가능하다. 또한 Qt어］
서는 QSystemSemaphore 클래스를 제공한다. 이 클래스는 독립된 프로세스 간의 통신을 위해1 시스템
공유 자원에 접근하기 위한 목적으로 사용한다．

즉, Qt에서 제공하는 QSharedMemory는 어플리케이션과 프로세스가 공유 메모리 영역에 접근하기 위
해 사용되고, QSystemSemaphore는 독립된 프로세스간 시스템 공유 자원에 접근할 때 주로 사용된다．


0D-Bus 아아00이
Qt에서는 小Bus를 사용할 수 있도록 QtDBus 모듈을 사용한다. QtDBus 모듈은 Un奴와 Linux 플랫
폼에서만 사용할 수 있다. Qt에서 제공하는 QtDBus는 시그널 슬롯 매커니즘을 사용한다. 예를 들어 다
른 프로세스와 연결하기 위해 시그널 이벤트가 발생하면 다른 프로세스의 슬롯과 연결된다．


0 아가ocess
QProcess는 Qt에서 제공하는 'P（그 중 하나이다. 자식 프로세스와 같이 외부 어플리케이션이 시작할 때
사용할 수 있다. 그리고 QProcess 클래스는 자식 프로세스를 모니터링하거나 제어하기 위한 목적으로
주로 사용된다. QProcess는 mODevice 클래스로부터 상속받았으며 자식 프로세스의 입출력 채널을 통
해 접근할 수 있다．



          TCP/IP
Qt에서 제공하는 IPC로 TCP/IP를 사용할 수 있다. TCP/IP는 QtNetwork 모듈을 사용해 구현할 수 있
으며 , 어플리케이션 및 프로세스 내부간 통신과 원격에 존재하는 프로세스 간의 통신을 위한 방법으로 유
용하게 사용할 수 있다．

QtNetwork 모듈은 TCP/II) 프로토콜 기반의 클라이언트와 서버 어플리케이션을 작성하는 클래스를 제
공한다. Low 레벨의 네트워크 접근을 위해 QTcpSocket, QTcpServer, QUdpSocket과 같은 클래스를
이용하고 Low 레벨의 네트워크 클래스를 제공한다. 일반적으로 프로토콜을 사용해 네트워크 동작을 수
행하기 위한 QNetworkRequest 클래스, QNetworkReply 클래스, QNetworkAccessManager 클래
스를 제공한다．




408 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 410 =====
'PC를 활용하기 위한 방법으로 TCP/IP는 네트워크 단원에서 소개했던 것과 같이 다양한 클래스를 사용
해 프로세스 내부 및 외부 통신이 가능하다．


0QtNet幻rk 모듈에서 제공하는 클래스

클래스                     설명

OLocalServer            서버 기반의 로컬 소켓을 위한 클라匹

OLocalSocket            로컬 소켓을 지원하기 위한 클래스

ONe棚幻rkAccess卜Aanager   네트워크로부터 데이터를 송／수신 응답 처리를 위한 클래스
QSocket卜幻tifier         네트워크로부터 알림 메시지를 모니터링하기 위한 클래스

OSsI                    모든 네트워크 통신상에 SSL 인증을 사용하기 위한 클래스

Os引Socket               클라이언트와 서버 간의 SSL로 암호화된 소켓 지원 클래스
QTcpServer              TCP 기반 서버 클래스
QTcpSocket              TCP socket
OUdpSocket              UDP socket



Qt에서 제공하는 QtNetwork 모듈은 표에서 보는 것 이외에도 다양한 프로토콜을 지원한다．
QtN毗work 모듈에서 제공하는 클래스어］ 대한 자세한 내용은 네트워크 단원에서 다루었다. Qt에서 제
공하는 네트워크 모듈은 프로세스 내부와 외부에서 접근할 수 있는 방법을 제공한다. 만약 내부 프로세스
간 통신을 위한 방법이라면 QLocalSocket 클래스 사용을 권장한다．



               Shared Memory

Qt에서 제공하는 Shared 八4emory 기반의 IF毛는 QShared八4emory 클래스와 QSystemSemaphore
클래스를 제공한다. QShared八ilemory 클래스는 공유 메모리 영역에 접근할 수 있다. 멀티 쓰레드와 프
로세스에 의해 공유 메모리 영역에 접근이 가눙하다. 또한 Qt에서는 QSystemSemaphore 클래스를 제
공한다. 이 클래스는 독립된 프로세스간의 통신을 위해 시스템 공유 자원에 접근하기 위한 목적으로 사용
한다.


0QSharedMemory 클래스
QShared八4emory 클래스는 공유 메모리 영역에 접근하기 위해 사용한다. 또한 이 클래스는 독점적인
메모리 영역을 사용하기 위한 방법으로 단일 쓰레드 및 프로세스어꺼 사용한다. QShared入4emory 클래
스는 플랫폼마다 다음과 같은 차이점이 있다．




                                                   3 Inter-Process Communication 409


===== PAGE 411 =====
 플랫폼            셜명
 배ndows         윈도우 플랫폼에서 QSharedMemory 클래스는 나누어진 공유 메모리 영역을 소유할
                수 없다. 대신 특정 공유 메모리 영역에 OSharedMemory 클래스를 통해 접근할 수
                있으며 QSharedMemory가 사용하는 메모리 영역을 해제하면 윈도우 커널은 자동으
                로 공유 메모리 영역을 반환한다．
 Unix or 니nux   유닉스 또는 리눅스 플랫폼에서의 QSharedMemor七 특정 공유 메모리 영역 중 사
                용하는 영역을 소유할 수 있다. 하지만 OSharedMemory가 소멸자에 의해 공유 메모
                리를 영역 반환하지 않으면 소유하고 있는 메모리 영역을 자동으로 반환하지 않는다．
 HP-UX          이 플랫폼은 프로세스당 사용할 수 있는 공유 메모리 영역은 하나밖에 접근만 허용한
                다. 따라서 HP寸ux 플랫폼에서 OSharedMemo四 클래스는 멀티 쓰레드0們 사용할
                수 없다．


QShared八4emory 클래스는 공유 메모리 영역을 Read하거나 \Wri扼할 때 lock( ) 멤버함수를 사용해 동
기화가 가능하다. 따라서 lock( ) 함수를 사용할 때 동기화 작업이 완료되면 unlock( ) 함수를 사용해 공
유 메모리 영역의 LOCK을 해제하는 것에 주의해야 한다. Qt에서 제공하는 QtShare心4emory와
QSharedM帥iory는 다르다. 따라서 이를 혼돈해서 사용해서는 안 된다．

QShared入'lemory 클래스는 공유 메모리 영역에 접근하기 위한 방법으로 attach( ) 멤버함수를 사용해
공유 메모리 영역어］ 접근할 수 있다. attach( ) 멤버함수는 공유 메모리 영역에 접근하기 위한 모드를 인
자로 지정할 수 있다. QSharedMemory::ReadOnly 모드를 사용하면 공유 메모리 영역을 읽기 모드로
만 사용할 수 있다. 이와 반대로 QShared八4emory::ReadWrite 모드를 사용하면 읽기와 쓰기 모드 모
두 사용할 수 있다.

QSharedMemory는 프로세스가 소유하고 공유 메모리 영역의 포인터를 반환할 수 있는 멤버함수를 제
공한다. constData( ) 멤버함수를 사용하면 void 타입으로 공유 메모리 영역에서 프로세스가 사용하고
있는 메모리 영역의 포인터를 리턴한다. QSharedMemory 클래스는 공유 생성 시 사용할 공유 메모리
영역을 Byte 크기의 단위로 지정할 수 있다. create( ) 멤버함수를 사용해 사용할 공유 메모리 영역을 바
이트 단위로 할당할 수 있으며 attach( ) 함수에서 제공하는 모드를 두 번째 인자로 지정할 수 있다．

QShared入4emory 클래스에 의해 특정 공유 메모리 영역을 고유한 키를 지정할 수 있다. 공유 메모리 오
브젝트를 위한 키를 지정하기 위한 방식으로 setNativeKey( ) 함수를 사용할 수 있다. 이 함수는 플랫폼
어］ 종속적인 공유 메모리 영역의 키를 사용하는 방법과 동일한 방식으로 키를 지정할 수 있다. 이와 반대
로 setKey( ) 멤버함수를 사용하면 플랫폼의 독립적인 키를 지정할 수 있다. setKey( ) 함수를 사용하면
플랫폼의 종속적 인 Native Key와 Mappir培하는 키를 생성한다.


I QSy없emSemaphore 클래스
QSystemSemaphore 클래스는 일반적인 시스템 세마포어를 제공하기 위한 클래스이다. Semaphore는
八4utex를 사용한다. M毗ex는 단지 한번만 LOCK을 사용할 수 있다. 그러므로 QSemaphore 클래스는
유효한 리소스에 대해 다중 쓰레드를 사용할 수 없다. 따라서 다중 프로세스 혹은 멀티 쓰레드에서는
QSystemSemaphore를 사용해 구현할 수 있다.

QSystemSemaphore은 QSemaphore와 달리 멀티 프로세스가 접근할 수 있다. 즉 QSemaphore어］비


410 CHAPTER 12놔 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 412 =====
해 무겁다. 따라서 하나의 쓰레드 혹은 단일 프로세스를 사용하는 경우라면 QSemaphore 사용하는 것
을 권장한다. acquire( ) 멤버함수는 리소스를 획득할 때까지 미ocking 된다. 그리고 release( ) 함수는
리소스를 해제하기 위한 기능을 제공하며 이 함수는 인자를 지정할 수 있다. 이 함수의 인자는 n>1만큼
리소스를 해제한다．

      QSystemSeinaphore sem( "market ' , 3, QSystemSemaphore: :Create) ;
                                      II resources available =口 3
      sem. acq口ire ( );               II resources available == 2
      sem.ac아lire( );                 II resources available == 1
      sem. acq口ire ( );                                               7/ resources available == 0
      sem.release( );                                                 7/ resources available == 1
      sem.release(2) ;                                                /7 resources available == 3



QSystemSemaphore 클래스를 사용하는 플랫폼어］ 따라 차이점이 있다. 윈도우 플랫폼은 기본 시스템
하위에 포함된 세마포어의 영역을 프로세스가 소유할 수 없다. 이는 특정 키어］ 대한 QSystemSema
phore가 세마포어의 공유 메모리 영역을 파괴하면 멀티 프로세스가 공유하고 있는 영역이 파괴되면 충
돌이 발생하기 때문어］ 윈도우 운영체제가 세모포어를 제거한다．

유닉스나 리눅스의 경우 기본 시스템에 포함된 세마포어 영역을 가질 수 있다. 특정 키를 사용해 QSys-
temSemaphore 클래스의 인스턴스가 소유한 공유 메모리 영역을 제거할 수 있다．


      3.2.1 QSharedMemo四 클래스를 사용한 예제
II毛를 구현하기 위해 QSharedMemory 클래스는 어플리케이션 혹은 두 개의 프로세스 간의 공유 메모
리 영역을 공유할 수 있는 기능을 제공한다. Qt를 설치하면 예제에 포함되어 있는 예제를 통해 Shared
八4emory를 사용하는 방법에 대해 살펴보도록 하자. 다음 그림에서 보는 것과 같이 동일한 예제 어플리케
이션 두 개를 실행한다．


！파SharedMer冊y뇨a什二：                                            b壘m '     i} SharedMero


                                                                궈
]                                                                 !
]{        L,
               ,   ，   小幽，   d rn四a         「，   .』「」*,   ;
                                                                         r『          ad image From File...

                                      '“·
                                                  ·亡Ii昧




      I    Launch two of these dialogs, In the first,                      Launch I'月o of these dialog邕 In the 如St.
      ! press the 拓p bu技on 剖｝dl口ad an image 打oma r                       press the top bu如n and load an image from a
      1 tile, In 出e second, 甘泊客s tIre bo仕om button 1                      川e. In the second, press the bottom button




                                                                 J
      !   and display the loaded image什om shared      r                    and display the loaded Image from shared
                                                                                            memory,



 匕，
      1   1
                        ;       『 "         "「
                             mage From Shared Mem叫
                                                  ‘

                                                                         i    Display Image FromShared Memo口
\                                                                 7



（그림） OSharedMemo四 클래스 예제 실행 화면



그림에서 보는 것과 같이 [Load Imaged 丑rorn File" '] 버튼을 클릭하면 파일 다이얼로그가 호출된다．
파일 다이얼로그에서 예제에 포함된 이미지를 선택하면 다음 그림과 같이 이미지가 예제 중앙에 디스플


                                                                                                                       3 Inter-Process Communication 411


===== PAGE 413 =====
레이 된다．

 刃 SharedMemory Examp旭                  [ g叫
              Load Image From File...                                  Load Image From F加...




                                                                Launch twO of these dialogs. In the 命st,
                                                             press the to口 bu在on 方nd 幻ad an ima恥 ft口ma
                                                              file. In the second, press the bottom button
                                                               and display the loaded image from shared
                                                                                mem아Sr.
                                                                                        』Click
                                                                                   戶
     r   D冶play Image From Shared b佃mor보 1                『r Display Image From Shared Memory
                                                  /


（그림） 이미지 로딩 예제 실행 화면



그림에서 보는 것과 같이 왼쪽 어플리케이션에서 이미지가 로딩된 다음, 오른쪽 실행 예제 화면에서 [Dis
-play Image From Shared 八4emory] 버튼을 클릭하면 왼쪽에서 어플리케이션에의 공유 메모리 영역
을 참조할 수 있다．

 i3 SharedMemcry 三ranr 근                                            Memory 日carr1p地

             Load Image From Frie.,.      』，口 1                        Load Image From File...           !



                                          Sha。
                                                      읔

     r Display Image From SharedMemory 1                        Display Image From Shared Memory
     m＝小尸H如         'H1Hm                      二J

（그림） QSharedMemor/ 클래스를 이용한 메모리 영역 공유



그림에서 보는 것과 같이 오른쪽 어플리케이션상에서 [Display Image From Shared Memory]
                                                                                                             버튼을
클릭하면 공유 메모리 영역에 저장한 이미지를 불러와 이미지를 어플리케이션상에 출력한다．

class Dialog : public QDialog
 {
         Q OBJECT

      public:
         Diaiog(QWidget *parent = 0) ;


     public slots:
         void 如adFro帖lie ( ) ;
         void loadFromMemory 0;

     private :



412 CHAPTER 12H 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 414 =====
       void detach() ;


     private:
       Ui: :Dialog Ui;
       QSharedMemory sharedMemory;
};


                                                  ］버튼을 클릭하면 호출되도록 연결된
loadFromFile( ) 함수는 GUI상에서 [Load Imaged From File"·
슬롯함수이다. 이 함수는 파일 다이얼로그에서 선택한 이미지 데이터를 공유 메모리 영역에 복사한다．
loadFrom玉4emory( ) 함수는 [Display Image From Shared 八ilemory] 버튼이 클릭되면 호출되도록
연결된 슬롯함수이다．

이 슬롯함수는 공유 메모리 영역에 저장된 데이터를 읽어와 GUI상에 이미지로 변환해 출력한다．
Detach( ) 함수는 공유 메모리 영역에 새로운 데이터를 저장하기 이전어］ 호출된다．

void Dialog: : bOa必吐帥File ( )
 {
       if    (sharedMemory.isAttached() )
             detach() ;


       ui. label- >setText (tr ( " Select an image file ") );
       QString fileName = QFileDialog: :getOpenFileName (O, QString() ,
                            QString() , tr ( "Tmages (* .png *.xpm *.jpg) ") );
       Qlmage image;
       if    ( ! image.load(fileName) ) {
              ui . label- >setText (
                  tr ( "Selected file   is not an image, please select another. ") );
              return;
        }
        ui. label- >setPixmap (QPi玎nap: : fromlnlage (image) );



                       ］버튼을 클릭하면 loadFromFile( ) 슬롯함수가 호출된다. isAttached( )
[Load Imaged From File"·
함수는 공유 메모리 영역에 접근할 수 있는지 확인할 수 있는 기능을 제공한다. 공유 메모리 영역에 접근
이 가능하다면 true를 리턴한다. isAttached( ) 함수가 false를 리턴하면 detach( ) 함수를 호출한다．
이 함수는 QShared入[emory 클래스의 detach( ) 멤버함수를 호출한다. 만약 공유 메모리 영역이
LOCK이 설정되어 있으면 LOCK을 해제하고 true를 리턴한다. 만약 LOCK이 설정되어 있지 않거나 다
른 프로세스에 LOCK이 설정되어 있다면 아무런 반응이 일어나지 않고 false를 리턴한다．

        QBuffer buffer;
        buffer. open(QBuffer: :ReadWrite) ;
        QDataStream out (&buffer) ;
        out << image;
        mnt size = buffer. size () ;

        if   ( !sharedMemory. create(size) ) {



                                                                      3_Inter-Process Communication 413


===== PAGE 415 =====
              ui. iabel- >setText (tr ( "tjnable to create shared memory segment. ") );
              re七urn;
         }

         sharedMemory.lock () ;
         char *to = (char* )shared?Iemory.dataU;
         const char *from = buffer. data () .data () ;
         memcpy (to, from, qMin(sharedNemory.size() , size) );
         sharedMemory.uniock () ;
    }


파일로부터 읽어온 이미지 데이터를 QBuffer를 이용해 데이터를 저장한다. QBu玗er에 저장된 데이터를
QDataStream 클래스를 사용해 데이터를 스트림 방식을 사용한다. create( ) 함수는 QSharedMe
mory 클래스의 멤버함수이다．

이 함수를 호출하면 공유 메모리 영역의 포인터 주소만큼 공유 메모리 영역에 복사한다. lock( ）과
unlock( ) 함수는 QSharedMemory 클래스의 멤버함수이다. 이 함수는 동기화를 위해 사용하였다. 동
기화를 통해 공유 메모리 영역은 작업이 완료될 때까지 다른 프로세스가 접근할 수 없다．

 void oialog: :loadFromMemory ( )
    {
        if   (! sharedNemory.attach( )) {
             ui. label->setText (tr ( "unable to attach to shared memory segment. \n"\
                                    "Load an image first. ") );
              return;
        }

        QEuffer buffer;
        QDataStream in (&buffer) ;
        Qlmage image;



loadFromM帥ory( ) 슬롯함수는 다른 프로세스가 공유 메모리 영역에 저장된 데이터를 읽어오기 위한
함수이다. [Display Image From Shared 入4emory] 버튼이 클릭되면 이 함수가 호출되며 공유 메모리
영역에 데이터를 읽어오기 위해 스트림 방식을 사용한다. Qlmage 클래스의 인스턴스는 공유 메모리 영
역에서 읽어온 데이터를 Qlmage에 저장한다．


        sharedNemory.iock ( );
        buffer. setData ( (char* ) sharedNemory.constData (   )r   sharedNemory. size ( ));
        buffer. open(QBuffer: :ReadOnly) ;
        in >> image;
        sharedNemory.uniock ( );


        sharedNemory.detach ( );
        ui. label叫>setPi刃nap (QPixmap: :fromlmage (image) );
}


414 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 416 =====
setData( ) 함수는 QBuffer 클래스의 인스턴스이다. setData( ) 함수의 첫 번째 인자는 공유 메모리 영
역 포인터를 지정한다. 두 번째 인자는 공유 메모리 영역 포인터에서 읽어올 데이터 크기를 바이트 단위
로 지정한다. constData( ) 함수는 QShare曲ilemory 클래스의 멤버함수이다. 이 함수를 호출하면 공유
메모리 영역의 포인터 주소를 반환한다．



          D-Bus Protocol

小Bus는 프로세스간 통신（II兀）및 RPC(Remote Process Call）를 하나의 프로토콜에서 통합된 프로토콜
로 기존의 II兀를 대체할 목적으로 리눅스 및 유닉스 플랫폼에서 사용할 목적으로 개발된 매커니즘이다．
小Bus는 시스템 수준의 프로세스（예를 들어 古H三웨어 디바이스）들과도 통신을 허용하도록 설계되었다．

小Bus는 낮은 지연（Latency）과 오버헤드가 적다. 그렇기 때문어］ 매우 빠르며 같은 시스템 내에서 프로
세스간 통신을 위한 방법으로 적합하다. 小Bus는 현재 freedeskt아）.org 프로젝트에서 정의되었다．

프로세스간 통신을 위한 방법으로 다대다（many的-many) 통신이 가능하도록 설계되었으며 어플리케
이션은 버스를 통해 연결되어 서버와 통신을 한다. 예를 들어 채팅 어플리케이션에서 모든 클라이언트어］
게 메시지를 전달하기 위해 서버로 메시지를 전달하면 서버는 접속한 클라이언트에게 모든 메시지를 전
달하는 것과 같이 小Bus는 동일한 구조로 설계되었다．

또한 小Bus는 두 개의 \Well-known 버스로 정의되어 있다. 두 개의 버스는 시스템 버스（System bus)
와 세션 버스（Sessi아lbus）로 불린다. 시스템 버스는 시스템 프로세스와 데몬들 간의 통신을 위해 사용
되며 임의의 응용 프로그램들이 시스템 버스를 이용하여 시스템 이벤트를 도용（spoof）할 수 없도록 고안
되었다. 세션 버스는 응용 프로그램에서 사용하는 통신을 위한 버스로 주로 사용된다. 세션 버스를 통해
시스템 버스로부터 메시지를 받을 수 있다．


1Service Name
어플리케이션은 버스를 통해 통신을 하기 위해 서비스 네임（Service Name）을 획득한다. 이것은 같은 버
스 상에서 다른 어플리케이션을 구분하기 위해 사용한다. Service Name은 小Bus 버스 데몬어］ 의해 중
계되며 다른 메시지를 라우팅（Routing）한다. 예를 들어 小Bus는 freedesktop. org에 의해 정의되었으
며 서비스 네임을 다음과 같이 사용할 수 있다．

org. freedesktop.DBus



0Object Path
小Bus는 어플리케이션간의 소스와 목적지간 메시지를 주고받는데 사용하는 주소를 Object path라 부
른다. 小Bus를 사용하는 모든 응용 프로그램들에서 메시지들은 특정 어플리케이션에게 전달하지 않고
Object로 전달하거나 전달받는다. 모든 ob把ct는 한 개 이상의 인터페이스를 제공한다． 인터페이스는
入4ethod 이름의 namespace로 사용된다. 단일 object는 여러 Method를 가진다. 또한 Method는 여러
개의 인터페이스를 가진다. Object path는 네트워크 호스트와 같이 다른 어플리케이션에 서비스를 지정


                                              3 IntE玎4가ocess Communi二졔ion 415


===== PAGE 417 =====
할 수 있는 기능을 제공한다. Parent-child의 관꼐와 같이 상하구조（hierarchically）로 되어 있다．


 org. example. QtDBus . PingExample/ pub/ test

                               中                           中
                         Service Name                  （가가ect Path
（그림） Object path



0Interface
Interface는 c+＋에서 추상화 클래스 혹은 자바의 interface 키워드와 비슷하다. 예를 들어 전화를 거는
사람과 받는 사람 사이의 연결을 하기 위해 사용되는 이름으로 사용된다. 인터페이스는 Method의 이름
의 네임스페이스로 사용된다．

Qt에서는 小Bus를 위한 API를 QtDBus 모듈을 통해 제공한다. QtDBus 모듈은 통신을 위한 인터페이
스 시그널과 슬롯을 확장한 매커니즘을 사용한다. D-Bi娼를 통해1 연결된 어플리케이션은 시그널 이벤트
를 발생하면 연결된 슬롯함수가 호출된다. 어플리케이션에서 QtDBus 모듈을 사용하기 위해서는 다음과
같은 헤더 파일을 사용한다．

 孝include <QtDBus>



헤더 파일어］ 추가하고 프로젝트 파일（.pro）어］ QtDBus 라이브러리를 추가해야 한다．




Qt는 D-Bus를 사용하기 위해 다음과 같은 클래스를 제공한다．

                             설명
QDBusAbstractAdaptor         D-Bus 어댑터 베이스 클래스
ODBusAbstractlnterface       D-Bus 인터페이스 베이스 클래스이며 원격 인터페이스에게 접속을 허용하기 위하1 제공되
                             는 클래스
QDBusArgument                클라이언트에서 원격 객체를 호출하71 위해 필요한 모든 정보를 묶어서 전송한다． 이러한 정
                             보를 묶는 것을 Marsh졔ing이라 한다. QDBusArgument는 m카shalt과 demarshall을
                             사용하기 위한 마Bus 인자를 제공하는 클래스이다．
0DBusConnection              D-Bus Daemon（게 연결하기 위해1 사용하는 클래스
QDBusConnecti이기nterf ace     마Bus 버스 Daemon 서비스에 접속하71 위한 클래스
QDBusContext                 마Bus context 호출을 결정하71 위하1 슬롯을 허용하71 위한 클래스
QDBusError                   마Bus 버스와 Rem아e 어플리케이션이 버스상에서 발생한 에러를 표현하71 위해 제공하
                             는 클래스
QDBuslnterface               Rem아e 오브젝트 상에서 인터페이스를 위한 F가oxy
QDBusMessage                 마Bus 버스 상에서 메시치를 송수신하기 위한 클래스
QDBus아가ec卄治卄1 마Bus 타입 시스템에 의해1 제공되는 0히ect path 타입을 식별하기 위하1 사용되는 클래스
0DB니sPendingCall             비동기 호출을 기다리71 위해1 참조하는 클래스
QDBusPendingCa小／Vatcher      비동기 응답을 기다리기 위해1 제공되는 클래스
oDBusPendingReply            비동71 Method 호출에 응답을 포함하는 클래스



416 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 418 =====
 클래스                               설명
 QDBusRe이y                         Rem아e ob忙아에게 Method 호출 응답을 저장하는 클래스
 QDBusServer                       같은 컴퓨터 상에서 프로세스 간의 통신을 위한 Peer나0-Peer 통신을 위한 클래스
 QDBusSer\기ceW計cher                유저가 버스 서비스가 변경되는 것을 감시하기 위해 제공되는 클래스
 QDBusSignature                    D-Bus 타입 시스템에 의하1 제공되는 듸GNATURE 타입을 식별하기 위해 제공되는 클래스
 QDBusUnixFileDescriptor           Unix 파일 Descri아or를 지정하:
                                                         21 위한 클래스
 QDBus Variant                     마Bus 타입 시스템에 의해 제공되는 Variant 타입을 식별하기 위한 클래스



 1Debugging
小Bus를 사용하는 어플리케이션에서 송수신하는 메시지와 관련한 정보를 보는 것은 구현에 있어 때때
로 유용하다. 각 어플리케이션에 小Bus 메시지를 디버깅 목적으로 참조하기 위한 목적으로 QDBUSe
DEBUG 환경 변수를 설정할 수 있다．

Qt를 설치하면 기본적으로 포함된 D-Bus 예제 중어］ D-Bus Remote Controlled Car 예제 어플리케
이션을 다음과 같은 방법으로 D-Bus 메시 지를 디 버깅 할 수 있다．

 examples/dbus /remotecontrolledcar/controller/ controller &
 QDBUS_DEBUG=1 examples/dbus/remotecontrolledcar/car/car &




 3.3.1 F기ng & Pong 마Bus 예제
Ping & Pong 예제는 小Bus를 통해 메시지를 주고받는 예제이다. 네트워크 프로그래밍에서 서버와 클
라이언트가 존재하듯이 Pong 어플리케이션은 Ping 어플리케이션으로부터 요청이 들어오면 메시지를 전
달한다．


F기ng                                    Pong



             Request




                 』 .-,   Request




（그림） F기ng & Pong 메시지 전달 과정



그림에서 보는 것과 같이 Pu名은 POT培에게 요청을 하면 Pong은 Ping에게 응답하는 구조이다. PiT培과
Pang 예제 어플리케이션은 정해진 Service Name과 Object Path를 사용해야 한다．

#de fine SERVICE_NANE                          "org. example.QtDflus . PingExample "



                                                                            3 Inter-Process Communication 417


===== PAGE 419 =====
org. example. QtDBus.PingExan叩le는 Ph培과 Pong 어플리케이션에서 DH＆娼를 이용해 통신을 연
결하기 위한 Service Name으로 설정한다. Object Path는 필수가 아니므로 이 예제에서는 지정하지 않
는다. 다음 예제 코드는 Ping 예제 어플리케이션 소스 코드이다．

QCoreApplication app(argc, argv) ;


if   ( !QDBusConnection: :sessionBus ( ) . isConnected() ) {
      fprintf (stderr, "Cannot connect to the D-Bus session bus. \n"
               "To start it,   run: \n"
               "\ teval ' dbus-launch --auto-syntax '\ n") ;
     return 1;
}

QDBuslnterface iface (SERVICE寸NANE, "I ",           r QDBusConnection: :sessionBus () );
if   (iface. isValid ( )) {
     QDBusReply<QString> reply = iface. call ( "ping", argc > 1 ? argv[ 1] : n 1' ) ;
     if   (reply. isValid ( )) {
          printf ( " Reply was: %s\n", qPrintable(reply. value () ));
          return 0;
      }

      fprintf (stderr, "Call failed:      %s\n", qPrintable (reply. error () .message ( ) ));
     re七l그rn 1;
}

fprintf (stderr, "%s\n",
          qPrintable (QDBusConnection: :sessionBus ( ) .lastError ( ) .inessage () ) );
re七urn 1;




QDBusConnection 클래스는 D-Bus Daemon에 연결을 위한 API를 제공한다. Daemon이란 유닉스 혹
은 리눅스 플랫폼에서 시스템상에서 특정 이벤트를 처리하기 위한 Listener와 같은 개념으로 이해하면 된
다. D-Bus는 System Bus와 Session Bus를 제공한다. System Bus는 시스템 레벨에서 D-Bus 메시지
를 교환하기 위한 통신 매체이고 Session Bus는 어플리케이션간 메시지를 주고받기 위한 매체이다．

상위 어플리케이션 System Bus에 연결이 불가능하며 Session Bus를 통해 시스템 레벨의 매체들과 통
신이 가능하다. 즉 sessionBus( ) 함수는 Session Bus를 Open하기 위해 제공되는 멤버함수이며
isConnected(）는 해당 Bus가 연결이 가능한지 확인하기 위해 제공되는 함수이다．

QDBuslnterface 클래스는 Service Name과 Object Path를 이용해 원격의 오브젝트인 Pong에게 접
근하기 위한 인터페이스를 제공하는 클래스이다. QDBusReply 클래스는 원격의 오브젝트인 Pong에게
메시지를 전달하기 위해 제공되는 클래스이다. Ping 예제 어플리케이션은 GI끄가 포함되지 않는
COMMAND 기반의 어플리케이션이다. 터미널상에 인자로 입력한 문자열을 Pong어꺼 전달한다．
QDBusI之eply 클래스의 call( ) 멤버함수는 인자로 입력한 문자열을 전달하기 위한 멤버함수이다. 다음은
Pong 예제 어플리케이션의 소스 코드이다.


418 CHAPTER 12.. 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 420 =====
    class Pong: public QObject
    {
        Q OBJECT
    public slots:
        Q SCRIPTABLE QString ping(const QSt,ring &arg) ;

1       "

Pong 클래스는 Session Bi娼를 통해 요청 받는 메시지를 처리한다. ping 멤버함수의 인자는 I기ng 예제
어플리케이션으로부터 받은 메시지이다. 이 메시지와 더불어 다음과 같은 메시지를 추가해 Ping에게 응
답한다．

    QString Pong: :ping(const QString &arg)
    {
            QMetaObject: : invokeMethod(QCoreApplication: : instance() , "q口it ' );
            return QString( "ping(\ "%l\ ") got called") .arg(arg) ;
    }

ping( ) 멤버함수는 리턴 값을 Session Bus를 통해 Ping에 메시지를 응답하기 위해 시그널 슬롯 이벤트
매 커니즘을 사용한다．

    QCoreApplication app( argc, ar可7) ;

    if      (! QDBusConnection: :sessionBus ( ) .isConnected( )) {
             fprintf (stderr, "Cannot connect to the D-Bus session bus. \n"
                      "To start it, run: \n"
                      "\ teval \ dbus-launch --auto--syntax ' \n") ;
             return 1;
    }

    if      (! QDBusConnection: :sessionBus ( ) .registerService (SERVICE_N月NE) ) {
             fprintf (stderr, "%s\n",
                        qPrintable (oDBusConnection: :sessionBus ( ) .lastError ( ) .message () ));
             e幻上 ( 1) ;
    }

    Pong pong;
    QDBusConnection: : sessionBus ( ) .registerObject ( "I ", &pong,
                                                   QDBusConnection: : ExportAliSlots) ;

    app.execQ;
    return 0;



    QDBusConnection 클래스에서 제공하는 registerOb如ct는 원격 오브젝트인 PiT培으로부터 응답을 처
    리하기 위한 이벤트를 처리한다. 첫 번째 인자는 Object Path를 명시한다. 두 번째 인자는 처리할 슬롯
함수를 명시한다. 슬롯함수는 QObject 클래스로부터 상속받은 클래스를 명시해야 한다. 세 번째 인자는
    연결된 오브젝트의 처리를 하기 위해 enum으로 제공되는 RegisterOpti아始를 명시한다．
    ExportAliSi毗S 값은 모든 오브젝트의 시그널을 처리하도록 지정한다. 세 번째 인자어］ 명시한 enum 값


                                                                            3 Inter-Process Communication 419


===== PAGE 421 =====
은 OR 연산을 통해1ei끄l1n을 중복해 사용할 수 있다．


ecdykt円目eddyktr,pc:，》1QtPrcjecrs/ptnq- batIdS . /ptng cteUo 口Bus

親｛儡論嶽섟們茹客：읽喆崙싻蒜 n




  뇨 ‘n 'n eddykhet ..,ddyk相寸pc ./QtProe(ts/pon9-buttd

" ：總雀썲；出盟．：器；:］客：;:：胃瓮搖1/P' " 9



（그림） F기ng & Pang 예제 실행 화면



 3.3.2 마Bus를 이용한 채팅 어플리케이션 예제
이번에 살펴볼 예제는 于Bus를 사용해 채팅 어플리케이션을 구현한 예제이다. 이 예제는 두 개의 창으
로 구성된다. 어플리케이션을 실행하면 Nick Name을 입력하기 위한 다이얼로그 창이 다음 그림 화면에
서 보는 것과 같이 활성화된다．



 Ne出'0崎kname:




（그림） 세ck Name 입력 다이얼로그



다이얼로그 창에 Nick Name을 입력하고 [OK] 버튼을 클릭하면 Nick Name 다이얼로그 창은 비활성
화되고 대화상자 윈도우가 활성화된다. 小Bus를 통해 메시지를 주고받기 위해 다음 그림에서 보는 것과
같이 두 개의 어플리케이션을 실행한다．


 " ecdy,口trn the dray                                   100,O卄吻的the chat
 " oorothy如lns the chat                                 .Dat야柳＞te5t
 亡t珀r吐l.y ted                                           .16匈＞ te1t
 <E1口PIe吼                                               .16小／'Hey咆 D＜目q口뿌
 .Eddy'tlaito Dorothy                                   tD010thy> m｛也 E小小r
 (i加r吐却＞Hd뇨，Id句




                                                        \1尸1느11}e            q 口d




（그림） 대화상자 윈도우



대화상자 윈도우 화면에서 전달할 메시지를 입력하고 [Send] 버튼을 클릭하면 다른 어플리케이션 대화상
자 위젯 상어］ 메시지가 출력한다．


420 CHAPTER 12m 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 422 =====
ChatMainwinclow: : ChatMainWindow ( )
    : mmnickname (QLatinlString ( "nickname ") )


    setupUi(this) ;
    sendButton->setEnabled (false) ;


    connect (messageLineEdit, SIGNAL (textChanged(QString) ),
             this, SLOT (textChangedSlot (QString) ));
    connect (sendButton, SIGNAL(clicked(bool) ),
              this, SLOT (sendClickedSlot ( ) ));
    connect ( actionChangeNickname, SIGNAL (triggered ( bool) ),
             this, SLOT (changeNickname(fl) ;
    connect (actionAboutQt, SIGNAL(triggered(bool) ), this, SLOT (aboutQt ( )));
    connect (qApp, SIGNAL(las七WindowClosedO) , this, SLOT (exiting() ));



messageLineEdit는 메시치 입력 위젯이다. 메시지가 변경되면 시그널 이벤트가 발생하며 이 시그널과
연결된 te玭ChangedSlot( ) 슬롯함수가 호출된다. 이 함수는 메시지 위젯 상어］ 입력한 문자열이 공백이
면 [Send] 버튼을 비활성화하고 그렇지 않으면 활성화한다．

void ChatMainWindow: :textChangedSlot (corist QString &new'Text)
{
    sendButton->setEnabled ( !newText. isEmpty () );
}


sendButton 버튼 위젯이 클릭되면 clicked( ) 시그널 함수가 발생하며 이 시그널과 연결된 슬롯함수
sendClickedSlot( ) 함수가 호출된다．

void ChatMainWindow: : sendClickedSlot ()
{
    I/ emit message (m_nickname, rnessageLineEdit->text ( ));
    QDBusMessage msg = QDBusMessage: :createSignal( "I ",
                                              "org.example.chat ", "message") ;
    msg << rn_nickname << messageLineEdit中>text () ;
    QDBusConnection: :sessionBus ( ) .send(rnsg) ;
    messageLineEdit->setText (QString( ));
}


QDbus入'lessage 클래스는 小Bus를 통하1 메시지를 송수신 하기 위한 기능을 제공한다. cateSignal()
함수는 새로운 小Bus 메시지를 Path로 전달하기 위한 함수이다. 이 함수는 메시지 전달을 위해 시그널
을 발생한다. 이 시그널이 발생하면 小Bus Path와 동일한 어플리케이션의 슬롯함수가 수행된다．

action(그hangeNickname은 파일 메뉴 상에서 [Change Nickname］을 클릭하면 발생하는 시그널 이벤
트이다. 이 시그널 이벤트는 changeNickname( ) 슬롯함수와 연결되어 있다. 이 함수는 변경된 Nick
Nan始을 멤버변수인 m_nickname을 변경한 다음 action( ) 시그널 이벤트를 발생한다. 이 시그널은


                                                                   3 Inter-Process Communication 421


===== PAGE 423 =====
actionSlot( ) 슬롯함수와 연결되어 있다．

    II add our 小Bus interface and connec七 七（그 먀Bus
   new ChatAdapto디七hi引 ;
   QDBusConnection: :sessionBus ( ) .registerObject ( "I ' , this) ;


   org: :example: :chat *iface;
   if ace = new org: :example: :chat (QString( ), QString( ),
                                       QDBusConnection: :sessionBus ( ), this) ;
   //connect (iface, SIGN2L (message(QString,QString) ), this,
                                       SLOT (messageSlot (QString,QString) ));
   QDBusConnection: :sessionBus ( ) .connect (QString( ), QString( ),
                                       "org.example.chat ", "message1' , this,
                                   SLOT(messageSlot (QString,QString) ));
   connect (if ace, SIGNL(action(QString,QString) ), this,
                                   SLOT(actionSlot (QString,QString) ));



QDBusConne毗ion 클래스는 小Bus에 연결하기 위한 기능을 제공한다. iface는 小Bus의 Interface
이며 Session Bus를 통해 연결된다. D-Bus와 연결을 위해 QDBusConnection 클래스에서 제공하는
connection( ) 함수를 사용해 D-Bus의 Session Bus와 연결을 시도한다．

마지막 iface 인스턴스를 connect( ) 함수에서 사용한 이유는 다른 어플리케이션에서 口Bus의 Session
Bus를 통해 연결된 원격 오브젝트 상에서 메시지를 요청받기 위해I Listener와 같은 역할을 한다．

   NicknameDialog dialog;
   dialog. cancelButton->setVisible (false) ;
   dialog.exec ( );
   m_n.icknanie = dialog.nicknanie->text ( ).triinmed( );
   emit action(m.enickname, QLatinlString( "joins the chat ") );




NicknameDialog는 사용자로부터 Nick Name을 입력받기 위한 다이얼로그이다. 사용자가 다이얼로그
상어꺼 Nick Name을 입력하고 [OK] 버튼을 클릭하면 Nick Name을 m nickname 멤버변수에 값을
저장하고 action( ) 시그널을 발생한다. 이 시그널의 첫 번째는 Nick Name이고 두 번째 인자는 Nick
Name과 함께 전달할 메시지이다．




422 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 424 =====
     .』1 QProcess
QProcess 클래스는 어플리케이션 내부에서 다른 프로세스와 통신을 하거나 다른 어플리케이션을 시작
하기 위한 기능을 제공한다. 프로세스를 시작하기 위해서 터미널과 같은 Command 입력 창에 이름과 인
자를 사용하는 것과 같이 QProcess 클래스어써 제공하는 start( ) 함수를 사용하면 된다. 그리고 프로세
스 뒤에 붙는 인자를 처리하기 위해 QStringList어］등록해 인자를 처리할 수 있다．

QObject *pareflt;


QString program = ". /path/to/ Qt/examples/widgets/ analogclock";
QStringList arguments;
arguments << "- style" << "fusion";


QProcess *myProcess = new QProcess (parent) ;
myProcess->start (program, arguments) ;



xli 윈도우 플랫폼에서 Analog 아ock 어플리케이션을 실행하기 위해 Command 입력 창에 어플리케
이션명을 입력하고 인자로 스타일을 변경하기 위한 인자를 추가하기 위해 예제 코드에서 보는 것과 같이
QStrii培List를 이용해 인자를 추가할 수 있다. start( ) 함수의 첫 번째 인자는 프로그램명을 명시하고
두 번째 인자는 사용할 인자가 있을 경우 명시한다．

이 외어匡 QProcess는 직렬 I/o 디바이스로부터 입력되는 신호를 처리할 수 있다. 이러한 신호를 처리
하기 위해 QProcess가 Running 상태로 진입하고 started( ) 시그널 이벤트를 발생한다. QProcess 상
에서 프로세스로부터 데이터를 READ/WI之ITE 하기 위해서는 주의사항으로 Windows CE 플랫폼에서
는 지원되지 않는다．

만약 QProcess가 종료되면 NotRunning 상태가 되고 finished( ) 시그널 이벤트를 발생한다. 이 시그
널 이벤트는 소스 코드가 종료되면 QProcess를 종료할 수 있도록 exitCode( ) 함수를 호출할 수 있다．

프로세스는 일반적으로 두 개의 출력 채널을 제공한다. 표준 출력으로 콘솔 창에서 output channel
(stdout）을 지원하고 채널 상에서 발생한 에러를 처리하기 위해1error channel (stderr）을 제공한다. 이
러한 표준 출력을 QProcess에서도 지원하며 setReadChannel( ) 함수를 Toggle하는 방식으로 호출해
사용할 수 있다. Channel 상어］ 데이터가 입력되면 QProcess는 readyRead( ) 시그널 이벤트를 발생한
다. 또한 에러 출력의 데이터가 발생하면 readyReadStandardError( ) 시그널 이벤트가 발생한다．

QProcess는 두 개의 표준 출력을 통합할 수 있다. 표준 출력과 에러 출력 사이의 모드를 변경하기 위해
setProcess（그hannelMode( ) 함수를 호출하면 된다．

QProcess builder;
builder. setProcessChannelMode(QProcess: :MergedChannels) ;
builder.start ( "make", QStringList () << "- j2 ") ;

if   (! builder.waitForFinished() )                                                        O


                                                              3 Inter-Process Communicafion 423


===== PAGE 425 =====
                                                                                          J
     qDebug() << n Make failed: " << builder.errorString() ;
 else
       qDebug() << "Make output: " << builder.readAll () ;


만약 어 떤 프로세스가 특정환경에서 동작하기 위해1setEnvironment( ) 함수를 사용할 수 있다．

 QProcess process;
 QStringList env = QProcess: :systemEnvironmentM;
 env << "T玉PDIR=C: \\MyApp\ \temp"; I/ Add an environment variable
 env.replacelnStrings (QRegExp ( " 八PATH= ( .기 ", Qt: :Caselnsensitive) , "PATH=\\l; C: \\Bin" ) ;
 process. setEnvironxnent (env) ;
 process .start ( "myapp") ;


그리고 특정 디렉토리에서 동작하는 프로세스를 위해 setWorkingDirectory( ) 함수를 통해 설정이 가
능하다．


. （가가ocess를 사용한 동기화 처리
QProcess 클래스를 사용해 프로세스로부터 출력되는 데이터 처리 동기화를 지원한다. 동기화 처리를 위
해서는 시그널을 사용해 처리할 수 있으며 제공하는 멤버함수는 다음과 같다．

클래스                      설명
 waitForStarted()        프로세스가 시작될 때까지 텨ocking 한다．
 waitForReadyRead()      Read Chann이상에 새로운 데이터가 READ 될 때까지 텨ocking 된다．
waitForBytesWritten()   『 프로세스에게 새로운 데이터를 WI귀TE할 때까지 텨ocking 된다．
waitForFinished()        프로세스가 종료될 때까지 텨ocking 된다．


메인 쓰레드에서 이러한 함수를 호출하게 되면 GI끄가 멈추게 되는 현상이 발생할 수 있다. 따라서 메인
쓰레드에서 사용할 때 주의해야 한다. 다음 예제는 이벤트 반복 없이 "Qt rocks!" 문자열을 압축하기 위
해 gzip 명령을 호출한 예제이다．

 QProcess gzip;
gzip.s七ar七（" gzip", QStringLis七（) << 느c " ) ;
if (! gzip.waitForStarted() )
    return false;


gzip.write ( "Qt rocks! ") ;
gzip.closeWriteChannel() ;

if   ( tgzip.waitForFinished() )
      return false;


QByteArray result = gzip.readAll( );




424 CHAPTER 12_ 데이터 커뮤니케이션과 인터넷 프로그래밍


===== PAGE 426 =====
CHAPTER




   멀티미디어


===== PAGE 427 =====
Qt 5 Programming




ri             ' 멀티미 디어
          （가는 멀티미디어 어플리케이션을 개발할 수 있는 오디오, 비디오, 카메라, 라디오 등 특정 디바이스의
           데이터를 처리할 수 있는 AP를 제공한다. 이번 장에서는 아에서 제공하는 멀티미디어 AP뻬 대해 알
          아보도록 하자．




Qt 4.0 버전부터 Qt어］ 제공하는 멀티미디어 API는 Qt Mobility를 위한 Multimedia Kit 모듈과 일반
적인 멀티미디어 지원을 위한 Qt Multimedia 모듈로 분류되어 개발자에게 제공하였다. Qt Mobility는
Smart Phone, Smart TV, Connected Car 등과 같은 플랫폼상에 멀티미디어를 지원하기 위한 API
를 제공하였다．

Qt 5.0 버전부터는 4.0 버전 이상에서 제공하던 기존의 일반적인 멀티미디어 모듈과 Qt Mobility의
Multimedia Kit 모듈이 Qt Mu!跏iedia 모듈로 통합되었다．

기존 4.0 버전에서 사용하던 Qt Multimedia 모듈로 개발된 어플리케이션 혹은 라이브러리는 최소한의
노력으로 5.0 버전에서 재사용할 수 있지만 Qt Mobility의 Multimedia Kit는 조금 복잡한 과정을 거쳐
야만 Qt 5.0에서 재사용이 가능하다．

또한 QVideoWidget 클래스와 같은 Widget 기반의 클래스는 Qt Multimedia Widget이라고 불리는
모듈로 분리되었다．

0Qt 5.0에서 새롭게 추가된 기능
   · QML에서 멀티미디어 사용이 가능한 API 추가
   · Video QML Type 추가, MediaF가ayer와 VideoO叫)Ut을 함께 사용할 수 있는 옵션 추가
   · QML Touch 클래스
   · 새로운 QAudioRecorder 클래스
   ·V아ume을 지원하기 위한 QAudioOutput과 QAudiolnput 클래스
   ·QSound는 Qt GI끄에서 Qt Multimedia로 이동
   ·C++ 뿐만 아니라 Q玉/lL어］서도 QSoundEffect를 활용
   ·FM Radio Data system 클래스와 타입을 활용（QRadioData, Radio Data)
   · 다양한 API의 개선과 버그 수정




426 CHAPTER 13_ 멀티미디어


===== PAGE 428 =====
S Qt 5.0에서 제거된 기능

제거된 API            설명
OMed回mage＼기ewer    많은 어플리케이션에서 사용하기에 적합하지 않7I 때문에 이 클래스는 5.0 버전부터 삭제되었다．



0at 5.0에서 변경된 （코 M네time비a Feature

변경된 Feature        설명
qmake의 .pro 프로젝    Ot 4 버전에서 사용하던 at 卜血jitimed治 Kit은 qmake의 프로젝트 파일 내에 다음과 같이 명시
트 파일에서 변경된 사항      해야 한다．
                   CON日G+ = m야川ty
                   MO테니TY + = m미timed治
                   at 5 버전부터는 다음과 같이 명시해야 한다．
                   QT+ = m미timed治
                   혹은 위젯 클래스를 사용하기를 원한다면 다음과 같이 사용해야 한다．
                   QT+ = multimedia multimediawidgets
Namespace          아MultimediaKit names口ace는 aM미timed治로 변경되었다. 이러한 namespace 변경은
                   SupportEstim졔e, Encoding（그uality, EncodingMode 그리고 AvailabilityStatus와 같은 몇
                   개의 Enumer졔ion에 영향을 미친다．
                   아M미timed治Kit를 OM미timed治로 대체하는 것은 멀티미디어 기능을 포팅하는데 수고를 덜어
                   준다． 그리고 atMultimediaKit에서 사용하던 Me怡 데이터는 aMediaMetaData로 분리되었다．
Meta da冶 ty口e      （카 Multimed治 Kit에서 마e-define된 메타 데이터 Key는 아M미timed治K什 네임스페이스에서
                   Enumer計山n로 정의되어 있다．
                   이러한 F가e-define된 Key는 aMe뎨aMetaDa治 네임스페이스에서 스트링 리터럴(Ii旭r졔引로
                   일관성 있게 변경되었다．
Meta da冶 Access와   enumeration Key 값들을 사용하i i가eH的fine된 meta data 상에서 연산을 위한
Method             aMe미aOb怜Ct 클래스의 metada怡（）와 같은 함수들과 스트링 키를 사용하1 확장된 me怡
                   da怡 상0私：1 연산을 위한 0M以ha아）尸Ct 클래스의 extendedMetaData(）와 같은 함수들이
                   at M미timed冶 Kit에서 두 가지로 제공되었다．
                   （기5에서는 Meta d計a를 접근하71 위해 스트링 키를 사용하는 방법과 Pre-define된
                   enumer례ion Key 키 값을 사용하는 방법 모두 사용할 수 있도록 하나로 통합되었다. （예
                   QMedia아기ect 클래스의 m（計aDat可 ) 함수）
at Met計y口1         at5는 이전 보다 Meta-o히ect 시스템으로 사용했던 것보다 클래스와 타입을 더 많이 등록되
registrat向n        었다．
                   at 卜爪기timedia 클래스에서 이전의 （工DEC냐＼RE_METATYPE을 적용했다면 at 5에서는 제거
                   하는 것이 바람직하다．
asoundEffect활용     이전에 사용되었던 SoundEffect aML 타입뿐만 아니라 C+＋에서도 at M미timed治 Kit에서 공
                   식적으로 사용했다. 아5에서는 asoundEt徊아로 변경해야 한다．
Camera 제어          디자인 설계상 문저까 있었던 카메라를 제어했던 많은 A미들이 개선되었다． 특히 일부 변수의 범
                   위 또는 데이터 유형이 조정되었다．




  till 오디오 컴포넌트
Qt에서 제공하는 Multimed奴는 오디오 입출력（Audio Ii叩ut/Ou印ut）을 처리하기 위해 High Level
에서 Low Level까지 접근할 수 있다. Audio 클래스를 제공한다. Qt는 /\udio 클래스를 사용해 멀티미
디어 기반 어플리케이션을 개발할 수 있도록 c+＋에서는 帥/lediaPlayer 클래스를 사용할 수 있다. 그리
고 QML을 사용한다면 Aud如와 MediaPlayer QML 타입을 사용할 수 있다．



                                                                                ] 멀티미디어 427


===== PAGE 429 =====
그리고 운영체제 플랫폼상어］ 의존적인 압축된 오디오 포맷을 지원할 뿐만 아니라 사용자가 인스톨한 멀
티미디어 Plug-in을 지원한다．

player = new QMediaPlayer;
II . . .
player->setMedia (QUr1: :fromLocalFile ( " /Users/me/Music/ coolsong.mp3 ") );
player->setVolume (50) ;
player->play () ;



Qt는 Audio 기능을 쉽게 구현할 수 있는 클래스를 제공한다. 앞의 예제 소스 코드에서 보는 것과 같이
帥iledial기ayer 클래스를 사용해 로컬 파일어］ 존재하는 MP3 오디오 포맷 파일 재생 기능을 쉽게 구현할
수 있다. 또한 원거리에 존재하는 오디오 파일을 네트워크를 경유하여 재생할 수 있는 기능도 쉽게 구현
할 수 있다．

player = new QMediaPlayer;


playlist   = new QMediaPlaylist (player) ;
playlist- >addMedia(Qurl( "http: //exarnple.comlmyfilel.mp3 ") )
playlist- >addMedia(QUrl( "http: IIexample .com/myfile2 .mp3 ") )
II . . .
playlist- >setCurrentlndex (1) ;
player->play () ;



1 오디오 데이터를 파일로 저장
Qt는 오디오 입력 디바이스로부터 들어오는 오디오 데이터를 특정 오디오 포맷 및 코텍（Codec）을 사용
해 레코드（Record) 기능을 제공한다. Qt에서는 오디오 입력으로부터 들어오는 데이터를 레코드 하기 위
해서는 QAudioRecorder 클래스를 제공한다．

audioRecorder = new QAudioRecorder;


QAudioEncoderSettings audioSettings;
audioSettings . setCodec ( "audio/amr ") ;
audioSettings . setQuality (QMultimedia: :HighQuality) ;


audioRecorder->setEncodingSettings ( audioSettings) ;


audioRecorder->setOutputLocation(QUrl: : fromLocalFile ( "test. amr ' ));
audioRecorder->record( ) ;




S 사운드 효과
멀티미디어를 위한 오디오 이외에 낮은 레벨의 사운드 효과를 재생하기 위한 목적으로 Qt는 QSound
Effect 클래스를 제공한다. 이 클래스는 사운드 효과를 재생하기 위해 WAV 포맷을 사용한다. QSound
Effect는 c+＋에서 사용하기 위한 클래스를 제공하며 QML을 지원하기 위해 SoundEffect 帥ilL 타입


428 CHAPTER 13_ 멀티미디어


===== PAGE 430 =====
을 제공한다. 이 두 클래스는 동일한 기능을 제공한다. 사운드 효과는 플레이 횟수를 반복적으로 재생할
수 있는 loop 기능을 제공한다．

이 기능을 사용하기 위해서는 QSoundEffect 클래스의 setLoop（그ount( ) 함수를 사용해 loop 횟수를
지정할 수 있다. 그리고 현재 지정된 반복 횟수를 알기 위해 loopCount( ) 함수를 사용하면 된다. 이 함
수는 설정된 loop 횟수를 m1lt 타입 값을 리턴한다．


e 오디오 데이터 플레이와 녹음하는 동안 데이터 모니터링
Qt는 오디오 데이터가 얼만큼 재생되고 있거나 어느 정도 녹음이 되고 있는지 모니터링 기능을 통해
Playback을 구현할 수 있다. 오디오 Playback 기능을 구현하기 위해 Qt에서는 시그널 슬롯을 통해 현
재 재생되고 있는 위치를 확인할 수 있다．

audioRecorder = new QAudioRecorder;


QAudioEncoderSettings audioSettings;
audioSettings. setCodec ( "audio/ amr ") ;
audioSettings . setQuality ( QNultimedia: : HigiQua1ity) ;


audioRecorder->setEncodingSettings (audioSettings) ;


audioRecorder->setOutputLocation(QUr1: :fromLocalFile ( n test. an-tr ") );


audioProbe = new QAudioProbe (this) ;
if   (audioProbe->setSource (audioRecorder) ) {
     connect (audioProbe, SIGNAL (audioBufferProbed(QAudioBuffer) ),
              this,   SLOT (calcuiateLevel (QAudioBuffer) ));
}

auclioRecorder->record() ;




* Low 레벨 오디오 데이터 처리와 레코드
Qt에서 제공하는 Multimedia는 오디오 입력과 출력을 통해 처리되는 Low 레벨 단위의 오디오를 출력
및 스피커를 통해 재생할 수 있는 기능과 녹음（Record) 기능을 처리할 수 있다. 예를 들어 하드웨어 기반
의 오디오 출력을 사용하는 특정 오디오 포맷을 제공할 수 있다．

이 러한 Playback 기능을 Qt에서는 QAudioOutput 클래스와 QAudiolnp毗 클래스를 사용해 Low 레벨
의 오디오 데이터를 처리할 수 있다. Qt에서 제공하는 Low 레벨 오디오 입출력은 두 가지 방식을 제공한
다. 그 방식은 push와 pull 방식을 제공한다. pull 기반의 방식은 QlODevice 클래스를 사용한다. 예를 들
어 QAudioOutp毗 클래스는 印ODe叭ce: :read( ) 함수를 사용해 들어오는 데이터를 pull 방식으로 처리
할 수 있다. 반대로 push 방식은 QAudioli叩毗 클래스를 QlODevice를 통해 직접 내보낼 수 있다．

또한 Qt에서 제공하는 QAudioO毗put은 높은 수준의 latency와 같은 Audio Playback 이외어］ 네트워
크를 경유하는 낮은 latency를 사용하는 \1oIP(Voice over Internet Pr毗oc아） 프로토콜을 사용해 오


                                                                              1 멀티미디어 429


===== PAGE 431 =====
디오를 재생하거나 녹음할 수 있는 기능을 제공한다．


e 메모리 상에 존재하는 오디오 데이터를 특정 포맷으로 Decoding
멀티미디어 어플리케이션을 개발하다 보면 여러 오디오 데이터 샘플을 MIX 할 수 있는 기능과 같이 메모
리상에 존재하는 오디오 데이터를 압축된 포맷으로 Decoding 할 수 있는 기능을 제공한다. Qt는 5.0 버
전부터 오디오 데이터를 Decodir乷하기 위해 QAudioDecoder 클래스를 사용할 수 있다. QAudio
Decoder 클래스는 印ODevice 인스턴스로부터 들어 오는 뎨이터를 직접 연결해 로컬 파일로 저장할 수
있다．

 QAudioFormat desiredForinat;
 desiredFormat . setChannelCount (2) ;
 desiredFormat. setCodec ( 1'audio/x-raw") ;
 desiredFormat.setSampleType (QAudioForniat: :UnSignedlnt) ;
 desiredForrnat.setSampleRate(48000) ;
 desiredFormat. setSaxnpleSize ( 16) ;


 QAudioDecoder *decoder = new QAudioDecoder (this) ;
 decoder->setAudioFormat (desiredFormat) ;
 decoder->setSourceFilenanie ( n levell. mp3 ") ;


 connect (decoder, SIGNAL (bufferReady () ), thiS I SLOT (readBuffer (fl) ;
 decoder->starti ) ;




0 （가에서 제공하는 오디오 클래스

클래스                         설명
QAudio                     오디오 클래스에서 사용하는 enum 타입을 포함하는 클래스
QAudioBt川er                오디오 샘플 ra也와 특정 포맷을 지정하:7 ' 위해 제공하는 클래스
QAud向Bu卄er::앉ereoFrame      스테레오 오디오 프레임을 위한 Wra口口er 클래스
QAudioDecoder              오디오 Decoding 기능을 제공하는 클래스
QAu뎨oDe미C이n幻               사용하는 오디오 디바이스에 대한 정보를 얻기 위한 클래스
QAudioFormat               오디오 스트림 파라미터 정보를 저장하기 위해 제공하는 클래스. 예를 들어 Hertz와 같은
                           Sam히e Rate, 오디오 채널 수, Samp冶 읽ze와 type 그리고 니비e endian과 B뗘
                           endian과 같은 Sam이e Order 파라미터를 저장하71 위한 클래스
QAudi이nput                 오디오 입력 디바이스로부터 들어오는 오디오 데이터를 처리하기 위한 클래스
QAudioOutput               오디오 데이터를 오디오 출력 디바이스로 전달하;71 위한 클래스
QAudi아＞robe                오디오를 재생하거나 녹음을 시작할 [111 모니터링을 제공하기 위한 클래스
QSound                     WAV 포맷 사운드 파일을 재생하71 위한 클래스
QSoundEftect               낮은 latency 사운드 효과를 재생하71 위한 클래스




430 CHAPTER 13_ 멀티미디어


===== PAGE 432 =====
     1.2 비디오 컴포년트

Qt에서 제공하는 Multimedia 기능은 Low 레벨에서 High 레벨 수준의 비디오 데이터를 재생 및 제어
할 수 있는 클래스를 제공한다. 또한 비디오 데이터를 Camera와 Audio 클래스를 비디오 데이터와
Overlap하여 사용할 수 있는 유용한 기능을 제공한다．

비디오 데이터를 처리해 어플리케이션을 구현하는 방식으로 C+＋과 QML을 사용해 구현이 가능하다．
C+＋을 사용해 비디오 데이터를 처리하는 멀티미디어 어플리케이션을 구현하기 위해 帥4ediaP1ayer 클
래스를 사용해 비디오 Decodir培이 가능하다．

비디오 데이터를 G｛끄상에 디스플레이 하기 위해서는 QVideoWidget과 QGraphicsVideoltem 클래스
를 사용할 수 있다. 또한 비디오 출력 영역을 사용자 정의 Custom 위젯을 제작해 비디오 데이터를 출력
을 위한 비디오 위젯을 구현할 수 있다. 다음 예제 코드는 QVideo＼肌dget 클래스를 사용해 비디오 데이
터를 출력하는 예제 코드이다．

player = new QMediaPlayer;


playlist = new QMediaPlaylist (player) ;
playlist- >ad小1edia(QiJrl( "http: //exarnple.com/myclipl .mp4 ") )
playlist- >addMedia(QUrl ( "http: //ex鈿nple.com/myclip2 .mp4 ") );

 videowidget = new QVideoWidget;
 player->setVideoOutput (videoWidget) ;

 videoWidget->show ( );
 playlist- >setCurrentlndex (1) ;
 player->play ( );



QVideoWidget 클래스는 로컬 파일로 존재하는 비디오 파일을 재생할 수 있을 뿐만 아니라 원격에 존재
하는 비디오 파일을 네트워크를 통해 낮은 latency를 처리할 수 있는 기능을 제공한다. QGraphics
Videoltem 클래스 또한 로컬 파일과 원격 비디오 파일을 제공할 수 있으며 사용하는 방법은 다음 예제
코드와 같다．

 player = new QMediaPlayer (this) ;

 QGraphicsVideoltem * item = new QGraphicsVideoltem;
 player->setVideoOutput (item) ;
 graphic sView->scene ( ) ->addltem( item) ;
 graphicsView->show() ;


 player->setMedia(QUrl ( "http: //example.com/myc11p4 .ogv " ) );
 player->play() ;




                                                                     ] 멀티미디어 431


===== PAGE 433 =====
 S QML을 이용한 비디오 재생
Qt는 C++ 외에도 QML에서 비디오 데이터를 재생할 수 있는 멀티미디어 어플리케이션을 구현할 수 있
도록 MediaPlayer와 Camera QML 타입이 제공하는 콘텐츠를 재생하기 위해 VideoO畇)Ut QML 타
입을 사용할 수 있다. 그리고 QML에서 비디오 출력 데이터 영역을 Shader Effect(QML Video
Shader Effects Example 참조）를 사용할 수 있다. 또한 비디오 데이터의 재생 모니터링을 위한
Playback과 재생 제어 기눙을 제공한다．


1Low 레벨 \/ideo 다ame의 조작
Qt는 Video Frame을 핸들링 하기 위한 Low 레벨의 비디오 데이터를 처리할 수 있는 클래스를 제공한
다. 또한 비디오와 카메라를 통해 특정 기능을 구현할 수 있는 기능을 제공한다. 예를 들어 카메라로부터
입력되는 Barcode를 Detectii培하는 것과 같이 비디오 프로세서를 적용할 수 있다. 이러한 비디오 프러1
임을 처리하기 위해 QVideoFrame 클래스를 사용할 수 있으며 시스템 메모리로부터 Mappii培된 비디
오 콘텐츠를 조작할 수 있다．

QVideoFrame 클래스는 QMediaPlayer와 QCamera로부터 처리되는 비디오 프레임 데이터를 조작하
기 위해 QAbstractVideoSurface 클래스로부터 파생되었다. 따라서 Low 레벨 비디오 프레임을 조작하
는 기능을 구현하기 위해I QAbstractVideoSurface 클래스를 상속받아 구현할 수 있다．

 class MyVideoSurface : public QlthstractVideoSurface
 {
      QList<QVideoFrame: : PixelFormat> supportedPixelrormats (
                  QAbstractVideoBuffer: :HandleType handleType =
                                    QAbstractVideoBuffer: :NoHandle) const
      {
          0 UNUSED (handleType) ;


          /7 Return the formats you will support
          return QList<QVideoFrame: :PixelFormat> ( ) << QVideoFrame: :Format RGB565;
      }

      bool present (const QVideoFrame &frame)
      {
          QUNtJSED ( frame) ;
          7/ Handle the frame and do your processing


          return true;
      }
 };
                                                                                        J



앞의 예제 소스 코드에서 보는 것과 같이 MyVideoSurface 클래스는 QAbstractVideoSurface 클래스
를 상속받아 구현하였다. 帥4edial기ayer 클래닉＝를 사용해 비디오 데이터를 디스플레이 출력 Surface를
지정할 수 있다．



432 CHAPTER 13_ 멀티미디어


===== PAGE 434 =====
iplayer- >setVideoOutput (myVideoSurf ace) ;


Qt에서 제공하는 비디오 클래스 기능뿐만 아니라 특정 비디오 Decode 기능을 구현하기 위해 QVideo
RendererContr아 클래스를 사용할 수 있다. 그리고 QML에서는 VideoO的）ut QML 타입을 통해 특
정 비디오 Decode 기능을 커스티마이징이 가능하다．

 class MyVideoProducer : public QObject
 {
      Q OBJECT
      Q PROPERTY ( QAbstractVideoSurf ace *vjdeoSurface WRITE setVideoSurface)


 public:
      void setVideoSurface (QAbstractVideoSurf ace * surface)
      {
            rn surface = surface;
            rn_surf ace->start (rnformat) ;
      }

      II . . .


 public slots:
      void onNewVideoContentReceived(const QVideoFrarne & frame)
      {
            if   (rn surface)
                 rn surface->present (frame) ;
      }

 private:
      QAbstractVideoSurf ace *msurf ace;
      QVideoSurfaceForrnat rn format;
 };
. 비디오 데이터 녹화 기능 구현
Qt는 비디오 데이터를 녹화（Recording）하기 위해 帥4ediaRecorder 클래스를 제공한다. 또한 카메라
입력으로부터 오는 데이터를 추가로 녹화할 수 있다．


0 비디오 프레임의 모니터링
Qt에서 제공하는 비디오 프레임을 재생할 때 얼마만큼 재생되었는지 Playback 기능을 구현하기 위해서
QVideoProbe 클래스를 사용할 수 있다. 이 클래스는 帥/lediaPlayer, QMecliaRecorder와 QCamera
에서 사용할 수 있다．

또한 QVide아斗obe 클래스는 QCamera어］서 입력되는 비디오 데이터 스트림을 조작하기 위해 QVideo
Probe를 통해 비디오 데이터를 캡처田apture）할 수 있다．




                                                                                 ] 멀티미디어 433


===== PAGE 435 =====
 . （값에서 제공하는 비디오 관련 클래스

 클래스                      설명
 QAbstractVideoButfer     비디오 데이터 처리를 위한 추상화 클래스
 QAbstractVideoSurface    비디오 데이터를 표시하는 Surface를 치정하기 위한 상위 클래스
 QVideoFrame              비디오 데이터 프레임을 표시하'I 위한 클래스
 QVide아가아）e               비디오 데이터 프레임을 모니터링 하기 위한 기능을 제공하는 클래스
 QVideoSurfaceFormat      비디오 데이터를 표시하는 Surface의 스트림 포맷을 지정하기 위해1
                          제공되는 클래스




       1.3 카메라 컴포넌트

Qt에서 제공하는 멀티미디어 API는 웹 카메라, 모바일 디바이스 카메라, 임베디드 디바이스 카메라 모듈
등과 영상 이미지를 접근할 수 있는 카메라 관련 클래스를 제공한다．

                          설명
 OCamera                   카메라 디바이스를 위한 인터페이스
 QCameraExposure           카메라 설정과 관련 ExF兀sure 인터페이스
 QCameraFocusZone          카메라 Au幻 幻cusing을 사용하기 위한 영역 정보 클래스
 QCameraFocus              Zoom, Focus와 관련한 카메라 설정 인터페이스
 OCameralmageCapture       미디어 레코딩을 위해 사용하는 클래스
 QCameralmageProcessing    카메라와 관련해 이미지 Processing을 처리하기 위한 인터페이스
（긔mageEncoderSe川ngs       이미지 Encoder 설정 클래스



0Viewfinder
Viewfinder는 카메라를 통해 영상을 확인할 수 있는 영역을 말한다. 대부분의 디지털 카메라는 낮은 해
상도（Resolution）에서 들어오는 카메라 영상으로부터 이미지를 이용해 Photo, Video를 구성할 수
있다．

또한 카메라 이미지 처리를 위한 낮은 해상도와 높은 해상도를 조절할 수 있다. Qt에서는 \[jew finder
를 보여주기 위해 카메라와 Video Ot此put을 함께 사용하며 QGraphicsView, Widget 중 사용자에게
보여지는 Viewfinder를 선택할 수 있다．

camera = new QCamera;
viewfinder = new QCameraViewfinder;
camera->setViewfinder (viewfinder) ;
viewfinder->show ( );

camera->start () ; // to start the viewfinder



카메라로 입력되는 신호를 프레임 단위로 처리하기 위해써 QAbstractV奴eoSurface와 QCamera 오브
젝트를 사용해 viewfinder를 구성할 수 있다. 이 경우어］ 이미지 처리를 위해 Viewfinder 이미지 영역을


434 CHAPTER 13_ 멀티미디어


===== PAGE 436 =====
다음과 같이 직 접 Rendering 해야 한다．

camera = new QCamera;
mySurface = new MyVideoSurface;
camera->setViewfinder (mySurface) ;


camera->s七ar七 ( ) ;
// MyVideoSurface: :present (. .) will   be called with viewfinder frames




. 카메라 이미지 Capture
카메라로부터 입력되는 \/iewfinder 영역을 이미지 캡처하기 위해 QCameralmage（그apture 오브젝트
초기화가 필요하다. Q（그ameralmageCapture 오브젝트를 초기화하고 start( ) 함수를 사용해 카메라
Viewfinder 영역이 이미지 처리를 시작하도록 start( ) 함수를 호출한다. 카메라 이미지 캡처가 발생하
면 카메라 이미지 처리를 한 다음 Pho的를 처리할 준비가 될 때까지 LOCK을 설정한다．

imageCapture = new QCameralmageCapture (camera) ;


camera->setCaptureMode ( QCaniera: : CaptureStilllmage) ;
camera->start ( ); II Viewfinder frames start flowing


//on half pressed shutter button
camera->searchAndLock () ;


I/ on shutter button pressed
imageCapture->capture() ;


I/ on shutter button released
camera->unlock () ;




. 카메라 영상 녹화 기능
QCamera는 카메라에 입력되는 이미지를 녹화하기 위해 帥4ediaRecorder 오브젝트를 사용한다. 카메
라 영상을 녹화하기 위해서 카메라 오브젝트를 생성하고 Viewfinder를 설정한다. 또한 영상을 녹화할
오브젝트를 초기화한다．

camera = new QCamera;
recorder = new QMediaRecorder (camera) ;


caxnera->setCaptureMode ( QCamera: : CaptureVideo) ;
camera->start () ;


//on shut土er 1乂it土on pressed
recorder->record( );


// sometime later,    or on another press
recorder->stop() ;



                                                                            1 멀티미디어 435


===== PAGE 437 =====
S 카메라 이미지 파이프라인 처리
카메라의 이미지 처리와 녹화와 같은 영상을 처리하는 기본적인 기능 이외에 카메라에 입력되는 영상을
파이프라인을 통해 처리할 수 있다. 예를 들어 파이프라인 처리란 카메라에 이미지를 다른 이미지와 합성
하거나 카메라 Focusir培을 조절하는 등 단순히 입력되는 이미지 처리뿐만 아니라 다른 이미지와 함께
처리함으로써 다양한 결과를 만들어 낼 수 있는 기능을 제공한다．

Qt에서 제공하는 Zoom과 같은 Focusing 기능은 QCameraFocus 클래스를 통해 처리할 수 있다．
QCameraFocus는 FocusMode와 FocusPointMode를 Enum 형태로 제공한다. 이러한 Enum은
AutoFocus, （兀砒inuousFocus, Infini甘Focus와 같은 설정이 가능하다．


. 카메라 이미지 F가ocessing 처리
Qt에서는 다양한 이미지 Processing 처리를 가능하도록 QCameralmageProcess 클래스를 제공한다．
이 클래스는 White Balance, contrast, saturation, Sharpening, denoising 기능을 포함하고 있다．



            라디오 컴포넌트

Qt가 제공하는 멀티미디어 API는 RDS(Radio Data System)에 접근해 라디오의 Tuner와 같은
Contr아를 제어할 수 있는 기능을 제공한다. 라디오 API는 두 개의 컴포넌트로 구성된다. 하나는 라디오
Tuner를 제어하기 위한 QRadioTuner 클래스이다. 다른 하나는 RDS 정보를 접근하기 위한
QRadioData 클래스이다．

QRadioTuner 클래스는 아날로그 라디오 디바이스 인터페이스를 제공한다. 이 클래스를 사용해 라디오
인터페이스를 구성하기 위해 다음과 같이 소스 코드를 작성할 수 있다．

radio = new QRadioTuner;
connect (radio, SIGNAL (frequencyChanged(int) ),
                                this, SLOT (freqChanged(int) ));


if   (radio->isBandSupported ( QRadioTuner: : FM) )
 {
     radio->setBarid ( QRadioTuner: : FM) ;
     radio->setFrequency ( yourRadioStationFrequericy) ;
     radio->setVolurne ( 100) ;
     radio->startj;




라디오 오브젝트는 라디오 상태가 변경됨에 다양한 시그널 이벤트를 제공한다. bandChanged( ) 시그널
이벤트는 라디오 Tuner가 변경되었을 때 발생하는 시그널이다. frequencyChanged( ) 시그널은 라디
오 Frequency가 변경될 때 발생한다. stereoStatusChanged ( ) 시그널은 라디오 스테레오 시그널을
받을 경우 발생하는 시그널 이벤트이다. searchingChanged( ) 시그널은 라디오 Tuner가 현재
Scanning 하고 있는지 판단해 시그널을 발생한다．


436 CHAPTER 13_ 멀티미디어


===== PAGE 438 =====
signalStrengthChanged( ) 시그널은 백분율로 라디오 신호강도가 변경되었을 때 시그널 이벤트가 발
생하며, volumeChanged( ）은 라디오 볼륨 시그널이 발생했을 때, mutedChanged( ）는 라디오 M毗e
시그널을 처리하기 위한 시그널 이벤트이다．

QRadioTuner 클래스의 setBand( ) 멤버함수는 Bandwidth를 지정할 수 있다. QRadioTuner 클래스
는 라디오의 Bandwidth를 구분하기 위해 다음과 같이 Enum형을 제공한다．

Constant           Value Description
QRad向Tuner::AM           520"怜伯KHz, 9 또는 10KHz 채널인 S口acing과 1610N
                         ］기0KHz까지 확장 가능
QRadioTuner::FM    1     87.5N伯8.0MHz, 일본은 76' 90MHz
QRadioTuner::SW    2     1.711"-'30.OMHz, 15Band로 파생. 5kHz 채널 spacing
QRadioTuner::LW    3     148.5"-283.5kHz, 9kHz 채널 spacing
                         (Europe, Atrica, Asia)
QRadioTuner::FM2   4     정의되지 않은 범위 FM 주파수를 지원하기 위한 영역


QRadioData 클래스는 라디오 시스템의 RDS(Radio Data System) 기능을 구현하기 위한 인터페이스
를 제공한다. 라디오 데이터 오브젝트는 라디오 데이티가 변경되면 시그널을 발생한다．

 radio = new QRadioTuner;
 radioData = radio->radioData( );




                                                                        1 멀티미디어 437


===== PAGE 439 =====
M@vvio


===== PAGE 440 =====
CHAPTER




데이터베이스


===== PAGE 441 =====
Ct 5 Programming




F尸1 >/데이터베이스
         ' 아는 MySQL, Oracle, MS-SQL, SQLite, DB2 등과 같은 데이터베이스와 연걸할 수 있는 인터퍼떼
           스를 제공한다. 이번 장에서 제공하는 AP를 사용해 데이터베이스를 핸들링하71 위한 AP뻬 대해 살펴
           보도록 하자．




수많은 어플리케이션에 서버 컴퓨터와 연결되어 방대한 정보를 사용자에계 효율적으로 전달하기 위한 방
법으로 데이터베이스를 사용한다. 또한 특정 목적의 용도로 사용되는 임베디드 디바이스 시스템에서 사
용하는 정형화된 데이터베이스를 사용함으로써 대량의 데이터를 효율적으로 관리하는 목적으로 메모리
기반의 데이터베이스를 사용한다．

Qt에서도 데이터베이스와 연동하여 응용 어플리케이션 개발을 위한 모듈을 제공한다. Qt에서 제공하는
API는 다른 개발 API에 비해 직관적이고 이해하기가 쉬운 구조로 되어 있다. Qt에서 제공하는 API를
사용하기 위해서 다음과 같이 헤더 파일을 추가해야 한다．

 #include <QtSq1>


프로젝트 파일（.pr이에 다음과 같이 Qt SQL 모듈을 추가한다．




데이터베이스와 연동하여 어플리케이션을 개발하기 이전에 데이터베이스에서 사용하는 SQL 언어에 대
해 사전지식이 필요하다. 예를 들어 SELECT, INSERT, UPDATE, DELETE문과 같이 SQL에서 사용
하는 구문에 대한 이해가 필요하다．

Qt를 이용해 응용 어플리케이션 개발을 위해 C++ 언어를 사용하듯 데이터베이스도 SQL이라는 언어를
사용하여 뎨이터를 질의한다. SQL은 데이터를 일정한 형태로 수집, 축적 , 보존한 데이터 파일이며 적합
한 정보를 정확하게 검색하도록 레코드를 논리적으로 질의할 수 있다．




440 CHAPTER 14_ 데이터베이스


===== PAGE 442 =====
. （가에서 제공하는 데이터베이스 클래스

클래스                       설명

QScil                     아에서 제공하는 SQL 라이뵤러리를 사용하기 위한 클래스
QSq I DriverCreatorBase   SQL 드라이버를 위한 상위 클래스
QSqlDriverCreator         드라이버 타입을 지정하기 위하1 제공되는 템플릿 클래스

QSalDatabase              데이터베이스에서 연결하기 위해 사용되는 클래스
QSqlDriver                특정 5（그［m 데이터베이스를 액세스하21 위해 제공되는 추상화 클래스
QSqlError                 데이터베이스에서 발생하는 에러 정보를 알리기 위한 클래스

QSqlFieId                 SQL 데이터베이스 테이블과 뷰(Views）에서 디이d를 조작하기 위하1 제공되는 클래스
QSqllndex                  데이터베이스 인덱스를 조작하기 위한 클래스

Os이Que四                    SQ[ 구문을 조작하고 실행하7I 위l1 제공되는 클래스

QScilRecord                데이터베이스 레코드를 은닉화한 클래스

Os이Result                 특정 데이터베이스로부터 데이터를 액세스하기 위해 추상화된 인터페이스 클래스

Os이Query卜加的1               SQL 결과를 위해 데이터 모델을 위해 단지 읽기 모드만 지원하는 클래스

QS（카Relation톄Table卜加del    외부 키（For이gn Key）를 사용하1 단일 데이터베이스 테이블에서 데이터 모델을 수정하71
                           위해 제공하는 클래스
QS뎨Table卜加del              단일 데이터베이스 테이블에서 데이터 모델을 수정하71 위한 클래스



Qt에서 제공하는 데이터베이스 클래스는 다음과 같이 3가지 형태로 나눠진다．



                               SQL API Layer      User Interface Layer
        Driver Layer

                            데이터베이스에 접근해         데이터베이스에 저장된 데이터를
  SQL 사긔와 데이터베이스를
                          데이터를 조작하기 위한 레이어        위젯과 연결해 사용자를
    연결하기 위한 레이어
                                               인터페이스를 제공하기 위한 레이어



（그림） S（그L Layer



S Driver Layer
QSqlDriver, QSqlDriverCreator, QSqlDriverCreatorBase, QSqlDriverPlugin, QSql Resu1t로
구성된다. 이 레이어는 특정 데이터베이스와 SQL API 레이어 사이의 Low-Level의 Bridge 연결을 위
한 레이어이다. 예를 들어 데이티베이스는 八4ySQL, Oracle, MS-SQL 등 다양한 데이터베이스에서 제
공하는 표준 드라이버를 제공한다．


 S SQL API Layer
SQL 드라이버 상위 클래스이며 데이터베이스에 접근하기 위한 QSqlDatabase 클래스를 제공한다 ．그
리고 데이터베이스어］ 접근해 데이터를 조작하기 위해 QSqlQuery 클래스를 제공한다. 또한 QSq1 Data
base와 QSqlQuery에서 QSqlError, QSq1Fie1d, QSqllndex, QSqlRecord를 지원한다．




                                                                         1 데이터베이스 441


===== PAGE 443 =====
 S User Interface Layer
뎨이터베이스에 저장된 뎨이터를 위젯과 연결해1 사용자의 인터페이스를 제공하기 위한 레이어다. QSql
QueryModel, QS아TableModel, QSqlR이atiionalTableModel 클래스가 이 레이어에 포함된다. 이
클래스는 Qt에서 사용하는 Model/View Framework를 사용한다．



            데이터베이스와 S（그［. 이하1

데이터베이스 시스템이란 저장 장치에 전산화된 뎨이터 파일의 저장 장치라고 보면 된다. 정보를 유지하
고, 이 정보를 이용 가능하게 하는 시스템을 말한다. 뎨이터베이스도 기본은 파일이며 데이터베이스는 파
일어］ 데이티베이스에 기록하거나 질의하는 등 필요한 기능을 제공한다．

데이터베이스는 데이터를 다루는뎨 테이블이라는 논리적인 구조에 레코드들을 저장한다. 레코드는 각 뎨
이터의 행으로 생각하면 된다. 레코드들이 모여 하나의 테이블이 되고 테이블들이 모여 하나의 독립적인
데이터베이스를 구성한다. 지금까지 설명한 데이터베이스 추가, 생성한 데이터베이스에 테이블을 추가하
고 테이블에 다시 레코드를 기록하거나 하는 기능은 파일을 이용하여 데이터를 직접 제어하는 것에 비해
어떤 장점이 있는지 알아보도록 하자．

  · 레코드의 중복으로 인한 오류가 감소
  · 방대한 뎨이터를 검색하는데 불일치한 데이터 검색 오류를 방지
  ·SQL이라는 언어를 통히f 데이터를 표준화

데이터베이스 응용 어플리케이션과 연동해 사용하는 대부분의 상용 및 공개 데이터베이스 소프트웨어는
대부분 RDBMS를 사용한다. RDBMS는 관계형 뎨이터베이스라 하며 시스템의 특징은 테이블간의 연관
관계를 지어 데이터를 검색할 수 있다. 관계형 데이터베이스 시스템의 특징은 다음과 같다．


S Primary Key
레코드를 이전에 행（Row）이라고도 한다. 행들은 열（C아umn)들로 분류되고, 행에 속한 열을 엔티티라고
한다. 이 엔티티들이 중복되지 않은 속성을 기본키 또는 Primary Key라고 한다．


S Null 기능
열 혹은 엔티티는 Null 값을 가질 수 있다．


S 데이터 무결성
엔티티 내의 각 행을 식별하는 일련의 속성들을 갖고 있다. 그러므로 어떠한 행도 테이블 내에 동일한 엔
티티가 존재할 수 없다. 이것은 모든 테이블이 기본키를 갖고 있어야 한다는 것으로, 데이터 무결성이라
한다．


S 데이터와 레코드 간의 Relation 관계
데이터베이스 내에 속한 테이블들은 외부키（Foreign key）를 통해서 서로 관꼐를 맺는다. 외부키는 가능


442 CHAPTER 14_ 데이터베이스


===== PAGE 444 =====
한 값의 집합이 두 번째 테이블의 기본키에서 발견되는 목적인 한 개의 테이블의 열（ROW）이다． 그렇기
때문에 테이블들을 조인（JOIN)하기가 쉽다. 참조 무결성은 어떤 외부키 열 내에 있는 값（Value）들이 참
조하는 기본키나 널（Null) 값으로 제한될 때 성취된다．

관계형 데이터베이스의 특징은 SQL을 이용하여 떼이터베이스와 연결해 데이터를 조작한다. SQL을 간
단히 살펴보면 SQL은 구조화 질의 언어라고 할 수 있다． SQL은 비프로시저 언어이다． 데이터에 접근가
여 조작하는 방법을 정확히 기술해야 하는 C 언어나 C++ 언어와는 달리 SQL은 내부적으로 요구한 것을
수행하는 방법을 결정한다. 그러므로 다른 언어에 비해 가독성이 좋으며 짧은 코드로 데이터베이스와 통
신할 수 있다．

지금까지 설명한 데이터베이스의 기본적인 개념과 특징을 SQL 언어를 통해 논리적으로 접근하기 위해
다음과 같이 특징으로 분류할 수 있다．


好 데이터베이스（DATABASE)
데이터베이스는 여러 개의 테이블（Table）이 모여 하나의 데이터베이스를 이룬다. 앞에서 설명한 데이터
베이스 구조에서 테이블을 이루는 데이터 파일만 확인할 수 있으며 나머지는 데이터베이스 내부에서 관
련된 정보를 갖고 있다. 하나의 데이터베이스는 파일 시스템에 파일로 존재한다．


彷테이블（TABLE)
기존의 파일 시스템에서 "1101터를 저장가는 곳은파일 " 1지만 "110］터베 ' ］스에서는 테 " 1블" 忙F는 데이터
베 "］스 구조에 "카' ］터를 저장가게 된다． 모든 터101블은 " 1름으로 구분되며 "110］터는 행（Row）이나 열
(Column) 단위로 저장된다． "]] ' ］터의 정확성을 보장가기 위긔
                                        '서 테 "］블을 생성할 때 각각의 열
(C아umn)에 제약사항을 지정할 수 있다.


小 인덱스(INDEX)
테 "］블 내의 " 카"］터를 검색하고자 할 때 속도를 향상시키는 방법으로 인덱스를 사용한다． 인덱스는 테 " ]
블에 사전적인 INDEX를 만들기 때문어］ 검색을 빨리 할 수 있는 장점이 있다. 그러므로 테이블에 대량의
데이터가 존재할 경우 인덱스를 생성하면 빠른 속도를 보장한다. 그러나 데이터를 삽입 , 수정 , 삭제를 할
때 인덱스를 다시 하게 된다．


1 뷰（VIEW)
뷰는 가상의 테이블이다. 실제로 존재하지는 않자만 실제 존재하는 테이블의 데이터를 연결하여 가상의
테이블을 만들 수 있는데 , 이것을 뷰라 한다. 뷰는 여러 개의 테이블을 하나의 가상의 테이블로 구성할 수
있다．


0 동의어（SYNONYM)
테이블어］ 이름을 다른 이름으로 참조할 수 있다. 예로 NAME이라는 필드를 "이름" 으로 다르게 동의어를
만들어 사용할 수 있다．


                                                        1 데이터베이스 443


===== PAGE 445 =====
D 시퀀스（SEQUENCE)
순차적으로 증가하는뎨 레코드어］ 번호를 부여할 수 있다. 이러한 순차적인 번호는 뎨이터가 추가됨에 따
라 자동으로 증가되게 할 수 있다．

SQL 특성은 언어의 특성을 가지므로 SQL을 이용해 데이터베이스에 저장된 데이터를 삽입 , 수정, 삭제
를 수행한다. SQL은 어떠한 구조적인 형태의 언어가 아니므로 C 언어와 0+＋과 같은 구조적인 프로그래
밍을 지원하지 않는다. 즉, IF문이나 반복문을 이용할 수 없다．

SQL을 좀더 구조적인 프로그래밍을 원할 경우 4GL을 사용하면 가능하지만, SQL 표준은 지원하지 않는
다. 그리고 SQL은 뎨이터 타입을 테이블의 Column에 지정할 수 있는데 이는 INT, CHAR,
VARCHAR 등과 같은 데이터 타입을 열에 지정해야 한다. SQL은 3가지로 분류할 수 있다．

        클래스                                 설명
        DML(Data Manipulation Language)     데이터를 검색하거나 변경하는 데이터 조작 언어
        DDL(Data Definition Language)       데이터의 구조를 정의하는 데이터 정의 언어
        DCL(Data Control Language)          데이터베이스 사용자에게 부여한 특권을 정의하는 데이터 제어 언어



   S SELECT문 : 테이블로부터 행 검색
 SELECT문은 녜개의 DML문 중에서 가장 많이 쓰이는 구문이다. 그리고 UPDATE, INSERT,
DELETE문 내에서 서브 쿼리로써 존재할 수 있다. SELECT문은 기본적으로 다음과 같이 구성된다．

        SELEC쏘 컬럼명 FR（外4 테아뷸명 WHER丑 검색 조건



예를 통해 뎨이터를 검색해 보도록 하자. STUDENTS라는 테이블의 이름을 다음과 같이 검색할 수 있다．

        SQL> SELECT NA侄 FROM STUDENTS;



학생의 이름과 나이를 질의하기 위해 다음과 같이 SQL문을 작성하면 된다．

        SQL> SELECT NAME, AGE FROM STUDENTS;



테이블의 모든 레코드를 검색해햐 한다면 다음과 같이 검색하면 된다．

}SQL>
              SELECT   *   FROM STUDENTS;



  SQL에서 사용되는 산술 연산은 C++ 언어에서 사용하는 산술 연산과 동일하다. 다음 예는 산술 연산을
 사용한 예이다．

        SQL> SELECT NAM日, AGE, KOR, ENG, (KOR+ENG) /2 AS AVG FROM STUDENTS;




        S 八SERT문 : 테이블에 행 추가
INSERT문은 테이블에 행을 추가할 때 사용한다．


  444 CHAPTER 14_ 데이터베이스


===== PAGE 446 =====
SQL> INSERT 工NTO STUDENTS（컬럼명r     . . . .) VALUES（컬럼의 값r       . . . . );



 UPDATE문 : 테이블 내의 기존 행 변경

SQL> UPDNI匣 STUDENTS SET KOR=88 WHERE NAN丑 LIK丑 1 홍길동1 ;



也 DELETE문： 테이블에서 행 제거

SQL> DELETE FROM STUDENTS; （모든 래코드 삭저I)
SQL> DELE쪼E FROM STUDENTS WHERE ENG=S2; （조건에 만족하는 레코드만 삭제r



小 NULL 연산자
관계형 데이터베이스에서는 어떤 열을 위한 널（Niill) 값은 다양한 용도로 사용할 수 있다. 열 값으로 널
(Null）을 갖고 있는 행을 SQL문을 이용해 다음과 같이 검색할 수 있다．

SQL> SELECT * FROM STUDENTS WHERE NAME IE;NOT NULL;



지금까지 살펴본 SQL 문법은 기초적인 내용이기．도 하지만 가장 많이 사용하기도 한다. 어떤 응용 어플
리케이션을 개발하는지어］ 따라 SQL문을 복잡하7n 작성해야 하는 경우도 있을 것이고 그렇지 않은 경우
도 있을 것이다．

어떤 데이터베이스를 사용하느냐어］ 따라 SQL문으q 문법도 약간 다를 수 있다. SQL문이 표준이긴 하나，
데이터베이스의 특성에 따라 표준을 따르지 않는 껑우가 많다. 이번 장에서 다룬 내용은 이 단원에서 설
명할 Qt SQL 모듈과 예제를 이해하는데 필요한 내용이다. 따라서 이번 장의 내용이 부족하다면 데이터
베이스 관련 자료를 참고하기 바란다．



乞才，1.2j 데이터베이스 연결과 지원하·는 드라0뻐

데이터베이스어］ 접근하기 위해 Qt에서는 QSq1Qi肥ry와 QSqlQueryModel 클래스를 사용해 특정 데이
터베이스에 연결해 테이블을 생성하거나 레코드를, 조작할 수 있다. QSqlDatabase는 데이터베이스 연결
을 위한 고유한 사용자 계정을 사용해 연결할 수 있다. 또한 사용자 계정을 사용하지 않는 데이터베이스
어］ 접근하기 위한 기능을 제공한다．

                             e: : addDatabiise ( H QMYSQL! );




                              );




                                                                             ] 데이터베0匹 445


===== PAGE 447 =====
 첫 번째 라인은 데이터베이스 연결을 위한 오브젝트를 생성한다. 그리고 setHostName( ) 멤버함수를
이용해 원격 혹은 로컬에 존재하는 데이터베이스에 접근할 수 있다. 데이터베이스 서버에는 여러 개의 데
이터베이스로 구성될 수 있다．

 QSqloatabase firstDB = QSqlDatabase: :addDatabase ( "Q玉YSQL", "first '! );
 QSqloatabase secondDB = QSqlDatabase: :addDatabase ( "Q卜YSQL", "second") ;



데이터베이스 연결 초기화가 완료된 후 open( ) 멤버함수를 사용해 데이티베이스를 연결해야 한다. 만약
open( ) 함수를 사용해 데이터베이스 연결이 실패하면 이 함수는 false를 리턴한다. 한번 연결된 특정 더］
이터베이스 내에 데이터베이스 파일을 연결하기 첫 번째 인자인 뎨이터베이스 드라이버명을 다음과 같이
생략할 수 있다．

iQSqlDatabase defaultDB = QSqlDatabase: :database ( );

i 쁘qluatanase tlrstii,B = Qbqloatabase: :dataDase tlrst )
1vbq上Jataoase seconauo   = 1?bq工uataoase: :oataoase ( secona J
                                                     (
                                                         "
                                                              '
                                                                  ,;.
따라서 뎨이터베이스를 지정하기 위해서 setDatabaseName( ) 함수를 통해1 지정할 수 있다. 사용자명과
패스워드를 지정하기 위해 seti招erName(）과 setPassword( ) 함수를 사용하면 된다. Qt는 데이터베이
스와 연결하기 위해 드라이버가 필요하며 다음과 같은 데이터베이스를 지원한다．

Driver name   DBMS
 QDB2         IBM DB2 (7.1 또는 그 이상 버전）
（긔BASE        Borland InterBase
QMYSQL        MySQ［口
QOCI          Oracle Call Interface Driver
QODBC         0口en Database Connectivity(ODBC） 卜川or（그sot t S（孔 Server와
              LF른 ODBC-compliant databases
QPSQL         PostgreS（그L(7.3 또는 그 이상 지원）
0S（가JTE2      SQLite version 2
QSQ니TE        SQL陀 version 3
QTDS          Sybase Ada帥ye Server (Ot 4.7 이상에서 지원）



SQLite는 프로세스 내에서 동작하는 경량의 데이터베이스이며 모든 운영체제 플랫폼에서 지원한다. 윈
도우와 리눅스 플랫폼상에서 OCT를 사용하는 Oracle, PostgreSQL과 MySQL은 Native Driver 또는
ODBC 사용이 가능하다．

Qt에서는 특정 데이터베이스 시스템과 연결하기 위해 필요한 드라이버를 플러그인 형태로 빌드할 수 있
다. 이러한 데이터베이스 드라이버를 플러그인 형태로 빌드하기 위해서는 데이터베이스 시스템에서 제공
하는 클라이언트 라이브러리가 필요하다．

리눅스와 Mac OS X 플랫폼 상에서 Qt configure 스크립트에서 빌드 시 클라이언트 라이브러리 파일을
찾을 수 있도록 명시해야 한다. configure 스크립트어］ 대한 자세한 도움말은 help 옵션을 통해 참고할


446 CHAPTER 14_ 데이터베이스


===== PAGE 448 =====
수 있다．

       ql- <driver>      Disable SQL <driver> entirely.
       ql- <driver>      Enable a SQL <driver> in the Qt Library, by default
                         none are turned on.


-plugin- sql-<driver> Enable SQL <driver> as a plugin to be linked to
                         a七 run 七irne.


                         Possible values for <driver> :
                         [ db2 ibase mysql o二i odbc psql sqlite sq1ite2 tds j



configure 스크립트는 필요한 데이터베이스 라이브러리와 헤더 파일을 찾을 수 없다. 그렇기 때문에 데
이터베이스 클라이언트 라이브러리 -L과 헤더 파일 I 옵션을 사용해 지정해야 한다．

예를 들어 MySQL을 인스톨된 디렉토리（/usr/l cal/mysql) 하위에 헤더 파일 디렉토리와 라이브러리
디렉토리가 포함되어 있다. （윈도우의 경우 c:\m sql\include) configure어］추가 옵션으로 헤더 파일의
경우 -I'岫바local/rn邪ql을 명시해야 한다．

윈도우 플랫폼의 경우 I 옵션 파라미터를 사용해 헤더 파일을 사용하지 않는다. 예를 들어 MySQL 디
렉토리를 지정해야 하며 c:\Program Files\mysql 대신에 C: \Program Files\n玎sql을 사용한다．

일반적으로 Qt에서 데이터베이스 드라이버를 빌드하기 위해                           q卜sql- <drive力를 사용한다. 만약 플러
그인 형태로 드라이버를 빌드하기 위해서는 -plugin-sqi- <driver> 옵션을 사용한다．


0（코에서 제공하는 MySQL 프로시저
MySQL5 버전부터는 SQL 레벨에서 저장 프로                       1를 제공한다. 하지만 IN과 OUT 파라미터를 제어하
기 위한 API가 없다. 그러므로 QSqlQuery: :bjr                alue( ) 대신해 SQL command를 사용해야 한다．
다음 예제는 저장 프로시저이다．

create procedure qtestproc (OUT parami INT, OUT paraxn2 INT)
BEGIN
      set paraml = 42;
      set param2 = 43;
END



Qt어］서 OUT 파라미터를 접근하기 위해서 다음과 같은 방법을 사용해야 한다．

QSqlQuery q;
q.exec ( "call qtestproc (@ outvall,     @Outva12) n) ;
q.exec (「 select @outvall, @outval2 'r ) ;
小 next ( ) ;
qDebug() << q. value (0) << g.value (l) ; 1/ outputs "42 " and "43 "




                                                                           ] 데이터베이스 447


===== PAGE 449 =====
DEmbedded MySOL Server
MySQL embedded server는 일반적인 MySQL 서버에서 제공하는 클라이언트 라이브러리를 교체해야
한다. Embedded MySQL Server를 사용하기 위해서 libmysqiclient 라이브러리 태신해 libmysqid
라이브러리를 Qt 플러그인 링크를 사용한다. 따라서 qmake에서 크mysqiclie砒r를 크mys 아d로
command를 변경해야 한다. 좀더 자세한 사항은 "libmysqid, the Embedded MySQL Server
Library" Chapter 또는 MySQL embedded server와 관련된 정보를 참조하기 바란다．


0Unix／니nux와 Mac OS X 플랫폼에서 at MyS（겄을 빌드
드라이버를 적용하기 위해 공유 라이브러리인 libmysqiclient. so 파일 뿐만 아니라 헤더 파일도 필요하
다. 리눅스 상에서 패키지를 배포하기 위해서는 "mysqi-devel" 패키지를 설치해야 한다. MySQL 헤더
파일과 공유 라이브러리를 qmake가 찾을 수 있도록 하기 위해서 다음과 같이 make 파일을 수행해야
한다．

Cd $QTDIR/ src/plugins/ sqldrivers/mysql
qmake "INCLUDEPATH+=/usr/local/ include" "LIBS+=-L/usr/local/ ll b
                                            .-lmysqlclient_r " mysqi.pro




0 윈도우 플랫폼에서 （값 MySOL 플러그인 빌드
윈도우 플랫폼에서 플러그인을 빌드하기 위해서는 MySQL 인스톨 파일이 필요하다. SETUP.EXE 파일
을 실행하고 "Custom Install" 을 선택한다. "Libs & Include File" 모듈을 인스톨하고 다음과 같이 플
러그인을 빌드한다．

cd %QTDIR% \ src\plugins\ sqldrivers\mysql
qmake "INCLUDEPATH+=C: /MySQL/include"
   "LIBS+=C: /NYSQL/MySQL Server <version>/lib/ opt/libmysql. lib ' mysqi .pro
nmake



만약 마이크로소프트에서 제공하는 컴파일러를 사용하지 않는다면 nmake 대신 make 파일을 사용한다．
그리고 Windows CE 플랫폼 기반에서는 플러그인을 지원하지 않는다．


0Oracle Call Interface를 위한 0001
Qt에서는 Oracle 9i, lOg 그리고 그 이상 버전에서 OCI 플러그인을 지원한다. Tnsnames. ora 파일 없
이 Oracle 데이터베이스에 연결하는 것이 가능하다. 이러한 방법은 데이터베이스의 호스트 네임 , 데이터
베이스명과 같이 드라이버를 연결하기 위해 뎨이터베이스 SID를 요구한다．

Qt에서 제공하는 QOCI는 내부 credential를 사용하기 위한 인증을 지원한다. 이는 Oracle에서 제공하
는 인증 매커니즘 대신 운영체제 플랫폼에서 제공하는 사용자 인증을 사용한다．




448 CHAPTER 14_ 데이터베이스


===== PAGE 450 =====
    tOCI BLOB/LOB지원
Qt에서는 Binary Large Objects(BLOBs）의 耳EAD/ WRITE를 지원한다． 가지만 "］러한 방식은 많은
몌모리를 사용한다． 이러한 방식을 사용하기 위해 LOB 파일을 선택하기 위해 Query를 사용해야 한다．


盟쓺．'］러한기
      "리를위채QSqlQuery
                “래1에；
                    " "］공가는
                          ""'"""' """""'"() "“버"“수를' "
                                                   ｝요
小 Unix/Linux와 Mac OS X 플랫폼상에서 O I 플러그인 빌드
Oracle l0g에서는 "'Client Package - B" ' ' "Instant Client Package - SDK" 가 필요하다． l0g
                                   "ic과
버전또는그 이人卜   '버전에서는Standard Oracl申 "lient와SDK패키지가필요斗다． liii O1터베 "］스드라
이버 파일을 빌드학기 위해서는 다음과 같은 Or톄cle 라이브러리 파일이 필요하다．

     ·libclntsh. so （모든 Oracle 버전에서 필요）
     ·libwtc9.so (Oracle 9에서만 필요）

Oracle 혜더 파일과 공유 라' ］브러리 파일의 위훠를 qmake7} 인식할 수 있도록 명시한 다음 make 파
일을 실행한다. 다음은 Oracle 9 버전의 예이다.

    cd $QTDIR/ src/plugins/ sqldrivers/ oci
    qmake "INCLUDEPATH+=$ORACLE HO玉恒/rdbms /public $O韶＼CLE HONE/rdbms /demo "
                                                                 n LIBS+=-L$ORACLE HO卜E/lib                                          -lclntsh -1wtc9 " oci .pro
    make



Oracle 10 버전에서는 Client Package SDK 11
이 위치를 지정하고 make를 수행한다．

    cd $QTDIR/ src/plugins/ sgldrivers/ oci
    qmake "INCLUDEPATH+=/usr/include/oracle/ 10.1.0. 3/client! "
                                       "LIBS+=-L!usr!lib! oracle/ lO. l. O .3/ client/ lib                                                    -lclntsh ' oci. pro
    make



만약 Oracle Instant Client package를 ' ｝용해 ' 乍 한다면 I끄LIBRARY PATH 설정 ' ] 필요하다．
OCI 드라이버를 플러그인 형태로 수동으로 설치하기 위해서는 다음과 같은 방법을 사용한다．

[ cd sOT平만斗c/p｝므gins! sqldrivers
  qmaKe 工NCLUD上；PATFI+
                                !oci - .                                                                      .                       .
!                       1nc1uOe/ orac上e/ iU.                                                                 3/ c上ient'
!
                                               =/usr/
                                                                                           .   i.
                                                                                                    0.
        '   L113S+=-L/                 usr/ llb/ orac工e/ 1U.       1.       U.   3/ c上lent/ lib.         ,                   .   .        .       .       .   U,         ,




i     -w上      '   -rpatn,              / USE／上1O/ orac上ei ju           '   t.   u i/ c上ient／上끄）
                                                                                  .                               m          上C上ntsn          -
                                                                                                                                                  上nnz1u           '   oci.   pro
i ma人e




1 윈도우 상에서 0（긔 플러그인을 빌드하기 위한 방법
Oracle    CD로부터             Client Ins申ller에서
                             Install               옵션을 선택한다．
                                                        Oracle                                                 "Programmer                            "                                  Oracle의
버전에 따라 "Call Interface (OCI)" 를 선택하몌 다음과 같은 방법으로 플러그인을 설치할 수 있다．


                                                                                                                                                                                    1 데이터베이스 449


===== PAGE 451 =====
set INCLUDE=%INCLUDE% ;c: \oracle\oci\ include
set LIB=%LIB% ; c: \oracle\oci\ lib\ msvc
cci %QTDIR% \ src\plugins\ sqldrivers\oci
qmake oci. pro
nmake



만약 마이크로소프트어써 제공하는 컴파일러를 사용하지 않는다면 nmake 대신 make를 사용하면 된다．
만약 어플리케이션을 수행하기 위해 추가로 oci. dli 파일이 필요하다. PATH에 다음과 같이 추가한다．

set PATH=%PATH% ; C: \oracle\bin



8ODBC를 지원하기 위한 QODBC
ODBC는 Multiple 데이터베이스 시스템을 연결하기 위한 일반적인 인터페이스이다. Qt에서 제공하는
QODBC 드라이버는 ODBC 드라이버 八4anager어］ 연결을 허용한다. 윈도우 플랫폼에서 0DB（그 드라이
버 Manager는 기본적으로 설치되어 있어야 한다. Un奴凡inux 시스템에서는 ODBC 드라이버
Manager가 설치되어 있어야 한다. 八4icrosoft SQL Server는 저장 프로시저를 실행하고 결과 set을 돌
려준다. Qt에서는 QSqlQuery 클래스에서 제공하는 setForward0nly( ) 함수를 사용하면 된다．

// STORED_PROC uses the return statement or returns multiple result sets
QSqlQuery query;
query. setForwardOnly(true) ;
query. exec ( " {call STORED PROC} " ") ;



小 ODBC UNICODE 지원
QODBC 플러그인은 UNICODE로 정의되어 있는 경우 UNICODE API를 지원한다. 또한 DBMS에서
지원하는 UNI(그ODE를 사용할 수 있다. 어떤 드라이버 Manager에서는 UNICODE를 지원하지 않는다．

이와 같이 UNICODE를 지원하지 않는 드라이버를 사용해 QODBC 플러그인을 사용한다면 Q_ODBC
_VERSION 2가 define되어 있어야 한다. Oracle 9 0DBC 드라이버와 같은 경우에 "SQL_WCHAR
support" 를 확인해야 한다．


eUnix!니flux와 Mac OS X 플랫폼에서 ODBC 플러그인 빌드
Un奴／Linux 플랫폼에서 ODBC를 사용해야 한다면 Un奴ODBC 사용하기를 권장한다. unixODBC의 최
종 버전을 unixodbc. org에서 다운로드 받을 수 있다. un奴ODBC 혜더 파일과 공유 라이브러리 파일을
qmake가 찾을 수 있도록 다음과 같은 옵션을 사용한다．

cd $QTDIR/ src/plugins/ sqldrivers /odbc
qmake "INCLUDEPATH+=/usr/local/ unixODBC/include 'T
                                       n LIBS+=-L/usr/local/ unixODBC/lib   -lodbc "
make




450 CHAPTER 14= 데이터베0난느


===== PAGE 452 =====
S 윈도우 플랫폼에서 ODBC 풀러그인 빌드
플러그인을 빌드하기 위해서 다음과 같은 방법으로 컴파일한다．

        cd %QTDIR% \src\plugins \sqldrivers\odbc
        qmake odbc.pro
        nmake


nfo1a
             ' 「「「c]1A1 1陪
                              『
                              「
                              “
                              '
                                   「   "   「   「哥
                                               "
                                               “'   "   「
                                                            "
                                                             "   『n                  "
                                                                                                         「
                                                                                     "「 「 !? nmake 대J make   A]   -   -"

                                                                                                                           「 ji
                                                                                                                           "｝
                                                                                                                                  '




彷 PostgreSQL을 지원하기 위한 QPSQL(7.3 이상 버전만 사용 가능）
QPSQL 드라이버는 PostgreSQL 7.3 이상 버전에서만 지원한다. QPSQL 드라이버는 PostgreSQL 데
']       터베이스가위치한드라이버를자동으로찾는다．                                        Unicode는서버에서                 지원한다면자동으로사용할수
있다． 만약 "IIOI터베 ' 1스에서 다른 " ncoding을사용한다면 I 1o］터베 " 1스서버는Unicod" 변환을지원
해야 한다. Unicode 지원은 PostgreSQL 7.1 버전 이상에서 지원한다．


心 QPSQL BLOB 지원
PostgreSQL 서버 버전이 7.1 버전 이상에서는
한다．


小 Unix／니flux와 Mac OS X 플랫폼 상에서 （羽SQL 플러그인 빌드
PostgreSQL을 지원斗기 위긔
                  '서 설치된 라" 1브러리와 헤 " ] 파일 ' 1 필요斗다． qmak" 가 설치된 공유 라
이브러리와 헤더 파일을 찾기 위해 다음과 같은 옵션을 사용한다．

        cd $QTDIR/ src/plugins/ sqldrivers/psql
        qmake "INCLtJDEPATH+=/usr/include/pgsqL " 1'LIBS+=-L/usr/lib -lpq" psql .pro
        make



S 윈도우 플랫폼 상에서 QPSQL 플러그인 빌드
윈도우 플랫폼에서 PostgreSQL을 사용하기 위하 다음과 같은 방법으로 플러그인을 컴파일한다．

        Cd %QTDIR% \src\plugins\ sqldrivers\psql
        qmake "INCLUDEPATH+=C: /psql/include "
                                          "LIBS+=C: /psql/lib/ ms/libpq. J.ib " psql .pro
        nmake



S IBM DB2 데이터베이스 연결을 위한 QDB2
Qt에서 지원 IBM DB2 데이터베이스는 플러그인을 사용해 연결이 가능하다. 7.1 이상 버전만 Qt에서 지
원하는 QDB2 플러그인을 컴파일하기 위해서는 IBM DB2 클라이언트 라이브러리를 설치해야 한다．

QDB2 드라' ］버는 BLOB의 RE川功WRITE와 U '1ICODE의 READ/WRITE를 "］원가며 DB2어］" ] 지원
하는 저장 프로시저를 호출할 때1QSqlQuery 클래스의 setForwardOnly( ) 함수 사용을 권장한다．


                                                                                                                  ] 데이터베이스 451


===== PAGE 453 =====
 Unix／니nux와 Max OS X 플랫폼어나］ QDB2 플러그인 빌드

cd $QTDIR/ src/plugins/ sqldrivers/ db2
qmake "INCLUDEPATH+=$DB2DIR/include " "LIBS+=-L$DB2DIR/ lib     -ldb2 "
make



m 윈도우 플랫폼에서 QDB2 플러그인 빌드
윈도우 플랫폼에서 QDB2 플랫폼을 빌드하기 위해 DB2의 클라이언트 라이브러리가 설치된 헤더 파일과
라이브러리 파일을 다음과 같이 명시해야 한다．

cd %QTDIR% \sre\plugins\ sqldrivers\ db2
qmake "INCLUDEPATFI+=<DB2 home> /sqllib/ include '
                                   " LIBS+=<DB2 home> /sqllib/ lib/ db2cli. lib "
nmake



0SQLite 2를 위한 QS（그니TE2
Qt에서 지원하는 SQLite2는 버전 3의 플러그인을 사용한다. 버전 3은 이전 2 버전과 호환성을 가지므
로 \lersion 3 플러그인을 사용해도 된다．


eSQL陀 3를 위한 QS（가JTE
Qt는 SQLite3 플러그인을 지원하며 2 버전과 3 버전을 사용할 수 있다. SQLite는 프로세스 내부에서
동작하는 경량의 데이터베이스이다. 따라서 데이터베이스 서버가 필요하지 않으므로 임베디드 분야에서
주로 사용된다. 또한 SQLite는 메모리 데이터베이스를 지원한다．

만약 SQLite 데이티베이스 내에 데이터를 READ/WRITE하거나 Commit과 Roll back을 하기 위한 트
랜잭션이 발생하면 어플리케이션의 메인 GUI는 멈추는 현상（Freeze）이 발생할 것이다. 따라서
READ/WRITE시 타임아웃으로 인한 리소스 LOCK이 발생하는 부분의 예외 처리가 필요하다. Qt에서
는 타임아웃 처리를 위해 QSqlDatabase 클래스의 set（그onnectionOptions( ) 함수를 제공한다．


1Unix/Linux 플랫폼에서 S（가JTE 플러그인 빌드
SQLite 3 버전은 Qt 내에 Third-party 라이브러리와 같은 INCLUDE되어 있다. 운영체제 플랫폼어］
포함된 SQLite 라이브러리를 사용하기 위해서는 configure 스크립트상에 -system-sqlite 옵션을 사
용할 수 있다. 반대로 그렇지 않은 경우 다음과 같은 방법으로 플러그인을 빌드할 수 있다．

Cd $QTDIR/ src/plugins/ sqldrivers/ sqlite
qmake "INCLUDEPATH+=$SQLITE/include" "LIBS+=-L$SQLITE/lib        -lsqlite "
make




452 CHAPTER 14. 데이터베이스


===== PAGE 454 =====
咎 윈도우 플랫폼에서 S（가JTE 플러그인 빌드

Cd %QTDIR% \src\ plugins\ sqldrivers\ sqlits
qrnake "INCLUDEPATH+=C: /SQLITE/INCLtJDE "     LIBS+=C: /SQLITE/LIB/ SQLITE3.LIB " sqlite. pro
nmake



. QsQ니TE 파일 포맷 호환성 문저1
SQLite 하위 버전에서 때때로 호환성 문제가 발생한다. 예를 들어 SQLite 3.3 버전은 SQLite 3.2 버전
으로 생성된 데이터베이스 파일을 READ할 수 있다. 하지만 SQLite 3.3 버전에서 생성된 데이터베이스
파일은 SQLite 3. 2 버전에서 READ할 수 없다. 따라서 이러한 경우 하위 버전 사이의 파일 호환성과 관
련한 로그 파일 변환 및 문서를 참조하기 바란다．


小 다른 데이터베이스 드라이버의 연결
Qt에서 제공하는 데이터베이스가 아닌 경우 플러그인의 드라이버를 추가하기 위한 방법으로 QSq1
DriverPlugin 클래스를 사용해 드라이버 플러긔인을 제작할 수 있다. QSqlDatabase 클래스는 데이터
베이스와 연결을 위한 기능을 제공하는 클래스아며 데이터베이스 드라이버를 관리하고 로딩하는 역할을
한다. QSqlDriver 클래스는 SQL 드라이버 레이어 기능을 정의하는 상위 클래스이다. 이 클래스에서 구
현된 open( ）과 close( ) 멤버함수와 같이 辛함된 기능은 데이터베이스 연결을 담당한다. 또한
QSqlDriver는 특정 데이터베이스 API어］ 접근하기 위한 QSqlQuery 클래스의 오브젝트를 생성할 수 있
다. QSqlDatabase 클래스는 QSqlDriver어］바로 호출할 수 있는 관련 기능을 제공한다.

QSqlI之esult 클래스는 SQL 데이터베이스 질의를 위한 기능이 정의된 상위 클래스이다. 이 클래스는
SELE（刃, UPDATE와 ALTER TABLE과 같은 SQL 구문을 해석할 수 있는 기능이 포함되어 있다. 즉
QSqlResult 클래스는 ne砒（）와 value( ) 멤버함수와 같은 기능을 포함하고 있다．

QSq11뇨iver와 QSqlResult 클래스는 매우 긴밀한 관계로 연결된 클래스들이다. Qt에서 제공하는 SQL
드라이버는 이러한 각각의 클래스가 추상화된 \[irtual 함수와 하위 클래스로 구현되어야 한다. Qt SQL
드라이버를 구현하기 위해서는 QPLUGIN_METADATA( ) 매크로를 사용해야 한다．

Qt 내에 제공하는 "QTDIR/src/plugins/sqldrivers and QTDIR/src/sql/drivers" 파일을 제공한다．
이 파일은 SQL 플러그인을 제작하기 위한 방법이 포함되어 있다. SQL 드라이버의 플러그인을 개발하기
위한 기본 구조（skeleton)의 소스 코드는 다음과 같다．

class XyzResult : public QSqlResult
{
public:
    XyzResul七（（兀昭t QSqlDriver 火driver)
        : QSqlResult (driver) {}
    사Xyz}之esult ( ) {}


protected:
    QVarian七 da七a(int ／火 index 火／) { return QVarian七（) ; }                                       O



                                                                                1 데이터베이스 453


===== PAGE 455 =====
      bool isNull (int   /* index *1) { return false; }
      bool reset (cons七 QString & ／士 아iery 女／) { re七urn false;    }
      bool fe七（二h (in七 ／火 index 火／) { re七urn false;   }
      bool fetchFirst () { return false; }
      bo（그1 fe七chLas七（) { re七urn false; }
      in七 size ( ) { re七urn 0; }
      mnt numRowsAffected() { return 0; }
      oSqlRecord record() const { return QSqlRecord() ; }
};

class XyzDriver : public QSqlDriver
{
publi（그:
      XyzDriver () {}
      -XyzDriver () {}


      bool hasFeature (DriverFeature 1火 feature *1) const { return false; }
      bool open (cons七 Os七ring & ／出 db 火／r const QS七ring & ／士 user 士／r
                （兀nst Q5七ring & ／士 password 士／r cons七 O5tring & ／士 host; 士／r
                 in七 ／士 port; 士／rconst QS七ring & ／士 options 火／)
           { return false; }
      void close () {}
      QSqlResult *createResult () const { re七urn new XyzResul七（七his) ; }
};



     ti. ? SQL 구문을 사용한 데이터베이스 질의
QSqlQuery 클래스는 SQL 언어를 사용해 데이터베이스어］ 질의할 수 있는 기능을 제공한다. SQL 구문
을 수행하기 위해 QSqlQuery 오브젝트를 생성하고 QSqlQuery 클래스의 exec( ) 함수를 사용한다．

QSqlouery query;
query.exec ( "SELECT name, salary FROM employee WHER丑 salary > 50000 ' ) ;



I Result S이을 이용한 데이터베이스 질의
QS이Query는 레코드의 Result Set을 접근하기 위한 방법을 지원한다. 이 클래스에서 제공하는 exec()
함수를 호출한 다음, QSqlQuery의 포인터가 첫 번째 이전 레코드 포인터에 위치한다. 따라서 첫 번째
레코드를 가리키도록 포인터를 이동하기 위해1next( ) 함수를 사용해야 한다. 또한 다른 레코드어］ 접근하
기 위해 next( ) 함수를 다음과 같이 반복해 사용한다．

while (query.next ( ))
{
      QString name = query.value (0) .toString ( );
      mnt salary = query.value (l) .tolnt ( );
      qDebug( ) << name << salary;




454 CHAPTER 14_ 데이터베이스


===== PAGE 456 =====
QSqlQuery 클래스의 value( ) 멤버함수는 현재 레코드에서 해당 필드의 값을 리턴하는 기능을 제공한
다. C)+＋의 다양한 타입을 지정할 수 있으며 Qt에서 제공하는 QStrii乷과 QByteArray 타입을 사용할
수 있다. 다른 데이터베이스 타입은 Qt 환경어］ 맞도록 자동으로 Mapping 한다．

Qt에서 지원하는 데이터베이스 특징들을 결정하기 위해 QSqlDriver 클래스의 hasFeature( ) 함수를
사용해 지정할 수 있다. 다음 예제 코드는 데이터베이스에서 지원하는 Result Set의 크기를 알아보기 위
한 예제 코드이다．

QSqlQuery query;
mnt nuxnRows;
query.exec ( "SELECT name, salary FROM employee WHERE salary > 50000 ") ;


QSqlDatabase defaultDB = QSqloatabase: :database () ;
if   (defaultDB.driver ( )->hasFeature (QSqlDriver: :QuerySize) ) {
     nur任之ows = query. size() ;
} else    {
     7/ this can be very slow
     query.last () ;
     numRows = query.at () + 1;
}


next( ) 함수와 seek( ) 함수를 통해1Result Set의 결과를 얻을 수 있는지 확인하기 위한 방법으로 QSql
Query 클래스의 setForwardOnly(true) 함수를 사용할 수 있다. 이 함수는 exec( ) 함수를 호출하기 이전
에 사용할 수 있다. 이 방법은 매우 큰 Result Set숄 얻어올 때 최적화 되어 있어 빠르게 질의할 수 있다．


. 데이터 레코드 삽입, 수정 그리고 삭저1
SQL 구문을 수행하기 위해 QSqlQuery 클래스를 사용할 수 있다. 다음은 INSERT 구문을 사용해 테이
블 레코드를 삽입하기 위한 예제 코드이다．

QSqlQuery query;
query.exec ( " INSERT INTO employee (id, name, salary) "
                  "VALUES (1001,      'Thad Beaumont' , 65000) ") ;



만약 많은 양의 레코드를 삽입하기 위한 방법으로 prepare( ) 함수를 통해1 네임 바인딩과 위치 바인딩을
사용할 수 있는 I기aceh아der를 사용할 수 있는 두 가지 방법을 제공한다．

QSqlQuery query;

                                                                      n
query.prepare ( " INSERT INTO employee (id, name, salary)
                  "VALUES (: id,     :name, :salary) ") ;
q口ery.bindValue ( " :id ", 1001) ;
query.bindValue ( " :name ",      "Thad Beaumont ") ;
query.bindValue ( " :salary ",      65000) ;


query.exec () ;



                                                                            1 데이터베이스 455


===== PAGE 457 =====
다음 예제는 포지션 바인딩 기법을 사용한 예제 코드이다．

QSqlQuery 아lery;
query.prepare ( " INSERT INTO employee (id, name, salary)
                                                             11



              "VALUES (? , ?, fl ' ) ;
query.addBindValue ( 1001) ;
query.addBindValue ( "Thad Beaumont ") ;
query.addBindValue (65000) ;
叩ery. exec O;



많은 양의 레코드를 삽입하기 위해1 단지 prepare( ) 함수를 한번만 사용하면 된다. 그리고 해당 레코드의
필드를 지정하기 위해 bindValueO, addBindValue( ) 함수를 사용하고 exec( ) 함수를 수행하면 된다．
성능 측면에서 I가aceholder 방식은 임의의 값을 쉽게 지정할 수 있는 이점이 있다. 다음 예제는 테이블
어］ 레코드를 수정하는 예제이다．

QSqlQuery query;
query.exec ( "UPDATE employee SET salary = 70000 WHERE id = 1003 ") ;



레코드를 수정하기 위해 prepare( ), bindValue( ）와 addBindValue( ) 멤버함수를 사용해 I기ace-
h아der 방식을 사용할 수 있다. 다음 예제는 테이블에 레코드를 삭제하기 위한 예제이다．

QSqlQuery query;
query.exec ( "DELETE FROM employee WHERE id = 1007 ") ;



데이터를 삭제하는 것도 Placeh아der 방식을 사용할 수 있다. 저장 프로시저를 사용하기 위해서 다음과
같은 출력 파라미터 방법을 사용할 수 있다．

QSqlQuery query;
query.prepare ( "CALL AsciiTolnt (? , ?)") ;
query.bindValue (0, "A") ;
query.bindValue (l, 0, QSql: :Out) ;
query. exec O;
m1lt i = query.boundValue(l) .tolnt ( ); II i is 65



Qt는 네 임 바인딩을 사용해 帥4ap과 같은 Bound Value를 처리하기 위해 다음과 같은 Iterator 방법을
사용할 수 있다．

QMaplterator<QString, QVariant> i (query.boundValues (fl;
while (i. hasNext () ) {
    i . next 0;
    cout << i. key0. toUtf8 () .data() << " : "
        << i. value ( ).toString( ).toUtf8 () .data() << endl;
}

바인딩을 통해1QList를 다음과 같이 사용할 수 있다．


456 CHAPTER 14_ 데이터베이스


===== PAGE 458 =====
QList<QVariant> list = query.boundValues () .values ( );
for (mnt i = 0; i < list. size() ; ++i)
    cout << i << ": " << ll st. at (i) .toString() .toUtf8 () .data() << endl;



0 트랜잭션 처리
사용하는 데이터베이스 엔진이 트랜잭션 처리를 지원한다면 Qt에서 제공하는 QSqlDriver 클래스의
hasFeature(QSqlDriver: :Transactions) 멤버함수를 사용해 트랜잭션 처리가 사용할 수 있도록 지정
할 수 있다. 트랜잭션을 초기화 하기 위해 QSqlD爭tabase 클래스의 transaction( ) 멤버함수를 사용하
고 각 트랜잭션에 대한 Comm此을 위해 commitC) 함수를 사용할 수 있다. 또한 특정 트랜잭션의 Roll
back을 처리하기 위해 QSqlDatabase 클래스의 rollback( ) 멤버함수를 사용할 수 있다. 트랜잭션을 사
용하기 위해서는 질의를 하기 전에 트랜잭션을 시작해야 한다. 다음은 트랜잭션 처리를 위한 예제이다．

QSqlDatabase: :database ( ) .transaction() ;
QSqlQuery query;
query.exec ( "SELECT Id FROM employee WHERE name = 'Torild Halvorsen' ") ;
if (query.next () ) {
   mnt employeeld = query.value (0) .tolnt () ;
   query.exec ( " INSERT INTO project (id, name, ownerid) n
                "VALUES (201, 'Manhattan Project ' , n
               + QString: :nun由er (employeeId) + ' ) ' ) ;
}
QSqlDatabase: :database() .commit ( );



Qt에서는 다양한 데이터베이스 시스템의 데이터 타입을 지원한다. 다양한 데이티 타입은 특정 데이터베
이스 시스템에서 사용하는 타입을 지원하기 위한 목적으로 제공한다．

1IBM DB2 데이터 타입

데이터 타입              SQL 타입                                                     추천 타입
SMAL니NT             16나川 nteger                                                아ntl6
INTEGER             32나川 nteger                                                （꾸nt32
미（引NT               64나川 nteger                                                qint64
REAL                32나川 floating 口oint                                        QString
DOUBLE PRECISION    64나川 floating p이ft                                         QString
FLOAT               64나川 floating p이nt                                         OString
CHAR                 Null(종료）이 포함된 Character                                   aString
VARCHAR             Null（종료）이 포함된 String                                       aString
LONG VARCHAR        Null0l 포함되지 않은 Charac伯rString                              OString
BLOB                 Null이 포함되지 않은 4Byte String Length Indicator               QByteArray
CLOB                 Character large string 오브젝트                               QString
DATE                 Nu以종료）이 포함된 Character 앉ring(yyyy-mm-dd)                   QDate
기ME                  NuII(종료）이 포함된 Character String(hh.mm.ss)                  QTime
기MESTAMP             Null0l 포함된 Character 앉ring(yyyy-mm-dd나）h mm.ss.nnnnn n)   ODateTime



                                                                                 ] 데이터베이스 457


===== PAGE 459 =====
 小 B이and InterBase 데이터 타입

 데이터 타입
 BOOLEAN
 기NYINT
 SMALLINT
                     SQL 타입
                     Boolean
                     8 bit Integer
                     16나朮 Integer
                                                           추천 타입
                                                           bool
                                                          이nt8
                                                          이ntl6
                                                                       1
 INTEGER             32寸朮 Integer                         뎨nt32
 BIGINT LONG         64나川 Integer                          대nt64
 REAL FLOAT          32나朮 floating p이nt                    QString
 FLOAT               64-bit 加ating p이nt                   QString
 DOUBLE              64-bit floating point                 OString
 DOUBLE PRECISION    64-bit Double floating point         QString
 VARCHAR STRING      Character string, Unicode            QString
 CLOB                （가）aracter large string 오브젝트         QString
 DATE                yyyy-mm-dd                           QDate
기ME                   hh:mm:ss' in 24나our 포맷              QTime
기MESTAMP             'yyyy-mm-dd hh:mm:ss'                QDateTime


0MySQL 데이터 타입

데이터 타입                SQl. 타입                        추천 타입
기NYINT                8 bit Integer                  typedef 대n侶
기N뮈NT UN미GNED       ,8 bit unsigned integer          typedet quint8
SMAL니NT               16나川 읽gned integer             typedet 이ntl6
SMA나INT UN미GNED      16-bit unsigned integer         typedef quintl6
八T                  」32-bit signed integer           typedet qint32
八T UNSIGNED          32寸朮 unsigned integer           typedef quint32
BIGINT               64寸朮 signed integer             typedef qint64
FLOAT                 32寸朮 디oating P이nt              QString
DOUBLE               64-bit Floating Point           QString
CHAR                 Character string                QString
VARCHAR              Character string                QString
기NYTEXI              Character string                QString
TEXT                 Character string                QString
MED띠MTEXT            Character string                QString
LONGTEXT             Character string               i QString
CLOB                 Character large string 오브젝트     QString
all BLOB types       BLOB                            QByteArray
DATE                 Date                            QDate
DATE기ME              Date와 Time                      QDa怡Time
기MESTAMP             Da也와 Time                       QDatelime
기ME                  Time                            Qlime
YEAR                iYear(int)                       QDateTime
ENUM                 Value 5et21 Enumeration         QString


458 CHAPTER 14.. 데이터베이스


===== PAGE 460 =====
小 아acle 데이터 타입
데이터 타입         SQL 타입                                      추천 타입
NUMBER         FLOAT. DOUBLE, REAL                         QString
NUMBER(38)     INTEGER 八T SMA나INT                          qint8/16/32/64
NUMBER(p,s)    NUMERIC(p,s) DECIMAL(p,s)                   QString
NVARCHAR2(n)   Character string (NATIONAL C HARACTER       QString
               VARYING(n) NATIONAL CHAR VAR눠NG(n)
               NCHAR VARYING(n))
NCHAR(n)       Character string (NATIONAL 1 HARACTER(n)    QString
               NATIONAL CHAR(n) NCHAR(n)
CHAR(n)        Character string (CHARACTE ' (n) CHAR(n))   QString
CLOB           Character large string 오브젝＝                 QStri ng
BLOB           A binary large object                       QByteArray
기MESTAMP       Year, month, Date day values hour, minu旭，   QDat이ime
               그리고 time second values


1ODBC 데이터 타입

1데이터 타입        SQL 타입                                      추천 타입
텨T             Boolean                                     BOOL
기NYINT         8 b仕 nteger                                 데nt8
SMAL［그NT       16나川 引gned integer                          액ntl6
INTEGER        32-bit signed integer                       대nt32
텨（引NT          64나川 히gned integer                          qint64
REAL           32나기t t幻ating p이nt                          QSt ring
FLOAT          64나이tDoub冶 floating p이nt                    QString
DOUB［三         64나川 Doub冶 floating p이nt                    QString
CHAR           Character string                            QString
VARCHAR        Character string                            QString
LONGVARCHAR    Character string                            QString
CLOB           Character large string object               QString
DATE           Character string                            QDate
TIME           Character Time, Character sti'ing           Q기me
TIMESTAMP      Character Time, Character st Ping           QDateTime


0PostgreSQL 데이터 타입
데이터 타입         S（그L 타입                                     추천 타입
BOOLEAN        Boolean                                     bool
SMAL니NT        16나川 引gned integer                          대ntl6
八TEGER         32寸朮 signed integer                         대nt32
BIGINT         64-bit signed integer                       대nt64
REAL           32나it floating p이nt                         OString
DOUBLE         64-bit floating point                       QString
PRECISION


                                                                            1 데이터베이스 459


===== PAGE 461 =====
 톄이터 타입         SQL 타입                                              추천 타입
 DECIMAL        사용자 지정                                               OString
 V사귀ABLE
 NUMERIC        사용자 지정                                               QString
 VAF킨ABLE
 VARCHAR       character string
                                                               나山
                                                                    QString
 CHARACTER     Character string                                     QString
 TEXT          Character string                                     QString
 CLOB          Character large string 오브젝트                          OString
 기MESTAMP      8 byte Date와 Time을 포함                                ODateTime
 DATE          4 byte Date                                          QDate
 기ME           8 byte Time (00:00:00.00 - 23:59:59.99)              QTime
기ME            12 bytes Time zone 00:00:00.00+12                    QDateTime


勿 SQL陀 3 데이터 타입

데이터 타입         SQL 타입                                               추천 타입
NULL           NULL value                                           NULL
 八TEGER        8, 16, 24, 32, 48 또는 64나川 Integer                    대nt町16/32/64
REAL           64寸朮 floating point                               QString
TEXT           Character string (UTF-8, UTF-16BE or UTF너6-LE). 1 QString
CLOB           Character 나ge string 오브젝트                            QString
BLOB           입력된 값 그대로 Binary로 저장                                 QByteArray


0Sybase Adaptive Server 데이터 타입

데이터 타입         S（그［ 타입                                              추천 타입
미NARY          고정된 255 byte                                         QByteArray
CHAR           Character String                                     QString
DATETIME       Date와 time (1753-01-01 00:00:00 through              QDateTime
               9999-12-31 23:59:59)
                                                               1
NCHAR          Character String                                     QString
NVARACHAR      Character String                                     QString
VARCHAR        Character String                                     QString
CLOB           Character large string 오브젝트                      ! QString
기MESTAMP       데이터베이스에서 Uni꾸je number                               QString
SMAL上DATE기ME   Date2F time (1900-01-01 00:00 through 2079-          QDat酊ime
               12-31 23:59)
비미CHAR         Character String (Unicode)                           QString
UNIVARCHAR     Character String (Unicode)                           QString
VAR미NARY       가변의 미nary value （최대 255 byte)                   ;QByteArray




460 CHAPTER 14 데이터베이스


===== PAGE 462 =====
     tm, Model 클래스
Qt는 QSqlQuery 뿐만 아니라 데이터베이스어］ 접근해 데이터를 READ/WRITE 하기 위해 다음과 같은
모델 방식의 클래스를 제공한다．

클래스                       설명
OSqiQueryModel            임의의 S（그［ 질의를 REI D하기 위한 모델 방식
OSqiTableModel            단일 테이블상에 데이터를 READ/V뱌기TE 하71 위한 모델 방식
OSqIR이ation쉐TabIeI加del    외부키（Fo回gn key）를 지원하는 oSqlTableMod이의 하위 클래스



이 클래스들은 QAbstractTableModel 클래스로부터 상속받은 클래스들이다. 데이터베이스에 접근해
가져온 데이터를 READ/WRITE하기 위해 QListView 클래스와 QTableVeiw 클래스 같은 아이템
VIEV/ 클래스 위젯의 아이템 데이터와 쉽게 연결할 수 있다．

                                                        "기 위해 파
'］러한클래스는또 다른 이점으로 "110］터베 "］스韋부터 읽어온 15110］터를XML파일어］ '］장4
일 포맷으로 변환하기 쉽다. 또한 데이터베이스에 접근해1 데이터를 READ/WRITE하기 위한 방식을 쉽
게 구현할 수 있다．


1QSqIQue四Model 클래스가 제공하는 데이터베이스 모델 방식
                                                          수
QSqlQueryModel 클래스는 데이터베이스에 접근해 READ한 데이터를 모델 방식으로 쉽게 구현할
있다. 다음 예제는 SQL 질의상에서 모델 방식을 사용한 예제이다．

 QSqlQueryModel model;
 model. setQuery ( "SELECT * FROM employee ' ) ;


 for (mnt i = 0; i < model.rowCount () ; ++i) {
     mnt Id = model.record(i) .value ( "id ") .to]int () ;
     QString name = model.record(i) .value "name " ) toString( ) ;
      qDebug() << id << name;
 }


QS아QueryModel 클래스가 제공하는 setQuery( ) 멤버함수를 통해 SQL 질의를 설정하고 record(int)
멤버함수를 호출하면 데이터베이스에 저장된 테이블의 레코드를 읽어올 수 있다．


0OSqiTable卜加del 클래스를 이용한 모델 방식
QS이TableModel 클래스는 데이터베이스상의 단일 테이블의 레코드를 READ/WRITE 할 수 있는 기능
을 제공한다．




                                                                       ] 데이터베이스 461


===== PAGE 463 =====
 QSqlTableModel model;
 model. setTable ( "employee ") ;
 model. setFilter ( "salary > 50000 ") ;
 model. setSort (2, Qt: :DescendingOrder) ;
 model. select ( );


 for (mnt i = 0; i < model.rowCountU; ++i) {
     QString name = model.record(i) .value( "name" ) .toStrlng() ;
      mnt salary = model.record(i) .value ( "salary ") .tolnt () ;
      gDebug() << name << salary;
 }


QS아TableModel 클래스는 각각의 SQL 테이블을 검색과 수정할 수 있는 기능을 제공하며 SQL 문법
지식이 없더라도 테이블상에 데이터를 읽어올 수 있다. 테이블에 저장된 레코드를 record( ) 함수를 통해1
데이터를 읽어올 수 있으며 setRecord( ) 함수를 사용해 각 행의 레코드를 수정할 수 있다. 다음 예제는
employee 테이블의 salary 필드의 값을 10퍼센트씩 증가하기 위한 예제이다．

 for (mnt i = 0; i < model. rowCountU; ++i) {
     QSqlRecord record = model.record(i) ;
     double salary = record. value ( "salary ") .tolnt () ;
     salary 士= 1.1;
     record. setValue ( " salary", salary) ;
     model. setRecord(i, record) ;
 }
 model. submitAll() ;



QAbstractltemModel 클래스로부터 상속받은 data(）와 setData( ) 함수를 사용할 수 있다. 다음 예제
는 setData( ) 함수를 사용해 레코드를 업데이트하는 예제이다．

model. setData(model.index (row, column) , 75000) ;
model. submitAll() ;



다음 예제는 레코드를 삽입하기 위한 예제이다．

model. insertRows (row, 1) ;
model. setData(model.index (row, 0) , 1013) ;
model. setData(model. index (row, 1) , "Peter Gordon") ;
model. setData (model.index (row, 2) , 68500) ;
model. submitAll() ;



뎨이터를 일괄 삭제하기 위한 방법으로 다음과 같은 방법을 사용할 수 있다．

model. removeRows (row, 5) ;
model. submitAllO;



462 CHAPTER 14= 데이터베이스


===== PAGE 464 =====
removeRows() 함수의 첫 번' 1 인' ｝는 테 ' ］블상에서 삭' 1］할 첫 번째 Index0］며 두 번째 인자는삭" 카할
레코드의 개수를 의미한다． subm土A끄（) 함수는레코드 변경 " ] 완료되면 "｝지막에 항상호출＝
                                                      " 乍 " 11O1
터베이스상에 적용된다.

테이블의 수정이 완료되면 subm代A11( ) 함수를                                  변경된 데이터를 적용하기 위해 이 함수를 호출
해야 한다. 수정한 데이터를 적용하는 방식 중                                      it로 OnRowChange의 enum값이 설정된다．
OnRowChange는 사용자가 선택한 레코드가 더］뎨터베이스어］ 변경이 있을 때 적용된다．

0小[anualSubmit은 submitAll( ) 함수가 되7 선까지 데이티베이스 변경이 적용되지 않는다. 마지막
으로 oi伊ieldChange는 VIEW 상에서 사용하7                        1   합한 방식이다. 이 방식은 submitAll( ) 방식을 호출
할 필요가 없다. 이 방식은 Cachii培을 사용하지                          기 때문어］ 성능이 떨어질 요소가 있다．


小 QSqlReIa的nalTa비e入加del 클래스를 이용한 모델 방식
QSq1R이ationaiTableModel 클래스는 외부키를 지원하는 QS아TableModel 클래스의 확장된 클래스
이다. 하나의 테이블의 필드와 다른 테이블의 Primary key로 지정된 필드를 1:1 Mapph乷을 위한 외부
키 (Foreign key）를 지원한다．

          N카ne         city     Coo           1D

  ]       Es口en    昑01          3'                     ospen    Oslo          Norway

2 2                      . --   4크                     Hara     mai而굶y
                                         b
                   s
                                         1:
  3       Sam      103          1                      Sam      San    Jose   USA
                                                   小




（그림 ) Foreign Key 설정 화면



다음 예제 코드는 QSq1I扼lationalTableModel 클래스를 사용해 외부키를 설정하기 위한 예제이다．

 model->setTable ( rr employee1' ) ;


 model->setRelation(2, QSqlRelation ( " city 1 r nidn, rrnamerr ) );
 model->setRelation(3, QSqlRelation ( "couri :ry" r U idn r rr name" ) ) ;



setRelation( ) 함수는 테이블 사이의 Relatio                     설정하기 위해 호출하며 employee 테이블과 city 테
이블의 두 번째 Field 필드를 지정한다. 이와 동일한 방법으로 3번째 필드를 설정한다．

READ/WRITE가 가능한 QSqlRelationalTableModel 클래스를 사용하면 GI끄를 제공하는 VIEW 상
에서 QSqlRelationalDelegate 클래스를 사용할 수 있다. 이 클래스는 사용하면 VIEW 상에서 Combo
bo ( 위젯을 제공한다．

 QTableView *vjew = new QTableView;
 view->setModel (model) ;
 view->setltemDelegate (new oSqlRelationalDelegate(view) );




                                                                                       ] 데이터베이스 463


===== PAGE 465 =====
           司Relation키Tab노MOd-.                                                                   枉m ' 尸多쯔
                  ID                Name                                                  City          Country
           11               Espen                O引o                                                N（玎way

            22              由：
                             出d                  曲mm帥叩y
            33
             3              Sam
                            53m                                                                     USA
                                                 San
                                                                               ,ose
                                                                                      J
                                                 Osl。
                                                 Munich
          뇨＝    =＝二二二그＝ 二：
                         二二：二；
                             ;＝二二二二二드                                          뇨




          （그림） R이ation Table Model 예제 실행 화면




                 ,, 1.5) Table View의 활용

          QSqlQueryModel, QS아TableModel, QSqlRelationalTableModel 클래스는 Qt에서 제공하는
          QListView, QTableView, QTreeView와 같은 VIEW상에 뎨이터를 표시하는 방법을 제공한다．

           U그 Re1at山nal Tab匣 ＼化del                                                                                   다 回 k叫
                       ID                 Name                                                   City              Country
           11                       已pen                                                  Os匕                卜］orway

           22                       Harald                                                                   Germany

                                    Sam                                                   San 幻5e
                                                                                                             USA




（그림） QTableView를 사용한 예제 실행 화면



          SQL 데이터 모델 방식 기반 VIEW를 생성하기 위해 다음과 같이 QTableView 클래스 위젯을 사용할 수
          있다．

          QTableView *view = new QTableView;
          view->setaodei (inodel) ;
          view->show() ;



만약 READ/WRITE를 지원하는 모델 방식인 경우 필드를 수정할 수 있는 기능을 제공하기 위해
    setEdit Triggers( ) 함수를 사용할 수 있다．

iview牛＞
                   Se七Edi七Triggers                     (Qlths七ract工七emVies寸：
                                                                                                                         :No且di七Triggers) ;




여러 개의 \1iew에서 데이터를 동일한 방식을 사용해 특정 데이터를 수정하기 위한 방식을 제공한다. 모
델의 헤더 제목을 설정하기 위해 setHeaderData( ) 함수를 사용할 수 있다. 이 함수를 사용하면 헤더 제
목을 설정할 수 있다．




464 CHAPTER 14_ 데이터베이스


===== PAGE 466 =====
model->setHeaderData (0, Qt: :Horizontal, QObject: :tr ( "ID") );
model->setHeaderData ( 1, Q七：냐幻rizon七al, QObjec七：比r ( "Name " ) ) ;
model->setHeaderData ( 2, Q七：:Horizon七al, QObject: 比r ( "Ci七y ', ) ) ;
model- >setHeaderData (3, Q七：: Horizon七al, QObjec七：：七r ( !' Coun七ry" ) ) ;



QTableView 클래스 위젯은 세로 축의 하더 제목을 설정할 수 있다. 그리고 VIEW 상에서 레코드 행이
수정되어 submitAll( ) 함수가 호출될 필요가 있을 경우 Asterisk（끼와 같은 표시를 제공하는 G｛끄를 제
공한다．다음 예제 실행 화면은 새로운 레코드 행이 추가된 예제 실행 화면이다．

:：小 中．..．弦萍于，寸也 . ，山 ' n나謐imi如知亂蜘료二玉 出；址낳蠶群나n二 1   Country各磊3多‘
     1             Espen          O引0              Norway

     2             Hara닌          Munich           Germany

     4               1     =      San 戶se

     3             Sam            San戶se           USA

（그림） 삽입된 예제 실행 화면



마찬가지로 레코드 행이 removeRows( ) 함수에 의해1 삭제된 경우 subm此A11( ) 함수가 실행되기 전까
지 K!) 표시를 제공한다．

Delegate를 사용해 VIEW에 표시된 아이템은 디폴트로 QltemDelegate로 설정되어 있다. 이 디폴트
설정은 int, QString, Qlmage 등과 같은 데이터 타입의 핸들링이 가능하다. 또한 Combo Box와 같은
에디트 위젯에서 제공하는 위젯상어］ 데이터를 표시하는 기능을 제공한다．

QS아TableModel 클래스는 단일 테이블 상에서 임의의 테이블에서 READ/WRITE가 가능하도록 최적
화되어 있으며 flag(）와 setData( ) 함수를 사용해 쉽게 구현할 수 있다．

 Qt: :ItemFlags EditableSqiModel: :flags (
              cons七 아幻dellndex &index) cons七
 {
         Qt: : ItemFiags flags = QSqlQueryModel: : flags (index) ;
         if   (index.column() == 1 1 1 index.column() == 2)
              flags 1= Qt: :ItemIsEditable;
         return flags;
 }

 bool EditableSqlModel: :setData(const QModellndex &index, const QVariant &value,
 mnt ／士 role 士／)
 {
         if   (index.column() < 1 I I index.column() > 2)
              return false;


         QModellndex primaryKeylndex = QSqloueryModel: : index (index.row ( ), 0) ;
         in七 id = da七a (primaryKeyIndex)．七（D1n七（ ) ;                                       0




                                                                                  ] 데이터베이스 465


===== PAGE 467 =====
     clear () ;


     bool Ok;
     if (index.coluxnn() == 1) {
         ok = setFirstName (id, value.toString() );
     } else {
         Ok = setLastName (id, value.toString() );
     }
     refresh() ;
     return Ok;




다음 예제는 setFirstName( ) 함수를 통해 레코드를 수정하는 예제이다．

bool EditableSqlModei: :setFirstName (int person工d, const QString &firstNarne)
 {
     QSqlQuery query;
     query.prepare ( " update person set firstname = ? where id = ? '1 ) ;
     query. addBindValue ( firstName) ;
     query. addBindValue ( personld) ;
     return query.exec () ;




     1.6      S（그［- 레코드 필드와 GUI 위젯 매핑

QSqlQueryModel, QSqlTableModel, QSqlRelationalTableModel 클래스를 이용해 VIEW 상에 데
이터를 표시하는 방법은 각 레코드 단위로 아이템을 상세히 표시하기에 부족하다. 하지만 Qt에서는 GUI
폼（Form) 기반의 테이블의 각 레코드를 상세히 표시할 수 있는 기능을 제공하기 위한 목적으로
QDataWidget八flapper 클래스를 제공한다．

QDataWidgetMapper 클래스는 데이터베이스 테이블 상에서 각각의 아이템을 八flapping 할 수 있도록
각각의 레코드를 아이템으로 처리할 수 있다. SQL 모델과 함께 QData＼肌dgetMapper 클래스를 사용하
면 아주 심플한 방식으로 데이터 폼을 표시하는 GI끄를 제공할 수 있다．




466 CHAPTER 14_ 데이터바이스


===== PAGE 468 =====
      Id    rmnm          咐as客           tyrmi1出x   녑 desa如h이1
                   123 MW' 由的
      1     A玭0    MW似 I的1                 101      101 Home
                   P0 B0工 32
      2     Bob    Ms寸 HI.寸19 鈿Vm          102      102 Work
      3     Car이   TIlO U9hV,o4e
                   Pm.目I. IllS너            103      103 Other
                   4733$ PI.II AV1yHJ0
      4 Donaic     B口 C.ty                 101
                   R口$4甘oh 琡$1心1
      5 Emma       B心Sc斗1叩                 103




       Name:       Car이

          Ad마as客 The Ugh小ouse
                 Remote I引and




（그림） SQL Widget Ma口口er 예제 실행 화면



Q（그Omb oB O ' 위젯과 八4apping Name 위젯읕 ' ｝용채
                                        ' "n "］터와 위젯을 Mapping가는 예 "{］이다．
Combo box는 Home, Work, Othe" 중 차나를 선택할 수 있으며 id와 typeinde" 간의 동일한 레코드
값을 이용해 데이터를 표시한다. 다음은 예제의 해더 파일이다．

 class Window : public QWidget
 {
    Q OBJECT
 public:
             Window ( QWidget; 枉埴rent; 客                ;

 private slots:
             void updateButtons (mnt row) ;
 private:
             void setupModel ( );
             QLabel *na1[teLabel;
             QLabel *addressLabel;
             QLabel *typeLabel;
             QLineEdit * naineEdit;
             QTe＞比Edit; 火address風虹幻
             QCon止）oBox 火typeCor［止）oB（그X;
             QPushBu七七on 出nex七But七on;
             QPushButton *prevjousButton;


             QSqlRelationalTableModel *model;
             QltemSelectionModel *selectiop4odel;
             QDataWidgetMapper *mapper;
             mnt typelndex;
 };
                     '와사용자인터페 "］스를구성가는카
QDataWidgetMapper클래스객기                " ' ｝용한Control은 ' ｝용"｝인터
페이스를 제공하기 위한 목적으로 구현되었으며 테이블 각각의 데이터 레코드를 적용할 수 있도록


                                                                 l 데이터베0匹 467


===== PAGE 469 =====
Address의 타입과 관련한 정보를 QStringListModel로 지정한다．


첫 번짜匠 쌍성자에서는 예제 데이터로 사용할 모델 방식을 설정한다. 모델은 sett叩Model( ) 함수에서
초기화되며 SQLite 데이터베이스에 포함된 "person" 테이블을 생성하고 생성한 테이블에 데이터를 삽
입한다. 그리고 primary key, name, address와 각 필드의 타입을 설정한다．

void Window: :setupModel()
{
     QSqlDatabase db = QSqlDatabase: :addDatabase ( "QSQLITE") ;
     db.setDatabaseName ( " :memory: ") ;
     if ( 1db．아尼n( ) ) {
          QMessageBox: :critical ( 0, tr ( "Cannot open database '1 ),
              tr ( "Unable to establish a database connection. \n"
                      "This example needs SQLite support. Please read '
                                                                                H
                      "the Qt SQL driver documentation for information how
                      "to build it. ") , QMessageBox: :Cancel) ;
            return;
     }

     QSqlQuery query;                                                  ＝斗m口＝
     query.exec ( "create table person (id mnt primary key, "
                  "name varchar (20) , address varchar (200) , typeid int) ") ;
     query.exec ( "insert into person values (1, 'Alice ' , H
                  1' 1 <qt>123 Main Street<br/>Market Town</qt>' , 101) ' ) ;
     query.exec ( " insert into person values (2, 'Bob' , "
                  " '<qt>P0 Box 32<br/ >Mail Handling Service"
                  "<br/>Service City</qt>' , 102) ") ;
     query.exec ( "insert into person values (3, 'Carol' , n
                  n 1 <qt>The Lighthouse<br/ >Remote Island</qt>' , 103) ") ;
     query.exec ( "insert   into person values (4, 'Donald' , "
                  " '<qt>47338 Park Avenue<br/ >Big City</qt>' , 101) ") ;
     query.exec ( "insert into person values (5, 'Emma' , "
                      " '<qt>Research Station<br/>Base Camp<br/ >'
                      "Big Mountain< /qt>' , 103) " ) ;



테이블의 각 행은 분리된 테이블과 일치시키기 위해 Address 타입을 포함하는 각 레코드에 typelndex
와 id 필드가 동일하도록 저장한다．




                                           回回回回
口m                ad山텨ig        lv的index


IIm1m       123 Ma,r, Street
            M日Iltet T帥기           101         卜伯me

目 B야）       P0 Box 32
            M04 Ham工 .5酊W（刃       102             叭幻rk

回 Car이      Tho L9ttth伽so
            Remote 四Is,너
            47338 Park Avenue
                                  103             Other
 4 ［沁nald   B, Cr1                101

目曲          Rexoarch Slatror,
            Base                  103

Addresstype 테이블을 생성하고 person 테이블과 필드 값이 일치하도록 테이블 레코드를 다음과 같이
추가한다．


468 CHAPTER 14_ 데이터베이스


===== PAGE 470 =====
   query. exec ( "create table addresstype
                             (Id mnt1 description varchar (20) )") ;
    query. exec ( "insert into addresstype values (lOl, 'Home ' )") ;
   query. exec ( "insert into addresstype values (102, 'Work ' )") ;
   query.exec ( " insert into addresstype values (103, 'Other ' ) ") ;


   model = new QSq1Rela七如nalTableModel（七hi引 ;
   model->setTable ( "person") ;
   model->setEditStrategy ( QSqlTableModel: : OnManualSubmit) ;


   typelndex = model->fieldlndex ( "typeid") ;
   model->setRelation ( typelndex,
          QSqlRelation ( " addresstype ", "id ",   "description" ));
   model->select () ;




person 테이블의 typeid 필드는 addresstype 테이블의 내용과 관련이 있다. 이러한 관계는 이전어］ 설

명한 QSqlRelationalTableModel을 경유채       '   섶정한다．
                                                    person
                                                             태 ' ］블의 typeid   필드와
                                                                                      addresstype
                                               '1 각 위젯과 " 11 ］터 모델을
터IcDI블에서 "d 필드는 서로 관계를 맺는다． 사용자 인터페 "］스를 제공가기 위레
설정하기 위하1 다음과 같이 예제 코드를 작성한다．

Window: :Window(QWidget *parent)
    : QWidget (parent)


    setupModel ( ) ;


    nameLabel = new QLabel (tr ( "Na&me: " ));
    nameEdit = new QLineEdit () ;
    addressLabel = new QLabe1(tr ( "&Address: ") );
    addressEdit = new QTextEdit () ;
    typeLabel = new QLabel(tr ( " &Type: ") );
    typeCorr由oBox = nei寸 QCor吐）oBox ( ) ;
    ne）比跏比on = new QPushBut土on ( tr ( "&Nex七11 ) ) ;
    previousButton = new QPushButton (tr ( "&Previous ") );


    nameLabel->setBuddy ( nameEdit) ;
    addressLabel->setBuddy ( addressEdit) ;
    typeLabel->setBuddy ( typeComboBox) ;



GUI상에서 모델 방식을 combo box와 연결가기 위개 typeid 필드와 연관관계를 맺는다． Combo box
의 해당 필드가 선택되면 setModelColumn( ) 함수가 호출된다．




                                                                                    ] 데이터베이스 469


===== PAGE 471 =====
      QSqlTableModel *relModel = rnodel->relationNodel(typelndex) ;
      typeComboBox->setModel ( relModel) ;
      typeComboBox->setModelColuisn(relModel->fieldlndex ( "description' ));


      mapper = new QDataWidgetMapper (this) ;
      mapper->setModel (model) ;
      mapper->setltemoelegate (new QSqlRelationalDelegate (this) );
      mapper->addNapping(nameEdit, model->fieldlndex ( "name' ));
      mapper->addNapping(addressEdit, model->fieldlndex ( "address ") );
      mapper->addMapping ( typeCoinboBox, typelndex) ;



setModel( ) 함수로부터 필드의 index가（兀mbo box 위젯에 설정되어 있다. typeid 값과 일치하는 값
을 入4appii培시키기 위해1QSqlRelationalDelegate 클래스를 사용한다．

     connect (previousButton, SIGNAL(clicked() ), mapper, SLOT (toPrevious () ));
     connect (nextButton, SIGNAL (clicked() ), mapper, SLOT (toNext () ));
     connect (mapper, SIGNAL (currentlndexChanged(int) ),
                                          七his, SLOT (upda七eBut土（:)ns (in七）) ) ;

     QGridLayout *layout = new QGridLayout () ;
     layout->addWidget (nameLabel, 0, 0, 1, 1) ;
     layout->addWidget (nameEdit, 0, 1, 1, 1) ;
     layout->addWidget (previousButton, 0, 2, 1, 1) ;
     layout->addWidget (addressLabel, 1, 0, 1, 1) ;
     layout->addWidget (addressEdit, 1, 1, 2, 1) ;
     layout->addWidget (nextButton, 1, 2, 1, 1) ;
     layout->addWidget (typeLabel, 3, 0, 1, 1) ;
     layout->addWidget (typeComboBox, 3, 1, 1, 1) ;
     setLayout ( layout) ;


     setWindowTitle(tr ( "SQL Widget Mapper ") );
     mapper->toFirst () ;




updateButtons( ) 함수는 현재 위치하고 있는 데이터의 index7} 표시가능한지 확인하기 위한 함수이다．

 void Window: : updateButtons (mnt row)
 {
     previousBut尤（>1l小＞setEnabled ( r （그i寸 > 0) ;
     nextButton->setEnabled(row < model->rowCount () - 1) ;
 }




470 C니APTER 14山 데이터베이스


===== PAGE 472 =====
                      tj7 Cached 테이블 예제
Cached테이블예제
                                         어플리케이션은사용자가야-JI상에배치된［Submit］버튼을클릭하기 전까지 변경
된 ]O1
   1O1터를 캐시（Cache）에서 수정이 이루어진다． O1 예 ' II는 Qt가 설치되면 예 " 11에 포함되어 있으며
TableEdito" 단일클래스로구성되어 있으며 사용자가 " 가 O1터베 " 1스에 접근개 " 가 O1터를수정할수있는
다이얼로그 GUI를 제공한다.



                                  Fir뵤 name

                             Denny




（그림） Cached Tab冶 예제 실행 화면



  TableEditor 클래스는 QDialog 클래스로부터 상속받' } 구현된 테 " 1블 에디터 위젯' ］다． 예 ' 1］의 헤 " ]
파일 구조는 다음과 같다．


              class TableEditor : public QWidget
              {
                       Q OBJECT

              pubi뇨二 :
                       explicit      TableEditor (const QString &tableName, QWidget *parent = 0) ;


              private slots:
                       void subinit () ;


              private:
                       QPushButton * submitButton;
                       QPushButton *revertButton;
                       QPushButton 抑iui七Bu七七on;
                       QDialogBut土onBox 싸m比onBox;
                       QSqlTableModel *model;
                  ;


          TableEditor 클래스의 생성 ' ｝는두 ' II의 인자를사용한다． 첫 번째 인자는 "카 ' ］터베 "］스의 테 "］블을 참
       조하기 위한 인자이다. 두 번째 인자는 부모 위젯의 포인터이다．

          QS아TableModel 클래스는 VIEW 클래스인 QThb1eView 위젯에 데이터를 연결하기 위한 모델을 제공


                                                                                                     ] 데이터베이스 471


===== PAGE 473 =====
한다. QSqlTableModel 클래스는 단일 테이블상에 데이터의 READ/WRITE가 가능한 모델 방식이다．
QSqlQuery 클래스는 SQL 구문을 사용해 데이터베이스에 저장된 데이터를 조작하기 위한 기능을 제공
한다．


TableEditor 클래스를 사용하기 전에 에디트상에 READ할 데이터베이스와 연결해 테이블을 생성해야 한
다. 테이블을 생성하기 위해 다음과 같이 createConnection( ) 함수를 먼저 실행시켜 테이블을 생성한다．
그리고 생성한 테이블에 레코드를 삽입한다. 먼저 main( ) 함수에 다음과 같이 소스 코드를 작성한다．

mnt main(int argc, char *argv[ ])
{
      QApplication app(argc, argv) ;
      if (! createConnection() )
          return 1;
      TableEditor editor ( n person " );
      editor. show ( );
      return app.exec () ;
}


어플리케이션을 실행하면 처음 createConnection( ) 함수가 실행된다. 이 함수는 예제에서 사용할 테이
블을 생성하고 테이블에 데이터를 삽입한다. 그리고 테이블과 데이터 삽입이 정샹적으로 완료되면 true
값을 리턴한다. createConnection( ) 함수에 대한 소스 코드는 예제 코드에 포함되어 있으므로 참고하
기 바란다．

S七a七ic bool crea七eConnec七ion( ){
      QSqlDatabase db = QSqlDatabase: : addDatabase ( "QSQLITE") ;
      db. setDatabaseName ( " :memory: ") ;                             1
      if ( !db．아冶n( ) ) {
          QMessageBox: :critical (O, qApp->tr ( "Cannot open databasen ),
             qApp->tr ( "Unable to establish a database connection. \n"

          return false;
      }

      QSqlQuery query;
      query.exec ( "create table person (id mnt primary key, n
                   "firstname varchar (20) , lastnaxne varchar (20) )") ;
      query.exec ( "insert into person values ( 101, 'Danny ' , 'Young )") ;




TableEditor 클래스는 단지 생성자와 submit( ) 슬롯함수로 구성되어 있다. 생성자에서 데이터 모델을
설정하기 위한 소스 코드가 포함되어 있다．




472 CHAPT타긋 14 데이터베이스


===== PAGE 474 =====
TableEditor: :TableEditor (const QString &tableName, QWidget *parent)
    : QWidget (parent)
{
    model = new QSqlTableModel (this) ;
    model->setTable ( tableName) ;
    model->setEditStrategy (QSqlTableModeJ : : OnNanualSubmit) ;
    model->select () ;


    model->setHeaderData(O, Qt: :Horizontal, tr ( "ID") );
    model->setHeaderData(l,    Qt: :Horizontal, tr ( "First name") );
    model->setHeaderData(2, Qt: :Horizontal, tr ( "Last nalne"fl;



첫 번째로 데이터 모델을 설정하기 위해 데이터베이스 테이블을 설정한다. 테이블을 설정하기 위해
setTable() 함수를호출한다． 그리고 "etEditStiategy() 함수는 submitol c,］루어지기 전까' 1 0110］터
베이스에 적용되지 않는다.

Select( ) 함수는 데이터베이스 QTableView                   데이터를 READ한다. setHeaderData( ) 함수는
QTableView의 헤더 제목을 설정할 수 있는 기능을 제공한다．

    QTableView *view = new QTableView;
    view->setNodel (model) ;
    view->resizeColumnsToContents () ;



QTableView클래스는 "카이티베이스에 '］장된申 '］터를Model/View기반방식을 ' ］용채
                                                      'View위젯
과연결가기 위한위젯을 ' 카공한다． 그리고GUI상에서 사용할［Submit], [Revert］그리고［Quit] 버튼
위젯을 배치하기 위해 다음과 같이 소스 코드를 작성한다．

    submitBut七on = nei了 QPushBu七七on(tr ( " Submit少 ) ) ;
    submitButton->setDefault (true) ;
    revertButton = new QPushButton(tr ( "&:Revert ") );
    quitButton = new QPushButton(tr ( "Quit " ) );


    buttonBox = new QDialogButtonBox (Qt: :Vertical) ;
    bu比onBox수addBu七七on(submitB毗七on, Qoialogsut土onBox: :ActionRole) ;
    bu七七onBox中＞addBut土on ( rever七Bu七ton, QDialogBut尤onBox: :Ac七ionRole) ;
    bu七七onBox->addBu七七on (quitBu七七（Dn, QDialogBu比onBox: :Rejec七Role) ;



[Submit] 버튼은 테이블 \hiew어］ 수정된 내용을 데이터베이스에 저장하기 위한 함수이며 , [Revert] 버
튼은 수정된 데이터를 원래대로 복원하는 함수가 구현되어 있다. 그리고 [Quit] 버튼은 어플리케이션을
종료한다．

    connect (submitButton, SIGNAL (clicked() ), this,        SLOT (submit ( )));
    connect (revertButton, SIGNAL (clicked() ), model, SLOT (revertAll () ));
    connect (quitButton, SIGNAL (clicked(fl,     this,     SLoT (close () fl ;



                                                                                   ] 데이터베이스 473


===== PAGE 475 =====
 [Submit] 버튼을 클릭하면 clicked( ) 시그널 이벤트가 발생하며 이 시그널은 submit( ) 슬롯함수와 연
결한다. 동일한 방법으로 revertButton 위젯은 revertAll( ) 슬롯함수와 연결하고 quitButton 위젯은
close( ) 슬롯함수와 연결한다. 지금까지 작성한 위젯을 레이아웃을 사용해 GUI상어］ 표시하기 위해 다음
과 같이 소스 코드를 작성한다．

     QHBoxLayout *majnLayout = new QHBoxLayout;
     mainLayout->addWidget (view) ;
     mainLayout->addWidget ( buttonBox) ;
     setLayout (mainLayout) ;
     setWindowTitle(tr ( "Cached Table") );
 }


윈도우 다이얼로그에서 [Submit] 버튼을 클릭하면 연결된 submit( ) 슬롯함수가 수행된다. 이 함수는
QTableView 상에서 수정된 데이터를 실제 데이터베이스에 적용한다．

 void TableEdi七（그r: : submi七（) {
     model->database ( ) .transaction() ;
     if   (Inodel->submi七AllQ) {
           model->database ( ) .coinmit () ;
     } else {
          model->database () .rollback ( );
          QMessageBox: :warning(this,       tr ( "Cached Table") ,
          叫11                       tr ( "The dat카：)ase reported an error: gl '1 )
           呵1 口                     . arg(model->lastError ( ) .text () ));




transaction( ) 함수는 데이터베이스의 트랜잭션을 처리하기 위해 제공되는 함수이다. 모델상에 수정된
데이터를 실제 데이터베이스상에 적용하기 위해 commit( ) 함수를 수행한다. 만약 submit( ) 수행 중 어］
러가 발생하면 Rollback을 처리하기 위해 QS이TableModel 클래스의 rollback( ) 함수를 호출하고
帥/IessageBox어］발생한 에러를 표시한다．



             Dr川 Down 예저1

Drill Down 예제는 데이터베이스어j 저장된 레코드를 검색하는 예제 어플리케이션이다. 데이터 검색뿐만
아니라 QSq1F扼lationalTableModel 클래스를 사용해 Submit을 처리하는 방법을 포함하고 있으며
QDataWidget八/Iapper 클래스를 사용해 위젯 및 데이터 모델과 연동하는 방법에 대한 예제도 다루고 있
다. 이 예제는 Qt를 설치하면 Exan叩노에 포함되어 있다．




474 CHAPTER 14_ 데이터베이스


===== PAGE 476 =====
（그림） Drill Down 예제 실행 화면



Drill Down 예제 어플리케이션을 실행하고 각 이미지를 클릭하면 해당 이미지의 데이터 정보를 보여주
는 팝업이 실행된다．
예제 어플리케이션 Qt오피스가위치한도시의 사친 이미지이며 팝업 메뉴는Qt오피스가위치한도시이
름, 국가명 , 이미지와 Qt 오피스의 정보를 변경하고 [Submit] 버튼을 클릭하면 데이터가 변경된다. 그리
고 팝업 위젯상에 [Revert] 버튼을 클릭하면 변경된 내용을 원상태로 되돌린다．

이 예제는다음과같은3개의 클래스로구성되어 。1다．
  ·ImageItem 클래스는 오피스 이미지의 정보를 표시하기 위해 사용하기 위한 사용자 정의 아이템 클
    래스' ］다．
  ·View 클래스는 위젯의 아이템을 배치하기 위에 구현된 클래스이다．
  ·Infomati아Window 클래스는 해당 이미지를 클릭하면 팝업 윈도우가 실행된다. 이 클래스는 팝업
    윈도우위젯의      "   11기
                     와
                     '    n ］터베 "
                          " 0       1스적용을위한   ［Submit] 버튼， [Revert] 버튼， [Close] 버튼 " TI
                                                                                      "1
    와 기능이 구현되어 있다．


1Inform計lonWindow 클래스 정의
II寸야m毗ionWindow 클래스는 QWidget 클래스루부터 상속받은 사용자 정의 위젯이다．




                                                                          ] 데이터베이스 475


===== PAGE 477 =====
!class
               InformationWindow   :   public
                                                QDialog
         {
             Q OBJECT

         public:
             InformationWindow ( mnt id, QSqlRelationalTableNodel *offices,
                                 QWidget *parent = 0) ;
             mnt id () ;


         signals:
             void imageChanged(int id, const QString &fileName) ;



Information window7} 생성될 때 해당 Location ID를 사용해 데이티베이스를 검색한다. 클래스의 생
    성자에서 Information window에 표시할 데이터를 표시하기 위해1 ID필드를 사용한다．

  윈도우가 생성될 때 I뇨blic으로 선언된 id( ) 함수가 사용된다. 이 함수는 데이터가 변경되면 변경된 데
이터를 메인 윈도우에 적용하기 위해 ID값을 리턴한다．

         private slots:
             void revert () ;
             void submit () ;
             void enableButtons (bool enable = true) ;



이 예제에서 사용자가 선택한 Location 데이터를 수정하고 다시 원상태로 복구하기 위한 기능을 제공한
다. 데이터가 원상태로 변경되거나 Subm此을 발생할 때 enableButtons( ) 슬롯함수는 버튼에 대한 활
    성화와 비확성화 처리를 담당한다．

         priva七e:
             void createButtons () ;


             mnt locationld;
             QString displayedlmage;

             QComboBox * imageFileEditor;
             QLabel *loca七ionText;
             QLabel 出火countryTex七；
             QTextEdit *descriptionEditor;


             QPushBu七七（:nl 火closeButton;
             QPushButton * submitButton;
             QPushButton * revertButton;
             QDialogBut土onBox 싸m七tonB야；


             ODataWidgetMapper *inapper;




   476 C니APTER 14m 데이터버이스


===== PAGE 478 =====
createButtons( ) 함수는 각 버튼에 대한 오브젝트를 생성하고 각 버튼의 시그널과 슬롯을 연결한다. 그
리고 생성한 버튼을 위젯 윈도우어］ 'JlI기                                     '를 표시가기
                           '한다．Inf9rmation window는 국' ｝와 오피스 위기
위해1QLabel 클래스 위젯을 사용한다.

                             용： ] "］지를 선택 변경할수 있다． 그리고오피스가위기
관련 ' ] " ] ' ] 파일은QComboBox를사 "                                "한상

)'li한 정보는 QTextEdit 위젯을 사용개 출력한다1U｝지막으로 QDataWidge出ilapper 클래스의 오브젝
트 mapper는 각 위젯을 데이터 모델과 Mapping하기 위해 사용한다．


Sin幻rm計ionV師dow클래스구현
생성자는 3개의 인자를 전달 받는다． 첫 번째 인자는 Location ID0］며， 두 번째 위젯은 " 110］터베 "］스의
포인터 , 세 번째 인자는 부모 위젯의 포인터를 넘겨 받는다．

QSqlRelationalTableModel 오브젝트는 "카 ' ］터볘 ' ］스의 외부키（Foreign key）와 연결된 "110］터 모델
을 수정학기 위한 기능을 제공한다.

 InformationWindow: : InformationWindow ( mnt id,
               QSqlRelationalTableModel *offices, QWidget *parent)
                  : QDialog (parent)
 {
     QLabel *locatjonLabel = new QLabel(tr ( "Location: ") );
     QLabel *countryLabel = new QLabel(tr ( "Country: ") );
     QLabel *descrjptjonLabel = new QLabel (tr ( "Description: ") );
     QLabel *jjageFj1eLabel = new QLabel (tr ( "Image file: ") );


     createButtons () ;


     locationText = new QLabel;
     countryText = new QLabel;
     descriptionEditor = new QTextEdit;



첫번째로데이터베이스어］              포함된데이터를표시하기
                                                 위한다양한위젯을생성한다．하지만Combo                 box
는 이미지 파일의 파일명을 표시한다．

     imageFileEditor = new QComboBox;
     imageFileEditor->setModel (offices- >relationModel ( 1) );
     imageFileEditor->setModelColumn
                           offices- >relationModel(1) ->fieldlndex ( "file ") );



 '에서 오피스와관련된 정보는 "offices" 카
예 카                              tI101터베 " 忙= 터］'] 블에 저장되어 있다． " 카"]터 모델을 생성
할때 ' ] 테 " 1블과두 번째 "images" 테 "］블사이에 외부키를사용한다． 따라서 "images" 테 "］블에 저
장된 레코드는 "offices" 테이블의 레코드와 1: L관계를 가지게 된다．

 데이터 모델은 QSqlRelationalTableModel 클래스의 relationModel( ) 함수를 통해 "images" 테이블
 어］ 저장된 레코드와 일치하는 데이터를 모델링 하기 위해 사용한다．

                                                                               1 데이터베이스 477


===== PAGE 479 =====
     mapper = new QDataWidgetMapper (this) ;                              1
     mapper->setModel (offices) ;
     mapper->setSubmitPolicy ( QDataWidgetMapper: : ManualSubmit) ;
     mapper->setltemDelegate(new QSqlRelationalDelegate (mapper) );
     mapper->addMapping(imageFileEditor, 1) ;
     mapper->addNapping( locationText, 2, "text ") ;
     mapper->addNapping( couritryText, 3, 1t;eXt;1' ) ;
     mapper->addNapping( descriptionEditor, 4) ;
     mapper->setCurrentlndex ( id) ;



addMapping( ) 함수는 데이터 모델의 부분을 위젯과 八flapping 한다. 만약 Mapper의 방향이 수평이면
모델에서 Section은 Column이며 그렇지 않으면 행을 뜻한다. set（그urrentlndex( ) 함수는 Location
ID와 관련된 데이터를 위젯어］ 초기화 하기 위한 기능을 제공한다．

mapper 오브젝트의 Policy는 八ilanaualSubm此으로 설정되어 있다. 즉 사용자가 [submit] 버튼을 클
릭해야만 실제 데이터베이스어］ 적용된다. 마지막으로 각 아이템을 사용해 mapper view와 연결된 아이
템의 Delegate（위임）를 지정한다．

     connect (descriptionEditor, SIGNPL (textChanged() ),
              this, SLOT (enableButtons () fl ;
     connect (imageFileEditor, SIGNPL (currentIndexChanged(int) ),
             this,   SLOT(enableButtons () ));


    QFormLayout *forlnLayout = new QFormLayout;
    如rn山ayou七수addRo叫locat江onLabel, locationText) ;
    formLayout->addRow( countryLabel, countryText) ;
     formLayout->addRow(imageFileLabel, imageFileEditor) ;
     formLayout->addRow(descriptionLabel, descriptionEditor) ;


    QVBoxLayout * layout = new QVBo工ayout;
    layout尸＞addLayou七 ( fonT工ayout) ;
    layout->addWidget (buttonBox) ;
    setLayout (layout) ;


    locationld = id;
    displayedlmage = imageFileEditor->currentText ( ) ;


    //setWindowFlags (Qt: :Window) ;
    enableButtons ( false) ;
    setWindowTitle (tr ( "Off ice: %1" ) .arg(locationText->text ( )fl;




enableButtons( ) 슬롯함수는 위젯상에서 윈도우상에 표시된 텍스트가 변경되거나 어떠한 변경이 이루
어지면 enableButtons( ) 슬롯함수가 호출된다. 이 함수는 사용자가 [submit] 버튼 또는 [Revert] 버튼
을 클릭하면 호출된다. QVboxLayout 클래스는 레이아웃을 사용해 윈도우상어］ 위젯을 배치하기 위한
기능을 제공한다．


478 CHAPTER 14.= 데이터베이스


===== PAGE 480 =====
mnt InformationWindow: :id ()


    return locationld;
}


윈도우가 생성될 때 , 메인 어플리케이션이 종료돨때까지 locationld는 삭제되지 않는다. 예를 들어 메인
윈도우에서 사용자가 선택한 locationld를 팝업 윈도우에 전달하기 때문이다. Public으로 선언된 id()
함수는 사용자가 선택한 이미지의 id값이 저장되어 있으며 각 테이블간의 외부키와 연결되어 있다．

void InformationWindow: : revert ()
{
    mapper->revert ( ) ;
    enableButtons (false) ;




revert( ) 함수는 [Revert] 버튼을 클릭하면 발생하는 시그널 이벤트와 연결된 슬롯함수이다．

이 예제에서 QDataWidgetMapper: :ManualSubm此이 설정되어 있다. 이 설정 값은 사용자가 팝업상
에 데이터를 변켱해匠 실제 데이터베이스에 적용되지 않는다. 따라서 [submit] 버튼을 클릭하기 전까지
데이터베이스에 적용되지 않으며 QData＼사idget八tapper 클래스의 revert( ) 슬롯함수가 호출되면 현재
변경된 데이터를 원래의 데이터로 복원한다．

void InformationWindow: :submit ( )
{
    QString newlmage(imageFileEditor->currentText ( ) );


    if   (displayedlmage != newlmage) {
         displayedlmage = newlmage;
         emit imageChanged(locationld, newlmage) ;
    }

    mapper->subndtU;
    mapper->setCurrentlndex ( locationld) ;


    enableButtons (false) ;
}


submit( ) 슬롯함수는 사용자가 위젯상에 [submit] 버튼을 클릭하면 호출되는 슬롯함수히다. 모델과
Mapping된 위젯의 데이터를 변경하고 QDataWidget八/Iapper 클래스의 submit( ) 함수가 호출되면 실
제 데이터베이스에 저장된다．

사용자가 다른 이미지 파일을 선택하면 이전어］ 사용된 이미지 파일을 대신해 변경된 새로운 이미지 파일
명을 저장하기 위해 imageChanged( ) 시그널이 발생한다．




                                                           ] 데이터베이스 479


===== PAGE 481 =====
void InformationWindow: : createButtons ()
{
    closeButton = new QPushButton(tr ( "&Close") );
    revertButton = new QPushButton ( tr ( "&Revert "fl;
    submitButton = new QPushButton(tr ( "&Submit ") );


    closeButton->setDefault (true) ;


    connect (closeButton, SIGNAL(clicked() ), this,       SLOT (close (fl) ;
    connect (revertButton, SIGNAL(clicked(fl,     this,    SLOT (revert () ));
    connect (submitButton, SIGNAL(clickedQ) , this,        SLOT (submit (fl) ;



createButtons( ) 함수는 생성자에서 호출하는 함수이며 위젯 버튼을 초기화하고 버튼의 시그널 이벤트
와 슬롯함수를 연결한다. closeBu仇아Ti 위젯의 클릭 시그널 이벤트는 close( ) 함수와 연결되어 있으며
revertB毗ton은 revert( ) 슬롯과 연결되고 submitB毗ton은 클릭 시그널 이벤트 발생시 submit( ) 슬
롯함수가 호출되도록 연결되어 있다．


小 니ew 클래스의 정의
View 클래스는 메인 윈도우 어플리케이션을 구현하기 위한 클래스이며 QGraphicsView 클래스를 상속
받았다．

class View : public QGraphicsView
{
    Q OBJECT


public:
    View(const QString &offices, const QString &images,
                                               QWidget; 柱冶rent = 0) ;
protected:
    void mouseReleaseEvent (QMouseEvent *event) ;


private slots:
    void updatelmage (int id, const QString &fileName) ;



QGraphicsV扼w 클래스는 윈도우상어］ 이미지를 표시할 Graphics View Framework의 일부이다. 사
용자의 이벤트를 처리하기 위해囚 각 이미지를 클릭하면 QGraphicsView 클래스가 제공하는 mouse
ReleaseEvent( ) 함수가 재구현되어 있다．

생성자는 두 개의 데이터베이스 테이블을 얻어온다. 첫 번째는 오피스와 관련한 정보가 저장된 테이블이
며 , 두 번째 테이블은 이미지 정보가 저장된 테이블이다．

updatelmage( ) 슬롯함수는 Informati아iWindow 클래스의 imageChanged( ) 시그널 이벤트가 발생
하면 Location 이미지를 변경하기 위한 기능이 구현되어 있다．




480 CHAPTER 14_ 데이터베이스


===== PAGE 482 =====
private:
     void addltems ( ) ;
     InformationWindow* findWindow(int id ;
     void showlnformation(ImageItem *image) ;


     QGraphicsScene * scene;
     QList<InformationWindow 火> informationWindows;



addltems( ) 함수는 생성자에서 호출되는 함수이며 아이템을 생성하기 위한 함수이다. fin小Window( ) 함
수는 자주 사용되는 함수이며 사용자가 선택한 이미지의 id를 인자로 넘기기 위한 기능이 구현되어 있다．


S View 클래스의 구현
View 클래스의 생성자는 데이터베이스로부터 이미지 파일 테이블뿐만 아니라 오피스 테이블 이름을 얻
은 다음 오피스 테이블에 QSqlRelationalTableModel 오브젝트를 생성한다．

View: :View(const QString &offices, const QString &images, QWidget *parent)
     : QGraphicsView( parent)
{
     of ficeTable = new QSqlRelationalTableModel(this) ;
     officeTable->setTable (offices) ;
     of ficeTable->setRelation( 1,
                                   QSqlRelation(images, "locationid ",    "file ") );
     off iceTab1e->se1ect ( );



오피스와 관련된 상세한 정보를 데이터 모델로 생성하는 것은 이미지 테이블의 일치하는 파일명과 연결
하기 위해1QSqlRelationalTableModel 클래스의 setRelation( ) 함수를 사용한다．

scene = new QGraphicsScene (this) ;
     scene->setSceneRect (0, 0, 465, 615) ;
     setScene (scene) ;


     addltems U;


     QGraphicsPixrnapltem *logo = scene->addPixmap (QPixinap ( " : /logo.png" ) ) ;
     logo->setPos (30, 515) ;


     setMinimumSize (470, 620) ;
     setMaximumSize (470, 620) ;


     setWindowTitle (tr ( "Offices World Wide ") );
 }

위젯상어］ 표시하기 위한 \／扼w를 생성한다. 예를 들어 Scene과 아이템을 표시하기 위해 각 아이템을 표
시한다. QGraphicsTextltem 오브젝트는 Location 라벨을 표시하기 위해 사용하며 QGrphics
Pixmapltem 오브젝트는 Qt 로고를 표시하기 위해1 사용한다. 마지막으로 윈도의 제목과 위젯의 크기를


                                                                                   ] 데이터베이스 481


===== PAGE 483 =====
 설정하기 위한 소스 코드이다．
1
     void View: :addltems ()
     {
             mnt of ficeCount = officeTable->rowCountU;


             irit imageOff set = 150;
             mnt leftMargin = 70;
             mnt topMargin = 40;

             for (mnt i = 0; i < of ficeCount; i++) {
                 ImageItem *mnlage;
                 QGraphicsTextltem * label;
                 QSqlRecord record = officeTable->record(i) ;

                 mrlt id = record.value ( "id " ).tolnt () ;
                 QString file = record.value ( "file ") .toString () ;
                 QString location = record.value ( "location ") .toString () ;

                 in七 c（그luxnnOff set = ( (i / 3) 士 37) ;
                 m1lt x = ( (i / 3) * imageOff set) + leftMargin + columnOff set;
                 m1lt y = ( (i % 3) * imageOff set) + topMargin;


                 image = new ImageItem(id, QPixmap ( ": /" + file) );
                 image->setData(0, i) ;
                 image->setPos (x, y) ;
                 scene->addltem( image) ;


                label = scene->addText (location) ;
                QPointF labelOffset ( (150 - label->boundingRect ( ) .width() )
                                                                            / 2, 120. 0) ;
                label- >setPos (QPointF(x, y) + labelOff set) ;
          }



어플리케이션의 메인 윈도우를 생성할 때 addltems( ) 함수는 단 한번 호출된다. 데이터베이스의 테이블
에 각 행을 id, file, location 정보를 QString 타입변수에 저장하고 이와 관련된 이미지를 윈도우 상어］
위치할 포지션을 계산한다．

각 레코드는 라벨 아이템을 생성할뿐만 아니라 계산된 위치에 각 아이템을 위치시킨다. 그리고 마우스 커
서가 Hovering되면 Animation을 사용해 Hovering된 이미 지를 확대시킨다．

void View: :mouseReleaseEvent (QMouseEvent *event)
 {
         if    (QGraphicsl七em 火j上em = item)抗（even七m가均S ( ) ) ) {
                if (ImageItem *image = ggraphicsitemcast<ImageItem *>(item) )
                    showlnformation (image) ;
         }
         QGraphicsView: :mouseReleaseEvent (event) ;
}


482 CHAPTER 14_ 데이터베이스


===== PAGE 484 =====
QGraphicsView 클래스의 mouseReleaseEvent( ) 함수는 마우스 이벤트를 처리할 수 있도록 제공되
는 Virtual 함수이다. 사용자에 의해 마우스 이벤트가 발생하면 이 함수를 호출하며 마지막어］ show In-
formation( ) 함수를 호출한다. 이 함수는 information window 팝업을 실행한다．

Graph姚 伽艸ramewo：比 qgraphicsiten c鈿） 함수를 제공한다． 이 함수는 QGraphicslt師
인스턴스 타입인지 아닌지 판단하기 위한 기능을 제공한다．
r
    void View: : showlnformation ( IrnageItem * image)
    {
        mnt id = image->id( );
        if (id < 0 I I id >= of ficeTable->rowCount () )
            return;


        InformationWindow *wjndow = findWindow ( id) ;
        if (window && window->isVisibleO) {
             window->raise ( );
             window->activateWindow ( );
        } else if (window && !window->isVisible ( ) ) {
             window->show() ;
        } else {
             InformationWindow *window;
             window = new InformationWindow(id, off icepable, this) ;


             connect (window, SIGNAL (imageChanged(int,       QString) ),
                      this, SLOT (updatelmage (int,      QString) ));

             window->move (pos () + QPoint (20, 40) );
             window->show( );
             informationWindows . append(window) ;
        }
    }


showlnformati아l( ) 함수는 ImageItem 오브젝트를 인자로 전달받으며 Location ID와 일치하는
location 정보를 출력할 information window를 생성할지 결정한다. 만약 동일한 윈도우의 경우 raise()
함수를 호출하고 해당 윈도우를 visible 처리한다. 만약 그렇지 않다면 새로운 윈도우를 생성한다．


1Image什em 클래스의 정의
ImageItem 클래스는 이미지 아이템의 Animation 기능을 제공한다. 그리고 ImageItem 클래스는
QGraphicsPixmapltem 클래스를 상속받았으며 이미지 아이템의 이벤트 Handler가 구현되어 있다．




                                                                            ] 데이터베이스 483


===== PAGE 485 =====
class ImageItem : public QObject, public QGraphicsPixinapltem

     O OBJECT

public:
   ImageItem(int id, const QPi因nap &pixmap, QGraphicsltem *parent = 0) ;
   void adjust () ;
    jot id ( ) ;

protected:
    void hoverEnterEvent ( QGraphicsSceneHoverEvent *event) ;
    void hoverLeaveEvent ( QGraphicsSceneHoverEvent *event) ;

private slots:
    void setFrame (int frame) ;
    void updateItemPosition( );

private:
    QTimeLine timeLine;
    mnt recordld;
    面uble z;
};


id( ) 함수는 관련된 Location 정보에 대한 고유한 키 값을 통해 해당 이미지 아이템을 구분하기 위해1 사
용한다. QTimeLine 클래스는 이벤트 Handler와 setFrame( ) 슬롯함수에서 사용한다. 즉 아이템의
Anim毗ion의 시간을 제어하기 위한 클래스다. 마지막으로 z값은 아이템 Stack에서 위치를 결정하기 위
해 사용한다．

1Imageltem 클래닐띄 구현
ImageItem 클래스는 단지 QGraphicsPixmapltem 클래스의 추가적인 설정을 위한 클래스이다. 이 클래
스의 생성자는 3개의 인자를 전달받는다. 첫 번째 인자는 Location id이고, 두 번째 인자는 QGraphics
Item과 P1자nap을 전달받는다．

ImageItem: :ImageItem(int id, const QPixmap &pixmap, QGraphicsltem *parent)
    : QGraphicsPixmapltem(pixmap, parent)
{
     recordld = id;
     setAcceptHoverEvents (true) ;

     timeLine. setDuration( 150) ;
     timeLine. setFrameRange (0, 150) ;

     connect ( &timeLine, SIGNAL) fraineChanged( int) ),
                                          七his, SLOT (se七F그rame (in七 ) ) ) ;
     connect (& timeLine, SIGNAL (finished(fl,
                                          this, SLOT (updatelteitPosition() ));

     adjust) );
}

484 CHAPTER 14_ 데이터베이스


===== PAGE 486 =====
참조할 아이템의 ID를 저장하고 hover 이벤트를 발생했을 때 슬롯함수와 연결한다. QTimeLine 클래스
는 animation의 시간을 제어하기 위한 기능을 ］공한다. 즉 timeLine은 hoveril乷된 이미지의 확대되
는 시간을 milliseconds 단위로 Duration을 설 茹｝기 위해 setFrameRange( ) 함수를 사용한다. 그리
고 timeLii始의 finished( ) 시그널 이벤트는 an mation 처리가 완료되면 발생하는 시그널 이벤트이다．
이 시그널은 updateltemPosition( ) 슬롯함수' 연결되어 있다．

    void IinageItem: :setFrame (int   frame)
    {
        adjust () ;
        QPointF center = boundingRect () .center () ;


        setTransform(QTransform: : fromTranslate (center. x () , center. y () ), true) ;
        setTransform(QTransform: :fromScaie (1 + frame
                                               / 330. 0, 1 + frame / 330. 0) , true) ;
        setTransform(QTransform: : fromTranslate (- center. x ( ) ,
                                               -center.y ( ) ), true) ;

,   }       小




timeLine" ] 동작할 때 setFrame( ) 함수가 호출된다． O1 함수는 ": ］템 " ] 변가는 위치를 지정가기 위한
함수이다. adjust( ) 함수는 아이템 이미지의 원래 사이즈로 복귀하기 위한 기능을 제공한다. 그리고 id()
함수는 현재 이벤트가 발생하는 아이템의 Location ID를 저장한다．

QGraphicsltem 클래스의 setZValue( ) 멤버함수는 아이템의 石value를 설정한다. 이 설정 값은
Stack에서 동일한 같은 아이템의 순서를 결정한다. z값으로 같은 항목의 아이템의 위에 그려지도록 설
정한다．

    void Image工七em: :adjus七（)
    {
        QMatrix matrix;
        matrix. scale(150/ boundingRect ( ) .width() ,
                                      120 / boundingRect () .height () );
        setMatrix(matrix) ;



    in七 Imagel七em: : id ( )
    {
        return recordld;
    }

    void ImageItem: :updateltemPosition()
    {
         setZValue ( z) ;




                                                                                         ] 데이터베이스 485


===== PAGE 487 =====
@v1o


===== PAGE 488 =====
     CHAPTER




Qt Test Framework


===== PAGE 489 =====
    n
Ut 5 Programming




           1 Qt Test Framework

           Un仕 테스트는 구현한 어플리케이션의 각 구현 모듈을 소스코＝상에서 정확하게 동작하는지 검사하71
           위한 테스트 방법 중 하나이다. （가는 Un作 테스트를 위한 목적으로 （코 Test Framewo마를 제공한다．
           이번 장에서는 （값에서 제공하는 Un仕 테스트 AP뻬 대하1 살펴보도록 하자．




Qt Test는 Qt 기반의 응용 어플리케이션과 라이브러리를 Unit 단위로 테스트를 제공하기 위한 프레임
워크이다. Un此 Testing framework에서 일반적인 모든 기능을 테스트 할 수 있을 뿐만 아니라 GUI
(Graphical User Interface）까지 포함해 확장된 테스트가 가능하다．

 Feature              Details
 경량의 코드               （가 Te없는 60개의 Export symb이과 약 6000라인의 코드로 구성되어 있다．
 자동화 테스트              GU口f 포함되지 않는 Testing을 위해 Core library로부터 단지 몇 개의 Symb이만을 요구한다．
 Rapid testing        Qt Test는 Te없를 위하1 특정 Runner 툴을 필요로 하지 않는다．
 Data-driven 테스트      테스트 항목은 다른 테스트 데이터를 활용하1 동시에 진행이 가능하다．
 Basic GUI testing    키보드와 마우스를 시뮬레이션으로 동작하도록 기능을 제공한다．
 Benchmarking         측정을 위한 밴치마킹과 백엔드를 지원한다．
 다양한 !DE 사용           （코 Te없는 피sua 앉ud向와 KDeve幻p 개발 환경으로 개발된 인터프리터를 통해 출력할 수 있다．
 Thr的d-satety         쓰레드 Sa伯ty와 Atom允 에러를 리포트 할 수 있다．
 Type-satety          템플릿의 광범위한 사용으로 인해 발생할 수 있는 임의의 타입 변환 오류를 방지할 수 있다．
 Easily extendable    테스트 데이터와 테스트 출력을 쉽게 추7딸 수 있다．




S Test 항목의 작성
Qt Test Framework를 이용해 테스트 항목을 작성하기 위해서 QObject 클래스를 상속받는 하위 클래
스와 Private으로 선언된 슬롯이 하나이상 필요하다．

각 Private 슬롯은 테스트 항목을 테스트하기 위한 Un此 Test 항목들이다. 테스트 오브젝트에서 모든
테스트 항목을 실행하기 위해I QTest 클래스에서 제공하는 qExec( ) 멤버함수를 실행한다．

추가로 테스트 항목과 같이 아직 신뢰성이 없는 테스트 기능을 연결한 4개의 Private 슬롯이 있다. 이 슬
롯들은 테스트 프레임워크에 의해 수행되고 전체 또는 현재 테스트 항목을 초기화하고 정리한다．




488 CHAPTER 15       Qt Test Framework


===== PAGE 490 =====
              打
              私
                           鉀

initTestCase( )           첫 번째 테스트 함수가 실행되기 전에 호출된다．
이eanu口TestCase( )         마지막 테스트 함수7F 실행된 후 호출된다．
init( )                   각 테스트 함수가 실행되기 전에 실행된다．
이eanup( )                 모든 테스트 함수가 호출된 후에 실행된다．



만약 initTestCase( ) 함수가 실패하면 테스트 함수가 실행되지 않는다. 또한 init( ）가 실패하면 다음과
같이 테스트가 실행되지 않으며 다음 테스트 항목을 실행한다．

class MyFirstTest: public QObject
 {
    Q OBJECT
private slots:
    void initTestCase()
    { qDebug ( "called before everything else '1 ) ; }
    void myFirstTest ()
    { QVERIFY (1 == 1) ; }
          void mySecondTest ()
          { QVERIFY (1 1= 2 " }
          void cleanupTestCase ()
           { qDebug( "called after myFirstTest and rnySecondTest ' ) ; }
 };



0Ot Test 다amewo마（의 빌드
Qt에서 제공하는 Test Framework을 qmake가 빌드하기 위해 프로젝트 파일어］ 다음과 같은 모듈을 추
가한다．

          += testlib


만약 make check를 수행한다면 다음과 같은 항목을 프로젝트 파일어］ 추가한다．

  CONFIG += 七es七case


make check에 대한 자세한 정보를 참고하기 위해 qmake 절을 참조하기 바란다．

만약 Qt Creator 이외어］ 다른 빌드 툴을 사용한다면 include path에 Qt Test 헤더 파일의 위치가 추가
되었는지 확인해야 한다. 만약 Qt Release build를 사용한다면 QtTest library어］ test를 링크해야 하
 며， debug build를 사용한다면 QtTest_debug릍 사용한다．


 0Qt Test Command 라인 인자
 자동화 테스트를 수행하기 위해1 다음과 같은 형식을 사용한다．

 I iestname [options] [testfuncti。ns [ : testdata] ]...


                                                                           } Qt Test 다amew아k 489


===== PAGE 491 =====
수행할 테스트 이름으로 testname을 대체한다. testfuncti아坮는 수행할 테스트 함수의 이름을 포함할
수 있다. 만약 testfuncti아娼를 지정하지 않으면 모든 테스트를 수행한다. testfunctions는 테스트 함
수가 테스트 데이터를 활용하기 위해 명시한다．

              /myTestDirectory$ testQString toUpper


톄스트 함수는 모든 활용 가능한 테스트 뎨이터를 사용해 toUpper를 수행한다．

[      /myTes七Dire毗.
                               ry$ 七estQS七： ing
                                                  七.Uppe: 七.I毗：zero


모든 활용 가능한 테스트 톄이터를 사용해 toUpper 테스트를 수행한다. 테스트 데이터를 활용한 的Tnt
테스트 함수는 zero를 호출한다（만약 특정 테스트 떼이터가 존재하지 않는다면 해당 테스트는 실패厚 간
주한다）.

       /myTestDirectory$ testMyWidget -vs -eventdelay 500



testMyWidget 함수 테스트를 수행한다. 모든 시그널이 발생하고 각 시뮬레이션 마우스／키보드 이벤트
가 500 milliseconds를 기다린다．


.                      로그 옵션
테스트 리포트를 파일과 포맷을 결정하기 위해f 다음과 같은 Command line 옵션으로 사용할 수 있다．



-o filename,format                 특정 파일에 리포트를 출력하:   71 위해 txt, xml, IightxmI 및
                                   xunitxml 중 하나를 명시해 포맷을 지정할 수 있다．
       a filename                  특정 파일에 리포트를 출력한다．
-txt
                                   텍스트로 출력한다．
       xml                         XML 문서와 같이 리포트를 출력한다．
니ightxn기                           XML Tag의 스트림과 같이 리포트를 출력한다．
-xunitxml                          Xun仕 XML 문서와 같이 리포트를 출력한다．



. 상서1 로그 옵션
좀더 상세한 테스트 리포트를 위해 다음과 같은（兀mmand line 옵션으로 사용할 수 있다．

옵션                       설명
-silent                  단지 Fatal error, test 실패와 최소한의 상태 메시지를 남긴다．
中＼ii                     자세하게 출력 斗 각 테스트 함수를 입력할 때 보여준다．
                         （이 옵션은 단지 텍스트 출력에 영향을 준다. )
-v2                      자세한 확장 출력 각각의 QCOMPARE(）와 QVERIFY( ) 함수를 보여준다．
                         （이 옵션은 모든 출력에 영향을 준다．)
-vs                      발생한 모든 이벤트 시그널을 발생하며 시그널의 결과를 호출한다，




490 CHAPTER 15_ （값 Test 다amew아k


===== PAGE 492 =====
小 테스트 옵션
좀더 상세한 테스트 리포트를 위해 다음과 같은 Command line 옵션으로 사용할 수 있다．

옵션                           설명
나unctions                    테스트에서 활용 가능한 모든 테스트를 출력하고 종료한다．
 datatags                   테스트에서 모든 데이터 태그를 출력한다．
                            （引obal 태그는 앞에 _global_' 이 붙는다．
-eventdelay ms               키보드와 마우스 시뮬레이션山T朗t::keyClick( ), QTest::rnouseClick 등）을 위한
                             Delay를 지정한다. 파라미터로 값을 지정할 수 있다．
 keydelay ms                 -eventdelay와 같이 키보드 시뮬레이션에 Delay를 지정한다．
 mousedelay ms                eventdelay와 같이 마우스 시뮬레이션에 Delay를 지정한다．
 rnaxwarnings number         Warr기ng 출력의 최대 수를 지정한다． 0을 지정하면 제한이 없다． 디폴트로 200001
                             설정된다.
 noc rash handler            유닉스／리눅스 플랫폼에서 （가ash 핸들러를 비활성화 시킨다．



巒 벤치마크 옵션
다음은 Command line에 벤치마크 테스트를 제어 옵션으로 사용한다．

옵션                    설명
 callgrind             벤치마크 타임을 분석하기 위해 사용한다. 이 옵션은 리눅스 플랫폼에서만
                       사용 가능하다．
나ickc（가Jnter           벤치마크 타임을 분석하기 위하I CPU의 기ck Cc川nt아를 사용한다．
-eventcounter          벤치마크 하는 동안 전달받은 이벤트 카운트 수
-rnhmurnva山e n         최소 허용 측정값을 설정한다．
 iterations n          축척 반복 횟수를 설정한다．
 median n              펑균 반복 횟수를 설정한다．
 vb                    자세한 벤치마크 정보를 출력한다．



S 벤치마크 측정을 위한 소스 코드 작성
벤치마크의 소스 코드를 작성하기 위해 다음과 같은 작성방법을 따라야 한다. 그리고 원하는 벤치마크를
작성하기 위해 테스트 코드어］ QB且NCHMAPJK 매크로를 추가한다．

class MyFirstBenchmark: public QObject
{
        Q OBJECT
private slots:
        void myFirstBenchmark ()
        {
             QString stringi;
             QString string2;
             QBENCHMARK {
                   stringi . localeAwareCompare ( string2) ;



    ;



                                                                          ] （코 Test 다amework 491


===== PAGE 493 =====
 QBENCHMARK 매크로 내부의 코드를 측정하고 또한 정확한 측정값을 얻기 위해 테스트 반복이 가능
하다. 선택한 측정 Back-end는 플랫폼에 의존한다. 따라서 Command line에 선택한 옵션이 가능한지
확인해야 한다．

 Name                 Command-line Argument    Availability
 Walltime             (default)                모든 플랫폼
 CPU tick counter      tickcounter             Windows, Mac OS X, Linux. UNIX
 Vaigrind Caligrind   -caligrind               Linux (V的rind가 설치 필요）
 Event Counter        -eventcounter            모든 플랫폼



Walitime은 모든 플랫폼에서 사용 가능하지만 유용한 결과를 얻기 위해 많은 반복을 필요로 한다. Tick
Counter는 일반적으로 사용할 수 있으며 적은 반복으로 결과를 제공한다. 하지만 CPU 대역폭의 스케일
링 문제어］ 취약할 수 있다．

Valgrind는 정확한 결과를 제공하지만 I/O account어］ 대기하지 않는다. Event Counter는 모튼 플랫
폼에서 사용할 수 있다. 그리고 이것은 해당 Target에 전송하기 전에 수신된 이벤트의 수를 제공한다．



              Unit Test
이번 장에서는 단순한 Unit Test 코드를 작성해 보도록 하자. QString 클래스의 동작（beha叭or) 테스
트하는 것을 가정하고 테스트 함수를 작성한다. 그리고 클래스는 QObject 클래스를 상속 받도록 소스 코
드를 작성한다．

 半include <Q七Test/QtTes七＞


 class TestQString: public Qobject
 {
     Q OBJECT
 private slots:
      void toupper ( ) ;
 };


QTest를 혜더에 추가하고 테스트 프레임워크가 발견하고 실행하기 위해 Private sl毗과 같이 테스트 함
수를 선언한다. 테스트 함수는 스스로 테스트를 수행할 수 있도록 다음과 같이 구현해야 한다．

 void TestQString: :totJpper ()
 {
      QS七ring s七r = "Hello " ;
      QVERIFY (str. toUpper () == "HELLO") ;




QVERIFY( ) 매크로는 인수로 전달된 표현식을 평가한다. 만약 표현식의 테스트 평가가 tn肥를 리턴하


492 CHAPTER 15_ Qt Test Framework


===== PAGE 494 =====
면 계속해 테스트를 수행한다. 그렇지 않으면 평I'} 테스트 실패 로그를 남기고 테스트 수행을 중단한다．
만약 테스트 결과의 자세한 출력을 하기 원한다면 QVERIFY( ) 매크로 대신에 QCOMPARE( ) 매크로를
사용해야 한다．

void TestQString: :toUpper ( )
 {
     QString str = "Hello";
     QCOMPARE ( str . toUpper () , QString ( "HELLC) " ) ) ;
 }


만약 문자열이 같지 않으면 테스트 로그 양쪽의 른자열 내용을 추가한다. 그리고 비교 결과가 왜 실패했
는지 즉시 표시한다. 마지막으로 테스트 케이스를. 독립적으로 수행하기 원한다면 다음과 같이 코드를 작
성한다．

QT丑ST냥끄＼IN(TestQStrin引
#include "testqstring.moc "



QTESTMAIN( ) 매크로는 간단히 테스트 함수듣三 인자로 설정해 수행할 수 있으며 , cpp 파일어］ 작성한
테스트 함수를 구현하고 선언한다. 또한 Qt7i 내부에서 동작하는뎨 필요한 MOC(Meta-Object
吼mpiler) 파일을 포함해야 한다． MOC에 대한 1자세한 내용은 Meta-Object Compiler 절을 참조하기
바란다.


印테스트함수의실행
빈 디렉토리에 작성한 테스트 함수를 임의의 소三. 코드 파일 이름（testQString. cp미으로 저장하고 다음
과 같이 qmak. 툴을 사용해 프로젝트 파일을 생1성한다. 프로젝트 파일이 생성된 것을 확인하고 qmake
를 실행하면 makefil.이 생성된다． 그리고 프롬三드트에 make를 실행한다．

 /myTestDirectory$ qmake -project "QT += 七es七lib "
 /myTestDirectory$ qmake
 /myTestDirectory$ make



만약 윈도우 플랫폼을 사용한다면 어떤 빌드 툴읕r 사용하는지에 따라 make 대신에 nmake를 사용해야
한다. 테스트 함수를 실행하면 다음과 같은 결과듣卜 얻을 수 있다．


叭 ＝月kKX乂C Stai北 te스ting of TestQStrin! ,
Config: U＄主ng Qie！   北 library     S．日1日戶 Qt S.目．目
I 'RSS    : TestQString: : initlestCase ()
PASS      : TestQStrinq: ;toUpper ()
PASS      : TestQString: :cleanuplestCase< )
Totals:    3 passed戶 日 failed戶 日 sSipped
r4口· “yX」‘y片 Finished testing     of TestQStrinp a1
P: esS <RETURN> to close this windowm 1.




（그림） 테스트 함수 실행 결과


                                                               1 Qt Test Framework 493


===== PAGE 495 =====
         ;t口 데이터 주도 테스트
 데이터 주도 테스트 기법（Data Driven Testing）은 테스트 입력 값과 예상이 되는 테스트 결과를 비교하
 기 위한 목적으로 행해지는 기법이다. 많은 양의 데이터를 테스트할 때 주로 소스 코드 내에 하드코딩하
 는 방식으로 테스트를 진행할 수 있다．

 하지만 이 기법을 활용하면 많은 양의 떼이터를 아이템 단위로 등록해1 함수 단위로 작성해 쉽게 테스트를
 진행할 수 있으며 데이터베이스와 같이 많은 양의 데이터를 테스트 해야 하는 경우 이 기법을 활용하면
 유용하다．

 QC아作恐피QS七rin引 "hell寸 ) .toUpper ( ) r QString( " 표EL山0" ) ) ;
 QCOMPARE(QString( "Hello " ) .toupper () , QString( "HELLO") );
 QCOMPrRE(QString ( "HellO " ) .toUpper () , QString( "HELLO") );
 QCOMPARE (QString( "HELLO") .toUpper ( ), QString( "HELLO") );



테스트 함수가 반복적인 코드를 작성해 종료하는 것을 방지하기 위해 Qt Test Framework은 테스트 데
이터를 계속해 추가한다. 그리고 테스트 클래스어］ Private 슬롯함수를 계속 추가할 수 있다．

 class Tes七QS七ring: public QObjec七
 {
          Q OBJECT


 private slots:
          void toUpperdata() ;
          void toUpper () ;
     ;



0 데이터 함수 작성
데이터 함수는 테스트 함수와 연관 이름을 사용하기 위해 다음 예제와 같이 함수 이름의 뒤에 " data" 를
사용한다．

 void TestQString: :totJpperdata()
 {
         QTest: : addColumn<QString> ( "string ") ;
         QTest: :addColurnn<QString> ( "result ") ;


         QTest: :newRow ( "all lower ") << "hello " << "HELLO";
         QTest: : newRow( "mixed")      << "Hello" << "HELLO";
         QTest: :newRow( "all upper ") << "HELLO" << "HELLO";
 }

첫 번째로 QTest 클래스의 addColumn( ) 함수를 사용해1 테스트 테이블의 아이템을 정의한다. 예를 들
어 테스트 문자열 그리고 비교 문자열을 적용한다. QTest 클래스의 newRow( ) 함수를 사용해1 테스트
테이블에 뎨이터를 추가한다. 각 데이터 열은 테스트 테이블상에서 분리되어 등록된다．


494 CHAPTER 15. （코 Test 다amewo水


===== PAGE 496 =====
QTest: :newRow( ) 함수의 인자는 데이터 열과 연관되는 이름을 사용한다. 만약 테스트가 실패하면 테
스트 결과 로그어］ 전달한 인자가 사용된다. 그리고 새로운 테이블에 등록할 데이터의 첫 번째 항목은 임
의의 문자열이다. 그리고 두 번째 항목은 예상되는 문자열을 적용한다. 예제 코드와 같이 테이블을 생성
하면 다음과 같은 형태의 테이블이 작성된다．

INDEX      NAME             STRING          RESULT
0          all lower         "he妃'          HLLO
j          mixed             "Hello"        HELLO
2          all upper         "HELLO"        HELLO



. 테스트 함수의 작성
toUpper( ) 테스트 함수를 다음과 같이 재작성한다．

void TestQString: :toUpper ()
{
    Q1咆TCH(QString, St丁in引 ;
    QFETCH(QString, result) ;


    QCOMPARE (string. toUpper ( ) , result) ;
}


작성한 TestQString 클래스의 切Upper( ) 함수는 이전어］ 데이터 함수에서 테이블에 등록한 3개의 아이
템에 대해 3번 테스트가 수행된다. QFETCH( ) 매크로를 사용해 테이블의 데이터 열에서 두 개의
Eleme砒를 가져온다．

QFETCH( ) 매크로는 두 개의 인자를 가진다. 첫 번째 인자는 테이블에 등록한 Elem아此의 타입이며 두
번째 인자는 Elem아此의 이름이다． QCOMPARE ( ) 매크로를 사용해 테스트를 수행한다．

이러한 방식을 사용해 데이터 주도 테스트를 수행하는 것은 추가적인 수정 없이 쉽게 테스트 데이터를 추
가할 수 있다. 그리고 테스트 케이스를 독립적으로 수행할 수 있도록 다음과 같이 작성할 수 있다．

q四ST_MAIN ( Tes七QS七ring)
孝include 1냐;es七qs七ring. moc "


QTEST_MAIN( ) 매크로는 모든 테스트 함수가 수행되도록 main( ) 함수를 단순하게 확장할 수 있는 기
능을 제공한다. QTEST_MAIN( ) 매크로 함수에서 사용한 인자는 클래스명을 지정한다．




                                                     ] （그tTest 다amework 495


===== PAGE 497 =====
                                         寸
         C,'（그t\Qt5.O O\IooIs\（간Creat:r ba,'qtcreator_t玎oces乞；tub.己七

              Start testing of lestQString
   onfig: Using QTest librarp S．日1目戶 (}t; S．  日月
   ASS    : TestQString: :initTestCase ()
   ASS    : TestQString: :toUpper (all  lower)
   ASS    : lestQString: :toUpper(nixed)
   ASS     z lestQString: :toUpper (all upper)
   ASS    : TestQString: :cleanupTe!;tCase ()
   ota1s : S passed. 目 failed尸 日 skipped
    ' (．누甘k片 Finished testing of TestQString o
 iress <RETURN> to close this window. ..




（그림） 데이터 주도 테스트 예제 실행 화면




               .3 GUI 이벤트 시뮬레이션

GUI 이벤트 시뮬레이션 테스트는 Qt Test Framework 중 하나의 Feature이다. 이 테스트 기법은 플
랫폼 기반의 Nat如e 윈도우 시스템의 시뮬레이션 대신에 Qt 이벤트 시스템 내부에 이벤트를 전송함으로
써 플랫폼 기반에 독립적으로 시뮬레이션이 가능하다. 따라서 GUI 이벤트 테스트를 위해 별도의 어플리
케이션 및 테스트 목적으로 사용되는 특정 Machine을 사용하지 않고 Qt Test Framework만으로 테스
트가 가능하다. 이번 장에서는 간단한 GUI 테스트 예제를 작성해 보도록 하자．


0GUI 테스트 코드 작성
Qt에서 제공하는 GUI 위젯 중 QLineEdit 클래스 위젯을 테스트 한다고 가정했을 때 테스트 함수를 포
함하는 클래스 작성이 필요하다．

 #include <QtWidgets>
 #include <Q七Test/Q七Tes七＞


 class TestGui: public QObject
 {
            Q OBJECT


private slots:
            void testGui ( ) ;


     ;



QtWidgets 클래스는 단지 테스트 함수에 사용할 GUI 위젯 클래스를 사용해야 하므로 include 선언이
필요하다．

 void TestGui: :testGui()
 {
            QLineEdit lineEdit;
            QTest: :keyClicks (&lineEdit,                       "hello world") ;
            QCO卜狂）ARE (lineEdit. text () , QString( "hello world") );
 }


496 CHAPTER 15_ （가 Test 다amew아k


===== PAGE 498 =====
첫 번째로 QLineEdit를 생성한다. 그리고 QTest 클래스의 keyClicks( ) 함수를 사용한다. 이 함수는
클릭 이벤트가 발생했을 때, 예상되는 결과를 출력하도록 설정할 수 있다．

keyClicks( ) 함수는 두 개의 인자를 사용한다. 첫 번째 인자는 테스트 대상이 되는 GUI 위젯을 사용하
고 두 번째 인자는 예상 결과값이다. 여기서는 "hello world" 문자열이 예상 결과값이다. 즉 QLine
Edit 위젯상에서 클릭 이벤트가 발생하면 "hello world" 문자열이 이 위젯에 입력되는 테스트가 예상 결
과이다. 그리고 시뮬레이션을 하기 위한 QTest: keyClicks( ) 함수는 추가로 각 키가 눌러진 후에 테스
트 Delay를 지정할 수 있다. 그리고 QTest: :keyClicks( ) 외에 QTest::keyPress( ), QTest::key
Release( ), QTest::mouseC1ick( ), QTest: :mouseDC1ick( ), QTest::mouseMove( ), QTest::
mousePressO, QTest: :mouseRelease() GU긔 이벤트 함수를사용할수 있다.

마지막 라인의 QCOMPARE( ) 매크로는 QLine屯dit의 텍스트의 예상되는 결과값과 비교하기 위해 사용
한다．

QTEST卜AIN ( TestGui)
 #include "testgui. moc '



QTEST_MAIN( ) 매크로는 모든 테스트 함수가 수행되도록 main( ) 함수를 단순하게 확장할 수 있는 기
능을 제공한다. QTEST_MAIN( ) 매크로 함수에서 사용한 인자는 클래스명을 지정한다．

                                                                 x
      C人Qt山巧 O（汰TooI5\（그tCreator寸)In\q'c『e크tX-. 口0Ce三 ;tJb exe

X」 片yUXX片 Staxt testing of lestGui 켜iiUXXXK片
（沁afig: L뇨ing QTest librarg 5．目1日1Qt 5．日．日
PASS     : Test（뇨i= = 如itlestCa各eO
 ASS     : TestGui::testGui ()
 ASS     : TestGui::cleanupTestCase (>
 otals: 3 passed戶 日 failed. 0 shipped
            Finished testing of TestGui cccxxx
Pi1es!; <RETURN> to close this window. .




（그림） GUI 이벤트 시뮬레이션 테스트 예제 실행 화면




     心4그 GUI 이벤트 Replay 테스트
GUI 이벤트 Replay 테스트는 연속으로 GUI 이벤트를 발생시켜 위젯을 테스트하기 위한 목적으로 사용
되는 테스트이다. 이 테스트 기법은 데이터 주도의 테스트 기법과 비슷하며, 데이터 함수와 테스트 함수
를 작성하고 이 함수를 포함하는 클래스를 생성한다．

 class TestGui: public QObject
 {
         Q OBJECT

 private slots:
     void testGui data () ;
     void testGui() ;
 };



                                                                     ] （그tTest 다amework 497


===== PAGE 499 =====
      0Replay 데이터 함수 작성
 데이터 함수는 테스트 함수와 연관 이름을 사용하기 위해1 다음 예제와 같이 함수 이름의 뒤에 " data" 를
 사용한다．

 口．
              。ld Tes七GuI: :tes七Gui data ( )
          {
                 QTest: :addColumn<QTestEventLlst> ( " events " );
                 QTest: :addColumn<QStrlng> ( "expected") ;


                 QTestEventList listi;
                 listi .addxeyClick ( ' a' );
                 QTest: :newRow ( "char ") << listi   << "a";

                 QTestEventList list2;
                 list2. addKeyClick ( ' a' ) ;
                 list2 . addKeyClick ( Qt: : Key_Backspace) ;
                 QTest: :newRow( "there and back again") << 1ist2 << " ";
      }


테스트 항목을 위해 데이터 테스트 기법과 같이 테이블에 Elem이此를 추가한다. 테이블에 Elem아此를 추
가하기 위해 QTest: :addC아umn( ) 함수를 사용한다．

첫 번째rEleme毗는 GI끄의 이벤트 리스트이고 두 번째 Element는 QWidget 상에서 이벤트 리스트를
적용했을 때 예상되는 결과이다. 한 개의 QTestEver此List는 발생시킬 이벤트 항목을 여러 개 등록할 수
있다．

데이터 함수상에 두 개의 QTestEventList 川ement를 생성한다. 첫 번째는 'a' 키 이벤트만 등록한다．
QTestEventList는 addKeyClick( ) 함수를 사용해 이벤트를 계속해서 추가할 수 있다．

QTest: :newRow( ) 함수의 인자는 데이터 Set의 이름이다. 그리고 다음 항목은 이벤트 리스트를 지정한
다. 다음 항목은 테이블상에서 예상되는 결과값이다．

두 번째 QTestEver此List는 키 Click 이벤트로 'a' 와 'backspace' 이벤트로 구성되어 있다. 두 번의
Click 이벤트가 발생하도록 이벤트 리스트를 생성하고 QTest: :newRow( ) 함수를 사용해 생성한
QTestEventList를 등록한다．


0Replay 테스트 함수 작성
Replay 테스트 함수는 다음 예제 코드와 같이 작성한다．

 void TestGui: :testGui()
      {
                QFETCH(QTestEventList, events) ;
                QFETCH(QString, expected) ;


                QLineEdit lineEdit;
                                                                            0


498 CHAPTER 15 01 Test Framework


===== PAGE 500 =====
       events. simu1ate (&1ineEdit) ;


       QCOMPAR丑(iineEdit. text ( ) , expected) ;
 }


QFETCH( ) 매크로를 사용해 테이블의 데이터 열에서 두 개의 Eleme砒를 가져온다. QFETCH( ) 매크
로는 두 개의 인자를 가진다. 첫 번째 인자는 테이블어］ 등록한 Elem아此의 데이터 타입이며 두 번째 인자
는 Elen呻此의 이름이다．

QLineEdit를 생성하고 QTestEventList: :sjmulate( ) 함수를 사용해 위젯상에 이벤트 리스트를 등록한
다. 마지막으로 QC0MPARE( ) 매크로는 QLineEdit의 문자열과 테스트 예상 결과 문자열을 등록한다．

 QTESTHMAIN ( TestGui)
 #inc lude "testgui . mac "



QTEST_MAIN( ) 매크로는 모든 테스트 함수가 수행되도록 main( ) 함수를 단순하게 확장할 수 있는 끼
능을 제공한다. QTEST小MAIl寸（) 매크로 함수에서 사용한 인자는 클래스명을 지정한다．

     C:
      ＼아口t5皿qb北4<m北計났기fl1qtcreat孔p

뉴共XX乂X弓1十X Start testing of TestGui r: nM／뇨八n片
（幻nfig: Using Qlest library    S．日．目戶 Qt 5 －日．目
PASS    : TestGui: :initlestCase ()
 ASS    : lestGui: :testGui (char)
 ASS    : TestGui: :testGui (there and back again>
PASS    : TestGui: :cleannplestCase()
Totals: 4 passed. 日 failed. 日 skipped
X斗吐甘m甘朴斗朴 Finished testing of TestGi上3-          片

Pi'eSs <RETURN> to close this window.

                                   川



（그림） GUI 이벤트 Re이ay 테스트 예제 실행 화면




        1.   5 벤치마크 테스트
벤치마크 테스트는 성능 측정과 같이 측정 결과를 통해 비교 테스트를 위한 목적으로 사용되는 테스트 기
법 ' ］다． 벤그
         ' "｝크 테스트를 위한 소스 코드를 작성가기 위긔
                                    ' QBENCHMARK " 뀨크로와 함께 테스트 함
수를 확장한다．

이 테스트 기법은 벤치마크 설정 소스 코드와 측정을 위한 소스 코드를 포함한 QBENCHMARK 매크로
로 구성되어 있다. 작성할 테스트 함수인 QStri咽:localeAwareCompare( ) 함수는 벤치마크 하기 위
해 다음과 같이 작성한다．

 void TestBenchmark: : simple ()
 {
       QString stri    = QLatinlString( "This is a test string ") ;
       QS七ring s七r2 = QLa七mniS七ring( "This is a 七es七 5七ring") ;                         O



                                                                      ] （거 Test 다amev四m 499


===== PAGE 501 =====
!        QCOMP客strl.
         QBENCHMIRK { localeAwareCompare              (str2)   ,   0) ;
1   ,    '   stri   iocaie   ware "ompare   str   "




설정은 함수가 시작되는 시점어］ 동작한다. QBENCHMARK 매크로 내부 소스 코드는 정확한 측정을 위
해 가능한 몇 번의 반복이 수행될 수 있다. 몇 번의 반복이 이루어지는지 백엔드 방식으로 Command
line에서 선택적으로 옵션을 사용해 가능하다．


    毋 데이터 함수 작성
데이터 함수는 여러 개의 데이터 입력을 비교하는 벤치마크를 생성한다. 예를 들어 표준 비교 대상과 상
응하는 비교 대상을 사용한다．

    void TestBenchmark: :multipleHdata ( ) {
         QTest: : addColumn<bool> ( "useLocaleCompare") ;
         QTest: :newRow ( "locale aware compare") << true;
         QTest: :newRow ( "standard compare") << false;




테이블에 Elen珀nt를 추가한다. QTest: :newRow( ) 함수의 인자는 데이터 Set의 이름이다. 그리고 다
음 항목은 테이블상에서 예상되는 결과값이다．


    的 테스트 함수 작성

    void TestBenchmark: :multiple( ) {
         QFETCH(bool, useLocaleCompare) ;
         OString stri = QLatinlString( "This is a test string") ;
         QString str2 = QLatinlString( "This is a test string") ;
         mnt result;
         if (useLocaleCompare) {
             QBENCHMARK {
                    result = strl. localeAwareCompare(str2) ;
              }
         } else {
             QBENCHMARK {
                    result = (stri   == str2) ;
              }
         }
         Q UNtJSED (result) ;
     }




    500 CHAPTE［극 15_ （코 Test 다amewo水


===== PAGE 502 =====
테스트 함수에서 사용한 "if (useLocaleCom 1are)" Switch는 테스트의 오버헤드를 피하기 위해
QBENCHMARK 바깥쪽에 위치시킨다. 두 개의 벤치마크 테스트 중 한 개의 QBENCHMARK 매크로가
활성화된다. 다음은 작성한 벤치마크 테스트 예저 를 실행한 결과이다．


難 벤치마크 테스트 결과

       火火士火火 Start; 七esting of Tes七Benchmark 士火火火升火火火火
Config: Using QTest library     5. 0. 0, Qt 5. 0. 0
PASS     : TestBenchmark: :initTestCase ()
PASS     : TestBenchinark: :simple ()
RESULT : TestBenchmark: :simple () :
       0. 00026 IT田ecs per i土erati이l (t（그tal: 70, i七era七ions: 262144)
PASS     : TestBenchmark: :multiple (locale aware compare)
RESULT : TestBenchniark: :multiple () :"locale aware compare ":
       0. 00032 msecs per iteration     (total:    86, iterations:    262144)
PASS     : TestBenchTnark: :multiple (standard compare)
RESULT : TestBenchmark: :multiple ( ) : "standard comparen:
       0. 000069 msecs per iteration     (total:    73, iterations:   1048576)




PASS     : TestBenchmark: :series (standard compare--8001)
RESULT : TestBenchmark: :series () : n standard compare--8001":
       0. 013 msecs per iteration   (total:   55, iterations:    4096)
PASS      : TestBenchmark: :cleanupTestCase ()
Totals: 15 passed, 0 failed,      0 skipped
火火火火火士士士士 Finished tes七ing of TestBenchmark 火士火火火火火火士




小 QTestLib Tool 프로젝트
QTestL小 Tool 프로젝트는 Qt 프로젝트의 하 이다. 이 프로젝트는 테스트 데이터를 조작하고 시각화
하기 위한 목적으로 활용할 수 있다. 테스트를                          행한 결과를 얻어와 성능을 비교하기 위한 툴이 포함되
어 있다. 그리고 이 툴은 테스트를 수행한 데이터를 가공해 웹 기반으로 테스트 성능 자료를 그래프로 생
성해주는 기능을 제공한다．

이와 관련해 자세한 정보는 Qt Labs(http:/／毗. gitorious. orglqt크abs/qtestl小 的아S）에 등록된
qtestlib-tools 프로젝트를 검색해 보기 바란다．




                                                                                1 Qt Test Framework 501


===== PAGE 503 =====
M@vo


===== PAGE 504 =====
  CHAPTER




Qt Quick과 QML


===== PAGE 505 =====
Qt 5 다og治m떼ng




F尸1 :// Qt Q uick과 QML
發罌

難囊驀罐難孕 （값 O내ck은 쉽고 빠르게 현대적인 GUI 인터페이스를 개발하는 목적으로 QML를 제공한다． OML은
        HTML과 같은 인터프리터 언어와 비슷하다. 즉, OML을 사용하I GUI 인터페이스를 개발할 수 있는 방
        법에 대해 알아보도록 하자．




Qt 帥ick은 개발자에게 현대적인 GUI 인터페이스를 쉽게 설계하고 어플리케이션에 척용하기 위한 목
적으로 제공되는 API이다. 이러한 GUI 인터페이스를 설계하는데 있어 Qt Quick은 QML을 사용한다．
기존의 QWidget, QPainter 등을 사용해 UI를 설계했던 것과 마찬가지로 QML은 UI 아이템의 행동을
정의하고 제어할 수 있다．

帥ilL은 declarative 언어이며 （절차 언어） 자바스크립트가 확장된 스타일의 문법구조를 가지고 있다．
QML은 JavaScript와 같은 절차 언어를 해석하는 Declarative 모듈이 있으며 C+＋을 사용해 소스 코드
를 작성하면 컴파일러가 실행 바이너 리를 생성하는 것과 같이 Declarative 모듈은 QML로 작성한 코드
를 실행할 수 있는 어플리케이션으로 변환하는 작업을 한다. 또한 QML 어플리케이션 내에서 C++ API
를 사용할 수 있다．

Qt Quick과 QML을 사용해 응용 어플리케이션을 구현하는 경우 Qt Quick과 QML로 완벽한 응용 어플
리케이션을 구현할 수 없다. 예를 들어 네트워크 Traffic 사용량을 확인하기 위한 어플리케이션을 구현
하기 위해 시스템 레벨의 네트워크 Traffic을 제어하기 위해 Native 라이브러리 사용이 필요하다. 따라
서 사용자에게 제공하는 GUI 단은 Qt Quick을 사용해 네트워크 사용량을 그래프로 표시하고 네트워크
Traffic을 측정하는 실제 구현 API는 전통적인 Qt API 및 시스템 레벨의 API를 사용해 구현하는 것이
가장 바람직하다．

따라서 Qt 伽ick으로는 G｛끄를 구현하고 실제 기능이 동작하는 모듈은 전통적인 Qt API를 사용해 구현
할 수 있다. 이러한 방식은 HTML5를 이용해 응용 어플리케이션의 구조와 흡사하다. 즉, 사용자에게 제
공하는 GUI는 HTML5를 사용하고, 실제 동작을 담당하는 모듈은 Native API를 사용해 HT八4L5 기반
의 응용 어플리케이션을 구현한다．

Qt Quick을 사용하면 디자인 로직과 프로그램 로직을 분리할 수 있는 장점이 있다. 즉 C+＋와 같은 프로
그래밍 언어의 지식 없이 QML만 이해하고 있다면 GUI를 디자인 할 수 있다. QML은 HTML5와 유사하
며 직관적이고 이해하기 쉽다. 그리고 전통적인 C+＋에서 제공했던 기능을 모두 지원한다. 예를 들어
QtWebKit, Anim毗幻n, 멀티미디어 등을 QML어］ 사용이 가능하다．


504 CHAPTER 16_ Ct QuickZ QML


===== PAGE 506 =====
이번 단원에서는 QtQuick에서 사용하는 QML 현어에 대해 이해하고 QML과 c+＋을 연동해 응용 어플
리케이션을 구현하는 방법에 대해 알아보도록 하兀．


                    （그tQuick 프로젝트 생성과 유용한 툴

QML은 Qt 伽ick어］ 포함된 Declarative 언어이다. 0+＋을 사용해 어플리케이션을 개발했던 것과 마찬
가지로 Qt Quick은 QML을 사용할 수 있다. 간단한 예제를 Qt Cre毗야를 통해 다음과 같이 프로젝트
를 생성한다．

駐 New

 Cbs'그Os a tern帥抛：                                                                               0esktop Ten ［止카尸1

 Projects                 口    Qt Gui Application
                                                                          Creates 미Qt Quick 2 applicafian project that
  Applicat口ns              4   QtQ山ck 1 Application (Belt-in Elementr     cao contain both 0ML and C++ code and
                                                                          includes 4 U0uickView
  Libraries                d   （갛（크月ck 2 Appllcatil거I (Bu昨in 티ements
  Other Project            4   Qt Quick I Application (from Existing Q卜
  Non-Qt Pr아ect           1    QtCons어e Applicat出n
  Impo八Pr이ect             目    HTMLS Applicati口n
 테es and 디asses            止匡iQt Quick lilt
                                                                          Support닉d 미atlorms: On引比旺｝
  C斗r                      덥 QtQuick2 UI
  Qt
  GLSI
  Gen酊긔




（그림） 010미ck 기반의 프로젝트 생성



앞의 그림에서 보는 것과 같이 왼쪽 [Projects                                                                 ' [Applications］를 선택하고 중앙의 리스트에서
Qt 伽ick 항목을 선택하고 아래 [Choose' " "1                                                             클릭한다. 다음 화면에서 프로젝트명을 입력하고
프로젝트 생성을 완료하자．

  m히n 口州 O1 Creator
 F爬    Ed比    Ba妃       Debug An引yze    a：刃Is   Windo叫   He巾
              Pr,기므사드              ! 口： 包 ［予 x       + 中        or쉬n시n기
                 C HelloWorid                                   ！好1：二＝ QtQuic          2. 0
                   匠 Hello나or吐마0
                 a t; 아quick2applicat心n너eWef               J Rectangle {
                      匠i 求S山rk2applicattond沌町eL可         4       width: 360
                    > J, Headers                         三       height: 360
                    ;， 斗 Sources                                 Text {1
                 4 ，恥 幻毗e5                                           text: qsrr) "Hello World")
                      的 maln.cpp                                     anchors. centerln: perera亡
                 d 也 Q卜내L
                    J 薰 qrrrl/Hel的w아Id                               Mo표seA_red {
                        圈 maxsqml                                        anchors, fill:          parent



（그림） 01 Quick 프로젝트 생성 완료



프로젝트 생성이 완료되면 main. qml 파일이 생성된 것을 확인할 수 있을 것이다. 이 소스 코드는 QML
언어로 작성된 예제이며 프로젝트를 생성하면 생성되는 디폴트 코드이다. 어플리케이션을 컴파일하고 실
행하면 "Hello World" 화면 중앙에 출력하는 간단한 예제 소스 코드이다．


                                                                                                                         ] Qt 0미ck과 QML 505


===== PAGE 507 =====
  import QtQuick 2. 0


  Rectangle {
      wid七h : 360
         hei야比： 360
         Text {
             text: qsTr ( "Hello World")
             anchors. centerln: parent
         }
      MouseArea {
             anchors . fill:     parent
             onClicked: {
                  Qt.quit () ;
             I




첫 번째 라인의 import는 c+＋에서 in이ude와 비슷하다. QML을 사용하기 위해서 QtQuick 2.0을
import 해야 한다．

Rectangle은 Qt 帥ick에 등록된 오브젝트이며 width는 가로 크기 , height는 세로 크기이다．
36呱360의 사각형 영역의 오브젝트가 생성된다. w姓th와 he琯ht는 Rectangle의 오브젝트로써 다음과
같은 프로피 티를 제공한다．

 항목                            예제코드
 border, color                 Rectangle
                                    width: 100
 border . width
                                    height: 100
 color                              color: "red"
 gradient                           border.color: "black "
                                    border.width: 5
radius
                                    radius: 10
 smooth                        }



Te玭 오브젝트는 Rectangle 오브젝트의 Child 오브젝트로 텍스트를 출력할 수 있으며 폰트 지정 , 폰트
크기／컬러 등을 지정할 수 있다. 또한 표시할 텍스트 안에 HTML Tag를 사용할 수 있으며 텍스트의 컬
러를 지정하기 위해 문자 포맷을 사용하거나 hexadecimal을 사용할 수 있다．

 Text {color: "#OOFFOO ";         ...}    // GREEN


마지막으로 MouseArea는 Qt Quick에서 제공하는 오브젝트로써 마우스 이벤트를 처리할 수 있다．
OnClicked 이벤트 프로피티는 마우스 버튼이 클릭되었을 이벤트를 처리하기 위한 시그널이며 마우스
클릭 시 어플리케이션을 종료한다．

이 예제 코드에서 구조상 MouseArea는 Rectangle어］ 포함되어 있다. 그러므로 MouseArea어］서 선언
한 이벤트는 Rectangle 오브젝트에만 적용된다．


506 CHAPTER 16.. Qt Quick과 QML


===== PAGE 508 =====
互3Hel幻＼Norld




                         Helk} 넥orid




（그림） 예제 QML 코드 실행 화면



앞의 그림은 프로젝트를 실행한 화면이다. 그림에서 보는 것과 같이 Rectangle 영역 내에서 마우스 이번l
트가 발생하면 어플리케이션이 종료된다．


難Ot QML Scene
Qt는 작성한 QML 소스 코드를 디버깅이 가능하도록 QML Scene을 제공한다. 이 툴을 이용해 작성한
QML 소스 코드를 파일 단위로 디버깅이 가능하

 包 C：쀼QtWQt5요C坍5_O.Oy由isvc2珏0쀼蜘C뀌qrnscene.exe             L므三回 h 燕




                                                He的 밖아1




（그림）（거 QML Scene 실행 화면



그림에서 보는 것과 같이 帥4L Scene을 사용해 1성한 예제 QML 파일의 결과를 확인할 수 있다. QML
Scene은 Qt가 설치된 bin 디렉토리에 위치해 있


1Qt QML Viewer
QML Viewer 툴은 帥ilL Scene과 마찬가지로 巾ML을 디버깅할 수 있는 기능을 제공한다. 또한 이 툴
은 실행한 결과를 그림 파일로 스냅샷 기능을 제 . 한다. 또한 원격에 떨어진 URL을 통해 帥ilL 파일의
실행 결과를 확인해볼 수 있다. 윈도우 플랫폼에서는 파일 탐색기를 통해 QML Viewer를 실행할 수 있
으며 이 툴은 Qt가 설치된 bin 디렉토리에 위치하1 있다．




                                                                     ] （가 0네ck과 QML 507


===== PAGE 509 =====
（그림） Qt QML Viewer 실행 화면




        tl. 2 기본 타입과 확장된 데이터 타입
전통적인 Native 기반의 Qt 응용 어플리케이션 int, bool, QByteArray 등과 같이 QML에서도 기본적
으로 데이터 타입을 제공한다．

또한 날짜를 표시하거나 font를 표시하기 위해 확장된 데이터 타입을 제공한다. 따라서 이번 장에서는 기
본 타입과 확장된 데이터 타입의 사용 방법에 대해 알아보도록 하자．


S 기본 타입

 타입               설명
 mnt
                   Number 타입, 0카 0, 10, 혹은      20.
 bool              BOOL 타입의 true／伯冶e 값
 real              Decimal Number 타압(0카 1.2 또는 -29.8)
 double            Double 타압 (0카 32155. 2355)
 없ring             문자열 타입
 url               리소스의 위치를 나타내끼 위한 타입
 list             （가너L 오브젝트 리스트
 var              일반적인 프로퍼티 타입
enumeration        열거형 데이터 타입



m1lt 타입은 숫자를 표시하기 위해 제공하는 타입이다. 표현할 수 있는 범위는 -2,000,000,000에서
2,000,000,000 범위까지 표현할 수 있다．

 Item {
         width: 100; height: 200
 }




508 CHAPTER 16_ （그tQuick과 （가너L


===== PAGE 510 =====
bool 타입은 이진 true/false 값을 표시하는 타입 이며 다음과 같이 사용할 수 있다．

         {
         us: true; clip:   false

L



real 타입은 Decimal number 타입을 표시하기 위한 타입 이다．

r4iem {
        width: 100. 45;
        height: 150. 82




double 타입은 소수점이 포함된 데이터 타입을 표시하기 위한 타입이다．

    Item {
        property double number: 32155. 2355
    }


string 타입은 "Hello world" 문자열과 같은 데이터 타입을 표현하기 위해 제공되는 데이터 타입이다．

    Item {
        text:   "Hello world! "




url 타입은 리소스의 위치를 참조하기 위해 제공되는 데이터 타입이다. 로컬에 존재하는 그림 파일 또는
"http: //www. q卜dev. corn" 과 같은 원격의 리숙스 파일을 참조할 수 있다．

    Image
    {
        source: "pics/ logo.png"
    }


URL은 "#" 과 같은 문자가 포함되어 있는 경우 문자를 Encodi培을 사용해 다음과 같이 접근할 수 있다．

    工mage
    {
        source: encodeURlComponent ( "/ tmp/ test#l. png" )
    }


    list 타입은 帥4L의 오브젝트 리스트를 참조하기 위한 목적으로 제공하는 타입이다. [ ］와 같은 대괄호를
    사용하며 리스트의 각 오브젝트는 "," 를 사용해 구분한다．




                                                              1 Qt C네ck과 CML 509


===== PAGE 511 =====
  Item {
       width: 100; height: 100


       S七a七es: [
          S七a七e { name: "a（比iva七ed" }r
         S七ate { na工ne: " deac七iva七ed " }
       ]

       Component . onCompleted: {
          console.log ( "Name of first state: ", statesl0] .name)
           for (var i = 0; i < states.length; i++)
               console, log ( "s七a七e ", i, 5七a七es [ii .name)
       }
  }


var 타입은 JavaScript의 var 타입과 같이 숫자, 문자, 오브젝트, 배열, 함수를 표현하기 위한 다양한
데이터 타입을 표현하기 위해1 제공한다．


       property var aNumber: 100
       property var aBool: false
       property var aString: "Hello worldt "
       property var anotherString: String( "#FF008800 ")
      property var aColor: Qt.rgba(0. 2, 0.3, 0. 4, 0. 5)
      property var aRect: Qt.rect (10, 10, 10, 10)
      property var aPoint: Qt.point (10, 10)
      property var aSize: Qt. size (10, 10)
      property var aVector3d: Qt.vector3d(100, 100, 100)
      property var anArray: [1, 2, 3, "four ", "five ",
                                      (function() { return "six "; H]
      property var anObject: { "foo": 10, "bar ": 20 }
      property var aFunction: (function() { return "one"; })
 }


enumeration 타입은 열거형 데이터 타입을 표현하기 위해 제공한다．

 Text {
      horizontalAlignnient: Text .AlignRight




S 확장된 데이터 타입
확장 데이터 타입은 QML에서 제공하는 기본 타입의 확장된 형태로 다음과 같은 데이터 타입을 제공한다．




510 CHAPTER 16_ Ct Quick과 QML


===== PAGE 512 =====
                타입                   설명
                date                 날짜를 표현하기 위한 타입
                口이ft                 x, y와 같은 좌표 지점을 표시
                rect                 X, Y, Wk朮h, H이ght와 같이 사각형을 표시
                듸 ze                 이미지와 같은 WI비h, h이ght를 표시
                time                 바:mm:ss 형식의 시간을 표시
                C이or                 red, 아een 또는 Iightstee比기ue와 같은 색상을 표시하기 위해 사용한다．
                                     문자열 형태 이외에도 #RRGGBB (#FF0000）와 #AARRGGBB (#800000FF)
                                     같이 방식으로도 사용 가능하다．
                幻nt                  OFont 프로퍼티를 표시하기 위한 데이터 타입
                vector2d             x, ' ' 좌표 속성을 가지는 타입 표시
                vector3d             x, y, z 좌표 속성을 가지는 타입 표시
                vector4d             x, y, z 좌표에 w를 포함하는 속성을 가지는 타입 표시
                quaterr기山n           Scalar, X, Y 그리고 z 속성을 가지는 타입 표시
                matrix4x4            4 x 4 (16개）의 타입 표시


    date 타입은 "YYYY小4M-DD" 형태의 타입을 표시하기 위한 타입을 생성할 수 있다．

                MyDatePicker {
                       minDate: "2000-01-01"; maxDate: "2020-12-31"
                }


  point 타입은 x, y 속성을 표시하기 위해 사용하는 데이터 타입이다．

!Custom0bject
                       myP。 intPr。
                                     {perty: "。,2。
point 타입은 QML에서 제공하는 p아nt( ) 함수에 다음과 같이 사용할 수 있다．

                Cus七omObj ec七 {
                       myPointProperty: Qt.point (0, 20)




rect 타입은 x, y와 더불어 \vidth와 height 속성을 표시하기 위해 제공하는 타입이다．

                Re（北angle
                {
                       wid七h: childrenRec七 . wid七h
                       height: childrenRect.height


                       Rectangle { width: 100; height: 100 }
                }




                                                                                            1 Qt Quick2F QML 511


===== PAGE 513 =====
width와 height 값을 표시하기 위해 "w姓th x height" 와 같은 방식으로 사용할 수 있다．

CustomObject

{
     myRectProperty: "50, 50, 100x100 "

}


rect 타입은 Qt에서 제공하는 rect( ) 함수어］ 인자로 사용할 수 있다．

CustomObject


     myRectProperty: Qt.rect (50, 50, 100, 100)




size 타입은 width와 height 속성을 표시하기 위해1 제공되는 타입이다. 예를 들어 이미지의 SIZE를 표
시하기 위해f 다음과 같이 사용할 수 있다．

Column    {
     Image { id: image; source: "logo.png" }
     Text { text: image. sourceSize.width + ", " + image. sourceSize.height }




또한 w姓th와 height 속성을 "w姓th x height" 와 같은 스타일로 표시할 수 있다．

Image {
     sourceSize: "150x50 "




Qt에서 제공하는 size( ) 함수에서 다음과 같이 사용할 수 있다．

Image {
   sourceSize: Qt. size (150, 50)
}


time 타입은 "hh:rnm:ss" 와 같은 스타일로 시간을 표시하기 위한 타입을 제공한다．

MyTimePicker {
     time: "14:22:15 "
 }


C아or 타입은 "red", "blue", "green" 또는 "lightsteelblue" 와같은 컬러를 지정하기 위한 타입이다. 이
타입은 "#RRGGBB" (#FF0000) 또는 "#AARRGGBB" (#800000FF）와 같은 스타일로 컬러를 표시할
수 있다．



512 CHAPTER 16_ Cl Quick과 CML


===== PAGE 514 =====
    Text {
        color: "red"
!   }    Component. onCompleted: console. log (color. r,       color.   g,   color.   b,   color,   a)
font 타입은 QFont 타입을 사용하기 위해 제공되는 타입이다. 九nt 타입은 일반적으로 다음과 같은 폰
트 타입과 폰트의 크기를 지정하는 속성을 제공한다．

    분류                       타입
프로퍼티                         string font.tamily
                             bo（引 幻nt.b이d
                             bool font.italic
                             bad1 tont.underIine
                             real font.pointSize
                             mnt tont.p以이Size
폰트 크71 속성                    enumeration font.weight
(p이nt와 p以이 지원）               bool tont.overline
                             bool tont.strikeout
                             enumeration tont.capitalization
                             real 幻nt.letterS口acing
                             real font.wordSpacing



폰트의 Scale어］ 대한 가중치佃eighting）를 지정하기 위한 범위는 0에서 99까지 지정할 수 있다. 표에서
보는 것과 같이 폰트와 속성을 지정하기 위해 다음과 같이 사용할 수 있다．

    Text {
       font. family: "Helvetica"; font.pointSize: 13; font.bold: true
    }
                                                                                                                 j
vector2d 타입은 x, y 좌표 속성을 표시하기 위해 사용되는 타입이다. vector2d 값은 " x, y " 형태의 문
자열 스타일로 표시할 수 있으며 Qt에서 제공하는 vector2d( ) 함수에서 사용할 수 있다．

    var a = Qt.vector2d(1, 2) ; var b = Qt.vector2d(3, 4) ;
    var c = a.dotProduct (b) ;
    console.log(c) ; II 11

    var a = Qt.vector2d(l, 2) ;
    var b = Qt.vector2d(3, 4) ;
    var c = a.times (b) ;
    console.log(c.toString() ); 7/ QVector2D (3, 8)


vector3d 타입은 x, y 좌표 속성에 z 속성을 표시할 수 있으며 Qt에서 제공하는 vector3d( ) 함수에 다
음과 같이 사용할 수 있다．




                                                                                                ] （거 0비ck과 QML 513


===== PAGE 515 =====
Ro七a七ic：玎l {
    angle: 60; axis: "0,1, 0 "
}

Rotation {
    angle: 60; axis: Qt.vector3d(0, 1, 0)
}


vector4d 타입은 x, y, z 좌표에 \7T 속성을 사용할 수 있으며 , Qt에서 제공하는 vector4d( ) 함수에서
다음과 같이 사용할 수 있다．

var a = Qt.vector4d(1,2,3, 4) ;
var b = Qt.vector4d(5, 6, 7, 8) ;
var c = a.dotProduct (b) ;
console.log(c) ; II 70



quaternion 타입은 Scalar, X, Y, Z 속성을 표시하기 위한 타입이다. 컴포넌트의 속성에 사용할 수 있
으며 Qt에서 제공하는 quaternion( ) 함수에서 사용할 수 있다．
matrix4x4 타입은 16개의 값을 표시할 수 있다. 즉 행과 열을 표시하기 위한 방법으로 사용하며 행렬을
표시할 때 유용하다．

var a = Qt.matrix4x4 (1, 2, 3, 4, 5, 6,7, 8, 9,10,11,12,13,14,15,16) ;
var b = Qt.matrix4x4 (4,5, 6,7, 8, 9,10,11,12,13,14,15,16,17,18,19) ;
var c = a. times (b) ;


console.log(c. toString(fl;
// QMatrix4x4 (120, 130, 140, 150, 280, 306,
/1 332, 358, 440, 482, 524, 566, 600, 658, 716, 774)




     1.3 아이템

Qt Quick에서 제공하는 아이템은 GI끄를 구현하기 위해 제공하는 오브젝트를 말한다. 예를 들어 C++
기반에서 전통적인 QWidget, QPushButton, QLineEdit 등을 사용해 GUI를 구현하는 것과 같이
QML을 히용해 GI끄를 구현할 수 있도록 다양한 시각적 인 오브젝트를 제공한다．

아이템 속성은 아이템의 내부 영역을 Gradient와 같은 속성을 지정하여 아이템 내부 속성에 대한 접근
등을 다루기 위해1 제공된다. 아이템의 생성은 Repeater를 사용해 연속적인 아이템을 생성하기 위해 제
공된다. 그리고 파일과 같이 미리 정의된 아이템을 사용하기 위해 Loader어］ 대해 다룰 것이다. 마지막으
로 아이템의 변환은 아이템의 이동, Scale, Rotati아i, Translate 등과 같은 아이템의 변환에 대해 알아
보도록 하자．




514 CHAPTER 16_ （그'a내ck과 QML


===== PAGE 516 =====
분류                  종류               설명
타입                  Rectangle        사각형 타입의 아이템
                    Image            이미지를 표시하기 위한 아이템
                    Borderlmage      지정한 영역에 Backgr（그und 이미지를 표시
                    Animatedlmage    움직이는 （引F와 같은 아이템을 표시하71 위한 아이템
                    AnimatedSprite   연속적인 프레임을 사용하1 애니메이션을 표시하71 위한 아이템
                    SpriteSequence   여러 아이템을 연속적인 프레임을 사용하1 표시
                    Text             문자열을 표시하기 위한 아이템
                    Window           상위 윈도우를 생성하기 위한 아이템
                    Item             사용자 정의 아이템
                    Anchors          레이아웃을 정의
아이털rAcces듸b咆                         아이템 속성 접근
속성 정의               Gra비ent          색상 Gra데ent를 정의
                    GradientSt（그口    영역 내에서 사용할 색상을 정의
                    SystemPalette    （거에서 제공하는 P쉐ette에 접근하기 위한 속성
                    Screen           아이템이 표시된 영역에 대한 정보
                    Sprite           표시된 아이템의 애니메이션 지정
                    Fon止oader        URL 또는 폰트 이름을 사용할 폰트 지정
Repeater2F Loader   Repeater         생성한 여러 아이템을 모델에 적용하71 위하1 제공
                    Loader           모듈 및 파일과 같이 분리된 아이템을 표시
Transformation      Transforn)       아이템의 변환
                    Scale            아이템의 스케일
                    Rotat山n          아이템의 회전
                    가ans冶te          아이템의 동작 속성 정의




1.   3.   1 타입
Rectangle은 사각형 타입의 아이템을 표시하7 위해 제공된다. Image는 영역에 이미지를 표시하며
Borderlmage는 각 Border 영역에 이미지를 사용해 표시하기 위해1 제공된다．

Animatedlmage, AnimatedSpr此e, Spri扼Sequence는 아이템 영역에 연속적인 프레임을 사용해 애
니메이션을 표시하기 위해 사용한다. Te砒는 문자열을 표시하며 硼ndow는 상위 윈도우를 생성하고
Item은 여러 타입을 지정한 사용자 정의 Item을 지정하기 위해 사용한다．




                                                                      ] （거 a미ck과 QML 515


===== PAGE 517 =====
的 Rectan이e과 중첩（Ne없ed) Rectang厄

impor七 Q七Quick 2. 0


Rectangle {
     wid七h: 400; heigh七： 400 // 전체크기
     color: "gray"

     Re（北angle { // 상단 Rectangle
          x: 50; y: 50 // x, y 좌표
          width: 300; height: 150
          color: "lightblue "


          Rec七angle { I/ 상단 중첩 Rec七angle
              x: 50; y: 50
              width: 50; height: 50
              color: "white"
          }
     }

     Rectangle { // 하단 Rec七angle
          x: 50; y: 200
          width: 300; height: 150
          color: "green"


          Re（北angle { // 하단 중첩 Re（北angle
              x: 100; y: 50
             width: 150; height: 50
              color: "blue"
          }
     }
 }

0Rec怡ngle의 Color

import QtQuick 1. 0

Item {
     width: 300; height: 100


     Re（北angle {
          x: 0; y: 0;
         width: 100; height: 100;
          color: "#ffoooo "
     }

     Rectangle {
          x: 100; y: 0;
         width: 100; height: 100
          color: Qt.rgba(0, 0. 75, 0,1) II   R, C, B, Alpha 범위 0. 0 - 1. 0




516 CHAPTER 16中 （그tQ네ck과 CML


===== PAGE 518 =====
        Rectangle {
                 x: 200; y: 0;
                width: 100; height: 100;
                 color: "blue "
        }
}


eImage
import QtQuick 2. 0


Rectangle
{
        width: 300; height: 300
        color: "white "


        Image
        {
                 x: 63; y: 120
                 source: " . /images/qtlogo.png"
            }




1Borderimage
Borderlmage는 Border 영역을 이미지로 사용하기 위해 제공하는 아이템 타입이다. Border 영역을 9
개로 나누고 각 영역을 프로퍼티를 사용레     '1 지정한다．




（그림） Border 영역



각 Border 라인은 Source 이미지의 각 Edge 부분을 픽셀 Offset으로 지정한다. 아래 그림은 Image와
Borderlmage의 차이점이다．

    II Image 아이템을 사용한 경우
    Image
    {
            source: "pics /borderframe . png "
    }




                                                     1 Qt Quick과 QML 517


===== PAGE 519 =====
          II   Borderlinage 아이템을 사용한 경우
          Borderlmage {
               width: 180; height: 180
               加rder {
                    left:    30; top: 30; right:   30; bottom: 30
               }
               hor妃on七alTil帥幻de: aorderlmage . Stretch
                verticalTileMode: Borderlmage . Stretch
                source: '1 pics/ borderfraxne . png"




          心 AnimatedImage
 Animatedlmage 타입은 GIF와 같이 움직이는 이미지를 표시하기 위한 아이템 타입이다. 움직이는 이
미지의 시작과 정지는 히ayii培과 paused 프로퍼티를 이용해 조작할 수 있다．

!import
                      QtQuick 2. 0


          Re（北帥gle {
               width: animation.width; height: animation.height + 8


                Animatedlmage { Id: animation; source: "animation. gif " }


               Re（北angle {
                       proper七y mnt fra工nes: anima七ion. fr可陀Count


                       width: 4; height: 8
                        x: (animation.width - width) * animation.currentFrame I   frames
                       y: anima七ion.heI드；h七
                       color: "red "                                                 口


                }
          }


      0Text
Te砒는 지정한 폰트를 사용해 화면상에 글자를 출력한다．

          Text {
                text:       "Hello World! ";
                font. family: "Helvetica";
               font. pointSize: 24
                color: "red"




또한 T幼ct는 HTML 스타일로 표시 가 가능하다．




  5侶 CHAPTER 16_ Ct C네ck과 QML


===== PAGE 520 =====
Text {
        text:     "<b>Hello</b> <i>World!</i> "
}

0Item
Item은 Qt Quick에서 제공하는 기본 타입이며 사용자 정의 위젯과 같이 여러 아이템을 중첩해 하나의
아이템 타입을 만들 때 사용하면 유용하다．

import QtQuick 2. 0


Item {
        Image {
            source: ntile. pngu
        }
        Image {
            x: 80
                 width: 100; height: 100;
                 source: n tile. pngn
        }
        Image {
            x: 190
                 width: 100; height: 100
                 filiMode: Image. Tile
                 source: "tile. png"
         }
    }


0Anchors
Anchors는 QML에서 레이아웃을 사용해 아이템을 정렬하기 위한 프로퍼티를 제공하며 정렬하는 기준
에 따라 Margin을 사용할 수 있다．
             C
             시      r                                                    !
        O
        r
        1    t
             O      e
                    t
        h    2n     n
                    e

             나       帥

                               top

                               verticalCentei

                               bottom


                      러U
                       n   U
                           八
                                웃
（그림） Ancho田




                                                  ] Ot Quick과 （가너［ 519


===== PAGE 521 =====
  import QtQuick 2. 0

 Rectangle {
        width: 300; height: 300
        color: "lightblue"
            id: rectanglel

            Text
         {
                        text: "Centered text ";
                        color: "green"
                        font. family: "Helvetica";
                        font.pixelSize: 32
                        anchors. centerln: rectangle1
            }
  }


anchors. cei此erln은 id 프로퍼티가 rectanglel인 아이템의 중앙에 Te砒 아이템을 정렬한다. Id 프로
퍼티를 명시하는 방법 이외에 "parent" 를 명시해 부모 아이템을 기준으로 정렬할 수 있다．

 import QtQuick 2. 0


 Rec七angle
 {
         width: 300; height: 300
         color: "iightblue"

         Tex七
        {
                       text: "Centered text ";
                       color: "green"
                       font. farnhiy: "Helvetica";
                       font.pixelSize: 32
                       anchors .centerln: parent
         }
 }


Text 아이템을 부모 Rectangle 아이템 영역의 오른쪽어］ 정렬하기 위해 anchors,right 프로퍼티 옵션
을 사용할 수 있으며 더불어 오른쪽 영역에 Margin을 사용할 수 있다．




                               rightMargrn



                bottomMargin
（그림） Anch아S의 margin



520 CHAPTER 16_ （그tQuick과 CML


===== PAGE 522 =====
그림에서 보는 것과 같이 오른쪽 영 역에 Margin을 사용하키 위해 다음 예제 코드와 같이 사용할 수 있다．

import QtQuick 2. 0


Re（北angle {
       width: 300; height: 100
       color: "lightblue "


              Text {
                         y: 34
                         text:   n Hello. World! ";
                         color: "green'
                         font. family: '1 Helvetica ";
                         font.pixelSize: 32
                                       parent. rigF 七
                         anchors, right:
                         anchors. ri야比Margin: 30
              }
 }



1.3.2 아이템 속성 정의
1       Accessible
Button, Checkbox, Radiobutton 등과 같이 사용자에게 UI를 제공하기 위한 목적으로 아이템을 정의
한다. 예를 들어 Access小le의 role 프로피티를 Check Box로 지 정하고 클릭하면 해당 이벤트는
checked 이벤트가 발생할 것이다．

    button.qml

 Rectangle
    {
         id: I乂it尤（Dfl
         property bool checked: false
         property alias 七ext : bu七七onText．七ext


         //! [bu七七on]
         Accessible. name: 七ex七
         Accessible.description: "This button does " + text
          Accessible. role: Accessible.Button


          function accessiblePressAction() {
              bu七七on. clicked ( )
          }

          signal clicked




                                                              1 （거 Q네ck과 QML 521


===== PAGE 523 =====
          main仰ni
      Button {
               width: 100;                                                mm=
               height: co1un'n.h + 20;                                  Subject; 卜／scation o sos
               text:   "Send";                                          HLwe're goIng to the Dolomites this summer.

                                                                                 you also going to nortrrern Italy?
               onClicked : {
                                                                        尸orent
                    sta七us . 七e)＜七 = "Send"
               }




Access小le의 role을 지정하는데 다음과 같은 프로퍼티를 제공한다．

 R이e                                          프로퍼티
 Button                                       acces미비아가essA아ion
 CheckBox. Radiobutton                        checked
 Slider, SpinBox, Dial, ScroliBar             va山e, minimumVa山e, maximumV톄ue, ste口Size



0（計a（키ent
Gradiei式는 혼합될 두 개 이상의 색상을 이용해 정의한다. 각 색의 위치를 지정하기 위해1 범위 값으로
0.0에서 1.0 사이의 값을 사용한다．

 Rectangle {
     width: 100; height: 100
     gradien七： Gradien七 {
                    GradientStop { position: 0.0; color: "red" }
                    GradientStop { position: 0. 33; color: "yellow" }
                    GradientStop { position: 1.0; color: "green" }
               }
      }


I SystemPalette
SystemPalette는 Qt 어플리케이션 Palette어］ 접근하기 위해 제공되는 속성이다. 즉 응용 어플리케이션
윈도우에서 사용되는 표준 색상에 관한 정보를 제공한다．

 import QtQuick 2. 0


Rectangle
 'C
            Sys七emPale七te {
                   id: myPalette
                   colorGroup: SystemPalette . Active
           }
                                                                                                                      O


522 CHAPTER 16_ （그tQ니ck과 QML


===== PAGE 524 =====
    width: 640; hei야此： 480
    color: myPalette . window


    Text {
           anchors, fill:   parent
           text:   "Hello! "; color: myPalette. windowText
    }
}
                                                                                            J


小 Screen
특정 아이템이 표시된 스크린에 관련된 정보를 저］4끙한다. 예를 들어 아이템의 w姓th, height 등을 제공
한다. 그리고 이 속성을 사용하기 위해 다음과 같이 모듈을 import 해야 한다．

import QtQuick.Window 2. 0



이 속성은 내부의 아이템에만 접근할 수 있으며 1:}-음과 같이 사용할 수있다．

Rectangle {


    Tex七 . wid七h: 200


    Text {
           anchors. fill:   parent




0FontLoader
FontLoader 아이템 타입을 사용할 폰트를 지정한·다. 폰트 지정 시 , 시스템에 존재하는 폰트뿐만 아니라
URL을 사용할 수 있다．

import QtQuick 2. 0


Column {
    FontLoader {
        id:   fixedFont; name: "Courier "
    }
    FontLoader {
        id: webFont; source: "http: I/ www.q
                                           卜dev . com/myf on匕七七f "
    }

    Text { text:      "Fixed-size font "; font. family: fixedFont.name }
    Text { text:      "Fancy font ";   font. family: webFon七．no工［le }




                                                                           ] （그tQ네ck과 QML 523


===== PAGE 525 =====
 1.3.3 Repeater2F Loader
 DRepeater
Repeater는 비슷한 형태의 아이템을 연속적으로 지정해 표시하기 위한 속성이다．

     import QtQuick 2. 0

 Row {
     Repeater {
                model: 3
                Rectangle {
                    wid七h: 100; hei야此： 40
                    border.width: 1
                    color: "yellow"
                }
            I
 I


Repeater는 View와 같이 데이터 Model과 Delegate를 가지고 있다. Repeater의 각 아이템은 Row 또
는 Column의 포인터를 내장하고 있다．

 Column
                                                               te作10
 {                                                             tern 1
        Repeater {                                             tern 2
                                                               tern 3
           model: 10                                           tern 4
                                                               tern 5
                Text { text: "I 'm item " + index }            tern S
                                                               tern 7
            }                                                  tern 8
                                                               tern 9




0Loader
Loader는 QML 컴포넌트를 동적으로 로딩해 사용할 수 있다. 예를 들어 다른 QML 파일어］ 정의된
QML 컴포넌트를 로딩하기 위한 목적으로 사용된다. 다음 예제 소스 코드는 마우스 이벤트가 발생하면
Pagel.qml을 로딩하는 예제이다．

 import QtQuick 2. 0

 Item {
        width: 200; hei야比： 200

        Loader { id: pageLoader }

        MouseArea {
                anchors. fill: parent
                onClicked: pageLoader. source = "pagel.qml "
        I
 }



524 CHAPTER 16_ （그to네ck과 OML


===== PAGE 526 =====
1.3.4 Transformation
DTrans幻rm
Transform 타입은 아이템을 Rotation, Scale, 田ranslate 속성을 변환할 수 있는 타입을 제공한다．

      import QtQuick 2. 0                                        i3HelloWarid 노놔旦心

  Re（北angle
      {
              width: 200; height: 200


              Image{
                                                                             p1
                      x: 60; y: 60
                      source: "images /HelloWorld80 .png"
                      ro七a七ion: 45 II 45도 회전
              }
      }
      import QtQuick 2. 0                                        i=] 'eIIowor1d   口


      Rectangle
      {
              width: 200; height: 200


              Image{
                      x: 60; y: 60
                       source: "images/HelloWorld80 . png"
                       scale: 1. 5 // 1. 5배 크:7厚 확대
              }

七p。
              rt      QtQuick 2. 。                               刃 HeIIoV以州d


      Rectangle
          {
              width: 200; height: 200
              Image
              {
                       x: 60; y: 60
                       source: "images/HelloWorld80 .png"
                                                                                         J

                       transform: Translate { x: -60; y: -60 }
                  }
          }




                                                                             ] （코 O비ck과 QML 525


===== PAGE 527 =====
 Rotation 타입은 아이템의 회전 방향으로 3D와 같이 z축을 사용할 수 있다．

 import QtQuick 2. 0
 Row { x: 10; y: 10; spacing: 10
     Image { source: "images/HelloWorld80.png" }
     Image { source: "images/HelloWorld80 .png"
          transform: Rotation {
              origin. x: 30; origin. y: 30; axis { x: 0; y: 1; z: 0 } angle: 18
          }
      }
      Image { source: "images/HelloWorld80.png"
          七ransform: I之ota七ion {
              origin. x: 30; origin. y: 30; axis { x: 0; y: 1; z: 0 } angle: 36
          }
      }
     Image { source: "images/HelloWorld80 .png1'
         transform: Rotation {
              origin. x: 30; origin. y: 30; axis { x: 0; y: 1; z: 0 } angle: 54
          }
     }
     Image { source:  'images/HelloWorld80.png"
          transform: Rotation {
              origin. x: 30; origin. y: 30; axis { x: 0; y: 1; z: 0
                                                                      } angle: 72
          }




（그림） z축을 사용한 Rotat山n 예제 실행 화면




   t1.4 사용자 입력과 이벤트 처리
C++ 기반의 어플리케이션의 사용자 입력과 이벤트를 처리하기 위해 시그널과 슬롯을 사용했던 것과 같
이 Qt Quick에서도 사용자 입력을 마우스와 키보드 입력 및 이벤트를 처리할 수 있는 인터페이스를 제
공한다．




526 CHAPTER 16小 （그to네ck과 CML


===== PAGE 528 =====
타입                        설명
MouseArea                 특정 아이템 내에 마우스 이벤트 처리
Keys                      키 입력을 조작하기 위하1 제공하는 추가 프로퍼티
KeyNavigatioin            화살표 방향의 키 내비게이션을 지원
FocusSc야）e                키보드 포커스 조정
Flickable                  "川cked"를 처리할 수 있는 C urtace 제공
PinchArea                 단순한 F긔nch Gesture 조작을 활성화 하기 위한 타입
MultiPointTouchArea       멀티 터치 포인터를 조작하기 위한 활성화 처리

［가ag                      아이템의 ［가ag와 ［가op을 지정하기 위한 타입
DropArea                  특정 영역에서 ［가ag와 Drop을 지정하기 위한 타입
Textinput                 사용자의 키 입력을 처리
TextEdit                  텍스트를 수정할 수 있는 Tex Editor
TouchPoint                 터치의 좌표와 관련한 정보를 포함하는 타입
PinchEvent                Pinch 영역에서 이벤트 처리
WheelEvent                마우스 wheel 이벤트와 관련한 정보를 제공
MouseEvent                마우스 이벤트와 관련한 정보를 제공
KeyEvent                   키 이벤트와 관련한 정보를 제공
［가agEvent                 ［가ag 이벤트와 관련한 정보를 제공



0Mouse와 이벤트 처리
c++ 기반의 어플리케이션에서 위젯상에 마우스 이벤트 시그널이 발생하면 연결된 슬롯이 실행된 것과
같이 Qt Quick의 아이템 영역 마우스 이벤트가 처리할 수 있도록 아이템 영역 안에 MouseArea를 선언
해야 한다．

import QtQuick 2. 0


Rectangle {
       width: 300; height: 300; color: "lightblue "
       Text {
            anchors. horizontalCenter: parent horizontalCenter
            anchors. verticalCenter: parent. verticalCenter
            七e그＜t: "Press me " ; 如毗．pixelS뇨e: 48
            MouseArea {
                 anchors. fill:   parent
                 onPressed: parent.color = "green"
                 onReleased: parent.color = "black "
             }
       }
 }


anchors, fill 프로퍼티의 값으로 parent를 지정하게 되면 Text 영역에서 선언한 onPressed와 on-
Released 이벤트가 처리된다．




                                                                 ] （그tQuick과 C）卜기［ 527


===== PAGE 529 =====
        Text {


                 MouseArea {
                        anchors. fill:   paren七 // 이벤트를 처리할 아이템 지정


                 }
        }


    시그널 슬롯 방식과 같이 시그널과 슬롯을 구분할 수 있는 프로퍼티가 있다. onPressed는 마우스가 클
    릭되었을 때 Parent Element 컬러가 녹색（green）으로 변경되고 마우스가 클릭된 상태에서 Released
    되면 Parent Element 컬러가 검은색（black）으로 변경된다. 즉 onPressed와 onReleased 프로퍼티는
    시그널이며 프로퍼티의 값은 슬롯으로 이해하면 된다．

     Text {


                 NouseArea {


                         onPressed: paren七．color = "green"   // 시그널과 슬롯
                         onReleased: paren七．color = 1七lack " // 시그널과 슬롯
                 }



    onPressed와 onReleased 이벤트 시그널 이외에도 마우스 입력 이벤트 시그널을 처리하기 위해 다음과
    같은 이벤트를 처리할 수 있다．

    이벤트                     설명
    Mouse movement          아이템 영역에서 마우스를 움직였을 때 발생하는 이벤트
    Mouse 에ck               아이템 영역에서 마우스 버튼을 클릭했는지 확인하기 위한 이벤트
    Mouse dragging          아이템 영역에서 마우스를 드래그 했을 때 발생하는 이벤트



    마우스 이벤트가 활성화 될 수 있도록 hoverEnabled 프로퍼티를 true로 설정하고 마우스가 이벤트 영
    역에 들어오면 mouseArea. containsMouse 프로퍼티가 true를, 그렇지 않으면 false를 리턴하도록 사
    용할 수 있다．

    import QtQuick 2. 0
    Rectangle {
        width: 400; height: 200; color: "lightblue "
        Rectangle {
            x: 150; y: 50; width: 100; height: 100
            color: mouseArea. containsMouse ? "green" : "white "


                 MouseArea { id: mouseArea
                     anchors. f ill: parent; hoverEnabled: true
                 }

!
    }       '


528 CHAPTER 16-. Ct Quick과 CML


===== PAGE 530 =====
mouseArea. containsMouse 프로퍼티가 true이면 Rectangle Elem이式의 컬러가 녹색으로 변경되고
그렇지 않으면 컬러가 흰색으로 변경된다. hoverEnabled 프로피티가 false이면 버튼이 Press된 이벤
트에만 반응한다．




                                         \



（그림） 마우스 영역 이벤트



. ［가ag와 Drop 이벤트
화면상에서 Drag와 Dr야） 이벤트를 처리하기 위해 Drag와 DropArea 아이템을 제공한다. 드래그 이벤
트에 아이템의 위치가 변경되면 아이템의 Dr아） 이벤트가 생성된다. Dr아） 이벤트는 DropArea 아이템
을 조작한다．

 import QtQuick 2. 0

 Item {
     width: 200; height: 200


     DropArea {
              x: 75; y: 75
              width: 50; height: 50


              Re（北angle
          {
                  anchors. fill:     parent
                  color: n green1'

                  visible:   parent. containsDrac




     Rectangle
    {
              x: 10; y: 10
              width: 20; height: 20
              color: "red"


              Drag. active: dragArea. drag. acti\ e
              Drag.hotSpot. x: 10
              Drag.hotSpot.y: 10

              MouseArea                                              0


                                                      ] ot O내ck과 （그ML 529


===== PAGE 531 =====
            {
                    id: dragArea
                    anchors. fill:     parent


                    drag. target: parent
                }
        }
}


毋 사용자 입력 아이템과 키 이벤트 처리
키보드 이벤트는 기본적으로 Textlnput과 TextEdit Elem이此에서 키의 입력 이벤트를 제어하거나
長雨 을 이용한 포커스 이동 및 방향키를 사용한 이벤트를 제어할 수 있다．

import QtQuick 2. 0


Rectangle {
        width: 300; height: 112; color: "lightblue "
        Textlnput {
                anchors.left:     parent.left;      y: 16
                anchors. righ七： parent. ri야此


                tex七： " En由edded Progra끄ming" ;
                font.pixelSize: 32
                color: focus ? "black " : "gray "
                focus: true
        }
        Textlnput {
                anchors.left:     parent.left;      y: 64
                anchors. right:      parent.right


                text:   "Thread Programming";
                font.pixelSize: 32
                color: focus ? "black " : "gray "
        }
 }


Te砒Input은 사용자로부터 키보드 입력을 처리할 수 있는 아이템이다. C아or, 프로퍼티의 focus가 true
이면 Textlnput의 텍스트 컬러를 검은색으로, 그렇지 않으면 회색으로 변경한다. 그리고 첫 번째
Textlnput 아이템에서만 focus 프로피티의 값이 true로 지정한 것은 첫 번째 디폴트 포커스로 지정하
기 위해 추가한 라인이다．

     첫 번째 Textiriput 의 Focus 가 true           두 번째 Textinput 의 Focus 'F true

Embedded Programming Embedded Programming「
Thread Programming   Thread Programmling
                                          i                                m




（그림） 키보드 포커스 이벤트



530     CHAPTER 16 （그tO네ck과 CML


===== PAGE 532 =====
               import QtQuick 2. 0


           Rectangle {
               width: 400; height: 200; color:           'black "

                  Rectangle { id: leftRect
                                  x: 25; y: 25; width: 150; height: 150
                                  color: focus ? "red" : "darkred"
                                  KeyNavigation . right: rightRect
                                  focus: true }


                  Rectangle { Id: rightRect
                                  x: 225; y: 25; wid七h: 150; hei야比： 150
                                  color: focus ? "#ooffoo ' : "green"
                                  KeyNavigation.left: leftRect }




KeyNavi，
                       毗ion프로퍼티는키의 방향상／하／좌누 이벤트를 처리할수 있다． 방향이외에도 區旦 이벤트
가 발생하면 KeyNavigati아i.tab 프로퍼티를 사용할 수 있고, " Sh姓＋區目" 이벤트를 처리하키 위해
KeyNavigation. backtab 프로피 티를 사용할 수 있다．

           肛yN丑寸的毗如瓦뇨ft 이벤트                       K.yl寸aviga七icn r均ht   0恥P.!畦




（그림） 키보드 KeyNavigation 이벤트



           import QtQuick 2. 0


           Rectangle {
               width: 100; height: 100; color: "black "


                  Image {
                      id: rocket
                      x: 50; y: 50
                      source: " Images/HelloWorld80 .png       n


                      transformOrigin: Item.Center
                  }

                  Keys.onLeftPressed: rocket.rotation = (rocket.rotation - 10) % 360
                  Keys.onRightPressed: rocket.rotation = (rocket.rotation + 10) % 360


                  fo（그us : 七rue
           }



                                                                                  1 0! Quick과 QML 531


===== PAGE 533 =====
                                                                      시
Keys. onLeft까essed와 Keys. onRightPressed 프로퍼티는 왼쪽과 오른쪽 방향키의 Press 이벤트
그널을 처리할 수 있으며 왼쪽 방향키 이벤트가 발생하면 10도만큼 감소시키고, 오른쪽 키 이벤트가 발생
하면 10만큼 증가한다．

Keys.onLeftPressed:rocket.rotation=(rocket.rotation-10)% 360




Keys.on대아出가essed:rocket.r아帥On늬rocke口이計In너0)% 360
 i= ｛二n




（그림） Keys.onLef t가essed와 Keys.onRightF가essed 이벤트




     打百］아0벰 Positioning
QML에서 사용한 아이템의 위치 정보를 얻기 위해 Positioner를 제공한다. 열, 행과 같이 배열 형태의
수직 방향의 C아umn, 수평 방향의 Row 아이템을 제공한다. C아umn과 Row 아이템과 같은 아이템을
Child 아이템으로 포함하기 위해 Grid 아이템을 제공한다．

Flow 아이템은 아이템을 배열하는 방향을 지정할 수 있다. 예를 들어 왼쪽에서 오른쪽으로 지정할 수 있
고 반대로 오른쪽에서 왼쪽으로 아이템을 배열할 수 있다．

Layout八/lirroring 아이템은 Row와 Column과 같은 아이템을 화면상어］ 표시할 때 마치 거울어］ 아이템
이 비춰진 것과 같이 수평 방향으로 아이템을 반대로 표시하기 위한 아이템이다. 이번 장에서는 지금까지
 언급한 Positi아血培과 관련된 아이템의 사용 방법에 대해 알아보자．

 타입                 설명
 Posit山ncr          Re口eater와 같은 아이템에서 Child 아이템에 대한 정보를 제공
  C이umn             배열과 같이 Co山mn 형태로 아이템을 표시
  Row                배열과 같이 Row 형태로 아이템을 표시
  Grid               Row와 Co山mn을 Child 아이템으로 포함하며 Grid 형태로 표시
  Flow               Flow 아이템은 Child Text 아이템을 나란히 배치하기 위한 기능을 제공
  LayoutM町oring      마치 거울에 비친 것과 같이 Child 아이템을 수평 방향으로 아이템 표시



 S Positioner
 Positioner 아이템은 C아umn, Row, Flow 및 Grid와 같은 Child 아이템을 가지고 있는 상위 아이템에


 532 CHAPTER 16_ （코 0네ck과 QML


===== PAGE 534 =====
서 특정 Child 아이템의 위치정보를 제공한다. 특정 아이템이 몇 번째 아이템인지 알기 위해 Positio
ner의 index 프로퍼 티를 사용하면 된다．

그리고 특정 아이템이 첫 번째 아이템인지 알기 위해 is까rstltem을 사용해 확인할 수 있다. 만약 첫 번
째 아이템이라면 isFirstitem은 true를 리턴하고 그렇지 않으면 false를 리턴한다. 이와 반대로 마지막
아이템인지 확인하기 위해 isLastltem 프로퍼티를 사용할 수 있다．

import QtQuick 2.0

Grid {
    Repeater {
       model: 16


           Rectangle {
               id: rect
               width: 30; height: 30
               border.width: 1
               color: Positioner.isFirstltem ? "yellow" : "lightsteelblue"

               Tex七 { 七e）比： rec七．Posi七ioner. index }
           }
       }



0c이umn
              （兀lumn)을 따라 아이템을 표시한다. 따라서 anchors를 사용하지 않고 연속적
C아umn 타입은 단일 열（
으로 아이템을 수직 방향으로 표시하기 위해 이 타입을 사용하면 쉽게 구현할 수 있다．

 Column
 {


                                                                      I
       spacing: 2


       Rectangle { color: "red"; width: 50; height: 50 }
       Rectangle { color: "green"; width: 20; height: 50 }             1
       Rectangle { color: "blue"; width: 50; height: 20 }
 }


 0Row
Row 타입은 단을 행（Row）을 따라 아이템을 표시한다．



                                                                             I
 Row
 {
       spacing: 2
       Rectangle { color: "red"; width: 50; height: 50 }
       Rectangle { color: "green"; width: 20; height: 50 }
       Rectangle { color: "blue"; width: 50; height: 20 }
  }

                                                                       1Qt Q네ck과 QML 533


===== PAGE 535 =====
    8Grid
Grid 타입은 Grid가 포함하고 있는 Child 아이템을 행과 열이 합쳐진 그리드（Grid) 형태로 배열한다．
첫 번째 아이템의 위치는 (0,0）이며 상단에서 오른쪽 순으로 아이템을 배열한다. Grid 타입은 C아umn
프로퍼티를 제공한다. 이 프로퍼티를 이용해 한 라인에 표시할 Column 개수를 지정할 수 있다．
Column을 지정하지 않으면 디폴트로 4가 지정된다．

각 아이템간의 간격을 픽셀 단위로 지정하기 위해 spacing 프로퍼티를 사용하면 된다．




                                                                             I
    impor七 Q七Quick 2 .0


    Grid
                                                                              1
    1
        columns : 3
           spacing: 2


        Rec七angle        color: "red"; width: 50; height: 50 }
        Re（北angle        color: "green"; width: 20; height: 50 }
        Rectangle        color: "blue "; width: 50; height: 20 }
        T？口n卜 二n八］口      color: "cyan"; width: 50; height: 50 }
1          ectangle      color: "magenta"; width: 10; height: 10 }




    茹 디ow
Flow 타입은 단어와 같은 Child 아이템을 나란히 자동으로 배치하기 위해 사용할 수 있다. 각 아이템간
의 간격을 두기 위해 margins 프로퍼티를 지정할 수 있다．

그리고 Child 아이템을 배치하는 방향을 지정하기 위해 layoutDirection 프로퍼티를 지정할 수 있다．
왼쪽에서 오른쪽으로 방향을 지정하기 위해 Qt.LeftToRight enum 값을 지정하고 오른쪽에서 왼쪽으
로 지정하기 위해 Qt.RightToLeft를 지정한다. 만약 layoutDirection을 지정하지 않으면 디폴트로
Qt.LeftToRight가 디폴트로 설정된다．

    Flow
    {
        anchors. fill:    parent
        anchors.margins: 4
           spacing: 10


        Ta:＜七 { 七ext: "Text " ; 如毗．pixelSize: 40 }
        Text { text:  "items "; font.pixelSize: 40 }
        Text { text:      "flowing";    font.pixelSize: 40 }
        Text { text:      "inside";    font.pixelSize: 40 }
        Text { text: "a"; font.pixelSize: 40 }                       Text items
        Tex七 { 七e）比： "I그low" ; 如nt.pixelSize: 40 }
        Text { text: "item"; font.pixelSize: 40 }
                                                                     flowing inside a
                                                                     디ow item


534 CHAPTER 16_ （그tQ미ck과 QML


===== PAGE 536 =====
S LayoutMirroring
Layout入'lirroring 타입은 거울과 같이 수평 방향으로 아이템을 Mirrorii培한 것과 같이 아이템을 배치
한다．

Rectangle {
      LayoutMirroring. enabled: true
      LayoutMirroring . childrenlnherit:     true
      width: 300; height: 50
      color: "yellow"
      border.width: 1


      Row {
           anchors { left:    parent.left;   margins: 5   }
           y: 5; spacing: 5
           Repeater {
                model: 5


               Re（北angle {
                    color: "red"
                     opacity: (5 - index) I    5
                     width: 40; height: 40
                     Te)＜七 {
                           text: index + 1
                           anchors. centerln: parent
                     }
                 }

       }
           }
                                                              >URN.
 }



     「‘ 1.6 State와 가ansition

Animation Framework에서 Animation 아이템에 State Machine 모델링 기법을 적용한 것과 같이
QML 아이템에 State 八4achine 모델링 기법을 적용할 수 있다．

State Machine을 좀더 정확하게 말해 Finite State Machine이라고 하며 , ON/OFF 스위치와 같이 상
태가 ON, OFF인 상태를 State라 정의하고 ON에서 OFF로 바뀌는 것을 행동, 즉 Transition이라 정의
한다．




                                                               LOt O미ck과 OML 535


===== PAGE 537 =====
                                    행동（Transition) 및 이벤트




                  ITh
              ON                                              OFF
            (STATE)                                         (STATE)




             \\
（그림） State Machine 모델링 기법
                                                  /
                                    행동仟ransition) 및 이벤트




State는 QML 아이템의 상태이고 어떤 이벤트에 의해 QML Element가 이동하거나 프로피티의 속성이
변경되는 것을 Trans比ion이라 정의할 수 있다．


  S怡也

 import QtQuick 2. 0
                                                                                     ON STATE   OFF STATE

 Rectangle {
   width: 150; height: 250




                                                                                     口
   Rectangle {
            id: onElement
            x: 25; y: 15; width: 100; height: 100
   }
   Rectangle {
            id: offElement
            x: 25; y: 135; width: 100; height: 100
   }

   S七ates :                 f
       S七a七e {
            name: "on '
            ProoertvChanoes            { target: onElement; color:    "red" }
            Pr（丑氾rt兀hanoes             { target: offElement; color:   "black "   }
       }r
       S七a七e {
            name: "off "
            Prc기그er七＼/Chanoes          { target: onElement; color: "black " }
            Pr（그ner七vChanqes           { target: offElement; color: "green" }
       }                "       "




   ]

   S七a七e: "on "                                                                                             0



536 CHAPTER 了6_ Qt 0비ck과 （玉AL


===== PAGE 538 =====
    MouseArea
    1
             anchors. f ill:   parent
             onClicked: parent. state == "on" ?
                            parent. state = 'off " Darent. state = "On"

     }
}


두 개의 Rectangle 아이템을 선언하고 첫 번째 Rectangle의 id는 onElem이此이며 두 번째 Rec-
tangle의 id는 offElem아此이다. 첫 번째 State가 ON일 때 첫 번째 Rectai培le의 컬러는 빨간색으로
변경하고 두 번째1Rectangle의 컬러를 검은색으로 변경한다．

두 번째 State가 OFF일 때는 첫 번째 Rectai培k의 컬러를 검은색으로, 두 번째 Rectangle의 컬러를
녹색으로 변경한다. 그리고 디폴트 State는 ON으로 지정한다．

MouseArea에서 parei此를 지정하였으므로 onClicked 마우스 이벤트는 최상위 아이템에 적용된다. 따
라서 마우스 클릭 시 QML Element의 모든 영역이 이벤트로 지정되고 onClicked 시그널 이벤트가 발
생하면 state를 "on" 또는 "off' state로 변경된다. 예를 들어 state의 이름이 "on" 인 경우 마우스 이벤
트가발생하면 state는 "off' state로 변경되고, 凱ate가 "off' 일 경우 ''on" state로 변경된다．


0 가ansition
이전에 다루었던 Animation Framework를 QML에서도 사용할 수 있다. 이번 예제에서는 State에서
의 예제와 동일하며 on에서 off로 변경될 때, 1초를 간격으로 컬러 값이 선명해지도록 하는 Animation
을 사용해 예제를 작성해 보자．

QML에서 Animation을 적용하기 위한 방법은 다음 장에서 다룰 것이며 이번 예제에서는 쉽게 이해할
수 있도록 간단한 프로퍼티를 사용해 구현해 보도록 하겠다．

    import QtQuick 2. O


 Re（北angle {
   width: 150; height: 250


     Rectangle
         {
              id: onElement
              x: 25; y: 15; width: 100; height: 100
         }

         Rectangle
         {
              id: of fElement
              x: 25; y: 135; width: 100; height: 100
         }                                                                              0


                                                                          ] （코 O내ck과 QML 537


===== PAGE 539 =====
  S七a七es: [
       S七a七e {
               name:   ' on
               Pr（가）er七yChanqes     { target: onElement; color: "red" }
               Proper七＼rChanc：丁es   { target: offElement; color: "black " }
       }r
       State {
               name : 口 ott,
               PronertvChanoes      { target: onElement; color: 1'black " }
               PropertyChanges      { target: of fElement; color: "green" }
           }
   ]

  state: "on"


  MouseArea {
               anchors. fill:     parent
               onClicked: parent. state == "on" ?
                               parent. state = "off " : parent. state = "on"
   }

       transitions:
       [
                 Transition {
                       fr아n: 노ff, ' ; 七0: 노n"
                       Proper七yAnimati（그n           {
                              targe七： onE lemen七
                              properties: "color "; duration: 1000
                       }
                 }r
                 Transition {
                       from: "on"; to: "off "
                       PropertyAnimation
                       {
                              target: offElement
                              properties: "color "; duration: 1000
                       }




PropertyAnimation의 프로퍼티는 컬러로 설정하고 duration 프로퍼티를 1000으로 설정하면 1000
millisecond 동안 color값이 선명해지는 것과 같은 애니메이션 효과를 사용할 수 있다. 첫 번째
Transition은 "off'' 에서 "on" state로 변경되도록 지정하였고, 두 번째 Transition은 "on" 에서 "off"
state로 변경되도록 지 정하였다．

여기서는 단순히 두 개의 Rectangle 아이템을 사용한 예제를 다루었지만 아이템의 개수가 많아지면
Transition을 사용함으로써 이벤트 처리를 위한 QML 코드를 간단하고 명료하게 작성할 수 있다．


538 CHAPTER 16_ （가 (a기ck과 QML


===== PAGE 540 =====
 ON S丁ATE                                 OFF STATE

                  ....
                  첫 번째 Transition




      口           두 번짜1Transition
                  1 1 1 1

（그림） Transition 실행 화면




    t        ]Animation
QML은 Animation을 처리할 수 있는 아이템을 제공하고, Anin追tion은 QML의 아이템에 적용이 가능
하다. 즉 다음과 같은 Anim毗ion을 제공한다．

 타입                      내용
 NumberAnimation         좌표 x, Y 또는 Opacim와 같은 투명 값 등과 같이 숫자를 이용한
                          Animation을 적용
 Pro口ertyAnim계ion        RGB, width, height 등 프로퍼티에 Animation을 적용
 P이ationAnim졔ion         회전 Animation을 적용


Animation은 Linear한 방향으로 진행하는 방식을 Easing Curves를 이용해 다양한 방향으로 진행할
수 있는 기능을 제공한다. 예를 들어 시작 좌표부터 마지막 좌표까지 이동하는 경로의 진행 속도를 보간
법을 이용해 움직임의 패턴을 변경할 수 있다．

  value                    va山




              口rogress                progress

          니near                  InQuad

（그림） Easing Curves



 또한 여러 개의 Animation을 그룹으로 지정한 다음 순차적으로 Animation을 적용할 수 있는 Sequen
 -tialAnimation과 Animation을 동시어］ 처리할 수 있는 Parall이Animation을 제공한다．

  타입                          내용
  SequentialAnimation         여러 개의 Anim계山n을 순차 실행
  Paral冶lAnim계山n              여러 개의 Anim計口n을 동시 실행




                                                                    ] （코 Q비ck과 QML 539


===== PAGE 541 =====
 I Number Animation

 impor七 QtQui（그k2 .0

 Re（北angle {
    width: 430; height: 130
      color: "lightblue"


      Image {
          source: "images/HelloWorld80.png"
          x: 10; y: 20;

              Nun山erAnima七ic끄lon x
          {
                  from: 10; to: 350
                  （沁ra七ion: 2000
              }
      }
 }


NumberAnin追tion은 숫자를 이용해 Animation을 아이템에 적용할 수 있다. x, y 좌표에 지정한
Image 아이템을 2000millisecond 동안 x 좌표가 10에서 350 값으로 변경된다. 만약 duration을 지
정하지 않으면 250millisecond가 디폴트 값으로 지정된다．




                       x좌표가 ]0에서 350으로 이동



（그림） Numb아Animal口n 실행 화면



0Property Animation
PropertyAnimation은 아이템의 프로퍼티어］ Animation을 적용할 수 있다. 예를 들어 Image 아이템
의 width 또는 height와 같은 하나 이상의 프로퍼티를 지정할 수 있다．

 import QtQuick 2. 0


 Rectangle
  {
      width: 200; height: 160
      color: " li야此blue"


      Image
      {
          id: proAni
          source: "images/HelloWorld80.png"
                                                                 0

540 CHAPTER 16_ （며 0네ck과 CML


===== PAGE 542 =====
                 x: 50; y: 40;
                 width: 50; height: 50;
         }

         PropertyAnimation
         {
                 target: proAni
                 properties: "width, height '1
                 from: 0; to: 100; duration: 1000
                 running: true
         }
 }


 Prop이勺 鈿im硝on : 나넌th 와 h啣ht 촤［：甘
                                                              卜




（그림） 마operty A대m계口n 실행 화면



0Rotation Animation
RotationAnimation은 지정한 시작과 마지막 각도까지 아이템에 회전 Animation을 적용할 수 있다．

 import QtQuick 2.0


 Item {
     width: 100; height: 100


         Image {
             id: rotAni
                  source: "images/uelloWorld8o.png"
                  anchors. centerln: parent
                  smooth: true

                  RotationAnimation on rotation {
                      from: 45; to: 315
                      direc七ion: Ro七ationAnima七ion.Shor七est
                      （沁ra七ion: 1000
                  }
             }
     }




                                                                  1（그to네ck과 QML 541


===== PAGE 543 =====
from 프로퍼티는 시작 각도이며 to는 Animation의 마지막 각도이다. direction 프로퍼티는 다음과 같
은 상수를 제공한다．

상수                                   설명
RotationAnimation.Numerical           form과 to 값 까지 linear 보간법을 이용해 회전， 방향은 시계 방향
R아ationAnimat山n｛긔ockv미se              f아m과 tc) 값 까지 회전하며 방향은 시계 방향
R삿at向nAnimation.Counterclocke기se      幻rm과 to 값 까지 회전하며 방향은 반시계 방향
R아졔ionAnimation.Sh가test               f아m과 to 값 까지 회전하며 방향은 반시계 방향, STEP은 20씩 적용됨




ra
      （기ockwise                 Counterclockwise




（그림） R이ationA대m計向n 실행 화면



0Sequentia꽈 Parallel Animation
SequentialAnimation은 아이템에 여러 개의 Animation을 순서태匠 실행하며 ParallelAnimation은
병 렬（동시）로 Animation을 실행한다．

                 ion

                          Para加次nimat幻n
                              幻疳iation
     Animation                                叫
                              An rn t四n



（그림） Sequenti졔Anim帥on과 ParallelAnimation


 impor七 Q七Quick 2. 0


 Rectangle {
     width: 200; height: 200; color: "#000040 "


     Image {
         Id: aniSeq
          anchors. centerln: parent
          source: "images/HelloWorid80 .png"



     SequentialAnimation {
          NumberAnimation {
                 target: aniSeq; properties: "scale"
                 from: 1.0; to: 0.5; duration: 1000



542 CHAPTER 16_ Qt Quick2F CML


===== PAGE 544 =====
         }
         NumberAnimation {
               target: aniSeq; properties: 'opacity "
               from: 1.0; to: 0. 5; duration : 1000
         }
         running: true
     }
 }


첫 번째 Animation은 l000millisecond 초 동안 0. 51111로 축소4
                                                 '기 위한 Animation' ］며， 두 번째
Animation은 투명 값을 1.0에서 0.5까지 변화사키도록 하는 Animation이다．

  축소 애니메이션                       투명 애니메이션
                             卜                           =1仁




（그림） Sequenti졔Animation 실행 화면



 import QtQuick 2. 0


 Rectangle {
     width: 200; height: 200; color: "#000040 '


     Image {
         id: aniPara
         anchors. centerln: parent
         source: "images/HelloWorld80 .png"
     }

     ParallelAnimation {
         N그mberAnimation {
               target: aniPara; properties: "scale"
               from: 1.0; to: 0. 5; duration: 1000
         }
         Nun山erAnima七ion {
               target: aniPara; properties: "opacity "
               from: 1. 0; to: 0. 5; duration: 1000
         }
         running: true
     }




                                                               1Qt Q네ck과 （가너L 543


===== PAGE 545 =====
ParallelAnimation은 아이템에 적용된 여러 Animation을 동시에 진행할 수 있다. 예제 코드에서
Scale을 1.0에서 0.5로 축소하는 Animation과 아이템의 투명 처리할 수 있는 opacity 프로퍼티를 1.0
에서 0.5로 변경하는 Animation을 동시어］ 실행한다．

                  축소 애니메이션과 투명 애니메이션이 동시 진행




（그림） Parall이Animal口n 실행 화면



DEasing Curve
이전에 살펴보았던 Anim毗ion Framework 장에서 다루었던 Easing Curve의 기능과 동일하며 帥ilL
또한 Animation어］ Easing Curve를 사용할 수 있는 기능을 제공한다. Easing Curve는 좌표의 이동，
투명 변경, 확대 및 축소 등과 같이 Anim毗ion의 시작 시간과 마지막 시간까지 Linear한 패턴이 아닌
다양한 Curve를 적용할 수 있다．

예를 들어 아이템의 시작 좌표부터 마지막 좌표까지 이동하는 경로 진행속도를 보간하여 움직임의 패턴
을 다음 그림에서 보는 것과 같이 변경할 수 있다．

 va山e
                   (1, 1)   valu:            (1. 1)




              progress                   口rogress

         Linear                     InQuad
（그림） Easing Curve


 import QtQuick 2. 0
                                                      Va山e          (1 1)
 Rec七angle
 {
     width: 200; height: 100; color: "black "
                                                                  progress
     Image                                                   OutEx口o
     {
            id: easCur
            anchors . centerln: parent
            source: "images /HelloWorld80 .png"




544 CHAPTER 16_ （값 0네ck과 CML


===== PAGE 546 =====
        NumberAnimation
        {
              七arge七： easCur; pr아氾rties: "scale ''
              from: 0.1; to: 1.0; duration: 1000
              easing. type: "OutExpo"
              running: true
        }
    }
}


easing, type 프로퍼티에 사용할 Easing Curve를 ' ］정할 수 있으며 ' ］전에 다루었던 Animation
Framework 장을 참조하면 사용할 수 있는 Easing Curve 항목을 확인할 수 있다．


S PauseAnimation
PauseAnim毗ion은 SequentialAnimation에서 순차대로 실행하는 Animation 사이에 duration 프
로피티에 지정한 시간 동안 일시 정지하기 위해 사용할 수 있는 Anim毗ion이다．

import QtQuick 2. 0


Rectangle {
    width: 200; height: 200; color: "#000040 "


    Image {
        id: rocke七
        anchors. centerln: parent
        source: "images/He1loWorld80.png"
    }

    Sequei此ialAn如咀tion {
        NuxnberAnimation {
              target: rocket; properties: "scale"
              from: 0. 0; to: 1. 0; duration: 1000
        }
        PauseAnimation {
              duration: 1000
        }
        Nurt由erAnima七ion {
              target: rocket; properties: "scale "
              from: 1. 0; to: 0. 0; duration: 1000
        }
        running: true
    }
}




                                                        ] Qt O네ck과 OML 545


===== PAGE 547 =====
첫 번짜1Animation이 실행되고 PauseAnim毗ion은 l000millisecond 동안 일시 정지한다. Pause
Animation의 duration 프로퍼티어써 지정한 l000millisecond가 지나면 세 번째 Animation이 실행
된다．

 NumberAnimation                                        卜Jum berA nimat山0
      mm1斗mn斗mm川1nmm竹mn力甘mm甘砂
                                일시 정지 duration : 1000
                                    millisecond

（그림） Anim計幻n 실행 순서




:::;，缸1.8J 데이터의 표현

제한된 GUI 영역에 많은 양의 데이터를 효과적으로 보여주거나 핸들링하기 위해 c++ 기반의 프로그래
밍에서 데이터를 정렬하여 표시하거나, Data Model을 적용한 View, XML 모델링을 이용한 \[jew 등
다양한 표현 방식을 QML에서도 활용할 수 있는 인터페이스를 제공한다．

이번 장에서는 C++ 기반에서 사용했던 다양한 데이터 표현 방식을 QML상에서 적용할 수 있는 방법에
대해 살펴보도록 하자．


好 아이템 정렬
아이템을 그리드와 같은 스타일로 표현하기 위해 Grid 아이템 타입을 제공한다. Grid 아이템 타입은 표
시할 아이템을 정렬하기 위해 C아umns와 rows 프로피티를 제공하며 각 Elem아此간 일정한 간격 공백
을 삽입하기 위해 spacing 프로퍼티를 제공한다．

 import QtQuick 2. 0


 Grid {



                                                                            1
      x: 15; y: 15; width: 300; height: 300


      columns: 2; rows: 2; spacing: 20


      Rectangle { width: 125; height: 125; color: "red" }
      Rectangle { width: 125; height: 125; color: "green" }
      Rectangle { width: 125; height: 125; color: "silver " }
      Rectangle { width: 125; height: 125; color: "blue" }
 }



0Repeater 정렬
Grid 아이템의 C아umn과 Rows 프로퍼티로 지정한 개수만큼 일정 패턴으로 반복되는 Eleme砒를 배치
할 수 Repeater 아이템을 제공한다．




546 CHAPTER 16_ Ct Quick2F CML


===== PAGE 548 =====
    import QtQuick 2. 0


    Rectangle {
           width: 400; height: 400; color: 1'black '
           Grid {

                         y5
               x: 5; y: 5
               rc六VS :        columns: 5; spacing: 10


              Repeater {
                    model: 24 // 24개의 Rec七angle
                    Rectangle {
                         width: 70; height: 70
                         color: "lightgreen "


                         Text {
                                                            0   ]             r그
                                                                                       4
                               1/ index 숫자를 표시함
                               tex七： index                  5   6    7        8        늬
                               如nt . pointS뇨e: 30
                               anchors . centerln: parent   10 1 1   12. 13 14
                                                                          .
                         }
                    }                                       j5 16 17' 18 19
                                                                          '




                                                                                   .
              } // end Repeater
                                                            20 21    no
       } /1 end Grid                                                          23



일정 패턴으로 반복되는 아이템을 표현하기 위해 Repeater 아이템을 사용하면 유용하게 사용할 수 있
다. Repeater Element는 Rectangle 이외에 이미지와 같은 아이템을 적용할 수 있다．




                                                            여m包 自如
                                                                  q
                                                                     0 1
                                                                     1 0 1
                                                                         0 1
                                                                           0
                                                                                       아아dq
import QtQuick 2. 0




                                                                     왑匹  q
                                                                   으
Rectangle {
    width: 810; height: 310;




                                                            n愍匹m在i企
   color: "black "
       Grid {
              x: 10; y: lo
              rows: 5; columns: 5; spacing: 10
              Repeater {
                    model: 24
                                                                              Q小
                    Image {
                       source: "images/HelloWorld80 .png"



       }
}




                                                                 1 Qt Q내ck과 QML 547


===== PAGE 549 =====
  I 니St卜加del
  ListModel은 아이템을 리스트 테이블과 같은 스타일로 표현하기 위한 기능을 제공한다. 그리고 List
  Model어］ 포함된 Child 오브젝트로 ListElem아此를 정의할 수 있다．

   ListModel {
       id: nameModel
       Lis七Elemen七 { name: "Animation" }
       ListElement { name: "Network " }
       ListElement { name: "Embedded" }
       Lis七Elemen七 { name: "Desktop" }
       Lis七Elemen七 { name: "Mobile" }




  ListElement는 이전어1 C++ 기반의 Model/View 장에서 다루었던 MVC 모델 개념과 동일한 모델링 기
  법을 사용한다. Data는 ListEleme砒와 동일한 개념이며 ListModel은 가공하지 않은 Data를 다양한
  View에서 사용할 수 있도록 추상화 하기 위해 제공하는 아이템이다．


        Data




                        Editing
Rendering

                         Delegate

                    Rendering

 （그림） MVC 모델



  Delegate는 View 아이템상에 표시하는 데이터를 다양한 방식으로 Style을 변경할 수 있다. 帥ilL에서
  Delegate는 Con叩onent를 사용해 적용할 수 있다．

   import QtQuick 2. 0


   Rectangle {
       width: 150; height: 200; color: "white"

        Lis七Model
       {
               id: nameModel
               ListElement { name: "Animation" }
               ListElement { name: "Network " }
               ListElement { name: "Embedded" }


        }                                                        O


  548 CHAPTER 16_ Ot Quick과 QML


===== PAGE 550 =====
      Component
    {
             id: nameDelegate
             Text {
                  七ext: name;
                  font. pixelSize: 20
             }
      }

    ListView
    {
            anchors. fill:   parent                                       刃 MVC    眩去  1
             model: nameModel
                                                                          Animation
             delegate: nameDelegate                                       Netw아k
             clip:    true                                                Embedded
        }
}                                                                                                 /




ListModel은 원시 데이터를 ListView 아이템에서 데이터를 표현할 수 있도록 추상화하기 위한 아이템
이다. Component Element에서 text 프로퍼티는 ListElem이此에서 지정한 name 항목을 Delegate
할 수 있도록 지정할 수 있으며 소스 코드에서 보는 것과 같이 name 항목의 폰트 크기를 변경할 수
있다．

그리고 ListElem釘此는 텍스트 이외에 이미지를 사용할 수 있다． name 항목의 값은 ListView 아이템을
통해 GUI 인터페이스상에 표현할 수 있다．


1 V治ualltem卜加del
VisualltemModel은View에서 사용가는 "; ］템을 포함가고 있다． 예를 들어 View상에 표시할 ' }"］템
을 포함하고 있기 때문에 아이템을 포함하는 delegate를 필요로 하지 않는다．

import QtQuick 2. 0


Rectangle {
                                                                               Animat幻n三
      width: 400; height: 200; color: "white '                                  Netwo다（
      VisualltemModel {                                                        Embedded
             id: labels
             Rectangle { color: "#cc7777 "; radius: 10. 0
                             wid七h: 300; heigh七： 50
                             Text { anchors. f ill:   parent
                                      font.pointSize: 32; text:   "Animation"
                                      horizontalAlignment: Qt .AlignHCenter     } }

             Rectangle { color: "#cccc55 "; radius: 10. 0
                             width: 300; height: 50
                             Text { anchors. f ill: parent
                                      f on七．pointSize: 32; 七ext: "Ne七i寸ork "                          O

                                                                                      ] （코 O내ck과 （가너L 549


===== PAGE 551 =====
                                                horizontalAlignment: Qt.AlignHCenter } }


               Rectangle { color: "#99cccc "; radius: 10. 0
                           width: 300; height: 50
                                     Tex七 { anchors. fil끄                paren七
                                                font.pointSize: 32; text: "Embedded'1
                                                horizontalAligninent: Qt.AlignHCenter } }
         }

         Column {
               anchors . horizontalCenter: parent.horizontalCenter
               anchors. verticalCenter: parent. verticalCenter
              Repeater { model: labels }
         }
  }


 0XML 卜加d&
QML에서는 XML 데이터를 표현하기 위해1XmlListMod이을 제공한다. XmlListMod이은 source 프로
퍼티를 사용할 수 있다. 이 프로퍼티는 xml 파일을 지정하거나 인터넷 URL을 지정할 수 있다．


             <守工m! vers土on="l. O " en口odimq=''fl F- 81' stalld. lon. m"yes"?>
             <items>
                    mm        ink=                                                </it. m>

                 em8>



                 intModel
                 Id : 乂mn的1 l
                 Source:
                 query: "I/ it

                 XulRole { name:

                 凡URole I name :     r1link "   cry :   @link/ stringO




（그림） XPath를 이용한 데이터 매핑



query 프로퍼티를 이용해 XML의 identify 부분을 지정하면 해당 XML의 데이터를 伽ery할 수 있으며
XmlRole은 XPath를 사용해1 데이터를 XmlListModel로 Mapping 할 수 있다．



 <?刃nl version=" 1. 0 " encoding= "UTF-8 " standalone= "yes "?>
 <items>
      <item link= "http: //자ww.qt- dev.com">Qt Developer Community</item>
      <item link= " http: //www. google.com">Google</item>
      <item link= "http: //www. facebook.com">facebook< /item>
      <item link= "http: //www.Ubuntu.com">Ubuntu</item>
</items>
 Ql心
import QtQuick 2. 0
import QtQuick. XmlListModel 2. 0


550 CHAPTE只 16_ （그to너ck과 QML


===== PAGE 552 =====
Re（北angle {
    wid七h: 600; hei야比： 260
    color: "#404040 '


    XmlListModel {
             id:      xm끄幻del
             source: "items. 刃nl "
             query: "I/ item"
             xmlRole { na工［le: n七j土le" ; query: "s七ring ( ) n }
             XmlRo1e { name: "link "; query: "@link/ string () " }
    }

    Component {
            id:       xmlDelegate
            Item {
                  width: parent.width; height: 64


                  Rectangle {
                       width: Math.max (childrenRect.width + 16, parent.width)
                       height: 60; clip:      true
                       color: "#505060 "; border.color: "#8080b0 "; radius: 8
                       Column {
                             Text { x: 6; color: "white"
                                             font. pixelSize: 32; 七e)＜七： 七3上le }
                                    Text { x: 6; color: "white "
                                             f on七．pixelSize: 16; 七e）比： link            } }
                  }



    ListView {                                                   Ot Deve向0er Cc幷rimun四
                                                                 ' 'It口汭VYV比이-devc口n
             anchors. fill:         parent
             anchors.margins: 4                                  Google
                                                                 nnD:/／니꿔나a'兀이e.col,,
             model: xmlModel
                                                                 facebo아（
             delega七e: xmlDelega七e                               I"기www I     h   r


        }                                                        Ubun加
}




 :t1.9 모듈화 프로그래밍
C＋十 기반의 언어를 이용해 어플리케이션 소스 코드를 작성할 때 미리 작성해 놓은 모듈을 클래스로 만들
어 재사용하는 것과 같이 QML에서도 파일을 분리해 클래스처럼 재사용할 수 있도록 모듈 프로그래밍이
가능하다．

또한 QML에서 제공하는 Element 이외에 사용자 정의 커스텀 컴포넌트를 작성할 수 있는 방법을 제공
한다. 이번 장에서는 모듈화 프로그래밍 구조를 이용해 QML 기반 어플리케이션을 작성하는 방법에 대해
살펴보도록 하자．

                                                                                              1 （며 Q네ck과 QML 551


===== PAGE 553 =====
簪 사용자 정의 아이템과 프로퍼티
사용자 정의 커스텀 아이템을 정의하기 위해 다음 그림과 같이 프로젝트에 LineEdit. qml 파일을 추가
한다．


       아&
     自 口 qn小／unt州ed



（그림） QML 파일 추가



추가한 LineEdit. qm1 파일에 다음과 같이 소스 코드를 작성한다．

 import QtQuick 2. 0


 Rec七angle
 {
      border.color: 'green"; color: "white"; radius: 4; smooth: true


      Textlnput {
          anchors. fill: parent
          anchors .margins: 2
          七e）比： "Hello World. "
          color: focus ? "black " : "lightgreen"
          font.pixelSize: parent.height - 4
      }
 }


LineEdit. qml 파일은 Textlnput E1em이此를 이용해 사용자로부터 입력을 받기 위한 아이템으로써 다
른 QML 파일에서 사용할 사용자 정의 아이템이다. 그리고 main. qml 파일에 다음과 같이 예제 소스 코
드를 작성한다．

 import QtQuick 2. 0

 Rec七angle
 {
      width: 400; height: 100; color: "lightblue "


      LineEdit
      {
          anchors. horizontalCenter: parent. horizontalCenter
          anchors. verticalCenter: parent. verticalCenter
          wid七h: 300; heigi比： 50
      }
 }




552 CHAPTER 了6_ Ot O내ck과 QML


===== PAGE 554 =====
LineEdit. qml 파일에서 구현한 Textlnput 아이템을 main. qml 파일에서 사용하기 위해 파일명과 동일
한 아이템명을 사용할 수 있으며 , QML 파일은 같은 디렉토리 내에 위치해야 한다．

Focus Out                      Foc(好 In


                                  Hello World.
（그림） 사용자 정의 아이템 예제 실행 화면



작성한 LineEdit. qml 파일어］ 커스텀 프로퍼티를 추가할 수 있는 방법에 대긔
                                               ' 살펴보도록 가' }.
LineEdit.qml 파일에 다음과 같이 소스 코드를 추가한다．

import QtQuick 1.0

Re（北angle {
   border.color: "green"
    color: "white"
     radius: 4; smooth: true


     Te）比Inpu七 {
         id: textlnput


    }

     // 아래와 같이 소스코드 추가
     property alias message: textlnput.text




property 키워드는 c++ 기반에서 변수 선언과 같' 1 QML에서도 변수 타입을 지정긔
                                                   " 사용할 수 있는 기
능을 제공한다．

 Syntax: proF危rty <iype> <n帥e>[: <value> ]

 property string message: "Qt Developer "
 property mnt nuin: 123
 property real numfloat: 123. 456
 property bool boolcondi: true
 property url address: "http: //www.qt_dev.com"



LineEdit. qml에서 사용한 사용자 정의 property는 main. qml에서 사용할 수 있으며 이전에 작성한
main. qml 파일에 다음과 같이 소스 코드를 추가한다．




                                                     ] at a네ck과 QML 553


===== PAGE 555 =====
import QtQuick 2. 0


Rectangle {
      width: 400; height: 100; color: "lightblue "


      LineEdit {
            id: lineEdit
            anchors .horizontalCenter: parent.horizontalCenter
            anch吐s.t；아）: parent．七아）
            anchors .topMargin: 16
            width: 300; height: 50
      }

      Text {
            anchors. top: lineEdit . bottom
            anchors .topMargin: 12
            anchors . left:     parent. left
            anchors. leftMargin: 16
            text:       "<b>Message:</b> " + lineEdit. message
      }




      He加 W(：川d.
 MeBsage: Hel幻 World.

（그림） 사용자 정의 프로퍼티 예제 실행 화면



. 사용자 정의 시그널
사용자의 이벤트를 처리하기 위해 MouseArea 아이템을 사용한 것과 같이 사용자 정의 아이템상에서 시
그널 이벤트를 정의할 수 있는 signal 키워드를 제공한다．

 Signal syntax: signal <name> [(<type> <value>, ...)]

MouseArea {
      anchors. fill:         checklmage
      onClicked: if          (parent. state == "checked") {
                             parent. state = "unchecked";
                             parent. checked (false) ;
                         } else {
                             parent. state = "checked";
                             parent. checked (true) ;
                         }
 }

 signal checked(bool checkValue)


예제 코드에서 보는 것과 같이 signal을 정의하여 사용할 수 있다. checked 시그널은 마우스가 클릭되


554 CHAPTER 16_ Qt Cuick과 QML


===== PAGE 556 =====
면 bool 값어］ true 또는 false 값을 할당해 정의한 커스텀 아이템에서 시그널 이벤트를 구현할 수 있다．

다음 예제 코드는 체크박스와 같이 동작하는 커스텀 아이템을 구현하기 위한 예제 코드이다. 프로젝트어］
NewCheckBox. qml 파일을 추가하고 다음과 같이 소스 코드를 작성한다．

import QtQuick 1. 0
Item {
    width: textltem.width + checklmage.width


    Image {
        id: checklmage
         anchors. left:       parent. left
         anchors. verticalCenter: parent. verticalCenter
    }

    Text {
         id: textltem
         anchors. left:       checklmage . right
         anchors. leftMargin: 4
         anchors. verticalCenter: checklmage . verticalCenter
         text:   ''Option"
         font.pixelSize: checklmage.height -           4
    }

    S七a七es: [
         State {
              name: "checked"
              PropertyChanges { target: checklmage; source: "checked. svg" }
         }r
         S七a七e {
              name: "unchecked"
              PropertyChanges { target: checklmage; source: "unchecked. svg" }
         }
    ]

    state: "unchecked"


    MouseArea {
         anchors. fill:       checklmage
         onClicked: if        (parent. state == "checked") {
                               parent. state = "unchecked";
                               parent. checked (false) ;
                          } else {
                               parent. state = "checked";
                               parent.checked(true) ;
                          }
    }

    signal checked(bool checkValue)




                                                                       ] （그to내ck과 QML 555


===== PAGE 557 =====
체크박스 아이템과 같이 마우스를 클릭하면 State에서 정의한 이미지를 변경함으로써 체크박스와 같이
동작하도록 작성한 예제이다. MouseArea에서 사용자 이벤트가 발생하면 曲gnal 키워드에서 정의한 시
그널 이벤트가 발생한다．

디폴트로 정의한 state가 unchecked 상태에서 마우스를 클릭하면 MouseArea 영역에서 정의한 signal
의 bool 타입의 checkValue 변수가 true로 변경된다. 반대로 state가 checked 상태에서 마우스를 클릭
하면 state가 unchecked 상태로 변경되고 bool 타입의 checkValue 변수가 false로 변경된다．

다음 예제 코드는 구현한 체크박스 아이템을 사용하기 위해 main. qml에 다음과 같이 소스 코드를 작성
한다．

 import QtQuick 2. 0
 import "itemsH


Rectangle {
    width: 250; height: 100; color: "lightblue"


      NewCheckBox {
          anchors. horizontalCenter: parent. horizontalCenter
          anchors. verticalCenter: parent. verticalCenter
          onChecked: checkValue ? parent.color = "red"
                                : parent.color = "lightblue"
      }



 State - unchecked     State - checked


   口O口如n

（그림） 시그널 예제 실행 화면



이전 예제에서는 QML 파일을 분리했던 것과 같이 import를 사용하면 여러 QML 파일을 구조화된 프로
그래밍을 구현할 수 있다. 이전 예제 코드에서는 main. qml과 동일한 디렉토리어］ 위치해야 하지만
import아서 디렉토리명을 명시하고 하위에 사용할 QML 커스텀 아이템 파일을 위치하면 된다．

白 啣 QML                            1
  日口 qml/Cust口mSignal
   日 口 陀ms
        角 NewChe:lB口HJ可ni
        main qml

（그림） import 디렉토리




556 CHAPTER 16_ （그to네ck과 (y＼朮


===== PAGE 558 =====
   已，1.10, Graphic Effects
Graphic Effect는 UI 컴포넌트와 같이 Qt Quick에서 제공하는 모듈이다. QML 타입으로 제공되며
Visual 아이템에 Effect를 사용할 수 있다. 이 API는 Blending, masking, Blurring, C아oring 등 다
양한 Graphic Effect를 제공한다．

Qt Quick에서 제공하는 Graphic Effects를 QML에서 사용하기 위해 QML 파일어］ 다음과 같이
import를 추가해야 한다．

import QtGraphicalEffects 1.0


Graphic Effect를 사용하기 위해 QML Scene에 특정 Effect를 지정하고 Effect 프로퍼티를 설정하면
된다. Graphic Effect는 Visual 아이템에 하나 또는 그 이상의 Graphic Effect를 사용할 수 있다．

그리고 사용할 Graphic Effect를 다양한 Visual 아이템 타입에 적용할 수 있다. 심지어는 Video 관련
아이템에도 적용이 가능하며 파이프라인을 통해 여러 Effect를 적용할 수 있다. 이번 장에서 살펴볼
Graphic Effect는 다음 표와 같다．


eGraphic Effect

분류            타입                   설명
미end          텨end                 미end 모드를 사용하1 두 개의 이미지를 Merge
c이or          BrightnessContrast   밝it와 대조
              c이orOverlay          Overlay 컬러를 적용한 소스 아이템의 컬러를 변경
              c이orize              HSL 컬러 공간에 색상 설정
              Desaturate           색상의 채도 감소
              GammaA이ust           원본 소스 아이템의 밝기 조절
              HueSaturation        HSL 컬러 공간에 원본 아이템 컬러를 조절
              LevelAd just         RGBA 컬러 공간에 색상 레벨 조정
Gradient      Car기cal(計adient      원뿔 모양의 Gradient
              LinearGradient       선형 라인의 Gra비ent
              RadialGradierrt      반지름 패턴의 Gra데ent
［기stortion    ［기splace             변위 매핑（d巴叱cement ma이에 따라 소스 아이템의 픽셀을 이동
Dr야） Shadow    Dro口Shadow          소스 이미지에 그림자 효과
               InnerShadow         소스 이미지 안쪽에 흐릿한 효과
Blur           FastBlur            소스 아이템에 Fast Blur 적용
               Gaussian Blur       높은 Quality Blur 효과 적용
               MaskedBlur          다양한 강도를 사용한 Blur 적용
               RecursiveBlur       반복적이고 강한 Blur 적용
Motion Blur    DirectionalBiur     특정 방향에 Blur 적용
               RadialBlur          아이템 중심점을 주변에 원의 방향으로 Blur 적용
               ZoomBlur            중심점을 기준으로 Blur 적용




                                                                    ] （그to내ck과 （가너［ 557


===== PAGE 559 =====
 분류                     타입                    설명
 이ow                    （引ow                  원본 이미지에 색상과 흐릿한 효과를 생성하고 원본 이미지에서 어두우면 영
                                              역을 강조하71 위해 사용
                        Rectangu1arG1ow       사각형 영역에 색상과 흐릿한 효과를 생성하고 어두운 영역을 강조하기 위해 사용
 Mask                   OpacityMask           다른 아이템을 사용해 소스 이미지를 마스크 적용
                        ThresholMask          원본 아이템에 마스크를 적용하고 임계 영역을 적용
 다pab冶과 Shader 다口ab冶                         Surface에 ' fu r가)ing" E卄e아를 제공
                        Shader Effect        Rectangle에 Vertex와 什agment shader를 적용
                        ShaderEtfectSource   Scene상에 여러 Tex山re를 미5이ay
                        GridMesh             균등하게 배치된 그리드로 이루어진 사각형 Mesh를 정의해 특정 형상을 생
                                             성하는 Effe아에 사용하71 위한 타입
                        Ct（그uick Parhcle 2   Qf(그uick 2버전부터 제공하는 시스템 타입


 S 미end
Blend Effect는 Source 이미 지와 Foreground Source 이미 지를 혼합한 Effect를 적용할 수 있다．

          Source 이미지           Foreground Source 이미지     Effect 적용 이미지




 import QtQuick 2. 0
 import QtGraphicalEffects 1. 0


 Item {
      width: 300
      height: 300


      Image {
          id: lenna
             source: "images/lenna.png '
             sourceSize: Qt. size (parent.width, parent.height)
             smoo七h : 七rue
             visible:     false
      }

      Image {
          id: butterfly
             source: '1 images/butterfly. png"
             sourceSize: Qt. size (parent.width, parent.height)
             smooth: true
                                                                                      0


558 CHAPTER 16_ Ct Quick과 CML


===== PAGE 560 =====
             visible: false
       }

       Blend {
             anchors. fill: lenna
             source: lenna
             foregroundSource: butterfly
             mode: "average"
       }
 }


렌더링의 성능을 향상시키기 위해 Cache를 사용할 수 있다. Blend 타입에서 제공하는 cached 프로퍼티
를 true로 설정하면 Cache를 적용할 수 있다. Blend 타입에서 source 이미지 아이템과 Foreground
source 아이템을 지정해야 한다. source 이미지는 source 프로피티의 지정할 아이템을 명시한다．


" " " " " " " " " "「" " " " " 는 "" " " " " " " " " " " " " " " "］가면된다·
Blend는 다양한 Effect 모드를 제공한다. 다양한 Blend Effect를 적용하기 위해 mode를 사용해 지정
                                                     『’
                                           뜨퍼티에
할 수 있다. mode 프로퍼티어］ 지정할 수 있는 값은 다음 표와 같다．

모드               설명
normal           A巾ha 이ending을 사용해 幻regroundSource의 픽셀 값을 Source 이미지 \Nriting
addition         Source 이미지와 幻regroundSource의 픽셀 값을 같이 사용
average          Source 이미지와 幻regroundSource의 픽셀 평균 값을 구하고 Writing
C이or             Source 이미지의 밝71 값과 幻regroundSource 이미지의 hue와 saturation을 함께 사용
c이orBuri기        SoL卄ce 이미지와 toregroundSource 이미지의 어두운 색을 강조
C이or［兀dge        Source 이미지의 밝은 부분의 픽셀을 더 밝게 처리하고 toregroundSourc氾 이미지의 어두운 부분은 더 어
                 둡게 처리
darken           So（玎ce 이미지와 幻regroundSource 이미지의 어두운 부분을 표시
darkerC이or       Source 이미지와 幻regroundSource 이미지의 어두운 픽셀의 RGB 값을 낮춘다．
d咐erence         Source 이미지와 化regroundSource 이미지 사이의 픽셀의 차이점을 렌더링
（기vide           Source 이미지의 픽셀 값과 伯regroundSource의 값을 나눈다．
exclusion        Source 이미지와 toregroundSoun氾 이미지의 경감된 contra없를 사용해 차이점이 발생하는 부분을 표시
hardLight        幻regroundSource 이미지 값에 따라 Source 이미지의 픽셀 값의 밝은 부분을 더 밝게 하거나 어둡게 처리
hue              toregroundSource 이미지의 밝은 부분의 값이 합쳐지고 Source 이미지를 표시
lighten          Source 이미지와 幻regroundSource 이미지의 밝은 부분을 표시
IighterC이or      Source 이미지와 toregroundSource 이미지의 가장 밝은 RGB 값을 표시
Ii아卄ness         幻re드roundSoun兀 이미지의 밝은 부분이 합쳐지고 Soucre 이미지에 표시
multipm          Source 이미지와 幻regroundSource 이미지를 함께 표시
negat山n          Source 이미지와 toregroundSource 이미지의 반전 픽셀을 표시
saturation       幻regroundSource 이미지의 색상이 밝은 색으로 채워지고 소스의 밝기를 표시
screen           Source 이미지와 toregroundSource 이미지의 픽셀 값이 반전되고 함께 표시
subtract         toregroundSource 이미지의 픽셀 값이 Source 이미지의 픽셀을 제거
sottLight        f아egroundSource 이미지에 따라 Source 이미지의 픽셀 값을 밝게 처리하거나 어둡게 처리




                                                                          1 Qt Q네比과 C）卜／IL 559


===== PAGE 561 =====
 0BrightnessContrast
이 Effect는 Source 히미지의 Brightness와 Car此rast를 조정할 수 있다. Source 아이템의 C이or를
밝게 하거나 어둡게 처리할 수 있다．

      Source 이미지       Brightness: 0.5, Contrast: 0.5   Brightness: 1.0, Contrast: 1.0




BrightnessContrast는 cached 프로퍼티를 사용해 렌더링 수행시간을 향상시킬 수 있다. cached 프로
퍼티를 활성화 하기 위해 값으로 true를 지정한다．

 import QtQuick 2. 0
 import QtGraphicalEffects 1. 0

 Item {
     width: 300
     heigh七： 300


     Image {
         Id: lenna
         source: "images/ lenna.png"
         sourceSize: Qt. size (parent.width, parent.height)
          smoo七h : 七rue
          visible: false
     }

     BrightnessContrast {
         anchors. fill: lenna
         source: lenna
         brightness: 0. 5
         contrast: 0. 5
     }
 }




560 CHAPTER 16_ O1 Quick과 QML


===== PAGE 562 =====
茹ColorOverlay
ColorOverlay Effect는 Source 이미지 아이템의 C아or를 설정한다．

    Source 이미XL           C이0r醬808的的0"1




import QtQuick 2. 0
import QtGraphicalEffects 1. 0

Item {
    wid七h: 300
    heigh七： 300


    Image {
        id: bug
        source: n images/butterfly. png"
         sourceSize: Qt. size (parent.width, parent.height)
         smooth: true
         visible: false
    }

    ColorOverlay {
        anchors. f ill:   bug
         source: bug
         color: "#Boooffoo '
    }



毋 C이orize
C아orize Effect는 Source 이미 지 아이템의 HSL C아or 공간에 C이or를 설정한다．
                               hue: 0.0            hue: 0.8
    Source 이미지             saturat幻n: 0.5      saturation: 1.0
                           lightness: -0.2      lightness: 0




                                                                 ] （가 0uk水과 QML 561


===== PAGE 563 =====
 import QtQuick 2. 0
 import QtGraphicalEffects 1. 0


 Item {
      width: 300; height: 300


      Image {
          id: lenna
          source: "images/ lenna.png"
          sourceSize: Qt. size (parent .width, parent .height)
          smoo七h : 七rue
          visible:    false
      }

     Colorize {
          anchors, fill:   lenna
          source: lenna
          hue: 0. 0
          saturation: 0. 5
          lightness: -0. 2
      }
 }


S Desaturate
소스 이미지의 RGB 값의 포화도（desaturation）를 저하시킨다. 예를 들어 흑백으로 표시하는 것과 같이
표시된다．

     Source 이미지               desaturation: 0.5   desaturation: 1.O




 import QtQuick 2. 0
 import QtGraphicalEffects 1. 0


 Item {
     width: 300
     height: 300


     Image {
         id: bug
          source: "images/bug. jpg"
          sourceSize: Qt. size (parent.width, parent.height)


562 CHA口TER 16_ O1 0내ck과 （가AL


===== PAGE 564 =====
          smoo七h : 七rue
          visible:     false
     }

     Desaturate {
          anchors. f ill:     bug
          source: bug
          desa七ura七ion: 0 . 8
     }
 }


1GammaAdjust
GammaA由ust는 power-law expression과 같이 미리 정의된 （노rye에 따라 각 픽셀을 적용하고, 이
Effect는 감마 값을 이용해 Effect를 적용한다．

     Source 이미지                 Gamma: 0.45      Gamma: 2.0




區而r七 Q七Quick 2 . 0
 import QtGraphicalEffects 1. 0


 Item {
     width: 300; height: 300


     Image {
         id: lenna; source: "images/lenna.png"
          sourceSize: Qt. size (parent.width, parent.height)
          smoo七h: 七rue
          visible:    false
     }

     GammaAdjust {
          anchors, fill:    lenna
          source: lenna
          gall旺na: 2 . 0
     }




                                                               t （코 Q네ck과 （가너［ 563


===== PAGE 565 =====
秀 HueSa山n캐on
HueSati.才毗'on은 Colorize Effect와 비슷하다. C아orize와 차이점으로 HueSaturation은 hue와
saturation 프로퍼티를 지정할 수 있다．

                                hue: -0.3                hue: 0.3
     Source 이미지              sa山n카山n: 0.5             saturation: 0
                             lightness: -0.1          lightness: 0




import QtQuick 2. 0
import QtGraphicalEffects 1. 0


Item {
     width: 300; height: 300
     Image {
         id: lenna; source: " images/lenna.png '
         sourceSize: Qt. size (parent.width, parent.height)
         smooth: true; visible:       false
     }

     HueSaturation {
         anchors. f ill:    lenna; source: lenna
         hue: 0. 3
         saturation: 0
         lightness: 0
     }
 }


DLevelAdjust
LevelAdjust는 Source 이미 지의 각 C아or 채널을 위해 색상을 분리하기 위한 Effect를 적용할 수 있다．

                                               minimuminput: ' #00000Q70'
     Source 이미지            崙： 羅齬機瑥0 .ma
                                    minim집mumO韶尉：
                                              ＃古擢Q.0"
                                                   maximumO뺘）ut 津ttttft




564 CHAPTER 16.. Ct Quick2F CML


===== PAGE 566 =====
import QtQuick 2. 0
import QtGraphicalEffects 1. 0


Item {
    width: 300; height: 300
      Image {
          id: butterfly;   source: "images/butterfly. png"
           sourceSize: Qt. size (parent.width, parent.height)
           smooth: true; visible: false
      }

      LevelAdjust {
          anchors. fill: butterfly
           source: butterfly
           minimumlnput: "#00000070 "
           maximumlnput: "#ffffff "
           minimumOutput: "#000000 "
           maximumOutput: "#ffffff    "
      }
}


S Conic瓠3radient
ConicaiGradient는 두 개 또는 그 이상의 C이or를 사용할 수 있으며 원뿔 모양의 Gradient Effect를
제공한다. 또한 ConicaiGradient는 원뿔이 향하는 방향의 각도를 통해 지정할 수 있다．

         angIe: 0               angIe: 45           angIe: 145.5
    horizontalO卄set: 0     horizontalOfiset: 0   horizontaloffset: 0
     verticaloffset: 0      verticalOffset: 0     verticalOffset: 0




import QtQuick 2. 0
import QtcraphicalEffects 1. 0

Item {
    width: 300; height: 300
    ConicalGradient {
        anchors . fill: parent
        angle: 145. 5


           gradient: Gradient {
               GradientStop { position: 0. 0; color: "white " }                          O

                                                                       1 （코 Quick과 （外사   565


===== PAGE 567 =====
               GradientStop { position: 1. 0; color: "black " }
           }
      }



horizontalOffset 프로퍼티는 중심 좌표로부터 수평 방향으로 Gradi아此의 중심을 이동시킬 수 있다．
반대로 verticalOffset 프로퍼티를 사용하면 수직 방향으로 중심을 이동할 수 있다. 만약 지정하지 않으
면 디폴트 값으로 0이 자동으로 입력된다．


簪 니near（計adient
LinearGradiei此는 두 개 또는 그 이상의 C아or를 사용해 Linear한 Gradient Effect를 적용할 수 있
다. Linear由adient는 시작점과 마지막 지점을 지정해야 한다．


 end: Qt.point(300, 300)   end: Qt.point(150, 150)   end: Qt.point(300, 0)
   없art: Qt.口oint(0, 0)     sta比 Qt .口（키nt(O, 0)      없art: Qt,p（긔nt(0, 0)




nimpor七 QtQui（그k2 . 0
 如四吐t QtGraphicalEffects 1. 0


 Item {
     wid七h: 300
     hei야此： 300


     LinearGradient {
          anchors, fill:    parent
          start:   Qt.point (0, 0)
          end: Qt.point (0, 300)
          gradien七： Gradien七 {
               GradientStop { position: 0. 0; color: "white " }
               GradientStop { position: 1. 0; color: "black " }
          }




566 CHAPTER 16 （코 a네ck과 CML


===== PAGE 568 =====
0Ra비aiGra비ent
RadialGradient는방사형태의 Gradient Effe供를제공한다． 수평 방향으로반' ］름을 ' ］정가기 위해
horizontaiRadius오十 verticall之adius 프로퍼티뷸 사용한다．

           angIe: 0                     angIe: 45                     angle: 90
     horizontalOffset: 0          horizontalO竹set: 0            horizontalOffset: 0
      verticalOffset: 0             verticalOttset: 0             verticalOffset: 0
    horizontaiRadius: 100        horizontalRadius: 100         horizontalRadius: 100
     verticaiRadius: 300          verticaiRadius: 300           verticalRadius: 300




    import QtQuick 2.0
    import QtGraphicalEffects 1.0

    Item {
        wid七h: 300
        heigh七： 300

       RadialGradient {
           anchors, fill: parent
           gradient: Gradient {

                                                         M 叱
               GradientS七아） { posi七ion:                        color: "white " }
               GradientStop { position:                        color: "black " }
                }
        }



S［기splace


然           「변" " " " (" ' " " ' " " " ' " " "
            ""                                   " " )"］   떠   " 「「   ']   "]   ']   " ""   ]'   " " " '을
                                                                                                     「      '呼   "   "］   :   「   '］   능을 "]
                                                                                                                                          '
        Source 이미지               DisplacementSource                 Effect 적용




                                                                                                            ] （그to내ck과 CML 567


===== PAGE 569 =====
  import QtQuick 2. 0
  import QtGraphicalEffects 1. 0

 Item {
      width: 300
      heigh七： 300


      Image {
          id: lenna
          source: "images/lenna.png "
          sourceSize: Qt. size (parent.width, parent.height)
          smooth: true
          visible: false
      }

     Rectangle {
         id: displacement
         color: Qt.rgba(0.5, 0.5, 1. 0, 1.0)
         anchors. fill: parent
         visible: false
          Image {
              anchors. centerln: parent
              source: !'images/ glass normal.png "
              sourceSize: Qt . size (parent .width/ 2, parent .height/2)
              smooth: true
          }
     }

     Displace {
         anchors. fill: lenna
          source: lenna
          displacementSource: displacement
          displacement: 0.1
     }
 }


displacement 프로피티는 변위 매핑 Scale을 지정할 수 있다. 디폴트는 0.0이며 최대값은 1.0까지 지
정할 수 있다. displacementSource 프로퍼티는 변위 매핑을 적용할 아이템을 지정한다．

cached 프로피티는 렌더링 성능을 향상시키기 위한 목적으로 cache를 사용한다. cache를 활성화 하기
위해囚 true 값을 지정하면 된다. 이 프로피티는 디폴트로 false 값이 지정되어 있다．


0DropShadow
}DropShadow는 Source 이미지에 그림자 Effect를 지정하기 위한 기능을 제공한다. radius 프로퍼티
는 그림자의 부드러움 정도를 지정한다. 이 프로퍼티의 값이 클수록 그림자의 Edges 부분이 흐릿하고 일
그러지게 표시된다. 또한 그림자의 컬러를 지정하기 위해 c아or 프로퍼티를 사용할 수 있다．



568 CHAPTER 16_ Ct Quick과 QML


===== PAGE 570 =====
    color: "#000000"        color: "#0000ff"     color: "#aa000000"
        radius: 8.0            radius: 8.0            radius: 8.0
       samples: 16            samples: 16            samples: 16
    horizontalOffset: 0    horizontalOftset: 0    horizontalOtfset: 0
     verticalOfiset: 20     verticalOffset: 20     verticalO卄set: 20
         spread: 0              spread: 0              spread: 0




     k
import QtQuick 2.0
import QtGraphicalEffects 1. 0

Item {
    width: 300
      height: 300


      Re（北angle {
          anchors, fill:   parent
      }

      Image {
          id: butterfly
           source: "images/butterfly. png"
           sourceSize: Qt. size (parent.width, parent.height)
           smoc此h: true
           visible: false
      }

      DropShadow {
          anchors .fill: butterfly
           color: "#000000 "
           radius: 8. 0
           samples: 16
           horiz（그n七alOffset: 0
           verticalOff set: 20
           spread: 0
           source: butterfly
      }
}


I Inner Shadow
InnerShadow는 그림자를 Source 이미지 안쪽에 그림자 Effect를 적용하기 위한 키능을 제공한다．
radius 프로퍼티는 안쪽 그림자의 부드러움 정도를 지정한다. 이 프로피티의 값이 클수록 그림자의


                                                                        ] （그to네ck과 QML 569


===== PAGE 571 =====
Edges 부분이 흐릿하고 일그러지게 표시된다. 또한 그림자의 컬러를 지정하기 위해 color 프로퍼티를

사용할 수 있다．


  color: "#000000"           color: "#ffffff"     c이or: ' 쌔0000"
       radius: 16               radius: 16            radius: 16
     sam히Os: 24               samples: 24           sam이es: 24
  horizontalOffset: 0      horizontalOffset: 0   horizontalOffset: 0
   verticalOffset: 0        verticalOffset: 0     verticalOffset: 0
     spread: 0.2              spread: 0.2           S口read: 0.2




import QtQuick 2. 0
import QtGraphicalEffects 1. 0


Item {
    width: 300; height: 300
    Rectangle { anchors. f ill:      parent }
    Image {
        Id: butterfly;    source: "images/butterfly. png"
          sourceSize: Qt. size (parent.width, parent.height)
          smooth: true; visible:       false
     }

    InnerShadow {
          anchors, fill:   butterfly
         radius: 16; samples: 24
         horizontalOffset: 0; verticalOff set: 0
          spread: 0. 2
         color: '# 000000 "
          source: butterfly




0FastB山r

FastBlur는 GaussianBiur보다 낮은 Blur Effect를 제공하지만 렌더링 속도는 GaussianBlue 보다

빠르다．




570 CHAPTER 16느 （그tQ네ck과 QML


===== PAGE 572 =====
    Soun氾 이미지                   radius: 32      radius: 64




import QtQuick 2. 0
import QtGraphicalEffects 1. 0


Item {
    width: 300; height: 300
    Image {
        id: lenna; source: "images/lenna.png"
         sourceSize: Qt. size (parent.width, parent.height)
         smooth: true
         visible:    false
    }

    FastBlur {
         anchors. f ill:     lenna
         source: lenna
         radius: 32
    }
}


心GaussianBiur
GaussianBlui"는 Effect를 계산하기 위해 Gaussian 함수를 사용하는 알고리즘으로 Blur Effect를 이
미지에 적용한다 . FastBlur보다 높은 Quality를 제공하지만 FastBlur보다는 렌더링 속도는 느리다．

                               de＼기at田n: 2      deviation: 4
    Source 이미지                  radius: 8        radius: 8
                               samples: 16      sam이es: 16




                                                               ] Ot O네比과 QML 571


===== PAGE 573 =====
 impor七 Q七Quick 2 . 0
 import QtGraphicalEffects 1. 0


 Item {
      width: 300; height: 300


      Image {
          id: lenna
          source: "images/ lenna.png '
          sourceSize: Qt. size (parent.width, parent.height)
          smoo七h : 七rue
          visible:    false
      }

      GaussianBlur {
          anchors, fill:   lenna
          source: lenna
          deviation: 4
          radius: 8
          samples: 16
      }
 }


S MaskedB山r
MaskedBlur는 각 픽셀어］ maskSource를 적용하여 각 픽셀에 흐림 강도를 적용할 수 있는 기능을 제공
한다．

      Source 이미지              maskSource          Effect 적용




 import QtQuick 2. 0
 i四ort QtGraphicalEffects 1. 0


 Item {
     width: 300
     height: 300


     Image {
         id: lenna
          source: '1 images/ lenna.png"
          sourceSize: Qt. size (parent.width, parent.height)
                                                               0

572 CHAPTER 16_ Qt Quck과 CML


===== PAGE 574 =====
          smoo七h : 七rue
          visible: false
    }

    LinearGradient {
        id: mask
        anchors. fill:     lenna
          gradient: Gradient {
              GradientStop { position: 0. 2, color: "#ffffffff  "   }
              GradientStop { position: 0.5;  color: n #00ffffff "   }
          }
          start: Qt.point (0, 0)
          end: Qt.point (300, 0)
          visible: false
    }

    MaskedBlur {
        anchors, fill: lenna
        source: lenna
          maskSource: mask
          radius: 16
          samples: 24
    }
}


I Recur引ye텨ur
RecursiveBlur 효과는 소스를 여러 번 흐리게 하는 재귀 피드백 루프를 사용하는 알고리즘을 사용해1 이
미지를 서서히 흐릿하게 하며 부드럽게 Blur Effect를 제공한다．

        Source 이미지            maskSource          Effect 적용




 import QtQuick 2. 0
 import QtcraphicalEffects 1. 0

 Item {
     width: 300; height: 300


        Image {
            id: lenna
            source: "images/lenna.png"                                                0


                                                                        ] （코 O미ck과 QML 573


===== PAGE 575 =====
                   sourceSize: Qt. size (parent.width, parent.height)
                    smo(＞七h: 七rue
                   visible:     false
              }

              RecursiveBlur {
                    anchors, fill:           lenna
                    source: lenna
                   radius : 7 . 5
                   loops: 50
              }
          }

          務 Dire아山n텨ur
DirectionB1i才는 특정 방향으로 Blur Eff'ect를 적용할 수 있．다．

                     Source 이미지                                  Effect 적용




!import            QtQuick 2.   0    ,   ,       .   .




          impori; 닙tUrapnice工玎工rects I · U


          Item {
              width: 300; height: 300
              Image {
                  id: lenna; source: "images/lenna.png"
                    sourceSize: Qt. size (parent.width, parent.height)
                    smooth: true; visible:               false
              }

              DirectionaiBlur {
                    anchors. fill:           lenna; source: lenna
                    angle: 90
                    length: 32
                    samples: 24




     574 CHAPTER 16_ Qf Quick과 QML


===== PAGE 576 =====
S Ra비톄Blur
RadialBiur는 특정 방향으로 아이템을 회전한 것과 같은 Blur Effect를 소스 이미지에 적용할 수 있다．

          SoL卄ce 이미지                       Effect 적용




import QtQuick 2.0
import QtGraphicalEffects 1. 0
Item {
    width: 300; height: 300
    Image {
        id: lenna; source: " images/lenna.pngn
         sourceSize: Qt. size (parent.width, parent.height)
         smooth: true; visible:    false
    }

    RadialElur {
         anchors. f ill:   lenna
         source: lenna
         samples: 24
         angle: 30
    }
}


S Glow
Source 이미지의 색상을 지정하고 Blur Effect를 생성한 후 그 위에 이미지를 위치시킨 형태의 Effect
이다. 이 Effect는 소스 이미지의 Glow Effect를 제공한다．




                                                              ] （거 Q네ck과 QML 575


===== PAGE 577 =====
            Soun氾 이미지                        Effect 적용




 import QtQuick 2. 0
 import QtGraphicalEffects 1. 0

 Item {
     width: 300
     height: 300


     Rectangle {
         anchors. fill:  parent
         color: "black "



     Image {
         id: butterfly
          source: " 如略ges/ bu七terfly.png"
          sourceSize: Qt. size (parent.width, parent.height)
          smooth: true
          visible: false



     Glow {
         anchors, fill:   butterfly
         radius: 8
         sar四les: 16
         color: "white"
         source: butterfly




576 CHAPT타긋 16小 ( t Quick과 CML


===== PAGE 578 =====
簪 Rectangle Glow
Rectangle 영역에 색상을 지정하고 Blur를 생성한 후, 그 위에 Rectangle 아이템을 위치시킨다．

         Source Rectangle                     Effect 적용




import QtQuick 2. 0
import gtcraphicalEffects 1. 0


Item {
    wid七h: 300' heigh七： 300
    Rectangle {
         id: background; anchors. f ill:   pa] 'ent; color: "black "
    }

    RectangularGiow {
         id: effec七
         anchors. f ill:    rect
         glowRadius: 10
         spread: 0. 2
         color:   'whiten
         cornerRadius: rect. radius + glowl 1.adius
    }

    Rectangle {
         Id: rect
         color: "black "
         anchors. centerln: parent
         width: Math.round(parent.width /
         height: Math. round (parent.height
         radius: 25
    }
}




                                                                       1 （거 Quk水과 （갉너［ 577


===== PAGE 579 =====
Rectangular（丑ow Effect는 RGBA 컬러를 정의해 다음과 같은 Glow Effect를 제공한다．

      cO10r: #ffffff            color #55ff55       cO幻r: #5555ff
    이owRadi냐s: 20               이owRa（小us: 20      glowRadius: 20
       spread: 0                  spread: 0           5口read: 0
   cornerRadius: 25            cornerRadius: 25   cornerRadius: 25




心0pacityMask
Source 이미지에 八4askSource를 이용해 入4ask를 처리하기 위해 제공하는 Effect이다．

     Source 이미치                  maskSource          Effect 적용




import QtQuick 2. 0
import QtGraphicalEffects 1. 0


Item {
     width: 300
     height: 300


     Image {
          id: bug
          source: "images/bug. jpg"
          sourceSize: Q七．5뇨e (paren匕wid比r parent.height)
          smooth: true
          visible:     false
     }

     Image {
         id: mask
          source: "images/butterfly. png"
          sourceSize: Qt. size (parent.width, parent.height)
          smo(：比h : 七rue
          visible:     false



578 C니APTER 16_ Ct 0내ck과 QML


===== PAGE 580 =====
    }

    OpacityMask {
         anchors. f ill:   bug
         source: bug
         maskSource: mask
    }
}


0ThreshoidMask
Thresh아dMask는 Source 아이템에 MaskSource 아이템의 임계값을 적용하는 Effect이다．
thresh아d 프로퍼티의 값이 클수록 임계 값이 커진다．

    E沁urce 이미지               maskSource          Effect 적용




import QtQuick 2. 0
import QtGraphicalEffects 1. 0


Item {
    width: 300
    height: 300


    Image {
         id: background
         anchors, fill:    parent
         source: "images/ checker.png"
         smooth: true
         filiMode: Image.Tile
    }

    Image {
         id: bug
         source: "images/bug. jpg"
         sourceSize: Qt. size (parent.width, parent.height)
         smooth: true
         visible:    false
    }

    Image {                                                                  0



                                                              1 Qt 0미ck과 QML 579


===== PAGE 581 =====
         id: mask
         source: 'images/ f og.png"
         sourceSize: Qt. size (parent.width, parent.height)
         smooth: true
         visible: false
    }

    ThresholdNask {
         anchors. f ill: bug
         source: bug
         maskSource: mask
         threshold: 0. 4
         spread: 0. 2
    }



0 테pab冷
Flipable은 아이템의 앞면과 뒷면 사이에 "flipped" Effect를 사용할 수 있다. Flipable은 Rotation,
State, Transition 타입과 함께 사용할 수 있다. 이 타입의 front와 back 프로퍼티를 사용해 아이템이
보여지는 앞면과 뒷면에 이미지를 사용할 수 있다．

import QtQuick 2. 0


Flipable {
    id: flipable; width: 240; height: 240
    property bool flipped: false
    front: Image { source: "images/ front. png"; anchors.centerln: parent }
    back: Image { source: "iinages/back.png"; anchors.centerln: parent }

    transform: Rotation {
         id: rotation
         origin. x: flipable. width/ 2
         origin. y: flipable. height/ 2
         axis. x: 0; axis.y: 1; axis. z: 0
         angle: 0     /7 the default angle
     }

     states: State {
         name: "back"
         PropertyChanges { target: rotation; angle: 180 }
         when: flipable. flipped
     }

    七ransiti（그！
              lS: Transi七ic月1 {
         NumberAnimation {
                     target: rotation;
                     property: "angle"; duration: 1000 }
     }                                                                        O


580 CHAPTER 16_ Qt Quick과 QML


===== PAGE 582 =====
        MouseArea {
            anchors. fill:   parent
            onClicked: flipable. f lipped = !flipable. f lipped
        }


QML 어플리케이션이 실행되고 마우스 이벤트가 발생하면 Flipable 且ffect가 발생한다．



              유용한 QM[- 타입

이번 장에서는 QML에서 시그널과 시그널 Handler를 연결하기 위한 Conn吼ti아Is 타입, 프로퍼티를 다
른 변수에 할당하는 Binding, 타' ］머를 제공하는 Timer 타입，                         Qt   Quick            응용 어플리케 ' ］션에 " ]
Thread 사용을 활성화 하기 위한 WorkerScr如t 타입에 대해 알아보도록 하자．

타입                 설명
Connections       시그널과 시그널 Handler를 연결

텨nding             프로퍼티를 다른 변수에 할당하는 텨nding
Timer              타이머 기능을 제공
\A幻rkerSc마升        Ct Cu姚 응용 어플리케이션에서 Thread 사용을 활성화



I Connections
（兀nne毗ions은 QML 시그널에 연결하기 위해 키능을 제공한다. QML에서 시그널을 연결할 때 일반적
으로 "on<Signal>" 을 생성해 시그널을 연결하였다．

 MouseArea {
        onClicked: { foo (parameters) }
 }


이러한 방법은 동일한 시그널을 두 개 이상의 여러 Handler와 연결할 수 없다. 그리고 시그널이 발생하
는 " 1벤트 범위 밖에서 발생하는시그널에 대해                    升   ［andler를   연결할수 없다．          또한QML에         '   ] 정의되 " ] 않
은 JavaScript와 같은 Target에 연결할 수 없는 단점이 있다．

이러한 제약 사항을 해결하기 위해 Qt 鈿ick에서는 Connections를 제공하며 다음과 같이 사용할 수
있다．

 MouseArea {
        Connections {
            onClicked: foo (parameters)




MouseArea 영역 C아inecti아坮를 선언하는 방법보다 더 일반적인 사용방법으로 Connecti아鳩는 다른


                                                                                         ] （그to네ck과 CML 581


===== PAGE 583 =====
          오브젝트의 Child 오브젝트 또는 외부에서 Connecti아坮를 선언할 수 있다．

            ouseArea {
                        id: area
           }
           7/   .   .   .




           Connections {
                        七arge七： area
                        onClicked: foo(parameters)




          Conn吼ti아坮의 ignoreUnknownSignals 프로퍼 티가 발생하는 시그널 중 Unknown 시그널을 활성화
          하거나 비활성화할 수 있다. 만약 이 프로퍼티를 true로 설정하면 발생하는 Unknown 시그널에 대해 처
          리하지 않는다. target 프로젝트는 시그널을 보내는 오브젝트 또는 타입을 지정한다. 만약 target을 지
          정하지 않으면 디폴트로 Parent 오브젝트가 지정된다．


          自 텨nding
          Bindii乷은 직접적으로 QML에 의해 아직 초기화되지 않은 오브젝트의 프로퍼티를 Bind할 필요가 종종
          발생한다. 즉, C+＋어］ 의해 생성된 변수를 QML의 프로퍼티와 연결해야 하는 경우가 발생하는 데 이런
          경우 Binding을 사용해 연결이 가능하다．

          예를 들어 C++ 기반의 응용 어플리케이션의 특정 프로퍼티 "enterdText" 를 QML의 프로퍼티와 연결하
          여 QML의 프로퍼티도 업데이트되면 어플리케이션의 특정 프로퍼티가 업데이트되도록 하기 위해 다음과
          같이 Bindir乷을 선언해야 한다．

          TextEdit { d: myTextField; text: "Please type here. .. n }
          Binding { target: app; property: 'enteredText '; value: myTextField. text }



          예제의 소스 코드에서 보는 것과 같이 만약 QML의 TextEdit가 업데이트되면 C+＋과 업데이트된 프로
          퍼티도 업데이트 될 것이다. Binding의 property 프로퍼티는 업데이트할 프로피티를 지정한다. target
          프로퍼티는 업데이트할 오브젝트를 지정하며 , value는 Target 오브젝트와 프로퍼티를 지정할 값을 설정
   한다. Bindh培과 관련해 추후 좀더 자세히 다룰 것이다．


          孕 기mer
    Timer는 어플리케이션 특정 Trigger를 처리하기 위해 한번만 실행되도록 하기 위한 타이머를 제공한다．
다음 예제 코드는 500m111iseconds마다 날짜와 시간을 업데이트하며 현재 시간을 얻어오기 위해
 JavaScript의 Date를 사용하였다．

!import
                            QtQuick 2. 0


          Item {
                    Timer {


582 CHAPTER 16m Ct Quick과 CML


===== PAGE 584 =====
         interval: 500; running: true; repeat: true
         onTriggered: time.text = Date () .toString()
     }
     Text { Id: time }




Timer 타입은 애니메이션 타이머로 동작하도록 동기화되어 있다. 일반적으로 애니메이션은 60fps로 설정
된 이후로 타이머가 동작하며 가장 좋은 반복 타임＝!l6ms가 가장 적합하다. 만약 Timer가 동작하고 있는
상황에서 interval 프로퍼티를 변경한다면 예제 코 드에서 보는 것과 같이 interval을 수정하면 된다．

예를들어 Timer의 intervalol 1000ms로 설정되어 반복되도록 변경되기 원한다면 초": ］정한 500ms
가 경과되고 난 다음 1000ms로 변경될 것이다. interval 프로퍼티는 반복되는 타이머의 시간을
millisecond로 "］정한다． repeat프로퍼티는b아丑값으로 ' 1정하며true를지정가면지정한 "nterval
만큼 계속 반복된다. 반대로 false를 지정하면 한번만 실행되고 반복되지 않는다．

만약 Timer의 running 프로퍼티를 true로 지정枓면 Timer의 start( ) 함수를 호출하지 않더라도 타이
머가 자동으로 시작된다. running 프로퍼티는 디                  트로 false로 설정되어 있다．

Timer의 onTriggered( ) 함수는 Timer!} 발생했을 때 호출가는 함수"］다． restart( ) 함수는 Time"가
                                     '1 다' ] 동작하도록변경할수 있다． start() 함
동작되 ' ] 않거나중단된상태에 ' 1 restart() 함수를호출레
수는 Timer가 동작하는 기능을 제공하고 stop( ) 함수는 Timer를 멈춘다．


0WorkerScript
WorkerScript는 Qt Quick 기반 어플리케이션에서 Thread를 사용하기 위해 제공되는 타입이며 새로
운 Thread를 동작시키기 위해 사용한다. send八4essage( ) 함수와 onMessage( ) 함수를 사용해 부모
Thread와 새로 생성한 Thread간의 메시지를 교환할 수 있다．

import QtQuick 2. 0


Rectangle {
    width: 300; height: 300
    Tex七 { id: myTex七； 七e>＜七： 'Click anywhere' }


     WorkerScript {
         Id: myWorker
         source: "scrip七．그5,,
         onNessage: myText. text = messageDbject.reply
     }

     MouseArea {
         anchors. fill: parent
         onClicked: myworker. sendMessage ({ 'x ' : mouse. x, 'y ' : mouse. y })
     }
 }


                                                                             ] （코 0네ck과 QML 583


===== PAGE 585 =====
JavaScript 파일인 script.js에는 새로운 Thread로 동작할 함수가 정의되어 있으며 script.js 파일은
다음과 같은 함수가 구현되어 있다．

 WorkerScript.onMessage = function(message)
 {
     WorkerScript. senclNessage ({ 'reply ' : 'Mouse is at 1
                                     + message. x +        message. y })




            Canvas
Car玎as는 라인, 곡선, 단순한 도형부터 복잡한 도형 그리고 그래픽 이미지를 표시할 수 있는 기능을 제
공하는 아이템이다. 뿐만 아니라 텍스트, 컬러, Shadow, Gradient, 패턴 그리고 Low 레벨의 픽셀을 조
작할 수 있다. 그리고 Canvas어］ 의해 표시된 그래픽을 이미지로 저장할 수 있는 기능을 제공한다．

width와 height 프로퍼티를 사용해 Canvas의 Drawing 영역을 설정해야 한다. 예를 들어 width가
100이고 height가 200인 Canvas 아이템을 정의하기 위해서 다음과 같이 예제 코드를 작성한다．

 import QtQuick 2. 0


 Canvas {
     Id: mycanvas
     width: 100
     height: 200
 }


0Rendering Target 방식
Canvas 아이템은 Rendering Target으로 Canvas.Image와 Canvas.Framebuffer아）昶Ct의 Target
방식을 지원한다. Canvas.Image Rendering 타깃 방식은 Qlmage 오브젝트이며, Rendering 과정은
Background Thread로 동작하도록 지원한다. Background Thread로 동작하기 때문에 복잡하거나 긴
시간을 요구하는 Painting 작업을 수행하더라도 UI가 Blocking 되지 않고 수행할 수 있다．

Canvas.FramebufferObject Rendering 타깃 방식은 하드웨어 그래픽 가속기 기반의 OpenGL에 최
적화되어 있기 때문에 시스템의 메모리상에서 동작하는 것보다 더 빠른 Rendering 결과를 얻을 수 있
다. Canvas의 Rendering Target은 디폴트로 Canvas.Image 방식으로 지정되어 있다．

Car싸as는 HTML5의 Canvas와 비슷하며 라인, 곡선, Gradient, 단순한 도형부터 복잡한 도형 그리고
그래픽 이미지를 표시할 수 있도록 다음과 같은 아이템을 제공한다．




584 CHAPTER 16_ Qt Quick과 QML


===== PAGE 586 =====
아이템                       설명
Canvas                    HTML5와 비슷하며 2D Canvas를 제공한다．
Context2D                 Canvas 아이템상에 2D 도형을 저공한다．
CanvasGradient            Canvas 아이템상에 （計a데ent를 제공한다．
CanvasPixelArray          Canvas를 사용해 픽셀 Array를 지정할 수 있는 기능을 제공한다．
CanvasimageData           Canvas를 사용해 이미지 데이터를 지정할 수 있다．
Tex棚etrics                Canvas를 사용해 텍스트와 폰트 데이터를 제공한다．



1Context2D
Context2D 오브젝트는 Canvas 아이템의 get（了" ntext( ) 메소드에 의개 생성할 수 있다． OI 함수는
Canvas 영역을 2D Viewport 영역과 연결해 드루잉이 가능하다．

 Canvas {
    Id: canvas
    width: 300
        height: 150

        （꾜Wain七 : {
             var ctx = canvas.getContext ( 12d1 ),
             II. . .
         }



con扼砒는 Context2D API를 이용해 Canvas 영역에 Drawing한 결과를 렌더링할 수 있으며 (0,0) 좌
표부터 지정한 佃idth, height) 좌표까지 Rendering이 가능하다．

(0,0)



                                            Canvas I'이酎仕
                                            (Default = 150 pixels)



                                            (300,15까
                       Canvas wd出
                       (De相U仕 = 300 pb姆빠
（그림） Canvas의 좌표



Cor此ext2D는 Canvas 영역에 이미지를 Rende가ing 하기 위해 drawlmage( ) 함수를 제공하며 이미지
로부터 픽셀 데이터를 얻어오기 위해 createlmageData( ) 함수를 제공한다. 그리고 부채꼴 모양의 /\rc
와 같은 도형을 그리기 위해 arc( ）와 arcTo( ) 메소드를 제공한다．




                                                                     ] （가 Ct기ck과 C）卜月L 585


===== PAGE 587 =====
    object Context2D: :arc (real x, real y, real radius,
                                 real startAngle, real endAngle, bool anticlockwise)




    object Context2D: :arcTo(real xl, real yl, real x2, real y2, real radius)




                                           『""亡>1'"""'
      (xl, yl) =(x2. y2)
                           \\
                                             (xl. vi)




Cor此昨比D는 API를 이용해 그래픽 요소를 바로 렌더링하지 않고 beginPath( ), cbOs可뇽th( ) 또는
stroke( ) 메소드를 사용해 그래픽 요소를 완료한 후 일괄적으로 렌더링할 수 있는 기능을 제공한다．




                                                                    q口7
    ctx. strokeStyle = Qt.rgba (0, 0, 0, 1) ;
    ctx. lineWidth = 1;
    ctx. beginPath( );
    C七x.moveTo(20, 0) ; // 시작 point
    ctx. bezierCurveTo(- 10, 90, 210, 90, 180, 0) ;
    c七x 's七roke ( ) ;



Path를 사용해 그래픽을 일괄 렌더링을 사용하는 이유는 상황에 따라 UI상에 렌더링되는 과정이 화면상
어］ 보여 지 거나 UI 화면이 깜박이는 현상을 방지할 수 있다．

C아此ext2D는 Context어］ 그려진 결과를 rotate( ) 메소드를 사용해 회전을 시킬 수 있는 기능을 제공
한다．
r
    ctx. rotate (Math.PI/ 2) ;
                                                                        (0, 0)
           (0, 0)




그리고 Context2D API 중 scale( ) 메소드를 사용하면 Canvas의 각 그래픽 요소의 Scale을 조정할 수
있다．


586 CHAPTER 16_ Qt Quick과 QML


===== PAGE 588 =====
ctx. scale (2.0, 0. 5) ;




     미                                       H
                           Scale (2, O. 5)




孕 CanvasGra데ent
CanvasGradient는 Canvas 영역에 Gradien               을 제공한다. 0.0에서 it. 0까지 0ffset을 지정할 수
있으며 사용할 Gradi아此의 （兀珀r를 지정할 수

var gradient = ctx. createLinearGradient (0, 0, 100, 100) ;
gradient.addColorStop(0.3, Qt.rgba (1, 0, 0, 1) );
gradient.addColorStop(0.7,   'rgba(0, 255, 255, 1' ) ;



咎 CanvasP以아낚ay와 CanvasimageDa怡
CanvasPixelArray 오브젝트는 이미지 데이터의 각 픽셀에 대응하는 색상에 접근할 수 있도록 인덱스를
제공한다. CanvaslmageData 오브젝트는 이미지의 픽셀 데이터의 오브젝트를 지정하며 이미지로부터
읽어온 픽셀 데이터 오브젝트의 리턴 값으로 처리할 수 있다．

예를 들어 Context2D의 createlmageData( ) 메소드를 이용해 특정 이미지로부터 읽어온 데이터를
CanvaslmageData 오브젝트어］ 포인터를 전달한다. 프로퍼티로 height와 \qidth를 지정할 수 있다．
height와 width는 이미지로부터 읽어온 픽셀 데이터의 길이를 지정하면 된다．

CanvasImageData createImageData (CanvasImageData imageData)
CanvaslmageData createlmageData (Cr1 imageurl)
CanvaslmageData createlmageData (real sw, real sh)



0Te났Metrics
TextMetric " 오브젝트는Context2D의 measureText() 메소드에서 인' ｝로 '｝용할Metrics를설정하
기 위한 기능을 제공한다. TextMetrics는 단지 帥dth 프로퍼티만 제공하며 READ 모드로만 사용한다．

variant Context2D: :measureText (text)




    1.13 Integrating QML과 C++
Qt 如ick은 개발자에게 현대적인 GUI 인터페이스를 쉽게 설계하고 어플리케히션에 적용하기 위한 목
적으로 제공되는 API이다. 이러한 GUI 인터페이人를 설계하는데 있어 Qt 伽ick은 QML을 사용한다．
기존의 邸Vidget, QPainter 등을 사용해 UI를 크계했던 것과 마찬가지로 QML은 UI 아이템의 행동을
정의하고 제어할 수 있다．


                                                                     ] （코 O비ck과 QML 587


===== PAGE 589 =====
QML은 declarative 언어이며 （절차 언어） 자바스크립트가 확장된 스타일의 문법구조를 가지고 있다．
QML은 JavaScript와 같은 절차 언어를 해석하는 Declarative 모듈이 있으며 C+＋을 사용해1 소스 코드
를 작성하면 컴파일러가 실행 바이너리를 생성하는 것과 같이 Declarative 모듈은 QML로 작성한 코드
를 실행할 수 있는 어플리케이션으로 변환하는 작업을 한다. 또한 QML 어플리케이션 내에서 C++ API
를 사용할 수 있다．

Qt Quick과 QML을 사용해 응용 어플리케이션을 구현하는 경우 Qt Quick과 QML로 완벽한 응용 어플
리케이션을 구현할 수 없다. 예를 들어 네트워크 트래픽 사용량을 확인하기 위한 응용 어플리케이션을 구
현함에 있어 시스템 레벨의 네트워크 트래픽을 제어하기 위해I Native 라이브러리 사용이 필요하다. 따라
서 사용자에게 제공하는 GUI 단은 Qt Quick을 사용해 녜트워크 사용량을 그래프로 표시하고 네트워크
트래픽을 측정하는 실제 구현 API는 전통적인 Qt API 또는 시스템 레벨의 API를 사용해 구현하는 것이
가장 바람직하다.

따라서 Qt Quick으로는 GI끄를 구현하고 실제 기능이 동작하는 모듈은 전통적 인 Qt API를 사용해 구현
할 수 있다. 이러한 방식은 HTML5를 이용해 응용 어플리케이션의 구조와 흡사하다. 즉, 사용자에게 제
공하는 GI끄는 HTML5를 사용하고 실제 동작을 담당하는 모듈은 Native API를 사용해 HTML5 기반의
응용 어플리케이션을 구현한다．


                                  Of A［갸引ication

                                  Ot Quick (GUI)
                                                                               -J
                                                                               \
                      Native Qt C++ API (Application fuctiori)
                                                                          -J
（그림） at o미ck과 Native （가 C++ API


S 프로퍼티를 사용한 0+＋과 QML간 데이터 전달
C+＋로부터 QML에 톄이터를 전달하기 위한 방법으로 프로퍼티, 메소드 파라미터 , 메소드 리턴 값 또는
시그널 파라미터 값을 사용한다. 이러한 방법은 QML 엔진에서 지원한다. 기본적으로 Qt C++ 데이터
타입을 QML 타입으로 변환하기 위한 과정은 자동으로 지원한다．

（코 타입                            QML 기본 타입                at 타입                     QML 기본 타입
bool                             bool                     QTime, QDateTime          time
unsigned int , i nt              mnt                      op이nt, OP이ntF             point
double                           double                   OSize, OSizeF             引ze
 float, qreal                    real                     ORect. ORectF             rect
oString                          string                   QMatrix4x4                mat rix4x4
QUrl                             real                     QQuaternion               quaternion
QC이or                            color                    QVector2D, QVector3D,     vector2d,
 QFont                           f。nt                     QVector4D                 vector3d, vector4d

 QDate                           date




588 CHAPTER 16_ （그to미ck과 OML


===== PAGE 590 =====
프로퍼티를 사용해 QML과 Qt C++ 간의 데이터 전달을 위해 Q_ PROPERTY( ) 매크로를 사용할 수 있
다. Q_PROPERTY( ) 매크로는 QObject 클래스로부터 파생된 다른 클래스에서 사용할 수 있다．
QOb昶ct로부터 상속받은 모든 프로퍼티는 QML에서 접근이 가능하다．

예를들어 author프로퍼티를사용해 八4essage클래스어］ 접근할수 있도록Q_PROPERTY() 매크로를
사용해야 한다．

class Message : public QObject
{
     Q OBJECT
     QPROPERTY (QString author READ author WRITE setAuthor
                                                    NOTIFY authorChanged)
public:
     void setAuthor (const QString &a) {
         if (a != U느au七hor) {
             mauthor = a;
                emit authorChanged() ;
            }
     }
     QString author () const {
        return m author;
     }
private:
     QString rn_author;
};


예제 소스 코드에서 보는 것과 같이 八4essage 클래스의 인스턴스를 생성해 QML과 프로퍼티를 통한 데
이터 전달을 위해 Context 프로퍼티를 다음과 같이 지정한다．

mnt main(int argc, char *argv[ ])
{
         QCoreApplication app(argc, argv) ;

         QOmlEngine engine;
         Message msg;
         engine.rootContext ( )->setContextProperty ( "rnsg'1 , &msg) ;
         oomlComponent component (&engmne, Qurl: : fromLocalFile ( 1'Myltern.qml") );
         component.create() ;


         return app.exec () ;
}




                                                                               ] Qt 0네ck과 QML 589


===== PAGE 591 =====
  다음은 QML 예제 코드이다．

 fimpor七
                     Q七Quick 2. 0


           Te)＜七 {
                 width: 100; height: 100
                 text: msg. author   II invokes Message: :author ( ) to get this value


                 Component. onCompleted: {
                    msg. author = "Jonah"    7/ invokes Message: :setAuthor )
                 }



I               0+＋과 QML간 메소드 호출
QObject 클래스로부터 상속받는 클래스는 QML 코드상에서 메소드를 호출할 수 있다. 또한 C+＋로 작
성된 코드는 QML상에서 작성된 메소드 호출이 가능하다. 다음 예제 소스 코드에서 보는 것과 같이
MessageBoard 클래스는 postMessage( ) 메소드를 QML상에서 호출하기 위해1QINVOKABLE 매크
로를 사용한다. 또한 QML에서 시그널을 통해 c++ 슬롯함수를 호출할 수 있다．

           class MessageBoard : public QObject {
               Q OBJECT
           public:
                 QINVOKABLE bool postMessage (const QString &msg) {
                     qDebug() << "Called the C++ method with" << msg;
                     return true;
                 }
           public slots:
                void refresh() {
                     qDebug() << "Called the C++ slot ";
                 }
           };


MessageBoard 클래스의 인스턴스는 QML 간의 데이터 전달을 위해 두 가지 방법을 제공한다. 첫 번째
방법은 QQmlEngine을 사용하는 방법이며, 두 번째 방식은 QQuickView 클래스를 사용하는 방식이다．

    自QmlEngine을 사용하는 방식

  QQmlEngine engine;
  QQmlComponent component (&engine, QUrl: : fromLocalFile ( "Myltem.qml") );
 QObject *object = component.create ( );


 delete object;




590 CHAPTER 16_ 01 Quick과 CML


===== PAGE 592 =====
 QQui口恐碌鈿匿 사용하는 방식
QQuickView view;
view. setSource (QUr1: : fromLocalFile ( "Myltem.qml") );
view. show() ;
QObject *object = view.rootObject () ;



S C+＋에서 QML 오브젝트 멤버의 접근
QML 오브젝트상에 정의된 프로퍼티는 c+＋에서 접근하기 위해 다음과 같은 방법을 사용할 수 있다．

II Myltem.qml
import QtQuick 2. 0

Item {
    property mnt someNuxnber: 100




예제 코드에서 보는 것과 같이 QML에 정의된 someNumber 멤버를 c+＋에서 접근하기 위해서 QQm1
Property 또는 QObject: : setProperty(）와 QObject::property( ) 함수를 사용할 수 있다．

QQmlEngine engine;
QQmlComponent component (&engine, "Myltem.qml ") ;
QObjec七 出objec七 = componen七．crea七e ( );


qDebug() << "Property value: " << QQmlProperty: :read(object,
                                                     r' someNu山er " ) .tolnt () ;
QQmlProperty: :write (object, "someNumber ", 5000) ;


qDebug() << "Property value: " << object->property ( "someNumber " ) .tolnt () ;
object->setProperty ( "someNumber ", 100) ;



S QML 메소드의 호출
모든 QML 메소드는 c+＋에서 제공하는 帥4eta0可吼t::jnvokeM毗hod( ) 함수를 사용해 호출할 수 있
다. QML에서 제공하는 메소드의 파라미터와 리턴값은 항상 c+＋에서 제공하는 QVariant 타입 값으로
전달된다.

ty工七em. qml
import QtQuick 2. 0
Item {
    function myomlrunction(msg) {
        console. log( "Got message: ", msg)
        re七｝그rn "some re七urn val끄e"
    }




                                                                            j （거 Q네比과 QML 591


===== PAGE 593 =====
ma끄1.cpp

QQmlEngine engine;
QQmlComponent component ( &engine, "Myltem. 꾸ll") ;
'QObj ect 士objec七 = componen七．crea七e ( ) ;


QVariant returnedValue;
QVariant rnsg = "Hello from C++";
QMetaObject: : invokeMethod(object, "myQmlFunction",
            QRETURNARG ( QVariant, returnedValue) ,
            Q   RG(QVariant, msg) );


qDebug() << "QML function returned: " << returnedValue.toString() ;
delete object;



0QML 시그널과 연결
QML에서 제공하는 모든 시그널은 c+＋의 슬롯함수와 연결할 수 있다. Qt C++ 기반에서 사용했던 전통
적인 방식과 동일하다. QML 시그널과 연결하기 위해 QObject 클래스에서 제공하는 connect( ) 함수를
사용해 QML에서 발생한 시그널을 c++ 기반의 슬롯함수와 연결할 수 있다．

 My工tern. gin]. 小n=

import QtQuick 2. 0


Item {
      id:   j土em
      wid七h: 100; heigh七： 100


      signal qmlSignal(string msg)


      MouseArea {
            anchors. fill:   parent
            onClicked: item.qmlSignal( "Hello from Q卜L")
      }

 maln.cpp
class MyClass : public QObject
{
   0 OBJECT
public slots:
      void cppSlot (const QString &msg) {
            qDebug() << "Called the C++ slot with message: " << msg;
      }
 };

irit main(int argc, char *argv[ ]) {
      QGuiApplication app(argc, arg叫;
                                                                       0


592 CHAPTER 16_ 01 QuickZ QML


===== PAGE 594 =====
        QQuickView view (QUr1: : fromLocalFile ( 1 Myltem.叩ll " ) );
        Q0bjec七 出i七em = vies寸．ro(＞七0bjec七（) ;


        MyClass myClass;
        Q0bject: :COflfleC七（j土em, SIGNAL（甲｝lSignal (QS七rin引 ) r
                            &myClass, SL0T(cppSlot (QString) ));

        view. show ( ) ;
        return app. exec () ;




   tm Mu川med治
Qt에서 제공하는 Multimedia 모듈은 C++ 기반의 API뿐만 아니라 QML에서도 활용할 수 있는 API를
제공한다. QML에서 제공하는 Multimedia 모듈을 사용하기 위해서는 다음과 같이 import 해야 한다．

 import QtMultimedia 5. 0


QML에서 제공하는 Mul恤.edia 모듈은 Video, Audio, Camera, Radio를 QML 타입으로 제공한다．

QML타입                           설명
Video                           Video 영상을 보여주기 위한 타입
Aud山                            Audio를 재생하기 위한 타입
MediaPlayer                     멀티 미디어 플레이어를 제공하71 위한 타입
Camera                          카메라 프레임에 접근， 사진과 동영상을 얻기 위한 타입
CameraCaplure                   카메라 이미지를 Ca口仙re하71 위한 인터페이스를 제공
CameraExposure                  카메라 Ex口osure와 관련된 설정을 위한 타입
CameraFlash                     카메라 디ash 설정과 관련된 인터페이스를 제공
CameraFocus                     카메라 포커스를 제공하기 위한 인터페이스 제공
Camer톄mageF가ocessing            카메라 Ca口山re 설정과 관련된 인터페이스 제공
CameraRecorder                  카메라 Recording을 제어하기 위한 타입
Pad山                            QML 어플리케이션에서 라디오 기능을 접근하기 위한 타입
RadioDa怡                        QML 어플리케이션으로부터 RDS 데이터를 접근
Torch                           단순한 터치 기능을 제어하71 위한 타입
VideoOutput                     카메라 또는 비디오의 Rendering과 관련된 타입 제공
SoundEftect                     QML에서 플레이 El伯Ct를 제공하기 위한 방법으로 사운드
                                타伯아를 제공하71 위한 타입



S Video
Video 타입은 비디오 영상을 출력하기 위한 인터페이스를 제공하기 위한 목적으로 八4ediaPlayer와
VideoO岫)Ut 타입을 함께 사용하며 비디오 영상의 Play 기능을 제공한다．




                                                                       l （거 C네ck과 CML 593


===== PAGE 595 =====
import QtQuick 2. 0
import QtMultimedia 5. 0


Video {
    id: video; width : 800;         height : 600
    source: "video. avi"


    MouseArea {
          anchors. fill:   parent
          onClicked: {
               video.play ()
          }
    }

    focus : 七rue
    Keys. onSpacePressed:
    video.playbackState == MediaPlayer . PlayingState
                                                   ? video.pause () : video.play ()
    Keys.onLeftPressed: video. seek (video.position - 5000)
    Keys.onRightPressed: video. seek (video.position + 5000)
}


또한 Video 타입은 일시 정지하기 위한 메소드로 pause( ）를 제공하며, 영상을 재생하기 위해서는 히ay()
메소드를 사용하면 된다．
비디오 영상의 특정 위치로 이동하기 위해 seek佃作set）을 사용할 수 있으며 정지를 위하 stop( ) 메소드를
제공한다．


I Audio
知dio 타입은 \UAV와 같은 멀티미디어 데이터를 재생하기 위한 목적으로 play( ) 메소드와 특정 위치로
이동하기 위해서 seek(offset) 메소드를 제공한다．

또한 재생되고 있는 멀티미디어 데이터를 일시 정지 또는 정지하기 위해서 pause( ) 메소드와 stop( ) 함
수를 제공한다．

import QtQuick 2. 0
import QtMultimedia 5. 0


Text {
    text:     "Click Me! ";
    font. pointSize: 24;
    width: 150; height: 50;


    Audio {
          id: playMusic
          source: "music .wav "
     }                                                                                0


594 CHAPTER 16_ Ot O네ck과 아／[


===== PAGE 596 =====
     MouseArea {
             id: playArea
             anchors, fill:     parent
             onPressed:       { playMusic.play () }
     }



eCamera
Camera 타입은 카메라로부티 영상을 이미지로 Capture하거나 비디오 데이터로부터 영상을 Capture
할 수 있는 기능을 제공한다. Camera 타입은 특정 프레임의 영상을 얻어오기 위해 \TideoO的)ut과 함
꼐 사용한다．

import QtQuick 2. 0
import QtMultimedia 5. 0

Item {
     width: 640; height: 360


     Camera {
        id: camera
             imageProcessing . whiteBalanceMode:
                                        CameralmageProcessing .WhiteBalanceFlash


             exposure {
                 exr均sureCompe粥毗珀n: -1. 0
                 exposureMode: Camera. ExposurePortrait
              }

              flash.mode: Camera. Flash之edEyeReduction


              imageCapture {
                  onlmageCaptured: {
                      photoPreview. source = preview
                   }
              }
         }

         VideoOu七pu七 {
              source: camera
              anchors. fill: parent
              focus : visible
         }

         Image { id: photoPreview }
 }




                                                                             ] （그to네ck과 QML 595


===== PAGE 597 =====
露 Radio
Radio 타입은 라디오 시그널과 관련한 정보를 얻을 수 있으며 라디오 Tune을 조정할 수 있다. 라디오를
시작하기 위해 start( ) 메소드를 사용하며 라디오를 정지하기 위해 stop( ) 메소드를 사용한다. 또한
Tune을 조정하기 위해 tuneDown( ）과 tuneUp( ) 메소드를 사용할 수 있다．

imp（그r七 QtQuick 2. 0
import QtMultimedia 5. 0


Re（北angle {
      width: 320; height: 480


      Radio {
          id: radio
          band: Radio.FM
      }

      MouseArea {
          X: 0; y: 0
          height: parent.height; width: parent.width / 2
          onClicked: radio. scanDown()
      }

      MouseArea {
          x: parent.width I 2; y: 0
          height: parent.height
          wid七h: paren七．wid七h / 2
          onClicked: radio. scanUp()




라디오 주파수 Bandwidth를 조정하기 위해 band 프로퍼티를 사용할 수 있으며 설정 값으로 다음과 같
은 enumeration을 제공한다．

Bandwidth       설명
AM              520"怜］0kHz 주파수 대역을 사용， 또한 ]610' 1710kHz까지 확장 가능
FM              87.5에서 ]08.0MHz, 일본의 경우 76' 90MHz
SW              1.711에서 30.0MHz, 15개로 band로 분할됨
LW              148.5에A1 283.5kHz, 9kHz (Europe, Africa, Asia)
FM2             정의되지 않은 주파수 범위




596 CHAPTER 16 （그to미ck과 （가너［


===== PAGE 598 =====
    CHAPTER




Qt 어플리케이션 배포


===== PAGE 599 =====
QI 5 ProgrammJng




          1 // 다양한 플랫폼에서
               Qt 어플리케이션 배포
          （거는 리눅스, 윈도우, Mac 0S, 안드로0匹 등과 같은 다양한 플랫폼상에 아로 개발한 어플리케이션
          을 배포하기 위한 방법에 대해 살펴보도록 하자．




개발한 Qt 응용 어플리케이션을 사용자에게 배포하기 위해 Static Linking 방식과 Shared 라이브러리
방식을 사용할 수 있다. Static Linking 방식은 컴파일 시 필요한 모든 라이브러리를 통합하는 방식으로
하나의 실행 파일로 실행된다. 그렇끼 때문어］ 배포하는데 라이브러리 의존성을 고려하지 않고 배포할 수
있는 장점을 가지고 있다. 하지만 Static Linking 방식은 응용 어플리케이션 크기가 매우 크기 때문어］
응용 어플리케이션 업그레이드 시 시간이 많이 소요된다．

예를 들어 인터넷 네트워크를 통해 사용자에게 업그레이드 버전을 제공하기 위해서 업그레이드된 일부만
다운로드 할 수 없다. 그러므로 응용 어플리케이션 업그레이드 시 많은 시간이 소요되는 단점이 있다．

Shared 라이브러리 방식은 응용 어플리케이션 실행 파일과 라이브러리가 분리된 형태이므로 크기가 작
아 사용자에게 업그레이드 시 용이하다. 단점으로 공유 라이브러리 의존성을 체크해야 한다. 만약 어플리
케이션을 실행하는 시스템에 어플리케이션이 사용하는 라이브러리가 없다면 실행이 되지 않는다. 따라서
라이브러리 의존성을 확인해야 한다．

Uni따 Linux, Windows, Mac OS X와 같은 여러 플랫폼을 지원한다. 이번 단원에서는 다음과 같은
플랫폼에서 Qt 응용 어플리케이션을 배포하는 방법에 대해 살펴보도록 하자．




598 CHAPTER 17中 Of 어플리케이션 배포


===== PAGE 600 =====
     ].] Un以와 匕flux

Un奴와 Linux 플랫폼에서 Qt 응용 어플리케이션을 배포하는 것은 조금 복잡하다. 예를 들어 Linux 플
랫폼은 Ubuntu, Fedora, Suse 등 다양한 배푹판이 존재하기 때문이다． 따라서 각 플랫폼마다 라이브
러리 의존성을 파악해야 하끼 때문어］ 개발한 Qt 응용 어플리케이션을 사용자에게 배포하는 것은 어려운
문제 중 하나이다．

Qt 응용 어플리케이션을 배포하는 방법은 일전에 설명한 것과 같이 Static Linking 방식과 Shared 라
이브러리 방식이 존재한다. Linux 또는 Unix                     ］서 Static Linking 방식을 이용해 어플리케이션
을 배포하기 위해서는 Qt API 빌드 시 configu巾 옵션에 " static" 옵션을 다음과 같이 추가해야 한다．

cd /path/to/Qt
./configure -static -prefix /path/to/Qt <other parameters>
make sub-src


그리고 Shared 라이브러리 방식으로 "11포차기 위 ": ］는 사용"｝의 플랫폼에 Qt 응용 어플리케 ' ］션 " ] 필
요로 하는 라이브러리가 존재해야 한다. Linux 또는 Un奴 플랫폼에서 라이브러리 관계를 확인하기 위해
ldd를 제공한다. ldd를 사용하면 어플리케이션이 사용하는 라이브러리 의존성을 확인할 수 있다．

ldd ./application


그리고 Linux와 Un奴는 RPM 방식을 사용하여 개발한 응용 어플리케이션을 사용자에게 배포할 수 있
다. RPM은 Red Hat Package 八/Ianager의 약자이며 Redhat에서 응용 어플리케이션 패키지를 관리하
는 목적으로 개발되었다. 현재 많은 Linux 및 Un奴에서 RPM을 사용하고 있으며 RPM 패키지를 사용
해 각종 소프트웨어 설치와 업그레이드를 편리하게 할 수 있다．

rpm 日tJvh ＜응용어플리케이션 패키지이름＞


또한 RPM은 플랫폼어］ 설치된 RPM 패키지에 대해 데이터베이스화 하므로 패키지 이름을 사용해 어플리
케이션을 업그레이드하거나 삭제가 쉽다. 예를 들어 설치된 RPM 패키지를 삭제하기 위해서 옵션으로
"-e" 옵션을 추가하면 된다. 그리고 설치된 RPM 패키지 목록을 rpm 옵션을 사용해 설치된 RPM 패키
지를 질의할 수 있다．

rpm -qa 1 more


RPM 패키지 관리자는 이외에도 이미 설치된 RPM을 업그레이드 하거나 의존성 등 다양한 옵션을 사용
할 수 있다．
Qt응용 어플리케 "］션을Shared 라" 1브러리 방섞으로 "TI포하다 보면 라"］브러리가 위치한 디렉토리에 대
한 접근이 필요하다. 만약 플랫폼에 라이브러리가 위치한 디렉토리를 찾지 못한다면 어플리케이션 내에서
QApplication 클래스의 addLibraryPath( ) 함수를 사용해 라이브러리 디렉토리를 지정할 수 있다．

qApp->addLibraryPath( " /some/ other/path'1 );


                                                       ] 다양한 플랫폼에서 아어플리케0썬 배포 599


===== PAGE 601 =====
            Windows
 0Static Linking
 Windows 플랫폼은 Qt 응용 어플리케이션을 배포하기 위한 방법으로 이전과 같이 Qt API를 Static 방
식으로, Qt 공식 홈페이지에서 \windows 버전을 다운로드 받은 다음 configure 옵션에 " static" 을 다
음과 같이 추가한 후 컴파일하뺘 한다．

 cd C: \path\ to\Qt
 configure -static <any other options you need>



 心 Shared 라이브러리
Shared 라이브러리 방식은 Qt가 설치된 하위 디렉토리에 존재하는 라이브러리 디렉토리와 Include 파
일이 위치한 디렉토리를 참조하도록 PATH를 지정해야 한다. 또한 사용자의 ＼航ndows 플랫폼에 Qt 라
이브러리가 없는 경우 Install Wizard와 같은 설치 프로그램에 응용 어플리케이션 라이브러리를 함꼐
배포해야 한다．

Windows 플랫폼은 Qt API를 컴파일하기 위해서 nmake와 n血培w32-make 중 하나를 사용할 수 있
다. Win如ws 플랫폼은 \uisual Studio 버전에 따라 다음과 같이 DLL의 명칭이 달라진다．

                    VC++ 8.0 (2005)   VC++ 9.0(2008)   VC++ 10.0 (2010)
  The C run-time     msvcr80.dll       msvcr90.dll      msvcr100.dll
 The C++ run-time    msvcp80.dll       msvcp90.dU       msvcp100.dll


0 라이브러리 의존성 체크
Windows 플랫폼은 Qt 응용 어플리케이션이 참조하는 라이브러리 의존성을 확인하기 위한 방법으로
Dependency Walker 툴을 제공한다. 이 툴은 32비트 또는 64비트 플랫폼을 모두 지원하며 트리 형태
로 참조하는 라이브러리 관계를 GUI 툴을 통해 확인할 수 있는 편리한 기눙을 제공한다．

Depend이icy Walker 툴은 \Windows 95, 98, Me, NT, 2000, XP, 2003, Vista, 7, 8 등 다양한 버전
어］ 사용할 수 있으며 의존관계의 라이브러리어］ 대한 상세한 정보도 참조할 수 있도록 디자인되어 있다．
이 툴은 www. dependencywalker. corn 사이트에서 다운로드 받을 수 있다. 사용 방법은 File 메뉴에서
의존관계를 확인할 Qt 응용 어플리케이션 실행 파일을 선택하면 된다．




600 CHAPTER 17_ O1 어플리케0k크 배포


===== PAGE 602 =====
叱 004陪ederwy Walker    lanimatror]                                                                                                  回   回    乂

 보 唯      떤8)80므n     야do首 pro州e       Window       He巾                                                                                  m 戶 니
］才 日      戶 岵       C丸 區     쿠 臣1 틔 JJ        늘0     .0 也 目 ［끄         k?
 日    口   AN))月All에EXE                               P1    0rdinal 八        Hot            FUndt心n                                               4
           쏘1 QT5QUICKD OLL                          回  5/4         2601000)041 갸帥갸n吼甘拉雹'f_k駐z                                                  洹三
           호） QT5QMLD DLL                            L그 N/A         294 心01207 _Crt015目op미Ta
                QTSOUIDDLL                      二    t그 N/A         311 (000137) 工it s etCire改Co나no
                                                     匠그 N/A         335 (000144) _0다奸1100
           !)
          . ) QTSC0060 DLL
                                                     區그 S/A         340 田0015 C) _CoxFrarrreH,크n出e心
      므   口 回呻L
                                                     匠그 S/A         3811000170) _d比00011                                                           !
          日    보 旺RNEL끄DLL             !
                                                     匠그 WA          3891000185 1 _getrnalflarg드                                                  1 '
                 艮引 NTDLLDLL                         1  小m U 小山a m m月小艸m小m!m m1m          1                                                 卜
      室   口 KERNEL32 DLL
              口 40卜MS川IN-CORE-町(SLOOP)               E     On비fld 八     네ft          F810tiOn                                      1
              口 NTDLLDLL                             口       1 (080001)   1 (000001) ?l0?1_SmnWait(O100@detarIiCo叱Unoo8y回(OQAE回0HA!J
                                                     口       2)010002)    2 田00002) ' (0及SI出n니／키t回106口也dote小四CO,]C냐01000四的QAP心Pt
          므 口 KERNOLEASOILL
                                                     11      3)000053)    3 (000003) 가Din)比Au旭巾에89回C000uneflo 9(0(006W四［z2
                  씨 NIOLLOLL
                                                     U目      4 田00034)    4)000004) 'lOluheth,回-p에'P四Coot urrencytLO心QAE@A四01＠唾）Z
              口 A外MS-Wi斗CORE-阻0(655                  口       5 似0035)     5)000005) "000hed미enP에ry四Concurr,nny(0@Q40002
              口 64卜MS川iN-Cl E-旺AP-LO-
                                                     므           드（0．
                                                                   즈0086)     61雙0006) '1叫艸므竺쁘．已'쁘饗唾些쁘드쯔빠쯔쁘．
                                                                                                           ．匹，
                쿤 쯔：二：r " " ""'n'r                   1 1 ,,Hnm    .mn1 們，,, J山m口艸m          r                                               1

    M口dA岫                           日)8 THree Starrrp                             UrA000o Starrrp
                                                                                                                          誥응응응客三
                                                                                                        ｝娑 ::                           000n擺押
  口 up나／도615-COO旿阻ORHAND마晦나1.0.0(1  2013-01＜낙 idOp                                2013-31-04 idAp
  口 A미-MS山너N -C ORE-日8태S-Li-)七.DLL  2013-01-04 143p                               2013-00-04 )44p
  그 API-,石-64斗Co昨FILE-L1-i-0 DLL    20)3-01-04 143p                               2013心1-04 144p         5.120 HA         080000FI2S    000000
  기 소만小i. W880r000.AUNflIOIO rflfll 沁m小LM rdtn                                    7n1 如l1md ! ddn        그 n77 H스         nYnnnnQt 7그   mnnnn 甘 i
 1  小小小 中나小叫小小月甲H트斗和m耐fm小a私mmm 小小‘; 小J
 Error, A) least one required enpAur or forwarded dependeocy 네as n升 f거Jnd




Fot))帥Lpro또 Fl                                                                                                                                   月
  n                                                                                                 m3n小n口口nn =     nm口



（그림） De口endency Walker 실행 화면



Qt 응용 어플리케이션을 Shared 라이브러리 방식으로 "뀨포斗다 보면 라' ］브러리가 위기
                                                   "한 디렉토리에
대한 접근" 1 필요가다． 만약 플랫폼에 라" 1브러리가 위치한 디렉토리를 찾지 못한다면 어플리케 " H크 내
에서 QApplicati아I 클래스의 addLibraryPath1( ) 함수를 사용해 라이브러리 디렉토리를 다음과 같이
지정할 수 있다．

 qApp->addLibraryPath ( H /some/ other/path") ;




                1.3 MacOSX
今Static Linking
Mac OS X 플랫폼은 Qt 응용 어플리케이션을 배포하기 위한 방법으로 Qt API를 Static 방식으로, Qt
공식 홈페이지에서 Mac OS X 버전을 다운로드 받은 다음 configure 옵션에 " static" 을 다음과 같이
추가한 후 컴파일해야 한다．

r cd /path/to/ Qt
 ./configure -static                                <other parameters>
 make sub-src



Configure 옵션에 대한 자세한 정보를 확인하기 위해서 옵션에 -help를 사용하면 configure어］ 대한
자세한 정보를 참조할 수 있다．


S Shared 라이브러리
Shared 라이브러리 방식은 Qt가 설기
                      '된 가위 디렉토리어］ 존 뀨
                                    "가는 라' ］브러리 디렉토리와 Includ" 파
일이 위치한 디렉토리를 참조하도록 PATH를 지정해야 한다. 또한 사용자의 Mac OS X 플랫폼에 Qt 라


                                                                                                                                   1 다양한 플랫폼에서 （거어플리케이션 배포 601


===== PAGE 603 =====
이브러리가 없는 경우 응용 어플리케이션 라이브러리를 함께 배포해야 한다．


D 라이브러리 의존성 체크
八4ac OS X 플랫폼은 응용 어플리케이션 라이브러리 의존관계를 체크하기 위한 툴로 otool을 제공한다．
이 툴을 이용하면 개발한 Qt 응용 어플리케이션의 라이브러리 관계를 확인할 수 있다．

otool -L MyApp . app/Contents/MacOS /MyApp


毗O아은 Mac OS X 플랫폼에 기본적으로 포함되어 있으며 터미널 상에서 사용할 수 있다. 이 툴은
Linux 플랫폼에서 제공하는 ldd 툴과 사용 방법이 비슷하며, 八ilac OS X 플랫폼 상어］ 응용 어플리케이
션 라이브러리 관계를 확인할 수 있다．



       1.4 Andr이d 플랫폼어因 （값 어플리케이션 배포

Qt를 이용해 작성한 소스 코드를 변경 없이 안드로이드 플랫폼에 적용할 수 있는 개발환경을 지원한다．
또한 구현한 어플리케이션의 디버깅을 위해 원격 Deploy를 지원한다. 따라서 Qt Creator상에서 컴파일
이 완료되면 안드로이드 플랫폼에서 배포할 수 있는 apk로 변환해 주고 원격 디버깅을 실행하면 안드로
이드 플랫폼에서 제공하는 에뮬레이터 또는 실제 디바이스에 자동으로 배포를 할 수 있도록 어플리케이
션을 실행한다．

Qt Creator 상에서 Deploy 기능을 실행하면 안드로이드 에뮬레이터 또는 실제 디바이스상에서 어플리
케이션이 실행될 뿐만 아니라 디버깅 모드를 지원한다．

안드로이드 플랫폼에서 Qt 어플리케이션을 배포하기 위해1Qt 공식 홈페이지에서 제공하는 안드로이드용
Qt 어플리케이션 프레임워크를 다운받아 설치하면 된다. 또한 다양한 운영체제에서 안드로이드 개발환
경을 구축하기 위해 Windows, Mac, Linux 운영체제상에서 개발환경을 구축할 수 있다．

운영체제          Qt 프레임워크
V피ndows       （가 5.x.x 幻rAndroid (Windows 32나川）
              Ot 5.x.x for Android (Linux 32-bit)
니nux
              Qt 5.x.x for Android (Linux 64-bit)
              Ot 5.x.x for Android (Mac)
Mac
              at 5.x.x for Android and iOS (Mac)



위의 표에서 보는 것과 같이 운영체제별 Qt 프레임워크는 Qt 공식 홈페이지에서 다운로드 받을 수 있다．
그리고 안드로이드 플랫폼을 위한 Qt 어플리케이션을 개발하기 위해 다음과 같은 패키지를 다운로드 받
아 설치해야 한다．




602 CHAPTER 17_ Qf 어플리케이션 배포


===== PAGE 604 =====
1패키지                                                                              다운로드 사이트

    Java SE Develo口ment Kit v6 이후 버전                                             http://www.oracle.com/technetwork/ java/ javase/downloads/index.html
    Android SDK Tools                                                             h뱌刃／dev이0口er.andrc沁．com/sdk기ndex.html
    Android NDK                                                                   httI玎／dev이야兀r.android.com八的冶／羽k/ndk기ndex.html
    A口ache Ant v 1.8 이후 버전                                                        http://ant.apache.org/bindown load.cgi



위의 표에서 나열한 패키지를 먼저 설치하거나 Qt 프레임워크를 먼저 설치하匠 상관없다. 여기서는 윈도
우 기반에서 개발환경을 구축하고 Qt로 작성한 어플리케이션을 안드로이드 디바이스에서 실행시켜 보도
록 하자．


S Java SE Development Kit v6 이후 버전 설치
안드로이드 개발환경 구축을 위해 Java SE Development Kit을 다운로드 받는다. 단, v6 이후 버전을
다운받아 설치하면 된다. (http://www.oracle.com/technetwork/java)

    盲云三ma
 e       +      C   什       WVn나
小


                                   小ern므거Y     DO나n匕MS        500jmenl帥그n    C口nm나미10      0근n기                                    Java!마姑 0110




                                                                                                                               茗
    J1Ya ＼侄
                                    Java SE Downloads
    I.e. 50 SU口P0n
    I.e. SD han50.d S Sn.
                                             He1t 如1ea!e5 任airy aeon＄引         Embedded Coo          n! 口   r口口 口C니mi口口亡

    I.e.!油added


                                                                                                                                于 Jean S円＄山nCo叫
1   O* 佃                                                                                                                             Jmm RDm
    Jaia Card
                                                   忌jay可                                                                        ! 1am 사긔S
1 1a뇨a N
    Hen m Jam
                                                     DO出NL｛汁n 1
    C口                                                                                                                          9 Fooeo.
    I甘1a Uigizule                               Java plallorm { JOKI 1151
                                                                                                                                9 foes 1
                                                                                                                                      Mi口a乙'I'
                                                                Java Platform, 針andard Edition                                  트 Ja寸且eel
                                      Java SE 7061                                                                                0.0叫D
                                      Tfl,sreleaye,noudeS mpv凡anl security tree alc口e S甘on아f recofllmeflaSti카 all 431O SE,
                                      USer5 UO口rcoArser匹 r叫ea5e



(그림) Java SE Development Ki



그림에서 보는 것과 같이 Java SE Development Kit를 선택하면 다음 그림과 같이 운영체제별 Java
SE Development Kit을 선택할 수 있다. 여기서는＼硝ndow용 Java SE Development Kit를 선택해
다운로드 받는다．


     亘始Va SE Den미야加cr11 K伎           X

    4- ．中 0             n   : ww山racle.com八echn아work力카a/j카ase/down幻ad的dk7-（幻ARt幻ads4880260.h

                                              Mac OS X 064                                  17949MB         ! 1'j瓦7551 macosx-n64.dm5
                                              Salons x86 (SVR4 packa9e)                     14502 M日        프 }div-I目51.s（只ans-1586,tar.Z
                                              S이crib eMS                                    9513 MS         !j4k- 71151 各olans-,5BS.tar.90
                                              Solaris 064 (SVR4 口ackaqe)                    2453 MD         !jdk- /u5l占lan,51564tar,Z
                                              S이arls *64                                    1628MB          ! ]46-7651-吼沁Iv斗n64.tar.gg
                                              60101,6 SPARC (SVR4 paceaov)                  135 39 MB       ! 月11-71151.5아an15 spa rc.tar.Z
                                              S이ails OP사？C                                  96 19 MD        ! jdlv-71151.s어ans-spany, bor,dn
                                              S미aIls SPARC 6小bit 喀VR4 PaCka口e               2394MB           竺 伯11-7的1占아aris.sparc岷.tarZ
                                              S이Cr15 SPARC 64七仕                             19 330日         !jdk. 7甘51占이ans-sparcv9.tar.qi
                                              바indowv edit                                  12364 M日
                                              Windows 694                                   12546M日         引芻客黑茗：然籌

    (II림) Window* Java SE Development Kit



                                                                                                                                          ] 다양한 플랫폼에서 （거어플리케이션 배포 603


===== PAGE 605 =====
 Java SE Development Kit 패키지 다운로드가 완료되면 설치를 시작한다．

                                                          yi斗
  스Java
                                                                 C>nAC1 E

  =mmq            따밀믈 II거하는 줌
                                                                                      뇨me111며IV 11111114 月Ya 5t 0eVrk叩r忙nt K吐 7 UpdliI Si




          3 Billion Devices Run Java
                                                                                      Jd Neit Ste［石 tn aCCe必 山寸心 Nn 如mmtmm dEVe奴好 9幻e됴 r由a5e mmS
          카m나 irm 뇨en tar',;' m                                                       a너 mJe tn m如 m 9et 5口ted md긔 dt l> L

          ,,, .0艾 亡arn口 山mn a{nd;


                              C）口ACLE



（그림） Java SE Develo口ment Kit 설치화면



 S Andr이d SDK Tools 설치
 Android SDK를 설치하는 방법은 Eclipse IDE를 먼저 다운로드 받은 다음 Android SDK를 플러그인
형태와 같이 다운로드 매니저를 통해1 설치할 수 있는 방법을 제공한다. 여기서는 Eclipse와 Android
SDK가 모두 포함된 ADT Bundle을 다운로드 받아 개발환경을 구축하도록 하자. 다음 그림에서 보는 것
과 같이 h就p: //devel아氾r. android. com/sdk/index.html 사이트에 접속하여 다운로드 받는다．


          and山ida［米 'An마미Si

              C    孔     0 developerandroid.com反tb/md毗htn너



 啼        Deve幻p可5 r            Design        Os-，叫叩            머stnbwte


 Training              At기 Guides      Ref efratce                    G어）이eS더ices               Sam머en



  DneetnpmT어ln                  Get the Android SDK

  Di）뇌Br如ad
                                The Android SOC provides you the API libraries and
  Settint) 印 WedS丁              den이0附 佃出 neness카yin build, tent, and debug
  Band涎
                                a口pa化rdndroid
  Setting up nfl
  E지Sting IDE                   作you rca new An如id developee. we,吐ml口lend P0U
                                由Dwnload the ADT Bundle to quickly start developing
  And,,거ASS叱山             V
                                apps it includes tIre enseetial Android SDI<
  E차加nng the S［米                cnmponefl沾and 0 0tis聊이 thiEdi5好e江泛 with
                                buil卜ingOT (Android De.叫여出To어旬 to 針man出ne
 ［幻Wa幻ad the SOIl
                                your Android op口den叫open帥t

  나0rm아Y                        w的 a 帥아叱oounload. the Aol Ban如 includes
                                everything you need to begin developing apps
  Support Libea斗                                                                                           Do나nloadtt氾 SDK
                                1 EU;哨eoAOlp山gin                                                            AnT 000dletor Windows
  Too뇨 Help




（그림） Andr이d SDK Tools 다운로드



그림에서 보는 것과 같이 "Download the SDK" 버튼을 클릭하면 32bit와 64bit용을 선택할 수 있다．
여기서는 32bit용을 선택하도록 하자 . 다운로드가 완료되면 adt나）undle- windows- x86-
YYYYMMDD. zip 파일로 압축되어 있는 파일을 압축 해제한다. 압축 해제가 완료되면 adt-bundle--
windows-x86-YYYYM八4DD 디렉토리 하위에 eclipse와 sdk 디렉토리가 생성된다.




604 CHAPTER 17_ Ot 어플리케이션 배포


===== PAGE 606 =====
                            卜 컴퓨터 卜 로걸 디스크 (C:) 卜 Android 卜 adt-bundle-windows-x86 卜

  구성 !                 라이브라리0듈 포맘 !                              공유 댜삼 !                급기    4 폴더

                                                               01률                                      ／丘＝ p
                                                                                                        jh


                                                               肛 ed唯Se                                  20]
                                                               案 S心k                                    20그
                                                                              riager.exe                20]



（그림） Andr이d SDK To이S 디렉토리 위치



그림에서 보는 것과 같이 C:\ 또는 D:\ 하위 디                                                                리에 Android 디렉토리를 생성하고 압축을 해제한
Andro姓 SDK To아S를 Android 하위 디렉토리                                                             ］동한다．

패키지                                           설치 위치

Andrc：永I SDK To이S                             C:\Android\adt-bundle-windows-x86


위의 표에서 보는 것과 같이 디렉토리명과 위치를 일치하지 않아도 된다. 따라서 독자의 편의에 따라 다
른 디렉토리에 위치해도 무방하다. 단, 추후 안드로이드 Qt 프레임워크를 설치할 Tril 각 패키지를 지정해
야 하므로 설치한 위치는 기억해야 한다. 압축 해제와 디렉토리 위치 지정까지 완료하였다면 다운로드 받
은 SDK가 제대로 동작하는지 Eclipse IDE를 실행시켜 보자. Eclipse IDE는 C: \Android\adt-bundle
 windows-x86\eclipse 디렉토리에 있으며 eclipse. exe를 실행해 보자.




（그림） Eclipse IDE 실행 화면



S Andr이d NDK 설치
Android NDK를 다운로드 받기 위해서는 http://developer.android.com/tools/sdk/ndk 사이트어］
접속한다．

    kadr미a von i An心어d [ a

         C   升      Li developer.aedtoid.conn八oolv/vdkfrvdkfiedex.htnvl

                              APIC prov1de the funcit이lality that pan need.
  Developer Toola
                              Downloads
  Dovadood             ／뇨

  Sett,ng Up the DoT           Plalfornt
  Bafldle                                          Package
                                Wndowv 32-ba        androd-ndk-t9c-wrndawsa86 z中
  Setting Up an        \/
  Exrrtng IDE                  나tadowa 64七it        endro,d-ndk-円C-wlndawS
  Andro,d Studro                                    a86_64 C巾

  Eoplorrng the Son             Mac OS X32-         andra.d-ndk-円c-dar사in-oaa tat 502
                                奴t
  DoVr 01004 the ODE
                                h a nn n0 V 二 月     n n겨 r八1d nai/ rnrb d


（그림） Andr이（I NDK 다운로드 사이트



                                                                                                     ] 다양한 플랫폼에서 （거어플리케이션 배포 605


===== PAGE 607 =====
그림에서 보는 것과 같이 \Windows 32小此용 Android NDK를 다운로드 선택해 다운로드 받는다. 압축
파일을 다운로드 받아 압축을 해제하고 다음 표와 같이 디렉토리 위치를 맞춘다．

패키지                                 설치 위치
Android NDK                         C:\Android\android-ndk-r9c



NDK는 Native Development Kit의 약자이며 JNI 기반의 c/c++ 또는 독립된 모듈로 사용하기 위한
c/c++ 소스 코드를 컴파일할 수 있다．


@U니                   , 컴퓨터 , 꼰드카:1 , Android 卜 android寸ndk-円（ 卜
      구섬 !          라이브러리0* 포함 r             공유 대삳 甲             云기           느r 폴더

                                        아릎

                                         案 build
                                         未 面Os
                                         U立g 히at幻rms
                                         轟 伊ebu滋
                                         案 sam히Os
                                         纛 5m兀小
                                         轟 tea뇹
                                         多 tod놔chains
                                         f    面cumenta如曲tm


（그림） Android NDK 디렉토리 위치



心 Apache Ant v 1.8 이후 버전 설치
Apache Ant는 http://ant.apache.org/bindownload.cgi 사이트에서 다운로드 받을 수 있다. 버전은
1.8 이후 버전을 설치한다．

r \   AF日
        （Ron    昏niHY ｛거51 X




         THE
         APACHE ANT
                                                                                         toe A4t求ie Rn sat

 11어ne   La코二03


1 " 「旨뜯，“n, '
    n L(enSe
    口 r1enS
    口 SeCie]tV RepoRts         Binary O朽tr什）utions
 1 m)rU1n們1tatkm
    口 Ha1거m
    n Relat日d Projects
    口 EXtenm TD어5 긔k1 了月
    U R8S어 CeS                 Apache Mmt m003aoa library anna C口mmand小mm. tao that ito. 山4小四 loft뉘ar日；
   口 Frey此city 心yod C＞此5Um5
   口Wm                          i加Wn幻athnq Apache Atte
   口 Ratings片OR片미1巧？
 1Oomnk)ad                     10. the 0田 be油mm no domonm比ad a bleary tisbutuose of tee boat on. of ott amen.,. It is
   口 日Salt Oltttlilfltc>       good Rotten. to coeft the ini口ate of the 小드tntu000 川0,. .놔） .ciaiy if you otto toting ore
   .5여JrCe 아5b1X川XX作           of ott t 口t 引ce.. In Order no do Ui, you tooth a. the 引gnatures from ott main ti s010al山n
   口 Ant M긔ned




（그림） Apache Ant 공식 홈페이지



그림에서 보는 것과 같이 Apache Ant를 다운로드 받는다. 메인 화면에서 "main distribution
directory" 링크를 클릭하면 다음 그림과 같이 binaries 항목을 선택한다．




606 CHAPTER 17_ （그t 어플리케0썬 배포


===== PAGE 608 =====
1ndex of /dist/ ant
        岫
          笹
 J口口口
                               a기 2-23니 3 04:02
                               2013-12-29 05: 12
                               2013- 끄-02 22:09


（그림） t기naries 항목 선택




                        n\ew.apache.org/ J:ct/aint!binanies/?C = MO= A


        epa아it-ant-I 요 3七 小 tar. 吐 .45        20日니 ?29 05 'Il    33

        apache-ant너 요3七in. tar, qp. shal      2013너2-29 05:11     41

        a口ache-ant니 且3-bin, tar. gp, sha512   20田니？四 05:11       I四

        a口&che-a吐니 且3七m 기p                    20田니？29 碼：11       7．미

        opec比-ent니 且 3七it pip. asc            2013나？29 ［石：tl     521

        apache-act니 且3七in. zi口md5             a기3-12-29 05: 11     크

        apache-ant니 요 3七In. 2Ip,帥at           2013너？四 ［石：II       41

        a口ache-ant니 9. 3七in zip, she듸2        20田너？四 [E: t1      I四


（그림） Apache Ant 압축 파일 선택



그림에서 보는 것과 같이 ZIP 파일로 압축된 Apache Ant 파일을 다운로드 받아 다음 표와 같이 압축 해
제한 후 디렉토리를 맞춘다．

 패키지                                                  설치 위치
 Apache Ant v 1.8 이후 버전                               C:\Andr이小apache-ant너요3




                      라이브러리에 포함 !                       공유 대상 !          굽기

        ,=1 卞긔＋. 日．                                    미릎                      수정한 날짜
         a-' 百서 尖 / 1
          上（沁四匣 드라이브                                   率 bin                   2014-01-1;
           斗 다운로드                                      幽 etc                   2014-01-1;
          =   바탕 호11                                   半 lb                    2014-01-1;
         冒 최근위치                                        拉 manu키                 2014心i-i;
                                                       圖似ch.xml                2013-12-2三
     旨 라어브러리                                           圃甲卜m2.xml               2013-12-2三
          國 문서                                         口INSTALL                201多蚣名


（그림） A口ache Ant 디렉토리 위치




                                                                               L다양한 플랫폼에서 아어플리케이션 배포 607


===== PAGE 609 =====
0 （값 5.x.x for Android(V피ndows 32나川） 설치와 환경 설정


                             口 中F玎（기ect.org/d口뇨vnloac八

                                           뇨7 Qt Online Installer for Windows (13 MB) (Into)

                                           心   9t5工0 for Andr이d（니flux 32-b汽490 MB)(Ini이

                                           幼   Qt 5,2.0 for Andr이d (Linux 64-b比488 MB) (InS이

                                       口       Qt 5.2.0 for Andr이d (Wind口ws 32-b比 761 MBl (,nf이

                                           乞iQt 5.2.0 for Linux 32-bit (425 MB) (info)



（그림）（가 5.x.x 伯r Andr이d 버전 다운로드



그림에서 보는 것과 같이 Qt 공식 홈페이지에 접속해 Qt 5 如r Android 32bit 버전을 다운로드 받는다．
다운로드가 완료되면 설치를 시작하자. 설치하는 과정에서 Installation Folder를 지정하기 위한 다이
얼로그가 활성화되면 안드로이드 Qt 프레임워크 버전이 설치될 디렉토리를 지정할 수 있다．

필자는 기존어］ 설치했던 윈도우 버전의 Qt가 설치되어 있으므로 안드로이드 버전과 구분하기 위해 디폴
트로 지정된 설치 디렉토리명을 "C:\Qt\Qt5. 2.0_android" 로 변경하였다．

                                                           晦心
                                                                               10 才520500rcp


  In引川｝誌on F어des                                                              Select C050p0000tts

  P冶a8日 spec御 th日 回der 늬here di 02.0 tetll beinetulled                        미ea5日 S미sot As components you 나units Install,
   C州0州0低之0-u叱m텍                                           6,000；且． 1          4 多야                                      아 5.00
                                                                                  三 3520                                 10沽 :ompsnent 놔ii oecu口y
                                                                                  三 1:d5                                 a口口m川rnatelp 2146떠 0n y0Ur
                                                                                                                         hard disk drive




   團Associate common tile types colA OtCreator.




（그림） 아5 化r andrc기d 설치 화면



두 번째 설치 화면에서 보는 것과 같이 "Select All" 버튼을 클릭하고 "Ne玭" 버튼을 클릭해 다음으로
넘어간다. 다음 화면에서는 라이선스 관련 사항이며 '동의함’ 라디오 버튼에 체크를 하고 "Ne砒" 버튼을
클릭하면 다음 화면과 같이 설치가 진행된다．

뇨) LI 350.0O1山P
  Installing Qt 520


  Installing component fssenOal nnsdulss


  蜃b9뾰0烈叫.1




（그림） 0而 向randroid 설치 화면


608 CHAPTER 17_ Qt 어플리케U썬 배포


===== PAGE 610 =====
그림에서 보는 것과 같이 설치가 완료되면 "Finish" 버튼을 클릭한다. 여기까지 진행하였다면 안드로이
드 플랫폼 상에서 Qt 어플리케이션 개발에 필요한 모든 패키지 설치가 완료되었다. 설치한 패키지 중
Android SDK Tools가 위치한 디렉토리 하위에 보면 eclipse 디렉토리가 있다. 이 디렉토리에 있는
eclipse. exe 파일을 실행해 Eclipse IDE를 실행시켜 보자．




           w解【R
（그림） Eclipse IDE 툴의 SPLASH 화면




  놔act a 끼口r1斗1呻
  A！兀stor們 叩Ut pn가ects in a！마derc균lied a workspace
  Choose a workspace fot如r to u始 fat this seusion


   orkupace: 小1幽田如                                        &owse...




   j 나seth在 astF比｛扼fault and do not ask ag出n


                                                     OK    Cancel

                                                                     /



（그림） Workspace를 지정하기 위한 Workspace Launcier 다이얼로그 화면



Workspace Launcher 다이얼로그 화면에서 프 로젝트 Workspace를 지정하는 화면이다. 여기서는 지
금까지 패키지를 위치시킨 디렉토리 하위에 wo "kspace를 지정하도록 하자. Workspace 위치 지정을
완료하고 다이얼로그 하단에 있는 "OK" 버튼을 王릭하자．

Eclipse IDE에서 AVD(Andro沁 \[irtual Devi{}e) Manager에서 안드로이드 에뮬레이터 또는 실제 안
드로이드 플랫폼을 등록해 보도록 하자. 다음 그 에서 보는 것과 같이 코；clipse IDE가 실행될 것이다．




                                                                1 다양한 플랫폼에서 (m어플리케이션 배포 609


===== PAGE 611 =====
 빡月匹吼薑瀜, 螂忿乞如 1 ,                                                              小 켜그gii
                                                                               I느   -   H
     e Ed作 Ref act아 Source Navigate Search Project 瓦；;;) 岫nod（乂O H叫p
                                    ＼又 拉 中 0 ' 1k Run
                                                   乙 Debug
       Pack羽亡 Eop小rer 1 1
                                                                                        Run History

                                                                                        Run As

                                                                                        Run Con徊urati아瓦


                                                                                        DeE乂J9 네5加싸

                                                                                        Debug As                             卜

                                                                                        Debug Con!心ura如Ins--



（그림） Ec먀冶e IDE 실행 화면



 Android Virtual Device를 등록하기 위해1 그림에서 보는 것과 같이 메뉴상에서 "Run" 메뉴 하위에 위
 치한 "Run Configurations
                  " 메뉴를 실행한다. 이 메뉴는 안드로이드 어플리케이션을 배포할 에뮬
레이터 또는 실제 디바이스를 연결하기 위한 메뉴를 제공한다. "Run Configurations" 메뉴가 실행되면
 왼쪽 선택 메뉴에서 "Android Applicati아I" 메뉴를 클릭하면 "New的nfiguration" 메뉴가 나타난다．
이 메뉴를 선택한다．


 口_t. . te 四t 11넋 ntn oooflgar.t油1日
 Q (And,머d] Pt이e0t Nanva 10 ieqjared


  L으 隘 川      宅 芽 1               I Nate也 New_v0rthgurat,而
  10口e 砥er md
   1 固 Mdro,d cipplnation
                                                                         r
       西 N태Jm佃出鉀어｝
                                  慝黑蛙呈忿
                                          씨w000 F片口lept to pock device
    而 U/don山山吐 Tort
    固 c/c, , A口伊的t心n                      녀unoh on all oornpavblo do너C出／AVOS
    m Java ap꺼ci                  L      Aulic드 do니Ce5 an口 A뇨l그 5 丁
                                  ;
    口jJava ci아州C盛由n
                                  n 孕 AvIate拙殉 머0k r帥附蜘曲吐 脚四5 山e5Pa佃叱 AVO 仕 sot 놔叫 加riches on compo0b似蜘叱./aNto oak.,姓5毛
    J0 Jun作
                                             Soloot a p0000nad aao卞아d V竹odDs吼e 幻r d叩1四mont
    卜 山unth 臼loop
                                              AVD Name                                         미attorm   U/I Leo甘   CPU/A川
                                                                   ho 立"P. O川abm




（그림） Run Configurations 실행 화면



그림에서 보는 것과 같이 하단에 위치한 "Manager" 버튼을 클릭한다. "Manager" 버튼을 클릭하면
Android Virtual Device 八/lanager 다이 얼로그가 실행된다．

     Android Virtual Devi氾 Manager



    Li默 {f existing Android Virtu히 Devices 炚doted at C：斟나S甘sWek恥Im境andrl沁什avd

                                                                                            API Level    CPU/AR!



（그림） Android Virtual Device Manager 실행 화면



"New" 버튼을 클릭하면 가상 머신을 등록하기 위한 다이얼로그가 실행된다．




610 CHAPTER 17_ Qt 어플리케이션 배포


===== PAGE 612 =====
 C     E計 小d也dv皎U칡 U                 (AVO)


     AVD Name:            QtV吐U出Device

     De니ce:               10로坡Xt3A Cr;比0 (1281) 工 800: md例

     Target               Mi打口附 4.4 - API Sm劍 19

     CPU/ABE              ARM 訂me計긔 Y7aj                                    r

     Keyboard:           回 Hard니1冒e keyboard 匹event
     S匕0:                團 D타地叩 蜘n 咐往h han柶are Co巾여S

     Front Cam臂可          None

     Back Camera:         None


     Mem畇心pBS가Is:          RAM: 512                 VNI Heap: 32



     Internal Storage       102                                     mm
     SD Card:
                           勘 S臣e:     1024                      ［皿m
                          ｛弓 File:



     Emulat由nOptions:      刃Sna阡Ia艾                     C好to目

            erride the exisOng AVD w41t the same name




                                                                   Cancel       ]

（그림） 새로운 Android V吐usi Device를 생성하71 위한 다이얼로그



그림에서 보는 것과 같이 설정이 완료되었다면 하단의 "0K" 버튼을 클릭해 설정을 완료하자．

1 Aik奴加 Virtual De너ce Manaxer                           ;j多侄乙               i弦       努驀，莩超月쩍＝斗＝
二  乙，n1                   /                              庶可 = 'm=           :: 三三      m4汪＝ :! 1                     乙


     Android Virtual Devices ! Device Definitions

      List 肝 existing Android V吐U引 Devices 眈曲datC斛出帥49叱由岫畔air小oid쀼av（쩍

       AVD Name          佃get Nan作                     마Ct把on        API Lev이       CPU/ABI         1nm
       V佯帥出oidV... Assdro넙 4.4                         4.4           19             ARt너 (arm eab
                                                                                                           Edit.

1                                                                                                         Del映e...

                                                                                                          Fee키




                                                                                                    am
                                                                                                            7.
                                                                                                    Ci:
（그림） Andr이d Virtual Device Manager 실행 화면



그림에서 보는 것과 같이 등록한 Virtual Device를 선택하고 하단의 "Start" 버튼을 클릭하면 안드로이
드 가상 디바이스가 실행되기 전 가상 디바이스의 Launch Options 다이얼로그가 실행된다. 다음 그림
에서 보는 것과 같이 "Launch" 버튼을 클릭해 가상 디바이스를 실행하자．




                                                                                                                         1 다양한 플랫폼에서 아어플리케oI. 크 배포 611


===== PAGE 613 =====
包I Launch OptLons

 Skin:    1280x800
 Density: Medium (16O)
 回 Sc引C 師的n0 re出 5注e


         Sce죤en 듸z숀 tin): 10.1

         r벼（가l屯可d目：      96            ！立


         Scale.

 ［그 w巾e user data
    Launch ; rom snapshot
    ；引／e to un햐）sh仗



            Launch            Cancel

                                       .1
（그림） Launch 0이向nS 다이얼로그 실행 화면



Launch Options 다이얼로그는 가상 디바이스의 실행 옵션의 크기 설정을 변경할 수 있다. 최초 가상
디바이스를 실행하면 디바이스가 실행 완료될 때까지 다소 시간이 소요된다．




（그림） 안드로이드 가상 디바이스 실행 화면



안드로이드 실행 화면이 정상적으로 동작되었다면 설치한 Qt 5 for Android의 Qt Creator를 실행해보
도록 하자. 실행이 완료되면 다음 그림에서 보는 것과 같이 "To아S" 메뉴 하위에 "Options" 메뉴를 선택
한다．




612 CHAPTER 17_ （가 어플리케이션 배포


===== PAGE 614 =====
   Qt Creator

 F陀   Ed比       m川d ［沁bug         An키yze
                                              (0     山C盛e..                      CtrloK
                                                     C++                                 卜

                                                     QMWS                                卜

                                                     F cc km a rks                       卜

                                                     （조de Pa笠［叫｝                         卜
                                                      知13Cn孤                             卜
                   E乂am이es                                                               卜
                                                      E玳em引
                                                     ［긔行．;;
                   Tutorials




（그림） 01 Creator 실행 화면



"Options" 메뉴를 실행하면 다음 그림과 같은 다이얼로그가 실행된다．

이 다이얼로그 왼쪽 메뉴의 "Android" 를 선택하면 오른쪽어］ Android 설정 화면이 나타날 것이다．
Android 설정 화면에서 Andr아d SDK, NDK, Ant 그리고 JDK 디렉토리 위치를 지정한다．

 항목                                          디렉토리 위치
 Andr이d SDK bOc계ion                          C:\Android\adt-bundle-windows-x86\sdk
 Android NDK location                        C:\Android\android-ndk十r9c
 Ant location                                C:\Android\apache-ant-1.9.3\bin\ant. bat
 JDK location                                C사가ogram Files 似86)\Java\ jdkl.7.O了



                     91d,oid
                     PD的dCot,佃raNor

                     Android SDKIocaN口m c附向1山이d卄adt七Un버小내nIO나8 X田Wadk                                                               i 日0늬＄日 1
                     Andro너 MW IoCa亡bE C卄end,이d쀼androl小od卜砒                                                                         L 日r0nBe       1
                                        Fat, rd 타00노hamns 幻Fe冶 NW.
                                        翌 仙torna血a仰 Cm伯 내引마 知出이a to이 'a톄n5

                                        사攝抹描鸚烈謐％騶期毗蜘山蜘帥，
                               Ant Inc帥ant C附Md세dwapache-aro-I,且引州rWaotbat                                                           日r口나5日

                           JOE Inc.如n ｛附ptogtam 테日5 m田）卄Jat,.쌔炚I.?.口引1                                                                ban田8


                      AdO Mflpr                                               Soalnot/data口arlAbi size: IMI MN   :   rS1anA1dr01dA너）Mao日8日引

                                        AVD Nam                      alto, 自叫                        CnUfa80                          Add      ]

                       야山Au眺乂니Ce                                     API 19       카n긔eat斗OP.                                         tattoos
                                                                                                                                1




                                                                                                          ！毛i年幽나 11鈿耐                뇨蜘i磁j




（그림） 0아向ns 다이얼로그 실행 화면


그림에서 설정을 완료하였다면 "APPLY" 버튼을 클릭한 다음 "OK" 버튼을 클릭해 설정을 완료한다. 이
전에 Eclipse IDE Tools에서 AVD(Andr아d Virtual Device) Manager를 실행시켰지만 Qt Creator
에서도 AVD Manager를 통해 안드로이드 에뮬레이터 또는 실제 디바이스를 관리할 수 있는 기능을 제
공한다．


                                                                                                                                    l 다양한 플랫폼에서 （코어플리케이션 배포 613


===== PAGE 615 =====
여기까지 진행하였다면 Qt 어플리케이션을 배포하기 위한 모든 준비가 완료되었다. 따라서 Qt Creator
에서 작성한 어플리케이션 프로젝트를 안드로이드 에뮬레이터에서 실행하기 위한 방법에 대해 알아보도
록 하자．



 J       Ne나 File or Project
 1j      Open F油 or Project               C1i1.O
         야祀nFile Wttli
         Recent Ales
         Recent Pr& t5
         Se各51O15
         Sessi마l Meneoer..


（그림） Ot Creator 프로젝트 생성



그림에서 보는 것과 같이 "File" 메뉴를 클릭하고 하위 메뉴에서 "New File or Pr이ect" 메뉴를 선택해
새로운 프로젝트를 선택한다. 다음 그림과 같이 New 다이얼로그 상에서 "Applications" 을 선택하고 오
른쪽에 "Qt Widgets Application" 을 선택한다．

釀New二1出                      ；『小                          毛芬m쿄二나m幷口小
  Chor그cc a 伯m히ate
  1
      마O洽Ct드                                                   t工 Qt出由e如A仍꿰cat心l
       AP하'coo며S                                                4   Qt Quick Application
       Ubrantes                                                1    QtCO陌이e Application
       Other Pr口忙Ct                                            目    HTML5 Applicat由n
       Nofl-Qt 꽈이cci                                           胡    QtQsjick UI
       ION乂月t 마의e心

      Fl隔 and Clas＄心

       C, +



（그림） 프로젝트 생성 다이얼로그



"Qt Widgets Application" 하면 다음 다이얼로그 화면에서는 프로젝트 이름을 등록하는 화면에서 프로
젝트 이름과 프로젝트 생성 위치를 지정한다．


                         Introd山煎川 and Project 山Ca如n
  中 L口cater
    K配                   Tb始 wizard generates aOl 쌔dgetn 却1小cation 마oject. The ap［小Carl口n deriues bed曲너I Iron,
                         OApplinatio,r and includes an empty widget.
        Details
        isteterats)

                             Name;     Cello붜0刈


                             Ctaate in: C附마아毗t
                             國Use as default prolect locadon




（그림） 프로젝트 이름과 위치를 지정하기 위한 다이얼로그



다음 다이얼로그는 Kits를 선택하기 위한 다이얼로그이다. 다음 그림에서 보는 것과 같이 두 번째 항목인
"Android for armeabi-v7a" 항목을 선택하고 하단어］ "Next" 버튼을 클릭한다．


614           CHAPTER 17_ Qt 어플리케이션 배포


===== PAGE 616 =====
 @              口 야Widgets Application


                                  Kit Selection
                1 口coO口n
            4   K沁                Ot Creator can use to日 f口Ilowing k的 f口r 미5忙ct Hello붜arId
                DeS키姑
                Su作1mary             巴Q Android 化r armeabi (6CC 4.8. Ut 5. 2. 0)                                          Det궤陌 !


                                     團Q Android for armeabi-yla (6CC 4.8. Ut 5. 2.0)                                      Details !


                                     回Q Android for cOO (6CC 4.0. Ut 5. 2.0)                                              Deta小3 !


                                     巴 m De引stop Ut 5. 2.0 MintS놔 32bit                                                   Details !




                                                                                                                            Cancel



（그림） Kits 선택 다이얼로그


                                                                                                                                m又＝m




J
                       Widgets A口p汝atlorr                                            月：
                                                                                                                                      i1
     ＠口Qt
]               .,,,,,,           p『이ect M“咽em帥
                     09.,, ,      Add as a uu,
                                             :
                                             bprujeC.   t to project: , None
                                                                         '
                                                                                                                  '   1
            ,Kits,                                                                                                     }




                                                                                                                                      11
              Details
                Summary           Add t。eersiun c。
                                                 ntr。
                                                    l:              r<       Nnne>                                , 皿m 1
 1                                  Files t。be added in
 1                                  Cr \proj'st\ fte11oWortd



「                                  變照：::                                                                                              掩
d                                   客：客然’，：놔


1
（그림） Summary 다이얼로그
                                                                                          mm1H小小小1mH中叫小J
                                                                                                           디S治h             Cancel    I




그림에서 보는 것과같' 1 "Finish" 버튼을클릭斗면 프로젝트 생성 ' ] 완료된다． 프로젝트 생성 " ] 완료되
면 mainwindow.ui 파일을 클릭해 UI Designe느 화면으로 전환될 것이다. 폼 상에서 다음 그림과 같이
QLabel 위젯을 배치시키고 라벨에 "Hello World" 를 입력하자．
如 rneine,nd毗벼 H베O 1
 File 日d Boild DetOg




（그림） QLabel 위젯 배치


                                                                                                                          ] 다양한 플랫폼에서 （가어플리케이션 배포 615


===== PAGE 617 =====
위의 그림에서 보는 것과 같이 위젯 배치를 완료하였다면 "Build" 메뉴에서 프로젝트 빌드를 선택하고
실행시켜 보자．



             方   Bu帖 All                     Ctil*Shift出   nwindo城h
             /   由川dP呵吼t ',F似口V的rtd"         Ctrl.B            IlAI卜｛WINDUW H
                 Run qrnake
                 a바ki F沁 1'rn斟TI硼ndm甘h'      Ctrl.Alt+B         <QHaintlinhlow
                 Deploy All
                                                             注！全 Ui {
                 加的y 多f미e咬 "Hel出Wo巾f
                                                              Liifl卄mndl｝川;
             火   Rebjifd All
                 Rebu小土 PT아ect "He加WI州d"                       in卄inth｝叫 : P 1王
             y   Clean All
                 Clean Project "Hellos敞州d"

             口 Cnc引 Build                                     二 LC主 t Hainl,lind
                                                             구"Z' n,力7n( ) ;
             >   Run                         Ctd...R




（그림） 프로젝트 실행 화면




 H쉬幻 World




（그림） 안드로이드 디바이스 상에서 （거 어플리케이션 실행 화면



그림에서 보는 것과 같이 Hello World를 출력하는 Qt 어플리케이션이 안드로이드 플랫폼상에서 실행된
것을 확인할 수 있을 것이다. 지금까지 안드로이드 에뮬레이터에서 실행하는 과정이 다소 느리다. 만약
독자 중 안드로이드 플랫폼 기반의 스마트폰 또는 태블릿과 같은 실제 디바이스를 가지고 있다면 실제 디
바이스와 연결해 Qt로 작성한 어플리케이션을 실행시켜 보도록 하자. 실제 안드로이드 디바이스와 연결
하기 위해서는 디바이스의 개발자 옵션에서 "USB 디버깅" 옵션을 체크한 다음 USB와 연결한다．




616 CHAPTER 17_ Qt 어플리케이션 배포


===== PAGE 618 =====
（그림） 안드로이드 스마트폰에서 USB 디버깅 체크



USB 디버깅 옵션을 체크하고 안드로이드 실제 디바이스와 컴퓨터를 연결하고 Qt Creator 상에서
Hello World 프로젝트를 "Run"하면 다음 그림과 같이 실행할 안드로이드 디바이스를 선택할 수 있는
다이얼로그가 실행된다．




              四U叫tmm
              A耐아d44 ABtatmeal汁C7a arC,08b




          Befre而B.而亡三區r] ［口i而g而i；
                                而礪；
                                  可而tiC可
        四 Nw.y日 US. Wit do너Ce f Or 台TCIIIIUSBUr므 ormOaC卜ode




（그림） He的 World 프로젝트를 실행할 디바이스 선택 다이얼로그



그림에서 보는 것과 같이 실제 안드로이드 디바이스를 선택하고 "OK" 버튼을 클릭하면 연결한 안드로이
드 디바이스에서 실행되는 것을 확인할 수 있다．




（그림） 안드로이드 디바이스에서 at 어폴리케이션 실행 화면


                                                              1 다양한 플랫폼에서 （거어풀리케이션 배포 617


===== PAGE 619 =====
四                                    Mod（이                       ]28     QDateEdit                   36, 42

Advanced Widget                94    Model 클래스                   461     QDateTime                   50, 176

Animation                     539    Mod이／View 아키텍처               ]27    QDateTimeEdit                     50

Animation 다amewo다
                （             274    Multimedia                  593     QDesk幻口Widget               94, 98
                                                                         QD回                          36, 51

回                                    回                                   QDialog                            37

Basic Widget                   34    OpenGL                        13    GD（그U벼eSpinBox              36, 53

Bearer Management             368    Overlays                    246     QEasingCurve              177, 278
                                                                         （正陀D洌og                           115

日                                    日                                   （아켜eSystemModel                  128

Canvas                        584    paintGL()                   245     QFocusFrame                 36, 55

Composition                   222                                        （아二ont                           177

C（그ntainer 클래스     ·164, 187, 308    回                                   아七ntCombo日ox                36, 58

Context2D                     585    QAbstractAnimation          276     （平on山ialog                        114
                                     QAnimationGroup             281     QFrame                             37

El                                   QBackingStore               209     QGLContext                       244

[） 日us                        415    QBitArray                   168     QGLFormat                        244

Debugger 설정                    23    QBrush                 169, 214     QGLWidget                        244

Delegates                     128    QButtonGroup                  37    QGraphicsBlurEttect              238

                                     QByteArray            169, 193      QGraphicsColorizeEttect     · . · · 241

回                                    QByteArrayMatcher           193     QGraphicsDropShadowEttect     · · 239

Gradients                     217    QCalendarWidget        94, 100      QGraphicsEttect                  238

Graphics View Architecture " · 227   Q（가伯r                       194     QGraphicsltem                    225

Graphics View Framework· " " 224     QCheckBox                36, 37     Q아a아ics야）配啣태ect             · · . · 242

GUI 이벤트 Replay 테스트         · ·.497   OColor                      173     QGraphicsScene                   225

GUI 이벤트 시뮬레이션 테스트 · . 496            DC이or[）回og                   113    QGraphicsS\／이tem 클래스          · · 269
                                     DC이un가小기ew               94. 95     QGra아기csView                     225
                                                              36, 40     QGridLayout                        92
口I                                   QComboBox

initializeGL( )               245    QCommand니nkBu卄on      · · ·36, 41   QGroupBox                          37

PC                            407    QConicalGradient             217    QHBoxLayout                       90

Iterator 클래스                  308    QCurs（그r                     173    （괴con                            178
                                     QDataWidgetMapper    · · ··94, 96   Qlmage                    178, 209

El                                   QDate                       174     （긔n口utDialog                      111

Main Window                   123    QDate 클라난느                    43    QKeySequence                     179




618 찾아보기


===== PAGE 620 =====
QLabel                    36. 60       QSpinBox       ·{            36. 53     GUn                      186
（丑atm ］앉ring                  194      Os이itter                          37    OVariant                  187
QLCDNumber                36. 60       Os이itte岫婉                         37    QVani카사Anim졔口n            277
O니nea떠治d陀nt                   217      QSq（그uery卜기cdel                   128   QVBoxLayout                91
Q［그neEd作                  36. 62       QSqlRelati。
                                                 n lTableM。
                                                          del        '   128   OWidget          36, 80, 209
QListView            94, 127, 131      Q5qlTableM。el                     128   QXml5treamReader 클래스 · '318
0匕00톄e                        195      Q5tackedWidet                     37    QXml5treamWriter 클래스   . · .3伯
QMacCocoaViewContainer        ·94      Os治ndard陀小卜加d쉬                    ]28
QMacNativeWidget               94      Ostring         1          184, 195     LI
qmake                           29     Q5tringList                       196   resizeGL()               245

OMargins                      180      Q5tringListM。   bel
                                                                         128
QMenu                     36. 64       Q5tringMatchr                     196   日
QMenuBar                       64      Os四Genera巾r 클래스                   270   SAX                      325
QMessa（그eB（그x                  118     QSvgRende뗘r 클래스                   270   scene 좌표                 230

QML                             10     Q5vgWidget 클래스                    271
QOpenGLPaintDevice            209      OsystemSem phore 클래스 " 410              II
QPainter                      208      Ot              I                  11   Thread                   288
아그alette                      180      Qt Assistant                 18, 26     Threading                247
OPen                    180, 212       이Crea幻r                            18   Transtormation           220
아긔cture                        181     아Cre졔0시D{ T的                  ]2 18
아긔xmap                  182, 209       Qt Designer                  18, 28     四I
QP이nt                         182      Qt Designer 1ooI                   28   Unit Test                492

QProcess                      423      Qt Quick                    14, 504
（아가（그gressBar             36. 67       아Test                             488
（아가四ress미slog                  111     Qt 프로젝트 생성                         19   m
（갸갸叩帥yAnimation               277      QTabBar                      36. 85     View                      128

QPushButton               36. 55       OTableView              94, 127, 132    View 좌표                  230
Q（그uaterr기ion                 182      oTabWidget               36, 37, 76
QRad治IG田데ent                   217     QThread 클래스                       292   口
QRadioButton              36, 68       OTime           1           46 185      XML                       316

ORect                         183      O기meEd仕                      36, 46
QRegion                       183      QT。
                                         。lBar             1              78   日
QScr에Area                       70     OT。
                                         。lB。
                                            x              1              87   다이얼로그                      ]]]

OScroliBar                 36. 71      OToolButton                  36. 88     데이터 주도 테스트               494

QSharedMemory 클래스         " " · '410   OTranst。
                                              rm       1                 186   데이터 클래스                   167

QSize                         183      OTreeView                         127   데이터베이스                   443

QSizeGrip                 36, 72       OtWebKit                          378   동의어                      443

QSlider                   36, 74       QUndoView                          94   디버깅 모드                     31




                                                                                                찾아보기 619


===== PAGE 621 =====
日                         口                       이벤트 처리        233

라디오 컴포넌트           436    사용자 정의 다이얼로그      ]21   인덱스           443

레이아웃                90    세마포어（Sema아'ore)   301
                          슬롯                ]58   日
回                         시그널               ]58   카메라 컴포넌트      434

멀티 쓰레드 프로그래밍       295    시퀀스               444
문자열 클래스        ]64, 193                           日
                          日                       테이블           443

回                         아이털J 좌표           230
벤치마크 테스트           499    에디터 기능             24   回
뷰                  443    에디터 툴바             24   프로젝트 버전 관리     21

비디오 컴포넌트           431    오디오 컴포넌트          427   폴러그인 제작과 배포   ]47




620 찾아보기


===== PAGE 623 =====
Qt 5
데스크탑, 임베디드 그리고 모바일 등과 같은
                               Programmir四
                               G네de

멀티 플랫폼 프레임워크 기반 애플리케이션 개발을 위한 예제 중심의 실무 가이드

I     아는C卄이외어r파이썬，루비， 펄등다양한언어를지원하며전서1계약40만명이상아7H발자가다양한컴퓨
I     팅롼경에서순多믄令프트웨어를7卄발하고있습니다· 따라서일반사용자깬플리케이션，멀티미디어· 시스템관리를
I     Back-end· 天陪자，국방，가선，모바일에이르71까지다양한분야에서아를활뇽 "가
                                                 고있습니다·
I     이책은고급G니와O甲nGL ES를사용한3D그래픽애플리케이션을개발 '차  고자차  "는사람들이읽기에좋은책으로·
I     개발에 필요한 아 A디를 예제를 통해 쉽게 이해할 수 있도록 하였다．




    Chapter 01 Overview                         Cha口ter 1(工Con怡ner 클래스와 Iterator 클래스
    Chapter 02 유용한 툴과 qrnake                    Chapter 11 XML
    Cha口ter 03+GUI 설계와 제작                       Chapter 12 데이터 커뮤니케이션과 인터넷 프로그래밍
    Chapter 04 시그널과 슬롯                          Chapter 13 멀티미디어
    Chapter 05데이El 타입과 유용한 조작 클래스               Chapter 14 데이터베이스




                                                                                            그
    Chapter 06 파일 입출력                           Chapter 15_Qt Test Framework
    Chapter 07 그래픽스                             Chapter 16Qt Quick2I- QML
    Cha아er 08卄Animation 다amev四rk과 없ate Mad기ne   Chapter 17 （값 어플리케이션 배포




                                                                                            敬盟區整？겋．n




    http://www.cyber.co.kr
                                                                            ,
                                                                                   I I II lilt ]]]
                                                                                7889   553192   of
                                                                                ISBN 978-89-키5-5키9그
