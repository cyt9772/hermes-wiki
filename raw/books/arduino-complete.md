---
source_url: /run/media/yutae/Data/아두이노 완전정복.pdf  # USB PDF (local-only; raw/books/arduino-complete.pdf gitignored)
ingested: 2026-11-07
sha256: eaca4a150ad45de5f967d9072cc61a24d58155b7f0c26dddc71239aba512a507
---

# 아두이노 완전정복 (raw source)

## Book metadata
- **Title:** 아두이노 완전정복
- **Authors:** 김경연 지음
- **Original:** —
- **Korean publisher:** 복두출판사 (JK전자, 2015)
- **Year (KR):** 2015
- **Pages:** 288 (pdfinfo)
- **kind:** text-layer (pdftotext -layout extraction 2026-11-07)
- **note:** cover page is OCR-garbled; body has text layer but carries some OCR artifacts, especially CJK/numerics. Cross-check against the local raw/books/arduino-complete.pdf for exact values.

## Full text (13318 lines)
                                                                                                   /
                                                                                              /
                                                                                     1d尸r
                                                                          //
                                                                ／戶
                                                           /
                                                 ／口




                                                                                              ［그
                                 h>                   \\
                                                                                                       /
                             H                                 m느m\

                                                                      \
                         /
                                                                                m\
                                                                                            ＼느m느




                                                                                                                                            hm놔
                                                                                                                                                              \
                                                                                                                                                  mH1




            心쇼四呻丑唯丹坦暐띱
                                                                                                                                                              二
                                                                                                                                                        뇨mh
        ／
    戶
戶
                                    N                                                                                                                   /

                                 可H1 0 o口口口I口口口口n1 1口口 口 口口 口 口 口i                                                                      /
                                 d
                                                                                                                                    /
                                      卜 自目目身 쿠 子 1 두", ,.," "                                                      /
                                                                                                                       /
                                                                                                                           /
                                                                                                                               /


                                         CSP2                    ,                                         /

                                          r써 nm <:7넛t) i.                  -j
                                                                                     日
                                          I I 蔽5 ArdUinD끼

                                                                                     蠱
                                                                                 小
小                                                                               小




                                      뇽         pa a 口口口口 a 口1




                                                                                                               \

                  \\                                                                                               \




                                                                                                                                   D, B.In化
  머리말



 Arduin아아두이노） 디바이스를 이용해서 자신만의 장난감, 원격 조종기. 로봇 등의
               여러 가지 홍미로운 프로젝트를 할 수 있다．


Chapter 1. 아두이노 시작하기에서는 아두이노 제품들의 종류와 사용법에 대해서 간단히 설명을
하고 Chapter 小9까지는 Arduino UNO R3 제품을 이용해서 아두이노 하드웨어와 함꺼］ 사용할
수 있는 많은 간단한 부품들과 센서, 확장 보드들의 자세한 사용법과 응용어］ 대해서 설명한다．
Chapter 10부터는 적외선 통신과, 지그비（z琯bee) 통신, 블루투스田luetooth) 통신을 이용해서 무
선으로 획득한 센서의 데이터를 전송하는 실험을 해보고 Chapter 12에서는 Arduino Ethernet
Shield 제품을 이용해서 아두이노를 인터넷에 연결하는 방법에 대해서 설명한다．


이 책의 집필 의도는 이런 멋진 기능을 구현하끼 위해서 복잡한 공학적인 내용을 셜명하려고 하는
것은 아니다. 때문어］ C언어에 대한 자세한 설명보다는 동작어］ 대한 기초 원리와 아두이노에서 어
떻게 이것을 활용할 수 있는가어］ 초점을 맞추었다．


공학을 전공하지 않아도 C/C+＋을 모르는 사람도 아두이노 IDE 프로그램과 아두이노 하드웨어만
갖춘다면 간단한 실습을 통해서 누구나 쉽거］ 아두이노 하드웨어들과 외부 세꼐를 연결해 주는 다
양한 센서들의 사용법을 익힐 수 있도록 하는 것（:)] 목표이다. 스커伏］ 코드에서 사용된 C/C++ 언
어에 대해서 완전하께 그리고 자세히 알고 싶은 독자는 시중어］ 넘쳐나는 C/C++ 문법관련 도서나
웹 사이트를 통해서 얼마든지 알아갈 수 있다．


물론 이미 시중에는 이러한 비슷한 형식을 갖추고 출간되어 있는 많은 아두이노 책들이 나와 있다．
거끼에는 번역서도 있고 국내 저자들에 의해서 집필된 도서도 있다. 필자도 번역서와 국내 서적들
을 여러 권 읽어 보았다. 이미 발간된 몇 권의 책을 읽어 보면서 많이 아쉬웠던 부분이 있었는더］,
그것은 아두이노 기본 하드웨어를 제외하고 책에서 실습어］ 사용되어진 다양한 센서들콰 입／출력



                                                          머리말 1 3
  장치들의 실험 재료들을 구하기가 어려워서 직접 실험을 해볼 수가 없기 때문어］ 책의 내용을 완벽
  하케 이해하는떼 한켸가 있었다는 것이다. 특히 외국 번역서들은 실험 재료들을 구할 수 있는 온
  라인 URL을 제공하지만 모두가 해외 구매처여서 국내 사용자들이 직접 구매하기는 쉽지 않았고
  국내 서적들도 실험 재료를 구매하거나 구할 수 있는 자료가 많지는 않았다．


  이 책은 집필할 때부터 교재에 사용된 모든 실험 세트들을 같이 제공하기 위해서 저렴하고 구매하
  기 쉬운 재료들을 사용하였고 본 교재에서 사默크 모든 실험 재료들을 갖춘 통합 개발키트도 같이
  판매하고 있다. 통합 개빌키트는 ht加:/／砥叭w.deviceshop.net에서 쉽거］ 구매할 수 있다. 또한 실험
  어］ 사용된 개별 재료로도 구매 가능하다．


  시간이 된다면 이 교재의 후속편으로 아두이노 응용 기술들을 다루는 조금 더 난이도가 있는 응용
  프루그램들어］ 대한 내용을 집필해 보고 싶다. 특히나 최근어］ 가격이 많이 내린 3D 프린터를 이용
  하여 아두이노 보드와 3D프린터로 출력한 끼구물들을 이용하여 실제 움직이는 RC 자동차, 쿼드콥
  터, 탱크와 갇은 제품의 Pro切tT祀을 해보고 싶다．

                                                     2015년 2월 저자 씀




     이 교재에서 사용한 모든 스케치 코드는 네이버카페 또는 JK전자 홈페이지에서 모두 다운로드
     받을 수 있고 모든 부품 또한 구매가 가능하다．


     口 JK전자 홈페이지 (http://www.jkelec.co.kr)
       JK전자 홈페이지 또는 온라인 쇼핑몰 디바이스십曲卄p://ww.dev匕esho口.net)을 통해서 이
       과卄에서 사용한 모든 부품들을 개별로 구매하거나 패키지 제품으로도 구매가 가능하다. 이
       교재에서 사용하는 모든 부품들에 대한 자서환 리스트는 부록에서 모두 확인할 수 있다．


      口 이 교재의 사후지원 카페伯tt口：//ca旭.naver.com/avr없U如）
       네이버카페를 통해서 이 ji仄Ii에 대한 문의사항이나 추가 요청사항들을 게시판을 통해서 지원
       하고 있고 또한 이 -I끄卄의 잘못된 사항에 대한 내용도 카퍼를 통해서 업데이트 하도록 할
       것이다．




4 1 아두이노 완전정복
Chapter


01        아두이도조깨小m＝小
          ] 1 아두이노（Ard네n이란7                 10
          1.2 아두이노 개별환경                     12
          1.3 Arduino UNO R3로 시작하기          14



Chapter


02        전기, 전자의 기초
          2. ]   전류와 전압                     32
          2.2    저항                         33
          2.3    LED                        36
          2.4    브래드보드 사용법                  38
          2.5    엔지니어링 공구                   41
          2.6    테스터기 사용법                   42



Chapter


03        디지털 입력과 출력
          3. ]   디지털 출력이란?                  48
          3.2    LED 깜박이기                   49
          3.3    7 세그먼트 구동하기                53
          3.4    버튼을 이용하여 스케치 없이 LED 제어하기   61
          3.5    버튼을 이용하여 LED 제어하기          63
          3.6    버튼을 이용하여 LED 상태 제어하기       67
          3.7    부저（Buzzer) 울리기             69



                                                 차례 1 5
      Chapter


     04         시리얼（RS232) 통신
                4. ] 시리얼（RS232) 통신 소개                     74
                4.2 PC와 시리얼（RS232) 통신하기                   76
                4.3 시리얼（RS232) 통신으로 LED 제어하71             79



      Chapter


     05                           력
                5. ] 펄스（Pw卜川로 LED 밝기 조절하기                  86
                5.2 펄스（Pw卜川로 부저（Buzzer) 연주하기               92
                5.3 가변저항 값 읽어오기                            97
                5.4 테스터기 흉내 4 전압 값 읽기                     102



      Chapter


      06        LCD 사용하기
                6. ] 패러럴 L（力 디스플레이（4七仕 모드）                108
                6.2 패러럴 L（力 디스플레이侶七it 모드）                 113
                6.3 시리얼 L（力 디스플레이                         117



      Chapter

      07
                7. ]   센서 소개                              122
                7.2    밝기 감지하71 - CDS 조도센서                122
                7.3    온도, 습도 감지하71 - DHT1] 온습도 센서        126
                7.4    화재 감지하기 1 화염감지 센서                  133
                7.5    기울기(Tilt) 감지하71 - SW-520D 기울기 센서   137
                7.6    진동 감지하기 = SW-18020D 진동 센서          142
                7.7    장애물과의 거리 감지하기 1 초음파센서              146




61 아두이노 완전정복
      Chapter


         8
                 81 소형 D（二 모터 사용하기                                                154
                 8.2 서보모터 제어하기                                                    160
                 8.3 스테핑 모터                                                       163


      Chapter


         9       디지털 통신 인터페이스
                9. ]     디지털 통신 인터페이스 개요                                          ]72
                9.2      12（二 통신 규약                                               ]72
                9.3      12C 통신으로 자이로 센서 사용하기 L3G4200D                            174
                9.4      SI기 통신 규약                                                ]82
                9.5      SI기 통신으로 자이로 센서 사용하기 - 匕3G4200D                          183
                9.6      자이로 센서로 서보모터 제어하기                                        ]90



      Chapter


10
                10. ] 적외선 수신하기                                                    198
                10.2 적외선 송신하기                                                     207




                ]] . ]   지그비（기gbee）란7                                             212
                11.2     지그비口gbee) 통신 테스트                                         213
                11.3     아두이노 지그비口gbee) 통신                                        221
                11.4     특청 XBee에만 통신하71                                          230



Chapter
                                         둔群我拉聽翼的我鴦甘箕큭姓曲羽在曲코斗南器拉世挺融丘升布8큐聲照怒羅是碼蜘恥



'12
                블루투스
                12. ] 블루투스 통신                                                     238
                12.2 안드로이드 스마트 폰으로 LED 제어하기                                       239




                                                                                        차례 1 7
      Chapter


     13         이더넷（Ethernet) 네트워킹
                13.1    이더넷（Ethernet）이란？            248
                13.2    Ard내no Ethernet Shield 소개   248
                13.3    웹 클라이언트（고정 IP)              249
                13.4    웹 브라우저로 아두이노 LED 제어하기       255



      Chapter


     14         사물인터넷이란？
                14. ]   사물인터넷이란 무엇인7口               264
                14.2    사물인터넷 주요 서비스                266
                14.3    주요 loT 제품 및 서비스 동향          268
                14.4    주요 loT 구성요소 및 현황            270
                14.5 가전, IT 기업들의 사물인터넷 플랫폼 주도 현황    271



      Chapter


     15         스마트홈
                15.1 스마트홈 서비스 개요                    274
                15.2 스마트홈 서비스 종류                    274



      Appen비x


       A        부록 및 색인
                이 교재어써 사용한 모든 부품 리스트                278
                찾아보기                                281




81 아두이노 완전정복
아두이노 소개

 ] . ] 아두이노（Arduin이란7
 1.2 아두이노 개발환경
 1.3 Arduino UNO R3로 시작하기
  小 A固내no e




      1.   1   아두이노（Ard내no）란7


   · 아두이노는 이탈리아 회사伯却力＼자ww.arduino.cc）에서 처음으로 개발되었고 AVR 기반
   의 마이크로컨트롤러 하드웨어와 소프트웨어 개발을 쉽게 해주는 개발환경(IDE）을 합쳐서
   아두이노라고 한다．
     아두이노 추立드웨어는 무료이고，오픈소스, cross-pi缸on可리눅스, Win面＼vs, 八'JAG (万
   등）을 지원한다. 하드웨어 디자인 또한 모두 공개되어 있는 오프 소스이다. 필자의 생각에
   이렇게 무료로 공개된 개발환경과 하드웨어 플랫폼을 기반으로 전 세계적으로 제작된 아두
   이노와 호환되는 수많은 하드웨어 자원들（센서 , 네트워크, 입출력 장치 등）, 이 자원들을
   쉽게 활용할 수 있도록 제작된 오픈된 소프트웨어 코드들（Sketch）과 아두이노에 흥미를
   가지고 있는 사람들의 수많은 커뮤니티들이 진정한 아두이노의 파워라고 할 수 있다.
     아두이노 환경은 전문적인 소프트웨어 혹은 하드웨어 엔지니어를 위해서 설계된 것은
   아니지만 뭔가 새로운 것을 만들고 싶고, 창의적인 아이디어는 있으나 공학에 대한 지식이
   부족한 사람들이 쉽게 이해하고 저렴한 가격에 하드웨어를 갖추어서 프로토타이핑을 하고
   싶다면 아두이노를 선택하라. 아두이노가 대단하다고 생각되는 것이 초보짜를 위해서 설계
   된 환경이지만 기초적인 일들만 할 수 있는 것이 아니라 아두이노 개발환경과 몇 가지
   하드웨어만 갖춘다면 다음과 같은 다양한 일들을 할 수 있다．



      H 모터제어를 통한 기초 로봇
      H 음악, 사운드 장치
      H 온도, 습도, 화염, 기울기 등 다양한 센서 인터페이스
      H 게임 분야 등
           유선, 무선 네트워크 시스템



     이러한 이유로 아두이노 플랫폼은 전 세계에 많은 사용자들을 확보하고 있고 현재 에도
   계속해서 발전해 나가고 있다．




10 I 제］장 아두이노 소개1
아두이노 소프트웨어                                                        .
  아두이노 소프트웨어는 공학을 전공한 사람에게는 좀 특이하게 생각되겠지만 "Sketch"
라는 용어를 사용하고 아두이노 통합개발환경 Integrated Development Environment(IDE)
 에서 코드를 작성할 수 있다. 아두이노 IDE 환경에서 작성되어친 추入쿠亡（Sketch）는 바로
IDE 환경에서 컴파일하고 아두이노 하드웨어（Arduino UNO R3, Leonardo 등）에 바로
업로드 할 수 있다. 원래 아두이노 하드웨어에서 사용하는 AVR 기반의 마이크로컨트롤러
들은 ISP라는 프로그램 장비가 별도로 있어야 하지만 아두이노에서는 II犯환경에서 별도의
추가 장비 없이 프로그램을 아두이노 하드웨어에 업로드 할 수 있다. 이러한 기능이 가능한
이유는 아두이노 하드웨어 CPU어］ 이미 ISP기능을 하는 Bootloader 라는 프로그램이 존재
하고 있기 때문이다．


아두이노 하드웨어

  아두이노 ID可개발환경）에서 작성한 코드를 업로드해서 실행할 수 있는 AVR CPu 기반
의 실제 타깃 보드이다. 아두이노 하드웨어에는 단순하지만 수십여 가지의 센서들, LCD,
모터 , 네트워크 등 쉴드라고 일컬어지는 모듈들을 연결하여 확장이 가능하다. 아두이노
하드웨어는 이탈리아의 아두이노사에서 정식으로 판매하는 제품들이 있고 전 세계적으로
아두이노와 호환하는 제품을 생산하는 수많은 Third Party들이 있다．
  어쨌든 아두이노를 처음 시작한다면 가장 인기 있는 하드웨어 제품인 Arduino UNO
R3(2013년 현재） 제품으로 시작하는 것이 좋다. Arduino I介JOR3는 아두이노 하드웨어
중에서 전 세계적으로 가장 많이 사용되는 하드웨어이고 바로 다운받아서 실행해볼 수
있는 수많은 재미있는 예제 리소스들이 존재하기 때문이다. 만약 아두이노 환경에 익숙하
고 좀 더 많은 확장을 원한다면 Aitluino 八4e甲 2560R3（최대 속도 16MHz) 제품을 사용하면
되고 최근에는 ARM 기반의 고성능 CPU를 기반으로 하는 Arduino DUE（최대 속도 84MH기
제품도 출시되었다. 아래 URL들은 아두이노 하드웨어를 자세히 소개하고 있는 사이트와
온라인에서 바로 구매가 가능한 사이트들을 나열하였다．


寸－ 아두이노 0川C洌 board
       http://www.arduino.cc/en/Main/Hardware


H- 아두이노 Corn口atible board
       htltp://지入／w. devicesho


                                                ]. ]   아두이노（Ard내n아란？ I 11
  .   Arduino



                  http://www.toolparts.co.kr



      小 Online guides 幻r ge川ng 없arted
                  http://arduino. cc/en/Guide/Windows : for Windows




            1.2        아두이노 개발환경


        여타 다른 마이크쿠 立 쿠세서 개발환경과 다르게 아두이노는 개발환경 S/＼刃부터 아두이
      노 H/W 모두를 오픈소스로 진행하고 있고 개발환경도 무료로 누구나 다운벋아서 사용이
      가능하다. 전 세계의 많은 사람들이 아두이노를 사랑하는 이유에 아마도 이 부분도 큰
      몫을 했을 것이다. 이 책을 읽는 독자 분들 중에 아두이노 이외의 다른 마이크쿠立쿠세서를
      사용해본 독자 분들이 계시다면 Al小4 Proi：邸or 계열의 개발 장비와 컴파일러 개발 환경이
      수천만원이 넘는다는 사실을 알 수도 있을 것이다．


      아두이노 통합개발환경(IDE) 다운로드

        아두이노 통합개발환경 소프트웨어를 h却://ardujno.cc/en/Main/鈿血ware에서 다운로
      드 받을 수 있다．


       Down 'oad                                                 Next steps
       Ar小ilno 1.0.5 (rel쁘뜨竺n｛쁘多）j玉比心ted陟 Google Code:           G世ng Started
                                                                 Reference
        +    w노面ws Insta血r, 砥枷面砥s (ZIP file)
                                                                 Environment
        +    MacOSX
                                                                 血51꺄kS
             Li끄ux: }1 b喀 64
                                                                 Foundations
        ++   source
                                                                 FAQ



      ｛加밖noad Arduino 1. 5 BETA 佃ith supp口Ft for Arduino Due 加及rd)

      if 卯uh괴肥 the new Due 且坦rd卯u must面硼riload the 工．S그 var虹on. Once you get 血e software 如如w t由 岫tml函｝n
      幻 get started wi血 the Aid川no 沁e.

                               ［그림 卜1]     아두이노 IDE 소프트워뻐 다운로드 화면




12 I 제1장 아두이노 소개1
 Linux, 入lac羽 X, Linux용 모두 있지만 우리는 싸indows 환경에서 아두이노를 사용할
것이기 때문에 Windows(ZIP file）용을 다운로드 받는다. 2013년 2월경에는 아두이노 소프
트웨어 버전이 1.0.3이었는데 책을 집필하고 있는 현재 2013.8월에는 벌써 1.0.5가 올라와
있다. 그리고 Al小4기반의 Arduino DUE를 사용하기 위해서는 현재에는 1.5 B町A 버전을
사용해야 한다. 이후에는 버전이 어떻게 바뀔지 모르지만 가장 최신 버전의 개발 환경을
유지하기 위해서는 http://arduino.cc／어］ 자주 방문하여 확인하는 것이 좋다. 아두이노 IDE
실행파일 이외에도 추入극7亡도 같이 다운받아서 분석해볼 수 있다．


아두이노 통합개발환경(IDE) 설치

 아두이노 통합개발환경은 w血面＼vs Installer 버천도 있고 설치 과정 없이 압축만 해제하
면 바로 실행 가능한 버전도 이다. 우리는 珌indows(ZIP file) 형태의 파일을 다운받을
것이다. 다운받은 프로그램은 별도의 설치 과정이 필요 없이 다운받은 ZI') 파일을 단순히
압축을 해제해서 사용하면 된다. 필자의 경우 "C:/Arduin아1.0.5" 어］ 압축 해제하여 설치를
하였다. 물론 ' C:/Arduino-1.0.5 " 폴더 이외의 다른 위치에 설치를 해도 문제가 되지는
않는다．
 설치가 완료되었으면 "arduino.exe" 프로그램을 실행해보자. 참고로 "Arduin아1.0.5" 의
"1.0.5"은 아두이노 프로그램의 버전이다. 다운받은 버전에 따라서 달라질 수 있다．
arduino.exe 파일을 더블클릭해서 실행을 하면 아래와 같이 스플래시 화면과 함께 실행이
된다．


          轟 java                                   2013-10-23 오享     파멀 폴더
         案 匪｝
         套 Iibr
         嘉 refer
         求 tc耐
         的耐U
         匯江ygi     ARDU工NO
          器．
         珏］ rev佑                                                         口   /
         邕 1XtX    사寸 OPEN PF心茫CT 닙RI丁TEN. OEBUO또D 사내［) SR口的町드U
                   B\ 阡及SE工卜mBNU. B丹玎B C1JABTIELLES       1마d 끄：0E
                   G1ANLUCA 卜1AR] 1京） A I, BA町끄 卜IELLIS



                   BASED (1R 帥0CESSIN口 ET CASEY 目EAS #ND B日니 FRY




        [그림 1-2] Arduino splash screen (version 1.0.5 in Windows 7)


                                                                                 1.2 아두이노 개발환경 1 13
  .   Arduino .-                                                     니




       아래 그림은 아두이노 프로그램을 실행했을 때 처음으로 나타나는 개발환경에서의 빈
      Sketch 화면이다．




                     ［그림 卜3] 아두이노 IDE (version 1.0.5 in Windows 7)


      1 아두이노 설치 관련 Troublesho아ing
              http://arduino.cc/en/Guidei1"roub1eshooting




      口m Arduino UNO R3로 시직后I.기

       Arduino I介JOR3는 아두이노를 처음 시작할 때 가장 많이 사용되는 하드웨어로 앞으로
      진행되는 대부분의 예제 실습들은 Arduino UNO R3 하드웨어를 가지고 진행이 될 것이다．
      물론 네트워크 실습에서는 Arduino Ethernet Shield를 추가로 확장해서 사용할 것이다．




14 I 제］장 아두이노 소개
                                                                                                                                            多
［표. Arduino UNO R3 하드웨어 사양］
 Microcontroller                       ATmega328
 0perating Voltage                     5V
 Input Voltage                         7-12V Recommended
 Digital I/O Pins                      14 (of which 6 provide P聊4 output)
 Analog Input Pins                     6
 DC Current per I/O Pin                40 mA
 Flash Memory                          32 KB
 SRAM                                  2 KB (ATmega328)
 BEPROM                                1 KB (ATmega328)
 Clock Speed                 1m        16 MHz



 Flash 八4em아y 용량만큼 아두이노 코드（Sketch）를 작성하고 업로드 해서 실행 시킬 수
있고 32KB 중에서 0.5KB는 부트로더에서 이미 사용하고 있기 때문어］ 실제로는 31.5KB
만큼의 Sketch를 작성할 수 있다．



                     k 씨k
                                                                                      指                                         作
                                                                         詐n叫n
                                                                                          m
                                                                                          r
                                                        4띠4 <
                                                                                 NH                  r\ 口 I'.. 寸 m 씨
                                                   H
                                                                                              m
                                                                                                         I I     t
                                               i
                              HH
                               n
                                                                                                     DIGITAl. (PIH- )
                                                                L
                                                                                      A                           0
                                                                                      00 :UN

                                                                                                                                    e씨N스如
                                  N生
                                           님
                                                                                                                           =
                                                                                                                           1
                                                                                                                           r1
                                                                                                                       什
                                                                                                                                에
                                                       : mm口 'ARDUINO
                                                                        bm                                         1
                                                                                                                   n



                                                                                                                           =H
                                                                                                                  n
                                                                                          h   才 =WV *ROUXV口 L (   M             1




                                       月 H툐
                                       t
                                                                    1
                                                                             1 뇨告日
                                                                                              I, m
                                                                                                  忿
                                       i
                                                                令
                            ［그림 卜4] Arduino UNO R3 사진




                                                                                                           1.3 Arduin（그 UNO R3로 시작하기 ! 15
 -. Arduino .-如山



   Ard내no UNO R3 하드웨어 구성



               Reset S/W


               USB
          Connector




                12V DC }
        Power Connector



                           ［그림 卜5]    Arduino UN0 R3 하드웨어 구성


     아두이노 하드웨어에 관심이 있는 독자라면 아래 U]毗에서 Ba뎀e, PDF 포맷의 회로도를
   다운로드 받을 수도 있다．


   永 /\rudino UNO R3 PDF 회로도
           h띠://www.jkelec.co.kr/arduino/uno-r3/Arduino_Uno Rev3-sChematiC[11.pdf
           http://arduino. CC/en/uploads/Main/Arduino_Uno_Rev3-sChematiC.pdf


     Arduino UNO R3 뿐만이 아니라 아두이노사에서 릴리즈한 모튼 하드웨어 회로도와
   Eagle 포맷의 PCB 데이터가 공개되어 있다．




       아두이노사에서 공개한 Eagle PCB 파일이 있으면 Eagle 프로그램에서 Gerber 포맷의 파일을
     추출하여 PCB 제조업체에 넘겨서 PCB 제작을 맡기면 아두이노 PCB를 만들 수 있다. 물론
     PCB만 있다고 해서 아두이노 보드를 만들 수 있는 것은 아니다. 비어있는 PCB 제품에
     ATMEGA328 CPU와 부 품들 을 납땜을 하면 나만의 아두이노 보드를 완성 할 수 있다. 부 품 을
     모두 올린 이후에 아두이노 부트로더 파일을 ATMEGA328 CPU어］ 업로드를 하면 아두이노 하드
      웨어가 완성된다. 필자도 아두이노 PCB에 직접 부 품들 을 손으로 납땜을 해봤지만 쉬운 작업은
     아니다.




16 I 제］장 아두이노 소개
Arduino UNO R3 전원공급

  Arduino UNO R3에 전원을 공급하기 위한 방법은 2가지가 있다. USB 케이블（Ato
B형）을 이용하여 PC와 Arduino UNO R3의 USB Socket어］ 연결하거나 Arduino UNO R3의
DC Socket어］卜12V DC Adapter（외경 : 5.5mm, 내경 : 2.1mm)를 연결하면 된다. 물론
아두이노 正）E（개발환경）에서 프로그램을 수정해서 Arduino 爪OR3 어］ 프로그램을 업로드
하려면 반드시 USB를 통해서 PC와 연결이 되어 있어야 한다.




                 ［그림 卜6] Arduino UNO R3 전원 연결


PC와 연결확인

 Arduino UNO R3 제품을 USB 케이블을 이용하여 PC와 연결을 하고 USB장치 드라이버
가 정상적으로 설치 완료되었다면 아래 그림과 같이 윈도PC의 장치 관리자에 "Arduino
Uno(COM9) " 포트가 올라와 있는 것을 볼 수 있다. "CO八49"의 "9"은 사용자의 PC마다
다른 번호로 나타날 수 있고 같은 PC라 할지라도 어떤 USB포트에 연결했는가에 따라서
번호가 달라질 수 있다．




                                          1.3 Arduino UNO R3로 시작하기 1 17
m+ 샤d내no 1




                      파얹（日 듐짝的     보기（田        도뮴맏0出

                       4 1 力圃［引 目圃 求키 陪
                  盒 컴퓨E1 관리（로켤）                          부 USB Compov在e Device
                  J a1 시스댐 도구                            乍 USR Corn刃5仕eDevice
                     【， (9 작업 스斗줄러                 1     弓 USB Root Hub
                        咽 이벤트 뷰어                         甘 USB R（刃t 卜-lub
                        必 공유 폴더                          甘 USB S目ial Converter
                        辯 로걸 사용자 맞 그吾                    투 USB Sen키Connecter
                        匈 성농                          自 사운드．텍디오 및 걔임 컨트I러
                        a 장치 관리자                    , 寸m 시스템 쟘치
                   d 毖 저잠소                         「， 奄 이미징 장지
                        打 디스크 관리                    」 i作 컴퓨터
                     큽：1 서비스 및 뮴용 프로그탬             !, 占 키보드
                                                   d 多工 보트（COM & 四7)
                                                         莎A喚Ii叩U匣壑垂曳
                                                         牙1US8 Serial Port(C（別7)
                                                         '平 USB Serial Polt(COM8)
                                                       日 프로I서
                                                               n1 ra =1 1\1 八   t1
                                                               ci               J

              뇨
                  H                =




                       ［그림 卜7] Arduino UNO R3와 Windows7 PC와 연결




     Wind叭vs 환경에서 장치관리자를 실행하는 방법은 실행메뉴（Windows+R）에서 dew끄암砒.msc를
     입력한 후 Enter를 누르면 된다．




     아두이노 USB 드라이버가 정상적으로 설치되었다면 위 그림과 같이 장치관리자에
   "Arduino Uno" 시리얼 포트가 올라오지만 Windows7 PC의 경우 아래 그림과 같이 USB
   드라이버가 인식이 되지 않아서 "알 수 없는 장치 "로 설치되는 경우가 있다．

                                                                                            1=
                           관리

                      팍社侄） 듕직（A)       보기（V)   도욤콸（H)

                      乍斗！乞圃！目圃 必
                                                        1kykim_ttrinkpad
                                                         08山煎刃th 숑수신 장지
                                                        1笛 DVD/CD求OM 드라미브
                                                                                     E十착멉
                                                         됴才 IDE AWATAPI 컨트룐러
                                                        型 Jungo
                                                        好 SM Driver

                          斗 孕지 관리자
                       d 好 저장소
                          甘 디스크 관리                     :) LJ 디스크 드라이브
                       口 邑 서텍스 및 용용 프로그탬               1 푸 디스퓰斗이 어댐턱
                                                       : 8 과우스 및 기Ef 포민띰 장지
                                                       :, 毒 모니터
                                                       :, 斗 배턱리
                                                       J무 범용 직匹 버스 컨트I러
                                                        ) ＝무 Generic USB H比
                                                       . .!1L）夕＝i




              ［그림 卜8] Windows7 PC에서 USB 연결이 잘 되지 않는 경우


18 I 제］장 아두이노 소7Q
  이러한 경우에는 수동으로 장치 드라이버를 업데이트 해주어야 한다．


         如現題
          파앝（日   듕작（.4   보기（너   도큠맏(H)
         巾 씨 力圃 日！型圃 必 i ;r '\ !!J
                                    心 回녑m가inkpad
                                    L, 心1 미此tooth 슘수신 장지
                                                             잠지 관리자
                                    卜곱 DVD/C口的M 드라이므
                                    D 14IDE 사NATAPI 컨트룔라        긔 드r 작업
                                    >f iungo
                                      .j SM Driver




                                                   ; 안

                                    :：絮裁         琫거（U)
                                    小橡 모L凋         하드寐이 변겋 사황 검색（A)
                                    小斗 빼터쾨
                                    Jj 범，용작르       속셤｛R}
                                       쿠 Uerlerrrt巧gm可


         선택한 장착0量 댜짜 ［드라하텍 소프트打어 업데이트 마법사］i      A！작험니다


             ［그림 卜9] Windows7 PC에서 USB 장치 업데이트


 장치 관리자에서 "알 수 없는 장치" 어］ 마우스 오른쪽 버튼을 클릭하면 "드라이버 소프트
웨어 업데이트" 명령을 수행할 수 있다．




            드라이버 소프트웨어는 어떻겨1 검색합니까？



             +   업데이트된 드라이버 소프트웨어 자동으로 검색（S)
                 컴퓨터와 인터넷에셔 장지01 璘한 최신 드라미텍 소프트籌어를 컴색함니다‘ 이套
                 7至 하지 않므려 면 장자 설자 설졀0弘4 0j 기능률 사용하지 많도록 설징혜야 會나
                 {：之



             斗 컴퓨터a和4 드라이버 소프트웨머 찾아보가承｝
               수동으로 드라미뻐 소프툐贇꺼믈 찾아 설지하십시오




           ［그림 卜］0] Windows7 PC에서 USB 장치 업데이트


 드라이버 소프트웨어 업데이트 창이 나오면 위의 그림처럼 "컴퓨터에서 드라이버 소프트
웨어 찾아보기（R) "을 선택한다．

                                                                 1.3 ,Ard내no UNO R3로 시작하기 1 19
.   Arduino .



                   r플긔찾.「보：               聲＋窄粉好’「，                                  唾꾀

                   1{
                   11
                          E   H岫小               “'   " 「「 “ ""
                                                           '
                                                                 j-   '"F   "AI2.
                          =U｝탐화면                                                    4

                          b諍라（}！브러리
                          > 烈 ky녑m
                          d4 컴퓨E4
                           11 로켤 디스크R깁                                              『




                 i匕二1111d1
                              D 上 켜d1血好1쇼3


                   1 11                                                             녀! I
                                                                                        :i
                              4 土 帥由jino-t (巧
                               J # 出i帑도
                                 b出F兀I
                                          USB머V目S
                      1        口拉 Exam目ES
                      1        I'必 mf小vVre
                               D出肛a
                               b士 lb
                      1        1' 上 枷却ES
                      1        b出 m佃xnce

                      1 : "，十亡쓰．                                                    f



                   ［그림 卜11] Windows7 PC어因 USB 장치 업데이트


      그리고 장치 드라이버가 있는 폴더의 위치를 아두이노 IDE 개발환경이 설치된 폴더
    "C: \arduino-1.0.5\drivers"를 선택한다．




                    ［그림 卜］21 Windows7 PC에서 USB 징以1 업데이트


      드라이버 위치를 선택했으면 "다음"으로 진행한다．



201 제］장 아두이노 소7卄
           이룡；Ard내no US8 Dr卜／之r
           게시Xh Ard山no LIC


                                                               다윰 잠지의 드라이버 소프트웨머 설치츨 뫈료혔습나q
   r    "Ar(如no UC' 의 소프트왝어는 함삼 신뢰（A)


   口    신뢰할 수 있뇬 I시자의 드라이버 소프트異어만 설치혜야 함나C
        흐F 차工 쏘三트왁어를 多裝햐느二 박볍




                        ［그림 卜］3] Windows7 PC어Ikf USB 장치 업데이트


아두이노 USB 장치드라이버가 성공적으로 설치된 화면이다．


       雀컴퓨4二叫小m=                                                         芬弗1毛晶屯뇨 느回心늬
       g蜀描茹哉뇨屯                                                                                                     目
         努 컴퓨터 관리（로켤）
          4 豁 시스뎀 도구
       重：   > 臼 작업 스斗줄러
       旨    b 圓 이볜트뷰머                                                                                               三

   量   b 莉 공유 폴뎌                                                                                                   主｝
   量   L, 毋 로켤 사용자 맞 그룹                                                                                            菖
   重   r》 匈 섬늠                                                                                                     旨
   量      世 잠치 관릭자
   量 a 毖 저장소
                                                                                                                   ！三
                                                                                                                   三；


                                                                                                                   量
   '      甘 디스크관리
     ) 昆 서！하스 및 뮴용 프로그램


                                          1    a ·fi于 포트（OM & (PT)

                                                                                            비i
                                          區I
                                                                                                                   1
                                               ! 沁望츠塑包쁘브凹嶝｝M璽
                                                                                                                   弓
                                          1    ! ｝『里出旴ena甲毗COM7)                             割
                                          1
                                          I
                                               i；甲 냐SB Sen引P0八（COM8)                        녀1
                                               -      프로Al大i                                寸 1
                                          r乞“ b中工驛瑥立君 '                                 ,     1
                                                                                                                   ii
            느：              韶      山1口四        口m1尸                  !              山             山／   注   r 臣1m   /


                  ［그림 卜14] Windows7 PC에서 USB 장치 업데이트 완료




                                                                                   1.3 Ard내no UNO R3로 시작하71 1 21
 1        A心내no .




     아두이노 보드에 맞는 IDE 환경 설정

           사용하는 아두이노 보드에 따라서 아두이노 II犯환경에서 설정을 해주어야 한다. 우리는
     Arduino UNO R3를 사용할 것이기 때문어］ 메뉴에서 "도구／보드／Arduino UNO"를 선택한
     다．
                                                                                  사duino inn
                                                                                  Arduirco Duemilanove W/ ATmega328
                                         자돔 포맷                Ctrl.T              Arduino Diecimila or Duenlilanove WI ATrnegal68
                                         스程치 보관하기                                 Arc抽no Nano ＼甘／ 사mega32s
                    sketch oct23e
                                         인코딤 수정 & 새로 고침                           Arduino Nano W/ ATmegal68
                                         시리멀 모니터              Ctrl+Shi什＋M         Arduino Mega 2560 or Mega 40K

                                         보드                                       Ard山no Mega (ATmega1280)
                                                                                  Arduino Leonardo
                                                                                   Arduino Esplora
                                                                                   Arduino 뻬cm0
                                                                                  4rduino Mini W/ ATmega328
                                                                                   Arduino Mini WI ATmepa168
                                                                                  酊duino Ethernet


                                              ［그림 卜］5]                 Ard네no 보드 설정



      스케치 불러오71

           아두이노를 처음으로 사용해 본다면 아두이노 IDE 환경에서 기본으로 제공하는 스케치
      부터 불러와서 테스트를 해보도록 하자. 친절하게도 아두이노 IDE를 설치하면 간단하게
      아두이노 보드를 테스트 해볼 수 있는 몇 가지 예제를 기본으로 제공하고 있다. 메뉴에서
          "파일／예제／01.Basics/Blink" 를 선택한다．

                                                                           F   OlBasics                 AnalogReadlerial
                                                                                                  卜
                                                 趙   1요罫                       02.0回t키                  EareMinimumn
                                                                               03;Analog          卜     Elink
                                     社寸소升처쯔靈字；


                                                           烈
                                                                               （놔Communication 卜        D呵t計如adlenial
                                                                               05.Contr이                Fade
                                                                               06tensors                ReadAn찌ogV비tage
                                                                               07.0따놔ay

                                                           Ct＋넥                08.Strings
                                    닫기
                                                           Ctrl+S              09.USB
                                    저잗
                                                                               lOst카怡rKit
                                    다론 이콥으로 저琶             Ctrl+5hift- S
                                                                               Ard바naIl!'
                                    업로드                    Ctrl+U
                                    프로그릭田1휼 이용해 업로드 CtrkSh洑놔J                  EEPE（가너
                                                                               Es!加ma
                                    패이지 설정                 Ct卄＋Shift+P
                                                                               Ethernet
                                    민솨                     Ctrl.P
                                                                               듸rmata
                                                           Ctrl+Cornma         GSM

                                    종료                                         LlquidCrystal
                                                           C出＋Q


                                          ［그림 卜16]               Arduino 스커因 불러오기




22 I 제］장 아두이노 소개1
  새로운 아두이노 스케치 창이 열리고 아래 그림과 같은 스케치를 불러온다．


               命帥k 햐드이노二0.5 ；』／                             m,
                                                                     ,1: 1發尋學＝I
               파일 편집 스神치 도구 도뮴닫                  口小              1   11   :1    1                큠
               n小 m朴n                                                                            冒



                                                                                                 I
           /
                 This e emple c。
                幻／,
                       ,,
                       』．
                               de Is in the pt I ic   d。
                                                           raein,                                1
                                                                                                 I



                                                                                                 1
               void setop
                 /1 initiel()ize the digital pines en 。utput.




          4」                                                              Arth,ino Uno on COMI


                            ［그림 卜17]           Arduino 스케치 불러오기


불러온 Blink 스케치의 실제 위치는


         "C:\arduino-1 .O.5\examples\01 .Basics\BIink\BIink.ino"


어］ 위치하고 있고 Windows7 (芬에서 파일의 속성을 보면 Arduino Source Code(.in이 파일
로 arduino exe와 연결되어 있는 것을 알 수 있다. 아두이노에서 제공하는 기본 스케치
파일들의 위치는 아두이노 IDE프로그램을 어떤 경로에 설치했는지에 따라서 달라진다．
본 교재에서는 설치 위치를 "C:\arduin아1.0.5"어］ 했기 때문에 위와 같은 경로에 기본 스케치
예제들이 위치한다．



                                                                               1.3 Arduino UNO R3로 시작하기 I 23
  .   Arduino .



                        '「’多궁linkin.속甘多 뇨拙嫡蝴恥＃甘11                                                                                  山1
                            일반 ！虹丁 8nb匣耳團                                                                                                            !
                                                                                                                                                     1
                                   蟲
                                   mm규
                                                         Blink. i加                                                                                   11
                                   파밀형식：                            Arduin。S。
                                                                            urce C。
                                                                                  deCin。
                                                                                       )                                                             1
                         }         면겊프로그램：                      的arduino,                 axe                        변召（됴） 卜            m            j
                        重 크:'i                                                                                                                       1
                         重         위치：                          C:Ward네no니且5Wexam미enWOl,日a引csWBlir
                                                                기0바미트（7104日트）
                         重         디스크할당크7卜                        4,00KB (4，啼바미트）                                                                   1
                         蛋                                                                                                                           1
                         筐         만든낟쨔                            201于크 10현 23잎 오느. 2시간11

                        旨 수정한납쨔 20仔크5훨 1砬금요멀                                                                 오華10:26:16

                        量 액세스한날恥 2013년I0쵭23밉오느 2시칸젼                                                                                                  了
                                                                                                         .



                                                                                                     .

                         案                                                                                                                           {

                        1重 특성 二j留21酉實（匪 團合깁（b)     r 고급（므）                                                                                           1

                    I                                                                                                                                1
                                                                                                                                  ，二1
                         므小：                                                  확댈              L玉：그                        1                          J

                    ［그림 ]-181 Arduino 프로젝트 파일 속성


      스케치 작성 및 저장하71

       우}크 불러온 스케치를 아무 수정 없이 메뉴에서 "파일／저장" 혹은 "C出＋S"를 하면 아두이
      노 기본 예제 스케치들이 읽기 전용으로 되어 있기 때문어］다른 장소에 스케치를 처장하라
      는 메시지가 나오게 된다．


                    파얻 뀐背스斗차恁垂罕毛舜畏臂恥                                                                                                    m        二m



                         Blink
                    ／女                                                                                                                                   二


                         Bllrk
                         T小陌        r an LEO ac I口r 口n므 드OCOIC. ti獅 oft f or ain SeCBo1, r텨）ecledly




                                                                                                                                                                   瓮繫好袋烈比茹姓客쏘二斗
                                                                                                                                                          ＜흩
                         lb比 in才          스케지논딤기전큠입니다 '                                            ,=,1              쯔多
                                                                                                                                                          量
                                                                                                                                                         立
                        1 /
                         r


                                                         파밀이 " 0471 전용“ 므로 표시됩 니c卜
                    f/ PIn 13                            다룐 잗소예 스7朴唾 다시 저잡휼 해야 험니다
                    // g加B It
                    mnt lid - I                                                    如甘
                    // the ；日t嗔） 11              1 1= 1 =                            1I · 乙＝'            =1                                                    :
                    acid setl브
                          // intiaNze tl比 di읽tel Pill B弓 ax 口Ut口Ut
                         p:r뗘ede(I毗 口月PUT);
                    }

                        J / 卜 hm   nmn   小h +   尸티   n   r느小   斗 小r         n nJ   거m r   m4n 1 m 1 1 rm     m
                    4                                                                                                                            !


                                                                                                                                                               旦
                                                                                                                 口   小   小m   m             小小           i客겹




                                                                                                                     Sidle口 Ui口 口r. C口m9



                         ［그림 卜19] Arduino 스커因 저징后F기



24 1 저n장 아두이노 소개1
 아두이노에서 제공하는 기본 스케치를 불러온 상태에서 수정을 하고 같은 위치에 바로
저장을 하게 되면 기본 스케치 예제코드가 훼손되기 때문에 다른 처장 장소에 스케치를
저장하는 것이 좋다. 스케치를 저장하는 위치는 어떤 곳이든 상관이 없지만 체계척인 관리
를 위해서 C드라이브에 작업 폴더 Work를 생성하고 "C:＼珉'brk\B血血＼ Blink.mlo" 위치에
저장하자. 앞으로 진행되는 모튼 스케치들은 C: \Work 폴더에 적당한 폴더를 생성하고
저장하도록 하겠다．




                ［그림 卜20]   Aid네no 스커因 저징方f기


 아두이노 스케치를 작성하는 문법（Synta功은 공학에서 널리 사용되는 C/C++ 언어와
유사한 형식을 가지고 있다. 이미 C언어를 공부한 사람이라면 스케치를 보면 굉장히 편안함
을 느꼈을 것이다. 하지만 지금 C언어를 모른다고 해서 너무 걱정하지 않아도 된다. 이
책에서는 초보자도 일아보기 쉬운 코드만으로 진행할 것이고 조금 복잡한 코드들에 대해서
는 그때 그때 상세하게 설명해 나갈 것이다. 그리고 이 책의 마지막 Chapter에서 스케치를
작성하는데 필요한 문법（Synta功에 대해서 따로 자세히 설명을 하고 있다.




                                         1.3 Arduino UNO R3로 시작하기 I 25
    Arduino 8



   스케치 컴파일 및 업로드

     스케치를 컴파일하는 방법은 간단하다. 메뉴에서 "스케치／확인＆컴파일"을 선택하거나
   단축키로 "Ct小R"을 누르거나 O阡이노 IDE어꺼 U아이콘을 누르면 된다. 작성한 스케치
   어］ 문법적인 에러가 없다면 아래 그림과 같이 컴파일이 성공적으로 완료되었다는三 내용과
   함께 아두이노 H人V（여기서는 사udino UNO R3）에 업로드 할 준비가 완료된 것이다．


                    孕 卦nk i 가듸하노 ：立5          四

                    파밀 편집 스斗지 도二 도묻랄

                    00 圄pp
                        Blink


                        B1 i oh
                        Turns on an LE0 口of口r one s旺別기i tln Off f口r son sec口rid, repeatedly,


                         Th卜弓 so카바기ecode     in the pLblic deMin
                        屯／


                    /1 미n 13 has an LE0 connected on oust Arduinn boards.
                    1/ give it 8 nope:
                    int led - 13;


                    /1 the setup routine ruS once 斗hen you press reset
                    void setup() {
                        /1 initial ize the digital pin vs nn Output
                        이nMude( led, 叫TPUT);
                    }




                    바미너리 스케치 사미즈              1 . 004 바미트 （최대 32. 206 바미트）


                                                                              酊d,ifla Una an C0M9




                                  ［그림 卜21]              Ard네no 스케치 컴파일


     스케치에 문법 에러가 발생한 경우에는 어떻게 되는 확인해 보기 위해서 문법 에러를
   발생시켜 보도록 하자. led라는 변수를 led_e珏로 수정한 이후에 컴파일을 해보자．




26 1 저Ii장 아두이노 소개
           玉 前nk I 아드이노 1.0.5




             Bl ink
             Turns on an LEO on for one second, then off for one second, repeatedly.

              Th油 餓帥미e Co由 is in the 口ubi ic 南an In
             /

            // Pin 13 has on LEO core化cted on Cost Arduirwo boerds,
            // give it e name:
            mnt led_rr 口 13;

           1/ the setup routine runs once when you press reset:
           yoid setup() f
             II initial ize the digitol pin anon output




            /1 the losS routine runs over and over seem



            led'was n。
                     t ci
                      ne아ared in 甘기s sc。
                                       pe                 forever:
                                   eu fbi
                                      ens   declurec       。。。。。
           Bl irik. ino: In turctii그li v미dl口口n( , '
           引 ink믄D 므rr口r         陀d 屹드 n口td日CS크red in this ！引二口p日




                 ［그림 卜22] Arduino 스케치 컴파일 에러


 정보 윈도우에 에러가 발생한 라인 번호와 원인을 알려주고 스케치 윈도우에도 주황색배
경으로 하여 에러가 발생한 라인을 시각척으로도 표시해 준다. 다시 에러를 수정한 이후에
컴파일을 해서 에러가 없어졌다면 이제 아두이노 UNOR3 하드웨어에 업로드 할 준비가
완료된 것이다. 아두이노 보드에 스케치를 업로드 하기 위해서는 장치관리자에 올라와
있는 아두이노 UNC）의 시리얼 포트 번호에 맞추어서 아두이노 IDE 환경에서 시리얼 포트를
설정해 주어야 한다. "도구／시리얼포트人：OM9"를 선택한다．




                                                                            1.3 Arduino UNO R3로 시작하기 1 27
  .   Ard내no .-




                      命帥.비아두안1.05 少幽磁 '耐1串                                                                                      日4百 乂
                          파밀 뀐집 스斗치洹묘 도움말

                           筐，                                             자동포맷                                Ctrl.T                      日


                      亨Bun
                        「                                                 슬：客乳로고침
                                   '    Blink                             시리얼모니E寸                             C벼   'Sh浪4M                     二
                                        伯mn on on LB[}                    보드                                                卜 rt山not日기1
                      a                                                   시리멀 포트                                            H    COM7
                                        Thin noa畔）ie CO                                                                          C（기너8
                                                                          프로그래머                                             卜

                                                                                                                                 COM9
                                   古／
                                                                          H 戶 戶 ra 三｝ 기1
                                                                          4느＝=＝느1 므 r 1

                           I/ Pin IT has en L I com祀cte. on 田ost                                  r. 1no ...r. s.
                               // 引on it a onu陀‘
                               i nt led = IT;

                               /'/ II目 net내） r며立inn runs once 咐ten you 口rest r日＄St:
                               So너 seti月）() {
                                        // initisuize the di이tol 미n as on 며Jt대it.                                                                 立
                                        pini佃de( I여， LB冊'UT);
                               }                                                                                                                  蛋3
                                                                                                                                                  =
                                                                                                                                              !
                               / ? 卜h 戶         1 1戶   나小 + : n h   H 기        1   nJ   尸   m Y n 거n : n   4 月 少八 m 少
                          ti                                                                                                              卜
                                                                                                                                                  1




                      t
                                          ［그림 卜23] Ard내no 시리얼 포트 설정


       "파일／업로드" 혹은 "Ctrl+U" 단축키를 이용하거나 U 아이콘을 눌러서 컴파일한 결과물
      （공학에서는 실행 바이너라파일）을 Arudino UNO R3 하드웨어에 업로드 한다. 실행에
      문제가 없다면 Arduino UNO R3의 I上D가 Blink(1초 주기로 I丑D가 on／아'1 됨） 되는 것을
      확인할 수 있다. C/C-'-＋어］ 익숙한 독자라면 아두이노 스케치 코드에서 main() 함수가 없다는
      것을 알 수 있을 것이다. 아두이노에서 niain() 함수가 없는 것은 아니고 아두이노 개발환경
      어］ 숨겨져 있다고 생각하면 된다. 아두이노 빌드 프로세스에 대해서 더 자세히 알고 싶다면
      加切://www. ardu力7O. C(兀7刃勿cking石Li끄dl뇨7cess I月E 1I』 페이지를 방문하면 디 상세히 알
      수 있다. I코D가 어떻게 Bli刊K가 되는지 첫 번짜1 아도이노 스케치 코드를 분석해 보도록
      하자．




28 I 제］장 아두이노 소개
      /* 아두이노 Blink 立로그램 구조 놔‘/

  /7 Pin 13 has an LED connected on most Arduino boards.
  7/ give it a name:
  milt led = 13:

  /7 the setup routine runs once when you press reset:
  void setu的 {
    /7 initialize the digital pin as an output.
       pinMode(led, OUTPUT);
  }
  7/ the ioop routine runs over and over again forever:
  void loopO {
    digitalWrite(led, HIGH);  7/ turn the LED on (HIGH is the voltage level)
    delay(1000) ;             7/ wait for a second
    digitalWrite(led, LOW);   /7 turn the LED off by making the voltage LOW
       delay(1000) ;           7/ wait for a second
  }


 아두이노 스케치의 천체적인 코드의 흐름은 위와 같다. 일반적으로 C/C++ 프로그램에서
프로그램의 첫 번째 시작 지점은 rnajn() 함수에서 시작이 되지만 아두이노 스케치 코드에서
는 mairiO이라는 함수는 존재하지 않는다. 정확히 이야기하면 존재하지 않는 것이 아니라
아두이노 II犯 환경 안에 숨겨져 있는 것이다. setup(）은 아두이노 스케치에서 한 번만
실행이 되고 loop(）는 아두이노 스케치가 종료될 때까지 반복적으로 실행이 된다. loop()
안에서 반복적으로 실행되고 있는 digitalWrite(led, HIGH）가 LED를 켜는 코드이고
digitalWrite(led, LC）町）가 I코D를 끄는 코드이다. delay(1000）은 1초동안 아무것도 하는
일 없이 기다리는 코드이다. loop() 안에서 LED를 켜고 1초 동안 기다린 후에 I正B를
끄고 다시 1초를 기다리는 것을 반복하면 LEL까 1초에 한번씩 Blink 된다．
 이러한 자세한 설명들은 앞으로 진행될 각 Chaptei들의 예제들을 통해서 자세히 설명하
도록 하겠다. 이제 아두이노를 사용하여 재미있고 다양한 예제들을 실험해볼 수 있는 모든
준비가 되었다. 각 Chapter들의 예제들을 직첩 실험해 보면서 아두이노를 가지고 어떤
일들을 할 수 있는지 직접 체험해 보도록 하자.




                                                      1.3 Ard내no UNO R3로 시작하기 1 29
전기, 전자의 기초

    2.1   전류와 전압
    2.2 저항
    2.3 LED
    2.4 브래드보드 사용법
    2.5 엔지니어링 공구
    2.6 테스터71 사용법
  .   Ard내no .




       전압, 전류, 저항 이러한 용어들은 한 번씩은 들어보거나 혹은 학교 다닐 때 배웠던
      내용일 것이다. 하지만 막상 책을 보지 않고 설명을 하려고 하면 쉽게 머리에 떠오르지는
      않는다. 우리가 아두이노를 배우는데 있어서 이러한 전자의 기초를 알지 못한다고 해서
      아두이노를 가지고 실험을 하는데 문제될 것은 없다．
       하지만 아두이노를 가지고 하는 실험들의 원리에 대해서 한번쯤은 생각해 볼만 하다．
      이번 장에서는 아두이노를 가지고 여러 가지 실험들을 하기 전에 전기, 전자의 기본적인
      내용들에 대해서 간단하게 알아보고자 한다. 물론 이번 장의 내용들을 다 알지 못한다고
      하여도 실망은 하지 마라. 이후의 장에서 실험을 해 나가면서 직접 체험으로 배워 나갈
      수도 있다．




        2.1      전류와 전압


       전자 기기를 구성하는 전자 소자는 기본적으로 천류가 흐르느냐 흐르지 않느냐로 켜기－
      끄기伯N-C）邸） 상태를 결정하여 복잡한 연산이나 기계의 논리적 작동을 해내게 된다. 이렇
      듯 천기의 이용에 있어서 전하들의 흐름을 전류라고 한다. 전류는 전위（전기적 위치에너지）
      의 차이 때문에 생끼는 것이다. 즉, 물이 높은 곳에서 낮은 곳으로 흐르듯이 전류도 마찬가
      지로 전압이 높은 곳에서 낮은 곳으로 이동한다．
       전위는 음의 전하가 많은 곳은 천위가 낮고, 양의 전하가 많은 곳은 전위가 높다. 양의
      전하가 많은 곳과 음의 전하가 많은 곳이 연결이 퇸다면 양의 천하는 전위가 낮은 곳으로，
      음의 전하는 전위가 높은 곳으로 앙쪽의 전위 차이가 없어질 때까지 움직일 것이다. 건전지
      의 경우 음극과 양극의 전위차가 없어지게 되면 건전지가 방천이 되어 더 이상 전원 공급을
      하지 못하게 된다.
       역시 말로는 쉽게 설명이 되지 않는다. 다음의 그림을 보자. 1.5V AA컨천지의 (+）쪽과
      (-）쪽의 전위차에 의해서 전기가 흐르면서 중간에 연결된 LED가 켜진다. 이때 (+）쪽에서
      (-）쪽으로의 전기의 흐름을 전류라고 하고 (+）극과 (-）극의 전위차를 전압이라고 한다．




32 I 제2장 전71, 전자의 기초
                  ［그림 午］] 전류와 전압



         항
         저
  2.2

 우리가 앞으로 실습을 하면서 가장 많이 사용하게 될 부품 중어］ 하나가 저항이다. 양쪽으
로 리드선이 길게 나와 있는 저항을 사용하게 될 것 이다. 저항은 극성이 없고 전류의
흐름을 억제하는 기능을 가진 전자 부품이다. 극성이 없다는 것은 저항의 양쪽 다리에
전원의 음극이튼 양극이든 상관하지 않고 연결을 하면 된다는 의미이다. 저항은 재료，
길이, 온도에 따라서 저항의 값이 변화한다. 도선의 저항（R）은 도선의 길이（L）에 비례하고，
단면적（S）에 반비례한다．


          R（저항） = L（도선의 킬이）Is（단면적）


 위와 같은 식으로 표현할 수 있다. 그리고 일반적으로 도선의 온도가 높아지면 도체
내부에서 전자와 원자들의 충돌 횟수가 많아져서 저항이 커지게 된다. 저항 값의 단위는
옴（Ohm)을 사용하고 기호로는 9와 같은 기호를 사용한다．




                                              22 저항 1 33
    Arduino 1




                     ［그림 2-2] 전류와 저항］


     아래 그림은 위의 부품간의 배선도를 회로 기호를 이용해서 표현한 것이다. 이러한 그림
   을 회로도라고 한다. 회로도를 잘 이해할 수 있어야 아두이노 스케치도 작성을 할 수 있다．
   처음에는 회로도에 익숙하지 않아서 어려울 수도 있지만 이 책에서는 모튼 실험에 대해서
   부품 연결 배선도와 회로도를 같이 제공할 것이다. 부품 배선도와 회로도를 비교해서 잘
   보면 이해할 수 있다．



                                         AA 배 &+ 리

                                           川F
                                 Red (633nm)
                                                     220Q




                     ［그림 ?3] 전류와 저항2


     위의 그림을 보면 이전 그림과 달리 LED 바로 앞에 저항이 연결되어 있다. 여기서 저항이
   하는 역할은 LED가 손상되지 않도록 보호하는 역할과 LED의 밝기를 조정 할 수 있다．
   I上D의 밝기는 (+）극과 (-）극으로 흐르는 전류의 양이 많으면 밝아지고 적으면 어두워진다．
     저항은 전류의 흐름을 방해하는 성질이 있기 때문에 저항의 값이 커지면 LED어］ 흐르는
   전류의 양이 작아져 LEL刈 밝기가 어두워진다. 앞에서 전류와 천압에 대해서 설명할 때
   그림에서 저항을 연결하지 않은 것은 올바른 I且） 연결 방법이 아니다. 比D소자에도 최대
   로 감당할 수 있는 전류와 천압 값을 가지고 있기 때문어］ 너무 많은 전류가 흐르게 되면
   LEI) 부품에 손상이 갈 수도 있다.



341 제2장 전기, 전자의 기초
  일반적으로 우리가 사용 하게 될 양쪽으로 리드선이 길게 나와 있는 저항은 4색（4 Band
Re덥ster）과 5색（5 Band Register) 2가지 종류를 많이 사용한다. 저항의 부품 크기가 작기
때문어 저항에 저항의 값을 전부 표시하지 않고 4선 or 5선의 색상으로 저항 값을 표시하고
있다. Band에 따른 저항 값 읽는 방법을 알아보자．


［표］ 저항 색상 표

         Color   ]St ［水｝仕    2nd Digit     3rd Digit       10의 승千            針卜11
 흑색（Black)              0              0               0              *1
 갈색（Brown)              1              1               1             巾10        1%
 적색（Red)                2              2               2            *100        2%
 오렌지색（아ange)            3              3               3       *1000(1K)
 황색（Y네ow)               4              4               4     *10000(10K)
 녹색（Green)              5              5               5   *100000(100K)      0.5%
 청색（Blue)               6              6               6            求끄d       0.25%
 자색(Vi이et)              7              7             7             卞10M       0.1%
 회색（Grayj               8              8               8          *100M       0.05%
 '백색（White)             9              9             9            *1000M
 금색（G이d)          N/A            N/A        N/A             N/A                 5%
 은색（Silver)       N/A            N/A         N/A            N/A                10%
 入[one            N/A            N/A        N/A             N/A



4 Band Register 읽는 법


                                            옆의 저항 값을［저항 색상 표｝를 참조해서 그디：1
                                            로 읽어보면 왼쪽에서부터 색깔 순서로


                                            갈색H흑各牛빨간색은색
                            오차
                            0그              =1-    0 寸 처00- 10%
                            2m Digit
                            1닦 Dig仕         = ]0*100
                                                                  ]rio,
                                           ：二 ] 0000 = ] 아（ Ohn가 士 LI /。


                            [4 Band Register 예저'II


아래 표의 저항들도 위의 법칙을 생각하고 읽어 보자．



                                                                           22 저항 I 35
-.   Arduino .




                                                   갈1오H적1금                                       오中적1갈m금
      卞1
                                                                                                 320 Ohm 士S) /0
                                                                      卞1
                                                   1.3K Ohm 士5%

                                                   길尸흑궉발우             mmm
                                                                                                 갈小흑오H은
                               燕                                                                 ] 0K Ohm 士 ] U
                                                                                                              (0//。
                                                   1K Ohm 士 10%
                   4   ,   :       " 』   小   g 寸




     5 Band Register 읽는 법

                                                                            옆의 저항 값을［저항 색상 표를 참조해서 그대
                                                                            로 읽어보면 왼쪽에서부터 색깔 순서로



                                    I    1
                                                         翼
                                                         和Digit
                                                                            갈색－흑색흑색－빨간색＋색
                                                                            = ] -0-     0 小 ' 10 - 10%
                                         I               2'fO呼t             = inn치（)
                                         '               1낚 0呼t
                                                                            二二 10000 = 10K Ohm 士 I U
                                                                                                   fl0//。

                                                          [5 Band Register 예저I]


     아래 표의 저항들도 위의 법칙을 생각하고 읽어 보자．

                                                   갈1오叫흑戶갈금                                      오1빨1흑中흑H금
                                                                                」喀 甘      神韋
           m1
                                                   1.3K Ohm 土 5%                                 320 Ohm 士J /。


                                                   갈1흑戶흑1갈믄                                      갈H흑1흑尸뻘卜은
                                                                                燾 i트 熏 ，【 嚼
           =m=
                                                   ] K Ohm 士 ] 0%                                10K Ohm 士］U /。




                 2.3

                 우리가 아두이노 실험에서 저항 다음으로 많이 사용하게 될 소자이기 때문에 I月D사용
     방법에 대해서 잘 익혀 두도록 하자．
                 珏D란 Light Em奴血g Di月e의 약자로 빛을 뿜어내는 반도체란 뜻이다. 발광다이오드의
     가장 큰 특징이라고 한다면, 기존의 전기 구동 발광체에 비하여 열을 적게 발생한다는


36 I 제2장 전기. 전자의 기초
것과 열손실로 인하여 낭비되는 에너지가 척다는 것, 반영구적인 수명을 들 수 있다．




        캐소드
              L   ;
        (Cathode) :
                       몌드
                        노
                                      lED를 희로 기호로 표시




                         ［그림 十4] LED의 특성


 LEI) 연결시 I上D의 몰딩 안쪽을 자세히 보면 위의 그림과 같이 쇠판이 작은 것과 큰
것으로 분리가 되어 있는 것을 볼 수 있다. 일반적으로는 쇠판이 작은 쪽이 다리가 길고
Anode（애노드）라고 한다. 반드시 vCC（전원）에 연결해야 한다. 그리고 반대편 다리는
Cathode（카소드）라고 하며 GND(그라운드）에 연결을 해야 한다. 저항과 달리 珏D는 극성
이 있기 때문어］ 반대로는 전류가 흐르지 못하기 때문어］반대로 연결을 하면 LED가 켜지지
않는다.




                      ［그림 }5]   LED의 올바른 사용법


 比D를 회로 기호로 표시를 하면 위의 그림과 같고 항상 저항과 같이 사용하여야 한다．
比D마다 최대 전압과 전류가 정해져 있다. 만약에 I코D를 켤 때 저항을 사용하지 않으면
LED가 허용하는 최대 전류 값을 초과하여 LED가 고장이 날 수도 있다．




                                                       2.3 匹D I 37
  s A川내no




      2,4    브래드보드 사용법


     이전 2.2절에서 LED를 켤 때 건전지와 부품들만을 이용해서 실험을 하였다. 부품이
   小3캐 정도라면 괜찮지만 연결해야할 부품의 개수가 3개 이상이 되면 연결하기가 쉽지
   않다. 이때 부품들 간의 연결을 점프 케이블이라는 것을 이용해서 간편하게 연결하도록
   도와주는 도구가 브래드보드이다．
     이번 절에서는 2.2절에서 珏I居 구동시켰턴 동일한 실험을 브래드보드를 이용해서 부품
   들을 삽입하여 I코D를 구동시켜 보자. 먼저 브래드보드의 구조에 대해서 자세히 일아보자．




                                 1   1   1   1   1   1   1       1       1       1       1       1   1       1




                                                             多       t       才       七       m           1       {   !   寸   午   卞   中 巾     q   寸   字   寸   卞   李
                                                             !       1       1       =       1           1       m   中   !   1   卞   卞   1   f   t   乍   卞   b   卞




                     ［그림 ?6]   브래드보드의 구조



     브래드보드는 부 품 들 을 구멍에 끼우면 브레드보드 안쪽에 숨어져 있는 금속 조각으로
   인하여 부품들이 연결되고, 이로써 회로를 구성하고, 실험하고, 간단하게 변경할 수 있는
   실험 도구이다. 브레드보드의 구조는 위의 그림과 같이 가장 위쪽의 2줄과 아래의 2줄은
   옆으로 모두 연결이 되어 있고 나머지 수직으로 나열되어 있는 5개의 홀들도 마찬가지로
   5개씩 수직으로 모두 연결이 되어 있는 구조이다. 즉 위의 그림에서 파란색 원으로 되어있
   는 27相 홀은 서로 연결이 되어 있다. 실제 부품들을 삽입해서 브래드보드에서 어떻게
   연결이 되는지 예를 들어보자．




381 제2장 전기, 전자의 기초
                                                                                                                                                                                                                                                                               多
                                                                                                                                                                                           서로 면걸되어
                                                                                                                                                                                            있지 많다．                                                          왼쪽 그림에서 붉은색 라인과 오
                                                                                                                                                                                                                                                            른쪽에 있는 파란색 라인은 서로
                                                                                                                                                                                                                                                            연결이 되어 있지 않다. 하지만
                                                                                                                                                                                                                                                            세로 방향으로 붉은색 라인이 있
                                                                                                                                                                                                                                                            는 5개의 홀끼리는 모두 연결이
                                                                                                                                                                                                                                                            되어 있다. 마찬가지로 붉은색 라
                                                                                                                                                                                                                                                            인 옆어］ 있는 파란색 세로 방향의
                                                                                                                                                                                                                                                            5개의 홀끼리도 모두 연결이 되어
                                                                                                                                                                                                                                                            있다．
                                        ［그림 午7]                                                                                브래＝ 부＝ 구조너

                                                                                                           뇨

                                2개의 지점   '}
                                                    ／巴亨中＼
                                은서로연켤 , ‘吐1
                                되어 있다． 뇨芦                                                                                                      1

                                                                                                                                                                                                                                                           왼쪽 그림에서 붉은색 세로 방향
                                蜘m＼         뇨，
                                             mm可，                       多怒쏘：
                                                                    뇨二




                                                                                                                                                                                                                                                           으로 5개의 홀은 모두 연결이 되어
                                                                                                                                                                                                                                                           있다. I上D의 (+）극와 (-）극이 모두
1

卞
        1

        牛
                1

                1
                        1

                        1       1       1   1               1       1              1       1           1       亡                                           4           卞   +       1           甘       +   f           心   也           仁       =       4
                                                                                                                                                                                                                                                           연결이 되는 이런 부품 배치는 하
1       甘


                                                                                                                                                                                                                                                           면 안된다. 브래드보드에서 LED
                                                                                                                                                                                                                                                           부품 연결 시 주의해야 한다．          n




                                        ［그림 十8]                                                                            브래＝ 부C二 구조-2


                                                                                                                                                                                                                                                           브래드 큰드의 가장 위쪽 가로 방향
                                                                                                                                                                                                                                                           의 노란색 라인끼리는 모두 연결이
                                                                                                                                                                                                                                                           되어 있고 마찬가지로 위에서 2번
                27g의 치첨은
                서로 연결되어
                                                                                                                                                                                                                                                           째 줄의 파란색 가로 라인끼리도 모
                                                                                                                                                           1       1       1       1       1       t       斗       4       1       1       1       1


                 있지 많다，

                                                                                                                                                                                                                                                           두 연결이 되어있다．
1       口                                                           4              Y       q           卞       巾       卞       1       t       t       牛   年       斗       斗       斗       斗       卞       8       卞       斗       寸       t       1

巾       1       1       1       1       1   1           1       t              1           卄           1       n       1       1       4       斗       1   1       1       8       巾       斗       卞       七       t       1       t       年       1

1       斗       寸       1       1       +   1           1       1              1           1           1       1       1       小       1y      1       斗   方       才       8       卞       1       寸       巾       t       1       斗       q       1

小       斗       m       1       1       1   1           1       1              1           1           +       1       1       1       1       1       斗   斗       拉       h       1       t       1       卞       和       李       斗       m       1

1       r       小       1       1       1   1           1       1              i           1           1       1       1       1       1       1       1   斗       1       e       m       甘       小       4       七       口       t       1       斗




    1                                               1
            1       斗       1       t           1           1           斗              小       1                   4       4       1       小       m           1       1       8       1       t               t       1       小       1       i
                                                    1                                              1
    1       t       寸       巾       寸           1           1           t          寸           斗                   1       1       1       4       t           夕       1       1       1       t               t       斗       1       m       t




                                    ［그림 午9]                                                                                브래＝ 부＝ 구조＜3



                                                                                                                                                                                                                                                                     2.4 브래드보드 사용법 1 39
  .        Ard네no 兮



            1개의 I코D, 저항, 건천지를 이용해서 rn 를 켜는 실습을 브래드보드를 이용해서 해보
      자．
                                                     AA 배 터 리



                                         I            玔
                                         1
                                             Red (633rim)       220Q




                      ［그림 乃10] 브래＝부＝를 이용한 匕ED 구동 실습



            브래드보드의 구조를 이해하기 위해서 일부러 좀 복잡하게 선을 연결해 보았다. 하지만
      회로도를 보면 2.2절에서 브래드보드 없이 연결했던 I코I) 구동 회로와 동일하다는 것을
      알 수 있다. 앞으로 진행되는 모든 실험들은 브래드보드를 이용해서 부품들은 연결해서
      실습을 진행해 나갈 것이다. 어렵지 않은 내용이니 지금까지 배운 브래드보드의 구조와
       저항, 比D의 특성에 대해서는 확실하게 이해를 하고 넘어 가도록 하자. 이 부분을 이해하지
      못한다면 이후의 실험들의 배선도와 회로도를 이해하기 힘들 것이다．



           戶Jn
              "브레드보드"라는 이름은 점대점 구성의 초기형태에서 이름이 유래되었다. 라디오 三三창기에
            비전문가는 구리 선이나 단자 스트립을 나무 기판 （글자 그대로 빵을 자르는 식판）에 둣박았고，
            땜납 전자 부 품 을 연결하였다. 가끔 도면 다이어그램은 단자, 부품과 전선의 배치를 O｝내하는
            것처럼 기판에 첫 번째로 붙였다．
                                                            Wikipidi2 참조




40 ! 제2장 전기, 전자의 기초
          2.5       엔지니어링 공구小m


      전자파트에서 취미로나 혹은 전문적인 일을 하는 경우에 반드시 필요한 엔지니어링
도구들이 있다. 가장 많이 사용하는 도구들을 나열해 보면 핀셋, 인두기, 납, 니퍼, 테스터기
틋이 'th斗 하가지 씬 그린윽 닙며서 새7] 꾸야J가． 요工二르 이岫1-닙又I-
                                         1   \J   !d1   t=   t:=   1 卞J+   1 1




                        핀셋1
                        주로 작은 부 품 을 잡거나 납땜을 할 경우에 핀셋을 이용하여 부 품 을 고정
 //
                        하고 납땜을 하는 용도로 사용된다. 굉장히 많이 사용되므로 17月 정도는
                        구비하는 것이 좋다．

                        인두기
                        납을 이용하여 부 품 을 PCB 기판에 고정하는데 사용하거나 전선을 연결하




叱
                        는 경우에도 인두기를 납과 인두기를 사용한다. 이 책에서는 브레드보드
                        를 사용하기 때문에 직접 인두기를 사용할 일은 없겠지만 전자파트에
                        취미가 있거나 일을 할 때 반드시 필요한 도구이다. 비싼 제품은 수십만원
                        어］ 달하는 제품도 있지만 5만원 이하의 제품도 쓸 만하다. 비싼 제품일수
      m    "

                        록 일정도 온도 유지와 사용자가 설정한 온도에 도달하는 시간이 빠르다．
               Hr
                        일반적으로는 20珥 정도의 인두기를 사용하면 된다.




          m
                        匕F


                        인두기를 사용하여 PCB 기판에 부품 을 조정할 때 사용




<
                        니퍼 ．
                        전선을 자르거나 피복을 벗．겨낼 때 반드시 필요한 도구이다．
-.   Ard내no .




                      테스터기
                      전압, 저항, 전류 등을 측정할 수 있다．
                      처음에는 별 필요성을 느끼지 못하겠지만 아두이노보드 혹은 전원에 이상
                      이 발생한 경우에 반드시 필요한 도구이다. 엔지니어라면 1가1 정도면
                      꼭 구비하기 바란다. 아두이노보드에 전원 I丑D가 켜지지 않는다면 테스
                      터기를 이용해서 아두이노보드의 5\/ 전원 단자를 측정하여 5,'/ 출력이
                      나오는지를 제일먼저 확인해 보아야 한다．

                      브래드보드
                      PCB제작을 하기 전에 브레드보드와 점프 와이어를 이용해서 Proto四恥을
                      해볼 수 있는 도구이다. 회로가 정확한지 모르는 상태에서 검증을 하지
                      않고 PCB제작을 하는 것은 비용만 중가하는 결과를 초래하게 된다．



                      점프 와이어
                      브래드보드 사용시 아두이노 보드와 부 품들 을 연결하기 위해서
                      하게 된다. 모든 실험에서 반드시 필요하다．




      위에서 나열한 도구들 이외에도 전문가들이 사용하는 고가의 오실쿠入극7ji, 로직분석기
     등 다양한 도구들이 있지만 초본 엔지니어가 반드시 갖추고 있어야할 도구들만 나열해
     보았다. 금전적인 여유가 허락 한다면 위에서 나열한 도구들은 반드시 갖추고 있는 것이
     좋다．




       2.6      테스터71 사용법

      2.5절에서도 테스티기에 대해서 이야기 했지만 다른 도구틀은 사용방법이 그리 어렵지
     않지만 테스트기에는 기능이 많아서 조금 상세하게 설명 하고자 한다．
      테스터기의 기능에 따라서 전압, 저항 이외에도 전류 측정도 되는 제품들이 있지만 이번
     절에서는 테스터기의 기능 중에서 가장 많이 사용이 되는 전압과 저항을 측정해 보도록
     하고 그리고 전선의 단락 검사를 해보자. 예전에는 아날로그 테스터기（바늘로 검사 결과
     수치를 알려 준다）를 사용하였으나 최근에는 대부분이 디지털 테스터기를 入鹿한다．



42 I 제2장 전기, 전자의 기초
                                    "蜘낳牛如

                        붉은색 Probe와
                          m可沙
                        검욘색 Probe률
                         연켤한댜，
                                J        戶
                                    小1




                   ［그림 즈11] 테스터7j


 테스터7 를 보면 중앙에 동그랗게 다이얼버튼이 있어서 측정하려고 하는 목적에 따라서
다이얼 버튼을 돌려서 측정을 하면 된다. 그리고 하단에는 검은색과 붉은색의 홀이 있는데
검은색 홀에는 검은색 Pit比를, 붉은색 홀에는 붉은색 Pr아戈를 연결하면 된다. 이제 테스터
기가 준비가 되었으니 테스터기를 이용하는 방법을 알아보자．


단락 검사를 해보자

 단락 검사는 쉽게 설명하면 전선이 끊어졌는지를 검사하는 것이다. 예를들면 LED를
켜기 위해서 아두이노보드와 브래드보드를 점프 와이어를 이용해서 연결했는데 아두이노
스케치 코드에 이상이 없는데 LED가 켜지지 않는다면 점프 와이어가 브래드보드와 아두이
노 보드사이에 정확하게 연결이 되었는지 단락 검사를 해보면 알 것이다．




                                             2.6 테스터71 사용법 143
 .   Ard내no .




                       ［그림 十12]   단락 검사



      위의 그림과 같이 다이얼 버튼을 위치시키고 2개의 Pro比를 가지고 단락 검사를 하려는
     전선의 양 끝을 접지시킨다. 만약 전선이 끊어지지 않았다면 보통은 " aH］尸尸" 하는 소리가
     날것이고 전선이 끊어졌다면 아무소리도 나지 않을 것이다．


     전압을 측정하1 보자

      아두이노 보드에서 출력되는 DC 5.OV 전압과 3.3\/ 전압을 측정해 보자．



                                       刈 n
                                       n日 n
                                       1 4
                                          i
                                   r
                                   =



                                             了k됴므
                                       n
                                       E h

                                       口

                                             ；卜H1
                                       5 n




                      ［그림 ?13] 5.o\/ 전압 측정



441 제2장 전기, 전자의 기초
 5V 천압을 측정하기 위해서 위의 그림과 같이 다이얼 버튼을 위치시키고 검은색 Pro比는
반드시 GND에 접지하고 붉은색 Probe는 아두이노 보드에서 5V 출력이 나오는 포트를
접지 한다. 올바르게 Probe를 연결했다면 테스터기의 액정 화면에 5.0이라고 표시될 것이
다. 여기서 액정 화면에 반드시 5.0이라고 표시되지 않을 수도 있다. 출력 천압이 5.OV보다
낮은 4.9V가 나올 수도 있고 5.2V가 나올 수도 있기 때문이다．
 어쨌든 5.OV와 비슷한 전압이 측청이 되면 맞는 것이다. 당연히 전압을 측정하기 천에
아두이노 보드에는 USB를 이용하거나 DC 어댑터를 이용해서 전원을 공급하고 있어야
전압이 측정이 된다. 그렇지 않으면 0v가 측정이 될 것이다．




                 ［그림 ?14] 3.3V 전압 측정


 이번에는 위의 그림과 같이 붉은색 Probe를 아두이노 보드의 3V3이라고 되어 있는
포트어］ 접지시킨 다음 테스터기의 액정 화면을 확인해 보자. 3.3V와 유사한 값을 표시하고
있을 것이다．


저항을 측정하1 보자

 2.2절에서 색 띠를 이용해서 저항 값 읽는 방법을 배웠었다. 색 띠를 보고 구분할 수도
있겠지만 이번에는 테스터기로 직첩 저항 값을 측정해 보자．



                                         2.6 테스터기 사용법 j45
  e Ard네n(그




                               \        m     /
                      ［그림 ?15] 저항 측정


      저항을 측정하기 위해서 위의 그림과 같이 다이얼 버튼을 위치시키고 검은색 Probe와
   붉은색 Pr아光를 저항의 양 끝에 접지시킨다. Pro比를 접지시킬 때 저항의 방향은 고려하지
   않아도 된다. 그러면 테스터기의 액정 화면에 처항값을 표시할 것이다. 전압을 측정할
   때와 마찬가지로 저항에도 오차가 있기 때문어］ 원래의 저항값과 유사한 값을 표시해 준다．




46 1 제2장 전기, 전자의 기초
디지털 입력과 출력

   3.1 디지털 출력이란7
   3.2 LED 깜박이기
   3.3 7 세그먼트 구동하21
   3.4 버튼을 이용하여 스케치 없이 LED 제어하기
   3.5 버튼을 이용하여 LED 제어하기
   3.6 버튼을 이용하여 LED 상태 제어하71
   3.7 부저（Buzzer) 울리기
-.          Arduino .-




       1互1 디지털 출력이란7

        아두이노에서 출력은 크게 디지털 방식과 아날로그 방식으로 나눌 수 있다. 아날로그
       출력은 이후의 Chapter에서 자세히 알아보기로 하고 이번에는 디지털 출력에 대해서 일아
       보자. 공학적인 개념에서 디지털 출력은 마이크로컨트롤러에서 외부로 데이터를 내 보내는
       더1, 결국은 마이크로컨트롤러의 특정 핀의 전압을 I-IIGH 또는 LOW로 설정하는 것을 말한
       다．
                             ［그림 3-1] Ard네no 디지털 포트


             아두이노에서 디지털 출력으로 사용할 수 있는 포트는 위의 그림에서 127긔 정도가 된다．
            참고로 "N" 표시가 있는 포트들은 I刈M(Pulse Width Modul的on）기눙이 있는 출력 포트
            들이다．
              참고로 아두이노에서 모든 포트들이 pW八4 기능을 갖지 못하는 이유는 PW入I 기능은
            CPU의 TIMER 라는 자원에서 지원을 해주고 있는데 ATMEGA CPU의 Timer에서 PW入4
            출력이 가능한 포트들이 제한이 있기 때문이다．




     481 제3장 디지털 입력과 출력
  3.2   LED 깜박이기


 Chapterl 에서는 아두이노 보드에 연결된 I표）를 깜빡이도록 하였고 이번에는 아두이노
하드웨어 외부에 브레드보드를 이용해서 LED를 깜박이도록 해보자．


실험에 필요한 준비물들




                                                 H
                    ：三n= 1


                              ;（珦   」／ .   S




                         a.                1


    브래드보드 17뀨        아두이노 UNOR3                적색 比D／끄（ 저항 2깨1




하드웨어 연결

 첫 번째 단계로 27胴 적색 LED와 저항(1지을 브레드보드에 연결한다. 브레드보드에
배선 연결 작업을 할 때는 항상 전원을 인가하지 않은 상태에서 작업을 해야 한다. 그렇지
않으면 쇼트 둥의 실수로 인해서 실험 부품 혹은 아두이노 보드가 고장이 날 수도 있다．
특히 vCC（천원）과 GND（그라운드）는 절대 쇼트（접촉）가 되어서는 안 된다．
 아래 그림이 배선도와 회로도이다. 아래 도면을 이해하지 못한다고 해서 걱정할 필요는
없다. 지금 회로도를 이해하지 못한다고 해도 단계별로 브레드보드를 이용해서 따라하다
보면 회로도를 읽는 요령을 습득하게 될 것이다．
 회로도에서 아두이노 보드의 디지털 핀 D8, I刃어］ 각각 I且）를 연결하고 전류를 조절하는
저항을 각각의 LED에 연결한다. 회로의 전원은 컴퓨터 USB 전원에 연결해서 공급한다．




                                                    3.2 LED 깜박이기 1 49
 .   Ar出_Aino .




                             1




                                 :

                                                           :;
                                         "!
                         甘
                  1              4   1        1   1         1   1   m   寸




                  :
                                 1   1        中




                                                                ［그림 +2]                LED 깜빡이기 배선도



                                 3V3                  5V        니N
                                                                    1
                  RESET                           Arduino                     TX/DO

                  日ESET2                           Uno                        RX/Dl

                  AREF                            （日ev3)                         D2

                  1OREF                                                      PWM 03
                                     사d미no UNO 日3
                                                                                 04

                  AO                                                         PWM 05

                  Al                                                         Pw 小 06
                                                                                               m＝
                                                                                                            LED1
                  A2                                                             D7                         Red (633nm)
                                                                                                      小mm
                  A3                                                             08
                                                                                                            LE02
                  A4/SDA                                                     PWM 09        m    幽1m
                                                                                                            Red (633nm)

                  A5/SCL                                                SS/PWM 010

                                                                    M（그없／P빠／011

                                                                            卞川SO/D12

                                                                             ScI0D化




                                                           OND




                                                                ［그림 +3]                LED 깜빡이기 회로도



50 I 제3장 디지털 입력과 출력
 프토二l램 작성

  아두이노 스케치에 아래와 같은 코드를 작성한다．

   mnt ledi = 8;
   mllt led2 = 9;

      void setupO
      {
          pinMode(ledl, OUTPUT);
          pinMode(led2, OUTPUT);
   }
   void loopO
   {
          digitalWrite(ledl, HIGH);
          digitalWrite(led2, HIGH);

          delay(500) ;

          digitalWrite(ledl, LOW);
          digitalWrite(led2, LOW);

          delay(500) ;
  }


加t ledi = (5,
加t 七d2 = 9;

             브레二부＝에 있는 LED 2개를 아두이노 보드의 디지털 출력 포트 8과 9에 연결을 했기
             때무게 아두이노의 디저털 출력을 이용해서 匡D를 제어하기 위해서 스커因 코드에서 변수
             를 선언하였다．


pinMode(ledl, OUTPUT);
pi小4ode(led2, OUTPUT);
             아두이노 보드의 8번 포트와 9번 포트를 출력으로 이용하기 위해서 0u耳UT으로 설정하였
             다. pin卜Aode(Ied1, OUTPUT) 대신에 pinMode(8, OUTPUT) 이라고 스케치 코드를 작성해도
             되지만 변수를 선언해서 코드를 작성하는 것이 훨씬 얄아보기 편하고 나중에 브레＝부二9r
             아두이노 보므2F2I 배선 연결이 변경이 되었을 경우, 즉 회로적으로 변경이 일어났을 경우게



                                                                3.2 LED 깜박이기 1 51
 .   Ard너no 1 -




            스케치 코드를 수정할 때 선언된 변수에서 값만 바꾸면 되므로 수정하기가 쉽다. 그리고
            아두이노 포트를 입력 혹은 출력으로 설정하는 것은 한번만 하면 되므로 Ioop() 함수에
             위치시키지 않고 한번만 실행이 되는 setup() 함수 내에 위치 시켰다．


     ci會亢a/Wi亡e口h끄， HIGIL七
     （如亡a/Wi北C伽ci乙 HIGI玹
             아두이노 보드의 8번과 9번 포트를 녜GH로 출력시키면 실저르 아두이노 보드의 8번과
             9번 포트에서 출력 전압 값이 0v에서 5.0V로 바뀌게 된다. 포트에서 5V 출력이 나오게
             되면 전류는 전압이 높은 아두이노 8번 포트오F9번 포트에서 전압이 낮은 GND 쪽으로
             전류가 흐르면서 匕ED］과 匕ED2가 켜지게 되는 것이다．


     deJaM免M方
             LED가 켜지고 나서 끄71 전에 약간의 지연 시간이 필요하다. delay() 함수는 milisecond
             단우를 시간을 지연시키는 기능을 가지고 있다. 飼ay0 함수의 인자로 500을 넘겨 주었기
             ［대뭔）카 500msec 동안 delay() 함수 다음에 있는 아두이노 스케치 코드들이 실행 되지 못하
             고 시간이 지연되게 된다．


     （如亢a/ Write伽dl, 工OW方
     m智亢a加必北e伽a乙 LO1彩七
             아두이노 보드의 8번과 9번 포트를 LOW로 설정하게 되는 아두이노 보드의 B번과 9번
             뜨三에서 출력되는 전압015v에서 0v로 바뀌게 되어 아두이노 보드의 포트와 GND 사이에
             전류가 흐르지 않게 되어 LED가 꺼지게 된다．


     실행결과

      컴파일을 해서 에리가 있다면 입력한 코드가 정확히 입력했는지 확인한다. 입력할 때
     괄호와 세미콜론을 정확히 입력해야 한다. 코드가 에러 없이 컴파일 되면 아두이노 보드와
      연결된 포트를 선택해서 코드를 업로드 한다. 아두이노 보드에 코드가 정상적으로 업로드
      되면 작성한 스케치를 아두이노 하드웨어에 업로드를 하면 500msec(0. 5초） 간격으로 珏D2
      개가 동시에 켜졌다가 꺼졌다가를 반복하게 된다. 만약 I丑D가 깜박이지 않으면 USB 케이
      블 연결을 제거하고 LED가 회로도 같이 연결 했는지 확인한다．




52 I 제3장 디지털 입력과 출력
                    7 세그먼트 구동하71


 3.2절에서 I丑I居 구동시켜 보았다. 하지만 珏D의 상태는 ON과 OFF의 상태만을 표시
할 수 있어서 자세한 정보를 표현하지는 못한다. 이번 절에서 실험할 7 Se얗nent는 내부에
7개의 LED를 내장하고 있다고 생각하면 된다．
 7 Segment는 7개의 LED를 가지고 I丑D가 표현하지 못하는 다양한 정보를 비교적 쉽게
표현 가능하다. 그래서 우리 주변의 가천제품 등에서도 많이 사용이 되고 있다. 7Se얗nent
는 1자지로 시작하여 10자리가 넘는 부품도 많이 있지만 이번 절에서는 한 자리 7 세그먼트
어］ 1부E49까치 수차륵 차돗으로 표시하누 심헉윽 해보다


실험에 필요한 준비물들

                                         ；計“萍‘ I


                                                    :EY9 1. .


                                               11       H   H   1
                                              e

                        브래드보드 1깨1          아두이노 UI幻 R3



                                                    I

                                                    年
      2                  2



      .

      '
               i:   -
                         '
                             壬:     3,
      匹 7                斗
          I-
      n                  口




   Common Cathode Type MT03911AR 17뀨         470옴 저항 8개




하드웨어 연결

 아래 실험은 Anode（아노드） 타입의 7 세그먼트를 이용한다. 7 세그먼트는 Anode 공통
형과 캐소드K加lode) 공통 형 두 가지 형태가 있다. 그래사회로를 연결할 때 공통 단자를
아노드 타입은 vcc어］ 캐소드 타입은 GND어］ 연결해서 사용한다．




                                                     3_3 7 세그먼트 구동하기 1 53
       no e




                                                                        +d6tTJ


               Common cathode Type                 Comn겨가｝ Anode TyF唯


                          [그림 3-4] LED 7 Segment Types


    우리는 공통 캐소드 타입을 사용할 것이기 때문에 공통（Common）단자에는 GND를 연결
   해야 한다. 그리고 위의 그림처럼 "甘자를 만들기 위해서는 e, b, a, c 번에 연결된 아두이노
   디지털 포트를 HIGH로 만들어 주면 된다．
     실험에 사용된 7 세그먼트는 Cathc乂le 타입이다. 회로에 220옴 시리얼 저항을 사용하는
   이유는 7 세그먼트의 恥rward Voltage 가 2V, 전류가 20n洽 그리고 아두이노 보드가 3.3V
   또는 5v를 사용한다. 그래서 (5-2)/0.02=150옴이 된다．
     시리얼 저항은 5V 아두이노 보드에서는 150옴 이상 시리얼 저항을 달아주면 된다. 3.3V
   아두이노 보드에서는 (3.3-2)/0.02=65옴 이상 저항을 사용하면 된다. 보통은 이런 복잡한
   계산식 필요 없이 우리가 진행하는 실험에서 470-옴 시 3K옴 상이의 아무 저항이나 사용해
   도 상관은 없다. 단지 저항의 크기에 따라서 저항의 값이 크면 전류의 흐름을 방해하는
   성질이 커져서 LED가 어둡게 켜지고 저항의 값이 작으면 比D가 밝게 켜지는 차이가 나타날
   것이다．




541 제3장 디지털 입력과 출력
                  ［그림 于51 7 Segment 배선도



         3V3    5V        너N                                                 I Sngmont


RESET          Arduino             TX/DO

RESET2           Uno               日X/D1                          4700

AREF           （日ev3)                 02

口REF                              PWM D3
                                                                             才＋
                                                                       人1
                                                          小，
           사d네no UNO R3
                                      04    mm.   ,$.m甘   冊小m件




AO                                FWM 05          뇨．
                                                   H,            葬00              才＋
/\1

P2
                                  PWM D6

                                      07
                                            나中十小H二阡
A3                                    08                         件
A4/SDA                            PWM DO
                                                                                  才＋
A5ISCL                         SS/FWM DIO

                           MOSI/PWM Dli
                                                        卜二卜于
                                                      二乙＋
                                h川S이0俚                           。4
                                                                 47。。       卞才＋
                                                                 Wi-
                                  SCKf 0出




                     GND




                                                                                       fritzing
                  ［그림 于61 7 Segment 회로도



                                                                             3.3 7 세그먼트 구동하기 I 55
 小. Ard네no .如



   프로그램 작성

     아두이노 스케치에 아래와 같은 코드를 작성한다．

     const mllt a=2;
     const m1lt b=3;
     const m1lt c=4;
     const mllt d=5;
     const m1lt e=9;
     const m1lt f=8;
     const m1lt _g= 7;
     const mllt dot=6;

     void display_number(int n)
     {
         switch(n)
         {
             case 0:
               digitalWriteCe,HIGH);
               digitalWriteLb.HIGH);
               digitalWriteCc,HIGH);
               digitalWriteCd,HIGH) ;
               digitalWriteCg,HIGH);
               digitalWriteCf.HIGH);
               digitalWriteCa,LOW);
               digitalWriteCdot,LOW);
               break;
             case 1:
               digitalWriteCe,LOW);
               digitalWriteCb,LOW);
               digitalWriteCc,LOW);
               digitalWriteCd,LOW);
               digitalWriteCg,HIGH);
               digitalWriteCf,HIGH);
               digitalWriteCa,LOW);
               digitalWri扼Cd毗,LOW) ;
               break;
             case 2:
               digitalWriteCe,HIGH);




561 제3장 디지털 입력과 출력
    digitalWriteLb,Low);
    digitalWriteLc,HIGH);
    digitalWri扼（코,HIGH) ;
    digita1Write(g,Low);
    digita1Write f,HIGH);
    digitalWriteLa,HIGH);
    digitalWriteLdot,LOw)
    break;
 case 3:
    digit刻．Write（卄e,HIGH);
    digithlwriteLb,LOw)
    digita1Write(c,LOw)
    digitaI1ATrite(d,HIGH);
   digitalwriteLg,HIGH);
   digitalWrite(j, HIGH);
   d溥talwrite（크,HIGH) ;
   digitalWriteLdot,Low);
   break;
 case 4:
   digitalWriteLe,Low);
   digitaI刀rite(b,HIGH);
   digitalWriteCc,Low);
   digita1Write(d,LOw)
   digita1Write(g,HIGH);
   digitalWriteLf,HIGH);
   digitalWriteLa,HIGH);
   digitalWrit可코毗,Low);
   break;
case 5:
   digitalWriteCe,HIGH);
   digitalWriteLb,HIGH);
   digitalwriteLc,LOw)
   digitalWriteLd,HIGH);
  digitalwriteLg,HIGH);
  digitalWriteLf,Low);
  digitalwriteLa,HIGH);
  digitalWriteLdot,LOW)
  break;
case 6:
  digitalWriteLe,HIGH);


                              3.3 7 세그먼트 구동하기 ! 57
         digitalWrite(b,HIGH);
         dligita1Write(c,HIGH);
         digitalWrite(d,HIGH);
         digitalWriteCg,HIGH);
         digitalWrite(f, Low);
         digitalWrite(a,HIGH);
         digitalWriteCdot,Low);
         break;
       case 7:
         digitalwriteLe,HIGH);
         digitalWrite（巾,I표GH);
         digitalWriteCc,Low);
         digitalwriteLd,Low);
          digita1write(g,HIGH);
         digitalWrite(j, HIGH);
          digitalWriteLa,Low);
          digitalWrite(dot,LOW);
         break;
       case 8:
          digita1Write(e,HIGH);
          digitaiW毗e（小, HIGH);
          digitalWriteCc,HIGH) ;
          digita1Write(d,HIGH);
          digitalWriteLg,HIGH);
          digita1Write(f, HIGH);
          digitalWriteCa,HIGH);
          digitalWriteLdot,LOW);
          break
        case 9:
          digitalWriteCe,HIGH);
          digitalWrite(b,HIGH);
          digitalWriteCc,Low);
          digitalWriteCd,HIGH);
           digitalWriteLg,HIGH);
           digitalWriteCf,HIGH);
           digitalWriteCa,HIGH);
           digitalWriteLdot,Low);
           break
        case 10:
           digitalWriteCe,Low);


581 제3장 디지털 입력과 출력
                 digitalWrite(b,Low);
                 digitalWriteCc,Low);
                 digitalWrite（코,L小V);
                 digitalWrite(g,LOW);
                 digitalWriteLf,Low);
                 digita1write(a,Low);
                 digitalwriteLdot,HIGH);
                 break;

  }
  void setupO
       {
           pinMode(a,OUTPUT);
           pinMode（上, O1了rPt了F);
           pinMode(Hc,OUTPUT)
           pinModeLd,아刃PUT);
           pinModeLe, OUTPUT);
           pinModeCf,OUTPUT);
           pinMode(g,OUTPUT);
           pi小加deLd야,아牙F兀JT);
  I;
  void loopO
   {
           m1lt i;

           如r(i=0;i<11；卄＋)
           {
               display_number(i);
               delay(1000);
           }
  }

 천체적인 스케치 코드의 흐름은 7 세그먼트의 각 핀의 이름 변수를 아두이노 보드에
연결된 핀으로 선언한다. void setup() 함수에서 7 세그먼트에 연결된 핀들을 O1工['PUT
모드로 선언하고 void loop() 함수에서 display卜number() 함수를 호출해 7 세그먼트에
숫자를 표시한다．



                                           3_3 7 세그먼트 구동하기 159
  .       Ard山狗 1小山




      consr jut _a=2,
      （乞flst mt _b=3;

               앞 절에서의 匹［) 켜기를 할 때와 마찬가지로 7 ＆刃FIeit와 연결된 아두이노 보드의 디지털
               출력 포트를 변수를 선언하였다. 약간의 차이가 있다면 m t 변수 선언 앞에 "const 라
                                                                "는
               예약어를 사용하였는데, 변수 선언을 할 때 데이터 타입似）잎比게 "(:(y놨"라는 예약을 붙여주
               면 0I 변수는 스케치코드에서 값을 수정하지 못하도록 제한하는 기능을 하게 된다. 스케치
               코드에서 이 변수를 수정하지 않는다면 "const" 라는 예약어는 붙이지 않아도 실행 결과는
               동일하다. +a=2라고 선언한 이유는 7 Segment 부품의 왼쪽 첫 번째 리드선0j 아두이노
               보드의 디지털 출력 포트 2번과 배선 연걸을 했기 때문이다. 나머지 변수들도 마찬가지이다．
               앞의 배선도 그림을 확인해 보기 바란다．


          m/
               O
               m 111i
                        d
                        d                  +




                                               小小
      I
               " i"라는 변수가 0부터 ]］보다 작을 때까지 증가하면서 반복해서 delay(10(刃） 함수에 의해서
               ］초 단위로 지연을 하면서 미splay_number(i) 함수를 호출하여 7 Segment 에 o, 9까지
               그리고 ". " 표시를 반복해서 출력을 하게 된다．


      실행결과

          1초 간격으로 小9까지의 숫자가 표시되고 마지막에 D아（점）이 표시가 되기를 반복하면
      정상적으로 실행이 완료된 것이다．
           연결 배선과 코드 입력에 이상이 없는데도 7 Segment어］ 숫자 표시가 올바르게 표시
      되지 않는다면 저항 연결 시 다리가 서로 SI珣奴첩촉）되지 않았는지를 확인해 본다. 필자도
      처음에 실험을 진행할 때 동작이 잘되지 않고 7 Segment의 특정 LED가 켜지지 않아서
      숫자가 제대로 표시되지 않는 현상이 발생하여 배선 연결과 스케치코드만 계속해서 검토하
      다가 결국은 7 Segment 부품 자체에 불량이 발생한줄 알고 부품까지도 교환해 보았지만
      원인은 브레드보드에 7 Segment의 리드선과 연결된 저항 들 끼리의 Shoit어］ 의해서 발생한
      사실을 거의 2시간 이상을 흔히 이야기하는 삽질 이후에 알아 차렸다．




601 제3장 디지털 입력과 출력
  3.4       버튼을 이용하여 스케치 없이 LED 제어하기


 3.2절에서 실험했딘 比D 동작을 이번에는 버튼을 이용해서 제어해 보자. 27｝땍 LED와
2개의 푸시 버튼을 브래드보드에 연결하고 첫 번째 버튼을 누르고 있으면 파란색 LED가
켜지고 버튼을 떼면 파란색 LED가 꺼지는 것이다. 2번째 버튼도 노란색 LET）어］ 대해서
마찬가지로 동작하도록 한다．
 이번 실험에서는 아두이노 개발환경에서 별도의 스케치 작업이 필요하지 않고, 순전히
회로적으로 동작하는 실험이다．


실험에 필요한 준비물들




                                                   ii
                     fl .
                             ；令9 「）. S


                            小口 1   小H1
                        .


        브래드보드 17가    아두이노 I外JOR3             파란색 , 노란색 I코Dl깨1




           年                 I
            I

                                                MM
        1K 저항 27卄      10K 저항 1개                 푸시버튼 27뀨




하드웨어 연결

 아두이노 보드에서 USB 케이블을 제거하고, 브레드보드에 2개의 푸시 버튼과 저항 I丑D
들을 연결한다．




                                                               71 1 61
                                   3.4 버튼을 이용하여 스케치 없at 匕ED 제어하:
-.   Arduino .-




                                      ［그림 +7]                     버튼을 이용한 LED 제어 배선도




                           3V3      5V         V什1


                  RESET          Aid네no                  TX/DO

                  RESET2           Uno                   RX/01

                  AREP            (Rev3)                    02

                  1아拒F                                   6E4 03
                             知d6flo I.JN0 93
                                                            04

                  AS                                    PWM 05                                                 116
                                                                                                               1 060
                  Al                                    PWM 06                               卞H         小H1m
                  AT                                        D7

                  A3                                        06               LEDI
                                                                        露S
                                                                             테ue lS2Snml
                  A4/SOA                                PWM DR

                  ASISCL                             ES/P벼M DIE
                                                                                             mmmmm小m=                  +
                                                 MOSI/PWM Oil
                                                      베SO,0俚                 LEES
                                                                             Yelow 1595n0n
                                                        506/013




                                         GND




                                         ［그림 于8] 버튼을 이용한 LED 제어회로도




62 I 제3장 디지털 입력과 출력
 푸시버튼의 가로방향의 다리는 서로 연결이 되어 있는 구조이고 버튼을 누르지 않았을
때 세로 방향의 2개의 다리가 떨어져 있다가 즉, LED의 Ano妃가 GM刈 연결되어 있다가
버튼을 누르면 세로 방향의 2개의 다리가 서로 연결이 되면서 珏D의 Anode 쪽으로 VCC（천
원）이 연결이 되면 比D의 Anode에서 Cathode 방향으로 전류가 흐르면서 LED가 켜지게
된다. 그리고 푸시 버튼의 다리에 직첩 연결된 2개의 저항에 대해서는 다음 장에서 따로
설명하도록 한다. 여기서는 그냥 풀다운 저항이라는 용어만 알아두도록 하자．




      1
          버튼을 이용하여 LEE) 처

 3.4절에서 실험했던 I코I) 동작을 이번에는 아두이노에서 버튼이 눌린 것을 디지털 입력
으로 받아서 디지털 출력으로 LED를 제어해 보자. 동작하는 방식은 이천 절에서 동작
했던 것과 동일하게 한다．


실험에 필요한 준비물들

 3.4절과 동일하다．


하드웨어 연결

 브레드보드에 2개의 푸시 버튼과 저항 I丑D들을 연결한다. 하지만 이번에는 푸시 버튼의
한쪽 다리를 아두이노보드의 12번과 13번에 연결하고 LED의 Anode를 아두이노 보드의
6번과 7번에 각각 연결한다．




                                   3.5 버튼을 이용하여 LED 제어하기 i 63
-.   Ard너no 今




                1




                              ［그림 于9] 버튼을 이용한 LED 제어 배선도




                             3V3     5V        VI


                    RESE了          Arduino


                                                      二
                    RESET2           Uno
                    AREF            (Rev3)
                    口REF
                               Arduno UNO 日3
                                                                   LED1
                                                                   Blue (525cm>


                                                                 二小如＝
                                                                    ｛嘉H小나H
                    AS                                    二，
                    Al

                    A2                                             Ye如叩 (595cm>

                    A3                               , , , DR

                    A4/SOA                           PWM DR

                    AS!SCL

                                                                                  52


                                                    " ，「
                                                       ，「‘미，「，
                                                                                  SI


                    N/（二




                                          UNO


                                           1
                              ［그림 3너0] 버튼을 이용한 LED 제어 회로도



64   제3장 디지털 입력과 출력
     위의 그림에서 첫 번짜1 푸시 버튼을 누르면 5V전원이 아두이노의 13번 포트에 연결이
되어 아두이노 스케치에서 13번 포트를 읽으면 HTGH(5V）가 읽혀질 것이고 버튼을 누르지
않으면 버튼의 다리와 GND어］ 직렬로 10K옴 저항에 의해서 LOW7} 읽혀지게 된다. 이런
저항을 Puildowm풀다운） 저항이라고 한다. 이런 풀다운 저항이 없다면 버튼을 누르지
않았을 경우에 아두이노 스케치에서 HTGI-I가 읽혀질지 L0明7} 읽혀지지 확실히 장담을
할 수가 없다. 여기서 풀다운 저항의 역할은 버튼을 누르지 않았을 경우에 아두이노보드의
13번 포트가 항상 LO明를 유지하도록 하는 역할을 해준다．


프툐二1램 작성


     mlt ledi = 7:
     mllt 1ed2 = 6;

     mllt keyl = 13;
     mllt key2 = 12;

     void setupO
     {
         pmnMode(ledl, OTJTPUT);
         pinMode(led2, OUTPUT);

         pmnMode(keyl, INPUT);
         pi小面de(key2, INPUT);
 }
 void loopO
     {
         if( digitalRead(keyl) == HIGH )
            digitalWrite(ledl, HIGH);
         else
            digitalWrite(ledl, LOW);

         if( digitalRead(key2) == HIGH )
            digitalWrite(1ed2, HIGH):
         else
            digitalWrite(1ed2, LOW);

         delay(100);
 }

                                           3.5 버튼을 이용하여 LED 제어하기 1 65
  .    Ard내no e



      加r Jedi = 刀
      hit 屯：12 = 6;

             LED들과 연결된 아두이노 보드의 디지털 출력 포트 선언


      加t keyl = ／茗
      rnr key2 = 12;
             푸시 버튼들과 연결된 아두이노 보드의 디지털 입력 포트 선언


      p亡iMode(k砂／夕 刃＼71兀／72r
      ／坑泌M民key2; 끄WI方
             LED를 제어하기 위해서는 아두이노 보드의 디지털 포트를 OUTPUT으로 설정해야 하지만
             푸시 버튼의 눌림 상태를 알71 위해서는 INPUT으로 설정하여 디지털 입력으로 해01: 한다．


      ii乙加／talR匕ad(keyl) == 丑／GH)
       （如伽加陌te(ledl, I끄GI카r
      else
        d孕노可功i北e(Iedl, LOW玄

             digitalWre() 함수와는 반대로 아두이노 보드의 만i가 IN다JT으로 설정된 포트를 읽어 오는
             함수이다. 아두이노 보드의 퍄i가 약 2V 八J5V 사이이면 HIGH이 읽어지고 그렇지 않으면
             匕Ow로 읽어진다．


      실행결과

        지금까지 디지털 출력 함수인 d增네싸rite(）를 사용하여 I코D를 (DN/OFF 하는 것까지는
      실습을 해보았다．
        이번에는 버튼 입력을 감지하기 위해서는 디지털 입력 함수인 di덥回Read(）를 사용하였
      다. digitalRead() 함수의 인자로 아두이노보드의 디지털 포트번호를 넘겨주면 아두이노보
      드의 디지털포트를 읽어서 LO明 or HIGH 중에 하나의 값을 넘겨준다．
        이번 실습에서는 버튼을 누르지 않았을 경우에는 LOW7} 읽어질 것이고 버튼을 누르면
      HIGH까 읽혀질 것이다．




661 제3장 디지털 입력과 출력
     3.6

     3.5절에서 실험했던 버튼을 누르고 있는 동안 계속해서 LED를 켜고 버튼을 누른 것을
떼었을 때 LED를 꺼지도록 LED를 제어하는 것은 약간 어색하다．
 우리 실 생활에서 일반적인 버튼의 동작은 버튼을 한번 누르면 LED가 켜지고 다시
한 번 버튼을 누르면 LED가 꺼지도록 하는 것이 좀 더 자연스럽다. 3.5절에서 작성했던
스케치를 약간 수정해서 이렇게 동작시켜 보도록 하자．


실험에 필요한 준비물들

 3.5절과 동일하다．


하드웨어 연결

 3.5절과 동일하다


 쿠그랄1 작성


 irit ledi = 7;
 jut led2 = 6;

 irLt keyl = 13;
 irtt key2 = 12:

 jut keyl status = LOW; /1 KEY1 상태
 jut key2 status = LO＼入／; // KEY2 상태

 void setupO
 {
     pinMode(ledl, OUTPUT);
     pinMode(led2, OUTPUT);

     pinMode(keyl, INPUT);
     pinMode(key2, INPUT);

     digitalWrite(ledl, LOW);




                                       3.6 버튼을 이용하여 匹D 상태 제어하기 1 67
    Arduino




          digitalWrite(1ed2, Low);
     }
     void loopO
      {
          if( digitalRead(keyl) == HIGH && keyl_status == Low)
          {
              digitalWrite(ledl, HIGH);
              keyl_status = HIGH;
          }
          else if( keyl_status == HIGH )
          {
              digitalwrite(ledl, Low);
              keyl status = Low;
          }
          if( digitalRead(key2) == HIGH && key2_status == Low)
          {
              digitalwrite(1ed2, HIGH);
              key2_status = HIGH;
          }
          else if( key2中status == HIGH )
          {
              digitalwriteQed2, Low);
              key2_status = Low;
          }
          delay(100) ;
      }


   加t key乙status = 끄71口 //K万vi 상甲
   mt 如r2万ratus = 끄)W // K万刃 상砂
                LED가 꺼져 있는 상태에서 버튼을 누르면 켜고 匹D가 켜져 있는 상태어H 버튼을 누르면
                끄기 위해서 상태 저쟝을 위해서 필요하다. 초기에는 匡D가 꺼져 있는 상태로 시작이 되기
                때문에 LOW로 초기화 하였다 ．변수 이름에 keyl, key2가 들어가서 조금 혼란스러울 수가
                있는데 key] 얹atus가 결국은 LED］의 상태를 저장하는 것이다.




681 제3장 디지털 입력과 출력
     1奸 d智亢aiRead(갚c-v刀 == ／끄GH ‘奴受 keyl_status == 끄)1I汐
     I
         a會亢a/Write伽（끄， 丑JGH);
         keyl_starus = 丑GH;
     I
               푸시 버튼］이 눌려지고 현재 LED] 이 꺼져 있으면 LED］을 켜고 LED] 의 상태를 니GH로
               변경한다．


     else if ( keyl_status == HIGH)
     I
         （如亢a川仕印cdl夕 工ow；七
         k印／_status = 끄71i乃
     I
               반대로 푸시 버튼］이 눌려지고 匹D] 이 켜져 있으면 匡미을 끄고 상탸를 LO로 변경한다．
               if 문장0似l key］卄status == 네GH를 비교하는 문장이 생략되었지만 결과는 동일하다．


     실행결과

         버튼1을 한 번 누르면 I묘끄이 켜지고 다시 한 번 버튼을 누르면 LED1이 꺼진다. 버튼2와
     I丑D2어］ 대해서도 동일하게 동작한다．



                  凹客三二nmmn心m冬二m=mmmmn炙出＝nnn:mm쯔如n크＝二 1n小小＝ 1


         3.7      부저（Buzzer) 울리기


         제어하는 방법은 굉장히 단순하지만 우리의 일상생활에서 부저는 굉장히 광범위하게
사용되고 있다. TV, 세탁기， 에어컨 둥에서 사arm음으로 사용되기도 하고 도난 경보기，
디지털 도어 록 등에도 사용되고 있다. 디지털 출력을 이용해서 간단한 연주를 할 수도
있겠지만 이번 절에서는 단순히 부저를 제어해서 켜거나 끄는 동작을 해보자. 부저 음의
주파수를 조정하여 연주를 하는 방법은 "Chapter 5 아날로그 입력과 출력"에서 다룰 것이
다．
                                                               3.7 부저（Buzzer) 울리기 169
 1   Arduino .




     실험에 필요한 준비물들




                 아두이노 UNOR3                          수동 부저




     하드웨어 연결

      부저를 보면 27胴 리드선이 나와 있는데 아래 그림에서 짧은 선이 검은 색으로 아두이노
     보드의 GND와 연결을 하고 긴 선이 붉은 색으로 아두이노 보드의 5\/ 출력 포트에 연결을
     한다．




                                       唵

                                               V 나

                                               m
                                           口
                                           H

                                               小




                       ［그림 3-11] 부저（Buzzer) 제어 배선도




70 } 제3장 디지털 입력과 출력
                 RES됴T       Arc加'no             TX/O0
                 F琵SF12        Uno               Rx/O1
                 AREF         (Rev3)                O2
                 IO日El                         PWM（好
                          知duin口 UNO R3
                                                    O4
                 A0                            P批4 O5
                 At                            F거耐拱 （蛤

                 A2                                ｛刃
                 A3                                 t毖
                 A4／缸琅                         P邸砧 ［羚
                 AS,芯CL                       ,,pw汕 {H0
                                            ss,
                                          MOSt/P咐M Ott

                                              M冶O/Ot2

                                               S아Co倡



                   C




                          ［그림 3-12] 부저（Buzzer) 제어 회로도


 위의 그림에서 아두이노 보드의 디지털 출력 8번 포트를 HIGI늅 설정하면 부저가 울리
고 LOW로 설정하면 부저가 울리지 않게 퇸다．


 쿠그램 작성


 jut buzzer = 8;

 void setupO
 {
     pinMode(buzzer, OUTPUT);
 }
 void loopO
 {
     digitalWrite(buzzer, HIGH); II Buzzer on



                                                          3-7 부저（Buzzer) 울리기 I 71
.   Arduino .-




          delay(1000);

          digitalWrite(buzzer, LOW); 7/ Buzzer off
          delay(1000) ;
      }


    tnt buzzer = 8;
             부저와 연결된 아두이노 보드의 포트 번호


    pinMode(buzzer, OUTPU方
              부저음을 울리기 위해서 포트를 OUTPUT으로 설정


    （如北a1功北e仍uzzer, I끄GI카r 7助zzef on
    delay(1｛兀兀꺄r
              부저를 켜고 ］초를 대기한다．


    （如亢a肛l亡e（加勿er; 끄7n功 / Buzzer o序
    成切了1尻也七
              부저를 끄고 ］초를 대기한다．


    실행결과

     1초 동안 부저가 울리고 부저가 꺼졌다가 다시 1초 후에 부저가 울리기를 반복한다．
    이번 실험에서는 단순히 부저를 울리게 하거나 꺼지게 하는 실험을 해보았지만 이 후의
    Chapter에서는 약간의 연주를 해보는 실험을 진행할 것이다．




72 I 제3장 디지털 입력과 출력
시리얼（RS232) 통신


    4. ]시리얼（RS232) 통신 소개
    4.2 PC와 시리얼（RS232) 통신하기
    4.3 시리얼（RS232) 통신으로 LED 제어하기
  t   Ard내no .




        4.   1        시리얼（RS232) 통신 소개1


       RS232 통신은 주로 IBM 호환 PC에서 쓰이는 시리얼 통신방법이다. 예전에는 주로 모뎀
      연결에 RS232통신을 많이 사용하였지만 요즈음에는 컴퓨터를 센서 또는 계측기 컨트롤
      등 여러 용도로 RS232를 사용하고 있다. RS232 통신은 최장 15m 정도까지 통신 가능하므로－
      15m 이상이 되는 거리에서는 RS232 통신이 불가능하다．
       Desktop PC은 아직도 RS232 통신포트를 가지고 있는 PC들이 많이 있지만 최근의 노트
      북 PC들은 두께, 무게 등을 줄이기 위해서 RS232 포트를 없애고 있는 추세이다. 아두이노는
      보드에서 기본으로 제공하는 USB포트를 이용해서 PC 혹은 다른 장비, 다른 아두이노 보드
      와 RS232 통신을 할 수 있다．
       아두이노를 PC의 USB장치와 연결을 하게 되면 아래 그림과 같이 장치관리자에 가상
      COM 포트가 만들어지기 때문에 가눙한 것이다．


             器也                                                 :J;      1夕므如hm可

             心1捕肖可＝夕嗽肉



                                                                             11
                                                                               屬； 二
                 密 컴퓨터 관리（로걸）
                 a 豁 시스탬 도구
                   !> 四 작업 스神줄러
                   b 國 이밴트 뷰머                                                        )JEF.
                                                                                         ..




                   b 我 공유 폴더
                   口 毋 로걸 사용자 및 그룹
                   !> 匈 섬늠
                      好 장치 관리자
                 4 齒 저잠소
                      岩 디스크 관리
                 , 融 서비스 및 읗용 프로그렴


                                      11 ! h堂LJSB Serial Port（叩M7)
                                               小甲 보트（COM & LP)
                                               i i1孕An仙no마幻(COM9) }          育큽1n1               重
                                      1        三；骨 USB Sen체 p0rt(COMa)       多!
                                      i        莎1 프로At서                      卞 1

                                        薑玉芷堪蝨"
                                     卜 雌：                                ,     !                 至
                                                                                                 立
             뇨      小山 d가                 1느          H亐                                      mm=2


                            ［그림 午］I       Windows 7에서의 아두이노 COM 포트




74 I 제4장 시리얼(RS232) 통신
                                                               多


           ［그림 午2] 아두이노 UNO R3의 가상 COM 포트 기능


 앞에서도 한번 설명했지만 장치관리자를 실행하는 방법이다．


 四n
 Windows 환경에서 장치관리자를 실행하는 방법은 실행메뉴（Windows+R）에서 devmnlt.msc를
 입력한 후 Enter를 누르면 된다．




 PC어］ 가상 COM포트가 올라오도록 하기 위해서는 아래 그림과 같이 USB 케이블을
이용해서 PC와 연결을 해야 한다. 물론 연결만 해서 끝나는 것은 아니고 아두이노 USB
장치 드라이버도 설치를 해야 한다. USB 드라이버 설치에 관한 내용은 Chapterl에서 자세
히 설명을 하였으니 참조하기 바란다．




             ［그림 午3] Ard네n(그 UNO R3와 PC의 USB 연결




                                            4. ]   시리얼（RS232) 통신 소개 I 75
  .   Ard山狗 11




       4.2          PC와 시리얼（RS232) 통신하기


       아두이노 보드에서 USB 케이블로 연결을 하고 RS232 통신으로 데이터를 주고받는 실습
      을 해볼 것이다．
       PC와 통신을 하려면 PC어］ 터미널 프로그램이 있어야 하는데 아두이노 개발환경에는
      이미 PC와 통신을 하기 위한 터미널 프로그램이 갖추어져 있다. 자세한 사항은 이번 절의
      "실행결과" 확인할 때 알아보도록 하자．
       아두이노에서는 RS232통신으로 데이터가 오기를 기다리고 있다가 데이터가 도착을 하면
      도착한 데이티를 곧바로 PC로 재전송하는 실험을 해보자. 여기서 아두이노 입장에서 생각
      해 보면 PC에서 데이터가 도착하는 것을 EX데이터라고 하고, 아두이노 보드에서 PC로
      데이터를 전송하는 것을 D ( 데이터라고 한다．


      실험에 필요한 준비물들

       이번 실험에서는 별다른 준비물은 필요하지 않다. 아두이노 보드와 PC가 USB 장치로
      올바르게 연결만 되어 있으면 된다．


      하드웨어 연결

       하드웨어 연결은 필요하지 않다. 아두이노 보드와 PC를 USB 장치로 연결한 다음 장치관
      리자에 가상 COM 포트가 제대로 올라왔다면 이상 없이 연결이 된 것이다．


      끄쿠기램 작성


       void setupO
       {
           Serial.begin(9600);
       }

       void loopO
       {
           char read data;


           if (Serial. available0)



76 1 제4장 시리얼（RS232) 통신
          read data = Serial.read0;
          Serial.print(read_data);
      }
      delay(10) :
  }


Sen뇨Lb啣ui凹m까r
           setu口（) 함수에서 Sen졔．t冶qn() 함수를 호출하였다. 이 함수의 역할은 아두이노보드가
           RS232 통신을 할 수 있도록 통신 설정을 초기화하는 역할을 한다. 괄호안의 9600이라는
           숫자는 통신 속도를 나타내는 것이다. 9600은 9600bps（日tPer Seconds）로 초당 9600b1t
           의 데이터를 송신할 수 있는 것이다. 이번 예제에서는 앉XXX耳月로 통신을 하였지만 이외어도
           많이 사용하는 통신 속도로 384C 力四, 1152C 力四 등도 많이 사용이 된다. 당연히 숫자가
           클수록 통신 속도가 빠르다. 만약 9600 이외의 다른 통신 속도로 설정하였다면 아두이노
           시리얼 모니터 프로그램어I) 도 통신 속도를 동일하게 설정을 해야 한다. 아두이노 개발환경
           에서 시리얼 모니터를 실행하는 방법은 이 Cha아아의 실행결과 부분을 참조하면 된다．


S匕F'뇨／.available（方

           이 함수는 수신된 시리얼 데이터의 개수를 반환하는 역할을 한다. 즉 함수의 반환 값이
           0보다 크다면 뭔가 시리얼 데이터가 수신이 되었다는 것이다．


Serial.readO,

           수신된 시리얼 데이터 ] 바이트를 읽어伯x) 온다. 스케치어I)'1 read_da怡 二二Sen톄.read(）라고
           작성을 하면 수신된 시리얼 데이터 ］바이트를 read da冶 변수에 저장하라는 의미이다．


Serial.pi力it（卜eadJ屯ta方
           이 함수는 read data라는 byte 데이터를 시리얼로 전송n지을 하는 함수이다．


실행결과
                             米 客？뀜 읖험후 卵陀 흘耳
  아두이노 개발환경에서 아래1 그림과 같은 아두이노 시리얼 모니터 아이콘을 클릭한다．


           0 回目目「

                                                  4.2 1거二와 시리얼（艮3232) 통신하기 I 77
  .   Arduino



       그러면 아두이노 개발환경의 시리얼 모니터 프로그램이 실행이 된다. 시리얼 모니터
      화면의 "Send" 버튼의 왼쪽 입력박스에서 PC의 키보드를 이용해서 아무 문자나 입력을
      하고 "Send" 버튼을 눌러보자. 입력한 문자가 그대로 시리얼 모니터 창에 표시가 된다면
      올바르게 실행이 완료된 것이다. 아래 그림처럼 " Send" 입력 박스에 "Hello Arduino."
      라고 입력한다. 그리고 반드시 ' 96（그0 baud"를 선택해야 한다. 통신 속도를 다르거］ 설정하면
      통신이 되더라고 올바르지 않은 데이터들이 송수신 된다.


                         回coM:6                              1：小尸 1能如，可 ;:,,: m厄的미
                                                                                                                II




                1
                                                                                                     Send
                                             n이
                卜ello』            『山.
                                                                                                            1
                                                                                                            ,



                望 望Aut口' croll                                        "
                必目澍注介蜘寸螂朴小                   斗升 n> nn   也毋
                                                                                      『9600       baud

                                        ［그림 午4] 아두이노 시리얼 통신 실행 결과 창


      "Send"창에 "Hello Arduino"라고 입력한 이후에 "Send" 버튼을 누른다．


                                        二口                                                                           mm




                                                                                                  L..』無烈m二
                         Ilel lo Arduino




                          ' '4尹「 A마Os尸．r口II                        Cardage return !           므600 baud


                                        ［그림 午5] 아두이노 시리얼 통신 실행 결과 창




78 I 제4장 시리얼（RS232) 통신
                                                            砬


  42     시리얼（RS232) 통신으로 LED 제어하기


 시리얼 통신을 이용해서 PC（아두이노 시리얼 모니터）에서 아두이노어］ 연결된 2개의
I코DOn／아f 상태를 표시하고 시리얼 모니터에서 "1"을 입력하면 첫 번째 I코D가 켜져
있으면 끄고 꺼져 있으면 켜는 실습을 해보도록 하자. 두 번째 I코D도 첫 번째 I코D와
마찬가지로 ' 2"를 입력하면 동일하게 동작하도록 한다．
 이번 예제는 ' 3.6 버튼을 이용하여 I코I) 상태제어하기"의 2번째 예제와 유사하다. 단지
I코I) 상태 제어를 버튼이 아닌 시리얼 통신의 입력으로 제어한다는 차이만 있다．


실험에 필요한 준비물들

                                   = =   1


                                              ; GX9   m t



                                         11     中小


          브래드보드 1깨1                아두이노 1꾜寸OR3




                                             亨
            茹舛       叫




            I   '1   fl
       파란색 , 노란색 LED 17뀨                 11( 저항 2개1



하드웨어 연결

 아래 LED제어 배선도의 그림을 참조하여 브러1드보드에 저항과 LED들을 연결한다．




                               4.3 시리얼（RS232) 통신으로 匡0 제어하기 1 79
    Arc｝내no




                                1
              1
                                1
              1

              1   1

              1   !



              1   !

              1   1

              1   1

              年       4

              1       1




                                   ［그림 午6]            시리얼 통신으로 LED 제어하기 배선도




                                     33    5V       너N


                          F三SET           Arduino            rX/D0
                          nESET2            Uno              nX/D1
                          ：日EF             (Rev3)              。2
                          好角EF        A川U',口08093          F斗91,寸03
                                                                04
                  H
                          月0                               PWYOS

                  H       Al                               PWM06
                                                                          乏ED2
                          缶2                                    07        YULW r1,澍n1끼）   .

                          首，j

                          二4冬0A
                                                                08

                                                           PWM 09
                                                                      H
                                                                          .4肛Hm小 .
                          n5/ SC                         S$伊WM 010

                                                      以冷甘p出M ［기 1

                                                          베so/a 侄

                                                           SCK汪기3 m




                                                080


                                                I
                                    ［그림 午7] 시리얼 통신으로 LED 제어하71 회로도




80 ! 제4장 시리얼（RS232) 통신
쿠기램 작성


mtlt ledi 二二 7;
mllt 1ed2 = 6;

jut ledi status = LO＼入／; // LED1 상태
jut led2 status = Low; II LED2 상태

void setupO
{
    pinMode(ledl, OUTPUT);
    pinMode(1ed2, OUTPUT);

    digitalwrite(ledl, LoW)
    digitalWrite(led2, Low);

    Serial begin(9600) ;
}
void loopO
{
    char read data;

    if (Serial. availableO)
    {
        read data = Serial.readO;

        if( read_data == '1' && ledi status == Low)
        {
            digitalwrite(ledl, HIGH);
            ledi status = HIGH;
            Serial.printlnC'LEDl ON");
        }
        else if( read data == '1' && ledi status == HIGH )
        {
            digitalwrite(ledl, Low);
            ledi status = LOW;
            Serial. printlnC'LEDl OFF");
        }
        if( read_data == '2' && led2 status == Low)



                                                  4.3 시리얼（RS232) 통신으로 LED 제어하기 I 81
   Ard내no .-




             {
                 小gitalWrite(led2, HIGH);
                 1ed2 status = HIGH;
                 Serial.println("LED2 0N");
             }
             else if( read_data == '2' && 1ed2小status == HIGH )
             {
                 digitalWrite(led2, Low);
                 1ed2 status = Low;
                 Serial.pr毗ln("I皿Dl 0F그F") ;
             }
         }
         delay(10) ;
     }



   力it Jedi = 刀
   加t led2 := 回
                 브레＝부二（게 있는 LED와 연결된 아두이노보드의 포트 번호0따．


   加t 奴江status = 끄71材 // 工皿刀 챵印
   立It 奴／2_status = 끄71材／그끄刃 샹甲
                 匕ED］과 匡D2를 시리얼 통신 입력으로 들｛거오는 데이터 " 1" or "2"에 따라서 에과 0FF의
                 상태를 유지시켜주71 위한 상태 변수이다．


   戶mM改兆伽山， OUTPUT);
   ／功小10(屯ied2, OLTTPUI方

                 LED］과 LED2를 제어하기 위해서 아두이노 포트를 0UTPUT으로 초기화 한다．


    d會亢a加必北e口氏11, 끄7Vr7;
    d會亢aiWi亢C口h妃 끄)斗玄
                  초기에 LED］과 匹D2를 꺼진 상태에사실행하기 위해서 L0W 값으로 Write 하였다．


       . begin幼ZM七
    品I血／
                  통신 속도를 9600b四로 초기화한다．



82 I 제4장 시리얼（RS232) 통신
    5匕i屯Lava끄拍帖0

          이 함수는 수신된 시리얼 데이터의 개수를 반환하는 역할을 한다. 즉 함수의 반환 값이
          0보다 크다면 뭔가 시리얼 데이터가 수신이 되었다는 것이다．


．免riaL read口

         수신된 시리얼 데이터 ］바이트를 읽어伯x) 온다. 스케치에서 read da伯 = Serial.rea北라고
         작성을 하면 수신된 시리얼 데이터 ］바이트를 read_data 변수에 저장하라는 의미이다．


11
 ( read data       /// 1奴景 /edl_stat끄S == 끄71影）
I
     d智亡a/Wi亡e俯끄，I끄G刊； /／工方Z刃을 켠다．
     led1_ status = 丑!GI君／工끄刀9 장印룰 刃침 샹球르 万장 한다．
     SerJaLp.加山寸7玉Z刃 （기V切
I
         수신된 데이터가 ' l ' 이고 현재 LED1으J 상태가 꺼져 있으면 LE미을 켜야 한다. 그리고
         Serial.口nfl卄n("匹Dl 0N') 라는 함수가 등장하였는데, Sen톄.口nint() 함수와의 차이점은 시리얼
         포트로 문자열을 출력하고 이후에 줄 바꿈 문쟈（"C다F"）를 자동으로 출력하는 기능이 있는
         함수이다. 아두이노 시리얼 모니터어因 줄을 바꾸어서 출력을 하기 위해서는 Sen톄,pnintln()
         함수를 사용하면 된다．


else if ( read data == 'I ' && ledi_status == HIGH)
I
    dA卽切1比北e伽dl, 끄7W玄 /／工끄刀골 끈다．
    ledl_srarus = 工O1材 /／工끄刃와 장印릍 꺼짚 상球로 저장한다．
          ．戶i出끄加但万Z刃 口下切
     5匕i낏뇨／

I
         수신된 데이터가 ' ] '이고 현재 LED］의 상태가 이미 켜져 있으면 匕ED］을 꺼야 한다．




                                                  4-3 시리얼（RS232) 통신으로 匡D 제어하기 1 83
.   Arduino




    실행결과

     아두이노 개발환경에서 아래 그림과 같은 아두이노 시리얼 모니터 아이콘을 클릭한다．




     그러면 아두이노 개발환경의 시리얼 모니티 프로그램이 실행이 된다. 사리얼 모니터
    화면의 "Send" 버튼의 왼쪽 입력박스에서 PC의 키보드를 이용해서 "1"과 " 2"를 눌러서
    브래드보드에 있는 LEI）의 상태가 바뀌는지를 테스트해보자．


                                       二，
                                            nh，丁
                                                                                    1
                                                                                        口口   回 枷昌m
              口
              1                                                                              珏筵｝1
                          LEDI ON                                                                      t1
                          LE01 0FF
                  1LE02
                               0N

                          LEft
                          LE01 0FF




                    1      m翔幻scroll
                                                              (Thrri-aye return 甲       므60［比aud   !        i
                                                   尸




                                            ［그림 午8] 시리얼 통신으로 LED 제어하기 실행 결과 창




841 제4장 시리얼（RS232) 통신
아날로그 입력과 출력

    5.1 펄스中WM）로 LED 밝기 조절하기
    5.2 펄스向시）로 부저（Buzzer)로 연주하71
    5.3 가변저항 값 읽어오기
    5.4 테스터기 흉내 1 전압 값 읽기
 .   Arduino .-



      Chapter 3에서는 디지털 입력과 출력에 대해서 살펴보았다. 이번 Cha아er에서는 아날로
     그 입력과 출력에 대해서 직접 실험을 통해서 공부해 보자．
      이전 Chapter에서는 단순히 ON, OFF 27胴 상태만 갖도록 제어를 했다면 아두이노
     보드의 P瓜4 출력 포트를 이용하면 부저와 珏l居 좀 더 멋지게 제어할 수 있다. 아두이노
     의 아날로그 입력과 출력을 이용하면 0---1023 즉 1024단계로 세밀하게 제어할 수 있다．
     아날로그 출력은 PWM 기능을 이용한다면 아날로그 입력은 전문적인 용어를 사용한다면
     ADC 기능을 이용하는 것이다. 자세한 사항은 실제 실험에서 다시 설명하도록 한다．




       5.1        펄스（PWM）로 LED 밝기 조절하기


      "3.2 I코I) 깜빡이기" 에서는 아두이노 보드에 연결된 I코D를 단순히 켜졌다 꺼졌다를
     반복하게 하여 깜빡이도록 하였지만 이번에는 Pw入4(Pulse 싸idth 入4odulation）기능을 이용
     하여 LED의 밝기를 조절해 보자．
      P明M은 펄스 폭 변조라는 말로 펄스폭을 조절해서 전류를 조청한다는 의미이다. · 이
     기능을 잘 이용하면 이용가능한 분야가 굉장히 많다. 스마트 폰에서조도 센서를 이용해서
     주변 밝기에 따라서 LCD의 백라이트를 PWM으로 조정하여 전원을 절약하는 기능을 가지
     고 있고 집안에 있는 간단한 무드 등을 제어하는 경우에도 이용할 수가 있다．
      아두이노 보드에서는 3, 5, 6, 9, 10, 11번 핀을 an丑ogWi挑e(0-255）라는 함수를 이용해
     서 pw八4 출력으로 사용할 수가 있다. 아두이노 하드웨어의 실크 인쇄된 부분의 출력 핀에
     aN " 모양으로 일반 디지털 I/O 핀과 구분을 하고 있다.
       다음 그림의 아두이노 보드에서 붉은색 네모 박스 안에 위치한 포트들이 PWM 출력
     기능을 가지는 포트들이다．




861 제5장 아날로그 입력과 출력
          ［그림 于］] 아두이노의 Pw卜月 출력 포트


                 Pulse Width Modulation
              0% Duty Cycle - analogWrite(0)
  5v

 0v




             50% DutyCycle- a         ite(127)




                  uty Cycle 皿 ana佃gWrite(191)




7
<
           100% Duty Cycle m analogWrite(255)
    V

 V
 0


［그림 于2I PW卜A 파형（http ://arduino cc/en/Tutori줴／Pw卜川 참조




                                        5. ]   펄스（다N卜가로 LED 밝기 조절하기 1 87
 .   Ard山狗 1




      아두이노에서는 ana1og玎rite() 함수를 이용해서 小255 사이의 값을 아두이노 보드의
     P勺V入l출력 포트로 출력을 시킬 수 있다．
      위의 그림을 보면 analogWrite() 함수에서 0, 64, 127, 191, 255 순으로 출력을 하였을
     경우에 출력되는 실제 파형을 오실쿠入극I立 장비를 이용해서 출력한 모양이다. 중간 값
     127을 사용하면 LOW, HIGH 의 구간이 동일한 비율을 가지는 펄스를 출력하고 64를 사용
     하면 HIGH인 구간이     25%, LC）叫 구간이 75％를 차지하는 펄스를 출력한다.
     an코og찌rite(255）를 사용하면 일반 디지털 LO에서 HIGH를 준 것과 동일하다. 比D 제어를
     할 때 일반 디지털 I/O에서 ON：과 OFF로만 제어할 수 있었지만 PWM 기능을 이용하면
     Duty Cycle어］ 의해서 LED를 밝기를 조정할 수 있다．


     실험에 필요한 준비물들




                  卄
               브래드보드 17뀨                     아두이노 UNO R3




                 적색 LED                        11( 저항 17가




     하드웨어 연결

      아래 도면을 참조해서 I五D와 저항을 아두이노 보드의 P사VM출력 기눙이 있는 11刃 포트에
     연결한다．




881 제5장 아날로그 입력과 출력
         1


     1




［그림 于3]                    펄스（Pw卜川으로 匕E[）밝71 조절하기 배선도


             I
             3V3
                      I
                      5V
                                 I
                                 V씨


RESET              사duino                 TX/DO

F1ESET2             Uno                   RX/Dl

A日OF               (Rev3)                    D2

010SF                                    P나너 03
               사dwr,o UN（그 103
                                             04

AD                                       PWM 05

Al                                       P넥M DO

A2                                           D7

A3                                           08

A4/SDA                                   P바M 09
                                                          LE［기
AS/Sd[                                SS/P넥M 010          Red (633nn)
                                  MOSI/PWM 011

                                       MISO/012

                                         SCK/013



N/C




                           GND


                            1
                                                                 fntzing

［그림 于4] 펄스（Pw卜A)으로 LED밝기 조절하기 회로도



                                                   5.1   펄스（帥M）로 L三D 밝71 조절하기 189
小＋ Ard내no 1




     쿠기램 작성

     아두이노 스케치에 아래와 같은 코드를 작성한다．


     ／水
              Fade

              This example shows how to fade an LED on pin 9
              using the analogWriteO function.

              This example code is in the public domain.
      水／
     mllt led = 9;                II the pin that the LED is attached to
     m1lt brightness = 0;         II how bright the LED is
     mllt fadeA均unt = 5;           II how many points to fade the LED by

     II the setup routine runs once when you press reset:
     void setupO {
       II declare pin 9 to be an output:
       pinMode(led, OUTPUT);
      }
     II the loop routine runs over and over again forever:
     void loopO
          {
              II set the brightness of pin 9:
              analogWrite(led, brightness);

              // change the brightness for next time through the loop:
              brightness = brightness + fadeAmount;

              II reverse the direction of the fading at the ends of the fade:
              if (brightness == 0 I I brightness == 255) {
                  fadeAmount = -fadeAmount ;
              }
              II wait for 30 milliseconds to see the dimming effect
              delay(30);
          }

9O1 제5장 아날로그 입력과 출력
    力it lel = 9,.

             LED와 연결된 아두이노 보드의 다N卜기 출력 포트 번호


    力it br侈加ness = i考

             an톄四Write() 함수를 이용해서 0 "-' 255 사이의 값으로 출력할 변수이다. 이 변수의 값을
             조정하면 LED의 밝기를 조정 할 수 있다. 변수의 값을 0으로 하면 LED가 꺼지게 되고
             255 값으로 하면 가장 밝게 켜지게 되고 ]28 값으로 하면 중간 밝기로 켜진다．


    Jut 辰deAmot끄It = 多J'

             delay(30) 에 의해서 30msec 단위로 밝아지거나 어두워지는 단계를 조정하는 변수이다．
             이 값이 크면 클수록 빨리 밝아졌다가 어두워지게 된다．


    尸ihJ五ide(led, OUT]兀／T);

             다A기 출력 모드로 사용하는 경우이도 아두이노 보드의 포트를 반드시（刃TR兀으로 설정해
             야 한다．


    ana／四Wr亢印ed, br唾功m7ess方

             실제로 아두이노 보드의 출력 포트를 통해서 Pw卜기 신호를 출력시키는 함수이다．


1   bi會加ness = br會／7tness + ／自比Amoun乙‘

             LED의 밝7롤 fadeAmount 만큼 조정하는 코드이다．


    if (I뇨智加ness == 0 // bi智加ness == 25刃 /
        ／自d匕4／끄01끄it = m／自deA／吼)uflt ;

    I
             만약 밝기가 가장 어두워지거나 밝아지면 반대로 하기 위해서 f刻eknount 변수의 부호를
             바꿔주고 있다．


    delay侈U方

             30msec 단위로 LED의 밝기를 조정하기 위하Pd 필요하다．


        위의 코드는 아두이노 튜토리얼 페이지（http://arduino.cc/en/Tutorial/Fade）에서 코드
    를 참조하였다．




                                               5. ]   펄스（뎌사뻬로 匡D 밝기 조절하71 I 91
  .   Ard내no 1 -




      실행결과

       I丑D의 밝기가 심장이 뛰는 것처럼 처음에 어두운 상태에서 점점 밝아졌다가 가장 밝아진
      이후에는 다시 서서히 어두워지고 가장 어두워진 이후에는 다시 서서히 밝아지기를 반복하
      게 퇸다．




        5.2            펄스（PWM）로 부저（Buzzer) 연주하기


       "3.7절 부저（Buzzer) 울리기" 실험에서는 단순히 부저를 켜거나 끄는 실습을 했지만
      이번에는 P硼M 출력을 이용해서 부저를 제어해서 간단한 연주를 해보자．


      실험에 필요한 준비물들


                       S 1      L ,1

                   量       「；今今侄西．1                  難
                       玉   ;




                               11; 向布 小11



                       아두이노 UNOR3                  수동 부저




                               系
                   S8050 NPN 트랜지스터 1가1
                                                     亨
                                                  10K 저항 17뀨




      하드웨어 연결

       아래 배선도를 참조해서 부저와 트랜지스터 , 저항을 연결한다. 반드시 트랜지스터의
      베이스 핀을 아두이노 보드의 8번 포트에 연결을 해야 한다. 트랜지스터 부품은 처음으로
      등장했는데 자세히 알아보자．



92 I 제5장 아날로그 입력과 출력
［그림 도5]            펄스（Pw卜川으로 부저 연주하기 배선도




             3V3     5V        VIN

 RESET             Arduino               TX/D0                           H




 RESET2              Uno                 RX/Dl                           H




 A日EF               (Rev3)                 D2                            1



                                                                         1
  OREF         Arduin。UNO R3
               ArdUn0UNOn3              PWM O3
                                            O4                           1




 AD                                     PWM D5                           1




 Al
                                                        茫U
                                        PWMD6                            H




 A2                                         07                           1




 A3                                         D8
 A4/SDA                                 PWM D0               Cl
  A.5/SCL.                           SS/PWM DiD

                                 MO텨／PWM O11
                                      M1001012

                                        SCK/O13



 N/C




                          ON




［그림 于6]            펄스（Pw卜川으로 부저 연주하기 회로도


                                                  5.2 펄스（PWM)로 부저（Buzzer) 연주하71 1 93
 -. Arduino .



       트랜지스터에는 PNP, NPN의 2가지 종류가 있다. 2개의 차이점은 PNP형은 베이스에서
   이미터보다 낮은 전압을 걸어 주면 전류가 이미터에서 컬렉터로 흐르게 되고 NT八형은
   베이스에 이미터보다 높은 전압을 걸어 주게 되면 전류는 컬렉터에서 이미터로 흐르게
   된다. 결론적으로 베이스에 이미터보다 낮은 전압을 가하느냐 높은 전압을 가해주느냐에
   따라 작동이 되느냐, 안되느냐의 차이점이다. 역시 말로는 설명이 어려워진다. 자세한
   내용은 아래 그림을 참고하기 바란다．




       NPN 트랜지스터와 PM) 트랜지스티의 동작


                                            NPN 트 래 지 스 Ej

                           C이lector                      Em浪er am
                      5V          +



                                            If ( Base젼압 > Em吐ter 전압 ) Then
                                                Collector + 타州姓er 로 젼류7F 흐름

                                            PNP 트랜지스El

                           Emitter



                                                         " "" ' "『
                                                 妊
                                      ：우P
                                            If ( Base전압 < Em仕ter전맙 ) Then
                                                En恤ter-* CoIl缸tor 로 전류가 흐름

   \




941 제5장 아날로그 입력과 출력
프로그램 작성


  mllt speakerPin = 8;

  mllt numTones = 10;
  m1lt tones[ ] = {261, 277, 294, 311, 330, 349, 370, 392, 415, 440}
  // mid C C# D D# E F 1津 G （겪羊 A

  void setupO
  {
  }
  void loopO
  {
      for (mlt i = 0; i < numTones; i++)
      {
          tone(speakerPin, tones[ii);
          delay(500) ;
      }
      noTone(speakerPin) ;

      delay(1000) ;
  }


 이 예제 코드를 완벽하게 이해하기는 쉽지 않다．
  C 언어에서의 배열이라는 자료 구조와 함께 여러 가지를 알아야 한다. 책의 머리말
에서도 언급했듯이 이 책의 집필 의도는 이러한 복잡한 공학적인 내용을 설명하려고 하는
것이기 아니기 때문에 C 언어에 대한 자세한 설명보다는 동작에 대한 끼초 원리와 아두이노
에서 어떻게 이것을 활용할 수 있는가에 초점을 맞추었기 때문어］ 핵심적인 함수의 역할에
대해서만 설명하고자 한다. 특정 음을 연주하기 위해서는 주파수를 정해주어야 한다. 각칵
의 음은 서로 다른 주파수를 가지고 있고 배열에 저장이 되어 있다. 배열에 있는 음읕
순서대로 연수하면 음계를 연주할 수 있다．


加r speaker／功2 = 8;
           스피커에 연결된 아두이노 보드의 출력 포트번호




                                                    52 펄스（F긔M)로 부저（B.皿er) 연주하71 I 95
         Ar:｝내no




     m t ft刃rnT끄肥S = ／그
     加t tones끄 = 仁61, 277, 乃i; 311, 33／工 319, 370, 39乙 4乃， 4乳功
                   소리 음계 데이터를 가지고 있는 배열 자료 구조


     [or (m7t I = 0; 1 (nuniTones; 1# #)
     I
          tone(speaker功l, ronesflJ);
          delay乃00七
     I
                   for I茯）p문에서 각각의 음은 tone［居 사용하여 연주를 하게된다. 아두이노 함수 tone(）은
                   두 개의 파라미터를 가지는데 처음 긺은 부저와 연결된 아두이노 출력 포트 번호이고 다른
                   것은 플레이할 음의 주파수 데이터이다．


     noTone(speaker／功2方
                   모든 음이 연주가 되면 noTone() 함수에 의해서 현재 연주되고 있는 음을 멈추711 된다．


          위의 스케치 코드는 http://arduino.cc/en/Tutori키月one어］ 있는 예제를 참조하여 작성
     하였다．


     실행결과

          실행을 시켜보면 8개의 다른 주파수를 갖는 음계가 연주가 되고 1초 후에 이 연주를
     계속해서 반복하게 된다. 아래 그림은 아두이노 보드의 출력에서부터 부저를 거쳐서 실제
     로 사람의 퀴에까지 데이터가 생성되는 경로를 그림으로 표현해 보았다．




                          아두이노 출력
                                                            r\ r

                                             Buzzer


                         ［그림 5-7] 디지털 출력0私d 아날로그 변환까지의 경로




%1       제5장 아날로그 입력과 출력
  5.3   가변저항 값 읽어오기


 지금까지 아두이노의 아날로그 출력에 대한 실험을 해보았다. 지금부터는 아두이노의
아날로그 입력 기능에 대한 실습을 해보도록 하자．
 아날로그 입력을 벋아들이기 위해서는 공학적으로는 ABC（帥alog Digital Con比凡er）라
는 기눙을 이용하는 것이다. ADC란 연속척인 신호인 아날로그 신호를 부호화된 디지털
신호로 변환하는 장치를 뜻한다. 이러한 ADC는 온도, 압력, 음성, 영상신호, 천압 등을
실생활에서 연속척인 아날로그 신호를 측정하여 그 신호를 컴퓨터로 입력하고 디지털로
변화하는 장치이다．




                    ［그림 도8]   A/D, D/A 변환




 이번 실험에서는 가변 저항의 저항 값을 읽어서 저항 값에 따라서 比D의 밝기를 제어하
는 실험을 해볼 것이다．


실험에 필요한 준비물들




        브래드보드 1개1                           아두이노 UNO R3




                                                 5.3 가변저항 값 읽어오기 I 97
    Ard내no .




                卄
               적색 LED/1K 저항 2개
                                             I
                                            가변저항 17뀨




   하드웨어 연결

     珏D를 연결하는 방법은 이제 익숙해졌을 것이다. 가변저항은 리드선이 3개가 나와 있는
   더］ 우선 가운데 리드선을 아두이노 보드의 아날로그 입력 기능이 있는 AO 포트에 연결한다．
   그리고 나머지 왼쪽과 오른쪽 리드선에는 GND와 vcc를 연결하면 된다. 왼쪽과 오른쪽
   구분 없이 그냥 연결하면 된다. 배선도를 확인해 가면서 연결을 하자. 그리고 아두이노
   보드는 디지털 포트와 분리하여 아날로그 입력 포트를 배치하였다．




                       ［그림 도9] 아두이노의 아날로그 입력 포트


     위의 그림에서 붉은색 녜모 박스 안에 위치한 포트들이 아날로그 입력 기능을 가지는
   포트들이다．




981 제5장 아날로그 입력과 출력
  ［그림 于］0]               가변저항 값 읽어오기 배선도




            1
           3813    581
                              1
                             yIN


RESET             사duino                 TX/DO
日ESET2             Uno                  RX/Dl
AREF              (Rev3)                    02
iOREF                                 PWM 03
             却9U1n0 U神O 日3
                                            04
40                                    PW4 05
Al                                    84811.1 DS                         H



'42                                         07                           m



'43                                         08                           놔



84/SOA                                PW1.4 09                           e



A5/ SC L                           SS/PWM 010                            H




                              MOSI/PWM oil
                                    PA怜이01?

                                     SCK/017



Sic




                     （카바）


                         1
［그림 于］]]                 가변저항 값 읽어오기 회로도



                                                   5-3 가변저항 값 읽어오기 199
  .   Ard내no



      끄쿠기램 작성

       아두이노 스케치에 아래와 같은 코드를 작성한다．


        m1lt sensorPin = A0;             II select the input pin for the potentiometer
        mllt led = 9;                   II the pin that the LED is attached to

        II the setup routine runs once when you press reset:
         void setupO
            {
                II declare pin 9 to be an output:
                 pinMode(led, OUTPUT);

                 Serial.begin(9600);
            }
        II the loop routine runs over and over again forever:
        void loopO
        {
                m1lt sensorValue = 0;

                II read the value from variable resistence
                sensorValue = analogRead(sensorPin);

                analogWrite(led, sensorValue);
                Serial.println(sensorValue) ;

                II wait for 10 milliseconds to see the dimming effect
                delay(10) ;
        }


      加t sensorPin = A｛考               // select t力e 加刃Ut pin for t方e／刃ten餉／neter
                   가변저항의 가운데 리드선과 연결된 아두0注 보드의 아날로그 입력 핀 번호


      亡it led = (考                     // the pin z力at 功e 工石Di뇨 atta（方ed to

                    LED와 연결된 아두이노 보드의 다／呱기 출력 핀 번호




1以） 1 제5장 아날로그 입력과 출력
／功iMo佃左d, OUTPU7方

       F꺼／\／卜,1 출력을 내보내기 위해서 0UTPUT으로 설정


5匕ri뇨／.b（召in(9t冽；

       가변저항에서 읽은 값을 아두이노 시리얼 모니터에 표현하기 위해서 초기화


sensor1自／Lie = anal岫和ad伽仍or／亐h方

       아두이노는 an톄（지Read() 함수를 이용해서 아날로그 데이터를 디지털로 변횐（A[X＞한 데이
       터를 읽어 올 수가 있다. 아두이노의 tx二 변환 장치의 범위는 0勺伯23까지이다. 즉 ］어而의
       Res이U化n을 가지는 AD0 변환기를 가지고 있는 것이다. 그러므로 an톄ogRead() 함수를
       0 용해서 아날로그 데이터를 읽으면 항상 小71023 사이의 값을 리턴하1 준다．


analogWrite伽d, sensor'白／ue方

       가변저항에서 읽어온 0' 1023의 값으로 LED의 밝기를 조정하고 있다．


Set勿／
    ．戶i力it／的日l夙7rVal毗方

       an톄ogRead() 함수로 읽어온 가변 저항의 값을 시리얼 통신을 이용해서 출력하고 있다．


 위의 스케치 코드는 http://arduino.cc/en/Tutorial/Analogli叩Ut에서 참조하여 작성을
하였다．


실행결과

 아두이노 시리얼 모니터 프로그램을 실행시키고 가변 저항의 손잡이를 돌리면서 테스트
를 해보면 저항의 중간쯤에서는 LED의 밝기도 중간정도로 밝아지고 왼쪽으로 돌리거나
오른쪽 끝으로 갈수로 比D의 밝기가 가장 밝아 졌다가 어두워진다. 그리고 시리얼 통신으
로도 데이터를 출력하기 때문어］ 아두이노 시리얻 모니터 상에 표시되는 숫자와 比D의
밝기를 비교해 보는 것도 좋다．




                                              5.3 가변저항 값 읽어오기 I 101
 .   Arduino .




                  口C0＼」：3                      ,        m吐 ![＼
                                                            口好卄늬
                  h,     ,                                                           Send
                   941
                  1936                                                                               1
                  1936                                                                               1
                  1936                                                                               1
                                                                                                     I
                  厓                                                                                  1h
                  1935
                  j935
                  [935                                                                               1
                                                                                                     i
                                                                                                "i
                  1935
                  1      '   Autoscroll
                                                        Carriage return !     9600 baud     -




                                          ［그림 于］2] 가변저항 값 읽어오기 실행결과




       5.4               테스터기 흉내I - 전압 값 읽기


      5.3절에서 아두이노의 아날로그 입력 기능을 이용해서 저항 값을 읽어오는 예제와 사실
     은 동일한 기능이지만 이번에는 읽어온 아날로그 데이터 값을 Voltage로 변환해서 표시해
     보도록 하자．


     실험에 필요한 준비물들

                                                                      ；冒m 1

                                                                                  :c9 「j 1


                                                                             11     m出 m小：H1
                                                                            1




                         H
                         브래드보드 17뀨                                     아두이노 ［爪OR3




                 적색 LED / 1K 저항 2개




102 ! 제5장 아날로그 입력과 출력
하드웨어 연결

 이전 절에서는 가변 저항은 필요하지 않고 이전 절에서 연결했던 LED와 저항은 동일하게
배선을 하고 아두이노 보드의 3.3V포트를 브레드보드에 연결하면 된다. 물론 아날로그
입력을 위해서 아두이노 보드의 A0 포트 연결은 해야 한다．




                         ［그림 千］3]       3.3V 전압 값 읽기 배선도


프로그램 작성

 아두이노 스케치에 아래와 같은 코드를 작성한다．


 mllt sensorPin = A0;         II select the input pin for the potentiometer
 mllt led = 9;               I/ the pin that the LED is attached to

 II the setup routine runs once when you press reset:
  void setupO
  {
      II declare pin 9 to be an output:
       pinMode(led, OUTPUT);

       Serial.begin(9600);



                                                          5.4 테스터기 흉내     전압 값 읽기 I 103
  .    Ard내rio e叫




            }
        II the loop routine runs over and over again forever:
        void loopO
        {
                m1lt sensorValue = 0’,
                float voltage = 0.0;

                II read the value from variable resistence
                sensorValue = analogRead(sensorPin);
                voltage = ((float)sensorValue/1023. 0)*5.0;
                Serial. prmnt(sensorValue);
                Serial.print(", ");
                Serial.println(voltage) ;

                analogWrite(led, sensorValue);

                II wait for 10 milliseconds to see the dimming effect
                delay(10);
        }


      加r sensori乞／ue = ｛彦

                   아두이노 아날로그 입력 포트 AO를 통해서 읽은 아날로그 데이터를 저장할 변수


      float voltage = a 0;

                    0勺伯23 사이의 아날로그 데이터를 전압（V에羽e) 값으로 변환한 값을 저장하기 위한 변수
                   를 소수점까지 표현하기 위해서 化at형으로 선언하였다．


      sensor Value = ana1碧Read(sen攷7rj가'I方
                    아두이노 아날로그 입력 포트 AO를 통해서 아날로그 데이터를 읽어 온다．


      （現oat方ensor白／ue

                    실수（소수점） 연산을 하기 위해서 정수형인 sensorValue 변수를 化at형으로 변환을 하는
                    두7［二




      vol氓ge = ((刃oat后ensor伍／U目/102多. 0戶夕. 0,
                    sens小alue의 최대긺이 ]023이기 때문에 ]023 값으로 나누고 나서 5.0을 곱해주면 아날



1041 제5장 아날로그 입력과 출력
      로그 데이터를 小5V 사이의 전압으로 변환할 수가 있다. 실수 연산을 하기 위해서 102301
      라고 하지 않고 ]02a0처럼 소수점을 붙여서 연산하였다．

駝ri뇨加rint(sens才I伍砒方
Seria如ri加1/F, ,,).
品r血／ ．戶i啣dn(乙叱智e方
      아날로그 데이터 값과 전압으로 변환한 값을 시리얼 포트를 이용해서 출력한다．


실행결과

 아두이노 시리얼 모니터를 실행해서 출력되는 결과 값을 확인해 보면 정확하게 5.OV라고
출력되지는 않는다. 이유는 아두이노 보드에서 출력되는 5V 출력 포트어］ 정확하게 5V가
출력이 되지 않을 수도 있고 아날로그 데이터를 디지털로 변환을 하게 되면 반드시 발생하
게 되는 오차가 존재하게 된다. 그렇기 때문에 원래의 데이터와 유사하게 출력이 된다면
올바르게 작동이 되고 있는 것이다．


         '因coM:B                  > 年 t#   11       量           多恥回 』片心m 켜
                                                                1正華了」



                              小




             756, 370
             754. 3.69
             751. 3.6?
             756. 3.70
             755. 3.69
             754, 3 . 咬｝
             755, 3．咬1
             754, 3.69
             754, 3.69
             753

             也Au加S아미I                       Carriage return !      9600 baud
         L                                                                乞




                           ［그림 5-14] 3.3V 전압 값 읽기 출력 결과


 이번에는 조금 바꾸어서 5,'/ 전압 값을 읽어서 출력을 해보자. 아두이노 스케치 코드는
동일하게 사용을 하면 된다. 단지 아래 그림처럼 아두이노 보드의 아날로그 입력 포트
AU를 아전과 다르게 5.OV 출력 포트와 연결을 해서 테스트를 하면 된다．




                                                          5.4 테스터기 흉내          전압 값 읽기 1 105
 .   Ard내no .




                        ［그림 도巧］ 5.O\/ 전압 값 읽기 배선도


      이 교재에서는 출력 결과 값을 표시하지는 않았지만 아마도 5.OV와 유사한 값들이 시리
     얼 모니터 프로그램 상에 출력이 될 것이다．




106 1 제5장 아날로그 입력과 출력
LCD 사용하기

 6.1   패러럴 LCD 디스플레이（4나出 모드）
 6.2 패러럴 LCD 디스플레이（8나升 모드）
 6.3 시리얼 LCD 디스플러떼
   Ard네m그 .



   LCD(Liquid Crystal I玉splay）는 우리 생활의 많은 부분에 사용되는 소자다. 손목에 차고
  다니는 손목시계부터 뉴스와 드라마를 보는 TV, 지하철역의 광고판까지 다양하다. 이번
  장에서는 이런 LD에 원하는 데이터를 아두이노를 이용해서 표시하는 방법에 대해 일아본
  다. 우선 Character LCI）어］ 데이터를 표시하는 타입에는 시리얼과 패러럴 방식의 두 가지
  가 있다. Character LCD는 간단한 문자 데이터를 표시하기에 적당하다．




     6.1      패러럴 LCD 디스플레이（4나이t 모드）


    Hitachi 印)44780은 시장에 판매되는 Character LCD 모듈에 많이 사용되는 LCI) 제어
  IC이다. 이 제어 IC는 많은 모양과 크기의 Dis히町를 지원한다. 이번 장에서는 16x1 LCD
  (16글자1열）를 사용한다. I-ID44780을 사용하는 LCD 모듈은 아두이노 IDE어］ Libra口가
  포함되어 있어 사용하기가 용이하다. 아래 표는 Liquid Crystal Libra玎에서 제공하는 함수
  들이다. 우리가 이번에 사용하는 LU刈 제어 IC는 정확하게 I-il乂478(）는 아니고 I-ID44780
   와 호환하는 IC를 사용하는 LCD이다.


   실험에 필요한 준비물들




               브래드보드 1개                   아두이노 UNOR3




              10K옴 가변저항 1711              16x1 Character LCD




1081 제6장 LCD 사용하기
 하드웨어 연결

  우리가 사용하는 LCD는 4bit모드와 8bit 모드를 사용할 수 있는데, 배선을 간단히 하기
 위해서 4bit 모드를 사용하였다．




                            ［그림 아］]   4b仕 LCD 구동하기 배선도



  희로도로 표현하기에는 그림이 알아보기 어려워 표로 정리하였다．

［표 6-2]          4b仕 LCD 구동하기 핀맵
   LCD Pin No                  Ard너no 디n                      LCD Pin
          1           GND                       Vss
          2           5V                        vCC
          3           Contrast（가변 저항에 연결）       vo
          4           D12                       RS(Register Select)
          戶뇨1/
                      GND                       R/W(Read/W血e)
          6
                      Dli                       Enable
      /
      H
                      NC（연결 없음）
          / 八
            8
                                                Data Bit 0
                      NC（연결 없음）                 Data Bit 1
          O
          /
          0
                      NC（연결 없음）                 Data Bit 2
          l

       l
                      NC（연결 없음）                 Data Bit 3
       l

       D
       二
                      D5                        Data Bit 4
       ］
       工
                      D4                        Data Bit 5
       八
       人
       口
       ］
       上
       d1
                      D3                        Data Bit 6
       4l
                      D2                        Data Bit 7



                                                6. ] 패러럴 LCD 디스플레에4七仕 모드） I i四
  + Arduino


      가능하면 L（그） 모듈 사용 전에 반드시 데이터 시트를 꼭 읽어보기 바란다. 데이터 시트는
    모듈을 구매하는 쇼핑몰 사이트나 모듈에 인쇄되어 있는 모텔명으로 검색해서 찾을 수
    있다. 대부분 I코tachi 7748() 호환 모듈들은 같은 핀맵을 사용하지만, 특별히 다르게 제작된
    모듈이 있으므로 핀 배열에 대한 정보도 반드시 확인해 봐야 한다．


    1) LCD의 \Iss를 (3ND어］ 연결한다. 그리고 Vcc핀을 아두이노 보드의 +5,\/ 단자나 +3V
      단자에 연결한다．
    2) LCD의 \T0 핀을 10K옴 가변저항의 가운데 핀에 연결한다. 저항은 극성이 없으므로
      가변저항의 왼쪽 다리를 +5V에, 오른쪽을 GNI）어］ 연결한다. 이렇게 가변저항에 연결하
      면 이제 가변저항을 이용하여 L:D 밝기 조절을 할 수 있다. 1x力를 테스트할 때 LD화면
      어］ 아무것도 표시되지 않거나 하얗게 녜모난 박스들만 보인다면 자가 표시될 때까지
      가변저항을 적당이 돌려 LCD화면의 밝기를 조절해야 한다．
    4) LCD의 RS(Register Select) 핀을 아두이노 디지털 12번에 연결한다. RS 핀은 LCD의
      내부 메모리에 접근 할 1 사용하는 핀이다．
    5) LCD의 E(Enable) 핀을 아두이노 디지털 11번에 연결한다．
      Enable 핀은 LCD 레지스터에 값을 쓸 수 있도록 하는 핀이다．
    6) LCD의 艮凹（Read/W血e) 핀을 아두이노 보드의 (3NI）어］ 연결한다．
    7) LCD의 DB4-DB7 핀을 아두이노 보드의 디지털 핀 D5-D2까지 연결한다．


    끄쿠그램 작성

      I/ include the library code:
      #include <LiquidCrystal.h>

      I/ initialize the library with the numbers of the interface pins
      LiquidCrystal lcd(12, 11, 5, 4, 3, 2);

      void setup0
       {
           7/ set up the LCD's number of coh.mms and rows:
           lcd.begin(8, 2);

      }
      void loop0


110 I 제6장 LCD 사용하71
     lcd. setCursor(0, 0);

     II Print a message to the LCD.
     lcd.print("hello, w");

      /1 set the cursor to column 0, line 1
     /1 (note: line 1 is the second row, since counting begins with 0):
     lcd.setCursor(0, 1);
     lcd,printC'orld!");

     delay(1000) ;




功nclude (Liqi끄dCrysra/．力I)

         아두이노의 L(：力 라이브러리를 사용하기 위해서 헤더 파일을 추가하다. 헤더 파일의 위치는
         小冶rd내no너 .0.5姸壯)rariesWLiq내dCrys囹"에 위치하고 있다．


L勾uidCrnta/ 兀d口乙 //, 多， 4, 3, 2七

        라이브러리 人f駱 하기 위해서 초기화 한다. lcd 초기화 값의 괄호안의 숫자들이 의미하는
        것은 아래와 같다. 즉 LCD와 연결된 아두이노보드의 핀 번호를 적어주면 된다．
        Icd(RS, Enable, Data Bit 0, Data Bit 1, Data Bit 3. Data Bit 4)


lcd.begin似 2上

        우리가 사용하는 j흔旦 ]6열 LCD이지만 아두이노 LCD 라이브러리를 그대로 이용하71 위하1
        서 2행 8열로 라이브러리를 초기화 하였다. 아두이노의 LCD 라이브러리는 원래 16문자
        2줄을 나타내는 LCD(1602 LCD릍 위해서 만들어졌기 때무게 匕CD 초기화 방법을 다르거1
        하였다. 아두이노의 LCD 라이브러리 예제는 h昨)://ard네no.cc/en/T내on졔／니叩idCrys囹를
        참조하기 바란다．


／口／.setCursor似 /2七

        LCD에 Dis口ay할 좌표를 정해준다．




                                                        6. ]   패러럴 LCD 디스플레이（4七it 모드） I 111
 1 Arduino



     ．尸thit(仍e끄b, I材宏
  ／匕（/
              우리가 LCD를 초기화 할 때 8열로 초기화했기 때문에 한 번에 8글자 이상 표현을 하지
              못한다. 8글자가 넘어가면 tcd.setCursor() 함수를 이용해서 0행에서 j행으로 행을 바꾼
              다음게 디스플러떼 하면 된다. 실저IL（力는 ］행 ]6열이지만 아두이노 라이브러리를 그대로
              이용하기 위해서 LCD가 2행 8열인 것처럼 생각하고 사용하는 것이다．


     위에서 설명한 함수 이외에도 아두이노 LCD 라이브러리에는 여러 가지 기능의 함수를
   다앙하게 제공하고 있다．



                      Function                        Description
    begin(int column, lot row)       LCD 화면의 열, 행의 개수를 지정
    clear()                          LCD 화면을 클리어 한다．
    borneO                           문자 표시위치를 왼쪽 상단으로 지정
    setCursor(int column, mnt row)   문자 표시위치를 열과 행으로 지정
    write()                          현재 커서 위치에 한 문자를 표시
    print()                          현재 커서 위치에 문자열을 표시
    cursor()                         현재 커서 위치에 커서（ 1' ) 모양 표시
    noCursor()                       커서 문자를 숨긴다．
    bunko)                           커서 모양을 깜빡 이도록 한다．
     noBllnk()                       커서 Blinking Disable

     displayO                        LCD Display On

     noDisplayO                      LCD I万splay O什

     scrollDisplayLeftO              왼쪽으로 한 문자 스크롤

     scroliDisplayRightO             오른쪽으로 한 문자 스크롤
                                     문자를 LCI) 디스플레이 범위를 넘어서면 왼쪽에서 오
     autoScrollO                     른쪽으로 자동 스크롤
                                     문자를 LCD 디스플레이 범위를 넘어도 자동으로．스크
     noAutoScroll()
                                     롤 하지 않음
     leftToRightO                    문자 표시 방향을 왼쪽에서 오른쪽으로 표시
     rightToLeft()                   문자 표시 방향을 오른쪽에서 왼쪽으로 표시




    실행결과

      컴파일을 해서 실행을 하면 LCD 화면에 "hello, world!"의 영문 글자가 표시된다．




112 I 제6장 LCD 사용하71
  6.2   패러럴 LCD 디스플레이（8-bit 모드）


 LCD를 8bit로 구동시키는 방법은 LCD와 아두이노 보드와의 배선만 다르게 하면 나머지
스케치 코드와 실행 결과는 동일하다. 배선이 좀 복잡하지만 8bit 모드를 사용하면 LCD어］
문자를 디스플레이하는 속도가 4bit 모드보다 빠르다는 장점이 있다．


하드웨어 연결

 이전 Chapter에서는 4bit무＝로 LCI居 사용하였고 조금 복잡하기는 하지만 이번에는
8bit 모드로 사용하기 위해서 배선 연결을 해보자．




              ［그림 아3] 8bit LCD 구동하기 배선도


 아래 표는 LCD를 8b且로 구동시킬 경우에 LCI파 아두이노 보드와의 핀 연결을 하는
방법이다. 8bit 무＝로두 한 번 구동을 시켜 보기 바란다. 배선 연결이 복잡하여 별도로
회로도는 그리지 않았다．




                                 6.2 패러럴 LCD 디스플레이（8나來 모드） 1 113
 1 Ard너no



  ［표 于4] 8b仕 LCD 구동하기 핀맵

     LCD 다n No                 솨dumnb 다n        ,                 LCD Pin
            1       GND                             Vss
            2         5V                            vCc
            3         Contrast(가변 저항에 연결）           V0
            4       D12                             RS(Register Select)
            5       Dli                             R/W(Read/Write)
            6         D2                             Enable
            7         D3                             Data Bit 0
            8         D4                             Data Bit 1
            9         D5                             Data Bit 2
            10        D6                             Data Bit 3
            11        D7                             Data Bit 4
            12        D8                             Data Bit 5
            13        D9                             Data Bit 6
            14        D10                            Data Bit 7



     쿠＝램 작성


     m1lt DI = 12:
     mllt RW = ii:
     mllt DBII = {3, 4, 5, 6, 7, 8, 9, 101;
     m1lt Enable = 2;

      void LcdConunandWrite(int value) {
       II poil all the pins
       mllt i = 0;
       for (i=DB[0]; i <= DI; i++) {
          digitalWrite(i,value & 01);
          value 力＝ 1;
       }
       digitalWrite(Enable,Low);
       delay岫crosecon由（1) ;
       II send a pulse to enable
       digitalWrite(Enable,HIGH);
       delayMicroseconds(1); // pause 1 ins according to datasheet
       digitalWrite(Enable,LOw)



114 I 제6장 LCD 사용하71
            delayMicroseconds(1);   1/ pause 1 ms according to datasheet
        }
    void LcdDataWrite(int value) {
            II poii all the pins
            mllt i = 0:
            digitalWrite(DI, HIGH);
            cligitalWrite(RW, LOW);
            for (i=DB[0} ; i <= DB[7]; i++) {
               digitalWrite(i,value & 01);
               value >>= 1;
            }
            digitalWrite(Enable,LOW) ;
            delayMicroseconds(1);
        II send a pulse to enable
        digitalWrite(Enable,HIGH);
        delayMicroseconds(1);
        小gitalWrite(Enable,LOW);
        delayMicroseconds(1); II pause 1 ins according to datasheet
    }
void initLCDO {
 delay(100);
 II initiatize lcd after a short pause
 II needed by the LCDs controller
 LcdCommandWrite(0x3A); II function set:
                                    II 8-bit interface, 2 display lines, display ON
        delay(10) ;
        LcdCommandWrite(0x0E);         II display control:
                                    I/ turn display on, cursor on, no blinking
    delay(10) ;
    LcdCommandWrite(oxol); II clear display, set cursor position to zero
    delay(10) ;
    LcdCommandWrite(0x06); // entry mode set:
                         I/ increment automatically, no display shift
    delay(10) ;
}
II this is the function used to send data to the
II LCD screen in the proper format, the others are
II working at lower level



                                                           6.2 패러럴 LCD 디스플레이（8나升 모드） 1 115
 .   Arduino .




      void printLCD(const char *s) I
        m1lt count = 0;
        while (*s) {
          if(count==8) {
             LcdCommandWrite(0xC0);                  //jump to the second part of the thsp1ay:
                           delay(5);
                       }
                       if(count> =16) 1
                          break;
                           }
                       LcdDataWrite(*s++);
                       count ++;
                   }
       }
       void setup 0 1
        mllt i = 0;
        for (i=Enab1e; i <= DI; i++) {
           pinMode(i,OUTPUT);
               }
               initLCDO ;
       }
       void ioop 0 {
         LcdCommandWrite(0x02); II set cursor position to zero
         delay(10) ;
         II Write the welcome message
         printLCD("Hellow World!");
                   delay(500) ;
           }


       8bit 모드에서는 아두이노의 LCD 라이브러리를 사용하지 않고 스케치 코드를 작성하여
     코드가 조금 복잡하다. L（力 초기화 코드들을 모두 이해하기 위해서는 LCD 데이터시트의
     모튼 내용을 이해해야 가능하므로 아두이노 보드에서 사용방법만을 알아보자．


     mr D/ 二＝ ／乙r
                               LCD Register Select 핀을 정의한 것이다．



116 1 제6장 LCD 사용하:71
m7r RW = 1亡
       LCD에 Data（문자）를 Write 하기위해서 필요한 핀이다．

加t DB/J = 夙 4; 多， 6, 7; 曷 ！亐 끄助r
       LCD이 8bit 데이터 핀이다．

"Jr 正na加C = 2,

       LCD에 데이터를 V내te하기 전에 반드시 LOW로 설정0I 되어야 한다．

／兀in比CD( '姚肌기y 1机刎넸吩

       LCD에 문자를 디스플러떼 한다．


실행결과

  컴파일을 해서 실행을 하면 LCD 화면에 "hello, world!"의 영문 글자가 표시된다．




mk= 시리얼 LCD 디스플러回
 시리얼 LCD와 패러럴 LCI刈 차이점은 시리얼 LCI거三 한 개 데이터를 보내는데 한
선만 가지고도 데이터를 전송할 수 있는 것이다. 시리얼 LC[파 연결되어 있으면 serial
.prir奴cammand）라는 명령어로 LCD에 다앙한 문자를 표시 할 수 있다. 그리고 LCD를
켜거나 끄기, 커서 이동 등 다앙한 LCD동작도 시킬 수 있다. 물론 이런 동작을 시킬 수
있는 코드들（h却://ard岫均. cc/playground/C（넜e/SerLCD）은 이미 아두이노 라이브러리로
작성되어 있지만 여기서는 아두이노 라이브러리 함수를 이용하지 않고 커스텀으로 작성된
함수를 사용해서 실험을 할 것이다．


실험oil 필요한 준비물들




           브래드보드 17뀨                    아두이노 UNOR3


                                             6.3 시리얼 LCD 디스플러떼 I 117
 .   Ard내no 1




     하드워뻐 연결

      시리얼 LCD의 가장 큰 장점은 역시 배선이 쉽다는 것이다. LCI）어］ 문자를 디스플레이
     하기 위해서 단순히 아두이노 보드의 D（포트와 시리얼 LCD의 RX 포트 1개의 연결만으로
     문자를 디스플레이 할 수 있다. 물론 LCI刈 천원 공급을 위해서 VCC, GND 27뀨 핀의
     연결은 필수적이다．




                     ［그림 아5]   시리얼 LCD 구동하기 배선도




118 I 제6장 LCD 사용하기
 위의 배선도에서 LCD옆에 4개의 핀이 나와 있지만 실제 제품에는 LCD 밑면에 4개의
핀과 밝기 조정을 위한 가변 저항 2개가 있다．
 위의 그림은 LCD 제품과 아두이노 보드의 배선도를 보기 쉽게 하기 위해서 약간 편집을
한 것이다. 실제 시리얼 LCD 제품의 그림은 아래 그림을 참조하기 바란다. 만약 실험에서
LCD화면에 문자가 제대로 보이지 않는다면 시리얼 LCD 밑에 있는 2개의 가변 저항을
돌려서 밝기를 조정해 보기 바란다. 171]는 LQ) 백라이트 밝기를 조정하는 저항이고 1개는
LCD에 표시되는 문자의 밝기를 조정하는 처항이다．




                             ［그림 &6] 시리얼 LCD 실저1 사진


프토그램 작성

 void setupO
 {
     Serial begin(9600);
 }
 void loop()
 {
     Serial.print("$ EARWWll'
     Serial.print("$GO 4
     Serial.print("$PRINT  ome 的Wi伽") ;
     Serial.print("$GO 2 1
                               , 1)
     Serial.printC'$PRI町     'kelec. co.krWrWn");
     Serial.print CURSO 1 1



                         /
                    "$
                (
     delay(i000);
 }


                                                      6.3 시리얼 LCD 디스플러떼 I 119
 .   Arduino .-



         . ZX땀加汐6a까‘
     S匕i勿／
             시리얼 통신을 통해서 LD 디스플레이를 하기 ［대무게 96C 力佛로 아두이노의 시리얼 통신
             을 초기화한다．


          ．戶n加附（Z丑4Rtrn切
     Serf눈／
             LCD 화면을 모두 지운다．


     Seria/print( "$GO 1 41rtn');
             LCD에 표시될 문자의 위치를 ］행 4열로 지정한다．


         .／功mnr($PRTh7T
     Sei勿／                    色／匕（me t이』r1可F).

             LCD에 문자를 디스플레이한다．


         ．戶rint尸修CL仄羽R / 1k뇨切
     Sei屯／
             커서를 l흔旦 ］열로 지정한다．

       주의할 사항은 LCD에 명령과 문자를 전송할 때 반드시 ' \r\n" 문자로 끝내야 한다．


     실행결과

      컴파일을 해서 실행을 하면 LCD 화면에 첫 번째 줄에는 "Welcome to"라는 문자가
     표시가 되고 두 번째 줄에는 "www.jkelec.co.kr"라는 영문 글자가 표시된다．




1加 1 제6장 LCD 사용하기
실제 세계와의
         통로 센서
7. ]   센서 소개
7.2 밝기 감지하기 - CDS 조도센서
7.3 온도, 습도 감지하기 -D나11 ] 온습도 센서
7.4 화재 감지하기 1 화염감지 센서
7.5 기울기（1-lit) 감지하기 - SW-520D 7울기 센人1
7.6 진동 감지하기 - SW-18020P 진동 센서
7.7 장애물과의 거리 감지하기 1 초음파센서
  1   Arduino .




        7.1       센서 소111


       센서의 정의를 Wi蜘edia에서 찾아보면 센서（sensor) 또는 감지기（感知器）는 온도나
      빛 같은 물리에니지를 천기신호로 바꿔 주는 정보탐지장치를 라고 정의하고 있다. 오늘날
      센서의 종류는 수도 없이 많고 실제 제품에서도 유용하게 이용이 되고 있다. 최근어］ 많이
      사용하고 있는 스마트폰에 숨겨진 센서들을 찾아보자．
       근접센서, 온도／습도 센서, 지자기 센서 , 자이로 센서 , 가속도 센서 , 조도센서 등 제품
      하나에도 여러 종류의 센서를 조합하여 사용하기 편리 하도록 제품에 다앙한 용도로 이용이
      되고 있다. 아두이노에서도 이용 가능한 센서들이 많이 있는데 크게는 아날로그 인티페이
      스 센서와 디지털 인터페이스 센서로 분류할 수 있다. 우선 우리가 실험해볼 센서들을
      2개의 종류로 나누어 보자．


      會 아날로그 센서
              CDS 조도센서

      I 디지털 센서
              DI끄11 온습도, 화염감지, SW-520D 기울기, SW-18020P 진동, 초음파센서


       위에서 나열된 디지털 센서도 인터페이스는 디지털이지만 센서 자체는 대부분 아날로그
      값을 출력으로 하는 센서들이 대부분이다. 이제부티 각 센서들을 하나씩 실험해 보자．




                  밝71 감지하기 -CDS 조도센서


       흔히들 알고 있고, 저렴한 가격과 활용도 때문어］ 많이 사용하는 빛 감지 센시이다. CI万
      센서는 광에 쏘여지면 저항 값이 감소하는 광도전효과（Photo conductive e丘ect）를 이용한
      반도체 포토센서이다．
       CdS라고 불리는 이유는 CdS Ph야oresist아를 만드는 주 재료가 카드늄（Cd）과 황（S）의
      화합물인 황화카드뮴（CdS）이기 때문이다 포토셀（PhotoCell)이라고도 많이 불리며, 빛의
      밝기에 반웅을 한다. 주위가 밝으면 저항이 줄어들고 주위가 어두우면 처항이 커지는 특징
      을 가지고 있다．


122 1 제7장 실제 세계와의 통로 센서
                            전극                   열처리한 CDS

                                                 리드선

                                 ［그림 갸］] CDS 셀의 구조


   즉 주위가 밝아지면 CdS저항이 줄어들어 Analog Input 핀에 높은 전압이 들어가고
  '- 긔i글 주의：
           가 （뇌특三훠又］口4cAs희 저흐如］ 쿼又］긔］ 되T그 亡三 0

들어간다．
   이번 실험에서는 CDS센서를 이용해서 주위가 어두워지면 아두이노의 Dli어］ 연결된
［丑D를 P\X/M을 이용하여 밝게 켜고 주위가 밝이찌면 어둡게 켜는 실험을 해보자．


실험에 필요한 준비물들

                                                         茗崔 S

                                                                :cD   1/
                                                                           .    1




                                                            1口   小나 m          --S
                                                           S

                  브래드보드 17뀨                              아두이노 UNO R3




                                                           r在}
                    1;
          적색 1上D / 1K, 10K 저항 17긔1                        CDS 센서 1깨1


하드워II어 연결

  아두이노의 p＼凹入4 기능을 이용하기 위하여 p明M 기능이 있는 디지털 핀 중에서 Dli어］
r T7r）르－ 11(   처巧：Fj기．. 히껴］ 여겨云i- -u cr-)s서］人a （기 처古1- zJ-으 (>11才己口 ；갸C) 己 으k뇌 튼．어0t
                                                   1 0 口八 己



하기 때문어］ Cl万의 2개의 리드선중 1개를 AU 핀에 연결한다．
  CDS센서에 보면 리드선이 27中｝나와 있는데 CDS센서도 저항으로 생각하면 극성을
구분해서 연결을 하지 않아도 된다．

                                                       7.2 밝기 감지하71 - CDS 조도센서 1 123
 .   Arduino .




                          ［그림 가2]               CDS 조도센서 배선도




             1
                                   3V3     5V        V씨


                          RESET          Arduino              TX'［兀

                          日ESET2           Uno                RX/01

                          AREF            (Rev3)                 02

                          IOREF                             PWM 03
                                     Aol내no UN0 63
                                                                 04

                          AS                                 PWM 05

                          Al                                 PWM 06

                          62                                     07

                          A3                                     08

                          A4/SOA                             PWM 09    -   LE01
                                                                           Re4 (633nm)
                          65/SdL                          SS/PWM 010

                                                      MO미／P나M Oil

                                                           베50/0俚      小

                                                             SCK/D侶




                                                UNO



                                                                                fritzng

                           ［그림 갸3]              CDS 조도센서 회로도
         CDS 센서의 한쪽 리드선을 AO에 연결하였으면 나머지 한쪽은 VCC(5.OV or 3.3V）에 연결한다．



124 I 제7장 실제 세계와의 통로 센서
  쿠기랄1 작성

  아두이노 스케치에 아래와 같은 코드를 작성한다．

  mllt lightPin = 0; II define a pin for Photo resistor
  m1lt ledPin=11;    II define a pin for LED

  void setupO
   {
        Serial.begin(9600); I/ Begin serial communcation
        pinMode( ledPin, OUTPUT);
  }
  void loopO
  {
       Serial.println(analogRead(lightPin));
       analogWrite(ledPin, analogRead(lightPin)/2);
       delay(10); I/ short delay for faster response to light.




Ju2t 五智／it／功7 = 0,

         CDS센서가 연결된 아두이노 아날로그 입력 포트 번호


加r ledPmn=11;

         P M으로 밝7를 조절할 아두이노 PWM 기능0I 가능한 포트 번호


pinMode( ledPin, OUTI兀／丁 方
         匕ED가 연결된 포트의 출력을 위해서 OUTPUT으로 설정


Serii/ printin白nak咨Read(岫加／'in)方
         CDS센서가 연결된 포트의 아날로그 값을 읽어서 시리얼 통신으로 출력한다. 아두이노의
         아날로그 입력 값은 小／1023 사이의 값이 출력된다. 이 값이 정해져 있는 이유는 아두이노
         가 AThIEGA CPU를 기반으로 하고 있기 때문에 ATh雁GACF기의 ADC 입력의 Resolu的n
         이 ］아出이므로 2의 ]0승으로 계산되는 값이다．


anak乷r比Ym伽dl物， analog)？匕ad？玉智／itPmn方'2上
         CDS센서의 밝기에 따라서 F긔사卜기 포트에 연결된 LED의 밝기를 조정하는 스커因 코드이다．



                                                         7.2 밝기 감지하71- CDS 조도센서 1 125
    Ard벼n（그   1




   실행결과

     a芬센서를 손이나 다른 물체로 가려 보자. 그리면 붉은색 I且）의 밝기가 밝아질 것이다．
   그리고 아두이노에서 시리얼포트 모니터 창을 실행하면 아래 그림과 같이 CDS센서에서
   읽어지는 값 O- -'1023 사이의 숫자를 계속해서 출력한다．

                    r宙Co낳：; ‘附m的朴            毛鱗蹄毋心小m 「                     口비叫
                          I                                                        Send
                          C161 value = 6出
                          CDS val尼 = 624
                          CBS value = 588
                          cc心 V미ue = 580
                          CBS value = 619
                          CBS V시四 = 615
                          CBS v미四 = 531
                          CtlSv키四 = 655
                          CtlSv미ue = 622
                          CBS eel四 = 日15
                          CBS 키此 = 6沔
                          CBS V키叱 = 578
                          CBS va lue = 591
                          CBS eel四 = 田4
                          CBS v이四 = 628                                                       i
                          CBSvalue= 6弱                                                        I
                          CflSvalue= 649                                                  i
                    hBS eel四 : 凹9                                                         I


                    伊：客                                                                   I
                    1MA        uitoscroll                   Carriage return 乞 卿0 baud     J
                                   ［그림 石4]    CDS 조도센서의 출력 결과 창




      7.3         온도, 습도 감지하기 - DHT1] 온습도 센서

     DHT11은 온도와 습도를 동시에 측정이 가능한 온습도 센서로 아두이노 PlayGround
   (http://playground.arduino.cc/main/DHT11Lib）에서 라이브러리를 제공하고 있다．
     DHT11은 온도와 습도를 동시에 측정할 수 있는 것은 아니고 서로 배타적으로 측정값을
   읽어올 수가 있다. 아래 표는 DHT11 온습도 센서의 사앙을 정리한 것이다


      Measurement                Humidity       Temperature
                                                                       Resolution                  Package
         Range                   Accuracy        Accuracy
       20-90%RH                                                                                   4 Pin Single
                                  士5%RH            士2乞                       1
        아50t                                                                                         Row




126 1 제7장 실제 세계와의 통로 센서
실혐에 필요한 준비물들




          브래드보드 17뀨                                                                          아두이노 UNOR3




                                                                                                1111
          4.7K 저항 1가1                                                                      DHT11 온습도 센서 I가1



하드웨어 연결

 DI-口11센서는 4개의 리드선을 가지고 있다. 왼쪽에서부터 순서대로 VCC, Data, NC,
GNT) 순이다. VCC어］ 인가할 수 있는 전원은 3\／巧. 5,'/ 사이의 DC전원을 연결하면 된다．
Data선은 아두이노 보드의 D2와 연결을 하고 NC(Not Connect) 선은 연결을 할 필요는
없다. NC는 연결을 하지 않아도 되는 선을 말한다. 아래 그림은 DHT11 4개의 핀을 그림으
로 표현한 것이다．

                                                          1
                                        心 口 1 1 1 1               m = 口 口 1 1
                                                      1
                            m m = = m                 1 1 1 1 1
                                                                                mm m m 4



                              b
                              n
                            1 H
                                                                  1             1


                              b
                            1 Dna t a
                                                                                H D
                            重 VCC

                ［그림 石5]   DHT1 ] 온습도 센서 핀 그림


 아두이노와 센서를 연결할 때 위의 그림을 참조해서 전원과 데이터 선을 연결하면 된다．
DHT11 온습도 센서와 아두이노 보드와 연결할 때 너무 길지 않도록 연결을 해야 하고
장시간에 밝은 빛이나 태양빛에 노출된 환경에서는 센서의 데이터에 이상이 올 수도 있다．


                                                                                 7.3 온도. 습도 감지하71- DHT11 온습도 센서 1 127
  .   Arduino 1




              :
                  ::

                           II,        ' '
                  1.
                       .
                           III




                                        ［그림 가6]               DHT1 ] 온습도 센서 배선도




                                              3V3     S'I       Vi


                                 什ESET              Arduino                                       RI4 7EQ
                                 日ESET2               Un（그
                                 AREF                (Aev3)                    "'   므，    ,’

                                 心目EF                                 PWM 03
                                                Ard네na UN口 n3
                                                                                     04

                                 AO                                   PWM 。5

                                 Al
                                                                                                            C
                                 A2

                                 A3                                                      07。8      RHT03
                                 .A4/SOA                                                        DAT斗5喀nl




                                                                                                       GND

                                                                     "'   뽄．   ，「 「，




                                                            3늬：그




                                            ［그림 가7]           DHT11 온습도 센서 회로도




128 I 제7장 실저1 세계와의 통로 센서
 쿠 '그 랄1 작성

 아두이노 스케치를 작성하기 전에 아두이노 PlayGround에 방문하여 DHT11 온습도
센서 라이브러리를 다운받아야 한다. 먼저 htt莎刀playground.arduino.cc/rn鈿／Dl打liLib
사이트에 접속한다．


              Oy二七：= je:') rrrtl:         y   命如d山no p啣如Un小D卜 X                                粒느
              e         C     姓       D冶느．兀y口Unaan그Unio. cc m ain/DH111Lb                                             玉
                              ‘疊 口 鈿姚蜘必麟9251工               =: 三 건갛트객캄已                              力 二 挺注：크
                     y石加e百d湃可面迂da匣而rmat. Criec乂                         니 口 , lot su까兀戊of theses斗4이5


              가陌 libra叩 珏 tested on a卜AEGA25BO and is con加n祀d working on an Ard내no 2C


              卜小esteszeck has made an 吐err바兀driven 出町 向 the DHT11 sensor



              Andy Dalton has made tt modified vers幻njJifference that the DATAPIN is deft
              cons蜘吐or, res岫ng 油 one sled兀ated o히毗 per sensor.
                                                                                   is
              Connection
              The Di-I乙"1 has three lines: GND, 卜SV and a single data line. By means of a handsl



                        ［그림 가8] DHT1 ] 센서 아두이노 디ayGround

 아두이노 플레이그라운드 DHT11L小 웹 페이지의 상단에 보면 "mod出ed version" 의
링크를 따라가 보자．


                  ) ardurno 'pr미ects/Dhtll 《 5.
                                             ；二m                    :           自字
          : <=         C      在   口    ‘너：1L 1兀 ，匕     1-       gttnub.conl
          ; 芦 聲퓰리飛쩍선 .            Emo믄我Mm呼丑1-f             =: 三 d감트玉캄＼                                r\   !   三   른： =   i




                  I' 二n引巴nmaster !     arduirn놔pr이C:            Dhtll_Libr칡y

                  Change 骨n 卄口rO rt tO S泣a4t. reoden9e：注

                     副카的n 크m      가 \ 가or出口S 寸孕그




                  圄 flhtll cpp                        朋ores恥Cairo

                  會 Dhtlt h                           5tonge pm from 1nt to s,ze_t reorder 듀elds

                  國 Make터e                            Change pro from 1nt to size t. reorder Selds

                  圄 Tern州叩妃dy CPP                     Add DHT1I RanedrtyiTemperature sensor rh




                              ［그림 가9] DHT1 1 Github 관리 사이트


                                                                         7.3   온도, 습도 감지하71 - DHT11 온습도 센서 1 129
 .   Ard내no 1




      Github(https://github.com/adalton/arduino/tree/master/projects/Dht11_Library)에서
     관리되고 있는 아두이노용 DHT11 센서의 라이브러리 파일들을 다운로드 받을 수 있다．
     다운받은 4개의 파일들을 ' /arduin아1.0.5\libraries\DI-IT11"와 같은 폴더를 생성하고 전부
     복사를 한다. 그리고 아두이스 스케치 코드를 작성한다．
      arduino-1.0.5라는 폴더는 현재 사용 중인 아두이노 개발환경의 버천에 따라서 달라
     질 수 있다．


       ／水
       http:1/playground. arduino.cc/main/DHT11Lib
        永／
       #include <dhtll.h>

       #define DHT11PIN 2

        dhtll DRT11;

        void setupO
             {
                 Serial.begin(9600) ;
                 Serial.println("DHTll TEST PROGRA江 ");
                 Serial. printCLIBRARY VERSION: ');
                 Serial.println(DHT11LIB_VERSION);
                 Serial.printinO;
             }
             void loopO
             {
                 Serial.println("Wn');

                 m1lt chk = DHT11.read(DHT11PIN);

                 Serial.print( 'Read sensor: ');
                 switch (chk)
                 {
                     case DHTLIB OK:
                               Serial.println("OK ');
                               break




1301 제7장 실제 세계와의 통로 센서
        case DHTLIB ERROR CHECKSUM:
                  Serial.println("Checksum error");
                  break;
        case DHTLIB ERROR TIMEOUT:
                      Serial.println("Time out error");
                      break;
        default:
                      Serial.println("Unknown error");
                      break;



      Serial.print("Humidity (%): ");
      Serial.println((float)DHT11.humidity, 2);

      Serial print("Temperature (O c): ");
      Serial println((float)DHT11. temperature, 2);

      delay(2000) ;
  }

李）左ic/ude (／方tiLh)

         DHT1 ] 라이브러리를 사용하기 위해서 반디1 추가해야 한다．


李乙／'eline DHTJ／尸刃V2

         센서의 데이터를 읽기 위한 아두이노 보드의 디지털 포트 번호이다．


（功di D月Ti';

         센서 라이브러리를 사용하기 위한 초기화 코드0다．


Set出n力ntin(DHTi끄j可1匹RSION);

         DHT1］니日VERSION의 값은 dhtll.h 파일에 정의되어 있다．


Jut C力k = DHTJLread口7月T1iP刃＼才

         아두이노보드의 D2 포트에서 센서의 데이터 값을 읽어온다. chk 변수가 DHTLIB_OK 인
         경우에만 정상적인 데이터가 읽혀진 것이다，




                                                  7.3 온도, 습도 감지하기 寸 DHT1] 온습도 센서 1 131
 .   Arduino .


             - DI羽［LIB_ERROR_CHECKSUM : 센서 데이터의 체크 섬 에러가 발생한 경우이다．
             - DF끄口JB_ERROR_TIMEOUT: 1초 이내에 데이터 읽기를 하지 못한 경우


         .／기TiflL加((floar江쪼[Til . 方UflIk万m 2七
     Sei始／
             센서에서 읽은 습도 값을 시리얼 통신으로 출력한다．


     品i油n功初切(1日oa功D匹刃끄. rei刃perat끄re, 2方
             센서에서 읽은 온도 값을 시리얼 통신으로 출력한다．

     de怡H加口口方

             올바른 센서 데이터를 읽기 위하IAI ］초 이상의 Delay 타임이 반드시 필요하다．


      DHT11 센서에서 1八wire 연결을 통해서 약 1초마다 한 번씩 온도와 습도 값을 읽어
     올 수가 있다. DHT11 센서에서 출력하는 데이터 포맷은 습도 데이티가 먼저오고 온도
     데이티가 온다. 정확한 포맷은 아래와 같다．

      Data format: 8bit integral RH data+8bit decimal RH data+8bit integral T data +
                  8bit decimal T data + 8bit check sum

       조금 복잡해 보일 수 있는데 상세한 사항을 알고 싶다면 아두이노 DI-ITli 라이브러리
     코드를 분석해 보는 것도 좋은 방법이다．


     실행결과

        2초 간격으로 습도와 온도가 터미널 창에 표시가 된다．

                     "的COM好                             簪“                    ／斗M冬뇨二1
                                                                                       Send

                         OHT11 TEST POQIORAM                                                  小
                         LIBRARV VERSION: 0.   4.
                                                    1



                                                                                                  亘
                      ：喆；):"즘.。。
                     心：
                         Temperature (A C): 26.00



                          fl Autoscroll                      Carriage return ! . 9600 baud    !
                                                                                                  4
                     L


                                   ［그림 가］0] DHT1 ] 온／습도 출력 결과



132 I 제7장 실제 세계와의 통로 센서
  7.4   화자1 감지하기 中 화염감지 센서


 화염 감지 실습은 화염 센서를 이용하여 화염의 파장을 인식하여 감지하고, 감지된 신호
를 아두이노 디지털 입력으로 인식하여 적절한 제어와 출력을 할 수 있는 실습이다. 이번
실험에서 사용할 센서는 화염의 파장을 감지할 수 있는 센서 모듈이다. 약 80cm 정도의
거리에서 발생한 불을 검출할 수 있는 센서 모듈이다. 이 모듈의 주요 특징은 다음과 같다．


 - 760nm에서 1,l00nm의 범위에서 불이나 광원의 파장을 감지
  （가변 저항으로 감도 조절 가능）
 - 80cm의 불을 검출
 - 감지각도는 약 60도 정도에서 화염 스펙트럼에 특히 민감


 화염 센서 모듈은 아래의 그림과 같이 화염 센서 , 비교기로 구성된다．




                                                    ［기이t키 Output




                 ［그림 가］l]   화염 감지 센서의 구성


 화염 센서 모듈의 동작은 화염 감지가 있는 경우와 없는 경우의 동작이 있다. 우선
화염 파장이 감지된 경우에는 화염 센서 입력 전압이 기준 전압을 설정하는 가변 저힝（파란
네모 모양 안에 십자 표시가 된 부품） 값에 따라 설정한 기준 전압보다 작으면 비교기에
玩w 값이 출력된다. 출력된 값은 위의 그림에서 보듯이 화염감지 센서에 부착되어 있는
I助가 ON 된다. 하지만 화염 센서 입력 전압이 거의 없다면 기준 전압보다 커서 비교기어］
I玉gh 값이 출력된다. 그러므로 LED는 OFF 된다．

                                     7.4 화자1 감지하기   화염감지 센서 I 133
 .   Arduino .



     실험에 필요한 준비물들




                    브래드보드 17뀨           아두이노 Ul幻 R3




                 적색 1코D / 11( 저항 27긔1   화염감지 센서 17月




     하드웨어 연결

      화염이 감지되었을 경우에 붉은색 珏D를 켜기 위해서 LED를 아두이노 보드의 D3 포트
     어］ 연결하고 화염감지 센서의 출력 핀（DO - Data Out）을 아두이노 보드에서 입력으로
     빌아들이기 위해서 아두이노 보드의 D2어］ 연결을 한다．




134 1 제7장 실제 세계와의 통로 센서
!




                   ［그림 가］2]              화재 감지하기 배선도




             3V3    5V         N


    RE앉그           Arduino              TX/Do
    日ESET2           Uno                RX/D1
                                                 Fire Sone아
                                                 Sonno四
    AREF            (Rev3)                O2      小0
    1C）日EF                            p넥M O3
              사dumnb UNO 63
                                                  n태｝
                                          D4      싸（(
    AS                                PWM O5

                                      p叫M O6
    A2                                    O7
    A3                                    Do
                                                              LED2
    A4/SDA                            p넥 너 O9                 Eel幻놔 (595nnr)

    A5/SCL                         so/p놔M O10

                               MO듸／p叫M O11
                                    싸Sc）八기 2      N
                                                  1k났
                                     SCKID田     ＋小m1川mmm


    川C




                         GND




               ［그림 7-13]                화자1 감지하기 회로도


                                                        7.4 화재 감지하;71          화염감지 센서 I 135
  .   Ard내no e -



       쿠기램 작성

       아두이노 스케치에 아래와 같은 코드를 작성한다．

        mllt led = 3;
        mllt sensor == 2;

        void setupO
        {
            pinMode(led, OUTPUT);
            pinMode(sensor, INPUT);
        }
        void loopO
        {
            if( digitalRead(sensor) == LOW)
               digitalWrite(led, HIGH);
            else
               digit刻‘Write(led, LOW);

            delay(100) ;
        }


      加t led = 秀

                화자까 발생하였을 경우 알려주기 위한 匕ED 포트


      tnt sensor = 2;

                화자1 감지 센서의 DO(미야톄 O내）와 연결한 아두이노 연결 포트


      加nMo兀(icc工 OUTFU1方
                LED를 켜기 위해서 LED와 연결된 아두이노 포트를 OUTPUT으로 설정


      /址mk屯sen聊；刀w迂／7方

                화재김仄1 센서에서 입력을 디지털 입력을 받기 위해서 INPUT으로 설정


      1町 d智亡沚R匕a毗ensor) == 工OW)
                화재감지 센서와 연결된 아두이노 포트를 읽어서 LOW이면 화자마 감지된 경우임



1361 제7장 실제 세계와의 통로 센서
（九／a汗／m土’

        ］초마다 한 번씩 화재를 감지 하기위해서 필요함．


실행결과

 화염을 제대로 감지하는지 테스트하기 위해서는 불꽃이 필요하다. 라이터나 촛불 등을
이용하여 센서가까이에 대보자. 그러면 브래드보드에 있는 LED가 켜질 것이다. 물론 화염
감지 센서 모듈에 있는 LED도 동시에 켜지게 퇸다. 불꽃에 제대로 반응하지 않는다면
화염감지 센서에 있는 파란색 모양의 작은 가변저항을 십자드라이버를 이용해서 미세하게
조정한 이후에 테스트하면 된다. 가변 저항을 이용하여 센서의 감도를 조정할 수 있다．




  7.5       기울기什lit) 감지하71 - SW-520D 기울71 센서


 기울기 감지 실습은 기울기 센서 모듈을 이용하여 기울기를 감지하고 감지된 신호를
아두이노 보드로 입력하여 적절한 제어와 출력을 할 수 있는 실습이다. 금으로 도금된
재질의 원형 하우징에 금속 볼을 내장하여 일정각도 이상 기울어지면 볼이 움직여 스위치
역할을 하게 되어 기울기를 감지한다. 기울키 센서 모듈은 아래의 그림과 같이 기울기
센서 , 비교기로 구성된다．




                                                         Digita1 Output




                ［그림 入14] 기울기（Tilt) 감지 센서의 구성




                                7.5 기울기cn忙） 감지하71 - SW-520D 기울71 센서 1 137
+ Arduino



    기울기 감지 센서 모듈의 동작은 기울기 감지가 있는 경우와 없는 경우의 동작이 있다．
 우선기울기가 감지된 경우에는 기울기 센서 입력 전압이 기준 전압을 설정하는 가변 저항
 값에 따라 설정한 끼준 전압보다 작으면 비교기에 IA叭V 값이 출력된다. 출력된 값은 위의
 그림에서 보듯이 LED가 ON 된다. 하지만 기울기 센서 입력 천압이 거의 없다면 기준
  천압보다 커서 비교기에 I玉합l 값이 출력된다. 그러므로 比D는 OFF 된다. 아래의 그림과
 같이 기울기가 특정각도 이상이면 기울기 센서의 두 핀이 연결되어 센서출력 전압이 LOW
  로 출력 된다．
    따라서 비교기의 입력이 기준전압보다 작으면 비교기 출력은 LOW로 출력된다. 그러므
  로 I且）는 ON 된다. 반대로 기울기가 특정각도 이하이면 기울기 센서의 두 핀이 떨어져
  센서 출력 전압이 HIGH로 출력된다. 따라서 비교기의 입력이 기준전압보다 크면 비교기
  출력은 HIGH로 출력된다. 그러므로 LED는 OFF 된다.




                   1a 1卞公
 참고로 기울기감지 센서의 모양은 앞의 센서가 둥그런 금속 모양으로 바뀐 것 이외에는
앞 Chapter 화염감지 센서와 동일하게 생겼고 사용하는 방법과 센서의 출력 데이터도
동일하다. 그래서 하드웨어 연결무분과 회로 부분은 화염감지 센서와 동일하다고 생각하면
된다．



하드크궤에 연결

 기울기가 감지되었을 경우에 붉은색 LED를 켜기 위해서 LED를 아두이노보드의 D3
포트어］ 연결하고 화염감지 센서의 출력 핀（DO - Data Out）을 아두이노보드에서 입력으로
받아들이기 위해서 아두이노 보드의 D2어］ 연결을 한다．




               ［그림 가］6]   기울기 감지하기 배선도




                              7.5 기울기(Ti忙） 감지하기 - 9N-520D 기울기 센서 1 139
 1 Arduino e




                              3V3    5V        미N


                     RESET          Arduino              Tx/Do

                     RESET2           Uno                RXID1
                                                                  Fire Sensor
                                                                  Sensors

                     AREF           （日ev3)                 02

                     IOREF                             PWM 03
                                Nd미no UN（그日3
                                                            04

                     AO                                PWM 05

                     Al                                PWM 06

                     A2                                     07

                     A3                                     08
                                                                                LED2
                                                                                Ye如나 (595nm)
                     A4/SDA                            PWM 09

                     A5/SCL                         SS/P밖M ［기 0

                                                MO없／P넥M ｛기 1

                                                     뻬50/0俚

                                                       SCK/D13




                                          GNO



                                                                                         fr1tzing

                                    ［그림 石］7] 기울기 감지하기 회로도


   IL쿠기램1 작성

     화염감지 센서를 인식하는 코드와 동일하다．

     m1lt led = 3;
     m1lt sensor = 2;

     void setupO
     {
         pinMode(led, OUTPUT);
         pinMode(sensor, INPUT);
     }
     void loopO
     {
         if( digitalRead(sensor) == LOW)
            digitalWrite(led, HIGH);




1401 제7장 실제 세계와의 통로 센서
       else
                            m小m나：




              digitalWrite(led, Low);

       delay(100) ;
   }


亡it led = 3;

               기울기가 감지되었을 경우 알려주기 위한 匕ED 포트


mt sensor = 2;

               기울기 감지 센서의 DO0g怡 Out）와 연결한 아두이노 연결 포트


pin凡匠x兀伽d, OUTPU7力

              匕ED를 켜기 위해서 LED와 연결된 아두이노 포트를 OUTPUT으로 설정


ph小／次兆（s' en吼'I; 끄＼7)i/ 7方

               기울기감지 센서에서 입력을 디지털 입력을 받기 위해서 INPUT으로 설정


'if （加伽／Read(sen以끄少 == 工O)口 )

               기울기감지 센서와 연결된 아두이노 포트를읽어서 LOW이면 화재가 감지된 경우임


delay(100);

              ］초에 한 번씩 기울기를 감지하기 위해서 필요함．


실행결과

 기울기 감지 센서가 삽입되어 있는 브레드보드를 좌위 혹은 앞뒤로 기울여보자. 그러면
브래드보드에 있는 珏D가 켜질 것이다. 물론 기울기감지 센서 모듈에 있는 LED도 동시에
켜지게 된다. 브레드보드를 기울였을 때 제대로 반응하지 않는다면 기울기 센서에 있는
파란색 모양의 작은 가변저항을 십자드라이버를 이용해서 미세하게 조정한 이후에 테스트
하면 된다. 가변 저항을 이용하여 센서의 감도를 조정할 수 있다．
  여기서 아쉬운 점은 기울기 감지 센서는 특정 각도로 기울였을 때 센서에 있는 금속원통



                                        7.5 기울기(ri卄） 감지하기 - SV＼尸520D 기울기 센서 1 141
    사dumnb .




   안의 구슬이 금속원통에 닿았을 때 만을 감지하기 때문에 기울기의 각도 등은 알 수가
   없다. 조금 더 자세한 기울기 측정을 하기 위해서는 다음 Chapter에 있는 자이로 센서를
   이용하면 가능하다．




      7.6         진동 감지하71- SW-18020D 진동 센서


     진동 감지 실습은 진동 센서 모듈을 이용하여 진동을 감지하고 감지된 신호를 아두이노
   보드로 입력하여 적절한 제어와 출력을 할 수 있는 실습이다. 진동 센서 모듈은 진동을
   감지할 수 있는 모듈이다. 외부의 충격이나 진동에 의해 진동 센서 내부의 스프링이 좌우로
   흔들리면서 스위치 ON/Ol下 역할을 하게 되어 진동을 감지한다. 진동 센서 모듈은 아래의
   그림과 같이 진동 센서 , 비교기로 구성된다．




                                      4
    Shake Sen的r




                  4                              ;,
                                                      두   Digital Output




                      ［그림 갸］8]   진동｛Shake) 감지 센서의 구성



     진동 센서 모듈의 동작은 진동 감지가 있는 경우와 없는 경우의 동작이 있다. 우선
   진동이 감지된 경우에는 진동 센서 입력 전압이 기준 전압을 설정하는 가변 저항 값에
   따라 설정한 기준 전압보다 작으면 비교기에 'ow 값이 출력된다. 출력된 값은 위의 그림에
   서 보듯이 LED가 ON 된다. 하지만 진동 센서 입력 전압이 거의 없다면 기준 전압보다
   커서 비교기에 I-UGH 값이 출력된다. 그러므로 LED는 OFF 된다．
     아래의 그림과 같이 진통이 발생하면 진동 센서의 두 핀이 연결되어 센서 출력 전압이
   LC）叫로 출력된다. 비교기의 입력이 기준전압보다 작으면 비교기 출력은 LC）叫로 출력된다．



142 I 제7장 실제 세계와의 통로 센서
그러므로 LED는 ON 된다. 반대로 진동이 없으면 센서의 두 핀이 떨어져 센서 출력 천압이
HT(표I로 출력된다. 비교기의 입력이 기준전압보다 크면 비교기 출력은 I끄GH로 된다．
그러므로 I丑I升三 OFF 퇸다．




                            1그I目II
                            1rH H       ft
                               日
                               日
                               日
                               日
                               FR
                             口
                                    卞



                ［그림 石］9] 진동（Shake) 감지 센서의 동작


실험에 필요한 준비물들


                                                斗1
                                                                   二二；    .




                                                               ; 今動心小1



                                                         . *    小   나小1




                                                     1


          브래드보드 1개1                             아두이노 UNOR3




                                              가．』：.『"「i노
          1亨
      적색 I코D / 11( 저항 2가1                      진동감지 센서 17뀨



하드웨어 연결

 진동이 감지되었을 경우에 붉은색 I肋를 켜기 위해서 I丑D를 아두이노 보드의 D3 포트
어］ 연결하고 화염감지 센서의 출력 핀（DO - Data Out）을 아두이노 보드에서 입력으로
받아들이기 위해서 아두이노 보드의 D2어］ 연결을 한다．




                                         7.6 진동 감지하71- SW-18020P 진동 센서 1 143
  .   사duino




                                ［그림 가2이 진동 감지하기 배선도



                          3V3     5V         VI


                 RESET          Arduino                 TX/D0

                日ESET2            Uno                   RX/［기
                                                                     Fire Sensor
                                                                     Senso田
                                 (Rev3)

                                                                 ；色
                사4EF                                       O2
                 FOREF                                PWM O3
                            Arr加ins UNO R3
                                                           04    4
                  0                                   PWM D0

                 Al                                   P叩M D0

                 A2                                        D7

                 A3                                        D0
                                                                                   LED2
                                                                                   Yel山꿔 (595rr,n)
                 A4/SOA                               P나U Do

                A5/SCL                             SS/PWM O10

                                                  MO듸／PWM Oil

                                                     MISO/Di 2

                                                      SCK/｛기 3




                                       GNO




                                ［그림 가21] 진동 감지하:7 ' 회로도


1441 제7장 실제 세계와의 통로 센서
 m1로그램 작성

  스케치 코드는 화염감지 센서의 스케치 코드와 동일하다．

   mlli; led = 3;
   mllt sensor = 2;

   void setupO
      {
          pinMode(led, OUTPUT);
          pinMode(sensor, INPUT);
   }
   void loopO
   {
          if( digitalRead(sensor) == LOW )
             digitalWrite(led, HIGH);
          else
             digitalWrite(led, LOW);

          ctelay(100);
  }

立it led = 3;

             화재가 발생하였을 경우 알려주7J 위한 LED 포트

力it sensor = 乙

             화재 감지 센서의 DO(Digital Out)와 연결한 아두이노 연결 포트

pin凡伽徊兀d, OUTI兀／I力

             匕ED를 켜기 위해서 LED와 연결된 아두이노 포트를 OUTPUT으로 설정

pin凡仰de(sensor) 刃＼rpui方

             화재김仄1 센서에서 입력을 디지털 입력을 받기 위해서 八PUT으로 설정

if(d如rtalR匕ad(sen切i少 == 끄7V口 )

             화재감지 센서와 연걸된 아두이노 포트를 읽어서 LOW이면 화재가 감지된 경우임




                                             7.6 진동 감지하기 - SW-18020P 진동 센서 1 145
  (屯a忖i'z宕
           ］초에 한 번씩 진동을 감지하기 위해서 필요함．


  실행결과

   진동을 감지하는지 테스트하기 위해서 진동감지 센서가 삽입되어 있는 브레드보드를
  흔들어 본자. 그러면 브래드보드에 있는 I코D가 켜질 것이다. 물론 진동감지 센서 ' 모듈에
  있는 比D도 동시에 켜지게 된다. 진동에 제대로 반응하지 않는다면 진동감지 센서에 있는
  파란색 모양의 작은 가변저항을 십자드라이버를 이용해서 미세하게 조정한 이후에 테스트
  하면 된다. 가변 저항을 이용하여 센서의 감도를 조정할 수 있다．




     7.7      장애물과의 거리 감지하71 - 초음파센서


    우리 일상생활에서 초음파가 활용되는 생각보다 많다. 예를 들면 인체 진단을 위한 초음
   파 검사기, 어업을 위한 어군 탐지기, 초음파 세척기, 가습기 등 귀에는 들리지 않지만
   엄청나게 많은 분야에서 사용되고 있다．
    초음파 센서를 이용해서 초음파 센서와 장애물과의 거리를 감지해 보자. 보통 인간의
   가청 주파수는 161七N加ki七로 알려져 있다. 초음파란 인간의 가청 주파수를 넘어가는
   20k!七 이상의 주파수를 가지는 음파를 이야기 한다. 즉 인간의 귀로 듣는 것을 목적으로
   하는 음파는 아니다．




     동물들이 내는 초음파 주파수의 범위
       돌고래 : 약 170kHz
       박쥐 : 100Hz N 200kHz




     아래 그림은 주파수별로 정리한 용어를 나타내었다. 이번에 우리가 사용하는 주파수는
   20k!七사1GHz이므로 초음파（U뇨asonic）를 사용하여 실험을 하는 것이다．




1461 제7장 실제 세계와의 통로 센서
                   20Hz                   20kHz

        Subs어卄C           Audible sound
                                                  Ut11.1d                     I
                             ［그림 가22] 주파수대별 용어


      우리가 사용하는 초음파 센서는 HC-SR04 기뵨적인 원리는 초음파를 발생하여 장애물어］
     의해서 반사되어 다시 돌아오기까지의 시간을 거리로 계산하는 것이다．




                                                            장애물
                                      초읖괴까 뱐사
                                      되어 돌아읖




                          ［그림 가23] 초음파 센서의 작동원리


     HC-SR04 초음파 센서는 송신과 수신이 분리되어 있는 센서이다. 자세한 사양을 알아보
자．
         - 동작 전압 : 5V
         - 주파수 : 40k1-Jz
         - 최대 감지 거리          3m
         1 죄소 감지 거리 : 3cm


     초음파 센서의 감지 거리가 3cm- -3m라고 언급은 하였지만 모든 장애물질에 대해서
감지를 하고 있는 것은 아니다. 철사, 줄과 같은 초음파가 반사될 수 없는 가는 물체나
스펀지, 섬유, 눈 둥과 같이 천파를 흡수하는 물체에서는 초음파 센서로 올바른 거리를
측정하기가 곤란하다．




                                                  7.7 장애물과의 거리 감지하기 e 초음파센서 1 147
-.   A仄加m o +




     실험에 필요한 준비물들




                    브래드보드 17긔1             아두이노 t八OR3




                HC-SR04 초음파센서 17긔1




     하드웨어 연켤

      초음파 센서의 Thg핀을 아두이노 보드의 D13, Echo핀을 D12어］ 연결한다. 그리고 \/CC
     는 아두이노 보드의 5V와 연결하고 당연히 GND끼리 연결하면 퇸다. 아래 그림을 참조하면
     연결 배선이 복잡하지는 않다．




                                         目8 니
                                           bCHJUL < 1 t




                1
                ［그림 石24] 초음파 센서를 이용한 쟁개물과의 거리 감지하기 배선도


 1481 제7장 실제 세계와의 통로 센서
                                                                                              多
                               1
                               3V3    ！列         VIN


                      RE＄日           Aid미no                  TX/D0
                      RESET2           Uno                   只X/Dt
                      AREF            (Rev3)                   O2
                                                                             匕
                                                                                   SP0"
                                                                                 ovcc
                      心R든F
                                肉dumnb I丑4O R3             pw崩 O3                寸rig
                                                               O4
                                                                                 匹cho
                                                                                 匹的
                      A0                                   P밖M O5
                      At                                  P四MOE
                      AT                                       O7
                      A3                                       O8
                      A4/SOA                              PWM O9
                      AS/Sd[                           ss/pw｝따 ｛기 0
                                                  MOSI/PWM Dli
                                                         1川＄O/｛기2

                                                          sct<戎H3



                      N心




                                           ONO

                                           i
          ［그림 갸25] 초음파 센서를 이용한 징애물과의 거리 감지하기 회로도


쿠 그램 작성

아쿠이노 스케치에 아래와 갇은 코드를 작성한다．

#define trigPin 13
#define echoPin 12

void setupO
{
    Serial begin (9600);


    pinMode(trigPin, OUTPUT);
    pinMode(echoPin, INPUT);
}
long microsecondsTolnches(long microseconds)
{

                                                                     7.7 장애물과의 거리 감지하기    초음파센서 1 149
    Arduino .




          II According to Parallax's datasheet for the PING))), there are
          II 73.746 microseconds per inch (i.e. sound travels at 1130 feet per
          // second). This gives the 小stance travelled by the ping, outbound
          II and return, so we divide by 2 to get the distance of the obstacle.
          II See: http://www.parallax.com/cll/docs/prod/acc/28015-PING-v 1.3.pdf
          return microseconds / 74 / 2;
     I
     long microsecondsToCentimeters(long microseconds)
      {
          II The speed of sound is 340 rn/s or 29 microseconds per centimeter.
          II The ping travels out and back, so to find the distance of the
          II object we take half of the distance travelled.
          return microseconds / 29 / 2;
      }
      void loopO
      {
          long duration, inches, cm;

          digitalWrite(trigPin, Low);
          delayMicroseconds(2) ;

          digitalWrite(trigPin, HIGH);
          delayMicroseconds(10);

          digitalWrite(trigPin, LOW);

          duration = pulseln(echoPin, HIGH);

          II convert the time into a distance
          inches = microsecondsTolnches(duration);
          cm = microsecondsToCentimeters(duration);

          Serial.print(inches);
          Serial.print("inch, ");
          SerialSprint(cm);
          Serial.println(" cm");

          delay(100);
     I


150 I 제7장 실제 세계와의 통로 센서
戒屯line ti會I뇨7 13

        아두이노 트리거 포트 번호


#de而fle e*：方oPin 12

        아두이노 에코 포트 번호


Serial bc팜介l r啣七

        초음파센서의 실행 걸과를 아두이노 시리얼 모니터 프로그램으로 출력하71 위해서 필요하
        다．
Pit刃硏X七(0會尸巨7, 01/叩1/7方

        초음파 출력을 내보내기 위해서 0UTPUT 모드로 설정


／元11力r汰光r比加I物노 끄VI叱/7方

        반사되어 돌아오는 초음파를 입력으로 받기 위해서 INPUT 모드로 설정


加1喀 m庇끄石比t2iX古Toln力es口比茗 il 坑TVS比tMt丙)

        초음파이 반사되어 돌아온 시간을 거리(Inch）로 변환하는 함수로 초음파가 ] 인치 반사되어
        돌아오는데 73.746 microseconds가 소요된다는 것을 이용하여 거리를 계산한다．


I七(ii,月口 n址ins比Vfl(古 // 7手 / =

        위의 계산식에서 74로 나눈 이휘게 다시 2로 나누어주는 이유는 반사되어 돌아오는 시간을
        계산하기 때문이다．


五'I乷 n址ins比OLIC古ToCet油7JCtC心口01茗 n끄ci玎比on'云)

        초음파이 반사되어 돌아온 시간을 거리（Dii）로 변환하는 함수로 초음파가 ］센티미터 반사되
        어 돌아오는데 29 mi아oseconds 가 소요된다는 것을 이용하여 거리를 계산한다．


I七Oil刃 microsecom古 / 汐 / 2;

        위의 계산식에서 29로 나눈 이후에 다시 2로 나누어주는 이유는 반사되어 돌아오는 시간을
        계산하기 때문이다．




                                       7.7 장애물과의 거리 감지하71 - 초음파센서 I 151
    ／놔duino .




   a會亢a/Write作t智Pin, 끄7W方
   delay.兀ficrosecon小(2七
   (／會ira!Write伽智Pin, 月k끄助
   de切凡ficrosecon小(II功
   d會亢可Write(rr會Pin, 끄7V已tr
            트리거 신호를 발생시키는 코드이다．


   duration = pu/seln(比奴寸기11, 丑／Gi助

            pulseln() 함수는 echoRn 포트가 HIGH가 될 때까지의 시간을 micr呻conds 단위로 리턴해
            준다．


   立1':方es = n끄rcrosea刃1小ToIt兀方es(d口ration方
   cm = 끄끄rcrOsecondsTOCei끄立nerers(miration方

            각각 인치와 센티미터로 변환을 수행해 주는 함수를 이용해서 시간을 거리로 변환한다．


   실행결과

     초음파 센서를 테스트 하는 방법은 간단하다. 아두이노 보드에 위의 스케치 코드를 업로
   드 하고 초음파 센서를 간단하게는 손이나 초음파 센서를 흡수하지 않는 물체를 이용해서
   가리께 되면 아두이노 시리얼 모니터에 초음파 센서와 장애물과의 거리를 inch와 cm로
   나누어서 표시를 해준다．




            目가
                  r命coM:9                                            ;，口哨好h旴可




                  r口
                       Autoscroll               Carriage return. r   9600 baud   J
                                                                                 小




                                    ［그림 가24] 초음파 센서 실행결과




152 I 제7장 실저1 세계와의 통로 센서
모터 제어하기

8. ]   소형 DC 모터 사용하기
8.2 서보모터 제어하기
8.3 스테핑 모터
m+ 사duino S




   모터가 사용되는 분야는 굉장히 광범위 하다. Deskt叩 PC의 DVD ROM, HDD에도
  모터가 사용이 되고 런닝 머신, 전동드릴, 선풍기 등 전력에 의해서 뭔가가 움직이는 분갸어］
  는 거의 모두 모터가 사용되고 있다. 모터의 종류에도 여러 가지가 많지만 이번 장에서는
  앞 장에서 디지털 입출력 관련 동작들과 센서사용 법에 관한 내용에 이어 DC모터, 서보모
  터 , 스텝모터의 제어에 대해 살펴본다．




              소형 DC 모터 사용하71


    작은 DC 모터들은 무선 조종 자동차와 보트, 전기 자동차 창문, DVD 플레이어 등
   다잉촨 장치에서 짖아 볼 수 있다. 소형 모터들은 일반적으로 1.5에서 30 볼트의 전원을
   사용한다. 그리고 모터 제조사들은 모터들에 대한 사용법을 제공해 준다. 모터를 구마1
   할 수 있는 곳은 다양하다. 요즘은 온라인 쇼핑몰이 잘 되어 있어 온라인에서 쉽게 구매
   가능하다．
    모터에 권장 이상의 전압을 가하면 모터의 코일이 손상된다. 그리고 너무 적은 전류는
   모터를 구동할 수 없다. 모터는 정회전과 역회전이 가능한데 DC모터에서는 역회천을 하려
   면 연결된 전원 선을 반대로 연결해 주면 된다. 작은 모터로 큰 힘을 내려고 하면 기어
   박스를 사용한다. 기어 박스는 고속 회전을 내는 DC 모터에 큰 출력의 힘（Torque）을 낼
   수 있도록 만들어 준다. 아두이노 보드는 모터를 충분히 구동할 수 있는 천류를 제공하지
   못한다.
     그래서 모터를 구동하기 위해 외부 전원을 공급해 주어야 한다. 아두이노 보드를 이용하
   면 모티의 Oii/O珏와 속도 조절도 가능하다．
     이번 실험에서 기어박스가 있는 DC모터와 모터를 정회전과 역회전을 시키기 위해서
   L293B 모터 구동 드라이버 IC를 사용할 것이다. L293B는 각 채널당 최대 1A의 전류를
   공급하여 모터를 27初切］ 구동할 수 있다．




154 1 제8장 모터 제어하기
                              ［그림 乎］]       기어박스가 장착된 모터


 기어박스가 있는 DC모터는 무선 RC자동차, 탱크 둥의 바퀴를 구동하는데 웅용해서
사용하기에 적당하다．


실험C카 필요한 준비물들

                                      薑玉 卄
                                  y           :, cx今        小   寸m , .   ,       ,,       m   可   』   a크＞        ：月




                                                                             L293B
                                                           卞4   ！뇌           m        q       U1      띠     r\   m

                                         a.     小      小
                                        S


       브래드보드 17뀨                      아두이노 UNOR3                L293B 모터 IC 17뀨



                          莎


                                         卄
                     뉵生
             牙   ;




             平戶戶
   뇨



   기어박스 DC 모터                     1N4003 다이오드 2깨1



하드웨어 연결

 4개의 다이오드와 L293B IC를 아래 그림과 같이 아두이노와 연결해 주면 되는데, 부품을
배치하기 전에 L293B IC의 각 핀들의 이름과 기능에 대해서 먼저 알아보자．




                                                            8.1 소형 DC 모터 사용하기                                         ]55
 .   Arduino 孕



                                                 4上
                            Motorl Enable                          VSS(4.5 - 36V)
                                                  (
                                   Input 1-1    斗
                                                J
                                                                   Input 2그




                                                       尸N山Wm
                                                 그나
                                  Output 1-1                       Output 乙2
                                                 41
                                        GND                        GND
                                                 <J
                                        GND                        GND
                                                               n
                                  Output 1- 2                      OutF：八it 二1
                                                               m
                                    input 1그                       Input 石1

                                 VS(35V Ma지                        Motor2 Enable


                                   ［그림 斗2]            L293B 핀 배치도



      핀 번호                                                     핀 설명

                  - Motorl Enable
                  - DC 모터의 경우 모터 1번의 회전 속도를 결정
         1        -1번 핀을 1-ilGI｛로 주면 최대의 회전 속도를 내고 PWM을 이용하여 Analogs刃i-i呵핀번
                    호, 128) 함수를 사용하면 모터의 회전속도를 5cY兀로 조정할 수 있다．
                  -1번 핀을 LO町로 주면 1번 모터가 동작하지 않는다．
                  . 모터 Input 1-1
                  - Input 1-1, It巾Ut 1-2는 1번 모터의 회전 방향을 결정한다．
                  - Input 1-1 을 HIGH로 주고 Input 1-2를 ID峴로 설청하면 청 방향으로 모터가 움직이고
                    반대로 Input 1-1을 LC）叩로 주고 Input 1-2를 HIGH로 설정하면 역 방향으로 모터가
          2         움직인다. 이것을 표로 정리해 보자．

                          모터 회전 방향                         Input ］너                 Input 卜2
                            정방향                              1丑GH                      LO町
                            역방향                               LO町                     HIGH

                  - 모터 Output 1-1
          3
                  - Output 1-2 핀과 함께1DC 모터에 있는 2개의 연결선 중에 한쪽어］ 연결
         自5       - GND
                  - 모터 0utput 1-2
          6
                  - Output 1-1 핀과 함께 DC 모터에 있는 2개의 연결선 중어］ 한쪽에 연결
                  - 모터 Input 1-2
          7
                  - Input 1-1 참조
          8       - 모터 구동 전원（최때I 36V)
      9, 10, 11   - M야onl 참조
        12,13     - GND
        14,15     . 八4（孔onl 참조
          16      - 모터 구동 IC 구동 전원（4.5- 36v)



156 I 제8장 모터 제어하기
                          ［그림 마3]                DC모터 제어하기 배선도




         3V3     50         니14                  L293)
日ESET          Arduino                   TX/DO

日ESET2           Uno                     RX/Ol

AREF            (Rev3)                     D2
                                                                                    !CI
OREF
           Arduno UN0 63
                                       PWM 03       나1- 앉4001                     L293D
                                  "        04
                                                                         ]
AU                                     P나M 05                                6141            V

Al

A2
                                       P넥M D6

                                           07
                                                           Ml
                                                                         三   1141

                                                                             Dull
                                                                                           IN4

                                                                                          0UT4
                                                                                                 =．三1
                                                                                                 =．三＝
                                                                         4
A3                                         08                                ov             Xv
                                                                         5
A4/SDA                                 PWM 09                                 V             0v
                                                                         6                              11
A5/SCL                            SS/PWM 010             021N4。。1            0U12         OUT3 H
                                                                                                        10
                              MO듸／P小月너 ［기 1                                  1N2           1143 1
                                                                                                        9
                                      뻬SO/ 012                                Vmotor       EN2 1
                                                                    中寸
                                       scqo化



N/C




                      GND


                      1
                                                                                                        fritzlrog

                          ［그림 마41 DC모터 제어하기 바썬도


                                                                         8. ] 소형 DC 모터 사용하기 I 157
  .   Arduino e



       위의 그림에서 모터드라이버 IC의 이름이 L293D로 되어 있지만 실험에서 사용한 드라이
      버 IC는 L293B를 사용하는 것이 맞다．


      끄쿠기램 작성

       아두이노 스케치에 아래와 같은 코드를 작성한다．

       #define motor lEnablePin 9
       #define motor1 1         2
       #define motor1 2         4

       void setupO
       {
           I加IVIode(mo切ri그, OUTI兀JT);
           pinMode(mo的ri그, O1玎I兀JT);
           analogWrite(motorlEnablePin, 0);
       }
       void loopO
       {
           dligitalWrite(motorl_1, HIGH);
           digi捌Write(mo切ri그, L（쪼w);
           analogWrite(motorlEnablePin, 1023);
           delay(2000);
           analogWrite(motorlEnablePin, 50);
           analogWrite(motorlEnablePin, 0);
           delay(1000) ;

           digitalWrite(motor1_i, LOW);
           digital＼자rite(mo切ri그, HIGH);
           analogWrite(motorlEnablePin, 128);
           delay(2000);
           analogWrite(motor lEnablePin, 50);
           analogWrite(motorlEnablePin, 0);
           delay(1000);
       }




1581 제8장 모터 제어하기
 壯兀作ne n丑7rorlEnabk下初 9

        DC 모터의 속도를 조정할 수 있는 아두이노 보드의 포트번호


 券匕在？hne niororl 1       2
        L293B 모터드라이버 IC의 In口Ut 卜］과 연결된 아두이노 보드의 포트번호


 戒兀／됴祀 ni(札on 2          手
        匕293B 모터드라이버 IC의 In口Ut 卜2과 연결된 아두이노 보드의 포트번호


1끄'7兀匠de在notorl工 ()tJ1PUT);
p血Mo七伽otorl小乙 ()UIII叱及方

        모터드라이버 IC의 In口Ut 卜j고F In口Ut 卜2를 제어하기 위해서 출력으로 설정한다．


 aria兀팜Write在notor／且iablePin, Q七

        초기어는 DC모터의 속도를 0으로 한다．


（抑ita!Wi元e伽m才I工 丑16吼七
diiraJWi*e(motor12, LOW).;

        DC 모터를 정 방향으로 회전하도록 설정한다．


an匹／qgWrire(moror1Ei伍砒件i, 102弦
        DC 모터를 정 방향으로 가장 빠르7카 회전시킨다．


analogWi沅e6刃otorl蜀7砒泌I뇨I노 多a七
analogWi元e(rnotonl月7ab1eP뇨乙 a七

        DC 모터의 속도를 서서히 감소시키다가 멈추도록 한다．


（如itaiWi伽(n奴on 1夕 끄71r方
（如ita11好伽白겊7torl乙 丑IGIL七

       DC 모터를 역 방향으로 회전하도록 설정한다．


an洌曾Wi北e白꼬,torlEnablei功兀 128七

       모터의 속도를 ]/10 속도로 회전시키도록 한다．




                                           8.1 소형 DC 모터 사용하기 1 159
  .   Ard내no



      실행결과

       2초에 한번씩 DC 모터가 정 방향으로 회전했다가 역방향으로 회전하기를 반복한다．
      이 코드를 잘 이용하면 I乂 모터를 사용한 RC카 등에서 리모컨을 이용해서 자동차의 속도를
      조절하는데 응용할 수도 있고 생각해 보면 응용 범위는 무수히 많다．




        8.2        서보모터 제어하:7 '


       서보 모터는 RC 장난감에서 흔히 볼 수 있다. 비행기의 날개, 보트의 방향키, 자동차의
      앞 바퀴 조향 장치에 들어가 있다. 서보 모터는 기어로 되어 있어 설정한 각도로 돌릴
      수 있다. 일반직으로 0에서 180도까지 움직일 수 있고, 4.8V 전원을 공급한다．


      실험에 필요한 준비물들




                                                   二
                                        ;CX9



                                   11    1小 HHH1
                                  1

               브래드보드 17)
                       1      아두이노 I八OR3           서보모터 17官




      하드웨어 연결

       서보 모터를 제어하기 위한 배선 연결은 I乂 모터보다는 단순하다. 서보 모티에는 3개의
      디드선이 나와 있는데 붉은색은 5,'/ 천원에 검은색은 GND에 연결하고 노란색은 아두이노
      보드의 D8 출력포트에 연결한다．




1的 1 제8장 모터 제어하;71
             ［그림 마5]               서보모터 제어하기 배선도




                             \qN


    日ESET        Arduino                 TX/D0

    日ESET2         Uno                   AX!［기
    A日EF          (Rev3)                    D2
    口REF                               Pwl너 03
              知d너ne 1外幻 R3
                                            04
    AU                                 P畔M 05
m   Al                                 P네 小 06
m   A?                                      07
中   A3                                     08
H   A町SDA                             P넥? i 0F
m   A5/SCL                         OS/P낵小d ［기 0

                              MOSI/PWM DII

                                     1키5O/012

                                      SCKID13




                      GNU


                       1
             ［그림 十6]           서보모터 제어하기 회로도


                                                   82 서보모터 제어하71 1 161
    Arduino



   프로그램 작성

     아두이노에는 이미 서보 모터를 제어하기 위한 훌륭한 라이브러리를 갖추고 있다. 뿐만
   아니라 다음 절에서 다루게될 스테핑 모터 제어 라이브러리도 있다．

     #include <Servo.h>

     m1lt motor control = 8;
     Servo servo;

     void setupO
      {
          servo. attach(m毗야下ontro ;
     }
     void loopO
      {
          m1lt i;


          servo. write(O);
          delay(1000) ;

          如r(i=0;i<1羽;i+=10)
          {
              servo. write(i) ;
              delay(20);
          }
          delay(1000);
      }


   抑址加de (Servo.h)

                서보모터 라이브러리를 사용하기 위해서 반드人1 추가하1 주어야 한다. 다시 말하지만 아두이
                노 개발환경에서 인클루드 헤더 파일은 대소 문자를 구분하기 때문에 유의해서 코드를
                작성해야 한다．


   mt m兀（叱cc玎itrol = 8;

                서보모터의 가운데 리드선인 펄스 핀과 연결된 아두이노 보드의 포트 번호




162 1 제8장 모터 제어하기
    Servo servo;

            서보모터 제어 라이브러리를 사용하기 위한 변수 선언


servoS arrach(moror_control);

            서보모터에 펄스를 공급해줄 아두이노 보드의 포트 번호를 라이브러리에 전달하1．준다．


servo. Wi北e(0七

            서보모터의 각도를 0도로 초기화한다．


尼r在＝＝口）了／8口1+=1勿
I
     servo. wi介e在七
     de1ay(20七
I
            서보모터를 0도에서 ]0도씩 180도가 될 때까지 회전을 시킨다．


실행결과

     실행을 시키면 1초에 한 번씩 서보 모터가 0도N娼0도까지 10도씩 회전하고 다시 1초
후에 0도로 돌아온 이후에 0도Nl&）도까지 10도씩 회전하기를 반복한다. 테스트를 해보면
서보 모터는 DC모터와 스테핑 모터와 다르게 0- 360도를 회전하지 않고 180도까지만
회전하는 특징을 가지고 있다．




      8.3        스테핑 모터


     스텝모터는 정교한 움직임을 제어할 수 있는 모터이다. 그래서 이 모터는 정밀한 제어가
필요한 3') 프린터나 (NC 가공기 등에 사용된다. 스텝모터는 프린터기 헤드나 종이 공급기
어］ 보면 많이 사용된다．
     스텝모터의 구분은 일반적으로 모터의 크기에 따라 분류된다. 그리고 같은 외형 크기에
서도 모터의 길이가 I기 긴 것은 더 큰 힘을 낼 수 있다. 스텝모터에는 유니폴라와 바이폴라
두 종류가 있는데, 정밀하면서도 강한 힘을 필요로 하면 바이폴라 모터를 사용하면 되고，
간단한 프로젝트에 저가형 제품이 필요하면 유니폴라 모터를 선택하면 된다. 그러면 스테
핑 모터의 구조와 제어 방식에 대해서 구체적으로 알아보자.


                                                   8.3 스테핑 모터 I 163
-.   Arduino .



     스테핑 모터의 종류

      스테핑 모터는 회전자但야아）의 종류에 따라서 크게 3가지로 구분한다．


       영구자석（Permanent Magnet)
      회전자（Rotor)가 N/S 극성을 갖는 영구자석으로 자화되어 있다．
     寸 가변 릴럭턴스（Variable Reluctance))
       회천자但야or）가 자석의 성분은 갖지 않지만 마지 기어의 톱니와 같이 회전자의 표면에
       홈이 새겨져있다．
     1 하이브리드（Hybrid)
       회전자（Rotor）가 N/S 극성도 가지며, 표면에 홈이 새겨져 있다．


       참고로 우리가 이번 실험에 사용할 모터는 영구자석을 사용하게 될 것 O 다．


     스테핑 모터의 구조

       스테핑 모터를 분해를 해보면 아래 그림과 같은 구조로 되어 있다. 크게는 회전자但아or)
     와 고정자（Sta幻r）로 구성되어 있다．




                                       巾
         스테핑 모터                            스테핑 모터 분리도




            스텝모터                                   고정자（S切幻r)   덮711
                             덮711      회전자（R아or)

                            ［그림 마7]     스테핑 모터분리도



      스테핑 모터의 구동 원리

        아래 그림과 같이 스테핑 모터는 권선 즉, 4선（바이폴라 보터）, 혹은 6선（유니폴라 모터）
      어］ 전류를 순서대로 흘려보냄으로서 고정자와 회전자 사이에 전자기력을 발생시켜 모터의
      중간에 있는 회전자（Rc乂or)를 자기력에 의해서 회전시키는 것이다．


1641 제8장 모터 제어하기
                                      권선으로 전류를 흘려줌

                                       코일의 전류가 흐름

                                     고정자의 생긴 전자기력으
                                      로 인히1 극성이 발생

                                     고정자와 회전자 사이의 자
                                         기력 발생

                                      회전자가 자기 력에 의히1
                                          회전함
                                       다른 권선의 전류를
              궈느
                                     흘려주면 회전자가 회전함

                      ［그림 予8]   스테핑 모터의 구동원리



실험에 필요한 준비물들




              브래드보드 17긔1                   아두이노 UNOR3



          -




      L293D 모터드라이버 IC                  kh42hm2-901 스테핑 모터 1가1




하드웨어 연결

 간단하거］ 스테핑 모티에 대해서 알아보았고 이제 실제로 결선을 하여 스테핑 모터를
구동시켜 보자. L293D IC를 아래 그림과 같이 아두이노와 연결해 주면 되는데, 부품 을
배치하기 천에 L293D IC의 각 핀들의 이름과 기능에 대해서 먼저 알아보자．



                                                      8.3 스테핑 모터 1 165
 -. Arduino .




                          1,2 Enable         VSS(4.5 사 36V)
                                 1A          4A
                                 ly          4Y
                               GND           GND
                               GND           GND
                                 2Y           3y
                                 2A           3A
                        VS(35V Ma지            3,4 Enable


                             ［그림 아8]   L293D 핀 배치도



      핀 번호                                핀 설명
                - 1,2 Enable
         1      -1번 핀을 HIGH로 설정해야 스테핑 모터를 구동시킬 수 있다．
                -1번 핀을 LO町로 주면 스테핑 모터가 동작하지 않는다．
                口 lAW나1)
         2      - 스테핑 모터의 A 제어
                - 아두이노 보드의 D8 포트에 연결한다．
                - lyK)Ti丁1)
         3
                - 스테핑 모터의 3번 선과 연결한다．
        自5      - GND
                口 2Y(OUT2)
         6
                - 스테핑 모터의 1번 선과 연결한다．
                - 2A(IN2)
         7      - 스테핑 모터의 A' 제어
                ' 아두이노 보드의 D9 포트에 연결한다．
         8      - 모터 구동 전원（최때1 36V)
                - 3,4 Enable
         9      -9번 핀을 HIGH로 설정해야 스테핑 모터를 구동시킬 수 있다．
                -9번 핀을 LOW로 주면 스테핑 모터가 동작하지 않는다．
                - 3A(IN3)
         10     - 스테핑 모터의 B 제어
                - 아두이노 보드의 1끄0 포트에 연결한다．
                尸 3Y(Ol了T3)
         11
                - 스테핑 모터의 6번 선과 연결한다．
        12,13   - GND




1661 제8장 모터 제어하기
          4Y（아了T4)
   14
        - 스테핑 모터의 4번 선과 연결한다．
        - 4A(IN4)
   15   - 스테핑 모터의 B' 제어
        - 아두이노 보드의 Dli 포트에 연결한다．
   16   - 모터 구동 IC 구동 전원（ 4.5-'36V




 L293D는 바이폴라와 유니폴라 모터에서 두 종류 모두 사용할 수 있다. 실험에서 사용하
는 스텝 모터는 유니폴라 모터를 사용한다. 아두이노 디지털 포트 D8번부터 Dli번을
L293D의 제어 핀에 회로도와 같이 연결한다. 유니폴라 모터 결선을 할 때 6선이 나와
있는데 L293D와는 4개의 선만 연결하면 된다. 모터의 중간에 있는 2번과 5번 라인은 연결
하지 않아도 된다．




              ［그림 8-10]   스테핑 모터 제어하기 배선도




                                            8.3 스테핑 모터 1 167
 .   Arduino 1




                          3V3     5V         ＼기卜寸

                                                                                                         'Cl
                 RESET          Arduino                 TX/DO
                                                                                L293D
                 RESET2           Uno                   RX/［기
                                                                       ]
                 AREF            (Rev3)                    02
                                                                           EN1                 V
                                                                       2
                                                                           IN1
                 回REF                                  PWM 03
                            Arduino UN0 83                                                          4
                                                                           0UT1         OUT4
                                                           04


                                                                      寸
                                                                                                    13
                                                                           Dv                 oV
                 AO                                    p넥M 05
                                                                                                    12
                                                                           Dv                 0V
                 At                                    PWM 06
                                                                       6
                                                                           0U12         OUT3
                 A2                                        07
                                                                       7                             0
                                                                           1N2               1！寸3
                 A3                                        08
                                                                           +Vm아or            E 2
                 A4/SDA                                p나M D9

                 A5/SCL                             SS/to叩M［기0

                                               MOSI/P넥M Dli

                                                     씨So'｛기2

                                                       SCKJDt3
                                                                      r\   口

                                                                                     녘멈召刃

                                                                                     <O니O刃



                                                                                 量
                                       GND


                                       i
                                                                                                               fritzirtg


                                    ［그림 乎］1]                스테핑 모터 제어하기 회로도


      쿠기램 작성

      아래 스케치 코드는 스텝 모터를 한 스텝씩 움직이게 하는 코드이다. 다행히 아두이노에
     서는 유니폴라와 바이폴라를 지원하는 스테핑모터 라이브러리를 제공한다. 이러한 라이브
     러리가 없다면 아마도 스테핑 모터 구동을 하는 스케치 코드를 작성하는 것이 쉽지만은
     않았을 것이다．




1681 제8장 모터 제어하기
      #include <Stepper.h>

      const mrlt stepsPerRevolution = 200;
      Stepper myStepper(stepsPerRevolution, 8,9,10,1?);

   void setupO
      {
          myStepper. setSpeed(100);
   }
   void loopO
      {
          :Lnt i;

          for(i印,1但00;i++)
          」1
                myStepper. step(1);
                delay(10);
          }
          for(i=0 ;i <200;i++)
          {
                myStepper. step(- 1);
                delay(10);
          }
  }

抑ndude (St印戶er．方J

               스테핑 모터 라이브러리를 사용하기 위해서 헤더 파일을 추가해주어야 한다．


口nst 力It St아'SF匕rRevolurion = 2兀彦

               우리가 사용하는 스테핑 모터는 ］스텝에 ] .8도를 회전하는 모터이다. 그러므로 360도를
               회전하기 위해서는 200 Resolu化n을 갖는다. 예를 들어 모터가 스텝 각이 ] .5도이면 360
               / 1.5 = 24001 된다. 0I 밀은 모터가 한 바퀴 도는데 24{) 번의 스텝이 필요하다는 것이다．


Stepper n砂＆아Y光H計아）可七i丑evo1uti加， 影t끄工／1);
               스테핑 모터 라이브러리를 초기화 한다. ／누A'-탸B'를 제어하는 아두이노 보드의 디지털
               포트를 순차적으로 나열하면 된다．



                                                             8.3 스테핑 모터 1 169
  .   Ard山10 卜中




      mySrepper. set毋,eed口a2七
             setSpeed() 함수는 ］분당 모터의 회전수를 설정하는 함수이다. 0I 함수는 모터를 실제로
             회전하게 하는 함수는 아니지만, 회전 시 회전 속도를 조절할 수 있다．


      mySrepper.stepW;
             실저로 스테핑 모터를 회전시키는 함수이다. 여기서 " l "이라는 값은 200이라는 R廣）이내ion
             을 갖는 스테핑 모터를 200 스텝 중 ］스텝을 회전하라는 것이다. 스테핑 모터를 반대로
             회전시키71 위해서는 이 함수에 마이너스 값을 넘겨주면 된다．


      실행결과

        스케치 코드를 실행시키면 정회전과 역회전을 200 스텝으로 360도씩 반복해서 회천한
      다. 실행 시에 주의해야할 사항은 L293D IC는 오랫동안 사용하게 되면 과열이 되어서
      오동작을 할 수 있다. 그래서 실제 제품을 구현하는 경우에는 L293D IC에 알루미늄 등의
      방열판을 부착하여 열을 식히거나 냉각팬을 가동시켜 과열이 되는 것을 방지해야 한다．
      이것은 스페팅 모터도 마찬가지이기 때문어］ 보통 모터를 장시간 쉬지 않고 사용하기 이해서
      는 모터에도 냉각팬을 설치하여 열을 식히면서 사용해야 한다.




170 1 제8장 모터 제어하기
디지털 통신
 인터페이스
9. ] 디지털 통신 인터페이스 개요
9.2 120 통신 규약
9.3 120 통신으로 자이로 센서 사용하기
         - L3G4200D
9.4 SF：가 통신 규약
9.5 SF가 통신으로 자이로 센서 사용하기
      - L3G42OOD
9.6 자이로 센서로 서보모터 제어하기
  .   Arduino .




        9.1       디지털 통신 인터페이스 개요


       I2C와 SPI 통신은 센서들과 아두이노 보드를 간단히 연결해서 사용할 수 있는 통신방식
      이다. 아두이노에서는 I2C와 SPI를 라이브러리로 제공하고 있어 사용자는 단순히 라이브러
      리를 호출해서 사용하면 된다．
       I2C는 2개의 신호선 만을 이용하여 여러 장치들을 아주 쉽게 아두이노와 연결할 수
      있다. 그리고 이 2깨의 선을 통해 신호를 통신한다. 그렇지만 I2C 통신은 SPI어］ 비해 통신
      속도가 느리다. I2C의 신호선 들에는 반드시 풀 업 저항을 달아 사용해야 한다．
       SPI는 입력과 출력 연결이 분리되어 있어 동시에 읽고 쓰기를 할 수 있으므로 데이터
      천송 속도가 빠르다. 그렇지만 장치별로 선택하기 위해1 각각의 연결선이 필요하다. 그래서
      대용량의 데이터 전송이 필요한 이더넷이나 메모리 카드는 SPI 통신을 사용하게 된다．
       I2C 통신을 통해서 인터페이스하는 주변 장치들은 주로 카메라 센서, 자이로센서, 가속도
      센서 등이 있고 SPI 통신을 통해서 인터페이스하는 주변 장치들은 MP3 코덱 저속 SD
      메모리 카드, SPI 플래시 메모리 둥에 주로 사용이 되고 있다．




        9.2       I2C 통신 규약


       I2C 통신 규약에 대해서 자세히 알지 못해도 아두이노에서 I2C 통신을 이용해서 실험을
      하는 테에는 아무 문제도 되지 않는다. 이미 아두이노에는 쉽게 바로 사용이 가능한 I2C
      라이브러리를 제공하고 있기 때문이다. I2C 통신에 대해서 완전하게 이해하기를 원하는
      독자만 이 절을 읽어도 된다．
       I2C 통신은 SCL(Serial clock）과 SDA(Serial data）의 2개의 통신선을 이용하여 주변의
      저속 디바이스들과 연결된다. 아두이노 보드에서는 아날로그 핀 5번을 Sc'로 사용하고
      아날로그 핀 4번을 SDA로 사용한다. 단, 入1ega 보드에서는 디지털 20번 핀을 SD心i 21번
      핀을 SQ.로 사용한다. 우리는 아두이노 Mega 보드가 아닌 아두이노 1介qOR3 보들 사용할
      것이다.
       I2C 버스에는 하나의 마스터와 하나 이상의 슬레이브를 연결해서 통신할 수 있다. 마스터
      는 SCL 클럭을 움직이고 통신의 시작과 끝을 제어하는 주체이다. 슬레이브는 이 클럭
      신호에 동기화해서 데이터를 내어주거나 받게 된다．


172 I 제9장 디지털 통신 인터페이스
                                                                             VDD
       Arduino                                                                                        마ocessor
       I2C Master                                                         Fh川．up 저함        :          I2C 듸ave


                               墅          I


                                                 1
                                                                                                      饗
                                                 V                 V         '   V
                                               EEPROM           FLASH      Sensor...
                                              12C 引ave


                                                      ［그림 아］]          20 통신 구성 0카


     여러 개의 슬레이브 디바이스가 I2C 버스에 연결되어 있을 때, 각각의 슬레이브 디바이스
들은 각자 고유한 어드레스를 가지게 된다. I2C 통신을 마스터가 시작하게 되면 통신하고자
하는 슬레이브 디바이스의 어드레스가 가장 먼저 날아오게 된다．


                                                                                                                          尸       1       1




      SDA




      SC

            1   S 1                                                                                                                   P
            1    -    I             II           IL_______1 1             II..       J l                  1目         1        4       4       U




        ST사iT             ADDRESS        由':1'       Ac未         DATA        ACK               DATA            ACK        STOP
       口ond油on                                                                                                           zandition
                                                                                                                              V巴Cm4




                                                     ［그림 아2]      I2C 데이터 통신 구조


     I2C통신은 위의 그림과 같이 S切式 조건으로 시작해서 Sop 조건으로 한 통신이 이루어진
다．
                                                                                                          9.2 I2C 통신 규약 1 173
  .   Ard네no .




       SDA                                                       SDA




       SCI                                                       SCL



                   Start                                 St叩
                 Condition                             C이寸II여｝

                             ［그림 아3]   I2C 데이터 통신 구조



       위의 그림을 보면 SCL 라인이 HIGH인 상태에서 SDA가 LO明로 내려가면 I2C 통신의
      시작을 알리는 Start 조건이 퇸다. 그 이후로 슬레이브의 어드레스 데이터가 나가게 되고
      마스터에서 슬레이브로 데이터를 Write하는 통신（LOW）인지 아니면 Read하는 통신
      (HIGH）인지 구분하는 1개의 비트가 오고 그다음에 ACK와 실제 DATA 그리고 마지막으로
      SCL이 HIGH인 상태에서 SI殆가 LO町에서 HIGH로 가면 St아） 조건이 되어서 I2C 통신이
      종료가 된다．




        9.3        I2C 통신으로 자이로 센서 사용하71 - L3G4200D


       이번 절에서는 I2C통신을 이용하여 L3G4200D 자이로 센서 모듈에서 데이티를 가져
      오는 실험을 해보도록 하겠다. 자이로 센서란 각속도를 측정하는 모듈로 한축을 기준으로
      단위시간에 물체가 회천한 각도의 값을 수치로 알려주는 센서이다. 이러한 기눙으로 최근
      어］ 스마트폰에서 모션 인식 기능으로 많이 사용이 되고 있다．
       스마트 폰으로 즐기는 자동차 게임 중 버튼을 이용하지 않고 모션으로 운전을 하거나
      비행 시뮬레이션 게임 등이 자이로 센서를 이용한 것이다. 스마트 폰 이외에도 쿼드콥티，
      드론 비행체 등에서 널리 이용되고 있다．




174 I 제9장 디지털 통신 인터페이스
                 ［그림 아4] 자이로 센서 회전각 축


 자이로 센서의 위의 그림에서와 같이 3개의 출력 데이터가 있는데 x축을 기준으로 x축은
좌우의 회전각(ro끄）,y축은 앞뒤의 회천각（pitch), z축은 평면에서의 회전각（yaw）의 출력을
갖는다．


실험에 필요한 준비물들

                      望笠 1                          L3G11 己 U口 D
                              ;c9 1    1        金 GNU    x    INT 1
                                                可S끄A    yZ     끄R 1
                                                臼 SCL          CS S
                                                自 vCC        SU0 S
                         a.    -       1
                        S

    브래드보드 17月         아두이노 UNOR3               L3G4200D 자이로센서



하드워他1 연결

 L3G4200D 자이로센서 모듈 왼쪽에 SI沮, SCL, GND, VCC라고 표기된 4핀을 아두이노
보드와 연결한다. 자이로센서 모듈에 SDA와 SCL핀은 I2C 통신을 위한 핀으로 SDA는
아날로그 포트 A4번에 SCL은 아날로그 포트 A5번에 연결한다．




                                   9_3 a二 통신으로 자0로 선써 人용하기-뗘34a乂O 1 175
  簪




           !!
           !!
           !!
           ::
           e 1




                          ［그림 아5] 자이로 센서 I2C 방식 배선도




                  qES亡T        Ar出Jino            Tx/D0

                  RESET2         Uno              AX/Ol

                  AR횬F          (Rev3)              ［芷

                  心REF                          P나U ［乂
                            MujflO U村O 日a
                                                     O4

                  AS                            PWM D5

                  Al                            P낵U OF

                  A2                                 O7

                  A3                                 O6

                  A司SDA                         PWM O9

                  A旬SCL                      SS/PWM Dl

                                            MO듸幷꺼叩U Oil

                                               씨 S｛그／O12

                                                Sc田Di T



                  N/c




                          ［그림 아6]           자이로 센서 口C 방식 회로도


176 i 제9장 디지털 통신 인터페이스
     L3G4200D 자이로 센서와 아두이노 보드사이의 연결을 표로 정리하였다．


           L3G4200D 자이로 센서 모듈                       아두이노 보드
                     GND                                GND
                     vcc                                3.3V
                     SCL                                 A5
                     SDA                                A4



프로그램 작성

 자이로 센서의 데이터 출력이 디지털（I2C) 통신으로 출력되어 코드가 조금 복잡하다．
아래 코드에서 실제로 I2C 통신 부분을 구현한 함수는 \V血eRe덥ster 와 readRe덥ster 함수
이다. I2C 통신에서 마스터는 아두이노 보드가 되는 것이고 L3G4200D는 슬레이브 디바이
스에 해당된다．
 슬레이브 디바이스인 L3G4200[刈 주소는 L3G4200D_Ad毗ss = 105이다. ＼자riteRe덥ster
와 readRe멉ster 함수에서 L3G4200D를 호출하면 자이로 센서에서 값을 읽거나 쓸 수 있게
된다．

 #include <Wire.h>

 #define CTRL REG1 0x20
 #define CTRL REG2 0x21
 #define CTRL REG3 0x22
 #define CTRL REG4 0x23
 #define CTRL REG5 0x24

 mllt L3G4200D_Address = 105; //I2C address of the L3G4200D

 m1lt x;
 m1lt y;
 m1lt z;

 void. setupO
 {
     Wire.beg1n0 ;
     Serial.begin(9600);



                                        93 120 통신으로 자0로 센서 人옹하기 -L3G42cw 1 177
 .   Arduino .




              Serial.println("starting up L3G4200D");
              setupL3G4200D(2000); II Configure L3G4200              - 250, 500 or 2000 deg/sec


                  delay(1500) ; I/ wait for the sensor to be ready
      }
      void loopO
      {
                  getGyroValuesO; II This will update x, y, and z with new values

                  Serial.printC'x=");
                  Serial.print(x, DEC);
                  Serial.print("Wt ');
                  Serial.printCy=");
                  Serial.print(y, DEC);
                  Serial.print(冊t");
                  Serial.print("z= ');
                  Serial.print(z, DEC);
                  Serial.printCWt");
                  Serial.printlnO;

                  delay(100); I/ Just here to slow down the serial to make it more readable
          }
          void getGyroValuesO
          {
                  byte X匹SB = readRegister(L3G4200D_Address, 0x29);
                  byte xLSB = readRegister(L3G4200D_Address, 0x28);

                  II 8bit 데이터 출력 2개를 l6bit x 변수에 저장하기 위해서 쉬프트（<< 8) 연산자와
                  II or( I ) 연산자를 이용하였다．
                  x = ((xMSB << 8) I xLSB);

                  byte yMSB = readRegister(L3G4200D_Address, 0x2B);
                  byte yLSB = readRegister(L3G4200D_Address, 0x2A);
                  y = ((yMSB << 8) 1 yLSB);

                   byte zMSB = readRegister(L3G4200D_Address, 0x2D);
                   byte zLSB = readRegister(L3G4200D Address, 0x2C);
                   z = ((zMSB << 8) I zLSB);
              }

178 I 제9장 디지털 통신 인터페이스
    mllt setupL3G4200D(int scale)
    {
        II Enable x, y, z and turn off power down:
        // 숫자 앞어］ "Ob" 가 들어가면 이것은 2진수를 의미 한다．
        writeRegister(L3G4200D_Address, CTRL_REG1, 0b00001111);

        //If you'd like to adjust/use the HPF,
        /1 you can edit the line below to configure CTRL_REG2:
        writeRegister(L3G4200D_Ad如ess, CTRL_REG2, ob00000000);

        II Configure CTRL_REG3 to generate data ready interrupt on INT2
        I'! No interrupts used on T寸T1, if you'd like to configure INT1
        II or INT2 otherwise, consult the datasheet:
        writeRegister(L3G4200D_Address, CTRL_REG3, 0b00001000);

        I,! CTRL_REG4 controls the full-scale range, among other things:
        if(scale == 250){
           writeRegister(L3G4200D_Address, CTRL-.REG4, Ob00000000);
        lelse if(scale == 500){
           writeRegister(L3G4200D_Address, CTRL_REG4, 0b00010000);
        }else{
           writeRegister(L3G4200D_Address, CTRL小REG4, 0b00110000);
        }
        1/ CTRL_REG5 controls high-pass filtering of outputs, use it
        I/ if you'd like:
        writeRegister(L3G4200D.' Address, CTRL_REG5, ob00000000);
}
void writeRegister(int deviceAddress, byte address, byte val)
{
            Wire.beginTransmission(deviceAddress) ; II start transmission to device
            Wire. write(address);      II send register address
            Wire. write(val);       II send value to write
            Wire. endTransmissionO;      I,! end transmission
}
mllt readRegister(int deviceAddress, byte address)

            mllt v'
            Wire.beginTransmission(deviceAddress) ;


                                                      9.3 I2C 통신으로 자0로 센서 人용하기H匕兀42X力 1 179
 .   Ard네no .



          Wire.write(address); II register to read
          Wire.endTransmissionO;

          Wire.requestFrom(deviceAddress, 1); II read a byte

          while(!Wire.availableO) {
                II waiting



          v = WireS read0;
          return v;
      }


     李初du加 (Wi노e．方I)

            I2C 시리얼 통신을 하기 위해서 인클루드 한다．


     卓比fine a꾜［ 冗夙刃 伽2口
     壯兀侮 e a꾜［ 兄EG2 0x21
     戒兀匠ne a丑L丑万G多 0x22
     戎兀万tie （그꾜L兄EG手 0x2多
     戒兀万tie （그꾜1; 모EG多 0x2字

            匕3G4200D 자이로 센서의 레지스터 번호를 정의


     mr L3G'I20끄)eAddress = 끄乃；／夕22Cad介ess of 功e L3G匡200D
                L3G4200[) 자이로 센서의 120 슬레이브 주소이다. 슬레이브 주소는 120 통신 인터페이스를
                가지고 있는 디바이스 별로 모두 다르711 정의되어 있다．




                자이로 센서의 출력 결과를 저장할 변수를 정의 乂 y. z의 출력값은 각각 rc川, pitch, yaw의
                출력 데이터이다．


     斗l比. 屍召加彷
                120 통신을 사용하기 위해서 초기화 하는 함수를 호출한다．




1801 제9장 디지털 통신 인터페이스
Sei始柏（g加臼60까r
        아두이노 시리얼 모니터로 자이로 센서의 데이터를 출력하기 위해서 초기화

seti功L3G4'200D(2伉柳 // cbn伽끄re L3G亡伉1 - 25O, 多O口 ()f 2口口口 a曾冶ec
        자이로 센서를 초기화하는 함수 호출

de／刃／I兄7r功' //wa止 /or 功e sensor to be rea方
        자이로 센서가 동작 가능한 상태가 되는 시간을 기다린다．

Serial．尸I力2r伽； DEC);
        Sen톄.口rint() 함수의 2번째 인자에 DEC라는 인자를 넘기는 첫 번째 인자 x의 데이터를
        10진수로 출력을 하라는 의미이다．

Ser血加rint尸'It吩
        "VW'는 특수 문자 출력으로 TAB을 출력하도록 한다．


  나머지 함수들에 대한 설명은 스케치코드에 있는 주석을 참조하기 바란다. 위의 스케치
코드를 완벽하게 이해하기 이해서는 L3G42001) 자이로 센서의 데이터시트를 완벽하게
이해하고 있어야 한다. L3G42（刃I) 자이로 센서의 데이터시트에 대한 완벽한 설명에 대한
것은 이 책이 원래 의도하는 사항은 아니며 책의 범위를 넘어서는 내용이 될 것 같아
사용법에 대한 설명한 하였다. L3G4200D 자이로 센서에 대한 모든 내용을 완벽하게 알고
자 하는 독자는 ht巾:1/cafe.naver.conilavrstud幻 흑은 http://＼자ww.仁elec.co.kr에 접속하
여 데이터시트를 다운받아 분석해 보기 바란다．


실행결과

  브레드보드에 연결된 자이로센서를 좌우 or 앞뒤 둥으로 움직여 보자. x축을 위로 하여
좌우로 기울여 보면 x축의 데이터 값이 변화하는 것을 알 수 있다. 아두이노 시리얼 모니터
를 통해 아래 그림과 같이 자이로 센서에서 값이 x, Y, z축의 각칵의 각속도 값이 출력되는
것을 확인할 수 있다．




                                        &3 I2(二통신으로 자D로 센d 人용하기-日342OO 1 181
 .   Arduino .



                                                                             ／口回戶妥m
                 的COM18

                 1                                                               [   Send
                                                                                                     ]1
                 N＝                                                                                  II
                 1X=큰
                                      1T      25
                                            z=21
                                            z=
                                    y=15
                                    si=
                         -2


                 Ix=-6              y=14    z=23                                                     1

                                    y너3       14                                                     1i
                                            z=24
                                            z=
                                    y=19
                 H너
                 Ix=0
                 Ix=-4              y=18    z=23                                                     I
                 I     r<=-B        y=14      20
                                             z=
                                                                                                     1
                 lx=-4              y=16     =25                                                     I
                               1      y미6         25                                                 ]
                 Ix＝니 y너3
                  卜：
                          -                  z=
                                                  円                                             r]
                 1 r] Aut。 ll                                                                         I
                                             z＝
                                     scr。              Carriage return   .   9600 baud      !




                                   ［그림 아7] 시리얼 모니터에 2O 자이로 데이터 출력




                       SF기 통신 규약


      SPI 통신은 마스터（Master）와 슬레이브（Slave）로 구성된 구조이다. SPI 통신도 I2C 통신
     과 마찬가지로 한 개의 마스터에 여러 개의 슬레이브 장치를 연결하여 통신을 할 수 있다．
      I2C 통신에서는 여러 장치 디바이스의 구분을 슬레이브에 미리 할당된 어드레스를 이용
     해서 구분을 할 수 있고 SPI 통신에서는 SS(Slave Select)라는 핀을 이용해서 구분이 가능하
     다. SPI 통신은 아래의 3개 채널로 통신하고 SS(Slave Select) 라인으로 다수의 슬레이브
     장치를 구분한다．


       - MISO-Master i叩ut, Slave output
       - 入lOST-Master ot却此 Slave input
       - SCK-Serial Clock


      入'ITSO 라인은 슬레이브에서 마스터로 데이터를 보내는 라인이다. M（丕I 라인은 마스티에
     서 슬레이브로로 데이터를 보내기 위한 라인이고, SCK은 테이터 전송에 필요한 Clock
     펄스를 전송하는 라인이다. 그리고 SS(Slave select) 라인이 있어 데이터를 전송하고자
     하는 디바이스를 선택할 수 있게 한다．




182 I 제9장 디지털 통신 인터페이스
    Ard네no                                                            마ocessor
    SPI Master                                                        SN 듸ave

               MOSI                                                  MOSI
               MISO                                                  M巧O
                SCK                                                卜 SCK

                  55                                                  ss

                      SD Memory                      Sensor...
                     SPI 引ayes

                                    ［그림 아8]    S디 통신 구조




               S디 통신으로 자이로 센서 사용하71 中 L3G4200D


 아두이노에서는 SPI를 쉽게 사용할 수 있도록 아래 표와 같은 라이브러리 함수를 제공한다．


          Function                                    Desc먀光on
begin()                          SPI 버스 설정을 초기화
endO                             SPI 기능을 Disable
setBitOrder(order)           SPI 버스에 데이터가 In 또는 Out 되는 순서를 설정
setClockDivider(amt)         SPI 버스의 Clock 분주 값을 설정
byte transfer(val)               SPI 버스에 한 바이트 데이터를 전송
setDataMode(mode)            Clock의 모드를 설청



 SPI 통신도 앞 절에서 사용한 L3G4200D 모듈을 사용하여 아두이노 보드와 SPI로 통신
하는 것을 실험하도록 한다．


하드웨어 연결

 SPI 통신을 위하여 L3G4200D 자이로센서 모듈과 아두이노 보드를 아래와 같이 연결
한다. 여기서 주의해야할 사항은 I2C 연결 배선의 경우와 마찬가지로 자이로 센서 모듈의
vCC에는 반드시 3.3V를 연결해야 한다．



                                                   9.5 S긔 통신으로 자0로 센서 사용하기 L3G42 U 1 183
  1   Arduino 1




                                                                     卜
                                                                     n
                                                                 L
                                                                 r        4




                                                                       m   t e




                                                                     e E h 5 q 亡




                           ［그림 아9] 자이로 센서 sF가 방식 배선도




                  RESET        Arduino              TXIDO

                  RESET2         Uno               RXID1

                  AREF          (Rev3)                02

                  IOIEF                           PW1 03
                            Ardu녑珀 UN（그 MD
                                                      04

                                                  PWNA 05
                                                                                   口3420001
                                                  四나.106

                                                      13 7
                                                      D日

                                                  .WM DO

                                               ss片）VM D10

                                             MO읾幷＞叩N Dli     -




                                                MI태DID坦

                                                  SCKIDID




                                      ONO




                           ［그림 +10] 자이로 센서 S디 방식 회로도


184   제9장 디지털 통신 인터페이스
 배선 연결이 복잡할 수 있어서 표로 다시 정리해 보았다．


             L3G4200D 자이로 센서 모듈                     아두이노 보드
                         GND                           GND
                         vCC                           3.3V
                         SCL                           D13
                         SDA                           Dli
                         SI刃                           D12
                         CS                            DIO
                         IT寸F                           D7
                         DR                             D6


프툐느그램 작성

 아두이노 스케치에 아래와 같은 코드를 작성한다. 자이로 센서는 출력이 디지털로 출력
되어 코드가 조금 복잡하다. 헤더 파일（L3G4200D.h) 파일도 같은 작업 폴더에 생성해
줘야 한다. 아두이노 개발환경에서는 헤더파일을 추가할 때 대소문자를 구분하므로 반드시
L3G4200D.h 파일 이름대로 대소문자를 구분해서 저장을 해야 한다．

 尸‘ L3G4200D.h 永／

 ／斗"永水水出出水才'水水水水水斗'串永永水水串水水永水串


        L3G4200D Registers
 水水斗 永水串水木才 永水永水水水出 水水永水才 水串才
    '
             '
                     '
                                '
                                    '
                                        水／
 #define WHO AM I 0x0F
 #define CTRL REG1 0x20
 #define CTRL REG2 0x21
 #define CTRL REG3 0x22
 #define CTRL REG4 0x23
 #define CTRL REG5 0x24
 #define REFERENCE 0x25
 #define OUT TEMP 0x26
 #define STATUS REG 0x27
 #define OUT X L 0x28
 #define OUT X H 0x29
 #define OUT Y L 小巴A
 #de fine OUT Y H 0x2B
 #defirie OUT Z L 0x2C



                                             9.5 S긔 통신으로 자아로 센서 사용하기H出
                                                                     （꿔a力 1 185
  .   Arduino .



       #define OUT Z H 0x2D
       #define FIFO CTRL REG 0x2E
       #define FIFO SRC BEG 0x2F
       #define INTl CFG 0x30
       #define I寸Tl SRC 0x31
       #define INTl TSH XH 0x32
       #define INTl TSH XL 0x33
       #define INTl TSH YH 0x34
       #define INTl TSH YL 0x35
       #define INTl TSH ZH 0x36
       #define INTl TSH ZL 0x37
       #define I寸rl DURATION 0x38



      I3g4200_s口i.in0 스케치 코드

       #include <SPI.h>
       #include "L3G4200D.h"

       // pin definitions
       const mllt int2pin == 6;
       const mllt intlpin == 7;
       const mllt chipSelect = 10;

       II gyro readings
       m1lt x, y, z;

       void setupO
        {
            Serial,begin(9600) ;

            II Start the SPI library
            SPI. begin0 ;
            SPI. setDataMode(SPI_MODE3);
            SPI. setClockDivider(SPI_CLOCK_DW8) ;

            pinMode(intlpin, INPUT)
            pinMode(int2pin, INPUT);
            pinMode(chipSelect, OUTPUT);
            digitalWrite(chipSelect, HIGH);
            delay(100) ;


1861 제9장 디지털 통신 인터페이스
    setupL3G4200D(2); II Configure L3G4200 with selectabe full scale range
    II 0: 250 dps
    7/ 1: 500 dps
    II 2: 2000 dps
}
void loopO
{
    '7 Don't read gyro values until the gyro says it's ready
    while(!digitalRead(int2pin))

    getGyroVa1uesO; II This will update x, y, and z with new values

    Serial print('x=");
    Serial.print(x, DEC);
    Serial.print("Wt");
    Serial.print("y=");
    Serial.print(y, DEC);
    Serial.print("Wt");
    Serial.print("z=");
    Serial.print(z, DEC);
    Serial.print("Wt");
    Serial.print1n0;

    //delay(100); // may want to stick this in for readability
}
mllt readRegister(byte address)
{
    mat 切Read;

    address I = 0x80;   7/ This tells the L3G4200D we're reading;

    digitalWrite(chipSelect, LOW);
    SPI. transfer(address);
    toRead = SF1. transfer(0x00);
    digitalWrite(chipSelect, HIGH);

    return toRead;
}

                                             9.5 S긔 툉닌으로 자이로 센서 사용하기- L孜弘2m   187
 +   Arduino 今




      void writeRegister(byte address, byte data)
      {
          address &= 0x7F; 1/ T址s to tell the L3G4200D we're

          digitalWrite(chipSelect, LOW);
          SPI. transfer(address);
          SF1. transfer(data);
          digitalWrite(chipSelect, FIIGH);
      }
      m1lt setupL3G4200D(byte fullScale)
      {
          II Let's first check that we're communicating properly
          II The WHO_ 玉_I register should read 0虹）3
          if(readRegister(WHO_AM_I)! =0xD3)
             return -1;

          II Enable x, y, z and turn off power down:
          writeRegister(CTRLREG1, 0b00001111);

          I/ If you'd like to adjust/use the HPF,
          II you can edit the line below to configure CTRL_REG2:
          writeRegister(CTRL_REG2, ob00000000);

          II Configure CTRL_REG3 to generate data ready interrupt on INT2
          II No interrupts used on INTl. if you'd like to configure INTl
          II or INT2 otherwise, consult the datasheet:
          writeRegister(CTRL_REG3, 0b00001000);

          II CTRL_REG4 controls the full-scale range, among other things:
          fullScale &= 0x03;
          writeRegister(CTRL_REG4, fullScale<<4);

          II CTRL-eREG5 controls high-pass filtering of outputs, use it
          // if you'd like:
          wr此訊明始ter(CTF江 REG5. ob00000000);
      }
      void getGyroValuesO
      {
          x = (readRegister(0x29)&0xFF) <<8;


1881 제9장 디지털 통신 인터페이스
         = (readRe뿌毗er（倣昭）&0xF}吐


      y = (readRegister(0x2B)&0xFF) <<8;
      y I = (readRegister(0x2A)&0xFF);


      z = (readRegister(0x2D)&0xFF) <<8;
      z I = (readRegister(0x2C)&0xFF);
  }


功nd口de (SPL．方)

         아두이노에서 si:기 통신을 사용하기 위해서 추가해야 한다．


豹nc/u比 伍3G'I200D．力／/

         L3G4200D 센서의 레지스터 번호를 별도의 헤더 파일로 분리하였다．


口)nSt 加t jilt孕亡1 = 回

         자이로 센서의 DR 핀과 연결할 아두이노 보드의 포트 번호


cons( mt 加(1／坑1 = 7;

         자이로 센서의 什寸1 핀과 연결할 아두이노 보드의 포트 번호


cons' jilt C方字混／比t = 1方

         자이로 센서의 슬레이브 선택 핀과 연결할 아두이노 보드의 포트 번호


立it X夕 J; 石’

         자이로 센서의 데이터를 저장할 변수들


SPI.LX召亡76;r

          SI긔 통신을 시작하도록 한다．


SF1. se吐治tall而ci日旬町고1O1그匹弦

         아두이노이 si기 클럭 모드를 설정한다．


SF1. setC.1比ki万1辰／er(5玎HCLOCK_1万V8七

         S디 슬레이브 디바이스에 맞추어서 적당히 속도를 조절하1 주어야 한다．


                                           9.5 S긔 통신으로 자0르 센Lk 사용하기- 342oco 1 189
 .   Ard내no   e




     sew／江3G4'2001가2上 // Con伽ure 工36吃伉7wJt方 se／比tabe uizll scaJe rat땀C
              자이로 센서를 초기화한다．

     w方끄e位岫亢a끄?ead在加孕in刀
              자이로 센서에서 데이터를 읽어올 준비가 되었을 경우어빤 데이터를 읽어오기 위해서 대기
              한다．


     실행결과

      코드를 컴파일해서 다운로드 하면 아두이노의 시리얼 모니터를 통해 아래 그림과 같이
     자이로 센서에서 값이 x, Y, z축의 각각의 각속도 값이 출력되는 것을 확인할 수 있다．
     출력 결과는 당연히 I2C 통신을 이용해서 출력하는 값과 같을 것이다．

                  "的COM1B                                         i          蜘콰缸냠3可
                  匕                                                              L垂쁘그1
                  阡2                  y=14三25                                        d
                  1x=-2               y=16   z=21                                            I
                  Ia=-6               y=14   z=23                                            I
                      1/    =1
                                      y=13   z=14                                            1
                  Ix=0                y=19   2=24                                            I
                  I <=-4              y=16   2=23                                            I
                  I x=-5              y=14   z=20                                            1

                      Ix＝니
                      卜＝         -4   y=16
                                      y＝怜
                                             z=25
                                             z=25
                                                                                             1I
                         _i



                  1 코Autoscroll                                                              1
                      Ix=
                                                         Carriage return !   9600 baud   !

                  L                                 --                                           4



                                 ［그림 아］1] 시리얼 모니터에 S디 자이로 데이터 출력




        9.6       자이로 센서로 서보모터 제어하기


       SPI 통신을 이용해서 자이로 센서의 데이터를 추출하고 자이로 센서의 x축 데이터를
     이용하여 축의 움직임에 따라서 서보 모터를 움직이는 실험을 해보도록 하겠다．


     하드웨어 연결

       하드웨어 연결 방법은 이천 절에서 했던 SPI 방식 자이로 센서 인티페이스와 서보모터
     제어 부분을 참조해서 연결을 한다．


1的 1 제9장 디지털 통신 인터페이스
                                             =H只口
                                  싸 L 八三듭프


                                    口

                                  V
                                  n
                                  b 4   \   m m

                                  n t e t h 5   t

                                              크
                                              4




［그림 아12] 자이로 센서 & 서보모터 si가 방식 배선도




        1
       5V


   사duino                TXf 00
    Uno                  RXI［거
   (Rev3)                   02

                       EWU 03
？口duflO 1升卞D Fta
                           04

                       F舟M 05
                                   L絮342001 r
                       PWE4 04                                      LI
                                                            尸
                            07

                           ［沼                                   e

                       F긔蜘t04

                    SS/PWM 040

                   MO띄／PWM 01
                      싸S臼｛기2

                       SCK/［키 3




            已；NO


             i
［그림 아］3] 자이로 센서 & 서보모터 S디 방식 회로도


                                                    9.6 자이로 센서로 서보모터 제어하기 I 191
  1   A川내no e




       이전에 SPI 방식의 자이로센서 배선도에서 아두이노 보드의 D8 포트에 서보모터만 추가
      되었다．


      끄쿠口램 작성

       SPI 방식의 자이로 센서 스케치 코드에 서보 모터 부분을 병합하고 자이로 센서의 x축
      출력에 대해서 약간의 계산을 추가하였다．

       #include <Servo.h>
       #include <SPI.h>
       #include "13g4200d.h'

       II pin definitions
       const m1lt int2pin = 6;
       const mllt intipin = 7;
       const m1lt chipSelect = 10;

       II gyro readings
       m1lt x, y, z;

       mllt motor control = 8;
       Servo servo;

       mllt potpin = 0; II analog pin used to connect the potentiometer
       m1lt va1;   II variable to read the value from the analog pin

       void setupO
       {
           servo. attach(motor_control) ;

           Serial.begin(9600);

           II Start the SPI library:
           SPI.begin0;
           SPI. setDataMode(SPI_MODE3);
           SPI. setClocklDivider(SPI_CLOCK_DIV8);

           pinMode(int坤n, INPUT);
           pinMode(int2pin, INPUT);
           piriMode(chipSelect, OUTPUT);



192 I 제9장 디지털 통신 인터페이스
    digitalWrite(chipSelect, HIGH);
    delay(100);

    setupL3G4200D(2);       II Configure L3G4200 with selectabe full scale range
    1/ 0: 250 dps
    /11: 500 dps
    /1 2: 2000 dps

    servo. write(0);
}

void loopO
{
    m1lt servo_range, old_servo_range;

    II Don't read gyro values until the gyro says it's ready
    whi1e(!digitalRead(int2pmn))

    getGyroValuesO; II This will update x, y, and z with new values

    Serial.prmnt("x=");
    Serial.print(x, DEC);
    Serial.prmnt("Wt");
    Serial.print("y=");
    Serial.print(y, DEC);
    Serial. prmnt("wt");
    Serial.prmnt("z=");
    Serial.print(z, DEC);
    Serial. prmnt("Wt");

    /1 reads the value of the gyro y axis (change if you use other axis)
    val = x,

    /1' scale it to use it with the servo (value between 0 and 180)
    val = map(val, 0, 1023, 0, 179);

    if( val < -20 I I val > 20 )
       servo. write(val) ;

    Serial.print("servo_range=");


                                                       9.6 자이로 센서로 서보모터 제어하기 1 193
 +   Arduir狗 .



          Serial.print("Wt");
          Serial.print(val, DEC);

          Serial.print1n0 ;

          delay(15);
      }
      mllt readRegister(byte address)
      {
          mllt 切Read;

          address I= 0x80; II This tells the L3G4200D we're reading;

          cligitalWrite(chipSelect, LOW);
          SPI. transfer(address);
          toRead = SPI. transfer(0x00);
          digitalWrite(chipSelect, HIGH);

          return toRead;
      }
      void writeRegister(byte address, byte data)
      {
          address &= 0x7F     II T址s to tell the L3G4200D we're writing

          digitalWrite(chipSelect, LOW);
          SPI. transfer(address);
          SPI. transfer(data);
          digitalWrite(chipSelect, HIGH);
      }
      m1lt setupL3G4200D(byte fullScale)
      {
          II Let's first check that we're communicating properly
          II The WHO小AM_I register should read 0虹3
          if(readRegister(WHO_A工I)!=0xD3)
             return -1;

          II Enable x, y, z and turn off power down:
          writeRegister(CTRL_REG1, 0b00001111);


194 I 제9장 디지털 통신 인터페이스
      /1 If you'd like to adjust/use the HPF,
      // you can edit the line below to configure CTRL_REG2:
      writeRegister(CTRL_REG2, 0b00000000);

      /1 Configure CTRL_REG3 to generate data ready interrupt on INT2
      // No interrupts used on INTl. if you'd like to configure INTl
      /1 or INT2 otherwise, consult the datasheet:
      writeRegister(CTRLm-REG3, 0b0000l000);

      /1 CTRL_REG4 controls the full-scale range, among other things:
      fuliScale &= 0x03;
      writefiegister(CTRL_REG4, fullScale<<4)

      // CTRL_REG5 controls high-pass filtering of outputs, use it
      // if you'd like:
      writeRegister(CTRLmREG5, 0b00000000);
  }
  void getGyroValuesO
  {
      x = (readRegister(0x29)&0xFF) <<8;
      x 1 = (readRegister(0x28)&0xFF);

      y = (readRegister(0x2B)&0xFF) <<8;
      y I = (readRegister(0x2A)&0xFF);

      z = (readRegister(0x2D)&0虹고F) <<8;
      z 1 = (readRegister(0x2C)&0xFF);
  }


  새로 추가된 코드만 설명하도록 하겠다．

val = X;:

         계산을 위해서 잠시 \／톄 변수에 저장하였다．


vat = ma／才vat, 0, 102多， O, ／乃功

         자이로 센서의 0' '-'1023 사이의 출력 값을 서보 모터에 출력할 수 있는 小기80 사이의
         값으로 스케일을 변경하는 코드이다．


                                                    9.6 자이로 센서로 서보모터 제어하기 1 195
  .    Arduino S




      if( Va! (- 20 II vat) 20)
        servo. Wf亢e白川；

              너무 미서환 흔들림에 서보 모터가 平r하지 않도록 하기 위해서 20 이상 움직임이 있을
              경우어만 서보 모터를 제어하도록 한다．


      실행켤과

        실행을 해보면 생각보다 잘 동작하지는 않는다. 자이로 센서를 이용해서 서보 모터를
      아주 정밀하게 제어하기 위해서는 자이로 센서의 데이터의 움직임을 예측하는 필티 알고리
      즘 둥이 결합되어야 어느 정도 정밀한 제어가 7陪하다. 여기서는 센서와 모터와 같은
      액추레이터를 어떻게 결합해서 웅용이 가능한지 예시만 했을 뿐이다. 관심이 있는 독자라
      면 A]日RS 센서와 같은 모션제어 모듈들 을 검색해 보기 바란다．




1961 제9장 디지털 통신 인터페이스
  .   Ard네no e如




       10,1          적외선 수신하기


       저비용으로 어떤 장치를 원격 제어하는 방법으로 적외선 사용을 들 수 있다. 이미 우리
      일상에는 TV, 에어컨, DVI) 둥의 가전제품들을 적외선을 이용하여 제어하는 제품들이
      많이 존재하고 있다．
       적외선 통신은 950nm 파장의 적외선을 햇빛이나 전등, 형광등 등에도 적외선이 포함되
      어 있기 때문에 외부의 영향을 줄이기 위해서 캐리어（Carrier) 주파수를 사용하여 정보를
      전달하는 방식이다. 그렇기 때문어］ 적외선을 수신하기 위해서는 이 캐리어 주파수를 필터
      링 하고, 약한 신호를 증폭하는 과정을 거쳐야 한다. 조금 복잡하1 보일 수 있지만，걱정하지
      마라 이런 역할을 해주는 적외선 수신기 부품들이 많이 나와 있다. 참고로 삼성, LG 리모컨
      은 주파수가 38kHz이다. 이번 실험에서도 38kHz 주파수를 수신할 수 있는 적외선 수신
      부 품 을 사용할 것이다．




           JIllIlIllIll    111111



              Modulation                   Demodulation


                              ［그림 ]0-1]   적외선 송수신 방식



       위의 그림에서 入lo血血tion이 적외선 송신부이고 Demodulation이 적외선 수신 파트이
      다. 아래 그림은 적외선 수신 부품의 블록 다이어그램이다. 물론 이 블록 다이어그램의
      내용을 전부 이해할 필요는 없다. 우리가 적외선 수신 부 품 을 만들 것은 아니기 때문어］
      그냥 적외선 수신기에서 이런 일을 하는구나 정도만 알고 사용만 잘 하면 된다．




198 i 제］0장 적외선(IRDA) 통신
                                                                                                                                  抄

                                                                                                                \"CC


                                                                                                      (20kI2)   I
                                                                                                                目J         1
                                                                                                                       -




                                                                                                                     R
                                                                                                                     「
          ai口콕）lthei       AGC            뵤P士      de끄｝odulator                  1
                                                                                                                           I VO
                                                                           -J.




                                                                                     1   c。
                                                                                          il뿌arator

                                                                       \\,                느＞\               rJ             "
           7r           1 \\      ll      /／八          느1

                          //              /   \        F.              //                 ：三：
           느，
                                  "
                                                                                            7/              Lh
 Pr)
   I   constant voltage          1 伊砒 hold 1                           nile얍at。
                                                                              r



                                                                  J.
                                                                       .



                                                                           GND

                                       ［그림 10-2]   적외선 수신 구조


실험에 필요한 준비물들




                       브래드보드 17뀨                                                 아두이노 I꾜qO R3




                          系
                37.9KHz 적외선 수신기
                 CHOB or KSM603L旺
                                                                  적색 LED / ii( 저항 2개




하드웨어 연결

 브래드 보드를 이용해서 척색 LED, CHOB 부 품 을 아두이노 하드웨어와 아래 그림과
같이 연결한다. 적외선 수신 부품은 37.9kHz 주파수대를 수신할 수 있는 어떤 부 품을
사용해도 상관없다. 적색 I코D는 적외선 수신이 되는 것을 확인하기 위해서 아두이노 보드
의 D12포트어］ 연결하였다. 그리고 실제로 적외선을 수신하기 위해서 적외선 수신 부품은
아두이노 보드의 D2 포트에 연결하였다．




                                                                                           10. ] 적외선 수신하기 1 199
Ard내no 1




                                  e




             1 1 1 1 1
                         1




             1




             ::




                                               ［그림 ]0-3] 적외선 수신 배선도




                                      3V3     5V        V八


                             RESET          Arduino                                          M35/GK0日
                                              Uno
                                                                                距
                             RESET2
                                             (Aev3)
                                                                         ：二
                             A日EF                                                                              1
                                                                                      +＜너                    ＼니

                             IOREF                            ,. ,
                                                                                ＜
                                       Arduino UNO R3         , . , D4
                                                                                口
                                                                                C
                                                                                m
                             AU                               PWM DR

                             Ui

                             A2                                                     LEDI
                                                                                    Red (633nm)
                             A3                               , . . O8

                             A4/SDA                           PWM 。9

                             AS/SCL




                                                             "'，“   쁩，   ’，「，




                                                   OND


                                                   1
                                                                                                  frit乙ing


                                                ［그림 ]0-4] 적외선 수신 회로도




甲   「"" 「 " “「" " "鄂
    "
    '
        '
                                             38kHz 주파수를 수신할 수 있는 적외선 수신 부품 H0B
                                             부품이다. 납작한 면을 기준으로 왼쪽에서부터 전원
                                             (vCC), 그라운드（GND), 출력伯utput）이다. Output 핀을
                                             아두이노 보드의 디지털 JO 12번 핀과 연결해야 한다．
                      VCC GND Output         VCC, GNI) 핀이 거꾸로 되지 않도록 조심해야 한다．



    쿠 그램 작성

아두이노 스케치에 아래와 같은 코드를 작성한다．

    #include <IRremote.h>


    ／水
              IR remote detector sketch
              An JR remote receiver is connected to pin 2.
              The LED on pin 12 toggles each time a button on the remote is pressed.
         水／
#include <IRremote.h>                               I/ adds the library code to the sketch

const mllt irReceiverPin = 2;                       i/ pin the receiver is connected to
const m1lt ledPin ＝二 12;

IRrecv irrecv(irReceiverPin);                        //create an JRrecv object
decode_results decodedSigna1                        //stores results from JR detectorvoid
setupO

void setupO
{
              /1 Open serial communications and wait for port to open:
               Serial.begin(9600) ;
               while (!Serial)
               {
                   ; Ii wait for serial port to connect. Needed for Leonardo only
              }
          pinMode(ledPin, OUTPUT)
          irrecv. enablelRlnO;                      Ii Start the receiver object
}


                                                                          10.] 적외선 수신하기 1 m1
  + Arduino .




      boolean lightState = false;    I/ keep track of whether the LED is on
      unsigned long last = millisO; i/ remember when we last received an JR
      message

      ／水
      II decode type
      #define NEC 1 --> Samsung remocorn
      #define SONY 2
      #define RC5 3
      #define RC6 4
      #define DISH 5
      #define SHARP 6
      #define PANASONIC 7
      #define JVC 8
      #define SANYO 9
      #define MITSUBISHI 10
      #define UNKNOWN -1
       永／
      void loopO
       {
               //this is true if a message has been received
               if (irrecv.decode(&decodedSignal) == true)
               {
                   if 佃皿始0 놔 last ) 250)
                   {
                       i/ has it been 1/4 sec since last message?
                       lightState = !lightState;               //Yes: toggle the LED
                       digitalWrite(ledPin, lightState);
                       Serial.print("value=");
                       Serial.println(decodedSignal. value, HEX);
                       Serial.printCdecode_type=");
                       Serial.println(decodedSignal. decode_type);
                   }
                   last = millisO;
                   irrecv.res工rne0;                           II watch out for another message
               }
           }


202 I 제］0장 적외선(IRDA) 통신
     척외선 수신을 위해서 IRr印均把라는 라이브러리를 사용하였다. 이 라이브러리는
血뽀夕／g파1的. com/shirr迂f/Ard岫io-IRremote에서 라이브러리 코드와 사용 예제들을 다운
받을 수 있다. Git 클라이언트를 이용하거나 아래 오른쪽 하단의 ' I兀＼지fll(氾d ZIP"를 이용해
서 압축 파일로 바로 다운로드 받을 수 있다．


后甘磁
1[(5;hi『附／
               出烏爲十「＝nm1
         如dumb如帥曲 J뇨니好鈿arch Here
                                                                                                                              t 「多 P i 0iti-ft,Inc的ex소칡
                                                                                                                              『'                                  目小多］
卄百，目 ,                           m , 큭이지(I'), 만전（5), 도구（0).Q，姻珝 (}                                                                                                   !i
4                                    -                                                                                            11                       1Wmkm小   기1
Ii1] ！杓帥叫
     :y四                " '叫始싻 ' 찌 " m批m혀"蛔耐
                          "呻 " 此出的     “m姻'“"毗
                                                                 "       "" "

                                                                                                                   L
                                                                                                                   " 『 '斗묘’   回    “"
                                                                                                                                                  凸

                                                                                                                                        ' 由" " " ' 阡       +Pu'翡                       11n
11    -    日oarrr머es                             Rdbed panasormmr arrml JVC p뵤0a어                                                         2 years age      ;     -                     I1
H     ,,                                                                                                                                                   ahG'aPhS                  ill
目     圄 !Rremote cpp                             m出a changes                                                                               a year ago      .                         1 乳


1- 브IRremote
                                                                                                                                                           VNetw（긔IC                   丑{

        In miCra
             chan畔                                                                                                                         ayearago                                  m
目     尸m




n 빠『" "" "' "
11                                               咐汕四"呻""'"札plname'며" 0y84                                                                       " 빤，쓰．
                                                                                                                                        5rnon8tsag   ：느，m 窟 네
           UULNSL tat                            Initial sonrrelt from Irre也 "amp                                                         4 ye毗 ago
                                                                                                                                                         ,m.
                                                                                                                                                            ..:，쁘，
                                                                                                                                                                 ,.n陌，                 n
11 目reaialte
   브 "eewordstot                                 miCra
                                                     cha"畔
                                                 Update readme tom- rx
                                                                                                                                          "a "year"" "ago"" 「'”二4 '"Clone
                                                                                                                                                                    " 回 mmtoesktOp     n
1t

1丑    m    .   .                                                                                               ;                                             11今 1知끼, Io.d게p



區＝二1＝『「＝ 二鈿！                                                                                              L}                                            小小小，dJ
                                                      ［그림 ]0-5] 적외선 라이브러리 다운로드 화면


     IRremote 라이브러리를 아두이노 개발환경에서 바로 사용하기 위해서 다운로드 받은
z巾 파
해제한                午．
                   d二立표丸茁뇨뇨延匹亡n二苔亡？y巴
                                 F)

                                 1!
                                      편집（E)      보기（V)

                                         라q브러己C告 포함 !
                                                           도구(1)         도뮴말（H)

                        ’쓰
                                                                          곰유 C卄쌈 !                碎 폴덕                                                   弓三三 中       亡g   鞋
                                                                                                      /


                                 주겨착71
                                                                     J
                                                                                미云
                                                                                     =
                                                                                                                       수졈한 날쿠r                   유헝                       三긔

                             也 다운로드                                             和 exam히es                              2013-12-18 오包             파일 즐더
                             = 바땅 호十1旨                                          드：크 IRcemoie;cpp                       2013-07-23 2草             c-., Source                   -
                             出 최근 위L                                            브 IRremote H                           2013-07-23 Q후..           C/C++ Header
                                                                                川IRremoteInt h                         2013-07-23 오皐.            C/Coo Header                  1
                             寸 랴이브러리                                            11kesvordstxt                          2013-07-23 모후              雙스트 분서
                                 싫 Subversion                                            나CENSE tot                    2013-07-23 오車             乏；트 룬서
                             코 문서                                                        ceadme                        2013心工23 오享               듕횰 三로그랄
                             日 미니Y
                             !4 {“진                                  !     { 鈿呻蜘蜘i蜘畔曲嬅嬅群啣 呻1小心曲唾三：
                                         7; 4 향목
                             i
                                                          ［그림 10-6]                               적외선 라이브러리 설치 화면


                                                                                                                                                        10.1 적외선 수신古
    A川네no .



   예제를 분석해 보면


   consr 立It 立Rece加en뇨1 = 才

           CHOB 적외선 수신 부품의 Ot퍄)Ut 핀에 연결된 아두0注 하드웨어의 핀 번호이다．


   (:（坦1St 血t 七dPin = 12,

           적외선 수신이 되었는지를 알려주는 적색 LED가 연결된 아두이노 하드웨어의 핀 번호，


   끄乙ecv 立recv(irRece／叱rPm上

           1다日Tote 라이브러리를 사용하기 위해서 적외선 수신 부품의 O山지t 핀이 연결된 핀 번호로
           라이브러리를 초기화 한다. 라이브러리 내부적으로 irPeceiverF万n 핀을 Input 모드로 설정하
           여 사용하게 된다．


   立recv. d比a兆6炙d比仇七d會nat)

           "&" 연산자에 의해서 由cx捻J旼y니 변수에 수신된 적외선 데이터가 담겨지게 된다 ，0언어
           에서는 함수의 인자에 "&" 연산자를 사용하여 함수에 인자를 전달하면 함수내부뻬人1 변경시
           킨 dec（刈edSign톄의 값이 함수 실행이 끝나 이후어匠 유지가 된다．


   立recv 1仍time彷

           적외선 수신이 완료된 이후에 다른 수신을 위해서 대기하도록 한다．


     ml血s(）는 아두이노에서 시간의 경과를 msec(1/1000 초） 단위로 알려주는 함수이다．



   실행켤과

      삼성 TV 리모컨을 이용해서 0-9까지의 버튼을 누르면 아두이노 시리얼모니터 윈도에
   아래 그림과 같이 버튼의 16진수（He幻값과 리모컨의 Type이 표시가 된다．




2041 제］0장 적외선(IRDA) 통신
                                                                                                                     醫

                 '的coM:3                                    찌      m          伊 ' 口！回 娥놔
                                                                                              Send

                             va 山e=200F4667
                             decode_type=I
                             va 山e=200FC837
                             decode_type=1
                             Va山e=200F2807                                                                     1量
                                   type=1                                                                ！重
                                                                                                           ii.
                  重decode_
                             v키ue=200FA85?
                             decode_ type=I                                                               JI
                             Va山e=200F6897                                                               :11
                                    type키
                             vaIue=200FEBI7
                 휼decode_
                                                                                                         }r
                   decode_type=l                                                                     n -
                 iva山e=200FlBE?                                                                     「 !
            1decode_type=l
             ! va山e=200F986?
            idec。 de_type=1
            tva山e=B1890683
              de印de_ ty口e＝니
            i Va山e=8E化1미4
            I decod巳tyi氾＝너

          1                                                                                          ,


          !Ri Autoscroll                                       Carriage return r       9600 baud
          卜mmm
                                                                                                               J




                                      ［그림 10-7]       적외선 리모건 수신 테스트 화면


 필자는 LG 리모컨이 없어서 테스트를 해보지는 못했지만 아마도 삼성 리모컨과 같은
Hex값을 표시할 것이다．


 M
                                                                                                                         \



  삼성 리모컨의 0,-'_,9의 각 버튼별 Hex 값

     버튼                            Hex        버튼            Hex               버튼                               Hex
     0                       缸20DF48B7            1      0x20DFC837                2               0x20DF28D7
     3                       0x20DFA857           4      0x20DF6897                5               0x20DFE817
     6                       0x20DF18E7           7      0x20DF9867                8               0x8789C683
     9                       0x8E1C1C14

                                                                                                                     I




                                                                                              10. ] 적외선 수신하기 1 205
  1   Arduino .




       10.2       적외선 송신하기


       이번에는 아두이노를 이용해서 적외선 송신 기능 실습을 해보자. 적외선 수신부는 이전
      절에서의 수신부를 그대로 이용하고, 적외선 송신 부분만 작업을 해서 송신부에서 보내는
      적외선 값을 이천 Chapter에서 했던 예제를 통해서 Type과 Hex 값을 아두이노 터미널에
      표시를 해보자．


      실험에 필요한 준비물들


                              社S
                              汪     ;（攷三）휼而；:1
                                                        I
                                  1스 小나 H小.             m
             브래드보드 17뀨                           S8050 NPN 트랜지＝!＝터 17}1




                  朴 升
                              아두이노 UNOR3




        100, 470 Ohm 저항 17뀨   CL-1L5 IR I上Dl깨1




      하드웨어 연결

       브래드 보드를 이용해서 NPN 트랜지스디, a-1L5 JR I且）, 저항 부 품 을 아두이노 하드웨
      어와 다음 그림과 같이 연결한다．




2061 제］0장 적외선(IRDA) 통신
                                                                             分

               볍




               ［그림 ］아8]               적외선 송신 배선도


                   사dumnb UN0 83




         3V3    EV       VIN


RESET          사d내no                Tx/Do
                                                LOOT
                                                Infrared (940am)

RESET2           Uno                RX/Dl

AREF            (Rev3)                D2

山日OF                               P밖M 03

                                      04

AO                                 P바M 05

Al                                 PWM 06

A2                                    07

A3                                     08   나



A4/SDA                             P밖M 09

A5!SCL                         SS/PWM 010

                           MO듸／PWM 011

                                M田O/O作

                                   SCK/O出



N/C




                     GND


                     1
               ［그림 ］아9]               적외선 송신 회로도




                                                                   102 적외선 송신하기 I 207
  亡 Arduino .---




                                          37.9kHz 주파수를 송신할 수 있는 적외선 송신 부품
                                          CL-1L5이다. I上D와 마찬가지로 1코D 연결시 I코D몰딩



                      Ii
                                          안의 쇠판이 작은 쪽 Anode（애노드）를 전원（vcc）에 연
                                          결해야 하고 큰 쪽 (h由ode（캐소드）를 그라운드（GNI가
                     GND VCC              어］ 연결을 해야 한다．


      위의 회로 그림에서 P凹M(Pulse Width 入l：넜ulation) D3에서 나오는 八'lodulation 신호로
   Q1(NPN 트랜지스터）의 베이스 부분을 제어하여 적외선 송신을 하고 있다. 트랜지스터가
   하는 기눙은 일반적으로 스위치 기눙과 증폭 기능이 있는데 여기서는 PWM D3 핀에서
   나오는 II之 제어 신호를 증폭하기 위해서 사용이 되었다．
      P硼M기능이 있는 핀은 CPU어］ 있는 Timer를 이용해서 원하는 주파수를 만들어 낼 수
    있고 Mo（加lation 기능으로 펄스의 폭을 조정해서 전류를 제어할 수 있는 기능이 있다．


   프로그램 작성

      아두이노 스케치에 아래와 같은 코드를 작성한다．

      #include <IRremote.h>

      IRsend irsend;

      void setupO
       {
           SerialSbegin(9600);
      }
       void loopO
       {
             irsend. sendNEC( 0xc5000000, 8);
             delay(1000);
             irsend. sendNEC( 0x45000000, 8);
             delay(1000) ;
             irsend. sendNEC( 0x25000000, 8);
             delay(1000);
             irsend. sendNEC( 0x85000000, 8);
             delay(1000);




2081 제10장 적외선(IRDA) 통신
예제를 분석해 보면


끄?seii/ 止send,

       적외선 송신 라이브러리를 이용하기 위해서 초기화한다．


立5cr汪／
     ,sen（刃V石C(o火C多口口口口口口， 8);

       NEC 포맷으로 적외선을 송신해 주는 라이브러리 함수이다. 첫 번짜1 파라미터 0xc50000(刃
       7 송신할 데이터이고 2번짜1 파라미터 "8"이 데이터 사이즈가 된다. 라이브러리에는 N日二이
       외어匠 Sony, Panason匕, JVC 등의 포맷을 지원한다．


실행결과

  예제를 실행해 보면 1초 간격으로 4개의 수신된 16진수（I-妃功값과 리모컨의 Type이
표시가 된다．




                                                                                                         i
                      '色:oi:1                                       -                       的岬냔 fl
                                                                n




                                  Ideco由jvpe＝너
                                                                                                 r三而可斗
                                   27AF0864
                          !decodemtype=-1
                                   卜키ue=
                          I v。lu日=DB399405
                                 de_type=
                                  1cJec。
                                                           -1


                          I n。山e=36B72A8l
                          I dec口de_type=-I
                          iv。 l ue=811E329F6
                          ldec。  de_ty口e＝니

                                                     2?AFD864

                                                          ;:
                            卜키ue:
                       deco
                       v。l u：                  므謐；
                      !decode_type=-l
                       ye山e=3t召?2Affl
                      idec。 de_type=-l

                             8l 0329F8
                      {decnde_type=-1
                        卜이ue:
                      iv키 ue=2?AF0864
                      沖cod町ype늬
                 奸en lue=1JB399405

                 和.od.穹「p,e=.-l
                                                                                                         ；弔
                                                                                                          J;
                 ,.
                                           J Autoncroll                 Carriage return ,   9600 baud


                                                     ［그림 ]0-10] 송신된 적외선을 수신한 화면


 이 기능을 잘 이용하면 적외선을 이용해서 무선으로 자동차, TV, 카메라 등을 조정하는데
이용해 복 수 있을 것이다．




                                                                                                         10.2 적외선 송신하기 I 209
지그비（Zigbee)
         네트워킹
]] , ]
     지그비仍gbee）란2
112 지그비仍gbee) 통신 테스트
11.3 아두이노 지그비口gbee) 통신
11.4 특정 XBee어빤 통신하기
 .   Ard내no .




                지그비仍的ee）란7


       지그비（Z增bee）는 블루투스（Bluetooth）의 고가격 , 고전력 소비의 단점을 보완한 IEEE
     802. 15.4(PHY, 入1AC）에 기반한 무션 기술로 벌이 Z坦-Zag로 날아다니면서 다른 동료들에
     게 정보를 전달하는 정보전달 체계를 착안하여 붙여진 명칭이다. 무선 리모컨, 조명제어，
     키보드, 마우스, 홈오토메이션, 센서 네트워크 등 다앙한 분야에 응용되고 있다．
      지그비는 산업, 과학, 의학용 무선 주파수（ISM 밴드 : Industrial, Scientific and 八4edica1)
     내에서 작동하며 블루투스와 같은 개인 통신망을 사용한다. 초당 전송 속도를 보면 와이파
     이 등에 비해서 느린 편이다. 전송거리는 2.4G1七 하드웨어의 경우 30m/indoor, over
     lOOm/outdoor 정도이다．


     주파수 대역 및 전송 속도

       - 전세계 : 2.4 GHz ISM Band (250 kbps)
       - 미국 : 915 MI-Iz ISM Band (40 kbps)
       , 유럽 : 868人끄크z(20 kbps)
        일본 : 2.4 GH爪250 kbps)
       - 한국 : 현재 乃gBee-용 주파수 확보를 위한 연구 중


     지그비 어플리케이션 드L파일

      지그비 얼라이언스（지그비 연합）가 지그비 스펙울 제정하는 표준화 단체인데 , 여기서
     스펙 뿐만 아니라 지그비의 애플리케이션 프로파일들을 정의하고 있다．


       - 가정 자동화（Home Automation)
       - 지그비 스마트 에너지（ZigBee Smart Energy)
       - 상업용 빌딩 자동화（Commercial Building Automation)
       - 통신 애플리케이션즈（Telecommunication Applications)
       - 개인, 가정 , 병원（Personal, I如me, and Hospital Care)




212 1 제］장 쟈그I l(Z暾ee) 네트워킹
  11.2 !       지그비位勾bee) 통신 테스트


  지그비 통신을 테스트하기 위해서는 최소한 송신, 수신 각각 1개씩의 지그비와 아두이노
보드가 필요하다. 아두이노 보드로는 Ard血O LJNO R3를 사용하고 지그비는 아두이노에서
쉽게 사용할 수 있도록 모듈 형태로 나와 있는 D塼사의 XBee 모듈을 사용하도록 하겠다．
  이번 Chapter에서의 최종 목표는 2대의 아두이노 보드어］ 각각 지그비 모듈을 연결하여
서로 통신을 하는 것이지만 처음부터 지그비 통신을 아두이노 스케치를 작성해서 테스트
하기보다는 D增사에서 제공하는 테스트 프로그램(cm)을 이용해서 XBee 모듈의 통신
상태를 점검하고 나서 진행하는 것이 좋다. 무선 통신이 잘 되지 않을 경우에 하드웨어적으
로 결선이 잘못되어 있을 수도 있고 스케치를 잘못 작성하여 통신이 되지 않을 수도 있고
XBee 무선 통신 모듈의 불량으로 되지 않을 수도 있다. 이러한 경우어］ 어디에서부터 문제를
해결해 나가야 할지 막막해진다. 그래서 이번 절에서 우선 XBee 모듈의 통신 상태부터
점검을 해 보도록 하자．


실험에 필요한 준비물들



                                                                    L
   U.
         ． 口




 !n#      二；今分孤分-..
                                  口＝4


                       r     /r                                6!       m,

                                                   m
                                                   m           드式如m朴．三
                                                   m
                                                   m           次Be냠
        e1     小 寸小｝
                                                               ! ,,如照三＞:




 力
  Arduino ［丹4O R3 2개       XBee USB Adapter 271)       XBP24-DM 1T-乃oJ 통신 모듈 271)



                                   口口
                                        71mm
                                        m川
  入lini USB 케이블 2개1         XBee C]江J 프로그램



하드웨어 연결

 x-cm 프로그램을 사용하기 위해서는 XBee 모듈을 PC의 시리얼 포트에 연결해야 하는
더］ XBee 모듈을 PC에 USB연결을 통해서 가상 시리얼포트로 변환해 주어 쉽게 PC어］ 연결


                                                         112 지그비仍9比e) 통신 테스트 I 213
  .   Arduino .




      하1 주는 모듈들이 많이 나와 있다. 또한 이러한 모듈들은 XBee어］ 3.3V 천원도 같이 공급할
      수 있어 편리하게 사용할 수 있다. 요즘 대부분의 노트북들은 두께와 무게를 줄이기 위해서
      시리얼 포트가 없이 출시가 되고 있다．


      (] ) XBee 모듈과 XBee USB Adapter 연결




                                               ［그림 ]1-1] XBee 啖；B Ada口ter 연결


      (2) XBee USB Ada아아를 PC에 연결
        PC에서 XBee USB Al姐pter를 제대로 인식시키기 위해서는 Ffl고 USB 드라이버를 PC에
      설치하먀 한다. 아래 URL에서 Ffl끄 USB 드라이버를 다운로드 받을 수 있다．
      http://www.ftdichip.com/Drivers/VCP.htm

                                                                                                                                                          =   回     23

                                  小」r汀ftdlchlp.c에5 Driven三dVCPhtrr,    P 1 8 口x
                                                                                        "S加키C아／         P0作Dr卜．P05            I기
                                    !   斗이지（m 1      만젼（St !    도




                         땜
                                             Future Techrs이ogy Devices                            It卄emotion이 나d.

                                                    USB Device So山tiovs            AS吃 Deogrv         Product Design




              Home                         > Virtual CON Port Dnvers
                  f가od日C뇹
                                          This page Contains the VCP drivers currently available for FT긔 de너ces
              O！柑era
                   VCP 0巾ers              For D2)X［거red drrners please click h旦旦

                   D2XX Dci四'5
                                          Installation grades are available horn the Instaltation Grades page of tIre Documents section of this site ton selected
              디rmware
                                          operating systems
                  Support
                  Andr이d
                  Sales Network            >   VcP Dnvers
                  Web Shop                Virtual CO서 port I比P} driv酊s cause the USB deece to appear as err ad벼tiorral COM port availa벼e to the PC
                  Ne出하etter               Applicatiorr ssft너可e c켜r access the USB desrce 1n the same way as S wou녑 access a standard COM port
                  Corporate
                  Contact Us
                                                                                                                                   " 口小srow.
                                                                                                                                           'td,
                                                                                                                                                  chr口cerniF了Coil
                                                             m曲dad ho Future丁echr이1                  《아'1            irvded
                                                                                                                              jh
                                                                                                            '9如n키l
                                                         ;
                                           ［그림 ]1- 2]                   다DI USB 드라이버 다운로드



214 I 제］］장 쟈그UI(z甘挑）네트워킹
 XBee USB Adapter를 PC와 연결하기 위해서는 미니 USB 케이블이 있어야 하고 미니
USB케이블의 A Type 포트를 먼저 PC의 USB포트에 연결하고 5핀 미니 커넥터를 XBee
USB Adapter의 미니 USB포트에 연결한다．
 USB드라이버가 제대로 설치가 되어 있고 연결이 정상적이라면 아래 그림과 같이 PC의
장치 관리자에 "USB Serial Port(COM7) "와 같이 가상 COM포트가 생긴것을 확인할 수
있다, 여기서 PC에 따라서 "COM7"이라고 올라오지 않고 C（羽2, COM3 등 다른 이름으로
올라올 수도 있다．



         파묀｛F}   튤좌（粉   보기（V)   도음말（H)

         舡 I, ! 力匠于目圃 'tt
                                   ．希 ky匕m_th)nkpad               업
                                       0 밂uetocth 송수신 잠지
                                    L5 냠i0110/CD-ROM 드라이브
                                    口mIDE AWATAPI 컨트룔러
                                     口坐 Jungo
                                     p. SM Drivef
                                    ＞立 네트워크 어댑터
                                    >ra 디스크 드라이브
                                    小兵 디스플래이 어댐日
                                    小心 댜우스 및 기타 포인텅 장지
                                    ＞壤 모니터
                                     目 母 배터리
                                     b무 범용 직렬 버스 컨트릎러
                                     枷寸 사운드‘ 비디오 및 개밈 건트튿러
                                     >4 시스탬 쟝지
                                     >+ 이미징 장지
                                    口4 컴퓨턱
                                    卜 心固 7 보드
                                     d6 " 포트（COM & LPT)
                                     ! 乙亐’ USE 鈿j키 Fl긔t(COMI)
                                     b 「   프로埠Aj
                                    卜礪 휴먼 인터파이스 챰지




        1=


                 ［그림 11-3]         FT미 USB 가상 시근얼 포트 장치관리자 화면




千CTU 프로그램으로 XBee 모듈 통신 설정

 x＜그lJ 프로그램을 이용해서 XBee 통신 테스트를 하는 것은 단순히 XBee 모듈들이
이상이 없는지 점검하는 이유도 있고 XBee 모듈 간 통신이 원활하게 이루지게 하려면
약간의 설정들이 필요하다. x-cnJ 프로그램을 이용하면 이러한 설정 작업들을 쉽게 할
수 있다．




                                                                11.2 지그비口gbee) 통신 테스트 1 215
  .   Arduino 斗



      (1) X-CTU 끄쿠기램 다운로드

       1玉gi 웹사이트에 접속하여 다운로드 받는다．
       http://入／ww.digi.com/support/kbase/kbaseresultdetl ?id=2125



               O馨乞m品兪岫鈿岫印4미如蜘蜘小1k
                 쇼 ! 日 r＝三 的 ! 目미지：P1! 안전（5) !                          도구（0) ' e! 珝 厠 0




                 小如r                    M2M E叩帥

                 旦凹뾰 > 蚤꼬끄묘쯔I > (sos너edne Bonn > Kno州edge 日use Ast,de



                                                                        斗CTU (XCTU) so什ware
                 MaxStream announces the X-CTU soft사are for configuring and testing MaxStream radio modems.
                 Features:

                       1Support for all MaxStream products.
                       1Integrated terminal window.
                       1Easy to use 幻opback range test.
                       1Display of Receive Signal Strength Indictator (RSSI).
                       1Upgrade RF module firmware in the field on all XCite modules and XStream modules version 4.29 and higher.
                       1Display both ASCII and hexadecimal characters in terminal window.
                       mCompose test packets in either ASCII or hexadecimal for transmitting in terminal interface.
                       1Save and retrieve commonly used module configurations (profiles).
                       1Autom誌ca啣 detect modu陀 type.
                       1Restore factory default parameters.




                                                    ［그림 11-4]                      X-CTU 프로그램 다운로드



      (2) X-C11J 끄쿠口램 설치
       다운로드가 완료되었으면 x-ctu_5. 2.8. exe 설치 프로그램을 실행하여 X-CTLJ 프로그램
      을 설치한다. 현재 프로그램 버전은 5.2.8이지만 이 책이 쓰여진 이후에 D增사에서 프로그
      램을 업데이트 한다면 설치 파일의 이름은 달라질 수 있다．



         닙elcome to the 乂CTU Setup 놔izard



                                    由e d디ae,e4Jkrditi5si쇄XCTUuaymacuns姓巴                   F七ade 1出七 a rsunent is read N也 lie帥8e 因eamrt mJ比 lip며aacce甘 lad 比m8 比1D比 C如k 띠
                                                                                           匈d닝‘汁比可Ned‘『 口寸em卄eecickc과t可『



                                                                                                                   greeene frncDrgr 工CTL- s-o小mre

                                                                                             In耳｝（月Sued! Read Ceref出is B艸sst胡beg the 立寸is'可e, 卯U 町e Cm5口it뇨g
                                                                                             to be 뇨rued by used use 1玘Cm丘昭 opoetyte Fl血 end-user licence
                                                                                             a可eein巴止
         wan새N더 T陋 C0畔沚New可n k 미이'a叱 啣 m나m咐 bW a1겨卄甘미,wieed bns出eS
                                                                                             Tf由 巴k工user license agreement（三ULA) in sI叩寸 a平eenle址 betwe口l
         Uno너is긔meUd바外Cahnn 며 d出蜘'a ' 寸 mm 口DaMn. 미 m낑目nised tes카 七sad          시目e C抑1      yme（寸her as 뇨小妃岫 m a 5뇨甘e d出ty) used Di恥nt텨not由nut Inc. for
         머 Cmm出 pen副吼』크nd 叫出 beaus日C1寸.dto 出C nseuaneen eBerN prne*A= 나닙나 d七匕1시                  De巨 乂口1j5硼In可e 岫岫 鈿如des con恥如r 5出W毗：smot沌
                                                                                             i- I끄n卜k丈Agee


                                                                                                                                 Cussed    1




                                                       ［그림 1］中5]                      冷CTU 프로그램 설치］



216 I 제］］장 쟈그비（雨bee) 네트워킹
  崩x.：札 ‘肯                          H                  呻I--..／晦耐1
                                                                              峀 X<TU f,    :‘티
  15eie（寸 In드;tallat山nF이der                                    1；在        1    Confirm Installation
                                                                少
  [
  1The沁如dm」                        ／(！山. 汁，伽枷似뇨                           1    me     人 七a由 m nnd 乂C化 m 艸J Ca껴Mm

              ro.出川11d11lol뇨』出k斗10寸나n벼dma出蜘m回由Len帥뇌m毗呻따呻en                H    C比k m把寸Ioa.e 寸七 m1如n

                                                                          ]
               Em뇨                                                        납
               尸WProg『미n日esWfig附XCTLIW                  B［呻C        1旨
                                                       ）炚毗           1甘
                                                                          曾
                                                                          斟
                                                                          目
  기             oleIIXCTUm叩Jme1아f아려가이七내刃山小th5C口1거）
                                                 1i甘

  허


  놔
                     吐，
                      ．艸，

                      ""   m                                              曾
  L                                         「毗‘ j '「，"" n二至莖二그r甘                                           CCC叫    !   世놘   1


                                                  ［그림 11-6] X-CTU 프로그램 설치2



               nstalting X-CTU
                                                               亡r
              IC-CTU 4 bol目 寸毗d



               FkdSe 叫出

                11             1




                                                                                 今提黑二据0 oheokDi加미兀如f마hrenw可' "여苡小？



    1                                                                1

                                                  ［그림 ]1-7] 冷CTU 프로그램 설치3


 위의 설치 과정 중 완료 시점에서 fhin下刃are update 하라는 메시지가 나오면 firrnware
업데이트를 시작한다. 물론 PC는 인터넷에 연결된 상태에서 진행해야 한다．


(3) 冷CTU 끄쿠口램 실행
 乂CT[J 프로그램을 실행하면 "Select Corn Port" 어］ USB Serial Port(COM7）이 올라온
것을 볼 수 있다. "Test/ （加eiy" 버튼을 눌러서 XB三 모듈의 버천과 통신 상태를 점검한다．




                                                                                                  11.2 쟈그비（刀gbee) 통신 테스트 I 217
  .   Arduino .



                           簪X-CTU                                                           ,：小          「（『7            耐的岫可
                                                             ,                                      .                                       !
                        ! 冗，5e11,rgs.1,A가日' Test Term"키N"巾' C耐如可' ni
                           IAbOUt
                        1 L1긔nr미（그口
                                                                                                                                            1
                                     （니J                                                                                                     1
                        I Se뇨ci C미,rport                                                                                                   I.
                        rUS:          t. S"'                                                      'M2   Baud    ：   『『
                                                                                                                    『    9600
                                                                                                                                       j
                                                                                                        Floor Control NONE

                                                                                                        Data Bhs

                                                                                                                                NONE
                                                                                                        Panty

                                                                                                                                       j
                                                                                                                                       j
                            - , . J町旬呵：::：寸
                                                                                                        St   BBs



                       r1 "쓰'抑lus帥田叩蜘
                                                                                                                           Ii
                                     '" nieri'빠 .뇨 ．
                                                                                                                                             i
                                    [r'
                                                EnabtedPi                 -     -,。ractem
                                                                                                                     i
                        n                  1!                     1 n     .




                                                                                                                                                 長


                        rCommand                     Bef。re (B：
                                          Guard TimeCharacter                               二二
                                                                                                                                             흩
                        1                 , .   J4        :,"L.         ,1 J.          :4



                        1 二꾜；二上；                                                                                                                 長

                        1
                        Ii叫如                         11
                                                 ［그림 11-8] 冷cm 연결 테스트


       XBee 모듈에 이상이 없다면 아래 그림과 같이 모듈의 Serial Nun小er와 Modem type
      이 읽혀진다. 우리가 사용하는 XBee 모뎀은 XBP24-DMW玎-2羽를 사용하고 있기 때문에
      Type은 XBP2＋마d가 읽어진다. "OK"를 눌러서 다음으로 진행한다．


                                    Corn test / Query Moder
                                          Communic計口n 바1(h modem. OK
                                          Modem lirmvaare version = 8062
                                          卜相dem 蜘e =X6P24-DM

                                          Serial Number = 13A2004098E11E




                        ［그림 11-9]                                                                X-CTU 연결 테스트 결과 화면



      (4) XBee 모듈 통신 설정
       "Modem Cot寸iguration"탭에서 "Read"를 하면 현재 XBee 모뎀이 사용하는 "Function
      Set"과 "Version"을 읽어온다．



218 1 제］］장 자그비（乙gt e) 네트워킹
                叱四2) X-CTJ
               口，                                                                         口          놔뇌
                 MO口em       Paramet횬r   Prof卄e    R們1rote Co［州gurat四0.             \／숀i-s心Os.,
               , PC Seingsi Range Test} Terminal Modem ConFiguration
                       끼 口   =m口1凸r =nH 口hm山＝r口       口＝r =n3凸E凸. 5／뇨1A1   口rnFa凸         \／口r시nn小


                唯m 닙'It已                          1 口ear Screen            "Save
                                                                                            Do叫nload nor시
                    枷홴0 Upd和旦깬쁘                         S므쁘坐쓰．
                                                             l＝                    쓰．
                                                                                    m4 小V쁘吟1
                 Modem: ><BEE-PRO Function Sat                                                Version
           긴빠삐1伽EE P日0蛔MESH 2.4                                                          깁匠而＝
                나"二J N以W可Kmq
                        白 [7FFF] 山 - Mode作LV山
                        自 (C) CM - Operating Channel
                        口 [A) R日 Mac Retries
                        白 [3) MT -M네t汀ransmit
                        口 [O) BH · 8山adea弑 Radius
                        口 1기 M尸 小lesh Retries
                        口 (7) NH - N以1시마kHops
                        口 [3) MN - Network Delay Slots
                        口 (0) CE - Coordinator Enable
                  d Addren自08
                        自 [1 3A200) SH - S日n비卜仙mber High
                        口 [409BE11E) SL- Seri톄 Number Lo叫
                   ·04· 1 (0) DH - Destination Address High
                        口 [FF阡］DL - Destinal山rr Add氾＄s Low
                        口 [ (NI 小妃de Identitier
                        口 (82) NT - Node Discovery 8ackolt
                        口 [0) NO 小妃de ［기＄covery 0的ens
                        [a          『」 - Device lype IdentiFier
                      1 ; ＝巾 n1

               下｛cad pararo叭日rs口시
           乳

                                                                                                                i
                m니2       9600 8-tI-i FLO姑rIONE XBP24-DM                                                        1
           \                        1               m                                                ＝드 rm口 已



         ［그台 j j呻］0]               冷CTU와 XBP24-DM과 연결이 완료된 화면



 나머지 1개의 XBee 모듈어］ 대해서도 x-cni 프로그램을 이용해서 위와 같은 과정으로
통신 점검을 한다．


(5) 乂-CTU 끄쿠그램을 이용한 XBee 통신 테스트
 XBee USB Adapter를 이용해서 PC의 USB에 XBee 모듈 2개를 동시에 연결한다. 다음
그림은 XBee USB Adapter 2개가 동시에 PC에 연결되었을 경우 장치 관리자 화면이다．
USB Serial Port포트가 2개가 올라오는 것을 확인할 수 있다．




                                                                                            11.2 지그비（酌bee) 통신 테스트   219
 +       Ard내no S



                                                                                                                                                                                         及
                                                         發 컴퓨E寸 관근.

                                                          파멀（F)   듕좍（A)     보기（V)       도움말（H)

                                                         白I. ! 츠曲目E크 」t二
                                                                                               i蟲 kykim thin印ad
                                                                                                口 C 텨uetooth 송수신 잠치
                                                                                               卜心 OVO/CO-ROM 드라이브
                                                                                               ＞呼 1匪 ATA/ATAPI 컨트룐러
                                                                                               卜望 Jun卯
                                                                                               1> 在 SM Driven
                                                                                               1, 型 LI트워크 어밉티
                                                                                               mt;> 디스크 드라이브
                                                                                                口 好 디스플21이 이댑터
                                                                                               ＞也 마우스 및 기타 포인텀 잠지
                                                                                               卜界 모니터
                                                                                               口斗 배터리
                                                                                               Is무 범용 직렬 버스 건트롤러
                                                                                               ＞뗘 사운드. 비디오 및 71임 건트롤러
                                                                                               ＞心 시스뎀 잠치
                                                                                               ＞毛 이미짐 잠지
                                                                                               卜斗 껌퓨터
                                                                                               m心 키보드
                                                                                               小甲 포트（COM & LPI)
                                                                                                !   뇨管 USB Se曲 加st(COM7)
                                                                                                !   乙孕 USB See]出 的rt(C（거너8)
                                                                                               ＞二 프로세서
                                                                                               卜奴 휴먼 인터斗이스 장치




                                                    ［그림 11-11]                 장치 관리자에 USB 시리얼 어댑터 2개가 연결된 화면


                                   이 상태에서 x-c1兀J 프로그램을 동시에 2개를 실행해서 COM7, COM8 각각의 포트에
     연결한다．

         n口！CO！납IT X-C了LI                           :r                                         m1a1 「m文啣／
         {J "                                       :i                                     "         n m=d i                  二矗磊薰鈿弘                                                            ，多了可出丹쯔和
     在；;.,, '二；忿，쀼ritecIrcle恣窯鴛客1 ' 邯""'
      「，                                                                                                             I            杯的妊珪難枷妃ten                   Profilo   N帥Ote Con)igunat由"      VernonE.

                                                                                                                         甘冗Seftir叫RerrgeTesll Terrnin계 Mod帥1.咐’叩"IcIi I
                                                                                                                                                                                                         .

                                                                                                                         卜＝
     苒：晷亡'1 烹打黑h每아                                                                                                       且 H沙叫’"呻' nd Fsnw沙了뼈．켓曲竺艾 尸'껜e
                                                                                                                         I22뜨느4므므已1 그드쁘드多 亡巴르뜨쁘j
                                                                                                                         I ! Also켁＄U口d카e나mWarL 놔刃oats日taunt)
                                                                                                                                                                                               raen:
                                                                                                                                                                                              LOO口 1
                                                                                                                                                                                                       Version妙
                                                                                                                                                                                                        山，삡，쐈，ne叫
                                                                                                                                                                                                                    i

                         Mndene XBEE-PRO F山ct sSe*                                                  Ver自on
                                                                                                                                                                                                       碼쁠니
                                                                                                                                                                                                         . .
                                                                                                                         I 卜由而油ED-PR口 Ft.,사cc Set
     ,         DM                               j
                            XBEE PRO DIGIMESH 2.4
                         IX8P24-                                                               늬 8062        ;       ,   IJX8P24-DM 크((BEE P日口叩MESH 2.4
     I '日 J Net'川otkrng                                                                                                  臂百표크 N clot口rkr8
       r                     1deco VID                                                                                   L      : 口1:        山如em
                  니1       口叫air凹Oh허甘祀1                                                                                  卜     「 口 口：      H 3口cIatrro引：n크「n뒤
                 1A1日N - Msic 日nines                                                                                               口 ,q1日1千Mac Rerrre.
                 [31 MI - Mssh-Trsnoen甘                                                                                      n     h [ 3] MT - hlrdr-lrsnorod
       t         1미NH - Br口ddCa引日ad口JS                                                                                          r h ]0] BH Bmadea針N혀抑J3
                 1기MR , Meals Ret,思S                                                                                            小 I 미MR - Mesh Retries
     "           (7) NH - Re加roslr Ho口S                                                                                         卜如 1 (7) NH - Nets呪가k Ho口＄
                 (3) NM - Nes叫osk 0nIas Slots                                                                        二          )1 (3) RN - Net叩ek DcIar Ohio
     1L          ]0) CE- Co미dotsi어End加                                                                               J          뇨 I (0100 - Co（河ale川며 Errs늬e
       1口臼 Ad士e啣'N                                                                                                          自臼 A1e啣｛
       1 i iHd             RH工m니卜山1m뇨게H汁1                                                                                      卜 1 (1羊；가刃I SH - S며叫Nosnbsir Hi出 』
         n I1'i呻旿ISL鈿酬岫L애 1
                                      1nM才In                                                                         n




                                                                                                                                汗 1) 4呻디저SI. 鈿玔sanbelLoesi
         I                         F 1 (01DM - Deshnat町n Address High                                                           i: 1 [01 DH 山因a似口消d士小oH帥
         I i                       卜 1 )FFFF] DL Deoleneiron Address Loo寸                                                          口 仟FFF) DL - Dealer川ccAddreos Lo나
         1 !                       弘h) ]NI - Nodelderd卄思1                                                            !             口 NI - N岫Idenhi目
         II                        卜 I 182) 61 卜化de Discovery B.c比fr                                                 !    !        口1821 NT - Node D休covesy 8ackott
         1i                        卜--Il미N口 卜比dcCi比novery 0［山Dn;                                                          i        口 ）나40卜化巾D山1m已『y七r0：卜
         1!                        二I 1550日8] 00- Deorce TRie IdeMMier                                           1                 口 日3000] DO - Dc미：E hnm戶nmy
                                                                                                                            C二 J 口口n.,h
         heo如learnet吼照
                                                                                                                            Chonge net叫0r日59 eel面亘寸




         伽而尸陶8(944-1 FLU낳：NONE 爾而OH                                                 1                                             CIMR       96[n8十小1 FL口＼H 汁LINE XBPLI4-D卜4
                                                                                                                              H      寸   H    +   艸   山小   山                                                 1




                                                                       ［그림 1］中12]                       XBP24-DM의 Serial Number 확인


220 I 제11장 쟈그비仍야ee) 네트워킹
       COM7, COM8 각칵의 포트에 XK그lJ 프로그램과 XBee 모튤이 연결된 화면이다. 여기까
지 성공을 했다면 통신 테스트를 하는 방법은 간단하다. 乂cm 프로그램에서 Terminal
탭을 선택하고 터미널창에 텍스트를 입력하면 또다른 x-cnj 프로그램의 터미널창에 입력
한 텍스트가 그대로 Dispi町되면 XBee 통신이 정상적으로 이루어진 것이다. 통신 테스트를
위한 준비 과정은 조금 복잡하였지만 X-CTTJ 프로그램을 통한 통신 테스트 방법은 그리
복잡하지는 않다．


蚣如｝4 乂口于昏                         깠노      :       m,,m : m好二m교L1               叩［CO'너8: X'CH                                                 口 다阡m娥捌
      Ab며Jt   XModem4
      吃Re比叩3i 日미呼Ic솨 Terrnin해 i Modern Cont므Urat山ni                            絮＝
                                                                                ，伊，山叫岫的      , ,m
     4好單如懈師的叫 古制乍州黑 絮二                                                         喆置뇨 喆뇨，口8rekr ：羅ntl麓刊器出：H
                                                                                1      「   1
                                                                                                 「
                                                                                                     「「   『   「   「   ‘「   「「   『
                                                                                                                                「  「
                                                                                                                                 「「「                ,，三ji




                                                                               ii                                                                      1L
!,                                                                         1

1    江：0M7    3텨刃84小］ ELIW:N0NE
                                              二
                                                   Rn: 0却ten
                                                  雨晦   中   1   H




                                  ［그림 ]1-13] X-CTU 프로그램에서 지그비 통신 화면
                                                                   ,
                                                                       +
                                                                           !    COM0   91000-N-i FLOW:N마90                             日乂 30bi8已S




       11.3               아두이노 지그비（z由bee) 통신


      이천 Chapter에서는 지그비 통신 테스트를 위해서 x-cni 프로그램을 이용해서 통신
점검을 해 보았다면 이번 절에서는 직접 아두이노 보드를 이용해서 작성한 스케치를 아두이
노 보드에 업로드 하여 통신 테스트를 해보도록 하자．




                                                                                                 11.3 아두이노 지그비仍야兀e) 통신 I 221
  .   Arduno .



      실험에 필요한 준비물들

       지그비 통신을 테스트하기 위해서는 최소한 송신, 수신 각각 1개씩의 XBee 모듈과 XBee
      쉴드, 아두이노 보드가 필요하다. 이전 절에서는 XBee 모튤과 PC연결을 편리하게 해주는
      XBee USB Adapter를 이용하였고 이번 절에서는 아두이노와 XBee 모듈간의 연결을 쉽게
      해주는 XBee Shield를 이용하게 될 것이다．




                                                 打拿
                  薑笠 1
                           ; 00nD . .



                      11     小什버r m小m까S                J岩斗攝，,
                     1

                 Arduino UNO R3 2711              XBee Shield 27뀨



                     ,,匕         ,
                                                             근
                                                           . 管 1'
                                                                 너？




                     드吃，
                                     :,,




                            抑枷             9


                     江Be냠
                     * .,, , PFoa
                                                  et            「




           XBP24-I呱小邸IT-2印J 통신 모듈 27뀨          USB A-B 가／pe 케이블 2개




      하드웨어 연결

       우선 XBee 모튤 2깨를 각각의 XBee Sheild에 연결을 한다. XBee Shie닢에 하얀색으로
      실크 인쇄된 모양을 보면 연결 방향은 쉽게 찾을 수 있다. 그리고 나서 XBee Sh妃匕를
      아두이노 UNO R3 2개에 다시 각각 척층（연결）한다. 아두이노 보드 1개는 XB代 송신용이고
      나머지 1다臣 수신용으로 사용할 것이다．




222 1 제］］장 쟈그베刀야乂e) 뱌트워킹
                                                                                   今



         ［그림 ]1-14] 아두이노 UNO R3와 XBee S볘이d를 적층해서 연결한 그림


아두이노를 이용한 기gBee 네트워크 통신

 2개의 아두이노 보드, XBee 모듈을 가지고 하나는 송신을 하고 다른 하나는 수신을

하는 지그비 네트워크 통신 실험을 해보도록 하자．


(i) XBee 송신용 끄쿠口램

 ／才' XBee 송신용 프로그램 'V

 II pin 13 has an LED connected on most Arduino boards.
 mlt led = 13;

 boolean ack = true;

 m1lt   serln;             II var that will hold the bytes-in read from the
                           /1 serialBuffer
 char serlnString[100]; II array that will hold the different bytes
                           II 100=l00characters;
                           II 今 you must state how long the array will be else
                           I/ it won't work.
 mllt   serlnlndx   = 0;   I/ index of serlnString[] in which to insert the next
                           II incoming byte
 m1lt   serOutlndx = 0;    I/ index of the outgoing serlnStringfl array;

 void setup0 {



                                                       11.3 아두이노 지그비口야冷e) 통신 I 223
  也   Arduino




           I/ initialize the digital pin as an output.
           pinMode(led, OUTPUT);

           Serial.begin(9600);
       }
       void loopO
       {
             if( ack == true )
             {
                 digitalWrite(led, HIGH);      II turn the LED on
                 delay(1000);                   II wait for a second

                 Serial.print('REQ");
                 Serial.printinO;

                 ack = false;



             readSerialStringO ;

             if( serlnlndx > 4 )
             {
                 if( strncmp(serlnString, "ACK", 2)     ==   0)
                 {
                     // Read XBee "ACKWCr丹Lf" Data
                     ack = true;

                     digitalWrite(led, LOW);    II turn the LED off
                     delay(1000) ;               II wait for a second
                 }
                 serOutlndx = 0;
                 serlnlndx = 0;
             }

       void readSerialString 0

             m1lt sb;
             if (Serial. available0) {



224 1 제］］장 지그비（乃g皎）e) 네트워킹
                      /7 Serial.print("reading Serial String: ");    I/ optional confirmation
                      while (Serial. available0){
                         sb = Serial.read0;
                         serlnString[serlnlndx] = sb;
                         serlnlndx++;
                         //serialWrite(sb) ;                        I/ optional confirmation
                      }
                      I/ Serial.printinO;
              }
      }
  vo.d printSerialString()
      {
          if( serlnlndx > 0) {

                  //loop through all bytes in the array and print them out
                  for(serOutlndx=0; serOutlndx < serlnlndx; serOutlndx++) {
                          Serial.print( serlnString[serOutlndx] );
                               I/ print out the byte at the specified index
                               I/ serb侶tring[serOutli넋뇌 = '''';
                                //optional: flush out the content
                  }
                  I/ reset all the functions to be able to fill the string back with content
                  serOutlndx = 0;
                  serlnlndx = 0;


          }
  }

 setup() 함수에서 시리얼 포트를 초기화 하고 Serial.print("REQ"); 어］ 의해서 XBee 모듈
로 "If小Q" 데이터를 송신한다. 이후에 readSerialString() 함수에서 XBee 수신부에서 회신된
"ACK'" 데이터를 수집되면 ack 변수가 true 로 설정이 되어 다시 "REQ" 데이터를 요청하게
된다．




                                                                    11.3 아두이노 지그비（刀gbee) 통신 I 225
 .   Ard네no



     (2) XBee 수신용 프로그램

      /"" XBee 수신용 프로그램 '
                        才／

      // Pin 13 has an LED connected on most Arduino boards.
      mllt led = 13;

      boolean ack = true:

      mllt serln;    II var that will hold the bytes-in read from the serialBuffer
      char serlnString[100]; II array that will hold the different bytes
      100= loocharacters;
                // 今 you must state how long the array will be else it won't work.
      m1lt serlnlndx = 0;      I/ index of serInStringn in which to insert the next
                                     I/ incoming byte
      mllt    serOutlndx = 0;        I/ index of the outgoing serlnStringli array;

      void setupO {
        I/ initialize the digital pin as an output.
        pinMode(led, OUTPUT);

           Serial.begin(9600) ;
       }
       void loopO
       {
              readSerialStringO;

              if( serlnlndx > 4 )
              {
                  if( strncmp(serlnString, "REQ'. 2) ==    0)
                  {
                      II Read XBee "REQWCrWLf" Data



                      digitalWrite(led, HIGH);   II turn the LED on
                      delay(1000) ;               II wait for a second


                      Serial,print("ACK");
                      Serial.printinO:




226 I 제11장 쟈그비仍야ee) 네트워킹
              digitalWrite(led, Low);   I/ turn the LED off
              delay(1000) ;              II wait for a second
          }
          serOutlndx = 0;
          serlnlndx = 0;




void readSerialString 0
{
     mllt sb;
     if(Serial. available 0) {
         while (Serial. available 0){
            sb = Serial.read0;
            serlnString[serlnlndx] = sb;
            serlnlndx++ ;
            //serialWrite(sb) ;                         //optional confirmation

          i/ Serial.printinO;

}
void printSerialString0
{
    if( serlnlndx > 0) {
        I/ loop through all bytes in the array and print them out
        for(serOutlndx=0; serOutlndx < serlnlndx serOutlndx++) {
             Serial.print( serlnString[seroutlnd뇌 );
                     I/ print out the byte at the specified index
               //serlnString[seroutlndx] = " ;     //optional flush out the content
      }
      I/ reset all the functions to be able to fill the string back with content
      serOutlndx = 0;
      serlnlndx = 0;
      Serial.printinO;




                                                         1L3 아두이노 지그비仍gbee) 통신 I 227
艸    小 사duino 督



         setup() 함수에서 시리얼 포트를 초기화 하고 1OO1) 안의 readSerialString() 함수에서
       XBee 송신부에서 보내온 "REQ" 데이터를 수집하면 웅답으로 "ACK" 데이터를 보내준다．




          스케치를 업로드 할 때 XBa三 모듈이 XB田 쉴드에 연결이 되어 있다면 스케치 업로드가 제대로
         이루어지지 않는다. 스케치를 업로드 하기 전에 반드시 XBee 모듈을 XBee 쉴드에서 제거하고
         스케치를 업로드 하거나 아래 그림과 같이 스위치를 USB라고 실크 힌색으로 실크 인쇄된 쪽으로
         이동시킨 다음 업로드를 마치고 업로드가 끝나고 나면 다시 스위치를 XBa? 쪽으로 실크 인쇄된
         쪽으로 이동하면 XBee를 다시 사용할 수 있다．




         XBee 송신부와 수신부가 제대로 통신이 이루어진다면 아래 그림과 같이 터미널에 REQ,
       ACK 데이티가 1초에 한 번씩 표시가 된다. 다음 그림에서 데이터를 전송하는 아두이노
       보드가 " COM15"이고 데이터를 수신하는 아두이노 보드는 "COM12" 이다．




    228 I 제］］장 지그비（刀야표）) 네트워킹
        r
              LJ CO卜r'二5                                          '냐U CON41.i                  4   m卦啣杵                                    」口 回       x교

              1                                                    J                                                                            !
                                                                                                                                                    Send   !
          1REQ                                                           I ACE
          1REQ                                                           I ACK
        t IRES                                                           I ACE
       nREQ                                                              1ACE
      나旺U                                                                  ACE
       1REQ                                                              I ACE
       dREQ
                                                                           ACE
      URES                                                        甘AEK
      나REQ                                                               iACK
       1REQ                                                              }AnK
                                                                   Mac
     1 IRER                                                       IMcK
      nREQ
                                                                  IIAac

     FI프身二＝;
     나隧0
                                                                  r ACK
                                                                  r5CR
                                                                  [
                                                              ［了쁘『삐                                如小小              』           鈿m’叩『“切mr%llUbaud 'j
                    ［그림 ]1-15]                                                      아두이노 보드끼리 지그비 통신 테스트 화면


 참고로 아두이노 개발환경에서 시리얼 모니터 화면은 "도구／시리얼 모니터 " 메뉴를 통해
서 확인할 수 있다．

                           r的x羽之了毛；
                                  n吼햐두0*二：:5                                                       'm肛                              口回吐끼’


                           阿毛Cti-l+T니키A
                                                  printSerinlStl                         사리畢모나旦               cm-
                                                                                                                .-Sh滋                      1
                                                                                                                                i
                                                                                                                              P !

                                                                                                                                           玉
                                                                                                                        ‘M小
                           藿i                 .   .       .   .    ,            .        보느                                                뇨i
                                          " " 田"'"’畔
                                                                                "        「
                                                                                         「말"


                                                      "I呻！hr09
                                                      ior呻rwtIn
                                                                                         프루그4머                                n            I
                                                                                         부트로q굽it                                뜨          I
                           亘                              潔恣靄烈黑零如］二品露＝"恣乳뜯 I
                           i
                                                      / /reset el i the tuncEions to be able to fl U tt ' stries back pith canter
                                                      serkjtlndx
                                                      serlnlnth                 =   。;



                               i}
                                          }                                                                                              口
                                                                                                              -ii呼呼柳汕4
                                      컴파밀뫈료
                                    4pp.eI
                                                                                                          1
                                                        C刈Users뺘如kmm加pUnts娥．cc키卄Tern口楸）ci I d841 40904680520871?4,
                                                                                                                                    '   끼
                                    盟蠶玄黑咨啣叩如10 32Z鈿대트）                                                                                     홑
                           b73                                                                            , ，如            mdm므쓰‘牡！尸깬乙，


                   ［그림 11-16]                                                       아두이노 시리얼 모니터 프로그램 실행 방법



                                                                                                                                113 아두이노 지그비仍야冶e) 통신 I 229
  .   Ard내no .小1




                특정 XBee어빤 통신하71


       이전 Chapter에서는 XBee 송신 모듈에서 데이터를 전송하면 모든 XBee 모듈에 수신되
      는 형태（Broadcast）로 테스트를 해보았다. 이번에는 내가 원하는 특정 XBee에만 선택적으
      로 데이터를 송신하는 방법에 대해서 알아보자．


      실험에 필요한 준비물들

       이천 Chapter와 동일


      하드워田1 연결

       이전 Chapter와 동일


      아두이노를 이용해서 특정 XBee에만 통신하기

       2개의 아두이노 보드, XBee 모듈을 가지고 하나는 송신을 하고 다른 하나는 수신을
      하는 지그비 네트워크 통신 실험을 해보도록 하는데 이번에는 송신부의 XBee 모듈을 AT
      명령어를 사용해서 원하는 XBee 모듈에만 수신이 되도록 송신부의 스케치를 수정하여
      테스트 해보도록 하자．
       다음 그림과 같이 XBP24 XBee 모튤에는 Destination Address I玉gh, Low 바이트가
      있다. 이전 Chapter에서 XBee 모듈어］ 아무 설정을 하지 않았을 경우에는 Destination
      Address High 바이트가 Ox, Destination Address Low 바이트가 呱FFFF로 설정이 되어
      있다. 이렇게 설정이 되면 송신되는 데이터가 모튼 XBee어］ 브로드케스트 된다．
       이전 Chapter에서는 이 목적지 주소에 아무 설정도 하지 않았기 때문어］ 기본적으로
      모든 XBee 모듈 간에 통신이 이루어진 것이다. XBP24 이전에는 이러한 형태의 데이터
      통신 담당을 XBee 코디네이터가 수행하였다．




230 1 제11장 쟈그bl(Zig比向 네트워킹
                r旦［Co狎斗C兀                                二   也加           ;:                   ’口               町］
                ! 1 PC SettingsP3r3me挻
                小mdem
                               i Range 「TestPrc沁     Re！耐. Corrfi9u『計‘m' ,
                                              Terminal Modem Conhuguration{
                                                                                           『／ ]1
                                                                                               H:                          nI
                nModem            Parameter and Firmware     Parameter View』   F   'ro川e   ,        Vers向ns            ,   1i
                H Head I쓰느J          Rests"                  스쁘쁘쁘-I                 브르니              U뗀巾ad n帥1 恥
                團 rA佃ayo Update Firmw酊C                      -쁘쁘奭쁘틔                 La쁘i              V己FS1口nS'n l i ii !
                까：旽而薛甬可Fun的S탸                                                                   比1。1。 '" 1 1
                附X8P24·DM 늬如EE PR口岫MESH斗                                                       늬佃62 늬III
                1 !！回，七aNet艸며ki口                                                                                  戶出1
                LII        口 7FFF) ID．卜4odem뷔D                                                                     가i
                圃          自［다CR - Dperating Chann터                                                                 1i
                UI      ,，」h {，슥］ AR小4ac Retries                                                                 三 1!
                旨！ ! :,，小h (3) MT -M내ti-I rassm仕                                                                 nm1
                뾔 { 卜‘. (0) BH- 8山adcast日adru$                                                                   山 1t i
                目i ! ·．6h ［기M尸 Mesh Retries                                                                         II
                I ! ---- h (7] NH - Network Hops                                                                    II I
                LI ! 1」·m (3] NN小Jel叫ork 0미aySloi                                                                   11 i
                同      ····44h[0) CE - Coordinah가Ers匕노                                                             !II I
                I I 自缸Ad山cool四                                                                                     i11 1
                뾰 i 卜·m[134200) SH. Serial Number High                                                                      I
                U t      i--- 4 . 1바            · II- k rr,.r 1t1                                                          津i

                小i
                11
                              h (U] DH - Destination Address High
                            4 " (FFFF) DL- Destination Address Low
                         卜4= H卜II - N口de Identilier
                                                                                                                           ]11
                                 !
                          )82] NT Node Li匹covery 8ackott
                n i r「 yIUlNU小J口do Discovery U的ons
                t         I-                         -




                                      Device T0口e Iderititrer
                甘 i 1二 日 [50000) DD -
                1 1 =    小 m1 q口n1 r1F11
                1Read
                               pararisetero.   .OK




                                                                                           r                  H1] j
                                                                                                                 :]1
                已뜨뾔푸빠叩匪 XBP24-D而
                         ［그림 ]]-17] XBee Destination Address 설정


  이번에는 송신용 XBee모듈의 Destination Address I玉gh 바이트의 주소와 I乂叭V 바이트의
주소를 송신용 프로그램에서 AT 명령어를 사용해서 목적지의 주소를 수신측 XBee 모듈의
Serial[ Nun小er로 변경하여 특정 Serial Nui小er를 가진 XBee 모듈에만 수신이 되도록
해보자．


(1) XBee2i Destination Address & Serial Number
  X-CTU j工 루口램에서 수신용 XBee 모듈의 SH(Serial Number I五gh) 부분과 SL(Serial
Number Low) 부분을 확인한다. 송신용 아두이노 스케치에서 AT 명령어를 사용하여 송신
용 XBee 모듈의 DH(Destination Address I七gh) 바이트의 값을 수신부의 SH(Serial
Number I玉gh) 값으로, DL(Destination Address Low) 바이트의 값을 수신부의 SL(Serial
Number Low) 값으로 설정하여야 한다．




                                                                                                         1t4           특정 Xbee에만 통신하기 I 231
  e Arduino S



                             昨 [COM7j 斗CTU

                                  塑押 恥呻
                                     I
                                        뗀巾；
                                        I
                                            帥，叩뗀出艸아「i 比匹沁꺄「『
                                                lange l,est    I ermin계    m口｛J目m. UUnn므U" ' 1口in, ,                . .
                                                                                                                                        i
                                                                                                                                        』
                                  H匕5e110550


                                   500cm raramerer Sf0 rlrflrw,are
                                                                . ,,   j   raram,.erer,, view   riori,rt
                                                                                                   C  ii. , .   r   velsiurlu

                                  村 .. 1 .1’．「'" .!＋二二-J ＝孑二，    ;H 나三．寸 1)0叫，
                                                                             Ill，
                                                                                빠呻0 I
                                  1 I0WSYS up口d［日rnmYVdre d스：:：二느므쁘U 小브뽀니           1
                                  Modem：乂8EE-Pfl0 凡0口巾岫et                                                                 Verelon
                                  1XB P24-DM      크如呻的蛔MESH 2.4                                                     늬 拍U而二
                                  담七크 Net!川0南00
                                    L 目 [7FFF) ID 小，化demV山
                                       므 f디OH - 0口erOtic5 Channel
                                       自 1) AR - Mac Retries
                                       目 MT - M내liT Iansm仕
                                       [a :I8H - Broadcast Radius
                                       自 U MR - Mesh日dries
                                    ！小 口 ｛기 NH - Netwerk H햐噫
                                    卜 口 r引卜J卜i- Network Delay Sb뇹
                                    L 口 ［叩正 二oordiraatoi Too벼C
                                  日臼 Addressing

                                      d1므 [13A200ISH -Se洲Numb미Hbh 11
                                        !日 [4098E12815L -Sen계旦브mb旦J꾜뾰-I
                                         m 1.IDH- D已din日lion Address H心h
                                                                                                                                        1
                                         口 ;5FF) DL De澍1nation Addres묘Low
                                         1= 卜기 卜4ode Id已ntitier
                                         旨그）NT- Node Disc口V巳ry Backolt
                                         ［크 a NO 卜妃de D喀conery Options
                                         口              乙三 Type너已fltiliei                                                           m

                                  ci,,日n그已 n타山가目口1七lingo




                             L艸                                                                                            帥d           」
                             匠0M7 了96008卄］ FLOW:NONE )nP24-I川                                                                   r
                         \



                                         ［그림 ]]-18] XBee Ser洌 Number 설정


   (2) 특정 XBee어빤 송신하는 끄쿠기램

     ／놔" 특정 XBee에만 송신하는 立로그램 """/

     /1 pin 13 has an LED connected on most Arduino boards.
     mllt led = 13;
     boolean is xbeeconfigured = false;

     boolean ack = true;

      m1lt serln;       II var that will hold the bytes-in read from the serialBuffer
      char serlnString[100]; II array that will hold the different bytes
                              II 100= loocharacters;
               II 今 you must state how long the array will be else it won't work.
      m1lt   serlnlndx       = 0;                I/ index of serlnStringfl in which to insert the next
                                                 I/ incoming byte
      mllt   serOutlndx = 0',                     I/ index of the outgoing serlnStringU array;



232 I 제l］장 자그비（刀야翔） 네트워킹
boolean response xbeeO
{
    String response ok = 'OKWr";
    String response = String("");

    while( response.lengthO < response ok. lengthO )
    {
        if( Serial.availableO > 0 )
        {
            response += (char)Serial.read0;
        }


    ]f(response. equals(responseok))
    [
        II digitalWrite(led, HIGH);
        return true;
    ]
    else

        II digitalWrite(led, LOW)
        return false;
    }
}
boolean configure xbeeO
{
    /1 XBee를 명령 모드로 진입 시킨다．
    Serial print("+++');

    if( response xbeeO )
    1
        Serial.print( 'ATDH13A200Wr");
        Serial.printCATDL409BE128Wr');
        Serial.print CATCNWr");
    }
    else
    {
        return false;
    }

                                                       11.4 특정 Xbee에만 통신하기 i 233
  .   Arduino .



           return true;
       }
       II the setup routine runs once when you press reset:
       void setupO
       {
           I/ initialize the digital pin as an output.
           pinMode(led, OUTPUT);
           Serial.begin(9600);
           digitalWrite(led, LOW);

           is_xbee_configured = configure_xbee0;

       }
       void loopO
       {
           if( is_xbee_configured )
           I
               if( ack == true )
               {
                   digitalWrite(led. HIGH);      II turn the LED on
                   delay(1000);                   II wait for a second

                   Serial.print("REQ");
                   Serial.printinO;

                   ack = false;
               }
               readSerialStringO;

               if( serlnlndx > 4 )
               {
                   if( strncmp(serlnString, "ACK", 2) == 0 )
                   {
                       II Read XBee "ACWWCr汗Lf" Data
                       ack = true;

                       digitalWrite(led, LOW);    II turn the LED off


234 1 제］］장 자그비（乙야Xe) 네트워킹
                     delay(1000) ;         II wait for a second
             }
             serOutlndx = 0;
             serlnlndx = 0;
         }
    ]
    else
    {
         delay(2000) ;

         is_xbee_configured = configure xbee0;        /1 Retry configure
    ]
}
ye al readSerialString 0
{
         m1lt sb;
         if (Serial. available0) 1
              1/ Serial.print('reading Serial String: ");    I/ optional confirmation
              while (Serial. available0){
                 sb = Serial.read0;
                 serlnString[serlnlndx] = sb;
                 serlnlndx++ ;
                 //serialWrite(sb) ;                        //optional confirmation
                 }
                 I/ Serial.print1n0;


}
vo:d printSerialString()
{
        if( serlnl[ndx > 0) {

             //loop through all bytes in the array and print them out
             for(serOut1ndx=0; serOutlndx < serlnlndx; serOutlnclx++) {
                  Serial.print( serlnString[serOutlnd뇌 );
                        I/ print out the byte at the specified index
                  //serlnString[serOutlnd뇌 = "; I/ optionaL flush out the content
             }
             I/ reset all the functions to be able to fill the string back with content


                                                                  1t4 특정 xt光e에만 통신하71 1 235
  1   사duino .




               serOutlndx = 0;
               serlnlndx = 0;

           }
       }


       위의 코트를 보면 이전 Chapter에서 추가된 부분은 configure_xbee() 함수이다．
      conf培ure_xbee(）에서 하는 일은 AT 명령어를 사용하여 송신측 XBee 모튤의 Destination
      Address를 설정하는 것이다. 스케치에서 코드를 좀 더 자세히 보면 XBee를 명령에 실행
      모드로 진입시키는 "+++"와 3개의 AT명령어를 사용하고 있다．


      - ATDH 명령어
       Destination Address I五gh 바이트를 설정하는 명령어
       e功 ATI가113A200
       DH(Destination Address I五gh）를 수신부의 SH(Serial Number I七gh）의 값으로 설정


      - ATDL 명령어
       Destination Address I五gh 바이트를 설정하는 명령어
       ex) ATDL409BE128
       DL(Destin餌아lAddress Low）를 수신부의 SL(Serial Number Low）의 값으로 설정


      - ATCN
       XBee 모듈의 명령에 모드를 종료하고 설정 내용을 저장한다．


       스케치를 테스트하는 방법은 이전 Chapter와 동일하다. 이번 예제에서 모드 XBee어］
      데이터를 브로드케스트하고 있는 수신부를 지그비 코디테이터의 역할, 특정 시리얼 넘버를
      가진 XBee에만 데이터를 전송하는 송신부를 지그비 라우터 역할이하고 생각할 수 있다．




236 I 제］］장 쟈그비仍g以澍 네트워킹
    블루투스 통신

    12. ]   블루투스 통신
1

    12.2 얜三로이드 스마트 폰으로 LED 제어하71
  1   Arduino .




       이전에도 블루투스 근거리 통신을 이용한 무선 헤드 셋, 무선 마우스, 키보드 등에 응용이
      되딘 블루투스 응용제품들이 많이 있었지만 최근어］ 스마트 폰에 블루투스 기능이 거의
      기본으로 탑재가 되면서 관련 액세서리 산업도 급격하게 발전하면서 관심이 커지고 있다．
      이번 Chapter에서는 안드로이드 스마트 폰과 아두이노 보드를 블루투스 근거리 통신으로
      연결하여 스마트 폰에서 아두이노를 제어하는 실습을 해볼 것이다．




      口꾜          블루투스 통신


       블루투스（Bluetooth）는 1994년 에릭슨이 최초로 개발한 개인 근거리 무선 통신（PANs）을
      위한 산업 표준이다. 블루투스는 나중에 블루투스 SIG(Special Interest Group）가 정식화하
      였고, 19昑년 5월 20일 공식적으로 발표되었다. 블루투스 SIG에는 소니 에릭슨, IBM, 노키
      아, 도시바가 참여하였다. 블루투스라는 이름은 덴마크의 국왕 헤럴드 블라트란트를 영어
      식으로 바꾼 것이다. 제안을 한 사람은 拉ii Kard丞h인데, 계기는 Frans （沁nnar Bengtsson
      의 바이킹과 헤럴드 블라트란트의 관한 역사 소설 The I工）ng S比伊를 읽고 있어서 제안했다．
      블루투스가 스칸디나비아를 통일한 것처럼 무선통신도 블루투스로 통일하자는 의미인 것
      이다．
       IEEE 802.15.1 규격을 사용하는 블루투스는 PAT寸s(Personal Area Networks）의 산업
      표준이다. 블루투스는 다양한 기기들이 안전하고 저렴한 비용으로 전 세계적으로 이용할
      수 있는 무선 주파수를 이용해 서로 통신할 수 있게 한다. 블루투스는 ISM 대역인 2.45
      GI七를 사용한다. 버전 1.1과 1.2의 경우 속도가 723.1kbps어］ 달하며, 버전 2.0의 경우
      EDR(Ex血anced Data Rate）을 특징으로 하는데, 이를 통해 2.1入小們의 속도를 낼 수 있다．
       블루투스는 유선 USB를 대체하는 개념이며, 와이파이（w卜Fi)는 이더넷伍themet）을 대체
      하는 개념이다. 암호화에는 SAFER(Secure And Fast Encryption Routine)＋을 사용한다．
      장치끼리 믿음직한 연결을 성립하려면 키워드를 이용한 페어링（pairing）이 이루어지는데，
      이 과정이 없는 경우도 있다. . 이상 功i初7坑力눋 참조 -
       블루투스 1.0을 시작으로 2014년 현재 4.1버전까지 업데이트가 되었다.




2381 저12장 블루투스 통신
                       舛41尸尸寸／
                  ［그림 ]2-1] 블루투스 응용분야


 위의 그림은 최근어］ 블 루투스 통신이 사용되는 주요 제품들을 나열해 본 것이다. 위의
제품들 이외에도 우리 일상생활에 무수히 많은 제품들에 응용이 되고 있다. 그리고 블루투
스 통신에는 응용 분야에 따라서 여러 가지 프로파일（Profile）로 세분화 되어 있다．


블루투스 프로파일

 프로파일（Profile）이란 블 루 투스와 기기사이의 통신규약으로 프로토콜이라고 한다 프로
파일의 종류어］ 따라 기눙이 다르다. 우리가 사용하는 HC-(石 모듈은 여러 가지 프로파일
중에서 시리얼 통신을 하기 위한 SPP(Serial Port Pr(：沮le) 프로파일이 구현된 것이다．




口可        안드로이드 스마트 폰으로 LED 제어하기


 이번 실험은 블 루 투스 기능이 있는 안드로이드 스마트 폰을 이용하여 스마트 폰에서
블 루 투스 응용 프로그램을 이용하여 아두이노 보드에 연결된 珏D를 제어하는 실습을 해보
도록 하겠다．




                                 12.2 안드로이드 스마트 폰으로 LED 제어하71 1 239
  .   Ard네no



      실험에 필요한 준비물들


                                           a.
                                       닯             ；的（匹9싸


                                                 11                      1
                                                S
                                                                                 卜／      ,




               브래드보드 I깨1                    아두이노 UNO R3                      적색 LED/1K 저항 2개1

               小
               ;   0
                       "   '   "   n            ruiru
               UI.
                                                               J




                                                 I         r11===1
                                                           i
                                                           1===1mm

                                                 스    口    心       11/
                                                 X    X    Z       kd
                                                 t    1H   口       >

                                                 1 亡 a.

        안드로이드 블루투스 APK                 HC-06 블루투스 모듈




      하드워때 연결

       우리가 사용하는 HC니而 블루투스 모듈은 아두이노에서 시리얼 통신을 이용해서 통신을
      할 수 있는 모튤이다. 4개의 핀이 있는 RXD, TXD, GND, VCC 핀을 가지고 있다 블루투스
      모듈의 vcc 핀을 아두이노 보드의 3.3,\/ 출력 포트와 GNT) 핀은 아두이노 보드의 GND
      포트와 연결을 하면 되고 RXD 핀은 아두이노 보드의 D3포트와 연결하고 乃a) 핀은 아두이
      노 보드의 D2 포트와 연결을 한다．
       HC-(石 모듈의 -I＞그） 핀을 아두이노 보드의 DO(RXI力 포트와 RXD 핀을 아두이노 보드의
      D1(TXD）핀과 연결하여 시리얼 통신을 해도 되지만 여기서는 아두이노의 소프트웨어 시리
      얼 포트를 이용해서 통신을 하기 위해서 D2, D3 포트에 연결을 하였다．




240 I 제］2장 볼루투스 통신
           ［그림 ]2-2]             HC-06 모듈 연결 배선도




     SET      Arc出Jino             TxI00
                Uno                RX/0I
                                                          64ue1o0甘）
                                                          Seror5
 REF           (Rev3)                 02

           Ar4U1nO UN0 R3        p聊盛｛［노3

                                      04

                                 p坰닒 D5
 1                               p附A 05

                                      07

                                      05
A F; /A                          PW1A 0！크
自汀S二 1                        ES伊WM 010

                            MC）듸伊WM ［기 1

                               h川5O/（긔 ?

                                 Sc町미:i




                    GND


                     i
           ［그림 ]2-3]           HC-06 모듈 연결 회로도



                                            12.2 안드로이드 스마트 폰으로 LED 제어하기 1 241
 1 Ar,：加'no



     쿠기램 작성

     아두이노 스케치에 아래와 갇은 코드를 작성한다．

      #include <SoftwareSerial.h>

                                  匕
                                  n
      m1lt bluetoothTx =
                                  d
                                  n
      m1lt bluetoothRx =
      mllt LED = 9;

      SoftwareSerial bluetooth(bluetoothTx, bluetoothRx);

      void setupO
      {
              Serial.begin(9600);
              delay(100);
              bluetooth.begin(9600) ;
              pinMode(LED, OUTPUT);
      }
      void loop()
      {
              char cmd;
              if(bluetooth. availableO )
              {
                  cmd = (char)bluetooth.read0;
                  Serial.print("Commarid = ");
                  Serial.println(cmd);

                  if( cmd == '1' )
                  {
                      Serial.println("LED ON");
                      digitalWrite(LED, HIGH);
                  }
                  if( cmd == '2' )
                  {
                      Serial.println('LED OFF');
                      digitalWrite(LED, LOW);
                  }
              }
          }


242 I 제］2장 블루투스 통신
 叛祉加ci匕1儡丹w打eSei娘／
                 ．方)
        원래 시리얼 통신을 하기 위해서는 아두이노 보드의 D0(F<D), D1(ThD) 2개의 포트를 이용
        해야 하는데 以）, D] 포트를 이용하면 하드웨어적으로 정확하7朴 이야기하면 ATMEGA CRJ
        에서 지원하는 하드웨어 시리얼 포트를 이용하는 것이고 아두이노에서는 소프트웨어적으로
        시리얼 통신을 할 수 있는 라이브러리를 지원하는데 이 라이브러리를 사용하기 위해서
        필요하다．


加rb／比to야方Tx = 乙‘

        블루투스 모듈의 Rx핀과 연결될 아두이노 보드의 D2 포트


mr blueroorhRx = 3;

       블루투스 모듈의 Tx핀과 연결될 아두이노 보드의 D3 포트


亡2r L丑O = 9,.

       안드로이드 스마트 폰에서 제어할 匕ED가 연결된 포트


So丹n位reSeri뇨／ b／口etc刃I方(blueroo功乃夕 blueroothR姑

       소프트웨어 시리얼 포트를 사용하기 위해서 선언한다．


5匕i勿／
    .6留加四呪也七

       하드웨어 시리얼 포트를 9600b口S 속도로 초기화한다．


Set勿Lb凹h四6疏까r

       소프트웨어 시리얼 포트를 9600bps 속도로 초기화한다．


II仍加吐OO1方.avail눈bleO)

       블루투스 모듈로부터 송신된 데이터가 있다면 . ..


cmd = (c／伍r乃／口etool力. read彷

       블루투스 모듈로부터 송신된 데이터를 읽음


Set始／.／끄力W'Con끄mind = 玄
Set勿如th끄加化rn라：

       블루투스 모듈로부터 송신된 데이터를 시리얼 포트로 출력




                                        12.2 안드로이드 스마트 폰으로 LED 제어하기 1 243
 .       Ard내110 S-




     Jf( and == '1')
     I
              ．戶i亡ltln(乞石D （기V吩
          Se虹눈／
          （如伽1W址e伍끄), I끄GI勁

     I
                송신된 데이터가 ' ] '이면 LED를 켠다．

     if( cmd == '2')
     I
          Sen눈／.pr1ndn(伍石D O1冽上：
          （娘加胛ni肥伍五1工 끄2W玄
     I/
                송신된 데이터가 ' 2'이면 匕ED를 끈다．

     실행결과

      이번 예제를 실행하기 위해서는 안드로이드 운영체제의 스마트 폰과 블 루투스 응용
     프로그램이 필요하다. I코D를 제어하는 블루투스 제어 애플리케이션（앱）을 개발하는 방법
     을 설명하끼에는 이 책의 범위를 한참 벗어나기 때문어］ 이번 실험을 할 수 있는 안드로이드
     용 애플리케이션은 이미 안드로이드 앱 장터에 많이 있기 때문에 그중에 한 가지를 다운로
         드하여 설치하여 테스트해보도록 하겠다.


         (] ) 애플리케이션 설치
          안드로이드 마켓에서 아래 그림과 같은 애플리케이션을 다운로드 하고 설치한다. 애플리
         케이션 이름은 "블루투스 컨트롤"이라는 애플리케이션이다. 참고로 아래 애플리케이션
         개발자의 이메일（ckh12312@grnail.c恤） 주소이다．




2441 제］2장 블루투스 통신
      (I,
                         앱                                                            <    （극，
                                                                                                            (0blueto-oth serial controller               q
                                  볼루투스 컨트를
                                  더MEAPPS                                                                    얩4
                                                                                                                           Bluetooth Spp
                                                                                 孚｛
                                                                                      ,

                                                                                                             客        2. B如e｛口oth SPI그 丁cot


                                                                                                             只＞        "    "




                                                                                                                      4 GetSIUe Blueto口th Reader. Demo

                                                                                                                      出 缶 咐食




      설명                                                                                                              毛 SRNA 8Trri引 미ueB口口Itt 丁er月Hnai

      뷸쿠투스毋 이용히여 시리얼 동신뇰 할 수 있습니다．




                                                      ［그림 12-4]                                       HC-06 모듈 연결 회로도


(2) HC-06 블루투스 모듈과 페어링
 블루투스 장치들끼리는 통신을 하기 전에 페어링이라는 과정을 거쳐야 한다. 한번 페어
링이 완료된 장치들끼리는 이런 과정을 거치지 않아도 자동으로 송수신이 가능하다．

            ,,   y
                     '                                                                           =?




            블루투스 등록 요청

                     HC-06욜（룔）듬록하려면 비밀번호（0000
                          또는 123긔를 입력 하세요


            H
     m                                                             2!
                                                                    -
     1               2       3        4       5       6   7        8                  9    0

                                      !       ?       八   r        火                  #
                     (       )                @1                    1

                                                                                           !
      1/3                \       3노       0       &           S              {            43

     ABC         每                    L尸J                     口염
                                                                        I/
                                                                                          완료


                                                              ［그림 12-5] 블루투스 페어링


                                                                                                            12.2 안드로0드 스마트 폰으로 LED 제어하71 I 245
    Arduino .-



     페어링을 하기위해서는 비밀번호를 입력해야 하는데 HC-06 모듈의 초기 비밀번호는
   "1234"이다．


   (3) 블루투스 애플리케이션 키（버튼） 설정
     블루투스 애플리케이션의 ' 키 설정 "이라는 메뉴를 이용해서 ' 0N"="l "로 설정하고
   "OFF"="2"로 설정한다．


                         J 1        >1
                         +     r1   =




                        Bluetooth Controller
                        연결되었습니 다HC06




                     ［그림 ]2田］ 블루투스 애플리케이션 키 설정


   (4) 아두이노에 연결된 HC-06 모듈과의 통신
     블루투스 애플리케이션에서 "0寸 버튼과 "0FF" 버튼을 눌러서 아두이노 보드에 연결된
   LED가 켜지거나 혹은 꺼지는지를 확인한다．




246 ! 제］2장 블루투스 통신
이더넷（Ethernet)
               네트워킹
  13. ]   이더넷（Ethern혜이란7
  ]3.2 Ard내no 日hernet Shield 소개
  13.3 웹 클라이언트（고정 P)
  13.4 웹 브라우저로 아두이노 LED 제어하71
  4 Arduino




   1ki4 이더넷（타hernet)이란9

      이천 절에서 乃gBee 네트워킹을 이용해서 센서의 데이터를 乃gBee 각 노드들 간에 근거
    리에서 무선으로 전송하는 실험을 해보았다면 거리에 상콴없이 아두이노 보드를 인터넷망
    혹은 LAN(Local Network Area）에 연결하여 센서 데이터를 공유하고 싶다면 이더넷
    (Ethernet）을 이용하면 쉽게 할 수 있다．


    .J小

        이더넷（E由emet）은 Li小을 위해 개발된 컴퓨터 네트워크 기술로, "이더넷"이라는 이름은 빛의
      매질로 여겨졌던 에테르（ether）에서 유래되었다. 이더넷은 Os' 모델의 물리 계층에서 신호와
      배선, 데이터 링크 계층에서 八4AC(media access contr아） 패킷과 프로토콜의 형식을 정의한다．
       이더넷 기술은 대부분 IEEE 802.3 규약으로 표준화되었다.       ' 위刃백과 안용




   口回 Arduino 단hernet Shield 소,ii
      임베디드 하드웨어를 인터넷망에 연결하는 작업은 쉬운 작업은 아니다. 물리척으로는
    이더넷 포트（소켓）와 이더넷 통신의 물리계층부터 어플리케이션 계층 이전까지를 처리해줄
    이더넷 통신 CI-印과 TCP/IP, UDP 등 프로토콜을 지원해줄 복잡한 소프트웨어가 필요하다．
    하지만 이것들에 대해서 모른다고 해서 걱정하지 마라. 다행히도 우리에게는 아두이노에서
    제공하는 Ethernet Shield라는 하드웨어 보드와 아두이노 IDE와 함께 제공되는 강력한
    소프트웨어 라이브러리가 있다. Arduino Ethernet Shield 이용하면 간단한 작업으로도
    이더넷 통신을 할 수가 있다.
      Arduino Ethernet Shield는 硼如et 사T5100 風hernet IC를 사용하여 TCP, UDP, ICMP
    등의 네트워크 연결에 대한 처리를 할 수 있도록 도와준다. 이 하드웨어는 단독으로 사용할
    수는 없고 Arduino UNO R3와 연결하여 사용 가능하다.




248 I 제］3장 이더넷乍I-日I甘） 네트워킹
                         ［그림 ]3- 1]   아두이노 日hernet Shield




1k미 월J 클라이언트（고정 ip)
 Arduino Ethernet Shield에 고정 II) 주소를 아두이노 스케치에서 설정한 이후에 인터넷
웹서버에 접속해서 인터넷 페이지를 요청하는 실험을 해보자. 구글이나 네이버 등의 웹서
버의 검색 메인페이지에 첩속해서 어떤 데이터가 오는지를 확인해 보자. 이 실험은 血（虹no
＆뇨met Shie뇌가 정상 동작을 하는지 확인해 볼 수 있는 가장 쉬운 방법이다. 이천까지는
Arduino UNO R3 보드만 필요했지만 이더넷 실험을 하기 위해서는 Arduino Ethernet
Shield 하드웨어도 같이 필요하다．


실험에 필요한 준비물들




   Arduino UNO R3 1711       Arduino Ethernet Shield 1711   刃45 인터넷 케이블



                                                            13.3 웹 클라이언트（고정 IP) 1 249
  .   ／놔d내no 卜




      하드웨어 연결

       아래 그림과 같이 Arduino UNO R3하드웨어와 Arduino Ethernet Shield 하드웨어를
      적충하고 네트워크 케이블을 이용하여 風hernet Shield의 珂45 유선 랜 포트와 데트워크
      HUB 혹은 인터넷 망에 연결한다．




                      ［그림 13-2] 아두이노 UNO R3 보드와 日hernet Shie녑 보드 적층


      끄쿠口램 작성

       아두이노 스케치에 아래와 같은 코드를 작성한다．

       1*
                 Web client

            This sketch connects to a website (http: //www. google. corn)
            using an Arduino Wiznet Ethernet shield.
            水／
       #include <SPI.h>
       #include <Ethernet.h>

       II Enter a MAC address for your controller below.
       II Newer Ethernet shields have a MAC address printed on a sticker on the
       shield
       byte macti = { 0xDE, 0xAD, 0xBE, 0xEF, 0xFE, 0xED I;

       I/ if you don't want to use DNS (aid reduce your sketch size)
       II use the numeric IF instead of the name for the server:




250 1 저13장 이더넷（다en甘） 네트워킹
 char server[] = "www.google.com";                 II name address for Google (using DNS)

II Set the static IP address to use if the DHCP fails to assign
IPAddress ip(192, 168,219,161);

I/ Initialize the Ethernet client library
II with the IP address and port of the server
II that you want to connect to (port 80 is default for HTTP):
EthernetClient client;

void setupO {
             II Open serial communications and wait for port to open:
             Serial.begin(9600) ;
              while (!Serial) {
               ; /1 wait for serial port to connect. Needed for Leonardo only
             }

         II start the Ethernet connection:
          if (Ethernet.begin(mac) == 0) {
             Serial.println( 'Failed to configure Ethernet using DHCP");
            II no point in carrying on, so do nothing forevermore:
            II try to congifure using IP address instead of DHCP:
            Ethernet.begin(mac, ip);
          }
         II give the Ethernet shield a second to initialize:
         delay(1000) ;
         Serial.println("connecting. .. U);

  /1 if you get a connection, report back via serial:
   if (client. connect(server, 80)) {
      Serial.printlnCconnected");
     1/ Make a HTFP request:
      client.println("GET /?gws rd=cr&amp ; eizjoumUuCxElrekAXNplDoCw
I끄叩P/ i 1");
     client.print1n0;
         }
  else
                   {
                 II If you didn't get a connection to the server:
                 Serial.println("connection failed");
         }

                                                                    13.3 웹 클라이언트（고정 IP) I 251
  +   사d내rio .




        }
       void loopO
         {
              I/ if there are incoming bytes available
             II from the server, read them and print them:
              if (client. availableO) {
                 char c = client.read0;
                 Serial.print(c);
              }
             //if the server's disconnected, stop the client:
              if (!client. connectedO) {
                   Serial.print1n0;
                   Serial.println("disconnecting.");
                   client. stopO;

                  Ii do nothing forevermore:
                    while(true);
              }



        이 코드는 단순히 네트워크 설정이 잘 되었는지를 확인하기 위해서 구글 웹서버에 FflTP
      프로토콜로 접속해서 GFI' 메소드를 요청하는 코드이다. 참고로 이 예제는 아두이노 사의
      튜토리얼（h叩／/arduino.cc/en/Tutorial!사陀bClient)에서 약간 수정한 코드이다．


      char serveril = "www.google.com'r
                   日hernet Shield에서 접속할 웹 서버의 도메인 이름을 지정하면 된다. "ww.de너cesh아）
                    .net". "낚川w.naver.com" 등 어떠한 웹 서버가 오더라도 상관은 없다．


      'P녔a바ess 巾口9乙끄5昌21旦끄刃方
                   日hernet Shield가 사용할 'P주소를 지정하면 된다. DHCP(Dynamic Host Configuration
                    다이oc이）를 이용해서 자동으로 P를 할당하는데 실패한다면 이 주소를 사용해서 인터넷
                    망에 접속할 것이다 ．어떤 'P 주소로 할당할지를 잘 모르겠다면 네트워크 관리자가 있다면
                    관리자에게 문의하거나 도움을 청할 사람이 없다면 보통은 아라1 그림과 같은 절차에 의해서
                    짐작을 할 수 있다. 윈도에서 명령 프롬프트 창을 실행시키고 "1口config " 명령을 실행한다.




252 I 제］3장 이더넷（日mm) 네트워킹
             四   귿큼 프롬프트                                                                        ' 二：그   쓰三1   "h5

             :以1sej-   '   r   n   -    -




             lindow毛'P 구성


             무선 1Jt1可 어댑터 무선 네트워크 연궐 2:

                 미디어 상타1                          · 미디어 띤결 끊김
                 연결별 D卜心 접미사

             무선 i小N 어댑터 무선 네트워크 연궐＝

                 연결별 OHS 접미사
                 링크h로컬 IPn6 주소          f e8日＝:8, d2 :bn91:a日3b 125Pdlill
                                                                                                                    !
                                                                                                                    1
                 IPw4 주소              - 192.168.219.192
                 서브넷 마스크              ' 255 - 255 . 255．日
                 기본 게이트워回 . . . . . . : 192．工68 . 219 .1

             이더넷 어댑터 Bluetooth 네트워크 연결：

                 미디어 상EH                            미디어 연궐 끊김
                 연궐별 OHS 졉미사

             II더넷 어댑터 로컬 영역 연궐＝

                 연궐별 DNS 접미샤． . .
                 링크1로컬 I Pu6 주소                   - FeB日：:6d2a: 9167: 74th   4日c1i1目1
                 IPu4 주소                          - 192.168.219 .168
                 서브넷 마스크                          . 255.255.255 .8
                                                                                        !
                 기몬 게이트워回                         · 192.168.219 1
                                                                .
         \                                  七旺如     小       醉           1                   小                       J




                                       ［그림 13-3] PC의 이더넷 'P 주소 확인


 위의 그림에서 ' IPv4 주소" 어］ 해당하는 192.168.219.160는 현재 윈도 PC가 사용하고
있는 'P주소이다. 그러므로 192.168.219.160를 제외한 192.168. 219.x匹 'p주소를 사용하
면 된다. 물론 이러한 방법도 Gateway에 따라서 항상 맞는 방법은 아니지만 일반적인
경우에는 이러한 방법으로 찾아낼 수 있다. 여기서 주의해야할 점은 사내 혹은 학교 등에서
다수의 PC가 운영되는 네트워크어］ 속해 있다면 192.168. 219.x承의 주소는 중복이 되어서
사용하면 안 된다는 것이다.

cJJein.prindn("GET／會wsrd=cr如짜加勻ournUuCx吼rekAX쨔ill石Cw 月m力. lit),,.
      위의 코드에서 "刀gws_rd=cr&amp ; ei=joumLJu(）
                                           日rekXN이以兀w "는 구글의 시작페이지
      를 나타내는 것이다. 이 방법 이외어匠 구글 서버에 다양한 （게ent 요청을 할 수 있다．

- "GET /search?q=arduino I卄［P/1.1" : 구글 서버에 "ardt血山"라는 검색어로 검색요청


실행결과

 아두이노 시리얼모니터 윈도에 "connected"라는 문자가 표시 된다면 일단은 Arduino
Ethernet Shie匕의 네트워크 설정이 올바르게 된 것이다. "connection failed"라는 문자가
보인다면 스케치 코드의 'P 주소 설정이나 네트워크 케이블이 올바르거］ 연결이 되었는지를
확인한다. 연결이 성공적이라면 시리얼 모니터에 아래와 유사하게 표시가 될 것이다．

                                                                                            13.3 웹 클라이언트（고정 IF그） I 253
  .   Arduino



                '熙느:o,，口                                                                       ,                 磊                ,                                      ,                   [ .c＝니回除也3叫1'

                                                                                                                                                                                                                 Send
                r                                                                                                                                                        나小    十十          尸H小




                                                                            1
                            뇨 m
                                                  十 小           小           小                                                                                                                                                    4




                量c。
                                     nnec少            "·    ·       ·                                                                                                                                                                )
                  I1TTP/1.1 200 마
                  Date; Tue. 10 Dec 2013 04:29:35 0NT
                多 Expi res: 口1
                量Cache-Control : private, max-age=O
                哥Content-  Type: text/html charset= 150-6859-1
                童Set-Cookie: PREF=山=adlf 63Sf 32b6daf I :FF=O: TM=I3665407?5:LM=1306649715:S=zWeUbtYrlF3
                賈 Set-Cookie: 聊＝67=H0Lk8rk0rRQ미凸TKO帥川妊朋pn니f TK7f s匪曲13洲p耐／Lo羽쩨田ab2止
                事P3P: CP=··This is n。 t a P3P p。
                                               l icy! See http: //wwe. g。。gle. c。
                                                                                m/supp。rt/accounts/bin/a
                  Server: gee
                  斗將S-Pr火action: I .' sode=b lock
                  0-Frame-Options: SAMEOR 101N
                  川ternat于마먀ocol : 80：叫比
                   Transfer-Encoding: chunked

                            8000
                            <!doctype html><htsl itemscope=' " itestype="http://schems.org/WebPage"><head><meta
                            삐ndoe. goo引e=4kE I／띠mU山匪0왜姑啼山ABA", get티 :function(s)｛化r(var b;a&&(1a.yetA
                            k);d,onerror=d.onIoad=d.onabort=functionQ{delete f[ e]};f[ e] =d;cII-1!=b. search('&ei
                            '   ;"    "   "   n   '        /1   .   _           n "   n"   '   n nnn    '   n   k41.   小   S9L.       .,_.小,   i八   .,aFC   .   .   .J   'tl   IIII \ II     "n八       \   ,1_   I, ,4. .,   4




                                塑Autosc『미                                                                                                                   Carriage re加
                                                                                                                                                                       『n.i 鈿m蜘立m簪
                    (       니 如如      卄nm                                                                                                                                                                                    山           텨


                                                                                  ［그림 ]3-4] 구글 검색 실행 결과


       위의 내용을 복사해서 go(넣e.hti쿄이라는 파일로 저장을 한 다음 웹 브라우저에서 열어
      보자. 저장을 할 때 " (html" 태그로 시작하는 부분에서 " (/htm1) "로 끝나는 부분까지만
      저장을 해야 한다．




                                                                                                        G口ogle Sea父a                           rm,-ee卜OQ LI比Ky




                                              Mood心rngF가ograms                                          Business S혀Cl田ns                        *Goage               Aboull3oc冬地            Go四le so kr
                                                                        1             小巴           mH                                                   口                                          n
                                              二




                                              ［그림 13-5] 인터넷 브라우저에서 실행결과 확인


254 I 제侶장 이더넛佃e了甘） 너트워킹
 아마도 위와 유사한 내용을 랜더링 해줄 것이다. 여기까지는 Ethernet Shield가 웹 클라이
언트의 역할을 수행하는 실험을 해보았다. 다음 Chapter에서는 Ethernet Shield를 웹 서버
로 변신시켜보자．




 13.4      웹 브라우저로 아두이노 LED 제어하71


 이번에는 Ethernet Sh妃넌를 웹 서버로 변신시켜 웹 클라이언트（인터넷브라우저）에서
아두이노어］ 있는 I且）를 켜거나 혹은 끄는 테스트를 해볼 것이다. 아두이노를 웹 클라이언
트로 동작시키는 것보다는 서버로 동작시키는 것이 많은 흥미로운 실험을 더 해볼 수
있다．
 이번 예제에서는 단순히 LEL를 （如／아I 하는 테스트이지만 만약 아두이노 風Llernet
S노eld가 온도센서, 조도센서 , 습도센서 둥에 연결이 되어 있다면 인터넷 브라우저를 통해
서 각종 센서들의 값을 조회할 수도 있다．


실험에 필요한 준비물들




  打duino LJNO R3 17귀1   Arduino 且hemet Shield 17뀨
                                                       H
                                                    적색 比D/1I( 저항 27下1




      브래드보드 17긔1           珂45 인터넷 케이블




                                          13.4 웹 브라우저로 아두이노 LED 제어하71 1 255
  .   Arduino



      하드웨어 연결

       우선 아두이노 UNOR3 보드와 Ethernet Shie닢를 적충한다. 그리고 나서 아래 그림과
      같이 웹 브라우저에서 제어할 LED를 아두이노 보드의 D3포트에 연결한다. 배선 연결은
      비교적 간단하다．




                   ［그림 ]3-6]    월J 브라우저로 아두이노 LED 제어하기 배선도


       위의 그림의 배선도에는 아두이노 1分qOR3 그림만 보이지만 실제 실험을 하기위해서는
      그림 13-2처럼 아두이노 UNOR3와 風hernet Sh妃匕를 적층해서 실험을 해야 한다．


      .1工쿠기램 작성

       아두이노 스케치에 아래와 같은 코드를 작성한다．

        #include <SPI.h>
        #include <Ethernet.h>


        /1 Enter a 入AC address and IF address for your controller below.
       II The IP address will be dependent on your local network:
       byte macEl = { 0xDE, 0xAD, 0xBE, 0xEF, 0xFE, 0xED };
       IPAd打ess ip(192, 168,219,161);



256 1 제3장 이더넷（E寸旬싻） 네트워킹
/1 Initialize the Ethernet server library
II with the IP address and port you want to use
II (port 80 is default for HTFP):
EthernetServer server(80);

m1ll; led = 3;
String get method string = String(20);

void setupO
{
      //initialize the digital pin as an output.
      pinMode(led, OUTPUT):
      digitalWrite(led, LOW):     /1 turn the LED off by making the voltage LOW



     II Open serial communications and wait for port to open:
     Serial.begin(9600) ;

     while (!Serial) {
      : II wait for serial port to connect. Needed for Leonardo only
       }

     II start the Ethernet connection and the server:
     Ethernet.begin(mac, ip):
     server.beginO ;

     Serial. printC'server is at "'):
     Serial.println(Ethernet. locallPO):


 }
void loopO {
     /1 listen for incoming clients
     EthernetClient client = server. avai1ab1e0;

     if (client)

       Serial.println("new client'):
       II an http request ends with a blank line



                                                   13.4 웹1 브라우저로 아두이노 匠D 제어하기 I 257
艸   如 0 Arduino



                  boolean currentLinelsBiank = true “,
                  while (client. connectedO)
                  {
                      if (client. availableO)
                      {
                          char c = client.read0;

                          if( get_method_string.length0 K 30 )
                               get_method_string. concat(c);

                          Serial. write(c);
                          I/ if you've gotten to the end of the line (received a newline
                          II character) and the line is blank, the http request has ended,
                          ii so you can send a reply
                          if (c == 'Wn' && currentLinelsBiank) I
                             II send a standard http response header
                             client.println("HT叩/ 1.1 200 OK");
                             client.println("Content-Type: text/html") ;
                             client.println("Connection: close"); // the connection will be closed
           after completion of the response
                     client.printinO;

                            client.println(" <.!DOCT그PE HTML>");
                            client.println(" <html>");
                            client.println(" <head> <title>打duino LED ON/OFF
           Test K/title> </head>");
                         clientS println(" <body>");

                            client.println(" <br />Arduino LED(Pin13) ON/OFF Test <br I> <hr
           /><br />") ;
                     client.println(" <form method=W"getW" name=W'ledW">") ;
                     client.println(" <input type=W"submitW' name=W"button1W"
           value=W"LED' ONW' />");
                     client.println(" <input type=W'submitW" name=W"button2W"
           value=W"LED OFFW" I>");
                     client.println(" </form>");
                     client.println(" </body>");
                     client.println(" </html>");

                             if (get_method_string.indexOf("buttonl=LED+ON")!=-1)



     258 I 제］3장 이더뺐텨eT甘）너트워킹
                           {
                                  digitalWrite(led, HIGH); /1 LED ON
                                  Serial.printlnC'=== LED ON");
                           }
                           else
                           {
                                  digitalWrite(led, LOW); II LED OFF
                                  Serial.println("=== LED O1그I그’ );
                           }
                           Serial.printlnC'get_method_string = " + get_method_string);
                           get_method_string = ";

                           break;
                       }
                       if (c == '砥／n ')
                       {
                           II you're starting a new line
                           currentLinelsBlank = true;
                       }
                   else if (c != 'Wr')
                   {
                           II you've gotten a character on the current line
                           currentLinelsBlank ：二 false;
                       }
               }
           }
           II give the web browser time to receive the data
           delay(1);
           II close the connection:
           client. stop0;
           Serial.println("client disconnected");
       }
   }

万的cr11cr5匕rver server(8口七

               인터넷 월J 서버（Hrm 서버）는 보통 80 포트를 사용하게 된다．




                                                             13.4 월J 브라우저로 아두이노 LED 제어하71 I 259
.   Ard내no .



      이 예제를 이해하기 위해서는 HTTI) 프로토콜과 I끄M어］대한 약칸의 이해가 필요하다．
    HTTP 프로토콜어］대한 자세한 내용은 h蚌刀＼www.w3.org/Protoco넣迂C2616肝c2616-sec5.html
    에서 확인할 수 있다. 많은 내용들이 있지만 우리가 일아야할 중요한 내용은 웹 클라이언트（브
    라우저）에서 어떤 요청이 올 때 마지막에 항상 "CRU고"가 붙는 것이다. 이 점을 이용해서
    스케치 코드 작성시에 웹 클라이언트의 요청에 대한 서버（Ethernet S比eld）의 HTE) 웅답을
    하면 된다.


    실행결과

      인터넷 브라우저를 통해서 아두이노 Ethernet Shield의 네트위크 'P로 접속을 한다．



                          三J.b::c   192.168;219.161   GUn乙fli二L已그 m 乙 "

               ＝了Arduino LED ON/OFF Test

               슉 ! 囹 寸         : 蜘 r 페이지（P) !          만전（S) !     도구（O）寸 S.! 列 卿 0


               Arduino LED(Pin3) ON/OFF Test




                     ［그림 13-7]             인터넷 브라우저로 匡D 제어 실행화면



      이제 브라우저에서 "I五DOI시力 Ornoa 五DOFF" 버튼을 눌러서 1介qOR3에 있는 I且）상태에
    변화가 있는지를 확인해 본다．




2印 1 제］3장 이더넷（테旬甘） 너트워킹
      圄COM9                                          :；難                     申 回！ 呈g n
                                                                                   繫哺解燕難
         server is at 192 , 188, 219. 161                                                        A
        ne뽀cl ient
      fT /?buttonl=LED+ON
                              HTTP/l , l
                                                                                             圄
                                                                                             녀
      Accept: text/html, a口P1 ication/ xhtml+x川』 士／+                                         囹
      Referer: http: //192. 168,219, 161/?butt。
                                              nl=L[fl+DN                                     뼈
      Accept-                KR
                           Language:
                                              ko-
                                                                                                     }
       User-
                  Agent:
                        I la/5月 (compatible; MSIE 9. Windows NT 6.
                                       MoZi
                                                       0
                                                           '            1;
                                                                             Trident/5. 0)       1
      Accept-Encoding: gzip, deflate
      Host: 192. 168.219: 161
      Connection: Keep-Al ive

      ===LED ON
      get_method_ string = 20BET /?buttonl=LED+ON HTTP/1 .
      cl ient disconnected                                                                   中
               固Autoscr미1                              Carria묘e:re如rn        廟00 baud        寸

                                       ［그림 ]3-81 LED저뻐 시리얼모니터 실행화면


 이 외에도 아두이노에 스텝 모터가 있는 II) 카메라 등이 연결되어 있다면 인터넷브라우저
를 통해서 모터를 제어해서 원격지의 II) 카메라의 상하좌우를 조정하여 원하는 장소의
화면을 복 수도 있을 것이다．




                                                               13.4 월1 브라우저로 아두이노 LED 제어하71 1 261
  ！冪훈
                                十 1寸了

                                      J
                                          澍瀜料
                                                鸚




사물인터넷이란？

        14. ]   사물인터넷이란 무엇인가2
        14.2 사물인터넷 주요 서비스
        14.3 주요 loT 제품 및 서비스 동향
        14.4 주요 loT 구성요소 및 현황
        14.5 가전, IT 기업들의 사물인터넷
                플랫폼 주도 현황
      .   Arduino .




           14.1       사물인터넷이란 무엇인가？


           사물인터넷을 자세히 알아보기 전어］ 우선 사물인티넷이 활성화되면 가정에서의 우리
          생활이 어떻게 변화되는지 상상해 보자. 지난밤에 약간 과음을 하고 늦은 시간에 귀가하여
          잠이 들었고, 아침 7시에 내 스마트폰에서 평소 내가 좋아하는 음악 소리의 알람에 따라서
          무겁게 눈을 뜬다. 평소에는 아메리카노를 즐겨 마시지만 집안에 설치된 환경 센서를 통해
          서 음주를 했다는 사실을 스n任i폰에게 자동으로 통보를 하고 스마트폰은 다시 커피머신에
          게 7시 전에 아메리카노 대신 음주 후에 즐겨 마시는 시원한 까페라떼를 만들어 놓으라고
          전달을 한다. 침대와 베게에 설치된 수면 상태 측정 센서와 변기에 설치된 소변 분석 센서는
          이미 수면 패턴과 소변을 통한 기초 컨강 상태를 체크하여 클리우드 서버에 나만의 생체
          보안정보와 함께 전송이 완료된 상태다. 커피를 들고 거실의 소파에 앉으면 T\／에서는
          내가 가장 관심 있어 하는 분야인 IT소식과 좋아하는 야구단 소식을 리스트해서 보여준다．
          가족들과 함께 아침 식사를 마치고 현관에서 아침 인사를 하면 현관에 설치된 스마트
          홈 모니터링 시스템은 이러한 행동 패턴을 분석하여 출퇴근용 자동차에게 명령을 하여
          엘리베이터 앞으로 이동을 하여 기다리라고 지시한다. 엘리베이터에서 내리면 바로 자동차
          가 대기 하고 있다.
           마치 공상과학영화에서나 가능할만한 이야기이지만 사물인티넷 시대가 되면 머지않아
          이러한 생활이 일상화 될 수도 있을 것이다. 이렇듯 사물인티넷이란 가장 간단하께 정리
          하자면 말 그대로 사물 간에 통신을 주고받는 것이다. 하지만 이와 같이 간단하게 정리하면
          사물통신（M2M小4achine to 八4achine), 과거의 유비쿼터스（Ubk弘迂ous）와 무엇이 다른가？
1         사물인터넷은 사물간의 통신이라는 기본 전제에 각 사물어］ 지능（Intelligence）을 더하고
          이러한 지능은 인간이 개입（컨트롤） 없이 사물간의 통신으로서 인간의 편의를 위한 데이터
          를 자동으로 수집하고 이 거대한 빅 데이터를 분석함으로서 지능적으로 인간에게 이로운
          편의를 제공하는 것이라고 정의 할 수 있다. 물론 이 교재에서 정의한 사물 인터넷에 대한
          정의가 절대적인 것은 아니다. 지금 이 순간에도 사물인터넷은 변화하고 발전하고 있기
          때문에 새로운 요구사항과 기술로 변경될 수도 있다. 하지만 가장 중요한 것은 이러한
          기술 발전은 인간에게 편리함과 혜택을 주는 방향으로 발전해야 한다는 것이다．
           사물인터넷이란 용어를 처음 사용한 것은 1998년 P&G에서 브랜드 매니저로 일하던
          케빈 에쉬튼이다. 그는 "RFID 및 센서가 사물에 탑재된 사물인터넷이 구축될 것"이라고
          언급하면서 이 용어를 사용했다．



    264 I 제］4장 사물인터넷이란7
    필자가 고둥학교 시절 교과서에서 21세기는 정보화 사회라는 내용의 공부를 한 것이
기억이 난다. 그때 선생님께서는 21세기에는 정보화 시대가 될 것이고 정보화 시대에는
정보 그 자체가 부가가치가 되며．정보를 사고파는 시대가 될 것이라고 하셨다. 그때는
선생님께서 하신 말씀이 무슨 내용인지를 제대로 이해가 되지 않았고, 그냥 시험에 나올
수도 있으니 머리에 암기하느라고 바빴는데, 지금에 와서야 몸으로 체험을 하고 있는 것
같다. 그때가 1990년이었으니까 그로부터 24년이라는 시간이 지났고 지금은 유비쿼터스
시대를 지나 사물인터넷(JOT - Internet of Things) 시대를 맞이하고 있다．



         Ubiquitous            M2M               Cloud Big Data




     i
           /}
                                     요
    目
                      卜              요
                                                     客P
                                                          :,   .   . ．   毖


                      ［그림 ]4-1] 사물인터넷의 기본 개념］




    유비쿼터스（Ubiqu汰치하는 라틴어 뇨bique를 어원으로 하는 영어의 형용사로 동시에 어디에나
    존재하는，편재하는1 이라는 사전적 의미를 가지고 있다. 즉, 시간과 장소에 구애받지 않고 언제나
    정보통신망에 접속하여 다앙한 정보통신서비스를 활용할 수 있는 환경을 의미한다. 또한, 여러
    기기나 사물에 컴퓨터와 청보통신기술을 통합하여 언제 ，어디서나 사용자와 커뮤니케이션 할
    수 있도록 하1 주는 환경으로써 유비쿼터스 네트워킹 기술을 전제로 구현된다. 사용자가 녜트워크
    나 컴퓨터를 의식하지 않고 장소에 상관없이 자유롭게 네트워크에 접속할 수 있는 정보통신
    환경이다. - wikipedia 참조
\




                                           14.] 사물인터넷이란 무엇인가? I 265
  + Arduino .




      M2M(Machine to M配hine）은 사물인터넷 용어와 혼용되어 사용되기도 하고 유사한 면도 있지
      만 엄밀히 말해서 M2M은 기계와r기계간의 통신을 이야기 하며 사물인터넷의 지능형 통신 서비스
      보다는 그 범위가 좁은 사물인터넷의 하위의 개념이라고 생각하면 된다. 入42M 서비스의 예를
      들어보면 고속도로 하이패스 시스템 , 수도, 가스 사용량 원격검침, 버스 정류장에 있는 버스
      도착 알림 서비스 등이 있다．




      14.2       사물인터넷 주요 서비스


      사물인터넷을 이용한 주요 서비스에 대해서 구체적으로 알아보자. 이번 절의 대부분
   내용은 2014.5월에 미래창조과학부에서 발표한 "사물인터넷 기본계획 "의 내용을 참조하여
   작성하였다．


   개인 loT - 사용자 중심의 편리하고 쾌적한 삶

                        ［표 ]4-11!    2014.5월 미래창조과학부 발표자료］

         Car as a service           Hea出）care as a service     Home as a SE rvice




                              심장박동, 운동량 정보 제공                주거환경 loT 통합 제어


     안전하고 편리한 운전              개인 건강 증진                       생활 편의, 안전성 제고

     米 긴급구난 자동전송, 무인           ;k 심장박동 케어, 건강 팔찌             米 가전 · 기기 원격제어，
       자율 주행 서비스 등                케어 서비스 등                     홈 ccliv 서비스 등




266 I 제］4장 사물인터넷이란？
                                                                             社


산업 loT m 생산성 · 효율성 향상 및 신 부가7 F天1창출


                     ［표 ]4-2]    2014.5월 미래창조과학부 발표자료

    Fact가-y as a Ser爪冶          Farm(&Food) as a Ser月ce     Pr刈uct as a Service




 공정분석 및 시설물 모니터링                생산 · 가공 유통 JoT 접목         주변 생활제품의 JoT 접목
 작업 효율 및 안전 제고                생산성향상 및 안전유통체계              고부가 서비스 제품화
 米 제조설비 실시간 니터링，                米 스마트 팜 · 축사 · 양식장，       米 식습관관리 포크, 심장
   위험물 감지 · 경보 서비스                식품 생산유통이력 정보              박동음 전달 베게, 행동
                                  제공 서비스 둥                  패턴 분석 신발 등




공공（도시） loT - 살기 좋고 안전한 사회 실현


                     ［표 ]4놔3]    2014.5월 미래창조과학부 발표자료

 다Jblic Safety as a Service     En＼月ronment as a Ser水：e    Energy as a Service




          관제셴터
 疋냥
斗난지에＼느七
           m叩   尸   쓰레기쭈키
          쭈쩍차目4



cclv, 노약자 GPS 등               대기질, 쓰레기양 둥                 에너지 관련 JoT 정보 제공
JoT 정보 제공                     JoT 정보 제공

재난 · 재해 예방                    환경오염 최소호F                   에너지 관리 효율성 증대
米 어린이／노인 안심이，                 米 스마트 환경정보 제공, 스            ;K 스마트 건물에너지 관리，
  재난재해 예보 서비스 둥                 마트 쓰레기통 서비스 둥                스마트미터 , 스마트 플러
                                                             그 서비스 등




                                                          142 사물인터넷 주요 서비스 I 267
 .   Arduino



      이렇듯 사물인터넷의 범위는 작게는 개인 서비스에서 크게는 도시 사물인터넷 , 국가
     사물 인터넷으로 그 범위는 확장될 수 있으며 미래에는 국가를 넘어선 전 세계가 사물인터
     넷으로 연결되는 그런 날이 올지도 모르겠다. 참고로 현재 여러 문헌과 자료에 따르면
     개인 서비스를 위한 사물인터넷 서비스 중에서도 헬스케어 제품이 가장먼저 사물인터넷의
     물꼬를 틀것으로 예측을 하고 있다. 현재에도 여러 웨어러블 기기와 스마트 디바이스들이
     심박수 측정과 혈당측정, 운동량 측정 등의 기능을 장착하여 이미 출시되어 있고 천 세계의
     글로벌 기업들이 이 분야에서 가장 많은 기기들을 출시하고 있다．




      14.3     주요 loT 제품 및 서비스 동향


      이렇게 설명을 해도 아직 사물인터넷이 무엇인지 개념이 정확히 잡히지 않을 수 있다．
     현재 이미 출시되어 있는 주요 사물 인터넷 서비스와 제품을 조사해 봄으로서 조금 더
     구체적으로 사물인터넷에 대해서 알아보자. 이 자료 또한 2014.5월에 미래창조과학부에서
     발표한 "사물인터넷 기본계획 "의 내용을 참조하였다．


                      ［표 14-4]       2014.5월 미래창조과학부 발표자료

                                     무선 실시간 혈압 모니터링
                                     - 제조사 : 미국, iHealth Lab
                                       블루투스를 통해 스마트폰 앱과 연동되어 실시간으로
                                       혈압을 모니터링




                                     해피포크（HA듸幻rk)
                                     - 제조사 : 홍콩， HapiLabs
                 HAPifork              음식 투입속도 및 포크 이용 횟수 둥 측정
                      E壯北wly.        - 사용자가 음식을 먹는 1기1 투입하는 속도와 포크질 횟수
                     Lose weight
                      Fe이 great! "     둥을 측정해1 다이어트에 필요한 식습관을 제안할 수
                     m                 있음
                                     - 측정된 기록은 블루투스를 이용해 스마트폰이나 컴퓨터로
                                       바로 동기화할 수 있음．




2681 제］4장 사물인터넷이란2
                  유린케어（UrinC可e)
                  - 제조사 : 한국, 아이티헬스
                  1 스마트폰 기반의 대 . 소변 관리시스템
                  - 스마트폰 기반의 대소변 관리 시스템， 乃gBee 기반의
                    센서를 내장한 기저귀와 감지시스템으로 구성
                    스스로 대소변을 처리하기 힘든 고령층 및 환자가
                    대소변시보호자 혹은 요양사에게 자동으로 정보를 전송

                  커넥티드 자전거
                  - 제조사 : 한국 삼성
                    자전거 주행속도, 운행거리 및 자신의 운동량 등 파악
                  - 미국의 자전거 제조업체 트렉（Trek）사와 협업해 갤럭시
                    노트3와 연동된 '커넥티드 자전거' 를 개발
                    자전거에 설치된 센서가 실시간으로 주행 속도, 운행 거리
                    등을 측정하여 자전거는 핸들 중앙에 거치되어 있는 스마트
                    폰으로 자신의 운동량이나 주행 거리 등을 파악

                  에이스캔（A田can)
                  - 제조사 : 한국, 에이스앤
                  - 입김만으로 알코올 농도 파악
                  - 사용자의 입김 속 알코올 농도를 측정 관리할 수 있음
                    앱으로 다양한 음주 및 건강에 대한 유익한 정보를 받을
                    수 있으며 , 사용자에게 음주운전 위험성을 담은 메시지를
                    지속적으로 알려주는 등 음주운전 예방에 도움



 현재 상용화 되어 있는 제품들의 특징은 특정 디바이스에 의존적이라는 것이다. 바로
스마트폰이다. 아직까지는 각 사물（디바이스）들이 지능적으로 서로 유기적으로 통신을
하여 맞춤형 서비스를 제공한다기보다는 스마트디바이스 기기들이 사람들이 공통적으로
가지고 있는 스마트폰 기기에 데이터를 집중시키고 사람들은 스마트폰을 이용해서 정보를
소비하고 있다. 이러한 것들은 진정한 의미의 사물 인터넷시대는 아직 아니고 유비쿼터스，
入42M에서 사물 인티넷 시대로 가고 있는 중간 과정이라고 할 수 있다.




                                  14.3 주요 loT 제품 및 서비스 동향 I 269
  .   Arduino




       14.4 (,   주요 loT 구성요소 및 현황


       사물 인티넷을 구현되기 위해서 반드시 필요한 구성요소와 각 구성요소들의 현재 현황을
      알아보자．


                       ［표 ]4-51 2014.5월 미래창조과학부 발표자료

        구성요소                            현 황

                 1 （공공） 다양한 시범사업을 추진하였으나, 개발 · 운영비용 부담 등으로 확산 저조
                 1 （산업） 대기업 중심으로 도입 , 중소기업은 비용문제로 도입 저조
      서비스（S)
                 . （개인） 웨어러블, 가전, 자동차 둥은 글로벌 기업 간 경쟁 중 중소기업은 다양한
                    생활제품 응용분야에 진출 노력 중

                 1 국내 대기업은 플랫폼을 개발 중이나, 글로벌 시장 주도력 부족
      플랫폼（P)
                 1 국내 중소기업은 플랫폼 부재로 시장진입 어렵고, 글로벌 기업에 종속우려

                 . 급증하는 트래픽을 S＼刃로 유연하게 처리하는 기술개발 중
      네트워크（N)    S 원격지 사물 연결을 위한 저전력 장거리 비면허 대역 통신요구 증대
                 15G, （코ga인터넷, IPv6 등 사물인터넷 활성화를 위한 인프라 개발·구축 중

                 S 스마트폰 이후 글로벌 기업 중심으로 실감찌능융합형 디바이스 개발 경쟁 중
      디바이스（D)
                 S 웨어러블 디바이스, 스마트센서 등을 중심으로 시장 확대1 전망

                 5 loT 서비스（흠가전, 의료 등） 보안 침해사고 사례가 나타남에 따라 보안 대책
      보안（Se)       논의를 시작하는 단계
                 S 설계단계부터 보안, 프라이버시 등을 고려한 기술 및 서비스 개발 필요



       필자의 생각에 사물인터넷을 구현하기 위한 필수 요소들이 여러 가지가 있지만 그중에서
      도 플랫폼과 보안 분야를 이끌어가는 사업자 혹은 국가가 앞으로 다가올 사물인터넷의
      중심에 설 것으로 예상이 된다. 이런 추측을 하는 이유는 현재 가장 이슈 사업인 스마트폰
      사업을 예로 들어보자. 전 세계에서 가장 많은 스마트폰을 생산하고 판매하는 사업자는
      한국의 삼성전자 이지만 가장 큰 시장을 점유하고 이익을 얻어가고 있는 사업자는 구글과
      애플 이다. 그 중에서도 구글은 제품 생산을 하지 않으면서도 안드로이드 Os 플랫폼을
      제공하고 많은 스마트폰 제조사들이 안드로이드 플랫폼을 기반으로 제품을 개발한다. 구글
      은 이러한 안드로이드 플랫폼 생태계를 조성해 놓고 수백만N수천만에 달하는 안드로이드
      앱 마켓의 광고이익과 안드로이드 앱（App) 매출이익을 가져가고 있다. 최근에는 스마트폰
      플랫폼 뿐만이 아니라 웨어러블기기, l\ /, 자동차, 엔터테인먼트 플랫폼까지 장악하기 위해


270 I 저114장 사물인터넷이란9


                                                        1
서 새로운 버 전의 안드로이드를 지속적으로 발표하고 있다. 이러한 전례를 볼 때 사물인터
넷 시대에서도 플랫폼을 장악하는 업체가 사물인터넷 시대를 이끌어 갈것으로 예상이 된
다．
丑m 가전, IT 기업들의 사물인터넷 플랫폼 주도 현황
     아직까지는 특정 업체가 사물인터넷 플랫폼을 주도하지는 못하고 운영체제 , 디바이스，
           스마트 홈, 네트워크 서비스, 보안 등 각각의 분야에서 독자적으로 혹은 연합을
통해서 플랫폼을 만들어 가고 있는 중이다．


                              ［표 14-6]

      기 업                         플랫폼 주도 현황

               . 삼성전자는 주로 자사의 생활가전제품과 스마트폰 등을 이용해서 사물인터넷
                 서비스를 준비하고 있는 것 같다．
      삼성전자     1 음성인식을 통한 냉장고, 에어컨, 스마트TV, 스마트폰, 태블릿 PC, 갤럭시 기어
      LG전자       등의 기기들을 하나의 플랫폼을 이용하여 제어하도록 하고 있다．
               1LG전자는 현재 삼성전자의 음성인식과는 다르게 "홈챗（HomeChat)" 이라는 메신
                 저를 통해서 유사한 서비스를 제공하려 하고 있다．

               1 인텔은 세계 최대의 CPU제조 벤더답게 사물인터넷 환경에 최적화된 네트워크와
                 의 연결 및 정보 수집을 위해서 하드웨어 플랫폼을 준비하고 있다．
       인텔      S 2014년 CES 2014에서 초소형 x86 컴퓨터인 "에디슨" 을 발표였다．
               1SD카드의 크기에 프로세서와 내장 그래픽카드, 무선랜, 블루투스 모듈까지 전부
                 갖추었다．

               1 가전 업계들과 개발자들을 자사의 플랫폼 "올조인（A可아n)" 에 끌어들이기 위해1
                 서 노력
               1 올조인 : 운영체제나 하드웨어에 상관없이 기기간 연결 플랫폼
               1 각기 다른 제조사에서 만들어진 조명 , 스마트워치, 가전기기등을 올조인이라는
      퀄컴 1
                 허브를 통해서 연결되고 소통하는 것을 지향하고 있다．
               S 퀄컴은 "올씬얼라이언스" 라는 이름의 사물인터넷 컨소시엄도 주도하고 있다．
               S 올씬올라이언스 주요 회원사로는 퀄컴을 비롯해 하이얼, LG전자, 파나소닉，샤프，
                 실리콘이미지 , 티피링크 등이 있다．

               1iOS7 발표와 함께 아이비콘(iBeacons）이라는 기능을 선보였다．
       11플
       0       S 아이비콘 : BI上를 기반으로 하고 10cm 미만의 NI了C 기술을 대체 아이비콘의
                 장점은 신호의 감지 거리가 최소 5cm에서 최대 49m


                                     14.5 가전, ri- 기업들의 사물인터넷 플랫폼 주도 현황 1 2 1
    Ard네no




               1 애플은 아이비콘 기술을 기반으로 하는 아이홈（ii如me）이라는 서비스를 통해
                 스마트홈 시장에 진출하여 "사물인터넷" 시대를 이끌어가기 위한 준비를 하고
                 있다．

                S 구글은 안드로이드라는 강력한（万 플랫폼을 기반으로 스마트폰과 태블릿， 최근어i
                  는 웨어러블기기를 넘어서 생활가전 플랫폼까지 안드로이드 플랫폼을 제공하려
                  는 움직임을 보이고 있다．
        구글
                S 사물인터넷 관련 디바이스 제조, 생산업체인 네스트를 3조 2천억원에 매입을
                  통해서 구글이 가지고 있는 막강한 3므뜨i웨어 플랫폼과 현금을 무기로 사물인터
                  넷 분야를 선도하려 하고 있다．



     최근의 추세를 보면 생활가전 등의 제조 기반의 사업자는 자사의 기기들（TV, 냉장고，
   에어컨 등） 간의 수직적인 하드웨어와 소프트웨어 인터페이스를 도입함으로서 사물인터넷
   을 선점하려 하고 있고, 소프트웨어를 기반으로 하고 있는 사업자는 제조사에 상관없이
   가전기기와 스마트 디바이스들을 연동할 수 있는 플랫폼 개발에 주력하고 있는 것 같다．
   그렇다고 제조 기반의 사업자들이 자사의 기기들끼리만 연동하는데 그치지는 않고 플랫폼
   개발 사업자들과 컨소시엄을 통해서 자사의 기기들을 표준 플랫폼에 연동하려는 움직임도
   병행하고 있다. 어쨌든 현채는 어느 한 사업자가 사물인티넷을 주도하고 있지는 못하고
   있고 다양한 사업자들이 사물인티넷 표준 플랫폼을 만들어 가고 있는 춘추전국시태타 할
   수 있다．
     지금까지 사물인터넷의 개념과 분야, 그리고 주력 사업자들의 동향에 대해서 살펴보았
   다. 앞으로 이 교채에서는 다루고자 하는 내용은 사물인티넷 분야 중에서 스마트홈 시스템
   구현에 대해서 간단하지만 구체적인 예제를 통해서 이해를 돕고자 한다. 헬스케어 분야와
   스마트홈 시스템이 사물인터넷 분야 중에서도 가장먼저 발전할 것으로 예상이 되고 현재에
   도 스마트폰과 연동하여 구현되는 사례가 가장 많기도 하다.




272 I 제］4장 사물인터넷이란7


                                                    1
         스마트홈

15. ]   스마트홈 서비스 개요
15.2 스마트홈 서비스 종류
.   Arduir刃 e




     15.1       스마트홈 서비스 개요


     스口냔i홈이란 무엇일까7 개념을 설명하기보다는 구체척인 예를 들어 보자. 가령 퇴근
    이후 스마트폰이나 스마트카드를 들고 현관에 접근하면 스마트 도어록이 자동으로 열리고
    현관에 설치된 체중계와 화장실 변기에 소변분석기가 부착돼 당뇨, 고혈압 등 만성질환을
    자가 진단하고 그 정보는 인터넷 망을 통해서 연계된 병원으로 자동 전달돼 관리된다．
    또, 집 밖에서 원격으로 미리 집 안의 가전기기 및 조명, 난방 등을 조절할 수 있고 전력，
    수도, 가스 등 에너지 사용량을 실시간으로 체크해 그 자리에서 사용요금을 파악하기도
    하고 침입탐지 시스템 등에 의해서 범죄예방 서비스도 가능하다．




      15.2      스마트홈 서비스 종류


     가정 내에서 가능한 서비스의 종류와 내용을 간단하게 요약하여 보았다. 이 교재에서도
    여기서 요약된 서비스들을 위주로 아두이노와 안드로이드를 이용해서 실제로 구현해 나갈
    것이다．


                               ［표 ]5-1]

        서비스 종류                        서비스 내용

                   sTy, 냉장고， 에어컨, 가스 등의 가전 기기들을 외부에서 스마트폰，태블릿
                     등의 디바이스를 이용해서 원격으로 제어가 가능하다．
                   1 실내에서는 음성명령, 문자 채팅 둥으로 대화를 통해서 원격제어하거나 거주
     생활가전            자의 행동패턴을 분석하여 거주자가 원하는 내용을 미리 파악하여 자동으로
                     서비스를 한다．
                   S Jp 카메라를 이용하여 원격지에서도 집안을 모니터링 할 수 있고 침입탐지
                     등에도 활용할 수 있다．

                   S 온도／습도／먼지／환경오염 센서 등을 활용하여 실내의 공기의 질을 실시간으
     실내 환경 모니터링
                     로 스마트 디바이스로 보여준다. 물론 원격지에서도 모니터링이 가눙하다．

                   S 인체감지 센서와 'P카메라, 소음 센서, 화재 감지 센서 등을 활용하여 외부
                     침입, 화재 여부를 알려준다．
     방범 시스템
                   . 귀중품에 RFII) 둥을 활용하여 도난（위치이동） 발생시 자동으로 알람을 해준
                    다．
274 I 제］5장 스마트홈


                                                      J
           S 현관에 설치된 스마트 체중계를 통해서 자동으로 체중 변화를 스마트 디바이
 홈 케어        스에 전송한다．
           S 소변기에 설치된 소변 분선기를 통해서 기본 건강 상태를 체크

 에너지 관리    S 전력, 수도, 가스 등 에너지 사용량을 실시간으로 체크




 위에서 나열한 모든 시스템을 전부 구현하기는 어렵지만 가능하면 많은 내용을 실험하고
구현하려고 노력하였다. 그리고 아직 스마트홈 서비스를 구현 하는데 중추적인 허브 역할
을 할 기기가 정해지지는 않았지만, 집안에 항상 위치하고 있어야 하고 24시간 항상 천원과
네트워크가 연결 되어 있어야 한다. 이 조컨을 만족시킬만한 기기로는 냉장고, TV 셋톱박
스, 인터넷 공유기 등이 있을 수 있다．
 이 교재에서는 지면 관계상 구체적인 구현 방법에 대한 내용을 싣지는 못하였고 사물인
터넷의 개념과 사물 인터넷 분야 중에서도 가장 먼저 다가올 스마트홈에 대해서 정리를
하였다. 사물인터넷 스마트홈에 대한 모튼 자세하고 구체적인 구현 내용은 2015년 중반에
출간 예정인 "아두이노 안드로이드 기반 사물인터넷 . 스마트 홈" 교재를 기다려 주기
바란다．




                                     15.2 스마트홈 서비스 종류 I 275
부록 및 색인
  .   Ardi.川기0         e




      이 교재에서 사용한 모든 부품 리스트

          미니 브래＝부＝                             아두이노 UNO R3                                                    LED 세트              저항 세트




                                                                                                                   卄I
                                               S 1        ,

                                           1             「 .;GX可m뇨 U


                                               雲   三
       ::::: ::::: ::::: ::::: :::::
                                                         a.                                      1
                                       ,            Sm                        ; ；』；   ;;;;;;.;




          부품들을 연결해서                        아두이노를 배우는더］ 가장                                            REt기 W1끄TB, BLUE,
                                                                                                                            각종 저항 키트 모음
           실험하는데 사용                          인기 있는 보드                                                  YELLO町 4개씩

      嚼枷立7 Segment                                       푸시 버튼                                                수동 부저               트랜지스터




              『： 뇨日，
          Common Cathode
                                                         M 中 m                                       부저 테스트 시 사용
                                                                                                                                   I
                                                                                                                                  S8050 NPN
                                                         4pmn Type

                 가변저항                              Character LCD                                        시리얼 LCD                   조도센서




              I  가변저항
                                           16 x 1 줄을 가지고 있는
                                                4hit, 8bit LCD
                                                                                                     戶
                                                                                                     16 x 2 줄을 가지고 있는
                                                                                                         Character LCD
                                                                                                                                    圃1
                                                                                                                             주변 밝7 어］ 따라서
                                                                                                                            저항 값이 바뀌는 센서

             온습도 센서                                화염김仄1 센서                                             기울71 센서               즈.1豁지 센서「聲弓群

                           S
                                                          5 en 三 그 H 느
                                               G                                                                             ct                    叫

                                                                                                                        多
                                                                 m       戶H




                                                          e      =       =                              ".s   ',   二’
                                                                                                                                         小   =     =
                                               C                     是毛                                                      口                   A뇨
                                                                                                                                                  二d




                       i 重i 玉
        DHT11 온도와 습도를                          화염의 파장을 인식하여                                            S＼肌520D 기울기          S＼甲－18020P 진동감지
         하나의 센서로 측정                               화재 감지                                                   감지센서                           센서




278 I 부록
   초음파 센서                           DC모터                     모터저뻐 IC                     다이오드




                                                                                        II
         꾼
         m心
             4
                    O                                          므； 쓰 :=   ;=   윽
                                                               L293B
             晏口 自




 HC-SR04 초음파센서                                                 L293B                      1N4003로
                      기어박스가 있는 DC모터
  거리를 감지 가능                                                 DC 모터제어 IC                  모터제어에 人｝용

    서보 모터                      모터제어 IC                       스테핑 모터                     자이로 센서




二
                                                                                          L크G 나 근口口D
                                                                                    e GND      x   INT 牡
                        Il_     LI      I     I   I   I
                                                                                      SDA     yZ    DR    仕
                                                                                    1   SCL         CS    朴
                              U I   I   I   U U I     U
                                                                                    心 vCC          S王）0




                           L293D                             kh42hm2-901              L3G4200D
0 싸 180도까지 회전 가능
                        스테핑 모터제어 IC                         2상 스테핑 모터               xYz 회전각 측정

  적외선 수신기               Character LCD                     XBee USB Adapter               XBee 모듈




      系
     37.9KHz
 CH0B or KSM603LM
                                 37.9K1七
                              CL-1L5 JR LED
                                                             Ffl끄 USB
                                                           시리얻 컨버터 내장
                                                                                   XBP24-DMWJT-2S0J


 USB 미니 케이블                   XBee Shield                 USB A-B 케0 블                  블루투스 모듈




力
XBee USB Adapter91-   아두이노 UNO R3에                        아두이노 UNO R3와
                                                                                  HC-06 시리얼 통신 가눙
PC를 연결하는더］ 사용         적층해써 사용 가눙                            PC를 연결




                                                                                                    부록 I 279
 -. Arduino 1




       Ethernet Shield     점프 케0        田45 인터넷 케이블




      아두이노 UNO R3와       브레드보드와 부품들올
                                        Ethernet Shie넌와 사용
       적층해서 사용             연결하는데 사용




                         이 교재에서 사용한 모든 부품들은


                           http: //www deviceshop.net


   온라인 쇼핑몰을 통해서 개별로 구매하거나 키트로 구매하실 수 있습니다．




280 I 부록
                      찾아보기



                                              B

4 Band Register        35   미uetoo仕1                   238
4-bit 모드              108   Buzzer                      69




5 Band Register        36   Cathode                     53
                            CDS 조도센서                   122

                  7         CHOB                       199


7세그먼트                  53


                        出
                            DC 모터                      154
                        囊
                            Demodulation               198
8-bit 모드              113   DHTII                      126
                            digitaiRead                 66
                            小gital사Vrite                66
                  A

ADC                   97
analogWrite            86
Anode                  53   Ethernet                   248
Arduino               10    Ethernet Shield            248
AT 명령어                236
ATCN                  236
ATDH 명령어              236
All兀 명령어              236   HC-06                      239
AVR                   11    HC-SR04                    147
                            HD44780                    108



                                                  찾아보기 1 281
   I끄GH                 65    pitch              175
   H11P                 260   PNP                 94
   Hybrid               164   Pu血如wn              65
                              P珉小4                48




   I2C                  172
   IDE                   12   Register           110
   IEEE 802.15.1        238   可45                250
   IEEE 802.15.4        212   roll               175
   IEEE 802.3           248   R아or               164
   IRDA                 197   R5232               74
   IRremote             203
   ISM Band             212


                              SCL                174
                              SDA                174
   L293B                155   Serial              77
   L293D                165   SH                 231
   L3G4200D             174   SL                 231
   LAN                  248   Slave Select       182
   LCD                  107   SPI            172, 182
   TED                   36   SS                 182
   LO町                   65   SW-18020P          142
                              SW-520D            137




   MAC                  248
   入ITSO                182   Tilt               137
   MOST                 182   T血er                 48




   PANs                       U뇨asonic            146
   Pern그anent 八1agnet
   pinMode



282 I 찾아보기
Variable Reluctance       164   마이 긔르 3工 쿠서1서          12
Voltage                   102   모터                    153




                          216   부저                     69
                          214   브래드보드                  38
                          222   블루투스                  238
                                블루투스 프로파일             239

                      Y

yaw                       175
                                서보모터                  160

                      z         센서                    122
                                소프트웨어                  11
乃gbee                     212   스마트 폰                 239
                                스테핑 모터                163
                                슬레이브                  173
                                시리얼                    74
가변 릴럭턴스                   164   시리얼 LCD               117
거리 감지하기                   146   시리얼 모니터                77
공구                         41   시리얼포트                  27
근거리 무선 통신                 238
기어박스                      155
기울기 센서                    137
                                아날로그               96, 97

                      다         아노드                    53
                                안드로이드                239
단락 검사                      43   업로드                    26
디지털 출력                     48   영구자석                 164
디지털 통신                    172   온습도 센서               126
디지털 포트                     48   와이파이                 238
                                웹 서버                 255
                                웹 클라이언트          249, 255


                                                찾아보기 1 283
   이더넷        248


                     패러럴 LCD   108
                     펄스        86
   자이로 센서     174    페어링       245
   장치관리자    18, 75   풀다운        65
   저항          33    풀다운 저항     65
   저항 측정       46    플레이그라운드   129
   적외선        197
   전류          32
   전압          32
   전압 측청    44, 45   하드웨어
   전원공급        17    하이브리드
   전위          32    화염감지 센서
   전하          32    회전각
   점프 와이어       42   회전자
   주파수대별      147
   지그비         212
   진동 센서      142




   초음파센서      146




   캐소드          53
   컴파일          26




   테스터기         42
   통합개발환경       12
   트랜지스터        94




2841 찾아보기
                      저자와의
                     협의에 의해
                      인지 생략




  실험 지T와 함께하는 ARDUIN0 입문서

 아두이노 완전정복
       3판 2쇄1            2015년 9월 ]0일

 저 자     김경연 / 장정형 / 박민상
 발행인     송광헌
 발행처     복두츨판사
 주 소     서울특별시 영둥포구 경인로82길 3-4
         센터플러스 807호
         （우） 07371
 전 화     02-216卜2580
 FAX     02-2164-2584
 등 록     1993. 11. 22. 제 10-902 호


                          정가 : 19,000원
                ISBN : 979-11-86333-14-3 93560

 小
(m片 힌국과학기'I판협회 회원사

 불법복사는 지적재산을 훔치는 범죄행위입니다（저작권법 제97조 5항）
1   玉卜：
     ？   「   1
About JK Electronics
－산업용. 교육용 Embedded 개발보드 깨빨 및 교육
-Arc!uino 공식 한국 디스트리뷰터
-Arduino 호환 Kordulno 깨빨
-FDM 방식 3D프린터 개빨 및 제조




                       ARDUINO
                           yduiflO 15 郁）（均en-的내te 叫CC恤抑CS
                          口mk乂yryna 아計orm besed On！陀川b地．
                                                                     ATMEGA2560 Rabbit 개벋보드 시리즈
     아두이노 100% 호환          easy너O小use hardw酊a and s（月te酊C.
                             1t'a 1ntended 的r ar姑摠. 小CS自1衿rS.          ATMEI. 스IVEGA斗8C 기반Pi8b11 개밟보도
      made in korea    !x,bbysts. and anvn크 甘lterested er c1eat,ny       온도신,1& Soc입러．r,RF241J몌 F下．
     by JK E陀C打on妃S        In妃cC데Va Ob忙Cts O1 CfW卄O1111祀11요                TFr 比O, VSI0O招 ups 듐
                                                                         다앙 + 모늄늅읔 면깁하여 네스트 가늉




                                                                                      夕
                                                                          J卜（듸ectr이lics
                                                                          (http:/Iwww.jkelec.co.kr)




                                                                                                        1
ARD네NO                                            by JK 티ec杆onics

                                                                                        母쿄斗 ＝   짙多mne斗可｛




I 제품소개1
                                                                                          · A1兀乂JNO Kit는 아두이노를 차음 시작하는 분들을 위한 사입니다．
                                                                                          · 구성품은 솨duino Urn R3 보드를 7뵨으로 개발자들이 가장 많
                                                                                                0I 사용하는 디지털, 아날로그 센서 및 7서1그먼트， 匡D, 저항, 서
                                                                                                미스E寸 등이 포함되어 있습니다．
                                                                                          ·Kit 구성품이 就田1 가지 않도록 단단한 플라스틱 케이스로 패키
                                                                                                天를 구성했습니다．
                                                                                          · 케이스는 킨막이로 나뉘어져 부품들의 보괸이 용｛기합니다．
                                                                                          · 워크샵이나 킥종 교육용 교재로 사용하기 적합하며 초보 엔지니어
                                                                                                를 위한 실험 사로도 손색이 없습니다．


I제품구성
                                                                                                           ] . 솨d내no Un) 田 - 1711
      11
                                                             享         2
                                                                            dmD ]                          2. 브러드 보드 - 1711
                                                                                                           a ［月B 다운로드 케0블 - 1711
                                            U I              U I
                           4                                           5           小1            6         4. 匹D(RED, 臣LE, （쿳：?EEN. 'y'日LOW. \／버旺） 각 4개씩
                                                                                                           5. 트랜자스터 38550. 38050 - 각 2개씩

                河          7
                                                  1i!
                                                        ,,             8             日 9
                                                                                  日．B：                     6. 가변저항 ]0K- VH
                                                                                                           7. 화이트 & 블루 가변저항 j（米 - 1711
                                                                                                           8. 저항 ]K. ]（米， 10(米 ]00. 47어ohm) - 각 20개씩
                       b0
                                                  I斗，                              目日           12         9. 7서口먼트 - 17fl
                                                                                                           10. 수동부저 - 17fl
            S
      世                13                     :t                       14   H15
                                                                                                           ]] . 조도센人I - 1)fl
                                                                                                           12. 기울기센서 - iifl
                                                                                                           13. 12半］2 Tact스위치, 스위치 캡 ］개
  -                    16               q1                         17             I口1           18         14. 6坮 Tact스위치, 스위치 캡 寸 4개


                                                                             싸
                                                                                                           15. 점퍼 와이어（약 ]8cm) 卞 20개
                       19                                          20                                      16. 적외선 원격제어수신기 - 17fl
                                                                                                21
                                                             1/



                                                                                                           17. 화염감지 센)寸 - 1711
      h22
                                            匯蠶 23                                               24         18. 진통감지 센서 - 1711
                                                                                                           19. 온도감지 서미스터 - 1)fl
                                                                                                           20. 기어박스가 있는 DC모터 - 1711
                                                                                                           21. 서보 모터 (SG90 的） - 1711
                                                                                                           22. DC 모터제어 IC 仁93B) - 1711
                                                                                                           23. 적외선 리모컨 中 l가1
                                                                                                           24. Character LCD (16거) - 1711




                    byJ" "芦的凸‘" ,/ 呻11回                            0
                    （스．}            ;         OO                                                                         Arduino K나 구입처 안내
                八
                니
                                \       )
                                                                                                                         ·복두마트 w뺀Lbdmart.kr
                           ／入                C)              fl
                                                                                                                         ·JK전자 ww너／.ikelec.co.kr
                                                                             I
/   m




                                                                                                                                    뵤咀卄茗何蓉8旨出
                                                          \m\
                                                                노＼

                                                                     \




                                                                                                   \
             /                                                                                         \                        \
                                                                                                               \        1
                                                                         /                                                      느




                                                                                                                                日




                                                                                                                                1
                                                                                                                            1
                                                                                                           /




                      N
                              N
                                  N
                                               아두이노
                                                         완전정복                                                      \b




    /
        //
                 1/
                          /
                                  尸／
                                                        Chc｝아er ] . 아두이노 소개1
                                                        Ch야) ter 2, 전기 , 전자의 기초
                                                                                                   I
                                                        Ch야)ter 3 , 디지털 입력과 출력
                                                        Chapter 4, 시리얼（RS232) 통신
                                                        Char乂er 5 , 아날로그 입력과 출력
                                                        Ch야)ter 6. LCD 사용하기
                                                        Chapter 7, 실제 세계와의 통로 센서
                                                        Ch야)ter 8, 모터 제어하기
                                                        Ch야)ter 9 . 디지털 통신 인터퍼四1스
                                                        Ch야六er 10 . 적외선(IRDA) 통신
                                                        Chapter 11. 지그비（Zigbee) 네트워킹
                                                        Chapter 12 블루투스 통신
                                                        Cha口ter 13 . 이더넷（Ethernet) 네트워킹
                                                        Chapter 14. 사물 인터넷이란7
                                                        Chapter 15 , 스마트 홈




                              http://www.bogdoo.co.kr

                              日OG900


                              본 도서의 자료 업데이트가 있을 경우 본사 홈페이지 자료실에
                              업로드 됩니다. 정기적으로 들러서 유익한 자료를 받아가시기                   9 791,]:::，나161
                              바랍니다．                                                  ISBN 979너卜86333- 4-3

