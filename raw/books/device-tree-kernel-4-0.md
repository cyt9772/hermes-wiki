---
source_url: /run/media/yutae/Data/Device Tree.pdf  # USB PDF (local-only; raw/books/device-tree-kernel-4-0.pdf gitignored)
ingested: 2026-11-01
sha256: 0df4dd2c2a73d7fce16f74732ceed8bce35dbcba499da7e81e783598fc527af9
---

# 디바이스 트리 상세 분석 in Linux Kernel 4.0 (raw source)

## Book metadata
- **Title:** 디바이스 트리 상세 분석 in Linux Kernel 4.0
- **Original:** (자작, 한국 원서)
- **Authors:** 정재준 지음
- **Korean publisher:** 커널연구회(발행인 정재춘)
- **ISBN (KR):** 978-89-97750-06-1
- **Year:** 2015
- **Pages:** 314 (pdfinfo)
- **kind:** text-layer (pdftotext extraction 2026-10-30)

## Body
         First Edition




Device Tree
상세분석 in Linux Kernel 4.0

                          정재준지음




       roo+..      겅렁젝l
                            커널연구회
                            www . kernel. bz
in Linux Kernel 4.0
        First Edition




        구회（叫iw.kernel.b기
   苔茗   rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                        저작권




저작권
Device Tree 상세분석 in Linux Kernel 4.0
저자 정재준


Copyright @ 2012-2015 커널연구회佃,ww.kernel.bz). All rights reserved.
Published by 커널연구회(I사니,w.kernel.b기．
서울 금천구 두산로 70 현대지식산업센터 A동 26층 261］호


커널연구회는 리눅스 커 널과 자료구조 알고리즘을 연구하고 리눅스 시스템 프로그래밍                                    및
디바이스드라이버 개발을 통하여 창의적인 프로젝트를 수행하여 幻T 관련 제품들을 만들어 일상
생활을 풍요롭고 편리하게 하는데 가치를 두고 있습니다.                         아울러 관련 기술들을 교육하여
여러사람들과 공유할 수 있도록 노력하고 있습니다.                       커 널연구회가 연구 개발한 결과물들은
체계적으로 문서화하여            온라인（www.kernel.bz）상에서     무료 혹은 유료로         제공하고    있습니다．
커널연구회가 제공하는 저작물에는 저작권을 표시하고 있으며 사용자는 저작권 표시를 보존하1
주어야 합니다.       커널연구회가 유료로 제공하는 저작물은 사용자에게 개인키（암호）를 부여 하므로
개인키를 타인에게 공개 및 양도하는 일이 없도록 해야 합니다．


기타 자세한 내용들은 커널연구회 웹사이트佃ww.kernel.b기를 방문해1 주시기 바랍니다．
감사합니다．




발행인： 정재춘
발행처： 커널연구회
출판사등록번호： 제2011-75호
출판사등록일：201］년 09월 27일
전화및팩스：031-594-5307
ISBN: 978-89-97750-06-1


초판발행일：2015년 08월 07일




                                       2 / 312
커 널 연구회（www.kern이幻z)                                        정쟤준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                              커널연구회 로드맵           3




커널연구회 로드맵

연구개발 및 교육

        시스템
      프로그래밍




        디바이스                                                                하드웨어 소프트 융합

        드라이버
                                                                            지능형 센서. 모터제어
                  出＝ mm   m心二 拙好 蜘   帥   明m 蜘   m出 甘喀；




         리눅스                                                                   자연어 학습
                                                          ARM Cortex-A
         커널
                                                             리눅스 커널 4.x      대화형 인터페이스

                                                           미g.LITTLE 스케쥴렇
        자료구조                                                멀티코어 병렬처라
        알고리즘                                             8+ Tree 자료구조 알고群肴．
                                                            네트워크 분산처리
                          mARM Cortex氓每

                                     온도. 습도
         C언어                 속도. 기울기. 경사
                                 도. 기압（고도）
                                     방향（나침반）
                                         거리
         ARM                             조도
        아키텍쳐




                    loT 데이터 수집기                          분산 병렬처리 시스템        머신 러닝      지능형 로봇




       제품 개발 프로젝트

                                                          3 / 312
커 널 연구회（www.kernel.bz)                                                      정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니nux Kernel 4.0                              커널연구회 교육과정         4




커널연구회 교육과정

                                                         환급
    1;
    在

    貫：            교육과정명          일수   시간         교육비                교육임시
                                                        （함인）
         三



                                                        일반인50%    매월 첫째주（월시목）
i            c언어와 자료구조 알고리즘      4일   32시간       88만원
                                                        대학생60%     09:00 N 18:00



                                                        일반인50%    매월 둘째주（월시목）
             리눅스 시스템 프로그래밍       4일   32시간       88만원
                                                        대학생60%     09:00 시 18:00



                                                        일반인50%    매월 세째주（월N목）
             AR卜A 아키텍쳐, 펌웨어 실습   4일   32시간       99만원
                                                        대학생60%     09:00 N 18:00



                                                        일반인50%    매월 넷째주（월N목）
4 리눅스 커 널 및 드라이버 실습              4일   32시 간      99만원
                                                        대학생60%     09:00 N 18:00



             出 모든 교육과정에 대하여 커널연구회에서 집필한 교재를 제공합니다．
             出 대학생은 모든 교육과정에 대하여 교육비 60% 할인해 드립니다．



弗 좀더 자세한 내용들은 커널연구회（www.kern쉬.bz) 웹사이트를 참조하세요．




                                       4 / 312
커널연구회（www.kern이b기                                         정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                 저자 소개1       5




저자 소II




정재준 (rgbi3307@nate.com) / 커널연구회（www.kernel.b기
저자는 학창시절 마이크로프로세서 제어 기술을 배웠으며 리눅스 커 널을 연구하고 있다． 15년
이상 쌓아온 실무 경험을 바탕으로 " C언어와 자료구조 알고리즘", " 리눅스 시스템 프로그래밍",
"리눅스 커 널과 디바이스드라이버 실습2",               " 오라클 실무활용 SQL튜닝2“등의       책을 집필하고，
월간임베디드월드 잡지에 다수의 글을 기고 하였다.                      또한 " 맞춤형 문장 자동 번역 시스템 및
이를 위한 데이터베이스 구축방법 (The System 幻rthe customized automatic sentence translation
and database construction method)" 라는 내용으로 프로그래밍을 하여 특허청에 특허출원 하였다.
최근에는 서울시 버스와 지하철 교통카드 요금결재 단말기에 들어가는 리눅스 커널과 디바이스
드라이버 개발 프로젝트를 성공적으로 수행했고 여러가지 임베디드 제품을 개발했다.                             저자는
스탠포드대학교의 幻hn L. Hennessy 교수의 저서 " Computer Organization and Design " 책을 읽고
깊은 감명을 받았으며, 컴퓨터구조와 자료구조 알고리즘 효율성 연구를 통한 기술서적 집필에
노력하고 있다.        저자는 온라인 상에서 커널연구회（http://＼사ww.kern이.bz/) 웹사이트를 운영하며
연구개발, 교육, 관련기술 공유 등을 위해 노력하고 있다．




+ 저자가 집필한 책들


                                       5 / 312
커 널 연구회 (www.kernel.bz)                                 정재준 (rgbi3307@nate.con가
Device Tree 상세분석 in Linux Kernel 4.0                          문서 표준       6




（목록단락）
Device 가ee 상세분석 in Linux Kernel 4.0
디rst Ed池on




문서 표준
1



（제목1)제＃장 대제목 맑은고딕 20 진하게

1.1 제목묶음

1.2제목묶음

1.3재목묶음


본문 내용（contents) 폰트는 맑은고딕 크기 ]0



（제목2)#.# 중제목 맑은고딕 16 진하게
본문 내용（contents) 폰트는 맑은고딕 크기 ]0



（캡션1)맑은고딕 14 진하게
본문 내용（contents) 폰트는 맑은고딕 크기 ]0


（캡션2）맑은고딕 ]2 진하게
본문 내용（contents) 폰트는 맑은고딕 크기 ]0


（캡션3）맑은고딕 11 진하게

본문 내용（contents) 폰트는 맑은고딕 크기 ]0


（캡션4）맑은고딕 10 진햐게

본문 내용（contents) 폰트는 맑은고딕 크기 10
（강한참조） 본문 내용（contents) 폰트는 맑은고딕 크7j 10
（약한참조） 본문 내용（CONTENTS) 폰트는 맑은고딕 크기 10




                                       6 / 312
커 널 연구회（ww以emn飢b기                                정재준 (rgb日307@nate.com)
Device Tree 상세분석 In 니nux Kerr倒 4.0                                                                           문서 표준              7




소스 코드 폰드는 돋움체 크기 9

    drivers/serial/8250.c                                 dr如ers/ser洲席尉通乞core.c                drive心加har/t口mk뇨C




    白＼
         seria18250 mnit
                                   \
                                           \\
                                                \,
                                                     \1
                                                            uart_register_dr iver
                                                                                    \
                                                            小                           ＼노
                                                                                                 tty_register_driver



위에서 타원형은 구조체를 나타내고 사각형은 함수를 의미한다.                                                       화살표 연결은 구조체와 함수간
의 데이터 흐름을 나타낸다．



소스를 상세1 설명하기 위한 태이붊
소스 코드 工            ;   1, 세   :/       r


함수원형          int uarLregistermdriver (struct uart_driver *drv)
  설명          uart core 계증에 드라이버 등록
매개변수         dry: 드라이버 구조체
소스파일         drivers/serial/serial_core.c
 구조체          struct uart driver                                                                                            1
              struct uart state                                                                                             2
              struct tty_driver                                                                                        -3
              struct tty_port                                                                                               4
              mnt uart_register_dr iver (struct uart driver *drv)
              {
                         struct tty_dr iver *florfflal ;
                         m t I , retvaL

                         BUG ON(drv->state) ;

                        /／중간생 략 . . .

                         if (retval >= 0)
                                  return retval ’,

                      put_ tty_dr iver (norrnal)
             out ktree:
                      ktree(drv->state) :
             out:
                      return -ENOMEM;


                                                                   7 / 312
커 널 연구회（www.kernel.b기                                                                        정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                           문서 표준      8




               }

m번호는 소스코드를 상세하게 설명하기 위한 색인 번호．
색인 번호별로 소스 코드 설명．




함수 요약 설명 테이뷸
     \     r   1
：소
                        함수명                                        설명
ser 1a18250_ init ()                              소스파일：drivers/serial/8250.c
     1   uart_register_dr iver ()                 uart core 계층에 드라이버 등록
     2   이 at 化rmJ이 比已al Ioc( )

     3   platform_device_add()
     4   ser ial8250_re9ister_ports()
     5   platform_dr iver_register ()
     6   platforrn_device_del ()
     7   platform寸device...put()
     8   uart_unregister_dr iver ()




번호는 함수를 설명하기 위한 색인 번호．
함수 색인 번호별로 소스 코드 설명．




                                        8 / 312
커널연구회（www.kernel.뇨）                                             정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                               목차       9




5a大I.
-1     !   -,




내용

DEVICE TREE 상세분석                                                        1

저작권                                                                     2

커널연구회 로드맵                                                               3

커널연구회 교육과정                                                              4

저자 소개                                                                   5

문서 표준                                                                   6

목차                                                                      9

1. 작업환경 및 소스경로                                                        14

     1 . 1 개요                                                         l4

     1.2 작업환경                                                         15
     1.3 DEV兀E TREE 소스경로                                              17

2. DEVICE TREE 소스 분석                                                  21

     2.1 DTS 기본 문법                                                    21
     2.2 DTS 기본 예제                                                    23
       2.2.1 CP(/ 표현                                                  23
       2.2.2 노드 g칭들                                                   24
       2.2.3 U바0／스 표현                                                 24
       2.2.4 comp口tible 속성                                            25
     2.3 주소 표현                                                        26
       2.3.1 C尸｛/ 주소 又-I종／                                            28
       2.3.2 毋모a/ 硏。
                   ／ 장X／들                                             28
      2.3.3 硏모a/ 硏。
                  ／ 응在／는 장X／들                                         了0
       2．了4／乙inges 속성                                                 了／

     2.4 인터 럽트 표현                                                     34
     2.5 사용자 추가 데이터                                                   37
     2.6 특별한 노드들                                                      38


                                       9 / 312
커녈연구회（www.kernel.bz)                             정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                               목차      10




   2.6.2 chosen 노드                                                    39

 2.7 진보된 주제들                                                          39
   2. 7. / 잔보돈／ 장刀 몌졔．                                                39
   2. 7.2 尸C/ 호스트 브릇／兀／                                               40
   2. 7.了／'C/ 주소 섄환                                                   40
   2. 7. 4 진보돈／ 으／E／럽트 깨팡                                             43

3. DEVICE TREE 실용 분석                                                  50

 3.1 CPU 표현                                                           54

 3.2 메모리 표현                                                           57

 3.3 인터 럽트 표현                                                         59

 3.4 CLOCK 표현                                                         63

 3.5 CCI 표현                                                           65

 3.6 내부 시스템 메모리 표현                                                    66

 3.7 MMC 표현                                                           66

 3.8入4CT（타이머） 표현                                                      67

 3.9 핀맵（p水CTL) 표현                                                     68

 3.10 AMBA 표현                                                         83

 3.11 I2S 표현                                                          84

 3. 12 SPI 표현                                                         85

 3.13 UAR1" 표현                                                        86

 3.141八WM 표현                                                          87

 3.15 AI)C 표현                                                         88

 3. 16 12C 표현                                                         88

  3.17 USB 표현                                                         91

  3.I8TMU 표현                                                          93

  3.19 멀티미디어 표현                                                       93

4. DEVICE TREE 실습                                                     96

  4. 1 삼성 ExyNos5420 이하I                                              97

  4.2 개발 환경 구축                                                       100
    4.2. / 우분투 살又／                                                   100
    4.2.2 万빨용 괘刀刀들 살차                                                /01


                                       10 / 312
커널연구회佃＼vw.kernel.b기                               정재준 (r야기3307@nate.comj
Device 가ee 상세분석 in Linux Kernel 4.0                               목차      ]1




   4.2．了 크로스 컴파알e/ 살X/.                                             103

 4.3 소스 빌드 및 포팅                                                     105
   4.3. li／小00/ 소스 삘드                                               /05
   4.3.2 마0／크로 ,SD카드 부탕                                             /13
   4.3.3 e／눅스 刃널 소스 빌드                                              /'7
   4．了．4 恥7스크 포듬／                                                   ／了4

 4.4 커 널 부팅 소스 분석                                                   151

 4.7 GPIO 드라이버                                                      179

  4.5 시리얼（UART) 드라이버                                                190

  4.6 USU 드라이버                                                      196

5. UART 드라이버 상세분석                                                   202

  5.1 UARI' 구조체                                                     204

  5.2 UART 드라이버 등록                                                  205

  5.3 UART 포트 등록                                                    206

  5.4 UART 드라이버 동작                                                  207

  5.5 UART 실행함수들                                                    207

6. UART 구조체                                                         209

  6.1 UART DRIVER 구조체                                               210

  6.2 CONSOLE 구조체                                                   211

  6.3 UART STATE 구조체                                                211

  6.4 TFY DRIVER 구조체                                                212

  6.5rcY PORT 구조체                                                   212

  6.6UART PORT 구조체                                                  213

  6.7UART 8250 PORT 구조체                                             2巧

  6.8 1TY OPERATIONS 구조체                                            216

  6.9 UART OPS 구조체                                                  217

  6.10끼rY STRUCT 구조체                                                218

  6.11 KTER卜4IOS 구조체                                                220

  6.12 UART ICOUNT 구조체                                              220

  6.13끼N LDISC 구조체                                                  221

  6.14 TTY BUFFER 구조체                                               222

  6.15 기타 구조체                                                       223


                                      11 / 312
커널연구회（www.kernel.b기                              정재준 仕gbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                목차




    6.15.1 cdev 구조A沙                                                  223

    6. /5.2 p／아／brm   구조A才                                            223

    6. 15.3proc (／加 entry 구조쳬                                         224

    6.15.4 file oper口tions 구조제                                        224

    6. /5.5 work struc/ 구조졔                                           225

    6.15.6circ b可 구조i泌                                                225

    6. 15. 7b口ud rate 잠수                                              226

7. UART 드라이버 등록                                                        228


  7.1 SERIAL8250 INIT()                                                229

  7.2 UART REGISTER DRIVER()                                           231

  7.3 TrY REGISTER DRIVER0                                             232

8. UART 포트 등록                                                          235


  8.1 SERIAL8250 REGISTER PORTS()                                      236

  8.2 UART ADD ONE PORT0                                               237

  8.3 SERIAL8250 ISA INIT PORTS()                                      239

9. UART 8250 드라이버 동작                                                   241


  9.1 SERIAL8250PROBE()                                                243

  9.2 SERIAL8250 SUSPEND()                                             248

  9.3 SERIAL8250 RESUME()                                              251

  9.4 인터 럽트 동작                                                         254

    9.4. / receive chars()                                             254

    9.4.2 transmit chars()                                             256

10. 삼성 UART 드라이버 동작                                                    257


  10. 1 드라이버 등록                                                        257

  10.2 포트 정보                                                           260

  10.3 PROBE                                                           262

  10.4 드라이버 동작                                                         264

  10.5 문자 전송（TX CHARS)                                                 266

  10.6 문자 수신（ RX CHARS)                                                268

II. TTY 실행 함수들                                                         271


  1 1.1 TTY 드라이버 등록                                                    273

                                       12 / 312
커널연구회佃WV寸kernel.b기                                정재준 (rgb13307@nate.corT기
Device Tree 상세분석 in 니flux Kernel 4.0                               목차       ]3




  I I .2 TTYOPEN0                                                     274

  1 1 .3 끼Y READ()                                                    277

  1 1 .4 FTYWRITE0                                                    279

12. UART 실행 함수들                                                       281


  12.1 입출력(1O) 함수들                                                    283

  12.2 UART OPEN()                                                    285

  12.3 UART WRITE()                                                   287

부록1. SENSOR 정보 요약                                                     289


  AI.l PHOTORESISTOR                                                  289

  A 1.2 PHOTOTRANSISTOR                                               290

  AI.3 거리 센서                                                          291

  Al.4 적외선(INFRARED) 센서                                               292

  AI.5 초음파（ULTRASONR> 센서                                              292

  Al .6 ACCELEROMETERS                                                293

  A1.7 MAGNETOMETERS                                                  294

  AI.8 GYROSCOPE                                                      295

  AI.9 배터리 센서                                                         296

  AI.10 위험（화재, 가스누출）감지 셴서                                             297

부록2. 병렬처리                                                             299


  A2. I 병렬처리 용어정리                                                     299

  A2.2 필요 기술                                                          303

  A2.3 동작 시나리오                                                        304

부록3. 커널연구회 교육과정                                                       308


  A3. 1 교육 일정                                                         308

  A3.2 교육 로드맵                                                         308

  A3.3 상세 교육 내용 테이블                                                   309

  A3.4 커 널연구회 로드맵                                                     引0

  A3.5 실습용 임베디드 보드                                                    311

  A3.6 커널연구회 교육학원 위치（약도）                                              引2




                                       13 / 312
커널연구회（www.kernel.bz)                              정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                          ] . 작업환경 및 소스경로      ]4




] . 작업환경 및 소스경로




                                                  + 필자의 주말농장에서 찍은 코스모스



].］개요
부트로더는 리눅스 커널을 타켓 보드의 RAM에 복사한 다음에 커널로 진입(jump）하는 역할을
한다.   커널은 CPU을 설정하고 가상 메모리를 초기화 하는 여러가지 작업들을 콘솔에 표시한다．
이러한 커널의 동작들은 장치들의 정보를 레지스터에 쓰면서 수행된다.                               프로세서 코어들의
종류가 많고 접근할 수 있는 메모리 용량도 다양한 상황에서 커 널은 어떻게 레지스터들의 주소를
알 수 있을까？ 쉽게 직관적으로 해결할 수 있는 방법은 커널 소스안에 플렛폼 의존적（맞춤형）인
부트 루틴을 만드는 것이다.              이것은 커 널 파라미 터들을 사용하여 설정할 수 있다．               이러한
방식은 모든것이 고정되어 있을때는 좋은 해법이 될 수 있지만, 장치들이 가변적으로 변경된다면
커널은 실행 시간（rur卜time）에 변경된 장치들을 알아내야 한다．


AR卜月 아키텍처는 점점 다양화 되고 있어 리눅스 커뮤니티에서 논란이 많아지고 있다.                             AR卜기
보드마다      자신만의     외부 장치들을         제각각   장착하고     있어서,   커널    안에   특별한 환경설정
파라미터를 패치하거나 헤더 파일들이 제멋대로 생겨나고 있다.                         이로 인해서 커널 소스가
난잡해지고 유지보수가 힘들어져서 커널을 분석하는데 점점 어려움을 느끼고 있는 실정이다．
또한, 커 널 소스가 특정 보드상의 특정 칩에 맞게끔 컴파일되어 실행 바이너리가 생성됨으로
인해서 모든 ARM 프로세서에 호환되지 못하는 상황이 벌어지고 있다.                        그러나 PC에서는 미Os가


                                       14 / 312
커널연구회（www.kern이.bz)                                      정재준 (rgbi3307@nate.con力
Device Tree 상세분석 in Linux Kernel 4.0                                               1. 작업환경 및 소스경로            15




있어서 하드웨어 장치가 변경되면 자동적으로 검출하여 동작하도록 해주는 작업이 쉽다.                                                       AR卜기
프로세서는 미Os가 없어서 리눅스 커널이 모든 역할을 다해주고 있어서 리눅스 커 널을 믿는
수밖에 없다.           그래서 리눅스 커널에 도입된 해결책이 디바이스 트리（device 打ee）이며， Open
Firmware (abbreviated OF) 혹은 디attened Device Tree (FDT）라고 언급되기도 한다．


디바이스 트리는 강력한 규정이라기 보다 엄격한 관례라는 관점으로 접근하는 것이 바람직하다．
예를들면, 디바이스 트리안의 경로와 파라미터는 어떻게 정하는 것이 좋은지 정해진 관례를
따라가는 것이다.             정해진 AP17F 특정 데이터에 접근하도록 표준화된 트리 구조체를 사용하도록
한다.      주변장치들의 버스, 주소, 인터럽트, 변수들은 정하찐 관례를 지켜서 디바이스 트리에
표현한다.         디바이스 트리는 커 널의 일부분으로서 하드웨어 정보를 추가, 제거, 운반하는 장소
역할을 한다.


디바이스 트리를 심도있게 학습하기 전에 먼저 아래에서 작업환경과 디바이스 트리 소스경로를
확인하여 기본적인 배경 지식을 요약 정리한다．




1.2 작업환경
Device Tree는 리눅스 커널 3.1(2011-10-24）부터 소스에 적용되었다.                                  그런데, 필자가 이글을 집필
할 때 리눅스 커 널 4.0이 배포되었으므로 가장 최신 소스인 Iinux-4.0을 가지고 Device Tree을 설
명한다． 하드웨어 아키텍쳐는 삼성 Exynos542U(Arndale Octa Board）을 선택하여 실습 했으며 리
눅스 Ubuntu 12.04 배포판（64비트 버전）에서 크로스 컴파일러 " arm-eabi- " 룰 사용하여 소스를 빌
드했다.


이곳에서는 이들을 간략히 설명하고, 좀더 자세한 내용들은 " 제4장 Device Tree 실습"에서 개발환
경 구축과 소스 빌드 방법들을 자세히 설명한다．


Linux Ken,耐 닯出rce Ver的口n Iinux-4.0



러뉵스 커甘 4企」
참조 :
https: fflkml .org/ lkml/ 2015/ 4/12/178
htt口:/ / I i i 1口Ut ing. corn/ 2015/0酊 I inUX叫4-0十em n이 released- f 아놔帥at 기 t 5；빛orth.htmi



2015년 4월 ]2일（일） 15:41
1ma Shee口와 리 너스 토발즈는 LKML 메일링을 통해서
니flux 319.4 배포이후 다음버전을 니flux 3.20으로 하지 않고 니flUx 4.0 으로 결정했습니 다．

나flux 4.0의 특징을 요약하면 ,

                                                    15 / 312
커 널 연구회（www.kerneib기                                                             정재준 (rgbi3307（亘）nate.con가
Device Tree 상세분석 in Linux Kernel 4.0                                ] . 작업환경 및 소스경로         ]6




니ye kernel 패치 기능으로 시스템을 리부팅하지 않아도 커널이 업데이트 됨 .
AMD Radeon 드라이버가 [）田playPort를 통하여 audio을 지원함．
Intel의 Sky lake 프로세서를 지원함．

니flux 4.0 버전은 새로운 기능들을 많이 추가한 것이 아니라
안정화에 초점을 맞춘 stable 이ease라고 언급하고 있습니 다．

니flux 4.1 버전에서 좀더 많은 변화7F 있을 것이라고 예고하고 있습니다．

Linux 4. 0 download:
https: //넥刊w. kernel . org/pub/ I inux/kernel/ v4. x/




Hardware Architecture: Samsung Exynos5420 (Arndale Octa Board)




위의 보드는 AR卜기 Cortex-Al 5 1.8GHz 코어 4개와 Cortex-A7 1.2GHz 코어 4개가 합쳐진
너9.니TTLE 아키텍처 구조로 되어 있으며 관련정보 및 구매는 아래1 링크를 참조하기 바란다．


Arndale Octa Board 관련 정보 홈페이지 링크：
http://www.arndaleboard.org/wiki/index.php/Main Page
Arndale Octa Board 구매 관련 링크：
http://www.arndaleboard.org/wiki/index.php/Saleschannel



                                                        16 / 312
커널연구회（www.kernelbz)                                                정재준 (rg너3307@nate.com)
Device Tree 상세분석 in 니nux Kerr油 4.0                                           ] . 작업환경 및 소스경로        17




크로스 컴파일러 버전은 다음과 같이 확인한다．




$ arm-eab I小gcc 小四田山n
arm-eabi-Qcc (6CC) 4.6.x-(}oo키e 20120106 (prerelease)
Copyright (C) 2011 Free Software Foundation, Inc.
This is free software; see the source for copying condit ions. There is NO
warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.




이글은 Iinux-4.O 커널 소스와 Documentation 경로에 있는 문서들을 챰조하여 집필한다.                                  Device
Tree는 커 널 소스의 Documentation/devicetree 경로에 설명되어 있다.                          아울러 Device Tree의 문법
적인 내용들은 아라1 사이트를 참조했다．


http://devicetree.orq/Device_Tree..Usage


디바이스 트리에 대해서 사전 지식이 있는 독자분들은 제2장의 내용들은 가볍고 확인하고 제3장
과 4장으로 바로가서 실습해 볼 수 있다．




1.3 Device Tree 소스경로
Device Tree 소스（스크립트）는 커널의 arch/arm/boot셔ts/ 경로에 있다． 소스 스크립트 파일은 아
키텍쳐별로 구성되어 있다． 삼성 Exynos5에 관한 스크립트 파일은 다음과 같이 확인할 수 있다．




$ cd arch/ arni/boot/ dts

$ I I exynos5士
  rw-rw-r-- 1 jungj j jungjj 12670 Feb 11 16: 01 exynos5250-arndale. dts
-rw-rw-r-- 1 jungj j jungj j 18304 Feb 11 16: 01 exynos5250. dtsi
  rw-rw-r-- 1 jungj j jungi j 16324 Feb 11 16: 01 exynos5250-pinctrl .dts
  rw-rw-r-- 1 jungj j jungjj 8737 Feb 11 16: 01 0xyn055250-smdk5250. dts
  rw-rw-r-- 1 jungj j jungjj 13126 Feb 11 16:01 exynos5250-snow. dts
-rw-rw-r-- 1 jungj j jungjj 7604 Feb 11 16: 01 exyn0s5260. dfsi
  rw-rw나-- 1 jungj j jungj j 11172 Feb11 16: 01 exyn055260-pinctr l . dtsi
  rw-rw-r-- 1 jungj j jungj j 1873 Feb 11 16: 01 exynos5260-xyref5260. dts
  rw-rw-r-- 1 jungj j jungj j 5463 Feb 11 16: 01 exynos54lo. dtsi
-rw-rw-r-- 1 Jungj j jungjj 1400 Feb 11 16: 01 exynos5410-smdk54lo. dts
-r中rw나-- 1 junqjj jungjj 9160 Feb 11 16:01 exynos5420-arndale-octa.dts
-r忙rw寸- 1 junjj jungjj 21756 Feb 11 16:01 exyn0s5420.dtsi
  rw-rw-r-- 1 jungjj jungjj 19229 Feb 11 16: 01 exynos5420-peach-pit. dts
  rw-rw-r-- 1 jungjj jungjj 14024 Feb 11 16: 01 exynos5420-pinctrl .dtsi
-rw-rw-r-- 1 jungjj jungjj 9710 Feb 11 16:01 exyn0s5420-smdk5420. dts

                                               17 / 312
커 널 연구회如,ww.kern이.b기                                                     정쟤준 (rgbi3 307@r日te.com)
Device Tree 상세분석 in Linux Kernel 4.0                                         ] . 작업환경 및 소스경로          18




-rw-rw나-- 1 jungj j jungjj 7093 Feb 11 16: 01 exynos5440.dtsi
  rw-rw-r-- 1 jungj j jungjj  871 Feb 11 16: 01 exynos5440-sd5vl . dts
  rw-rw-r-- 1 jungj j jungjj 1559 Feb 11 16: 01 exynos5440-ssdk5440. dts
  rw-rw-r-- 1 jungj j jungjj  684 Feb 11 16: 01 exynos5800.dtsi
  rw-rw-r-- 1 jungjj jungjj 18961 Feb 11 16: 01 exyn0s5800-peach-pi . dts
-r州나w나-- 1 jungJj iungij 2796 Feb 11 16:01 exynos5.dtsi




.dtsi 파일은 System On Chip(SoC) 레벨에서 정의한 인클루드 파일이고，.dts 파일은 보드 레벨에서
정의한 스크립트 파일이다.                 dts 파일은 XML처럼 데이터의 구성을 문법적으로 기술한 것이다．


dts 스크립트를 바이너리 파일（.dtb）로 컴파일하는 Device Tree Corn이er 소스는 커널의 scriptsldtc
경로에 있다.           dtb 파일은 커널을 빌드할 ［대1 아래의 Makefile 정보를 참조하여 생성된다．
                 卜기akefile 에서 EXYNOS（게 관련된 것만 확인하1 보면 다음과 같다．
arch/arm/boot/dts／




dtb-$(C0NHG_ARCH_EXYN0S) += exynos42lO-or igen. dtb W
        exynos4210-smdkv310. dib W
        exyn0s4210- trats.dtb W
        exynos42lo-universal_c210. dtb W
        exyn0s4412山야이山3. d比 w
        exynos4412-odroidx. dtb W
        exynos4412-o먀이dx2. d比 w
        exynos4412-or igen. dtb W
        exyn0s4412-smdk4412 d t b W
        exynos4412- tiny4412. dtb W
        exyn0s4412- trats2. dtb W
        exynos5250-arndale.dtb W
        exyn0s5250-smdk5250 . dtb W
        exyn0s5250-snow. dtb W
        exynos5260-xyref 5260. dtb W
        exyn0s5410冬mdk5410. d比 w
        exynos5420-arndale--octa.dtb W
        exynos5420-peach-pi t .dtb W
        exyn0s5420-smdk5420. dtb *
        exyn0s5440-sd5vl .dtb *
        exynos5440田記碼440. d比 w
        exyn0s5800-peach-p i . dtb




dtb 파일은 부팅할 때 부트로더仙七oot)에 의해서 적재되고 커널이 파싱한다． 나boot에서 부팅
명령어인 bootz에 dtb가 있는 메모리 주소를 다음과 같이 알려준다．


bootz kernel addr ramdisk addr dtb addr
bootz 0x20008000 0x21000000


커널에는 kernel_entry() 함수에 d由ad먀를 다음과 같이 전달 한다．

                                                 18 / 312
커널연구회（www.kernel.b기                                                         정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니nux Kernel 4.0                               1. 작업환경 및 소스경로           19




OLD: kernel_entry(0, machid, atag_addr)
NEW: kernel_entry(0, mach_id, dtb_addr)


커널 소스를 빌드할때는 menuconfig에서 아래 내용이 선택되어 있는지 확인한다．


Boot options 今 Flattened Device Tree support


커널을 부팅한 이후에는 /proc/device-tree 경로에서 다음과 같이 장치 설정정보들을 확인할 수 있
다．
# Cd /proc/ device- tree/
# 아vd
加roc/ dev ice나 ree
# Is -a
#address-cel Is                    mmc@12210000
#SI Z寸아키 Is                        mmc@12220000
                                   model
                                   name
adc@12D10000                       phy@12100000
al iases                           phy@12130000
amba                               phy@12500000
audss-cl ock-cont ro I Ier@3810000 pinctr l@03860000
cc i@10d20000                      pinctr l@13400000
chip i d@10000000                  pinctrl@13410000
chosen                             pinctr I@14000000
clock-control ler@10010000         pinctr 1 @14010000
codec@11000000                     ［째ver-如ma i n이0044000
compat it키 e                       P0나er 寸（幻mal n@10044020
Cpus                               power -doma 1 n@10044060
dp-control ler@145B0000            P0나er （加mai n@10044120
dsi@14500000                       pwm@12dd0000
f imd@i14400000                    r t c@] 이 E0000
f i rmware@02073000                ser ial@12C00000
f ixed-rate-clocks                 ser 1 al@12C10000
q口i 0_keys                         ser ial@12C20000
hdrn i @14530000                   ser ial@12C30000
hdru i phy@14500000                spi@12d20000
i 2c@12C60000                      spi@12d30000
i2c@12C70000                       sp 1 @12d40000
i2c@12C80000                       sss@10830000
I 2c@12C90000                      syscon@10050000
I 2c@12CA0000                      sysram@02020000
12c@12CB0000                       system-control ler@10040000
I 2c@12CC0000                      tmu@10060000
i2c@12C00000                       tmu@10064000
i2c@12E00000                       t mu@10068000
i 2c@12E10000                      tmu@1006c000


                                                 19 / 312
커 널 연구회（ww＼사．kernel.b기                                           정재준 (rgbi3307@nate.con가
Device Tree 상세분석 in 니flux Kernel 4.0                         ] . 작업환경 및 소스경로          20




 2c@12E20000                     tmu@100a0000
 2s@03830000                     usb@12000000
 2s@12D60000                     usb@12110000
 2s@12D70000                     usb@12120000
 nterrupt卜contro1 Ier@10440000   usb@12400000
 nterrupt-control Ier@10481000   video-phy@10040714
 nterrupt-parent                 v ideo-phy@10040728
mct@101C0000                     미 deo-sca ler@13e00000
memory                           video-scaler@13e10000
mixer@14450000                   V怡tchdo（抱10化0000
mmc@12200000


지금까지 Device Tree에 대한 개념을 간단히 요약하여 설명했다.                   이제부터는 Device Tree 소스구
조와 이것을 어떻게 빌드하여 커널에 적재후 부팅하는지 자세히 알아 보도록 하자.                            Device Tree
에 대해서 사전 지식이 있는 독자분들은 제2장의 내용은 가볍게 확인하고 제3장부터 실습할 수
있다．




                                               20 / 312
커널연구회佃ww.kernel.b기                                         정재준 (rg너3307@nate.com)
Device Tree 상세분석 in 니flux Kerr倒 4.0                                         2. Device Tree 소스 분석   21




2. Device Tree 소스 분석




                                                                 年 필자의 주말농장에서 찍은 장미꽃



2.1 DTS 기본 문법
아래 예제는 DTS 기본 문법을 개념적으로 표현한 것이다．


/{
     nodel {
         a-string-property = "A str ing ' ;
         十String니 1st-아0口erty = 나 나St str ing'' , "second string" ;
         十byte너카a가V叩아ty = [OxOl 0x23 0x34 0x56] ;
          chi ld-nodel {
               f I rst-chi Ic卜아operty;
               second-chi ld-property = <1> ;
               十St ii n丁아叩아 ty = "Hel lo , 川or Id " ;
          };
          아i Ic｝느node2 {
          };
     };
     node2 {
          a十em口口가玎 operty ;
          十ce I卜아叩아 ty = <1 2 3 4>; ／士 each number (cel l) is a u1nt32 */
          chi ld-no把l {
          };
     };
};
                                                    21 / 312
커 널 연구회（ww比kerneLb기                                                    정재준 畇b日307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                 2. Device Tree 소스 분석




／는 루트 노드를 의미한다.                 노드는 {｝로 범위를 규정한다.         루트 노드는 nodel, node2라는 child
노드를 가지고, node］는 또다시 child-nodel, child-node2을 가지고, node2는 ch山十node］를 가진
다. 위의 노드를 트리구조로 표현하면 다음과 같다．




{｝안에 노드 속성들을 표현하며 다음과 같은 종류들이 있다．


長자얹：" "을 사용하여 다음과 같이 표현한다．

string-property = "a string";


C州除 <＞을 사용하여 다음과 같이 32비트 부호없는 정수로 표현한다．

cell-property = <0xbeef 123 0xabcd1234>;


이진 톄이터·. [］을 사용하여 다음과 같이 표현한다．
binary-property = [OxOl 0x23 0x45 0x67];


혼합된 데이터：,을 사용하여 다음과 같이 표현한다．

mixed-property = "a string", [OxOl 0x23 0x45 0x67], <0x12345678>;


문자얹 리스트·, ,을 사용하여 다음과 같이 표현한다．
string-list = "red fish", "blue fish";




                                           22 / 312
커널연구회佃ww.kern이b기                                                    정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                        2. Device Tree 소스 분석      23




2.2 DTS 기본 예제
아래와 같이 간단한 ARM 호환 머신（제조사 " Acme", 제품명 "Coyote's Revenge"）을 예제로 디바이
스 트리를 표현하1 보자． 이 AR卜ii 프로세서는 로컬 버스 형태로 memory mapped 시리얼 포트，
SPI 버스 컨트롤러, 12C 컨트롤러 인터럽트 컨트롤러 , 외부 버스 브릿지를 가지고 있댜．


2개의 32비트 AR卜月 CPU.
0번지 위치한 256MB 크기의 SDRAM,
0x101F1000 와 0x101F2000 번지에 위치한 2개의 시리얼 포트．
0xi0l F3000 번지에 위치한 G미O 컨트롤러．
0x10170000 번지에 위치한 SPI 컨트롤러, 아래의 장치를 가지고 있음．
      ss 핀이 G미O#] 에 연결되어 있는 MMC 슬롯．
외부 버스 브릿지, 아래의 장치들을 가지고 있음．
      주소가 0x10100000인 외부 버스에 연결되어 있는 SMC SMC9111] 이더넷 장치．
      0x10160000 주소에 연결되어 있는 I2C 컨트롤러, 아래의 장치를 가지고 있음．
             슬레이브 주소 1101000 (0x58）에 응답하는 Maxim DS1338 리얼타임클럭（RTC)
      0x30000000 주소에 연결되어 있는 64MB의 NOR 플래시 메모라




위의 예제를 디바이스 트리로 표현하기 위해서 첫번째로 해야 할일은 구조체 root를 다음과 같이
표현하는 것이다．


I {
      compat 比）比 = 「 acme ,coy아es나everige " ;
};


compatible 속성은 시스템의 이름을 “제조사，제품명" 형태로 기술한다.                  이것은 namespace 충돌을
회피하는 역할을 하며, 장치를 정확하게 기술하기 위해서 꼭 필요한 부분이다． 커널은 머신을
어떻게 실행할 것인가에 대한 판단을 이 값을 가지고 하므로 정확하게 표현해야 한다．



2.2.1 Cpu 표현
시스템에 있는 CPU들을 cpus {} 노드를 사용하여 다음과 같이 기술한다｛dua卜core Cortex A9)


/ {
      compatible = "acme, coyotes-revenge ' ;

      야）us {
          cpu@O {
              compatible = 'arm,cortex-a9n;


                                                23 / 312
커 널 연구회（www.kerr｝이．bz)                                     정쟤준 仕gbi3307（亘）nate.con가
Device Tree 상세분석 in 니flux Kernel 4.0                                  2. Device Tree 소스 분석     24




            };
            cpu@1 {
                compatible = 'arm,cortex-a9" ;
            };
       };
};
각각의 Cpu 노드안에 있는 compati비e 속성은 " 제조사，모델명 " 으로된 문자열 형태로 정확하게
기술해먀 한다.               위의 Cpu 노드는 아주 기본적인 것만 표현했으면 좀더 다양한 것들은 실제
예제에서 자세히 설명한다．



2.2.2 노드 명칭들
모든 노드에는 name[@un小address] 형태의 명칭이 있다.                              nan祀은 ascii 형태의 문자열로
표현하며 31711 문자 길이까지 가능하다.                             name은 어떤 종류의 장치인지를 일반적으로 나타낸다．
예를들면, 3com 이더넷 장치를 name으로 표현할때 3com509 라고 표현하지 않고 일반적인
명칭인 ethernet 이라고 표현한다．


un比ad打ess는 장치의 주소를 의미한다.                              일반적으로, 장치 주소는 장치에 접근하고자 할때
사용되는 것으로 reg 속성에 나열된다.                               reg 속성은 이후에 자세히 설명한다.      형제 노드들의
name은 유일하게 표현해야 하지만, 주소가 다르다면（serial@10卄］000 & serial@101f2000) 동일한
name으로 표현해도 된다．



 2.2.3 디바이스 표현
시스템에 있는 각각의 장치들은 노드로 표현한다.                                  위에서 DTS 기본 예제로 기술한 시스템을 디
바이스 트리 노드들로 표현하면 다음과 같다．


 / {
       compatible = "acme, coyotes-revenge";

       Cpus {
           cpu@O {
               compatible      " arm,cor tex-a9" ;
            };
            야）u@1 {
                compatible     "arm,cortex-a9 ' ;
            };
       },
       serial@101F0000 {
            compatible = 'arm,plOll '' ;
       }:
                                                      24 / 312
 커 널 연구회（www.kerne냐끄）                                                정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 나nux Kern이 4.0                                         2. Device Tree 소스 분석   25




     serial@101F2000 {
          coin口at 仕）le = 'arm , 이011 n ;
     };
     a이砲化作3000 {
        compat 比니e = "arm , 이061 " ;
     };
     interrupt-control ler@10140000 {
         compatible = "arm,p1190";
     };
     spi@10115000 {
         compatible = "arm,p1022";
     };
     external-bus {
         ethernet的,0 {
             compatible = "smc,smc9lclll ";
              };
               i2c@1,0 {
                   corn口at 1 ble = "acme , 키234니2c寸）us', ;
                   rtc@58 {
                        com口at 比니e = 'max i叱ds化38" ;

              };
                    };
              f m앍他2刀 {
                  compatible = "samsung,k8t1315ebm", 'cf i- f lash";
              };
      };
};


위의 디바이스 트리는 장치들이 시스템에 연결되어 있는 구조를 표현한다. 위의 표현에서 몇가지
틀린 곳이 있는데， 이것은 장치들간에 연결 정보가 서로 맞지 않아서 발생한 것이며, 자세한 이유
는 계속 설명 된다． 위의 디바이스 트리에서 몇가지 중요한 부분을 다음과 같이 정리할 수 있다．


          .        각각의 장치 노드는 compati비e 속성을 가지고 있다．
          1        flash 노드는 compat巾旭 속성에서 2개의 문자열을 가지고 있다．
                                                          （이유는 계속 설명된다）
          1        이미 언급한 내용이지만， 노드의 명칭은 장치 모델명이 아니라 일반적인 장치 이름으로
                   명칭을 정한다．



2.2.4 compatible 속성
장치를 표현하는 각각의 노드는 compati비e 속성울 필요로 한다.                                  compati비e 속성은 커널이 어떤


                                                             25 / 312
커널연구회（www.kernel.b기                                                      정재준 岫印307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                2. Device Tree 소스 분석     26




디바이스 드라이버를 해당 장치와 연결할 것인가를 판단하는데 사용한다． compati키e은 문자열
형태의 리스트이댜.            첫번째 문자열은 " 제조사, 모델명 " 형태로 장치를 정확히 표현한다.                      그 다음
문자열은 이 장치와 호환되는 또다른 장치명을 표현한다.                              예를들면， Freesca旭 卜4PC8349 System
on Chip (SoC）은 시리얼 장치이며 Nat向nal Semiconductor ns16550 레지스터로 구성되어 있다．
이 장치를 compatib恒로 다음과 같이 표현할 수 있다‘


compatible = "fsl,mpc8349-uart' , "nsl 6550";


"fsl,mpc8349-ua八" 는 정확한 장치를 표현하고， "ns16550"는 National Semiconductor 16550
UART와 호환된다는 장치를 의미한다.                     "ns16550" 에 제조사를 기술하지 않은 것은 역사적으로
nsl 6550은 제조사를 가지고 있지 않기 때문이다．                         그러나 대부분의 장치는 제조사를 표현해먀
한다． 한가지 주의할점은 "fsl,mpc83xx-uart " 처럼 와일드 문자 " xx "를 사용하지 말고 제조사와
제품명을 모두 정확하게 표현해 주는 것이 좋다．




2.3 주소 표현
디바이스의 주소를 디바이스 트리에 표현하기 위해서 정하匹 속성에는 다음과 같이 3가지가 있다．


#address-cells
＃引ze-ce小

reg


이 속성은 서로 연관 관계를 가지고 있다．
"#ad（打ess-cells" 속성과 " #size-cells" 속성은 reg 속성의 데이터에 대한 갯수 규칙을 지정한다．
"#a(k打ess-cells" 속성과 "#size-cells" 은 부모 노드에서 지정하고 reg 속성은 자식 노드에서
지정한다.      먼저 reg 속성에 대해서 알아보자. reg 속성은 다음과 같은 형식을 가진다．


reg = ＜주소］ 길이］［주소2 길이21［주소3 길이31 ... >


주소와 길이가 하나의 묶음이 된다.                       보드에 있는 디바이스를 제어하기 위해서 하나의 주소
일수도 있고 여러개의 주소를 가지고 았을 수도 있다.                              또 각 주소는 연속적일 수도 있고 불연속
적 일 수도 있다.          그래서 시작주소와 시작주소부터의 주소 범위를 하나의 묶음으로 지정하고
이것을 나열하게 된다.              여기서 우선 셀（cell) 이라는 용어에 대해서 알아 보자.                    주소나 길이를
나타내기 위해서는 32비트 정수값을 사용한다.                            예를들면 0xl 2345678 또는 0 처럼 표현할 수
있다.    이런 값 하나를 셀이라고 한다.                  결론적으로 셀은 32비트 정수값이라고 보면 된다.                 reg는


                                                26 / 312
커널연구회佃wwkernel.b기                                                  정쟤준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니nux Kernel 4.0                                        2. Device Tree 소스 분석     27




다음과 같이 셀들의 데이터 집합으로 표현한다．


reg = <0x0C00 0x0 0xFFFF02 0x3333>


여기서 0x0C00 0x0 0xFFFF02 0x3333 이 셀들이다.                       그런데 여러분은 이 값들의 의미가 이런
식으로 될것이라고 예상할 수 있을 것이다．


0x0C00 : 시작 주소
0x0             : 주소 범위 크기
0xFFFF02: 시작 주소
0x3333          ·. 주소 범위 크기


이렇게 생각하면 맞을 수도 있고 틀릴 수도 있다.                                  만약에 64비트 주소 체계라면 위의 표현이
맞을까？ 아니면 특수한 주소라서 32비트로 모두 표현할수 없다면？ 이런 문제를 해결하기 위해서
"#adc打ess-cells" 속성과 "#size-cells" 속성이 있는 것이다.                       보통 다음과 같이 reg 의 셀들이
주소를 지정하기 위해서 몇개의 셀을 사용할지를 결정하고 길이를 지정하기 위해서 몇개의
셀들을 사용할지를 결정해1 주는 것이 바로 "#adc如ess-cells" 속성과 "#sjze-cells" 속성이다.


32비트 시스템에서는 #address-ce小 값이 ] 이고 ＃引ze-ce小 값도 ] 이 된다.                            64비트 시스템에서는
#address-cells 값이 2이고 ＃引ze-ce小 값은 2가 된다.                        이처럼 #ad如ess-ce小 속성은 reg 속성
값에 시작 주소를 지정하기 위해서 몇개의 셀을 사용할 것인가를 지정한다.                                          #sjze中cells 속성은
reg 속성 값에 길이를 지정하기 위해서 몇개의 셀을 사용할 것인가를 지정한다． 개념적인 설명을
위해서 시작 주소는 27卄의 셀을 가지고 길이는 1;Il의 셀을 가질 경우에 대한 예를 들어본다.
실제 사용 방법은 CPU와 디바이스를 추가 할따1 다시 설명할 것이다.


parent {
           #address-cel Is = <2>;
           #size-cel ls = <1> ;
           chi ld {
                reg = <0xC0000000 0x0000 1024> ;
           };
           chi ld {
                reg = <OxD0000000 0x0000 1024 0xE0000000 0x0000 2048> ;
           };
};
위의 예제에서 #ad打ess-ce小 속성과 #size-c이Is은 자식 노드에만 영향을 준다.                                행당 노드에 대한
셀 지정은 상위의 부모 노드0杉］ 지정한다.                            이제 주소 지정과 관련하여 CPU부터 디바이스까지
좀더 자세히 알아 보도록 하자．

                                                  27 / 312
커 널 연구회（ww比kernel.b기                                                      정쟤준 (rgbi3307@nate.com>
Device Tree 상세분석 in Linux Kernel 4.0                                    2. Device Tree 소스 분석    28




2.3.1 Cpu 주소 지정
보통 주소라 하면 머리속에 연상되는 것중 하나가 버스 주소일 것이다.                                     하지만 주소라는 것올
이런 제한적인 개념으로 보지 말고, 어떤 디바이스를 접근하거나 다루기 위한 구별자로 보는 것이
이해하기 쉽다.            CPU의 주소 지정 역시 버스 주소가 아닌 구별자로써 의미를 갖는다.                           다음 CPU
노드에 대한 표현은 CPU 주소 지정에 대한 간단한 예제이다．


Cpus {
          #address-cel ls = <1>;
          #size-cel ls = <0>;
          cpu@O {
              Compatib 'e = 'arm,cortex-a9";
              reg = <0>;
           };
          cpu@1 {
              compat 汁)Ie       narm,cor tex-a9 ' ;
              reg = <1>;
           };
};
위의 예제에서 각 CPU의 선언에는 주소를 이용하여 하나의 고유 山를 주소로 부여하고, 크기에
대한 정보는 없음을 보여 주고 있다.                             위에서 Cpus 노드에 #adc打ess-c이！S은 ] 로 설정하고 #size-
ce小은 0으로 설정하고 있다.                         이 의미는       CPU 각각을 표현하는 자식 노드의 reg 속성 값의
셀들에 주소는 ]7卄의 셀로 되어 있고 길이 값은 셀을 사용하지 않으므로 아예 없음을 나타낸다．
좀 쉽게 이야기하면 reg 속성값에 셀들이 모두 주소라는 것이다． 이전에 노드 이름을 지정할 때
주소는 구별하기 위한 값으로 어떤 것을 사용해匠 된댜고 했다.                                    하지만, 규정에는 노드의 reg
속성값으로 사용된 첫번째1 주소 값을 노드 이름의 장치 주소에 사용하도록 하고 았다.                                           위의
예제에서도 이름에 대하여 이런 규칙을 적용하고 있다．



2.3.2 메모리 미悟 장치들
CPU와는 다르게, 대부분의 장치들에는 메모리 주소가 매핑 된다.                                    이러한 장치들에는 주소를
범위（range）로 지정한다.                  지정하는 방식은 위에서 이미 설명한 #addre弱ce小 속성과 #size-cells
속성을 그대로 사용한다． 아래의 예제를 보도록 하자．


 / {
       #address-cel ls = <1>;
       #size-cel ls = <1>;




                                                      28 / 312
커 널 연구회（www.kern이.b기                                                   정재준 (rgb日307@nate.com)
Device Tree 상세분석 ir) 니flux Kernel 4.0                   2. Device Tree 소스 분석     29




     serial@101f0000 {
          compat ible = 「 arrn,ploll " ;
          reg = <0x101f0000 0x1000 >;
     };
     serial@101f2000 {
          compatible = 'arm,ploll ' ;
          reg = <0x101f2000 0x1000 >;
     };
     야io@101f3000 {
        compatible = " arm,p1061 " ;
         reg = <0x101f3000 0x1000
                0x10114000 0xOOlO> ;
     };
      interrupt-control Ier@10140000 {
          corn口at 吐니e = " arrn,p너90「 ;
          reg = <0x10140000 0x1000 >;
      };
     spi@10115000 {
         compat ible = 'arrn,p1022 ' ;
         reg = <0x10115000 0x1000 >;
      };
};


우선 디바이스 주소에 정보를 다루기 위해서 reg 속성을 사용한다.                   그리고 reg 속성의 값에서
주소와 길이를 표현하는 셀의 갯수를 지정하기 위해서 부모 노드인 " /" 노드에서 椒dress-ce小
를 사용하여 시작 주소를 표현하기 위해1 몇개의 셀을 사용하는지 지정한다.                      위의 예제에서는 ]
이므로 한개떽 셀 즉 32 비트 부호없는 정수를 사용해서 시작 주소를 나타낸다.                         마찬가지로
＃탉ze｛이k를 사용해서 길이를 나타내기 위해서 몇개의 셀을 사용하는지도 지정한다.                       일반적으로
셀의 개수는 32비트 시스템에서는 ］을 64트 시스템에서는 2를 사용한다．                       위예에서      G미O
디바이스 주소를 살표보면 GPIO 디바이스 주소는 0x10113000 싸 0x10卄3術와 0x10卄4000 싸
0xi이f40아의         두7卜1 주소 범위가 부여되고 있음을 알 수 있다．


그런데， 노드들은 하부에 자식 노드들이 포함될 수 있고 해당 자식 노드 역시 reg 속성을 가질 수
있다.        이따1 #adc打ess-cells오f ＃듸ze-cells은 특별히 아래에서 선언하지 않으면 자식 노드에게
상속되어 그대로 적용된다.                       그런데 상위에서는 하나의 주소값만이 필요하지만 하부의 자식
노드에서는 두개의 셀로 구성된 주소값이 필요할 수도 있다． 아래의 예제를 보면，


external-bus {
        #address-cel Is = <2>
        #size아키 Is = <]>',


                                           29 / 312
커 널 연구회（www.kernel.bz)                                 정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                2. Device Tree 소스 분석     30




       ethernet@0,0 {
           compatible = "smc,smc9lclll ";
           reg = <0 0 小l000>;
       };
       i2面］,0 {
          compatible = "acme, a1234- i2c-bus' ;
          reg = <1 0 oxl000>;
          rtc58 {
              compatible = "maxim,ds1338";
            };
       };
       f I asr世2,0 {
             compatible = 'samsung,k8f1315ebm' , 'cf i- f lash";
             reg = <2 0 0x4000000>;
       };
};
externa卜bus 노드는 #address-ce小을 두개 지정했고 #size-c이Is은 한                     II 지정했다.    따라서
external-bus 노드안의 자식 노드들은 위의 주소 지정방식을 따르게 된다.                            주소 값으로 두개의
셀을 지정했으므로 reg에 표현한 첫번째1 값은 칩 선택 (ch巾 selection) 번호이고 두번째 값은 칩
선택 기준으로부터의 오프셋이다.                     세번째 값은 주소의 크기이다．


위의 예제에서 externa卜bus는 상위 부모 노드에 해당되는데, 이곳에서 #ad如ess-cells고F #size-
ce小로 그 하부의 자식 노드들의 reg 속성 값에 대한 사용 셀 수를 지정하고 있다．


어떤 디바이스는 주소를 표현하는데 하나의 셀을 사용할 것이고 어떤 디바이스는 두개의 셀을
사용할 것이다.         이런 경우에는 그 하부에 다시 셀에 대한 설정을 하지 않는다면, 상위의 셀 수
에 대한 정의가 모두 하부 노드에 적용된다.                                그러므로 상위 노드에서 가장 많은 셀 수를
사용하는 디바이스 노드에 대한 수로 지정헤1 놓으면 하부의 모든 노드는 동일하게 표현될 수
있다.    여기서 기억해야 할 것이 노드이름에 대한 장치 주소는 reg 속성의 첫번째1 주소 지정의
값을 사용해먀 한다는 것이다.                     위의 예제에서 플래쉬의 경우를 보면 노드명을 " flash@ 2,0" 올
 사용하고 있다.        2,0으로 표현하고 있는데, 노드의 reg 속성에 첫번째 주소를 지정하기 위해서 2
와 0 을 사용하고 있는 것이다. 이것을 ', ' 로 분리해H 지정하고 있음을 기억해1 주시기 바란다．



 2.3.3 메모리 매핑 않되는 장치들
 어떤 디바이스들은 프로세서 버스에 직접 메모리 매핑 될 수 없는 것들이 있다.                                    이들은 주소
 범위를 가질 수 있으나 CPU가 직접적으로 접근할 수 없다.                                 대신에 상위의 부모 장치의
 드라이버가 CPU를 대신하여 간접적으로 접근하게 된다. 12C 장치를 보면. 각각의 장치가 주소를

                                                  30 / 312
 커널연구회佃ww.kernel.b기                                                정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                      2. Device Tree 소스 분석     31




가지고는 있으나 길이나 범위로 표현되지 않는다.                                      이것은 CPU를 주소 지정한 것과 같은
방식으로 다음과 같이 표현할 수 있다.                       아래 예제를 보자．


   i2c@1,O {
           compat 比기e = " acnie, a1234니2c나）us " ;
           #a（出打ess-cel Is = <]> ;
           #size-cel ls = <0> ;
           reg = <1 0 0x1000> ;
           rtc@58 {
               compat ible = 「maxim, ds1338'' ;
               reg = <58> ;
            };
       },
maxim의 ds1338 디바이스는 i2c 버스 상에서 주소가 필요하다.                              이것은 CPU의 로컬 버스 주소는
아니기 때문에 메모리 맵핑이 되지 않은 경우이다.                                    이런 경우에는 #ad打ess-ce小 와 ＃引ze-ce小
를 이용해서 하부에 대한 셀 수를 재 지정한다.                             이때는 길이에 대한 것이 없어진다．




2.3.4 Ranges 속성
지금까지 디바이스에 주소를 부여하는 방식에 대해서 설명했다.                                     하지만 지금까지 다룬 주소는 각
디바이스 노드의 관점에서 local 주소를 다룬 것이다.                                  아직까지 이러한 디바이스 幻cal 주소를
CPU가 사용할 수 있는 형태로 매핑하는 방법을 설명하지 않았다．


루트（/) 노드는 항상 CPU 관점에서 주소 공간을 기술한다.                                 루트의 자식 노드들은 항상 CPU 주소
공간을 사용하므로 또다시 명시적으로 매칭하지 않아도 된다.                                     예를들면, serial@10卄0000 장치는
직접적으로 0x10卄0000 주소에 할당된다．


루트의 직계 자식이 아닌 손자 노드들은 CPU의 주소 영역을 사용하지 못한다． 그러므로 주소를
변환하는 방식을 디바이스 트리에 도입하四F 하는데 ranges 속성이 그 역할을 한다．


12C 버스에 연결된 디바이스를 제어하기 위해서는 I2C 버스상에 표현되는 주소만 필요할 것이다．
CPU에 연결된 시리얼 디바이스라면 CPU와 연결된 로컬 버스상의 주소를 댜룰 것이다.                                          하지만
12C 버스에 연결된 디바이스를 CPU 입장에서 다룬다면, CPU는 로컬 버스 주소와 I2C 버스간에
변환 방법을 알아야 한다.                   왜냐하면 CPU 입장에서는 12C 버스의 주소 정보는 CPU의 로컬
버스에 적용할 수 없기 때문이다． 디바이스 트리의 루트 노드는 보드 그 자체이고 루트 노드의
주소는 CPU가 접근하는 주소 공간이다．                               그래서 모든 주소 정보는 CPU의 입장에서 해석
가능해먀 한다.          조금 더 구체적으로 이야기 하면, I2C 버스에 연결된 디바이스는 CPU의 주소

                                                    31 / 312
커널연구회（www.kern目b기                                                        정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니nux Kerr倒 4.0                                             2. Device Tree 소스 분석




공간에서 직접적으로 접근이 불가능하다.                               반드시 12C 컨트롤러를 이용하여 접근한다.                  즉 12C
버스에 연결된 디바이스는 I2C 버스에서 선택햐고 접근할 수 있는 주소 뿐만아니라 이런 정보를
적용할 12C 컨트롤러와 연관된 주소도 알려 주어야 한다． 물론 모든 디바이스가 이런 제한을
갖는 것은 아니다.               만약 serial 디바이스가 CPU 도메인 공간에서 접근할 수 있는 로컬 버스에
연결되어 있고 맵핑되어 있다면, serial 디바이스의 노드에 표현된 노드의 reg 속성에 있는 주소
정보는 CPU가 바로 사용할 수 있다.                            그러나 앞에서 예로든 l2C 버스에 연결된 디바이스는 CPU
가 접근 가능한 12C 컨트롤러와 관련된 부가 주소 정보를 더 제공하먀 한다.                                              정리하면, 모든
디바이스들은 각 디바이스 노드의 주소 도메인과 CPU의 주소 도메인간의 변환이 가능하도록
관련된 정보를 제공해야한다.                       이런 정보를 제공하는 것이 바로 ranges 속성이다.                         즉， 부모
도메인과 자식 도메인간의 주소 변환 정보를 이 ranges 속성을 통해서 제공하는 것이다.                                             아래의
예제는 ranges 속성을 설명하기 위해 추가한 것이다．



I{
     conipat ible = "acrne, coyotes-revenge" ;
     #address-cel ls = <1> ;
     #size-cel ls = <1>;

     external-bus {
         #address-cel Is = <2>
         #size-cel Is = <1>;
         ranges = <0 0 0x10100000        0x10000      II Chipselect 1, Ethernet
                    1 0 0x10160000       0x10000      II Chipselect 2, i2c control ler
                    2 0 0x30000000       0xl000000> ; II Chipselect 3, NOR Flash

         ethernet@O, O {
             compatible = 'smc, smcOlclll ";
              reg = <0 0 0x1000>;
         };
          i2c@1,O {
              compat 吐le = "acme, a1234시2c寸）us' ;
              #address-cel Is = <1> ;
              #size-cel ls = <0> ;
              reg = <1 0 0xi 000>;
              rt（廻58 {
                  compat ible = "maxim, ds1338 ' ;
                  reg = <58> ;

          },
          t lash@2, O {
                compatible = "samsung, k8f1315ebm" , "ct i- f lash";
                reg = <2 0 0x4000000> ;



};



                                                     32 / 312
커 널 연구회（www.kern飢bz)                                                          정재준 畇bi3307@nate.com)
Device Tree 상세분석 in 니nux Kern이 4.0                     2. Device Tree 소스 분석     33




ranges 속성은 주소 변환에 필요한 정보를 제공하는 리스트 구조이다.                    ranges 속성의 값은
다음과 같은 형식으로 표현한다．


        ranges = ＜자식주소］ 부모주소］ 자식주소크기］
                 자식주소2 부모주소2 자식주소크기2
                 자식주소3 부모주소3 자식주소크기3
                 자식주소4 부모주소4 자식주소크기4>;


위 형식에서 보듯이 자식주소, 부모주소, 그 자식들의 주소 공간의 크기의 묶음들의 리스트로
표현된다． 이 값을 지정하는 방식은 앞에서 설명했듯이 셀이라는 단위로 지정된다． 그렇다면 각
주소와 크기를 나타내기 위해서 몇개의 셀이 사용되는지를 지정하는 속성이 예상된다.                          실제로
사용은 이미 앞에서 설명한 reg에 사용된 것이 그대로 사용된다． 자식 주소와 부모 주소의 셀
수를 지정하는 것은 이전에 사용했던 #adc打e弱c이匕을 사용하고 크기의 셀 수를 지정하는 것
역시 ＃引ze｛이匕을 사용한다.           그런데 이 #address-cells 속성과 ＃引ze-cells은 부모용과 자식용이
따로 없다.     그렇기 때문에 부모 노드에서 지정한 #address-ce小 속성은 부모 주소의 셀수를
지정하고 자식 노드에서 지정한 #address-ce小 속성은 자식 주소의 셀수를 지정한다． 자식 주소
크기를 나타내는 셀 수는 자식 노드에 선언된 ＃읽ze-ce小 속성에 지정된 크기를 셀 수로 사용한다．


external-bus 노드에서 선언하는 ranges 속성에서 표시하는 자식 주소는 2개의 셀을 갖는다．
부모 주소는 ] Il의 셀을 갖고 크기 역시 ］개의 셀만을 사용하게 된다.                   그래서 위 예제에서
ranges 속성에 첫번째 주소 변환 정보인


       ranges = <0 0   0x10100000    0x10000


이것은 0과 0이 자식 주소 정보이고 0xl 0100000은 부모 즉 CPU 입장에서 로컬 버스 주소가
되고 0x10000은 자식 주소 크기가 된다.               이것을 외부버스에 대한 해석을 한다면 다음과 같이
해석 된다．


       칩 셀렉트 0 번의 오프셋 0은 小<1아00000..0xl0lOffff 의 주소 범위로 맵핑된다．
       칩 셀렉트 ] 번의 오프셋 0은 0x10160000..0x1016ffff 의 주소 범위로 맵핑된다．
       칩 셀렉트 2 번의 오프셋 0은 0x30000000..0x30ffffff 의 주소 범위로 맵핑된다．


만약 부모와 자식 주소 공간이 동일하다면， 값이 빈 ranges 속성을 사용할 수 있다．                     값이 빈
ranges 속성이 있다는 것은 자식의 주소 공간과 부모의 주소 공간이 ］·．］로                  맵핑된다는 것을
의미한다．     ]:] 맵핑 되는 경우0伍 ranges 속성을 사용해서 주소 변환 정보를 졔공할 필요가
있을까 하는 궁금증이 생길수 있다.                 이런 경우의 예로 로컬 버스와 전혀 다른 주소 공간을 갖는


                                         33 / 312
커널연구회（ww比kernel.b기                                    정쟤준 (r야)i3307@r伯te.com)
Device Tree 상세분석 in 니flux Kernel 4.0                   2. Device Tree 소스 분석     34




PCI 같은 특정 버스는 운영체제입장에서 로컬 메모리 공간으로 맵핑되어야 하고 보여야 한다.                        또
다른 경우라면 어떤 디바이스는 DMA 엔진을 갖을 수 있는데 이와 관련된 처리를 하려면 실제
버스 상의 물리적 주소값을 알 필요가 있다.                 디바이스들이 동일한 소프트웨어적으로 프로그램
가능한 물리적 주소를 모두 공유하는 경우에 디바이스는 서로 구룹 지어질 필요도 있기 때문이다．
어떻든지 간에, ]:] 맵핑은 운영체제가 필요로 하거나 하드웨어 디자인에 따라서 필요하고
사용된다.      여러분은 i2c@1,0        노드에 ranges 속성이 없음을 알려야 합니다．          그 이유는
외부버스와 다르게, i2c 버스위에 있는 디바이스는 CPU 주소 영역에 메모리 주소 맵핑을 할 수
없기 때문이다.        대신에, CPU는 rtc@58 디바이스는 12c@1,0 를 통해서 간접적으로 접근한다．
ranges 속성이 없음은 해당 디바이스의 부모 이외엔 어떤 디바이스도 직접적인 접근을 할수
없음을 의미합니다．




2.4 인터럽트 표현
주소 범위 변환은 디바이스 트리 구조내에서 트리 구조로 계증화 표현이 가능 하지만, 인터럽트
신호는 머신의 특정 장치에서 발생하여 그 장치에서 종료된다.                    디바이스 트리에 구조적으로
표현된 주소 접근 장치와는 다르게, 인터럽트 신호는 디바이스 트리와는 독립적인 노드들에
연결되는 방식으로 표현된다.               보통 인터럽트는 디바이스의 하드웨어가 인터럽트를 발생하고
인터럽트 컨트롤러가 해당 신호를 수신하는 구조로 되어 있다.                    그래서 인터럽트는 디바이스
트리의 구조와 별도로 디바이스 노드간에 링크 구조로 표현된댜.                    인터럽트는 디바이스 노드의
속성 형태로 표현한다.           인터럽트 간의 연결을 표현하기 위해서 4개의 속성이 있으며 아래에
이들에 대해서 정리한다.



如tm恥的如抑甘
interrupt-contr히1er 속성은 값이 없는 빈 속성으로 해당 노드의 디바이스가 인터럽트 신호를
수신하는 인터럽트 컨트롤러 디바이스 임을 표현한다．




interrupt-parent 속성을 통해서 라벨 참조 형태로 지정하는 디바이스를 디바이스 트리의 계층
구조에서 가장 상위의 인터럽트 컨트롤러로 정의 하게 된다.                  interrupt-parent 속성을 갖지 않은
노드들은 그들의 부모 노드중 interrupt-parent 속성이 선언된 노드의 interrupt-parent 속성을
상속 받는다．




쒸riterrupt-celIs 속성에 지정된 값은 interrupts 속성에서 인터럽트에 대한 정보를 속성값으로

                                       34 / 312
커널연구회（www.kern이b기                                     정쟤준 (rgbi3307@nate.com)
Device Tree 상세분석 ir} 니nux Kerr倒 4.0                             2. Device Tree 소스 분석      35




표현할때 사용될 셀수를 나타낸다（#address-cells오F #size-cells고f 비슷한 역할임）.                   interrupt-
controller 속성이 선언된 노드에 같이 선언한다．



km 1批
interrupts      속성은 디바이스가 발생하는 인터럽트 출력 신호에 대한 정보의 리스트를 값으로
표현한다．


interrupts의 속성에 표현되는 한개의 인터럽트에 대한 정보는 여러개의 셀로 구성된다.                                 이
인터럽트는 인터럽트 컨트롤러에 연결된 인터럽트 입력에 관란 정보이다．                                 아래 예제를 보면
대부분의 디바이스는 보통 하나의 인터럽트 출력만 있다.                              그러나 어떤 디바이스는 여러개의
인터럽트 출력이 있을 수 있다.                          interrupts의 속성 값에 지정되는 정보의 의미는 인터럽트
컨트롤러에 의존적이다.                    인터럽트 콘트롤러마댜 인터럽트를 다루기 위한 나름대로의 특성이
있으므로 이에 맞는 것으로 정의하고 이에 따라서 셀수가 결정된다．


아래 코드는 위에서 계속 예제로 사용하고 있는 Coyote's Revenge 샘플 장치에 인터럽트와
관련된 것을 추가한 것이다．



 I{
      corn口at 比니e = "acme, coyotes中revenge " ;
      #address-cel ls = <1> ;
      #size-cel Is = <1> ;
      interrupt-parent = <&intc>;

      cpus {
          #address-cel Is = <1> ;
          #size-cel Is = <0> ;
          야）u@0 {
              compat ible = "arrn, cortex-a9";
              reg = <0> ;
           };
           야）u@1 {
               compat ible = "arm, cortex-a9";
               reg = <1>;

      };
           };
      ser ial@101t0000 {
           compat 吐니e = "arm , 이011「 '
           reg = <OxlOlf0000 0x1000 >;
            interrupts = < 1 0 >;
      };
      serial@101t2000 {
           compat 山le = "arm , 이011 "
           reg = <0x101t2000 oxl000 >;

                                                 35 / 312
커 널 연구회（ww比kernel.b기                                           정재준 什gbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                            2. Device Tree 소스 분석   36




         interrupts = < 2 0 >;
   };
   gpio@101f3000 {
       corn口atib陀 = "arm , 히06尸 ;
       reg = <0x101f3000 0x1000
               0xiOl f 4000 0xOOlO> ;
        interrupts = < 3 0 >;
   };
   intc: interrupt-control Ier@10140000 {
       compatible = "arm,p너9o느
       reg = <0x10140000 0x1000 >;
       interrupt-control ler;
       #interrupt-cel Is = <2>;
   };
   spi@10115000 {
       compatible = "arm,p1022";
       reg = <0x10115000 0x1000 >;
       interrupts = < 4 0 >;
    };
   external-bus {
       #address-cel ls = <2>
       #size-cel ls = <1>;
       ranges = <0 0 0x10100000           0x10000     II Chipselect 1, Ethernet
                  1 0 0x10160000          0x10000     II Chipselect 2, i2c control ler
                  2 0 0x30000000          0xl000000>; II Chipselect 3, NOR Flash

         ethernet@0,0 {
             compatible = "smc, smc9lclll ";
              reg = <0 0 0xl000>;
              interrupts = < 5 2 >;
         };
         i2c'@1,0 {
              compatible = "acme,a1234니2c由四n ;
              #address-cel Is = <1>;
              #size-cel ls = <0>;
              reg = <1 0 0xl000>;
              interrupts = < 6 2 >;
              rtc@58 {
                  compatible = "maxim, ds1338";
                  reg = <58> ;
                  interrupts = < 7 3 >;
              };
         };
         f I asr他2, 0 {
               compatible = "sarnsung, k8f1315ebrn" , 'cf i- f lash'' ;
               reg = <2 0 0x4000000>;
         };



                                                       36 / 312
커 녈 연구회（ww＼사．kernel.b기                                                        정재준 (rg너3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                       2. Device Tree 소스 분석     37




위의 예제를 통해서 주목해먀 할 몇가지가 있다.                    위의 코드에서 표현하고 있는 샘플 장치에는
노드 이름이 interrupt-controlle恒)10140000로 지정된 한개의 인터럽트 컨트롤러를 가지고 있다．
여기서 특이하게 'intc:' 라고 하는 라벨이 인터럽트 컨트롤러 노드에 추가된 것을 볼 수 있다.                        이
라벨은 루트 노드에서 interrupt-parent 속성으로 사용한다．


       interrupt-parent = <&intc>;


이 interrupt-parent 속성 값은 시스템의 디폴트 인터럽트 컨트롤러를 지정한다.                   자식 노드들은
해당 인터럽트를 수신하는 것이 어떤 것인가를 지정하지 않고 상위 노드에서 interrupt-parent
속성으로 지정된         인터럽트 컨트롤러를 해당 디바이스 노드에                   연결된   인터럽트 컨트롤러를
디폴트로 선택한다.         왜냐하면 모든 자식 노드들은 해당 속성을 쓰지 않아도 상위 노드에 지정된
interrupt-parent 속성에서 상속되기 때문이다.          각 디바이스의 interrupts 속성은 각각의 인터럽트
입 력 라인을 기술하기 위해서 사용한다.                   이때1 인터럽트 컨트롤러를 표현한 노드에 정의된
荊nterrupt-ce小 속성은 interrupts 속성에서 하나의 인터럽트를 기술하기 위한 셀 수를 지정한다．
위 예에서 "# jnterr叩卜cells"은 2개이다..        그래서 하나의 인터럽트 입력을 표현하기 위해서는 2
개의 셀이 필요하다．           위의 예제에서는 인터럽트 라인 번호를 표현하기 위해서 첫번째 셀이
쓰이고. 두번째 셀은 액티브 되는 인터럽트 레벨의 조건이 레벨 하이인지 로우인지 엣지인지를
나타낸다.     여러분이 다루고자 하는 인터럽트 컨트롤러에 인터럽트 입력에 대한 부분을 다루고자
한다면 해당 인터럽트 컨트롤러의 매뉴얼을 참조하기 바란다．



2.5 사용자 추가 데이터
지금까지 댜룬 일반적인 속성 이외에 여러분이 필요하다고 생각되는 임의의 속성이나 자식
노드들을      노드에 포함시킬 수 있다.               만약에 디바이스 트리에 여러분이 다루는 운영체제에서
필요로 하는 어떤 데이터를 추가 하고 싶다면 다음과 같은 규칙을 준수하여 추가 하기 바란다．


첫째, 새로운 디바이스 노드에 추가할 속성 이름은 표준 속성 이름과 충돌을 방지하기 위해서
제조사 접두사를 붙여야 한다．


둘째, 속성의 의미와 자식 노드에 대한 것은 운영체제의 디바이스 드라이버 개발자가 해당 내용을
이해할 수 있도록 바인딩 문서에 문서화 하기 바란다.                        여기서 디바이스 트리에서 바인딩이라고
하는 의미는 디바이스 트리 안에서 디바이스가 표현되는 것을 의미한다.                             바인딩관 관련되어
기술되는 문서에는 해당 디바이스 노드에 새로 만들어지는 속성은 어떤 의미인지 , 속성은 어떤
값을    가질수     있는지,     자식     노드를      가지고   있는지 ,    기술하고자   하는   디바이스가     어떤
디바이스인지가 표현되어야 한다.                    디바이스를 표현하는 노드 각각은 compati비e 속성 값에


                                        37 / 312
커널연구회（www.kerne냐）기                                        정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0               2. Device Tree 소스 분석




각각이 서로 구별될 수 있는 고유의 문자열을 사용해먀 한다.                 새로운 디바이스들에 대한
바인딩은 이 문서가 있는 사이트의 위키에 문서화 되어야 한다.                 아울러, 문서 형식과 검토
프로세스에 대해서 설명하는 메인 페이지를 참조하기 바란다．


세째， devicetree-discuss@小ts.o기abs.org 메일링 리스트에 새로 만들어진 바인딩과 관련된 검토
내용을 제출하기 바란다. 포스팅을 하면 나중에 발생할 수 있는 많은 예상되는 문제들 중 공통된
실수를 해결해 나갈 수 있다．




2.6 특별한 노드들


2.6.1 aliases 노드
어떤 노드는 노드 이름으로 /external-bus/ethernet@0,0 와 같이 전체 명칭 즉 긴 이름을
사용한다.      또는 이러한 긴 이름보다는 ethO와 같은 짧은 이름을 선호할때가 있다.                그래서
디바이스 트리를 볼 때 "eth0가 무슨 디바이스일까7" 라는 생각으로 보게 된다.               이런 경우들에
대해서 디바이스 트리는 帥ases 라는 노드를 제공하여 쉽7朴 긴이름을 짧은 이름으로 치환하게
하거나 일반적으로 알수 있는 용어로 바꾸어 사용할 수 있도록 해줄 수 있다.               예를들면，



   al iases {
        ethernetO = &ethO;
        seria山 = &serialo;
   };
즉 ethernetO는 ethO라는 이름과 같다는 것을 표현해 줄 수 있다． aliases 안에 기술되는 형식은


         별칭 = ＆라벨．
                 ,


형태가 된다.       이런 문법 표현은 별칭에 해당하는 문자열을 라벨에 대한 참조로 사용할 수 있도록
한다.     이런 표현은 운영체제가 디바이스의 식별자를 부여하는 방법으로 환영할 만한 것이다．
그리고 위 표현 방법의 의미는 interrupt-parent 속성 값을 표현 할때 사용했던 '＜釗abel> '과는
다른 것임을 주의하자．




                                       38 / 312
커널연구회佃ww.kern이.b기                                 정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                2. Device Tree 소스 분석    39




2.6.2 chosen 노드
chosen 노드는 실제 디바이스를 디바이스 트리에 표현하는 것은 아니다.                                                단지 , 부트 아큐먼트와
같이       펌웨어0私］          운영      체제에        전달된        데이터를         파씽하기        위한        방법으로    제공된다．
일반적으로           .dts   소스      파일들내에          기술된       chosen     노드는         왼쪽    키    부분이    비어   있다．
그리고 그 정보는 부팅 동안만 유효하다．                              예제     시스템에서          펌웨어는 chosen 노드를 다음과
같이 추가 하도록 한다．


chosen {
           bootargs = "rootr/ dev/ nfs rw nfsroot=192. 168.1.1 console=ttyS0,115200 " ;
    };




2.7 진보된 주저匿


2.7.1 진보된 장치 예제
지금까지 디바이스 트리를 이해하기 위한 기본적인 정의만 다루었지만, 이제 좀 더 디바이스
트리를 완벽하게 사용하기 위해서 좀 더 진보된 하드웨어를 샘플에 추가 하고자 한다.                                                        이런
복잡한 하드웨어로 PC! 호스트 브릿지가 있다.                                  이것을 샘플로 추가하1 보자．                 이 PCI 호스트
브릿지는 0x10180000률 제어 레지스터 주소로 갖고 0x80000000 주소를 BARs 영역의 시작
주소를 갖는 것으로 가정한다.                       지금까지 사용한 예제에 다음과 같은 PCI 호스트 브릿지 노드를
추가하는 것으로 설명을 시작한다．


           pci@10180000 {
                compatible = "arm, versat i 1 e-pci-hostbr idge " , 'pci ' ;
                reg = <0x10180000 0xl000> ;
                interrupts = <8 0>;
           }


위의 예를 보면 PCI 호스트 브릿지는 제어를 위한 주소가 reg 속성으로 0x10180000 번지부터
크기는 0x1000의 범위를 가진다.                      이 번지영역을 이용하여 호스트 브릿지를 제어하게 된다.                               이
호스트 브릿지는 시스템 인터럽트에 8번 인터럽트를 통해서 인터 럽트 처리를 하게 된다．




                                                     39 / 312
커 널 연구회（www.kerne나끄）                                                            정재준 (rgbi3307@nate.corr卄
Device Tree 상세분석 in Linux Kernel 4.0                                        2. Device Tree 소스 분석      40




2.7.2 PCI 호스트 브릿지
이 섹션은 Host/PCI 브릿지 노드에 대해서 설명한다.                             사전에 양하1 드리고 싶은 것은 이 섹션을
설명할 때 여러분은 이미 PC뻬 대한 기본 지식이 있을 것이라는 가정을 두고 있다.                                          이 문서는
PCI에 대한 학습문서가 아니기 때문에 PCI(게 관련된 내용은 다른 곳에서 도움을 얻기 바란다．
ePAPR나 Open Firmware(htt口：사나WW. openf i rmware. o四／oh四化In帥gs/pci /pci2j ,pdf ) 의 PCI Bus
미nding에 대한 것을 참조 하면 많은 도움이 될것이다.                               필자는 여기에 있는 내용을 일부
챰조하여 PC를 디바이스 트리로 어떻게 표현하는지 이해하고자 했다．


먼저 , PCI 버스 번호를 처리하기 위해서 추가된 아래의 예제를 보도록 하자．


         pci@0x10180000 {
              compatible = " arm, versati le-pci-hostbridge " , 'pci ' ;
              rep = <0x10180000 0x1000>;
              interrupts = <8 0>;
              bus-ranges = <0 0>;
         };
보통 각각의 PCI 버스들은 해당 버스에 유일한 번호가 매겨진다.                                       이 버스에 번호를 부여하기
위해서 두개의 셀을 포함하는 bus-ranges 속성을 사용하여                                  디바이스 트리내에 PCI 노드가 표현
된다． 이 bus-ranges 속성 값의 첫번째 셀은 이 노드에 부여된 버스 번호이다.                                    즉, 0번 버스라는
의미가 된다． 두번째 셀은 하부의 PCI 버스들 중애서 가장 큰 번호를 표현한다.                                           샘플 장치는
하나의 PCI 버스만을 가지기 때문에 이 값은 0이 된다．



2.7.3 PCI 주소 변환
앞에서 댜루었던 외부 버스 공간과 비슷하게, PCI 주소 공간도 CPU 주소 공간과 하드웨어 적으로
완벽하게 분리되어 있다.                 그래서 PCI 주소에서 CPU 주소를 얻기 위해서 주소 변환이 필요하다．
이 주소 변환에 사용하는 속성은 앞에서 이미 설명했던，


ranges
#address-cells
＃引ze-ce小


위의 속성들을 사용한다．                   아래는 ranges 속성의 의미를 한번더 정리한 것이C卜（위에서 이미

                                                  40 / 312
커널연구회佃w比kernel.b기                                                          정재준 (rgb13307（包nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                             2. Device Tree 소스 분석     41




설 명 했음）


ranges = ＜자식주소1 부모주소］ 자식주소크기］
             자식주소2 부모주소2 자식주소크기2
             자식주소3 부모주소3 자식주소크기3
             자식주소4 부모주소4 자식주소크기4>;


이들을 이용해서 주소 변환을 표현하는 예제를 보도록 하자．


       pci@0x10180000 {
           compat ible = 'arm, versat i le-pci-hostbridge " , " pci '' ;
           reg = <0x10180000 0x1000>;
           interrupts = <8 0>;
           bus-ranges = <0 0>;

             #address-cel Is = <3>
             #size-cel Is = <2> ;
             ranges = <0x42000000 0 0x80000000 0x80000000 0 0x20000000
                        0x02000000 0 0xa0000000 0xa0000000 0 0x10000000
                        0x01000000 0 0x00000000 0xb0000000 0 oxOl000000> ;
       };
위의 예제를 보면, #a由打ess-cells 속성에 표현한 것처럼 자식주소］(PCI 주소）는 3개의 셀을
사용한댜．


0x42000000     0   0x80000000       //phys.hi     phys.mid     phys. low


그리고, 부모주소］은 ]211 셀을 사용한다.                        이것은 이미 상위 노드에서 정의한 것이다．


0x80000000


그리고, ＃引ze-ce小 속성에서 정의한 것처럼 자식주소l의 크기（PCI 범위）는 2개의 셀로 표현된다．


0 0x20000000


우선. 자식주소］(PCI 주소）를 표현하기 위해서 32비트 셀이 세개가 필요한지 궁금할 것이다.                                                이
세개의         셀들은     다음과      같이      phys.hi,   phys.mid     그리고           phy引ow의   순서대로   나열한    자식
주소값이 다．


 phys.hi cel l : npt000ss bbbbbbbb dddddfff rrrrrrrr

                                                    41 / 312
커널연구회佃ww.kernel.bz)                                                             정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                        2. Device Tree 소스 분석    42




phys.mid cel l : hhhhhhhh hhhhhhhh hhhhhhhh hhhhhhhh                                //MSB
ptys. I0w CeI I : I I I I I I I I I l l I l I l l l I I I I I I I I I I I l I I I   IILSB


PCI 주소는 64비트 주소폭을 갖는다.                                    그래서 phys.mi미MSB）와 phy引ow(LSB）가 ranges 속성값 중
진짜 자식주소로 사용된댜.                                 64비트 주소폭 중에서 상위 32비트는 phys.mid（卜ASB）이고 하위
32비트는 phys.Io叫LSB）가 된다.                            그런데, 여기서 조금 복잡하지만 알아 두어야 할것은 phys.high
이다.        이것은 다음과 같은 비트 필드로 구성되어 있다．


n : 工H 배치 가능영역 표시（0이면 재배치 가능, ］이면 불가능）

P : 프리펫치 가능 영역 표시（］이면 프리펫치 가능, 0이면 불가능）
t : 어드레스 정렬 표시
ss    ·. 영역 구분 코드
             00 : 환경 설정 영역
             01     ·. I/o 영역
             10 :32 비트 메모리 영역
             11 :64 비트 메모리 영역


bbbbbbbb : 8비트 PCI 버스 번호, PC七 계층적으로 구성된다．
                    그래서 서브 버스로 정의될 수 있는 PCI/PCI 브리지를 가질수도 있다．
ddddd           : 5비트 디바이스 번호, 보통 IDSEL 신호와 연결되어 있다．
ff1             :3비트 기능번호, PCI 디바이스가 여러 기능을 가지고 있을 경우 사용된다．
rrrrrrrr        :8비트 레지스터 번호, PCI 환경 설정 단계에서 사용된다．


PCI 주소 변환의 목적상 가장 중요한 필드들은 P와 ss 이다. phys.hi 안에 있는 P와 ss의 값은
PCI 주소 공간이 어떤 특성이 있는지를 나타낸다.                                                 몇가지 예를들면，


ss = 00 일때1, 환경설정을 표현하므로，
n,p,t는 각각 0이 되어야 하고，
bbbbbbbb,ddddd,fff,rrrrrrrrr는 환경설정 공간의 주소이고，
hh...hh,II...Il은 0이 되어야 한다．


 ss = 0] 일때1, I/O 공간을 표현하므로，
P는 0이 되어야 하고，
 bbbbbbbb,ddddd,ffl,rrrrrrrrr는 영역의 기준 주소 레지스터를 식 별하고，
 hh...hh는 0이 되어야 하고
 n=］이면 n...n은 I/O 공간의 주소가 된다．

                                                                    42 / 312
 커 널 연구회（
        ＼們們사kerne比기                                                                         정재준 內bi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                            2. Device Tree 소스 분석   43




ss = 10 일때1,32비트 주소공간 메모리를 표현하므로，
hh...hh는 0이 되어야 하고
n=］이면 II...II은 메모리 공간의 32비트 주소가 된다．


ss = 1] 일때, 64비트 주소공간 메모리를 표현하므로，
t=0이 되어야 하고，
n=］이면 hh...hh,Il...ll은 메모리 공간의 64비트 주소가 된다．


이제 위의 샘플에 기입된 ranges 속성에 있는 값을 해석하면 다음과 같이 세가지 영역에 대한
것을 기술하고 있다．


PCI 주소 0x80000000를 시작주소로 갖고 32비트 프리페치 가능한 512卜기Byte 크기의 메모리
영역은 호스트 CPU의 0x80000000에 맵핑된댜．


PCI 주소 0xa0000000를 시작주소로 갖고 32비트 프리페치가 불가능한 256MByte 크기의 메모리
영역은 호스트 CPU의 0xa0000000에 맵핑된다．


PCI   주소   0x00000000를   시작주소로         갖는   16卜4Byte   크기의    I/O   영역은   호스트   CPU의
0xb0000000에 맵핑된다．


운영체제 입장에서 보면 phys.hi 비트 필드는 해당 노드를 PCI 브릿지의 영역으로 다룰때
주소변환 목적에 상관없는 필드는 무시할 수 있고 이와 관련된 정보 정도만 필요로 한다.                                그래서
주소 변환 목적에 상관없는 필드는 무시할 수 있다.                       경우에 따라서 어떤 운영체제는 추가적인
필드의 마스크에 대한 것이 필요할 수 있다.                     이때 운영체제는 해당 필드 마스크 값을 얻기
위해서 PCI 버스 노드에서 "PC尸 문자열을 이용해서 찾을 것이다.                        이런 경우라면 필요한 phys.hi
비트값들을 기입할 필요도 있다




2.7.4 진보된 인터럽트 매핑
이제 가장 흥미로운 부분인 진보된 인터럽트 매핑까지 왔다.                             PCI 디바이스는 判NTA, 判NTB,
判NTC,   判NTD 라고 불리는 네개의 신호선을 이용하여 인터럽트를 트리거 할수 있다.                                만약
하나의 PCI 디바이스가 여러가지 기능을 가지고 았지 않다면 인터럽트를 判NTA만 사용할 것이다．
그러나, 각 PCI 슬롯 또는 디바이스 입장에서 동일한 인터럽트가 나가지만 인터럽트 컨트롤러에는
다른 입력으로 연결되어 있다.             보통 하드웨어적으로            인터 럽트 네개의 라인을 한 라인씩 시프트


                                        43 / 312
커널연구회（ww比kernel.b기                                            정쟤준 (rgb日307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                             2. Device Tree 소스 분석   44




되는 방식으로 연결한다.                 예를들어 첫번째 슬롯의 判NTA는 PCI 인터럽트 컨트롤러에 判NTA로
연결되지만 두번째 슬롯의 判NTA는 PCI 인터럽트 컨트롤러에 쒸NIB로 연결되고 세번째 슬롯의
쒸NIA는 PCI 인터럽트 컨트롤러에 ＃小JIC로 연결된다.                               다른 인터럽트 역시 이와같이 쉬프트 한
상태로 연결된다.           이런 연결 특성을 표현하기 위해서 디바이스 트리는 각 PCI 인터럽트 신호를
인터럽트 콘트롤러에 맵핑하는 방법이 필요하다.                                 이런 복잡한 인 터럽트 매핑에 관련된 속성은
다음과 같은 것이 있다．


쒸nterrup卜ce小
interrupt-map
interrupt-map-mask


이 속성들이 PCI 인터럽트 맵핑을 기술하는데 사용될 수 있다.                                       사실 , 이 속성들은 PCI 버스의
인터럽트 매핑에 한정되어 사용되는 것은 아니다.                               이 속성들은 복합적인 인터럽트 맵을 기술할때1
필요해서 정의된 것이지만, 주로 PC떽 인터럽트 같이 복잡한 인터럽트 매핑을 다룰따1 사용 된다．
아래에 이런 복잡한 PCI 인터럽트 매핑에 대한 예제가 있다．



       pci@0x10180000 {
           compatible = "arm, versati le-pci-hostbr idge " , 'pci " ;
           reg = <0x10180000 小l000> ;
           interrupts = <8 0>;
           bus-ranges = <0 0>;

            #address-cel Is = <3>
            #size-cel ls = <2> ;
            ranges = <0x42000000 0 0x80000000      0x80000000   0 0x20000000
                       0x02000000 0 0xa0000000     0xa0000000   0 0x10000000
                       0x01000000 0 0x00000000     0xb0000000   0 0x0l000000>;

            #interru口t-cel ls = <1> ;
            interrupt-map-mask = <0xf800 0 0 7> ;
            interrupt-map = <0xc000 0 0 1 &intc 9 3 II 1st slot
                              0xc000 0 0 2 &intc 10 3
                              0xc000 0 0 3 &intc 11 3
                              0xc000 0 0 4 &intc 12 3

                              0xc800 0 0 1 &intc 10 3 II 2nd slot
                              0xc800 0 0 2 &intc 11 3
                              0xc800 0 0 3 &intc 12 3
                              0xc800 0 0 4 &intc 9 3> ;
       };


이 중에서 가장 먼저 interrupt-map 속성을 설명한다.                           댜음 내용을 이해하기 전에 복잡한
인터럽트 매핑에 대한 정확한 작업 표현 방법은 "Open Firmware Recommended Practice:


                                                  44 / 312
커 널 연구회（www.kernel.b기                                                       정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                              2. Device Tree 소스 분석      45




Interrupt Mapping"( htt口：I/ www. openf i rmware .or이俚75巾ra아 IC이a叩/ i ma沁_9d. pdf )롤 참조하기
바란다． 이 내용을 살펴보면 interrupt-map 속성은 다음과 같은 형식을 가진다．


interrupt-map = < 자식오J터럽트4정보］ 부모m인터럽트4컨트롤러정보l                        부모오J터럽트H정보］
                      자식 인터럽트e정보2       부모m인터럽트1컨트롤라 정보2             부모 인터럽트 정보2
                      자식e인터럽트m정보3       부모인터럽트H컨트롤러H정보3              부모e인터럽트1정보3


                 >;
위 예제의 한 부분인


interrupt-map = <Oxc000 0 0 1 &intc   9 3


에서 정의한 엔트리


0xc000 0 0 1 &intc    93


를 위 정의에 대입하면，


0xc000 0 0 1     /／자식 인터 럽트 정보］
&intc            /／부모 인터럽트 컨트롤러 정보］
93               /／부모 인터럽트 정보］


에 해당한다．


자식 인터 럽트 정보］를 표현하기 위해서 사용하는 셀 수는


#address-ce小； = <3>
쒸nterrup卜ce小 = <] >


위와 같이 지정되어 있는 것을 알 수 있다．


여기서     #ad如e弱．ce小로        표현된   주소     정보가      어떤    의미인지는 뒤에서         자세하게       설명한다．
料nterrupt-ce小로        표현되는 것은 자식            인터럽트의      번호를   의미한다．      보통    PCI   디바이스
하드웨어의 인터럽트 번호를 의미 하는데 0으로 시작하지 않고 ］로 시작되는 것에 주의하기
바란다.     PCI 하드웨어 인터럽트 번호는 1부터 시작한다.                    이 PCI 주제 이전에 시스템 인터럽트를


                                            45 / 312
커널연구회佃ww.kernel.b기                                              정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니nux Kernel 4.0                                     2. Device Tree 소스 분석    46




설명할 때, 시스템 인터럽트는 IRQ번호와 해당 인터럽트의 검출 방법에 정보가 필요하기 때문에
인터럽트의 정보를 표현할 셀 수를 쒸nterrupt-cells 속성을 이용하여 2개의 셀을 지정했다．
그러나 PCI 인터 럽트의 검출은 항상 로우 레벨일 경우만 검출되는 것으로 규정되어 있기 때문에
위의 예에서 보듯이 PCI 인터럽트는 ]7H의 셀만 지정하고 있다．


이제 이 자식 디바이스 인터럽트를 받는 부모 인터럽트 컨트롤러 정보를 표현하고 있는 부분을
살펴보자.          예제를 보면 &intc로 표현하고 있다.                       이것은 앞의 예제에 이미          다음과 같이
표현했을때1,



     intc: interrupt-control Ier@10140000 {
            compatible = "arm,p너90' ;
            rep = <0x10140000 0x1000 >;
             nterrupt-control ler ;
             #interrupt-cel ls = <2>;
     };
인터럽트 컨트롤러로 라벨 intc를 참조 하도록 표현한 것이다．                                이 표현에서 주의 깊게 보아야

하는        것은    쒸nterrupt-ce小       속성이다.           이것은      interrupt寸nap   속성의    엔트리    중
부모 인터럽트정보］를 지정하는 셀 수로 사용된다．


#interrupt-ce小 = <2>


로 지정했기 때문에 부모 인터럽트 정보］을 표현하기 위해서 2개의 셀을 사용한다는 것을 알 수
있다.       위 예에서 보듯이 2개의 셀을 사용해서 표현하고 있고，


93


이것의 의미는 인터럽트 번호가 9번이고 PC땍 인터럽트 검출 레벨은 항상 로우 액티브 이므로
이것에 대한 표현 값으로 3을 지정하고 있다．


이제 #address-ce小로 표현된 주소 정보가 어떤 의미인지를 설명한다.                                   위의 예를 보면 이
디바이스 트리가 표현하는 샘플 보드는 interrupt-map 속성의 주석을 보시면 알수 있듯이 4개의
인터럽트를 가지는 2개의 PCI 슬롯을 가지고 있음을 알수 있다． 그래서 8개의 인터럽트 라인을
인터럽트 콘트롤러에 매핑해야 한다.                           하나의 PCI 버스상에서 각 PCI 디바이스들은 判NTA 등과
같은 인터럽트 라인을 4개만 가지고 있다.                            그래서 인터 럽트가 발생했을따1 어떤 디바이스의
인터럽트인지 구별하는데 문제가 있다．                           다행스럽게도, 모든 PCI 디바이스는 사용가능한 유일한
디바이스 번호를 가지고 있다.                   그래서 이 디바이스 번호를 추출하먀 하는데                    이것은 앞에서 다룬

                                                 46 / 312
커널연구회佃w毗emn이b라                                                        정쟤준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                 2. Device Tree 소스 분석     47




다음과 같은


phys.hi    셀 값의 의미 : npt000ss bbbbbbbb dddddfff rrrrrrrr
phys.mid 셀 값의 의미 : hhhhhhhh hhhhhhhh hhhhhhhh hhhhhhhh
phy引ow 셀 값의 의미 : 111111n 川11111 11111111 11111111


주소 정보 중에서              phys.hi의    정보중 디바이스              번호의 비트    필드 정보가 필요하다． 앞에서
설명했던 부분을 다시 한번 나열하1 보면，


n                   : 재 배치 가능영역 표시

p                   : 프리펫치 가능 영역 표시
t                   : 어드레스 정렬 표시
S                   : 영역 구분 코드
           00       : 환경 설정
                                                               的
                                                               的
           01       : I/O 영역
           10       : 32 비트 메모리 영역
           ]]       : 64 비트 메모리 영역
bbbbbbbb            : 8비트 PCI 버스번호． PCI는 계층적으로 구성된다．
                     그래서 서브 버스로 정의될 수 있는 PCI/PCI 브리지를 가질 수도 있다．
ddddd               : 5비트 디바이스 번호, 보통 IDSEL 신호와 연결되어 있다．
ff1                 : 3비트 기능 번호． PCI 디바이스가 여러 기능을 가지고 있을 경우 사용된다．
rrrrrrrr            .8비트 레지스터 번호 : PC 환경 설정 단계에서 사용된다．


이 중에서


ddddd               : 5비트 디바이스 번호, 보통 DSEL 신호와 연결되어 있다．


부분이 필요하다.             이 부분의 정보를 다루기 위해서 #ath打ess-cells(게 지정된 셀 수의 정보를
나열한 것이다． 이따1 디바이스 번호의 비트 필드 이외에는 필요 없는 정보이므로 필요한 ddddd
정보 영역에 대한 것만 다음과 같이 나열한 것입니다．


0xc000 0 0


여기서 이 주소 정보의 셀은


#address-cells = <3>


                                                    47 / 312
커널연구회（www.kernel.b기                                                 정쟤준 仕9bi3307（孕nate.com;
Device Tree 상세분석 in Linux Kernel 4.0                      2. Device Tree 소스 분석     48




로 지정하고 있다.          여기에 이 주소를 비트 마스크 하여 원하는 비트의 유효범위를 지정하기
위해서，


interrupt-map-mask = <0xf800 0 0 7>;


와 같이 지정햐고 있는데


0xf800 0 0


는 주소 정보를 추출하기 위한 비트 마스크 값이고


7은 인터럽트 번호를 추출하기 위한 비트 마스크 값이 된다.                       이 마스크 값을 가지고 AND
논리연산 한다．


이제 interrupt-map 속성을 좀 더 설명하고자 한다.                  개별적인 PCI 디바이스의 인터럽트률
구별하기 위해서는 PCI 디바이스 번호와 PCI 인터럽트 번호로 구성된 묶음이 필요하다.                          좀 더
쉽게 이야기 하면, 4개의 셀을 가지고 있는 자식 디바이스의 인터럽트 정보 값을 만들어야 한다．


phys.hi, phys.mid, phys.low의 각각에 해당하는 값을 기술하고 이를 위해서 #ad打ess-cells 속성
값은 3으로 지정하고 있다.            判NTA, 判NIB, 判NTC, 判NTD중 하나를 지정하기 위해서 荊nterr叩t
cell 속성 값은 ］로 지정하고 있다.             interrup卜map-mask 속성은 자식 디바이스 인터럽트 정보와
같이 4개의 셀로 구성된다．              마스크 값의 각 비트들을 ］로 사용하여 필드의 비트중 유효한
비트임을 표시한다．


이제 위 예제에 표현된 것을 다시 정리하면， 비트 필드 ddddd을 얻기 위해서는 phys.hi 값을
오른쪽으로 ]］만큼 쉬프트하四F 한다．                  PCI 슬롯］에 대한 phys.hi 값인 0xC000을 오른쪽으로
]］비트 만큼 쉬프트 연산해서 디바이스 ID 24仙口8）를 얻는다. PCI 슬롯2에 대한 phys.hi 값인
0xC800을 오른쪽으로 ]] 비트 만큼 쉬프트 연산해서 디바이스 ID 25(0x19）를 얻는다．                    아래의
내용은 이 모든 것을 담은 interrupt-map 속성을 해석한 것이다‘


슬롯］의 쒸NTA는 限Q9 이고, 주 인터럽트 콘트롤에서 로우 레벨일따1 인식된다．
슬롯］의 判NTB는 限Q 10 이고, 주 인터 럽트 콘트롤에서 로우 레벨일때1 인식된다．
슬롯1의 判NIC는 限Q1] 이고, 주 인터 럽트 콘트롤에서 로우 레벨일때1 인식된댜．
슬롯］의 判NTD는 IRQ 12 이고, 주 인터럽트 콘트롤0私 로우 레벨일따1 인식된다．



                                         48 / 312
커널연구회（ww岫emn이．b기                                         정쟤준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                     2. Device Tree 소스 분석   49




그리고，


슬롯2의 휘NTA는 IRQ 10 이고, 주 인터럽트 콘트롤에서 로우 레벨일따1 인식된다．
슬롯2의 判NIB는 IRQ 1] 이고, 주 인터럽트 콘트롤에서 로우 레벨일때 인식된다．
슬롯2의 判NTC는 限O12 이고, 주 인터럽트 콘트롤에서 로우 레벨일따1 인식된다．
슬롯2의 쒸NTD는 限O9 이고, 주 인터럽트 콘트롤에서 로우 레벨일따1 인식된다．


interrupts = <8 0>; 이라고 표현된 속성은 호스트／PC卜브릿지 컨트롤러 자신에게 트리거 될 수
있는   인터럽트들을 기술한다.              이런      인터럽트들은 PCI   디바이스들이   트리거    할 수 있는
인터럽트들과 혼합하지 않는다．


마지막으로 설명할 것은． interrupt-parent 속성인데 interrupt-map 속성은 모든 자식 및 손자들
노드들에 대해서 디폴트 인터럽트 콘트롤러를 바꿀 수 있댜.                     위의 PCI 예제에서는, PCI 호스트
브릿지가 디폴트 인터럽트 컨트롤러가 된다는 것을 표현하고 있음을 앞에서 설명했다.                            만약에
PCI 버스를 통해 연결된 디바이스가 또 다른 인터럽트 컨트롤러에 바로 연결되어 있다면，
interrupt-parent 속성을 가지도록 기술되어야 한다.




                                         49 / 312
커널연구회佃ww.kern이.bz)                                      정재준 岫b日307@nate.com)
Device Tree 상세분석 ir) 니flux Kernel 4.0                                      3. Device Tree 실용 분석   50




3. Device Tree 실용 분석




                                                                 + 필자의 주말뇽장에서 찍은 호박




지금까지 디바이스 트리에 대한 기본적인 문법은 설명했다.                                이것을 바탕으로 이번장부터는 좀더
실용적인 예제를 통하여 깊이있게 디바이스 트리를 이해하도록 하자.                                       예제는 리눅스 커널 4.0 버
전의 arch/arm/boot/dts/ 경로에 있는 삼성 Exynos5에 관한 소스 파일들을 분석한다.                                관련되는
정보는 커 널 4.0 버전의 Documenta如n/devicetree 경로에 있는 문서들을 참조한다．


먼저， 아래와 같이 삼성 ExynosS에 관한 디바이스 트리 소스 파일들을 확인해 보자．



$ ed arch/ arrn/boot/ dts
$ I I exynos5*
-r나rw나小 ] jungjj jungjj 12717 Jun 9 03:19 exynos5250-ar nda j e. d t s
  r놔rw나小 ] jungjj jungjj 6889 Jun 9 03:19 exynos5250-cros-cornnion . dis
-r나-rw나小 1 jungjj jungjj 17448 Jun 9 03: 19 exynos5250 . d t si
-r나-rw나小 ] jun｛기 j jungjj 15764 Jun 9 03: 19 exynos5250-pinctr I .dtsi
나中1W나小 ] jungj j jun（기 ] 8752 Jun 9 03:19 exynos5250-smdk5250. dts
  r나rw寸小 ] jungj j jungjj 4422 Jun 9 03: 19 exyn0s5250-snow. dts
나中rw寸n戶 ] junqjj jungjj 8954 Jun 9 03:19 exynos5420-arndale-octa.dts
나忙IW나- 1 jungjj junujj 17457 Jun 9 03:19 exyn0s5420.dtsi
나忙rw나-- 1 jun0jj junqjj ia中54 Jun 903:19 exynos5420-pinctrl . dtsi
  rv中rw나小 ] jungj j jungj j 8654 Jun 9 03:19 exynos5420-snidk5420. dts
  rw-rw-r-- 1 jungjj jungjj 7020 Jun 9 03:19 exynos5440. dtsi
  r中rw나小 ] jungjj jungjj     871 Jun 903:19 exyn0s5440-sd5vl . dts

                                              50 / 312
커 널 연구회（www.kernel.b刃                                                  정재준 (r야)i3307但）nate.com)
Device Tree 상세분석 in 니nux Kerr倒 4.0                                              3. Device Tree 실용 분석     51




     rw-rw-r-- 1 jungjj jungjj   1559 Jun   9 03:19 exyn0s5440-ssdk5440. dts
     rw-rw-r-- 1 jungjj jungjj   2600 Jun   9 03:19 exynos5. dtsi

$ I I sk*
  r나나w寸小 ] jungj j jun（기 J 324 Jun        9 03:19 ske1et0n64. dtsi
-rw-rw-r-- 1 jungjj jungjj 297 Jun        9 03:19 skeleton. dtsi




위의 파일들 중에서                   skeleton dtsi, exynos5.dtsi, exynos5420-pinctrl.dtsi, exynos5420.dtsi,
exynos5420-arndale-octa.dts 파일들이 중요 관심 대상이다.                             이들을 열어보면 skeleton.dtsi 今
exynos5.dtsi 今 exynos5420-pinctrI.dtsi 今 exynos5420.dtsi 今 exynos5420-arndale-octa.dts 순으로
포함 관계를 가지면서 인클루드 됨을 확인할 수 있다.                                        아래1 테이블은 이 파일들의 의미를 요약
정리한 것이다．




     skeleton.dtsi                       부팅에 필요한 디바이스트리의 뼈대구조 기술
     exynos5.dtsi                        Exynos5 계열에 공통적인 장치 기술
     exynos5420-pinctrl.dtsi             Exynos5420 CPU 핀에 대한 용도를 기술
     exynos5420.dtsi                     Exynos5420 CPU 내부 장치들 기술
     exynos5420-arndale-octa.dts         Exynos5420 CPU가 탑재된 보드에 대한 장치 기술


먼저 skeleton.dtsi 파일을 열어 보면，




／士
     * Skeleton device tree; the bare minimum needed to boot; just include and
     * add a compat ible value. The bootloader wi l l typical ly populate the memory
     火 node.
     士 /




/ {
             #address-cel Is = <1> ;
             #size-cel ls = <1>;
             chosen { };
             al iases { };
             memory { device_ type = " memory ' ; reg = <0 0> ; };
};
파일 명칭인 skeleton의 사전적 의미가 말해주듯이 디바이스 트리 뼈대 만으로 구성되어 있다．
부팅에 필요한 최소한의 정보를 담고 있고,                               메모리에 관한 정보는 부트로더에서 설정되도록 맡겨
져 있다． #address-ce小 = <]＞이고 ＃引ze-ce小 = <]＞이므로 32비트 주소로 접근함을 알 수 있다．
참고로 64비트 버전은 다음과 같이 skeleton64.dtsi 파일을 열어 보면, #a改ress尸cells = <2＞이고


                                                      51 / 312
커 널 연구회（www.kern이b기                                                            정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                             3. Device Tree 실용 분석     52




#size-ce小 = <2＞로 시작함으로 참고하기 바란다．


／女
     * Skeleton device tree in the 64 bits version; the bare minimum
     * needed to boot; just include and add a compatible value. The
     * bootloader wi l l typical ly populate the memory node.
     出／
/{
               #address-cel ls = <2> ;
               #size-cel Is = <2>;
               chosen { };
               al iases { };
               memory { device_ type = " memory" ; reg = <0 0 0 0> ; };
};
다음으로 exynos5.dtsi 파일을 열어보면， Exynos5 계열에 공통적인 장치（인터럽트， 시리얼， RTC）에
대해서 기술하고 있다．




      * Samsungs Exynos5 SoC series common device tree source

      * Copyr ight (c) 2012-2013 Samsung Electronics Co. , Ltd.
                        http: //w놔W. samsung. com

      * Sanisungs Exynos5 SoC ser ies device nodes are l isted in this fi le. Particular
      * SoCs from Exynos5 ser ies can include this f i le and provide values for SoCs
      *S口ecf ic I키nd i ngs.

      * This program is free software; you can redistr ibute it and/or modify
      * it under the terms of the GNU General Publ ic License version 2 as
      * publ ished by the Free Software Foundation.
          女／
 #include 'skeleton. dtsi

I{
               interrupt-parent = <&gic> ;

               al iases {
                            ser ialO = &ser ial 0;
                            seriall = &serial 1;
                            ser ia12 = &serial 2;
                            5er ia13 = &serial 3;
               };

               chipid@10000000 {
                        compat ible = ' samsung, exynos42lo巾chipid' ;
                        reg = <0x10000000 oxloo>;
               };

                                                       52 / 312
     커 널 연구회佃w낚,.kernel.b기                                                      정쟤준 (rgbi3307@nate.com)
Device Tree 상세분석 in 나nux Kernel 4.0                                         3. Device Tree 실용 분석   53




       combiner: interrupt-control ler@10440000 {
                compatible = 'samsung,exyn0s4210-combiner ";
                #interrupt-cel Is = <2> ;
                interrupt-control ler;
                samsung,combiner-nr = <32> ;
                reg = <0x10440000 0xl000>;
                interrupts =       <0 0 0>, <0 1 0> , <0 2 0>, <0 3 0>,
                                   <040>, <050>, <060>, <070>,
                                   <0 8 0>, <0 9 0>, <0 10 0>, <0 11 0>,
                                   <0 12 0>, <0 13 0> , <0 14 0>, <0 15 0>,
                                   <0160>, <0170>, <0180>, <0190>,
                                   <0 20 0>, <0 21 0>, <0 22 0>, <0 23 0>,
                                   <0 24 0> , <0 25 0> , <0 26 0> , <0 27 0>,
                                   <0 28 0>, <0 29 0> , <0 30 0>. <0 31 0>;
       };
       이c: interrupt-control ler@10481000 {
               compatible = "arm,cortex-a15-gic "' , "arm,cortex-a9-gic";
               #interrupt-cel ls = <3> ;
               interrupt-control 1 er;
               reg =    <0x10481000 0x1000>,
                        <Ox10482000 0x1000>,
                        <0x10484000 0x2000>,
                        <Ox10486000 0x2000>;
               interrupts = <1 9 0xfo4>;
       };
       seria匕0: serial@12C00000 {
               compatible = n samsung,exynos42lo-uart ";
               reg = <Ox12C00000 0x100>;
               interrupts = <0 51 o>;
       };
       serial_i: serial@12C10000 {
                compatible = "samsung,exynos4210-uart " ;
                reg = <Ox12C10000 0x100>;
                interrupts = <0 52 0>;
       };
       seria匕2: serial@12C20000 {
               compatible = "samsung,exynos4210-uart ";
               reg = <Ox12C20000 0x100>;
               interrupts = <0 53 o>;
       };
       serial_3: serial@12C30000 {
                compatible = "samsung,exynos42lO-uart ' ;
                reg = <Ox12C30000 0xlOO>;
                interrupts = <0 54 0>;
       };
       rtc@101E0000 {
                compatible = "samsung, s3c6410-rtc";
                reg = <Ox101E0000 0x100>;
                interrupts = <0 43 0>, <0 44 0>;

                                              53/ 312
커 널 연구회（www.kernel.b기                                                    정재준 的bi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                3. Device Tree 실용 분석     54




                 status = 'disabled ' ;
       };
        fimd@14400000 {
                 cornpat ible = "sarnsung,exynos5250- f imd";
                 interrupt-parent = <&combiner>;
                 reg = <0x14400000 0x40000>;
                 interrupt-names = "t ifo", "vsync", "lcd_sys";
                 interru口ts = ＜化 4>, <18 5>, ＜化 6>;
                 samsung, sysreg = <&sysreg_system_control ler>;
                 status = "disabled";
        };
       dp-control ler@145B0000 {
                compatible = "samsung,exynos5-dp";
                reg = <0x145B0000 oxl000>;
                interrupts = <10 3>;
                interrupt-parent = <&combiner>;
                #address-cel ls = <1>;
                #size-cel Is = <0>;
                status = 'disabled";
        };
};




3.1 CPU 표현
삼성 Exynos5420 CPU을 표현한 디바이스 트리는 exynos5420.dtsi 파일을 열어보면 다음과 같이
확인할 수 있다．




        compatible = "samsung,exynos5420", "samsung,exynos5";

       ／士 중간 생략 火／




                 cpu0: cpu@0 {
                          device_ type = 'cpu";
                          co畔）atible = "arm,cortex-a15";
                          reg = <oxo>;
                          clock-frequency = <1800000000>;
                          c이兀애tro卜port = <&cci contra너＞;



                 cpul : cpu@1 {
                           device_ type = "cpu";

                                               54 I 312
커 널 연구회（ww＼사.kernel.b기                                             정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니nux Kern이 4.0                              3. Device Tree 실용 분석     55




                       compatible = "arm,cortex-a15";
                       reg = <Oxl>;
                       clock- frequency = <1800000000>;
                       cdi-control-port = <&cci_contro너>;
               };
               cpu2: cpu@2 {
                        device_type = 'cpu";
                        compatible = "arm, cortex-a15";
                        reg = <0x2>;
                        clock- frequency = <1800000000>;
                        c이-cont ro卜port = <&cci_contro너＞;
               };
               cpu3: cpu@3 {
                        device_type = 'cpu ' ;
                        compat ble = "arm,cortex-a15";
                        reg = <0x3>;
                        clock- frequency = <1800000000>;
                        cci-control-port = <&cci_contro너>;
                };
               cpu4: cpu@100 {
                        device_ type = "cpu ' ;
                        compatible = "arm,cortex-a7느
                        reg = <Oxloo>;
                        clock- frequency = <1000000000>;
                        cci-cont rol-port = <&cci_controlo>;
                };
               cpu5: cpu@101 {
                        device_type = "cpu";
                        compatible = "arm,cortex-a7' ;
                        reg = <oxlol> ;
                        clock- frequency = <1000000000>;
                        cc卜凹ntrol-port = <&cc匕controlo>;
               }

               cpu6: cpu@102 {
                        device_type = "cpu ' ;
                        compatible = "arm, cortex-a7";
                        reg = <0x102>;
                        clock- frequency = <1000000000>;
                        cci-control-por t = <&cci_control巾;
               };

               cpu7: cpu@103 {
                        device_ type = "cpu ' ;
                        corn口at 比니e = "arm,cor tex-a7 " ;
                        reg = <0x103>;
                        clock- frequency = <1000000000>;
                        C이叱ont ro卜port = <&Cc匕controlO>;
                };
       }:

       ／士 이하 생략 士／

                                            55 / 312
커 널 연구회（ww납／.kernel.bz)                                        정쟤준 (r야)i3307@nate.com)
Device Tree 상세분석 In 니flux Kernel 4.0                                       3. Device Tree 실용 분석     56




};


삼성 Exynos 5420은 CPU 코어를 8개 가지고 있으며 ARM의 너9.니TILE 구조를 채택했다.                                 big 프
로세서는 Cortex-Al 5 아키텍쳐이며 내부 클럭 속도는 ] .8GHz이다.                             위의 소스를 보면 cpu0, cpul,
cpu2, cpu3 노드들로 각각의 속성들을 표현하고 있음을 알 수 있다.                                  니TTLE 프로세서는 Cortex-
A7 아키텍쳐이며 내부 클럭 속도는 1.0GHz이댜． 위의 소스를 보면 cpu4, cpu5, cpu6, cpu7 노드
들로 각각의 속성들을 표현하고 있음을 알 수 있다．



甘셩 自批os 5420 blg.UTTII CPt席


     Cortex-       Cor始x-        Cortex-         Cortex-
      A15           A15           A佰              A佰




CPU 노드를 표현할 때 몇가지 주의할 점이 있다.                                       노드의 명칭은 반드시 cpus로 해야하고
#address｛이Is은 32비트 경우는 <]＞로 하고 64비트 일때는 <2＞로 한다.                                그리고 ＃針ze｛이匕는
반드시 <0＞으로 해야하고 device_type 또한 반드시 " cpu" 로 해야함을 주의하자．


아래는 여러가지 종류의 프로세서들에 대해서 cpus                                       노드를 표현한 디바이스 트리 예제들이다．
참고하길 바란댜．



Example 1 (dual-cluster big.LITTLE system 32-bit) :

          Cpus {
                    #size-cel Is = <0> ;
                    #address아키 Is =; <] >‘,

                    cpu@0 {
                              device_ type = 'cpu " ;
                              COIl口at 냐키e = "arm, cortex卞a15 " ;
                              reg = <OxO>;
                    };
                    cpu@1 {
                              device_ type = 'cpu ";
                              compatible = "arm, cortex-a15";
                              reg = <oxl>;




                                                    56 / 312
커 널 연구회（ww＼사．kernel.b기                                                    정재준 (rgbi3307@nate.com)
Device Tree 상세분석 ir) 니nux Kerr倒 4.0                                 3. Device Tree 실용 분석    57




                  야）u@100 {
                              device_ type = " cpu " ;
                              compat ible = "arm, cortex-a7 " ;
                              reg = <Ox100> ;
                  },
                  야）u@101 {
                              device_ type = "cpu";
                              compatbie = "arm, cortex-a7 " ;
                              reg = <OxiOl> ;
                  };
         };
Ex帥口le 2 (Cortex-A8 uniprocessor 32-bit system) :

         야）us {
                  #size-cel Is = <0> ;
                  #address-cel ls = <1> ;

                  야）u@0 {
                              devicetype = "cpu";
                              corn口at 比니e = "arm, cor tex-a8 " ;
                              reg = <OxO> ;
                   };
         };
Ex帥ple 3 (ARM 926EJ-S uniprocessor 32-bit system) :

         cpus {
                   #size-cel Is = <0> ;
                   #address-cel Is = <1> ;

                  cpu@0 {
                              device_ type = "Cpu ";
                              compatible = "arm, arm926ej尸s";
                              reg = <OxO>;

          };




3.2 메모리 표현
삼성 Exynos5420은 32비트 시스템이므로 4GB의 메모리 주소 공간을 가지고 있다.                             이 공간을 사
용 목적별로 다음과 같이 나누었다. (Exynos5420 데이터시트는 아직 공개 되지 않아서, 아래 테이

블은 Exynos5250 메모리 맵이다）



甘첨 自少m心250I모러 뫼



                                                    57 / 312
커널연구회（www.kernel.bz)                                               정재준 仕gbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                              3. Device Tree 실용 분석       58




 시姦k키藿） 추소 1               쏘毋 주소mm3:3          盈因           斗m1/4     「1茗           섧형 二＼, 11/ 1        크
0x0000 0000            0x0000 FFFF                64 KB    iR(가너八RAM/SROM
0x0200 0000            0x0200 FFFF                64 KB    IROM (mirror of 0x0 to 0xFFFF)
0x0202 0000            0x0207 7FFF              352 KB     iRAM
0x0300 0000            0x0302 7FFF              160 KB     Data memory of SRP
0x0302 8000            0x0303 FFFF                96 KB 卜cache of SRI'
0x0304 0000            0x0304 8FFF                36 KB    Configuration memory of SRI
                                                                                     ' (write-only)
0x0380 0000            0x0386 FFFF              448 KB     SFR region of AudioSS
0x0400 0000            0x0402 0000              128 KB     SROMC's Bank 0
0x0500 0000            0x0502 0000              128 KB     SROMC's Bank 1
0x0600 0000            0x0602 0000              128 KB     SROMC's Bank 2
0x0700 0000            0x0702 0000              128 KB     SR아너C's Bank 3
0x1000 0000            0x1FFF FFFF              256 KB     SFR reg向n
0x2000 0000            0xFFFF FFFF            3586 KB      DRAM


위에서 각종 레지스터들은 SFR reg向n(0x1000_0000 N 0x］댜F_FFFF）에 위치하고 있다.                                          각종 디바
이스 드라이버들은 이 영역에 있는 레지스터들에 정보를 설정한다.                                             사용자 어플리케이션이 실행
되는 메모리는 DRAM(0x2000_0000 N 0xFFFF_FFFF) 영역이다.                              보통 사용자 메모리라 함은 이영
역을 말하는 것이다．


사용자 메모리는 arch/arm/boot/dts 디바이스 트리 경로를 보면 exynos5420-arndale-octa.dts 파
일에 댜음과 같이 정의되어 있다．


#include "exynos5420. dtsi "
#include <dt-bindings/ interrupt-control ler/ irq.h>
#include <dt-bindings/ input/ input.h>

I{
         model = ' lnsignal Arndale Octa evaluation board based on EXYNOS5420n ;
         compatible = " insignal ,arndale-octa ' , 'sarnsung, exyn0s5420 ' , 'samsung, exynos5 ' ;

         memo四 {
                   reg = <0x20000000 0x80000000> ,
         };
／士 이하 생략 士／

};


memory 노드 속성에 레지스터 시작 주소가 0x2000 0000 이고 크기가 0x8000 0000 이므로， 사용
자 메모리는 기준주소 0x2000 0000부터 2GB 용량으로 설정되어 있음을 알 수 있다．


                                                   58 / 312
커 널 연구회（www.kern이.b기                                                            정쟤준 (rgbi3307t nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                     3. Device Tree 실용 분석    59




3.3 인터럽트 표현
삼성 Exynos5의 인터럽트 콘트롤러는 더C(Generic Interrupt Contr에ers）와 Interrupt Combiners로
구성되어 있다.         더C는 CoreLink （引C-400을 채택했다.              이것의 구조에 대해서는 인터넷에서 아래
내용으로 검색하면 PDF 문서로 다운로드할 수 있다．


CoreLink GIC-400 Generic Interrupt Controller-Technical Reference Manual, Revision rOpO
ARM Generic Interrupt Controller-Architecture Specification, Architecture version 2.0


위의 내용에서 G（의 특징만을 간단히 요약하면，
    .   （引C는 한      Il 이상의 프로세서에 적용할 수 있는 인터럽트 인터페이스이다．
    0   AMBA(Advanced 卜4icrocontrolIer Bus Architecture) 버스 구조에 최적화 되어 있다．
    1   AXI(Advanced eXtensible Interface) 구조에 최적화 되어 있다．
    0   SoC(System on Chip) 환경에서 인터럽트를 검색, 관리 , 분배한다．
    1   SG I(Software Generated Interrupts) 인터럽트를 지원한다.
    0   각각의 프로세서에 대하여 PPI(Private Peripheral Interrupts) 인터럽트를 지원한다．
    1   SPI(Shared Peripheral Interrupts) 인터럽트를 지원한다．




                                              59 / 312
커널연구회（ww比kernel.bz)                                                    정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                              3. Device Tree 실용 분석                              60




                                                           GIC
        CFGSDISABLE8-.
                                           tX璥ribu幻I.




                                              :
                  sP怜             In佃rupt 心
                           132-
                                      1019                                                                                       m入
                                                                         4           내客盟껑寶．. hd誌：

                           口I                                       L    V壯ual
                                                                          CPU
                                                                                   什韶茗驩쁜
                                                                        m佃相ce7( m) 作F心，＼川tO）亡
                                                                                                                        To
                                                                                                                       V浪U冬
                                                                                                                      ma아出埠
                                                                                                                                             工口
                                                                                                                                          口ro的＄＄澍
                                                                                                                                             7



                           I
   F｛甘
                   PP怡
                           仄奴하rupt ID
                                                                    Cpu   卜냐Min헒弦岩麓d,
proce$sor                                       M S｛引               erface 7+L
    7                             nterr。
                                     18                 reque얽                    b- 中 FIQ , 眼Q
                                      -如
                           1
            (FIQ, IRO）口                                                      p-




                                                                                                                                      i

                                                                                                                                      1




                                                                                       Memo싸小好pped                       而
                                                                                       !nterfa羽，GICH " '              by尹라邸아


                                                                                       如쓰叫性i芦乞기                          !0
                                                                                       In哨mt氾1＼二11/ V                                       To
                                                                                                                      5virtUai
                                                                                                                                          pm的ssor
                                                                                        VFIQ, VIRO)        그m各chine                          0
                                  油始m刃'ID                                              M陋mor恥1l하恥ed
                   PP陌                                                                 In伯卄可：e, 미CC.
   F어                                16-31
口rO的＄$步                           Interrupt 心           敬引
    0                                 0-15              request
            (FIQ和, IRQ)b     H




위의 (3IC 내부 구성도를 보면, （引C는 ［기stributor 블럭과 한                                            II 이상의 CPU 인터페이스 블록으로
구성되어 있다.              또한 Virtual CPU 인터페이스 블럭이 추가되어 있다.                                            Distributor 블록은 인터럽
트 종류별로 우선순위를 판별하여 CPU 인터페이스 블록으로 분배하는 역할을 한다.                                                                                    CPU 인터페
이스 블록은 우선순위 마스킹, 선점제어 등의 작업을 해당 CPU에 대해서 수행한다．


인터럽트 山는 0번에서 ]5번이 S더이고, 16번에서 3] 번이 PPI, 32번에서 ]59번이 S미이다．


아래는 삼성 Exynos5250의 （引C 특징을 테이블로 간단히 정리한 것이다．




                                                                  60 / 312
커 널 연구회佃／ww.kerne냐끄）                                                                          졍재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                            3. Device Tree 실용 분석   61




external Private Peripheral Interrupts (PPl)              8 (4 for each processor)

Shared Peripheral Interrupts (SPI)                        128

Priority Level                                            32

Legacy interrupt Support                                  No

Number of CPUs                                            2



삼성    Exynos5250에서       인터럽트 소스들은 몇 개의 그룹（32개b으로 묶어서                                 표현할 수 있으며

Interrupt Combiners가 이         역할을 수행한다．               따라서      인터럽트        컨트롤러는 （引C와 Interrupt
Combiners로 디바이스 트리에 표현한다．


리눅스 커널 4.0 소스의 arch/arm/boot/dts 디바이스 트리 경로를 보면 exynos5.dtsi 파일에 다음

과 같이 인터럽트 컨트롤러가 정의되어 있다．


/ {
          interrupt-parent = <&gic>;

         ch回d@10000000 {
                compat ible = Usamsung, exynos42lo_chipid「 ;
                reg = <0x10000000 oxloo> ;
          };
         combiner: interrupt-control Ier@10440000 {
                  compatible = "samsung, exynos42lo-combiner " ;
                  #interrupt-cel Is = <2> ;
                  interrupt-control ler;
                  samsung, combiner-nr = <32> ;
                  reg = <0x10440000 oxl000> ;
                  interrupts =       <0 0 0>, <0 1 0> , <0 2 0>, <0 3 0>,
                                     <0 4 0>, <0 5 0> , <0 6 0>, <0 7 0>,
                                     <0 8 0>, <0 9 0>, <0 10 0> , <0 11 0> ,
                                     <0 12 0> , <0 13 0> , <0 14 0> , <0 15 0>,
                                     <0 16 0> , <0 17 0> , <0 18 0> , <0 19 0> ,
                                     <0 20 0> , <0 21 0> , <0 22 0> , <0 23 0> ,
                                     <0 24 0> , <0 25 0> , <0 26 0> , <0 27 0> ,
                                     <0 28 0>, <0 29 0> , <0 30 0> , <0 31 0> ;
          };
         gic: interrupt-control ler@10481000 {
                  compat ible = "arm,cortex-alS-gic " , "arm,cortex-ag-gic ";
                  削nterrup卜cel ls = <3> ;
                  interru아叱ontrol 1 er ;
                  reg =     <0x10481000 0x1000> ,
                            <0x10482000 0x1000> ,
                            <0x10484000 0x2000> ,
                            <Oxi 0486000 0x2000> ;
                   nterrupts = <1 9 0x104> ;
         };

/* 이하 생략 士／

                                                 61 / 312
커 널 연구회（www.kern이. b기                                                       정재준 (I야키3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                           3. Device Tree 실용 분석       62




};


위의 내용을 확인해 보면， 삼성 Exynos5 （引C는 다음과 같이 표현된다．


        gic: interrupt-control ler@10481000 {
                  compat ible = 'arrn,cortex-a15-gic ' , 'arm,cortex-a9-gic
                  削nter ru아-cel ls = <3> ;
                  interrupt-control ler;
                  reg =     <0x10481000 oxl000> ,
                            <Oxi 0482000 0xi 000>,
                            <Oxi 0484000 0x2000> ,
                            <Oxi 0486000 0x2000> ;
                  interrupts = <1 9 0xf04>;
         };

（引C 레지스터의 기준주소는 小(1048 1000에 있고 인터럽트 셀은 3개이다．
첫번째 셀은 인터럽트 타입을 나타낸다.                          0이면 spi 타입의 인터럽트이고, ] 이면 ppI 타입의 인터
럽트이다.       두번째 셀은 인터럽트 번호이다.                    SPI 인터럽트는 0에서 987 범위이고 ppl 인터럽트는
0에서 ]5범위의 번호를 가진다． 세번째 셀은 인터럽트 플래그이며 다음과 같이 해석한다．


비트［크이은 다음과 같이 인터럽트가 기동되는 레벨이다．
1: low-to-high edge triggered
2: high-to-low edge triggered
4: active high level-sensitive
8: active low level-sensitive


비트［15:8］은 PPI 인터럽트 Cpu 마스크이다． 각각의 비트는 8개의 Cpu를 나타낸다． 해당 비트가
] 이면 그 Cpu로 인터럽트가 가능함을 의미한다.                           이 규칙은 p미에만 해당된다.                 인터럽트7F 다음
과 같이 표현되고 있으므로，


                    nterrupts = <1 9 0xf04>;


1: PPI 타입의 인터럽트
9: 인터럽트 번호（Virtual maintenance interrupt)
0xf04: 인터럽트 플래그（ac如e high level-sensitive, 4개 Cpu 인터럽트 가능）


위와 같이 판독된다．


reg 속성은 다음과 같이 표현되고 있으므로，



                                                 62 / 312
커널연구회（www.kernel.bz)                                                          정재준 (rgbi3307（亘）nate.con功
Device Tree 상세분석 in Linux Kernel 4.0                                         3. Device Tree 실용 분석    63




                   reg =    <0x10481000 0x1000> ,
                            <0x10482000 0x1000> ,
                            <0x10484000 0x2000> ,
                            <0x10486000 0x2000> “,


0x1048그000 0x1000: GIC 분배기（Distributor) 레지스터 기준주소와 크기
0x1048_1000 0x1000: GIC CPU Interface Register 기준주소와 크기
0x1048_1000 0x1000: Virtual Interface Control Register 기준주소와 크기
0x1048_1000 0x1000: Virtual CPU Interface Register 기준주소와 크기


위와 같이 판독한다．


삼성 Exynos5의 Interrupt Comi기ners는 다음과 같이 표현되어 았다．


       combiner: interrupt-control Ier@10440000 {
                compat ible = "sarnsung, exynos4210-combiner n ;
                #interrupt-cel Is = <2> ;
                interru아兀叩trol ler;
                samsung, combiner-nr = <32> ;
                reg = <0x10440000 oxl000> ;
                interrupts =       <0 0 0>, <0 1 0> , <0 2 0> , <0 3 0> ,
                                   <0 4 0> , <0 5 0> , <0 6 0> , <0 7 0>,
                                   <0 8 0>, <0 9 0> , <0 10 0> , <0 11 0> ,
                                   <0 12 0> , <0 13 0> , <0 14 0> , <0 15 0> ,
                                   <0 16 0> , <0 17 0> , <0 18 0> , <0 19 0> ,
                                   <0 20 0> , <0 21 0> , <0 22 0> , <0 23 0> ,
                                    <0 24 0> , <0 25 0> , <0 26 0> , <0 27 0> ,
                                    <0 28 0> , <0 29 0> , <0 30 0> , <0 31 0> ;
        }   ,




Interrupt Com1기ners의 개수는 32개이며 기준주소가 0x1044 0000부터 0x1000 크기 범위에 정의된
다．
3.4C幻ck 표현
삼성 Exynos5 Clock 제어기는 장치마다 독립적으로 동작 클럭을 제공한다．                                         아래 테이블은
Exynos5250의 내부 장치마다 동작하는 주파수를 정리한 것이다．




                E4D Dual-core                                      1.7 GHz
CPU
                CoreSight                                           200 MHz
                DREXII                                             400 MHz/533 MHz/800 MHz
DMC
                SSS, MIU                                            266 MHz/400 MHz


                                                 63 / 312
커 널 연구회（www.kerne比z)                                                       정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니nux Kernel 4.0                                            3. Device Tree 실용 분석     64




LEX             Data Bus/Peripheral Bus                             266 MHz/133 MHz
R0X/Rl X        Data Bus/Peripheral Bus                             266 MHz/133 MHz
G3D             3D Graphics Engine                                  533 MHz
MFC             M미t卜化rmat Codec                                     333 MHz
ISP             Image 듸gnal 마oces引ng                                266 MHz, 400 MHz for MCU ISP
GEN             Rotator, MDMA, JPEG                                 266 MHz (up to 166 MHz for JPEG)
［기Spi           디卜기Dl , 卜川El , 卜川P1 DSI1, VP; 卜川XER, TVENC          200 MHz/333 MHz
GSCL            GSCL0 to 3                                          266 MHz/333 MHz
FSYS            USB, SATA, S［가너MC, SROMC, P［가너AO, P［가너Al            200 MHz, 400 MHz for MCU_FSYS
MAU             Au（抑：)SS(MAU［기이                                     192 MHz
PERIC           UART, l2C, SPI, 12S, PCM, SPDIF, PWM                66 MHz
PERIS           CHIPID, SYSREG, PMU/CMU/TMU Bus I/F,                66 MHz
                MCTimer, WDT, RTC, KEYIF, SECKEY, TZPC


Exynos5420 Clock 제어기는 디바이스 트리 경로 arch/arm/boot/dts의 exynos5420.dtsi 파일에 다
음과 같이 정의 되어 있다．


#inc山de <dt寸）indings/ clock/exynos5420.h>
쒸nc山de "exynos5. dtsi "
#include "exynos5420-pinctr l .dtsi '

／시 nclude <dl七m di四S／이ock/ exyno釘叩ds于이k . h>

/ {
      compat ible = 'samsung, exyn0s5420', "samsung, exynos5 " ;


      ／出 중간 생략 出／

      clock: clock-control Ier@10010000 {
           compat ible = "samsung, exynos5420-c lock ' :
           reg = <Ox10010000 0x30000>;
           #clock-cel ls = <1> :
      };
      ／大 이하 생략 大／
};


reg 속성을 보면 Clock 레지스터의 기준주소가 0x1001 0000이고 크기는 0x30000으로 표현되어
있다.        Clock 셀은 1이 되어야 한다． 이렇게 정의된 Clock 제어기를 다른 장치 노드에서 사용할
때는 다음과 같이 표현한다．


           uart_0: ser ial@12C00000 {
                     clocks = <&clock CLK. UARTO> , <&clock CLKSCLKUARTO> :

                                                     64 / 312
커 널 연구회（ww比kern飢b기                                                            정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                         3. Device Tree 실용 분석     65




                   clock-names = " uart ", "clkuart baudO";
         };
         uart_1 : ser ial@12C10000 {
                   clocks = <&clock CLKUART1> , <&clock CLK_SCLK_UART1> ;
                   clock-names = "uart ' , "clk_uart baudO " ;
         }'
         uart_2: ser ial@12C20000 {
                  clocks = <&clock CLK_UART2> , <&clock CLK_SCLK_IJART2>;
                  clock-names = "uart ", "clk_uart_baudO";
          };
         uart_3: ser ial@12C30000 {
                  clocks = <&clock CLKUART3> , <&clock CLK_SCLK_UART3> ;
                  clock-names = "uart ", "c나_
                                            (uart_baudO " ;
          };
         r）밖rn: p벼m@12dd0000 {
                    compatible = "samsung, exynos4210-pwm " ;
                    reg = <0x12dd0000 0xlOO> ;
                    samsung, pwm-outputs = <0> , <1> , <2> , <3> ;
                    抑川vrn-ce u 1s = <3> ;
                    clocks = <&clock CLK PWM>;
                    clock-names = n t imers ' ;
          };


clocks   속성은       Clock    제어기0似］         어떤      Clock을      사용할    것인지     가술한다.      CLK_UARTO,
CLK_SCLK_UARTO는        Clock    종류를 숫자로            정의한        것이댜．    커널     소스의   inc山de/dt七in帥gs
/clock/exynos5420.h 헤더파일에 정의되어 있다.                       clock-names 속성은 clocks 속성에 정의한 Clock
과 일대일로 연결되는 이름이다．




3.5 CCI 표현
CCI(Cache Coherent In扼rconnect）는 exynos5420.dtsi 파일에 다음과 같이 정의 되어 있다.                         CCI는
big.니TTLE 아키텍처0私］ big 코어들과 LITTLE 코어들을 서로 연결시키고 메모리를 관리하여 자원
들을 분산 시키는 역할을 한다.                     캐시를 사용하므로 외부 메모리 접근은 최소화 하고 소프트웨어
부하를 줄여서 시스템의 성능을 향상 시킨다．


         cci@10d20000 {
                   corn口at 比니e = "arm, cci-400' ;
                   #address-cel Is = <1> ;
                   #size-cel Is = <1> ;
                   reg = <0x10d20000 0xl000>;
                   ranges = <0x0 0x10d20000 0x6000> ;

                   cci controlO: 引ave기 他．4000 {
                            compatible = "arm, cci-400-ctr I- if ";


                                                   65 / 312
커 널 연구회佃ww.kern飢b기                                                          정쟤준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                     3. Device Tree 실용 분석    66




                           interface- type = 'ace";
                           req = <0x4000 0xl000>;
                 };
                 cci -中contro너 : 引ave니他5000 {
                            compat 比니e = "arm, cci寸400-ctr I니 尸 ;
                            interface-type = 'aCen ;
                            reg = <0x5000 0xl000>;
                 };
       };
삼성 Exynos5420은 CC읕 0x10D2 0000 레지스터 기준 주소에 설정한다． 3.1절에서 언급한 CPU
표현을 확인해1 보면， big 코어（Cortex구너5）는 CCI 제어 포트로 cci_contr이］을 사용하고 LITTLE 코
어（Cortex-A7）는 cci_controlo을 사용함을 알 수 있다．




3.6 내무 시스템 메모리 표현
Exynos5420 내부 시스템 메모리인 浪AM은 exynos5420.dtsi 파일에 다음과 같이 정의 되어 있다．


       sysr am@02020000 {
                  compatible = "mmio-sram";
                  reg = <0x02020000 0x54000>;
                  #address-cel Is = <1>;
                  #size-cel ls = <1>;
                  ranges = <0 0x02020000 0x54000>;

                  smp-sysram@0 {
                            compatible = 'samsung,exynos42lo-sysram";
                            reg = <OxO 小l000>;
                  };
                 S叩四ysra昶53000 {
                        compatible = "samsung,exynos42lo-sysram-ns";
                        reg = <0x53000 小l000>;
                      };
            };
iRAM의 기준주소는 0x0202P000이며 크기는 0x54000 (336KB）로 정의되어 있다．



3.7 MMC 표현
플래시 메모리를 제어하는 MMC는 exynos5420.dtsi 파일에 다음과 같이 37l1의 노드（포트）로 정의
되어 있다．

                                                66 / 312
커 널 연구회（ww比kerneLbz)                                                    정재준 (rgb日307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                       3. Device Tree 실용 분석    67




       rnmc_O: mmc@12200000 {
                  compatible = "samsung , exynos5420-dw-mshc-smu";
                  interrupts = <0 75 0>;
                  #address-cel Is = <]>;
                  #size-cel ls = <0>;
                  reg = <0x12200000 0x2000>;
                  clocks = <&clock CLK_MMCO> , <&clock CLK_SCLK_쌔CO>;
                  이ock-narnes = 'b山' , "C나In ;
                  fifo-depth = <0x40>;
                  status = "disabled";
         };
        mmc_1 : mm砲1쏘1凹00 {
                 compatible = "samsung,exynos5420-dw-mshc-smu ";
                  interrupts = <0 76 0>;
                 #address-cel Is = <1>;
                 ＃引ze-(氾u 1s = <0>;
                 reg = <0x12210000 0x2000> ;
                 clocks = <&clock CLK_MMC1> , <&Cm아； CLK SCLK小씨내거＞;
                 clock-names = "biu", "ciu";
                  fit于的아h = <0x40>;
                 status = 'disabled";
         };
         mmc_2: mmc@122200刃 {
                  compatible = "samsung, exyn0s5420-dw-mshc";
                  interrupts = <0 77 0>;
                  #address-cel ls = <1>;
                  #size-cel Is = <0>;
                  reg = <0x12220000 oxl000>;
                  clocks = <&clock CLK_MMC2> , <&clock CLK_SCLK_MMC2> ;
                  clock-names = "biu", "ciu";
                  fito-depth = <0x40>;
                  status = "disabled";
         };




mmc0는 레지스터 기준주소 0x1220_0000, mmc_］은 0x1221_0000, mmc_2는 0x1222 0000에 정의

된 다．




3.8 MCI（타이머） 표현
MCT(M미ti Core 기mer)는 exynos5420.dtsi 파일에 다음과 같이 정의 되어 있다．


       mct: mct@101c0000 {
                  compatible = "samsung, exynos42lo-mct ";
                  reg = <0x101C0000 0x800> ;

                                               67 / 312
커 널 연구회 (wwv出kernelbz)                                                    정재준 (rgb日307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                            3. Device Tree 실용 분석     68




                  nterrupt-control b er ;
                 #interrups-cel Is = <i> ;
                 interrupt-parent = <&mctjnap> ;
                 interrupts = <0> , <1> , <2>, <3> , <4> , <5> , <6> , <7> ,
                                    <8>, <9> , <10> , <11> ;
                 clocks = <&clock CLK_F나_  1PLL> , <&cbock CLK_MCT> ;
                 clock-names = f in_pl l ", "act " ;

                 mctjnap: mct-map {
                          #interrupt-ceb Is = <1> ;
                          ttaddress-ceb Is = <0> ;
                          #S i ze-ce l bs = <0> ;
                            nterrupt-map = <0 &co吐）iner 23 3> ,
                                                  <1 &combiner 23 4> ,
                                                  <2 &combiner 25 2> ,
                                                  <3 &combiner 25 3> ,
                                                  <4 &gic 0 120 0> ,
                                                  <5 &gic 0 121 0> ,
                                                  <6 &qic 0 122 0> ,
                                                  <7 &gic 0 123 0> ,
                                                  <8 &gic 0 128 0> ,
                                                  <9 &gic 0 129 0> ,
                                                  <10 &gic 0 130 0> ,
                                                  <11 &gic 0 131 0>;
                 };
3.9 핀맵巾incti) 표현
Exynos5420 핀맵들은 exynos5420.dtsi 파일에 다음과 같이 정의 되어 있다． 핀맵은 CPU의 핀들
을 어떤 용도로 사용할지 정의한다.                       아래를 보면 크게 5개1 그룹으로 분리하여 관리하고 있음을
알 수 있다.        첫번째 댁nctL0는 0x13400000 주소에 정의하고 두번째는 0xi 3410000, 세번째는
小<14000000, 네번째는 0x14010000. 다섯번째는 0x03860000 주소이다．


       미nctr l_0: pinctr 回3的0000 {
                 compatible = "sarnsung, exynos5420-pinctr I ";
                 reg = <0x13400000 oxl000> ;
                  nterrupts = <0 45 0> ;

                  wakeup- interrupt-control ler {
                            compatible = "sainsung, exynos42lo-wakeup-eint ";
                            interrupt-parent = <&gic> ;
                            interrupts = <0 32 0> ;

        };
        pinctr匕i: pinctr l@13410000 {
                corn口at 比니e = ' samsung , exyn0s5420口inctrb ' ;

                                                  68 / 312
커 널 연구회（www.kernel.b기                                                          정재준 (rgbi3307@nate.com)
Device Tree 상세분석 ir) 니flux Kernel 4.0                                           3. Device Tree 실용 분석    69




                       reg = <0x1341C )00 0x1000>;
                       1nterrupts = < ) 78 0> ;



             pinctr 匕2: pinctrl@140C )000{
                      coAl口at 比니e = ;amsung, exynos5420-pinctr I n;
                      reg = <0x1400C )00 oxl000> ;
                      interrupts = < ) 46 0>;
             };
             pinctr 匕3: pinctrl@14010000{
                      compat 仕키e = n sanisung, exyn055420-pi nctr I " ;
                      reg = <0x1401C 000 oxl000>;
                      interrupts = < 0 50 0>;
             };
             이 nc t r 匕4: 口 inctrl@038E )000 {
                        compatible = n ;arnsung, exyn0s5420-pinctr I n ;
                        reg = <0x0386C )00 0x1000> ;
                        interrupts = < ) 47 0>;
             };




위의 핀설정 그룹들은 /arch/arm/boot/dts/exynos5420- pinctLdtsi 파일에 다음과 같이 자세히 기술
되어 있댜.            아래땍 내용을 확인해 보면，
첫번째 그룹인 pinctrl@13400000에는 GPX 포트들에 대해서 사용 용도를 정의한다.                                        GPX 포트는
주로 외부 인터 럽트를 처리하는 용도로 사용한다．
두번째1 그룹인 F키nctrl＠녀3410000에는 GPC, GPD, GPY 포트들에 대해써 사용 용도를 정의한다.
GPC 와 GPD 포트는 기본적으로 SD 버스（MMC) 인터페이스로 사용한다.                                            GPY 포트는 주로
SRAM을 연결하는 용도로 사용한다．
세번째1 그룹인 pinctrl@14000000에는 GPE, GPF, GPG 포트들에 대해서 사용 용도를 정의한다． 이
포트들은 기본적으로 카메라를 연결하는 용도로 사용한다．
네번째 그룹인 택nctrl@14010000에는 GPA, GPB, GPH 포트들에 대해서 사용 용도를 정의한다．
G PA 포트는 기본적으로 UART와 SPI 인터페이스 용도로 사용한다.                                       GPB 포트는 주로 I2C 훅은
Pw卜月 인터페이스 용도로 사용한다. GPH 포트는 범용의 G미O 인터페이스로 사용한다．
다섯번째 그룹인 pinctrl帥3860000에는 GPZ 포트에 대해서 사용 용도를 정의한댜.                                         GPZ 포트는
기본적으로 사운드 데이터 출력을 위한 I2S 인터페이스로 사용한다．



四1m54朴-                    4出
／大
     * Samsung 's Exynos5420 SoC pin-ni Jx and pin-config device tree source
     士


     * Copyright (c) 2013 Samsung Ele :t ron比s Co. , 나d.
                      http: /／나넥w. sarns ing .com



                                                       69 / 312
커널연구회（www.kernel.bz)                                                           정재준 什gbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                             3. Device Tree 실용 분석   70




     * Samsung 's Exynos5420 SoC pin-mux and pin-config options are l isted as device
     * tree nodes are l isted in this fi le.
     士

     * This program is free software; you can redistribute it and/or modify
     * it under the terms of the GNU General Publ ic License version 2 as
     * publ ished by the Free Software Foundation.
士／
I{
             pinctrl@13400000 {
                      gpy7: gpy7 {
                                gpio-control ler;
                                #gpio-cel ls = <2>;

                                interrupt-control 1 er;
                                削nter ru아-cel ls = <2>;
                      };

                      gpx0: gpx0 {
                               gpio-control ler;
                               #gpio-cel ls = <2>;

                                interrupt-control ler;
                                interrupt-parent = <&combiner>;
                                #interrupt-cel ls = <2> ;
                                interrupts = <23 0>, <24 0>, <25 0>, <25 1>,
                                              <26 0>, <26 1>, <27 0>, <27 1>;
                      };
                      먀）xl : gpxl {
                                gpio-control ler;
                                #gpio-cel ls = <2>;

                                interrupt-control ler;
                                interrupt-parent = <&combiner>;
                                쒸nter ru아叱el Is = <2>;
                                interrupts = <28 0>, <28 1>, <29 0>, <29 1> ,
                                              <30 0>, <30 1>, <31 0>, <31 1> ;
                       };
                      gpx2: gpx2 {
                               gpio-control ler;
                               #gpio-cel ls = <2>;

                                interrupt-control ler;
                                #interrupt-cel ls = <2> ;
                       };
                      야）x3: 야）x3 {
                               gpio-control ler;
                               #gp I 0-cel l S = <2>;

                                interrupt-control ler;
                                #interrupt-cel Is = <2>;
                           };


                                                        70 / 312
     커 널 연구회（www.kernel.b기                                                       정재준 似拘日307@nate.com)
Device Tree 상세분석 ir) 나flux Kernel 4.0                         3. Device Tree 실용 분석     71




                dp_hpd: dphpd {
                         samsung,pins = " gpxO-7' ;
                         samsung, r기 十仙nct 山n = <3> ;
                         sarnsung,pin-pud = <0>;
                         samsung ,口I fl (打V = <0>;
                };
        };
       pinctrl켜3410000 {
                야兀0. ［和cO {
                         gpio-control Ier ;
                         #gpio-cel ls = <2> ;

                          interrupt-control ler ;
                          #interrupt-cel ls = <2> ;
                };
                gpcl : gpcl {
                          gpio-controHer;
                          #gpio-cel Is = <2> ;

                          interrupt-control ler;
                          荊 nterru口卜cel ls = <2> ;
                };
                g口c2: 야）c2 {
                         gpio-control ler ;
                         #gpio-cel Is = <2>;

                          interrupt小control ler ;
                          #interrupt-cel ls = <2> ;
                };
                ｛算）c3: (｝口c3 {
                           gpio-control ler;
                           #gpio-cel Is = <2> ;

                          interrupt-control ler ;
                          #interrupt-cel ls = <2> ;
                 };
                gpc4: gpc4 {
                         gpio-control Ier ;
                         #gpio-cel ls = <2>;

                          interru아-c叩trol ler ;
                          #interrupt-cel ls = <2>;
                };
                gpdl: gpdl {
                         gpio-control ler;
                         #gpio-cel Is = <2> ;

                          interrupt-control len ;
                          #interrupt-cel Is = <2> ;
                };
                                                  71 / 312
커 널 연구회 (www.kernel.bz)                                      정재준 (rgt이3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                        3. Device Tree 실용 분석      72




               gpy0: qpyO {
                        gpio-controUer;
                        #gpio-cel ls = <2>;
               };
               gpy1 : gpyl {
                        gpio-control ler ;
                         #gpio-cel ls = <2> ;
               };
               gpy2: gpy2 {
                        Qpio-control ler;
                        #gpio-cel Is = <2>;
               };
               gpy3: gpy3 {
                        gpio-control ler ;
                        #gpio-cel ls = <2>;
               };
               gpy4: gpy4 {
                        gpio-control ler;
                        #gpio-cel ls = <2>:
               };
               gpy5: gpy5 {
                        Qpio-control 1 er;
                        #gpio-cel ls = <2>;
                };
               gpy6: gpy6 {
                        gpio-control Ier ;
                        #gpio-cel ls = <2>;
               };
               sdO_clk: sd0-c나； {
                        samsung,pins = nqnC(:)U(:)" ;
                        samsunq,pin- f unction = <2>;
                        samsung ,이n-叩d = <0>;
                        samsung,pin-drv = <3>;
               };
               sdO_cmd: sdO-cmd {
                        samsung,pins = 'gpcO-l ' ;
                        samsung,pin- f unction = <2>;
                        samsung,pin가川d = <0>;
                        samsung,pin-drv = <3>;
                };
                sdO_cd: sd0-cd {
                         samsung,pins = 'gpco-2";
                         samsung,pin나 unction = <2> ;
                         saoisung,pin-pud = <3>;
                         samsungpin-drv = <3> ;
                };
                                                72 / 312
커 널 연구회佃八사w.kerneLb기                                       정재준 /gbi3307（亘）nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                         3. Device Tree 실용 분석      73




               sdO니bus1: sd0-bus-widthl {
                        samsung,pins = "gDC03' ;
                        sainsung,pin- f unction = <2>;
                        sarnsung,pin-pud = <3>;
                        samsung,pin-drv = <3>;
               };
               sd0_bus4: sdO-bus-width4 {
                        sanisung,pins = " gpcO-4", "gpcO-5 ' , '대：)co-6느
                        samsung,pin- f unct ion = <2> ;
                        samsung,pin-pud = <3>;
                        sarnsung,pin-drv = <3>;
               };
               sdo_bus8: sdO-bus-w1dth8 {
                        samsung, p ins = " gpc3-0", " gpc3-1" , "gpc3-2 " , "gpc3-3느
                        sanisung,pin- funct on = <2>;
                        samsung , r기n-口ud = <3>;
                        sanisung ,口in卜dry = <3>;
               };
               sdl_clk: sdl-c나（ {
                        sanisung,pins = 노｝DC] 40' ;
                        samsung,pin- f unction = <2>;
                        samsung,pin-pud = <0>;
                        samsung,pin-drv = <3>;
               };
               sdl_cmd: sdl-coid {
                        samsung,pins = "gpcl-l '' ;
                        samsung,pin- function = <2> ;
                        samsung,pin-pud = <0>;
                        samsung , 이m먀V = <3>;
               };
               sdl_cd: sdl-cd {
                        samsung , pins = 노刃cl-2느
                        samsung,pin- funct ion = <2>;
                        samsung，口in小pud = <3>;
                        samsung,pin-drv = <3>;
               };
               sdl_ int: sdl- int {
                         samsung,pins = 'gpdl-l ' ;
                         samsung,pin- funct ion = <2>;
                         sarnsung,pin-pud = <3>;
                         samsung,pin-drv = <0>;
               };
               sd1Hbus1: sdl-bus--widthl {
                        samsun口,pins = 'gpcl-3' ;
                        samsung,pin- f unction = <2> ;
                        samsun口, pin巾ud = <3>;
                        samsung,pin-drv = <3>;
               };
                                             73 / 312
커 널 연구회佃ww.kern이.bz)                                                       정쟤준 (rgbi3307（亘）nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                             3. Device Tree 실용 분석      74




                sdl_bus4: sdl-bus-width4 {
                         samsunq,pins = 'gpc1-4 ' , "gpcl-5", 'gpcl-6" ;
                         samsung,pin- funct ion = <2>;
                         samsung,pin-pud = <3>;
                         samsung,pin-drv = <3>;
                 };
                sdl_bus8: sdl-bus-w1d1h8 {
                         samsung,pins = 'gpd1-4", "gpdl-5 ' , 'qpd1-6' , 'gpdl-7느
                         samsunQ,pin- funct ion = <2>;
                         samsung,pin-pud = <3>;
                         samsung ,이n-山＼/ = <3>;
                 };
                 sd2 （기k: sd2-（기k {
                          samsung,pins = 'gpc2-O ' ;
                          samsung,pin- funct ion = <2>;
                          samsung,pin-pud = <0>;
                          samsung,pin-drv = <3>;
                 };
                 sd2_cmd: sd2-cmd {
                          samsung,pins = 'gpc2-1 ' ;
                          samsung ,이m仙nct ion = <2> ;
                          samsung,pin-pud = <(:)>;
                          samsung ,pin小（打V = <3>;
                  };
                  sd2_cd: sd2-cd {
                           samsung,pins = "gpc2-2 ' ;
                           samsung,pin- function = <2> ;
                           samsung,pin-pud = <3>;
                           samsung,pin-drv = <3>;
                      };
                  sd2_busl : sd2-bus-widthl {
                            samsung,pins = "gpc2-3 ' ;
                            samsung,pin- function = <2> ;
                            samsung,pin-pud = <3>;
                            samsung,pin-drv = <3>;
                  };
                      sd2_bus4: sd2-bus-width4 {
                               samsung, pins = " gpc2-4", 'gpc2-5", "gpc2-6" ;
                               samsung,pin- funct ion = <2>;
                               samsung,pin-pud = <3>;
                               samsung,［키n-（抑V = <3>;
                      };
        };
        pinctrl@14000000 {
                 gpe0: gpeO {
                          gpio-control ler ;
                           #gpio-cel ls = <2>;


                                                    74 / 312
커 널연구회佃ww.kernel.b기                                                              정재준 (r야)i3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                       3. Device Tree 실용 분석     75




                        interrupt-control ler;
                        #interrupt-cel Is = <2> ;
               };
               gpel : gpel {
                         gpio-control ler;
                         #gpio-cel ls = <2>;

                        interrupt-control ler ;
                        #interrupt-cel ls = <2> ;
               };
               g［幷0: gpfo {
                        gpio-control ler;
                        #gpio-cel ls = <2> ;

                        interrupt-control ler;
                        #interrupt-cel ls = <2> ;
               };
               g아］: 0口fi {
                      gpio-control ler;
                      #gpio-cel Is = <2> ;

                         nterrupt-control ler ;
                        #interrupt-cel ls = <2> ;
               };
               0口gO: g口gO {
                        gpio-control Ier ;
                        #gpio-cel ls = <2>;

                        interrupt巾control ler ;
                        荊nter rup卜cel ls = <2>;
                };
               gpgl: gpgl {
                        gpio-control ler;
                        #gpio-cel ls = <2> ;

                        interrupt-control ler ;
                        #interrupt-cel Is = <2> ;
               };
               gpg2: gpg2 {
                        gpio-control ler;
                        #gpio-cel Is = <2> ;

                        interrupt-control ler;
                        #interrupt-cel ls = <2> ;
               };
               야기4: g口j4 {
                      gpio-control ler;
                       #gpio-cel ls = <2>;


                                               75 / 312
커 널 연구회（ww比kerr伯l.bz)                                     정재준 (rgbi3307@nate.com)
Device Tree 상세분석 ir} 나flux Kernel 4.0                                         3. Device Tree 실용 분석




                             interrupt-control ler ;
                             #interrupt-cel Is = <2>;
                };
                ca叱gp山코： cam-叩山-a {
                       samsung,pins = "gpeO-O ' , " gpeO-1 , "gpeO-2" , "qPe0H3“,
                                       'gpeO-4' , 'gpeO-5", 'gpeO-6", 'gpeO-7 ' ,
                                       "gpel-O" , 'gpel-l '1 ;
                       samsunQ,pin나unct ion = <2>;
                       samsung , 이十叩d = <0>;
                       samsunQ,pin-drv = <0>;
                };
                cam_g口jo_b: cam-叩jo七 {
                         samsung,pins = "gpfo-0 ' , "gpfo-1 ' , "gpf0-2' , 'gpf0-3",
                                          " gpfl-0 ' , 'gpfl-l ' , n gpfl-2", n gpfl-3";
                         samsung,pin- function = <3> ;
                         samsung,pin-pud = <0>;
                         samsung , 이十먀V = <(:)>;
                };
                cam_ i2c之加s: cam니2c？山S {
                         samsung,pins = 'gpfo-4' , 'gpfo-51' ;
                         samsung,pin- function = <2>;
                         samsung,pin-pud = <3>;
                         samsung ,pin寸（打V = <0>;
                 };
                cam_sp너_bus: cam나sp ii尸bus {
                        samsung,p ins = 'gpeO-4' , 'gpe0-5 ' , 'gpt0-2", 'gpfo-3 ' ;
                        samsung,pin-t unction = <4> ;
                        samsung , pin가川d = <0>;
                        samsung,pin-drv = <0>;
                };
                cam i2cl加s: cam니2c卜加5 {
                        samsung,pins = "gpfO-2", " gpfO-3' ;
                        sa肥ung,pin- f unction = <2> ;
                        samsung,pin-pud = <3>;
                        samsung,pin-drv = <0>;
                };
                cam 12c0나bus: cam니2c아山S {
                         samsung,pins = 'gpfo-O ' , 'gpfO-l ' ;
                         samsung,pjn- f unction = <2>;
                         samsung,pin-pud = <3>;
                         samsung,pin-drv = <0>;
                };
                 cam_spi 0_bus: cam-sp jO-bus {
                           samsung,pins = "gpfl-O", "gpfl-l ' , 'gptl-2 ' , 'gpfl-3' ;
                           samsung,pin- f unction = <2> ;
                           sarnsung,pin-pud = <0>;
                           samsung,pin-drv = <0>;
                 };
                     cam_bayrgb_bus: cam-bayrgb-bus {

                                                 76 / 312
커 널 연구회佃I,'사니,.kerne .뇨）                                                    정재준 (r야)i3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                          3. Device Tree 실용 분석   77




                          sanisung,pins = " gpgO-O ' , ' gpgO-1' , gpg0-2", 'gpgO-3",
                                            "gpgO-4", 'gpgO-5", "gpgo-6", " gpgO-7' ,
                                            'gpgl-O ' , 'gpgl-l ", ngpgl-2' , 'gpgl-3' ,
                                             'gpg1-4' , n9口g]1511, 'ppgl-6' , "gpgl-7' ,
                                            ng口q210 " ;
                          samsunp,pin- f unction = <2>;
                          samsung,pin-pud = <0>;
                          samsung,pin-drv = <0>;

       };
                 };
       미nctr l@14010000 {
                gpa0: gpaO {
                          pp ic-control ler;
                          #gpio-cel ls = <2>;

                          interrupt-control ler;
                          #interrupt-cel ls = <2>;
                 };
                gpal : gpal {
                         ppio-control ler;
                          #gpio-cel ls == <2>;

                         interrupt-control ler;
                         削nter rup卜cel ls = <2>;
                 };
                ppa2: gpa2 {
                         gpio-control ler;
                         #g口10小cel ls == <2>;

                          interru아叱ontrol ler;
                          #interrupt-cel Is = <2>;
                };
                ppbO: gpbO {
                         gpio-qontrol ler;
                         #gp i o-ce1 Is = <2>;

                         interrupt-control ler;
                         #interrupt-cel ls = <2>;
                };
                gpbl: gpbl {
                         gpio-control ler;
                         #gpio-cel ls = <2>;

                         interrupt-control ler;
                         #interrupt-cel ls = <2>;
                };
                gpb2: gpb2 {
                         gpio-cpntrol ler;
                         #gpio-cel ls = <2>;


                                                 77/ 312
커 널 연구회 (www.kern이b기                                                       정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                3. Device Tree 실용 분석




                              interrupt-control ler;
                              쒸nterru아-cel ls = <2> ;
               };
               gpb3: gpb3 {
                        gpio-control ler;
                        #gpio-cel ls = <2>;

                              interrupt-control 1 er;
                              #interrupt-cel ls = <2>;
               };
               gpb4: Qpb4 {
                        gpio-control ler;
                        #gpio-cel Is = <2>;

                              interrupt-control 1 er;
                              #interrupt-cel ls = <2>;
               };
               gphO: gpho {
                        gpio-control ler;
                        #gpio-cel ls = <2>;

                              interrupt-contr01 1er ;
                              쒸nterru아｛el Is = <2>;
                };
               uart0Hdata: uartO-data {
                        samsung,p ins = 'gpaO-O ", " gpaO-1 ' ;
                        samsung,pin- f unction = <2>,
                        samsung ,이n-四（J = <0>;
                        samsung ,이n-먀V = <0>;
                    };
                uart0Hfct1: uartO- fctl {
                         samsung,pins = "gpaO-2", 'gpaO-3";
                         samsung,pin- funct ion = <2>;
                         samsung ,이n기川（J = <(:)>;
                         samsung,pin-drv = <0> ;
                    };
                    uartLdata: uartl-data {
                            samsung ,pins = "gpaO-4", "gpaO-5";
                            samsung,pin- funct ion = <2> ;
                            samsung,pin-pud = <0>;
                            samsung ,口in-（打V = <0>;
                     };
                    uar ti 扼tl : uar너나아 1 {
                             samsung,pins = "gpao-6 ' , 'gpaO-7日;
                             samsung,pin- funct ion = <2>;
                             samsung,pin-pud = <0>;
                             samsung,pin-drv = <0>;
                         };
                                                  78 / 312
커 널 연구회（www.kernel.b기                                               정재준 (r야키3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                       3. Device Tree 실용 분석     79




               i2c2_bus: i2c2-bus {
                        samsung,pins = " gpaO-6 ' , 「 gpaO-7 ' ,
                        samsung,pin- function = <3> ;
                        samsung,pin-pud = <3>;
                        samsung,pin-drv = <0>;
               };
               uart2_data: uart2-data {
                        samsung,pins = "gpal-O ' , "gpal-l ' ;
                        samsung,pin- funct ion = <2>;
                        samsung,pin-pud = <0>;
                        samsung,pin나（打V = <0>;
               };
               uart2_tctl : uart2-tctl {
                        sarnsung,pins = 'gpal-2", "gpal-3' ;
                        samsung,pin- f unction = <2> ;
                        samsung,pin-pud = <0>;
                        samsunq,pin-drv = <0>;
               };
                i2c3_bus: i2c3-bus {
                         samsung,pins = 'gpal-2'' , 'gpal-3 ' ;
                         samsung,pin- funct ion = <3>;
                         samsung,pin-pud = <3>;
                         samsung,pin-drv = <0>;
                };
               uart3_data: uart3-data {
                        saoisung,pins = 'gpal-4 ' , 'gpal-51' ;
                        samsung,pin- funct ion = <2> ;
                        sanisung,pin-pud = <0>;
                        samsung,pin-drv = <0>;
                };
               spiO_bus: spiO-bus {
                        samsung, p ins = 'gpa2-O' , " gpa2-1" , 'gpa2-2", "gpa2-3느
                        sainsung,pin- f unction = <2>;
                        samsung,pin-pud = <3>;
                        samsung,pin-drv = <0>;
               };
                sp너mbus: 바）너-bus {
                        samsunu,pins = ''qpa2-4", "gpa2-6' , ''gpa2-7";
                        sainsung,pin- fUnct ion = <2> ;
                        samsung,pin小pud = <3>;
                        sanisung, pin小drv = <0>;
                };
                    i2c4_hs_bus: i2c4-hs-bus {
                             samsung,pins = n gpa2可, "gpa2-1' ;
                             samsung,pin- function = <3> ;
                             samsung , 이 m叩d == <3>;
                             samsung , 이n-먀V = <0>;
                };
                                                79 / 312
커 널 연구회（www.kernekbz)                                                     정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니nux Kerr伺 4.0                                           3. Device Tree 실용 분석    80




              i2c5_hs_bus: 12c5-hs-bus {
                       samsung,pins = "gpa2-21' , "gpa2-311 ;
                       sarnsung,pin- f unction = <3> ;
                       samsung,pin-pud = <3>;
                       sarnsung,pin-drv = <0>;
              };
              i2sl_bus: i2sl-bus {
                       samsung,pins = 'QpbO-O ' , "gpbO-l '' , 'qpb0-21' , 'gpbO-3 ' ,
                                            'gpb0-41' ;
                       sauisung,pin- funct ion = <2> ;
                       sarnsung,pin-pud = <0>;
                       samsung , r키n-（打V = <0>;
              };
              pcm1Hbus: pcml-bus {
                       samsung,pins = 'gpbO-O", 'gpbO-l ", 'gpbO-2' , "gpb0-3' ,
                                         'gpbO-4";
                       samsung,pin-function = <3> ;
                       samsung,pin-pud = <0>;
                       samsung,pin-drv = <0>;
              };
               i2s2_bus: i2s2-bus {
                        samsung,pins = 'gpbl-O ' , "gpbl-l , 'gpbl-2", 'gpbl-3",
                                            'gpbl-41' ;
                        sainsung,pin나 unction = <2>;
                        samsung,pin-pud = <0>;
                        samsung ,이m먀V = <0>;
               };
              pcm2_bus: pcm2-bus {
                       samsung,pins = 'gpbl-O ' , 'gpbl-l ", 「 gpbl-2", " gpbl-3 " ,
                                           "gpbl-4";
                       samsung,pin- funct ion = <3>;
                       sarnsung,pin-pud = <0>;
                       samsung,pin-drv = <0>;
              };
              spdif_bus: spd나寸）us {
                       sainsung,pins = "gpbl-O", "gpbl-l ' ;
                       samsung,pin- function = <4>;
                       samsung,pin-pud = <0>;
                       samsung,pin-drv = <0>;
              };
              spi2_bus: sp12-bus {
                       sarnsung,pins = "gpbl-l ", "gpbl-3' , 'gpbl-4 ' ;
                       samsung,pin- f unction = <5>;
                       sarnsung,pin-pud = <3>;
                       samsung,pin-drv = <0>;
              };
               12c6_hs_bus: 12c6-hs-bus {
                        samsung,pins = 'gpbl-31' , 'gpbl-4";
                        samsung,pin- f unction = <4>;

                                              80/ 312
커 널 연구회（小/'사w.kern이.b기                                                     정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kern& 4.0                                3. Device Tree 실용 분석




                         samsung, p나）1口ud = <3>;
                         samsung,pin-drv = <0>;
                },
               F川vmO out : p叫mO-out {
                          samsung,pins = n gpb2-0 ;
                          samsung,pin- f unction = <2>;
                          samsung,pin-pud = <0>;
                          samsung,pin-drv = <0>;
               };
               pwnl］寸out : 口wnil -out {
                          samsung,pins = "gpb2-1";
                          samsung,pin- funct ion = <2> ;
                          samsung，口ir｝가川d = <0>;
                          samsung,pin-drv = <0>;
                };
               pwm2_out: pwm2-out {
                        sainsuhg , 이ns = 'gpb2尸2'느
                        samsung,pin- funct ion = <2> ;
                        samsung,pin-pud = <0>;
                        samsung,pin-drv = <0>;
                };
               p升n3_out: p베m3-out {
                        samsung,pins = "q口b213n;
                        samsung,pin-t unction = <2>;
                        samsung,pin-pud = <0>;
                        samsung,pin-drv = <0>;
                };
                i2c7_hs_bus: i2c7寸）s-bus {
                         samsung,pins = 'gpb2-2", '' gpb2-3";
                         samsung,pin- funct ion = <3>;
                         samsung，口in巾ud =; <3>;
                         samsung,pin-drv = <0>;
               };
               i2c0_bus: i2c0小bus {
                        samsurig,pins = 'gpb3-0", "gpb3-1 ' :
                        samsung,pin- funct ion = <2>:
                        samsung,pin-pud = <3>;
                        samsung,pin-drv = <0>;
               };
                i2cl_bus: i2cl-bus {
                         samsung,pins = 'gpb3-2 ' , 'gpb3-3 ' ;
                         samsung,pin- function = <2>;
                         samsung,pin-pud = <3>:
                         samsung,pin-drv = <0>;
               }:
               i2c8_hs_bus: i2c8-hs-bus {
                        samsung,pins = 'gpb3-4", 'gpb3-5 ' ;
                        samsung,pin- funct ion = <2> ;

                                               81 / 312
커 널 연구회佃ww.kern이.bz)                                              정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                           3. Device Tree 실용 분석    82




                          samsung，口In巾ud = <3>;
                          sarnsung,pin-drv = <0>;
                };
                i2c9_hs_bus: 12c9-hs-bus {
                         samsung,pins = 'gpb3-6n, " gpb3-7 " ;
                         samsung,pin- funct ion = <2>;
                         samsung,pin-pud = <3>;
                         sarnsung, pin尸（打V = <0> ;
                };
                 2c10_hs_bus: 12c10-hs-bus {
                         sainsung,pins = ' gpb4-O ", "gpb4-1 ' ;
                         samsung,pin- f unction = <2> ;
                         sanisung , 이 n-叩（i = <3>;
                         samsung,pin-drv = <0>;
                };
       };
       口inctrl@03860000 {
                gpz: gpz {
                          gpio-control 1 er;
                          #gpio-cel ls = <2>;

                          interrupt-control ler;
                         ！시nter ru아兀el Is = <2> ;
                },
                 i2s0_bus: i2s0-bus {
                          samsung,pins = 'gpz-O " , ' gpz-1' , "gpz-2", " gpz-3 " ,
                                                'gpz-4' , 'gpz-5' , Ugpz_6fl ;
                          sanisung,pin- t unction = <2> ;
                          samsung , 이 m텍（J = <0> ;
                          sarnsung,pin-drv = <0>;
                 };
        };
};
위에서 핀들의 사용 용도를 정의할 때 다음과 같은 속성들을 사용한다．


samsung,pin- function: 입출력 방향 설정．
samsung,pifl-val: 핀 출력버퍼의 초기값．
samsufig,하n-pud: 풀업／다운 설정．
samsung,pin-drv: 드라이브 강도 설정．
samsung, 이n-pud-pdn: 파워 다운 모드에서 풀업／풀다운 설정．
samsurig,pin-山v-pdn: 파워 다운 모드에서 드라이브 강도 설정．


예를들면：

                                                82 I 312
커널연구회佃ww.kernel.bz)                                                          정재준 (rgbi3307@nate.com)
Device 가ee 상세분석 in Linux Kernel 4.0                                                 3. Device Tree 실용 분석   83




samsung,pin-function = <# >1,
핀의 입출력 방향：＃이 0이면 입력용도, ］이면 출력용도．


samsung,pin-pud = <#>;
디폴드값（풀업／풀다운）: ＃이 0이면 풀업다운 없음，］이면 풀다운（Low), 3이면 풀업（High).




3.10 AMBA 표현
A卜月BA(Advanced 卜川Cr야ontr에er Bus Architecture) 버스 구조는 exynos5420.dtsi 파일에 다음과 같
이 기술 되어 있댜．


       amba {
                 #address-cel ls = <1> ;
                 #size-cel ls = <1> ;
                 compat 比니e = "arm, amba寸）us " ;
                  nterrupt-parent = <&gic>;
                 ranges;

                 adma: adma@03880000 {
                          corn口at 比）le = "arm , 이330' : "arm , 口r i mece I I ' ;
                          reg = <0x03880000 oxl000> ;
                          interrupts = <0 110 0> ;
                          clocks = <&clock audss EXYNOS ADMA> ;
                          이ock-names = " apb下）C나；" ;
                          #drna-cel ls = ci> ;
                          #dma-channels = <6> ;
                          #dma-requests = <16> ;
                 };
                 pdmaO: pdma@121A0000 {
                          compat 吐니e = "arm，이330 " , "arm，口r i mece I I " ;
                          reg = <0x121A0000 oxl000>;
                          interrupts = <0 34 0> ;
                          clocks = <&clock CLK PDMAO>;
                          이ock-names = 「 apb_pc나（「 ;
                          #dma-cel ls = <仁;
                          #dma-channels = <8> ;
                          #dma-requests = <32> ;
                 };
                 口dmal : 口dma@121B0000 {
                           compatible = "arm, p1330", "arm, pr imecel l " ;
                           reg = <0x121B0000 0xl000> ;
                           interrupts = <0 35 0> ;
                           clocks = <&clock CLK PDMA1> ;
                           이ock-names = "apb_pc나；" ;
                           #dma-cel Is = <1> ;


                                                    83 / 312
커 널 연구회佃ww.kern이I끄）                                                                정재준 杓너3307@nate.con가
Device 가ee 상세분석 in Linux Kerr倒 4.0                                           3. Device Tree 실용 분석     84




                           #dma-channels = <8>;
                           #dma-requests = <32>;
                 };
                 ndmaO: mdrna＠化8000凹 {
                          compatible = 'arm,p1330' , 'arm,prirnecel l ";
                          reg = <0x10800000 0xl000>;
                           interrupts = <0 33 0>;
                          clocks = <&clock CLK_MDMAO>;
                         （기ock-names = "a以)_pclk " ;
                          #dma-cel ls = <1> ;
                          #dma-channels = <8>;
                          #dma-requests = <1>;
                 };
                 mdmal: mdma@11C10000 {
                          compatible = "arm,p1330", 'arm,primecel l ' ;
                          reg = <0x11C10000 0x1000>;
                          interrupts = <0 124 0> ;
                          clocks = <&clock CLK_MDMA1>;
                          clock-names = "apb.pclk ' ;
                          #dma-cel ls = <1>;
                          #dma-channels = <8>;
                          #dma나eques始 = <]>;
                            /*
                                 * MDMA1 can support both secure and non-secure
                                 * AXl transactions. When this is enabled in the kernel
                                 * for boards that run in secure mode, we are getting
                                 * imprecise external aborts causing the kernel to o야s.
                                 六／
                            status = 'disabled";
                      };
       };
3.11 125 표현
exynos5420.dtsi 파일에 다음과 같이 정의 되어 있다．


       i2s0: i2s@03830000 {
                 compatible = 'samsung,exynos5420- i25";
                 reg = <0x03830000 0xloO>;
                 dmas = <&adma 0
                           &adma 2
                           &adma 1> ;
                 dma-names = 나x ' , "rx ' , ' tx-sec ";
                 clocks = <&clock_audss EXYNOS_12S_BUS> ,
                           <&c I ock_audss EXYNOS_ I 2S_BUS> ,
                           <&C I ock_audss EXYNOSSCLK_ I 2S>;
                 clock-names = " i iS", "i2s.中opc나；0 ' , ' i2s_opclkl " ;
                 samsung, idma-addr = <0x03000000>;

                                                   84 / 312
커 널 연구회（ww'사.kernel.b기                                                      정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                      3. Device Tree 실용 분석     85




                pinctr I-names = "default ";
                pinctrl-0 = <8 i 2s0mbus>;
                status = "disa L니 ed" ;
       };
       i2sl: i2s@12D60000 {
                compat 比니e = n samsung, exyn0s5420니 2s";
                reg = <0x12060 000 oxlOo>;
                dmas = <&pdmal 12
                             &pdma 1 11>;
                dma-names = n t x ", "rx ' ;
                clocks = <&clc ck CLK그2S仁 , <&clock CL凡吼LK그2S1>;
                clock-names = " i is", "12s_opclko";
                p i nct r I-names ="default ";
                pinctrl-0 = <8 i 2s1_bus>;
                status = "dise bled";
        };
        i2s2: i2s@12D70000 {
                 compatible = ' samsung,exyn0s5420- i2s";
                 reg = <0x12D7C 000 oxloo> ;
                 dmas = <&pdmaC 12
                           &pdinaDii>;
                 dma-names = 11t x ", "rx";
                 clocks = <&clc ck CLK_ l2S2>, <&clock CLK_SCLK_12S2>;
                 clock-names = "u is", "12s_opc나；o";
                 pinctr I-names = "default ";
                 pinctrl-0 = <8 i2s2 bus>;
                 status = "disc bled";
        };
3.12 SP1 표현
exynos5420.dtsi 파일에 다음과 같이 정의 되어 있다．


      印匕0: spi@12d20000 {
              compatible = "1 amsung,exynos42lO-sp i ' ;
                                Q
                                나


                                八J
              reg = <0x12d201 00 0xloo>;
                                八J
              interrupts = <I 68 0>;
              dmas = <&pdmaO 5
                        却dmaO 4>;
              dma-names = ' tx
              #address-cel Is =     ;<1>
              #size-cel ls = <0>;
              pinctr I-names = "default ";
              pinctr卜O = <&Spi0Hbus>;
              clocks = <&clock CLK_SPIO>, <&clock CLK_SCLKSPIO> ;
              clock-names = n S이 " , "sp匕busclkO' ;
              status = 'disab led";
       }

                                               85 / 312
커널연구회（www.kernel,bz)                                                     정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kern이 4.0                                      3. Device Tree 실용 분석




       spi_1 : spi@12d30000 {
                 compatible = "samsung,exynos4210-spi ';
                 reg = <0x12d30000 0xlOO>;
                  interrupts = <0 69 0>;
                 dmas = <&pdmal 5
                           &pdmal 4>;
                 dma-names = "tx ' , "r x";
                 #address-cel Is = <1>;
                 #size-cel Is = <0>;
                 pinctr I-names = "default ";
                 이nctr 1-0 = <&sp너bus>;
                 clocks = <&clock CLI(..SPl1>, <&clock CLK_SCLK_SP너>;
                 이ock-names = "5口i " , "5口L나busc나（0 " ;
                 status = "disabled";
       };
       sp匕2: s口咆］2d40000 {
               compatible = "samsung,exynos42lo-spi ";
               reg = <0x12d40000 0xl0o>;
               interrupts = <0 70 0>;
               dmas = <&pdma0 7
                         &pdma0 6>;
               dma-names = 'tx ", "rx";
               #address-cel ls = <1>;
               #size-cel ls = <0>;
               pinctr I-names = "default ";
               pinctr卜0 = <&S이之山5>;
               clocks = <&clock CLK_SP12>, <&clock CLK_SCLK_SPI2>;
               이ock-na肥5 = 'spi " , "spLbusc나；0느
               status = "disabled";
        };
3.13 UART 표현

exynos5.dt引 파일에 다음과 같이 주소 정보가 정의 되어 있다．


        seria匕0: serial@12C00000 {
                compatible = "samsung,exynos42lo-uart ";
                reg = <0x12C00000 oxioo>;
                interrupts = <0 51 0>;
        };
            serial_i: serial@12C10000 {
                     compatible = "samsung,exynos42lo-uart ";
                     reg = <0x12C10000 小ioo>;
                      interrupts = <0 52 0>;
             };

                                                  86 / 312
커 널 연구회（www.kern이.bz)                                                   정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                     3. Device Tree 실용 분석     87




       seria匕2: serial@12C20000 {
               compatible = 'samsunQ,exyn0s4210-uart ";
               reg = <Ox12C20000 0x100>;
               interrupts = <0 53 0> ;
       };
       serial_3: serial@12C30000 {
                compatible = 'samsung,exynos4210-uart ' ;
                reg = <Ox12C30000 0x100> ;
                interrupts = <0 54 0>;
       };

exynos5420.dtsi 파일에 다음과 같이 클락 정보가 정의 되어 있다．


       uart_O: serial@12C00000 {
                 clocks = <&clock CLK_UARTO>, <&clock CLKSCLK_UARTO>;
                 clock-names = 'uart " , "clk_uart느baudO ' ;
        };
       uar그: serial@12C10000 {
              clocks = <&clock CLK_UART1>, <&clock CLKSCLK_UART1>;
              이ock-names = 'uar t ' , 'c나；卞uar t小baudO ' ;
        };
       uart2: serial@12C20000 {
               clocks = <&clock CLK_UART2> , <&clock CLK_SCLK_UART2>;
               clock-names = 'uart ' , 'c냐； uarLbaudO";
        };
       uart_3: serial@12C30000 {
                clocks = <&clock CLK_UART3>, <&clock CLK_SCLK_UART3>;
                clock-names = 'uart ", " c나_
                                           ;uarLbaudO";
       };




3.14 P＼사卜A 표현
exynos5420.dtsi 파일에 다음과 같이 정의 되어 있다．


      ［川［n   口win丘서2dd0000 {
                  compatible = " samsung,exynos4210-pwm";
                  reg = <0x12dd0000 0x100> ;
                  samsung, pwm-outputs = <0>, <1>, <2>, <3>;
                  #p베m-cel ls = <3>;
                  이0（水5 = <&clock CLK小F뾔M>;
                  clock-names = n timers' ;
        };



                                               87 / 312
커널연구회（www.kernel.bz )                                                   정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니nux Kernel 4.0                            3. Device Tree 실용 분석     88




3.15 ADC 표현
exynos5420.dtsi 파일에 다음과 같이 정의 되어 있다．


      adc: adc@12010000 {
                compatible = "samsung,exynos-adc-v2";
                reg = <0x12010000 0x100>, <0x10040720 0x4>;
                interrupts = <0 106 0> ;
                clocks = <&clock CLK_TSADC>;
                clock-names = "ado";
                #io-channel-cel Is = <1>;
                i 0-channel -ranges;
                status = "disabled";
       };
3.16 I2C 표현
exyn0s5420.dtsi 파일에 다음과 같이 정의 되어 있다．


       i2c_0: 12c@12C60000 {
                 compatible = "samsung, s3c2440-12c";
                 reg = <0x12C60000 oxloo>;
                 interrupts = <0 56 0>;
                 #address-cel ls = <1> ;
                 #size-cel Is = <0>;
                 clocks = <&clock CLK_ l2C0>;
                 clock-names = n i2Cn ‘,
                 pinctr I-names = "default ";
                 pinctr卜0 = <&i2c0_bus>;
                 status = "disabled";
        };
        12c 1: i2c@12C70000 {
                 compatible = "samsung, s3c2440- i2c ";
                 reg = <0x12C70000 oxlOo>;
                  interrupts = <0 57 0>;
                 #address-cel ls = <1>;
                 #size-cel ls = <0>;
                 clocks = <&clock CLKJ2C1>;
                 clock-names = n i2Cn ;
                 pinctr I-names = "default ";
                 pinctrl-0 = <&i2cl_bus>;
                 status = "disabled";
        };

                                               88/ 312
커 널 연구회（www.kernet.b기                                         정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                        3. Device Tree 실용 분석   89




        i2c_2: i2c@12C80000 {
                 compatible = "samsung, s3c2440-i2c";
                  reg = <0x12C80000 oxloo>;
                  interrupts = <0 58 0>;
                 #address-cel ls = <1>;
                 #size-cel Is = <0>;
                 clocks = <&clock CLK_12C2>;
                 clock-names = ' 12c ' ;
                 pinctr I-names = 'default ";
                 pinctrl-0 = <&i2c2_bus>;
                  status = 1'disabledn;
        };
        12c_3: i2c@12C90000 {
                 compatible = 'samsung, s3c2440- i2c ";
                 reg = <Ox12C90000 0xlOo>;
                  interrupts = <0 59 0> ;
                 #address-cel Is = <1>;
                 #size-cel ls = <0>;
                 clocks = <&clock CLK I2C3>;
                 이oc小叱mes = "i2c " ;
                 pinctrl-nanies = "default ";
                 pinctrl-0 = <&i2c3_bus>;
                  status = "disabled";
        };
       hsi2c_4: i2c@12CA0000 {
                compatible = 'samsung,exynos5-hsi2c '1 ;
                reg = <0x12CA0000 0xl000>;
                interrupts = <0 60 0>;
                #address-cel ls = <1> ;
                #size-cel ls = <0>;
                pinctr I-names = "default ";
                pinctrl-0 = <&i2c4_hs_bus>;
                clocks = <&clock CLKmUSIO> ;
                clock-names = 'hsi2c";
                status = "disabled";
       };
        hsi2c_5: i2c@12CB0000 {
                 compatible = "samsung,exynos5-hsi2c ' ;
                 reg = <0x12CB0000 oxl000>;
                 interrupts = <0 61 0>;
                 #address-cel ls = <1> ;
                 #size-cel Is = <0>;
                 pinctr I-names = "default ";
                 pinctr卜0 = <&i2c5_hs_bus>;
                 clocks = <&clock CLK US너>;
                 clock-names = 'hsi2c ";
                 status = "disabled";
         };
       hsi2c_6: i2c@12CC0000 {
                compatible = 'samsung,exynos5-hsi2c ' ;
                reg = <0x12CC0000 小l000>;
                interrupts = <0 62 0>;

                                               89 I 312
커 널 연구회 (ww比kern이. t끄）                                     정재준 杓bi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                        3. De＼月ce Tree 실용 분석   90




                #address-cel ls = <1>;
                #size-cel Is = <0>;
                pinctr I-names = "default ' ;
                pinctr卜0 = <&12c6_hs_bus>;
                clocks = <&clock CLK US12> ;
                clock-names = "hsi2c";
                status = 'disabled";
       };
       hsi2c_7: i2c1@12CD0000 {
                compatible = "samsung, exynos5-hsi2c ";
                req = <Ox12CD0000 0x1000>;
                interrupts = <0 63 0>;
                #address-cel ls = <1>;
                #size-cel Is = <0>;
                pinctr I-names = "default ";
                pinctr卜0 = <&i2c7_hs_bus>;
                clocks = <&clock CLK_US13>;
                clock-names = "hsi2c ";
                status = 'disabled";
        };
       hsi2c_8: i2c@12E00000 {
                compatible = "samsung,exynos5-hsi2c";
                reg = <Ox12E00000 0x1000>;
                interrupts = <0 87 0>;
                #address-cel ls = <1> ;
                #size-cel Is = <0>;
                pinctrl-names = "default ";
                pinctr卜0 = <&i2c8_hs_bus>;
                clocks = <&clock CLK US14>;
                clock-names = "hsi2c";
                status = "disabled";
       };
       hsi2c_9: i2c@12E10000 {
                compatible = "samsung,exynos5-hsi2c ";
                reg = <Ox12E10000 0xl000>;
                interrupts = <0 88 0>;
                #address-cel ls = <]>;
                #size-cel Is = <0>;
                pinctr I-names = "default ";
                pinctr卜0 = <&i2c9_hs.mbus>;
                clocks = <&clock CLK_USI5>;
                clock-names = "hsi2c ";
                status = "disabled";
       };
       hsi2c_10: i2c@12E20000 {
                compatible = "samsung,exynos5-hsi2c ";
                reg = <Ox12E20000 0x1000>;
                interrupts = <0 203 0>;
                #address-cel ls = <1>;
                #size-cel ls = <0>;
                pinctr I-names = "default ";
                pinctr卜0 = <&i2clOhs bus>;

                                                90 / 312
커 널 연구회（w납八vkern飢b기                                        정재준 （四b日307@nate.com)
Device Tree 상세분석 In 나nux Kernel 4.0                                         3. Device Tree 실용 분석    91




                이ocks = <&C I ck CLK_US16> ;
                이ock-names = "hsi2c";
                status = "disi bled" ;
       };
3.17 USB 표현
exynos5420.dtsi 파일에 다음과 같이 정의 되어 있다．


      usbdrd3_O: usb@12000000
                compatible = 'H ,amsung , exyn0s5250-dwusb3";
                clocks = <&clo( ,k CLK IJSBD300>;
                clock-names = u5bdrd30";
                #address-cel Is =     ;
                                      <1>
                #size-cel ls =  .1>;
                ranges;

                usbdrd dwc3 Q: （畑c3 {
                         compa ible = "snps,dwc3";
                         reg = <0x12000000 0xl0000>;
                         interi upts = <0 72 0>;
                         phys = <&usbdrd. phy0 0>, <&usbdr냐hy0 1>;
                         phy-ni mes = "usb2-phy", "usb3-phy느
                };
        };
       usbdr d.phy0: phy@121000 10  {
                 compatible = ' ;amsung, exynos5420-usbdrd-phy느
                 reg = <0x121001100 oxl00>;
                 clocks = <&clo :k CLK_USBD300> , <&c lock CLK_SCLK_USBPHY300> ;
                 clock-names = 口hy " , he尸 ;
                 samsung, pmu-sy ;con = <&pmu_system..control ler>;
                 却hy-cel Is = < >;
        };
       usbdrd3_1: usbl@12400000 {
                com口at 仕니e = 「 ;amsung, exynos5250-dwusb3";
                clocks = <&clo :k CLK USBD301> ;
                clock-names = usbdrd30";
                #address-cel Is =    ;<1>
                #size-cel ls = :1>;
                ranges;

                usbdrd dwc3 1: （抽c3 {
                         compa ible = "snps, dwc3";
                         reg = <Ox12400000 0x10000>;
                         inter upts = <0 73 0>;
                         phys = <&usbdrd_phyl 0>, <&usbdrd. 巾yl 1> ;
                         phy-ni mes = "usb2-phy", "usb3-phy느
                };
                                               91 I 312
커 널 연구회（WW\사．kernel.b기                                                    정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kern이 4.0                                     3. Device Tree 실용 분석    92




       };
       usbdrd_phyl: phy@12500000 {
                compatible = "samsung ,exynos5420-usbdrd-phy ' ;
                req = <0x12500000 0x100>;
                clocks = <&clock CLK_USBD301>, <&clock CLK_SCLK_USBPHY301> ;
                clock-names = "phy ", "ret ' ;
                samsung,pmu-syscon = <&pmu_system_control let>;
                #phy-cel ls = <1>;
       };
       usbhost2: usb@12110000 {
                compatible = 'samsung,exynos4210-ehci ";
                reg = <0x12110000 0xlOO>;
                interrupts = <0 71 0>;

                clocks = <&clock CLK_USBH20> ;
                clock-names = ."usbhost ' :
                #address-cel ls = <1> ;
                #size-cel Is = <0>;
                port@0 {
                         reg = <0>;
                         phys = <&usb21-phy 1>;
                };
       };
       usbhostl: usb@12120000 {
                compatible = "samsung,exynos4210-ohci H ;
                reg = <0x12120000 小lOO> ;
                interrupts = <0 71 0> ;

                clocks = <&clock CLK USBH20> ;
                clock-names = "usbhost ";
                #address-cel ls = <1> ;
                #size-cel Is = <0>;
                port@0 {
                         reg = <0>;
                         phys = <&usb2phy 1>;
                };
        };
       u5b2phy: phy@12130000 {
               compatible = "saulsung, exynos5250-usb2-phy ' ;
               reg = <0x12130000 oxlOO> ;
               clocks = <&clock CLKUSBH20>. <&clock CLK_SCLKUS甲바300>;
               clock-names = "phy ", "ret ' ;
               #phy-cel ls = <1> ;
               samsung, sysreg-phandle = <&sysreg尸systemcontrol 1 er>;
               samsung,pmureg-phandle = <&pmusystemcontrol let>;
        };
                                              92 / 312
커널연구회佃＼Nw.kern이b기                                                     정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kern& 4.0                                         3. Device Tree 실용 분석       93




3.18 TMU 표현
TMU(Therma1 Management Un仕 ）는 CPU 내부의 온도를 관리하는 용도로 exynos5420.dtsi 파일에
다음과 같이 정의 되어 있다．


       tmu_cpuo: t叩們0060000 {
                 compatible = 'samsung,exynos5420- tmu' ;
                 reg = <0x10060000 0x100>;
                 interrupts = <0 65 0>;
                 clocks = <&clock CLK_TMU>;
                 이oc小names = 나m山叩이 尸 ;
        };
       tmu_cpul: tmu@10064000 {
                compatible = " samsung,exynos5420- tmu";
                reg = <0x10064000 oxloo>;
                interrupts = <0 183 0>;
                clocks = <&clock CLK TMU>;
                이ock-names = 나mu_apb if ' ;
       };
        tmu_cpu2: tmu@10068000 {
                 compatible = 'samsung,exyn0s5420- tmu-ext- triminfo";
                 reg = <0x10068000 0x100>, <0x1006c000 0x4>;
                 interrupts = <0 184 0> ;
                 clocks = <&clock CLK_TM(J>, <&clock CLK_TMU>;
                 clock-names = "tmu_apbif ' , 'tmu_ triminfo_apbif ";
        };
        tmu_cpu3: tmu@1006c000 {
                 compatible = " samsung,exyn055420- tmu-ext-tr iminfo";
                 reg = <0x1006c000 0x100> , <0x100a0000 0x4>;
                 interrupts = <0 185 0> ;
                 clocks = <&clock CLK_TMtJ>, <&clock CLK_TMU_GPU>;
                 clock-names = ' tmu_apbif ", 'tmu_ triminto_apbif ' ;
        };
        tmu+-gpu: tmu@100a0000 {
                  compatible = n samsung,exynos5420- tmu-ext- triminfo";
                  reg = <0x100a0000 0xl00>, <0x10068000 0x4>;
                  interrupts = <0 215 0> ;
                  clocks = <&clock CLK_TMU_GPU>, <&clock CLKTMU> ;
                  이ock-names = 'trnu_a以）if' , " tmu trimin化a的i 尸 ;
        };
3.19 멀티미디어 표현
exynos5420.dtsi 파일에 다음과 같이 정의 되어 있다．


                                               93 / 312
커 널 연 구회（wwv疎帥泡bz)                                                         정재준 (rgb13307（亘）nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                      3. Device Tree 실용 분석     94




      mfc: codec11000000 {
               compatible = "samsung,mfc-v7 ' ;
                reg = <Ox11000000 0xl0000>;
                interrupts = <0 96 0>;
               clocks = <&clock CLK MFC>;
               （기ock尸names = 'mfc ' ‘,
                samsunq，口애아기把ma i n = <&mf（乙pd>;
       };
       mtc_pd: power-domain@10044060 {
                 compatible = "samsung,exynos42lo-pd ' ;
                 reg = <0x10044060 0x20>;
                 clocks = <&clock CLK_FIN_PLL>, <&c比ck CLK_MOUT_SW_ACLK333>,
                          <&c lock CLK_M0UT_USER. ACLK333>;
                 clock-names = 'oscclk ' , "pclkO", 노lkO";
        };
       msc_pd: power-domain@10044120 {
                compatible = "samsung,exynos42lo-pd";
                reg = <0x10044120 0x20>;
        };
       rnipLphy: video-phy@10040714 {
                 compatible = "samsung, s5pv2lo-mipi-video-phy";
                 reg = <0x10040714 12> ;
                 却hy兀el Is = <1>;
        };
        dsi@14500000 {
                 compatible = 'samsung,exynoss4lo-mipi-dsi ";
                 reg = <0x14500000 oxl0000>;
                 interrupts = <0 82 0>;
                 口hys = <&m巾匕phy ]>;
                 phy-names = "dsim";
                 clocks = <&clock CLK_DSIM1>, <&clock CLK_SCLK_NIPI1>;
                 이ock-names = "bus ci卜；" , 'p1匕c나（n ;
                 #address-cel ls = <1>;
                 #size-cel ls = <0>;
                 status = "disabled";
         };
         fimd: fimd@14400000 {
                  이ocks = <&clock CLK_SCLK 디MD1>, <&clock CLKJ기씨기＞;
                  이ock-names = 'sc나（ f i md ' , 냐 imd" ;
         };
       hdmi : hdmi@14530000 {
                  compatible = " samsung,exyn0s5420-hdmi n ;
                  reg = <0x14530000 0x70000>;
                  interrupts = <0 95 0> ;
                  clocks = <&clock CLK_HDMl>, <&clock CLK_SCLK_HDMI>,
                            <&clock CLK_DOUT_PIXEL>, <&clock CLK_SCLKHDMIPHY>,
                            <&clock CLK MOUT 1-IDMI>;

                                              94 / 312
커 널 연구회（www.kern이b기                                                      정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kern이 4.0                                      3. Device Tree 실용 분석     95




                이ock-names = 'hdm i , "Sc나； hdm i ' , "sd1卜；_p i xe尸，
                          "sclk_hdrniphy ", "mouLhdmi " ;
                phy = <&hdmiphy>;
                samsung, syscon-phandle = <&pmu_system_control ler>;
                status = 'disabled";
       };
       hdmiphy: hdmiphy@145D0000 {
                reg = <0x145D0000 0x20>;
       };
       mixer: 川xe旭14450000 {
               compatible = "samsung,exynos5420-mixer " ;
               reg = <0x14450000 oxl0000>;
               interrupts = <0 94 0>;
               clocks = <&clock CLK_MIXER>, <&clock CLK_SCLK_HDMI>;
               clock-names = "mixer ", "sc나；_hdmi ";
       };
       gsc_0: video-scaler@13e00000 {
                compatible = "samsung,exynos5-gsc ";
                reg = <0x13e00000 oxl000>;
                interrupts = <0 85 0>;
                clocks = <&clock CLK_GSCLO>;
                clock-names = 'gsc I ' ;
                samsung巾애아K幻ma i n = <&gsc中pd>;
       };
       gsc_1 : 미de于凹키아이扼10000 {
                compatible = "samsung, exynos5-gsc ";
                reg = <0x13e10000 小l000>;
                interrupts = <0 86 0>;
                clocks = <&clock CLK GSCL1>;
                clock-names = "gscl ";
                samsung,power-domain = <&gsc_pd>;
        };
                                              95 / 312
커널연구회（www.kernel戶bz )                                                   정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                               4. Device Tree 실습    96




4. Device Tree 실습




                                                           + 필자의 주말농장0私1 찍은 수밖


이번장부터는 삼성 Exynos5420 AP가 탑재된 Arndale Octa Board에 리눅스 커널 4.0 버전을 포팅
하여 디바이스 트리를 익혀보도록 하자.                   Arndale Octa Board는 아래 사이트에서 관련정보를 확인
할 수 있고 온라인 구매도 가능하다．


Arndale Octa Board 관련 정보 홈페이지 링크：
http://www.arndaIeboard.orq/wiki/index.php/Main斗Paqe


Arndale Octa 師aid 구매 관련 링크：
http://www.arndaleboard.org/wiki/index.php/Saleschannel


위의 웹사이트（위키）에서 부트로더 , 커널 및 안드로이드 소스를 다운 받아서 포팅할 수 있도록 설
명하고 있으나, 제공하는 커널이 비교적 오래된 버전인 3.4.39이고 소스내0私］ 디바이스 트리를
사용하지 않고 있어서 디바이스 트리를 학습하기에는 부족함이 있다.                           그래서 필자는 리눅스 커 널
보관소 웹사이트（http://ww毗ernetorg）에서 최근의 리눅스 커널인 4.0 버전을 다운받아서 여기에
있는 디바이스 트리를 학습할 수 있도록 내용을 구성한다.                           단, 안드로이드 소스는 포팅하지 않고
부트로더 , 리눅스 커널, 램디스크까지만 빌드하여 Arndale Octa Board를 부팅할 예정이다． 이번장
의 내용들은 필자가 실습하여 검증한 내용들을 그대로 실었으므로 독자들께서 그대로 따라하면서
이해할 수 있을 것이다．



                                           96 / 312
커 널 연구회（ww比kerneLbz)                                          정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                            4. Device Tree 실습   97




본격적인 실습에 들어가기 전에 삼성 Exynos5420 아키텍처 이해와 개발환경 구축이 선행되어야
한다． 먼저 삼성 Exynos5420에 대해서 알아보도록 하자． 필자가 이책을 집필하는 시점에, 삼성
에서 아직 Exynos5420 데이터시트를 공개하지 않고 있어서 자세한 내용 분석은 시간이 좀더 걸릴
듯 하지만. 몇가지 공개띈 기능 위주로 내용을 요약한다．



4.1 삼성 Exynos5420 이해
삼성 Exynos5420(Exynos5 Octa）은 Galaxy 卜幻te 제품군에 탑재되었으며 ARM의 big.LITTLE 기술을
적용한 프로세서이다.              Exynos5420 안에는 8개의 코어（octo-core）가 내장되어 있다.                    8개의 코어를
2개 집합으로 분리하여， 첫번째 집합은 성능이 높은由ig) 4개의 코어들로 구성했고 두번째 집합은
성능이         낮은（니TILE)    4개의     코어들로 묶는 방식으로                  설계했다.      이러한 개념으로          인해서
''big.니ITLE"이라는 명칭이 부여 되었다．
리눅스 커널의 스케쥴러는 아래 그림과 같이 task들을 코어들에게 골고루 분산시켜서 프로세싱 성
능은 높이고 전력소모（발열）는 감소 시키는 방향으로 발전하고 있다．




간단한 task들은 Cortex-A7(LITILE）에서 수행되도록 하고, 복잡한 연산을 많이 수행하는 task들은
Cortex-A］돠너g）에서 수행되도록 하면, 아래 그래표와 같이 작업들을 효과적으로 분산 시킬 수 있
다．
                                                                 U枉好次好 快必炫湘恥礪撤

                                 （知目由tv c月岫奴m7          " " “缸
                                               /
                                                   /y
                                                   ,1     --




                                           I
     늉多口八                          /
                                       /                          呻Cortex-A15
                                                                  m咬：ortex寸Al

                          ，匕
                                   Con心-A坊蜘텨的喀P01駐

                    十，
                         才戶H却沖潘tC여I心次字 0材旨磁油gP的鹹
                 甘伍拙 C이lu-Al q peratug Poa蚣


                               Performance

                                               97 / 312
커널연구회（www1kernel.b기                                                     정재준 (rgbi3307@nate.com)
Dev心 Tree 상싸분석 in Linux Kernel 4.0                                       4. Device Tree 실습   98




삼성 Exynos5420(Arnda旭 야ta Board) 量록도




Arndale Octa Board 구성도
                                                                  p.附
                                                                 白冊t耐
                                              U" 各. 0
                                                        USIL,0    0( 鉀
                                               N.m




                                                                             Ext.rn닙 B胡牛
                                                                             打的 t Il針＜: 3陀
                                                                             存戊. ＄아쇼 U希燕事




                           O心口tay 夕ort
                                                     ！川plc釘 4i帥們
                           知UPI 0SZ／卞op



                                          98 / 312
커 널 연구회（ww比kern어. b기                                               정재준 （띠b日307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                       4. Device Tree 실습   99




       ARM Cortex-A15 MPCore (Quad core) processor, which is BIG-core.
              3.5DMIPS per core with 1.8GHz operating frequency
              32 KB(lnstruction)/32KB(Data)L1 Cache and 2MB L2 Cache
              1TB physical addressing
       ARM Cortex-A7 class MPCore (Quad core) processor, which is LITTLE-core.
              1.86 DMIPS per core with 1.2 GHz operating frequency
              32 KB(lnstruction)/32 KB(Data)L1 Cache and 512 KB L2 Cache
       Multi-format Video Hardware codec(MFC): 1920X1080@60fps
       OpenGL ES1.1/2.0/3.0, OpenCL1.1, OpenVG1.0.1, DirectX 11, Google Renderscript
       Suppo八 HDMI 1.4a interfaces with on-chip PHY
       One channel eDP output Single WQXGA
       Suppo八 MIPI DSI Standard Specification Vi.0l rl 1
       Support MIPI CSI standard specification Vl.0 Tow ports
       Support USB3.0 Host 1-channel that suppo小 SS(5Gbps) with on-chip PHY
       Support USB2.0 Device 1 -channel that' supports LS/FS/HS with on-chip PHY
       Support USB2.0 Host 2-channel that supports LS/FS/HS with on-chip PHY
       Support USB HSIC 1-channel that suppo心 480Mbps with on-chip PHY
       Support 10/100Mbps Ethernet One Port
       Support One channel e卜肋너C 4.41 DDR in 8b仕 4GB
       Support One channel SDIO 3.0
       Support One channel SD2.0
       Support Four channel high-speed UART(up to 3Mbps data rate for Bluetooth 2.0 EDR and
       IrDA 1.0SIR)
       Support Three channel high-speed SPI
       Support Three channel 24-bit 12S audio interface
       Support Four channel 12C interface support, up 400kbps
       Support Four channel HS-12C up to 3.1 Mps
       Support 24bit 96kHz Stereo CODEC
       Support Configurable GPlOs
       Support lEA Configurable Button
       Support 1 EA Configurable LED
       Hold currents up to 2.3A
       INPUT POWER DCSV




                                            99 / 312
커널연구회（ww낚／.ke毗1.1끄）                                                정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                                 4. Device Tree 실습   ]00




4.2 개발 환경 구축
아래와 같은 순으로 개발 환경을 구축하도록 하자．


    .        우분투 12.04(64비트 버전） 설치
    1        개발용 패키지들 설치
    0        크로스 컴파일러（Toolchai,가 설치



4.2.1 우분투 설치
먼저 아래 우분투 웹사이트에서 Ubuntu 12.04 (64비트 버전）을 다운 받아서 설치하도록 한다． 우
분투 64비트 버전이 아니면 크로스 컴파일러에서 오류가 발생하므로 반드시 64비트 버전을 설치
하기 바란다．


http://releases.ubuntu.com/12.04/


우분투 설치 방법은 구글에서 " 우분투 ]2.04 설치 " 라고 검색하면 참고할 수 있는 사이트들이 많이
있으므로 참조하기 바란다．



                                                                                                          ubuntu色

   Ubuntu 12.04.5 LIS (Precise Pangolin)


           Select an image
           Ub벼加 捻 d朽liii沁摠d 아"I '肥 却1거陌 of ins因es des希b因t belc州


           Desk加p CD
           The desk畑pcd 斟여晤 V어J 地 Icy Ut比n地 1升咐K沁h出anqing y｛比rcompc료針 at 심I, and at yoc茗（耶Don to in的曲 臣 penn去忙0鉀 幻旭I
           Tt出5 蜘a of cd us 낼hat mc｝료 i料料ew明빛ait to u드e. You w菰 need at lea嗽 384M氾 of R腑 to natal f民nIfli針姓

           There a陪 柶0 蜘sq田 av州帥妬, each 幻rad而酊ent t叩eof侃npu慨：

           PC (In姓 5拙6) de敬缸岸cCD
                 Fm 川most all PC됴 -t却S Inc來川ies 0目璥 m미出inesw澍II,卄야浜Mt긔아C 却pe pvc比咬缶t甘S 카at 笛most 斟 C'算c4ute四 枷am ii川1
                 婚汀Os（矗 Wiidows, as 싸에 as newer A1甲把 M配机加針'S羚螂nsbi四ad on In蛇1 莎oce胡여묘 Ch여玲e 枷四 甘 叩U 出a 孤 苡

    164哺        PC t; ;!梵4t  d哨卞t曲CD     I
                 Um比se me tot的哈 打川 auvantage of e여i띠ite心 he叱d i가l 小e ME片4（玎 EM64T arc拓佃吐出e 也g, 慰It如064,（却ten月1,
                 EM64T Xeon, C唯e 까 'If（丑j have a us恥-64缸tprocessor ma血 byAMD, nc 耳 恥沁 i始ed 知且 닦'p며壯 for 32由往 code, use
                 the lot여 x86 im因es In없e配，




                                                            100 / 312
커 널 연구회（www.kern이.bz)                                                                       정재준 (rgbi3307@ nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                             4. Device Tree 실습     101




우분투 버전은 아래와 같이 확인할 수 있다．


$ uname -a
Linux myHome2 3.13. 0-32-generic #57-precisel-Ubuntu SMP Tue Jul 15 03: 51: 20 UTC 2014 x8664 x86 64
x86_64 GNU/Linux




4.2.2 개발용 패키지들 설치
다음으로 개발 및 빌드에 필요한 각종 패키지들을 아래와 같은 순서로 설치한다．



  亡g끼키지毋 任쳐
$ sudo apt-get instal l git- core gnupg f lex bison gperf bui ld-essential W
  zip curl 1 ibc6-dev l ibncurses5-dev xllproto-core-dev W
  I ibxl］尸dcv I 比玎eadl ine6-dev I 山gi卜mesa닙Ii W
  I i bg너-mesa-dev g++-mu It i 1 山 m ng此2o口enjdk-6기dk 加fr叱Os w
  口ython-markdown I 山xm口山t i ls xsl 如roc zl 山幻귐cv

/／약 3분정도 소요됨 . . .

$ sudo apt-get update
$ su（把 apt-get instal l ia32니 山5

/／약 5분정도 소요됨 . . .




다음으로 repo를 설치한다． repo는 g仕 프로젝트를 하나로 묶어 관리할 수 있도록 python으로 만
든 실행파일이다.           대량의 소스를 다운로드할 [[II 사용하는 도구이다．




$ su root

/／루트 권한으로 실행한다．

# curl https: //storage.9000leapis. com/gi t-repo-downloads/ repo > /bin/ repo

/／아래와 같이 다운로드 메시지가 나타난다‘

% Total     % Received % Xferd    Average Speed  Time    Time    Time Current
                                    미oad 뱌) load   Total   S口ent   Left Speed
100 24081   100 24081    0       0 50192       0 小11小 小11 小 小11 小 55486

/／실행 권한 부여 한다．

# chmod a+x /bin/ repo




                                                101 / 312
커 널 연구회（www.kernel.bz)                                                     정재준 (r야키3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                            4. Device Tree 실습        102




다음으로 fastboot 프로그램을 설치한다.                     fastboot는 u-boot와 커널. 램디스크를 보드에 올릴 때

사용하는 도구이다．



fastboot 싫치
# add-apt- repos tory ppa: nh larimogard/webupd8

You are about to add the fol lowing PPA to your system:
 The main Web Upd8 PPA maintained by: http: //叫w叫. webupd8.org/

To add this PPA, simply paste this in a terminal :
sudo add-apt-repository ppa:ni lar imogard/ webupd8

Packages in this PPA: audacious, ap-hotspot, awn-applet-radlo, awn-applet-wm, cau ise, cmus,
dockbarx, dockbarx- themes-extra, dropbox-share, emerald, exai le, tbmessenger, gnome-subti ties,
gnome-window-applets, 아sync, grive, gthumb, launchpad-getkeys, mc, mdm (Mint Display Manager) ,
minitunes, minitube, musique, notifyosdconfig, nauti lus-columns, powertop, ppa-purge, rosa-media
player, fixed pulseaudio-equal izer, subtitleeditor, syncwal l , umplayer, unity-reboot, wiml ib,
youtube-dl , xfce4-dockbarx-p山gin, xournal , yad and others. Almost al l packages are updated to their
latest version.

For other (special ized) PPAs we maintain, see: https: //launchpad.net/-webupd8team
 More into: https: //launchpad.net/-ni larimogard/+archive/ubuntu/webupd8
Press [ENTER] to continue or ctrl-c to cancel adding it

/／엔터를 누른후 아래 명령을 수행한다．

# apt-get update
# apt-get instal l android- tools-adb android-tools- f astboot

I/ fast boot가 설치된다．




다음으로 소스를 빌드할 때 사용하는 도구들을 설치한다．



쐬드佃邕ke) 도구 설치

# a口t-get instal l u七的卜too由

//mk image 프로그램이 설치된다．


# apt-get instal l texinfo

 //make info 프로그램이 설치된다．




아래와 같이 Device Tree Compiler 버전을 확인하여 1.4 이상이 아니라면 다음과 같이 DTC 소스를
다운받아 빌드하여 설치한다．


                                                   102 / 312
커널연구회（WW\A床ernei.L끄）                                                     정재준 了gbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                    4. Device Tree 실습   103




# dtc -v
The program 'dtc ' is currently not instal led.       You can instal l i t by typing:
apt-get instal l device- tree-compi ler

# apt-get instal l device- tree-compi ler

# dtc -v
Version: DTC 1.3. 0



# git clone gi t: //git. kernel . org/pub/ scm/uti ls/ dtc/ dtc.git

# cd dtc

# make
# cp dtc /usr/bin

/／설치후 버전을 확인한다．

# dtc -v
Version: DTC 1 . 4.1-gaa719618




4.2.3 크로스 컴파일러 설치
먼저 아래의 웹사이트0私］ u-boot 소스 빌드시 사용하는 크로스 컴파일러를 다운로드 한다．


http://www.arndaleboard.org/wiki/down幻ads/supports/arm-2009q3.tar


arm-none-linux-4.4工2009q3.tar.xz 파일이 다운로드 된다．


/／설치 경로 생성

# mkdir -p /opt/ toolchains

/／압축을 해제한다．

# xz -d arm-none- I inux-4. 4.1-2009q3. tar. xz
# tar xvf arm-none- I inux-4. 4.1-2009q3. tar -c /opt/ toolchains/

/／아래 경로에 압축이 해제되면서 설치된 다．

幻아 /to이 ch미 哨／
/opt/ tool cha i ns/ arm-2009q3/b in

/／루트 경로에 PATH를 등록한다．


                                                    103 I 312
커 널 연구회佃ww.kernei.bz)                                                           정재준 (rgbi3307（흐）nate.con가
Device Tree 상세분석 in Linux Kernel 4.0                                          4. Device Tree 실自1也4 1




# vi N /.bashrc
ex口ort PATH=$PATH:／야乂It的比ha ins/ar小加09q3/bin

/／일반 사용자 경로에 PATH를 등록한다 .（필자의 경우 jungjj)

# su jungj j

$ vi -/.bashrc
export PATH=$PATH: /opt/ toolchains/arm-2009q3/bin
$ source -/.bashrc

/／버전 4.4.1을 확인한다．

$ ar咐none니 i nux-gnueab i小gcc -尸version
arm-none- I inux-gnueabi-gcc (Sourcery G++ Lite 2009q3-67) 4. 4.1
Copyright (C) 2009 Free Software Foundation, Inc.
This is free software; see the source for copying conditions. There is NO
warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.




다음으로 커널 소스 빌드시 사용하는 크로스 컴파일러를 아래 웹사이트에서 다운로드 한다．



http://odroid.com/dokuwiki/doku.php?id =en:xu3_buildinq_kernel



arm七abi-4.6.tar.gz 파일이 다운로드 되는데， 이 크로스 컴파일러는 우분투 64비트에서 실행되므로

아래와 같이 이름을 변경한다｛구분을 위해서 단순히 rename 하는 것임）




$ my arm-eabi-4.6. tar. gz arm-eabi-4.6_x64. tar.gz

$ su root
#


아래와 같은 순서대厚 설치한다．


/／압축이 해제되면서 설치된다．

# tar xvfz arm-明이-4 . 旬x64. tar.gz -C 幻pt/ t的比ha ins!

/／루트 경로에 PATH를 등록한다．

# vi -/.bashrc
export PATH=$PATH: /opt/ toolchains/arm-eabi-4.6/bin

/／일반 사용자 경로에 PATH를 등록한다．（필자의 경우 Jun｛기 i)

# su jungj j

$ vi -/.bashrc
export PATH=$PATH: /opt/ toolchains/arm-eabi-4.6/bin

                                                104 / 312
커 널 연구회佃／w＼사.kern텨.t끄）                                                 정재준 了gbi3307@nate.com)
Device 가ee 상세분석 in Linux Kern이 4.0                                                   4. Device Tree 실습         105




$ source -/.bashrc

/／버전 4.6. x를 확인한다．

$ arrn-eabi-gcc -v
Using bui lt- 1 n specs.
COLLECT_GCC=arrn-eab i -gcc
COLLECT_LT0旴1APPER=／叩t/ to이ch미四／arrn-e的卜4.6/bin!. .11 山exec!gcc!ar rn- eab i /4.6 . 七goog陀／나0-
出rapper
Target: arm-eabi
Configured with: /trnp/ android-15472!src/bui Id!. ./gcc/gcc-4.6/ configure --prefix=/usr/ local --
target=arrn-eabi 小ho없＝x8旬餌니 i flux-gnu 叫bui ld=x8旬64니 inux-gnu --With-gnu-as 小with띠nu니d --
enable니anguages=c, c++ 小with띠nip=/trnp!an먀이小朽472／야j/ te叩니nstal I 小w나h-rn아尸/ trn口／android-
15472／야기／temp니nstal I 巾with-rn口c=/ trnp/ an먀아小拓472／야j!temp니nstal I 小with에卜叩1 小州 th에卜이的g
小di sab陀니 ibss口 --ena비e- threa卞 小disable-nls --disable니 ibmudf lap 小di sab陀니 ibgornp --disab陀
1 由stdcH싸3 --（키 sable-si I j-exce아 ions 小（ii sab I中帥ared 叫（키 sab 比나 Is 小（키 sab 陀니 比）its 小1叫 i th-
float=soft --with- fpu=vfp --wi th-arch=arrnv5te --enable- target-optspace ---with-abi=aapcs --with-gcc-
version=4.6 --with-binuti Is卞ver욕ion=2. 21 --with-grnp-version=4.2. 4 --with-rnpfr-version=2.4.1 --with-
gdb-version=7.3. x --with-arch=ar:rnv5te --with-sysroot=/tmp/ android-15472/ instal l/ sysroot --with-
pref ix=/trnp/android-15472/ instal l 小with띠에卜V아引에＝2.21 --enable-gold -中disable中gold 小（키sa바e-
mu It i 1 比） U1口rogra小trans化rrn-narne= 님針鈿rrn-e的卜＆1
Thread model : single
gcc version 4. 6. x-google 20120106 (prerelease) (0CC)



$ arrn-eabi-gcc --version
arm-eabi-gcc (0CC) 4.6. x-google 20120106 (prerelease)
Copyright (C) 2011 Free Software Foundation, Inc.
This is free software; see the source for copying conditions. There is NO
warranty; not even for MERCHANT肥ILITY or FITNESS FOR A PARTICULAR PURPOSE.




4.3 소스 빌드 및 포팅

이제 개발환경을 구축했으므로 u-boot, kernel, ram비敬을 빌드하도록 하자．




4.3.1 u-boot 소스 빌드
Arndale Octa Board을 위한 각종 소스들은 아래 웹사이트를 참조하여 다운로드 가능하지만，


http://www.arndaleboard.orq/wiki/index.php/OWiKi


$ repo mnit-u git: //git. insignal .co.kr/ insignal/arndale_octa- jb_rnrl. 1/android/rnanifesf -b jb-mrl . 1


$ repo sync

                                                 105 / 312
커 널 연구회（www.kerne比z)                                                         정재준 (rgbi3307@nate.com)
Device 가ee 상세분석 in Linux Kernel 4.0                                              4. Device Tree 실습    106




/／소스를 모두 다운로드 하는데 3시간정도 소요됨 .




소스를 다운로드 하는데 오래걸리고 소스를 구성하는 절차가 복잡하므로, 필자가 미리 작업해둔

u-boot 소스를 아래떽 커널연구회 웹사이트에서 다운로드 한다．


http: //dev.kernel .bzldownloadlexynos542olu-boot_2012. 07 exynos5420marnda1e. tar.gz




/／소스파일을 다운로드한 경로로 이동



/／압축해제

$ tar xvzf u-boot_2012.07_exynos5420_arndale. tar .gz

$ Cd U나)OOt

$ II
total 604
drwxrwxr-x 22 jungj j    jungjj   4096 Feb 11 14:32 .1
drwxr-xr-x   9 jungjj    jungjj   4096 Mar 28 15:10 . .1
drwxrwxr-x   2 jungjj    jungjj   4096 Feb 11 14:31 api/
drwxrwxr-x 16 jungjj     jungjj   4096 Feb 11 02:53 arch!
 rw-r--r--   1 jungjj    jungjj 15360 Dec 13 2013 arndale_octa.bll. bin
 rw-r--r--   1 jungjj    jungjj 14592 Dec 13 2013 arndale_octa.b12.bin
-rw-r--r--   1 jungjj    jungjj 262144 Dec 13 2013 arndale_octa. tzsw.bin
drwxrwxr-x 283 iungjj    jungjj 12288 Feb 11 02:53 board!
-rw-rw-r--   1 jungjj    junqjj 112647 Feb 11 02:53 boards. cfg
 rw-rw-r--- 1 jungjj     jungji 43071 Feb 11 14:32 .boards.depend
drwxrwxr-x   2 jungjj    jungjj   4096 Feb 11 14:31 common!
-rw-rw-r--   1 junqjj    jungjj 10465 Feb 11 02:53 config.mk
-rw-rw-r--   1 jungjj    jungjj 16398 Feb 11 02:53 COPYING
-rw-rw-r--   1 jungjj    jungjj 18674 Feb 11 02:53 COPYING. txt
-rw-rw-r--   1 jungjj    jungjj 12102 Feb 11 02:53 CREDITS
drwxrwxr-x   2 jungjj    jungjj   4096 Feb 11 14:31 disk!
drwxrwxr-x   5 jungjj    jungjj 12288 Feb 11 02:53 dod/
drwxrwxr-x 26 jungjj     jungjj   4096 Feb 11 02:53 drivers!
drwxrwxr-x   2 jungjj    jungjj   4096 Feb 11 02:53 dtsl
drwxrwxr-x   4 jungjj    jungjj   4096 Feb 11 02:53 examples!
drwxrwxr-x 10 jungjj     jungjj   4096 Feb 11 02:53 ts!
먀wxr州xr기（ 2 jungjj       jungjj   4096 Feb 11 14：化 .이t/
-rw-rw-r--   1 jungjj    jungjj    836 Feb 11 02:53 .git ignore
drwxrwxr-x 17 jungjj     jungjj 12288 Feb 11 14:31 include!
drwxrwxr-x   7 jijngjj   jungjj   4096 Feb 11 14:31 l ib!
-rw-rw-r--   1 jungjj    jungjj 24302 Feb 11 02:53 MAINTAINERS
-rwxrwxr-x   1 jungjj    jungjj 20815 Feb 11 02:53 MAKEALL*
-rw-rw-r--   1 jungjj    jungjj 27541 Feb 11 02:53 Makefi le
  rwxrwxr-x  1 jungjj    jungjj   4249 Feb 11 02:53 mkconfig*
drwxrwxr-x   3 jungjj    jungjj   4096 Feb 11 02:53 nand_spl!
dr나xr나町出 2 jungjj        jungjj   4096 Feb ]] 14:31 net!

                                                106 I 312
커 널 연구회（www.kerr倒.b기                                                        정재준 (rgbi3307@nate.com)
Device Tree 상세분석 ir) 니flux Kernel 4.0                                             4. Device Tree 실습   ]07




dr벡xr나xr )(    3 jungjj     jungjj   4096 Feb 11 02:53 onenand_ ipl!
drwxrwxr-x     6 jungjj     jungjj   4096 Feb 11 14:31 post!
 rv中rw나小       ] J ungj J   jungjj 177186 Feb 11 02: 53 README
中r나-rw나十       ] ] ungj J   jungjj   2487 Feb 11 02:53 rules. mk
dr나xr나xr )(    6 jungjj     Jungj J  4096 Feb 11 02:53 sd_ fuse!
 Iv中rW나十       ] jungjj     Jungj J    17 Feb 11 02:53 snapshot. commit
drwxrwxr-x     2 jungjj     Jung] I  4096 Feb 11 02: 53 spl!
drwxr벡XI出     ]2 jungjj     jungj J  4096 Feb 11 14: 31 tools!




이제 다음과 같이 부트로더를 환경설정한 후 빌드한다．



/／환경 설정하21

$ make ARCH=arm CR0SS_C0MPlLE=arm-none니 inux-gnueabi- clobber
$ make ARCH=arm CR0SS_C0MP比E=arm-none- l i nux-gnueab i- arndale_octa_conf ig
Conf iguring for arndale_octa board. . .

// 빌 드하기

$ make ARCH=arm CR0SS_C0MPlLE=arm-none- l inux-gnueabi

/／빌드 실행됨（수분정도 소요됨 )



/／빌드한 실행 파일 확인

$ I I u나）oot大
 rwxrwxr-x 1 jungjj jungjj 1045332 Mar 28 15:17 u-boot*
-r忙rw나- 1 jurvgjj jungjj 259152 Mar 28 15:17 u-boot.bin
 rv中IW나小 ] jungjj jungjj       923 Mar 2815: 17 u-boot. lds
나Iv中1W나十 ] jungj j jungjj    97015 Mar 28 15:17 u-boot. map
 rv中rw나十 ] jungjj jungjj 777552 Mar 28 15:17 u-boot. srec




이제 최종적으로 작성한 이미天 파일을 uboot에 올려보도록 하자． 부트로더에 올리는 파일이 아

래와 같이 4개가 존재하는지 먼저 확인한다．


$ I I 士 .bin
 r나나小r十 ]        jungjj   jungjj 15360 Dec 13 2013 arndale_octa.b너 .bin
  rw-r--r- - 1   jungjj   jungjj 14592 Dec 13 2013 arndale_octa.b12.bin
-rw-r--r- - 1    jungjj   jungjj 262144 Dec 13 2013 arndale_octa. tzsw.bin
 r낵-1W寸十 ]       jungjj   jungjj 259152 Mar 28 15:17 u나）oot 力in




먼저 타겟보드의 uboot와 USB OTG 통신하는 fastboot 유틸리티 프로그램이 리눅스（우분투） 호스

트 PC에 설치되어 있는지 확인하여 설치되어 있지 않다면 다음과 같이 설치하도록 한다．


!!root 계정으로 실행한다．


                                                    107 / 312
커 널 연구회 (www.kernel.b기                                                       정재준 (rg니3307@nate.com)
Device Tree 상세분석 ir) 니flux Kernel 4.0                                             4. Device Tree 실습   ]08




# add-apt-reposi tory ppa:ni tar imogard/webupd8
# a아띠et update

# apt-get instal l an먀이小tools나as比cot

# fastboot help
usage: fas比cot [ <0아 山n> I <command>

commands:
  update <fi lename>                         reflash device from update.zip
  f I asha I I                               flash boot + recovery + system
  flash <partition> [ <fi lename> I          write a fi le to a flash partition
  erase <partition>                          erase a flash partition
  format <partition>                         format a flash partition
  getvar <variable>                          display a boot loader variable
  boot <kernel> [ <ranidisk> I               download and boot kernel
  flash: raw boot <kernel> [ <ramdisk> ]     create boot image and flash it
  devices                                    l ist al l connected devices
  continue                                   continue with autoboot
  reboot                                     reboot device normal ly
  reboot나兀of loader                          reboot device into boot loader
  he 巾                                       sho出 th治 he巾 message

opt ions:
   w                                         erase userdata and cache (and format
                                             if supported by partition type)
  -u                                         don아 f 나St erase 口artition before
                                             化rmatting
   s <specif ic device>                      specify device serial number
                                             or path to device port
  -l                                         with 'devices", l ists device paths
  -p <product>                               specify product name
  -c <cmdl ine>                              override kernel commandl ine
  -i <vendor id>                             specify a custom USB vendor id
  -b <base_addr>                             specify a custom kernel base address
  -n <page size>                             specify the nand page size. default: 2048
  -S <size>[KIMIGI                           automatical ly sparse fi les greater than
                                             引ze. 0 to （키sab陀




리눅스（우분투） 호스트 PC와 타켓보드는 다음과 같이 연결되어 있어야 한다．




                                                   108 / 312
커널연구회（www.kernel.b기                                                       정쟤준 (rgbi3307（亘）nate.cor가
Device Tree 상세분석 in Linux Kernel 4.0                                    4. Device Tree 실습   109




    Tennin出 (Linux Ubuntu)
                                    USS otg C身b陌




                                     Seni計Cab地
                                                      Embcddcd
                                                     Linux 1'缸孚(




                                               nat 丁ermn쿠1



리눅스 Host PC（우분투）에서 시리얼（/dev/ttySo) 터미널 프로그램인 minicom을 실행하여 타겟 보
드에 접속하여 부트로더（uboot) 명령 프롬프트에 진입한다．


시리얼 터미널 프로그램을 이미 사용하고 있는 독자분들은 그것을 그대로 사용하면 되지만, 처음
으로 사용하시는 독자분들은 아래와 같이 우분투 호스트 PC에 minicom이 설치되어 있는지 확인
하여 설치되어 있지 않다면 아래와 같이 설치한댜．



'V出Mmm 件쳐卦인
$ minicom -v
mini에 version 2.5 (compi led May 2 2011)
Copyr ight (C) Miquel van Snioorenburg.

This program is tree software; you can redistr ibute it and/ or
modify it under the terms ot the GNU General Publ ic License
as publ ished by the Free Sottware Foundat ion; either version
2 ot the License, or (at your opt ion) any later version.




'V出甘m享t 任치
사루트 계정으로 설치후 실행한다．

# apt-get instal l minicom

/／실 행
# mi n I com

Ctrl+A 0 /／환경설정


                                               109 I 312
커 널 연구회（www.kernel.bz)                                             정쟤준 (r야이3307@nate.com)
Device Tree 상세분석 ir) 나flux Kerr佃 4.0                                            4. Device Tree 실습




minicom을 처음으로 사용하는 독자분은 인터넷에서 관련정보를 검색하면 사용법에 대해서 많이
나오므로 참조하기 바란다．



이제, 아래와 같이 타겟보드의 uboot로 진입하여 명령 프롬프트에서 fastboot올 실행하여 USB

OTG Ca비e이 정상적으로 연결되었는지 확인한다．



타겟보드 uboot에서 fastb＜沁t 싶형
U-Boot 2012. 07-g8c348a3 (Mar 11 2015 - 15: 31: 43) for ARNDALE OCTA

CPU: Exynos5420 Rev2. O [Samsung SOC on SMP Platform Base on ARM CortexA15I
APLL = 800MHz, KPLL = 600MHz
MPLL = 532MHz, BPLL = 800MHz

Board: ARNDALE OCTA
DRAM: 2 GiB
WARNING: Caches not enabled

TrustZone Enabled BSP
BL1 version:

Checking Boot Mode . . . SDMMC
MMC:   S5P_MSHC2: 0, S5P_MSI-ICO: 1
冊C Device 0: 7. 5 (｝沼
MMC Device 1: 7. 3 GiB
MMC Device 2: MMC Device 2 not found
there are 口en（키ng interrupts Ox00000001
In:    serial
Out:   serial
Err:   serial
Net:   No ethernet found.
Hit any key to stop aut아）oUt: 0     - 여기서 스페이스바를 엔터하면 부트로더로 진입한다．

/／부트로더 명령 프롬프트에서 환결설정 값을 확인한다．

ARNDALE # print
baudrate=115200
bootargs=console=ttySAC3,115200n8 root=/dev/ root init=/sbin/ init ini trd=0x21000000, 32M ramdisk=32768
bootcrnd=run bootcmd_normal ; run bootcmd_extend
bootcmd extend=mmc read 1 20008000 7800 8; source 20008000
bootcmd extend sd=oimc read 0 20008000 7800 8; source 20008000
bootcmd nornial=rnovi read kernel 0 20008000;movi read rootfs 0 21000000 100000;bootz 20008000
21000000
bootde I ay=1
r00tfs1en=0x9c1d6
stderr=ser ial
stdin=ser i al
St（幻叭＝serial

Environment size: 377/16380 bytes



                                                110/ 312
커 널 연구회（www.kernel.b기                                                    정재준 (rg너3307@riate.com)
Device Tree 상세분석 in Linux Kern이 4.0                                                4. Device Tree 실습   ]11




I/ f as比oot을 실행한다．

AR卜［)ALE # f as比oot
[Partition table on MoviNAND]
ptn 0 name= fwb너 start=0x3 len=N/ A (use hard-coded info. (cad: niovi ) )
ptn 1 name= 'b12 start=N/ A len=N/ A (use hard-coded info. (crnd: movi ) )
ptn 2 name= boot loader start=N/ A len=N!A (use hard-coded info. (cmd: movi ) )
ptn 3 name= tzsw star t=N/ A Ien=N/ A (use hard-coded info. (cad: rnovi) )
ptn 4 narne= 'kernel start=N/ A len=N/ A (use hard-coded info. (cad: movi ) )
ptn 5 name= ramdisk ' start=N/ A len=oxo(-27262976}KB) (use hard-coded info. (cmd: rnovi) )
ptn 6 nanie= system start=0x3 len=oxo(-548352000KB)
ptn 7 name= userdata' start=0x3 len=0xO(-548352000K8)
ptn 8 name= cache start=0x3 len=OxO(-548352000KB)
ptn 9 narne= 'fat start=0x3 len=0x0(-1924911104KB)
1138 cable Connectedl[CH-0]




위와같이 OTG cable Connected! 메시지가 나오면 정상적으로 연결된 것이다.                                      타겟보드의 uboot
에서 fastboot가 실행되어 있는 상태에서 우분투 호스트 PC에서 다음과 같이 fastboot을 실행하여
앞에서 만들어둔 부트로더 이미지들을 타겟보드에 전송한다．



早붚平 Hc寸t 代m사如出孝比仕甘
//fas比oot는 루트 계정으로 실행한다．

$ I I 女．bin
 r나나小r小 ] jungjj       jungjj 15360 Dec 13 2013 arndaleocta.b너 .bin
 r나나小r小 ] jungjj       jungjj 14592 Dec 13 2013 arndaleocta．이2力In
 rw-r--r-- 1 jungj j   jungjj 262144 Dec 13 2013 arndale_octa. tzsw.bin
 r놔나베나小 ] jungjj       jungjj 259152 Mar 28 15:17 u七oct .bin

$ su root
Password:

# fastboot fla寸1 fwb너 arndale_octa.bll. bin
sending ' fwb녀 (15 KB) . . .
OKAY [ 0. 005s]
나rit ing ' fwb 너 . . .
OKAY [ 0. 042s1
f inished, total time: O. 047s

# fastboot flash b12 arndale octa.b12.bin
sending b12 (14 KB) . . .
OKAY [ 0. 005引
wr iting 'b12 ' . . .
OKAY [ 0. 023引
f inished, total t ime: O. 028s

# f as比oot fla針） b어）tloader u寸刃ot.bin
sending 'bootloader (253 KB) . . .
OKAY [ 0. 037s]
writing ' bootloader ' . . .
OKAY [ 0. 063s]

                                                111 I 312
커 널 연구회佃ww太ernel.1끄）                                                       정재준 (rgbi3307@nate.com)
Device Tree 상세분석 ir) 니flux Kernel 4.0                                           4. Device Tree 실습     112




f inished, total time: O. lOls

# tastboot flash tzsw arndale octa. tzsw.bin
sending tzsw (256 KB) . . .
OKAY [ 0. 037s]
卄rit ing ' tzs텍 ．
OKAY [ O. 053s}
f inished, total time: 0. 090s

사타겟보드를 리부팅한다．

# fastboot reboot
rebooting. . .

f inished, total time: O. 000s




타겟보드（Arndale Octa Board）가 리부팅되면서 시리얼 터미널에 아래와 같이 타겟보드의 부트로더

가 부팅되는 메시지（로그）를 확인할 수 있다．




U-Boot 2012. 07-g8c348a3 (Mar 11 2015 - 15:31: 43) for ARNDALE OCTA

CPU: Exynos5420 Rev2. O [Samsung SOC on SMP Platform Base on ARM CortexA15]
APLL = 800MHz, KPLL = 600MHz
MPLL = 532MHz, BPLL = 800MHz

Board: ARNDALE OCTA
DRAM: 2 （引B
WARNING: Caches not enabled

TrustZone Enabled BSP
BL1 version:

Checking Boot Mode . . . SDMMC
MMC:    S5P_MSHC2: 0, S5P_MSHCO: 1
MMC Device 0: 7. 5 GiB
MMC Device 1: 7. 3 GiB
MMC Device 2: MMC Device 2 not found
there are pending interrupts Ox00000001
In :    S（玎 ial
Out:    serial
Err:    serial
Net:    No ethernet found.
Hit any key to stop autoboot : 0
reading kernel . .device 0 Start 1263, Count 10240
MMC read: dev # 0, block 4 1263, count 10240 . . . 10240 blocks read: OK
co叫키 eted
reading RFS. . device 0 Start 11503, Count 2048
MMC read: dev # 0, block 4 11503, count 2048 . . . 2048 blocks read: OK
comr니 eted




                                               112 / 312
커 널 연구회（www.kern이. b까                                                      정재준 (rgbi3307@ nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                             4. Device Tree 실습   113




이제 리눅스 커 널 소스를 빌드하도록 하자．



4.3.2 마이크로 SD카드 부팅
필자가 타겟보드로 선택하여 실습하고 있는 Arndale Octa Board는 부팅장치로 eMMC와 마이크로
SD카드를 선택하여 부팅할 수 있다.                       다음과 같이 보드에 있는 D下 스위치의 4번핀을 On하면
eMMC로 부팅한다． 보드를 구매하면 기본적으로 eMMC로 u-boot가 부팅된다．




아래와 같이 ［기P 스위치 3번핀을 (Jn하면 마이크로 SD카드로 부팅한다．




마이크로 SD을 신규로 구입했다면. 부팅가능하도록 파티션들을 다음과 같이 만드는 작업이 필요
하다.     먼저 앞에서 작업한 u-boot 소스경로에서 sd fuse 경로로 진입하여 그곳에 있는 파일들을
확인한다．



$ Cd sd_ fuse
$  1'
total 636
drwxrwxr-x 6 jungjj     jungjj   4096 Mar 29 17: 34 .1
drwxrwxr-x 22 jungjj    jungjj   4096 Mar 29 17: 23 . .1
-rw나小r小 ] jungjj        jungj j 15360 Mar 28 20: 23 arnda陀山cta力너 .bin
-rw나小r小 ] jungj J       川ngjj 14592 Mar 28 20: 23 arnda陀 octa．이2上In
-rw-r--r- - 1 jungj j   jungjj 262144 Mar 2820: 23 arndale_octa. tzsw.bin
-rw-rw-r-- 1 jungjj     jungj j  1607 Feb 11 02: 53 exynos-mkbl2. c
  rw-rw-r-- 1 jungjj    junqjj    839 Feb11 02: 53 Makef i le
  rwxrwxr-x 1 jungjj    jungjj   8896 Mar 29 17: 21 mkb12*
  rwxrwxr-x 1 jungjj    jungj j 13131 Mar 29 17: 21 sd_ fdisk*
  rw-rw-r-- 1 jungjj    jungj j  7356 Feb 11 02: 53 sdfdisk. c
  rwxr-xr-x 1 jungjj    jungj j  1258 Mar 29 17:29 sd_ f using_5420. sh*
  rwxr-xr-x 1 jungjj    jungj j  2452 Feb 11 02: 53 sd_ fusing. sh*
drwxrwxr-x 2 jungjj     jungj j  4096 Feb 11 02: 53 srndk4x12/

                                                113 / 312
커 널 연구회佃w比kern이b기                                                           정재준 （띠bi3307@nate.com)
Device Tree 상세분석 in 니nux Kerr側 4.0                                                 4. Device Tree 실습         114




drwxrwxr-x   2 jungjj    jungjj   4096 Feb 11 02: 53 smdk5250/
drwxrwxr-x   2 jungj j   jungjj   4096 Feb 11 02:53 smdk5410/
drwxrwxr-x   2 jungj j   jungj j  4096 Feb 11 02: 53 snidk5420/
 rw-rw-r--   1 jungjj    jungjj 259152 Mar 28 20: 23 u-boot.bin




위의 파일들이 있는지 확인한 다음, 마이크로 SD카드를 우분투 호스트 PC에 장착하면 다음과 같

이 마운트 된다.           mount 명령으로 다음과 같이 마운트된 장치명을 확인한다．




$ mount
/dev/ sdal on / type ext4 (rw,errors=remount-ro)
proc on /proc type proc (rw,noexec,nosuid,nodev)
sysfs on /sys type sysfs (rw, noexec,nosuid,nodev)
none on /sys/ fs/ fuse/ connect ions type fusectl (rw)
none on /sys/kernel/debug type debugfs (rw)
none on /sys/kernel/ security type securi tyfs (rw)
udev on /dev type devtrnpfs (rw,mode=0755)
devpts on /dev/pts type devpts (rw,noexec,nosuid,gid=5,mode=0620)
tmpfs on /run type tmpfs (rw,noexec,nosuid, size=10%,niode=0755)
none on /run/ lock type trnpfs (rw, noexec,nosuid, nodev, size=5242880)
none on /run/ shrn type tinpfs (rw,nosuid,nodev)
gvfs- fuse-daemon on /home/ jungj j/ .gvfs type fuse. gvfs- fuse-daemon (rw,nosuid,nodev,user= jungj j)
/dev/sdbl on /media/F27F-1469 type vfat
 (rw,nosuid, nodev, uid=1000,gid=1000, shortname=mixed,dmask=0077,utf8=1, showexec, f lush,uhelper=udisks)

/／口F이크로 SD가 /devi sdb에 마운트 되어 있다．
/／독자분들의 PC에 장착되어 있는 디스크 개수에 따라서 /dev/ sdc 혹은 /dev/ sdd 등에 마운트될 수도
/／있으므로 위와 같이 mount 명령으로 확인한다．

I/ sd_ f（키sk을 실행하여 부팅가능한 파티션을 생성한다．

$ ./sd_fdisk /dev/ sdb




부팅가능한 파티션을 생성 했으므로, 이제 이 파티션에 부팅에 관련되는 실행 이미지들을 fusing

한다． Fusing은 루트 계정으로 실행한다．



$ su root
Password:

# ./sd_ fusing_5420. sh /dev/ sdb

/devlsdb reader is ident ified.
BL1 fusing
30+0 records in
30+0 records out
15360 bytes (15 k8) copied, 0.125485 s, 122 kB/ s
BL2 fusing
28+1 records in

                                                  114 / 312
커 널 연구회（www.kerr）飢b기                                                       정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                             4. Device Tree 실습




28+1 records out
14592 bytes (15 kB) copied, 0.174694 s, 83. 5 kB/ s
U吐珣of fusing
506+1 records in
506+1 records out
259152 bytes (259 kB) copied, 1.44148 s, 180 kB/ s
TrustZone S/W fusing
512+0 records in
512+0 records out
262144 bytes (262 kB) copied, 1.38831 s, 189 kB/ s
U-boot image is fused successful ly.
Eject SD card and insert it again.




위와 같이 진행하면 마이크로 SD가 부팅 가능한 상태가 되었으므로 타겟보드에 마이크로 SD을

장착한후 부팅하면 아래와 같o u七oot가 부팅된다．


U-Boot 2012. 07 (Mar 28 2015 - 15:15: 44) for ARNDALE OCTA

CPU: Exynos5420 Rev2. 0 [Samsung SOC on SMP Platform Base on ARM CortexA15]
APLL = 800MHz, KPLL = 600MHz
MPLL = 532MHz, BPLL = 800MHz

Board: ARNDALE OCTA
DRAM: 2 （키B
卄ARN 나40: Caches not enat니 ed

TrustZone Enabled BSP
BL1 v（玎引on:

Checking Boot Mode . . . SDMMC
MMC:   S5P_MSHC2: 0, S5P_MSHCO: 1
MMC Device 0: 3. 7 GiB
MMC Device 1: 7. 3 GiB
MMC Device 2: MMC Device 2 not found
there are pending interrupts 0x00000001
士女女Warning - bad CRC, using default environment

1n :    ser ial
Out:    serial
Err:    ser ial
Net:    No ethernet found.
Hi t any key to stop autoboot: 0
reading kernel . .device 0 Start 1263, Count 10240
MMC read: dev # 0, block ft 1263, count 10240 . . . 10240 blocks read: OK
Co叫니eted
reading RFS. . device 0 Start 11503, Count 2048
MMC read: dev ft 0, block ft 11503, count 2048 . . . 2048 blocks read: OK
Co叫) leted
Bad Linux ARM zlmage magic!

MMC read: dev ft 1, block # 30720, count 8 . . . 8 blocks read: OK
ft# Executing script at 20008000
Wrong image format for 'source ' command

                                               115 / 312
커 널 연구회 (www.kerrie나끄）                                                      정쟤준 （呼)13307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                             4. Device Tree 실습




ARNOALE # mmc l ist
S5P MSHC2: 0
 S5P MSI-ICO: 1

ARNDALE # fdisk
Usage:
f（키sk 千p> <device_flue>
fdisk <-c> <device_num> [<sys. part size(甛)> <user data part size> <cache part size>I
ARNOALE # fdisk -p 0

partion #     size(情｝)    block start #      block count   partition_Id
   1           3803            8192           7788544        0xOB
ARNDALE # fastboot
Error : 卜幻 MBR is 化und at SD/MMC.
Hint: use fdisk command to make parti tions.



/／씨叩이 없다는 오류가 나타나면 아래와 같이 MBR올 생성하는 명령을 실행한다．

ARNDALE # fdisk -c 0
fdisk is completed

partion #    size(MB)      block start #    block count    partition_Id
   J
   1
              2768           1988820         5669280         0xOC
   n<
               301            137160          617220         0x83
    QU
               301            754380          617220         0x83
    4
    1
               301           1371600          617220         0x83
ARNDALE # fdisk -p 0

partion #     size(MB)     block start #    block count    partition_Id
    J
    1
               2768          1988820         5669280         0xOC
    n
    亡
                301           137160          617220         0x83
    Q
    U
                301           754380          617220         0x83
    d
    1
                301          1371600          617220         0x83

ARNOALE # fastboot
[Parti tion table on MoviNANDI
ptn 0 name=냐wb너 ' start=0x3 len=N/A (use hard-coded info. (cmd: movi) )
ptn 1 name= b12 ' start=N/ A len=N/ A (use hard-coded info. (cmd: movi) )
ptn 2 name= 'bootloader ' start=N/A len=N/ A (use hard-coded into. (cmd: movi) )
ptn 3 name=나zsw ' start=N/ A Ien=N/A (use hard-coded info. (cmd: movi) )
ptn 4 name= 'kernel ' start=N/ A len=N/ A (use hard-coded info. (cmd: movi) )
ptn 5 name= ramdisk ' start=N/ A len=0x0(-27262976KB) (use hard-coded info. (cmd: movi) )
ptn 6 name= 'system start=0x3 len=oxo(-316016640KB)
ptn 7 name= 'userdata start=0x3 len=0x0(N316016640KB)
ptn 8 name= 'cache ' start=0x3 len=0x0(-316016640K8)
ptn 9 name= fat ' start=0x3 len=oxo(--1392295936KB)
USB cable Connected! [CH-0I




위와 같은 순서대로 u-boot로 진입하여 fastboot 명령까지 실행하면 마이크로 SD에 리눅스 커 널
과 램디스크를 포팅할 준비가 된 것이다．



                                               116 / 312
커 널 연구회（ww比kern飢b기                                                        정재준 內bi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                                     4. Device Tree 실습     117




4.3.3 리눅스 커널 소스 빌드
먼저 리눅스 커 널 소스 보관소 웹사이트에서 최신의 리눅스 커널 소스를 다운로드 한다.                                                      필자가

이글을 작성하는 시점에서 가장 최근에 안정화된 리눅스 커널 소스는 4.0 버전이다．




/／일 반 사용자 계정 으로 실행한다．

$ su jungjj

$ pwd
/home/ jungj i/ projects/Kernel

/／커 널 소스 다운로드

$ wget https: //놔w나. kernel . org/pub/ I inux/kernel/ v4. x/ l inux-4. 0. tar. xz

／后따분 정도 소요됨 .




다운로드한 소스 파일（ i flux콕. 0. t카．xz）을 아래와 같은 방법으로 압축을 해제한다．




$ 11
total 80392
di베xi볘xi )( 2 jungjj jungjj   4096 Apr 18 16: 47 ./
（打베xr벡xi水 7 jungjj jungjj     4096 Api 4 09: 38 . . /
 r벡iw나十 ] j ungj J jungjj 82313052 Api 1307: 42 I inux-4.0. tar . xz

//xz 압축 해제

$ xz -d l inux-4.0. tar. xz

$ 11
total 576192
drwxiwxi-x 2 jungjj jungjj    4096 Apr 18 16: 54 ./
（打바xi벡xi小）( 7 jun（기 I lUfl9lJ 4096 Api 4 09: 38 . . /
1n中iw나十 ] jungjj jungjj 590008320 Api 1307: 42 l inux-4. 0. tai

//tar 압축 해저1

# tar xvf I inux-4. 0. tar

사압축 해제 완료

$ 11
total 576196
diwxrwxr-x 3 jungjj      jungjj      4096 Api 18 16:55 ./
drwxiwxr-x 7 jungjj      jungjj      4096 Api 4 09: 38 . . /
drwxiwxi-x 23 jungjj     jungjj      4096 Apr 1307:12 l inux-4.0!
 rw-rw-r-- 1 jungjj      jungjj 590008320 Api 1307: 42 l inux-4.0. tai


                                                      117 /312
커 널 연구회（www.kern이. t끄）                                                              정재준 仕gbi3307（亘）nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                          4. Device Tree 실습   118




$ cd I inux-4.O/
$ II
total 628
drwxrwxr-x 23 jungjj jungji     4096 Apr 13 07:12 .1
drwxrwxr-x    3 jungjj jungjj   4096 Apr 18 16:55 . .1
（打wxrw町水 32 jungjj jungjj       4096 Apr 13 07:12 카ch/
dr叫xi벼자水      3 jungjj jungjj   4096 Apr 13 07:俚 block!
-rw-rw-r--    1 Jungjj jungjj 18693 Apr 13 07:12 COPYING
寸中1W나小        ] jungjj jungjj 96226 A口r 13 07:12 CREDITS
drwxrwxr-x    4 jungjj jungjj   4096 Apr 13 07:12 crypto/
drwxrwxr-x 108 jungjj jungjj 12288 Apr 13 07:12 Documentation!
drwxrwxr-x 122 jungjj jungjj    4096 Apr 13 07:12 drivers!
drwxrwxr-x 36 jungj j jungjj    4096 Apr 13 07:12 firmware!
drwxrwxr-x 75 jungjj iungii     4096 Apr 13 07:12 fs!
-rw-rw-r--    1 jungjj jungjj   1220 Apr 13 07:12 .git ignore
drwxrwxr-x 28 iungjj jungjj     4096 Apr 13 07:12 include!
drwxrwxr-x    2 jungjj jungjj   4096 Apr 13 07:12 m it!
drwxrwxr-x    2 jungjj jungjj   4096 Apr 13 07:12 ipc/
-rw-rw--r--   1 jungjj jungji   2169 Apr 1307:12 Kbui ld
  1w-lw-i- -  1 jungjj iungjj    252 Apr 13 07:12 Kconfig
drwxrwxr-x 16 jungjj jungjj     4096 Apr 13 07:12 kernel!
drwxrwxr-x 11 jungjj jungjj 12288 Apr 1307:12 l ib!
-rw-rw-r--    1 jungjj jungjj   4968 Apr 1307:12 .mai lmap
-r州-r나나1e     ] jungjj jungjj 305968 A口r 13 07:12 枾시NTAINERS
-rw-rw-r--    1 jungjj jungjj 54559 Apr 1307:12 Makefi le
di나xr나xr水     3 jungjj jungjj   4096 A口r 13 07:12 mm!
dr나xr나町水 59 jungjj jungjj       4096 Apr 13 07:12 net!
-rw-rw-r--    1 jungjj jungjj 18736 Apr 13 07:12 README
卞rw-rw-r--    1 jungjj jungjj   7485 Apr 13 07:12 REPORTING-BUGS
drwxrwxr-x 14 jungjj jungjj     4096 Apr 13 07:12 samples!
drwxrwxr水 14 jungjj jungjj      4096 Apr 13 07:12 scripts!
drwxrwxr-x    9 jungji jungjj   4096 Apr 13 07:12 security!
drwxrwxr-x 22 jungjj jungjj     4096 Apr 13 07:12 sound!
먀Wxr나자-x 19 jungjj jungjj       4096 Apr 13 07: 俚 加이sl
drwxrwxr-x    2 jungjj jungjj   4096 Apr 13 07:12 usr!
drwxrwxr-x    3 jungjj jungjj   4096 Apr 13 07:12 virt/




리눅스 커널 소스를 빌드하기 전에 아래와 같이 크로스 컴파일러 버전（arm-eat升gcc 4.6．자을 확인

한다.     훅시 아래의 버전 정보가 나타나지 않으면 앞의 크로스 컴파일러 설치 과정을 다시 확인하

여 설치하도록 한다．


$ arm-eabi-gcc --version
arm-eabi-gcc (6CC) 4.6. x-google 20120106 (prerelease)
Copyright (C) 2011 Free Software Foundation, Inc.
This is free software; see the source for copying conditions. There is NO
warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.




크로스 컴파일러 버전을 확인했다면 아래와 같이 커널 환경설정 파일（.config）을 생성한다．


                                              118 / 312
커 널 연구회（ww比kernel.b기                                                   정재준 的bi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                 4. Device Tree 실습   119




$ make ARCH=arm CROSS_COMPILE=ai 咐eabi- exynos_defconf ig
  HOSTCC scripts/ basic/ f ixdep
  HOSTCC scr ipts/kconf ig/ conf.(
  SHIPPED scr ipts/kconf ig/ zconf tab. c
  SHIPPED scr ipts/ kconf ig/ zconf I ex . c
  SHIPPED scr ipts/ kconf ig/ zconf hash. c
  HOSTCC scr ipts/kconf ig/ zconf tab.o
  HOSTLD scr ipts/kconf ig/ conf
#
# conf iguration written to . con
#


위에서 생성한 환경설정 파일（.config）은 커널 소스의 arch/arm/configs/exynos_defcorifig 파일을
참조하여 생성한 것으로서 그 내용을 확인하1 보면 아래와 같다．


$ vi .conf ig

#
# Automatical ly generated fi le; )O NOT ED나．
# Linux/ arm 4. 0. 0 Kernel Conf igu rat 山n
#
CONE떠 ARM=y
CONE I G_ARM_HAS_SG_CHA I N=y
CONE떠_NEED_SG_DMALENGTH=y
CONE 田小剛DMA기SE그 OMMU=y
CONEIG ARM DMA IOMMU ALIGNMENT=8
CONE 田씨애T_HAVE_PC I =y
CONEIG SYS SUPPORTS APM EMULATIO
CONE I G_HAVE_PROC_CPU=y
CONF I G_NO_ I OPORT_MAP=y
CONE떠_STACKTRACE_SUPP0RT=y
CONE I G_LOCKDEP_SUPPORT=y
CONE 10_TRACE_I RQFLAGS_SUPPORT=y
CONE I G_RWSEM_XCHGADD_ALGOR I THM=y
CONE I G_ARCH_HAS_BANDGAP=y
CON디G匪NER比 H叫EIGHT=y
CONE IG_匪NER IC_CAL IBRATE_DELAY=y
CONE I G_NEED_DMA_MAP_STATE=y
CONE I G_ARCH_SUPPORTS_UPROBES=y
CONEIG VECTORS BASE=Oxffff0000
CONE I GARMJATCH_PHYS_V I RT=y
CONEI(; 匪NER比 BU（뉴y
CONE떠 DEECONEIG LIST='/ I 山加odu Ies/$UNAME_RELEASE/ .conf ig'
CONE 田그 叩川애小y
CONE I G_BU I LDT I ME_EXTABLE_SORT=y

/／이하 생략．. .




위의 환경설정 파일의 내용들은 아라1 명령을 사용하여 메뉴 형태로 다시 설정할 수 있다．



                                               119 / 312
커 널 연구회（www.kerne比z)                                            정재준 (r야키3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                      4. Device Tree 실습   ]20




$ make ARCH=arm CROSS_COMPILE=arm-eabi- menuconf ig




                         Li針ux/ ar湃 4，已日 K色mnel Conftgur各t乞on
      Arrow keys navigate the menu. <Enter> sel. ects submenus - - -> (or empty
      subnenus - - - -). Highlighted letters are hotkeys. Pressing <Y>
      includes, <N> excludes, <M> moduLarizes features. Press <Esc><Esc> to
      exit, <?> for Help, </> for Search. Legend: [*} built- in [ 1 excluded

           (8) 卜始xthum PAGEm SIZE order of alignment 加r D卞4A 10卜倂U buffers
               General, setup - - ->
           [*3 Enable 如adable module support
           -卉． Enable the block layer
               System Type
               會us support
               Kernel. Features
           I   Boot o.ttons --..>
               cPu Power Management - - ->
               Floating point emulation
               珏serspace binary formats
               Power management options
           [*3
               Networking support - - ->
                莎evice Drivers 七 m m>
               FUe systems - - ->
               Kernel, hacking - - ->
                5ecurity options - - ->
               Cryptographic API - - ->


                 <Select>     < Extt >       < Help >     < Save >    < Load >




위에서 Boot options 메뉴를 엔터하여 아래떽 device tree 관련 내용이 설정되어 있는지 확인한다．




                                              120 / 312
커널연구회佃ww,ker肥l.b기                                                    정재준 內bi3307@nate.com)
Device Tree 상세분석 in 니flux Kerr倒 4.0                                       4. Device Tree 실습   121




         i的gi起)rflyHO蜘＝a 和／p.’이ectsfker！在eI/ inux-4.0



                                   鈿口t' 心弘t定m心
      Arrow keys navigate the menu. <Enter> selects submenus 」, -> (or empty
      submenus ----).  Highlighted letters are hotkeys. Pressing <V>
      includes, <N> excludes, <州> modularizes features. Press <Esc><Esc> to
      exit, <?> for Help, <I> for Search. Legend: [*] built- tn [ I excluded

          a   Flattened Devtce Tree su· . or d
          [*}   Support 加r the tradttt｛  가lal 有了AGS b口＜珪 data passing
          [ J      Provide old way to pass kernel parameters
          (exe) Co夙pressed RON boot loader base address
          (exe) Compressed RO川 boot loader BSS address
          [*J Use appended device tree blob to zlmage (EXPERIMENTAL)
           *j   Supplement the appended 0TB with traditional ATAG information
                   笑ernel comnand line type (Use bootloader kernel arguments 1.
          (root=/dev/ ram0 1w randtsk=8192 tnttrd=0x41000660, 8卜4 console二ttySAC
                Kernel command line type (Use bootloader kernel arguments if
          [ jKexec system call (EXPERIMENTAL)
          [ ] Build kdurnp crash kernel (EXPERIMENTAL)
          .밖. Auto calculation of the decompressed kernel image address




               5electa      < Exit >       <Help>       < Save >     < i 心弓硅 :>




위의 정보들은 커널이 부팅하는 지점（kernel_entry）에서 디바이스 트리의 dtb의 위치를 전통적
(OLD）으로 ATAGS를 사용하는 것으로 설정하는 것이다．


OLD: kernel_entry(0, mach_id, atag_addr)
NEW: kernel_entry(0, mach_id, dtb_addr)


또한, 커널를 빌드한 이미지인 기mage에 device tree 비ob(dtb）를 추가하고 전통적（OLD）인 ATAGS
정보에 dtb를 추가하여 부팅한다는 의미이다．




다음으로 아래 그림과 같이 Systen갸 Type 今 Samsung EXYNOS 메뉴를 엔터하여 EXYNOS5420을
선택한다．




                                           121 / 312
커널연구회佃ww.kern이.bz)                                                 정재준 四bi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                                                                                                  4. Device Tree 실습   122




                                           en'中HomeZ: -/projec乞5/Ke rn亡t/ilflU多「4



                      ! tnuxfar同 4.o.e g色r六el. Confi.易uratti｝朴
    Arrow keys navigate the menu, <Eater> selects submenus , - -> (or empty
    submenus - .. -). Htghflghted letters are hotkeys. Pressing <V>
    Includes, <H> excludes, <M> modularizes features. Press <Esc><Esc> to
    exit, <?> for Help, e/> for Search. Legend: VJ built- tn [ j excluded

         如) N磊xl.卜艮Jm PAGEmS王ZE order of alignment for DMA I｛外們U buffers
              General setup
         [기 Cnable loadable nodule support
         - 出- Enable the block lever - m ->
         U    :) stem iT 1e
              S 5tem      e == =
              Bus support 1 - ->
              Kernel Features --->
              馱犯t options , · ,>
              cpu Po났er 卜4anagement -寸 」＞
              多b0ating 叩tnt emubatt（가｝ - ,->
              日serspa四 binary 加mmats -. ,>
              枷｝wer manage川ant opti｛가｝S , m 戶＞
         [*] Networking support - - ,>
              Gevtce Drivers - 中 ->
              rile systems - - ->
              Kernel hacktag . - ->
              Security opti야｝S - - 戶＞
    11
         .*. Cmyptographtc API - - ->


                                            elect>        < Extt >               <Help>                     < Save >                    < load >




                                                     e2: -/proje       釘KerneIi.




     Arrow keys navigate the menu. .<Enter> selects submenus -- -> (or empty
     submenus - - - -). Highlighted letters are hotkeys. Pressing <V>
     includes, <N> excludes, eM> modularizes features. Press <Esc><Esc> to
     exit, e?> for Help, </> for Search. Legend: [*J built- tn [ 1 excluded
    i1



                         ] j lj l
                                j
          L  rexas Instru川ents Keystone Devices
          [  Amlogic Meson SoCs
          [ Freescale t. Mx famtty
          [ ?iedtatek MT65Xx & MTB1xx SOC
             Ti OMAP/ AM/DMIORA Family - - ->




         rLrLrtrtfLr1在
                         m
                         1
                         J}J mj 1j 4
                                   i
                                   J
             Qualcomm Support
             Rockchtp RK2928 and RK3xxx WCS
             Altera SOCFPCA family
             ST SPEAr Family
             STMicroelectronics Consumer Electrontcs SOCs
             Samsuno SSPV210/SSPC1IB

         L
         r                                 Samsung Common options --.>
                         ]

                                           建enesas AR卄 SOCS



          ［小trt [
                         l j 斗1J 까1j =iJ
                                           晟blwtnner SOCs
                                           (SR StRF
                                           N' 'IDIA Tegra
                                            1- Ericsson UBS88 Series


                                           Selec          < Exit >                < Help >                  < Save >                    < Load >
                                                       n蜘；4   g니 小m好心k 注 i ;m ；心 口出片74斗mmm   ;   蜘拙   m   日a m｝土mt   i   寸‘ n出i   口二m m附口쿄4 교   n如   =   二 1   1 n,   m 4 和




                                                                                                 122 / 312
커 널 연구회（www.kern이.b기                                                                                                                                     정쟤준 (rgbi3307@nate.com)
Device Tree 상세분석 a) 나flux Kernel 4.0                                                             4. Device Tree 실습   ]23




                                                 ]projects/Kerne(/Unux.4.O




                                                                                                              1
                                                             艮汪’ =，」r14 毛X났朴C三
      Arrow keys navigate the renu. <Enter> selects subr'ienus 4 . 4 > (or erpty
      subrenus ,. , · ). Highlighted letters are hotkeys. Pressing <V>
      includes, <N> excludes戶 <M> r'odularizes features. Press <Esc>cEsc> to
      exit, <?> for Help, <f> for Search. Legend: [*] built. in [ ] excluded

                                       SaNsung EXYNOS


            rL小trL
                    1j miJ 1
                           1iJ
                                         SA州SUNG EXW蛇S3
                                         S尉作UNG EXYNOS4
                           玄
                                         S丹用SUNG EX넉4055
                                         *古六 EXYNOS socs *玄*




            r뇨 rL r
                  11m rL rL
                              }J l J
                                         느사4SUNG EXVNOSS256
                                         qAMSUNG EXYNOS 5266
                                         bAMSUNG EXYNOS54IO
                     古
                                         SAMSUNG EXYNOSS42
                     4
                     1tJ 4iJ 1j
                                         SMiSUNG EXYNOSS440
                                         SAMSUNG EXVNOS 5880
           L
           r
                             士
                                         ExynosS420 Multt- Cthster PM support




                                       Se1.ect    < Exit >      c Help >         < Save >    < Load >




< Save > 메뉴를 실행하여 환경설정 파일（.config）에 저장한후 < Ex仕 ＞하여 아래와 같이 커널 소
스를 빌드（컴파일）한댜．




$ make ARCH=arm CROSS_COMPILE=arm-eabi

/／중간 생략．. .

  CALL     scr ipts/ checksyscal ls. sh
  HOSTCC scriptsldtcldtc. o
  HOSTCC scripts/ dtc/ f lattree. o
  HOSTCC scripts!dtc/ fstree. o
  I-IOSTCC scripts/ dtc/ data. o
  HOSTCC scr ipts/ dtc/ I ivetree. o
  HOSTCC scripts/ dtc/ treesource 0
  HOSTCC scripts/ dtc/ srcpos. o
  HOSTCC scr ipts/ dtc/ checks. o
  HOSTCC scr ipts/ dtc/ ut i i .0
  앉UPPED sdr 나)tSldtC八Jtc니exer . I ax . C
  SHIPPED scr 1 ptsfdtcfdtc-parser tab.h

                                                                  123 / 312
커 널 연구회（ww比kernel.b기                                                                        정쟤준 內bi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                               4. Device Tree 실습   ]24




 HOSTCC scr ipts/ dtc/ dtc- Iexer. lex.o
 SHIPPED scr ipts/ dtc/ dtc-parser . tab. c
 HOSTCC scripts/ dtc/ dtc-parser . tab. o
 HOSTLD scr 나）ts/ dtc/ dtc

/／이하 생략．. .




커널 소스를 빌드하면 위와 같이 커널 소스 경로의 scripts/dtc/ 관련 파일부터 빌드됨을 확인할

수 있다.      이후에 커널 소스 환경설정（.config）에 따라서 커널 소스 파일들이 빌드된다． 빌드가 완

료될때까지 기다리도록 한다. （수십분 정도 소요됨）



빌드가 완료되면 아래와 같이 arch/arm/boot 경로에 기mage 파일과 arch/arm/boot/dts 경로에 아

키텍별로 dtb 파일들이 생성된다．




  LD       arch/ arm/boot/ compressed/ vml inux
  OBJCOPY arch/armlbootlzlmage
  Kernel : 카oh/arm伯oot／기niage is ready
  DTC      arch/ arm/boot/ dts/ exyn0s421 0-or igen.dtb
  DTC      ar ch/arni/boot /dt s/ exynos4210-smdkv310 . dtb
  DTC      arch/ arm/boot /dts/ exynos42lo- t rats. dtb
  DTC      arch/ arm/boot/ dts/ exynos4210山niversa匕c210. dtb
  DTC      카ch/arrn巾oot/ dts/ exynos4412山먀이du3. dtb
  DTC      arch/ arm/boot /dts/exynos4412-odro I dx. dtb
  DTC      arch/arm/boot/ dts/exynos4412-odroi dx2.dtb
  DTC      arch/ arm/boot/ dts/ exynos4412-or igen. dtb
  DTC      카ch/ arm/boot／아s/exynos4412四mdk4412. d比
  DTC      카ch/ arm幻oot /dt s/exynos4412나 Iny4412.d比
  DTC      arch/arru/boot/ dts/ exynos4412- t rats2 . dtb
  DTC      arch/ arm/boot서四/ exynos525아카nd키e. d比
  DTC      arch/ arm/boot/dts/ exynos5250-smdk5250 . dtb
  DTC      arch/arm/boot/ dts/ exynos5250小snow. dtb
  DTC      카ch/ arm/boot /d四／exyn0s526아刈ref 5260. d山
  DTC      arch/arm/boot/dts/exynos5410-smdk5410. dtb
  DTC      arch/arm/boot/dts/exynos5420-arndale-octa.dtb
  DIC      arch/ arm/boot/ dts/exynos5420-peach-pi t .dtb
  DTC      arch/ arm/boot/ dts/ exynos5420田mdk5420. dtb
  DTC      arch/ arm/boot/ dts/exynos5440尸sd5vl .dtb
  DTC      arch/ arm/boot /dt s/ exynos5440-ssdk5440 . dtb
  DIC      arch/ arm/boot/dts/exynos5800-peach-pi .dtb




이제, 커널이 빌드된 경로인 arch/arm/boot 경로로 이동하여 커널 이미지 파일인 기mage 끝에

dtb 파일（exynos542아카nd키中이ta.dtb）을 추가하여 기mageexyn0s5420나dtb 파일을 만든다．




$ cd arch/ arm/boot/




                                                124 / 312
커 널 연구회佃咐w.ker昶！. t끄）                                          정쟤준 杓t키3307@nate.com)
Device 가ee 상세분석 in Linux Kernel 4.0                                              4. Device Tree 실습   125




 total 10364
drwxrwxr-x 5 jungjj    jungjj    4096 Apr 18 17:30 .1
drwxrwxr-x 90 jungjj   jungjj    4096 Apr 13 07:12 . .1
drwxrwxr-x 2 jungjj    jungjj    4096 Apr 13 07:12 bootp/
drwxrwxr-x 2 jungjj    jungjj    4096 Apr 18 17:30 compressed!
drwxrwxr-x 3 jungjj    jungjj   45056 Apr 18 17:30 dts/
-rw-rw-r-- 1 jungjj    jungjj      46 Apr 13 07:12 .gitignore
-rwxrwxr-x 1 jungjj    jungjj 7014208 Apr 18 17:30 lmage*
  rw-rw-r-- 1 jungjj   jungjj      98 Apr 18 17:30 . lmage. cnid
  rw-rw-r-- 1 jungjj   jungjj    1648 Apr 1307:12 instal l .sh
-rw-rw-r-- 1 jungjj    jungjj    3148 Apr 1307:12 Makef l ie
나나xr川町걔 ] jungjj       jungjj 35녀880 Apr 18 17: 30 기sage士
-rw-rw-r-- 1 jungjj    jungjj     125 Apr 18 17:30 .zlmage. cmd

$ i i dts／火 . d山
-r볘-rw나小 ] Jun（기 J jungj J 36947 Apr 18 17:30 dts!exynos5250-arndale.dtb
-r벡rw나1 ] jungjj jungj J 34377 Apr 18 17: 30 dts1exynos5250-sindk5250.dtb
-r나-rw나小 ] fungi j jungjj 38826 Apr 18 17:30 dts!exynos5250-snow.dtb
-r川rw나--1 jungjj Jungj J 36636 Apr 18 17:30 dts!exynos5250-spring. dtb
  r벼-r나-r-- ] jungjj jungj } 1419가 Apr 18 17: 30 dts!exynos5260-xyref5260. dtb
-r놔-rw나1+ ] jung} J jungj J 5095 Apr 18 17:30 dts/exynos54lo-smdk54lo.dtb
-r卄-r卄-r-- 1 junqjj Jungii 37359 Apr 18 17:30 dts/exynos5420-arndale-octa.dtb
-rw놔rw나--1 jungjj jungjj 47542 Apr 18 17:30 dts!exynos5420-peach-pit. dtb
-r叫rw寸叫 ] Jun（기 J jungj J 38117 Apr 18 17: 30 dts/exynos5420冬mdk5420. dtb
  rw-rw-r-- 1 jungjj jungj J 3685e Apr 18 17:30 dts!exynos5422-odroidxu3. dtb
-rw-rw-r-- 1 jungjj jungj J 7726 Apr 18 17:30 dts!exynos5440-sd5vl. dtb
-r나卜rw나11 ] jungjj jungjj 8261 Apr 18 17:30 dts!exynos54中［)-ssdk5440. dtb
  r네-r刊r-- 1 jungjj jungjj 47236 Apr 18 17: 30 dts!exynos5800-peach-pi .dtb



$ cat zimage dts!exynos5420-arndale-octa.dtb > zlmage_exynos5420_dtb

# ii
 total 13832
drwxrwxr-x 5 jungjj jungjj    4096 Apr 18 17:36 .!
drwxrwxr-x 90 jungjj jungjj   4096 Apr 13 07:12 . ./
drwxrwxr-x 2 jungjj jungjj    的96 Apr 13 07:12 bootp!
drwxrwxr-x 2 jungjj jungjj    的96 Apr 18 17: 30 compressed!
drwxrwxr-x 3 jungjj jungjj   451)56 Apr 18 17:30 dts!
  rw-rw-r-- 1 jungjj jungjj    1 46 Apr 13 07:12 .git ignore
-rwxrwxr-x 1 jungjj jungjj 7014208 Apr 18 17:30 lmage*
  rw-rw-r-- 1 jungjj jungjj    1 98 Apr 1817:30 . image. cmd
나中rw寸11 ] jungjj jungjj       布48A口r 1307:12 i nstai l . sh
나中rw나4e ] jungjj jungjj                 1307:12 Makef l ie
-r놔xr베xr-x ] jungjj jungjj 35］作80 Apr 18 17:30 기mage火
                                帥48A口r
-rw-rw-r-- 1 jungjj jungjj     125 Apr 18 17:30 .zlmage.cmd
-r中rw나- 1 jungjj jungjj 3549239 Apr 18 17:36 zlmage_exynos5420_dtb




이제 최종적으로 작성한 커널 이미지 파일（기mag吐xynos5420_dtb）을 uboot에 올려보도록 하자．
아래와 같이 uboot 명령 프롬프트에서 fastbo야울 실행하여 USB otg Ca비e이 정상적으로 연결되
었는지 확인한다．



                                               125 / 312
커 널 연구회（www.kernel.bz)                                                  정재준 (rgl키3307@nate.con가
 Device Tree 상세분석 In 니flux Kernel 4.0                                             4. Device Tree 실습




 타겟보드 ubo八에서 fast&地ot 실행
 U-Boot 2012. 07-g8c348a3 (Mar 11 201o   15: 31: 43) for ARNDALE OCTA

 CPU: Exynos5420 Rev2. O [Samsung SOC on SMP Platform Base on ARM Car texAl5l
 APLL = 800MHz, KPLL = 600MHz
 MPLL = 532MHz, BPLL = 800MHz

 Board: ARNDALE OCTA
 DRAM: 2 （키B
 WARNING: Caches not enabled

 TrustZone Enabled BSP
 BL1 version:

 Check ing Boot Mode . . . SDMMC
 MMC:    S5P_MSHC2: 0. S5P_MSI-ICO: 1
 MMC Device 0: 7.5 G氾
 MMC Device 1: 7.3 GiB
 MMC Device 2: MMC Device 2 not found
 there are pending interrupts Ox00000001
 In:     serial
 Out:    serial
 Err:    serial
 Net:    Mo ethernet found
 Hit any key to sto口 autoboot: 0 e 여기서 스페이스바를 엔터하면 부트로더로 진입한다．

  /／부트로더 명령 프롬프트에서 환결설정 값을 확인한다．

 ARNDALE # print
 baudr ate=115200
 bootargs=console=ttySAC3,115200n8 root=/dev/ ramO init=/sbin/ init initrd=0x21000000, 32M ramdisk=32768
 bootcmd=run bootcmd_normal ;run bootcmd_extend
 bootcmd extend=mmc read 1 20008000 7800 8; source 20008000
 bootcmd normal=movi read kernel 0 20008000;movi read rootfs 0 21000000 100000;bootz 20008000
 21000000
 bootde I ay=1
 root fs I en=Ox9c1d6
 stderr=ser 1 al
 stdin=ser ial
 stdout=ser ial

  Environment size: 377/16380 bytes

  I/ f astboot을 실행한다．

  AE卜1)ALE # fastboot
  [Partition table on MoviNANDI

nnnnnn
        0
         name= fwb너 ' start=0x3 len=NIA (use hard-coded info. (cind: movi) )

tt   ttt


                U d
              d Q
                  1 5
         name= 'b12 ' start=NIA Ien=N/ A (use hard-coded info. (cmd: movi) )



            4
            1 n
口 口L
   1DDn
         name= 'boot loader ' start=N/A len=NIA (use hard-coded info. (cmd: movi) )
         name= tzsw start=NIA len=NIA (use hard-coded info. (cmd: rnovi) )

       10
         name= 'kernel ' start=N/ A len=NIA (use hard-coded info. (cmd: movi) )
         name= 'ramdisk start=N/ A Ien=0xO(-27262976KB) (use hard-coded info. (cmd: movi) )

                                                 126/ 312
  커널연구회（艸w.kern이.b기                                                        정재준 ｛了gbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                             4. Device Tree 실습   ]27




ptn 6 narne= ' system star t=0x3 Ien=OxO(- 548352000KB)
ptn 7 narne= 'userdata ' start=0x3 len=OxO(NM8352000KB)
ptn 8 nanie= 'cache' start "0x3 len=OxO(-548352000KB)
ptn 9 name= ' fat ' start=0x3 Ien=OxO(N1924911104KB)
USB cable Connected! [CH-O]




위와같이 OTG cable Connected! 메시지가 나오면 정상적으로 연결된 것이다.                                   타겟보드의 uboot
에서 fastboot가 실행되어 있는 상태에서 리눅스 Host PC에서 다음과 같이 fastbo야을 실행하여
앞에서 만들어둔 커널 이미지（ulmage_exynos5420_dtb）를 타겟보드에 전송한다．



우長平 Host PC州 如幽奴
I/ root 계정으로 실행한다．

# fastboot f lash kernel zlmage_e xynos5420_dtb
sending kernel (3466 KB) : . .
OKAY [ O. 438s1
writ ing 'kernel ' . . .
0KAY [ 0.625s]
f inished, total time: 1. 064s




위의 명령이 수행되면 타겟보드三의 uboot에서 대기중인 fastboot에서 다음과 같이 커널 이미지를
전송 받는다．


Starting download of 3549239 byt es

downloading of 3549239 bytes f in i shed
flashing 'kernel
wr i t ing kernel . . device 0 Start 1263, Count 10240
MMC write: dev # 0, block # 1263 , count 10240 . . . 10240 blocks wr i te: OK
co叫키 이ed
part i t ion 'kernel ' f lashed




이제 우분투 Host PC에서 아래！와 같이 타겟보드를 재부팅하자．



# fastboot reboot




시리얼 터미널에 아래와 같이 타겟보드（Arndale Octa Board）의 커널이 부팅되는 메시지（로그）를 확
인할 수 있다.         혹시 아래의 부팅 메시지가 나타나지 않으면 디바이스 트리 생성과정에서 문제가
발생한 것이므로 앞의 과정을 다시한번 확인해 보기 바란다．



                                                  127 / 312
커 널 연구회佃1W＼사．kerr祀나끄）                                                       정재준 畇bi3307@nate.com)
Device 가ee 상세분석 in Linux Kernel 4.0                                             4. Device Tree 실습       ]28




U-Boot 2012.07 (Mar 28 2015 - 15:15:44) for ARNDALE OCTA

CPU: Exynos5420 Rev2.0 [Samsung SOC on SMP Platform Base on ARM CortexA15]
APLL = 800MHz, KPLL = 600MHz
MPLL = 532MHz, BPLL = 800MHz

Board: ARNDALE OCTA
DRAM: 2 G氾
WARNING: Caches not enabled

TrustZone Enabled BSP
BL1 version:

Checking Boot Mode : . . SD새너C
MYC:   SSP_MSHC2: 0, S5P_MSHCO: 1
MMC Device 0: 3. 7 GiB
MMC Device 1: 7.3 GiB
MMC Device 2: MMC Device 2 not found
there are pending interrupts Ox00000001
In:    serial
Out:   serial
Err:   serial
Net:   No ethernet found.
Hit any key to st야） autoboot: 0
reading kernel . .device 0 Start 1263, Count 10240
MMC read: dev # 0, block # 1263, count 10240 . . . 10240 blocks read: OK
completed
reading RFS. .device 0 Start 11503, Count 2048
MMC read: dev # 0, block # 11503, count 2048 . . . 2048 blocks read: OK
coi까니eted

Starting kernel .

      0.0000001 Booting Linux on physical CPU Ox0
      0.000000] Linux version 4.0.0 (jungjj@myHome2) (gcc version 4.6. x-google 20120106 (prerelease)
 0CC) ) #1 SMP PREEMPT Sat Apr 18 17:30:18 KST 2015
      0.000000] CPU: ARMv7 Processor [412fc0f3] revision 3 (ARMv7) , cr=10c5387d
      0.000000] CPU: PIPT I VIPT nonal iasing data cache, PlPT instruction cache
      0.000000] Machine model : Insignal Arndale Octa evaluation board based on EXYNOS5420
      0.000000] cma: Reserved 64 MiB at 0x9b800000
      0.000000] Memory pol icy: Data cache writeal loc
      0.0000001 Samsung CPU ID: 0xe5420020
      0.0000001 Running under secure firmware.
      0.000000] PERCPU: Embedded 10 pages/cpu @ee77d000 s11136 r8192 d21632 u40960
      0.0000001 Bui lt 1 zonel ists in Zone order, mobi l ity grouping on. Total pages: 517136
      0.000000] Kernel command l ine: console=ttySAC3,115200n8 root=/dev/ ram0 init=/sbin/ init
 ni trd=Ox21000000, 28M ramdisk=28672
      0.0000001 PID hash table entries: 4096 (order: 2, 16384 bytes)
      0.0000001 Dentry cache hash table entries: 131072 (order: 7, 524288 bytes)
      0.000000] Inode-cache hash table entries: 65536 (order: 6, 262144 bytes)
      0.000000] Memory: 19556761(12074624K avai lable (4734K kernel code, 193K rwdata, 1680K rodata,
 140K mnit, 275K bss, 53412K reserved, 65536K cma-reserved, 1239040K highmem)
      0.0000001 Virtual kernel memory layout:
      0.0000001      vector : 0xtfff0000 - 0xffff1000       (   4 kB)
      0.000000]       fixmap : 0xffc00000 - 0xfff00000      (3072 kB)
      0. 0000001     vmal loc : 0xf0000000 - 0xff000000     ( 240 MB)

                                               128 / 312
커 널 연구회 (www.ker昶냐끄）                                                       정재준 (rgbi3307@nate.com)
               Device 가ee 상세분석 in Linux Kern이 4.0                                                                          4. Device Tree 실습   ]29




                           0.000000]         1owinem : 0x(t0000000      Oxef 800000  ( 760 MB)
                           0.000000]         pkmap     : 0xbfe00000 - 0xc0000000     (   2MB)
                           0.000000]         modules : 0xbf 000000      0xi幷e00000   ( 14MB)
                           0.000000 1          . text : 0xd0008000      0xc064bc50   (64化 kB)
                           0.000000]           . nit     UX000IC000 - 0xc0688000     ( 240 kB)
                           0. 000000]          .dat a    ux00000ijlju - 0xc06b8740   ( 194 kB)
                           0.000000]             . bss : 0xd06b8740 - 0xc06fd3c0     ( 276 kB)
                           0.0000001 SLUB: HWal ian=64J 0rder=0-3. MinObiects=0. CPUs=8. Nodes=1
                           o.ouuuuoj vreemptioie nierarcnicai icu implementation.
                           0.0000001 Additional per-CPU info printed with stal ls.
                           0.000000] NH그RQS:16 nr_ i 띠5：化 ]6
                           0.000000] GIC physical location is 0x10481000
                           0.0000001 L2C: fai led to 1 rUt: -19
                           0.000000] Switching to timdr-based delay loop, resolution 4lns
                           0.000006] sched_clock: 32 비ts at 24MHz, resolution 4lns, wraps every 178956969942n5
                                                                     d
                           0. 000286] Console: colour ummy device 80x30
                           u.uou口i'+ j i.di IDrating a키ay loop \ sK 甲peu) , vaiue eaicuiatea using timer frequency. . 48.00
                       ogo川PS ( 巾卜240000)
                           0.000334] pid_max: default: 32768 minimum: 301
                           0.000496] Mount-cache hash table entries: 2048 (order: 1, 8192 bytes)
                           0.0005111 Mountpoint-cache hash table entries: 2048 (order: 1, 8192 bytes)
                           0.001209] CPU: .   Testing
                                                        writ1e buffer coherency: Ok
                           0.001574] l.,roo. u먀iate cpu니C텍idei ty iO,)O
                           0.001588] CPUO: thread            cpu     1
                                                                     socket 0, mpidr 80000000



                [[[[
                                                        .   -                 :           .
                                                                1,
                                                                         0,
                                                                                              .   .   .   . 1.   ,   ..


                           0. 001762] aett ing up stst iq iuerit i ty nap 101 0x亡0'}iu0亡o - 0X亡0'IIUL)00
                          0.081328] CPU1: update cpu capacity 1535
                           0. 0813361 CPW: thread -1, cpu 1, socket 0, mpidr 80000001
                          0.101334] CPU2: update cpu卞apacity 1535
rL
t r                       0.1013411 CPU2: thread -1, cpu 2, socket 0, mpidr 80000002
                          0.1213261 CPU3: update cpu_capacity 1535
               [
    L
    r                     0. 121334] CPU3: thread -1, bpu 3, socket 0, mpidr 80000003
                          2. 140016] CPU4: fai led to come onl ine



              [[ [ [
              r
                          4.1600321 CPU5: fai led to come onl ine
                          6.1800491 CPU6: fai led to come onl ine
                          8.200065] CPU7: fai led to come onl ine
                          8.200100] 마ou帥t up 4 CPUs




    [
          [   [[
                          8.200］侶｝ SMP: Total of 4 processors activated (192.00 BogoMIPS) .




                   [   [[   [[
                          8. 200123] CPU: Al l CPU(s) s:tarted in SVC mode.




                                 [[
                          8.200826] devtmpfs: initial ized
                          8.203076] VFP support v0.3: implementor 41 architecture 4 part 30 variant f rev 0
                          8.2053671 pinctrl core: i ni tial ized pinctrl subsystem




r
LL
                          8.228525] NET: Registered p ' 아oco1 fami ly 16




  r   L
      rLr
                          8.230126] DMA: preal located 256 KiB pool for atomic coherent al locations




            L
            r    L
                 r   L
                     r
                          L
                          8.242923] exynos-audss-clk 3810000. audss-clock-control ler: setup completed




                          r    L
                               r
                          8.2509881 EXYNOS5420 PMU ini tial ized
                          8.304656] SCSI subsystem initial ized
                          8.305425] usbcore: recistered new interface driver usbfs
                          8.305590] usocore. rea, sterea new interiace ariver nuo
                          8.3058751 usocore. regisierea new aevice ariver U5D
                          8.3079661 Advanced Linux So nd Architecture Driver Initial ized.
                          8.3092341 Switched to clock ource mct- frc
                          8.333815] NET: Registered p otocol fami ly 2
                          8. 334611] TCP establ ished h sh table entries: 8192 (order: 3, 32768 bytes)
                          8.334724] TCP bind hash tab e entries: 8192 (order: 5, 163840 bytes)
                          8.3349251 TCP: Hash tables onfigured (establ ished 8192 bind 8192)
                          8.3349831 TCP: reno registe ed

                                                                                  129 / 312
    커 널 연구회佃ww.kern包b기                                                                                               정재준 kgbi3307@nate.com노
Device Tree 상세분석 in Linux Kernel 4.0                                                                                                            4. Device Tree 실습




     8. 3350031 UDP hash table entries: 512 (order: 2, 24576 bytes)
     8.335053] UOP-Lite hash table entries: 512 (order: 2, 24576 bytes)
     8.3353291 NET: Registered protocol fami ly 1
     8.3356381 Trying to unpack rootfs image as initramfs. . .
     8.3362741 rootfs image is not initramfs (no cpio magic) ; looks l ike an initrd
     8.4277201 Freeing initrd memory: 28672K (c1000000 - c2c00000)
     8.4308001 futex hash table entries: 2048 (order: 5, 131072 bytes)
     8. 4512531 romfs: ROMFS MTD (C) 2007 Red Hat, Inc.
     8. 4523据］ bounce: pool size: 64 pages
     8.4523361 lo scheduler noop registered
     8. 4523531 io scheduler deadl ine registered
     8.4530041 io scheduler cfq registered (default)
     8.4538521 exynos-m巾너시由아的y 10040714 . 미deo가）hy: regmap lookup fai led: -19
     8.4538761 exynos-mipi中video-phy 10040714. video-phy: can 't request region for resource [mem
0x10040714-0x1004071 f I
     8.4539041 exynos-mi pi-v i deo phy: probe of 10040714. video-phy fai led with error -16
     8. 4553341 12100000.phy suppl y vbus not found, using dummy regulator
     8.455416] 12100000. phy suppl y vbus-boost not found, using dummy regulator
     8. 4559571 12500000.phy suppi y vbus not found, using dummy regulator
     8.4560321 12500000. phy suppl y vbus-boost not found, using dummy regulator
     8. 4609311 dma-p1330 3880000. adma: Loaded driver for PL330 DMAC-241330
     8.4609491 dma-p 1330 3880000. adma: DBUFF-4x8bytes Numfhans七 Num Per卜］6 Nu旺탸ents七
     8. 4666421 dma-p 1330 121a0000 .pdma: Loaded driver for PL330 DMAC-241330
     8. 466659] dma-p 1330 121a0000 .口dma:         DBUFF-32x4bytes Num_Chans-8 Num_Per i- 32 Num_Events-




 鉅 [ [ 鉅 [ [ [ [ [ [ [ [ [ [ [ [ [ [ [ [ [ [ [ [ [ [ [ [ [ [ [ [
                                                                   8. 472435] dma-p1330 121b0000.pdma: Loaded driver for PL330 DMAC-241330
                                                                   8.4724521 dma-p 1330 121b0000 . pdma:       DBtJFF-32x4bytes Num_Chans-8 Num_Per i -32 Num_Events-

                                                                    8.4740731 dma-p1330 10800000.mdma: Loaded driver for PL330 DMAC-241330
                                                                    8. 4740891 dma가키330 10800000. m（如a:           0텨JFF小64x앉가tes Num_Ctians-8 Num中Per卜］ Nu旺Even ts-32
                                                                    8. 592294] Serial : 8250/16550 driver, 4 ports, IRQ sharing disabled
                                                                    8.5947501 12c00000. serial : ttySAC0 at MM山 0x12c00000 ( irq = 58, base_baud = 0) is a S3C6400/10
                                                                    8. 5953671 12c10000. seria1 : ttySAC1 at YMl0 0x12c10000 ( irq = 59, base_baud = 0) is a S3C6400/10
                                                                    8.5959831 12c20000. serial : ttySAC2 at MMI0 0x12c20000 ( 나q = 60, base_baud = 0) is a S3C6400/10
                                                                    8.596593] 12c30000. serial : ttySAC3 at MMI0 0x12c30000 ( irq = 61, base_baud = 0) is a S3C6400/10
                                                                    9.2400331 console [ttySAC31 enabled
                                                                    9.2453411 [drm] Initial ized drm 1.1.0 200608杓
                                                                    9.2646551 brd: module loaded
                                                                    9.2753891 loop: module loaded
                                                                    9.2782421 usbcore: registered new interface driver asix
                                                                    9.2825551 usbcore: registered new interface driver ax88179_178a
                                                                    9. 2885811 usbcore: registered new interface driver cdc_ether
                                                                    9.294449] usbcore: registered new interface driver smsc75xx
                                                                    9.3001931 usbcore: registered new interface driver smsc95xx
                                                                    9.3058241 usbcore: registered new interface driver net1080
                                                                    9 . 없］488] usbcore: registered new interface driver cdc_subset
                                                                    9. 317355] usbcore: registered new interface driver zaurus
                                                                    9.3229781 usbcore: registered new interface driver cdc_ncm
                                                                    9.3294261 usb@12000000 supply vdd33 not found, using dummy regulator
                                                                    9.3350111 usb@12000000 supply vddlO not found, using dummy regulator
                                                                    9.7450461 usb@12400000 supply vdd33 not found, using dummy regulator
                                                                    9. 7501981 usb@12400000 supply vddl0 not found, using dummy regulator
                                                                   10.1583611 xhci-hcd xhci-hcd,2.auto: xHCl Host Control ler
                                                                   10.162434] xhci-hcd xhci-hcd.2. auto: new USB bus registered, assigned bus number 1
                                                                   10.1703691 xhci-hcd xhci-hcd, 2. auto: hcc params 0x0220f04c hci version 0x100 quirks 0x00010010
                                                                   10.178722] xhci-hcd xhci-hcd,2. auto: irq 108, 1 0 mem 0x12000000

                                                                                                              130 / 312
커 널 연구회（蜘／w.kerne山기                                                                                                                      정재준 如gbi3307@nate.com)
Device 가ee 상세분석 in Linux Kernel 4.0                                            4. Device Tree 실습      131




   10.1848931 usb usbi: New USB device found, idVendor=ld6b, idProduct=0002
   10.191430] usb usbi: New USB device strings: Mfr=3, Product=2, SerialNumber=1
   10.198590] usb usbi: Product: xHCl Host Control ler
   10.2034711 usb usbi: Manufacturer: Linux 4. 0.0 xhci-hcd
   10.2087271 usb usbi: SerialNumber: xhci-hcd.2.auto
   10.2146211 hub 1-0:1.0: USB hub found
   10.217342] hub 1-0:1.0: 1 port detected
   10.221827] xhci-hcd xhci-hcd.2.auto: xHCl Host Control ler
   10.226686] xhci-hcd xhci-hcd. 2.auto: new IJSB bus registered, assigned bus number 2
   10.2345841 usb usb2: New USB device found, idVendor=ld6b, idProduct=0003
   10.241082] usb usb2: New USB device strings: Mfr=3, Product=2, SerialNumber=1
   10.248242] usb usb2: Product: xHCl Host Control ler
   10.253124] usb usb2: Manufacturer: Linux 4.0.0 xhci-hcd
   10.2583801 usb usb2: SerialNumber: xhci-hcd.2.auto
   10.264224] hub 2-0:1.0: USB hub found
   10.266992] hub 2-0:1.0: 1 p4rt detected
   10.2715601 xhc i-hcd xhci-hcd.5.auto: xHCl Host Control ler
   10.276347] xhc i-hcd xhci-hcd. 5.auto: new USB bus registered, assigned bus number 3
   10.2843351 xhc i-hcd xhci-hcd. 5.auto: hcc params 0x0220f04c hci version 0x100 quirks 0x00010010
   10.292707] xhc i-hcd xhci-hcd. 5.auto: irq 109, io mem 0x12400000
   10.2987911 usb usb3: New USB device found, idVendor=ld6b, idProduct=0002
   10.3053821 usb usb3: New USB device strings: Nfr=3, Product=2, SerialNumber=1
   10.312569] usb usb3: Product: xHCl Host Control ler
   10.317391] usb usb3: Manufacturer: Linux 4.0.0 xhci 中hcd
   10.322830] usb usb3: SerialNumber: xhci-hcd.5.auto
   10.328475] hub 3-0:1.0: USB hub found
   10.331323] hub 3-0:1.0: 1 pqrt detected
   10.3357381 xhc i-hcd xhci-hcd.5.auto: xHCl Host Control ler
   10.340669] xhc i-hcd xhci-hcd.5.auto: new USB bus registered, assigned bus number 4
   10.3484921 usb usb4: New lJSB device found, idVendor=ld6b, idProduct=0003
   10.355032] usb usb4: New USB device strings: Mfr=3, Product=2, SerialNumber=1
   10.362223] usb usb4: Product: xHCl I-lost Control ler
   10.367045] usb u5b4: Manufacturer: Linux 4.0.0 xhci-hcd
   10.3725161 usb u5b4: SerialNumber: xhci-hcd.5.auto
   10.378152] hub 4-0:1.0: USB hub found
   10.3809741 hub 4-0:1.0: 1 port detected
   10.385470] ehcLhcd: USB 2. 0 Enhanced ' Host Control ler (EHCl) Driver
   10.3913481 ehci-exynos: EHCI EXYNOS driver
   10.395919] exynos-ehci 12110000.usb: EHCI Host Control ler
   10.4009901 exynos-ehci 12110000.usb: new USB bus registered, assigned bus number 5
   10.408767] exynos-ehci 12110000.usb: irq 107, io mem 0x12110000
   10.4293961 exynos-ehci 12110000.usb: USB 2. 0 started, EHCI 1. 00
   10.434122] usb u5b5: New USB device found, idVendor=ld6b, idProduct=0002
   10.440709] usb usb5: New USB device strings: Mt r=3, Product=2, SerialNumber=1
   10.447867] umb u5b5: Product: EHCI Host Control ler
   10.452750] umb usb5: Manufacturer: Linux 4.0. 0 ehci hcd
   10.458005] usb u5b5: SerialNumber: 12110000. usb
   10.463579] hub 5-0:1.0: USB hub found
   10.466358] hub 5-0:1.0: 3 ports detected
   10.471373] ohcLhcd: USB 1.1 'Open ' Host Control ler (OHCI) Driver
   10.476485] ohci-exynos: OHCI EXYNOS driver
   10.481101] exynos-ohci 12120000.usb: USB Host Control ler
   10.486026] exynos-ohci 12120000.usb: new USB bus registered, assigned bus number 6
   10.493794] exynos-ohci 12120000.usb: irq 107, io mem 0x12120000
   10.563508] usb u5b6: New USB device found, idVendor=ld6b, idProduct=0001
   10.568812] usb u5b6: New USB device strings: Mfr=3, Product=2, SerialNumber=1

                                             131 / 312
커 널 연구회佃／ww.kerne나）기                                                   정재준 仕gbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                           4. Device Tree 실습




[   10.576189] usb usb6: Product: USB Host Control ler
[   10.580797] usb usb6: Manufacturer: Linux 4. 0. 0 ohci hcd
[   10.586054] usb usb6: SerialNumber: 12120000. usb
[   10.591622] hub 6-0:1.0: USB hub found
[   10.594406] hub 6-0:1.0: 3 ports detected
[   10.599538] usbcore: registered new interface driver usb-storage
1 10.605142] mousedev: PS/2 mouse device common for al l mice
1   10.6111741 53c-rtc 101e0000. rtc: fai led to find rtc source clock
[   10.615975] s3c-rtc: probe of 101e0000. rtc fai led with error -2
[   10.6222691 i2c /dev entries driver
[   10.660884] PVDD_MlFS_1V1: ramp_delay not set
[   10.671115] PVDD_G3DS그VO: ramp_delay not set
[   10. 707862] thermal thermal zone0: fai led to read out thermal zone (-22)
[   10.7化］51] 10060000. tmu supply vtmu not found, using dummy regulator
[   10.7伯881] thermal thermal zonel: fai led to read out thermal zone (-22)
[   10.726192] 10064000. tmu supply vtmu not found, using dummy regulator
[   10.732963] thermal thermal zone2: tai led to read out thermal zone (-22)
[   10.7393091 10068000. tmu supply vtmu not found, using dummy regulator
[   10.746046] thermal thermal zone3: tai led to read out thermal zone (-22)
1 10.752387] 1006c000. tmu supply vtmu not found, using dummy regulator
[   10.7591571 thermal thermal zone4: fai led to read out thermal zone (-22)
1 10.765473] 100a0000. tmu supply vtmu not found, using dummy regulator
[   10. 773114] s3c2410-wdt lold0000. watchdog: watchdog inactive, reset disabled, irq disabled
[   10. 780897] device-mapper: ioctl : 4.30.0- ioctl (2014-12-22) initial ised: dm-devel@redhat.com
[   10.788477] Driver 'mmcblk ' needs updating - please use bus_type methods
[   10.795231] usb 5-1: new high-speed USB device number 2 using exynos-ehci
[   10.802011] sdhci : Secure Digi tal Host Control ler Interface driver
[   10.8080861 sdhci : Copyright (c) Pierre 0ssman
[   10.8126631 Synopsys Designware Multimedia Card Interface Driver
[   10.819055] dwmmcexynos 12200000.mmc: nurn-slots property not found, assuming ] slot is avai lable
[   10.8273091 dwmmc_exynos 12200000.mmc: IDMAC supports 32-bit address mode.
[   10.834174] dwmmc_exynos 12200000. mmc: Using internal DMA control ler.
[   10.840494] dwmnic_exynos 12200000. mmc: Version ID is 250a
[   10.845889] dwmmc_exynos 12200000.rnmc: DW MMC control ler at irq 87, 64 bit host data width, 64
dee口 f i fo
[   10.8559851 dwminc_exynos 12200000. mmc: No vqmmc regulator found
[   10.899349] dwminc_exynos 12200000. mmc: 1 slots initial ized
[   10.903662] dwmmc_exynos 12220000.mmc: num-slots property not found, assuming 1 slot is avai lable
[   10.912406] dwmmc_exynos 12220000.mmc: IDMAC supports 32-bit address mode.
[   10.919170] dwmmc_exynos 12220000.mmc: Using internal DMA control ler.
[   10.925528] d川rnmc_exynos 12220000. mmc: Version ID is 250a
[   10.930955] dwmmc_exynos 12220000. mmc: DW MMC control ler at irq 88, 64 bit host data width, 64
deep f ifo
[   10.961109] usb 5-1: New USB device found, idVendor=05e3, idProduct=0610
[   10.966330] usb 5-1: New USB device strings: Mfr=0, Product=1, SerialNumber=0
[   10.973474] usb 5-1: Product: USB2.0 Hub
[   10.9785321 hub 5-1:1.0: USB hub found
[   10.981482] hub 5-1:1.0: 4 ports detected
[   10.982289] mmc0: MAN_BKOPS_EN bit is not set
[   10.983037] mmc_host mmc0: Bus speed (slot 0) = 50000000Hz (slot req 52000000Hz, actual
50000000HZ div = 0)
[   10.9835101 mmc_host mmco: Bus speed (slot 0) = 100000000Hz (slot req 52000000Hz, actual
50000000HZ div = 1)
[   10.983693] mmco: new DDR MMC card at address 0001
[   10.984970] mmcb1k0: mmc0: 0001 M8G1WA 7. 28 GiB
    10.985234] mmcblkobooto: mmco:0001 M8G1WA partition 1 2.00 MiB

                                             132 / 312
커 널 연구회（www.kern이.b기                                                   정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                             4. Device Tree 실습         133




    10.9855101 mmcb나；obootl: mnicO: 0001 M8G1WA partition 22.00 MiB
    10.985770] mmcblkorpmb: mmco: 0001 M8G1WA partition 3 128 KiB
    10.9894441 dwmmc_exynos 12220000.mmc: 1 slots initial ized
    10.991266] 때ncb나（0: p] 口2 口3 p4
    10. 9966961 usbcore: registered new interface driver usbhid
    10.9967071 usbhid: IJSB HID core driver
    11 . 0082771 TCP: cubic registered
    11.0083051 NET: Registered 아아叩ol fami ly 17
    11.0084291 NET: Registered protocol fami ly 15
    11.0090331 Registering SWP/SWPB emulation handler
    11.0135861 power-domain: Power-off latency exceeded, new value 380250 ns
    11.0138461 power-domain: Power-off latency exceeded, new value 230375 ns
    11.013878] power-domain: Power-off latency exceeded, new value 354333 ns
    11.014281] power-domain: Power-ott latency exceeded, new value 374917 ns
    11.014322] power-domain: Power-off latency exceeded, new value 377125 ns
    11.0161711 input: gpio_keys as /devices/platform/gpio_keys/ input/ inputo
[   11.017761] drivers/ rtc/hctosys.c: unable to open rtc device (rtc0)
[   11.048669] mmc_host mmcl: Bus speed (slot 0) = 50000000Hz (slot req 50000000Hz actual
50000000HZ div     0)
1   11.048814] mmcl: new high speed SDHC card at address b368
[   11 .0501681 mmcblkl: mmcl: b368        3.71 GiB
    11.052847] mmcblkl: p1 p2 p3 p4
    11.1214131 PVDD_G3D_1V0: disabl ing
    11.127247] PVDD_G3DS_1VO: disabl ing
    11.130350] random: nonblocking pool is initial ized
    11.133125] PVDD_HSIC_1V8: disabl ing
    11.134721] PVD口AB巳1V8: disabl ing
    11.136305] PVDD_ANA나_1V8: disabl ing
    11.137888] PVDD_ANA나_1VO: disabl ing
    ] ] 기 394751 PVDD_ADC_1V8: disabl ing
    11.1410641 PVDD_APIO_lV8: disabl ing
    11 .1474301 ALSA device l ist:
    11.147438]     No soundcards fo[    11.1830471 RANDISK: gzi p image found at block 0
    11.2596631 VFS: Mounted root (ext2 fi lesystem) readonly on device 1:0.
    11.254918] devtmpfs: mounted
    11.267958] Freeing unused kernel memory: 240K (c064c000 - c0688000)
Starting logging: OK
Initial izing random number generator. . . done.
Starting network. . .

Welcome to Exynos5420
Exynos5420 login: [   11. 459626] usb 5-1.4: new high-speed USB device number 3 using exynos-ehci
[   11.570751] usb 5-1.4: New USB device found, idVendor=0b95, i dProduct=772a
    11.576146] usb 5-1.4: New USB device strings: Mfr=1, Product=2, SerialNumber=3
    11.583467] usb 5-1. 4: Product: AX88772
[ 11.5873221 usb 5-1.4: Manufacturer: AS以 Elec. Corp.
[ 11 .592389] usb 5-1.4: SerialNumber: 000001
[ 11 .598865] asix 5-1. 4:1. 0 (unnamed net_device) (uninitial ized) : inval id hw address, using random
[ 12.423901] asix 5-1.4:1. 0 ethO: register 'asix ' at usb-12110000.usb-l. 4, ASIX AX88772 tJS8 2.0
Ethernet, 96:5e:48:ds:bc:51

Welcome to Exynos5420




그런데, 아직 램디스크는 포팅하지 않은 상태이므로 대부분의 독자분들 타겟보드에서 아래와 같이

                                               133/ 312
커 널 연구회（ww比kerne나끄）                                                       정재준 (rg너3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                             4. Device Tree 실습        13可




램디스크를 마운트 하는 과정에서 오류 메시지가 나타날 것이다．


     6.710420] RAMOISK: gzip image found at block 0
     6.753019] usb 5-1.4: new high-speed tJS8 device number 3 using exynos-ehci
     6.769121] List of al l partitions:
     6.771170] b300          7634944 mmcb1k0 driver: macblk
     6.776431]   b301           5881238 mmcblkOpl 00000000-01
     6.7817051 b302              537372 mmcb1k0p2 00000000-02
     6.7870031 b303              537372 mmcb1k0p3 00000000-03
     6.792275]   b304            537372 mmcb1k0p4 00000000-04
     6.797568] b3化                128 mmc비korr痲） (driver기
     6.802814] b310              2048 mmcblkObootl (driver?)
     6.808047] b308              2048 mmcblkOboot0 (driver?)
     6.813358] b320          7822336 mmcblkl driver: mmcblk
     6.8186181 b321             6074100 mmcblklpl 00000000-01
     6.823904]   b322            535500 mmcblk加2 00000000-02
     6.829189]   b323            535500 mmcblk加3 00000000-03
     6.834500]   b324            535500 mmcblklp4 00000000-04
     6.839772] No fi lesystem could mount root, tried: ext3 ext2 ext4 cramfs vfat msdos romfs
     6.8479941 Kernel panic - not syncing: VFS: Unable to mount root fs on unknown-block(0,O)
     6.8562281 CPU: 0 PID: 1 Comm: swapper/0 Not tainted 4.0 #1
     6.8621371 [<c0013b5c>1 (unwin&.backtrace) from [<c0010d1c> ] (show_stack+Oxl0/0x14)
     6.869839] [<cOOlOdic> ] (show_stack) from [<c041f2a4> ] (dump_stack+0x68/0xb8)
     6.8770271 [<c041f2a4> ] (dump_stack) from [<c041c174> ] (panic+0x8c/oxlfo)
     6.883873] [<c041c174> ] (panic) from [<c05b3160>] (mount_blockjoot+0x258/0x2a0)
     6.891323] [<c05b3160> ] (mount_block_root) from [<c05b3dc8> ] ( mni trd_ load+0xbc/0x2e0)
     6.899207] [<c05b3dc8> ] ( m i trd.joad) from [<c05b33b8> ] (prepare..namespace+0xc4/oxlc4)
     6.907184] [<c05b33b8> ] (prepare_namespace) from [<c05b2db4>1 (kernel_ m i t_freeable+0x180/0x1c8)
     6.916021] [<c05b2db4> ] (kerne匕init_ freeable) from E<co4ladcc> ) (kerne匕init+0x8/0xe4)
     6.9240791 [<co4ladcc> ] (kernel_ m it) from [<c000e638> ] (ret_from_fork+0x14/0x3c)




4.3.4 램디스크 포팅
이제 램디스크를 포팅하자.                  램디스크는 아래의 buildroot.org 웹사이트에서 램디스크를 쉽게 생성
할 수 있는 도구를 제공해 준다．


http://八／ww.buildroot.org


먼저 이t 명령으로 buildroot 도구 프로그램을 다운로드 받는다．



$ gi t clone git: //gi t.bui ldroot.net/bui Idroot


/／아래와 같이 bui Idroot 경로가 생성되면서 관련 파일들이 다운로드 된다 .（몇분 소요됨）

Cloning into 1 bui ldroot . . .
remote: Counting objects: 163662, done.
remote: Compressing objects: 100% (60707/60707) , done.
remote: Total 163662 (delta 112493) , reused 150204 (delta 102131)

                                                     134/ 312
커 널 연구회（ww＼사, kernel.b기                                                  정재준 佃b日307@nate.com)
Device Tree 상세분석 in 니nux Kernel 4.0                                           4. Device Tree 실습   135




Receiving objects: 100% (163662/163662) , 40.75 MIB I 219 KiB/ s, done.
Resolving deltas: 100% (112493/ 112493) , done.

$ cd bui Idroot
$ II

drwxr-xr-x   14 jung) ] jungjj  4096 Mar 28 14: 03 .1
drwxr-xr-x    6 jungjj jungjj   4096 Mar 28 13: 58 . .1
di나xr나M出      2 jung] ] jungj j 4096 Mar 28 14: 03 카ch/
drwxrwxr-x   25 jungjj jungj j  4096 Mar 28 14: 03 board/
drwxrwxr-x   15 jungjj jungj j  4096 Mar 28 14: 03 boot/
-rw-rw-r--    1 jungjj jungjj 146433 Mar 28 14:03 CHANGES
  rw-rw-r--   1 jungjj jungjj 19111 Mar 2814: 03 Config. in
  rw-rw-r--   1 jung] ] jungjj 42307 Mar 2814: 03 Conf 1 g. in, legacy
drwxrwxr-x    2 jungjj jungjj   4096 Mar 28 14: 03 configs/
-rw-rw-r--    1 jungjj jungj j 17987 Mar 28 14: 03 COPYING
m대中1W나小       ] lun｛기 j jungj j 1246 Mar 28 14:03 .defcont ig
drwxrwxr-x    5 jungjj ;ungj j  4096 Mar 28 14:03 docs/
drwxrwxr-x   14 jungjj jung] )  4096 Mar 28 14:03 fs/
drwxrwxr-x    8 jungjj jung] ]  4096 Mar 28 14: 03 .git/
  rw-rw-r--   1 jungjj jung] ]   125 Mar 28 14: 03 .git ignore
drwxrwxr-x    2 jungj] jungj j  4096 Mar 28 14: 03 I inux/
  rw-rw-r--   1 jungj] jungj] 34526 Mar 2814:03 Makef i le
  rw-rw-r--   1 jung) ] jungjj  2432 Mar 2814:03 Makefi le. legacy
drwxrwxr小x 1221 ]ungj] jung] ] 36864 Mar 28 14:03 package/
  rw-rw-r--   1 jungjj jungj]   2032 Mar 28 14: 03 README
drwxrwxr-x   11 jung] j jungjj  4096 Mar 28 14: 03 support/
drwxrwxr-x    3 Iungjj jungjj   4096 Mar 28 14: 03 systern/
drwxrwxr-x    5 jungjj jungj j  4096 Mar 28 14: 03 toolchain/


buildroot 경로로 이동하여 make menuconfig 를 실행하여 빌드 환경설정을 수행한후 make을 통

하여 램디스크를 생성한다.                 아래와 같은 순서대로 실행한다．

먼저 make menuconfig 명령을 실행하면 다음과 같은 환경설정 메뉴가 나타난다.




                 Buti.心r肖恥｝t 2015. 妨嶝仕出B和3S呼｝9c8？客每今 Con姓琴甘各tton
       Arrow keys navtgate the menu. .cEnter> selects submenus ---> (or empty
       submenus 」- - -). Highlighted letters are hotkeys. Pressi,ng <V> selectes
       a feature, while <N> will exclude a feature. Press sEsc><Esc> to extt,
       <?> for Help, </> for Search. Legend: [*J feature is selected [ ]

                  TarS et 小 tton三
                  拉uUd options      h>

                  Toolchatn 卄 - ->
                  System configuration - - ->
                  Kernel - ! 口>
                  Target packages - . ->
                  Ftlesysten images - - ->
                  Bootloaders 4 4 >
                  Host utilities   - ->
                  Legacy config options 4 - ->




                                                 135 / 312
커 널 연구회如四Vw.ker倒.b기                                                       정재준 似恥妃307@nate.com)
Device 가ee 상세분석 in Linux Kernel 4.0                                          4. Device Tree 실습   ]36




위에서 Target 야川ons는 다음과 같이 설정한다．


        un羽管rnyHon作2: -/pr기e改s/t t_exyn055420/30小rem（치5k/buItdroot
        難芸璘必唾珏玎 되｝:
        弘澍交的翕汗
                                  加r心好t ｛珀ti-毓特
    Arrow keys navigate the menu. <Enter> selects submenus -. -> (or empty
    sub斛enus 8 .4 . ). Highlighted letters are hotkeys. Pressing <V> selectes
    a feature, white <N> wilt ecclude a feature. Press <Esc><Esc> to exit,
    <?> for Help, </> for Search. Legend: [*} feature is selected [ j
         1
             rarget Binary Format (ELF) - 4- >
             Target Architecture Variant (cortex- Als)
             Target ABI (EABI)
             Floating point strategy (VFPv4- 016)
             義R川 instruction set (ARM)




    L


             Select      < Exit ;>    < Help >      < Save >     <; Load >




다음으로 Build 이乂向ns는 다음과 같이 설정한다. （기본적인 옵션）




                恥Ltldr好臼t 2615.C｝됴叫gtt-e拉芍654g9c828好9 Confl穹Urat Lu斗
     Arrow keys navigate the menu. <Enter> selects subrienus - - -> (or empty
     submenus - -- -). Highlighted letters are hotkeys, Pressing <Y> selectes
     a feature, while <N> will exctude a feature. Press <Esc><Esc> to exit,
     <?> for Help, </> for Search. Legend: [*] feature is selected [ }

                          tton
              Build o. ttons --->
              Toolchatn m m . >
              system configuration - - ->
              弦ernel --->
              Target packages - - ->
              芦ilesystem images , - ->
              缸｝otl始ders - - ->
              F衣｝st utilities   - 中 n>
                egacy config options -中 ->



                                             136 / 312
커 널 연구회（www.ker昶나끄）                                                    정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                        4. Device Tree 실습   137




                                                                                      1
                                      蜘tid （叩ti各l's
        Arrow keys navigate the menu. <Enter> selects sub尹lenus . -> (or empty
        submenus - ---). Highlighted 1.etters are hotkeys. Pressing <Y> selectes
        a feature, white <N> will, exclude a feature. Press <Esc><Esc> to exit,
        <?> for Kelp, <I> for Search. Legend: [*] feature is selected [ ]

           I    Coi.wiands
            ($(coNF1G_DIR) /defconftg) Location to save butldroot conftg
            ($(ToPorR) /dl) 的wnl.oad dir
            ($(BASE小DIR)／卜'ost) 汁：.st dir
                Mtrrors and i沁닝nl.oad locations    寸, >
                Number of jobs to run simultaneousl.y (0 for auto)
                Enable compiler cache
                 Show options and packages that are deprecated or obsolete
                 build packages with debugging symbols
                 strip command for binaries on target (strip)
                毋xecutables that should not be stripped
                 directories that should be skipped when stripping
                 孕cc opti尹伉zati｛기） level 佃ptirrtze 加r size)
                 t士tenabling stack Smashing Protectton requires support in the
                 Libraries (shared only) - - ->
            ($(CONFIC_DIR刃locat.mk) tocation of a package override file
            C) global patch directories
                 缸如anced . n ->


    I

                Select>    < Exit >     < Help >     < Save >    < Load >




댜음으로 Toolchain 옵션은 다음과 같이 설정한다．




                    取it珌r蜘蛇 2旣！恣5小珏培餌好唾虹蛇帥多 Conft客臂r
        Arrow keys navigate the 竹enu. <Enter> selects submenus - -4 > (or empty
        submenus ----).      Highlighted letters are hotkeys. Pressing cY> selectes
        a feature, while <N> will exclude a feature. Press 'zEsc><Esc> to exit,
        .z? > for Kelp, .c/ > for search. Legend: [*] feature is selected [ ]

                rarget options - - ->
                客uild 小ti口ns , - .>

                   stem configuration
                Kernel -- ->
                Target packages -
                Ftlesystem images U >
                I300tloaders - n ->
                Host utilities    - - ->
                Legacy config options - - 小




                                              137 / 312
커 널 연구회（www.kern이. b기                                                정쟤준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                   4. Device Tree 실습   13




          'Un釘｝曲rnyHomez: ‘加r이ects／針小母5yn0s5420,凸色ramd作k/buitdroot




       Arrow keys navigate the rlenu, <Enter> selects sub가enus ---> (or eripty
       subisenus . . --). Highlighted letters are hotkeys. Pressing <Y> sel.ectes
       a feature, white <N> will exclude a feature. Press <Esc><Esc> to exit,
       c?> for Helps </> for Search. Legend: [*] feature is selected [ j

          1   T. .lchatn t 'e Butl'r. .t t. 1tChntn
          (butl.droot) {, ustoN toolchatn vendor name
              必*卞 Kernel Header Options **六
              恥ernel Headers (Linux 3.18. x kernel, headers)
              C library (uCltbc)
              *士六 ucl.tbc Optt아｝S 女士*
              uC1.ibc C library Version (uCtibc 6.9. 33. x)   -.>
          (package/uclibcfuCltbc小.9. 33.config) oCltbc configuratton file to
          [*3 Enable large file (files > 2 GB) support
          [ jEnable IPv6 support
          [ 3 Enable RPC support
          ［사 드nable 닒CHAR support
          [) Enable toolchain 如cale/ t18n support
              Thread library thpl.er'* ntatton (Native P0SIX Threading (NPTL) )
          [ 3 Thread 1,tbrary debugging
          [ ] 呈nable stack 마oteCt如n support
          [*3 Conpile and install uClibc utilities
          [ 3 conpil.e and install. uClibc tests
              古出士 Btnuttls Optio,心 必* 身
              Etnuttls Version (binutils 2. 24)


              cSetect>     < Exit >         < Help >       < Save >         < Load >




다음으로 System conhigurat山n 옵션은 다음과 같이 설정한다．


          尸ng甘孕싸Home함 姓莎이a吐sf6lexynos5420乃아ramdkkfbuitdroot


  y1             山口 1 1 口 므   4 = 나  m 山   1 .   日 日 = H 日 4 =1       戶거        1       !   U二5斗느丘養月g
                 t恥八乞or心心t    <!J:L>！口b..91. t. .口口0心＞m9yCb亡｛j心y   L口nri. g王jr苾ttQn
       Arrow keys navigate the nenu. <Enter> selects submenos - - 小 (or enpty
       submenus -小 -). Highlighted letters are hotkeys. Pressing <Y> selectes
       a feature, while <N> will exclude a feature. Press ctsc><Esc> to exit,
       .c?> for Help, </> for Search. Legend: [*3 feature is selected [ 3

               Target options . m 」＞
               Eutld options --->
               了ool.chatn - -
               S steri conft.uratton 山竹 中＞
               Kernel. - - ->
               了arget pac卜；ages
               Filesysten inages
               eootloaders - ! ->
               Host utilities   m - ->
               ,egacy config options




                                                 138/ 312
커 널 연구회（www.kernel.bz)                                                           정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니nux Kern이 4.0                                                              4. Device Tree 실寸139




       沁ng水myHome: 갸多r이cc                            61.exynos5420/30卄ramdisk/buttdro口



                                              at
    Arrow keys navigate the menu. <Enter> selects submenus . m . > (or empty
    subrienus - --).  Htghltghted letters are hotkeys. Presstng <Y> sel.ectes
    a feature, whil.e <N> will, exclude a feature. Press <ESC><ESC> to exit.
    .z?> for Help, </> for Search. Legend: [*] feature is selected [ ]

          . nos5420 S stem hostname
         4e
        (Welco까e to exynosS420) system banner
            Passwords encoding (mds)
             mnit system (BusyBox) ...>
             /dev management (Static using device table)
        (system/devicem table. txt) Path to the permission tables
        仁yste丙／devtc乞tablec相v. txt) 莩‘ath to the device tables
             駟ot FS skeleton (default target skeleton)
        () Root password
             /bin/ sh (busybox ' default shell.) . ' '>
        E*1 Run a getty (login prompt) after boot
               孕etty options , n .>




              [( [( ( ( /
                   j
             remount root filesystem read,write during boot
                   女

                   뇨
                   1/




                        \
             Network interface to configure through DHCP
                              }
                              iJ
             Install, ttmezone Info
                   )
             Path to the users tables


                    1
                    }/\/ 1J
             Root fil. esystem overlay dIrectories
             Custom scripts to run before creating ftlesystem images
              J
             Custom scripts to run after qreating filesystem Images



                                   Select     < Extt >       < Help >   < Save >     < Load >




다음으로 Filesystem images는 다음과 같이 설정한다．




                utldr心口t 2作 5.05件gtt-苾毋珏05－穿多c82臼好孕 如a桃藝urat蜘a
     Arrow keys navtgate the menu. <Eater> selects submenus - - -> (or empty
     submenus 4, , -). Highlighted letters are hotkeys. Pressing <Y> selectes
     a features white <N> will. exclude a feature. Press <Esc> cEsc> to exit,
     <?> for Help, </> for Search. Legend: [*3 feature is selected [ 3

                                   Target options . . .>
                                   Build 口ptions 戶 , ->
                                   Tool.chatn . . ->
                                   System configuration
                                   Kernel -- ->
                                    ar

                                   Boottoaders - - ->
                                   H. st utilities  - + 4>
                                   Legacy config options




                                                                 139 / 312
커 널 연구회（www.kernel.b기                                                                    정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                                     4. Device Tree 실습   }40




          恥ng加各myHorl｝日2: 낳projects/61斗exyr山s5420/30呻ramdisk/buitdroot



                                  卜注，Le！浮stem t外ages
      Arrow keys navigate the menu. <Enter> selects subrienus - -> (or empty
      submenus -.--).  Htghl.tghred letters are hotkeys. Pressing <Y> selectes
      a feature, white <N> will exclude a feature. Press <Esc><Esc> to exit,
      <?> for Help, </> for Search. Legend: [*] feature is selected [ j

              r1
              [
              1
              iJ mj j
                     .=i旺m1汪衣朴4如띠MSt1I Ll뇨三41A [4小胤血닙
              亡pio the root fil. esystem (for use as an initial RAM filesystem)
                    t
              r;ramfs root filesystem
                 [ r1
                    1
              t?xt2/ 3/ 4 root ftl. esystem
                  ext2/ 3/ 4 variant (ext2 (reve) ) -, ->
          ()      fil. esystem label
          （하      size in blocks (leave at 8 for auto calculation)
          (0)     modes (leave at 8 for auto calculation)
          (0)     reserved blocks percentage
                  Compression method (gzip) --->
              希出北 inttramfs needs a Linux kernel to be built 亡六六
              } j 1iJ 11
                       1J 11J
               jffs2 root fttesystem
              r＜坪｝fs root ftlesyste同
                          卉
              squashfs root filesystem
              riL r1
                   1牛 riL riL
              tar the root ftlesystem
               \J
                  Compression 和ethod (grIp)
          1
          m
               r1\
                  other random options to pass to tar

                         기 J ]1J
              ubtfs root ftlesystem
               t rL
              yffs2 root filesystem




                             <Select>   < Exit >      < HeLp >       < Save >      < Load >




그리고 나머지 옵션（Kernel, Ta띠et packages, Bootloaders, Host utilities, Legacy config options）들은
설정없이 defau仕로 한다．


위와 같이 설정한후 <Save> 하면 다음과 같이 .config 파일이 생성된다.


$ H
total 428
drwxr-xr-x             15 jungjj jungjj    4096 Mar 28 14: 24 .1
drwxr-xr-x              6 jungjj jungj j   4096 Mar 28 13: 58 . .1
drwxrwxr-x              2 jungjj jungj j   4096 Mar 28 14: 03 arch!
drwxrwxr-x             25 jungjj jungj j   4096 Mar 28 14: 03 board!
drwxrwxr-x             15 jungjj jungj j   4096 Mar 28 14: 03 boot!
 rw-rw-r---             1 jungjj jungj j 146433 Mar 28 14: 03 CHANGES
-rw-rw나--               1 jungjj jungjj 55199 Mar 28 14:22 .config
 rw-rw-r--              1 jungjj jungj j 19111 Mar 28 14: 03 Conf ig. in
-rw-rw-r--              1 jurigj j jungjj 42307 Mar 2814:03 Cont 1 g. in, legacy
drwxrwxr-x              2 jungjj jungjj    4096 Mar 28 14: 03 cont igs/
나볘나w나小                  ] jungjj jungjj 17987 Mar 28 14: 03 COPYING
  rw-rw-r--             1 jungjj jungjj    1246 Mar 28 14: 03 .defcontig
drwxrwxr-x              5 jungjj jungj j   4096 Mar 28 14: 03 docs!

                                                         140 / 312
커 널 연구회佃쌔／w.kernel.bz)                                                             정재준 內bi3307@nate.con功
Device Tree 상세분석 ir) 니flux Kernel 4.0                                           4. Device Tree 실습    ]41




drwxrwxr-x   14 jungjj   jungjj     4096 Mar 28 14:03 fs/
drwxrwxr-x    8 jungjj   jungjj     4096 Mar 28 14:10 .git/
-rw-rw-r--    1 jungjj   jungji      125 Mar 28 14:03 .git ignore
drwxrwxr-x    2 jungjj   jungjj     4096 Mar 28 14:03 l inux!
-rw-rw-r--    1 jungjj   jungjj    34526 Mar 28 14:03 Makef l ie
-rw-rw-r--    1 ;ungjj   jungjj     2432 Mar 28 14:03 Makef l ie. legacy
drwxrwxr-x    3 jungjj   jungjj     4096 Mar 28 14:10 output!
drwxrwxr-x 1221 jungjj   jungjj    36864 Mar 28 14:03 package!
나忙rw寸十        ] jungjj   jungjj     2032 Mar 28 14:03 README
drwxrwxr-x   11 jungjj   jungjj     4096 Mar 28 14:03 support/
drwxrwxr-x    3 jungjj   jungj j    4096 Mar 28 14:03 system!
drwxrwxr-x    5 jungjj   jungjj     4096 Mar 28 14:03 toolchain/


.config 파일의 내용을 확인해 보면 위에서 설정한 여러가지 환경변수들이 설정되어 있음울 알 수
있다．


#
# Automatical ly generated fi le; DO NOT EDIT.
# Bui Idroot 2015.05-gi t-00605-g9c82009 Configuration
#
BR2_HAVE_DOLCONF I G=y

#
# Target options
#
# 8R2 arcie is not set
# BR2 arceb is not set
BR2_ar m=y
# BR2 armeb is not set
# BR2 aarch64 is not set
# BR2 bf in is not set
# BR2 1386 is not set
# BR2 microblazeel is not set
# BR2 microblazebe is not set
4 BR2_mips is not set
# BR2_mipsei is not set
# BR2_mip564 is not set
4 BR2_mip564e1 is not set
4 BR2 nios2 is not set
# BR2_r兀나erpc is not set
# BR2_powerpc64 is not set
4 BR2. 刃werpc64ie is not set
# BR2 sh is not set
# BR2 sh64 is not set
4 BR2_sparc is not set
4 BR2 x86 64 is not set
4 BR2 xtensa is not set
8R2 ARCH="arm"
BR2 ENDIAN="LITTLE"
BR之吼C_TARGET_ABI=' aapcs니 I nux m
BR2_GCC_TARGET_CPtJ= ' cor tex-a15'
BR2_GCC_TARGET_FPU= ' Vt pv4-d16 "
BR2_GCC_TARGET_FLOAT_ABI = 'sot ftp
BR2_GCC_TARGET_MOOE=' arm"

                                                  141 / 312
커 널 연구회（www.kern毗끄）                                                        정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                         4. Device Tree 실습     142




BR2_ARCH_HAS_ATOM I CS=y
BR2_B I NFMLSUPPORTSSHARED=y
BR2_B I NFMT_ELF=y
BR2_ARM_CPU_HASNE0N=y
BR2_ARM_CPU_HASVFPV2=y
BR2_ARM_CPU_HAS_VFPV3=y
BR2ARM_CPU_HASVFPV4=y
BR2_ARM_CPU_HAS_ARM=y
BR2ARM_CPLHAS_THUMB2'=y
BR2_ARM_CPU_ARMV7A=y
# BR2 arm9201 is not set
# BR2 arm9221 is not set
4 BR2 arm926t is not set

/／이하 생략 . . .

' .cont ign 2755 l ines, 55199 characters


다음으로 make을 실행하여 램디스크를 빌드한다.                           이 작업은 램디스크에 포함되는 각종 도구들과
패키지들을 관련 사이트에서 다운로드 하면서 빌드하기 때문에 ］시간정도 소요된다．


$ make

/／빌드 실행 된El (］시간 정노 소요됨 )




빌드가 모두 수행되면 다음과 같이 output八mages/ 경로에 9기p으로 압축된 램디스크 파일이 생
성 된 다．


$ I I output/ images!
total 4060
dr벡xr볘肝出 2 jun（기 J tun（기 ]      4096 Mar 28 16:12 . /
drwxrwxr-x 6 jungjj jungjj      4096 Mar 28 16: 09 . ./
  rw-rw-r-- 1 jungj j jungjj 2317312 Mar 28 16:12 rootfs.ext2
-r川-rw나-- 1 jungjj jungjj 635500 Mar 28 16:12 rootfs.ext2.Uz
-rw-rw-r-- 1 jungj j jungjj 1464320 Mar 28 16:12 rootfs. tar
  rw-rw-r-- 1 jungj j jungjj 633072 Mar 28 16:12 rootfs. tar.gz



이제 위의 램디스크如otfs.ext2.g기을 타겟보드에 올려 보도록 하자.                                먼저 타겟보드의 u-boot에
진입하여 다음과 같이 fastboot을 실행한다．


U-Boot 2012.07-g8c348a3 (Mar 11 2015 - 15: 31 :43) for ARNDALE OCTA

CPU: Exynos5420 Rev2.0 [Samsung SOC on SMP Platform Base on ARM CortexA15]
APLL = 800MHz, KPLL = 600MHz
MPLL = 532MHz, BPLL = 800MHz

Board: ARNOALE OCTA

                                               142 / 312
커 널 연구회（www.kernel.bz)                                                 정재준 (rgt이3307（흐）nate.con昑
Device Tree 상세분석 in Linux kernel 4.0                                            4. Device Tree 실습   143




DRA批 2 GiB
WARNING: Caches not enabled

TrustZone Enabled BSP
BL1 version:

Checking Boot Node . . . SDMMC
NMC:   S5P_NSHC2: 0, S5P_MSHCO: ]
MMC Device 0: 7.5 GiB
MNC Device 1: 7.3 GiB
MMC Device 2: NNC Device 2 not 1 ound
there are pending interrupts Ox( 0000001
In:    serial
Out:   serial
Err:   serial
Net:   No ethernet found.
Hit any key to stop autoboot: (

ARM孤LE # f as比oot
[Partition table on MoviNAND]
ptn 0 name= 'fwb너 ' start=0x3 1 er =N/ A (use hard-coded info. (cmd: movi) )
ptn 1 name= 'b12 ' start=N/ A len=f IA (use hard-coded info. (cmd: movi) )
ptn 2 name= 'boot loader ' start=N A len=N/A (use hard-coded info. (cmd: movi) )
ptn 3 name= 'tzsw ' start=N/ A lenS N/ A (use hard-coded info. (coid: movi) )
ptn 4 name= ' kernel 1 star t=N/ A IE n=N/ A (use hard-coded info. (cmd: movi) )
ptn 5 name= ramdisk ' start=N/ A en=OxO(시27262976KB) (use hard-coded info. (cmd: movi) )
ptn 6 name= 'system ' start=0x3 k n=0x0( -548352000KB)
ptn 7 name= 'userdata ' star t=0x3 I en=0x0( -548352000KB)
ptn 8 name= 'cache start=Ox3 1 er =OxO( -548352000KB)
ptn 9 name= 'fat ' start=0x3 len=( xO(-192491110계KB)
USB cable Connected! [CH-O]


다음으로 우분투 호스트 PC에서 fastboot을 실행하여 램 디스크를 타겟보드에 올린다．


$ ed output/ images/

/／루트 계정으로 실행한다．

$ su root
Password:

# fastboot fla寸｝ ramd治k rootfs. ( 1xt2.gz
sending 나amdisk ' (620 KB) . . .
OKAY [ O. 081s1
writing 'ramdisk ' . . .
OKAY [ O.128s]
finished, total time: O. 209s

# fastboot reboot
rebooting. . .

finished, total time: 0.000s




                                              143 / 312
커 널 연구회（www.kernel.bz)                                                   정재준 汀gbi3307@nate.com
Device Tree 상세분석 in 니flux Kernel 4.0                                            4. Device Ti尸ee 실습       144




타겟보드를 재부팅 하면 다음과 같이 부트로더, 커널. 램디스크가 성공적으로 부팅되면서 사용자
（루트） 로그인 프롬프트가 나타나고, 엔터하면 콘솔에서 명령들을 실행할 수 있다.                                           부팅시간은 약

12초가 소요된다．


U-Boot 2012. 07 (Mar 28 2015 - 15:15:44) for ARNDALE OCTA

CPU: Exynos5420 Rev2.0 [Samsung SOC on SMP Platform Base on ARM CortexA151
APLL = 800MHz, KPLL = 600MHz
MPLL = 532MHz, BPLL = 800MHz

Board: ARNDALE OCTA
DRAM: 2 0汨
WARNING: Caches not enabled

TrustZone Enabled BSP
BL1 version:

Checking Boot Mode . . . SDMMC
MMC:    55P.JSHC2: 0, S5P_MSHCO: 1
MMC Device 0: 3. 7 GiB
MMC Device 1: 7.3 GiB
MMC Device 2: MMC Device 2 not found
there are pending interrupts Ox00000001
In:     serial
Out:    serial
Err:    serial
Net:    No ethernet found.
Hi t any key to stop autoboot: 0
reading kernel . .device 0 Start 1263, Count 10240
MMC read: dev # 0, block # 1263, count 10240 . . . 10240 blocks read: 에
c에）이eted
reading RFS. .device 0 Start 11503, Count 2048
MMC read: dev #0. block #11503, count 2048 . . . 2048 blocks read: OK
comr니eted

Starting kernel . .

1      0.0000001 Booting Linux on physical CPU OxO
[      0.0000001 Linux version 4.0.0 (jungjj@myHome2) (gcc version 4.6. x-google 20120106 (prerelease)
(0CC) ) #1 SMP PREEMPT Sat Apr 18 17:30:18 KST 2015
[      0.000000] CPU: ARMv7 Processor [412fc0f3] revision 3 (ARMv7) , cr=10c5387d
[      0.0000001 CPU: PIPT / VIPT nonal iasing data cache, PIPT instruction cache
[      0.0000001 Machine model : Insignal Arndale Octa evaluation board based on EXYNOSS420
[      0.0000001 cma: Reserved 64 MiB at 0x9b800000
[      0.0000001 Memory pol icy: Data cache wr i teal b c
[      0.0000001 Samsung CPU ID: 0xe5420020
[      0.0000001 Running under secure firmware.
[      0.0000001 PERCPU: Embedded 10 pages/cpu @ee77d000 s11136 r8192 d21632 u40960
[      0.0000001 Bui lt 1 zonel ists in Zone order, mobi l ity grouping on. Total pages: 517136
[      0.000000] Kernel command l ine: console=ttySAC3,115200n8 root=/dev/ ram0 init=/sbin/ init
 ini trd=0x21000000, 28M ramdisk=28672
[      0.000000] P山 hash table entries: 4096 (order: 2, 16384 bytes)
[      0.000000] Dentry cache hash table entries: 131072 (order: 7, 524288 bytes)
[      0.000000] Inode-cache hash table entries: 65536 (order: 6, 262144 bytes)

                                              144 / 312
커 널 연구회（www.kernel.b기                                                     정재준 內bi3307@nate.com)
Device Tree 상세분석 in Linux kernel 4.0                                            4. Device Tree 실奇斗45




[    0.000000] Memory: 1955676K/ 2074624K avai lable (4734K kernel code, 193K rwdata, 1680K rodata,
240K mnit, 275K bss, 53412K reserved, 65536K cma-reserved, 1239040K highmem)
     0.0000001 Virtual kernel memory layout:
     0.0000001      vector : 0xffff0000 - 0xffff1000     (    4 kB)
     0. 0000001     fixmap : 0xffc00000 - oxf ff00000    (3072 kB)
     0. 0000001     vmal loc : Oxf 0000000- 0xff000000   ( 240 MB)
     0. 000000]     lowmem : 0xc0000000 - Oxef 800000    ( 760 MB)
     0.0000001      pkmap     : 0xbfe00000 - 0xc0000000  (    2 MB)
     0.0000001      modules : 0xbf 000000 - 0xbfe00000   ( 14 MB)
     0.0000001         . text : 0xc0008000 - 0xc064bc50  (6416 kB)
     0.0000001         . mnit : 0xc064c000 - 0xc0688000  ( 240 kB)
     0.0000001         .data : 0xc0688000 - 0xc06b8740    ( 194 kB)
     0.000000]           .bss : 0xc06b8740 - 0xc06fd3c0   ( 276 kB)
     0.0000001 SLUB: 배al ign=64, 0rder=0-3, Min0bjects=0, CPUs=8, Nodes=1
     0.000000] Preemptible hierarchical RCU implementation.
     0.000000] Additional per-CPU info printed with stal ls.
     0.000000] NR_ IRQS:16 nr_ irqs:16 16
     0.0000001 GIC physical location is 0x10481000
     0.0000001 L2C: fai led to 1 nit: -19
     0.0000001 Switching to tinier-based delay loop, resolution 4lns
     0. 000006] sched_clock: 32 bits at 24MHz, resolution 4lns, wraps every 178956969942n5
     0.0002861 Console: colour dummy device 80x30
     0.000314] Cal ibrating delay loop (skipped) , value calculated using timer frequency. . 48.00
Bogo씨PS ( 作기＝240000)
[    0.000334] pid_max: default: 32768 minimum: 301
[    0.0004961 Mount-cache hash table entries: 2048 (order: 1, 8192 bytes)
     0.000511] Nountpomnt-cache hash table entries: 2048 (order: 1, 8192 bytes)
     0.001209] CPU: Testing wr ite buffer coherency: Ok
     0.001574] CPUO: update cpu_capacity 1535
     0.001588] CPUO: thread -1, cpu 0, socket 0, 畔idr 80000000
     0.0017621 Setting up static identity map for 0x2047db28 - 0x2047db80
     0.081328] CPU1: update cpu_capacity 1535
     0.081336] CPU1: thread -1, cpu 1, socket 0, 때idr 80000001
     0.1013341 CPU2: update cpu_capacity 1535
     0.1013411 CPtJ2: thread -1, cpu 2, socket 0, mpidr 80000002
     0.1213261 CPU3: update cpu capacity 1535                  ,
     0.121334] CPU3: thread -1 , cpu 3, socket 0, rnpidr 80000003
     2.140016] CPU4: fai led to come onl ine
     4.160032] CPU5: fai led to come onl ine
     6.180049] CR16: fai led to come onl ine
     8.2000651 CPU7: fai led to come onl ine
     8.200100] Brought up 4 CPUs
     8.2001131 SMP: Total of 4 processors activated (192.00 BogoMIPS) .
     8.200123] CPU: Al l CPU(s) started in SVC mode.
     8.200826] devtmpfs: initial ized        '
     8.203076] VFP support vo. 3: implementor 41 architecture 4 part 30 variant f rev 0
     8.205367] pinctrl core: initial ized pinetrl subsystem
     8.228525] NET: Registered protocol fami ly 16
     8.230126] DMA: preal located 256 KiB pool for atomic coherent al locations
     8.2429231 exynos-audss-cl k 3810000.audss-clock-control ler: setup completed
     8.250988] EXYNOSS420 PMU initial ized
     8.304656] SCSI subsystem in 'tial ized
     8.305425] usbcore: registered new interface driver usbfs
     8.305590] usbcore: registered new interface driver hub
     8.305875] usbcore: registered new device driver usb
     8.307966] Advanced Linux Sound Archi tecture Driver Initial ized.

                                              145 /312
커 널 연구회（www.kernel.b기                                                    정재준 岫bi3307@nate.com)
Device Tree 상세분석 in 나flux Kernel 4.0                                                        4. Device Tree 실습        ]46




     8.309234] Switched to clocksource rnct- frc
     8.333815] NET: Registered protocol fami ly 2
     8.3346111 TCP establ ished hash table entries: 8192 (order: 3, 32768 bytes)
     8.334724] TCP bind hash table entries: 8192 (order: 5, 163840 bytes)
     8.334925] TCP: Hash tables configured (establ ished 8192 bind 8192)
     8.334983] TCP: reno registered
     8.3350031 UDP hash table entries: 512 (order: 2, 24576 bytes)
     8.3350531 UDP-Lite hash table entries: 512 (order: 2, 24576 bytes)
     8.335329] NET: Registered protocol fami ly 1
     8.3356381 Trying to unpack rootfs image as initramfs. . .
     8.336274] rootfs image is not initramfs (no cpio magic) ; looks l ike an initrd
     8.4277201 Freeing initrd memory: 28672K (c1000000 - c2c00000)
     8.430800] tutex hash table entries: 2048 (order: 5, 131072 bytes)
     8.451253] romfs: RO肝S MID (C) 2007 Red Hat, Inc.
     8.4523181 bounce: pool size: 64 pages
     8.452336] io scheduler noop registered
     8. 452353] io scheduler deadl ine registered
     8.4530041 io scheduler cfq registered (default)
     8. 4538521 exynos-mipi-video-phy 10040714. video-phy: regmap lookup fai led: -19
     8.4538761 exynos-mipi-video-phy 10040714. video-phy: can 't request region for resource Emem
0x10040714-0x1004071 f I
[    8.4539041 exynos-mipi-video-phy: probe of 10040714. video-phy fai led with error -16
[    8.455334] 12100000.phy supply vbus not found, using dummy regulator
[
     8. 4554161 12100000.phy supply vbus-boost not found, using dummy regulator
r
L [
     8.4559571 12500000.phy supply vbus not found, using dummy regulator
     8.456032] 12500000. phy supply vbus-boost not found, using dummy regulator
r
1
L [
     8. 460931] dma-p1330 3880000.adma: Loaded driver for PL330 DMAC-241330
     8.4609491 dma-p 1330 3880000. adma: DBIJFF-4x8bytes Num_Chans-6 Num_Per i -16 Num_Events-6
[
     8.4666421 dma-p1330 121a0000.pdrna: Loaded driver for PL330 몌AC-241330
[
     8.466659] dma-p 1330 121a0000 .pdma:         DBUFF-32x4bytes Num_Chans-8 Num_Per i -32 Num_Events-
n
亡
Q
U [
             8.472435] dma-p 1330 121b0000 . pdma: Loaded dr i ver for PL330 DMAC-241330
[
             8. 472452] dma-p1330 121b0000.pdma:           DBlJFF-32x4bytes Num_Chans-8 Nuni. .Peri-32 Num_Events-
n
/
Q
U [
             8.474073] dma-p1330 10800000.mdma: Loaded driver for PL330 DMAC-241330
[
             8. 474089] dma-p1330 10800000.mdma: .        DBtJFF-64x8bytes Num_Chans-8 Num_Peri-1 Num_Events-32
[
             8.592294] Serial : 8250/16550 driver, 4 ports, IRQ sharing disabled
[
             8. 594750] 12c00000. serial : ttySAC0 at MM山 0x12c00000 ( irq = 58, base_baud = 0) is a 53C6400/10
[
             8.595367] 12c10000. serial : ttySAC1 at MMI0 0x12c10000 ( irq = 59, base_baud = 0) is a 53C6400/10


r
1
L r
  L [
             8.595983] 12c20000. serial : ttySAC2 at MMI0 0x12c20000 ( irq = 60, base_baud = 0) is a 53C6400/10
             8.596593] 12c30000. serial : ttySAC3 at MM山 0x12c30000 ( irq = 61, base_baud = 0) is a S3C6400/10
             9.2400331 console [ttySAC3] enabled
[
             9.245341] Idrm] Initial ized drm 1.1. 0 20060810
[
             9.264655] brd: module loaded
[

[
             9.275389] loop: module loaded
             9. 278242] usbcore: registered new interface driver asix
[
             9.282555] usbcore: registered new interface driver ax88179_178a



r
1
11 rL rL [
             9.288581] usbcore: registered new interface driver cdc_ether
             9.2944491 usbcore: registered new interface driver 5msc75xx
             9.300193] usbcore: registered new interface driver 5msc95xx
             9.305824] usbcore: registered new interface driver net1080
[
             9.311488] usbcore: registered new interface driver cdc_subset
[
             9.317355] usbcore: registered new interface driver zaurus
[
             9. 322978] usbcore: registered new interface driver cdc_ncm

rL r[
             9.329426] usb@12000000 supply vdd33 not found, using dummy regulator
             9.3350111 usb@12000000 supply vddl0 not found, using dummy regulator

                                                        146/ 312
커 널 연구회（www.kerr祀I.bz)                                                              정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                           4. Device Tree 실습      ]47




[    9.7450461 usb@12400000 supply vdd33 not found, using dummy regulator
[    9.750198] usb@12400000 supply vddl0 not found, using dummy regulator
[   10.158361] xhci-hcd xhci-hcd.2.auto: xHCl Host Control ler
[   10.162434] xhci-hcd xhci-hc( .2.auto: new IJSB bus registered, assigned bus number 1
[   10.170369] xhci-hcd xhci-hccL2.auto: hcc parains 0x0220f04c hci version 0x100 quirks 0x00010010
[   10.178722] xhci-hcd xhci-hcd.2. auto: irq 108, io mem 0x12000000
[   10.184893] usb usbi: New IJSB device found, idVendor=ld6b, idProduct=0002
[   10.1914301 usb usbi: New IJSB device strings: Mfr=3, Product=2, SerialNumber=1
[   10.198590] usb usbi: Product: xHCl Host Control ler
[   10.2034711 usb usbi: Manufacturer: Linux 4. 0.0 xhci-hcd
[   10.2087271 usb usbi: SerialNumber: xhci-hcd.2.auto
[   10.214621] hub 1-0:1.0: USB hub found
[   10.2173421 hub 卜0:1.0: 1 pdrt detected
[   10.2218271 xhci巾hcd xhci-hccL2. auto: xHCl Host Control ler
[   10.2266861 xhci-hcd xhci-hcd. 2. auto: new USB bus registered, assigned bus number 2
[   10. 234584] usb usb2: New USB device found, idVendor=ld6b, idProduct=0003
[   10.2410821 usb usb2: New USB device strings: Mfr=3, Product=2, SerialNumber=1
[   10.248242] usb usb2: Product: xHCl Host Control ler
1   10.253124] usb usb2: Manufacturer: Linux 4.0. 0 xhci-hcd
[   10.258380] usb usb2: SerialNuinber: xhci-hcd.2.auto
1   10.264224] hub 2-0:1.0: USB hub found
[   10.266992] hub 2-0:1.0: 1 port detected
[   10.271560] xhci-hcd xhci-hcd.5. auto: xHCl Host Control ler
1   10.276347] xhci-hcd xhci-hcd.5.auto: new USB bus registered, assigned bus number 3
[   10.2843351 xhci-hcd xhci-hcd.5. auto: hcc params 0x0220f04c hci version 0x100 quirks 0x00010010
[   10.2927071 xhci-hcd xhci-hcd.5.auto: irq 109, io mem 0x12400000
[   10.298791] usb usb3: New USB device found, idVendor=ld6b, idProduct=0002
[   10.305382] usb usb3: New USB device strings: Mfr=3, Product=2, SerialNumber=1
[   10.312569] usb usb3: Product: xHCl Host Control ler
[   10.317391] usb usb3: Manufacturer: Linux 4.0.0 xhci-hcd
[   10.322830] usb usb3: SerialNumber: xhci-hcd.5.auto
[   10.3284751 hub 3-0:1.0: USB hub found
[   10.3313231 hub 3-0:1.0: 1 port detected
[   10.3357381 xhci-hcd xhci-hcd.5.auto: xHCl Host Control ler
[   10.340669] xhci-hcd xhci-hcd. 5.auto: new USB bus registered, assigned bus number 4
1   10.348492] usb usb4: New USB device found, idVendor=ld6b, idProduct=0003
[   10.355032] usb usb4: New USB device strings: Mfr=3, Product=2, SerialNumber=1
[   10.362223] usb usb4: Product: xHCl Host Control ler
[   10.3670451 usb usb4: Manufacturer: Linux 4.0.0 xhci-hcd
[   10.3725161 usb usb4: SerialNuniber: xhci-hcd.5.auto
[   10.378152] hub 4-0:1.0: USB hub found
[   10.380974] hub 4-0:1.0: 1 port detected
1   10.385470] ehci_hcd: USB 2. 0 'Enhanced ' Host Control ler (EHCl) Driver
[   10.3913481 ehci-exynos: EHCI EXYNOS driver
[   10.395919] exynos-ehci 12110000.usb: EHCI Host Control ler
[   10.4009901 exynos-ehci 1211어）00.usb: new USB bus registered, assigned bus number 5
[   10. 4087671 exynos-ehci 12110000.usb: irq 107, io mem 0x12110000
[   10. 429396] exynos-ehci 12110000.usb: USB 2.0 started, EHCI 1.00
[   10.434122] usb usb5: New USB device found, idVendor=ld6b, idProduct=0002
[   10.440709] usb usb5: New USB device strings: Mfr=3, Product=2, SerialNumber=1
[   10.447867] usb usb5: Product,: EHCI Host Control ler
[   10.452750] usb usb5: Manufacturer: Linux 4.0.0 ehci_hcd
[   10.458005] usb usb5: SerialNumber: 12110000. usb
[   10.463579] hub 5-0:1.0: USB hub found
[   10.466358] hub 5-0:1.0: 3 ports detected
[   10.471373] ohci_hcd: USB 1.1 'Open ' Host Control ler (0HCl) Driver

                                             147 / 312
커 널 연구회（ww比kern이b기                                                     정재준 (r야)i3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                           4. Device Tree 실습        ]48




    10.4764851 ohci-exynos: 0HCl EXYNOS driver
    10.4811011 exynos-ohci 12120000.usb: USB Host Control ler
    10.4860261 exynos-ohci 12120000.usb: new USB bus registered, assigned bus number 6
    10.4937941 exynos-ohci 12120000.usb: irq 107, io mem 0x12120000
    10.563508] usb usb6: New USE device found, idVendor=ld6b, idProduct=0001
    10.568812] usb usb6: New USE device strings: Mfr=3, Product=2, SerialNumber=1
    10.5761891 usb usb6: Product: USE Host Control ler
    10.580797] usb usb6: Manufacturer: Linux 4.0. 0 ohci_hcd
    10.586054] usb usb6: SerialNumber: 12120000.usb
    10.5916221 hub 6-0:1.0: USB hub found
    10.594406] hub 6-0:1.0: 3 ports detected
    10.599538] usbcore: registered new interface driver usb-storage
    10.6051421 mousedev: PS/2 mouse device common for al l mice
    10.611174] s3c-rtc 101e0000. rtc: fai led to find rtc source clock
    10.6159751 53c-rtc: probe of 101e0000. rtc fai led with error -2
    10.622269] i2c /dev entries driver
    10.660884] PVDD_MlFS_1V1: ramp_delay not set
    10.6711151 PVDD_G3DS_1V0: ramp_delay not set
    10.7078621 thermal thermal_zoneo: fai led to read out thermal zone (-22)
    10.7131511 10060000. tmu supply vtmu not found, using dummy regulator
    10.7198811 thermal thermal_zonel: fai led to read out thermal zone (-22)
    10. 7261921 10064000. tmu supply vtmu not found, using dummy regulator
    10.732963] thermal therma匕zone2: fai led to read out thermal zone (-22)
    10.7393091 10068000. tmu supply vtmu not found, using dummy regulator
    10.746046] thermal therma匕zone3: fai led to read out thermal zone (-22)
    10.752387] 1006c000. tmu supply vtmu not found, using dummy regulator
    10.7591571 thermal thermal_zone4: fai led to read out thermal zone (-22)
    10.7654731 100a0000. tmu supply vtmu not found, using dummy regulator
    10.773114] 53c2410-wdt lold0000.watchdog: watchdog inactive, reset disabled, irq disabled
    10.7808971 device-mapper: ioctl : 4.30.0- ioctl (2014-12-22) initial ised: dm-devel@redhat.com
    10.788477] Driver 'mrncblk needs updating - please use bus_ type methods
    10.795231] usb 5-1: new high-speed USE device number 2 using exynos-ehci
    10. 802011] sdhci : Secure Digi tal Host Control ler Interface driver
    10.8080861 sdhci : Copyright (c) Pierre 0ssman
    10.812663] Synopsys Designware Multimedia Card Interface Driver
    10.8190551 dwmmc_exynos 12200000.mmc: num-slots property not found, assuming 1 slot is avai lable
    10.827309] dwmmcexynos 12200000.mmc: IDMAC supports 32-bit address mode.
    10.8341741 dwmmc_exynos 12200000.mmc: Using internal DMA control ler.
    10.840494] dwmmc_exynos 12200000.mmc: Version ID is 250a
    10.8458891 dwmmc_exynos 12200000. mmc: DW MMC control ler at irq 87, 64 bit host data width, 64
deep fifo
[ 10.8559851 dwmmc_exynos 12200000.mmc: No vqmmc regulator found
[ 10.899349] dwmmc_exynos 12200000. mmc: 1 slots initial ized
[ 10.9036621 dwinmc_exynos 12220000.mmc: num-slots property not found, assuming 1 slot is avai lable
    10.9124061 dwrnmc_exynos 12220000. mmc: IDMAC supports 32-bit address mode.
    10.9191701 dwmmc_exynos 12220000. nimc: Using internal DMA control ler.
    10.9255281 dwmmcHexynos 12220000.mmc: Version ID is 250a
    10.9309551 dwmmcexynos 12220000.mmc: OW MMC control ler at irq 88, 64 bit host data width, 64
deep fifo
    10.961109] usb 5-1: New USE device found, idVendor=05e3, idProduct=0610
    10.966330] usb 5-1: New USE device strings: Mfr=0, Product 1, SerialNumber=0
    10.973474] usb 5-1: Product: USB2.0 Hub
    10.9785321 hub 5-1:1.0: USE hub found
    10.9814821 hub 5-1:1.0: 4 ports detected
    10.982289] mmco: MAN_BKOPS_EN bit is not set
    10.983037] mmc_host mmco: Bus speed (slot 0) = 50000000Hz (slot req 52000000Hz, actual

                                             148 / 312
커 널 연구회佃＼사小,'. kernel.b기                                               정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 나flux IerneI 4.0                                            4. Device Tree 실습         149




50000000HZ div = 0)
[    10.9835101 mmc_host mmco: Bus speed (slot 0) = 100000000Hz (slot req 52000000Hz, actua
50000000HZ div = 1)
     10.9836931 mmc0: new DDR MMC C:ard at address 0001
     10.9849701 m1ncb1k0: mmc0: 0001 M8G1WA 7.28 GiB
     10.9852341 mmcblk0boot0: mecO: 0001 M8G1WA partition 1 2.00 MiB
     10.9855101 mmcblk0bootl: mmco: 0001 N8G1卄A 口artit ion 2 2. 00 씨B
     10.9857701 mmcblkOrpmb: mmco: C1001 M8G1WA partition 3 128 KiB
     10.989444] dwmmc_exynos 12220(I00.mmc: 1 slots initial ized
     10.991266] mmcblko: p1 p2 p3 p4
     10.9966961 usbcore: registereci new interface driver usbhid
     恤9967071 usbhid: USB HID cor'e driver
     11.0082771 TCP: cubic register'ed
     11.0083051 NET: Registered pr()tocol fami ly 17
     11.0084291 NET: Registered pr ()tocol fami ly 15
     11.0090331 Registering S卄P'S朴)B emulation handler
     11.013586] power-巾main: Po너er'-off latency exceeded, new value 380250 ns
     11.013846] Pa나er너에떼n: Po나er'-off latency exceeded, new value 230375 ns
     11.0138781 Pa川er- 加main: Po따er -off latency exceeded, new value 354333 ns
     11.0142811 Pa벼er小（拍main: Po베er -off latency exceeded, new value 374917 ns
     11.0143221 P0나er-的main: Pa뱌ei -off latency exceeded, new value 377125 ns
     11 .0161711 input: gpio_keys ar3 /devices/platform/gpio_keys/ input/ inputo
1    11.0177611 dr ivers/rtc/hctosyrs.c: unable to open rtc device (ricO)
[    11.048669] mmc_host mmcl: Bus 5口eed （引아 0) = 50000000Hz （引at req 50000000Hz, actual
50000000HZ div = 0)
[    11.0488141 mmcl: new high spew d SDHC card at address b368
[    11.050168] mmcblkl: mmcl :b3681          3.71 GiB
[    11 .0528471 rnmcblkl: p1 p2 p3 口4
[    11.121413] PVDD G3D ivo: disat기 i ng
[    11.127247] PVDD G3DS 1V0: disr北니 I ng
[    11.130350] random: nonblockint그 口aol is initial ized
[    11.1331251 PVDD HSIC 1V8: disr北I i ng
[    11.134721] PVDD_ABB_1V8: di sat키 ing
 [   11.136305] PVDD ANA下 1V8: di r3ab I i ng
 [   11.137888] PVDD_ANA나）_1V0: di r3abl 나）g
 [   11.139475] PVDD ADC 1V8: disat키 ing
 [   11.141064] PVDD API0 1V8: disrabl ing
 [   11.1474301 ALSA device l ist:
1    11.147438]    No soundcards fo
[    11.183047] RA吐I斗；: qZ巾 im叩e found at block 0
[    11.259663] yES: Mounted root I:ext2 f i lesystem) readonly on device 1:0.
[    11.264918] devtmpfs: mounted
[    11 .2679581 Freeing unused kerr]eI memory: 240K (c064c000 - c0688000)
Starting togging: OK
 Initial izing random number genera1tor . . . done.
Starting network. . .

Welcome to Exynos5420
Exynos5420 login: [    11 .459626] usb 5-1.4: new high-speed USB device number 3 using exynos-ehc i
    11.5707511 usb 5-1.4: New USB device found, idVendor=0b95, idProduct=772a
    11 .5761461 usb 5-1.4: New USB device strings: Mfr=l, Product=2, SerialNumber=3
    11.5834671 usb 5-1.4: Product: AX88772
    11 .5873221 usb 5-1.4: Manufacturer: ASIX Elec. Corp.
    11.5923891 usb 5-1.4: SerialNumber: 000001
    11.5988651 asix 5-1.4:1.0 (unnamed net_device) (uninitial ized) : inval id hw address, using random
    12.423901] asix 5-1.4:1.0 ethO register 'asix ' at usb-12110000.usb-1.4, ASIX AX88772 1lSB 2.0

                                              149/ 312
커 널 연구회（www.kerrrel.b기                                                   정쟤준 (rgb日307@nate.com)
Device Tree 상세분석 a) 니flux Kerr倒 4.0                                           4. Device Tree 실습   ]50




Ethernet, 96:5e: 48: d5:bc:51

Welconie to Exynos5420
Exynos5420 login: root
Password:

# uname -a
Linux Exynos5420 4.0.0 #1 SMP PREEMPT Sat Apr 18 17:30:18 KST 2015 armv71 GNU/Linux




                                              150 / 312
커널연구회（ww比kern이b기                                                       정재준 內bi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                                     4. Device Tree 실습   151




4.4 커널 부팅 소스 분석

시스템이 부팅될 때 리눅스 커널은 泊町mairi.c 소스의 start_kernel() 함수에서 각종 시스템 자원들
을 초기화 한댜.           아래는 이 함수의 실행 흐름을 블록 다이어그램으로 정리한 것이다．



startmkernel() 실헹 흐吾


                                 II기t/m키ftC

                                 start_kernel()




    arch/arm/kerneVsetup.c                           1nit/main.c
    setup_archO                                      rest_initO




                                   1ait/main.c
                                                    /               \      init/main.c
                                    kernel_thread(kernel_init)             kernel_thread(kthreadd)



                                                    1二，
                  iriit/main.c                             In仕in沼in.c

                  kernel m itmfreeable()                   run_initmprocess()




start_kernel() 함수에서 하는 역할은 크게 2가지로 구분된다.                                첫째는 setup_카ch(）에서 시스템（cPu,
메모리, 인터럽트） 자원들을 설정하고 두번째는 rest_in仕0에서 시스템에 장착되어 있는 각종 장치
들을 설정한다．            rest_init() 함수는 커널 쓰레드 pid가 ］번인 kernel in仕 쓰레드와 pid가 2번인
kthreadd 쓰레드를 생성한다． 각종 디바이스 드라이버들은 kernel_init() 쓰레드 함수에서 초기화
된다．


kernel_init() 쓰레드 함수는 다시 kernel_in仕 freeable() 함수를 호출하는데, 아래는 이 함수의 실행
흐름을 블록 다이어그램으로 표현한 것이다．



kernel m it卄freeable() 실행 흐륭



                                                    151 / 312
커널연구회（www.kernel.bz)                                                            정재준 (r야키3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                  4. Device Tree 실습   ] 52




                             H] 4/1ndjfl C

                             kernel_initjreeable()




         init/main.c                                 sys_openC/dev/console")
         do_basic_setup()                            ramdisk execute command =




     汨itJmain.c
     （幻in社ca小0
       如in作call_levelO
         do_one_initcall()




위에서 （如initc체（) 함수들은 /II기t/main.c 소스 파일에 다음과 같이 정의되어 있다．



如initcall () 함수듈 소스

extern 1 ni tcal I_ t + in1 tcal 1_startt 1;
extern initcal l_ t __initcal lO寸start[ ];
extern m i tcal l_ t _initcal I1_start[ ];
extern initcal l_ t __initcal l2_startE] ;
extern initcalLt _1n1tca113_start[ j;
extern initcal匕t _1n1tca114_start[ 1;
extern initcal l_ t _initcal l5_start[ 1;
extern initcal l_ t _initcal l6_start[ ];
extern initcal l_ t _1n냐ca1 17_start[ I;
extern initcal l_ t _initcal匕end[ I;

static initcal l_ t *initcal l levels[ ] _initdata = {
         _initcal 10_start,
            initcal li_start,
         _initcal l2_start,
            initcal 13_start,
            initcal 14_start,
            initcal 15_start,
         H+in itca I 16_start 1
            initcal l7_start,
            initcal I_end,
};
/出 Keep these in sync with initcal ls in inc山de/ I inux/ init.h */
static char *jnjtcal ! level names[ ] _initdata = {

                                                      152 / 312
커널연구회佃ww.kern이.b기                                                                정재준 (rgb日307@nate.com)
Device Tree 상세분석 in 니nux Kernel 4.0                                                       4. Device Tree 실습   153




          'ear ly ",
          ncore           '   ,


            'postcore " ,
          "arch           '   ,


           'subsys",
          냐S”         ,


          "device",
          ' late ' ,
};
stat ic void _init d工initcal l_IE vel ( mnt level)
{
                  nitcal l t *fn;

          strcpy( initcal I_command l ine, saved_command_ l ine) ;
          parse_args( initcal i_ levi '匕namesl level 1 ,
                        nitcal l cor mand그 I ne , 나star匕H口aram,
                       寸St야＝_pai am - __start寸mparam,
                       level , leve
                       &repai r_env str ing) ;

            tor (fn = ini tcal l_ leve sE level ] ; fn< inifcal l_ levels[ level+1] ; fn++)
                     do one initcal ( 火fn) ;
 }
stat ic void _ini t do_ initcal ls(i 이 d)
{
                  mnt level ;

             for ( level = 0; level < ARRAY_SIZE( initcal I_ levels) -1; level++)
                       do ini tcal l lei el ( level ) ;
 }



In仕call_levels는 initcall_t 타입의 함수 포인터 배열이댜.                          배열의 요소 개수는 H in仕c키10_start에서
小initc키i_end까지 9개이다.                이 배열의 인덱스 순번인 0에서 9까지가 化r 반복문의 제어변수 level
이 되어 （幻_initc訓1ev이（) 함수를 순차적으로 호출한다.                                  do_initcall_lev이（) 함수에 전달된 level에
따라서 do_one_initcaii(）에 initcail 함수 포인터 ' fn이 전달되어 순서대로 실행되는 구조이다．


Lev이은 "early", 'coro" , "postcore ' , 'ar아寸 , "subsys " , 냐s" , "device " , 니ate' 순으로 정해지며
이것은 기nciude/linux/init.h 헤더 파일에 정의되어 있는 아래의 매크로 함수 호출을 통하여
결정된다．



k啼Lca靴r 4크三 斗수*
#def ine_ def ine_ ini tcal l (tn, id) Y
         stat ic ini tcal l t     initc il l 倂打n＃쒸d usedW
         _attr ibute_( (_ sect ion ( 「 , ru tcal I '' #id ' . H] i t ") )) = fn; W
         LTO_REFERENCE_ IN I TCALL(      nit cal 匕＃#f n料 뗘）

                                                     153 / 312
커 널 연구회（www.kerneLbz)                                                                정재준 （呼)13307@nate.com)
Device Tree 상세분석 in 口flux Kernel 4.0                                                          4. Device Tree 실습    154




／火
           * Early initcal ls run before initial izing SMP.

           士Only for bui lt- in code, not modules.
           火／
#dof ineearly_ initcal l (fn)                      _define_ initcal l (fn, early)



           * A "pure " inhtcal l has no dependencies on anything else, and purely
           * ini tial izes variables that couldn 't be statical ly ini tial ized.

           * This only exists for bui l t- in code, not for modules.
           士 Keep main.c: initcal l level narnes[ ] in sync.
           六／
#define pure_ initcal l (fn)                                _define_ initcal l (fn, 0)

#define core_ initcal l (fn)                                  define_ initcal l (fn, 1)
#def mne core_ mni teal l_sync(fn)                          _define_ initcal l(fn, is)
#define postcore_ initcal l (fn)                            _define_ initcal l (fn, 2)
#define postcore_initcal l_sync(fn)                           define_ initcal l (fn, 2s)
#define areh_initcal l (fn)                                 _define_ initcal l (fn, 3)
#define arch_ initcal l_sync(fn)                            _define_initcal l (fn, 3s)
#define subsys_mnitcal l (fn)                               _define_ initcal l (fn, 4)
#def m e subsys_ ini teal I_sync( fn)                       _define_ initcal l (fn, 4s)
#defino fs_ initcal l (fn)                                  _define_ initcal l (fn, 5)
#def i ne fs_ initcal I_sync(fn)                            _define_ initcal l (fn, 5s)
#define rootfs_ initcal l (tn)                              _definejn냐cal 1 (tn, rootfs)
#define device_ initcal l (fn)                              _卞detine_ initcal l (fn, 6)
#define device_initcal l_sync(fn)                           _define_ initcal l (fn, 6s)
#define latejnitcal l (fn)                                  _define_initcal l (fn, 7)
#define late_ initcal l_sync(fn)                            _definejnitcal l (fn, 7s)

#define __initcal l (fn)                                    device_ initcal l (fn)



#define _exitcal l (fn) W
         static exitcal I_ f _exitcal l_##fn _exit_cal l = fn

(（중간 생략）)


     ／火士
            * module. Jnit () - driver initial izat ion entry point
            古 自）x: function to be run at kernel boot time or module insertion

            火 module in나（) 붜i l l 이 ther be cal led during 血Jnitcal IsO ( if
            * bui ltin) or at module insert ion time ( if a module) . There can only
            * be one per module.
                士／
#define module_init (x)                  _initcal l (x) ;

     !／士士


                * module_exit () - driver exi t entry point
                * @x: function to be run when driver is removed


                                                             154 / 312
커 널 연구회（ww比kern이.b기                                                                      정재준 (rgbi3307@nate.com)
Device Tree 상세분석 ir) 니flux Kernel 4.0                               4. Device Tree 실습    155




 六 module_exit ( ) wi H 胄ra口 the driver 이ean-u口 code
 火 with 이eanu口module( ) 빛hen used 邪 th rmmod when
 * the driver is a module. If the driver is stat ical ly
 * compi led into the kernel , module_exit () has no effect.
 tThere can only be one per module.

#det ine module_exit (x)      exitcal l (x) ;




디바이스 드라이버가 처음으로 초기화 되는 함수는 위의 initcall 매크로 함수들에 의해서 커널이
빌드될 때 함수 포인터로 등록된다.                        커널을 빌드하게 되면 최상위 빌드경로에 System.map 파일
이 생성되는데 이 파일의 내용을 보면 initcall 함수들이 아래와 같이 생성되어 있음을 확인할 수
있다．



$）唇tem.map 파읾의 initcati 함수듈
c068ec40 T   initcal l start
c068ec40 T _se山m帥d
c068ec中1 t _.initcal l_ init_static_ idniapear ly
c068ec48 t __initcal l_exynos_mcpm_ initear ly
c068ec4c t _initcal l_spawn_ksoft irqdearly
c068ec50 t _jnitcaI匕ini tworkqueuesear ly
c068ec54 t _initcal 1_migration_ initear ly
c068ec58 t _initcal 匕check_cpu_stal匕initear ly
c068ec5c t _initcalLrc山印帥n卯_kthreadear ly
c068ec60 t _ini tcal匕cpu_stop_ in ' tear ly
c068ec64 t _initcal 匕cci_ initear y
c068ec68 t   ini tcal I_ rand_ initial izeear ly
c068ec6c t _initcalLdummy_ timer_registerearly

c068ec70 T  initcal lO start
c068ec70 t 그ni tcal 니pc_ns_ initO
c068ec74 t  ini tcaI 나nit_mmap_min_addrO
c068ec78 t  ini tcal I net ns initO

c068ec7c T   ini tcai ll start
c068ec7c t H ini tcal l_vfp_ initl
c068ec80 t 小m i tcal匕ptrace巾re訊In ' ti
c068ec84 t _ini tcal 匕v6긔朗叩age_ in i ll
c068ec88 t _ini 比al 匕cp比hoH키ug 口m町nc_ in ill
c068ec8c t    ni tcal I_al Ioc_ frozen_cpusl
c068ec90 t JnitcaI 匕wq_sysfs_ init1
c068ec94 t _initcal 匕ksysfs_ ini tl
c068ec98 t __ini tcal I_pm_ mni ti
c068ec9c t _ini tcal匕init_ j i tf ies_clocksourcel
c068eca0 t _mnitcal 匕cgroup_wq_ initl
c068eca4 t 十initcal 匕cpu_pm그niti
c068eca8 t _initcal l_ init_zero_pfnl
c0680cac t   initcal I cma mni t reserved areasi
c068ecb0 t _mnitcal匕fsnot ify_ initl
c068ecb4 t   initcal I fi lelock initi
c068ecb8 t _initcal匕init_scr 나）t_bmnfmtl


                                                155 / 312
커 널 연구회（www.kern飢b기                                            정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                              4. Device Tree 실습    ]56




c068ecbc t _initcal l_ init_elf_binfmtl
c068ecc0 t _ini teal I_debuQfs_ ini ti
c068ecc4 t _initcal匕securityts_initi
c068ecc8 t _initcal l_prandorn_ ini tl
c068eccc t _ini 比a!匕cc匕이카form_ in iti
c068ecd0 t _initcal l_pinctr 나nitl
c068ecd4 t __initcal匕regulator_initi
c068ecd8 t   initcal l of initi
c068ec（把 t 1 in나cal 1_exynos크udss_c比_initl
c068ece0 t   initcal l sock initi
c068ece4 t _ini teal I_net_ mnuse_ mni ti
c068ece8 t __initcal I_net I ink_proto_initi

c068ecec I    initcal l2 start
c068ecec t _initcal匕카om i乙P00匕ni t2
c068ecf0 t _initeal匕exynos_ 加u_ init2
c068ecf4 t    initcal l bdi class init2
c068ecf8 t __initcal 나m_sysfs_ init2
c068ecfc t _ini teal l_kobject_uevent_ ini t2
c068ed00 t 中－ initcal l_samsung괴nctr匕dry_re이計er2
c068ed04 t    mni teal I led class mni t2
c068ed08 t _ini teal I_back! ight_class_ ini t2
c068ed0c t    in i tea1 l amba in i t2
c068ed伯 t _initcal l_tty_이的s_ mni t2
c068ed14 t _initcal l_vtconsole_class_ init2
c068ed18 t    initcal l iommu dev init2
c068ed1c t __initcalL州ake叩j아卄ces뗘ebugfs_init2
c068ed20 t __initcal l_regmap_ initcal l2
c068ed24 t    initcal l sram init2
c068ed28 t __initcal匕syscon_ init2
c068ed2c t _initcal匕spi_ init2
c068ed30 t    initcal l i2c init2

c068ed34 I   initcal l3 start
e068ed34 t __initcal匕gate_vma_init3
c068ed38 t   initcal l customize machine3
c068ed3c t _initcal l_exceptions_ init3
c068ed40 t _initcal匕exynos4_pm_ i n i 냐）0나er面ma i n3
c068ed44 t   initcal l s3c arch init3
c068ed48 t _initcal l_dma_bus_ in1t3
c068ed4e t   initcal l dma channel table init3
c068ed50 t _initcal l_ iommu_ init3

c068ed54 T __initcal 14_start
c068ed54 t _initcal l_ topolo아_init4
c068ed58 t   initcal l uid cache init4
c068ed5c t _initcal匕param_sysfs_ in1t4
c068ed60 t _initcalL珉sysrq_init4
c068ed64 t _initcal匕hung_task_ init4
c068ed68 t   initcal l default bdi init4
c068ed6c t _in나cal l 口ercpu_ena비已async4
c068ed70 t   initcal l_ init_reserve_notifier4
c068ed74 t   initcal l_ init_admin_reserve4
c068ed78 t   initcal l mnit user reserve4
c068ed7c t _initcal匕crypto_wq_ init4
c068ed80 t _initcal匕cry口的mgr_ init4

                                                 156 / 312
커 널 연구회（www.kern이.b기                                         정재준 (rgbi3307@nate.con吩
Device Tree 상세분석 in 니nux Kernel 4.0                         4. Device Tree 실습    157




c068ed84 t _inhtcal l_ iniLbio4
c068ed88 t 1 initcat I_b 나；_settinQs_ init4
c068ed8c t    initcal l bik oc ini t4
c068ed90 t _initcal匕blk_softirq_ in1t4
c068ed94 t _initcal 匕b나；_iopol 匕setu口4
c068ed98 t _initcal匕blkjnqin1t4
c068ed9c t _initcal l_genhd_device_ init4
c068eda0 t _initcaI I_gpioI ibdebugfs_init4
c068eda4 I _ini tcal l_pw町debugfs_ ini t4
c068eda8 t 卞m i tcal匕pw町테針s_ init4
c068edac t    initcal l tbmem init4
c068edb0 I _initcal Lregulator_f! ixedv이tageJn1t4
c068edb4 t _initcal匕gpio_r的띠카아_ 1n1t4
c068edb8 t _initcal _max14577_regulator_ init4
c068edbc I _initcal匕max8997pmic_ in냐4
c068edc0 t _initcal l_max77686巾micjnit4
c068edc4 t _initcal I_s2mpslljmic_ init4
c068edc8 t _initcal l_s5m8767. pmic_1nit4
c068edcc t _initcal _tps65090_regulator_ init4
c068edd0 t    initcal l misc init4
c068edd4 t _initcal l_ tpm_1nit4
c068edd8 t _initcal I_exynos_ iommu init4
c068eddc t    initcal l max14577 i2c 1nit4
c068ede0 t _initcal I_max77686_ i2cjnit4
c068ede4 t _initcal l_max77693J2c_ init4
c068ede8 t     initcal l max8997 i2c 1nit4
c068edec t _initcal匕tps65090_init4
c068edf0 t _initcal匕sec_pmic_ init4
c068edf4 t     initcal l dma but ini t4
c068edf8 t _initcal l_ init_scsi4
c068edfc t _initcalLphy_ init4
c068ee00 t     initcaN usb 1n1t4
c068ee04 t     initcaH usb udc ini t4
c068ee08 t     initcat i serio init4
c068ee0c t _initcat 니nput_ init4
c068ee10 t     initcal l rtc ini14
c068ee似 t _initcal 니2c_Q口io_ init4
c068ee18 t _initcal l_ i2c_adap_s3cjnit4
c068ee1c t Hm initcal匕P0州er＄叩이 y_class_ ini t4
c068ee20 t     initcal l h川mon init4
 c068ee24 t _initcal l_watchdog_ ini t4
 c068ee28 t    initcat i mmc init4
 c068ee2c t .1initcal匕s2叩引ic나； inr t4
c068ee30 t     initcal l i io init4
 c068ee34 t    initcal l m it soundcore4
 c068ee38 t    initcal l alsa sound ini t4
c068ee3c t _initcal l_proto_ init4
 c068ee40 t JnitcaI I_net_dev_ ini t4
c068ee44 t _initcal匕neiQh_ init4
c068ee48 t _initcat 匕gen匕init4

c068ee4c I   initcat l5 start
c068ee4c t 1나mni tcal匕이oc工叩_ init5
c068ee50 t 小_ini tcal 匕din之的buQ_do_ init5
c068ee54 t _initcal I_al ignment_ in1 t5
c068ee58 t _initcal匕이吼的ourc已的ie上oot i ng5

                                           157 / 312
커널연구회（ww岫erne나끄）                                       정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                             4. Device Tree 실습




c068ee5c t _initcal 니nit_pipe_fs5
c068ee60 t _initcal l_eventpol l_ init5
c068ee64 t    initcal l anon mnode init5
c068ee68 t _initcalLproc_cmdl ine_ init5
c068ee6c t _initcal匕아0（乙cons이es그ni t5
c068ee70 t _initca!匕아oc工四in化in나5
c068ee74 t _initca!匕아oc d到ices_ in 1t5
c068ee78 t _initcal l_ 汀oc_ interrupts_ init5
c068ee7c t _initcal I_proc_ Ioadavq_ init5
（乂）68ee80 t __initcal匕아oc m帥info_ in I t5
c068ee84 t _ini tcal I_proc_stat_ mni t5
c068ee88 t _initcal l_proc_uptime_ init5
c068ee8c t _initcal l_아oc_version_ init5
c068ee90 t _initcal l_아oc 5야 t 나qs_ mnit5
c068ee94 t _initcal匕아0（乙帥羽_ ini t5
c068ee98 t _initcal l_proc_page_ mn1t5
c068ee9c t    ini tcal I_ mni t_ramfs_ fs5
c068eea0 t _initcal l_blk_scsi_ ioctl_ init5
c068eea4 t    initcal l fb console init5
c068eea8 t 小initcal匕引畔니efb_ ini t5
c068eeac t    initcal l chr dev in1t5
c068eeb0 t    initcaI I_firmware_class_ init5
c068eeb4 t    initcal l thermal init5
c068eeb8 t _initcal l_sysctl_core_ init5
c068eebc t    initcal l eth off load init5
c068eec0 t __initcalLinet_ init5
c068eec4 t _initcal l_巾v4_offload_ in1t5
c068eec8 t    initcal l at unix init5
c068eecc t _initcal l_ ipv6_offload_1nit5
c068eed0 t _initcal Lpopulate_rootfsrootfs
c068eed0 I    initcal lrootfs start

c068eed4 I   in1tca1 16 start
c068eed4 t _initcal匕bL_switcher_dummy_if_ init6
c068eed8 t _initcal 나roc_execdomains_init6
c068eedc t   initcal l ioresources init6
c068eee0 I _initcal l_ init_sched_debug_procfs6
c068eee4 t _initcal l_ irq_gc_ init_ops6
c068eee8 t _initcal匕i rq_pm_ init_ops6
c068eeec t _initcal l_ init_posix_ timers6
c068eef0 t _initcal 匕m i 냐兀引 x1（和u_ f imers6
c068eef4 t _initcal匕timekeeping_ mnit_ops6
c068ee18 t _initcal l_ mnit_clocksource_sysfs6
c068ee1c t _initcal l_ init_ timer_l ist_procfs6
c068e100 t   initcal l alarmtimer init6
c068e104 t _initcal匕clockevents_init_sysfs6
c068e108 t _initcal l_sched_clock_syscore_1nit6
c068e10c t   initcal l futex init6
c068ef10 t _initcal匕아oc Ni的띠es_ in it6
c068ef14 t _initcal匕kal lsyms_1n1t6
c068ef18 t _initcal 냐id_narnespaces_ init6
c068e11c t _initcal I_utsname_sysctl_ init6
c068e120 t _initcal l_ init_per_zone_wmark_min6
c068ef 24 t 尸in i tcal 匕ks바apd_ ini t6
c068ef28 t 卞jnitcal匕extfrag_debuQ_1n1t6
c068ef2c I _initcal l_setup_vmstat6

                                                158 / 312
커널연구회（www.ker爬lb기                                           정재준 (rgbi3307@nate.com)
Device 가ee 상세분석 in 니flux Kernel 4.0                          4. Device Tree 실습    159




c068ef30 t _initcal匕mnicom口ute上카ch_init6
c068ef34 t _initcal l_引的巾roc그ni t6
c068et38 t _inhtcal匕work in小이_ init6
c068ef3c t _initcal l_proc_vmal loc_ init6
c068ef40 t _initcal l_me的lock_ init_debugfs6
c068ef44 t _in如al匕아ocswa叩Jni田
c068ef48 t _initcal匕引的_sysfs中init6
c068ef中二 t _initcal匕fcntl init6
c068ef50 t _initcal Lproc_fi lesystems_ init6
c068et54 t _initcaH_start_dirtytime_writeback6
c068ef58 I    initcal l dio init6
c068et5c t _initcal l_fsnotify_rnark_ init6
c068ef60 t _initeal l_dnotify_ in1t6
c068e164 t _inhtcal l_ inotify_user_setup6
c068ef68 t _initcal l_aio_setup6
c068ef6c t _initeal 냐片oc그ocks_ init6
c068ef70 t _initcal Linit_mbcache6
c068ef74 t _ini teal I_ mni t_devpts_ ts6
c068ef78 t _initcal l_ init_ext3j86
c068ef7c t __initcal l_ init_ext2_fs6
c068ef80 t _initcal l_ext4_init_f$6
c068ef84 t _initcal l_ journal_ init6
c068ef88 t _inhtcal l_ journal_ init6
c068e18c t __initcal l_ init_cramfs_fs6
c068ef 90 t _initcat l_ init_fatjs6
c068ef94 t    initcal l i nit vfat fs6
c068ef98 t _initcal I_ init_msdosfs6
c068et9e t _initcal I_ init_nls_cp4376
c068e1a0 t _initcal 1_ init_nis_asci i6
c068eta4 t    initcal l_ iniLnls_ iso8859 16
c068efa8 t    initcal l init romfs Is6
c068efac t Hm nm 托al l_ i미口ni (6
c068efb0 t _initcal l_ ipc小sysct匕 init6
c068etb4 t 寸initcal l_crypto_a山叩i init6
c068efb8 t _initeal匕chainiv_module_ init6
c068ef be t _initeal l_eseqiv_module_ init6
c068efc0 t _initcal匕sha256_gener ic_mod_ mnit6
c068efc4 t _initeal l_crypto_cbc小odule_ init6
c068ef好 t __ini teal 1_aes_ ini t6
c068ef cc t _initcal匕crc32c_的d_ init6
c068ef拘 t Hinitcal匕kr叩_mod_ in it 6
e068efd4 t 1h기 teal 냐玎0（乙genhd_ ini t6
c068efd8 t _initcal l_ init_emergency_poo16
c068efdc t _initcal l_noop小ii키 t6
c068efe0 t    mnitcal l deadl ine ini t6
c068efe4 t __initcal l_cfci_ init6
c068efe8 t 寸＋initcal l_percpu_ 兀un t아 없artup6
c068e1ec t _initcal Lphy_core_ init6
c068eff0 t 11m i teal匕exynos_dp_미由아phy_dr iver_ init6
c068eff4 t Hm i teal匕exynos小巾匕미 配아phy_먀 iv아_ mnit6
c068eff8 t m小m ni teal 匕samsun吼四b2_phy_dr iver_ini t6
c068o1fe t _中ini teal I_exynos5_usb3drd_phy_ ini t6
c068f 000 t 1m i teal 匕애1兀sa胎Un且driver尸init6
c068f 004 t 1initcal匕이 計 form그 ed펴r iver_ ini t6
c068f 008 t 小m i teal匕qener icbL （打 iver_ init6
c068f00c t _initcal I_pwm_backl ight_driver_ init6

                                          159/ 312
커 널 연구회佃ww.kerne나끄）                                     정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니nux Kernel 4.0                         4. Device Tree 실습    160




c068f010 t _jnitcal匕exyno乞ml이뗘S匕driver_ init6
c068f014 t _initcal l_p1330_driver_ init6
c068f 0侶 t _initcal匕max77693巾川c_dr iver_ ini t6
c068f01c t _initcal匕max77802j加比뗘r iver_ ini t6
c068f020 t _initcal I_s2mpa01_pmic_driver_ init6
c068f024 t _in나cal l_pty_ init6
c068f028 t _initcal匕sysrq_ init6
c068f02c t __initcal l_seria18250_ init6
c068f030 t _initcal I_samsung_serial_driver_ init6
c068f034 t 尸initcal匕이-r니atf아兀ser 泊匕dr iver_ ini t6
c068f038 t _initcal l_hwrng_modinit6
c068f03c t _initcal I_exynos_rng_driver_1n1t6
c068f040 t _戶initcal匕rng_1nit6
c068f044 t __initcal匕tpmjis_12c_driver_ init6
c068f048 t    initcal t drin core init6
c068f04c t _initcal l_exynos_drm_ init6
c068f050 t _initcal匕pane匕引叫키e_ ini t6
c068f054 t _.Jnitcal Lptn3460_driver_ init6
c068f058 t -_Jnitcal I_ topology_systs_ init6
c068f05c t __initcal l_cacheinfo_systs_init6
c068f060 t    initcal l brd init6
c068f064 t _initcal l_ loop_ init6
c068f068 t __initcalLinit_cryptoloop6
c068f06c t _initcal l_cros_ec_driver_ init6
c068f070 t _initcal l_cros_ecdriver_spi_1n1t6
c0681074 t    initcal l init sd6
c068f078 t _Jnitcal 니nit_sq6
c068f07c t _initcal匕s3c64xx_sp匕山 i ver그n1t6
c068f080 t    initcal l net olddevs init6
c068f084 t _initcal l_smsc9llx_ init_rnodu1e6
c068f088 t    initcal l asix driver init6
c068f08c t    initcal l ax88179 178a driver init6
c068f090 t    initcal l cdc driver init6
c068f094 t    initcal l smsc75xx driver init6
c068f098 t __ini tcal l_smsc95xx_dr iverini t6
c068f09c t    initcal l net1080 driver init6
c068f0a0 t    initcal l cdc subset driver init6
c068f0a4 t ._.initcal I_zaurus_driver_ init6
c068f0a8 t _initcal l_usbnet_ init6
c068f0ac t    initcal l cdc ncm driver init6
c068f ObO t   initcal l dwc3 driver init6
c068f0b4 t _initcal匕d나c3小exyno乞driver_init6
c068f0b8 t _initcal l_xh이巾治t_ ini t6
c068f0bc t _initcal I_ehci_hcd_ init6
c06810c0 t _initcal 匕ehc匕exynos_1nit6
c068f0c4 t _initcal l_ohci_hcd_mod_ init6
c068f0c8 t _ini tcal I_ohci_exynos_ ini t6
c068f Ccc t _initcal l_xhci_hcd_ init6
c068f0d0 t _initcal l_usb_storage_driver_ init6
c068f0d4 t    initcal l usb3503 init6
c068f0d8 t _initcal l_serport_ init6
c068f0dc t    initcal l mousedev init6
c068f0e0 t _initcal l_evdev_ init6
c068f0e4 t    initcaI I_atkbd_ init6
c068t 0e8 t _initcal l_cros_ec_keyb_driver. init6
c06810ec t _initcal匕samsung_keypad_driver_ init6

                                           160 / 312
커 널 연구회（www.kerne比기                                    정재준 (rgbi3307@nate.com)
                                                              4. Device Tree 실습   ]61
Device Tree 상세분석 in Linux Kernel 4.0




c068f0f0 t _initcal l_cyapa_driver_ in1t6
c068f0f4 I _ini tcal匕mxt_dr iver_ ini t6
c068f0f8 t _initcal l_max77686_rtc_driver_init6
c068101c t _initcal匕max77802_rtc_driver_1n1t6
c068f100 I _initcal l_s3c_rtc_driver_ 1n1t6
c068f104 t _initcal匕s5m_rtc_driver_1n1t6
c068f108 t _initcal l_12c_dev_ 1n1t6
c068f10c t _initcal l_exynos5_12c_driver_1n1t6
c068f110 t _initcal匕ec_12c_ tunnel_driver_ 1n1t6
c068f114 t _initcal l_12c_arbitrator_driver_init6
c068f118 t 尸initcal I_的乞battery_dr i陀乙ni t6
c068fllc t _initcal l_max17040_ 12c_dr iver_1n1t6
c0681120 t _initcal l_rnax17042_12c_driver_ init6
 c0681124 t _initcal匕max14577_charger_driver_1n1t6
 c068f128 t _initcal匕max77693야）a띠e乙dr iver_ ini t6
 c068f12c t _initcal匕tps65090_charger_driver_ 1n1t6
 c0681130 t     initcal l 1m90 driver init6
 c068f134 t _ini tcal I_exynos_ tinu_dr iver_ ini t6
 c068f138 t jnitcal l s3c2410川dt driver 1n1t6
 c068f13c t _initcal l_dm_1n1t6
 c068f140 t _initcal l_rnmc_blk_ init6
 c068f144 t     initcal l sdhci dry 1nit6
 c068f148 t     initcal I sdhci s3c driver init6
 c068114c t      initcal l dw mci 1n1t6
 c068f150 t -그 ni tcal匕曲mc匕p1 tfrn_dr iver_ini t6
 c0681154 t _initcal匕伽小C匕exynos_pltf旺driver_ init6
  c0681158 t _initcal l_hid_ init6
  c068f15c t _initcal匕hid_generic_ in1t6
  c068f160 t _initcal I_a4_driver_1nit6
  c0681164 t _initcal l_apple_driver_ in1t6
  c068f168 t __initcal l_be나in_driver_1n1t6
  c068f16c t 나initcaI I_ch_driver_ init6
  c068f170 t _initcal l_ch_driver_ init6
  c068f174 t _initcal I_cp_driver_ ini t6
  c068f178 t _initcal l_ez_driver_ 나1t6
  c068f17c t _ini tcal I_ks_dr iver_ ini t6
  c0681180 t _initcal l_ Ig_driver_ init6
  c068f184 t      initcal l ins driver ini t6
  c068f188 t      initcal l mr driver 1n1t6
  c068f18c t 尸ni tcal匕이帥tr이ii cs펴r iver_ ini t6
   c068f190 t     initcaI I_hid_ init6
   c068f 194 t __initcal I_max77686_c나_  (driver_ 1n1t6
   c0681198 t _initcal I_max77802_clk_driver_1n1t6
   c068f19c t     initcal l extcon class init6
   c06811a0 t _initcal l_max14577_muic_driver_ in1t6
   c068f1a4 t _initcal I_max77693_muic_driver_ init6
   c068f1a8 t __initcal I_exynos_adc_ driver_ in1t6
   c068f1ac t _initcal l_alsa_timer_ init6
   c068f1b0 I _initcal匕alsa_pcm_ init6
   c068f1b4 t _initcal匕snd_compress_ in116
   c06811b8 I __initcal I_snd_soc_ ini t6
   c068f1bc t _initcal I_max98090_12c_driver_1n1t6
   c068f1c0 I _initcal匕max98095_ 12c_driver_1n1t6
   c068f1c4 t _initcal匕sacnsun_ i2s_driver_ init6
   c06811c8 I _initcal l_asoc_ idma driver_ init6
   c068f1cc t _initcal l_snow_driver_ in1t6

                                               161 / 312
 커 널 연구회（www.kern이.b기                                      정재준 畇bi3307@nate.com)
 Device Tree 상세분석 in 니flux Kerr佃 4.0                                                  4. Device Tree 실습   ]62




 c068f1d0 t _ini tcal匕sock_d泊g_ ini t6
 c068f1d4 t _initcal l_gre_oftload_ init6
 c068f1d8 t _initcal l_sysctl_ 1pv4_ init6
 c068f1dc t _initcal l_xfrm4_beet_ init6
 c068f1e0 t _initcal匕xfrm4_ transport_1nit6
 c068f1e4 t _initcal l_xfrrn4_cnode_ tunnel_ init6
 c068t1e8 t _initcal l_ inet_diag_ init6
 c068f1ec t _initcal 나C口di叩_ init6
 c068f1f0 t __initcal !_cubictcp_register6
 c068t1f4 t _그nitcal匕packet_1n1t6
 c068f1f8 t _initcal 니psec_pfkey_1nit6

 c068f1fc I _initcal 17_start
 c068f1fc t _initcal匕in it_rn配hi肥_Iate7
 c068f200 t _in나Cal 匕S빠) em미카 山n_ mni t7
 c068f204 t _initcal l_bL卄switcher_1n1t7
 c068f208 t 卜initcal匕init_oops_ id7
 c068f20c t _initcal l_sched_init_debug7
 c068f 2化 t _initcal 냐m小qos_ 冷빠er_ in it7
 c068f214 t _initcal l_prn_debu아s_ mnit7
 c068f218 t _initcal I_pr intk_Iate_ init7
 c068f21c t _initcal l_ tk_debug_sleep_ tirne_ init7
c068f220 t _initcal l_tau나中카ound뗘的叩t s7
c068f 224 t 小ni tcal 匕ma凡5나apf i Ies_check7
c068f 228 t _initcal 匕prandorn_reseed7
c068f22c t 寸_ initca!匕化_logo그ate_ in it7
c068f230 t _initcal l_deferred_probe_ initcal l7
c068f234 t _initcal匕genpd_powerotf_unused7
c0681238 t __initcal匕gpio_keys_ init7
c068f23c t _initcal匕rtc_hctosys7
c068f240 t _initcal l_of_fdLraw_init7
c068f 244 t 戶 in itca I I_c作匕由bu且ni t7
c068f248 t _initcal匕tcp_congestion_defau1t7
c068f24c t _initcal I_regulator_init_co叩lete7s
c068f250 t _initcal l_clk_disable_unused7s
c0681254 t _initcal l_alsa_sound_last_init7s
c068f258 I _con_initcal I_start
c068f258 t    initcal l Con mnit
c068f258 T    initcal l end




커널은 위에 등록된 呵tcall 함수들을 통하여 디바이스 드라이버들을 초기화 한다.                                              따라서 각종
디바이스 드라이버들은 이 함수들에서부터 실행이 시작된다．


필자는 /init/rn리n.c 소스 파일의 do_orre_initcall() 함수에 아래와 같이 디버그 코드를
                                                       직접 삽입하
여 위의 initcall 함수들이 실행되는 로그를 printk로 출력해서 확인해1 봤다. （굵은
                                                      글씨처마 필자
가 추가한 디버그 메세지를 출력하는 코드이다）



#def ine USER, .DEBUG(fmt, args. . .)                                                 w
          do {                                                                        뾰
                     printk( '/ /KDBG:%s:%d: '' frnt, _func__,   LINE   , ##args) ;   w

                                                  162 / 312
커 널 연구회佃ww.kern이.b기                                                           정재준 (rgb日307@nate.com)
Device 가ee 상세분석 in Linux Kerr佃 4.0                                                       4. Device Tree 실습      163




            } 岵ii le (0)



    nt_ init_or_nioduledo_one inj tcal l ( jnj tcal匕t fn)
{
          ft count = preempt_count ( ) ;
        1 nt ret;
        char msobuf[ 64] ;
倂fdef C에F田_USER_DEBJJG_BOOT
        char *fn.mname;
#end if

         사USER少EBUG_BOOT( "The St三n                                                              싻n',
#ifdef CO卜Ii기G_USER_DEB1．用 旼XT
         fn咽肥 = kasprintf (呼巳旺剛EL, H琡）尸 , fn) ;
         USER_DEBUG( 'f n_name: 美sWn ' , f n_name) ;
         kfree(fn_name) ;
#end it

            it ( initcal匕blackl isted(tn) )
                      return -EPERM;

            it ( initcal I_debug)
                      ret = do_one_ initcal I debug(fn) ;
            e I1 Se
                 se
                      ret = fn() ;

            msgbuf[ 0] = 0;

                f (preempt_count () != count) {
                        S아 intf (msgbuf , ’工玎eem口tion imbalance ") ‘,
                        preernpt_count_set (count) ;
            }
                f ( i rqs_disabledO) {
                          str lcat (msgbuf , :dIsat니ed interrupts   引zeof (ms야）Ut) ) ;
                          I oca匕 나 4帥的陀（) ;
            }
            WARN(msgbuf[ 0I , "initcal l %pF returned wi th %sWn ' , tn, nisgbuf) ;

            //USER_DEBUCBOOT( 'The End                                                       神

            return ret;
}


위의 코드를 빌드하여 커널을 다시 부팅하면 아래와 같이 디버그 메시지가 출력되는 결과를 확인
할 수 있고, 커 널이 부팅되면서 어떤 initcall 함수가 실행되는지 그 명칭을 알 수 있다.                                                  아울러 디
바이스 드라이버가 시작되는 초기화 함수（진입함수）를 확인할 수 있다． " "//KDBG:" 로 시작되는 문
자열이 필자가 추가한 디버그 메시지이다．



커널 부팅 로그（디버그 매시지）


                                                       163 / 312
커 널 연구회佃ww.kerne比기                                                                 정재준 四bi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                             4. Device Tree 실습      ]64




Starting kernel . .

f/ star tj<erriel () 』. .
[      0.000000] Booting Linux on physical CPU Ox0
[      0.0000001 Linux version 4.0.0 (jungjj@kernel . bz) (gcc version 4.6. x-google 20120106
(prerelease) (6CC) ) #1 SMP PREEMPT Tue May 5 09: 42: 48 KST 2015
[
       0.0000001 CPU: ARMv7 Processor [412fc0f3] revision 3 (ARMv7) , cr=10c5387d
[
       0.0000001 CPU: PlPT / VlPT nonal iasing data cache, PlPT instruction cache
[
       0.000000] Machine model : Insignal Arndale Octa evaluation board based on EXYNOS5420
[
       0.0000001 cma: Reserved 64 M汨 at 0x9b800000
rL [
       0.0000001 Memory pol icy: Data cache writeal loc
       0.0000001 Samsung CPU ID: 0xe5420020
[
       0.0000001 Running under secure firmware.
[
       0.0000001 PERCPU: Embedded 10 pages/ cpu @ee77d000 s11136 r8192 d21632 u40960
r느 [
       0.0000001 Bui lt 1 zonel ists in Zone order, mobi l ity grouping on. Total pages: 517136
       0.0000001 Kernel command l ine: console=ttySAC3,115200n8 root=/dev/ ram0 init=/sbin/ init
 mni trd=0x21000000,32M ramdisk=32768
[      0.0000001 PID hash table entries: 4096 (order: 2, 16384 bytes)
[      0.0000001 Dentry cache hash table entries: 131072 (order: 7, 524288 bytes)
[      0.000000] 1 node-cache hash table entries: 65536 (order: 6, 262144 bytes)
[      0.0000001 Memory: 1951528K/2074624K avai lable (4734K kernel code, 193K rwdata, 1728K rodata,
240K m it, 275K bss, 57560K reserved, 65536K cma-reserved, 1239040K highmem)
 [     0.000000] Virtual kernel memory layout:
 [     0.0000001          vector : 0xff ff0000 - 0xffff1000    (   4 kB)
 [     0.0000001          t ixmap : 0xffc00000 - 0xfff00000    (3072 kB)
 [     0.000000]          vmal loc : 0xf0000000 - 0xff000000   ( 240 MB)
 [     0.000000]          lowmem : 0xc0000000 - 0xe1800000     ( 760 MB)
 [     0.000000]          pkmap      : 0xbfe00000 - 0xc0000000 (   2 MB)
 [     0.0000001          modules : 0xbf000000 - 0xbfe00000    ( 14 MB)
 [     0.0000001              .text : 0xc0008000 - 0xc0657c10  (6464 kB)
 [     0.000000]              . m it : 0xc0658000 - 0xc0694000 ( 240 kB)
 [      0.000000]             . data : 0xc0694000 - 0xc06c4740 ( 194 kB)
 [      0.000000]               .bss : 0xc06c4740 - 0xc07093c0 ( 276 kB)
 [      0.0000001 SLUB: I刪al ign=64 , 야der=0日, 씨n아기ects=0, CPUs=8, Nodes=1
 [      0. 000000] 마eempt 仕기e hier카ch比al R（기 im1키ementat ion.
 [      0.0000001 Additional per-CPU info printed with stal ls.
 [      0.0000001 NR_ IRQS:16 nr_ irqs:16 16
 [      0.000000] GIC physical location is 0x10481000
 [      0.0000001 L2C: fai led to mnit: -19
 [      0.000000] Switching to timer-based delay loop, resolution 4lns
 1      0.0000061 sched_clock: 32 bits at 24MHz, resolution 4lns, wraps every 178956969942n5
  [     0.0002931 Console: colour dummy device 80x30
  [     0.0003211 Cal ibrating delay loop (skipped) , value calculated using timer frequency. . 48.00
 BogoMIPS ( lpj=240000)
        0.0003401 pid_rnax: default: 32768 minimum: 301
        0.0005011 Mount-cache hash table entries: 2048 (order: 1, 8192 bytes)
        0.0005151 Mountpoint-cache hash table entries: 2048 (order: 1, 8192 bytes)
        0.0012141 CPU: Testing write buffer coherency: Ok
        0.001247] !/KDBG: start小kernel :686: The End

I/ rest_ mni tfl. . .
      0.0012591 //KDBG: start_kernel :687: rest_ initO. . .
      0.001270] //KDBG: rest_init: 388: The Start
      0.001407] //KDBG: resLinit:398: kerne匕thread(kernel_init) : pid=1.
      0.001441] //KDBG: rest init:405: kernel_ thread(kthreadd) : pid=2.
      0.001461] I/ KDBG: kthreadd:489: The Start

                                               164 / 312
 커 널 연구회佃川w.kern이.b기                                                       정재준 (r야)13307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                              4. Device Tree 실습     ]65




[    0. 001483] /!KOBG:kernel inie:964: The Start

//kernel_ init_ freeable()
[    0.001493] //KDBG:kernel_ ini _ freeable:1019: The Start
[    0.001671] CPUO: update cpu_古apacity 1535
[    0.001683] CPUO: thread -1, cpu 0, socket 0, mpidr 80000000
     0.00侶35] //KDBG; do_one_ ini caI i :801; f n_name: cpu_suspend_al loc_ep
     0.00化63] //IKDBG: do_one_ initca1 l :801; tn_name: init_static_ idmap
     0.001891] Setting up static identity map for 0x2047d688 叫 0x2047d6e0
     0. 001920] //KDBG: do_one_ initcal l :801: fn_name: exynos多cpm_init
     0.001996] //KDBG: do_onejni ttcal 1 :801: tn_name: spawn_ksott i rqd
     0.002035] !/KDBG:kthreadd:5가t: create_kthread(create) . . .
     0.0200伶］ //KDBG: do놔one_ initCal l :801: fn_name: init_workqueues
     0.020141] //KDBG:kthreadd: 514: create_kthread(create) . . .
     0.020250] //KDBG:kthreadd:514: create_kthread(create) . . .
     0.020459] !/KDBG:kthreadd:514: create_kthread(create) . .
     0.020658] //KDBG: do_one_ initcai l :801: tn_name; m igration_ mnit
     0.020690] //KDBG: do_one_ initcal l :801: tn_name: check_cpu中stal l_ m it
     0. 020711] //KDBG: do_one_ initcai 1 :801: tn_name: rcu_spawn_gp_kthread
     0.020737] //KDBG:kthreadd: 514: create_kthread(create) . . .
     0.020817] !/KDBG:kthreadd:514: create_kthread(create) . . ,
     0.020888] //KDBG: kthreadd: 514; create_kthread(create) . , .
     0.020957] //KDB0: do_one_ initcal i :801: tn_name: cpu_stop_ mnit
     0.020987] //KDBG:kthreadd:514: create_kthread(create) . . .
     0.040031] //KDBG: do_one_ initcal 1 :801; tn_name: ,cci_ init
     0.040056] //KDBG: do_one_ initcal i :801: tn_name: rand_ ini tial ize
     0.040397] //KDBG: do_one_ initcal i :801: tn_name: dummy_ timer_register
     0.040433] //KDBG;kthreadd:514; or eate_kt hread( Cr eat e) . .
     0.060196] //KDBG: kthreadd:514; create_kthread(create) . .
     0.060300] //KDBG: kthreadd:514; create_kthread(create) . . ,
     0.080014] IIKDBG:kthreadd:514: create_kthread(create) . .
     0.080115] //KDBG:kthreadd:5141 create.j<thread(create) . .
     0.0802051 月KDBG 水 threadd:514: or eate_k t hr ead( cr eat e) , , .
     0.081369] cPu1 : update 야）u놔ca口acity 1535
     0.081376] CPti1: thread -1, cpu 1, socket 0, mpidr 80000001
     0.081510] //KDBG; kthreadd; 514: Cr eats_k t hr ead( cr eate) . . .
     0.081602] f/KDBG:kthreadd: 514; Cr eate_k t hr ead( create) . . .
     0. 100016] IIKD80: kthreadd:514: create_kthread(create) . . .
     0.100133] !/KDBG:kthreadd:514: create_kthread(create) . , ,
     0.100224] //KDBG:kthreadd:514: create_kthread(create) . .
     0. 101379] CPU2: update cpu_capacity 1535
     0.101387] CPU2: thread -1, cpu 2, socket 0, mpidr 80000002
     0.101520] !/KDBG:kthreadd: 514; create_kthread(create) . . ,
     0.101605] //KDBG:kthreadd: 514; create_kthread(create) . . .
     0. 120015] /!KDBG:kthreadd:514; create_kthread(create) . . .
     0.120121] IIKDBG;kthreadd:514: create_kthread(create) . . .
     0.120211] /!KDBG:kthreadd:514: create_kthread(create) . . :
     0月213641 CPU3: update cpu_capacity 1535
     0.12］釘1] CPU3: thread -1, cpu 13, socket 0, mpidr 80000003
     0.121507] //KDBG;kthreadd: 514: 口reate_kthread(create) .. .
     0.121604] //KDBG:kthreadd:514: 나eate_kthread(create) . . .
     0. 140015] //KDBG:kthreadd:514: reate_kthread(create) . ' .
     0. 140123] //KDBG:kthreadd:514: create_kthroad(create) . . .
     0. 140212] //KDBG:kthreadd: 514: create_kthread(create) . . .
     2. 140017] CPIJ4: tai led to come Onl ine
     2. 1400731 //K08G:k나＼readd:5t4: 아eate kthread(create) . . .

                                                165 / 312
커 널 연구회（w蜘床아nel.bz)                                                         정재준 (rgbi3307（흐）nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                               4. Device Tree 실습    ]66




     2.1401561 //KDBG:kthreadd:514: create kthread(create) . . .
     2.1600311 //KDBG:kthreadd: 514: create_kthread(create) , . .
     2.1601301 //KDBG:kthreadd: 514: creat e_kthread(create) . .
     2.160220] !/KDBG:kthreadd:514: create_k thread( create) . - .
     4.1600331 CR15: fai led to come on I i ne
     4.1600861 //KDBG:kthreadd: 514: create_kthread(create) . .
     4.160171) //KDBG: kthreadd: 514: create_kthread(create) . . .
     4.1800491 //KDBG:kthreadd: 514: create_kthread( create) . . .
     4.180150] //KDBG:kthroadd: 514: create_kthread(create) . . .
     4.1802461 //KDBG:kthreadd:514: create_kthread(create) . . .
     6.1800501 CR16: fai led to come onl ine
     6.1801021 //KDBG:kthreadd:514: create_kthread(create) .. .
     6.1801921 !/KDBG:kthreadd: 514: ereate_kthread( create) . . .
     6.200065) //KDBG:kthreadd:514: create_kthread(create) . . .
     6.200170) //KDBG: kthroadd: 514: ereate_kthread(creale) . . .
     6.200260] //KDBG:kthreadd: 514: create_kthread(create) . .
     8.200066] CPU7: fai led to come onl ine
     8.2001011 Brought up 4 CPUs
     8.2001131 SMP: Total of 4 processors activated (192.00 BogoMIPS) .
     8.2001231 CPU: Al l CPU(s) started in SVC mode.

 Ido_bas i c_setupO. . .
     8.200343] !/KDBO:do_basic_setup:900: The Start
     8.200395] /!KDBO: k卄｝readd: 514: create_kthread(create) . . .
     8.200582] //KOBG:kthreadd:514: create_kthread(create) . .
     8.2008111 devtmpfs: initial ized

 /do_ initcal 나evelU: 0: early. . .
     8.202803] //KDBG: do_ initcal I_ level :870: [early]
     8.202868] //KDBG: do_one_ ini tcal 1 :801: tn_name: ipc_ns_ ini I
     8.202888] //KDBG: do_one_ initcal l : 801: tn_name: init_mmap_min_addr
     8.2029101 //KDBG: do_one_ initcal l :801: fn_name: net_ns_init
     8.2029831 //KDBG:kthreadd:514: create_kthread(create) . .

 /do initeal l level () : 1: core. . .
     8.2030981 //KDBG: do_ initcal l_ level :870: [core]
     8.2031551 //KDBG: do_one_ ini tcal 1 : 801: tn_name: vIp_ mni t
     8.203179] VFP support v0.3: implementor 41 architecture 4 part 30 variant f rev 0
     8.203210] //KDB（土面_one_ ini teal 1 :801: tn_name: 口tra四力reak_ ini t
     8.203235] //KDBG: do_one_ initcal l :801: tn_name: v6_userpage_init
     8.2032611 I /KDBG:的_one_ initcal ! :801 : fn小name: 야）u_hotr）山g_pm_syn乙nit
     8.203286] //KDBO: do_one_ initeal i : 801: tn_name: al loc_ frozen_cpus
     8. 203311] //KDBG: do_one_ ini teal 1 :801: tn_name: wa_systs_ ini t
     8.203400] /IKDBG:kthreadd:514: create_kthread(create) . . .
     8.203661] //KDBG: do_one_ initcal 1 :801: tn_name: ksysfs_init
     8. 203734] //KDBG: do_one_ ini teal 1 :801: tn_name: pm_ m i t
     8. 203971] //KDBG: do_one_ ini teal 1 :801: fn_name: m!ll t_ j i tf ies_clocksource
     8.203995] //KDBG: do_one_ 나1itcal 1 :801: tn_name: cgroup_wq_ init
     8.204203] //KDBG: do_one_ mni teal 1 :801: tn_name: epu_pm_ in it
     8.204227] //KDBG: do_one_ mnitcal 1 :801: tn_name: init_zero下tn
     8.204253] (/KDBG: do_one_ inm teal 1 :801: tn_name: cma_ ini t_reserved_areas
     8. 205551] //KDBl3: do_one_ ini teal 1 : 801: tn_name: t sn아 1 h乙nit
     8.205583) //KDBG: do_one_ mni teal 1 :801: tn_name: ti lelock nit
     8.205640] IiKDBG: do_one_ ini teal 1 :801: tn_name: init_ser ipt_binfmt
     8.2056651 //KDBG: do_one_ mni teal 1 :801: tn_name: mnit elf binfint
     8.205687] //KDBG: do_one_ mni teal 1 :801: tn_name: debugfs_ ini t

                                                 166 / 312
커 널 연구회（www.kern이.b기                                                          정쟤준 (rgbi3307@nate.con가
Device Tree 상세분석 in Linux Kernel 4.0                                                 4. Device Tree 실습   167




    8.2057221 /!KDBG: do_one_ i n iltcal 1 :801: tn_name: securityts_init
    8.2057551 /!KDBG: do one ini caI 1 :801: tn_name: prandom_ init
    8.205783] / /icuod.ao_one_ i n1{ cai 1 :801: tn_name: cci_ 니atform_init
    8.205803] /!KDBG:do_one_ in 1tcal f :801: tn_name: pinctr匕init
    8.205817] pinctrl core: initial ized pinctrl subsystem
    8.205924] //KDBG: do one initcal ! :801: tn_name: regulator_ 汀｝it
    8.206724] //KDBG:do_one_ ini t cal i :801: fn name: of 1nit
    8.228430] //KDBG: do one ini tcal 1 :801: t n_name: exynos_audss_clk_ mni t
    8.228580] //KDBG: do_one_ ini fcal 1 :801: fn_name: sock_ mnit
    8.228705] //KDBG: do_one_ initcal 1 :801: tn name: net m }use 1nit
    8.228737] //KDBG: do_one_ ini tcal I :801: tn_name net I in凡미oto_ ini t
    8.228970] NET: Registered protocol fami ly 16

 !do_ mnitcal l_ levelO: 2: postcor . . ,
     8.229013] //KDBG: do_ mni teal 亡level :870: [postcorej
     8.229074] //KDBG: do_one_ initca I :801: tn_name: atomic_pool_ m it
     8.230600] DMA: preal located 256 KiB pool for atomic coherent al locations
     8.230622] //KDBG:do_one_ initcal l :801: tn_name: exynos_pmu_ mnit
     8.230781] //KDBG:do_one_ mnitcal l :801: tn_name: bdi_class_init
     8.230901] //KDBG:do_one_ initeal l :801: tn_name: mrn_systs_init
     8.230937] !/KDBG:do_one_ initcal l :801: tn_name: kobject_uevent_init
     8.230974] //KDBG:do_one_ initcal l :801: tn_name: samsung_pinctrl_drv_register
     8.231108] //KDBG:do_one_mnitqai l :801: tn_name: lcd_class_mnit
     8.231212] //KDBG: do叫one_ initclal l :801: tn_name: backl ight_class_ init
     8.231315] //KDBG: do_one_ mnit寸al l :801: tn_name: .amba_init
     8.231475] //KDBG: do_one_ mnitgal l :801: tn_name: tty_class_ init
     8.231577] //KDBG: do_one_ init申l I :801: tn_name: vtconsole_class_ mnit
      8.231890] //KDBG: do_one_ initcal l :801: fn_name: iommu_dev_ mnit
      8.231997] //KDBG:do_one_ initcal l :801: tn_name: wakeup_sources_debu아s_ init
      8.232040] /!KDBG:do_one_ mn냐col l :801: tn_name: regmap_ initcal l
      8.2320781 /!KDBG:do_one_mnitcal l :801: tn_name: sram_init
      8.2322171 /!KDBG:do_one_ initcal 三:801: fn_name: syscon_ mnit
      8.2323521 //KDBG:do_one_ initcal l :801: tn_name: spi_ init
      8.232599] /!KDBG:do_one_ initcal l :801: tn_name: i2c_init

口‘do_ initcal l_Ievel0 : 3: arch. . .
     8.232863] //KDBG:do_ in汁cal I_ level :870: [arch]
     8.232921] //KDBG: do_one_ ini tcal 1 :801: tn_name: gate_vrna_ ini t
     8.232942] //KDBG:do_one_ ini teal 1 :801: tn_name: customize_machine
     8.243749] exynos-audss-c나； 3810000.audss-clock-control 1 er: setup completed
     8.251825] EXYNOS5420 PMU initial ized
     8. 2568681 //KDBG: do_one_ initcaI l : 801: tn_name: exce口tions_ m it
     8.256897] !/KDBG: do_one_ initcali l :801: tn_name: exynos4_pm_ ini f_power_domain
     8.257659] //KDBG: do_one_ in나ca1 1 :801: tn_name: s3c_arch_ init
     8.257685] /!KDBG: do_one_ initca1 1 :801: tn_name: dma_bus_ mnit
     8.257810] //KDBG:do_one_ initcal l :801: tn_name: dma_channel_ table_ mnit
     8.2578671 //KDBG: do_one_ initcal l :801: tn_name: iommu_init

  do_ mnitcal l_ levelO: 4: subsys. . .
     8.257899] //KDBG:do_ mni teal I_ level :870: [subsys]
     8.257957] //KDBG:do_one_ initcal i :801: fn_name: topology_ mnit
     8.259644] //KDBG: do_one_ mnitcaFl :801: tn_name: old_cache_ mnit
     8.259678] //KDBG: do_one_ initcal 1 :801: fnm'name: param_sysfs_ ini t
     8.276206] //KDBG: do叫one_ initcal l :801: tn_name: pm_sysrq_mnit
     8. 3200861 //KDBG: do_one_ initcal :801: tn_name: hung_ task_ mnit
     8.320117] //KDBG:kthreadd:514: create_kthread(create) . .

                                                  167/ 312
커 널 연구회（www.kern包b기                                                           정재준 杓bi3307@nate.com)
Device Tree 상세분석 ir) 니nux Kernel 4.0                                                4. Device Tree 실습   168




    8. 3202101 //KDBG: do_one_ initcai l :801: tn_name: default_bd나nit
    8. 3202641 !/KDBG:kthreadd:514: create_kthread(create) . . ,
    8. 3206051 //KDBG: do_one_ initcal l :801: tn_name: per cpu_enab I e_async
    8. 3206341 !/KDBO:do_one_ ini tcal 1 :801: tn_name: m} it reserve notifier
    8. 320658] //KDBG: do_one_ ini tcal 1 :801: tn_name: tni 1_admin_reserve
    8. 320676] !/KDBG: do_one_ ini Ical 1 :801: in_name: ni t user reserve
    8. 3206941 I/ KDBG: do_one_ mni tcal 1 :801: tn_name: crypto． 川qU！기 i
    8. 320821] //KDBG:kthreadd:514: create_kthread(create) . . '
    8. 320886] //KDBG: do_one_ ini tcal 1 :801: fn_name: cryptomgr_ ini
    8.320905] //KDBG: do_one_ initcal l :801: tn_name: init_bio
    8.32化80] //KDBG:kthreadd: 514: create_kthread(create) . . .
    8.3211461 /!KDBG: do_one_ initcal l : 801: tn_name: bik_settings_ ini t
    8. 321］弱］ /!KDBG: do_one_ initcal l :801: tn_name: blk_ ioc_ init
    8. 3211881 //KDBG: do_one_ initcal l : 801: tn_name: blk_softirq_ init
    8. 321211] //KDBG: do_one_ initcal l :801: fn_name: blk_ iopol I_setup
    8. 321232] /!KDBG: do_one_ initcal l :801: fn_name: blk_mq_ init
    8.3212531 //KDBG: do_one_ initcal l : 801: tn_name: genhd_device_init
    8. 321474] //KOBG:kthreadd: 514: create_kthread(create) . . .
    8. 3216081 /!KDBG: do_one_ initcal i :801: tn_name: gpiol ib_debugts_init
    8. 3216461 //KDBG: do_one_ ini tcal 1 : 801: tn_name: p娜_debugfs_ ini
    8. 321679] //KDBG: do_one_ initcal l : 801: tn_name: p蜘_systs_ ini t
    8. 321781] //KDBG: do_one_ initcal l : 801: tn_name: tbmem_init
    8. 3219041 !/KDBO: do_one_ initca! l :801: tn_name: regulator_ f ixed_voltage_init
    8.3221町］ //KDBG: do_one_ initcal l :801: fn_name: 야io_re야lator_ init
    8. 322448] //KDBG: do_one_ initcal l :801: tn_name: max14577_repulator_init
    8.322643] !/KDBG: do_one_ initcal l :801: fn_name: max8997_pmic_init
    8. 3228421 !/KDBG: do_one_ initcal l :801: fn_name: rnax77686_pmic_ init
    8. 3230391 //KDBG: do_one_ ini tcal 1 :801: tn_name: s2mpsll_pmic_ ini
    8. 323233] //KDBG: do_one_ initcal l : 801: tn_name: s5m8767_pmic_.init
    8. 323422] //KDBG: do_one_ ini tcal l :801: tn_name: tps65090_regulator_ init
    8.3236181 //KDBG: do_one_ initcal l :801: in name: misc_ mr} it
    8.323739] //KDBG: do_one_ ini tcal 1 :801: tn_name: tpm_ ini
    8.323844] //KDBG: do_one_ initcal l :801: tn_name: exynos_ lommu_ init
    8.324033] //KDBO: do_one_ initcal l :801: inHname: max14577_ i2c_init
    8.324173] /!KDBG: do_one_ ini Ical 1 :801: fn_name: max77686_ i2c_ini
    8.324317] //KDBG: do_one_ ini tcal l :801: tn_name: max77693_ i2c_ ini
    8.324451] //KDBG: do_one_ initcal l :801: tn_name: max8997_ i2c_ init
    8. 324585] //KDBG: do_one_ initcal l :801: fri_name: tps65090_ init
    8. 324717] //KDBG: do_one_ initcal l :801: in_name: sec_pmic_ init
    8. 324850] //KDBG: do_one_ initcal l :801: tn_name: dnia_but_ init
    8. 324902] /IKDBG: do_one_ ini tcal 1 :801: fn_name: m } i t_scsi
    8. 325427] SCSI subsystem initial ized
    8.325449] !/KDBG:
                //KDB(;:d0
                        do_one_
                           0ne ini
                                 n tcal    :801: tn_name: phy_ in it
                                    tCa1 1 :80]
    8.325898] //KDBG: do_one_ initcal l : 801: fn_na丹毛: usb_ init
    8.326246] usbcore: registered new interface driver usbts
    8.326414] usbcore: registered new interface driver hub
    8.326701] usbcore: registered new device driver usb
    8.326723] //KDBG:do_one_initcal l : 801 : tn_呻肥： U삯L岫乞m it
    8. 326833] //KDBG: do_one_ initcal l :801: tn_name: serjo. init
    8. 326990] !/KDBG: do_one_ initcal l :801: in_name: inputinit
    8. 327114] //KDBG: do_one_ initcal l :801: tn_name: rtc_ init
    8. 327217] //KDBG: do_one_ initcal l : 801: tn_name: i2c_gpio_ init
    8. 3274631 //KDBG: do_one_ ini tcal 1 :801: tn_name: i2c_adap_s3c_ ini
    8. 327811] /!KDBG: do_one_ initcal l :801: tn_name: power_supply_class_ mnit
    8. 327909] //KDBG:的_one_ mnitcal l :801: tn_name: hwrnon_init
    8.328006] /!KDBG: do_one_ initcal l :801: tn_name: watchd四_ mnit

                                                168/ 312
커 널연구회（www.kern이.b기                                                         정재준 內bi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                4. Device Tree 실습   169




    8.3281091 //KDBG: do_one_ initcal 1 :801: fn_name: mmc 나｝It
    8. 3285131 //KDBG: do one initcal I :801: tn name: s2mpsll_clk_ ini t
    8.328710] //KD8G:do_one_ ini tcaI i :801: fn_name: ho i nit
    8.328878] //KDBG: do_one_ initcal 1 :801: fn_name: init soundcore
    8.328979] //KDBG: do_ono_ initcal l :801: fn_name: alsa_sound_init
    8.3290421 Advanced Linux Sound Architecture Driver Initial ized.
    8.3290601 //KDBG: do_one_ ini cal l :801: tn_name: proto_init
    8.3290931 IIKDB0: do_one_ ini  cal 1 :801: fn_name: net_      dev_   init
    8.3301861
               i ir쓰叩咀삐甲비甲o,iji                 . in小name. neign_Inli
    8.330212] ,, 八L,ou. oo oneHInI 가caI I . oul . Tn_name. geni_InI t

//do. jnitcal l_ IeveiO: 5: fs. . .
      8.3302521 //KDBG: do_ initca1匕1oveI : 870: [tsl
      8. 3303121 !/KDBG: do_ one 나｝i thaI 1 :801: tn_name: 아oc工pu_ mnit
      8. 330341] //KDBG: do one initbal l : 801: fn name: dma_debug_do_ mni
      8.330364] /fcuI Ij:ao_ one_InIipaI I .eui: in iame ' al ignment_ ini I
      8.3303951 //KDBG: do_one_ inithal l :801: tn_name: 이 oc陌에roe由ne少oot rng
      8.3304721 Switched to clocksource mct- frc
      8. 330493] //KDBG:do_one_ initcal 1 :801: tn_name: mnit_pipe_Is
      8.3305631 //KDBG: do_one_ initI1al I :801: fn name: evontpol I_ mnit
      8.330601] //KDBG: do one inital l :801: In name: anon_ mnode_mni t
      8.3306641 IIrL)bT . cTo_one_ 나）I Ical i :801: In name: 아0（乙cmdl ine mni t
      8.3306981 //KDBG: do_one_ ini tcai I :801: In name: 마oc下ons이 es_ in it
      8. 330729] //KDBG: do_one_ initcal I :801: tn name: 아oc下川 into_ mni I
      8. 330760] //KDBG: do one initcal ! :801: tn_name: Proc_deVces_ init
      8.3307921 //KDBG:do_one_ initcai I :801: fn name: 아oc_ interru이 $ mnit
      8.330824] IIKDB0: do_one_ initcal 1 :801: In name: 아oc그 oada四m ni I
      8. 3308561 //KDBG: do one initcal l :801:
                                              下name:
                                                              proc_meminlo_init
      8.330886] //KDBG: do_one_ ini tcal I :801: tn name: 아oc_stat_ ini t
      8.330917] //KDBG: doone ini tcal 1 :801: tn_name: 아oc I叩time_ in it
      8.330949] //KDBG: do_one_ ini tcal 1 :801: fn name: F玎oc中v아引on_ in it
      8.330980]
                  IIKDBG겨山익叫，叫 뗀01: tn_name: 아oc釣ftirqs_ mnit
      8.331011] /f八uDU. aO_orle_ IFII t U町 1 .OW. fn_name: 아oc小msg_ in it
      8.331042] /!KDBG: do_one_ ini tc 1 1 :801: In name: proc_page_ in It
       8.331081] I! KDBG: do one initc I I :801: fn name: mni t_ramnfs_ts
       8.3311031 /IKDBG:由巾陀_ ini tc I I :801: fn name: blkscsi ioctl m it
       8.331123] /IKDBG: do_one_ ini tcs I I :801: fn_name: lb凹nso沌 m it
       8.3313821 //KD80: do_one_ 나litcal I :801: fn name: 引m口 m化．. mnit
       8.3316721 //KDBG:doono initcal l :801: tn name: chr dev 1nit
       8.3508851 //KDBG: do_one_ initca三 I :801: fn name: f irm싸are 이ass 나｝It
       8.3509141 / !KDBG: do one_ in I tca I 1 :801: In name: thermal mnit
       8.353010] //KDBG: do_one_ initcal I :801: fn name: sysct I_core_ mnit
      8.3530751 //KDBG: do one initca.l I :801: tn_ name: eth oft load mnit
      8.353101] //KDBG: do_one_ initca ': I :501: tn_name: mnet m }it
       8.3531881 NET: Registered protocol fami ly 2
       8.3536581 /!KOBG:kthreadd:514: create.kthread(create) . . .
       8.3539971 TCP establ ished hash table entries: 8192 (order: 3, 32768 bytes)
       8.3541091 TCP bind hash table entries: 8192 (order: 5, 163840 bytes)
       8.354311] TCP: Hash tables configured (establ ished 8192 bind 8192)
       8.3543671 TCP: reno registered
       8.354386] UDP hash table entr ies: 512 (order: 2, 24576 bytes)
       8.354435] UDP-Lite hash table entries: 512 (order: 2, 24576 bytes)
       8.354694] !/KDBG: do_one_ initcal i :801: In_name: ipv4_offload_init
       8.354722] //KDBG: do one initca니:801: Inname: af_unix_ init
       8.354749] NET: Registered protobol tami ly 1
       8.354789] !/KDBG: do_one_initcal i :801: tn_name: 1pv6_olt load_ m it

                                                       169/ 312
커널연구회佃w比kern이b기                                                                 정재준 畇b日307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                        4. Device Tree 실습   ]70




     8. 3548161 //KDBG: do_one_ initcal l :801: tn_name: populate_rootfs
     8. 3550831 Trying to unpack rootfs image as initramfs. . .
     8. 3555991 rootfs image is not ini tramfs (no cpio magic) ; looks l ike an initrd
     8. 459941] Freeing ini trd memory: 32768K (c1000000 中 c3000000)

/!do_ i n 1 比al l그ev이 ( ) : 6: device. . .
     8. 459958] //KDBG: do_ initcal l_ level :870: [deviCe]
     8. 4600321 /IKDBG: do_one_ ini tcal 1 : 801: I,｝叫name: bL_switch아dum町i t m it
     8. 4603851 //KDBG: do_one_ ini teal 1 :801: in name: 아xec把mains_ in 1 t
     8. 460425] //KDBG: do_one_ ini teal 1 :801: tn_name : oresources m it
     8. 460504] //KDBO: do_one_ ini tcal 1 :801: In name: 나ii t_sched_由加gj玎odfe
     8. 460532] !JKDBG: do_one_ ini tcal 1 : 801: In name: i rQ_g乙nit叩S
     8. 460553] //KDBG: do_one_ ini teal 1 :801: in name: 1 rq小口［n nit o口5
     8.460572] //KDBG: do_one_ ini teal 1 :801: In name: init_posix_ timers
     8. 460618] //KDBG: do_one_ ini tcal 1 :801: In name: mrli t_ 兀引凡C四_t imers
     8. 4606371 //KDBG: do_one_ ini tcal l :801: fn name: timekeeping忖tni t_o口S
     8. 460657] //KDBG: do one iriitcal l :801: fn name: mnit이 ocks이玎ce S叩is
     8. 461113] //KDBG: do_one_ ini teal 1 :801: In name: mnit_tim아l ist中口rocts
     8. 4611411 //KDBG: do_one_ ini teal 1 :801: In name: alarstimer nit
     8. 461638] //KDBG: do_one_ ini tcal 1 :801: tn_name: clockevents_ ini t_systs
     8. 463612] I/ KDBG: do one initcal l :801: fn name: sched_c I ock_syseor e_ in it
     8. 4636361 //KDBG: do_one_ ini tcal 1 :801: tn_name: tutex 나｝i t
     8. 463660] futex hash table entr ies: 2048 (order: 5, 131072 bytes)
     8. 463754] / /KDBG: doone_ in it cal 1 :801 : tn name: 아oc_m叱비es_ in it
     8. 463782] //KOBG: do_one_ ini teal 1 :801: tn_name: kal isyms_init
     8. 463809] //KDBG: do_one_ ini teal 1 :801: tn_name: pid_namespaces_ ini t
     8. 463846] //KDBG: do_one_ ini teal 1 :801: tn_name: utsname_sysctl_ init
     8. 463894] I/ KDBG: doone mni teal 1 :801: tn_name: init_per_zone_wmark_min
     8. 4639761 //KDBG: do_one_ ini teal 1 :801: tn_name: kswapd_init
     8. 4640081 //KDBG:kthreadd: 514: create_k t hr ead( cr eat e) . .
      8. 464113] /IKDBt3: do_one_ in i tcal 1 :801: in_name: exttrag_debug_ init
     8. 464176] //KDBG: do_one_ initcal 1 :801: fn_name: setup_vmstat
     8. 464230] //KOBG: do_one_ ini teal 1 : 801: tn_name: mm_compute_batch_ mni t
      8. 464252] //KDBG: do_one_ ini teal 1 :801 : tn_name: 51 b少이乙m it
      8. 464280] //KDBG: do_one_ ini tcal i :801: tn_name: workingset_init
      8. 464303] I/ KOBG: do_one_ ini teal 1 :801: tn_name: proc_vmal loc_init
      8. 464334] //KDBG: do_one_ ini teal 1 :801: tn_name: memblock_ ini t_debu아s
      8. 464402] !/KDBG: do_one_ ini tcal 1 :8（川 : tn_name: 아ocs邪叩s_ in it
      8. 464432] //KDB13: do_one_ ini tcal 1 :801: in_name: slab_systs_ ini t
      8. 482026] 사KDBG : d아on已.ini t cal 1 :801: In name: tentl ! nit
      8. 482073] //KOBG: do_one_ initcal 1 :801: In尸n帥e: 아oc_t i lesystems_ ini t
      8. 482107] /!KDBG: do_one_ initcal 1 : 801: tn_name: star t_di rtyt ime_wr i teback
      8. 482135] //KDBG: do小one_ ini tcal 1 :801: in name: dio 1 nit
      8. 482179] //KDBG: do_one_ ini teal 1 :801: tn_name: tsnotity_rnark_ Enit
      8. 482209] //KDBG:kthreadd:514: create_kthread( create) . . .
      8. 482303] //KDBG: do_one_ ini tcal 1 :801: tn_name: dnotity_ inht
      8. 4827031 //KDBG: do_one_ initcal 1 : 801: tn_name: inotit3乙us아 setu口
      8. 4827491 //KDBG: do_one_ mnitcal 1 :801: tn_name: ale_setup
      8. 4828491 //KDBG: do_one_ iai teal 1 : 801: tn_name: proc_ locks_ mni t
      8. 482883] //KDBG: do_one_ ini teal 1 :801: tn_name: mni t_mbcache
      8. 482909] !/KDBG: do_one_ initcal 1 :801: tn_name: init_dev口四is
      8. 482996] //KDBG: do_one_ ini tcal 1 :801: tn_name: init_ext3_ fs
      8. 4833941 //KDBG: do_one_ initcal 1 : 801: in_name: init_ext2_fs
      8. 483770] //KDBG: do_one_ ini teal 1 : 801: fn_name: ext4_init_is
      8. 485649] //KDBG: do_one_ ini tcal 1 :801: tn_name: journal_ in1t
      8. 486425 1 I/ KDBG: do_one_ ini teal 1 :801: tn_name: journal_ m it

                                                    170 / 312
커 널 연구회（www.kernel.b기                                                             정재준 (r야)i3307@nate.com)
Device 가ee 상세분석 in 니nux Kernel 4.0                                             4. Device Tree 실습    ]71




    8.486908] //KDBG: do_one_ intcaH:801: fnm.name: 吼cramfs_ts
    8.486959] //KDBG: do_one_ ini tcaH:801: tn_name: initjat_ fs
    8.4876661 //KDBG: doone ini tcaH:801: tn name: init vfat fs
    o.4o(OJIJ iirsL)15u. ao_one_ inlfcaiLoui : in_name: iriii_msaos_is
    8.487726] IiKDBG: do one ini cal l :801: fn name: m it nls co437
    a.40(Io.jl /t\ uau. aoone inhtcal i .aui: in name: !nit nis asci i
    o.'mHIi3J ,nwau: oo_one_ inI (cai i :oui : rn_name. nit_nis_ isoaooi_i
    8.487806] //KDBG: do_  pne_ mni 겋cal l :801: fn_name: nit_romfs_fs
    8.487824] romts: RO싸S MID (1C) 2007 Red Hat. Inc.
    8.488192] /IKDBG: do_one_ mnitcal l :801: fn_name: i pc_ m it
    8.488236] //KDBG: do_one_ initcaI l :801: tn_name: ipc_sysctl_init
    8. 488274] //KDBG: do_one_ initcal l :801: tn_name: crypto_algapi_ ini t
    8. 488300] //KDBG: do_one_ initcal l :801: tn_name: chainiv_module_ init
    8.488320] //KDBG: do_one_ initcai l :801: fn_name: eseqiv_module_init
     8.488340] //KDBG: do_one_ initcaH:801: tn_name: sha256_generic_mod_init
     8.488370] //KDBG:kthreadd:5141: create_kthread(create) . . .
     8. 488502] !/KDBG:kthreadd:511: create_kthread(create) . . .
     8.488625] //KDBG: do小one_ mnit4aI 1 :801: tn_name: crypto_cbc叫module_init
     8. 488644] //KDBG: do_one_ mnit4aI 1 :801: tn_name: aes_init
     8.488671] //KDBG:kthreadd: 514: create小k卄）read(create) . .
     8.488780] !/KDBG: do_one_ initcal l :801: tn_name: crc32c_mod_init
     8.488807] //KDBG:kthreadd:514: create_kthread(croate) . .
     8. 488916] //KDBG:do_one_ initqal 1 :801: tn_name: krng_mod_init
     8.488945] //KDBG:kthreadd: 514t: create_kthread(create) . .
     8. 489053] //KDBG: do_one_ initc뇨I i :801: fnname: .proc_genhd_ ini t
     8.489087] //KDBG: do_one_ mnitc目l l :801: tn_name: nit_emergency_pool
     8.489151] bounce: pool size: 64 pages
     8.489164] /!KDBG: do_one_ initcbl l :801: tn_name: noop_ init
     8.4891印］ io scheduler noop registered
     8.489194] //KDBG: do_one_ ini tcal 1 :801: fn_nanre: deadi mrle_ mni I
     8.489209] lo scheduler deadl ine registered
     8.489223] //KDBG: do_one_ initcaH:801: tn_name: cfq_init
     8.489964] io scheduler ctq registered (default)
     8.489984] f/KDBG: do_one_ initcal l :801: tn_name: percpu_counter_startup
     8. 490007] //KDBG: do_one_ ini tc串 1 : 801: tn_name: phy_core_ ini t
     8.4901化］ //KDBG: do_one_ initcai l : 801: tn_name: exynos_dp_video_phy_dr 沁er_init
     8.490896] //KDBG: do_one_ mni tca j : 801: fri叫name: exynos_mipi_video_phy_driver_ inil
     8. 4910601 exynos-mipi-video-phy 10040714. video-phy: regmap lookup tai led: -19
     8.491083] exynos-mipi-video-phy 10040714. video-phy: can 't request region for resource [mem
0x10040714-0x1004071 f I
[    8.491111] exynos-mipi-video-phy: probe of 10040714. video-phy tai led with error -16
1    8.491284] //KDBG: do_one_ initca 1 :801: fn_name: samsung. usb2_口hy_driverminit
     8.492537] //K아G:do_one_ ini Ica 1 : 801: tn_name: exynos5_usb3drd_phy_ ini
     8.492853] 12100000.phy supply vbus not found, using dummy regulator
     8. 492934] 12100000.phy supply vbus-boost not found, using dummy regulator
     8.493572] 12500000.phy supply vbus not found, using dummy regulator
     8.493647] 12500000.phy supply vbus-boost not found, using dummy regulator
     8.494265] //KDBG: do_one_ ini tcal 1 :801: fn小na用e: 口卄ii｝느samsung_dr iver_ ini I
     8.494962] //KDBG: do_one_ initcal 1 : 801: fn..naine: platform_ lcd_driver_ mnit
     8.495212] /IKDBG: do_one initcal 1 :801: tn_name: goner icb I_dr iver_ ini t
     8. 495403] //KDBG: do_one_ initcal I :801: tn_name: pwm_backl i phI_dr iver_init
     8. 4956521 /!KDBG: do_one_ ini tcal 1 :801: tn_name: exynos_mipi_dsi_dr iver_ ini t
     8. 495846] /!KDBG: do_one_ ini tcal 1 :801: tn_name: p1330_dr iver_init
     8.499668] dma-p1330 3880000.adma: Loaded driver for PL330 DMAC-241330
     8. 4996861 dma-p1330 3880000.adma: DBUFF-4x8by1es Num_Chans-6 Num_Peri-16 Num_Events-6
     8.506884] dma-p1330 121a0000. pdma: Loaded driver for PL330 DMAC-241330

                                              171/ 312
커 널 연구회（www.kerne나끄）                                                    정재준 內bi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                      4. Device Tree 실습          172




[
           8. 506901] dma-p 1330 121a0000 . pdma:        DBIJFF-32x4bytes Nurn_Chans-8 Num_Per -32 Num_Events-
n
/L

           8. 5141591 dma-p1330 121b0000.pdma: Loaded driver for PL330 DMAC-241330
nd r L r
       [

n亡
           8.5141761 dma-p 1330 121b0000 . pdma:       DBUFF-32x깎）ytes Num_Chans-8 Num_Per i -32 Num_Events-
八＜
 U



            8.5161601 dma-p 1330 10800000 .mdma: Loaded dr i ver for PL330 DMAC-241330
            8.5161771 dma-p 1330 10800000.mdma:              DBUFF-64x8bytes Num_Chans-8 Num_Per i-i Num_Events-32
            8.5163291 //KDBG: do_one_ initcal 1 :801: tn_name: max77693小pmic_driver_init
            8. 516533] //KDBG: do_one_ initeal 1 :801: tn_name: max77802_ pmic_driverjnit
            8.516733] /IKDBG: do_one_ initeal l :801: tn_name: s2mpaol_pmic_driver_ init
            8.5］的28] //KDBG:do_one_ ini teal 1 :801: tn_name: pty_ ini t
            8.640382] //KDBG:do_one_ initeal t :801: tn_name: sysra_init
            8.640428] //KDBG:do_one_ initcal l :801: tn_name: seria18250_ ini t
            8.640447] Serial : 8250/16550 driver, 4 ports, lRQ sharing disabled
            8.642867] //KDBG: do_one_ initcal l :801: fnname: sanisung_serial_driver_ init
            8.643115] 12c00000.serial : ttySAC0 at MMI0 0x12c00000 ( irq = 58, base_baud      0)   is a S3C6400/10
            8.6437611 12c10000.serial : ttySAC1 at MMI0 0x12e10000 ( irq = 59, base_baud      0)   is a S3C6400/10
            8.6443891 12e20000.serial : ttySAC2 at MM山 0x12e20000 ( irq = 60. base_baud       0)   is a S3C6400/10
            8.6450121 12c30000. serial : ttySAC3 at MM山 0x12c30000 ( irq = 61, base_baud      0)   is a S3C6400/10
           10.0312631 //KDBG:kthreadd:514: create_kthread(create) . . ,
           10.0313491 //KDBG:kthreadd: 514: ereate_kthread(create) . . .
           10. 031422] //KDBG:kthreadd: 514: create_kthread(create) . . .
           11.2702921 console tttySAC31 enabled
           11.274780] //KDBG: do_one_ ini tcal 1 :801: fn_name: of_platform_serial_dr iver_ init
           11.281670] //KDBG: do. 0ne_ ini teal 1 :801: tn_name: hwrng_jnodinit
           11.2872751 //KDBG:do_one_ ini teal 1 :801: tn_name: exynos_rng中dr ivor_ ini
           11.2937961 //K080: do_one_ ini teal 1 :801: tn_name: mng_ mni t
           11.298966] //KDBG: do_one_ ini teal 1 :801: tn_name: tprn_ tis_ i2c_driver_init
           11.3057891 //KDBG: do_one_ ini teal 1 :801: fn name: dun core mnit
           11 .引佰871 [drml Initial ized drm 1.1.0 20060810
           11.3化0311 /!KDBG: do_one_ ini teal 1 :801: tn_name: exynos_drm_ini
           11.323127] IiKDBG: doone initeal l :801: tn_name: panel_simple_ mnit
           11.328693] //KDBG:do_one_ ini teal 1 :801: tn_name: ptn3460_dr iver_ ini t
           11.334645] //KDBG: do_one_ ini teal 1 :801: tn_narne: t야刈ogy_s邱治mm it
           11.341099] //KDBG: do_one_ ini teal 1 :801: tn_name: cachemnto_systs_ init
           11.347229] //KDBG: c幻_one_ ini teal 1 :801: tn name: brd init
           11.353767] brd: module loaded
           11.3556281 IIKDBG:do_one_ ini teal 1 :801: tn_name: loop_ m it
           11.361422] //KOBG:kthroadd: 514: ereate_kthread(ereate) . . .
           11 .366651] //KDBG:kthreadd: 514: ereate_kthread(ereate) . . .
           11.381655] loop: module loaded
           11.3833331 //KDBG:do_one_ initcal 1 :801: tn name: 1nit工四야이 00口
           11. 389316] //KDBG: do_one_ initeal 1 :801: fn name: eros_ee_dr iver_ ini t
           11.395793] //KDBG: do_one_ ini teal 1 :801: tn name: 아os_ec_dr iv아小5口匕nit
           11.4024581 //KDBG: do_one_ initeal 1 :801: tn name: mnit sd
           11.4078801 //KDBG: do_one_ initeal 1 :801: tn name: mni t_sg
           11. 413063] //KOBG: do_one_ ini teal 1 :801: fn name: s3e64xx_sp i_dr i ver_ i nit
           11 .419947] //KDBG:do_one_ ini teal 1 :801: fn name: net olddevs mnit
           11.4256651 !/KDBG: do_pne_ initeal 1 :801: tn_name: Sn侶c91似 mnit modum
           11.4323081 //KDBG:do_one_ initeal l :801: tn_name: asix_driver_ init
           11.4382611 usbeore: registered new interface driver asix
           11. 443501] //KDBG: do_one_ ini teal 1 :801: tn_name: ax88179_178a_driver_ init
           11.4503641 usbcore: registered new interface driver ax88179_178a
           11.456325] //KDBG: do_one_ initeal l :801: tn_name: ede_driver_init
           11.4624291 usbeore: registered new interface driver edc_ether
           11.468079] //KDBG: do_one_ initeal 1 :801: tn_name: smsc75xx_driver_init

                                                       172 / 312
커 널 연구회（www.kernel.b기                                                              정재준 四bi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                           4. Device Tree 실습      173




   11.474684] usbcore: registered new interface dr iver 5m5c75xx
   11 .480211] //KDBG: do one initcal l :801: in name: 5m5c95xx driver m it
   11.486814] usbcore: registerd new interface dr iver sm5c95xx
   11 .492373] //KDBG: do_one_ ini teal ! :801 : fe_name: net1080 driver 나lit
   11 .498794] usbcore: registered new interface dr iver net1080
   11.504332] /IKDBG: doone initcal i :801: in name: cdc_subseLdriver_ ini t
   11 .511048] usbcore: registered new interface dr iver cdc subset
   11.516779] //KDBG: do'one_ ini teal 1 : 801: fn_name: zaurus driver m！기t
   11.523177] usbcore: registered new interface dr iver za（玎 us
   11.528563] //KDBG: do one init,cal l : 801: fnname: usbnet nit
   11 .534244] I/ KDBG: do one mnl teal 1 :801: fn name: cdcncm driver 1nit
   11.540713] usbcore: registered new interface di iver cdc ncm
   11.546154] //KDBG: do_one_ mnitcal 1 : 801: frLname: dwc3 driver m } u t
   11.552509] //KDBG: do_one_ ini teal 1 :801: fnname: d싸c3_exynos_dr 山아1r기 t
   11.559694] usb@12000000 supply vdd33 not found, using dummy regulator
   11.565498] usb12000000 su口p四 vddl0 n아 化und, using dummy regulator
   11.9757131 usb@12400000 supply vdd33 not found, using dummy regulator
   11.980857] usb@12400000 supply vdd伯 not found, using dummy regulator
   12. 388887] IIKDBG:do工ne_ in i比al l :801 : fn中name: xhc匕히at nit
   12.393650] xhci-hcd xhci-hcd. 2. auto: xHCl Host Control ler
   12.398812] xhci-hcd xhci-hcd.2 'auto: new USB bus registered, assigned bus number 1
   12.406790] xhci-hcd xhci-hcd. 2. aulo: hcc params 0x0220104c hci version 0x100 quirks 0x00010010
   12. 415169] xhci-hcd xhci-hcd. 2. auto: irq 108, io mem 0x12000000
   12.421303] usb usbi: New USB device found, idVendor=ld6b, idProduct=0002
   12. 427810] usb usbi: New IJSB device strings: Mfr=3, Product=2, SerialNumber=1
   12.435033] usb usbi: Product: xHCl Host Control ler
   12.439854] usb usbi: Manufacturer : Linux 4.0.0 xhci-hcd
   12.445169] usb usbl: SerialNumber: xhci-hcd.2.auto
   12.451089] hub 卜0녀 . 0: USB hub found
   12.453752] hub 1-0:1.0: 1 port detected
   12.458201] xhci-hcd xhci-hcd. 2. auto: xHCl Host Control ler
   12.463132] xhci-hcd xhci-hcd. 2. auto: new USB bus registered, assigned bus number 2
   12.470986] usb usb2: New USB device found, idVendor=ld6b, idproduct=0003
   12.477463] usb usb2: New USB device strings: Mfr=3, Product=2, SerialNumber=1
   12.484686] usb usb2: Product: x卜ICI Host Control ler
   12.489507] usb usb2: Manufacturer: Linux 4.0.0 xhci-hcd
   12.494821] usb usb2: SerialNumber: xhci-hcd.2.auto
   12.5007261 hub 2-0:1.0: USB hub found
   12.503407] hub 2-0:1.0: 1 port detected
   12.507957] xhci-hcd xhci-hcd. 5. auto: xHCl Host Control ler
   12. 5127961 xhci-hcd xhci-hcd. 5. auto: new USB bus registered, assigned bus number 3
   12.520744] xhci-hcd xhci-hcd. 5. auto: hcc params 0x0220f04c hci version 0x100 quirks 0x00010010
   12.529076] xhci-hcd xhci-hcd. 5. auto: irq 109, io nem 0x12400000
   12. 535234] usb usb3: New USB device found. idVendor=ld6b, idProduct==0002
   12. 541792] usb usb3: New USB device strings: Mfr=3, Product=2, SerialNumber=1
   12.548951] usb usb3: Product: xHCl Host Control ler
   12.553958] usb usb3: Manufacturer: Linux 4.0.0 xhci-hcd
   12.559090] usb usb3: SerialNumber: xhci-hcd.5.auto
   12. 565005] hub 3-0:1.0: USB hub found
   12.567702] hub 3-0:1.0: 1 port detected
   12. 572196] xhci-hcd xhci-hcd. 5. auto: xHCl Host Control ler
   12. 577048] xhci-hcd xhci-hcd.5. auto: new USB bus registered, assigned bus number 4
   12.584935] usb usb4: New USB device found, idVendor=ld6b, idProduct=0003
   12.591444] usb usb4: New USB device strings: Mfr=3, Product=2, SerialNumber=1
   12.5986041 usb usb4: Product: xHCl Host Control ler
   12.603639 1 usb usb4: Manufacturer: Linux 4.0.0 xhci-hcd

                                             173/ 312
커 널 연 구회佃wa床ernel.b기                                                   정재준 (rgbi3307（亘）nate.com)
Device Tree 상세분석 II) 니nux Kernel 4.0                                            4. Device Tree 실습   ]74




[     12.608743] usb usb4: SerialNumber: xhci-hcd.5.auto
[     12.6146781 hub 4-0:1.0: USB hub found
[     12.617354] hub 4-0:1.0: 1 port detected
[     12.6219701 i/ KDBG: do_one_ initcal l : 801: tn_name: ehci_hcd_init
[     12.6270331 ehci_hcd: tJSB 2.0 'Enhanced ' Host Control ler (EH기) Driver
[     12.633567] //KDBG: do_one_ initcal l :801: tn_name: ehci_exynos_ ini t
[     12.639598] ehci-exynos: EH기 EXYNOS driver
[     12.644237] exynos-ehci 12110000.usb: EHCI Host Control ler
[     12.649242] exynos-ehci 12110000.usb: new USB bus registered, assigned bus number 5
[     12.6570831 exynos-ehci 12110000.usb: irq 107, io mem 0x12110000
[     12.6805171 exynos-ehci 12110000.usb: USB 2.0 started, EHCI 1.00
[     12.6852511 usb usb5: New USB device found, idVendor=ld6b, idProduct=0002
[     12.6918351 usb usb5: New USB device strings: Mfr=3, Product=2, SerialNumber=1
[     12.698993] usb usb5: Product: EHCI Host Control ler
[     12.703875] usb usb5: Manufacturer: Linux 4.0.0 ehc匕hcd
[     12.709131] usb usb5: SerialNumber: 12110000.usb
[     12.714793] hub 5-0:1.0: USB hub found
[     12.717484] hub 5-0:1.0: 3 ports detected
[     12.722695] //KDBG: do_one_ ini tcal 1 :801: tn_name: ohci_hcd_mod_ ini t
[     12.727596] ohci_hcd: USB 1.1 'Open ' Host Control ler (아기) Driver
[     12.7337951 !/KDBG: do_one_ ini tcal 1 :801: fn_name: ohci_exynos_ ini t
[     12.7398141 ohci-exynos: OHCI EXYNOS driver
[     12.744291] exynos-ohci 12120000.usb: IJSB Host Control ler
[     12.749370] exynos-ohci 12120000.usb: new USB bus registered, assigned bus number 6
[     12.757128] exynos-ohci 12120000.usb: irq 107, io mem 0x12120000
[     12.824917] usb usb6: New USB device found, idVendor=ld6b, idProduct=0001
[     12.830224] usb usb6: New USB device strings: Hfr=3, Product=2, SerialNumber=1
 [    12.837446] usb usb6: Product: USB Host Control ler
 [    12.842207] usb u5b6: Manufacturer: Linux 4.0.0 ohci hcd
 [    12.847466] usb usb6: SerialNumber: 12120000.usb
[     12.8531261 hub 6-0:1.0: USB hub found
 [    12.855818] hub 6-0:1.0: 3 ports detected
 [    12.860792] //KDBG: do_one_ initcal 1 :801: tn_name: xhci hcd mnit
[     12.865593] //KDBG: do_one_ initcal 1 :801: tn_name: usb_storage_dr iver...ini t
 [    12.872526] usbcore: registered new interface di iver usb-storage
1     12.878236] //KDBG: do_one_ in나cal 1 :801: tn_name: usb3503 mnit
1     12.884374] //KDBG: do_one_ initcai l :801: tn_name: serport_ init
 [    12.889682] //KDBO: do_one_ initcal 1 :801: tn_name: mousedev m} it
 [    12.896094] mousedev: PS/2 mouse device common for al l mice
 [    12.901059] //KDBG: do_one_ initcal l :801: tn_name: evdev_init
 [    12.9065801 //KDBG: do小one_ ini tcal 1 :801: tn_name: atkbd_ini t
 [    12.912314] !/KDBG:的＋ne_ initcal 1 : 801 : fn－小name: 아Os ec如沁_dr i ver小nit
 [    12.919129] 사KDBG : d町ne_ mni tcal 1 :801 : fn牛name: samsung小ey口ad出 !ver_init
 [    12.926244] //KDBG: do_one_ initcal l :801: tn_name: cyapa_driver_ init
 1    12.9321211 //KDBG: do_one_ in汁cal l :801: tn_name: mxt_driver_init
 [    12.938061] //KDBG: dq..one_ mnitcal l : 801: tn_name: max77686_rtc_driver_init
 [    12.944925] //KDBG: do_one_ inmtcal l :801: fn_name: max77802_rtc巾driver_init
 [    12.951521] /IKDBG:kthreadd:514: create_kthread(create) . , .
 [    12.951933] //KDBG: do_one_ initcal l :801: tn_name: s3c_rtc_driver_init
 [    12.9524101 53c나tc lOle0000. rtc: fai led to find rtc source clock
 [    12.952474] s3c-rtc: probe of 101e0000. rtc fai led with error -2
 [    12.953057] !/KDBG: do_one_ initcal l :801: fn_name: s5m_rtc_driver_init
 [    12.953530] !/KDBG: do_one_ mnitcal 1 :801: tn_name: i2c_dev_ init
 [    12.953541] 12c /dev entries driver
  [    12.953727] //KDBG: do_one_ initcal l :801: tn_name: exynos5_ i2c_driver_init
  [    12.997430] //KDBG:kthreadd: 514: create kthread(create) . . .

                                               174 / 312
 커 널 연구회（니八사w.kern이.b기                                                   정재준 的bi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                 4. Device Tree 실습   ]75




[
    13.040592] usb 5-1: now high-speed USB device number 2 using exynos-ehci
[
    13.075547] /!KDBG: do_one_ initcal l :801: tnriame: ec_ i2c_ tunneLdriver_ ini t
[
    13.081240] //KDBG: do_one_ initcal l :801:       name: i2c_ arbi trator_      init
[
                                                                      driver_
                                            tn_
    13.088126] //KDBG: do one inifcal i :801: tn_name: sbs_battery_driver_init
[
    13.094701] /IKD8G: do_one_ ini cal 1 :801: tnname: maxll04o_ i2c_driver_ init
[
    13. 1017661 /!KDBG: do_one_      caI l :801: fn_namo: max17042_ i2c_driver_ init
[
                              ini
    13. 108189] //KDBG: do_one_ ini tcaI 1 : 801: tn_name: max14577_charger코r iver_ ini
[
    侃］153901 //KDBG: do_ono_ ini tcaI 1 : 801: tn_name: max77693_charger_dr iver_ ini


rL rt [
    13. 122492] //KDBG: do_one ini t al 1 : 801: tn_name: 1ps65090_charger中dr iver_ ini I
    13.129627] //KDBG: do_one_ initbal I :801: tn_name: Im90_driver_ init
    13.135599] //KDBG: do_one_ ini 比aH:801: tn_name: exynos_tmu_driver_ init
[
    13. 142415] thermal thermal_zoheo: fai led to read out thermal zone (-22)
[
    13.148751] 10060000. tmu supply vtmu not found, using dummy regulator
r
1L [
    13.155500] thermal thermal_zonel: tai led to read out thermal zone (-22)
    13. 161917] 10064000. tmu supply vtmu not found, using dummy regulator
[
    13.1686271 thermal thermal_zone2: fai led to read out thermal zone (-22)
[
    13.174953] 10068000. tmu supply vtmu not found, using dummy regulator
[
    13. 1817211 thermal therma匕zone3: fai led to read out thermal zone (-22)
[
1
    13.188004] 1006c000. trnu supply vtmu not found, using dummy regulator
 =[ [
    13.194960] thermal thermal_zone4: fai led to read out thermal zone (-22)
    13.201167] 100a0000. tmu supply vtniu not found, using dummy regulator
 r
 1L [
    13.207895] usb 5-1: New USB device found, idVendor=05e3, idProduct=0610
    13.214163] usb 5너: New USB device strings: Mtr=0, Product=1, SerialNumber=0



 [L rL rL [
    13.214328] IIKDBG:do one initcal i :801: fnname: s3c241鈿d1 driver init
    13.222229] 53c2410-wdt lold0000.watchdog: watchdog inactive, reset disabled, irq disabled
    13.222598] //KDBG: do_one_ initcal l :801: tn_name: dm_ init
    13.224412] device-mapper: ioctl : 4.30.0- ioctl (2014-12-22) initial ised: dm-devel@redhat.com
 [
    13.224428] //KDBG: do_one_ ini tcbl 1 :801: tn_name: mmc_b泳_ ini
 [
    13.224449] Driver 'mmcblk ' needs updating - please use bus_type methods
 [
    13.224702] //KD8G: doone initcal 三:801: tnnanie: sdhci drv init
 [
    13.224716] sdhci : Secure Digit削 Host Control ler Interface driver
 [
    13.224724] sdhci : Copyright (c) Pierre 0ssman
 [
    13. 224738] //KDBG: do_one_ initcal i :801: tn_name: sdhci_s3c_driver_init
 [
    13.225388] !/KDBG: do_one_ initcal l :801: tn_name: dw_mci_ inii
 [
    13.225401] Synopsys Designware Multimedia Card Interface Driver
 [
    13.225416] //KDBG:的巾ne_ init凋1 1 :801: in_name: d叱叩匕이 tt兀山 ver_ in나
 [
    13.226050] //KDBG: do_one_ initcall l :801: tn_name: dw_mci_exynos_pltfm_driver_init
 [
    13.2270401 dwmmc_exynos 1220000t .mmc: num-slots property not found, assuming 1 slot
 [
    13.2272321 dwmmc_exynos 12200000.rnmc: IDMAC supports 32-bit address mode.
[   13.227352] dwmmc_exynos 12200000. rnmc: Using internal DMA control ler.
[   13.227369] dwmmc_exynos 12200000. rnmc: Version ID is 250a
[   13.227517] dwmmc. exynos 12200000. rnmc: DW MMC control ler at irq 87, 64 bit host data 州 (Jth, 64
deep fifo
[   13.236410] dwmmc_exynos 12200000. mmc: No vqmmc regulator found
    13.290774] dwmmc_exynos 12200000.mmc: 1 slots initial ized
    13.2914811] d州mmc_exynos 12220000. rnmc: num-slots property not found, assuming 4 引아
    13.2916591 dwmmc_exynos 12220000.mnic: IDMAC supports 32-bit address mode.
    13.291784] dwmmc_exynos 12220000.mmc: Using internal DMA control ler.
    13.291800] dwmmc_exynos 12220000. mmc: Version ID is 250a
    13.291946] dwmmc_exynos 12220000.mmc: OW MMC control ler at irq 88, 64 bit host data width, 64
deep tito
[   13.293308] //KDBG:kthreadd: 514: ;   七：reate_kthread(create) . . .
[   13.401440] usb 5너: Product: USB2.0 Hub
[   13.408074] hub 5너:1.0: USB hub found
[   13.410587] dwmmc_exynos 12220000.mmc: 1 slots initial ized
[   13. 410840] hub 5너:1.0: 4 ports detected

                                                  175 / 312
커 널 연구회（www.kern이.b기                                                            정재준 (rgb日307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                           4. Device Tree 실습   176




     13. 420102] //KDBG: do_one_ ini tcal 1 :801: tn_name: hid_ in t
     13.425401] //KDBG: do. ..one_ initcal l :801: tn_name: hid_generic_ mnit
     13.431428] //KDBG: do_one_ mnitcai l :801: fri_name: a4_driver_ init
     13.437287] //KDBG: do_one_ initcal l : 801: tn_name: appledriver_ ini t
     13.443490] //KDBG: do_one_ initcal l : 801: fnmname: belkin_driver_ init
[    13.443959] mmcO: MAN_BKOPS_EN bit is not set
[    13.444723] mmc_host mmco: Bus speed (slot 0) = 50000000Hz (slot req 52000000Hz, actual
50000000HZ div = 0)
[    13.445108] mmc_host mmco: Bus speed (slot 0) = 100000000Hz (slot req 52000000Hz, actual
50000000HZ div = 1)
     13.445229] mmc0: new 0DB 씨C card at address 0001
     13.4507351 //KDBG:kthreadd:514: create_kthread(create) . . .
     13.450893] mmcb1k0: mmc0: 0001 M8G1WA 7.28 GiB
     伍451065] //KDBG:kthreadd:514: create_kthread(create) . . .
     13. 451222] mmcb나；ObootO: mmco:000l M8G］卄A 口artit 泊n ] 2.00 씨B
     13. 451372] //KDBG:kthroadd: 514: create_kthread(create) . . .
     13. 451515] mmcblkobootl: mmco: 0001 M8G1WA partition 2 2.00 NiB
     13.451671] //KDBG:kthreadd: 514: create_kthread(creato) . . .
     13.451814] mmcblkorpmb: mmc0: 0001 N8G1WA partition 3 128 KiB
     13.461294] mmcblko: p1 p2 p3 p4
     13.509675] nmc小ost mmc1 : Bus s口eed （引아 0) = 50000000Hz (slot req 50000000Hz, actua
  0000000HZ div =0)
     13.5097971 mmcl: new high speed SDHC card at address b368
     13 .引0864] //KDBG:kthreadd:514: create_kthread(create) . .
     13.511057] mmcblkl: mmcl :b358             3.71 GiB
     13. 513911] 때；icb I ki : p] 口2 口3 p4
     13.553713] //KDBG: do_one_ ini tcal 1 : 801: in name: ch_dr iver_init
     13.5595721 !/KDBG: do_one놔ini tcal 1 : 801: fn_name: ch_dr ver_ ini t
     13. 565494] //KDBG: do_one_ ini tcal 1 : 801: in name: cp_dr iver_ init
     13.5713861 //KDBG: do_one_ ini tcal 1 :801: fn name: ez driver m u t
     13.577251] !/KDBG: do_one_ ini tcal 1 :801: in name: ks driver 나｝it
     13.583171] //KDBG: do_one_ ini tcal 1 : 801: in name: lg_dr iver_ ini t
     13.589042] //KDBG: do_one_ mni tcal 1 :801: in name: ms driver nit
     13.594956] /!KDBG: do_one_ ini tcal 1 :801: fri name: mr_driver_i nit
     13.600849] //KDBG: do_ono_ ini tcal 1 :801: in name: plantronics_dr iver_ ini t
     13.607498] //KDBG: do_one_ ini tcal 1 :801: in name: hid m } it
     13.612963] usbcore: registered new interface driver usbhid
     13. 618352] usbhid: USB HID core driver
     13.622178] /!KDBG: do one initcal ! :801: in name: max77686 c沫 driver init
     13.629089] //KDBG: do_one_ ini tcal 1 :801: tn_name: max77802 c 나（ driver mnit
     13.635847] //KDBG: do_one_ initcal 1 :801: in name: extcon class i nit
     13.641897] //KDBG: do_one_ initcal 1 :801: in name: max14577 muic driver mnit
     13.648809] !/KDBG:do one mnitcal l :801: in_name : max77693 muic driver mnit
     13.6556841 //KDBG: do_one_ ini tcal 1 :801: in name: exynos_adc_dr iver_ ini t
     13.662537] //KDBG: do_one_ ini tcal 1 :801: in name: alsa timer mnit
     13.668399] //KDBG: do_one_ mni tcal 1 : 801: in name: 키 sa_r兀叱m it
     13.673935] //KDBG: do_one i ni tcal 1 :801: fn name: snd工om아ess_ ini t
     13.680041] /IKDBG: do_one_ ini tcal 1 :801: tn name: snd soc mnit
     13.686435] //KDBG: do_one_ initcal 1 :801: tn_name: max98090_ i2c_dr iver_ ini
     13.6909651 usb 5너 . 4: no닙 high四口eed USB device number 3 using exynos-ehci
     13.6995501 //KDBG: do_one_ ini tcal 1 :801: fn_name: max98095_ i2c_dr iver_ ini t
     13.706317] //KDBG: do_one_ ini tcal 1 : 801: tn_name: samsung_ i2s_dr iver_ ini I
     13. 713236] !/KDBG: do_one_ ini tcal 1 :801: fri_name: asoc_ idma_dr iver_ ini t
     13 . 거9521 ] //KDBG: do_one_ ini tcal 1 :801: fn_name: snow driver mnit
     13.725722] //KDBG: do_one_ ini tcal 1 :801: tn_name: sock_diag_ init
     13.731406] //KDBO: do_one_ ini tcal 1 :801: tn_name: gre_off load_ mnit

                                              176 / 312
커 널 연구회（www.kern이.b기                                                    정재준 (rgb日307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                               4. Device Tree 실습      177




   13.7374291 /!KDBG: do_one_ ini [tcal 1 : 801: tn_name: sysctl_ ipv4_init
   13.7436391 //KDBG: do one initcal l :801: In name: xfrm4 beet mnu t
   伍749455] //KDBG: do_one_ initcal 1 :801: tn_name: xtrm4_ transport_ ini t
   13. 755894] //KDBG: do one initcal l :801: fn name: xtrm4_mode_ tunnel_ ini t
   13. 762477] //KDBG: do one 1 nitcal l :801: fn name: inet_diag_ ini t
   13. 768349] //KDBG: do_one_ initcal l : 801: tn_name: t（耳乙（hag_ m i t
   13.774177] //KDBG: do.,one_ mni Ical 1 :801: tn_name: cubi ctcp_reg i ster
   13. 780319] TCP: cubic registered
   13.783613] !/KDBG: do中one_ mnitcal l :801: tn_name: packet_ mnit
   13.789224] NET: Registered prjotocol fami ly 17
   13.793686] //KDBG: do_one_ initcal l :801: tn_name: ipsec_ 片key_ mnit
   13.7997611 NET: Registered protocol fami ly 15
   13.8025901 usb 5-1.4: New USB device found, idVendor=0b95, idProduct=772a
   13.8026021 usb 5-1.4: New USB device strings: Mtr=1, Product=2, SerialNumber=3
   13.8026131 usb 5-1.4: Product: AX88772
   13.8026241 usb 5-1.4: Manufacturer: ASIX Elec. Corp.
   13.8026351 usb 5-1.4: SerialNumber: 000001
   13.807847] asix 5-1.4:1. 0 (unnamed net_device) (uninitial ized) : inval id hw address, using random

//do_ initcal I_ level) ): 7: late . . .
[   13.840188] //KDBG: do_ir나calLlevel :870: [ late]
[   13.844837] //KDBG: do_one_ init4a1 1 :801: fn中name: nit_machine_ late
[   13.851391] !/KDBl3:do_one_ initcaH:801: fnmname: swp_emulation_init
[   13.857185] Register ing SWP/SWPB emulation handler
E   13.861950] //KDBG: do one 1n1tda1 1 :801: fnmname: bL_swi tcher_ ini
1   13.868000] //KDBG: do_one_ initcal l :801: fn_name: init_oops_ id
[   13.873751] //KDBG: do_one_ initcaH:801: fnmname: sched_ in if_debug
[   13.879793] //KDBG: do小one_ ini tcai i :801: fn_name: p呱叩5_po叫er_ m it
[   13.886865] //KDBG: do_one_ initcaH. :801: fn n계ne: p町debu아s_ in it
[   13.891949] //KDBG: do_one_ initcal l :801: fn name: 口r in作그카e_ in it
[   13.897979] //KDBG: do_one_ initc히l :801: fnHname: tk_由bu吼S陀e口_ t ime_init
[   13.904773] //KDBG: do one initc古l l :801: fn name: faul t_around_debugfs
[   13.9111861 I/ 入ubu: ao_one_ lnIicaI I .bui: in_name. saxj붜a아 i les_出eck
[   13.9174721 /!KDBG: do_one_ i nitc I 1 :801: fn name: prandom_reseed
[   13.9234551 /!KDBG: do_one_ ini tcal 1 :801: tn_name: 化그 ogo_ late_ ini t
[   13.9295181 //KDBG: do one initcal l :801: fn name: deferred_probe_initcal I
[   13.936247] //KDBG:kthreadd: 514:[ create. kthread(create) . . .
[   13.9418561 !/KDBG: do._one_ initc印1:801: fnmname: genpd_poweroff_unused
1 13.948250] //KDBG: do one initca三 l :801: fn놔name: gpio_keys_ init
1   13.948265] //KD8G:kthreadd: 514 create_kthread(create) . . .
1   13.959521] power-domain: Power-off latency exceeded, new value 11343084 ns
[   13.962321] input: gpio_keys as /devices/platform/gpio. keys/ input/ inputo
[   13.9672711 //KDBG: do斗one_ in냐ca! I :801: tn_name: rtc_hctosys
[   13.9672941 /home/ jamesjung/DEV/40_projects/61_exynos5420/20_kernel/ l inux
4.0/drivers/ rtc/hctosys. c: unable t0 open rtc device (rtcO)
[   13.9673101 //KDBG: do_one_ initca: l :801: tn_name: of_ fdLraw_init
[   13.9675211 //KDBG: do_one_ initcal l :801: tn_name: cik_debug_init
[   14.002677] //KDBG:kthreadd: 514: create kthread(create) . . ,
[   14. 002831] power-domain: Power-off latency exceeded, new value 229667 ns
[   14.0030131 power-domain: Power-off latency exceeded, new value 386291 ns
[   14.003047] power-domain: Power-off latency exceeded, new value 183666 ns
[   14.0032661 power-domain: Power-off latency exceeded, new value 184834 ns
[   14.0455771 !/KDBG: do_one_ initcal 1l :801: tn_name: tcp_congest ion_default
[   14.050755] //KDBG: do_one_ initcal l :801: tn_name: regulator_ m it_complete
[   14.059351] random: nonblocking pool is initial ized
[   14.0711161 //KDBG: do_one_initcai l : 801: tn_name: clk_disable_unused

                                              177 / 312
커 널 연구회（w小八사．kernel.b기                                                   정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                             4. Device Tree 실습




    14.0780191 //KDBG:do.one_ initcaH:801: tn_name: alsa_sound_ last_ init
    14.083012] ALSA device l ist:
    14.0859161 No soundcards found.
    14.089322] //KDBG: do_basic_setup:914: The End

[   14.6245201 asix 5-1.4:1. 0 ethO: register ' asix ' at usb-12110000.usb-1.4, ASIX AX88772 USB 2.0
Ethernet, d6:92:b6:5d:63:6a
[   14.6343811 RAMDISK: gzip image found at block 0
[   15.0679891 VFS: Mounted root (ext2 fi lesystem) readonly on device 1:0.
[   15.073326] devtmpfs: mounted
[   15.0760971 //KDBG:kernet_ init_ freeable:1081: The End



{   15.085747] Freeing unused kernel memory: 240K (c0658000 尸 c0694000)
    15.091919] //KDBG:kerne匕init:996: run_ init_process(execute_comrnand)
Starting logging: OK
Initial izing random number generator. . . done.
Starting network. . .

Welcome to Exynos5420




위의 커널 부팅 로그에서 확인할 수 있듯이 디바이스드라이버에 해당하는 코드가 전체 커널 소스
의 80% 이상을 차지한다.               위의 모든 소스를 분석하려면 많은 노력과 시간이 필요하지만, 커널
소스가 실행되는 흐름을 먼저 이해하고 그것의 설계도면부터 그려 나간다면 한층 커 널 소스에 쉽
7卄 다가갈 수 있을 것이다.               지금까지 필자는 시스템이 부팅되면서 커널 코드가 실행되는 흐름을
기술했고, initcall 함수에서부터 실행되는 디바이스드라이버 코드의 초기화（진입） 함수를 소개했다．
커널 소스 코드를 ]00층짜리 건물에 비유한다면 각층으로 이동하는 엘리베이트 위치와 각층에서
원하는 방으로 이동하는 복도의 구조는 파악한 셈이다.                                이제 원하는 방으로 접근하여 방문을 열
고 방안의 내용물들을 파악하는 작업이 남았다.                           디바이스드라이버 프로그래밍을 경험해본 독자분
들은 이미 감을 잡았겠지만, 앞장에서 설명한 디바이스 트리는 100층짜리 건물에서 내가 원하는
층으로 이동하여 방으로 진입하기 위한 주소정보들을 가지고 있다.                                          이제 주소정보들을 어떻게
활용하는지 알아보도록 하자.                  100층짜리 건물의 모든 방을 찾아 다니는것에 앞서서, 몇가지 관심
있는 방부터 찾아가는 방법을 익혀두면, 커널 코드의 설계 구조상 나머지 장치들의 디바이스드라
이버도 쉽게 이해할 수 있을 것이다．


필자는 G미O 디바이스드라이버와 시리얼（UART) 디바이스드라이버, USB 디바이스드라이버를 먼저
선별하여 설명한다.              GPIO乍eneral Puq兀se Input Output）는 CPU의 일반적인 입출력 포트를 사용
하는 것으로 디지털신호（Low/High）를 입출력하여 장치들을 제어할 수 있다． 필자는 GPIC）를 통하
여 LE［瑨 간단히 점멸（On/Off）하는 예제를 설명할 것이다.                            이 드라이버를 잘 이해한다면 나머지
드라이버들도 이와 유사하므로 쉽게 접근할 수 있을 것이다. 이것을 바탕으로 시리얼（UART) 드라
이버와 USB 드라이버를 자세히 알아보도록 하자．




                                               178 / 312
커널연구회（www.kern이.b각                                                       정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                             4. Device Tree 실습   179




4.7G미O 드라이버
G미O 드라이버는 CPU의 핀맵을 어떤 용도로 사용할지를 디바이스 트리에 먼저 기술해먀 한다. (3

장 9절 참조）.        G미O는 커 널의 디바이스 트리에 다음과 같이 등록되어 있다．


# I I /proc/ device- tree/pinctr 1*

/proc/ device- tree/pinctr I@03860000:
total 0
drwxr-xr-x      4 root      root          0 Jan   1 00: 56 .7
drwxr-xr-x    83 root       root          0 Jan   1 00:55 . .1
나十r-나m卞         ] root      root         27 Jan   ] 01:00 corn口at 汁니e
drwxr-xr-x      2 root      root          0 Jan   1 01:00 gpzl
drwxr-xr-x      2 root      root          0 Jan   1 01:00 i2s0-bus/
 r--r-나--       1 root      root         12 Jan   1 01 : 00 interrupts
나 나H나--         1 root      root          8 Jan   1 01:00 name
나小r-나小          ] root      root          8 Jan   ] 01 : 00 reg

/proc/ device- tree/pinctr I@13400000:
 total 0
drwxr-xr-x      9 root      root          0 Jan   1 00: 56 .7
drwxr-xr-x    83 root       root          0 Jan   1 00:55 . . /
  r十r-나小        ] root      root         27 Jan   ] 01:00 compat 仕기e
drwxr-xr-x      2 root      root          0 Jan   1 01:00 dp_hpd/
drwxr-xr-x      2 root      root          0 Jan   1 01: 00 gpxo/
drwxr-xr-x      2 root      root          0 Jan   1 01:00 gpxl/
（打나xr尸xr-x      2 root      root          0 Jan   ] 01:00 야）x2/
drwxr-xr-x      2 root      root          0 Jan   1 01:00 gpx3!
drwxr-xr-x      2 root      root          0 Jan   1 01:00 gpy7/
나 나 나小          ] root      root         12 Jan   1 01:00 interrupts
나 나小r--         1 root      root          8 Jan   1 01:00 name
나 나H나小          ] root      root          8 Jan   1 01:00 reg
drwxr-xr-x      2 root      root          0 Jan   1 01:00 wakeup- interrupt-control ler!

/proc/ device- tree/pinctr 1@13410000:
total 0
drwxr-xr-x    33 root       root          0 Jan   1 00: 56 .7
drwxr-xr-x    83 root       root          0 Jan   1 00: 55 . .1
나 나叫r--         1 root      root         27 Jan   1 00: 58 corn口at 比니e
drwxr-xr-x      2 root      root          0 Jan   1 00: 58 gpco/
dr나xr느xr )(     2 root      root          0 Jan   ] 00: 58 야兀1!
drwxr-xr-x      2 root      root          0 Jan   1 00: 58 gpc2/
drwxr-xr-x      2 root      root          0 Jan   1 00:58 gpc3/
drwxr-xr-x      2 root      root          0 Jan   1 00: 58 gpc4/
drwxr-xr-x      2 root      root          0 Jan   1 00:58 gpdl/
drwxr-xr-x      2 root      root          0 Jan   1 00:58 gpyo/
drwxr-xr-x      2 root      root          0 Jan   1 00: 58 gpyl/
drwxr-xr-x      2 root      root          0 Jan   1 00: 58 gpy2/
drwxr-xr-x      2 root      root          0 Jan   1 00: 58 gpy3/
drwxr-xr--x     2 root      root          0 Jan   1 00: 58 gpy4l
drwxr-xr-x      2 root      root          0 Jan   1 00: 58 gpy5/
drwxr-xr-x      2 root      root          0 Jan   1 00: 58 gpy6/
-r- -r- --r--   1 root      root         12 Jan   1 00:58 interrupts

                                             179 / 312
커 널 연구회 佃Iv八사．kerneLbz)                                                  정재준 (rgt키3307@nate.con가
Device Tree 상세분석 in Linux Kernel 4.0                                                             4. Device Tree 실습   ]80




나1나＋r나         ] root     root          8 Jan    ] 00:58 name
나小I-나1e        ] root     root          8 Jan    ] 00:58 reg
drwxr-xr-x     2 root     root          0 Jan    1 00:58 sdo-bus-widthl/
drwxr-xr-x     2 root     root          0 Jan    1 00:58 sdo-bus-width4/
drwxr-xr-x     2 root     root          0 Jan    1 00:58 sd0-bus-width8/
drwxr-xr-x     2 root     root          0 Jan    1 00:58 sdO-cd/
drwxr-xr-x     2 root     root          0 Jan    1 00:58 sd0-clk/
drwxr-xr-x     2 root     root          0 Jan    1 00:58 sdO-cmdl
dr놔xr-xr-x     2 root     root          0 Jan    1 00:58 Sd卜山于widthl/
drwxr-xr-x     2 root     root          0 Jan    1 00:58 sdl-bus小width4/
drwxr-xr-x     2 root     root          0 Jan    1 00:58 sdl-bus-width8/
drwxr-xr-x     2 root     root          0 Jan    1 00:58 sdl -cdl
drwxr-xr-x     2 root     root          0 Jan    1 00: 58 sdl-clk/
drwxr-xr-x     2 root     root          0 Jan    1 00:58 sdl-cmdf
drwxr-xr-x     2 root     root          0 Jan    1 00:58 sdl-int/
drwxr-xr-x     2 root     root          0 Jan    1 00:58 sd2-bus-widthl/
drwxr-xr-x     2 root     root          0 Jan    1 00:58 sd2-bus-width4/
drwxr-xr-x     2 root     root          0 Jan    1 00:58 sd2-cd/
drwxr-xr-x     2 root     root          0 Jan    1 00:58 sd2-clkl
drwxr-xr-x     2 root     root          0 Jan    1 00: 58 sd2-cmdl

/procldevice- treelpinctr l@14000000:
total 0
drwxr-xr-x   18 root       root          0 Jan   1 00:56 .1
drwxr-xr-x   83 root       root          0 Jan   1 00:55 . .1
drwxr-xr-x     2 root      root          0 Jan   1 01:00 cam-bayrgb-bus/
drwxr小xr-x     2 root      root          0 Jan   1 01:00 cam-gpio-al




                                                       이 이 이 이 이 이 이 이 이 이 이 이 이 이 이 이 이 이
                                                 d
                                                 1 ]
drwxr-xr-x     2 root      root          0 Jan   1 01:00 cam-gpio-b/
먀wxr-町-x       2 root      root          0 Jan   ] 01:00 cam니2c아山sl
                                                 ]
（抑wxr-xr-x     2 root      root          0 Jan   ] 01:00 cam니2c卜加sl
                                                 ]
drwxr-xr-x     2 root      root          0 Jan   1 01:00 cam- i2c2-bus/
                                                 ]
drwxr-xr-x     2 root      root          0 Jan   1 01:00 cam-spiO-busl
                                                 ]
drwxr-xr-x     2 root      root          0 Jan   1 01:00 cam-spil-bus/
                                                 1
나巾나4나--        1 root      root         27 Jan   1 01:00 compatib陀
                                                 ]
drwxr-xr-x     2 root      root          0 Jan   1 01:00 gpe0/
                                                 ]
drwxr-xr-x     2 root      root          0 Jan   1 01:00 gpel/
                                                 ]
drwxr-xr-x     2 root      root          0 Jan   1 01:00 gpfol
                                                 ]
drwxr-xr-x     2 root      root          0 Jan   1 01:00 gpfll
                                                 ]
drwxr-xr-x     2 root      root          0 Jan   1 01:00 gpgo/
                                                 1
drwxr-xr-x     2 root      root          0 Jan   1 01:00 gpgl/
                                                 ]
drwxr-xr-x     2 root      root          0 Jan   1 01:00 gpg2/
                                                 ]
（打川xr-xr-x     2 root      root          0 Jan   ] 01: 00 야기4'

                                                 4
                                                 1 J
                                                   1
-r--r--r--     1 root       root        12 Jan   1 01:00 interrupts
-r--r--r--     1 root       root         8 Jan   1 01:00 name
-r--r--r--     1 root       root         8 Jan   1 01:00 reg

/proc/ device-tree/pinctr 1@14010000:
total 0
drwxr-xr-x    41 root      root          0 Jan   1 00:56 .1
drwxr-xr尸x    83 root      root          0 Jan   1 00:55 . .1
나小r-나卜1        ] root      root         27 Jan   ] 01:00 compat 나)le
drwxr-xr-x     2 root      root          0 Jan   1 01:00 gpa0/
drwxr-xr-x     2 root      root          0 Jan   1 01:00 gpal/
drwxr-xr-x     2 root      root          0 Jan   1 01:00 gpa2/
drwxr-xr-x     2 root      root          0 Jan   1 01:00 gpbO/
drwxr-xr-x     2 root      root          0 Jan   1 01:00 gpbl/

                                            180 / 312
커 널 연구회（www.kernel.b가                                                                        정재준 的b日307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                                            4. Device Tree 실습    ]81




                                                    ]]]]]]j]]]]]jl]]]]j1]]]]]jl]]lljll
drwxr-xr-x      2 root     root             0 Jan   1 01:00 gpb2/
drwxr-xr-x      2 root      root            0 Jan   1 01:00 gpb3l
drwxr-xr-x      2 root     root             0 Jan   1 01:00 gpb4l
drwxr-xr-x      2 root     root             0 Jan   1 01:00 gphol
drwxr-xr-x      2 root     root             0 Jan   1 01:00 i2c0-bus/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 i2cl-bus/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 i2c10-hs-bus/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 i2c2-bus/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 12c3-bus/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 i2c4-hs-bus/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 12c5-hs-bus/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 i2c6-hs-bus/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 12c7-hs-bus/
dr나xr-xr尸）(     2 root     root             0 Jan   1 01:00 12出寸冶七us!
drwxr-xr-x      2 root     root             0 Jan   1 01:00 12c9-hs-bus/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 i2sl-bus/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 12s2-bus/
-r--r--r--      1 root     root            12 Jan   1 01:00 interrupts
-r- -r- --r--   1 root     root             8 Jan   1 01:00 name
drwxr-xr-x      2 root     root             0 Jan   1 01:00 pcml나：)us/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 pcm2-bus/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 pwmo-out/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 pwml-out/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 p뻐n2-out/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 pwm3-out/
나叫r-寸1e         ] root     root             8 Jan   1 01:00 reg
drwxr-xr-x      2 root     root             0 Jan   1 01:00 spdif-bus/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 sp10-bus/
dr싸xr느xr-x      2 root     root             0 Jan   ] 0七00 sp너-bust
drwxr-xr-x      2 root     root             0 Jan   1 01:00 sp12-bus/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 uart0-data/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 uartO-fctl/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 uartl-data/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 uartl-fctl/
drwxr-xr-x      2 root     root             0 Jan   1 01:00 uart2-datat
drwxr-xr-x      2 root     root             0 Jan   1 01:00 uart2나ctlt
drwxr-xr-x      2 root     root             0 Jan   1 01:00 uart3-datat
#


G미O는 커널이 부팅될 때 gpiolib_sysfsin仕 에서 등록된다． 아래는 커널의 부팅 메시지에서 gp向
를 초기화（등록）하는 부분을 표시한 것이다．

#
r
L   dmesg 1 grep gpio
       8.230728] /IKD텨｝:do에e_initcal 1 : 801 : tn_n的怡： 야키ol ib_sys招_init
       8.2371721 gpiochip_add: registered GPI0s 0 to 7 on device: gpy7
       8.2373941 gpiochip_add: registered GPl0s 8 to 15 on device: gpx0
       8.2376171 gpiochip_add: registered GPl0s 16 to 23 on device: gpxl
       8.2378431 gpiochip_add: registered OPIOs 24 to 31 on device: gpx2
      8.238064] gpiochip_add: registered GPI0s 32 to 39 on device: gpx3
      8.2395671 이iochip_add: registered GPIOs 40 to 47 on device: gpc0
      8.2397961 이iochip_add: registered GPl0s 48 to 55 on device: gpcl
      8.2400171 gpiochip_add: registered GPIOs 56 to 62 on device: gpc2
      8.2402661 이기ochip_add: registered GPIOs 63 to 66 on device: gpc3
      8.2404971 아iochip_add: registered GPIOs 67 to 68 on device: gpc4

                                               181 / 312
커 널 연구회（ww比kerneLb기                                                                      정재준 (rgbi3307（亘）nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                             4. Device Tree 실습         182




       8.2407231 gpiochip_add: registered GPl0s 69 to 76 on device: gpdl
       8.2409521 gpiochip中add: registered GPIOs 77 to 82 on device: gpy0
       8. 241176] 야키och巾코dd: registered GPl0s 83 to 86 on device: gpyl
       8. 241403] 미키och巾크dd: re（기stered GPIOs 87 to 92 on device: gpy2
       8.241634] gpiochip_add: registered GPIOs 93 to 100 on device: gpy3
       8.2418611 gpiochip_add: registered GPl0s 101 to 108 on device: gpy4
       8.2420831 gpiochip_add: registered GPIOs 109 to 116 on device: gpy5
       8.2423111 gpiochip_add: registered GPl0s 117 to 124 on device: gpy6
       8.2435021 gpiochip_add: registered GPl0s 125 to 132 on device: g口eo
       8.2437341 gpiochip_add: registered GPl0s 133 to 134 on device: gpel
       8.2439611 gpiochip_add: registered GPI0s 135 to 140 on device: gpf 0
       8.2441851 gpiochip_add: registered GPl0s 141 to 148 on device: gpf 1
       8.2444071 gpioch巾_add: registered GPI0s 149 to 156 on device: gpg0
       8.244639] gpiochip_add: registered OPIOs 157 to 164 on device: gpgl
       8.244865] gpiochip_add: registered GPl0s 165 to 166 on device: gpg2
       8.2450891 gpiochip_add: registered GPl0s 167 to 170 on device: gpj4
       8.246239] gpiochip_add: registered GPIOs 171 to 178 on device: gpa0
       8.2464721 gpiochip_add: registered GPl0s 179 to 184 on device: gpal
       8.2466971 gpiochip_add: registered GPl0s 185 to 192 on device: gpa2
       8.246927) gpiochip_add: registered GPl0s 193 to 197 on device: gpbo
       8.247153] gpiochip_add: registered GPl0s 198 to 202 on device: gpbl
       8.247378] gpi어；hip_add: registered GPl0s 203 to 206 on device: gpb2
       8.2476091 gpiochip_add: registered OPIOs 207 to 214 on device: gpb3
       8.2478401 gpiochip_add: registered GPl0s 215 to 216 on device: gpb4
       8.2480661 이iochip_add: registered GPIOs 217 to 224 on device: gphO
       8.2493191 gpioch巾_add: registered GPl0s 225 to 231 on device: gpz
       8.311628] //KDBG: do_one_ initcal l :801: fn_name: gpiol ib_debugfs_ init
       8.312221] IIKDBG:由_one_initcal l : 801: tn_name: g口io r印내카or그nit
       8.3172021 //KDBG:do_one_ initcal l :801: fn_name: i2c_gpio_init
           12. 734753] 아月et_named月이叱_ f1ags: can나 parse ' samsung, vbus寸gp i 0        아operty of node
  /usb@12110000[ 0] '
[     13.589875) //KDBG: do_one_ initcal l :801: fn_name: gpio_keys_init
[      13.590389] ot_get_nanied_gpiod_f lags: parsed 'gpios ' property of node '/ gpio_keys/wakeup[ O] '
status (0)
[     13.590497] gpio-31 (SW-TACT1) : gpiod_set_ 把bounce: missing set () or set_debounce() operations
[     13. 5917141 input: gpio_keys as /devices/platform/gpio_keys/ input/ inputo


필자는 삼성 Exynos5420 AP가 탑재된 Arndale Octa Board에서 실습하고 있으므로 이 보드에서
G미O 핀을 하나 선정하여 Low/High을 출력할 예정이다． 보드에서 제공하는 회로도를 보면 아래
와 같이 LED(부품번호 D10）를 점멸（아）/O什）하는 핀인 XEINT_24가 있댜．




                                               182 / 312
커널연구회佃ww.kerr犯나끄）                                                        정재준 似和日307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                                                                                            4. Device Tree 실습    ]83




                                                       PVDD AP心 1V8




장치번호 U14는 PDTC114 트랜지스터이므로 XEINT긔 핀의 출력이 네gh이면 LED(D10）이 On되고
XEINT_24 핀의 출력이 Low이면 LED(D10）이 Off 되는 회로이다.                                                                                             아래의 회로도를 보면 XEINT_24
핀은 CPU의 GPX3 0 포트에 연결되어 있댜．


          x딤N下0/GPXO_0/AUD 了CK/ALV TCKIMFC TCK應町 小玎400
         XE們1打아狄乞1/A벼3 TMS/亂vj s滋FC TMS／타I IN丁的J
            xErNT 2/S目X0 2JAUD 在沖A如 TDI/MI6 下DI應X丁IN了4可2 느｛<.= x
                                                                                                                           秘
         XEINT_ 3厄때已3仄UD工油A比夜刃庶印TOO厓X亡INT如＞卞努拭
   X드村寸I 4IOPX0 4/AU口｝只SIN?戶吃V ｛箋｝S 回MFC 了RST똬EXT                             I！
                                                                      寸m 1 戶r如 1 町40
                                                                                 = 1十 1m 4 6쿄   1'
      뇨11m1ii        1; 11 nk小1七a 小 1 1 i二 d11 a\ 石
                   i r 八 14ii n 1 rn                J 1 =r드；
                                                           K m斗 八 1 J                   小小 V 1V \ /
      八CIPI       卞；y1射1八U中랴八OU              nIa＼     伊mVJJ口U小IFMr뇨叫代；                          L4\ ／亡入！   打늬 i 4U    ;,   口4及   J\

                                               XE坪/1敬叩XQ.6/ALV夕宬乞班X了J町406
                              XEIN丁 가Gexo 킥t겻：叱 HPD/ALV 口853戶E）心 作昨407
                     X태旴
                     1 1巾11
                            1mm小 14 m七1 1 1mon汗AC튼！
                                  8/S甘xi                     ）尉AB照LV七日S中4尼町그心41七
                                                1 mmH1 1 m 呻nU  i m1 1 m小 戶 1 1 口
                                                                                   mm m mUm가 1吐 1m4m11 tm11 d m
                                                                                                                      ：쩝
                                                                                                                      r11 1 1 J
                     入口 늬 1 甘八카甘入1 i! IrUL亡珏3丹 i科 8n따LV U匕너 a／匕入 i II나 141 ] r\mF亡 八
                 XEINT       10捉弘；     'Xl    2月-I；亡AC타：     IA丁Al珝ALV그：             蹈甘耐EXT              INT4l      2  X忿                              IN了 10
                 入트I,
                 1 r片 11
                         1mmm 1 d 14 小＝ 1 1mn nmm 1 n m4
                        반件1-I心빈＼뇨삐 Pt八L；匕i斗U／뇨｝計AL也지呼二J應차IN
                                                              4 m 1 m d 1 r 1 느 d J尸m d느
                                                                                         斗mm 1H口
                                                                                                    1mm1= 1口卞 1 m4
                                                                                                             i 41小j그秀
                                                                                                                      LJ11J
                                                                                                                                                      日NT 卄
                 X느1NT121GPX1                 괴IRACEL1ATA              12IALV       DUG      8甁XT        INT4l      4  A;a                             IN了 12
                 1 1m 1 n小
                  入七［NI
                              1 1 t 4 ==1 1 d
                             ii八針J入］
                                              = ==== 1 =1 1=4 = = 1
                                              JIPtAt之UAlP
                                                                       1=   느 口 m {mm4 m 小 1 4 r口＝1 1=n1m11 m日 d Lm1m
                                                                           73／八LV        Ut承j     i月匕乂 !   1싸 i 41
                                                                                                                      i끼11J
                                                                                                                     :}    B6亡                       X딤N丁 13
                1 Jr111 1七
                入：I, 寸 '
                           ; 1 Uh11b d 4
                            I丹八J尸八 !
                                           ; 尸寸hrb 口 m1mJ노 크 叫n 1
                                           0i 1 人八뇨ntJA       1 /1
                                                                     ;     = F = i 1 1 三＋노 小
                                                                         }4汁LV         131針J
                                                                                                :r1 Hm1 r呼什H1 1牛 1 ＝小
                                                                                                 11月亡八 1   口耳 { 坪 1   느
                                                                                                                           口二V
                                                                                                                           1                           ！町 14
                                                                                                                                                     X표！
                XE恥T_15/SPXIJ及RACEDAT凡佃亂닉夕05,, 1｝應XTjN1417                                                                                           x日！町 15
                X타！町小促心P尨j好｝之AC日次TA佈／ALVmDOG I雄XTm岷r420                                                                                              XE次丁 匡6
                X巴NTm1刃GPX2m1FTRACEOATA. 17/ALV，多B｛乞13/EXT_H目2쪼                                                                                      X色NT 17
                XE甘呵個GPX之帥RAG的ATAI8／札V力8GI4/EX互杆慰之筐효舛                                                                                                x됴IN丁 18
                X느Il나L拇心畔毛可［짜kCEL）사凡j到ALY,끄bG,)5/EX里甘4T畔旨3-移云                                                                                        好多N了 19
                X巨1NT斗깝)I3PX之4/T用咤EDAT凡冽風VI招乞化雁xl꾀iT4燾4戶 C..,,                                                                                       X타NT 20
                X틔NT것心맥之5匹RACED町A211赴V邪三妊唇자小m耐2多 巨i;                                                                                                 XEIN了 21
                X느洌1？孤卦J多고U江RACEOATA2刀AL蚣j裂恁尹퀄EXT IN丁42, 6 k夕A                                                                                       X日！町 22




                                                                                                                            篤 靄騶固
     1          뜨呵冬)V.0？多7쯔｝
                           ：뜨므사人C며쌕照＝l匹夾捉！g! 8而
                                                                                                                                                     Y됴 汁d 丁   '1


                八CH쩍 1 mmr14／너戶八그JJ/          ! rt八뇨C1J八      1 月巴 三         川t. 薑中U1八堤브1月C八            匕II斗   t 斗3                                  XEINT 24
                JICI?玎多(arm 1/기叭比I,莎 尸＝k: 乞00QI (CflT_Iffl43_ I
                                                                                                                                                 >> 'C드！卜IT小28
            娼紊就升恥芝卄醫時臘몲豁求崙궁
                辯下3舟丘｛斗品祛몲咎누器解嶽｛瓮仁퓨                                                                                               XX X
 X터NT 30心PX3 前H. 느 （二                       卜町43七 노寸,U
                      ·吸EOA了可竄I/AL丁005m2日巨Xl＞                                                                                                    分 XE作月m烈y卜虹거渽的SEC
 x듸卜仄釘心PX絮'I,堤 뇨 P;m ' " CEr3AT疋知胤町OB可2가타(T그NT43: 1 U= '                                                                                         方 'C嵐町3蚣카汁札H赳）




                                                                                                  183 / 312
커널연구회（www.kernel.b기                                                                                                                        정재준 (rgbi3307@nate.com)
,Device Tree 상세분석 in Linux Kernel 4.0                                                             4. Device Tree 실습    ]84




먼저 리눅스 커널에 있는 G미O 인터페이스를 사용하는 방법을 알아 보도록 하자.                                                            아래와 같이
커널의 menuconfig 을 실행하여 sysfs interface가 선택되어 있는지 확인한다，


Device Drivers
        4                       GPIO Support
                                      [*J Debug GPIO calls
                                      [*] /sys/class/gpio/... (sysfs interface)


         戶me＄加ng的myH야昶（, ./DEV/40pr이ect5f6下，exyn心s5420/20啣kerneL/tInux-4亡



                                       (；口I口 Supp口rt
     Arrow keys navigate the menu. <Enter> selects submenus , - -> (or empty submenus
     * .- -). Highlighted letters are hotkeys. Pressing <V> includes, <N> excludes,
     <M> 卜lodularizes features. Press <Esc><Esc> to exit, <?> for Help, </> for
     Search. Legend: [*] built- tn [ ] excluded <M> module < > module capable

             -- - GPIO Support

            有       旨ebu. GPIO calls

                                      六玄希 Memory mapped GPIO drtvers: 士六*




             < < < <[ 尸
                                      GPIO driver for l4xx- Ics with 邸4IO access
                                >




                      L < < <
                                      Generic memory- mapped GPIO controller support (MMIO platform devtce)
                                >




                                      Synopsys DesignWare APB GPIO driver
                                >




                                      Ena Mobile GPIO
                                >


                                }

                                      ISI ZEVIO Soc memory napped cPIos
                                m1J   Prtnecell PL061 GPIO support
                                >
                                      SMSC SCH311x Superl/O GPIO
                                      GPIO based on SVSC아
                                >



                                >
                                      4er0f1ex Gatsler GRGPIO support
                                      *古士 I2C GPIO expanders: *寸女
                                      Maxt져 片AX7300 GPIO expander
                                      MAX7319. MAX7326- 7327 I2C Port Expanders
                                      PCA9S[ 3573x, PCA9698, TcAo4xx, and MAX731e I/ O ports
                                      PCFB57x, PCA{85, 96}lx, and MAX732[ 89] I2C GPIO expanders
             [                  ]     Sentech SX1S6x I2C GPIO expander


                                       t5elect       < Exit >       .z Help >     < Save >   < Load >




다음으로 Debug Filesystem이 선택되어 있는지 확인한다．


Kernel hacking
         4                      Compile-time checks and compiler options
                                ［시 Debug 테esystem




                                                                     184 / 312
커널연구회（w們N.kern飢bz)                                                                           정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 나nux Kernel 4.0                                           4. Device Tree 실습   185




             e勻ung簪myHome      -/DEV幷0마햐虹缸／恥 目가yn0s5420/20, kern烈川



                        n빠姓뇨士蜘毋 Ch芝芝亐仁 韋n｛亨 Co卜琿汽王er ｛珏｝t乞O六二
     Arrow keys navigate the renu ' <Enter> selects submenus ---> (or empty sub扮enus
     ----).  Highlighted letters are hotkeys. Pressing <'v'> 1.ncl.udes, <N> excludes,
     <M> modularszes features. Press <Esc><Esc> to exit, <?> for Help, </> for
     Search. Legend: ［시 t乂八1.t七） [ j excluded ＜竹＞ NO（札Ic < > module capable

          伊1 { ompt1.e the kernel with debug info
          [ ]   Reduce debugging information
          [ ]   Produce split debuginfo tn .dwo ftles
          [ ]   Generate dwarf4 debugtnfo
          [ I   Provide GOB scripts for kernel, debugging
          [*] Enable _deprecated logic
          [*} Enable 呻丙略t_check logic
          (1824) Warn for stack frames larger than (needs gcc 4. 4)
          [ }Strip assembler- generated symbols during link
          [ }Generate readable assembler code
          [ I Enable unused/ obsolete exported symbols
          I   Track n ate owner
          11* Oebu. Files Ste
          [ }Run 'make headersmcheck' when building vr'olinux
          [ j Enable full Section mismatch analysis
          [ ] Force weak per- cpu definitions



                                                                                            141

                    Selec        < Exit >         < Help >    < Save >   < Load >




만약 위의 menuconfig 옵션들이 선택되어 있지 않댜면, 선택하여 커널을 다시 빌드한다. （빌드 방
법은 4.3.3절 챰조）


위의 옵션들로 커널이 빌드되어 있다면， 아래와 같이 debugfs을 /sys/kernel/debug/ 경로에 마운
트한후 /sys/kernel/debug/gp向 파일의 내용을 확인해1 보면 G미O 포트들의 명칭에 연결되어 있는
핀번호를 알 수 있다．


# mount -t debugfs none /sys/ kerneI/ debuq/

# cat /sys/kern이川ebug/ gp山

GP I Os 아7 , 히at化101셔3400000．이nctr I , gpy7:

OPIOs 8-15, plattorm/13400000.pinctr , gpxO:

GPIOs 16-23 , 이at化101서3400000口inctr I , 야）xl :

OPIOs 24-31, platform/13400000. pinctrl , gpx2:
 gpio-31 (SW-TACT1              ) in hi IRQ

GPIOs 32-39, platform/13400000.pinctrl , gpx3:

                                                  185 / 312
커 널 연구회（www.kerr）飢b기                                                     정쟤준 岫bi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                4. Device Tree 실습    ]86




GPIOs 40-47, platform/13410000.pinctrl , gpcO:

GPI0s 48-55, platform/13410000.pinctr l , gpcl:

GPI0s 56-62, 이at form셔3410000．口inc t r I , 야）c2:

GPI0s 63-66, platform/13410000.pinctr l , gpc3:

GPI0s 67-68, platform/13410000.pinctrl , gpc4:

GPl0s 69-76, platform/13410000.pinctrl , gpdl:

GPI0s 77-82, 이at化rm셔3410000.pinctrl , 0口yo:

GPI0s 83-86, platform/13410000.pinctrl , gpyl:

GPI0s 87-92, platform/ 13410000.pinctrl , qpy2:

GPI0s 93-100, platform/13410000.pinctr l , gpy3:

GPI0s 101-108 , 이at化rm/13410000꾸inctr I , 0口y4:

OPIOs 109-116, platform/13410000. pinctr l , gpy5:

GPI0s 117나］24 , 이at form셔3410000．口inctr I , gpy6:

OPIOs 125-132, platforrn/ 14000000.pinctrl , gpe0:

OPIOs 133-134, platforrn/ 14000000.pinctrl , gpel:

GPI0s 135-140, platform/ 14000000.pinctrl , gpf0:

GPI0s 141-148, platform/ 14000000.pinctrl , gpfl:

GPI0s 149-156, platform/14000000.pinctr l , gpgo:

GPI0s 157-164, platform/14000000.pinctr l , gpgl:

GPI0s 165-166, platform/ 14000000.pinctr l , gpg2:

GPI0s 167-170, platform/ 14000000.pinctrl , gpj4:

GPI0s 171-178, platforrn/14010000.pinctrl , gpao:

GPI0s 179-184, platform/14010000.pinctrl , gpal:

GPI0s 185-192, platform/14010000. pinctr l , gpa2:

GPI0s 193-197, platform/14010000.pinctr l , gpbo:

OPIOs 198-202, platform/14010000.pinctrl , gpbl:

GPI0s 203-206, platform/ 14010000.pinctrl , gpb2:

OPIOs 207-214, platform/14010000.pinctrl , gpb3:

                                                   186 / 312
커 널 연구회（www.kern飢b기                                            정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kerr倒 4.0                                             4. Device Tree 실습   ]87




GPIOs 215-216, platform/14010000.pinctr l , gpb4:

GPI0s 217-224, platform/14010000.pinctr l , gphO:

GPlOs 225-231, platform/ 3860000.pinctrl , gpz:




위에서 우리가 관심을 가지고 있는 G미O는 gpx3 이고 이것은 GP山 번호 32에서 39까지 할당된
다．
32: gpx3. 0
33: gpx3그
34: gpx32
35: gpx3_3
36: gpx3_4
37: gpx3_5
38: gpx36
39: gpx37


/sys/c治ss/gpio 경로로 이동하여 아래와 같이 G미O32번을 제어할 수 있는 정보들을 만든다．


# Cd IsysIclass/ gpio/

# pwd
IsysIclass/gpio

# Is
export       g미och巾］35 야) iOChi이71 gpiochi口215 야)10chip56        9p10ch1p87
gp,ochipO    gpiochipl4l gpiochipll9 gp10chip217 gp1och1p63      gp loch 나）93
gpiochiplOl gp1ochip149 gpioch1p185 gpi0ch1p225 gp1och1p67       unex口ort
gp10ch1p109 gp10chip157 gp1och나）193 gp10ch1p24   gpiochip69
야loch 나니 ] 7 야loch냐)16   야）10ch1p198 먀iochi口32   gpiochip77
gpioch 나니25 gp10ch냐）165 gp10ch나）203 gp1och1p40   gp10ch1p8
gpioch 나)133 gp10ch1p167 Qpiochip207 gp1och1p48  gp1och1p83



It echo 32 > /sys/ class/gpio/ export
# Is
ex口ort        gpi0ch1p133 QpIochip167 gp1och1p207 gp1och1p48     gp10ch1p83
어：)io32       gp1ochip135 gpiochipl7l 야기och I p2化 먀loch i口56     gp10ch1p87
g미 och 나刃     야）loch냐）14] 야키och나）179 야> ioch냐）217 gpioch나）63     gp10ch1p93
gpioch 나)101 gp10ch1p149 gpi0ch1p185 gp10ch1p225 gp山ch巾67        unexport
g口 och 냐)109 gp10ch1p157 9pi0ch나）193 gp10ch1p24     gp10ch1p69
U口 och 나）117 gpiochipl6     gpi0chip198 먀) iOch냐）32 g口loch냐）77
gp10chip125 U미och巾］65 g口i och I口203 gp10ch1p40      g口10chip8

It cd gpio32


                                                  187 / 312
커 널 연구회（www.kernel.bz)                                                  정쟤준 畇너3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                                                      4. Device Tree 실습     188




# II
total 0
（打나xr-자出          3 root     root                    0 Jan               ] 00:16 . /
drwxr尸xr-x        8 root     root                    0 Jan               1 00:13 . .7
  r나나小r--         ] root     root                 4096 Jan               ] 00:16 active Jo벼
lrwxrwxrwx        1 root     root                    0 Jan               1 00:16 device -> . .7. .!. ./13400000.pinctr l/
  r놔나小r--         I root     root                 4096 Jan               ] 00:16 （키 rect ion
  rw-r--r--       1 root     root                 4096 Jan               1 00:16 edge
drwxr-xr-x        2 root     root                    0 Jan               1 00:16 power!
lrwxrwxrwx        1 root     root                    0 Jan               1 00:16 subsystem -> . .7. .!. .1. .!. ./class/gpio/
나wr---r--         1 root     root                 4096 Jan               1 00:16 uevent
  rw나--r小-        1 root     root                 4096 Jan               1 00:16 value

# echo   "out "    > direction




echo 명령을 사용하여 direction 파일에 " out "을 쓰면 해당 G끼O(gpi032: gpx｛이을 출력용으로 사
용하겠다는 의미이다． 이제 gpi032번（gpx｛아을 제어할 준비가 되었다． 네gh/Low 값을 출력하기
위해서 아래와 같이 명령을 내리면 된다．




I/ High 출력
4 echo 1 > value




                             ？」：.:：毛旨＝1
                                                         ；轟                         明
                                                                                          「’
                                                                                          「

                               ，‘茗‘「芦L, j.;"寥
                             ，立：                                                          .
                                    'i誓i
                                       , " "" " '             -        益" 三
                                      ii          n .朴 '1 ' 三t，
                                                            노二：三三云 뇨畿，
                                                                   「프輦L』‘，

                                     羲1夕''p-.．亡：
                                               斗m횬
                                              I..,                .注          恥 '         工스：絮



                                     'I 'g 彖年d多 '
                                           m口＝m   m1 1             n          크 H   =1=   H11




                                     프 明 在于‘ 絮磁璽戴蕪蘿駐匯횰




                                                                  188 / 312
커 널 연구회（ww＼사.kernel.b기                                                                           정쟤준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니nux Kernel 4.0                    4. Device Tree 실습    ]89




//Low 출력
# echo 0 > value




위와 같이 gp向32번（gpx｛이에 네gh(1）을 출력하면 D10 LED가 On 되고 Low(0）를 출력하면 LED가
Off됨을 확인할 수 있다．




                                      189 / 312
커널연구회（www.kern이b기                                 정재준 (rgbi3307@nate.com)
                                                                             4. Device Tree 실습   190
Device Tree 상세분석 in 니flux Kernel 4.0




4.5 시리얼（UART) 드라이버
UART 디바이스드라이버는 커널의 디바이스 트리에 다음과 같이 등록되어 있다． (3.13절 참조）


# I I /proc/device_ tree/ serial*

/proc/device-tree/ser ial@12C00000:
total 0
drwxr-xr-x     2 root      root         0 Jan   1 00:56 .1
drwxr-xr-x   83 root       root         0 Jan   1 00:55 . .1
나 나小r小         ] root      root        20 Jan   1 01 : 05 이ock-narnes
-r小나小r--       ] root      root        16 Jan   ] 01:05 이 ocks
나 나小r小         ] root      root        24 Jan   1 01:05 compat 比니e
-r--r--r--     1 root      root        12 Jan   1 01 :05 interrupts
나1尸r-냐小        ] root      root         7 Jan   ] 01 : 05 name
-r--r--r小      1 root      root         8 Jan   1 01: 05 reg

/proc/device-tree/ser ial@12C10000:
total 0
drwxr-xr-x     2 root      root         0 Jan   1 00: 56 .1
drwxr-xr-x   83 root       root         0 Jan   1 00: 55 . . /
나e나나尸          1 root      root        20 Jan   1 01:05 이 ock-names
寸4나4나--        1 root      root        16 Jan   ] 01:05 이 ocks
-r尸나나小         ] root      root        24 Jan   1 01 : 05 compatit니e
나＋r-나H卜        ] root      root        12 Jan   ] 01: 05 interru口ts
나 나나小          ] root      root         7 Jan   1 01: 05 name
mr十나H十r尸卜      ] root      root         8 Jan   ] 01:05 reg

/proc/device-tree/ser ial이2C20000:
total 0
drwxr-xr-x     2 root     root          0 Jan   1 00: 56 .1
ctrwxr-xr-x  83 root      root          0 Jan   1 00: 55 . .1
나 나小r小         ] root     root         20 Jan   1 01 :05 이 ock-names
寸4나사--         1 root     root         16 Jan   1 01: 05 （기ocks
-r-나1나小        1 root     root         24 Jan   ] 01:05 compat 比키e
-r--r--r--     1 root     root         12 Jan   1 01: 05 interrupts
나 나小r小         ] root     root          7 Jan   1 01:05 name
나 나 나小         ] root     root          8 Jan   1 01:05 reg

/proc/device-treelser ial@12C30000:
total 0
drwxr-xr-x     2 root      root         0 Jan   1 00: 56 .1
drwxr-xr-x   83 root       root         0 Jan   1 00:55 . .1
나나나小           ] root      root        20 Jan   1 01 : 05 clock놔names
나 나나小          ] root      root        16 Jan   1 01:05 clocks
寸＋r-나小         ] root      root        24 Jan   ] 01 :05 corn口at 比) le
-r--------     1 root      root        12 Jan   1 01 : 05 interrupts
-r--r--r--     1 root      root         7 Jan   1 01 : 05 name
나 나 나小         ] root      root         8 Jan   1 01: 05 reg




                                            190 / 312
 커 널 연구회（www.kerr）飢b기                                                    정재준 眄비3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                             4. Device Tree 실습        ]91




아래는 4.4장에 있는 커널 부팅 로그 메시지에서 시리얼（UART) 디바이스 드라이버의 초기화（진입）
코드에 해당하는 것을 가져온 것이다．


# dmesg I grep serial
[    0.0002971 //KDBG: s3c24xx_seria匕console_ jnjt:1459: s3c24xx_seria匕console_initO: start. . .
[

[
     0.0003081 IlK田G: s3c24xx_s帥a匕cons이已羽뺘j:2127: s3c24xx_ser ia匕console_setupO: start. . .
     8 . 羽凹24] I/ K.D凹：do_one_initcal 1:80七 fn小nan冶： sen키叩50_i nit
[
     8.599079] IIKDBG: ser ia18250_ ini t :3780: uart_register_dr iverO: end.
rL [
     8.6009521 //KDBG: 5eria18250_ ini t:3799: platform_dniver_registerQ: start. . .
     8.601166] //KDBG:do_one_ initcal l :801: tn_name: sarnsung_seria匕driver_init
[
     8.601289) //KDBG: s3c24xx_ser ia匕probe:1824: s3c24xx_ser ial_probeO: index=0
L [
r
1
     8.601443] 12c00000.serial : ttySA（刃 at MMI0 0x12c00000 ( irq = 58, base_baud = 0) is a S3C6400/10
[
     8.601461] I/ KDBG: s3c24xx_ser ia匕console_setup:2127: s3c24xx_ser ia匕console_setu口O: start. . .
     8.6019521 //KDBG: s3c24xx_ser ia냐robe:1824: s3c24xx_ser iaI_probe() : index=1
r
t [
     8.602048) 12c10000. serial : ttySAC1 at 刪0 0x12c10000 ( 나q = 59, base_baud = 0) is a S3C6400/10
     8.602064] IlKDB0: s3c24xx_ser i匕console_setup:2127: s3c24xx_ser ial_console_setupO: start. . .
[
     8.6025671 //KDBG: s3c24xx_ser i a匕probe:1824: 53c24xx_ser ia냐robeO: index=2
[
     8.602660] 12c20000. serial : ttySAG2 at MMI0 0x12c20000 ( irq = 60, base_baud = 0) is a S3C6400/10


r
L r
  1L [
     8.602676] //KDBG: s3c24xx_ser ia匕console_setup:2127: 53c24xx_ser ia匕console_setupO: start. . .
     8.603165] //KDBG: s3c24xx_ser ia匕probe:1824: s3c24xx_ser ia匕probeO: index=3
[
     8.603259] 12c30000. serial : ttySAC3 at NMI0 0x12c30000 ( irq = 61, base_baud = 0) is a S3C6400/10
     8.603275] //KDBG: s3c24xx_ser ia匕console_setup: 2127: s3c24xx_ser ia匕console_setupO: start. .
[
    11.366785] //KDBG: do_one_ initcal l :801: tn_name: of_plattorm_serial_driver_init
#




위에서 seria18250_init() 함수에서부터 시리얼（UART) 디바이스 드라이버 소스를 분석하는 작업율
시작하자.        필자는 분석 대상함수가 커널 소스 파일들 중에서 어디에 정의 되어 있는지 검색할 때
아래의 인터넷 웹사이트를 활용한다．


http://lxr.free-electrons.com/ident


위의 웹사이트에서 sen키8250_in仕을 검색하면 다음과 같은 결과로 검색된다．




ser ia 田250_ ini t
Defined as a function in:
drivers/ tty/ serial/8250/8250_core. c, l ine 3761
Referenced ( in 1 fi les total) jn:
drivers/ tty/ ser ia11825018250_core. c:
l ine 3761
l ine 3839




위의 검색결과를 보면 seria18250_in仕 함수가 정의되어 있는 소스 파일은 /drivers/tty/serial/8250/

                                               191 / 312
커 널 연구회（w'사w.kernel.b기                                                   정재준 岫b日307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                     4. Device Tree 실습




8250_core.c이고 이곳의 376］행에 소스 코드가 있음을 알 수 있다.                                   이 링크를 클릭하면 바로 소
스가 있는 위치로 이동한다．



static mnt _init ser1a18250_init (void)
{
           mnt ret;

           ser i 키 陀50_ isa_ in it尸ports( ) ;

           printk(KERN_ INFO "Ser ial : 8250/16550 driver,
                    "%d ports, IRQ sharing %sabledWn", nr_uarts,
                    share_ i rqs ? "en" : ndiSD ;

#i fdef CONFIG_SPARC
          ret = sunserial_register_minors(&seria18250_reg, UART_NR) ;
#else
          seria18250_reg.nr = UART_NR;
          ret = uart_register_driver (&seria18250_reg) ;
#endi f
          if (ret)
                   goto out;

           ret = ser1a18250_pnp_initO;
           if (ret)
                    goto unreg_uar t_drv;

           ser ia18250_ isa_devs = platform_device_al Ioc( "ser ia18250",
                                                                PLAT8250_DEV_LEGACY) ;
           if ( !ser i키叩50 isa 把vs) {
                      ret = -ENOMEM;
                      go如 unreg_pn口；
           }
           ret = platform_device_add(seria18250_ isa_devs) ;
           if (ret)
                    goto put_dev;

           ser ia田250_register_ports(&ser ia18250_reg, &ser ia18250_ isa_devs->dev) ;

           ret = platform_driver_register (&serial8250_ isa_driver) ;
           if (ret == 0)
                    goto out;

           platform_device_del (seria18250_ isa_devs) ;
put_dev:
         platform_dev ice_put (ser i a18250_ i sa_devs) ;
unreg_pnp :
         ser i 키 陀50_pnp中exit ( ) ;
unreg_uar t_drv:
#ifdef CONFIG SPARC
         sunserial_unregister_minors(&seria18250_reg, UART_NR) ;
#e 1 se
         uart_unregister_dr iver (&ser ia18250_reg) ;

                                                  192 / 312
커 널 연구회（www.kern텨.b기                                                          정재준 (rgbi3307@nate.com)
Device Tree 상세분석 In 니flux Kernel 4.0                                                4. Device Tree 실습   ]93




#endi t
out:
          return ret;
}
static void n exit seria18250_exit (void)
{
          struct 이at form펴帥比e 치sa dev = ser I키明50_ isa_devs;



           * Thus tel ls ser1a18250_unregEster_port () not to re-register
           * the ports (thereby making seria18250_ isa_driver permanently
           * in use. )
           十 r




          ser I키明50_ isa펴evs = NULL;

          platform_dr iver_unregister (&ser ia18250_ isa_dr iver) ;
          platform_device_unregister ( isa_dev) ;

          ser ia18250_pnp_exi tO;

#ifdef CONFIG SPARC
         sunser i a匕unre이없아小in아s(&ser ia18250_reg, UART_NR) ;
#eIs（크
#e 1 S（크
         uart_unregister_driver (&seria18250_reg) ;
#endi f
}
module_ ini t (seria18250_ init) ;
module_exi t (ser 1a18250_exit) ;




위에서 디바이스드라이버 초기화（진입） 함수인 sen키8250_in仕은 module init() 매크로 함수에 의하1

서 등록되는데, 이 매크로 함수는 다시 device_initcall() 함수로 정의되어 있다.                                   4.4장에서 기술한
기nclude/Iinux/init.h 헤더파일에 이 매크로 함수가 정의되어 있다．


UART 디바이스는 serial 방식으로 데이터를 주고 받는 방식으로 동작한다.                                        요즘의 장치들은 대부
분 sen히（직렬） 방식으로 데이터 통신하므로 UART 디바이스 드라이버의 동작 원리를 잘 이해하면

이와 유사하게 동작하는 12C, 12S, SPI, USB, Ethernet 등의 디바이스드라이버도 쉽게 분석할 수 있

다．
먼저 UART 디바이스드라이버의 동작을 확인해 보자． UART 드라이버는 다음과 같이 장치노드 파

일 ttySAC0, 1, 2, 3번 포트로 생성된다．



# I I /dev/ ttySAC火
crw              1 root      root      204,   64 Jan   1 00:00 /dev/ ttySAC0
crw              1 root      root      204,   65 Jan   1 00:00 /dev! ttySAC1


                                                   193 / 312
커 널 연구회（ww比kerriel.b기                                                          정재준 內t키3307@nate.com)
Device Tree 상세분석 in 니nux Kernel 4.0                                                                                              4. Device Tree 실습   ]94




                     1 root      root      204,        66 Jan 1 00:00 /dev/ ttySAC2
crwcrw               1 root      r。
                                  。t       204,        67 Jan 1 00: 00 /dev/ ttySAC3



필자가 실습하고 있는 삼성 Exynos5420(arndale-octa 보드）은 다음과 같이 CPU 내부에 4개의
UART 포트가 있다．


                                                      （月A

                                            R벼 n
         x旴苡Do                                        XURXD 0/GPA0 0/EX丁 作4了10
         乂uTXDO                                       胤玎xD 明GPAO hEX了 什寸TI 1
         XuR了앉10                                      XURTSN OIGPA0 3厄X丁 INTl 3
         XuC了S的                                       xUC了＄N OIGPA0 2尼好 INTl 2
                                                                                                                                            UART
                                             殆m 山 m
         XuRXD1
                                                      Xu只xD 依3PAO 町EX丁 f卜昨14
         Xlii城거                                       XUTXD h/GPA0 5乍Xi IN下15
         XuRTSn1/I2C 2 SCI.                           胤丹t了SN 卄GPA0 7／住C 2 SCLJ프Xi IN下］ 7
         X出：井Sn打［2C 2 SOA                             XUC了SN ！心PAO $／促C 2 SONEXT 作4了IS


                                             m M m忍
         X旴｛xD깝GPAI (}                                XURX口 刀GPAI 아UART AUD心 RXD應x了 INT2 0
         凡玎X02/GPAI }                                 XUTXD 2/GPAI 1/UART AUDIO TXD/E焰 州12 I
         XuR下＄n刃口C 3 ScI.                             XUR下＄N 刀GPAI 3/12C 3 Sd)드XT 什4作 :}
         風iCiSn요／口C 3 SDA                             xUc下＄N 2/CPA! 却2C 3 SDA應X丁 'p昨22
         luftXD3心PA1 4                       町        XURXD 카CPAI 町UART AOl거0 RXD芯Xi '！町24
         XuTX口智OPA喜 5                                 XUTXD 카（3PA1 SILJA｝町 AUDIO 了xo／巨x了 [N了25




위에서 UART1(Jdev/ttySAC 1）은 arndale-octa 보드에서 아래와 같이 외부로 연결할 수 있는 커넥터
핀（CON6）을 제공하고 있다.                       핀번호 24는 UART1의 RxD］이고 핀번호 26은 TxD］에 해당한다．

                                                      DC5V
                                                      O
                                                      ·
                                                                             C361
                                                                                i                 1( 247uF. 6.3F


                                                                                               CON6
                                                                              2                 m




                                                                                                                          多
                                                                                                          3


                                 宦
                       XuRXD0




                                                              1 1 l 個 的 蚣 叫 恥 茹 羽 的 銓弘 鈴 鋸 的
                       XuD(D0                                                                             7
                       XuR了＄no




                                                            8 0m<4 8
                                                                                                          9
                                                                                                          1
                       XUCTSr0




                                 多
                                                                                                                     口나
         XuRXD2/GPA1 0

                                                                                                          a! d1 d1
         XU了XD2JGPA下 i                                                                                   ii               >> XHStCDATA0
         Xu！打＄n2／泛C3..SCL                                                                                V
                                                                                                         n
         XuCTSr刀i2C 3 SDA                                                                                뷰           1    冷 xH＄尤S再均BE0

                                  柔                                                                            차
                                                                                                                          ?? X棚柚CICLK
                                                                                                                          ?? X云4h巖；1C系AD




                                                                   1
                                                                   4
                                                                                                                          /? XMl,希cicr;月녘

                                                                                                               3 亡U 7羽
              Xsp李CL卜（l／促M艸＄CL卜
                              （                                                                                           ?? 好船ACID呵烈）
              肛piCS粕1／應서－多們싸1                                                                                             d? XMMC1DATA1

                                                                                                              引3
                                                                                                                  33
              x斟芦MtS아                                                                                                     e? XMMCIDATA2

              篇썲驢甘                                                                                                        나/) XMMC1DATA3

              x配弑｝A斛4                                                                                                     >>   Xn只ESE了
                                                                                                 i1




                                            玄y                Nq匪AIDER 20X2 2rr吼月r冬尹




                                                                  194 / 312
커 널 연구회（ww比kern텨. b기                                                                                                      정재쭈 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                              4. Device Tree 실습    195




다음과 같이 명령을 실행하면 핀번호 26인 TxD1에서 serial 데이터가 출력됨을 확인할 수 있다．



# echo   test ' > /dev/ ttySAC1




                  :
                  ＝




                  毛朴撥管m




                 鬚簪L
                  三t口n;
                          (
                          i



                  ;=q
                          1


                          =




                                                   m
                                                   n =   n 느   喆許 t 2
                                                                        珏d                  小
                                                               =＝
                                                                小




위의 사진에서 핀번호 26에 해당（화살표）하는 TxD] 신호를 스코프로 찍어보면 아래와 같이 " test'
데이터가 출력됨을 확인할 수 있다．




아래 그림은 위의 파형을 확대하여 좀더 자세히 분석한 것이다. ］비트를 전송하는데 0.l04lms가


                                       195 / 312
커 널 연구회（www.kernel.bz)                                                       정재준 (rgL기3307@nate.com)
Device Tree 상세분석 in 니nux Kernel 4.0                                                  4. Device Tree 실습   ]96




소요되었으므로 역수를 취하여 주파수를 계산하면 9.602kHz(9600bps) 속도로 전송됨을 확인할 수

있다．




UART 디바이스 드라이버 소스는 5장부터 상세하게 분석한다．




4.6 USB 드라이버
아래는 4.4장에 있는 커널 부팅 로그 메시지에서 USB 디바이스 드라이버의 초기화（진입） 코드에

해당하는 것을 가져온 것이다．


# doiesg I grep usb
      8.315936] //KD텨｝:do_one_ini tcal I :801: f凡name: usb_ini
      8.3162711 usbcore: registered new interface driver usbfs
      8.316436] usbcore: registered new interface driver hub
      8.316713] usbcore: registered new device driver usb
      8.316731] //KDBG: do_one_ initcal l :801: fn_name: usb_udc_init
      8.4783031 //KDBG: do_one_ ini tcal 1 :801: fn_name: samsung_usb2_phy_dr i ver_ ini
      8.479317] //KDBG: do_one_ initcal l :801: tn_name: exynos5_usb3drd_phy_ init
    11.5294451 usbcore: registered new interface driver asix
    11.5415751 usbcore: registered new interface driver ax88179_178a
    11. 5536181 usbcore: registered new interface driver cdc_ether
    11. 5658681 usbcore: registered new interface driver smsc75xx
    11.5779751 usbcore: registered new interface driver smsc95xx
    11.589982] usbcore: registered new interface driver net1080
    11.602229] usbcore: registered new interface driver cdc_subset
    11 .614362] usbcore: registered new interface driver zaurus
    11.6197991 //KDBG: do_one_ initcal l :801: fn_name: usbnet_init
    11 .631905] usbcore: registered new interface driver cdc_ncm
    11 .6508581 usb@12000000 supply vdd33 not found, using dummy regulator
    11 .6567021 usb@12000000 supply vdd杓 not found, using dummy regulator
    12.0666221 usb@12400000 supply vdd33 not found, using dummy regulator
    12.071759] usb@12400000 supply vddlo not found, using dummy regulator
    12.5120531 usb usbi: New US8 device found, idVendor=ld6b, idProduct=0002
    12.518567] usb usbi: New USB device strings: Mfr=3, Product=2, SerialNumber=1
    12.525788) usb usbi: Product: xHCI Host Control ler
    12.5306381 usb usbi: Manufacturer: Linux 4.0.0 xhci-hcd
    12.5358951 usb usbl: SerialNumber: xhci-hcd.2.auto
    12.5617411 usb u5b2: New USB device found. idVendor=ld6b. idProduct=0003
    12.568219] usb usb2: New USB device strings: Mfr=3, Product=2, SerialNumber=1
    12.575442] usb usb2: Product: xHCl Host Control ler
    12.580262] usb usb2: Manufacturer: Linux 4.0.0 xhci-hcd


                                                 196 / 312
커 널 연구회 (wwwkerne比기                                                          정재준 (rgbi3307@nate.com)
Device Tree 상세분석 In 니flux Kernel 4.0                                        4. Device Tree 실습         ]97




[   12.5855781 usb usb2: SerialNumber : xhci-hcd.2.auto
[   12.6259901 usb usb3: New USB device found. idVendor=ld6b. idProduct=0002
[   12.6325471 usb USDd. New Ubb aevice sir 1 ngs· Mir=乞 rroauci=Z, berIaINumDer=i
1   12.639707] usb usb3: Product: xHCI Host Control ler
[   12.6447151 usb usb3: Manufacturer: Linux 4.0.0 xhci-hcd
[   12.6498461 usb usb3: SerialNumber: xhci-hcd.5.auto
[   12.6756971 usb usb4: New USB device found, idVendor=ld6b, idProduct=0003
[   12.6822001 usb usb4: New USB device strings: Mfr=3, Product=2, Set ialNumber=1
[   12.6893601 usb u5b4: Product: xHCl Host Control ler
[   12.6943931 usb u5b4: Manufacturer: Linux 4.0.0 xhci-hcd
[   12.6994981 usb usb4: SerialNumber : xhci-hcd.5.auto
[    12.734753] of_get_named_gpiod_f ags: can ' t parse 'samsung, vbus-gpio ' property of node
 /usb@12110000[ 0] '
[
     12.7349881 exynos-ehci 12110000 usb: EHCI Host Control ler
r1 [
     12.7399971 exynos-ehci 12110000 usb: new USB bus registered, assigned bus number 5
     12. 7478411 exynos-ehci 12110000 usb: irq 107, io mem 0x12110000
[
     12.7705591 exynos-ehci 12110000 usb: USB 2.0 started, EHCI 1.00
r
1
1L [
     12.775287] usb u5b5: New USB device found, idVendor=ld6b, idProduct=0002
     12.7818711 usb u5b5: New USB device strings: Mfr=3, Product=2, SerialNumber=1
[
     12.789030] usb u5b5: Product: EHCI Host Control ler



rL rL r
      1L [
     12.793912] usb usb5: Manufacturer: Linux 4.0.0 ehci hcd
     12.7991681 usb u5b5: SerialNumber: 12110000.usb
     12.8343241 exynos-ohci 12120000.usb: USB Host Control let
     12.8394071 exynos-ohci 12120000.usb: new USB bus registered, assigned bus number 6
[
     12. 8471611 exynos-ohci 12120000.usb: irq 107, io mem 0x12120000
[
     12.9149531 usb usb6: New USB device found, idVendor=ld6b, idProduct=0001
[
     12.920260] usb usb6: New USB device strings: Mfr=3, Product=2, Set ialNumber=1
[
r
     12.927482] usb usb6: Product: USB Host Control ler
[
     12.9322431 usb usb6: Manufacturer: Linux 4.0.0 ohci hcd
[
     12.9375021 usb usb6: Set ialNumber : 12120000. usb
[
     12.955620] /／肛好6: do叩巳initcal 1 :801 : fn尸name: usb_storage_dr iver_ ini t
[
     12.9625011 usbcore: registered new interface driver usb-storage




=[ rt rL rL [
     12.968268] //KDBG: do_one_ initcal l :801: fn_name: usb3503_init
     13.1307061 usb 5너: new high-speed USB device number 2 using exynos-ehci
     13.3028971 usb 5-1: New USB device found, idVendor=05e3, idProduct=0610
     13.3088271 usb 5너: New USB device strings: Mfr=0, Product=1, Set ialNumber=0
     13. 3159691 usb 5너: Product: USB2.0 Hub
 [
     13.5786941 usbcore: registered new interface driver usbhid
 [
     13. 5787021 usbhid: U鋸 HID core driver
 [
     13.6109711 usb 5너 .4: new high-speed USB device number 3 using exynos-ehci




 r
 1L [1 [L r
          1L [
     13.7225981 usb 5너 . 4: New USB device found, idVendor=0b95, idProduct=772a
     13.7226111 usb 5너 . 4: New USB device strings: Mfr=1, Product=2, Set ialNumber=3
     13.7226221 usb 5너 . 4: Product: AX88772
     13.7226321 usb 5너 . 4: Manufacturer: ASIX Elec. Corp.
     13.7226441 usb 5너 .4: Set ialNumber: 000001
 [
      14.544553] asix 5-1.4:1.0 ethO: register 'asix ' at usb-12110000.usb너.4, ASIX AX88772 USB 2.0
Ethernet, de:14:19:cd: cd:b2


위에서 usb_init() 함수에서부터 USB 디바이스 드라이버 소스를 분석하는 작업을 시작하자.                                        필자
는 분석 대상함수가 커널 소스 파일들 중에서 어디에 정의 되어 있는지 검색할 때 아래의 인터넷
웹사이트를 활용한다．


http://lxr.free-electrons.com/ident

                                            197 / 312
커 널 연구회（ww比kerneli끄）                                                  정재준 (rgbi3307@nate.com」
Device Tree 상세분석 in Linux Kernel 4.0                                                         4. Device Tree 실습   ]98




위의 웹사이트에서 usb_in仕을 검색하면 다음과 같은 결과로 검색된다．



usb_ I n I t
Defined as a funct ion in:
drivers/net/ wireless/ zdl2llrw/ zdusb.c, l ine 1547
drivers/ usb/ core/usb. c, l ine 1045
Referenced ( in 2 fi les total ) in:
dr ivers/net/ wireless/ zdl2llrw/ zd usb. c:
l ine 1547
l ine 1551
l ine 1578
dr ivers/ usb/ core/ usb. c:
l ine 1045
l ine 1119




위의 검색결과를 보면 usb_in仕 함수가 정의되어 있는 소스 파일은 /drivers/usb/core/usb.c이고 이
곳의 ]045 행에 소스 코드가 았음을 알 수 있다.                                     이 링크를 클릭하면 바로 소스가 있는 위치로
이동한다．


/y



         mnit
    *1
stat ic mnt _ini t usb_ init (void)
{
                    nt retval ;
                    f (nousb) {
                            pr_ info( '%s: USB support dsabledWn " , usbcore_name) ;
                            return 0;
                }
                usb_ init_pooI_rnax ( ) ;

                retval = usb_debugfsjni t ( ) ;
                if ( retval )
                          goto out;

                usb_acpi_register () ;
                retval = bus_register (&usb_bus type) ;
                  f (retval)
                          goto bus_registerjai led;
                retval = bus_register_notifier (&usbbus_ type, &usb_bus_nb) ;
                if (retval)


                                                          198 / 312
커 널 연구회（ww比kerne냐끄）                                                                    정재준 (rgL기3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                      4. Device Tree 실습   199




                    g아o bu丘n아 if ier tai led;
           retval = usb_major_initU;
           if (retval)
                    goto major_mnit_ f: i led;
           retval = usb_register (&usb [s_driver) ;
           it (retval)
                    gob driver_regis 1er_fai led;
           retval = usb_devio_initQ;
           if (retval)
                    goto usb_devio_ in it_ fai led;
           retval = usb_hub_initQ;
           if (retval)
                    goto hub_ init_ fai led;
           retval = usb_register_devi e_dr iver (&usb_gener ic_dr iver , THIS_MODULE) ;
           it ( 나etval)
                    goto out;

          usb_hub_c I eanup() ;
hub_ init_ fai led:
          usb_devio_cleanupQ;
usb_devio_ ini t_fai led:
          usb叱re이 ster (&usbf 乞dr iv ?r ) ;
driver_register_fai led:
          usb_major_cleanupQ;
major_ init_fai led:
          bus_unregister_not if ier (&u 就乙bus_ty口e, &usb_bus_nb) ;
bus notifier tai led:
          bus_unreg i ster (&usb_bus_ty )e) ;
bus_re미 없er_ tai led:
          usb코叩匕unre（기 ster () ;
          usb_debugts_cleanupO;
out :
          return retval ;
}
／大
     玄 이eanu口
     玄 /


static void _exit usb_exit(void)
{
           /* This wi l l matter if shu tdo川n/ reboot （幻es exitcal ls: 士／
           if (nousb)
                    return;

           usb_deregister_device_dr iv er (&usb_gener ic_dr iver) ;
           usb_ma如n이 明nupO;
           usb_deregister (&usbfs_dr iv 스．r ) ;
           usb_dev i 0_cl eanupO;
           usb_hub_c I eanupO;
           bus_unregister_not if ier (&u 故乙bus_ty口e, &usb_bus_nb) ;
           bus_unregi ster (&usb_bus_ ty Dc) ;
           usb_acpLunregisterO;
           usb_debugfs_cleanupO;
}
subsys_ ini tcal l (usb i nit) ;

                                                  199 / 312
커 널 연구회 (www.kern이.bz)                                                        정쟤준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                              4. Device Tree 실습   200




module_exi t (usb_exit) ;
MODULE_LICENSE( n GPL ' ) ;




USB 포트에 USB를 장착하면 아래와 같이 인식 메시지들이 술력되고 mount 명령을 사용하여 파

일시스템을 마운트하여 사용할 수 있다．


[11338.990535] //KDBG:kthreadd:514: create_kthread(create) . . .
[11339.200550] usb 3-1: new high-speed USB device number 2 using xhci-hcd
[11339.342485] usb 3-1: New USB device found, idVendor=058f, idProduct=6387
[11339.347702 1 usb 3-1: New USB device strings: Mfr=1, Product=2, SerialNumber=3
[11339. 354846] usb 3-1: Product: Mass Storage
[11339.358878] usb 3-1: Manufacturer: Generic
[11339.362991] usb 3-1: SerialNumber: 43089E5B
[11339.368313] usb-storage 3-1:1.0: USB Mass Storage device detected
[11339.373238] //KDBG:kthreadd:514: create_kthread(create) . . .
[11339.378744] //KDBG:kthreadd:514: create_kthread(create) . .
[11339.384305] //KDBG:kthreadd:514: create_kthread(create) . . .
[11339.389621] scsi hostO: usb-storage 3-1:1.0
[11340.391381] scsi 0: 0:0: 0: Direct-Access       Generic Flash Disk      801 P0: 0 ANSI : 2
[11340.399037] //KDBG:kthreadd:514: create_kthread(create) . . .
[11340. 404118] ad 0:0: 0:0: Attached scsi generic sg0 type 0
[11340. 408900] sd 0:0:0:0: [sda] 123518 512-byte logical blocks: (63.2 MB/ 60. 3 MiB)
[11340. 416654] scsi 0:0:0:1: CD-R에                Generic Autorun Disk    8. 00 PQ; 0 ANSI : 2
[11340.424232] //KDBG:kthreadd:514: create_kthread(create) . . .
[11340.426187] scsi 0: 0:0:1: Attached scsi generic sgl type 5
[11340. 431068] sd 0:0: 0:0: [sda] Write Protect is off
[11340. 431535] sd 0:0: 0:0: [sda] No Caching mode page found
[11340. 431549] sd 0: 0: 0: 0: [sda] Assuming drive cache: write through
[11340.451246] !/KDBG:kthreadd:514: create_kthread(create) . . .
[11340.600956] sda: sdal
[11340.603686] sd 0:0:0:0: [sda] Attached SCSI removable disk

# mount -t vfat /dev/sdal /mnt/
[11440.763183] //KDBG: kthreadd:514: create_kthread(create) . . .

ft I I !mnt/
[11448.099009] //KDBG:kthreadd:514: create_kthread(create) . . .
total 355
drwxr-xr-x    9 root     root         16384 Jan 1 00:00 .1
drwxr-xr-x   19 root     root          1024 Mar 14 2015 . .1
나水r-肝-x       ] root     root            57 Sep 6 2011 AUTORUN.FCB*
drwxr-xr-x    2 root     root          2048 Sep 6 2011 Appl ications!
drwxr-xr-x    2 root     root          2048 Sep 6 2011 Cl ient!
drwxr-xr-x    2 root     root          2048 Jan 1 2013 LOST.DIR/
나叭r-xr水       ] root     root           492 Sep 21 2014 PnS. lnk*
drwxr-xr-x    3 root     root          2048 Dec 19 2012 SMRTNTKY/
drwxr-xr-x    2 root     root          2048 Sep 6 2011 User Manual!
-r- xr-xr-x   1 root     root        167936 Nov 9 2010 bf3ln.exe*
-rwxr-xr-x    1 root     root         28672 Apr 14 2008 set upSNK. exe*
drwxr-xr-x    2 root     root          2048 Nov 30 2013 temp!
drwxr-xr-x    3 root     root          2048 Sep 6 2011 wePresent나：기us!
-rwxr-xr-x    1 root     root           415 Sep 6 2011 wePresent-Plus. lnk*

                                                200/ 312
커 널 연구회（www.kerr忙L.b기                                                     정재준 (r야)i3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                 4. Device Tree 실습    201




나出r-xr出     ] root    root      129024 May ]]   2010 yv .exe士
#


USB 디바이스드라이버 소스는 다음 기회에 자세히 분석하여 기술할 예정이다．


지금까지 G미O, 시리얼（UART), USB 드라이버에 대해서 간단히 실습했다.                        이중에서 시리얼（UART)
은 장치들간에 RxD, TxD 라인으로 연결되어 직렬로 데이터를 송수신하는 방식이다.                              이것을 커 널
에서 어떻게 운행하고 있는지 자세히 알아두면 다른 대부분의 장치들(I2C, I2S, SPI, USB, Network...)
의 드라이버들도 쉽게 이해할 수 있다.                  시리얼（UART) 드라이버는 모든 장치들의 드라이버를 이해
하는데 필요한 기본 지식이 되므로 필자는 이것을 자세히 분석한 내용을 다음장부터 기술한다．
이제부터 본격적으로 커널 소스 탐방이 시작 되므로 독자분들도 커널 소스와 친구가 되도록 노력
하1 주기 바란다．




                                         201 / 312
커널연구회佃ww.kerri이b기                                               정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                   5. UART 드라이버 상세분석          202




5. UART 드라이버 상세분석




                                                   + 필자의 주말농장0私寸 찍은 장미꽃




시리얼（UART) 디바이스드라이버 소스를 자세히 분석하기 전에 먼저 전체적인 소스 코드의 흐름을
정리한후 이것을 바탕으로 상세하게 소스를 분석하도록 하자.                    UART 드라이버는 아래와 같은 흐
름으로 소스가 구성되어 있다．




                                       202 / 312
커널연구회（w'사比kern텨.b기                                     정쟤준 (rgbi3307@ nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                           5. UART 드라이버 상세분석          203




사용자 어플리케이션
                                                                  System Files(/proc, /sysfs, /dev)
tty山．c
                                                       System Call (open, read, write, ioctl, close)
                                                 linux/syscalls.h, copy_from_userO, class, module
TTY 드라이버


serial core.c


                                              drivers/base, device_driver, driver_registerO, probe0

Low-Level 드라이버
                                                                         tty line discipline(tty_ldisc)
8250 core.c
samsung.c
                                                                 bus_type, device, device_create()
하드웨어




먼저 사용자 어플리케이션 계층에서 UART 드라이버가 어떻게 생성되어 있는지 다음과 같은 방법
으로 확인가능하다． "/proc/tty/drivers " 파일의 내용을 보면，


# cat IprocIttyIdr I vers
                                       二U
/dev/ tty              /dev/ tty                  0 system: /dev/ tty
                                       二U
/devlconsole           /dev/ console              1 system: console
                                       仄U
/dev/i나mx               /dev/ptmx                 2 system
                                       d
                                       1
/dev/ vc/ 0            !dev/ vc/ 0                0 system: vtmaster
s3c2410 serial         /dev/ ttySAC 204           64-67 serial
ser ial                 /dev/ ttyS     4          64小67 ser 나크1
pt y_s I ave            /dev／口ts     136
                                     只니
                                                  아1048575 ［乂y: sI ave
pty rnaster             /dev/ptm                  0-1048575 pty:master
                                     nZ
                                     J1

                                       Q니
pt 兀引 ave              Idevi t typ                0-255 pty: slave
                                       n
                                       ／느 4
口ty_master             Idevipty                   0-255 pty:master
                        /dev/ tty                 卜63 console


위에서 드라이버 명칭이 " s3c2410 serial " 인 것이 필자가 실습하고 있는 삼성 Exynos5420 보드의
UART 드라이버이다． 이 드라이버에 사용자가 접근하는 노드는 " /dev/ttySAC "이고 주장치번호가
204, 보조장치번호가 64에서 67까지 4개가 있음을 알 수 있다．


UART 드라이버는 위의 구조를 구조체（struct）로 상호 연결한다.                                    따라서 UART 드라이버를 이해하
기 위해서는 자료구조（구조체）를 파악하는 작업이 선행되어야 한다.                                           구조체가 어떻게 연결되어 있

                                                   203 / 312
커 널 연구회（www.kern이. b기                                                          정재준 內bi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                 5. UART 드라이버 상세분석                 204




는지 먼저 파악하고 이들을 사용하는 함수의 흐름을 이해하면 UART 드라이버를 정복하기 쉬울
것이다．




5.1 UART 구조체
UART 디바이스드라이버는 include/linux/serial_core.h（게 정의되어 있는 uart driver 구조체를 사용
한다． 이 구조체에서 하위로 연결되는 구조체들의 자료구조를 전체적으로 정리하면 다음과 같댜．
（타원은 구조체명, 화살표는 연결관계）




            미nclude/linux/serial_core.h>




<include/linux/serial_core.h>                                          <indkkde/ linux/tty_driver.h>




이nc山de川nux/                                linux/serial_core.h>        <include/lin, tty_driver.h>




     <include/linux/console.h>   <include/linux/serial core.h>    미nc山de가inux/device.h>


UART 디바이스드라이버는 위의 자료구조에 등록된 정보들을 가지고 동작하므로 위의 구조체들을
잘 파악해 두는 것이 중요하다.                UART 디바이스드라이버의 동작을 이해한다는 것은 위의 구조체
들의 연결관계를 파악하는 과정이다.                   댜음장에서 이 구조체들을 하나씩 기술하겠지만, 이들을 전
체적으로 간략히 정리하면, 먼저 UART 디바이스드라이버는 uart driver 구조체부터 시작하여
uart state 구조체로 연결되어 tty-F兀rt 구조체에서 시리얼 통신 포트들의 정보를 관리한다.                                       시리
얼통신의 실제적인 동작은 uart_port 구조체에 연결되어 있는 uart_ops 구조체에서 이루어진다.
UART 디바이스드라이버와 사용자 어플리케이션과의 인터페이스는 tty_driver 구조체에 연결되어
있는 tty_operation 구조체내의 멤버 함수인 open, write, 向ctl, close 등의 함수들에 의해서 이루어


                                              204 / 312
커널연구회佃ww.ker昶l.bz)                                                    정재준 kgi기3307@nate.com)
Device Tree 상세분석 in 나flux Kernel 4.0                                           5. UART 드라이버 상세분석




진다．




5.2 UART 드라이버 등
              등록
UART 디바이스드라이버가 커널에 등록되는 소스 코드는 drivers/tty/serial/8250/8250_core.c 소스
파일의 ser1a18250_init() 함수에 았다． 이 함수에서 uart_register_driver() 함수를 호출하여 UART
드라이버가 커널에 등록된다．



UART 드라이버 통록 흐룝
             8250 core.c                   serial core.c                              tty_io.c



            ,,：之巴入＼
      (,
           ser ia18250 mnit
                              \\
                                   \
H!1 卜
    「
                                   노
                                       uart_re[} ister_dr iver
                                                                           '
                                                                      \,
                                         寸HM尸Hm中




                                       m如亡났耐 m 計4J   小프 可 느 仰ak針心璉4


                                                                                  tty_register_dr iver


    口1
    」如恤毗已a」
Device Tree 상세분석 in Linux Kernel 4.0                               5. UART 드라이버 상세분석               206




구조체는 8250中core.c 파일내에서 전역 구조체로 다음과 같이 정의 되어 있다．


static struct platform_device *seria18250isadev5;


이 장치를 메모리 할당하여 히計幻rm_devic已add() 함수에 파라미터로 전달하여 커널의 플랫폼
장치로 등록한다．


UART 포트 구조체는 8250 core.c 파일내에서 전역 구조체로 다음과 같이 정의 되어 있다．


static struct uart_8250_port seria18250_ports[UART_NR];


이 구조체는 seria18250_register_ports() 함수에서 등록된다． 마지막으로 히at化rm_driver_reqister()
함수를 호출하여 UART 드라이버를 커널에 등록한다．



5.3 UART 포트 등록
UART 포트 정보는 inc山de加ux/serial_core.h에 정의되어 있는 uart_port 구조체에 저장된다.                              이
구조체에는 시리얼 통신 포트 장치들의 정보가 저장되며, 이 정보는 UART 드라이버가 아obe될 때
실행되는 seria18250_probe() 함수에서 사용자로부터 정보를 전달받아서 저장된다.                               정보를 전달받
는 함수는 dev_get히atdata(）이며 이 함수를 자세히 분석하면 사용자가 설정한 디바이스 정보가
어떤 방식으로 커널에 전달되는지 이해할 수 있다.                            우선 UART 포트가 커 널에 등록되는 전체적인
흐름부터 알아보도록 하자．



UART 포트 吾륙 호묩
            8250 core.c                          serial core.c                 tty如．C



                                         曝箕黛，H1已쁘 ' 1手 r尸1弔크唾的
      sor ia18250_probe


  戶

    戶e/
                                               珏發鉀나‘「乞戈싸努，
                                     /      uar t_add_onepor t


                                                             \
                                    尸




                                                                    \
                                                                        tty_register_ dev1ce
  ser ia18250_register_8250_port                      1r

                                            uart_conf igure_port




                                              206 / 312
커 널 연구회佃ww.kernel.b기                                               정재주 內bi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                      5. UART 드라이버 상세분석           207




sen키8250_probe() 함수는 사용자로부터 넘겨받은 정보들을 uart_8250_port 구조체에 저장한후
ser1a18250_register_8250_port() 함수에게 매개변수로 전달한다.                     이 함수에서 포트정보들을 설정하
여 uart크dd尸one_F兀rt() 함수에게 넘겨서 UART 포트가 등록된다．




5.4 UART 드라이버 동작
UART 디바이스드라이버의 동작은 풀랫폼 드라이버로 등록되어 수행된다.                                        UART 플랫폼 드라이버
구조체는 drivers/tty/serial/8250/8250_core.c 소스 파일에 다음과 같이 정의되어 있다．


stat ic struct platform_dr iver seria18250 isadrjver   =   {
          .probe             = ser ia18250_probe,
          .remove            = seria18250_remove,
          .suspend             ser ia18250_suspend,
          .resume              ser 1a18250_resume,
          .（打 ver              {
                    .name       'ser ia18250 ' ,
         }   ,




．아obe에는 UART 드라이버가 처음으로 인식되어 실행되는 함수（seria侶250_probe ）가 연결된다．
.remove에는 UART 드라이버가 제거될 때 실행되는 함수（seria田250_remove）가 연결된다．
.suspend에는 UART 드라이버 동작을 잠시 멈출 때 실행되는 함수（sen키8250_suspend）가 연결된다．
.resume에는 UART 드라어버 동작이 재개될 때 실행되는 함수（seria侶250_resume）가 연결된다．


위의     구조체는         UART      드라이버가          처음으로              초기화   되는    ser1a18250_init()   함수에서
하at化rm_driv이_register() 함수에 매개변수로 전달하여 커널에 플랫폼 드라이버로 등록된다．




5.5 UART 실행함수들
UART 드라이버의 실행은 tty_operatiofls 구조체에 연결된 함수에 의해서 실행된다. tty_operatioris
구조체는 drivers/tty/seri키八erial_core.c（게서 다음과 같이 실행 함수들이 연결되어 있다．


stat ic const struct tty_operat ions uart_ops = {
          . open              uart_open,
          . close          = uart_close,
          ．나r i te         = uar t베r ite,
          . put_char       = uart_put_char,
          . f lush_chars   = uart_ f ush_chars,
          . write_room     = uart_w ite_room,

                                               207 / 312
커 널 연구회（ww너i.kern이. t끄）                                                   정재준 (rgb日307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                          5. UART 드라이버 상세분석         208




         . chars in buffer   = uar f_chars_ in上山 fer ,
         .f lush buffer      = uart_ f lush_buffer,
              山Cf            = uart_ iocf I ,
          . throttle         = uar I_ throttle,
          .unthroftle          uart_unthrottle,
          . send xchar         uar Lsend_xchar,
          . set termi。 s     = uart_set_ termios,
            set Idisc        = uart_set_ Idisc,
          . stop             = uart_stop,
          . start              uar t_star t ,
          ' hangu口             uar I_hangup,
          . break ctl          uar I_break_ct I ,
          . wait unti l sent = uar t나al t unti 匕sent ,
#1 fdef CONE IG_PROC_FS
          .아0（乙fops          = &uart_proc_ fops,
#endi f
          . t 1 ocmget       = uart_ tiocmgel,
          . f iocniset         uart_ t iocmset,
#jfdef CONEIG CONSOLE POLL
          . p01匕 m it          uar I_pol l_ in i
          刃01匕get_char         uart_pol I_get_char ,
          . pol 匕口Ut char      uart_pol I_put_char ,
#endi f
};

사용자가 UART 디바이스드라이버를 open하여 write, ioctl, close 등의 작업을 실행하면 위의
구조체 멤버 변수에 연결되어 있는 함수들이 실행된다．


지금까지 UART 드라이버가 커널에 등록되는 과정을 전체적으로 간략하게 요약하여 정리했다．
이것으로 UART 드라이버가 어떻게 구성되어 있는지 전체적인 설계도는 파악할 수 있을것이다．
이것을 바탕으로 다음장부터 좀더 자세하게 UART 드라이버를 분석하도록 하자．




                                                  208 I 312
커널연구회佃w毗ernel.bz)                                             정재준 (rgl이3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                           6. UART 구조체       209




6. UART 구조처I




                                                   弗 필자의 주말농장에서 찍은 장미꽃




UART 구조체는 uart나driver 구조체에서 아래와 같은 계층구조로 연결되어 있다.                 이번장은 이들
구조체에 대해서 상세히 설명한다．




                                       209 / 312
커널연구회佃ww.kernel.b기                                     정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                              6. UART 구조체     210




               <include/linux/serial_core.h>




<inc山de/linux/serial_core.h>                                        이nclude/linux/tty_driver.h>




이nc山de川nux/tt




 이nclude/linux/conso e. > <include/linux serial_core.h> <inc u.e inux/device.h>




6.1 uart_driver 구조체
uart 드라이버를 표현하는 가장 상위단의 구조쳬로서 이nc山de川nux/serial_core.h＞에 다음과 같이
선언 되어 있다. （주석문으로 설명함）




struct uart_driver {
         struct module       六0놔ner ;          /／모듈 소유자 구조체
         const char          *dr i ver name;   /／드라이버 이름
         const char          *dev name;        /／장치 이륨
         rn t                major;            /／주번 호
         1 nt                minor ;           /／보조번 호
         1 nt                nr;               /／가녀느
         struct console      *c0ns ;           /／콘솔 구조처1

         /／火

          女 아래 구조체들은 private: 10邪 level 드라이버는 이 구조체에 접근하지 않음，
          亥 이듈은 NULL로 초기화 되어야 함．

        struct uart state *s1a1e;
        struct tty_dr iver *tfy driver;
};


                                               210 / 312
커 널 연구회佃ww.kernel.b기                                               정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                              6. UART 구조체     211




uartmdriver 구조체는 drivers/tty/seri키肥250/8250工ore.c내의 전역 구조체이며 컴파일 할따1 아래와
같이 초기화 된다．


static struct uart_driver 5eria1825()_reg = {
         . owner                    = THIS_MODULE,
         , driver name              = "ser 나｝1 n ,
         .dev name                  = "ttyS" ,
         . maj or                   = TTY_MAJOR.          1/ 4
         . minor                    =64,
         . cons                     = SERIAL8250_CONSOLE. //NULL
};




6.2 cons이e 구조체1
cons이e 구조체는 디nc山e川flux/clDns이e.h＞에 다음과 같이 선언되어 있다．



con＄아e 구조체1
struct console {
         char     name[ 161;
         void     (*write)(struct c(insole *, coast char *, unsigned) ;
         mnt      (*read) (struct c。  i isole *, char *, unsigned) ;
         struct tty_driver *(*devic())(struct console *, i nt *);
         void     (*unblank) (void) ;
         mnt      （出seth口）(struct cc)nso陀 出 , char 士） ;
         나lt     卜ear IL羽tup) (vo d) ;
         short    flags;
         short     index;
         m4t      cflag;
         void     *data;
         struct console *nexf;
};




6.3 uart_state 구조체
uart 드라이버의 상태 정보를 표르쳔하는 구조체로서 시nc山de가inux/serial_core.h＞에 다음과 같이
선언되어 있다．



struct uart_state {
         struct tty_ 均rt            port;

         mnt                        미兀state;
         struct circ but            xmit ;

                                               211 / 312
커 널 연구회（www.kerr倒. b라                                                     정재준 岫bi3307@nate.con가
Device Tree 상세분석 in Linux Kernel 4.0                                    6. UART 구조체    2任




       struct taskiet struct       tlet;
       struct uart_port            *uar t_por t ;
};




6.4 tty_driver 구조체
tty 드라이버를 기술하는 구조체로서 <include加ux/tty_driver.h＞에 다음과 같이 선언되어 있다．


struct tty_driver {
         i nt              magic;            /／이 구조체를 위한 sag i c 번호
         struct kref       打ef;              /／참조 관리
         struct cdev       cdev;
         struct modu 陀     火0빠ner ;
         const char        士driver name;     /／드라이버 명칭
         const char        *name;
         in!               name base;        /／출력되는 명칭의 오프셋
          mnt              major ;           /／주 장치 번호
          mnt              minor start;      /／보조 장치 번호의 시작
          t nt             씨nor num;         /／가능한 장치들의 수
            nt             num;              /／할당된 장치들의 개수
         short             type;             //tty 드라이버의 형태
         short             subty口e;          i/ tty 드라이버의 보조 형태
         struct ktermios    init_termios;    I/ Initial termios
          mnt              flags;            //tty 드라이버 퓰래그
         struct 아oc_di r_entry       챠玎oc_entry; // /proc Is 진입지점
         struct tty_driver           火other;       iIPTY 드라이버률 위해 사용됨

        //t ty 데이터 구조체 포인터
        struct tty_struct **ttys;
        struct ktermios **termios;
        struct ktermios 火火termios locked;
        void              *driver state;

        /／드라이버 me比ods
        const struct tty_operat ions   *ops;
        struct l ist_head              tty_drivers;
};




6.5 tty_port 구조체
tty 포트를 기술하는 구조체로서 미nc山de加ux/tt沖＞에 다음과 같이 선언되어 있다．




                                                212 / 312
커널연구회佃ww.kerne나）기                                              정재준 的1이3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                                          6. UART 구조夫II堪特




struct tty_port {
         struct tty_struct         켜tty;                   f/Back 포인터
         const struct tty_port _operdt ions *ops;          사포트 동작들
         S이 nlock_ t                 l。 ck:                f/ tty 공유자원 보호를 위한 락킹
          mnt                       t locked_open;         /／열기 위한 대71
          } nt                      b。  unt;               月걔수
         咐ait_queu已head_ t           open巾싸alt  ·，         月열기 대기자
         놔alt.시ueue_head_ t         이ose wait;             /／닫기 대기자
         wa I t_queue_head_t         delta msr 叫i크i 1;     /／모뎀 상태 변경
         unsigned long               flags;                //TTY flags ASY
         unsigned char               console: 1;           /／포트 콘솔
         struct ml八ex                mutex ;               가락킹
         struct mutex                buf mutex;            /／버퍼 할당 랒
         unsigned char               士xmit but ;           사선택적 버퍼
         unsigned in!                close_delay;          /／닫기 포트 지연
         unsigned in!               이 0s1ng川alt ;          /／출력을 위한 지연
          i nt                      （打am4이ay;
         struct kref                 kref;                  /／참조 회수
};




6.6 uart_port 구조체
uart_port 구조체는 이nclude加ux/serial_core.h＞에 다음과 같이 선언되어 있다．



uart_port 구조체

struct uart_port {
         spin lock_ t                lock;                           ,／六 port lock 士／
         unsigned long               lobase;                         1* in!out[ bwl] */
         unsigned char _iomem        出membase;                       ／出 read!wr I te[ bwl ] 升／/
         unsigned mnt                (*serial_ ln) (struct uart_port 士, 1 nt) ;
         void                        (*serja匕out) (struct uart_port 六, i nt, int) ;
         void                        (*set_ termios) (struct uart小port 火,
                                                       struct ktermios 女ne札
                                                       struct ktermios *old) ;
         void                        (*set_mctrl) (struct uart_port 士 , unsigned i nt) ;
         int                         (*startup) (struct uart_port *port) ;
         void                        (*shutdown) (struct uart_port *port) ;
         void                        (* throttle)(struct uart_port *port) ;
         void                        (*unthrottle)(struct uart_port *port) ;
         mnt                         （士handle 나cl) (struct uart_port 火） ;
         void                        (*pm) (struct uart_port *, unsigned mnt state,
                                              unsigned mnt old) ;
         voi d                       (*handlebreak) (struct uart_port *);
         mnt                         (*rs485c0nf1g) (struct uart_port 出,
                                                          struct serial_rs485 *r5485) ;
         unsigned mnt                汁q;                  /／古 irq number 六／'
         unsigned long               나qf lags;            ／亥 I rq ! lags 士／'
         unsigned mnt                uartc나C,             ／大 base uart 아ock 大／
         unsigned 1 nt               fIt os I ze;         /‘出 tx fito 引ze 火／


                                                     213 / 312
커 널 연구회（w'사w.kernel.b기                                                          정재준 (rgbi3307@nate.com)
Device Tree 상세분석 ir) 니flux Kernel 4.0                                                          6. UART 구조체   214




         unsigned char                 x char ;            f* xon/ xoff char */
         unsigned char                 regshift;           ／士 reg offset shift 古／
         unsigned char                 iotype;             ／火 1 o access s押沌 士／
         unsigned char                 unusedi;

#define UPIO PORT             (SERIALIO_PORT) 1* 8b I/ O port access */
#define UPIO_HUB6             (SE이AL그0刈B6) ／士 Hub6 ISA card */
#define UPIO MEM              (SER I赴그0_MEM)               ／火 8b 秘MIO access 火／
#define UPIO MEM32            (SERIAL_ IO_MEM32) 1* 32b l ittle endian */
#define UPIO_AU               (SERIAL_ b )_AU)             7* Au1xOO and RT288x type i 0 古/
#define UPlO_TSI              (SERIAL_ IO_TSI)             1* lsil08/109 type 10 火7
#def m e UPIO_MEM32BE         (SERIALIO..MEM32BE)          /* 32b big endian *7

         unsigned i nt                 read status mask; ／『火 driver s口ec；나 IC 火／/
         unsigned i nt                 ignore_status_mask;         /／火 driver s口ec나 Ic 士／/
         struct uart state             火state;                     ／火 r兀inter to parent state 火／
         struct uart icount            icount;                     1六 statistics 士7

            struct console                 *cofls;                       7士 struct console, if any *7
#1 f def i ned( CONF I G_SER I AL_CORE_CONSOLE) I I def i ned( SUPPORLSYSRQ)
            unsigned long                  sysrq;                        /* sysrq timeout *1
#endif

         /／女 flags must be updated whi le holding port mutex 火1
         u아J                         flags;

                                                                                        d1
#define UPF FOURPORT                   ( (_ force upf_ t) ASYNC FOURPORT
                                                                                    士




                                                                                        n
                                                                                        ／나 4
#define UPF SAK                        ( (_ force upf_ t) ASYNC SAK
                                                                                    士




#define UPF SPD HI                     ( (_ force upf_ t) ASYNC SPD HI         /／火 4 女／/
                                                                                    火



                                                                                        二U
#define UPF SPD VHI                    ( (_ force upf_ t) ASYNC SPD VH I       ／亥 5 火／
                                                                                    玄




#define UPF SPD CUST                   ( (__force upf_ t) ASYNC_SPD_CUST   7* OxO030 */
#define UPF SPD WARP                   ( (_ force upf_ t) ASYNC SPD WARP ／士 Ox化化 乞／
#define UPF SPD MASK                   ( (- 化rce u아_ t) ASYNC_SPD_MASK     1* Ox1030 乞
#define UPF SKIP TEST                  ( (_ torce upf_ t) ASYNC_SKIP_TEST      7* 6 *1
#define UPF AUTO IRQ                   ( (_ force upf_ t) ASYNC_AUTO_ I RQ     ／士 7 出／/
#def m e UPLHARDPPSCD                  ( (_ force upf_ t) ASYNC_HARDPPS_CD     1大 11 */
#define UPF SPD SHI                    ( (_ force upf_t) ASYNC SPD SHI         ／火 12 屯／
#def i ne UPLLOLLATENCY                ( (_ force upf_ t) ASYNC_LOWLATENCY     7女 13 */
#define UPF BUGGY UART                 ( (_ force upt_t) ASYNC_BUGGY_UART      ／出 14 치／
#define UPF NO TXEN TEST               ( (_ force upf_t) (1 << 15) )
#define UPF MAGIC MULTIPLIER           ( (_ force upf_ t) ASYNCMAGIC_MULTIPLIER 7古 16 */ )

/* Port has hardware-assisted h/ w f m바 control 士／
#define UPF AUTO CTS                  ( (_ force upf_ t) (1 << 20) )
#define UPF AUTO RTS                  ( (_ force upf_ t) (1 << 21) )
#define UPF HARD FLOW                 ( (_ 化rce U口f_ t ) (UPF_AUTOCTS I UPFAUTORTS) )
7* Port has hardware-assisted s/ w f low control *7
#define UPF SOFT FLOW                 ( (_ force upf_ t) (1 << 22) )
#define UPF CONS FLOW                 ( (_ force upf_ t) (1 << 23) )
#def m e UPF_SHARE_ IRQ               ( (H化rce u口f느t) (1 << 24) )
#define UPF EXAR EFR                  ( (_ torce upf_ t) (1 << 25) )
#define UPF BUG THRE                  ( (_ force upf_t) (1 << 26) )
7玄 The exact UART type is known and should not be probed. *7
#define UPFFIXEDTYPE                  ( (_ force upf_ t) (1 << 27) )
#define UPF_BOOT_AUTOCONF             ( (__force upf_t) (1 << 28) )
#det ine UPF_FIXED_PORT               ( (_ force upf_ t) (1 <<29) )

                                                   214 / 312
커 널 연구회（www.kern이.b기                                                            정재준 (rgbi3307@nate.cori力
Device Tree 상세분석 iF) 니flux Kernel 4.0                                                      6. UART 구조체n2求丘難小



#define UPF DEAD                        ( (_ force upf_ t) (1 << 30) )
#define UPF I0REMAP                     ( (_ force upf_ t) (1 << 31) )

#def m}e UPF CHANGE MASK                0x17f ft
#define UPF CHANGE MASK                 ( (- 化rce upf_t) 小UPF_CHANG巳MASK)
#define UPF USR MASK                    ( (_ force upf_ t) (UPF_SPD_MASKIUPF_LOW_LATENCY) )

#if -寸UP巳CHANGE긔ASK > ASYNC FLAGS
#error Change mask not equivalent to userspace-visible bit def ines
#endi f

         ／士
              * Must hold terrnios rwsem port mutex and port lock to change;
              * can hold any one lock to read.
              火／
         upstaLt              status;

#def i ne UPSTAT_CTS_ENABLE             ( (._force upstat_ t) (1 << 0) )
#define UPSTAT DCD ENABLE               ( (_ force upstat t) (1 << 1) )
#define UPSTAT AUTORTS                  ( (_ force upstat_t) (1 << 2) )
#define UPSTAT AUTOCTS                  ( (_ force upstat_t) (1 << 3) )
#define UPSTAT AUTOXOFF                 ( (_ force upstat_t) (1 << 4) )

         I nt                        h叫5加pped;             1出 sw-assisted CTS f low state */
         unsigned 나lt                mctrl ;                ／升
                                                              current modem ctrl settings */
         unsigned m 1t               timeout;               ／士
                                                              character-based timeout *1
         unsigned mnt                type;                  ／火
                                                              port ty口e 士／
         const struct uart_ops       士야）5;
         unsigned mnt                custom 비미sor ;
         unsigned mnt                l ine;                ／出    口ont index 玄／
         resource size t             mapbase;               ／六
                                                                 for ioremap */
         struct device               *dev;                  ／士
                                                                 口arent device 出／
         unsigned char               hub6;                  ／火
                                                                 this should be in the 8250 driver 士1
         unsigned char               suspended;
         unsigned char               I rq州ake;
         unsigned char               unused[ 21;
         struct attribute_group      *attr_gr0up ;                   1* port specific attributes */
         const struct attr 仕）ute_grou口 出士t ty_groups;      ／火 al t attributes (serial core use only) *1
         struct seria匕r5485           rs485;
         void                        士private느data;                   ／士 generic 이at化rm data pointer 士／
};




6.7 uartf250_ 兀rt 구조체
uart_8250_t兀rt 구조체는 inc山de川nux/serial_8250.h 소스파일에 다음과 같이 선언되어 있다．



uart8250_port 구조체
struct uart_8250_port {
         struct uart_port               口ort ;


                                                   215 / 312
커 닐 연구회 (ww＼사．kern飢b기                                                           정쟤준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                     6. UART 구조체1




         struct timer l ist            timer;               ／士 "' no irq'' tinier 火／
         struct l ist head             l ist;               ／出 ports on this IRQ 士／
         unsigned short                capabi l ities;      ／火 口ort capabi l ities 火／
         unsigned short                bugs;                ／玄 port bugs 女／
         boo I                         f i fo_bug;          ／士sin RX trigger if enabled */
         unsigned in!                  tx loadsz;           It transmit fifo 比ad 읽ze 士／
         unsigned char                 acr;
         unsigned char                 fcr;
         unsigned char                 ier;
         unsigned char                 1cr ;
         unsigned char                 mcr;
         unsigned char                 mcr mask;            ／火 mask of user bits 士／
         unsigned char                 mcr force;           ／女 mask of fc나cad bits 火／
         unsigned char                 cur_10type ;         ／火 Running I/ O type 大／
         unsigned mnt                  rpm_tx_active;
         unsigned char                 canary;              f士 non-zero during system sleep
                                                                 if no_console_suspend
                                                             火/



         ／出

          升 Some bits in registers are cleared on a read, so they must
          * be saved 싸henever the register is read but the bits wi l l not
          * be immediately processed.
          士/

#def i ne LSR SAVE FLAGS UART LSR BIlK ERROR BITS
           unsigned char               lsr_saved_ f lags;
#define MSR SAVE FLAGS !JART_MSR_ANY_DELTA
           unsigned char               msr_saved_f lags;

         struct uart 8250 dma          *dma;

         ／古 8250 s口ed! IC Cal 山acks 玄／
         mnt                        (*dl_read) (struct uart_8250_port *) ;
         void                       (*d匕write) (struct uart_8250_port 士 , int) ;
};
6.8 tty_operat泊ns 구조체
tty_operat向ns 구조체는 tty 계층에서 동작하는 함수들을 <inc山de기inux/t寸_driver.h＞에서 다음과
같이 선언한다．




struct tty_operations
         struct tty_struct * (* lookup) (struct tty_driver *driver,
                             struct m ode *inode , mnt idx) ;
          mnt (* instal l)(struct tty_driver *driver, struct tty_struct *tty) ;
         void (*remove) (struct tty_driver *driver, struct tty_struct *tty) ;
          m } t 卜0口en) (struct tty_struct 士 tty, struct fi le 火 fi 比）) ;
         vo汨 （火close) (struct tty_struct 火 tty, struct fi le 女 fi 巾）;

                                                  216 / 312
커 널 연구회（www.kern이. b기                                                         정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                                     6. UART 구조체




           黑    (*shutdown) (struct ttyHstruct *tty) ;
                (*cleanup)(struct tty_struct *tty) ;
           m
                (*write)(struct ttystruct * tty,
                           consf unsigned char *buf, 1 nt count) ;
          int (*put_char) (struct tty_struct *tty, unsigned char ch) ;
         vo뗘卜f lus九ch카s) (struct tty_struct 士tty) ;
          mnt (出write_room) (strucl tty_struct *tty) ;
          1nt (士chars_ in_buffer)(struct tty_struct *tty) ;
          mnt (* ioctl)(struct ttystruct *tty, struct fi le * fi le,
                         unsigned mnt cad, unsigned long arg) ;
          long (士compat_ ioctl) (struct tty_struct *tty, struct fi le * fi le,
                                     unsigned mnt cad, unsigned long arg) ;
         void (*set termios) (struct ttv struct *ttv . struct ktermios * old) ;
         voia t 士rnrollle) ,srrucl ity_siruci * 11yJ 1
          void (*unthrottle) (struct tty_struct * tty) ;
          void (*stop) (struct tty_struct *tty) ;
          void (士start) (struct tty_struct *tty) ;
          void (士hangup) (struct tty_struct *tty) ;
           mnt (*breakctl)(struct ttj_struct *tty, in! state) ;
          void (女flush-Hbuffer) (struc tty_struct *tty) ;
          void (*set_ ldisc) (struct t y_struct *tty) ;
          void (*wait unti l sent) (st uct tty_struct *tty, in! timeout) ;
          void (*send_xchar) (struct ty_struct *tty, char ch) ;
           mnt (士tioc旺｝et)(struct tty_struct *tty, strucf fi le *fi le) ;
           mnt (* tiocmset)(struct tty_struct *tty, struct fi le *fi le,
                                unsigned mnt set, unsigned in! clear) ;
           mnt (*resize) (struct tty_s ruct *tty, struct winsize *ws) ;
           in! (*set_ termiox) (struct ty_struct *tty, struct termiox *tnew) ;
#i fdef CONFIG_CONSOLE_POLL
           mnt (*pol l_ mnit) (struct tty_driver 出driver, i nt l ine, char *options) ;
           mnt (*pol l_get_char) (struct tty_driver *driver, mnt l ine) ;
          void (*pol l_put_char) (struct tty_driver *drjver, nt l ine, char ch) ;
#endi f
          const struct fi le_operations *proc_ fops;
};
6.9 uart_ops 구조체
uart_ops 구조체는 UART의 물리적인 장치에서 동작하는 함수들을 <Inc山de/linux/serial_core.h＞에
서 다음과 같이 선언한다．



uart_ops 구조채
s나uct uar Lops {
        unsigned mnt         (* tx_empty) (struct uart_port *) ;
        void                 (*set_mctr l)(struct uart_port *, unsigned in! mctrl) ;
        unsigned in!         (*get_mctr l)(struct uart_port *) ;
        void                 （士St야냐x) (struct uart_port 出） ;
        void                 (*start tx) (struct uart中port *);
        void                 (*send_xchar) (struct uart_port 士, char ch) ;

                                                  217 / 312
커 널 연구회（wwv吐ernel.bz)                                                         정쟤준 四b日307@nate.com)
Device Tree 상세분석 II) 니flux Kern& 4.0                                                        6. UART 구조체   218




         void                 （士sto口rx) (struct uarLport 士）;
         void                 (*enablems) (struct uarLport *) ;
         void                 (*breakctl)(struct uarLport 出 , m} t ctl) ;
         mnt                  (*startup) (struct uart. port *);
         vo d                 （女shut（幻wn) (struct uart_i川t 火） ;
         vo d                 (*flush_buffer)(struct uarLport *) ;
         void                 (*set_ termios) (struct uart .port 女, struct ktermios *new,
                                                struct kterrnios 士이d) ;
         void                 （女set그비印) (struct uart_port 出）;
         void                 (*pm) (struct uart..port 士 , unsigned mnt state,
                                     unsigned mnt oldstate) ;
         mnt                  (*set_wake) (struct uart_port *, unsigned mnt state) ;

         ／出
              * Return a string describing the type of the port
              士／
         coast char *(* type) (struct uart..port *) ;

         ／女
              * Release tO and memory resources used by the port.
              * This includes iounmap if necessary.

              。v'   id        (*reteaseport)(struct uart..port *);

         ／玄
              * Request 10 and memory resources used by the port.
              * This includes iomapping the port if necessary.
              士／
          i nt             (士request_porl)(struct uart..port *);
         void              (*configport)(struct uart.port 火, int) ;
          mnt              (士verifyport)(struct uart.port 女, struct seriat_struct *);
          mnt              (* ioc(t)(struct uart_port 士, unsigned int, unsigned long) ;
#i tdef C아FIG_CONSOLE_POLL
         void     (朴）ot 냐）ut char) (struct uart_port *, unsigned char) ;
          mnt              (士pol t_get_char) (struct uart_port *);
#end if
};
6．伯 tty_struct 구조체
tty_struct 구조체는 미ac山de기inux/tty.h＞에 다음과 같이 선언되어 있다．



t勺_struct 구조쳬
struul tty_struct {
         1 nt      magic;
         struct kref kret;
         struct tty_driver *driver :
         c거｝st struct tty_operat ions *ops;
         1 nt index;

        ／出 마이的始 1 disc changes: Lock tty not p如

                                                  218 / 312
커 널 연구회佃ww.kern이.b기                                                          정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kern이 4.0                                                   6. UART 구조체1




        struct mutex disc mutex;
        struct tty_ k키Sc 시dis（二

        struct mutex termios mutex
        spinlock_t ctrl_ lock;
        ／士 Termios va山es are 口！乙t cted by the termios mutex 士1
        struct ktermios *termjos, 打ermios_ locked;
        struct termiox 士termiox; 1士 May be NULL for unsupported 火1
        char nane[ 64];
        struct pid 火pgrp;                            ctrl lock 火／
        struct pid 士sess ion;
        unsigned long flags;
         nt count;
        struct winsize winsize;               7* termios mutex */
        unsigned char 計op口ed:1 , h町없야）pedl , I lo叫stop口ed:1 , 口acket :1;
        unsigned char low_ latency:1, warned:1;
        unsigned char ctr匕st카us; ／火 ctr i_ lock 卞／
        unsigned m } t receive_room; ／北 Bytes free for queue 乞／

        struct tty_struct *1 ink;
        struct fasync_struct *fasy c ;
        stru아 tty－上U什'ead buf;                 ／火 Locked internal ly 士／
        in! alt_speed;                 7* For magic substitution of 38400 bps *7
        wai t_queu乞head_ t 나r i te川alt ;
        卄ai t_queu已head_ t read_나ai I ;
        struct work_struct hangup_work;
        void *djsc data;
        void *driver_data;       I/ st
        struct l ist_head tty_fi les

#define N_TTY_BUF_SIZE 4096

         ／出
              t The fol lowing is data f)r the N_TTY l ine discipl ine. For
              * historical reasons, thi is included in the tty structure.
              * Mostly locked by the BKI..
              出／                       1
        unsigned 나｝t column;
        unsigned char lnext:1, erasrng:1, raw:1 , real_raw:1 , icanon:1;
        unsigned char closing:1;
        unsigned char echo_overrun "i;
        unsigned short minimum_ to_wake;
        unsigned long overrun_ time
        in! num overrun;
        unsigned long 아oces乞ch카小a口［256/（小引ze이如陌띠ned long) )] ;
        char *rearjJ,uf;
        in! read_head;
        mnt read_ tai l ;
        in! read_cnt;
        unsigned long read_f lags[ N_TTY_BUF_SlZE/ (8士sizeot (unsigned long) )];
        unsigned char *echo_buf;
        unsigned mnt echo_pos;
        unsigned in! echo_cnt;
        mnt canon data;
        unsigned long canon_head;
        unsigned mnt canon_column;

                                                  219 / 312
커 널 연구회（너／납／＼사．kernel.bz)                                                     정쟤준 (rgbi3307@nate.con卄
Device Tree 상세분석 in Linux Kernel 4.0                                          6. UART 구조체      220




          struct mutex atomic read lock;
          struct mutex atomic write lock;
          struct mutex output_ lock;
          struct mutex echo lock;
          unsigned char *write_buf;
           mnt write_cnt;
          spinlock_t read_ lock;
          I火 If the tty has a pending do_SAK, queue it here - akpm
          struct work_struct SAK_work;
          struct tty_port *p0rt ;
};
6.1] ktern）油S 구조체
ktermios 구조체는 아키텍처 의존적이며 <arch/arm八nc山de/asm/termbits.h＞에 다음과 같이 선언

되어 있다．



khm奴 쿠玉川
struct ktermios {
         tcflag_ t c_if lag;        /* input node flags */
         tcf lag_ t c_of lag;       /* output mode flags 火 /
         tcflag_ t c_cf lag;        ／火 control mode flag$ 士／
         tcf lag_ f c_ I f lag;     /* local mode flags */
         cc t c l ine;              ／六 l ine discipl ine 士／
         cc_t c_cc[ NCCS] ;         /* control characters t /
         speed_ t c_ ispeed;        ／火 input speed 古／
         speed_t c_ospeed;          ／士 out口ut 5口eed 出／
};
6.12 uart_icount 구조처1
이nc山de기inux/serial_core.h>（게 다음과 같이 선언되어 있다．


struct uart_ icount {
           u32     아s;
           u32     dsr;
           u32     mng;
           u32     dcd;
           u32     rx;
           u32     tx;
           u32     frame;
         _u32      overrun;
         _u32      parity;
           u32     brk;

                                              220 / 312
커 널 연구회佃w니／.kern이.b기                                                 정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                           6. UART 구조체     221




                         u32   buf overrun;
};




6.13 tty_Idisc 구조체
tty line discipline 구조체인 啣J비乳는 시nclude加ux/ttyl비sc.h＞에 다음과 같이 선언되어 있다．


struct tty_ ldisc_ops {
         mnt       magic;
         char      *flame;
          mnt      nurn
          mnt      flags;

          ／士
                    * The fol lowing rout ines d recal led from above.
                    士/
         mnt      (*open) (struct tt) struct 火） ;
         void     (*close) (strucf tt 止struct 出） ;
         vo뗘      （町 i us比but fer)(st ruct tty_struct *tty) ;
         ssize_ t (*chars in buffer) (struct tty.+struct *tty) ;
         ssize_ t (*read) (struct tty struct * tty, struct fi le * fi le,
                            unsigned char _user * but, size_t nr) ;
         ssize_ t (*write) (strucf tt y_struct * tty, struct ti le * fi le,
                              const ur 引gned char 出 buf , 引ze_ t nr) ;
         mnt      (* ioctl)(struct tt 兄struct 出 tty, struct fi le 出 fi le,
                              uns I gnec mnt crnd, unsigned long arg) ;
         long     （士corn口at_ioctl) (st ruct tty_struct * tty, struct fi le * fi le,
                                          jnsigned mnt cmd, unsigned long arg) ;
         void     (*set termjos) (str uct tty_struct *tty, struct kterrnios * old) ;
         unsigned 1 nt (*pol l) (strucl tty_struct 火, struct fi le *,
                                    St IL ct 口oI l_ta비乞struct 女） ;
         mnt      (*hangup) (struct I ty_struct *tty) ;

               ／士
                    * The fol lowing routines E recal led from below.
                    出／
          void                  (*recejvebuf)(str uct tty_struct 出, const unsigned char 士cp,
                                                  c1 ar *fp, 1 nt count) ;
          void                  (*wr ite_wakeup) (sl ruct tty_struct *);
          void                  (*dcd_change) (stri Cf tty_struct 士 , unsigned nt,
                                                     struct tirnespec *) ;

          struct               In얘u 陀 火0네ner ,’

               tnt refcount;
};
struct tty_ ldisc {
         struct tty_ ldisc_ops *ops;
         at에ic t users;


                                                           221 / 312
커 널 연구회 (www.kern이.b기                                                                정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                               6. UART 구조체1蛇茗珥二




tty_Idisc_ops 구조체는 drivers/char/n_t勺（에 다음과 같이 선언되어 있다1


struct tty_ ldisc_ops tty_ ldisc_N_TTY = {
         . magic             = TTY_LDISC_MAGIC,
         . name              = 'n_ tty ' ,
         . open              = n_tty_open,
          . close            = n_ tty_close,
          . flush_buffer     = n_tty_f lush_buffer,
          . chars_ in_buffer = n_tty_chars_ in_buffer,
          .read              = n_ tty_read,
          . write            = n_tty_write,
          . ioctl            = n_tty_ ioctl ,
          .set_ termios      = n_ tty_set_termios,
          . pol l            = n_tty_ 均l I ,
          .receive_buf       = n_ tty_receive_buf,
         ．놔ri te叫akeu口       = n ttL나r i te_wakeup
};




6.14 t勺上uffer 구조체
<inc山de加ux/tty.h＞에 다음과 같이 선언되어 있다．


struct tty_buffer {
         struct tty_buffer *next;
         char *thar1buf_ptr;
         unsigned char *flag_buf_ptr;
         1 nt used;
          mnt 引 ze;
          mnt commit ;
          mnt read;
         ／士 Data points here 士／
         unsigned long data[ O];
};
struct tty_bufhead {
         struct delayed_work work;
         spinlock_t lock;
         struct tty_buffer *head; ／士 伽eue head 士／
         struct tty_buffer *tai I ; ／女 Act ive buffer 士／
         struct tty_buffer *free; ／士 다ee queue head 士／
          mnt memory_used;          /* Buffer space used excluding tree queue 火／
};




                                                  222 / 312
커 널 연구회（www.kern이.b기                                                   정碍준 (rgbi3307@nate.cori가
Device Tree 상세분석 in Linux Kernel 4.0                                                6. UART 구조체     223




6.15 기타 구조체
UART 디바이스드라이버에서 보조적으로 사용하는 기타 여러가지 구조체들은 다음과 같다．




6.15.1 cdev 구조체
시nc山de川nux/cdev.h>


struct cdev {
         struct k아기印t k야기 ;
         struct module 火0벼ner ;
         const struct fi le_operat 山ns 大야）5,
         struct l ist head l ist;
         dev t dev;
         uns} gned mnt count ;
};
6.15.2 히at化rm中 구조체
<include/linux/platform_device.h>


struct platform_device {
         const char         *flame ;
         mnt                id;
         struct device      dev;
         u32                num_resources;
         struct resource    *res0urce ;
         const sfruct platform_device_ id       火 (f_entry ;
         ／火 arch specif ic addi t 山ns 文／
         struct pdev_archdata         archdata;
 };
struct platform_driver {
           nt (*probe) (struct platform_device *) ;
           nt (*remove) (struct platform_device *) ;
         vo뗘 （士shutdo叫n) (struct platform_device 出） ;
         mnt (*suspend) (struct platform_device *, pm_message_ t state) ;
          jnf (*resume) (struct platform_device *) ;
         struct device driver dr iver;
         const strucf platform_device_ id *id table;
 };
                                                  223 / 312
커 널 연구회（www.kernel.b기                                                       정재준 的bi3307@nate.com)
Device Tree 상세분석 In 니flux Kernel 4.0                                                  6. UART 구조체   224




6.15.3 procmdir_entry 구조체
<include/linux/proc_fs.h>


struct 아oc펴나_entry {
        unsigned mnt low_ m o;
        unsigned short namelen;
        const char *name;
        mode_ f mode;
        nh ink_ t nl ink;
        山d t uid;
        q i d_ t 이d;
        loft t 引ze;
        const struct 1 node_operations 女아oc i叩s;

         const struct fi le_operations *proc_fops;
         struct 아oc_di r_entry 六next , 朴）arent , 火subdir ;
         void *data;
         read_f玎oc t 士read.j片oc;
         wr I tej汗oc t 士나r i te.j玎oc;
         atomic_ f count;              /* use count */
         mnt 口de_user 5;      ／火 number of cal lers into modu陀 汀｝ 아ogress 火／
         spinlock_ t pd巳山load_ lock; ／大 아oc f叩s checks and 口de_users bumps *7
         struct completion 사）cje--unloadecomplet ion;
         struct l ist head 口de_opener 5;         ／大 咐｝o did ->0口en, but n아 ->release 六／
};
6.15.4 州e,,，多perat油ns 구조체
디nc山de기inux/fs.h>


struct f i le_operations {
          struct modu比 火0叫ner ;
           loff_t (* l lseek) (struct fi le 女, loff_ t, i nt) ;
          S읽四J （出read) (struct ti le 女 , char __user 士 , 引ze_t, IofLt 火） ;
          5引ze t （出나rite) (struct fi le 士 , const char _user 出 , 引ze_ t, loff t 出） ;
          ssizet (*aio_read) (struct kiocb *, const struct lovec 士, unsigned long, loff_ t) ;
          ssizet (*aio write) (struct kiocb 出, const struct iovec *, unsigned long, lotf_ t) ;
           mnt (*readdir) (struct fi le 出, void *, j l ldir_ t) ;
          unsigned mnt （사）oI l) (struct fi le 士 , struct pol l_ ta비巳없ruct 士） ;
           mnt (* ioctl) (struct m lode 女 , struct fi le 士, unsigned int, unsigned long) ;
           long (*unlocked4 ioctl) (struct fi le 六, unsigned int, unsigned long) ;
           long (出c에｝pat_ ioctl) (struct fi le 出, unsigned int, unsigned long) ;
           mnt (*mmap) (struct fi le 士, struct vm_area_struct *);
           mnt (*open) (struct mnode 火, struct fi le *);
           m } t (士f lush) (struct fi le 士, fl_owner_ t Id) ;
           mnt (玄release) (struct mnode 士, struct t i le *) ;

                                               224 / 312
커 널 연구회（w\사w.kern이.b기                                                    정재준 （呼)i3307@nate.com)
Device               Tre   ,   상세분석 i, 니, , ,   Ker   h,   4.   0                             6. UART 구조채




              m }l (* fsync) (struct fi le *, 1 nt datasync) ;
              mnl (*aio_fsync) (struct k ocb 士 , i nt datasync) ;
              m ) t (* fasync) ( int, struct fi le *, i nt) ;
              mnt (* lock) (struct fi le * mnt. struct fi le_ lock *);
              S引ze t （士sendpage) (struct fi le 火 , struct 口age 士 , mnt , 引ze- t , lot f_f 士 , int) ;
              unsigned long (*get_unmappd_area) (struct fi le *, unsigned long, unsigned long, unsigned
     long, unsigned long) ;
              나｝t （女check小flags) ( i nt) ;
              mnt (* f lock) (struct fi le + , i nt, struct fi le_ lock *);
              ssize_ t (*spl ice_write) (struct pipe_ mnode_ info *, struct fi le *, loft_ f *, size_ t, unsigned
      nt) ;
              ssize_ t (*spl iceHread) (strucf fi le *, loft_f *, struct pipe_ mnode_ info 女, size_t, unsigned
      nf) ;
              mnt (*setlease)(struct fi le *, long, struct fi le_ lock **) ;
         };
         6.15.5 work struct 구조：눼
         디nclude/linux/workqueue.h>


         struct 베0댜；_struct {
                    카에ic_ long_ t data;
         #define 暇）RK STRUCT PENDING 0                ／士 I if wo가； i tem 口ending execution 火／
         #define WORK STRUCT STATIC 1                  /* static initial izer (debugobjects) 六1
         #def 1 ne WORK_STRUCT_FLAG_MASK (3UL)
         #def i ne WORK_STRUCT_WQ_DATA_MASK (내 tRK_STR내計F녀6_MASK)
                    struct l ist_head entry;
                    work func t func;
         #i fdef CONFIG_LOCKDEP
                    struct lockdep_map lockdep-, map;
         #endif
          };
         6.15.6 circ buf 구조체
         circ_buf 구조체는 디PC山de川flux/clrc buf.h＞에 다음과 같이 정의되어 있다．


              /／大

               * See Documental ion/ cl rcular-buf far s ,txf for more information.
               士／
          #i I ndef _LINUX_CIRC_BUF_H
          #define LINUX 이吼BUF I-I ]

          struct circ_buf {


                                                                    225 / 312
          커 널 연구회（www.kernel.b기                                                       정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                                   6. UART 구조체     226




           char *buf ;
            nt head;            /／입력（producer) 위치 index
           mnt tai l ;          /／출력（consumer) 위치 index
 };
／火 버퍼에 입력된 아이템（데이터）의 개수 반환 t/
#define CIRC_CNT(head, tai l , size) ( ( (head) - (tai l) ) & ( (size) -1) )

／火 버퍼에서 사용 가능한 크기（o . 引ze너） 반환． head == tai i 이면 버퍼가 empty 상태이다． 火／
#detine CIRC_SPACE(head, tai l , size) CIRC_CNT( (tai l) ,( (head) +1) ,(size) )

It 버퍼에 입력된 아이템의 끝（end) 인덱스 반환 士／
#def i ne CIRC_CNT_TO_END(head, tai l ,size) W
           ({ int end = (size) - (tai l) ; *
              mnt n = ( (head) + end) & ( (size)-1) ; w
             n < end ? n : end; })

／士사용 가능한 버퍼크기 반환 士／
#def i ne CIRC_SPACE_TO_END(head, tai l , size) W
           ({ int end = (size) - 1 - (head) ; W
              i nt n = (end + (tai l) ) & ( (size) -1) ; w
             n <= end? n : end+1; })

#endif ／士 工小以CIRC BUF H 出／




6.15.7 baud rate 상수
시리얼 통신 속도 상수는 <arch/arm기nclude/asm八ermbits.h＞에 다음과 같이 정의되어 있다．


／火 c_cf lag bit mean나｝0 出／
#detine CBAUD      0010017
#define B0         0000000               ／火 hang up 士／
#define B50        0000001
#detine B75        0000002
#define B110       0000003
#define B134       0000004
#define B150       0000005
#def i ne B200     0000006
#define B300       0000007
#defmne B600       0000010
#define B1200      0000011
#define B1800      0000012
#define B2400      0000013
#define B4800      0000014
#define B9600      0000015
#define B19200 0000016
#define B38400 0000017
#define EXTA B19200
#define EXTB B38400
#define CSIZE      0000060
#define    C85     0000000

                                                     226 / 312
커 널 연구회佃ww.kern이. b기                                                           정재춘 （띠너3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                         6. UART 구조체    227




#def 나｝e  CS6     0000020
#define   CS7     0000040
#define   CS8     0000060
#detine CSTOPB    0000100
#define CREAD     0000200
#define PARENB    0000400
#detine PARODD    0001000
#detine HUPCL     0002000
#define CLOCAL    0004000
#define CBAUDEX 0010000
#define    BOTHER 0010000
#detine    B57600 0010001
#define B115200 0010002
#define B230400 0010003
#define B460800 0010004
#define B500000 0010005
#define B576000 0010006
#define B921600 0010007
#detine 81000000 0010010
#defino B1152000 0010011
#define 81500000 0010012
#det ine 82000000 0010013
#define B2500000 0010014
#define 83000000 0010015
#define B3500000 0010016
#define B4000000 0010017
#dofine CIBAUD       002003600000      !밖 input baud rate 士/
#detine CMSPAR     010000000000        /火 mark or space (stick) par ity 士1
#define CRTSCTS      020000000000      /* flow control *1




                                        227 / 312
커널연구회佃ww.kernel.b기                                                정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                    7. UART 드라이버 등록        228




7. UART 드라이버 등록




                                                   + 필자의 주말농장0私I 찍은 딸기




UART 디바이스드라이버가 커널에 등록되는 소스 코드는 drivers/tty/serial/8250/82 50_core.c 소스
파일의 seria18250_init() 함수에 있다． 이 함수에서 uart_register_driver() 함수를 호출하여 UART
디바이스드라이버가 커널에 등록된다．




                                       228 I 312
커널연구회佃w比kerr刈b기                                       정재준 (r아키3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                                      7. UART 드라이버 등록       229




hART 드라이버 둥록 支룝
                 8250 core.c                                                 serial core.c                    tty_io.c



      「，   ＼   「二，              』：【，   y0         「＞   \
                                                           \

           ser       ia18250_               ini
                                                       K        \,\
                                                                늬
                                                           \\
                                                                          uarLregister_ dr ver

                                                                                                      \
                                                                                                 \\
                                                                      1
                                                                                                          I t乙re미 없아 dr 1 ver

     「alform_d毗而11
뇨＝
Device 가ee 상세분석 in 니flux Kernel 4.0                                                7. UART 드라이버 등록   230




                    . suspend               = seria18250_suspend,

                    . resume                = ser1a18250_resume,

                    . driver                = {

                                   . name   = "seria18250 " ,

                    },
          };


          stat ic mnt _ini t seria18250 in1t (void)
          {
                         nt ret;

                    月포트 초기（이dser al port) 정보 설정
                    ser ia18250_ isa_ ini t_ports() ;

                    pr intk (KERN_ INFO 'Serial : 8250/16550 driver,
                               喘d ports , 나tO shar ing 弦sab led姆n " , nr_uar ts,
                               share_ i rqs ? 'en ' : "d! SD ;

          了ti tdet CONE田 SPARC
                     ret = sunserial_register_minors(&serial8250jeg, UART_NR) ;
          #els（크
                     serial8250_reg.nr = UART_NR;
                     ret = uart_register_dr iver (&ser ial8250_reg) ; If! 三라이버 듕록
          #endi i
                      f (ret)
                              goto out;

                    刃CONE I GSER I AL_8250_마叩가 섣정되어 있뇬 강우 pnpjegister_dr iver (）을
          싣행 한다 .
                    ret = ser1a18250pnp_ ini t () ;
                    it (ret)
                             goto unreg_uarLdrv;

                   月이atf아叱d田ce을 메모리 할당한다．
                   ser ia18250_ isa_devs = platform_device_al loc( "ser1a18250 ' ,
          PLAT8250_DEV_LEGACY) ;
                    f ( lser1a18250_ isa_devs) {
                             ret = -ENOMEM;
                             goto unreg_pnp;
                    }
                    //plat formd아ice에 추가한다；
                    ret = plattorm_device_add(seriaI8250jsa_devs) ;
                    it (ret)
                              goto put_dev;

                   ／江1리얼 포트를 등록한다 .
                   seriaI8250_register_ports(&serial8250_reg, &seriaI8250그sadevs->dev) ;

                    사퓰랫폼 드라이버로 등록한다
                    ret = plattorm_driver_register (&seriaI8250_ isa_dr iver) ;
Device Tree 상세분석 in Linux Kernel 4.0                                           7. UART 드라이버 등록     231




                      it (ret   ==   0)
                                 goto out;

                     plattorm_dovice_del (ser ia18250_ isa_devs) ;
          put_dev:
                   platform_device_put (ser ia18250_ isa_devs) ;
          unreg_pn口:
                   ser I 키明50_pnp_태 1 t ( ) ;
          unreg_uart_drv:
          #ifdef CONFIG SPARC
                   sunserial_unregister_minors(&seria18250_ reg, UART_NR) ;
          #else
                   uart_unregister_dr iver (&ser1a18250_reg) ;
          #endif
          out:
                   return ret;
          }




7.2 uartjegister_driver()

함수원형       1nt uartmregister driver (struct uart driver *drv)
          ua나 드라이 비 등록
  설명
매I H변수    struct uart dr iver *drv

소스파일      drivers/ tty/ ser ial/ ser ial_core. c

 구조체      struct tty dr iver *flormal ;

              nt uart_register_driver (struct uart_driver *drv)
          {
                      struct tty_driver *normal ;
                       nt I , retval ;

                      BUG_ON(drv->stale) ;

                      ／女
                       火 Maybe 艸e should be us汗｝g a 읽ab cache 化r this. es口eCi a I 卜｝/ if
                       出 we have a IE玎ge number of 口orts to handI느
                       士/

                      drv->state = kzal loc(sizeot (struct uart_state) * drv->nr , SEP_KERNEL) ;
                      i t ( !drv->state)
                                 goto out;

                      normal = al loc_ tty_dr iver (drv->nr) ;
                      i t ( normal )
                                goto out_ktree;

                      drv->tty_dr iver = normal ;
Device Tree 상세분석 in Linux Kernel 4.0                                        7. UART 드라이버 등록         232




                   noro비 今driver_name            = drv->driver name;
                   normal->name                  = drv->dev name;
                   nor ma1 ->ma j or             = drv->major ;
                   normal->minor start           = drv->minor;
                   normal->type                  = TTY DRIVER TYPE SERIAL;
                   normal->subtype               = SERIAL_TYPE_NORMAL;
                   normal->init_termios          = tty_std_termios;
                   normal->init_termios ,c_cf lag = B9600 I CS8 I CREAD I 내JPCL I CLOCAL;
                   normal->init termios. c_ ispeed = normal->init_ termios. c_ospeed = 9600;
                   normal->f lags                = TTY_DR I태_R태L_RAW I TTY_DR I VER_DYNAMI C_DEV;
                   normal->dr iver_state     == （打v;
                   tty_set巾operations(normal , &uart_ops) ;

                    /

                    出 UART state（引 초기화
                    六 /

                   for ( i = 0; i < drv->nr; j++) {
                             struct uart_state *s(ate = 먀v->state + i ;
                             struct tty夕ort *port = &state->port ;

                               tty_port_ ini t (port) ;
                               port->ops = &uart中port_0ps;
                   }
                   retval = tty_register_dr iver (normal) ;
                   if (retval >= 0)
                            return retval ;

                   for (i = 0; i < drv->nr; i++)
                             tty_port_destroy(&drv->state[ i I .port) ;
                   put_tty_dr iver (normal)
          out kfree:
                   kfree(drv->state) ;
          out:
                   return -ENOMEM;
           }




7.3 tty_register_drivero

함수원형       m t tty小re9ister_driver (struct tty_dr iver *dr iver)

  설명       t ty 드라이버 등록

매개변수       struct tty_driver *drjver

소스파일      drivers/ ttyltty_ io.c

 구조체1      struct tty_driver *driver

  소스       int tty_register_driver (struct tty_driver *driver)
           {
                    i nt error ',

                                              232 I 312
커 널 연구회（ww比kerne나）z)                                                      정재臣 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kerr佃 4.0                                            7. UART 드라이버 등록        233




                    nt 1 ;
                   dev t dev;
                   struct device 出d;

                   if ( !driver->major) {
                             error = al loc_chrdev_region(&dev, driver->minor_start,
                                                                    dr iver->num, dr iver->narne) ;
                             나 ( ! error) {
                                       driver->rnajor = MAJOR(dev) ;
                                       driver->minor_start = MINOR(dev) ;
                             }
                   } 이se {
                             dev = MKDEV(driver->major, driver->minor_start) ;
                             error = register_chrdev_region(dev, driver->num, driver->name) ;
                   }
                   if (error < 0)
                            goto err;

                   if (driver->f lags & TTY_DRIVER_DYNAMIC_ALLOC) {
                            error = tty_cdev_add(driver, dev, 0, driver->nurn) ;
                            if (error)
                                      gob err_unreg_char;
                   }
                   mutex_Iock(& tty_mutex) ;
                   I ist_add(&driver->tty_drivers, &tty_drivers) ;
                   mutex_unlock(& tty_mutex) ;

                   if ( !(driver->f lags & TTY_DRIVER_DYNAMIC_DEV) ) {
                             for ( i = 0; i < driver->num; i++) {
                                       d = tty_register_device(driver, i , NULL) ;
                                       if ( IS_ERR(d) ) {
                                                 error = PTR_ERR(d) ;
                                                 gob err_unreg_devs;
                                        }
                             }
                   }
                   proc_ tty_register_dr iver (dr iver) ;
                   dr iver->t lags 1= TTY_DRIVER_ INSTALLED;
                   return 0;

          er r_unreg_devs:
                    for ( i--; I >= 0; i--)
                              t bUnr明田te口由vice(dr iver,        j)   ;

                   mutex_ lock(& tt止mutex) ;
                   I ist_del (&dr iver->tty_dr ivers) ;
                   mutex_unlock(& tty_mutex) ;

          er r_unreg_char:
                    unregister_chrdev region(dev, di iver->num) ;
          err:
                    return error;
          }
          EXP0RT_SYMB0L(tty_re引ster+dr iver) ;


                                               233 I 312
커널연구회佃w比蛇rnel.b기                                                           정재준 (rgbi3307@nate.con升
Device Tree 상세분석 in 니flux Kernel 4.0                 7. UART 드라이버 등록          234




                                       234 / 312
커널연구회（www.kern飢b기                                  정재준 (rgb13307@nate.corT升
Device Tree 상세분석 in 니flux Kernel 4.0                                    8. UART 포트 등록       235




8. UART 포트 등록




                                                              + 필쟈의 주말농장0和1 찍은 나팔꽃




UART 포트의 개수는 drivers/tty/serial/8250/8250_core.c 소스 파일에서 다음과 같은 전역변수로
정의되어 있다．


#def ine UART NR   C0NFIG SERIAL 8250 NR UARTS
static unsigned nt nr_uarts = C0NFIG_SERIAL_8250_RUNTIME_UARTS;


위에서 CONF IC; 상수들은 커널이 환경설정（.confi이될따1 정의 된다．


UART 포트들은 seria18250_register寸ports() 함수에서 nr uarts에 설정된 개수 만큼 루프를 돌면서
uart_ad&oneport() 함수를 호출하여 등록된다．                        이때 전달되는 구조체들의 연결관계를 Flow
미agram으로 정리하면，




          uart 8250 porl
           er n키 8250 pcir t하 UART. .NR]




                                                 235 I 312
커 널 연구회（www.kern이b기                                               정재준 (rgbi3307@nate.com)
Device Tree 상세분석 ir) 니flux Kernel 4.0                                                         8. (JART 포트 등록       236




UART 포트 둥록 흐룝
           8250 core.c                                     serial core. c                       ttyio.c


            uart dr iver
                        '

                              /\,,,
         ser ia18250 1 ni t




             1戶卜
                                                 \\\
                                                       oar t_addone.por t


                                                                       \
   serial8250_register ports                                                  \
      /，낀r／ 恥                               毛，

                                                                Ir
                                                                                   '   tty_ regist: r_device
                                                                                                               1
          戶                           甘노寸
                                                       uarLconf igure port



    IV

   ser ia18250jsajnit_ports




8.1 seria18250_register_ports()
ser1a18250_register_ports() 함수는 drivers/t勺/serial/8250/8250_core.c 파일에 다음과 같이 정의되어
있다．


함수원형          static void   nit
              seria田250- reaisterports(struct uart_driver *drv, struct device *dev)

  설명          oar t 포트 등록

매개변수          dry: uart driver 구조체 포인니
              dev: device 구조체 포인터
소스파일          dr ivers/ tty/ ser ial /8250/ 8250_core. c

 구조채          struct uart driver
              struct device
              struct uart8250port


  소스          static void   mnit
              seria18250jegis1er_ports(struct uart_driver *drv, struct device *dev)
               {
                            mnt i ;

                            for ( i = 0; i < nr_uarts; i++) {
                                      struct uart_8250_port *up = &ser ia18250_ports[ i ] ;                    1

                                                            236 / 312
커 널 연구회（www.kern이.b기                                                              정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                 8. UART 포트 등록          237




                              up->qur_ iotype = OxFF;
                    }
                    ser ia18250_ is乞init_portsO;                                                        2

                    for ( i = 0; i < nr_uarts; i i-+) {
                              struct uart_8250_ 兀rt *up = &seria18250j. orts[ i] ;

                              up->port. dev = dev;                                                 -3
                                 if (up->port. flags & UPF_FIXED_TYPE)
                                         ser1a18250_init_fixed_ type_port (up, up->port. type) ;        4

                              .카t_add_。n.巾.:t                   p아t)   ·，                               5
                    }
                                                          ＆叩，
                                                  (drv,
           }




8.2 ua八madd끄ne下아to)
uart_add_one_port() 함수는 d rivers/tty/seria 1/seria l_core.c 소스 파일에 다음과 같이 정의되어 있다．



함수원형       mnt uart코叱neJ）아t (:struct uart_driver *drv, struct uartmport *uport)


           uar t 포트 구조체 등록
  설명

매개변수      （打v: uart driver 구조체 포인 터
          uport: uar Lport 구조체 포인 터
소스파일      driverslserial/ serial_core.c

 구조체       struct uart_dr iver
           struct uarLport
           struct uart state
           struct ttyport
           struct device

           mnt uart_add_one_port (struct uart_driver *drv , struct uart- port *uport)
           {
                    struct uart state *5tate ;
                    struct ttyport *p0rt ;
                    1 nt ret = 0;
                    struct device *ttydev;

                    BUG_ON( in그 nterru야 ( ) ) ;

                    it (uport->I ine >= drv->nr)
                             return -EINVAL;

                    state = drv->state + uport->I mne;
                    port = &state->port;
Device Tree 상세분석 in 니flux Kernel 4.0                                            8. UART 포트 등록    238




                  mutex_ lock(&port_mutex) ;
                  mutex_ lock(&port->mutex) ;
                  it (state->uart_port) {
                            ret = -EINVAL;
                            goto out;
                  }
                  state->uart_port = uport;
                  state->pm_state = -1 ;

                  uport->cons = drv->cons;
                  uport->state = state;

                  ／士
                        士 이 포트가 콘솔 이라면 , spinlock은 이미 초2陣H日어 있다．
                        火/
                  it (! (uart_coflsole(uport) && (uport->cons->f lags & CON_ENABLED) )) {
                            spin_lock_init (&uport->Iock) ;
                            lockdep_set_class(&uport->lock, &port_ lock_key) ;
                  }
                  uart_ 兀nfigure_port (drv, state, uport) ;

                  ／出
                        火 포트 존재（검출） 여부에 상관없이 포트를 등록한다，
                        出／
                  tty_dev = tty_register_device(drv->tty_driver , uport->I ine, uport->dev) ;
                  if ( I ikelyUIS_ERR(tty_dev) )) {
                             device_init_wakeup(tty_dev, 1) ;
                             dev比已朗L肥keup_ena이e(tty_由v, 0) ;
                  } 이se
                             printk(KERN_ERR 'Cannot register tty device on l ine %dWn",
                                    uport->l i ne) ;

                   1*
                        士 UPF_DEAD가 설정되지 않도록 확실히 함．
                        士/


                  uport->f lags &= -UPF_DEAD;

           out:
                  mutex_unlock(&port->mutex) :
                  mutex_unlock(&port_mutex) ;

                  return ret;
          }




                                             238 / 312
커 널 연구회（www.kernei.bz)                                                 정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Ker et 4.0                                                   8. UART 포트 등록   239




8.3 seria18250_isajnit_ports()
이 함수는 UART 포트별로 정보를 초기화 한다．



함수원형      static void 叫 nit ser1a18250_ isa_iniLports(void)


 설명       uar t 포트별로 정보 조기 화

매개변수

소스파일      dr ivers/ ser iaI18250. c

구조체       struct uart_8250_port

          static void _init 5eria18250_isa_iniLports(void)
          {
                    struct uart_825Qj均rt 火U口；
                    stat ic mnt first = 1:
                    m } t i , irqf lag = 0;

                    if ( ! first)
                               return;
                    first = 0;

                    for ( i = 0', i 卞 nr_uarts; i-i-+) {
                              struct uarL8250_port *ijp = &seriala25o巾orts[ iJ;
                                      1
                              up->pdrt. l ine = i·，




                              spin_ ockJni t (&up->port . lock) ;

                              mni Lt imer (&up->t imer) ;
                              up->ti1mer. function = seria18250 timeout;

                              r*
                               玄 ALPI-lAKLUDG드 柚CR needs to be ki t 沌d.

                              up->nsr_mask = -ALPHAj(LUDGE_MCR;
                              U口게하J아ce = ALPHA_KLUDGE MCR;

                              up->port ,ops = &seriat825Q)ops;
                   }
                   if (share그rq引
                            irqflab = IRQF_SHARED;

                   for ( i = 0, up 卜 seria18250_ports;
                         i < ARRAY_SIZE(old_serial_port) && I < nr_uarts;
                         i++, up++) {
                             up->port. iobase =old_seriaLport[ i ] .port;
                             U口＞1兀 ' t . 汀p      = ira 'canonical ize(old_serial巾아t [ 1 ] ' i rq) ;
                             up->po 't. irqflags = old_seriaLport[ i j. irqf lags;
                             up->po t.uartclk = old_seria냐ort[ i ] .baud_base * 16;
                             up->po "t. flags    =old_seriaLporf[ i j. flags;
                             up->port.hub6       = old_seria匕port[ i] .hub6;
                                                                         8. UART 포트 등록
Device Tree 상세분석 In 니flux Kernel 4.0




                          U口＞r兀it . rnembase = 이d ser ia匕口ort[ ] . iomeni base;
                          up->port. iotype   = olcLseriaLport[ i ] Ho_ type;
                          U口＞port. regsh나 t = 이dj아 治냐刈t[ i l. iomeni_reqsh냐t;
                          setjo_ from_upio(&up->port) ;
                          up->port. 나qflags 1= 1 rqf1ag;
                   }
           }




                                           240 / 312
  커널연구회（www.kern이. b기                                               정쟤준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                              9. UART 8250 드라이버 동작     241




9. UART 8250 드라이버 동작




                                                              + 필자약 주말농장에서 찍은 봉숭아꽃




UART 디바이스드라이버의 동작은 플랫폼 드라이버로 등록되어 수행된다.                                UART 풀랫폼 드라이버
구조체는 drivers/tty/serial/82 50/8250_core.c 소스 파일에 다음과 같이 정의되어 있다．


static struct platform_driver se1 ia18250_ isa_dr iver = {
         . probe           = ser ia18250_probe,
         . remove          = seria18250_remove,
         . suspend         = seria18250_suspend,
         . resume          = ser1a18250_resume,
          .   driver           =   {
                       .name   = Hser1a18250" ,

};
         },
.probe에는 UART 드라이버가 처음으로 인식되어 실행되는 함수（seria治250_probe ）가 연결된다．
.remove（걔는 UART 드라이버가 제거될 때 실행되는 함수（sen키8250_remove）가 연결된다．
.suspend에는 UART 드라이버 동작을 잠시 멈출 때 실행되는 함수（sen키8250_suspend）가 연결된다．
.resum可게는 UART 드라어버 동작이 재개될 때 실행되는 함수（sen調250_resum이가 연결된다．




                                                  241 / 312
커 널 연구회（ww比kern飢b기                                                 정재준 內bi3307@nate.com)
                                                                        9. UART 8250 드라이버 동작   242
Device Tree 상세분석 in Linux Kernel 4.0




                                                              드라이버로
위의 구조체는 히計幻rm먀如아_register() 함수에 매개변수로 전달되어 커널에 플랫폼
                                                                같이 정
등록된다. 히at化rm먀如아_register() 함수는 drivers/base/p怡卄orm.c 소스 파일에 다음과
의되어 있다．


mnt 1이at form펴liv아re이ster (struct r니at for町driver 大dry,
                                struct modu陀 火0州ner)
{
         drv->driver. owner = owner;
         drv->dr iver. bus = 匈기atform_bus_ type;
         if (drv->probe)
                   drv->dr iver .probe = platform_dry_probe;
          if (drv->remove)
                   drv->dr i ver . remove = platform_dry_ remove;
          if (drv->shutdown)
                   먀中刈river .shutdown = 이atfor旺먀v帥utd1：           川n;

          return dr iver_register (&drv->dr iver) ;
 }
EXPORT_SYMBO나叩L(1이카 form_dr iver_register) ;



                                                           등록된
 위의 함수 매개변수에 seria18250_isa_driver 구조체가 전달되어 커널의 플랫폼 드라이버로
                                                           " 책의
 다. 플랫폼 드라이버에 대해서는 필자가 집필한 " 리눅스 커널과 디바이스드라이버 실습2
    ]］장 8절에 설명되어 있으니 참고하기 바란다．




                                                      242 / 312
     커널연구회（www.kern텨.b기                                                   정재준 仕9b13307（孕nate.com」
Device Tree 상세분석 in 니flux Kernel 4.0                                          9. UART 8250 드라이버 동작             243




9.1 seria18250_probeo
seria田250_probe() 함수는 drivers/tty/serial/82 50/8250_core.c（게 정의되어 있다.                        이 함수는 UART
드라이버가 커 널에 인식될 때 실행된다.                              이 함수에는 사용자가 설정한 UART 포트 정보가
히at化rm device 구조체에 전달되어 uart_port 구조체에 저장된다．                                    uart_port 구조체에 저장된
UART 포트 정보는 seria18250_register_port() 함수를 통하여 커널에 등록된다.                                    아래는 이 과정을
Flow 미agram으로 정리한 것이다．



probe() 함수에서 UART 포트정보 저장
             8250 core.c                                 serial core.c                      ttyjo.c



  /1뇨將少／;                                  （二＝
                                /                                               小
                                                  uar t_add_one_por t
     ser ia18250_probe                     /
                                          7
         「       :   250 port                                 ,     \                     蜘村呻小

                                                  uart_conf igure_port   \\    \\
                                                                                    tty_register_device_attr




                                                                                              ;1
  ser 1a18250_register_8250_port




                                                                                       device_register




seria18250_probe() 함수의 소스는 drivers/tty店en키／8250/8250卞core.c에 다음과 같이 정의되어 있다．


함수원형         static 1 nt seria18250_ 玎obe(struct platform_device *dev)

  설명         플랫폼 장치에 시리얼 장치를 등록한다．

매개변수         dev: 이atfor町由v I CO 구조체 포인터

소스파일         di ivers! tty/ ser ial/ 825018250_core. c

 구조체         struct platform_device
             struct plat_seria18250_port
             struct uart_port


  소스         stat ic mnt seria18250_probe(struct platform_device *dev)
             {

                                                    243 / 312
커 널 연구회（ww比kern이.b기                                                            정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                    9. UART 8250 드라이버 동작        244




                     struct plat_seria18250_port *p = dev_get_platdata(&dev->dev) ;
                     struct uart 8250_port uart;
                     1nt ret, i , irqf lag = 0;

                     mernset (&uar t , 0 , 引zeof佃카t) ) ;

                      i f (share_ irqs)
                                irqf lag = 1 ROE SHARED;

                     for ( I = 0; p && p->f lags != 0; p++, i++) {
                               uart.port. iobase                    = 口키obase;
                               uar t .por t . membase               = p->membase;
                               uart.port. irq                       = p->irq;
                               uart.port. i rqf lags                = p->irqf lags'
                               uart .por t .uar tc 나                = p->uartclk;
                               uart.port. regshi ft                 = p->regshi ft;
                               uart.port. iotype                    = 寸기야ype;
                               uart.port. f lags                    = r느＞flags;
                               uar t . pert .mapbase                = p->mapbase;
                               uart.port.hub6                       = r느＞hub6;
                               uar t .por t . pr ivate_data         = p->pr ivate_data;
                               uart.port. type                      = 寸＞type;
                               uart.port. serial_ in                = p->serial_ in;
                               uar t .por t . ser i al_out          = 口＞ser 1 a匕out ;
                               uart.port.handle_ irq                = p->handle_ irq;
                               uart.port.haridle_break              = 寸＞hand陀 뱌eak;
                               uar t . p01 t . set_ term i Os       = p->set_ term105;
                               uar t .por t . pm                    = r느＞口rn
                               uar t . port. dev                    = &dev->dev;
                               uart .port. irqf lags                1= irqf lag;
                               ret = seria18250_register_8250_port (&uart) ;
                               i f (ret < 0) {
                                     dev_err (&dev->dev, 'unable to register port at index %d '
                                                         ' ( t0%lx MEM% i ix IRQ%d) : %dWn " , ,
                                                        寸키的ase, (unsigned long long)p->rna口base,
                                                        口늬 rq, ret) ;
                                 }
                     }
                     return 0;
            }



seria18250_register小8250_port 함수는 drivers/tty/serial/8250/8250_core.c（게 다음과 같이 정의되어
있다．


mnt ser ia18250_register_8250_port (struct uart_8250_port *up)
{
         struct uart_8250_port *uart;
         mnt ret = -ENOSPC;

          f (up->port. uartc나； == 0)
                  return -EINVAL;


                                                244 / 312
커 널 연구회佃iww.kern이. b기                                                     정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                   9. UART 8250 드라이버 동작         245




       mutex_ lock(&ser ial_mutex) ;

       uar t = ser i키明50_f ind_matc九아_unused(&u口叩ort) ;
       if (uart && uart->port. type 1= PORT_8250_CIR) {
                 if (uart->port.dev)
                          uart_remove_one_port (&ser ia18250卞reg, &uart->port) ;

                 uart->port. i obase      = up->port. 泊base;
                 uar t->por t .membase    = up->por t .rnembase;
                 uart->port. irq          = 바느＞口ort . i rq;
                 uart->port. irqf lags    = 바느＞port . i rqf lags;
                 uart->port . uar tclk    = U口H＞口ort.uartc나G
                 uart->port. f ifosize    = up->port. fifosize;
                 uart->port. regshif!     = up->port. regshitt;
                 uart->port. iotype       = 바느＞port . i otype ;
                 uart->port . flags       = up->port. f lags I UPF_BOOT_AUTOCONF;
                 uar t->bugs                 = 바느＞b四5;
                 uar t->por t .mapbase    = 바느叩or t . mapbase;
                 uart->port.pr ivate_data = up->口ort.pr ivate나data;
                 uart->port. fifosize        = up->port. fifosize;
                 uart->tx_ loadsz            = up->tx_ loadsz;
                 uart->capabi l ities        = up->capabi l ities;
                 uart->port. thrott le       = up->port. throttle;
                 uart->port.unthrottle       = up->port.unthrottle;
                 uart->port. rs485_config    = up->port. rs485_config;
                 uart->port. rs485 = up->port. rs485;

                 1* Take tx_ Ioadsz from fifosize if it wasn' t set separately *j
                 if (uart->port. fifpsize && !uart->tx_ loadsz)
                          uart_>tx_ loadsz = uart->port. fitosize;

                 if (up->port.dev)
                         uart->port.dev = up->port.dev;

                 if (up->port. f lags & UPF_FIXED_TYPE)
                         seria18250_init_fixed_ type_port (uart, up->port. type) ;

                 set_ io_from_upio(&uart->口Ort) ;
                 』／六Poss吐）ly overr 油e default I/ O functions. 女／
                 if (up->port. serial_ in)
                           uart->port. serial_ in = up->port.serial_ in;
                    (up->port. ser ial_out)
                           uart->port. serial_out = up->port. serial_out;
                 if (up->port.handle_ i rq)
                           uart->port.handle_ irq = up->port.handle_ irq;
                 ／士 Possibly overr ide set_ terrnios cal l 玄 /
                 if (up->port. set_ termios)
                           uart->port. set_termios = up->port. set_ termios;
                    (up->port. set_mctrl)
                           uart->port. set_mctrl = up->port. set_mctrl ;
                    (up->port. startup)
                           uart->port. startup = 바느＞port. star tu口;
                    (up->port . shutdown)
                           uart->port.shutdown = up->port. shutdown;
                    (up->port.pm)
                                       F      245 / 312
커널연구회 佃w比蛇me比z)                                                           정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                       9. UART 8250 드라이버 동작       246




                              uart->port.pm = up->port.pm;
                     if (up->port. handle_break)
                              uart->port.handle_break = up->port.handle_break;
                     it （바卜＞d匕read)
                              uar t->d匕read = 바느＞di_read;
                     if (up->d匕write)
                              uar t->d匕나rite = up->dl 너rite;
                     if (up->dma) {
                              uart->dma = up->dma;
                              if ( 山ar t->dma寸＞tx_dma)
                                        uart->dma->tx_dma = ser ia18250_ tx_dma;
                              if (!uart->dma->rx_dma)
                                        uart->dma->rx dma = seria18250 rx dma;
                     }
                     냐 (ser 治出250_is之conf ig != NULL)
                             seria18250_ isa나config(0, &uart->port,
                                               &uart->capabi l it ies) ;

                     ret = uart_add_one_port (&seria18250_reg, &uart->port) ;
                     if (ret == 0)
                              ret = uart->port. l ine;
          }
          mutex_unlock(&ser ial_mutex) ;

          re山rn ret ;
}
EXPORT SYMBOL( ser i al 8250_reQ i ster_8250_por t) ;




uart_add_one_port() 함수는 drivers/t勺／serial/serial_core.c에 다음과 같이 정의되어 있다．


mnt uart_add_one_port (struct uart_driver *drv , struct uart_port *uport)
{
          struct uart_state *5tate;
          struct tty_port *p0rt ;
          mlt ret = 0;
          struct device *ttydev;
          mnt num_9roups;

          BUG0N( in_ interruptO) ;

          if (uport->l ine >= drv->nr)
                   return -EINVAL;

          state = drv->state + uport->l ine;
          port = &state->port;

          mutex_ lock(&p아 L叩tex) ;
          mutex그 ock(&p아卜>mutex) ;
          if (state->uart_port) {
                    ret = -EINVAL;
                    goto out;
          }
                                                        246 / 312
커 널 연구회（www.kernei.b기                                                       정재준 (rgb日307@riate.com)
Device 가ee 상세분석 In 니flux Kernel 4.0                                               9. UART 8250 드라이버 동작        247




        ／古 니flK tfl@ r均it to the diver state tab沌 and vice versa 士／
        state->uart_port = uport ;
        uport->state = state;

        state->pm_state = UART_PM_STATE_UNIDEF INED,
        uport->cons = drv->cons;

        ／肯
                  * It this port is a console, then the spinlock is already
                  * initial ised.
                  出／
        it ( ! (uart_console(uport) && (uport->cons->f lags & cON_ENABLED) )) {
                   spin_Iock_init (&uport->Iock) ;
                   Iockdep_set_class(&uport->Iock, &口0rt_Iock_key) ;

                            (uport->cons && uport->dev)
                                  of_cons이乞check（叩ort->dev＋야小ode, uport->cons寸＞name, u口ort->l mne) ;

        uart_configure_port (drv, state, uport) ;

        num_groups = 2;
        if (uport->attr_group)
                 num_groups++;

        uport->tty_groups = kcal loc(num_grou口S , 引ze아（士up아卜놔b띠roups) ,
                                        GEP_KERNEL) ;
        if ( luport->tty_groups) {
                 ret = -ENOMEM;
                 goto out;
        }
        uport->tty_groups[ O] = &t ty_dev_attr_group;
        if (uport->attr_group)
                 upor卜놔口띠roups[ 1 I = uport小＞attr尸grou口；

             ／士
                   * Register the port whether its detected or not. This al lows
                   * setserial to be used to alter this port 's parameters.
                       士／
         tty_dev = tty_port_register中device_attr (port, drv->tty_driver,
                               uport->l ine, uport->dev, port, uport->tty卞groups) ;
         if ( l ikelyUlS_ERR(tty_dev) )) {
                    dev i ce_set_wakeup_capab I e( t ty_dev, 1) ;
         } 이se {
                    dev_err (uport->dev 「 Cannot register tty device on l ine %dWn ' ,
                             uport->l mne) ;
         }
             ／六
                       卞 Ensure UPF DEAD is n아 S小：
                       士/
        uport->t lags &= -UPE_DEAD;

 out:
        mutex_unlock(&port->mutex) ;
        mutex_unlock(&口ort_mutex) ;

                                                            247 / 312
커 널 연구회（
       ＼사낚／＼六／
             k아n이.bz)                                                               정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니nux Kernel 4.0                                                   9. UART 8250 드라이버 동작            248




             return ret ;
}




9.2 seriaI8250msuspend()
UART 드라이버의 포트 동작을 잠시 멈출 때 seria18250_suspend() 함수가 호출된다.                                                      이 함수의
동작 과정을 Flow D治gram으로 정리하면，



suspend 동작 흐룝
                 8250 core.c                                                  seriaf core.c




                                                                              日
     』蜘雉煎娩口m.           ,.   小吼宓泣出極再




             ，十                                        uar t_suspend_por t
                                                   戶
             V                             /   7
        se r i a 18250_suspend         7                                 \\
    1= ，心r   느挺 尸nf 小 됴斗n小小

                                                       uar t_change_pm                        uart shutdown

             小了 八놔1n ＝二小二dm 느 nr二小




seria18250_suspend() 함수의 소스는 drivers/tty/serial/8250/8250_core（에 다음과 같이 정의되어
있다．
함수원형               static     nt ser1a18250_suspend(struct platform_device *dev, pm_message_ t
                   state)


     설명            UART 포트 농작을 멈춤

매개변수               dev: platform_device 구조체 포인터
                   state: pm_message 구조체
소스파일               dr ivers/ tty/ ser ial/8250/ 8250_core. c

    구조체            struct platform_device
                   struct uart_8250_port

     소스            static i nt ser1a18250_suspend(struct platform_device *dev, pru_message_ t state)
                   {
                              nt L

                                                             248 / 312
커 널 연구회（帥／w.kernel.b기                                                                   정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                            9. UART 8250 드라이버 동작            249




                          for ( i = 0; 1 < UART_NR; j++) {
                                    struct uart_8250_port *up = &ser ia18250_ports[ i j;

                                        i f (up->port. type 1= PORT_UNKNOWN && up->port. dev == &dev->dev)
                                                 uart_suspend_port (&ser ia18250_reg, &up->port) ;
                          }
                          r （놔 urn 0;
                 }


uart_suspend_port() 함수는 drivers/tty/seri키八erial_core.c에 다음과 같이 정의되어 있다.                                  소스 코

드의 흐름을 따라가 보면



uport->suspended = 1;



uart_port 구조체의 멤버변수인 suspended를 ］로 설정하여 동작 멈춤을 제어함을 알 수 있다．




    ft uart_suspend_port (struct uarf_dr iver *drv, struct uart_port *uport)
{
            struct uart_state *state = drv->stafe + uport->I mne;
            struct tty_port *port = &state->port;
            strucf device 女I tf乙dev ;
            struct uar f_match match = {uport, drv} ;

            mutex_ Iock(&p아卜加ulex) ;

            fty_dev = device_ f ind_chi ld(uport->dev, &match, ser ial_match_port) ;
            {1 (device_may_wakeup(tty_dev) ) {
                     it ( ! enable_ irq_wake(uport->i rq) )
                               叩or卜＞i rq_wake = ] ;
                     put_device( tty_dev ;
                     mutex_unlock (&port->mutex) ;
                     return 0;
            }
            put_dev I ce( tty_dev) ;

            了／火 Nothing to 口o f the conso沌 s not sus口end ng 士／'
              f ( ! console_suspend_enabled && uart_console(uport) )
                        goto unlock;

            uport->suspended = 1;

                f (port->flags & ASYNC INITIALIZED) {
                        const struct uart_ops 女야）S = 叩ort＞叩5,
                        1 nt tries;

                       set_bi t (ASYNCB_SUSPENDED, &por t->t lags) ;
                       clear_bi t (ASYNCB_ INlTlALlZED, &port->f lags) ;


                                                        249 / 312
커 널 연구회（www.kernel.b기                                                              정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                       9. UART 8250 드라이버 동작        250




                     叩 in_ lock_ i rq(&u口ort小＞lock) ;
                     ops->stop_ tx(uport) ;
                     ops->set_mctr l (uport, 0) ;
                     ops->stop_rx(uport) ;
                     spin_unlock_ irq(&uport->lock) ;



                      * Wai t for the transmitter to empty.
                      出/
                     for (tries = 3; !ops->txempty(uport) && tries; tries--)
                                 msleep(10) ;
                     if ( 1 tr ies)
                                 dev_err (uport->dev, %s%d: Unable to drain transmitterWn" ,
                                           dr v->dev_name,
                                           drv->tty_dr iver->name_base + uport->l mne) ;

                     ops->shutdown(uport) ;
         }
         /／士


             士 Disable the console device before suspending.
             t   /


         i f (uart_console(uport) )
                   console_stop(uport->cons) ;

         uar t_change_prn(state, UART_PM_STATEOFF) ;
unlock
         mutex_unlock(&port->mutex) ;

         return 0;
}




                                                  250 / 312
커널연구회佃ww.kern이b기                                                             정재준 (rgbi3307@nate.com)
Device Tree 상세분석 ir) 니flux Kerr倒 4.0                                                9. UART 8250 드라이버 동작       251




9.3 seria$8250_resume()
UART 드라이버의 포트 동작을 재개할때1 seria18250_resume() 함수가 호출된다.                                               이 함수의 동작
과정을 Flow ［기agram으로 정리하면，



resume 동작 흐푭
            8250 core.c                                                     serial core.c




                                                                                 느
     汁小小口     1 ‘口        「了J知涵再3＝」；/
                     =1 已呼"




                                                 uar t_resume_por t


                     V
                                             I
                                             /
       S（玎 1 키 8250 resume
                                                                      \\\


                     1
      ser i a 18250_resume_port         /
                                         /        uar t_change_speed                        uart_startup




seria田250_resume() 함수의 소스는 drivers/tty/serial/8250/8250_core.c（게 다음과 같이 정의되어 있
다．
 함수원형          static 1 nt ser1a18250_resume(struct platform_device *dev)


      설명       UART 포트 농작을 재개 .

 매개변수          dev: 이atform device 구조체 포인터


     소스파일      di 1 vers/ ser ial/8250. c

     구조체       struct platform_device
               struct uart_8250_port


      소스       stat ic    nt seria18250 reE;ume(struct plattorm_device *dev)
               {
                            mnt i ;

                           化r ( i = 0; 1 < UART_NR; i++) {
                                    struct uart_8250_port *jp = &seria18250_ports[ i ];

                                         f (up ->port. type 1= PORT_UNKNOWN && up->port . dev == &dev->dev)
                                                 seria18250_resume_port ( i ) ;
                            }



                                                        251 / 312
커 널 연구회（www.kernel.bz)                                                                정재준 什gbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                              9. UART 8250 드라이버 동작      252




                                     re山In 0 ;
                   }


ua八_resum已port() 함수의 소스는 driverslttylserial/serial_core.c（川 다음과 같이 정의되어 있다. 소
스 코드의 흐름을 따라가 보면



uport->sus口ended = 0;



uart_port 구조체의 멤버변수인 suspended를 0로 설정하여 동작 재개를 제어함을 알 수 있다．




    nf uart_resume_port (struct uart_dr iver *drv , struct uart port *uport)
{
            struct uart_state *state = drv->state + uport->I mne;
            struct tty_
                      port *兀rt = &state->port;
            struct device *ttydev;
            struct uart_niatch match = {uport, drv} ;
            struct ktermios terinios:

            mutex_ lock (&port->mutex) ;

            tty_dev = device_ f ind_chi Id(uport->dev, &match, serial_match_port) ;
            if ( 'uport->suspended && device_may_wakeup(tty_dev) ) {
                     if (uport＞나q네ake) {
                               disable_ irq_wake(uport->irq) ;
                               뱌）or卜＞I rq叫ake = 0;
                         }
                         put_device( tty_dev) ;
                         mutex_unlock(&port->niutex) ;
                         return 0;
            }
            put_device(tty_dev) ;
            uport나＞sus口ended = 0;

            ／大
                 tRe-enable the console device after suspendIng.

                 f (uart_console(uport) ) {
                         ／大


                              士 F 냐st try to use the conso陀 cf k크g setting.
                              士 1/


                         memset (& termios, 0, sizeof (struct ktermios) ) ;
                         termios. c_cf lag = uport->cons->cf lag;

                         ／士
                              大 If that 's unset, use the tty ternilos setting.

                         if (port->tty && termios. c_cf lag == 0)
                                  termios = port->tty->terfnios;



                                                         252 / 312
커 널 연구회（www.kern이. b기                                                              정재준 （呼)13307@nate.com)
Device Tree 상세분석 In 니nux Kerr伺 4.0                                          9. UART 8250 드라이버 동작        253




                1I (console_suspend_enabled)
                         uar t_changej)m( state, UART_PM_STATE_ON) ;
                uport->ops->set_ termios(uport, &terrnios, NULL) ;
                it (console_suspend_ena키ed)
                         console_star t (upor t->cons) ;
       }
       i t (por t->f lags & ASYNC_SUSPENDED) {
                  const struct uart_ 야）5 大ops = 叩ort-＞야）s;
                  m tt ret;

               uar t_change_prn( state, UART_PM_STATE_ON) ;
               印in_ I oc匕irq(&u叩r t->lock) ;
               ops->set_mctr l (uport, 0) ;
               spin_un lock_ irq似叩아卜키 ock) ;
               if (console_suspend_enabled 1 1 Iuart_console(uport) ) {
                         』／士Protected by port mutex 佃r now 士／
                         struct tt'y_struct *tty = port->tty;
                         ret = ops->startup(uport) ;
                         if (ret == 0) {
                                    if (tty)
                                              uart_change_speed( tty, state, NULL) ;
                                    sp I fl_加애Urq(&upor卜키 ock) ;
                                    ops->set_mctrl (uport, uport->rrictrl) ;
                                    ops->star t_tx( upor t) ;
                                    spin_unlock_i rq(&uport->lock) ;
                                    set_bit (ASYNCB_INITIALIZED, &口ort->f lags) ;
                         } 이se {
                                      ／士
                                           火 Pa i 陀d to resume   maybe hard빠are went a텍ay?
                                           * Clear the "initial ized" flag so we won 't try
                                           六 to cal l the low level drivers shutdown method.
                                           火 /

                                      Liar t_shutdown( I ty, state) ;
                            }
                   }
                   clear_bi I (ASYNCB_SUSPENDED, &port->f lags) ;
       }
       mutex_unlock(&port->mutex) ;

       return 0;
}




                                                    253 / 312
커 널 연구회（ww比k日ne나az)                                                           정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                              9. UART 8250 드라이버 동작                                254




9.4 인터럽트 동작
시리얼 8250 인터럽트 서비스 루틴은 8250 core.c 소스파일의 seria18250Jnterrupt() 함수이다.                                                               아
래는 이 함수가 동작되는 흐름을 다이어그램으로 그린 것이다．



UART 인터럽트 동작 흐룝
                                            drivers/tty/serial/8250/8250core.c


    /r        ,       fi fe
              .口．;，攝8七，       尸」J少才／   r           ／戶 ser ia182印小and le_r兀It               uart insert char

                                               /
                                                                        \/
                                                          //
                      '                    I
                                                                                  /7
         ser 키 叩50_ interru아               7
   小                                                receive chars
                                                                      人\                       port .state->x目｛it
                                                                                    喀辯無蜘韜聲鉀努
                                                                 transmit chars
                                                                                           L                                 m戶



                                                                                                                   尸耐J   "
                                                                                                  1            .




9.4.1 receive_chars()


함수원형              static void
                  receive.;chars(struct uart_8250_port *tjp, unsiQned i nt *status)

  설명              uart 레지스터로부터 문자를 수신함

매개변수              up: uart_8250口ort 구조체 포인터
                  status: 상태값


소스파일              di ivers/ ser ial/ 8250. c

 구조체              struct uart_8250_ 珣rt
                  struct tty_struct


  소스              stat ic void
                  receive chars(struct uart_8250_port *up, unsigned mnt *status)
                  {
                                 struct tty_struct *tty = up->port. state->port. tty;
                                 unsigned char ch, 1 sr = *status;
                                  nt max count = 256;
                                 char f lag;

                                 do {
                                           f ( I ikely( lsr & UART_LSRDR) )

                                                               254 / 312
커 널 연구회 佃／ww.kern이.bz)                                                                  정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                         9. UART 8250 드라이버 동작         255




                                       ch = serial_ inp(up, UART_RX) ;
                            e I se
                                       ch = 0;

                            f lag = TTY_NORMAL;
                            up->port. i count. rx++;

                            lsr 1= up->lsr_saved_f lags;
                            U口키釘_saved_f I ags = 0;

                            if (unl ikely( lsr & UART_LSR_BRK_ERROR_BITS) ) {
                                      /／통계목적으로 사용
                                      if ( Isr & UART_LSR_BI) {
                                                I sr 8= -( UART_LSR_FE I UART_LSR_PE) ;
                                                up->port. icount.brk++;
                                                if (uart_handle_break(&up->port) )
                                                           goto ignore_char;
                                      } else if ( I sr & UART_LSR_PE)
                                                up小>port. icount.par ity++;
                                      else if (lsr & UART_LSR_FE)
                                                up->port. icount. frame++;
                                      if ( lsr & UART_LSR_OE)
                                                up卞>port. i count .over run++;

                                        ／女
                                             * Mask off conditions which should be ignored.
                                             屯／
                                        lsr &= up->port. read_status_mask;

                                        if ( lsr 8 UART_LSRBI) {
                                                  DEBUG_ INTR( "handl ing break. . . . ..) ;
                                                  flag = TTY_BREAK;
                                        } else if ( i sr & UART_LSRYE)
                                                  flag = TTY_PARITY;
                                        else if ( I sr & UART_LSR_FE)
                                                  flag = TTY_FRAME;
                            }
                                f (uart_handle_sysrq_char (&up->port, ch) )
                                        goto ignore_char;

                            uart_ insert_char (&up->port, lsr, UART_LSROE, ch, flag) ;

           1gnore_char:
                              lsr = serial_ inp(up, UART_LSR) ;
                   } whi le ( ( lsr & (UART_LSR_DR I UART_LSR_Bl) ) 88 (max_count-- >0) ) ;
                   spin_unlock(&up->port. lock) ;
                   tty_f I 巾上uffer_push(tty) ;
                   spin_ lock(&up->port. lock) ;
                   *status = lsr;
           }




                                                  255 / 312
커널연구회（www.kernel.b기                                                             정쟤준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                  9. UART 8250 드라이버 동작   256




9.4.2 transmit_chars()


함수원헝      static void transmit_chars(struct uart_8250.port *up)


  설명      uart port의 버퍼（C나C上山） 내용을 uar t에 출력

매개변수      U口： uar t_8250p0r t 구조체 포인터


소스파일      dr iverslser ial/8250. c

 구조체1     at ruct uar t_8250por t
          struct circ but

          static void transmit_chars(struct uart_8250.町t *up)
          {
                    struct circ_buf *xmit = &up->port. state->xmit;
                    mnt count;

                    if (up->port. x_char) {
                             ser 治匕ou呵u口, UART_TX, up->port . 凡char) ;
                             up->port. icount. tx++;
                             up->port. x_char = 0;
                             return;
                    }
                    if (uart_tx_stopped(&up->port) ) {
                             ser ia18250_stop_ tx(&up->port) ;
                             return;
                    }
                    if (uart_circ_empty(xinit) ) {
                             十針叩_tx(up) ;
                             return ;
                    }
                   （刃unt = U口놔xJo耐끄；
                   do {
                             serial_out (up, UART_TX, xmit->buf[ xmit->tai ll) ;
                             xmit->tai l = (xmit->tai l + 1) & (UART_XMIT_SIZE - 1) ;
                             up->port. icount. tx++ ;
                             if (uart_c汀（L帥아叭加it) )
                                      break;
                   } whi le (- c어Jnt >0) ;

                    if (uart_ci rcchars卞pending(xmi t) < WAKEUP_CHARS)
                             uart_wr ite_wakeup(&up->port) ;

                    DEBUG_ INTR( 'THRE. . .") ;




           }
                    if   ("" " '   욘
                          uart_circ_empty(xmit) )
                                 stop_ tx(up) ;
Device Tree 상세분석 in Linux Kernel 4.0                           10. 삼성 UART 드라이버 동작         257




10. 삼성 UART 드라이버 동작




                                                             + 필자의 주말농장0杉｛ 찍은 장미꽃




지금까지 UART 드라이버가 어떻게 커널에 플랫폼 드라이버로 등록 되는지 기술했다.                                  필자는 삼
성 Exynos5420 보드로 실습하고 있으므로 실제적인 UART 동작은 삼성 Exynos5420 CPU 내부에서
이루어진다． 그러므로 삼성 Exynos5420 UART 동작을 확인하려면 drivers/ttylseriallsamsung.c 에
있는 소스들을 분석해먀 한다.                 지금부터는 saumsung.c에 있는 소스들이 어떻게 동작되는지 기술
한다.    이곳의 소스들은 위에서 기술한 UART 등록 논리와 비슷하므로 쉽게 이해할 수 있을 것이
다． 이곳의 소스를 이해하면 Exynos5420 CPU에서 UART가 동작되는 데이터를 실제적으로 확인할
수 있다．



10.1 드라이버 등록
먼저 drivers/tty/serial/samsung.c 에서 드라이버 등록에 관련되는 소스만 선별하면 아래와 같다．



staHc const struct dev_pmops s3c24xx_ser iaLpm_ops = {
        . suspend = s3c24xx_ser la匕suspend,
        . resume = s3c24xx_ser ia匕resume,
        . resume_noi rq = s3c24xx_ser ia匕resume_noi rq,
};
#def I ne SERIAL_SAMSUNG_PMOPS     (&s3c24xx_ser i a巾旺ops)


                                            257 / 312
커 널 연구회（www.k日n飢bz)                                              정재준 (rgl이3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                      10. 삼성 UART 드라이버 동작          258




#1 f def ined( CONE IG_ARCFLEXYNOS)
#define EXYNOS COMMON SERIAL DRV DATA                                        싸
           . info = &(struct s3c24xx_uart_ info) {                           卄
                      . name             = "Samsung Exynos UART ' ,   W
                      . type             = PORT_S3C6400,                     w
                      . has dlv引아        = ],                                w
                      .rx_ tifomask      = S5PV210_UFSTAT_RXMASK,     W
                      . rx_ t i foshi ft = S5PV210_UFSTAT_RXSHIFT,    W
                      . rx_ f i foful I  = S5PV210_UFSTAT_RXFULL,     W
                      . tx_ f i foful I  = S5PV210_UFSTAT_TXFULL,     W
                      . tx_f if omask    = S5PV210_UFSTAT_TXMASK,     W
                      . tx_f i foshi ft  = S5PV210_UFSTAT_TXSHIFT,    W




                                                                             뾰WW싸싸WW
                      . def _c比se I      = S3C2410_UCON_CLKSELO,
                      . num 이ks          = ],
                      .clksel_mask       = 0,
                      .clksel_shift      = 0,
          },
          .def_cfg = &(struct s3c2410_uartcfg) {
                   .ucon             = S5PV210_UCON_DEFAULT,
                   .uf con           = S5PV210_UFCON_DEFAULT,         W
                   . has_ f racval   = 1,                                    W
          }                                                                  W

static struct 53c24xx_ser ia匕drv_data exynos4210_ser ial_drv_data = {
         EXYNOS_C川MON_SERIAL_DRV_DATA,
         .fifosize = { 256, 64, 16, 16 },
};
stat ic struct s3c24xx_seria匕drv_data exyn0s5433_seria匕drv_data = {
          EXYNOS_COMMON_SER I AL_DRV_DATA,
          .fifosize = { 64, 256, 16, 256 },
};
#def i ne EXYNOS4210_SER I AL_DRV_DATA ( (kern이 ulo叩J 涵exyn054210_ser ia匕dry由ta)
#def i ne EXYN0S5433_SER I AL_DRV_DATA ( (kernel_ulong_t)&exynos5433_ser i al_dry_data)
#e I se
#detine EXYNOS4210 SERIAL DRV DATA (kernel_u Iong_ t)NULL
#define EXYNOSS433 SERIAL DRV DATA (kernel_u Iong_ t)NULL
#end if


static struct r니at f아叱由Vi(氾_ id s3c24xx_ser 治匕dr iver_ ids[ ] = {
          {
                     n可ne
                    .n aie             = \;3C24j0mUar
                                         's3c2410-uart n" ,
                    . dr
                     dnver
                         1Ver1data
                              data     = S3C24]0HSER1AL
                                         53C2410_SERIAL_DRV_DATA,
           },   {
                    .name
                     name              = nS3C24j2mUar
                                         "s3c2412-uart n,
                                                       ",
                    .（打 iVer data
                    .driver            = S3C2412_SER1AL
                                                    I _DR DRVDATA,
                                                            V_DATA,
           },   {
                    .name
                      name             = ns3c2440-uar
                                         nS3C2440mUar tn" ,
                    . driver
                         iVer data     = S3C2440_SER I AL_DRy_DATA,
                                                 SER1ALDRV
           },   {
                    .name
                      name             = HS3C6400UUar
                                         's3c6400-uartn, ",
                    . dr
                     driver
                         h/erHdata                     AL_DRV_DATA,
                                       = S3C6400_SER I1AL中DRV－
                                                             卜DATA,
           }.   {
                                                  258 I 312
커 널 연구회佃八사w.kernel.b기                                                        정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                    ](). 삼성 UART 드라이버 동작        259




                    .name              = "s5pv210-uartH,
                     dr i ver_data     = S5PV210_SER I AL_DRy_DATA,
         } {
                    .name              = " exynos4210-uart 'i ,
                    .dr iver_data      = EXYNOS4210_SERIAL_DRV_.DATA,

                    .name              = 「 exyn0s5433中uart「,
                    .driver_data       = EXYNOS5433_SERI AL_DRy_DATA,
         },
         { },
};
MODULE_DEVICE_TABLE(platform, s3c24xx_ser ial_dr iver_ ids) ;

#ifdef CONFIG OF
static const struct of_device_ id s3c24xx_uart_dt_match[ I = {
           .compatible = n samsung. s3c2410-uart ' ,
                  . data = (void *)S3C2410 SERIAL;DRV DATA },
           .compatible = "samsung, s3c2412-uart n,
                  . data = (void *)S3C2412 SERIAL DRV DATA }
           .compatible = n samsung, sc2440-uart ",
                  . data = (void *)S3C24405ERlALDRvDATA },
           .c에patible = " samsung ,s3c6400-uart ' ,
                  .data = (void *)S3C6400HSERIALmDRV DATA },
           .c에patible = 'samsunD ,s5pv210-uart' ,
                  . data = (void *)S5PV210-.SERIAL DRV DATA },
           .co1叩atibIe = ' s낌nsung,exynos4210-uart ' ,
                  .data = (vo너 日태川冬4210_SERIAL＝매V매TA },
           .compatible = " samsung,exynos5433-uar t" ,
                  . data = (void *)EXYNOS5433 SERIALeDRV DATA },
         {},
};
MODULE山테IC巳TABLE（아 , s3c24xx尸uar t卜dt尸match) ;
#endif

static struct platform_driver samsung_serial_driver = {
         .probe              = s3c2缸x胡rial.巾rc力e,
         . remove            = s3c24xx_serial_remove,
         . Id냐的le            = 53心取凡＄er ia匕dr iver_ids,
         . driver            = {
                     name    = "samsung-uart ",
                   . pm      = SER I AL_SAMSU새3_PM_OPS,
                   ; of match tab比 = of_mat ch_山（s3c24xx긔카t dt m카ch) ,
          }   :


}
modu 陀_platf아叱dr iver (samsunD_ser 泊匕dr iver) ;




위의 소스에서 플렛폼 드라이버로 등록하는 함수는 modu旭巾冶卄orm_driver(samsun（工羽rial먀iver);
이다．      이        함수는 매크로            정의되어     있으며      module_p怡卄아mdriver     매크로를 따라가       보면
히at化rm먀iv可_register() 함수를 호출하면서 이 함수에 매개변수로 samsung_serial_driver 구조체
를 넘긴다．            이 구조체는 멤버 변수로 id_tab陌과 of_match_tab旭을 가지고 있는데, 이곳에 삼성


                                                  259 / 312
커 널 연구회佃시／w.kernel.b기                                                     정재준 (rgbi3307@nate.con力
Device Tree 상세분석 In 니flux Kernel 4.0                                          10. 삼성 UART 드라이버 동작             260




UART를 식 별하는 정보를 전달된다.                               이 정보는 3장 ]3절에 언급한 UART 디바이스 트리 정보이다．
3장 ]3절에 있는 정보를 한번더 표시하면 아래와 같다．



如4姓
         serial_O: ser ial@12C00000 {
                  c에patible = ' sainsung,exynos4210-uart '' ;
                  reg = <0x12C00000 0xiOO> ;
                  interrupts = <0 51 0> ;
         };
         serial_i: serial@12C10000 {
                  co叫：}atible = "samsunq,exynos4210-uar t ";
                  reg = <0x12Ci0000 0xloo>;
                   nterrupts = <0 52 0>;
         };
         ser ia匕2: serial@i2C20000 {
                  compatible = ' samsunq,exynos4210-uart느
                  reg = <0xi2C20000 oxioo> ;
                   nterrupts = <0 53 0>;
         };
         ser ial_3: serial@i2C30000 {
                   compatible = 'samsung,exynos4210-uart ';
                   reg = <0xi2C30000 oxioo> ;
                   interrupts = <0 54 0>;
         };

위에서 compati비e 속성을 소스에서 파싱하여 UART 드라이버로 등록한다.                                             실제적인 등록은 플렛
폼 드라이버 구조체의 probe 멤버변수（함수 포인터）에 연결되어 있는 s3c24xx_seria냐玎obe() 함수
에 의해서 이루어 진다．




10.2 포트 정보
삼성 UART 포트정보는 다음과 같이 samsuflg.c 소스에 정의되어 있다．



#def ne _PORT_LOCK_UNLOCKED( i ) W
           SPIN_LOCK_UNLOCKED(s3c24xx_ser ial_por ts[ i ] port. lock)
static struct s3c24xx_uart_port
53c24xx_ser 1 a I _por ts[ CONE I G_SER I AL_SAMSUNG_UARTS} = {
          FO]   =   {
                        .port   =   {
                                        . lock         = _PORT_LOCK_UNLOCKED(O) ,
                                        . iotype       = UPIO_MEM,
                                        .uartc나（       = 0,
                                        .fitosize      = i6,

                                                        260 / 312
커 널 연구회（www.k타fl이b기                                                                 정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니nux Kerr倒 4.0                                       10. 삼성 UART 드라이버 동작           261




                                 ．야）S             = &s3c24xx ser 治匕叩S.
                                 .flags           = UPF_BOOLAUTOCONF,
                                 , l ine          =0,




                         .port = {
                                     . lock       = _PORLLOCK_UNLOCKED( 1) ,
                                     . iotype     = UPIO_MEM,
                                     .uartclk     = 0,
                                     .fifosize,   = 16,
                                     .ops         = &53c24xx_seriaLops,
                                     .flags       = UPF_BOOT_AUTOCONF,
                                     . l ine      = 1,
                         }
          },
卞치1 CONFIG SERIAL SAMSUNG UARTS >2

          t21    =   {
                         .port = {
                                     . lock       = _PORT_LOCK_UNLOCKED(2) ,
                                     . iotype     = UPIO_MEM,
                                     .uartc나（     = 0,
                                     .fifosize    = 16,
                                     ．야）5         = &s3c24xx ser 泊匕叩s,
                                     . flags      = UPF_BOOT_AUTOC에F,
                                     . l ine      = 2,
                         }
          },
#endif
#if CONFIG_SERIAL_SAMSUNG_UARTS > 3
          [ 3]   =   {
                         巾ort = {
                                     . lock       = _PORT_LOCK_UNLOCKED(3) ,
                                     . iotype     = UPIO_MEM,
                                     .uartclk     = 0,
                                     .fifosize    = 16,
                                     .ops         = &s3c24xx_seria匕ops,
                                     .flags       = UPF_BOOT_AUTOCONF,
                                     . l ine      = 3,
                         }
           }
#endi I
};
#undef     PORT LOCK UNLOCKED




                                                   261 / 312
커 널 연구회佃ww.kernel.bz)                                                          정자춘 四bi3307@nate.con力
Device Tree 상세분석 in 니flux Kernel 4.0                                        10. 삼성 UART 드라이버 동작               262




10.3 probe
실제적인 UART 드라이버 정보는 s3c24xx_serial_probe() 함수에서 설정된다． 이 함수는 UART 드
라이버가 커널에 인식될 때 실행된다.                             이 함수에서 삼성 Exynos5420 UART 포트 정보가 초기화
（정보 설정）되고 커널의 TTY 장치로 등록된다.                                 이 함수가 실행되는 과정을 Flow ［거agram으로 정
리하면 다음과 같다．



삼성 UART 드라이버 probe Flow 아agram
                samsung.c                                serial_core.c                          tty白．C



    4놔）                                              ar二묘＞



                                                 뇨    uar t_add_one_por t
        s3c24xx_ser iaLprobe                     尸




    4
                                                                    「

    (                                                                              1


                                                                               \
                                                                                        ＼枷畔叫小
                                                     uart_conf gure_port
                        'V
                                                                                   tty_register_device_attr

        s3c24xx_ser ial_ ini t_port

                                                                                                 1r
                                                                                       dev I ce_leg i ster




아래는 s3c24xx_serial_probe() 함수의 소스 코드이다．



static mnt s3c24xx_serial_probe(struct platforni device *pdev)
{
            struct device_node *np = pdev->dev.of node;
            struct s3c24xx_uart port *ourport;
            mnt index = probe index;
            int ret;

            if (np) {
                        rot =of_al ias_get_ id(np, n serial ") ;
                         f (ret >= 0) index = ret;
            }
            USER_DEBUG UART( 's3c24xx卄ser ial_probeO: index=%dWnn , index) ;


                                                        262 / 312
커 널 연구회柶w比kernel.b기                                                            정재준 杓bi3307@nate.com)
Device Tree 상세분석 ir) 나flux Kernel 4.0                                    ](). 삼성 UART 드라이버 동작        263




        dbg( s3c24xxmser ial_probe( p) %dWn'' , pdev, index) ;

        ourport = &s3c24xx_seriaL兀rts[ index] ;

        ourport->drv_data = s3c24xx_get_dr iver_data(pdev) ;
        if ( !ourport->drv_data) {
                 dev_err (&pdev->dev, "could not find dr iver dataWn") ;
                  return -ENODEV;
        }
        ourport->baudclk = ERR_PTR(-EINVAL) ;
        ourport->info = ourport->drv_data->info;
        ourport->cfg = (dev_get_platdata(&pdev->dev) ) ?
                          dev_geLpl atdata(&pdev->dev) :
                          ourport->drv_data->def_cfg;

        i f (np)
                   of_proper ty_read_u32(np,
                             "samsung,uart- fifosize", &ourport->port. t ifosize) ;

        if (ourport->drv_data->f i fosizef index] )
                 ourport->port. fifosize = ourport->drv_data->f 너osize[ index] ;
        else if (ourport->info->f i fosize)
                 ourport->port. fifosize = ourport->info->fifosize;

        probe_ index++;

        dbg( %s: initial sing port %p. , ,Wn「, 叫func_, ourport) ;

        ret = s3c24xx_seria匕init_port (ourport, 口dev) ;
        if (ret <0)
                 return ret ;

        if ( !s3c24xx_uart_drv. state) {
                  ret = uart_register_dr iver (&s3c24xx_uart_drv) ;
                  if (ret <0) {
                           pr_err (「Fai led to register Samsung UART driverWn) ;
                           return ret ;
                    }
        }
        dbg( "%s: adding 口ort岬n" , 寸func_) ;
        uart_adcLone_port (&s3c24xx_uart_drv, &ourport->port) ;
        platform1set_drvdata(pdev, &ourport->port) ;


            * Deact ivate the clock enabled in s3c24xx_seria匕ini t_port here,
            * so that a potential re-enabiornent through the pm-cal lback overlaps
            * and keeps the clock enabled in this case,
            t/
        c 나；_disable_unprepare(ourport->clk) ;

        ret = s3c24xx ser 治匕cpuf req_re이없er (ourport) ;
        if (ret <0)
                 dev_err (&pdev->dev, tai led to add cpuf req notifierWn") ;


                                                 263/ 312
커 널 연구회（www.kernel.b기                                                        정재준 四bi3307@nate.com)
Device Tree 상세분석 in 니flux Kerr倒 4.0                                   10. 삼성 UART 드라이버 동작            264




         return 0;
}




10.4 드라이버 동작
삼성 UART 드라이버 동작（실행）은 uart_ops 구조체로 정의되어 았는 s3c24xx_seria l_아巧 의 멤버변
수들（함수 포인터）에 연결되어 있는 함수들에 의해서 실행된다．



static struct uar Lops s3c24xx_seria匕ops = {
          . pm                = 53c24xx_seria匕pm,
          . tx_empty          = 53c24xx_ser ia匕tx_empty,
          .get_mctrl          = s3c24xx_seria匕get_mctrl ,
          .set_mctrl          = 53c24xx_serial_set_mctr l ,
          . slop_ tx          = s3c24xx_ser al_stop_ tx,
          . start_ tx         = 53c24xx_ser ial_start_ tx,
          . stop_rx           = s3c24xx ser ia匕stop_rx,
          . break_ct I        = s3c24xx_serial_break_ctl ,
          . startup           = s3c24xx_seria匕startup,
          .shutdo나n           = s3c24xx seria匕sh叭do나n,
          .set_ terrnios      = s3c24xx_serial_set_ termios,
          . type              = s3c24xx_seria匕type,
          . release_port      = 53c24xx seria匕r이明se_i兀rt,
          . request_port      = s3c24xx_ser ia匕request_port,
          .cont ig_port       = s3c24xx_ser ial_config_port,
          . verify_port       = s3c24xx_ser ia匕verify_port,
#11 del ined(CONF IG_SERIAL_SAMSUNG_CONSOLE) && del 1 ned(CONF田_CONSOLE_POLL)
            pol l_get_char = s3c24xx_ser ia匕get_pol I_char,
          .pol 匕口ut char = s3c24xx seria匕put_pol匕char,
#endif
};



위의 함수들에서 먼저 s3c24xx_serial_startup() 함수의 소스를 확인해 보면 아래와 같다．



static i nt s3c24xx_serial_startu口(struct uart_port *port)
{
         struct s3c24xx_uart_port *ourport = to_ourport (port) ;
         int ret;

         dbg( .: s3c24xx ser 1 a匕star tu可 r）아卜却 幅081 1 x .9b口）枷］” ,
             port, (unsigned long long)port->mapbase, port->membase) ;

         rx_enabled(port) = 1;

         ret = request_ i rq(ou나兀rt今rx_ i rq, s3c24xx_ser 泊匕rxJ才m田， 0,
                               s3c24xx_seria匕portname(port) , ourport) ;

                                               264 / 312
커 널 연구회（www.kerr倒. b기                                                      정재준 佃bi3307@ flate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                         10. 삼성 UART 드라이버 동작           265




        if (ret 1= 0) {
                 dev_err (port->dev 「 cannot get irq %dWn ' , ourport->rx_ irq) ;
                 return ret;
        }
        ourport->rx_claimed = 1;

        dbg( request ing tx irq. . .Wn「) ;

        tx_enabled(port) = 1;

        ret = request irq(ourport->tx irq, s3c24xx_seriaLtx_chars, 0,
                            s3c24xx seria匕叩I tname(p아 t) , ou나）ort) ;

            t   (ret)   {
                        deverr (port->dev,   cannot get irq %dWn『 , ourport->tx_ irq) ;
                        gob err;
        }
        ou나）ort ：나x claimed = ] ;

        dbg( ''s3c24xx_ser 1 al_startup okWn ") ;

        f玄 the port reset code should have done the correct
         士 register setup 化r the 口orb contro始 치／

        八나urn ret ;

err :
        s3c24xx seria匕帥utdo늬n如or ) ;
        return ret;
}


위의 소스에서 request_irq() 함수에서 커널의 인터럽트 서비스 함수로 등록되는 s3c24xx尸serial_tx
_chars() 함수와 s3c24xx_serial_rx_chars() 함수를 주의 깊7카 분석해 보자. 이들 함수를 분석하면
삼성 UART에서 어떻게 시리얼 라인에 문자를 전송制하고 수신（以）하는지 이해할 수 있다．




                                                     265 / 312
커널연구회（www.kern이.b기                                                               정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                   10. 삼성 UART 드라이버 동작            266




10.5 문자 전송(-奴工hars)
삼성 UART 장치에서 문자 전송은 s3c24xx_serial_tx _chars() 인터럽트 서비스 루틴 함수에서 동작
한다.     uart_port 구조체의 멤버 구조체인 ua八_state에서 circ buf（링버퍼）를 가져와서 이곳에 있는
데이터를 삼성 UART 전송 레지스터에 write하여 전송한다.                             아래는 이 함수가 실행되는 과정을
디ow 미agram으로 정리한 것이다．



삼성 UART 문자 전송
           drivers/tty/serial/samsung.c                          arch/arm/include/asm/io.h



      毋：d뜨出曾，毋＝m

    s3024xx ser ial tx   chars


    小

                                                        /
                                                               Hra叱나r i teb(val ,   I orneni 出addr)


      H
         H
                    \                               I
       wr_regb(uartport, reg, val)
                                               /
                          \\               /
               (uart_port) ->membase + (reg)




s3c24xx_serial_tx chars() 함수의 소스는 다음과 같다．



stat ic irqreturnj s3c24xxseriaLtx_chars( mnt irq, void *id)
{
         struct 53c24xxuart_port *ourport = id;
         struct uarLport 士port = &ou나）ort느＞口or t ;
         struct circbuf *xmit = &port->state->xmit;
         unsigned long t iags;
         1nt count;

         spin그oc乂나qsave（却아卜키吼k, f lags) ;

         count = CIRC_CNT_TO_END(xmit->head, xinit->tai I , UARLXMIT_SIZE) ;

                                               266 I 312
커 널 연구회柶WI以erne나끄）                                                        정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                   ](). 삼성 UART 드라이버 동작             267




        if (ourport->dma && ourport->dma->tx_chan && count >= port->fifosize) {
                s3c24xx_ser ia匕start_ tx_dma(ourport, count) ;
                goto out;
       }
        if (port->x_char) {
                 wr_regb(port, S3C2410_UTXH, port->x_char) ;
                 port->icount . tx++;
                 port->x_char = 0;
                 goto out;
        }
        /* if there isn t anything more to transmit, or the uart is now
         * stopped, disable the uart and exit
        文 /




            f (uart_이rc크叩ty(xmi t) 1 I uart놔tx_stopped(port) ) {
                    53c24xx seria匕針叩JM port) ;
                    goto out;
        }
       ／火 try and 小am       the buffer . . . 火／

        count = port->fifosize;
        whi le ( 山art_circ_empty(xmit) && count-- >0) {
                  if (rd_regl (port, 銘C2410_UFSTAT) & ourport->info->txjifoful l )
                           break;

                   畔r_regb(port, S3C2410_UTXH, xmit->buf[ xmit->tai l} );
                   xmit->tai l = (xmit->tai l + 1) & (UART_XMIT_SIZE - 1) ;
                   port->icount . tx++;
        }
        if (uart_circ_chars.'pending(xmit) < WAKEUP--CHARS) {
                 spin_unlock(&port->Iock) ;
                 uar t느卄r i te州akeu口（port) ;
                 S口in_ lock(&p아卜키 ock) ;
        }
        if (uart_circ_empty(xmit) )
                 s3c24xx_se r 治匕針叩_ tx( 叩rt ) ;

out
        spin_unlockjrqrestore(&port->lock, f lags) ;
        return IRQj-IANDLED;
}




                                                  267 / 312
커 널 연구회（www.ken倒. b기                                                          정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                            10. 삼성 UART 드라이버 동작         268




10.6 문자 수신(rx工hars)
삼성 UART 장치에서 문자 수신은 s3c24xx_serial_rx _chars() 인터럽트 서비스 루틴 함수에서 동작
한다． 이 함수는 삼성 UART 수신 레지스터에서 데이터를 읽어서（수신） tty_buffer（게 저장한다．
아래는 이 함수가 실행되는 과정을 Flow 미agram으로 정리한 것이다．



삼성 UAR了 문자 수신
                       drivers/tty/serial/samsung.c                            arch/arm/indude/asm/io.h



        茸珌好社趨m多珌越巍；



                        V

      s3c24xx_ser ia匕rxchars_pio




                                                                       1
                                                                                1ra叱readb(＋山meni 女addr)
                                                                           /
                                                             //
    口＝뇨二 f唾   小全．已   쪼1立芦j   卄烏.   n卦小小出斗品已二




        卞戶卞
          rd_regb(uart_port, reg)
                                                       /
                                     \            /                    /
               (uart_port) ->menibase + (reg)
                                                                   /
                                                            /
                                               uart insert chars


                                               .＝再雙m也 노g ：斗， 고小呼m




s3c24xxser1a1 rx _chars() 함수의 소스는 다음과 같다．


stat ic irqreturn_ t s3c24xx_seria匕rx_chars( int irq, void *dev_ id)
{
               struct s3c24xx_uarLport *ourport = dev_ id;

               1f (ourport->dma && ourport->dma->rx_chan)
                        return s3c24xx_ser ial_rx_chars_dma( irq, dev id) ;
               return s3c24xx_seria匕rx_charspio( irq, dev_ id) ;


                                                         268 / 312
커 널 연구회（叫／w.kernel.b기                                                             정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 나flux Kernel 4.0                                      10. 삼성 UART 드라이버 동작           269




}


stat ic irqreturn_t s3c24xx_seria匕rx_chars_pio( int irq, void *devejd)
{
        struct s3c24xx_uart卜port *ourport = dev_ id;
        struct uart_port *port = &ourport->port;
        unsigned mnt utcon, ch, flag, utstat, uerstat;
        unsigned long flags;
        mnt max_count = port->fitosize;

         spin_Iock_ irqsave(&port->lock, flags) ;

        叫hu 1e (max工에nt小 > 0) {
                 utcon = rd_regl (pqrt, S3C2410_lJFC0N) ;
                 uf stat = rd_regl (port, S3C2410_tJFSTAT) ;

                  if (s3c24xx_seriaLrx_ fifocnt (ourport, ufstat) == 0)
                           뱌 eak;

                  uerstat = rd_regl (port, S3C2410_UERSTAT) ;
                  ch = rd_regb(port, S3C2410_URXH) ;

                  if (port->f lags & UPFf에오다에） {
                           mlt txe = s3c24xx_serial_ txempty_not ifo(port) ;

                            if (rx_enabled(port) ) {
                                     if ( ltxe) {
                                               rx_enabled(port) = 0;
                                               cont inue;
                                     {}
                            } 이 se
                                          it (txe) {
                                                   Ut con 1= S3C2410_UFCON_RESETRX;
                                                   wrjegl (port, S3C2410_UFCON, ufcon) ;
                                                   rx_enabled(port) = 1;
                                                   sp i n_叩lock_i rqre없ore(&por卜키 ock,
                                                                       flags) ;
                                                   goto out;
                                          }
                                      （均nt inue;
                            }
                  }
                  1士 insert the charabfer into the buffer */

                  flag = TTY_NORMAL;
                  port-> i count. rx++;

                  it (unl ikely(uerstat & S3C2410_UERSTAT_ANY) ) {
                            dbg( "rxerr : port ch=Ox%02x, rxs=0x%08xWn",
                                 ch, uerstat) ;

                            ／士 check for break 火／
                            it (uerstat & S3C2410_UERSTAT_BREAK) {

                                                    269 / 312
커 널 연구회（V們川w.kerr何.b기                                                         정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kern이 4.0                                      10. 삼성 UART 드라이버 동작          270




                                       dbg( 'break!Wn" );
                                       port->icount.brk++;
                                       if (uart_handle_break(port) )
                                                 goto ignore_char;
                              }
                              if (uerstat & S3C2410_UERSTAT_FRAME)
                                       port->icount. frame++;
                              if (uerstat & 33C2410_UERSTAT_OVERRIJN)
                                       port->icount .overrun++;

                           uerstat &= port->read_status_mask;

                              if (uerstat & S3C2410_UERSTAT_BREAK)
                                       flag = TTY_BREAK;
                              else if (uerstat & S3C2410_UERSTAT_PARITY)
                                       flag = TTY_PARITY;
                              else if (uerstat & (S3C2410_UERSTAT_FRAME I
                                                     S3C2410_UERSTAT_OVERRUN) )
                                       f lag = TTY_FRAME;
                  }
                  if (uart_handle_sysrq나char (port, ch) )
                           goto ignore_char;

                 uart_ insert_char (port, uerstat, S3C2410_UERSTAT_OVERRUN,
                                     ch, flag) ;

ignore_char:
                 coat inue;
         }
        spin_unlock_ irqrestore(&port->lock, flags) ;
        tty_f 巾上Ut fer_push(&port->stat아叩아 t) ;

out:
         return lRQ_HANDLED;
}




                                                 270 / 312
커 널 연구회（www.kern이.b기                                                        정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                        11. TTY 실행 함수들       271




11. TTY 실행 함수들




                                                   + 필자의 주말농장에서 찍은 망태꽃




TTY 계층은 사용자 어플리케이션과 커 널의 UART 드라이버를 서로 연결시켜주는 역할을 한다.
TTY 계층을 위한 clas：는 커널이 부팅될 때 tty_classjnit() 함수에 의해서 설정된다· 아래는 이 함
수에서부터 tty class가 등록되는 흐름을 디ow Diagram으로 정리한 것이다·




                                       271 / 312
커 널 연구회佃ww.kernel.b기                                   정재준 (rgbi3307@nate.COm)
Device Tree 상세분석 in 니nux Kerr倒 4.0                                                                                              11. TTY 실행 함수들       272




TTY class 듕륙
       drivers/tty/tty_io.c                                                                              drivers/base/class.c



       tty_ciass_ inht


                                   \\\
                                                                              \+
                                                                                        1이弱乞아eate( "tty " )




                                                                                   叫
                                                                              戶尸d戶1d戶

                                         .                          (／
                                                                             尸戶


                                                                                                                         add class attrs
                              ,y二小 小           r/      i       ,   丘4 놔n 1



                 \/

                tty_devnode
                                                                                                             :
                                                                                        1classJ叩田 ter
                                                                                                                   /1
                                                                                                                            class create t i le ns


   阿   『／   ,   J沙   ‘   只   「「’   「好小       「 「1／ 「       ，   邕    d斗n
                                                                                        口三三＞                                           \/

                                                                                                                            sysf s_create_ f l ies




tty 계층에서 실행되는 함수는 drivers/tty/tty_io.c에 다음과 같이 fUe_operat山ns 구조체에 함수 포
인터로 연결되어 있다． 이들은 tty 드라이버가 등록될 때 tty 장치에 연결되어 동작한다．



liv 계충의 싫형曾수長

static const struct f i le_operat ions tty_fops = {
         . I Iseek          = no_ i iseek,
         , read             = tty_read,
         . wi i te          = tt）乙벡rite,
         .pol i             = tty_poi l ,
         .unlocked_ iocti   = tty_ ioct i ,
         . compat_ ioctl    = tty_compat_ iocti ,
         . open             = tty_open,
         . release          = tty_reiease,
         .fasync            = tty_ fasync,
};
stat ic cons! struct tu 1e_operations console_ fops = {
          . i lseek         = no_ i lseek,
          . read            = tty_read,
          . wri te          = redirected_ tty_wri te,
          .poi i            = tty_pol i ,
          .uniocked_ ioct l = tty_ ioct l ,

                                                                                             272 / 312
커널연구회（www.k아n飢b기                                                                                                        정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                  11. TTY 실행 함수들       273




                .compat_ ioct l          = tty_compat_ ioctl ,
                .open                    = tty_open,
                . release                = tty_release,
                .fasync                  = tty_ fasync,
};
stat ic const struct fi le_operations hung_up_ tty_ tops = {
          , I Iseek         = no_ I 1 seek,
          . read            = hung_up_ tty_read,
          . write           = hung_up tty_write,
          ．口oI l            = hu四_up_ tty_pol I ,
          .unlocked_ ioctl = hung_up_ tty_ ioctl ,
          .compat_ ioctl    = hung_up_ tty_compat_ioctl ,
          . release         = tty_release,
};
11.1 TTV 드라이버 등록
TTY 드라이버는 drivers／杖y/tty_io.c 소스에 있는 tt比re아吼er_driver() 함수에 의해서 커널에 등록된
 다． 이 함수부터 실행되는 흐름을 디ow ［거agram으로 정리하면 아래와 같다．



 TTY 드라이버 동륙
                                      drivers/tty/tty_io.c                            fs/chardev.c




                    iver
                               ,,：「
     뇨dr                   ,




            tty_register_dr iver
                                                             I ty_cdev_add
                                                         /
                     Ir

           tty_re9ister_device
                                                                             \    cdev mni t
                                                 ／늠
                                             /
                                                                                 <；」如如11)
                                                 J


           tty_register_device_attr




     위와 같이 TTY 드라이버 등록 과정을 거치면 사용자 어플리케이션에서 TTY 드라이버를 open,
     read, write, 山ctl, close 등의 함수를 통해서 시스템 콜하여 실행할 수 있다．




                                                                 273 / 312
     커 널 연구회（www.kernel.bz)                                                      정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                              11. TTY 실행 함수들          274




11.2 tty_open()
tty_open() 함수는 drivers/tty/tty_io.c 소스파일에 다음과 같은 흐름으로 구성되어 있다．
t勺op帥_current_tty(）에서 tty 구조체를 가져와서 이곳에 연결되어 있는 open 함수 포인터를 호출
하면 UART 소스 코드쪽의 uart_open() 함수가 호출된다．



ttyHopeno Flow Diagram
                                 drivers/tty/ttyio.c                       drivers/serial/serial_core.c


    工   尸도느 U   .   뇨m   工 小




                          纛知 小小 뇨




         tty_open




                                                                                  uar t_open


                                                                       /
        tty_open_cur rent_ tty                                              7*
                                                                   7
                                                    tt少＞ops＋야）en
                                               느

戈磁蓼斗斗＝
     「缸唯「 쁘包凞擾毋y                          1




tty_open() 함수의 실제 소스는 다음과 같다．



static mnt tty_open(struct i node *inode, struct fi le *fi 巾)
{
                struct tty_struct *tty;
                m }l noctty, retva1 ;
                struct tty_driver *drjver = NULL;
                m } t index;
                dev_ t device = inode->i_rdev;
                unsigned saved_flags = fi lp->f_f lags;

                nonseekable_open( mnode, fi lp) ;

retry_open:
         retval = tty_al b c_f i le(f i 巾) ;
         if (retval)
                  return -ENOMEM;

                noctty = fi 作卜놔_f lags & 0_NOCTTY;

                                                       274 / 312
커 널 연구회（www.kernel.b기                                                      정재준 (rgb13307@nate.corr力
Device Tree 상세분석 in Linux Kernel 4.0                                                 11. TTY 실행 함수들   275




        index = -1;
        retval = 0;

         tty = tty_open_current_tty(device, fi lp) ;
         if ( ! tty) {
                    mutex_ lock(& tty_niutex) ;
                    driver = tty_ lookup_driver (device, fl ip, &noctty, &index) ;
                    if (IS_ERR(driver) ) {
                              retval = PTR_ERR(driver) ;
                              goto err_unlock;
                  }
                  /* check whether were reopening an existing tty *1
                  tty = tty_driver_ lookup_ tty(driver, mnode, index) ;
                  if ( IS_ERR(tty) ) {
                            retval = PTR_ERR(tty) ;
                            goto err_unlock;
                  }
                   if (tty) {
                            mutex_unlock(&tty_mutex) ;
                            ttv lock(Ltv) ;
                            /火 saTe 19 crop me icrei irorn TTY_OflVer_ iOOKU_1tYT. ) *1
                            tty_kref_put (tty) ;
                            retval = tty_reopen(tty) ;
                            if (retval <0) {
                                     tty_unlock(tty) ;
                                     tty = ERR_PTR(retval) ;
                             }
                   } 이se { ／女 Returns 밖나h the tty_ lock hold for now 火／
                           tty = tty_ init_dev(driver, index) ;
                           nutex_un I ock(&t ty_mutex) ;
                   }
                   tty_dr iver_kref_put (dr iver) ;
         }
         if ( lS_ERR(tty) ) {
                   retval = PTR_ERR(tty) ;
                   goto err_fi le;
         }
         tty크dd_ fi le(tty, fi 作）) ;

         check_tty_count ( tty, _func_) ;
         if (tty->dr iver->type == TTYDRIVER_TYPE_PTY &&
                t ty寸>dr i ver->subtype == PTY_TYPEMASTER)
                      noctty = 1;
#ifdef TTY DEBUG HANGUP
         printk(KERN_DEBUG ''%s: opening %s . .Wn ' , __func__, tty->name) ;
#end if
         it (tty->ops->open)
                      retvai = tty->ops->open(tty, fl ip) ;
         e I se
                      retval = -ENODEV;
         f i 作卜놔_ f lags = saved_f lags;

                                                      275 / 312
커 널 연구회（www.kernel.b기                                                          정재준 似拍日307帥ate.con吩
Device Tree 상세분석 in Linux Kernel 4.0                                               11. TTY 실행 함수들   276




          i f (retval) {
#i fdef TTY_DEBUG_HANGUP
                    printk(KERN_DEBUG %s: error %d in opening %s. . . Wn ' , _func_ ,
                                       retval , tty->name) ;
#endi f
                    tty_unlock(tty) ; /* need to cal l tty_release without BTM */
                    tty_release( inode, fi 巾) ;
                    if (retval != -ERESTARTSYS)
                             return retval ;

                    if (signaLpending(current) )
                             return retval ;

                    scheduleQ;
                    /t
                     士 Need to reset t_야） in case a ha均up ha口口ened.
                     士／
                   if (tty小hung_up_p( f i 巾）)
                            fi lp->f_op = &tty_ fops;
                   goto retry_open;
          }
         clear_bi t (TTY_HUPPED, &tty->f lags) ;



            read_ lock(& taskl i st_ lock) ;
            spin_ lock_i rq(&current->sighand->sjglock) ;
            it ( !noctty &&
                 current->signal->leader &&
                 ?current->signal->tty &&
                 tty->session == NULL)
                      卞아oc 5이J 勺(t 口）;
            spin_unlock_ irq(&current->sighand-->sjglock) ;
            read_unlock(&taskl i st_ lock) ;
            tty_unlock(tty) ;
            return 0;
err_unlock:
           mutex_un lock(&tty_mutex) ;
           ／士 after b0c卜；s to avoid deadlock 火／
            if (! IS_ERR_OR_NULL(dr iver) )
                      tty_dr iver_kref_put (dr iver) ;
err f i le:
            tty_free_f i le(f i 巾) ;
            return retval ;
}




                                                   276 / 312
커 널 연구회佃ww.kern이.b기                                                        정재준 (rgb日307@nate.com)
Device Tree 상세분석 in 나flux Kernel 4.0                                                 11. liv 실행 함수들        277




11.3 ttymread()
tty_read() 함수는 TTY 장치파일에서 사용자 버퍼에 주어진 크기만큼 데이터를 읽는 역할을 한다．
이 함수가 실행되는 흐름을 Flow D日gram으로 정리하면 아래와 같다．



ttyread() Flo놔 아agr카TI
     drivers/tty/tty_io.c                         drivers/char/tty_Idisc.c        drivers/char/n_tty.c


 mb       ，戶r'




                                             1r    tty_ ldisc_reLwait



                                              /
    tty_ read                ///




        戶
                                         /

        뇨
                                                                             1        n_ tty_read




   tty_ ldisc수야冷今read
                                   나
                                     /
ttymread() 함수
 함수명             static ssize_t tty_read(struct fi le *fi le, char muser *buf, size_ t count,
                                                   loff_ t *ppos)


  설명             t ty 장치 파일에서 읽기

매개변수             f i le: tty 파일 포인터
                 buf :   사용자 버퍼
                 count : 사용자 버퍼의 크기
                 叩Os: 사용되지 않음


 소스파일            drivers/ char/ tty_ io. c

 구조체             struct   f i le
                 struct   tty_struct
                 struct   1 node
                 struct   ttyjdisc


   소스            static ssizej tty_read(struct f i le *f j le, char _user *buf, size t count,


                                                         277 / 312
커 널 연구회佃八Nw.kernel.b기                                                            琶재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                                       11. TTY 실행 함수들   278




                                             比ft t 出야）os)
          {
                  나lt   1 ;

                  struct tty_struct *tty ;
                  struct 1 node *jnode;
                  struct tty_ Idisc *ld;

                  Ity = (sfruct ttystruct *)f j Ie->private_data;
                  1node = f i l中기-r冶th. dentr少刈Unode;
                  it (tty_paranoia_check (tty, i n0de, 「 tty_read") )
                              return -EIO;
                    f ( ! tty I I (test_bit (TTY_ 10_ERROR, &tty->f lags) ))
                              return -EIO;

                  ／玄 We want to 卯alt for the Hne dis이이 1 ne to sort out in th田
                       Si tuat ion 火／
                  Id = tty. idiscjef_wai t (tty) ;
                     f ( ld->ops->read)
                               1 = ( ld->ops->read) ( tty, f i le, but, count) ;
                  （키 se
                               1 = -EIO;
                   t ty그미sc_deref ( Id) ;
                  if ( I      >   0)
                                   inode->i_at ice = current_ f s_ tinie( inode->i_sb) ;
                  retu口） 1 ;
          }




                                                    278 / 312
커널연구회（www.kernel.bz)                                                              정재준 (r야)i3307@nate.com)
Device Tree 상세분석 in Linux Kerr이 4.0                                                                                  11. TTY 실행 함수들      279




11.4 tty_write()
tty_write() 함수는 사용자 버퍼에 주어진 크기 만큼 전달한 데이터를 TTY 장치파일에 쓴다． 이 함
수가 동작되는 흐름을 Flow 미agram으로 정리하면 아래와 같다．



ttywrite() Flow Diagram
            driversltty/tty_io.c                                                  drivers/char/ttyldisc.c         drivers/char/n_tty.c


    (,
          ,：」으，        /




                                                                             7     tty_ ldis（乙refe州a나
                                                           /
                                                                             /
                                                                        //
          tty_ wr I te


                   瓢心穹客ty丹鮎叩Ct
                                                                        /
                                                               /j
                           二小나／
                                                                                                            1        n_ t ty_wr i te

               m   小   尸          1   m !r小구   r   山




                                                                                                     1
                                                       m   ' 卄； 三




                                                                             1/
                                                                                                                                \I
         t t y_ k키 Sc-＞야冷U＞州rite                                    /
                                                                                                                      uart wri te




tty_write() 함수의 실제 소스는 다음과 같다．



stat ic ssize_l tty_write(struct f i le *fi le, const char _user *buf ,
                                                         引ze_ t count , 10ff_I 朴）口os)
{
                   struct I ty_struct *tty = I i Ie_ tty( f i le) ;
                   struct tty_ ldisc *Id;
                   ssize t ret:

                   if (ttyparanoia_check(tty, fi le_ inode(f i le) , ' tty_wri te' ))
                               re山rn -EIO;
                   if ( ! tty I I ! tty->ops->wr i te I I
                               (test_bi t (TTY_ IO_ERflOR, &tty->f lags) ))
                                          return -EIO;
                   /火 Short term debug to catch buggy drivers */
                   if (tty->ops->write_room == NULL)
                               pr intk (KERN_ERR " fly dr iver %s lacks a wr i teroom rnethod. Wn' ,
                                          tty->driver->name) ;
                   Id = tty_ Idisc_ref_wait (tty) ;
                   i t ( I ld->ops->wr i te)


                                                                                         279 / 312
커 널 연구회（www.kernel.b기                                                                                           정재준 (rgb日307@nate.com)
Device Tree 상세분석 in 니flux Kerr伺 4.0                                               11. TTV 실행 함수들     280




                ret = -EIO;
       （키 se
                 ret = dotty_wr ite( ld->ops->write, tty, f i le, but, count) ;
       tty_ ldiscderet ( Id) ;
       return ret;
}




                                              280 / 312
커널연구회（www.kerneLb기                                                        정재준 (rgb13307@nate.corr卄
Device Tree 상세분석 in Linux Kernel 4.0                                     12. UART 실행 함수들        281




12. UART 실행 함수들




                                                                  平 필자의 주말농장0私I 찍은 장미꽃


시리얼 포트별로 실행되는 함수는 uart_ops 구조체를 seria治250_ 刃PS 라는 이름으로 drivers!

  serial/8250.c 에서 다음과 같이 함수 포인터로 연결된다．



uart叫ops 구조체에1
                   ud, L_opS ser ia18250下）ops = {
           . tx_empty             = ser ia18250_ tx_empty,
           .set_mctrl             = ser 1a18250_set_mctr I ,
           .get_rnctr I           = ser ia18250_get_mctr I ,
           . stop_ tx             = seria18250_stop_ tx,
           . start_ tx            = ser ia18250_start_ tx,
           .stop_rx               = ser 1a18250_stop_rx,
           . enablems             = ser ia18250_enable_ms,
           . break ct l           = ser1a18250_break_ctl ,
           . startup              = ser ia18250_startup,
           . shutdown             = ser ia18250_shutdown,
           .set_ terrnios         = ser 1a18250_set_ termios,
           .set_ Idisc            = seria18250_set_ Idisc,
           . pm                   = seria18250_pm,
           . type                   seria18250_ type,
           . release_i兀rt           ser 回8250_re陀ase_r兀rt,
           . request_ 兀rt           ser i a18250_request_por t,
           .conf ig_port            ser ia18250_config_port,
           . ver i ty_port          ser ia18250_verify_port,
   itdef CONFIG CONSOLE POLL

                                                    281 / 312
커널연구회（www.kerne냐끄）                                                    정재준 (rg1기3307@nate.com)
Device Tree 상세분석 in 니nux Kernel 4.0                                12. UART 실행 함수들           282




             pot 匕get_char = seria18250_gef_poH_char,
            .p01 Lput_char = ser ia18250_put_pol I_char,
  #endif
  };


위에서 정의된 sen키8250中p야巧는 UART 포트가 등록될 때 실행되는 seria18250_reg ister_portsQ
함수에서 ser1a18250_isa_in比ports(）를 호출하여 uart_port 구조체별로 uart_ops 구조체에 연결된다．




UART 드라이버의 실행은 tty_operations 구조체에 연결된 함수에 의해서 실행된다. tty_operations
구조체는 drivers/sen키八erial_core.c에서 다음과 같이 실행 함수들이 연결되어 있다．




stat ic const struct tty_operat ions uart_ops = {
          .0口en                 uart 야氾n,
          . close               uart_close,
         ．나ri te              = uar I 나r i te,
          . put_char          = uart_put_char,
          . f lush chars      = uart_ f lush_chars,
          . wri te_room       = uart_wri te_roorn,
          . chars_ in_buffer = uart_chars_ in_buffer,
          . f lush_buffer       uart_ f lush_buffer,
          . 山ctl                uart그octl ,
          . throttle            uart_ throttle,
          .unthrottle         = uart_unthroftle,
          .send_xchar         = uart_send_xchar,
          .sef_ fermios       = uart_sef_ termios,
          .sef_ ldisc           uart_set_ ldisc,
          . stop              = uart_stop,
          . start             = uart_start,
          . hangup            = uart_hangup,
          .break_ctl          = uarf_break_cf I ,
          . wail_unt i l_sent = uart_wai f_unti l_sent,
#ifdef CONFIG PROC FS
          , proc_ fops        = &uar f_proc_fops,
#endi f
          .fiocmgef           = uarf_ t iocmget,
          .liocmset           = uart_ t iocmset,
#ifdef CONFIGCONSOLE POLL
          ．口01匕tnt f          = uart_pol匕nit,
          . pot 匕get_char     = uar f_r珣1匕get_char,
          . pot I_put_char    = uar t_pol I_put_char,
#endi f
};

위의 구조체 함수는 UART 드라이버가 등록될 때 실행되는                              uart_reg ister_driver() 함수에서

                                                  282 / 312
커 널 연구회柶ww.kernel.b기                                           정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                           12. UART 실행 함수들     283




tt比set_operations(）를 호출하여 tty_driver 구조체의 tt丘operations에 연결된다．




12. ] 입출력（山） 함수들


입츌력 함수 매크로 정의
 매크로      ser m匕in口（U口 , of f set)
          ser 泊匕ou呵up, offset, va山e)

  설명      시리얼 입줄력 매크로 성의

매개변수      up: uart_8250port 구조체
          offset:
          value:


소스파일      dr ivers/ ser ial/8250. c

 구조처1      struct uart_port
           struct uart_8250_porf


  소스       #def ine serial_ in(up, offset)                 W
                     (up->port .ser ia _in(&(up) ->port, (offset) ))
           #def ine seria匕out (up, offset, value)          W
                     (up->por t .ser ia匕out (&(u口卜叩ort , 如ffset) , (va山e) ))

           #def ine ser ial inp(up, offset)               serial_ in(up, offset)
           #define ser ia匕outp(up, offset, value)         serial out (up, offset, value)




입출력 함수 섧정
 함수명       static void set_io_fronLupio(struct uartport *p)


  설명      시리얼 'L깁 술력 암수 O．크 길

매개변수       p: uart_port 구조체 포인터


소스파일       dr ivers/ ser ial/ 8250. c

 구조체       struct uart_port
           strucf uart_8250_port


  소스       statHc vo川 set_ iojr예J이이struct uart porf 사）)
           {

                                              283 I 312
커 널 연구회佃ww.kerne나）z)                                                     정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                      12. UART 실행 함수들     284「茗芬，三




                  struct uart_8250_port *ijp = (struct uar t_8250_port 火）口；
                  switch (p->iotype) {
                  case UPIO_HUB6:
                           r느＞ser m匕in = hub6 serial in;
                           p->ser ia匕out = hub6 serial out;
                           break;

                  case UPIOJEM:
                           p->ser 治匕in = mem_ser 治匕in;
                           口＞ser 治匕out = mein_ser ial_out ;
                           break;


                 ：業：   UPIO_RM9000:
                       UPIO_MEM32:
                           마＞ser 治匕in = mem32_ser ial_ in;
                           p->serial_out = mem32_serial_out;
                           break;

          #i fdet CONFIG_SERIAL_8250_AU1XOO
                    case UPIO AU:
                             p->serial_ in = au_serial_ in;
                             p->serial_out = au_serial_out;
                             바eak;
          #endi f
                    case UPIO TSI :
                             p>seria匕in = tsi_serial_ in;
                             F戶＞ser a匕out = ts匕ser 治匕out ;
                             break;

                  case UPIO_DWAPR:
                           p->serial_ in = mem_serial_ in;
                           口＞ser 治匕out = dwa以Lser 治匕out;
                           break;

                  default:
                             p->serial_ in = io_serial_ in;
                             口＞ser 泊匕out = io_ser ial_out;
                             break;
                  }
                  /* Remember loaded lotype */
                  뱌戶＞cur_ ioty口e = m키아y口e;
          }




입츌력 함수
 매크로      static unsigned mnt mern_serial_ in(struct uart_ 呵t *p, 1 nt offset)
          static void mem_serial_out (struct uart_ 川t *p, nt offset, mnt value)


  설명      시리얼 입줄력 함수

매개변수      p: uart나port 구조체 포인터
          offset:
          va山e:


                                            284 / 312
커 널 연구회柶ww.k아祠幻z)                                                    정재준 (r야이3307@nate.com)
Device 가ee 상세분석 in Linux Kernel 4.0                                         12. UART 실행 함수들   285




소스파일      di ivers/ serial/ 8250. c

 구조체      struct uarLport

          stat ic unsigned mnt memseriaI_ in(struct uartj)ort *p, mnt offset)
          {
                    offset = map_8250_ in_reg(p, offset) << p->regshift:
                    return readb(p->niembase + offset) ;
          }
          static void mem_ser ial_out (struct uart port *p,   nt offset, mnt value)
          {
                    offset = map8250out_reg(p, offset) << p->regshitt;
                    writeb(value, p->membase + offset) ;
          }
Device Tree 상세분석 in Linux Kernel 4.0                                               12. UART 실행 함수=          28e




다음은 uart小open() 함수의 소스 코드이다．


static mnt uart_open(struct tty_struct *tty, struct fi le *fi lp)
{
         struct uart_driver *drv = (struct uart_driver *)tty->drjver->drjver1state;
         mnt retval , l ine = tty->index;
         struct uart state *state = drv->state + l ine;
         struct tty_port *pOrt = &state->port;

         pr_debug( 'uartopen(%d) cal IedWn' , l ine) ;

         spin_lock_ irq(&port->lock) ;
         ++port->c0unt ;
         spmn_unlock_ 나q(&port->lock) ;

         ／火
              * We take the semaphore here to guarantee that we wont be re-entered
              * whi le al locating the state structure, or whi le we request any IROs
              * that the driver may need. This also has the nice side-effect that
              * it delays the action of uart_hangup, so we can guarantee that
              * state->port. tty wi l l always contain something reasonable.
              士／
         if (mutex그ock_ interru아 i비이＆por卜加utex) ) {
                  retval = -ERESTARTSYS;
                  goto end;
         }
         i f (! state->uart...port I I state->uart_port->f lags & UPF_DEAD) {
                    retval = -ENXIO;
                    g아o err긔n山ck;
         }
         tty->driver_data = state;
         state->uart_port->state = state;
         state->port. low_ latency =
                  (state->uart_port->f lags & UPF_LOW_LATENCY) ? 1 : 0;
         tty_port_ tty_set (port, tty) ;

         1*
              * Start up the serial port .
              玄／
         retval = uart_startup(tty, state, 0) ;

         ／卞
              * If we succeeded, wait unti l the port is ready.
              火／
         mutex_unlock(&port->mutex) ;
         if (retval == 0)
                  retval = tty_port_block.ji l_ready(port, tty, fi lp) ;

end:
         return retval ;
err_unlock:


                                                  286 I 312
커 널 연구회（www.kernel.b기                                                           정재준 (rgbi3307（亘）nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                                                                                 12. UART 실행 함수旨 287




                  mutex_un lock(&por t->mutex)
                  g아o end;
}




12.3 uart_write()
시리얼 8250을 위한 uart_write() 함수의 Flow D治gram은 아래와 같다．


                                                           drivers/tty/serial/serial core.c                                             8250 core.c


         ；斗＼ 7 ' "母   「       1乞
                                           "   「   '   :       口小二                「小




                                                                                                                 uart start



                                                                                                        I
                                                                                                            月L
                                                                      뇨            『       n吼小／mm
                                                                    唾；心




                                                                                                                         \    H    ser ia18250 start tx


                                                                                                    /
                                                                                                                                       尸m卜
                 uart wr i te



                                                                                              /
                                                                   니m叫， ,\




        「「奸提：『／多／                                                     ＼       「        ／
    m
                          r        口                       刃   1          '            ；二    月                                       transmit chars




아래는 uartwrite() 함수의 소스 코드를 정리한 것이다．


함수원형                                   計at i（二 mnt
                                       uart_write(struct ttymstruct *tty, coast unsigned char *buf,                                      nt count)

        설명                             비퍼의 내용을 uart port에 쓰기

매깨변수                                   tty: ttystruct 구조체 포인터
                                       but : 데이터 버퍼
                                       count : 버퍼 안의 데이터 개수


소스파일                                   drivers/ ser ial/ serial core. c

    구조체                                struct tty_struct
                                       struct uart state
                                       struct uart_port
                                       struct circ but


        소스                             stat ic mnt
                                       uart_wri te(struct tty_struct *tty, coast unsigned char *but , ! nt count)
                                       {
                                                                                                                 287/ 312
커 널 연구회（ww比kern이b기                                                                                                                정재준 畇bi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                        12. UART 실행 함수들      288




                  struct uart_state *state = tty->driver_data;
                  struct uarLport *port ;
                  struct C나c buf 女（irc;
                  unsigned long flags;
                  mnt c, ret = 0:

                  ／出
                       t 포트7F 이osed 된 이후에 이 함수를 호출 한다면
                       火/

                  if (! state) {
                            WARN_ON( 1) ;
                            return -EL3HLT;
                  }
                  port = stat中＞uartj兀rt ;
                  circ = &state->xrnit ;

                  if (!circ->but)
                           return 0;

                  spin_ lock_ irqsave(&port->lock, flags) ;
                  whi te (1) {
                            c = ClRC_SPACE_TO_ENO(circ->head. circ->tai l , UART_XMIT_SlZE) ;
                            if (count < c)
                                      C = （兀unt ;
                            if (C <= 0)
                                      break;
                            memcpy(circ->buf + circ->head, buf, c) ;
                            circ->head = (circ->head + c) & (UART_XMIT_SIZE - 1) ;
                            buf += c;
                            count -= C;
                            ret += c;
                  }
                  spin_untock_ irqrestore(&port->Iock, flags) ;

                  uart_start (tty) ;
                  return ret;
          }




                                              288 / 312
커널연구회佃w比畑rnel.b기                                                       정재臣 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                         부록1. Sensor 정보 요약        289




부록］, Sensor 정보 요약




                                                        年 필자의 주말농장에서 키운 토끼들

Al .1 Photoresistor

         Ught sensitive
        芦r e冶meat               Ph아ores治tor


 4二｝
                                 schematic
                                  symb여




                                 CdS
                               photocell


      Voltage increases            Voltage decreases
      as light increases           as light increases



                                           289 / 312
커널연구회佃w比kernel.bz)                                          정재준 (rgbi3307@nate.com)
                                                                    부록1. Sensor 정보 요약     290
Device Tree 상세분석 in 니flux Kernel 4.0




Al .2 Phototransistor


  디a卄ened edge




                    H冒
                                              Phototrans治t아
                                                schematic
                                                 symb이

                                     Emi姓or
           Collector I   I Emitter




                      V이始                                   5v야Is


                                                     Res洽tor
      Ph磁O                                           (see text)
    trans團tor



                                                  Ph아｛)             Output
           Re鈿S伯미 I          Output             trans油心r
           (see 把嗽）



           ＼씨怡ge increases                            允胎ge decreases
           as light increases                         as iorn increases




                                                290 / 312
  커널연구회佃w毗ernel.bz)                                                 정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                 부록］.Sensor 정보 요약          291




A1.3 거리 센서




Sharp IR Sensor




                                       291 / 312
커 널 연구회（www.kernel.b기                              졍재준 (rgbi3307（亘）nate.con升
Device Tree 상세분석 in Linux Kernel 4.0                                    부록1. Se小아 정보 요약             292




A1.4 적외선(Infrared) 센서

                                                                 Obstacle surface




                                                                             1
         5v이怡




 낟깖dt}: （毛，蠶붊：
                                          Output



                                                           LED
                                                                         -   II     -    Photo
                                                                                                「
                                                                                        transist。
                                                                                                r



              ' Ex口e幷rnentwithd斛erent valu客＄
              化rb日＄t ＄曲）＄烈vity
                                                                         누 I   I
                                                                               Ba州e




A1.5 초음파（U卄rasonic) 센서




                                               LED




                                        SRF02
                                       Vie놔ed from
                                     component side




                                               292 / 312
커 널 연구회佃w＼사.kernel.b기                                                 정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                    부록］. Sensor 정보 요약   293




Al .6 Accelerometers

참조AI-0'
    i i-E:. http://www.freescale.com/webapp/sps/site/homepage.jsp?code= SNSHOME&tid = ESH



Accelerometers（속도, 거리 측정）

 FXLS8471O Xtnn出c 14-b祛 Aco叫en取｝eter 田（X水 O治gram




                             三 "'형烈’響：..' ! 嚆礫卜                  1 趨繫單"
            斤乙타日.bon Veti甘
                                                                                             Oflantation
               瓷赳U寶                                  Det日di에       嚼竄曾                i1     DtC奴m

                                 !         "           中         니小       手            '         中
                                Amym小WA小口蜘en L口毋；出nh Pf口伊帥口4b如 小批inmt C口니rd甘


                                                                           智맵沙呻q恤
                     患熙：崙卄       粃‘踞炒4 加,, W球斗鈿叩，A"trS隘여"                  L0W 片口H甘 1 f出自사
                                                                           汁字，n自b口1心1느
                                                                           ！啣n씨




圄 $en邸也Blod仍     區 四帥S          Digital因（}cks    r    鈿pporting密ocks




                                                293 / 312
커널연구회（www.kern이.b기                                                                 정재준 (rgb日307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                            부록1. Sensor 정보 요약        294




Al .7 Magnetometers


M叩netometers（방향 측정，日ectronic Compass)




 Cap-A                     GND
  VDD                      INTl
   NC                      VODIO
 Cap-R                     SCL
  OND                      SDA


           (TOP ViEW)
                                                  (TOP VIEW)

 MAG3110 B幻ck C기agram




                                  MUX
                                              \

                              Lu

                        （갓O<水 Oscili針or




                                          294 / 312
커널연구회（www.kernel.b기                                            정재준 (rgt키3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                              부록1. Sensor 정보 요약        295




A1.8 Gyrosc아犯


Gyrosc이犯 （자이로스코프， 방향 기울기 측정）


  芦XAS21000 Xtrin鈿口 3-Ax治（却rO鉛｛苒冶




  心 i斗名e羽蜘佃出m魚困y




 원 I: http://blog.naver.com/PostView nhn?bloqld =eleexpert&logNo=140173635717




                                          295 / 312
 커널연구회佃ww.kernel.b기                                              정쟤준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                              부록1. Sensor 정보 요약       296




A1.9 배터리 센서

볘터러 섄서 （배터리 잔량 측정）

 MM912叫837 Simplified Application Drawing

                                                           912 637




                                                                                                          >?7 \J \ J }
                                                                                          工客1
                                                             啣
                                               AGNO                    LGN毋
                                                ADCGND
                                               ＼屈）Dt       奴地mai

                                                                                                 恕
                                                                        了SUP
                                                VDOH       知m弘       , ＼斗EMP
                                                           ＄母n莩U
     Z5VSupIy
                          {,
                                               VOO020      枾流i口｛a                                    岫
                               尸m
                                               낳針口x                    V아갸
     邕OVSoF弔寸y <                                                     V＄타＋SE
                                               V泣珉x
                           I                   功母4D
                                                                       vsu伊
                          낱
                                       /r
                                               VSS02D
                                               VSSRX




                                                                                                         \iiyi/ \trii/
                                               RE＄芒I
                  湘U橄t                         良ES횬y A
                               r               PA出M喀0
                                               PAl月나0針              溶ENSEH
                               三               PA2心CK
                                               PA춈죠
   5,OVD4芦珌堆＞ (                                PM
                                               PAS
                                               PAS
                               노               PA7
 0a奴嶝出너E泌帥名1                                   毋xcm爪'OOC
    Os亡毋帥畔                                     PE0EXTAI
                                               甲El汰TAt.
                                                                                H




                臘Xj了a址 4                       1毛ST




  M9Z1多38 匐mpl而ed Application 口曲wing


                                              工

                                                    ；斗月吼耐ar
                                            7V녑H4 VSENSEO




                卜
                   12V                                       VDDX
                                                  VDDA
                    日m놔
                                                              PAC
                                                  P180
                                                                                en      vd
                                                  F汗B5         TXf玉        t
                                                                                      CAN
                                                                                    Interface
                                                               只xD         rx
                                                  is딤4SEH
                                                                           am
                                                   SENSEL P1B4{
                                                      GWDs                           O     9
                                                       L                              V팜111多S
                                                                                     CA 寸 bus


                                    12 VA湃疝cation, CAN Communicati아｝




                                                              296 / 312
커널연구회佃w比陀rn이b기                                                                                  정쟤준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                부록］. Sensor 정보 요약     297




A1.10 위험（화재1, 가스누출）감지 센서

화재（열） 감지




  나ghttr어｝l




              I
 fire or flame -
 ／卜H步

 ／小＼   H十



             In打ared
            p豆＄S 釉始r
                10k
              re鈿苡아
            占焦g엾：ci




열（온도） 섄서




        LM34
     temperature
       sensor




                                       297 / 312
커널연구회佃ww.kerne나）z)                                 정재준 岫니3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                         부록］.Sensor 정보 요약         298




연기（CO2) 감지


  *-Near infrared                      Fan   raredmm   .




    2000 nm         3000 am
                                 戶


                              4000 am
                                             \
                                             5000 am




   們겪蜘 cour畑y 尸ar口蔽｝nhCi




                                         298 / 312
커 널 연구회（www.kernel.b기                                      정재준 (rgL기3307@nate.cori가
Device Tree 상세분석 in 니nux Kerr側 4.0                                                   부록2. 병렬처리        299




부록2. 병렬처리




                                                                                   斗 필자의 주말농장

A2.1 병렬처리 용어정리
（참조： http://ww＼사，w作dpedia.orq)

Multicore processor

동일한 칩에 여러 개의 실행장치（"cores"）을 내장하고 있는 아ocessor.
실행 싸이클마다 여러개 쓰레드안의 명령들을 동시에 처리할 수 있음．



Symmetric multiprocessing(SMP)

버스를 통하여 메모리를 공유하는 다중 처리기 .                            메모리를 공유해서 사용하므로 메모리 비용 부담
은 줄어 들지만, 메모리 bandwidth을 높여서 병목현상을 줄여야 하는 문제가 있음．


         (cPu    1        /CPU '  I        (CPU
                                                        1     <:
                                                                   :.   :>
                                                                    h/O

     /          System Bus or   Crossbar Switch         /
     /                   Mem이V
 /
                                                  299 / 312
커널연구회佃w比kern미b기                                                              정쟤준 (r야이3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                     부록2. 병렬처리




Asymmetric multiprocessing(AMP)

S卜4P 이전에 사용된 비대칭 다중처리 시스템．


         Processor   Process1玎         I/O




                                                     小山니




                                                           1\
        Mem미V




Distributed computing(distributed memory multiprocessor)

분산된 메모리 다중처리기 시스템.               처리 요소들은 네트워크로 연결됨．



(a)
           寸，        O
 (




                                  Processor


                                   Memo싸




  (c)
                                         300 I 312
커 널 연구회 (ww比kern飢b기                                             정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                            부록2. 병렬처리           301




Cluster computing

낮은 비용의 마이크로프로세서, 높은 속도의 네트워크, 고효율의 소프트웨어가 결합된 분산형 컴
퓨터 시스템．


Large Linux cluster at the Chemnitz University of Technology, Germany




Cubieboard cluster running Apache Hadoop (High-availability distributed object-oriented platform)




                                            301 / 312
커널연구회（www.kernel.bz)                                                    정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                                                   부록2. 병렬처리   302




                           : 전력（열） 소비

P = C x V2 x F


C: Capacitance(clock cycle마다 변화되고 트랜지스터 수에 비례）
\/: V히tage
F: processor Frequency(cycles/second)




프로그램의 병렬화. 마ocessor 수. 속도와의 상관관계
참조: http://en.wikipedia.orq/wiki/File:AmdahlsLaw.svg



                                                                               Amda川남 Law
     小n f4t


     '   "   ' W
                                                                                    /   ／尸／     十

     18,oo                                                                      /
                                                                           /                        Parallel Portion
     16小B                                                                J/                         們艸呼50%
                                                                    /                               卄- 75여뇨
     14船                                                      /                                          며昑6
                                                      /                                             m1弱弓自
     I且여｝                                         /
  季旨 '"      ‘的                      /
                                             //
                                                          /
                                                                  /／尸
         aDO
                                 /
                                         /
                             /
         。。O
                   " " "                 胄 斜 8 身 好 텅 賈 貫 弩 菖 亘 音 喜
                                                                        抽Un址ler of Proc月묘三or玉




                                                                               302 / 312
커 널 연구회（ww\A庶erne나）z)                                                                                    정쟤준 什gbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                                   부록2. 병렬처리      303




A2.2 필요 기술
니flux 커널을 cluster용으로 포팅
TCP기P 네트워크 프로그래밍
미9-Data 분산처리 알고리즘
Key(c山e) index 관리용 Hash Table 설계
맞춤형 B+Tree 자료구조 설계
SSD 동작 톡성을 파악하여 미g-Data에 최적화되는 SSD 디바이스드라이버 개발．
효율적인 TCP기P 네트워크 프로그래밍을 통하여 작업을 고르게 분산 배치 처리．
고객의 요구사항에 맞춤형으로 key index을 생성하여 Hash Table로 관리．
Key index를 빠르게 검색하는 맞춤형 B+Tree 자료구조 구축．
다양한 통계자료를 분산 병렬처리하여 산출．




                                1.7GHz               1.7GHz                1.7GHz       1.7GHz
                                  4GB                  4GB                  4GB          4GB
                                   1                       2                 3            4

                                   1       r               1     「     口    1      r       1
                                 1.7GHz              1.7GHz                1.7GHz       1.7GHz
                                  4GB                  4GB                  4GB          4GB
                                   5                       6                 7            8




                                                                     Hmn




                                 1.7GHz               1.7GHz               1.7GHz        1.7GHz
                                   4GB                     4GB               4GB          4GB
                                       9                   10                11           12

                                                           1                 1             1
          Contr이
            PC




                                               303 / 312
커널연구회（www.kernel.bz)                                                        정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                                 부록2. 병렬처리         304




A2.3 동작 시나리오
여러가지 다양한 미g- Data 중에서 교통정보와 의료정보에 대한 동작 시나리오 예시



其n毋手薑戈 사나쩍오
버스, 지하철등에서 발생하는 교통카드 결제 정보에 대하여 keywords을 부여하여 통계자료 산출．


버스와 지하철은 승객들의 승하차 시간, 승하차 장소등을 분석하여 시간 및 장소별로 승객들의 이
동 패턴 통계를 산출할 수 있다．


데이터 key index: 승객데이터（주민번호， 성별, 나이） / 승하차 장소 / 승하차 일시 /
통계 패턴 예제： 승객들의 성별 및 나이별로 승하차량이 가장 많은 장소（혼잡지역）, 일시（혼잡시간）


                                 승객              장소key      일자key         시간key
                                 hldeX            index
                                                  indeX     index
                                                            indeX         index
                                   l                   2      3             4

                                                       1     1              1
                                 장소                장소        일자            일자
                                 일자                시간        장소            시간
                                   5                   6      7             8

                                   1                   1     1              1
                                                                      H


                                  시간                   시간
                                  장소                   일자
                                       9               10                   12

                                   1                   1                    1




                                           304 I 312
커널연구회佃w＼사．kern이b기                                            정쟤준 (rgbi3307@nate.com)
Device Tree 상세분석 in 니flux Kernel 4.0                               부록2. 병렬처리   305




버스（청색）. 지하철（적색） 관심도（구글 트롄드）




          笠｝35                             2渡蘿     3斛 耳




강남역（청색）. 삼성역（적색） 관심도（구굻 트렌드）




서울qj청색）, 喜H(적색） 관심도（구글 트렌드）




                                                              Di
                                                               E
                                                          g
                                                          i
                                       305 / 312
커널연구회（ww毗erriel.b기                                  정재준 杓bi3307@nate.com)
Device Tree 상세분석 1n 니flux Kernel 4.0                                 부록2· 병렬처리        306




의丑겅보 長쩍 시나러오
병원의 진료기록 정보에 대하여 keywords를 부여하여 통계자료 산출．


병원에 진료기록이 있는 환자들의 진단（병명）정보, 각종검사（혈액, 초음파, 내시경）정보, 처방약정보
를 분석하여 의료정보에 관한 통계자료를 산출할 수 있댜．


데이터 key index: 환자정보（주민번호， 성별, 나이, 거주지， 직업） / 병명 / 검사정보 / 처방약정보
통계 패턴 예제·. 환자들의 성별, 나이, 거주지, 직업별로 질병 통계자료 산출．




                                 환Xr1            병명key      주소key         직업key
                                 index            index     index         index
                                   求1                  2      3             4

                                   1                   1      1       '     1
                                  병명               병명        주소            주소
                                 주소                직업        병명            직업
                                   S                   6      7             8

                                                       1      1             1
                                  직업               직업
                                  병명               주소
                                       9               10     11            12

                                   1「1「1'                    1 1            1




                                           306 / 312
커널연구회佃wwkerne陋）                                              정재준 (rgb日307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                             부록2 . 병렬처리        307




아산병원（황색）. 서울대병원（청색）. 세브란스병원（녹색）. 삼성서울병원（적색）




위암（적색）. 대장암（황색）. 폐암（뉵색）. 갑암（청색）




감기약（청색）, 진통제（황색）, 소화제（적색）



  i孕3




  8珏




                         笠好了                       各；n               2013




                                       307 / 312
커 널 연구회（www.kerne나끄）                                     정재준 (rgbi3307@nate.com)
     Device Tree 상세분석 in 니flux Kernel 4.0                    부록3. 커널연구회 교육과정                  308




     부록3. 커널연구회 교육과정

     A3.1 교육 일정


薑1
                                                            환급
斗                   교육과정명            일수     시간      교육비                   교육일시
                                                           （할인）
                                                                    ]
         !
                                                           일반인50%       매월 첫째주（월N목）
     i       c언어와 자료구조 알고리즘           4일    32시간    88만원
                                                           대학생60%        09:00 N 18:00



                                                           일반인50%       매월 둘째주（월N목）
             리눅스 시스템 프로그래밍            4일    32시간    88만원
                                                           대학생60%        09:00 N 18:00



                                                           일반인50%       매월 세째주（월N목）
             ARr＼기 아키텍쳐 , 펌웨어 실습      4일    32시간    99만원
                                                           대학생60%        09:00 싸 ] 8:00




「4 리눅스커널및드라이버실습4일 32시간 99만원 哉：:: "卄월，
                                   ,：넷，
                                     깬주，
                                      （월，
                                        ”，목）
             士 모든 교육과정에 대하여 커 널연구회에서 집필한 교재를 제공합니다．                                       '
             古 대학생은 모든 교육과정에 대하여 교육비 60% 할인해1 드립니다．

     亭 좀더 자세한 내용들은 커널연구회佃ww.kernei.b기 웹사이트를 참조하세요



     A3.2 교육 로드맵


              C언어                  리눅스                                     리눅스커널
             자료구조                  시스덛1                                     디바이스
             알고리즘               프로그래낑                                     드라이버실습




                                            308 / 312
     커널연구회佃w比kernel.L끄）                                      정재준 (rgbi3307@nate.com)
Device Tree 상세분석 in Linux Kernel 4.0                                   부록3. 커널연구회 교육과정                             309




A3.3 상서1 교육 내용 테이블
                   기초지식                1                  실무 실습                            심화 학습
           형태， 연산자， 표현                 三 포인터와 주소, 함수, 배뎔                      구조체 함수, 배열, 포인터
           제어흐름, 문장과 블록                    주소연산                               객체 지향 코딩
     C언어   조건판단, 반복문, 분기                   포인터 배열                             모듈화, 라이브러화
           함수, 영역（Sc야）e)                   함수 포인터                             대형 프로젝트 설계 코딩
           매크로, 전처리기                   三 복잡한 포인터 해석

           반복, 재귀, 포인터                 『 Linked List 구현                       Red-Black Tree 구현
자료구조       정렬 알고리즘                     三 Stack, Queue 실습                      B-Tree 구현
알고리즘       Bubble, Insertion,              Hashing 실습
           Merge, Quick, Heap              태nary Search 丁ree
           파일 입출력 이해                       마ocess 이해 및 실습
 리눅스
 시스템
           open, read, write, sync         化rk, exec 실습                ::::'二二“"""" """" " !
           seek, select, poll, epoll       zombi, daemon, wait
 프로그랭
           mmap                            thread , mutex 실습           1 네트워크 프로그래밍                               重




                                                                     目同
           ARM CortexM可計呼m呻기 UART, 12C쨔枉非이스                          "“삐
     ARM   AR卜ii Cortex-I\ 이해              12S, SPl 인터페이스
 아키텍쳐      메모리 맵                       1ADC, USB 인터페이스
蘿繫         어드레싱 이하1                    1RTC, TFT-LCD 인터페이스

           커널 자료구조 이해                      프로세스 스게쥴링 이하1               下玉而百可函1기
 리눅스       커 널 알고리즘 효율성                i 프로세스 스게쥴러 분석

     커널    마ocess 이하1                  i1 OIRI 己-l ［三 oh 六d
                                           나   니1
                                                    느J1   니   1 비1


     이론    문맥 교환 이해                        兀p/Bo如m Halves 이해
           쓰러匹 이해
                                                                       .'     0   '   나I   Q   너 크     나!         1
           리눅스 커널소스 빌드                     GPIO 드라이버 실습                三 l2C, SPI 장치 실습                           '1
 리눅스
           램디스크 포팅                         시리얼（UART) 드라이버                     USB 장치 실습
     커널
           부팅 과정 실습                        USB 드라이버 분석                        ADC 장치 실습
 디바이스
           Device Tree 이홰1                 UART 드라이버 상세분석                     통신 장치 실습
     실습
           Device Tree 실습                                                     (B山eTooth, WiFi)

           loT 데이터 수집기 작성                  분산 병렬처리 시스템                 1머신 러닝
                                                                                                                  1
                                                                                                                  :

     으요    온도， 습도. 속도, 기울기                 임베디드 클러스터 시스템                                   학습
                                                                       1                                          1
                                                                       1자연어                            '




 프로젝트      경사』 기압（고도）                      네트워크 분산처리                          대화형 인터겨           "1이스
           방향（나침반）, 조도                     빅데이터 수집 서버                  ! 지능，형 로봇                            . .   ]

希 좀더 자세한 내용들은 커널연구회（www.kernel.bz) 웹사이트를 참조하세요．


                                                    309 / 312
커 널 연구회(w사w.kernel.b기                                                         정재준 （四bi3307@nate.com)
Device Tree 상세분석 in 니nux Kernel 4.0                          부록3. 커널연구회 교육과정              310




A3.4 커널연구회 로드맵


연구개발 및 교육

        시스템
      프로그래밍

                                      忖




       디바이스                                                  하드워101 소프트 융합

       드라이버
                                                             지능형 센서. 모터제어


        리눅스                                                     자연어 학습
                                           ARM Cortex-A
         커널
                                              리눅스 커널 4.x      대화형 인터페이스
                                            미g.LITTLE 스케쥴링
       자료구조                                  멀티코어 병렬처리
       알고리즘                               B+Tree 자료구조 알코라奮
                                             네트워크 분산처리
                        ARM Cortex-M

                           온도. 습도
         C언어            속도. 기울기. 경사
                         도, 기압（고도）
                          방향（나침반）
                             거리
         ARM                 조도

       아키텍처




                   loT 데이터 수집기            분산 병렬처리 시스템        머신 러닝        지능형 로봇




      제품 개발 프로젝트

                                          310 / 312
커 널 연구회（www.kernel.b기                                        정쟤준 (rgb13307（흐）nate.cc乂n)
Device 가ee 상세분석 in Linux Kernel 4.0               부록3. 커널연구회 교육과정         311




A3.5 실습용 임베디드 보드，

ARM C아挺x-A15, Al（삼성 Exyn們542아




ARM Cortex-M3 (STM3ZF2)




                                      311 / 312
커 널 연구회佃ww.kern이b기                                정재준 的t키3307@nate.com)
    Device Tree 상세분석 in 니nux Kernel 4.0                     부록3. 커널연구회 교육과정           312




    A3.6 커널연구회 교육학원 위치（약도）

        .      주소： 서울시 금천구 두산로 70 （독산동 291-1)
                      현대지식산업센터 A동 26층 261］호


        S 교통： 지하철 ］호선 독산역 ］번출구
                     （도보 11분, 이동거리 708미터）
海醬戎餐표瓣瓣器樹1解三娜娜攝쪼反球好嫡駐解簪懈汝如熙＝      姆

!                              企
    즈광러畔'저      ,m, ra中      슐쩍聾
    크L11
     조각 ' 1     보참，몰드
                斗3丑二1        磊rI.
                             오피스혤 .뇨

                사문겋모델슐翠｛크


                                          幽
        t4tr                            쑹얗하파熙
                                                                    총거리 I＼加
                                                                    도보   U분
                                                                    자전거 3분


                                                                     可B동




                                                                                 1
                           蝕           용잔하이톄프
                          태옇햐짜r




                                                                                 /
    希 기타 내용들은 커널연구회佃ww.kernel.b기 웹사이트를 참조하시기 바랍니다．
    弗 감사합니다．




                                                312 / 312
    커널연구회佃ww.kern이幻기                                        정재준 (rgbi3307@nate.com)
1
Device Tree 상세분석 in 니flux Kernel 4.0
저자 정재준
 Copyright @ 2012-'-2015 커널연구회(www.kernel.bz). All rights reserved.
I뇨blished by 커널연구회（www.kernel.bz).
서울 금천구 두산로 70 현대지식산업센터 A동 26 층 2611 호



커널연구회는 리눅스 커널과 자료구조 알고리즘을 연구하고 리눅스 시스템 프로그래밍 및 '
디바이스드라이버 개발을 통하여 창의적인 프로젝트를 수행하여 JoT 관련 제품들을 만들어 일상 생활을
풍요롭고 편리하게 하는데 가치를 두고 있습니다. 아울러 관련 기술들을 교육하여 여러사람들과 공유할 수
있도록 노력하고 있습니다. "Device Tree 상세분석 in Linux Kernel 4.寸은 커널연구회가 그동안 수년동안
최신의 리눅스 커널 소스를 분석하고 정리해온 노력들이 그대로 책속에 담겨져 있습니다. 또한 삼성
Exynos5420이 탑재된 Arndale Octa 助ard에 리눅스커널 4.0 소스와 Device Tree를 포팅하는 과정을 '
그대로 따라하면서 실습할 수 있도록 내용을 구성하여 독자분들이 현장 업무에 그대로 적용할 수 있도록
했습니다．




Arndale Oc怡 Board 관련 정보 홈페이지 링크：
http://www.arndaIeboard.org/wiki/index.php/Main_page
Arndale Oc怡 Board 구매 관련 링크：
http://www.arndaIeboard.org/wiki/index.php/SaIeschanneI                   값 28,000원


      커널연구회
      /\／뇨＼
          ／뇨v. kernet.bz
                                                                      ,       IIll 卄
                                                                          7889 7 75 。,

                                                                          ISBN 978-89-97750-06-1

