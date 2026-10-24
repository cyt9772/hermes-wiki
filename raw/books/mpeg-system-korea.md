---
title: MPEG 시스템
authors: [유시룡, 장규환, 이병욱, 김종일, 정해묵]
publisher: (원문 미확인)
year: 1997
language: ko
pages: 253
book_slug: mpeg-system-korea
tags: [book, engineering, video-compression, mpeg-standard]
source_url: local-usb-drive (2026-10-24)
ingested: 2026-10-24
sha256: b7065f618d448fc3944735481331851d0acbf659ee2b769947af7f1eab9d9122
---

# MPEG 시스템 (raw source)
> 한국어 기술서, 253p (pdfinfo 기준). 텍스트 레이어 추출(pdftotext -layout) — 영문 알파벳 대문자가 깨지는 OCR 노이즈 다수(예: MPEG이 'MPG' 등 기타 문자열로 추출), 본문 가독.

## Book metadata
- title: MPEG 시스템
- authors: 유시룡 · 장규환 · 이병욱 · 김종일 · 정해묵 공저 (머리말 서명: 장규환, 1997년 7월)
- publisher: (원문 미확인)
- year: 1997
- pages: 253
- text_layer: yes (extraction verified, OCR 노이즈 있음)

## Chapter structure (from TOC)
1. 서론
2. 용어 정의
3. 약자와 기호
4. **트랜스포트 스트림과 프로그램 스트림** (스트림·패킷·패킷화, 시스템 인코딩 및 다중화, TS/PS 개요, PES 패킷, 타이밍 모델, 조건부 수신, 시스템 목표디코더 및 응용)
5. **시스템 목표디코더 모델** (프로그램 정의·구성정보, PSI 다중화/역다중화, **T-STD** 모델·버퍼·데이터 처리, **P-STD** 모델, 시스템 클럭 시맨틱: PCR·SC·ESCR·DTS·PTS, TS 스플라이싱)
6. **PES 패킷의 신택스와 의미** (일반적 PES, PSM, PSD PES 패킷)
7. **트랜스포트 스트림에서의 신택스와 의미** (TS 패킷, 적응필드, ...descriptor 계열, 부록: CSPS·참고 국제표준·TS 디코딩)

## Extracted text (pdftotext)
유시 룡 장규환    ] 병 욱 김 종일 정해 묵 공저




     MPEG은 시스템 , 비디오, 오디오의 작은 그룹들로
                            이루어져 있다．
                0I 책은 비디오, 오디오를 제외한
                 MPEG 시스템 부분을 기술적으로
           이해하고자 하는 사람들을 위한 것이다．
   따라서 0I 책은 MPEG을 알고자 하는 사람들을 위해
         만틀었으며 다양하고 쉽게 접근할 수 있는
                        방법을 제시하고 있다．
 MPEG 시스템
유시룡 · 장규환 · 이병욱 · 김종일 · 정해묵 공저
                                               好
                                                                                     可m口：
                                                                                        口：小：
                                                                                           口：小：口H口：
                                                                                                  口：口：
                                                                                                     口：口：
                                                                                                        口：



                                               머 리 말韆難難饔
                                                茗難魂":k 蚣鞋 N礫薰附難蓄




                   머리말

                                               ::::::;::';:；宅；:;:;:;:;：巖：:：我始；
                                                                              :;:;:：名守；   :;:;:;::;:;;:i:;:i:i:i：我：::::：解三羅牡ai
                                               !::：든薑그芒：:::：客：:::::::::::::::：妊：泣：   :::::::::::::::::::::::::a七고




 入4PEG은 디지털 화상 및 음성의 압축 표준화를 위한 국제기구의 약
식명칭으로 1988년부터 회의가 시작되었으나 印）11／가 활발해진 90년
대 초반에도 入4PEG은 일부 극소수 전문가만이 알고 있는 용어였다．
入4PEG은 시스템, 비디오, 오디오의 작은 그룹들로 이루어져 있으며 그
룹마다 각각의 분야에 대한 국제표준이 나와있다. 入4PEG 비디오표준은
入4PEG 오디오표준보다 획기척인 성공을 거두었으며 入IPEG이라는 용어
에서도 의미하듯이 入'IPEG은 곧 화상압축을 위한 국제표준이라고 알고
있는 사람도 적지 않다. 이렇게 널리 알려진 MPEG 비디오신호를 전송
또는 저장하기 위해서는 시스템의 도움이 절대적으로 필요한데 vll毛G
시스템은 入i:i묘J비디오와 오디오에 비해서 덜 알려져 있는 것이 사실
이다．
 入4PEG시스템은 入4PEG 표준의 일부분으로써 入4PEG비디오 또는 오디
오와 뗄래야 뗄 수 없는 관졔를 갖고 있다. 入4PEG 영상압축방식을 이
용한 CD-Video, Video on Demand나 디지털방송의 모든 데이터가
入WEG 시스템에서 정의되는 스트림형태로 저장 또는 전송된다. 그러나
入4PEG 시스템표준은 入4PEG 비디오 표준보다 더 까다로우며 기술적인
내용이 체계적으로 정리되어 있지 않아서 시스템 규격서만으로는 그
표준의 세세한 부분까지 알기가 힘든 형편이다．
 대우전자 영상연구소는 이미 MPEG 비디오에 대한 해설서를 발간하
였는데 이 책은 그동안 入4P1X；에 대해서 알고자 했던 많은 사람들의 갈
증을 풀어주었다고 감히 단언한다. 이제 다시 入4PEG 시스템부분의 갈
증을 해소해 주기 위해서 시스템부분에 대한 해설서를 선보이게 되었
는데 이미 발간된 入'IPEG 비디오와 이 책을 모두 이해하면 오디오를 쩌1
MPEG 시스템


           외한 入'IPEG의 모든 스트림들을 이해하는데 모자람이 없을 것으로 생각
           한다．
            이 책은 入WEG 시스템을 기술적으로 이해하고자 하는 사람들을 위한
           것이다. 따라서 혼동을 피하기 위하여 入'IPEG에서 정의한 용어나 매개
           변수들은 그대로 영어로 썼으며 , 표들도 入4PEG 표준에 있는 표를 그대
           로 이용하였다. 또한 入4PEG 표준을 참고하고자 하는 사람들을 위하여
           入IIPEG 표준에서의 표나 그림들의 번호를 따로 표시하여 참고에 편리하
           도록 하였다．




                                          1997년 7월
                                            장 규환
                          차 려1



1. 서론 / 7


2. 용어 정의 / 11


3. 약자와 기호 / 19

  0 연산자
                                       20
   cD 산술연산자                            20
   （勾 논리연산자
                                       21
   (3) 관계연산자                           21
   侄） H］트연산자
                                       21
   6) 할당연산자                        1   22
   但） 간략기호
                                       22
   (2) 상수                              23
 . 복호과정기술을 위한 통례
                                       23
   a:) 신택스기술을 위한 방법                    23
  （刃 함수의 정의
                                       25
   @ Re羽rv毗 白rbiddei긱 marker_bit
                                       27

4· 트랜스포트 스트림과 프로그램 스트림 / 27

 .개요
                                       28
 . 스트림， 패킷 및 패킷화의 개념
                                       29
 . 시스템 인코딩 및 다중화
                                       30
 0 트랜스포트 스트림
                                       31
MPEG 시스템


             . 프로그램 스트림                                                 34
             . 트랜스포트 스트림과 프로그램 스트림간의 상호변환                               35
             . 트랜스포트 스트림과 프로그램 스트림의 비교                                  36
             1PES(Packetized Elementary Stream) 패킷                      37

             . 타이밍 모델                                                   41
             . 조건부 수신                                                   44

             . 시스템 목표디코더 및 응용                                           45


           5. 시스템 목표디코더 모델 / 47

           卜 개요                                                         48

           卜프로그램                                                        48

              1 프로그램의 정의                                                48

              0 프로그램 구성정보                                               51

              1 PSI관련 시스템 다중화                                           56

              1 PSI관련 시스템 역다중화                                          59

           卜 T-STD(Transport stream System Target Decoder) 모델 및 동작 ' """ 61

              0卜STD 구성과 관련용어                                            61

              0卜STD의 입력시간                                               64

              1 T-STD의 버퍼와 트랜스포트 버퍼에서의 데이터 출력률                          66

              1 버퍼의 크기                                                   68

              0 다중화 버퍼로부터의 데이터 출력방법                                      70

              0卜STD에서의 데이터처리                                             73

              0 디코딩                                                      76

              1 재생                                                       76

              1 버퍼운영방법                                                   77

           卜 P-STD(Program stream System Target Decoder) 모델 및 동작         78

              0 P-STD 구성과 관련용어                                           78

              0 P-STD의 입력시간                                              80
    1P-STD 버퍼                                      80
    1PES 스트림
                                                   82
    1P-STD에서의 디코딩 및 재생
                                                   83
 卜 시스템클럭 및 시칸 표현
                                                   83
    S 시스템 클럭의 주파수와 오차
                                                   83
    0 PCR, SCR, ESCR
                                                   84
    1 DTS(Decoding Time
                         Stamp) "                  89
   0 PTS(Presentatjon Time
                            Stamp)                 92
   . 비디오 스트림에서 D心의 발생방법
                                                   95
   . 시스템에서의 시간정보 및 PSI의 발생시기
                                                   98
卜 트랜스포트 스트림의 스푤라이싱
                                                   98
   . 스플라이싱의 정의와 종류
                                                  98
   S 스폴라이싱에 태한 정보
                                                 100

 6. P匹 꽤킷의 신택스와 의미 / 101

卜 일반적인 PES 꽤킷
                                                 102
卜PSM(program stream map) PES 패킷
                                                 119
卜PSD(program stream directory) PES 패킷
                                                 123

7· 트랜스포트 스트림에서의 신택스와
                                      의미 / 129

卜 일반적인 TS 패킷
                                                 130
   S 적응필드
                                                 134
卜PSI(Program Specific
                       Information)              148
   0 PAT(Prograrn As釵ciation
                             Table)              150
   0 CAT(Condjtjonaj Acc弱
                            Table)               153
  1 PMT(Program Map
                       Table)                    155
  0 Private section의 신택스
                                                 159
MPEG 시스템


           8. 프로그램스트림0巾i의 신택스와 의미 / 163

           卜 프로그램 스트림의 pack                          ·   164

           卜System header                                166


           9. 서술자 / 171

             . 프로그램과 program element의 서술자                172

             S Video stream descript可                    173

             S Audio stream de釵：ript可                    175

              SI五erarchy des（그虹丈or                       176

              S Registration descriptor                  177

              0Data stream 呱gnment de釵그ipti丑             178

              0Target background grid descriptor         179

              0Video window descriptor                   180

              1Conditional access descriptor             ill

              S ISO 639 language des그iptor               182

              0System clock d釵riptor                     183

              S Multiplex b山fer utilization descriptor   184

              S Copyright descriptor                     185

                0Maximum bitrate descriptor              186

                0Private data indi沮tor des그iptor         186

                0Smoothing buffer descriptor             187

              1STD des그iptor                             188

                0IBP de釵그如切r                             188



            부    록

           卜CSPS(constrained system parameters stream)    192

           卜 참고국제표준                                       193

           卜 TS 스트림의 decoding 여］                          194
                                                          ]. 서 론




                                               서 론




 MPEG2는 시스템 , 비디오, 오口2 등의 작은 그룹들로 이루어져 있으며 , 현재 국제표준으로
된 01 3개 표준의 공식 명칭은 시스템이 ISO기EC 13818너 , 비디오가 ISO/lEG 13818귄 , 오C1
오가 ISO기EC 13818-301E1.
MPEG 시스템




            MPEG은 入'Loving Picture Exj玘us Omup의 약자로 정식 명칭은 ISO/IEC
           JTC1/SC29/WG11이다. 즉 국제 표준기관인 'So와 IEC의 Joint Technical
           Commit把e에서 SubCommittee 29의 Woul血gGmup 11이다. MPEG은 1988
           년에 설립되어 15명 정도로 시작하였으나 나중에는 20배가 넘는 인원
           으로 불어났다. 처음에는 저장매체를 근간으로 하는 1.外化PS급 이상의
           M匹好1으로 시작하였으나 入IPEGi 이 끝날 즈음인 1990년 9월 미국 산
           타클라라 회의부터 外4bps급 이상의 MI묘32에 대한 논의가 시작되어
           1994년 싱가폴 회의에서 MPEG2 IS(Intemational Standard）가 만들어지게
           되었다. MPEG2는 시스템, 비디오, 오디오 등의 작은 그룹들로 이루어
           져 있으며, 현재 Is로 된 이 3개 표준의 공식 명칭은 시스템이 ISO/IEC
           13818-1, 비디오가 'So雁C 13818그, 오디오가 ISO/IEC 13818-3이다．
            MPEG은 비디오와 오디오 신호를 압축하기 위한 표준으로 이미 널리
           알려져 있지만 시스템 부분은 그에 비해서 덜 알려져 있는 것이 사실
           이다. 시스템은 비디오와 오디오 파트에서 만든 elementaiy stream을 저
           장 또는 전송하기 위하여 패킷화하는 과정이다. 이 과정은 크게 두 가
           지로 구별할 수 있는데 하나는 CD求O入4과 같은 저장매체에 저장하기
           呈한 프로그램 스트림(program s住earn)을 만드는 과정이며, 또 하나는 너］
           트워크에서의 전송 또는 방송을 위한 트랜스포트 스트림（tra叫玭t
       . stream)을 만드는 과정이다. 트랜스포트 스트림은 실시간 전송을 목표로
           하여 구성되기 때문에 프로그램 스트림에 비해서 더 복잡하고 까다로
           운 면이 많다. 이 두 스트림은 각각의 특성에 맞도록 하기 위하여 구성
           방법이 틀리지만 공통되는 부분도 많기 때문에 이 책에서는 트랜스포
           트 스트림과 프로그램 스트림을 두 부분으로 크게 나누어 설명하지 않
           고 구성요소별로 설명하였다. 入IPEGi 표준은 저장매체를 목표로 하고
                                                                   ]. 서 론


있기 때문에 프로그램 스트림이 쓰이고 있으며, 八'IPEG2 표준은 프로그
램 스트림과 트랜스포트 스트림 모두를 포함한다. 따라서 八4PEG2 시스
템을 이해하면 MPEG! 시스템을 자연스럽게 이해할 수 있다．
 MPEG2 시스템파트는 II出oduction을 포함하여 Section 1, Section 2 및
부록의 너］ 부분으로 구성되어 있다. hltroduction 부분은 시스템 인코딩
과 디코딩에 관한 전반적인 소개와 Section 2에서 언급될 여러 가지의
개념들에 대한 설명으로 구성되며 Section 1 에는 시스템에서의 영역, 참
고문헌 및 표준들이 기록되어 있다．
 Section 2의 내용은 시스템 디코딩과정 및 용어들에 대한 뜻을 설명해
놓은 것이다. 시스템에서의 용어는 이 책의 2장에서 설명되는데 다소
생소할 뿐만 아니라 그 용어가 뜻하는 것을 정확하게 알지 못하면 나
중에 혼동될 염려가 있기 때문에 처음 대하는 용어들은 뜻을 한번 새
겨보고 넘어가는 것이 도움이 되리라 생각한다. 시간이 없는 사람이라
도 용어들 중 access unit, program, program 이ement 및 皿esentation unit는
꼭 한번 읽어보고 넘어가기 바란다. 기호나 약자 용어들에 대한 설명
은, 이 책의 3장에서 기술되었다. 이중 상당수는 대부분의 엔지니어들
에게 이미 알려져 있는 것이고 또 필요하면 언제든치 찾아볼 수 있지
만 미리 익혀두면 이해에 도움이 되리라 생각한다. Sect幻n2의 나머지
부분은 트랜스포트 스트림과 프로그램 스트림의 설명 및 신택스에 관
한 것이다. 이 설명 중 트랜스포트 스트림과 프로그램 스트림의 비교
및 상호변환등의 전체적인 설명은 본 책의 4장에서, 트랜스포트 스트림
의 시스템 목표디코더（T-STD）와 프로그램 스트림의 시스템 목표디코더
(P-STI가에 대해서는 5장에서 설명하겠다．
 제 5장에서는 시스템 인코딩이나 디코딩시의 클럭 , 타이 밍 , 프로그램
정보를 기술하는 방법 및 재생하는 기법등을 설명하였는데 필요에 따
라 적절한 예를 들어 표현하였다. 이는 신택스부분에 들어가기 전에 필
수적으로 이해해야 할 부분이다. 특히 이 부분에서는 프로그램의 구체
적인 개념정의와 入4PEG 시스템 표준에서 가정한 이상적인 시스템 디코
더 모델인 STD(system ta띵et decoder) 및 이에 준한 시스템 인코더구성에
MPEG 시스템


           대하여 참고적으로 언급하였다. 따라서 시스템 부분의 전체적인 개념
           파악 및 시스템의 신택스와 의미부분을 이해하는데 많은 도움을 줄 것
           이다. 入WEG 시스템의 부록은 본론 부분 중 몇 가지의 중요한 항목에
           대한 추가적인 설명이므로 따로 구성하치 않고 본문의 해당부분에서
           갇이 설명하도록 하겠다．
            참고로 MPEG2 표준은 디코딩규격이라는 점을 밝혀둔다. 入4PEG2에서
           는 특별히 인코딩과정을 규정하지 않고 있으므로, 인코딩은 어떻게 해
           도 관꼐가 없으며 비트 스트림이 신택스에 맞기만 하면 디코딩이 가능
           하다. 이러한 규정에 익숙하지 않은 사람은 이상하게 들릴지 모르지만
           이러한 이유로 入4IPEG2에는 인코더가 어떠한 것이 되더라도 디코딩이
           가능하도록 보호장치들이 되어 있다. 뒤에서 이러한 것을 언급할 필요
           가 있으면 그때그때 언급하도록 하겠다．
            이 책은 MPEG 시스템파트를 기술적 입장에서 알고자 하는 사람들을
           위하써 쓴 것이다. 그런 사람들이라면 入4PEG2 IS를 봐도 되지만,
           入4PEG2 IS는 보기가 그렇게 만만한 권고안은 아니다. 행간의 뜻을 읽어
           야 하며 뒷이야기를 알아야 한다. 이 책은 그런 사람들이 좀 더 시스템
           IS를 이해하기 쉽게 재구성하고 해설한 책이다. 마지막으로 덧붇이고
           싶은 말은 八4PEG은 전 세계의 전문가들이 모여서 수년간 만든 것이다．
           따라서 어떻게 보면 단순할지 모르지만 막상 프로그램을 짜려고 한다
           던가 특수한 경우에 대해서 入4PEG 시스템을 해석할 때는 만만한 문제
           들이 한 두 가치가 아니다. 따라서 이 책은 소설을 읽듯이 읽어도 되겠
           지만 그랬을 U귀 뒷부분으로 가면 갈수록 앞에서 나온 변수들이 혼동되
           고 뜻도 더 모호해지게 된다. 따라서 저자는 5장의 STD모델에서 설명
           되는 의미를 정확히 파악하기를 바라며, 6장 이후의 신택스부분에서 설
           명되는 변수들은 되도록 의미를 정확히 파악하고 그때그때 그 이름과
           뜻을 외우면서 나갈 것을 권하는 바이다．
                                                2. 용어 정의




                               용어 정의




access un仕 : 재생하고자 하는 단위의 부호화된 형태 . 오디오인 경우 엑세스 단위는 한 오디2
         프레임（frame）에 대한 코딩된 모든 데이터이며 비디오의 경우 엑세스 단위는 한
        咐ure의 모든 코딩된 테이터와 S加卄ing부분을 가리킨E}.
MPEG 시스템




    卜                                 용 0] 정 의



           1 access unit
               재생하고자 하는 단위의 부호화된 형태（coded rep肥senta砬on). 巨自코인
               경우 엑세스 단위는 한 오디오 프레임位跏e）의 코딩된 모든 데이터
               이며 呱疼의 경우，엑세스 단위는 한 pictu肥의 모든 코딩된 데이터
               와 stuffing부분을 가리킨다. 보통 한 picture의 엑세스 단위는 picture
               header를 포함하는데 picture data 앞에 sequen氾header나 G아） header가
               있는 경우의 엑세스 단위는 이 header들을 모두 포함하며 sequence의
               마지막 picture인 경우는 sequence endc以妃까지 포함한다．

           1
               bitrate
               압축된 비트 스트림이 채널로부터 디코더의 입력단으로 전달되는 속도

               byte aligned
           1




               어떤 비트가 그 비트 스트림의 첫 비트로부터 8비트의 배수되는 곳에
               위치할 때, 그 비트는 바이트 단위로 정렬（byte al坦ned）되었다고 말함

           1
               channel
               ISOfIEC 13818 스트림을 처장하거나 운반하는 디지털 매체

           1
               coded representation
               부호화된 형태로 표현되는 데이터 항목

           1
               com1月七ssion
               데이터 항목을 표현할 때 사용되는 비트 수를 줄이는 것

           1constant bitrate
               압축된 비트 스트림의 처음부터 마지막까지 비트율이 일정한 것
                                                         2, 용어 정의


·constrained system p針a犯ter stream(CSPS)[system]
     부록 1 에서 정의된 제한 조건이 적용되는 프로그램 스트림

 1
     CRC
     데이터가 틀리치 않았는가를 검증하기 위한 순회 중복체크 부호（cyclic
     redundancy check)

 1
     data element
     부호화 이전과 복호화 이후에 표현된대로의 데이터 항목

1
     decoded stream
     압축된 비트 스트림이 복호되어 복원된 것

1decoder
    복호과청을 구현하는 장치

1decoding(process)
     입력 부호화 비트 스트림을 받아들여 복호된 화상 또는 오디오 샘플
    값들을 출력하는 ISO/IEC 13818에서 정의되는 과정

     deco小ng time stamp(DTS)[system]
    PES 패킷 헤더에 나타나는 필드로서 시스템 목표디코더（Sm）에서 액
    세스 단위가 디코딩되는 시각을 나타낸다．

     小gital 就야age media(DSM)
    디지털 쩌장, 전송 기기, 또는 시스템

     DSM-CC(digital storage media command and control)
1




 Digital storage media 제어를 위한 명령과 제어문

·entitlement control message (ECM)
    조건부 수신（condi如n시 a凹ess）을 위하여 부가적으로 추가하는 제어명
    령이나 기타 제어정보. 보통 스트림에 따른 스크램블링이나 제어파라
 메터를 말한다．
MPEG 시스템


           1entitlement management message(EM江
            조건부 수신佃nditional access）을 위하여 부가적으로 특정 디코더의 허
            가 범위나 人相］스의 형태를 나타내는 정보. 한 7겪 또는 여러 개의 디
            코더에서 이용될 수 있다．

           1editing
               하나 이상의 압축된 비트 스트림들로부터 새로운 압축된 비트 스트
               림을 만드는 과정. 편집된 비트 스트림들은 ISO/IEC 13818에 정의되
               는 요구조건들을 만족해아 한다．

           1
               element世y stream
               부호화된 비디오, 부호화된 오디오 또는 기타 부호화된 비트 스트림
               중의 하나를 나타내는 일반적인 용어．
           1
               elementary stream clock r婉rence (ESCR)[system]
               PES 스트림의 디코딩을 위한 디코더가 시간을 맞추기 위해서 쓰는
               시간기준값

           1encoder
               부호화과정을 구현하는 장치

           1enc에ng(process)
               입력화상 또는 오디오 샘플의 스트림을 받아 들여 ISO/IEC 13818어］
               정의된 것과 같은 유효힌： 비트 스트림을 만들어내는 과정으로
               ISO/IEC 13818에는 규정되어 있치 않다．

           1entropy coding
               정보의 중복도佃1undai兀y）를 줄이기 위하여 디지털로 표현된 신호에
               적용되는 비손실 가변 킬이 부호화（variable length coding)
           1
               event
               공통의 시간기준값과 시작 시간, 끝나는 시간을 갖는 elementary
               steam들의 집합
                                                         2. 용어 정의


 1fast forward playback[video]
  화상 羽叩en（氾 또는 sequenc允의 일부를 화면에 실시간보다 빠르게 표
  시하는 과정

1forbidden
  "사용금지" 란 용어가 부호화 비트 스트림을 정의하는 조항에 사용되
  면 그 값은 절대 사용되지 않아야 함을 의미한다. 이것은 보통 시작
  부호（St쏘tcode）가 에뮬레이션되는 것（즉 데이터가 start C(넜e처럼 보이
  는 것）올 방지하기 위하1 사용된다．

· ITU-T REC丑끄2.01IISO/IEC 13818(multi川exed) sti氾帥B玲帥11
  ISO/IEC 13818-1에서 정의되는 대로 구성되는 0개 이상의 elementaiy
  stream으로 구성된 비트 스트림

· layer [video와 sys鈿1]
  'so爪iC 13818-I과 ISO/I C13818-2에서 정의되는 비디오와 시스템규격
  의 데이터 졔층구조에 있는 단게의 하나

1pack[system]
 팩은 팩 헤더와 그 뒤에 딸린 하나 이상의 패킷으로 구성된다. 이것
 은 ISOfIEC 13818-1에서 기술되는 시스템 부호화 구문상에 있는 계층
 중의 하나이다．

1packet[system]
 패킷은 헤더와 그 뒤에 딸린 여러 개의 연속된 elementary stre쏘TI의 바
 이트들로 쿠성된다. 이것은 ISO/IEC 13818-1 에 기술되는 시스템 부호
 화 구문상에 있는 계층의 하나이다．

1packet data [system]
 패킷 내에 있는 elementa口 stream의 연속된 데이터 바이트들

   ket ideni正er (ND)［町S扼ml
S 胛：
 하나 또는 여러 개의 transport stream에서 한 프로그램에 관련된
 이ementary stream들을 나타내기 위하여 사용되는 고유 번호
MPEG 시스템



           ·padding[audio]
               오디오 프레임에 슬롯을 추가함으로서 오디오 프레임의 평균 길이를
               해당 PC丕4 샘플 구간에 맞추는 방법

           1payload
                        Packet의 header 뒤에 따라 오는 b外e들（유료부하）

           1PES[system]
               Packetized E岫nenta口 Stream의 약어

           1PES packet[system}
               Elementa口 S甘earn의 데이터들을 운반하기 위하여 사용되어지는 데이
               터 구조. PES packet header와 유료부하로 구성된다．

           1PES packet header[system]
               PES packet에서 PES packet data byte 부분을 제외한 앞부분

           ·PES stream [system]
               유료부하에 갇은 종류의 elementa口 snam을 포함하고 S把am_id가 모
               두 같은 PES packet의 열

           1presentation thne stamp(PTS)[system]
               Packet header어］ 나타나는 필드로서 재생단위(presentation unit）가 시스
               템 목표디코더（S-Fl기에서 디스플레이되는 시각을 나타낸다．


                    " 毗t “m]                 /h入，
               복호된 오디오 액세스 단위 또는 복호된 pi아U肥로써 땐생트윅를 나
                                 ［玎就
               p心恤fib
           '
               타냄

           1program[systeml
               Program elen妃nt들의 집합. Pingrarn element는 이ementary strearn들이 될
               수 있으며 , 규정된 시간기준（time base）를 갖을 필요는 없지만 공통의
               동기된 재현을 위한 시간기준은 있어야 한다．
                                                      2. 용어 정의


 1program clock reference(PCR)[system]
  Decoder의 시간을 맞추기 위하여 시간기준값으로 transpo戊 stream에서
  전송된다．

 1program element[system]
  하나의 프로그램에 연관된 elementaiy stream들 또는 data stream들의
  총칭

 ·program specific i寸bimation(PSI)[町stem]
  까ogram이 어떻게 구성되어 있는지를 나타내는 것으로써 transport
  stream으로부터 프로그램을 성공적으로 재현하기 위해서 쓰이는 정보

1random access
  임의의 위치에서 부호화된 비트 스트림을 읽고 디코딩을 시작하는 과정

1reserved
  부호화 비트 스트림을 정의하는 구문에 사용되는 이 용어는 그 값이
  장차 Isofwc에 의한 확장에 사용될 수 있다는 것을 의미한다
                                         . 특별
  한 규정에 없으면 모든 reserved bit는 l 이 되어야 한다．

escrambling[system]
  허가받지 않는 수신을 방지하기 위하여 비디오, 오디오, 또는 그
                                      밖
  의 데이터의 순서를 바꾸는 것

1source stream
 압축부호화 이전의 다중화되지 않은 샘플들의 단일 스트림

1splicing[system]
 시스템레벨에서 두 개의 서로 다른 두 개의 elementa口 stream들을 접
 목시키는 일， 접목된 스트림은 ISO/IEC 13818-1의 규정을 다시 만족
 해야한다．

1start codes[system]
 비트 스트림 상의 32비트 부호로서 신택스내의 계층의 존재를 확인
 해주는 것을 포함하여 몇 가지 목적으로 사용된다．
MPEG 시스템


           1STI岫斟此bul吼r[system]
            시스템 목표 복호기의 입력단에 있는 F표乙 버퍼로서 복호하기 전에
            elementary 誼eam을 저장하기 위한 것이다．
           1
               sti［印ictw氾
            li-i住a co曲병된 하나의 pictu妃. 이 picture는 자신의 vrs를 갖고 있으며．
               뒤따라오는 picture들의 재생시간은 적어도 2장의 picture 이상 떨어져
               O｝ 한다．
           1
               system header[system]
                                匣 13818-1에 정의되는 데이터 구조로서 LSO/IEC
               Sys妃m header는 'so／
               13818-1 다중화 스트림의 시스템 특성이 요약되어 있는 정보를 전달
               한다．
           1
               system clock reference (SCR)[system]
               디코더의 시간을 맞추기 위하여 쓰는 시간기준값으로 pmgram st1eam
               에서 전송된다．
           1
               system target decoder(S띠D)[system]
               ISO/IEC 13818-1 다중화 비트 스트림의 의미（semantic하를 기술할 때
               사용되는 디코딩과정의 가상적 모델

               血e stamp[system]
               사건이 발생하는 시각을 나타내는 용어

           1transport strewn packet header[systemj
               Transpoit stream packet어］서의 처음부터 continuity_counter 변수까지의
               부분

               variable bitrate
               압축 비트 스트림을 복호할 때 비트율이 시간에 따라서 변하는 것
                                                          3. 약자와 기호




                                 약자와 기호




b引bf : 帥string left bit 仰st 여기서 le卄 b仕란 01 표준에서 쓰여진 bitstring을 그대로 보아서
      왼쪽이란 뜻이다．
MPEG 시스템




    卜                        약자와 기호



           이 표준을 기술하는데 쓰이는 약자와 기호들을 다음과 갇이 정의한다．


           0 연산자

           d) 산술연산자
              +
                       ：덧셈
              m


                       ：뺄셈
              卄
                       : l4식 증가
              小


                       : 1씩 감소                   1




                   水
             x 혹은 水 : 곱셈
             八
                       : 제곱승（power)
             /
                       : 결과를 0쪽으로 만들어주는 정수나누기. 예를 들어
                        刃4와 小 7/ -4의 결과는 1이고, - 7/4와 7／尸4의 결
                        과는 尸 1이다．
             //        : 결과를 가가운 정수쪽으로 만들어주는 정수나누기．
                        단, 딱 중간인 경우는 특별한 언급이 없는 한 0에서
                        먼쪽으로 올림한다. 예를 들어 3'口의 결과는 2이고
                         e 引口의 결과는 -2이다．
             Dlv       : 결과를 마이너스 무한때1 쪽으로 만들어주는 정수나누
                        기. 예를 들어 31玎V2의 결과는 1이고 - 31小口는 -2
                        이다．
             %         : 나머지 연산（양수에1 대해서만 정의됨）

                             지    -   1   (x> 0인 경우）
                         駐   酬
                                      0   (x==O인 경우）
                                  -   -   (x< 0인 경우）
                                                                   3. 약자와 기호

          的           )
                       : 가장 가까운 정수를 선택함. 중간값인 0.5는 1로 된다．
          鈿
                      : sine 함수




          邸 帥 r 岫 唾
                      : （刃sine 함수
                      : exponential 함수
                      : square r刃I: 함수
                      ：상용로그
                      ：자연로그


（刃 논리연산자

     II               : 논리적 OR

          姚 !
                      : 논리적 AND
                      : 논리적 NOT


(3) 관계연산자

                        크．
                                                                    >

          乂
                      : 크거나 같은
      <
                      ：작은
      乍
                      : 작거나 같은
      =
                      ：같은
      느
                      : 갇지 않은
 max{,..., } : { ｝안의 값중 최대값
 n丘n{,.··, } : { ｝안의 값중 최소값


4) 비트연산자

 &                    : bit별 AND
 1                    : bit별 OR
 >                    : MSB가 왼쪽이라고 가정하고 shift right(sign bit는 그냥
                       연장시킨다．)
  <          : MSB가 왼쪽이라고 가정하고 shift le丘(LSB쪽은 0으로
               채운다．)


(5) 할당연산자

  =          : 할당


（今 간략기호

  ·bslbf: Bitstring left bit 如.st 여기서 le丘 bit란 이 표준에서 쓰여진
      bitstring 그대로 보아서 왼쪽이란 뜻이다. B畑tring은 '0000 0001'
      과 같이 single quo把 ma水로 둘러쳐서 표시한다. 비트 스트림내
      의 빈칸은 아무 의미가 없으며 단지 읽기 쉽게 하기 위한 목적
      으로 사용된다．
      ch: 채널
      gr: 오디오 꼐층 II에서 3 x 32개 서브밴드 샘플로 구성된 그래
      뉼（granule) 또는 오디오 꼐층 ifi에서 18 x 32깨의 서브밴드 샘
      플로 구성된 그래뉼（오디오）
  ·main.data: 비트 스트림의 main data 부분은 스케일 팩터와 허
      프만 부호화된 데이터 및 보조 정보를 포함한다但－디오）.
  ·ma通data小eg: 비트 스트림상에서 그 프레임의 main由ta가 入］
      작하는 위치. 그 위치는 이천 프레임의 main由ta가 끝나는 위
      치에 1비트를 더한 것과 같다. 이것은 이전 프레임의 main
      data_end값으로부터 꼐산된다（오디오）.
      pai仁len帥： 스케일 꽥터로 사용된 n佈nd趾all］트의 수（오디오）
      rpchof: 나머지 다항식의 계수들, 최고차 항이 먼처 나온다但．
      디오）.
      sb: 서브밴드（오디오）
      Sc箇： Sca1efact兀 selection information. 스케일 팩터 선택 정보
      switch_pointJ: 윈도우내에서 스위칭이 일어나는 위치에서의 스
      케일 팩터 대역의 번호（긴 블럭 스케일 팩터 대역 : 오디오）
                                                                            3. 약자와 기호


           Si村tch_poii北HS : 윈도우 내에서 스위칭이 일어나
                                             는 위치에서의
           스케일 팩터 대역의 번호（짧은 블러 스케일 팩터
                                                                  대역 : 오디
           오）
           tcimsbf: two's complement integer, most significant
       1

                                                               bit first. 2's
           （刃mple毗nt 정수, 최상위 비트가 먼저 나온다．
           uiinsbf: unsigned integer, n均St significant bit first. 부호없
       1

                                                                     는 정수표
           현, 최상위 비트가 먼저 나온다．
           vldbf: variable length coding, left bit first. 가변킬
                                                              이 부호, 좌측 비
           트가 먼저 나온다. 여기에서 좌측은 가변장부호가
                                                                 쓰여지는 순
           서를 의미한다．
           window: blockj까玘＝2, 0 <= window <=2인 경우에
                                                                  실제 타임슬
           롯의 번호


    여러 개의 바이트로 이루어진 부호어에서는 최상위
                               바이트가
   먼저 나온다．


(2) 상 수

  7r              :3.14159265358 ···
  e               : 2.71828182845 ···



0 복호과정 기술을 위한 통려1

d) 신택스 기술을 위한 방법

       Syntax의 각 data항은 굵은 문자로 표시되고, 각 항목마
                                  다 이름，
  bit수가 나와 있다. 또한 전송순서와 형태는 간략기호伽ne
                                    monics)
  로 나타내고 있다. 다음은 이 표준에서 쓰이는 문장의
                                 예를 표시
  한 것이다．
MPEG 시스템



           while (condition)
           {
                                       만약 조건이 참이면 뒤의 data element가 실행된다．
                   da七a elernen七
                                       이는 조건이 참이 아닐 때까지 반복된다．

               }

           do {
                   data element
                                       data 타ement가 적어도 한 번은 일어난다．
                                       이 조건이 참이 아닐 때까지 이 data element는 반복된다．
           }
           while (condition)

           if (condi亡ic江1)         {
                   da亡a elernen七
                                       만약 조건이 참이면 첫번째 data element가 실행된다．
           }else (                     만약 조건이 거짓이면 두 번째 data element가 실행된다．
                   da七a elernen七
           }

           for (i=O; in;        i)
           {
                   da七a elernen七       data element가 n번 실행된다．


           }

           ／女 cormien七 女／/             설명을 위한 부분으로 지워도 된다．


                     1
                         data_etement[ ] : data-element[］는 뎨이터의 어레이이다. 데이터
                         성분의 개수는 문장 전후 관졔에 의해 알 수 있다．
                     1
                         data_element[n] : data_element[n］는 그 데이터 어레이의 n+1 번째
                         성분이다．
                         data_element[m][n] : data_e佃nent[m][미는 2차원 데이터 어레이의
                         m+1, n+1번째 성분이다．
                     1
                         data_element[I][m][n] : data_element[1}[m][n］는 3차원 데이터 어레
                         이의 1+1, m+1, n+1번째 성분이다．
                                                          3. 약자와 기호


     1
         data_element[m..n] : data_element에서 m번째와 n번째를 포함하는
         m과 n 사이의 범위이다．


(2) 함수（ft끄iction)의 정의
    · byte川igned() : 현재의 위치가 by也의 比undaiy에 있을 때, 즉
      bit出emn의 바로 다음 bit가 다른 byte의 처음 bit면 1을 나타내
         고 아니면 0을 나타낸다．
         nextbitsQ: Bi帥earn에서 바로 다음 bit와의 비교를 의미한다．
     1



    1
         next_st카t凹de() : 영으로 된 bit나 by把의 stu飯ng을 제거한 후
         의 그 다음 S切it code를 나타낸다．


（匈Re- 극erved, forbidden, marker bit
    · I心erved: 미래의 사용을 위하여 특별한 정의를 하지 않은 값
         forbidden: 이 표준에서 사용되어서는 안되는 값（데이터가 stait
    1




         code처럼 보이는 것（emula如n)올 피하기 위한 이유 등으로）
    1
         marker_bit: Start code emulation올 피하기 위하여 신택스상에
         강제로 값이 "1" 인 한 bit를 집어넣은 것．
                            4. 트랜스포트 스트림과 프로그램 스트림




                       스포트
                       프로그‘




 TS s甘田m은 일련의 TS packet으로 구성되는데 이 TS 附J俄의 킬이는 항상 ]88by也로 동일하다．
PS S甘明m은 일련의 Pa水으로 구성되는테 pa沫의 킬이는 일반적으로 가변적이고 보통 TSpad俄의 킬
이보다 훰씬 킬［:}.
MPEG 시스템



           .    개요

               ISO/fEC 13818-1의 시스템 파트는 시스템 코딩에 관한 전반적인 분야
           의 퀀고안이다. 여기서 시스템 코딩이란 압축된 오디오나 비디오 스트
           림뿐만 아니라 필요에 따라 사용자 데이터를 다중화하여 전송 또는 저
           장에 적합하도록 만드는 포장（d毗a formatting）에 관한 것이다. 이와 갇이
           여러개의 비트 스트림을 입력받아 일련의 스트림으로 포장하는 과정을
           시스템 인코딩이라 하고, 포장한 것을 원래의 입력된 형태로 풀어내는
           과정을 시스템 디코딩이라 한다. 여기서 포장하는 규칙을 신택스라 하
           며 신택스를 만드는 과정에서 각 부분의 의미를 규정해 둔 것이 신택
           스의 의미（semantics）이다. 入'JPEG 시스템 파트에서는 포장하는 규칙인
           신택스를 규정하고 있으므로 시스템 코딩시 이와 갇은 규칙에 따라 시
           스템 비트 스트림을 만들어야 하며 , 시스템 디코더는 이 규칙으로 만들
           어진 스트림을 디코딩할 수 있어야 한다. 여기서 시스템 인코딩을 수행
           하는 시스템 인코더는 다음과 같은 기본적인 5가지 동작을 효율척으로
           수행할 수 있는 방법을 제공한다．

               · 동기화（synchmnization): 복수 개의 elementaxy stre帥i(user data 포함）으
                로 구성된 프로그램을 시스템 디코더에서 디코딩할 때 각 elementary
                slitam 디코더 상호간의 동기를 맞추어 재생할 수 있도록 한다．
               · 다중화： 복수개의 이ementary stream을 하나의 단일 스트림으로 묶어
                저장 또는 전송 등의 응용에 적합하도록 하는 방법을 제시한다．
               , 버퍼 초기화
                      ： 시스템 디코더의 출력인 각 elementary stream들에 대
                한 디코딩 초기 동작시 버퍼의 초기 동작 레벨을 맞추어 준다．
               ' 버퍼관리： 초기의 버퍼레벨 조정 후에도 elementary stream 디코더의
                버퍼 레벨제어를 효율적으로 수행하도록 하여 디코더 단의 모든 버
                퍼에서 und아flow나 ov口flow가 발생하지 않도록 한다．
               · 시간규정 : 각 elementa口 stream 또는 프로그램（프로그램의 개념은 5
                장에서 언급됨）마다 시간을 나타내는 값을 삽입하도록 하여 스트림
                또는 프로그램들의 재생, 상호변환을 용이하게 하며, 다른 스트림이
                              AT1 -L=
                                   드 랴나뇨 立 드 人 드 at ifl 五 근 기 己H 人 드 己1
                                       - 니니m1 미11叫 口 m기
                                                      -H느   -c口   --I=




     나 프로그램으로 또 다시 다중화하는 경우에 시간기준값을 유지하
     도록 하여 원래의 스트림이나 프로그램을 효율적으로 재생할 수 있
     도록 한다．

    위에서 설명한 5가지의 기능에 모두 부합하는 시스템 스트림（transport
혹은 pm얍am stre町n）을 구성할 수 있도록 system IS는 시스템 목표디코
더와 신택스를 규정, 퀀고하고 있다．


.    스트림' 3괘킷 및 패킷화의 개념

    본 절에서는 入IPEG sys把mIS를 이해하는 과정에서 독자가 혼동하기
쉬운 스트림 , 패킷, 패킷화등에 대하여 간단 명료히 기술하기로 한다．
스트림은 비트열로서 보통 시스템 인코딩을 수행한 결과를 총칭하는
용어로 사용되거나 또는 특정한 스트림의 부분만을 치칭하여 쓰일 수
있으므로 system IS를 읽어가는 과정에서 너무 엄밀한 의미로 해석하려
하면 혼동될 수 있다. 예를 들어 입력 스트림은 입력되는 비트열을 의
미하며 이것이 ele毗ntary stream일 수도 있으며, 만일 시스템 디코더로
입력되는 스트림이라면 시스템 인코딩된 트랜스포트 스트림이나 프로
그램 스트림일 수도 있다. 따라서 상황에 따라 융통성있게 이해하며 해
석해야 한다．
 .패킷은 보통 header와 유료부하（pa列oad）로 이루어진다. 유로부하 부분
에는 스트림이 일정한 길이로 잘려서 삽입되며, header 부분에는 기타의
유용한 정보（예를 들어, 시간정보, 주소나 꼬리표 등）가 들어간다. 패킷
읖 만드는 과청을 패킷화라 한다
                ． 본 시스템 코딩에서는 elementa口
stream이 패킷화（packetiz血g）를 수행하기 위한 입력 스트림이 되며, 좀더
광범위한 의미로는 어떤 형태의 스트림이라도 시스템 인코더의 입력이
될 수 있다. 이 elementary str啣Ti이 패킷화된 겻읖卜    (pzed elemen-
taiy stream) packet이라 한다. 이 과정을 간단히 블럭으로 표시하면 그림
午1 고｝ 같다．
MPEG 시 人 Eli
         口
        111




                    elementary                  PACKETIZER                    PES packet
                    stream
                                                         A
                                                         1
                                                         1
                                                         1
                                                  valuable data
                                       (identification, time, length, etc.)

                          그림 午1. Elementary stream, packetizer 및 PES packet으｝ 관꼐1



               0 시스템 인코딩 및 다중화

                시스템 인코딩과정은 단순히 각각의 압축된 오디오, 비디오 스트림들
               을 묶어 결합시키는 기능 뿐만 아니라 스트림을 디코딩하는 과정에서
               시스템 디코더 내부의 버퍼제어 및 각 디코딩된 스트림들의 동기를 맞
               추어 재생하기 위한 변수들（parameter）이 삽입된다. 시스템 인코딩 방법
               은 伽nspo仄 stream 인코딩과 program stream 인코딩의 두 가지 형태가 있
               다. Transport stream은 주로 전송을 위해 사용되고 pm얍m stream은 주로
               저장을 위하1 사용된다. 보통 편의상 仕ansport stream을 四 誼eam이라 하
               고 program stream을 PS stream이라 한다. Aud幻／video stream으로부터
               packe血er를 거처 PS stream 또는 四 stream을 만드는 개략적인 시스템
               인코더의 블럭도는 그림 中2와 갇다. 그림 4-2에서 오디오 인코더와 ii
               디오 인코더는 八WEG1, 또는 入皿EG2 오디오 또는 비디오 인코더로 가
               정할 수도 있지만 일반적으로 入WEG2 시스템 인코딩은 入4PEG 계열이
               아닌 다른 인코더로 인코딩된 스트림을 배제하지는 않으므로 11.261 비
               디오 인코더나 CCITF G.721 오디오 인코더, 혹은 특정한 사용자들만을
               위해 사용하는 독특한 오디오, 비디오 인코더도 가능하다. 이들 인코더
               에서 인코딩된 데이터를 elen伸佃口 stream이라 하는데 이 elementary
               stream들은 일차적으로 각각의 packe血er를 통하여 패킷화된다. 이 과정
               을 거치면 PES(Packefized 日e毗n恤y Stream) 패킷이 만들어지는뎨, PES
               packet을 만드는 packe血er를 PES packe血er라 한다. 그림 4-2에서 audio
               /video PES packe血er를 거친 각각의 PES pa味et인 audio PES packet, video
               PES packet은 PS(Program Stream) MUX 혹은 TS(Transport Stream) MUX
                                       4. 트랜스포트 스트림과 프로그램 스트림



                                            Audio
             Audio
                 H              Audio       PES
             Encoder          Packetizer               PS
                                                            Program


                                                    MUX.    Stream
             Video
                 H              Video
             Encoder   瓜

                       1
                              Packetizer

                                    Video
                     d畔，뼈塔 如m"      PES
                                                       TS
                                                            Transport

                                                            Stream
                                                    MUX.




                                 시스템 스트림 작성부
                                     (sytem encoder)


                그림 小2. ISO在EC 13818 Sy弑em EnX녔町의 개요



단에 입력되고 이 부분에서는 각각 PS stream과 TS stream을 만들게 된
다. 시스템 인코딩 이란 결국 그림 +2의 점선 이후를 지칭하는데
elementary stream을 입력받아 PES 패킷화를 하고 TS stre缸n이나 PS
stream을 만드뉵 과정에 해당한다．


.    트랜스포트 스트림

    TS(Transp（月tS甘eam) 는 일련의 TS packet으로 구성되는데 TS packet들
은 각각의 길이가 188byte로 일정하다. 이는 MP且끄, MPEG2 및 기타의
방법으로 압축된 elementary s甘earn등을 전송에러가 존채하는 채널로 전
송하기 위하여 정한 일정한 형식을 말한다. 入IPEG2에서 언급하는 TS
S甘啣n은 대표적으로 아래와 같은 다섯 가지 경우에 있어서 최소한의
동작으로 구현 가능하도록 구성되어야 한다．
MPEG 시스템



                                                            Video           )Decoded
                                                            Decoder
                                                                              Video
                                                                A




                       Channel           Transport
             Channel                     Stream              Clock
                       spec小c                                contr이
                       decoder           demultiplex
                                         and decode




                                                            Audio            >Decoded
                                                            Decoder            Au五O
                                 Transport Stream
                                 containing
                                 one or multiple
                                 pro얍ams

              그림 中3. TS S七毗'In으로부터 각각의 el已l妃ntary steam읕 디코딩하는 여］




           ·TS stream으로부터 각각의 elen妃ntaty stream을 디코딩할 수 있어야
            한다（그림 牛3).
           · 여러개의 프로그램으로 구성된 TS Stream에서 하나의 프로그램을
            춧출하고 이 추출된 한 개의 프로그램으로부터 TS Stream을 만들
            수 있어야 한다（그림 4-4).
           · 한 71] 혹은 여러 개의 TS Stream으로부터 한 7긔1 혹은 여러 개의 프
            로그램에 관한 TS Stream을 추출한 후 이를 다른 TSStn氾m으로 만




                Channel     Channel                     Transport
                            specific                    Stream
                            decocer                     remultiplex




                                        Transport Stream              Transport Stream
                                        containing                    with
                                        multiple programs             single program

           그림 午4. 복수 개의 立쿠口랩으로 구성된 TS Sti才n에서 하나의 三工쿠 口램으로 구성
                  된 TS Stream을 만드는 여］
                                                4. 트랜스포트 스트림과 프로그램 스트림




                                program [I]     Transport                 TS Stream
                                                Stream
                  Transport



      I
                                                remultiplex               w亢／i
                  Stream
                                                                          single program
                  demultiplex
                                     1
                                program [2]
   Transport Stream                  LeH->      Transport                 TS Stream
   containning single or
                                                Stream
   multiple programs
                                                remultiplex               with
                                program [ii
                                     rHH+
                                                                          multiple program

                  Transport
                  Stream
                  demultiplex                   Transport                 TS Stream
                                                Stream
                                program [i+l]   remultiplex               with
                                                                          single program

:2림 小5. 한 711 이상의 TS Stmam으로부터 다른 立쿠口램으로
                                                                           구성된 흐｝ 7下1 이상
          의 TS Stream읕 만드는 예


 TS Stream으로부터 하나의 프로그램을 추출하고 이것으
                                  로부터 PS
 Stream을 만들 수 있어야 한다（그림 牛6).



                                                      Program                   Progrrm


                                 program [11
                                            1         stream
                                                      multiplexer
                                                                      爪
                                                                                Stream

                                                                  1
   Channel     Channel           Transport                    1
               specific          Stream                 Clock
               decoder           demultiplex            control
                                 and decode



                                                      Program                  Progrrm
                                                      stream
                                                      multiplexer               Stream

                      Transport Stream
                      containing
                      one or multiple
                      programs

그림 4-6. 한 7뀨 （키상의 J工무기램으로 구성된 1S Stre旺TI으로부터
                                                                            한 7뀨 이상의 PS
        Stream읕 만드는 여］
MPEG 시스템


               1
                   PS stream을 받아 TSstream을 구성하는 과정에서 원래의 PSsnealn
                   과 동일한 기능을 수행할 수 있는 정보를 갖도록 IS stream을 구성
                   할 수 있어야 한다．


           .       프로그램 스트림

               PS stream은 일련의 pack으로 구성되는데 오디오나 비디오 스트림이
           나 그 이외의 데이터를 전송에러가 거의 없는 선로나 저장매체를 통하
           여 송수신하기 위한 목적으로 이용된다. 컴퓨터 네트워크를 이용한 통
           신이나 CD-RO入4등에서의 저장 또는 재생, 컴퓨터 상에서의 소프트웨
           어를 이용한 압축 또는 복원등에 적합한 방식이며 디지털 VCR에도 응
           용가능한 스트림의 형태이다. 대표적인 PS stream 디코더의 형태는 그
           림 4-7과 같다. 채널을 통해 수신된 PS stream은 program stream dem따小
           미exer와 시스템 디코더를 거쳐 각각의 elementary stream으로 변환된다．
           이 elementa口 stream은 각 elementary stream 디코딩을 통해 원래의 오디
           오나 비디오신호로 재생된다. 이 과정에서 각 elementary stream의 재생
           (p肥sentaion）시 각 스트림간의 동기는 인코딩시 추가된 시간정보와, 디


                                                            Video     Decoded
                                                                           1
                                                            Decoder   Video



                               Channel        Program
                     Channel                                （그ock
                               spec小C         Stream
                                              demultiplex   contr아
                               decoder
                                              and decode



                                                            Audio     Decoded
                                                                           >
                                                            Decoder   Audio


                                    programs Stream
                                    containing
                                    audio and video
                                    elementary streams
                       羽        跆
                                  sbam으로부터 각각의 日en玘ntary sfream올 디코딩하는 ofi
                                            4. 트랜스포트 스트림과 프로그램 스트림



코더단의 클럭제어 과정을 통하여 맞추어지게 되며 또한 디코딩
                                            시의
버퍼제어도 적절히 수행되어 버퍼의 underflow -- overflow를 방지해
                                              주
거］ 된다．


.   프로그릴1 스트림과 트랜스포트 스트림간의 상흐변
                                                                        환

  PS stream과 TS stream간의 상호변환은 PES(Packetized
                                               Elementary
Stream) packet의 형태로 수행되는태 이 과정은 그림 午8과
                                              갇다. 즉 상

                                           Audio
                Audio         Audio        PES
    1中누


                                                         TS    TS
                Encoder       Packetizer
                                                               Stream
                                           Video
                Video         Video        PES          MUX.
    H
                Encoder       Packetizer



                                                   나＋
                                                         PS    PS
                                                               Stream


                                                        MUX.




          TS                    TS         Audio         PS    PS
          Stream                           PES                 Stream
           .4
                              RE           Video        DE
                                      {
                              MUX.         PES          MUX.



          PS                    PS         Aud幻          TS
                                                               TS
          Stream                           PES
           .4
                                                               Stream

                              RE           Video        DE
                                   <
                              MUX.         PES          MUX.

                    그림 小8. TS stream과 I冬 Sb毛am간의 상호변환
                               MPEG 시스템


                                          호변환시 PES I沼cket올 완전히 풀어서 elemental)' stream의 형태로 만든
                                          후 변환되는 것이 아니라 PES packet의 단위로 변환되는 것이다． 그림
                                          4-2의 시스템 인코더 블럭도에서 알 수 있듯이 audio packetizer 출력인
                                          audio PES packet와 video packetizer 출력인 video PES pa比et는 PS 入4UX
                                          로 입력되어 PS stream이 만들어지며, TSMUX로 입력되어 TS sbeaJn이
                                          만들어진다. 이와 같이 만들어진 PS stream이나 Th stream들은 각자의
                                          목적으로 이용될 수도 있고 상호변환하려는 경우에는 시스템 디코더，
                                          즉 PS stream DE_MUX나 TS stream DE_MUX롤 통하여 PBS stream을
                                          얻고, 이 PES stieam으로부터 다시 Is 5bealfl이나 PSsiream을 만들 수
                                          있으므로 결국 PES stream을 중심으로 상호변환을 할 수 있다. PSTFS
                                          packet의 header부분에는 스트림간의 상호변환시 필요한 정보나 표 등이
                                          있으므로 이를 참조하여 상호변환한다．


                                          .    프로그램 스트림과 트랜스포트 스트림의 비교

                                              lS stam은 그림 午9(a）와 갇이 일련의 TS packet으로 구성되는데 이
                                          TS packet의 길이는 항상 188by把로 동일하다. PS stream은 그림 午9(b）와



m
  發芬燾器韋燾艀專聽齬騷聯拍瀜難駐莪毖咎蟲巒i

                                          갇이 일련의 pack으로 구성되는데 pack의 길이는 일반적으로 가변적이
                                          고 보통 Is packet의 길이보다 훨씬 길다. Packet의 길이가 동일하면서
                                          鞏으면 다중화（m毗빠exing). 재다중화（re-mult빠exing) 및 역다중화
難難難難難
                                          (demultiplexing) 또는 수신기 제작등에 있어서 용이하고 Al入4에서 셀의
；可소；
   ：斗可：;:;:；好出；:；可F4:＋坪：·：·：

難難難難難聲雛娜難繫難蚤




心
發驪m繫聲難蝴聲懿器難旨難簪
                                               ( U loss）와 같은 전송 오차시의 손실이 적다는 장점이 있다. 특히
                                          이와 같은 경우에는 기존의 ATM 망과의 호환성이 보장되는데 188byte



I
                                          의 길이를 갖는 Is 恥cket이 4캐의 ATMce끄（53by1回로 변환되는 예는
                                          그림 午10과 갇다． 그림 午10은 188by把의 한 TS packet올 4개의 Al入4

如難醬難驪韆蠶
         m獅好m融烈難砥瀜드
                                          ce끄로 변환하는 과정인데 53byte의 A1爪4ceU 중 5by把의 header와 Iby妃
  難難小螂葬難雛算聲轟蛋

        驪黨難輦難難難難三                         AAL(ATM Ada磐翅切帥을 쓰는 경우 ' 1A1入4 cell의 유료부하
              吐고泌코吐；
                   모芒：:5釘모泌恥t和； 可소극


                                          payload) 길이닢47by把까 되므로 한 TS packet를 4개（4水7= 188）로 쪼개
           모巧꼬斗모斗모亡己모斗H小：口：
                          口：口뵤小：小：+:




      難難難蠶難



心
  器發爀毖熙難法滋滋難難群聲嚮；
                ．礪難滋
 難娑難難驪難難難難轟難難難難轟驀
                                          서 변환하는 亦淳l러나 PS 毗跏의 경우에는 pack h明tie：와 p玭k으
                                          로 구성되며 pack은 여러 개의 PBS 恥cket으로 구성될 수 있다． I뇨：k의
                                                                     4. 트랜스포트 스트림과 프로그램 스트림



        ,(   比ansport
                           packet> I transport packet   I transpo八 packet   ,   I transport packet
    1




                                                                                 1
                                                                        audio PES header
             video PES he口der二


        tr口nsport 力e口（ler
                                                          回




                                1 video PES packet                  : 』1 audio PES packet




         video ／기드S header                               audio／기모She口der                  video／万S 加a九r



                        pack header
                                                          向
                                                        (b)

                                그림 小9. TS stream과 PS stream의 구성 여］
                                             (a) '1'S stream       (b) PS stream

                                                                                                          中灣
유료부하에는 PES packet의 형태가 유지되므로 소프트웨어를 이용한 스
트림의 처리에 적합하고, 入4PEGI의 system multiplex/demultiplex 방식을
이용하는 시스템과 호환성이 있다．



0PES(Packetized Elementary Stream) 패

  TS snearn과 PSs甘earn은 PES packet으로부터 만들어지는데 이 PES
packet의 구성을 간단히 개념적으로 도시한 것이 그림 午11 이다. PBS
packet은 header와 유료부하로 구성되며 header에는 현재 packet의 유료
MPEG 시스템


                                                  transport packet length = 188bytes
                         (


                                                  184 packet bytes possible including optional
                                                  and conditional adaptation field elementants


                         HEADER

                             47by       / ad '
                      ,   中 -     - ' ] 47byte payload
                   >J IY把sAl加I packet {
              P{     1                        >                         47byte p口y勿口d
                     :                                              <                   >
                                                                                            47byte payload
                                                  (



               A




                                         -I
                                                               J

                               User a：二九（/ / b싸eAAL


                                       勺stem 口dded 5 勿伽 Am/ 加ader

             그림 小10. 188by也의 길이묠 갖는 TSpac蛇t이 4개의 ATI匹 cel［로 변환되는 （겨1




           부하에 있는 데이터의 특성 및 전체 스트림을 구성하는 데이터와의 관
           계를 나타내는 정보 및 시간정보 또 유료부하의 길이 정보등이 있다．
           이러한 header 정보는 결국 PES packet의 이식성을 좋게 하는데 header
           의 정보자체가 유료부하에 있는 데이터의 소속을 명확히 해주고 또한


                                    One PES Packet                             One PES Packet



                   header                     payload               header                  payload


                                                  그림 小11. PES Pa出et의 구성도
                                       4. 트랜스포트 스트림과 프로그램
                                                                        回
그 특성을 나타내 주므로 유료부하의 내용을 보지 않고도 header만을
이용하여 다른 스트림의 변환이나 재다중화통작등을 능률적으로 수행
할 수 있다．
  El印兀nta口 stream을 입력받아 전체적인 TS strean工 혹은 PS stream의
구성에 맞추어 적절히 PES header를 만들고 이 header의 내용과 부합하
도록 유료부하를 구성하여 packet을 만드는 과정을 수행하는 것이 PES
packetizer이다. Video PES packe血er는 video elen妃nta玎 stream을 입력받아
video PES packetS 만들고 audio PES packetizer는 audio elementary stream
올 받아 audio PES packet을 만든다．
  PES stream이란 일련의 PES packet을 의미하는데, 한 PES stream이란
같은 종류의 PES packet으로 구성 된다. 여기서 갇은 종류란 갇은
ID(Identifica由n）를 갖는 PES pack毗으로서 이 ID는 자신의 신분을 나타
 낸다고 볼 수 있으며 PES packet의 header 부분에 있다；   PES packet의
.header에 있는 ID를 stream ID라 하는데 이 ID는 결국 PES packet 유료
부하의 종류를 나타내는 것이 된다． 예를 들어 너deo elementaiy stream을
유료부하로 하는 PES packet으로 구성된 스트림은 미deo PES stream이라
하며 여기서 비디오가 하나의 ID를 나타낸다. 특별히 PES S仕earn이
ESCR(Elementaiy Stream Clock Rate) 및 ES_Rate(Elementaiy Steam Rate) 정
보를 header부분에 추가로 갖고 있는 경우에는 시스템 디코더나 재다중
화기에서 TS stream이나 PS stream과는 독립적으로 PES stream 자체만으
로 디코딩하거나 재다중화할 수 있다．
 위와 같이 구성된 PES packet은 TS packetizer(TS_MUX.）나 PS
packetizer(PSj爪IX.)로 입력되며 각각의 packetizer는 다시 TS packet, PS
packet을 만들게 된다. 이 과정에서 PES packet의 내용은 모두 TS나 PS
packet의 유료부하에 있게 된다. 결국 lS나 PS packet을 만드는 시스템
인코딩과정은 두 번의 패킷화과정을 거치게 되는데 TS stream 의 경우에
는 PES 패킷화과정과 l 's 패킷화과정을 거치게 되며 , PS stream의 경우
는 PES 패킷화과정과 PS 패킷화과정을 거치게 된다. 패킷화시 입력되
는 스트림은 모두 packet의 유료부하 부분에 입력되고 packet의 header
MPE(; 시스템



            부분에는 유료부하에 있는 데이터에 대한 정보 및 전체 스트림콰 관련
            된 정보들이 실리게 된다. PES packet header에는 유료부하에 있는
            elementaiy stream에 관한 정보가 있게 되고 TS나 PS 恥Cket header에는
            전체 스트림을 구성하는 프로그램 정보, 프로그램의 시간정보 및 전체
            sys也m을 제어하기 위한 제어정보등이 들어가게 된다. 위에서 기술한
            elementaiy stream으로부터 PES packet과 TS packet을 구성하는 스트림의
            형태를 종합적으로 나타내면 그림 午12와 같다. 마찬가지로 PS stream에
            서도 elementary stream으로부터 PES packet을 구성하고 난 후 그림 午9
            의 (b）와 같이 pack 유료부하에 PES pa昧et올 넣어 PS stream을 만든다．
            한 PES packet의 유료부하 부분에는 복수 개의 ac兀ess ui血이 있을 수 있


                Elementary Stream
                (Compressed audio, video, or PSI data)


                                                 \

                                      start code:




                 header :   payload   header :       payload   header :   payload


                     188 Bytes              188 Bytes              188 Bytes
                                                                               TS Packets

                            그림 中12. TS Siream융 만드는 전반적인 구성도
                               4. 트랜스포트 스트림과 프로그램 스트림



으며, 또 한 개의 access unit이 여러 개의 PES packet으로. 나뉘어져 들
어가기도 한다. 이 때 그림 牛12와 같이 PES packet 유료부하의 처음 시
작부분이 access unit의 처음 시작부분이 아닐 수 있다. 그러나 이것은
일반적인 구조이며 보통의 경우에는 access unit의 start code는 PES
packet 유료부하의      처 음에   들어 가는    것이    관례 이 다（6.1 절 의
data제帥ment_ indic欲or에서 설명）. 그러나 PES packet이 PSs甘因TI과 TS
stream의 유료부하에 들어가는 경우에는 PES packet의 처음 시작부분이
항상 pack(PS 앉ream의 경우）이나 packet(TS 5甘跏TI의 경우）의 유료부하
시작부터 들어가도록 해서 정렬（出ignment) 시켜줘야 한다．


.    타이밍 모델

    入WEG 시스템 파트에서는 시스템 신택스 및 그 의미를 기술하는 과
정에서 몇 가지의 가정을 두고 있는데 이러한 가정들은 실제의 시스템
과 다를 수가 있다. 그 중의 하나가 스트림의 흐름을 나타내는 시간의
문제인데 이에 관련하여 시스템 파트에서는 타이 밍（timing) 모델을 정의
하고 있다. 시스템에서 가정하는 시간은 항상 이상적인 모델을 바탕으
로 ' 하는데 하나의 프로그램을 구성하고 있는 각각의 elementa口 S甘earn
이 시스템 인코더에 입력되어 중간의 전송채널 또는 저장매체등을 거
친뒤 시스템 디코더에서 디코딩되고 재생되기까지의 지 연시간（처리시
간）은 각 elementaiy stream어］ 관계없이 모두 동일하다고 가정하는 것이
다. 이와 같은 치연시간에는 인코딩시간, 인코딩후의 버퍼링, 재다중화，
전송을 위한 시간 및 디코딩등에 소요되는 모든 시간이 포함된다. 이와
갇이 전체적인 지연시간（혹은 각각의 처리시간）을 일정하다고 간주하
는 이유는 어떤 균일한 원칙하에 시스템 인코더 및 디코더를 설명하끄
낸함인데 실제의 시스템 인코더 및 디코더를 설졔할 때는 각각의 처리
‘ 과정에서 발생할 수 있는 지연시간을 예측하여 이를 별도로 보상해 주
어야 한다. 마찬가지로 시스템 인코더 부분은 入4PEG에서 규정하는 대 』
로 스트림을 만들되 각각의 처리과정에서 시간을 기술하는 값들을 별
MPEG 시스템


           도로 꼐산해 줄 필요가 있다. 예를 들어 5장에서 다시 자세히 기술하겠
           지만， 꾀田m蟹텍쁘on Time Stan型）라는 시간型읖 디코더에서 디코딩된
           이erneataly s甘earn을 재생해야 하는 시간을 알려주는 값인데 이 1r田값을
           기준으로 실제의 지연을 맞추어야 한다. 만약 vrs값만을 그대로 이용
           ’하는 경우에는 재생시 음성과 화면의 내용이 서로 일치하지 않을 수가
           있다．
            시스템 부분에서 시간을 기술하는 방법으로 공통의 클럭을 이용하는
           더］ 이 클럭을 기준으로 각각의 원하는 시간을 상대적으로 표현하게 된
           다. 예를들어 이 클럭의 값이 100이고 prs의 값이 200이었다면 디코더
           에서는 클럭의 값이 200인 순간에 재생을 하면 되는 것이다. 이 과정은
           더 자세한 설명이 필요한데 5장에서 키술하기로 한다． 여기서 인코톺
           의 클럭을 기준 클럭佃佃帥：e cli乂k）이라고도 하는데 이는 다른 모든 시
           간이 이를 기준으로 기술되기 때문이다. 기준 클럭의 값은 시스템 인코
           더와 디코더단에서 언제든지 참고할 수 있어야 하므로 이를 위하여 인
           코더에서는 수시로 클럭값을 전송하고 디코더는 이 값을 참고로 클럭
           을 재생하며 이 기준값으로부터 기술된 다른 시간정보인 I可S나 DTS의
           값을 해석한다． 이 부분도 5장에서 다시 자세히 기술하기로 한다． 온디
           온나 비디오의 샘플링 클럭은 시스템의 기준 클럭과 배수관계를 갖도
           록 하는데 이러한 제한조건은 디코더 단에서 효율적인 클럭 추출（clock


                 TSor／咨                          AU五oorVith氾
                 Stream                          elementary stream
                                                       1
                                                       1
                                      BUFFER and       1
                                                               Elementary   Presentation
                                  卜   TS or PS         Y
                                                           >   Stream                 누

                                      Demultiplexer            Decoder




                     Rate             BUt十ER                    CLOCK
                     Controller       Monitoriong               Contr아


                     그림 小13. 채널 전송율을 제어할 수 있는 시스템의 구성도
                                           4. 트랜스포트 스트림과 프로그램 스트림



m（刃veiy）을 하기 위함이다．
 저장매체에 있는 TS 없ream이나 PS stream을 디코딩하려는 경우 만일
저장매체의 전송율을 디코더에서 조정할 때의 클럭 시스템은 그림 午
13과 같이 구성할 수 있다. 이 경우의 전송을 조정은 버퍼를 감시함으
로서 수행할 수 있다. 즉 디코더에서 버퍼가 overflow될 가능성이 있으
면 천송율을 줄이고 underfiow의 가능성이 있으면 전송율을 올리면 된
다. 따라서 전송채널을 조정할 수 있는 경우에는 버 퍼의 제어를 충분
히 할 수 있다. 클럭의 동기는 TS나 PS S甘earn을 역다중화（demultiplex-
ing）시킨 후 system clock의 데이터를 추출하여 행한다. 채널의 전송율
을 조정할 수 없는 경우（예 , 방송 수신기）에는 그림 4-14와 갇이 디코
더 시스템을 구성할 수 있다. 이 경우에 TSII冬 DEMUX로부터 추출된
클럭정보를 이용하여 클럭 추출과정을 수행한다. 이와 같은 클럭조정
은 디코더 버퍼를 제어하는 과정과 동일하게 간주할 수 있는데 이는
클럭의 조정이 디코더 버퍼의 underfiow나 overflow와 바로 연관되기
때문이다. 즉 디코더 클럭의 조정은 입력되는 데이터의 속도를 조절하
거］ 되므로 위와 같은 클럭조정이 재대로 수행되지 않으면 디코더버퍼
에서 underfiow L1- overflow가 발생하게 된다. 이렇게 데이터를 전송하면


       TS or PS                   Audio or Video
       Stream                     elementary stream


                  BUFFER and
                                       1        Elen妃ntary   Presentation




                                                   +
                  TS orPS                   )   Stream
    Channel       Demultiplexer                 Decoder




                                                              CLOCK
                  System Clock                                Generator
                  Parameters
                  Monitoring


                                                （그ock Rate
                                                Controller


          그림 小14. 채널 전송율을 저］어할 수 없는 시스템의 구성도
MPEG 시스템


                  서 클럭을 조정하고 버퍼의 제어를 하는 통작을 총칭해서 multiplex-
       . wide 아玘ration이라 한다．
                   여러개의 elementary stream으로 구성된 한 프로그램은 시스템 인코딩
                  과정을 거치면서 l 's stream이나 PS stream으로 표현된다. 이 과정에서
                  갈 elementary stream이 시스템 디코더에서 재생佃esentation）되어야 할 시
                  간을 나타내는 정보를 삽입하는데 이를 I끼田（F妃sentation Time Stamp）라
                  한다. Elementary stream 디코더를 통해 디코딩된 elementary stream들은
                  각각의 FF5를 갖고 있으므로 각각의 스트림에 대응하는 FF5어］ 맞게
                  재생佃resentation）하게 되면 모든 스트림간에 동기가 맞게 재생이 된다．
                  그러나 앞에서 설명했듯이 실제의 재생단위(presentation unit）들의 지연차
                  이가 있을 경우에는 이를 고려하여 동기를 맞추어야 한다．
                   yrS는 90k1也의 단위로 표현되고 전체 시스템의 기준시간을 나타내는
       伽R如얍跏
         ／
             Clock Refe肥.Ce: TS stream의 경우）과 西邸ys把m Clock
           ＼니뇨叫                                            !HHr!




                  匙如en此： PS stream의 경우）및 elementary stream의 시간을 나타내는
                       lementa口 Stream Ck兀k Referen氾）은 27卜41七의 단위로 표현되어
                  있다. 전체적인 시간의 동기는 각각의 스트림 재생시간을 동일한 시간
                  기준에 맞추어 표현하고 동시에 이 기준으로 디코더에서 재현함으로서
                  맞출 수 있다. FS stream이 복수 개의 프로그램으로 이루어진 경우에는
                  갉각의 프로그램이 각각의 PCR을 가질 수 있고， 서로 다른 시간기준
                  (time base）을 가칠 수 있다. 그때 단일 프로그램으로 이루어진 PS stream
                  에서의 SCR값은 항상 하나이다．


                  S 조건부 수신（conditional access)

                   권고안의 형식에 따르면 1'S stream과 PS stream의 송수신 시에 조건부
                  수신（허가받은 경우만 수신하는 제한된 통신）을 위한 암호화등이 가능
                  하도록 별도의 규정을 두고 있다. 그러나 이러한 통신은 응용분야에 따
                  라 다를 수 있으므로 조건부 수신을 위한 규정은 두고 있으나 자세한
                  방법은 기술하지 않고 있다．
                                     4. 트랜스포트 스트림과 프로그램 스트림



.    시스템 목표디코더 및 응용

    시스템 목표디코더（STh: System Target Decoder）는 System Reference
Decod아라고도 하는데 5장에서 자세히 기술할 것이지만 본 절에서는 간
단히 개요만을 기술하기로 한다. 1'S steam이나 PS snarn을 복호화하는
시스템 디코더는 응용분야 및 구현 과정에 따라 여러 가지의 형태가 있
을 수 있으나 퀀고안을 기술하는 과정에서 이상적인 시스템 디코더 모
델을 바탕으로 설명을 해야 천반적인 사항들에 대한 기준을 정할 수 있
거］ 된다. ISO/IEC 13818-1(MPEG그 system)에서 TS stream을 처리하는
Sys也m Target Decoder를 T-STD(Tran聊it stieam-S11가라 하는데 이 T-釘D
는 전체적인 시스템 디코딩 및 재다중화과정을 이상적인, 하지만 권고안
에서 필요한 조겊들을 71
             ［숲하71엔늪 충분한 기능블럭을 포할하고 있다．
    PS pack을 처리하는 System Target Dec月er를 P-STD(Pmgram Stieam-
STI가라 하는데 이 p-Sm도 T-STD와 마찬가지로 간략하면서 PS stieam
을 디코딩하는 과정을 기술하는데 충분한 블럭을 제시한다. 따라서 전
체적인 퀀고안의 틀을 만드는 과정에서 도입한 Sm는 응용목적에 따
라 실제로 구현하고자 하는 시스템 디코더와는 많이 다를 수도 있으나，


       For severe error rate              Computer, multimedia,
                                          MPEG-L MPEG-Il
       나＞188 Bytes 凡IPE（二／/               without transport l口yer.
       Transport Stream                   나＞ Interoperates 口t
                                          compression layer or use
                                          ATM




       via Ct功／elSatel／初e                  4:1 packet ratio

       ATV, HDTV, GA/MPEG-I!               B-ISDN/SONNKr
        transport stream                   ATMtr口n야刃rt 53 bytes
       for moderate error rate             low latency switching,
                                           勿w error r口把


                     그림 小15. 入iP耿花 시스템 스트림의 응용 분야
MPEG 시스템



           시스템 퀀고안을 이해하고 이에 맞게 시스템을 설계하는테는 개념적으
           로 중요한 부분이므로 이를 숙지해야 한다. 인코딩 시스템은 여러 가지
           의 구현가능한 방법이 있겠으나 결과의 출력 스트림은 Si]）어］ 맞게 만
           들어져야 하는데 , 이는 권고안을 기준으로 Si]）어］ 맞추어 설계한 디코
           더에서 디코딩할 수 있어야만 함을 의미한다．
            ISOfIEC 13818-1 의 광범위한 응용분야로서 그림 午巧와 같이 디지털
           저장매체（d坦it出 storage media) 및 컴퓨터 메모리에의 데이터 저장이나
           복원등을 생각할 수 있다．
                                      5. 시스템 목표디코더 모델




                      ’시스템
                  목표디코더 모델




 STD(Sys也m Target Decoder) 모델은 실제의 시스템에서 발생하는 지연과 같은 컷을 고려하
지 않은 개념적인 모델로서 스트림을 디코딩하는 과정에서 필요한 기능이［-F 변수들을 정확히 기
술하기 위한 이상적인 口코［크 모델이［:}.
MPEG 시스템




    卜                           -JII
                                / 11
                                       0
                                       =LJ




               본 장에서는 시스템 목표디코더（STD）에 대해서 설명한다. 이 시스템
           목표디코더는 入WEG 시스템파트를 이해하기 위해서 필수적으로 필요한
           개념으로 뒷장의 신택스부분과 밀접한 연관을 갖고 있다. PS stream을
           위한 시스템 목표디코더를 P-Sm但ogmm stream STD）라 하며 容sbealn
           을 위한 시스템 목표디코더를 T-S1D(fl鈿port stream S기D）라 하는데 이
           책에서는 편의상 T-STD, P-STI) 또는 Sm라고 표기하겠다. S띠2를 이해

           하기 위해서는프로그램에대한 정의，프로그램 구성정보多프
           Spec小c Information), 프로그램의 시간기준을 나타내는 但C묘但始ram
           Clock Reference) 및 시간값들에 대한 표현방법등의 이해가 필요하다． 따
           라서 이 장에서는 먼저 프로그램에 대해서 설명하고 T-STD 모델과 P-
           Si-I）모델을 설명한 후 시간값의 표현방법에 대해서 살펴보기로 한다．




    卜                        프 로 그 릴Ij



           .    프로그램의 정의

               시스템에서 언급하고 있는 프로그램이란 2장의 용어설명 부분에 있
           듯이 program element들의 집합인데 여기서 말하는 program element는 곧
           elementaiy S配am을 의미한다. Elementary stream이란 오디오 또는 비디오
           데이터가 入'IPEGi, MPEG2 등과 갇은 부호화방법으로 압축된 스트림을
                                           5. 시스템 목표디코더 모델


只］칭한다 I如gram eler配nt는 어떤 시간기준（山iie ba配）올 갖는데 이와 같
은 시간기준값은 하나의 프로그램을 구성하는 모든 pm胛m element에
 고
        方人 0
               는H갚희의으l 한다. 따라서 보편적으로 MPEG 시스템 파
트에서 말하는 ,                 일한 시간기준값을 갖는 elementary
stream들의 집합이라고 말할 수 있다. 만일 pmgram element가 프로그램
이고 0] 복수 개의 프로그램들이 모여 또 하나의 스트림을 구성하면서
동일한 시간기준값을 갖는다면 이것도 하나의 프로그램이 되는 것이다．
그런떼1 이와 같이 프로그램이 공통의 시간기준（time base）을 갖는
pmgram element들의 모임이라는 고정된 관념을 고수하면서 시스템 퀀
고안을 본다면 때에 따라 이해하는데 어려운 부분이 있다. 프로그램은
TS stream 또는 PSstieam의 형태로 패킷화되어 송수신되는데 중간 과
정인 패킷화된 프로그램의 형태도 프로그램이라 말하는 경우가 있다．
 그림 5-1(a）는 하나의 elementary stream이 하나의 프로그램을 구성하는
예이며 그림 5-1(b）는 두 개의 elementary stre可n（오디오와 비디오）이 하
나의 프로그램을 구성하는 예이다. 전자의 경우는 라디오를 예로 들 수
있으며, 후자의 경우는 텔레비젼을 예로 들 수 있다. 이와 같은 경우에
오디오 또는 비디오 신호가 인코더를 거쳐 압축되면서 elementary stream
이 되고 이 elementa口 stream에 대한 PES 패킷화수행시但SCR乍e毗ntary

StreamClock Rereren的및（三I蜘帥don Time S帥p), 區企如
Time Stamp）를 PES packet header부분에 추가할 수 있다． PES packet
header에 추가되는 ESCR/FS月끄'S에 대한 각 시간값의 의미는 뒤에서
다시 자세히 기술하기로 한다. 이와 같은 ESCR/VfS           는 디코더나 역
다중화기（demul却lexer）에서 특별한 목적에 이용되는데 여기서 중요한
것은 각 값들이 동일한 클럭을 기준으로 표현된다는 것이다. 즉
ESCRIPTS/I끄'S가 나타내는 값들은 동일한 시간기준값으로서 인코더의
system clock을 7］준으로 표현된 것 '］다·
                              흐y些뜨으甦是씻슨甦보콘틔
                                              0
가 프로그램을 만들 때 쓰는 기준클럭이며, 디코더0         럭도 (> 기준클

현斗卑쁘브 ' 乍한다" ］와 갇은 동'］를 多횃 電垂）' ]'］는 그．프로
구랩의 푠型如帥 Clock Refem"떠 또는쁘 陟'把m Clock Refere"此）값
MPEG 시스템


                                       elementary                        PES
                                                                                                   親
                                       釘re口刃i                            packet


                                                                                                             1


              source          Elementary                PES                       TS/PS
                              Stream
                                                                                               -    -




              缸gnal                                     Packetizer                Packetizer       Program
                              Encoder



                                                 ESC가）TS/DTS
                                                                   t
                                                                    1                    PCR/SCR

                                                                                       二和 이苞 小吃
                                                            CLOCK

                                                             (a)
              audio
              signal      Audio                Aud沁 PES                   PES
                          Encoder              Packetizer                 packets
                                                    1
                                                        1
                                           ESC가）TS/DTS
                                                                         H
                                                                                  TS/1咨            program
                        elementary =            CLOCK                                                   >
                        針re口m                                                     Packetizer


                                           ESCR가）TS/DTS                       PCR/SCR


              video
              signal      Video                Video PES                  PES                      TS/PS
                                           >
                          Encoder              Packetizer                 p口ckets                  計re口m
                m나
                                                                   (b)

                     그림 5-1   工쿠＝램의 기준시간 구성
                              (a) 寸ng으 el丑I比n切rysti毛am으로 구성되는 J工쿠 口램
                              (b) audio/vidm ei江nenataly sti七am으로 구성되는 立쿠 -1램




           을 TS packet header와 PS packet header부분에 각각 기록하게 된다. 다시
           말하면 I 'S stmam에서는 시간기준값을 PCR로 표시하며 PS stream에서
           는 SCR로 표시하는 것이다. 그러나 여러 개의 프로그램들이 모여 하나
           의 1'S stream을 구성하는 경우에 각 프로그램의 PCR값들은 다를 수가
           있지만 되도록이면 각 PCR값들이 동일한 기준을 갖고 기술되는 것이
                                                     5. 시스템 목표디코더 모델


바람직하다. 일반적으로 TS strewn은 복수 개의 프로그램으로 구성될
수 있고 PS stream은 단일 프로그램으로만 구성된다. 다시말하나1 PS
stream은 단순한 시스템 코딩의 한 방법이지만 그 용어가 의미하듯이
하나의 프로그램을 저장하기 위해서 포장한다는 의미가 담겨 있다．


S 프로그램 구성정보

 프로그램 구성정보（P鋤어］ 대한 신택스 부분은 7장에서 자세히 기술
될 것이지만 본 절에서는 다음 절에서 설명할 다중화（numti미exing) 및
역다중화（demultiplexing) 부분과 관련하여 몇 가지 중요한 개념을 전반적
으로 정리하기로 한다. PSI정보는t시스템 디코더가 TS stream 亘［에，오A는
프로그램을 디코딩할 수 있도록 사용자가 점읠型주는 프로그램，정보들
을 지칭한다. PSI정보는 다음과 갇은 4개의 정보를 포함할 수 있는데
이를 테이블로서 구분하여 표현하므로 PSI정보는 4개의 테이블로 구성
된다고 볼 수 있다. 4개의 테이볼은 PAT(Pn鉀n Association Table), I小if
(Pro留am Map Table), . N1T(N苡Work Informalion Table) 및 CAT(Condi如nal
Access Table）이다. 각 테이블의 이름에서 알 수 있듯이 PAT와 I爪IF는
프로그램을 구성하고 있는 program element들에 관한 정보들이고 N口는
전송네트워크에 대한 규정값들에 해당한다. 또 CAT는 조건부 수신
(conditional access）이 필요한 경우 스크램블링 혹은 사적인 스트림（priva把
sbem)에 관련된 것이다．
 PAT와 I小if에서는 어떤 패킷이 어떤 I기D를 갖고 있는가 하는 정보
를 보내주는데 PID는 'IS packet header어］ 있는 패킷 ID를 말한다. 이
PID는 TS packet의 소속을 나타내주고 있기 때문에 역다중화（demul-
ti미炚ing）하는 과정에서는 이 P11）만을 보고 패킷들을 구분하게 되는 것
이다. 한 TS stream어］ 여러 개의 프로그램을 시분할 형태로 전송할 수
도 있고，감 프로그램은 복수 개의 elementa玎 stre缸n들을 포함할 수도
있다. 또한 전송중에 한 프로그램이 다른 프로그램으로 대치되거나 삭
제될 수도 있고 프로그램 내의 elementary s配am의 구성이 달라질 수도
있다. 이와 갇은 과정에서 디코더는 가능한 빠른 시간 내에 달라진 정
MPEG 시스템



           보를 받을 수 있어 ' 乍 하는"]] "］를 위해서트只정보를 일정한 시간간
           격으로 전송해 ' 乍 한다· MPEG에 ' ］는 최대한딴多 "］내에 飴I정보를 전
           솜해야 한다고 규정하고 있다． 따라서 시스템 디코더는 0.7초 이내에
           프로그램 구성정보를 받아볼 수 있고 이를 이용하여 모든 program
           el이nent들의 PID를 알 수 있으므로 원하는 처리의 초기 동작을 진행할
           수 있다. 여기서 말하는 초기 동작이란 현재 수신하고 있는 Th packet
           이 어떤 데이터인지를 아는 것으로부터 시작하여 적절한 다음 동작을
           수행하는 것을 의 "
                        ］한다·                   4놔e            小
            그림 5-2의 TS packet header부분에 있는 PD는 32日］트의 header중（므)
           비트를 차지하는데 이 값은 자기 패킷이 어떤 소속인지를 알려준다. 그
           림의 예는 PD값이 xx, xy인 두 IS packet올 나타내고 있는데, 예를 들
           어 xx의 PD값을 갖는 꽤킷을 오디오 패킷, xy의 PD값을 갖는 패킷올
           비디오 패킷이라고 하면 시스템 디코더는 Pu）값을 해독하여 PID71- xx '
           인 패킷은 audio TS stream bu什er에， PD가 xy인 패킷은 video 'IS stream
           bu甘er에 각각 넘겨주게 된다 ．이 와 같이 어떤 P11）값이 오디오이고 ，어
                                                                                            이
           甲 PD값이 비디오O］가 하누 것퉁은 PSI정보에 "포함되어 있는뎨，
           ! SI 정보는 톡수한 낀D값을 갖는 姪附et에서 천총뇐다．
                                  ] 0 '」］ 1'S .acket은 PAT . 보를 7 고               ｝二
                                                                                      7-1

           처음부터 규정을 하고 있다. 따라서 시스템 디코더는 시스템을 켰을 때
           P11）값이 0인 TS packet만을 찾으려고 한다. 'I'S str曲m은 일반적으로 복
           수 개의 프로그램을 다중화（mu!印lexing）하여 구성할 수 있는데，
                                                 ．쁘r셴1
           는 현재 전송되고 있는 1'S stream이 어떤 프로그램들로 구성되어 있는


                         188 bytes                     188 bytes
                         transport stre口刃I             transpo月 stre口刃i

                                     侍A1tjte
                    勉듬 4      <     payload        header
                                                            卜＜
                                                                     payload



                    P11) 工X
                               工1
                                                   PID xy        -ty
                               elementary stream                 elementary stream



                         그림 5口. 玉an町x才tsbam에서 꾀［I) 및 유료부하
                                              5. 시스템 목표디코더 모델


지를 나타내는 프로그램 번호와 이에 해당하는 PD를 갖고 있다. 여기
서 프로그램 번호와 함께 전송되는 PD는 program map P11) 또는 PMT-
PD라고 하는테 프로그램 번호 10의 I爪if-P1D7f 100, 프로그램 번호 20
의 I呱4T-PID가 200이었다면, 현재 수신되고 있는 TS stream은 2개의 프
로그램으로 구성되어 있으며, 프로그램 번호 10으로 명명한 프로그램의
I水4T는 Pu）값이 100인 TS packet으로 전송되고 있는 것이고 프로그램
번호 20에 해당하는 프로그램의 PMT는 Pm가 200인 TS packet으로 전．
송되는 것을 나타내준다. 이 관계를 그림으로 도시한 것이 그림 5-3(a)
이다．
 外'IT(Progam Ma+ Table）은 한 프로그램에 포함되어 있는 elementary
和ealn들에 대한 내용 및 PD를 나타내는데 이 PMT정보는 PAT에서 지
켰한 PMT_PID를 PD로 갖는 TS packet으로 전송된다． 그림 5-3(b）는 그
림 5-3(a）에서 PAT가 나타내는 I水4T_PID에 따라 I爪if가 구성되는 것을
도시한 것이다. 프로그램 10에 대한 PMT에서는 audio elementa口 stream
의 PD가 101, video elementa口 stream의 PID7} 102라고 알려주므로 프로
그램 10은 오디오 l 개와 비디오 I 개의 pm留am elem印t들로 구성되어
있음을 알 수 있다. 따라서 PD값을 이용하여 프로그램 10을 구성하는
모든 TS packet을 찾을 수 있게 된다. 마찬가지로 프로그램 20은 3개의
elementary stream, 즉 2개의 audio 이ementary stream과 1개의 video
elementary stream으로 구성된다. 여기서 프로그램 번호는 구체적으로 방
송국에서의 한 채널을 의미할 수도 있고 아니면 같은 채널이라도 방송
프로에 각각 다른 프로그램 번호를 할당할 수도 있다. 수신단에서 미리
어떤 프로그램 번호가 어떤 채널인가를 알고 있으면 되므로 프로그램
번호값은 그리 중요하지 않다. 즉, 예를 들어 기존의 TV채널에서 채널
번호 9는 KBS-1 을 의미하는데 이는 이미 시스템 디코더에서 알고 있는
값인 것이다. 그림 三3(b）에서 프로그램 번호가 20인 프로그램이 어떤
케이블 TV 방송에서 영화채널로 할당된 것이라면 시스템 디코더는 이
프로그램의 PMT_PII）를 찾는데, P八if의 PD가 200이므로 TS packet의
PD값이 200인 패킷을 찾아 영화 프로그램을 구성하는 모든 elememtary
stream들의 PD를 찾아 디코딩할 준비를 한다. 오디오가 음성다중인 경
MPEG 시스템



           우에는 하나의 video elementaiy stream과 두 개의 audio elementaiy strewn
           이 필요한데 그림 5-3(b）는 aud的그 stream의 PID가 201, audio_2 stream의
           PID 71- 202, video stream의 PID가 203임을 나타내주고 있다. 각각의 경우
           에 TS pa疎et의 구성을 그림 5－카C）에 도시하였다．
            MT(Network Information Table）는 전송에 관련된 파라메터를 나타내주
           늠 값으로서 I크）M(Frequ口lcy Divi駐onMul印lex血g）의 경우에는 주파수나，
       ．트랜스포트 번호 등에 관련된 데이터를 예로 들 수 있는데 이와 같은



                                                                                 program nwnber        :10
                                                                                  ／기才T_ PID            :100
                                                                                 progr口m num方er        :20
                                                                                  PMT_ PID             :200      1


                                                       188 bytes
                                                       tr口7工SI刃rt stream


                                                  header   +           payl
                                                                                 oad


                                                             progr口m ft口nbers
                                                 PID 0
                                                             program PMT-PIDs

                                                             (a)
                                  188 bytes                                       188 bytes
                                  tr口n叩ort strea刃i                                tr口nsportst肥am


                      header              I        payload                     header
                                                                                         )
                                                                                                  payload
                                      꺼   ＜



                                              PMTof                                          PMT of
                     PID 100                                                  PID 200
                                              program number 10                              program number 20



                                                  I
                                                                                                  1


                                                      4切叱 耐旽                                      1

                                                                                                  1

                                                           두r＼앉씨 告毛                               1




                    I끄） 100인 tran斗X꾜t j月
                                       （火et                            尸ll             인 tran啄x끄tpacket
                    의 m yk坦d에1 있는 내용                                   의 .1石yl(石d에1 있는 내용



                               audio st肥am PH갸101                             口udio_1 stream小尸／I가201
                               video stre口m PID:102                           audio 2 缸ream끼I갸202
                                                                   d          video stre口刃i 尸／D :203
                                                                   佃
                                                                                                           5. 시스템 목표디코더 모델


                         188 bytes                                            188 bytes
                         transport stream                                     tr｛가is／기7rt strea刃l


                  he
                       ader   +            payl
                                                  oad                header
                                                                                                 p
                                                                                                     a
                                                                                                         yload   >




                              口udio ele刃ientary                                      바deo element口ry
        PID 101                                                PID 102
                              sire口m ofprogr口m /(/                                   stream ofprogram 16




                         188 bytes                                            188 bytes
                         tr口ns工wrt stre（가n                                    transport stream


         header
                              +     payl
                                                  oad
                                                                header
                                                                                  44       payload
                              audit乙／element口ry                                     口udio 2 element口rv
                                                               尸ID 202
                              釘re口m ofprogr口m26                                     stream ofprogram 26




                                                   188 bytes
                                                   transport 計re口刃i


                                           header


                                                        video elementary
                                   PID 201
                                                        釘re口m ofprogr口m 20


                                                         (c)
    그림 5-3. TS strea了n에서 1冬1정보와 I皿）및 ml用&et 유료부方｝ 내용
                       (a) PlC = 0인 TS packet의 내용（Program A爵뇌ation Tab뇨）
                       (b) I기［C = PMT__PID인 1-SI坦dcet의 내용（Program Map Table)
                       (c) I기D = elen祀ntary sti毛amPID인 1-SI俎（出：et의 내용




데이터를 포함（전송）하는 패킷의 P11）는 PAT에서 알려주게 된다. PAT에
서 프로그램 번호가 0인 PMT_PII）는 NiT_P끄）를 나타낸다. 따라서 PAT
에서 프로그램 번호가 0인 PMT.YID가 있었다면 이 P11）를 갖는 TS
packet는 I江1'정보를 갖고 있는 것이다．



                                                                                                                        55m吼뇨小二社까：
                                                                                                                     驪難難驪難蠱難難鱗
                                                                                                                     批難難難驩難驪難難箋
MPEG 시스템


            CAT(condiuonal Access Table）은 PID가 1로서 이미 결정되어 있으므로
           PID가 1 인 패킷에는 조건부 수신（conditional access）의 정보가 있다. 스트
           림이 스크램블링된 경우의 프로그램에서는 CA_descr地tor(conditional
           access descriptor)에서 관련 정보를 보내는데 , 이는 9장에서 다시 언급하
           기로 한다．


           .psI 관련 시스템 다중화

            TS stream은 여러 개의 프로그램을 시분할 형태로 전송할 수도 있으
           며 각각의 프로그램은 복수 개의 elementa口 stream들을 포함할 수도 있
           다. 또한 전송중에 한 프로그램이 다른 프로그램으로 대치되거나 삭제
           될 수도 있고 이e毗ntary stream의 구성이 중간 단계의 재다중화
           (remu川plexing）과정에서 달라질 수도 있다. 이러한 모든 과정을 시스템
           다중화라 할 때 TS stream의 구성정보를 나타내는 PSI정보는 시스템 다
           중화과정에서 첨가되거나 수정되는데 이 과정을 예를 들면서 설명하기
           로 한다. 대표적으로 시스템 다중화는 그림 5-4와 갇이 PES stream 단
           겨］, 단일 프로그램 TS stream 및 멀티 프로그램 TS stream 단계로 구성
           될 수 있으며, 그림 5-5는 3개의 프로그램으로 구성되는 TS stream의
           예를 도시하였다. 그림 5-4에서와 같이 PES stream 단게에서는 어떤 프
           룬그램에 관련된 모든 pmgrarn element, 즉 elementa玎stream들의 PID값올
           할당하고 단일 프로그램 TSstream 단계에서는 그 프로그램의 PMT_PID
           를 결정한다. 그림 5-4의 예는 5개의 elementa口 stream으로 구성되는 영
           웅본색이라는 프로그램이 프로그램 번호 1로 지정되면서 이 프로그램
           어］ 대한 外'IT_PID는 l（刃으로 할당된 예이다. 따라서 5개 elementa玎
           stream들의 PD들은 PH) 100인 패킷으로 전송되는데 이 때 PAT에는 프
           로그램 번호 1의 I爪4T_PID= 1(刃이라는 정보가 기록될 것이며브旦엔늪
           5개의 elementary stream들의 streamjD（毗am이 어떤 형태의 stream인지
           룔 나타내는 정보）왕 TS packet PD를 기록흐｝게 된다． 갇은 방법으로
           프로그램 번호 2인 마치막 황제, 프로그램 번호 3인 셜록홈즈 프로그
           램도 각각 단일 프로그램 TSstream의 단계를 거치게 된다. 이 3개의
                                                              5. 시스템 목표디코더 모델



      Packetized                 Single Progam        Multi Program
      elementary                 Transport            Transport
      Stream                     Stream               Stream


    video 1 (PID:101)
         audio 1 (PID:102)
             audio 2 (PID:103)




            auxiliary data (PID:104)
                                                   r_ L
        closed caption (PIDP105)                     nrnc'r그m    I
    elementary stream map (PID: 100)                 association 1
                                                   : k功／e pi/／刃 1.




                                                 program number I       :
                                                 ( 영 웅 본 색 =:
                                                 program map pid: 100

                                                 program number 2
                                                 ( 마지 막 황 제 )
                                                 progr帥1 map pii蚣00

                                                 program number 3
                                                 ( 셀 록 홈 즈 )

                                                 prog"跏map p嶝巴

  그림 5-4. 3 개의 program으로 구성된 transport stream의              system level
          multiplexing 과정 및 PSI 정보



프로그램이 하나의 TSs甘earn으로 다중화되는 과정에서 처음에 있었던
PAT에 프로그램 번호와 이 프로그램 번호에 해당하는 PMT_PII）의 정
보가 차례로 기록되면서 PAT는 그림 5-5의 P11）가 0인 패킷의 내용과
같이 구성되는 것이다. 물론 이 과정에서 각 프로그램의 PMT는 그림
    MPEG 시스템


               5-5의 P11느 100. PID= 200. PID= 300의 패킷 내용과 같이 구성되고 이
               과정을 모두 마치면 TS packet의 구성이 그림 5-5의 아래 부분에 도시
               한 TS packet고｝ 갇이 된다. 이와 갇이 구성된 멀티 프로그램 Th stream


                                   PID 0

                                        영 웅 본 색            (pro얍叩1 number 1 ; 1呱4T_PID=100)
                                        마지 막 황제 (program number 2 ; PMT_PII뇨200)
                              4 · 셀 록 홈 즈 (program number 3 ; P｝뇨4T_PII뇨300)




                                                                               PID 300


                                                                                                                          m 聊
                                                                                elementary stream

                                                                                        너deo 1
                                                          Pm 200
                                                            elementary stream                   PID                      302

                                                                   .videol                      201
                                    PID 100
                                        elementary stream                PID                    202

                                    -             video I                101
                                        -         audio 1                102
                                                . audio 2                103
                                                · auxiliary data         104
                                                , closed caption         105




                      ：尸／ij                 尸／/j audio / :P/ij audio 2         ancil1ar iPIL
                                                                                                          1PID   video
                      :101:   ：烈
                                            102! sIre口In :10카 sIre口m           data     !105!    畿：   .    201   stream   /
                                                                                            :

                      header payload
                                            1                                           1

                       188加tes                                                          188 bytes
                       tr口n卑k刃1packet                                                   tr口'a叩0月packet

                                                                                                                                뗘
                  그림 5小. 그림 2- 4에서의 PAT 내용． 각 program의 I呱rr정보 및 program
                         대한 b ar心1拉tst七am 내용




蠶蠶蠶蠶蠶蠶難難醫
                                         5, 시스템 목표디코더 모델


은 최종 프로그램 수혜자에게 직접 전송될 수도 있고 재다중화기에 연
결되어 또 다른 멀티 프로그램 TSstream을 만들 수 있다. 또 다른 프
로그램을 추가하거나 일부의 프로그램을 삭제하는 경우에는 해당되는
프로그램 번호와 I呱4T_Pll）를 PAT에서 추가하거나 삭제하면 되는 것이
다. 그림 5-4와 같이 구성된 멀티 프로그램 TS stream의 PSI가 그림 5-5
와 같이 구성되어 있지만 만일 이 멀티 프로그램 TS 없ream이 다른 다
중화기로 넘어가서 다른 TS stream과 혼합되어 다른 형태의 멀티 프로
그램 Th strea工n을 구성하는 경우 처음에 만들어진 PAT의 내용이 완전
히 바뀔 수 있다. 즉 프로그램 번호 1의 영웅본색이라는 프로그램이
PMT PD = 1（刃으로 되어 있었지만 다른 TS stream으로 바뀐 경우의
PAT에는 프로그램 번호 11어］ I爪'iT_Pil느 1100일 수 있는 것이다. 7장의
PSI 신택스 부분에서 PAT와 I爪'iT의 자세한 내용이 다시 언급된다．


.    PSI 관련 시스템 역다중화

    PSI와 관련하여 시스템 역다중화하는 과정을 앞에서 설명한 3개 프
로그램 四 stream의 PSI정보를 예로 들어 그림 5-6어］ 도시하였다. 그림
5-6에서는 四 stream을 입력으로 하여 PSI를 추출하고 이를 이용하여
프로그램 번호 1 의 영웅본색 프로그램을 역다중화하고 나머지는 다른
시스템으로 전달해주는 과정을 도시하고 있다. TS stream이 입력되면
P표）7f 0인 TS packet을 찾는데 이는 현재의 수신되는 TS stream이 어떤
프로그램들로 구성되어 있는지를 나타내는 PAT를 찾는 과정에 해당한
다. 시스템 디코더에서 프로그램 번호 1의 프로그램을 수신하고자 했다
면 PAT에서 이에 해당하는 마'iT의 PD7f 100임을 확인하고 두 번째의
였다중화단에서 O] 패킷을 찾아 프로그램 번호 1의 프로그램이 어떤
program element들로 구성되어 있는지를 확인하고 각각의 program
elen妃nt들에 대한 elementaiy stream P11)를 찾는다． 위의 과청이 완료되면   ！重重i
프로그램 번호 1에 해당하는 PD는 100의 PMT_PII）를 포함하여 101,
102, 103, 104, 105임을 알 수 있으므로 최종단의 역다중화에서 각각의
P11）를 갖는 TS packet을 프로그램 l 디코더에 넘겨주고 나머지 패킷은
MPEG 시스템



                             nulti-program
                           transport stream                   I PID =
                                                              1 101, 102,
                                                              : 103. 104.
                                                              1 105?


                                                         demux     !
                                                                  十 elementary
                                                                    tr口ns／色r 口／/

                                                                        計re口刃11）口cke打
                                                                        to the decoder
                                                                        ofprogram 1

                                                                        dump
                                                                        unselected
                                                                        packets to
                                       尸MT PID = /｛刃    elemental)'
                                                        計re口mPH乃        other玎釘em




                  obtain PMT PIDs

                      . program 1 : PID= 100
                      . program 2 : PID =M0
                      . program 3 : PID = 犯0




                   program number: 1
                                                       .video 1 : PID = 101
                    ( 영 웅 본 색 )                        .audio 1 : PID = 102
                                                       .audio 2 : PID = 103
                                                       .closed ...    ...

                   program selection


             그림 5-6. Demultiplexer/decoder C거1 서 의     PSI정 보    추출과정 과          program
                     demulfiplexing or日出이l



           다른 시스템으로 넘겨주게 되는 것이다. 위의 과정이 지나면 단일 프로
           그램 TS stream(프로그램 번호 1만을 포함하는 1                             suml)이 선택되어
           TS stream 디코더에 전달된다. 이후에 프로그램 1 의 四 sneam이 어떤
           과정올 통하여 디코딩되는지는 다음 절의 T-STD에서 설명한다．
                                                                                               5. 시스템 목표디코더 모델




卜 1
                          1-   ST. 모」및동작

      下STD 구성과 관련용어

   T-STDFran莎月t 없肥am Sys妃mT뇨get Decoder）는 시스템 인코더에서 TS
없始am을 만드는 경우나 혹은 시스템 디코더에서 TS sUeam의 디코딩
과청에 있어서 관련된 용어를 정확히 기술하기 위한 개념적인 모델로
서 블럭도는 그림 5-7과 같다. T-STD는 단순히 이론적인 개념을 기술
하기 위한 모델이므로 실제의 시스템 인코더나 디코더와는 다르지만
MPEG 시스템 파트에서 설명하는 용어를 이해하기 위하여 완벽히 이해
할 필요가 있다. T-STI）와 관련된 용어 및 표기법은 다음과 같다．

i,i ',i "      TS steam상에서 특정한 by妃들을 지칭하는 인텍스佃dex）이다．
               맨처음 by妃의 인덱스는 0이고 0번째 by把라고 말한다．


            卜th by妃 可
            Transport Stream

                                   Rxi          Rbxi       Ai(j)              Video
                                                           td'(j)                              入J뜨目
                                                                                          oi
                                                                    \,
                                                                                               ,\       tpi(k)


                                                           /
                               l         MBi       EB,
                                                            十 二／

                                           j-th access unit              k-th presentation unit
                                                                                                    /
                   O O
                      O


                               TBn
                                         Rx11
                                                       氏   喆                                   P (k)
                                                                                               tpn(k)


                                         RXSyS
                                   B
                                                                         立＞           Systein control
                                                           由   耐
                그림 卜7. 끄-an司a才-t stream system target decoder in｛넜el의 붑럭도


                                                                                吼
   dE小毛，,h'弓 eh幽" " :                       ;, ktk1 k") I

    tC        弘4氏 :            i (t( ,(tt)
MPEG 시스템



           j        Elemantary stream에서 J번째 access ut血올 나타내는 인덱스
           k,k'小" Elemenary stream에서 k, k', k" 번째 .presentation unit을 나타내는
                     인덱스
               n
                    n번째 elemantaiy stream올 나타내는 인덱스

               P的
                     TS stream에서 p번째 TS packet을 나타내는 인덱스
                     TSstream 중 i번째 by把가 T-S기）에 입력되는 시간으로서 단위
                    는 초（second）이다. t(0）는 첫번째 1乃te가 입력되는 시간인데 디
                    코더는 임의의 시간에 동작할 수 있으므로 이는 임의의 상수
                     값을 갖는다．
           PCR(i)   i번째 byte에 대한 PCR값으로서 i는 PCR 필드중 base 필드
                    (program_cl（乂k_reference_base) 마지막 번째 by把를 가리킨다. 따
                    라서4PCR(i)는 PCR base 필드의 마지막 by把가 T-STI）에 입력

               m     되는 시점을 2呱표-Jz의 클럭단위로 표현한 것이다．
               凡                                                        O
                    n번째 , elemantaiy stream에서 J번째 ac（允ss UI血를 나타낸다．
                    순서는 디코딩되는 순서에 따라 인덱스가 부여된다．
           tdn(j)   n번째 elen妃nta玎 stream에서 J번째 ac（戈ss unit이 Sm텍서 디코＋
                    뭅되늪시가을 나타낸다．
                    n번째 elementary stream에서 k번째 口esentation w血에 해당한다．
                    已(k）는 凡(j)을 디코딩한 결과이며, 이 인덱스 순서는 재생
                    (p忙sentation）되는 순서로 한다．
           印뀨c)     n번째 ele毗ntary stream어］서 k번째 presenata丘Ofl UI血이 STI刈
                    서 재생佃esentat幻n）되는 시긴佃cond）올 의미한다．
                    초（second) 단위의 시간
           F (t)    t의 시점에서 可번째 elementary stream어］ 대하여 sm 입력버퍼
                    위 충족도（ii괴ness）를 byte 단위로 나타낸 것이다．
           B.       , n번째 ele毗ntary stream의 main bu卄町를 나타낸다． 이 main
                    bu什er는 au小o elementary stream에 대해서만 있다．
               Sn
           ,BSn
           1
               B    by把 단위로 표현된 民의 크기          ．.
       . 玎           m에서 시스템 정보를 위한 main bu卄er혀m하r당한다． 여기서
                                                           5. 시스템 목표디코더 모델


              시스템 정보란 현재 디코딩되고 있는 이ementa口 stream을 포함
              한 프로그램 정보를 의미한다．
      BSSyS   byte 단위로 표현된 艮邪의 크기
      MBn     n번짜르lernentaiy s먀am에 대한 multiplexjiig bu什er를 므旦낸단；
              이 bu珏er는 video elementaiy sti七alll의 경우에만 존재한다．
              byte 단위로 표현된 入'lB, 의 크기
              n번째 elementaiy stream어］ 대한 elemen切rystieambu丘er를 나타
              낸다· 이 b너Ter는 video elementa玎 stream의 경우에만 존재한다．
  EBS.        byte 단위로 표현된 EB, 의 크기
      m9y8    현재 디코딩되고 있는 프로그램에 대한 시스템 정보를 갖고
              있는 TS packet들을 저장하기 위한侮nsport bu且er
      TBS돠S   by把 단위로 표현된 1且y, bu什er의 크기
1瓦            n번째 elementaiy stream어］ 대한 岫nsport buffer
  TBS.        byte 단위로 표현된 TB, 의 크기
D玎5           n번째，
                 PSsiream의 시스템 정보를 디코딩하기 위한 디코더
1\            n번째 elementa口 stream의 디코더
on
              n번째 video elementa口 stream어］ 대한 reorder bu什er
R町S
              民d世卄er로부터 출력되는 datai趾e
Rxn           TBnb咐町로부터 출력되는 data rate
Rb\ 匹勇廂亘4용誰’경；l 쿄，으로부터 PES pack姻 유료
              부하가 출력되는 thtara把． 이는 너deo elementary stream의 경우

H             少만존재更다·
Rbx (j) 딴브艸多퓜을 이용하는 경우 MB.으로부터 PES packet의
              유료부하가 출력되는 data ra妃. 이는 video elementa玎 stream의
              경우에만 존재한다．
F氓ys          TB邸로부터 시스템 데이터가 추출되는 data rate
R1冬           video elementary stream의 sequence header어] 있는 video elemen-

              쁘蜘의匹才
MPEG 시스템



           1T-STD의 입력시간

            T-STI) 모델에서는 1'S steam이 T-STJ）에 입력되는 상황을 설명하기 위
           해서 화번에 하나의 프로그램만을 디코딩하｝二 것을 기본 가정으로 한
           다. 따라서 T-STJ）에 관련하여 기술되는 모든 시간변수는 하나의 동일
                                        k을 기준으로 하는데 MPEG2에
           한 시간기준（time base）값, 즉 sys把m 面：

           서의自些쯔스쁘쓰쓰吐끄坦垂이다· 이와 같은 시간기준값을 디
           코더에 알려주기 위하여 PCR을 전송하는데 이는 시간을 sys把m clock
           fraquency로 샘플링한 값이다. PCR은 MPEG1과의 호환성을 고려해서
           PCRJ瑯e 필드와 PCR_extension 필드로 나누어 전송한다. 이 system dcx火
           과 PCR에 대해서는 5장에써 자세히 설명한다．
            그림 5-7에서 1S strean이 T-STI）어］ 입력되는 비트율은 구간별로 일정
           (piecewise constant rate）하다고 가정하는데 :rssbeam의 i번째 切te가 T-
           11STD에 입력되는 시칸우 t(i）로 표시한다． 일반적으로 t(i)는 PCR(i '）와
           岫nsport rate를 이용하여 다음과 같이 구한다．

                         Kn=           PCR(i            +        卜- l
                                                                                    (5.1)
                                             ")
                          "    syste刃IeC勿毗U戶叩uency          transport - r口te(i)



                  i P
                          TS sfl   에서 in (j <i' 사이의 임의의 by妃 인덱스이다．
                          현재 디코딩되고 있는 프로그램에서 가장 최근에 수신된 N只
                          伽D母am_clock_re佃ence) base 필드의 마지막 b丘가 포함된 by把
                         S를 가리키는 인덱스이다．
             PCR(it') i " 번째1 by把에서의 PCR값을 나타낸다．


            皿'a啣ort rate는 연속되는 2개의 PCR 필드와 그 사이의 byte 개수를
           이용하여 다음과 같이 구한다．

                        tr口nS끄Ort_ r口te(i) = ((i' 叫i")X莎stem - clock -戶eque兀cy) .     的
                                                       PCR(i') - PCR(i"i

             i,
                          현재 디코딩되고 있는 프로그램에서 PCR(program뇨a（乂k_iefer-
                          ence) base 필드 바로 다음의 bit를 포함하는 byte의 인덱스이다．
                                                       5. 시스템 목표디코더 모델


     따라서 i는 (i" K i5 i')의 조건을 만족하게 된다．


     프로그램이 바뀐 경우나 또는 동일한 프로그램에서도 시간기
                                                              준（time
base）이 바뀔 수 있는데 이와 같이 시간기준값이 불연속
                                                       이 되는 부분에
서는 IS packet header어］ 있는 小scontinui口jdicator）꾀서
中m
      1 1
                                   이를 알려주게
                           /
된다. 만일 이와 같은 불연속점이 생기게 되면 식 (5.1) 과
                                     '   \   +   尸 '
                                                                   m     '




                                    식 (5.2）는 불
연속이 되는 점을 기준으로 이전의 마지막 PCR 필드로
                                  부터 이후의 처
음 PCR 필드 사이에서는 적용될 수 없다. 이와 같은
                                   경우에는 새로운
time base로 바뀌는 스트림에서 최소한 2개의 PCI之
                                  필드가 있어야 식
J5J）과 식 (5.2）를 적용할 수 있게 된다． 다시말해서 t(i)와
                                                        trapsport rate
값은 현재의 스트림에서 time base가 바뀌기 전의 마지막
                                      번째와 마지
막에서 두 번째의 두 PCR들을 이용하여 계산하며 , time base가
                                         바뀐 후
에는 서로 동일한 time base를 갖는 새로운 두 개의
                                 PCR을 이용해야
한다．
 PCR값은 허용되는 정확도（tolerance）가 있는데 정확도
                                    란 수신되는
PCR값에서 허용되는 최대 오차를 의미한다. 이 PCR값의
                                    오차는 PCR
값 발생 당시의 오차를 포함하여 중간의 재다중화佃m
                              ulti히炚ing）과정에
서 생길 수 있는 오차등이 있을 수 있다. 그러나 여기서
                                  네트워크 지터
나 그 밖의 다른 원인으로 생길 수 있는 패킷 도착시간
                                  오차는 포함하
지 않는다. 入4PEG 시스템 파트에서 명시하는 PCR의 정확도
                                           （tolerance）는
+, 500n이다. 이와 갇은 PCR의 오차는 transport rate의
                                          계산과정에 영
향을 미치게 되므로 이는 곧 transpo凡꾜te의 오차가
                                  됨을 의미한다．
 복수 개의 프로그램으로 구성된 TS sneam인 경우에
                                    는 각각의 프로그
램이 다른 time base를 가질 수가 있으나 T-STI）어］ 입력되
                                        는 岫nsport
rate는 어떠한 프로그램이 T-STD에 입력되는가에
                               따라 결정된다. 이와
갇은 T-S1D의 가정 때문에 복수 개의 프로그램으로 구성된
                                    가변전송율
을 갖는 IS stream이라도 선택된 하나의 프로그램에
                                대해서는 입력비트
율이 구간별로 일정하다고 가정할 수 있는 것이다．
MPEG 시스템


            1
              下STD의 버푀와 트랜스포트 버퍼에서의 데이El 출력률

             T-S1D에서의 버피는 크川帥spo代 b雨呼而疝瀜 나뉘어진다．
           多TD buffer는 audio elementary stream과 시스템 정보의 경우에는 main
           쓰和롸고 불리우며 video elementary stream의 경우에는 multiplexing
           . bu卄er와 이ementary stream b咐er로 나뉘어져 있다． Transport buffer는 전송
            된 TS packet을 일시적으로 저장하기 위한 버퍼로 일단 전송된 모든 TS
           附：ket은 曲nsport buffer에 저장되며 이 버퍼에서 (Iur小cate 1'S 恥炚et은
           유료부하가 없는 TSi死icket이 걸러진다. STh bu珏er는 디코딩을 위한 버
            퍼인데 비디오의 경우 ele毗ntaiy stream 레벨에서의 버퍼제어가 필요하
            기 때문에（MPEG 비디오파트 참조） elementa口 stream buffer EBn을 따로
            독립시켰다. 따라서 이 EBn은 바로 비디오파트에서의 \TBVbu什er와 갇
            거］ 된다. Transr刃rtbu什er어4 저장된 '1'S packet에 저장되어 있는 PES
            packet의 일부분과 유료부하가 main bu什er 또는 multiplexing buffer로 옮
            겨지게 되며 그 이외의 TS packet hea把r부분에 있는 정보들은 sm를
            제어하는데 쓰이거나 버려지게 된다．
             그림 5-7에서 T-S1D에 입력되는 n번째 elemen切ry stream의 Th packet
            은 TS packet header에 있는 PID에 따라 역다중화되어 elementary stream
            n의 transport buffer인 TB으로 전달된다. 이 때의 천달과정에서 n번째
            elementary stream의 P11）를 갖는 모든 TS packet은 손실없이 TB으로 가
            거］ 되며 duplica妃 TS packet이나 유료부하가 없는 TS packet도 그대로．
            TB으로 전달된다. 역다중화되는 시간은 0으로 가정하므로 t(i)의 시간
            에 1번째 byte가 T-STI）어］ 입력되어 岫nsport bu什er TB으로 전달되는 동
            작이 순간적으로 이루어지는데 이는 TB에 1번째 by把가 도착하는 시간
            도 t(i)임을 의미한다．
              TB洲 저장되어 있는 PEST刃姚et의 일부분과 유료부하는 R＼의 전송
            읖로 버퍼를 빠져 나가는데 PES 恥icket이 audio elementary stream이라면
            main bu丘er 瓦에， 시스템 정보라면 玹羚어］ 전달되고 video elemenataiy
            . stream이라면 multiplexing 加卄erMB으로 전달된다． 이외의 다른 데이터
            （예 : duplicate I 'S stream pa火et)는 특별한 다른 목적으로 쓰일 수는 있어
                                                   5. 시스템 목표디코더 모델


도 瓦， 八'1떠11' 民，의 버퍼로 전달되지 않는다． 이와 같은 동작으로 bu什er
TB11으로부터 오디오, 비디오, 시스템의 각 데이터는 비워지게 되는데 만
일 TB11어］ 데이터가 없다면 Rx11은 0이 되며 TB, 어］ 데이터가 있는 경우
각각의 데이터가 각 transport bu卄h로부터 비워지는 속도는 아래와 갇다．


 d) 비디오의 경우

                Rxn= 1.2 x R11, X [pmfile,level]            的

    여기서 I릭mXmn)5把，leve끄는 入4PEG 비디오책（연암출판사）의 표 6-
   13 小IPEG IS는 table 8-13）에 규정되어 있는데 이는 특정한 profile
   및 level어］ 따른 각 video elememntary stream의 최대 전송율이다．
   특히 MPEG1 video stream인 경우에 RXn은 1.2水Rnm이 되는데 여
   기서 艮nax는 入4PEGI stream의 Constrained Parameters bitstream에서
   최대 비트율이 된다．


(2) 오디오의 경우

                    Rx= 2 x 106 bits/sec                 (5.4)


c) 시스딛J 정보의 경우

                    Rx11= 1 x 106bits/sec                (5.5)

     위에서 Rx11의 값은 system cli乂k frequency와 관졔가 있다. 즉
   27M bits/sec의 비트 전송율（bit rat이인 경우에는 system cli乂k의 8개
   펄스 동안에 정확히 Ibyte가 전송된다. 이는 시스템 인코더에서
   데이터가 system clock을 기준으로 전송되는 것을 의미한다. 현재
   프로그램에 관련된 시스템 정보를 갖고 있는 데이터는 岫nsport
   bu什er인 TB 어］ 입력된다． 시스템 정보를 갖는 패킷이란 P표）의
   값이 0, 1이거나 프로그램 구성정보인 PAT 및 PAT에서 시스템과
   관련된 PB）의 값을 갖는 모든 데이터를 말한다. 그러나 l汀r로서
                                               MPEG 시스템


                                                                                                      PMT에서 지정하는 Nrr_PID의 패킷은 TB邪로 전달되지 않는다．
                                                                                                      R人邪의 속도로 1且邪에서 비워지는 데이터는 瓦，로 전달되는데 이
                                                                                                      동작도 지연없이 순간적으로 이루어진다. 인코딩과정이나 재다중
                                                                                                      화佃multip妃x血g) 단꼐에서 특별한 목적으로 만들어지는 血plicate
                                                                                                       TSs甘earn packet은 瓦로 전달되지 않는다． Tansport bu什er에서
                                                                                                      main buffer나 multiplexing bu拜er로 전달되지 않는 데이터는 이 도중
                                                                                                       에서 처리되는 것을 의미한다．


                                                                                                   0 버퍼의 크:
                                                                                                          71


                                                                                                    모든L鈿P0. 빠坪芦J쁘唯로恥地 vi如 如啣
                                                                                                   sti帥 b“卄e' 의 크7L쁘陟 vi如 卿"' "凹 岫de"에 있는 'vbv_b"侄"!
                                                                                                   1없ze와 동일한 크기를 갖는다. 역시 video stream에 대하여 정의되는

                                                                                                   multiplexing b咐er의 크小雙考쓰쁘브쁘으回프갚' ] 규정된다·

                                                                                                    CD Low 및 Main level
                                                                                                                                                                          的
                                                                                                            MBSn = BS:m仄 + BSth + VBVmX[pmfiie,leveI] - vbv_buffer_size

                                                                                                            위에서 MBS.으로 건네지는 PBS packet의 일부 데이터 용량에 해
                                                                                           妾葬；
                                             ::::::::::::::;:;::;;::::E: :::i:;:i:::::;:;:：二           당되는 BSth(PES I刃rket overhead 加脆ring）은 아래와 갇이 규정된다．




I
                                        ::::i:
                                磁芟瑟轟轟蠶囊轟藝轟轟發
           ;;.:;.:;.:：휴：
                       驛磊：:::::::::::::：子표薑표：:::：룐珌：::;::::::：른煎：:i客泌：;:;
  難黨小蠱箋難難蝴難爵
                                                                                                                                                                          的
                                                                                                                     BS曲 = (11750)seconds x Rm [profile,level}

                                                                                                            또한 데이터의 분리를 위한 용량에 해당하는 BS1m佃dditional
                                                                                                       multi-plex buf扼ring）는 다음과 같이 정의된다．
m．   螂雖昏跏雜．   聃礪律
斗雄守雕三娜蝴難難艀44磁携．螂望

                                                                                                                                                                          幽
               口7Ja?a


                                                                 芟i;i；죵                                              BSnm仄 = 0.004 seconds * Rn日X [profile,level]
                                                              ;;:．囍轟
                                                    難i：磊挽：磁磁磁：:;:;:；룐룐i
                        m鱗壽醱重重
                                                                                                            VBVm[profile,level]은 入WEG 비디오책（연암출판사）의 표 6-14
       *
                                                                                                       (rvll毛GIS는 table 8-14）에서 규정하는 값을 가지며， vbv_bu什er啣e
                                                                                                        는 video elementary stream sequ毗ehe在奴에 있는 값이다．
                                                                                                        는
嫡壽身乍叫立們：
:i：景滋뇨．；朴；"多4胛．
    ！쩍：
               轟          麝射．  蜘礪；     凝繫瑟雄흘
                             .4韜易姿魏：;：發瓮舞．::.::．藿므
      :.;i;:1<:. +". · 甲弁5嚴粥磊發望글愍羅｛鞋藿
                                                                                                        1
    F芬F/    /h心        "1그 妊妊：11 /’·：＋소듣妊妊客壹妊妊：         ：듣든a
                                      多莪簇轟群聾瑟
                                         d;1;r1;:;:;:;:;FFF:;
                                               =;;:：근：口：;
                                               任任牡：       ：毫妾毫소姓｛

                                                                         書藝蓄．
                                                                           蠶醫．        ::::::::::
                                                         5. 시스템 목표디코더 모델


 @:)High 1440 및 城gh level

                      MBS = BSm仄 + BSth                       (5.9)

    여기서, BSm는 다음과 같이 규정된다．


             BSth = (11750)seconds )< 艮naxEP川이야eli           (5.10)

    또한 BSm따는 아래와 같다．


             BSmX = 0.0O4 seconds * Rjprofi1e,level]
                                                 )
                                                     (            <
                                                                          l
                                                                          l
                                                                      1
                                                              J
                                             /
     Rmax[profile,levell은 MPEG 비디오책（연암출판사）의 표                             6

    13小4PEG IS table 8-13）에서 규정되는 값이다．


（匈Constrained Parameters ISO/IEC 11172-2(八PEG1 vide아 bitstreams

          MBSn = BSm仄＋BS曲 + vbv_max 小 vbv_buffer_size        (5.12)

   여기서 BSth는 다음과 같이 정의된다．


                  BSQh = (11750) seconds X Rn目X              (5.13)

   BSmX is는 아래와 같다．
                                                             今
                  BSmX= 0．어꽈 S心X丑lds 半 R1mX                  6

     여기서 RnmX와 vbv_max는 入IPEGi b］디오파트의 Constrained
   I뇨time啣s bitstream에서 최대 비트율 및 최대 vbvbuffer뇨Si깝＝를 의
   미한다．
     MB욱의 버퍼용량 중 B옥의 양이 데이터분리（伽1如lexin匐에 필
   요한 용량이며 나머지의 용량은 BSm나 혹은 초기의 multiplexing
   어］ 이용될 수 있다
             ．
     呵bu脆【 S岫인 廓景 아래와 같다．
MPEG 시스템



               d) 오디오의 경우

                                                                        <
                                                                        J   <J
                               BSn = BSnm + BS4( + BS1, = 3584bytes

                                                                        死   h
                       위에서 access unit decoding bu卄er의 크기인 BS缸 및 PES
                      overhead bu珏町의 크기 BSm는 아래와 같이 제한된다．


                                    BS虹小4蜘                             (5.16)

                       ;3584byte 중에 736by妃는 추가 mu川plexing bu丘er田Smux）용으로
                      사용되고 나머지의 2848by把는 BS虹， BS血 및 추가의 multiplexing에
                      이용될 수 있다．


               (2) 시스털1 정보의 경우

                      入4缸.b.珏erB莎의 크기는碼6啣쿄이다．
           0 다중화 버퍼로부터의 데이터 출력방법

               Multiplexing bu什er는 vid的elementaiy stream의 경우에만 이용되는데
           buffer MBn으로부터 EBn bu拜er으로 전달되는 방법은 leak방법과 vbv
           delay방법이 있다．




               I上ak방법은 multiplexing bu甘er MB.으로부터 elementaiy stream bu珏er
           EB으로 데이터를 전달하는 한 방법으로서 그 속도는 Rb＼인데 아래에
           기술하는 어떠한 조건이 만족되더라도 이용될 수 있다．

               ／小 TS stream 상에서 해당 eleme曲口stream의 STD descriptor가 없는 경우
           (     S.   STI光明ciiptor가 있기는 하지만 leak_valid의 값이 I 인 경우
                      sm dSCrip兀가 있고 leak日V出id의 값이 '0' 이지만 video stream 상에써
                      vbv코elay의 값이 I下FF(H）이거나 trick mc月e가 참인 경우

                위와 같은 조건이 만족되는 경우 Rb＼은 다음과 같다．
                                                                   5. 시스템 목표디코더 모델


         a Low 및 M曲i level

                            =
                                Rb;   = Ril떠乂,profile,level)              (5.17)


         (2) 1云gl卜1440 및 I五gh level

                                                                                8\J/
                      Rbx. = 叫 (1.05 x 凡，Rm(pmfile,leve1)}                 <
                                                                           J    l
                                                 (
                                                                            口
                                             \
         G) ISO/IEC 11172-2 (入PEG1 video)OIIAI Constrained Parameters bitstream

                                           1.2 x R ；「          =
                                                                          (5.l9.

         위에서 Rn日x는 ISO/fEC 11172-2 Constrained Parameters bitstream에서의
       최대 bit ra把어］ 해당한다．
        만일 MB겨1 PES packet의 유료부하가 있고 bu珏er EB, 이 꽉 차지않은
       경우에는 PES packet 유료부하는 M瓦으로부터 EB, 어］ Rb, 의 속도로 전
       달된다. 그런데 EB이 꽉 찬 상황에서는 MB, 으로부터 데이터가 전달되
       지 않는다． M玩으로부터 데이터가 EB.으로 전달되는 동작에서 모든
       PES packet heal匕r 부분의 데이터는 순간적으로 디코딩되어 처리되므로
       싣질적으로는 유료부하 부분의 elementary stream만이 지연없이 전달되
       는 것이다. 만일 MBn buffer어］ 유료부하 부분에 해당하는 데이터가 없
       다면 아무런 데이터도 EBn으로 전달되지 않는다. 일단 M떠, 으로 입력된
       데이터는 모두 MB.으로부터 비워진다. 즉 MB어］ 있는 데이터는 EB, 어］
       전달될 수도 있거나 전달되지 않을 수도 있치만 MB, 어］ 상주하는 데이
       터는 없는 것이다．


&bv_
             de1a
                    y 방법）

        Vbv_delay 방법은 T-STD의 MB으로부터 EB으로 천달되는 시점을
  video elementary stream에 부호화된 vbv_delay의 값을 이용하여 정확히
 ：경시하는 방법이다． Vbv_delay방법은 해당 elementary stream의 Sm
       descri아or가 TS stream 상에서 존재하고 descriptor어］ 있는 leak_valid의 값
MPE(; 시스템


            이 0이면서 너deo elemenatry stream 상에 있는 vbv_delay의 값이 FFFF(1刃
            가 아닌 경우에 이용될 수 있는 방법이다. 入4PEG1 과 入WEG2 비디오파
            트에서 명시된 바에 따르면 한 너deo sequence어］ 있는 모든 vbv_delay 중
            어］ 하나라도 FT下F(H）이 아니면 이 咀꿔ence안에 있는 모튼 vbvjelay값
            은 FF1下（H）가 될 수 없다. 따라서 vbv셔elay방법을 이용하는 경우에
            video sequen凹에서 처음으로 나타나는 vi兀delay의 값을 한번만 참조하
            면 vbv_delay방법을 쓸 수 있는가를 알 수 있으며 일단 vbvdelay방법을
            :］용한 경우에는 이 쁘쁘多엣쁘뜨늪모툿그by겯奭y랖법으로끄Bd岬亘
            를 비우게 되는 것이다. Vbv_delay의 방법 J번째 picture start c以妃의 마
            지막 byte가 叫（j) - vbv_delay(j）의 시점에서 MB, 으로부터 비워진다. 여
            기서 叫a)는 picture j어］ 대한 디코딩시간을 의미하고 vbv_delay(j）는 초
            (second）의 단위로서 J번째 picture의 vbvHdelay값을 나타낸다. J번째
            pi야ure에 대하여 tdn(j) 尸 vbv_dela只j) 의 시점에서 M떠n으로부터 데이터를
            비우기 시작하여 구간별 고정비트율（pi凹ewise constant i砒e) RbXa）로 EB
            으로 전달되는데 이 때의 전달속도는 매 picture마다 다르게 된다. 한
            picture에서의 전달속도 R敬a)는 현재 picture sta八 code의 마지막 by把와
            다음 번 picture start code의 마지막 byte까지 적용된다. 각각의 picture어］
            대한 R敬)는 다음과 갇다．


                 R (j) = NBC) / (vbv_delay(j) - vbv_delay(j+1) + tdl(j+1) - tda))   (5.20)


             식 (5.20）에서 vbv_dela叭什1) 와 叫a+1)의 값은 만일 video elementa玎
            stream의 sequence ex妃nsion 부분에 있는 lowJ이ay의 값이 1인 경우 정
            상적 인 상황에서 요구되는 값과는 다를 수도 있다. 따라서 video
            extension field의 low_delay를 확인하기 전까지는 이 값을 정확히 예측할
            수 없는 것이다. 또한 위 식에서 NBC)는 J번째와 j+1번째의 pictu肥 start
            code 사이에 있는 J번째 picture 由ita어］ 대한 byte수를 의미하며 PES
            header data는 포함하지 않는다. 위에서 계산되는 R瓠a)는 八4PEG2 비디
            오 혹은 MPEG1의 constrained parameter video stream인 경우에 Rm
            (pmfile肥比1) 의 값보다는 작거나 갇아야 하고 MPEG1 의 video stream의
                                                  5. 시스템 목표디코더 모델


 경우에는 stream_id =01(H）를 갖는 elementary stream의 cons甘ained parame-
 ter어］서 허용된 최대 비트율보다 작거나 갇아야 한다．
  MB으로부터 EBn으로 전달되는 과정에서 M且어］ 있는 모든 PES
packet은 순간적으로 처리된다. PES packet header부분은 유료부하를 분
리하는데 이용되고 분리된 PES 유료부하는 EB, 으로 입력된다. 따라서
PES packet은 MB으로부터 지연없이 비워지며 O] 중의 일부 데이터가
순간적으로 EB, 어］ 쌓이게 되는 것이다．


 0
     T-STD에서의 데이터처리

EBB, Bn I叭표fer의 데이터 처리

  Transp（끄t Buffer -I且으로부터 분리된 elementa口 stream들은 각각의 ele-
menta口 stream bu珏er EBn과 main bu丘er 욕어］ 저장된다. 이 elemenatiy
stream들은 access unit 단위로 처리되는데 시간적으로 가장 오래된 access
. unit, 凡a)는 叫a)의 시간에 순간적으로 디코딩됨과 동시에 elementary
  stream bu珏町로부터 데이터가 비워지게 된다. PES packet의 유료부하에는
이emenataly stream과는 직접적으로 관계없는 stuffing data가 있을 수 있으
며, 이 stuffing data는 이ementary stream bu什er어］ 저장된다. STD모델에서는
tdn(j) 시점에 access unit An(j）이 디코딩되면서 이 시간 이전까지
elementa口 stream bu作er어］ 저장되어 있었던 모든 stu佈ng data는 갇이 비
워진다고 가정한다. 따라서 T-STD의 elememta日 stream bu卄er어］ 영원히
머물게 되는 PES packet의 유료부하는 없는 것이다. Access unit \a) 이
디코딩되는 시점은 叫a)인데 이 시간은 DTS field나 I기［'S field에 의하1
표현된 값이다. 그 밖의 j+l, j+2번째1 access unit에 대한 디코딩시간인
叫a+1), 叫(i+2）는 이에 해당하는 DI'S 혹은 Fm를 이용하여 구하게 되
지만 만일 이에 해당하는 프FS/DTS가 없다면 이전의 FT馴）Is값을 이용
하여 구한다. T-STD 모델에서는 디코딩 및 재생（presentation）할 때의 지
연시간을 0으로 간주하므로 오디오의 경우에 PES packet의 데이터가
access un奴加me）로 elementary stream bu什er를 빠져 나왔다면 이는 즉시
MPEG 시스템


           디코딩되어 재생되게 된다. 그러나 비디오의 경우에는 재배열(reordering)
           이 필요한 picture는 디코딩되어 재생되기까지 일정한 시간동안 기다려
           야 하므로 재배열지연（reordering delay）이 있을 수 있다.         러나    디오에
           서도 마찬가지로 디코딩하는 시간 및 재생하는떼1 소요되는 시간은 0으
           로 간주한다．




            시스템 정보의 경우에는 main bu珏h인 耳羚로부터 아래의 艮y: 속도로
           비워진다． ,O] 동작은 隘 bu脆r에 한 byte의 시스템 정보만 있더라도 O1
           속도로 비워지게 되는 것이므로 民，에서의 underfiow 상황은 발생할 수
           있으나 이는 전체 시스템 동작에는 문제가 되지 않는다．

                                                   (                      ln乙
                  凡 = max[80000bitsls力anspor乙毗(i) x8bit毗艸＋500]
                                               )                  <
                                                                      1
                                                                  U
                                               /
            위에서 岫nsporti毗가 큰 경우에는 艮邪도 더불어 증가하는데 이는 시
           스템 데이터인 Pmgram S1玘C而ci沚ormation에 대한 정보도 늘어남을 의
           미한다．


       LLow delay모드I처리
           샌翅少쁘照쁘m 중에' ] video卿”' "此 "' 妃nsio" 의 low_delay가 1
           인 경우에는 EB에 underfiow 7} 발생할 수 았다g作EG 비디오파트 참
           고）. 이와 같은 상황에서는 J번째 ac戈ss unit을 디코당하기 위하여 T-
           s-rn의 EBn을 td (j)의 시점에 조사한 결과 이 ac（氾ss unit에 대한 데이터
           가 모두 수신되지 않은 경우이다. 이러한 경우가 발생하께1 되면 T-STD
           는 EB, 을 두 field 간격을 두고 졔속 조사하면서 access ux血의 데이터가
           多전히 수신되면 순간적으로 이 데이터를 일시에 비워야 한다． 이는 실
           제의 시스템 디코더 설꼐시 low delay m（뇌e에1 대한 특수 처리과정이 필
           요함을 의미한다. T-STD에서 이와 같은 EBn underfiow 7} 발생하면
           DTh/I江'S의 값이 의미없는 값이 되므로 VFS/DTS의 값으로 디코딩 및
재생동작을 수행해서는 안되며 위에서 기술한때로 2field 단위로 조사한
결과 EBn bu珏er어］ 완전한 access ur血의 데이터가 있다면 이 시점을 기
준으로 가능한 빨리 디코딩 및 째생을 수행하도록 해야 한다． 디코더에
서는 EBn und釘加w의 상황이 종료되기까지는 정상적인 디코딩 및 재생
을 수행할 수 없는데 이는 FTS/DTS가 나타내는 값을 이용하여 디코딩
및 재생을 할 수 없다는 것을 의미한다． 디코더는 EBn underfiow의 상황1
으］. 종료된 후 vrsirn's의 값이 새로 전송되는 시점부터 정상적인 디코.
                                           ．
：딩 및 재생을 수행할 乞 있는 것이다·




 多pic血ire 형태의 access unit이 처음 시작하는 PES 恥姚et에서 이 PES
                쓰竺쁘翊 값이 1이고 trick_rn（月e_conti沚field의
yacket header의色쁘：
값이 '(X끄' (slow motion), '010' (fieeze 丘ame), 혹은 '100' (slow reverse）인
경우에는 이전의 어떤 picture field斗데이터가 여러번 디코딩 및 재생되브
로 마지막 번째의 디코딩 및 재생과정이 끝날 때까지 이 B-picture 뎨이
터를 EB.으로부터 버리지 말아야 한다． 비디오 데이터들을 디코딩하는
과정에서 한 picture data에 대한 반복적인 재생은 slow motion, slow
reverse 및 fieldjd_cntl의 경우에 발생할 수 있다. 이러한 상황에서는 다
음 picture에 대한 ac（玘ss UI血를 EB.로부터 추출하는 시점이 rep_cntl（반복
되는 회수）에 따라 다르께1 된다
                 ．
 한 picture의 picture start code의 첫번째 by把를 포함하는 PES packet의
header부분에서 . DSM出ck_mode flag의 값이 1인 경우는 trick_mode의 상
황에 해당하는데 이는 PES packet의 유료부하 중 picture stail code가
EBn으로부터 추출되는 시점부터 시작되는 것을 의미한다. 이와 갇은
trick mo妃의 상황은 hea（把r의 DS入4_trick日mode의 값이 0인 PES packet의
유료부하에 있는 새로운 pictu肥 start （刃de의 첫번째 l乃rte가 EBn으로부터
추출되는 시점까지 게속된다. Trick mode의 상황에서는 EBn에서
underfiow가 발생할 수는 있으나 스트림에 대한 이외의 다른 제한조건
은 그대로 유효하다．
MPEG 시스템



           .    디코딩

               1-sm에서의 복호화 동작은 순간적으로 이루어진다. 그림 三7의 블럭
           도에서 B., EB, 어］ 저장되어 있던 elementa口 sliam들은 각각의 디코더인
           瓦과 a. 어］ 저장되어 있던 elementary stream들은 각각의 디코더인 1기과
           I긱어］ 의해 순간적으로 디코딩된다. .디코딩된 孤'A兀ss UI血은 재생장치로
       －천달되거나 혹은 reordering buffer O1으로전달된다． Reordering bu作er로
           천달되는 경우는 비디오스트림의 경우에만 적용되며, 이는 elementary
           stream이 디코딩되는 순서와 재생되는 순서가 다른 경우인데 B-pictu玉
           이전의 I-picture나 P-picture가 이에 해당된다. 이외의 다른 데이터, 즉 디
           코딩되는 순서와 prese曲tion되는 순서가 동일한 데이터들은 모두 재생
           장치로 전달된다. 비디오의 B-1加ture 및 오디오의 경우가 이에 해당된다．
               Present抛이lunit은 비디오의 경우에는 ' 디코딩된 picture이고, 오디오의
           了 우에는 디코딩된 한如        드크잊털인다． T-STI）모델에서는 디코딩하는
           데 컬리는 시간을 0으로 가정하므로 k번째 presen帥on unit인 P (k）는
           吼(k）의 시점에 재생(presenta如n）되는데 , 만일 reordering이 없다면 디코
           딩 시점인 叫（k）과 tp,(k）는 동일한 값을 갖는다. 따라서 비디오의 B-
           picture나 오디오의 경우에는 디코딩 시점과 재생시점을 나타내는 叫（k)
           과 따（k）의 값이 서로 같다. 반면 reordering을 거치는 I-picture, P-i加ture
           는 叫（k）과 따（k）의 차이가 frame 간격의 정수배 만큼 난다. 이와 같은
           비디오의 부호화 및 복호화 순서에 대한 자세한 내용은 MPEG-2 비디
                                                                      /
           오파트를 참고하기 바란다．


           0 재생

               일반적인 시스템 디코딩의 목적은 압축된 elementa口 stream을 디코딩
           한 후 서로간의 동기가 맞게 재생하는 것이다. 1-sm모델에 맞게 인코
           딩된 시스템 스트림은 실제의 디코더 시스템에서 발생할 수 있는 지연
           시간을 0으로 가정하고 있다. 예를 들면 모니터의 디스플레이시간과 같
           이 비디오 재생시 발생할 수 있는 지연요소나 앰프 또는 스피커를 거
                                                  5. 시스템 목표디코더 모델



  치는 동안의 오디오신호의 지연시간을 모두 0으로 가정한 것이다. 따라
  서 시스템 디코더를 직접 설꼐하고자 하는 경우에는 실제의 디코더 시
  스템 각 단계에서 발생하는 치연시간을 고려하여 디코딩시간이나 재생
  시간등의 시간변수값들을 보정하여 사용해야 한다．


奴枷 버퍼운영방법
   TS sirearn어］ 대한 s-ri）의 각 버퍼는 아래에 기술한 버퍼상태에 맞도
  록 만들어져야 한다．

   ' -I且과      y   절대로 overflow가 발생해서는 안되며 일초에 적어도
       한 번 텅빈（emp口） 상태에 있어야 한다．
   1
       瓦에서는 절대로 und口flow나 overflow가 발생하지 않아야 한다．
   1
       EB, 는 underfiow가 발생해서는 안되지만 video sequence extension 부
       분의 lo싸 delay flag가 1이거나 trick mode의 상태가 참인 경웃에는
       예외적으로 underfiow가 발생할 수 있다．
   ' I上ak방법으로 ri떠n으로부터 데이터를 비워나가는 경우 M瓦에는
       ov口flow가 발생되지 않도록 해야 하고 적어도 일초에 한 번씩 텅빈
       (empty) 상태가 발생해야 한다．
   1
       Vbv小delay방법으로 MBn으로부터 데이터를 비워나가는 경우 MB에
       는 overflow나 underfiow가 발생되지 않도록 해야 하고 EBn은
       overflow가 발생하지 않도록 해야 한다
                              ．
   ·STI）의 각 버퍼를 통과하는 모든 데이터의 지연시간은 1초보다 작
       거나 갇아야 하지만 정지화면（still picture）에 대해서는 이보다 큰 只］
       연시간을 허용한다. 즉, J번째 access unit인 凡（j) 내에 있는 임의의 i
       번째 by把어］ 대하여 叫（j) - t(i) I Sa刃nd(for a끄j) 의 조건을 만족해야
       하고, 정치화면（still picture）인 경우에는 叫（j) - t(i）드印second（向r카ii)
       의 조건을 만족해야 한다．
       瓦（t)가 璘의 버퍼상태이고 t = t(0）일 때 F小) =0이라 하면 임의의 t
   1




       와 n어］ 대하여 05 F (t) 5 BS궈 조건을 만족해야 한다．
MPEG 시스템




    卜                      「-   STD모』및동작

           DP-STD(Program stream System Target Decoder)
            구성과 관련용어

              그림 5-8의 p-sm 모델은 T-STD와 마찬가지로 실제의 시스템에서 발
           생하는 지연과 같은 것을 고려하지 않은 개념적인 모델로서 PS stream
           을 디코딩하는 과정에서 필요한 기능이나 변수들을 정확히 기술하기
           위한 이상적인 PS stream 디코더 모델이다. 이와 같은 이상적인 디코더
           모델을 기반으로 본 시스템 권고안의 PS stiearn어］ 관련된 신택스가 기
           술되므로 독자는 Th stream에 있어서의 T-STI) 모델과 마찬가지로 P-
           Sm 모델을 정확히 이해할 필요가 있다．
             P-s-n）와 관련된 용어 및 표기법은 다음과 같다．

           i,i '   PS steam 상에서 특정한 byte들을 지칭하는 인덱스이다. 맨처
                   음 by妃의 인덱스는 0이고 0번째 byte라고 말한다．


                     1卜thbvte of       1

                     :multiplex Stream :
                                      J




                                          그림 5-8. P-STI）붑럭도
                                                             5. 시스템 목표디코더 모델


     j           El이nanta口 stream에서 J번째 ac（氾SS UI血을 나타내는 인덱스
     k,k',k" 日e毗n出y stream에서 k, k', k" 번째 prese曲tion unit을 나타내는
                 인덱스
     n           푀emanta口 stream을 나타내는 인덱스
     t
         (i)     PS stream중 i번째 by妃 data가 STI）어］ 입력되는 시간으로서 단
                 위는 초（second）이다. t(O）는 첫번째 byte가 입력되는 시간인데
                 디코더는 임의의 시간에 동작할 수 있으므로 이는 임의의 상
                수값을 갖는다．
     SCR(i)     叫i째 byte어］ 대한 SCR값으로서 i는 SCR필드 중 base필드
                (system_ck乂k_reference_base) 마지막 번째 byte를 가리킨다. 따라
                서 SCR(i)는 SCR base필드의 마지막 byte가 P-Sm에 입력되는
                시점을 2呱4Hz의 클럭단위로 표현한 것이다．
                .n번째 elemant켈y＋흐nmm에서 J 번째 出cess unit를 나타낸다. 이
                순서는 디코딩되는 순서를 따라 인덱스가 부여된다．
                凡n번째 ele    tary stream 어］서 J번째 access unit이 Sm에서 디코
                딩되는 시간을 나타낸다．
                n번째 elementary stream어］서 k번째 I玘sentation unit에 해당한다．
                P (k）는 凡(j)을 디코딩한 결과이며 이 인덱스 순서는 재생
                (p妃senta如n）되는 순서로 한다．
                n번찌1 이ementaty stream어］서 k번째 presenatation unit이 sm에
                서 재생伽tsentation）되는 시간（second）을 의미한다.
                초佃cond) 단위의 시간
Ft
          (t)   t의 시점에서 n번째 elementa口 stream어］ 대하여 sm입력버퍼
                의 충족도伽Ilness）를 byte단위로 나타낸 것이다．
                n번째 element缸y s甘earn의 main bu什er를 나타낸다. 이 main
                bu作er는 audio elementary stream어］ 대해서만 있다．
                by妃단위로 표현된 틔의 크기
                n번째 elementary stream의 디코더
。Dn             n번째 video elementary stream어］ 대한 reorder bu什er
MPEG 시스템


            0
                  P-STD의 입력시간

            PSsbeadn의 1번째 by把7f P-STh로 입력되는 시간 t(i)은 PS stream의
           pack header어］ 있는 Pt璡ram_mux_ra妃와 羽R(sys妃m뇨야乂kre色妃n(氾）값을 이
           용하여 구할 수 있다. PCR과 마찬가지로 SCR도 base 필드와 extension
           필드로 구성된다．
                                                                                                 刃
                         (i)   =             SCR   (i   ')   .   +             i-   i   '   -.
                                                                                                 5
                                    system - clock - frequency       program - mux - rate X DU
                     r
             i,
                                   pack header어］ 있는 sys把m cl(乂kre也re毗小ase필드의 마지막 bit
                                   가 포함된 byte를 가리키는 인덱스이다．
             i                     pack header를 포함하여 pack 안에 있는 임의의 by把를 가리키
                                   는 인덱스이다．
             SCR(i')               i ' 번째 byte어］서의 SCR값을 나타낸다．

            pm留帥1mux皿te는 PS stream이 P-Sm로 수신되는 데이터율（data rate)
           을 의미한다．
            어떤 한 pack의 마지막 번째 데이터가 p-Sm어］ 수신된 후 다음의
           byte가 수신되기까지 데이터가 없을 수도 있는데 이는 pack과 pack 사
           이에 시간간격（time in妃rval)이 존재할 수 있음을 의미한다．

            1
                  P-STD 버퍼

            그림 5-8의 블럭도에서 입력되는 PS stream의 n번째 elemantaiy stream
           올 갖고 있는 PES packet은 입력버퍼인 瓦으로 전달된다. 이 과정에서
           S끄）에 입력되는 i번째 byte data가 입력버퍼 瓦으로 전달되는 동작은
           순간적으로 이루어진다고 가정하므로 O] 버퍼에 입력되는 시간도 t(i)가
           된다. 입력되는 데이터에 해당하는 system header, 혹은 PES packet header
           에 있는 ID정보（stream-id）를 이용하여 입력되는 데이터가 어떤 종류의
           elementa工y stream인지를 구분한 후, PES packer의 유료부하에 있는 내용
           을 y력버퍼 瓦에 전달한다 Pack header, system header 및 PES packet
                                ．예를 들어 SCR, DTh, Fl'S
       4header의 데이터들은 瓦에 전달되지 않는다
                                              5. 시스템 목표디코더 모델


 및 pack아_length와 같이 header어］ 실린 내용은 시스템 제어를 위한 정보
 로서 이용된다. 따라서 p-S끄） 보델에서 B, 에는『            packet의 유료恥 2
 만이 저장된다고 가정한다．
  PES packet header어］ 입력버퍼 B, 의 크기를 나타내는 P-Sm buffer size
 가 전송되는데 자세한 내용은 6장의 PES packet의 신택스 부분을 참조
 하기 " 下란다：,，烈烈 대한 디코딩 ' ］간인 叫a）는 DTS나 P1S로부터 알
 수 있는데 만일 V's의 값만이 있다면 DTS의 값은 Vrs의 값과 동일하
 거］ 간주한다. Access Unit은 한 fi n妃data예 해당하고 이ementary str跏Ti들
 의 fiamera把는 이미 알고 있으므로 DTS, F'TS가 없는 ac无ss unit에 대한
 디코딩시간은 가장 최근에 수신된 叫a)값을 이용하여 만든다. 즉 Ana)
 에 대한 DTSa)값으로부터 叫（j) 값을 알았다면 叫（j+ 1), 叫（j+ 2), ···의
값들은 한 frame간격을 띠라 할 때, （叫) + tf11), （叫) +2非tf,), ···으로 구
 한다. Fm工ne rate를 나타내는 신택스는 elememtaiy stream header에 있는데
자세한 사항은 入4PE(끄의 오디오, 비디오 파트를 참조하기 바란다．
  P-sm에서의 복호과정은 T-STI）와 마찬가지로 순간적으로 이루어진
다고 가정한다. 그림 5-8의 블럭도에서 버퍼인 弓과 瓦어］ 저장되어 있
던 elementaiy stream들은 각각의 디코더인 1기과 Dn어］ 의해 지연없이 순
간적으로 디코딩된다. 디코딩된 elemen仕ay stream은 재생장치로 전달되
거나 혹은 reordering bu珏brOl 어］ 전달된다. 이 이후의 동작은 T-STD어］
서 가정하는 것과 동일하므로 이 부분을 참조하기 바란다．
  P-sm 모델에서 지속적인 디코딩 과정중 각 elemetemtaxy stream 버퍼는
. und耐low나 overflow 7} 발생하지 않아야 하는데 이 조건은 아래와 같다. '


                 05乙(t) 드邵.   向r때나and n              伍23)

  F (t)   i-sm에서 瓦의 버퍼충족도（bu珏er fullness）를 나타낸다．
  BSn     瓦의 크기를 나타낸다．
  t       t(O）인 순간에서의 버퍼충족도（bu什er fullness) F小）는 0이다．

 I冬 stream이 sm의 각 버퍼에서 소요되는 지연시간은 정지화면（still
pict네e）인 경우를 제외하고 다른 모든 데이터에 대하여 1초를 넘지 않아
MPEG 시스템



           야 하는데, 여기서 지연시간이라 함은 어떤 데이터가 瓦에 입력되어 디
           코딩되기까지 걸리는 시간을 의미한다． 이와 갇은 조건은 J번째 access
           unit 내에 있는 임의의 i번째 byte어］ 대하여 아래와 갇이 정리할 수 있다．


                 叫（力 - t(i) 5 1：比 (S出I picture video data가 아닌 경우）            M
                                                                             5
                 ki (j) - z(i) 5 1:eC (still picture video 缸a인 경우）

            Video elementa口 stream 중에서 video sequence ex把nsion의 lo뾰코elay가 1
           인 경우에는 B, 어］ underfiow가 발생할 수 있다小4PEG 비디오 파트 참
           고）. 이와 갇은 상황에서는 J번째 access unit을 디코딩하기 위하여 P-
           Sm의 육을 叫（j) 의 시점에 조사한 결과 이 access ui血에 대한 데이터가
           모두 수신되지 않은 경우이다. 이러한 경우가 발생하게 되면 P-Sm는
           B, 을 두 field 간격을 두고 꼐속 조사하면서 access unit의 데이터가 완전
           히 수신되면 순간적으로 이 데이터를 일시에 비워야 한다. 이는 실제의
           시스템 디코더 설계시， low delay m에e어］ 대한 특수 처리                     O ] 필
           을 의미한다. P-S11）에서 이와 갇은 EBnund이flow가 발생하면 1끄s/vrs
           의 값이 의미없는 값이 되므로 PTS/I끄'S의 값으로 디코딩 및 재생동작
           을 수행해서는 안되며 위에서 기술한대로 2fle1d 단위로 조사한 결과
           Bnbu作er어］ 완전한 access unit의 데이터가 있다면 이 시점을 기준으로 가
           능한 빨리 디코딩 및 재생을 수행하도록 해야 한다／단쿠旦에서는 B
           underfiow의 상황이 종료되기까지는 정상적인 디코딩 및 재생을 수행할
           수 없는데 이는 P1'S/I끄'S가 나타내는 값을 이용하여 디코딩 및 재생을
       百耳쿄다는 것을 의미한다. 디코더는 B, un由rflow의 상황이 종료된
           후 P1'S/ I끄'S의 값이 새로 전송되는 시점부터 정상적인 디코딩 및 재생
           을 수행할 수 있는 것이다．


           0 PES 스트림

            PES stream이란 동일한 elementa口 stream어］ 대한 일련의 PES packet을
           의미한4. PES-STD(Packetized Elementary Stream-System Target Decoder) 모델
           은 p-Sm와 비슷한 모델로 생각할 수 있는데 PS stream이 단지 하나의
                                                  5. 시스템 목표디코더 모델


 elementary stream으로만 구성된 경우라고 간주하면 P-Si]）는 곧 PES-STD
 가 된다. PES-STD 모델에서는 PES stream을 디코딩하기 위한 가상의 디
 코더이므로 P-STI必｝ 같은 개념으로 디코딩 동작을 설명할 수 있으나
 p-S-n）와의 차이점은 P-Sm의 SCR(System Cli乂k Refe肥nce) 대신 ESCR
 (Elementary System Clock Reference）를 사용하고, program_mu凡只te 대신
 ESmrate를 이용하는 점이다．


 0P-STD에서의 디코딩 및 재생

     P-Si,'）의 디코딩 및 재생과정은 T-SiD에서와 동일하다．




卜뇨』클」* AI ]i
 .    시스템 클럭의 주파수와 오차

     그림 5-1에서 도시한 클럭은 시스템 인코더를 구성하는 모든 블럭에
제공되는 시스템 클럭에 해당하는데 이 시스템 클럭의 주파수는 식
(5.25）와 갇은 제한조건을 만족해야 한다．


      ?7r狂初 - 810Hz 莎Ste刃LCI0(火jrequen口5 27卜爪也＋810R乙
      玎stem下勿ckj沌quency의 시간변화율575 x l03llzlsec         (525)

     식 (5.25）의 제한 조건은 최소한의 제한 조건인데 만일 이보다 더 정
확한 sys妃m clock올 필요로 하는 프로그램의 경우에는 시스템 인코더 단
에서 더 정확한 클럭을 이용하여 프로그램을 만들면서 이 때의 system
ckFk의1-I斗환 정확도를 별도의 정보로 전송할 수 있다. 이 정보는IyS把m)
   ck desciipto 란늑 정보인데 이는 9장에서 다시 설명할‘玉。
( l。                                    ld-. -고二
MPEG 시스템



           템파트에서 언급하고 있는 y                       ］란 식 (5.25）를 만족하는 클럭이
           며 sys把m ckx火desci如tor부분에서 특별한 언급이 없는 한 1S stream이나
           PSsliam은 식 (5.25）의 조컨을 만족하는 sys把m clo永을 이용하여 만들게
           된다. 식 (5.25）의 의미로 본다면 sys妃m比乂k fiequency는 2亦皿七에서 +,
           - 810Hz의 오차를 허용하는데 이는 27M1由를 기준으로 +, -0.003％의
           범위에 해당된다. 또한 이 오차의 범위에서 동작을 한다 할지라도 클럭
           의 변화가 급격하게 생기면 안되는데 이를 두 번째의 식에서 규정하고
           있다. 이는 I초에 0.075Hz의 변화까지를 허용하는 것으로서 1초에
           2乃皿七로 동작한다면 360M 클럭에 한 클럭이 어긋남을 의미한다．


           1PCR, SCR, ESCR

           t匹R毋Dgram Clock Re免ren回은 시스템 전반에 컬처 중요한 개념인데 이
           러한 시간값의 의미와, 인코더에서 이런 시간값을 만드는 과정 및 디코
           더에서 이 값들을 이용하는 과정등을 명확히 이해하기 위해서는 몇 가
           지의 개념들이 복합적으로 설명되어야 한다. 이 서］ 개의 시간값들은 이
           용하는 경우가 틀릴 뿐이지 개념 및 방법은 모두 갇다. 따라서 이 서］ 가
           지 시간값에 대한 入IPEG 시스템 파트에서의 정의를 먼저 기술하고 그
           후 PCR을 예로 들어서 이 서］ 가치 시간값들의 의미를 살펴보기로 한다．
           仄：R(l如甲m Clock Re也mm无）은 TS sUeam에서 프로그램에 대한 시간기준값
           을 나타내며 이 기준값은 식 (5.26）과 같이 계산된다. 식 (5.26）에서 i는 i
           번째 by把를 의미하고 t(i)는 i번째 byte가 T-STI）어］ 입력되는 시간이다．

              PCR1自as的 = 佈y毗m曲ckjreuency x t(功DIV3以）) % 233
              PCR寸ext(i) = 佃四em下뇨允加quency >< i(i))DIV1) % 300           茄
                                                                        5
              PCR(i) = RCR_base(i) x 300 + PCR_ext(i)

              SCR_b口貂(1) = ((system_clockJ跏凹 x 仰DIV 3叫 % 233
              SCR_ext(i) = ((system_clock加quency x t(i)) DIV 1) % 300   刃
                                                                        5
              SCR(i) = SCR_b口Se(i) x 300+ PCR_ext(i)

              ESCR_base(i) = ((system_clockj油ie砒功m力끼V300) % 233
              ESCRext(i) = ((s釘e刃_clockjrequen乃7 x 1(i)) DIV 1) % 300
                                                                        <
                                                                        U   八乙
                                                                                 8
              ESCR(i) = ESCR_base(i) x 300+ PCR_ext(i)                  1
                                                 5. 시스템 목표디코더 모델



 이 시간값들은 식 (5.25）의 조건을 만족하는 system_cl(乂k伽equency로 샘
 플링하여 만든다. 이 과정에서 PCR/SCRJESCR은 잇）日aZ 단위（syst咆즈峽k
 航q此ncy/300）로 표현되는／3三；目）트 킬이의 而盂鈿匹啣ESCR如S이
 와 27入4H『 단위（system_clock_frequency）로 표현되는 Q브틔의 PCRU
 ext(S（二巳切se/ESCR小ase）로 구성된다. PCR(i)(SCR(i)/ESCR(i力에서의 i는
 PCR_base(SC艮ba打ESCR_ba配）의 마치막 bit를 포함하는 by倪를 가리킨다      ．
 겸국 PCR(iXSCR(i)厄釵R(i)）는 PCR_base(SCR base/ESCR base）의 마지막 bit
．가 포함된 byte가 T-STD(P-S1D/PES-STD）에 입력되누 시칸을 sys妃mck乂k
    f佃ency로 나타낸 것이다. 이에 대한 설명을 위하여 샘플링, PCR中base
 의 마지막 by也, s-Il）어］ 입력되는 시간등의 개념을 살펴보기로 한다．
  PCR값은 시스템 인코더에서의 산갚量귿꼬쁘三의． S工曾므딤딴
                                     읖르쏘
，퓰里한쏘이다． PCR은 MPEGI과의 호환성을 고려해서 base필드의 33
 비트와 extension 필드의 9비트로 나누어 나타내는데 중간에 6비트의 의
 미없는 reserved비트를 추가하여（실은 by把－align을 하기 위함임） 총
 48bits(6by也5）로 구성된다. PCR을 만드는 과정에서 시간은 system_clock_
 frequency로 샘플링되므로 샘플간의 시간은 sai 叩ling_clock_介equency 의
 역수（0.0037n配이에 해당한다. 샘플링된 시간값은 42비트로 표현되므로
뇨

 42비트로 표현된 한 단위의 정수값이 곧 샘플링 간격（0.0037nsec）에 하1
당되며 PCR로서 표현할 수 있는 시간의 범위는 0초에서 시간간격
(0.0037nsec) 水 최대값（42비트로 표현할 수 있는 최대 정수）= 162890.4초
이다. 仄：R이 최대값에 도달한 경우 다시 0으로 되는 modu幻의 연산이
 된다. 식 (5.26）에서 알 수 있듯이 이 값은 伽quency州me）으로 계산되므
로 결과의 값은 단위가 없는 상수인데 frequency는 system_clock叫
frequency이며, time은 i번째 byte가 Sm에 입력되는 시간 t(i)를 말한다．
따라서 PCR값을 systen냐k乂k_frequency로 나누게 되면 t(i)에 해당하는
시간이 된다．
    식 (5.26）에서 t(i), 즉 i번째 by把가 S-
                                 ID에 입력되는 시간이란 0번째
byte의 시간이 0일 때m이＝0), i번째 byte어］ 해당하는 시간을 나타내는데
lransp朮r毗rs       의 전송율）가 (b少eJsec）의 단위로 표현된 값이므로
(i/trai咨port_rate）초에 해당한다. 일반적인 관계를 그림 5-9에 나타내었는데
MPEG 시스템


           이 그림에서 1-s snemn부분과 time부분을 같이 보면 이 관계를 쉽게 알
           수 있을 것이다. 그림에서 1-S stream의 한 클럭 길이는 (iby把）에 해당하
           는 시간인데 이는 (1/tran斗刃仄mte）초에 해당한다. PCR(b）에서 b번째 byte
           란 PCR(b）의 PCR_base 필드의 마지막 bit를 포함하는 by把카 s-Il）어］ 입력


                ／迎址
                                                                                              b-th byte
                                                   (b-a)bytes
                                                   m
                r                                                                                         ed+e工tdai口：
                                                                                                                    ,
                                                                                                          /
              PCR(a)                                                      PCR(b)
                                                                                                                     r눋’
                                                                                                          I byte intereval =
                                                       extj
                                                                                                          口力ran斗刃rt r口te) sec
                               !reserved+
             b口S丘   <                                            (
                                                                  b口seth玎口

                                                                     H
                                                                      H           그
                                                                                          入<                2
                                                                                  ＝
                                                                                      니

                                                                                                             TS stream
                         伊CR_b口se 斗300+PCR．尸e川 clock 加 27MHz Unit


                                            （뇨기力rans까7月_rate (sec)
                L{


                                                                          PCR e玎
                            PCR_base *300(clock)                          clock
                                                                      >   (               }




                                                                              r




                                                                                                            27 MHz clock
                    卯KHz 杉00 = 27兀川z
                    Li                            >




                                                                                                            90 MHz clock




                                                                                          口
                                                PCR base clock




                t(a)                                                          /'          t(b)                time(sec)

                                                      玎b) == 玎口） + (b－口刃ra啣or乙r口妃 sec


                                              그림 5떠. 1-s sen과 PCR. clock 및 dnt의 관계
                                           5. 시스템 목표디코더 모델



되는 시간인 t（均를 1X꾜로 표현한 것이며 PCR손므邑궐트늪3羽塑虹坦十
i bit）이므로 t（匈는 그림과 같이 PCR(b）의 구간 중 4by把가 지난 시점이
뽀단느그리고 PCR(b) 구간 중 나머치 구간은 reserved와 PCR_ ext 필드를
전송하는 구간이 된다. PCR로 표현하는 과정은 90KHz 단위로 ’나타낼
수 있는 PCR뇨base필드와 엇)kHz로 나타내고 남은 시간을 27入'II七로 표현
하는 P(只ext 필드로 구성되며 P(：取a）도 마찬가지로 구성된다. TS stream
의 a번째 byte어］ 해당하는 시간 t(a）와 b번째 byte어］ 해당하는 시간 t(b)
와의 차이는 （他따伽nspo凡ra把）초가 되며, 그 구간에서의 system clock 개
수는 그림 5-9에서와 같이 PCR니base어］ 해당하는 부분인 (PCR寸base半300)
클럭과 그 나머지인 (PCR_ext）클럭으로 나누어 생각할 수 있다. 결국 t(b)
는 그림에서와 같이 ((t(a) + (b - a))/trai珥壯trat이가 되는 것이다. 이와 갇
이 PCR올 나누어서 계산하는 이유는 入4PEG1 (ISO/IEC 11172）에서 入4PEG2
의 PCR과 갇은 기능을 하는 SCR(Sys妃mGk乂k Reference）이 入WEG2 system
Hckx火_frequency의 1/300에 해당하는 잇)KHz로 계산되므로 이는 入4PEG1
시스템과의 호환성을 주기 위함이다. 즉 MPEG2의 TS sUeam으로 入4PEG1
의 elementaiy stream을 전송하고 수신기에서 MPEG1 시스템 디코더를 이
용하여 프로그램을 디코딩할 때 入4PEG1 시스템 디코더는 入'IPEG2 P1'S
stream어］서 PCR日base 부분만을 보고 마치 八4PEG1의 SCR로 간주하는 것
이다. 결론적으로 PCR(b）의 base 필드는 식 位26）에서처럼 system_cl(乂k
frequency水t(b）를 300으로 나누어 정수값만을 취한 후（DiV 300연산） 이를
2好의 m以川O 연산을 수행하여 bin町33bit로 표현한 것이고, PCR_e毗는
system_clock_frequency 永 t(b）의 값에서 정수값을 취한 후（DIV1 연산）
modulo 300의 연산을 수행하여 이를 9비트로 표현한 것이다. 결국
RR(b）는 이들을 합한 PCR上ase水300 + PCR_e胤의 값으로 계산된다．
 그림 5-10은 인코더의 sytem clock으로부터 PCR을 만들어 이 값을 TS
packet의 adaptional header부분에 삽입하고 다시 시스템 디코더에서 이
값을 추출하여 디코더클럭을 맞추는 과정을 나타낸다. 이 과정에서 인
코더의 n口R(i)값은 1'S stream 중 i번째 byte가 만들어지는 시점에서의
PCR값을 갖게 되며, 디코더에서는 이 i번째 byte를 수신하여 처리하려
는 시점에서 이 PCR값을 알 수 있게 된다. 따라서 전송과정에서의 지
MPEG 비디오



           연을 생각하면 결국 인코더와 디코더에서의 PCR이 나타내는 절대적인
           시간은 차이가 나게 된다. 그러나 C1(乂k mcovery는 철대적인 시간을 기
           준으로 하는 것이 아니라 인코더에서 만든 PCR값을 기준으로 해서 상
           대적으로 디코더 시간（ci（乂k）을 맞추는 것이기 때문에 디코더는 인코더
           에서 쓴 값을 그대로 읽어 이용하며 전송 중 또는 처리과정에서의 只］
           연시간은 고려하지 않는다. 본 시스템 파트에서 가정하는 타이밍모델에
           서는 앞에서 설명한 바와 같이 일정한 지연시간을 갖는다고 가정하는
           더］ 이 가정대로 해석하면 절대적인 시간기준으로 인코더에서 특정 byte
           를 만들면 특정시간 후 디코더에서 이 byte를 읽지만 이러한 지연시간
           도 0으로 가정하면（무시하면） 인코더에서 고려하는 시간은 곧 STD에
           서의 시간인 것이다． 따라서 일코더에서 PCR을 만들 때 P(그R(i)에서의

                                               one TS packet with PCR field
                           <


                                               header


                                   adaptioanal
                           4 bytes
                                   header with
                           header
                                   PCR(i)


                                                                                                  m
                               ,   ,   ,   1     "   "


                TRANSMISSION
                BUt十ER                                              TRANSPORT
                                                                    B1序下ER in STD
                                                         인코더
                                                     system

                                                                     trasnport
                  trasnport            PCR(i)                        stream
                  stream                                             de_packetizer
                  packetizer                                                    !
                       A
                                                               PCR(i)                    clock
                                                                            1
                                                                                         re叩j므21
                  system
                                                                        1
                                           PCR
                  clock                    counter                decoder           >
                                                                                        PCR
                                                                  clock                 counter
                                                                                                    U



                                                                                        recovered
                                                                                        PCR回

                  그림 5-10. 인코더 PCR(i)값과 幻刀에서의 수신 시간관계
                                                           5. 시스템 목표디코더 모델


 t(i)는 Sm의 岫nsport bu珏er어］ i i째 by妃가 쓰여지는 시점과 동일하다고
 가정할 수 있는 것이다．


     0DTS(Decoding Time Stamp)

     DTS는 STI）에서 이ementa口 S甘earn을 디코딩하는 시점을 나타내는데
 이 값은 system Cl(乂k fiequency의 1/300단위로 표현된 값으로서 식 位29)
 어］ 같이 계산된다．


           DTS(J) = ((system_c勿ckfrequency x t41(力DIV 300) % 2B   (5.29)

     D作의 값은 PES packet header부분에 있는데 DTS(j）는 그림 5-13에 나
 타낸 바와 갇이 PES packet의 유료부하에서 처음으로 나타나는 J번째
 access unit을 elementaiy stream 디코더에서 디코딩해야 하는 시점을 나타
 卜



 낸다. 여기서 access unit이란 2장의 용어정의 부분에서 기술한 바와 갇
 이 재생하고자 하는 단위의 부호화된 형태로서 한 frame의 오디오나
 picture 데이터롤 말한다．
     DTS값과 PCR값을 이용하여 디코더에서 elementary s出am을 디코딩하
 는 S恤I signal을 만들어주는 과정을 그림 5-11어］ 나타내었다. DTS(j)는 n
 번째 elementary stream어］서의 J번째 access w血을 디코딩해야 할 시간인
叫(j)를 (sys把m (永乂k玉equency/300）의 주파수로 샘플링해서 33비트로 표
．현한 것이다． 따라서 디코더에서는 DTh）의 값을 (sys把m cl(乂k_frequency
 /30力으로 나누면 디코딩해야 하는 시간을 알 수 있는데 여기서 의미하
 는 시간은 PCR올 기준으로 표현된 상대적인 시간이다. 앞 절에서 설명
 한 바와 갇이 PCR은 곧 system do出으로 표현되는 값인데 이 값중 PCR
base인 하위 33비트에 해당하는 것이 DTh에서와 같은 ck兀k frequency를
 갖는다. 예를 들어 sm에서 DTSj)값을 읽는 시점에서 디코더 PCR의
하위 33t3］트의 값이 10000이고 D1Sj)의 값이 2以乂0이었다면 이ementary
stream 디코더는 현재의 시점에서 PCR 하위 33U］트의 값이 2000(）이 될
때까지 기다렸다가 20000이 되는 시점에서 elementary stream을 디코딩하
는 것이다. 결국 DTSj) 의 비트를 읽고 난 후 10000水 300/sys也m1ck兄k누
MPEG 비디오


                  TS stre口刃i      ／坦S計re口／n             elementary 針re口m



                                                                    elementary              elementary
              +    TS stream            PES stream          w
                                                       1=       +
                                                                    stream                  stream
                   denacketizer         depacketizer
                                                                                 -+
                                                                    BIJi卜匕R                 decoder



                                         DTS
                       PCR                                          comparator
                                         extraction
                                                                                        A
                                                                                        1
                               decoder clock recover-v bloc
                                                                                        1
                                                                                      釘口rt
                                          PCR counter                                 signal
                                          lower 33 bits



                      그립 5-11. DTS, PCR 및 el日nent쏘7 stream d텨）)der으4 동작관계



           frequency의 시간（2乃dHz의 sys妃m cl(乂k인 경우 lllpsec）동안 기다려야 한
           다. 디코더에서 디코딩타임에 맞추어 디코딩한다는 것은 곧 디코더의 버
           퍼를 조절하면서 디코딩하는 것인데 만일 曲nsport rate가 小4b外elsec인 경
           우 위의 예에서 l000000byteJsec永O.lllsec = lll000byte의 데이터가 디코더
           버퍼에 쌓이게 되는 시점에서 디코딩하는 것이다. 따라서 DTS의 값이
           언긋나 있다거나 잘못 계산된 경우에는 디코더버퍼의 underfiow나
           ov口flow가 발생할 수 있다. 여기서 한 가지 고려할 사항은 Dl's값이 갖
           고 있는 시간 오차의 문제이다. Dl's는 샘플링 frequecy의 역수인 (300/
           sys把m_cl(乂k玉텍uency）의 시간간격을 갖는데, 四 stream은 system ckx火
           frequency어］ 맞추어 입력되므로 Dl's 와의 시간 오차가 최대（3田system_
           clock_frequency）초인 것을 의미한다. 즉 DTS는 최대 11.llsec의 오차범위
           (_ 5.55／초eC에서 +5.55usec 사이）를 갖는다. 이는 곧 디코더에서 이 오차
           어］ 해당하는 데이터를 담아놓을 수 있는 여분의 버퍼가 필요한 것을 의
           미하며 1Mbyte/sec의 transp아Irate인 경우 11. ibyte어］ 해당하는 양이다．
            이러한 Dl's 오차의 해결 방안은 크게 두 가지가 있는데 하나는 Dl's
           의 오차를 줄이는 방법과 다른 하나는 어느 정도 DTS 오차를 허용하면
           서 버퍼크기를 늘이는 방안이다. DI'S의 값은 매 access unit마다 전송되
                                                            5. 시스템 목표디코더 모델



는 것이 아니라 최대 0.7초 이내에 전송하는 것을 MPEG에서 규정하고
있는데 예를 들어 그림 5-12와 갇이 30Hz丘帥e율을 갖는 비디오 신호
의 경우 한 frame의 간격이 33邸ec이므로 인코더에서 최대 2lframe마다
한번씩 DTh값을 전송하면 되는 것이다. 여기서 나머치 20frame어］ 해당
하는 DTh값을 어떻게 디코더에서 만들어 낼 것인가의 문제가 DTS의
오차를 줄이는 첫번째 방법이다. 보통의 경우는 맨처음 frame의 DTS값
．어］ 33msec씩을 더해나가는 방법을 이용한다. 또한 오디오의 경우는 그
림 5-12와 갇이 24msec간격의 aud的ft加叱으로 이루어져 있는데 비디오
의 경우와 같이 처음 frame의 DTS에 24msec씩을 더해나가면 된다. 두
번째 해결방안으로는 발생할 수 있는 DTS의 최대 오차한꼐를 구한 후
岫nsportra妃어］ 따라 여분의 버퍼를 두는 방법이다. 따라서 이와 같은 하1
결방법은 실제의 응용 분야 및 구현시스템의 안정도에 따라 이외의 여
러 가지의 접근 방법이 있을 수 있으므로 각각의 경우에 어떤 방향이
효율적인 시스템이 될지는 많은 변수가 있는 것이다. 저자가 퀀유하고
싶은 것은 우선 허용오차의 한꼐를 설정하는 것이 시스템의 다른 부분
을 설계하는데에도 도움을 줄 것이라는 것이다．
 入4PEG 시스템 파트에서 가정하는 Sm는 elementary stream 디코더에서
디코딩하는데 걸리는 시간을 0으로 간주한다. 이는 시스템 디코더，
elementary stream, 코딩기법 등의 종류에 따라 디코딩 타임이 가변적이기
때문에 이렇게 가정한 것이다. 다음 절에서 기술될 v1S(PI邙entation끄me
Stamp）는 디코딩된 access ui血이 재생（p忙sentation）되어야                  }1m              을 나
타내는 디코딩된 access unit이 곧바로 재생佃esentation）되어야 한다면 이
access unit에서는 DTS값과 Pm값이 동일하게 된다. 그러나 비디오의 경


      IL       I
      1 33msec I 33msec
              >1<          1
                          'y
                               I
                                     .
                                          I 24msec
                                          I   '
                                                      24msec I 24msec

                                     y                                    }

                                   time                            time

               (a)                                    (b)

             그림 5-12. Audio人油eO 신호의 丘as［祀 간격
                      (a) 30k也 fr nt1묘也 Vida) 뵤gnal
                      (b) 41.67 Hz frame rate audio 敬gnal
MPEG 시스템



           우 p-I丘cture는 디코딩을 먼저 하지만 디스플레이는 B-picture 다음에 해
           야 하기 때문에 pm와 D四값이 다르며 B-pictu肥의 경우는 디코딩된
           후 곧바로 화면에 디스플레이해야 하므로 pm 와 DTS가 갇다. Audio
           frame의 경우에는 매 frame의 데이터가 디코딩하는 즉시 스피커로 내보
           내야 하므로 PTS와 DTS의 값이 갇으며, 별도의 DTS값을 보내지 않고
           1nS값을 DTS로 간주한다．


           0PTS(Presentation Time Stamp)

            pm는 디코딩된 access unit이 재생（presenta如n）되는 시점을 나타내는
           값으로서 앞 절에서 기술한 I끄'S와 마찬가지로 system cit乂k frequency의
           1/300단위의 클럭으로 표현한 것인데 계산 방법은 식 (5.30）과 같다．


                   one TS packet      one TS packet          one TS packet




                 PID   PES stream   PID    PES stream      PID   PES stream

                                                                                      /
                                                                                          /
                                                                                              //
                                                                                            /

                                                                                          / / / //
                                                                             /        /


                                                                     .   '       夕／
                                                                                               /




                                                              /'current frame start code

                    DTS


                               previous frame data         current frame data
                                                       가
                 PES header          PES payload (element出y stream)

                                      one PES packet

                                          (b)

                  그림 5-13. TS packet고｝ de坦dcetized돈i lS mket으J 더］이터 내용
                           (a) TS packet
                           (b) depacketied packet(PES pa寸［et)
                                                                                      5, 시스템 목표디코더 모델


                                                                                                                  그U
                                                                                                                       0
             PTh(j) = (Q艸7刃1C勿ckfi芭quency X tp助DIV 300) % 233
                             )
                                                                                                          <
                         /
                                                                                                      U
                                                                                                              1




 , n田는 DTS와 마찬가치로 PES packet header부분에 있는데 vrs는 그
 PES pa火et의 유료부하 부분에 반드시 있게 되는 psc@ictum s啣tcod이로부
 터 시작되는 한 acx兀ss unit의 비디오 데이터를 디코딩한 후 디스플레이
해야 하는 시간을 알려준다. 만일 PES packet의 유료부하에 psc가 여러
 7뀨 있는 경우에는 처음으로 나타나는 picture start code를 대상으로 한다．
 그러나 일반적으로 PES packet의 길이가 가변적이며 TS packet보과 훨씬
 길지만（최대 65535byte) 이는 압축된 한 picture缸a보다는 작기 때문에 그
 림 5-14와 같이 pictu肥1의 데이터는 보통 두 개 이상의 PES packet어］ 걸
．쳐서 존재하게 된다． 또한 그림에서와 갇이 picti此2의 시작부호인 1乂s2
는 유료부하의 중간 부분에 있을 수 있다. 일반적으로는 vrs의 값이 모
든 picture에 있는 것이 아니고 DTh와 마찬가지로 최대 0.7sec 이내에 전


            one PES packet                                                 one PES picket
      .4
                                          header
           header
               )    <
                        payload       I
                                          i   .
                                                  payload
                                                                                            payload


                                                            PI'52,       1ItL
                                                            DTS 2:       卜瓣鞋子1




                                      까clure / data
                                                                           1
                                                                肛eture 2 data




                                      m                        m




                                  <
                                              難難聲 蠶難難簧難難藝賈
                                                                     (psc:picture start code)

     그림 5-14. VId心） PES pacl라S고｝ 관련된 elerr比ntar3r Sbeam bt寸fer의 내용
MPEG 시스템



           송되는 것으로 규정하고 있으므로 태부분의 picture에는 없을 수가 있다．
           이 경우에는 디코더에서 system C1(乂k을 분주하여 vrs를 만들어내야 한
           다. PBS packet의 유료부하 내용은 곧 elemenaliy stream이므로 그림 5-14
           에서와 같이 각각에 해당하는 pictui data는 PBS packet에서 분리된 후
           video elemenatty sti跏Ti加脆r어］ 저장되어 디코딩을 기다리게 된다．

              TS stream
                                                 1
                                                 decoder clock recovery block                    10
                                                                                                 audio丘Jideo
                                                                                                 Co刀i／兀Zr口b7r
             TS stream                                          PCR counter
             depacketizer                                       lower 33 bits

                                                                                                     mH
                                                                                                      m
                                                                                                          J
                                                                                                      V

                    口udio ／기므S stre（刃n
                                           ele刃妃ntary stre口m
                                                                  decoded stream

                          audio PES                elementary stream             decoded            D/A
                  J和                                                         ,
                          depacketizer
                                            二＋
                                                   buffer & decoder
                                                                         1
                                                                                 stream    나1+
                                                                                                    amp! H+
                                                                                 memory             speaker



                          audio PTS                audio
                          extraction               comparator          presentation
                                           H十
                                                                       釘口rt sign口／


                                                                PTS 甘                             sound music
                                                                                                  &




                                                                                                           11
                     ideo PES stream                                                              picture
                                                                                                                J

                                           ele刃妃ntary stream
                                                                  decoded stream

                    니＋   video PES    _L.. elementary stream                     decoded          D/A
                         depacketiZet      buffer & decoder
                                                                             戶   stream           matrixing
                                       1
                                                                                 memory           monitor
                                   1
                               +
                         너deo PTS                 video
                         extraction               comparator        presentation
                                                                    計口rt sig兀口／


                                                               P1'S V

                             그림 5-15. 1玎S. PCR 및 elementary stream의 재생
                                              5. 시스템 목표디코더 모델


 vrS는 D四와 마찬가지로 PCR에서 나타내는 시간값을 기준으로 하
여야 의미가 있게 되는데 이 콰정을 그림 5-15에 도시하였다. 그림 5-15
에서 PCR값은 TS stream에서 분리되어 하위 33비트만을 P15를 위한
기준값으로 만들어낸다. P15값은 PES packet header어］ 있으므로 audio!
너deo PES depacke血er를 거치면서 header부분의 vrs와 유료부하 부분의
audio/video elemen啣y stieam이 분리되어 각각의 버퍼에 저장될 것이고
                                             이
데이터는 DTS에 맞게 디코딩된 후 au小아vid的decoded men枸口에서 재생
(prese恤tion）되는 시점을 기다리게 된다. Audio/vid凹corn叫砒아는 수신된
旦udio加id凹의 P15와 PCR의 하위 33비트를 비교한 후 서로 같아지는
시점에서 presen毗on start signal올 만들어준다. I뇨se恤tion sta式sign띠에 맞
추어 디코딩된 스트림들은 각각 재생되는데 오디오 신호는 D!A 앰프를
거쳐 스피커에서 재생되며 비디오 신호는 D/A 앰프등을 거쳐 모니터에
서 디스플레이된다．
 Sm 모델에서는 디코딩시간을 0으로 가정하므로 만약 디코딩된 데이
터가 그대로 재생된다면 V心의 값과 DTh의 값이 동일하므로 인코더에
서는 P15만 전송하며 P15만 있는 access ui血은 디코더에서 이 I汀'S를
DTS로 간주한다. 예를 들어 B_pic曲re는 디코딩 즉시 디스플레이되므
로 I江'S만이 전송되고，I_picture나 므picture는 디코딩된 후 디스플레이되
기까지 일정시간을 기다려야 하므로 vrs와 D心7} 동시에 천송된다．
FF5와 DTh를 모두 고려하는 디코더의 전체 블럭도를 살펴보면 그림
5-16과 같다.


0 비디오 스트림에서 DTS의 발생방법

 入4PEG2 시스템 파트에서는 DTS값을 만드는 수식과 다음 DTS까치의
시간간격 및 D'TS 의미를 설명한 것이 전부이기 때문에 DTS를 어떻게
만들어 줄 것인가에 대한 구체적인 언급은 없다. 본 절에서는 DTS를
만드는 한 방법을 생각해 보기로 하는뎨 다른 접근방법도 있기 때문에
시스템 인코더 설계자, 혹은 卜4PEG2 프로그램 제공업자는 구현시스템
의 안정도에 따라 좀더 정교한 DTS를 만들 수도 있을 것이다．
MPEG 시스템



           TS stream
             1
                                  decoder clock recovery block
                                                                                           (O띤크如吻C口威ng,
             1
             1
             中
                                                                 F丁S_a F丁S_v               d凸끄lay control
                        PCR                                                            ]   b勿以
           TS stream                    PCR counter
           depacketizer                 lower 33 bits            DTSa t珪Sv
                                                                                       戶   //) tU닢加｝ a71戶，l,J.
                                                                                                             ,1．』1
                                                                                           （如p！口y con幷可
                                                                                           block

                 audio 尸ES 計rea刃i
                                elementary stream
                                                                  d配O(屯／stream




                                                                                                               T
                                                                             decoded               D/A
                     audio PES   r, elementary stream                    +
                              .      H느戶
                                                ;                            stream         -
                                                                                                   amp/
                                    ［乂ijier （又 uecuuer
                                                    1
                     uepacKeu乙er
                                                                    H:
                                             1    nr   n


                                                                             memory                speaker



                    PES                  audio docoding, di i口y co,出可
                    header
                           Y        ODTS a
                     audio                       comparator
                     PTS/DTS
                     extraction                                  comparator                요꺄ndmi玎ic
                                        1

                                      片叩Sa                                                 &
                                                                                           PLC九ire




                                                                                                       T
                                                                                   J


                                                                             艱
                                                   DTSj
                 video ／기呱 釘ream
                                elementary stre口刃i
                                                                  d配仇奴／stream

                                                                                 decoded          D/A
                       video PES H           elementary stream                   stream                     H+
                                                                                                  matrixing
                                                                                            m1+

                       depacketizer          buffer & decoder
                                                                                 memory           monitor



                     PES                    쁘奭Moc口幻ng, 山：SI,／口y contr아
                     header         ODTS V
                       video                >comparator
                       PTS/DTS
                       extraction                                comparator
                                     OPTS V
                                                                                   J




                              그립 5-16. Deixxler s邪奴TI의 전체적QJ 블럭도
                                              5, 시스템 목표디코더 모델


 DTS는 video ele毗ntary stream에서 vbv_delay와 유사한 개념을 갖는다．
비디오 디코더에서 버퍼를 조절하기 위하여 비디오 인코더에서 picture
header부분에 V山뗘elay값을 전송하는데 이는 디코더에서 picture start code
를 검출한 후 vbvdelay 시간동안 기다리면 디코더의 버퍼가 인코더에
서 가정한 버퍼레벨에 맞게 된다. 마찬가지의 원리로 시스템 인코더에
서는！邱packet을 만드는 과정에서 PES pa火et header부분에 DTh의 값올
넣어주는데 이는 디코더에서 디코딩시간을 조절하여 시스템 디코더 버
   ]   을 시스템 인코더에서 가정한 레벨로 맞추기 위함이다. rideopES
packet의 header부분에 필요에 따라 추가하는 DTS는 video elementary
sneam에서 vbv코elay를 참조하여 만들 수 있다. 다른 모든 elemen啣y
simam의 경우에도 DTS 정보가 삽입되는데 시스템 디코더에서는 각각의
DTh를 기준으로 하여 모든 elementa玎stream 디코더의 버퍼를 조절한다．
비디오 데이터의 경우 vbv셔elay는 video sequen（无 header를 포함하여 각
pi艾urn header의 시작인 picture start code까지 검출한 후 디코더에서 이
p奴urn를 디코딩하기까지 기다려야 하는 시간을 의미하므로 시스템 인
코더에서 I끄S를 전송해야 하는 시점이 오면（최대 O.7sec 이내） PES
packetizer는 유료부하 부분에 picture start（刃de를 포함하도록 패킷화하면서
picture sta八code 뒤에 있는 vbvdelay값을 참조하여 PES header어］ DTS를
만들어 삽입한다.
 그런데 DTh는 90KHz로 표현되며 vbv코elay도 90KHz의 단위로 만들
었기 때문에 상대적으로 어렵지 않게 만들 수가 있으며 DTh는 유료부
하에서 처음 시작하는 ac四ss unit의 디코딩시간을 알려주므로 vbv느delay
와 같은 개념이라고 볼 수 있다. 따라서 비디오 데이터가 시스템 인코
딩을 거친 후에는 I玎.5의 값이 V加Jelay의 의미를 대신할 수 있다. 따
라서 식 (5.29）의 td.(j)는 식 (5.31)과 갇이 표시될 수 있는데 여기서 t(j)
는 J번째 byte가 Si]）로 입력되는 시점이고, J번째 by妃는 access unit어］
해당하는 S切抗c어妃의 첫번째 可te이다．

                                                                  l
              屹(j) := 劤 + (v加H比切／90000) sec                 八4U
                                                        <
                                                                              \
                                                                          1
                                                                      1
                                                    U
                                                                  /
MPEG 시스템



           1 시스템0私J의 시간정보 및 PSI의 발생시기

                   시간에 관련한 정보인 PCR, SCR, ESCR, DTh, VFS 등은 자주 전송을
           하면 디코더에서 원래의 의도한 목적을 수행하는데 유리할 것이나 이
           는 전송 정보량이 많아치는 단점을 초래하므로 일정한 시간을 규정해
           서 이 시간 내에 다시 천송하도록 入'JPEG 시스템에서는 명시하고 있다．
           이와 같은 시간정보들을 일정한 시간 내에 다시 전송하도록 하는 이유
           는 시스템 디코더에서 임의시간에 시스템을 ON시켰을 때 디코딩할 수
           있도록 하기 위함인吼艮R값은 최대 0.1초． SCR尼SCRIPTS/DTS는 최대
           0.7 초, PSI정보는 최대 0.7초 이내에 재전송하도록 규정하고 있다. 수신
           단에서는 임의 시간에 사간정보의 값들이 필요할 수 있는데 이 경우에
           는 시스템 디코더에서 내삽佃啣刻ation）하여 사용한다. 그러나 PSI정보
           는 내삽할 수 없다. TS stream을 수신하여 디코딩한 스트림을 화면에 디
           스플레이하기까지의 시간은 PSI정보, PCR값을 이용한 시스템 디코더의
           C1(乂k recovely, PTS/DTS= 정보의 선정등을 필수적으로 거쳐야만 하는데
           이와 같은 정보가 각각의 최대 시간에 서로 임의대로 전송된다고 하면
               최소한 2초 이상의 지연이 생기게 된다. 인코더 시스템에서는 디코더에
           서의 지연시간이 가능한 적게 걸리도록 스트림을 만들어 주어야 한다．




           卜            「』   ＞1B     p   " .   B」   21   -
                                                         .』   '   - -   I r IAI
                                                                        I   . c




               .    스플라이싱의 정의와 종류

                   두 개의 서로 다른 elememtary stream을 1-s stream상에서 묶어주는 것을
               스플라이싱이라 한다. 각각의 elemen啣y stream은 만들 당시 서로 다른
                                                    5. 시스템 목표디코더 모델




                                                            毗




      Input progr刀                         output program
      TS stream                            TS stre口刃i




                     그림 5-17. Spi岫垠의 개념도



시간에 서로 다른 곳에서 각기의 다른 목적으로 만들어진 스트림일 수
있다· 일반적인 프로그램이 스플라이싱되는 개념을 그림 5-17에 도시하
였다．
 한 개의 TSs的am이 연속적으로 전송되는 도중에 스플라이싱이 일어
나 다른 스트림 ' ] 끼워지는 경우 스플라이싱이 생기는
                                                    부분을 splicing




                                                                   芬
point라 한다· 이 斗小cing point는 결국 서로 다른 스트림의 경졔부분을
의미한다· 이러한 경계부분이 생기게 되면 시스템 디코더에서 디코딩시
불연속점 ' ] 생겨서 매끄러운 디코딩을 하지 못할 수 있는데 디코딩시
의 연속성에 따라 연속 스플라이싱과 불연속 스플라이싱으로 구분한다．
웰속 스플라이싱은 시스템 디코더에서 splicing point부분을 연속적으로
y코딩할 수 있는 스플라이싱을 의미하며 불연속 스플라이싱은 그렇지
몰한 겸우이다． 시스템 디코더는 연속 스플라이싱을 디코딩하고 재생하
는 과정에서 지연없이 자연스럽게 동작할 수 있지만 불연속 스플라이
싱에 대해서는 이와 같은 매끄러운 디코딩 및 재생동작이 보장되지 않                              箋饔．
                                                                     蠶薰畺
                                                                   姿：::::::：珌i：羅咎照斜踐守器표； :;::::::;:::;:::：發；
                                                                                       裝牡；
                                                                   多：妊珏妊坪可汗汗舟交吐恥：::：兮泌코妊妊妊薑妊8丘｝戶：

는다.
                                                                   好蛋發器發發
                                                                   轟蠶難難難蠱難箋難繫難難
                                                                         驪難蘿難難難驪蘚轉娜難i
                                                                         熙三娜藿雄蒡聯難攝湃瀜轟器轟藿難難幾藿藝．三
                                                                        難難難蠶難難難蠶難蠶
                                                                        i::;：弦：:；汗斗F:；坪：;:::;:::::::::：萍：::::::::::::::::：滓：妊妊a妊妊妊：;;;:;:;:::::;:;:4




                                                                   斗好gmi
MPEG 시스템



           0 스플라이싱에 대한 정보

            하나의 Th sbemn이 전송되던 도중 스플라이싱이 일어나는지에 대한
           정보는 TS packety header의 adapt的onal fie닢부부에서 알려준다. Splice_
           countdown은 1-s stieam 상에서 스플라이싱이 생기는 위치를 알려주는 값
           으로서 그림 5-18과 같은 의미를 갖는다. 그림 5-18은 入포只 프로그램
           도중 광고가 삽입되는 스플라이싱이 발생하는 경우의 splicing的nt 및
           splic乞凹untdown의 예를 도시한 것이다. Splice_凹untd이wn은 양, 음의 정수
           값을 가지며, 양의 값은 현재의 TS packet으로부터 sp11出rig poii止까지의 남
           은 TS packet 수를 나타낸다. 음의 값은 스플라이싱이 발생한 후, splicing
           m奴부터 경과한 Th packet의 수를 나타낸다. 이와 같은 spli（无Hq沁nt面Wll
           의 값은 시스템 디코더로 하여금 splicing p이nt의 전, 후 위치를 알려줌으
           로서 디코딩 및 재생시의 적절한 동작을 수행하도록 한다．


                                            TS packet


                 splice countdown                                 splice 口7l口ztdown



                                                              1

                  sport program         commlercial program         sport program
                                                                     (continued)




                                    \               /
                                          splicing point

                         그립 5-18. Pmgram 삽입시의 spli _ （刃untdown의 011
                                       6. PES 패킷의 신택스와 의미




                           PES 패킷의
                          신택스와 의미




  PES packet은 header와 유료부하（pa加ad）로 구분되는［카 유료부하 부분에는 이ementary
stream 또는 사용자 데이터로 채워지며 PSM, PS[) 및 일반 PES packet으로 나눌 수 있［:}.
MPEG 시스템




           PES packet의 계층적 구조는 그림 6-1과 갇고 자세한 내용은 표 6-1고干
           같다．



                      packet
                                    PES    opt幻nal
                      start  stream
                                    packet PES              PES packet data bytes
                      code   id
                      prefix        length HEADER



                                                                                            1\
            寸／/




                                                                        PES
                PES                 data
                           PES                          origin띠         header optional stuffing
            '10 scrambling priority alignment copyright or
                  '                                             7 flags
                                                                        data   fields
                                                                                        bytes
                control             indic欲or               copy                         (OxFF)
                                                                        length
              2     2         1          l       11        1／ 尸 낸卜／죵／                       m8



                                                    DSM                previous
                           驃      ESCR
                                         E므，
                                                    trick
                                                    mode
                                                            additional
                                                                       PES
                                                            copy info CRC
                                                                                PES
                                                                                extension


                             好芻
                                    42         22




                                    pack                   PES
                             PES           program
                             pnvate header packet   P-sm extension PES
                                                                   extension
                                                    buffer field
                             data   field  seq cntr                field data
                                                           length
                                         8           8        6
                                                              l        n1J
                              128

                            그림 6-1. PES packet syntax diagram(MP표（; IS: Figure F-2)
                                                               6. PES 패킷의 신택스와 의미


 이 PES packet의 header부분은 bitstre出n어］ 따라 크게 서］ 가지 형태로
구별되는데 小ti-earn_id가 'padd血且stream' 인 경우에는 정보가 없는 단순
한 덧붙이기（padd加g）에 이용되며 이때 그림 6-1 의 맨 위에서 optional
PBS HEAl兆R와 PBS packet data by把S부분은 모두 padding寸bytes로 채워
진다． 두 번째로 stream_id가 pmgram小stream中map, ECM, EMM, program_
stream_di叱ctoiy, DSMCC_streani, 1TU-T Rec. R221.1 type E-stma可표． 6-2
참조）중의 하나인 경우에는 그림 6-1의 . optional PBS HEADER와 PBS
packet data bytes부분은 모두 유로부하로 채워진다. 마지막으로 stream_id
가 위의 어느 경우에도 속하지 않으면（주로 오디오와 비디오： 표 6그
참조） 그림 6-1의 optional PBS HEADER부분은 그림에서 표시된 것처럼
여러 가지 필드로 구성된다．
 Progmms配跏n_map과 I斗ogral心t妃am_directo日어］ 대해서는 6.2절과 6.3
절에서 설명한다． !' "n                       PgD


                       표6-1. PES packet(MPEG Is: Table 2-18)




PES_packet() {
     packet_start_code_prefix
     stream id
     PES_packet_length
     氓 S毗缸n id 느 programstreammap
     && s配am id 느 padding_stream
     && streamjd 느 privatr乙stream그
     && stream_id 느 ECM
       M
        stream id h= E入M
     && stream_id != pmgram_stream_directo口                            如
     && stream id != DSMCC stream                                            丁" 七 [
                                                                               h
                                                               cc 'I
                                                                               J
     && stream_id 느 ITU-T Rec. H.222.1 ty伏日毗帥泮／6此＼       j.
                                                                       n
                                                                       乙
                 '10'                                                  2 bslbf
                                                                       八
                                                                       乙
                 PES_scrambling_contml                                 2 bslbf
                                                                       l
                 PES尸priority                                          I bslbf
                                                                       l
                 data_alignment_indicator                              1 bslbf
                                                                       l
                 copynght                                              1 bslbf
                                                                       l
                 ori멈nal_or_copy                                       i bslbf
                                                                       八J乙
                 PTS_DTS_flags                                         2 bslbf
MPEG 시스템



           ESCR_flag                     1    bslbf
           ES_rate_flag                  1    bslbf
           DSM_tnck_m油_flag              i    i:川bf
           additional_copy_info_flag     I    bslbf
           PES_CRC_flag                  1    bslbf
           PES_ex把nsion_flag             1    bslbf
           PES_header_data_length        8    uimsbf
           if (丁S_DTS_flags =='lO') {
                   '0010'                 4   bslbf
                   FT'S [32..30]          3   bslbf
                   marker bit             1   bslbf
                   Fl'S [29..15]         15   bslbf
                   marker bit             1   bslbf
                   1玎S[14. .O]           15   bslbf
                   marker bit                 bslbf
           }
           if (FFS_DTS_flags =='l 1' )
                   '0011'                 4   bslbf
                   Fl'S [32.30]           3   bslbf
                   marker bit             1   bslbf
                   Fl'S [29..15]         15   bslbf
                   marker bit             1   bslbf
                   Fl'S [14..0]          15   bslbf
                   marker bit             1   bslbf
                   伉nrH                   4   bslbf
                   DTS [32..30]           3   bslbf
                   marker bit             1   bslbf
                   DTS [29..15]          15   bslbf
                   marker bit             I   bslbf
                   DTS [14..0]           15   bslbf
                   marker bit                 bslbf
           }
           if (ESCR_flag=='l') {
                  reserved                2   bslbf
                  ESCR_base[32..30]       3   bslbf
                  marker bit              1   bslbf
                  ESCR_base[29..15]      15   bslbf
                  marker bit              I   bslbf
                  ESC나：)ase[ 14..0]      15   bslbf
                  marker bit              1   bslbf
                  ESCR extension          9   uimsbf
                  曲八e汕                    1   bslbf
                                                          6. PES 패킷의 신택스와 의미



if (ES_rate_flag == '1') {
        marker bit                                           I bslbf
        EState                                              22 uimsbf
        marker bit                                           1 bslbf
}
if (DSM_thck_m넜e_flag == 'I') {
        trick mode control                                   3   uimsbf
        if ( tnck_mode_control == fast_forward) {
               field id                                      2 bslbf
               intra slice refresh                           1 bslbf
               frequency_tmncation                           2 bslbf
         }
        else if ( trick_mode_control == slow_motion) {
               rep_cntrl                                     5   uimsbf
         }
        else if (trick_mode_control == freeze_frame) {
               field id                                      2 uimsbf
               reserved                                      3 bslbf
         }
        else if ( trick_mode_con甘ol == fast_reve八e) {
               field id                                      2 bslbf
               intra slice refresh                           1 bslbf
                frequency_tmncation                          2 bslbf
        else if ( trick_mode_control == slow_reverse) {
               rep_cntrl                                     5   uimsbf
         }
        else
               reserved                                      5   bslbf
}
if ( additional_copy_info_flag == '1') {
          marker bit                                         1 bslbf
        additional_copy_info                                 7 bslbf
}
if ( PES_CRC_flag == '1') {
        previous_PES_packet_CRC                              16 bslbf
}
if ( PES_extension_flag == 1') {
        PES_priva把data뇨flag                                  1   bslbf
        pack_header_field_flag                               I   bslbf
        program）缸：ke냐equei准下ou毗r_flag                        1   bslbf
        P-S1T1工bu娩r_flag                                     1   bslbf
        reserved                                             3   bslbf
        PES_e岫ens幻n_flag그                                    1   bslbf
MPEG 시스템



                              if ( PES_pnvate_data_flag == '1') {
                                     PES_private_data                         128 bslbf
                              }
                              if (pack_h出er_field_flag == '1') {
                                     pack_field_length                         8 uimsbf
                                     pack_header()
                              }
                              if(progran나）acke匕텍uen此下叫恤flag == 4X
                                                                                1
                                                                                l
                                     marker bit                                     bslbf
                                                                                거
                                                                                ／
                                     pmgram_packet_sequence_c刈nter                  uimsbf
                                                                                d
                                                                                l
                                     marker bit                                     bslbf
                                                                                1
                                                                                1
                                     入4PEG1 入狂'EG2 identifier                       bslbf
                                                                                /
                                                                                O
                                     original_stuffJeng出                            uimsbf
                              }
                              if ( P-STD_bu拜er_flag == '1') {
                                     '01'                                      2 bslbf
                                     P-STh_buffer_scale                        1 bslbf
                                     P-STh_buffer_size                        13 uimsbf
                              }
                              if ( PES_extension_flag_2 == ' l '){
                                     marker bit                                1 bslbf
                                     PES_extension_field_length                7 uimsbf
                              for(i=0;kPES_extension_field_length;i-i-t-) {
                                                                                8
                                     reserv(넜                                       bslbf
                                     }
                              }
                      }
                     for (i=O;i<NI i-i-+) {
                              stuffing.byte                                    8 bslbf
                      }
                     for (i=0;kN2;i十卜） {
                              PES寸packet_data_byte                             8 bslbf
                      }
           }
           else if (stream_id = pm留am_stream_map
           II streamjd == priva把夕mam그
           II stream id == ECM
           卄 stream id==EMM
           I, S仕eam_id == pm留帥鉀eam dii耐이y
           II stream id == DSMCC_stream)
           II stream id==ITU-TRec. H.222.1 ty思Estream {
                         如r (i닉）,i<PES_packet Jen帥；奸＋) {
                                                                                8
                                PES_r吼ket코跏小yte                                     bslbf
                                                      6. PES '41킷의 신택스와 의미



                  }
       }
       else if ( stream_id == padding_stream) {
                      化d i닉);i<PES_pack吃length針＋) {
                                                            8
                         padding_byte                           bslbf


       }
 }


packet_start_code_pefix : 24bits
     · "（刃伉）仗）伉) (刃어）伉$30 0000伏$31" (00C乂）01(H))

     ·packet start code(32bits）는 packet日start뇨code_肛efix와 stream_id로 구성
       된다．

stream Id : 8bits
     · 표 6-2와 갇이 elementary stream의 타입과 번호를 나타낸다．

PES_packetJength : l6bits
     · 이 변수의 마지 -t            yte 바로 다음부터 PES packet 끝까지의 byte수
     .0값은 PES packet의 유료부하（p町load）가 비디오 elementa口 Snemn이
      고. TS pa味et으로 전송되는 경우만 허용되는데 그 뜻은 길이가 정
      해지지 않았거나 또는 범위가 한정되어 있지 않다는 뜻이다．

PES_scrambling_control : 2bits
     · PES packet 유료부하의 스크램블링 모드를 결정한다（표 6-3).
     · 그림 6-1의 PES packet header와 optional 丘elds는 스크램블링하지 않
      는다．

PES_p如rity : ibit
     ·if ("l") : 그 PES packet의 유료부하 부분의 데이터가 PES_priori口 =
      "0" 인 유료부하들보다 우선순위가 높다는 것을 의미
       O] 변수값은 1S stiam을 처리하는 과정에서 변경될 수 없다．
MPEG 시스템



                              표． 6-2. Stream id ad inents(MPEG Is: Tab1e2-19)

                     stream id               Note                      dream co竝ng

                     1011 1i00                 l         program_s的m_map
                     10111101                  2         priva妃1요ream1
                     10111110                           padding_stream
                    1011 1111                  3        priva把_stream_2
                     ll0xxxxx                           ISO/IEC 13818-3 orISO/IEC 11172-3 audio
                                                        stream number x xxxx
                    1110 xxxx                           ITU-T Rec. H.262 I ISO/IEC 13818-2 or
                                                        ISO/IEC 11172-2 video stream number xxxx
                    11110000                  3         ECMstream
                    11110001                  3         EMMsueam
                    1111 0010                 5         1TU-TRec. H.222.0IISO/IEC 13818-1
                                                        AnnexAorISOf1EC 13818-6 DSMCC stream
                    11110011                  2         ISO/IEC 13522 stream
                    1111 이00                  6         ITU-TRec. H.222.1 type A
                    1111 0101                 6         ITU-T Rec. H.222.1 type B
                    11110110                  6         ITU丁Rec. H.222.1 type C
                    11110111                  6         ITU-TRec. H.222.1 type
                    1111 1000                 6         ITU-TRec. H.222.1 typeE
                    11111001                  7         anc寸1aly寸stream
             11111이0절 1111 1110                         reserved data stream
                    1111 1111                 4         programstreamdi七Ct아y

           The notation x means that the v出ue '0' or '1' are both permitted and results in the same stream
           type.
           띠陀 S的am num比r is 曾yen by 毗 values 趾en by the 乂5.
           Note 1: PES pack毗 of ty四 p畔l帥小跏兀dii叱Ct呵 have unique sy岫x sr比師ed in 6.3.
           Note 2: PES packets of type p加毗皿ream1 and ISO/if兀그3552_st呻m follow I如 跏iie PES
           packet syntax as those for ITU-TRec. H.222.0 I ISO/IEC 13818-2 video 可｝d ISO/LEC 13818-3
           audio streams.
           Note 3: PES packets of type priva虹st跏_2, ECM_strearn and EMM_stream are similar to
           private_s打eam_i except no syntax is specified a匕r PES中packet_iength field.
           No把 4: PES packets 可type program誼eamH幽呵加口 t咀ye a unique sy恤x 畔cified 沇6.3.
           Note 5: PES packets of type DSM-CC_stream have a unique syntax specified in ISO/IEC
           13818- 6, which is a compatible extension of ITU-T Rec. H.222.0 I ISO月EC 13818-i An妃x A.
           Note 6: Ths streamid is associated with streamHtype 0x09 in table 6-8.
           No把 7: liii外岫帥1 idi印fly used in PES packets, w川ch cany 山姐 加ma Program 鈿eam or
           an ISO/IEC 11172-1 System Stream, in a Transport Stream.
                                                          6. PES jl뷰1킷의 신택스와 의미


           그림 &3. PES ＄그ambling conth丑 valu心伍1PEG Is: Table 2-20)


                    ＼刎뇨e                  Description

                       00                 not scrambled
                       01                 user defined
                       10                 userde丘ned
                       11                 user defined



data_allgnmentJndicator : ibit
  · if("1") : PES packet hea：뇨r 바로 다음에 video start code 또는 audio
    SyI乂＼V아d（또는 다른 start code가 올 수 있는데 이에 대해서는 247 참
    조）가 따라온다는 것을 의미 . 보통 이 flag이 1 이면 표 9-8의 data
    stream alignment descriptor가 전송되는데 만약 이 descriptor가 전송되지
    않으면 표 9-9와 표 9-10의 au卽ment_ty光의 값은 아（H）로 가정한다．
  ·if ("O") : 따라올 수도 있고 아닐 수도 있다．
  · 이 alignment는 표 9-9에서도 알 수 있듯이 작게는 slice 단위로도 맞
    출 수 있기 때문에 하나의 access unit이 여러 개의 PES packet으로
    나뉘어쪄 패킷화되어도 얼마든지 alignment를 시킬 수 있다. 따라서
    보통의 경우 data_alignmentjndicat야는 1 이지만 특수한 경우에는 이
    와 같은 alignment를 주지 않을 수도 있다．

copyright : ibit
  · if("l") : 그 PES packet의 유료부하가 특허퀀을 갖고 있다는 것을
    뜻한다．
  · if("O") : 특허퀀을 갖고 있는지 없는지 모른다．

origin出1or尸-copy : ibit
  · if("l") : 그 PES packet의 유료부하가 원본임을 나타낸다．
  · if("O") : 카피본임을 나타낸다．

PTS_DTS_flag : 2bits
  · if("lO") : V's 정보가 PES packet header어］ 존재 한다．
  · if("ll ") : I江'S와 I끄'S 정보가 PES packet header어］ 존재한다．
MPEG 시스템



                .' if("OO") : 꾀［S도 DiS도 PES packet head虹에 존재하지 않는다．
                ·01" 값은 사용금지

           邱CR丑ag : ibit
                                             畑
                ' if("l") : ESCR 청           畔
                                     } PES packet header어］ 존재한다．
                · if '0't) : 존재하지 않는다．

           ES_rate_flag : ibit
                ' if("1") : ES_rn把가 PES packet header에 존재한다．
                · if("O") : 존재하지 않는다．

           DSM_trick_mode_flag: ibit
                ' if("l ") : trick mode 정보（8bits）가 존재한다．
                · if("O") : 존재하지 않는다．

       addition시_copy_info_flag : ibit
                ' if("l ") : addi如nal_copy_info가 존재한다．
            · if("O") : 존재하지 않는다．

       PES_CRC_flag: ibit
            ' if("l ") : CRC 정보가 존재한다．
            · if("O") : 존재하지 않는다．

       P11요e地nsion_flag : ibit
            ' if("l") : PES ex把nsion이 PES 恥cket header에 존재한다．
            · if("O") : 존재하지 않는다．

       PES_header_d虹le唯eh : 8bits
                    이 변수 바로 다음부터 PES_packet data누by把 ‘ 바로 전까지（卜n개의
                1




                    stuffing by妃 포함）의 by妃수

       m針ker_bit : ibit
            1       tIl? I



            ' 0이 졔속되는 것을 막기 위해서 데이터 중간에 삽입된다．
                                                      6. PES 패킷의 신택스와 의미


PTS(p七Sentation 血lle stamp) : 33bits
  .5장에서 설명된 pm값을 여기서 전송

          PTS(k) = ((system_clock加quency X tp,(k)) DIV 300) % 233

  .0이 계속되는 것을 방지하기 위하여 표 6-1 처럼 중간중간에 marker
   Hbit삽입

DTS(decoding time stamp) : 33bits
  .5장에서 설명된 DTS값을 여기서 전송

           DTS(J) = ((system_clock斤equency X tp,(j)) DIV 300) % 233

  .0이 꼐속되는 것을 방지하기 위하여 표 6-1처럼 중간중간에 marker
   1bit삽입

ESCRHbase; ESCR extension : 44bits
  ·앞에서 발생된 ESG目base와 E舡R_e玳ension값을 여기서 전송

        ESCR_base(i) = ((system_clockjrequency * t(i)) DIV 300) % 233
        ESCR中ext(i) = ((system_clockjrequency * t(i)) DIV 1) % 300
        ESCR(i) = ESCR_base(i) X 300 + ESCR_ext(i)

  .0이 계속되는 것을 방지하기 위하여 표 6-1처럼 중간중간에 marker
   1bit삽입

ES_rate(elementary stream rate) : 22bits
  . PES stream만을 생각할 때 s-fl）가 PES packet을 받는 byte율
  · 새로운 E＆茹妃값이 주어지기 전까지는 갇은 stream의 계속되는 PES
    packet들에서 이 값은 유효하다（그러나 갇은 PES stream에서도 극단
    적으로 packet마다 값이 바뀔 수 있다）.
  . 50bytes/second 단위로 계산（즉 ES_rate = 10이면 초당 500byte의 PES
    stream을 받는다는 것을 뜻함）
  .0값 사용금지
MPEG 시스템



             · 이 값은 PES-STI）뿐만 아니라 P-STI）의 입력단에서 PES stream의
                 切rte들이 도착하는 시간을 계산하기 위해서 사용될 수 있다．

           trick mode control : 3bits
             · 해당 video elementa口 stream에서 표 6-4와 갇이 어떤 trick m어把가
                 사용되는가를 나타낸다（다른 종류의 elementary stream에서는 이 변
                 수와 바로 다음의 5bit는 사용되지 않는다）.
                 trick mode가 선언되지 않으면 디스플레이되는 picture수는 ISO138l8
             1




                 -2(MPEG2 너deo）에서 정의한대로 re 尤at如st_field와 top_field_first값에
                 따라 다르게 된다．
             1
                 trick n好Je가 선언되면 디스플레이되는 picture수는 각 trick mode마
                 다 달라진다（뒤의 fie넌id와 rep叫c이山o1에서 설명）.
                 thck-mo把 con汀이값이 변하거나 trick n似le가 끝나면 다음과 같은 불
                 연속이 발생할 수 있다．
                 a) time base어］ 있어서의 불연속
                 b) 디코딩의 불연속
                 c) continuity counter의 불연속


                         K 6-4. Trick mode antml values(MPEG Is: Table 2-21)


                                ＼刎뇨e                   Description

                                  '000'                fast forwaid
                                  '001'                slow motion
                                  '010'                freeze frame
                                  '011'                fast reverse
                                  '100'                slow reverse
                               '101-1111'              reserved


             ·trick mode에서는 slice구조가 유효하지 않을 수 있으며 다음과 같은
                 변수 값들도 올바른 값이 아니기 때문에 디코더는 이 값들을 사용
                 해서는 안된다．
                                                              6. PES 패킷의 신택스와 의미


    a) bit_rate
    b) vbv_delay
    c) iepeat_frist_field
    d) v_ax蛇四師이l
    e) field_sequence
    1) su比an把r
    g) burst_amplitude
    h) sut兀amer下hase

field id : 2bits
  · 어떤 m넌를 디스플레이 해야 하는가를 나타낸다（표 6-5).


              표6-5. Field id field cont刃l values(MPEG Is: Table 2-22)


                   Value                 Description

                   '00'          display from top field only
                   '01'          display 加m bottom field only
                   '10'          display comple妃 frame
                   '11'          肥served


  · 해당 field는 이 field_id를 포함하는 PES packet에서 시작하는 pictuIe
    을 말한다．
  · 만약 유료부하가 없으면， 해당 fie넌는 가장 가까운 바로 전 pictu肥
    가 된다．

intra slice ref心h : ibit
  · if("l") : 入4PEG2 비디오의 most general slice구조에서는 slice 사이의
    macn力k乂k들이 코딩되지 않는 경우가 있는데（예를 들어 fast니forward
    나 fast爬ye心e의 경우） 이 PES packet의 slice 데이티 사이에 이렇게
    코딩되지 않은 m町小娩k이 있다는 것을 표시한다．
  1if("O") : 그렇지 않다．
  · 디코더에서는 없어진 macmbli乂k을 그 전 decoded pic汕e의 동일한
    위치에 있는 macrobk兀k으로 대치할 수 있다．
           MPEG 시스템


                                       ·trickm어妃가 鈿t_forward나 fast_reverse인 경우에 쓰인다．

                                     frequenc寸truncation : 2bits
                                       · 이 PES packet의 비디오 데이터가 표 6-6과 같은 조건들로 제한이
                                         되어 있다는 것을 나타내기 위하여 쓰인다．


                                                     표 6떠. Cfficient 配I텨：仕)tl vah心(MPEG is: Table 2-23)


                                            \／刊［ue                           Descriplion

                                             '00'         Only DC cc玘伍c妃nts are non-zero
                                             '0l'         typi出ly only the first 曲ee c玘fficients are non-zero
                                             '10'         typic세y only the 丘匹t Si：乂 (X比術C妃nts are non-zero
                                             '11'         all c玘fficients may be non-zero


                                       ·trick mo扼가 fa鉅如rward나 fast爬verse인 경우에 쓰인다．

                                     rep_cntrl : Sbits
                                       · fleld(intelaced pic恤e인 경우）나 什ame(progressive picture인 경우）이 되


好聲蟹m量
                                         풀이되어 디스플레이되는 횟수를 나타낸다．
                                       · 0값은 사용금지
             幾聲瑟붚幾瑟i
    ：亨娜m
            在：::::::::：二i:;i：三：
                              三：
                               a：玉
                                       · progressire sequence인 경우 되풀이되어 디스플레이되는 picture수는
                                         디코더에서 출력되는 picture수를 N이라 했을 때 , (NXrepcn出）이
                                         되는데 trick mod乞cn出과 top-－丘eld1血5t(入WEG vid凹part의 변수）에 따
                                         라 다음과 같이 틀려진다．
                                          a) tnck_mode_cntrl = "slow motion" 인 경우
                                            비디오 신호가 MPEG1 또는 MPEG2의 ping七鹹妃 S欲私ence인 경우 해당
                                            picture는 (NX 1디兀cn出）번 반복된다.

                                            비디오 신호가 MPEG2의 in也riaced sequence인 경우 해당 picture의 각
                                             field는 (NXre仁cn出／2）번씩 반복된다（즉, 처음 field가 (N X rep_cntr112）번
                                             반복된 후에 두 번째 fie넌가 그후 (N X rep_ce甘V2）번 반복된다）. 그런데
 鱗驪醬．   蠶難驪難難賈
 辱如m如
 餐罐罐難聲難簿懿聲懿瑟變難．ii:.                          만약． 해당 picture가 frame picture인 경우에 幻p-玉eld如匹t = "1" 이면 top
 驪難難難難難難簾                                    field가 먼저 (N X rep中cnl콰2）번 반복되고 그 후 bottom field가 (Nx
 룔m難難難
                                                                            6. PES 패킷의 신택스와 의미


        'tp_cn出／2）번 반복된다. 반대로 top_field_first = "0" 이면 比盛om field가 먼
        저 반복된다．

      b) thckjnode_cn甘1= "slowm아ion" 인 경우 다른 것은 (a）와 같고 단
        지 top_field_first = "1' ' 인 경우 bottom 如id가 먼저 반복되고
        to아ield_fl胤＝"0" 인 경우 top field가 먼저 반복되는 것이 다르다
       （왜냐하면 reverse인 경우는 field 순서가 반대로 되어야 하기 때
        문이다）.

addition川_copy_info : 7bits
  · 특허권에 대한 추가적인 정보를 여기에 실을 수 있다．

previous_PES卞packet_CRC: l6bits
  · CRC(cydic redui넌ancy check）에서 16개의 레지스터값이 모두 0이 되
    거］ 하는 CRC값（다항식은 넜6 +Xl뇨x5 + 1을 사용）
  1
      즉 그림 6-2와 갇은 CRC 디코더에서 각 레지스터값을 모두 " 1" 로
      초기화시킨 후 이 CRC 변수값을 MSB부터 차례로 입력시켜 CRC
      변수의 마치막 bit가 Z(1旬와 더해지고 그 값이 Z(0）에 입력된 후의
      모든 레지스터값은 0이 되어야 한다．


                  received data and CRC 16 bits
                    (most significant bit first)




            (0)




                         (1)    z(2)    z(3) +     z(4) +（今＜

                                                                            -o         0 0
                                                         니
                                                                  z
                                                                      (5)


                                                             啣니
                                                                            z
                                                                                (15)
                                                                                         -
                        그림 小2. l6bit CRC de（刃der model
MPEG 시스템


             1
                 이 값은 주로 네트워크의 유지보수를 위한 중간과 에러검출을 위해
                 쓰이는데 PES packet header값은 바뀔 수 있기 때문에 유료부하 부
                 분의 데이터 값만을 이용한다．

           PES_private_da切_flag : ibit
             · if("l") : PES packet header어］ user data가 존재한다．
             · if("O") : 존재하치 않는다．

           pad乞header－伽迂flag : ibit
             · if("l") : 入'JPEG] 의 pack header 또는 入띠PEG2의 PS pack header가 현
                 PES packet header어］ 존재한다．
             1
                 if("O") : 존재하지 않는다．
             1
                 만약 PES packet이 PS stream의 유료부하 부분에 있다면rs sUam은
                 관계없다） pack header 내용이 중복되므로 pack_header玉eld_flag = "0"
                 이 되어야 한다．

           program_packet_sequence_counter_flag : ibit
             · if(" 1") : program_packet_sequence_counter, MPEG1_MPEG2_identifier,
                 on帥mi_stu珏_leng由가 현 PES packet header어］ 존재한다．
             ·if ("O") : 존재하지 않는다．

           P-STh_buffer_flag : ibit
             · ifC'l ") : P-S기D1bu珏er_scale, I乙STI工buffer표ze가 PES packet header어]
                 존재한다．
             · if("O") : 존재하지 않는다．

           PES_extet喊on fi叩그 : ibit
             · ifC'l ") : PES_ex妃nsion_fie넌_length와 콴련 데이터（현재는 肥served로
                 되어 있음）가 PES packet header어］ 존재한다．
             · if("O") : 존재하지 않는다．

           PES_private_data   128b1ts
             1user data
                                               6. PES 패킷의 신택스와 의미


  · 이 PBS下nv趾e_data가 packet_start_code_i끄efix로 오인되는 것을 막기
    위해서 packet_氈art_code_j끄efix와 같은 비트열이 128bit 중 어디에도
    나와서는 안된다．

pad（上叱Jength : 8bit
  · pack_header() 길이의 byte수

pack_header()
  · pack_header_field_flag = "1" 이면 존재한다．
  · 入4PEG1 의 pack header 또는 MPEG2의 PS pack header를 저장하는 곳

program_packet_sequence_counter : Thits
  · 연속적인 PES pa味et에서 l씩 증가하는 continui口 （刃unt町역할（최대값
    127까치 가면 다시 0부터 시작）
  · 연속적인 PBS packet이란 MPEG2의 한 I冬 stream 또는 八'IIPEGi의
    system stream 내의 PBS packet들 중 MPEG2의 IS stream에서 하나의
    프로그램에 관계된 PBS packet들을 의미한다．
  ·duplica妃 PBS packet은 없기 때문에 똑갇은 program_packet_sequence_
    counter를 갖는 PBS packet은 존재하지 않는다．

八IPE(표 MPEG2 identii丘er : ibit
  · if("l") : 현 PBS packet이 入'IPEGI system stream을 갖고 있다．
  · ifC'O") : 현 PBS packet이 入'IPEG2 PS stream을 갖고 있다．

original_staff_length : 6bits
  · MPEG2의 PES packet header나 入4PEGI 의 packet header의 원본
    stream에서 ste佈n且切te의 숫자

P STh buffer scale : ibit
  · 현 PBS packet이 PS stream로 되어 있을 때만 유효하다．
  · P-STD_bu什e乙size를 계산할 때 스케일 팩터（scale factor）를 선택하기
    위해 쓰인다．
  1stream id가 오디오면 P-S끄口上U什er_scale = "0"
MPEG 시스템


             ·stream id가 비디오면 P-STh_buffer_scale = '1'
             · 그 밖의 다른 stream에서는 "0" 또는 "1" 값을 가질 수 있다．

           P-STD buffer size : l3bits
             · 현 PES packet이 PS stream로 되어 있을 때만 유효하다．
             · P-sm에서의 버퍼 크끼 BSn을 다음과 같이 계산한다．
                a) P-STh_buffer_scale = "0" 이면 BSn = P-STh_buffer_size x 128(bytes)
               b) P-STh_buffer_scale = "1" ]면 BSn = P-STh_buffer_size x 1024(bytes)
             · 이렇게 계산된 버퍼 크기는 P-STI工bu什er_size 변수가 p-sm에 도착
               된 즉시로 p-sm에서 이용된다．

           PES_exten前on_fieldlength : Thits
             · 뒤의 reserved 부분의 byte수

           stuffingbyte : 8bits
             1 "1111 1111"
             · 빈칸을 메우기 위해서 사용
             · 한 PES packet에서 32byte 이상 사용할 수 없다．

           PES_packet_data_byte
             · 유료부하 부분（el印妃nta日 steearn 또는 user data)
             · elemen啣ys配am이 入4PEG2 비디오나 오디오인 경우 PES_packeL1data
               -．切te들은 MPEG2 시스템 데이터들과 바이트 정렬（byteal坦ned）되어
               야 한다．
               이ementa口 stre出11들의 byte 순서는 지켜져야 한다．
               이 유료부하 부분의 byte수는 PES．下acket_length 변수의 바로 다음
               byte부터 PES工acket data旬te의 바로 전 t乃rte까지의 byte수를 PESe
               packet_len맘h값에서 뺀 값이 된다．

           padding尸byte : 8bits
               "1111 1111"
             · 빈칸을 메우기 위해서 사용
             ·streai可id가 paddin且stre帥인 경우 사용
                                                                        6. PES 패킷의 신택스와 의미




卜                          PSMPES 패킷


 이 program streaml map은 PSs配am어］ 있는 이ementary stream들을 서술
헤주며 서로간의 관계를 나타내준다. 또한 이 program St肥am map의 내
용은 Th stream 내에 있을 때 절대 변경될 수 없다. Program s配am map
의 계층적 구조는 그림 6-3과 갇고 자세한 내용은 표 6-7과 갇다. 표 6-
7의 내용은 program stream map을 위한 PES packet의 구조를 나타낸다.
여기서 packe匕切nHq月e工refix는 PES packet에서와 동일하고 map_s配am
1id는 표 6-2에서 pr唱ram_stream_map의 stream_id인 BC(I刃가 된다. 따라
서 이 program stream map은 하나의 PES packet을 이루며 , 그림 6-3에서
Cu'妃nt n炚t i岫C缸or부터 CRC부분까지가 표 6-1의 PES packet에서 PESm
packeL data byte어］ 해당하는 부분이 된다.


    packet   map    program    current         program   program N
    start    stream stream     next            stream    stream  loop
    code     id     map        indicator       map     퓨 info    descriptors
    prefix          length                     version =length

      24       8      16           1       2       5        7     16


                            elementary     N
                            stream         loops
                       y
                                                       努C
                            map
                            length




                   stream     이ementary        elementary       N
                   type       stream           stream           loop
                              id               info             descriptors
                                               length
                      8           8                 m


           그립 6요 I뇨）肛am Stl毛amrn町） dia肛am(MPEG Is: Figure F-8)
MPEG 시스템


                                     6-7. ram Stream map(MPEG Is: Table 2-35)

            S弘ltax                                                       No.of bits   八nemonic

            program1streamjnap() {
                     packet_stait_code_prefix                                   24    bslbf
                     map_stream_id                                               8    uimsbf
                     pmgram_stream_mapJength                                    16    uimsbf
                     cuntnLnext_indicator                                        1    bslbf
                     reserved                                                    2    bslbf
                     pmgmm_stream_map_version                                    5    uimsbf
                     reserved                                                    7    bslbf
                     marker bit                                                  1    bslbf
                     pmgr帥_stream_infoJength                                    16    uimsbf
                     for (i=O;i<N;i++) {
                                  desedptor()
                     }
                     elementaiy_stream_map_length                               16    uimsbf
                     如r (i닉上kN너＋+) {
                                  s甘eamtype                                      8    uimsbf
                                  elementary_stream_id                           8    uimsbf
                                  elementar寸stream_info_length                  16    uimsbf
                                  for (i=O;kN2;i++) {
                                      descnptor()


                     }
                     CRC 32                                                     32    rpchof




           packeLstart_code_pr必x                24bits
             1OOOO01(H)

           map_streamjd : 8bits
            1 BC(I刃

           program_stream_mapJength: l6bits
             · 이 변수 바로 다음 by妃부터 끝까지 (C그긋C_32 포함）의 by把수
             · 최대값은 1018
                                             6. PES 패킷의 신택스와 의미


cur七nt ne砒 indicator : ibit
  · if("l ") : 현재의 PSM이 유효한 것이며 현재의 PS入4에 있는
      program_stream_map_比rsion값이 유효한 I冬M의 버젼값을 가리킨다．
  1
      if("O") : 다음에 전송될 PS入4이 유효한 것이라는 것을 나타내며 , 그
      PS入4어］ 있는 pr略ram誼earn_map_v이.sion값이 유효한 PSM의 버젼값
      을 가리킨다．

pr略ram1就ream_map_vel寸on : Sb沁
  .Ps入4의 버젼을 나타낸다．
  ·PSM값이 한 번 바뀔 때마다 1씩 증가한다（31까지 증가하면 다시 0
      부터 시작한다）.

marker bit : lbit



pro毋am_stream_infoJen팝h : 1日站
  · 이 변수 뒤에 오는 descriptor() 길이의 by把수를 나타낸다．

desciiptor()
  · 프로그램이나 프로그램 요소에 대해 확장정의하기 위해서 사용되는
      서술자로 9장에서 설명된다．

elementat工曲eam_n姐p_le唯th : l6bits
  · 이 변수 바로 다음 by把부터 CRC_32 바로 전까지의 정보（이 PSM어］
      서 기술된 elementaiy stream들에 대한 기술）의 by妃수를 나타낸다．

stream_type : 8byts
  · 표 6-8과 같이 elementaiy stream의 타입을 나타낸다．

elementary_stream_id : 8bits
  · 이 elementa口 stream이 저장된 PES packet header어］ 있는 stream_id값
      과 동일하다．

elementary_stream_info_length : l6bits
  · 이 변수 바로 뒤에 있는 descriptor( ）의 byte수
MPEG 시스템


                        표6-8. Streai ty光 心ignments(MPEG Is: Table 2-36)

            Value                       Description

             0x00       ITU-T I ISO/또C Reserved
             0x0l       ISO/IEC 11172 Vid以
             0x02       ITU-T Rec. H.262 I ISO/IEC 13818-2 Video or ISOIIEC 11172-2
                        constrained parameter 너deo stream
             0x03       ISO/IEC 11172 Au如
             0x04       ISO/IEC 13818-3 Audio
             倣05        ITU-T Rec. H.222.0 I ISO/IEC 13818-1 private_sections
             敬（石        ITU-T Rec. H.222.0 I IS이IEC 13818-1 PES pCk眈sco曲岫평 口ivate data
             0x07       ISO/IEC 13522 MI-lEG
             0x08       ITU-T Rec. H.222.0 I ISO江EC 13818-1 Annex A DSM CC
             0x09       rru丁 R凹. H.222.1
             敬0A        ISO/IEC 13818-6 type A
             0x0B       ISO/IEC 13818-6 type B
             0x0C       ISO/IEC 13818-6 type C
             0x0D       ISO/IEC 13818-6 type D
             0x0E       ISO／표iC 13818-1 au以小aiy
           0x0F-t次7F    ITU丁 Rec. H.222.0 I ISO/IEC 13818-1 Reserved
           伽80-0x}下     User Private




                             received data and CRC 32 bits
                               (most significant bit first)




                       (0)


                                켜쁘）

                                                  z   (     z(3) 斗（今＜


                                                                  니 z(4十啣

                                                                                (31)
                                                                           z
                                                                    啣니
                                                                                       跏
                       그림 6-4. 32b1t CRC decoder m以lel(MPEG Is: Figure
                                               6. PES 패킷의 신택스와 의미


descriptor()
  .9장에서 설명

CRC 32 : 32bits
  · CRC(cycic redun由ncy ch凹k）에서 32개의 레지스터값을 모두 0이 되
    거］ 하는 CRC값（다항식은 X32+ X26+ X23+ X22+ Xl6+ Xl2+ Xn+ Xl0+ X8+
    寸+ X5 +X4 +X2 + x + 1을 사용）
    즉 그림 64와 같은 CRC decod町에서 각 리江］스터값을 모두 " 1" 로
    초기화시킨 후 이 CRC 변수값을 入4SB부터 차례로 입력시켜 CRC
    변수의 마지막 bit가 Z(31) 와 더해지고 그 값이 Z(0）에 입력된 후의
    모든 레지스터값도 0이 되어야 한다．




卜                    ND PES 패킷


  PES packet으로 운반되는 스트림들의 디렉토리를 나타내며 PSD들의
내용을 모두 모으면 전체 디렉토리를 얻을 수 있다. PSD도 PES packet
의 하나로써 stream_id가 I下(H）이다. 이 디렉토리를 보고 각 picture나 오
디오의 frame을 참조하기 위해서는 directory entry가 필요한데 각 경우의
面ecto口 entry는 다음과 같다．


  · 중간에 picture header없이 sequence header 바로 뒤에 나오는 I-picture
    의 directo口 entry는 sequence header의 첫번째 byte이다．
  · 중간에 picture header없이 (]OP header 바로 뒤에 나오는 I-picture의
    directory entry는 GOP header의 첫번째 byte이다．
  · 그 밖의 다른 picture들의 directory entry는 pictu肥 header의 첫번째
    匈te이다．
MPEG 시스템


              1
                  Audio stream에서의 direc的iy ently는 audio fi跏ae의 sync word이다．
                  Directoiy에서 access unit의 기술 순서는 그 access unit이 bitstream어］
                  서 나타나는 순서와 동일해야 한다. PSD의 구조는 표 6-9와 같다．

           packet_s始rt_code_pr丘X : 24bits
             · 000001(H)
                                    h
                                    腑
           dha：
              匈口盛曲mid
             1 FF(H)

           PES_ 그1acketJength : l6bits
             · 이 변수 바로 뒤 byte부터 PSD끝까지의 byte수

           number of access units : i듸bits
             · 이 PSD PES packet어］서 언급되고 있는 access ui血의 개수

           P1七V寸dii七ctory_offset : 45b沁
             · 현재 PSD 앞에 있었던 바로 천의 PSD를 갖고 있는 PES packet stan
                  code의 첫번째 by把부터, 현재 이 prev_小rectory_o瓜et변수를 갖고 있
                  는 PSD PES packet의 start code 바로 전까지의 byte수（즉， 앞쪽 byte
                  address offset)을 나타낸다．
             · 이 변수값이 0이라는 것은 바로 전의 PSI) 정보가 없었다는 것을
                  뜻한다．

           next_directory_offset : 45bits
                  이 next面邙toiy_o砥et을 갖고 있는 PSD PES packet start code의 첫번째
                  byte부터 현재 PSD 이후에 전송될 다음 PSD PES packet s切it code의
                  첫번째 byte 바로 전까지의 byte수（즉, 뒷쪽 byte add配ss offset)을 나
                  타낸다．

           packet_stream_id : 8bits
             · 이 디렉토리 엔트리에 의해서 언급되는 access unit을 포함하는
                  elementaiy stream의 stream_id
                                                        6. PES 패킷의 신택스와 의미


    표6-9. PES packet syntax for Pmgrarn Steam d嶝缸y(MPEG Is: Table 2-37)


Syntax                                                No. of B批S                                                               加Inemonic

曲ectoty_匹昱恥ck呱 ){




                                                              가8珀巧l巧l巧l巧l巧l巧l巧l
   packet_st키tHc（뇌e工）or丘乂                                                                                                      bslbf
   directory_stream_id                                                                                                         uimsbf
   PES_packetJength                                                                                                            uimsbf
   number_of_access units                                                                                                      uimsbf
   marker bit                                                                                                                  bslbf
   prev_directoiy_offset[44..30]                                                                                               uimsbf
   marker bit                                                                                                                  bslbf
   prev_directory_offset[29..15]                                                                                               uimsbf
   marker bit                                                                                                                  bslbf
   prev_directory_offset[14..0]                                                                                                uimsbf
   marker bit                                                                                                                  bslbf
   next_directoryHoffset[44..301                                                                                               uimsbf
   marker bit                                                                                                                  bslbf
   next_directmy_offset[29..15]                                                                                                uimsbf
   marker_bit                                                                                                                  bslbf
   next_ 血ectoiy_offset[14..0]                                                                                                 uimsbf
   marker bit                                                                                                                  bslbf
   for(i = 0; i <num比r of acces乞urn姓 i4f) {




                                                                                                          口 l ＜口 l 8 l l 2 4
            packet_stream_id                                                                                                   uimsbf




                                                                 8 l1 41 l ＜口 1王 <U l /b l n4口 그1V l <U l ＜
            PES_header_pos地on耐놨sign                                                                                            tcimsbf
                                                              l
            PES1吃ader_position_o卄凹t[43..30]                                                                                    uimsbf
            marker bit                                                                                                         bslbf
                                                              l
            PES_ 比ader_position_offset[29..15]                                                                                 uimsbf
            marker bit                                                                                                         bslbf
                                                              l
            PES_heade냐'Os地on崎奴[14..0]                                                                                          uimsbf
            ma卞：er_bit                                                                                                         bslbf
                                                              l
            reference offset                                                                                                   ulmsbt
            marker bit                                                                                                         bslbf
            肥served                                                                                                            bslbf
            PTS[32..30]                                                                                                        uimsbf
            marker bit                                                                                                         bslbf
                                                              l
            PTS[29..15]                                                                                                        uimsbf
            marker bit                                                                                                         bslbf
                                                              l
            PTS[14..0]                                                                                                         uimsbf
            marker bit                                                                                                         bslbf
                                                              ]
            bytes_to_read[22..8]                                                                                               uimsbf
            marker bit                                                                                                         bslbf
            bytes_to_read[7..0]                                                                                                uimsbf
            marker bit                                                                                                         bslbf
            intra a넜edin小cator                                                                                                 bslbf
            codng_parame把rs_indicator                                                                                          I川bf
            reserved                                                                                                           bslbf
     }
}
MPEG 시스템



           PES_header_p好世on_offs吐S也n : ibit
             · PES上ea由口螂ition_o瓜et의 부호
             · 부호에 대한 자세한 설명은 PES上明de口螂而on o依et부분에서 한다．

           PES_header小p珞ilion_o趾et : 44bits
             · 이 PES_header_j姚ition_o砥아변수를 포함하는 PSD PES packet start
              c茯妃의 첫번째 by妃부터 이 디렉토리에서 언급되는 access unit의 첫
              번째 byte를 포함하는 PES packet start co妃의 첫번째 by也바로 전까
              지의 byte 수
            · if (PESH如ade디四sition_offse匕坦n = tI0'I) : access unit의 PES packet이
              뒤에 있다（邸蜘e offset).
            · if (PES_header_position_offset_sign = "1') : access unit의 PES packet 1
              앞에 있다（negative o什set).
            ·0값은 access unit이 없다는 것을 뜻한다．

       I七fei七nce off甘et : l6bits
            · 언급된 access unit의 첫번째 byte를 포함하는 PES packet의 첫번째
              byte부터 언급된 access unit의（유료부하에 있는） 첫번째 byte 바로 전
              까지의 byte수
                                           b
       PTS(presentation_tirne_stamp)       玔

            · 언급된 access unit의 P1S

       bytes_to_read : 23bits
            · reference_아Iset어］서 언급된 access unit의 첫번째 byte부터 언급된
              ac凹ss unit을 완벽하게 디코딩하기 위하여 필요한 byte수를 PS siream
             상에서 계산한 것（이 byte수는 시스템 동작 중에 삽입되거나 다중화
              된 PS stream상의 모든 정보를 전부 포함한다）.

       intra coded indicator : ibit
            1 if("l") : 언급된 access unit이 video stream이고 전부 intra로 코딩된
             경우
                                                                6. PES 패킷의 신택스와 의미


 ·if ("O") : 언급된 欲x无SS UI血이 video stream이고 전부 in仕a로 코딩되지

   않은 경우
 ·steam이 MPEG2 vid凹7} 아닌 경우는 이 flag은 정의되지 않는다．
 1 표 6-10


               표； 6-10. Intra 口：Kied indic카야（MPEG Is: Table 2-38)


                        V出ue                     Meaning

                          0                      Not Intra
                          l                      Intra



C어如唯下aramenta乞in小毗or : 2bits
  · 언급된 access unit을 디코딩하기 위해서 필요한 변수（parameter）들의
   값의 상태와 전달위치를 표 6-Il과 갇이 나타낸다．


            표6-11. Codin나）arameters indicator(MPEG Is: Table 2-39)


   V出ue                               Meaning


    m아
                削1 coding parameters are set to their default v出ues
                시1 c岫ag paramete八 are set in this access unit, at least one of
                them is not set to a default.

    mn
                Some coding parameters are set in this access unit.
                No c川ng parameters are coded in this access unit.
                            7. 트랜스포트 스트림에서의 신택스와 의미




                                   트랜스포트
                          스트림에서
                          신택스와 의：




 TS packet은 ]88byte로 구성되어 있으며 , header부분의 sync上yte는 바이트 정열（byte
訓gned）되어 있다. 따라서 TS stream에서 바이트 정열시켜서 sync抑te를 찾아내면 IS packet을
추출해 낼 수 있다．
MPEG 시스템




    卜                               咐적』TS!H킷
            일반적인 TS packet의 계층적 구조는 그림 7-1과 갇고 자세한 내용은
           표 7-1과 같다. TS packet은 그림 7-1과 같이 188by妃로 구성되어 있으며
           header부분의 sync-切te는 바이트 정렬（by妃 띠igned）되어 있다. 따라서 l 's
           steam에서 바이트 정렬시켜서 sync_byte를 찾아내면 TS packet을 추출해
           낼 수 있다．


                                -   188bytes -
                transport
                   packet




                 transport      payload                  transport  adaptat由n

            謐    error
                 indicator
                                unit start
                                indicator
                                           transport
                                           pnonty
                                                     PID scran出ling field
                                                         control    con甘이
                                                                                         continuity
                                                                                         counter    『辯難：
                                                       13          2                          4
                                                                                          +
                                                            elementary
                adaptation                   random
                           discontinuity                    stream                     optional    stuffing
                field                        access                        5flags
                           indic카or                         priority                   fields      bytes
                length                       indicator
                                                            indicator




                                              transport                   adaptation
                                              private        transport    field                    :option日
                         splice                              pnvate                      3 flags
                PCR OPCR                                                  extensi아l                 fields
                         countdo낵n            data
                                                             data
                                              length                      length
                            仁
                 42



                             ltw valid    ltw          piecewise         斗小ce
                                                                              DTS next au
                             flag         offset       rate              type

                                                   n
                                                   乙
                                                            n
                                                            乙
                                                            n
                                                            乙              4             八
                                                                                         J
                                                                                         그
                                                                                         U




                      .J.림 7-1. Transport Stream syntax diagram(MPEG Is: Fig끄e F-i)
                                                      7. 트랜스포트 스트림에서의 신택스와 의미


      표
       7-1. ITU丁 Rec. H.222.0 I ISO/IEC 13818 transport packet(入4PEG Is: Table 2-3)

  Syntax                                                               No. of bits 入nemonic

  transport尸packet( ){
           sync_byte                                                               8 bslbf
           transport_errorjn小C趾or                                                  1 bslbf
           payload_山liLstart_indicator                                             1 bslbf
           transport느pnotity                                                    1      bslbf
           PID                                                                 13      uimsbf
           transport_scrambling_control                                         2      bslbf
           adaptation_field_contr丑                                      2              bslbf
           continuity_counter                                           4              uimsbf
           if(ada口帥on五eld中conti이 =='10' II ad叩tation_field_c刃ntrol＝난11가
                    adaptation_field()
           }
           i!(ada比ation_field_control =='0l' II 征蚣ptation_field_control =='lI) {
                    白r (i닉가kNm+){
                               data_byte                                           8   bslbf
                     }
           }
  }


sync_byte : 8bits
      "아000111"
  · 주기적으로 반복되는 다른 부분（예를 들어 P11기에서 이 값은 사용
      될 수 없다．

transport_error_indicator : ibit
  ·if ("l") : 그 TS packet에 적어도 한 7下1 이상의 고칠 수 없는 에러가
      발생했다는 것을 의미
  · 다시 "0" 으로 바꾸기 위해서는 그 에러들을 모두 정정해야 한다．

payload_unit_start_indicator : ibit
  ·null packet인 경우는 "0" 이 되어야 한다．
      a) 유료부하가 PES packet을 포함하는 경우

          if("l") : 그 TS packet의 유료부하가 PES packet으j 첫번째 byte부터 시
          작됨을 의미
MPEG 시스템


                  if 'O") : 그 TS packet의 유료부하에 새로이 시작되는 PES 們cket이 없
                  다는 것을 의미（새1로운 PES packet은 유료부하의 중간 부분에서 시작할
                  수 없다．)
               b) 유료부하가 PSI 정보를 포함하는 경우
                  if("l") : 유료부하의 첫번째 byte가 PSI정보의 p이nter_fie넌를 나타낸다．
                  if("O") : PSI 정보가 없다．

           tr게ii叩야냐)riority : ibit

            ·if ("l") : 갇은 PH）를 갖는 packet들 중에서 그 packet이 transpoit_
              priority = '0" 인 packet어］ 비해서 우선순위가 높음을 의미
             · 이 값은 인코더나 디코더에서 우선순위를 바꾸기 위하여 변경할 수
               있다．

           PlO : 13bits
             · 유료부하에 있는 데이터 타입을 나타낸다．
             I 할당된 Ph）값은 표 工2와 같다．
                                      이0(H)-i邱E(H）인 곳에서는 PCR 정보를
             · P11）값이 (X00(H), 0001(H ）
               전송할 수 있다（PC艮PID).


                                 표7-2. PID table(MPEG Is: Table 2-4)

                          V심ue                             Description

                                                  Pro입m Association Table
                                                  Conditional A凹ess Table
                                                  reserved
                                                  may be assigned as network_PD,
                                                  Program_map_PID, elementaiy_PID,
                                                  or for other purposes.
                                                  Null packet




           transport_scrambling1control : 2bits
             · 유료부하 부분의 스크램블링모드를 표시한다（표 工3).
                                            7. 트랜스포트 스트림에서의 신택스와 의미



              표； 7-3. S口日工nbling （刃fir아 vahi心小PEG Is: Table 2-5)

                       V可ue                    Description

                         00                    not scrambled
                         01                    user defined
                         10                    user defined
                         11                    user defined


  1
      packet header와 adaptation field는 스크램블링되지 않는다．
  1
      null packet인 경우에 이 변수값은 "0" 이 되어야 한다．

adaptation_field_contml : 2b1ts
  · 그 packet의 유료부하 부분에 adaptation field 또는 유료부하의 존재
      유무를 나타낸다（표 7-4).


            표卜4. Adapta仕丑i field （刃fir아 vaiu田小'IPEG Is: Table 2-6)

              \／刊tue                       Description




                m아mn
                                  reserved for future use by ISO/LEC
                                  no adaptation_field, payload only
                                  adaptation_field only, no payload
                                  adaptation_field followed by payload


  1
      null packet인 경우의 값은 "01" 이 되어야 한다．
  1
      "0" 값을 갖는 packet은 시스템 디코더에서 버린다．

continuity_counter: 4bits
  · 같은 PID를 갖는 TS packet 한 개당 1씩 증가하지만 adaptation_field
      J刈血ol값이 "00" 또는 "10" 인 경우는 증가하지 않는다（즉, 유료부하
      가 없는 경우는 증가하지 않는다）.
  1
      최대값 15어］ 도달하면 그 다음 0으로 순환된다．
  1
      duplicate packet어］서의 continu好_counter값은 같다（참고로 伽plicate
      packet어］서는 仄：R 정보를 제외한 모든 값은 같다）.
MPEG 시스템



                  null packet의 경우 COT心nui竝J：에n把r값은 정의되지 않는다．
             1



             1
                  이 continuity_counter는 뒤의 adaptation_field( ) 부분의 小scontinuity_
                  indic欲or가 "1" 인 경우에는 불연속일 수 있다．

           adaptation_field()
             · adaptation_field_帥ixol이 "10" 또는 " 11" 인 경우에 존재
             · 적용필드 참조

           data_byte : 8 X N bits
             · 유료부하에서 보내려고 하는 PES packet, PSI 정보, user data, 메우는
                  더］ 쓰는 것佃呻ing) 등을 말한다．
             · adaptation_fleldj刃ntrol이 "01" 또는 " 11" 인 경우에 존재
             ·N= 1＆乍（adaptation_fl이d(）의 길이 )


           0 적응필드（adaptation field)

             적응필드의 구조는 표 7-5와 같다．

           Adaptation_fieldJength : 8bits
             · 총 adapta如n_field(）의 byte수eiby妃（adaptation_丘eld_len믄付l 변수）
             · if (adaptation_field_control = "11") : adapta如n_field士ngth값은 0부터 182
                  까지의 값을 갖는다．
              1
                  if (adaptation上이d_conti이＝"10") : adaptation_如通le璡th값은 183
                  PES packet의 첫번째 byte는 TS packet 유료부하의 처음부터 시작하1
              1




                  야 하기 때문에 바로 전 TS packet의 유료부하 부분이 남는 경우가
                  있다. 이와 갇이 남는 공간은 의미없는 데이터로 메워줘야 하는데
                  (stuffi雎） 이를 adaptation field의 ste飯雎上yte 부분에서 하게 된다. 따
                  라서 , adaptatio兀field_length는 이 모든 stuffing_byte 부분까지 포함한
                  길이를 나타내게 된다．

           小scoutinui勺1indica切r : ibit
             · if("l") : 불연속 상태（曲continuity stat이가 참（tnie)
             · if("O") : 불연속 상태（discontin山y stat미가 거짓（false)
                                     7. 트랜스포트 스트림에서의 신택스와 의미



이 변수의 의미는 다음과 갇은 두 가지 경우에 각각 서로 다른 의
미를 갖는다．
a)
     system time-base discontinui口

     TS packet의 P표）가 PCR_PID를 갖는 경우에만 해당

     "불연속 상태" 가 참이면 그 해당 프로그램이 새로운 system c1ock(즉 새1
     로운 PCR）을 이용한다는 뜻（즉, PCR에 불연속이 생긴다）인데 그 새로
     운 PCR은 이 小羽on血떼.y_indi：趾or변수 뒷쪽 어디에서도 전송할 수 있
     다. 다시 말해서 discontinuity_mdicalor = "1" 인 현재 TS packet의 1X:R필드
     에서도 전송가능하며（이때1 PCR；丑ag = "1") 또한 PCR필드없이 (liscon-
     山iuityJndicator = "1" 인 TS packet들（이 packet들의 PCR_flag = "0" 이고 PD
     = PCR_PH）이어야 한다）을 연속적（중간에 한 개라도 小scontinuity_
     indicator = "0" 이 될 수 없다）으로 전송하다가 바로 다음 TS packet에서
     PCR필드를 전송해도 된다（이 packet도 역시 discon山luity_indicator = "1" 이
     어야 한다）.

     System time-base가 "바뀌는 점 " (dis（刃ntinui口 1X血t)은 새로운 PCR을 갖
     고 있는 TS packet의 첫번째 切'te가 T-STI）에 도착하는 순간으로 한다．

     System tin好加se가 "바뀌는 점 " (discontinuity ix万nt) 전에 새로운 PCR을
     기준으로 한 I玎S나 DTS를 갖고 있는 TS packet의 첫번째 by把가 T-
     S1D에 도착해서는 안된다．

     System time-base가 "바뀌는 점 " (discontinuity point) 후에 지난 PCR을 기
     준으로 한 vrS나 DTS를 갖고 있는 TS packet의 첫번째 by把가 T-STD
     어］ 도착해서는 안된다．

     일단 한번 새로운 PCR로 바뀐 다음에는 그 바뀐 PCR필드가 적어도
     두 개 이상 전송된 후에 또 다른 PCR로 바꿀 수 있다．

     또한 어느 순간에 T-STI）의 버퍼 내에 있는 한 프로그램에서 서로 다
     른 PCR읕 갖는 데이터들의 개수가 최때1 두 개까지 허용된다（즉 버퍼
     용량 내에서 PCR이 두 번 바뀔 수 있다）.

b) conitnuity_counter dis刃ntinuity
     TS packet의 PD가 PCR_Pll）인 경우 "볼연속 상태" 가 참이면 system
     血ne七ase가 "바뀌는 점" 에서만이 packet（즉 새로운 PCR이 전송되는 TS
     packet）의 con山1u均下ount心값에 "불연속" 이 생길 수 있다（같은 PCR_PID
     를 갖는 바로 전의 TS packet과 비교해서）.
MPEG 시스템


                      표 7-5. Transport Stream adaptation field( 入PEG Is: Table 2-7)

           S끄ltax                                                            No. of Bits   八nemonic

           adaptation_field() {
                                                                                       8        曲
               ada꺄毗ion_field_len멤h
                                                                                            1
                                                                                            m
               if(adaptation_field_leng仕1 >0) {
                 discontinuity_indicator                                              I    bslbf
                 random_access_indic趾or                                               1    bslbf
                 elementa口_stream＋加的_indicator                                        1    1川bf
                 PU之_fiag                                                             1    bslbf
                 아C巳flag                                                              1    bslbf
                 splicing_point_flag                                                  I    bslbf
                 transport_pnv毗코姐丑ag                                                  1    bslbf
                 adaptation_field_ex把nsion_flag                                       1    bslbf
                 if(PCR_flag=='l') {
                         pmgram_clock_reference_base                                 33    uimsbf
                         reserved                                                     6    bslbf
                         program_clock_reference_extension                            9    uimsbf
                 }
                 if(OPCR_flag=='l) {
                         ori멈nal_
                              pmgram_clock_reference_basc                            33    uimsbf
                         reserved                                                     6    bslbf
                         originalpm얍am_clock_i可毗nc乞以帥sion                             9    uimsbf
                 }
                 if (splicing_point_flag == '1) {
                                                                                      8
                         s小cc寸countdown                                                    tcimsbf
                 }
                 if(transport_private_data_ flag == '1') {
                                                                                      8
                         tr毗port_piivate_由laJength                                         uimsbf
                          for (id); i<transp끄t_piivate_data_length;i-i-+){
                                                                                      8         帥
                                  private_data_byte


                 }
                 if (adaptation_fiek匕胤ens幻心lag =='l ' ) {
                         ada曲lion配넌H炚妃nsion_leng山                                     8    uinisbf
                         ltw_flag                                                     1    bslbf
                         piecewise_rate_flag                                          1    bslbf
                         seamless_splice_flag                                         1    bslbf
                         reserved                                                     5    bslbf
                         if (ltw_flag=='V) {
                                              7. 트랜스포트 스트림에서의 신택스와 의미



                    ltw_v出id_flag                        1 bslbf
                    ltw offset                          15 uimsbf
            }
            if (piecewi仁rate_flag == '1') {
                     reserved                            2 bslbf
                     piecewise_rate                     22 uimsbf
            }
            if (seamless_splice_flag == 'D{
                     splice_ty玘                          4   bslbf
                    DTS_next_AU[32..30]                  3   bslbf
                     marker bit                          1   bslbf
                    DTS_next_AU[29..151                 15   bslbf
                     marker bit                          1   bslbf
                     DTS_next_AU[14..O]                 15   bslbf
                     marker bit                          1   bslbf
            }
            for ( i=O;i<N;i++) {
                     reserved                            8 bslbf
            }
    }
    for (i=O;i<N;i-i-+){
             st나ffing_byte                               8 bslbf



}


    TS packet의 P표）가 PCR_PID 7} 아닌 경우 "불연속 상태" 가 참이면 같
    은 PD를 갖는 바로 전 TS packet고干 비교해서 continuityJ刃unt町값에
        "불연속" 이 생길 수 있다（아닐 수도 있다는 뜻）. 그러나 일단 한번
        discon血nnty如毗缸or= '1" 이면 같은 PD를 갖는 3개（즉 PD가 같으면서
        연속적으로 discontinuity_indicator = "1" 인 packet을 3개까지 허용） packet
        이내에서 col仙恤口下ount町의 "불연속" 이 적어도 한 번 발생해야 하며
        con山Iu均coli毗er의 불연속이 생길 때까지 그 패킷과 그전 패킷들의
        discontinuit느indicator값은 "1" 을 유지해巾乍 한다．

        TS 附：ket이 elementary stream을 유료부하로 갖고 있는 경우 conitnui口小
        count町의 "불연속" 이 발생하면 그 패킷 또는 그 후 같은 P11）를 갖는
MPEG 시스템


                   TS packet의 유료부하에 있는 이en祀ntary stream의 첫번째 byte는 오디오
                   의 경우 audio 丘ame의 첫번째 by把이며 비디오의 경우 羽叫ence header
                   의 첫번째 byte가 되거나 sequence header전에 sequenc乞end_c뇌e가 있으
                   면 그 sequen此endJ兀de가 되어야 한다．

                   해당 프로그램의 system time base불연속이 발생했을 1대F 그 후의 PCR
                   PD 7} 아니면서 elen祀ntaly stream을 포함하고 （刃n山m均下ounter의 "불연
                   속" 이 발생하고 새로운 I끼is나 DTS를 갖는 TS packet은 system time-
                   base 불연속이 발생한 후에 T-STI）어］ 도착해야 한다．

                   "불연속 상태"가 참인 경우 같은 PD를 갖고 con仕nu柳下ount町값이 같
                   으며 adaptation五eld_contml값이 "01" 또는 " 11" 인（즉 유료부하가 있다는
                   뜻） packet이 두 7뀨 존재하면 뒤의 packet은 버린다（시스템 인코더는 이
                   런 사실을 숙지하고 이렇게 버려지는 패킷이 어떤 손실이나 어려움올
                   가져오지 않도록 고려해야 한다）.

                    "불연속 상태" 가 참인 경우 PsI 정보를 포함하는 TS packet에서 PSI 섹
                   션의 veiSiOn皿nnl光r어］ 불연속이 생길 수 있다. 이때1 그 해당 프로그램
                   의 TSj加입ammap配ction은 section_length = 13으로 하고 current_f思xt
                   indicator = 1 인 상태로 전송되어야 한다（이는 program_descriptor나
                   이ementaly 앉ream이 없다는 것을 뜻한다）. 그후 그 해당 프로그램의
                   T5program_n啣sec如n이 vers幻兀num比r를 하나 증가시키고 current_next
                    in毗缸or= I 인 상태로 다시 전송되어야 한다．

           random access indicator : ibit

             · if("l ") : PD가 갇은 현재 또는 그 다음 IS packet에서 처음 시작되

                 는 PBS packet에서（왜냐하면 현재 TS packet의 유료부하 부분이
                 adaptation field로 전부 찰 수가 있기 때문에） sequence headei們］디오
                 의 경우） 또는 frame（오디오의 경우）의 첫번째 byte가 시작한다（즉，

                 다음번 TS packet부터 임의접근（random access）이 가능하다는 의미）.
                 이때 그 PBS packet이나 그 다음 PBS packet어］서 위의 sequence
             1




                 header 또는 audio frame 바로 뒤의 picture나 frame어］ 대한 FF5를 쩌1

                 공해 주어야 한다．
                 현재의 Pu）가 PCR_PII）면 뒤의 PCR小flag = "1" 이 되어야 한다．
             1
                                          7. 트랜스포트 스트림에서의 신택스와 의미



elementary_stream_priority_in小c毗or : ibit
  · i且" 1") : 그 TS packet의 유료부하 부분의 데이터가 elementaiy_stream_
      priority_indicator = "0"인 유료부하들보다 우선순위가 높다는 것을 의미
  · 예를 들어, 비디오에서 intra coding된 데이터인 경우 " 1" 로 세팅해서
      우선순위를 높일 수 있다．

PCR_flag : ibit
  · if("l") : PCR 정보가 adaptation尸fleld(）에 존재한다．
  · if("0") : 존재하지 않는다．

OPCR_flag: ibit
  · if("l") : OPCR 정보가 adaptation_fleld(）에 존재한다．
  1
      if("0") : 존재하지 않는다．

Sr네icing_poim卄H仇ag : ibit
  · if("l") : 斗小ce_countdown 정보가 adapta加n_field()에 존재한다．
  · if("0") : 존재하지 않는다．

transport_priva虹data_flag: ibit
  · if("l") : 한 byte 이상의 private_由Ia가 adaptation field어］ 존재한다．
  · if("0") : 존재하지 않는다．

adaptation_fleld_extension_flage : ibit
  ·if ("l") : adaptation_fleld(）의 ex把nsion이 존재한다．
  · 迂
    （"0") : 존재하지 않는다．

        program_cl어k_reference_base : 33bits
        reserved : 6bits
        program_clock_reference_ex妃nsion : 9bits

      P:R은 다음 식과 갇이 계산되며 , 이는 program_eli姚reference加se
      의 마지막 bit를 포함하는 by把가 T-S기）Gystem target decoder）에 도달
      되는 시간을 의미한다．
      다음 식으로 계산된다．
MPEG 시스템



                PCR血ise(z) =((s瑁切也clockj初ueu功＜ 瓦功끼V3伉) % 233
                PCR_ 奴1) = ((묵y町功Lm兀丸-t沌que夙）>< z(i力DIV 1) % 300
                PCR(i) = PCR_base(z) X 300 + PCR_ext(i)

              original_pmgram_cl乂k_refemnce._base : 33bits
              reserved : 6bits
              0旽inal_pr孕amCI(乂k卞佃ence_ex把的on : 9bits


           · 위의 PCR 정보가 있을 때만 이 OPCR 정보를 보낼 수 있다．
           · 이는 원래 프로그램의 PCR 정보로써 단일 프로그램（single program)
            인 경우 PCR과 OPCR이 갇다. 그러나 여러 개의 프로그램（跏l如le
            pro留am) 으로 이루어진 TS sneam의 경우는 틀리게 된다．
            여러 개의 프로그램으로 이루어진 TS stream으로부터 단일 프로그
            램을 뽑아서 단일 프로그램 TS sneam을 만들고자 할 때는 아X:R값
            을 PCR로 옮겨 쓰면 된다．
            다음 식으로 꼐산된다．

               OPCR_base(i) = ((s少把m寸clo(火-J加quency X 瓦功川V艾劤 1)/1。h33
               OPCR_ex仄I) = ((syste／刃寸clockj沌quency >< l(i力DIV 1) % 300
               OPCR(i) = OPCR_ba貂(i) x 300 + PCRext(i)


       slice countdown : 8bits
           · 하나의 elementa口 stiam을 다른 elementaiy stream어］ 끼우거나 연결
            (splicing）할 때에 연결하는 위치를 countdown함으로써 디코더에 알
            려주는 역할을 한다．
            duj小ca妃 TS packet이나 adaptation field()만을 포함하는 TS packet에서
            는 countdown되지 않는다．
           · 음양값을 가지며 2con叩lement로 표시한다（즉 +n이면 splicing되는 위
            치까지 n byte가 남았다는 뜻이며, H n이면 spicing된 후에 nbyte가
            지나갔다는 의미이다）（그림 5-17 참조）.
                                            7. 트랜스포트 스트림에서의 신택스와 의미



 ·splicing되는 위치는 Sm 모델의 TBn 버퍼로부터 그 TS packet이 옮
    겨진 바로 직후이다. 그때 splice countdown값도 0이 되고， 그 TS
    packet 유료부하의 마지막 byte는 audio fran配이나 picture coding data
    의 마지막 byte가 되어야 한다（오디오의 경우는 audio frame의 마지
    막 byte이며 비디오의 경우는 sequence_end_code의 마지막 byte 또는
                                                                      丘
    羽叩en凹end code의 바로 전 byte가 된다）.
  ·splicing이 된 후에는 splice_countdown값은 음수가 되는데 splice
    countdo낵n값이 -1 인 경우의 TS packet의 유료부하에서 시작되는
    PES packet의 유료부하는 audio 丘ame이나 너de4느sequence_header의 첫
    번째 byte 또는 sequen凹end code부터 시작한다．

transport_ 그1rivate_data_length : 8bits
  · 바로 뒤에 있는 priv毗dat心恥e의 by把수를 나타낸다．

11加a虹d毗a切te : 8bits
  · transport_pnvate_data_length 수만큼 꼐속되는 user data

adaptation_field_extension_length : 8bits
  · adaptation_field( ) 부분의 byte수를 나타낸다（뒤의 肥served 부분까지
    포함）.

ltw_flag : ibit
  · if ("1") : ltw小offset이 존재한다．
  · ii ("0") : 존재하지 않는다．

piecewise_rate_flag : ibit
  · if ("1") : piecewise_ra妃가 존재한다．
  · if ("0") : 존재하지 않는다．

seamless_splice_flag : ibit
  · if ("1") : sj小ce竝pe과 DTS_ne粒／1V가 존재한다．
  · 寸 (11011) : 존재하지 않는다．
  · splice_p（뇨nt_flag = "1" 인 경우에서만 이 flag이 " 1" 로 될 수 있고 splice
MPEG 시스템



               _countdown이 양수일 때 일단 이 flag이 " l " 로 되면 sp丘ce_countdown
               이 "0" 이 될 때까지（"0" 인 경우까지 포함） 그 뒤의 같은 r皿）를 갖
               는 모든 冗 packet에서 이 flag값은 " l " 로 유지되어야 한다．
               이 flag이 " 1" 인 경우 elementaiy stream이 오디오 신호면 뒤의 splice
               jype 변수값은 "0000" 이 되어야 하며, 비디오신호면 sp五此_tyl玘어］서
               규정하는 조건을 만족해야 한다．

           岫v valid丑ag : ibit
             · if ("l") : it也O砥et의 값이 유효하다는 것을 의미
             · if ("O") : it'w_o瓜et의 값이 의미가 없다는 것을 의미

           ltw offset (legal 仙nle window offset) : l5bits
             ·ltw_valid_flag = "1" 인 경우만 유효
             · 시간의 단위는 (30姸砂이고 fs는 해당 P11）어］ 속하는 프로그램에서
               사용한 system_야姚玉equency이다．
             · 佃山砥et값은 다음과 같이 졔산한다．

                   ltw_offset = t1(i) H 1(i)

              여기서 t1(i)는 legal time window인 [t0(i), t1(i刀구간의 상한값（UPI兄r
              bound）이며 t(i)는 현채 TS packet의 첫번째 by把가 T-STD에 도착하
              는 시간이다．
              LTW(logal time window）는 하나의 TS packet마다 설정된 시간상의
              구간으로써 그 패킷의 첫번째 byte가 LTW구간 내에 T-STD에 도달
              하면 入4Bn버퍼（비 디오의 경우）나 Bn버퍼（오디오의 경우）에서
              overflow i+ underflow가 발생하지 않는다는 것을 뜻한다. 이
              ltwH아Iset은 송신기나 재다중화기佃multi미exer）등 IS packet을 송신하
              는 측에서 header부분에 넣어주며 이 ltwHO瓜et이 작다는 것은 지연
              이 크다는 것이고（많이 기다려야 한다） 岫少承et이 크다는 것은 일
              찍 도착한다는 것이다. 만약 이 TS packet 이 t1(i)보다 늦게 도착하
              면 MBn이나 Bn버퍼에서 underflow가 발생하고 t0(i)보다 빨리 도착
              하면 ovefflow 7} 발생한다. 수신측에서는 t1(i)를 알치 못하며 이 IS
                                          7. 트랜스포트 스트림에서의 신택스와 의미



    packet의 도착시간인 t(i)를 측정하면 상한값인 t1(i)를 계산하1 낼 수
    있다. 이 t1(i)가 결국 그 패킷이 도착해야 하는 한계시간을 나타내
    거］ 된다． 따라서 이 佃四什set은 MBn버퍼제어에 쓰이는데 EBn버퍼
    에서의 vbvdelay역할과 비슷하다고 볼 수 있다. 또한 이 [TW의 구
    간인 [t0(i), t1(i月에서 t1(i)는 허용되는 최대 지연에 따라 정해지고
    t0(i)는 MBn버퍼사이즈와 MBn에서 EBn으로 전송되는 데이터율에
    의해서 정해지지만 이 入4PEG2 규격에서는 자세한 내용을 정의하지
    않았지만 앞의 T-STI) 모델에의 버퍼값 계산에서 이를 고려하여 겨］
    산할 수 있다．

piecewise_rate : 22 bits
  · ltw_flag= "l "이고 Itw_valid_flag = "1" 인 경우만 유효하다．
  · Itw_offset이 없는 TS packet의 경우에는 받는 쪽에서 l鈿 依町즉
    t1(i)값）을 계산하따따 하는데 이를 계산하기 위해서는 같은 PID를
    가지면서 ltw_o瓜et이 있었던 TS packet으로부터 유추해 낼 수 밖에
    없다． 이때 쓰이는 전송을 R은 어느 정도의 구간에서는 일정（piece-
    wise cons帥）하다고 가정하고 계산하는데 그때의 전송을 R을 이
    piecewis乞ra配변수에서 전송하게 된다．
  · 伽O依et이 있었던 IS packet 이후로 N개의 ltw 岱et이 없는 TS
    packet(물론 갇은 P11）를 갖는다）이 천송되고 그 (N+1）개의 packet들
    의 첫번찌1 byte들의 index가 八, 八＋1' ···, Ai+ N이라고 가정하면
    ltw_offset이 없는 두 번째 packet부터의 l吐砥et과 t,(Ai +j)는 다음
    과 갇이 계산한다

        tl（八日）=t1(Ai) +j 水 188 永 8/R (second) j= 1, 2, ..· 小1
        ltw_o什set = ti（八시） -1（八＋P, j= 1, 2, ...,r나

    여기서 i（八，9는 (i +j）번째 TS packet이 T-STD에 도착한 시간을 말
    한다．

piecewise_rate : 22bits
  · It꿔_flag과 ltw_valid_flag이 모두 " I " 인 경우에만 의미가 있다．
MPEG 시스템


           splice_ty比 : 4bits
             · 이 값이 일단 한번 존재하면 splice_countdown이 "0" 이 될 때까지（tt0ll
                 인 경우까지 포함） 그 뒤의 갇은 PB）를 갖는 모든 TS packet에서
                 이 값은 같게 유지되어야 한다．
                 elementa口 sUeam이 오디오신호면 이 값은 "0000"이 되어야 하고 비
                 디오신호면 profile, level, splice_t只玘값에 따라서 표 工6부터 표 7-15
                 에서처럼 정의된다．
             1
                 비디오 elementary stream은 다음과 갇은 조건을 만족시켜야 하는데
                 이때 splice_decoding_delay와 m炚_splice_ra妃값은 표 工6부터 표 工15
                 에서 구할 수 있다．


                             표； 7-6. Splice parameters table 1(MPEG Is: Table 2-8)

              罰n叩le I노oflie Main I月vet小4amn Profile 岫in I月vet, SNRI노硼eMaini上vet 伽th layers),
              Spatial Profile High-1440 Level (base layer), High Profile Main Level(middle + base layers)

              Splice_type                                      Cond小oils

              0000                 splice_deco玉ng_delay = 120ms; max_splice_ra把 = 15.0 X 106bit/s
              0X끄                  splice_deco血g_delay = 150ms; max_splice_ra把 = 12.0 X 106bit1s
              0010                 splice_decoding_delay = 225ms; max_splice_rate = 8.0 x 106bit/s
              0011                 splice_deco五ng_delay = 25야1ls; max_splice_rate = 7.2 x l戶bit/s
              0100-1011            reSelV出
              110O-1111            user니Jefined



                             표i7-7. Spli（羌 pars毗虹-s table 2小'IPEG Is: Table 2-9)

              入1amn Profile LA叭vi尤vet, SNR Profile I刃＼vi尤vet (b야h layers), I五gh Proffle 入'laini尤vel
              (base layer) Video

              Splice_ty光                                       Conditions

                                   splice_dec넘ing_delay = ll5ms; max_splice_ra把 = 4.0 x l06bitis
                                   splice_dec뇌ing_delay = 155ms; max_splice_rate = 3.0 x l伊bitJs
                                   splice_deco五ng_delay = 230ms; max_splice_rate = 2.0 X l06bitJs
                                   splice_decoding_delay = 250ms; max_splice_rate = 1.8 X l06bitls
                                   reserved
                                   user-defined
                                                7. 트랜스포트 스트림에서의 신택스와 의미


              표． 7-8. Splice paramet巴s table 3(MPEG Is: Table 2-10)

入4amn Pn而le }五gh-14401尤vel, Spatial F뇨）file I-地h-i的01月ye! (a]]나ayers), High Profile
I五합l-l4401尤vel (而ddie + base laye搭n八deo

Spli（氾누type                                     Cond消oils

                     splice_dec뇌ing_delay = 120ms; max_splice_rate = 60.0 X 1戶bi1/s
                     splice_dec刈1ng_delay = 1日ms; max_splice_rate = 45.0 x l戶bitJs
                     splice_deco如lg_delay = 240ms; max_splice_rate = 30.0 x 1戶bit/s
                     splice_decoding_delay = 250ms; max_splice_rate = 28.5 x 1戶bit/s
                     reserved
                    user-defined



              표7-9. Splice paramleters table 4(MPEG Is: Table 2-11)

Main Profile High Level, High Profile High-1440 Level (all layers), High Profile High
Level (middle + base layers) Video

Splice_type                                     Conditions

                     splice_d町세雎코elay= 120邸；maxU制ice_rate = 80.0 >< 仰bit's
                    splice_dec뇌ing_delay = 160ms; max_splice_rate = 60.0 x l06bitls
                    splice_dec넜ing_delay = 240ms; max_splice_rate = 40.0 x l (Pbitis
                    splice_decoding_delay = 250nis; max_splice_rate = 38.0 X l (Pbitls
                    reserved
                    user-defined



              표 7-10. Splice paramet크＄ table 5(MPEG Is: Table 2-12)

                       SNR Profile Low Level (base layer) Video

Splice_type                                     Conditions

0000                splice_decoding_delay = 115 ms ; max_splice_rate = 3.0 x lI戶 bit
                                                                                  's
0001                splice_decoding_delay = 175 ms ; max_splice_rate = 2.0 x 1戶 bit
                                                                                 's
0010                splice_decoding_delay = 250 ms ; max_splice_rate = 1.4 x 106 bit/s
0011-1011           reserved
lltlX工1111          user니：lefined
MPEG 시스템



                         표卜11. Splice parameters table 6(MPEG Is: Table 2-13)

                                  SNR P뇨）file卜vlainl月vel (ase lay町）Video

           Splice_type                                      Con小tions

           0000                 splice_decoding_delay = 115 ms ; max_splice_rate = 10.0 X 1戶 bit/s
           0001                 splice_decoding_delay = 145 ms ; max_spli玘_ 砒e = 8.0 X 1戶bit/s
           0010                 splice_decoding_delay = 235 ms ; max_spli玘_rate = 5.0 x 1戶 bit/s
           0011                 splice코ea妓咀由lay = 250ms ; max빠ce_rate= 4.7 x I（戶bit/s
           01(刃-1011            reserved
           1100-1111            user-d呱n出



                         표7-12. Splice parameters table 7(MPEG IS: Table 2-14)

                          Spatial Piofile High-1440 Level (middle + base layers) Video

           Splice_type                                      Conditions

                                splice_dec月ing_delay = 120 ms ; max_splic乙rate = 40.0 X 1伊 bit/s
                                splice_decod岬코elay = 16帥히 m吐叩奴ra把＝30.0x IC戶t寸t/s
                                splice_dec넜ng_delay = 240 ms ; max_splice_rate = 20.0 X 1戶 bit/s
                               spli（氾J奴M雎小lay= 250m히曲凡帥此니rate= 19.0x 1（戶 bit/s
                               reserved
                               user-defined



                         표7-13. Splice paramet日s table 8(MPEG Is: Table 2-15)

             High Profile Main Level (出l layers), High Profile High-1440 Level (base layer) Video

           Splicem打pe                                       Conditions

           0000                 spli：乞deco叩_delay = 120邸 ; m炚鉀奴J毗＝20.ox 1(戶bit/s
           0001                 spli（无J比（姓雎止lay = l60ms ; ma凡叩lice_rate= 15.Ox I（少bit/s
           0010                 splice_dec刈ing_delay = 240 ms ; max_splice_rate = 10.0 X 1伊 bit/s
           0011                splice_decodi眼delay = 25아ns; ni炚H叩奴_rate= 9.5 )< 1(戶t丘tls
           이00-1011            reserved
           1100-1111           user-defined
                                                     7. 트랜스포트 스트림에서의 신택스와 의미


                  표7-14. Splice parame也ls table 9(MPEG Is: Table 2-16)

                           High Profile High Level (base layer) Video

    Splice_type                                      Cond沁0I肖

    0000                 splice_decoding_delay = 120 ms ; max_splice_rate = 25.0 x 1戶bit/s
    ()(）아                splice_decoding_delay = 165 ms ; max_splice_rate = 18.0 x 106 bit/s
    0010                 sp血无뗘ec（寸踞J由片 250 n咨 ; m吐牡ice_rate = 12.0 x 仰bit/s
    0011-1011           reserved
    1100-1111           user-defined



                  표7-15. Splice parameters table 10(MPEG IS: Table 2-17)

                           High Profile High Level (all layers) Video

    Splice_type                                     Conditions

                        splice_decoding_delay = 120 ms ; max_splice_rate =100.0 x l戶bit/s
                        splice_deL乂ding_de1ay = 160 ms ; max_splice_rate = 75.0 x l06 bit/s
                        splice_dec뇌ing_delay = 240 ms ; m炚_splice_rate = 50.0 X 1戶bit/s
                        splice_decoding_delay = 250 ms ; max_splice_rate = 48.0 x 1伊 bit/s
                        reserved
                        user-defined



    Spli凹下ountdown이 0으로 되는 TS packet에서 끝나는 (oded picture의
    마지막 byte는 VBV bu珏er어］ (splice_decoding_delay - DP (k)）동안 머
    물러 있어야 한다. 여기서 DP（目는 n（目休번째 presentation unit）가
    재생되는 시간간격이며 k는 凡(iXi번째 access unit)가 위의 coded
    pict네七（splice_cout妃own이 0으로 되는 TS packet으로 끝나는）를 포함
    하도록 하는 J에서 tp (k) = td (j)가 되는 때의 값이다．
1
    VBV bu什er는 splice_decoding_delay 기간동안 max_splice_rate와 갇은
    고정비트율을 갖는 스트림으로써 입력이 절환되었을 때 절대 over-
    flow 7} 발생하면 안된다．
MPEG 시스템


           DTS_next_AV(decoding time stamp next ac戈弱 u沚t) : 33 bits
             · 어떤 splicing point에서 만약 spli面喀이 일어나지 않았거나 se町川ess
               splicing이 일어났다고 가정했을 때 splicing p이nt 바로 다음 access
                  unit의 디코딩시간을 나타낸다．
             · 이 디코딩시간은 splice_countdown이 되는 IS packet에서 유효한 由ne
                  base를 기준으로 표시한다．
                  이 값이 일단 한번 존재하면 splice_count面wn이 "0" 이 될 때까지
              1




                  ("0" 인 경우까지 포함） 그 뒤의 같은 P11）를 갖는 모든 TS packet어］
                  서 이 값은 같게 유지되어야 한다．

           stu町big_byte : 읾址ts
             1 "1111 1111"
             · 남는 공간을 메우기 위해서 사용하며 디코더에서는 버린다．




                                              PSI
                         (Program Specific Information)
                                                                      d
             PSI 정보는 표 7-16과 같이 4가지 테이블로 구성된다. 이 4개의 테이
            블은 TS stream어］ 따로따로 삽입된다．
              이 PSI 정보는 冗packet의 유료부하 부분에 삽입되는데 수신기에서의
            초기화등을 위해서 일정한 시간간격 내에 되풀이되어 전송되어야 하며，
            유료부하의 어느 부분에도 위치할 수 있다. 위의 테이블들은 앞에서도
            설명했듯이 각기 다른 PU)를 가지며, 한 개의 IS packet에는 한 종류의
            테이블만을 전송한다. 그러나 테이블의 길이가 킬 때를 대비해서 각 터］
            이블들을 한 7뀨 이상의 섹션Gcc如n）으로 나누며, 위와같이 MPEG2에서
            정의된 테이블들의 각 섹션의 길이는 최대 1024byte이다. 단 사용자가
                                                 7. 트랜스포트 스트림에서의 신택스와 의미


               표 卜16. 1뇨坦ram sr比cificini向rrnation小1PEG Is: Table 2-24)


  Str口cture Name       Stream Ty比     Reserved P11키               Description

                   rr냐TRec.
Program A駱（乂iation                 0x00
                                                        Associates Program Number and
                   H.222.0l
Table                                                   Program Map Table PID
                   ISO/IEC 138 恪-I

                     rru丁Rec.
                                     Assigned in the    Specifies PID values for compo-
Program Map Table    H.222.0 I
                                     PAT                nents of one or more programs
                     ISO/IEC 13818-1

                                                        Physical network p可ameters such
Network Infor好tion                    Assigned in the
                   Piivate                              as FDM frequencies, Transponder
Table                                 PAT
                                                        Nun寸姓s, etc.

                     ITU-TRec.                          Associates one ormore (private)
Conditional Access
                     H.222.0 I       0x0l               EMM streams each with a unique
Table                                                   PID v키ue
                     ISO/IEC 13818-1




정의하는 private section의 최대 길이는 4096by倪이다. 각 테이블의 뜻과
구성예는 앞의 5장 프로그램 절에서 설명한 바와 같다．
 유료부하 부분에 PSI 섹션이 있을 때는 TS packet header 부분에 있는
payload_unit_start_indicator = "1" 로 되고 그때 유료부하의 첫번째 byte가
표 7-17과 갇은 m뇨n妃rfield를 나타내게 된다. 이 p이nter_field는 pointer
mfield 바로 다음 byte부터 PSI섹션이 시작되기 바로 전 byte까지 간격
의 byte수를 나타낸다. PSI정보는 남는 공간에 쓸 수 있도록 하기 위
하여 유료부하의 어느 위치에서도 시작할 수 있게 했으며 이 p이nter
Hfield는 그 시작하는 위치를 나타내는 필드가 된다. 따라서 p이nter-
field = "0000 0000" 인 것은 pointer_field 바로 다음부터, PSI가 시작됨을
나타낸다．


          표7-17. Program specific information pointer(MPEG Is: Table 2-25)


                     Syntax             No. of bits         Mnemonic

                 pointer_field               8                uimsbf
0PAT(Program Association Table)

  PAT(program assoc油on岫le）의 졔층적 구조는 그림 工2와 갇고 각 섹션
은 표 7-18과 갇이 정의된다．

table id : 8bits
  · 표 7-19와 같이 PSI섹션의 정보가 어떤 것인가를 나타내준다．

section_syntax_in小cator: ibit



section_length : l2bits
  1 MSB 2bits는 "00"
  · 나머지 lOb畑가 羽ction_length 바로 다음 t乃te부터 섹션끝（CRC_32 포
    함）까치의 byte수를 나타낸다．
    한 섹션의 최대 길이는 lo24byte이고 羽（允on_len咎h까지가 3byte이므
    로 section_le雎th의 최대값은 1021 이다．

transport_streamjd : l6bits
  · 네트워크에서 이 1S steam을 알아보기 위한 레벨의 역할을 하며，
    사용자에 의해서 정의된다．

version number : 5bit
    PAT의 버젼을 나타낸다．


                 section               transport           current           last
      픕ble
                 syntax
                 indicator
                           0
                               Section stream 算 vera幻n next
                               leng仕1 id         二：
                                                 肖
                                                    number indicator
                                                                     section
                                                                     nun小er
                                                                             section
                                                                             number       匐   賢C
                                                                                                   犯
             8     1            12       16     2         5    l                      8


                                                                               program
                               program 穹 network              program
                               number 0 1: P11)               number I         map
                                                                               PID i
                                     陌    八4U
                                                l   n4J
                                                                   l
                                                                   /0    八4U
                                                                                  그
                                                                                  1
                                                                                  U
                 그림 7그. I거［ogram a莩DC at on 弱范on 小agram(viPEG Is: Figs丑'e F-3)
                                                    7. 트랜스포트 스트림에서의 신택스와 의미


  1
      PAT값이 한번 바뀔 때마다 l씩 증가한다（31까지 증가하면 다시 0
      부터 시작한다）.

cun七nt ne毗 in血沮切r : ibit
 · if("l ') : 현재의 PAT가 유효한 것이며, 현재 PAT에 있는 version
      num比r값이 유효한 PAT의 버젼값을 가리킨다．
      if("0") : 다음에 천송될 PAT가 유효한 것이라는 것을 나타내며 그
      PAT에 있는 vers幻n叫n比r값이 유효한 PAT의 버젼값을 가리킨다．


                표卜18. Pn增可na爵玭ation 曳ction小PEG Is: Table 2-26)


   匈口itax                                                No. of bits   八Ineni田nic

  pmgram_小socialion_section O {
            table_id                                              8    uimsbf
            弱出on_syntax_indic毗or                                  I    bslbf
             '0'                                                  1 bslbf
            reserved                                              2 bslbf
            section_length                                       12    uimsbf
            transport_stream_id                                  16    uimsbf
            reserved                                              2    bslbf
            version_number                                        5    uimsbf
            cunent_next_indicator                                 1 bslbf
            section_number                                        8    uimsbf
            last_section_num玘r                                    8    uimsbf
            for (i닉上 kN;什＋) {
                       pmgram_number                             16    uinisbf
                       reserved                                   3    bslbf
                       if(pmgram_number == 0) {
                                  network P1])                   13    uimsbf
                       }
                       else{
                                  program_map_PID                13    uimsbf
                       }
            }
            CRC 32                                               32 叩ch可
      }
MPEG 시스템


                         표7-19. table id a冬；ignment values(MPEG Is: Table 2-27)

                      Value                               Description

                     0x00                   pmgram_association_section
                     0x0l                   conl而on심4access配ction(CA_se力on)
                     敬02                     TSpro留mmapsecu이l
                     0x03-0x3F              ITU-TRec. H.222.0 I ISO/IEC 13818 reserved
                     0x40-0xFE              User pnvate
                     0炡下                     forbidden



           current ne砒 indicator: ibit
             · if("l") : 현재의 PAT가 유효한 것이며 , 현재 PAT에 있는 ye八幻nH
               nut汕er값이 유효한 PAT의 버젼값을 가리킨다．
             · if("O") : 다음에 전송될 PAT가 유효한 것이라는 것을 나타내며 그
               PAT에 있는 version num比r값이 유효한 PAT의 버젼값을 가리킨다．

           section number : 8bits
             · 이 섹션의 번호를 가리킨다．
             · 첫번째 섹션의 번호는 0이며, PAT의 섹션이 한 개 증가할 때마다 l
               씩 증가한다．

           last section number : 8bits
             · 마지막 섹션의 sect on끄urn比r를 표시한다．

           proram_number: l日：its
             · program_map_PID, 즉 프로그램 번호를 가리킨다．
             · 0값은 net씨ork P11）어］ 할당되어 있고 나머지 번호는 모두 사용자에
               의해서 사용되어질 수 있다. 그러나 PAT의 같은 버젼 내에서는 갇
               은 번호를 2번 이상 사용할 수 없다（예를 들어 방송채널번호를 이
               pro얍am_num比r어］ 할당해도 된다）.

           network P11) : l3bits
             · N1T(network i小orm的on小le) 정보를 담고 있는 IS packet의 PID를 가
               리킨다（그러나 표 7-2의 규정된 값을 이용해야 한다）.
                                                                 7. 트랜스포트 스트림에서의 신택스와 의미


pr恥ai兀map_Pifi : 13b沁
  ·program_map_section을 포함하는 TS packet의 PID를 가리킨다．
  · 프로그램 하나당 program_rn叩_PID(=PMT_PID）는 항상 한 개씩 할당
    되어야 하며, 표 7-2의 규정된 값을 이용해야 한다．

CRC 32: 32bits
  · CRC(circular iedundancy check）에서 32개의 레치스터값이 모두 0이 되
    거］ 하는 CRC값（다항식은 x32+ x26+ x23 +x22+ x'6+ x'2 +x'1+ x'0+ x8 +
    尸+ X5 +X4 +X2 + x + 1）을 사용
  · 6.2절의 （그R（二32 참조


1CAT(Conditional Access Table)

  CAT의 구조는 그림 工3과 같고 자세한 내용은 표 工20과 갇다．

table id : 8bits
  · 표 7-19와 같이 PSI 섹션의 정보가 어떤 것인가를 나타내준다．

section_synta足in小ca切r : ibit



section_len철世h : l2bits
  S 入4SB 2b抽는 "00"
  · 나머지 lObits가 sectior匕length 바로 다음 by把부터 섹션끝（CRC_32
    포함）까지의 t乃rte수를 나타낸다．
  · 한 섹션의 최대 길이는 1024byte이고 section_len曾h까지가 3byte이므
    로 section_length의 최대값은 1021 이다．



                 Section                                       current          last    N
                                      section        version            section
                 syntax           '                            next             section 30이：1
                                      leng由          number             number
                             'O
                 indicator                                     indic카or         number descriptors
      픕ble
                                                                                                     努C
             8      l             1 2 12        18     5          l       8        8                      32


                 그림 卜3. Conc五tional ac（生兮； 配Cti이l 小a肛am(MP且；Is: 夙gure F-4)
MPEG 시스템



                                표卜20. Conditional acm弱 羽otion(MPEG Is: Tabl巳 ?28)


                 Syntax                                                No. of bits   入nemonic

                 CA_section() {
                          table_id                                              8    uimsbf
                          section_syntax_indicator                              1    bslbf
                          'O'                                                   I    bslbf
                          reserv出                                               2    bslbf
                          section_length                                       12    uimsbf
                          reserved                                             18    b北f
                          version_number                                        5    uimsbf
                          current_next_indicator                                1    bslbf
                          section num比r                                         8    너msbf
                          last_section_num玘r                                    8    uimsbf
                          for (i=O; kN;i-f+) {
                                 descriptor()
                          }
                          CRC 32                                              32     叩chof
                 }


           transport_streamjd : l6bits
             · 네트워크에서 이 TSsneam을 알아보기 위한 레벨의 역할을 하며，
                 사용자에 의해서 정의된다．

       version number: 5bit
            ·CAT의 버젼을 나타낸다．
            1CAT값이 한번 바뀔 때마다 1씩 증가한다（31까지 증가하면 다시 0
                 부터 시작한다）.

       current next indicator: ibit
            1if('l ") : 현재의 CAT가 유효한 것이며, 현채의 CAT에 있는 version
                 num比r값이 유효한 CAT의 버젼값을 가리킨다．
                 if("O") : 다음에 전송될 CAT가 유효한 것이라는 것을 나타내며 그
             1




                 CAT에 있는 ye八幻n_num比r값이 유효한 CAT의 버젼값을 가리킨다．
                                                                        7. 트랜스포트 스트림에서의 신택스와 의



section nt괴［ni：거己r : 8bits

  · 이 섹션의 번호를 가리킨다．
  · 첫번째 섹션의 번호는 0이며, CAT의 섹션이 한 7뀨 증가할 때마다
       l씩 증가한다．

last section number: 8bits
  · 마지막 섹션의 S凹面n_num比r롤 표시한다．

CRC 32: 32bits
  · CRC(ciitul町redundancycheck）에서 32개의 레지스터값이 모두 0이 되
       거］ 하는 CRC값（다항식은 X32 +X26 +X23 +X22 +X16 +Xl2 +Xn +Xl0 +X8 +
       X7+ X5 +X4 +X2 + x + 1）을 사용
   1
       6.2절의 CRC_32 참조


.P卜八T(Progran} 入iap Table)

  PMT의 구조는 그림 7-4와 같고 자세한 내용은 표 7-21과 같다．



                  section                                              current           last
                                         section program       version           section             PCR
                  syntax            그1                                 next              section
                                         length number         number            number              PID
                              101
                  indicator                                            indicator         number
       픕ble
              8               12          12      16       2        5        l         8     8     3 134



                                    program      N
                                    info         loop               Nl。。p    CRC 32
                                    length       descriptors




                                                    stream          elementaiy       ES it寸O N
                                                    type            PID              length loop
                                                                                            descriptors
                                                       8        3       13       4     12


                    그림 卜4. Th i且＼igrarn map 弱出예 diagram(MPEG IS: 珌gure F-5)
MPEG 시스템


                          표 7-21. Transport Strnsm program map 配ction(MPEG IS: Table 2-29)

                 Syntax                                                   No. of bits     Mnemonic

                 TS_pro胛m....map毗tion( ) {
                                                                                    8
                       table_id                                                    8      uimsbf
                                                                                    1
                                                                                    1
                            sect由n_syntax_in血：a幻r                                  I      bslbf
                                                                                    l
                            'O'                                                    1      bslbf
                                                                                    八
                                                                                    乙
                            reserved                                               2      bslbf


                                                                                  l l ／
                                                                                    八
                                                                                    乙
                            section_len曾h                                         12      uimsbf
                                                                                      n
                                                                                    /
                                                                                    b
                            program_numb江                                         16      uimsbf
                            reserved                                               2      bslbf
                                                                                    느＜
                                                                                     口
                            ve八ion_number                                          5      山msbf
                                                                                    l
                            cunent_next_indic趾or                                   1      bs小f
                                                                                    8
                            sec的n_num比r                                            8      uimsbf
                                                                                    8
                            last_section_number                                    8      uimsbf
                                                                                    n
                                                                                    4
                                                                                    V
                            reserved                                               3      bs出f
                                                                                  l 八
                                                                                    4
                                                                                    U
                            PCR_PID                                               13      uimsbf
                                                                                    4
                            reserved                                               4      bslbf
                                                                                  l 2
                            program_info_length                                   12      uimsbf
                            如r（江0; kN; i卄）{
                                    descriptor()
                            }
                            for (i=0;kNl;i++) {
                                                                                    8
                                    stream ype                                            uimsbf
                                                                                    n
                                                                                    4
                                                                                    V
                                    reserved                                              bslbf
                                                                                  l 八
                                                                                    4
                                                                                    U
                                    elementaiy_PID                                        uimsnf
                                                                                    4
                                    reserved                                              bslbf
                                                                                  l D
                                                                                    4
                                    ES_info_length                                        uimsbf
                                    for (i=(）水N2; i卄）{
                                            descnptor()
                                    }
                            }
                           CRC 32                                                32       rpchof
                 }


           table id : 8bits
             · 표 7-19와 같이 PSI섹션의 정보가 어떤 것인가를 나타내준다．

           section_syntax_indicator: ibit
                 I 'll,
             1
                                 7. 트랜스포트 스트림에서의 신택스와 의미



section length: l2bits
  S 入ISB 2bits는 "00"
  · 나머지 lOb畑가 section_length 바로 다음 byte부터 섹션끝（CRC_32
       포함）까지의 by把수를 나타낸다．
  · 한 섹션의 최대 길이는 1024byte이고 section_leng由까지가 3hyte이므
       로 sectio凡le曜由의 최대값은 1021 이다．

program_number: l6bits
  · 하나의 프로그램에 대한 구성은 하나의 TS_prograrn_map_section에서
       전송되는데 현재 TS_pmgram_map_section을 나타내는 prograrn_num比F
       를 나타낸다．
       프로그램에 대한 설명 또는 정의는 최대 10拓切妃까지 허용된다．

version number: 5bit
  .1-s-I加얍arnm叩S帥on의 버젼을 나타낸다．
  · TSpro얍跏_map_section값이 한 번 바뀔 때마다 1씩 증가한다（31까
       지 증가하면 다시 0부터 시작한다）.

cun＼三nt i妃毗 indicator : ibit
  · if("l") : 현재의 宿-plo胛rn_map_s凹tion이 유효한 것이며 , 현재의 l 's
       -I加얍帥mape記ction어］ 있는 version_num比r값이 유효한 TS ）畔ram
       map_section의 버젼값을 가리킨다．
   1
       if("O") : 다음에 전송될 lSJm얍arnm叩section이 유효한 것이라는
       것을 나타내며 그 PSpn)帥rn_map_section어］ 있는 ver如n_num比r값
       이 유효한 TSpm留帥_map_section의 버젼값을 가리킨다．

曳Ction number : 8bits
  .O] 섹션의 번호를 가리킨다．
  · 첫번째 섹션의 번호는 0이며, 1's_i加gramm叩J凹tion의 섹션이 한
       7긔1 증가할 때마다 1씩 증가한다．

last section number: 8bits
  · 마지막 섹션의 so曲on_nur毗or를 표시한다．
MPEG 시스템


           PCR Pifi: l3bits
             ·pro帥m_num比r가 가리키는 프로그램에서 쓰는 유효 PCR을 갖고
                 있는 TS packet의 P11）값을 나타낸다．
             1                                                  O
                 어떤 sli     이 PCR과 관계없는 것일 때                         PCR나PID값은 모든 bit
                 가 I로 되어야 한다．

           program寸I]小0_len멥h : 12b沁
            . 入4SB 2bit는 "00"
            · 나머지 ]Obit는 program_info_length 바로 뒤에 나오는 descriptor( ) 길
                 이의 byte수를 나타낸다．

           Shmm寸bpe : 8b沁
            · elemen沮口1PID에서 표시된 P표）값을 갖는 packet어］ 들어있는 program
              element의 타입을 나타낸다（표 工22).


                          표． 7-22. Streani type a ignnnts(MPEG Is: Table 2-36)

              Value                                    Description

              0x00             ITU-T I ISO/EEC Reserved
              0x0l             ISO/EEC 11172 Vid以
              0x02             ITU丁 Rec. H.262 I ISO/IEC 13818-2 Video or ISO/IEC 11172-2
                               constr小ned p出ameter video stream
             0x03              ISO/EEC 11172 Audio
             0M놔              ISO/EEC 13818-3 Audio
             0x05             ITU-T Rec. H.222.0 I ISO/EEC 13818-1 private_sections
             0x06             ITU-T Rec. H.222.0 I ISO/EEC 13818-1 PES packets containing
                              private data
             0x07             ISO/EEC 13522 MHEG
             敬（好              ITIJ-TRec. H.222.0 I ISO/EEC 13818-1 Annex A DSM CC
             敬（刃              ITU-TRec. H.222.l
             0x0A             ISO/EEC 13818-6typeA
             0x0B             ISO/EEC 13818-6typeB
             0X（兀             ISO/EEC 13818-6typeC
             0x0D             ISO／任兀 13818-6 type D
             0x0E             ISO/EEC 13818-1 auxiliary
             0X0F-0X7F        1W丁 R凹. H.222.0 I ISO/I且二 13818-1 Reserv旼l
             0x80-Oxl下        User Private
                                                             7. 트랜스포트 스트림에서의 신택스와 의미


elementa工PID: l3bits

  · 그 pmgram ci帥'ent들이 들어있는 TS packet의 P11）값을 나타낸다．

ES_info_length : l2bits

  S 入ISB 2bit는 "00"
  · ES_info_len曾h 바로 뒤에 있는 descriptor() 길이의 b少e수

CRC 32 : 32bits

  · CRC(circular redundancycheck）에서 32개의 레지스터값이 모두 0이 되
     거］ 하는 CRC값（다항식은 x32+ x26+ x23 +x22+ x16+ x12+ x"+ x'0+ x8 +

     x7+ x5+ x4+ x2+ x+ 1)을 사용
     6.2절의 CRC_32 참조


 0
     Private sed沁n의 신택스

 Private section의 구조는 그림 工5와 같고 자세한 내용은 표 工23과

같다．



                   section                         pnvate
                                   pnvate
                   syntax                          section
                                   indicator
                   indicator                       length
       픕ble
              8       l               l        2       12




                                          N private data bytes




                  table                        current              last    N
                                   version                  section
                  id                           next                 section pnvate
                                   number                   number
                  extension                    indicator            number data
                                                                                     發C
                    16         2          5        l                                      32


                    그림 7-5. Private 曳etion 小agralrl(l뇨'IPEG Is: Figuxe F-6)
                                  MPEG 시스템


                                                                             표7-23. Private 田tion(MPEG Is: Table 2-30)


                                                     Syntax                                                      No. of bits   Mnemonic

                                                    private中sect幻n( ) {
                                                              table id                                                    8    uimsbf
                                                              section寸syntax_in小C趾or                                      1    bslbf
                                                              pnvate_mdic趾or                                              1    bslbf
                                                              reserved                                                    2    bslbf
                                                              priva妃H記ction_len멤                                         12    uimsbf
                                                              if (section_syntax_indicator== 'cO {
                                                                         for ( i닉）;i<N;i-H-) {
                                                                                    pnvate_da奴上yte                        8    bslbf
                                                                         }
                                                              }
                                                              else {
                                                                         tab追뽀1e胤ens幻n                                   16    uimsbf
                                                                         reserved                                         2    bslbf
                                                                         vers幻n_num比r                                     5    uimsbf
                                                                         current_next- indicator                          1    bslbf
                                                                         section_i仙祉壯                                     8    uimsbf
                                                                         last s伐由n_number                                 8    uimsbf
                                                                         如r (i=가i<pnvat乞配ction士咽h-9小＋) {
                                                                                  private_data_byte                       8    bslbf
                                                                         }
                                                                         CRC 32                                          32    rpchof
                                                               }
                                                        }


                                                 table id : 8bits

                                                   · 표 7-19와 갇이 PSI 섹션의 정보가 어떤 것인가를 나타내준다．

                                                 section_syntax_indicator: ibit
                                                    1
                                                        if("1") : t刪e_id_e帥sion, version_number, cunent_next_indicator, se比ion_num-
                                                        比r, la筵S凹tion_num比r가 기술된 후에 口如ate나dat之切把가 따라온다．
                                                        if("O") : proviate_sectionjength 후에 곧바로 priva妃4dat之旬te가 따라
                                                    1




                                                        온다．




         咐呻m鹹姚m幽                       朴難燐難簞羅艅
                   難
饌難
 嫩mm排m
         雛                  難
                            叫
                           湃滋
                             懈m
                                  懈跏
                   螂
                       啣
                           朴
                           唯砒
                       艸
                       艸
                       啣
                       娜
                                  7. 트랜스포트 스트림에서의 신택스와 의미


11加ate_indica的r : ibit
   · 사용자들이 특수한 목적에 쓸 수 있는 flag

private_sectionJength : l2bits
   · private_s凹由n_leng由 바로 뒤의 byte부터 private section이 끝나는 byte
     까지의 byte수
   · 이 값은 4093보다 클 수 없다．

11加a虹data_byte :
  · 사용자 데이터

table id extension: l6bits
  · 사용자가 정하고 이용할 수 있다．

version number: 5bit
  · priva妃S凹tion의 버젼을 나타낸다．
  · pnv毗J凹tion값이 한 번 바뀔 때마다 1씩 증가한다（31까지 증가하
    면 다시 0부터 시작한다）.

cur七nt next indicator: ibit
  · if("l") : 현재의 privat口section이 유효한 것이며, 현재의 private_
    羽ction어］ 있는 ye八幻n_num比r값이 유효한 priva把卞記ction의 버젼값을
    가리킨다．
  · if '0") : 다음에 전송될 private_s凹tion이 유효한 것이라는 것을 나타
    내며 그 private_section어］ 있는 ye八幻n批m比r값이 유효한 private_
    section의 버젼값을 가리킨다．

section number: 8bits
  1 이 섹션의 번호를 가리킨다．
  · 첫번째 섹션의 번호는 0이며, pnva妃J凹tion의 섹션이 한 개 증가할
    때마다 l씩 증가한다．

Last section number: 8bits
  · 마치막 섹션의 section_num比r를 표시한다．
MPEG 시스템


           piivate_databyte
             I 사용자가 쓸 데이터 부분

           CRC 32: 32bits
             ·CRC(circular tedundar兀ycheck）에서 32깨땍 레지스터값이 모두 0이 되
                 거］ 하는 CRC값（다항식은 X32 + x26 +X23 +X22 +Xl6 +Xl2 + xli + x'0 +X8 +
                 尸 + X5 + x4 + x2 + x + 1）올 사용
             1
                 6.2절의 CRC_32 참조
                               8. 프로그램 스트림에서의 신택스와 의미




                                           즈工 무 m 1 래
                                          中14H         나艸     I- I


                            스트림에서의
                            신택스와 의미




 PS stream에서는 packet 대신 pack이라고 한［:}. Pack에서는 pack hea（畑가 있으며, 일반적으
로 packet보다 킬이가 킬D. 또한 전송을 목적으로 하기보다는 주로 저장을 목적으로 이용된CF.
                 MPEG 비디오




      *.*
                               卜                           프로그』스트」 1                                               2   .      pack
                                      PS stream어］서는 packet대신 pack이라고 한다. Pack에서는 pack header가
                                     있으며 일반적으로 packet보다 길이가 길다. 또한 전송을 목적으로 하기
                                     보다는 주로 저장을 목적으로 이용된다. Pack의 계층적 구조는 그림 8-
                                     l과 같다. PS stream은 연속적인 pack들로 구성되면 모든 pack들이 끝나


                                        13818                                                                                          小
                                                           pack                          pack
                                        Program                            pack 1                         pack 2
                                                                                                                                       耐
                                                                                                                                             pack n
                                        Stream             header                        header                                        岫
                                           pack                    program              pack

                                       隘
                                                                                                     pak     syrtem
                                           start               SCR mux                  stuffing     stuf丘hg                 PES packet 1
                                                     '01   '




                                                                                                             he拍er
                                           code                    ra妃                  leng由        byte '




                                                                                                PES packet n


醫瑟難難；;
難難莩．纛難難：
驀鑿醬難舅
                                           system
                                                                                                              audio        video
                                           header header rate  audio                                                                 video
                                                                                                              lock         lock
                                           start  length bound bound                                                                 bound 卜1的이：1
                                                                                           隘d        諱S
                                                                                                              flag         flag
                                           code

                                            32                 16         22        6           1         l                           5



                                                                           P-STD         P-STD
                                                   stream                  buffer        buffer
                                                   id               'IF    bound         size
                                                                           scale         bound

                                                           8          2        l                13
                       ．聲景旨蹄籬三卦
                                                       그립 小1. Pm酊amstl毛am diagram(MPEG Is: Fi肛reF小7)
    驀醬誓
                    ::．芎”
                       :.:..；蘿轟難纛藝
                    羅難難퓽罐簪．聲
                     羅巍幾難｝:；轟轟｝
            艅雀咨釜牡旨玆瑾毖弑瑾i斜堪赫薑瑾方旨
                                                      8. 프로그램 스트림에서의 신택스와 의口



면 맨 뒤에 있는 MPEQprogram_end_code(00(刃0]B9(H)）가 붙게 된다．
Pack header 구성은 표 8-1과 같고 pack의 유료부하에는 PES packet이 들
어간다．


                표8-1. Program stream pack header(MFEG Is: Table 2-33)

   Syntax                                                    No. of bits     Mnemonic

   pack_header() {
                                                                     八
                                                                     J
                                                                     e
           pack_start_code                                           32
                                                                     그
                                                                     U
                                                                             bslbf
                                                                      ／
                                                                      八
            '01'                                                      2      bslbf
                                                                       q 각
                                                                         口
            system_cl乂k_reference_base[32..30J                        3      bslbf
                                                                       l
            marker_bit                                                1      bslbf
            system_clock_reference_base[29..15]                      15      bslbf
            marker_bit                                                1      bslbf
            system_clock_reference_base[14..0]                       15      bslbf
            marker_bit                                                1      bslbf
            system_clock_reference_extension                          9      uimsbf
            marker_bit                                                1      bslbf
            pr唯rat兀m때_rate                                           22      uimsbf
            marker_bit                                                1      bslbf
            marker_bit                                                I      bslbf
            reserved                                                  5      bslbf
            pack_stuffin且leng由                                        3      uimsbf
            for 乍0;kpac（如ffing_length;i卄）{
                    stuffing1byte                                     8      bslbf
            }
            if (nexthits( ) == system_header_start_code) {
                    system_header O
            }
   }

pack_start_code : 32bits
  1 000001BA(H)

system下뇨kHre屯ence上ase : 32b1ts

SySem_clock_reference_base_extension: 9bits
  · SCR을 표시하는 42bits
  · 5.5절에서 설명
MPEG 비디오


           m町ket bit: ibit



           pmgrammux_rate : 22bits
             ·PS stream을 생각할 때 P-s-n）가 pack을 받는 byte율
             · 새로운 값이 주어지기 전까지는 갇은 stream의 pack들에서 이 값은
                 유효하다. 그러나 같은 pack stream에서 극단적으로 pack마다 값이
                 바뀔 수 있다．
             1
                 50bytes/second 단위로 계산（즉, program_mnx_rate = 10이면 초당
                 500byte의 pack stream을 받는 것）
             1
                 0값 사용금지
             · 이 값을 P-S-ri刈 입력단에서 pack의 byte들이 도착하는 시간을 계
                 산하기 위하여 사용된다．

           pack_stuffingjen인：h : 3bits
             · 이 pa味ste佈叩_length 바로 뒤에 오는 ste飯n且切te들의 byte수

           stuffing中byte:
             1 "1111 1111"
             · 빈칸을 메우기 위하여 사용

           systemmheader()
             · 8.2절에서 설명




    卜                                System header



             System header의 구성은 표 &2와 갇다．
                                               8. 프로그램 스트림에서의 신택스와 의미



                표 8그. }뇨gram Stream system header小作EG Is: Table 2-34)

   Syntax                                                No. of b沁    入Inemonic

   system_header () {
           system_header_start_code                             32    bslbf
           hear把乙length                                         1t    uimsbt
           marker bit                                            1    bslbf
           late bound                                           22    uimsbf
           marker bit                                            1    bslbf
           au小ob에ad                                              t    ulnlsbt
           ：fi 乂ed：卄flag                                         1    bslbf
            CSPS_flag                                            1    bslbf
            sys把m1au（五o1li乂k_flag                                1    bslbf
            system_videoJock_flag                                1    bslbf
            marker bit                                           1    bslbf
            video bound                                          >    uimsbt
            packet_rate_restnction_flag                          I    bslbf
            reserved_byte                                        7    bslbf
            while (nextbitsO=='l') {
                                                                 8
                      stream id                                         uirnsbf
                                                                 n乙
                      '11' e                                            bslbf
                     P-Sm buffer bound scale                     I      bslbf
                     P-Sm buffer si四 bound                      13      uimsbf
            }
   }

町stem_header_start_code: 32bits
  1 00000IBB(H)

header Jength: l日：1its
  · header_length 바로 뒤 byte부터 system header의 마지막 byte까지의
       切巾e수；

rate bound : 22bits
  · PS stream의 pack들에 있는 P11凹am_mu＼只妃의 최대값보다 같거나
       큰 상한값
  · 이 상한값을 기준으로 시스템 디코더는 그 mstream을 디코딩할 수
       있는가 없는가를 가늠한다．
MPEG 비디오


           audio bound : 6bits
             · 디코딩이 진행중일 때 入4PEG1 또는 MPEG2의 audio str町Ti의 개수
              （예를 들어, 스테레오는 2, 5.1 채널은 6）의 최대값보다 갇거나 큰
                  상한값 )
             .0부터 31까지의 값을 갖는다．

           fixe&flag: ibit
             ·if ('l ") : 고정 비트율（fixedb虹ate)
             ·if ("O") : 가변 비트율（van的le帥rate)
             · 고정 비트율인 경우 SCR 변수는 다음 식을 만족해야 한다．

                       SCR_b口Se(i) = ((ci * i + c2) DIV 300) % 233
                       SCR_exl(i) =((cl * , + c2)DIV 1) % 300

                  여기서 ci과 c2는 모든 I어］ 대해서 유효한 실수값을 갖고 있는 상
                  수이며, i는 system_dc兀kref毗nce 필드의 마지막 bit를 포함하는 byte
                  의 인덱스이다．

           CSPS-flag: ibit
             · if("l") : 부록 l의 cSPS의 제한 조건을 만족시킨다．

           system_audioJock_flag: ibit
             · if("i ') : PS stmairi의 모든 audio elementa口 SneTi에서 다음과 같은
                  SCASR이 항상 일정하고 표 &3을 만족한다．

                           SCASR=              systemH clock - frequency
                                        audio - sample - rate - in - the - P - STD


             여 기人1 1. 는 실수연산을 나타낸댜．
              -    -   .    x_      .   .   ,   .   .   八   .   .   .   .




                            I



           systemmvideo Jock-flag : ibit
             · if(I) : PSs甘帥Ti의 모든 video elementary s仕earn에서 다음과 같은
                  SCPR이 항상 일정하고 표 8-4를 만족한다．
                                                8. 프로그램 스트림에서의 신택스와 의미


                                    표 &3. SCASR

Nominal audio sam-
pling fiequency(k七)
                          16        32        22,05        44,1         24        48


SCASR                 刃（11)(11)   刃（xx1o 27111XX1J 刃（11)q1) 刃（11X11) 刃（11Xn)

                         16000     160(X)    16000     16000           16000     16000



                                     표． 8-4. SCPR

Nominal picture
rete仕i기         23,976      24      25      29,97     30          50     59,94     60


SCPR           1126125 1125(11) l（표XXX) 900900 엊刃 900 540 000 450 450 4500(X)



    SCPR이 고정값이기 때문에 normal picture rate값이 23.976, 29.97,
    59.94인 경우에 실제의 pictu肥rate는 약간씩 다르게 된다．

video bound : 5bits
  · 디코딩이 진행될 때 入'IPEGi 또는 MPEG2의 video stream의 개수（예
    를 들어 입체 영상인 경우는 2）의 최대값보다 갇거나 큰 상한값
  ·0부터 16까지의 값을 갖는다．

packet_rate_restriction_flag: ibit
  · if(CSPS_flag = 1) : CSPS의 조컨이 부록 I어］ 있는 것처럼 바뀐다．

reserved_byte : 8bits
  1 "1111 1111"

st七am id : 8bits
  · if("lOll 1000") : 뒤의 P-s기口加珏아_bound_scale과 P-sm上u卄er Si配e
    比und가 PS stream에서의 audio stream어］ 관계된다．
  1 if(1011 1001) : 뒤의 P-STD_bu仟er_bound_scale과 P-si그D.Hbu什er_size小
    比und가 PS없xam에서의 vidio stream어］ 관계된다．
  · 만약 " 1011 1100" 보다 크거 나 같은 다른 값을 갖는다면 표 6-2와 같
    은 경우를 나타낸다．
MPEG 비디오


           P-STh buffer bound scale: ibit
             · P-STI工buf佃j刃und_sca把과 p-sm上咐er_size士ound는 PS stream의 각
              elementaiy stream에서 system_header에 딱 한번 언급된다．
             · stream_id가 audio stre쏘TI이면 이 flag값은 "0"
             ·stream Id가 vid凹stream이면 이 flag값은 " 1"
             1 다른 stream어］ 대해서는 "0" 또는 "1"

           P-STD buffer 前ze bound: l3bits
             · P-STI）의 버퍼 크기인 BSn의 최대값보다 크거나 같은 상한값
             . if(P-STD_buffer_bound_scale == "0")

                             BS 드 /) 小 STD加和乙毗e加undX 128;

             · if(P-STD_buffer_bound_sc고e == "1")

                             BS 드 /) -m）卞bu和r＝缸ze血兀4fldX 1024;
                                                  9. 서술자




                                         서술자




 서술자（descriptor)는 口0아am과 마0아am 이ement룔 규정하기 위하여 사용되어지는 것으로
모든 descript아는 des에ptor_tag와 descript아_Iength로 시작된다．
MPEG 비디오




           .     프로그램과 program 이ement으1 서술자

            서술자（Descriptor) 는 Pr唯ram과 pro얍an比lement를 규정하기 위하여 사
           용되어지는 것으로 모든 descri꺄아는 desc如tor그ag와 descriptor_leng小로
       시작되는데 이 두 변수는 공통으로 등장하는 것이므로 미리 살펴보고
       들어가도록 한다．


                     표 9-1. Pro冒am 카id progr키n element dd）그iptors小IPEG Is: Table 2-40)


               descriptor_tag    l 's     PS                         Identification

                     0          n/a       n/a      Reserved
                     l          n/a       n/a      Reserved
                     2           x        x        video_stream_descriptor
                     3           x        x        audio_stream_descrip的r
                    4            x        x        hierarchy_descriptor
                    5            x        x        re멉strat如n_desciii荒or
                    6            x        x        data_stream_alignment_descriptor
                    7            x        x        target_background_grid_descriptor
                    8            x        x        너deo_window_descriptor
                    9            x        x        CA_descriptor
                    10           x        x        ISO_639_language_descriptor
                    11           x        x        system_clock_descriptor
                    12           x        x       multiplex_buffer_u出ization_descriptor
                    13           x        x       copyright_descriptor
                    14           x                maxim山ll bitrate descriptor
                    15           x        x       private data indicator descriptor
                    16          x         x       smoothing buffer descriptor
                    17          x                 Si]工descrip卜or
                   18           x         x       IBP descriptor
                  19-63         n/a      n/a      ITU-T Rec. H.222.0 I ISO/lEC 13818-1 Reserved
                 64-255         n/a      n/a      User Private
                                                                                    9. 서술자


descriptor_tag: 8bits
  · 각 descri아아를 표 9-1과 같이 규정한다（표 9-1에서 x표시가 있으면
    그 descri만아가 l 's나 PS stream어］ 적용된다는 것을 뜻한다）.

descriptor_length : 없血S
  · 이 descriptor_length 바로 다음 byte부터 descriptor 끝까지의 byte수


DVideo stream descriptor

  Vid的S岫m descriptor는三 비디오 elementa口 stream의 기본적인 코딩파라
메터를 서술한다．


m네iple_frame_rate_flag: ibit
  · if("l") : video stream에 fran妃rate가 여러 711 존재한다는 것을 나타
    낸다．
  · if('O") : 오로지 한 개의 frame rate가 존재한다．


                   표． 9口. Vidre stx毛am de얹그iptc才小IPEG Is: Ta比1 2-41)


    Syntax                                                 No. of bits   Mnemonic

    video_stream_descriptor( ){
             descnptor_tag                                          8    uimsbf
             descnptor_length                                       8    uimsbf
             multiple_frame_rate_flag                               1    bslbf
             frame rate code                                        4    uinisbf

                                                                                             m
                                                                                             ;：丘；裝：
                                                                                                  ：裝丘
             入IPEG_1_only寸flag                                      I    bslbf
             constrained_param把r_flag                               1    bslbf
             still_picture_flag                                     1    bslbf
             if (I｛旺iG그_only_flag == 1){


                                                                                             m
                     pr呱畦an町ev吐血dicat由n                              8   uimsbf
                      c뇨이na 如m俎t                                     2   uimsbf
                      frame_rate_extension_flag                      1   bslbf
                      reserved                                       5   bslbf
             }
    }
MPEG 비디오


           frame rate code : 4bits
             ·MI표｝2 video sequence heat把r에서의 frame rate code와 갇은 값을 갖는다．
             · 다만 위의 multiple小Bme_r毗小fi雎= Ill " 로 되면 표 9-3의 오른쪽 부분
                 과 갇은 framera妃들이 여러 개 존재한다（예를 들어 multiple士ame
                 rate_flag = "1" 이고 frame_rate_code = 30.0이면 23.976, 24.0, 29.97까지
                 포함해서 도합 4개의 丘ame ra妃가 존재함을 의미한다）.


                              표9-3. F쾨l玘 rate code(MPEG Is: Table 2-42)

                                               also includes

                              23,976
                              24,0             23,976
                              25,0
                              29,97            23,976
                              30,0             23,976 24,0 29,97
                              50,0             25,0
                              59,94            23,976 29,97
                              60,0             23,976 24,0 29,97 30,0 59,94


           MPEG_i_only_flag: ibit
             · if("l") : 오로지 入4PEG1 video stream만을 포함한다는 것을 뜻한다．
             ·if ("O") : 그 video stream이 八4PEG1 또는 入41毛G2 video stream을 포함하
                 는 것을 뜻한다．

           constrained下arameter flag: ibit
             1 MPEG_I_only_flag = "1" 이면 이 값은 무조건 " 1"
             · if("l") : 그 너d凹stream이 unconstrained入4PEG1 비디오 데이터를 포
                 함하지 않는다．
             1
                 if("O") : 그 video stream이 constrained parameter 및 uncons仕ained入IPEGi
                 vid印stream을 포함한다．

           sfream_picture_flag: ibit
             1
                 if("1") : 그 vid凹stream이 정지 영상（still pictu配）만은 포함한다．
             1
                 if("O") : 그 vid凹stream이 정지（sti끄pict毗） 또는 동영상을 포함한다．
                                                                                    9. 서술자


proffle_andJevel_indication : 8bits
   1
       入4PEG 비디오 파트의 Pr可ii口and_level_indic曲이1 변수값과 갇다．

chroma format: 2bits
   · 入JPEG 비디오 파트의 chmmafomat 변수값과 같다．

frame_rate_extension_flag : ibit
   · if("l") : 入WEG 비디오 파트의 frame_rn也1ex妃nsion寸n와 frame rateH

       ex妃nsion크 중 적어도 하나는 0이 아니다．


0Audio stream descriptor

  A岫o stream descriptor은 오디오 elementaiy stream의 기본적인 코딩파라
메터를 서술한다．


free_format_flag: ibit
  1 if("1") : audio stream의 bitrate_index = "0000"
  1 il("0") : biti-ate_index 手 "0000"

ID: ibit
       audio stream의 ID값과 같다．

layer : 2bits
   1
       audio stream의 Ia玎er값과 갇다．


                  K 9-4. Audio stream denriptor(MPEG IS: Table 2-43)

   Syntax                                                  No. of bits   人nemonic

   audio_stieam_descriptor( ){
            descdPtorJag                                            8    uimsbf
            descnptor_length                                        8    uimsbf
            free_format_flag                                        1    bslbf
            ID                                                      1    bslhf
            layer                                                   2    bslbf
            vai-iable rate au小o ndi cator                           1    bslbf
            reserved                                                3    bslbf
   }
MPEG 비디오



                               표； 9-5. 1五erarchy de요그ir巾才小PEG Is: Table 2-44)

              Syntax                                                 No. of bits          Mnemonic

              川erarchy_descriptor() {




                                                                                8 8 4 4
                      descnptor_tag                                                       uimsbf
                       descriptor_length                                                  uimsbf
                       reserved                                                           bslbf
                       hierarchy_type                                                     uimsbf
                                                                                乙
                                                                                n
                       reserved                                                           bslbf
                                                                                6
                       hierarchy_layer_index                                              uimsbf
                                                                                乙
                                                                                n
                       reserved                                                           bslbf
                                                                                6
                       hierarchy_embedded_layer_index                                     uimsbf
                                                                                乙
                                                                                八
                       reserved                                                           bslbf
                                                                            b
                                                                            /
                       hierarchy_channel                                                  uimsbf




           variable rate audio indicator: ibit
             · if( 'l ') : 관련 audio stream이 bit끄ite가 변해도 audio什帥le을 포함한다．


               Hierarchy descriptor

             계위적（hierarchy）으로 코딩된 비디오, 오디오 또는 priva把stream의 프로
           그램 요소정보를 서술한다．


           hierarchy_type : 4bits
             · 표 9-6과 같이 hierarchy tyl尤을 나타낸다．

           hierarchy_layer_index : 8bits
             · 코팅 꼐위에서 연관된 까四ram el印'ent의 index를 나타낸다（이 index
               는 하나의 프로그램에서 고유하다）.

           hierarchy_embeddedJayer_index : 6bits
             · 이    川erarchy descriptor에서 관계된 elemen啣y stream을 디코딩하기 전
               어］ 필요한 pro밈an比lement의 hierarchy table index를 나타낸다．
               만약 hierarchy ty光이 base layer이면 이 변수는 정의되지 않는다．
                                                                                                         9. 서술자


                                표 아6. }五erarchy t玎思 field valu田（MPEG Is: Table 2-45)

        V出ue                                Description




            0 l 2 3 4 5 6 뀨 巧
                                            reserved
                                            ITU-T Rec. H.262 ISO/IEC 13818-2 Spatial Scalability
                                            ITU-T Rec. H.262 ISO/IEC 13818-2 S寸R Scalability
                                            ITU-TR凹．H.拍기 ISO月EC 13818-2Te빠)oral Scalab小ty
                                            ITIJ-T Rec. H.262 I ISO/任iC 13818-2 Data partitioning
                                            ISO/IEC 13818-3 Ex把nsion bitstream
                                            ITU-TRec. H.222.0I ISO/IEC 13818-1 Piivate Stream
                                            reserved
                                            Base layer



hierarchy_channel : 6bits
  · 순서가 매겨진 몇 개의 채널 중 관련된 program el이l妃nt의 의도하고
       자 한 채널 번호를 나타낸다．
  · 가장 안정된 채널에 가장 낮은 채널 번호를 할당한다．


1Registration descriptor

 Registrali이ldesci如tor은 priva妃data를 혼동없이 정확하게 구별해 내기
위한 방법을 제시한다．


                                 표9-7. Registration de釵：riptor(MPEG IS: Table 2-46)


   Syntax                                                                       No. of bits   Mnemonic

   registration_descriptor() {
                  descnpto乙tag                                                           8    uimsbf
                  desedptor_leng由                                                        8    uimsbf
                  formatjdentifier                                                      32    uimsbf
                   for (i = 0; i <N; i++){
                                   additionaLidentificalion_info                         8    bslbf
                   }
   }
MPEG 비디오



           format identification : 32bits
             1 SC92 위원회로부터 얻는 등록번호

           additional identification info:
             1forma코entifier를 받는 사람에 의해서 정의되는데 한번 정해지면 절
               대 바꿀 수 없다．


           0Data stream alignment descriptor

             Data s毗am띠ignment descri少아는 관련된 elementaiy stream에 어떤 형태의
           정렬（alignment)이 존재하는가를 나타낸다. 만약 PBS packet header의
           data_.alignment_indicator = "1' ' 이고 뒤에 descriptor(）가 존재하면 이 data
           stream alignment desci如tor가 필요하다．


                          표． 아8. Data stiam alignn咽it c困뇌r肋r(MPEG Is: Table 2-47)


              Syntax                                                No. of bits   Mnemonic

              d趾乞誼tlne曲gn毗nt_desc印tor( ) {
                       desc印奴如g                                              8    uimsbf
                         descriptor_leng山                                    8    uimsbf
                         alignment_type                                      8    uimsbf
               }


           曲gnmen냐ype : 8bits
             ·PBS packet의 data_alignment_indicator = "1" 이면 표 9-9와 같이 정의
                   된다．
             ·video誼tarn인 경우에 PES_ 猛cket缸a_byte부분에의 첫번째 切'te부터
                   표 9-9에 기술된 부분이 들어가는데 예를 들어, vid的sequence의 처
                   음 부분이라면 sequence header의 첫번째 byte부터 정렬（align）되어서
                   들어간다．
             ·audio stream인 경우는 표 9-10과 같다．
                                                                                       9. 서술자


           표9-9. Video stream ali甲lment values(MPEG Is: Table 2-48)

                Al呻In妃nt ty比                            Description

                       00                        reserved
                       01                        Slice, or video access unit
                       02                        video ac此ss unit
                       03                        GOP, or SEQ
                       04                        SEQ
                      05-I下                      reserved



          표 9-10. Au如 stream alignment value小PEG Is: Table 2-49)

                시ignment 帥1e                           Description

                       00                              res心ved
                       01                              syncwoid
                      02-1下                            reserved



0Target background grid descriptor

 하나 이상의 video stream이 있고, 그 디코딩된 picture들이 그림 9-1과
같이 화면의 일부분씩을 차지할 때 각각의 pictu肥들의 위치를 target-
back凹.oun也帥d_descnptor와 너deo1wrn面w_descri마아어］ 의해서 정할 수 있
다． 이때 ta띵et_backg叩und召rid_descriptor는 화소단위 gnd의 恤get back-
giound의 크기를 결정하고 vid印mwindow코escriptor는 picture를 디스플레
이하고자 하는 창(win面叫의 O依et를 나타낸다．


                       A


                           vertical offset

     (                >y

         horizontal
         offset                video presented                     vertical size
                                    here




                                                                                   >
                              horizontal size                  V



  그림 9-1. Target background grid deacriptor display area(MPEG Is: Figure 2-8)
MPEG 비디오


                       표9-li. Target background grid deaHptor(MPEG Is: Table 2-50)


              Syntax                                               No. of bits        入nemonic

              target_background_giid_desciiptor() {

                                                                          8 8 4   4
                       descriptorjag                                                  uimsbf


                                                                              l l
                       descn까아그en肛h                                                   uimsbf
                       ho比ront심 size                                                  uimsbf

                                                                                1
                                                                                4
                       vertical 前ze                                                   uimsbf
                       aspect_rat幻Jnformation                                         uimsbf
              }

           horizental 前ze: l4bits
             · target backgr(沁nd grid의 수평축 크기
             · 단위는 화소

           vertical 前：ze : 14b沁
             · target back跡川nd grid의 수직축 크기
             · 단위는 화소

           aspect ratio_infonnalion : 4bits
             · target back留Dund grid의 asi比ct_ratio를 결정
             · 入4PEG2 비디오 파트의 asr玘ct1r曲o_information과 값이 갇다．


           1Video window descriptor

                             표
                               9-12. Wdeo window d困그虹巾才小IPEG Is: Table 2-51)


              Syntax                                               No. of bits        Mnemonic

              video_window_descriptor() {

                                                                          8 8 4 4
                      des（그i巾Dr1tag                                                   uimsbf
                       descnptor length                                               uimsbf


                                                                                 14
                       horizontal offset                                              uinisbf
                       vertical offset                                                uimsbf
                       windowpiiority                                                 uimsbf
              }
                                                              9. 서술자


horizontal offset: l4bits
  · picture를 디스플레이 하고자 하는 창佃indo刈의 왼쪽 윗 화소의 수
    평축 offset
  · 이 값이 0이 되면 picture가 target background의 맨왼쪽 가장자리에
    딱 붙게 된다．

vertical offset: l4bits
  · picture를 디스플레이 하고자 하는 창佃indow）의 왼쪽 위 화소의 수
    직축 offset
  · 이 값이 0이 되면 picture가 target background의 맨 윗쪽 가장자리에
    딱 붙게 된다．

window_priority : 4bits
  · 각 창들이 겹쳐지는 순위를 결정함．
  .0이 가장 밑에 있게 되고, 15가 가장 위쪽에 있게 됨（즉, 15를 갖
    는 창은 가려지지 않은 전체를 볼 수 있다）


0Conditional access descriptor

 조건부 수신（con毗onal access）관리를 위한 Bvll 이나 ECM정보를 표시
하기 위하여 사용되며, TS1爪恥rn_map_s凹如n과 program_stream_map어］
서 이용된다. 만약 어떤 elen妃nta口st妃am이 스크램블되면 CA descriptor가
반드시 존재해야 한다. 만약에 시스템 차원에서 전체적으로 스크램블을
하면 CA descriptor가 PSI 정보의 （刃nd地onal access table어］ 존재한다. CA
descriptor가 TS_program_map_section어］ 존재하면 CA_PU）는 EC入4과 갇은
정보를 갖고 있는 packet을 가리킨다. 이것이 프로그램 정보로 존재하면
모든 시스템에 적용되고 elementary stream정보로 존재하면 관계된
program ele毗nt어］ 적용된다. CA descriptor가 CA_section어］ 존재하면
CAH끼D는 Bll        과 같은 정보를 갖고 있는 恥炚et을 가리킨다．
MPEG 비디오


                            표    3
                                   Conditional ac：昑； d咀그iptor(MPEG Is: Table 2-52)


              Syntax                                                  No. of bits               八nem且lic

              CA_descriptor() (




                                                                                8 8 6 八4H n4U
                     des口jptorjag                                                               uimsbf
                     descriptor_length                                                          wmsbf
                                                                               l
                    C凡system_ID                                                                 uinisbf
                     reserved                                                                   bslbf
                                                                               l
                    CA PID                                                                      uimsbf
                     for ( i=0; kN; i- -+) {
                               private_data_byte                               8                uimsbf
                       }
              }


           CAH町stem_ID : 1日Lits
             · 관련된 可玉4이나 B＼小4의 조건부 수신 시스템의 타입을 말한다．
             · 각 사용자들이 알아서 정한다．

           CA-ND: l3bits
             · CA_s邪tern_ID어］ 의해서 지정된 조컨부 수신 시스템의 可丕4이나
                E\14정보를 포함하는 TS packet의 PID를 가리킨다．

            0
                Iso 639 language descriptor

           LSO 639 Janguage code : 24bits
             · 관련된 pri名ram element에서 사용된 언어의 종류를 나타낸다．


                           표9-14. ISO 639 language descriptor(MPEG Is: Table 2-53)


              Syntax                                                  No. of bits               入nemonic

              ISO_639Janguage_descriptor() {
                     descriptor_tag                                            8                uimsbf
                     descriptor_length                                         8                uimsbf
                     for (i=0;i<N;i-H-) {
                               lSO_639_langiiage_code                         24                bslbf
                               audio_ty思                                       8                bslbf
                       }
              }
                                                                        9. 서술자


  ·ISO 639 part2에서 규정된 3byte code를 이용．
  · N은 1보다 크거나 갇은데 예를 들어 multi_lingu出인 경우는 N은
      보다 크게 된다．

audio_type: 8bits
  · 표 9-15와 갇은 타입을 나타낸다．


                    표 9-15. Audio ty玘 values(MPEG Is: Table 2-54)

                       Value               Descriplion


                      m이m仍倣
                                           undefined

                      mmm야耳
                                           clean effects
                                           hearing impaired

                          倣
                                           visual impaired commentaly
                                           reserved



  1
      표에서 clean effects는 언급된 pm留an比lement가 언어를 포함하지 않
      는 경우이다．
  ·hearing impaired는 청각장애자를 위해서 마련된 pr孕am element라는
      것을 나타낸다．
  ·visual_imp孤red_commen啣y는 시각장애자를 위해서 마련된 program
      element라는 것을 나타낸다．


0System clock descriptor

 System cl(乂k에 대한 정보를 나타내기 위하여 쓰인다．

external dock reference in小cator
  · if(" 1") : system cl(乂k이 디코더에서의 ex把mal frequency ic把曲ce로부터
      얻어진다．

dock_accuracy_integer : 6bits
MPEG 비디오



           clock恥cura町_exj刃nent : 3bits
             ·sys把m clock이 3(汭끄TI보다 더 정확해야 하면 Cl(兀k의 정확도（accuracy)
               정보를 이 두 변수를 통해서 전송하는데 Cl(兀k의 정확도는 다음과
               갇이 계산된다．

                       clock_accuracy_integer X 10 - cl乂k_accuracy_exponent(ppm)

               만약 ck兀k_accuracy_integer = "0" 이면 sys妃m clock의 정확도는 30ppm
               으로 한다．


                            표 9-16. Sys也rn 吐)ck d咀：riptr才(mEG Is: Table 2-55)


              Syntax                                               No. of bits       人nemonic



                                                                                           忿啣
              system_clock_descriptor() {


                                                                             8 8 l
                                                                                                    r
                                                                                                    l
                      descriptor_tag
                                                                                                    r
                                                                                                    l
                      descriptor_length
                      external clock reference indicator
                                                                           l
                                                                           1
                                                                           1
                      reserved                                                       bslbf


                                                                                      U山 1山 比
                                                                             /0                 nt nt
                      clock_accuracy_integer
                                                                             八
                                                                             4U
                                                                                                 咽 咽
                      clock_accuracy_exponent
                                                                             <U
                                                                                                可
                      reserv出
              }


           1Multiplex buffer utilization descriptor

             이는 STD mt此히炚bu珏er의 정확도에 대한 한졔치를 제공해준다. 이는
           remultiplexer등을 위해서 제공된다．


           bound_valid_flag: ibit
             · if("l") : LTV끄必et lower1比m넜와 LilY！
                                                示et_upj光rb刃nd가 유효하다．

           LTW offset lower bo비ad: l5bits
             · 이 descn皿아에서 언급된 stream들의 모든 packet에 있는 LilY中O侄set
                  값들 중 최소값
                                                                                            9． 서술자


            표 9-17. 入4ultiplex buffer uti丘za血끄i de요그如tot-小'IPEG Is: Table 2-56)

   Syntax                                                     No. of bit.s       八nemonic

   m띠tiplex_bu什er_utiTh乙afion中desciiptor( ) {


                                                                         8 8 l
           descriptor_tag                                               8        uimsbf
           descriptor_len햅h                                             8        uimsbf
          bound_valid_flag                                              1        bslbf
          L꾀 offset lower bound                                        15        uimsbf
          reserved                                                      I        bslbf
          LTW-1offs炚_upper_bound                                       14        uimsbf
   }


  ·(27入4H71300) C1(兀k伏i-i（넜의 단위를 갖는다．
  · 이 값은 새로운 descriptor 전까지 유효하다．

LTW_offset_upper_bound: l5bits
  · 이 desci如tor에서 언급된 steam들의 모든 packet어］ 있는 LTIW_o丘set
       값들 중 최대값
  · (27MiHzJ300) ci（乂k꺄nod의 단위를 갖는다．
  · 이 값은 다음 descriptor 전까지 유효하다．


0Copyright descriptor

copyrightJdentifier: 32b1ts
  · SC292부터 얻은 copyright 등록번호


                    표． 9-18. ci叩yright d困그iptorUviPEG 15: Table 2-57)


   Syntax                                                      No. of bits       Mnemonic

   copynght_descriptor() {
          descriptor_tag                                                 8       uimsbf
          descriptor_len叩l                                               8       uimsbf
          copyright_identifier                                          32       uim없：)f
          for (i= 0;i< N; i-i-+){
                     additional_copyright_info                           8       bslbf
              }
       }
MPEG 비디오



           addition刻_copyright_info :8 bits
             · copyn帥t_ident出er를 받는 사람에 의해서 정해진다．
             · 한번 정하면 바꿀 수 없다．


           0Maximum bitrate descriptor

                               표
                                 아19. 入iadm山n bitra也 d因그如tor(MPEG Is: Table 2-58)

                 Syntax                                               No. of bits    八nemonic

                 maximum-bitrate_desciiptor() {
                          descriptorjag                                        8     uimsbf
                          descriptor_length                                    8     uimsbf
                          res心ved                                              2     bslbf
                          maximum_bi岫te                                       22     uimsbf
                 }

       m缸imum bitrate: 22bits

                 이 pmgmm 또는 prr增ml이印似吐들이 전송되는 최대 비트율化地如：
                 TS의 oven祀ad까지 포함）의 상한값을 나타낸다（pmgram에서 규정되
                 면 그 program에만 해당되고 program element에서 규정되면 그
                 pm얍am element에만 해당된다）.
                 50bytes/second의 단위로 게산
            1




                 I水if어］ 이 desci如tor가 삽입된다．
            1




       0Private data indicator descriptor

                          표． 9-20. Private data indic沮切rd咀ii的r(MPEG Is: Table 2-59)

            S刃ltax                                                   No. of bits    入nemonic

            private_datajndic止or_descniptor() {
                     descriptor_tag                                           8     uimsbf
                     descriptor length                                        8     uimsbf
                     private_data_indicator                                  32     uinisbf
             }
皿如a虹data如血汕야 : 3的ts
                                                                                        難難藝難難難驪蘿難
 . 개인에 의해서 자유롭게 이용될 수 있다．                                                               :::::::::::::::：弦：::::::::;::::：交蜘哺：::::;:;:;:;:;:;::：旨｝m든；:;:：芳：斑妊묘玉心1
                                                                                        小雛d蘆｛                                               器舜群群薄髓藤




1Smoothing buffer descriptor
                                                                                        月發好發芬三
                                                                                        巒難雛旨變．難聾巒轟轟瑟難薛至
                                                                                        難難藝難蠶難娜難
                                                                                        鱗爀難羅麟彗．難聽囊醬重

 이 smooti뇨ng bu什er descriptor는 sm(：刃師雎bu什er SBn의 크기에 대한 정보                              難蠱難難驪難
                                                                                        鑿難m冒
                                                                                        i梓礪牲烈疊注互妊擢舜七i難｛游i


를 서술한다. TS stream의 경우 1Sstream어］ 있는 해당 program element의
                                                                                        難鱗鱗磁雜難難多｝灘轟蠶轟饌聽巖璉發




                                                                                        多發珏m
                                                                                        疊驢滋難往撫咎注巍聾8君磁器磁르磁好無聽三羅專鞋滋程
TS packet들이 SBn의 입력이 된다（입력은 byte 단위이며 SBn의 크기는
sb_size이다）. PS stream의 경우 해당 이emen啣y stream의 P6 packet들이
SBn의 입력이 된다（입력은 byte 단위이며, SBn의 크기는 缸없ze이다）.                                            驪囊難難難難難驪臺
                                                                                           蘿難難難難難難難難難難麓發
                                                                                                   .::.：크포每携擴機弑牡熬：排；
                                                                                            :;::.：羅；               .:i：꿉難澣표疊훑i
 SBn bu什er에서 byte들을 추출하는 율은 sbJeak_rate이며 SBn은 절대                                                       珏字玉器蘿系珏露菱g旨毋
                                                                                                            ；藿iii;i;i；斑妾裝르鞋珽

overflow가 날 수 없다. 하나의 프로그램이 계속되는 한 그 프로그램의
각 program el帥妃nt들의 smoothing bu卄er descnptor어］ 있는 값들은 변할 수
없다. 또한 이 descriptor는 I呱if나 program s配am map에서만 정의된다．
心 stream의 경우 이 desci如tor가 I爪if의 ES정보에 있으면 그 program
element와 같은 P11）를 갖는 '1'S packet은 모두 SBn어］ 입력된다. TS stream
의 경우 이 descriptor가pro留an정보에 있으면 그 프로그램에 속해 있는
모든 elementaiy_PII）롤 갖는 모든 elementaiy stream과 이 섹션의 I爪if
PiT와 같은 PID를 갖는 모든 TS packet들은 SBn어］ 입력된다. 어느 시점
에서 각 progran比lement를 서술하는 descri恥아와 전체 program을 서술하
는 desci如tor는 한 7下1 이상 존재할 수 없다．


           표． 9-21. Smoothing buffer des그ipt才(MPEG Is: Table 2-60)


  S恥ltax                                              No. of bits            人nemonic




             客如 毗
                       的
                         () {




                                                               8 8 2 끄 2 끄
                                                                             uimsbf
                       h
                                                                             uimsbf




             蜘1畔客忿 毗
                                                                             bslbf
                                                                             uirnsbf
                                                                             bslbf
                                                                             uimsbf
  }
MPEG 비디오



           sb leak rate : 22bits
               · 해당 이ementa口 stream에 대한 SBn bu卄町에서 빠져나가는 비트율
                   （양수）
             · 400(bitslsecond) 단위로 계산

           sb size : 22bits
             · 해당 이ementa口stie出n어］ 대한 SBn buffer의 크기를 나타낸다（양수）.
             · ibyte 단위로 계산


           DSTD descriptor

            이 desci如tor는 T-STI) 모델에서 vid凹이ementary stream어］만 적용된다．


                                  표 아22. STD I뇨；心汭m(V下EG Is: Table 2-61)

               Syntax                                             No.0比沁       入Inemonic

               STD_descriptor() {
                        descriptor_tag                                     8   uimsbf
                        descriptor_length                                  8   uimsbf
                        reserved                                           7   bslbf
                        leak_v띠id_flag                                     1   bslbf
               }

       leal三느valid_flag : ibit
            ·if ("l") : T-STD 모델에서 leak방법이 쓰인다．
            1if("0") : vbv曲ay방법이 쓰인다（단, vid凹毗跏어꺼의 vbv曲ay값
             이 WI下（H）가 아니어야 한다）.

           1
               JBP descriptor

       dosed모咀flag : ibit
            · if(l) : 모든 I-frame 전에 （刃P header가 붙어 있으며, GOP header의
               closed名叩＝"1" 로 되어 있다．
                                                                                   9． 서술자


                      표 아23. IiBP de그.ip切r(MPEG Is: Table 2-62)


   Syntax                                                No. of bits     M妃monic

   ibp_desci기丈or( ) {

                                                                   8 8
            desci갸）tor小tag                                               uimsbf
            descriptor_length                                            uimsbf
            closed_gop_flag                                       1      uimsbf
            identical召叩_flag                                       1     uimsbf
            ma人g야니eng出                                            14     uimsbf
   }                                                                     bslbf



identical니gop_flag: ibit
  · if( 'l ") : 한 sequence 내에서 G아） 구조, 즉 (I-frame 사이의 p와 B-
       frame의 개수， picture coding ty［光 또 picture口m）이 모두 갇음을 의미
      （단, sequence 구조상 첫번째 G아） 구조는 틀릴 수 있다 : 入WEG 비
       디오 파트 참조）

n好乂.gop_len亭h : 14b沁
  · 한 sequence 내에서 연속된 2캐의 I-picture 사이에 있는 coded picture
       의 개수를 나타낸다．
  1
       0은 사용금지
MPEG 비디오




    卜                                                csps

           PS stream 중에서 변수（param毗r）들이 이 절에서의 규정을 만족시키면
           그 program stream올 CSPS(Cons岫inded Sys把mP毗neters Stream)라 한다．


           Packet Rate
            만약 cSpS에서 rat町聊nd값이 4,500,c［刃bits/second(packet_rate_mstriction_
           flag = "1" 인 경우） 또는 2,(刃0jy叩蛙四／sec刃nd(packet_ra把_restnction_flag =0인
           경우）보다 작거나 갇으면 cSPS에서의 packet rate는 300(packs/second）가
           된다. 그러나 rate 1刃und값이 위에서 언급한 값보다 큰 경우에는 다음과
           같이 정해진다．

            吐（packet_r汕et心出出Ml fi雎낟1')


                           N四tin阡t,(i))焰00／恤f九6

            寸（pad妃tl丑挽J心出出)n_flag = '0')

                           NP (tm                          ) X 300 x max[                   8

                                                                                      。x 1。
                                                                                          6
                                                                            1,        'm,
                                  (i   ')   -   t,   (i)
                                                                                 2.
                                                                                                ]
            여기서 尺mt= 8 x 50 x r口比boi甘idb畑／sec이며, NP는 서로 인접한 두 7가
           의 pack_start_code 사이 또는 마지막 pac如匕tart_code_pref奴와 system_
           header_s恤Ic奴妃들의 개수이다. 또한 뇨(1)는 I冬stream에서 p번째 p缸火의
           SCR에 있는 시간값（초）이고 뇨(i')는 MPEGJ加留mn_end_code의 마치막
           bit를 포함하는 by把가 P-STI）에 도착하는 시간을 나타낸다．


           Decoder B너脆r Si配
            cSPS에서는 Sm의 입력버퍼의 크기가 제한되는데 각 elementary
stream어］서 각기 다른 크기제한이 가해진다. 비디오의 경우 BSn은
vbv_bu什er_size-i-BSadd가 되는데 BSadd는 다음과 같은 조건을 만족한다．

                    BSm 5 MAX [6 x 1024, /(ma x 0.001] bytes

  여기서 R,_ 버퍼의 피크 비트율（peak bit ra妃）을 나타낸다．




卜                          참고 국제표준


1TU-T Rec. H.262 I ISO/IEC 13818-2:1994 Information technology - Coding of
moving pictuis and associated audio - Part 2: Vid凹.

ISO 8859-1:1987, Information pr兀essing- 8 bit single-byte coded graphic character
Sets - Part 1: 1月tin alph삯玘tNo. 1.

ISO/IEC 11172-1:1993 Information technology - Coding of moving pictures and
ass乂iated audio for digital storage media at up to about 1,5 M啣s - Part 1: Systems.

ISO/IEC 11172-2:1993 Information technology - Coding of moving pictures and
associated audio ford咆油1 st이age media 毗 up to 狐)Ut 1,外小姚 +art 2: Vid的．

ISO/IEC 11172-3:1993 Information technology - Coding of moving pictures and
ass乂iated audio for di曾tal storage media at up to about 1,5 Mbit/s - Part 3 Audio.

ISO/IEC I 3818-3:1994 Information technology - Generic co五ng of moving pictuis
and associated audio information- Part 3 Audio.

Recommendation 1TU-R BT601.3 Encoding parameters of digital television for
studios.

R凹ommendation 1TU-R BT470-2 Television systems.
MPEG 비디오


           Recommendation ITIJ-R BR648 Digital recor小ng of audio signals.

           Report 1TU-R BO.955.2 Satellite sound bmadcasting of vehicular, po八able, and fixed
           receivers in the range 500- 3000MHz.

           CCIYF Re刃mmendation J.17 Pre七mphasis used on Sound-Pmgramme Ciituits.

           I日EE St카ld可d 1180-1990 Stan由JdSr思c而cation 向r the Implementa加ns of 8 by 8
           Inverse Discrete Cosine Transform.

           IEC Publication 908:1987, CD Digital Audio System.

           ISO/CD 13522-1;1993 Information technology - Coded representation of multimedia
           and hypermedia information objects - Part 1:Base notation..

           ISO/CD 639-2; 1991, Terminology - Codes for presentation of names of languages
           Part 2: Alpha-3 code




    卜                     TS스트」의decoding예
             七Sc> go
             In七elmJ1尤： PID OxO de七ec七ed.



             tsc> （玉口np

             sync_h七e = 0x47
             transr刃rt乙error_indica七or = 0

             payload_unit_s tart_ indicator = 1

             transport_priority     = 0
             PID ：二 小＜0

             transport_scrambling_control = 0
             adap七a七ion나field_contr아 = 1
continuity_counter = 0
 47 40 00 10
00 00 b0 15 00 7b ci 00 00 00 00 e0 37 00 01 e0 4d 00 02 e0 4d 97 c9
04 37 ff ft ff ff ff ft ff if        ff ff ft ft ff ff ft ff ff ff ff ff ff
 ff ifff ff ff ff ff ft if if ff ff ft if ft ft ft if ff ft ff ft ff
ft ft ft ft ff ft ff ff ff ff ft ft ff ff ff ff ft ff ft ft ft ft ff
ff ff ff if if ft ft if ff ff ft ft ff ff ff if ff ft ft ff ft ff ft
ft if    ff ft if if   ff ft if   ff ff ff ff ff ft ff ff ff ft ff ft ft ff
if if ff ft ff ff ft if ft ff ft ff ft ff ff ft ft ff ff ff ff ft ft
ft ft ft ft ft ft ft ft ft ff ft ff ft ff ft ff ff ft ff ft ft ft ft


tsc> pa七
Proc工ram Assc兀ia七如nT出丑e


table id = 小＜O
section_syntax_indicator = 1
'   0r
res凹Ne크 = 3
sec七ion뇨length == 21
transport_strean_id = 0x7b
reserved = 3
version num氾r = 0
口J工rent n曲＜七 1工idica七（>r == 1
sec七ion_nu姓冶r = 0
is引： sec七ion numi氾r = 0


pr四：
   rani_nu姓氾r = 0
netnDrkP끄） = 仍＜37


   ram x끼址氾r = 1
pr四：
pr四ram_n텍乙PID = 0x4d


prograx屯ni工沚氾r = 2
program_n텍乙PIn = 0x4d


cf之C 32 = 仍＜97c90437
MPEG 비디오


                tsc> ca七ch 仍＜37 interru此

                Add 呵 an臼' PID fil七er.


                tsc> ca亡ch 呱4d inte工mJ1比

                Addil珂 an日VPID fil七er.


                七Sc> cc江it
                끄止emn四七： PID 0x4d de亡ec七ed.


                tsc> durip
                sync_byte = 0x47
                tman匐？O此_error_indica七or = 0

           payload_unit_start_indicator = 1
            transport_priority     = 0
           PID = 0x4d
            tran同9吐L多cral做江ir啞mcon七mc江 = 0
           ada尤ation_field_con匕幻1 = 1

           continuity_counter = 0
           47 40 4d 10
           00 02 bO id 00 01 ci 00 01 e0 38 f0 00 02 e0 38 f0 03 02 01 01 04 e0
           39 f0 03 03 01 02 7b e4 31 42 ff ff ff ff ft ff ft ft ff ff ff   ff ff
           ff ft ff ff ff ft ft ff ft ff ff ff ft ft ft ff ft ff ft ft ft ff   ff
           ff ft ft ft ff ff ft ft ft tf ft ff ff ff ft ff ft tf ff ff ft   ft ff
           ft ff ft ft ff ft ft ft ff ff ft ff ff ft ff ff ff ff ft ft ff ff ft
           ff ff ft tf ff ft tf tf ft ff ft ff ff ft ff ff ff tf ff ft ff ff ff
           ff ff ft ff ff ff ff ff ft ft ff ff ff ff ff ff ff ff ff ff ff ft   ft
           ff ff ff ff tf ft ft ff ft ft ff ft ft ff ff ff ff ff ff ff ff ff ff


           七sc> sn七
           功：乙gram l工珏） Table


           table id = 0x2
           section_syntax_indicator = 1
           '0
                 '

                             U
           res回：ved
sec七ion나length = 29

        工mt油r = Oxl
pr（珂rain；
rese工＼尼d = 3

vers i （그n fli.nhi戶r = 0

current_nex七_indicator = 1

sec亡i（工lnurni氾r = 0

last sec亡ion nun幻er = 1



res凹：
    ＼尼d == 7

PcR PID = 0x38

reserved = 15

program_it迂o 1回自냔l = 0



stream뇨t）四e := 小＜2

(IIU-T Rec. H. 2621190/ m    13818-2 Video
 or I羽/ 1或 11172口 （兀ns七rained parar陀ter vide（그 stream)

rese工＼
     ／日크 = 7

e1arntary_P표） = 仍＜38

rese工＼尼d = 15

ES_inf（그니length = 3



         descri1尤O乙tag = 2
          (video_stream_descriptor)

         descrir比or_leng냔l = 1

         multiple_frame_rate_fl ag = 0
         frame_rate_code = 0

         l41月3_i_ only_flag = 0

         constrained_ 月rameter_flag = 0
         still_ picture_flag = 1



stream_type = 0x4
(I&그／IB2 13818日 1뇨idi이

rese工＼
     ／日크 == 7

elenentar）
         乙PID = 仍凸9

res凹：ved = 15
MPEG 비디오


                               mtU
      =
           ES_info_leng上


                   descriptor_tag = 3
                   (audi（乙St工e帥니descrip亡吐）

                   descri1尤or_leng나l = 1
                   free如nrat：
                            寸flag = 0
                   끄） = 0
                   layer = 0
                   vriable_ rateaudioJndicator = 0
                   reserved = 2


           CRC 32 = 小＜71氾43142


           tsc> vcatch 0x38 interru尤 af
           Adding a video P끄) filter.


           七sc> aca七ch 缸39 inte工mJ1尤 pusi
           Adding an audio PID filter.


           七sc> con七
           Th七ern1比： PID 缸4d de七ected.


           tsc> durrp

           Syfl(乙byte = 小＜47
           trar目刃rt＝町ror_indica七or == 0

           payload_unit_start_indicator = 1
           trans均rt_priority = 0
           P1]
            ) = 0x4d
           tran司9江L多cra［趾）1뇨ig_control = 0
           adaptation_field_con口ol = 1
           continuityj兀ur止er = 1
           47 40 4d 11
           00 02 hO ld 00 02 cl 01 01 e0 3a f0 00 02 e0 3a f0 03 02 01 01 04 e0
           3b f0 03 03 01 02 de le b7 a6 ff ft ft ff ft ff ff ff ft ff ff ff ft
           ff ff ff ff ff ff ft ft ft ff ft ff ft ff ff ff ff ff ff ff ff ff tf
           ff ff ff ft ff ff ff ft ft ff ft ft ft ff ff ft ft ft ff ft ff ff ff
ff        ff          ff ff ff      ff ff ff ff ff if    ff ff ff ff ff ff ff ff ff ff if         ff
ff if                 if    ff if   ff ff if    ff ff ff ff if   ff if   ff ff ff ff ff ff if     ff
ff if                 if    ff   ff ff ff ff ff ff ff ff if      ff if   if   ff ff ff ff ff if   ff
ff        ff ff ff               ff ff ff ff if    ff ff ff ff ff ff ff ff ff ff ff ff ff ff


tsc> pitt
p끄均ram卜ap Table


table id = uxZ
sec亡끄工-"-S恥北a)＜니끄X虹ca亡or = I
          .   .   U                 .   .   .




'0    '



reserved = .3
section日1包m그l = 29
pr四ram_nt끄m氾r = 0x2
reserved = .3
version._jiutU：尼r = U
口江-r臼it_next_iridica七（>r = 1
sectionniln氾r = I
last sec亡ion nt工m氾r := I


res凹：ved = 7
PcR_PID = 小＜3a
reserved = 15
pr四rant士迂o_len야h = 0


str田m_ty兀 = 0x2
(I四-T Rec. H.262IIS3/LC 13818-2 Video
     or ISD/ IEX 11172-2 cons七rained paraxeter video stream)
res回：ved = 7
elqrenta工l二p끄） = 仍＜3a
rese工ved = 15
ES_info_le야h = 3


                           descriptor_tag = 2
                           (video_stream_descriptor)
MPEG 비디오


                  descriptor_length = 1
                  nultiple_ franE_rate_f lag = 0
                  fraire rate code :: 0

                  MP且乞1아ily_f lag = 0
                  cons匕aine&paraceter_f lag = 0
                  still_ picture_f lag = 1


           strean냐：y1氾 = 0沁
           (ISO/IC 13818日 j udio)
           reserved = 7

           elerentary_P끄：) = 0x3b
           rese工＼尼d = 15
           ES ii迂O 1包lgth = 3



                  descriptor_tag = 3
                   (audio_stream_descriptor)
                  descriptor_length = 1
                  free뇨f(＞工T[atHflag = 0
                  ID = 0

                  layer = 0
                  variable rate audio indicator =
                  reser＼厄d = 2


           cRC 32 = 0xde1eb7a6


           七sc> con七
           끄北ern1尤： PID 仍＜id就e（北ed.


           tsc> d工1p
           sync_i乃7七e = 炚47
           trans1刃r七1e그or_indica七or = 0
           payload_unit_start_indicator = 1
           transport_priority = 0
           1？끄） = 小d

           七ransport多cran幻ling_control = 0
adaptation_field_control = 1
continui勻二Cou砒er = 0
47 40 01 10
00 01 bO if                ff ff ci 00 00 09 14 00 05 e0 50 43 41 5f 44 45 53 43 52
5f505249 56415445d04e0f5bfffffffffftfffffffffff
ff ff ff ff ff ff ff ff ff tf ff ff ff ff ff ff if                  ff ff ff if   tf ft
ff ff if              ft ff ft ff ft ff ft ff ft ff ff ff ft ft ft ff if     ff ft ff
tf tf if              ft ft ft ff ff ft ft if   ft if   ft ft tf ff ff ff ft ff ft ff
ft ft ft ff ff ft ft ff ff ft ft ff ff ff ft ft ft ft ft ff ft ft ft
tf ff ff ft ft ft ff ff ff ff ff if                ft ft ff ft ff ff ff ff ft ft ft
ff ff ft ft tf ff ft ft ft ft ft ft ff ff ft ff ft ft ft ft ff tf ff


七SC> Ca七
Conditional Access Table


table Id = Oxi
             U                .       .




section_syntax_mctica口＞r = I
    '0   '



resexvect = j
sec亡ion日上engtfl = i-I.
res臼：
    ＼尼d = 0xffff
reserved = 3
version_nu咐光r = U
Cu工rentnextindica七（Dr = 1
section ni.nter = U
las亡 sec亡ion ni고趾冶r = U
.                1     .          .




                     descriptor_tag = 9
                     (CA나descriF尤or)
                     descriptor_length = 20
                     CA_sy就q七ID = 缸5
                     res臼：
                         ＼尼d = 7
                     CA口p표） = 0x50
                     private_data_by七e =
                             43 41 5f 44 45 53 43 52 5f 50 52 49 56 41 54 45
MPEG 비디오



           CRC 32 = 0xd04e0f5b


            tsc> Ca七ch 0x50 inte工工lJr比
           Mding a nei' PID filter.


           tsc> con七
           Interni比： I江D 劤＜37 de七ected.


           亡SC> （如旺）
           sync_byte = 0x47
           transport_ 工ror_rnthcator = 0
           payload뇨uni七日日S七art_rnthca亡or = 1

           txan駐力rt_priority = 0
           PID = 0x37
           t工帥啄肋上多Crarnbllng_.口丑止rol = 0
           adaptation_field_control = 1
           C（丑比lrlUlty_C(壯l七er = 0
           47 40 37 10
           00 28 f0 lb 00 00 Cl 00 00 4e 45 54 57 4f 52 4b 5f 49 4e 46 4f 5f 54
           41 42 4c 45 52 15 dd 6c ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
           ff ff ff ff ff ff ff ff    ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
           ff ff ff ff ff ff ff ff    ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
           ff ff ff ff ff ff ff ff    ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
           ff ff ff ff ff ff ff ff    ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
           ff ff ff ff ff ff ff ff    ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
           ff ff ff ff ff ff ff ff    ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff


           七SC> p工＼/
           Priva七e SeC七ion


           table id = 0x28
           sec七ion니syntaxindica七or == 1
           priva七e뇨andica七or = 1
           resen／
                日크 = 3
                                                                           부 록

se（北如n나len哄h = 27
tab1e_id_e;<tension = 0x0
reserved = 3
version_nurr螂 = 0
Cu工ren七J）包t indicator = 1
sec七ion nm光r = 0

last_section_nunb町 = 0
pri＼厄七e니datam妨亢e =
         4e 45 54 57 4f 52 4b 5f 49 4e 46 4f Sf 54 41 42 4c 45


七SC> C아l七

In七e工그nJP七： E江D 缸50 detected.


tsc> （虹11)
$yllCJ刀七e = 0x47
transpor七_error_indicator = 0
payload누unit多七a此1indic配or = 1

t工an斗均此pr如rity = 0
PID = 小凸0

transport_scrambling_control = 0
ada尤a七ion日fiel口cont그그＞1 = 1

（兀n七inuit二counter = 0
47 40 50 10
00 29 f0 10 00 00 ci 00 00 43 41 Sf 49 4e 46 4f 06 05 ab 18 ff ff ff
ff ff   ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
ff ff   ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
ff   ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
ff   ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
ff ff   ff ff   ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
ff ff   ff ff   ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
ff ff   ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff


tsc> pry
Priva七e Sec亡jJ丑l


t：祉江e id = 缸29
            MPEG 비디오


                                section_synt그_indicator = 1
                                private_indicator = 3.
                                res回：
                                    ＼尼d = 3
                                sec七ion구er呵나l = 16
                                table idextension = O山
                                rese工＼尼d = 3
                                versi（丑1 flU!!止氾r = 0
                                cu工rent flex七_indica匕＞r = 1
                                sec七i（丑-i nutt止羌r = 0
                                las七 sec七ion nuid氾r = 0

                                private_data_ 乃／te =
:i;；藿．
     i:．童                               43 41 5f 49 4e 46 4f


發發m多
麟藎珽器轟薑｝



弓裝發裝鞋鞋鞋轟；i；滋難瀟；激i
工1JJ7三口m乙乙口1=＝口Jr万口且口二L느느UddJ
                                七sc> con七
                                In七ertlJ1北： PID 0x39 de七ec仁ed (r月yload_unit_s tar七Hindica七or) .


                                七sc> 凸Jni)
                                sync_byte = 0x47
                                transport_error_indicator = 0
                                payload_unit_start_indicator = 1
                                transport_priority = 0
                                p끄：) = 0x39

                                transi兀rt多cran幻lirig_的nt工O1 = 0
                                adaptation_field_control = 1
                                C（丑l七inuity늑coun七er = 0
                                47 40 39 10
                                00 00 01 c0 01 6a 80 80 05 21 00 05 22 el ff fc b4 04 0c 98 77 55 55
                                77 66 65 55 45 45 23 23 48 a4 89 24 90 00 00 00 00 00 00 c0 00 00 08
                                0a088aaeab1ea9c67496ec62ab29f1c64b30a7                     1be6b7 1a
                                f1be9c71b3      2c2cc3 2bb3d2bc6fc2dc          f4bb6d2dcb0bf4c3
                                3d 2f （땄） lc af d3 lc af ca 且） fO 上毛 ec ef 1兀 fd 3d fd 7d 3c fc 9a 21
                                862822 8d 85 9b 75 e7 db 6165 d9 8b 5485 cd4c 6b24 bl b6 3237
                                ced0ebd2dc36ddcb64284d98d1cc5a0539db9abc7a98                      7a
                                95c1b4 f5 日：) 끄：)a7c6 9b2e372c2d3f         25 71eea3 5a09 51b71고：)
                                                  부 록


PES H口켸平才




packet_start_co크e_pref ix = 000001
stream id = OxcO
PES_r묘炚就_1eng나l = 362

'10 '
P邱1scran幻uin丑con口ol = 0

PES_priority   = 0
data누alignrt日北 inc虹cator == 0

copyright = 0
original_or_copy = 0
r'TS_prS_f lags = 2
ESCR_f lag = 0
ES_rate_flag = 0
1X到trick_p넜e_f lag = 0
additional_copy_info_flag = 0
P邱小（系C_flag = 0
PES e>＜七amsion나flag = 0
PES_header_data_length = 5


'0010 '
PrS[32. .30] = OxO
cc日工ker bi七 = 1
PTS[29. .15] = 0x0002
cc日rkei二上it = 1
PrS[14. .0] = 0x11f0
cc日rkerj竝七 = 1
tsc> con七
끄止ern 尤： P끄） 小＜38 detec七ed (ad크pta七ion_field) .


tsc> di.ucp
sync_byte = 0x47
transport_error_indicator = 0
paylc沮    uni七1stan尤 ir五ca匕＞r = 1
MPEG 비디오


            transport trioritv   = 0
            PID = 小＜38

            trar)sDort scrarnblmo control = U
            aciac亡atlon rielci control = 3
           C（丑止iriuitv cowl七er = 0
            47 40 38 30

           0790000002 e8 7f20 00000le00f               fe80c00a31     0005 3f01 11
           00 05 22 el 00 00 01 b3 2c 02 40 83 04 e2 22 a9 10 11 ii     12 12 12 13
           13 13 13 14 14 14 14 14 15 15 15 15 15 15 16 16 16 16 16 16 16 17 17
           17 17 17 17 17 17 18 18 18 19 18 18 18 19 la la la la 19 lb lb lb lb
           lb ic ic ic ic le le le if    if   21 00 00 01 b5 14 82 00 01 00 00 00 00
           01 b8 00 08 00 c0 00 00 01 00 00 0f ad d8 00 00 01 b5 8f ff f3 88 00
           00 00 01 01 52 cd fi 3d 2b 28 45 21 37 d2 a9 lc 4f e7 27 62 73 9e 9f
           b7 6el크fld3       8e 60 76 4aa6 6e ca 5a 25 玉二 Oc 6f 9ae9 32 8437d6


           tsc> af
           AdaP七a七ion Field


           adaptation_field_leng나l = 7


           discontinuity_indicator = 1
           randn_access indicator = 0

           elannta工l二strea旺priori四indica七or = 0
           FR_f lag = 1
           o1X그之_f lag = 0

           splicing_point_flag = 0
           transport_private_data_f lag = 0
           a（姐就a七ion_field卞畔比nsion뇨flag = 0


           program_clock_reference_ 月se = 0x0000005d0
           res臼：V日l = 63

           program니clock_reference寸라七ens如n = 0x120


           tsc> pea
           PES Header
packe七HS七a'七－工ode＝皿ef ix = 000001
streanLid = 0xeO
PES_packet卞length = 4094
'10 '
PES_scra幻ling_con口ol = 0
PES工riority = 0
data_alignrrerit_indicator = 0
copyright = 0
original_or_co乃／ = 0
PrS_1yrS_f lags = 3
E요玉_f lag = 0
ES工a七e_f lag = 0
DSM口ick_irK珏乙flag = 0

add뇨切na느copy_u出乙flag = 0
PES니（묘：
      乙flag = 0
PES_e＞比ension日flag = 0
PES_header_data_length = 10


'0011'
PTS[ 32. .301 = OxO
markerbit = 1
PTS[ 29. .151 = 0x0002

marker bit = 1
vrS[14. .01 = 0x1f80
O日rker bi七 = 1
'。   。。1   'e




DI'S[ 32. .30] = OxO
marker bit = 1
ty끄S[ 29 . . 15) == 炚0002
rr日그가'er hi七 = 1
tYrS (14. .0] = 0x11f0

markerbit       = 1


七sc> cont
Inter乙四匕： PID 0x38 de七e（北ed (adap七a七ion나field) .
MPEG 비디오


           tsc> （玉m1)
           sync_byte = 0x47
           transport_error_indicator = 0
           payloa也unit多tart_indicatc江 = 0
           transp才t_priority = 0
           p끄） = 0x38
           tran啄刃比_scranbling_co毗如1 = 0
                                 rol = 3
           adapta七jar]나field나cor比：
           continuit크乙（兀Un七er = 6
           47 00 38 36
           7b 00 ft ft ff ff ff ff ff ft ff ft ft ff ft ft ft ft ft ff ft ff ff
           ft ft ff ff ff ft ff ft ft ft ft ff ff ff ft ff ft ft ft tf ff ft ff
           ff ff ff ff ff ff ft ff ft ft ff ff ft ft ft ff ff ff ff ft ff ft ft
           ff ff ft ft ft tf ff ff tf ft ft ft tf ft ft ff tf ff ff ff ff ff ff
           ff ff ff ft ft ff ff ff ff ff ff ff ft ft ft ff ft tf ft ff ff ft ft
           ff ff ft ff tf ft tf tf ft d9 96 1d4b 8b Ob la 1159 it   4028 由 0e
           c2 e7 8b 68 72 d7 6d 54 ae f2 2b 4e b3 7d 63 68 ad 2d 54 f3 29 39 8b
           4a b2 cO c5 25 b6 34 33 39 a7 dd c8 58 f6 t4 99 a7 e5 18 36 06 86 84


           tsc> at
           ?daptation Field


           adaptation_field_l色gth = 123


           （虹scon七inuit乙indica七or = (:)
           randQn_acce3si.ndicator = 0
           elai日lta工l二就ream山nioni勻뇨indicator = 0
           R:R_fl ag = 0
           01X:R_t1ag = 0
           印licinq point_flag = 0
           tra啄ort_private_data_flag = 0
           adaptation_field_extensio뇨flag = 0


           s七1lff_byte = 0xff * 122
                                                                         브   로




tsc> con七

Interrupt: PD) 0x39 detected (payload_unit_start_indicator) .


tsc> durrp
sync_byte = 0x47
transport_error_indicator = 0

payload_ 끄lit_start_indicator = 1
transport_priority   = 0
l？끄） = 0x39
trans恥以＝scra耐江ir啞下ont工C江 = 0
a아크恥：a七ion뇨fieid_cont工ol = 1
continuity_counter = 2
47 40 39 12
00 00 01 c0 01 6a 80 80 05 21 00 05 33 ci 5e e8 3e Of 67 66 77 78 64
4a 19 db 47 87 4d 24 40 d2 4a f8 29 52 be b3 56 e6 b6 06 12 01 fe 12
02 06a2 81b89f89f82181f7            9b7e076106b9ed8c1cd0aecc
ac e9 lb c3 2d 8e bO f9 b6 cd 27 id 52 Gb be 7b 75 2d ae 8d 23 08 弱
4a f8 30 be 42 47 0f dd dc 14 73 03 3e b9 07 2d 3b dl 4f a9 4e a3 b9
47 64 2a 13 le 66 82 81 21 de 2e 82 0c 23 54 b3 9b 39 Gb ab 14 al 40
bO b3 f3 83 7f 59 a3 95 e5 f5 be b9 7a if   5b a3 96 5d f2 99 c5 l月 af
6c d4 66 57 52 b7 91 2c 61 5a b3 a6 92 86 4b e5 ef 5c a6 13 58 04 b4


七sc> pes
PES Header


                prefix
packet_start_co크e_         = 000001
streanid = OxcO
PES_
  packet_iqlgth = 362
'10 '
P邱＝
  －多cran幻lrng_c(丑itrol = 0
PES_priority   = 0
dat&_aiignxnt_in五cator = 0

copyright = 0
original_or_c四y = 0
PIg그끄＄jlags = 2
MPEG 비디오


           표艾R_f lag = 0

           匹乙ra七已flag = 0
           DSM_七rick_rctxie_f lag = 0
           add!匕ional_的仍二info_flag        0
           p邱1C1之C_fl ag = 0
           PES_extension_fl ag = 0

           1표乞header_da七乏len守th = 5


           '0010 '
           PTS[ 32. .30] = OxO
           marker bit = 1
           PTS[ 29. .15] = 0x0002
           marker bit = 1
           PTS[14. .0) = 小＜巧e0
           marker bit = 1


           tsc> con七
           Inte工工-UI尤： P끄） 缸39 de七e（北ed (payload_unit_star七_indicator) .


           tsc> durip
           sync_ 乃／te = 0x47
           transport_error_indicator = 0

           payload_unit小就a工七 inc五catc江 = 1
           transl均此_pri（그rity = 0
           PID = 0x39

           匕rans1均rt_scra끄的ling_c丑itrol = 0
           adaptation_field_control = 1
           continuity_counter = 4
           47 40 39 14
           00 00 01 c0 01 6a 80 00 00 c6 91 61 2c 6d 47 0b 52 ca d5 2d 53 5c 15
           c7 05 75 b9 7c 70 5f lb 94 bf 25 71 b5 끄D d2d2 f4 f2 b5 2d 33 4f 2c
           53 갔D1530b9 4ced67 3b99ca b6 b3 a9 9c ec 6a fa db d2 a6 b0 a9
           Sd 2a 73 3b 9b ca e7 0e 38 el 11 4e 68 f0 b7 57 9c 32 ed Se 7b le b4
           9c f9 a2 5c 32 eb 3b 18 el 4d 52 b5 al 16 c6 ed 끄＞ ed 7c 49 fl   94 50
           b5 al 17 50 ed 02 18 36 47 le 78 88 b7 d2 e8 lb 14 11 d8 76 3e 48 54
                                                                       부 록


62 92 b2 b8 4a 97 ce 73 ba 7d c2 bc 29 66 8c ca 44 a0 54 12 99 15 a5

e0 48 bO a4 2e a9 db 7a d4 a3 d0 3844 ada6 if   49 c5 88 b6 0b ea d2




PES Header



packe七HS七art_c（月e工ref ix = 000001

stream id = OxcO

PES냐月cket_iength = 362

'10 '
PES_scrai祉且in互con比C江 = 0

p표｛工non勻／ = 0

data_aiignn nt_indicator = 0

copyright = 0

original_ or_copy = 0

PrS_t1TS_f lags = 0

E요工니flag = 0

ES_rate_flag = 0

DSM_trick_ n月e_f lag = 0

addi亡:1-（丑）al11c（그1乃／Hinf o_f lag = 0

PES_cRc_f lag = 0

p묘乞라t曲sion뇨flag = 0

PES_header_data_iength = 0



tsc> cont

II止巴m4比： PID 缸38 de七e（北ed (ada尤a七ion_field) .



tsc> duirp

sync_byte = 0x47
transport_error_indicator = 0

payload_unit多tar七1n(五ca七or = 0

亡ransp<그r七니priority = 0
p끄） = 小＜38

transport_scrambling_control = 0

a（士ptat如ri_field나cont工아 = 3
MPEG 비디오


           continui亡y-(兀U砒er = 13
           47 00 38 3d
           83 00 ft ff ff ff ft ff ft ft ff if     ff if   ff ff ft ff ff ff ff ff ff
           ff ff ff ff ft ff if   ff ff ft ff ff ft ft if     ff ff ff ff ff ff ff ft
           ff ff ff ft ft ft ft ff ff ft ft ff ft ft ff ff ft ft ff ff ff if       ff
           ff if   ft ft ft ff ft ff ft ft if   ft ff ft ft if   ff ff ft ft ff ft ff
           ff ff ft ft if   ff ft ff ft ft ft ff ff ff ff ft ff ff ft ff ff ft ft
           ff ft ft ff ff ff ff ff ff ff ft ft ft ff ft ft ff ac e6 d8 96 15 67
           8c ad fO a3 8a 8d f4 80 07 ft 6b d3 ef 7d 62 ba 93 72 42 65 if       24 85
           6568 7c lb lbaf     e9 dc 4f 2a 30 e2 43 52 7b 54 8f c8 c9 c6 51 b6 62


           七sc> af
           Adaptation Field


           adar比a七ion_f ield_lengt士l = 131


           discontinuity_indicator = 0
           randcin access indicator = 0
           eiateitar二streai工nioni勻二ir五ca仁or = 0
           1X그L.flag = 0
           o1X그之누flag = 0
           splicing_point_flag = 0
           transt兀rt_pr如毗e da七乏flag = 0
           a姐ptation_field_e乂tension니flag = 0


           stuff_切te = 小＜ft 女 130


           七sc> con七
           Interru就： 1江r) 小＜4d de七e（北的‘


           tsc> durrp
           sync_byte = 0x47
           trans均rt_error_indicator = 0
           payload_unit_start_indicator = 1
           trar囹刃此Jr如rity = 0
PIn = 0x4d
trans刃比尸scra岫un王con比（Dl = 0
ada尤a七ion_f iel之con比（Dl = 1
con七1工luity_courl七er = 2
47 40 4d 12
00 02 bO id 00 01 ci 00 01 e0 38 f0 00 02 e0 38 f0 03 02 01 01 04 e0
39 f0 03 03 01 02 7b e4 31 42 ff ff ff ff ff ff ff ff ff ff ff ff ff
ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
ff       ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
ff ff       ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
ff       ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff


tsc> 1xn七
Program 姓｝p Table


亡able id := 小＜2

sec七1아-l나syntax나indicator = 1
'0   '



res回：V日크 = 3
section_length = 29
prograx띠flu耐冶r = 仍ci
reserved = 3
versic江i nui祉毛r := 0
（二끄그：entnext_ indicator = 1

sec七ionnum氾r = 0
last_sec七ion_nu址氾r = 1


reserved = 7
P::R P끄） = 仍＜38
rese工＼厄d = 15

program_info_length = 0


stream_ty氾 = 0x2
MPEG 비디오


           (I叭J-T Rec. H. 2621193/IEC 13818-2 Video

            or ISO/ I且그 11172口 const그：ained paran 七er video str吐Sn)

           reserved = 7

           elanentary_PID = 0x38

           rese工＼尼d = 15

           표乞info_le四냔l = 3



                   descriptor_tag = 2

                   忖ideoj七resin니descri1尤or)

                  descriptor_length = 1

                  rmiltiple_fra毗뇨ra匕e_f lag = 0

                   franre rate code := 0

                  52n11夕ni止flag = 0

                  coils七rained_pa工ar陀亡臼乙flag ＝二 0

                   still_ picture_flag = 1



           stream냐M冶 = 0沁

           (IS가m 13818-3 Audio)

           rese工＼厄d = 7

           elanres止ary_P표） = 0x39

           rese工＼尼d = 15

           ES_inf（그11巴lgth = 3



                   descriptor_tag = 3
                   (audio_s亡ream_descriptor)

                   descri1尤or_le四냔1 = 1
                   free此工T[a七Hfl的 = 0

                   ID = 0

                   layer = 0

                   v工iable rate audio indicator = 0

                   rose工＼厄d = 2



           C묘C 32 := 0x7L冶43142

           七Sc> cc江I七

           In七e工工U1尤： PID 0x4d de七ec七ed.
                                                                                       부 록

七Sc> d工4)
syncj：乃／七e = 小＜47
transport_error_indicator = 0
payload_un1t多tart_indica七C江 = 1
transpor亡_pr如rity = 0
PID = 小4d
transport_scranbling_control = 0
adaptation_field_control = 1
continuity_coux止er = 3
47 40 4d 13
0002b0 1d0002c10101e03af00002e03af0                                03 02 010104e0
3b f0 03 03 01 02 de le b7 a6 ff if               ff if   ft ff ff ff ff ff ft ff ff
tf       ff   ft ff if     ff ff ft ft ff ff ff if   ft ff ff ft ft ft ff ff ft ff
ft       ff   ft ft ff     ft ff ft ft ft ft ft ft tf ff ft tf ff ft ft ft ft ft
ff tf         ft ft ft ft       ff ft ff ff tf ff ff ft ff ff ff ff ff ff ff tf ff
ft       ft ft ft       ft ff   ff ft ff ff ft ft ff ft ft ft ff ff ft ff ff ff ff
ff       ff ff   ft ff     ff ff tf ft ff ft ff ft tf ff tf ff ff ft ff ft ft ff
ft       ff ft   ff ft     ft ff ff ft ff ft ft ff ft ft ft ff ft ff ft ft ft ff


tsc> rn七
Program 旺珏） Table


七able id = 缸2

section_syntax_indicator = 1
'0   '



res回：
    ＼旭d = 3
section_length = 29
program_nurn冶r = 小＜2
res凹자ed := 3
＼戶凹:si丑1 nu姓兀 r = 0
current_next_indicator = 1
section number = 1
last_section_num氾r = 1


     田
     r              n
                    /
MPEG 비디오


           1X: R_PID = 0x3a

           rese工＼
                ／日크 = 15
                                       0
           pr四rami址o_length
           =



                 小




           strea皿t孤冶 = 小＜2

           (끄u-T Rec. H.26211SO/IEC 13818-2 Video

               or ISO/ I   11172-2 cons口：
                                        ained paraxeter video stream)
           rese工＼尼d = 7

           elanenta工l二PID = 出凸a

           rese工＼厄d = 15

           邱LJnfo_1eng匕h = 3



                      descriptor_tag = 2

                       忖ideoj口田m_descri1尤or)

                      descriptor_length = 1

                      riultiple_ frarre_rate_f lag = 0

                      frarre rate code = 0

                      MP1i3뇨ionb二flag = 0
                      cons trained_i月rare七回＝flag = 0

                      still_ pict끄re_flag = 1



           stream_type = 0x4
           (I요：)/IFQ 13818日 A idi이

           res凹：ved = 7

           el日entaxy_PID = 0x3b

           rese工ved = 15
           ES_info_leng나l = 3



                      descriptor_tag = 3
                       (audio_stream_descriptor)

                      descriptor_length = 1

                      free_f orma七小flag = 0
                      ID = 0

                      layer = 0

                      v끄riable rate audio indicator = 0
           reserved = 2


cRc 32 = 0xde1e刃a6


七Sc> COfl七
     工기4比： PU) 小＜39 de七ected (payload：
In七el：                                尸UI-li七1star七_indica七or) .


tsc> d工ip
sync_byte = 0x47
transport_e工ror_indicator = 0

payload_unit_start_indicator = 1
transport_priority    = 0
PID = 0x39
trar띄叩比1多cra姓）ling_con口：ol = 0
ada尤ation_field.工on七rol = 1
（均n七inuity_coun七er = 6
47 40 39 16
00 00 01 c0 01 6a 80 80 05 21 00 05 44 al 53 cb 2b 4b d5 8d 2a 33 e7
63 42 fa Ob 9d eQ 4e 48 81 ee 83 5b 17 39 f2 6b 09 46 05 ae 5b 58 f9
f3 e6 b5 af 9a c2 00 00 28 89 ld e7 35 ec 91 b6 dd 99 9b ac 3c bO c9
42 dd 29 85 ab d2 cf dc c3 6a e3 4d dl 8a fd 84 f5 e3 8c 6e d8 65 74
b0 f9f3     5ad7cd6b5b6dc6667df7def7           上氾 且＞ eeeefbefndef
7bdeeeefbe 日그def7df7def7bdef7bdef7bdef7Jdef7bde
b63e7cf9ad6be6b5ae38e3             33bef그cf7bdf7e07777df7de
f7bdef77       77df7def7befbef7       넜ef7bdef7h1ef7bdef7bd


七sc> pes
PES 什＝거斗＝r


packet_sta此Hcodej江ef뇨 = 000001
stream_id = OxcO
PES工acket_length = 362
'10 '
p邱_scramt丑in王（兀ntrol = 0
PE니Priority = 0
data니alignn日it_indica七（>r := 0

copyright = 0

original夕rc아乃／ = 0
prs_tirs_f lags = 2

S즈艾：R_fl ag = 0

珪; ra七e뇨flag = 0

DSMt工ick니nk:月已flag = 0

ad五tiorial_（兀마mfo_flag = 0

PES_cRC_f lag = 0

PES_extension_flag = 0

PES_header_data_length = 5



'0010 '

PrS[32. .30] = 小＜O

mark臼r bit          = 1

PI'S[ 29. .15] = 0x0002

mark臼r bit          = 1

vrS[14. .01 = 0x22d0

marker bit          = 1



tsc> （갓in七

In七e工mJ1尤： PID 小＜38 먀北acted 似拓pta七ion나field) .



七SC> c口rrp

Syn（乙byte = 呱47
t工SI四porq叫error 끄코끄cator = U
                   （끄cator = U
payload니Un끄乙없：ar口＝끄1

transport_priority             = 0
P끄） := 0x38

transpor乙HscrarrD1그끄g_cont그幻-i = U
acia乂：at끄in小field＝尸cor止끄)工 := 3

continuity_counter = 4
47 00 38 34

83 10 00 00 09 fc fe b4 if f ft                    ft   ft   ft   ff   ff   ff   ft   ft   ft   ff   ft   ft   ff

ft   ff   ff   ft    ft   ff   ft   ff   ff   ft   ff   ft   ft   ft   ff   ff   ft   ff   ft   ft   ff   ft   ft
ff ff     ft ft ff ft ft ff ft if   ff ft if   ft ff ft ff ft ft ff ft ff ff

if   if   ff ft ff ft ff ff ft ft ft ff ff ft ff if     ff ff ff ff ff ff ft

ff   ff ff ft ff   ff ft ft ft ff ff ff ft ft ft ff ff ff ff ft ft ff ft
ff ff     ft ff ft ft ft ft ft ff ft ff ft ft ft ff ff 60 58 e6 58 6a le
3592 cf c9 a7 27 ac 1d46 d6 e3 ba 4b 15 a9 86 a7 75 6dd5 8b 15b2
f9 96 b2 04 ca 73 61 b8 d7 的 02 8a 0a 64 cd af 3d e4 0f b4 aS 9c c8


七Sc> af
Ad1尤a七i（丑i Field


adaptation_field_leng나l = 131


discon七ir그i七y_indicator = 0
random_access_indicator = 0
elen r止ary_strearn工nioni勻＝in（五cator = 0
rc之：ef lag = 1
o1X죠之_t lag = 0

splic ' p point_flag = 0
七ranspor七_pniva七e da七a나flag = 0
adaptation_field_extension_flag = 0


pr四ram_clock_refer回lce_base = 0x0000013 t9
reserved = 63

progr帥뇨clock工efer텨ice_extensi（끄l = 0x0b4


S七uf f_byte = 小＜ft 火 124


亡Sc> vcatch 0x38 ii止en工기四七 pusi
Adding a video P1]) filter.


tsc> con七
工I止err4比： P1]
           ) 0x39 de七ec七ed (1冶yload_uni上寸S七art乙indicator) .


tsc> dunp
syn（乙by七e = 0x47
MPEG 비디오


            t工an同刃玭_error_indicator = 0

           payload_unit_s七art_indicator = 1

            trans刃r七H皿iority = 0
           PID = 小＜39

            trar四port多cran幻ling_co枇rol = 0
           adaptation_field_control = 1
           continuity_counter = 8
           47 40 39 18

           00 00 01 C0 01 6a 80 00 00 82 38 9f 63 a8 7b 60 ae 7a 6c cc e9 9c cd
           88 d8 b0 519eb6 7867 8e 84 d9 Sb 65456176 0f aa 98 3c 82 8176
           3adcba2514e9d1d65ca0bb98d3             96 8b9b4d45a0 42 3c 35 d0
           7b a5 55 15 51 9d 4a fa a7 57 65 64 7e 56 e6 16 54 ld a2 56 55 25 8d
           b6d3 6a2548af6934e9        516d78ec6b463635ec6aa7          93 66a9
           9499 df24 38b3 8b76 49949522 5a26a3 8647656444 5e11 e4
           d8 05b5 56 싫D6e27 35 e6 6e39 29b9 54 7a f0 4d5ac6b2 10 a.5 16
           aS a6 04 af b2 7d 64 75 0e 91 29 50 92 9f 28 d5 9d 57 d9 6c 9a 97 5d


           亡Sc> pes
           PES H由der


           packet_s七art_code_pref ix = 000001
           stream id = OxcO
           PES_packet_length = 362
           '10 '
           P邸_scraml표in工con口ol = 0
           F匹：
             工riority = 0
           data_alignrrnt_indicator = 0

           C（그1乃／right = 0
           original_or_c아乃／ = 0
           PTS_LIPS_f lags = 0
           EXR_f lag = 0
           ES니ra七e뇨flag = 0
           1石Mt工ick니1在Dde뇨flag = 0
           additional_copy_info_flag = 0
           PES_cRC_f lag = 0
p邱1e＞比ex四如n나flag = 0
PES_header_data_lerigth = 0


tsc> cont
In七err四t: PID Oxl de七ec七ed.


七Sc> d工11)
易m乞旬te = 小＜47
七ran틔；)ort_e工ror_indica七or = 0
payload_unit_s七art_indicator = 1
transport_priority = 0
1？끄） = 小(1
t그：ansport多cran幻ling_control = 0
ada比ation_field니cont工ol = 1
continuity_counter = 1
47 40 01 11
00 01 bO lf    ft ft cl 00 00 09 14 00 05 eO 50 43 41 Sf 44 45 53 43 52
5f 50 52 49 56 41 54 45 d0 4e 0f 5b ft ft ft ft ft ft ft ft ft ft ff
                        ft tf tf ff ft ff ft ff ft ft ff ff ft ft ff ff
                        ft ft ft ft ft ft ft ft ff ff ft ff ff ft ft ft
ff ft ft if    ff ff ff ft ff ff ft ft ff ft if   ft ft ff ff ft ff ft ff
ft ff ft ff ff ff ff ft ft ff ft ft ft ff ff ft tf ff ft ff ff ft ft
ft ft ft ff ft ft if    ff ft ft ft ft ft ft ft ft ft ft ft ft ft ft ft
tf ff ff ft ft ft ff ft ft ft ff ft ft ft ft ft ft ft ft ft ft ft ft


tsc> ca七
Conditional 石ccess Table


七ble id = 0x1
sec七ion나S）及1tax나indica七（>r = 1
'0   '



reserved = 3
sec七ion구巴9냔｝ = 31
res臼：-V日크 = 小旺ft f
rese工＼尼d = 3
MPEG 비디오


           versi이_i flu耐光r = 0
           C山丁曾it next乙indica由r = 1
           sec亡ion fli5T：冷r = 0
           las七 sectI （丑1 nuinb크r = 0



                    descriptor_tag = 9
                     (CA_descriptor)

                    descriptor_length = 20
                    CA나sys匕an니ID = 0油
                    reser＼尼d = 7
                    CA P끄） = 仍＜50

                    priva七e data1-t：근）
                                     ／七e三 =
                             43 41 5f 44 45 53 43 52 5f 50 52 49 56 41 54 45


           cRC_32 = 0xd04e0f5b


           七Sc> con七

           Inte工：工갸J1北： PID 0x38 de七ec亡ed (pay1oadl끄uit_start_i工idica七（Dr) .


           七Sc> （出口rtp

           syn（乙旬七e = 小＜47
           transport_error_indicator = 0
           payload_unit_start_indicator = 1

           transport_priority = 0
           PID = 0x38

           transport多cra岫llng_c(丑it工아 = 0
           ada1尤a七ion日field_c이止끄＞1 = 1
           continuity_counter = 5
           47 40 38 15
           00 00 01e0 0f fe80 00 007061614d8a6042             98 83c6 80d5b4ec
           Of di a7 57 16 87 Sd 56 e7 c8 58 68 7c 50 9b e8 10 d4 c9 aa ft ac 92
           53 42 6a Od 90 7b 6a 4d b6 as 95 0a be a8 a3 82 lb 85 72 53 54 72 78
           55 6d5690d9bOd5 fec3cbaa374f258531db1621c842                        802d
           6e ld 86 c8 81 be 03 80 a6 d9 32 25 53 al 2c 63 5b 43 57 2d 86 48 80
           3c 8a 43 29 bc 87 58 99 83 cb 21 8d 00 e9 bd 64 a5 ad 80 7c le de 41
 C0 38 ca 3692 5b 36 d5 aadd le cbaa 1273 2e 6992 dO c3 9bc3 e4
 86 42 9b d2 f7 85 ac 42 e2 56 la 5a b2 8f 01 cO c5 46 b7 8a 4c if   63


 tsc> pes
PES FT二뎌月Pr


packet_start_ code_pref ix = 000001
stream id = OxeO
PES냐月cke七H노ng난I := 4094
 '10 '
PES_scrair丑뇨으－-cOntrO1 = 0
PES_priority     = 0
data_aligrntent_iridicator = 0

C（不）yrigh亡 = 0
origirial夕rc（刃y = 0
PTSprS_f lags = 0
ES그
  （eflag = 0
ES_rate_flag = 0

D臼L七rick井月e_f lag = 0
ad키上ional_c叩）二in요乙flag = 0
PES_cE<_f lag = 0

P표乞飮七帥sion_f lag = 0
PES_header_data_l可gth = 0


七Sc> con七
In比rn 比： PEr) 小＜39 de七acted (1月yload_unit多tart_indica七or)
                                                            .


t.sc> durtp
Sync_i乃／七e = 0x47
transport_error_indicator = 0
payload_unit_s七art_indicator = 1
trans 그r七_;江如rity = 0
P끄：) = 0x39
七ransport_scran幻hir으J兀nt그그＞1 = 0
adaptation_field_control = 1
MPEG 비디오


           cc江止inuity_coui北er = 10
           47 40 39 la
           00 00 01 c0 01 6a 80 80 05 21 00 05 55 81 f0 92 97 25 3a 54 a4 67 45
           94 77 5c e0 65 d9 c8 cO cc c4 a2 ae c7 21 d8 66 33 6d 55 54 9e d6 5a
           8455 29b6 2fb6 8428 c4 8c 33 da 68 aa 20 de 15 fb 3c ac f168 28
           85856948454260 dell          8e 4252 b7 lc 6ab5 5f 3eadd6 edd7 32

           28b8 23 日：)52 35ce82 a93a42 t兀2d9cd9 4a35 5d59 9a3173 a6
           94 Sb 49 a6 5a 67 a9 a3 37 a2 Se 21 96 b6 f4 d6 63 ae c7 43 07 73 39
           4a 9d af al c4 73 86 c8 41 4d cd 7c 4d cd aS Of 9b 65 35 c5 da 19 a6
           38 bc 6d79 6685 6ab8 a9 88 611c 600611 끄：) 86 e152 6949 a4 b8



           七Sc> pes
           PES Header


           packet_start_code_prefix = 000001
           stream id = OxcO
             packet_leig口l == 362
           P田_

           * 10 '
           P邸_scrarnbling_con匕rc江 = 0
           PE니Priority = 0
           data_alignirent_indicator = 0
           copyri야比 = 0
           or!孕nalmor c아Y = 0
           PTS_E1rS_f lags = 2
           표互：R_f lag = 0

           ES_rate_flag = 0
           1石M뇨七rickj往月e_f lag = 0
           additional_copy_info_flag = 0
           PES_cRC_f lag = 0
           PES_ex七ension_fl ag = 0
           PES_header_data_length = 5


           '0010 '
           Pl'S[ 32. .30] = OxO
           ma 來er bit = 1
 ?TS[ 29. .15) = 0x0002
It日工ker bi七 = 1
PTS[14. .0) = 0x2ac0
1mr}咤r bi七 = 1


七SC> COfl七

In比LL'尤： PU) 仍＜37 detec七ed.


tsc> duirp
sync乙t乃比e = 0x47
transport_error_indicator = 0
payload_unit_start_in五cator = 1
transport工riority = 0
P끄） = 0x37
七ranspo比_scraml江in王con七rol = 0
ada1北ation_field_c이吐工（Dl = 1
cot止如Ui七）
        乙cour止er = 1
47 40 37 11
00 28 fO 끄：) 00 00 cl 00 00 4e 45 54 57 4f 52 4b Sf 49 4e 46 4f 5f 54
41 42 4c 45 52 15 dd 6c ff ff ff ff ff ff ff ff ff ff if           ff ff ff ff
ff ff ff ff ff ff ff ff ff ff ff ff if         ff ff ff ff ff ff ff ff ff ff
ff ff ff ff ff ff ff ff ff ff ff ff if         ff ff ff ff ff ff ff ff ff if
ff ff ff ff ff       ff ff ff ff ff ff ff if   ff ff ff ff ff ff if   ff if   ff
ff ff ff ff ff       ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
ff   ff ff ff ff if     ff ff ff ff if   ff ff ff ff ff ff ff ff ff ff if     ff
if   ff   ff if   ff ff ff ff if   ff ff ff ff ff ff ff if   ff ff ff ff ff ff


七sc> pry
1노iva七e Sec亡ion


table id = 0x28
sec七ion日ynta)＜日indica七（Dr = 1
private_indicator = 1
reserved = 3
section_leigth = 27
MPEG 비디오


           table ide：
                    比帥sion = OxO
           rese工ved = 3
           version x피ml氾r = 0
           current nex七 indicator = 1
           section number = 0
           last sec七ion_numl冶r = 0

           private_data_byte =
                      4e 45 54 57 4f 52 4b Sf 49 4e 46 4f 5f 54 41 42 4c 45


           七sc> con七
           끄止ertUP七： PID 0x50 de七日北ed.



           tsc> &nrp
           syn（乙切te = 小＜47
           trans刃比_error_indica七or = 0

           payload뇨unit_s匕ar七_indica七or = 1
           transport_priority = 0
           PID = 0x50
           七ransp吐L多cran的hir旺ecor比r아 = 0
           adap七a七如n뇨field_<兀nt工O] = 1
           continuity_counter = 1
           47 40 50 11

           00 29 f0 10 00 00 cl 00 00 43 41 5f 49 4e 46 4f 06 05 ab 18 ff ff ff
           ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
           ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff          ff
           ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff if          ff ff ff ff if
           ff ff if    ff ff ff ff ff ff ff ff ff if   ff ff ff ff ff ff ff if     ff ff
           ff ff ff ff if    ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff if       ff
           ff ff ff ff ff ff ff if    ff ff ff if   ff ff ff ff ff ff ff if     ff ff ff
           ff ff ff ff ff ff ff ff ff ff ff ff ff if      ff if   ff if   ff ff ff ff ff


           tsc> pry
           Priva七e Sec七如n


           table id = 0x29
                                                                       부 록

sec七ion_syI止ax_indica七（Dr = 1
private_indicator = 1
res臼：ved = 3
section_length = 16
七able i工e)＜七ensi（丑l == OxO
reserved = 3
version nl. T1羌r = 0
C1끄丁en七 nex七 indica七or = 1
sec七ion nurni羌r = 0
la馱： sec七ion_nur幻er = 0
priva七e da亡a_b／七e ==
        43 41 5f 49 4e 46 4f


七sc> con七
In七凹江4比： p끄：) 小＜38 detec七ed (payl（그ad：그jnit：
                                           山_start_indicat그＞r) .


tsc> （由工Ip
sync_J 'te = 小＜47
trai）琢均rt er끄Dr_lndlca七or = 0
payload_unit_start_indicator = 1
tran駐x＞此priori亡y = 0
PID = 小＜38
tr히nsport乙多cran幻ling_cont끄＞1 = 0
ada光a七k丑1土iel之cont工皿 = 1
con七in王jit=coun七er = 12
47 40 38 lc
00 00 01 e0 0f fe 80 00 00 c4 d2 e2 04 b7 4a a8 e6 e7 6d la a9 cO de
6a 06 9b 60 50 07 8d bf 68 75 83 4f 50 b3 9b 6c b6 16 39 81 b6 8e le
d6d2d5ae07 47d6f1b099adeef8               6f 0b9132a8d6 2b36a8 fd
47 46 33 3a c8 fc b4 b8 b0 86 13 08 6d cb 13 c6 fl 4b 85 29 e4 96 ef
37 Gb 60db f3 f5 a5 d6 d7 cdb9 96 c2 ca 5900 d5 6f 6a 23 e6 bf 4c
78 e2 6c Oc 83 40 a2 db cb la 6c 28 6c 3dbd 98 ed 56 e6 85 b0 0000
010b52d9 f12a737baa96d6 f0b4e6 f7552d6e2e06b7d2 91
7f 41 6d af 85 04 34 b0 71 6c b4 b2 43 Sc dc 2d f5 2d 4d ae 44 3c ea
MPEG 비디오


           tsc> pes
           PFS}卞＝거r과F>r



           F姐cket_sta此1code山ref ix = 000001

           str由m id = UxeU

           PES_packet_length = 4094

           '10 '

           PES吼ra址丑ir旺下on七rol = 0

           PE니Priority = 0
           data_all孚mem＝끄Iclicat（끄r = U

           C叩yri야比 = 0

           original夕乙co乃r = 0
           PTS_tTS_f lags = 0

           ESc日f lag = 0

           ES_rate_flag = 0

           DSM_trick_rr月e_f lag = 0

           a苡lit끄Dnal_copy_lrlt（乙nlag = U

           PES_C묘
                （乙flag = 0
           PES_e）比ensi이느flag = 0

           P邱_header_data_length = 0



           匕sc> cc江I七

           Interrupt: PID 0x39 detected (payload_unit_start_indicator) .



           七Sc> d工1耳：)

           sync_byte = 0x47
           transport_error_indicator = 0

           payload_unit_start_indicator = 1

           transr刃此_priori勻／ = 0
           PID = 0x39

           t工ansport乙scra岫lin工con比ol = 0

           adaptation_field_ control = 1

           continuity_counter = 12
           47 40 39 lc

           00 00 01 c0 01 6a 80 00 00 4d 6b 5a d6 a7 7e 09 a4 f7 32 5f bl 43 a3
                                                                        부 록


 94 6944a5 5ccdc4495499ca99          且） 31b127 34 에D4ca641da97
 66 36 5d 76 b9 32 aS 36 5b 3a 59 24 84 c3 la d6 b6 06 Cf 56 aa 2a 66

 a9 4e 71 85 75 df ld 89 5c d5 a9 66 da a9 cc 33 59 d4 ae 95 99 b0 95

 cd9cd8e2a3       25c1298e4ecd16cc534e76b5eee742               104ea4
 18 50 3f 95 26 4c 55 db b8 17 41 71 36 f2 4e c5 07 c8 65 e4 2e 42 e8

 96 dc 51 6b 56 94 24 2d 29 5a 39 lc 43 69 87 43 Sd Od 2a 71 5a a8 c5

aca42e50ead5d936553c64534a45b78a67a2a51b38596d



 tsc> pes
PESt乖＝거dnr



packe乞HS匕ar亡code나江efix = 000001

str田m id = 小＜cO

PES_packet_leng나l = 362
 '10 '

P표乞scr&t幻ling_control = 0

P표｛
  四riority     = 0
data_alignn 砒_iridicator = 0

C아刀rig比 = 0

original_ or_copy = 0
PTS_DrS_f lags = 0

E요玉뇨flag = 0
ES_rate_flag = 0

D쿄4m七nic凡J1YDde뇨flag 二＝ 0
addi七ional小C（그py_inf a；
                      口flag = 0
P邱니cm_f lag = 0
PES_extension_f lag = 0

P邱_header_data_l帥gth = 0



tsc> Cont
II吐：
   臼：工up亡： PID 缸38 de亡ec七ed (payload_unit_start：
                                               寸indica七or) .


tsc> duiTp
sync_b七e = 0x47

transi均rt＝臼m끄1ir五ca七or == 0
MPEG 비디오


           payload_unit_s七art_indicator = 1

           transport_priority   = 0
           p끄：) = 0x38

           transport_scrambling_control = 0
           ada光a七ion_field뇨的nt丑江 = 3

           continuity_counter = 3
           47 40 38 33
           07 1000001145 fe9c000001e00ffe80000036d48bc1c5b2
           6f b3 9a 6e d7 c2 63 f7 6c 0a 48 71 f0 2d b4 36 2e d7 76 b크 0a a9 0e
           b0 9989 6a 59 2a 0e a7 56 dc de 4bb6 6e 4b 0e 66 d4 e5 6c fc 80 e7
           4249 0dal a8 78 0e 7425 b2 la 14 4b 61 a9 97 b4 68 di aS 9b 53 43
           66e49a022c2100b5b4b66e4073a124a8d63586a66962d1.

           a3 4336ac68d2 605c6c34fa02e6d7a740l5c6cb4fal351Xl
           98 03 9a 10 c9 ad 963538 7b 5c d5 64 5b lbcaa7    5086 la 9d 9bad

           f2 e7 28e4 56 f3 4507 ca38 84decc f6 f0 3f 00 14b9 100712 2a


           tsc> pes
           PES Header


                           prefix
           packet_start_code_         = 000001
           stream id = 0xe0
           PES_packet_length = 4094
           '10 '
           PE좌_scran幻1뇨旺con比O1 = 0
           PEs_priority = 0
           data_a1ignnnt_thdicator = 0
           （兀pyr均ht = 0
           original_or_copy = 0
           PTS_DTS_f lags = 0
           표艾：瓦jlag = 0
           표乞ra七e_f lag = 0
           I石卜4_trick니m>d已flag = 0

           additional_copy_info_flag = 0
           PES_cRC_f lag = 0
           P邸1ex七em）釘on뇨flag = 0
PES_h田der_data_length = 0


tsc> （그丑l七
끄比回如1尤： P11) 小＜39 dete（北ed (payload_unit_start：戶．indica七or) .
tsc> d工11)
sync_i乃／te = 小＜47
transport_e工끄江i1五ca的r = 0
payload_unit_sta此_indicator = 1
transport_priority   = 0
PID = 0x39
t工an斗力比_scrart蚊in工con口ol = 0
adaf尤a七ion_f iel工ont그그＞1 == 1
continuity_counter = 14
47 40 39 le
00 00 01 c0 01 6a 80 80 05 21 00 05 66 61 59 cc b4 63 97 48 78 27 83
88 58 76 67 63 2a 91 61 dd d9 ad a9 85 a7 55 23 89 55 da 61 2c d6 53
c6e376b77bc2         042a94d6a8 92td14a6ed6acac1b3              8769de
9d l乂 db c2 22 al b6 dd 44 Sd 88 f4 6b 513a aa 32 a3 49 a6 94 c8 b5
12 aa a7 51 b6 에：) 96 ac 61 ce 8c 5a 에D ddbe 4c f0 56 c4 ld 2642 4b

8490a0ce36a32a1acdeca921f5e6cd48747a6961561198
da1328b6db75a4d5cce3a2b6ca552842294737                   00419d61
led6 0f a4 5d 33 13 50 ce 8c e8 7108 ef 2f 93 0b25 ba cab4 c6 ad


tsc> pes
PFS 什＝거月F>r


packet_s ta七_code_ 江efix = 000001
streanuid = OxcO
PESI月cket_len야］l = 362
'10 '
PES_scrarrbling_control = 0

PE니priority = 0
data_aligr五唯止J珏五ca七or = 0
C叩yri야比 = 0
original_or_copy = 0

                                                                             辯


                                                                         ；難轟蠱蠱   玉．
                                                                                  籌：
MPEG 비디오


           Prs_刃S_f lags = 2
           且丑R_f lag = 0
           E즈；1尸ra七e니flag = 0
           DS'1_trick_rr月e뇨flag = 0

           addi七ional_copy小info뇨flag = 0
           PES_cRC_f lag = 0
           E邱尸‘e）比en.sion뇨flag = 0

           PES_header_da七al可呵口l == 5


           '0010 '
           PTS[ 32. .30) = OxO
           marker bit = 1
           PTS[ 29. .15] = 0x0002
           marker bit = 1
           PTS[14. .0] = 0x3330
           0日rker bi七 = 1


           七SC> C0fl七

           Inte工m叩七： P11) 小＜38 detec匕ed (1月yload_uni늑多ta此 ir虹ca七吐）.


           tsc> （如Op
             （乙tyte = 缸47
           syn
           trar同刃比_error_indica亡or = 0
           payload_unit_start_indicator = 1
           transport_priority    = 0
           PID = 0x38
           trans1刃r七1scran幻ling小q丑itro1 = 0
           adapta亡ion日field_cont工ol = 1
           conti工luity_coun七er = 10
           47 40 38 la
           00 00 01 e0 0f fe 80 00 00 3d 79 e5 9e Od e8 6e 4d 67 e7 8d 56 e0 6d
           58 71 ed 上冶 45 6e e8 a3 73 lf   8f 94 a4 bO Oa 6e 16 29 fl b9 9c 54 28
           a6 f9 eca5 35c3 8274 60d6 ld 0a 6a d6 0f 6d db 66 ab fa 77 f4 由
           5b 7d 6a c4 b6 51 95 工b e5 9c bf ld 55 54 74 6f aa 06 8f 2d af 5b di
           a8 d4 田：)06 3160 c5b크06 e9 6a 77 0b 8b 64 96 0c ad e5 ic 26 52 69
                                                                        부 록

56 f8 37 ad 71 32 35 0d 9e 6d c3 9b a3 72 69 ed 5f eQ 73 51 끄：) a5 af
5a 50 e6 e3 f3 aebi 68 c6 f4 56 b8 64 a7 c6 e7 b5 8911 ba 2d1f 19
8d a3 eQ 5a 34 2d 51 48 6c 끄． 6a aS a5 05 92 9b al bl 6a d5 08 e7 c2




PES H田der


packet_star七1cc月e工ref ix = 000001
streamid = Qxe0
PES_ 月cket_leng갔l = 4094
'10 '
p丑三多cran幻un且1的nt如1 = 0
PES_priority    = 0
data_aui箏men七_indica七or = 0
copyright = 0
original느夕r_copy = 0
PTS_rrrS_f lags = 0
ES(工나flag = 0
ES_rate_flag = 0

D因L七rick끄Dde_f lag = 0
additional_copy_info_flag = 0
E心1四C.－寸flag = 0
PES_extension_f lag = 0
PES_header 奴七a나leng나I = 0


七sc> con七
In亡err口1尤： P:r) 0x39 detec七ed (1月yload_山lit多tart_indicator) .


tsc> durrp
sync슈byte = 小＜47
transport_error_indicator = 0
payload_unit_start_indicator = 1
trans1均r七니？riority    = 0
p끄） = 0x39
tran斗力rt＝吼ran幻hiog_con口oh = 0
                        MPEG 비디오


                                                                        ada尤ation_fi eld_control = 1
                                                                        continuity_counter = 0
                                                                        47 40 39 10
                                                                        00 00 01 C0 01 6a 80 00 00 6c c2 85 98 92 Ib 15 d6 b9 ce d6 69 10 1크
                                                                        81 ae 7374 c7 2d 67 2f Oc 97 ad77 75 d8 dd 8de6 le 21 51 5da9 46
                                                                        el dl cIa 2125 c8 5d 99 b2 73 6db7 62 8d 7b eb 13 5908 29 Gb 61 0b

                                                                        dd4a8lf59a9994         hCea7a52e72cb3 f03f62b43b55b7cb9d
                                                ::::::::::::::::::
             ;:::::::::：再：朴堪；煎：:::::::::::::::::::::：든룐玄；
                                                                        4b 54 f9 b7 d5 8c la 91 a7 41 c7 d2 43 69 36 5d ae c7 42 bl 69 18 Sc
  驩難難饌磁髓춈難難宙辯立｝i
   :::::::::::::::::::::::::::n::::::::::::::::::：그：沁：::::::::::::::;   b5 ce 6d 9c d2 12 23 a7 71 37 ef 62 62 84 7c 9e cc fc 51 73 45 4d 99
                                                                        lf   14 fl 0e 68 03 c2 0e 24 ca al 32 22 17 42 a8 db 18 0c 05 aO cf Se
                                                                        b62478 68dbd1ef 6b610720 9e29 1a79e2d53deecbc63dcb


                                                                        tac> pes
                                                                        PES Header


                                                                        packet_start_code工）refix = 000001
                                                                        stream id = OxcO
                                                                        P표3냐）ack就_leng냔l = 362
                                                                        '10 '
                                                                        1必＝_scrambli工ig_cont그：ol = 0

                                                                        PES냐江如rity = 0
                                                                        data_alignrrent_in五cator = 0

                                                                        c（그pyrigh七 = 0
                                                                        original_or_copy = 0
                                                                        PrSmJ)rSmflags = 0
                                                                        ES心Lflag = 0


蠶難難難m
蘿難蘚醬難驪難籌難難羅難푿
                                                                        표乞ra七e_f lag = 0
                                                                        D쿄L七rick_n 扼1flag = 0
                                                                        additional_copy_info_flag = 0
                                                                        1丕'S中（：요c_f lag = 0

                                                                        PES_extension_flag = 0
                                                                        E쯔느header_da七a日1色目th = 0


                                                                        七sc> cont
                                                                        In比工mJ1尤： PIt) 小＜39 de七ected (payload_un1t多tartJndica的r) .
tsc> d工rp

Sylk乙I刀七e = 0x47

transport_e工ror_indicator = 0

payload나unit_s七ar七miridica七or = 1

transport_ 江iority = 0

PID = 0x39

trans1x江t_scran幻1뇨ig的nt丁ol = 0

ada尤atior)나field나cont工ol == 1
continuity_counter = 2
47 40 39 12
00 00 01 C0 01 6a 80 80 05 21 00 05 77 41 5a d8 68 56 58 9a a3 Sf 35
b2b21녔45 出：)c9a3l687587b8aa8a87a98id079a66l65l83
203463 67 la cc b8 e3 5ab2 b2 d0 97 2e 6103 9db6 日：) 52 d5 4471
657452 a6 e9 49 b3 0c dO ef 7dle 1de2 226261 d5 5d 6244 9d 95
9a 95 a6 73 bi 14 8ba3 2980 ab 593972 e2 49 if     3d 52 9b 6529 ce
62 03 14 94 Ib 21 b5 33 73 16 f3 lx 34 31 cd a9 9a 99 le 81 eb c6 32
ed844a94a649 66 f1bcd424d2 2d4b4da67c fa6d6b4489ad
6b 61 06 b4 00 00 00 ff fc b4 04 Gb 16 55 54 44 55 55 66 55 43 43 44


七sc> pes

PES H田der



                prefix
packet_s七art_code_         = 000001

St그：
   田In id = OxcO

PE乞packe七11色哄士l = 362

'10 '

1狂Lmscran幻ii皿U兀毗rol = 0

PRS냐止如rity = 0

data_aligrnTent_indicator = 0

C（그1乃irigh七 == 0

original_ or_copy = 0
PTS_DTS_f lags = 2

E 그Lflag = 0
ES_rate_flag = 0

D 4_trick_ 幻de_f lag = 0
MPE(; 비디오


             additional_copy_info_flag = 0
            p且3=（玉C_f lag = 0
            p표乞炚七色）駐on놔flag = 0
            PES_header_data_1ength = 5


             '0010 '
            PI'S[32. .301 = Ox0
            0日工ker bi七 = 1
            PTS[ 29. .15] = 0x0002
            0日rk吐 bi七 = 1
            PTS[14. .0) = 0x3月0

            0四來凹rbit = 1


            tsc> con亡

            Internipt: P11) 0x38 detected (payload_u此_start_indicator) .


            七Sc> duirp
            sync_I乃／te = 缸47
            tran同刃r七H旦：
                      ror_ nc五cator = 0
            payload_unit_start_indicator = 1
            transport_priority    = 0
            PID = 0x38
            transrx江t_scran幻1mg_n丑itr아 = 0
            adaptation_field_control = 1
            continuity_counter = 1
            47 40 38 11
            00 00 01e0 0f fe80 00 00b6a6 56e3 52 37 70a3 16 8e94b6ed01
            b8cd86af      f27c 哉i27ab79c3 4a4ideOa8ade9dd1             6c6e71 f4
            2b 6f 8b 79 fO b3 db 66 a7 3b fd df Od c4 88 b2 86 17 25 2a 12 lb bd
            4b b6 8d b4 b6 c9 c8 0e 74 04 40 03 48 02 f0 96 d4 dd 9a 7d 6c a) 6a
            ddb5 db 36 if    2a 81 41 0d 47 3c de 6972 if   50 a8 75 2d 0a 43 8636
            c6 8d 6a 31 93 60 ci 8b 46 a6 ia b3 c3 c7 ca 56 85 52 48 63 55 62 14
            dd 98 55 8d c3 d8 9b b0 35 be 47 ad be a6 ed ad 4e dO ci 8b 06 f9 56
            ea6d18b0 68c3 36d1a3 46 0c32 6c 583160c3 0da3 7278 2f if
                                                                          부 록nm                            g
tsc> 1氾S




                                                                                       在
l毛SF口n日F>r



                                                                       難蘿；
packet_start_code_pref ix = 000001                                     醬蠶箋
                                                                       址；
                                                                        ：珌；
                                                                          ：珌注

stream_id = 0xe0
                                                                       難難難難難
PES_packet_len七h = 4094
                                                                       驪難m
                                                                       鑿驪V    m臺貫



                                                                       吐
'10 '
p표乞配rathh江ir咀工on七如1 = 0                                                難蠶難驪量驢돌mm難難i

PES_priority   = 0
data니a1igrreit_ix그dica七（Dr = 0

copyright = 0
original_or_copy = 0
prS_DTS_f lags = 0                                                     難小難難驪難難
咀：
 B나flag = 0
                                                                                1I
ES工a七e_f lag = 0                                                            느堆竝控珌고；:::::::;:；卦布好：:：吐；::::::F:;F可4可易每：斗：斗1                :::
                                                                                                                              !:i三：;:;:;:;:;:i
                                                                                                                               ;:;:;:;:;:;:;:;:
DSM_七rick.jrcde_flag = 0                                                                                              往聾群鮮裝｛
                                                                                                                       囊；蟹器i要
addi七如na느opy_inf o_f lag = 0                                                                                                ;：」：::i;:::::::::::
                                                                                                                  ;:;::;：뇨：느：
                                                                                                               客裝燕聾甕景蘚甕：
                                                                                                                                  芬：i:i:iE
PES_cPC_f lag = 0                                                                                                                 :f

PESext：
      帥Si（丑i_flag = 0
PES_header_data_leigth = 0


tsc> con七
Intei그nJ1尤： 1江I) 小＜39 de七e（北ed (payload_unit_star七_indica七or) .


tsc> dunp
sync_byte = 小＜47
transport_e工ror_indicator = 0
payload_unit_start_indicator = 1
transport_priority   = 0
P11) = 0x39
七ransport_scrambling_control = 0
ada就毗如i_field_cont丁ol = 1
con七inuit止cou毗er = 4
47 40 39 14
00 00 01 c0 01 6a 80 00 00 18 38 la 34 22 d8 de Sc Be 69 b2 6d Oc 49
MPEG 비디오


            69 52 93 33 89 12 31 6b 73 96 60 5c bc 07 33 53 34 da a6 ce 87 67 58
            63 84 4d 67 b6 76 ha f0 7e lb 5e39 田：)d4 el 1文） 20 6c d6 10914976
            5d 506252 54 b7 ldbl     22 35 ac 65 ac 5415 ad 53 ae fi dc fO eb le
           dc263d331512d88d6755c2666cc14b9175016cd2a68992
            64 4db6 4d 92 Sd 221文） 77 aa 9a 35 f4 a6 1052 94 ec 6c 38cc ac 3e
           a3 9e 54 b6 88 75 12 51 64 d5 59 95 62 e8 ha 95 59 86 b7 22 95 0d e3
           91be5b03 41a6 f5        三47ab6a5520 69 3a75ad5ac1518e79d4


           七Sc> 下冶S

           PES Header



           packet_s tart_ code_prefix = 000001

           streE匹n id = 仍＜cO

           P旺냐沮味就小length = 362

           '10 '

           E표乞scrai曲ling_cont工ol = 0

           PES냐江如rity = 0
           data니alignu日止 indica七or := 0

           copyright = 0

           original_or－르＞1乃r = 0
           1玎S니끄S_f lags = 0

           EScR_fl ag = 0

           匹Lra七乞flag = 0

           DSMt工ic乂皿넜之flag = 0
           additional_copy_info_f lag = 0

           P邱J꼬（乙flag = 0
           I표乞畔tension나flag = 0
           PE=header_da七a_len야：
                              h 二 0


           七Sc> con七

           In亡e工工-UI：尤： PID 仍＜4d de七ec七ed.



           tsc> 凸mP
           易及Ic 1:乃／七e = 小＜47

           trarlsl兀rt_error_indica七C丁 = 0
payload_unit_start_indicator = 1
 tran琢均rLpriority = 0
1？끄） = 小＜4d

 tra斗ort_ scrambling_control = 0
adap七ation日日el己cont그그＞1 = 1

C（끄itinuity_c（그Un七er = 4
47 40 4d 14
00 02b0 1d00 01 c100 01e0 38 fO 00 02 e0 38 fO 03 02 01 01 04 e0
39 f0 03 03 01 02 7b e4 31 42 ff ff ff ff ff ff if             ff ff ff ff ff if
ff       ff if   ff ff ff ff ff ff if   ff ff ff if   ff ff ff ff ff ff ft ff if
ff if       ff ff ff ff ff if     ff ff ff if   ff ff ff ff ff if   ff ff ff if   ff
ff       ff if   if   ff ff ff ff ff ff ff ff ff ff ff ff ft ff ff ff ff ff ff
ff       ff if   ff ff ff ff ff ff ff ff ff if     ff ff ff ff ff ff ff ff ff ff
ff if       ff ff ff ff ff ff ff ff ff if       ff ff ff ff ff ff if   ff ff ff ff
ff ff       ff ff ff ff ff ff ff ff ff ff ff ff ff if       ff if   ff ff ff ff ff


tsc> rint
Program Nap Table


tableid = 0x2
sec七ion뇨多丑止財뇨indicator = 1
'0
     '



rese工ved = 3
se北ion나length = 29

pr（好ram_nunt冶r = 0xl
reserved = 3
versi（丑I nus止氾r = 0
CU工rentnexti工Idica七（Dr = 1
sec七ion I끄Jnt光r = 0
las七 section nun고光r = 1


rese工＼/e크 = 7
PcR PID = 0x38
res臼：ve크 = 15
   ran느info_lengt士l = 0
pr四：
MPEG 비디오



           stream_type = 0x2
           (ITt.J-T Rec. H. 2621150/IEC 13818口 Video

            or ISO/IEC 11172-2 constrained paranEter video stream)
           res凹：
               ＼尼d := 7
           elaTenta工y_P끄） = 奴38
           reserved = 15
           ES_info_length = 3



                  descriptor_tag = 2
                   忖ideo_stream_descriE尤吐）

                  descrip七or山Hlen드；th = 1
                  rr&iltiple_ frarre_rate_f lag = 0
                   frare rate code = 0
                  M:PB3_l_only_f lag = 0
                  con馱工ained_paranE七er_flag      =    0
                  眺ill_ picti；
                             工E乙flag = 1


           strearn_七YE冶 = 0x4
           (ISO/Is그 13818尸：3 Aidi이
           reserved = 7
           e1qnen七axy_PIIJ = 小＜39
           res回：Ved = 15
           ES_in fo_length = 3


                  descriptor_tag = 3
                   (audio多口曲in_descri1尤or)
                  descrip七or_leng납l = 1
                   free_forn t_f lag = 0
                  ID = 0

                  layer = 0
                  variable rate audio indicator = 0
                  rese工＼厄d == 2


           CRC 32 = 0x7be43142
      七Sc> con七
      Interru比: PID 劤＜4d detected.


      tsc> （加rrp
      sync_1,yte = 0x47
      t工帥斗,ort_error_i珏虹catc江 = 0
 paylo&工uni口戶tart_i珏坵at力r = 1
      t工ansport 江的rity = 0
  Pl工） = 0x4d
  tran斗刃r七scranbiir므下on比C江 = 0
 adapta七ion니field니control = 1
 c（丑止inuit乙counter = 5
 47 40 4d 15
 00 02 bO id 00 02 ci 01 01 e0 3a f0 00 02 e0 3a f0 03 02 01 01 04 e0
 3b f0 03 03 01 02 de le b7 a6 ff ff ff ff ff ff ff ff ff ff ff ff ff
 ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
 ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
 ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
 ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
 ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff
 ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff ff


tsc> pnt
Program Map 丁able


table id = 仍口
section_町砒aJri竝cator = 1
 '0
       '


res町＼7的 = 3


                          四 毗
sectior_].d目th
prograxn.工l皿t氾r
r（蛤吐ved = 3
＼應rsionji工吐冶r == 0
currentjiext_indicator = 1
sec七ionJ1l끄苡氾r = 1
MPEG 비디오


           la馱： sec七ion nu姓氾r



           rese工＼尼d = 7

           R그t P끄＞ = 小＜3a

           rese工＼尼d = 15

           pr四ram_u迂乞1包啄：
                        i-i = 0



           stream＝七yr氾 = 0x2

           (ITU-T Rec. H. 262IIS3/ m      13818-2 Video
            or ISO/ I且그 11172口 con馱工ained pararr七er video str曲in)

           rese工V日 = 7

           e1aentary_PID = 小＜3a

           rese工＼尼d = 15

           匹Linfo4le四나l = 3



                     descrir尤吐tag = 2

                     忖ideojtre帥＝descrip的r)

                     descriptor_leng너口l = 1

                     mul七ip1e_frane_ra七e뇨flag = 0

                     frane rate code = 0

                     M1묘乞1_oni止flag = 0

                     cons七rained 月rane七回乙flag     =   0
                     still_ picture_f lag = 1



           stream_ty冶 = 0x4

           (ISO/lEr 13818-3 Audio)

           reserve    = 7

           elanntar乙PID = 0x3b

           rese工ved = 15

           표Li-nfo_leng比 = 3



                     descriptor_tag = 3
                     (audio_stream_descriptor)

                     descriptor_length = 1
                     free_fonit_ f lag = 0
                 ID = 0
                 layer = 0
                 Va工ial丑之rate_audio_i皿五ca的r = 0
                 rese工＼
                      ／日크 = 2


c        _32 = 小cd日eb7a6


七Sc> cont
Interru北： PU) 小＜1 detec七ed.


 tsc> durrp
syncJ刀te = 0x47
trenSrx江t包ror_i珏五cator = 0
payload_un!七1多七art_inc五ca七（Dr = 1
trans1均氏- 江如rity = 0
PID = 小d.
transport乙多cran幻ling_cont工（>l = 0
ada尤a七ion나field_con匕幻1 = 1
cor止inui勻二counter = 2
47 40 01 12
00 01 b0 lf          ff ff ci 00 00 09 14 00 05 e0 50 43 41 5f 44 45 53 43 52
5f505249564l5445d04e0f5bffffffffffffffff                                     ftffff
ff       ft if    ff ff   ff ff ft ff ff ff ft ft ft ft ff ff ff ff ft ff ff ff
ff ff       ft ff if      ff if   ft ff if   ff ff ff ft ff ff ft ff ft if   ff ft ff
ft ff       ff ff ft ft ft ff ff ff ft ff ff ft ff ft ff ft ft ff ff ft ft
ft tf       ff ff ft ft ff ff ff ff ff ff ff ff ff ff ff ft ff ff ff ff ft
ft ff       ff ff ff ff ft ft ft ft ff ff ff ff ft ft ft ff ff ff ft ft ft
ff ff       ff ff ft ff ft ff ff ff ft ft ff ff ff ff ff ff ft ft ff ff tf


七sc> ca七
Conditional 玉ccess Table


table_id = 小＜i

section_syntaxjsidicator = 1
'0
     '
MPEG 비디오


           rese工＼尼d = 3

           section_length = 31
           rese工＼尼d = 小＜ffff
           res曲：
               iie크 = 3
           \／回石ion flUITt羌r = 0
           （크J工rent next indica亡（>r = 1
           section num羌r = 0
           la引： secti아lnum氾r ＝二 0



                   descriptor_tag = 9
                   (C2노descrip七or)
                   descriptor_length = 20
                   CA_systan_ID = 0x5
                   res凹入尼d = 7
                   CA_P표） = 0x50

                   priva七ed亡ita나by七e =
                           43 41 5f 44 45 53 43 52 5f 50 52 49 56 41 54 45


           CRC 32 = 0xd04e0f5b


           tsc> cont
           끄lter工UI尤： PU) 小＜38 de七ected (I月yloa 그끄ii七尸多七art i工dica늡그r) .


           tsc> dunp

           syn（乙byte = 小＜47
           transport_error_indicator = 0
           payload_unit_start_indicator = 1
           transport工）riority     = 0
           PID = 0x38
           trar巧I兀rt_scrambl뇨으下ontrol = 0
           adaptation_field_control = 1
           continui勻二coun亡er = 8
           47 40 38 18
           000001 eQ Of fe 8000009843 8da9 9993 36 d.c 80 0a le 7c d.c fc
           ed 0e 90bcb4 28 b0 84 9073 6c e5 e4 f7 ebdi 0da5 40 c8 5409 al
 ada9 8b 26 a4 6d4e 54 d9 4759 7c 285129 b8 d7 b7 3f ce 3e 6997
 9a fc 31 16 2f a4 0d 48 58 da dd e6 Cd 4d Od b2 72 ft 3d 59 12 66 4c
 c8 3520 fa dada 3064 c3 6c a6 af 9144 cf 52 d5 b4 5a 6db6 9f 6d
 ac ec 59 bO d8 34 68 c5 93 Gd 71 f0 8f 2e ca 3f id 40 20 6e b9 96 aa
 41 ad cd 3f 38 a3 &1 3d 2d 8d dO f2 b5 68 c2 8b 09 18 ca 45 39 a9 a9
 e1dceb8ef0a7      37 0blf   1f46 0e2c73 76 5fc571 63 152865 ic


四c> pea
 PES Header


packet_start_Code_prefix = 000001
streanuid = 0xe0
PES_
  packet leng갔l = 4094
 '10 '
P표乞scran幻hir으H的ntrol = 0
PES니pri吐ity = 0
data_aui邙皿日깠：_ind.ica七（>r = 0

copyri야比 = 0
original_or_co乃r = 0
Prs；
   끄始뇨flags = 0
E,9R_fl ag = 0
ES_rate_flag = 0

D臼L口ick냐a月e니flag ＝二 0
additional_copy_info_flag = 0
PES_그
    （_f lag = 0
PES_extension_flag = 0
P표乞hea西rd砒a_length := 0


tSc> con七
끄ltel그4比： P끄） 小＜39 dete（北ed (payload_unit_start_indicator) .


tsc> di工rp
5yncJyte = 0x47
七rar）워；均r七_error_indica七or = 0
payloa&i끄d七_start_indica七or = 1
MPEG 비디오


           trans乂）rt_priority = 0
           PID = 0x39
           transp江t多cran幻ling_的ntrol = 0
           ada화a七1아i_f iel之con七rol := 1
           C아北inuity_counter = 6
           47 40 39 16
           00 00 01 c0 01 6a 80 80 05 21 00 05 88 21 a5 5d cb e6 奴 b5 6a 53 96
           d6 b6 27 52 72 73 5e 82 67 c2 58 62 6e 74 bl 43 14 3a 52 aS 53 dl b6
           9aad06d1284341e4422489386429aa7cad32e2447a6450
           a54a20dad6be3bed4cecc230f328cf689ad3b94aa98399
           4a 39 70 9b 96 lc el dl 14 62 d8 e3 44 cc 27 4c 89 2d 39 4b 86 95 7a
           e9 5b 54 eb b5 ad 6b 5a d0 00 00 00 ff fc b4 04 le 87 55 44 33 65 56
           56 55 55 54 55 34 91 24 a4 49 22 49 00 00 00 00 00 aa be aa aa aa aa
           aa 由aaa4 93 4d 35 da59 a5 96 5d75 d7 5d75d8 5d86 1969 a6 9b


           七Sc> pea
           PES H由der



           packet_欲ar七下ode山ref ix = 000001

           streamid = OxcO

           P旺냐月cket_leng냔l = 362

           '10 '

           1표t多cran幻hio且con口幻1 = 0

           PES_priority   = 0

           data_alignrrent_indicator = 0

           copyright = 0

           original_or_c아乃r = 0
           PrS_끄S_f lags = 2

           匹蚣R나flag = 0

           표tra七e_f lag = 0
           D釵d냐：nic凡irnde_f lag = 0

           add!七ional_c叩y_inf（乙flag = 0

           PES_cRc_f lag = 0
           PE.S니e>＜七ension니flag = 0

           PES_header_data_length = 5
'0010 '
1刃rs [32 . . 301 = 小＜0
trarker bit = 1
PrS[ 29. .15] = 0x0002
rrerkerbit = 1
PTS[14. .0] = 0x4410
ii日rkerj竝七 = 1


tsc> con七
工ntern 比： p工D 缸37 de七ec七ed.


tsc> d口ITP
syncjyte = 0x47
t工ansport_err吐_indica七C江 = 0
payload나unit＝多tart_indicat刃r = 1

t工an斗刃rt냐江iority = 0
PID = 出＜37

trar珥力比_ crarrbl뇨咀下ont工ol = 0
adaptatiorLfield._contro1 = 1
cc江北mlu虹）'- coun七er == 2
47 40 37 12
0028 f0 1b00 00 ci 0000 4e45 54 57 4f 52 4b Sf 49 4e 46 4f 5f 54
41 42 4c 45 52 15 da 6c ff ff ff ff ff ff ff ff ff ff ff if                 ff ff ff
ff   ff   ff if   ff   ff ff ff ff if   ff ff if   ff ff ff ff ff ff ff ff ff ff
ff ff if     ff ff     ff ff ff ff ff ff ff if     ff ff ff ff ff ff ff ff ff ff
ff ff     ff ff   ff ff ff ff ff ff ff ff if       ff ff ff if   if   ff ff ff ff if
ff   ff ff   ff ff ff if     ff ff ff ff ff if     ff ff ff ff ff ff ff ff ff ff
ff   ff if   ff ff     ff ff ff ff ff ff ff ff ff ff ff if       ff ff ff ff ff ff
ff   ff   ff ff if     ff ff ff ff ff ff if   ff ff ff if   if   ff ff ff ff ff ff


tsc> pry
Priva七e Sec七ion


七able id = 小＜28
MPEG 비디오


           section_syntax_indicator          = 1

           private_ indicator      = 1

           rese工＼尼d = 3

           sec七ion뇨．
                   length = 27

           tab1e_idextens ion = OxO

           res臼刃ed = 3

           version num氾r = 0

           current next indicator          = 1

           sec七1（丑1 fli丑趾氾r := 0

           is馱： sec七ion nuin冶r = 0

           priva七e_data뇨hyte =

            4e 45 54 57 4f 52 4b 5f 49 4e 46 4f 5f 54 41 42

            4c 45



           七ac> con七

           In七elmJ1尤： PID 0x50 d北ected.



           亡sc> （九끄m>

           syn（乙by七e = 0x47

           transport_ error_ 끄lcticator = U

           payloacl_unit_ 歐art＝끄l1lc司二or = .1

           transport_priority       = 0

           PID = 小＜50

           口：ansport多cran止）I끄ig_con亡rol = U

           adaptation_field_ control = 1

           con七inui七＼/ C（그unter = 2

           47 40 50 12

           00 29 f0 10 00 00 ci          00 00 43 41 5f 49 4e 46 4f 06 05 ab 18 ff          ff   ff

           LE El: Er El: El: El: El: El: El: El: Er El: El: El: l:E EE El: l:E El: El: Er El: El:

           EE EL E1 El: EE Er El: Er El: l:E El: El: l:E Er Er El: El: EL El: El: El: EE EL

           EL EL El: El: El: El: El: rr     El: El: El: El: l:E Er El: tE El: EL El: El: El: EL LE

           EL EL EL El: EE EE Er El: EL El: El: El: l:E Er EL EL El: EL EL EE El: El: Er

           EL EL l:l: El: El: El: El: El: El: El: El: El: EL EL EL EL El: EL EL El: EL EE rr

           EL El: El: El: l:l: El: l:E El: El: EE El: El: El: El: EE El: l:E Er El: El: El: EL EL

           EL EL El: El: EE El: rr       tl: EE EE El: El: EE Et El: El: El: EL EL El: l:l: EL EL
tsc> pry
Priva七e Sec七ion


亡able id = 0x29
se（北如n日syr止카_indica七C江 = 1
private_indica七C江 = 1
rese工＼尼d = 3
section_length = 16
七able id e>＜七日四ion == OxO
rese工ved = 3
versi（工- flu雌氾r = 0
ci江rent ne＞比 indica亡or = 1
sec七ion i코끄m冶r = 0
lastse（北ion flu沁羌r = 0
private_data나1:乃／七e =
 43 41 5f 49 4e 46 4f


tsc> con匕
In七el工'4尤： pn) 小＜38 de七ec七ed (payload_unit_s七ar七_indica七or) .


tsc> dunp
sync_ 乃／te = 0x47
transport_error_indicator = 0

payl(沮d나unit就ar七_indicatc江 = 1
transport_priority    = 0
PID = 0x38
t工ar囹叩比_scrant江뇨으下on亡rol = 0
a由1尤a七ion누fiel工con口ol = 1
continuity_counter = 15
47 40 38 lf
000001 e0 0f fe 80000012 61 cdel d5 95 5b22 7b 6a 63 54 5f 5b
76 cd30 39 1462 b6 3ad5 c6 eb 84 d6 e7 3a 35 7f e9 5bb7 62 6c 2e
52 d9 f8 9f 98 de 76 49 af 7a 86 37 la 3a 4a 53 79 6a 8d d7 5a aS cc
b5b크8dd7db0a84b6f2           l5ba 68 ad4b15 2c 6d2aa2 c3 e3 53 fe
85 f3 dd4de8 cl d5 4737 b2 6f 8d Ob 1137 2ed3 e4 6f a2 79 4adc
MPEG 비디오


           91 06 31 54 6그 6f Of ec 08 60 0c eO b2 18 58 0b 9b 06 c3 62 53 99 32

           18ec83a460de4214df71b536d6a87a19d5e26a6aca32b6
           31 5d 63 dc 5c 2d 6b 72 db 8d c4 88 de a7 25 22 37 80 29 f7 55 58 00




           1毛S H月dnr



           Packet_start_ code工）ref ix = 000001
           針：ream_id = 小＜eO

           p邱山acket_1日珂냔l = 4094

           '10 '

           1표乞吼ran幻ling_con七rol = 0

           PES_priority   = 0
           data_alignrrent_indicator = 0

           copyright = 0

           origin丑1or c아Y = 0
           PlS11)rS1flags = 0

           묘艾艮flag = 0

           ES_rate_fl ag = 0

           D쿄4口ick냐a月e_f lag = 0

           additional_co乃_in fo_flag = 0

           P묘3=（그之
                 （乙flag = 0

           E厄S呼七帥sion나flag = 0
           PES_h由der_dat之length = 0



           tsc> cont

           Ir止臼：mJ1比： p工D 缸38 de七ected (r月yloa卞n1t多ta此Uindica七（)r) .



           tsc> dinTp

           sync_byte = 0x47
           trar囹；'or七H町ror_indica七or = 0

           payload_unit_start_indicator =

           transport_priority   = 0
           P1D= Ox38

           transport_scran幻hr으1的nt工丑 =
a（拓pta七ion_field_con七rol = 3
（兀1北inuity_c叩玭er = 6
47 40 38 36
07 10 00 00 if a3 7e 18 00 00 01 eO Of fe 80 c0 0a 31 00 05 93 61 11
0005 3f 01 ac 93 a7 Sf 6f 2a ac cd 26 b3 31 aa 7eb6 4d 6c 65 a3 79
e5 91 9d 55 99 ac 91 aa 9e 91 68 c6 9e 68 de 75 23 03 23 42 c6 b6 ad
75 fc da b3 63 62 32 35 b5 d2 b3 29 93 54 c2 c6 50 8a db 08 01 ac 2b
a8 ca cd 93 53 f9 58 d4 37 7f f3 la 95 7c 2d b4 46 86 dc 66 46 ed 90
47 c6 ce 41 8d 48 c9 b7 31 9db4 79 ca cS hi ad 93 54 11 51 a2 b3 b5
d629ec9a5a9f9995ba7e43ad8c89a3d866db9ac5b74b5b
3c aa cd 86 00 00 01 22 52 al fi 2a de 9a ad la de 6a 9c de 87 2a 14




packet_ tart_co扼_ 江ef ix = 000001
str由xn_id = 小＜eO
E丕滔4)ack就尸1吐呵갔l = 4094
'10 '
p표乞恥ran幻lbaqJ刃nt工（Dl = 0
PES_priority = 0
（姐ta_alignnent乙如dica七or = 0
cc刃yri的t = 0
origna1_or_copy = 0
PTS I丑乞flags = 3
ES玉1土lag = 0
ES_rate_flag = 0
D쿄_trickj     de_flag = 0
addi七ional中copy_info．
                    土lag = 0
p邱＝eR乙flag = 0
PES_extensior나flag = 0
p邱＝header_data나leng七i-i = 10


 '0011'
P'rS[ 32. .301 = 小＜0
MPEG 비디오


           marker bit = 1

           FrS[ 29. .15] = 0x0002
           marker bit = 1

           PTS [14. .0] = 小＜49b0

           marker bit = 1
            '0001'
           DrS[ 32. .30] = OxO
           marker bit = 1
           DrS[ 29. .15] = 0x0002
           marker bit = 1
           DTS[14. .0] = 0x1f80
           It日rker bi七 = 1


           七sc> con七
           Inte工mJ1尤： p끄） 小＜38 de七e北ed (1月파oa之unit就art乙indicator) .


           七sc> （加娘）
           Syn(乙by七e = 小＜47
           t丁an司刃rt_error_indica七or = 0

           payload_unit乙多tar七Hind1ca七or = 1
           transport_priority    = 0
           pw = 小＜38

           transport_scrartbling_control = 0
           a（泊就a七ion_f iel叱con口ol = 1
           continuity_counter = 13
           47 40 38 id
           00 00 01 eO Of fe 80 00 00 a7 02 e9 02 41 c6 aS 74 80 d3 80 c0 42 73
           e2 86 88 33 39 ac 07 14 aa 27 la 09 51 4a 20 72 14 47 b7 fb 80 06 f0
           10 80 e5 12 71 84 3f c8 c4 66 15 58 e3 fc id id c8 26 07 끄． 39 50 63
           f0 69 ff f8 78 07 70 00 be if   44 e8 61 13 08 72 78 lb c4 6b 03 eO aa
           00 50 50 06 el fO la a2 50 a0 cb 83 0b 12 e6 4a 00 la 6c 4e 58 00 di
           89 47 d0 63 8a 끄． e2 98 f5 9f 0e 06 7f ff 84 51 34 ff 00 0d e크 84 9d
           82c090752dOf96ce8e28aa6fla70e82b37ec718859                      6b 田
           01 fd73 b9 00 c3 0091 eldb 98 aa24 fa Oc 9842 0003 c8 3838 3f
PES Header


packet_start_.아月e工refj그＜ = 000001
stream id = 0xe0
PES_packet乙1包l9七h = 4094
'10 '
P邱_scraml江ir旺下ontrol = 0

PES_priority    = 0
data_aligrirrnt_indicator = 0

copyright = 0
original_or_copy = 0
PrS_DrS_f lags = 0
E&系나flag = 0

ES니ra七e_f lag = 0
DSN七rick日nK)de_f 1四 = 0
additional_copy_info_flag = 0
P邱_cRC_f lag = 0
P邱1ex七ension니flag = 0
PES_header_data_length = 0
                                   저자약력


.유시룡                                       S깁종일
 1972년 서울대학교 전자공학과 졸업                      1988년 연세대학교 전자공학과 졸업
 현 대우전자 상무（TV사업부장）                         1990년 연세대학원 전자공학과 졸업（석사）
                                           현 대우전자 영상연구소 주임연구원
S장규환
 1977년 서울대학교 전자공학과 졸업                      S정해묵
 현 대우전자이사 （영상연구소 담당）                       1985년 서울대학교 전자공학과 졸업
                                           1987년 서울대학원 전자공학과 졸업（석사）
S 이 병욱
                                           1992년 서울대학원 전자공학과 졸업（박사）
 1979년 서울대학교 전자공학과 졸업
 1981년 KAIST전기 및 전자공학과 졸업（석사）              현 대우전자 영상연구소 선임연구원

 1991년 Stan如rd Univer前ty졸업（박사）
 현 대우전자 영상연구소 수석연구원




                MPEG 시스템1
                1997년   8월    5일      초판 인쇄
                1997년   8월 10일        초판 발행


                저   자 : 유시룡 · 장규환 · 이병욱 · 킴종일 · 정해묵
                발행인 : 최 정 헌                          r


                발행처 : 大 其 社．                             인 지
                        서울시 서대문구 충정로 3가 &5           L


                        전화 : 393-0417--8
                        팩스 : 313-0104
                        등록 : 제 9-204호

                 妓 잘못된 책은 바꾸어 드립니다．
                ISBN 89-7163-075-2-93560


                정가 ]0,0(刃원
