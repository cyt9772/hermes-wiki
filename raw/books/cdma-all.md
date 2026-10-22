---
source_url: /run/media/yutae/Data/CDMA의 모든 것.pdf
ingested: 2026-10-22
sha256: 6d3f344c018d56e9fc5e102d91e05c3b3cfa7ba7d60e7a1c3dfdd3efa785b36f
---

# CDMA의 모든 것 (raw source)
> Text-layer PDF (poppler pdftotext -layout), Korean, 530p, 2002.

## Book metadata
- title: CDMA의 모든 것 (CDMA All-inclusive)
- author: 김갑용 (Kim Gap-yong) — cover/front-matter credit "김갑용 지음", 진한도서
- publisher: 진한도서 (Jirihan Books INC.), 2002
- ISBN: 89-8432-087-0
- pages: 530
- price: 24,000원
- note: "우리나라에서 CDMA가 상륙한 지도 벌써 10년을 넘어섰고... 한국은 세계 최초의 CDMA 상용화를 성공하였으며, 지금은 2000만이 넘는 사람들이 CDMA 방식의 휴대전화기를 사용" (머리말)

## Chapter structure (from TOC)
| # | topic |
|---|------|
| 1 | 이동통신방식 (Cellular 이동통신, 무선전화/TRS, 기지국-셀, 주파수재사용, S-95 and Friends, 표준화 ITU/TIA/3GPP2, PCS 시스템, 망자원할당) |
| 2 | Basic Concept (Correlation & Normalization: 자기상관/직교/규준화, 선형계(LTI), Fourier 변환과 신호분석) |
| 3 | DSSS와 코드이론 (DSSS, Walsh/Gold/PN code, IS-95) |
| 4 | CDMA Demodulator (PN code 동기, Rake receiver, despreading) |
| 5 | 전력제어 (CDMA power control, closed/open loop, near-far effect) |
| 6 | Handoff ( 셀룰러 핸드오프, soft/hard handoff) |
| 7 | 무선전송기술 (Qualcomm, IS-95, vocoder, channel estimation, interleaving) |
| 8 | 호처리 (call processing, channel assignment, congestion) |
| 9 | Vocoder (voice coder, AMR, IS-2000/CDMA2000) |

## Extracted text (poppler pdftotext -layout)

e77진한도八1
    머리말                                             3
.




    우리나라어］ CI呱/IA가 상륙한 지도 벌써 10년을 넘어섰고 그러한 와중어］ 한국은
세계 최초의 CI呱끄＼상용화를 성공하였으며, 지금은 2000만이 넘는 사람들이 CI呱4A
방식의 휴대전화기를 사용하면서 이동 통신 서비스를 사용하고 있다．
    이와 발맞추어 우리의 기업들은 수많은 CDMA제품들을 생산하고 수출하고, 또
한 운영하고있다. 즉 CI呱dA와 관련된 일을 하지 않는 정보통신 업체가 없을 정도
로, CDMA기술과 관련된 기업체가 늘어가고 있다. 따라서 수많은 Cl孤'IA기술자들
이 필요하며, 또한 CDMA기술자들이 있다. 이 책은 매년 증가하고 있는 수많은
CI呱/11\ 신입 사원들이 CDMA를 두고두고 공부하기에 알맞은 책으로 제작되었으
며, 기존어］ CDMA분야에서 일해오던 사람들도 이 책을 통해서 기존의 CDMA와
관련된 많은 오해와 궁금증을 깨끗이 정리하고 나만의 논리체계로 CDMA를 정리
할 수 있을 것이다．
    이 책은 크거］ 9장으로 나누어져 있으며 1장 Cellular 이동통신방식과 2장이 Basic
Conce吼, 3장 DSSS와 코드이론에서 이동통신과 CDMA의 기본적인 이해를 위하1
서 먼저 공부하게 된다. 이러한 지식은 이 책의 전반에 걸쳐서 항상 문제를 푸는 열
쇠가 될 수 있는 단서가 되므로 정확하게 공부해야 할 것이다. 특히 이러한 내용을
좀더 심도 있게 이해하기 위한 공부는 2장에서 하게 될 것이다. 우리가 2장을 통해
서 수학을 공부하는 것은 단순히 수식을 나열하기 위함이 아니라 수식이 내포하고
있는 함축퇸 의미를 찾아내는 것이고 새로운 의미를 부여하는 것이 목적이다.
    4장 CDMA Demodulator, 5장 전력제어, 6장 Handoff는 CDMA의 핵심 기술들
로 무엇보다 중요하게 공부해야 할 부분들이다. 4장에서는 초기 PN Code의 동기와
이러한 코드의 추적어］ 대해서 공부하며, 아울러서 Rake 수신기의 동작어］ 대한 공부
를 하게 된다. 5장 전력제어에서는 CDMA의 전력제어의 방식과 그것들의 의미와
문제점 등어］ 대해서 공부하게 된다. 흔히 하는 말로 작전어］ 실패한 지휘관은 용서받
을 수 있을지라도 배식어］ 실패한 방위는 용서받지 못한다는 말과 같이 전력제어어］
실패한 CDMA는 용서받을 수 없다. 6장에서는 셀룰러 이동 통신 시스템인 CDMA
    4                                               머리말
                                                          1


시스템에서의 Handoff어］ 대해서 공부하게 되며, 최근어］ 개선된 Hando侄어］ 대한 공
부도 아울러서 할 수 있다. 현재 CI呱IA와 관련되어 국내외에 공개된 특허 중
Handoff와 전력제어 관련 특허가 상당부분을 차지하고 있다는 것만으로도 이러한
것이 얼마나 중요한 내용인지 짐작할 수 있을 것이다．
 이 책의 7, 8장은 현재 우리나라를 비롯하여 미국 등지에서 서비스되고 있는 상용
CDMA인 Qualcomm사의 CDMA를 예로 들어서 CDMA시스템의 무선 전송 기술
(WI丁 : Radio Transmission Technology）과 호 처리어］ 대한 공부를 하게 된다．
이어서 9장 Vocoder에서는 7, 8장의 IS-95 혹은 IS-2000（북미지역에서는 C먀na2000
이라고도 함）을 기반으로 하여 전송되는 Be町er인 음성신호의 부호화 방식과 복호
화 방식어］ 대해서 공부하게 퇸다. 통신 또는 이동통신의 발전형태가 음성 위주의 저
속에서 데이터 위주의 고속으로 바꾸어 가고 있는 상황에서 Bearer가 음성 신호어］
서 데이터 신호의 기능이 커지고 있고 따라서 이와 관련된 기술권고나 기술 사항들
이 무선 데이터 서비스라는 이름으로 발전해오고 있다．
 이 책의 특징은 크게 3가지로 이야기할 수 있다．
 첫째 새로운 표현과 언어를 사용하였다. 우리가 어떠한 내용을 이해하는데 에는
사람마다 나름 데로의 방식으로 이해하고 설명하고 응용할 것이다. 동일한 개넘일
찌라도 그것을 표현하는 방법은 대 부 분 으 비슷할 것이나 사람마다 다른 것이 일반
적이다. 따라서 이 책에서는 우리가 상식처럼 알고있는 혹은 꼭 그렇게 표현해야 퇸
다고 하지도 않았는뎨 그렇게 표현하지 않으면 안 된다고 섕각하는 식의 표현들을
지양하였다. 즉 어느 책을 보나 천편일률（千篇1律）적인 내용들을 좀더 다른 표현
으로 설명하였다. 사실 우리의 기술서적 중에는 최초의 번역자의 번역 오류조차도
묵인된 내용을 포함하고 있는 것이 없다고는 할 수 없다.
 둘째로 독자들의 이해를 돕기 위해서 삽화를 많이 사용했다. 삽화는 본문 내용을
다시 요약하써 그려놓기도 했지만 삽화 자체가 또 다른 설명을 하고 있는 경우라고
보아도 될 것이다. 이러한 그림들은 독자들만의 생각어］ 편견과 선입견을 심어주는
결과가 될 수도 있겠으나 방향타가 되리라는 기대를 한다．
 직관적이지 못한 지식은 완성되지 못한 지식일 수 있다. 자신의 지식을 자신의 직
관으로 바꾸지 못한다면 그것은 아직은 미완성일 가능성이 있다. 이 책의 서］ 번째
특징은 적절한 예화와 예문이다. 전자기학의 발전의 틀에는 앞서서 연구되었던 역
학의 틀어］ 기초하였듯이 우리의 생활 속에서 일어나는 수많은 일들이 우리가 공부
                                                 5


하는 공학어］ 적용되어 지는 것을 우리는 알 수 있다．
 누구나 쉽게 알 수 있는 내용은 그리 깊지 않은 내용일 것이다. 또한 누구나 알고
있는 지식은 그것의 가치가 크지 않을 것이다. 이 책은 " 알기 쉬운 ··· " 이나, " 일주
일 만하면 ··· " 등과 같은 관용사를 사용하지 않았다. 또한 이 책은 알기 쉽게 쓸려
고 했지만 알기 쉽게 알 수 있는 내용들은 아니다. 한가지의 내용을 두고 고민하고
고민하는 가운데 정말로 귀한 나의 지식과 나의 논리체계를 가질 수 있을 것이다．
 끝으로 이 책을 통해서 CDMA를 공부하고자 하는 모튼 독자들께 감사 드리며 부
족하지만, 그들 모두에게 이 책이 참신한 동기부여와 복퇸 복음의 소리가 되었으면
하는 바램입니다．


                                            2002. 7. 17
                                              옥윤철
         차 례
     .




4,       이통통신방식                                                      25
           1.1   어科선 Al口1스                                           29
                 1.1.1 무선전화（Cr : Codeless Telephone)                 29
                 1.1.2 和斗1-I= 공용통신 시스템（TRS : Trunked Radio System)   30

           1.2   셉룰21 이동통신                                           32
                 1.2.1 기지국과 셀                                        32
                 1.2.2 주파수 재사용                                       36

           1.3   "'仄1딜 통신 기II요                                       44
                 1.3.1 So丁ce Coding                                  45
                 1.3.2 C떠nnel Coding                                 46
                 1.3.3 Modulation                                    47
                 1.3.4 Frequency Spreading                           49
                 1.3.5 Multiple Access                               50

           1.4   S-95 and Friends .                                   51
                 1.4.1 표준화 동향                                        51
                 1.4.2 표준화 기구                                        52
                 1.4.3 ITU(Intemationa1 Telecommunication Union)     52
                 1.4.4 TIA(Telecommunication Industry Association)   55
                 1.4.5 기타                                            59
                 1.4.6 IMT2000을 위한 표준화 . 3GPP/3GPP2                  60

           1.5   PC$ 시스끼1                                             62
                 1.5.1 시스템의 구성                                       62
                 1.5.2 망 자원 할당                                       64
             8                                        차례
                                                           .



巨）
     Basic
                     Concept
                                                           67
             2,1   CorreIation그1 Normalization                 68
                   2.1.1 자기상관（Aut아Correlation)             70
                    2.1.2 Orthogonal                       71
                    2.1.3 규준홰Normalization)                73

             2.2   산형겨'(Linear System)                         75
                   2.2.1 함수                                75
                   2.2.2 Linear Time Invariant(LTI)        77

             2.3   Fourier으1 신오븐석                              80
                   2.3.1 Fourier의 생각                       80
                   2.3.2 Fourier Spectrum                  81
                   2.3.3 Four妃r Transf아m                   83
                   2.3.4 恥urier 변환의 성질                     88
                   2.3.5 지수함수 e 1w0t의 Fourier 변환           91
                   2.3.6 주기함수의 恥U加r 변환                     91
                   2.3.7 신호의 에너지／전력 표현                     94
                   2.3.8 Matched Filter                    95

             2.4 工伊 01푠                                    97
                   2.4.1 자연 표본화（Natural Sampling)      100
                   2.4.2 순간 표본화（Instance Sampling)     101
                   A吐외 I시
             2.5   I.                                  103
                   2.5.1 데시벨（dB)                       103
                   2.5.2 대역폭（Bandwidth)                104
                   2.5.3 Error 함수 町的와 e加（力             105

             2.6   器（Noise)                            107
                   2.6.1 열 잡음m妃rmal Noise)             108
                   2.6.2 잡음지수                          109

         2.7       Shannon이 말口t는 六'I닐용량                112
  차 례                                                    9



唱／ DSSS오- （丸de이론                                             115

    3.1   Spread Spectrum                                    116
          3.1.1 Frequency Hoping과 Direct Sequence            117
          3.1.2 확산통신 : Direct Code Spread Spec甘urn           118
          3.1.3 확산의 의미                                       119
          3.1.4 확산통신의 정량적인 해석                                122

    3.2   CD州／CD川A 통신방삭                                      ]29
          3.2.1 확산동신과 기존의 통신                                 129
          3.2.2 CDMA 통신방식의 정량적 해석                            131
          3.2.3 Jamming과의 전투                                 134

    3.3   디1의왁장                                              !39

    3.4   용망                                         .       140
          3.4.1 얻랑 용량                                        140
          3.4.2 CD入4A 가입자 용량                                 143

    3.5   Code 小eo싸                                          152
          3.5.1 G키여s Field                                   153
          3.5.2 선형 Code와 생성 다항식                              154
          3.5.3 선형 Code의 대수적 표현                              157
          3.5.4 원시 다항식                                       159

    3.6   PN Code                                            163
          3.6.1 최장코드의 수                                      164
          3.6.2 PN Code의 특성                                  166
          3.6.3 PN Code를 CI呱4A에서 사용하는 몇 가지 이유                171

    3.1 놔비計i Code                                            172

    3.8   Gold Code                                          174
     I    10                                                        차례
                                                                         S



七）
         CDMA Demodul아or                                             177
          4.0   A1 E                                                     178
                 4.1 Searcher Engine                                 180
                 4.1.1 PN Code                                       181
                 4.1.2 Dwell Algorithm                               181
                 4.1.3 Searcher의 동작                                  182
                 4.1.4 주요 기능                                         185

         4.2    Searcher Block '     기눙                                  187
                4.2.1 SEARCH Block                                   189
                4.2.2 ACQCI표（ 미ock                                   192
                4.2.3 INC 블록                                         193

         4.3    Finger Demodulator                                       198
                4.3.1 RSSI(Received Signal Strength Indicator) 계산    199
                4.3.2 주파수 에러 산출                                      199
                4.3.3 Time Tracking - 위상추적                           200
                4.3.4 Phase Lock L兀p(PLL)                            203
                4.3.5 Delay Lock L刃p(DLL)                            205
                4.3.6 Tau( r) Dither Loop                            210

         4.4    Rake 수신기                                              212
                牛4.1 심벌 결합기（Syn倣이 Combiner)                          213

         4.5    Searcher Task의 동작－Sof押are                            219
                4.5.1 탐색 Parameter                                   220
                4.5.2 각 상태（S幟e）의 동작                                  221



         전럭저円］                                                      229
         5.1 오II 전릭'11어를 口II야 하는가？                                   229

         5.2    어띱게 전쩍져1어릎 하며 어핀 죵二m1 裝가？                            2和
                5.2.1 Forward 전력제어                                   232
                5.2.2 Reverse 전력제어                                   233
    차례                                                      11
N

     5.3   이동 통신 六It닐 특징                                         234
           5.3.1 Fading                                          235
           5.3.2 Delay Spread                                    236
           5.3.3 Doppler Spread                                  236
           5.3.4 음영현상（Sha面wi雎）                                   237
           5.3.5 인접채널 및 동일채널 간섭                                  237
           5.3.6 경로 손실（Pa血 loss)                                 237

     5.4 0pen Loop Power Control                                 238
           5.4.1 추정된 Access 출력                                   239
           5.4.2 개선된 Open Loop 전력 Estimation                     243

     5.5   Closed to叩 Power 白ntrol                               川4
           5.5.1 전력제어그룹 - PCG(Power Control Group)               245
           5.5.2 Forward 전력제어 부채널                                246
           5.5.3 Reverse 전력제어 부치俚                                249
           5.5.4 전력제어 부채널 전송 Timing                              250
           5.5.5 Gated M어妃에서의 동작                                 252
           5.5.6 전력제어 Bit (PCB)                                  255
           5.5.7 전력제어 임계치（전력제어 띠Fireshold)                       262

     5.6   0ther Closed Loop 산력 - t3 긴쩍끼어                        오飯
           5.6.1 관련 메시지 .1                                       263
           5.6.2 Fr跏ne error Rate 통꼐보고                           267
           5.6.3 단말기의 동작                                         267
           5.6.4 Gain 조정                                         269
           5.6.5 전력관리                                            271
           5.6.6 EIB/QIB어］ 의한 방법                                 272

     5.1 0uter Lo에1 Power Control                                214
           5.7.1 Outer Loop Power Contr이 관련 시스템 Parameter        276
           5.7.2 Outer L아1 Power Control Algorithm               277
           5.7.3 단말기의 Outer I兀op Power Cot血이                     281
           5.7.4 0uter Loop Power Control Parameter              281
      I    12                                                                               차 례
                                                                                                      a

           5.8    이 겅읖 따쳐핀시···
                                                                                                      283
                  5.8.1 瓦／N0와 FER의 관계                           ;                                284
                  5.8.2 전력제어의 불확실성                                                               285
                  5.8.3 간섭어］ 대한 향후 방법들                                                           285



/8'\ Hand。
         ff                                                                                   287
'＼寸
                         'mHmHm11미m口H=
                                           H1HHmmmmmHmmmmmHm=       mmmmmmmmm柶nmmmmm小H口H=
                                                                                             HHm蜘m加




           6.1   Han（托ff를 위깐 九rameter                                                             288
                  6.1.1 Pilot Set                                                                288
                  6.1.2 Search Window                                                            290
                  6.1.3 Threshold                                                                295

          6.2    Mobile Assistant Soft Handoff (MASH0)                                            298
                 6.2.1 Pilot Set의 천이                                                            298
                 6.2.2 Soft Handoff 절차                                                          303

          6.3    New Soft Handoff                                                                 309
                 6.3.1 Why New algori仕m?                                                        309
                 6.3.2 Dynamic Threshold                                                        311
                 6.3.3 Pilot Set의 천이                                                            312
                 6.3.4 Fast Rising Pilot                                                        314

          6.4    Hard Han山府                                                                      317
                 6.4.1 Hard Hando什 절차                                                           317
                 6.4.2 Hard Hand可1의 유형                                                         318
                 6.4.3 주파수간의 Hard Hando什                                                       319
                 6.4.4 RC간 Hard Handoff                                                        321
                 6.4.5 Hard Hando什의 메시지 처리                                                     322

          6.5    枇AHH0: M的扼 Assistant Hard Handi口if                  .                          攷5
                 6.5.1 Failure and Return                                                      325
                 6.5.2 Search기능                                                                327
                 6.5.3 入4AHHO를 위해 새로 지원되는 메시지들                                                 330
                 6.5.4 Call Flow                         .                                     337
차 례                                                              尸了
  6.6       Idle Handoff                                          339

            6.6.1 절차                                             341

            6.6.2 Neighb可 Configuration                          342


  6.7       Access Handoff                                        345

            6.7.1 Pilot Reporting                                346

            6.7.2 Access Entry Handoff                           350

            6.7.3 Access Probe Handoff                           351

             6.7.4 Access Hindoff                                352

             6.7.5 Extended System Parameter message             354

             6.7.6 채널할당 중 Soft Handoff                           356

  6.8       겅끼하기                                                  351




 Radio Transmission Technique                                    359

  1.0       Qualcomm의 기본쩍인 셍각은 ?                                  360


  1.1        Channel Coding                                       361

             7.1.1 Convolutional 부호화                              363

             7.1.2 Viterbi 복호화기                                   365

             7.1.3 路95의 Convolutional 부호화기                        367

             7.1.4 Code Symbol Repetition                         371

             7.1.5 티보 부호화                                         373


   1.2       Interleaving                                          378

             7.2.1 데이터 스크램블링                                      381


      7.3    Modulation                                            381

              7.3.1 디지털 천이 변조                                     382

              7.3.2 위상천이 변조와 BPSK                                 383

              7.3.3 QPSK(Quadrature Phase S址ft Keying)            386

              7.3.4 OQPSK(Offset Qua血ature Phase Shift Keying)    388

              7.3.5 瑥95의 변조                                       389

      7.4    다중호1와 =1중접속                                           393
 14                                            차 례
         1                                           1

 7.5 白rward 11l닙 구조                                  395
       7.5.1 Pu아 채널                              396
       7.5.2 동기채널                                 398
       7.5.3 호출채널                                400
       7.5.4 Forward 통화채널                        403

1.6   Reverse 1끼U 구조                                 407
       7.6.1 Access 채널                           407
       7.6.2 Reverse 통화채널                        411
       7.6.3 Reverse P加t 채널                      413



IS-95 Call Flow

8.1   Initial State 쳐끼                               4化
       8.1.1 시스템 결정 상태 : 사용할 시스템 선택              419
       8.1.2 P如t 획득 상태 : CDMA시스템의 Pu야 채널을 획득     420
       8.1.3 동기 획득 상태                            420
       8.1.4 시간 변경 상태 : CDMA시스템과 동기를 맞춘다         423

8.2   Idle(Page) State 쳐텨                            425
      8.2.1 Slotted Mode                         426
      8.2.2 호출채널 入4omtor                         429
      8.2.3 Overhead Messages update             431
      8.2.4 Page Match Operation                 436
      8.2.5 Broadcast Si아 M曲的ring                437
      8.2.6 Quick 호출채널                           440
      8.2.7 명령과 메시지 처리 동작                        441

8.3   Access Attempt State '口I                   445
      8.3.1 Access 처리                            446
      8.3.2 System Access의 Sub State             457

8.4   Traffic State 쳐끼                           463
      8.4.1 Service Option                       463
      8.4.2 Service 구성                           465
      8.4.3 Service 협상                           467
    차 례                                                             15
1

                8.4.4 Service 구성과 협상을 지원하는 메시지                           473

                8.4.5 I刃ng Code 천이                                       473

                8.4.6 통화 상태의 Sub Sta把관리                                  474

      8.5       단말기 식＝그1 뵤안                                              418

                8.5.1 단말기의 식별                                            478
                8.5.2 IMSI_S의 부호화                                        479
                8.5.3 Hash 함수                                            480

                8.5.4 의사 랜덤 발생기                                          483

      8.6       사용짜 인죵                                                    484

                8.6.1 개요                                                 484

                8.6.2 공유 비밀 데이터（ssI기의 갱신                                 486
                8.6.3 단말기 등록인증                                           488
                8.6.4 유일시도 응답（Un匈ue Challenge Response Procedure)        489

                8.6.5 단말기 발호인증                                           489
                8.6.6 단말기 착 호 인증                                         490
                8.6.7 CAVE Algorithm                                     491

      8.7       왁인깁싸                                                      495

                8.7.1 대기상태의 메시지 확인                                       495
                8.7.2 통화상태                                               499

      8.8       묶（Re如如如n)                                                 50口




     c。
／弓＼ V。 der                                                                     5

          9.1   Voice Source Coding 방식                                    吼6
          9.2   발셩의 윈a1                                                   508

          9.3   QCELP(Qualcomm Code Exited Linear Predictive)             511
                 9.3.1 스펙트럼 분석 : LPC(Linear Predictive Code)             513
                 9.3.2 Pitch탐색                                            520
                 9.3.3 Codebook 탐색                                        525

          9.4   짇숑릎 ］겅                                                    529

          9.5    길론                                                        531
     16                                       차 례
                                                    U




（표 1-1> TR의 종류                                      57
（표卜2> CDMA관련 IS 시리즈                                 58
（표卜3> 3GPP와 3GPP2이 비교                               61
（표 ?1) 정규분포의 확春 (x)                             107
K표 3-1> Erlang B Blocking Probability           142
（표 3-2) GF(23）의 모든 다항식에 의한 시퀀스 발생               159
（표 3-3> SR어］ 따른 최장 코드의 수                        165
（표 午1) 프로세서 정합 타이밍 조건                           196
<표 4-2> Searcher Parameter                      220
（표 午3) 하드웨어의 상태별 동작                             227
（표 5-1) Access Attempt 변수들                      241
（표 5-2> FPC小'JUDE어］ 따른 Forward 전력제어 Scheme      250
（표 5-3) 전력제어 duration및 전력 level                 256
（표 5-4) 시스템 Parameter의 전력제어 관련 필드               263
（표 5-5> PMI孤4의 전력제어 관련 필드                       265
<표 5-6> Closed Loop Power Control Step Size     266
（표 5-7) 기지국 변조기 ASIC의 전력제어 관련 write 레지스터        270
（표 5-8) 외부 루프 Parameter                         276
（표 5-9) 목표 FER                                  282
（표 臼1> Searcher ＼入／in面w 크기                      293
（표 价2> Han面If Dr야） T노ler 만기종료 값                 297
（표 6-3> Pilot Set의 전위                           301
（표 价4> SEARCH1TYI下 （兀des                        330
（표 6-5) 탐색주기 값                                  331
（표 6-6> SEARCH소'JUDE Ty1光5                      331
K표 6-7> CF_NGHBR_SRCI-LMODE                     333
（표 7-1> Cony아毗幻nal 부호화기의 연결                     365
（표 7-2) 데이터 Bit의 천공형태                           378
（표 7-3) 동기채널 Interleaver 입력 Frame               379
（표 7-4) 동기채널 Interleaver 출력 Frame               380
（표 7-5> QPSK 계열의 I, Q채널 위상 八'Japping            387
（표 7-6> 64진 직교심벌 집합                             392
（표 &1> Sl야 Cycle Index어］ 따른 검색주기                427
<표 8-2> Station Class Mark                      430
    차 례                                        17
口


'(표 8-3) Address Type                               432
K표 8-4> Preferred MSID Type                         435
（표 8-5) 명령 메시지의 명령코드와 ORDQ                          444
（표 8-6) 표준 Sei자ice Option에 대한 번호할당                  464
（표 斗7> Default Cot寸塘urati아1                         삯i8
K표 8-8) Service Option Categories                   471
（표 8-9> BCD대응                                       480
K표 8-10> Hash Function Modifier                     482
K표 8-11> Auth_Signature 입력 Parameter                485
（표 9-1) 속도 감소를 위한 타당한 속도 수정                         531




（그림 1-1) 일반적인 유／무선 통신 시스템                            26
（그림 1-2) 단말기 이동성의 발달                                 28
（그림 1-3) 무선전화의 발전                                    29
（그림 1-4) TRS의 채널 이용 방법                               31
（그림 1-5) 주파수 공용통신 시스템의 구성                            31
（그림 卜6) 셀의 크기와 전장의 균일성                               33
（그림 1-7) 다앙한 형태의 셀 배치                                36
（그림 1-8) 셀룰러 서비스의 예                                  37
（그림 1-9) 셀룰러의 서비스할 때 용량증가                            38
（그림 1-10) 자원의 재사용 계수가 7일 때 같은 주파수를 사용하는 인접 셀         39
（그림 卜11) 주파수 사용계수어］ 따른 셀 클러스트                        40
（그림 卜12) 주파수 재사용 패턴                                  41
（그림 1-13) 3 섹터 셀의 和斗수 재사용 계수와 거리                     42
（그림 1-14) 디지털 통신의 개요                                 44
（그림 1-15) ITU-R의 조직                                  54
（그림 1-16) PCS 망 구성도                                  62
（그림 1-17) BSS의 자원                                    65
（그림 2-1) 상관（Correlation）의 의미                         69
（그림 2-2) 직교신호로 임의의 신호표현                              73
（그림 2-3) LTI 필터                                      79
（그림 ?4) Fourier의 생각                                  80
      18                                                         차 례
                                                                       U

（그림 2-5) 주기 구형파의 Fourier Spectrum                                      82
（그림 2-6) 주파수와 시간의 장벽                                                   85
（그림 2-7) 임펄스 함수의 설명                                                    87
（그림 ?8) Filter와 八4odulation                                            90
（그림 方9) 디지털 신호의 대역폭                                                    93
（그림 2-10) 구형파의 에너지                                                     95
(그림 2-11) Filter System                                                95
（그림 2-12) matched filter의 모델                                           96
（그림 2-13) 임펄스어］ 의한 표본화                                                 98
（그림 2-14) Fourier 스펙트럼에 의한 표본화 정리 해석                                 99
（그림 2-15) Natural 표본화                                               101
（그림 ?16) 순간 표본화                                                     102
（그림 2-17) 순간 표본화의 임펄스 표본화로 등가화                                      102
（그림 ?18) 대역폭의 종류                                                    104
（그림 2-19) 정규분포의 확률 분포 함수와 확률（적분값）                                   1（馬
（그림 2-20) 일반적인 증폭기                                                  110
（그림 3-1) DSSS와 FHSS의 수학적 표현                                         117
（그림 3-2) 확산 변조의 신호 표현                                               118
（그림 3-3) 펄스의 Fourier 변환                                             120
（그림 3-4) : 펄스의 전력 스펙트럼 표현과 전송 대역폭                                   120
（그림 3-5) 시간 영역의 전송속도와 주파수 영역의 대역폭                                   122
（그림 3-6) 확산 변조된 정보 Bit의 형태                                          123
（그림 3-7) 확산 변조와 병행된 BPSI( 변조신호의 전송과 복조                              123
（그림 3-8) 잡음신호의 수학적 표현                                               124
（그림 3-9) 확률 분포 함수와 확률                                               126
（그림 3-10) 什ocessing Gain의 설명                                        127
（그림 3-11) 기존의 통신방식                                                  130
（그림 3-12) 확산 스펙트럼 방식                                                130
（그림 3-13) Jamming과 Pr（兀essing Gain과의 전투                             137
（그림 3-14) Fundan祀ntal Channel과 IS-95B의 Suppleme砒a! Code Channel · · 140
（그림 3-15) 인접기지국으로부터의 간섭                                             149
（그림 斗16) 불균등한 기지국 부하                                                150
（그림 3-17) LFSR의 구성                                                 156
（그림 3-18) 다항식 의 LFSR 표현                                            157
（그림 3-19) LFSR의 상태천이                                               158
（그림 3-20) 대수적 표현                                                   158
（그림 3-21) 시퀀스의 대수표현                                                159
                                                     19
                                                           I
（그림 3-22) 다항식 의 상태천이                                      160
（그림 3-23) 최장코드의 구성                                        164
（그림 3-24) 최장 코드의 정규화된 주기적인 자기상관함수                         167
（그림 3-25) 자기상관의 종류                                        168
（그림 3-26) 분할에 의한 시퀀스의 생성                                  170
（그림 3-27) Hadam可d 八4atri（의 확장                             173
（그림 3-28) OVSF 와 Hadam可d 방식의 비교                           174
（그림 3-29) Gold Code의 발생                                   175
（그림 4-1) DSSS 시스템에서 쓰이는 PN Code 동기장치의 일반적인 형태             178
(그림 4-2) MSM Demodulating Functional Block Diagram        179
（그림 午3) Double Dwell PN 동기 획득 시스템                         180
(그림 4-4) Double Dwell Algorithm                           182
（그림 千5) Searcher Engine                                   183
（그림 午6) Searcher 통작 흐름도                                   184
(그림 4-7) Non Coherent Energy Detection                    187
（그림 午8) Se可ch Block I万agram                               1羽
（그림 午9) PN Code 발생기                                       190
（그림 午10) 상관기                                              191
（그림 午11) CTRK 블록                                          192
（그림 十12) ACQ_CHI( 미ock Diagram                            193
（그림 午13) INC 미ock I万agram                                 194
（그림 午14) SLEW/ 블록도                                        194
（그림 午15) 프로세스 정합 신호 Timing                                195
（그림 午16) MCS 블록도                                          197
（그림 午17) Jumping Slew 및 1/2 칩 Slew 동작도                    197
（그림 +18) Finger Dem（月ula的r                                198
（그림 十19) 주파수 에러 측정과 주파수 오차                                200
（그림 十20) Early小Late Tracking Loop의 구분                     201
（그림 士21) Phase와 Frequency Error                           203
（그림 午22) 기본적인 Phase Lock Lc叩                              203
（그림 午23) PLL 내부 파형                                        204
（그림 士24) 주파수 스텝 입력어］ 대한 PLL의 동작                           2（万
（그림 千25) 기본적인 Delay Lock Lc야）                             206
（그림 十26) DLL Tracking system의 분석 여］                       2(石
（그림 午27) 추정오차어］ 의한 Error신호의 자기상관도                         208
（그림 午28) 士1/2 칩 Early-Late 옵셋일 때 오차신호의 자기상관도              209
（그림 午29) Non Coherent DLL의 Envel야光 Correlation            210
                                                      차 례
                                                            .

（그림 午30) Non Coherent Early-Late Tau-Dither Loop 해석     211
（그림 午31) Deskewer블록의 동작 타이밍                             214
（그림 午32) 심벌 결합기가 Deskewer bu卄er를 읽는 타이밍                 215
（그림 午33) Slam Operati아I 이 일어날 때의 타이밍                    216
（그림 午34) 심벌 결합기가 Fir增er를 추적하는 T如ing                     218
（그림 午35) 상태도                .                           222
（그림 午36) Searching 砥／indow틀                             222
（그림 午37) Detect state                                   223
（그림 十39) Verify State                                   224
（그림 午38) Dwell State                                    225
（그림 午40) Pull小In State                                  226
（그림 5-1) 전력제어의 개요                                       231
（그림 5-2) 이상적인 전력제어                                      232
(그림 5-3) Access Attempt2f Access Probe                  239
（그림 5-4) Open Loop와 Closed Loop의 연계                     242
(그림 5-5) Interference Correction                        243
（그림 5-6) RC1인 경우의 전력제어 Sub채널                            246
（그림 5-7) RC2인 경우의 전력제어 Sub채널                            247
（그림 5-8) Reverse 전력제어 부채널                               249
（그림 5-9) Timing                                         251
（그림 5-10) Reverse CD八/11\ 채널 가변 데이터 율 전송                253
（그림 5-11) Forward Reverse 전력제어 부채널 전송 timing            254
（그림 5-12) 전력제어 Bit의 위치 결정RC1                            255
（그림 5-13) PCB의 시작위치의 랜덤화-RC4(non-TD)                    257
（그림 5-14) 전력제어 Bit의 다중화                                 258
（그림 5-15) 전력제어 Bit의 결정                                  259
（그림 5-16) CSM 미ock I玉agram                              260
（그림 5-17) 전력제어 Bit 결정 시점                                262
（그림 千18) PWR_REPJJELAY의 개넘도                             264
(그림 5-19) Modulator                                     269
（그림 5-20) E1B의 전송                                       274
（그림 5-21) Outer Loop Power Control의 개념도                 275
（그림 5-22) 외부 Loop 전력제어 상태천이도                            277
（그림 5-23) OUTLO아乙START State flow Cha比                  278
(그림 5-24) OUTLOOP_FUL_RATE_RLJN state Flow Chart        279
(그림 5-25) OUTLOOP_II)LE state Flow Cha比                 280
（그림 6-1) 단말기의 Pilot Set의 분류                             289
 口
     차 례
                                                  21
                                                        I
（그림 价2) 乂Y에서 Soft Handoff가 일어나기 위한 SRCH小WIFLA          291
（그림 6-3) 1万I毗 PN Set 검색                                294
（그림 6-4) Handoff의 신호세기 및 시간 여유 Hys扼resis 형태            297
（그림 6-5) Pilot Set 분류를 위한 P11야의 일생（H生）                 302
（그림 6-6) Active Set어］ 할당되기 위한 조건                       302
（그림 6-7) Pu毗 Phase계산                                   303
 (그림 6-8) Pilot Strength Measurement Message           304
 (그림 6-9) Extended Handoff Direction Message           305
 (그림 6-10) Handoff Completion Message                  307
（그림 6-11) Handoff 처리과정                                 307
(그림 6-12) Neighbor list update Message                 3月
（그림 6-13) Handoff 절차 비교                                310
（그림 6-14) New Algori仕Em                                311
（그림 6-15) IS-95A의 Set 관리                               313
（그림 6-16) IS-95B의 Set 관리                               313
（그림 什17) Fast Rising Pilot의 효과                         314
（그림 臼18) Dyn꾜1, fl, 의 상관관계                             315
（그림 6-19) Active Set의 가장 강한 Pilot의 EC/J0               317
（그림 6-20) 서로 다른 FA간 Hando卄의 예                          319
（그림 6-21) Round Trip Delay 방식                          320
（그림 6-22) Dummy P11야 방식                                321
（그림 6-23) Dummy Pilot 과 Handoff 경계                     321
（그림 6-24) RC간 Handoff                                  322
（그림 6-25) 다른 주파수의 방문                                   327
（그림 臼26) 유휴 Han面付의 여］                                  341
(그림 6-27) System Access Diagram                        345
（그림 6-28) ACCESS_Ho_LIST와 OTHER_REPORTEI工LIST발생        348
（그림 6-29) Access I노obe어］서 Pilot Report                 349
(그림 6-30) Access Handoff Timeline                      349
(그림 6-31) Access Entry Handoff Flow Chart              3印
（그림 6-32) Access Handoff Flo＼入／ Cha此                   353
（그림 6-33) 단말기 상태별 Handoff                              358
（그림 7-i) Enc어五ng의 원리                                   361
（그림 7-2) Burst Error                                   362
（그림 7-3) Convolutional 부호화기（R=1/2,K=3)                 363
(그림 7-4) Trellis Diagram                               364
(그림 7-5) Viterbi Algorithm                             367
     22                                                       차 례
                                                                    .


（그림 7-6) 코드율 r=1/2인 Convolutional 부호화기                            368
（그림 7-7) 코드율 r=1/3인 Convolutional 부호화기                            369
（그림 7-8) 코드율 r=1/3인 Convolutional 부호화기                            370
（그림 7-9) 데이터의 Repeatation                                         372
（그림 7-10) 터보 부호화기                                                 374
（그림 7-11) 궤환 복호화기 ..                                              376
（그림 7-12) IS-95C의 Turbo Code                                      377
（그림 7-13) ASK, FSK, PSK 변조의 파형 비교                                 383
（그림 7-14) 다앙한 PSI떠 위상 표시                                          384
（그림 7-15) QPSI( 블록도                                               386
（그림 7-16) : QPSI( 변조신호                                            386
（그림 7-17) OQPSK의 블록도                                              388
（그림 7그8) OQPSK 변조신호                                               388
（그림 7-19) 위상천이도                                                   389
（그림 7-20) For＼丙／町d의 QPSK/BPSK                                     389
（그림 7-21) 다중화와 확산                                                 394
（그림 7-22) CDMA For／缸d 채널                                          395
（그림 7-23) Pil毗 채널의 구조도                                            397
（그림 7-24) 동기채널 형성                                                 399
（그림 7-25) 동기채널 구조                                                 400
（그림 7-26) 호출채널 형성                                                 401
（그림 7-27) 호출채널 Long Code mask                                     401
（그림 7-28) 호출채널 구조                                                 402
（그림 7-29) RC1의 Forw可（I 통화채널 형성                                    404
（그림 7-30) RC 3의 Fundamental Channel과 Supplemental Channel의 형성     405
（그림 7-31) 八4odulator(I, Q 八4apping)                               406
（그림 7-32) CDMA Reverse의 논리 채널들                                    407
（그림 7-33) Access 채널 형성                                            408
（그림 下34) Access 채널 구조                                             409
（그림 7-35) Randomization delay후 전송되는 /\ccess 채널 八4essage           410
（그림 7-36) Access 채널 긴 코드 마스크                                      411
（그림 7-37) RC1/2의 통화채널 구성                                          412
(그림 7-38) RC 3의 Reverse Fundamental Channel4 Supplemental Channe1의
          구성                                                      413
（그림 7-39) Reverse 전력제어 부채널과 Pilot 채널                              414
（그림 7-40) Reverse 프리엠블                                            414
（그림 7-41) Reverse 변조                                              415
    차 례                                  23
1

（그림 斗1) 단말기 초기화 과정                            418
（그림 斗2) 동기채널                                  422
（그림 斗3) 단말기 내부 타이밍                            423
（그림 斗4) Forw可d CDMA 채널 Pilot PN 옵셋            425
（그림 &5) 호출 Si毗의 구성                            426
（그림 &6) 다중 Si毗 방송 메시지 전송                      437
（그림 &7) Periodic Broadcast 호출의 여］             438
（그림 斗8) Quick 호출채널 구조                         440
（그림 斗9) 대기상태 정리                               445
（그림 斗10) 단말기의 Random Access                   447
（그림 斗11) Access Probe의 구성과 랜덤화                448
（그림 斗12) Request와 Resp아始e 경우의 /\ccess         450
（그림 斗13.1) Access 절차 여］ 1                     453
（그림 斗13.2) Access 절차 여］ 2                     454
（그림 斗14) Access 채널 긴 코드 마스크                   455
（그림 斗15) 개인Long Code 入4ask 형태                 456
（그림 斗16) System Access 상태 천이도                 457
（그림 斗17) System Access 상태 정리                  462
(그림 8-18) Service Option Number Format        464
（그림 斗19) 통화채널의 부 상태                           475
（그림 斗20) 시간정렬                                 477
（그림 斗21) IMSI의 구조                             479
（그림 斗22) IMSI_S 이진 Mapping                    479
（그림 斗23) SSD의 구성                              485
（그림 斗24) SSD계산                                486
（그림 斗25) AUTHES계산                             486
（그림 斗26) SSD Update 入4essage Flow             487
（그림 斗27) 단말기 등록 인증을 위한 AUTHR계산                488
（그림 斗28) 유일시도 응답을 위한 AUTHIJ계산                 489
（그림 斗29) 단말기 발호인증을 위한 /WTHR 계산                490
（그림 斗30) 단말기 착 호 인증을 위한 /\IJTHR 계산            491
（그림 9-1) 음성의 부호화와 복호화                         507
（그림 9-2) 사람의 발성 기관                            508
（그림 9-3) 공기의 흐름과 성대의 동작                       509
（그림 9-4) 소리의 합성／분석                            510
（그림 9-5) Bit 할당                               512
（그림 9-6) QCELP DeCoder의 구조                    513
                          차 례
   24                           1


（그림 9-7) 격자형 분석 필터          518
（그림 9-8) 격자형 합성필터           520
（그림 9-9) 원음성 파형             521
（그림 9-10) 예측 잔차             522
（그림 9-11) 잔차 신호의 모델화        522
（그림 9-12) 성대에서의 공기 펄스 열     523
（그림 9-13) Pitch탐색           525
（그림 9-14) Codebook 탐색       527
（그림 9-15) QCELP의 구조         532
    l. 이동통신 방식                                         25
=                                                  [




 인간은 태초부터 감각적, 시각적, 청각적 언어의 전달을 통하1 의사전달을 수행해
왔다. 인류가 정보를 기호화하는 수단을 갖게 된 이후 종이의 발명은 정보를 기록하
고 전달하는 중요한 매체로서 정보전달 및 저장의 정확도를 증대시켜 정보의 대량
복제가 가능해졌다．
 정보를 원격지어］ 전송하고자 하는 노력은 우리나라의 경우 봉화를 통해 기호화하
여 조직적인 정보전달을 시도한 예를 찾아볼 수 있다. 그러나 정보전달 속도가 획기
적으로 발전하게 퇸 것은 전기통신의 등장과 1835년에 발명된 사무엘 모르스
(Samuel F.B.M야se）의 유선 전신기가 실용화되면서부터라고 해도 과언이 아닐 것
이다. 그 후 전신망의 형성은 사람의 목소리를 저장하였다가 재생하1 주는 에디슨
(Thomas A. Edison）의 축음기의 발명과 1876년어］ 벨（Alexander Graham Bell）어］
의한 전화기의 발명으로 통신시대의 서막이 오르기 시작했다．
 전기신호를 이용한 초기의 통신은 1:1의 통신에서 댜다의 통신이 됨으로 통신의
일반화가 이루어졌으며, 이러한 통신은 통신 시스템이라는 개념이 필요하게 되었으
며, 이러한 통신 시스템의 핵심에는 Switching기능과 Routing기능을 하는 교환기
     26                                            ] . 이동통신 방식
                                                                 .


가 발명되기어］ 이른다. Sw抗ching이란 사용자의 가입자 라인（Local loop）을 연결할
것인가 아닌가어］ 대한 ON, OFF기능을 한다는 관점에서 Switch라 할 수 있고, 여
러 가입들의 연결을 위한 기능을 Ho岫ng이라고 한다．




                                                          L




                 （그림 ]-1) 일반적인 유／무선 통신 시스템


  이러한 교환 시스템에서 일반 가입자의 연결고리가 있을 것인데 이것을 우리는
가입자 라인（Subscribe Line）이라고도 하고 Local loop라고도 이야기한다. WLL이
란 玖／ireless Local Loop를 나타내는 말로서 Local Loop를 무선으로 사용한다는
것이다. 이것은 미국과 같이 광범위한 영토를 가진 국가에서 유선 케이블의 설치의
불편함과 비용 측면에서 처음으로 제안되었텬 것이다. （그림 卜1）은 이러한 통신 시
스템의 개요를 보여준다．
 유선전화는 교환 시스템과 유선으로 연결되며, 무선전화기는 무선으로 연결되어
있다. 즉 교환 시스템과 연결되는 연결점의 입장에서만 본다면 무선통신의 경우 넓
은 의미로는 BTS(Basestation Transceiver Subsystem)와 BSC(Base Station
Controller), BSS(Base Station System)를 포함한 영역을 Local Loop로 해석할
수 있다．
 또한 PCS망이든 셀룰러 망이튼（사실 PCS와 셈룰러로 대변되는 011의 차이는 아
무것도 없으며, 단지 RF주차수 대역이 차이가 나는 것이다．) 무선통신이라고는 하
    1 . 이동통신 방식                          27
口


지만 기지국과 단말기까지의 전송로만이 유일하게 무선 구간이고 나머지는 모두 유
선 구간이라 할 수 있다. 따라서 정보의 흐름 측면에서 볼 때 거의 대부분의 경로가
무선경로가 아닌 유선경로인 것을 알 수 있다. 일반적으로 기지국에서 신호를 중계
선을 통해서 전송하는 전송라인은 Ti, El급의 전송로를 사용하며, 그 상위 단에서
는 좀더 넓은 대역의 중계선로를 사용할 것이다．
 또한 이러한 통신은 단말기의 위치가 고정되어 있는 고정통신에서 이동통신으로
발전을 하게 되면서 이동성 관리라는 새로운 기능을 하는 시스템이 필요하게 되어
통신 시스템은 더욱 복잡하게 퇸다. 이와 더불어서 이동통신은 그것의 통신방식이
전송하는 신호의 형태가 아날로그에서 디지털화하여 전송하는 디지털 통신으로 발
전하게 되었으며, 독립퇸 커버리지를 가지는 셀이라는 영역으로 전지역을 나누어서
서비스하는 셀룰러의 형태로 발전하였다．
 통신의 발전사를 이동성의 입장에서 본다면 지금 현재의 이동통신의 서비스가 향
후 어떻게 진행될지를 나름대로 생각하1 볼 수 있다. 초창기의 전화기는 특정한 위치
에 고정되어 있으며, 한 동네어］ 하나씩 혹은 좀더 발전하여 한 집어］ 하나씩이라는
개념의 고정퇸 전화였다. 이러한 전화는 사람들에게 전화를 하기 위해서는 전화기
가 위치하고 있는 곳으로 가야 한다는 생각을 가지게 되었으며, 이때는 고정된 전화
기로 사람들이 이동해야 한다는 특징이 있다. 이러한 전화기의 특징은 좀더 발전된
전화기의 형태인 무선전화기에서도 마찬가지였으며, 단지 무선전화기에서는 전화기
로 이동해 가는 사람들이 전화기가 있는 '바로' 그곳으로 이동하햐 하는 번거로움
대신어］ 전화기 근처로 이동하면 퇸다는 생각을 하게 하였을 뿐 이것 역시 전화기는
상전（2）일 수밖에 없었다．
 이후에 셀룰러 이동통신 기술의 발달로 이동 전화기라는 개념이 생기면서 더 이
상 전화기가 가정어］ 하나씩 혹은 동네어］ 하나씩 있는 공공의 소유의 형태가 아니라
개인별로 하나씩 가질 수 있는 개인 소유 전화기의 개념으로 바뀌게 되었다. 따라서
사람들은 전화를 하기 위하써 전화기가 있는 곳으로 이동하1 간다는 의식은 점차 사
라지게 되었으며, 이때부터 전화기를 사용하는 사람의 이동성은 더욱 자유롭게 되
었다. 따라서 그 사람의 전화가 있는 곳에는 그 사람이 있다라는 식으로 전화기의
이동성이 사람의 이동성과 동일하게 취급되게 되었다. 이러한 형태의 서비스가 지
금 현재 서비스되고 있는 휴대전화 서비스인 것이다．
    그러나 이러한 서비스에서도 사람들은 전화를 하기 위해서는 여전히 전화기를 가
   28                                                      1. 이동통신 방식
                                                                        U


지고 다녀야 된다는 점에서 이러한 서비스는 사용자의 이동이라기보다는 전화기의
이동이라고 생각하햐 할 것이다. 단말기의 이동성이 아니라 전화기의 이동성이 강
조된 시스템이라고 볼 수 있다．
 최근에는 스마트 카드 혹은 ST八4(Subscriber Identity Module) 카드 등과 같은
것들이 개발되어서 더 이상 단말 이동형의 이동전화 서비스를 개인 이동성을 더욱
발전시킨 형태로 발전하고 있다. 즉 사용자는 자기 자신의 개인정보가 담겨져 있는
마이크로칩이 내장퇸 카드를 가지고 다니면서（전화기는 필요 없음） 전화를 걸고 싶
을 때에는 어떠한 전화기（기계）를 사용해서 자신의 7냔三를 전화기에 삽입하써 마치
자신의 전화기와 같이 사용하는 것이다. 이렇게 되면 사람들은 전화를 하기 위해서
전화기를 반드시 항상 가지고 다닐 필요가 없어지는 것이다. 사용자가 사무실어］ 있
을 때에는 사무실에 있는 전화기계가 그 사람의 전화기가 되는 것이고, 집에서는 집
에 있는 기계가 역시 그 사람의 휴대 전화기가 되는 것이다. 물론 자동차 안에서도
자동차의 휴대 전화기가 그 사람의 휴대 전화기가 되는 것이다. 이제서야 사용자의
이동성이 어느 정도 중심이 된 듯하다．


                                 ＼나1


                        1李 + +
                                                  ＼
                                              丘
                                          鞏
                                 4 m1
                                      ?
                                  \
                             /



          고정형          단말 이동형                         개인 이동형


                （그림 卜2) 단말기 이동성의 발달


（그림 卜2）는 탄말기의 이동성을 정리해서 보여 준다. 특히 개인 이동형의 경우
여러 개의 단말기를 여러 명이 사용할 수 있다는 것을 다시 확인할 수 있다. 이러한
     ] . 이동통신 방식                                                     29
口


예로는 친구의 사무실을 방문했을 때 그 방문지에서 전화를 하고자 할 때 그 친구의
전화기를 잠시 빌려서 자신의 카드를 삽입하여 자기의 전화기같이 사용할 수 있는
경우를 말하는 것이다．




  대표적인 이동통신 서비스는 무선호출（Pager）부터 발전하囚 오늘날의 PcS
(Personal Communication System), 나아가서 IMT-2000(Intemational 八/1아血e
Telecommunication-2000）까지 발전하게 되었다. 이러한 이동전화의 발전 선상어］
서 무선전화（CT), 주파수 공용통신（TRS), 휴대용 전화 및 PCS에 대해서 공부하겠
다．
      1.1.1 무선전화（CT : Codeless Telephone)

 일반 전화기는 전화회선을 통하여 음성신호를 전달하나 무선전화는 전화기 몸체
와 전화기를 무선으로 연결하여 음성을 전달하는 전화이며 제한된 반경 내에서 이
동성을 확보한 것이다. 즉 무선전화기의 본체가 소형 기지국과 같은 형태로 제공된
다고 볼 수 있다．
  이러한 무선전화는 옥내에서 한정하여 사용하는 CT-i과 과거어］ 삐삐 이후어］ 서
 비스되었던 시티폰과 같이 개인이 옥내외의 공공 장소에서 발신 전용 무선전화로 사
 용할 수 있는 CT-2가 있으며, 이 기능어］ 추가된 무선호출의 기능이 더해진 CT그＋
 와 교환기를 이용하여 수신된 전화를 바로 연결하는 서비스 기술까지 개발되었다.



                가정（옥내）용
                8 channels
              - FDMAJFDD                          Ilandoff
              1 아나로그                            叫 착발신기능
                90（呱1Hz대                        m 음성의 암호화
                                                - Data Application
                               m 옥내외 공공장소
                                                  TI꾜出A/TDD
                                            .
                               m 발신기농（휴대공중전화＼
                                                m 디지털
                               e 이용요금저렴
                               m 보행자중심의 대중성
                               山 FDMA/TDD
                               m 口시털


                             （그림 卜3) 무선전화의 발전
   30                                          ]. 이동통신 방식
                                                            1


 이러한 무선 전화기의 CT시리즈들은 지금 현재 서비스되고 있는 셀룰러 이동통
신이나 pCs등과 갇은 서비스와 공통적인 것은 무선 인터페이스로 인해서 단말기의
위치가 이동할 수 있다는 것이나 차이가 나는 것은 이러한 이동성이 제한되었는가
그렇지 않은가의 문제이다. 즉 CT 시리즈는 이동성의 관리를 망에서 하지 않기 때
문어］ 발신어］ 대한 제한은 없으나 착신에는 제한퇸다．
 이러한 CT폰들은 이동전화의 발전 선상어］ 있는 과도기적인 시스템이라고 생각
할 수 있다. （그림 1-3）은 CT시리즈 폰들의 발전과 그것들의 기능을 나타낸다. 여
기에서 CT-i은 흔히 가정에서 볼 수 있는 가정용 무선전화를 말하며, CT-2는
1980년대 유럽에서 널리 사용되던 보행자용 이동전화 시스템으로 우리나라에서도
시티폰이라는 이름으로 일시적으로 서비스되기도 했다.


  1.1.2 주파수 공용통신 시스템（TRS : Trunked Radio System)

 주파수 공용 통신 시스템은 미국과 일본에서는 入/ICA小佃ti-Channel Access),
한국과 유럽어써뇹區勃Frunked Ra小. 鈿扼m）라고 한다· TRS란 다수의 가입
자가 다수의 주파수를 공용함으로써 주파수의 이용효율을 높일 목적으로 개발된 이
동통신이며, 기업활동어］ 주로 이용되는 서비스이다．
 국내에서는 38呱旺七대와 800llTz대가 할당되어 있으며 휴대용 전화보다 이용요
금이 싸고 사무실과 영업자간 온라인으로 연락이 되는 등 사업의 생산성 향상과 합
리화어］ 공헌하고 있다．
 TRS는 1개 기지국으로 加30Km를 담당하는 광역 셀 방식이며, 통신시간을 제
한함으로써 주파수 이용 효율을 향상시키려는 노력을 하고 있다. 이것은 휴대용 전
화가 셀 방식으로 주파수를 재이용함으로써 주파수 이용효율을 높이려는 것과는 비
교가 된다．
 또한 TRS와 무전기의 차이점은 （그림 卜4）와 같다. 즉 TRS는 무선자원을 관리
할 때 통합적으로 관리함으로써 필요 없이 비어 있는 채널을 없애고 채널을 모두
같이 사용할 수 있게 해주었다. 즉 호가 연결될 때 그 호의 시간을 제한하는 방법을
사용함으로 이러한 방법이 사용될 수 있다. 이것은 특정 자원이 특정 사람에게 항상
고정적으로 할당되지 않는다는 측면에서 마치 토지 공（公）개념과도 비슷한 개념이
라고 생각할 수 있다. 이러한 의미에서 TRS를 주파수 공용통신 시스템이라고 번역
한 것은 상당히 타당하다 하겠다.
    1. 이동통신 방식                                                                  31
.



                  무전기                           TRS




                                                                    0 0 0 0 0
         Busy    C乂） 1 e CH 1     0             -     0-
                                                            CII 1

         Busy        느
                       D CH Z聲 .                -,  .       CII 2

         Free        卜    CII 3
                                        (D (D (D 1+ 0       CH 3

         Free             CH 4                  -,  .       CH 4

         Busy      0 卜 e 二CH5 1                 1+ D        CH 5


                                      O통화대기 1        통화 중

                      （그림 卜4) T日S의 채널 이용 방법


    국내에서는 1992년 부산지역의 남쪽 6개 항만에 TRS 방식이 도입되어 현재 주
요 항구의 선박회사 또는 조합 사무실과 각 어선들이 80k皿이내의 근해에서 힌국
TRS어］ 의해 통화서비스를 받고 있으며, 아남 텔레콤 등 다수의 사업자가 서비스를
준비하고 있다. 또 경찰에서도 일부 지역에서 사용하고 있으며 소방, 의료 등 공공
기간과 석유, 전력, 컨설, 운수업체 등에서 서비스하고 있다. 가장 대표적인 것이 요
즘 유행하는 퀵서비스에서 많이 사용하고 있다．
    주파수 공용 통신 시스템의 시스템 구성은 다음의 （그림 卜5）와 같다．




                   （그림 卜5) 주파수 공용통신 시스템의 구성
   32                                 ]. 이동통신 방식
                                                   U




 1.2 셀푿러 이동통신                                      )


 통신 시스템은 발전어］ 발전을 거듭해 오면서 언제 어디서나 누구와도 통화할 수
있는 형태의 요구어］ 의해서 이동통신이 발명되었고 이러한 이동통신은 많은 사람이
사용하기를 원했고 또한 다양하고 복잡한, 즉 더 많은 정보를 교환하기를 원하는 요
구어］ 의해서 그저 막연하게나마 무한정이라고 생각했던 전자파라는 것이 여러 가지
이유로 인해서 무한하지 않고 사용상어］ 제한이 되는 자원이라는 다소 겸손한 인식
을 하게 된다（기술적인 상황어］ 의해서 무한하지 않다는 이야기도 될 수 있다）.
 이러한 생각에서 사람들의 고민의 방향은 이제 어떻게 하면 더 많은 자원을 사용
할 수 있을까라는 생각을 하게 되었을 것이다. 그리고 그러한 고민을 하던 중 독립
된 공간에서 사용하던 자원을 또 다른 독립된 공간에서 사용할 수 있을 것이라는
생각을 하게 되었다. 예를 들어서, 미국에서 사용하는 주파수 대역을 힌국에서 사용
한들 어떠한 문제도 발생하지 않는다는 것과 같다. 즉 미국에서 사용하는 주파수 대
역의 신호가 너무나 미약한 신호가 되어서 한국에는 유효하게 영향을 끼치지 못하
기 때문이다．
 이와 비슷하게 특정한 지역에서 사용하는 신호의 출력이 엄격하게 통제된다면 일
정한 거리가 떨어진 지역에서는 또 다시 그 자원을 사용할 수 있다는 이야기가 된
다. 여기에서 설명하고 있는 이러한 독립된 공간을 셀이라고 하였고, 셀을 기반으로
하여 통신하는 방식을 셈룰러라고 한다．

  1.2.1 기지국과 셀

 이동통신은 사용자의 위치 혹은 단말기의 위치가 제한적인 혹은 고정적이었던 것
어］ 반해서 이동적이며 가변척이라는 면에서 동적인 통신이라고 할 수 있다. 이러한
단말기 혹은 가입자의 위치 이동이 자유롭다는 이유로 인해서 교환 시스템 혹은 통
신 시스템과 가입자 단말기간의 링크인 가입자 라인（Local Loop）이 무선으로 이루
어질 수밖어］ 없다．
 따라서 이동통신 기술의 새로운 관점이라면 무엇보다도 무선링크어］ 대한 정의일
것이며, 이러한 기술의 대표적인 것이 TIA月iIA在S-95와 같은 무선 인터페이스 규
격이다. 이 절에서는 셀어］ 대한 이야기어］ 초점을 맞추어서 이야기하고 다음 절에서
pcs시스템을 공부할 때 전반적인 이동통신 시스템어］ 대해서 공부하도록 하자．
    1. 이동통신 방식                                比
1


    가장 고전적인 셀룰러 무선통신 방식의 예는 방송 서비스라고 이야기할 수 있다．
KBS의 방송국에서 남산어］ 커다란 송신탑을 세워서 아주 강한 출력으로 방송신호
를 송출하는 방식이 지금 현재 서비스되고 있는 TV혹은 라디오 방송 서비스의 방
법이다. 전자파는 발산하는 속성이 있는 물리량으로 거리어］ n승에（자유공간에서는
2, 일반적인 도심에서는 4정도임） 반비례하여 그것의 필드를 형성하1 간다. 따라서
송신탑에서 송출되는 신호는 모든 신호가 LOS(Line Of Sight）통신이 퇸다면 거리
어］ 의한 감쇠어］ 의해서 그것의 신호의 영향이 끼치는 데는 모두가 시청권이 된다.
즉 방송신호의 통화권이 된다. 이러한 통화권의 범위 밖에는 시청권이 되지 않을 뿐
아니라 만약 시청을 원한다면 송신탑의 출력을 높이든지 새로운 송신탑을 세우면
된다. 즉 남산에서 출력하는 송신탑의 출력어］ 의해서 형성되는 통화권 혹은 셀의 크
기를 크거］ 하든지 새로운 통화권 혹은 셀을 만드는 방법이 있을 수 있다．




                 （그림 卜6) 셀의 크기와 전장의 균일성


    서울 시내 전역을 무선 이동통신 통화권으로 설정하기 위한 방법을 생각하1 보자．
우선 서울의 중심부에 가장 높은 지점에（대략 남산이 될 것이다） 송신탑을 세워서
서울의 가장 외곽지인 광명, 구리 등지에서는 통화가 되지 않을 정도로 출력을 조정
해서 신호를 송출하는 방법이 있을 것이다. 그런데 이 방법에서는 셀의 가장 자리어］
충분한 세기의 신호의 강도가 될 수 있게 하기 위해서 출력을 조절하다 보니 송신탑
근처에서는 상당히 큰 전자파 필드가 형성될 것이다. 이것은 셀 전체로 볼 때 （그림
卜6）과 같이 전장의 분포가 균등하지 못한 결과를 가져온다．
    또한 이러한 형태는 각각의 단말장치에서 Access가 필요로 한 통신 시스템에서
   34                                      ] . 이동통신 방식
                                                         U


는 상당한 문제가 있다. 방송에서는 방송국에서 각각의 단말장치（TV나 라디오）로
일방적으로 정보가 제공되므로 문제가 없을 수 있으나 통신 시스템에서는 각각의
단말도 주체적으로 망에 /\ccess를 하는 링크, 즉 Reverse Link어］ 대한 문제로 인
해서 문제가 될 수 있다. 즉 통화권의 균형인데 정보를 통신 시스템에서 단말로 내
려보내 주는 Forw可d Link와 Reverse 링크가 균형이 이루어져야 한다. 즉
Reverse 통화권과 Forw可d 통화권이 균형을 이루어야 한다는 것이다. 통화권을 하
나의 송신탑（기지국）으로 아주 넓은 지역을 형성하게 되면 단말장치의 출력 또한
상대적으로 상당히 커야 한다는 이야기이다. 참고로 위성통신에서는 위성에서 지구
국으로 내려오는 정보 링크를 Down Link라고 이야기하며, 올라가는 정보링크를
Up Lii永라고도 이야기한다.
 탄말기의 출력이 커야 한다는 것은 단말기의 크기가 커져야 한다는 것과 같이 생
각되어야 할 부분이다. 일반적으로 이동통신이라 할 때 이동성을 생각하게 되는데
지금의 그것보다 상당히 큰 형태의 단말기를 생각할 때 과연 그것의 휴대성이 용이
할지의 문제를 생각할 때 단말기의 크기와 이동의 용이함이 맞물려 있고 단말기의
크기와 셀의 크기와도 연관되어 있다고 할 때 이동통신에서 사용하게 될 셀의 크기
는 방송국에서 사용하는 형태는 타당하지 않다는 것이다．
 이와는 구별되게 수년 전어］ 유행했던 Pager 혹은 삐삐의 경우 양방향 통신형태의
서비스가 아니라 방송의 서비스와 유사하다는 측면에서 그것의 셀이 이동통신의 셀
의 형태보다는 방송국의 셀의 형태와 더욱 닮아 있다는 것을 확인할 수 있다．

 셸의 크기와 사용자 수
 우리가 통신 시스템에서 처리할 수 있는 용량을 셀 단위로 생각할 때 셀의 크기
가 작을수록 단위 면적당 셀의 개수는 많아질 것이며, 따라서 단위 셀당 사용자 수
도 증가하계 될 것이다. 그러나 여기에서 중요한 것은 셀간의 상호작용이다. 셀간어］
완전한 독립이 보장된다면 이러한 가정들은 만족하게 될 것이다. 이렇게 셀간어］ 서
로 상관성이 없도록 하기 위한 방법 중 하나는 주어진 자원을 나누어주는 것이다．
각각의 자원, 즉 채널은 서로칸에 구별되어지는 것들이며, 이러한 채널들은 나누어
가지는 것이다．
 예를 들어서 특정 지역어］ 주어진 채널이 100개라고 할 때 이러한 채널을 하나의
거대한 셀에서 모두 사용하는 방법이 있을 수 있을 것이나 그 지역어］ 셀을 작게 나
    ] . 이동통신 방식                             35
.


누어 작은 셀10개어］ 10개씩 나누어준다 해도 별반 달라지는 것은 없을 것이다. 그러
나 다음 절에서 이야기할 주파수 재사용 부분에서는 이러한 것이 달라지는 어떠한
장점이 있음을 알 수 있다. 어찌되었든 이러한 시도는 단순히 자원을 배분한다는 것
어］ 불가하다. 다시 셀간의 독립적인 이야기를 하게 된다면 셀간의 통화권에 대한 경
계를 확실하게 하는 것이다. 그것은 기지국의 출력의 세기를 조정해서 할 수도 있고
사용하는 주파수 자원의 구분을 엄격하게 하는 것이 그것들이다.


    셀의 구분과 의미
    셈룰러에서 서비스 지역을 작은 셀로 나누고 셀 경계를 정하기 위해서 셀 모양을
정의해야 한다. 실제 서비스 지역이 완전한 평면이라면 셀 모양은 원형어］ 가깝다．
이것은 앞서 이야기되었듯이 셀은 통화권역을 의미한다고 할 수 있으며, 이런 통화
권역은 기지국의 출력어］ 의해서 특정한 통화품질을 낼 수 있는 공간상어］ 가상의 선
혹은 경계이기 때문어］ 발산하는 전자파의 경우 구형의 모습이 될 가능성이 크기 때
문이다．
    그러나 쉽게 생각 할 수 있는 원형의 셀은 평면적으로 배치할 수 없으므로 사용
하기가 곤란하므로, 평면적으로 배치할 수 있는 다각형 형태를 사용하여야 한다. 평
면으로 배치할 수 있는 다각형으로는 （그림 卜7）에서 보여 주는 바와 같이, 삼각형
과 사각형 그리고 육각형이 있다. 셀 모양으로 삼각형과 사각형 그리고 육각형 형태
의 셀을 비교하1 보면 육각형 형태의 셀이 중첩되는 영역이 가장 적으므로 가장 경제
적인 셀 배치를 할 수 있다．
    셀의 크기를 결정할 때 우리는 몇 가지 사항을 가정（정의）하고 해야 한다. 즉 어
디까지를 셀이라고 할 것인가이다. 다시 말하면 어디까지가 통화권역인가를 말하는
것이다. 이것은 서비스의 품질어］ 대한 기준이 있어야 한다. 기지국의 신호가 제대로
단말기어］ 수신이 되어서 전달하고자 하는 정보를 복원（복조, 복흐를 모두 포함） 가
능한지가 기준이 될 것이다. 이러한 기준은 단말기와 기지국의 변복조기를 비롯한
시스템의 성능과 아주 관계가 깊다. 예를 들어서 현재 우리나라에서 서비스되고 있
는 이동통신망어］서는 셀의 경계를 기지국의 신호가 약延玉如 전력이 형성되는
지점까지를 이야기하며， 이때 통화 攻聊理궂四갱흐엣j갰上超姓엣서 에러가 발생
하는 경향이 있는 상태를 말한다．
   36                                     ] . 이동통신 방식
                                                        .




        八


                  （그림 ] 7) 다양한 형태의 셀 배치


 따라서 셀을 설계하는 사람들은 이러한 생각을 가지고 머리 속어］ 그려져 있는 셀
들의 모양을 기지국의 출력을 조정하므로 만들어 가는 것이다. 이러한 셀들은 상호
작용을 하며, 때문어］ 이러한 셀들을 주변의 채널환경을 고려하여 셀을 배치하고 그
것의 크기를 적절하게 조절하는 것을 "Cell Planning"이라고 하는데 이것은 이동통
신에서 상당한 High Tech라고 할 수 있다. 이것을 위해서는 훌륭한 채널환경 데이
터베이스가 구축되어 있어야 할 것이다．

  1.2.2 주파수 재사용

 셀룰러 이동전화 시스템에서는 제한퇸 주파수 자원을 보다 효율적으로 사용하기
위하여 종래에 한 송신기가 한 반송 주파수로 서비스하던 넓은 지역을 작은 셀로
나누어 통신하는 방법이라고 공부했다. 또한 이러한 셀룰러 시스템은 단위면적당
채널수를 증가시키는 방법으로 셀 반경을 줄이는 것을 알았다. 이 절에서는 이것 외
어］ "주파수 재사용 계수"를 통한 셀룰러의 용량어］ 대해서 공부하자．
 주파수 재사용 계수란 셀룰러 시스템에서 주파수 효율이 얼마인지는 나타내는데
사용하는 Parameter로, 전체 주파수 대역을 사용하는 셀의 묶음으로 나누는 것을
말한다. 즉 주파수 재사용 계수 이상의 셀 혹은 그 이상 떨어진 셀에서는 동일한
대역에서 주파수의 간섭 없이 또 다시 통신을 할 수 있다는 것을 나타낸다. 이것은
셀 중간에 위치한 기지국이 저출력의 특정 주파수를 사용하여 서비스를 제공하도록
하되 일정 거리 이상 떨어진 다른 기지국에도 같은 주파수를 동시어］ 사용할 수 있게
하였다. 이렇게 주파수를 재사용함으로써 주파수 사용효을이 늘어나고 가입자 수용
용량도 상당히 증대되지만, 같은 반송 주파수를 셀룰러 시스템 내의 여러 기지국어］
서 동시어］ 사용하기 때문에 동일 채널 간섭이 발생하여 통화품질을 나쁘게 할 수
    ] . 이동통신 방식                                37
口


있a 口로 신중하게 고려되어야 한다．
 다음과 같은 경우를 한번 생각하1 보자. 여기어써 간단한 주파수 분할방식（FDMA)
을 가정하여 설명한다. 주어진 총주파수 대역폭이 3卜皿也이고, 각 통화채널어］ 할당
해야 하는 대역폭이 30KHz이라면, 총주파수 대역에서 얻을 수 있는 통화채녈수는
3000/30 = 100개가 퇸다 이 100개의 채널은 （그림 1-8）의 전지역에 할당되었는데，
이것을 지역을 A, B지역으로 나누어 서비스한다고 생각하1 보자. 그리고 각 지역의
중심부에 기지국을 세우고 출력을 한다고 할 때 각각의 지역어］ 100개씩의 채널을
할당하면 어떻게 되겠는가？ 당연히 통신이 잘 안 될 것이다. A지역에서 사용하는
채널을 B지역에서도 누군가 사용한다면 둘 사이에는 혼선이 생길 것이기 때문이다．




                  （그림 卜8) 셀룰러 서비스의 예


 이러한 문제를 극복하려면 각각의 지역어］ 채널자원을 골고루 나누어주어서 각각
50개씩 의 자원으로 출력을 하게 하면 될 것이다. 즉 각각의 지역의 통신로를 보장
하1 주어야 한다는 것이다. 즉 모튼 자원을 같이 사용하게 되면 나의 통화가 남의 간
섭이 되기 때문이다．
 이상과 같은 방법을 사용하면 A, B지역을 모두 합쳐서 하나의 기지국으로 서비
스할 때와 달라진게 있다면 기지국의 규모일 것이다. 즉 통합해서 서비스를 한다면
하나의 기지국의 규모가 커질 것이나 나누어진다면 작은 기지국으로 기지국 하나의
부담은 그만큼 덜하찔 것이다．
 그러나 이것이 전부는 아니다. 이제 우리는 새로운 생각을 해보자. （그림 1-9）와
같이 각각의 지역을 각각 7개의 작은 구역인 '셀'로 나눈 다음 주어진 총통화채널을
7개로 나누어서 각각의 셀어］ 100/7 늑 14개의 채널을 할당하면 （그림 卜9）와 같이
갇은 채널을 사용하는 구역이 각 셀의 반경어］ 비해서, 서로 멀리 떨어져 있으므로
   38                                   ] . 이동통신 방식
                                                      1


(A와 A ' 사이）, 서로의 간섭이 무시할 수 있을 정도로 작게 만들어 혼신의 염려가
없도록 한다. 즉 （그림 1-9）의 경우 A, B지역에서 사용하는 총채널 수는 200개가
되어 （그림 卜8）의 경우와 비교해 보면, 사용할 수 있는 채널이 두 배로 증가했음을
알 수 있다. 이렇게 서비스 구역을 잘게 나누면 수용용량이 증가함을 알 수 있다．
여기에서 중요한 것은 a과 a' 셀간의 간섭이다. 이러한 간섭이 무시할 수 있을 정도
로 약하다는 가정이 있어야 할 것이다．




            （그림 卜9) 셀룰러의 서비스할 따1 용량증가


 여기서 만일 셀 반경을 반으로 줄이면 셀 수는 4배로 증가하게 되고, 셀에 주파수
를 할당하는 방법을 그대로 적용하면, 각 셀당 14개의 통화채널을 그대로 각 셀에
할당할 수 있으므로, 전체 서비스 지역의 통화채널수도 역시 4배로 증가하게 된다．
이와 같이 셀 반경을 조절하여 통화채널 용량을 조절할 수 있으므로, 수요에 따라
셀 반경을 설정하여 가입자가 많아도 이를 수용할 수 있게 퇸다. 물론 무조컨 셀 반
경을 줄일 수 있는 것은 아니다. 시스템의 특성, 전파 환경 등어］ 의해서 줄일 수 있
는 한계가 있다. 또한 중요한 것으로 6장에서 공부하게 될 Handoff도 셀의 크기와
무관하지 않다. 초창기 Pcs의 경우 저속 보행자만을 대상으로 시스템을 설계할 때
만하더라도 그것의 셀의 크기는 피코 셀 이하의 나노 셀까지 이야기가 되었다. 이렇
거］ 작은 셀이 가능했으므로 가입자 용량이 많아지고 때문어］ 박리다매（薄利多賣）라
고 저렴한 통신 서비스를 할 수 있을 것이라고 하였으나 지금의 Pcs의 모양은 그
렇지가 않고 단순히 기존 통신 사업자의 경쟁사적인 성격만을 가지고 주파수 대역
의 차이만 있는 또 다른 형태의 마크로 셀의 셀룰러 시스템이다．
   이동통신 방식                                     39




      재사용 계수
 다음의 예를 통해서 재사용 계수어］ 대해서 좀더 생각해 보자. 주파수 재사용 계수
가 2, 4, 7인 경우어］ 대해서 주어진 통화채널이 100개인 망에서 셀당 할당할 수 있
는 통화채널 수를 계산해 보면, 재사용 계수가 3인 경우는 100/3= 33개, N= 4인
경우는 100/4 =25개, N=7인 경우 100/7=14개로, 주파수 재사용 계수가 작아질수록
각 셀에 배정할 수 있는 통화채널수가 많아진다는 것을 알 수 있다. 즉 가능하면 주
파수 재사용 계수를 작게 하면 셀당 할당할 수 있는 통화채널 수가 증가하여 단위
면적당 채널 수가 증가한다는 것을 알 수 있다．
 그러나 주파수 재사용 계수가 작아질수록 동일한 주파수를 사용하는 기지국간의
거리가 가까우므로 간섭성분이 강해져서 통신이 제대로 되지 않을 가능성 때문어］
주파수 재사용 계수를 무작정 작게 할 수는 없다．




   （그림 卜］0) 자원의 재사용 계수가 7일 때 같은 주파수를 사용하는 인접 셀


 또한 동일 채널 간섭은 같은 주파수를 사용하는 기지국간의 거리（D）인 주파수 재
사용 거리에 많은 영향을 준다. 동일 채널간의 간섭을 줄이기 위해 인접 기지국간어］
는 같은 주파수를 사용하지 않고 일정 거리 이상을 유지하면서 같은 주파수를 사용
할 수 있도록 기지국들은 배치한 것을 주파수 재사용 패턴이라 하며 다음 （그림
卜10）에서 7개 셀로 구성퇸 주파수 재사용 패턴을 보여 준다. 여기에서 이용 가능한
주파수 대역을 모두 할당한 기 지국들로 구성된 주파수 재사용 패턴의 한 단위를 클
    40                                                l . 이동통신 방식
                                                                    .



러스터（Cluster）라 하며, 클러스터 내의 셀 수를 주파수 재사용 계수（Fre恥ency
Reuse Factor : K）라 한다．




            (a) N=3        )b) N=4       （이 N= 7




           (d( N=3/ 9    (e ( N=4/ 12   (f( N=7/ 21


               （그림 ］너］) 주파수 사용계수에 따른 셀 클러스트


 여러 가지 경우의 주파수 재사용 계수를 갖는 셀 클러스터 모양을 （그림 卜11）어］
서 보여 주고 있다. 셀 모양을 정육각형으로 가정하여 셀 클러스터의 셀 수, 즉 주파
수 재사용 계수가 3, 4, 7인 경우에 대해서 전방향 셀（Ornt寸directional Cell)인 경
우와 3섹터 셀（Sec切red Ce피인 경우에 대해서 셀 클러스터의 셀 배치 모양을 보여
주고 있다. （그림 1-11）의 (a), (b), (c）는 전방향 셀어］ 대한 셀 배치 모양이고 (d),
(e), (f）는 섹터 셀인 경우의 셀 배치를 나타낸 것이다．
 여기서 전방향（Onini) 셀이란 기지국이 셀의 가운더］ 위치하여 수평 방향으로 360
도 전방향으로 전자파를 송신하는 안테나를 사용하여 서비스하는 셀을 말하며, 섹터
셀이란 기지국이 어떤 특정 방향으로 전자파를 송신하는 안테나를 사용하여 셀을 여
러 개의 섹터로 분할하여 각각의 섹티마다 서로 다른 안테나와 RF 장비를 사용하는
기지국으로, 전방향 셀어］ 비하여 간섭량을 줄여 줄 수 있어 CDMA와 같은 간섭 제
한 시스템에서는 용량증대에 기여할 수 있는 또 하나의 요인으로 고려될 수 있다．
 현재 사용중인 CDMA의 경우 각 섹터별로 서로 다른 옵셋을 사용하여 각각
A珀ha, Beta, Gamma sect아라고 하는 섹터 셀을 사용하고 있다．
     ] . 이동통신 방식                               41
.




    셸 반경과 주파수 재사용 거리
 주파수 재사용 계수어］ 따른 간섭량의 변화를 살펴보자. 먼저 육각형 형태의 전방
향 셀을 가정하면 셀 반경과 같은 주파수를 사용하는 셀 사이의 거리는 주파수 재사
용 계수의 함수임을 알 수 있다．
 （그림 卜12）에서는 한 클러스터어］ 7개의 셀이 있으므로 7개의 서로 다른 주파수
를 배치하게 된다. 이때 이 7개의 주파수는 인접 클러스터들에서 재사용되는데, 같
은 주파수를 사용하는 기지국은 한 기지국에서 오른쪽으로 i= 2 기지국, 위쪽으로
j= 1기지국만큼 떨어져서 위치하게 된다. 기지국의 최대 반경을 R이라고 하면, 인
접 기지국간의 직선거리는（3R이므로 같은 주파수를 사용하는 기지국간의 직선거
리, 즉 주파수 재사용 거리 D는 피타고라스 정리어］ 의해서 D2= SR2 (i2dj +j2)
인 관계가 성립한다汪한 주파수 재사용 계수K : i2 + ii +甘瞞斜r茹口로, 나d
주파수 재사용 거리 D, 지역반경 R, 그리고 주파수 재사용 계수 K사이에는 다음과
같은 관계가 있다. 이것은 주파수 재사용 계수가 1인 경우의 배수로 나타내는 이른
바 주파수 재사용 계수에 의한 정규화（normalize）라고 할 수 있다.


           D1R   Vi百                                (1-1)
                                                     =




                       7 cell cluster




                         （그림 卜］2) 주파수 재사용 패턴



     예를 들어서 셀 반경이 2km인 셀의 주파수 재사용 계수가 7인 경우 같은 주파수
    를 사용하는 셀과의 거리는 약 9.2km이라는 것이다. 이 이야기는 만약 시스템을 설
    42                                       ] . 이동통신 방식
                                                           1

계하는 설계자가 주파수 재사용 계수를 7로 가지고 가고자 할 때 일반적으로 기지
국의 출력이 자기 자신의 통화권역은 물론이고 최대 9.2Km밖에서는 신호가 발켠되
지 않게 되게끔 조정하여야 한다는 것이다．


 섹터 셀에서 주파수 재사용 거리
 시스템 성능어］ 영향을 주지 않으면서 동일 채널간섭을 더 줄일 수 있는 방법이
바로 기지국에서 전방향（OMNII玉rectional) 안테나 대신 지향성（Directional) 안테
나를 사용하는 섹터화（Sec的rization) 방식이다. 지향성 안테나를 사용하면 안테나
의 복사 방향어］ 있는 동일 채널의 기지국에만 주파수 간섭을 주기 때문어］ 그만큼
동일 채널간섭이 줄어들어 주파수 재사용효율이 증가한다．
 가장 흔하게 사용하는 섹터 셀로는 3 섹터 셀이며, 여기에서도 3섹티 셀을 기준으
로 주파수 재사용 계수어］ 따른 셀 사이의 간격을 공부해 보자．




          （그림 卜］3) 3 섹터 셀의 주파수 재사용 계수와 거리


 （그림 卜13）과 같이 3섹터 셀이 분포하고 있을 때, 같은 주파수를 사용하는 셀 사
이의 거리를 계산하1 보자. 각 주파수 재사용 계수에 따라 3섹터 셀의 셀 반경어］ 대
한 셀간 거리는 위의 수식을 적용하면 다음과 같다. 결국 셀읔 섹터화하면 셀의 재
사용 계수가 3배 더 커지는 효과가 있다는 것이 퇸다. 왜냐하면 결국 섹터 자체가
     ] . 이통통신 방식
.


주파수 성분의 제한적인 방사로 통화권을 제한하겠다는 의미이므로 이러한 관점어］
서 볼 때 셀의 형성 이유와 비슷하기 때문이다．
    따라서 다음의 결과와 같이 정리될 수 있다．


          k= 7       扼又7又3＝
                   DR＝    侮，
                                        .:7.   9
                                                   섹터화로 인한 주파


                       4而＝r“「‘
                   二V三긋 트
                               1
                                        1

                                                   수 재사용 계수의 새
          k= 4                                     로운 수정 요인．


          k=3 므＝.J3x3x
              K
                       3＝纛征5.2     1   d:




 여기에서 R은 셀의 반경이다. 이동통신 시스템에서 신호복구어］ 필요한 시스템（기
지국, 단말기）의 신호대 잡음비（C江 또는 Eb/N이를 작게 설계하여, 주파수 재사용
계수를 줄이는 것이 채널 용량 증가어］ 크게 기여할 수 있음을 알 수가 있다．
 실제 예를 들어 설명해 보면, 대개 디지털 방식의 셀룰러가 아날로그 방식 셀룰러
보다 용량이 크다고 하는데, 주어진 주파수 대역으로 제공할 수 있는 통화채널 수만
비교하1 보면, 앞에서 예를 다시 적용해 보면, 15 八4Hz 주파수 대역폭인 경우 아날로
그인 AMPS 시스템의 경우 통화채널 수가 500개이고, 디지털 방식인 GS八4은 600
개로, 총통화채널 수만 비교하면 용량 차이가 1.2배이다. 그러나 AMPS 시스템의
경우는 S/N비가 18dB 이어서 주파수 재사용 계수를 7을 적용하고 있고, GSM의
경우는 S/N비가 6dB로 주파수 재사용 계수를 4를 적용할 수 있다. 따라서 GSM
방식이 All冬 방식에 비해서 셀룰러 방식으로 통신할 때 용량이 2배 이상임을 알
수 있다．
 특히 새로운 무선접속 방식인 CDMA의 경우 이론적인 주파수 재사용 계수는 1
이고, 실제의 경우에도 1/0.6 정도이므로 다른 무선접속 방식（아날로그인 Alvil冬,
    TI呱4A 디지털 방식인 GS八4）에 비하여 각각 이론적으로는 주파수 재사용 졔수어］
    서만 아날로그어］ 비해서 4배, TDMA(Time I万Vision IM回tiple Access) 방식에 비
    해서 十2.4배 차이가 난다. 즉 CI巫IA(Code Division Multiple Access) 방식이
    다른 무선접속 방식어］ 비해서 채널 용량이 큰 가장 큰 이유가 CDMA의 주파수 재
    사용 계수에 있음을 알 수 있다. 즉 CI呱4A는 간섭을 제어하는 능력에（주파수 재사
    용 효율） 따라서 용량이 결정될 수 있는 셀룰러 통신방식에서 가장 효과적으로 용
           44                                                     ] . 이동통신 방식
                                                                                .


량을 확보할 수 있는 방법이라고 이야기할 수 있다. 이때 문제는 과연 CDMA방식
으로 통신할 때 기본적으로 스펙트럼 효율이 AMPS나 GSM정도가 되는지어］ 대해
서는 3장에서 좀더 자세하게 설명하겠다．
       이러한 셀룰러 방식에 대해서 각각의 경우를 예를 들면 미국의 AT&T에서는 7
셀 클러스터 방식과 기지국당 한 개의 안테나가 120도를 커버하도록 3개의 안테나
를 사용하는 3섹터방식을 사용하여, 이때 D/R(4.58정도이다. 한편 M毗oroh사에서
는 4개의 클러스터 방식과 기지국당 한 개의 안테나가 60도를 커버하도록 6개의 안
테나를 사용하는 6섹터 방식을 사용하는데, 이때 D/R(3.46정도가 된다. 즉 Motorola
사의 방식에서는 D/1이 AT&T사의 방식보다 작으므로 시스템 성능이 떨어질 수
있다. 그러나 M야町ola사는 섹터 공유 방식으로 시스템 성능 저하를 방지하고 있다．



       1.3 디지털 통신 개요                                                            )

       통신의 발전의 한 축에는 아날로그 통신에서 디지털 통신으로의 발전이 있다. 아
날로그 통신과 디지털 통신의 구분은 전달하고자 하는 정보의 형태가 아날로그의
형태로 가공이 되느냐 아니면 디지털의 형태로 가공되느냐어］ 따라서 나누어지게 된
다. 따라서 처리하는 과정에서 차이가 있으므로 용어에서도 그것들의 차이를 찾아
볼 수 있는데 디지털의 경우 정보를 가공하고 처리하는 과정에서 coding이라는 말
을 사용하며, 변조의 경우도 아날로그의 경우 변조라는 용어를 사용하나 디지털의
경우 의미는 비슷하나 전혀 다른 용어인 shift keyii培이라는 용어를 사용하기도 한
다（물론 QAM과 같은 경우는 변조라는 말을 사용한다）.
  이 두 가지 단어는 디지털통신의 의미를 잘 포함하고 있다．


       +    Source       =>   Channel
 <m나
            Coding   <        Coding


           PCM            Block Code               BPSK    CDMA
           ADPCM          - Hamming                QPSK    TDMA
           QCELP          - Reed-Solomon           OQPSK   FDMA
           EVRC           - Convolutional Code     GMSK
                             (Viterbi Algorithm)

                                （그림 ］너4) 디지털 통신의 개요
    ] . 이동통신 방식
                                                     기
                                                    45
1                                               !
    어찌 되었든 디지털 통신은 아날로그어］ 비해서 제어하기어］ 용이한 여러 가지의
장점들이 있다. 이러한 디지털 통신은 다음의 （그림 卜14）와 갇은 블록도로 정리할
수 있다. 각각의 블록은 서로 기능상 독립적이지만 블록간에는 상호간어］ 긴밀한 연
계가 필요하다．
    이 절에서는 （그림 1-14）의 각각의 블록을 중심으로 디지털 통신의 내용을 간단
하게 소개할 것이다. 이러한 내용을 설명하는 가운데 사용되는 예들은 그것의 내용
을 좀더 쉽게 이해하기 위해서 사용한 것이니 만큼 전반적인 내용을 알지 못하는
가운더］ 예문 자체를 확장하여 이야기하고 생각하는 것은 자칫 원래의 내용을 곡해
할 수 있기어］ 이러한 것은 정확하게 시스템을 이해하는 데에는 도움이 되지 않는
경우도 있을 수 있음을 미리 밝혀 둔다.


     1.3.1 Source Coding

    Source Coding은 디지털 통신에서 처음 행하는 단계로써 analog 신호를
Norm曲zed된 펄스로 곱해서, 즉 펄스 변조해서 아날로그 신호의 최대 주파수의 2
배의 빠르기로 순간 값들을 취한다（이러한 내용은 2장의 샘플링정리를 공부할 때 보
다 상세히 공부할 것이다）. 이것을 우리는 PAM(I뇨ise Amplitude 八4odulation) 신
호라고 한다. 지금까지가 Sou丁ce coding의 첫단계인 표본화이다. 이것을 디지털화
하기 위해서 특정한 레벨（보통 64kbps의 데이터 율일 경우 8 Bit, 즉 2의 8승 개의
레벨로 나눈다．
       ）로 나누어 2진수로 표시한다（양자화）. 일반적으로 Voice 통신 시스
템에서는 전송할 신호의 대역을 한 채널을 4k1七로 대역 제한한다. 따라서 4kHZ로
대역제한 샘플링하고 8 Bit로 양자화하면 64Kbps가 된다（4kH기吃X 8=r64kbp5).
    사실 모든 신호 성분들을 전송하기 위해서는 무한대의 대역폭이 필요하지만 그것
은 세상에서 1대 1의 통신이라면 가능하겠으며, 설사 그러하다 하더라도 무한대의
대역폭에서 동일한 응답 특성을 갖는 시스템 구현이 더더욱 비현실적이다. 샘플링
전단졔어囚 신호를 대역제한을 한다. 또한 사람의 귀가 느낄 수 있는 가청 대역폭이
제한되어 있으므로 이러한 무한대에 걸쳐 있는 모튼 고조파 성분들을 모두 전송한
다는 것은 사실상 아무런 의미가 없다．
    표본화 이론어］ 펄스 신호의 전송시어］ 적어도 main lobe에서 무간섭으로 전송하
기 위해서는 샘플링 주파수가 음성신호의 최고 주파수의 최소 2배이어야 한다. 따
라서 샘플링된 신호를 데이터의 표현 단위인 bps로 표현하면 8 kbps가 된다．
   46                                     1. 이동통신 방식
                                                       1


 이렇게 생성퇸 sa끄［ip1ed 신호는 그 펄스의 레벨이 일정하지가 않다. 이것은 음성
신호가 정규화된 형태가 아니기 때문어］ 더욱 그러하다. 그러므로 우리는 이러한 신
호들을 구별시켜 주어야 하며 이것을 위해서 우리는 신호의 크기의 레벨을 나누어
주어야 한다. 일반적으로 이것을 양자화（Quant切毗ion）라고 하며 보통 8 Bit를 사용
하여 256레벨로 구별한다. 이렇게 하여 발생되는 펄스의 rate는 64kbps가 된다. 여
기서 발생된 펄스 열은 다음 단계인 channel codii堆으로 넘겨진다．
 이렇게 발생된 펄스 열은 시스템의 대역폭과 직접적으로 관련이 있으며, 따라서
이것이 작을수록 대역폭의 효율이 좋을 것이다. 때문어］ bit rate를 줄이는 노력이 더
해지고 있다. 물론 bit rate가 줄더라도 타당한 통화질이 유지되어야 함은 두말 할
것도 없으리라. 이러한 노력들로 인해서 압축기술이 개발되고있고 이러한 압축기술
의 예로는 /\DPCM, CELP등이 있다. ADPC八/1인 경우 보통 32K ADPCM을 많이
사용하며, QUALCOMM社의 Q-CELP는 8K, 13K Vocoder를 사용한다. 유럽의
GSM의 경우도 이러한 보코더 형태인 RPE-LTP라는 보코더를 사용한다.
 최근의 이동통신에서는 보코더라는 새로운 소스 코딩 기술이 선보이고 있는데 이
것은 파형 그 자체를 코딩하고 압축하는 것이 아니라 파형을 분석하여 그것의 성분
별로 Parameter화하여 전송하는 방법이다. 즉 파형을 만들 수 있는 근거자료를 전
송하는 것이다. 이러한 보코더에 대한 공부는 9장에서 상세하게 할 것이다．


  1.3.2 Channel Coding

 Source Coding된 신호를 넘겨받아서 다음으로 수행하는 Process가 Channel
Coding이다. 이것의 역할은 전송할 데이터가 채널환경에 의해서 왜곡되어 에러가
발생되는 것을 방지하는 것 아니 더 정확하게는 에러가 발생되더라도 복원이 가능
하게 하기 위해서 전송되기 전어］ 특정한 조치를 취해 주는 절차를 말한다．
 가장 직관적인 예로서 필자는 간혹 다음과 같은 예를 든다. 전달하고자 하는 정보
가 "당신을 사랑해"라는 말이 정보라고 할 때 이 정보를 "당신을 사랑해. 당신을 사
랑해."라는 식으로 전송한다튼가 "당당신신을을 사사랑랑해해"라고 전송한다고 하
면 중간어］ 한 글자 혹은 하나의 자모음이 빠지더라도 내용은 해석할 수 있는 확률은
높아질 것이다. 이렇게 채널환경을 거친 데이터어］ 비록 에러가 발생했다 하더라도
정보를 정확하게 해석할 수 있는 확률을 높여 주는 기능을 채널 코딩이 수행한다．
여기에서 부가적으로 추가되는 정보를 우리는 Redun由ncy라고 한다．
a
    ] . 이동통신 방식                                   47
                                                       I
 이러한 채널코딩은 Block 부호화와 Cony아utional 부호화로 구별해서 생각할 수
있으며, 이것은 코드워드를 생성하는 생성 다항식과 입력 다항식간어］ 어떠한 형태
로 구해지느냐어］ 의해서 구분되는 방식이며, 일반적으로 Convolutional 부호화는
훨씬 큰 Re把ndancy를 가지며, 따라서 훨씬 강력한 코드성능을 가진다. 물론 대역
폭과의 tradeo卄로 얻어지는 장점이다. 이러한 코드의 내용어］ 대해서 6장의 RTT를
공부하면서 좀더 상세하게 확인해 보자
  Block 부호화는 전송할 데이터를 얻마씩 Package화하고, 거기에 Parity Check
bit를 첨가하여 전송 도중의 에러로부터 보호하는 방법이며, 잘 알려진 Hamming
Code와 Burst한 에러의 해결어］ 용이한 Reed-S이on均n Code는 이러한 Block
Code어］ 해당된다．
 Convolutional 부호화 방법은 현재의 데이터와 앞으로의 몇 개의 데이터 그리고
뒤로의 몇 개의 데이터들의 특정한 조합들로 데이터를 Codii培하는 방법이다. 이
것은 Elias어］ 의해서 처음 소개되었으며, 순차적 부호화（Sequ印tial decoding) 방
식이 웬즈 크래프트（Wozencraft）어］ 의하써 소개되었으며, 궤환 부호화（Feedback
decoding) 방식이 八/Iassey어］ 의해서 개발되었다. 그리고 비티비（Viterbi)에 의해서
복호화 방식이 발견 분석되었다. 그리고 Fomey와 오무라（Urn出a）에 의해서 최대
확률론적 부호화低佃dmum likelihood decoding) 방식으로 입증되었다.
 Block Code는 k개의 정보 Bit를 하나의 코드워드 단위로 부호화시키는 특성을
갖는데 비해서 （沁nvoli式ional Code는 위도우 개념을 이용하여 유한한 과거입력 더］
이터들이 현재의 데이터어］ 영향을 미치는 특성을 이용화하여 부호화한다고 구별할
수 있을 것이다.
  현재 상용화되어있는 Qualcomm사의 CDMA System의 경우 Cony아utional
Encodir垠과 \Iiterbi DeCoder를 사용하고 있으며, 고속데이터의 Burst한 에러를
해결하기 위해서는 Turbo Code를 사용한다．

     1.3.3 Modulation

 지금까지의 과정들은 데이터를 형성하는 과정이었으며, 이렇게 형성된 데이터들을
전송하기 위한 과정이 또 필요하다. 이러한 처리과정을 Modulation이라고 한다. 그러
므로 Channel Coding된 펄스열은 전송을 위해서 시스템의 MODEM(Modulator /
DEModulat아）어］ 이르게 된다. 여기서는 실지로 데이터를 전송하기 위해 Carrier
     48                                                  j. 이동통신 방식
                                                                      口


신호어］ 실어서 보낸다. 디지털 통신의 入4odulation 방식은 아날로그와는 달리 전송
할 데이터의 경우의 수가 유한하다. 사실 이것은 2의 n승으로 경우의 수가 있으나
특별한 경우를 제외하고는 2, 4, 8, 16 정도이다. 그래서 디지털 통신의 Mo血lation
은 각각을 구별 가능한 적당한 Sinusoidal신호로 入4appir瑁이라고 생각할 수 있다．
그래서 디지털 Modulation방식에 Shift Keying이라고 부르는 데이터의 천이 형태
의 방식이다. 이러한 디지털 변조방식은 다음의 예와 같이 아날로그 변조와 구분될
수 있다．
  우리는 화장실에서의 대화를 생각해 보자. 화장실에서 사용하는 노크는 전형적인
디지털 변조방식의 예라고 볼 수 있다. 즉 첫 번째 노크는 " 안어］ 누가 있나요7"라는
의미가 될 것이며, 두 번째 안에서 하는 노크는 " 안어］ 사람이 있습니다"라는 의미를
가진다. 이러한 방법에서 우리는 특정한 기호가 미리 약속된 의미를 담고 있고 이러
한 기호로 통신하는 방법을 디지털 통신이라 할 수 있으며, 이러한 디지털 통신에서
정보를 전송하는 방법인 디지털 변조 방식이다. 즉 전송되는 師usoid瓠신호의 위상，
진폭, 주파수 등어］ 이러한 기호의 의미를 실어서 전송하는 방법이 디지털 변조 방식
이다. 이러한 이유로 디지털 변조에서는 실지로 전송되는 신호는 각각의 의미를 담
은 위상 정보 혹은 주파수 정보 또는 진폭 정보에 실려서 전송되는 것이다．
  아날로그 Modulation에서와 마찬가지로 Carrier 파는 기저대역（Baseband) 신호를
운반하기 위한 재료로 진폭과 주파수 위상이 있다. 이것어］ 따라서 ASK(知nplitude
Shift Keying), FSK(FreQuency Shift Keying), PSK(Phase Shift Keying)로 나
누어 생각할 수 있다．
 入如dulation방식은 대역폭 효율, 전력 효율, 인접 채널간의 간섭 등의 요구 조건
들로 인해서 기본형의 수정된 형태들이 등장하게 되었다. 일반적으로 PSK는 대역
폭 효율과 전력 효율면에서 FSK나 ASK보다 월등하게 좋으므로 많이 사용되어지
고 있다.     현재 가장 많이 사용되고 있는 Modulation 방식들은 실지로 QPSI（계열
로 볼 수 있는 OQPSK, /4-QPSK, 入1SI도 （盈4SK 등이다. H 인접 채널간의 간섭을
줄이기 위해서 八4SK, GMSI( 등이 있으며， 대역폭 효율을 개선한 Modulation방식
이 QPSK, 8PSK, 16QAM 등이다．
 통신에서 효과적인 전송을 위하여 八如dulation방식어］ 적당한 Detection방식이 중
요하다. Detection으로는 크거］ Coherent와 Non-Coherent Detection이 있다．
 （노herent 방식은 n개의 Correlat아를 사용하는 방법과 八1atched filter를 사용
    ] . 이동통신 방식                                       49
I


하는 방법 그리고 가장 많이 사용되고 있는 IQ 채널 방식이 있다. 이 방식은 하
나의 Carrier어］ 몇 개의 정보가 실려 있다 하더라도 단 2개의 Correlator로만이
Detection이 가능하다는 것이다. 중심이 되는 아이디어는 서로 Orthogonal한 두
성분으로 좌표를 형성하여 그러한 좌표 내에서 I- 성분을 체크하고 Q-성분을 체크
하여 수신퇸 데이터로부터 정보를 얻는다는 것이다． 이것은 Modulation시에도 마
찬가지이다．
    이러한 방법 이외에 Carri町파를 수신단에서 비교한다는 측면에서 Coherent 방
식으로 보여지는 Differential Detection이 있다. 이것은 Carrier를 수신단에서 재생
하지 않고 바로 앞어］ 수신한 신호를 Carrier파로 사용하는 방식이다. 이것은 결과적
으로 Detection이 ／뇨的correlation을 함으로 구해지는 것이다. Non-Coherent 방식
은 Discriminator Detection, Envel아光 Detection 등이 있다.


     1.3.4 Frequency Spreading

    CDMA에서는 다른 접속방법과는 달리 Modulation이 두 번 행해진다고 생각할
수 있다. 그 두 번째의 八4odulation방식이 FREQUENCY SPREADI1나G이다. 이것
은 Random성이 아주 강한 PN Sequence로 八如dulation하는 것을 말하는데 이러한
Sequence는 Chip rate가 아주 빠르며 따라서 이러한 Ch如이 채널을 통과하기 위해
서는 엄청나계 넓은 대역이 필요하며, 이것과 부합되기 위해서 대역은 확장이 일어
난다. 여기서 간과（看過）하지 말아야 할 것은 PN이 완벽한 Noise가 아니라는 것이
다. 따라서 확장되어진 대역은 연속적일 수 가 없으며 PN Sequence의 rand아n성이
더욱 더 강해질수록 대역의 연속성은 더욱 더 강해진다는 사실이다. 이것을 명확하
게 하기 위해서는 어떤 통신이론의 교과서든 빼놓지 않고 나와있는 "Si光ctrum
analysis Part"를 확인해 보면 될 것이다．
    이러한 방법은 기존의 MA(Mu出pie Access) 방식들은 채널들을 주파수 혹은 시
간으로 구분되 었으나 서로 Orthogonal한 어떠한 물리량으로나 Coordinat아를 형성
할 수 있다는 개념 아래에서（이것은 변조에서도 적용되는 개념이다．) 이것을 좀더
확장하여 주파수나 주파수와 함수관계인 시간과는 별개인 새로운 개념 전송률
Code로써 채널을 구분하는 새로운 방법인 CDMA어］ 적용되어진다．
    실지로 이 방법은 채널의 용량에서 상당한 확대를 거둘 수 있으며, 하나의 채널이
엄청나게 넓은 대역을 사용하므로 Jamming 등과 같은 간섭어］ 상당히 강하다．
                                                        ] . 이동통신 방식
                                                                      U


    1.3.5 Multiple Access

  통신에 있어서 八4u出比o-Multi의 통신에서는 이것을 중간에서 중계를 해주는 시스
템이 필요하며, 이러한 시스템을 Switching System이라고 한다. 이러한 針版tching
System과의 접속을 위한 처리가 八/[ULTIPLE ACCESS이다．
  이것의 기본 IDEA는 여러 명의 각기 다른 개인들이 그들이 원하는 특정한 개인
과 통신을 위해서는 자기 신호만의 통로가 필요할 것이다. 이러한 통로의（이것은 채
널이라고 함） 필수조컨은 서로가 구별 가능한, 즉 완벽하게 Orthogonal해야 한다．
다시 말하면 어떤 Orthogonal한 물리량이 있으면 그것으로 구별하여 다중접속을
실현할 수 있다는 것이다. 물론 이러한 양（量）들이 통신어］ 얼마나 적용 가능하느냐
도 중요한 문제가 될 것이다．
  다중접속은 크게 Fl呱4A(Frequer兀y Division 入/Iult珀扼 Access), TDMA(T如e
Division Multiple Access), 그리고 CDMA(Code Division Multiple Access)로 3
가지가 있다. 이것들의 특징은 서로 0rthogonal한 주파수를 사용하여, 서로 Ortho
gonal한 T如e Sl毗를 사용하여 서로 Orthogonal한 Code를 사용하여 자기의 정보
를 표시하1 주는 것이라고 생각하면 될 것이다．
 이것을 좀더 직관적으로 이해하기 쉽게 예를 들면, 두 Co叩k의 연인들이 로비에
서 대화를 할 때 Couple A의 연인이 또 다른 Couple B의 대화로 인해서 방해를
받지 않기 위해서 Couple A의 연인들의 성대와 귀는 소프라노의 소리만으로 말할
수 있고 들을 수 있으며, 또 다른 Couple B의 연인들의 입과 귀는 베이스의 소리만
을 말하고 틀을 수 있다고 한다면 그들은 서로 방해를 하지도 받지도 받지 않고 대
화를 할 수 있을 것이다. 이렇듯이 두 Couple의 연인들이 그들만의 주파수로 그들
의 정보를 교환할 수 있다. 이러한 것이 주파수 분할 다중접속 방식인 Fl呱4A인 것
이다．
 만약 그들은 서로 한마디씩 교대로 하기로 약속을 하고 대화를 한다고 하면 그것
이 비록 같은 소프라노의 소리만으로 대화를 한다 하더라도 역시 대화가 가능할 것
이디．. 이렇듯이 두 Couple의 연인들이 그들만의 시간으로 정보를 교환할 수 있다．
이러한 것이 시분할 다중 접속 방식인 TDMA인 것이다. 이러한 방법에서는 자기
파트너가 말하는 시간을 정확하게 알아야 함이 필요하다는 것을 알 수 있을 것이다.
 또한 서로가 상대방이 알아들을 수 없는 외국어로 대화를 한다고 해도 그들만의
대회를 할 수 있을 것이다. 이 경우는 동일한 주파수 동일한 시간이라고 하더라도
    1. 이동통신 방식                                           51
1


대화가 가능한 것이다. 그러나 여기에서는 다른 Couple의 말이 내가 알 수 없는 말
일지라도 그것의 소리가 너무 커서 방해가 될 수 있음을 주의해야 할 것이다. 이렇
듯이 두 Couple의 연인들이 그들만의 언어로（혹은 코드） 정보를 교환할 수 있다. 이
러한 것이 코드 분할 다중접속 방식인 CDMA인 것이다．
 이상과 같이 각종 다중접속 방식을 예로써 설명했다. 그러나 주의해야 할 것은 이
러한 예들은 시스템을 이해하는데 필요한 예일 뿐이지 시스템은 이러한 것과 똑같
지는 않다는 것을 이야기하고 싶다．
 디지털 통신은 마치 물컨을 공장에서 만들어 시장어］ 내다 파는 것으로 비교를 한
다면 공장에서 원자재를 구입하는 것을 下orm的ng”이라 하고 그 원자제로 제품을
만드는 것을 Source Coding 이라 하며, 이 제품을 유통과정에서 보호 및 구매자의
눈어］ 띠게 할 수 있게 하는 상품포장을 Channel Codir垠이라고 할 수 있다. 또한 제
품을 수송하는 과정을 入如dulation이라고 하며, 많은 구매자에게 적당한 가격으로
판매하는 것을 入4u1tip1e Access라고 할 수 있다．



    1.4 IS-95 and Friends

 통신에서 가장 많이 나오는 이야기 중의 하나가 "I노毗ocol", 즉 통신의 규약이다．
이것은 서로 약속된 방식으로 신호를 주고받아서 의사교환을 하자는 통신방식의 원
칙일 수 있다. 이러한 원칙들은 가장 보편적이고 타당하게 정의되는 것이다. 그러나
이러한 보편적이고 타당하다는 것은 먼저 기술을 개발하고 그것을 정의하려고 하는
사람이나 집단의 입장에서 보편적이고 타당하다는 표현이 더욱 정확할 것이다．
 이 절에서는 이러한 통신의 표준화기관과 그러한 기관들어］ 의하써 권고되고 있는
표준안들에 대한 전반적인 내용을 공부할 것이다. 특히 여기에서는 아통통신 시스
템어］ 대해서 주로 이야기할 것이다.


     1.4.1 표준화 동향

  일반적으로 세계표준화추진 체계는 국제전기통신연합(ITU : International Tele
conimun妃ati아i Unisons), 국제표준화기구 ISO(Internationa1 Stand可d Organi
zation) 등 국제표준화기구를 중심으로 하는 공식 표준화（de 佃re standardization)
 r '52기                                              ] . 이동통신 방식
                                                                   1


활동과 각종 포럼이나 단체 등을 중심으로 하는 사실상 표준화個e facto standar
dization) 활동으로 나눌 수 있다. 1快刃년대 이후 세계표준화 활동의 두드러진 특징
은 1990년 25개에 불과했던 기술표준화 포럼이 최근에는 1（刃여 개 이상으로 급격히
증가하는 등 특정 기업들이 자율적으로 포럼 등을 구성하여 시장이나 기술 지배력
을 바탕으로 한 사실상의 표준화 활동이 급격히 증가하고 있다는 점이다．
 이러한 포림이나 단체들은 ITU등 국제표준화 기구와의 경쟁 또는 협력을 통해서
그 영향력을 급격히 확대하고 있으며, 이들 포럼이 매우 다양하江］고 증가함으로써
표준어］ 대한 인적자원이 부족한 개발 도상국이나 후진국은 세계표주화어］ 대응이 더
욱 어려워지고 있다．

   1.4.2 표준화 기구

 전세계적으로 이동통신을 위한 표준화 기구는 국제조직과 지역을 기반으로 하는
조직, 그리고 산업체 조직으로 분류할 수 있다. 국제조직으로 표준화 기구의 대표적
인 기구는 유엔산하의 ITU를 이야기할 수 있다. ITU는 ITU小T와 ITU-R로 구성
되며, 이것은 각각 CCITT와 CCIR의 새로운 통합된 형태이다. 여기에서 ITU-T의
경우는 유선망 분야의 표준화를 담당하며, ITU-R은 무선망어］ 대한 표준화를 담당
한다．
 산업체 조직으로 분류되는 표준화 기구로는 ATM Forum고｝ CDG(CI呱4A
Development Group) 등이 있다. 특히 CDG 恥rum은 CDMA관련해서 산업체들로
구성퇸 포럼으로 우리나라의 CDMA 장비제조사와 서비스 업체들이 이 포럼어］ 참
여하고 있다．
 이외에도 각 지역을 기반으로 하는 표준화 기구들이 있는데 유럽의 ESTI, 미국
의ANSI, 우리나라의 TTA, 일본의 ARIB, 북미 지역의 EIA/TII\ 등이 여기어］ 해
당된다．

  1.4.3 ITU(Internationa1 Telecommunication Union)

 국제 전기통신연합인 ITU는 범세계적인 전기통신 표준화 추진, 무선 주파수 사
용시의 질서유지, 기술 조작상의 문제어］ 대한 연구 및 개선책 마련, 각 나라들의 전
기통신체제 개발지원 등의 활동을 하는 유엔 산하의 조직이다．
 1865년 ITU는 창립되어서 1927년에는 CCII값무선）을 설립하였고, 1947년에는 유
    ] . 이동통신 방식                                             53
1

엔 산하기관으로 등록이 되었다. 1952년에는 국제기구로서 기술협력 활동을 개시하
였으며, 이 해어］ 한국이 가입했다. 19晟；년에는 CCIF와 CCIT를 통합하여 CCITT를
설립하였다. 그리고 1羽2년에는 CCITT를 ITU-T로, CCIR을 ITU-R로 개칭하여
오늘날어］ 이르고 있다．
    ITU의 하부조직으로 전권 위원회（Pp : Plenii刃tentiary Conference), 이사회
(Council), 사무국（General Secretariat), 국제통신회의(World Conference on
International Telecommunication）으로 구성되어 있다. 특별히 이러한 조직 이외어］
유선망 분야의 표준화를 담당하는 ITU-T와 무선망 분야의 표준화를 담당하는
ITU-R을 하부조직으로 가지고 있다．


           T

    ITU-T는 표준의 재／개정을 승인하고, 연구과제（Quest幻n）의 채택 등을 수행하
는 \VTSC(World Telec아nfl叱nication St可idardization Conference）와 표준화 활
동의 전략, 우선 순위의 검토와 작업계획의 시행 절차를 검토하고 각 연구위원회의
작업 가이드 라인을 제시하는 전기통신 표준화 자문반（TSAG : Telec아imu血
cation Standardization Advisory Group) 1 91다.
    또한 실무작업을 하는 14개의 연구반（SG: Study Group）이 있는데 주요 SG의
기능은 다음과 같다．


     SG                   설명                      비고

                                      19얹；넌 SG1가 SG14를 폐지하고 SG16유
     SG1       서비스, 번호체계, 트래픽성능
                                      신설함
     SG4       TMN
     SG7       Security
    SG11       Signaling과 프쿠두콜        I入'IT-2000의 표준화를 주관하고 있음．
    SG16       부호화, 압축 및 다중화 기법
    SG12       No7, ISPC할당계획



    각각의 SG에서 제정한 권고안은 \VYSC의 결의안（Resoh此ion）으로 정의된다．
    54                                              ] . 이동통신 방식
                                                                  .




 ITU-R

 이 조직은 ITU-T와 마찬가지로 유엔 산하의 ITU의 하부조직으로 무선통신어］
관련된 규격을 제정하고 배포하는 기관이다. 이 기관은 6개의 하부조직으로 구성되
어 있다．
 ITU-R의 수행업무로는 세계 전파통신회의（WRC）와 지역 전파통신회의를 개최
하여 전파규칙을 개정 보완 및 주파수 스펙트럼의 새로운 이용을 결정하고, 무선통
신 서비스와 시스템어］ 대한 기술적인 특성과 운영절차어］ 대한 권고를 제정한다. 또
한 서로 다른 국가의 무선국간 유해한 장애나 간섭을 막기 위해 필요한 조치를 강구
하고, 전파통신 관련 새로운 기술적 방법을 연구하고 제시한다. ITU-R의 구조는
（그림 卜15）과 같다．




         전파통신총회                         지 역 전파통신회 의 (RRC)
           (RA)


         전파통신연구반                        전파관리위원회 [RRB)
           (RRC)


                                         전파통신 자문위 원 회
                                            (RRC)

                       전파 통신국
                         (BR)                   1
                    （그림 卜］5) ITU日의 조직



 ITU-R의 주요 조직과 기능은 다음과 같이 요약할 수 있다．
 주파수 할당 및 배분 계획의 개정 및 보완기능과 전자파통신 관련 기술운영 사항
을 심의하는 세계전파통신회의(WRC : World Radiocommunicati아i Conference)
가 있으며, 전파통신 연구반（SG: Study Group）별로 과제를 배정하고 이를 승인하
며, 때로는 연구반을 신설하고 폐지하는, 즉 ITU-R산하의 8개의 전파통신연구반을
총괄하여 관리하는 전파통신총회（RA: Ra（五ocon끄Tiunication Assem川y）가 있다．
전파통신총회에서는 다음과 갇은 주요 켤과 문서들이 있다．
     j . 이동통신 방식
 1                                                          55

     半 연구과제（Question) : 연구를 통하여 결과가 요구되는 기술적 또는 운영절차상
      의 문제
     米 권고（Rec아nmendation) : 국제적으로 통용될 정도로 수행된 연구과제어］ 대한
      결과
     水 결의（Res아ution) : 총회와 연구반 작업을 위한 조직, 수행 방법 등어］ 대한 지시
      문서
     半 보고서（Report) : 연구과제 또는 준비회의어］ 의하여 제공된 연구과제어］ 대한
      연구 수행 잠정 결과
     永 핸드북（Handb（刃k) : 전파통신어］ 관한 현재의 수준을 기록하고, 현재 연구상황，
      효율적인 운영 또는 기술적 관행 등을 제공하는 문서
     전파통신 연구반의 경우 전파통신 관련 연구 및 권고（Recommendation) 초안을
준비한다. 이러한 권고안은 전파통신 연구반 차원에서 채택하거나 전파통신총회에
서 승인을 받는다. 전파통신 연구반의 산하조직으로는 연구수행 작업반들로 ＼入／P
(Working Party), TG(Task Groups), JTG(Joint Task Groups), J자P(Joint
Working Pa此ies) 등이 있으며 wP에서는 연구반어］ 분배된 연구과제를 수행하며，
시급한 연구과제는 TG에서 수행하며, 복수개의 연구반으로부터 전문가의 참석이
필요한 연구과제어］ 대해서는 JTG 및 JwP와 같은 연합 작업반을 구성하여 연구과
제를 수행한다. 전파통신 연구반들로는 요즘 부쩍 많은 관심의 대상이 되고 있는
M江JAN(Wi托less LAN) 분야를 담당하는 SG2와 IMT-2000, 이동전화 및 위성통
신 서비스 분야를 담당하고 있는 SG8 등이 있다. 특히 SG8내에 임시로 구성된
TG8에서는 瓜'IT-加00관련 표준화 작업을 진행중이다. ITU내에서 실제 표준화 작
업들은 SG에서 이루어진다.
 또한 전파통신 분야의 중장기 소요를 제기하고 업무 방향을 수립하고 ITU-T와
업무협조 및 조정을 담당하는 전파통신 자문반（RAG : Radiocommunic毗ion
Advis이y Group）이 있으며, 이외에도 전파통신국（RB : Radiocoi끄Lrnunication
Bureau), 전파콴리위워회／전파조정국（RRB: Radio Regulation Board) 등이 있다．


     1.4.4 TIA(Telecommunication Industry Association)

 TIA는 북미지역에서 통신관련 표준화를 담당하는 기관으로 이 기구는 전반적으로
업무를 총콸하는 사무국（Bo町（I of Direc的r）과 이들어］ 의해서 형성되는 Tec노lical
       56                                                j . 이동통신 방식
                                                                       .


Conirnittee가 있다. 기술적인 사업들은 모두 끄／\Tec如ical Committee의 통제하
에서 이루어지며, 표준화와 기술부서 스탭들은 Tee如ical Committee와 engineering
committees, 그리고 그것들의 하부조직 각각어］ 행정적인 지원을 제공한다．
     Technical Committee는 지휘 평의회어］ 의해서 조직된 특별위원회 중의 하나이
며, 의장은 사무국의 멤버 중에서 한다. Tee如ical Comm玭ee는 이 협회의 사무국
기술정책 형성을 위한 전반적인 책임을 지며, 여기에는 Techn아ogy Department와
Engineering Committee가 포함이 되며, 그것들의 처리정책과 조직을 포함한다．
Technical Comm批侊는 특별한 주제를 가지고 일을 해야 할 때 수시로 Engineering
Committee를 만들어서 일을 해당 EC에 할당한다．
     Engineei如g Committee는 Subcommi仇ees(SC）나 SC의 하부조직으로 형성되
는 Working Group(W(引을 만들어서 세부적인 일을 추진하며 좀더 세부적인 일을
위해서는 SC나 \VG의 필요에 의해서 Task Grou可TG）을 조직하囚 좀더 작은 연
구조직으로 세부적으로 연구를 수행한다. 이러한 작업을 통해서 나오는 결과물어］ 대해
서는 FO, TR 등과 같은 접두어를 사용해서 관리된다. 예를 들면 TR-8, TR-14,
FO-2, FO小 등이 그것이다．
     또한 TIA는 광범위하게 변화하는 무선 통신 규약어］ 대처하기 위한 산업체의
자발적인 표준화의 참여를 주도하도록 ANSI(／뇨rnerican National Stand可ds
Ins蹴ute）로부터 공인되었다． 이로 인해서 TIA는 산업체의 70여 개 이상의 공식적
인 표준화 그룹에게 지원하는 5개의 division으로 구성되었으며, 그러한 5개의
thvision은 Fiber Optics, User Premises Equipment, Network Equipment,
Wireless Communications, Sateffite Cot그nfl그unications와 같은 5개의 division이
다．
     TIA의 기술요구 사항, 즉 TR(Technical Requirement）은 Engin比ring Cot列mittee
의 이름이거나 그것의 연구범위를 나타낸다. 이러한 TR은 그것의 Engineering
Committee의 이름과 내부에 존재하는 SC및 WG가 또 존재한다면 그것의 이름을
가지고 표시한다. 즉 TR-45인 경우 Engineering Comm批ee를 지칭하며, TR-45.1
은 Engineering Commi伉ee내의 SC를 지칭하는 것이다. 이러한 방법으로 확장되어
서 TR-45.1.1의 경우 Engineering Committee내의 \TG의 이름까지를 나타내는 것
이다. 현재 활동중인 TR의 종류는 ＜표 卜1＞과 같다．
    ] . 이동통신 방식                                                      57
U

                              （표 ］너 ) T日의 종류

    01 름                                  설    명

    TR8      Land Mobile Service

    TR-14    Point to Point Communication System

    TR그9    Facsimile System and Equipment

    TR-30    Data Transmission System and Equipment

    TR-45    Mobile and Personal Communication Public 800 Standard

    TR-46    Mobile and Person삼 Communication Public 1800 Standard



 각 Engineering Committee어］서 표준화 작업을 위해 프로젝트를 개시할 때 TIA
의 사무국어］ 개시신청을 해야 하며, 이때 부여받은 번호가 PN(I노이ect Nuii小er）이
된다. 이러한 PN은 그것이 사용될 때 PN을 접두어로 하여 뒤어］ 4자리의 숫자가
기록되며, 이 4자리의 숫자는 고유한 번호가 된다. 예를 들어서 PN召383 등이 그러
한 예이다. 따라서 TIA어］ 발생되는 모든 문서는 PN번호가 모두 기록되어 있어야
한다. 이와는 구별되는 것이 SP라는 것이 있다. SP는 각 Engineering Committ아｝
에서 표준작업의 절차로서 각 TIA 회원사들에게 회람시킬 때 부여하는 명칭으로
이것 역시 뒤의 4자리의 고유한 숫자가 오며, 이 4자리의 숫자는 PN 번호와 동일하
다. 즉 PN-3383으로 작업을 시작하써 회원사에게 회람시킬 때에는 SP-3383으로
배포되는 것이다. 여기에서 SP는 Standard Pr야X羚al을 나타낸다．
 이것 이외어］ Engineering Committee에서 PN이나 SP로 분류하기어］ 부적절한 경
우어］ 문서의 출판어］ 부여하는 번호로 TSB(Teleco跏叱nica如n System Bulletin)
라는 것을 사용한다. 이것의 예로는 Service Option을 분류해 놓은 문서로 TSB-58
등이 있다．
 TIA에서 최종적으로 출간되는 규격이 우리가 친숙하게 들어본 IS(Interim
Stand可d）이다. 이것은 TIA의 지원을 받는 산업체 연합체인 EIA의 입장을 충분히
고려하여 최종적으로 산업 현장에서 빛을 발하게 된다．

 IS(Interim Standard)
 접두어 Is는 북미의 통신규격에서 많이 사용되는 것으로 우리에게는 CDMA의
     58                                                    ] . 이동통신 방식
                                                                          U

규격을 통해서 쉽게 접할 수 있다. 이 접두어 뒤에도 고유의 번호가 붙여져서 그것
의 형상을 대변할 수 있게 해 준다．
  유럽의 GS八l어］ 대응되는 북미방식의 TDMA의 이동전화 규격인 IS-54 등이 대
표적인 예이다. 다음의 （표 1-旬에는 QCDMA에 사용중인 혹은 연관된 Is 시리즈
들을 정리해 두었다．


                      （표 卜2) CDMA관련 Is 시리즈
  0i름                                 설 명
           伽alcornm CDMA의 무선 인터페이스 구간을 규정하는 규격으로 OSI 7layer
  IS-95
           중 layer3까지 규정하고 있음
           Qualcornm Cl呱4A의 Code Exited Linear Predictive Codac의 동작을 규정
  IS-96
           하는 규격
  IS-97    Qualcomm CDMA의 기지국의 하드웨어관련 취소 규격을 규정하고 있음
  IS-98    Qualcomm CDMA의 단말기의 하드웨어관련 취소 규격을 규졍하고 있음
 IS-125    13K QCELP의 동작어］ 관련된 규정을 기술하고 있음
 IS-126    EVRC의 동작어］ 관련된 규정을 기술하고 있음
 IS-637    CDMI\ 시스템의 Short 八4essage Service(S入43) 규격임
 IS-683    CI呱4A 시스템의 Over-the Service(OTA) 규격임
           무선 Date Service를 위한 규정들을 기술하고 있음. 이 부분에 대해서는 10장
 IS -707
           에서 다시 공부할 것임．



  IS-95의 경우 1993년 Qualc아nm사에서 제안된 것이 TIA에서 정식으로 권고안
으로 제정 발표되었으며, 이때 Is丹；의 보코더 규격과 갇이 나와서 초창기의
CDMA시스템의 형상을 구성할 수 있었다. 나중어］ 저속무선 데이터 서비스가 기능
에 추가되면서 Is小弱A로 발전하였으며, 후에는 중속 데이터 서비스 기능이 추가된
CAI(Common Air Interface）가 되면서 IS-95B로 발전하게 된다. 물론 MDR
小4ed油rn Data Rate) 서비스 이외에도 IS- 95B에서는 IS-95A의 Handoff나 전력
제어（Power Control) 등에 기능이 발전된 형태를 제안하고 있으며, 특히 Handoff
기능상어］ 많은 부분을 수정하여 시스템 성능을 업그레이드하고 있다．
 이후어］ 데이터의 기능을 좀더 보강한 IS-95C가 출현하게 되고 이것은 고속 데이
터의 실현을 위해서 새로운 RTT를 구성하는 것으로 RC(Radio Conf地uration）을
     j . 이동통신 방식                                        59
I                                                   1

세분화하여 규정하고 있다. 이러한 고속 데이티의 구현은 기존의 MDR과는 달리 S
 upplemental Channel(MDR의 경우 Supplemental Code Channel)이라는 새로
운 개념으로 하였다. 이러한 내용은 다음 장에서 공부한다．
 이러한 IS寸95C는 IMT-2000시대를 꿈꾸게 할 수 있는 전초전으로 흔히 2.5세
대 이동통신이라 하며, 그것의 이름 또한 IS-95시리즈를 벗어나서 IS-2000 혹은
cdma2000이리고 불리 운다. 이러한 이름들은 사람들의 기호나 지역에 따라서 같은
의미이지만 다른 이름으로 불려지고 있다．
  이렇게 무선 인터페이스가 발전해 오면서 데이터 서비스 기능 관련 규격들도
IS-99에서 좀더 포괄적인 통합 규격인 IS -707로 발전하였고, 이 IS-707시리즈의
경우도 데이터의 속도가 빨라지면서 부분적으로 수정되면서 규격 자체가 확장되고
있다. 물론 이러한 발전과 더불어서 보코더의 기술도 발전하여 관련 규격들이 새로
속속 발표되어 권고되고 있다.


      1. 4.5 기타


     CDG(CDMA Development Group)

  CDG는 Cl呱4A의 개발을 위하씨 북미의 4개의 주요 제조사인 I小TNQ(Lucent
Technology, Mo的rola, Nor tern Telecom, Qualc아l끄Ti)가 주도하여 만든 단체로
한국에서도 많은 제조업체와 이동통신 서비스 업체들이 이 단체어］ 가입하여 활동하
고 있다. 이 단체는 표준문서를 만들어 내지는 않으나 미국 내 표준화 기관인 TIA,
ANSI 등어］ 영향을 행사하7 위한 Forum, 기고지 등을 작성하는 형태로 활동하고
있다. 우리나라의 PCS에서 사용하는 13QCELP도 초기에는 이 단체에서 실행했던
For끄m과 기고지어］ 내용이 나중어］ 정식으로 규격으로 권고되어 사용되고 있다．


     ANSI(American National Standards Institute)

     미국 규격협회인 ANSI는 미국의 공업분야의 규격을 표준화하는 비영리 조직으
    로 국제표준화기구(ISO）의 멤버이기도 하다. 이 협회는 규격을 제정하지 않고 미국
    내의 각종 단체가 마련한 규격안의 심의를 돕고 승인한 뒤 분류기호와 번호를 부여
    한다. 따라서 상기어］ 공부한 TIA, CDG 등어］ 영향력을 끼치고 있다, 현재 우리나라
    에서 상용화된 2세대 이동통신의 핵심망 규격은 ANSI-41이다．
    60                                                 ] . 이동통신 방식
                                                                     S




 ETSI(European Telecommunication Standard Institute)

 1988년 CEPT(C파玎）의 표준화 업무를 인계받은 유럽 지역의 실질적 표준화 주
도 기관으로 32개국 412개 정회원 기관을 보유하고 있는 기관이다. 여기에는
General Assembly, ETSI Bo可d, Finance Committee, ETSAG, 14개의 기술위원
회, 6개의 특별위원회, 12개의 ETSI Pr이ect로 구성되어 있다. 현재 GS八l을 위해서
11개의 SMG에서 작업을 수행하고 있다．


 ARIB(Association of Radio Industries and Business

 일본의 통신 관련 무선분야 표준화 작업을 수행하는 기관으로 ITU-R과 관련된
작업을 수행하고 있다. 이것은 전체를 총괄하는 방식 작업반을 포함해서 6개의 작
업반을 가지고 있다. 6개의 작업반은 무선접속 작업반, 위성 작업반, WI工 작업반，
CODEC 작업반, 시험 작업반이다. AR떠와는 상호협조 관계어］ 있는 YFC(Telecom
munication Techn이ogy Committee）는 ITU-T와 관련된 유선망 관련 작업을 수
행하고 있다．


 TTA(Telecommunications Technology Association)

 국내의 표준화 기관으로 한국의 표준화 활동을 전담하고 있다. 여기에는 표준화
제정을 위한 11개의 분과위원회가 있으며, TMT그以刃과 관련해서는 약칭SC7인 차
세대 이동통신 분과 위원회에서 수행하고 있다．


  1.4.6 IMT2000을 위한 표준화 - 3GPP/3GPP2

 瓜IT2000는 국제 로밍과 고속 데이터 서비스를 구현하여 세계 어디에서나 통화
（나아가서는 화상전화 등과 같은 고속 서비스）를 할 수 있게 하는 것이었다．
 특히 국제 로밍어］ 의한 규격을 위해서 세계 단일규격 제정이 필요했다．
 처음에는 국가별로 표준이 나름대로 정해지고, ITU-R의 일정과 방법어］ 맞추어
국저1 표준화 작업이 순조롭게 진행되는 듯했으나 제출된 표준규격들은 각국의 이해
를 대변하는 것으로 그것의 종류가 단일표준을 지향하기에는 너무 많고 또한 각 지
역별 이해관계가 너무 첨예하게 대립되어 있어서 ITU가 이를 조정하기에는 실상
한계가 있을 수밖어］ 없었다．
    1 . 이동통신 방식
U

 따라서 유사한 방식을 지향하는 표준들을 권역별로 통합할 필요가 먼저 생겨났
으며 이러한 필요성어］ 의해 자발적으로 조직이 구성되었다. 그 결과 탄생한 것이
바로 비동기 방식 \V-CDMA 규격 단일화를 위한 조직인 3GPP(3rd Generation
Partnership Pr이ect）와 동기방식 cdma2000을 중심으로 규격 단일화를 위한 조직
인 3GPP2인 것이다．
 우리나라의 경우에는 처음부터 두 가지 방식 모두어］ 대해 표준을 제출한 상태였
으며, 따라서 양대 기구에서 동시어］ 활발히 활동하고 있다. 이 두 개의 단체는 법적
단체는 아니지만 각각을 구성하는 표준화 공인단체에서 협력사업을 협력하여 주창
하고 있다. 이 둘의 비교는 앞의 ＜표卜3＞과 같다．

                          （표卜3) 3GPP와 3GPP2이 비교

     명 칭                     3GPP                    3GPP2

    참여기관         ETSI, ARIB, Ti, TTA, TTC   TIA, TTA, ARIB. TTC
                 발전된 GSM핵심 망과 참가자들이         발전된 ANSI-41 핵심 망과 동기식
                 지지하는 무선접속기술을 바탕으로          CDMA로 알려진 cdma2000, 3GPP
     모＝ 처        한 3세대 이동통신 시스템에 대하여        를 바탕으로 한 3G 이동통신 시스
                                            템 관련 기술규격 및 기술보고서의
      中기
            1




                 전세계적으로 적용가능 한 기술규격
                 과 보고서를 준비, 승인 및 유지．        준비, 승인 및 유지．
                  사업조정그룹（PCG）과 기술규격그룹       운영위원회（SC: S自ring con끄"U
     조직
                  (TSGs)                    nities.）와 기술규격그룹（TSGs)
                  RTT관련해서는 FDD 방식의 \V       cdma2000과 ANSF-41의 발전형태
                  CDMA 및 TDD방식의 TD-CD入IA    로 기본적인 틀을 짜고있으며, 주요
                  방식을 추진하며, 핵심망은 기존의        활동으로는 3GPP무선 인터페이스
    활동범위 및        GS入4시스템의 발전 혹은 확장 형태      개발, 무선 패킷 데이터망 구성, A-
      목표                                    인터페이스 시스템 및 단말장치 개
                  로 규격작업을 하고있음. 아울러서 단
                  말기와 서비스개발관련업무도 병행해        발 등이 있음．
                  서 추진함．
                  협력사업설명서
     기본문서
                  협력사업작업절차
                  영위원회 작업참가권
 기관 참가자의
                  · TSGs 작업참가권
   권리
                  · 기술규격 및 보고서의 저작권 공동 소유
    협정의 개정        Consensus Agreement
       종료         탈퇴할 경우 6개월 전어］ 통보
           기 간    기간 참가자가 별도로 정할 때까지 효력발생
    추가 참가자        소재지에 불구하고 기관에 개방
    62                                             j . 이동통신 방식
                                                                 .




  1.5 Pcs 시스템

   1.5.1 시스템의 구성

 이 절에서는 PCS망을 좀더 일반적으로 이야기하기 위하1 이동통신망의 구성과 각
network element의 기능을 공부한다. 이동통신 시스템의 기능어］ 의한 구분은 사람
들마다 조금씩 다르겠으나 필자는 이동성 관리기능을 수행하는 /\ccess망과 라우팅
기능과 이동성 관리를 위한 데이터베이스 관리기능을 수행하는 교환망으로 구분한
다. 일반 공중전화망（PSTN: I뇨blic Switched Telecommunication Network), 즉
우리나라의 경우 한국 통신망이나 하나로 통신망 등과 같은 고정전화 서비스망의
경우 이동성 관리의 기능은 없으며, 가입자 라인과 교환망으로 구성된다．
 그러나 PCS 등과 같은 이동전화망은 가입자 각각의 이동성에 대한 정보를 관리
하는 기능이 필요할 것이다. 이러한 기능을 수행하는 영역이 BSS(Base Station
System)로 불리우는 영역으로 여기에서의 주요 기능은 Handoff 등과 갇은 이동호
에 대한 이동성 관리를 수행한다．
 개인 휴대통신 교환기인4 S Mobile Switching Center）는 주기능인 Switching
기능과 Routing기능은 물론 가입자의 접속, 과금, 시스템과 망의 운영, 유지보수에
관련퇸 기능을 수행하는 장비이다. 가입자의 통화요구를 받아 통화가 가능하도록
선로를 구성하며, 특별한 상횡어］ 대해서는 안내방송으로 응답하거나 부가서비스가 처

                       VMS!FMS
            CSBS




           卜｛LR


                                       HSC




         1WF!PDSN            없1S/VAD


                    （그림 卜］6) PCS 망 구성도
    ] . 이동통신 방식                                            63
U


리되도록 한다. 또한 八4SC牧IGSjnter Gateway System)와（'V四(Inter Working
                     ＼뇨mm中戶
                                    뇨         \-    /.\1
Function), VMS, FMS, VA]), 自啞 Short Message Service), (T方(Home
                              ／中＼
I刀cation Registrat幻n), CSBS, NMC/OMC와 연동하면서 동작한다．
  가입자의 정보를 일시적으로 관리하는＼兀R포함하며 관리한다. 교환기내의 VLR
(Visi的r Location Register）은 가입자가 서비스 영역으로 들어오면 HLR로 정보를
받아 관리하고, 나가게 되면 정보를 삭제한다. 또한 가입자 인증기능을 수행한다．
 IGS를 통해서 다른 시스템, 즉 한국통신, 테이콤, 다른 이동통신 업체 등과 접속
이 가능하도록 하며, 과금 및 검증작업 등을 한다. 비음성 데이터망과도 연동할 수
있도록 IWF와 연동하며, Packet data, Fax, Internet, Asynch 등과 같은 다양한
서비스를 이용할 수 있도록 해준다. 그리고 과금 및 통계처리를 CSBS(Customer
Service & Billing System）어］ 넘겨주어서 과금처리를 할 수 있도록 한다.
 BSS는 BTS(Base Transceiver Subsystem:71지국)와 BSC(Base Station
Controller : 제어국）을 합쳐서 부르는 것으로 BTS는 직접 가입자와 연결되는 기
지국으로 BSC를 통하여 모든 신호를 처리한다. BSC는 여러 개의 BTS를 관리하
며, 八45C와 결합되어 단말기간에 원활한 접속이 이루어지도록 한다. 이러한 BSS는
이동통신에서 추가된 시스템으로 이동통신에서만 제공되어야 할 기능들을 전담한
다. 그것은 이동성 관리와 무선 인터페이스 지원기능이다．
 HLR(Home Location Register）은 대용량의 실시간 데이터베이스이다. 망에서
요구하는 이동 가입자어］ 대한 정보를 처리해 주는 중요한 망 요소이다. HLR은 지
역을 이동하는 가입자어］ 대한 위치정보를 VLR로부터 받아서 저장하며, 해당 가입
자어］ 대한 호 요구시 HLR은 그 위치를 \7LR에 통보하여 가입자가 서비스 가능한
모든 지역에서 통신이 가능하도록 한다. 또한 가입자별 다양한 부가 서비스어］ 대한
상태 및 과금 Category 정보를 관리하여, 서비스가 올바르거］ 제공되도록 하며 이어］
대한 올바른 과금이 되도록 한다．
                     '저］, 국젯프쥴 SQL 을 지원하는 데 ' ］터베 " ]
 CSBS는 대형 컴퓨터， 개방형 운영긔
스, 객체지향 개발도구 등을 사용하여 개발돠七SBS뇬 고객어］ 대한 제반 모든 업무
를 처리하고 관리하며， 고陪어］ 콴련된 사항含乖向며 주요 기능은 다음과 같다．
    半 고객 정'보관리, 조회 및 무선 자동등록（OTA) 지원을 수행한다．
    水 상담접수, 이력관리, 요금정책 정보관리를 수행한다.
    米 실시간 과금자료를 수집, 저장하며 청구서 발행을 담당한다．
     64                               1 . 이동통신 방식
                                                    .


  水 가입자별 유형분석, 통계관리, 불법검사 등을 담당한다．
  PcS를 개통하는 절차라는 것은 Pcs의 전자일련번호와 전화번흐를 시스템과 단
말기어］ 각각 대응시켜 주는 것이다. 시스템에서는 그것을 HLR에 대응시켜 주는 것
이다. 그러나 사용 폰의 과금을 위해서 일반적으로 개통작업은 CSBS에서 이루어지
며, CSBS에서는 그것의 전자일련번호와 전화번호를 HLR로 넘겨 주어서 통화가
되게 한다．
 가입자의 전화수신이 불가능할 경우 또는 가입자에게 간단한 메시지만을 전달하
려고 하는 경우에 사용하는 부가 서비스로 기존의 문자호출과 유사한 瓢(IS(Short
入(Iessage Service）가 있다．
 단문 메시지의 발송은 단문과 단말기의 번호를 고객셴터 안내원에게 알려추어 전
송하는 방법과 PC통신, 인터넷을 이용하는 방법, 단말기의 키 패드를 이용하는 방
법 등이 있다. 단문이 수신되면 신호음（또는 진동）이 울리며 가입자는 단말기를 통
하1 내용을 확인할 수 있다.
 이 서비스의 가장 큰 장점은 통화중에도 사용이 가능하며, 전자우편 등의 수신 여
부도 확인할 수 있다. 뉴스, 날씨, 경기결과, 바이오리듬 등 다앙한 문자정보 서비스
도 받을 수 있다.


   1.5.2 망 자원 할당

 통신 시스템에서 통신의 대상이 되는 두 지점간을 연결하기 위해서 사용하는 자
원을 망 자원이라 한다. 그렇다면 통신을 위해서 사용하는 자원이라는 것은 무엇이
겠는가. 전자통신에서는 정보를 전달하는 전자파의 대역폭괴． 주파수를 가지고 망
자원이라 하며, 이것은 흔히 무선 주파수 자원이라고 한다. 이러한 무선 주파수 자
원은 배타적인（Excius押C) 특성이 있어서 무한정 사용할 수 있는 것이 아니다．
 이 절에서 이야기하려는 것은 이러한 무선자원뿐 아니라 통신시스템 내부의 중계
선상의 자원, 즉 시스템 장치의 성능（혹은 능력이라고 표현할 수도 있을 것이다）과
도 관련된 총체적인 자원을 이야기한다．
 이동통신 시스템에서는 이러한 망 자워 관리를 BSS에서 관리한다. 이러한 망 자
원은 무선망 자원과 중계선망 자원으로 분리해서 이야기할 수 있다. 무선망 자원의
경우 기지국에서 관리하고 할당되지만 중계선 망 자원의 경우 BSC에서 이러한 기
능을 수행한다. 무선망 자원을 우리는 통화채널 할당의 과정을 말하며, 중계선 자원
    j . 이 동통신 방식                                           65


                                           동인한 .kJ코．더 프래임옵셋이 여러 기
                                           지국에 닉 냐용되고 있으며， 이겻은
                                           ie11 Diver곡 t.y륜 외미한다，




1 1 目目1 통화 채널 프레임
0   l   2 3   중계선 프레임（보코더 프레임 옵셋）

                        （그림 卜］7) BSS의 자원



의 할당은 보코더 Frame 옵셋의 할당을 말한다. 따라서 BSS에서는 현재 특정한
단말기가 여러 개의 기지국으로부터 각기 다른 통화채널 번호를 할당받아서 통화를
한다 하더라도 중계선 자원, 즉 보코더 Fra끄［le 옵셋의 번호는 변함이 없다．
 （그림 1-17）에서 보는 바와 같이 BSC는 특정한 호어］ 할당된 보코더의 Frame 옵
셋을 여러 개의 기지국의 통화채널어］ 실어서 전송한다. 이것은 여러 개의 기지국의 신
호를 Combining하여 통신하는 Rake 수신기를 사용하는 단말기의 Cell Diversity로
동작한다고 이해해야 한다. 즉 （그림 卜17）의 경우 해당 단말기의 경우 기지국에서
할당되는 통화채널의 채널번호는 2번 Code Channel을 사용하며, 중계선의 자원,
즉 보코더 Frame 옵셋은 0번을 사용하여 통화를 하고 있다．
    만약 이러한 보코더 Frame의 변화가 불가피할 경우에는 망에서 다른 망 자원을
관리하는 영역으로 넘겨주어 새로운 Frame 옵셋을 할당받기 위하囚 기존어］ 가지고
있던 자원을 반납해야 하는 하드 Handoff를 해야 한다. 이동통신 시스템에서 이루
어지는 Handoff 중에서 중계선 자원간의 Han面卄가 발생될 때 중계선을 관리하는
II寸ra가 다르므로 하드 Han面卄가 발생한다. 이러한 경우를 해결하기 위해서 상위
의 새로운 프로세스를 둠으로 해결될 수 있는 것이다. 이러한 사항은 6장 Handoff
에서 좀더 공부해 보자．
   66                                1. 이동통신 방식
                                                  U


 사실 BSC, 즉 기지국의 상위 단에서 자원을 관리하는 것은 나름대로 타당한 것
이, 자원의 관리 측면에서 볼 때 이동통신의 경우 특히 셀룰러의 경우 자원의 할당
이 통신 Infra의 변동사항이 불가피하며, 이러한 불가피한 사항을 전체적으로 통제
하고 관리하기 위해서는 전체적인 내용을 알고 볼 수 있는 상위 프로세스에서 이러
한 것들을 관리하고 수행하는 것이 필요하기 때문이다．
    2. Basic Concept                          67
.




                               Basic Concept




    뜨거운 여름날 데카르트（R Desc8丁tes）는 누워서 낮잠을 즐기고 있었다. 그러던
중 그의 낮잠을 깨운 것은 그의 콧잔등을 누비고 다녔던 파리였다. 잠에서 깬 데카
르트는 순간 "파리의 움직임을 수식으로 표현할 수 없을까？"라는 다소 엉뚱한 생각
을 하게 되었다. 그러나 결국 이러한 것의 계기가 오늘날 우리가 수학시간어］ 배우고
있는 원, 타원, 쌍곡선, 포물선 등의 수학적 표현이 나오게 되었고 데카르트는 해석
기하학이라는 수학의 새로운 분야를 개척하게 되었다．
    수학의 수식표현은 이렇게 엉뚱하게 발견되는 경우도 있지만 대 부 보으 자신의 생
각이나 관념들을 체계적으로 정리하기 위해서 발견되고 발전되어 왔다. Issac
New切n이 자신의 운동법칙을 체계적으로 생각하고 설명하기 위해서 미적분학을
발견하였듯이 말이다. 이러한 수학적인 사고방식 아니 체계적인 사고방식은 우리가
돈을 셀 때 등과 같은 일상생활 속에서도 쉽게 접할 수 있다. 많은 톤을 정확하게
세기 위해서 우리는 일정한 단위를 사용한다. 이를테면 10장씩 혹은 100장씩 나누
어서 센다면 더욱 정확하고 체계적으로 셀 수 있다（이것은 진법이다）.
    이렇듯 수학은 우리의 사고를 체계적이고, 논리적이게 해준다. 그러므로 우리의
    68                                        2. Basic Concept
                                                                 .


사고방식을 체계적이고 논리적으로 만들지 못하고 수학 수식의 수많은 기호들에만
맴도는 적어도 순수 수학을 공부하지 않는다면 이것은 더 이상의 수학이 아니라 단
순한 스트레스일 수밖어］ 없다. 이 절에서는 주로 수학을 통하여 통신에서 사용되는
여러 가지의 加O1들어］ 대한 이야기를 할 것이나, 앞서 밝힌 필자의 생각대로 우리가
이끌어 내려는 개념들을 체계적이고 논리적으로 이해할 수 있게 해주는 방법들을
찾고자 하며, 독자들의 새로운 사고방식과 논리체졔를 형성해 갈 것을 권한다．
  수식은 함축된 의미의 표현이어야 하고, 새로운 혹은 또 다른 관점의 제시이며,
체계적인 사고의 결과이어야 한다는 것이 필자가 수식을 보는 견해이다．



  2.1 Correlation과 Normalization

 부전자전（父傳子傳）이라는 말이 있다. 이 말을 모르는 독자는 거의 없을 것이다，
이 말은 아들은 아버지를 닮았다는 이야기가 될 것이다. 생물학적인 측면에서 보더
라도 아들이 아버지를 닮는다는 것은 너무나도 당연하다. 이렇듯 닮았다는 것은 그
것의 특정 혹은 일부 속성들이 같다라는 것이다. 또한 아버지를 닮은 아들은 사람들
이 많이 모여 있는 장소어］ 아버지와 떨어져 있다 하더라도 다른 사람은 아버지와
아들을 비교적 쉽게 찾아낼 수 있을 것이다. 이러한 예는 좀더 닮은꼴인 쌍둥이의
경우 더욱 확실해진다.
 우리가 이 절에서 공부하게 될 상콴성, 즉 (iorre1ation은 이러한 닮은꼴의 닮은
정도어］ 대한 공부를 할 것이다. 물론 사람이 아니라 신호어］ 대한 것이다．
 이러한 생각은 1930년 \Vinner어］ 의해서 생각되었다. 그는 불규칙한 신호의 해석
을 위해 발견한 것으로서 임의의 시간 T만큼 떨어진 동일 파형 혹은 서로 다른 파
형 사이의 값어］ 관해 유사한 정도를 나타내는 척도이다. 상관이란 한 쌍의 시계열
사이의 선형 관계의 정도를 나타내는 것으로 이들 시계열의 닮음 정도나 혹은 두
시계열이 얼마나 선형함수로 나타내어질 수 있는가를 측정한다. 주파수 영역에서의
일관성과 유사한 시간 영역에서의 개념이다．
 상관함수는 두 신호 혹은 한 신호의 시간 영역에서의 상관성을 나타내는 함수로
서, 크거］ 자기상콴（Au的＜iorre1ation) 함수와 상호상관（Cross七Correlation) 함수로
구분된다.
     2. Basic Concept
 .                                                                                                  69


     상콴（Correlat幻n）의 수학적인 표현은 두 함수를 곱하여 함수의 주기 동안 적분하
고 그것들을 적분주기로 나누는 형태가 된다. 이것은 적정한 시간구간 스t의 간격
으로 두 신호（함수）를 곱하여 이 시간구간 동안 비교하게 되며, 이것을 상관값을 구
하려는 구간까지 계속 반복하게 된다. 이러한 시간구간 스／는 불연속적인 신호（함
수）인 경우에는 그것의 값이 "0"보다 충분히 클 것이지만 불연속 함수인 경우에는
"0" 어］ 최대한 접근할 것이다. 즉 거의 "0" 일 것이다. 이렇게 매 구간 비교된 값들의
평균값이 구간의 상관값으로 구해지게 된다.

           小J   工   =-l   ,   八1   , ,   ,4 .   =1   ,     1 iT   』． .   . .        .    .
          （선윽얌구느J 소ft才얌日＝ = ;;;}) /(rJ gU旭t                                                         (2-1)
                                                           I


     만약 시간에 대해서 변화하는 것이 연속적이지 않고 이산적이라면 적분은 필요
없을 것이며, 모두 Sumn追tion하면 될 것이다．


          연속함수의상관함수＝ 誰／（打）g(kt)                                                                     (2-2)
 （그림 ?1）은 이러한 상관에 대한 개념을 정리하여 보여준다. 즉 스／의 시간구간을
기준으로 하는 경우의 예를 다음과 같이 생각해 보자. 즉1／스／ Hz의 Clock으로 구
동되는 경우어］ 두 신호의 Bit들 각각은 매 Clock 동안 비교될 것이다. 즉 곱해질 것
이다. 그런데 여기에서 dc兀k의 주파수가 점점 빨라진다면 이것들은 곱해지는 경우
가 많아질 것이며（물론 평균을 구하므로 나누어지는 수도 많아진다）, 이것은 1／스t
가 작아질 때이다. 만약 스t7f "0"이 된다면 Clock의 빠르기, 즉 비교하는 경우 혹은
곱하는 횟수는 무한대가 될 것이다 이 것이 연속함수의 경우이다. 여기에서 알



                                                                               연속 함수의 경우 변화량이
                                                                               매 시간마다 있으므로 매시
                                                                               간 연속적으로 비교하게 됨 . {




                                                                                              스
           f (t)

           g(t)                                                                 f
                                                                                        (t)


                                                         Urn小＞0 亡포 = dt


                                         （그림 2-1) 상관（Corr이ation）의 의미
    70                                2. Basic Concept
                                                         .


수 있듯이 Clock의 구간동안 비교할 때 곱하기를 한 것이 연속적인 함수에서는 모
튼 점佃面北）에서 이루어진다고 생각할 수 있다. 이상과 같이 상관（Correlation）어］
대한 직관적인 설명을 깊이 생각하1 보라！
 신호 ／佃와 帥）의 상관성을 찾는다고 할 때, 그 상관값의 의미는 ／佃의 경우
的）에서 자신의 모습인 ／佃의 모습을 찾는 것이다. 이것과 상대적으로 g( t)도
／佃에서 자신의 모습인 g佃의 모습을 찾는 것이 퇸다. 켤국 상관성이라는 것은 두
신호의 공통점을 찾는 것으로 이러한 공통점은 두 가지의 신호가 서로 같은 부분을
가지고 있기 때문어］ 혹은 전혀 없기 때문어］ 신호의 해석에서 상당히 중요하게 사용
퇸다. 아버지와 아들을 볼 때 그 아들을 통해서 그 아버지의 모습을 찾게 될 때 우
리는 아들이 아버지를 닮았다고 이야기하며, 이것은 아버지와 아들의 상관성이 클
수록 두드러지게 나타난다．
 이러한 신호간의 상관성을 상호상관이라고 하며, 식 (2-1)에서 확장퇸 형태로 식
(2읾과 같이 상호상관 식을 쓸 수 있다．
           八八八n7m/   =




                                                  (2- 3)


 즉 앞서 말 한대로 두 개의 파형을 시간 V만큼 서로 어긋나게 곱을 만든 다음 시
간 평균한 값으로 구하게 된다．
 상호상관은 두 시계열의 유사성 및 선형성의 척도로서 정규 상호 상관값은 -1어］
서 +1의 값을 가지며 +1일 경우는 두 시계열이 완전히 일치함을 뜻하고 1일 경우
는 모양은 동일하나 위상이 역전된 경우를 나타내며 0인 경우는 두 시계열 사이의
유사성이 전혀 없음을 말해 준다. 이러한 경우를 우리는 뒤에서 공부하겠으나
Orth四onal이라고 한다．
 이러한 상관성의 한가지의 경우로 자기 자신과의 상관성을 계산하는 자기상관
(Auto-Correlation）이 있다．


   2.1.1 자기상관（Auto- Correlation)

 자기상관 함수는 자기 자신과의 상관성을 나타낸다. 언뜻 듣기에 자기 자신과의
상관성은 언제나 같은 값이 아니겠는가를 생각할 수 있으나, 특정한 시간이 지난 후
의 자신과 현재의 자신 혹은 특정한 시간 동안의 과거의 자기 자신과 현재의 자신과
의 상관성이라고 이야기하면 어느 정도 이해가 될 것이다．
    2. Basic Concept                                             기
1                                                       -   H
                                                                71

    과거의 자신과 현재의 자신의 상관성을 통해서 현재의 나는 과거의 나 자신에 비
해서 어떻게 변화되었는가를 생각할 수 있다. 이러한 상관성 계산을 과거에서부터
계속해 왔다고 한다면 이러한 （상관성의） 정보는 미래를 예측하는 것으로 사용될
수 있다. 왜냐하면 지금 현재의 나는 미래의 나의 입장에서는 과거의 내가 되기 때
문이다. 이러하듯이 자기상관 함수는 과거의 값으로부터 미래의 값을 어느 정도 여］
측 가능한가, 또는 T만큼의 지연시간 후에 파형이 현재의 값어］ 따라 어떻게 변하는
지를 나타내는 통계학적 측정량이라 말할 수 있다．
    이러한 자기상관성의 특징은 임의의 함수의 주기성을 찾아내는 데에 사용되기도
한다. 즉 주기함수의 경우 시간 옵셋이 0인 경우와 T인 경우의 자기상관의 값이 같
다면 이 신호는 반드시 주기적인 신호일 것이고, 이것의 역의 논리인 주기신호라면
그것의 자기상관은 특정한 간격으로 최대값1）의 자기상관값을 가질 것이다．
    신호 x(t）의 자기상관 함수를 일반적으로 I改妖r)로 나타내며, 시간 ／에서 신호
尤（t)와 시간 t+r에서 신호 尤（t+ r)값의 상관성을 말하는 것이며, 이것 역시 곱을
신호의 주기 T어］ 걸쳐서 평균한 값으로 나타내며, 다음과 같다．


          凡（7)
          R (t) =
                =-   i   j
                         T   x   (t)   x   (t+   r)dt           (2- 4)

    이때 지연시간 V는 양수 또는 음수일 수 있으며, 혹은 0일 수도 있다. 즉 자기상
관 함수는 시간이 지난 후 미래의 자신 혹은 과거의 자신과 현재의 자신과의 상관성
을 찾는 것이다. 이것은 채널상에서 같은 신호가 시간에 의해서 지연되어서 서로
다른 형태로 나타날 따r 현재 신호와 다른 경로를 통해서 전송퇸 또 다른 나와의 상
관성을 확인하는 것으로 우리가 앞으로 공부하게 될 동끼식 CDAM의 대표격인
Qualcomm CDMA 방식에서 동일한 생성다항식어］ 의해서 생성된 PN Code들의
동기를 찾을 때 요긴하게 사용한다. 여기에서 이것을 상호 상관이라 하지 않는 것은
동일 생성다항식에서 생성된 동일 코드이기 때문이다．

     2.1.2 0rthogonal

    앞서 공부한대로 두 신호간의 상관성을 측정했을 때어］ 완전히 일치하는 신호가
있는가 하면 완전히 일치하지 않는, 즉 공통성이라고는 전혀 없는 신호가 있을 것이

1) 자기상관 함수의 값은 시간 옵셋이 0일 때1, 즉 같은 시간이 같은 신호의 상관값이 가장
   크다는 것을 직관적으로 알 수 있을 것이다．
   72                                  2. Basic Concept
                                                          U


다. 이러한 두 신호간어］ 유사성이 전혀 없을 때, 우리는 이러한 두 신호는 직교
幻rthogonal)한다고 이야기한다. 이러한 직교한다는 것은 서로가 서로에게 어떠한
영향도 끼치지 않는다는 독립성（Inde硏三ndent）과도 연관이 될 수 있는데 직교한다면
두 신호는 서로 독립적일 것이다. 그러나 독립적이라면 반드시 그것이 직교한다고
는 할 수 없으므로 직교한다는 것은 독립적이라는 것의 필요조건이지 필요충분조건
은 아니다．
 이러한 직교는 상관성의 극단적인 경우라고 이해할 수 있다. 이러한 직교성은 통
신에서뿐만 아니라 우리의 일상생활 가운데에서도 상당히 유용한 사고방식들을 제
공한다. 즉 자석어］ 대해서 철과 비철은 서로 직교하는 성질이 있으므로 많은 모래
더미에서도 우리는 금속성분을 구별해서 추출할 수가 있다. 이것은 비철 성분의 물
질은 철 성분의 물질과 자석（magnetic）의 입장에서 봤을 때에는 Orthogonal하다는
특징을 이용한 것이다．
 직교성은 두 신호간의 내적이 0일 때 직교한다고 할 수 있다. 즉 두 신호간어］ 위
상 차이가 90도일 때 두 신호의 내적은 0으로 나타날 것이다. 이러한 직교성을 가지
는 신호 혹은 양은 임의의 값（혹은 신호）을 표시하는 새로운 좌표축을 구성할 수 있
으며, 이러한 좌표축들이 형성하는 좌표계를 직교 좌표계라고 한다. 우리가 흔히 사
용하는 尤, y 좌표계 역시 직교 좌표계이다．
 즉 이러한 직교하는 성분들로 임의의 값을 표현할 수 있다는 것이다. 이러한 생각
들을 좀더 확장하1 간다면 임의의 신호들은 직교하는 신호들로 표현할 수 있다는 생
각을 할 수 있을 것이다. 이러한 생각에는 임의의 신호는 더 이상 나누어질 수 없는
부분， 즉 가장 기본이 되는 요소가 있다는 생각이며, 이러한 기본 요소들이 될 수 있
고 알 수 있는 판단조건이 되는 것이 직교성이라는 것이다. 이러한 기본적인 생각어］
의하써 다음 절에서 공부할 Fourier의 사고방식과 그의 정리들을 공부하도록 하자．
 다음의 그림을 통해서 직교신호로 신호를 표현하는 경우와 그렇지 않는 경우를
생각하1 보자. 임의의 신호는 직교신호로 표현되지만 이러한 직교신호는 각각어］ 가
중치를 가지고 표현될 것이다. 이러한 가중치는 단순히 상수이어야 되지 특정한 변
수（시간）의 함수가 되어서는 안 된다. 시간의 함수라는 말은 또 다른 형태（이것은
양이 될 수도 있다）로 직교성분으로 표현된다는 것이기 때문이다. 따라서 가중치는
그 직교성분 신호의 단순한 크기만을 나타내는 것이 되어야 한다.
 이러한 일반신호의 표현을 다음의 （그림 2-2）와 같이 된다고 할 수 있다．
    2. Basic Concept                                                           73
U                                                                          1




            S(t) = aA(tJ + bB(t) + cC(t) + dD(t)      (2司
            S(t) = aA(t) + bB川 +      C(t) + dD川        (2川


                                              t의 함수이므로 c(t）역시 또 다른 직교성분으
                                              로 표현될 수 있는 신호이므로 이 식에서는
                                              직교 성분이 모두 표현된 것이 아님．




                         （그림 ?2) 직교신호로 임의의 신호표현


 임의의 신호는 서로 직교하는 신호들의 선형 조합으로 구성될 수 있다는 생각을
했었다. 따라서 이러한 임의의 신호의 전력 에너지는 직교신호들 각각의 전력／어］너
지를 합한 것과 같다고 할 수 있다．
 이러한 직교성을 가지는 함수들의 종류로는 삼각함수를, 지수함수들과 통신에서
많이 사용되는 Bessel 함수, Legendre 함수 등이며, 특히 CDMA에서 논리 채널 구
분용으로 사용되는 \Vaish함수 등이 있다. Walsh함수（코드）의 직교성은 주파수를
공통으로 사용하는 CI呱4A통신에서 채널을 구분해 주는 새로운 구분자로 사용되게
하1준다．


     2.1.3 규준화（Normalization)

 사람들은 자신이 지금 처하1 있는 상태를 파악하기 위해서 다른 사람의 상태와 비
교하는 것이다. 그것은 재산이 될 수도 있고, 자식이 될 수도 있고, 힘이 될 수도 있
다. 즉 누구누구와 비교해보니 내 수준이 좋은 혹은 나쁜 수준이구나 라는 판단을
할 수 있다. 이와 비슷하게 우리가 생각하는 나아가서 일정한 값을 객관적으로 표시
하기 위한 것이 척도이다. 킬이（Length）라는 값을 객관적인 데이티로 하기 위해서
우리는 자를 사용하고 무게（혹은 질량）라는 값을 나타내기 위해서는 우리는 저울을
사용한다. 그런데 이러한 자나 저울은 그것의 표시가 특정한 량의 몇 배라는 식으로
표시퇸다. 즉 30 cm자（혹은 또 다른 종류의 자）는 1cm를 기준으로 해서 표시하며,
저울은 ig을 기준으로 해서 표시한다. 물론 더 작은 조각으로 나눌 수 있다. 이러한
조각들을 우리는 단위라고 한다．
 이러한 단위는 기준이 되는 값을 말하며, 임의의 값을 이 단위의 배수로 표현하기
위함이다. 이러한 단위는 아주 클 수 있고 작을 수도 있으며, 이 값이 작을수록 정밀
하게 혹은 하나님만이 아시는 실제 값어］ 근접한 값을 나타낼 수 있다． 이러한 것을
I     74                                2. Basic Concept
                                                           U


resolution이 좋다고도 이야기한다．
    예를 들어서 길이의 값이 17.234cm이라고 한다면 이 길이를 정확히 측정하기 위
해서는 1000분의 1cm의 단위를 가지를 자를 가지고는 17.234cm라는 것을 측정할
수 있으나, 단위가 0.1cm까지 밖어］ 없는 자라면 17.2cm로 측정할 것이다．
 이렇듯이 우리는 특정한 값을 기준이 되는 값어］ 빗대어서 표시하며 그렇게 해야
만 언제든지, 어디에서나 그 값의 객관성을 유지할 수가 있다. 이러한 특정한 값어］
기준 하여 " 몇 배"라는 식으로 표현하겠다는 생각과 방법을 규준화라고 한다. 이러
한 개념의 내용은 공학을 공부하는데 에서나 이 책의 CDMA를 공부하는데 에서나
아주 중요한 수학적 사고방식이다. 이러한 방식의 좋은 예가 dBm이라는 단위이다．
원래 dB는 상대비교의 단위인데 여기에서는 상대 비교하는 단위를 1mW로 정해두
어서 항상 사용한다. 따라서 이것은 자연스럽게 전력의 단위가 되어버렸다. 다음의
예제는 이러한 규준화의 예를 잘 보여준다．


           시골길을 걷고있는 두 명의 나그네가 맑은 가을 하늘의 깨끗한 공기
           를 마음껏 마시면서, 길가를 걷고있는데, 한 개의 긴 목재를 실은 달
           구지를 만나거］ 되었다. 이 두 사람은 이 목재의 킬이가 얼마나 될까
           하고 예상을 해봤는데, 그 중에서 수학에 흥미 있는 한 친구가 그 목
           재의 길이를 측정하는 간단한 방법을 생각하따円肛｝. 그는 자기의 평
           균보폭이 약 0.5m라는 것을 알고 있었기어］, 우선 천천히 주행하는 달
           구지진행 방향으로 쫓아가서 그 목재의 옆에서 걷기 시작했다. 140보
           가 걸렸다. 다음에는 방향을 바꾸어서 달구지의 반대방향으로 걸었는
           더］ 이번에는 목재의 옆을 컬어가는데 20보밖어］ 컬리지 않았다. 이 사
           나이는 이 두 가지 측정치로서 재목을 산출할 수 있다고 하는데, 자
           그러면 과연 재목의 길이는 얼마나 될까요9

           답은 17.5m이다. 이 문제에서 우리는 기존의 속도개념을 수정할 필요
           가 있다. 기존의 속도는 1초라는 단위로 표현하였다. 따라서 기존의
           속도는 단위시간당 이동한 거리라고 하였는데 여기에서는 사람의 한
           걷음으로 규준화한다면, 즉 1보를 걷는 시간동안 이동한 거리라는 속
           도개념으로 문제를 접해보자 그러면 그 나그네의 속도는 0.5m/1보로
    2. Basic Concept                                    75
.


               나타낼 수 있고 달구지의 속도는 x ni/i보이다. 따라서 목재의 길이는
               20(0.5 + 功과 140(0.5 - 功로 나타날 수 있으며, 여기에서 구한 x=
               3/8이다. 따라서 목재의 길이는 140(1/8）이므로 17.5m이다．



    2.2 선혐계（Linear System)

     2.2.1 함수

    세상의 많은 것들은 독립된 하나만의 속성이라기보다는 둘 혹은 그 이상의 상호
간의 관계에서 이루어진다. 이러한 관계는 사람간에도 있게 된다. 이러한 두 711 혹
은 그 이상의 변량 혹은 변수들의 관계를 규정하는 것이 함수（Function）라고 한다．
이러한 함수관계의 예로는 우리가 흔히 볼 수 있는 상거래에서도 볼 수 있다. 즉 가
게에서 과자를 사고 돈을 지불하면 주인은 과자를 건네 줄 것이다. 그러나 돈을 지
불하지 않고 그냥 가게 되면 주인은 그를 경찰어］ 신고해서 구금을 하든지 아니면
과자를 가지고 가지 못하게 할 것이다. 즉 가게주인 , 손님, 과자, 돈 등은 이러한
관계 속에서 특정한 규칙을 따르게 된다. 이러한 것이 함수의 한 예이다．
    이러한 수의 관계, 즉 함수는 수학을 통해서 체계화되고 조직화되며, 확장되어질
수 있다. 수학에서는 함수 관계가 있는 변량을 구분하는데, 그것의 값이 독립적으로
변할 수 있는 변량을 독립변량 혹은 독립변수라고 이야기하며, 이러한 독립변수에
의해서 변하게 되는 변수를 종속변수라고 한다. 따라서 함수는 이러한 독립변수와
종속변수와의 관계를 규정하는 것이다．
    대우주의 모튼 관계들은 다음과 같은 함수 관계들로 정리할 수 있을 것이다.


           종속변수           1「   독립변-I-   m1       함수여부

             1개                 1개               함수임

             1개                 다수               함수임
            다수                  1개              함수 아님

            다수                  다수              함수 아님



    이상과 같이 정리될 수 있으며, 독립변수가 여러 개일 경우는 그것이 우주어］ 존재
      76                                     2. Basic Concept
                                                                U


하는지 여부와는 관계없이 우리가 이야기하는 수학에서는 함수로 정의하지 않는다．
이러한 경우는 종속변수가 1개인 경우가 여러 개 있다고 생각하는 중첩의 정리로
생각할 수 있다. 물론 이러한 중첩의 정리가 적용되지 못하는 경우도 있을 것이다．
어찌 되었든 우리가 알고 있는 수학으로 이러한 모든 것들을 규정하려고 하는 노력
은 어쩌면 지나친 으만일 수도 있을 것이다. 아무튼 어찌 되었든 함수는 이러한 톡
립변수와 독립변수에 의해서 변하게 되는 종속변수로 이루어져 있다．
 이러한 독립변수와 종속변수의 관계가 1차 함수의 관계일 때 우리는 그러한 함수
를 선형 함수라고 한다. 이러한 선형함수의 취급은 상대적으로 비선형 함수와 비교
했을 때 상당히 간편하고 쉽게 해석할 수 있기 때문어］ 수학에서는 복잡한 함수를
단순한 선형함수로 치환（적당한 단어가 떠으르지 않으나··D 혹은 변환하는 방법틀
을 제공해 준다.
 일반적으로 함수를 표현하는 방법은 여러 가지가 있으나 가장 대표척인 경우 한
가지만을 예를 들면 독립변수 兀, y, 名어］ 의해서 변하게 되는 종속변수 F가 있다면
이러한 것의 함수 표현식은 다음과 같다．

           F= f （兀乂z)                                    (2小7)
 식 (2기과 같은 관계에서 변수간의 관계는 단순한 1, 2, 3, ···차의 관계일 수도
있고, 삼각함수나 로그함수， 미분함수의 형태일 수도 있다. 그러나 중요한 것은 이러
한 관계들을 우리가 생각하기에 쉽게 논리적으로 조직화하고 분리하여 생각하는 방법
이고 이러한 기술을 제공해주는 것이 수학의 기술들일 것이다. 이러한 가장 일반적인
해석방법은 수학에서 가장 많이 사용하는 Approx血iation괴－가정인데 이러한 방법
들은 복잡한 생각을 단순하게 풀어주고 그것을 다시 조합하는 생각을 하게 한디．.
 이 절에서 공부하는 함수의 내용은 어느 것보다 기초가 되며, 우리가 접하게 되는
수식을 수식 자체로서가 아니라 수식어］ 함축되어 있는 의미를 찾을 수 있는 방향
제시를 위해서 공부한 것이다. 다음의 예제를 통해서 배운 내용을 다시 한번 확인해
보자．


 예저I 2-2      전력（Power）은 저항과 전류와 전압의 콴계로 표시될 수 있다. 즉 전
              력 P는 （전류）2><（저항）이며, 또한（전압)2/（저항）이다. 그렇다면 전력
              은 저항어］ 비례하는 것일까 아니면 반비례하는 것일까？
    2. Basic Concept                                 77
.


               전력은 전류가 일정한 회로에서는 저항어］ 비례하고 전압이 일정한
               회로에서는 저항어］ 반비례한다. 즉 직렬회로에서는 저항이 큰 전구가
               더 밝고, 병렬회로에서는 저항이 작은 전구가 더 밝게 된다．


     2.2.2 Linear Time Invari톄t(LTI)

    선형성이라고 하는 것은 수학과 물리에서 상당히 중요한 개념이며, 우리는 이러
한 선형성이 있는 시스템을 해석하고 사용한다. 선형성의 가장 큰 특징은 중첩의 정
리이다. 즉 선형성이 있는 함수가 있다면, 그것은 나누어서 생각할 수도 있고, 그것
자체가 하나의 요소로서 구성되어 있을 수도 있다는 이야기이다．
    예를 들어서 우리가 흔히 사용하는 편미분의 경우 각각의 변수들을 각각 분리하1
서 생각할 수 있는 것은 선형함수이기 때문어］ 그러하다．
    가격이 일정한 상품, 예를 들면 1권어］ 500원하는 노트가 있다. 이때, 구입하는 노
트의 권수를 兀, 가격을 y라 하면 兀와 y는 서로 함수관계가 성립하게 되며,
y= 50뇨로 표시할 수 있다. 또한 철수가 구입한 노트의 권수를 兀l라하고, 순희가
구입한 노트의 권수를 尤2라 하면 두 사람이 구입한 노트의 수는 兀l+ 抑가 된다. 이
어］ 대한 금액은 只兀l＋兀2)로 나타낼 수 있다. 이것은 각각의 금액 /（兀l), f (x2)의
합과 같다면 그것은 선형인 것이다. 물론 다를 수도 있을 것이다．
    또한 5사람이 노트를 각각 尤권을 구입할 때의 금액은 人缸）이지만, 이것은 한 사
람의 금액 人功의 5배와 같다면 이것 또한 선형임을 나타내는 속성이 된다. 즉 중첩
의 성질이 있는 것이다．
    앞서 말한 바와 같이 이러한 선형성을 나타내는 함수들은 각각의 요소를 가지고
있는 함수로서 역시 선형이다．
    다음은 문구점 제품들의 카탈로그의 일부라고 하자.

轟艱融聽難疑烈瀜珌難轟難
                       恁毖峀꾜1 1 공책      연필     스커匡浩千

         가격                  500원      200원   1000원

         무게                   20g      15g     40g


    이 문구점에는 공책이 自권, 연필이 兀2자루 그리고 스케치북이 抑권 있다고 할
때, 이것의 전체가격을 Yi, 전체무게를 Y2라고 한다면, 이것의 무게와 가격은 다음
과 같이 각각 쓸 수 있다．
1   78                                                            2. Basic Concept
                                                                                     1


         乂 = 500직 + 200毛 +1000兀3
         兀 = 20工l +15石 +40兀

 위 2개의 식은 각각의 경우에 사용된 변수간어］ 각각 선형성을 가지고 있다. 또한
이 2개의 식은 각각 또 다른 선형함수의 요소들이 되는 것이다. 즉 이것을 행렬로
표시하면 다음과 갇다．

                                                             兀l
         [
             '1
                  =        [500
                                           200    10001
                                                             工2               (2-8)
         [y2]              [20             15          40]
                                                             工3



 따라서 위와 같은 행렬은 선형함수를 표시하는 전형적인 수학의 형태이며, 따라
서 선형대수라는 이야기를 한다．


                  Y＝兀＋2尤2＋尤3인 함수는 선형인가 비선형인가9

                  위의 식을 다시 표현하면 다음과 같이 표현할 수 있다. 즉 y는 尤，                                 ,
                  尤3와 각각 선형의 관계어］ 있으며, 따라서 이러한 선형의 식의 합 또한
                  선형일 것이다. 이러한 관계는 다음 식에서 더욱 명백하게 나타난다．

                                                 1」
                  「」「 2 ii]
                                                  ［x
                  [
                      y]
                                  =
                                  ＝
                                      [i
                                                                             (2-9)
                                                       工3
                                                       x2x


 이러한 선형성은 우리가 시스템을 해석하는 데어］ 상당히 중요하며, 우리가 흔히
수학에서 선형대수를 공부하는 것은 복잡한 식을（혹은 시스템）을 간단하게 선형의
식으로 （혹은 시스템）으로 분리하여 생각하기 위해서이다. 앞서 이야기한 Fourier의
생각과도 비슷하다．
 이러한 선형성은 물리적 채널에 대한 제한적 채녈 모델에서 가장 일반척으로 사
용되는 개념이며, 이것은 시 불변 조컨과 함께 생각되고 고려된다．
 선형성이라는 것은 시스템의 상태를 나타내는 것으로 시간어］ 대해서 변화되지 않
는다는 혹은 변한다는 시간적인 요소가 없었다. 즉 상태 혹은 현상 그 자체의 특성
을 말하는 것이다. 우리가 시스템을 분석할 때에는 시간적인 요인도 고려할 때가 생
길 것이다. 앞의 예에서 공책값이 시간이 지나, 즉 내일은 550워으로 변했다던가 하
    2. Basic Concept                                                     79
U


는 식을 말하는 것이다．
 이러한 시 불변성을 생각할 때 우리는 선형 시 불변 연속 시스템（Linear Time
Invariant Continuous System)과 선형 시 불변 이산 시스템（L岫ar Shift
Invariant I玉screte System)으로 나누어서 생각할 수 있다. 여기에서는 디지털 신
호의 해석을 위한 것에 대해서 이야기하기 위해서 시작한 이야기이므로 이산 시스
템에 대해서만 이야기하겠다．



                          입력                선 형 시스템
                                                         >
                          x(t)                  h(t)   W卞x（少！i(t)


                                       （그림 ?3) L기 필터


 일반적으로 LTI필터의 입출력 관계는 （그림 2-3）의 형태가 전형적이라 할 수 있
다. 선형시 불변 연속 시스템（L岫arTin肥-Invariant Continuous System)에서의
출력은 잘 알고 있는 것과 같이 입력신호와 임펄스 응답과의 Convolution어］ 의해서
구해질 것이다. 그러나 선형 시 불변 이산 시스템 (Linear Shift-Invariant Discrete
System)에서는 그것의 출력 시퀀스는 입력 시퀀스와 임펄스 응답과의 Convolution
합으로 표현되어야 할 것이다. 이산 시스템에서 인자들의 개수가 유한 개이면 그것
의 선형 필터는 FIR(Finite 임펄스 Response) 시스템이 되고                           무한 개이면 h1R
(Infinite 임펄스 Response) 시스템이라고 한다．
 이러한 선형 시 불변 시스템은 시간 영역에서 시간의 변화가 전혀 없는 임펄스를
입력으로 가했을 때 얻어지는 출력응답을 낸다고 볼 수 있다. 앞서 이야기했듯이 선
형 시스템은 시간의 흐름과는 무관하게 생각되어야 하기 때문어］ 그러하다. 이렇게
함으로 시간이 배제된 시스템의 상태 특성만을 얻을 수 있기 때문이다. 여기에서 임
펄스는 출력은 있으되 그것의 출력을 표현하는 시간이 없는 관념적인 값이다. 그러
므로 선형 시스템의 특성을 시간 영역에서 찾기 위해서는 필터함수 [[ x(t月이 다음
과 같을 때 구할 수 있다.

           y(t) = L[x(t)]. (,)=.(f) = L[S(t)]= h(t)                      (2-10)

 주파수 공간에서는 당연히 /z( t)의 Fourier 변환 값인 H(f）일 것이다．
    선형시 불변 이산 시스템을 정리하면 다음과 같이 정리할 수 있다．
I         80                                                               2. Basic Concept
                                                                                              .



      y(t) =L[ a尤(t)]
      y( /) = L[ 口1尤1 + 口2兀2]                           중첩의 정리
      y(t- t0) =L{ a兀(t- t0)]                           Time Invariant


 이상과 같이 표기한 것은 Time Invariant 개념까지 포함한 표현이기에 그러하다．
 즉 시간이 지난다 해도 시간어］ 의해서 그것의 값이 변화하지 않는 것을 말한다．
즉 이제 시간의 개념이 도입되는 것이다. 시간이 전체적인 시스템의 특성을 변화시
켜서는 되지 않는다는 말이다. 이러한 의미에서 사람(human）은 나이가 들면 늙는
다는 관점에서 Time Invariant 시스템은 아니라고 할 수 있다．



    2.3    Fouri아의 신호분석


     2.3.1 Fourier의 생각

 신호를 표현하는 방법에는 신호를 시간상에서 표현하는 시간 영역 표현과 주파수
상에서 표현하는 주파수 영역 표현이 있다. 두 표현 방법은 동등하며 단지 갇은 신
호를 다른 관점에서 관찰하는 것이다. 즉 동일한 신호를 Oscillosc야光를 통해서 관
찰하면 시간 영역으로 나타내는 것이며, 스펙트럼 분석기를 통해서 관찰하면 주파
수 영역으로 나타내는 것이다. 중요한 것은 용도어］ 맞게 효율적인 표현 방법에서 다
른 표현 방법으로 변환이 가능하며 이를 Fourier 해석이라 한다．
 프랑스의 수학자 Fourier의 생각은 " 세상의 복잡한 것은 단순한 것들의 합들로
구성될 수 있다"는 것이다. 여기에서 단순한 것들이란 그것만의 고유한 특성을 가지
는 것들, 즉 다른 단순한 것들과는 완벽하게 구별되는 또 다른 말로써 Orthogonal
한 특성을 가지는 것이라고 생각할 수 있다．



                          /     +.
                                      ．斗   寸．
                                                .   \
                                        + J. + 기 + ir + i如 + 文 +     j   + 표三



                                     （그림 2-4) Fourier의 섕각
    2. Basic Concept                           81
1

 이러한 개념은 우리가 사용하는 언어에서도 적용해서 알 수 있다. 즉 한글에서 자
음 14개와 모음 10개는 서로 독립적이며, 그것들 하나하나는 다른 부호어］ 비해서 구
분되는 그들만의 정체성이 있다. 우리가 흔히 사용하는 언어는 이러한 근본 요소들
의 조합으로 이루어진다. 이러한 관점에서 세종대왕과 Fourier는（비단 이 두 사람뿐
은 아니지만）같은 생각을 했던 것이다．
 이러한 Fourier의 생각이 좀더 구체화되고 정형화되어서 새로운 수학이론이 나오
게 되었으며, 이것은 공학에서는 신호의 스펙트럼 븐석어］ 사용되는 가장 기본이 되
는 정리되었다．


     2.3.2 Fourier Spectrum

 Fourier의 이러한 생각은 신호해석에도 적용되었다. 물론 그 당시는 신호개념이
아니라 수학의 sine과 cosine함수이었을 것이다. 어찌 되었튼 Fourier는 아주 복
잡한 신호도 기본이 되는 서로 Orthogonal한 신호의 단순한 합으로 구성되어 있
다고 생각하였다. 때문어］ Fourier는 일반적인 주기함수를 식 (2-11）과 같이 생각
하였다．

           f (t) =A0+ ZA,,sinno万+ZB,cosno茗      (2-11)
                       ?1=l    , =1



          叩／zere 只t) : periodic 加冗加n(T)

 결국 신호 /(t)는 A0, An, Bn를 계수로 가지는 성분들로 구분퇸다고 할 수 있
다. 각각의 성분들은 우리가 알고 있는 주기신호 ／佃를 적분하는 과정에서 구할 수
있었다. 즉 凡）를 한 주기 동안 적분하면, 교류성분인 S加과 cos항은 모두 '0'이 된
다. 즉 이 식으로부터 A0를 구할 수 있다. A0는 수학적으로는 상수이며, 전기적으
로는 직류성분이다. 직류성분은 파형을 한 주기 적분하여 평균했을 때 '0'이 안 되는
경우어］ 존재하는 성븐임을 알 수 있다. 또한 A , 을 구하려면, 식 (2-11）의 양변어］
S勿in毗를 곱하고 한 주기 적분하면（다음에 이야기되겠으나 sinn口比를 곱한다는 말
은 S勿in毗성분과 Orthogonal한 모든 항목은 없어지게 하기 위함이다．) 식 (2-11）의
우변에서 S加2刃毗가 되는 경우에만 한 주기 적분했을 때 '0'이 안 되고 나머지 경우
에는 모두 '0'이 되기 때문이다. B, 도 갇은 방법으로 구할 수 있다. 이러한 결과는
다음과 같다．
      82                                                                                                   2. Basic Concept
                                                                                                                                                   1



           나ff (t)dt
                 A=;rf(t)sinn毗dt,B=;rf（加.Sn毗dt                                                                                                (2-12)


 앞의 식 (2-12）에서 S加항과 cos항을 지수함수로 표시하여 정리하여 표시하면 식
(2-13）과 같이 된다．

                f (t)=F;+2F,ea+2尸，em =2F,e""아                                                                                                 (2-13)
                                    n놔                        ／了＝l                        n＝ 小




           F;＝凡

            心｛
                    [B,
                              山A,
                                             ],
                                                         尸戶｛              [B，
                                                                                    幻Aj
 식 口13）에서 급수 F刃은 양변에 可j"回t를 곱하고 1주기 동안 정적분 하여 구할
수 있다．


           肛｝
                    丘／(t）                可
                                                  "' "
                                                   ‘
                                                         d7
                                                                                                                                              (2-14)


 식 口14）에서 F , 은 변수 t어］ 관해서 정적분하여 구한 것이므로 加의 함수이다．
즉 주파수의 함수이다. 즉 스펙트럼의 크기 성분은 주파수어］ 따라서 그 크기가 다르
거］ 나타날 수 있다는 이야기이며, 이것은 해당신호가 여러 가지 고조파 성분을 가지
고 있는테 그것의 각 고조파들의 크기 성분이 각각 다르다는 것이다. 마치 한 아버
지 슬하어］ 여러 명의 자녀가 각각 다르듯이

                              月t)



                                         TH
                          A




                                                                                                 ]
                              十卞
                                                                                                                         也T



  켜                                                                  t>
                                                                                4                                    1
                                                                                                                         尸
                                                                                                                         1        i
                                                                                                                                      1
                                                                                                                                          ;
                                                                                                                 1
                                                                                                                              瓦
                                                                                                             1
                                                                                                     (b)

                              （그림 ?5) 주기 구형파의 Fourier Spectrum
         2. Basic Concept                                 83
     .


         지금 Fourier 스펙트럼의 응용의 예로서 （그림 2-5）와 같이 주기 T를 가진 펄스
파형의 경우를 생각해 보기로 하자．
         먼저 식 (2-4)으로F, 을 구하고 이 F, 을 식 (2-14）어］ 대입하면 주기적인 구형파
의 恥urier 스펙트럼을 나타낼 수 있다. 즉 식 (2-15）과 갇이 된다．

                       ＝갸，M切夕回帥/2)1                       (2-15)
                            T ""j   T [- nw。
                                           r12   j
                          2ir
                       n兀＝;

         식 口15）의 F, 은 시간 t어］ 관하여 정적분 하여 얻은 값이므로 n口加의 함수가
되며, 이 값을 통해서 폭이 V이고 주기가 T인 주기 구형파는 그것의 스펙트럼의
크기가 sin과 유사한 형태로 나타남을 알 수 있다. 여기에서 F, 은 주파수를 나타내
는 함수라고 생각할 수 있으며, 다시 말하면 只t)의 주파수 해석이라고 할 수 있다．
         식 (2-1히에서 구한 凡（na)o)의 값을 식 (2-13）어］ 대입하면 식 口16）과 같은 결
과가 된다. 또한 그 결과는 （그림 2-5）의 우측 그림과 같다.


               肛如따'"'"무斗"써'}J                             (2-16)


         이상의 식 (2-15）와 식 (2-16）를 통해서 위의 （그림 2-5）의 (a）어］ 나타난 주기 펄
스열의 경우 주차수 영역을 대변해 주는 F, 어］ 의해서 고찰할 때 주파수 영역에서
무한히 많은 고조파 성분을 가지고 있음을 알 수 있다. 이 내용은 주기함수의
Fourier 변환과 나아가서 표본화 이론을 공부하면서 좀더 상세히 생각하1 보자．

          2.3.3 Fourier Transform

         앞의 （그림 2-5）어］서 구형파의 주기 T를 무한대로 킬게 하면, 좌표의 중앙에 있
는 구형파 하나만 존재하게 되며, 이때 그림（b）에서는 스펙트럼간의 간격 스回는
     dw가 되어 0에 근접하게 퇸다. 따라서 이산적으로 존재하던 스펙트럼이 연속적으
로 존재하게 되며, 이때 스펙트럼의 포락선의 변화는 생기지 않는다. 이상과 갇이
주기적인 파형에서 주기가 무한대가 되면, 주파수 스펙트럼 F,( n帥는 F, ( 回）가 된
다．
   84                                                   2. Basic Concept
                                                                           .


 식 口14）을 식 口13）어］ 대입하고 T가 무한대라는 조건을 넣으면 식 口-17）은
다음과 같이 다시 쓸 수 있다．
                m r ] T         그
         /('）
           『二［祛f(t) e_"0tdt]e""                                   口‘「）
 주기가 무한대인 비 주기 함수이므로 T가 무한히 커진다. 따라서 적분구간과 각
각의 인자들은 다음과 같이 고쳐 써야 한다．

        uirn二＝可, 丘 -4二 , 已L
 또한 이산적인 값들도 연속적인 값으로 표시되어지므로 可j"凹t 및 可／"毗는
e -i"叫악 可jnwt로 바뀌게 된다. 이러한 결과를 식 口17）어］ 대입하면 식 口18）과
같이 된다．

        f(t)=f吐肛m小mft e_.0h1寸"可                                    (2-18)


 식 (2-미에서 괄호 안은 시간 ／어］ 관해서 정적분하였으므로 이 정적분 치는 (1)만
의 함수인 只功가 된다. 즉口-19）과 口그0）은 같아진다．


                   "a．再
        f (t) =1臂．繭7
                                      ：卜
                                           rr｛山It卜 }n
                                                                    (2- 19)


        F(o)) = ff (t) e1'tdf                                      (2- 20)
 식 口19）은 시간 ／의 함수 凡）를 주파수 口J의 함수 只帥로 변환시키는 식으로
서 Fourier 변환이라고 한다. 또 口20）은 (.0의 함수只功를 t의 함수 犬t)로 변환
시키는 식으로서 Fourier 역 변환이라고 한다. 그렇다 Fourier 변환은 Fourier 스펙
트럼의 주파수에 대한 극한값이라고 말할 수 있다. 다음과 갇이


     Fourier Transform = urn Fourier Spectrum
                                    a나O


 원래 모든 파형은 변수 t와 (0를 포함하고 있는 함수이므로 0)어］ 관해서 정적분하
면 t만의 함수가 되고 t로 정적분하면 C,)만의 함수가 된다. 따라서 임의의 함수의
／佃를 알면 F佃）를 구할 수 있고 반대로只帥를 알면 ／佃를 구할 수 있다. 이
    2. Basic Concept
I

Fourier 변환식은 앞으로 우리가 공부할 모든 부분에서 상당한 위치를 차지하게 될
것이다. 때문어］ 열심히 그리고 정확히 알아야 한다．
    이러한 Fourier 변환이 존재하려면 다음과 같은 절대 적분 가능조컨이 만족해야
한다．

           （태曲的
          亡／                                     口21)

    그러나 이러한 조건은 Fourier 변환이 존재할 필요충분 조건이 아니라 충분 조컨
이다. 따라서 함수 /(t)이 절대적분 조건을 만족하면 Fourier 변환이 존재한다고 할
수 있으나, Fourier 변환이 존재하는 ／佃는 절대 적분가능 조건을 만족한다고는 할
수 없다. 이것은 뒤어］ 공부하게 되겠지만 주기함수의 Fourier 변환은 극한에서
Fourier 변환이 가능하기도 한다. 또한 반대로 임펄스 함수의 경우도 절대 적분가능
조건을 만족하지 않으나 Fourier 변환은 존재한다．
    Fourier 변환은 일반적으로 직관적이라고 할 수 있는（물론 여기어］ 대한 정의는
필자의 주관적인 의견이다） 시간 영역에서의 관점을 주파수 영역의 관점으로 확대
해서 해석할 수 있게 하1 주며, 이러한 것은 신호해석에서 또 다른 물리량인 주파수
를 우리의 사고（思考） 속으로 포함시키게 하1 주는 결과를 가져온다．
    식 (2-19）과 식 (2口이에서 생각해 볼 때 시간 영역과 주파수 영역으로 변환시켜
주는 변환자가 e jwt와 可j毗이라는 것어］ 주의해 볼 필요가 있다．
    시간 영역의 신호를 주파수 영역에서의 해석하기（그 자신의 주파수 영역의 모습
을 보기） 위해서 우리는 Fourier 변화을 통해서 할 수 있다는 것을 공부했다. 그런데
이러한 Fourier 변환 식 (2-19）과 식 (2-20）은 앞서서 공부한 상관성을 나타내는 식
으로 볼 수 있다. 즉 시간 영역에서 표시된 신호를 주파수 영역으로 변환하여 표시




               ；轟 乍 III
                       2
                    (k二；
                            III
                (
                           （그림 ?6) 주파수와 시간의 장벽
   86                                   2. Basic Concept
                                                           U


할 때는 해당신호를 eM와 상관성을 계산한 값이 되고, 주파수 영역에서 표시퇸 신
호를 시간 영역으로 변환하여 표시할 때는 해당 신호를 可jwt와 상콴성을 계산한
값이 시간 영역에서의 그 신호의 모습이 된다. 이러한 생각에서 우리는 시간 영역과
주파수 영역을 구분해 주는 e jwt라는 거울을 생각할 수 있다. 시간 영역의 임의의
신호가 자신의 주파수 영역의 신호를 보고 싶을 때는 이 거울을 통해서 주파수 영역
의 자신을 볼 수 있을 것이다. 이것의 역의 경우도 마찬가지이다. 즉 신호의 Fourier
변화은 e '毗라는 거욱2）어］ 보여지는 모습이라고 할 수 있다.


 비 주기 구형파의 Fourier 변환
 앞의 （그림 2-5）의 (a）에서 구형파가 하나만 존재하고 주기가 전혀 없다고 할 때
이 파형의 Fourier 변환어］ 대해서 생각하1 보자. 이러한 파형의 Fourier 변환은 비
주기 함수의 그것에 비해서 훨씬 간단하게 구해질 수 있다．
 앞서 이야기한 Fourier 변환 식 (2-10）에 의해서 Fourier 변환을 구하면 다음과
같이 구할 수 있다. 즉

            /2 加和小孕 ' .巴｛H／呼｛)
        F回＝._il
            ! /2        JW\    )

           =A Si
             r"呼．父，rSa(擘)                          (2- 22)
                   呼2
 이 식은 앞의 주기 구형파의 스펙트럼과 비슷하게 나타난다. 그러나 이것의
Fourier 변환은 스펙트럼과 같이 이산적인 값이 아니라 연속적인 밴드로 형성퇸다．
이것은 T가 무한히 커지므로 rAfT가 0과 같이 되어 스펙트럼 함수 아니 Fourier
변환이 연속적인 함수가 되기 때문이다. 즉 여기에서는 모튼 주파수가 기본 주파수
가 된다는 이야기가 되며, 이러한 비 주기 함수는 모든 주파수 스펙트럼이 아니라
대역을 가진다는 이야기이다．




2) 필자가 이것을 거울이라고 표현했으나 창이라고 생각할 수도 있다. 그러나 필자가 굳이
   거울이라고 하는 이유는 자신의 모습이 비쳐진다는 의미에서이며, 이것은 비쳐지는 모습
   이나 비추는 그것이 같은 객체임을 강조하고 싶어서 이니 독자들은 그것의 의미를 다시
   한번 생각하1 보기 바란다．
    2. Basic Concept                                             87
.



          함수
    이상적인 콘덴서 C에 전압 V가 인가되었을 때 콘텐서에 흐르는 전류 1는 다음과
같이 표시된다는 것을 우리는 회로 이론 시간에 배워서 잘 알고 있을 것이다．

          i= C史                                                  (2- 23)
              dt

    그런데 전압 V가 이상척인 단위 계단함수 u(t）라고 한다면 콘뎬서어］ 흐르는 전류
1는 片0에서는 너무나 큰 값이어서 불확정적이며, t= 0이외에서는 모두 0이 된다．


               u(t)                                Ur(t)




                            (a)
                                                           (b)




                            (C)                            (d)

                                  （그림 ?7) 임펄스 함수의 설명


    그러나 （그림 2-7）의 (b）와 같이 이상적이지 않은 단위 계단파 Ur( I）가 콘텐서어］
인가되었다면 콘덴서의 전류는 (d）와 같이 형성될 것이다. 여기에서 a를 0에 무한히
근접시킨다면 町t)는 u(t)와 같아질 것이다. 이 미분치（전류）는 높이가 1／口이고
폭이 口인 단형 펄스파가 되는데 口가 0에 근접함에 따라서 펄스의 폭은 무한히 좁
아지고 단형파의 면적은 유한한 값（r1）이므로 높이는 무한히 커진다．
    앞서 이야기한대로 단위 계단함수 u(t)의 미분이 존재하지 않으므로 단위 o1그'터 /\
                                                 a=H

함수 m）는 다음과 같이 극한으로 정의할 수 있다．

           ..     . d r . . = . . L. .
          O(t) = lirn- --Iu,(t)j = llm- tu(t) - u(t- a)]         (2- 24)
                  十川'at             n+U (i

    이 식에서 (7를 무한히 영어］ 근접시키면 mt)는 높이가 무한대이고 폭이 0인 펄스
   88                                                          2. Basic Concept
                                                                                  U


의 형태로 나타낼 수 있다．

        fs (t)dt=1
        8(t) =0      r才0


   2.3.4 Fourier 변환의 성질

   （기 주파수 천이성

 주파수 천이성이란 주파수 영역에서 주파수 천이한 스펙트럼어］ 대응하는 시간 영
역 신호는 원래의 신호가 위상만 변경퇸 신호가 된다는 것이다. 이것은 시간 천이성
과는 상대성원리와 같은 것으로 시간 영역이나 주파수 영역에서，
 만약어］ 人勿의 Fourier 변환이 F（回）라고 한다면 /(t)e1"t의 Fourier 변환은 어떻
게 되는지를 생각하1 보자. 즉 ／。{sec］나 w。[ra可sec］만큼 천이하게 되면 각각의 위
상이 (H 岫）[rad］이나 ( wt。)[rad］만큼 변하게 된다. 이러한 Fourier 변환의 주파
수 천이성은 통신에서 상당히 유용한 성질이다．

        S[/(r)e'""' ] =Ff (t)eJ0301e "' 'tdt = f f (t)e_i(o田0)tdt = F(w -w) (2-25)
 주파수 영역에서 回0만큼 이동한 것은 시간 영역에서 e '聊를 곱한 것과 같다. 시
간 영역에서 인자 e毗를 곱해 주면 주파수 스펙트럼 F（功가 만큼CO0 이동한 것이
되므로 이 정리를 주파수 천이 정리라고 한다. 통신 시스템에서 주파수 스펙트럼을
이동시킬 필요가 있다. 이와 같은 주파수 천이 과정을 변조라고 한다．

   (2) 시간 천이성

 Fourier 변환의 시간 천이성이란 시간 영역에서 시간 천이한 파형의 스펙트럼은
다음과 같이 원래 파형의 스펙트럼과 비교하여 진폭 스펙트럼은 동일하고 위상 스
펙트럼만 변환한다는 것이다. 시간 영역에서 ／。[sec］만큼 천이된 파형 /t- t0）는
／佃와 비교하여 신호의 모양이 변하지 않았으므로 人펙트럼의 크기는 변하지 않고，
시간 지연에 따라 위상이 ( H口斤0）만큼 변하게 된다．
 만약어］ 只勿의 Fot끄ier Transform이 F(力라고 한다면 只t- to）의 Fourier
Transf이m는 어떻게 되는지를 생각하1 보자. 즉
    2. Basic Concept                                        89
1


         3[f (t -t。
                  )] = ff (t -t。
                               )e1'tdt
    여기에서 (t- t0)＝兀라고 할 때，

          S[/(r - t。)] = f f (x)eJ (" '0)dx = F(tO)e '"아0   (2-26)
    이 정리의 의미는 ／佃의 신호가 어떤 시스템을 통과할 때 통과시간이 片 t, 초 걸
렸다면 이 人0신호의 크기（II追gn孔ude) 스펙트럼 IF佃기는 변화가 없고 위상 스펙
트럼만 늦어지게 된다는 결과가 된다는 것이다. 이것은 凡）가 가지고 있는 각 주파
수 성분이 이 시스템을 통과하는 시간이 다 같이 to이고 이 시스템을 통과할 때 감
쇠가 일어나지 않음을 의미한다. 다시 말하囚 시간 영역에서의 to의 천이는 주파수

영역에서 e -jw0t를 곱한 것, 즉 위상정보만 변한 것으로 나타난다．


      (3) Convolution

    만약어］ 月（/）의 Fourier Transform이 玎功이고 月（/）의 Fourier Transform이
戶20功이라고 한다면 F1回凡（口D는 시간 영역에서 어떻게 표현되겠는가를 생각
해 보자．

         且（w)戶；(0))=L工（r)e '"毗dr 1;(o)=Lf (r）戶；(a)e '"毗dr
    여기어］서 凡佃e - jw0t는 식 口26）어］ 의해서 /b(rmr）가 된다. 즉

          且（n))F;(m)＝二工（T)f (t -r)dr＝工（t) * J如）             아27)

    식 (2-27）은 시간의 Convo뇨lion으로 정의할 수 있다. 즉 주파수 영역에서의 곱
하기 연산은 시간 영역에서의 Convolution의 형태의 연산자로 새롭게 표현될 수 있
다. 그러므로 우리는 여기에서 또 다른 연산자인 （允fly이玭如n을 다음과 같이 정의
할 수 있다．

          f1(t)* f2(t) 三 ff (r)f2(t-r)dr
          3[J,(t)* f2(t)]= F (c))I,(o力                      (2- 28)


    이것은 마치 초등학교 1학년에 입학하여 덧셈과 뺄셈을 배워서 한창 " +", " h"를
    90                                                             2. Basic Concept
            1                                                                         U


셈하던 학생들이 2학년으로 진급하여 구구단을 외우며 처음으로 곱셈을 대하게 되
던 때와 동일한 경우이다. 즉 우리는 Fourier를 통해서 기존의 시간 영역에서 벗어
나서 주파수 영역으로의 사고의 영역이 확대되었으며, 이러한 가운데 새로운 연산
자인 Convolution을 알게 되었다. 앞으로 계속 이야기가 될 것이며 이 Convolution
을 통신에서는 상당히 유용한 연산자이며 여러 븐야에서 많이 사용된 것이다．
 어떤 함수 ／佃와 임펄스（단위 충격함수） 知）와 의 Convolution은 그 함수 자체
가 된다. 즉 (2口이에서 보는 바와 같이 /(t)와 的）의 Convolution의 결콰는 r= t
일 때 凡）는 출력이 있으므로 결국 ／佃가 되는 것이다．

         f (t)站(t) =ff    (r滔小r)d丁＝八t)                                        仁29)

 즉 임펄스는 Coi싸아ution 연산의 항등원이 된다． 이러한 관계들에서 우리는 다음
의 관계를 알 수 있다．

         f (t) *S(t_ T) =f (t- T)                                           (2-30a)
         f (t叱少하t - t2) = f （卜tl叫）                                          仁30b)
         S(t- t1) *8(t -t2) = S(t -t _t)                                    (2-30c)

 일반적으로 주파수 응답을 가질 수 있는 시스템은 크거］ 필터와 변조로 그것의 특
성을 대변할 수 있다. 이것들의 차이는 소스 데이터와 전달 함수간어］ 시간 영역 혹
은 주파수 영역에서 곱하기 연산 혹은 Convolution으로 출력을 얻을 것이냐는 것으
로 구분할 수 있다．

                s(t)
                         可t)             肛J    丹t) ＝計t) .可t) :Modulation


                s(t)
                         可t)
                                         (t)
                                               只t) = 可t戶可t) : Filtering
                                    卜／
                          （그림 ?8) 다旭口FModu囹ion


 즉 시간 영역에서 곱하기 연산어］ 의한 출력값은 변조라고 할 수 있고, Convolution
연산의 결과는 필터라고 할 수 있다．
    2. Basic Concept
U                                                        1   91



     2.3.5 지수함수 e '口『의 Fourier 변환

 지수함수 e 3w0t를 oo<t＜아）의 시간구간어］ 대하여 Fourier 변환을 생각하1 보자．
지금 지수함수 e 1w0t를 정현파로 표시하면 다음과 같다．

         e"0t =cosojt+ jsinwt

 따라서 이것을 Fourier 변환하면，
         斗니
          "日[ cos毗＋州nw月
                 =i[S(w- w。)+S(w+ w)-a(w+co) +S(w- w)}
                 =2,rS(w- w。)

 그러므로 e'山의 Fourier 변환은 凹＝回0에서 강도가 2兀인 임펄스임을 알 수 있

다. 여기서 주의할 것은 e1W0t의 신호는 시간의 실함수가 아니기 때문에 a) = a)0에서
만 스펙트럼이 존재한다는 것이다．


     2.3.6 주기함수의 Fourier 변환

 앞서서 설명한 바와 같이 Fourier 변환은 Fourier 급수에서 주기함수 /(t)의 주
기를 무한대로 극한을 취하여 구하였다. 여기서는 반대로 Fourier 변환의 특별한 경
우가 Fourier 급수가 된다는 것을 증명하겠다. 이와 같은 사고방식은 주기함수와 비
주기함수를 통합하여 취급하는데 아주 편리하다．
 엄밀히 말하면 주기함수는 모든 구간에서의 적분값이 유한하지 않으므로 Fourier
변환이 가능하지 않다. 그러나 이 경우에도 Fourier 변환은 극한개념을 통하여 얻을
수 있다. 다시 말해서 먼저 주기함수가 유한한 구간 ( T/2 - T/2 ）에서 존재한다고
가정하고 T를 무한대로 극한을 취하여 구할 수 있다．
 한편 주기함수는 Fourier 급수로 표시할 수 있으므로 주기함수의 Fourier 변환은
Fourier 급수의 각각의 성분을 각각 Fourier 변환하여 합하여도 구할 수 있을 것이
다. 주기가 T인 함수 /(t)는 다음과 같이 표시할 수 있다.

            ）＝흐F,d4나叱却，'
          /（》   n＝寸 \           I   /


 이 식의 양변을 Fourier 변환을 하면，
   92                                      2. Basic Concept
                                                              N




        F(o.)=SD0)]=S［츠Ed'""］這四e"' )
가 된다. 이 식은 다시 지수함수 e7硏의 Fourier 변환을 이용하여 다음과 같이 다시
쓸 수 있다．

        F(co) =3[f (t)}=2irZF S(o- nco。)              (2-31)

 이 식은 매우 중요하다. 위의 결과식을 보면 주기함수의 Fourier 변환, 다시 말해
서 이 함수의 스펙트럼 밀도 함수（SI玘ctral De的ty Function) F, 는 신호의 고조
파에 존재하는 임펄스들로 구성되어 있으며, 각 임펄스의 크기는 Fourier 급수의 각
해당 급수의 2,r바1 한 것과 같음을 알 수 있다．
 우리는 여기에서 독립된 신호, 즉 비 주기 신호의 경우 Fourier 변환은 주파수의
연속함수 이나 주기함수 /(t)의 경우 주파수 영역에서 이산적인 함수로 나타난다는
것이다. 이러한 결과는 주기함수 자체가 이산적으로 존재하는 고조파의 주파수 성
분을 가지고 있음을 나타내는 결과라고 할 수 있다．
 아주 관념적인 이야기가 될 수 있는데, 주기함수라는 것은 시간의 개념이 고려된
함수이고, 비 주기 함수라는 것은 그렇지 않다는 것이다. 다시 말해서 주기함수의
경우 시간어］ 의해서 규정되어지는 함수이므로 신호 자체가 불연속일 수는 있으나
（신호가 불연속 구간은 Fourier 변환을 할 수 없다） 그 신호의 표현은 시간적으로
연속적이다（즉 시간이 흐르고 있는 상태의 함수）. 그러나 비 주기 함수는 그것어］ 대
한 시간적인 의미는 없으며, 단지 그 상황인 것뿐이다. 이러한 것의 예로는 움직임
있는 사람에게는 그것의 시간이라는 개념이 있으나 사진 속의 사람의 경우 시간이
아니라 상태밖에는 없는 것이다．
 이러한 이유에서 주기함수의 Fourier 변환은 주파수 영역에서는 불연속적으로 나
타날 것이며, 비 주기 함수는 주파수어］ 연속적인 함수로 표현되어지는 것이다．

 Zero Crossing 대역폭
 즉 주기함수의 Fourier 변환을 구하기 위해서는 우선 식 (2-4)을 이용하여 F（功
을 구하고 이렇게 구한 只功은 식 (2-16）어］ 대입되면 결과적으로 Fourier 스펙트
럼의 계수들이 임펄스로 나타나게 된다．
    2. Basic Concept
口                                                                               93


 여기에서 우리는 새로운 사실을 확인하기 위해서 （그림 2-5）와 같이 폭이 t이고
주기가 T인 주기함수 人t)의 Fourier 변확을 생각하1 보자. 이때 （그림 2-5）의
F（功은 식 (2旬와 갇이 표현할 수 있다．
          ,, .   .     Ai ... (n2rr\        -         戶 , ,    sinx
         it (72nt } = =1中H）미 1         1   w九ere      ia（工） == 1
                       I    \ I    )                               兀

 이것을 식 口31）어］ 대입하면 주기함수 人t)의 Fourier 변환은 다음과 갇다．


          F(w)=2끈｝
                -I
                      蜘呼）
                   ' .＝小 \ 1 )
                               6(m-.mb)                                         (2-32)
 따라서 이 함수의 Fourier 변환은 주파수가 0인 DC를 비롯하여, 士 m0, 士2wo,
··· 士／I口J0, ··· 등어］ 존재하는 임펄스로 구성되어 있으며, "W= nO)0"에 존재하는 임

펄스의 크기는 27r(ArT)S口（n7rrT)로 주어짐을 알 수 있다. 이것은（그림 2-5）의 (b）와

긷미 나타나게 되며, 이것은 펄스 폭 t와 주기 T어］ 의해서 새로운 고찰이 있을 수 있다．

                                                j7n




                                       \
                                                                       0)


                            4+              나                               V
                             （까7

                            （그림 ?9) 디지털 신호의 대역폭



 （그림 2-9）와 갇이 식 口32）의 결과를 표시할 수 있으며, BW와Am를 표시할
수 있다. 이 값들은 결국 V오｝ T에 의해서 변동될 수 있다．
    V는 변하지 않고 T가 증가한다면 첫 번째 zero crossing은 불변이지만, 스펙트
럼의 크기는 감소하고 스펙트럼의 사이인 wo(= 27r17）는 감소할 것이다. 반대로 T
가 고정되어 있고 V가 증가퇸다면 식 (2-32）에 의해서 스펙트럼의 크기가 상승하
며, 변한다면 zero crossing 대역폭은 감소할 것이다．
 이상과 갇이 주파수 스펙트럼의 사이인 m0는 T에 반비례하고, 스펙트럼 주파수
      94                                                                                                   2. Basic Concept
                                                                                                                              .


폭（대역폭）은 r에 반비례함을 알 수 있다．


      2.3.7 신호의 에너지／전력 표현

 신호에는 주기성이 있는, 즉 주기함수로 표시될 수 있는 신호와 주끼성이 없는，
즉 비 주기 함수로 표시될 수 있는 신호가 있다. 주기성의 주기는 어떤 의미에서 무
한（Ii出址te）이라는 개념과 같은 의미이다. 즉 주기가 지나고 그 다음은 새로운 것이
아니라 예전의 그것이기 때문이며, 변화가 없는 것은 예전의 그것이지 새 것이 아니
기 때문이다. 때문어］ 우리가 공부하는 신호해석에서도 주기신호에 대한 해석은 한
주기내로 제한되어도 전체어］ 대한 해석과 같다. 그리고 무한주기의, 즉 비 주기성의
신호에 대해서는 전구간어］ 대한 해석을 해야 할 것이다．
 이러한 사전의 생각에 의해서 신호의 전력과 에너지는 구별되어 생각되는 개념인
데 주기함수의 경우는 그것의 에너지 값이 발산（diversity）하는 형태의 무한값이 되
므로 의미가 없으며, 때문에 이것을 시간평균（미분 혹은 나눈）한 전력으로 나타낸
다. 반면 비 주기성 신호는 그것의 전구간 적분값이 유한한 값으로 나타나므로 그대
로의 에너지를 표시한다.
 여기에서 우리는 새로운 이론어］ 대해서 공부한다. 임의의 비 주기 신호의 에너지
를 1옴（아im)으로 정규화하여 신호의 에너지를 전압으로만 표시하면 다음의 식과
같다．

               E= ff2(t)dt                                                                                               (2-33)
 여기에서 F(功는 凡）의 Fourier 변환이라고 한다면 식 口33）의 에너지 표현식
은 다음과 같이 정리될 수 있다．
                                                                                     dm mm   4         \
                                                                                1戶



 ,,         rm . ,- . .           r的 . -   1    . - . . ..,., . --      .4' rm ,-. '.,, 尸. .. . ,,.
 也＝    J-    '- ,／끄）   at=   J.     f (t   2兀   .F   （幼'   " '   awjat＝   旨J-         BJ0J (t)e
                                                                                        戶        （W)              "dtJ   '


      그丁而沮-w)d。
       2兀 J小 '.'.H , ' "
                         = -- r IF(w)I2dw
                           2兀J小1 " '
                                                                                '""/                            (2- 34)


 결과적으로 신호는 시간과 주파수 모두로 표현될 수 있는 함수이므로 시간으로
표현된 식은 주파수로 표현된 식과 같다는 이야기가 된다. 이것은 （그림 2-10）에서
표현된 펄스의 경우로 이야기하자．
    2. Basic Concept
1                                                                             95

                                                              나K끼 2
                  町t)
                   A




     4                                > t
           -T/2          T/2                     -2/T     -l/T 0 lIT    2/T

                               （그림 2너0) 구형파의 에너지



    즉 시간축에서 표시된 구형파의 에너지는 구간 T와 크기 A의 곱인 끄4의 제곱이
퇸다. 이것은 주파수에서 표시되는 구형파의 빗금친 부분의 전체 면적과 같다는 것이
다. 여기에서 주목할 것은 그림 (b）에서 첫 주기 동안의 신호는 (AT)2의 면적보다
작으며, 그것의 차이는 나머지 대역들의 모든 에너지의 합과 같다는 것을 알 수 있다．


     2.3.8 Matched Filter
                                        0,
    디지털 통신 방식의 경우에서는 메시지 신호의 형태는 두 가지로 " ,, "1" 이다．
이것은 신호가 있느냐 없느냐의 관점이지 그 신호의 형태가 어떠한가는 크거］ 중요
한 것이 아니다. 즉 디지털 통신에서 수신기는펄스 폭 T 만큼의 시간 동안 펄스가
있느냐 없느냐만을 확인할 수 있는 기능이 있으면 되고 여기서 이야기될 Matched
Filter의 경우 신호의 유무（有無）를 더욱 더 명백하게 판단해 주는 F血er이다．
    즉 수신신호의 signal성분을 강화시켜 주고 잡음 성분은 감소시켜 주는 filter로서
그 시스템의 임펄스 response는 SNR을 최대로 하는 것이어야 한다. 이러한 기본적
인 생각으로 시스템을 설계하면 된다. （그림 2-li）과 같이 F血er의 입력신호를
如）+ n(t)로 표시하고 출력을 sO(t) + nO(t）로 표시하기로 하자. 여기서 巾）는 펄스
신호이고 n(t)는 통신 선로상의 잡음이다. 지금 片t切에서 (sO(t)/nO (t力를 최대로
하는 경우를 생각하1 보기로 한다. 그러나 여기서는 평균의 자승으로 표시하기로 하
며, 그것은 식 口35）를 최대로 하는 것이면 된다．

                        s(t) + n(t)                     s0(t) + n0(t)



                                 （그림 ?]]) Filter System
   96                                                                                     2. Basic Concept
                                                                                                             .


        S (t)
                                                                                                     (2中35)
            (t)
        n
 위의 식 口35）를 Fourier 변환을 이용하고 또 여기에 Schwarz의 부등식을 이용
해서 최대 경계치를 구하여 최대값을 구하면 식 2-36과 같은 임펄스 응답을 구할
수 있다．

        h(t) =ks(                       -t)                                                          (2-36)

 여기서 펄스의 유무 판단을 빨리 하기 위해서는 t=tm로 이동해 주면 퇸다. 따라
서 최적 시스템의 임펄스 응답은 메시지 신호 山）의 영상으로서 나타나며, 우측으
로 뇨초만큼 이동한 것이라고 볼 수 있다．

                                                      引t)                      t = tr7l



                                                                                           가tm)
                                                                    적분기（LPF)
                  f   (t)   =   s   (         .   1         ,   .



                                                  （그림 2나2) matched filt아의 모델


 한편 八'latched F血er은 （그림 2-12）와 같이도 표현될 수 있다. 지금 八'latched
F血er의 입력을 ／佃로 표시하고 Matched F血er의 임펄스 Resi刃nse를 風t)라고
하면 入'latched F血er의 출력 巾）는 다음과 같다．

        r(t) = r .i（兀)h(卜工)d                                                                         仁37)

 여기서 r仕)는丑U및 計x+ 뇨)로 주어지는 Filter 이다. 따라서

        r(t) = r f (x)s（工＋t나）d兀                                                                      口38)

가 된다. 그런데 출력 단에서의 판별 결정은 t= t加에서 출력 <tm）어］ 의해서 한다．
그러므로 다음과 같이 정리된다．

        r(r,)=57（兀）S（工）d兀                                                                            (2中39)


 이 식으로부터 K功은 （그림 2-12）어］ 나타난 바와 같이 끼me Correlator어］ 의
해서 얻을 수도 있다. （그림 2-12）에서 입력신호 巾）＋可t)에 如）를 곱한다. 이것
    2. Basic Concept                                      97
.


은 명백히 Synchronous Detection이 된다． 따라서 八4atched Filter I）毗ection은 본
질적으로 Synchi띠nous Detection임을 알 수 있다．



    2.4   표본화 이론


    임의의 고조파들을 포함하고 있는 파형어］ 특정한 간격으로 신호를 추출해 낼 때 특
정한 간격으로 추출퇸 데이터는 과연 어떤 정보를 어떤 의미로 가지고 있게 되는 걸
까？ 이러한 상황을 확인하는 것은 나중어］ 알게 되겠지만 상당히 큰 의미를 얻기 위해
서 공부하게 된다. 우선 임의의 고조파들을 포함한 그저 평범한 신호를 /(t)라고 하자．
그리고 일정한 간격으로 人t)의 신호를 추출하게 될 신호를 임펄스로 생각하자．
    결국 추출된 /(t)의 성분인 瓜t)는 다음과 같이 쓸 수 있다. 그리고 추출하는 과
정을 우리는 지금부터는 표본화（sampling）라고 하겠다．

          f (t) = f (t)S(t)                               (2-中［)

    식 口40）은 별로 특이하게 보이지는 않는다. 그러나 이 식을 Fourier 변환을 해
보면 엄청난（?) 의미가 숨겨져 있다. 식 口1）의 Fourier 변환은 /(t)와 8(t) 각각의
Fourier변환의 Convolution으로 나타날 것이다．

          F，回극mm少a，佃月극k回吃6(m-nw《，
                                )!
                =｝身(W)*45((J)-fl따）=｝츠F(w-n따）              (2-41)
    결과적으로 식 口41）으로 표현될 것이며, 이 식은 （그림 2-13）과 같이 전송되는
각각의 펄스 열들은 원래 신호인 /(t)의 모튼 주파수 성분을 포함하게 된다는 것을
알 수 있다．
    이상에서 이야기한 표본화 이론은 통신이론에서 대단히 중요한 정리이다. 이것은
아날로그 신호를 디지털화하는 과정에서 상당히 설득력 있는 기술적 근커가 되며，
이 정리어］ 근거하여 AD conve此ing 등이 이루어진다．
    이러한 표본화 이론은 정리하면 다음과 같다．
    98                                                                          2. Basic Concept
                                                                                                   .



   주파수 烏（H기 이상되는 성분이 없는 대역폭이 제한된 신호를 ]/2烏초 이
  하의 균등한 시간 간격으로 표본화하여 전송한 데이터는 원 신호가 가지
  고 있는 모든 주파수 성분들을 모두 포함하고 있으므로 원 신호를 그대로
  전송하였을 경우와 동일한 효과를 낼 수 있다．


 이것은 또 다른 의미로 생각할 수 있는데, 즉 표본화하는 주파수로 임의의 연속적
인 신호가 대역제한 필터（Band Pass Fil扼r）를 통과되었다고 생각할 수 있다．
 （그림 2-13）에서 T는 Nyquist 간격이라고 하며, Nyquist 간격은 신호의 표본화
속도와 관계가 있다．


               ／仕)




                                                                            t               CL)

             5(t)


     t十  -

                                                                            t
               T




                                                                            !
                         "'        "
                    ""        1"
                                       "
                                           "f"
                                                 "'   "｝   ·．.，·卞·   · ·，




                                                                                           (I)

                                                 （그림 ?13) 임펄스에 의한 표본화


 이 문제를 다시 설명하면, 표본화는 표본화 주파수로 신호의 성분, 즉 변화분을
추출하는 작업이다. 너무 직관적이지 않는가？ 즉 주파수가尻으로 제한퇸 신호의 주
파수 성분을 그대로 추출하기 위해서는 양（posit加e）과 음（negat如e）으로 변하는 값
을 읽으면 되므로 2!겨                                    빠르기로 표본화를 하면 그 파형의 모든 정보를 읽을 수
있지 않겠는가．
 （그림 2-14）는 표본화 정리를 직관적으로 이해할 수 있게 하1 주는 그림으로
    2. Basic Concept                                  99
1

Fourier 스펙트럼으로 신호를 분리해서 생각하는 것이다. 즉 (a）는 (b）와 같은 고조
파 성분들의 합으로 구해질 수 있다고 생각할 수 있다r 이것은 이제 나와 Fourier의
생각이다. 이러한 가운더］ 가장 빠른 주파수인 可의 위상의 극한치가 상향과 하향 2
개를 취한다면 2可번 신호를 취했을 때 왼쪽의 그림 (a）의 형태를 재현할 수 있을
것이다．




                       (a)
                                           (b)

                （그림 2너4) Fourier 스펙트럼에 의한 표본화 정리 해석


    그림에서 보는 바와 같이 가장 낮은 주파수의 상향 하향 변곡점을 취한다면, 즉
표본화한다면 그보다 낮은 수많은 주파수들은 모두 이미 표본화된 신호어］ 포함되어
있을 것이다．
    여기에서 재미있는 가정을 하1 보자. 만약 어떤 신호의 고조파·성분 중 가장 높은
고조파 성분이 n／라고 할 때 만약 표본화 빈도（주파수）를 2(n- 1)／로 한다면 어떤
결과가 나오겠는가？ 그렇다. 이렇게 표본화된 신호로 신호를 다시 재생한다면 可의
고조파가 빠진 형태의 신호가 복원될 것이다. 즉 표본화 프로세스는 표본화 주파수
로 대역제한 필터（Band Pass Filter）의 역할을 하고 있다고 생각할 수 있다.
  이러한 표본화 정리는 통신이론에서 가장 중요한 정리라고 할 수 있다. 이것은
Source Coding단계에서 Analog형태의 신호를 I玉gital로 변환해 준다. 이러한 작업
（표본화 작업）을 음성이나 영상이나 기타 등등의 Sou丁ce들을 Coding하게 된다. 9
장에서 공부하게 될 Vocoder 역시 입력 데이터는 음성신호를 표본화한 값을 압축
하는 방식어］ 대한 이야기이다．
 I    100                                                                                           2. Basic Concept
                                                                                                                       S


     2.4.1 자연 표본확（Natural Sampling)

 앞서 이야기한 표본화는 표본화하는 함수가 이상적인 임펄스 함수였다． 때문어］
표본화되는 순간의 시간이 순간이었으나, 현실적으로 임펄스 함수로는 표본화를 할
수 없으며, 시간 폭이 유한한 펄스신호로 표본화를 할 것이다. 그렇다면 표본화하는
동안어］ 유한한 시간이 흐른다는 이야기가 되고 이러한 시간이 흐르는 현상이 주파
수 영역에서는 어떠한 현상으로 나타나는지를 이 절에서 공부하자．
 폭이 T이고 주파수가 Nyquist 간격 T는 1屈品초로 생각하자.
 여끼서도 역시 소스 신호는 ／佃이고 표본화 함수는 仄0이고 표본화퇸 신호는
f (t)이라고 하자. 표본화된 신호는 소스 신호와 표본화 함수의 곱으로 나타날 것이
며, 이 함수의 주파수 영역에서의 특징을 알아보기 위해서 Fourier 변환을 하게 되
면 결국 只力의 Fourier 변환 F（功와 표본화 함수는 力（t)의 Fourier 변화 只功의
Convolution이 된다. 그런데 표본화 함수의 Fourier 변환은 식 (2d7）과 같이 구했
었다．
 표본화된 신호의 Fourier 변환 F , 佃）를 口뇨의 함수로 정리하면 다음과 같다．


        F,
        F5
             (m)
             (o)
                   =
                   =
                        Aro
                              7[
                              -
                                    ,   F
                                               (o.
                                                     )*
                                                          乶
                                                          n＝小
                                                                Sa
                                                                     (niw,
                                                                             ,)S   (o-   2no
                                                                                               ,)
                         三 2 Sa(ni.to, ) F(o力 站佃H力i包，)4'
                                                ,////
                         I         在：뇨

                         Ar二三" : " ." " ．·，二二. - .
                       =.-三2' Sa(nwL)F(w- 2nco, ,)                                                            (2-42)
                         乂·
                                  ．:：小．     ....     ,     "


 식 口42）은 앞서 이야기한 주기 구형파의 스펙트럼 밀도함수 /7, 의 변화 형태로
각각의 주파수 대역의 크기가 결정되는 형태를 가지게 된다. 즉 /(t)와 力（勿의 곱어］
의한 표본화 작업의 결과로 F (功의 모튼 주파수 성분을 포함한 대역이 무수히 많
이 형성되며 이것의 크기들은 임펄스로 변조했을 때와는 달리 변조하는 펄스의
Fourier 변환식과 같은 추세로 그것의 세력（크기）이 변해 감을 알 수 있다．
 그러나 우리가 복조단에서 신호를 찾을 때는 결국 초기의 대역을 찾게 되므로 임
펄스일 때나 펄스일 때나 그것의 결과는 동일하게 얻을 수 있다. 그것은 임펄스의
경우 우리가 신호를 복원할 때 사용되지 않을 모든 대역의 신호를 감쇠 없이 전송한
다는 것이고 펄스인 경우는 표본화할 때 임펄스와 갇은 성질을 갖지 않으므로 나머
    2. Basic Concept
口                                                      101


지 대역의 신호가 감쇠된다는 것이다. 그러나 우리에게 필요한 것은 중앙의 하나의
대역의 신호이므로 달라질 것은 없다．


                                           戶"R川




                            t                     0)




                            t




                       （그림 ?］듸 Nat바톄 표본화


 이것어］ 의하써 우리는 얼마의 빠르기로 표본화를 한다는 것이 표본화된 신호가
가지고 있는 주파수 정보를 포함하는가의 여부와 관계가 있는 것이며 따라서 표본
화하는 신호는 단지 특별한 의미가 없는 그것의 크기만을 결정한다는 것을 알았다．
참고로 크기가 별 의미가 없다는 것은 증폭이라는 간단한 절차로서 해결될 수 있는
문제이기 때문이다．


     2.4.2 순간 표본화(II鳩tance Sampling)

 앞 절에서는 표본화가 이루어지는 동안 시간이 흘렀을 경우에 주파수 영역에서는
대역의 세력이 점점 약해지는 것을 확인했다. 그렇다면 표본화하는 파형의 모양이
자유로우나 표본화되는 시간이 순간적인 순간 표본화의 경우를 생각하1 보자. 즉 표
본화는 순간적으로 이루어지나 표본화퇸 출력신호는 표본한 신호의 대역폭어］ 대한
정보를 여전히 가질 것이므로 주파수 영역에서의 비정상적인 효과는 우리가 미리
짐작할 수 있을 것이다．
 즉 （그림 2-16）과 같은 경우라고 생각하1 보자．
                                            2. Basic Concept
                                                               1




                                卜   t


                       （그림 2너6) 순간 표본화


 （그림 2-16）에서 임의의 파형 Q（砂를 표본화어］ 사용하고 입력신호를 人勿라고 할
경우 표본화 된 신호인 x (t)는 다음과 같다．


     x3(t) = 2 f (nT)q(t- nT)                          (2-43)
           n=mm




 주의할 것은 앞의 자연 표본화와는 달리 순간적인 신호를 표시함으로 불연속적인
신호로 표시해야 할 것이다. 위의 식은 임펄스로 표본화한 경우의 신호 /( t)와 비
교할 수 있다．

     ／沁戶 Z只町戶(t -兀T)
           r1＝小




 식 口40）은 표본화 간격을 연속적인 함수로 표시하였으며, 식 e-44）은 불연속
적으로 표시한 것이다．
                      fs(t)
                                h(t) = q川




           （그림 ?17) 순간 표본화의 임펄스 표본화로 등가화



 이제 兀 ( t)의 스펙트럼을 구하자. 여기에서 우리는 이상과 같은 상태를 입력신호
가 /K勿이고 시스템의 임펄스 응답이 q( t）인 시스템이라고 생각하고 구할 수 있다．
 따라서 식 (2-44）의 주파수 대역의 식은 식 (2-41)에서 다음과 같이 쓸 수 있다．
    2. Basic Concept
.                                                          103



              . . 』，. . =m . . 1 J:, 小 . . 寸．          .
           入5 ((z)) = Q(CO)t (W) =三？二U(nUf'(n) - 2flO)m)   (2- 45)


    (2-45) 식에서 표본화 함수 凡(t)의 스펙트럼은 주기적인 반복 스펙트럼 只功
어］ q( t)의 스펙트럼 Q（帥를 곱하여 표시되는 것을 알 수 있다. 식 口42）과 식
口45）를 비교하면 口42）에서 어느 주기동안이나 일정한, 즉 F , 佃）의 상수배아나
식 口弱）은 그것의 변화형태가 口J의 함수의 형태로 변화하는 형태로 나타난다．
    이러한 순간 표본화는 표본화하는 과정어］ 시간이 순간적이면 되므로 표본화될 때
펄스의 모양이 변화되지 않는 형태로 표본화가 되어도 동일한 결과가 나올 것이다．



    2.5   신호의 표시
                                                                 )
     2.5.1 데시벨（dB)

    통신 시스템에서는 흔히 신호의 전력을 나타낼 때 로그 스케일을 사용한다. 즉 식
口띠6）과 같이 전력비를 log scale로 나타낸 것이다．

          차a'기 = lulog寸dli]
           戶   .   h,   』   八   ．        r   .   小   1



                                                           (2- 46)
                                    7)
                      ／二

    데시벨은 전력비에 의한 값이므로 그것의 단위는 dimension이 없는 배（倍）가 된
다. 그리고 log의 밑은 10이다. 이러한 데시벨은 신호를 표시할 때 log scale로 함으
로써 취급하기어］ 예를 들어서 표를 그리기에도 편리하게 퇸다. 또한 이러한 데시벨
은 비단 전력과 전력뿐 아니라 전압 전류 등의 전기량들도 서로 비교되는 값으로
표현할 때 사용되기도 한다. 통상 전력의 비를 위의 식과 같이 표현했으므로 전압으
로 표시할 때는 lOlog( V1/ V2)2의 값이 20log( V1/ V2）로 바뀌게 될 것이다．
    여기에서 한 가지 생각해 볼 것은 lolog(1/2）의 값을 생각하1 보자. 이 값은 약
召［dB］가 된다． 즉 3[dB］라는 것은 측정하고자 하는 전력이 기준전력의 2배임을 나
타내는 것을 의미하며, 3[dB］라는 것은 측정하고자 하는 전력이 기준전력의 반이
되는 것을 말한다. 우리가 흔히 3[dB] 아래지점이라는 말을 많이 하는데 그것은 현
재 전력의 반이 되는 지점을 이야기하는 것이라고 이해하면 될 것이다．
    이러한 데시벨의 단위는 기준값을 고정시켜 둠으로 해서 또 다른 의미의 단위로
   104                                 2. Basic Concept
                                                          .


사용되기도 한다. 즉 데시벨은 상대적인 값을 나타내는 말인뎨 그 상대가 되는 값을
정규화된 값으로 설정하게 되면 그 값어］ 대해서 얼마나 큰 값이 되는지를 표시할
수가 있게 된다. 이러한 단위는 실지로 RF Power 등을 나타낼 때 상당히 자주 사
용된다. 가장 흔하게 사용되는 기준값은 1W와 1mW이다．
 기준값이 1W라고 했을 때 그것의 단위는 dBW라고 표시하며, 2W의 전력을
dB刀로 표시하면 1W의 2배, 즉 3dB이 크므로 3dB＼刀가 되는 것이다. 또한 기준값
이 1mW일 경우에는 그것의 단위를 dBm이라고 표시한다．
 dBm과 dBW는 그것의 기준단위에서 1000배의 차이가 남으로 dBm을 dBW로 표
시할 때는 30을 빼 주어야 하고, dB刀을 dBm로 표시할 때는 30을 더해 주어야 한다．


  2.5.2 대역폭（Ban小vidth)

 아날로그 신호를 디지털 신호로 변환해 주는 표본화 정리는 표본화 율어］ 의해서
통과대역을 제한해 주는 것이 필연적이다. 그러나 그러한 신호는 무한시간 구간을
가지므로 실현 가능하지 않다. 대역폭의 정의는 여러 가지가 있으나 통상 스펙트럼
밀도의 넓이어］ 대한 척도로서 나타낸다．




                    （그림 ?18) 대역폭의 종류


 （그림 2-18）은 여러 종류의 대역폭의 정의를 나타낸다. 3dB대역폭은 스펙트럼 밀
도가 최대값보다 3[dB］떨어지는 주파수 구간, 즉 에너지가 반으로 떨어지는 주파수
대역까지를 말하며, 잡음등가 대역폭은 스펙트럼 밀도가 백색잡음 스펙트림 밀도와
  2. Basic Concept                              105


똑같은 면적을 가질 때의 주파수 구간을 말한다. 영점 사이의 대역폭은 스펙트럼 밀
도가 첫 번째 영（zer이이 되는 구간을 말하며, 99% 에너지 대역폭은 에너지（스펙트
럼 밀도의 주파수 영역적분）가 99%를 차지하는 주파수구간을 말한다．


       역폭
 필터는 주파수로 해석되는 회로이며, 입력신호의 시간요소는 의미가 없다. 저역통
과 필터（LPF : Low Pass Filter）는 입력신호를 받아들여 차단 주파수五 이하의 모
튼 주파수 성분을, 고역통과 필터（I표下 : High Pass Filter）는五 이상의 모든 주파
수 성분을 통과시킨다．
 대역통과 필터（BPF: Band Pass Filter）는 통과대역 이내의 주파수 성분만 통과
시키며, 대역제한 필터（notch Filter）는 통과대역 이내의 주파수 성분을 제한한다．
이때 차단 주파수 /，는 주로 3[d그B] 대역폭을 사용한다. 즉 四(J叩이 최대값의 1/2
이 되는 지점을 차단 주파수라고 한다．


   2.5.3 Error 함수 erf住坦｝ erfc（幻

 평균이 0이고 편차가1인 Gaussian 확률믿도 함수를 우리는 정규분포라고 한다．
이것은 일반적으로 Bit 에러 확률을 생각할 때 랜덤하게 발생되는 형태가 이 분포
함수와 비슷한 형태로 나타난다고 해서 통신에서 많이 사용한다. 특히 복조기의 성
능을 평가하는 척도로 많이 사용퇸다. 이러한 Gaussian 확률밀도함수는 다음과 같
이 쓸 수 있다. 즉

                     1
                                                (2- 47)
                           .   x2/
                                /2
                m
         hrV\
        P＼人I - 1= =t二
                    V乙7r

 이러한 확률밀도함수는 랜덤한 변량 x의 함수이고 x보다 더 큰 값이 나타날 확률
을 나타내는 확률은 이 함수의 정적분으로 나타난다．
        n/ V\ 1 1 尸    Jm                       . .48).
        Q(x) =+= I e '2dz                       (2-
        乂＼八／ 扼구1V                               "     "
   106                                                  2. Basic Concept



                                 확률

                                                 H확률이 작아자뇬 방향
                           확률이   沚三 방향 켜1
                                                     町／C伽J




                                                             변량
                                            \r
              （그림 2-］이 정규분포의 확률 분포 함수와 확률（적분값）


 （그림 ?19）는 이러한 것을 나타내는 그림이다. 여기에서 알 수 있듯이 Q(0）은
0.5이고 Q(-미는 1이다. 물론 0佃）는 0이다．
 여기에서 우리는 이러한 확률밀도함수와 그것의 적분에 근거하여 에러함수, 즉
에러 발생 확률함수 e玎（力에 대해서 생각하1 보자. （그림 2-19）에서 보는 바와 같이
尤＝0을 중심으로 대칭적인 함수이다．
 따라서 한쪽 방향을 생각하여 2배로 계산하면 모든 것이 동일하게 적용될 수 있
다. 즉 에러가 발생한다는 것은 변량 Xi!- 0부터 兀의 범위에 들어 있다는 것이라고
한다면 이것은 다음과 같이 쓸 수 있다．

                   2
         町／（刃 = 1三＝       i2dt                                     (2-49)
                ,Jz兀

 이것은 일종의 확률함수인 O（功이며, 이것은 erft缸）=1- 臼火功로 표현되는 또
다른 형태인 erfc(功로도 나타날 수 있다．
 우리는 통신 시스템에서 그것의 성능을 0（功의 값으로 설정하여 거기어］ 부합되
는 尤의 값을 구하는 것이 일반적이다. '
 식 口47）과 식 (2-48）을 사용하여 O（功와 erfc(兀）와의 콴계를 새로 정립하면 다
음과 같다．

           . .  1  . / 工 \
         (/（工）= -ei／디 1三 1                                         (2-50)
               乙       \VZ7

 다음의 표는 尤7} 큰 값으로 나타날 때 에러확률이다．
    2. Basic Concept                                                     107
1

                              （표 2너） 정규분포의 확률0(x)

    x     dB           O(x)     x     d日       O(x)       x     d日       O(x)
 3.00    4.77     1.35E-03     4.00   6.02   3.17E-05    5.00   6.99   2.87E-07
 3.05    4.84     1.14E-03     4.05   6.07   2.56E-05    5.05   7.03   2.21E-07
 3.10    4.91     9.68E-04     4.10   6.13   2.07E-05    5.10   7.08   1.70E-07
 3.15    4.98     8.16E-04     4.15   6.18   1.66E-05    5.15   7.12   1.30E-07
 3.20    5.05     6.87E-04     4.20   6.23   1.33E-05    5.20   7.16   9.96E-08
 3.25    5.12     5.77E-04     4.25   6.28   1.07E-05    5.25   7.20   7.61E-08
 3.30    5.19     4.83E-04     4.30   6.33   8.54E-06    5.30   7.24   5.79E-08
 3.35    5.25     4.04E-04     4.35   6.38   6.81E-06    5.35   7.28   4.40E-08
 3.40    5.31     3.37E-04     4.40   6.43   5.41E-06    5.40   7.32   3.33E-08
 3.45    5.38     2.80E-04     4.45   6.48   4.29E-06    5.45   7.36   2.52E-08
 3.50    5.44     2.33E-04     4.50   6.53   3.40E-06    5.50   7.40   1.90E-08
 3.55    5.50     1.93E-04     4.55   6.58   2.68E-06    5.55   7.44   1.43E-08
 3.60    5.56     1.59E-04     4.60   6.63   2.11E-06    5.60   7.48   1.07E-08
 3.65    5.62     1.31E-04     4.65   6.67   1.66E- 06   5.65   7.52   8.03E--09
 3.70    5.68     1.08E-04     4.70   6.72   1.30E-06    5.70   7.56   6.OOE-09
 3.75    5.74     8.84E-05     4.75   6.77   1.02E-06    5.75   7.60   4.47E-09
 3.80    5.80     7.23E-05     4.80   6.81   7.93E-07    5.80   7.63   3.32E-09
 3.85    5.85     5.91E-05     4.85   6.86   6.17E-07    5.85   7.67   2.46E-09
 3.90    5.91     4.81E-05     4.90   6.90   4.四E-07     5.90   7.71   1.82E-09
 3.95    5.97     3.91E-05     4.95   6.95   3.71E-07    5.95   7.75   1.34E-09



                                                                                   \
    2.6 잡음（N이se)                                                                    1

    잡음이란 예기치 못하게 원하지 않는 신호가 전송시스템 및 전송매체 등어］ 의하1
서 발생하여 전송신호어］ 추가되어 통신 성능을 저하시키는 요인이 되는 신호를 말
한다. 잡음들은 그것의 발생 원천에 따라서 외적잡음(E毗emal Noise）과 내적잡음
(Internal Noise）으로 구분퇸다．
    외적잡음은 사람어］ 의해서 만들어질 수도 있고 자연적인 현상으로 만들어질 수도
있다. 번개가 칠 때 TV방송이나 라디오 방송에 잡음이 발생하는 경우는 이러한 외
적잡음의 대표적인 경우이다. 이때 가해지는 잡음은 임펄스 잡음（임펄스 Noise）이
라 하며, 이것은 순간적으로 굉장히 큰 전기적인 충격이 가해지므로 앞서 공부한 임
       108                                 2. Basic Concept
                                                              1


펄스의 형태와 유사한 신호로 표현되며, 때문어］ 아주 넓은 대역에 걸쳐서 잡음신호
의 영향을 끼치게 되는 것이다．
     이때는 아마 우리가 알고 있는 모튼 통신 시스템어］ 알게 모르게 이러한 임펄스
잡음의 영향을 받을 것이다. 지금까지 공부를 정확히 한 독자는 알고 있겠지만 이러
한 임펄스 형태의 번개의 영향은 그것이 발생하는 시간, 즉 아주 짧은 시간어］ 의해
서 그것의 충격이 얼마나 넓은 주파수 대역에 영향을 끼치는지를 알 수 있을 것이
다．
     비가 오거나 습기가 많은 날 전화를 사용할 때 다른 사람의 전화내용이 함께 들
리는 누화 현상（Cross Talk) 또한 잡음어］ 의해서 발생되는 것이다. 이것은 전화선
로가 인접한 다른 전화선로와 전자기적 상호작용을 함으로써 발생된다.
     내적인 잡음의 예로는 송신측과 수신측에서 사용하는 통신 시스템의 비 선형성
（入［on-linearly）으로 인해서 발생하는 잡음인 상호변조잡음（mt町그Tiodulation）이다．
이는 전송신호를 반송 주파수로 변조시킬 때 변조된 전송 신호뿐 아니라 이들 두 주파
수의 합과 차어］ 대한 배수의 주파수 성분들이 생성되는 것이다. 이를 방지하기 위해서
는 통신 시스템의 선형성이 최대한 보장될 수 있게 설계하고 구현하여야 한다．
     동작중인 통신 시스템어］ 인접하여 동작하는 다른 송신기나 신호원천 역시 잡음원
천의 역할을 할 수 있다. 이때 동작중인 시스템에서 원하지 않는 신호가 들어왔으므
로 그 시스템의 동작어］ 영향을 줄 수 있는데 이것을 간섭（Interferei（이이라고 하며，
넓은 의미에서 이것도 잡음이다.
     외적잡음은 우리가 어찌할 수 없는 잡음이라고 할 수 있으나 내적 잡음의 발생원
인을 줄이는 것이 필요하며, 시스템의 성능을 평가할 때 이러한 잡음에 대해서 어느
정도의 극복력을 가지는가가 그것의 성능을 평가하는 척도가 되기도 한다．

      2.6.1 열 잡음（Thermal Noise)

     내적 잡음에는 여러 가지가 있으나 통신 시스템에서 가장 중요한 문제가 되는 것
은 열어］ 의한 잡음인 열 잡음（Thermal Noise）이다．
     열 잡음（존슨 잡음）은 전기도체 내에서 온도어］ 따른 전자의 운동량 변화어］ 의해서
발생되며， 모든 전자소자와 전송매체에서 발생하고, 온도어］ 비례하여 증가한다. 열 잡
음은 모튼 주파수 영역에 걸쳐서 고루 분포되므룩 이를 백색잡음(White Noise）이라
고 한다． 일반적으로 빛의 3원색을 모두 합하면 백색이 되는 것어］ 기인한 것이다．
    2. Basic Concept
N                                              109


즉 빛의 3원색의 주파수 대역을 다 포함하고 있는 색이 흰색이기 때문이다．
 이러한 열잡음의 평균전력은 도체의 절대온도어］ 비례하며 이 도체를 통해서 전송
되는 신호의 주파수 대역폭에도 비례한다. 이는 도체가 유한한 온도어］ 놓여 있을 때
그 도체를 잡음전력 발생기로 생각할 수 있다는 것을 나타낸다．


 백색 가우스 잡음
 잡음신호 可t)가 모튼 주파수 성분을 가지며, 전력 스펙트럼 밀도가 모튼 주파수
에서 일정한 잡음을 갖는 잡음을 백색잡음이라고 한다. 잡음신호가 모든 주파수 성
분을 갖는다는 의미는 모든 주파수에 잡음의 영향을 그것의 전력 스펙트럼 밀도만
큼 영향을 끼칠 수 있다는 말과 갇다. 실제의 통신 시스템에서 채널이나 전자부품의
열에 의한 전자의 운동으로 발생되는 열 잡음은 이러한 백색잡음의 성질을 갖는다．
 통신 시스템의 채널에는 백색잡음 이외에도 여러 종류의 잡음이 존재하지만 그
중에서 가장 중요하고 기본이 되는 잡음이 백색잡음의 성질을 갖는 열 잡음이다. 또
한 열 잡음은 랜덤 신호이므로 특정 시간어］ 그 크기가 랜덤하게 변한다. 따라서 이
러한 랜덤성을 가지는 신호, 즉 열 잡음의 표현은 평균이나 분산 등의 통계적 성질
로 표현할 수밖어］ 없다. 이때 표현되는 통계분포 함수가 가우스（정규） 분포어］ 의해
서 표현되어진다. 이러한 가우스 분포는 평균이 0이고, 분산이 (2인 통계분포이며，
이 분포는 랜덤 함수를 표현하는 가장 일반적인 분포함수이며, 가장 자연스러움을
표현한 함수이다.
 우리가 통신 시스템을 이야기하는 가운데 AWGN(Addit如e White Gaussian
Noise）이라는 말을 많이 사용하는데 여기에서 \Vhi扼라는 말의 의미가 재미있다．
일반적으로 빛의 3원색인 R（砒d), G(Green), B(B血e) 성분이 모두 있는 색이 흰색
(White）이다. 즉 모든 빛의 주파수 성분을 모두 가지고있으면 White가 된다는 것인
더］, 이것은 가시광선의 경우에서 이야기하는 것이지만 모든 주파수를 포함하고있는
（잡음） 신호를 표현할 때 우리는 또다시 "M小ite"라는 단어를 사용해서 표현한다．


     2.6.2 잡음지수

 우리가 알고 있는 통신 시스템의 개략은 다음과 같다．
 송신측에서는 송신할 신호를 최종적으로 변조단에서 전송할 것이다. 그러나 이러
한 신호는 송신단의 출력어］ 의해서 무한히 클 수는 없으므로 수신측에서 그 신호를
I     1 10
             1
                                         2. Basic Concept
                                                            1


수신하여 복조할 때는 증폭 을 통해서 채녈상에서 소실된 전력 부분을 보상하게 될
것이다. 또한 채널 상에서 송신된 신호는 그것의 진폭뿐 아니라 주파수 위상 등과
같은 정보들도 잡음에 의해서 왜곡 혹은 손실될 것이다. 이것은 모든 통신채널은
AWGN 채널을 포함하는 채널이기 때문어］ 전 대역에서 이루어질 것이며, 이것은 경
로손실 등과 같은 원인어］ 의해서 발생퇸 신호의 감쇠 성분을 보상하1 주는 증폭장치
에서 양호한 신호와 갇이 증폭될 것이다. 즉 잡음과 신호를 구분하는 단계 이전어］
전력이 증폭되어 이러한 잡음도 같이 증폭이 이루어진다（어쩔 수가 없다）.
 만약 수신된 신호의 증폭, 복조, 신호처리 등의 여러 과정에서 별도의 내부 잡음
이 생기지 않는다면 설사 잡음이 신호와 같이 증폭된다 하더라도 수신단의 신호 대
잡음비와 출력단의 신호 대 잡음비가 같게 될 것이다. 그러나 실제로 증폭기 자체어］
서 내부잡음이 발생하므로 일반적으로 수신단의 SNR은 송신단의 SNR보다 작거］
나타난다.
    잡음지수（Noise 까gi玎e）란 입력 SNR과 출력 SNR의 비를 말하며, 일반적으로 1
배（0dB）보다 큰 값이 되며, 잡음지수가 크다는 것은 그 증폭기가 발생하는 내부잡
음이 그만큼 크다는 말이 된다.
 （그림 2-20）어］서 입력신호 전력이 P前（W), 입력잡음 전력이 Pm(W）인 신호가 이
득이 g배인 증폭기를 통과하였을 때의 출력신호 전력 民(W), 출력잡음 전력
民(W）을 생각하1 보자．




                   （그림 ?20) 일반적인 증폭71


 출력신호 전력은 당연히 입력신호 전력이 g배 증폭된 것이므로 /)s。=g／工，이다．
그러나 출력잡음 전력은 입력잡음 전력이 g배 증폭된 것과 증폭기에서 발생한 내부
잡음（초과잡음이라고 하며, Pax(W) 라고 표기하자）이 더해진 것이므로 여기에서
입력 SNR은 ／늪사乙川고, 출력 SNR은 凡／Pn, 이므로 잡음지수는 다음과 갇고 1보
다 큰 값이 된다．
    2. Basic Concept
1                                                         1 11




          F-P"PS今,戶
               /JJ,        /(gIJ,i+之)
                                                          (2- 51)




    여序甘 2-11 입력 신호전력이 2[W], 입력잡음전력이 0.02［硼, 출력신호 전력이
               20[WII, 출력 잡음 전력이 0.4[W］라고 할 때 이 증폭기의 잡음지수를
               구하라．
        ？晦h뇨           1   H   .   .   .
     푿oI.;     먼저 이 증폭기．의. 이．득은 g=20/2=10배， 즉 10dB임을 알 수 있다． 또
               한 입력잡음 전력이 10배 증폭되면 0.2[W］가 되므로 증폭기의 초과
               잡음이 0.4-0.02 x 10=0.2임을 알 수 있다. 이 증폭기의 잡음지수를
               계산하면
                 2/0.02 -
               F= ' ,    =2（帥          or   3dB
                 20/ 0.4

               가 됨을 알 수 있다．
    일반적으로 수신기에는 여러 단의 증폭기가 캐스 케이드로 연결되어 있다. 이득
이 幻배이고 잡음지수가 Fl인 전치증폭기와 이득이 g, 배이고 잡음지수가 F , 인
증폭기를 통과했을 때 전체이득과 시스템 전체 잡음지수는 어떤 관계가 있는지 알
아보자．
    시스템 전체이득은 gl · g2이다． 물론 dB로 표현되었을 경우는 더하면 퇸다．
GE dB] = G1 [dB1 + G2 [dB］가 된다. 그러나 시스템 전체 잡음지수 F=F1+ ( 尻 -1)/g1
이 된다. 여기에서 주목할 것은 일반적으로 g,은 F, 에 비해서 큰 값이므로 시스템
의 전체 잡음지수는 거의 전치 증폭기의 잡음지수어］ 의해서 결정된다. 즉 통신 시스
템의 수신기 설계어］ 있어서 전치 증폭기는 반드시 저잡음 증폭기（LNA）를 사용해야
한다는 것이다.
    예를 들어서 전치 증폭기의 이득이 10배, 잡음지수가 2이고, 주증폭기의 이득이
1以）배， 잡음지수가 5인 경우 시스템 전체이득은 10(刃배, 즉 30dB가 되고 시스템 전
체 잡음지수는 F=2+(5-1)/10=2.4이 되어 전치 증폭기의 잡음지수 2의 근처 값이 된
다． 수신기어］ 입력퇸 신호의 크기가 미약하므로 시스템 전체이득을 키우는 것도 중
   112                                 2. Basic Concept
                                                          1


요하지만 시스템 전체의 잡음지수를 낮추는 것도 그어］ 못지않게 중요하다．
 이 두 가지의 문제점을 동시어］ 해결하는 방법이 바로 전치증폭기의 잡음지수를
낮추고 다음 단의 증폭도를 높이는 것이다．




 이 절에서는 통신로를 통하여 전송할 수 있는 전송률（transmission rate）과 에러
의 관계를 공부한다. 이어］ 앞서서 정보의 전송률을 정의하면 다음과 같다．
 통신로를 통하여 T초 동안에 송신측으로부터 수신측어］ 전송되는 정보량을 IBit
라고 하면 탄위시간당의 전송정보량（정보전송 속도） I？은 다음과 같다．

         R=   1-   [bpsl                          (2- 52)
               T

 상호 정보량（정보 전송량）I는 송신신호 巾）의 확률밀도함수 力（S）어］ 의하1 변화하
는 양이다. 그렇지만 송신신호에는 무엇인가의 구속요컨, 예를 들면 전력이 일정하
다라는 조컨이 존재하므로 전송정보량 I는 유한이며 최대치가 존재한다. 전송정보
량 ／가 최대가 되도록 송신신호 巾）의 확률밀도함수 力（0를 정할 때 단위 시간당
의 전송정보량을 채널용량이라 한다．
 정보원이 많은 메시지들 중 하나를 r[message/sec］의 비율로 보낼 수 있다고 가
정한다. 예를 들어서 만약 데이터의 소스가 팩스라면 전송률은 1초당 기호의 수일
것이다. 만약 각각의 정보에 대한 확률을 알고 있다면 엔트로피, H[bit/message］를
계산할 수 있다. 그리고 엔트로피 H와 메시지율 r의 곱을 취하면 R[bits/sec］로 표
시되는 정보율을 알 수 있다. 따라서 R = rH[bps］이다. 하나의 예를 들어서 1초당
2메시지로 전송되었다면 정보율은 3[bps］이다．
 일반적으로 주어진 통신 시스템에서 정보율이 증가되면 단위시간당 발생하는 어］
러의 수도 증가한다는 것을 직관적으로 알 수 있다.
 C.E.Shannon은 통신채널이 주어지면 이 채널이 가질 수 있는 정보 최대 전송률
C가 있음을 증명하였다. 이 최대 전송률을 통신용량이라 한다. 만약 정보율 R이 C
보다 작다면 부호화 기술어］ 의해서 임의의 작은 오류확률어］ 접근시킬 수 있으며，이
것은 잡음이 존재하는 경우에도 적용된다. C.E.Shannon의 정리는 그 반대도 성립
    2. Basic Concept                            1 13
U


한다. 즉 정보율 R이 통신용량 C보다 크다면 부호화 기술을 사용하여도 에러를 피
할 수 없다. 이런 기본적 이론의 증명은 생략한다．
 AWGN이 존재하는 대역 제한된 채널에 관하여 살펴보기로 한다. 이 경우 통신
용랑은 다음과 같이 주어진다．

          C=Wlog2(1＋多自）                         (2-53)


 여기에서 C는 bps의 단위를 갖는 통신용량이고, M兀I七］는 채널의 대역폭, S/N은
신호 대 잡음비이다. 위의 식을 Shannon-I拓此ley 정리라고 한다(Hartley가 예비적
인 작업을 했고 Shannon이 정확히 유도했다고 한다）. 식 口53）는 직관적으로 이해
할 수 있다．
 즉 채널의 태역폭이 증가하면 정보신호가 다 빠르게 변할 수 있으며, 이로 인하여
정보율이 증가한다. 또한 S/N을 증가시키면 잡음 때문어］ 발생하는 에러를 방지할
수 있으므로 정보율도 증가시킬 수 있다. 위의 내용에서 주목할만한 사실은 잡음이
전혀 존재하지 않는다면 SNR은 무한대가 되고, 대역폭어］ 구애받지 않고 무한대의
정보를 전송할 수 있다는 것이다. 식 口53）에서 대역폭이 무한대에 접근하게 된다
면 통신용량 또한 무한대에 접근하게 된다. 하지만 후자의 결론은 옳지 않다．
 왜냐하면 채널내어］ 백색잡음이 존재한다고 가정했기 때문어］ 대역폭이 넓어지면
넓어질수록 더 많은 잡음이 시스템에 영향을 미치게 되므로 식 口53）에서 B가 증
가하면 SNI｛이 감소하기 때문이다. 후자어］ 관하여 좀더 자세히 살펴보는 것은 바람
직하다. 총주파수［H기당 신호대 잡음비［S/N/H기가 고정되었다고 가정하고 최적의
채널을 설계하고자 한다．
 시스템의 대역폭을 증가시키는 것은 비용과 밀접한 콴계가 있O 口로 최대 통신용
량을 구하여야 한다. 채널의 잡음이 백색잡음이고 그 전력 스펙트럼 밀도가 N0/2라
고 가정하자. 또한 신호의 전력이 S라는 특별한 값으로 고정퇸 경우 식 口53）로 부
터 통신용량은 다음과 같이 주어진다.

          C＝꺼／log2(1『夕自，y                       (2-54)
 여기서 \V의 단위는 [I初］이고는 [Watts力F-I기를 단위로 하는 전력스펙트럼 밀도임
을 주목하라. 이제 \V가 무한대어］ 접근할 때 통신용량의 값을 구하면 다음과 갇다．
                                                      2. Basic Concept
                                                                         .



      C ＝抑w10帥4自）
       ＝駟（夕自，
            )log2[1砂/(N。
                       ,B)1N08/S
       呵仙咀e=1.叫自，)                                               (2-55)

 식 口55）은 가능한 최대 통신용량이 신호전력과 잡음전력 밀도의 함수임을 보여
준다． 실제적으로 시스템을 설계하는 경우 통신용량을 위 식의 값과 비교하여 대역
폭을 더 증가시키는 것이 타당한가를 결정하는 것이 비용면에서 바람직하다．
 즉 C보다 낮은 전송속도로 정보를 전송하면 오류확률은 0에 접근한다는 것이다．
Shannon은 그러한 시스템을 설졔하는 방법을 설명한 것이 아니고 이론적으로 그러
한 시스템이 가능함을 증명했다. 그러므로 설계자는 허용된 오류확률 범위 내에서
가능한 한 C에 가까운 데이터 율을 갖는 시스템을 이상적 시스템이라 부른다．
 만약 2진 통신시스템을 설계하기 위하여 통신채널의 대역폭과 최대 신호전력 그
리고 잡음전력밀도를 식 口55）어］ 대입하면 최대 정보율 C를 산출할 수 있고 표본
화율과 양자화의 Bit 수를 대입하면 정보 전송률의 R[bps］를 계산할 수 있다. 그 결
과로부터 R이 C보다 작음을 알 수 있다. 따라서 Shannon은 2진수 데이티 계열을
잘 부호화한다면 임의의 낮은 오류확률을 얻을 수 있다고 했다．

":'; 恥多聲：" 채널의 대역폭이 3000[H기이고 채널 출력의 S八＝1000인 경우 대역
         통과 채널의 통신용량을 계산하라．

 二 j吐二   C= Wlog2 (1+ S/N) =(3000) 1og2 (1+1000) 七30, OOO
         위 예제의 Parameter는 표준 음성용 전화선에 관한 것이다. 현재 이
         러한 채널에서 얻을 수 있는 최대 전송률은 9600[bps/sec］이다. 이보
         다 더 높은 값을 얻으려면 매우 복잡한 변조기와 복조기를 사용하여
         야 한다．
    3. DSSS와 Code이론                         115
.




                           DSSS와 Code이론




    통신은 원시시대부터 사람들 사이에서 행해져 왔으며 그 방법은 시대를 거듭할수
록 발전해왔다. 이러한 정보를 교환하는 행위인 통신은 그것을 위해서 사용되는 매
체가 유선이냐 아니면 무선이냐어］ 따라서 유／무선통신으로 구분할 수가 있다. 즉 원
시인들이 혹은 전자파의 발견 이전의 통신방식은 모두 무선, 즉 선이 없는 통신 방
식이었다. 그러나 이러한 무선어］ 정보를 실어보내는 매체를 마르코니 이후에 전자
파（줄여서 전파라고도 함）를 사용하게 되었으며, 이러한 변화는 통신의 형태를 파격
적으로 변화시켰다．
    즉 이러한 매체를 사용할 수 있게 퇸 도구의 인간은 더 멀리, 더 많은 정보를 그
리고 더 정확한 정보교환을 할 수 있게 해주었다. 이러한 정보의 교환, 즉 통신은
현대에 와서는 전송해야 할 정보량이 더욱 많아지고 또한 그것이 보편화됨으로써
무한한 것 갇은 전파자원의 제한이라는 문제어］ 직면하게 된다. 따라서 그 이후의 통
신은 더 많은 정보를 전송하는 방법에 치중하게 되면서 통신 시스템의 용랑을 배가
할 수 있는 방법을 찾고자 많은 과학자들이 노력해 왔다．
    이러한 배경에서 확산 스펙트럼이라는 전송방식이 이론적인 출현 이후 90년대 초
   116                                       3. DSSS와 Code기론
                                                               U


에 미국의 Qualcomm사에서 개발되었고 그것이 얹）년대 중반어］ 한국에서 최초로 상
용 서비스를 하게 되었다. 당시 세계에는 TDMA라는 기술이 유럽 등지에서 사용되
고 있었으며, 특히 유럽의 GSM과 DECT는 10년 이상을 상용에서 사용되던 시스
템이라서 자연스럽게 비교가 되고 개발기술과 운영기술이 이미 어느 정도 단계어］
있는 TDMA방식에 비해서 확산통신 방식은 초라하게 보일 수 있었으나, 이 기술은
분명히 기술발전 선상에서 봤을 때 TDMA보다는 진보된 기술임에는 틀림이 없었
기에 현재 진행되고있는 3세대 통신의 瓜'ff2000에서는 확산 스펙트럼 방식이 표준
으로 사용되고 있다．
 앞으로 이 장에서는 이러한 확산 스펙트럼 통신 방식의 원리와 특징어］ 대해서 자
세하게 공부하게 될 것이다．



         read Spectrum
                                                               )
 확산 스펙트럼 통신방법은 크거］ 직접 확산 스펙트럼（DSSS : 1玉rect Code
Spread specti끄m)과 주파수 도약 스펙트럼（FHSS : Frequency Hopping Spread
spectrum) 2종류가 있으며, 주파수 도약 방식은 항공기간의 혹은 항공기와 지상간
어］ 중요한 통신내용을 교신할 때 사용되었으며, 현재 우리가 사용하고 있는 PCS는
이것과는 다른 직접 확산 통신 시스템을 사용하고 있다．
 확산 스펙트럼（Spread Spectrum)은 일반적으로 전송할 정보신호의 대역폭보다
훨씬 큰 대역폭을 통해서 신호를 전송하는 방법이다. 이러한 생각을 실현하기 위해
서, 즉 정보데이터를 확산하기 위해서는 정보 Bit보다 훨씬 빠른 변조 Bit를 곱해
주면 이러한 확산은 이루어진다．
 이러한 확산통신과 비교되는 또 다른 통신의 기술이 다중화(M毗iple油ig）이다．
다중화 처리를 위해서는 각각의 정보들을 고속으로 샘플링하는 처리를 거치게 되면
이것 역시 상당히 넓은 대역을 사용하여 통신을 하게 된다. 즉 30KHz의 개별적인
정보를 El급이나 Ti급으로 다중화하게 되면 훨씬 빠른 전송속도가 되며, 훨씬 넓
은 대역을 사용하여 통신하게 된다. 그러나 이것은 확산통신이라 하지 않는다. 이것
은 전송하려고 하는 정보량이 30K1七대역폭의 신호 여러 개를 합（合）한 것이므로
광태역으로 전송되기는 하나, 하나의 정보가 확산되어서 전송되는 확산통신과는 구별
    3. DSSS와 Code이론
1                                                             117

된다． 예를 들어서 버스를 타고 많은 사람이 이동하는 것과 버스 크기의 Limousine
을 한 사람이 타고 이동하는 것이라고 생각하면 될 것이다．
    이 책에서는 이러한 직접확산 시스템에 대해서만 자세히 공부하고 주파수 도약방
법에 대해서는 간단하게 언급하겠다．


     3.1.1 Frequency Hoping과 Direct Sequence

    주파수 도약（Frequency Hopping）과 직접확산（Direct Code Spread Spec甘urn)
은 전송파의 성분 중 어느 성분에 확산용 코드가 변조（곱해지는가）되는가어］ 의해서
구분되는 방식이다．
    전자기파를 이용한 통신에서는 정보의 변화량을 전자기 신호어］ 태응小1apping)
시켜 주는 작업과 이러한 八4appir垠신호를 복원하는 작업이라고도 정의할 수 있다
（이러한 정의가 학술적으로 가장 정확하지는 않을지라도 필자가 이야기하려고 하는
내용에 비추어 볼 때 어느 정도 타당성은 있으리라 생각한다）. 결국 정보를 전송신
호어］ 대응하는 방법은 전송신호의 변화 성분인 진폭 주파수, 그리고 위상어］ 전송할
수가 있다. 이러한 통신 방법을 각각 AM(Amplitude Modulation), FM(Frequency
八4od끄lation), PM(Phase Modulation）이라고 부른다.



                      S仕) Acos (o材 + 冽                DSSS
                      Acos 佃(t) o材 + 冽                刃.Iss
                      여기 에서
                       s(t) : 확산용 Code
                       Acos(ctt+ 砂 : Carrier Signal


                      （그림 :3-1) DSSS와 FHSS의 수학적 표현


    이야기는 여기에서 끝나지 않는다. 이러한 방법과 마찬가지로 전송하는 신호, 즉
Carrier Signal어］ 잡음과도 같은 성질을 가지는 코드를 대응시킴（곱한다）으로 그 전
송신호가 잡음과 같은 코드신호의 변화 형태를 싣고 전송되게 하는 것이다. 즉 그러
한 변화형태를 변조신호의 진폭에 대응시켰을 때에는 이것을 우리는 직접확산이라
고 하고 그것의 변화 형태를 주파수어］ 대응시켰을 때에는 주파수 도약방식이라고
   118                                               3. DSSS와 Code이론
                                                                       U


이야기한다．
 다시 말하면 랜덤한 확산용 코드를 전송신호어］ AM의 형태로 대응시킨 것을 직
접확산， FM의 형태로 대응한 것을 주파수 도약방식이라고 한다. 주파수 도약방식
어］ 대해서는 다음 기회어］ 자세히 공부하도록 하자．


  3.1.2 확산통신 : Direct Code Spread Spectrum

 일반적으로 잡음신호는 광대역어］ 걸쳐서 분포하며, 그것의 특성이 랜덤하여 통계
적으로 해석할 때 평균이 '0' 인 형태의 신호이다. 이러한 형태의 신호를 기존어］ 전송
할 신호어］ 곱하여 전송하는 경우에 기존의 신호는 잡음으로 변조된 상태라고 할 수
있다. 이렇게 변조된 신호는 전송 채널상에서는 마치 잡음신호와 같이 전송되어서
수신단까지 전송이 되고 이러한 신호를 수신한 수신기는 변조된 잡음의 헝태를 이
미 알고 있으므로 Coherent Detection을 통해서 원 신호를 찾을 수 있다. 이것이 확
산통신의 개요이다. 즉 신호를 잡음인 것처럼 해서 잡음의 환경어］ 노출시켰다가 이
렇게 함으로 잡음으로부터 보호한 후 신호를 복원한다는 개념이다. 마치 태조 왕컨
이 공산（公山）에서 백제에게 패한 후 적군（백제 군졸）의 복장으로 적진을 빠져나온
것과도 같은 개념이라 할 수 있다．
 이러한 방식은 기본적으로 잡음을 제어해보겠다는 생각이다. 그러기 위해서는 우
리가 변조하는 잡음신호의 정보를 수신단에서 알고 있어야 하듯이 만약 우리가 모
든 형태의 잡음신호를 알고 있다면 우리는 모든 수신된 신호에서 잡음을 제거할 수
있는 기술을 가질 것이다. 이러한 가정 자체가 무의미한 것이지만 이야기를 하다 보
니 가장 원칙적인 이야기를 다시 확인하게 퇸 것이다．
 따라서 확산통신 방법은 이미 변조된 신호를 한번 더 （확산）변조하는 기술이라고
이야기할 수 있다. 좀더 구체적으로 얘기하면 기저대역 변조와 확산 변조를 순서적
으로 실시한다는 것이다. 이러한 사실은 （그림 3-2）의 식을 통해서 확인할 수 있다．


                                                  ,．』 기저대력   변조를
         확산변조를 위한
         확산용 코드의 "l
         간 함수
                      Es
                           (t)
                                 妗cos   to恥社YUj
                      （그림 3-2) 확산 변조의 신호 표현
     3. DSSS와 Code이론
 U                                              119


  즉 이러한 두 번의 변조는 각각 그것의 사용 목적이 다른데 하나는 신호를
sinusoidal 형태로 入4appii坦하는 기저대역의 변조외． 전송대역을 확산하는 형태로
구분되어 생각할 수 있다．
 （그림 3-2）에서 s(t)는 확산 변조를 위한 확산용 코드의 시칸함수이며, 이것은 코
드의 특성어］ 따라서 목적이 다르나 일반적으로 많이 사용하는 코드가 뒤에 설명될
최장 코드인 PN Code나 최장 코드의 변형형태인 （拍id Code 등이 사용된다. 이러
한 확산용 코드가 전송신호의 진폭의 변동성분으로 표현되어졌으므로 이것은 직접
확산 변조의 형태라고 할 수 있다．
 P(t）의 경우 이것은 전송신호의 위상변화 성분에 대응되는 형태이며, 여기의 신호
가 천이 방식으로 대응되는 디지털 변조방식으로 표현된다고도 할 수 있다. 그렇다
면 위의 식은 기저대역 신호를 QPSK(Qi坦dra加re Phase Shift Keying）이든
BPSK(Bi- Phase Shift Keying）이튼 디지털 변조가 이루어진다고 할 수 있다．
 이렇듯 두 가지의 변조가 이루어지고 있으며, 이것은 전송신호의 위상과 진폭어］
각각 변동을 주는 형태임을 알 수 있다．


     3.1.3 확산의 의미

 확산의 처리는 앞서 이야기한 대로 전송대역을 정보전송어］ 필요한 대역폭보다 훨
씬 넓게 사용하는 것이다. 이것을 시간의 관점에서 본다면 확산 변조를 위해서 곱하1
지는 신호가 훨씬 속도가 빠른 펄스신호로 곱해질 것이라는 것을 알 수 있다. 우리
는 앞서 2장에서 이러한 펄스어］ 대해서 Fourier 변환을 구해본 적이 있다. 여기서
구한 결과식, 즉 주파수 영역에서의 펄스신호의 형태는曲w(f）함수의 형태로 나타
났다．
 이러한 S勿兀함수는 주기함수이며, 그것의 주기는 시간 영역에서 펄스의 폭이 반
복되는 주파수의 정수배가 되는 주파수에서 Zero Cross하며, 그것의 값은 주파수가
증가될수록 계속 감소되어 감을 알 수 있다．
 （그림 3-3）에서 보는 바와 같이 펄스는 그것의 폭어］ 의해서 Zero Crossir堆하는
주파수의 위치가 다르게 된다. 즉 펄스의 폭이 크면 클수록 처음으로 zero crossing
하는 위치는 낮은 주파수에서 이루어질 것이며, 폭이 작을수록, 즉 펄스가 빠를 수로
zero cros前ng하는 지점은 큰 주파수의 값이 될 것이다. 여기에서 이야기의 주제가
되고 있는 zero crossir坦하는 첫 번째 지점은 그때까지의 스펙트럼 밀도를 보면 디：1
   120                                                                                               3. DSSS와 Code이론
                                                                                                                       1


                         x(t)


                                A1




                         口                         t



                                               丁斗，(1｝
                                                    和希df
           -T/ 2                     T12                                   -2/T\ _/-1/T 0 1/T '\ Y2/T




                                           //\ , 1t I 5 T/2                                    sinirfT
   玎t) = A rect 仕／T)                   =                                     X(f) = AT
                                                                                                irfT
                                           \0. I t I 2 T/2                           = AT sinc(fT)

                                               （그림 3-3) 펄스의 Fourier 변환


체로 큰 값임을 알 수 있다. 이것을 더욱 명확하게 하기 위해서 전력 스펙트럼 믿도
를 나타내는 （그림 3-4）로 계속 설명을 하겠다．

                                                                                       IXi(끼 2



                                 A1 x (t) = A rect (ilT)




            -T12                     T/2                                    -2/T       -l/T 0    itT     2/T


    ETOT= J繭꼬I拉斗뇨，.,..,
                           （刃



                                                                                         r
                                                                                             전력밀도 함수는 시간 축이나 주



              J
                            00                   r1 q)                                       파수 축에 관계없이 그것의 크기
                                                                                             를 제곱하여 무한 주기 동안 적분
    ETOT           JIX           (f)I2df   =           /ATsinc(刀/   2d1=       A2T
                                                                                             하면 구해진다．
                         r1l/T

           E' = J규ATs加(I-끼' 心羽口孔42T)＞万T.何卯易

                          （그림 3-4) : 펄스의 전력 스펙트럼 표현과 전송 대역폭


 （그림 3-4）의 전력 스펙트럼 밀도에서 알 수 있듯이 펄스의 주파수 성분들의 전
력은 FZCP(First Zero Crossing Point）어］ 약 90% 이상 집중되어 있다는 것을 알
    3. DSSS와 Code이론
.


수 있다. 즉 （그림 3-4）에 나타나는 펄스를 전송하기 위해서는 모튼 고조파 성분을
모두 통과시켜 주는 필터를 설계하고자 한다면 무한대의 대역폭이 지원되어야 하나
그것이 이상적이어서 불가능하다고 한다면 어느 정도의 trade off를 통해서 일부의
고조파를 포기하고 90%의 전력어］ 포함된 고조파만을 사용한다면（즉 그러한 전송채
널 혹은 필터를 통과한 신호는 제외된 고조파 성분만큼 외곡될 것이다） 신호의 통
과 대역폭은 FZCP까지의 대역폭으로 제한하여 사용할 수 있을 것이다．


    디지털 신호의 전송 대역폭
    이상과 같이 펄스를 전송하기 위해서는 모든 고조파를 전송할 때 무한대의 전송
대역폭이 필요하나 FZCP까지의 대역어］ 90% 이상의 전력이 집중되어 있으므로 우
리는 이러한 점을 생각할 때 디지털신호의 대역폭은 일반적으로 FZCP까지 사용한
다. 이러한 논리가 타당성을 가지는 또 다른 이유는 송신단에서 찾을 수 있다．
    앞서 2장에서 공부한 임펄스에서 임펄스는 그것의 변화량（기울기）이 무한대인 신
호였다. 즉 시간축에서 아주 짧은 시간어］ 아주 크거］ 변화하는 신호는 주파수에서는
아주 넓은 주파수대역에 걸쳐서 전송된다는 것을 임펄스를 통해서 알 수 있었다. 따
라서 （그림 3-4）의 펄스에서 아주 Sharp호｝edge를 가지는 펄스는 이러한 edge성분
이 대분분의 높은 고조파（FZCP보다 큰 주파수）어］ 의한 것이라는 것을 알 수 있다．
그러므로 송신단에서 이상적인 펄스를 만드는 것 자체가 불가능한 것이므로 송신단
의 펄스 자체가 무한한 고조파 성분을 포함하는 것은 아니다．
    이러한 이유로 인해서 디지털 신호의 전송대역을 펄스의 폭, 즉 펄스의 전송속도
와 같다고 할 수 있을 것이다．

                i尸H           山   小   m小




                      Band功k社h = Channel I入就a Rate



    추가적으로 여기어］ 발진기（Oscillator）의 주파수 오차범위가 추가될 것이며, 전송
되는 데이터가 어떠한 스펙트럼 효율을 가지는 변조기에 의하써 전송되는가어］ 따라
서 다시 그것의 대역폭을 정의할 수 있다．

         B＝凡＋2f                                      (3-1)
           n
   122                                                            3. DSSS와 （兀de이론
                                                                                    U


 여기에서 B는 태역폭이고, Rd는 데이터 전송률이며, n은 사용하는 변조기의 스펙
트럼 효율이며 (BPSK인 경우 1이며, QPSK인 경우 2), 스／는 전송 주파수의 변동
폭이다．
 어찌 되었튼 우리는 지금까지 공부한 것들에서 펄스폭이 작아서 펄스의 변화가
극심한 혹은 펄스의 전송속도가 빠른 신호는 넓은 대역으로 전송될 수 있다는 것을
확인했다. 또한 넓은 대역으로 전송되는 데이터는 아주 빠른 데이터 율을 가지는 더］
이터라는 것을 알 수 있다．


                                                                 注町기2




             -2/1                 2/ T              fo-11T       fo+IIT


                                                                 냐町기2

                                         明二＝ >    i可'可“'
                        jA
                                  T/ f
         미          1        "=
                                         卜   t                            f
                                                 和lIT        '       乙＋1/T

              （그림 :3-5) 시간 영역의 전송속도와 주파수 영역의 대역폭


（그림 3-5）는 시간 영역의 전송속도와 주파수 영역의 대역폭의 관꼐를 비교할 수
있도록 하는데 정보 데이티가 확산통신을 위해서 대역확산을 하기 위해서는 전송되
는 데이터의 빠르기를 증가시켜 주면 퇸다는 것을 알 수 있다．

  3.1.4 왁산통신의 정량적인 해석

 지금까지는 확산 스펙트럼의 정량적인 특징어］ 대해서 공부하였다. 이 절에서는
지금까지 공부한 내 Q。들 을 좀더 상세하고 구체적으로 공부하기 위해서 정량적인 해
석을 할 것이다．
    3. DSSS와 Code이론                                                                         123
1                                                                                       1

    DSSS(Direct Code Spread Spec打urn）의 처리를 거친 정보신호의 표현 식은 다
음과 같이 표현될 수 있다．

          V(t) =g(t)s(t) =Pg(t)d(t)cos w0t                                                   (3-2)

    여기에서 的） 확산 변조를 위한 PN Code이며 d(t)는 전송될 데이터 신호이다．
일반적으로 g(t)의 Chip rate 五는 d(t)의 bit rate 兀보다 엄청나게 크며 이것은
g(t)를 매우 빠른 데이터로 함으로써 광대역어］ 걸쳐져 있는 데이터로 만들어서 마
치 이상적인 잡음의 형태로 접근시키기 위함이다. 이러한 변조절차를 거쳤을 때
V(t)는 /,＞九이므로 玖t)의 모양이 g(t)와 같은 모양일 것이다．
    즉 어떠한 정보 데이터라 하더라도 확산 변조가 이루어진다면 그 결과는 확산 변
조를 위해서 사용되는 확산코드의 모양으로 될 것이라는 것이다. 결국 확산 변조된
신호는 확산 변조용 코드의 형상만 남아 있고 자신의 정보는 숨어 있게 된다．

                                                                         n
                                                                         小
                                                                                 H口口




                     확산용 PN 코드 아t)




                        정型 데아터 d(t)


                                                                                                  十
                                                                                                  ：:! 三
                                                                                                  m
                                                                                                  :
                   확산변조된 정보 아t)d(t)



                        （그림 3-6) 확산 변조된 정보 마의 형태


    이것은 어떤 면에서는 여러 개의 정보 데이터가 하나의 광대역의 신호어］ 묻혀서
전송되는 다중화의 형태라고도 생각할 수 있다． 이 이야기는 기지국의 출력신호와
단말기의 출력신호는 마치 잡음을 출력하고 잡음을 수신하는 형태의 통신이 이루어
질 것이다．
                                           잡음 n(t)

                                                                                 적 분기
            d(t)
                                                     V,(t)                   Vo(t)


                     Ps cosn砒   g(t)   !         ;           g(t)   I：눔 coso力t


           （그림 3-7) 확산 변조와 병행된 BPSK 변조신호의 전송과 복조
   124                                               3. DSSS와 CodeOl론 U



 이러한 확산 변조와는 별도로 또 다른 디지털 변조가 이루어지는데 이 두 가지의
변조는 어떤 것이 먼저 이고 어떤 것이 나중이고 하는 식의 순서는 별 의미가 없으
나 여기에서는 디지털 변조 후 확산 변조를 하는 것으로 생각하1 보자. 또한 이러한
디지털 변조는 BPSK를 수행한다고 하자．
 （그림 3-7）에서 나타나 있듯이 전달하고자 하는 신호 d(t)는 BPSK 변조된 후
확산용 PN（뇨le어］ 의해서 한번 더 변조된다. 또 복조 과정에서도 확산용 PN Code
어］ 의해서 먼저 복조 되고 BPSK 복조가 이루어진다고 하자. 그림어］ 나타난 전송과
정의 Noise는 확산기술에 의해서 재생신호어］ 영향을 주지 아니하며, 재생신호는 확
산신호 자체에도 영향을 받지 아니한다．
 （그림 3-7）과 같이 전송 경로상어］ 잡음 혹은 拓mming을 가한다고 했을 때의 상황
을 생각해 보자． 위의 그림의 Noise n(t) 대신어］ normalized power가 乃인
sinusoidal파어］ 간섭을 받는다고 하자. 일반적으로 잡음은 전송정보 신호의 모든 부
분어］ 컬쳐서, 즉 진폭, 위상, 주파수어］ 영향을 준다. 따라서 잡음신호는 다음과 같이
표현할 수 있다．

                                             전송정보의 위상에 변화
                                             를 주는 성분
             전송정보의 진폭애                 1r1

             변화를 주는 성분
                            Pj t OSj(4唯F q
                                             전송정보의 주파수에 변
                                             화를 주는 성분


                     （그림 3-8) 잡음신호의 수학적 표현


 이때 수신단으로 입력되는 수신신호는 정보신호와 채널에서 추가퇸 잡음 혹은
Jammit培신호의 합의 형태이다. 즉

         V1 = Pd(t)g(t)cosw。        t + 0)
                           t +Pcos(w。                             (3-3)

 입력단에서는 우선 확산성분을 복조하기 위해서 송신단에서 변조어］ 사용된 PN
Code와 동일한 PNCode g(t）를 식 (3-3）어］ 곱한다. 이후어］ RF Carrier 성분 역시
제거하기 위해서 동일한 신호성분을 곱하게 된다. 여기에서 곱한다는 것은 수학적
으로 그렇게 표현될 수 있으나 실지로 시스템의 구현상에서는 위상과 주파수 정보
를 알고 있는 가운더］ 복조가 이루어지는 Coherent detection을 하게 된다. 이렇게
복조과정을 거치게 되면 복조되어서 저역 통과 필터인 적분기어］ 입력되는 신호는
U
    3. DSSS와 Code이론                                               125
                                                                          I
다음과 같다．

         VO = f- d(t)(1+ cos2wj) +Pg(t)(l + cos2따t)cosO +Pg(t)sino。
                                                                  tsin8
                                                                    (3- 4)

 식 仔4）은 저역 통과 필터인 적분기를 통과하게 되면 고주파 성분들인
sinus아dal형태는 모두 없어지게 되며, 다시 정리하면 식은 다음의 식 仔5）과 같이
간소화된다．

                                       Single Tone


         %＝只d(t) 葫餉，雨／                 끕’erference                  (3-5)
                                       m1lterferenCe
                                       성분



 주목할 것은 식 (3-旬에서 앞 항의 정보성분에는 d(t) 성분은 포함하고 있으나 간
섭성분은 없으며, Jamming 신호는 오히려 광대역 신호로 나타난다. 이것으로 변조
과정에서 정보신호어］ 확산신호로 한번 더 변조하여 전송한 신호는 복조과정에서 확
산신호로 한번 i:] 복조하는 과정을 통하여, 전송 도중의 간섭신호로부터 효과적으
로 보호받을 수 있다는 것을 다시 한번 보여 주는 것이다．
 그렇다면 과연 Jamming 신호로부터 보호되는 것은 무엇과 관계 있는지를 생각
해 보자． 적분기를 통과한 신호의 표현인 식 (3旬에서 간섭성분의 Power Spectral
Densi打는／如的Correlation의 Fourier Transform으로 구할 수 있다는 것은 2장
의 Parseval의 정리에서 공부했다. 이렇게 구한 식에서 이 신호가 九인 cut-off주

파수를 가지는 저역 통과 필터인 적분구간이 兀인 적분회로를 통과할 때 다음과 같
이 정리된다．


         G＝乷' " ; 1피듸月                                              (3- 6)


 이렇게 구한 Power Spectral Density는 에러 확률함수어］ 적용되어진다. 일반적
으로 에러는 랜덤하게 발생되므로 확률함수로 표현된다. 즉 에러가 발생할 수 있는
확률로 그것의 성능을 이야기할 수 있다는 것이다. 이러한 에러확률을 위해서는 어］
러가 발생될 수 있는 확률의 분포함수가 정의되어야 한다. 이러한 확률분포함수어］
서 확률을 구할 수 있으며, 확률은 분포함수의 적분값으로 나타난다．
 즉, 확률분포함수의 전구간에서의 적분값, 즉 면적은 1이다. 또한 발생될 수 있는
값은 확률분포함수에서 구간의 범위어］ 존재할 확률로 나타난다. （그림 3-9）는 확률
   126                                                                               3. DSSS와 Code이론
                                                                                                       1


분포함수와 확률을 나타내는 것으로 여기에서 이야기할 Bit 에러 확률은 정규분포
의 형태로 나타나므로 정규분포의 경우를 예로 들어서 나타낸다．

                                                        확률                     확률이 작아지는 방향
                                                                               H
                                                                     寸1=
                                                                           =




                                                                   1는 방향




                                                                                        변량
                                                                           \


                                      （그림 3-9) 확률 분포 함수와 확률


 여기에서 e仄乂功는 Gaussian확률분포함수의 발생확률을 표현해 주는 함수로써
그림의 빗금 친 부분의 적분값, 즉 일어날 확률을 尤의 함수로 표현한 값이다. 여기
에서 알 수 있듯이 尤값이 클수록 확률값은 점점 작아지게 되며, 이것과 반대되는
개념이 en佃）라고 있다. 이 내용은 2장에서 공부한 바 있다．
 이러한 에러가 발생할 확률은 전력과 관련이 있을 것이며, Power 匐玭tral
Density는 이러한 이유로 다음과 같이 정리된다. 식의 중간 전개과정은 생략하고
Bit 에러율은 다음과 같다．


                                                                                                (3- 7)
         P-
              _
                  _
                      1e叱
                            Ci/
                                  p   \'fb
                                             'f   1jO
                                                        I, ,   1
 각 0는 정보신호를 전송하는 Carrier 신호의 위상과 Jamming 신호간의 위상각
이다. 이러한 위상각의 차이는 임의의 값（Random Variable）이다. 여기에서 日가 45
도인 경우의 Jamming 전력을 유효전력이라고 하고 이것과 Jamming Power간어］
는 다음과 같은 관계가 있다．

                                                                                                (3寸8)




 위의 식 (3-助에서 동일한 Jamming 전력 乃에서 兀仇가 클수록 유효 Jamming
전력 乃，町는 작아진다． 즉 九어］ 대한 九의 값이 커지면 유효 Jamming 전력，
尸／,elf. 가 작아진다는 것이며, 이것은 확산용 PN Code의 Ch如（B出 Rate가 정보 더］
    3. DSSS와 （兀de기론                                                         127
U


이터의 bit rate보다 훨씬 크다면 유효 Jamming 전력은 확실히 감소한다. 여기에서
우리는 Processing Gain （和를 식 (3이와 갇이 새롭게 정의한다. Qualcomm's
Engineering Handbook에서는 이것을 Spread Factor, 즉 확산계수라고도 한다. 식
仔9）은 확산처리 과정을 통하여 원래 정보 데이터가 얼마나 빠른 데이터로 혹은
얼마나 넓은 대역으로 확산되는가를 나타낸다는 측면에서 확산졔수라는 말도 나름
대로 타당성이 있다．

         ／기   H


         '-7尸 = 二m
                       /;                                                    (3-9)
                       Jb

 특히 이러한 DS-SS 통신방법은 PN Code의 Chip Rate가 빠를수록 Jamming어］
강하다는 것을 알게 되었다. 그러므로 우리는 Ch如 Rate가 데이터의 Bit Rate어］ 비
해서 상당히 빨라야 하며, 각 Code간의 Au切＜沁rrelation값을 위해서 그것의 주기
또한 충분히 긴 Code가 필요함을 알았다. 이러한 특징은 거의 완벽한 Noise의 특징
을 갖기 위함이다．
 또한 DSSS통신은 전송한 신호의 대역을 미리 충분히 넓혀서 Power Spectral
Density를 낮춘 후 전송하여 수신단에서는 거의 White Noise 레벨 혹은 그 이하의
레벨로 수신되어 송신시 대역을 넓힐 때 사용한 방법을 역으로 사용하여 수신된 신
호의 대역폭을 좁힌 후 Power Spectral Density가 충분히 커지면 일반적인 통신방
식으로 복조하여 정보를 검출하는 방법이다.

                                셔                  T = Ni           0

                  A

                       t
                            +       4尸
                                                                        T


                  -A
                                     （그림 3-10) 마ocessing Gain의 설명
                                         3. DSSS와 Code이론
I11
       128                                                 1


      이러한 논리어］ 의하면 대역폭이 충분히 넓으면 아주 낮은 신호대 잡음비（SNR :
Signal to Noise R毗幻뻐］서도 통신이 가능하다는 결론이 나오며, 이는 이미 Shannon
 의 Channel Capacity 이론어］ 의해서도 공부하였다. 아래와 갇이 입증이 퇸다．
      （그림 3-10）에서 보는 바와 같이 확산 스펙트럼은 정해진 전력을 어떻게 전송하
느냐로 기존의 방식들과 구별될 수 있다. 즉 정보데이터가 가지고 있는 에너지를 넓
은 대역어］ 골고루 분배하여 전송할 것인지 아니면 좁은 대역어］ 에너지를 몰아서 전
송할 것 인지의 문제이다. 즉 대역폭과 그 대역에 존재하는 에너지의 총합이 전체
에너지라고 했을 때 （그림 3-10）와 같이 사각형의 가로를 길게 할 것인가 아니면 서］
로를 길게 할 것인가의 문제이다. 이런 측면에서 주어진 정보 데이터의 에너지에서 정
보의 전송은 대역폭을 넓게 할 것인가 전력을 크게 할 것인가의 선택 사항인 것이다．
      이러한 주파수상의 문제는 시간축에서 관찰될 때는 그 펄스의 폭이 훨씬 빨라지
는 것을 의미하며, 이것은 정보의 전달이 단순히 1과 0으로 전달되어지는 디지털의
경우에 동일한 정보가 훨씬 짧은 시간어］ 전달되어야 한다는 것을 의미한다. 정보의
전달은 신호의 유（" l " ) 혹은 무（"0"）라는 측면에서 그것을 표시하는 시간이 그 정보
를 전송하는 대역폭이라는 생각에서 이러한 사항들을 해석해볼 때 지극히 타당한
결과라고 할 수 있다．
      이상과 같은 결과로 볼 때 확산통신의 처리이득은 대역을 비상식（7）적으로 넓게
사용해서 정보를 전송함으로 더 빠른 시간어］ 정보를 전송할 수 있는 것을 얻게 되는
 것의 이득을 말하는 것이다．
      중국의 송나라 때 저공（狙公）이 자신이 키우던 원숭이에게 먹이를 주는뎨서 유래
 되었던 조삼모사（朝三暮四）라는 말이 생각이 난다. 자신이 키우는 원숭이들에게 아
침에 3개, 저녁어］ 4개씩 먹이를 주겠다고 하자 화를 냄으로 아침어］ 4개, 저녁어］ 3개
씩 주겠다고 하니 원숭이들이 기뻐하였다는 이 고사는 잔꾀로 남을 속인다는 이야
기인데, 결국 전체의 신호 에너지를 시간 축상에서 나누어 보내느냐, 그렇지 않으면
주파수 축상에서 나누어 보내느냐라는 관점에서 본다면 조삼모사라는 고사와 그것
의 의미가 통하지 않나 생각이 된다．
      그런데 우리는 여기서 다음과 같은 점을 생각해 보자. 우리가 먹이를 먹는 것은
몸어］ 필요한 영양분을 공급하기 위함과 혀로 그것의 맛을 느낄 때의 욕구충족 등
또 다른 기타의 요인이 있다고 한다면 먹이를 결국 7개를 먹는다는 것은 그 현상의
하나의 단면일 뿐일 수 있다는 것이다.
    3. DSSS와 Code이론                                           129
1


    예를 들어서 아침에는 하루 종일 일을 해야 함으로 되도록이면 많은 먹이를 먹을
수 있도록 하고 저녁에는 반대로 운동량이 없으므로 적게 먹게 하는 것은 나름대로
이유가 있는 것이다. 마찬가지로 확산 시스템이 결국 자원을 여러 사용자에게 나누
어주는 입장에서는 주파수를 일률적으로 나누어주는 것이나 별반 다른 거］ 없다 할
지라도 우리가 그것의 성능을 제어할 수 있다고 한다면 우리가 tradeo卄해서 얻는
이득은 그것이 조삼모사와 유사한 현상이라 하더라도 또 다른 해석이 충분히 있을
수 있을 것이다．



    3.2 CDM/CDMA 통신방식

    CDWCDMA(Code Division Multiplexing/Code Division Multiple Access)
통신방식은 새로운 미래의 통신으로 떠오르는 방식으로 IMT-2000 등의 통신에서
사용하게 될 다중화／다중접속 방식이다. 이 책에서는 이러한 명칭을 단순히 CDMA
시스템으로 줄여서 이야기하겠다．


     3.2.1 확산통신과 기존의 통신

    기존의 통신방식은 각각의 통신로의 독립성을 보장하1 주기 위해서 주파수 자원을
나누어서 채널을 이루어 주었다. 이러한 방식은 스펙트럼 효율을 고려할 때 하나의
채널어］ 많은（넓은） 대역을 할당해 줄 수 없었다. 따라서 이 방식은 상대적으로 확산
통신에 비해서 협대역일 수밖어］ 없다．
    이렇게 사용된 대역은 채널환경에서 각종 여러 가지의 모든 잡음신호로부터 정보
데이터를 보호하기 위해서는 주어진 대역폭에 충분한 에너지가 집중되어 있어야 했
다． 여기에서 잡음은 모든 헝태의 잡음을 통칭하는 것으로 인접채널의 간섭도 포함
되는 것이다. 이러한 방식의 통신방식은 （그림 3-li）과 같이 설명될 수 있다.
（그림 3-11）에서 보면 알 수 있듯이               RF단에서의 SNR이나 기저대역에서의
SNI｛이 같게 나타나며， 이때 흥미 있는 것은 잡음어］ 비해서 정보의 에너지가 충분
히 커야 재미있는 것은 기존통신이나 확산통신이나 정보의 에너지는 갇을 것이나
이것이 전송되는 채널 상에서는 11七로 에너지를 정규화 했을 때어］ 에너지가 확산
통신에서는 훨씬 낮게 나타나게 된다. 즉 확산통신 방식은 정보의 에너지를 조금씩
나누어서 각각의 넓은 대역어］ 골고루 분포시켜서 전송하는 것이다．
                                                                                          3. DSSS와 Code이론
  130                                                                                                        .



 이러한 사실은 확산통신 방법이 채널효율을 고려해야 한다면 전력（출력）을 엄격
히 제한해야 되는 시스템이라는 것을 말해 준다. 이러한 사실은 기존의 시스템이 스
펙트럼의 사용을 엄격히 제한했던 것과는 구별퇸다. 이 두 시스템은 주파수 대역폭

          Baseband Spectrum                                                RF Spectrum




             니 尸2B11
                 f나                                                                   A




               -13    0
                                                                                               f


               !
                                    잡음 Spectrum

                                     N0 watts/ Hz
                                                                                채널


                                                                                4
                                             fo

             Demodulation                                                 수신된 Spectrum

                " JJ
             斗口，中＝ii                                              0              f0
                                                                                               f
          (S/ N)data = (S/ N)RF                             (S/ N)RF = (AW) /(N0W) = PS/ 1뇨


                                    （그림 3-11) 기존의 통신방식


         Baseband Spectrum                                  P8= A1W=A0B RF Spectrum

                              A


            거  -B    0 B
                          卜   '-   2B,

                                    J
                                          II나
                     PJ=N0W
                                         Jamming Spectrum
                                         \\N0watts/    Hz
                                                                                      平
                                          1   )
                                             m\



                                                                      F    斗              채널




        Demodulation Spectrum
                                                  /。
                                                                                      4
                                                                              수신된 Spectrum




                                                                          土
                                                                                          w

                                                                  “
                                                                                                     f
                                                              픗
                                                                                           1

                                                                                          fo
  (S / N)data=(AOB) / (NoB)=(W/ B)(S/ N)ss=(PG) (S/ N)ss                  (S / N)00 = (A川) / (N。
                                                                                               W) = PSI PN

                                   （그림 3-12) 확산 스펙트럼 방식
    3. DSSS와 Code이론
1


과 이러한 대역어］ 할당되는 출력간의 Trade off를 한 시스템들이라고 말할 수 있다．
이러한 점을 생각하1 볼 때 전송하는 정보의 양과 그 정보의 에너지는 같은데 그것을
주파수 대역을 제한하면서 전송하느냐, 아니면 전력을 제한하면서 전송할 것인가의
차이이므로 어떤 것이 더욱 용이하게 시스템 성능향상이 가능하냐어］ 따라서 그것의
성능이 판단되어야 한다．
    미래의 무선통신 방식에서는 기존의 방식들은 새로운 방식인 확산통신 방법으로
그것의 무선구간을 설꼐하고 있는 것이 일반적인 추세이다. 우리가 잘 알고 있는
IMT-2以刃의 경우 동기식과 비동기식 2가지의 방법으로 구분되나 이 2가지 모두
확산통신 방법의 내용들이다．


     3.2.2 CDMA 통신방식의 정량적 해석

    Mul如le Access에 있어서 각각의 사용자에게 원하는 신호를 접속시켜 주는 것
은 각각의 사용자를 주파수로 구별하여 주느냐, 시간으로 구분하여 줘二냐어］ 따라
서 TDMA와 Fl呱4A로 구분할 수 있음은 잘 알고 있다. 여기에서는 주파수도, 시간
도 아닌 코드로 사용자를 구별해서 통신하는 방법인 CDMA통신방법을 생각해 보
겠다．
    일반적으로 확산통신 방식에서는 다중접속을 위해서 각각의 사용자를 별도의 새
로운 구분자 혹은 식별자로 구별시켜 주는 것을 코드를 사용하여 수행한다. 여기어］
사용되는 코드는 그 코드가 변조되어 출력될 때 출력이 엄격히 제한받아서 시스템
에서 요구하는 허용 신호대 잡음비, 즉 尻／N0를 유지할 수 있게 출력된다.
    정보신호를 대역 확장하는 방법에는 어떤 방법을 사용할까？ 정보신호 자체를 아
주 빠른 데이터로 변환시켜 주는 방법, 즉 정보 데이터의 속도를 증가하는 방법이
있을 것이고 정보신호를 정보신호보다 훨씬 빠른 신호로 변조해 주는 방법이 있을
것이다. 그런데 훨씬 빠른 정보로 변조한다면 어떤 신호로 변조해야 하는가에서 우
리는 특정한 성질을 가지는 코드로 변조한다는 생각을 할 수 있다.
    이때 고유한 코드들은 정보 데이터에 비해서 상당히 넓은 대역으로 확산되어서
전송되는 확산통신 방식어］ 적용된다. 확산통신에서는 전송되는 신호를 잡음과 유사
하게 만들어서 전송한다는 생각으로 수행되므로 코드 자체의 특징도 이러한 신호의
성격과 비슷하게 나타나는 코드로 적용될 것이다. 즉 여기어］ 사용되는 코드는 그것
의 발생 경우가 상당히 커서 거의 랜덤하며, 전체적인 값이 평균적으로 영어］ 가까운
   132                                                     3. DSSS와 Code이론
                                                                             .


경우라고 할 수 있다. 이러한 확산을 위해서 사용되는 가장 일반적인 코드가 최장
길이 코드 중의 하나인 PN Code이다. 이 코드는 그것의 변화형태가 상당히 다양하
며, 그것의 특징 또한 잡음과 비슷한 성격으로 나타나는 유사함이 많다．
 CDMA통신의 대표적인 Q凡ialcomm사의 CDMA의 경우 채널의 다중화를 위해서
서로 Orthogonal 코드인 Walsh Code를 사용하여 논리채널을 생성하기도 한다. 히
것은 확산용으로 사용되는 코드와는 달리 채널간의 구분을 명확하게 하기 위해서
직교성이 상당히 강조된 코드라고 볼 수 있다．
 CI呱4A의 동작을 설명하기 위하여 동일한 시간어］,k개의 가입자들이 동일한
Carrier 주파수 兀에서 전송하는 데이터와 DSSS spectrum을 사용하며, 특정 가입
자의 특정한 코드 蜀（t)를 정의하자. 이때 특정한 가입자는 다음과 갇은 형태의 신
호를 수신하게 될 것이다．

         V(t) =>只＆(t)町t)cos他사的                                        (3-10)
               i=   O


 여기서 각각의 신호는 수신단에서 동일한 Power PS로 나타난다고 가정하고, 각
각의 PN Code, 즉 g( t)는 동일한 chip rate I，로 표시되며, 임의의 사용자 1어］ 의
해 전송되는 정보 데이터는 呱t)로 표시한다. 물론 각각의 사용자 정보데이터의 더］

이터 전송속도는 九로 동일하다. 또한 0七 random phase로 통계적으로 다른 사
용자들의 각각의 위상어］ 대해서 독립적이다. 여기서 열적 Noise는 설명을 간단히
하기 위해서 고려 대상에서 제외시킨다．
 만약 수신자 k명의 신호를 수신하려고 한다면 k개의 상관기가 필요할 것이며 만
약 1번 가입자의 경우를 생각할 때 상관기에서 PN Code 신호 g1(t)와 정보 데이터
미（t) cos 恥t+ 目）가 곱해질 것이며, 이것은 고주파 성분을 제거하기 위해서 저역
필터인 적분기로 입력된다. 이러한 신호가 적분기를 거쳐서 고조파 성분이 모두 여
과퇸 후의 신호는 다음과 같다．

         V,,,l(r) = Pd1(t)+Z Pg1(t)g』(t)d1(t)cos(91 -Or)              (3-11)


 여기서 우리는 모든 瓠勿들은 동일한 시간에 전송된다고 본다. 이러한 경우
的（D, 蜀(t)의 곱은 어떤 g1( t)들이 가지고 있는 chip rate인 /，를 동일하게 가진
1
    3. DSSS와 Code이론                                                            [
                                                                                   133   I
다. 그리고 개별적인 針（勿들은 Random Code이며 自(t) g1(t)三g11( t)이다. 또한
cos(01- Oi）三cos日li라고 한다면 식 侶-11）은 다음과 같이 다시 쓸 수 있다．

         V。
          ,, (t) = 只띠（t) +Z只g1(加os011                                              (3-12)
                                                  i=2


    여기서 주목할 것은 식 (3-12）은 눈어］ 익다는 것이고 그것은 Single Tone
Interference에서 얻었던 식 仔5）와 닮았다는 것이다. 즉 이것은 Single Tone
Interference 대신어］ (k-i)개의 독립적인 간섭신호임을 알 수 있다. 그렇다면 앞 절
에서와 마찬가지로 간섭신호의 Power Spectral Density어］ 대해서 알아보고 아울러
에러확률을 찾아보자. 간섭신호의 Power Spectral Density는 식 (3-6）에서 몇몇
값의 변화만으로 구할 수 있다．
    식 (3-12）의 신호의 크기 PS는 나 이외의 (k-i)개의 신호의 크기이므로 잡음신호
인 乃와 같다고 생각할 수 있고， (k-i)개의 독립적인 간섭신호의 총 Power
Sj光ctral Density는 간섭신호 각각의 Power 匐玭tral Density의 (k- 1）배이다. 또
한 유효한 拓rnmrng신호의 위상이 45도 라고 할 때 간섭신호의 총 Power Spectral
Density는 다음과 같다．

         （力(J）三 休 卞1)中늣
         H   .   4   .   .   .   .   .        ,




                                                        IJ匡 Jb                     (3-13)
                                         j)
                     'l.Jc

    Bit Error Prob曲小ty는 식 仔7）에서 尸7=（左- 1)尸S로 생각함으로 다음과 같이
구할 수 있다．
                                                                 l보다 훨씬 큰 값
                                                                 일 1때1Pe값이 작
                                                                 아짐 .
                                                                                   (3-14)


    그러므로 확산 스펙트럼의 CDMA System에서는 다른 사용자들로 인해서 발생
되는 잡음신호를 포함하는 모든 잡음신호 간섭에서 낮은 에러확률을 유지하기 위해
서는 e寸 (功의 尤값이 1보다 매우 크면 된다. 즉 다음과 같다．


         唾）))（븅）                                                                   (3-15)
    이상과 같이 CDMA 통신방식어］ 대해서 생각하1 보았다. 결국 확산 스펙트럼 통신
의 CDMA System의 성능은 적어도 Pr（兀essing G沚n, （如，어］ 의해서 결정되어진
   1 34                                   3. DSSS와 （兀de이론
                                                            口


다. 즉 2배의 Processing Gain, G1，는 가입자 수 (k- i) 보다가 훨씬 커야 한다는
것이다. 예를 들면 1개의 Carrier和斗수를 사용하는 사용자의 수를 ioo명이라 하고，
음성 소스의 출력이 8Kbps라고 한다면 확산을 위해서 사용되는 코드의 Chip Rate
는 0.8入Thps보다가 훨씬 커야 한다는 것이다．
 만약 사용자수가 10명으로 줄어든 가운데 전송대역은 0.邵爪七로 그대로 사용퇸
다고 한다면 상대적으로 정보 데이터의 PG이 증대되는 결과이므로 Bit 에러확률은
현격하게 줄어들 것이며, 이것은 각 정보 데이터들의 출력을 더욱 낮추어도 된다는
의미가 될 것이다．
:, r: 拱好J 전송대역을 1.228融瓜七로 하고 하나의 채널당 할당되는 대역폭이
          301(1七로 할당되는 주파수 분할 다중접속（Fl呱4A) 방식을 사용하는
          시스템에서는 약 41개의 채널이 가용될 수 있다. 그렇다면 Vocoder
          source의 출력이 9.6kbps인 CI呱4A시스템에서 동일한 전송대역을
          사용한다고 할 때 이상의 FDMA시스템과 동일한 용량을 가질 때 얼
          마의 BER을 나타내겠는가9

          앞에서 공부한 식3-14로부터 가입자의 수와 까ocessing Gain을 대
          입하여 2장의 표 2-1의 값에서 데이터를 찾으면 퇸다. 즉 k=41, 玎fb
          = 128을 대입하여 계산식 3-14식을 2-50과 같은 형태로 수정하게
          되면 x = 3.6이 퇸다. 따라서 표 2-1에서 3.60일 때 에러확哥2侶．6)
          은 1.59 xm4이다．


   3.2.3 Jamming과의 전투

 일반적으로 CDMA방식의 확산 스펙트럼은 확산어］ 의한 Processing Gain을 통
하여 주위의 간섭이나 Jar跏ing어］ 강하다라는 것을 공부했다. 이러한 점은 CDMA
의 하나의 장점으로 이해할 수 있으나, 실제 Cl呱4A시스템에서는 이것을 고려하여
채널용량을 설정함으로 또 다른 장점이라고 하기에는 문제가 있고 Cl呱4A의 특징
이라고는 말할 수 있다．
 일반적인 상용통신에서는 주어진 주파수 자원에서 될 수 있는 대로 많은 가입자
를 서비스하게 하는 데에 주요 목적이 있을 것이다. 앞서서 여러 번 이야기되었듯이
Cl呱4A에서 가입자 용량은 각자의 전력의 적정한 배분이었다고 공부했고, 이것은 원
 .1 3. DSSS와 CodeOl론                                                                  기
                                                                                135
                                                                                  1
래 신호보다 월등히 큰 잡음신호 가운떼에서 통신을 하는 시스템을 생각하계 했다．
  이러한 생각을 다른 관점에서 볼 때, 이를테면 전장（戰場）에서 적군들이 우리의
통신시설을 마비시키기 위해서 우리의 수신기의 대역내로 아주 강한 전력의 잡음신
호를 지속적으로 송출한다고 할 때, CI呱4A와 같은 방식으로 광대역으로 통신을 한
다면 이러한 잡음으로부터 나의 신호를 온전히 복조할 수 있다는 생각을 할 수 있을
것이다． 이때는 여러 사용자가 통신함으로 인한 다중화 잡음이 아니라 Jamming 잡
음어］ 대한 복조능력을 이야기하는 것이다．
 CDM/CDMA통신 시스템은 이러한 외부의 Jamn血培신호（또 다른 의미로 간섭
신호）어］ 의해서 시스템의 가입자 용량이 결정되어지므로 가입자 용량과 Anti-
Jammn坦과의 trade-o卄는 충분히 생각할 수 있다. 이것은 우리가 공부하고 있는
CDMA시스템은／뇨lti-Jamming성능이 우수하다고 이야기할 수 있다．


 Jamming Margin Equation
 CDMA시스템에서 재밍 방정식（Jamnming M可帥i Equation）을 구하기 위해서
다음과 같이 몇 가지를 설정하자．
 즉 정보신호의 수신전력을 S, 원치 않는 Jamniii坦신호의 전력을 J, 전송 데이터
율을 r, 확산 대역폭을 \V, 수신 Bit당 月b, 잡음의 전력밀도를 1％라고 할 때
Jamming방정식은 다음과 같이 표현될 수 있다．
 즉 재밍 신호 J는 전송대역 전체에 컬쳐 있는 잡음의 에너지 밀도함수의 곱으로 나타
날 수 있으며, 신호의 에너지는 Bit당 에너지에서 Bit의 주기로 나누면 될 것이다. 이렇
거］ 해서 구하게 된 신호 대 잡음의 비는 결과적으로 다음과 같이 나타난다．


                二牡긴드吸珂缸包dB)
                       今4,           ，그으4;' 1,,/.(....，·"
                             'b' '"·．i．                     ivo
                                                   \\H니
                                                                허용할 수 있는
                Processing                                  i   정보 비트낭      신
                Gain                                        !   호대 잡옴 1J1




 즉 시스템의 신호어］ 대한 잡음의 분석은 Processing Gain에서 우리가 허용할 수
있는 에러 확률을 유지하게 해주는 Bit당 신호대 잡음비를 뺀 값으로 나타나며, 이
것은 이 시스템이, 즉 CDMA시스템이 추가로 허용될 수 있는 잡음 혹은 Jamming
에 대한 저항력이라고 할 수 있다．
                                         3. DSSS와 Code이론
                                                           .


 여기서 주의할 것은 PG가 클수록 Jamming어］ 대한 여유（M可gin)는 점점 커진다
는 것이며, 이러한 PG는 정보에 대해서 전송대역이 얼마나 넓은 대역인가를 나타내
는 척도인데 전송대역이 정보대역보다 클수록 Jamming어］ 대해서 여유가 커진다는
이야기다. 사실 이러한 CI呱4A시스템은 초기에는 군사용으로 사용되면서 고도의
비밀이 유지되는 통신에 사용되었다. 이러한 CDMA가 군사용으로 빛을 볼 수 있었
던 원인 중어］ 또 다른 하나가 ／뇨iti-J可nniir瑠성능이었다．
 지금까지의 사실을 볼 때 우리는 앞서서 이와 비슷한 내용을 가지고 이야기를 한
적이 있다. 즉 PG가 커질수록 Jamming신호어］ 대한 저항력도 커지지만 또 다른 측
면에서 다중통신 시스템이라고 할 때는 가입자의 용량이 많아진다고 이야기했었다．
이 두 가지의 가정들은 등가적인 이야기이다. 즉 이 절에서 이야기하는 佃DI恤堰은
또 다른 의미에서는 여러 명의 가입자로 인하여 발생되는 잡음신호와도 같다고 볼
수 있는 것이기어］ 그러하다．
二1. p 壯昏： 정보 Bit의 대역폭이 100bps이고 송신기에서 출력되는 전송신호의
         대역폭이 10MHz이리고 한다면, 그리고 이때 요구되는 S/N비가 100
         이라면, 이때 CDMA Pr兀essing Gain어］ 의한 이 시스템의 ／뇨1ti-
         Jamming 入4argin은 각각 얼마인가9
 =, n二二 Processing Gain은 정보 Bit의 대역폭과 전송 대역간의 비이므로
         107/102 = 50dB이다. 또한 S/N비가 10dB이므로 이러한 잡음으로부
         터 자유로울 수 있는 M可gin은 50 - 10 = 40dB이다. 즉 이것은 정
         보신호보다 40dB즉 10(刃배 정도 큰 전력을 출력하는 잡음 환경 하어］
         서도 기저대역에서는 주어진 신호대 잡음비인 10dB를 만족하면서
         통화를 할 수 있다는 것이다. 구체적인 값으로 다시 이야기하면 신호
         의 전력이 0.1mW인 가운데어］ 잡음의 세기가 1W로 강하게 작용해
         도 기저대역에서는 충분히 신호를 복조할 수 있다는 것을 의미한다．
         놀랍지 않은가7
 （그림 3-13）은 Jamn五ng하에서 확산 스펙트럼의 Processing Gain을 통한
Anti-J可nniii垠의 성능을 도식적으로 표시한 것이다. 이것은 마치 신호원의 영역어］
악성 잡음신호가 침투해올 때 이것의 침투로부터 방어하는 형국을 연상시킨다. （그
림 3-13）의 왼쪽의 신호원은 오른쪽의 동일한 대역에서 동일한 전력을 송신하는
    3. DSSS와 Code이론                                                      137
1


Jamming신호원의 영향으로부터 자신의 세력권을 나타내는 마치 등전선（等電腺）
의 모양을 그린 것이다. 이때 실지로 전력의 분포가 어떠한 형상으로 변화되는지를
확인해 보자．

                                                                Jammer


         송신 기




      통신




        S/J = -20dB      S/J = 10dB



                                S/J = 3dB          S/J = -3dB

                                       S/J = 0dB

                      （그림 3-13) Jammi四과 마oces帥（그（把In과의 전투



    좌표의 표시를 ( 兀, y）로 할 때 신호원의 좌표는 (0,0）이며, Jamming신호원의 좌표

는 (200,0）이다. 정보 신호원이든 Jamming신호원어］ 의한 전력의 분포는 거리, 즉 I？左
에 반비례하며 ，자유공간이라고 가정할 때 ，전력의 변화는 단순히 가우스 정리어］ 의한
발산어］ 의해서 2로 정리된다. 또한 정보신호나 拓mming신호의 크기를 같다고 가정하
였을 때 우리는 수신된 신호와 Jamming신호의 비를 다음과 같이 표현할 수 있다．



         [}]，七匕 긺* 2
                  y2＝
                   『                                                     (3-16)



    여기에서 p는 정보신호어］ 대비해 재밍신호의 크기를 나타내는 값이며, 이 값어］
의해서 새롭게 형성되는 신호의 분포곡선을 그리기 위해서 위의 식 仔11）을 다음
과 같이 고쳐 쓸 수 있다．
   138                                                                       3. DSSS와 Code이론
                                                                                               .




         (x+   200      )   2+    y2 =   (   200而 2     )
                                                                                        (3-17)
               1- p                           1-p

     반경：= 200而 ,                             원의중심（ 200p , 0)
          卜p                                      卜p

 즉 반경과 중심은 p의 함수로 나타난다. 여기에서 p가 10dB, 즉 정보 신호원보
다 10배 크다고 한다면 그것어］ 의한 전력선의 분포는 중심이 (222,0）이고, 반경이
70인 원의 모양으로 나타날 것이다．
 이 절의 앞 부분에서 확산 스펙트럼의 ／뇨it卜Jamming이라는 특성이 상용통신망
에 적용될 때는 그것은 통화용량으로 설명퇸다는 이야기를 하였다. 즉 Jamming의
성질은 또 다른 사용자의 출력을 의미할 수 있기 때문이다. 즉 군사용과 같이 사용
하는 확산통신은 그것 자체가 보안이나 ECCM 등과 같은 재밍으로부터 보호받는
것을 성능으로 생각할 수 있고 상용에서는 더 많은 사용자의 확보로, 즉 용량으로
시스템의 성능을 평가할 수 있다．


               군사용

               .T / R 쯔
                                 W/ R
               니 ' -,            Eb/ N
               w : 확산대역                                     ,J : 수신된 Jamming（잡음） 전력
               1之 : 정보대역                                    S : 수신된 신호 전력

               Eb/ No : 수신기의 성능｛신호대 잡음비）


               상업용
                                              1 !   1



               ,.                W 'R    !'n . n..:..
               ",．‘斗 丘
                     ；/됴 !．늑．
                            누二
               M : 셀 당 동시에 통화 가능한 수                         Gv : 음성 활성화로 인한 이득
               GA : 섹터화 이득                                  Ho : 인접 셀의 간섭에 의한 손실




 상업용으로 사용하는 확산 스펙트럼 방식은 흔히 CDMA라고 불리우는 셀룰러
및 Pcs폰의 경우이며, 이것의 용량 역시 또 다른 의미의 간섭신호어］ 대한 투쟁이라
    3. DSSS와 Code이론
口


할 수 있다. 이러한 상용통신이 셀룰러인 점 등어］ 의해서 발생되는 인접 셀간의 간
섭은 시스템의 용량의 감소요인이 되며, 이러한 간섭을 줄일 수 있는 여러 가지 방
법, 즉 섹터화로 인한 간섭의 제한과 보코더의 음성 활성화도어］ 따른 전송정보의 조
절 등과 같은 방법 등도 결국은 간섭신호의 억제를 위한 방법이며, 이것을 통한 용
량 증대를 꾀하려는 노력이다．
 상업용의 용량에 대해서는 다음 절에서 상세히 새롭게 공부할 것이다．



    3.3 대역확장                                            }
 이 장에서 공부하는 대역확산과는 좀 거리가 있는 이야기가 될 수 있으나, 어떤
의미에서는 연관이 있으므로 이 절을 이 장어］ 포함했다. 이 절에서 이야기하게 될
대역확장은 무선통신에서 사용자에게 할당되는 채널의 대역폭을 확장하는 것을 의
미하며, 이것은 사용자 1인 당 할당할 수 있는 대역폭이 기본음성 호뿐 아니라 데이
터 호 등의 사용시어］ 확장될 필요가 있으므로 사용된다. 추가적으로 필자는 이러한
방법을 대역확산과는 구별하기 위해서 "확장" 이라는 단어로 그것의 의미를 구분하
고자 한다. 사실 이 내용을 이 장어］ 포함시키는 것도 고민스러운 일이나 대역폭의
변화라는 측면에서 혹은 대역확산의 개념을 좀더 확고하게 이해하기 위하써 대비
(?）될 수 있는 내용으로 이 내용을 이 장에 추가하기로 했다. 어찌 되었든          .
 대역확장이라는 것은 사회가 더욱 정보화로 가면서 개인이 처리하게 될 정보의
양이 많아지고 그것을 현실적으로 전송, 수신하기 위해서 필요하게 되었다. 이러한
것은 QCDMA의 IS-95B에서부터 사용되어 오고 있는 MDR小/ledium Data Rate)
데이터 서비스에서부터 소개되고 있다. 이것은 기본적으로 할당되어 있는 음성신호
의 대역폭의 정수배로 동일한 사용자에게 여러 개의 기본 대역신호를할당하는 방
식이다. CDMA에서 채널이라 함은 Code Channel을 말하는 것이며, 이 Code
Channel을 하나의 사용자에게 여러 개 할당함으로 그 사용자는 자연히 기존의 대
역보다 n배 넓은 대역을 사용할 수 있게 된다．
 즉 전송할 수 있는 정보의 양이 많아질 수 있는 것이다． 이러한 이유로 이렇게 할
당되는 채널은 Supplemental Code Chan佃(SCCH）이라고 한다．
 이것을 그림으로 표시하면 （그림 斗14）와 갇다. 실지로 IS-95B에서는 이러한 대
역 확장용으로 사용되는 Code Channel의 수를 8개까지 확장되게 이야기하고 있다.
   140                                            3. DSSS와 Code이론
                                                                    U



             C:;




         (a) 기본코드채널   (b) 대역 확장된 부가코드채널   (C) 대역확장 된 부가채널

   （그림 3-14) Fundament계 Channelif 呼95B의 Sup이en冷nt키 Code Channel


즉 9.6K bps의 Fundamental Channel의 경우 76.8Kbps까지 대역확장이 가능하고
14.4K bps인 경우 115.2Kbps까지 대역확장이 가능하다. 그러나 현재 우리나라에서
서비스되고 있는 八'IDR의 경우 5개의 Supplemental Code Channel을 사용 가능한
형태이며, 그것도 Reverse으로는 제공이 되지 않는 형태이다．
 이것을 위해서는 여러 개의 논리채널（Code Channel)을 하나의 개인코드어］ 대응
시켜 주면 되고 이것은 IS나弱A의 상황과는 많이 다른 것이다. 즉 예전에는 하나의
개인（ode Channel(Long C（넜C）이 하나의 Code Channel이라는 개념이 성립되었으
나 이제는 하나의 개인채널이 여러 개의 Code Channel을 관리할 수 있다는 것이
된 것이다．
 이것과는 좀 다르게 대역확장 방법이 또 하나 있는데 이것은 확산단계에서 확산을
위한 확산율을 조정하는 것이다. 즉 기존의 확산은 하나의 정보 데이터가 64＼人ralsh
칩의 한 주기어］ 대응이 되는 형태이었다. 그러나 그것을 3才刀alsh의 한 주기어］ 대응
을 시킨다면 전송할 수 있는 정보량은 2배로 증가하게 될 것이다. 이러한 방법을 사
용한다면 \Valsh의 주기를 조정함으로 대역을 확장할 수 있다는 것이 된다. 따라서
기본대역의 16배가 되게 하기 위해서는 \Valsh의 주기가 16배 빠른, 즉 1/16주기의
Walsh를 사용하면 된다. 즉 그것의 주기가 4인 \Valsh를 사용하면 될 것이다．




 3.4 용량

   3.4.1 얼랑 용량

 가입자당 발생 통화량佃ifered load）은 확률과 통계어］ 기반을 둔 대기이론
(queing theory）을 통하여 설명할 수 있는 일종의 랜덤 신호이다. 호의 도달률
    3. DSSS와 Code이론                                     141
.


(arrival rate）을 A（호／초）라고 하고（호의 도달률은 일반적으로 助isson 분포를 한
다고 알려져 있다）, 호의 서비스율（service rate）을 尸（호／초）라고 하면（호의 서비스
율은 일반적으로 exponential 분포를 한다고 알려져 있다） 가입자당 발생 통화량 a
는 A人K얼랑／가입자）로 주어진다. 이때 각 호가 도달하는뎨 걸리는 시간과 서비스
（처리）되는데 걸리는 사간은 각각 1/A와 1／肛（초／호）로 주어짐을 알 수 있다．
    예를 들어서, 호의 도달률이 A = 0.8（호／시간）이고, 각 호가 서비스되는데 걸리는
시간이 l/ p= 1.76（분／호）라고 하면, 가입자당 발생 통화량은 다음과 같이 계산할
수 있다．
         口   ＝   凡＝    0.8  (1.76x60)
                             x
                 /1   60x60         '
             = 0.0235（얼랑／가입자）
             = 23.5（밀리 얼랑／가입자）

    이렇게 가입자당 발생 통화량이 주어지면, 다음과 같은 통화량 예측모델（BBC
model : Blocked Calls Cleared model) 또는 식 (3-18）과 얼랑 B공식에 의해 가입
자 용량과 호시도 차단을 그리고 채널수 등의 관계를 구할 수 있다. 여기서 호시도
차단율（Blocking Probability) PB란 통화（호）의 시도가 차단되는 비율을 말하며, N
은 특정한 통신 시스템에서 이용 가능한 채널의 수를 말하고, A는 특정한 통신 시
스템에서 이용 가능한 총 통화량, 즉 가입자 용량을 말한다．

                            IAN
          F= B(A,N) = N!.                                (3-18)
                            <：끼 I    .
                             > 』1   /4
                            ；二 k!
    이 얼랑 B 공식은 계산이 매우 복잡하므로 부록에 있는 얼랑 B표（Erlang B
Table）를 이용하여 구하게 된다. 예를 들어 가입자당 발생 통화량이 0.029（얼랑／사
용자）라고 가정하고, 채널당 53 사용자수를 수용할 수 있으며 총 6채널로 구성된 시
스템 1（八1J 시스템）과 채널 당 37 사용자를 수용할 수 있으며 총 6채널로 구성된 시
스템 2（八/11( 시스템）에 대하여 가입자 용량과 호시도 차단율을 각각 구해보자. 먼저
각 시스템의 가입자 용량 ／뇨과 /\2는 다음의 계산으로 구할 수 있다．
    A1=0.029 x 53 x 6= 9.33 (얼랑）
    A2= 0.029x37x6= 6.51(얼랑)
   142                                                     3. DSSS와 Code이론
                                                                                        U


 이제 각 시스템에서 채널수와 가입자 용량이 주어졌으므로 얼랑 B표어］ 의하1 각
시스템의 호시도 차단율을 구하면 다음과 같다．
 PBI = B(9.33,6)竺50[%]
 ／눙戶及6.51,6）르301%1
 위의 예에서는 시스템 1의 호시도 차단율이 50[%］이므로 평균 2번의 통화시도
중 1번 꼴로 통화가 차단되게 되며, 시스템 2의 호시도 차단율은 30B旬이다. 실제의
이동통신 시스템에서 이렇게 호시도 차단율이 높으면 곤란하며, 2[%] 이내의 호시
도 차단율을 유지하도록 규정하고 있다.


                   K표 3-1) Erlang B Blocking Probability

  회선      0.001    0.05       0.   1     0.2       0.3        0.4           0.5
  1       0.001    0.053     0.111      0.250     0.428      0.664       1.000
  2       0.046    0.381     0.四5       1.000     1.449      2.000       2.132
  3       0.194    0.899     1.271      1.93      2.633      3.180       4.591
  4       0.4羽     1.525     2.045      2.945     3.890      5.021        6.髥）].
  5       0.762    2.218     2.881      4.010     5.189      6.596     ,''8.437, .}
                                                                        1
                                                                            1 1 1 1 1 1! 1


  6       1.146    2.960     3.758      5.109     6.514      8.191      .10.394
  7       1.579    3.738     4.（文文；     6.230     7.856      9.800. *."' 12.354
  8       2.051    4.543     5.5｛刃      7.369     9.213      1j.45i     14.321
  9       0.557    5.370     6.546      8.522    l0·娶｝．··' "13.053      16.293
  10      3.092    6.216                      ·'
                               7，自Ui ， 으晏｝5· "11954          14.681     18.271
  11      3.651    7.076   :"'8.487了t '10.860    13.333      16.312     20.253
  12      4.231    7.950      '可．474'  12.040    14.721      17.953     22.244




           산전 연구소에서 근무하는 홍길동 씨는 업무상 통신사업부에서 실무
           자들과 대면하면서 처리하햐 할 일이 많아서 통신사업부어］ 자주 간
           다． 마침 산전연구소에서 이러한 사람들을 위하여 자전거를 5대 구입
           해 주었다. 그런데 홍길동 씨가 이 자전거를 이용할 때면 두 번어］ 한
           번은 다른 사람들이 먼저 이용해서 사용할 수가 없었다. 그렇다면, 산
           전연구소에서는 몇 대의 자전거를 더 구입하면 홍길동 씨가 열 번어］
           아홉 번은 이용할 수 있을까9
    3. DSSS와 Code이론
.


             자전거를 사용할 blocking 확률을 0.5에서 0.1로 줄이는 것이 목적이
             다．
             자전거는（N) 5대이다. 즉 N=5일 때 PB가 0.5이면 이때 얼랑 B표에
             서 확인하면 8.44이다. PB가 0.1일 때 이 값과 가장 가까운 값일 때
             는 N=11이다． 즉 6대의 자전거를 추가로 구매하면 자전거를 사용할
             확률을 的96로 할 수 있다．


     3.4.2 CDMA 가입자 용량

    확산대역 기술은 정밀거리 측정 및 추적뿐 아니라 앞서 이야기한대로 /nti-Jam
및 다중경로성분의 제거어］ 오랫동안 응용되어 왔으며, 최근에는 CDMA시스템으로
응용되어 사용하고 있다. 초기에는 셀룰러 시스템의 다중접속 방식으로 사용되던
FDMA나 TDMA어］ 비해서 용량면에서 떨어진다고 생각했으나 그 이후 CDMA의
용량은 간섭어］ 의해서 개선이 가능하며, 간섭이 효과적으로 개선될 때 그것의 용량
이 선형적으로 증가함을 확인하면서 CDMA 가 빛을 보기 시작했다．
    따라서 CI呱TA시스템은 간섭을 효과적으로 제어할 수 있는 시스템으로 개발되었
으며, 예전에는 크거］ 고려치 않았던 사항들이 용량과 직결된다는 이유로 새로운 연
구와 관심을 가지게 되었다．
    결국 CDMA 셀룰러 시스템의 용량을 결정하는 주요 파라메타로는 처리이득
(Processing Gain）에 의한 용량어］, 간섭요인과 관련퇸 추가요인들인 적정한 통화품
질을 위해서 요구되는 瓦IN0, 음성의 부하율（voice duty cycle), 주파수 재사용
효율 그리고 기지국 안테나의 섹터수 등이 있다．
    이 절에서는 현재 한국에서 상용화되어 있는 Qualcomm의 CDMA시스템을 통해
서 이야기를 학 것이며, CDMA시스템이라는 것은 이 시스템을 이야기한다．


    尻／N0값의 제어를 통한 용량

    尻／사는 디지털 변조와 부호화 방식의 장단점을 비교할 때 쓰이는 표준지수이
다． 이것은 아날로그 FM 변조에서의 반송파 대 잡음비（CM깁와 비슷하다고 할
수 있다． 효율적인 변조기술， 강력한 오차교정 부호와 다이버시티의 다중 사용 때
문어］ 비록 동적 다중경로 환경하일지라도 CDMA가 광대역으로 정보가 전송된다
   144                                  3. DSSS와 Code이론
                                                          U


는 사실 때문어］ 평균 6dB의 Eb/N0 정도만 확보되면 좋은 성능이 보장퇸다. 이러
한 사실은 앞서 2장에서 공부한 샤논의 정리에서 그것의 이론적 원리를 찾아볼
수 있다．
 이것은 아날로그 FM사용시 동일 조컨에서 18dB의 반송파 대 간섭비가 요구되는
것과는 좋은 대조를 이룬다. 이것은 동일한 정보량이 광대역과 협대역으로 구분되
어서 전송될 때 얻어질 수 있는 처리이득이라고 볼 수 있다. 참고로 6db는 약 3.98
이며, 18db는 63.1정도이다．
 Bit 에너지 대 잡음 전력비는 시스템 동작의 신뢰성어］ 매우 중요하다. Bit 에너지
瓦는 신호 에너지를 전송속도로 나눈 것으로 정보 Bit의 평균 에너지이며, 잡음 전
력 1％은 N-1) 개의 또 다른 사용자의 신호 에너지를 전체 대역으로 나눈 것이다．
즉 이것을 표시하면,

         Eb H SIR  H WIR
                                                   (3-19)
         N0 (N크）S八V N- i

 여기에서 瓦／1％는 필요한 Bit 에러 성능을 유지할 수 있는 수준이어야 하며, S
는 각각의 사용자어］ 의한 신호의 세기를 말한다. CDMA에서는 이것이 작은 값이
선택될 수 있을 때 더 많은 채널용량을 확보할 수 있다. 따라서 瓦／1％을 낮게 유
지할 수 있는 시스템적인 성능개선이 필요하다. 이러한 것의 성능개선을 위해서 가
장 중요한 것은 Reverse 링크어］ 대한 위상동기 진폭감쇄（Fading) 특성, 전력제어
기술의 성능 등이다. CDMA 시스템에서는 이러한 것을 위해서 기술적인 역량을 모
으고 있으며, 위상동기와 Fading어］ 대한 대처방안 등에 대해서는 4장에서 공부한
다. 또한 전력제어어］ 대한 공부는 이어서 5장에서 하게 될 것이다.
 이상의 八'Ia拍r한 요인들 이외에도 채널환경에서 랜덤하게 발생하는 간섭신호이
며, 이것의 확률분포를 해석하고 보상해 주는 것이다. 이와 관련해서 일반적으로 상
당히 강력한 채널코딩을 사용한다．
 한편 열 잡음과 의사간섭어］ 의한 배경잡음을 갇이 잡음으로 생각하면 식 (3-19)
는 다음과 갇이 다시 쓸 수 있다.

         且＝ WI熙，.7         열 잡음에 의 한 잡음성분

                                                   (3- 20)
         N. 小1）뇨．.（照）'
    3. DSSS와 Code<기론                           145
U


 여기에서 가입자수, 즉 채널용량과 瓦／N의 관계가 어떠한지를 생각해보자. 따라
서 식 侶-15）을 가입자수 N을 표시하면 다음의 식 (3-21）과 갇이 표현할 수 있다．
                    77
         N= l+ W/R                             (3- 21)
               瓦／N。 S

 즉 가입자의 수는 Processing Gain을 尻／사로 나눈 값이며, 여기어］서 변복조
기와 복호기의 성능을 나타내는 瓦/ 1％이 작으면 작을수록 용랑은 증대하게 된다．

디지털 통신의 경우 이 값은 io-3 이하가 되는 값이다．
  식 仔21）에서 가입자 용량（N）은 확산대역어］ 걸쳐 있는 잡음신호 전체의 에너지
(WT나0)를 정보 신호의 총 에너지（REb)로 나눈 것, 즉 확산된 대역의 에너지를 각각
의 개인에게 나누어 주는 형태라는 것을 알 수 있다. 즉 사용자수는 총확산대역폭
내의 사용자당 신호대 잡음비로 반비례한다. 이동통신 시스템의 SNR은 송신기의
전력 레벨어］ 의해서만 제한된다. 다음의 근거 설명어］ 앞서 SNR을 요량면에서 한
사람의 사용자를 감소시키는 것과 동일한 수준으로 가정한다. 따라서 배경잡음어］
따라서 기지국어］ 필요한 수신신호 전력이 결정되고 이에 따라 가입자 송신전력 혹
은 최대 송신전력하의 셀 반경이 결정된다．
 CDMA 시스템의 Reverse Link는 Non-Coherent 시스템이며, 다중경로 페이딩
채널환경이다. 이러한 환경하에서는 2개의 안테나 다이버시티와 구속장이 9(9Clock
전의 상태까지 현재 상태어］ 반영）이며, 코드율이 1/3(1개 정보어］ 2개의 리턴던시를
붙여서 3개로 만듬）인 강력한 Cony이utional코드（이러한 부호화 기술은 7장에서 상
세히 공부하자）를 사용하면 瓦IN0값은 7dB이다．


    V아ce Acti\／卄y m 음성신호 감지

    부호화 혹은 변조기술을 통해서 필요한 瓦iN0를 얻는데는 앞서 공부한 샤논의
한계（Shannon Limit）어］ 의해서 제한되어 있다. 따라서 우리는 용량증대를 위한 새
로운 관점으로 식 侶-19）의 분모항을 줄임으로써 용량을 증대하는 방안을 생각해
보자. 즉 이 방법은 주어진 잡음환경에서 줄여줄 수 있는 잡음을 줄여 주자는 생각
인데 이것의 대표적인 방법으로는 \Toice Activity를 통한 전송속도의 가변적인 적
용이다．
    우리가 전화통화를 할 때 혹은 일반적인 대화를 할 때 전형적인 방법은 상대방의
   146                                     3. DSSS와 CodeOl론 U



말을 튿고 말을 한다. 즉 두 사람이 대화를 한다는 것은 한 사람이 말하고 또 다른
사람이 말을 하는 경우 그리고 그것의 반대의 경우, 두 사람 모두 말이 없는 경우
마지막으로 이런 경우는 싸움을 하거나 특별한 상황어］ 이루어지는 두 사람이 동시
어］ 말을 하는 경우이다．
 이렇게 볼 때 한 사람의 입장에서 본다면 대화하는 시간어］ 발생될 수 있는 4가지
의 경우 중 2가지는 자신이 이야기하는 시간이 될 것이다. 그러나 두 사람 모두 말
하는 경우는 그리 많지 않다. 그렇다면 3가지의 경우가 있는데, 이 중에서 말하게
되는 시간은 약 1/3에 해당된다 ．실지로 전형적인 양방향 음성대화시 각 음성의 부
하율은 단지 35%-40%어］ 불과하다고 하는 통계적인 데이터가 있다.
 섹터당 통화자수가 제한되어 있는 경우 동시통화자수가 평균 통화자수 이상 일
수 있는 가능성을 무시할 수 없기 때문어］ 실지로 음성 부하율어］ 의한 용량증대는
약 2 이라고 할 수 있다．
 CDMA 시스템에서는 음성이 없을 때 데이터 속도를 감소시키고, 송신전력을 줄
임으로써 결과적으로 다른 사용자어］ 대한 간섭을 줄여준다. 다른 사용자어］ 의한 간
섭 정도가 용량을 결정하기 때문에 통화하는 시간의 반은 내가 사용하고 나머지 반
을 다른 대화자가 사용한다면 그것으로 인해서 간섭을 줄일 수 있으며, 직관적으로
약 2배의 용량증대를 이룰 수 있다.

         万； 1   WIR
                                                       (3- 22)
         N。 (N-1)a+ (77/ S)

 식 仔22）는 가변적인 Bit율을 가지는 CELP(Code Exited Linear I노edictive)
（力dec고｝ 같은 V（兀oder를 사용할 때, 尻／N0의 감소로 용량의 증가를 가져올 수
있다．


 섹터화를 통한 용량 획대
 간섭을 줄여서 용량증대어］ 기여할 수 있는 또 다른 방법으로는 기지국에 지향성
안테나를 사용해서 섹터로 나누는 섹터화어］ 의해서 이루어질 수 있다．
 지향성 기지국 안테나를 사용할 때 섹터의 수가 S이면, 실제의 값은 S로 나눈
     （이때는 1/S영역 내에 있는 단말기만 탐당하므로） 그러므로 전체 시스
값이 퇸다．
템에서 지원할 수 있는 용량은 거의 S배（다른 섹터로부터의 누설에 의한 추가 간
    3. DSSS와 Code이론
U


섭으로 인해 보통 섹터 효율이 득을 최대로 얻을 수 있는 이득의 85% 정도로 감
   ）만큼 증가한다. 예를 들어서 3개의 섹터로 나눌 때 전방향 안테나일 때보
소한다．
다 간섭은 1/3이 된다. 즉 N= 3Ns이다． 따라서 3-19식은 다음과 같이 다시 쓸 수
있다．

         Eb e    W仄
                                               (3- 23)
         N。 (N3-1)a+(7/S)

 식 仔23）에서 Ns = N/3과가 3/8에 의해서 약 8배의 이득을 얻을 수 있으며, 이
것으로 인해서 尻／N0가 7dB일지라도 가입자수 N은 Processing Gain(W在n에 근
접하게 됨을 알 수 있으므로 적어도 독립된 셀에서 CI呱4A와 같이 광대역으로 신호
를 전송한다 할지라도 그 대역을 쪼개어 통신하는 기존의 방식어］ 용량이 뒤지지 않
는다는 것을 확인할 수 있다．
 다중셀의 경우 주파수 재사용상의 또 다른 사항이 있으나 모든 셀에서 동일한
주파수 대역을 사용하는 CI呱IA의 경우 이러한 것은 상대적으로 장점이 될 수 있는
것이다. 이러한 장점들을 계산하기 위해서는 먼저 전력제어 기술 및 전력제어가 다
중 셀에서의 간섭에 미치는 영향을 고려해야 한다.


         재사용
 지금까지는 독립 셀의 경우 용량어］ 영향을 미치는 것들어］ 대해서 생각하1 보았다．
그러나 상용의 통신망을 생각할 때 우리는 셀 단위로 통신을 하게 되는 셀룰러의
특징이 채널용량과 연관지어질 수 있다는 것을 간과해서는 안 퇸다. 셀룰러는 앞서
1장에서 공부하였듯이 채널자원을 재사용하기 위해서 기하학적으로 제한된 영역을
설정하여 그 영역 내에서는 독립적 혹은 고립적으로 망 자원을 사용하는 형태이다．
따라서 셀 간의 경계는 이러한 관점에서 상당히 중요하게 보장되어야 할 것이다．
 이러한 셀룰러의 다중 셀 시스템에서는 일반적으로 특정한 넓이의 대역폭을 각각
의 셀어］ 할당하고 어느 정도 이하의 간섭성분만 허용되는 거리가 떨어진 지점에서
다시 그 주파수 자원을 사용한다. 그러나 CDMA의 경우 모든 셀에서 동일한 주파
수 대역폭을 같이 사용하게 되므로 주파수 대역간의 간섭이 전혀 없다고 할 수 있
다. 이러한 이유에서 CDMA의 주파수 재사용 계수는 1이다. 즉 1개 셀 단위로 주파
수 재사용이 가능하다는 이야기이다.
   148                                     3. DSSS와 Code이론
                                                             U


 Fl呱4A나 TI孤4A는 인접 셀에서 갇은 주파수를 사용하면, 서로 간섭이 일어나
통신을 할 수 없다. 이러한 상황에서 셀룰러의 특징 중의 하나인 주파수 재사용률이
다． 어느 한 단말기에서부터 기지국으로 들어오는 신호어］ 대한 전체 간섭은 같은 셀
내에 있는 다른 단말기로부터의 간섭 그리고 인접 셀 내의 다른 단말기로부터의 간
섭 및 기본적인 열 잡음으로 구성된다． 전력전파가 거리의 4승에 반비례하는 통화
권 내의 균등 분포된 가입자로 인해서 시스템에 완전 부하가 컬렸을 때, 이 기지국
에 대한 모튼 인접 기지국의 간섭량은 같은 셀 내의 다른 단말기어］ 의해서 생기는
간섭의 &3% 정도가 된다. 이러한 경우 CDMI\ 셀룰러 시스템에서의 각 기지국 용
량은 인접 기지국이 없는 단일 기지국 용량의 60% 정도가 된다．
 이제 이상의 결과어］ 의해서 정량적인 해석을 해보자. 생각을 쉽게 하기 위해서 공
간분리 효과만을, 즉 무 지향성 안테나의 경우만어］ 대해서 설명하겠다．


 (1) 경로 손실은 4승에 비례한다．
 (2) 셀 내에는 N개의 단말기가 있고 따라서 l寸-1깨1의 간섭원인 단말기가 있다．
三(3) 모든 위치에서 기지국으로부터 동일한 전력을 수신하는 전력제어가 되고 있다．




 이상의 3가지를 가정하고 기지국에서 수신된 총 신호 대 간섭비를 표현하면 다음
과 갇다．
         C              1
         I   N+ 6Nk] +12Nk, +18Nk3+...

 이것을 인수분해하면，

         C               1
                                                      (3- 24)
         I   N(1+ 6k1 + 12k2 +18k3 +...)

 여기에서 N 은 셀당 단말기의 수이며, k1, k2, 岫은 중앙기지국을 중심으로 한 동
심원의 1, 2, 3, · ' · 겹어］ 위치한 각 기지국이 중앙 기지국어］ 미치는 간섭을 중앙 기
지국 자체의 간섭과 비교한 비교치이다. 이러한 k값은 중앙에 위치한 기지국의 경
로손실과 간섭 단말기의 간섭 단말기의 자기 기지국어］ 대한 전력제어어］ 따른 전력
감소와 함수콴계가 있다．
 주파수 재사용 효율 F는 식 侶그3）과 같이 정의하며, 이 것의 값은 일반적인 해석
1
U 3. DSSS와 CodeOl론                             149




                     （그림 3-15) 인접기지국으로부터의 간섭


적인 방법으로는 풀 수 없고 수치 적분 방식이든지 컴퓨터 시뮬레이션 방식으로 F
값을 구할 수 있다．
 CDMA에서는 이러한 주파수 효율이 모든 같은 주파수를 사용하써 1이라고 생각
할 수 있으나 동일 채널 간섭의 허용치어］ 의해서 약 0.65라고들 이야기한다. 이것은
현재 기지국의 다른 단말기로부터 받는 간섭과 기타 주변 기지국으로부터 받는 간
섭이 거의 비슷하다는 이야기가 된다． 즉 1.5개（=1/0.65）의 셀 건너 주파수를 재 사
용할 수 있다는 것이다．이것은 기존의 AMPS어］ 비하면 상당히 혁신적인 수치이며,
CDMA가 셀룰러에서 상당히 적합한 시스템이라는 반증이 되기도 한다．
 （그림 3-15）는 인접한 기지국들로부터 받는 간섭을 %로 표시한 것이다．
 첫 번째 주변 원에서는 각 셀들로부터 약 6%씩의 간섭을 받으므로 36%의 간섭
을 받으며，두 번째 및 그 이상의 외곽 원들로부터 받는 모든 간섭은 4% 미만이 된
다． 지향성 기지국 안테나， 즉 120도 섹터 안테나를 사용할 경우 각 안테나는 기지
국내어］ 있는 단말기의 1/3정도만 관장하게 되므로 간섭량도 평균1/3로 감소하게 된
다． 따라서 전체 시스템이 지원 가능한 용량도 3배 가까이 증가하게 퇸다. 이것은
앞서 이야기되었던 부분이다．


 불균등한 기지국간 통화량 분포
 기지국 내의 단말기들의 분포는 앞서 이야기한 간섭효과어］ 어떠한 영향을 미치겠
는가？ 앞서서 공부한 CDMA 시스템의 주파수 재사용 방안은 단말기가 통화퀀역
I    11n                                 3. DSSS와 Code이론
                                                           1


내에, 즉 셀 내어］ 균등하게 분포되어 있다는 가정 하에서 이루어진 것이다. 그러나
이러한 가정을 무색하게 할만한 비정상적인 단말기의 분포가 종종 있다. 예를 들어
서 월드컵 경기장과 같이 많은 사람이 밀집되어 있는 곳을 들 수 있다. 간섭제한 시
스템인 CDMA의 경우 가용 채널수는 인접 기지국의 통화량 분포와 어느 정도 상관
성이 있으며， 인접 기지국의 통화량이 많지 않을 경우 통화량이 많은 기지국어］ 채널
이 더 할당될 수도 있다．
    CDMA시스템에서 단말기의 실제 분포어］ 따라서 용량이 10N 50% 증가될 수 있
다． 일부 기지국들이 심하게 통화집중이 되어 있다면 나머지 기지국들에는 통화량
부하가 분명히 적다. 통화량이 많지 않은 기지국들이 통화량이 높은 기지국들어］ 주
는 간섭이 크지 않으므로 통화량이 많은 기지국들에게 채널을 많이 할당할 수 있다.
예를 들어서 고속도로상에 위치한 기지국들을 살펴보면 이들어］ 대한 주변 기지국들
의 통화량은 고속도로 통화수요의 절반 정도밖어］ 안 된다．




                 （그림 3-16) 불균등한 기지국 부하


（그림 3-16）의 예와 갇이 정상용량의 30%어］ 해당하는 적은 통화량이 부과된 기
지국들이 통화량이 높은 기지국들을 둘러싸고 있는 경우가 있다. 이 경우의 정상용
량이란 주위의 모든 기지국들도 동일한 용량으로 부과되었을 경우의 통화량으로 가
정한 것이다. 이 경우 통화량부하가 높은 기지국이 주위 기지국으로부터 받는 간섭
은 감소된다. 이러한 간섭의 감소는 고부하 기지국의 용량증대를 가져온다. 주위 기
지국들이 정상용량의 30%어］ 해당하는 통화량부하를 받을 경우 과부하 기지국의 용
량은 정상용량의 120%로 늘어난다．
 이와 같은 유동적 용량변화는 기지국과 단말기어］ 같이 적용된다. 물론 이러한 과
    3. DSSS와 Code이론                                            151
                                                                 H기
.                                                          1

부하가 예상되는 기지국에는 충분히 확장 가능한 CI呱4A 모뎀이 있어야 하며, 가변
용량이 적용될 수 있도록 운영 프로그램이 되어 있어야 할 것이다．


       A용랑산출 정리
           ［llCDMA의 용량산출은 이상의 내용들을 종합할 때 다음과 같이 정리
    Qualcoi列
될 수 있다．

              쁘R
                   ！且川
                         l d
          N              1
                               F   G   =

                                                               (3- 25)



              여 기에 서
              N : 기지국 당 통화 채널 수
              w : 확산 스펙트럼 대역폭 （예 : 1.25MHz)
              R : 데이터 전송속도， Kbps （예 : 9600bp引
              Eb/ N0 : 비트당 에너지대 잡음전력 스펙트럼 밀도［예 : 7dB)
              D : 음성부하 점유시간 비율 （예 : 40% )
              F : 주파수 재 사용효율 （예 : 60% )
              G : 섹터 분할 이득 （예 : 3섹터 2.55}   夕在無特回缸而쿄添出磁蕪




    이상의 그림에서 나타난 수치들은 CDMA시스템에서 설정할 수 있는 그리고 사
용하고 있는 실제 값들이다. 이때 기지국당 무선용량은 약 98개 채널이 퇸다. 아울
러 2%의 통화 차단율이 있을 때 이 시스템의 얼랑 용량은 72얼랑이 된다. 얼랑 산
출시 소프트 용량 제한은 사용되지 않았다. 예를 들어서 최대 용량인 N개의 통화를
진행중인 기지국어］ 또 하나의 통화가 시도되었을 때 이어］ 대한 서비스는 거부되며，
재시도가 없다고 가정하였다. 소프트용량 제한기능이 사용되면 전체 사용자의 Bit
오차율이 약간 증가되면서 위의 추가 통화가 가능하다. 동일한 서비스 등급으로 비
교할 경우, 3섹터 AMPS기지국은 36얼랑을 제공하는데 할당된 대역폭 전체가 사용
된다. 같은 대역폭이 CI呱4A시스템어］ 사용된다면 그것보다 약 201얼랑 높은 720얼
랑이 될 수 있다고 한다．
    결론적으로 셀룰러 시스템에 할당된 전주파수 대역폭을 CDMA어］ 사용하면, 기
본적으로 Processing gain으로 표현되는 단순한 주파수 채널배정의 효과에 이상어］
서 열거한 CDMA만의 속성어］ 의해서 용량 증대를 꾀할 수 있다. 이것은 대략 10배
   152                                 3. DSSS와 Cod今기론
                                                         U


로 증가한다는 것이 명백하며, 낮은 Bit 속도의 음성 부호화기를 개발하거나 1a 많
은 섹터를 나눔으로써 사용자수를 증가시킬 수 있다. 주의할 것은 가변 코드율의
voCoder사용이나 cell의 sect아화 및 높은 정정율의 coding 등은 CDMA만이 갖는
용량 증대 성질이다．
 CDMA 셀룰러 System의 대표적인 예라 할 수 있는 Qualc아nm CDMA
System의 경우 결국 용량증대를 위해서는 작은 瓦／m로도 충분히 통신이 되게 하
는데에 주관점을 두었다고 생각할 수 있다. Soi표ce C어五ng에서는 가변 Bit율인
CELP를 이용한 QCELP를 사용하여 전체적으로 Bit Energy를 작게 하였으며，
Channel Coding에서도 에러 정정율에 상당히 치중하여 Code Rate이 낮은（노小ng
을 하여 Bandwidth와 Trade）卄했으며, 이러한 결과는 Modulation단계에서도 적용
되어 Spectral Efficiency보다는 EBR의 개선어］ 더욱 관심을 가졌다고 생각할 수
있다. TDMA나 FDMA의 경우 그것들의 용량 증대가 더 많은 주파수 밴드를 가지
느냐 혹은 더 작게 Time Sl야을 쪼개느냐인데, CDMA는 이러한 두 가지 시스템어］
비해서 주파수에서만은 상당히 여유가 있어서 Bandwidth와 Error 정정율을
Trade-Off하여 설계하였다．



     Code
            theor y                                      )
 CDWCI呱4A는 주파수를 공유하면서 또 다른 구분자로 각각의 사용자를 구분하
는 통신방식이라는 것은 앞 절에서 공부하였다. 즉 정보 뎨이터가 공유대역（즉 광대
역이 되겠다）으로 정보를 전송할 때 여러 명이 동시어］ 통신을 한다면 그냥 정보를
썩혀버리는 결과가 될 것이다. 여기서 우리는 이러한 신호가 공유 대역폭으로 전송
퇸다 하더라도 그 각각을 구별해 주는 구분자로 신호어］ 표시를 하1 주어야 한다는
것을 알 수 있다. 이러한 표시인자가 바로 코드이다．
 이 절에서는 이러한 CDM/CDMA시스템어］ 사용되는 코 三의 생성방식과 그러한
코드들의 특징 등어］ 대해서 공부할 것이다.
 이것어］ 앞서서 앞으로 공부할 내용의 이해를 돕기 위해서 다음과 같은 기본적인
내용어］ 대해서 이해가 앞서야 한다. 임의의 수가 있을 때 그 수는 그 수를 구성하는
약수（혹은 인수）를 가지며, 또한 이러한 약수는 그것의 배수가 있어서 서로 약수와
배수는 상대적인 입장이 되는 것이다. 또 한가지 중요한 것은 솟수（p由ne）인데 이것
    3. DSSS와 （兀de<기론                          153
.


은 더 이상 쪼개어（나누어）지지 않는 기본적인 요소 수인 것이다. 일반적으로 수를
표현하면 이러한 솟수의 멱 급수로 표시되게 된다. 이것과 병행해서 두수를 비교할
때 요소수인 솟수 중에서 서로 공통되는 솟수가 없다면 이러한 두 수는 서로 소라고
한다． 이상의 이러한 기본적인 수의 개념은 앞서 공부한 2장의 내용과 비슷한 개념
이다는 것을 알 수 있다．


     3.5.1 Galois Field

    물리학에서 장（場 : Field）이라 함은 특정한 물리량어］ 의해서 그것이 영향력이 미
치는 범위를 장이라고 한다. 이를테면 정지한 전하들 간어］ 상호작용에 의해서 형성
되는 전기장, 또한 움직이는 전하에 의해서 형성되는 자기장 등이 그것의 대표적인
예이다. 즉 장이라 함은 그것의 영역이라는 의미 혹은 범위라는 의미로 사용되는 말
이라고 이해할 수 있다．
    이러한 영향력의 의미를 수의 집합들에 적용해 볼 때 우리는 수로 구성퇸 또 다
른 집합단체를 숫자들의 집합의 장으로 또 다른 이름으로 장（場 : Field）이라고도 한
다. 이러한 장은 그것의 구성원소가 유한할 수도 있고 무한할 수도 있다. 특히 유한
한 숫자의 집합을 우리는 유한 장이라고 한다. 여기에서는 이러한 유한 장에 의한
공부를 할 것이다.
    유한 필드는 그 필드를 형성하는 요소의 수가 유한한 경우라고 했다. 즉 자연수나
정수 등은 유한 필드가 될 수 없을 것이며, 0에서 100 사이의 실수 등도 유한 필드
라고는 할 수 없다． 그러나 0에서 100사이의 정수라든가 100보다 작은 자연수라든
가 하는 수의 집합들은 유한 필드라고 할 수 있을 것이다.
    그러면 유한 필드는 그것의 크기（범위）로 그것이 정의될 수 있다. 즉 그것의 영향
력이 필드의 크기어］ 의해서 제한된다는 의미일 것이다. 여기에서 우리는 구성요소
의 크기가 m인 유한 필드 F를 정의해 보자. 이러한 유한 필드는 일반적으로 곱셈이
나 덧셈 등과 같은 연산에 대해서 닫혀있어야 한다. 즉 그러기 위해서는 모튼 연산
의 결과값은 유한 필드의 크기로 제한되어야 하므로 n均dubO-rn으로 계산되어질 것
이다.
    그리고 만약 이 필드가 요소 q를 가지는 또 다른 필드인 E를 크키 m으로 확장하1
서 만들어진 필드라고 한다면, E는ci의 요소를 가지겠으나, E어］ 의해서 확장퇸 F는
／요소들을 가지게 된다. 이때 확장어］ 기본이 되는 유한 필드 E를 Prime Field라
   154                                        3. DSSS와 Code이론
                                                                .


고 한다. Prime Field의 요소들은 0이 포함된 소수이어야 하며, 만약 구성 요소들이
솟수（1과 자신이 약수인 수）의 급수로 나타난다고 한다면 그것은 Prime Field가 아
니라 확장 필드라고 해야 할 것이다. 따라서 요소 q로 표현되는 유한 필드는 q의 크
기가 될 것이며, 이것을 m으로 확장한 확장필드 F의 경우 그것의 크기는 ／이 될
것이다．
 임의의 소수（素數） q의 급수와 양의 정수 m에서, GI疋功로 표현되는 유한 장은
GF佃吩로 표현되는 유한장의 서브 필드이며, GF佃吟는 G只a）의 확장 필드라고
이야기한다. 이러한 Notation을 사용하는 유한 필드를 Galois Field라고 하고 일반
적으로 GF(力로 표현한다. GF（功는 이 필드의 모든 요소를 표현할 수 있는 요소
（앞의 설명에서는 소수라고 하였다）를 가지게 될 것이며, 이러한 요소를 기본요소
(Prin丘tive Element）라고 한다. 또한 이러한 Primitive Element를 근（root)으로 하
는 생성 다항식을 가질 것인데 이것을 Primitive P아ynomial라고 한다. 모든 Galois
field GF(q）는 Prim逋ye Polyno而고을 최소한 한 개를 가져야 한다．
 추가적으로 G只a）를 n과 m으로 확장한 GI疋 "an
                            ）와 GF(q씨의 경우 m이 n으로
나누어 지지 않는고 또한 n이 m으로 나누어지지 않는 다면, 즉 " 서로 소" 라면
GF(a'）는 GF(q吟 의 서브 필드가 아니며, GF( a仇）역시 GF( q'）의 서브필드가 아
니다．
 일반적으로 G只a）의 요소들은 q개가 있으며, 이러한 요소들은 modul아q로 연산
결과의 크기가 제한된다. 실질적으로 우리는 이 장에서 공부하게 될 때 Prime Field
의 구성요소가 '0'과 '1'의 두 가지 element를 가지는 G只2）에 대해서 이야기할 것
이다. 우리의 관심사와 이렇게 유한 필드어］ 대해서 공부하는 이유는 기본요소가 2
인 Galois field를 이야기하기 위해서 였다. 즉 G只2) 혹은 GF( 2끼으로 표현되는
유한 필드어］ 대해서 공부하자.


   3.5.2 선형 Code와 생성 다항식

 일반적으로 선형 코드의 생성을 위해서 선형 필터를 사용하게 된다. 이러한 선형
필터는 Excius如e-OR로 구성된 Parity Generat아（PG）와 Shift Register 역할을
하는 N개의 지연요소들로 구성되어 있다. 이러한 구성으로 출력되는 코드는 선형
코드이며， 대표적인 것이 PN Code이며, PN Code뿐만이 아니라 디지털 신호를 코
딩하기 위해서 사용되는 필터 등에서 많이 사용되는 전형적인 방법이다．
    3. DSSS와 Code이론                                 155
1


    이러한 선형 필터는 각각의 지연요소인 tap의 값을 피드백시킨다고 해서 선형 피
드백 천이 레지스터（LFSR: Linear Feedback Shift Register）라고 한다. 이때 각
각의 tap에서 그것의 값이 변경되거나 또 다른 연산을 하게 되는 형태가 아니므로
이것은 시 불변 선형 시스템이다. 따라서 이것은 선형 필터라고 한다．
    일반적으로 N개의 Shift Register를 사용하여 값을 피드백시킨다면 피드백되는
형태는 피드백 여부에 따라서 2N가지가 있게 된다（피드백할 거냐 피드백하지 않을
거냐에 의한 2가지 경우어］ 의해서 계산된다）. 여기에서 만약 최종 단의 Shift
Register가 피드백을 하지 않는다면 결국 N-i개의 Shift Register 만 있는 결과가
되므로 최종단의 Shift Register 는 항상 피드백이 된다고 한다면 마지막 피드백 단
의 경우가 없어지므로 피드백의 형태는 少이 2N1로 다시 이야기해야 한다. 그리
고 마지막 단 이외어］ 모튼 단이 피드백이 없는 경우 또한 더 이상의 코드 생성이
되지 않는 경우이므로 피드백의 경우의 수에서 제외되어야 한다면 최종적으로 N단
의 LFSR의 피드백의 형태 혹은 생성 다항식의 표현 가능한 수는 다음과 같다.

              생성 다항식의 수 = 2 \   1       (3-26)
              여기에 서 N은 지연요소 인 Shi1 lIes治ter의 수



    또 한가지 생각할 것은 이러한 N단의 LFSR에 의해서 생성될 수 있는 최장의 코
드의 길이는 얼마나 되겠는가9 답은 간단하다. 즉 N단의 Shift Register의 상태가
'0' 혹은 'i '이므로 2N개의 상태가 있을 수 있다. 그런데 중요한 것은 이러한 2N 개
의 상태가 모두 발생될 수 있는 피드백 조합이 필요하게 될 것이다（이것은 최장 코
드 부분에서 상세히 공부하겠다）. 만약 이러한 조건이 만족되는 경우에는 少개의
상태에 의해서 少개의 길이의 코드가 생성될 수 있는 것이다. 그러나 그것의 상태
가 모두 '0' 인 경우를 생각해보자. 이때는 더 이상의 순환은 없어지고 계속 모든 SR
이 '0' 인 상태만을 유지하게 된다. 따라서 최장코드가 되기 위해서는 어떠한 경우라
도 모두 '0'이 되는 상태로 천이 되어서는 안 된다. 따라서 최장코드의 길이는
2'v_ l이라고 해야 할 것이다．
    이러한 Shift Register의 피드백 시키는 형태를 대수적으로 표현한 것을 생성 다
항식이라고 한다. 이러한 생성 다항식은 각각의 Shift Register가 피드백을 하면 i
로 표시하고 그렇지 않으면 0으로 표시（즉 그 항을 없앤다）한다. 이러한 생성 다항
                                                               3. DSSS와 Code이론
                                                                                 .



식은 n개의 지연요소（SR）를 가지는 경우 尤" 과 1은 항상 포함되어서 표시되는 " "
+ ... +1" 의 형태이다. 이러한 생성 다항식은 즉 어떠한 지연요소를 피드백시키는
가는 그것의 상태가 모튼 요소들을 표시할 수 있는가 아니면 일부 부븐 상태에서
계속 맴도는가를 결정지을 수 있는 것이다．


                                  Modulo-2 Adder


                                        /
       Output 寸_ F, (t) 41F1l 1 (t）띠H瓦- 2(t)   寸H
                                                    (U .-.   F (t)


                                                             J        Clock


                                （그림 3-17) LFSR의 구성



     （그림 3-17）는 이러한 LFSR을 나타내는 일반적인 경우이다. 여기에서 각각의
SR들의 경우 그것의 출력이 공통된 시스템 Clock어］ 의해서 다음 단으로 전달되는
경우와 그 출력이 또다시 입력으로 피드백 되는 2가지의 경우가 있다고 볼 수 있다．
여기에서 우리는 SR이 피드백 되는 신호어］ 기여하는지 여부， 즉 Parity Generator
로 연결되어 있는지어］ 따라서 그 SR단, 즉 시간지연 성분단을 '1'로 표시할 컨지 '0'
로 표시할 컨지를 결정한다．
     이때 F/F의 초기값은 상태변화를 위해서 "1"로 하며 PG의 입력 또한 이러한 이
유로 인하여 항상 최종 단의 F/F의 입력을 포함시킨 짝수 개의 입력을 연결시킨다．
     다음 절에서 공부할 PN Code도 이러한 장치에서 SR의 몇 개의 출력을 선택하여
Panty Gener砒아로 피드백 시키고 마지막 SR로부터 출력을 얻을 때 최장의 출력
을 발생하기 위해서 어느 지연요소（SR）의 값을 피드백시킬 건지를 신중히 선택한
다．
     지금까지 공부한 내용을 생각하1 볼 때 눈치가 빠른 독자는 벌써 다음과 같이 생
각했을 것이다. 그렇다. 이상의 설명에서 N단의 Shift Register의 상태는 GF(2自의
유한 장을 표시한다는 것과 이 필드의 모든 요소들을 모두 표현할 수 있는 다항식과
근이 있다는 생각을 했을 것이다．
     즉 SR의 단이 N개인 경우 각각의 단이 가질 수 있는 값이 2라고 했을 때 각각의
    3. DSSS와 Code이론
.                                                         157
                                                      1

단은 2N개의 값들을 표현할 수 있을 것이며, 이것은 GF(2小의 유한 필드의 요소들
을 나타낸다고 할 수 있다． 따라서 이러한 SR의 각각의 상태가 유한 장의 요소들을
표현할 때 그것의 출력은 상태가 다를 경우어］ 출력되는 값은 고유한 값이 될 것이
다． 다시 말해서 출력은 0혹은 1이나 그것의 0혹은 1은 이러한 출력을 나오게 하는
SR의 상태어］ 의해서 결정되므로 그것의 과정이 모두 少가지의 경우가 있다는 이야
기가 되는 것이다．
                                             x2단 즉 두 번 지연된
                                             데이터 값은 modulo -
                                             2 add를 위해서 피드
                      Modulo-2 Adder         백 되지 않는다．




      Outpu m         x3


                                              （기ock


                （그림 3-18) 다항식 g佃）＝兀3＋尤＋1의 LFSR 표현


    （그림 3-18）에서는 1번째와 3번째의 레지스터 출력이 2진 덧셈 되어 1번째 레지
스터의 입력어］ 피드백되는 규칙을 가졌을 때, 즉 생성 다항식이 g佃）＝尤3＋兀＋1로
주어질 때 발생하는 선형코드의 생성과정을 나타내었다．
    만약 （그림 3-18）에서 출력은 尤3단 이후가 아니라 工2단 이후어］ 뽑아낸다면 어떠
한 결과가 발생하겠는가？ 이때는 출력을 형성하는 SR의 피드백 형태가 바뀐 것이
아니라 출력을 뽑아내는 시점의 차이이므로 x3단 이후의 출력 시퀀스어］ 비해서 한
Clock 빠르게 정보가 출력되므로 한 Clock 앞선 시퀀스, 즉 iBit가 천이된 동일한
시퀀스가 출력될 것이다.

     3.5.3 선형 Code의 대수적 표현

    생성 다항식이 g佃）＝兀3＋尤＋1인 LFSR에서 초기값이 모두 1일 때 발생되는 코‘
드들을 생각하1 보자． 여기에서 발생되는 코드는 각각의 SR의 상태 등어］ 의해서 발
생되며, 이러한 SR의 상태의 천이는 다음 그림과 같이 나타난다．
   158                                                                                     3. DSSS와 Code이론
                                                                                                             1




                                                                                                    1
                                        （그림 3-19) LFS日의 상태천이


 이러한 생성 다항식은 GF(x3）의 유한 필드어］ 있는 임의의 요소를 근으로 할 것이
다． 근이 되는 임의의 값 口를 생성 다항식어］ 대입하면 그것의 값은 0이 된다는 것
이다. 즉 1+ a+ a3= 0이며, 각각의 상태를 이러한 임의의 값인 생성 다항식의 근으
로 대응시킨다면 다음과 같이 정리할 수 있다. 다음 절에서 공부하겠으나, GF（們
의 유한 필드어］ 있는 모튼 상태를 표현할 수 있는 생성 다항식의 근을 우리는 원시
요소（Primit如e Element）라고 한다．



         000   （寸）        /   "     1      .



                                               .


                                                   1            모든 요소들이 기본 요소인 寸이하
                                                                                               /
         001   （乂l :                a                           로 표현이 가능하며 , 크기 8로 (23)      /
                                                                                              /

                                                                으로 제한되고 있음．
         010   a2                 （甲

         011   a3                 14a
                                                            寸＝14U 이 다．
         100   (Xl                (X+(X2


         101   （戶    i 1+ai-a
                                                        겨 L 耐在六付" 奸 '他「
         110   c多    i.           1녀寸X2 /
                                                   J
                                                          GF(23) = {0, 1, cx，寸, （工3, .. . . .. , 寸｝이다．
         111   a7         \         1 /


                                                       （그림 3-20) 대수적 표현


 여기에서 주의할 것은 부호가 없다는 것과 갇은 값 2개는 서로 없어진다는 것이
다． 이것은 전형적인 excius如e-OR연산의 결과에 의해서 그렇다. 이러한 점을 생각
하여 정리하면 （그림 3-20）과 같은 결과가 나타날 것이다. 이상과 같은 결과로 볼
때 크기가 n-i인 다항식어］ 의해서 생성되는 시퀀스를 n-tuple 2진 벡터로 표현하는
방법을 정리해 보자．
 즉 지연요소를 나타내는 兀' 에서 n은 지연의 값을 나타낸다고 볼 수 있다. 즉 n=0
이면 지연이 없는 현재의 Bit정보를 말하고, n= 3이면 3번 지연된, 즉 3 Clock 전
1 3. DSSS와 CodeOl론


어］ Bit정보를 말한다． 예를 들어서 발생된 시퀀스가 "1110100" 이라면 오른쪽에서
첫 번째 0은 현재의 출력Bit를 말하는 것이고 오른쪽에서 5번째의 1은 이미 4번 지
연된， 즉 2 C1兀k 이전 당시의 현재 값이므로 현재의 시점에서는 2 Clock 전（前）
과거의 값이다．
 따라서 이 시퀀스를 대수적으로 표현하면 工6＋尤5＋尸＋尸+ 1로 표현된다．


         1      1   1     0    1     0    0         x6 + x5 + x4 + x2 + 1



          현재시점올    기준으로 4                현 재시 점
          이ock 앞의 값으로 현시점
          에서는 4번 지연된 값                   x6+ x5+ x4+ 0x3+ x2+ 0x1+



                              （그림 3-21) 시퀀스의 대수표현


   3.5.4 원시 다항식

 우리는 앞서서 유한 필드에서 존재하는 요소들을 표현할 수 있는 방법어］ 대해서
공부했다．이러한 요소들을 표현할 수 있는 방법은 선형 필터의 피드백 형태를 규정
하는 생성 다항식으로 가능하다는 것을 알 수 있었다. 그런데 이러한 생성 다항식은
N개의 SR로 구성되어 있는 선형 필터에서 21 1小1개가 존재할 수 있다는 것을 공
부했다. 예를 들어서 N=3일 때 才-1_i = 3개가 구성될 수 있다. 즉 尤3＋尤2＋兀＋1와
兀3＋兀＋1, /＋尸＋1 등이 그것들이다．
 그렇다면 이러한 3개의 생성 다항식은 이것들이 표현하고자 하는 GF(23）의 모든
요소들을 표현할 수 있겠는가7 지금 확인해 보자．
 즉 초기값을 111로 둔 상태에서 각각의 다항식에 의해서 발생되는 SR의 상태를
정리하면 （표 3-2）와 같다．

                （표 3-2) GF(23）의 모든 다항식에 의한 시퀀스 발생

    다항식                                            상태천이                       和鞋
 兀3 + r + 兀＋1       111        111

   工3 + 兀＋1         111        110       101      010   100     001   011   111

   / + 尤2 + 1       111        110       100      001   010     101   011   111
   160                                  3. DSSS와 Code이론
                                                          U


 （표 3-1>에서 첫 번째 다항식은 초기상태 111에서 더 이상 진행되지 않는다는 것
을 확인할 수 있다. 물론 이 다항식도 7개의 초기상태를 가질 수 있으나 특정한 순
환의 주기어］ 포함된다 하더라도 그것의 상태천이가 111로 들어오면 더 이상 진행이
되지 않는다는 것을 우리는 알 수 있다. 첫 번째 다항식은 다음의 （그림 3-22）과 갇
이 3가지의 서로 독립된（연관되어지지 않은） 3개의 순환들로 각각 구성되어 있다．
 즉 초기상태가 111일 때는 계속 111어］ 머물러 있고, 초기상태가 010이나 101일
따는 이 두 상태를 맴톤다. 마지막으로 나머지 상태들은 그것들끼리 또 순환주기를
유지하면서 더 이상 진행되지 않는다．
 또한 나머지 2개의 다항식은 그것이 GF(23）상의 모튼 요소들을 모두 표현할 수
있는 상태를 가지고 순환함으로 어떠한 초기상태에서도 （표 3-1）의 형태와 같은 상
태로 회전함을 알 수 있다. 즉 이러한 다항식어］ 의해서 발생되는 코드는 순환적인
코드임을 알 수 있다. 이것은 임의의 SR의 상태가 이전 상태와 진행할 상태가 언제
나 존재하기 때문어］ 순환이 된다는 것을 확인할 수 있다．




            （그림 3-22) 다항식 尸＋/＋兀＋1의 상태천이


 위의 결과를 통해 알 수 있둣이 유한 필드 GF(23）의 모든 요소들을 표현할 수 있는
생성 다항식은 모튼 생성 다항식이 아니라 몇몇 개의 다항식어］ 의해서 구해진다. 이러
한 다항식은 그것의 근이 원시요소（I거imitive Element）인 원시 다항식（Primitive
P아ynomial)이다. 이러한 원시 다항식은 그것의 근이 Galois Field의 모튼 요소들
이 아니라 몇몇의 요소이므로 원시 다항식 역시 모튼 생성 다항식이 될 수 없다．
 원시 다항식은 약분할 수 없는 P1如ne이다. 즉 낮은 차수의 다항식들의 곱으로 표
현할 수 없다（그렇다고 약분 불가능한 다항식은 모두 원시 함수인 것은 아니다）. 원
시 다항식이 아닌 다항식들은 주기가 ( 2m_ 1)보다 작은 수열을 발생한다. 예를 들
면 g佃）＝兀5＋尸＋尸＋尤＋1은 원시 다항식이고 주기가 31인 m 시퀀스를 생성한다．
    3. DSSS와 Code이론                             161
口


그러나 g佃）＝尸＋尤3＋尸＋尤＋1은 낮은 차수의 약분함수로 나누어지지 않으므로
약분 불가의 다항식이지만, 주기가 15가 아니고 5인 시퀀스를 발생하므로 원시 다
항식이 아니다．
 g佃）＝兀5＋兀＋1= (x3＋尸＋1)(x2十兀＋1)로 인수분해되므로 약분이 가능한 함수
이다. 두개의 요소다항식 付＋尸＋1)과 付＋尸+1)는 원시 다항식으로서 약분이
불가능하다．


 최장코드와 원시 다항식의 관계
 우리는 위에서 원시 다항식어］ 의해서 생성되는 최장 코드는 모든 요소들을 모두
표현하는 주기적인 형태를 나타낸다고 공부하였다. 또한 이 최장 코드의 킬이는 L
(2m_ 1)로 표현되며, 원시 다항식의 최고차 항은 ／오l 것도 알았다（여기에서 m은
지연요소인 SR의 수）.
 그렇다면 여기에서 흥미로운 사실을 하나 찾아보자. 원시 다항식과 이 다항식어］
의해서 생성되는 시퀀스간에는 어떠한 관계가 있겠는가？
 생성 다항식은 그것어］ 의해서 생성되어지는 시퀀스를 대표하는 것을 말하며, 이
것은 수학에서 함수의 표현을 간단히 수식으로 표현하는 것과 갇은 의미이다. 우리
가 주기함수를 표현할 때에는 한 주기의 표현으로 그 함수를 모두 말할 수 있다. 즉
최장 코드를 생성하는 생성 다항식인 원시 다항식은 이 다항식어］ 의해서 출력되어
지는 시퀀스를 modulo연산하면 그것의 모양과 같은 것이 된다. 다음의 예제를 풀어
보자.

             SR이 3개 있는 생성 다항식어］ 의해서 초기상태가 111인 경우어］ 출
             력되는 시퀀스는 11101（刃이다. 이때 생성 다항식을 구하여라．

             생성 다항식은 시퀀스의 modulo연산을 취함으로 구할 수 있으며, 그
             것은 시퀀스의 대수적 표현식을 ( 1＋尸）로 나누어서 구할 수 있다．
             즉 시퀀스의 대수적 표현은 1110100 : l＋兀＋尸＋尸 이다．
             즉 시퀀스를 1＋尸로 나누어서 쿠한 근은 (1＋兀＋兀3)이며, 이것은
             생성 다항식이 된다. 그런데 만약 초기상태가 111이 아니라 001과 갇
             이 첫 번째 요소가 1이 아닌 경우는 어떻게 되겠는가？ 이것 역시 마
             찬가지로 출력 시퀀스는 각각의 요소들이 주기적으로 순환함으로 결
  162                                                                                                                                 3. DSSS와 Code이론
                                                                                                                                                                         1


             국은 그것의 표현이 기본 출력 시퀀스 万（尤）어］ 工"을 곱한 형태로 나
             타날 것이며, 이것은 力佃）의 n번 지연된 시퀀스라는 것을 나타내는
             결과가 될 것이다．


                                                      1 + x + x3

                                    1+   y+

                                    "V
                                                                           ?／   伽뇨0/ #                   '                                *                *:,,,,,
                                                      乂 + x + X? +
                                                      X*
                                              y                                                                                                  OA*
                                                                 小，                                                         Ox1
       '1110100' 의 대수적 표현                                       \ +\1X? + Ox' 了· x寸 + 口v' #                                                                   +

                                                                \ \x2 + X了 +
    乞巾




                                                                                    \J*        \v            -     \x             '   +    Ox"         Y x'
                                                                                    Xy ＋낭 入／Y X"
                                                                                                                                                       0

 초기상태가 ()(끄인 경우에는 어떻게 되는지 직접 확인해 보자．




    x가］ + x + x2) = 心n川         r' + Y，了 + /'                                                                                     ::,,4
                                                                           #                                 '          *                                            #
                                                                                           '
                                                                                                                                             # Ox』*
                                                           乂*
                                                                      Ox
                                                  ／
                                                                                六
                                                                                                    a/
                                                                                                                                                              Oxh
                                                           乂f X + /                        +


                                                                X +\Y多 + {／낯「" + x4 于 a寸" 于 n\/' +
                                                                \ 쿠＼\X2 + Xx1 +
         '1110 100' 보다 2이ock앞

          선 "0011101' 의 대수적
                                                                                          낳＋V勺%X" + ：六
                                1                                                          i +\                  \xb                      t x'
                                                                                                                                                       0

 결과적으로 이것의 몫은 /（枷吃이며, 이것은 肛）에서 출력되는 시퀸스보다 2
Clock 빠르게 출력되는 시퀀스라는 것이 될 뿐 마찬가지로 동일한 생성 다항식을
가진다．
 따라서 시퀀스를 통해서 우리는 생성 다항식을, 즉 원시 다항식을 구할 수 있다는
것을 확인할 수 있었다．
    3. DSSS와 Code이론                                   163
.




    3.6 PN Code                                             )

    앞서 공부한대로 선형코드는 선형 피드백 천이 레지스터（LFSR）에 의해서 생성
되어진다. 이때 LFSR은 각각의 지연요소인 SR의 상태에 의해서 출력되는 값이 결
정되므로 그 값이 비록 같다 하더라도 그 값이 결정되는 SR의 상태는 다르게 된다．
즉 SR의 개수, 즉 지연성분의 길이7FN인 경우 SR의 상태는 0과 1인 2가지 상태이
므로 모두 少가지의 초기값이 있을 수 있다. 때문어］ 그것의 길이는 少이라고 할 수
있다. 그러나 그것의 초기값의 결정은 피드백된 신호가 무엇인가어］ 따라서 이러한
최대의 초기값을 가질 수도 있지만 그렇지 않을 수도 있기 때문어］ 모든 경어］ 코드의
길이가 최대 길이인 少이 된다고는 할 수 없다. 여기에서 주의할 사항은 초기값이
모든 SR에 '0'일 경우에는 더 이상의 진행이 되지 않O므로 이 경우를 제외한다면
최대길이는 少-1이 되는 것이 타당할 것이다.
    즉 N개의 SR을 가지는 선형 필터어］ 의해서 생성되는 최장 코드인 PN Code의
길이 L은 兀＝2'v_ l로 표현된다. 즉 PN Code의 길이는 7, 15, 31, 63, 127,    등
의 길이민을 가지게 된다. 여기에서 N은 SR의 수이다. N개의 tap에서 생성되는 코
드（즉 경우의수）의 킬이는 沙이나 초기 상태가 모두 zero일 때를 제외하게 되기 때
문이다. 만약 모든 값이 0일 때는 더 이상 코드의 상태가 진행되지 않을 것이다. 이
러한 이유로 인해서 PN Code의 "1"과 "0" 의 개수는 "1"이 하나 더 많다.
    원시 다항식에서 얻어지는 PN Code는 앞 절에서 설명한 Galois Filed내의 모든
원소들을 다 포함하는 최장 길이小勿ximal length Code) 코드이다. 이러한 최장 길
이의 코드는 코드를 생성하는 다항식어］ 의해서 최장 코드인지 아닌지를 결정할 수
있으며, 전체 지연요소의 길이어］ 의해서 가능한 수가 별도로 제한되어 있다. 이와
같이 PN Code는 상당히 긴 주기 코드이다. 즉 주기가 상당히 길다는 이야기이고
이것은 잡음의 성질과 비슷하게 랜덤성을 가진다는 것이다. 만약 주기가 짧은, 즉
크기가 작은 유한장의 요소들을 가지는 코드의 최장 코드라고 할지라도 이것은 주
기가 짧기 때문어］ 랜덤성이 상당히 떨어진다고 할 수 있다．
   164                                           3. DSSS와 Code이론
                                                                   S


  3.6.1 최장코드의 수

 앞서서 공부했듯이 크기가 m인, 즉 GF( 2씨인 Gahiis 필드내에 존재하는 수많은
코드들 가운데에서 크기 m인 필드의 모든 요소들을 모두 포함하는 코드를 최장
(Maximal Length）코드라고 하였다. 이러한 최장코드는 m깨의 지연요소인 SR을
가지며, 이것에 의해서 출력되는 코드의 길이는 (2m寸1)으로 나타난다．
 이러한 최장코드는 그것이 생성되기 위해서는 몇 가지 특별한 조컨을 만족하는
다항식어］ 의해서 생성되는데, 크기가 m인 다항식이 （兀" +1)의 약수 혹은 약분 다
항식이며, 더 이상 분리되지 않는 기약분 다항식일 켱우어］ 최장코드라는 것을 공부
하였다．
 예를 들면 8佃）＝尤5＋尸＋尸＋兀＋1과 8佃）＝兀5＋尤3+ l은 5차의 원시 다항식이
다. 왜냐하면 g（功가 나누어 떨어질 수 있는 최소의 차수가 다항식의 크기 刃i= 5인
경우의 길이인 乙＝25-1= 31 이기 때문이다. 즉 （尤缸＋1)는 8佃）가 나누어 떨어
지는 최소 차수의 다항식이기 때문이다. 그러나 8佃）＝兀5+尸＋尤3＋尤2＋尤＋1은
냠+1)을 약분할 수 있으므로, 乙＝6이 되고 이것은 크기 m= 5인 경우의 최장코
드의 길이인 31의 차수가 아니므로 원시 다항식이 아니다．



    약수들은 각각이 서
    로 배수 관계가 없
    는 솟수로 나누어져
    야한다. 즉 幻（노) 는
    r+ ／올 제외한 어
    뗘한 다른 약수와도
    배수관계가 없어야
    한다．




         (,Y/' + 1）이 끄7차의 다항식 g (x) 로 나누어 떨어지는 최소차 항인 경우이다．

                      （그림 3-23) 최장코드의 구성



 그렇다면 크기가 m인 유한 장어써 존재하는 원시 다항식의 수는 얼마나 되겠는
가？ m차의 원시 다항식의 수는 다음과 갇다．
     3. DSSS와 （兀de이론
 1                                                                      165


          -q (2"' -1)
                 .   .   _...




                                                                        (3- 27)
             1
          m

     여기에서 叭L)는 Euler의 함수라고 하며, 그것의 값은 다음과 갇이 구할 수 있다．

          . . .    .    l . .』 1 . . .. 1 .
          9 L) == I乂1- -乂1- -月＼(1- -)                                   (3- 28)
                       I가      p2       p,
  여기에서 功는 L의 솟수들이다．
  예를 들면, 中（15) = 15(1卜1/3)(1 -끄旬= 8이 되고, 15보다 작고 서로소인 수는 1,
2, 4, 7, 8, 11, 13, 14이며 8개이다. 소수 p보다 작은 모든 자연수는 p와 서로 소이므
로 p의 Euler의 함수 a功＝佃- 1）임을 알 수 있다．


                                （표 3-3) S日에 따른 최장 코드의 수

       SR수（=m)                  길이（L=2m너）          f (L)        최장 코드 수
          3                         7                6             2
          4                         15               8             2
          5                         31              30            6
         6                          63              36            6
          7                        127              126           18
         8                         255             128            16
         9                         511             432            48
         10                        1023            600            60
         15                       32767       27000(7,31,151)    1800


 （표 3-3）은 지연 요소인 SR의 수어］ 따른 최장 코드를 형성할 수 있는 원시 다항식의
수를 나타낸다． 여기에서 시퀀스 길이 L은 (2仇- 1)이며, 최장코드 수는 功（2m- 1)/L
로 구해진다．
 위의 생성 다항식 중 특히 g佃）＝兀加＋兀左＋1(1＜七＜刃2) 형태의 식은 세 개의 0이
아닌 항을 가지는 식으로 3항식（t1in이nial)이라고 한다. 3항의 생성 다항식은 선형
레지스터 피드백 회로어］ 차수 m어］ 관계없이 단 하나의 exclusive OR Gate를 가지
                                                  3. DSSS와 Code이론
                                                                    .



므로 지연이 적어서 고속이 된다. 따라서 실제회의 설계 시어］ 비용이 적게 들 뿐 아
니라 고속이므로 유용하다．
寸，J r ( 砦肖： m이 15인 경우 이러한 LSFR(L岫ar Shift Feedback Register）에
            서 존재할 수 있는 원시다항식의 수는 모두 몇 개인가 ?

          이 경우 최장 코드의 길이는 L= 2馬- 1= 32767이다. 여기에서 功
          (32767）을 구해서 m=15로 나누면 된다. 叭32767）를 구하기 위해서
          32767의 솟수를 구해야 하는데 32767=7X 31 x 151로 표시될 수 있
          으며, 따라서 32767을 구성하는 솟수는 7, 31, 151라는 것을 알 수 있
          다. 따라서 功（32767) = 32767(1- 1/7)(1- 1/31)(1- 1/151) = 27000이
          다 .




       따라서 원시 다항식의 수는 27000/15=1800개이다．
 위의 예제의 경우 현재 우리나라에서 사용하고 있는 CDMA 이동통신시스템의
PN Short Code인 경우인데 이것은 기지국 식별용으로 사용된다. 재미있는 것은
SR이 15인 경우 가능한 생성 다항식의 수는 214_ 1= 16383개인데 그 중의 약 10%
만이 최장코드를 생성할 수 있는 다항식이라는 것이다. 물론 최장코드의 수와 전체
생성 다항식의 수와는 선형적인 관계가 있는 결코 것은 아니다.（식 仔27）과 (3-28)
을 참고하라） 따라서 모든 생성 다항식의 10%정도가 최장코드의 생성 다항식이라
고 할 수는 없다. 다만 최고 코드의 생성 다항식이 아주 특별한 경우라는 것을 강조
한다．
 SR이 15와 42인 PN Code는 각각 Short, Long Code로 사용되는데, 현재 상용
시스템의 경우 1.2288八flcps의 대역으로 이러한 코드를 전송하므로 길이가 32767
인 short코드의 경우 약 26.7ms이면 한 주기를 모두 전송할 수 있고, 길이가
43980465111303인 PN Long Code의 Q43579139초但恥1박 42일）가 경과해야 한 주
기를 전송할 수 있다．

   3.6.2 1가dCode의 특성

 최장 길이 코드인 PN Code는 앞에서 공부한 m코드가 가지고 있는 모든 특성을
가지고 있다. 이 절에서는 특히 우리가 관심 있게 보아야 할 그리고 실지로 이러한
코드가 적용되는 CDMA 시스템에서 적용되는 특성들을 주요 관심사항으로 정리하
    3. DSSS와 Code이론
1                                                                       167


겠다．


    천이 및 합（合）의 특성

    하나의 최장 코드와 또 다른 최장코드를 mod 2로 합하면 또 다른 최장 코드가
된다．
    즉 최장 코드의 각각의 Bit를 mod2연산하게 되면 각 Bit별로 더하게 되므로 킬
이는 최장 코드의 길이가 될 것이다. 또한 각각의 Bit의 값들은 0혹은 1로 나타난다．
최장 코드는 모든 요소들이 모두 동원되어서 표현되는 길이의 시퀀스이므로 이러한
연산의 결과는 결국 최장 코드의 또 다른 모습일 수밖에 없다. 차이가 난다면 아마
도 코드를 생성하게 될 것이다．


 자기상관함수의 특성
 PN Code는 정규화한 자기상관함수로 다음과 같이 표현퇸다．


        凡（i)   ＝諱
                                （-
                                     1)
                                          "! ' " i"


                    =l
                                                 江0
                                                      (mod N)
                                                                        (3- 29)
                              卜1/N               泮0 (mod N)

 위의 식에서 알 수 있듯이 자기상관함수는 PN 시퀀스와 그 시퀀스의 천이되어진
형태의 코드와의 각각의 Bit별 mod-2연산 결과의 평균을 말하는 것이다. 이러한
연산의 결과는 PN 시퀀스의 길이로 발생될 것이며, 앞서 공부한 바와 같이 천이 및
합의 특성어］ 따라서 또 다른 천이를 하게 된 PN 시퀀스가 된다. PN 시퀀스의 경


                                                            +1




                         -N
                                                                -I/ N

            （그림 3-24) 최장 코드의 정규화된 주기적인 자기상관함수
                                                                   3. DSSS와 Code이론
                                                                                     U



우 항상 1이 0보다 하나 더 많으므로 1가 0이 아닌 이상 자기상관의 값은 1/N의
값이 될 것이다. 즉 동일한 지연을 갖는 PN Code간에는 자기상관 값이 가장 큰 값
이 발생되나 조금이라도 어긋난 경우에는 현저하게 떨어지는 자기상관 값을 가짐을
알 수 있다. 이것은 다음 장에서 공부하게 될 Code동기어］ 아주 유용하게 사용된다．
               A= 0(刃100110101111의 ／뇨此o-Co玎elati아i R(5）를 구하라．

               A = 000100110101111, T'5A = 011110001001101로 위어］서 7자리가
               일치하고 8자리가 다르다. 즉 Aq）戶A는 7개의 0과 8개의 1을 가진
               수열이며, 이것은 또 다른 최장 코드이다. 어찌 되었든 R(5）는 - 1/15
               로 나타난다．
 이상과 같이 최장 코드는 위상차佃ut-of-Phase）가 있을 때와 없을 때어］ 자기상
관함수의 값이 극단적으로 나타남으로 코드 동기（Code Syi兀뇨on切毗ion）어］ 아주
좋은 특징을 가진다. 이것은 4장어꺼 다시 상세하게 공부하게 될 것이다．


                                      동기창




    1                      >

                          t= 0                           t= T

                                                  (a) 주기성 자기상관



                   1> 0
               1                  +    +    +        +

     받-J                       t= 0                         t= T


                                           t= T
        t= o
                                                  (b) 비 주기성 자기상관

                                           （그림 3-25) 자기상관의 종류



 여기에서 동기를 확인하는 윈도우의 크기어］ 따라서 주기상관함수와 비 주기 상관
함수로 구분할 수 있는데, 창의 크기가 최장코드의 길이보다 크다면, 즉 최장코드의
한 주기를 한꺼번어］ 자기상콴함수를 구한다면 （그림 3-24）과 같이 주기적인 상관함
수로 주어질 것이다. 그러나 （그림 3-25）의 (b）와 같이 창의 크기가 최장 코드의 1
    3. DSSS와 Code이론
U


주기보다 작거나 같은 경우에는 비 주기적인 상관함수가 될 것이다. 그러나 최장 코
드가 너무 길 경우에는 주기상관함수를 구해서 한다는 것은 현실적이지 못하기 때
문어］ 2단계로 나누어서 초기에는 부분 동기창을 통하써 특정한 값 이상을 나타내는
지를 비 주기 자기 상관으로 확인 후 전체적인 비교를 하는 주기 자기상관함수로
동기를 맞추는 방법이 일반적인 방법이다．

 Run 특성

 런（Run）은 1또는 0의 연속된 열로써 어떠한 최장 코드도 각 부분들이 정수로 구
성되어 있으면 런들의 반（1/2）은 길이가 1이고, 1/4은 길이가 2이고 (1/2)3은 길이
가 3, ··· 이다. 특히 길이 rn인 런이 하나, 길이 rn- i인 0의 런이 하나, 길이
k(0<k<rn- 1)인 런의 경우 1이튼 0이튼 그 수는 같고 2m나口이다．
    블록을 일련의 1의 런（1로 구성된 string, 즉 11···111), 그리고 갭（gap）을 일련의
0으로 구성퇸 줄이라고 정의한다.
  첫째 창 특성어］ 의해서 rn개의 연속된 1은 단 한번 존재한다. 그리고 이 블록은
0이 앞어］ 오거나 뒤어］ 따라온다. 그러나 111···10(1이 rn- i개）이나 01...lii은 단 한
번 발생되므로 oii1...11i0은 결코 일어나지 않으며, (rn-i)의 길이를 가지는 블록
은 존재하지 않는다．
    둘째 길이가 左(0（左＜仇- 1)인 블록의 개수는 沙d肝2）이다．
    셋째 블록의 총 개수는 1+zmd肝기＝2（桁助이다．
    넷째 블록의 경우와 마찬가지로 길이가k(0 (k<rn- 1)인 블록의 개수는 2仇4m2）이다．
    다섯째 길이가 m인 갭은 없으며, (rn-i)인 갭이 하나 존재한다. 갭의 총개수는
l ＋兄mm2) = 2 伽-2)이다.
    예를 들어서 주기가 31인 최장 콰三 lililol000iooioloii0000iilooiio의 런 특
성은 다음과 같다．

           런 길이            Bk그ok (B幻ck)         갭（Ga이
            k=1                 4                 4
            k=2                 2                 2
            k=3                 1                 1
            k=4                 0                 1
            k=5                 l                 0
    170                                                 3. DSSS와 Code이론
                                                                          U




 분할 특성（Decimation Property)

 최장코드 C의 n분할은 d川으로 표시하고, 모두 0이 아니면 주기 N/ gcd(N, 功
을 가진다．
  n을 양의 정수라고 할 때 시퀀스 兀의 매 n번째의 Bit를 취하여 시퀀스 y라고
한다. 즉 모든 i는 z의 원소이며 )b＝尤万이다. 시퀀스 y를 尤의 n분할이라고 하
고 尤［川으로 표시한다. 특정 위상 특성을 입증하기 위해서 N=7개의 시퀀스 중 단
지 cr1001011만 Ci＝匈를 만족한다.

 분할특성의 좀더 구체적인 실 예를 한번 생각하1 보자. c = 1110010을 고려하면
N=7이고 소수佃如cie）이므로 분할시퀀스 c[n](n 'l, 2, 3, 4, 5, 6）은 모두 주기가 7
이고 최장 코드이다. 이때 c{1] =c이고, c{2] =1100101= T 'c, c[3] = 1001110,
c[4] =1011100= T5c, c[ 5] ==1101001= T5c[3], c{6] =1010011= T5c{3] O]다.
c[1], c[2] 그리고 c[4］는 다항식 g佃）＝兀3＋尤＋1어］ 의해서 생성된다. 결과적으로
분할특성은 단 하나의 회로로 적절한 분할을 통해서 서로 다른 최장 코드를 생성할
수 있다는 것이다. 따라서 m차의 하나의 원시 다항식이 주어지면 다른 모든 m차의
원시 다항식을 구할 수 있다．
 위의 예의 경우, 최장코드 c[nl = c{3] = 1001110을 생성하기 위해서는 （그림
3-26）의 회로를 사용하여 구할 수 있다. 그러나 원래의 Clock 속도보다 n= 3배로
동작시키고 회로의 출력 단에서 매 3번째 샘플을 추출하여야 한다. 일반적으로 분
할 시퀀스 c[N-1]은 최장 코드 C의 역천이와 동일하다．

                                                  매3단마다 샘푤링
                                                  '.. 1001110.




                                                    中
                                      샅쐐L
                             0 l      111
                          日
                          9           011
                                      001

                             3 4 ma
                                      100
                                      010
                         h
                         n            101
                                      110


                  （그림 3-26) 분할에 의한 시퀀스의 생성
1
    3. DSSS와 Code<기론                                 171
                                                           I
     3.6.3 PN Code를 CDMA에小I 사용하는 몇 가지 이유

    무선 이동통신에서 확산 스펙트럼을 이용한 통신을 할 때 전송할 신호를 특정한
코드어］ 대응시켜서 통신하는 CDMA방식을 앞서 공부하였는데, 이때 사용되는 코
드는 몇 가지 중요한 특성을 필요로 한다．
    첫째로는 그것의 상관 특성이 좋아야 한다．
    이러한 특성은 코드를 주파수나 시간구분 이외의 또 다른 구분인자로 사용하는
CDMA에서는 필수적인 사항이다. 즉 코드간의 구분이 용이하고 명백해야 새로운
구분자（코드）가 유용하기 때문이다. 그러나 PN Code의 경우 상관 특성이 다른 코
드간에는 그리 좋은 편이 아니다. 즉 같은 코드일 경우에는 높은 피크를 나타내지만
다른 코드간에는 같은 코드일 때와 구분이 가지 않을 정도로 현저하게 떨어지지 못
하기 때문이다. 그러나 동일 코드에서 약간만（1 Chir汐］상） 위상이 어긋나도 그것의
자기상관 특성은 현저하게 저하되므로 CDMA 시스템에서는 PN Code를 사용하나
동일한 코드를 사용하고 그것의 위상지연（시간 지연 성분）만을 주어서 구분하는 방
식을 사용한다. 이러한 문제로 인해서 현재 상용 CI끄江A시스템（QCI呱4A）는 각각
의 기지국들에서 정확한 시각정보를 가지고 있어야 하며, 관리하고 있는 시간정보
는 기준시점을 PN Code의 옵셋으로 환산해서 관리한다. 이런 특징으로 인해서 흔
히 이 시스템을 동기식 CI呱4A 시스템이라고 한다．
    두 번째로 충분히 그것의 주기가 충분히 길어야 한다．
    충분히 길지 못하면 상기와 같은 방법으로 기지국 혹은 단말기를 구분하는 동기
식인 경우에는 그것의 옵셋이 작아지던지 코드의 개수가 작아지던지 둘 중 하나가
되어야 한다. 따라서 충분히 긴 코드가 필요하다．
    기지국간을 구별하기 위해서는 충분한 PN Ch加의 옵셋이 필요하다. 이 옵셋은
전송경로의 차이로 인해서 서로 다른 기지국의 신호가 동일한 기지국의 신호로 오
인될 수 있는 가능성을 줄이기 위함이다. 1.2288八4cj羚인 경우 iCh如은 약 266m정
도의 거리를 나타낸다. 즉 PN Code의 1ch巾의 차이는 전송경로 차이가 266m가 되
면 동일한 신호로 오인될 수 있다는 이야기가 퇸다. 따라서 충분한 옵셋을 줌으로
이러한 문제를 사전어］ 없앨 수 있는 충분한 코드의 길이가 필요하다.
    QCDMA의 경우 64Ch如을 1 Pilot Index로 설정하여 PN Short Code의 길이가
(2巧 1)이므로 전체적으로 512개의 옵셋을 관리한다.
        172                                  3. DSSS와 Code이론
                                                               1



      3.1 w눼sh Code

      1923년 J.L.Walsh는 직교 함수계를 정의하였다. 이러한 직교 함수계의 직교 코드
     들은 서로가 직교佃rthogonal）함으로써 그것의 상호 상관값은 "0"이 된다. 이 말은
     서로 다른 코드인 경우에는 서로 상관성을 계산하면 0이 되므로 분명히 구분이 된
     다는 것으로 코드를 이용해서 구분하고 싶을 때에는 이러한 직교 코드를 사용하는
     것이 가장 이상적이다. 따라서 이러한 직교 코드인 M囹sh Code는 CI呱4A와 같은
     시스템에서 채널을 구분해 주는 용도로 사용되고 있다. 우리가 흔히 Code Channel
 이라는 말을 하는뎨 이러한 채널 코드의 형성어］ 사용되는 코드가 \7Ta1sh Code인 것
 이다.
      Walsh C月e가 직교 코드이기 위해서는 직교계 내어］ 있는 또 다른 코드와의 상관
성이 직교의 값인 "0"이 되어야 하고 따라서 각각의 Bit간의 비교값이 같은 경우와
다른 경우가 같은 수로 나타나야 한다. 예를 들어서 1100과 1010는 서로 같은 Bit가
2개, 다른 Bit가 2개씩으로 전체적으로는 같은 Bit와 다른 Bit가 2개씩으로 같다．
      Walsh 함수를 생성하는 방법은 Raden追cher함수를 이용한 방법, Walsh 함수의
대칭성을 이용한 방법, H可damard n也trices를 이용한 방법, 선형 천이 레지스터를
사용한 방법 등이 있다. 그러나 이 절에서는 현재 사용되고 있는 Hardamard
n也trices를 이용한 방법과 \Valsh 함수의 대칭성을 이용한 방법에 대해서 설명하겠
다．
     ＼자aish Code, 즉 직교계의 코드들은 Bit별로 비교할 때 같은 Bit와 다른 Bit가 같
다고 했다. 그렇다면 코드 자체를 이런 형태로 만들어 주면 될 것이다. 또한 이러한
직교 코드의 경우 할상 짝수 개의 Bit로 구성되는 코드들일 것이다. 따라서 가장 작
은 코드의 경우 가장 작은 짝수인 2의 길이를 가진 코드가 될 것이며， 그것은 같은
Bit 하나와 다른 Bit 하나로 구성되기 위해서 (10）콰 (11）로 구성될 것이다.
     여기에서 우리는 이러한 점어］ 착안하여 다음과 같은 행렬을 생각할 수 있다.


          [: 小［二：骨］                                    (3-30)


     그리고 이러한 행렬의 하나의 요소들은 또 다른 행렬로 생각할 때 다음과 같이
확장이 가능하다．
         3. DSSS와 Code이론
     .


         （그림 3-27）과 같은 형태로 직교계를 형성하는 행렬을 Hadamard 八4atrix라고 한
다. Hadamard M比小（는 직교계를 나타내는 행렬로 그것의 구성이 되는 요소들이
직교 코드가 된다. 이러한 방법은 현재 사용되고 있는 CDMA 망에서 채널을 구분
하는＼자aish C넌e를 생성할 때 사용한다. 또한 이러한 직교계는 그것의 코드 하나하
나를 표시하기 위해서 인덱스를 가지며, 실지로 이러한 인덱스는 IS-95의 Reverse어］
서는 변조방식어］ 응용되어 사용되기도 한다. 자세한 사항은 7장을 참고하라．

                                             ／尸                                     \



                                                  0   0   0   0     0   0   0   0

                                                  0   1   0   1     0   1   0   1

                                                  0   0   1   1     0   0   1   1

                                              i0      1   1   0..   0   1   1   0

                      0    0         0   0        0   0   0   0

                      0    1         0   1        0   1   0   1

                     {)1   0                      0   0   1   1

                                                  0   1   1   .9
                      0    1             0


                               (b)

                               （그림 3-27) Hadamard Matrix의 확장



         또 다른 형태의 \Valsh Code의 생성방식은 다음과 같다. 이 방법은 대역확장을
용이하게 하기 위해서 Code Channel어］ 사용되는 \Valsh Code를 발생하게 하는 것
이다. 이것은 OVSF(Orthogonal Variable Spread Fac切r）라고 하며 3GPP에서, 즉
비동기 CDMA에서 Code Channel을 만들 때 사용한다． 앞서 한 직교계와 달라질
것은 없다（직교계의 구성요소가 바뀐다는 것은 말이 안 되고···）. 다만 그것의 코드
의 순서, 즉 인덱스가 달라지는 것이다. 이것은 코드에서 1혹은 0의 무리를 한꺼번
어］ 모아서, 즉 연속적인 1 혹은 0으로 코드의 인덱스를 재배치한다고 생각할 수 있
다．
         이것은 코드워드의 길이의 반은 그대로 두고 반은 역으로 하는 형태로 코드를 구
성한다 하여서 Bit Reverse 방법이라고도 한다.
 I     174                                                3. DSSS와 Code이론
                                                                              1




                                          0   0   0   0   0   0   0       0
                         Ii   1   1   1   0   1   0   1   0   1   0       1
                          0   0   1   1   0   0   1   1   0   0   1       1




       I
                 1   1    1   1   0   0   0   1   1   0   0   1   1       0
                 0   1    0   1   0   1       0   0   0   1   1   1       1
             1   0   1    1   0   1   0   0   1   0   1   1   0   1   0
             1   1   0    0   1   1   0   0   0   1   1   1   1   0   0
                 1   0   1    0   0   1   0   1   1   0   1   0   0   1


             (a) OVSF'방식                          (b) Hadamard 방식

                     （그림 3-28) OVSF 와 Hadamard 방식의 비교



     3.8 Gold Code                                                            )

 다중접속 방식어］ 사용되기 위한 코드신호는 몇 가지의 특징이 있어야 한다. 우선
다른 신호와의 구별을 용이하게 하기 위해서 상관특성이 좋아야 한다. 상관특성이
좋다는 이야기는 그것의 상관특성이 극단적이어야 한다. 즉 같은 코드인 경우（여기
에서 같은 코드라는 것은 위상과 주파수를 모두 알고 있는 상태의 동기가 이루어진
코드를 말한다） 상관값이 최고 치로 아주 커아 하고, 그렇지 않은 경우에는 아주 작
은값, 즉 0에 가까운 값을 나타내는 양극화 현상이 두드러져야 한다는 것이다. 이런
측면에서 앞서 공부한 PN Code의 경우 아주 좋은 예라고 할 수 있다.
 그러나 PN C(넜e의 경우 주어진 코드 필드에서 생성될 수 있는 코드의 수가 극히
제한되어 있다. 이러한 것을 셀룰러에서 기지국 식별용 코 三로는 상당히 부족하다
고 할 수 있다. 사실 이것보다 더욱 중요한 것은 코드의 생성과정에서 문제라고 할
수 있다. 만약 기지국마다 서로 다른 코드를 사용하게 된다면 코드발생 선형필터의
종류도 그만큼 다양해야 하고 ASIC의 종류도 그만큼 다양해져야 한다. 이러한 이
유로 현재 QCDMA의 경우 동일한 코드를 발생하여 일정한 시간 옵셋으로 식별하
는 방식을 사용하고 있다．                                                        J
 어찌 되었튼 이러한 목적어］ 맞는 코드를, 즉 상관특성이 좋고 코드의 종류도 다양
한 코드를 Robert Gold 박사어］ 의해서 발견되었다．
    3. DSSS와 Code이론                                                              175
1


    이 코드는 2개의 독립적인 PN Code를 통해서 얻을 수 있는데 그것의 대략은 다
음의 그림과 같다. 그림에서 알 수 있듯이 서로 다른 원시 다항식어］ 의해서 생성되
는 최장 코드두개를 bit-by-bit modul-2연산을 통하여 새로운 코드를 만든다．


                       n-stage PN Generator
                               Pi(川
                                                          +

                               i
                                                      Bit-by-Bit
                                                                         G아d
           Clock                                      Modulo 그         >Code
                                                        Adder

                       n-stage PN Generator
                               P2似J
                                                          +
                             （그림 3-29) G이d Code의 발생



    여기에서 출력되는 코드의 길이는 2개의 PN Code와 길이가 같을 것이다. n단의
LSFR을 통해서 얻어지는 PN Code는 앞서 공부한데로 (2'- 1)이 된다. 따라서
Bit 대 Bit를 m硫네o-2연산 또한 (2 "- 1）번 행해지게 되고, 출력 시퀀스 또한
(2 "- 1）의 길이를 갖게 될 것이다．
    예를 들어서 n= 3인 경우어］ 2개의 PNC（넜e를 사용하여 （拍id Code를 생성
해 보자. 여기어］ 사용되는 PN Code의 생성 다항식（원시 다항식）은 각각
P1佃）＝尤3＋尤＋"            P2佃）＝尤3+ x2+ 1이다. 이런 경우에는 9개의 （拍id Code가 생
성될 수 있다．

    S1(0) = 0011101           Gi 亡 Si(0）由錢(1)                 Gi = Si(0)由Sz(4)
                                   = 00011101                      = 00011101
    S2(0) = 1110010           GI = S1(0)      S2(2)           GI = 針(0）田S2侮）
                                   = 00011101                      = 00011101
    Gi = S1(0)eS2(O)          GI = S1(0)      S2(3)           GI = S1(0)ES2(6)
       = 00011101                  = 00011101                      = 00011101


    이러한 Gold Code는 PN Code와 비교했을 때 그 코드의 종류（수）는 비교도 할
수 없을 정도로 많다. 앞서 공부한대로 식 仔27）로 PN Code의 수를 표시할 수 있
다. 크기가 n인 PN Code를 2개 곱해서 만들어지는 경우 그것의 필드는 才이 될 것
                                           3. DSSS와 Code이론



이며, 그러한 필드의 최장 코드의 경우 (22"_ 1）의 길이를 가지는 코드가 될 것이다．
그러나（拍Id（加e의 경우 그것의 크기가 (2" 1）의 코드이므로 최장 코드는 아니라
는 것을 확인할 수 있다. 또한 여기에서 우리는 이러한 필드어］ 존재하는 G아d Code
의 수를 확인할 수 있는데 그것은 전체 필드에서 코드의 길이를 나누면 몇 개의
（拍id Code가 존재하는 것인가를 확인할 수 있다．
 즉 （전체 필드의 크기）/(Gold Code의 길이）= (22n_ 1)/(2n_ 1) =(2n+1)이다．
따라서 G아d Code의 경우 Gold C넜e를 생성하는데 사용되는 하나의 PN Code의
길이（크기）보다 2개 더 많은 것이 된다. 예를 들어서, n단인 LFSR을 사용하는 경우
PN Code와 Gold Ccx扼의 수를 각각 계산해 보자．
 PN Code의 경우 식 侶-27）에 의해서 다음과 같이 구할 수 있다．
       砂（2" -1)＝中（210 H
                        1) =607下

 （拍ld Cc月e의 경우 2 "+ 1= 2'0+ 1= 1025개이다．
 우리는 이러한 예를 통해서 （拍ld C(넜e가 얼마나 많은 코드를 가질 수 있는 가를
확인할 수 있다． 이러한 Gold Ccx扼는 3GPP에서 기지국 식별용으로 사용을 하며，
다양한 코드의 종류로 인해서 각기 다른 코드 즉 코드 자체의 논리적인 구별이 가
능하므로 모든 시스템이 공통적인 기준 시각정보를 고유할 필요가 없게 퇸다. 따라
서 3GPP에서 제안하는 \VCDMA방식은 GPS 등과 갇은 정보가 필요 없으며, 따라
서 동기 시스템에 대해서 반대가 되는 비동기 시스템이라고 흔히 이야기한다. （丸ld
Code는 여기어］ 사용된다.
    4. CDMA Demodulator                    177
1




                          CDMA Demodulator




    예전어］ 모 방송사에서 이산 가족 찾기라는 프로그램을 방영한 적이 있었다. 수십
년 동안 떨어쪄 살아서 그들의 만남은 그야말로 만감이 교차하는 그것이었을 것이
다. 그런데 이 프로그램에서 이산가족을 찾기 위해서 가장 많이 사용된 방법들이 여］
전어］ 살던 집의 주소, 이름, 그리고 어렴풋한 기억들이었다. 이런 것들을 가지고 그
들은 그들 자신의 형제 자매인지를 결정하는 초기 단서가 되었음은 물론이다. 그러
나 막상 만나서 더 많은 정보를 확인하다 보니 내가 찾던 사람이 아니라는 결론이
나서 쓸쓸히 헤어지는 경우도 없지 않았다．
    그리고 최종적으로는 정말 자신의 혈육인지를 마지막으로 확인하기 위해서 유전
자 식별작업까지 하는 것을 우리는 보았다. 결국 이 모든 방법들의 공통점은 그들이
가지고 있는 정보의 일치성을 통해서 동질인지 아닌지를 확인하는 작업이었다. 우
리가 이 장에서 공부하게 될 CDMA 복조 역시 이러한 각각의 비교 정보들을 통해
서 최종적으로 동질의 신호인지를 찾아가는 작업을 하게 될 것이다．
   178                                4. CDMA Demodulator
                                                            1


 4.0 서론

 PN Code로 확산되어서 수신되는 신호를 찾아내는 과정, 즉 복조 과정을 위해서
는 수신된 신호와 Cohere毗한 국부신호를 찾아야만 한다. 이러한 과정은 대략적인
동기를 맞추는 획득（Acquisition) 과정과 PN부호의 계속적인 위상추적（Tracking)
과정으로 이루어진다．
 수신단은 PN 부호 위상획득 과정을 통하여 수신신호의 PN부호 위상어］ 대한 국
부 PN 부호의 위상을 1칩 이하의 오차로 동기를 맞추는 획득（Acquisit幻n) 작업을
하는데 이러한 동작을 하는 부분을 Se可cher라고 한다. Searcher어］ 의한 대략적인
수신신호의 PN 부호 위상정보를 바탕으로 시간적으로 변하는 수신신호어］ 대하여
PN 부호 추적루프롤 사용함으로서 칩 경계어］ 대하여 미세한 조정과 유지를 하여
계속적으로 동기를 유지하게 되는데 이 부분을 I往nger라고 한다．
 （그림 午1）은 DSSS에서 쓰이는 전형적인 PN Code 동기화이다. 코드 획득 시간
어］ 획득장치는 수신 PN Code와 국부발생 PN Code가 정렬되도록 계속하여 국부발
생 코드의 위상을 조정하여 코드 위상오차 可t)가 허용범위 내에 오도록 한다. 코드
위상오차는 수신코드와 국부 발생코드의 위상차이다. 추적루프어］ 대해서 허용범위




              , PN 코毖
              Generator




    （그림 4-1) DSSS 시스템에서 쓰이는 PN Code 동기장치의 일반적인 형태
    4. CDMA Demodulator                                                        179
.


는 통상 코드 추적의 특성지표가 될 수 있는 것이다. 코드 위상오차가 허용범위 안
어］ 있게 되면 L叱k 검출기는 동기장치가 In-I玭k 상태가 됨을 인지하고 칩의 미세
조정을 위해서 획득장치에서 추적장치로 기능을 넘기게 퇸다．
    추적과정에서 채널의 유동성 및 잡음에 의하여 코드 위상오차가 허용범위를 초과
하게 되면 동기장치는 out-寸Lock될 수도 있다. 이 경우 I乂兀k검출기는 재획득 과
정으로 돌아가며, PN Code 동기장치를 코드 획득장치로 되돌아가게 한다．
    기지국（혹은 단말기）의 송신신호는 채널을 통과하면서 반사 굴절 등 여러 가지
채널 환경요인으로 인해서 변질되게 된다. 만약 수신단에서 수신된 다중경로 신호
성분 중에서 특정한 경로의 신호성분만을 추적하여 데이터를 복원할 경우 다른 신
호는 간섭신호로 작용하게 되어 수신성능의 저하를 초래할 수 있다. 이러한 이유로
수신단에서는 수신된 모튼 다중경로 신호성분들을 최종 데이터 복원어］ 사용하는데,
이러한 수신기를 Rake 수신기라고 한다. 이러한 Rake 수신기는 심벌 결합기, 주파
수 오차 결합기 등을 포함하고 있다.
    즉 Searcher에서 탐색된 모든 다중경로 성분의 신호들은 기본척인 획득오차의
범위 안어］ 들어오면, Lock 검출기에 의해서 각각의 Fir垠er의 추적루프로 넘겨 주어
서 계속적으로 추적（Tracking）하여 복조퇸다. 이러한 데이터들은 Rake 수신기를



                                                    Combining
                 Demodulating Finger 3                   브 己J
            미＋
                      Demodulating Finger 2
                 >                                   Symb｛月       Svnc80M
                       Demodulating Finger 1        Combiner
                  >

                                                   Frequency
                                                     Err｛才        TRK LO ADJ
                                                   Combiner
                            Searcher Engine

                                                  Power Control
                       1 1rnr尸口a 11HI \;
                                                      Unit
                         ,nn
                       口叩砧가 인가됨


         CHIPx8 - -.             --
              十 Microprocessor 由 Master ,      > EPOCH
                      Control Unit




                 （그림 午2) MSM Demodulating Function계 텨ock 미agram
   'P1)                                                   4. CDMA Demodulator
                                                                                .


통하여 결합되고, 주파수오류를 최종적으로 정정하여서 다중경로 성분의 신호를 복
원할 수 있다．
 여기에서 이야기되는 내용은 IS-95에서 사용된 기술을 중심으로 이야기하겠다．



 4.1 Searcher Engine

 대역확산된 신호로부터 원래의 정보신호를 추출（복조）하는 과정에서 정확한 동기
를 획득하는 것은 시스템의 용량 및 서비스 품질에 영향을 미치는 중요한 요소이다．
수신기에서 복조를 수행하기 위해서 송신기에서 사용하여 전송된 PN Code의 위상
을 획득하는 작업이 선행되어야 하는더T이러한 작업이 초기동기 획득작업이다．
 Searcher에서는 수신퇸 PN Code를 1/2칩 이내로 맞추는 작업을 수행하게 되는
더］, 일반적으로 확산을 위해 사용되는 파형은 광대역인 것이 상식이다. 때문에 확산
파형의 주기는 길고 대역폭 또한 넓으므로 위상 및 주파수 동기가 쉽지 않다. 이러
한 수신코드 위상을 획득하는 과정에서 Fading 채널환경에서 수신신호의 위상이
계속 변화하고 있기 때문어］ 신호의 위상정보와는 무관하게 동기 획득 과정을 하는，
즉 비동기 획득 과정을 수행해야 한다. 또한 동기 획득 이후 다중경로릅통하여 수
신되는 신호로부터 다중경로 탐색으로 인한 각 경로어］ 대한 에너지 값과 PN Code
위상을 프로세서어］ 보고하여 복조시 분리하여 복조 과정을 수행할 수 있도록 해야
한다. 여기서 Slew는 PN C月e의 위상을 지연 또는 전진시키는 기능을 말한다.
 초기동기를 위해서 널리 사용되는 방법은 동기가 이루어질 때까지 부호의 모튼
위상과 주파수를 순차적으로 탐색하는 것이다. 각각의 국부위상과 주파수는 수신된




                                                      V




                                 "a
                                        今＋   計              )+：咎         "'
                                                                   no
                                                 'a
          PN 코드r
                    Search Next Phase
           발 생 '1



                （그림 午3) Double Dwell PN 동기 획득 시스템
    4. CDMA Demodulator                                181
1


신호를 역확산함으로써 평가되어진다. 만일 추적된 부호의 위상과 주파수가 옳다면
역확산이 이루어지며 이를 감지하게 된다. 만일 부호의 위상이나 주파수가 정확하
지 않다면 수신된 신호의 역확산은 일어나지 않을 것이며, 국부파형은 새로운 위상
및 주파수어］ 대해서 평가되어질 것이다. 이러한 기법을 지금 현재 널리 사용되고 있
는 직렬탐색이라 한다．
    또한 이러한 직렬탐색은 Single Dwell과 Do的leDw네이 있으며, 여기에서는 현
재 CDMA에서 사용하고 있는 Double Dwell어］ 대해서 이야기한다．

     4.1.1 PN Code

    PN Code는 3장에서 공부한대로 Linear Feedback Shift Register 등과 같은 시
간지연 요소들의 선형조합으로 이루어진 선형필터를 통해서 생성된다. 이러한 PN
Code는 각각의 기지국을 식별하기 위해서 코드를 생성할 때 초기값을 다르게 하여
코드를 생성한다. 즉 갇은 형태의 선형필터에서 나온 코드가 각각 옵셋만을 달리하
여 마치 다른 코드와 같이 사용되는 형태이다. 이러한 방식을 사용함으로 인해서 이
장어꺼 공부한 동기 획득 과정은 이러한 특징을 이용하여 수행된다．
    IS-95의 경우 1.2288八n七로 확산이 이루어지며, 따라서 PN Code의 1칩의 발생
시간은 1/1,2288八IHz = 813.802ns이다. 또한 15개의 지연 tap을 사용하는 PN
Short Code의 경우 1 PN Roll은 26.67ms이고 이것은 32,768칩이다．
    PN C(月e의 옵셋은 64칩을 하나의 Index로 설정하여서 최소한 64칩의 차이가 나
는 코드를 사용하게 하였다. 이것은 전파상의 지연으로 인해서 코드식별의 애매함
을 극복하기 위한 것이다．

     4.1.2 Dwell Algorithm

    각 Phase(PN 옵셋）에 대한 alignment를 체크하기 위해서 T必］간 동안 적분을
한다． 이때 계산된 에너지（El）을 첫 번째 Threshold(Thi, Early Thresh이d)와 비
교한다. Ei 1 T뇨보다 작을 경우 Searcher는 다음 hypothesis로 옮겨간다. 만약 Ei
이 Th1보다 크다면 T刃｝지 적분구간을 확장한 다음 다시 2번째 Threshold (Th2,
I如eli Threshold)와 비교한다. 여기서 E2값을 계산하는 방법을 생각할 때 Ei값어］
계속해서 더하는 방법을 생각할 수 있고, 다른 하나는 지금까지 계산한 E1값을 무시
하고 E2값을 새로 계산하는 방법을 생각할 수 있다. 만약 珌가 T比보다 작다면 역
   182                                              4. CDMA Demodulator
                                                                          .


         Energy                                     Next hypothesis




                                                    Accept hypothesis
                  Ti             T2

                   （그림 午4) Double Dwell Algorithm


시 이 경우에도 다음 hypothesis로 옮겨간다．
 이러한 Do曲e Dwell Algori小m의 장점은 획득 시간을 줄이는 것이다. Single
Step 시gorithm과 비교할 때 적분시간은 Ti<T<T卄끄（여기에서 T는 Single
Step에서의 적분시간）이지만, 대부분의 가 First Step에서 False Alarm을 갖기 때
문어］ 전체 /\cquisition tin妃을 비교할 때 많은 시간을 줄일 수 있다. 즉 " 될성 부른
나무는 떡잎부터 알아본다"는 속담어꺼 힌트를 얻은 방식이라고 생각할 수 있다．

   4.1.3 Searcher의 동작

 1) Searcher는 다음의 Block I万agram과 같이 구성되며, Searcher의 필요한 기
   능들을 S/W와 H!＼刀어］ 나뉘어서 구동되게 되었다. 여기어］서 H小刀라고 함은
   ASIC 칩小4SM : 八'I야皿e Station 八4odem)을 말하는 것이다．
 2) 초기어］ 入4icroprocessor는 다음의 값들을 읽어 들인다．
   木 SEARCHJNTERGRATETIME : 각각의 코드위상（Search Hypothesis)
    마다 몇 개의 칩을 적분할 것인지를 설정
   水 SEAR아
         ［ACC PASSES : 각 코드위상에서 몇 번의 Coherent 적분을 행
    할 것인지를 결정하는 값
   半 EARLYTHRESHOLD_Tllv1E: Early Dump Check를 수행하기 전까지
    몇 개의 칩을 적분할 것인지를 나타내는 값임
   米 SEARCH公U入'1 : SEARCHDON且爪TERRUFT를 발생하기 전까지 검
    색할 코드위상의 수로 Search V丙ndow의 크기와 관련됨
1
     4. COMA Demodulator
                                                                                                   1
                                                                                                          183
                                                                                                                    I
       * EARLYTHRESHOLDHENERGY : EARLY1THRESHOLD1TllV1E 서
           의 임계 에너지 값．
       永 SEARCH_SLEW : 탐색을 시작하기 전에 (+/                                        X）를 load한다. 여기서 x는
          advance/retard할 칩의 개수를 나타내며, 이것의 Resolution은 1/8칩이다．
          즉 士 16,384CF표P x 8Clock이다．


                                    EARLY_THE TIME
                                                         Compare


                                    SRCH_INTER_TIME

                                                                               EARLY THRENO



                                                                                    1
                                            Counter


                                                                                  弓oergy
                                                                                  Compare
                         Offnet
    BINARY OFFSET                             Counter
                        omparator




    5CC PS I MASK       I_PN_GEN




    乳H批요MASK        니   且PN SEN
                                                                                        ACC PASS
                                                                                                       川（, ENERGY
                                                                                                       COMPARE

     SLEW VALUE          Rtewtng       -*   Delay



                        Pontttun
    SCH. POSITION   4
                        CountIng                                                                                    小


                                               위상 日 가 존재            loden
                                                                               >SCH_MAXINDEX
                                               하는 Coherent         Co山ollng
                                               Integration
                                                                      V

                                                    SEARCH
                                                        NUM 늬 蜘나H馳ARCHDONE

                                        （그림 小5) Searcher Engine


    3) Searcher는 모든 Counter, Accumul毗or, Contr아 I力gic을 Reset 한다．
    4) Searcher Engine은 PN Code 발생기와 연결된 adviret line을 제어하고
        Slew Number만큼 코드위상을 이동시키는 동안 모든 Counter를 reset으로
        유지시킨다．
    5) Searcher Engine은 적분을 시작한다．
    6) Integration Counter가 EARLY1THRESHOLI工TII\侄과 같은 시점이 되면，
        (j2 + 寸） Engine을 구동하여 에너지를 구한다. 일반적으로 위상이 다른 두 신
      184                                                                                 4. CDMA Demodulator
                                                                                                                .


      신호의 합을 구한 결과 역시 그것의 크기와 위상이 같이 표현되어야 한다. 이
      적분에서는 크기만을 구함으로 위상이 배제된 값이 될 것이며, 이것은 각각을
      제곱하여 더한 후 구하게 된다. 이때도 적분은 계속된다．


                                           Register 초기 화

      SEARCH_PNJIQ
          MASK
                         PN 코드            PN 코드 역 확산
      SEARCH什B八ARY
          OFFSET
                                                       Y
      SEARCI [POSITION                             Gain                                     CTL



       SEARCI1_SLWE      Slew 계산                  l차 적분                                SEARCH_NUM

                                                                                   EARLY_THRESHOLD_TIME
                                        ．尸戶d戶4＝   戶＝
                                                       ；느1b1m
                                                                     '
                                                                         뇨뇨．




                                                  12 + Q2                      J



    人 OC
           는는기제후
Oa2
  ＝亡
                         Index 중가                                                  EARLY_THRESHOLD中ENERGY
           되기하 尸
m있L샹하斗餉    려크제挻한
           n 三和각仁
           nm의t각 ［
위두위위곱구
                                                  2차 적분                                SEARCI-LNUM



                                    0     //<
                                                   1      \
                                                       > 砂二／샤1
                                                                느＞             1
                                                                                   SEARCHJNTEGRATE_TIME


                                                                                     SE／났之CH小ACC PASS

                                                       T                            SEARCH_MAXJNDEX




                                           Max Energy계산


                           （그림 4-6) Searcher 동작 흐름도


7) Searcher Engine은 이 값을 EARLY_THRESHOLD1ENERGY와 비교한다．
8) Searcher Engine은 Early-Late Tin肥에서의 측정값의 결과치와 임계값을 비
      교하여 측정치가 EARLYTHRESHOLI工ENERGY보다 작으면 Step 11로
      간다．
9) Searcher Engine은 SEARCH日THRESHOLD中TIME 칩만큼 적분을 계속하
      고 SEARCH－丁HRESHOLD_TIME어］서 Accumul砒아의 출력을 latch하고
    4. CDMA Demodulator
.


       (12 + Q2 )Operation을 시작한다．
    10) Searcher Engine은 Integration Counter와 Accumu1ator를 Reset한다.
    11) Searcher Engine은 (12+ 寸）를 취하고, 에너지와 Index를Microprocessor
       로 보내기 위해 DMA engine을 구동한다．
    12) Searcher Engine은 Coherent하게 더하고, SEARCH_ACC_I次SSES가 1보
       다 크다면 Step 4번으로 천이한다．
    13) Sweep Index Nu끄riber를 전진시켜서 최대 에너지와 최근 에너지를 비교하고
       Index를 갱신한다．
    14) 만약 Sweep Counter가 SEAR아1_NUM보다 작다면, Step 5번으로 간다．
    15) 한 Window의 Sweep이 끝났음을 D曲rip Done Interi끄I光 신호를 Micr아兀O-
       cessor어］ 알리고 Status I九mp Information을 Latch한다．
    16) 八小cropr（兀essor는 최대 에너지와 최대 Index를 읽는다．
    17) 처음으로 간다．

      4.1. 4 주요 기능


    Early-Late Correlation

    이 장에서 이야기할 동기 획득 시스템과 동기 추적 시스템은 Early小Late
Correlation을 통하써 그것의 기능을 수행한다. 이러한 생각은 알지 못하는 수신파
형의 위상정보를 찾아내는 과정에서 가장 기본이 되는 것이 확산 코드인 PN Code
의 ／뇨to-Correlation특성을 가지고 하는 것이다. 앞서 3장에서 이야기하였듯이 PN
（沁de는 자기 자신과 위상지연이 동일한 경우의 코드와는 상당히 우수한 자기상관
(Auto＜二咐elation) 특성을 가진다. 반면, 어긋난 위상의 코드와는 거의 상관성이
없는 것으로 나타나거］ 되는데, 이러한 코드의 특성을 이용하여 위상지연 성분을 찾
는 것이 가장 올바른 방법이다．

    Coherent Integration
    이 적분은 수신된 신호에서 위상 0 가 존재하는, 즉 VQ채널간어］ 구별이 되는 상
태에서의 에너지 축적을 한다. 이러한 이유로 에너지의 축적은 1/Q채널별로 각각
이루어지게 된다. 동기 획득 시스템에서 Coherent 적분을 수행하는 것은 입력신호
                                         4. CDMA Demodulator
                                                               .


가 I 채널과 Q채널로 나뉘어서 들어오기 때문이며, 이러한 신호들을 구별해서 처리
해 주어야 하기 때문이다．


 Non-Coherent Integration

 이 적분은 Early Di叩liP 시간 이후어］ Enable되며, Non-Coherent 적분을 통하여
지금 입력되고 있는 PN （뇨le의 에너지 값만을 확인한다. 물론 신호가 완벽하게
Coherent detection이 되기 위해서는 주파수 오차도 고려되어야 하나 여기에서는
그러한 주파수 오류는 다음 단 （나중에 이야기될 Fir培er와 Combiner）의 처리로 미
루어진다．
 어찌되었든 여기에서의 관심은 입력되는 PN C(넜e와 수신기에서 추정되어서 만
들어진 국부 PN Code간의 에너지 상관성에만 관심이 있고, 이러한 기능을 충실히
수행하기 위해서 주파수성분이 배제된 Non-Coherent Integration이 사용된다．


 Non-Coherent Energy Detector

 주파수 에러로 인해서 Pilot 에너지 검출시어］ 감쇄가 발생되는 것을 줄이기 위해
서 （그림 午7）과 같은 형태의 Non-Coherent Detect아를 사용한다. R刃와 RXQ는
Sinusoidal 신호로 신호어］ 교류성분이 살아 있는 신호이며, 이러한 和斗수는 칩
rate의 8배, 즉 9.8304入'IHz(8x 1.2288 MH기이다. 이러한 RXI와 RXQ는 역확산을
위해서 ONJime과 LATE 1 Time어］ latched퇸다.
 각각의 latched time은 칩 rate와 같은 주파수로 동작된다. RXT와 RXQ는 주파수
에러를 가질 것이며, 다음의 방정식어］ 의해서 표현퇸다．

                         , sinG
       RXI =Aa/, cos9+ Aa0                               (4-1)


                           , cosO
       RXQ = -Aa/, sinG +Aa0                            (4- 2)

 식 (4-1), 식 (4-기의 sinG항은 주파수 에러에 의해서 추가된 항들이다. 즉 sinG
로 인해서 원래 신호인 cos 0항이 tan六 口, Q/ a, /）만큼의 위상차이가 생기기 때
문이다．
    4. CDMA Demodulator                                                          187
U


        RXI -                     Ii唯h
                 4-bit register       MUX             I       1小
                                                              III LVg14 I.IULI


                이k                low
                                                          >    & ＄解are
                                         seli乂




        RXQ                       hi日h
                 4-bit register       MUX
     ON_ time1+
             -  clk               low
     LATE time                           selec


         PN_I                                    , !PN I과PNQ이 같지 않을
                                                     때 MUX의 h坦h가 출력되
        PN_Q                                       : 어 RXI가 exclusive-OR
                                                     표ate어］ 인가됨．
                                  >

                      （그림 小7) Non Coherent Energy D아ec的n




    4.2 Sear아｝er B伯ck 별 기능                                                             1
 이 절에서는 실제 사용되고 있는 Qualcomm의 고속 동기 획득기의 경우로 Block
별 기능을 확인해 보자．
 Searcher의 레지스터는 기능별로 크게 탐색과 적분을 수행하는 Search 미ock 과
Search Block 의 계산결과를 근거로 에너지값과 최대1 에너지값을 검사하여 동기가
획득되었는지를 판단하여 획득 여부를 판단하는 ACQCHK과 이러한 처리를 위해
서 수행되어야 할 전반적인 동작과 제어신호를 생성하여 제어하는 INC 미ock 으로
나뉘어진다．
 Searcher를 제어하는 레지스터는 다음과 같다．
 SEAR아LCTL레지스터는 크거］ 두 가지의 제어명령으로 구성되어 있다. 첫 번째
명령인 SEARCHER_GAll나 (DATA[1:0]）은 ONPN칩과 LATE PN칩의 역확산
과정에서 계산된 상관 에너지값을 증폭하는 레벨을 지정한다. 이 값이 '00'이면 1,
'01'이면 2, 그리고 '10' 이면 4, '11'이면 8배 증폭하게 된다. 그리고 DMAH
CTL(DATA[2]) 명령은 [兀TA를 통하여 데이터 전송시 DMA의 요구시점 및 전송
데이터의 종류를 지정한다. 만약 이 Bit가 '1'이면 모든 탐색 옵셋어］ 대하여 전송이
요구되고, '0'이면 1차 경계값을 통과한 옵셋의 에너지만을 전송한다．
I     1db                                 4. CDMA Demodulator
                                                                .


    SEARCHNI瓜4 레지스터는 Searcher의 On time과 Late time어］ 대하여 상관도
를 구할 코드의 범위를 지정한다. 하위 iBit는 0으로 초기화되고, 상위 7개의 Bit만
이용하여 탐색구간을 정의하게 된다．
    SEARCH_ACC_PASSES레지스터는 제곱기 출력의 비동기 결합 횟수를 지정한
다. 즉 이는 적분기 II의 적분구간을 SEARCHJNTEGRATE1TIME X (SEARCH
ACC_PASSES + 1）로 지정하는 것이다. 이 레지스터는 DATA 버스의 하위 3Bit
만을 이용하고 있다．
    SEARCH소/IA)LENERGY레지스터는 정해진 Window size내에서 계산된 최대
에너지값을 검출하여 프로세서의 제어에 의하여 최대 에너지값을 출력하는 레지스
터이다．
    SEARCH小4AXJNIJEX는 Search 모드에서 최대 에너지값을 나타내는 코드위
상을 1/8칩 단위로 표시한다. 이 레지스터는 小2040까지 표시한다．
 DMADATA는 Searcher의 에너지값을 DMA 요구 이후 하나의 RD/ 신호어］
따라 먼저 ON time 상관 에너지값을 출력하고, 다음으로 LATE time에너지를 출
력한 후 마지막을 PN Code의 Index를 출력하게 된다．
    SEARCH코II沮RY_OFFSET은 기지국의 코드위상 옵셋을 지정하는데 사용하
며 동기채널을 수신한 후 옵셋 값을 알아낸다．
    SEARCH_PNJ小'JASK와 SEAR아［PNQ소flASK는 단말기 자체 PN 생성기
의 코드 위상을 변동하기 위한 데이터로 각각 3개의 Address중에서 가장 상위 Bit
Address가 가장 나중어］ 들어와야 한다．
    SEARCH卜SLEW는 Searcher가 지정된 위치로 \Tin如w를 이동시키는 양을 1/8
칩 단위로 표시한다. Search를 시작하기 위해서는 어떠한 값이튼 꼭 기록되어져야
하고, 하위 3Bit는 0으로 재초기화되어 1칩 단위로 Slew가 수행된다. 입력되는 더］
이터는 반드시 상위 Byte가 가장 마지막으로 들어와야 한다．
    SEARCHPOSITION는 \Win面w내어］ Searching을 할 때 PN Code의 0 옵셋을
기준으로 절대위치를 가리키며 1/8칩 단위이다.
 EARLYTHRESHOLDENERGY는 Window 내어］ 서 계산된 에너지값이 최소
임계치 보다 큰가를 비교하기 위하여 미리 설정한 값이다. 이 값은 적분기 I의 첫
번째 적분구간어］ 대하여 적용한다．
    SEARCHJNTEGRATETIIVIE는 Searching시 적분구간을 나타내며, 32-1020
    4. CDMA Demodulator
.


칩까지 지정하며， 小FF값으로 write하여 내부에서는 4배를 곱하여 사용한다．
    EARLYTHRESHOLI工TIME는 적분기 I에서 정해진 Window 사이즈 내에서
처음 적분구간을 나타내며, Searcher내부의 Threshold값과 비교한다. 범위는 16-
(SEARCH_끄나TEGRATE－丁I八'IE X 4 - 8)PN 칩으로 정의한다．


     4.2.1 SEARCH Bl以：k

    Search Block 은 수신신호와 자체 발생된 PN Code와의 상관도를 계산하고, 이
를 Thresh아d time 동안 누적하고 에너지를 구하는 부분이다. 전체 Block
Diagram는 （그림 午8）과 같다．




                                                         D. OUT



                                                        二二：
                                                         CLR




                                                                  NCO_TRKt2:OJ




                          （그림 4-8) Search 테ock 미agram


    이 미ock 에서는 가장 먼저 무선부에서 기저대역으로 down conversion된 후 기
저대역 아날로그 Block 의 A/D변환기에서 Chip x 8로 Over Sari叩ling되어 수신되
는 신호를 칩 rate으로 8:1로 Decimation하는 기능을 수행한다. 8배로 Over
Sampling된 신호어］ 대해서 On Tm肥과 Late Time 각각어］ 대해서 8:1로
Decimation하기 때문에 Maximum T油e Tracking Error는 /16 PN이 된다. 그리
고 Decimator어］ 인가되는 1.2288M1初 Clock은 Pilot PN 생성기와 동일한 텨ock
   190                                              4. CDMA Demodulator
                                                                          .


을 사용하여 신호를 인가한다．
 다음으로 칩 속도（CI丑n와 같은 빠르기로 표본화 된 입력 신호들과 국부 발생된
PN 부호와 상관도를 상관기 B1兀k 에서 계산하게 되고 이 졔산치를 누적기에서 누
적하게 된다. 누적기는 제어미ock 에서 발생되는 ACC_CLR 신호에 의해서 Clear
된다．
 따라서 ACC_CLR의 발생은 새롭게 적분이 시작됨을 의미하므로 이 신호의 발생
시점은 1차 및 2차 적분구간을 의미한다. 누적된 데이터를 제곱기어］ 입력 Bit인 8
Bit로 제한하기 위하여 CTL Block 을 사용하였으며, 제곱기에서 각 채널 누적값의
크기를 구하기 위해서 제곱하여 합함으로서 에너지를 구하게 된다. 제곱된 이 데이
터는 비동기 결합 횟수만큼 다시 누적된 후 다음 Block 인 ACQCHK 미ock 의
입력된다. 비동기 결합 횟수는 1차 동기 획득이 되었을 때에만 의미가 있다. 따라서
NCTRK Block 에서는 1차 동기검출이 발생될 때까지 누적을 수행하지 않고 입력
되는 에너지값을 출력으로 내보내게 된다．

 PN Code 발생기

                                              UNMASK PN

                          듣：
                           二                                     1

         DATA[7:O]                            MASK PNJ

      WRE 1C.1E.2O]



           CHIPX1                             UNMASK PN

                          :：二
                                                                 Q

                                              MMASK PN
                                                ASKPN5
      WR[22,24,261




                                        카운터 ／비
                                         교기
      WR[32.34.361
                                       'CLK
                                              CLK

          RECLRB


                      （그림 4-9) PN Code 발생기
    4. CDMA Demodulator
口


 이 B1乂k 은 역확산할 PN Code를 발생하고 그것의 위상을 조정하는 기능을 한
다． 따라서 크게는 Slew, Zero Insertion, 八4asking 등의 기능을 수행한다．
 단말기의 PN Code 발생기는 기지국과 동일한 생성 다항식을 사용하여
1.2288八4cps의 속도로 PN Code의 LQ톄이터를 생성한다. 발생되는 PN Code는 전
체 주기를 사용하지 않고 앞의 20m sec만을 사용한다. 따라서 20msec마다 Seed를
초기화하는 동작을 수행하며, 이렇게 됨으로 생성되는 PN Code는 언제나 뒤쪽의
O.667msec 부분은 나타나지 않는다. 즉 약 8191 칩이 빠진다．
 발생되는 PN Code는 INC 미ock 에서 생성되어지는 신호 CHIPX1 Clock어］ 의
하1 발생되는 위상이 제어되도록 하였으며, 20ms마다 발생되는 동기신호를 생성하
기 위해 내부에 PN Code 발생과 동기된 동일한 Clock을 이용하여 카운트되는 카
운터가 내장되어 있다．
 또한 이 B1乂k 은 PN 마스크를 이용하여 PN Code의 위상을 64칩 단위로 이동
할 수 있도록 구현되어 있다. 이는 호출채널과 Forw可d 통화채널의 복조시 인접 셀
의 P표毗을 탐색하는 경우 Slew동작을 수행하는데 걸리는 시간을 줄이기 위하여
Cic兀k을 이용하지 않고 PN 부호의 Sh玭and-Add특성울 이용하여 Slew동작을
수행하기 위한 것이다． 이 PN 마스크를 이용하여 64칩 단위의 Slew 동작을 수행
하는 경우에는 Hold 할 필요가 없다．



             LC_I
           凡d13:O]
                                               CI[4:O]
            LC_Q
          RxQ[3:O]




                                              CQ[4:OI




                          （그림 午］0) 상관기

 상관기에서는 수신된 PN Code 신호와 국부 PN발생기에서 발생된 I채널 및 Q
                                                                                         4. CDMA Demodulator
                                                                                                               .


채널의 신호와의 상콴도를 계산하는 Block으로 계산식은 다음과 같다．
        Corr, = Rx1 ' LC, + RXQ ' LCQ
        CorrQ = RxQ ' LC, + Rx, ' LCQ

 위와 같은 식을 이용하여 상관도를 계산하여 각 채널에서 발생하는 Cross Talk
를 제거하게 되다．

 CTRK 미ock

 상관기의 출력을 제곱기의 입력 Bit수인 8 Bit로 한정하기 위한 Block 으로 먼저
데이터를 uns塘ned형으로 변환하고 하위 5 Bit를 절삭하게 된다． 이를 구성하기 위
한 Block Diagram는 다음과 갇다．


     引［14]                                                                 MAGJ[7:0]
                             U1112:01                      Al가）           MAG_Q]7：이
     SI[ 12'OI          /
                       13
                               n0卄                            SUM          MAGJ(8'I]
                                                  B                       MAG_Q[9:21
                                           ,/,>                     l
                            S1114]                                                                 MIE7tO]
                                                  Cm                       MAGJ[9'2]
                                                                          MAG_


     SQII4J      \                                                       MAGJLIO召1
                            UQ[ 12:01                      ADD           MAG_QI 10:3I1
     SQ112:0i                                                                                      MQ[7:OJ
                       13
                                                              Si-月.1 1MAGJ[      1C4]
                 I
                                     mm＝   中＞ B                          MAG_Q ( 1
                         SQ[ 14] l3
                                                       n                 MAGJI1C5)
                                                                         MAG_Q[ 12:51r




                                       （그림 午］1) CT日K 블록


   4.2.2 ACQ_CHK Block

 1차 및 2차 적분기의 상관값을 에너지값으로 변환하여 동기 획득 여부를 검사하
는 Block 으로 동기 획득 과정에서 동기 획득어］ 소요되는 시간을 줄이고 정확한 동
기 획득을 위하여 이중 적분직렬 방식을 사용한다. 즉 동기 유무를 판단하가 위한
1차 적분 시간 동안 PN상관을 수행한 다음 상콴값과 기준값을 비교하게 퇸다．
 이 과정에서 상관값이 기준값보다 작으면 PN Code 발생기의 위상을 1/2 칩
Slew한 다음 다시 1차 적분시간 동안 상관값의 적분 작업을 수행하는 위의 동작을
1차 동기가 획득될 때까지 반복한다. 1차 동기 획득이 이루어지면 보다 정확한 동기
    4. CDMA Demodulator                                                                                           193
1


유무를 판단하기 위해서 상당히 긴 2차 적분 시간 동안 상관값의 적분을 수행한다．
동기 획득에 소요되는 시간을 줄이기 위해 1차 적분 시간을 짧게 설정하였기 때문
어］ 오보확률（False Alarm)이 크다. 따라서 1차 동기가 선언되면 PN Code어］ 대해
서 Slew를 수행하지 않고 긴 적분 시간 동안 상콴을 수행하여 1차 동기의 오보 유
무를 확인하는 것이다. 2차 적분에 대해서도 동기가 선언되면 동기 획득이 이루어
졌다고 판단하고， 동기가 선언되지 않았으면 1차 동기를 오보로 판정하고 다시 1차
적분 및 비교를 수행한다．

                                                                                                       ME115:0]

                                                                               ]   a   a

                                                                                   >   Q
                                                                 CMP
                                                                                                 MAX
                          GEThMAX 1七＋ A                 QH   A   A>B.>Il

                                                                           Q
         0"上［' " 『"누，步；                        >        a
         LT,..Etl5:0L.言. B
                             A)B=>H   나＞   >                                               0_   I.
                                                                 CMP

              DATA[7:O]                                          A>B=>H                          AC0
                                               1)       a    B
                  싸ROS
                                               >
                  WROA
                                                   dr
                                                   A
                 MRTRG
                ACQTRG
                RESETE
                RECLRB

                               （그림 午］외 AGO CHK 텨ock 미agram


 （그림 士12）는 ACQ小CI표（ 미ock을 나타낸다. ACQ_TRG및 METRG는 INC
미ock 에서 발생되는 제어신호이다. ACQ－丁RG신호는 적분 시간 동안 카운트하여
동기 획득을 검사할 시점에서 발생되는 트리거이고 METRG신호는 1차 적분 결과
동기 획득이 확인퇸 상태에서 2차 적분 시간 통안 카운트되어 발생되는 트리거이다．

     4.2.3 INC 블록

    INC 블록에서는 각각의 프로세스와 연동되어 동작하는 각종 레지스터를 가지고
있으며 1呱4A데이터를 전송하기 위한 동작을 수행하게 된다. 그리고 SEA兀H
Block 이나 ACQ_CHK Block 에서 필요로 하는 트리거와 신호를 발생하는 역할을
한다. 또한 자체 PN Code의 위상을 계산하는 부분을 포함하고 있다．
                                                                                      4. CDMA Demodulator
                                                                                                                    U


                               尸．b   WR[02,04,08,OA,]0112,1
                               I -   毛l6『l8.lJ＼·！C,l匕，2U.ZZ·          S.D(가寸E, SDRQST, ACC_CU떠
                               1     24,26,D8,2AJ                     ACQTRGJAE_TRG, ACC_TRG
                                                                      CO_TRK[2:0], NCO_T] K[2:0[
                                      Ha卜 RECLRB
    ADD [7:0]
                            WAD                                        CHIPXB
                                                                       'I丁1日q늬U
                                             ADD (7:0]
                                                                                                           CHIPX1
     csB        S
                                               ACQ

     MRB                                 WRL0立凹， （乂.0                      31冬B
             S
                                         且2C.2E.30]                       PS_I寸S
                                                                                                           CHIPX8
     WRB                                                                  SLEWB




                            RAD
                                        RE(02,2022,24,26,
                                        28.2A.2C.2E]
                                                            >



       RDB



                                     （그림 4너3) INC 텨ock 미agram



 이 Block은 입력되는 Ad血ess bus를 복호하는 Block 과 Thresh아d Time과 PN
Code의 Index 그리고 ji.끄nping Slew를 제어하는 부분이 포함된 SLEW 미ock,
I孤4)＼어］ 관련된 작업을 수행하는 [呱4A中RE Block 과 마지막으로 안정된 칩 Clock
을 발생시키는 八4CS Bl以k으로 구성되어있다．


       미ock
                                                                           T枷伉_CMP
                                                                        DATA          ME그'RD 十기 M且TRG
                                                                        CI-)伊자i      ACQTRG -ACQ_      TRG
                                                                        SOS可ro         SLOWS -     SLEWB
                                                                        EPOCHB      CM只340M5 -CMPJ놔UMB
                                                                        10.13)水00    ACC_TRG     -ACC TRU
                                                               ACQ      ACQ           CO_TRE -      CO_TRK
                                 CTL_JS             WRA [04，此1兀，0R)     텍RA[ 41      NCO_TRK ------ NCO_TRK
                                                                                    ACC_CLRB 1Hm ACC_CLRB

      DATA[7:0I 11 DATA
        아IIPXF p   CHLPX卜
                            RESETB      마SLEW                                                      1冬_NS
        RESETS
       EPOCHB            + EPOCHB        JS_DONE
      WRA[2c,2e,30   m    + W兌AL3)
                                                                             G_INDEX 3
                                                                            XE
                                                                            TB




                                                                           ，칡 쁘巴自’                 "" "" ""

                                          （그림 午］4) SLEW 블록도
     4. COMA Demodu'ator                                              i0 5
.


    전체 3개의 Block으로 구성되어 동기 획득 시스템에서 필요로 하는 각종 신호를
생성하는 부분이다. TIJVIEeCMP Bi以k은 동기 탐색 동작시 탐색 Window의 크기
를 제어하고 1차 및 2차 적분 시간어］ ACQ아끄（ Block에서 사용되는 트리거
(ACQ_ TRG, ME_TRG）를 발생시킨다. 이 트리거들은 Chip x 8 Clock을 카운트
한 값과 Threshold time과 비교하여 신호를 생성한다. 그리고 G皿寸DEX Blo比은
PN Code의 Index및 Position을 계산하여 출력한다. 마지막으로 CTLJS 미ock은
Jumping Slew를 제어하는 부분으로 Jumping Slew동안 MCS Block 의 입력으로
사용되는 ST冬B신호를 '0'으로 유지하여 Ji.그
                          ［mping Slew 동작을 제어하게 된다.

    DMA RE 미ock

    이 비ock에서는 프로세스가 데이터를 읽어갈 수 있도록 데이터를 보관하는 역할
과 DMA 뎨이터를 구성하여 프로세서의 제어어］ 의해 뎨이터를 출력하게 된다. （그
림 午15) 프로세서 정합신호 타이밍에서는 프로세서와 연동될 때의 각 신호들을 나
타내고 있다． 이 신호들의 타이밍 요구사항 들은（표 午1) 프로세서 정합 타이밍 조
건에서 정의하고 있다．


                            <


DATA BUSX ADDRW:7]




    ALE




놔RI

                                                       ;1
RDI
                                t\   Vr
                                                  ,,        td   ,4   노   +



                      （그림 4 ］듸 프로세스 정합 신호 기ming
         196                                                  4. CDMA Demodulator
                                                                                    U


                              （표 午］) 프로세서 정합 타이밍 조건

  텨gnal                          역할                     최소          최다1      단위

  tdsu         Data setup to WR/rising                  15                    ns

  tdh          Data hold after WR/rising                5                     ns
  tcw
               CS/falling to Wi/rising                  35                    ns
  tu尼改
               Address hold after Wi/rising             5                     ns
  twc
               CS/hold after Wi/rising                   0                    ns
  taw
               Address v싫id to Wi/falling               10                    ns
  tWr
               ＼人／R//＼入／
                       idth                             120                   ns
  ta$    74    Address valid to ALE falling             10                    ns

  tak          Address hold after A玉 falling            5                     ns
  ta／    凹     A万 faffing to Wi/falling                 10                    ns
  tar
               Address valid to RD falling              5                     ns

  trd          RD/falling                               120                   ns
  trc
               CS/
                hold after RD/rising                    0                     ns

  乙day         RD/hold after RD/rising                              100       ns

  乙m力工乙        Data hold after RD/rising or CS/rising   5           15        ns

  ／口寸r
               ／표』E 倒ling to RD/fa血ng                   10                    ns



 MCS Block

 PN Code 발생기에서 발생되는 코드의 위상을 변화시키는 과정인 Slew는 변화
량어］ 따라서 크게 2가지로 나누어볼 수 있다. 먼저 PN Code의 위상을 1/2칩 이내
로 맞추는 과정에서 발생하는 Slew와 위상을 정확히 얻기 위하여 1/8칩 Slew하는
과정에서 발생하는 Slew로 나눌 수 있다. 이 찌ock 은 이 두 가지 과정에서 동시어］
사용될 수 있는 안정된 칩 C10(永을 발생시키는 부분이다．
 Searcher의 Slew는 동기 획득 과정에서 동기가 맞지 않을 때 1/2칩만큼 위상을
움직이는 Delta Slew와 프로세서의 명령어］ 따라서 Slew하는 2가지 모드가 있다．
（그림 午16) 八4CS Block I五agram에서 입력되는 신호어］ 대해서 살펴보면, 먼저
'VFHEN신호는 PN 위상추적기능을 수행할 때 '1'가 되어 Slew양을 1/8칩으로 한정
하여 TE 값어］ 의하囚 Slew를 결정하게 되고 만일 이 신호가 '0'을 가지게 되면 1/2
    4. CDMA Demodulator
1                                                                                                                   卜？7


       -I丁1EN 1           卜       E\             LC      -            . LD      M8C
          Jps/ 1H卜 'H'                   LOAD                     少 LE/
                                                  1 F:                                Q[ 2:OI           [2이    卜 CHIPx1


                                                         U
        PS_NS 1+              PSNS
                                                                                                으
                                                                                                    ’
                                                                  少 RESET!                          3         Q,[2]

      TE[ 1:O] mm규＋           TE[1:O]       RESETI            .        CLK
                 2
                          >   Q 1 L2：아
                    QU
                                            RESET2
                              Q2[2:O[
                                                                                M8C
                    n켜U

                                                                       LD

                                                                       LE/                    q[ 2：아
                                                                                      Q[ 2;O] 나- 1H -s.- CI-IIPxF
                                                                       RESET!                  3     Q,[2[

       CH1Px8                                                     >    CLK




                                          （그림 午］이 MCS 블록도


칩 Slew동작을 수행하게 된다. JPS/ 신호는 加mping Slew 동작시 '0'의 값을 가지
거］ 되는 신호이다. 또한 PS卞NS 신호는 PN 위상을 전진시킬 것인지 후진시킬 것인
지를 결정하는 부호신호이다．
 Jumping Slew와 delta Slew어］ 관해서 （그림 午17) jumping Slew및 1/2 칩
Slew동작에 나타내었다. 다음 그림어］ 나타난 것과 같이 Cl-IIPX1 Clock을 이용하
여 PN Code를 생성하게 된다．

       Jumping Slew
       JPS/
                                 \                                              I
       CHIPxJ
       If PS_ES＝丁
                                  4              Nch叩 delay

       CHIPXI
       If PS_ES＝可
                                                N chip advance


       Searching Slew
       SLEW/



      CH[PXI
      If PS_ES＝丁



      CHIPXI
      If PS_NS＝可




                    （그림 千］7) Jum口ing Slew 및 1/2 칩 Slew 동작도
                                                                                                                   4. CDMA Demodulator
     198




 4.3 Finger                     Demodulator
                                                                                                                                                             )
 다음은 Finger Dem以加1毗야의 모튼 동작을 나타내는 것이다. 여기에서는 Pu毗
획득을 위해서 행해지는 Finger의 동작을 설명한다. Fii追er의 주된 임무를 수행하
기 위해서는 기본적으로 초기 Acquisition이 이루어진 상태이며, 이제부터 Finger
는 RSSI를 생성하고, 지금까지는 생각하지 않았던（혹은 문제로 생각하지 않았던）
주파수 에러를 산출하고 이러한 두 가지 값들은 Con小iner로 제공된다．


                                                                                                                Lock                   Lock RSSI
                                                                                                              Threshold                Comparator
Fn CODE                                                                          w미oh
  Cl-I ID
                                              WALSH_CODE_GEN
                                                                                                                                            +
                                                                                                                                        Lock RSSI
                                                                                                                         。2            Accumulator
                                                                                            Integration +
                                                                                                                    Q。
                     Offset                                                                 Filtering for                                          FR丘且oak
 BINARY                                             Counter                                                                                       to Corobtner
                                                                                                Gain
 OFFSET            Comparator                                                                                                                              b
                                                                                                          과
                                                                                                              碼+
                                                                                                                           I, 。。Q。


                                                                           EXt
 Fn_PN                                              卜 I ON_TIME                                                                                 Sr世BOL OAI'A
                    I_RN_DEN
 I MASK                                                                                     Integration                                           to Conbtner
                                                                                   甲aish                                             니＞ FIFO
                                                                                            for Symbol
                                                                           RXQ                  Size
                                                        Q_ ON_TIME

已｛耀- Q.YNGEN F
                                                    뇌                      爲                Integration

                                                                                                          :
                                                                 EL_TIME
                                                                                                 for
                                                                                                               L/ + 9e12
                                                             _
                                                         I
                                                                                                                              니. EARLY-LATE
                     SLE WING                                                                Processing
                                                                                        1       Gain
                                                                 EL_TIME
                                                                                                                                     Time Tracking
                                                        Q_
                                                늬
                                                                                                                                        Enable
   Rn              Position
 POSITION          Counting

                                                                                                          黑：詰：
                                                                                                             ！斜H
                                                                                                                                      Bandwidth
                                                                                                                                       Conrol
                                                                                                              A
       S1WCD0ITOIP8rawE&
                                                                                                                                     Time Tracking
                                                                                                                                     Accumulation
          0/ W F! OCtl00 B化Ck




                                                                  （그림 午］8) 日nger Demodulator



 또한 획득 상태의 PN Code를 1칩 이하의 오차로 계속 유지하는 Time Tracking
（혹은 필자는 Phase Tracking이라고 표현해 보겠다）을 한다. 정리하써 다시 말하
면 초기동기 상태에서 찾은 1칩 미만의 위상오차를 시간적으로 계속 유지한다는 것
이다．
     4. CDMA Demodulator
 1                                                        199
                                                            H기
      4.3.1 RSSI(Received Signal Strength Indicator) 계J

     시간추적을 하는 Fit坦er는 Pilot 신호를 측정하여 RSSI을 구한다. 여기에서 사용
되는 Non Coherent Energy Detect아는 앞의 （그림 士7）의 측정과 동일하다. 입력
되는 신호는 Searcher를 통해서 역확산되고, 64칩 시간 동안 적분하고 이것을 에너
지로 변환한다. 이 에너지는 Se可cher에서 Pu毗 획득을 위한 에너지와는 달리 신호
복조를 얼마나 타당하게 할 수 있는지를 확인하는, 즉 신호의 세기를 측정하는 것이
다. 이러한 내용은 Controller어］ 보고된다．
 이렇게 측정된 RSSI값은 임계치와 비교되어서 충분히 강하다고 판단되면 그 신
호를 Fit띵er가 Lock상태를 유지할 것인지, 그리고 Timing Tracking을 Enable할
것인지를 판단한다．
 I刃Ck된 Finger의 주파수 에러（FREQ_ERR）와 \Va1sh-decovered 신호（SYMBOL_
DATA）는 Combiner로 제공된다. Lock상태를 결정하기 위해서는 （그림 午7）과 같
이 Hysteresis（어떤 물리량（物理量）이 현재의 물리 조건만으로는 결정되지 않고，
그 이전어］ 그 물질이 경과해 온 상태의 변화 과정에 의존하는 현상） Lock 비교기를
사용하여 판단한다．
 만약 RSSI가 Thi보다 작다면, Finger는 Lock된 것이 아니다. 만약 Fir培er가
Pilot어］ L炚k되었다고 한다면, 수신된 신호는 양호하게 복조될 수 있는 상태이다.
이러한 동작은 가장 양호한 PN 옵셋의 Pilot 신호를 찾는 Searcher의 Detect상태
이후에 제어기어］ 의해서 Enable된다．


     4.3.2 주파수 에러 산출

 Combiner는 Carrier 주파수의 에러를 조정하기 위해서 Frequency Tr孔蜘培을
한다． 이것은 Fir坦er에서 제공해 주는 주파수 에러 정보를 통해서 이루어진다. 때문
어］ Fir坦er에서는 Cor曲iner로 제공될 주파수 에러를 산출한다．
 주파수 에러를 측정하기 위해서 Fir坦er는 Pilot Channel을 역확산하고 64칩의
역확산된 Pilot 신호 데이터를 적분함으로 에너지를 구한다. 만약 까nger가 Pilot 신
호어］ Lock되었다면（RSSI가 임계치보다 더 큰 상태） 우리는 주파수 에러만에 의해
서 감쇄될 수 있는 에너지는 이 단계에서는 무시한다．
   200                                            4. CDMA Demodulator



                                 硏indow
         mH> 시간의 증가방향
                                          41Window 01동방향




            늬 누 \1 주파수가 왜곡된 부분이
            I I    n4! 적분 Resolution에
          주파수 에러 의해서 에너지 값이 잘
                   못. 계산 된다，



                （그림 午］9) 주파수 에러 측정과 주파수 오차


 또한 주파수 에러가 있다면 앞서 측정한 에너지와 현재 측정된 값이 차이가 날
것이다. 주파수의 에러가 있다는 이야기가 된다. 이것어］ 대한 설명은 （그림 午19）을
참고하라．
 （그림 午19）와 같이 주파수 오차는 초기동기가 맞게 이루어진 상태에서 입력되고
있는 신호들을 적분 Resolution으로 적분해 갈 때 앞선 시간의 적분값과 현재 적분
값이 차이가 날 때라고 생각할 수 있을 것이다. 때문어］ 이러한 오차를 측정하기 위
해서는 "IONQPREV + IPREVQON"를 계산하여 Con曲iner로 전송한다．
 지금까지 우리는 위상오차를 조정해 왔으며, 이제 까nger는 주파수 오차를 조정
하기 위해서 주파수 오차를 Con的iner로 보내준다. 주파수 오차추적은 Combiner어］
서 하기 때문이다．


   4.3.3 Time Tracking - 위상추적

 대역확산 동기 시스템에서는 필연적으로 송수신 기간의 확산부호의 동기가 요구
된다. 전송된 확산부호와 수신기의 국부 확산부호간어］ 동기가 한 칩 이상 맞지 않는
다면, 데이터를 신뢰성 있게 검파하기 위하여 요구되는 신호 에너지의 전달이 불가
능할 것이기 때문이다. 확산부호의 동기획득（Acquis出on) 및 유지는 전적으로 수신
기의 역할로 부여되는 것이 일반적이며, 확산부호의 동기는 보통 초기동기 및 동기
추적의 2단계를 거쳐서 수행된다. 앞서 이야기한대로 부호의 초기위상은 통상적으
로 한 칩이 이내의 동기를 성취하게 된다. 즉 초기획득은 그것의 Resolution이 1칩
    4. CDMA Demodulator                                              201
口


이내가 된다. 초기동기가 성공한다면 펴］ 루프 동작으로 보다 정밀한 동기추적
(Tracking) 과정이 시작되며, 이를 통해서 연속적인 최적의 확산부호의 동기가 이
루어진다. 이때 적분 Res아ution은 1/8 칩으로 행해진다．


 Tracking Loop의 종류

 동기추적 시스템은 Coherent한 기준 반송파의 생성을 위해 요구되는 P1工기법
과 유사한 방법으로 수행되는데 두 가지 기법의 주된 차이는 위상 판별기의 구조라
할 수 있다. 반송파의 동기를 위해서 요구되는 판별기는 단순한 곱셈기인 반면에 부
호의 동기추적 루프의 위상 판별기에서는 수 개의 곱셈기는 물론 저대역 여파기
(LPF) 쌍과 포락선 검파기를 포함한다．


                                             -   Coherent Mode
                               Delay Lock
                               Lo아） (DLL)
                                                 Non Coherent Mode
             Early-Late
            Tracking Loop
                                                 Coherent Mode
                               Tau Dither
                               Loop (TDL)
                                                 Non Coherent Mode


                    （그림 4-20) Early-Late Tracking Loo口의 구분


 대역확산 시스템의 동기추적 루프는 여러 가지 기준으로 분류할 수 있다. 우선 수
신 반송파의 위상정보의 이용 여부에 따라서 Coherent및 Non-Coherent로 구분할
수 있다. 또한 대부분의 동기추적 루프는 그 위상 동기루프가 수신신호와 국부발생
확산부호의 Early-Late 위상간의 상관관계를 이용하는 Early-Late Tracking ioop
에 속하는데, 이에는 2개의 독립적인 상관기（Correlator）를 사용하는 Delay Lock
I刃op(DLL）과 1개의 상관기를 공유하여 시분할（time-sharing) 방식으로 사용하는
이름하여 Ta出 r) Dither Loop(TDL）가 있다．
 （沁herent 방식의 기저대역 동기루프는 실제적인 대역확산 통신 시스템에서 적용
이 어렵다. 우선 확산부호의 동기추적어］ 앞서서 반송파의 동기가 이루어져서 수신
신호의 복조가 선행되어야 하는데, 대역확산 시스템은 전형적으로 전송대역에서 신
호 대 잡음비가 매우 낮은 상태에서 동작하므로, Coherent한 반송파의 발생 및 복
    202                                     4. CDMA Demodulator
                                                                  1


조의 수행이란 보통 어려운 일이 아니다. 더욱이 통상적인 통신 시스템은 송수신 기
간어］ 임의의 정보전달을 목적으로 하며 이러한 정보데이터의 변조는 기저대역 루프
의 적용을 더욱 어렵게 하는 부가적인 요소로 작용하게 된다. 이러한 한 점으로 인
해서 Non-Coherent 방식의 Full time Early-Late Tracking loop혹은 delay
Locked loop가 널리 사용되고 있다．
 하지만 이러한 DLL에도 2가지의 문제가 있다. 첫째는 Early-Late II구 채널간의
진폭특성이 정확하게 평행이 이루어져야 한다는 것이다. 만일 두 채널간어］ 이득의
불균형이나 기타의 불일치가 존재하면, 위상 판별기의 특성에 옵셋이 존재하므로
추적오차가 '0' 일 때일지라도 오프셋 전압을 가하게 될 수도 있다. Full time Loop
의 경우 또 다른 문제점은 다소 고가의 부품인 상관기 등이 이중으로 사용된다는
것이다． 이상의 문제점들은 2개의 Early-Late 채널 대신어］ 한 개의 상관 채널을 공
유하는 Non Coherent Tau dither Early Late loop를 사용함으로 해결할 수 있다．
이것은 잡음 성능면에서 다소 손해를 본다는 것으로 trade off퇸다．
雄難難無뇨

 Phase21- Frequency Error

 채널을 통해서 수신단에 수신된 신호는 여러 가지 형태로 왜곡된다 ．이것은 우리
가 신호를 정의할 때 사용하는 진폭과 주파수와 위상어］ 왜곡을 가할 수 있으며, 이
러한 진폭과 위상과 주파수와 같은 물리량은 우리가 정보를 실어보내는 변수들이기
어］ 이러한 왜곡을 수정하는 것이 더욱 중요하다．
 이 장에서는 이렇게 변질된 주파수와 위상의 정확한 참값을 추적하는 것을 공부
한다． 아울러서 주파수 오차와 위상오차어］ 대해서 미리 이야기한다．
 위상의 오차는 원래 파형이 시간축상에서 왜곡치만큼 천이된 것이라고 할 수 있
다． 반면 주파수 오차는 시간축상이 아니라 주파수축상에서 왜곡치만큼 천이된 형
태로 설명할 수 있다. 이것을 그림으로 나타내면 다음의 （그림 午21）과 같다．
 즉 Coherent detection이란 이러한 위상과 주파수의 오차를 정정하여 원래의 신
호를 복조해내는 것을 의미하며, 여기에서 C小erent（꼭 달라붙다）라는 말의 원 뜻
과 같이 두 개의 신호가 완전히 일치한다는 말이며, 그러기 위해서는 수신된 신호의
정확한 위상과 주파수 정보를 알고 있어야 한다. 이와 더불어서 우리는 흔히
Synchronize와 Coherent를 비교해서 이야기할 때 Sync뇨onized는 시간적인 의미，
즉 위상정보를 파악한 상황을 이야기하나, Coherent는 여기에다가 주파수 정보까지
    4. CDMA Demodulator
U




                                                t   원 신호




                                                    위상 왜곡된 신호




                            ．「‘多 . p
                          A寸；                       주파수 왜곡된 신호
                            岺：   , .   \
                                       I.久八．
                                           小J



                      （그림 午21) Phase와 다equency Error


파악된 상태를 이야기한다고 할 수 있다．
    우리가 흔히 수학적으로 변조나 복조를 설명할 때 " sin w,刃tx cos 口JC/' 라고 들
많이 쓰는데 생각을 실제 시스템으로 구성할 때에는 결국 곱하는 두 신호의 정확한
파형을 알아야 함으로 이러한 방식을 Coherent Detection이라고 한다. 즉 서로 곱
하게 될 두 신호의 sinusoidal 신호의 주파수, 위상의 정보를 정확히 알고 있어야 한
다는 말이다. 이러한 의미에서 이것을 Coherent（이것의 영어사전적 의미는 짝 달라
붙은, 밀착된）라고 한다는 것은 어쩌면 너무나 당연하고 재미있는 표현이다.

     4.3.4 Phase Lock Loop(PLL)

    PLL은 주기적인 신호의 위상어］ 대해서 동작하는 피드백 시스템이다. （그림 +4)
는 위상 비교기（Phase Detect), 루프필터（Loop Fil扼r）와 VCO(Voltage Contr이
Osc皿at아）로 이루어진 간단한 PLL이다．
    위상 비교기는 피드백 루프에서 艾（t)와 y(t)의 위상차이 스0을 최소화하기 위해
오차 증폭기（error amplifier）로 동작한다. PLL에서 동기山乂k）는 스0가 일정할
때, 따라서 입력 兀（0와 출력 y(t)의 주파수가 일치할 때로 정의한다．

           x(t)




                      （그림 午22) 기본적인 Phase Lock Loop
                                                            4. CDMA Demodulator



 동기 된 상태에서 루프 안의 모든 신호는 정상상태가侮tead少就ate) 되고 PLL은
다음과 같이 동작한다. 위상 비교기는 스0어］ 비례하는 직류 전압을 만들고 루프필
터는 위상 비교기 출력의 고주파 성분을 제거한다. vco는 입력과 같은 주파수와
L0의 위상차이를 가지는 출력을 만들어낸다．
 （그림 午23）는 PLL 루프 안의 여러 신호를 보여준다. 입력과 출력은 같은 주파수
를 가지지만 위상차이를 가지고 있고, 위상 비교기는 입력과 출력의 Zero-crossing
사이의 시간차이와 같은 펄스 폭을 만들어내고 있다. 즉 비교 대상이 되는 신호
尤（砂와 只砂가 각각 변할 때마다 위상검출기의 출력은 현 상태를 변경한다．


                                    ,
                                        이 rising에서 PD의 출력은 현재
     이 rising에서 P1）의                    출력의 역인 ' l '올 출력
                               /'
     출력은 현재 출력의
     역인 '0’율 츌력            \
                玎t)
                       \
                           n
                y(t)

               PD
            Output
                                                                        >


         Loop Filter
            Output


                           （그림 午23) PLL 내부 파형


 이 펄스는 Loop F血er를 통과하면서 Low Pass Filtering되어 출력되는 직류전
압으로 vco를 동작시켜서 원하는 주파수를 만들어낸다．
 PLL이 t< to에서 동기상태어］ 있다가 /0시간어］ 입력주파수가 스日만큼 증가하는
경우 （그림 午5）어］ 대해 생각해 보자. 입력주파수가 출력주파수보다 크기 때문어］ 입
력 兀（勿의 위상이 더 빨리 증가하고 위상 비교기의 출력펄스는 점점 더 넓어지게 된
다. 이런 펄스는 루프 필터의 직류전압을 증가시키거］ 되고 vco의 출력주파수는 증
가하게 된다． 입력과 출력주파수의 차이가 줄어들면서 위상 비교기의 펄스폭은 줄
어들고 결국 입력과 출력의 주파수는 일치하게 된다．
 입력주파수가 천천히 변한다면 그 변화는 연속적인 스텝 주파수 입력으로 볼 수
있으며 PLL은 （그림 午24）에서와 같이 동작하여 출력주파수를 입력주파수와 일치
    4. CDMA Demodulator
1


                                                                 주파수가 왜1
                                                                 곡된 영역
                           U初
                                    ....,．他：   烈：
                                                ............/d


                                                                  노．
          x   ()



          y (t)      Th
              PD
          Outpu                          1그그-Lf
       Loop Filter
         Output

                     （그림 午24) 주파수 스딛J 입력에 대한 PLL의 동작


하도록 vco를 구동하게 된다. PLL이 동기화되기 위해서는 두 가지의 조컨이 만족
되어야 한다． 한 가지는 입력과 출력의 주파수가 일치하여야 한다는 것과 또 다른
하나는 입력과 출력의 위상 차이가 적당한 값으로 고정되어야 한다는 것이다. 즉 어
느 시점에서 주파수가 서로 일치하여도 위상차이가 적당히 작지 않으면 계속 출력
주파수가 변하는 과도（transient) 상태어］ 있게 된다．


     4.3.5 Delay Lock Loop(DLL)

    DLL은 PLL과 마찬가지로 주기적인 신호의 위상어］ 대해서 동작하는 피드백 시
스템이다． 그러나 PLL은 vco를 가지는 반면, DLL은 VCDL(Vo物ge Contr아led
Delay Line）을 가지고 있어 다른 특성을 보이게 퇸다. （그림 午25）는 위상 비교기，
루프필터와 VCDL로 이루어진 간단한 DLL을 나타내고 있다．
    위상 비교기는 PLL에서와 마찬가지로 피드백 루프에서 妖t)와 出）의 위상차이
스0를 최소화하기 위한 오차 증폭기로 동작하고 동기는 스0가 일정하게 되어있을
때이다. DLL은 PLL과 달리 입력신호의 위상신호만을 바꾸기 때문어］ 주파수는 고
려되지 않는다. 동기 된 상태에서 루프 안의 모든 신호는 정상상태가 되고 DLL의
동작은 다음과 같다．
    위상 비교기는 스0어］ 비례하는 신호를 만들고 루프필터는 위상 비교기 출력의
                                                                4. CDMA Demodulator
                                                                                      .


고주파 성분을 제거한다. VCDL은 입력신호와스0위상차이를 가지는 출력을 만들
어낸다. 정상상태에서는 PLL과 같은 결과를 보인다．



                        1J        Phase i
                 川t)                   r r-
                                 Detect。



                                              VCDL                   y(t)


                         （그림 4-25) 기본적인 D이ay Lock Loo口



 DLL의 아이디어는 주기적인 신호가 그 주기의 배수로 delay되면 위상천이는 결
과적으로 0이 된다는 것이다. 따라서 위상 비교기는 尤（t)와 只t)의 위상차이가 주기
의 배수가 되도록 루프를 구동한다. 보통 위상차이는 한 주기가 되도록 한다. 兀（t)
는 주기가 T인 신호이고 兀（t)와 y(t)의 위상차이가 Td라고 하면 VCDL은 T-Td의
delay를 더 추가하여 주면 兀（t)와 只t)의 위상차이는 T가 되고 DLL은 동기되는 것
이다．
 PN Code는 Aut아Correlation특성이 거의 orthogonal한 특징을 가지고 있다. 때
문에 이러한 특징은 PN Code를 확산코드로 사용하는 CDMA시스템에서 중요한
특징으로 사용하고 있다. 그런데 여기에서는 Early-Late의 위상을 가지는 PN
Code 조합을 생각하1 보자．


                                                     yi(t)

          수신된 신호 Sr(t)




                                                     y,(t)

Early Spreading Waveform (ESW)                Late Spreading Waveform (LSW)


               K1C(t- fd)
                                                             Clock

                       （그림 午26) DLL 가acking sys抱m의 분석 예
    4. CDMA Demodulator                                                                                       2（刃
.


    여기에서 Channel을 통해서 수신되는 신호는

          S,(t) =-%.[1c(t- Td )+n(t)                                                                           (4-3)

라고 하고 국부 PN Code 발생기로부터 출력되는 Early Channel의 ESW와 Late
Channel의 LSE는 다음과 같다．

          ESW＝小T,+AT
              \
                     "
                                   "    2       "
                                                                                                               (4- 4)




         LSW=.1t글미                                                                                             (4-5)
    여기어꺼 LI는 칩 Duration（혹은 주기）으로 정규화된 Early Ch帥nel과 Late
Channel간의 시간차이라고 정의한다. 아울러서 PNG에서 설정한 추정오차와 실제
전송위상과의 차이를 칩 I거iration（혹은 주기）으로 정규화 시킨 것을 '3로 정의한다．
즉 정리하면 다음과 같다．

          .     T,,,/, - TL:,
         LI =                                                                                                  (4-6)
                        T


          a= 7;m                                                                                               (4-7)
                   T,
    이때 백색잡음 n(t）가 없는 상태라고 가정하고 에러신호 e(r, 3）를 표시하면 다
음과 같다．

         E(r,7二，乙）= y2(t,7二，乙）中 y1(t,7二，乙）

                            ＝瓦i-       V2   c   (t   －   祉   （!   －   乙1;   ,).   (   （   『－   乙   『id)   ]    (4卞8)


    위의 식에서 나타난 에러신호의 DC성분, 즉 위상성분이 제거된 신호가 위상추적
의 정보로 사용된다. 때문어］ 우리는 위의 식에서 DC성분을 찾아야 한다. 때문어］ 식
(4-1)을 한 주기 동안 적분하면 Sinusoidal 성분은 모두 없어질 것이며, DC성분만
남을 것이다. 주의할 것은 에러신호의 주기는 PN Code의 주기와 같다는 것이다．
    주기가 L인 PN Code인 경우 에러신호의 DC성분은 다음과 같이 구해진다. 아래
의 식에서 새롭게 정의된 功는 DC성분만을 나타냄으로 더 이상 시간어］ 대한 함수
   208                                                             4. CDMA Demodulator
                                                                                         .


(time varying）가 아니므로 t가 사라졌다. 그러나 이 함수는 여전히 전송지연위상
(Td）과 추정위상（Ta의 함수로 표시되며, 때문어］ 우리는 위상추적어］ 사용되는 이
값을 켤정하기 위해서 전송지연위상（Td）과 추정위상（Td）의 값들의 변동을 고찰함
으로 해석할 수 있을 것이다. 이와 갇은 이유로 계속 수학시간어］ 배운 이상한 기호
들을 계속 쓰겠다．



 E（乙Td):(，伽(1;,力
   ＝古，此出1-c(t
           V2 －乙｛「（『－乙－슬工）-c(t-T『슬미*                                             (4-9)


 여기에서 LTC는PNCcx妃인 c(t)의 주기이다. 일반적으로 c(t)의 자기상관함수를

다음의 식 (4-10）과 같이 정의한다면, 에러 성분의 I乂성분 중 전송지연위상（乙）과


                       D (8)                                        Da(8)
         스＜ 1.0인 경우                                   l ＜八＜2인 경우




                               Rj (&+A'2)Tj




                                    1   RJ(- 酊2)T J
                                                 ,    :




         /\= 1.0인 경우




                       (c)
               （그림 午27) 추정오차에 의한 Error신호의 자기상관도
    4. CDMA Demodulator                                         209
1

    추정위상（Td）의 함수로 표시되는 1入는 다음의 식 (4-11）으로 표현된다．

                    =
          R                               +         dt          (4中10)
              (r)
                        T
                                              'r)
                                     (!
                                o.
                        ljT.
          D (乙t）띠乙－나斗m-t中）
                               =Rj(S-슬)
                                     2 Tj-Rj(8+슬)T]             (4-11)
                               三IM히

    결국 I刀는 a의 함수로 표현될 수 있으며, 이것은 추정오차와 전송오차간의 차이
가 신호오차어］ 영향을 끼치므로 이 값을 통하여 추정오차를 줄여갈 수 혹은 오차를
일정한 범위 안어］ 둘 수 있다는 이야기를 할 수 있다. 그러므로 지금까지의 결과로
볼 때 DLL의 Error 신호의 특성은 식 (4小11）어］ 의해서 （그림 午27）과 같이 생각하1
볼 수 있다．
                                                         1뇨侮）




          （그림 午28) 士］/2 칩 Early-Late 옵셋일 ［대 오차신호의 자기상관도


    여기에서 우리는 에러 신호는 결국 d의 크기어］ 따라서 （그림 午27）과 같은 다양
한 자기상관 값을 가진다. 결국 이러한 형태가 되었을 때 PN Code를 추적하는 범
위는 이러한 /\uto Correlation값이 선형적으로 변화하는 부분일 것이다. 즉 DLL어］
서 코드를 추적하는 과정은 그것의 자기상관 값이 선형적으로 변하는 부분일 것이
며, 때문어］ DLL의 Delay Line은 선형적으로 변경되면 되는 것이다．
   D"n                                                            4. CDMA Demodulator
                                                                                        .


 또한 앞에서 이야기된 초기 코드 획득단계는 Early-Late의 위상을 가지는 PN
Code의 자기상콴 값을 선헝적으로 변하는 영역으로 진입시키는 역할을 한다고 볼 수
있다．


      2V乭c(t-Td)cos(o勿t＋中) + noise




            乃巾- TJ2) 尸 Td)cos(w。十 凹                 ＼厄巾＋ TJ2)         于d)COS(W0+ 回伊）t




                                          n   n-i       ... ...    1 三＜11 VC'6n
                                      1             t                 !             』



                                              n-stage LFSR

             （그림 午29) Non Coherent DLL의 Envelo口e Correlation


 （그림 午29）는 l如n Coherent DLL의 Envelope Correlation을 설명하고 있다．
결국 Phase Detect부분은 그림과 같은 중간주파와 Sinusoidal신호가 변조된 상태
로 입력되나 Envelope Correlation Network에서 위상성분을 제거하여서 Non
（노herent하게 Correlation을 하고 있음을 보여 준다．
  또한 이러한 신호는 Low Pass Fil扼ring을 수행하는 Loop F血er를 통하여 저대
역 신호만 살아남게 되며, 이것은 우리가 앞서 설명한 식 (4助의 에러만을 VCC로
전송하게 될 것이다．

   4.3.6 Taufr) Dither Loop

  Tau( r) Dither Loop는 기존의 DLL과는 달리 1개의 상관기를 가지고 시분할하
여 이루어지게 하였다. 기본적인 원리는 DLL과 동일하나 이러한 상관기가 다르며，
하나의 상관기에서 Early와 Late Channel을 구성해야 하므로 이것을 적절히 교대
로 출력할 수 있게 하1 주는 Sw迂ching 회로가 추가될 것이다．
  （그림 午30）은 Non Coherent Early-Late Ta寸미ther Loop의 전형적인 예이
다. 이것은 （그림 午26）과 비교할 때 PN Code 발생기에서의 출력은 early-late
    4. CDMA Demodulator
1


channel 각각 2개로 같은데 Phase detect야부분은 하나로 구성되어 있다. 또 다른
하나의 차이는 PN Code 발생기어］ Sw仕ch가 있어서 출력을 조정한다는 것이다. 이
때 이 Switch의 속도, 즉 Sw此C蜘g Frequency fq는 (2TqY1로 정의되며, 이것은
Dither Frequency라고 한다．
    Dither Frequency는 이 tracking loop의 특성을 결정짓는 중요한 요인이 된다．
그럼 이 I玉ther Fr因uency와 이 tracking loop의 특성이 어떤 영향이 있는가를 고
찰해 보자．
    수신된 신호 巾）는 앞 절의 DLL을 해석할 때와 마찬가지로 PN Code의 위상지
연 성분과 carrier 주파수로 변조되어서 Sinusoidal 신호 항이 첨가된 형태의 신호
일 것이다. 이 신호는 Local PN Code 발생기와 Local Osc皿毗아의 신호가 합쳐진
신호, 즉 Local Oscill砒or의 발생신호로 변조된 또 다른 위상의 Sinusoid出형태의
신호와 곱해지어 결국 신호 y(t)는 BPF를 통과되면서 고주파 성분의 carrier은 없
어지고 IF성분의 Sinusoidal만 남게 된다．


                                  PN 코드가 RF및 위상 지
                                  연 성분에 의한 주파수의
                                  정보를 담은 Sinusoidal신
                                  호에 의해1 곱해진（변조된）                                중간 주파수                 모든 Sinusoid키의
                                  형 태．                                           성분이 제거                 주파수성분이 제거된
                                                                               1 된 신호；                  DC 신호．


    추측된 r (t) 신                                                            Sciu are La\\
                                         ya) 難發難擊籌 訂r7
                                                                                                                          艸




    호 : RF와IF포                                                   嫡
                                                                 斛          En ye In1) (1
    함．                                                                       I) F I ( (1 口
                                   可I)
                                                                                                -q(t)




            心t卄O.5 '   T     1            心I   '   -        5'   Tj
     Reference （노de뇨
                        ')                             O.
                             r）卜J n．口n0r口＋nr           <
        Sequence             ' " 니UU山H四'                             Spreading waveform Clock     饌蠶怒蚤纛置

                       r (t) 心 V仁7깆 c(t - 乙) casio勿t + 仇(t - 乙 ) + 9 1

                       口片 入／( 馬) 和- T力 + q（加. 5스 乙)cos[(的 + 0IF汁＋甲' ]
                                                                                                세곱하고        더하기      하는
                  BPF를 통해서 제거됨L                                                                 Envelose Detection에서 제거
                  BPF애서 띠F성분율 7斗                                                                됨     이     과정을     통하여
                  기 시킴．                                                                         미nusoidal은 모두 없어 짐．


       y(t) 七 乃K；戶 尺끄S 土 0；됴l7 兀Icosi（聊I + 아(t 小 7；
                                                  口 + q）小q)' /

              （그림 4-30) Non Coherent Early卜Late Tau-Dither Lao口 해석
                                                      4. CDMA Demodulator
                                                                                 .


 이러한 출력신호 z（砂는 이제 마지막 남은 Sinusoidal항의 중간 주파수의 주파수
성분을 제거하기 위해서 제곱을 취하고 더하는 처리 일명 envelope detection을 통
해서 DC성분만을 찾아낸다．
 우리가 지금까지 왜 힘들게 DC성분을 찾았는가를 DLL을 설명할 때도 이야기했
지만 까nger에서는 위상추적만하며, 주파수로 인한 왜곡성분은 Con小in町에서 하게
된다. 즉 전체적으로 생각하1 본다면 지금 나타나고 있는 에러는 위상과 주파수에 의
해서 발생되는 총체적인 에러일 것이나, 이러한 에러를 찾아가는 과정에서 위상과
주파수를 불리하여 각각의 에러를 별도로 수정하겠다는 생각이며, 이것은 위상 어］
러와 주파수 에러가 각각 독립적이어서 그것들의 정정 결과를 super position해도
퇸다는 생각에서이다．
 다시 원래 이야기로 돌아가서 결국 에러신호 e( t, d）는 DLL의 출력과 비슷하나
S硼眈h q(t)에 의해서 다음 식과 갇이 표현될 수 있다．

           n
           D
               十和小如－[(8*如｝
       i
       E                                    /
                                                      )
                                            (
                                                          }
                                                      /
                                            \
               -1-q(t）戊小二［(5슬）4］
                               『[(8『슬）끄}］
               근瓦P｛町하斗,卜呻＋스
                2   L    2         2   叫和       『兀＞           ＞助op   (4-   12)
 즉 Switch의 동작 주파수가 Loop의 대역폭보다 많이 작다면 하나의 상관기로 구
성된 tacking loop가 2개의 상관기를 가진 tracking ioop의 동작과 거의 같은 특징
을 가진다고 할 수 있다. 이러한 Tau Dither 乙刃p(TDL）은 帥alcomm사에서 제안
된 CDMA 시스템에서 사용되는 방식이다．



  4.4 Rake 수신기                                                                       )

 Rake 수신기는 크거］ 3가지 부분, 즉 심벌 결합기（Syn也아 Combiner), 주파수 오
차결합기（Frequency Error Combiner), 전력제어단（Power Control Unit）으로 그
것의 기능을 나눌 수 있다．
 주파수 선택적인 다중경로 Fading 채널환경（Freq呻兀y Selective Mult珀ath
    4. CDMA Demodulator                            2化
1


Fading Channel) 하에서 다중경로 성분 중 하나의 경로신호 성분만을 추적하여 복
원할 경우, 나머지 성분들은 잡음으로 작용하여 성능저하를 초래한다. 그러나 모튼
다중경로 신호 성분들은 최종 데이터 복원에 이용하면 SNR측면에서 이득을 얻게
퇸다. 이러한 이유로 심벌 결합기는 각각 독립된 경로를 추적하고 있는 까nger어］ 의
하여 복원된 다중경로 신호 성분들을 적당한 가중치를 곱하여 더하게 된다. 또한 각
Fir坦er는 독립된 다중경로 신호를 추적하게 되므로 서로간어］ 시간정렬이 되어 있지
않다. 이와 같이 시간적으로 정렬이 되어 있지 않은 복조된 데이터들은 최종 데이터
복원을 위하여 심벌 결합기 안에서 시간적으로 정렬시켜야 하는데 이러한 작업을
Deskewer이라고 한다. 이처럼 시간정렬을 하는 방법으로 심벌 결합기는 특정한
Finger어］ 기준하여 다른 Fir培er들의 뎨이터를 복조한다. 일반적으로 가장 먼저 도
착한 경로를 복조하는 Fir坦er를 기준으로 사용한다. 그러나 시간적으로 변화하는
채널 환경하에서는 가장 먼저 도착한 신호라 할지라도 시간적으로 변하게 퇸다. 따
라서 심벌 결합기는 새로운 Finger어］ 다시 동기를 맞추어야 한다. 이러한 동작을
Slam Operation이라고 한다. 수신단의 Fir培er는 PN부호추적 루프를 사용하여 특
정한 경로 신호성분을 추적하여 계속적으로 동기를 유지하게 된다. 그러나 송수신
단의 시스템 Clock의 주파수차이로 인하여 수신된 다중경로 신호성분들은 수신단
의 시간기준어］ 대하여 시간적으로 흐르게 된다. 즉 현재 심벌 결합기가 동기를 맞추
고 있는 Fir坦er도 시간적으로 흐르게 됨으로 올바르게 뎨이터 복원을 하기 위해서
는 심벌 결합기도 시간적으로 계속 Finger어］ 동기를 맞추어야 한다. 이러한 동작을
Finger Tracking이라고 한다．
    주파수오차 결합기는 각 다중경로 신호성분에서 추정된 잔여 주파수오차를 결합
하는 부분이다. 각 Finger어］ 의하여 추적된 신호성분에서 잔여 주파수오차 추정기
(Frequency Error Estima加r）에 의해서 추정퇸 和斗수 오차는 주파수오차 결합기
를 통해서 최종적으로 PD入4(1뇨ise Density Modu胤幻n）으로 출력퇸다．

     4.4.1 심벌 결합기（Symbol Combiner)

    심벌 결합기는 Deskewer, 덧셈기, Clock/ 제어부 등으로 나뉘어진다．
    는 시간적으로 정렬되어 있지 않은 복조된 데이터들을 시간적으로 정렬시키는 부
분이고 덧셈기는 정렬된 데이터들을 더하써 최종 데이터로 출력한다. Clock／제어부
는 심벌 결합기 전체를 제어하는 신호를 발생한다. 심벌 결합기는 각 Finger어］ 있는
                                                                     4. CDMA Demodulator
   214                                                                                     1



Clock들과 독립적으로 Clock 발생 돼ock 을 가지고 있다．

     ewer

 이것은 시간적으로 정렬되어 있지 않은 까nger의 데이터들을 시간적으로 정렬하
는 부분이다. 원래 Skew는 시스템의 내부 Clock과 외부 Clock간의 위상차이를 가
질 때 이러한 위상의 차이를 일컫는 말이다. 그런데 여기에서는 동기 시스템에서는
수신된 PN Code와 국부 PN Code간의 위상차이를 이야기한다고 생각할 수 있다．
이러한 skew를 제거하는 것을 de-skew나er 라고 이름붙인 것이다．
 한편 Searcher에 의하써 탐색된 많은 다중경로 성분들은 각 Finger어］ 할당되어
동기를 유지하게 된다. 따라서 각 까nger어］ 의해서 복조된 데이터 Frame들은 다른
Frame 시간기준, 즉 PN Roll을 발생하게 된다. 이렇게 다른 시간 기준을 가지는 각
복조된 데이터들은 각각 다른 Deskewer buffer어］ 저장된다. Deskewer 버퍼어］ 저
장되는 데이터 순서는 저장주소를 각 까nger의 시간 기준인 PN Roll로 초기화함
으로서 Frame의 첫 번째 심벌을 첫 시작번지어］ 저장하도록 한다. 또한 한 Frame의
크기가 버피의 깊이의 정수배가 되도록 버퍼의 깊이를 정하면 매 Frame의 첫 번째




                         M厘ite
                        Address

                    寸2 Symb이S卜켜2 Sy岫이S H


                          PN R이1



         Finger 2



                     1가3t1I
                    4e노뉘




                                      read
                                     address


                              4 Syn心이5         Timing 1   Timing 2         Timing 3



                     （그림 午31) Deskewer블록의 동작 타이밍
    4. CDMA Demodulator
口                                                                                                   2伯


심벌은 첫 번째 시작번지어］ 저장할 수 있다. 그리고 매 Frame의 PN Roll로 버퍼의
저장 주소를 초기화함으로서 시간적으로 변경되는 까nger의 상태어］ 유동적으로 첫
시작번지에 첫 번째 심벌이 저장되도록 할 수 있다. 이것은 Si계ii Operation에서 자
세히 설명하기로 하고 여기에서는 Finger에 추적되고 있는 뎨이터가 변화되지 않고
안정적으로 이루어지는 경우, 즉 Deskewer의 경우만을 우선 생각한다．
 Fir坦er가 처리하는 Frame의 시작값을 각각의 버퍼의 시작 번지에 입력하게 하
여서 처리하므로 이 버퍼의 크기는 다중경로로 인해서 지연되어지는 Frame의 수와
같을 것이다. 즉 버퍼의 크기가 8이라고 한다면 다중경로로 인한 경로차이가 8
Frame 정도가 되는 것이다. （그림 午31) Deskewer 미ock 동작 타이밍도는 이러
한 동작을 이해하기 쉽게 하기 위해서 2개의 까nger와 Deskewer 버퍼의 깊이를 4
로 하여 앞으로 설명하겠다．
 （그림 +31）에서 까nger2은 Fingerl 보다 1심벌 지연된 다중경로 성분이다. 앞서
이야기대로 심벌 결합기는 먼저 들어온 경로인 까nger 1의 PN Roi띠］ Combiner의
시간을 맞춘다. 즉 심벌 결합기의 PN Roil은 까ngerl보다 버퍼 깊이만큼 늦은 4심
벌 지연을 가지고 동기를 맞춘다．


                         Finger 1 Deskewer                      Finger 2 Deskewer

        Timing 1


                    Write    2
                   Address
                                                            Write    1
                                                                         >
                                                           Address
                                             0                                l
                                                  Read                                0    Read
                    Write    4                   Address                          4
                                 卜                                                        Address
        Timing 2   Address
                                     4
                                                            Write    3
                                                                         >
                                     3                     Address
                                                                              3
                                             2    Read                                2    Read
                                         4                                        寸
                                                 Address                                  Address
                                     2                                        2

                                     l                                        l


       Timing 3
                                                                              4

                    Write                                                     3
                   Address
                                                                              2
                                                            砥rrite   l
                                                           Address
                                                                         >1
                                                                              5
                                                  Read                                0    Read
                                                 Address                          4
                                                                                          Address



             （그림 十32) 심벌 결합기가 Deskewer buffer를 읽는 타이밍
                                                                                                4. CDMA Demodulator
                                                                                                                                 =


 따라서 버퍼어］ 도착한 Finger 1의 데이터는 같은 시간어］ 읽혀질 Finger 2의 심벌
을 1심벌 시간 동안 기다린 후 （그림 午32）와 같이 Combiner어］ 의해서 읽혀진다．
 Timing 1에서下inger 1은 버퍼에 datal, data2, 즉 두 심벌을 섰으며, 1심벌 지
연을 가지는 Finger 2는 한 개의 심벌, datal을 버피어］ 섰다. 따라서 심벌 결합기는
Timing 1에서 각 버퍼로부터 첫 심벌인 datal을 읽게 된다. Timing 2에서는 3번
째 심벌인 data3을 읽으며, Timing 3에서는 5번째 심벌인 data5를 읽는다.
 심벌 결합기는 가장 빠른 경로를 복조하고 있는 까nger 1의 PN Roll어］ 버퍼 깊
이 만큼인 4 심벌 지연을 가지고 동기를 맞추고 있으므로 심벌 결합기는 언제나
Finger 1의 저장주소와 2심벌의 간격을 가지고 읽히고 있다. 즉 Finger2가 추적하
고 있는 신호가 Fingerl보다 2심벌 간격 이내의 지연이라면 결합기는 정상적인 동
작을 할 수 있을 것이다．

 Slam Operation

 S1a끄 O硏貂tion은 심벌 결합기의 시간기준을 새로운 Fit坦er의 기준시간어］ 동기
를 맞추는 것이다. 심벌 결합기는 앞서서 이야기된 때로 가장 빠른 신호어］ 동기를
맞춘다. 이것은 일반적으로 가장 빠른 경로의 신호가 Fa五ng을 가장 적게 받았다고
볼 수 있기 때문이다. 어찌 되었든 이렇게 심벌 결합기가 가장 빠른 신호어］ 동기를

       까ng아_1 PN Roll
                                                                                  A                              J
                                                                                                                 \
                                                                                                                 1
     Finger 1                Frame 1                     Frame 2                      Frame 3
                                                                                                                 \
                -



                                JL                          JI                              A



          Fi唯er그 PN Roll
                                                     A                                A
     Finger 2
                        !1
                                  Frame 1                        Fram                           Frame 3


                                                                    r
                                         L                                                           A



                    Combiner R여l                                                                L
                                                            A뇨力
                                A
                                 (
                                                                                            J
    Combiner                                 Frame
                                 Finger_i Tracking
                                                     1
                                                                    (    Frame2
                                                                    拉inger_2 Tracking
                                                                                           X             Frame       3
                                                                                                     Finger_i Tracking
                                                                                                                         )   卜



                              Timing 1                            Timing 2                Timing 3

                    （그림 午33) SIam C巾er帥on 이 일어날 때의 타이밍
    4. CDMA Demodulator
.


맞춘다 하더라도 시간적으로 랜덤하게 변하는 채널환경에서 심벌 결합기의 동기를
제공해 주고 있는 다중경로 성분이 사라질 수도 있으며, 또는 현재 신호보다 더 빨
리 도착하는 성분이 나타날 수도 있다. 따라서 심벌 결합기는 이러한 경우가 발생했
을 경우 다시 새롭게 동기를 맞출 필요가 있다. 이것을 Slam Operation라고 한다．
    이러한 Slam Operation작업을 위해서는 다중경로 신호 성분에 대해서 시간적으
로 계속 주시하먀 할 필요가 있으며, 이러한 작업은 Searcher가 수신된 신호어］ 대
한 계속적인 탐색을 통해서 이루어진다．
    （그림 午33）의 Timing 1시간에서 심벌 결합기는 Fingerl어］ 동기를 맞추고
Timing2어］서 Fingerl의 신호가 사라졌을 경우어臣 Finger2로 시간을 맞춘다. 그
리고 Timing 3에서는 다시 까ngerl이 살아났으므로 까ngerl어］ 동기를 맞춘다．
    현재 가장 빨리 도착한 신호를 추적하고 있는 까nger가 버퍼어］ 데이터를 쓰는 주
소번지가 심벌 결합기가 버퍼를 읽는 주소번지보다 2심벌 빠르다. 그러나 만약 현
재 다중경로 성분보다 더 빨리 도착하는 새로운 신호가 발생했을 때 그 신호성분을
추적하고 있는 Fii坦er가 데이터를 버퍼어］ 쓰는 시간은 심벌 결합기가 버퍼를 읽는
시간보다 2심벌 이상 차이가 난다. 이러한 이유로 버퍼의 깊이를 정할 때 현재 신호
보다 더 빨리 도착하는 새로운 신호가 발생할 때, 이 신호의 데이터를 버퍼어］ 쓸 수
있는 여유가 있어야 한다. 때문어］ 4심벌의 버피 깊이라면, 현재 가장 빠르다고 생각
하고 있는 경로가 가장 늦을 가능성도 있으므로 Search Win面w을 설정하는 것과
비슷한 원리로 버퍼 깊이의 1/2정도를 지연하는 이유가 여기어］ 있다．
    다시 말하면 버퍼 깊이가 4라는 것은 현재 신호보다 더 빨리 도착한 신호성분이
버퍼어］ 데이터를 쓸 수 있는 여유 2심벌과 지연된 신호의 지연성분 보상을 위한 2
심벌을 생각한 것이다.
    （그림 午33）에서 보여지듯이 Slam Operation은 Frame 단위로 일어나며, 따라서
Slam Operation이 일어날 때마다 심벌 결합기의 Frame 기준시간이 달라진다. 이
러한 이유로 Sl계ii Operation이 일어날 때마다 Frame의 길이가 달라지며, 따라서
Slam Operation이 일어나는 Frame 경계점에서 데이터들이 깨지게 된다．
    또한 이러한 동작어］ 의해서 심벌 결합기는 새로운 시간기준을 갖으며 이 시간기
준은 수신신호어］ 대한 수신단의 모든 시간기준을 제공한다. 즉 심벌 결합기는 수신
신호의 최종 soft decision 데이터 출력에 대하여 심벌 결합 다음 단의 수신 뎨이터
처리어］ 대한 모든 Cl(兀k을 제공한다. 단말기 송신기의 PN Roll을 안테나에서 수신
   218                                                                 4. CDMA Demod미atc玎
                                                                                            .


된 기지국 송신신호의 PN Roll이 안테나에 도착한 시간과 일치하도록 하는데, 이렇
게 모든 단말기가 기지국의 시간에 동기를 맞춤으로 기지국은 쉽게 단말기의 신호
어］ 대한 탐색을 할 수 있다. 이렇게 단말기의 송신신호의 기준시간이 필요한데, 이
기준시간은 심벌 결합기가 제공한다. 즉 단말기는 심벌 결합기가 동기를 유지하고
있는 Fir培er의 시간기준을 기지국의 시간기준으로 여긴다．

 심벌 결합（Symbol Combining)
 심벌 결합기에서 최종 심벌 결합은 각 Deskewer버퍼에서 읽혀진 데이터를 더하
면 된다． 이 부분에서 문제가 될 수 있는 사항은 하드웨어의 복잡성이다. 실제로 각
Fir坦er에서 복조된 데이터들은 역확산 후 한 심벌 동안 누적된 결과이기 때문어］ 실
제 시스템에서는 많은 Bit수를 가지고 있다. 또한 각 Deskewer 버퍼에서 읽혀진 심
벌들을 더할 경우 까nger의 개수어］ 따라 덧셈기가 필요하다．

 Finger Tracking

 앞서 설명되었듯이 심벌 결합기는 가장 빨리 도착한 다중경로 신호성분을 추적하
고있는 Finger어］Deskewer bt迂fer깊이 인 4심벌의 간격을 가지고 동기를 유지한다．
그러나 이 신호성분은 시간적으로 변하는 여러 가지 채널환경 및 송신단과 수신단
의 구동 Clock의 주파수 차이로 인하여 시간적으로 위치가 변하게 된다．


                            l 집이 전진한 견과


         Positive Slewlng            5th         4th      丑i1 2nd      1st




          INO b ICW1fle        nth         4th         A1K11111 Z nU    1st




         iegative iewingcm 4th 1目므 "fld 1st                        l 짚C가 후甘한 켤꽈


                （그림 午34) 심벌 결합기가 日nger를 추적하는 Timing

 신호가 시간적으로 변하면 추적루프를 사용하여 신호를 추적하고 있는 까nger의
위치도 시간적으로 변하게 된다. 따라서 심벌 결합기는 시간적으로 변하는 Finger
    4. CDMA Demodulator
.


어］ 동기를 유지해야 하며, 이러한 동작을 까nger Tracking이라고 한다. （그림
午34）은 심벌 결합기가 Fit垠er를 추적하고 있는 과정을 보여 준다. 시간적으로
까nger의 위치가 변하지 않을 경우 4심벌 지연된 까nger의 PN Roll은 심벌 결합기
의 PN Roll과 일치한다. 즉 4심벌 지연된 Finger의 PN Roll이 심벌 결합기의 PN
Roll어］ 비해서 앞어］ 있으면 심벌 결합기는 앞으로 움직여야 하며, 뒤어］ 있으면 심벌
결합기는 뒤로 움직여야 한다. 위와 같이 심벌 결합기의 위치를 조정하는 것을
Slew血g이라고 한다. 이러한 Slewing 동작은 심벌 결합기의 구동 Clock을 조정하
여 이루어진다. 또한 이러한 Slewing 동작은 Frame의 기준인 PNRo끄의 위치를
가지고 이루어지므로 한 Frame어］ 한 번씩 보상된다. 이렇게 한번 보상될 때, 얼마
나 움직일 것인가는 구현하고자 하는 시스템의 특성 및 환경어］ 따라서 다를 것이다．


         오차 결합기

    수신단에서 수신된 신호를 가지고 올바르게 데이터를 복원하기 위해서는 주파수
오차 및 위상오차어］ 대한 보상을 하1 주어야 한다. 심벌 결합기 앞 단에 있는 위상오
차 추정기 및 보정기는 최대 수백 I七까지 주파수 오차를 보정할 수 있지만 이보다
큰 범위의 주파수 오차는 IF단에서 보정해 주어야 한다. 각 Finger어］ 있는 잔여 주
파수오차 추정기어］ 의해서 추정된 주파수 오차는 주파수 오차 결합기를 통하여 더
한 뒤 PDM(I＼표se Density 八如血lation) 형태로 출력퇸다．



         Searcher Task의 동작-Soft叫are

    Acquisition State에서 Software는 복조가 가능한 충분한 세기의 Pil毗을 찾는다．
소프트웨어는 4단계（Stage）로 구성되어 있고 각 단계는 각각 4개의 상태（State）로
구성되어 있다. 각 상태간의 천이는 Searcher가 전체 PN Roll동안 P丑야의 위상을
찾지 못했을 때 발생되며, 이때 So且w可e는 각 상태어］ 해당하는 Se계rching
Parameter를 玩ading한다. 각 State동안 Software는 기본적으로 다음과 같은 일
을 수행한다．
    米 Searcher와 Fit培er를 초기화시키고 start시킨다．
    半 탐색이 끝나기를 기다린다（DUMP DONE interrum를 기다린다）.
    永 탐색이 끝났으면 그 결과를 읽어와서 evaluate한다．
    220                                                    4. CDMA Demodulator
                                                                                 U


 이와 같은 일을 수행하기 위해서 소프트웨어는 다음과 같은 Parameter들을
Se町cher engine어］ 제공한다．
 水 \Vindow size（옵셋의 수） : 이만큼의 옵셋어］ 대해 Searcher는 energy를 계산
   한다．
 1k G沚n
 * Number of 칩 to integrate
 * Number of non-Coherent pass to integrate
 * Number of 칩s for Early dump
 * Early dump Threshold


   4.5.1 탐색 Parameter

 Searcher는 그 （加eration을 위해 다음과 갇은 Parameter들을 사용한다. 이
Parameter들은 Searcher가 1PNR에 동안 Pu毗을 찾지 못했을 경우 다음 state의
것으로 교체되며 4 PN Roll 이후어臣 state 4의 Parameter들을 이용하여 계속 탐
색한다．


                            （표4-2) Searcher Parameter
              l단계                    Detect value   Dwell va山e      Verify value
 Window Size(1/8 칩 단위）                  64X8            64< 8          6X8
 Gain                                   0x02            0x02           0x02
 札f 칩 to in扼rgrate(4 칩 단위）              128/4           128/4          128/4
 Passes intergrated non-Coherently      OxOO            OxOl           0x07
 Early dump af扼rx 칩（4칩 단위）               64/4           120/4          120/4
 Early dump Threshold                    173            378             81
 硏／indo＼入／ 欲：cept T뇨esh이d                864            1253           2059

              2단7引                   D이ect va山e     Dwell value     Veri如 va山e
＼사indow Size(1/8 칩 단위）                  64x8            6X8            6X8
 Gain                                   0x02            0x02           0x02
 #of 칩 to intergrate(4 칩 단위）            160/4           160/4          1以）/4
 Passes intergrated non-Coherently      0x00            0xOl           0x07
 Early dump af比rx 칩（4칩 단위）               80/4           152/4          152/4
 Early dump Threshold                    189             479            81
 Window accept Threshold                 918            1｛炙；6          2574
     4. CDMA Demodulator                                                 221
.


                 3단741                  Detect va山e    Dwell va山e   ＼旭II加 value
    Window Size(1/8 칩 단위）                  64X8           6X8          6X8
    Gain                                   0x02           0x02         0x02
    #of chip to intergrate(4 칩 단위）         128/4         128/4         128/4
    Passes intergrated non-Coherently      0x02           0x05         0x07
    Early dump after x 칩（4칩 단위）            120/4         120/4         120/4
    Early dump T뇨eshold                     270           270           81
    Win面w acce1元 Thresh아d                  1440           2160         2059

                 4단2켜                   Detect value   Dwell va山e   Verify value
    Window Size(1/8 칩 단위）                  24 x 8         6X8          6X8
    Gain                                   0x02           0x02         0x02
    札f chip to intergrate(4 칩 단위）           72/4          72/4         72/4
    Passes intergrated non-Coherently      0x06           0x07         0x07
    Early （如rnp after x 칩（4칩 단위）            64/4          64/4         64/4
    Early dump T뇨e針l아d                       36            36           0
    Window accept Threshold                1166           1401         1150



       4.5.2 각 상태（State）의 동작

    각 상태는 Searcher, Finger, Cor的iner를 제어하는 서로 다른 Parameter 세트
를 사용하는 것으로 구별퇸다. 전체 상태를 종합하써 나타내면 （그림 士44）와 같다．


    Searching Window의 개념

    Searcher가 전체 PN Roll을 탐색할 때 전체 off set을 한꺼번어］ 검사하지 않고
몇 대의 옵셋으로 나누어서 탐색하는데 이렇게 나뉘어진 단위를 \Vin面＼V라고 하고
보통 64칩을 한 \Vindow로 해서 탐색을 한다. 즉 64 칩의 위상 후보들을 순차적으
로 탐색한다는 것이다．
    처음 탐색하는 비교적 넓은 \Vin面w를 DE丁ECT ＼入TTNDOW라 하고 여기에서
찾은 max energy position(A）을 중심으로 좁게 만든 \Vindow를 DWELL
Window라 한다. 또 여기에서 찾은 max position(B）을 중심으로 새롭게 만튼
Window（이것 역시 Dwell Window와 비슷한 크기）를 VERFY Window라 한다.
이와 같이 \Vindow의 크기가 줄어들게 하는 것은 우리가 찾고 있는 위상값의 후보
를 추려내었다는 의미이다．
I   222                                                      4. CDMA Dem（가加冶tc玎
                                                                                  U


                                 Stage 2




    \ mL
    1, liii. 2, 3 : Searcher 丑nergy 임 계 치
    2. FTh : Finger Energy 임계치



                                       （그림 4-35) 상태도


 I如ell 또는 Ve市y Window에서 False Alarm이 발생했을 경우 다음 탐색위치
는 가장 최근의 Detect Window의 마지막 위치（C）가 퇸다．


                    Detect Window (64칩)      -    Next detect Window




                            띠口     卜

           탐색시작        Ver fy Window [6칩)
            지점

                             （그림 4-36) Searchin（그 Window들
    4. CDMA Demodulator                                                                     223
.



       Ct state

    Detect State에서는 주어진 \?Vindow size(64칩）에 대해 탐색을 명령한 후 dump
面ne interrupt를 기다린다. 만약 max energy가 T뇨eshold 보다 큰 Pilot O卄set
을 찾았으면 그 위치로 Finger Slewing시키고, 그 옵셋을 중심으로 새로운
Wind이V（이 \Vindow는 detect Window어］ 비해서 훨씬 작게 잡는다.）를 만들어 탐
색을 다시 명령한다. 그리고 Dwell state로 간다. 또 소프트웨어는 이 state어］ 있는
동안 Searcher가 전체 PNRo끄을 다 검사했는지를 che吐한 후 한 PN Roll어］ 대한
탐색이 끝났으면 다음 state의 Parameter를 load한 후 state 천이를 한다.




          다옴 state의 파라매터를 loading하       H/w에서 detect state의 쟤어
          고 다음 state의 detect state 탐색    파라메터를 읽어온다．
          올 시작．
                                                    4
                                              탐색을 시작한다

                                                    中
                                        DUId甲 DONE interrupt를 기다린다．

                                                    4                     Searcher
                                         Se可cher로부터 탐색결과를 읽옴．
                                                                          Energy
              Time Tracking                                               Threshold   "
              올 Enable




                        V                                                       V
            최대 에너지 값이 얻어진 옵샛으로                                        앞선 탐색창의 최종위치로 모든
            모든 Finger를 정열．                                            텨nger롤 정렬


                         V                                                      V
            최대 에너지 값이 좁은 창의 중앙이                                       다음의 Detect 창을 위해서 다
            되 게 Searcher릍 없ew.                                        시 탐색을 전송


                     V                                                           V
            다음 탐색을 위해서 1沁eli 파라메                                        Detect state로 이동
            터를 load


                          V
                 小sell state로 이동


                                    （그림 午37) Detect 없ate
   224                                                             4. CDMA Demodulator
                                                                                         U




 Verify State

 Verify 상태에서는 Searcher가 찾은 Pu毗의 에너지뿐 아니라 Fii坦er가 계산한
에너지를 고려한 Eva1uation을 한다. 또Dr야） Cou砒er를 두어서 Searcher 에너지
가 작더라도 入4aximum Drop Counter만큼 같은 Window를 반복해서 탐색할 수
있도록 했다. 갇은 \Vindow를 다시 탐색하기 전 \?Vindow를 조정하는데 이때 조정
하는＼사in面w의 크기는 1 칩 내외로 한다.
 이렇게 해서 최대 에너지가 임계치보다 작고 dr야）Counter가 岫xdr야）Counter
보다 큰 경우만 다시 detect state로 돌아간다．

                     verify state 시작



                  네w에서 verify state의 쟤어
                  파라메터를 읽어온다．



                  以끄dP DONE interrupt를 71
                  다린다．



                  Searcher와 Finger로부터 탐      Searcher
                  색 결과를 읽욤．
                                             Energy
                                             Threshold
          drop+
                      max_eng> verify_ J
                            由?




                           drop>
                         max drop?
                                                   RSSI>
                                                  꺄n只 th?

                  Detect 파라매터를 load하
                  고 앞의 Detect 창의 마지막                                최대 에너지를 찾은 지점
                  위치로 Searcher와 Finger                              으로 Finger를 引ew 한
                  률 듸ew한다．                                          다．
                                            주파수error와 old 주파
                                            수 에러를 읽는다．

                    Detect state로 이동

                                             Pull 1ll state로 이 동

                         Combiner로부터
                         주파수추적 누적치
                         를 취함．


                          （그림 4-39) Verify State
    4. CDMA Demodulator
口



       1 state

 Dwe끄 상태에서는 Detect 상태에서 찾은 위치어］ Fir坦er를 이동시킨 후 진행된
탐색이 끝나기를 기다린다. 즉 dump done inte玎upt를 기다린다. detect상태와 마
찬가지로 탐색결과와 위치도 조정한 다음 다시 탐색을 명령한 후 verify 상태로 간
다. 이때, Fir坦er의 RSSI register를 초기화한다. 이 값은 다음 상태에서 탐색결과
를 evaluate하는데 사용된다． 물론 이 상태에서도 Searcher가 찾은 최대 에너지가
임계치보다 작을 경우 dete毗상태로 돌아간다．


                                     小well state 시작


                                          V
                                  HIW에서 Dwell state의 제어
                                  파라메터를 읽어온다．


                                             V
                                DUMP DONE interrupt를 기다린다．


                                            V
                                 Searcher로부터 탐색 결과를 읽음．
                                                                Searcher
                                                                Energy
                                                                Threshold




                     V                                               V
         새로운 최대 에너지 위치로 모든                                   Detect 파라메터를 load
         Finger를 정렬한다．

                                                                       V
                     V                                    앞선 Detect창의 마지막 위치로
         Searcher를 듸ew하고 탐색 창을                            Searcher룔 Slew함．
         조절한다．

                                                                      V
                   V                                         Detect state로 이동
                                         Combiner어｝서
         최대 에너지 위치에 sweep의 중앙
         올 프로그램 한다．                      주파수 추적올
                                         하기위해서
                                         Fit培er가 주파
                     V                   수 에러를 계산1
         모든Finger를 Lock시킴（주파수 추h 1       하는       것을
         적을 enable)                      enable함


                      V
             Verify state로 이동


                                （그림 午38) Dwet State
   226                                                                                 4. CDMA Demodulator
                                                                                                             U


 Searcher 에너지뿐만 아니라 까nger의 RSSI값도 임계치보다 큰 경우 I乂ill in
state로 넘어가는데, 이때 Frequency error을 읽어 다음 state어］서 Frequl巴1cy의
stable함을 evaluation할 때 사용한다．


 Pull In State

 Pull In상태에서는 주파수의 안정함을 check한다. DUMP DONE interi끄pt 이후
에 Searcher의 최대 에너지값을 비교한 다음, 그 값이 임계치 값보다 크면
Frequency error accumul毗아의 값을 새로 읽는다. 그리고 그 값과 이전 state에서
읽었던 값의 차이를 계산한 후 정하찐 임계치보다 작은가를 검사한다. 이 값이 임계


                                [Pull_        In
                                                    state   .   1작


                               H/w에서 pull in state의 제어
                               파라메터를 읽어온다．



                               1乂IMP DONE intern!야를 기
         최대 에너지를 찾은 지점         다린다．
         이 다음 탐색 창의 중앙이
         되 게 Searcher룰 S旭w 한
         다．
                               Searcher와 Con由iner로부터
                                                                     Searcher
                               결과를 읽음．
                                                                     Energy    ,.
                                                                     Threshold    /

                drop+
                                          ma凡eng > pall in山
                                               th?




                                               drop>
                                             max_drop?
                                                                     Combiner에서 주파
                                                                     수 에러를 읽고 예전       Combiner
                                                                     주파수 에러와 비교        에서 세긍
                               Detect 파라메터를 load하
                                                                                       된 값
                               고 앞의 Detect 창의 마지막
                               위치로 Searcher와 Finger
                               릍 引ew한다．
                                                                        Is Frequency
                                                                            stable?

                                         Detect state로 이동                      Y
                                                                                       최대 에너자를 찾은 지점
                                                                     채널 복조 상태로 이동      이 다음 탐색 창의 중앙이
                                                   Pilot                               되게 Se可cher를 Slew 한
                                                   Chann아을                             다．
                                                   찾은 상태



                                            （그림 小40) Pull-In State
         4. CDMA Demodulator
     口                                                                    227


치보다 작을 경우 이 상태가 Pilot을 획득한 상태인 것이고, 즉 지금 현재 수신하고
있는 Pilot 신호의 주파수 튜닝된 위상정보를 정확하게 알게 되어서 국부 PN Code
발생기로부터 신호를 만들 수 있고 따라서 sync Channel을 복조할 수 있는 상태이
다．
     만약 Frequency error의 de岫값이 임계치보다 크더라도 마찬가지로 drop
Cou砒er를 이용해서 최대값만큼 재시도를 할 수 있다．
     I뇨II in state이후 Searcher Softw可e는 동기채널이 복조되기를 기다린다. 동기
채널이 복조된 다음에는 동기채널로부터 얻은 system Timing정보를 이용하여 단
말기의 내부Clock（혹은 시계）를 시스템 시간어］ 맞춘 후 호출채널을 감시한다


     각 상태에서 HIM／으1 동작
     각 상태에서 HiW의 동작을 요약하면 다음의 （표 4-3）와 같다．
     여기에서 주의할 것은 detect와 dwell상태에서는 Searcher로부터 최대 에너지


                               （표 4-3) 하드웨어의 상태별 동작

         상태           Searcher               Hnger                （力mdner
               (B Search Window에 있
                  는 각각의 옵셋의 에너
                  지를 측정한다．
     Detect    (2) Search Window 중에 동작 없음                    동작 없음
                  서 최대에너지를 찾는다．
               (3) 최대 에너지와 그것의
                  위치를 보고한다．

                                     (l) T油e 추적되고 있는
                                       RSSI를 구한다．
     Dwell     위의 동작을 계속                                     동작 없음
                                     (2) Frequency err야를 구
                                       한다．
                                                             (B Frequency e寸or을 구
     Verify    위의 동작을 계속             위의 동작을 계속한다．              하고 그것을 보고한다．
                                                             (2 Frequency 추적한다．
     Pull hi   위의 동작을 계속             위의 동작을 계속               위의 동작을 계속
   228                                     4. CDMA Demod미atc汗
                                                                U


및 그것이 측정된 위치가 제공되고, Verify 상태에서는 이러한 Searcher 정보는 물
론 Finger의 RSSI 값까지 제공된다. 또한 I뇨11 in 상태에서는 이러한 Searcher정보
와 Coi油iner의 Frequency Error Accumulation이 제공된다．
                                         229
                                               1




                                   전력제어




 복잡한 거리에서 휴대전화기로 전화를 할 때 우리는 나 자신도 모르게 소리 높여
서 이야기한다. 또한 조용한 실내에서 귀어］ 이어폰을 꼽고 있는 사람에게 말을 걸면
그 사람이 비정상적으로 큰 소리로 이야기하는 것을 종종 본다．
 이러한 것들은 모두 자신이 느끼고（듣고） 있는 감각어］ 의해서 행동하는 것이다．
즉 이러한 메커니즘은 자신에게 입력된 신호에 대응하여 출력신호를 결정하는 일종
의 피드백 시스템인 것이다. 또한 그 응답은 입력과 선형적인 관계를 맺고 있다．
 이러한 일련의 처리절차와 동일하게 CDMA에서는 그것의 출력을 제어하는 전력
제어를 수행한다. 앞으로 공부하겠지만 이러한 전력제어가 시스템의 성능을 결정한
다는 측면에서 CD八心＼시스템이 기존의 다른 시스템과는 달리 시스템의 진단기능까
지 가지고 있다고 생각할 수도 있다.



 5.1 오H 전력제어를 해야 하는가？
                                               )
 CDMA시스템은 지금까지의 다른 시스템과는 전혀 달리 주파수 자원을 효율적으
                                                       5. 전력제어
      230                                                        1



로 사용해서 용량증대를 이루어야 한다는 강박관념을 탈피한 시스템으로 또 다른
자원의 사용과 분배가 필요하다. 이 내용에 대해서는 앞서 3장에서 충분히 언급이
되었O 口로 추가적인 이야기는 하지 않겠다. 다만 기존의 Spectr비［n Band limited
이던 시스템과는 달리 전력 Limited 시스템인 CDMA에서는 匐玭trum Band를 효
과적으로 나누어 쓰는 것만큼 알맞은 전력의 분배가 시스템의 용량 등과 같은 성능
어］ 상당히 중요하다. 때문어］ 잘 수행된 전력제어는 우수한 CDMA를 만드는 초석이
된다고 할 수 있다．
 전력제어의 최우선의 목표는 단말기가 처하1 있는 상황에서 최적의 전력을 할당하
는 것이다. 이 ' 최적'이라 함은 ' 최소'라는 의미와 무관하지 않다. 예를 들어서 RF상
황이 좋지 않은 단말기가（즉 현재 상당히 강한 Forward 전력을 할당받고 있는 상
태의 단말기） 좀더 강한 신호로 신호전송을 해줄 것을 계속 요구한다면 이러한 요
구는 추가적인 전력할당을 하기 보다는 다른 양호한 단말기들의 출력을 위해서 호
자체를 끊는 방법을 택하는 것이다. 이것은 특정한 단말기에 최소의 전력 이상을 저］
공하는 것은 다른 단말기에 간섭이 증가될 수 있는 또 다른 요인이 될 수 있기 때문
이다. 즉 적당한 전력을 소모하는 범위에서 최대 혹은 최소의 전력이라는 개념이 있
을 수 있는 것이다. 이것은 마치 범법자를 징역형에 처하는 사회 시스템과 유사하다
고 볼 수 있다. 이런 의미에서 이 시스템은 상당히 이성적인 시스템이라고 할 수 있
다．
 전력제어는 크거］ Open Loop, Closed Loop, Outer Loop로 구성되며, 이것들은
각각 Near Far, 瓦／N0, FER어］ 의해서 구상되어진 채널환경을 보상하기 위해서
이루어진다．
  또한 IS앉)에서는 이러한 전력제어보다 훨씬 느리게 진행되는 전력제어를 Forward
Link 쪽어］ 적용하고 있는더］ 이것들은 FER의 통계정보를 가지고 layer3의 Signaling
으로 처리되기도 하며, EIB(Erase Indicator Bit), QIB(Qu싫ity Indicator B北）를 사
용하여 Frame 단위로 이루어지는 전력제어를 병행해서 수행하기도 한다．



     5.2 어떻7카 전력제어를 하며 어떤 종류가 있는가？

     CDMA 시스템의 전력제어는 개루프（Open Loop）와 폐루프（Closed Loop) 같은
 U                                                                        231

내부 루프（Inner Loop) 전력제어가 있고, 기지국 제어기의 Vocoder까지 그것의 영
역이 확장되는 외부루프幻uter Loop) 전력제어가 있다．
 （그림 5-1）은 전력제어의 전체를 나타낸 것이다. 일반적으로 전력제어는 원근 문
제로 인한 전력을 보상해 주기 위한 0pen Loop 추정어］ 의한 전력제어의 초기값 설
정이 있으며, 이러한 초기값 설정을 바탕으로 계속적인 채널변동 상황을 반영하여
수시로 보상하1 주는 Closed Loop Power Contr아（보상）가 있다. 또한 Closed Loop
의 T뇨eshold를 효과적으로 갱신하기 위해서 이루어지는 Outer Loop Power
Control가 있다．



            Base Station                            Mobile Station



                            Va nab Ic
                           XMIT HPA

                                                           Dei nterleaver
                                                            & Decoder




                                         Variable
                                        XMIT HPA

                                                            1nterieaver
                                                            & Encoder

                      （그림 5-1) 전력제어의 개요

 Closed Loop Power Control는 그것의 판단기준이 Searcher와 Fir瑠er에서 수신
한 신호의 瓦屈의 값에 의해서 이루어지며, Outer Loop Power Contr이는 Closed
Loop Power Control와는 달리 FER에 근거하여 현재 설정되어 있는 Closed Loop
Power Control의 임계치가 타당한가를 판단하여 갱신하는 것이다．
 따라서 （그림 5-1）의 그림과 같은 전력제어는 초기의 0pen Loop전력제어로 시
 =
작되며, 거기에서 설정된 값으로 수신 Bit（혹은 CDMA에서는 칩이라고도 함．) 신호
의 신호 대 잡음비에 근거하여 （그osed Loop Power Control를 1.25ms마다 하며，
이러한 전력제어의 임계치는 복조가 끝나고 \/（兀oder Frame 단계에서 Error 검증
단계에서 2劤'is마다 Frame error Rate어］ 근거하여 갱신한다．
 이것은 마치 시계의 작은 침（시침）과 긴 침（분침）의 움직임과 유사하다. 즉 시침
과 분침은 그 움직임이 12:1이나 이러한 전력제어의 주기는 16:1로 이루어진다.
 이상적인 전력제어는 각각의 단말기가 느끼고 있는 채널환경을 완벽하게 보상하1
주는 것이 문제의 해결이 되나 중요한 것은 채널환경을 완벽하게 모델링할 수 없다
는 것이 문제가 될 것이다．
 우리가 사용하고 있는 CDMA 채널의 경우 800bps의 전력제어 Bit를 1.25ms길
이의 전력제어 그룹으로 전송되고 있으며 이것은 결국은 800Hz정도로 변경되는 채
널 전력을 보상한다는 말이고 때문어］ 800Hz보다 빠른 Fading어］ 대해서는 보상이
되지 않는다는 이야기다．


            Po＼以｝r


                        재널의 변동상황


                                   이상적인 전력세어
                                    의 결과 출력

                      이상적인 전력졔어

                                    t

                     （그림 5-2) 이상적인 전력제어


   5.2.1 Forward 전력제어

 CI呱4A 시스템에서 채널자원이라는 것은 결국 전력이 되므로 채널자원을 관리하
는 기지국의 입장에서는 Forw可d 전력제어를 통해서 알맞은 전력배븐이 필요하다．
이러한 기본입장에서 기지국은 임의의 Forw針d CDMA 채녈의 전력을 제한하고
있다. 이것은 임의의 Forward CDMA 채널이 규정된 전력 이상을 사용할 경우 다
른 셀 또는 섹터어］ 대한 간섭이 커지게 되며, 이것으로 인해서 전체시스템의 용량이
떨어지는 효과를 초래할 수 있다. 또한 이렇게 비정상적으로 전력할당을 하게 되는
                                                     233


상황은 그러한 전력을 할당받는 단말기도 양호한 서비스를 유지하는 경우가 드문
것이 대부분이다. 따라서, Forward CDMA 채널의 전력이 포화되지 않도록 관리해
야 한다. 이를 위해 針luffle down 과 cell shrink 등의 방법을 쓰며, 이에 대한 관리
는 기지국 상위단에서 이루어진다．
 Forward CI呱'Il\ 채널의 전력은 기지국에 따라 일정량이 지정되어 있으며, 이 전
력을 P11毗 채널, 동기채널, 지원되는 호출채널, 그리고 모든 통화채널（통화채널）이
공유한다． 각 단말기의 위치에 따라 기지국에서 단말기까지의 전송 손실이 다르기
때문어］ 기지국은 각 단말기마다 충분한 크기의 신호가 전달될 수 있도록 해야 한다．
이를 위해 기지국은 각 통화채널의 전력 할당분을 필요어］ 따라 변화시킨다. 한번의
전력제어어꺼 전력량의 변화 범위는 공칭점（nominal po血t）을 중심으로 十4dB 정
모기다．
 모든 채널에는 7 Bit의 小gital gain이 주어져 있으며, 각 채널의 전송전력은 이
小gital gain의 제곱어］ 비례한다. Forw可d 링크 전력제어는 주로 Forw可d 통화차1
널어］ 대해서 이루어진다． 그 이유는 I꾜야 채널, 동기채널, 그리고 호출채널의 경우
는 결국 신호의 도달 범위가 항상 기지국의 전서비스 지역이어야 하기 때문이다．
 Forw可d의 전력제어 과정은 다음의 두 단계로 이루어진다. 첫 단계에서는（단말
기로부터의 수신전력을 사용하여）Forw可d 링크의 전송손실을 공칭 gain으로 설정
한다. 두 번째는 단말기와 함께 지속적으로 小gital gain 을 조정하는 단계이다
(Closed Loop). 즉 기지국은 단말기가 보고하는 Frame 에러율 통계（Frame error
rate stat始如S）를 사용하여 해당 통화채널의 전력을 올리거나 내린다. 그러나 계속
적인 전력 증폭으로 포화상태가 되지 않도록, 즉 Forward CI呱4A 채널의 전력이
규정된 값을 넘지 않도록 해야 한다．
 기지국에서 단말기로 송출되는 전력을 제어하는 Forward 링크 전력제어
(Forw町（I Link 전력제어）는 기지국이 각 Code Channel의 digital gain 을 조정함
으로써 이루어진다． 각 Code Channel의 전송전력은 이 digital gain 의 제곱어］ 비
례하게 퇸다．


   5.2.2 Reverse 전력졔四I

 Reverse 전력제어는 Forward 링크로 이루어지며, 단말기의 위치변화어］ 따라 단
말기에서 기지국까지의 전파손실（propagati아I loss）이 대부분 다르고 여기어］ 이동
   234



통신 채널상의 Fading어］ 의해서 감쇄되는 신호를 적절히 보상해 주는 전력제어를
하지 못할 경우 요구되는 통화의 질（quality）을 기대할 수 없다．
 Reverse 전력제어의 경우 CI呱TA의 Reverse 링크의 Reverse 용량을 결정짓는
요인이며, 이것은 Forw可d 전력제어가 Forw可d 용량을 결정짓는 요인인 것과 같
은 이유이다．
 Is-的의 경우 일반적으로 Forw可d보다 빠르고 정교한 전력제어를 한다．
Reverse은 cdma2(X刃이전에는 N이i Coherent한 링크였다. 따라서 적절한 전력 소
모보다는 좀더 많은 전력을 소모함으로 운영되어온 링크였다. 즉 상대적으로
Forward보다 훨씬 많은 전력이 사용될 가능성이 높은 시스템이다. 이러한 이유로 더
빠른 전력제어가 Reverse에서 이루어졌다. 실지로 Reverse 전력제어의 resolution은
1.25ms인데 반해서 Forward 전력제어는 최소 20msec정도어］ 불과했다．



 5.3 이통 통신 채넘 특징

 통신에 필요한 송신전력이나 서비스 구역의 크기, 서비스 구역내의 통신품질 등
을 결정하는 것이 전자파 전파（Propagation) 특성이고, 송신기에서 수신기까지의
전파손실이나 전파손실의 장소적, 시간적 변동 등이 주요한 요소가 된다. 이동 통신
의 전자파 전파 경로는 송신 점에서 방해 없이 도달하는 직접파, 건물의 벽 등으로
인한 반사를 거쳐서 도달하는 반사파, 건물의 옥상 등에서 회절하여 도달하는 회절
파 등 3종류의 전자파가 수신점에서 수신된다．
 이들 각각의 전파 레벨은 이론적인 취급이 가능하다. 그러나 이동전화 등과 같이
송수신점 간어］ 거의 직접파가 없이 다수의 반사파나 회절파가 수신되는 경우, 이들
모튼 전파를 이론적으로 검토하는 것은 사실상 불가능하기 때문어］ 전자파 전파 특
성의 기술에는 측정 데이터의 통계처리어］ 의한 실험식 등이 쓰이고 있다. 따라서 사
용자의 이동성, 기지국 설계 및 주변환경어］ 의해서 형성되는 전자파 전파 채널은 동
일 주파수 재사용으로 인한 다른 기지국의 간섭으로부터 충분한 격리방법을 제공하
여야할 뿐만 아니라 그 기지국 내 서비스를 위한 고품질 전송방법을 제공해야 한다．
 용량이 크게 요구되는 인구밀도 지역은 컨물, 인공 조형물, 나무 등과 같이 전송
경로를 가로막는 장애물들로 꽉차 있으며, 이러한 장애물들로 인한 과다손실은 다
른 셀들과의 필요한 격리를 얻는데 이용되고 있다. 장애물들로 꽉찬 비교적 작은 셀
    5 . 전력제어
                                                  2i5
1


권역 내에서의 전자파 전파는 기지국과 단말기 안테나 주변 구조물로부터의 반사와
산란어］ 의해서 지배된다. 모든 방향으로부터의 도착신호를 수신하는 전방향 안테나
는 어려운 전자파 전파환경어］ 있는 환경어］ 있는 단말기어］ 효과적으로 쓰인다. 그러
나 이동통신 방식에는 기지국 안테나의 지향성어］ 제한이 있어 지상 근접 구조물 전
체가 산란 및 반사를 하게 되어 기지국과 단말기 사이어］ 다중 경로를 제공한다．
    이동통신의 주요 채널은 다음과 같다．

     5.3.1 Fading

    수신 전계 강도가 둘 이상의 경로를 달리하는 전파간의 간섭 또는 전파경로의 상
태변화 등어］ 의해서 시간적으로 변하는 현상을 페이딩이라 한다. 페이딩은 짧은 시
간 구간 동안 빠르게 변하는 단구간 페이딩과 긴 시간 구간어］ 컬쳐 느리게 변화하는
장구간 페이딩으로 대별할 수 있다. 단구간 페이딩（Short Term Fading）은 빠른 페
이딩（Fast Fading）이라고도 부르는데, 이는 단구간 페이딩이 기지국과 단말기 사이
의 장애물로 인한 전자파의 반사 등의 영향어］ 의해 경로길이의 차가 달라지거나 단
말기가 이동하기 때문어］ 생기는 도플러 효과어］ 의하여 페이딩이 빠른 율로 발생하
기 때문이다．
    이러한 페이딩은 랜덤하게 발생되는 값이므로 일반적으로 그것을 표현하기 위해
서는 확률 분포함수를 사용하며, 이 값은 그것의 지형 지물 등어］ 대한 제한적 요인
들을 가정한 가운데 표시하는 것이 일반적이다.
    단일경로가 아닌 다중경로 때문어］ 발생하는 단구간 Fading은 송신점에서 방해
없이 도달하는 직접파, 컨물의 벽으로 인한 반사를 거쳐서 도달하는 반사파, 컨물
의 옥상 등에서 회절하여 도달하는 회절파 등으로 구성되는데 이동통신 채널에서
는 직접파의 성분이 거의 없고 주로 반사파나 회절파들로 구성되므로 수신점에서
의 수신 전계 강도의 진폭 및 위상이 레일리 확률분포함수를 따르기 때문어］
Rayleigh Fa小ng이라고 부른다.
    그러나 위성통신 채널에서는 직접파의 성분이 상대적으로 강하므로 수신점에서
의 수신 전꼐 강도의 진폭 및 위상이 라이시안 확률분포함수를 따르기 때문어］
Rician Fading이라고도 부른다．
    장구간 Fading(long term Fading）은 주어진 기지국과 단말기 사이의 거리 안어］
서 단말기가 그 주변으로 이동할 때 지형의 변화로 인해 발생하는 Fading으로서 느
   236



린 페이딩율을 가지기 때문어］ 느린 Fading(slow Fading）이라고도 부른다. 또한 장
구간 Fa小ng은 수신 전계 강도의 변화가 log-normal확률분포함수를 따르기 때문
에 log-normal Fa小ng이라고도 부른다．


   5.3.2 Delay Spread

 이동 통신 채널을 통하여 디지털 신호를 수신할 때는 전파경로의 길이가 다른 다
중경로 전파현상 때문어］, 각 경로를 따른 신호가 수신기어］ 동시어］ 도달되지 않는다．
이렇게 한 신호가 여러 경로를 통하여 수신시간 지연이 달라지는 현상을 지연확산
이라고 한다. 이 도달 시간의 차이가 수신데이터 심볼간의 간섭(ISI: J砒町Symbol
Interference）을 일으켜 수신기가 데이터를 정확하게 복원하는 것을 어렵게 만든다．
 또한 여러 경로를 통하여 수신된 신호들은 시간 영역에서 확산되므로 주파수가
선택적（frequency selective）이다. 즉 주파수가 다른 두 신호가 동일한 다중경로로
수신되었어도 각기 파장어］ 대한 상대적인 크기들이 다르기 때문어］ 그 페이딩 특성
이 같지 않다. 상관콴계가 거의 없는 Fading을 갖는 주파수 간격을 coherence 대역
폭이라 하며, 도심지에서는 대략 100- 300KI七정도이다. 그러므로 송신신호의 점유
대역폭이 coherence 대역폭을 넘게 되면 주파수 선택적 Fading이 문제가 된다．
coherence 대역폭과 지연확산은 반비례하며, 도심지에서의 지연확산이 대략 十10
PS정도이므로 등화기를 쓰지 않는다면 전송속도가 제한된다．


  5.3.3 Doppler Spread

 다중경로 전파현상과 이동체의 움직임 때문어］ 이동통신 채널을 통하여 디지털 신
호를 수신할 때는 전파경로의 입사각이 다른 신호가 수신기어］ 도달된다. 이렇게 한
신호가 여러 입사각을 통하여 수신되므로 수신신호 주파수가 변하는 현상을 도플러
확산이라고 한다. 또한 여러 경로를 통하여 다른 입사각도로 수신퇸 신호들은 주파
수 영역에서 확산되므로 시간선택적（time selective) Fading이라고 한다. 도플러 확
산어］ 의한 주파수 변화를 포플러 편이（Doppler shift）라고 한다. 이 도플러 편이는
이동체의 속도어］ 비례한다. 예를 들면 20001V11七에서 시속 100Km로 달리는 경우의
도플러 편이는 대략 185Hz어］ 퍼져 있게 된다. 도플러 편이는 이동체가 사용하는 반
송파의 주파수에도 비례하므로 복잡한 신호처리 기법을 사용하지 않으면 이동체의
최대 이동속도가 제한된다．
                                                  237


   5.3.4 음영현상（Shado的지）

 이동통신 채널을 통하여 디지털 신호를 수신할 때는 단말기가 기지국의 주변으로
이동할 때 전파경로가 큰 컨물이나 언덕 등어］ 의해 가려져 일시적으로 수신 전계
강도의 변화가 발생하게 된다. 음영현상은 이렇게 장애물어］ 의해 발생하는 Fading
으로써 느린 페이딩률을 가지기 때문어］ 느린 Fadir垠이라고 부른다. 또한 음영현상
은 수신 전계 강도의 변화가 Log-Normal 확률분포함수를 따르므로 log-normal
Fading이라고 부른다. 따라서 이동통신 시스템을 설계할 때는 지형의 변화도 고려
하여야 한다．


   5.3.5 인접채널 및 동일채널 간섭

 이동통신에서 인접채널에서 작동중인 이동체 간의 송신기와 수신기의 상대적인
위치가 가까워지면 간섭이 일어날 수 있다. 이렇게 단말기의 이동어］ 따라서 인접
채널 송신기로부터 발생하는 간섭을 인접채널 간섭（ACI : A데acent Channel
I砒erferei兀e）이라 한다. 이러한 인접채널간섭은 가급적 인접한 셀들을 이용하는 반
송파 주파수차이가 많이 나도록 셀을 설계하여야 하며, 수신기의 선택도가 아주 높
아야 한다． 이동통신 시스템에서는 인접채널 간섭 외에도 같은 셀 내에서 주파수가
재사용되므로 수신기의 선택도어］ 상관없이 간섭이 일어날 수 있다. 이러한 간섭을
동일채널 간섭（CCI: Co-Channel Interference）이라고 한다. 이러한 동일채널 간섭
은 셀룰러 이동통신 시스템의 용량을 결정하는 중요한 요인이 되므로 지향성을 가
진 안테나들을 여러 개 사용하는 섹티화로 해결하고 있다．


   5.3.8 경로 촌실（Path loss)

 이동통신 시스템에서는 수신전력 감쇠를 수반하게 된다. 자유공간에서는 전파신
호의 수신전력이 송수신 거리의 자승의 관계로 감쇠하지만 이동통신 채널에서는 일
반적으로 감쇠율이 十4승 사이에서 비례한다고 알려져 있다. 이 수신전력 감쇠를
경로손실이라고 한다. 이 경로손실은 지역에 따라 다르며 도심지와 같은 복잡한 지
역일수록 감쇠율이 높은 것이 일반적이다. 따라서 도심지에서는 경로손실을 보상하
기 위하여 상대적으로 강력한 송신출력이 필요하다．
   238




 5.4 0pen Loop Power Control                             )
 직관적으로 멀리 있는 단말기에는 가까이 있는 단말기보다 강한 세기로 신호를
송출해야만 통신이 잘될 것이라는 것을 우리는 짐작할 수 있다. 이것은 강한 세기로
출력해야만이 더 먼 거리어］ 있는 단말기까지 전달될 것이라는 즉 경로손실을 보상
해야만이 먼 거리까지 도달될 것이라는 것을 우리는 알 수 있다. 이렇듯 전파음영
(shadowing）과 거리감쇠（Nea卜F出 문제를 보상하는 절차가 필요하며, 이러한 것
을 해결하기 위한 것이 Open Loop Power Control 이다．
 Open Loop Power Control는 단말기가 호 /\ccess 과정에서 기지국으로부터의
수신전력에 따라서 단말기의 출력을 송출하는 것이다. 여기서는 Turn Around
Factor k를 이용하는데 Turn／뇨ound Factor k에는 기지국 송신전력과 기지국 수
신 Ew'N 값이 포함되어 있다. 따라서 단말기의 수신전력으로 恥rw可d 경로감쇄를
추측할 수 있고 이를 Reverse 경로감에 예측치로 이용한다. 또한 E1/ 됴값을 기준으
로 Noise성분보다 일정 수준 더 높은 전력을 단말기가 송출하도록 한다．
 그러나 이 방법은 단말기가 수신한 신호의 세기를 측정하여 송신출력을 측정할
때 FDD시스템에서는 Tx와 fix 대역의 주파수 간격이 Coherent Bandwidth를 초
과할 때는 문제가 될 수 있다.
 Open Loop의 기본법칙은 다음과 같다．
         Tx[dBm} = k - Rx[dBm]                   (5-1)

 즉 수신신호는 원래 송신신호에서 경로손실을 뺀 나머지 신호라는 것이다. 다시
말하면, 송신한 신호와 다시 돌아올 신호를 더하면 turn around fact아인 K가 퇸다
는 것이다. 이러한 관계는 식 行1）을 말하며, 이러한 상수 K는 다음의 식 (5-기로
구해진다．


         k＝尸‘134+N月巴介lOlog(1+針c2) 1010g(1 x)     (5-2)
 여기어］서
 永 Pt : 切ta1BS 전력 /＼八'IF. Output
 半 NFC : 기지국 수신기 Noise Figure
 水 ;l : 타 셀로부터 수신퇸 전력과 단말기가 속한 셀로부터 수신된 전력의 비
  5 . 전력제어
                                                                                                                   239
11



 永 :2 : thermal noi配와 단말기가 속한 셀로부터 수신된 전력의 비
 * X : cell loading
 이상과 같은 절차로 turn around factor k의 값을 구하면 8001V11七대의 셀룰러의
경우 73이며, 1.8GHz대의 Pcs의 경우 76 정도가 퇸다．

   5.4.1 추정된 Access 출력

 단말기가 기지국에（좀더 정확히 말하면 망） 접속을 초기어］ 시도할 때 나름대로의
접속을 위한 출력어］ 대한 기준을 가지고 접속시도가 있어야 한다. 이러한 과정이 개
루프 전력제어어］ 의하서 결정되며, 이렇게 결정이 정의된 출력은 구체적으로
Access Probe라는 신호 덩어리로 기지국으로 전송이 된다. 물론 이 신호의 내부에
는 /\ccess와 관련된 정보들이 포함되어서 전송될 것이다．

                                                       Access Attempt
       Response      Access probe                                                 Seq. MAX_RE S_SEQ
        Attempt       Sequence 1    Seq. 2           Seq. 3         Seq 4               (iS max)




                         11                                                                       il        ,
                                                         ,RS   J1
                                                                                              System time


                                                     Access Attempt
       Request                                                                                         1
                     Access probe                                                   Seq.MAX_RE Q_S E Q
       Attemj此        Sequence 1             Seq 2                   Seq 3               (15 max



                        II                                            II
                                                                                                  卄！    ,
                  卜I- PD늬 (RS斗PD +                                                            System time



       .     . t1             Requestmessag쓰沙啣
       /i譽e88rroue 尸尸寸／十 /1                                                      Access PrsbE
         己equenuto
                                                                                1+NUM STEP
                                                                                   (16 max)


                                                                             Access Probe 4




                                                                                                           ystem
                              Selects Access 채널 (RA) initializes transmission 전력                           Time


                    （그림 5-3) Access A卄em아와 Access Probe
   240                                          5 . 전력제어
                                                           1


 이러한 /\ccess는 （그림 5-3）과 같이 이루어진다. 이러한 /\ccess 과정어］ 대해서
는 8장에서 좀더 공부하도록 하자. 다만 여기에서는 이러한 /\ccess Probe들의 전
력 관리와 관련된 이야기를 주로 진행하겠다．
 （그림 5-3）어］ 나타난 것과 같이 단말기는 /\ccess Probe라는 /\ccess를 위한 가
장 기본 형태의 출력을 송출하며, 이러한 Access Probe는 일정한 양만큼의 전력을
증가하게 된다． 이렇게 단순히 특정한 전력을 추가하여 다음 Probe의 출력전력을
결정하는 형태는 여기서 설명하는 개루프 전력제어가 시간어］ 대해서 채널환경이 급
변하는 혹은 변하게 하는 다중경로를 보상하1 주는 전력제어가 아니라 시간과는 전
혀 무관하게 현재 단말기의 위치와 관련된 부분, 즉 Nea卜Far를 보상해 주는 전력
제어를 한다고 이야기할 수 있는 근거가 된다. 좀더 쉽게 이야기하면 전력을 단순히
증가한다는 이야기는 현재 있는 위치에서 충분히 기지국어］ 도달할 수 있는 출력을
찾기 위해서 행해지는 절차이다. 여기서 주의할 것은 이러한 Access 상황이든 통화
로가 열려서 폐루프 전력제어를 하고 있는 상황이튼 다중경로로 인한 페이딩 환경
은 언제나 존재한다는 것이다.
 이러한 Access Probe들은 Access Sequence로 하나의 무리가 지워지며, Access
Sequence들간에는 동일한 형태의 접속 시도를 단순히 반복하는 과정이다. 즉
Access Sequence의 최종 Probe의 출력이상의 출력은 현재 기지국 내에서는 단말
기의 위치를 보상하1 줄 수 없는 위치어］ 있다는 망의 판단인 것이다. 즉 （좀 극단적
으로 이야기하면） 단말기가 해당 기지국의 서비스 영역밖에 존재한다고 생각하는
것이다．
 이러한 Sequence들의 모두를 /\ccess Attempt라고 한다．
 Access를 위한 전력제어를 페루프가 아닌 개루프, 즉 초기시도어］ 태한 가부（可
否） 여부어］ 대한 응답이 없는 가운데 단말기가 독자적으로 응답이 없으면 부（不）하
다고 판단하는 형태의 열려 있는 루프 형태의 전력제어로 실시한다. 이것은 요구어］
대한 응답이 없으면 연결되지 않는 것이라고 본다는 기본적인 생각이고, 때문어］ 이
러한 절차 후에 단말기는 초기어］ 추정한 자신의 위치와 /\ccess Attem姚의 대상인
기지국과의 거리를 수정하게 된다. 즉 더 먼 거리어］ 있다고 수정 추정하여 더 강한
전력으로 다음의 /\ccess Probe의 출력을 설정하게 된다．
 우리말어］ 무소식이 희소식이다라는 말이 있는데 여기에서는 무소식이면 연결이
되지 않았다는 소식이 된다. 그렇다면 얼마 동안 기다려 보고 그것이 연결되지 않았
     5 . 전력제어                                                       24 1
.

다고 생각해야 하겠느냐 라는 문제와 연결이 되지 않았을 때 얼마만큼 더 강한 출력
을 해야 되는지가 필요할 것이다．
    이러한 절차로 단말기는 초기에 망어］ Access할 때 최초의 /\ccess Probe의 출력
결정을 다음의 식 (5-읾과 같이 한다．

           평균출력전력 (仍川＝평균입력전력（a跏）-76+NOM -／기VR(dB)
                      -16NOM _PWR卜五Xli' + 1／口T_ PWR但助                    (5-3)

    위의 식에서 PWRSTEP, NOMPWR, NOM寸P＼자B뉴EXT, INITPWR는
Access Parameter어］ 규정된 값들로서 망에서 단말기어］ 제공해 주는 값들이다. 이
값들로 설정된 /\ccess Probe는 다음의 /\ccess Probe까지 TA+RT만큼 후어］
PWR_STEP만큼 전력을 증가시켜서 시도를 한다．
    Access Attempt는 Request와 Response인 경우로 나누어지며 이러한 차이는
layer 1에서는 차이가 없으나, layer 3에서 차이가 있다. 어찌되었든 첫 번째
Access I노obe Sequence에서 접속이 돠지 않으면 Response인 경우 RS만큼,
Request인 경우 RS+I力만큼 기다린 후 다시 Sequence를 시도한다. Access Probe
의 구성은 위의 그림과 같으며, 여기어］ 나오는 변수들은 다음과 같다．

                             （표 5너） Access Attempt 변수들

변수          이름                        발생                         범위        단위
          Open Loop     IP=-평균입력 전력（dBm卜76+NOM느PWR(dB卜16
    'P                                                                    dBm
         전력의 초기치        NOMHPWREXT+IMTJWR(dB)
          Persistence   지연은 지속성 시험이 통과할 때까지 slot 단위로
    PD                                                                     slot
            Delay       계속된다．
    F'    전력 증가분        PI=PWR_STEP                             0- 7       dB
         Access Channel 매 sequence 이전어］ 발생된 0과 ACCHCFIAN 임
    RA                                                          0- 31
            number      의의 값
           PN           0과 2 尸只羽且PNJ?AN- 1사이의 값으로 ESN을 사용
    RN Randomization    하여 hashing : Access Attempt 초기어］ 한번 발   0- 511     chip
          Delay         생．
           Sequence     0과 1+BKOFF사이의 임의 값 : 첫 번째 Sequence
    RS                                                          0- 16      slot
            Backoff     를 제외한 매 Sequence전에 발생
                        0과 1+PROBEeBKOFF 사이의 임의 값 : 이어서
    RT PROBE Backo打                                             0-46       slot
                        출력되는 Probe 전어］ 발생．
         Ack. Respeonse TA=80 x (2+ACC_TMO):slot 끝으로부터 시간종
    TA                                                     1以）-13鼠） ms
            timeout     료
   242


 이러한 /\ccess Probe어］ 의하써 이루어지는 Open Loop Power Contr이의 결과
는 망으로부터 Ack를 수신하면 종료되고 이러한 전력제어의 교정치 값은 Closed
Lo야） Power Control의 초기값으로 사용되게 된다．
 일반적으로 접속을 시도할 때는 전력을 P1만큼 증가시키는 것이 원칙이며, 이것
은 0pen Loop Power Con打ol가 채널환경이 시간어］ 의해서는 거의 변하지 않는다
는 기본적인 생각을 가지고 단지 초기의 /\ccess Probe 전력이 약했기에 Ack가 오
지 않았다고 가정하였기에 이러한 원칙이 성립할 수 있는 것이다. 즉 Open Loop
Po1刀er Contr아는 다중경로어］ 의한 신호의 감쇠어］ 대한 보상을 하는 것이 아니라
near-far 문제어］ 대한 해결을 위한 전력제어라고 생각할 수 있다.
 따라서 전력 증가분 P1는 초기의 전력이 /\ccess어］ 충분하기어］ 보상해 주는 전력
이라는 단순한 의미의 값이다．
 그러나 채널은 /\ccess Probe간의 시간인 TA(ms)+RT(slot) 동안 다중경로의
padding 신호어］ 의해서 수시로 변할 것이며, 이 변화는 좋아지든 나빠지든 혹은 현
상태를 유지하튼 거의 랜덤어］ 가까울 Access를 시도한다면, 초기 /\ccess시의 전력
은 채널환경어］ 비해서 대체로 강한 신호일 것이다. 이러한 현상은 P1의 값이 클수록
더욱 심화될 것이며, 이것은 access 속도와는 이율배반적인 관계가 될 것이다.



         진력
              Open Loop 추정단꼐1      이osed Loop 조정단계




                                    Access probe의 츨력을 계속
                                    증가 시켜서 망과 연결이 되딴
                                    그 값으로 폐루프 전력제어를
                                    수행 함．



                                                           time >

                （그림 5-4) O口en 匕00p와 （긔osed Loop의 연겨1


 P1가 너무 낮게 설정되면 또 한번 이상（n번）의 Probe가 있어야만이 Ack를 받을
수 있을 것이므로 n{TA(ms)+RT回ot)｝만큼의 시간지연이 있어야 할 것이며, PT가
커질수록 최고 PT만큼의 과잉전력이 필요하게 되는 것이다．
 이러한 /\ccess 절차는 이러한 요인들을 잘 고려하여 사용되어야 할 것이다．
                                                                       243

 （그림 5-4）에서 확인할 수 있는 것과 같이 /\ccess I노obe의 출력을 （상향）조정하
는 Open Loop를 통해서 연결하고 연결되면 그 값을 초기값을 하여 Closed Loop
Power Control가 시작되게 된다．

   5.4.2 개선된 Open Loop 전력 Estimation

 Open Lo야） 전력 Estimation Correction는 기지국에서 수신되고 있는 /\ccess
I斗obe의 성공 확률을 증가하게 하기 위해서 새롭게 개선된 방안이다. 단말기가 감지
하고 있는 채널환경은 그것이 대기상태어］ 있든 /\ccess 상태에 있튼 혹은 통화상태
에서 안정적으로 전력제어를 하고 있는 상황이튼 채널환경은 변화무쌍하다. 즉 단말
기가 그러한 환경어］ 적응하는 방안을 찾아야 한다. 이러한 문제어］ 대해서 Is-앉5B에
서는 구체적인 해결책들을 제시하고 있으며, 이 장에서는 전력제어에 대한 이야기를
하기로 되어 있어 개루프 전력제어와 연관된 항목어］ 대해서 이야기하겠다. 물론 또
다른 개선안인 /\ccess Handoff어］ 대해서는 6장의 Han面卄에서 공부하겠다．
 어찌되었든 초기 /\ccess Probe의 실패율을 감소시키기 위해서 개루프 전력제어
어］ Interference correction이라는 새로운 물리량을 추가해서 초기의 추정 전력어］
인접 P11毗의 간섭성분을 보상을 하1 준다는 아이디어이다．
 간섭 보정치（Interference Correction）는 현재 active set의 Pilot Ec/lo가 지나치
거］ 약해서 인접해 있는 P11야의 간섭어］ 민감해질 수 있는 부분을 보상하1 주는 값이
다. 여기에서는 그것의 임계값을 7dB로 설정해 두었다. 이러한 생각에서 간섭 보
정치 IC는 다음의 식과 갇이 정의되어진다．



       加   「「「
             「毗「Correction=   mi｛   니－
 여기에서 Ecj 는 최대 500ms앞에 측정된 Pil毗의 且／lo값이다．
                                          7＋        』］,       7]
                                                                        (5-4)




                                               Interference
                                               Correction
                 A      B             C




                                                          EC/ I0(dB1



                     （그림 5-5) Interference Correc的n
UI              I                                                  5 . 전력제어
11
     1    244   1
                                                                              .


         위의 그림에서 알 수 있듯이 간섭 보정치는 Ac如e Pilot의 세기가 -7보다 작고
     14보다 클 때 /\ctive Pu毗의 세기어］ 의해서 크기가 선형적으로 변하게 되며, 그
이하에서는 보상을 7dB 이상은 해 주지 않는다는 말이다. 이 말의 또 다른 의미는
-14dB 이하의 Pilot은 active set이라 할지라도 충분한 강도를 갖지 못하므로 의미
가 없다는 말이며, 따라서 영역A는 의미가 없는 영역인 것이다．
         또한 영역C에서의 보정값은 0으로 이때는 Ac山e Set내에 있는 Pilot의 강도가
-7dB를 초과하는 강한 신호를 수신하므로 /\ccess 채널의 신호가 주변 기지국의
간섭신호어］ 크거］ 영향을 받지 않으므로 IS-95A의 형태와 동일하게 적용되는 구간
이다. 즉 개선안의 이득을 얻을 수 없는 지역이다. 사실 이러한 개선안은 약한 Pilot
을 수신하고 있는 상태에서의 개선안이기 때문이다．
         앞서서 설명한 식 行3）의 식은 추정하는 전력 자체가 전력어］ 대한 보상치들 이
외에는 없다. 그러나 이러한 간섭 보정치를 추가한 식은 전력뿐 아니라 간섭으로 인
해서 신호의 유실되는 부분을 보상하1 줄 수 있다는 측면에서 약한, 즉 7dB이하의
Active Pu毗의 상황에서도 /\ccess 실패확률을 줄일 수 있는 방안이다.
         이러한 방식으로 했을 때 첫 번째 출력되는 /\ccess Probe는 다음과 같이 표현될
수 있다．
     mean output power(dBm) = mean input power(dBm) + offset power +

                             NOM PWR-16NOM _PWR_EXT+ INIT_PWR

                             + inter色rence correction
                                                                       (5-5)

         이러한 간섭 조정치는 새로운 /\ccess Probe가 출력될 때마다 새로운 값으로 변
 경되어서 반영된다. 따라서 식 任5）로 출력된 /\ccess Probe는 다음 번의 /\ccess
I노obe가 출력될 때는 전력 증가분인 P＼자RSTEP과 간섭 보정치의 변동성분， 그리고
 평균 입력전력의 변동성분이 합해져서 그 다음 번의 Access I노obe의 출력이 된다．



         5.5 이osed Loop Power Contr이                                              )
         단말기나 기지국어］ 의해서 전송되는 무선신호는 단말기의 위치나 속도, 또는 전
 송매질어］ 따라서 채널의 이득이나 위상 특성이 변화하는 Fading을 겪게 된다. 일반
                                                    245
                                                [

적으로 Fading은 Rayleigh Fading으로 대표되는 짧은 시간어］ 걸쳐서 나타나는 빠른
Fast Fading과 대수정규분포（Log Normal Sha面＼ving）로 대표되는 느린 Fadit坦으
로 구분할 수 있다．
 여기어］서 짧은 페이딩 혹은 느린 Fading이라는 것은 신호를 왜곡시키는 세력의
전반적인 변화율을 말한다．
 이동중인 단말기는 원근 문제로 인한 수신전력의 변화와 더불어서 다중경로
Fading어］ 의한 전력변동도 함꼐 고려되어야 한다. 이 절에서 이야기될 전력제어는
채널 상태를 측정한 후 보고하고, 출력에 반영하는 절차를 반복하는 형태의 개루프
와 구별되는 폐루프 전력제어 이다. 이러한 채널측정을 carrier 신호의 신호 대 잡음
비, 즉 月b刀％로 수행한다. 이러한 방법은 빠른 Fading어］ 의한 신호감쇄를 보상하
기 위해서 이루어지는 전력제어이다. 전력제어는 앞에서 이야기되었듯이 단말기어］
거］ 최적의 전력을 할당하기 위해서 이루어지며, 이것의 궁극적인 목적은 지금 현재
처하1 있는 채널환경에서 여러 가지 신호 감쇄요인 중 다중경로 페이딩 혹은 빠른
Fa五ng으로부터 손실될 전력을 보상하기 위해서 이루어진다．
 이러한 Fading어］ 의한 전력변화가 궁극적으로는 전력제어의 수행 빈도가 되어야
한다. 현재 Qualcomm사의 IS-95에서 행해지고 있는 전력제어는 1.25n娼마다 한번
씩 이루어진다. 이것은 IS-95에서는 여러 가지 trade off 요인들을 고려할 때
800Hz이하의 페이딩 주파수를 가지는 신호까지만 전력제어로 보상을 하겠다는
Qualcomm의 시스템 설계자의 생각을 짐작할 수 있을 것이다.
 이것보다 더 빠른 전력제어를 하고자 해서 그러한 전력제어를 한다면, 훨씬 빠른
Fading의 문제를 보상해 줄 수 있으나 그만큼 통화채널의 잠식을 감수해야 한다는
단점이 있을 것이라고 생각할 수 있다．
  瓦／1％어］ 근거해서 행해지는 이러한 전력제어는 IS-95A小인 경우 Reverse 링크
전력제어로 행해지며, IS-95C 혹은 IS-2000（북미에서는 동일한 규격을 cdma21X刃이
라고도 함）에서는 Reverse은 물론 Forw町d 링크의 전력제어는 모두 이 방식을 사
용한다．

   5.5.1 전력제어그룹 - PCG(Power Contr이 Group)

 전력제어 그룹 PCG는 페루프 전력제어의 전형적인 형태인 채널 측정과 출력 조
정명령 전달의 역할을 하기 위한 기본단위라고 할 수 있다. 즉 Forw可d （혹은
                                                                         5 . 전럭제어
   246                                                                              U



Reverse) 전력제어 그룹의 Em나0 상태를 측정하고 거기어］ 대한 해당명령을
Reverse（혹은 Forw可d) 채널의 전력제어 그룹으로 전송하는 것이다． 이렇듯 전력
제어 그룹은 전력의 측정대상이면서 또한 측정명령을 전송하는 전달자인 것이다．
전력제어를 수행하기 위해서 20ms의 통화채널 Frame을 1.25ms씩 16개로 나눈 각
각을 말한다. RC1과 RC2는 전송데이터 속도는 다르나 확산 이전의 최종 변조심벌
의 속도는 모두 19.2Ksi月이다. 따라서 I？町w可d 통화채널의 경우는 24 개의 변조
Syn小O1로 구성되고, Reverse의 경우 텨ock Interleave를 통과했을 때 28.8Ksps인
데 여기어］서 64-Aiy Orthogonal Modulation을 통과한 후의 1.25m5의 전력제어
그룹은 6개의 변조심벌을 갖게 된다. 64-ary orthogonal 변조심벌은 64 ch如이 하
나의 심벌이다．
  그러나 RC1과 RC2를 기반으로 대역확장을 이루어 고속 데이터 통신신용으로
Supplemental Channel어］ 사용되는 RC3과 RC5는 Forward의 확산 이전의 최종
심벌은 38.4시旬4.4K町羚까지 발생된다. 따라서 전력제어를 위해서 사용될 수 있는
자리는 최저 속도인 38.4 ksps를 기준으로 이루어져야 하며, 때문어］ RC1/2보다 전
력제어 Bit가 존재할 자리가 2배가 되는 것이다.

   5.5.2 恥rward 전력제어 부채널

 Forw可d 전력제어 부채널은 1.25ms 마다 iBit즉 data rate이 800bps로 전력제
어 bit를 전송하는 F아＼'.7可d 통화채널의 부채널이다. 이것은 Forw町d 통화채널의
일부를 잠식하여 전송되는데, 이것은 data scrambling후어］ Forw可d 통화채널어］

         且=E沁 艮＝E亦 艮＝E亦 육＝E亦 艮=E/x                     艮=E小 변조 심벌 당 에너지
                         i                                   Scrambling된 변조
           Ci
               （다＋l Ci+2 ! ci*3 C1,4                    C1,5      심벌

                     Punctured     i
                 iiodulation symboP
                 ! 艮2E此    E江5J2 !       bit당 2 심벌




          艮=E沁
                그    전력제어 Bit

                    E拌推    艮E/2
                                   1      PCB stream


                                       艮=E亦 艮=E亦 艮=E亦 전송된 심벌 당 에너지

                                                               전송된 심벌 Stream
            ci       전력제어 Bit          ci+3   ci
                                                   "    ci+5

                 （그림 5-6) 日C］인 경우의 전력제어 S먀y채널
 口                                                                       247


천공방식으로 1 25n心마다 104.1＆升·· 尸S를 빌려서 구성된다. 즉 통화 데이터들은
없어진다. Cdma200(）에서는 통화채널뿐 아니라 F町＼V可d Dedicated 채널상어］ 구성
되기도 한다．
 （그림 5-6）은 RC1인 경우의 전력제어 Sub채널의 구조를 나타낸다. 여기에서 x
는 전송률어］ 따라서 다르게 하여 구별되며, 이것은 전송할 뎨이터의 /!kctivity어］ 따
라서 조정하기 위한 값이다. 이것의 구체적인 값은 血11 rate일 때 2이며, 1/2, 1/4,
1/8은 각각 4, 8, 16으로 Bit의 에너지를 달리한다. 이것은 데이터 Rei光tition어］ 1댜
른 결과이다. Repetition은 시스템 clock에 따라서 동작하기 위해서 Vocoder의 출
력의 Frame의 속도를 맞추어 주는 과정인데 출력 전력으로 그것의 간섭을 줄여 주
는 Voice Activi甘의 효과를 내기 위한 방법이다. 이것은 전송 rate에 따라서 iBit
당 할당되는 에너지가 다르기 때문이다. 자세한 사항은 7장에서 공부하자．
 이러한 데이터 심벌의 에너지가 할당되나 전력제어 Bit만은 언제나 Full Rate일
때와 같거나 크다. 더구나 2 Bit를 사용하여 전송함으로 전력제어 Bit를 복조하기가
다른 정보보다는 훨씬 용이할 것이다. 이것은 다른 Bit들보다 훨씬 중요하다는 이야
기이고, 전력 Bit어］ 이렇게 긴 시간（2심벌）과 큰 에너지를 할당하는 것은 전력제어
Bit가 포함하고 있는 정보는 일반 데이터 심벌어］ 비해서 최소 2배, 최대 32배의 중
요성을 가지고 있다고 생각할 수 있다．

         육＝E/X 艮＝E沁 艮＝E小 且＝E沁 且＝Eb/x             且＝E沁 변조 심벌 당 에너지
                                                        Scramblin日된 변조
          ci      c+1      C汁2    C汁3   Ci+4     C1,5         심벌
               nuncturec
               modulatlo1i
                symbol !
                E芦珉屈i               bit당 1 심벌


          J丁"t.
        且＝E亦    且Ed2 艮2E/2
                                    PCB stream


                                 艮=Eb/x 艮＝E沁 艮＝E亦 전송된 심벌 당 에너지
              전력제어 B't
          （다． i     i            Ci,3   Ci* 4    C汁5    전송된 심벌 匐ream

               （그림 5-7) RC2인 경우의 전력저때 Sub채널


 （그림 5-7）은 RC2인 경우의 전력제어 Sub卜채널이다. 여기에서 且는 심벌의
energy를 나타내고 x는 전송 율어］ 따라서 다르게 적용이 되는 값으로 （그림 5-6）과
동일하다. 여기서 x값은 Full Rate일 때 4/3이고 1/2, 1/4, 1/8일 경우 각각 8/3,
16/3, 32/3이다. 그러나 여기에서 특이한 점은 전력제어 Bit로 사용하는 Bit가 1심
벌이라는 것이 차이가 나고 그것의 에너지는 Full Rate보다 크거나 같다는 것은 동
일하다．
 어찌되었든 전력제어의 정보를 담은 PCB는 일반 다른 변조 심벌들과는 다른 전
력으로 전송이 되며, 다른 일반 심벌들은 동일한 전력으로 출력이 된다. 이것은 그
민큼 전력제어 Bit가 같은 시간 크기의 다른 심벌어］ 비해서 중요한 정보를 담고 있
다는 것을 의미한다. PCB는 하나의 전력제어 그룹 내의 많은 다른 변조 심벌들의
전력어］ 대한 정보를 가지고 전송되므로 충분히 그럴만한 가치가 있다고 할 수 있다．
물론 PCB가 전달하는 전력제어 그룹의 전력정보는 2개 이전의 전력제어 그룹의 정
보가 될 것이다．
 좀더 생각하1 보면 1.25ms의 정보를 전송하는데 약 104ps의 시간의 정보가 사용
된다고 생각할 수 있다．
 전력제어 그룹（PCG）은 20ms의 통화채널 Frame을 1.25ms씩 16개씩 나누어서
전력제어가 이루어지기 위한 기본단위를 말한다. 이러한 전력제어 그룹은 Forward
통화채널의 경우에는 24개의 변조 심벌을 갖게 되며, Reverse 통화채널의 경우에는
6개의 硏／aish 변조 심벌을 갖게 된다．
 기지국에서 수신하는 Reverse 통화채널의 전력제어 그룹은 전력 측정의 단위가
되고, Forward 통화채널의 전력제어 그룹은 전력제어 Bit가 포함되어 있다． 즉
Reverse 통화채널의 6개의 \Walsh Symb아을 가지고 energy를 측정하고, Forward
통화채널의 Walsh Symbol 중어］ 2개를 사용하여 전력제어 명령을 전달한다．
 PCB를 data scra끄曲ling이 된 이후에 하는 천공하는 이유는 무엇이겠는가7 그것
은 Closed Loop Power Control가 5O11丁ces data의 품질인 FER어］ 의한 것이 아니
라 변조퇸 데이터의 품질인 万c/Jo어］ 의하써 전력제어를 하기 때문이며, 이러한 형
태로 이루어져야 빠르게 전력제어가 이루어질 수 있을 것이다. 여기서 구별하고 싶
은 것은 흔히 이러한 전력제어를 빠른 전력제어라고 하나, 이것의 빠름의 의미는
800Hz로 이루어지는 것이 빠르다는 의미이고 필자가 여기서 Carrier 신호의 복조
단계에서 전력제어 정보를 얻을 수 있어서 빠르게 전력제어를 할 수 있다는 것은
다른 의미로 이야기한 것이다. 즉 처리가 빠른 것과 빈도가 빠른 것을 구별해서 이
해해야 할 것이다.
    5. 전럭제어
                                                                                       249
1

     5.5.3 Reverse 전력제어 부채널

    cdma200(）에서는 Reverse Pilot 채널을 통해서 전력제어 부채널을 전송하게 퇸
다. 이것은 Is的M3와는 달리 cdn追2(X刃의 RTT에서는 Reverse Pilot이 존재하
며, 이것으로 인하여 Reverse이 （力herent하게 되며, 아울러서 Forward 전력제어
도 Fast 전력제어를 수행할 수 있게 되었다. 이러한 Reverse I亐lot어］ 추가된 전력제
어 부채널은 （그림 5-8）과 같다



                                                            1            'll ' '
                                            0ne Frame (20ms)

                                                  8
                                                  4그




                        U
        PCG 번호      0   1   2   3    5                  9   10    11 12 13   14   15


                 II                                     I
                                                             'I
         역방향                                      44}




                                                        \
         파일럿
          채녈
                                                        역방향 전력제어 부채널
              프레임 경계 1 PCG(1.25ms)


                                         Pilot



                            ! x빠艸H
                            卜        1 전력제어 그둡 = -
                                                                   寸mH
                            1       1536 X N PN Chips

                        （그림 5-8) Reverse 전력제어 부채널


    cdma2000에서는 Reverse Pilot 채널어］ Forw町（I 링크의 출력을 조정하는 전력
제어의 정보를 실어서 전송한다. 이것은 변조 단계에서 행해지는 800bps급의 빠른
전력제어를 위한 PCB는 물론 Frame의 질을 나타내는 EIB(Eras네田 Indicator
Bit), QIB(Quality Indicator Bit)를 전송하기도 한다. 이것은 Forw可d 전력제어 동
작 모드를 나타내는 FPC소4ODE에 의해서 결정퇸다. 고속 데이티 서비스를 위해서
cdma200(）에서는 Fundamental Channel(IS什95A/B의 통화 채널과 동일） 이외어］
데이터 전송을 위한 전용채널로 Supplemental Channel을 사용하고 있다. 따라서
전력제어 또한 이러한 채널들을 별도로 해 주어야 할 것이다. 때문어］ Fundamental
Channel의 전력을 제어하는 1차 Reverse 전력제어 부채널과 Supplemental
Channel을 전력제어는 2차 Reverse 전력제어 부채널을 생각할 수 있으며, 이것은
FPC소4ODE어］ 의해서 결정되어진다. FPC_MODE에 따른 Forw打（I 전력제어 형
태는 다음의 （표 5-2）와 같이 정리될 수 있다．
   250


             （표 5-2) FP（二MODE에 따른 Forward 전력저때 Scheme

FPC        l차 Reverse          2차 Reverse             G계ed
                                                              전송日it    속도（b口s)
MODE      전력제어 부채널            전력제어 부채널                N幻de

 0（刃      모든 PCG(16개）                                 사용      PCB        800
 001      짝수 PCG(8개）          홀수 PGC(8개）                      PCB        10
                            0,2,3,4,6,7,8,10,11,12,
 010     1, 5, 9, 13번 PCG                                     PCB      200/600
                               14,15번 PCG
 011      모든 PCG(16개）                                         Em         50
 100      모든 PCG(16개）                                          QIB       50
 101      짝수 PCG(8개）          喜수 PCG(8개）                     QIB/EIB     50
 110      짝수 PCG(8개）          홀수 PCG(8개）              사용     PCB/EIB    400/50



 FPCHMODE가 101인 경우에는 1차 Reverse 전력제어 부채널은 QIB로 2차
Reverse 전력제어 부채널은 Effi를 전송하여 전력제어를 한다. 그리고 FPCHPRI
CHAN값을 통해서 전력제어할 채널을 FCH(=0）로 할 것인지 DCCH(=1）로 할 것
인지를 선택한다．
 FPC公4ODE가 110인 경우에는 1차 Reverse 전력제어 부채널은 PCB를 전송한
다． 그리고 2차 Reverse 전력제어 부채널은 Em를 전송하여 전력제어한다. 그리고
FPC_SEC_CHAN값을 통해서 전력제어 할 SCH 채널번호를 선택한다. 이를테면,
0인 경우는 0번 SCH를 1인 경우는 1번 SCH를 전력제어한다．
 ＜표 5-2）에서 알 수 있듯이 Supplemental Channel을 전력제어할 때 ()01, 010인
경우는 PCG에 PCB를 천공하여 전송하고 101, 110인 경우는 각각이 PCG에
QJB/EIB를 삽입하써 전송한다．

  5.5.4 전력제어 부채널 전송 Timing

 이 절에서는 전력제어 부채널이 언제 전송되어야하고 혹은 수신된 전력제어 부채
널의 내용을 언제 반영해야하는지어］ 대해서 공부해보자．
 전송퇸 전력제어 정보는 일반적으로 round trip delay와 시스템의 처리시간 등을
고려하여 n번째 전력제어 정보는 n+2번째어］ 반영된다. 이것은 전력제어그룹 단위
혹은 Frame 단위로 이루어진다. 전력제어는 크거］ Ew'No어］ 의해서, FER어］ 의해서
                                                                              251



이루어지는데 Eb/NO는 하나의 전력제어 그룹이 끝나면 판단 혹은 분석되는 값이고，
FER은 Vocoder 쪽에서 Frame을 전체적으로 복호가 완료되어야 하므로 Frame이
끝나야 그것에 대한 분석이 이루어진다. 때문어］ 다음의 （그림 5-9）과 같이 전송 타
이밍이 결정될 것이다．
 （그림 5-9）에서 알 수 있듯이 PCG어］ E1B나 QIB와 같이 Frame 품질지시자가 한
Frame어］ 16개씩 들어가게 되는 형태로 Frame이 구성퇸다. 이것은 Frame 당 Effi
가 하나씩 전송되던 종전의 방식과는 사뭇 다르다．
 Supplemental Channel의 경우 1X IS그000에서는 최대 16배까지의 대역확장이
가능하다. 즉 한 Frame어］ 전송되는 정보량이 16배가 된다는 이야기이다. 앞의 문단
에서 이야기한 내용은 이러한 Fra工ne구조를 볼 때 전력제어Bit정보가 가지는 의미
를 생각해볼 때 특별한 의미를 가진다는 것을 알 수 있을 것이다．

                                           F-FCH : 순방향 Fundamental 채널
                                           DCCH : Dedicated Control 채널
                                           F-Sd11 : 순방향 Supplemental 채널

   수신된 F FCH혹                                      日
                         卜1
   은 DCCH의 프레1
   임                  20mses                                   8혹은 16 개의
                                                               PCB가 EIB 나
                                                               QIB로 설정됨

   수신된 전력제어               H
                                                   1
   부채 널
                                              i+
          (a) 1차 역방향 전력제어 부채널 전송Timing : FPC+MODE= '011', '100', '101'

   수신된 F_SCH
   의 프레임
                                                               8, 16혹은 32개의
                                                               PCB가 BIB로 설
                    미 F SCH 立러1익 겻겨1 卜                         정됨

   수신된 전력제어
   부채널                          1
           (b) 2차 역방향 전력제어 부채널 전송Timing : FPC_MODE= '101', '110'




                 1 PCG=1.25ms
                                                       M


                     d                                                p
                                        1 프래임＝20ms


                                    （그림 于9) 기ming
      252
                                                                1


   5.5.5 Gated Mode에써의 동작

  CDMA시스템에서 특징적인 것 하나가 간섭의 억제를 위해서 Voice Activity를
평가하써 전송에 반영하고 이것의 실질적인 전송헝태가 Gated 출력 모드이다. 전
송하는 Frame을 voice（혹은 data) activity어］ 따라서 그것의 속도를 Full, Half,
1/4, 1/8 rate으로 나누어서 전송한다. 이로 인해서 Reverse에는 전력제어 그룹이
언제나 일정하게 될 수가 없고 그것의 속도도 달라지게 된다．
 （그림 5-10）은 Reverse 전송의 예를 보여 주고있다. 여기에서 각각의 PCG들은
Interleavit坦이 끝난 데이터들이 각각 2줄씩 실려질 것이다. 여기에서도 데이터가
full rate이 아닌 경우는 R아光atation된 데이터가 되므로 Interleaver matrix
(32x18）에서 한 줄씩 건너뛰면서 실려지게 될 것이다．
  그렇다면 문제는 Full rate이 아닐 때 어떤 PCG가 전송되어야 할 것인가를 결정
지어야 한다. 이러한 과정을 뎨이터 버스트의 랜덤화 과정이라고 한다. 이러한 Data
Burst Ran面m과정은 전송되는 데이터의 속도와 Long Code masking이 끝난 더］
이터 중 14 Bit 그것의 위치를 결정하게 된다. 이 14 Bit는 앞 Frame에서 2번째 전
의 전력제어 그룹에서 끝에서부터 14 Bit를 취한다. 즉 앞 Fran妃이 14번 PCG의 마
지막부터 Bit수를 읽어오는 것이다. 즉 （그림 5-10）에 나타난 것과 같이 읽혀지게
된다．
 또한 전송속도어］ 따라 전송 전력제어 그룹을 결정한다.
 우선 Full rate인 경우는 모튼 전력제어 그룹이 전송될 것이다． 당연히                   ．
 전송 데이터가 4800bps혹은 7200bps인 경우 bO, 2+bl, 4+b2, 6+b3, 8-'-b4, 10+b5,
12나月, 14+b7번째의 8개의 전력제어 그룹이 결정된다.
 전송 뎨이터가 240bps혹은 孤)0bps인 경우는 다음과 같은 과정을 거쳐서 4개의
전력제어 그룹이 결정된다．
 水 b8이 0일 때 妖）, 혹은 b8이 1일 때 2+bl
 水 b9이 0일 때 4+b2, 혹은 b9이 1일 때 6+b3
 木 bl0이 0일 때 8+b4, 혹은 bl0이 1일 때 10+b5
 木 bli이 0일 때 12+出, 혹은 bil이 1일 때 14+b7
 전송 데이터가 1200bps 혹은 1800bps인 경우는 다음과 같은 과정을 거쳐서 결정
된다. 이때는 2개의 전력제어 그룹이 전송될 수 있으므로 2개의 위치를 찾는다． 첫
번째 PCG는 (b8, b12）의 쌍의 값과 (b9, b12）을 보고 결정한다. 즉 (b8, b12）이
    5 . 전력제어
                                                                                                                                                                                                             253
.


                                                                                                                                           1 프레임인 20m sec는 96 information bit 즉
    36개의 （그＜) de                                                                                                                           576걔의 repeated 된 Code sya小아（22.8 Ksp引，
    symbol( 인터 리 빙                                                                                                                         혹은 96개의 modulation syn山아， 혹은 16걔
    S瑥打奴의 2개줄）) 6                                                                                                                          익 PCG로 구성된다．
    개의 변조심벌, 1개
    외 PCG로 구성된다．
                                                                                                                20m sec

                 -

                                     H-              1.25 m sec

     앞의 프레임                                                                                                                                                                                              9600/14400
                                                 1            1           1            1            1           1              1       1       i        i          1          1        i        t        bps 프레임
    12 I 131 111 1                               1 2 1 3 1 4 1 5 1 6 I 7 I 8 j 9 10                                                            1        111
                                                                                                                                                                   112        1 13 1 14 1 15
                                                                     Code syn小ol들은 인터리빙된 테이터들이다
                                                                   『 인터리빙은32工18로 2개의 행이 연속 해서
                                                                     하나의 PCG에 들어간다．

     앞의 프래임                                                                                                                                                                                              4800/7200
                                                                                                                                                                                                         bps 프레임
    12 j 13 1 14115            0          l             2          3             4         5            5                                  9       10         11         12       13       l        is




     앞의 프래임                                                                                                                                                                                              2400/3600
                                                                                                                                                                                                         bps 프레임
    12 1 l3 1 14 1 15          0          l             2          3             4          S           6                          S       9       10         11 12               13 1 14           15




                                                                                                                                                                                                         1200/1800
                                                                                                                                                                                                         bps 프레임
                               0           l            2          3             4          b           5 1 7                      8       9        0         11 12               13       14       15


                                                                                                                                       랜덤화를 위한 stream이 {bO,bl. ... .
                                                                                                                                       b13} =00101101100100인 경우

                                                                                                    bl]
               bl

                                                                                           b l nU           b l n乙   b 1l nd
               b0       b n乙       b nd   b 41   b 二U       b nh   b nr   b RU       b 0
                                                                                       U




                        （그림 5-10) Reverse ODMA 채널 가변 데이터 율 전송


(0,0）이면 hO, (1,0）이면 2+bl이고 (b9, b12）이 (0,1）이면, 4+b2, (1,1）이면， 6+b3이
졀정퇸다．
    또 다른 하나의 위치는 (blO, b13）의 쌍의 값과 (bli, b13）을 보고 결정한다． 즉
(blO, b13）이 (0,0）이면 8+b4, (1,0）이면 10+b5이고 (bil, b13）이 (0,1）이면, 12+b6,
(1,1）이면 14+b7이 켤정된다．

    Forward Reverse 전력제어 부채널 전송 timing
    이상과 같은 방법으로 Reverse이 전송될 때 Forw町d쪽도 이어］ 상응하는 처리가
     254


                                   J
                                                                                               20 mn 묘 16 Pi,wir C汁｝ ！쩍J1(;
                                                                                                                    ilb쩍ilOros玎｝
                                                                                                                            r0i玎｝ii                                            h



                                                                 1                        15 1 17                       1                1 1 1
           Forward
                                   1
  i뇨Wer（如ntr야 S,1brhanne1 寸                           '25 ma                                                                                                                          >
                                                     1 1 2                                             6                    9       1。       11        12   13       14   15
                                               卜
   1ta}18n玎件日ion Mtl軋K) bpn
                                   1
                                                                          3                                     1   8
                                                                                  4
                                                                              1
                               +           +Rornsd Thp


                                                                                                                                                                                   n
                                                                                                                                                                                   J
       nati1l客 Roir 甘 l

                                                                                                                                             눠U                           너
                                                                                                                                                                          尸斗
                                             l jj . 나 . 너 rU I
                                                                                                                                                      ri
      R的哮然密佃'셔                                                                                    J        H                    I                                J                     1


                                        Pil。 4u
                                           t P。
                                              wir
                                               I, C,
                                                  C。 Intr。' Ill                       '




                                                                                                                                                                     口         H1Jd
                                       4                                                       衣｝in在 枉 16 Pbwer Control (i기otlp咎
                                                q- l25 ma

                                             , , 口., r기 , ri , 口,, F구，, 12
                               +
           恥｝ntard
  Pa'甘Mi Cmiii口I Subdm,心坤l 끼
   Trm.8im毖81口n or 400 lip히                                                                                                                                 13


       oti堪   Rate - 1/ 2
                               + 4和쁑，抄如

                                        1 0 口1
                                                                                               ?                                                             7
      Room恥｝ 芍lot,
                  Cii日srno14
         ' 妖000ps거｝ll                                        , ., 니 , 二了 ,, 三긔 , 7                                                       m
                                                                                                                                                                     14
                                                                                                                                                                                      >




                               寸                                                                                                                            口                  H1JU
                                                                                               20 ma 月 16 知짜orCi月strolOr,싸pa
                                                411.25 ma


                                                                                                                        口
          F"nrLUnn立
  P0니屯0 Coistr朴 客1工bhLm甘1 띠
  ］노mJ｝月11}i台在Mm at 玄好 如8                       1i       2       1        3
                                                                              1   4       r;      '6
                                                                                                           17       8
                                                                                                                                    ,,   1   ,,   1    ,,
                                                                                                                                                                     主4
                                                                                                                                                                                      1


                                       : '     Rm끄41i 'l노Mi
       O帥0母 Rob       쿄 1/ 4   -           !1-   DtLay



      Rn喀忿남岫毗i.                         1, 1 , 1             ,       回，
                                                                                                               莩' 8 1 9 f 1。";': 12 1 1코 14曜

                      （그림 5-11) Forward Reverse 전력제어 부채널 전송 timing


이루어져야 할 것이다. 이러한 이유로 Reverse 전력제어 그룹어］ 대응되는 Forward
전력제어 그룹의 형태가 새롭게 정의되어야 함으로 새로운 Forw可（I 전력제어 부채
널의 형상이 있을 것이다．
 단말기가 Gated Mode로 동작하지 않을 경우는 8(）力PS의 빠르기로 전력제어 부
채널이 전송될 것이다. 또한 1/2 rate의 Reverse Pilot채널이 gated로 전송되고 있
다면, Forward 채널에서는 짝수 번째의 전력제어 그룹에만 전송하고（呱力ps), 1/4
rate의 Reverse Pilot채널이 gated로 전송되고 있다면, Forw可d 채널에서는 1, 5,
9, 13번째의 전력제어 그룹에만 전송（200bps）한다．
 （그림 5-11）는 Forw町（I Reverse 전력제어 부채널 전송 timing을 나타낸다.
 RC 3- 6과 갇이 cdma2(X刃에서 새롭게 사용되는 채널 형상들에서는 기지국은 단
말기로 전송한 전력제어 그룹을 시점으로 (REV_P＼入／RCNTLDELAY) X 1.25ms
경과 후 시작되는 PCG에서 전력제어 Bit를 전송한다. 여기에서 REVPWR小
CNTLDELAY는RC 3- 6에서 gated mode로 동작하는 Reverse fundamental 채
널의 Reverse 링크 전력제어 지연성분이며, round trip delay성분이 0일 때
                                                                                                                         255


Reverse 링크 PCG의 마지막과 Forward 링크 PCG小1간의 시간이다．

   5.5.6 전력제어 Bit (PCB)

 단말기의 전력을 조정하는 Bit로 1.25ms마다 전송된다. 전력제어 Bit가 0이면 해
당 단말기로 하여금 전력을 올리라는 것이며, 1이면 내리라는 것이다. 전력제어 Bit
의 값을 결정하기 위해서 기지국의 Reverse 통화채널 수신기는 자신이 할당된 단
말기의 신호 세기를 전력제어 그룹 단위로（1.25ms마다） 어림잡는다. 이를 이용하여
전력제어 Bit의 값을 결정한 후, 이 전력제어 Bit를 신호 세기를 어림잡은 Reverse
통화채널의 전력제어 그룹 이후 두 번째 전력제어 그룹어］ 실어 Forward 통화채널
로 전송한다．
 전력제어 Bit의 길이는 104.1666··· 尸S로 Forw町d 통화채널의 변조 Symbol 두
개의 길이와 같다. 전력제어 Bit는 data scra끄［ibling 후에 Forw可d 통화채널어］ 실
리게 되는데, 두 개의 연속퇸 변조 Syn小이을 전력제어 Bit로 대치한다（Symbol
puncturing). 전력제어 Bit가 대치되는 위치는 전력제어 그룹 내의 24 개의 변조
Symbol 중 Symb아 0부터 Symbol 15 까지 16개의 위치가 가능하다. 바로 앞 전력


 역방향



                                          m
 통화 채널

                                                                6            7         8     9     1。 니，小小4 15
   l. 25ms   -5                           1Bas              ,       亂，   tion
                                                 1) 신호강도측정
                                                 2) 측정치를 전력제어 Bit로 변환
 순방향                                             3) 전력제어 Bit 전송
 통화 채널            *-Round Trip Delay


                       1 1 2     3 1 4 1 5 1 6                           7                  9 1 10 I 11 I 12 I 13 i 14 I 15

  1.25ms
                                                                                                                      사용하지 않
                               Value=11                                                                                는 PCB
                               PCB 위치                                                  }1의 변조 심벌 인PCB
                                                                                       송


                                                  111
                   n
                   U                                   \U
                                                   ,                ,    ,       F滋I       I社， 131 , ,
                                                                                             「           1,   ,


                                 16 possible starting전력제어bit
                                                 1.25 ms = 24 modulation symbols
                                                                                                    -니            卜
                        （그림 5-12) 전력제어 텨t의 위치 결정m日Cl
   256


제어 그룹의 변조 Symbol 23（八4SB), 변조 Symbol 22, 변조 Symb이 21, 변조
Symbol 20(LSB）으로 결정되는 4 Bit 이진수로 현재 전력제어 그룹에서 전력제어
Bit의 위치가 결정된다. 전력제어 Bit의 에너지는 최소한 Eb 이어야 한다．
 전력제어 Bit 하나어］ 의한 단말기 출력전력의 공칭 변화량은 1dB 이며, 여기서
0.5 dB까지의 변동은 허용퇸다. 같은 부호의 유효한 10개의 전력제어 Bit어］ 의한
단말기 출력 전력의 변화량은 공칭 변화량 10배의 20 % 이내이어야 한다.
 PCB는 각각의 전력제어 그룹마다 한번씩 전송되는 Bit로 2번째 전의 PCG의 전력
값어］ 의하써 변조과정에서 결정되며 전력을 증감하라는 명령을 나타내는 Bit를 말한다．
 일반 데이터 열 가운데에서 PCB로 대치되는 위치는 랜덤하게 결정되며, 그것의
상서慢｝ 위치는 PCG내의 24개의 변조심벌 중 0번에서 15번까지의 16개 중의 하나
가 그것이다. 이것은 바로 직전의 PCG의 변조심벌 23（八4SB), 22, 21, 20(LSB）번의
값들이 나타내는 2진수의 값으로 현재의 PCG에 PCB를 천공할 위치를 지정한다.
 그런데 IS-95C 혹은 IS小2000의 RC3이상인 경우어］ 훨씬 빠른 채널에서는 이러한
것이 달라진다. 즉 1개의 전력제어 그룹 내에 포함된 Bit가 많아졌기 때문이다. 여
기에서 IS弱C의 Forw可d 채널어］ 천공되는 Bit들의 위치와 Bit수를 정리하면 다
음의 표와 같다．

                （표 5-3) 전력제어 duration및 전력 level

              Punctured     Minimum       Starting
     RC       Modulation   전력제어 Bit       Symb이            Decim카ed Bit
               Symb이        Energy        Position
      1           2           月b        0, 1, " .., 15     23, 22, 21, 20
      2           1          3/4 且b     0, 1, " " " j 15   23, 22, 21, 20
  3(non-TD)       4            丑b       0, 2, " ', 30      47, 46, 45, 44
   3(TI力          4           ib        0, 4, " ', 28       47, 46, 45
  4(non-TD)       2            丑b       0, 2, ···, 14        23, 22, 21
    4(TD)         2           月b        0, 2, " ' " ! 14     23, 22, 21
  5(non-TD)       4           月b        0, 2, " ', 30      47, 46, 45, 44
   5(TD)          4            丑b       0, 4, ..., 28       47, 46, 45
      6           6           月b        0, 6, "·,42         71, 70, 69
      7           3            万b       0, 3, " ' " , 21    35, 34, 33
      8           6           E6        0, 6, " ", 42       71, 70, 69
      9           3           月b        0, 3, " ", 21       35, 34, 33
                                                              257
.

    이상의 표와 같이 전력제어 Bit가 천공될 위치를 나타내는 것은 랜덤하게 이루어
진다. 또한 이러한 Bit들은 고속 테이터 전송시에는 그 Bit들의 위치도 랜덤하지만
순서도 단순증가가 아니라 2n 혹은 2n+1의 형태로 제공된다. 여기에서 n=0,1,..인
실수이다. 여기에서 TD는 Transm孔 I玉versity로 Orthogonal Trans而tl玉versity
(OTD）와 Space T油e Spreading(STS）를 포함하는 것이다．


                         Va1ue=6                2개의 변조 심벌
                        PCB 위 치                  PCB 전송


                      。111213141516171819110111P，
                                       \\=
              l

                                                牛 ,，까i41i51
                                    1.25 ms = 24 modulation



                  （그림 5너3) FOB의 시작위치의 랜덤화냐극C4(non-TD)


    （그림 5-13）은 non-TD의 RC4인 경우 PCB의 시작위치 랜덤화의 예이다．
RC4(n아i-TD）인 경우는 ＜표 5-3）에서 알 수 있듯이 시작위치를 나타내는 Bit는
시작Bit를 계산할 때 짝수의 형태로 증가함으로 6번째 짝수인 12가 되고 여기에 2
Bit를 전력제어 Bit로 천공하게 된다．

    F心｛三 于화
    전력제어의 정보를 가지고 전송되는 PCB는 빠른 처리를 위해서 변조퇸 심벌에
천공방식으로 완전히 채녈 데이터를 파괴하면서 쓰여지게 된다. 즉 가장 마지막 단
계어］ 이루어지는 처리이므로 수신단에서는 가장 먼저 이루어지는 단계로 처리가 빠
를 것이다. 이것은 전송채널자체의 품질어］ 대한 기준으로 평가하는 전력제어이므로
이러한 방법으로 행해진다．
    다음절에서 이야기될 FER에 근거한 전력제어는 결국 데이터가 \/（兀oder까지 가
서 복호되는 과정이 되어야만 전력제어를 위한 판단이 설 수 있으므로 차이가 난다
고 할 수 있다．


    FCB의 결정 - Finger Demodulator

    기지국의 Finger Demodul毗아로 입력되는 신호는 서］ 섹티의 두 개씩의 수신 안
    258


                                                     다음 단계는 Quadrature
                                                     PN 확산 변조가 이루어짐．


               Convolutional   Modulation symbol
                EnCoder &
      User
                InterIeav釘
      Data
                                                          전력 제어
                                                         bit 800 bps

                                                                                  Walsh
                                                                       800 Hz
                                                                                 sequence
     PN Long                      De口matoi" 引m蜘          Decimation             orthogonal
      Code                        every 64m symbol       Ml.戊 timing            spreading
      mask                          11288.8/19石             can汁ol



                       （그림 5-14) 전력저때 텨t의 다중화


테나로부터 온 기저대역의 신호를 PN chip rate 의 8 배로 샘플링한 디지털 데이터
이다．BSD(Base Station Demodula的r）의 데이터는 출처어］ 따라서 6개（3섹터의 각
각 2개의 수신 안테나）로 분류된다．
 BSD로의 데이터 입력은 24개의 신호선을 통하여 이루어진다. 이 24개의 데이터
입력 선은 다시 8개씩 서］ 그룹으로 나누어지는데, 각 그룹은 각 섹터로부터의 데이
터를 담당한다. 24개의 모튼 데이터 입력선은 각 섹터의 2개의 수신 안테나의 데이
터가 time multiplex 되어 있다. 따라서, 각 입력선의 data rate 는 PN chip rate
의 16배가 된다．
 BSD(Base Station Dc曲dula的r）의 Front End Interface는 입력 데이터를 안테
나 1과 안테나 2로 De그miltiplex 한 다음 F岫er와 2개의 searcher 에게 6개의
data stream 중 하나를 서로 상관없이 선택하여 공급한다．
 Fir坦er는 공급되는 데이터를 PN chip rate로 decimate 하고, I채널과 Q채널의
데이터를 각각 I차뻘 Pilot PN Sequence와 Long Code PN Sequence의 곱과 Q채
널 Pilot PN Sequence 와 Long Code PN Sequence 의 곱을 사용하여 Despread
한다． Despread 퇸 후 까nger는 \Valsh 칩의 주기만큼 데이터（4개의 PN칩）를
accumulate 하여 Fir垠er의 Fast Hadamard Tran虹아m(FHT) 블록으로 보낸다．
FHT 블록에서는 입력 데이티와 64개의 Walsh S珥nb아 각각어］ 대한 상관함수를
구한다． I와 Q채널의 64쌍의 상관함수 결과는 64개의 \Valsh Symbol어］ 해당하는
에너지의 크기를 구하는데 사용된다. 여기에서 가장 큰 크기의 예너지를 갖는
    5 . 전력제어
.                                                                                            259


Walsh Symbol이 복조된 \Ualsh Symbol로 선택된다．
    복조된 Walsh Symb아은 채널 Element(EC) 프로세서 인터페이스를 통하여 프
로세서에게 읽혀진다. 프로세서어］ 제공되는 데이터는 복조 퇸 \Valsh Symbol 인덱
스（FINGER_DEMOI工SYMBOL), 추정된 ＼入／aish Symb아의 크기（FINGER뇨
SYMBOLJvIAG), 그리고 위 두 값을 결정하기 위해 사용된 I채널과 Q채널 성분
(FIl寸GER小4AXJ와 FE나GER小/JA乂．Q）이다．


    PCB의 결정-Walsh Symbol Interrui丈 Handler

    복조기에서 Reverse Link 통화채녈을 Walsh Symb아 단위로 복조한다. 따라서，
채널 Element의 프로세서는 복조기의 복조된 데이터를 \Valsh Syi工由이 단위로 처
리해야 한다. 이를 위해서 채녈 Element의 프로세서는 208.333··· 尸S마다 발생하는
Walsh Symbol 인터럽트를 사용한다．
    Walsh Symbol interrupter Handiler는 인티럽트가 발생하면 채널의 in-lock 상
태의 복조기에서 복조퇸 Walsh S珥nbol의 FINGER小4AXJ와 FINGER_MAX_Q
를 읽어온다. 읽어온 각각의 값들을 제곱하여 더한 후 다시 이를 제곱하고
PC_TRUNC(= 12）만큼 오른쪽으로 Bit shift하여 energy metric 을 구한다．
in-lock 상태의 모든 복조기의 energy metric 을 더한 다음 전력제어 Bit의 결정을
위해 축적한다. 전력제어 Bit의 결정은 6개의 仄7alsh Symb이의 energy metric 이
축적된 후 수행뒤다．

                            Filter Matched
                                 to Wo
               -

                                           +




                            Filter Matched
                                 to Wi
                   1+
                                                  Select
      역 확산퇸                                      Maximum                                  Power
                                                                              compare
       신호
               H        +
                            Filter Matched
                                 to W2     +
                                                  of 64    +
                                                               Z
                                                               ] 나1n］니
                                                                         +      砥rith
                                                                             T뇨esh아d
                                                                                      +   Up및
                                                                                          Down


                                  1 1 1




                            Filter Matched   1
                                             n
                   -




                                t" 싸 " "

                                      （그림 5-15) 전력저때 텨t의 결정
                                                                                                 5; 전력제어
   260                                                                                                     1

 축적된 6개의 \Walsh Symbol의 에너지 metric은 전력제어 임계치와 비교되어
에너지 n祀tric이 전력제어 임계치보디． 크면 전력제어 Bit에 1을 넣고 작으면 0을
넣는다．
 CS八4(Ce11 Site Modem) 내에서 처리되는 절차는 다음과 갇다．
 CSM(Cel1 Site Modem)으로 입력되는 신호는 3 sector 각각의 2개씩의 안테나
로부터 수신된 기저대역의 신호를 Sect아당 PN chip rate의 8배로 표본화한 디지
털 데이터이다．
 따라서 CSM의 데이터 입력선은 24개로 이루어지며, 이 24개의 데이터 입력선은
각각의 sect아를 담당하도록 8개씩 할당된다．
 24개의 모든 데이터 입력선은 각 섹터의 2개의 수신 안테나의 데이터가 Time
multiplex되어 있으며, 각 입력선의 data rate은 PN chip rate의 16배이다．
 이 신호는 CSM의 Front End Interface를 통하여 Fir垠er와 Searcher로 공급되
며, Finger는 이 신호를 De面'ate하여 Short兀ong PN Sequence Demodulation과
FHT(Fast Hardarm可d Transform)를 수행하여 해당 \Va1sh Symbol을 찾는다．
 1/Q 채널의 데이터를 각각 I/Q 채널 P11毗 PN Sequence와 Long Code PN
Sequence로 곱하여 Despread한다．




                                                                                                 Rx data
                                                                                            +Packet




                                                                       전력 information
                                                                  >   Time tracking




                                 Cascade Input :
    RxI 소 R乂Q:
                                 （知1a,. 口h f뇨1 겨h m
    的，U1, 比，目，1. 1
                                 JLaJ[O..31, T乂mQ(o..3]
    RxaJ[O..31. Tx. .u.Q[O..3]
                                 le且J[O..3], TxJLQ10..3]
    取JJEO..3]. TxWQ[O..31
                                 1N_ 1[O..3], Tx -Q[O..3]   ,
    RxyJIO..3]. Tx...Y1QEO..3)

                  T虹 & TxQ                                            부호화기            lix data
                  1丸． U,, 民，Bl, %, 呱         <                           및        < P正涵
                  T乂1CLILO..3], Tx...a..QIO..3]                       9l E] 긔i긔
                  Tx1njEO..3], TxJLQ[O..31
                  Tx41[O..3]. Tx_ LQ[O..3]


                                            （그림 5-16) CSM Block 미agram
                                                     261


  Despread퇸 후 Fii坦er는 \Ualsh Symb이의 주기만큼 데이터（4개의 PNch巾）를
accumulate하여 Fir垠er의 FHT 블록으로 보낸다．
 FHT 블록에서는 입력 데이터와 64개의 Walsh Symbol 각각어］ 대한 correlati아l
을 구하며, I/Q 채녈의 64쌍의 correlation 결과는 64개의 砥／alsh Syn小이에 해당되
는 에너지를 구하는뎨 사용되며, 여기에서 가장 큰 에너지를 갖는 \Valsh Syn而이
이 선택된다佃此hogonal Code인 \Ualsh Code의 우수한 Orthogonality를 이용）.
 복조된 \V出sh Symbol은 CE（채널 Element）의 I노ocessor Interface를 통하여
Processor어］게 읽혀진다．
 Pr（兀essor어］ 제공되는 데이터는 복조된 \Vaish Symb이 index(FE나GER나DEMOD
_SYMBOL), Walsh Symb아의 크기（F瓜GERmSYMBOL_MAG), 그리고 위의 두
값을 결정하기 위해 사용된 T/Q 채널 성분（FINGER小4AXJ와 FINGER소4AXm
Q）이다．
 CE는 \Vaish Syn小아 단위로 발생하는 \Vaish Syn由이 interru吼를 사용하여 채
널의 N- LOCK 상태의 복조기에서 복조된 w싫sh Symbol의 FINGER小4AX寸I와
Fn寸GER_MAX_Q를 읽어온다.
 이 값틀의 각각을 제곱하여 더한 후 이것의 제곱근을 구하고 PC_TRUNC( =12)
만큼 오른쪽으로 bit shift하여 energy metric을 구한다．
 In_Lock 상태의 모든 복조기의 energy metric을 구한 다음 전력제어 bit의 결정
을 위해 축적한다. 전력제어 bit의 결정은 6개 Walsh S珥I由이의 energy metric이
축적된 후 수행퇸다．
 축적된 Walsh Syff由ol energy m曲ic은 전력제어 Threshold와 비교하여 전력
제어 bit를 결정하며, 이렇게 결정퇸 전력제어 bit는 Forw可d 통화채녈의 전력제어
부채널을 통하여 단말기로 전송된다．


 전력제어 Bit(PCB) 결정 시간
 그렇다면 이러한 전력제어 Bit는 어느 시점어］ 결정되겠는가7 전력제어 Bit의 결
정이 일어나는 정확한 시점은 전력제어 그룹 내의 4번째 \Val計i Symbol의 에너지
가 축적되고 난 직후이다. 그러므로, 전력제어 Bit의 결정을 위히］ 사용되는 에너지
측정치는 이전 전력제어 그룹의 네 번째, 다섯 번째 Walsh Symb아의 에너지와 현
재 전력제어 그룹의 첫 번째부터 너］ 번째까지의 Walsh Symb이의 에너지이다. 전
         /
                                                 5 . 전력제어
   262                                                      .



력제어 Bit의 결정이 한 전력제어 그룹의 끝에서 행해지지 않고 중간에서 이루어지
는 이유는 전력제어 Bit 위치 기록과 전력제어 Bit 기록어］ 필요한 충분한 시간확보
때문이라고 생각퇸다．
 （그림 5-17）을 보면 round trip delay(1마일당 대략 6개의 PN 칩） 때문어］
Reverse 통화채널의 5번째 전력제어 그룹의 끝이 Forw可d 통화채널의 6번째 전력
제어 그룹어］ 놓여 있음을 알 수 있다．


             전력제어 bit 결정 시점




                      （그림 5-17) 전력제어 Bit 결정 시점


   5.5.7 전력제어 임계치

 전력제어 임계치는 전력제어 Bit 결정의 기준이 되는 값이다. 축적된 6개의
Walsh Symb아의 에너지 metric과 전력제어 임계치를 비교하여 에너지 metric이
전력제어 임계치보다 크면 전력제어 Bit어］ 0을 넣고 작으면 1을 넣는다． 전력제어
임계치는 Selec的r/Vocoder로부터 20ms마다 보내오는 값으로 갱신된다. 이 전력제
어 임계치는 최대값과 최소값의 사이에 있어야 하며, 만약 Selector/Vocoder로부터
보내져 온 값이 이 범위 밖어］ 있으면 공칭값으로 갱신퇸다． 전력제어 임계치의 최대
값, 최소값, 그리고 공칭값은 Selector/Vocoder를 관장하는 BTS제어기인 BSC로
제공된다．



  5.6 0ther 이osed Loop 천력 . L3 전력제어                             )


 지금까지 이야기한 폐루프 전력제어는 변복조 과정에서 전력제어의 정보가 교환
된다는 측면에서 physical layer쪽에서 이루어지는 전력제어라고 볼 수 있다. 그러
나 또 다른 형태의 폐루프 전력제어는 IS-95C의 최상위 단인 前gnaling layer에서
이루어지는 전력제어를 이야기할 수 있다. 이러한 전력제어는 전력제어 자체가
 U                                                        263

IS-2000에서 규정한 메시지들로 이루어진다는 측면에서 그렇게 생각할 수 있다. 물
론 앞서 이야기한 전력제어들도 그것들의 기본적인 정보는 L3의 Signaling
Message들로 전송이 되지만 이것은 전력제어 자체를 수행하는 것이 아니므로 L3
에서 행해지는 전력제어라고 구분할 수는 없다．
 L3의 전력제어를 수행하기 위해서 기지국은 Forw町d 통화채널 전력제어를 다음
의 두 가지 방법으로 Enable한다. 첫째는 기지국이 호출채널로 보내지는 System
Parameter 八1essage를 사용하여 Forw可d 통화채널 전력제어를 enable 할 수 있
다． 또 하나는 Forw可d 통화채널로 보내지는 전력제어 Parameter Message를 사
용하여 할 수도 있다. 기지국이 Forw可（I 통화채널 전력제어를 enable 하지 않으면
단말기는 Forward 통화채널 전력제어의 기초자료인 Frame 에러율 통계（Frame
error rate statis侃5）를 기지국으로 전송하지 않는다. 이것은 IS-95C로 규격이 발
전되면서 추가퇸 채널인 Forw可d Dedicated Control 채널（F-DCCH）과 Forward
Supplemental 채널（F-Sd1키어］ 대해서도 FPC小4ODE와 별도로 진행퇸다．


     5.6.1 관련 메시지


 System Parameter Message

 Forw可d 전력제어를 위해서 호출채널을 통해서 전송되는 System Parameter
八/Iessage의 관련 내용은 다음의 （표 5-4）와 같다．


            （표 5-4) 시스템 Parameter의 전력제어 관련 필드

                    필드                          길이（bit)
            P사R REP THRESH                        5
            PWR REP Frame S                       4
            PWRTHRES표mENABLE                      1
            PVRPERJODENABLE                       1
            PWRREPJJELAY                          5


 P＼사RREPTHRESH는 전력제어 Rej兀曲ig Threshold로 임계치 보고어］ 사용
되는 불량 Frame수의 임계치를 나타내는 필드이다. 한 측정 주기 동안어］ P＼入／R
   264


REP_THRESH개의 불량 Frame이 수신되면 단말기는 전력 入'leasurement Report
入/Iessage를 사용하여 기지국어］ 임계치 보고（Thresh아d reporting）를 한다. 기지국
은 P＼자艮THRESH ENABLE 필드를 1로 설정하고 이 필드를 佚X刃0으로 설정하
면 안 된다．
 PWR_REI乙FRAMES는 전력제어 Reporting Frame Cou毗로 주기보고（perio如
reporting)에서 사용되는 한 측정 주기의 Frame수를 나타내는 필드이다. 단말기가
불량 Frame의 개수를 세는 한 측정 주기의 Frame수는 다음과 같이 주어진다．
         2PWR_REP_FR1iES12 x 5
 PWR1THRESHEN／
             出LE는 Threshold report mode indicator로 기지국은 이
필드를 1로 설정함으로써 임계치 보고를 enable한다. 따라서 단말기는 망으로부터
수신한 임계치어］ 해당되는 Frame 에러가 발생하면 망으로 보고한다．
 그리고 Period report mode indicator인 P＼자R_PERIOI工ENABLE가 1로 설정
되어서 기지국으로부터 전송되어 오면 단말기는 정하困 시간마다 주기적으로 현재
의 FER상태를 망으로 보고한다．
 PWR_REP_DELAY는 전력 report delay이며, Frame 에러율 통계보고를 단말
기가 전력 入'leasurement Report Message를 통해서 한 후 수신한 전체 Frame과
에러 Frame의 값을 모두 reset시킨 후 "PwI亡REP DELAYX4 Frame" 동안
Frame 카운터를 동작하지 않게 하는 것이다. 이것은 Forw可d 링크의 전력을 제어
하기 위해서 필드 상황을 보고하였으나, 지금 전송한 PMR1\ 們］ 의해서 Forw打（I 링
크의 전력제어가 아직 적용되지 않는 시간, 즉 다시 말하면, 지금 보고한 사항이 반
영되지 않는 Forward 링크에서의 상황을 수집하여 보고할 필요가 없기 때문어］ 이
러한 시간지연이 필요하다．
                                       PSMM어］ 의해
                             PSMM읔     서   전력 제어가
                             보고한 시 점   반영된 시점



                                 tfl       t1
                                        1n에 PSMM윤 통해 "I L1고한 1
                          叫향 전력 세어를
                                        방향 링크 정보가 아직 日I .
                           서 순방향 링
                                        않은 구역임 . 따라서 이 r
                        ！이 IER윤 측정
                                        링크 忿보가 ti이후의 링크 징보
                                        와 합쳐 지민 안됨，



                        （그림 5-18) PWR 딕EP DE匕AY의 개념도
                                                     265


 System Parameter 八'lessage의 기능은 비단 전력제어 관련 정보뿐만 아니라 여
러 가지 정보가 더 많이 추가되어 있다（부록 참고）. 그러나 전력제어만을 위한 메시
지로 지금까지 설명한 필드를 가지고 있는 전력제어 Parameter 入4essage가 있다．
이 메시지는 入4SG TYI下 필드, 공통 필드, RESERVED 필드를 제외하면 System
Parameter 入4essage어］서 설명퇸 5개의 필드만을 갖고 이를 전송하는 전력제어 전
담하는 메시지라고 할 수 있다.


 Parameter Measurement Report Message

 기지국이 Forw町d 통화채널 전력제어를 enable하면 단말기는 전력 Measurement
Report 入lessage를 사용하여 기지국어］ Frame 에러율 통계（Frame error rate
stat始tics）를 보고한다. Reverse 통화채널을 통하여 기지국어］ 보내지는 메시지로
전력제어와 관계된 필드는 （표 5-旬와 같다．


                  （표 5-5) PMRM의 전력저뻐 관련 필드

                       필드                     길이（bit)
        ERRORS DETECTED                         S
        PwI{ 八tIERS FRA八tIES                    10
        DCCH1PWI｛소'IEAS小INCL                    1
        DCCHPWR_MEASFRAMES                   0 혹인 10
        DCCH_ERRORS_DETECTED                  0 혹은 5
        SCRYW小EASJNCL                           I
        SCH_ID                                0 혹은 1
        SCH PWI{ 入'WAS FRA入4ES               0 혹은 16
        SCH ERRORS DETECTED                  0 혹은 10



 여가에서 ERRORS_DETECTED는 검출된 Frame Error 수 이다. 한 측정 주기
동안 수신된 불량 Frame의 수가 31보다 작거나 같으면 단말기는 이 필드를
BAJ工FRAMESs로 설정한다. 만약 불량 Frame의 수가 31을 초과하면 단말기는
이 필드를 11111로 설정한다．
 또 P＼자RMEAS-FRAMESs는 한 측정 주기의 Forw可d 통화채널의 수이다. 단
    266                                                       5. 전력제어
                                                                        U

말기는 이 필드를 한 측정 주기 동안의 Forw打（:1 통화채널의 Frame수（TOTAL
Fr缸neSS）로 설정한다．
  IS -95C에서는 DCCH와 SCH를 위해서 ＜표 5-5）의 색칠해진 부분이 추가되었
다. 즉 이 메시지에 DCCH관련 FER 통계보고를 한다는 것을 표시하기 위해서
DCCHH P玖TR小4EAS卞爪CL를 사용하고 이어서 DCCH의 전체 수신 Fran祀수
와 에러가 발견된 Fran妃수를 각각 DCCHHPWR소EEAS_Fr계nes와 DCCH1
ERRORS卜DETECTED로 나타내었다．
  Supplemental Channel의 경우도 마찬가지로 FER 통계보고를 한다는 지시자
(SCH_P＼자R소4EAS工나CL）와 전체 Frame수（SCHPWR小4EAS_Frames), 그리
고 에러가 발견퇸 Frame(SCH_ERRORS_DETECTED）을 나타내었다. 추가적으
로 Supplemental Channel의 채널 번호（SCH工기를 추가하여 나타닌作十．

「Power Control Message

  이 메시지는 IS-95C 이후 추가된 메시지로 전력제어와 관련퇸 전반적인 값들을
단말기에 전달해 주어 전력제어 환경을 설정하는테 사용퇸다. 여기에는 다음 절에
서 이야기될 O毗er Loop Power Control 관련 값들도 포함되어 있다. 여기에서는
O毗er Loop Power Contr아와 관련된 부분은 생략하겠다．
 PWR_CNTL_STEP 은 폐루프 전력제어를 위해서 제공되는 전력증가 혹은 감소
의 폭을 지정해 주는 값이다. 이 값은 IS弱A에서는 1dB로 고정된 값이었다. 이 값
은 다음의 （표 5-旬과 같이 설정된다.
 FPC工寸CL은 Forw可（I 전력제어 관련정보가 이 필드가 포함된 메시지어］ 포함되
어 있는지 여부를 나타내는 필드이다. 1이면 포함되어 있는 것이다．


              （표 5-6) Closed Loo口 Power Contr이 Ste口 Size
          PWR CNTL STEP                       전력제어 Ste口 미ze
               000                                 1
               001                                0.5
               010                                0.25


 FPC_OLPC_FCHJNCL은 Forw町d 채널 O毗er Loop Power Control 관련
                                                    267


Parameter가 포함되어 있는지 여부를 나타내는 것으로 이와 비슷한 개념의
Forw可d   DCCH에     대한    FPC_OLPC_DCCH_INCL와   SCH에       대한
FPC_OLPC_SCH_INCL가 있다．


   5.6.2 Frame error Rate 통계보고

 Frame 에러율 통계보고는 주기 보고와 임계치 보고의 두 가지가 있다. 주기 보고
와 임계치 보고는 동시에 둘 다 enable될 수도 있고, 둘 중 하나만 enable될 수도
있고, 어떤 순간에는 둘 다 disable될 수도 있다．
 주기보고（Periodic Reporting）는 PWR_PERIOI工ENABLE 필드를 1로 설정함
으로써 enable된다. 한 측정 주기 동안 수신된 불량 Fran祀의 수를 규정된 기간마다
기지국어］ 보고한다. 측정 주기는 PwI｛尸RET乙FRAIVIE5로 확인할 수 있다.
 임계치 보고（Threshold Report恤g）는 P＼자RTHRESHENABLE 필드를 1로
설정함으로써 enable된다. 측정 주기어］ 상관없이 수신퇸 불량 Frame의 수가 규정
퇸 임계치어］ 도달할 때마다 기지국어］ 보고한다. 불량 Frame수의 임계치값은
們TR1REP叫THRESH로 정의된다.
 이것을 위해서 전체 Frame과 에러가 발생퇸 Frame coui抗er가 필요할 것이며，
이러한 카운터는 Fundamental Channel은 물론 DCCH와 Supplemental Channel
어］ 대해서도 동일하게 설정되어 있고 관련될 것이다．


   5.6.3 단말기의 동작

 Forw可d 통화채널 전력제어를 위해 단말기는 Frame 에러율 통계를 기지국어］ 보
고한다. 기지국이 주기 보고를 enable하면 단말기는 규정퇸 시간마다 Frame 에러
율 통계를 기지국어］ 보고한다. 기지국이 임계치 보고를 enable하면 단말기는
Frame 에러율이 규정된 임계치어］ 도달할 때마다 Frame 에러율 통계를 기지국어］
보고한다. 주기 보고와 임계치 보고는 동시에 둘 다 enable될 수도 있고, 둘 중 하나
만 enable될 수도 있고, 어떤 순간에는 둘 디． disable될 수도 있다．


 Frame 카운터 유지

 단말기는 수신된 Frame의 수（TOT FRAIVIESs）를 세기 위한 카운터와 불량
Fran祀의 수 (BAJ工FRAMESS）를 세기 위한 카운터를 유지해야 한다. 여기서 불량
     268                                                          5. 전력제어
                                                                            1


Frame이란 Frame 카테고리（Frame category) 9와 10으로 분류되는 Fran祀을 말
한다． 단말기는 수신되는 Frame마다 다음과 같은 절차를 수행한다. 즉
  水 단말기는 TOT FRAMES5를 1 증가시켜야 한다．
  永 수신된 Frame이 불량일 경우는 BAD_FRAMESS를 1 증가시켜야 한다，
  米 임계치 보고가 enable되어 있고（P叭／艮THR丑SH玉NABLES = 1) BAD
    FRAMES5가 P＼자RREPTHRESHS와 같거나 주기 보고가 enable되어 있고
     (P＼자H니PERIODENABLES = 1), TOTFRA八띠E:Ss 가 2 PWR_ R丑P FRAM丑S"/2><5
    와 같으면 단말기는 전력 入4easurement Report Message를 기지국어］ 보내야
    한다．
  米 끄)T_PRAMESs이 2 PWR_REP_FRAMESs /2X5와 같으면 단말기는 TOThFRAMES5
    와 BAI工FRAMESs를 0으로 설정해야 한다．
  米 전력 八'leasurement Report Message를 보내고 난 후 단말기는 TOTH
    FRA入侄S5와 BAD_FRAMES5를 0으로 섣정해야 한다. 그리고 메시지 송신
    첫 Frame 이후 P＼자R_REP_ DELAYS 4 Frame의 시간 동안에는 두 카운터
    를 증가시키지 않아야 한다．


  Multi히ex Option에 따른 Forward 통화채널 Frame 분류

  multiplex optioni어］ 대하여 단말기는 수신되는 Forward 통화채널의 Frame을
14개의 카테고리로 분류한다. 그 중에서 9번과 10번으로 분류되는 "얹300 bps
Frame, Primary Traffic only, with bit errors", "Frame with insufficient Frame
quality"는 불량 Frame이다．
  카테고리 9는 Frame quality 血dicat아（CRC）는 Fran祀에 Bit 에러가 있음을 나
타내더라도 다른 Par缸neter로부터 9600bps 의 Frame을 수신했음을 알 수 있는 경
우이다. 카테고리 10은 수신된 Frame의 data rate를 결정할 수 없는 경우이거나 카
테고리 9에 속하지 않는 불량 Frame일 경우이다．
 또한 Multiplex Option 2어］ 대하여 단말기는 수신되는 Forw可d 통화채녈의
Frame을 26개의 카테고리로 분류한다. 그 중에서 26번으로 분류되는 "적절한 품질
을 갖지 못하는 Frame"만이 불량 Frame으로 구분된다. 이 카테고리는 단말기가
Frame을 수신은 했으나 Frame의 속도를 결정할 수 없거나 에러가 검출되었을 때
어］ 사용되는 것이다．
                                                                                                            269
                                                                                                                  I
   5.6.4 Gain 조정

 각 Forward Code Chann이의 전송전력은 기지국 변조기 ASIC의 gain stage어］
서 조정된다（기지국 변조기 ASI(刈 Block Diagram을 참조）. gain stage에서는 전
송되는 신호의 파형을 주어진 scale factor어］ 따라 키우거나 줄인다. scale fact야는
변조기의 레지스터（GAIN_SO과 GAThL없）어］ 쓰여지는 7 Bit의 숫자로 digital
gain 또는 Forw可d ga血이라고도 한다. 따라서 127단계의 전력제어가 이루어진다．
scale fact아가 0일 경우는 아무런 신호도 전송하지 않는 경우이다．


        ALPHA[8:                        BETA[ 8: 0]                     GAMMA[ 8: 0]

                   Data Combiner and Multipluxer
                              AAA
                                                 n      卄A
                                               Gain          Gain
                                               는江age    Stage
                                               卜" IS     FIX
                                               Filter   Filter
                                                 4                  +
                                    Pilot PN                 1           Pilot PN
                                   Genera加r                         4    Generator


                                                     十十                   Q Phase
                                    I Phase

                                                 Walsh
                                             如누 Sequence
                                                 Cover
      Puncture
       Contr아


     Long Code =      블럭                 i     C。
                                                nv。
                                                  luti。
                                                      nal且nCoder                                      ADDl5:O]
        PN      켜 Inter                 口         K=9, r=1/2     寸1 Mit 汀pro: : ri                    Data[7:O]
     Scrambler                                                         Interface                    Cs
           ＋껸쁘：口』     뷸럭                뇨                                                           RD/
                                                                                                    WR
       L)브e川M    커   Interleaver        !
                                                                                      Timing     니1 ENC DMAR
      臘妥長                                                                            Generator
                                                                                                 中中 ENC n寸
                                                                                                 -  PPBOMS
                                                                                                 -  CHIPXB


                                             （그림 5-19) 卜,lodulator




 기지국 변조기 ASI(二 의 Write 레지스터

 Forw可d 링크 전력제어어］ 관계된 기지국 변조기 ASIC의 \write 레지스터는（표
5-7）과 같다．
       270


                 （표 5-7) 기지국 변조기 ASIC）의 전력저뻐 관련 write 레지스터

  Add                     Reg囹er or 日it
         R/W       Bits                                         Descripdon
 (He지                        Name

                                          Update 80 ms. When set to 1, the gain and
                                          output     control   mode         select   bits        for   the
                                          gain/combiner stage will take effect on the next
 OF          W      0     UPDATEH80MS
                                          internal    trans毗         system 80 ms bound可y
                                          following the write. When set to 0, these bits
                                          will take effect when written.
                                          Section 0 Forw缸d Channel Gain. This is the
                                          scaling    factor    如r     the 打an師血             section 0
                                          Forw可d Channel gain. Values range from 0 to
                                          127.     The    transmit      waveform            is     scaled
  24               6:0                    accordingly after the FIR filtering. The new
                                          gain information will take effect either when
                                          written or at the next internal tramsmit system
                                          80 ms frame boudary according to the setting of
                                          UPDATE 80MS.
  27                       RESERVED
                                          Section 1 Forward Channel Gain. This is the
                                          scaling    factor    for    the    transmit       section 1
                                          Forward Channel gain. Values range from 0 to
                                          127.     The    transmit      waveform            is     scaled
  2C               6:0      GAIN SI       accordingly after the FIR filtering. The new
                                          gain information will take effect either when
                                          written or at the next internal tramsmit system
                                          80 ms frame boudary according to the setting of
                                          UPDATE 80MS.
  2F                       RESERVED



 Gain 설정

 변조기의 GAIN SO과 GAIN Si의 레지스터어］ scale factor를 쓰는 일은 void
encoder_hndlr() 와 \Va1sh Symb아 인터럽트 Handler인 void Symbol_hndlr(）에
                                                        271
U                                                   1

서 이루어진다．


 Encoder 인터럽트 Handler

 Encoder 인터럽트는 20ms마다 일어나며 타이밍은 20ms 경계에서 2ms 전이다．
encoder_hndlr(）은 tx_Traffic_type이 SEL小DATA인 경우 일련의 함수 Paging
과정을 거쳐 void set_new丑aiw끄ag(）를 Pagii坦한다．
 set_new_gain끄ag(）는 변수 new_gain_saved를 TRUE로 설정하는 단 한 가지
의 작업만 한다. 변수 new召am_saved는 Selector/Vocoder로부터 scale factor어］
대한 새로운 값이 보내져와 지정된 저장장소어］ 저장되었음을 나타내는 플래그（flag)
이다. new_
       gain_saved가 TRUE일 경우만 변조기의 GAIN_SO과 GAIN_Si 레지
스터어］ scale fact아를 직접 쓰는 함수 void write_new_
                                         gain_to_mod(）가 Paging
된다．


 Symb아 인터럽트 Handler

 208.333"· 尸S마다 발생하는 \Valsh Symb이 인터럽트를 처리하는 routine으로
write_new_gain_切_mod(）를 Pagir垠하는 것은 \Valsh Symb이 인터럽트 Handler
인 Symbol小hndlr(）이다. S恥nb아_hndlr()은 자신이 실행될 때마다 지금의 시간이
20ms 경계인가 점검한다. 2劤TIS 경계일 경우 Selector/Vocoder로부터 새로운 gain
이 전송되어 왔다면（new丑am_saved = TRUE일 경우） write_n이v_g帥1的mod()
를 Pagir垠하여 새로운 gain을 기지국 변조기의 해당 레지스터에 기록한다．


    5.6.5 전력관리

 Forw打d CDMA 채널의 전력은 각 기지국, 섹터, 그리고 FA에 대하여 정해져
있다. 따라서 Forw可d CDMA 채널의 전력을 각 Code Channel어］ 대하여 적절히
할당함으로써 전력관리를 한다．


 전력 뱅크
 전력 bank는 한 Forward CDMI\ 채널의 전력을 저장하는 장소이다. Code
Channel이 active되면 전력 bani（에서 적당량의 전력을 빼서 해당 채널에 할당한다．
active Code Channel이 inactive되면 해당 채널의 전력을 전력 bank에 저장한다．
     272



active Code Channel의 전력 필요량이 변화되면 현재의 전력을 전력 bank어］ 반납
하고 요구된 새로운 전력을 해당 채널에 할당한다．
  다른 셀이나 섹터어］ 대한 간섭 때문어］ 한 Forward CI呱4A 채널은 규정된 전력
이상을 사용할 수 없다. 따라서, 전력 bank에 전력 여분이 없는 상태에서 C에e
Channel어］ 의해 전력이 요구될 경우, 기존의 전력 할당분을 조정하여 전력 요구에
응하던가（S加ffle down), 또는 P如t 채널의 전력을 줄임으로써 전력 요구에 대응한
다（cell si끄ink).


  전력관리 절차

  단말기에서 송신되는 전력 Measurement Report Message는 곧 바로 Selector/
Vocoder로 보내져서 F아w可d gain 결정어］ 이용된다. 결정퇸 Forward gain는 통
화채녈로 보내져서 Encoder 인터럽트 Handiler와 \Valsh Symb아 인터럽트
Handiler어］ 의해 기지국 변조기의 관련 레지스터어］ 기록된다. 이따1 새로 설정된
gain 이 high Threshold 와 low Thresh아d로 이루어지는 범위를 넘어서면（즉 타
당하지 않는 디지털 ga血이 발생되면） 통화채널은 Forward Lii血 전력제어 Report
Message를 BTSC 로 보내 현재의 gain 레벨을 알린다. Forw可（I Link 전력제어
Report Message는 주기적으로도 보내진다．
  BSC에서는 Forw町（I Link 전력제어 Report Message의 메시지 Handler인
cc_pwr_I就_msg_hdlr("·）를 호출한다．
  cc小wri祉_msg小hdlr("·）는 effective_Tra付1<：召ain(·"）을 호출하여 통화채널이
보내온 gain을 전력 bank 관리어］ 사용되는 effective gain으로 변환시키고，
rea＆兀ate上＝전력（···）을 호출한다. realli兀ate上：쪼i력（···）은 현재의 전력을 전력
bani但 반환하고 새로운 gain어］ 해당하는 전력을 해당 채널어］ 할당한다．


    5.6.6 EIB／아B에 의한 방법

 삭제 지시자 Bit를 사용하는 방법으로 IS弱A/B의 Rate Set 2에서 사용되어 온
방식이다． 이것은 앞서 이야기된 QIB를 사용하는 것과 비슷하나, 이것은 그것의 위
치가 음성 Frame어］ 위치하게 된다．
 불량 Fr跏e을 수신한 단말기는 기지국 송신 Frame을 통해서 삭제 지시자 bit를
'1'로 설정하여 기지국어］ 불량 Frame 수신을 알린다. 기지국은 可B를 '1'로 수신하
                                                 273
                                                       I
면 단말기가 Bad Fr계ne을 수신한 것으로 판단하고 이것을 Svc의 SPCB에 보고
한다. 단말기로부터 EBI='1'을 특정한 Threshold 이상 연속해서 수신한 경우 기지
국은 채널 상황어］ 따라서 전력제어를 수행한다. 이러한 Thresho닢는 Bad Frame이
연속해서 2번 또는 250개의 연속된 Frame 중 4개 이상 Bad Frame이 존재하는 경
우로 한다．
     이러한 EIB를 사용하는 전력제어를 위해서는 FPC_State, 즉 Forward 전력제어
State를 관리하며 전력제어를 실시한다. FP(二State는 F아＼V可d Link 채널의 상태
를 2가지의 형태로 나타내는데 상태가 양호하다는 FPC_State_Good과 상태가 좋지
않다는 FPC_State_Erasui氾로 표시한다. 초기 상태에는 항상 FPC_State_Good으
로 표시하도록 한다. 이러한 상태의 변화는 수신되는 Effi의 상태를 축적하여 결정
하게 된다．
     채널 이득의 상향 조정은 삭제 지시자 B北（EIB）가 연속해서 T뇨esh아d만큼 '1'이
수신되면, 즉 좋지 않은 상태의 Frame이 연속해서 임계치만큼 수신되었다고 보고
된다면, 기지국은 FP(二State어］ 따라서 채널 이득을 다른 폭으로 상향 조정하게 된
다．
     이러한 경우어］ FPC_St毗e_Good인 상태였다면 채널 이득을 작게（SMALL_UP
DELTA) 증가시킨다. 그러나 FPC_State_ Erasi.可e 인 상태였다면 채널 이득을 크
게（BIG尸UP DELTA) 증가시킨다. 즉 현 상태가 좋은 상태에서 수신퇸 E1B는 일시
적인 현상일 수 있다고 판단한 것이고 현 상태가 좋지 않은 상태에서 수신된
EIBBit가 1인 경우는 계속해서 좋지않은 상태가 지속되고 있다는 의미이므로 강한
전력증가를 요구하게 되는 것이다． 일종의 가중처벌의 이치와 비슷하다．
     채널 이득의 하향 조정은 상향 조정과는 완전히 별개로 이루어진다. 즉 상향 조정
의 조정요인이 Effi였지만, 하향 조정을 위해서는 EIB가 양호한 Fr可ne이라는 것은
더 이상 조정요인이 될 수 없다. 이 말은 채널환경에서 양호한 Frame이 수신되는
것은 당연한 것이지 전력을 하향 조정할 만한 근거가 되지 못한다는 이야기이다. 때
문어］ 하향 조정을 위해서는 타이머를 이용하며, 타이머의 설정시간은 채널 상태에
따라서 변하게 한다．
     타이머가 종료되면 채널 이득을 정해진 만큼 감소시키고 타이머를 현재의 Down
Time 값으로 다시 설정한다. 즉 전력을 증가시키는 요인이 있었으나 시간이 지나도
더 증가해야겠다는 것이 없다면, 그것은 전력을 감소하라는 채널환경의 묵시척인
                                                                             5. 전력제어
I11
        274_a                                                                          1


의미라고 이해해야 한디는 것이다．
      이때 Down Tin祀은 FP(二state가 어느 상태이냐에 따라서 증가 또는 감소한다．
즉 FP(二Sta扼니Good인 경우 Down T油e은 T油e-down Delta만큼 감소시키고
FPC_State_ Erasure인 경우 Down Time은 Time-up Delta만큼 증가시킨다. 즉
timer를 더 길게 가져가게 한다는 이야기는 전력증가 요청이 더 있을 것이라는 이
야기가 되고 짧게 한다는 것은 지금 현재 전력이 충분히 강하다는 것이며, 아울러서
더 이상의 전력증가 요청이 없을 것이라는 예측어］ 의해서 이루어지는 절차라고 할
것이다．

                                 Category 26 「   11

           수신된 프레임         卜1           1              1+
                                                            1       j+
                                                                         2

                       띠1- 20mses 十



                                             \\\lB가                 ，로 설정
                                                                4
           전송할 프레임         卜1                         i+
                                                            1       1+
                                                                         2

                           （그림 5-20) 日B의 전송


      Effi Bit는 RS2의 각 Frame의 가장 앞어］ iBit로 설정하게 되며, Forward으로
수신된 Frame의 2Frame 후의 Reverse Frame어］ 표시되어서 기지국으로 전송퇸다．
      이러한 전력제어는 20ms마다 한번씩 이뤄지는 5o1也의 빠르기로 이루어진다. 이
것은 앞의 폐루프 전력제어의 （표 5-2）의 내용과 비슷하다. 그러나 그것과의 차이
는 그것은 501七의 빈도로 전력제어가 일어나지만 한 Frame당 16개의 EIB/QIB가
2번째 전의 Fran犯의 질을 나타낸다．
      또한 그것의 정보는 Pilot 채널을 복조할 때 알아낼 수 있는 형태이나 이 방법의
경우 Frame을 복조해야만 확인할 수 있다는 차이가 있다．



      5.7 0uter Loop Power Control

      CDMA에서 Tra州c Frame은 2（뇨玲이며, Frame 단위로 전력제어를 한다면
1.25ms단위로 이루어지는 Fast 전력제어보다는 느리게 진행되나, 이러한 전력제어
     5 . 전력제어
                                                                           275
1


는 Closed Loop Power Contr아가 carrier 신호품질어］ 근거하여 전력제어를 하는
반면 최종 복호 대상이 되는 Frame어］ 의한 전력제어는 bearer data의 품질에 근거
하여 전력제어가 이루어진다는 점이 다르다고 할 수 있다．
    이러한 전력제어는 Closed Loop Power Contr아의 Set＋여nt설정을 위한 Outer
Loop Power Control가 있으며, Forw可（l 링크를 통해서 내려오는 전력
八4easurement Parameter어］ 의해서 이루어지는 Reverse 전력제어는 RC1인 경우
에 적용된 방법이 있으며, RC2인 경우 Reverse Frame어］ 포함퇸 EIB(Erase
Indicator Bit）를 통하써 이루어지는 Reverse 전력제어가 있다．

        역방향
        TCH 프레임




                                       Error:가 발생한
                                       프레 임 수와 rate에
                                       따라 覓咐1, Set
                                       Paint결정      " '          ,
                                                                     ,,/


                                                           ///
                                     ＼戈                i
                                          "\      //
                                               a뇨；
                           기지국


                  （그림 5-21) Outer Loo口 Power Con甘이의 개념도


    0毗er Loop Power Contr이의 목적은 현재 진행되고 있는 Closed Loop Power
Cor血이를 위한 Set-Point를 갱신해 주기 위한 것이다. 앞서 이야기되었듯이
Closed Lc叩 Power Contr아는 하나의 전력제어 그룹 단위로 Eb/NO를 계산하여
미리 설정퇸 Threshold와 비교하여 출력 전력제어 그룹에 전력제어 Command를
추가하여 전송한다. 여기에서 사용되는 Threshold는 앞서서 진행되었던 Closed
Loop Power Contr이로 전력이 반영된 Carrier어］ 의해서 전달퇸 Data, 즉 Frame의
품질과 연관되어 있는 값이어야 한다. 이러한 값을 우리는 Set-Poi砒라고 한다．
    이러한 Set-Point를 갱신해 주는 Outer Loop 전력은 Carrier신호에 근거하여 이
루어지는 전력제어가 좀 더 현실감 있게 Frame의 품질어］ 근거한 값을 T뇨eshold
로 사용할 수 있게 한다．
    （그림 5-19）에서는 SVC는 CE로부터 Frame을 받아 Error 여부와 Frame rate어］
   276
                                                                 1


따라 Eb/Nt Set-Point을 증감시킨다. 증감은 1 Frame 단위로 일어나며 증감범위
와 Step 크기는 System Parameter로 설정할 수 있다．


   5.7.1 Outer Loop Power Contr이 관런 시스템 Parameter

 외부 루프 전력제어를 위해서 시스템은 다음의 （표 5-8泣｝같은 Parameter를 정
의하써 전력제어를 실시한다．


                    （표 5-8) 외부 루프 Param아er

  Parameter                FuU Name            卜幻minal Va'ue

    pnom       전력제어 Nomin出                      19416(7.5dB)

    pmax       전력제어 八4ax                            34256(9dB)

    pmin       전력제어 八uin                            8288(5dB)

    pupf       전력제어 Up Full                            3072

    pupe       전력제어 Up Erasure                         248

    pupel      전력제어 Up Erasure Little                   50

    pd         전력제어 Down                                48

    pvd        전력제어 Variable Down                       4
    pfw        전력제어 Full Wait                           1
    可rr        전력제어 Run Reset                            2
    r光rl       전력제어 Run Limit                           5



 이상의 Parameter들 중에서         Pu可는 FULLRATEHRUN 入'I以le인 경우
T뇨e計iold 증가값을 나타내며, pupe는 erast玎C수가 5 이상인 경우어］ IDLE 八4ode
인 경우 Threshold 증가값이다. 이와 비교되는 erasure수가 5 이하인 경우의 IDLE
八4ode의 Threshold 증가값은 pupel 이다. 또한 pd와 pvd는 각각 FULL_RAT且‘
RUN 入4ode인 경우, 표）LE mode 인 경우 Threshold 감소값이다．
 즉 현재 수신되는 Frame의 상태어］ 따라서 임계치들을 달리 관리하므로 효과적
인 전력제어를 수행하는 것이다. 계속적으로 Full/I拓표Frame이 수신되는 상태인
FULL1RATERUI나 Mode 경우 전력증감의 폭이 다른 상태어］ 비해서 훨씬 크디＝
    5. 전력제어                                                                                                             277
1


     5.7.2 0uter Loop Power Control Algorithm

    Outer Loop Power Control는 Outlo叩S切此상태, Outlo叩尸Fu止Rate_Run 상
태, O毗lo야兀Idle상태들을 관리하며 수행한다. 이러한 상태들은 각각의 다른 전력제
어를 위한 Parameter 값들을 가지고 전력제어를 수행하게 되므로 상태의 천이요인
이 전력제어를 수행하는 중요한 근거가 된다．
    상태 천이도
    이러한 상태들의 천이가 이루어지는 triggering pointer는 svC의 Vocoder는 수
신 Frame을 다음과 같이 구분하여 처리한다．
    * Fu끄 rate : 9600 bps Frame
    * Half rate : 4800 bps Frame
    * Quarter rate : 2400 bps Frame
    * Eighth rate : 1200 bps Frame
    * F毗likely : 9600 bps Frame with bit error(CRC Error)
    水 Erasure : Frame의 Data Rate 알 수 없는 경우
    Outlo叩_Start상태에서는 수신되는 Fra工ne이 Fu끄이나 Half Rate 등과 같이 음
성복조어］ 모음 성분들어］ 일반적으로 대응되는 Fran祀이 수신되지 않으면 상태천이
는 이루어지지 않으며, 그러한 Frame이 수신될 때 비로서 0毗10叩1Full_Rate_Run



                                                                                          /／戶＼                   ,




                                                                                                             Half
                                                                                 OUTLOOP FUL
                                                                                  I RATE RUN                     J
                                                                                                          Erasure
                               /／卜


        9
        Quarter   ,   ,   ,7
                                                    汐／                 Quarter
                                                                                                 仄，   ;   Full_likely

        Ei延hth                                                         El只hth
        Erasure                      OUTLOOP START                             1
        Full_likely                                                    Erasure
                                                                       Full_likely




                                                ,   ,

                                                El日hth
                                                         ,   ,
                                                                 //\               1
                                                Erasure                          OUTLOOP IDLE
                                                Full_likely




                                     （그림 5-22) 외부 匕00口 전력저때 상태천이도
   278



상태로 천이가 이루어진다．
 또한 0utloop_I七止Rate_Run 상태가 유지되기 위해서는 계속적으로 Full이나
Half rate의 Frame들이 수신되어야 한다. 만약 Quarter이나 可ghth 등과 같은
Fran祀이 수신되면 그것의 상태는 Outlooj：
                           匕Idle로 천이된다．
 물론 0毗oopJdle상태에서도 계속적으로 Full이나 Half rate 수신퇸다면 Outloop_
Full_Rate_Run 상태로 천이가 이루어질 것이며, Fu끄이나 Half rate가 계속적으로
수신퇸다면 현 상태, 즉 Outloop_Idle를 계속 유지할 것이다．
 어느 상태이튼 CRC 에러가 동반된 Full rate의 데이터인 Fu止likely와 Frame의
정체를 알 수 없는 Eras네re를 수신하게 되면 최근어］ 수신한 Frame어］ 따라서 현 상
태를 유지할지 아니면 다른 상태로 천이될지가 결정된다.


 OUTLOOP START State

 Outer Loop Power Control가 시작될 때 들어오는 state로 해당 호어］ 대한 최초
의 Rx Frai끄e이거나 호 시작 후 Full 또는 half rate Frame이 한 번도 수신되지
않는 경우이며, 전력제어 임계치를 Nominal 값으로 설정한다．
 Rate가 F吐이거나 half인 경우만 다음 Frame 처리시 Fu止Ra扼1Run상태로 천
이되어 임계치 갱신을 위한 동작을 한다．


                  OUTLOOP START




                                    No



                       Yes




                 START=OUTLOOP FU

                   LL RATE RUN




            (그림 5-23) OUTLOOPSTART State flow Chart
                                                                279




 OUTLOOP FULL RATE RUN State

 이전 Frame이 ful 혹은 ha寸인 경우 또는 Full/Half Frame이 연속 3회 이상 수신
된 상태에서 이전 Frame이 Erasi.可e나 FuliJikely로 수신된 경우어］ 이 상태의 임계
치들로 전력제어를 수행하게 된다. 즉 이전어］ Fu끄／Half Frame이 수신되었다면 현
재 들어오는 Frame이 Erast可e나 Fu止likely일지라도 Full/Half Frame이 수신되
고 있는 상태라고 판단할 수 있다는 생각이다．
 OUTLOOItFULLmRATERUN 상태에서 Full또는 Half Rate Frame을 직전
어］ 연속해서 3(=fi皿1num s찌rn)회 이상 수신하였다면 Frame어］ 에러가 없으므로
전력제어 임계치를 48로（rpd) 하향 조정한다. 이러한 하향 조정 최소치는 8288
(=p而n）이다．
 OUTLOOP_FULL_RATE_RUN 상태에서 Quarter또는 可ghth Rate Frame을
수신하면 다음 Frame 처리시 OUTLOO므Idle state로 천이하여 처리한다．
 OUTLOOP1FULL1RATERUN 상태에서 현재 Full_likely 또는 Erasure
Frame 수신하였을 때에는 이전 Frame이 연속해서 3（可ul匕mm_s찌rn）회 이상 Full
또는 Half로 수신되었고 임계치 증가작업이 직전 Frame 처리시 수행되지 않은 경
우에 한하여 임계치를 증가한다. 이러한 상향 조정 최대치는 342弱（=pmin）이다．

                                0UT LOOP - FULL
                                  RATE RUN


                                          1
                       FULL LIKELY or
                         ERASURE




    Th=min(Th+pupf,
                        full well cnt<O
          pma引
     Full well cnt=2




              (그J 5-24) OUTLOOP_FUL_RATE_RUN state Flow Chart
       280



     OUTLOOP IDLE

     OUTLOOP_IDLE 상태에서 Quate／可ghth/Erasure在뇨止likely인 Frame을 수
신하였거나 이전 Fu끄1Ra扼Run상태에서 Quate/Eighth/Erasure/Full_likely를 수
신하면 이 상태로 천이된다. 이 상태에서는 수신되는 Frame어］ 의해서 전력제어를
수행하고 상태천이를 한다．
     OUTLOOI乙IDLE 상태에서 Full/Half로 수신된 경우 다음 Frame은 Ful1_R毗e
Run상태에서 처리되어야 古냔로 상태를 갱신한다．
     Rate가 Quarter/Eighth로 수신된 경우에는 전력제어 임계치를 4(=pvd) 감소시
킨다. 이때 하향 최소값은 8288(=pmin)이다．
     Rate가 Fulllikely在rasure로 수신된 경우에는 Frame 수신 후 연속 5(=per1)회
이상의 erasure나 加11_likely Frame이 수신되면 임계치 248( =pupe）증가한다．
     그 밖의 경우 임계치 馭)(=pu1刈） 증가한다. 이때 상향 조정값은 34256(=pmax）이
다．
                             OUTLOOP_
                              L RATE RUN
                                     F孤
                                           J三
                             FULL LIKELY
                                                                  +
                                                               FULL or
                             or ERASURE                         HALF




      era run cnt=O
      Th=max(Th+pvd
          ,pmln)




                      （그림 5-25) OUTLOOP IDLE sta也 Flow Chart
                                                         281


       5.7.3 단말기의 0uter Loop Power Contr아

      Forward 전력제어의 Eu/N洲］ 근거한 Closed Loop Power Control를 지원하기
위해서 IS-2000에서는 단말기에서 FER어］ 근거한 Outer Loop Power Control를
수행한다．
      단말기에서는 수신퇸 Forw可（I 전력제어 모드어］ 따라서 외부 루프를 지원할 것인
지를 결정할 것이다. 또한 외부 루프 관련퇸 전력제어를 위한 Parameter 등을 저장
한다．
      1/2차 전력제어 부채널 모두가 PCB를 전송하게 되는 형태인 For＼入／可d 전력제어
모드（FPC소4ODEs）가 '000', '001', '010' 인 경우어］ 단말기는 Forw町（I Dedicated
Contr이 채널, Forward Fundamental 채널, Forw可d Supplemental 채널을 포함
하는 모든 Forw可d 통화채널에 대해서 외부 루프를 지원한다. 또한 1차 전력제어
부채널은 PCB로 2차 전력제어 부채널은 EIB를 전송하게 되는 경우인 FPC小
MODEs ='110' 인 경우 단말기는 Forw可d Dedicated Control 채널 과 Forward
Fundamental 채널 등과 같은 채널이 단말기어］ 할당된 채널어］ 외부 루프를 실시한
다．
      만약 단말기가 Forw可d Fundamental 채널을 감시하고 있다면, 단말기는
加m訌在an祀의 Forward F끄idamental 채널상의 앉刃0bps 혹은 14400bps data rate
의 목표 FER을 이루기 위해서 FPC_FCH_CT刃RR_SETPTs(Eb/N0）을 조정한다．
FPC_ FC}LCURR_SETPTs가 FPC_FCH小4AXSETV八보다 클 때 단말기는
FPC尸 FCH_CURR_SETPTs를 FPC_FCHJVIAX_SETPTs으로 설정한다. 또는
FPC_ FCH_CURR_SETPTs가 FPC_FCH_MIftSETPTs보다 작을 때 단말기는
FPC_ FCH_CURR_SETPTs를 FPCJ구CHjVIINeSETPTs으로 설정한다. 이러한
방법은 Forw可（I Dedicated Control 채녈과 Forward Supplemental 채널어］ 대해
서도 비슷한 조치를 취한다. 탄 Supplemental Channel의 경우 최대 데이티 속도의
목표 FER이 조정의 대상이 퇸다．


       5.7.4 0uter Loop Power Control Parameter

      외부 루프를 수행하기 위해서 단말기는 다음과 갇은 정보들을 저장하고 관리한
 다．
  282


永 FPC_DELTA_SCH_SETPT: FCH의 Set的砒와 SCH의 S曲疝nt간의 차이
  이다. 즉 1차와2차 전력제어 부채널로 이루어지는 전력제어의 결과로 FER의
  차이를 나타내는 값이다. 이 값은 SCH의 Setpoint를 콴리하는 기준을 FCH의
  Setpoint어］ 근거해서 하기 때문이다．
米 FPC_DELTA_SETPT: FCH의 Setp*丘nt와 DCCH의 Setpoint간의 차이이다．
 이것 역시 DCCH의 Setpoint를 관리하는 기준을 FCH의 Set油nt어］ 근거해서
 하기 때문이다．
氷 FPC_FCH_CURR_SETI丁 : FCH의 전력제어 부채널 외부 루프의 Setpoint
  의 현재 값이다. 이와 비슷한 개념들로 채널에 따라서 Dedicated Control 채널
 의 경우, FPC_DCC且CURR_SETPT, Supplemental 채널의 경우 FPCH
 SCH_CURR_SETI玎［i]이다． 여기에서 i는 SCH의 식별번호를 나타낸다．
水 FPC_FCILFER : F-FCH의 목표 FER
 목표 FER은 다음의 （표 5-助와 같이 설정되어서 전송된다．


                         （표 5-9) 목표 FER
   尸E只의 2진 표현값                          Frame Error Rate
        00000                    0.2%
        00001-40100              0.5% - 10%(0.5%단위）
        10101 S- 11001          11% - 15%(0.5%단위）
        11010-11110             18% - 30%(0.5%단위）
        11111                    현재 사용치 않고 나중에 사용 예정


永 이것과 동일한 개념으로 Dedicated Control, Supplemental 채널 각각의 값은
 FPC_DCCH_FER, FPC_SCH_FERO다.
米 FPC_FCH小IAX SETPT: F-FCH의 전력제어 부채널 외부 루프 Se加曲lt의
 최대값을 나타내며, Fundamental 채널의 O毗er Loop E1JN0 Sel꾸oil此의 최대
 값을 나타낸다. 이것은 0.125dB 단위로 표시 설정된다. 이와 비슷한 개념들로
 채널에 따라서 Dedicated Control 채널은 FP(二DCCH소4AX1SETI丁, Sup
 plei그riental 채널은 FPC_SCH小4AXSETPT가 있다．
    5. 전력제어
                                                       283
U


 水 FPC_FCH소flN_SETPT: F-FCH의 전력제어 부채널 외부 루프 Se缸疝nt의
     최소값을 나타내며, Fundamental 채널의 O毗er Loop Eb/No Se加oint의 최소
    값을 나타낸다. 이것은 0.125dB 단위로 표시 설정된다. 이와 비슷한 개념들로
    채널에 따라서 Dedicated Control 채널은 FPC_DCCH소/IIXSETPT로 표시
     되며, Supplemental 채널은 FPC_SCH_MIX_SETPT로 표시되는 값이 있다．
 水 FPC소4ODE: Forw町d 전력제어 동작 모드
 水 FPC소'IOD且NO_.SCH : Forward Supplemental Channel 할당 간격 동안 여］
    견되는 Forw可d 전력제어 동작 모드
 米 FPC소4ODE_SCH : For刀町（I Supplemental Channel 할당 간격 동안의
    Forw可d 전력제어 동작 모드로 （표 千3) FPC小lODE에 따른 Forward 전력
     제어 Scheme어］ 나타나 있는 값으로 설정한다．
 米 FPC_PRI_CHAN : 전력제어 부채널 지시자로서 Forw町d Fundamental 채널
     어］ 전력제어 부채널이 다중화되어 있고 단말기가 이러한 채널을 수신해서 1차
     전력제어 제어를 단말기가 수행하면 0으로 설정하고, 이러한 동작을 DCCH어］
    대해서 수행하면 '1'로 설정한다. 따라서 Fundamental 채널이 할당되었다면 기
     지국은 이 필드를 '1'로 해서 전송할 것이다．
 永 FPC_SEC_CHAN : 入4aster Supplemental 채널 index로서 FPC소lODE가 1
    혹은 2일 때 八4aster Supplemental 채널 index로 설정해서 통보한다. 즉 이 채
     널어］ 대해서 전력제어를 하자고 통보한다．
 水 FPCSETPTTHRESH: DCCH의 전력제어 부채널 외부 루프 Setpoint 임
     계치로 단말기에서는 이 값을 outer loop report message로 보고하고 기지국
     은 이 값을 상향 조정하여 0.125dB단위로 설정해서 단말기어］ 통보한다. 이것과
     비슷한 개념의 값으로 FPCHSETPTTHRESHSCH이 있으며, 이 값은 SCH
     의 전력제어 부채널 외부 루프 Setpoint 임계치이다．



        이 장을 마치면서···                                         )
 전력제어는 RF신호의 전력을 제어하는 것이 아니라 RF어］ 감추어져 있는 개인의
정보어］ 대한 전력제어이다. 실지로 기지국에서는 여러 개의 신호를 동일한 RF출력
    284



(Ml毗일 수 있음）으로 출력할 것이다．
 단말기는 기지국의 Pilot 신호를 수신하면서 자신에게 주어지는 통화채널을 사용
함으로 통화 상태가 된다. 이때 단말기는 통화채널의 이득을 조절해 줄 것을 요청하
는데 이것이 전력제어가 된다．


   5.8.1 瓦刀％와 FER의 관계

  전력제어를 수행하는 요인은 Eb/No와 FER 두 가지 모두일 수 있다. 만약 아무
리 且屈0가 좋지 않다 하더라도 Vocoder에서 적당히 복호가 이루어질 수도 있는
것이다. 물론 이것의 역으로 瓦IN0은 아주 양호한데 FER이 좋지 않다면 어떻겠는
가9 물론 이러한 가정은 정상적이지 않을 수 있다. 그러나 양흐한 FER을 위해서 지
나치게 높은 瓦IN0를 설정해 놓을 수도 있다．
 전력제어도 결국은 전송하는 데이터의 무사한（?) 도착을 위해서 수행된다는 측면
에서 생각할 수 있다. 일반적으로 물리 계층에서는 이러한 작업을 위해서 수행하는
Channel Coding단계는 흔히 Forw缸d Error Correction(FEC）로 이루어진다. 즉
폐루프로 데이터 전송수신 확인 및 전송수정 등의 과정이 아니다．
 여기에서 이야기 하려고 하는 것은 瓦／N0에 근거해서 수행되는 전력제어는 물
리 계층에서 온전한 데이터의 수신을 위해서 취해지는 프로세스라고 한다는 측면에
서는 Channel Coding과 공통점이 있으나, Channel Coding 이 FEC의 형태라는 측
면어］ 대해서 이것은 전송되어진 정보의 품질정보가 Feedback되어서 다음의 즈｛송어］
반영퇸다는 것이 다르다. 물론 완전히 재전송을 요구하는 형태가 아니라 다음에 전
송할 데이터들의 전송 Parameter를, 이를테면 전력, 수정하는 것이다． 즉 다음 번
전송어］ 직전 데이터의 내용어］ 관한 정보가 Feedback된다는 측면에서 FEC와는 구
별된다고 할 수 있다．
 또한 FER에 근거한 전력제어의 경우 역시 결국은 데이터의 온전한 복구（혹은 복
호）이다. 이와 유사한 데이터 전송을 위한 RLP에서는 이런 경우 재전송을 요구하나
이것 역시 재전송은 이루어지지 않는 단지 전송과 관련된 직전 Frame의 채널정보
를 제공하므로 다음 번 전송에 반영하고자 하는 것이다．
 독자들의 오해를 막기 위해서 물론 RLP(Radio Link 까야oc아）와 FER과는 동
（同） 계위의 데이터들은 아니다. 다만 FEC(Forward Error Correction）와 /\IRQ
    5. 전력제어
                                              285
1


(Aut毗atic Re硏垠t Request）의 중간형태의 제어방식이 전력제어라는 이야기를 하
려고 시작한 이야기이다．

     5.8.2 전력제어의 불확실성

    앞서 공부한 이러한 전력제어를 수행한다 하더라도, 즉 해결해야 하는 몇 가지의
문제가 있다．
    첫째로는 널리 이야기되고 있듯이 Forw可d의 채널환경을 통해서 Reverse의 전
력제어를 한다는 것이다. 현재 상용 서비스되고 있는 CI呱4A시스템의 경우 Forward
과 Reverse은 충분한 주파수 이격거리（90MH기를 둔다. 이것은 FDD(Frequency
D如面on Duple幻 방식의 전형적인 모습이다. 이 거리는 코히어런스 대역폭을 충분
히 넘어서는 거리로 상관성이 거의 없다고 봐야 할 것이다．
    또 하나의 문제는 단말기가 Hi毗의 신호를 통하써 통화채널의 전력제어를 한다
는 것이다. Pilot 신호는 기지국에서 언제나 일정하게 출력된다. 단지 그것을 수신하
는 단말기의 위치나 다중경로 페이딩어］ 의해서 순간적 혹은 지속적으로 다른 단말
기와 차이가 날 수 있다. 어찌되었든 탄말기는 이러한 환경어］ 통화채널도 같이 놓여
있게 된다는 생각에서 Pu毗의 품질로 통화채널의 전력제어를 수행한다 ( 瓦刀％). 즉
전력제어는 통화채널을 조절하는데 Pu毗 채널은 언제나 같이 수신된다．

     5.8.3 간섭에1 대한 항후 방법들

    CDMA는 간섭제한 시스템이라는 이야기를 여기에서도 아니 할 수 없다. 이러한
간섭제한 시스템에서 간섭을 효과적으로 관리할 수 있는 방법이 이 장에서 공부한
전력제어 방식이다. 이러한 전력제어를 효과적으로 수행하기 위해서 전력제어 방식
들에 대한 갖가지 아이디어들이 속출하고 있다. 이를테면 전력제어 Bit에 따른 출력
의 증감 여부를 결정할 때 적응 Aigori由m으로 상황에 따라서 현재 입력Bit가 갇더
라도 출력을 다르거］ 적용하는 방식 등도 있다. 또한 간섭어］ 강력히 대응하기 위해서
간섭 제거기라든가 안테나의 섹터화의 확장 형태 혹은 발전 형태로 이해할 수 있는
스마트 안테나 등과 갇은 간섭보호（혹은 예방）시스템 들이 발전되고 있다. 많은 사
람들이 이러한 CDMA의 고민거리를 두고 많은 생각들을 했으며, 관련 기술들 을 발
전시켜 나가고 있다. 이러한 발전을 위한 노력들이 결국 처음 Qualcomm이 말했던
CDMA의 성능어］ 콴한 광고의 내용을 실현시켜 줄 것이다，
    6. Handoff                                   287
1




                                          Handoff




    셀룰러는 제한된 망 자원을 셀이라고 불리우는 특별히 제한된 지역에서 폐쇄적으
로 운영퇸다. 이러한 폐쇄적인 셀 운영은 망 자원을 재사용할 수 있다는 또 다른 공
유의 개념에서 비롯된 것이다. 때문어］ 이러한 폐쇄적인 셀을 다른 인접한 셀과의 상
호작용을 할 수 있게 해주는 것이 Handoff라는 수단이다. 돌이켜 보건대 셀룰러는
자원의 재사용이라는 용량적인 측면에서 폐쇄적인 셀을 사용했고 이러한 폐쇄적인
문제를 해결하는 대안이 Han面珏라는 이야기는 Han面侄가 셀룰러의 용량과 상당
한 관계가 있다는 이야기가 된다. 이러한 개넘을 가진 가운데 이 장을 시작하1 보자.
    Han面付는 셀룰러 이동전화 시스템에서 통화의 연속성을 보장하1 주거나 착신의
안정성을 보장하기 위한 절차라고 할 수 있다고 했다. 일반적으로 Hando卄는 통화
상태에서 이루어지는 것을 말하나 대기 상태에서도 시스템과 configuration정보와
page정보를 수신하기 위해서 유휴 Hando卄라고 불리는 절차를 사용한다．
    IS-95B 이상에서는 이러한 유휴 Hando珏의 개념으로 확장하여, 즉 Traffic 상태
가 아닌 경우의 Hando什를 확대하여 /\ccess Hando卄라는 개념이 도입되었다. 또
한 새로운 시gori出m을 사용하는 soft Hando侄의 도입으로 Handoff를 위한 예약
   288                                        6. Handoff
                                                           1


채널의 확보를 줄일 수 있어서 시스템 용량 증대의 효과를 가져왔으며，
MAHHO（八4obile Assistamt Hard Handoff）를 도입하여 주파수간의 Hard
Handoff시 Handoff 성공률을 높여 주는 방식도 새로운 방식으로 소개되고 있다．



 6.1 Handoff릍 위한 Parameter

 Han面卄는 현재 서비스되고 있는 통화채널이 여러 가지 상황（사용자가 이동하거
나 채널상황의 변동 등）으로 인해서 새력이 약해지고 그러한 과정에서 새로운 강한
신호가 수신될 때 단말기는 연속적인 서비스를 유지하기 위해서 새로운 강한 신호
로 통화채널을 변경하게 퇸다. 이러한 절차를 우리는 Handoff 혹은 핸드오버라고
한다．
 Handoff（혹은 Handover）라는 이름은 ce11ular system에서 한 셈에서 통화로를
잡고 있다가 다른 셀로 잡고 있턴 손（통화로）으로 넘긴다 혹은 끊는다는 의미에서
나온 말로서 두 가지 모두 같은 의미의 말이며, Handover라는 말은 유럽에서
Han面卄라는 말은 북미를 비롯한 한국에서 많이 쓰이고 있다．
 이러한 Han面卄는 새로운 채널로의 천이를 위한 과정에서 일련의 순서어］ 의하써
Soft Hando珏와 Hard Handoff로 나눌 수 있다. 즉 현재 서비스되고 있는 채널을
유지하는 가운데 새로운 채널로 또 다른 통화로를 열었다가 이 채널이 안정되면 기
존의 채널을 끊는（즉 make and break) Soft Handoff와 기존의 채널을 미리 끊고
새로운 채널을 잡는（break and make) Hard Han面珏라고 한다．
 현재 상용화되어 있는 CDMA cellular나 PCS의 경우 CDMA 방식의 다중접속
방식을 사용하므로 셀간어］ 주파수간의 Hando侄의 발생을 줄일 수 있으므로 make
and break방식인 soft Handoff로 Hando卄를 할 수 있다는 장점이 있다. 반면 주파
수로 셀간의 자원을 구분하는 방식인 FDMA에서는 셈간어］ Soft Handoff를 위해서
2개 이상의 대역 필터를 가지고 있어야만 가능하다.


   6.1.1 Pilot Set

 단말기는 경우어］ 따라서는 엄청나게 많은 신호를 수신한다. 그러므로 이러한
Han面ff작업을 위해서는 수신퇸 Pu毗 신호들을 강도어］ 따라서 구분하여 콴리해야
    6. Handoff                                                                 289
U


할 것이며, 그로 인한 Pilot 군의 수도 제한되어야 할 것이다. 때문어］ 그러한 Pu毗들
을 그것의 세기와 그 세기의 유지시간 등의 정보로 신호 복조용으로 사용할 수 있을
지 여부를 결정하기 위해서 다음과 같이 구분하여 관리한다．
 첫 번째로 /\ctive Set이다. 여기에 속한 Pu毗들은 Forward 통화채널(Walsh
（뇨de）이 할당된 채널로 단말기의 Rake 수신기의 Fir垠er가 할당퇸 Pu毗을 말한다．
이 Pilot Set은 단말기와 기지국간어］ 서로 통화로를 위해서 인정된 Pilot이라고 할
수 있다.
 두 번째는 Candidate Set이다. 여기어］ 속한 Pil毗들은 Fir乷er가 할당되지 않아서
실지로 신호를 복조하지는 않는 Pil毗이지만 충분히 복조할 수 있는 신호 강도를 가
지는 Pilot Set을 말한다. 이것은 A出ye Set와는 달리 단말기가 일방적으로 충분한
세기가 되었다고 인정되는 P11毗들이다．
 세 번째는 Neighbor Set이다. Handoff를 위하여 충분히 Candidate Set이 될 수
있는 Pilot PN Set들이 여기에 속한다. 즉 잠재된 Candidate Set이다．
 마지막으로 Remair血g Set의 Pu毗들은 단말기에서 수신되는 모든 Pilot PN Set
을 말한다. 즉 /\ctive, Candidate, Neighbor Set을 제외한 모든 P11毗들을 말한다．


                   , . . ,   . ,   " '   " "   '   "
                                                       Reniatniug
                                                                    Set   ,i
                  （그림 &]) 단말기의 미아 S이의 분류


 즉 Handoff가 일어날（혹은 통화로가 할당될） 수 있는 가능성어］ 따라서 /\ctive
Set, Candidate Set, Neighbor Set, Remaining Set를 나누었고 Thresh아d로 그
것의 수를 제한하여 관리하고 있다고 할 수 있다．
   290                                             6. Handoff
                                                                U


 IS-95C에서 단말기가 처리해야 할 Pu毗 Set은 A出ye Set이 최대 6개, Candidate
Set이 최대 10(5）개, Neighbor Set이 최소 40(20）개로 정의하고 있다. 따라서 단말
기는 현재 서비스 받고 있는 기지국을 포함하여 6개의 /\ctive Set을 가질 수 있으
므로 주위의 5개 PN Offset을 사용하는 기지국과 Han面if를 수행할 수 있다．
 단말기가 저장 및 관리하는 P11毗 Set은 （그림 6-1）과 같이 개념적으로 이해할 수
있다. 단말끼의 searcher는 지속적으로 /\ctive Set, Candidate   Set, Neighbor
Set, Remaining Set을 설정되어 있는 Se可ch Window 크기로 검색한다．


   6.1.2 Search 꿔indow

 단말기는 Se可ch Window를 통해서 각각의 P11毗 Set들을 감시하여 강도와 위상
정보 등을 얻어서 Pilot Set을 갱신한다. 이러한 Search Window의 크기를 망에서
는 호출채널을 통해서 단말기에게 알려 준다．
 호출채녈을 통해서 전송되는 System Parameter Message의 SRCHWINA /
SRCILWII'LN / SRCHWIN_R는 이러한 Search Window의 크기를 나타내는 항
목들이다．
 이러한 Se可ch Window은 연속적으로 틀어오는 Pilot 신호를 수신한 위치에서
일정한 처리를 위해서 관심을 가지고 보는 혹은 특정한 의미를 부여하기 위한 범위
라고 할 수 있다．
 Search Window의 중심에는 최초로 도착한（다중경로 성분의） 신호를 설정하여
Pilot 신호의 Offset을 찾기 위한 A毗아correlation을 윈도우 크기만큼 delay시켜
가며 시행한다（이러한 절차는 시스템 획득단계에서 이루어지며 자세한 내용은 이
책의 4장을 참고하라）. 물론 PN Code 전체어］ 컬쳐서 이러한 처리작업을 해야 하지
만 그것은 시스템 획득단계（이 책의 4장을 참고）에서는 가능하며, 이미 기준이 되는
PN Offset정보를 알고 있는 이상 다중경로어］ 의한 지연성부에 대한 검색만 수행하
면 될 것이다．
 따라서 Hando丘를 위한 Search Window의 경우 최단거리와 최장거리로 단말기
어］ 수신된 신호의 경로 차이를 보상해서 신호를 찾는다는 의미를 가진다. 최단거리
의 신호를 Search Window의 중앙어］ 잡고 혹시 바로 그 신호일지 모르는 지연성분
을 위하囚 창의 크기가 n chit汐］ 필요하게 된다. 그러므로 여기서 말하는 n ch如은
중앙어］ 위치한, 즉 최초로 도착한 신호와 경로차이가 n chip이 나는 신호라고 생각
 6. Handoff                                                      291



하고 검색한다. 이러한 이야기는 다음의 2가지 예제를 통해서 더욱 분명해 진다．

              CDMA망의 전파환경에서 단말기에서 직선경로는 1Km이다. 그리고
              다중경로 성분은 5Km이다. SRCH_砥江N1A의 크기는 얼마인가？

              CDMA 1 chip은 약 244m이므로 직선경로의 경우 약 4.lchip 지연
              이 생기게 되고 다중 경로의 경우 약 20.5chip정도 지연이 생긴다고
              볼 수 있다. 즉 최단거리를 가지는 신호를 Search Window의 가운더］
              어］ 둔다면 지연성분을 탐색하기 위해서는 지연 차이인 20.5c1五p
              4.1 chip = 16.4chip이 된다. 그러므로 창의 크기는 16.4의 2배인
              (32.8chip) 33chip 이어야 한다. 우리가 최초로 도착했다고 생각한
              신호를 Se계rch Window의 중앙어］ 두는 이유는 최초로 도착한 신호
              가 최종적으로 도착한 신호일 수도 있기 때문이다．
 0I刈6-2       그림과 같은 경우 )GY지역에서 Hando侄가 일어나게 하려면 Search
              Window의 크기는 어떻게 정의해야 하겠는가2
              경로차이가 가장 큰 경우는 x와 Y의 위치어］ 있는 각각의 단말기들
              은 Cell A/B로부터 신호를 수신하는 경우이다. 또한 이러한 2가지는
              동일한 조건이므로 x의 경우로 문제를 풀자.
              이 위치의 단말기의 경우 /\i13셀로부터 신호를 수신할 것이다． 물론
              복조할 수 있는 신호강도를 가질 것이다. 그렇다면 최초로 들어온 신
              호와 나중에 들어온 신호의 경로차이를 Search Window의 크기로
              설정하면 되므로 다음과 같이 풀이할 수 있다．
              x 위치에서 단말기가 수신한 A cell 신호와 B cell 신호의 지연거리
              는 4Km이므로 4000/244=16.4 ch加의 차이가 난다. 그러므로 창의
              크기는 16.4X2=32.8 ch如이므로 유효한 창의 크기는 33ch如이다．


               Cell A 孤         Soft Handoff 영역


                                                    A   cell B


                          6Km
                                  II) Km
                                            16 Km



        （그림 &2) X-Y에서 Soft Handoff가 일어나기 위한 SRCHJ川NA
   292                                            6. Handoff
                                                               a


 예제 6-2의 문제는 더 정확하게 이야기하면 단말기가 수신한 신호가 어떠한 경로
이튼 A cell의 신호는 6Km로 B cell로는 10Km의 경로로 수신되었다고 보아야지
기지국의 위치가 그렇다고 해석해서는 안 된다．
 SRCILW끄tA로는 적당한 크기의 RSSI가 계산되지 않는 신호는 현재 탐색중
인 신호의 지연성분이 아니라 새로운 신호라고 보아야 한다. 즉 현재 양호한 신호가
수신되는 기지국보다 훨씬 먼 거리에 위치한 기지국으로부터 온 신호라고 봐야 할
것이며, 이러한 신호는 현재 기준으로 잡고 있는 신호원보다 훨씬 먼 거리어］ 있으므
로 창의 크기가 훨씬 더 커야 한다. 물론 이렇게 큰 창으로 신호의 에너지를 측정하
여도 그 결과 값은 /\ctive Set의 그것보다 훨씬 작을 것이다．
 이렇게 훨씬 먼 거리어］ 있는 신호를 찾기 위한 창을 SRCH_WIN_N在｛이라 하고
Active Set이나 Candidate Set을 위한 창의 중앙을 가장 빨리 도착하는 PN 신호
로 한 것과는 달리 Neighbor Set, Remaining Set은 단말기의 시간을 기준으로 한
PN 성분으로 창의 중앙어］ 오게 한다. 여기에서 단말기 시간기준小心TR : 八4obile
Station T油e Reference）은 초기상태에서 동기채널로부터 수신한 system 出ne을
말한다. 정리하면 다음과 같다．
 水 SRCHWIN卜／\ : Act加e Set과 Can小date Set의 Search Window 크기
 木 SRCHW爪小 : Neighb才 Set의 Search Window 크기
 永 SRCH_WJN_R : Remaining Set의 Se계7ch Window 크기
 따라서 Search Window의 크기는 상기와 같이 결정되며 이것은 전파환경어］ 따
라서 시스템에서는 최적의 값을 할당하는 것이 통화품질을 위하여 매우 중요한 요
소가 된다. 위의 예제에서 최단거리 성분과 최장거리 성분은 이러한 전파환경어］ 의
해서 측정 혹은 정의될 수 있기 때문이다．
 일반적으로 기지국 간격이 좁은 대도시 밀집지역에서는 /\ctive Set의 Search
Window는 기지국의 서비스 영역이 상대적으로 넓은 시골 지역보다 좁게 설정되어
야 한다. 이것은 기지국간 거리가 먼 곳어］ 있는 시골 지역에서는 l너［ultipath Fading
어］ 의하여 주된 신호성분의 분포가 넓게 분포할 수 있기 때문이다.
 System Parameter Message에는 전송되는 Search Window의 크기 정보는 다
음의 （표 6-1）과 갇이 실제 chip수와 대응된다.
     6. Handoff                                               293
口

                     （표 6-1) Searcher Window 크기

      SRCH W八 A                      SRCH WIN A
   SRCH WIN N                        SRCH WIN N
                     Window Size                    Window Size
 SRCH WIN NGHBR                    SRCH WIN NGHBR
                      (PN chi口）                      (PN chip)
   SRCH W八 P                         SRCH WIN R
     CF SRCH WIN N                  CF SRCH WIN N

            0             4               8             60

           1             6                9             80
           2              8              10             100

           3             10              11             130
            4            14              12             160

           5             20              13             226

           6             28              14             320

           7             40              15             452


 예를 들어서, SRCH_WIN_A : 7(40 PN chips), SRCFL＼入／H나寸N: 9(80 PN
chips), SRCH_WIN_R: 10(100 PN chips）를 수신했다면 가장 단순히 생각할 때
이 시스템에서는 임의의 위치어］ 있는 단말기는 왕복거리를 생각할 때 4.88Km범위
의 기지국들의 Pul毗 신호를 /\ctive Set으로 하며, 9.76Km의 범위의 기지국들의
Pu'毗 신호를 Neighbor Set으로 한다. 또한 12.2Km 의 범위어］ 있는 기지국들의
Pilot 신호를 Remaining Set으로 한다는 것을 이야기할 수 있다．
 Active/Candidate Set Window 크기는 빠른 검색을 위해서 가능한 한 좁은
Search Window를 가져야 하지만 다중경로 페이딩 성분은 수용할 만큼은 커야 한
다. Candidate Set은 Traffic상태에만 설정되며 창의 크기는 /\ctive Set과 동일하
다.




 Neighbor Set Window 크기는 /\ctive/Canthdate Set Window와는 상대적으
로 먼 거리의 Pu毗을 검색하게 된다. 따라서 일반적으로 Neighbor Set Window7f
큰 값으로 설정된다. 이것은 또한 각 다중경로 페이딩 성분은 비슷한 크기로 넓게
분포되어 있기 때문에 이를 수용하기 위해서이다. Neighbor Set Window의 중심
은 단말기의 시간기준으로 PN이 설정된다．
 Remaining Set Window 크기는 검색이 가장 먼 거리의 Pu야을 검색하므로（전
                                                          6. Handoff
    294                                                                .

파지연이 넓게 분포） 일반적으로 가장 큰 크기의 M及ndow를 가진다. 이 \Vindow
역시 중심점은 단말기의 시간기준이다．




                            Search Remaining Set

                      （그림 &3) P11아 PN Set 검색


 여기서 우리가 한번 생각하1 볼 것은 Qualc아ian CDMA의 경우 동기식 방식으로
동일한 PN Long/Short Code를 사용하여 특정한 Offset으로 구분하는 방식이다．
여기에서는 지연으로 인해서 자칫 잘못된 신호로 오인할 수 있는 요인이 있으나 이
러한 것을 원천 해결을 위해서 Pu毗 index를 64 ch珀으로 함으로 신호의 다중경로
지연을 왕복하는 성분까지 생각할 때 7.8Km까지는 보장할 수 있다. 단말기는 Pu毗
increment를 기준으로 위의 검색창들을 지속적으로 검색하며, 효과적인 검색을 위
하여 Active와 Candidate Set을 먼저 검색하고 Neighbor, Remaining Set 순으로
검색한다.     PILOT皿寸C는     호출채널에서        Overhead     Message인   Extended
Neighbor List Message, 통화 상태에서는 Neighbor list update 八4essage로 전송
되며 Remaining Set 검색은 Pilot 증가 step어］ 정의된다. 예를 틀어 4로 설정되어
있으면 0, 4, 8, 12, ·．·의 순으로 검색퇸다. 실제 칩으로 정의하면 PILOTJNC x 64
c岫羚가 된다. （그림 价3）은 단말기가 각각의 Pilot Set들을 검색하는 과정을 나타
낸다．
 또한 Pul毗 increment를 통하囚 그러한 마진을 더욱 배가시킬 수 있다. 예를 들어
U
    6. Handoff
                                                  I
                                                      295
                                                            I
서 PILOT_INC=4이면 약 31Km의 다중경로까지 보상할 수 있다．


     6.1.3 Threshold

 단말기는 Pilot Set의 분류를 위해서 각각의 Pu毗의 에너지기준과 시간 기준을
가지고 분류하며 관리하고 있다. 이러한 에너지 기준은 TADD, TDR아）,
TCOM甲들이고 시간 기준은 T_TDROP Parameter를 이용한다. 이들의 의미는
다윽과 갇다．


 T ADD

 Neighbor Set에서 Candidate   Set이 되기 위한 기준점, 즉 Neighbor Set의
P11毗이 TADD를 넘어서면 Candidate Set으로 천이된다. 즉 이 값은 수신되는
신호를 충분히 복조할 수 있다고 판단이 되는 신호강도 point라고 할 수 있다．


        op
 Active Set에서 ThTDROP이 동작하는 기준점， 즉 이 값은 수신되는 신호를 충
분히 복조할 수 없다고 판단이 되는 신호강도의 point라고 할 수 있다．


        MP

 Active Set과 비교하는 기준값이며, 이 값은 단말기가 해당 Pilot을 HI呱'I에 포함
시켜 줄 것을 재요구할 때 혹은 확인할 때 쓰이는 값이라 할 수 있다．


 T TDR아）

 TDROP이하로 떨어질 때 동작하는 timer로 P11毗이 약화되어서 T-DR아）이하
로 떨어졌을 때 이렇게 떨어진 값이 어느 정도 신뢰할 수 있는지를 확인하기 위한
시간 기준치이다．
 혹자는 이런 질문을 할지 모르겠다. TADD가 Pilot Set을 상향 조정하는 기준치
이고 T_DROP이 하향 조정치라면 ThADD와 TDROP이 같은 값이 아니겠는가
말이다. 그렇다. 우리가 공부하고 있는 CDMA시스템에서의 Han面甘는 Pilot Set의
급격한 변화를 줄이기 위하여 일종의 hysteresis 형태로 TADD와 TDR아）사이
의 여유 값을 두어서 상태유지를 상태변환보다 우선으로 하고 있다．
    296                                                             6. Handoff
                                                                                 U


                         （표 &2) Hand（그if Drop Timer 만기종료 값

 I TDR아J           기mer 만기종료 값（초）                T-T［가2（가J   Timer 만기종료 값（초）
    0                        0.1                      8            27
    I                        1                        9            39
    2                        2                        10           55
    3                        4                        11           79
    4                        6                        12           112
    5                        9                        13           159
    6                        13                       14           225
    7                        19                       15           319



 이러한 목적으로 사용되는 것이 두 가지인데 하나는 신호의 세기 M可g血이고 또
다른 하나는 시간 M可gin이다. 신호의 세기 마진은 앞 단락에서 이야기한대로
TADD와 TDROP의 값이 같지 않고 어느 정도 여유를 두는 것을 말하며, 시간
（마진은 T_TDROP이다．) 이러한 내용을 정리하면 （그림 &4）와 같다．


        Pilot Strength


                  기지국 A                                        가지국 B




                                                                 시간 여유
                    신호세기 여유

        TADD

        ThDROP


                 기지국 C

                                                                    Time
                                   사 了FO,,{ 환 산된 신호
                                   시I.기 이유부



              （그림 6-4) Hando卄의 신호서끼 및 시간 여유 Hysteres洽 형태


 즉 빗금 친 부 분으 Hando珏가 일어나는 영역인데 여기에는 시간 여유분이 같이
포함되어 있으며, 신호 세기 여유분이 시간으로 환산되어서 보여지고 있다．
    6. Handoff                                              297
U

 이러한 Thresh아d는 System Parameter/Extended Handoff I玉rection 八4essage
등어］ 포함되어서 단말기에 전달퇸다．



         M야川e Assi없ant Soft Handoff (MASHO)

 이동통신 시스템에서 Hando卄는 또 다른 의미에서는 망이 단말기를 관리하고 있
다고 생각될 수 있으며, 또한 단말이 망어］ 자신의 존재를 알린다고도 볼 수 있다．
이런 측면에서 통화중, 즉 망이 단말기의 모든 부분을 관리하고 감시하는 상황에서
의 Han面if는 단말기의 지원이 당연히 필요할 것이다．


     6.2.1 Pilot Set의 천이

 단말기는 Hando珏를 위하여 Pilot Set을 체계적으로 관리하고 있다는 이야기는
앞서서 이야기한 적이 있다. 이러한 관리는 단말기의 독단적인 처리가 아니라 충실
히 망과의 교감이 있은 후에 이루어진다. 즉 단말기가 체감하고 있는 각각의 신호의
강도를 망에 보고하고 거기어］ 따라서 망에서는 Reverse link의 상황을 고려하여
Tra侄妃을 할당할지를 결정하여 단말기에게 통보하게 된다. 이때 단말기에서는
Pilot Set의 갱신이 이루어진다. 단말기는 이러한 절차들을 위해서 판단기준어］ 앞서
서 이야기된 몇 가지의 Thresho닢를 가진다．
 그러면 각각의 Pul毗 Set들은 어떻게 관리되는가 알아보자．




 Traffic과 직접 연관되어 있으며 상당히 강한 신호로 수신되고 있는 /\ctive Set
의 경우 단말기는 최대 6개까지 Pil毗을 가지며 이러한 Act如e Set내의 Pu［야들은
단말기어］ 의해서 항상 감시되고 있어야 한다. 단말기는 처음으로 Forward 통화채
널을 할당받았을 때, Forw可d 통화채널이 열려 있는 Pilot 하나만을 가지도록 초기
화한다（E砒ended/Gener出／ Universal). Handoff Direction 入4essage를 수신하면
서 그 메시지어］ 명시되어 있는 Pil毗들로 이 값은 갱신된다．
 물론 그 전어］ 단말기는 자신이 느끼고 있는（측정한） 신흐의 강도어］ 근거하여 Pilot
strength measurement 八lessage(PS入4N1）를 망어］ 전송할 것이며, 이러한 메시지는
    298                                                   6. Handoff
                                                                       1


기지국을 통하여 Handoff를 관장하는 기지국 제어기어］ 보고가 될 것이다. 기지국
제어기는 수신된 신호강도를 참고하여 채널할당, 즉 Handoff의 시행 여부를 결정한
다. 이러한 결정은 망에서 지시되는 각종 Handoff Direction Message(HDM）에 의
해서 통보되며, 이것을 수신한 단말기는 자신이 가지고 있던 Candidate Set의 일부를
Active로 천이시키게 된다. 시스템에서 /\ctive Set을 제어할 수 있는 것은 유휴 상태
에서는 채널 /\ssignment Message이고 Traffic State에서는 Handoff I万rection
Message이다．
 HDM에는 E砒ende.VGener카／Universal H]呱'1가 있다. 물론 그냥 I끄呱/1도 있다.
이것들의 이름은 초기의 IS弱A에서는 I끄呱/1이었으나 PCS가 나오면서 EHDM을
사용하게 되었으며, IS-95B의 Supplemental Code Channel(SCCH) 할당과 관련퇸
G印呱'I(General Handoff Direction 八4essage）가 나왔으며, IS-95C의 Supplemental
Channel(SCH) 할당과 관련된 UI끄呱4(Universal Handoff Direction Message）이 나
으게 되었다．


 Candidate Set

 현재 신호의 강도는 신호를 복조하기어］ 부족함이 없으나 복조기（finger）가 할당
되지 않은 Candidate     Set은 최대 5개까지 관리할 수 있다. 단말기가 처음으로
Forward 채널을 할당받을 때 아직 Candidate Set이 있을 상황이 아니므로 '0'으로
초기화되어 있을 것이다．
 Candidate Set은 /\ctive Set과는 달리 망의 혀락 없이 단말기가 자체적으로 적
정한 기준인 T소山D를 통과만하면 어떤 상태에서 머물던 Pu毗들도 천이 될 수 있
다. 그러나 망의 허락이 아직은 없O 口로 실질적인 복조를 할 수 있는 경로는 할당
되지가 않는 것이다. 때문에 /\cfive Set에서 Candidate Set으로 천이할 때도 HDM
내어］ 포함되어있지 않으면 Candidate Set으로 떨어진다. 여기에서 T-TDROP시간
동안 회복되지 않으면 이 신호는 다시 Neighbor Set으로 떨어지게 된다. 즉
T-TDROP의 만회할 수 있는 시간적인 여유를 주는 셈이다．
 Candidate Set은 5개의 Pilot PN Set만 처리할 수 있으므로 5개 이상의 Pil毗
PN Set이 있는 경우는 Handoff dr야） timer를 기준으로 가장 오래 동안 여기어］ 머
물러있는 Pil毗을 우선적으로 Candidate         Set에서 버린다. 동일한 Handoff dr아）
timer일 경우는 수신 전계 강도를 기준으로 수신강도가 약한 PN을 버린다．
.
      6. Handoff                                               299
                                                                     I
    扇嬅群裝枷뇨


    Neighbor Set

    Neighbor Set은 유휴state에서 Extended    Neighbor List 八Iessage, Traffic
state에서Neighbor list 皿코ate Message로 전송되는 Pilot PN Set을 우선적으로
설정한다．물론 /\ctive Set이나 Candidate Set은 제외시킨다. 그리고 Extended
Neighbor List Message어］ 새로운 Pilot PN이 있고 특정수량 이상을 초과할 경우
해당 PN어］ 대하여 AGE（오래퇸 정도）를 꼐산하게 되며 NGHGR小/LAXAGE를
초과하면 Neighbor Set에서 버린다. AGE는 Neighbor Set의 변경이 있을 때마다
각 Pilot PN의 counter를 증가시키며 counter값이 많을 경우 오래된 PN(aged PN)
이다．
    Neighbor Set은 일반적으로 최대 20개를 관리하며 20개를 초과하는 경우는 이
Set어］ 가장 오래 머물고 있는 Pu毗 PN Set을 버리고 동일한 조컨이면 전계 강도가
적은 PN을 버린다．


    Remaining Set

    Remaining Set이 되는 경우는 Neighbor Set에서 Set의 크기（PN의 개수）가 커
서 버려진 Set와 AGE가 NGHBRMAX1AGE값보다 클 때 발생퇸다．
    시스템 Parameter 내의 NGFIBR小'lAX_AGE는 Neigh加r Set에서 각각의 Pu毗
PN이 오래된 정도를 나타낸다. 즉 이 Set어］ 호래 있을수록 나이가 들게 퇸다. 따라
서 나이가 많은 Pilot PN은 특정 조건이 되면 Neighbor Set에서 버리게 퇸다．
    P표毗의 변화를 통해서 이 P11毗이 어떻게 상태가 천이 되는지를 생각해보자.
    米 해당 Pilot PN은 Neighbor Set에서 Candidate Set으로 전환하기 위하여 기
       지국어］ Pilot strength measurement Message를 전송한다．(Candidate Set)
    永 기지국은 Han面ff1玉rection 八4essage를 전송한다．(Candidate Set)
     永 해당 Pilot PN은 /\ctive Set으로 천이하고 Handoff completion Message를
       전송한다.(Act如e Set)
     半 전계 강도가 TJIROP이하로 떨어지면 단말기는 Handoff dr아） timer를 동작
       시켜 T1TDROP이 되는지를 검사한다．
                            （如t如e Set)
     米 Handoff 市op timer가 종료되면 해당 P11毗 PN에 대하여 단말기는 Pu毗
        strength measurement Message를 전송한다.(A毗加e Set)
    300                                                          6. Handoff
                                                                              1


                            （표 &3) Pu아 S이의 전위

  Origin     Destination                        Event

                           HDM에 Pu毗이 포함되어 있지 않았으나 TTDROP이 만료되
             Candidate
                           지 않았을 때．
  Active
                           HI呱4어］ P丑毗이 포함되어 있지 않았으나 ThTDROP이 만료되
             Neighbor
                           었을 때1.
                    1
               Active      I끄呱4에 Pilot이 포함되어있는 경우．
 Cand姓ate
             Neighbor      T_TDROP이 만료되었을 때．

               Active      HI呱4에 Pilot이 포함되어 있을 때．

             Candidate     Pil야 강도가 TLADD를 초과할 때
 Neighbor
                           Neighb(玎 Set이 만원인 경우 NGHGRMAX卞AGE를 초과했
             Remaining
                           을 때1.

               Active      HDM에 Pilot이 포함되어 있을 때．

             Candidate     Pilot 강도가 ThADD를 초과할 때1
 Remaining
                           Neighbor 小I/Neigh比r list update 八4essage에 포함되어 있
             Neighbor
                           을 때．



 水 기지국은 단말기어］ Hando什 Direction Message를 전송한다.(Act如e Set)
 半 단말기는 해당 Pu毗 PN을 Active Set에서 Neigh加r Set으로 전환하고
   Handoff completion Message를 전송한다.(Neighbor Set)
 （그림 6-6）는 Pilot Po가 /\.ctive Set으로 변화하는 과정을 나타내고 있으며 그림
과 갇이 T_COMP x 0.5 dB를 기준으로 결정된다. 단말기가 통화 중에 Candidate
Set으로 분류된 Pilot PN P0가 /\ctive Set으로 전위하는 과정으로서 To시점에서
TADD값을 초과하면 단말기는 기지국으로 Pu毗 strength measurement
Message(PSMIVI）를 전송한다. 이러한 PSMM은 Neighbor Set이나 Remaining
Set이 TADD를 초과할 때나 Candidate Set이 /\ctive Set어］ 비해 TCOMP X
0.5dB를 초과할 때 /\ctive Set이 TJJROP이하에서 T_TDROP가 종료되었을 때
어］ 전송퇸다．
    6. Handoff
.


            Pilot Strength




        I     ADD

       T DROP




                                 (1)        (2) (3)             (4)   (51(6) (7)      Time

                      Neighbor         Can出date        如e Set                      Neighbor
                        Set               Set                                        Set

                      （그림 &5) 미아 Set 분류를 위한 미아의 일생（1生）


    또한 단말기내에서 /\ctive Set으로 분류된 P1어］ 비해 ThCOMP x 0.5 dB를 초
과하면 이때도 Pilot strength measurement 八/Iessage를 전송한다. 동일한 원리로
Active Set인 P2를 초과하면 Pilot strength measurement Message를 전송한다．


                Pilot Strength
                                                                             Pilot P0



                                                                  T COMP
                                                       A        x 0.5dB
                                                                               Pilot P.)
                                                      T 'COMP '
                                                      x 0.5dB
                                                      T                        Pih亢 P1

              T ADD




                                          L            乙
                                                                 T2     Time


                             （그림 &6) Active Set에 할당되기 위한 조건


    전체적으로 정리하면 단말기에서 Pu毗 Strength Measurement Message를 전
송하는 시점은 To, T1, T州］ 이루어진다. 그리고 P0는 /\ctive Set인 Pilot Pi어］ 비
古｝1T_COMP x 0.5 시점인 T1에서 Handoff Direction 八4essage를 수신하여
   302                                                            6. Handoff
                                                                               U


Active Set으로 설정된다．


   8.2.2 Soft Handoff 절차

 Traffic state에서 수행되는 I七indo珏는 망에서는 단말기에게 채널할당 혹은 채녈
회수를 해야 하므로 단말기가 느끼고 있는 채널상황어］ 대해서 보고 받아야 한다. 따
라서 단말기는 자신이 관리하고 있는 Pilot Set의 변경사항이 있을 때에는 그러한
정보를 기지국으로 보고한다. 기지국은 이러한 정보를 가지고 Han面卄여부를 결정
하게 된다．
 여기서 생각해볼 것은 단말기가보고하는 RF환경정보라는 것은 Forw町d에 관한
것이다. 그러나 망에서 채널할당이라는 것은 Forwarc/Reverse 양방향어］ 대한 정보
로 이루어져야 하나 그렇지 못하고 있다. 이러한 F-R간의 RF상황은 실제로 전혀
다를 수도 있다는 것을 무시하고 이루어지고있다．
 단말기는 Pu毗 Strength 八Ieasurement 八/Iessage를 통해서 단말기가 현재 가지
고있는 Pilot의 위상과 세기 정보를 망어］ 보고한다．


 Pilot strength2.I Phase와 Phase

 단말기는 Handoff와 Supplemental Channel 할당（S叩p1印ei北al Code Channel
혹은 Supplemental Channel) 할당을 위해서 Pilot 강도와 위상 정보를 망으로 보
고한다． 여기에서 보고하는 값은 잡음 신호에 대한 신호의 비로써 Pilot PN chip
당 수신된 Pil毗 에너지 Ec와 총 수신된 스펙트럼 밀도（잡음과 신호）Jo의 비를 나
타낸다． 이것은 searcher에서 행해지며, 상서伎｝ 사항은 이 책 4장을 참고하라．

                       PN period
                  千日- 32768 chip -
    Base
   Station
    기준                                              i+ l             time
                    Base PN          Pilot Arriva
         놔        뇌- Offset              Time


   Svstem
    기준 1
                         l           i+ l                  time


                      （그림 &7) 미아 Phase계산
      6. Handoff
                                                                    303

     PN 위상은 통화채널과 관련되어 성공적으로 복조하기에 충분한 강도를 가지는
Pu毗의 첫 번째 다중 경로 성분의 도착시간을 사용하여 꼐산된다. 즉 기지국 시간
 인 reference Pilot을 기준으로 위상을 계산하고 결국 시스템 시간 기준어］ Offset을
구해서 Pu야의 위상을 측정한다. 이러한 내용은 （그림 6-7）과 같다．
     예를 들어서 단말기가 알고 있는 기지국 PN Offset = 15360 ch虹刈고 P11毗 도착
시간 = 20480 Chip일 때, 이 기지국의 PN Phase는 다음과 같이 구할 수 있다．
     PN Phase = (20昭0+15360) mod 32768 = 35840 mod 32768 = 3072
     즉 PN Offset은 好이다．

     Pilot Strength Measurement Message

     단말기는 （그림 6-8）과 같은 형태의 PSMM으로 망에 단말기가 느끼고있는 RF
상황을 보고한다．


               12/ 30/ 98 07:34:04.215 !!! 단말기 역방향 통화 채널 메시지 !!！曜
                Pilot Strength Measurement Message

                   Ref_pn : 492
                   pilot_strength : 12
                   Keep : i
                   !!! 1 1 1 variable Message occurrance I!!
                   Pilot_pn_phase : 3849
                   Pilot_strength : 16
                   keep: 1

                     （그림6-8) PiLot Strength Measurement Message


     （그림 6-8）에서 REF_PN은 단말기에서 수신하여 Pu야정보를 이미 알고 있는
Pu毗이다. 여기에서는 492번의 Pilot index를 가지는 PN이다. 또한 PILOT卞PN.
Phase 라는 것은 R吐PN을 기준으로 해서 위상을 측정한 신호로 이 값은 ch珀의
phase 이므로 나누기64를 하여서 실제 PN Offset값을 찾을 수 있다. 즉 메시지의
변동사항을 발생시킨 PN값은 "60" 이다．
     여기에서 P凡OTSTRENGTH와 PILOT_PN_PHASE는 다음의 식으로 산출된
다．
     PILOT_STRENGTH = L- 2 X l0logio(Ec/Jo)j
     PILOT_PN_PHASE = (PILOT_ARRIVAL + (64 X PILOT_PN)) mod 215
 1
       304   1                                                      6. Handoff
                                                                                 U



     여기에서 PThOT사｛RJAVL은 단말기의 Fit培er를 통하여 Combiner(3개의
finger가 합쳐지는 부분, 이것을 이용하여 八4aximum Ratio Combination을 수행）
어］ 처음으로 수신되는 Path의 도착시간이며 PThOTPN은 해당 PN Offset이다．
Mod 2'5는 PN Code가 주기적인 코드이기 때문이다．
     그리고 KEEP은 현재 기지국이 Power Cot出아 대상이 되고 있다는 것으로 통화
채널이 여전히 열려있다는 뜻으로 /\ctive Set어］ 있는 해당 Pilot PN의 Handoff
drop timer가 끝나지 않았음을 나타낸다．
     이러한 PSMIVI은 다음과 같은 조컨에 전송될 수 있다. 나중어］ 이야기되겠지만 새
로운 Handoff 방식에서는 이러한 사항도 조금 변하게 퇸다．
     永 망에서 Power Measurement Request Order를 받을 때．
     永 Neighbor Set이나 Remaining Set이 TAIJD를 초과할 때．
     永 Candidate Set이 Act如e Set어］ TCOMP x 0.5를 초과할 때．
     永 /\ctive Set의 Han面ffdr아） timer가 종료된 경우（Handoff 도중）.
     Extend Handoff Direction Message
     Extend Han面ff1玉rection 八4essage는 기지국에서 전송되며 이것은 단말기가
보고한 PSMM어］ 대한 결과로 내려오는 것이다. 이 메시지를 통해서 단말기는 자신
이 가지고 있는 /\ctive Set의 Pilot들을 갱신한다. 즉 이러한 갱신작업이 Handoff
인 것이다．


                 12/ 30/ 98 07:34:04.516!!! 단말기 순방향 통화 채널 메시 지！!!
                  Extended Handoff Direction Message

                    hdm_seq : l
                    search included : 0
                    hard included : 0
                    addjength : 0
                    Pilot_pn : 492
                    pwr_comb_ind : 0
                    Code chan : 60
                    Pilot_pn : 60
                    pwr_comb_ind : 0
                    Code_chan: 11



                      (그림 6-9) Extended Handoff Direction Message


     （그림 6-9）의 예에서 단말기가 Extended Handoff Direction Message를 수신하
    6. Handoff                                        305
U


게 되면 /\ctive Set어］ Pu毗 PN을 492와 60을 추가하여 양쪽 기지국과 동시에 통화
를 하게 된다. I끄外工SEQ는 Handoff Direction Message의 일련번호이며 순차적
으로 증가한다. 이상과 같은 상황일 때는 단말기는 492와 60와 동시어］ 통화로가 열
려서 메시지와 통화가 이루어지고 있는 상황이다．
 PWR_CO八4BJND는 Power Control Set을 말하며 '1'로 설정되면 같은 Set이고
'0'이면 다른 Set을 말한다. 즉 4장에서 설명된 Combiner에서 결합되는 신호어］ 포함
퇸다는 것이다. 그리고 CODECHAN은 통화채널의 ＼入／aish Code 번호를 의미한다.
 일반적으로 단말기가 첫 번째 기지국과 통화로가 형성되어있고 새로운 두 번째
기지국의 전계 강도가 새롭게 강하게 되어서 2개의 기지국과 동시어］ 통화로를 열어
서 사용한다. 단말기는 Pilot search를 하여 TADD이상의 새로운 Pilot이 등장하
면 이러한 사항을 Pilot strength measurement 八/Iessage를 기지국으로 전송한다．
또한 이 메시지를 망이 단말기에 요구할 수도 있다. 기지국 제어기는 기지국을 통해
서 단말기로부터 PSMM을 수신하면 EHDM(E玭ended Handoff I万rection
Message）를 전송하며 이때 기지국 제어기는 어떤 Pilot어］ 추가로 새로운 Traffic을
할당할지를 결정하여 이 내용을 EHJ呱4어］ 실어서 전송한다
 참고로 Han面if Direction 八4essage는 그것이 사용되는 Common Air Interface
어］ 따라서 이름이 3가지가 더 있다. IS-95이후에 한국형 PCS의 CAl 규격인 J-
STD008에서는 그것의 이름어］ Extended가 붙여졌으며, IS-95B에서는 Supple
mental Code Channel의 할당과 관련퇸 필드가 추가된 형태의 General 印孤4이 있
고, IS弱C에서는 Supplemental Channel의 할당과 관련퇸 필드가 추가된 형태의
un如ersal 印呱4이 있다．


 Handoff Completion Message

 이 메시지는 Han面珏의 최종단계 확인 메시지로서 단말기가 수신한 EF끄孤4내의
Pil毗들을 /\ctive Set어］ 포함시켜서 각각에 Finger demodulat아를 할당함을 나타
낸다. 그전에는 단말기는 자체적으로 판단한 Pil毗을 Candidate Set어］ 포함시켰으
나 /\ctive Set이전 단계이므로 실제 Fii坦er는 할당하지 못한 단계였다. 그러나
EHDM을 통해서        /\ctive Set으로 할당이 가능하게 퇸 것이다．
 이것어］ 대한 응답 혹은 확인으로 단말기는 현재 /\ctive Set어］ 포함되어 있는
Pil毗들을 이 메시지어］ 상술하여서 전송한다.
   306                                                              6. Handoff
                                                                                 U


             12/ 30/ 98 07:34:04.575!!! 단말기 역 방향 통화 채널 메시 지 !!!
         ,    Handoff Completion Message

                last_hdm_seq : l
                Pilot_pn : 492
                Pilot_pn S 60


                     （그림 &10) Handoff Corn이etion Message


 （그림 6-1이는 실제 Handoff Completion Message의 예이며, 이 메시지는 최종
적으로 정의퇸 /\ctive Pu毗 Set을 명시하고 있다．
 이러한 일련의 단말기들은 Han面if를 위해서 별도의 확인체제를 갖추고 있는데
그것은 Han面卄의 일련 번호관리 이다．즉 Hando珏를 지시하는 메시지인 FifiM에서
는 이것이 몇 번째 Han面if지시라는 것을 hdm_seq를 통해서 나타내며, HCM에는
이러한 일련번호어］ 대한 확인작업으로 동일한 일련번호를 사용한다. 즉 last hdm,
seq를 hdm多eq와 동일한 것으로 표시한다．
 물론 이러한 확인이외에 L2쪽의 확인을 위한 확인절차도 미리 이루어질 것이다．


                                                      BTS A BTS B
                      夕단말기
                                   Conversation




                     PSMM : Pilot Strength Measurement
                     EHDM : Extended Handoff Direction Message
                     HCM : Handoff Complete Message

                             （그림 6너 ]) Handoff 처리과정
    6. Handoff                                                     307
.

    이러한 확인절차는 8장을 참고하라 1.
    （그림 6-11)은 전체적인 Han面If의 과정을 보여주고 있다. 즉 Han面ff가 일어날
때에는 단말기는 2개 혹은 그 이상의 기지국들로부터 동일한 통화를 할당 받아서
잠시 통화를 한다. 이로 인해서 기지국에서는 Hando珏를 위한 채널여유 분을 준비
하고 있어야 한다. 물론 이것으로 인해서 단말기는 cell 小versity를 얻을 수 있다．
    이러한 Han面if를 위한 여분의 채널은 실지로 Han面ff가 망의 용량성분과 밀접
한 관계가 있음을 나타내며, 때문에 IS95C의 고속데이터의 경우 Supplemental
Channel의 경우 이러한 Soft Handoff를 수행하지 않고 Hard Handoff를 한
다．Handoif는 단말기에서 제공한 Pu毗정보를 근거로 하여 Handoif가 행해지므로
Mobile Assistant Soft Hando卄m'IASHO）라고한다 이것은 H町d Handoff 방식의
개선안인 MAHHO와 비교될 수 있다．

                 12/ 31/ 99 07:34: 10.817!!! 단말기 역 방향 통화 채 널 ［州시
                 지 !!!
                  Neighbor List Update Message

                    Pilot Inc : 4
                    Nghbr_pn : 164
                    nghbr_pn: 100


                        (그림 6-12) Neighbor list update Message

    단말기는 새로운 기지국으로 새로운 호가 열려지면 그 기지국으로부터 수신한
Neighbor list update 入4essage를 수신하여 이 메시지어］ 포함된 PN을 우선척으로
Neighbor Set어］ 포함시킨다. 호출채넘의 Extended Neighbor List Message 기
능을 가지고 있으며 차이점은 Neighbor list update 入Iessage에는 NGHBR1
CONFIG가 없는 것이다. 이것의 형태는 （그림 6-12）와 같다．
    IS-95에서 Handoif를 위해서 제공되는 이웃기지국의 정보를 나타내는 메시지는
통화상태어］ 제공되는 Neighbor List Update Message와 대기상태어］ 제공되는
Extended Neighbor List 入4essage가 있다. 이러한 메시지의 근본취지는 갇으나 이
것들의 기능은 조금 다르다고 할 수 있다. 그것은 이것들이 관련된 Hando卄의 차이
때문이다．
    통화상태의 경우 단말기는 앞으로 Han面ff의 대상이 될 수 있는 기지국의 상세
정보를 가지고 있을 필요가 없다 왜냐하면 Hando侄를 위해서는 항상 망에서 거기
   308                                             6. Handoff
                                                                U


어］ 대한 정보를 제공받기 때문이다. 때문어］ 단지 단말기는 자신이 수신하고 있는 신
호가 인접기지국인지만을 확인하는 작업만이 필요할 것이다．
 반면 대기상태어］ 이루어지는 유휴 Han面珏의 경우 단말기는 모든 것을 자신이
알아서 Handoff 해야 하는 상황이다. 즉 망에서는 단말기가 Hando侄를 하는지, 혹
은 하지 않는지어］ 대해서는 관심을 가질 수도 없고 가지지도 않는다. 이러한 이유로
대기상태어］ 제공되는 인접기지국의 정보는 더욱 상세한 정보가 제공된다. 이러한
사항은 다음절인 유휴 Han面卄에서 자세히 공부하자．
 이러한 이유로 Neighbor List Update Message와 Extended Neighbor List
Message의 구성의 차이가 있는 것이다. 참고로 메시지 이름 앞어］ Extended가 붙
은 것은 초기의 규격사항에서 새롭게 나온 메시지라는 의미의 이름이고 이와 같은
맥락에서 General 이라는 말이 IS斗95B의 메시지들어］ 또 추가되어진다. 물론 각각
의 메시지들마다 기능상의 차이는 있을 것이다．



 6.3 New Soft Handoff

  6.3.1 Why New algorithm?

 IS -95B이전의 Handoff방식은 단말기가 수신퇸 신호에서 원래 신호를 복조할 수
있을지 혹은 없을지어］ 대한 판단은 T-ADD/TJJROP들과 같은 절대적인 기준어］
의해서 이루어졌다. 그러나 이러한 방법들은 모든 신호가 T-ADD/T_DROP를 초
과하면 Han面珏가 일어날 수 있는 가능성이 있으므로 통화품질을 위한 Han面珏가
아니라 Handoff를 위한 Handoff가 일어날 수 있다．
 지금 현재 /\ctive Set내에는 아주 양호한 Pil毗이 수신되어서 그것을 통하여 신
호를 복조하고 있다. 이때는 추가로 새로운 Pilot 신호에 수신기를 할당할 필요가
없다고 생각이 되지만 새로운 Pu야이 TJ\DD만 초과하면 Han面If될 수 있으므로
단말기와 망은 필요 없는 절차를 수행해야 한다. 또한 /\ctive Set의 Pilot들이 난립
할 가능성도 있다．
 현재 신호가 불량하지 않을 경우를 생각하1 보자. 현재 /\ctive Set내어］ 충븐히 복
조 가능한 Pilot 이 있는데도 불구하고 어느 정도의 세기만 되면 모두 /\.ctive에 포
함될 수 있으므로 실제 통화를 위해서 설정한 /\ctive Set이 아니라 /\ctive Set을
     6. Handoff
 U                                                                                            309


위한 /\ctive Set 이 되어 버릴 수 있다. 이것은 비슷한 예로서 요즘 난이도가 떨어
지는 수능시험으로 인해서 누구나 고 득점이라 할 수 있는 300점을 넘는 경우와 비
슷한 경우라 할 수 있다．


                                                                ..1
                                                                      Pilot 1의 Handoff drop
                                                                      timer가 만료되고 단말
        rPilOt
                 2가   T_
                           .Add룰


                                                                      기는 PSMM올 전송함．
       浮파앴고     냔냘n亡
       ！그것을 Candidate
       !set으로 이농시김．                                                         恁말기는 Pilot 1을
                                                                            入日ghbor set 으로
                                                                             drop하락는 El土UM
                                                                            ！을 수신함.
                           T_Add

                                                                                  rT_Dr。p이하
                           TDr야）                                                   로    떨어진
                                                                                   후 Pilot 1의
                                   Pilot                                 Pu毗 1     Handoff
                                                                                   drop timer
      !1가lot 2가 T_Dyn. Add를 초                                                      가 만료．
      ：과했고 단말기는 PSMM을
      ：전송함．
                                                            n謐毋崙花計 ' ""
                 ：단말기는 Pilot 2를 /\ctive set에
                 !add하라는 EHDM을 수신함．

                                                       m1    기존의 Handoff

                                                       1m    새로운 Algorithm Handoff

                                           （그림 &13) Hand아f 절차 비교


 반대로 신호가 불량할 경우를 생각하1 보자. 신호가 불량할 경우 기존 방식은 모튼
신호가 절대적인 기준치어］ 못 미치므로 현재 /\ctive Set의 신호는 갱신되튼 그렇지
않든 약한 신호를 가지고 통화를 할 것이다. 새로운 시gorithm에서는 어찌되었튼
그 상태에서 가장 양호한 신호가 A曲ye Set어］ 포함되어 통화를 할 것이다. 물론 이
때는 기존의 Algorithm에서 사용하는 Pu毗이나 새로운 Algorithm어］ 의한 Pilot이
동일한 Pil毗일 가능성이 많을 것이다．
 이러한 이유로 새로운 Algorithm은 현재 /\ctive Set어］ 포함되어 있는 Pilot 신호
들의 세기와 비교하는 상대평가어］ 의해서 Dr아） 및 Add시키는 방법이라 할 수 있
다. 즉 새롭게 /\ctive Set어］ 포함되기 위해서는 기존의 /\ctive Set의 Pu'毗의 셰기
보다 더 커야 만이 그 Pui毗이 새롭게 Act如e Set에 포함될 수 있는 이유가 된다는
논리이다．
 이러한 개선된 Handoff Algorithm은 （그림 6-13）과 같은 형태로 나타나게 된다．
    3伯                                                              6. Handoff
                                                                                 .


   6.3.2 Dynamic Threshold

 이상과 같이 T뇨esho넌가 가변적인, 즉 Dynamic한 Threshold가 필요할 것이다．
이러한 Threshold는 현재 Act如e Set에서 서비스하고 있는 Pilot 세기와 연관되어
있어야 할 것이다. 즉 Threshold와 /\.ctive Set의 Pilot 세기는 일정한 함수관계를
유지되어야 할 것이다. IS-95B에서 이야기하고 있는 Dynamic Thresh아d는 이 둘
의 관계가 선형적인 1차 함수관계로 정의하고 있다. （그림 6-14）는 그러한 상태를
보여 준다．
 （그림 6-14）에서 보았듯이 T_DynADD는 Pilot 세기와 1차적인 비례상수를 갖
는 1차 함수의 관계를 가지며, 일정한 intercept값을 가질 것이다. 즉
 T_Dyn_ADD = max{S (Active Set Pi1ot의 Ec/h의 합) + IA, T_ADD}

            Pilot E0/I0
                           새 Algorithm은 C] 지역에서
                           PSMM을 전송하지 않음                T_Dyn_ADD




                                                         T_ADD

                                                           'p.
                                         Active Set total Ec/lo

                          （그림 6나4) New Algorithm

 여기에서 S는 soft 없ope라 하고 IA는 ADI工INTERCEPT라고 한다. S는 "0" 이
될 수 있으며, 이 값은 /\ctive Set의 모든 Pu毗의 且：/k의 합의 값에 얼마만큼의 가
중치를 둘 것인가를 결정하는 값이다. 이와 마찬가지로 T끄yn_ADD에 의해서 다
음과 같이 정의할 수 있다．
 T_Dyn_DROP=S（특정한 Pilot 보다 강한 /\ctive Set P丑毗의 且끄0의 합） + ID
 이러한 Parameter들도 일반 Handoff Parameter와 같이 System Parameter
入4essage및 Ex扼nded,/General Handoff Direction 八4essage어］ 포함되어 단말기어］
거］ 전해진다．

           Dynamic Threshold의 T_Dyn_Drop의 정의는9

           T_Dyn_Drop=S(total 且：/Jo of pilots stronger than pilot i in
 .
      6. Handoff
                                                                     311
                                                                           I
                   Active Set)+ID
                   ID = Drop_Intercept ; S = Soft_Slope (can be 0)
                   T_Dyn_Drop과 비례상수 Soft_Slope S를 만족하는 pilot strength
                   의 의미는 /\rtive set니：1어］ T_Dyn_Dropi될 처지의 pilot보다 약한
                   Pilot이 없다는 의미의 값이다. 마찬가지로, TDyn_ADD의 경우에
                   도 /\ctive set 내에 현재 adding되기 위한 특정한 Candidate
                                                         set
                   pil야보다 강한 Pu야이 없다는 의미로 생각할 수 있다. 이것은 Add
                   혹은 drop을 위한 방식이 절대평가에서 상대평가로 바뀌었다는 이야
                   기도 된다．

                   Dyn_th에서 듸ope가 '0' 이라면 IA만 남게 퇸다. 또한 읾ope= O 이라
                   면 TADD만에 의해 Han面侄가 이루어지는 IS弱A의 방식인데 그
                   렇다면 TADD= IA인가9

                   T_Dyn_Add = S(total Ec/lo of Active Set)+IA
                   IA = Add_Intercept ; S = Soft_Slope (can be 0)
                   TI方n_Add의 정의식에서 S가 '0'이라는 말은 Dyn_th에서 /\ctive
                   set내의 power어］ 대해서는 무관심하겠다는 이야기가 된다. 또한
                   Dyn_th의 개념이 없는 기존의 Soft Han面珏에서는 어떠한 변수（혹
                   은 변량）와도 연관성이 없는 정적인 변수（?), 즉 상수인 TADD에
                   의해서 이루어졌다. 여기에서 중요한 것은 TDyn_Add 가 적용되는
                   시점이 TADD를 넘어선 상황이므로 TA1JD보다 작은 Pil毗
                   strength에서는 의미가 없다. 즉 IA 는 T_Dyn_Add의 초기값 혹은
                   offset값으로서의 의미 이외에는 없다. Adding을 위한 Threshold를
                   정리하면 Thresh아d > TADD이라는 단서가 첨가되어야 한다．
                   T_Dyn_Add=S(total Ec/lo of Active Set)+IA (T뇨eshold >
                   TJ\DD)

      6.3.3 Pilot Set의 쳔이

     새로운 시gori出m은, 즉 단말기가 관리하는 각각의 pilot set간의 천이가 이루어
지는 triggering point의 변화라고 이야기할 수 있다. 따라서 자1로운 Algorithm의
적용은 곧 Pilot Set천이의 변화를 가져온다고 할 수 있다. 이러한 변화를 기존의
   312                                                                                                                   6. Nandoff
                                                                                                                                      a

IS-95A의 형태에서 비교해서 설명할 수 있다．
 （그림 6-15）는 IS-95A의 Set 관리를 나타내고 （그림 6-16）은 새로운 Algorithm
이 적용된 IS-95B의 Set관리이다．


                                               E       >Tj;   I
                                                       (
                                                ,/I。
                                               PSMM 전송

                                                                                                             丑HDM 수신）P.
            1  r小h,               ‘， 」"   m나

                                                                                                              Tdrop 만료
               ＞임의의
          ' EJI。                                                   Candidate Set
         뇨스ctive pilot + ·，,
         LT_ Comp
                                                                                          EHDM 수신, 'I느
                                                                                          Tdrop 미 만료
                                               EHDM 수신




                   _i T_Tdrop"동안
                  '.-. EJIo<T_Drop ,
                      ＼뇨H

                            느41
                                                                  PSMM 전송



                                                       （그림 6-15) IS-95A의 Set 관리

 즉 Neighbor Set어］서 Candidate Set으로 천이되는 과정어］ PSMM 전송이 없어
지고 /\.ctive set으로 천이 되기 위해서 일정한 TAdd가 아니라 채널환경을 반영
한 T_dyn코dd가 사용되고, TjJr야） 대신 T_dyn_drop의 값이 사용된다．


                                                                   Neighbor Se


                AE者，」「．
                ｛卜，  中TAdd
                O.5T加Comp 邑
                                                                                    T_Tdrop가 又
                                                                                   民／Io<T_Drop인


         ,'「 ElI0>旨半'd小 ",\                                                                                  HDM수신
                                                                                                             (to Drop)
                                                                  Candidate Set
                                                                                          표DM수신
                                               PSMM 전송                                    r+nn.   ....'
                                                                                          \ U1J 1J1 17iJ !
                                                                                                             PS


                                                HDM 4= 신
                                                (to Drop}


                                                                        ,U
                                                                             \\'



                                                                       『EdIo<T_dyn_drop
                                                                      「「 이며
                                                                     「， T_Pdrop가 만료되 ,
                                                                         었을 때



                                                       （그림 &16) IS-95B의 Set 관리
    6. Handoff                                                                                                                                                 313
U

     6.3.4 Fast Rising Pilot

 새로운 Algorithm을 이해하기 위해서 다음과 같은 상태를 가정해 보자. 즉
 1) Active Set에는 1개의 Pilot이 존재한다．
 2) FRP(I구ast Rising Pilot）은 n dB/sec의 속도로 Pilot 강도가 증가한다．
 3) 꾸는 Pilot각각어］ 할당된 I刃＼ver의 %이며, Pil毗 강도의 합은 汐］ 된다．

           y1 = nt + b/                                                                                                                                         (6-1)

                               느                                                                                                                                (6- 2)
          1010 + 1010 = 17
             ！旦
 여기에서 刃는 n dB/sec로 증가하는 FRP의 Pilot 세기의 변화성분이며， y七
Active Pil毗의 강도이다. 앞서서 정의했듯이 m을 SOFTSLOOP, 蜘를 /WD
INTERCEPT라고 할 때 dynamic Threshold Dyn_th는 다음과 같다．.

          Dynjh =                        my
                                                       ,   + bd =           mlol。
                                                                                                  g{
                                                                                                         ij
                                                                                                                  -
                                                                                                                          10' "   }
                                                                                                                                      +bd
                                                                                        (
                                                                                                                                                                (6-3)
                                                                                            "t+
                                     =
                                     =
                                               mlol。
                                               ml0l.
                                                              g{
                                                              g{       fl 10
                                                                       qH
                                                                          l0        -
                                                                                                       b1)
                                                                                                        "     /       }
                                                                                                                          +b4
                                                           l0Yi/ }
                                                           10                                                                                                   (6- 4)
           y, =l0l0g{
                  =lol。
                                g{            ii-
                                              n1
                                                                   "
                           EC/ I0                                                                                                     Fast Rising Pilot : yf


                                                       Active
                                                       Pilot : Ya

                                                       Dvnth


                          T ADD




                                                           （그림 &17) Fast 딕團ng Pu아의 효과


              t, 寸 그吻i t肛T 肋D]
                                     n

                                              iL. .                         f. .b』4/                              小（m寸bf)"/"\"'1 - . 小］
                                                                                                                             I -i. ....AJJDI                    (6- 5)
                                     =-1U1og11U ' " 1 11-lu
                                              'ft
  314                                           6. Handoff
                                                              .

 우리는 여기에서 앞의 식들을 가지고 여러 가지로 고찰해 보고 이러한 식을 통해
서 우리가 또 다른 편의 생각을 유도하 보자. 혹은 너무나 당연한 이야기들을 앞의
식들이 하고 있는지도 모르겠다．


  只：
   :1                                                 斗   1

  나1 식 佇3）에서 알 수 있듯이 /\ctive Pu毗과 Dynami二下h肥sh아d는 서로
    비례한다． 또한 식 (6-1)에서 보듯이 Fast Rising Pu毗但RP）과1Act如e
   Pu毗은 서로 반비례한다． 따라서 FRP의 세기가 증가할 畔Act押e Pilot과
   Dynamic Threshold는 감소한다는 것을 확인할 수 있다. 측아주빠르게 성
    장하고 있는 P표毗이 있을 때에는 어떠한 상황이든 간에, 예를 들아서 아주
    빠르게 셀간을 이동하는 경우 상태척으로 기존의 Pu毗의 새기는 약해지는
    것이고 아울러서 Dynamic Threshold도 동반해서 약해진다는것이다.




          식 (6-5）어］서 알 수 있듯이 스／는 FRP의 기울기에 반바례한다. 추가적으
   로함수 Dyn_th(n）에서 n의 증가에 의한 것보다스／는 빠르거r감소한다r
   1그\13D를 통과한 후 Dyn_th까지 증가하는 시간이 짧아진다는 것은FRP의
    기울기가 급격하다는 말이고 그림에서 나타난 것과 같이 스t가r감소했．을 때
   Dyn_th=cont.일 때와 가변일 때의 기울기는 가변일 때가U훨씬 크다. 즉
   Dyn_th이 n의 함수이며, 여기어］ 아주 강한 감소성분이 있다는 이야기가 된
    다．
         Ech1o                  Ech1。




                                T Al끄）




                 （그림 &18) Dynth, n, 스／의 상관관겨1
    6. Handoff                                               315
.                                                        ]



      整？J
         FRP과 Dyna而c Threshold가 만나는 지점은 특정 FRP의 Dyn_th를 의
        미한다. 이러한 겅우에 Dyn_th가 일정하다고 할 때 FRP의 기울기 n과 스／
         와는 식 (6助와 같은 함수콴계가 있．다. 즉 n과 스t와는 서로 반비례하게 된
        다. 또한 n 이 일정하다고 할 따 Dyn_th와 八t와도 역人］ 식 (6旬와 같은
         관계가 있으며, 이것들은 서로 비례하는 관계가 있다．
           여기에서 이야기하는 Dyn叫出가 일정할 때, n이 일정할 때라는 가정은 우
         리가 처음 생각했던 가정인 하나의 FRP와 하나의 /\ct如e Pilot 존재라는 문
         제와 배치되는 가정들이다. 즉 D恥th가 일정할 때 n이 변화될 수 있는 경
         우는 /\ctive set내에 여근 개의 Pu毗이 존재한다는 이야기가 된다.



      e= 1 1

           瓦汀0가      7.1dB보과 작은 Pilot으］ Act如e set어］ 단일 Pu毗의 경우어］,
         Dyna帥c Thresh아d는 언제나 T了山D보다 작으며, 같은 시간에 2가지의
         경우, 즉 개선 전괴 개선 후의 Algorithm을 사용하는 단말기들은 add된다
         (SOFT小SLOE下＝2.25, ADD_INTERCEPT=3으로 가정）.



    고철5!
        만약          스t가 Searcher의 탐색주기보다 작다면, 그때 FRP은 2개의
         Algoi就hm은 동일한 효과를 낼 것이다. 즉 식 (6-5）의 첫 번짜 식에서 스t
          七0이라면 Dyn_th 七T卄ADD의 결과가 나올 것이다．



      a브j
               (t2 十 ti）이 탐색주기보다 크고 가장 강한 Pu야의 Ec/J0가 다음읔 만족할
         만큼 긴 Act如e set에 N개의 Pilot이 있다면 2개의 단말기 모두 동일하게 동
         작할 것이다．




               EC , T_ ADD- ADD_ INTERCEPT
                                             l0log(N)         (6- 6)
               I)       SOFT SLOPE
                                                             6. Handoff
    316                                                                   .

                     寸；

                          7

                     쿄3
           Active
           Set       山9
           Pilot으］        la
           최 태1
                          11
           Ec/ 10
           (dB}      中l 2

                          3
                                                        叫小
                           4
                               7           3             4
                                       N. Active Set의 크기


                （그림 &19) A에ye S아의 가장 강한 아아의 Echo




  6.4 Hard Handoff

   6.4.1 Hard Handoff 절차

 H針（ii Han面仕는 기지국과 단말기간어］ Handoff가 일어날 상황에서 기존의 통화
로를 끊은 후 새로운 통화채널로 재 접속하는 방식으로 call drop이 발생하기 쉽다．
이러한 방식을 "break and make"라 한다. 이러한 것은 Traffic이 열려 있지 않은
상태에서 이루어지는 Han面珏인 Idle/Access Handoff들은 이런 의미에서 모두
H可d Hando표를 수행한다고 할 수 있다. 그러나 대기상태에 있을 때 Hando珏는 상
대적으로 간단히 처리된다. 새로운 서비스 지역어］ 진입했을 경우 호출채널의
CDMA Channel List Message를 이용하여 해결할 수 있고 등록조건이 되었을 경우
해당하는 등록（주로 Parameter change registration이나 zone based registration)
을 수행하면 된다．
 반면 후어］ 이야기되겠지만 /\ecess 상태에 이루어지는 /\ccess Hando什와
Traffic 상태에서의 Han面卄에서는 이러한 처리보다는 좀더 복잡하게 이루어지고
있다. H計（IHan面ff가 일어나게 되는 가장 근본적인 원인은 resou丁ce를 관리하는
관점에서 해석되어야 한다. CDMA시스템에서 Vocoder frame을 관리하는 기지국
제어기의 CCP에서 Handoff를 관장하는 것도 어떤 의미에서는 상대적으로 안정적
인 soft Han面仕를 실현하기 위해서이다. 따라서 현재 CDMA시스템에서 어쩔 수
없이 Hard Han面ff가 일어나야 될 상황이라고 한다면, 별도의 H八V혹은 S/W를
    6. Handoff                                        317
U


가져야 하는 주파수간과 RC간어］ 이루어지는 Hando珏는 불가피하게 h可d Handoff
이것이다．
 이러한 Hard Hando珏는 새로운 채널을 할당받기 위해서는 기존의 채널을 관리
하고있는 관리자에게 우선 반납하고 새로운 채널을 할당받아야 하므로 call dr야戶］
발생할 확률이 증가하계 된다. 따라서 이를 효과적으로 처리하는 것이 통화품질어］
영향을 미친다고 할 수 있으며, 이러한 것을 개선한 새로운 H町d Handoff 방식이
MAHHO와 같이 제안되고 있다．


     6.4.2 Hard Handoff의 유형

 일반적으로 Hard Hando卄는 주파수간, Frame 옵셋간 등과 같이 2개의 망 자원
관리자가 동시어］ 공유할 수 없는 경우어］ 발생하게 되는데, 이러한 H可d Hando卄는
상대적으로 Soft Handoff어］ 비해서 성공률이 떨어지므로 가능하면 Soft Han面ff로
프로세스를 수정하는 작업을 많이 한다. 이러한 작업은 주파수나 RC 등과 갇이 기
지국의 형상정보와 직결되는 문제와 연관된 경우는 원천적으로 불가능하며, 이러한
형상정보가 바뀌게 된다면 문제는 해결될 수 있을 것이다. 이를테면 2FA인 기지국
이 인접 기지국과 Soft Handoff를 위해서 FA를 증설한다든가 RC3이상이 지원되
지 않는 기지국(IS-95A小 기지국）이 IS-95C기지국으로 叩grade가 된다든지 하면
문제는 해결될 수 있을 것이다．
 또한 형태의 경우 Han面侄의 주체를 망의 계위상 상위 계위에서 수행하게 하면
가능한 것이 있다. 즉 기존의 CCINTJ에서 수행하던 일을 포함하고 관리하는 또 다
른 프로세서를, 즉 망의 계위상 상위 계위어］ 속하는 MC狐m혹은 그 이상의
TMCINTJ 등과 갇은 처리과정을 추가하면 가능하게 된다. 이러한 처리가 이루어질
때 이동단말기는 초기어］ 호가 설정된 자원을 어느 장소에서나 유지하게 된다．
 이러한 직접적인 경우는 단말기가 초기어］ 설정한 지역에서의 Vocoder frame
offset과 이동지역의 frame Offset이 다를 경우이다. Vocoder frame Offset은 전송
선로의 다중화를 위해서 시분할하여 사용하는데 모든 단말기는 system time을 기
준으로 加i-Is 단위로 전송하므로 각 탄말기간 1.25ms 단위로 전송시점을 다르게 하
여 전송한다. 이러한 Vocoder frame offset은 CCII日U에서 관리함으로 인해서 그것
의 상위단 간의 Handoff 일 경우 H可dHan面侄가 발생하나 그러한 자원（Vocoder
frame offset ) 관리를 상위에서 하1 준다면 다시 말하면 상위의 프로세스를 정의하1
   318                                                   6. Handoff
                                                                      .


주면 이러한 H可d Handoif의 가능성은 없어질 것이다．
 예를 들어서 서울에서 호를 설정한 후 고속도로를 이용해서 부산까지 이동했다면
부산까지 가지고간 호는 서울에서 설정한 Vocoder frame offset이 그대로 부산어］
서도 사용하고 있을 것이다. 즉 서울의 특정한 Svc가 부산에서 이루어지는 호를
위해서 사용되고 있다는 것이다．


   6.4.3 주파수간의 Hard Handoff

 주파수간의 Hando珏는 기본적으로 Soft Han面卄가 이루어질 수가 없다. 왜냐하
면 주파수간의 Soft Hando卄를 위해서는 단말기는 동시어］ 2개의 주파수로 신호를
복조해야 하기 때문이다. 그러기 위해서는 단말기는 여러 개의 주파수 대역필터와
이에 따른 복조기를 가지고 있어야 하기 때문이다. 이러한 Hard Handoif는 셀룰러
에서 망 자원을 구분할 때 주파수를 사용해서 하는 FDMA방식의 이동통신에서는
H町（I Han面ff가 불가피하게 퇸다. 이러한 측면에서 모튼 주파수 자원을 공유하면
서 사용하는 CI呱hA는 Soft Han面if라는 선물을 한 것이라 생각할 수 있다


                                       B셀에서 F2 로   통화畺
                                       하다가 』A에서 꾼 j乙 으
                                       로 每화8衣갸 하늄 상황

                            1FA   /     2FA




         A셀에서 l乙 로   통호卜爵
         하다가 B셸에서는 1乙으
         望 퉁화해야 하는 상황



                 （그림 &20) 서로 다른 FA간 Hando卄의 0카


 （그림 6-20）은 서로 다른 FA간 Handoif를 나타내고 있으며 단말기가 통화상태
이면 Handoff Direction 入4essage를 사용하여 처리하게 된다. （그림 &20）의 A에
서 B로 이동하는 경우 Hard Handoif어］ 큰 문제점은 발생하지 않는다. 왜냐하면 1
FA지역에서 서비스 받고 있는 FA(Frequency Assignment）를 2 Fl\ 지역에서도
     U
         6. Handoff                                             319

연속적으로 사용하면 되기 때문이다. A 지역인 1FA 지역에서 B지역으로 이동할
때 B기지국의 전계 강도는 차츰 강해지기 시작하므로 특정조컨이 되면 단말기는
PSMM을 전송하게 된다. 기지국은 이 정보를 이용하여 Handoif 명령을 내리게 된
다. 여기에는 변경될 H可dHan面仕의 정보들을 같이 제공해 줄 것이다．
     그러나 2FA 지역에서 iF) \ 지역으로 이동할 때 서비스받고 있는 FA가 이동지
역어］ 없을 경우 calldr야戶］ 발생한다. 즉 이러한 시점어］ Handc湃가 필요한 것이다.
이러한 Hando什를 수행하는 데에는 현재까지는 미국의 伽alcomm사에서 제안한
Dummy Pu야방식（일명 Beacon방식이라고도 함）과 Round Trip Delay 방식이 있
다．
             냥식
     이 방식은 기지국과 단말기간 주고받는 신호의 지연량（Round Trip Delay）에 따
라 Han面if의 시점을 결정하여 주는 방식으로 허용 지연량은 각 기지국 환경어］ 맞
추어 최적화시어］ 확인하여 기지국의 Parameter로 설정하1 주어야 한다．


                        RTI)어｝ 의헤서 추정된 벨이며 ,
                      ! 실제 Ilandoff기； 꿸 반켱보다
                      4 작욤．




                                （그림 6-21) Round Trip Delay 방식


     이러한 방법은 Soft웨어로 실현되므로 추가적인 장비가 필요하지 않다는 장점이
있으나 셀 영역이 불규칙적인 곡선일 때 필요 없는 지역에서 Han面珏가 될 수 있는
가능성이 있으며, 실지로 （그림 &21）과 같이 Han面卄경계가 실제 셀의 영역어］ 비
해서 작을 가능성이 많다．

     Dummy Pilot(일명 Pilot Beacon) 방식
     （그림 6-22）와 같이 2FA지역에서 통화하다가 1FA지역으로 이동할 때 자신이
사용하던 주파수 채널이 없으면 문제가 발생된다. 이러한 문제를 해결하기 위하여
1FA 지역어］ 2FA지역에 비해서 빠져 있는 Pi［야을 dunin寸로 출력하는 방식이 있
   320                                                       6. Handoff
         1                                                                U


다. 이러한 Pilot beacon 기지국은 실제로 통화채널이 없는 overhead 채널만 전송
하여 단말기의 searcher에서 Pilot PN search를 도와주는 역할을 수행한다. 단말기
의 searcher는 하나의 FA만 search하므로 다른 FA 정보는 검색할 수 없다. 따라서
2FA 지역에서 1FA지역으로 이동할 때 경계지역에서 2FA를 전송하여 단말기가
PSMM을 전송하도록 유도한다．




                                         기지국내에서
                                         1갸lot Change 수헹 .




                    （그림 &22) Dummy 마아 방식



 시스템에서는 단말기의 PSMM 정보를 이용하여 FA를 할당하여 2FA 지역에서
1 FA 지역으로 원활한 Han面卄가 수행되도록 한다. 물론 이러한 방법은 별도의 기
지국 h可dw可e가 필요하므로 비용이 소요된다는 단점을 가질 수 있으나, 앞서 이야
기된 RTD방식과 비교했을 때 Han面卄경계가 분명하다는 장점도 더불어 가지고 있
다. 또 한가지의 장점은 이방식으로 할 경우 기지국간에는 나중어］ 기지국 내부에서
Serving Frequency로 천이 할 것이지만, 어떠한 모양이든 간어］ Soft Hando珏를 한
다는 것이다．




                                H中놔 실제 셀 경계
                                111RID셀 경계1
                                1HHDummy Pilot셀 경겨］

                （그림 &23) Dummy P11아 과 Handoff 경겨1

   6.4.4 RC간 Hard Handoff

 IS-95C에서는 그것이 제공하는 서비스 형상의 발전으로 인해서（예를 들면 고속
패킷 데이터） 새롭게 Radio Configuration 등을 정의하였다. 이러한 RC는 전반적
    6. Handoff                                                      321
1

인 RTT의 변화를 가져오며, 이러한 RC간의 통화로의 교환 등의 절차, 즉 Handoif
도 별도의 Hard웨어를 2개 이상 가지지 않는다면 주파수 Han面if와 동일한 이유로
어쩔 수 없이 Hard Hando珏를 수행할 수밖어］ 없다. 즉 그것의 시나리오는 주파수
Hando卄와 비슷하다．


                                                 B셀에서 RC3으로 통화룔
                                                 하다가 A에서는 Rd l 으로
                                                 통화하따 하는 상황

             95B 기지국                                      95C 기지국

                  A




                            l을     入 三   入   R   과 RC3를


                 A셀어卜서 RC1 으로 봉
                 화를 하다가 王｝ 셸에 나
                 는 Rd l 으로도 통화li
                 가눙한 상황．


                             （그림 &24) 日C간 Handoff


    （그림 6-24）와 같이 RC간 Han面珏가 발생될 수 있는 상황에서는 Handoif 지시
를 할 때 그것의 내용을 역시 단말기에게 알려 주어야 한다. 이러한 RC간의
Handoif를 지원하기 위해서 망은 Universal Han（如if Direction Message를 사용
하며, 여기에서는 새롭게 사용될 통화에 대한 정보, 즉 서비스 형상정보를 내려보내
줄 것이다．

     6.4.5 Hard Han由什의 메시지 쳐리

    Hard Hando卄를 위하여 단말기는 이동하기 위해 전지역에서 사용하던 Parameter
를 계속 사용하는 여부를 Han面ff1玉rection Message로 수신하게 되는데 이것이
PRJVATE_LCM(private Long Code mask), RESET_L2(reset acknowled-
gement pr乂edure）이다. PRIVATELCM은 음성 암호화를 위하여 mask 상태를
변경하는데 사용되고 RESET_L2는 ACI( 치리와 관련된 Par帥ieter를 그대로 유지
하는 여부가 전송된다. 이외에도 전력제어와 관련퇸 Parameter들의 변경 여부도 포함
되어 전송된다．
   322                                                                                                         6. Handoff
                                                                                                                            U

다음은 실제 필드에서 이루어진 주파수간 H可dHan面卄의 예이다．

 12/30/98 07:35:43.070．단말기 艮TCH 入lessage
   Pilot Strength Measurement Message
          msg_type : 5     ack_seq : 4                                                             단말기가 기준으로 잡고있는
                                                                                                   즉 가장 오래 동안 잡고있는
          msg_seq : 3     ack_req : 1       ..                 ' "                                 Pilot이 60이다．
        encryption : 0 . , . ,畔召4.:, 69." "
     Pilot_strength : 25        keep : 1
   !!! [ 2].veriaMe. essage occurrance !!!
     Pflot_pn_phase 노 27906
     氏如t_ strength酉亡小玉碗少卜小小，,                                                                        Handoff 타이머가 만료
                                                                     나   1
                                                                             小   ，나   니
                                                                                          n小   中




     Pil;:f:p뵤：phb:se : 31478                                                                        되지 않은 Pilot들의 위
     Pilot_strength : 18                                                                             상과 강도를 보고．
                              keep : 1

 12/30/ 98 07:35:43.851- 단말기 艮TCH Message                                                      현재 진행되고 있는 Handoff
                                                                                               의 일련번호로 단말기가 수신
  Extended handoff Direction Message/--" "
                                                                                               한 Handoff 관련 메시지들의
      Msg_type : 17       a吐stl丁3                                                              짝을 맞추기 위한 것이다．
      msg_seq : 5 /       ack_req : 1
      encrvDtion : 0      use time : 0                                                         탐색 파라메터가 바뀌게 될 때
                                                                                               이 필드 이하를 규정하여 사용
      action_ume : U nam_seqj.2戶                                                               한다．
      search included小．丁' "
      srch_win_a : 7 -> 40(PN chips)                                                           Hard Handoff 관련 항목들이
                                                                                               포함되었다. 즉 Hard Handoff
      t_add : 26        t_drop : 30 . . . //, ' " '                                            룔 지시할 때 사용한다．
      t_comp : 5         t_tdtop亡茗；> 2(seconds)
      hard, included ,: r ' '
                                                                                                   Long Code mask의 변경，L2의
      franqJOffget 'l4.
                            ..                                                                     확인절차 변경夕 전력제어정보
     而毗已1cm: 0 re諦軍；0‘尸小“                                                                          변경） 이로 인해서 새로운 동
                                                                                                   기를 잡기위한 preamble정보
     뇨邑etSf.少1已．.. . ,r·S   1
                                 , ,, ,
                                1S


     encrypi_Im入l毛기기＝> nncrypuon aisaoiea
                                                                                                   둥이 발생될 때 표시되는 영역


      nom_pwr_ext : 0 nom_pwr : 0
                                                                                               이 경우 한국형 PCS의 475주
      nom_pr照艸1e_: 0
                                                                                               파수 채널의 492번 Pilot으로
      b乞ieCclass : 4 =>- '1iQREAN PCS                        --「                               Handoff하며！ 코드 채널 62번
     的ma_freq : 475             S1,   ,
                                          ,,,   1   '   "'

                                                                                               Frame Offset 10으로 통화를
                                                                                               계속하게 될 것이다．
     뇨dd_length : 0
      +                          S
      l노iot_pn
          . _ : 492    pw1._tomb_ind : 0
      Codegfr彷l뇨 i 6g111



RC간 Hando卄는 동일한 조건이나 Handoff 지시가 UH[小T으로 이루어진다．
    6. Handoff
.
                                                                                                                323

           12/ 30/ 98 07:35:4吼090- -단말기 艮TCH
             Handoff Completion Message
                     Msg_type : 10
                     Ack_seq : 5
                                                                                         hdm_seq가 2인 EHDM에 !
                     Msg_seq : 4                                                         대한 웅답 이며 , 최종적으
                     Ack_req : 1                                                         로 492번의 Pilot으로
                                                                                         Handoff 학．
                     Encryption : 0
                     k畔！Mffi?"s毛自' 弘？,

                    텍斗pn,:, 492 , ...'
        1/16/02 06:55:33.466 - MS 순방향 통화 채널 메시지
         Universal Handoff Direction Message
                 msg_type : 34 ack_ seq : 0 msg_seq : 4
                 ack_req : 1 encryption : 0
                 use time : 1           action time : 19
                 hdm_seq : 1
                 params_inci : 1
                 1匕rev : 5
                 serv_neg_type : 1
                 srch inc : 1
                 srch_win_a : 7         srchwin_n : 9
                 srch win r : 10        t add : 26
                 t_drop : 30            t_comp : 5
                 t_tdrop : 2            soft_slope : 0
                 add_intercept : 0                drop_intercept : 0                  이 필드 이하에는 순y역방향 다중
                 extra_parms : 1                                                  .   화 옵션！ 서0 스 옵션등의 서비스
                                                                                小口／
                                                                                      형상 정보（setvice configuration)
                 packet_zone_id : 0                                  //
                                                                          . "         등이 기록됨 . 서비스 형상 정보는
                 band_class :4          cdma_freq :450 ,/                             8장어弘寸 공부하게 된다．
                                                                //



                 return_if_ho_fail : 0                    . "
                 periodic_srch : 0                   "'
                 scr_included : 1            ./
                 serv_con_seq : 1 ,/
                 record_len : 15 . /,"
                                  / "
                                                                                              전력제어 관련 형상， 등
                 record       tvoe ;，中 -> service confi므uration
                  1 1 二 1 1 Cl rY1! 1                  V                                      과같은 비협상 서비스
                                                                                              형상 정보들로 이 필드
                                                                                              를 三설정한다．
                 nnscr included: 1
                 record_len : 2
                 rec斗Ph包；哄 ,:. 恥,>'fi叩斗熙otiable service configuration




    이상과 같이 RC간의 Han面珏에서는 새로운 서비스 형상과 비협상 형상 등과 같
이 호를 구성하는 속성들의 협상 절차가 필요하며, 그것이 Handoff 지시 메시지에
      324                                       6. Hancioff
                                                              1


포함될 수도 있고 8장에서 설명될 별도로 Service 협상（Negotiation) 절차어］ 의해
서 결정될 수도 있다．
     추가적으로 U印呱'I에는 Han面if의 Parameter들과 데이터호의 도먼트와 관련
있고 데이터 서비스의 영역을 표시하1 주는 packet_zone_id 등의 변경에 대한 정보
도 함께 제공되어 이러한 망 요인들도 Handoif 할 수 있음을 나타낸다. 만약 주파
수간의 Han面侄라면 새로 천이할 주파수에 대한 정보를 제공해 주며, MAHHO기
능의 return고HhoHfail의 기능과 아울러서 탐색의 모드 등과 같은 정보로 MAHHO
의 형상어］ 대한 정보도 제공한다．
     결과적으로 UBIJM을 위시하여 모든 Handoff 지시 메세지들은 이렇게 교환할
망 정보를 전송하고 Handoif를 지시하는 역할을 한다.



         MAHHO: Mobile Assistant Hard Handoff

     八끄나표Io는 IS-95B이상의 Hard Handoff 형태로서 기존의 H可dHan面if와는
Han面ff 성공 율을 향상시키기 위해서 크게 2가지의 기능을 개선 혹은 추가하였다．
그것은 Handoif 할 대상이 되는 무선주파수 채널로 단순히 그것의 상황이 어떤지
를 확인 방문해 보는 Se可ch기능과 Hando卄를 시도했다가 실패했을 때 원래 사용
하던 주파수로 돌아올 수 있는 기능인 Handoff 실파1 복귀 기능이다．
     참고로 여기에서 사용될 주파수들은 기지국에서 단말기에게 Handoif 하도록 지
시하는 목표 주파수인 TF(Target Frequer（功와 현재 서비스되고 있는 주파수를
나타내는 SF(Serving Frequency), 그리고 기지국이 주파수간 Handoif를 위해서
단말기에게 탐색을 지시하는 주파수인 CF(Candidate Frequency）가 있다．


      6.5.1 Failure and Return

     또 한가지의 특징은 Failure and Return의 기능이다. 이것은 Han＆町를 실패시
다시 톨아올 수 있는 방식으로 Han＆湃의 실패에 대한 불안함을 감소시켜 줄 수 있
다．
     Fail네te and Return기능을 위해서는 우선 Han面付가 실패되었는지 성공되었는
지어］ 대한 판탄기준이 선행되어야 할 것이다. 따라서 Handoif 실패를 선언하는 판
1
    6. Handoff                                         25
                                                            1
정기준은 target frequency의 전체 수신전력의 임계치와 새로운 /\ctive set의 pu毗
月c/b의 임계치로 Hand沮가 실패되었는지를 판정한다. 또한 Candidate Frequ

ency로 첫 번째로 양호한 Frame을 수신할 때까지의 최대시간 등을 통해서도 판단
한다. 또한 이러한 판단기준이 어느 정도의 시간 이후에 발생될 수 있듯이 이러한
것을 위해서 기지국은 H可（I Handoff 성공 후에도 original frequency어］ 할당되었
던 resources를 주어진 시간 동안 keep한다．
    CFSRec小I는 return on fail싸re 기능 동작을 관리하는 Thresholds를 포함하며，
이러한 메시지를 단말기로 전송한다. 또한 기지국은 GI끄呱4 등을 통해서 RETUIL캅나
IF나拓ndoff_FAIL==1로 설정하여 단말기로 전송한다. 이러한 정보를 수신한 단말
기는 return on failure 기능을 수행할 수 있게 퇸다. 단말기는 다음과 같은 절차를
수행한다．
    水 단말기는 현재 사용하고 있는 Serving Frequency관련 Parameter를 저장해 둔
     다．
    木 단말기는 SF의 사용뜯｝ 불연속적으로 동작한다. 이러한 동작은 Target
     Fre恥ency와 병행해서 동작하기 때문이다．
    永 TF로 완전히 변경하여, 즉 I缸d Hando且를 완전히 수행하여 동작한다. 이때
     단말기는 계속 TF의 입력전력을 측정한다．
    串 단말기는 측정한 결과인 "SF의 input power - TF input power" 를 임계치 비
     교하여 임계치보다 크다면, 이번어］ 수행한 Hard Handoff는 failure로" 보고퇸
     다．
    木 또한 단말기는 TF Active set 각각의 I꾜ot들의 丑c/b를 측정한다．

    米 TF Active set Pilot들의 EC加 의 합이 특정한 임계치보다 작다면 이것 역시
     H町d Handoff는 failure로 보고된다．
    木 마지막으로 단말기는 TF에서 양호한 frame을 기다리는 최대시간의 타이머가
     만료되면 H可d Handoff는 failure로 보고된다．
    이상과 같이 단말기는 RF단의 단순한 신호의 세기로 Handoff의 성공 여부를 판
단하고， 기저대역 복조기에서 신호대 잡음비인 万c/b로 판단하고 마지막으로 frame
의 성능으로 Han面珏의 성공여부를 확인한다. 이러한 판단기준으로 판단하여서
Han面侄가 실패라고 판단될 때 단말기는 다음과 같은 추가적인 절차를 수행한다．
   326                                                     6. Handoff
                                                                        .


 永 단말기가 GUI孤4의             COMPLETE_SEARCH가 '1'이라면, 또한 T可get
  Frequency와 Candidate Frequency가 같은 경우 CF Search Set의 Pu毗들
  어］ 대한 탐색은 끝낸다．
 水 그리고 다시 Serving Frequency(SF）로 돌아와서 이것을 통하여 통화를 계속
  유지한다．


 來 SF Parameter를 다시 저장한다．

 水 SF상에서 이루어지던 모든 것들을 그만둔다．
 水 단말기는 이러한 정보들을 담은 Candidate Frequency Search Report
  Message(CFSRptM）를 기지국으로 전송한다．


  6.5.2 Search기능

 Searching기능은 MASHO와 비슷하게 단말기에서 제공해 주는 무선상황을 고려
하여 Handoff를 수행하게 하는 것이다. 단말기는 이러한 이웃 주파수의 채널정보를
수집하기 위해서 탐색을 위한 t可get frequency로 순간적으로 천이하여 해당 주파
수를 탐색하여 그 값을 망어］ 보고한다. 이러한 탐색기능으로 인해서 망은 좀 더 확
실한 정보를 가지고 Hando卄를 수행할 수 있으며, 이것은 좀더 신중한 Hando珏를
하게 하는 방법이다. 손자병법어］ 知彼知己면 百戰百勝이라는 말이 있듯이 이러한
방법은 Han面ff할 대상이 되는 주파수의 상황을 알고 주파수 Hand咐를 하겠다는
방식으로 기존의 방식보다는 좀더 합리적인 방법이라 하겠다．
 이러한 탐색은 주기적으로 탐색이 행해지는 주기탐색（Periodic Search）과 상황
어］ 따라서 이루어지는 단일탐색（Single Search）으로 이루어진다. 이러한 탐색은


              CFSReq          Report EHDM



              II ; 十 I t
         F2


         F1            .



              CFSReq                         Report EHDM
         F2


         F1

                           （그림 &25) 다른 주파수의 방문
     6. Handoff
 1                                                        327


Candidate Frequency Search Reques勺／Contr이 八4essage를 통해서 이루어진다．
 （그림 6-25）는 다른 주파수를 탐색하는 것을 보여준다. 이러한 탐색을 위해서 후
보 주파수 채널로 이동하는 것을 방문（Visit) 이라고 이야기한다．
     기지국은 단말기에게 이러한 탐색을 지시하기 위해서 Candidate              Frequency
Request/Contr이 Message 등을 이용한다. 이러한 메시지들을 통해서 명령을 받은
단말기는 이러한 명령을 거절할 상황인지를 확인하고 필요하다면 거절할 수도 있
다. 또한 정상적으로 명령을 수행할 수 있다면 수행 후 결과를 Candidate
Frequency Response Message로 응답한디．. 또한 기지국에서는 이러한 방문의 형
태와 수 등을 규정할 수도 있다．
 기지국은 CF Neighbor set information을 CFSReqM을 통해서 CF Neighbor
set, CF Neighbor set Window, CF Remaining set Window, CF pilot PN
increment의 값들을 단말기어］ 전송하여 준다．

         e Search
 CFSCtr1M혹은 CFSReqM의 SEARCHTY}下의 값이 '1'로 설정되어 있을 때
단말기는 Single Search를 수행한다. 이러한 Single Search를 위해 단말기는 각각
의 visit에서 단말기는 다음과 갇은 과정을 수행한다 :
 永 우선 현재 서비스받고 있는 SF의 Parameter를 저장해 둔다．
 半 이러한 Visit를 수행할 때 단말기는 CF를 방문하기 위해서 SF상에서 불연속적
     인 동작을 하게 된다．
 米 단말기는 모든 복조 시스템을 CF로 튜닝한다.
 永 CF와 SF상의 입력 power의 차가 단말기가 CDMA CF상의 Pu毗을 측정하기
     위해서 설정해 놓은 임계값인 DWFRXHPWRTHRESH보다 작으면 현재
     叭5仇는 cancel한다.
 水 위의 조건이 만족되면 단말기는 해당 CF search set의 Pil毗들의 subset의 구
     성 P표毗의 EC/IO를 측정하여 통화를 위하여 요구되는 EC/JO인지를 확인한다．
 半 단말기는 다시 자신이 원래 사용중이며, 현재 Serving Frequency로 사용중인
     주파수로 돌아온다.
 米 여기에서 지금까지 저장하1 두었던 SF Parameter로 모튼 장치를 새롭게 설정
     하고 SF상의 동작을 다시 시작한다．
   328                                          6. Handoff
                                                             口


 이상과 같이 단말기는 단일 탐색을 수행하며, 이러한 CF se可ch set의 모튼 P如t
들을 측정하는 동안 다음 叭sit를 예정한다. 또한 단말기는 필요하다면, Single
Search 과정을 반복하며, 입력 power와 CF의 Pil毗 세기 측정치를 CI고SR印M를
통해서 가지국어］ 보고한다. 이러한 내용은 기지국으로 보고한다．

 Periodic Search

 단말기의 주기탐색은 단일탐색과 더불어서 MAHHO의 탐색기능의 중요한 한 부
분이다. 이러한 주기탐색이 발생하는 경우는 단일탐색보다는 좀더 다양한 경우어］
발생퇸다. 물론 단일탐색과 마찬가지로 CFSReqM 혹은 CFSCtrl八4의 탐색 형태를
지정하는 필드인 SEARCHTYPE가 '11'로 설정되어 있는 경우에 수행이 된다. 이
것은 Return on Failure기능이 있는지, 혹은 없는지어］ 따라서 수행된다．
 米 Return on Failure 기능이 없는 상태에서 Hard Hando侄가 성공되어 있는 경
  우 PERIODIC SEARCH 가 '1'로 enable되어 있고 현재 단말기가 Peri以Jic
   Search을 하고 있지 않고 있으면서 TF와 CF와 다를 때에도 단말기는 주기탐
   색을 한다．
 米 Return on Fai뇨re기능이 있는 상태에서 H可（IHan面ff가 성공 후, PERIODIC_
   SEARCH가 '1'이고, TF가 CF와 다르다면 주기 탐색을 한다. 또한 Hard
   Han面ff가 실패한 후에도 PERIODIC_SEARCH가 '1'이면 주기 탐색을 한다．
 단말기는 CFSReqM어］ 기술된 Search Period의 Periodic T油er의 설정과
T油er Enable에 의해서 Periodic Search를 수행한다. T油er가 만료되기 전어］ 단
말기는 우선 Frame마다, SF입력 r刃wer와 Threshold값의 비교치어］ 근거하여
timer를 disa川e 혹은 reset시킨다. 그리고 Single Search와 동일한 방법을 사용하
여 CF Se可ch Set상의 모든 P11야의 강도를 측정한다. 이것이 끝나고 나면 현재
search 주기상의 CF1TADD이상으로 측정한 모튼 Pu毗틀의 万c/b합이 入4ll
TOTALJ凡OT_EC_IO보다 작다면, 기지국으로 CFSRptM를 전송한다．
 이러한 주기탐색은 단말기가 H可d Handoff를 위하써 EHI呱4 혹은 GI]DM/
U1{1孤4을 수신했을 때는 더 이상 Hancli渡를 준비하는 탐색을 할 필요가 없 O 口로
단말기는 SF Periodic Search를 중지한다. 또한 수신한 CFSReqM 혹은 CFSCtr小4
의 SEARCHmMODE가 '0000'이고 SEARCH TYPE이 '00'이라면 더 이상 탐색이
필요 없다는 정보를 수신하였으므로 탐색을 정지한다. 여기에서 단말기가 CF
    6. Handoff                                            329
1

Periodic Search를 중지하기 위해서는 유지하고 있던 어떠한 CF visit도 cancel하
며, 그것어］ 대한 정보는 CFSR就M를 통해서 망으로 보고하지 않는다. 또 한 가지의
방법은 Periodic timer를 disable하는 것이다．


     6.5.3 MAHHO를 위히1 새로 지원되는 메시지들

    IS-95B이상 또는 므REV이 4이상일 경우 이 절에서 설명하는 MAI표1O의 기능
을 제공하기 위해서 Layer 3의 새로운 메시지들이 제공퇸다. 이러한 메시지들은 실
지로 하위계층의 기 능들 을 제어한다．


      (1) Candidate Frequency Request Message

    이 메시지는 MAHHO기능을 위해서 새롭게 제공된 메시지로 탐색에 관련된 전
반적인 자료를 단말기로 제공해 주는 역할을 한다. 이 메시지에는 모튼 Candidate
Frequency로 출력되고 있는 P如t들의 PN offsetsj斗 Search 砥／indow Size를 포함
하는 목 록 을 가지고 있으며, 탐색할 Pil毗의 subset을 나타내고, 불필요한 탐색과 보
고를 방지하기 위해서 임계치를 상술하고 있다. 또한 주기탐색의 탐색주기를 상술
하고 있다．
    다음은 세부적인 필드들의 기능틀이다．
    · CFSRM_SE（그 : Candid貳e 다equency Search Request Message 일련번호
    · SEARCH_TYPE : 탐색 명령


                         （표 &4) SEA딕CH TYPE Codes

    SEARCH TYPE                                 의미
         00         임의의 탐색이 진행되고 있는 중어］ 정지를 위해서 단말기어i 지시
         01         단말기에게 Single Sea丁ch를 지시
         11         단말기에게 Periodic Search를 지시



    SEA日C나PER1OD: CF상의 연속적인 탐색간의 시간
    330                                                  6. Handoff
                                                                      .


                           （표 &5) 탐색주기 값

  SEARCH PB귀（그Ds      탐색주기（초）       SEARCH PERIODs   탐색주기（초）
          0              0.48             8               30
          1              0.96             9               40
          2               2              10               風）
          3              2.96            11               60
          4               4              12               80
          5              4.96            13              100
          6               10             14              150
          7               20             15              200



 SEA日OH MODE : 탐색모드


                      （표 6-6) SEA日OHMODE Ty口es

   SEA只CH MODE                            설명
          0000       Candidate Frequency로 출력되는 CI呱iIAP如t들을 탐색하라．
          0001       Analog 채녈들을 탐색하라．



 이 값을 수신한 단말기는 자신의 SF의 Act如e Set Pu毗들의 EC의 전체 값이
total_ec_thresh 보다 클 경우에는 CF의 탐색을 할 필요가 없다고 생각하고 탐색하
지 않는다．
  · SF TOTAL EC그（二THRESH : SF의 전쳬 P11아의        万c/b임계치
 이 필드도 CF를 탐색할 때 사용되며, 이 필드의 값이 "111111" 일 때는 사용되지
않는 값이라는 표시이다. 구체적인 값은 다음과 같이 결정되며 단말기어］ 전달퇸다．
 匕20xlogl0(total_ ec_ it乙t力res九）]

 이 값을 수신한 단말기는 자신의 SF의 Active Set Pil毗들의 EC의 전체 값이
total ec t뇨esh 보다 클 경우에는 CF의 탐색을 할 필요가 없다고 생각하고 탐색하
지 않는다．
 · ［긔FE 日X_PWR_THRESH : 수신된 전력의 최소 차이값
         6. Handoff                                             331
     1


         만약 단말기가 CF로 출력되는 수신된 전력과 무관한 CD入4A CF상의 Pilot을 탐
색한다면, 기지국은 이 필드를 '00000'으로 한다. 그렇지 않다면 다음과 같이 설정한
다．
         [(mi面urn_pow叱耐f+ 30)/21

         (cand_freq_pwr - serving_freq_pwr）가 minimum_p이ver_diff보다 작다면 탐
색하지 않는다． cand_freq_pwr는 수신된 CDMA CF의 전력이고, serving_freq_
pwr는 수신퇸 CDMA SF의 전력이다. 이러한 값들은 dBn/1.23 八4T七로 표시된다．
         · MIN_TOTAL_PILOT_EC_IO : 전체 P卄아들의 且c/J。의 최소값
         Active Set의 Pilot의 강도를 무시하고 Forw카（I 통화채널을 복조하려고 단말기
가 시도한다면, 기지국은 이 필드를 '00000'으로 한다. 그렇지 않다면 기지국은 다음
과 같이 값을 설정한다．
     匕20기og加tal_ p加1加帥毗]

         이 값을 수신한 단말기는 자신의 SF의 /\ctive Set Pil毗들의 EC의 전체 값이
的t可ect뇨esh 보다 클 경우에는 CF의 탐색을 할 필요가 없다고 생각하고 탐색하
지 않는다. 단말기의 /\ctive set내의 모든 Pu毗의 합이 加talp如t_thresh보다 크다
면, Forward 통화채널을 복조하기 위한 시도를 하지 않을 것이다．
         · CF_T_ADD : CDMA Candid計e 다equency의 P11아검출 임계치
         단말기는 이 값을 참고하여 CDMA CF의 주기적 탐색동안 Candidate
Frequency Search Report 入4essage 의 전송을 결정한다. 기지국은 이 값을 부호
가 없는 값으로 다음과 같이 표시해준다．
         [_2xloxlog1。E /I,]

         · TF_WAIT_TIME : CDMA TF상의 최대 대기 시Z}
         기지국은 이 필드를 단말기가 CI呱4ATF상에서 N11mX20m sec 동안 충분한
신호의 질의 Frame이 수신되는지 기다리는 시간인 Wait time의 최대값으로 설정
한다．
         · CF小미LOT그NC: Hando卄이후 CDMA CF상에서 출력하는 P11아 PN sequence
offset index increment.
         · 아_SRCH小w八Jd :Can配ate 다equency Search S이의 탐색 윈도우 크기
         이 값은 앞서 설명한 （표 6-i）과 같이 사용된다. 개념 또한 동일하다. 단말기는
   332                                              6. Hancioff
                                                                  U


구체적으로 Pilot 각각어］ 대해서 Search Window이 주어지지 않았을 때 이 값을
Default로 사용한다．
  · CF_SRCH叫V피NR : CDMA CF의 Remaining S아의 Search Window 크기
 Han面侄가 성공적으로 끝난 후 CDMA CF상의 Remaining Set의 Pu毗의 탐색
하기 위해서 할당됨．
  · 아_NGHBR_S日CH MODE : CF Search S아의 탐색모드


                      (표 6-7) CFNGHBRSRCHMODE

    값（2진수）                                    설닫1
         00         탐색 우선순위가 없거나 Search Window의 설명이 없음
         01         탐색 우선순위 설명
         10         Search Window 설명
         11         탐색 우선순위와 Search Window의 설명



  · A나GN_TI卜川NG : Align Timing 지시자
 SEAR아HI_OFFSET 필드를 사용할지 여부를 나타내는 필드임．
 1 SEARCH OFFSET : Search O什set
 단말기가 탐색을 시작하는 시점을 명시하기 위해서 사용하는 필드로 기지국은 이
필드를 통해서 단말기에게 탐색 시점을 지정해 준다．


 Search_offset_tin始은 CFSReqM 혹은 CFSCtrlM의 action tin祀으로부터 처음
탐색을 시작하는 초 단위의 시간 옵셋을 나타낸다．

    (2) Candidate Frequency Control Message

 이 메시지는 단일탐색과 주기적인 단일탐색을 초기화하고, 진행중인 임의의 주기
적 탐색을 종료하게 한다. 이 메시지는 앞에서 설명한 CFSReq入l 내어］ 포함퇸
SEARCH TYI下 필드를 제공한다．

    (3) General Handoff Direction Message

 H町d Handoff 실패의 발생에서 보고와 복구를 제어한다. 이 메시지의 또 다른
    6. Handoff                                          333
1


중요한 기능은 IS-95B의 入'DR을 위한 Supplemental Code Channel 할당어］ 사용
된다．

      (4) Candidate Frequency Search Response Message

    기지국에서 요구한 CF탐색을 수행한 결과를 전송하는 메시지로 이러한 메시지는
기지국이 Handoff 지시를 할 때 사용되는 정보가 되며, 이것으로 인해서 M아血e
／뇨前St라는 개념이 나오는 것이다. 즉 MASHO에서 PSMM의 기능과 갇은 역할을
한다．
    CF를 방문하여 탐색을 수행하고 Serving Frequency로 다시 돌아오는 전체시간
(total off time）과 CF로 방문하여 탐색의 일부를 수행하고 다시 SF로 돌아오는 시
간중 최대시간（ma血num o卄-time）을 추정하여 그 값을 전송한다．
    메시지의 상세 내용은 다음과 같다.
    · 녀ST_CFSF朴兀SEQ - CFSReqM의 일련번호
    단말기는 이 메시지가 응답할 CFSReq八4의 CFSRM_SEQ 필드값과 같이 하여
탐색의 일련번호를 관리한다．
    · TOTAL나OF尸TIME_FWD : 단말기가 Forw可（l 통화채널을 아f하는 전체시간
    단말기는 CF로 천이하고 요구된 탐색을 수행하고, 다시 SF로 돌아오는 처리를
하기 위해서 그것의 현재 Forw町d 통화채널 처리를 유지하는 것이 필요할 것인 전
력제어 그룹 혹은 Frame의 전체수의 단말 추정치를 이 필드어］ 설정한다. 만약 단말
기가 요구된 탐색을 마치기 위하써 CF를 여러 번 방문하는 것이 요구된다면, 단말
기는 이 필드를 탐색주기중어］ 모튼 CF를 방문하기 위한 Frame의 전체수（PCG놔
OFFTIIVIE 이 '0'으로 설정되어 있다면） 혹은 전력제어 그룹（PCG1OFF中TIME
이 '1'로 설정되어 있다면）으로 설정한다．
    · MA乂OFF尸기M日日ND : 단말기가 Forward 통화채널을 떠난 총시간
    단말기는 이 필드를 CF로 천이하고, 요구된 탐색의 부분을 수행하고, 다시 SF로
돌아오는 처리를 하는 동안에 Forward 통화채널을 유지하기 위하써 필요한 Frame
의 최대치（PCG1OFFHTIIVIE 이 '0'로 설정되어있다면） 혹은 전력제어 그룹（PCG_
OFF1TIME 이 '1'로 설정되어 있다면）의 단말 추정치로 설정한다．
    · TOTAL_OFF_TIME_REV : 단말기가 Reverse 통화채널을 떠나는 전체시간
    단말기는 CF로 천이하고, 요구된 탐색을 수행하고 다시 SF로 돌아오는 처리를
     334                                                   6. Handoff
                                                                        1


하기 위해서 그것의 현재 Reverse 통화채널 처리를 유지하는 것이 필요한 것인 전
력제어 그룹 혹은 Frame의 전체수의 단말 추정치를 이 필드어］ 설정한다. 만약 단말
기가 요구된 탐색을 마치기 위해서 CF를 여러 번 방문하는 것이 요구퇸다면, 단말
기는 이 필드를 탐색주기중에 모튼 CF를 방문하기 위한 Frame의 전체수（PCG
OFFTIME 이 '0'으로 설정되어 있다면） 혹은 전력제어 그룹（PCG_OFF_TIME
이 '1'로 설정되어 있다면）으로 설정한다．
  · MAX_OFLTIMEREV : Reverse 통화채널을 떠난 최대시간
  단말기는 이 필드를 CF로 천이하고, 요구퇸 탐색의 부분을 수행하고 다시 SF로
돌아오는 처리를 하는 동안어］ Reverse 통화채널을 유지하기 위해서 필요한 Frame
의 최대치（PCGOFFTIME 이 '0'로 설정되어 있다면） 혹은 전력제어 그룹（PCGH
OFFTIME 이 '1'로 설정되어 있다면）의 단말 추정치로 설정한다．
  · PCG_OFF_TIMES - off times 이 PCG단위로 규정된가를 나타내는 지시자
  · ALIGN_TIMING_USED : Alignment timing used indicator.
 기지국에서 요구된 것과 같이 SF를 떠나는 그것의 방문의 시간할당이 있다면 1
로 설정한다．
  · MAX_NUM_니이TS : 탐색주기당 방문의 최대수
 주기 당 최대 방문 수에서 1을 뺀 수로 이 필드를 설정한다．
  1 八TER스기SIT寸기ME : Inter-visit time
 단말기가 MAXHNUMHVISITS 필드를 포함하고 0이 아닌 다른 값으로 설정되
어 있다면, 단말기는 이 필드를 포함하며, 이 필드의 값을 다음과 같이 설정한다．
 min(63, [inter_visit_time / searth_tin比_resolution 1)

  여기에서 단말기가 PCGOFI亡TIMES을 0으로 설정한다면 search_time_
resolution은 0.02이다. 그렇지 않다면 search立me_resolution은 0.00125이며
inter_vis迂－time는 SF를 떠나는 연속적인 방문을 시작하는 시간간의 초 단위 단말
추정시간이다．


    (5) Candidate Frequency Search Report Message

 이 메시지는 CFSRM와 마찬가지로 SF와 CF의 Rx 전력, Pu야들의 丑c/b을
보고한다. 또한 H可d Hando卄 실패 후 원래 주파수로 다시 돌아가기까지 사용된다．
    6. Handoff                                   3   L;

U


상세 내용은 다음과 같다．
    · LAST小SRCH_MSG : 수행한 탐색의 형태 지시자
    CFSCtr1入4혹은 CFSRM로 지시된 단일 혹은 주기탐색의 결과가 올라간다면, 단
말기는 이 필드를 0으로 설정할 것이다．
    · 나＼ST_SRCH_MSGSEQ : 탐색결과를 위한 일련번호
    만약 이 메시지가 CFSC八l의 응답으로 올라간다면, 단말기는 이 필드를 CFSC의
CFSCM_SEQ 丘eld로 설정한다. 이 메시지가 CFSReq八4의 응답 메시지라면, 이 필
드를 CFSReqM의 CFSRM_SEQ 필드로 설정한다．
    만약 이 메시지가 GI끄呱4/U印孤4의 응답으로 올라간다면, 이 필드를 GHDM/
UFil呱4의 HDM中SEQ필드로 설정한다．
    1 SEARCH MODE : Sea兀h mode
    CSReqM에서 상술된 탐색 Parameter와 부합되는 ＜표 6-旬의 SEARCH_
MODE값으로 이 필드를 설정한다. 즉 이 메시지로 전송되는 정보가 어떠한 탐색모
드어］ 대한 답인지를 나타낸다．
    만약 SEAR아끄MODE가 CDMA 채널을 탐색하라는 모드（0000）이면, 다음과
같은 필드를 추가로 포함한다．
    1 BAND CLASS : Band class
    이 메시지가 Hard Han面if가 성공되지 못했음을 보고할 때에는 이 필드를 TF의
CDMJ＼주파수 FA와 부합되는 Band class로 설정한다. 이 메시지가 CF상의 측정
결과를 보고한다면 CF의 FA가 해당되는 band class를 기록한다．
    · CDMA나FREQ : 주파수 할당（FA)
    위의 Band class어］ 해당되는 주파수 할당번호를 기록한다．
    · SF_TOTAL_RX_PWR : SF상으로 수신되는 전체전력
    단말기는 이 필드를 다음과 같이 설정한다．
    刃洌31,[(l0lo計k加乙rece加ed규刃刊e기日10)12])

    여기에서 的t吐received_power는 SF상에서 단말기에 의하囚 수신된 평균입력
전력으로 mW/1.23 八4Hz. 단위이다．
    · CF TOTAL－小AX PW日 : TF 혹은 CF상에서 수신된 전체 전력 지시자
    시도한 Hard Han面珏가 성공하지 못했다는 것을 보고할 때면 단말기는 TF상어］
서 수신퇸 전체전력은 포함한다. CF의 측정결과를 보고한다면 단말기는 CF의 수신
   336                                                6. Handoff
         U                                                         1


된 전체 전력으로 이 필드를 설정한다．
 단말기는 이 필드를 다음과 같이 설정한다．
 min(31,[(lolog(total - received _ power) +110)/21)

 여기에서 的t吐received_i刃＼ver는 CF혹은 SF상에서 단말기어］ 의해서 수신된 평
균 입력전력으로 mW/1.23 MHz. 단위이다．


 NUM_PIL0T&S : Pilot의 수

 이 필드는 이 메시지가 포함된 Pu毗의 수를 나타내며 이것은 0에서 Neigh加r
set의 최소 크기인 40개까지 가질 수 있다. 이 필드가 포함되어 있을 때에는 이 필
드에서 나타내는 수만큼 Pu毗의 측정된 위상, 그 Pu毗의 강도를 나타내는 필드를
추가하며, 추가적인 Pilot 정보가 필요한 경우（P丘OTHRECHTYI下＝1）에는 Pilot
레코드 형태（PILOT_REC_TYPE), 길이（RECORD_LEN）필드를 추가한다．


   6.5.4 Call Flow

 다음과 같은 3가지로 MAHHO 시나리오의 호의 흐름을 살펴보도록 하자．
 우선 Return On Failure기능이 작동되는 경우어］ I｛町d Handoff가 성공한 경우와
실패인 경우, 그리고 Candidate Frequency Se町ch하는 경우로 나누어서 생각해
보자．


 Handoff 성공 - RIF(Return If Failure）기능

 단말기는 망으로부터 CFSReqM를 수신한다. 이때 단말기는 명시퇸 모드로 CF
의 탐색을 시작한다. 단말기는 망으로부터 RIF=1인 GHDM/UFII呱'I를 수신하여
Hando卄를 지시받는다．
 단말기는 전력제어를 위한 TOTHFRA入1E과 BAI工FRA入4E계산을 계속하고
RS2인 경우 최근 2개의 E田를 저장한다. 그리고 LOST叫FRAME cou毗er를 시작
한다. 이것은 안정적인 채널환경을 점검하기 위한 절차라고 이해할 수 있다．
 SF의 정보들을 저장하고 Handoff Dr야） T油er를 disable시킨다.
 Handoff Timer를 시작하고 八4S는 TF로 주파수를 Tun血g한다. 단말기가
Cl孤IA-Cl呱4AH可d Hando侄를 위해서 수신 정지된 후 재개되어 수신되어야 할
Frame수인 1(Niim）개의 양호한 Fran妃을 수신하였으므로 새로운 주파수 채널로 통
    6. Handoff                                        337
1                                                 1

화로가 정상적으로 열려졌다（Han面珏성공）. Handoff Tim町를 disable시킨다．
    Hando卄를 성공한 단말기는 Handoff Dr야） T如er를 reset하고 enable한다. 또한
저장된 SF Paran）毗er들을 discard하고, CF의 탐색을 중지한다. 그리고 CF
NSET寸TI乙ASET인 NSET로 NSET를 갱신한다．
    단말기는 NUM_PREAMBLES（통화채널 프리앰블 수）개의 Frame을 전송하고，
HCM를 기지국으로 전송한다. 단말기는 2개(p硫）의 연속적인 양호한 Frame을 수
신하고 TOTFRA八4E과 BAD_FRAME계산을 시작한다．


    Handoff실패 - RIF기능

    단말기는 망으로부터 CFSReqM를 수신한다. 이때 단말기는 명시된 모드로 CF
의 탐색을 시작한다. 단말기는 망으로부티 R1F=1인 G印呱4/UI1巫'I를 수신하여
Han面If를 지시받는다．
    단말기는 전력제어를 위한 TOTHFRAME과 BAD_FRA八/IE계산을 꼐속하고RS2
인 경우 최근 2개의 可B를 저장한다. 그리고 LOST_FRAME counter를 시작한다．
이것은 안정적인 채널환경을 점검하기 위한 절차라고 이해할 수 있다．
    SF의 정보들을 저장하고 Han面If Dr야） T如er를 disable시킨다．
    Handoff T如er를 시작하고 八4S는 TF로 주파수를 Tuning한다. 단말기는 양호
한 Frame 수신을 기다린다. 그러나 DWFRX日PWRTHBESH와 TOTALASF江H
P瓦OT_EC_J0_THRESH의 값이 LOW나타났다. 즉 임계치보다 작은 값이 나타났
으므로 단말기에서는 HHO 실패로 한다．
    Handoff T油er가 만료된다.
    단말기는 H可d Hando珏가 실패되었다고 선언한다. TF와 CF가 같고, 탐색이 끝
났으며, H可d Handoff실패이유가 /\ctive Set의 Pilot들의 전체 EC/I0가 임계치보
다 작거나 Handc）卄 伽ner가 만료된 것일 때 단말기는 SRCH_CF_NSET_R을 기다
린다．
    단말기는 SF로 tuning한다. 그리고 SFParameter를 다시 회복시키고, Han面ff
Drop Timer를 enable시킨다．
    단말기는 전력제어를 위한 TOTmFRAJ\I伍과 BAD_FRAME꼐산을 재개하고
RS2인 경우 최근 2개의 Effi를 저장한다. 그리고 LOST_FRA八lE이 12개보다 크다
면 2개의 연속적인 Frame을 기다린다．
       338                                          6. Handoff
                                                                 U


     단말기는 Candidate Frequency Se可ch Report 八4essage를 기지국으로 전송한
다．
     Candidate Frequency Search

     단말기가 CFSCtr1M/CFSReqM을 수신하였다．
     CF탐색 Periodic timer를 시작한다（CF탐색 Periodic timer가 만료되었을 때에는
Handoff Drop T岫er를 小sable시키고 SF정보를 저장한다）.
     단말기는 전력제어를 위한 TOT_FRAME과 BAI工FRAME계산을 계속하고RS2
인 경우 최근 2개의 可B를 저장한다. 그리고 LOST_FRAME counter를 시작한다．
     단말기는 CI啞 주파수를 Tuning한다. 그리고 주파수채널 상태를 측정한다．
     단말기는 SF로 주파수를 Tuning한다．
     SF정보를 회복시키고, Handoff Drop Timer를 enable시킨다. 단말기는 전력제
어를 위한 TOT1FRAME과 BAD_FRAIlVIE계산을 재개하고 RS2인 경우 최근 2개
의 可B를 저장한다. 그리고 LOST_FRAME이 12개보다 크다면 2개의 연속적인
Frame을 기다린다. 2번부터 7번까지가 하나의 visit이며, 단말기는 CF中NSET내의
모튼 P표毗이 측정될 때까지 계속한다. 단말기는 Candidate Frequency Se可ch
Report Message를 기지국으로 전송한다．



         Idle Handoff

     이동통신 시스템에서 이루어지고 있는 Han面if는 Hando卄의 수행에서 망은 자
원을 관리하는 측면에서 주도적으로 행하지만 단말기의 상태를 파악하여 즉 入4obi1e
Assistant로 Han面珏가 이루어진다. 이러한 이야기는 앞서서 이야기되었다. 그러나
단말기의 독자적으로 이루어지는 Han面ff도 필요할 것이다，
     예를 들어서 망에서 개별적으로 관리하지 않는 망 자원, 이를 테면 broadcast하
는 호출채널 자원 등어］ 대해서는 별도의 관리가 없으므로 단말기에서 독자적으로
판단하여 Han面if를 시행한다．
     이러한 방식은 단말기가 대기상태어］ 있을 때 호출채널의 교제시어］ 이루어진다．
     유휴 Handoif는 단말기가 유휴상태 동안 하나의 기지국이 담당하는 영역으로부
터 또 다른 기지국이 담당하는 영역으로 이동할 때 발생되며, 현재 기지국의 Pilot
    6. Handoff                                          339
U


신호보다 강한 다른 호출채널 신호를 감지할 때 발생된다．
 단말기가 대기상태（유휴state）어］ 있을 때 서비스 채널에서 지속적으로 전계 강도
가 강한 Pilot PN을 찾는다. 이러한 과정을 Pilot search라고 하며 그 결과 Active
Set, Neighbs兀 Set, Remaining Set으로 구분하여 관리한다. Active Set은 현재 서
비스받고 있는 호출채널의 Pilot PN이고, Neighbor Set은 Han面珏가 가능한 I꾜毗
PN의 집합으로 Extended Neighbor List Message로 수신된 PN Set이고，
Re曲ining Set은 검색되는 나머지 집합이다.
 단말기가 대기상태에서 관리하는 /\ctive Set은 Tra州c 상태와는 달리 1개이며,
일반적으로 Neighbor Set은 20개 정도로 관리한다. 대기상태에는 경로D如ersity의
필요성이 없으므로 최소한의 /\ctive Set만이 필요할 것이다.
 유휴 Handoff는 단말기가 기지국의 도움 없이 자체적으로 판단하여 수행하게 되
며 이 결과를 등록으로 기지국에 보고한다. 물론 해당되는 등록조건이 없을 경우 등
록을 수행하지 않는다. 또한 유휴 Hando珏를 수행하는 동안 단말기는 non slotted
n均de로 호출채녈 메시지를 수신하여 단말기의 상태가 새로운 기지국으로부터 새로
운 Parameter들을 받아서 갱신하는 처리를 수행하는 데에만 전력（全力）한다．
 유휴 Hando丘를 수행하는 동안 단말기는 non slotted mode로 동작하여 새로운
호출채널의 메시지를 수신한다. 만약 이동한 지역에서 정상적인 메시지를 수신하게
되면 해당되는 slotted mode로 동작한다. 이때 조건은 타당한 Page Channel
Message를 하나 이상 수신하는 경우이다. 단말기가 새로운 기지국 또는 섹티로 이
동했을 경우 이전의 overhead 八Iessage는 모두 무시하고 새로운 overhead
Message로 갱신한다. 이것은 단말기가 이동한 지역의 망 정보가 바뀌었으므로 새
로운 정보로 갱신하는 과정이라고 할 수 있다．
 단말기에서 유휴 Handoff를 수행하는 기준은 단말기 searcher에서 수신되는
Pilot Set의 Neighix兀 Set중에서 임의의 Pilot의 Ec江o7f Active Set의 보다 3dB
클 경우 수행한다. 새로운 Pil毗으로 유휴 Hanth：府를 수행한다．
 기본적으로 유휴 Handoff는 Extended Neighbor List Message의 Pilot Set어］
서 수행되며 이밖의 값이 수신될 경우 단말기는 초기화 과정부터 다시 시작한다．
 유휴Handoff를 단말기가 독자적으로 수행하는 가장 큰 이유는 Forw可d의 RF
상황만을 가지고 결정하나 Reverse 출력이 없으므로 Reverse 링크어］ 대한 보장은
network으로부터 받을 필요가 없기 때문이다．
   340                                                6. Handoff
                                                                   1


  6.6.1 절챠

 유휴 Hando珏는 기본적으로 인접한 기지국으로 Hando珏하기 위해서 이웃한 기
지국의 상황을 알고 있어야 하므로 이러한 정보를 NGHBR_CONFIG를 통해서 알
수 있고 유휴 Hando珏를 수행할 수 있다．
 단말기는 대기상태에서 기지국으로부터 전송되는 많은 기지국 형상정보 중 지금
현재 서비스 받고 있는 기지국의 인접한 기지국의 정보도 수신할 수 있다. 대기상태
어］ 내려오는 이러한 인접 기지국의 정보들은 단말기가 （그림 6-26）과 같이 셀과 셀
간 중첩지역어］ 들어가게 될 때 계속적으로 호출채널을 감시할 수 있는 신호를 결정
하기 위한 절차, 즉 유휴 Hando妊를 하게 될 때어］ 유용하게 사용된다．
 실지로 단말기의 Fii坦er는 대기상태에서는 cell diversity mode로 동작하고 있지
않기 때문어］ 하나의 확실한 Pilot 신호만을 찾게 된다. 결국 H可d Handoff를 하게
되는 것이다．
                                         이 셀로 이동하는 단말기는 주
                                         파수와 호출 채널과 slot올 새 :
                                         롭게 할당 받아서 대기상태를 !
                                         유지해야 한다.           ;




    기지국은 자신이 인접     U                         인접한 기지국
    한 기지국의 형상을                               파수, 호출 채널
    NGHBRCONFIG로                             른 기지국임．
    자신의 출력이 미치는 !
    모든   단말기（영역）에
    뿌려준다．


                    （그림 6-26) 유휴 Hando什의 예


 Extended Neighbor List 八4essage의 NGHBR_CONFIG는 이러한 형태로 이루
어지는 유휴 Handoff를 수행할 수 있는 정보를 제공해 준다. 이러한 정보는 인접
기지국의 FA, 호출채널의 개수 등어］ 대한 정보이고 해당 단말기는 수신하고있는
Pilot 중 세력이 점점 강해지는 Pilot의 이러한 자원과 관련된 형상정보를 참고하여
유휴 Handoff를 수행하는 것이다．
 단말기가 새로운 기지국에서 새로운 주파수 채널 혹은 새로운 호출채널 및 slot
혹은 이 모두를 할당받아 정상적으로 메모리를 갱신할 때 비로소 유휴 Handoff는
완성되는 것이다．
 유휴 Handoff가 수행되는 동안 단말기는 새로운 호출채널을 통하여 적어도 하나
      6. Handoff
 .                                                  341


이상의 유효한 메시지를 수신할 때까지는 비 슬롯 모드로 동작하며, 이후 슬롯모드
로 돌아온다. 그리고 Handoff 수행 후 이전 호출채널로 받은 모튼 메시지는 버린다．


      6.6.2 Neighbor Configuration

     새로운 기지국이 이전 기지국의 Neighbor list어］ 포함되어 있다면, 새로운 기지국
으로 전환하기 위하여 NGHBR_CONFIG(3bits）를 다음과 같이 사용한다. 만약 그
렇지 않다면, NGHBRHCON町G를 '011'로 설정함과 동시어］ 그 목록 안의 Pilot어］
대해 동일한 Hando侄동작을 수행한다．
     단말기는 NGHBRCONFIG가 기지국의 형상을 알 수 없는 경우를 제외하고는
가장 최근 수신한 /\ccess Parameter 八4essage의 일련번호（ACC소'ISG_SEQs）를
NUT工로 설정하고 새로운 호출채널을 전송하는 기지국의 PN Offset을 저장하는
절차를 수행한다. NGHBRCONFIG는 FREQ牛JINCL, NGHBRBAND, NGHBR니
FREQ 등을 동반하여 인접한 기지국의 형상정보 및 유휴 Handoff어］ 태한 정보를
제공한다．
     유휴 Han面if를 성공적으로 수행하기 위해서는 단말기는 이웃 기지국의 주파수
및 호출채널과 확장 채널 목록 등과 같은 기지국의 형상어］ 대한 정보를 수집해야
한다. 유휴 Han面什를 할 때 주파수간의 천이가 필요할 경우는 주파수 변경자를 통
해서 인식하게 되며, 그렇지 않으면 현재의 채널을 유지하며, 현재의 채널에서 출력
되는 호출채널의 변경사항이나 RC 변경사항 등의 사항을 NGHBR CONFIG를 통
해서 정보를 얻어서 유휴 Hando珏를 수행한다．
 NGHBR_CONFIG= '000'
 이러한 값을 갖는 이웃한 키지국은 현 기지국과 비교할 때 동일한 호출채널 번호，
동일한 CDMA CH(FA) 번호를 갖는 기지국이다. 만일 이 레코드어］ 대해서 주파수
변경성분 FREQ_INCL이 '0'이며, 새로 대응되는 FA는 현재의 CI呱4A주파수를 그
대로 유지하며, FREQ_爪CL이 '1'이면, 단말기는 자신이 감시하던 주파수를
NGHBRBANI）및 NGHBR.YREQ에 명시되어 있는 값으로 이동하여 동기를 맞
추며, 그 다음 단말기는 동일한 호출채널이므로 같은 Code Channel을 이용하여 새
로운 기지국의 호출채널 감시를 시작한다.
 따라서 단말기가 새로운 호출채널어］ 대한 구성 Parameter를 저장하지 않았거나
저장된 정보가 현재 값이 아닌 경우어］ 새로운 형상정보를 받아야 하고 이전 것은
   342                                      6. Handoff
                                                         口


필요 없는 정보이므로 CONFIG小心G_SEQ（시스템 Parameter, 인접 셀 목록，
CDMI\ 채널 목록, 확장형 시스템 Parameter, 확장형 인접 셀 목록 메시지어］ 대한
메시지 일련번호） 값을 NULL로 설정한다．
 NGHBR CONFIG= '001'
 이 값으로 표시되는 인접 기지국은 현 기지국과 다른 호출채널 번호를 사용하게
되며, 동일한 CDMA CH(FA) 번호를 갖는 기지국이다. 만일 이 레코드어］ 대해서
주파수 변경성분 FREQJNCL이 '0'이며, 새로 대응되는 FA는 현재의 Cl呱4A주파
수를 그대로 유지하며, FREQ_INCL이 '1'이면, 단말기는 자신이 감시하던 주파수를
NGHBR小BANT）및 NGHBR_FREQ에 명시되어 있는 값으로 이동하여 동기를 맞
추며, 그 다음 단말기는 다른 호출채널이므로 1차（prim계y) 호출채널의 감시를 시
작한다．
 따라서 단말기가 1차 호출채널에 대한 구성 Parameter를 저장하지 않았거나 저장
된 정보가 현재 값이 아닌 경우 단말기는 CONFIG小4SG_SEQs（시스템 Parameter,
인접 셀 목록, CDMI\ 채널 목록, 확장형 시스템 Parameter, 확장형 인접 셀 목록
메시지어］ 대한 현재 메시지 일련번호） 값을 Nm工로 설정한다．
 현재 CDMA시스템에서 제공되는 호출채널의 수를 나타내는 PAG且CHANs값
을 '1'로 설정한다.
 NGHBR_CONFIG= '010'
 이웃 기지국은 현 기지국과 비교하여 호출채널과 CI呱4A 주파수가 모두 다른 경
우이다. 만일 이 레코드에 대해서 FREQ皿나CL이 '
                            '0이면 ，이웃 기지국은 현 기지국
이 전송한 CDMA 채널목록 메시지의 CDMA채널상에서 Prim町y 호출채널로 이동
해야 한다. 만일 FREQ_INCL이 '1'이면, 대응하는 Cl呱4A 주파수는 NGHBR
BA口）및 NGHBR_FREQ에서 지정된 Cl呱4A주파수상의 1차 호출채널로 이동해
야 한다. 또한 단말기가 Extended 채널 List를 수신하여 처리할 수 있다면 단말기
는 확장채널 목록 중 첫 번째 주파수로 천이하여 새롭게 주파수를 선택하먀 하고,
그럴 수 없다면 채널목록의 첫 번째로 천이해서 새로운 주파수를 할당받아야 한다.
물론 단말기는 천이된 그리고 할당된 새로운 주파수에서 첫 번째 호출채널에서 호
출채널번호와 Si毗을 다시 할당받을 것이다.
 단말기가 1차 호출채널어］ 대한 구성 Parameter를 저장하지 않았거나 저장된 정
보가 현재 값이 아닌 경우 단말기는 CONFIGUMSG_SEQ（시스템 Parameter, 인접
      6. Handoff
 .                                               343


셀 목록, CDMA 채널 목록, 확장헝 시스템 Parameter, 확장형 인접 셀 목록 메시지
어］ 대한 현재 메시지 일련번호） 값을 1로 설정한다．
     그리고 CDMABAND(CDMA대역등급. CDMA대역등급은 단말기가 사용한다）.
값을 NGHBRB사nX이웃 대역등급）로 CDMACH(CDMA 채널 번호） 값을
NGHBRFREQ（이웃CDMA 채널번호）로 설정하고 새로운 CDMA 채널에 동기를
맞춘다．
     NGHBR CONFIG= '011'
     이 값은 단말기가 새로운 시스템 표시와 함께 단말기 초기상태의 시스템 결정 부
상태로 들어가서 새롭게 시스템을 획득하여서 유휴 Hando卄하는 것을 표시한다. 이
때도 단말기는 새로운 시스템 획득을 위해서 가장 먼저 이루어지는 Pil야 획득 과정
에서 사용하는 채널을 현재의 CDMA 채널로 할 것인지（FREQ皿寸CL = '0'), 아니
면 새롭게 표시된 주파수와 밴드등급으로 할컨지（FHEQ_INCL = '1'）를 FREQ_
INCL 필드를 보고 판단하여 수행한다．
     이상의 결과들을 정리하는, 예를 들어 단말기가 유휴Hando珏를 할 때 NGHBR
CONFIG가 '001'로 설정되어 있는 기지국으로 이루어진다면 같은 FA로 이동하햐
하며, 호출채널 번호는 현재 서비스받고 있는 호출채널 번호가 아니라 Primary 호
출채널로 이동해서 Has川ng어］ 의해서 새로운 번호로 이동할 것이다．
     중첩지역에서 NGHBRCONFIG를 '010’으로 설정하여 단말기에 정확한 주변상
황을 알려주어야 한다（현재 서비스 받고 있는 CI呱4A CH에서 첫 번째 있는 FA로
이동하여 Primary 호출채널을 수신）. NGHBR_CONFIG가 '010'일 경우는 주변의
기지국이 FA가 다르다는 것을 알려준다. 하지만 NGHBR小CONFIG가 2(='010'）이
므로 현재 서비스받고 있는 채널의 CDMA Channel List Message에서 제일 첫 번
째 FA로 이동하여야한다. 이때 단말기는 초기화 상태로 천이하지 않고 단순히 FA
만 이동하여 대기상태가 된다.
 새로운 FA로 이동하였을 경우 호출채널은 Prirnaiy 호출채널로 설정한다. 따라
서 단말기는 새로운 FA의 Primary 호출채널로 이용하여 overhead Message를 이
용하여 서비스 받을 FA, 호출채널, slot nun小er를 결정한다．
 유휴 Hando拜는 Extended Neighbor List Message를 근간으로 수행되므로
Ilandoff 완료 후 바로 대기상태가 될 수 있다. 즉 단말기는 Pilot PN값을 모두 알
고 있으므로 새로운 Pu야을 검색할 필요는 없다．
    344                                                                        6. Handoff
                                                                                            口


 단말기는 유휴Handoif를 수행할 때 인접 PN의 정보는 Extended                                         Neighbor
List Message의 NGHBRCON町G에 정의되어 있다. 이 메시지에는 인접 기지국
의 FA, 호출채널 번호 등의 정보가 들어 있다．



       Access Handoff


 IS -95의 므REV가 4보다 작은 단말기는 시스템어］ 접속하기 위한 상태에서 동작
할 때는 망과의 Interoperab小ty를 위하1 호출채널을 바꾸는 일종의 유휴 Hando卄를
수행하지 않고 Pilot se可ch만 수행하였다. 그러나 이러한 상태에서도 이러한
Handoif 동작이 필요한 상황은 충분히 발생될 수 있으며, 이것으로 인해서 호 접속
실패어］ 대한 가능성은 충분히 있는 것이다. 때문에 이러한 상태에서도 유효한
Pagii垠을 계속적으로 monit아할 수 있는 절차가 필요하다. 따라서 이 절에서 공부
하게 되는 /\ccess Han面if가 바로 그러한 절차를 나타낸다．
 이와 관련하여 IS-95B 이상에서는 /\ccess 채널상의 Pu毗 보고와 /\ccess En甘y
Handoff, Access Probe Handoff, Access Hando卄과 채널 할당 중 Soft Handoff
그리고 /\ccess Probe back-o卄 delay감소 등의 기능이 추가되어서 좀더 안전한
Access Attempt가 되게 하고 있다．
 （그림 6-27）은 단말기가 /\ccess 상태어］ 어떠한 경우로 동작이 되는지를 나타내
는 그림이다．



          戶戶
        호的 채 넌   단밗가 뇬
                                 I      長       P
                                        단발7! 가 立출 群
                                                      1               聽
                                                                          /
                                                                   단먈기가 호發 채널
                                                                               I
                           System
                                           \\
        슐럿 외 시   AEH04蚤    Access       녈］08L長三 검출한                lost發 건爵한 후 또
        쟈섞       수행할       Attempt 전입   후 1:］꾼 기지국으                다뷴     기지국으로
                 수 있음．                  로 APHO율 수행．                AHO율 수행．




   r   겹 단말기가 깨어나서 가장 강한 파일럿 신호탐색 [                   I OVIH) 갱신

   L H그 GPM의 호출을 수신                             1     1 吼로운 BS로 첫번째 /\CCeSS Probe 전

    三；
     ii難難重 OVHD 메시지 수신 가농．                      驪蠱 ACK클 수신하지 봇하고 다윰 Probe 전송

   -      첫．번째 Access Probe 전송                  區目目 Access Probe 에 대한 ACK수신

    :;;::" ' ::ACK룔 수신하지 못하고 다음 Probe 전송        111       여러 개의 Pilot Set윤． 니따내뇬 ECAM수신

                          （그림 &27) System Access 미agram
    6. Handoff                                        345
.


     6.7.1 Pilot Reporting

    모든 /\ccess 채널 메시지들이 Pilot 강도 측정과 관련된 공통필드를 가지고 있으
며, 이것은 Access시에도 단말이 느끼고 있는 수신 전계 강도 정보를 망으로 보고
하고 있어서 이러한 /\ccess Handoff를 실현할 수 있게 하1 준다. 이러한 방식은 기
존의 그것과는 달리 단순히 Pilot의 탐색과 측정이 아니라 그러한 결과를 망으로 보
고한다는 측면에서 진일보（進1步）한 방식이라 할 수 있다．
    통화채널이 완전히 열리지 않는 상태에서 Pilot 보고가 있게 된다면 분명히
Access 시도 상태에서의 성능 개선은 분명하다. 이러한 Pilot보고 방식은 단말기가
채널을 할당받을 때 Extended 채널 Assignment Message를 통하여 /\ctive Set의
하나 이상을 포함하여서 단말기가 가능한 빨리 Soft Hando珏를 가능하게 금해 준
다. 또한 이러한 Pil毗 보고는 /\ccess와 Access Probe Hando侄를 위해서 P11毗 정
보를 제공한다．
    이러한 Pil야 보고는 단말기가 측정하고 보고할 Pil야들을 관리하는 절차가 필요
하기 때문어］ 가능하다．
    단말기의 Pilot 보고 대상이 되는 것은 대기상태의 /\ctive Set으로 생각될 수 있
는 ACCESS_HO_LIST와 Candidate Set으로 생각되는 OTHER니REPORT_
LIST들의 P11야들이다. 이러한 목록들은 시스템 /\ecess 상태진입 이후 첫 번째
Access Probe가 전송되기 전어］ 구성된다. 때문어］ 이때부터 P11毗보고가 이루어지
며, 이러한 보고는 /\ccess Probe를 통해서 이루어진다．
    이러한 /\ccess Probe는 /\ccess 채널 八1essage를 전송하며, 때문어］ 모든
Access 채널 메시지들은 이러한 Pu야보고사항을 전송할 수 있다. 그러나 이러한
사항은 단말기가 대기상태어］ 수신한 Extended System Parameter Message의
PILOT1REPORT필드를 통해서 /\ccess 채널 메시지어］ ACCESS_HO_LIST와
OTHER_REP아｛TLIST의 Pil毗들을 어떻게 보고할 것인지를 결정한다. 예를 들
면 PILOT_REPORT필드가 1이라면 모든 /\ccess 채널 메시지들이 Pilot 보고를
하고, 0이면 단말기가 전송하는 Origination과 Page Response 八4essage에만
ACCESS_HO_LIST와 OTHER_REP아｛TLIST의 P11야을 보고한다．
席嬅露聲無瓢

    Access Handoff List

    ACCESS_HO_LIST은 단말기가 Access 혹은 /\ccess I노obe Hando珏를 수행할
    346                                          6. Handoff
          1                                                   .


때 사용하는 P11毗들로 이 목록 으 목록안의 P11야의 강도와 Pu毗셋의 정보가 기지국
어］ 의해서 인정 받은（이 Pu야들이라 할 수 있다. 이러한 의미에서 우리가 이야기한
Active Set과 유사한 개념의 분류라고 할 수 있다
  이젓들은 최대 6개까지 관리될 수 있으며, 이것은 단말기가 Access Probe를 막
전송하려고 하는, 즉 시스템 접속시도 상태 이전어］ 구성이 되며, 바로 그때 적용될
수 있는 이웃 기지국 정보이다. 즉 그때가 아니면 다음에는 쓸모없는 데이터가 된
다. Access 단계에서 이루어지는 Handoff가 채널의 변화 상황을 잘 반영하여
Han面If를 수행하기 위해서 이것은 이러한 시간이 치나면 효과가 없어지고 갱신되
어야 하는 것이 지극히 타당할 것이다．
 Access Handoff List의 갱신은 ESI呱4내의 ACC_HO_LIST_UPD값어］ 의해서
이루어지는데, 그 값이 '0'이라면 ACCESS_HO_LIST는 처음 이 목록의 Pu毗들의
Pul毗 강도를 매 /\.ccess Probe마다 그것들의 값을 갱신하여 보고한다. 그리고
ACCHOLISTUPD값이 '1'이라면 ACCESS_HO_LIST는 /\ccess Attempt 때
마다 새롭게 ACCESS_HO_LIST를 재구성하고 이것들의 Pilot 값들을 보고하는
형태로 진행될 것이다．
 즉 ACCHHO_LISTmUPD값이 '0'일 때는 Pilot 목록 은 변함이 없고 Pu毗 강도만
이 갱신되어서 매 /\ecess I노obe 마다 보고되고, '1'일 때는 Pilot 목록과 그 Pil毗들
의 값까지 모두 갱신하게 되는 경우이다．


 Other Reported List

 OTHER REPORTEI工LIST는 TAIJD를 넘는 세기를 가진 Pil毗이지만 실지로
Access 혹은 /\ccess Probe Hando卄를 위해서 사용될 수 없는 Pil毗들이다. 이것
역시 망어］ 알려져 있는 I出毗이나, 이것의 Pilot은 ACCESS_HO_LIST가 모두 망어］
보고되고 message capsule Size에 여유가 있을 때 이것은 /\.ccess 메시지어］ 포함
될 수 있다. 이런 의미에서 ACCESS_HO_LIST와 대조적이며, 이것의 Pilot 구분
상의 성격이 통화채널상에서 관리되는 Candidate Set과 유사하다.
 이것 역시 시스템 접속시도 상태에 들어간 후 첫 번째 /\ccess Probe가 전송되기
이전어］ 구성이 되며, 연속적인 /\ccess 채널 Probe들을 전송한 후 그것의 개수, 강
도, 위상 등이 갱신된다. 즉 OTHER_REPORTEI工LIST는 그것의 개수가 변하며，
그것은 단말기가 /\.ccess Attem砒의 각각의 /\ccess Probe를 전송하기 이전어］
     6. Handoff                                                                                         347
1

OTHERJEPORTEI工LIST를 재생산한다．
 席響客絮無，

    IDLE Handoff REC

    Idle Handoif, Access Entry Handoff, Access Handoff, Access Probe Handoff
을 수행하기 위해서 단말기가 관리하는 Pilot 셋이며, 이것은 Extended/ General
Neighix才 List Message어］ 포함된 모튼 Pilot들이며, 이러한 Pilot 목 록 은 단말기만
이 관리하고 보관하는 Pilot 목록으로 앞서 설명한 OTHER REP아｛TED卄 LIST와
비슷하게 기지국으로는 Pilot 강도, 위상 등과 같은 정보가 보고되지 않는다．
    이상의 항목들은 단말기에서 관리하고 있는 Pilot 목록들로 Pilot 분류의 기본 개
념은 앞서 이야기한 통화시 Pilot 분류의 개념과 흡사하다. （그림 6-27）과 28은 이러
한 Pilot 보고의 과정을 보여 준다. 이러한 Pilot 보고는 이후어］ 설명될 /\ecess
Handoif를 위한 기본정보로 사용되며, 이러한 기능으로 인해서 /\ccess Han面If가
이루어질 수 있다. （그림 6-30）은 이러한 /\ccess Han面if의 종류와 발생시점을 보
여 준다.


                                                    P l
                  Access Attempt시작            a  '
                                              9 h 있； Fi lot
                                                  VJ
                                                   촤디1 허용 'n "
                                                                                                              \
                                                                                                              \
                  Tirst_Access_Probe                  包1'] 하 띤 N =
                      = l ' 로 설정
                                                                                 「 뇨rm1        口n   n

                                                                                  [ 1
                                                                                        11 1
                          Y
                   기지국으로 보고할
                   Pilot수 N올 결정．



                   기지국으로 보고할
                   P11야수 N을 결정．                                   OTHER_REPORTED_LIST
                                                                          발생


                                                            ACCESS_I 10_LIST발생



                                                       First코ccess_r玎obe = 0
                   first_access_prob   yes* f江st_pil。
                                                    t=Active sot pilot
                          e=1 ?                          prey_pilot = none
                            no


                   ACC_HO_LIST_U       ve.s
                       PD=1?

                            no                                   和 ACCESS卞HO_LIST 갱신


             （그림 &28) A0CESSHO니ST와 OTHE日e日EPO日TEDLIST발생
 1    348                                                                                                6. Handoff
                                                                                                                               .




       Access i i '.『 MSG叫
       Active Set Pilot윤 보
       고내용윤           」’d 겅 하고
       Access量｝ 시도
                                                                                                   yes
                                                                                                    ,>Access attempt
                                                                                                           성공
                                         V

       目;P\！얘 포함             rCCIOS_ \I I E 1r'T= FRLE
         .:F 확인



                                 PILOT_REPORT =1?




                                  OrgM 먀 PRM ?                          yes
                                                                                           Access 채녈 l匹SG어｝
                                  1\               /1raH
                                                                                           ACCESS_HO_ LIST 와
                                                                                           DIRER REPORTED LI
      4! 川 MS G ' art只nation
                                                                                           ST: I Pilot :｝윽 보고．
      '1｛「Page re키）onse
      meSeage 'n ' }?


                             （그림 &29) Access Probe에서 P11아 日eport




      Idle   State                                                   S外tem Access State




                        Update Overhead                                         Paging, Response
                          Information                                              Substate
                            Substate
         Access                                            Access
                                                                                     Access
        品듬誥                                                 Probe
                                                           Handoff                 1-landoff




                                                                      BS PCK                                 MS 戶CK




 1
                                                                      Order




                                                                        I
 q끼                                                                                                           0rder




                                                                                                       11.
                                                  PRM                                                 CJ4




                                                             .   .
                                                                                                                       .   .
                                             d.
                                 （그림 &30) Access Handoff 기m레ne

 여기서 설명되는 모든 /\ccess Han面甘들 역시 break before make형태로 이루
어지며, 따라서 유휴 Han面if와 마찬가지로 Hard Han面侄의 일종이다．
    6. Handoff                                                                                                  349
.

     6.7.2 Access Entry Handoff

    System Access상태의 Overhead Information 갱신 부 상태어］ 들어가기 전에 단
말기가 감시하던 유효한 호출채널을 유실한 경우에 단말기는 Access Entry Handoff
를 수행한다. 이것은 유휴 Han面if의 특별한 형태의 Han面ff로서 이러한 방법이
사용됨으로써 단말기는 /\ccess Attempt 이전에 가장 양호한 Pilot 신호를 선택할
수 있다. 때문어］ Access Attempt의 실패를 줄일 수 있는 하나의 방법이 된다．
    이러한 /]三HO를 위해서 단말기는 유휴상태 동안어］ 망으로부터 수신한 Extended
System Parameter의 ACCESS_ENTRY_HO를 확인하여 이 Handoff 허용 여부
확인한다. 물론 해당되는 Event가 발생시 AEHO를 수행한다．
    이때 단말기는 이웃 기지국들 목록인 NGHBR1REC에 있는 이웃 기지국의
ACCESSHENTRYH0필드가 '1' 이면서 그 기지국이 ACC1ENTHO1ORDER이
'1'인 경우 이 Hando奸를 수행할 수 있다. 물론 이때도 단말기는 해당 기지국과
page match가 이루어진 상태이어야 한다．
                                                                  (i I'M 시 ' 1 t j
                                                                  AIC ENI' II
                                                                  I CJEUEl=
                                                                       'I   '   )            \I 1:I:ss E\ Fi(
                    Received MSG                                                            [ [f) = 1 "1
                    other than GPM                                                          NG!lFIR Rflt.
                                                           No                               entry 4 L』    1 "




                     Received GPM


        AcLlvt I'LIOt 갸 A ( 나rI Liti                                    AEHO 이루어짐
        기      1았斟          r이 ' 『，]
        ACCESS ENTRY HO = I
        9I Plo     - :1 ’小놔드 ,1
        성 하벼 . (> } !r} h｝이 ptIc,I                                     가장 강한 Pilot .
        욜 닦색立I- :! ' s(arehcr                                          으로 AEHO 수행
                                       Construct List
        d나1 쌔 ' 三／小汁；




                                        Seerch detects          Yes

                                        S strnn口 sInt
                                       " " "
                                               시느뇨




                                                     ;




                                           Access Entry ! landoff                   Idle I landoff


                            Cit림 6- 31) Access Entry Handoff Flow Chart
                                                    6. Handoff
                                                                 U


 （그림 6-31）은 /\ccess Entry Handoff의 순서도이다．
  Access Entry Hando侄는 대기상태에 이루어지지만 이것은 Page Response상태
와 명령 & 메시지 처리상태에만 이루어진다. origination상태는 단말기가 언제
onmnation상태로 되는지는 임의적이기 때문이다．

   6.7.3 Access Probe Handoff

 Access I노obe Hando卄는 단말기가 Access Probe를 전송하고 다음의 출력을 전
송하기 전, 즉 /\ccess Probe간어］ 이루어지는 Handoif를 말한다. （그림 6-30）을 참
고하라．
 Access Probe Handoif 는 ACCESS_HO_LIST내의 Pu야으로 Handoff를 시도
하는지 여부와 Access Probe 내에 포함된 메시지의 종류어］ 따라서 다음의 4가지
경우로 구분하여 이야기할 수 있다. 우선 ACCESS_ HOLIST 내에 포함된 I꾜야
으로 Hando珏를 시도하는 2가지 경우를 생각하1 보자．
 그것의 내용이 Origir追tion혹은 Page Response 八4essage일 경우 단말기는
ESI呱4어］ 포함된 ACCESS_PROBE_HO가 '1'로 설정되어서 APHO가 허용되어 있
으며, 현재 MAX_NTJM_PROBE_HO+1개보다 작은 수의 Access 什obe를 출력
한 상태인, 즉 Access Probe 상태에서 시PHO를 진행될 수 있다. 혹은 /\ccess
I斗obe어］ 포함된 내용이 발신 혹은 호출 응답 메시지가 아닌 다른 메시지라면 이
상의 조건 이외어］ ACC卞PROBE_HO_OTHER小4SG enable(=1）되어 있어야 한디‘．
 다음으로 ACCESSm HOHLIST어］ 포함되어 있지 않은 Pilot으로 Han面if를 시도
하는 2가지 경우를 생각해보자．
 첫 번째로 /\ccess Probe의 내용이 Origination혹은 Page Response Message일
경우 다음의 경우가 만족되어야 APHO를 수행할 수 있다．
 木 단말기는 Pilot 목록과 Pilot 강도를 매 I노obe마다 갱신해야 하므로 ESI爪4오부
  터 ACCmHOLISTUPD를 1로 수신했어야 하고, APHO을 수행하기 위해서
  ACCESS_PROBE_HO를 1로 수신했어야 한다．
 水 또한 Handoif의 대상이 되는 새로운 I꾜야의 강도가 ACCESS_HO_LIST의
  Pn毗의 가장 강한 Pilot보다 강하햐 하고 그 기지국이 NGHBR_REC어］ 포함되
  ACCESS_HO_ALLOW=1로 /\PHO을 허용하고 있어야 한다. 이것은 모든 준
  비가 다되었어도 목표 기지국이 APHO을 수용할 수 없다면 아무것도 안 되기
         6. Handoff                                             351
     .


          때문이다．
         水 ACCESS_HO_LIST내에 새로운 Pilot이 포함됨으로 인해서 Access 채널의
          최대 Capsule Size를 초과하는 경우가 없어야 하고, Access 채널이 보고하는
          F出야수가 N13m(6개）을 넘지 않아야 한다．
         半 단말기가 Paging Response 혹은 Origination 시도 부 상태어］ 있어야 하고, 단
          말기가 현상태에서 入'IAX_NUM_PROBE_HOs + 1개의 /\ecess Probe Handoff
          보다 작은 수를 수행했어야 한다．
         永 두 번째로 /\ccess Probe의 내용이 Orimnation혹은 Page Response 八4essage
          외의 다른 메세지라면 위의 모든 상황을 유지하면서 추가로 ACC_PROBE_
          HO_OTHER1MSG=1인 상태일 때 APHO가 진행될 수 있다．
         이상의 조건이 만족된다면 단말기는 호출채널의 loss및 h鳩ul沮ciency일 때
APHO를 수행한다．
         단말기는 새로운 기지국으로 /\ccess I노obe를 송신하기 전어］ 새로운 호출채널
을 통해서 수신한 System Parameter/Access Parameter/Extended System
Parameter에 근거하여 단말기의 Parameter 값들을 갱신하고 처리한다. 또한 단말기
는 Neighbor List/三xtended Neighbor List /General Extended Neighbor List
Message를 수신하여 값들을 갱신하고 처리한다. Global Service Redirection
Message에서 새로운 기지국을 떠나라는 명령을 받으면 떠나야 한다．

          6.7.4 Access Handoff

         단말기는 관련 /\rcess 채널과 가장 강한 Pilot 신호강도의 호출채널을 사용하기
위해서 /\ecess Handoff를 지원한다. 이러한 Handoff는 기지국으로 응답 요구어］
대한 응답 혹은 기지국어］ 대한 응답을 기다리는 중어］ 발생하며, 이러한 기간은 앞의
（그림 6-30）에서 보았듯이 Page Response 혹은 Origination상태의 12초（T42m）이
다．
         이 Han面珏가 이루어져야 하는 경우는 호출채널의 강도에 의해서 결정되는 요인
과 응답을 하는 경우와 응답을 받는 경우 등의 조합으로 다음과 같이 4가지로 정리
된다.
    352                                                                                                                        6. Handoff
                                                                                                                                            U


          Origination 혹은 Page
          Response에    단말기는
          성공적으로 억세스 시도
          한다. T42m 시작




                                                                                                     Yes
               中                                                                             ///                         \'\ ,..
                                    PCH lost or        AHO시도 佃alt
          CAM혹은 ECAM욜               rnsufficient -+    for ECA八I or 艸乍＜                              HO 성공 ?  /
          기다린다．                                        LAM)                                         \,\   - -
                                                       n   .   1   r1
                                                                                              \\\




                                                                                                     N。      "   "




                                     C샤4혹온             단말기는 통화 채
                  V             -
                                     ECA玉4수신       -
                                                       널상에서 제어한
          Message requiring                            다．
          rest兀nse rece汁ed


                                                                                             帥Idle                       Sta   「그


                                               0



      ＜
      ( 兮三＞'";                         ACCES&HQM
                                    \．년： LRSP = 1?
                                                                        Yes
                                                                              AHO시도
                                                                              (Measage. +\
                                                                                             /"/
                                                                                                      ],,.
                                                                                                     HO 성긍? /7>+
                                                                                                    \\///
                                                                                                                 \\,,,
                    0


                        （그림 6-32) Access Handoff 디ow Chart


 System Access 상태에서 단말기가 기지국으로부터 응답을 기다리고 있는 중에
Pagii培을 잃어버렸을 경우, 즉 page loss상태이다．
 System Access 상태에서 단말기가 기지국으로부터 응답을 기다리고 있는 중어］
현재 감시하던 Paging의 세기가 약하게 되어서 더 이상 쓸모가 없어질 정도일 때의
경우，즉 page Insufficiency 상태이다. 이상의 2가지의 경우어］ 단말기는 H帥doff 할
대상이 되는 기지국이 /\ccess Handoff List어］ 포함되어 있고 이전에 수신한 ESPM
에서 기지국이 /\ccess Handoff를 지원한다는 조컨이 확인되면, 또한 현재 단말기가
Access 시도를 하고 있지 않은 상태에서 /\ccess Handoff를 수행할 수 있다．
 System Access 상태에서 단말기가 기지국으로부터 응답을 수신 후 그 메시지어］
대한 응답을 하기 전에 Pagii培을 잃어버렸을 경우이다. 즉 page loss상태이다．
 System Access 상태에서 기지국으로부터 응답을 기다리고 있는 중어］ 호출채
널이 빈약해 져서 더 이상의 복조가 되지 않아서 유용하지 않다면, 즉 page
Insufficiency 상태이다．
         6. Handoff                                             353
     .


         이상의 2가지의 경우에도 단말기는 Handoff 할 대상이 되는 기지국이 /tccess
Handoff List어］ 포함되어 있고 이전어］ 수신한 ESPM에서 기지국이 /\ccess
Hando珏를 지원한다는 조건이 확인되고, 단말기가 /\ccess 시도를 하고 있지 않으
며ACCESS_HO_MSG_RSP가 1인 상태 일 때도 /\ccess Han面珏를 수행할 수 있
다．
         위의 （그림 6-32）는 /\ccess Handoff의 처리과정을 나타낸다．

          6.7.5 Extended System Parameter message

         · F기LOT 日EP아玎 : P11아 보고 지시자

         기지국이 단말기에게 TADD를 초과하는 Pilot을 보고할 때 모든 /\ccess 채널
로 보고를 명할 때는 1로 설정하고 Origination 八4essage과 Page Response
Message에만 보고를 지시할 때는 0으로 설정한다．

         ·AC（二ENT_HO_ORDER : AEHO 허용 지시자

         If NGHBRSET1ENTRY皿寸FO 가 '1'이라면, 메시지를 수신한 후 대기상태에
서 Order와 Message Processing Operation중어］ 단말기에게 /EHO을 허용한다면
1로 설정한다．

         ' NGHB日SET_ACCESS_INFO : AHO Neighbor Set 포함 지시자

         기지국이 access Handoff 혹은 Access Probe Handoff 의 Neighbor Set상의 정
보를 포함하고 있다면, 기지국은 이 필드를1로 설정한다

         ·ACCESS_HO: Access Handoff 허용 지시자

         If NGHBR_SET_ACCESS_II
                              ＼ 下O이 '1'이라면, 기지국은 단말기가 AHO을 수행
하게 하기 위해서 이 필드를 1로 설정한다．

         ·ACCESS_HO_MSG_RSP : 메시지 응답을 위한 AHO허용 지시자

         ACCESSeHO 이 '1'이면, 단말기가 메시지를 수신한 이후어］ 그리고 그 메시지어］
대한 응답을 하기 전 상태인 시스템 /\ccess 상태 중어］ AHO을 수행된다면 기지국
은 이 필드를 1로 설정한다．
    354                                                  6. Handoff
                                                                      U


  · ACCESS_PROBE_F伯 : APHO허용 지시자

 NGHBR_SET_ACCESS_INF0가 1일 때, 기지국은 이 필드를 포함하며, 단말기
가 APH0를 지원한다면 이 필드를 1로 설정한다．

  ·ACC+HOH니ST_UPD : Access Handoff list 갱신 허용 지시자

 ACCESS_PROBE_H0이 포함되어 있고 이 값이 1이라면, 단말기가 /\ccess
Attempt중 /\ccess Handoff List를 갱신하는 것을 허용하려면 1로 설정하고, 그렇
지 않으면 0으로 한다．

  ' ACC_PROBEHOOTHERMSG : Origination과 Page Response 01외의
   Message들의 APHO를 허용 여부 표시자

 ACCESS_PROB且上[0가 '1'이라면, 단말기가 이외의 메시지들의 /PH0를 수행
하는 것이 허용되게 하려면 기지국은 이 필드를 1로 설정한다．

  ·MAX_NUM_P日OBE小HO - APHO이 수행될 수 있는 최대 시간

 망에서 APHO이 허용되었다면, 전체 /\ccess Probe에서 하나 뺀 （즉 순수하게
Access Probe 사이의 시간만을 나타내는）상태에서 APHO룔 수행하는 것이 허용
된 단말기에게 최대 시간을 기지국은 필드어］ 기록한다．

  ' NGH마_SET_SIZE : Neighbor S이의 크기

 NGHBR_SET_ENTRY皿寸FO 혹은 NGHBR_SET_ACCESS_INF0이 1이라
면, 기지국은 Neighbor List Message, Extended Neighbor List Message, 혹은
General Neighbor List 入'lessage어］ 포함된 P如t의 수로 이 필드를 설정한다．
 NGHBR4SET小ENTRYINF0가 '1'이라면, 기지국은 ACCESS卞ENTRYHO필
드를 NGHBR_SETSIZE번 이 메시지어］ 표시한다．

  ·ACCESS_ENTRY_F伯 H 시스템 Access 상태에 진입했을 때 AEHO 허용자

 대기상태어］ 호출채널을 통해서 메시지를 수신한 시간과 시스템 /\ccess 상태로
진입한 후 그 메시지의 응답을 하는 중어］ 관련퇸 P11毗의 기지국으로 /\EH0을 수행
하는 것이 허용된다면 이 필드를 1로 설정한다．
 기지국은 Neighbor List 八/Iessage, E：乂tended Neighbor List 八'lessage, or
    6. Handoff
U                                                  355


General Neigh比r List Message.어］ 들어 있는 사용중인 P11毗으로써 이 메시지의
ACCESS_ENTRY工띠을 위해서 동일한 명령을 사용할 것이다．
 상세하게 ACCESS1ENTRY4HO필드의 1 번째 항목은 각종 Neighbor List
八/Iessage의 1 번째 I出ot이다．
 NGHBR누SI汀HACCESSJNFO이 '1'이라면, 기기국은 ACCESS. HQALLOWED
필드를 NGHBR니SETSI2厄 만큼 더 가지게 된다．

    · ACCESS_HO_ALLOWED : APHO과 AHO허용자

 단말기가 시스템 /\ccess 상태에 APHO 혹은 AHO을 수행하는 것을 허용할 때
1로 설정한다. '


     6.7.6 채널할당 중 Soft Handoff

 채널할당 중 Soft Hando卄기능은 과거, 즉 IS-95의 프로토콜 개정번호가 4이하
인 소위 말하는 IS-弱A에서는 없었던 기능이며, IS -95B 이후의 시스템어］ 새롭게
적용된 Handoff 이다．
 IS-95A에서는 단말기어］ 호출채널 혹은 통화채널이 할당된 후어］ 할당된 특정한
채널상으로 수신과 전송만을 할 수 있다. 즉 Handc心는 이루어지지 않았다. 그러나
채널할당 과정에서 Soft Handoff를 수행할 수 있는 정보를 제공하1 준다면 이러한
시간에도 Soft Han＆虹를 진행할 수 있을 것이다. 즉 Soft Handoff로 진입하기 위
해서는 여러 개의 채널을 동시어］ 복조할 수 있어야 하며, 기지국은 Rake rece如er의
fir坦er의 재구성을 위한 Han面珏지시메시지 등과 갇은 또 다른 메시지를 전송해야
한다．
 기지국 혹은 망은 단말기에게 가능한 이른 시간에 Soft Handoff를 수행하게 하
기 위해서 IS円5B이상에서는 Extended 채널 Assignment 八4essage가 사용된다．
여기에는 실지로 단말기가 신호를 복조할 수 있을 정도의 하나 이상의 Pilot 신호
정보들을 포함하고 있으며, 이러한 이유로 과거에는 볼 수 없었던 통화채널 초기상
태와 시스템 Access 상태어］ Soft Hando珏를 할 수 있다．
 이러한 Han面卄가 발생될 수 있는 시간은 정확하게 말하면 단말기가 통화채널
상태로 들어가고 데이터 전송과 수신할 준비가 완료된 때에 바로 Soft Handoff상태
로 진입할 수 있다．
                                                6. Handoff
      356                                                    1



 ECAM은 4가지의 ASSIGN小4ODE를 가지며, 이러한 4가지 모드 중에서 통화
채널을 할당하는 모드인 ASSIGN소4ODE값이 " 000" 인 경우에만 채널 /\ssignment
Soft Handoff의 정보를 가지게 된다. 나머지 4개 모드（ASSIGN소4ODE=001, 010,
011）의 경우는 정상적으로 모든 채널이 할당되어도 여러 개의 Pilot 신호를 복조하
는, 즉 cell diversity를 이용하는 Soft Hando仕를 수행하지 않기 때문어］ 이러한 작
업을 하지 않는다.
 통화채널 초기상태에서 단말기의 주기능은 새로운 주파수로 천이가 필요할 경우
새로운 주파수로 tunir垠하며, 여러 개의 Pil毗을 위해 searcher 구성을 수정하고, 통
화채널의 다중화 옵션과 Rate Set 등을 설정하여 수신준비를 완료한다．
 다음은 ECAM어］ 포함되어서 CASH을 지원해 주는 필드들이다．

     · F기LOT_PN : 미아 PN sequence 에set index

     기지국은 이 필드를 A曲ye Set의 P11毗들을 64 Chii) 단위로 PN 옵셋을 설정한다．

     · PWR_COMB_IND : 전력제어 심벌 결합 지시자

 이 P丑毗과 관련퇸 Forward 통화채널이 동일한 폐루프 전력제어 부채널 Bit를 전
달한다면, 기지국은 이 필드를1로 설정한다. 그렇지 않다면 "0"으로 설정한다. 이 머］
시지 내에 이 레코드의 처음 발생되기 위해서, 기지국은 이 필드를 "0" 으로 설정한
다．
     ·CODE_CHAN : Code Channel Index

  기지국은 단말기에서 이 P11야과 연관된 Forw可d 통화채널이 사용되는 (ode
Channel index로 이 필드를 설정한다. 만약 RC 1,2,3, 혹은 5가 사용되면, 기지국은
이 필드어］ 1에서 63까지 설정한다. 만약 RC 4, 6 혹은 8을 사용한다면, 기지국은 이
필드를 1부터 127까지의 값으로 설정한다. 만약 RC가 7혹은 9라면, 이 필드의 범위
를 1에서 255까지로 한다．



            정리하71                                                )


     지금까지 각종 Handoff어］ 대해서 공부했고 이리한 Handoff 들의 특성과 그것들
    6. Handoff                                                                            357
U

이 이루어지기 위한 조컨 혹은 제공되어야할 정보들에 대해서 공부했다. 기존의
Hando卄 방식（여기에서 기존은 Is-弱A）과 개선된 방식을 볼 때 우리는 어떠한 필
요어］ 의해서 새로운 방안이 나오게 되었는지를 보아야 할 것이다．
 （그림 臼33）어꺼 보듯이 이제 우리가 사용하고 알고 있는 단말기는 Hand(：府가
이루어질 필요가 있는 어떠한 상태에서도 Handoff를 수행할 수 있다. 그리고 단말
기가 처해 있는 상황이 Hando珏를 수행하기 위해서 독자적으로 수행해야만 하는가
아니면 망과 의논하면서 해야 하는가에 따라서 또 나누어 생각할 수 있고 이것은
망 자원의 사용 성격과도 직결될 것이다. 단말기가 독자적으로 행하는 Hando卄는
망에서 관심이 없다는 이야기 혹은 망에서 알 수 없다는 이야기가 된다. 이러한
Handoff 들은 망에서 자원관리를 개별적으로 하지 않는 경우일 것이다．


                       OROM or l 'RM      SCAM or
                                 +         CA知i
                                                     SCM SCCM AWIM
                                                                             Rek:as
                                                                             e order



                          十
           Idle HO AEHO     APHO       MW               CASH          MASt-JO
                                                                      MAHHO



                                                                                                ==
           AEHO : Access Entry Handoff
           APHO : Access Probe Handoff
           AHO : Access Handoff                                     Idle State
           CASH : 채널 Ass唯nment Soft Handoff
           MASHO : Mobile Assist Soft Handoff                       System Access State
           MAHHO t Mobile Assist Hard Handoff
                                                               111Initial Traffic State
           GPM : General Page Message
           OROM : Origination Message
           PRM : Page Hesponse Message                         111Traffic State
           E(AM : E汀比ndtd iI녈 /\ssi표nmcnt Mes謫恥
           SCM : Serelee （沁nuert tori 入tessa只t三                -    Sync State
           E江；CM : Service （뇨ri nec lion （油ft帥ne 入lessa！恥
           AWiM .4 Alert With Information Messa只e


                              （그림 &33) 단말기 상태별 Handoff


（그림 6-33）에서 유일하게 Handoff가 없는 영역이 동기상태이다. 이 상태는 시스
템을 처음 결정하는 상태이므로 변경할 시스템도 망도 없는 상태이므로 Hando珏와
다음어］ 이야기될 로밍도 전혀 필요가 없는 상태이다. 사실 이 상태를 이야기하면서
Han面丘이니 로망이니 하는 이야기를 하는 것 자체가 논리적으로 이야기가 되지
않는다．
 이제 Handoff어］ 대한 이야기는 대충 다 한 것 같다．
    7. 日ad向 Transmission Technic卜Jo                 359
.




                                      adio Transmission
                                             Technique




    우리가 버스를 탈 때에 버스어］ 오르면서 토큰이나 교통카드를 인식한 후 운전기
사의 묵시적인 허락 후 버스를 탄다. 만약 누군가 버스를 탈 때 이러한 규칙을 어긴
다면 어떻게 되겠는가？
    또한 집에서 전화를 걸 때 우선 수화기를 들고 통화 가능한 링 소리를 확인한 후
다이얼링을 하고 신호가 가는 소리, 즉 링 백 톤을 틀으면서 상대방이 전화받기를
기다린다. 그런데 만일 누가 이러한 규칙을 어긴다면 어떻게 되겠는가9
    버스를 탈 때나 전화를 걸때나 나름대로 규칙이 있으며, 이러한 규칙은 준수될 때
어］ 비로소 예상하는 다음의 절차를 수행할 수 있다. 이러한 규칙 혹은 규약 등을 통
신에서는 프로토콜이라 한다. 이 장에서는 CI呱4A 통신을 위한 무선인터페이스상
의 규약과 그 이러한 규약의 설정 혹은 재정시 필요한 고려사항 등을 통해서 전반적
인 CDMA 이동통신의 이론과 IS-95방식의 예를 공부하겠다．
I1m
       360                        7. 日ad山 Transn기ss山n Technique




         Qualcomm의 기본적인 생각은 ?


      Qualcomm의 시스템 엔지니어들은 새로운 무선 통신망어］ 대한많은 고민을 했을
것이다. 그들의 목표는 기존의 TDMA나 FDMA의 방식들과는 무언가 차별화될 수
있는 시스템을 원했을 것이다. 그러한 차별화라는 것은 차라리 획기적이라고 이야
기하는 것이 더 타당할지 모르겠다. 어찌 되었든 그들은 좀더 우수한 품질의 서비스
를 더 많은 사람에게 할당하1 줄 수 있는 방법이 목표였을 것이다．
      그 당시 유럽에서는 다중접속 방식을 TDMA를 사용하는 GSM방식의 이동전화
가 대중화를 이루었으며, 이미 디지털 신호 처리기술, 즉 데이터 압축기술 등은 상
당한 수준어］ 올라와 있었다. 이러한 조건에서 Qualconim에서는 상당히 역설적인
방법을 생각하게 되었으며, 그러한 생각의 결과가 다중접속 방식을 CI呱4A 방식으
 로 하는 방안을 찾은 것이다．
      이 방식은 기존의 TI孤4A나 Fl呱lA에서 채널 용량을 증가하기 위해서 스펙트럼
 효율어］ 관심을 기울였던 것과는 정반대의 방법을 택한 것이다. 즉 스펙트럼 효율을
 에러 확률로 trade off할 수 있는 값이라고 규정함으로 이것이 가능해졌다. 즉
Qualcomm Engineer들은 다중접속 방식을 CI呱4A로 설정하고 여기어］ 맞는
Source Coding, Channel Coding 八如dulation방식들을 CDMA어］ 가장 적합한 방
 식들로 그것을 선정하였다. 즉 스펙트럼 효율은 떨어지더라도 에러 확률을 향상시
  켜서 좀더 높은 CII爪IA Processing Gain을 확보하여 용량증대를 꾀하려고 했을 것
 이다．
      또한 Qualcomm에서는 TI呱4A나 Fl孤hA에서 용량을 확보 혹은 조절하는 것이
  거의 불가능한 반면 주어진 대역에서 용량 증대를 위해서 CDMA방식은 그것의 증
 감 여부를 조절 가능하다는 장점도 생각했을 것이다．
      이 장에서는 이러한 IS-95의 RTT를 이러한 관점에서 고찰할 것이다. Source
 Coding의 경우 QCELP나 EVRC 등과 같은 variable 코드율을 통해서 에러 확률을
줄여줄 수 있게 했으며, 이것어］ 대해서는 9장에서 상세하게 공부해 보자. Channel
（뇨血堆과 modulation 등은 이 장에서 좀더 깊이 공부할 수 있을 것히다．
口
    7. Radio Transmission Technique                                     361
                                                                              I
口학的」ing                                                                       1
 일반적으로 Channel Coding은 전송할 디지털 데이터를 채널상에서 발생할 수
있는 각종 에러로부터 보호하여 정보의 복호어］ 문제가 없도록 취해 주는 사전작업
이다. 이것은 전송한 데이터어］ 대해서 안전하게 도착했는지의 여부를 알아보고 조
치를 취하는 확인의 일종으로 Forward Error Correction(FEC）이라 한다. 이것의
반대개념으로 ARQ（如的m毗ic Repeat rQuest）라고 하며, 재전송을 요구하는 형태
의 Channel Coding 방식도 있다．
    Is的의 RTT에서는 앞서서 이야기된 대로 Error pr的的小ty를 가능한 작게
하기 위해서 아주 강력한 채널코딩을 수행한다. 이러한 방법으로는 Convolutional
부호화를 사용한다. 이것은 작게는 75%, 크게는 100%가 넘는 redundancy를 가지
고 전송되어진다．
 일반적으로 코딩은 코딩될 데이터와 코딩된 데이티, 그리고 코딩해 주는 시스템
으로 구성된다. 즉 입력할 데이터를 In(S）라고 할 때 출력은 In(S)H(S）일 수 있고，
In(S）米H(S）일 수 있다. 즉 이 2가지 형태 중 하나로 부호화될 것이다. 이러한 결과
값은 일반적으로 입력보다 더 넓은 대역을 가지는 신호가 된다. 이러한 잉여분의 대
역어］ 해당하는 정보를 Redun由ncy라고 하며, 이러한 Redundancy는 데이터의 신
뢰성을 더 높여주는 역할을 한다. 이러한 Redundancy 성분으로 인해서 대역폭이
넓어지게 되는 것이다. 즉 채널코딩은 대역폭을 희생해서 달리 이야기하면 스펙트
럼 효율을 감소시켜서 에러성능을 향상하는 방법인 것이다．


          입력 테이터 In(S)            Encoding Syste       출력 데이터 Out(S)
          (Codtfl죵할 뎨이터） 1卞             Li(S)      나尸卜 (Coding 된 데이터）


                             （그림 石］)Encoding의 원리



 이러한 채널 코딩은 크거］ Block 부호화와 Cony아毗ional 부호화가 있는데, 이 둘
의 차이는 앞서서 이야기한 대로 출력이 입력 데이터와 Coding System간어］ 곱하
기로 인해서 코딩하는 방식을 미ock 코딩이라고 하고 Cony아ution 연산어］ 의해서
만들어지는 것을 Convolutional 부호화이라고 한다．
     362                             7. 日ad山 Transmiss山n Technique
                                                                     U

  Block Code는 정해진 Frame내의 데이터들의 구성 패턴들을 Redundancy어］ 실
어서    전송하는 것, 즉 고정퇸 시간에서            독립적으로 이루어지는 것이고，
Convolutional 부호화는 Block 부호화기가 특정한 시간, 즉 Frame 동안의 데이터
를 취급하여 시간적으로 불연속적인 부호화나 이 방식은 현재 부호화되고 있는 더］
이터는 특정한 시간（즉 Clock) 앞의 값어］ 의해서 현재 값이 결정되는 형태이며, 결
국 현재의 값은 특정한 시간 동안 계속 영향을 끼치는 형태이다．
  일반적으로 Convolutional 부호화가 Block 부호화에 비해서 훨씬 강한 코드율을
가지며 IS-95에서는 에러 확률을 줄이기 위해서 이러한 Convolution 코드를 사용
하고 있다．
  전송하는 데이터의 속도가 빠를수록 Burst한 Error 가 발생할 가능성이 훨씬 커
진다. 일반적으로 에러가 발생하는 시간이 같다고 한다면 같은 시간구간 동안 더 많
은 데이터가 전송되는 고속에서는 더 많은 데이터의 Burs한 에러가 발생할 것이다．


                                          16개의 정보비트
                                          가 소실됨．


                                     卜




                                      >
                                     4캐의 정보비트가
                                     소실됨．


                    （그림 石2) Burst Error


 （그림 7-2）는 이러한 것을 보여주는 예이다. 즉 채널의 환경은 전송되는 데이터의
양을 상관하지 않고 시간어］ 따라서 랜덤하게 발생될 것이다. 즉 가정하기를 빠른 속
도로 전송되는 정보 Bit와 상대적으로 느리게 전송되는 정보 Bit가 있다면 같은 시
간어］ 에러가 발생된다 하더라도 빠른 정보 Bit의 경우 깨지는 정보 Bit의 수가 훨씬
많을 것이다．
 이러한 Bur就한 에러를 교정하는 부호화 방식에는 Reed-S이on均n 코드（Block
부호화）와 터보 부호화（C이wolutional 부호화）가 있다. RS 코드의 경우 고속전송을
하는 ATM(Asynchronous Transfer Mode）에서 주로 사용 코딩 방식이며, 무선어］
1
    7. Radio Transmission Technique                                  36 a
                                                                            1
서는 아무래도 Turbo Code를 많이 사용한다．
    여기에서는 IS-95에서 제안되고 있는 Cony아utional 부호화에 대해서 공부한다．


     7.1.1 Cony아Ut沁nal 부호화

 Cony아岫onal 부호화는 유한한 과거 입력 데이터（구속장）가 현재의 영향을 미치
는 특성을 이용한 부호화로서 이동통신 채널에서 산발적으로 발생하는 오류들어］ 특
히 강한 오류 정정능력을 지니는 채널 부호화 기법이다. 동기채널, 호출채널 및
Forw可d 통화채널은 Convolutional 부호화되어 전송되며, Convo뇨tional부호 생
성 단위는 Frame 단위와 동일하다．
 채널 부호화라는 것은 전송 Line를 통해서 데이터를 전송할 때 가능하면 오류
없이 전송하기 위한 수단이라고 할 수 있다. 이러한 방법 중에서 여기서는
Cot싸아U如nal 부호화기어］ 대해서 생각하1 보기로 한다. 이 방법은 Elias어］ 의해서
처음소개 되었으며, Sequential 복호화 방식이 ＼入／ozencraft어］ 의하써 소개되고, 궤
환 복호화 방식이 Massey어］ 의해서 개발되었다. 이 방법의 특징은 유한한 과거 입
력 데이터들이 현재의 데이터어］ 영향을 미치는 특성을 이용하여 부호화를 하는 것
이다. 여기서 부호화기의 N毗毗幻n을 살펴본다. 일반적으로 N毗吼幻n은 (n,k,K)와
같이 쓸 수 있다.
    來 n : 단위시간 동안에 출력되는 채널 Bit 수
    永 k : 단위시간 동안어］ 입력되는 정보 Bit의 수
    米 K : lengh of con就raint（구속장의 길이）
    永 또한 코드율 R= k/n 이다．




                                              Ui : 첫 번짜1 코드 symbol
                Input bit m
                                              u2 : 두 번째 코드 symbol




                       （그림 下3) Cony이utional 부호화기（日＝1/2,K=3)
    364                                                                              7. Radio Transmission Technique
                                                                                                                                                                          U


 즉 Channel Coding을 하면 可k배만큼의 B.W.가 더 필요하다. 그러나, 서두에도
말한 대로 오류가 적은 데이터를 전송하기 위해서 이러한 테크닉을 사용한다. （그림
7-3）은 Convolutional 부호화기（R=1/2,K=읾이다．
 （그림 7-3）과 같이 하나의 Input Data에 2개의 Output Data가 출력퇸다. 여기서
초기상태를 '00', '10', '11', '01'이라 두고 Input Data어］ 대해서 각기 어떤 출력을 내
는지（어떤 형태로 부호화됐는지）를 생각해 보자．
 Convolutional 부호화기는 현재상태에서 특정한 입력이 들어올 때 다음의 상태로
전개해가면서 출력을 발생한다. 그러니까 부호화할 Data의 현재 상태와 그 Data값
어］ 의해서 부호화값과 다음 상태가 결정된다. 이것은 복호화할 때 Data를 복호화기
어］ 입력할 때의 복호화기의 상태와 다음 상태와 상태 천이시의 출력 값으로 Data를
검출해 낼 수 있다．

   （가 초기상태가 ' 00'일 때

 Input Data가 '1'인' 경우 : 출력은（부호화） '11'이고 다음 상태는 '10'
 Input Data가 '0' 인 경우 : 출력은（부호화） '00'이고 다음 상태는 ' 00'


   (3) 초기상태마 '01'일 때

 Input Data가 '1'인 경우 : 출력은（부호화） '00'이고 다음 상태는 '10'
 Input Data가 '0'인 경우 : 출력은（부호화） '11'이고 다음 상태는 '00'


                   ti        t2                   t3                       t4                             t5
                                                                                                                                     m
                                                                                                                                                     C
                                                                                                                                                     0
                                                                                                                                                                 d
                                                                                                                                                                 아m
                   1 . 00. 00 1 , 00 1, 00
                                                                                                                                                             1
                                  ,uu             q·
                                                       ·，   u.   J／
                                                                                「．
                                                                                         ·
                                                                                             ·，   U                 00                                   d
                                                                                                                                                                 Wh
                                                                                                                                                                 ee
    State a = 00
                                                                                                      I
                                                                                                          0.
                                                                           /
                                                                                     '


                        11        11                   11              l                     11                " ii.
                                                                                                                '


                                    "                                 11                       ' l1                    ' l
                                                                                                                                 :
          b= 10    S
                                                                                                                                             1
                                                                                                                                         D
                                        1 l
                                              0                                                                              0
                                                                                                                                                                 Input
          c= 01    5         S                         V                                                                                                          bit 1

                                              0
                                                       V
                                                       V               \0                         l                 0        0
                                                                                                                                                 -               Input

                                                                                                                                         l1b
                                                            1l
                                              =


                                                                                                                                                                  bit 0
          d= 11
                             S                               0                                    0
                   1                                        l          m                          i                          n




                             （그림 刀4) Trellis 미aqram
     .
         7. Radio Transmission Technique                                   365
                                                                                 I
            (5) 초기상태마 '10'일 때1

         Input Data가 '1'인 경우 : 출력은（부호화） '01'이고 다음 상태는 '11'
         Input Data가 '0' 인 경우 : 출력은（부호화） '10'이고 다음 상태는 '01'

            (4) 초기상태가 ']]'일 때

         Input Data가 '1' 인 경우 : 출력은（부호화） '10'이고 다음 상태는 '11'
         Input Data가 '0'인 경우 : 출력은（부호화） '01'이고 다음 상태는 '01'
         이것은 부호화기의 모튼 상태를 나타낼 수 있다. 그러나 이것은 어떤 특정한 순간
의 값이며, 시간어］ 대해서는 전혀 표현되지 않았다（실지로 입력 Data는 Plus
Stream이다）. 따라서 시간어］ 대한 표현으로 재구성할 필요가 있으며, 경로 또한 중
첩을 막는 것이 필요하다. 따라서 재구성한 것이 （그림 7-4）의 Trellis I玉agram이
다．
         이러한 Cox싸아utional Code 발생기를 구현하기 위한 접속은 ＜표 7-1>과 같다．


                              （표． 7-1> Cony이山onal 부호화기의 연결

               구속장 길이                                 코드의 탭 계수
         (Length of costraint : K)           Gi                    G2
                    3                      111                   101
                    4                      1111                  1101
                    5                      11101                 10011
                    6                      111101                101011
                    7                      11111001              1011011


           7.1.2 Viterbi 복호화기

         Viterbi 복호화기는 최대 확률론적 복호 방식이며, Bit Metric Branch 入Ietric
Path 入4etric 등을 계산하여 상태의 변화를 찾아가다가 八4erge가 일어나면 Data를
복호화할 수 있다. 주어진Path His的ry내에서 Merge 가 일어나지 않을 때는 Path
入4etric가 가장 작은 경로로 Data를 복호화한다．
         半 Bit Metric : 상태 천이시어］ 발생된 Bit와 입력된 Bit의 차이를 정량적으로 표
           현한 량
    366                            7. Radio Transmission Technique
                                                                     .


  永 Branch Metric : 한 개의 Branch어］서의 Bit Metric의 총합. 이것은 복호화기
   에서 가정한 가정치와 부호화기의 실제값의 차이의 척도라고 볼 수 있다．
  來 Path 入/Ietric : 어떠한 경로까지의 Branch 入4etric의 合으로 그 경로까지의 복
   호화기에서 가정한 가정치（假定値）와 부호화기의 실제값의 차이의 척도라고
   볼 수 있다．
  Viterbi 복호화기는 기본적으로 수신단에서도 송신단과 마찬가지로 입력되는
data들에 대해서 상황전개를 그대로 재현하면서 최종적으로 패스 metric의 값이 최
소인 경로를 선택하여 그것으로 복호화할 수 있다. 예를 들면 시간이 t2인 상태에서
'01'이 입력 되었다면 이 경우 어떤 data가 01로 부호화되었느냐를 찾는 것인데, 이
것은 '0'과 '1'모두 확률이 1/2 이다. 여기서 송신측에서는 부호화된 data의 前의 상
태를 알 수가 없다. 따라서 부호화 될 때의 상황을 전혀 모른다. 앞에서도 이야기했
지만, 부호화기의 현재상태（차후의 시간에는 前의 상태가 됨） 부호화기어］ 입력된
data의 값을 알면 출력값과 後의 상태를 알 수 있다고 했으나, 여기서는 출력값만을
알고（부호화된 신호） 이것으로 前의 상태를 알아야 하고, 나아가서는 부호화된 데이
터를 찾아야 한다. 그러기 위해서는 기준이 되는 상태（이 상태를 前의 상태로 가정）
를 설정하고 입력 data의 있을 수 있는 모든 경우 2가지를 모두 찾아서 그 각각의
출력값과 입력된 data값을 bit별로 비교하여 얼마나 틀리냐를 찾는다．
 여기서 출력값과 입력된 data값을 bit별로 비교하였을 때 틀린 이유는 前의 상태
가 임의로（reference state) 설정했으므로 정확하지 않고, 또한 가정한 입력이 '0' 혹
은 '1' 하나만 맞으므로 한 경우는 순전히 전의 상태를 몰라서 생기는 error이고 또
다른 한 경우는 前의 상태도 모를 뿐 아니라 입력의 가정치도 틀렸기 때문이다．
 이러한 방법으로 따라가다 보면, 임의의 길이에서（前의 상태를 자꾸 유추해 가다
보면） '0'과 '1'의 경우가 합쳐지는 경우가 있을 것이며（merge) 이때 우리는 data를
복호화 할 수 있다 .실지로 경우의 수를 따지면 " 2, 4, 8, 16, 32,··· "이 되지만 상태들
이 겹쳐져서 경우의 수는 8로 포화가 된다．
  R=1/2인 부호화기／복호화기의 경우 발생할 수（고려할 수） 있는 상태는 '()0', '01,
                                                           ,
'10', '11'로 4개가 있으며, 여기어］ 입력 data가 '0', '1'인 2가지의 경우까지 생각하면，
어떤 상태에서 또 다른 상태로 천이하는 경우의 수는 최고 8가지의 경우가 있다. 또
한 한 상태로 들어가는 경우로는 2개 이상이 될 수 없다. 이것은 상태천이를 유발시
키는 입력 data가 '0'과 '1' 두 종류밖어］ 없기 때문이다.
U
    7. Radio Transmission Technique                                                   367

                               입력 데이터 시퀀스       M:   1     1   0   1    1
         -       Input bit 0
                               전송된 코드워드         U:   11 01 01 00        01
                 Input bit 1
                               수신된 시퀀스          Z:   11 01 01      10   01


                                                                             Branch
         State   a = 00                                                      Metric




                 b = 10




                 C = 01




                 d = 11


                               （그림 下5) Vitert升 Algorithm

 때문어］ 중복된 상태에서 그 상태까지 이르는 2가지의 경우를 비교하여 하나의 경
로만을 선택하고 나머지의 경로는 제거할 수 있다. 이것은 merge를 유도하는 실제
적인 방법이다．

     7.1.3 IS-95의 Convolutional 부호화기

 IS小95에서는 구속장이 9인（沁nvolutional 부호화를 사용하며, 필요어］ 따라서 코
드율을 달리 사용한다. 이러한 코드율은 IS小95C 이전의 RC1, 2（혹은 RS 1,2）에서
는 1/3, 1/2인 경우로 사용하는 2가지가 있었으며, 고속Packet Data를 전송하기에
적합한 RC3이상인 RTT에서는 좀더 강한 코드율인 1/4을 사용하기도 한다. 물론
다음에 이야기가 되겠으나 일정한 속도 이상의 데이터의 경우는 터보 부호화로
Burst Error를 복구해 준다．
 Forw可（I 링크의 Convo뇨tional부호는 부호율（R）이 1/2이고 구속장이 9이다. 부
호율 1/2이 의미하는 바는 1개의 입력Bit가 입력되어 Bit당 2개땍 Code Symbol이
생성되어짐을 의미하며, 구속장（K）이 9라는 의미는 Convolutional 부호화기의 천이
레지스터의 수가 9-1=8개임을 의미한다．
繭嬅藝囊瓢

 코드율이 1/2인 Convolutional 부호화기
 이러한 부호화 방식은 1개의 Bit가 입력되면 2개의 Bit가 출력되는 형태의 코딩
    368                                   7. 日ad山 Transmiss幻n Technique
               r                                                          .


을 말하며, 이것은 일반적으로 Redun由ncy가 100%가 되는 경우가 없는 Block 부
호화방식어］ 비하면 상당히 높은 코드율이라고 할 수 있으며, 상대적으로 대역효율
이 상당히 떨어지는 방식이라고 할 수 있다. 물론 반대급부로 에러 확률은 훨씬 좋
아질 것이다．
 이러한 코드율로 부호화되는 채널은 Reverse의 경우 RC2인 경우의 Reverse
Fundamental Channel4 Reverse Supplemental Code Channel 1 9으며, RC 3
에서 N=6120 이하인 경우 Reverse Supplemental Channel어］서 사용된다．
Forw可d의 경우 기존의 IS-95B의 모튼 Forw可d 채널들이 이 방식으로 부호화되
며, 여기에 IS-95C에서 추가된 방송제어 채널, 공통할당 채널, Forward 공통제어
채널 등과 Radio Configuration이 4등급인（RC4) 경우 Forward Dedicated
Control 채널과 Forw可d Supplei그nental Channel 등어］ 적용된다．

                                                               Co
          정보       f朴搏三l
          비트＋겨n汁，小
           력
          O｝
                                                               Cl



                    （그림 下6) 코드율 r=1尼인 Cony이ution비 부호화기


 이 코드의 발생 다항식은 2진수로 표시하면 g0가 111101011, g1이 101110001이
다. 이러한 이진 표현은 천이 레지스터의 입력과 8개의 출력을 연결하는 방법을 규
정한다. 이러한 표현은 앞의 3장의 코드 이론을 참고하라！
 즉, g0=111101011이란 1, 2, 3, 4, 6, 8, 9번째의 데이터들이 2진 가산되어 Code
Symbol C。
        를 만든다는 것을 의미한다. 마찬가지로 罰＝（弱1)8(101)(110)(001)2이란
1, 3, 4, 5, 9번째의 데이터들이 2진 가산되어 Code Symbol C읕 만들게 된다.
 이렇게 하여 생성퇸 Code Symbol은 생성함수 go어］ 의해 부호화된 Code
Symbol( C。
         ）이 먼저 전송되고, 생성함수 的어］ 의해 부호화된 Code Symbol( C1）이
     7. Radio Transmission Technique
.


다음에 전송된다. 초기화시의 Convolutional 부호화기 천이레지스터의 상태는 모두
0인 상태이다． 초기화 후에 처음 전송되는 Code Syn巾ol은 생성함수 g0어］ 의하1 부
호화퇸 Code Symb이이다. 동기채널과 호출채널에서는 Convolutional 부호기 천이
레지스터의 상태가 Frame 사이어］ Reset되지 않는다. 따라서 통화채널의 Frame어］
만 초기화를 위한 8 Bit의 꼬리 Bit가 필요하다．
    이 코드는 부호기의 각 데이터 Bit 입력에 대해 2개의 Code Syn小ol을 발생한다．
罰어］ 의해서 부호화된 코드심볼 Co가 제일 먼저 출력되고, gl어］ 의해서 부호화된
코드심볼 C尸］ 순서 대로 출력퇸다. （그림 7-6）은 코드율 r=1/2인 Convolutional
부호화기의 실제 구성을 보여 준다．
    m嬅慰立蜘뇨




    코드율이 1/3인 Convolutional 부호화기

    코드율이 1/3인 Convolutional 부호화기는 초기의 RS1의 속도를 가지는
Reverse 채널어］ 사용되었다. 즉 Reverse의 /\ccess 채널들과 RC1의 Reverse
Fundamental Channel과 RC1의 Reverse Supplemental Code Channel어］ 사용되
었다．
    이 코드의 발생 다항식은 2진수로 표시하면 g0가 101101111, g尸］ 110110011,
g27f 111001001이다. 이 코드는 부호기의 각 데이터 Bit 입력어］ 대해 3개의 （允de




             정보
             비트
             입력




                   （그림 7-7) 코드율 r= 113인 Cony（그1utiona 부호화기
   370                              7. Radio Transmission Technique
          1                                                           .


Syn小ol을 발생한다. g0에 의하써 부호화퇸 코드심볼 Co가 제일 먼저 출력되고，
幻어］ 의해서 부호화된 코드심볼 C1, g2어］ 의해서 부호화퇸 코드심볼 C까 순서대
로 출력된다．
 이 부호화기의 초기상태는 모두 0이며, 초기화 이후 처음으로 발생되는 Code
Syrr由ol은 g0어］ 의해서 생성되는 Code Symbol이 된다．


 코드율이 1/4인 Convolutional 부호화기

 1/4의 코드율을 가지는 부호화기는 RC3이상의 IS-95C용 RTT에서 찾아볼 수
있다. 즉 고속 데이터의 전송을 위한 채널코딩으로 새롭게 제안된 방식이다. 앞서
이야기 되었듯이 이 방식은 원래 전송하려고 하는 데이터의 4배의 정보를
redundancy로 가지고 전송하게 되는 어쩌면 상당히 별난 형태의 부화화기의 출력
데이터가 된다．
 이러한 방식은 Reverse Forw可d어］ 골고루 사용되고 있는데, Reverse의 경우
IS小％C가 되면서 새롭게 추가된 모든 채널에서 이러한 부호화기를 사용하며, RC

                                                           Co




     정보
     비트
     입력




              （그림 工8) 코드율 r=1后인 Cony이ution졔 부호화기
    7. Radio Transmission Technique
1


3, 4를 사용하는 Reverse Fundamental Channel과 Reverse Supplemental
Channel어］ 사용된다. 여기어］서 RC3의 경우 N이 6120보다 작을 때 Reverse
Supplemental Channel에서 사용한다．
    F야M／可d의 경우도 Reverse과 다름없이 이러한 코드율이 IS-95C에서 새롭게 적
용된 방식이어서 Forward Dedicated Control 채널을 포함한 Forward어］ 새롭거］
추가된 채널들어］ 적용이 되며, RC 3, 4의 Forward 기본 및 Supplemental Channel
어］ 적용되는 부호화 방식이다.
    이 코드의 발생 다항식은 2진수로 표시하면 g0가 111110101, g1이 110111001,
g2가 011001011, g3가 100111011이다. 이 코드는 부호기의 각 테이터 Bit 입력어］

대해 4개의 Code Syn由아을 발생한다. g0어］ 의해서 부호화된 코드심볼 Co가 제일

먼저 출력되고, g1어］ 의해서 부호화된 코드심볼 C1, g2어］ 의해서 부호화된 코드심
볼 C2, g3어］ 의해서 부호화 된 코드심볼 C3가 순서대로 출력된다.
    이 부호화기의 초기상태는 모두 0이며, 초기화 이후 처음으로 발생되는 Code
S珥曲ol은 g0에 의해서 생성되는 Code Symb이이 된다．


     7.1. 4 Code Symbol Repetition

    기본적으로 가변속도를 제공하는＼幻코드 r로부터 나오는 데이터들은 동일한 시
스템 Clock으로 동작하기 위해서 동일한 전송속도로 맞추어져야 한다．
    Forward 채널은 기본적으로 여러 개의 신호가 한꺼번에 전송되어지는, 즉 전송
되는 신호가 다중화된 신호이다. 기지국은 여러 사람의 신호를 같이 전송해야 할 경
우가 많을 것이다. 이러한 이유로 Forw可d 채널의 데이터들은 Reverse에서 행해지
는 Gated Mode의 출력은 없으며, 언제나 동일한 속도로 전송 데이터를 전송해야
할 것이다. 이러한 기능을 제공하기 위하써 Forw可d 데이터는 데이터의 속도를 동
일하게 맞추어 주어야 한다. 이러한 방법의 가장 기본적인 개념은 느린 속도의 데이
터는 동일한 데이터를 반복하여 속도를 맞추어 준다는 것이다．
    이러한 기능을 제공하기 위해서 Code S恥nb이 Repetition이 행해지며, 이러한 작
업 후 만들어진 데이터 Bit열들은 그것의 보코더에서 출력퇸 전송속도어］ 맞추어 어］
너지값이 조정되어진다. 즉 full rate인 데이터는 half rate의 데이터보다 Bit 에너지
가 2배로 설정될 것이다. 물론 이러한 방법을 할 때에 각각의 정보 Bit어］ 할당된 어］
                                                                           7. Radio Transmission Technique
   372                                                                                                       1


너지는 그것의 반복 횟수어］ 반비례하게 할당된다. 이렇게 함으로써 CDMA채널은
Repeatation을 통해서 채널의 용량 마진을 가질 수 있게 된다. 좀더 자세하게 이야
기하면, CDMA시스템에서 사용하는 보코더는 QCELP나 EVRC와 같은 variable
코드C으로 정보량어］ 따라서, 즉 Voice Activity어］ 따라서 전송하는 정보를 변화시
켜서 CDMA채널어］ 부하를 털어주는 역할을 하였다．


                      1        O   1       O   1       O   1       O




                                           늬                           h
                                                                       毗




                1土 T11 i
                               l           O   l       l   O       O
                                   O
         EbI2                                                              반복된 후 정보비트 : 4 bps


                           1           0           1           0

            眺                                                              반복되기 전 정보비트： 2 bps
                T1

                                       （그림 下9) 데이터의 Repeatation



  자칫 이러한 Repeatation이 이러한 Voice A曲vity의 효과를 상쇄시킬 수도 있기
어］ 여기어］서 할당되는 Bit의 에너지를 Repeatation이 되는 수어］ 반비례하게 할당하
는 것이다. 즉 Bit 에너지 측면에서 생각해 보면 반복된 Bit의 경우 반복되지 않은
정보 Bit의 에너지를 마치 시간축상어］ 늘려 놓은 것과 같은 효과를 나타낼 것이다．
 IS-95의 Forw町d의 경우 Convolutional 부호화기를 거쳐서 생성된 Code
Symb아은 Code Symb아 반복을 거쳐서 일정한 심벌률을 가진 변조심벌을 만든다．
동기채널에서 Convolutional 부호화퇸 각 Code Symbol을 2.4kbps의 심벌률을 가
지며 Bk兀k Interleaving 하기 전어］ 1번 반복（각 Code Syn小이은 2번 연속으로 발
생）의 심벌률을 가진 변조심벌이 된다．
 Convolutional 부호화퇸 각 Code Symb아의 심벌률이 19.2와 9.6kbps의 2가지로
구성되어 있는 호출채널과 심벌률이 19.2, 9.6, 4.8, 2.4 kbps의 4가지로 구성되어 있
는 통화채널에서는 심벌률이 19.2kbps인 Code Symb아율은 반복될 필요가 없지만
그 외의 심벌률을 가진 Code Symb아들은 텨ock Ii北erlea叭ng하기 전에 반복되어
      7. Radio Transmission Technique             r叫m牛I
 .                                                I   373   I


19.2kbps의 심벌율을 가진 변조심벌이 된다．
     半 Code Syn巾ol의 심벋률이 9.6kbps인 경우（데이터 율이 4.8kbps인 경우） 1번
      반복（각 Code Syn小이이 2번 연속발생）
     水 （力de Symb아의 심벌률이 4.8kbps인 경우（데이터 율이 2．欲bps인 경우） 3번
      반복（각 (ode Symbol이 4번 연속발생）
     半 Code Syn也이의 심벌률이 2.4kbps인 경우（데이터 율이 1.2kbps인 경우） 7번
      반복（각 （允de Syn巾ol이 8번 연속발생）
     됨을 알 수 있다．
     Reverse 링크에서도 Forw카（I 링크와 같이 Convolutional부호를 거쳐서 생성된
Code Syn也이은 Code Syn小ol 반복에 의해서 일정한 심벌률을 갖는 변조심벌을
만튼다. Reverse 통화채널에서의 Code Syn由이 반복률은 데이터 전송속도어］ 따라
서 변한다. Code Symbol의 반복은 Forw可d과 같이 데이터 율어］ 따라서 최고속도
의 데이터 속도어］ 맞추기 위해서 반복된다．
     Reverse 통화채널에서 이들 반복된 (ode Symbol들은 중복해서 여러 번 전송되
지 않는다. 반복된 Code S珥的이들은 Block Interleaver의 입력으로 사용되고 실제
전송 전어］ 반복된 Code Syrr由ol 중 하나만 남기고 나머지는 모두 지워진 후 가변전
송 듀티 사이클로 전송퇸다．
     데이터 전송속도가 4800bps로 고정된 /\ccess 채널에서의 각 Code Symbol은
Convolutional 부호화기를 거치면 14.4Kbps의 심벌률을 가지므로 1번 반복되어 전
송된다（각 심벌은 연속해서 2번 발생）. Access 채널에서는 통화채널과는 달리 반복
된 심볼 모두가 전송퇸다．


      7.1.5 터브 부호화

 일반적으로 무선채널상에서 발생하는 에러에 대해서 Convolutional 부호화가 탁
월한 복호 능력을 가지고 에러를 정정하는 방법을 많이 사용한다. 그러나 전송되는
데이터기 고속이 될 때는 발생하는 에러의 형태가 Burst한 에러로 발생되기 싶다．
이러한 에러를 Convolutional 부호화기로 정정하기 위해서는 그것의 구속장의 길이
가 상당히 커야 하고 그것은 또 다른 지연과 프로세스상의 문제를 유발할 수도 있
다. 이러한 형태의 에러를 정정할 수 있는 능력을 배양하기 위하1 고속 데이터용 부
호화기로 제안되어서 사용하고 있는 터보 부호화를 소개한다．
    374                                   7. Radio Transmission Technique
                                                                            U


  최근 Berrou 등어］ 의하1 제시된 Turbo （뇨le는 AWGN 환경에서 비교적 간단한
복호 Algori出m을 가지면서 18번의 반복 복호시어］ 0.7dB 라는 낮은 신호대 잡음비
에서 Bit Error Rate 가 iO-5 이라는 획기적인 성능을 보임으로써 많은 관심을 불러
일으켰다. Turbo Code는 또한 페이딩 채널상에서도 신뢰성을 보장할 수 있는 강력
한 코딩 기법으로 알려져 있다．


  Turbo C兀de의 구성

  Ti.玎bo   Code를 구성하는 주된          요소로는 부호화기와 복호화기,                   그리고
Inter1eaver7- 있다. Turbo Code는 parallel concatenated recursive systematic
（力fly이utioi追1Cx扼라 말할 수 있는데, 이 말은 터보 부호화기의 특징을 잘 나타내
어 준다. 터보 부호화기의 구성은 （그림 下10）과 같다．
  터보 부호는 기본적으로 Cony아utional 부호（Coi싸olutional Code）를 병렬 연접
하는 방식이다. 이것은 두 개 이상의 구성 부호화기（component 코드）에 같은 시퀀
스의 서로 다른 배열을 적용하는 것이다. 즉 원래 연구되어 오던 직렬 연접 부호가
전송하고자 하는 시퀀스어］ 하나의 부호를 적용하여 부호화한 다음 이 부호화된 시
퀀스어］ 다른 부호를 적용하여 다시 부호화하는 이중 부호화의 과정이었다던 것어］
비해 새로 제안된 터보 부호는 같은 시퀀스를 배열만 바꿔서 서로 다른 부호화기어］
적용하는 방법이다．
  즉 회퀴적인（Recursive) Convolutional 부호화기가 대칭적으로 있으며, 하나는


                따                                      x




                                                       Yl




                                                       Y2

                         （그림 工］0) 터보 부호화기
     7. Radio Transmission Technique
 a                                                       375


입력신호 그대로 또 다른 하나는 Interleaving을 거친 데이터가 입력이 되는 형태이
다. 입력으로 정보 Bit (dk)가 들어가면, 정보 한 Bit당 세 Bit의 출력이 나온다. 정보
Bit와 동일한 Bit, 즉 Systematic 출력과 함께 Convolutional 부호화기의 출력으
로 한 B迂(Yl）가 나온다. 이 때 부호화기는 일반적으로 사용되는 Convolutional 부
호화기와는 조금 다르게, 입력이 궤환되어 출력을 결정하며, 순환적인 코드를 만드
는 형태인 Recurs如e Convolutional 부호화기라 한다（3장 참고）. 나머지 한
Bit(Y力는 정보 Bit가 Interleaver를 통과해서 나온 B此mk）를 입력으로 하는
Recursive Convolutional 부호화기의 출력이다．
  Yl, Y2를 결정하는 두 Recursive Convolutional 부호화기의 발생 다항식은 항상
같을 필요는 없으나 일반적으로 같은 것을 사용한다．
  입력 시퀀스 dk는 첫 번째 구성 부호화기를 통해서 부호화하지 않은 출력 x와 부
호화된 출력 已를 발생시킨다. 같은 입력 시퀀스 dk는 I砒町leaver를 통과한 후 두
번째 구성 부호화기를 통과하여 부호화된 출력을 통과하여 부호화퇸 출력 Y2를 발
생시키게 된다. 이러한 터보 부호의 부호화 방법은 지금까지 많이 적용되어 온 직력
연접 부화처럼 한 부호화기를 통과한 시퀀스에 다른 부호화기를 적용한다기 보다는
두 개의 부호화기가 비록 배열은 다르지만 같은 입력 시퀀스의 집합에 적용된다는
점 때문어］ 이를 병렬 연접 부호 (p可a끄el concatenated 코드）라고 부른다.
 （그림 7-10）의 경우 코드율은 1/3이고, 코드율을 높이고 싶으면 천공된 코드를 사
용한다． 부호화기의 구속장의 킬이가 커질수록 성능은 좋아지지만 복잡도가 증가하
거］ 된다. 구속장의 길이가 정해졌을 때 어떤 생성 다항식을 쓰는 것이 가장 최적인
지는 이미 밝혀져 있다（3장을 참고하라）.
 Interleaver는 주로 pseudo-random Interleaver가 사용된다. Turbo Code의 성
능어］ 영향을 미치는 것은 Interleaver의 종류라기보다는 Interleaver의 크기이다．
Interleaver의 크기가 커질수록 성능은 더 좋아진다. I砒町노aver의 크기가 10배가
되면, BER(Bit Error Rate）은 대략 1/10배가 된다. 하지만, Interleaver 크기가 커
지면 그어］ 따라 delay도 증가하게 되므로 원하는 성능을 얻기 위해서는 delay와
복잡도 사이에서 trade-o侄가 필요하다. 한편 Turbo Code의 수신단에서는 궤환
을 통한 iterative 복호화를 하게 된다. （그림 7-11）은 Turbo Code의 궤환 복호화
기 이다.
                                                         7. Radio Transmission Technique
   376                                                                                     U



                        乙，
                             ,r따7   rDe-
                                           Interleaver
                                                                乙2e('d 'k)




          yl 寸    4 복호화기 1
                                                                   복호화기 2
            HHg
            大k    三


                                                                    복호화기
                                                                         +
                                                                    0utput
                             >m
                       （그림 7-11) 궤환 복호화71



 Codeword dk, Y1, Y ' l71- modulation된 신호가 채널을 통과한 후 수신단에서
Demodulation되어 나온 값을 각각 尤左, Yi, Y2근｝ 하고, Interleaver 깊이만큼의 더］
이터를 받았다고 가정한다. 이 때 兀左, M를 입력으로 하는 첫 번째 복호화기의 출력
값은 hard-decision에 의한 값이 아니라    ， 신뢰성 있는 정보를 함께 가지는
soft-decision어］ 의해 얻어진 값이다. 이 값은 systematic 성분어］ 의한 값과 priori
probability어］ 의한 값, 그리고 parity bit yl어］ 의한 값으로 나눌 수 있다．
  이중 parity bit어］ 의한 값을 Extrinsic Information(Lie( 따力이라 하고, 이 값을
두 번째 복호화 기에서 이용하여 신뢰도를 향상시킨다. 복호화기2에서도 복호화기
1과 마찬가지로 Extrinsic Information (Lie( 따））을 복호화기 1로 궤환시킨다．
 이런 iteration을 대략 10회 정도 수행한 후 soft-output의 부호를 보고 최종적으
로 hard-decision을 내린다. 복호화기1, 복호화기2는 sof卜output 복호화
Algorithm 이어야 하고, 두 복호화기는 서로 같을 수도 있고 다를 수도 있다. 이제
복호화기1, 복호화기2어］ 사용되는 복호화 Algoi砒hn뗘］ 대해 알아보자．


  복호화 algorithms

  Turbo Code의 복호화 Algorithm은 크거］ 두 종류로 분류될 수 있다．
  첫 번째는 Optimal MAP Algorithm어］바탕을 두고 있는 시gorithm이다. 八/IAP
Algorithm은 information bits의a 1刃steriori probabilities를 계산하여 이 확률이
최대가 되도록 복호화를 한다. MAP algorithm은 Cony아utional코드어］ 사용하면
성능이 우수하지만 계산량이 많아서 1974년 발표퇸 이후, 실저］ 시스템에서 쓰인 적
은 거의 없었다. 그러다가 Turbo Co扼가 제안되면서 새롭게 주목을 받으며 계산량
    7. 日ad山 Transmiss山n Technique                                                           377
1


을 줄이기 위한 연구들이 많이 이루어지고 있다．
    두 번째는 Viterbi Algorithm에 바탕을 툰 Algorithm이다. 기존의 Viterbi
Algorithm을 적용하여 얻을 수 있는 h카d-d凹始幻n을 적용한 값어］ 신뢰성값을 더 겨］
산하여 성능을 개선시키는 Soft-O毗put Viterbi Algorithm(SOVA), 하나의 八IL
Sequence만 찾는 것이 아니라 여러 개의 Paths를 찾아내는 List Viterbi
Algorithm(LVA) 등이 그 예이다. 이런 Algorithm들은 Sub-Optim出이고 Optin追1
MAP Algorithm어］ 비하면 성능이 떨어지지만 계산량이 적다는 장점이 있다．


           회기 적  길쌈
           부호화 가
                                                           x        >
                           ,,＼부宣화7卜．J
                                                      Yn            尸   심벌
                            dO})=13 D-+ iy,i                            천공과
                            fic趾） .)=l+ D十ly三；                  1
                                                  3                     반복
                                                      Y9
                            fl i(IY4= 1 * r\ 4 ri                                   코드 심벌
                                                                              H1卜    출력
                               부호화기 2                 x'        1
                                                      Y
                                                           l'   1
                            dW)=1 十 L)2+ LY
                            nn(D)=1+ D- I)            Y7'
                            n1(D) '1+ r)+ r2+ ul


                        （그림 石12) IS-950의 Turbo Code



    이러한 Turbo Code를 사용하여 Shannon 극한어］ 근접하기 위한 성능의 핵심이
되는 것은Coi짜ol毗ional 부호화기의 회기척인 구조와 Interleaver의 사용에 있다．
 （그림 7-12）는 실지로 IS中％C에서 사용하고 있는 터보 부호화기이다．
    여기에서는 1/2, 1/3, 1/4 등과 갇은 3가지의 부호화 율을 제공하는데 이러한
부호화 율을 천공 방식 등을 이용하여 부호화기의 입력을 척정한 혹은 설정퇸
코드율어］ 부합되게 출력을 조정한다. 이러한 것을 직접 보여주는 것은 다음의 표
7-2이다.
    표 7-2에서 알 수 있듯이 각각의 코드율을 맞추기 위해서 6개의 출력 중 2개를
선택하든지 혹은 3개를 선택하든지 그것도 아니면 4개를 선택하는 방법으로 그것의
코드율을 조정한다. 여기에서 0은 해당 Bit를 없애는 것이고 1은 통과시키는 것을
의미한다．
                                      7. 日ad山 Transn기ss山n Technique
    378                                                               .


                       （표 7-2）》 데이터 帥의 천공형태
                                      코드율
       츌력                1/   2        1/   3             三／   4
          x               11              11               11
          Y1             10               11               11
          y2              00              00               10
          x2              00              00               00
          Y1
                          01            11                 01
          Y,2             00              00               11




  7.2 Interleaving

 Block Interleavir垠은 무선 경로상에서 나타나기 쉬우며, 여러 Bit에서 연속적으
로 뭉쳐서 발생하는 연집（burst）한 오류를 막기 위하여 데이터를 일정한 규칙어］ 따
라 분산시키는 방법이다. 산발오류어］ 대처하기 위하여 Convolutional 부호화기를
거친 동기채널과 호출채널 그리고 통화채널은 （力de Symbol을 수행한 후에 다시
연집오류어］ 대처하기 위하여 Block Interleavii坦을 수행한다．
 동기채널의 변조심벌 속도는 4800sps이고 1 Frame에는 128개의 변조심벌이 존
재하므로 Frame의 길이가 128/4800=O.02667=26.67ms가 된다. 짜ock Interleaving
은 Frame         단위로   이루어지므로      통화채널은        2伍ns로   동기채널의       Bkx永
Interleavii培의 길이는 26.67ms가 된다. （표 7-3）어］ 심벌을 2.4ks1冷인 Code
Symbol 64개(1餌）로부터 Code Symbol 반복어］ 의하1 생성퇸 128개의 심벌율
4.8ksps인 변조심벌들로 구성된 Frame의 구성을 나타내었다.
 이 Frame의 변조심벌들은 왼쪽 열부터 차례로 위에서부터 아래로 그리고 그 다
음 열의 순서로 Block Interleaver어］ 입력된다. Block Interleaver는 각 변조심벌들
의 순서를 바꾸는 역할을 하는데, 동기채널의 경우에는 입력된 Frame의 1열 1, 3,
5, 7행의 변조심벌（심벌 1,2, 3, 4）을 순서를 바꾸어 （심벌 1, 3, 2, 4) 1행 1, 2, 3,
4열어］ 배열하고, 1열 2, 4, 6, 8행의 변조심벌（심벌 1, 2, 3, 4）을 순서 바꾸어（심벌
1, 3, 2, 4) 1행 5, 6, 7, 8열에 배열한다.
    7. Radio Transmission Technique                            379
.

                     （표 下3) 동기채널 Interleaver 입력 다ame
     1         9         17           25   33    41     49       57
     1         9         17           25   33    41     49       57
     2         10        18           26   34    42     50       58
     2         10        18           26   34    42     50       58
     3         11        19           27   35    43     51       59
     3         11        19           27   ：斐)   43     51       59
     4         12        20           28   36    44     52       60
     4         12        20           28   36    44     52       60
     5         13        21           29   37    45     53       61
     5         13        21           29   37    45     53       61
     6         14        22           30   38    46     54       62
     6         14        22           30   38    46     54       62
     7         15        26           31   39    47     55       63
     7         15        26           31   39    47     55       63
     8         16        24           32   40    48     56       64
     8         16        24           32    40   48     反；       64


    이러한 순서 재배치 규격으로 5, 3, 7, 2, 6, 4열의 변조심벌들을 각각 2, 3, 4, 5,
6, 7, 8행으로 배열한다. 그 다음에는 다시 1, 5, 3, 7, 2, 6, 9, 10, 11, 12, 13, 14, 15,
16행으로 배열한다. 이렇게 순서가 바뀌어서 배열된（Interleaving된） Block
Interleaver의 출력 Frame의 구성을 ＜표 7-4）어］ 나타내었다. 미ock Interleaver어］
의해서 순서를 바꾸는 이유는 연속된 변조심벌들어］ 의해 연집오류가 발생하더라도
수신기에서 Bk乂k Interleaver를 사용하여 원래의 배열순서로 복원하면 연집오류가
산발오류로 바뀌게 되어 Coi싸oh也onal부호의 복호기（일반적으로 \Titerbi 복호기）
에서 오류를 정정할 수 있기 때문이다．
    호출채널과 통화채널의 변조심벌 속도는 19.2ks1羚이고, iFran妃에는 384개의 변
조심벌이 존재하므로 Frame의 길이는 384/19.2k=20ms가 된다. 따라서 호출채널과
통화채널의 Block Interleaver의 길이는 20ms가 된다. 그러나 16XX8크기의 128변
조 심벌틀로 구성되는 동기채널의 Block Interleaver Frame과는 달리 호출채널과
통화채널의 미ock Interleaver Frame은 24X 16크기의 384 변조심벌들로 구성된다．
변조심벌들의 순서를 재배열하는 Block Interleaving 과정은 동기채널의 Block
Interlea叭ng과 유사하며, 동기채널에서 8변조 심벌 단위로 순서를 재배열하는 것이
호출채널과 통화채널의 경우에는 16 변조심벌 단위로 이루어진다.
      380                                                          7. 日ad山 Transmiss山n Technique
                                                                                                                   1


                           （표 刀4) 동기채널 Interleaver 출력 다ame

   1              3              2             4              1              3              2             4
   33         35             34                36             33             35             34            36
   17         19             18                20             17             19             18            20
   49         51             50                52             49             51             50            52
   9          11             10                12             9              11             10            12
   41         43             42                44             41             43             42            44
   25         27             26                28             25             24             26            28
   57         59             弱                 旼）             57             59             58            60
   5              7              6             8              5              7              6             8
   37         39             38                40             37             39             38            40
   21         23             22                24             21             23             22            24
   53         55             54                攷；             53             55             54            닸；
   13         15             14                16             13             15             14            16
   45         47             46                48             45             47             46            48
   29         31             30                32             29             31             30            32
   61         63             62                64             61             63             62            64


 Reverse 링크에서는 액세스 채널과 통화채널 모두 Code Sy且由아 반복을 거친 후
어］ 28.8k町月의 심볼율을 가진 （力de Symbol이 되고, 이 · 심벌들이 미ock
Interleaver어］ 입력된다. Access 채널과 통화채널은 모 三 Frame 킬이가 20ms이므
로 Block Interleaver Frame은 20X28.8=575개의 변조 심벌들로 구성된다．
 B뇨：k Interleaver의 입력 메모리는 32행 8열의 크기로 구성되며, Forw可d 링크
의 경우와 같이 왼쪽 열부터 차려泣 위에서부터 아래로 그리고 그 다음 열의 순서
로, 즉 1열부터 시작하써 1행, 2행, ··· 순서로 입력된다. 그러나 Block Interleaver
의 출력 메모리는 입력Frame의 1열을 구성하는 32행 단위로 다음과 같이 순서를
바꾸어서 각 행을 구성하고 1행부터 시작하여 1열, 2열, ··· 순서로 변조심벌을 출력
한다．

  · 통화채널의 Full ra伯인 경우

 1      2    3        4     5        6    7         8    9         10   11        12   13       14   15       16
 17     18   19       20    21       22   23        24   25        26   27        28   29       30   31       32
U
    7. Radio Transmission Technique
                                                                           38： 크
    · 통화채널의 Half rate인 경우

    1    3    2    4    5    7    6    8    9    11   10   12   13   15   14   16
    17   19   18   20   21   23   22   24   25   29   26   30   27   31   28   32


    · 통화채널의 1/4 rate인 경우

    1    5    2    6    3    7    4    8    9    13   10   14   11   15   12   16
    17   21   18   22   19   23   20   24   25   29   26   30   27   31   28   32


    · 통화채널의 1/8 rate인 경우

    1    9    2    10   3    11   4    12   5    13   6    14   7    15   8    16
    17   25   18   26   19   27   20   28   21   29   22   30   23   31   28   32


    ·Access 채널인 경우

    1    17   9    25   5    21   13   29   3    19   11   27   7    23   15   31
    2    18   10   26   6    22   14   30   4    20   12   28   8    24   16   32


        7.2.1 데이터 스크램블링

 데이터 스크램블링은 호출채널과 Forward 통화채널에만 해당되며, 각 개인에게
부여된 Long Code를 이용하여 데이터를 랜덤화함으로써 개인의 정보를 보호하는
역할을 수행한다. 데이터 스크램블링은 Block Interleaver의 출력 변조심벌과 Long
Code PN 칩을 2진 덧셈함으로써 수행된다. 여기서 사용되는 스크램블링용 코드는
각 채널의 \Vaish Code어］ 대응하는 Long Code 八4ask로부터 칩률 1,2288入1cps인
Long Code를 발생시킨 후 이 코드를 다시 주파수 감소기（decima加r）로 19.2ksps
로 감소한 코드이다. 이때 1.2288 x 103/19.2=64이므로 매 64ch如중에서 첫 번째 출
력만이 데이터 스크램블링어］ 사용퇸다．



    7.3 卜加dulation                                                                  )
 일반적으로 변조라 함은 전송할 데이터를 전송을 위해서 처리를 해주는 과정이라
고 한다. 이때 기저대역의 신호를 RF대역으로 그야말로 변조하1 주는 과정을 포함한
    3E2                             7. Rad山 Transn기ss山n Technique
                                                                    U


다. 이러한 변조는 신호의 변화되어짐을 신호의 진폭, 주파수, 위상어］ 대응시켜서 새
로운 신호를 만들어낸다. 이것은 우리가 전통적으로 임의의 신호를 진폭, 주파수, 위
상의 함수로 표현하고 사용하고 있기 때문이다．
 이러한 변조는 크게는 아날로그 변조와 디지털 변조로 나누어진다. 이러한 2가지
변조 방식의 차이를 생각하1 볼 때 필자는 그것들의 이름에서부터 차이를 찾고자 한
다. 아날로그 변조의 이름들은 주로 帥4(Amplitude 八4odiilation), F八4(Frequency
入4odulation), PM(Phase 入4odul砒ion）와 같이 M以加lation이라고 하고, 디지털 변조
의 경우 그 이름들은 ASK(Amplitude Shift Keying), FSK(Fr凹uency Shift
Keying), PSK(Phase Shift Keying）과 같이 Shift Keyir垠이라는 방식을 사용한다．
 즉 디지털 변조의 경우 신호 그 자체를 변조하는 것이 아니라 신호를 몇 가지의
이를테면 0과1의 조합, 설정된 진폭, 주파수, 위상 등의 신호로 mapping시키는, 즉
천이방식을 사용한다는 것이다. 다시 말하면 아날로그 변조의 경우 피변조파 자체
를 변조하는 것이나 디지털 변조는 피변조파의 의미를 전달한다고 할 수 있다. 좀더
직관적인 예를 들면 화장실의 예를 들겠다．
 우리가 화장실어］ 가서 노크를 하고 상대가 다시 노크로 응대하는 것은 노크어］ 다
음과 갇은 의미가 포함되어 있다. 즉 첫 번째 노크는 화장실어］ " 누가 들어 있어요2"
라는 질문이고 상대방이 응답하는 노크는 " 여］, 들어있어요"라는 말의 의미전달 방
식이다. 여기에서는 IS-95 RTT에서 사용되고있는 변조 방식인 디지털 변조들어］
대한 이야기만 하겠다. 이에 앞서서 천이변조어］ 대한 이야기를 추가로 좀더 진행해
보기로 한다．


   7.3.1 디지털 쳔이 변조

 디지털 통신에서는 디지털 정보를 n上로 표현하며, m1는 0과 1로 구성된 2진 시퀀
스가 된다. 이 2진 시퀀스는 각 Bit가 (0, T) 구간 동안 특정한 PCM 파형으로 변환
된 뒤 디지털 정보신호 IIMt)가 된다. 이 과정을 기저대역 변조라고 부른다．
 통과대역에서 디지털 변조는 "0" 또는 "1" 어］ 해당하는 기저대역 신호가 정현 반송
파의 성질을 변환시키는 것으로 이렇게 시간구간 T초 동안어］ 기저대역 신호어］ 의
해 변조된 정현파를 통과대역 디지털 심벌이라고 한다. 즉 각 2진 데이터에서 "0"은
So(t）의 파형으로, "1"은 S1(t）의 파형으로 변환되어 전송된다. 이러한 변조방식을 2
진 변조방식이라고 한다.
    7. Radio Transmission Technique
.

    한편 각 Bit어］ 대응한 PCM파형을 만드는 대신 정보 Bit열을 k Bit로 구성된
Block 을 한 단위로 하여 기저대역 신호를 만든다면, M=2k개의 기저대역 신호가
존재하게 된다. 따라서 이 경우에는 八4개의 기저대역 신호가 정현 반송파의 성질을
변화시키므로 八4개의 통과대역 디지털 심벌이 존재하게 되는데 이를 八4中a3/ 변조
방식 이라고 한다. 앞서 이야기한 2진 변조방식은 k=1인 경우라고 할 수 있다．


             기 대대 역신호
                          0           2T   3T   4T   5T          t




                                                          m\ \

                (c) PSK
                                 .,',1/,1'.'.\'1J1．人’1
                    （그림 下］3) ASK, FSK, PSK 변조의 파형 비교
                                                                 t




    이러한 변조방식은 각 디지털 정보에 대응되는 入'I개의 파형이 반송파의 진폭, 주
파수, 위상을 변화시키는 것어］ 따라서 ASK, FSI듸 PSK가 있다고 앞서 이야기하였
다. （그림 7-13）은 이러한 변조파형의 예를 보여준다．

     7.3.2 위상천이 변조와 BPSK

    2진 위상천이 변조인 2진 PSK(BPSK* : Binary Phase Shift Keying）는 다음과
같이 진폭과 주파수 모두가 일정한 반송파를 이용하며 그 위상을 2진 전송부호어］
대응시켜 변화시키는 방식인데 부호오율 및 대역폭 효율 양면에 있어서 우수하므로
널리 사용된다．


木 Bi寸Phase 혹은 Binany Phase라고도 하나 어느 것도 틀린 것은 아니라고 생각한다. 의
  미를 정리하면 2개의 위상이든 2진으로 표현되는 위상이든 결국 2가지의 위상으로 Shift
  Keyir培하는 것이기 때문이다．
   384                                                                    7. Radio Transmission Technique
                                                                                                            1


         옥(t) = Acos2可，t                     （부호가 1일때）
         욱(t) = Asin2可，t                 （부호가 0일때）

 일반적인 八4진 위상 천이 변조인 MPSK(M-ary PSK)어］ 대한 수학적인 표현식
은 다음과 같다．


         S,   (t)   ＝片如却小）                       小t\            T,   i=     1,   A,   M              (7-    1)
 식 作1）에서 알 수 있듯이 위상성분 吻（t）는 八/1개의 기저대역 신호에 의해 변조
퇸 八4개의 이산 값을 가지게 되며, 일반적으로 다음의 식과 같이 퇸다．

         . . . 2危                        A   M
         色 (t) =1H
                                                                 =
                                                                                                     (7- 2)
                                     L
                M
                                     J
 여기에서 八4 =2k는 허용되는 위상 상태의 수, k＝위상 상태 M을 지정하는데 필요한
데이터의 Bit수이다. 디지털 통신 시스템에서는 일반적으로 八/1=2일 때의 BPSK나
八/1=4인 QPSK가 많이 사용된다. 이들어］ 대한 위상 상태도는 （그림 7-14）와 같다．
 MPSK신호를 벡터상의 점으로 표현하기 위하여 cos 0를 가로축으로 sin0를
세로축으로 설정하여 표현한다. 이 두 가지 coordinator에 의해서 생성되는 2차원평
면은 0의 값이 자유롭게 변할 수 있는 0의 평면이 된다. 이 두 축은 서로 직교하므
로 흔히 가로축을 동위상（In叫Phase), 세로축을 직교위상（Quadrature-Phase）으로
부르기도 한다. MI冬K신호를 벡터상의 점으로 표현하기 위해서는 八/1개의 직교축이
필요하나 1M任冬K신호는 단지 두 대의 직교 축만을 사용하므로 여러 가지의 장점과
단점을 동시어］ 가지고 있다．
                             BPSK                        QPSK                             BPSK




                    M = 2'                             M = 22                         M = 23
                    심벌률 = I之                           심벌률 == 1t                      심벌률 = 1之
                    비트율 = R                            비트율 = 2R                       비트율 = 3R

                                    （그림 工］4) 다양한 PSK의 위상 표시
    7. Rad向 Transmiss向n Technique
1                                          1   385켜1

 （그림 7-14）어써 보듯이 MP町（ 신호는 두 축으로 구성되는 2차원 평면에서 크기
가 일정한 원을 따라서 위상만 다른 점들로 표현된다. 따라서 신호간의 위상 차이는
BPSK인 경우 180도, QPSK는 얹）도가 됨을 알 수 있다. 특히 QPSK는 2개의
BPSK를 각각 I, Q축에 실어보내는 것과 유사하다는 것을 알 수 있다．
    여기서 한 가지 주목할 사항은 위상상태의 개수가 증가함어］ 따라서 Bit 율은 증
가하지만 보드율（baud rate）은 그대로 유지된다는 점이다. 그러나 데이터 율어］ 있
어서 이러한 증가는 어떤 대가를 요구하게 된다. 즉 갇은 BER(Bit Error Rate）을
유지하기 위해서는 SNR의 증가가 요구되기 때문이다．
    또한 만약 어떤 정보가 일정한 시간구간 내에서 전송되려고 한다면 l＼乍ary 시스
템에서는 심벌률이 인자 k 만큼 감소됨을 알 수 있다. 필요한 채널 대역폭은 심벌률
어］ 비례한다. 따라서 심벌률의 감소는 보다 적은 대역폭을 사용할 수 있다는 것올
의미한다. 또 다른 관점에서 본다면 심벌률이 고정될 때 고차 시스템은 주어진 대역
폭을 통해서 더 많은 정보 Bit를 제공할 수 있음을 나타낸다．
    그러한 이유로 入4-ary시스템은 주파수 효율이 좋다고 이야기한다. 하지만 그어］
대한 대가가 있으니 바로 에러 확률이다. 그것은 앞의 （그림 7-14）에서 알 수 있듯
이 고차 시스템이 될수록 신호간의 거리가 작아지는 것을 확인할 수 있으며, 이것은
또 다른 측면에서 고차 시스템이 그것보다 차수가 낮은 시스템과 동일한 에러 성능
을 위해서는 전력이 증가해야 된다는 것도 알 수 있을 것이다. 이렇듯 변조 시스템
은 주파수 효율, 에러 확률, 전력 등의 문제가 서로 물고 물리는 trade off로 설명될
수 있고 우리가 필요한 것이 무엇인가를 찾아서 상태적으로 필요 없는 부분과 trade
off함으로 얻고자 하는 성눙을 얻을 수 있을 것이다.
    BPSK방식이 입력한 Bit마다 하나의 신호가 전송되는데 비해서 QPSK방식은 입
력 두 Bit마다 하나의 신호로 전송된다. 따라서 QPSK신호의 전송대역폭은 BPSK
의 1/2이다. 즉 QPSK가 BPSK보다 2배 주파수 효율이 높다.
    이 장에서 이야기하고자 하는 IS-95에서는 Forw카d에서 BPSK방식과 QPSK방
식을 혼합한 방식을 사용하고 있다. 이로 인해서 흔히 IS-95의 RTT의 도면상에서
독자들은 BPSK/QPSK라고 쓰여진 것을 볼 수 있을 것이다. 이것어］ 대한 이야기어］
앞서서 QPSK의 전송방식어］ 대해서 좀더 이야기를 하겠다．
   386                                                  7. 日ad山 Transmiss向n Technique
                                                                                        .


  7.3.3 QPSK(Quadrature Phase Shift Keying)

 QPSK는 먼저 직／병렬 변환기어］ 의해서 홀수 번째 Bit들은 I 채널로, 짝수 번째
Bit들은 Q 채널로 보내지고 각 채널에서는 레벨 변환기어］ 의해 "0" Bit는 1로
"1"Bit는 1로 치환된다．




                            （그림 石］5) QPSK 블록도


 이때 직／병렬 변환기의 입력신호는 Bit율이 1! Tb[bps］이므로 한 Bit의 시간구간
은 Tb[sec］가 되며, 직／병렬 변환기의 출력신호는 심벌률이 1/2로 되므로 한 심벌의
시간구간은 t[ sec］가 되므로 乙= 2乙인 관계가 있다. 즉 심벌구간은 Bit구간의 2
배가 된다． 레벨 변환된 I 채널신호를 cos 回d와 곱하고, Q 채널신호를 sin a) t와
곱한 후 다음 두 신호를 합하여 전송하면 QPSK변조퇸 신호가 된다．


                    1       1   0   1   1       0   0       0   1       1   1       0

           입력신호




            I 채널        1                   l           0           1           1




                        l                   0           0           l




                    （그림 工16) : QPSK 변조신호
     7. Rad向 Transn기ss山n Technique
.


    （그림 7-16）은 QPSK변조기의 미ock 도와 （그림 7-16）은 임의의 입력신호어］ 대
하여 1/Q채널신호로 직／병렬 변환된 신호를 보여준다．
    위의 （그림 7-16）에서 /(t)는 +1 ‘또는 1 이므로 I (t)cos 口巾는 결국 심벌구간이
Ts[sec］인 심벌 m）에 의해서 BPSK 변조퇸 신호와 같다. 또한 Q（加in w0t도
Q(t）가 sin w弘를 BPS}( 변조한 것과 같으므로 QPSIE( 변조된 신호는 변조된 신호
는 다음의 식과 같이 /(t)와 Q(t)가 2개의 직교 반송파를 변조하여 합한 것과 같다．

           S(t) = I (t)cosw。           z'
                           t - Q(t)sinw。                                                      (7-3)

    이 QPSK 변조신호는 최종적으로 하나의 sinusoidal 신호로 전송될 것이며, 그것
의 형태는 다음과 같다．

           S(t) = .V' cos[iD。t+ 0(t)]                                                         (7- 4)


    위상성분 0(t)는 /(t)와 Q(t)의 조합어］ 의해서 4가지의 값을 가질 수 있다. 예를
들어서 입력데이터가 '01'인경우 I 채널은 1로 Q채널은 1로 된다. 따라서 변조신호
는 단음의 식과 같이 된다．

                                                                                              (7中5)
           묵（t)    =A   (-    cos   2磁！   -   sin2磁！        )=V三Acos        2磁
                                                                                 『和
                                                                                 『

    이와 같이 계산하면 서로 다른 4가지의경우의 입력 쌍（00, 01, 10, 11）은 4개의 가
능한 정현파 위상 중 하나와 대응된다. 입력 Bit와 출력신호와의 관계는 각각
(0.75 it, 0.75 it, -0.25 it, 0.25 力이다. 다음의 표는 QPSK의 위상 mappii垠을 정리
한 것이다．


                             （표 石5) QPSK 계열의 I, 0채널 위상 Mapping
               i                                       1尸              （그             Phase

              0                                                        0               兀／4
              1                                                        0              3 兀／4
              1                                                        1               /4
              0                                                        1                兀／4
                                                             7. Radio Transmission Technique
                                                                                               1


  7.3.4 OQPSK(Offset Quadrature Phase Shift Keying)

 QPSK방식에서는 변조신호 사이의 최대 위상변화가 180도인 경우가 발생한다．
이렇게 갑자기 위상이 변하는 신호는 대역 제한된 채널을 통과할 때 왜곡이 발생된
다. 이와 같이 변조신호의 급격한 위상천이를 줄이기 위해서 QPSK의 변조과정어］
서 Q채널의 신호어］ Tb만큼의 시간지연佃ifset）을 시켜 변조 신호간 최태 위상천이
를 90도로 줄인 방식이 offset QPSK 또는 OQPSI( 방식이다．




                         （그림 7-17) OQPSK의 블록도


 （그림 7-17）에서 알 수 있듯이 OQPSK 방식은 변조 신호간의 최대 위상변화가
90도로 줄어튼다. 이러한 OQPSI( 방식은 Reverse 링크어］ 사용된다．


                 0       1   1       1   0       0   1        0   (1       1   1       0




                     1           l           0           l             0           l




                                                                                           0

                 Tb 켜1

                         （그림 7-18) OQPSK 변조신호
    7. Radio Transmission Technique                                                       389   1
U


 이러한 OQPSK의 I와 Q 채널의 매핑은 QPSK와 동일하나 위상천이는 （그림
下19）와 같이 차이가 난다. 이러한 위상천이는 변조 후 발생되는 Side lobe의 변화
를 가져온다．

        QPSK                   Q                    (I,Q)   OQPSK          Q


         (1.0() 紮小二
                r / (0,0) '"""
                    \   '\,\




                               \\
                                    '也           ,, , ,                        0.   1)

                                                                               Zero Crossin只
                                                                                윽 하지않음


                                                （그림 下］9) 위상천이도


     7.3.5 IS-95의 변조

 IS앉)에서 사용하는 변조방식은 BPSK와 QPSK계열의 OQPSK를 사용한다．
Forward어꺼 사용하는 BPSK방식은 그것의 형상이 QPSK와 동일한 형상으로 인
해서 QPSK로 생각되어지기도 하는데, QPSK가 4상 신호를 가지고 전송된다는 측
면에서 볼 때 이 방식은 QPSK라기보다는 BPSK를 2개 합해 놓은 형태이다. 즉
BPSK 신호가 2가지의 경로로 속도가 전혀 감소되어지지 않는 환경에서 전송되며，
때문어］ BPSI叫 비해서 상대적으로 유리하게 작용되었던 QPSK의 스펙트럼 효율
이 향상되지는 않는다．


      정상적인 QPSK인 경우는 입
      력신호가 각각의 채널로 할
                                     ' 1.2888Mc
                                      卜，
                                           ,,



      당될 때 속도가 나누어서 할                                       태벨 변환
      당되므로 I. Q채널의 속도가
      입력신호의 절반이다．


                           Input(t)                                                      S(t)
                1. 2288Mcps




                                           1.228$Mcps               客   Q(t)

                                    （그림 万20) Fo八yard의 QPSKIBPSK
                                   7. Rad山 Transn기ss山n Technique
   390                                                             U



 이상과 같은 이유로 인해서 Is寸95의 Forw町d 링크의 변조 방식은 BPSK/QPSK
라고 표시하는 문서나 논문 등을 우리는 볼 수 있다. Reverse의 경우 앞서 설명한
OQPSK를 사용하여 Non Coherent Detection을 수행하는 방식을 사용한다．
 이러한 변조 방식들은 다중접속 방식 및 다중화 방식이 코드 D如始幻n이라는 관
점에서 볼 Iqi 에러 확률을 최소화할 수 있는 효과적인 방법들로 생각될 수 있으며，
이것은 CDMA의 I노ocessing Gain을 얻기에 충분한 에러 확률을 가질 수 있는 변
조 방식일 것이다．
 최근어］ 이야기거리가 되고 있는 HDR의 경우는 이러한 관점과는 조금 거리가 있
으며, 때문어］ 변조방식의 선정도 스펙트럼 효율이 높은 QAM 방식 등이 사용되고
있다. 조금 다른 관점에서 볼 때 우리는 CDMA시스템에서 이루어지는 변조를 형태
가 아니라 기능상으로 확인해 보고자 한다.


 Long Code 변조

 Reverse 통화채널과 /\ccess 채널은 긴 코드어］ 의한 직접 계열확산이 적용퇸다．
Reverse 통화채널어］ 대해서 이 확산동작은 데이터 버스트 랜덤화기에서 발생퇸 출
력신호와 긴 코드 八4odulo-2연산이다. Access 채널어］ 대해서는 64-ary 직교변조
출력열과 긴 코드의 八'Iodu1o-2 연산이 퇸다. 이 긴 코드는 2乙1칩의 주기를 가지고
있으며 다음 특성 다항식어］ 의해 규정퇸 선형 순환을 만족한다．

         P（功 = 寸 ＋工35 ＋工弱 ＋工引＋工刃＋尸＋少＋寸＋尸＋工19 ＋工18 ·
               ＋工16＋工10＋工7 ＋工6＋兀5＋工3＋工2＋工 +1                 (7- 6)



  긴 코드의 PN 칩들은 시퀀스 발생기의 42 Bit 마스크와 42 Bit 상태 벡터의
入4odulo그 내적에 의해 생성퇸다．


  획산 변조 - PN Short Code 변조

 확산 변조라는 것은 입력되는 데이터를 CDMA의 전송 대역폭인 1.2288Mcps로
변화시켜주는 변조로 이때는 입력 데이터어］ 입력 데이터보다 훨씬 빠른 변조파를
곱해서 이러한 절차가 이루어진다. 일반적으로 변조라고 하면 수학적으로 해석할
때 시간 영역에서 곱하기 연산의 결과라는 이야기는 앞서 이야기되었다. 이러한 곱
하기의 패턴은 단순히 주파수 대역이 shift되는 결과를 나타내기도 했지만, 대역 자
.
    7. Radio Transmission Technique                 391
                                                          I
체가 확산되는 경우도 확인하였다. 자세한 사항은 앞의 3장을 다시 공부해 보라！
    여기어］ 사용되는 확산용 코드는 It卜phase와 Quad岫te 성분의 PN Short Code가
있다. 이러한 코드의 다항식은 다음과 같다．

          P1 ＝工巧＋寸＋尸 + xg +r ＋工5 +l

          e＝工" +x'2 +xt'＋工'" ＋工6＋寸＋工" ＋工3+l
    위의 식어］ 의해서 발생되는 최장 길이 코드는 LSFR(Linear Shift Feedback
Register）에 의해서 발생되며（3장 참고!), 이것은 실지로 다음과 같은 선형 순환식
으로 나타난다．
    이 PN Short Code 변조는 Forw可d일 때는 PN offset을 가지는 기지국의 신호
임을 나타내고 Reverse일 때는 해당 Pilot의 기지국으로 /\ccess한다는 의미이다．
이 short는 QCDMA의 모드 기지국에서 동일한 값으로 사용되며, 이 값의 옵셋으
로 기지국을 식별함으로 정확한 시간정보가 필요할 것이며, 때문어］ 동기식 CDMA
라고 불리운다. 반면 비동기식 CDMA는 이러한 시간정보가 필요없는 것으로 이러
한 각각의 기지국식별코드를 별도의 코드로 만들어서（별도의 ASIC) 변조하는 방식
으로 이 방식은 특별한 옵셋이 식별자가 아니므로 시간정보가 전혀 필요없다．
    이상과 같은 내용들을 정리할 때 확산 변조가 이루어지는 것은 기본 출력 데이터
가 고속의 전송 데이터 율로 바뀌게 되는 시점이 확산이 이루어지는 시점이라고 볼
수 있으며, 일반적으로 이러한 chip rate을 가지는 것은 PN Short Code이다．


    Orthogonal 변조 -w키sh 변조
    IS-95시스템에서도 다중화를 위한 채널 형성이 이루어져야 할 것이며, 이러한 채
널을 형성하는 형성인자는 주파수나 시간이 아닌 코드가 되는 것이다. 이러한 코드
는 서로간어］ Correlation 성질이 우수하햐 하며, 이러한 우수한 상관성을 가지는
orthogonal한 코드를 사용한다. 만약어］ 이러한 코드의 상관성이 불량하다면 각각의
코드들의 구별성은 떨어지며, 각각의 코드들의 입장에서는 상호간어］ 간섭이 될 것
이다．
    이러한 직교성을 가지는 코드를 직교코드라고 하며, 이러한 직교코드는 \Va1sh
（노de로 알려진 코드들을 사용한다. 이러한 \Valsh C力de를 곱함으로, 즉 변조함으
로 신호는 玖Taish 채널어］ 실려서 전송되게 되는 것이다. 더불어 서로 다른 \U싫sh
       392                                                                                 7. Radio Transmission Technique
                                                                                                                                                          .


Code 인텍스를 사용한다면 또 다른 채널이 될 것이다. W出sh Code어］ 관한 내용 등
은 3장을 참고하라．


     Walsh Array 변조

     여기에서 행해지는 ＼入／aish 변조는 앞서 이야기한 직교변조와는 그것의 성격과 구
성은 완전히 다르다. 이것은 Reverse어］ 사용되는 변조 방식 혹은 코딩 방식이라고
할 수 있다. Reverse CDIVIA 채널에서의 변조는 64可y 직교변조를 사용한다. 각
6개의 반복퇸 Code Symb아어］ 대해 64개의 가능한 변조심벌 중 하나가 전송된다．
변조심벌은 Walsh 함수를 이용해서 생성되는 64개의 상호 직교인 파형 중어］ 하나
이다. 이런 변조심벌은 （표 7-6泣｝같고 아63까지 번호가 부여되어있다. 변조심벌
의 선택은 다음 수식어］ 의해서 이루어진다．
     변조심벌 참조번호＝ c0+ 2c1+ 4c2+8c3+ 16c4+32c5
     여기에서 C5는 변조심벌을 구성하는 6개의 반복퇸 Code Syi工由아 중 마지막어］ 발
생된 반복（沁de Syr的ol이고 Co는 처음에 발생된 반복Code Syff由01로 이진 값이다．


                                                     （표 下6> 64진 직교심벌 집합

                                                      Walsh Ch巾 小／仕hin Symb이
                    t i l t
     0123 4567 99。1 2345 67n                         計弱 詐計 託計 芥北 詐詐 計災 災計 喆計 詐詐 計詐 計芥
0    0000    0000      0000      0000      0000      0000      0000      0000      0000    0000      0000      0000      0000      0000      0000      0000
1    0101    0101      0101      0101      0101      0101      0101      0101      0101    0101      0101      0101      0101      0101      0101      0101
2    001 1   001 1     001 1     001 1     001 1     001 1     001 I     001 1     001 1   001 1     001 1     001 1     001 1     001 1     001 1     001 1
3    01 10   01 10     01 10     0t to     0t to     01 10     Ot t0     01 10     0t t0   0i ls     01 10     01 10     01 10     01 10     01 10     01 10

4    0000    l i i i   0000      t i l l   0000      11 1 1    0000      t i l t   0000    1 1 11    0000      1 1 11    0000      1 1 1 1   0000      l i i i
5    0101    1010      0101      1010      0101      1010      0101      1010      0101    1010      0101      1010      0101      1010      0101      1010
6    001 1   1 100     001 1     1 100     001 1     1 100     001 1     1 100     001 1   1 100     001 1     1 100     001 1     1 100     001 1     1 100
7    01 10   1001      01 10     loot      0t t0     toot      01 10     tool      01 10   loot      01 10     1001      01 10     loot      01 10     tool

8    0000    0000      1 1 1 1   l i l t   0000      0000      l i l t   t i l l   0000    0000      1 1 1 1   1 1 ] ]   0000      0000      l i l t   1 1 1 1
9    0101    0101      1010      1010      0101      0101      lob 0     1010      0101    0101      1010      1010      0101      0101      1010      1010
10   001 1   001 1     1 100     1 100     COl t     001 1     1 100     1 100     001 1   001 1     1 100     1 100     001 1     001 1     1 100     1 100
it   01 10   0t to     tool      tool      01 10     0t to     1001      tool      01 10   0t to     1001      1001      01 10     01 10     1001      lOOt

12   0000    1 1 1 1   1 1 1 1   0000      0000      l i l t   l i l t   0000      0000    111 1     1 1 i t   0000      0000      l i l t ] 1 1 1     0000
13   0101    1010      1010      0101      0101      1010      1010      0101      otol    tots      iota      0101      0101      1010 1010           0101
14   001 1   1 100     1 100     001 1     001 1     1 100     1 100     oot t     001 1   i t 00    1 100     001 1     001 1     1 100 1 100         001 1
to   0t to   loot      1001      01 10     0t to     tool      tool      Ot to     0t to   tool      tool      01 10     0t to     1 001 tOOl          0t is

16   0000    0000      0000      0000      l i t 1   1 1 1 1   l i l t   t i l l   0000    0000      0000      0000      1 1 1 1   111 1     l i i i   1 1 1 1
17   0101    Clot      0101      0101      lots      1010      1010      1010      0101    0101      0101      0101      1010      1010      1010      1010
18   00i 1   001 1     001 1     001 1     1 100     l iO0     1 100     t too     001 1   001 1     001 1     001 1     1 100     1 100     1 100     1 100
19   01 10   01 10     01 10     01 10     toot      1001      tool      tool      0t to   0t to     01 10     SI l0     tOOl      lOOt      1001      toot

20   0000    i t t ]   0000      1 1 1 1   t I l l   0000      t i l t   0000      0000    1 1 1 1   0000      1 1 1 1   1 1 1 1   0000      1 1 1 1   0000
21   0101    toto      0101      lots      tots      0101      1010      0101      0101    1010      0101      tots      1010      0101      1010      0101
쏘    001 1   1 100     001 1     1 too     1 100     001 1     1 too     001 1     001 1   1 100     001 1     1 100     1 100     001 1     1 100     001 1
四    01 10   loot      0t to     loot      toot      0t 10     loOt      0t to     0t to   loot      0t to     1001      1001      01 10     tOOl      01 10

24   0000    0000      t i l l   l i l t   1 1 1 1   t i l l   0000      0000      0000    0000      t i l l   l i t 1   1 1 1 1   I l l 1   0000      00 00
25   0101    0101      1010      1010      1010      1010      0101      0101      0101    0101      1010      1010      1010      1010      0 ] 0 1   0 ] 0 ]
茹    001 1   001 1     ] tO0     1 100     1 100     1 100     001 1     001 1     001 1   001 t     1 100     1 too     1 100     1 100     00 1 1    00 ] ]
27   0t to   01 10     1001      1001      loot      tool      01 10     01 10     0t to   01 10     tool      1001      1001      1 00 1    01 ] 0    0 1 1 0
.
     7. Radio Transmission Technique                                                                                                                M
                                                                                                                                                    m

                                                                                                                                                              I
田    0000    1 111     11 1 1    0000      11 1 1    0000      0000       1 1 1 1   0000      1 1 1 1   1 1 1 1   0000      1 11 1    0000      0000      11 1 1
囚    0101    1010      1010      0101      1010      0101      0101       1010      0101      1010      1010      0101      1010      0101      0101      1010
了）   001 1   1 100     1 100     001 1     1 100     001 1     001 1      1 100     001 1     1 100     1 100     001 1     1 100     001 1     001 1     1 100
31   01 10   1001      1001      01 10     1001      01 10     01 10      1001      01 10     1001      loot      01 10     1001      01 10     01 10     1001

끄    0000    0000      0000      0000      0000      0000      0000       0000      1 1 1 1   11 1 1    1 1 1 }   11 1 1    11 1 1    1 1 1 1   1 1 1 1   1 1 1 1
羽    0101    0101      0101      0101      0101      0101      0101       0101      1010      1010      1010      1010      1010      1010      1010      1010
34   001 1   001 1     001 1     001 1     001 1     001 1     001 1      001 1     1 100     1 100     1 too     1 100     1 100     1 100     1 100     1 100
35   01 10   01 10     01 10     01 10     01 10     01 10     01 10      01 10     1001      1001      1001      1001      tool      1001      1001      1001

弱    0000    1 1 1 ]   0000      1 1 1 1   0000      1 1 1 1   0000       11 1 1    1 1 11    0000      1 1 1 1   0000      1 1 1 1   0000      1 1 1 1   0000
37   0101    1010      0101      1010      0101      1010      0101       1010      1010      0101      1010      0101      1010      0101      1010      0101
38   001 1   1 100     001 1     1 100     001 1     1 100     001 1      1 100     1 100     001 1     1 100     001 1     1 100     001 1     1 100     001 1
羽    01 10   1001      01 10     1001      01 10     1001      01 10      1001      1001      01 10     1001      0t to     1001      01 10     1001      01 10

40   0000    0000      1 1 1 1   l i l t   0000      0000      11 11      111 1     1 1 1 1   l i i i   0000      0000      l i l t   l i i i   0000      0000
41   0101    0101      1010      1010      0101      0101      1010       1010      1010      1010      0101      0101      1010      1010      0101      0101
42   001 1   001 1     1 100     1 100     001 1     001 1     1 100      1 100     1 100     1 100     001 1     001 1     1 100     1 100     001 1     001 1
43   01 10   01 10     1001      1001      01 10     01 10     tool       1001      1001      1001      01 10     01 10     1001      1001      01 10     01 10

44   0000    1 1 1 1   11 1 1    0000      0000      1 1 1 1   1 1 1 1    0000      1 1 1 1   0000      0000      1 1 1 1   1 1 1 1   0000      0000      1 1 1 1
45   0101    1010      1010      0101      0101      1010      1010       0101      1010      0101      0101      1010      1010      0101      0101      1010
48   001 1   1 100     1 100     001 1     001 1     1 100     1 100      001 1     1 100     001 1     001 1     1 100     1 100     001 1     001 1     1 100
47   01 10   1001      1001      01 10     0t to     1001      tool       01 10     1001      01 10     0t to     1001      1001      01 10     01 10     1001

48   0000    0000      0000      0000      1 1 1 1   11 3 1    1 1 1 1    1 1 11    1 1 1 1   1 1 1 1   1 1 1 1   11 1 1    0000      0000      0000      0000
49   0101    0101      0101      0101      1010      1010      1010       1010      1010      1010      1010      1010      0101      0101      0101      0101
50   001 1   001 1     001 1     001 1     1 100     1 100     1 100      1 100     1 100     1 100     1 100     1 100     001 1     001 1     001 1     001 1
51   01 10   0t to     01 10     01 10     1001      1001      1001       1 001     1001      1001      1001      1001      01 10     01 10     01 10     01 10

고    0000    1 1 1 1   0000      1 1 1 1   l i l t   0000      1 1 1 1    0000      1 11 1    0000      1 1 11    0000      0000      1 11 1    0000      11 1 1
弱    0101    1010      0101      1010      1010      0101      1010       0101      1010      0101      1010      0101      0101      1010      0101      1010
54   001 1   1 100     001 1     1 100     1 100     001 1     1 100      001 1     1 100     001 1     1 100     001 1     001 1     1 100     001 1     1 100
弱    01 10   1001      01 10     1001      1001      01 10     1001       01 10     1001      01 10     1001      01 10     01 10     1001      0t to     1001

弱    0000    0000      1 1 1 1   1 1 1 1   1 1 1 1   1 1 1 1   0000       0000      1 ] 1 1   1 1 1 1   00 00     0000      0000      0000      11 ] 1    1 ] 1 ]
57   0101    0101      1010      1010      1010      1010      0101       0101      1010      101 0     0 ] 01    010l      0101      0 10 ]    1010      10 10
田    001 1   001 1     1 100     1 100     1 100     1 100     001 1      0011      1 100     l 100     001 1     00 ] j    00 1 1    001 1     1 100     1 100
羽    01 10   01 10     1003      1001      1001      1001      01 10      01 10     ] 001     l 001     0 1 10    01 1 0    0 1 10    01 10     1001      1001

苡）   0000    1 1 1 1   1 1 1 1   0000      1 ! 1 1   0000      0 0 (} 0   111 1     11 11     0000      000 0     1 1 l 1   0000      11 ] 1    1 11 1    0000
61   0 101   10 10     1010      010 1     1010      0 ] 0 l   0 1 (} l   1010      1 0 j 0   0 ] 01    0101      1010      0 ] 01    l 010     1010      0101
m    001 1   1 ] 00    1 100     001 1     1 100     001 t     00 1 1     1 100     ] 100     001 ]     0011      1 1 00    001 1     1 100     1 100     0011
因    01 10   1001      1001      01 1 0    1001      0110      01 1 0     100 1     ] 001     0 ] 10    01 10     100 1     0110      100 1     100 1     01 10




     하나의 변조심벌을 전송하는데 필요한 시간주기는 l/ 4800초（208.333... 尸S）이다．
따라서 변조심벌의 l/ 64어］ 해당하는 시간주기는 하나의 \ValSh칩어］ 해당하며，
l/ 307200초（3.255... //S）이다. 하나의 변조심벌 안에는 \ValSh칩들이 0, l , 2, ···, 63
번의 순서로 전송된다．



     7.4 다중 斗와 다중접속                                                                                                                                                 )
     다중접속（N血出de ACCeSS) 방식은 여러 개의 접속 요인들, 즉 단말기들이 하나
의 /\CCeSS망어］ 접속하는 방식을 규정한 방식으로 다중화低lmhm이dng) 와 대비되
는 개념이라 할 수 있다. 즉 다중화란 여러 개의 신호를 각각의 신호를 수신하고자
하는 단말기만이 의미를 부여할 수 있는 식별자를 사용하여 한꺼번어］ 전송하는 방
식을 말하며, 다중접속은 그러한 단말기들이 각각의 신호어］ 구별자를 가지고 망어］
ACCeSS하는 형태를 말한다. 따라서 정확히 우리가 1SH95시스템을 이야기할 때는
   394                              7. Radio Transmission Technique
                                                                      .


CDM/CDMA라는 표기방식을 사용해야 할 것이다. 이러한 표시는 실지로 몇몇 자
료에서 우리는 확인할 수 있다．
 이러한 구별인자가 특정한 코드 혹은 암호로 이루어지는 방식이 Code Div逋이l
방식이다. 이러한 코드는 설정된 시스템에서 사용하는 주파수와 Clock수어］ 부합되
는 신호이며, 단지 신호의 형태가 이러한 코드의 형태 혹은 변량으로 전송되는 것을
말한다. 즉 IS -95의 경우 최장 코드인 PN Code의 형태로 그 코드의 속도를
1.2288MHz로 변경한다는 것이다.



              ！늬   m1
                                     H나
                                      『니

                                      且，
                                     코          나




                                           的蜘
           다중화 그        1i   m
                                                    그



                        （그림 石21) 다중화와 확산



 우리가 흔히 전송되는 신호는 원래 신호의 변화 양상을 우리가 정해 놓은 신호어］
대응시켜 그 신호의 변화분를 채널을 통해서 전송하는데 CDMA의 경우는 그러한
변화의 형태가 정해진 코드의 변화 형태로 전송된다는 관점에서 볼 때 Cl孤'I(Code
I万vision Multiplexing) 방식은 또 다른 변조를, 즉 확산 변조를 수행한다고 볼 수
있다．
 일반적으로 다중화는 각각의 정보 신호들어］ 비해서 상당히 넓은 대역을 가진다．
즉 30KHz의 기저대역의 정보를 10개를 다중화한다면 최소 300KHz의 대역이 필요
할 것이다. 그런데 우리는 3아(Hz의 정보가 300K1七의 대역으로 전송된다고 해서
이것을 확산이라고 하지는 않는다. 이것은 30KHz의 정보 10개가 같이 전송퇸다는
의미에서 그러하다. 그렇다면 우리는 진정한 의미의 확산 스펙트럼의 통신이 이루
어지는 것은 기저대역 신호가 여러 개가 전송되기 위하써 넓은 대역을 사용하는 것
    7. Radio Transmission Technique                                    395
1


이 아니라 하나의 기저대역 신호를 전송할 때 넓은 태역으로 전송하는 것을 확산이
라고 하므로 CI呱4A가 확산통신이라고 이야기할 수 있을 것이다. 만약 그렇지 않다
면 다중화 프로세스 자체가 확산 스펙트럼이라고 이야기해야 하는 오류를 범하게
되는 것이다. 즉 정리하면 CDM은 다중화를 위한 방식이고, CDMA는 확산 스펙트
럼 통신이라고 이야기 할 수 있다．




目        Forward 채널 구조


    IS-95의 채널은 크게 기본 데이터 속도가 앉耿0bps의 Rate Set 1과 14400bps의
                                                                             )



Rate Set 2로 구븐된다. 이러한 속도집합은 각각 상위와 하위의 속도 속성들을 가
지고 있다. RS2의 경우 한국의 PCS에서 초기어］ 이 속도집합을 사용하여 현재 1000
만여 명의 사용자가 사용하고 있는 점을 생각할 때 무시할 수 없는 규격이 되어버렸
지만 유럽의 GS八4이나 초창기의 IS-95 등의 보코더의 기본 대역폭은 8KHz였으며，
이것어］ 부합되는 속도집합인 앉好0bps가 기본이었다．
    또한 이러한 속도집합의 상위로는 IS-95C의 고속 패킷 데이터 전송을 위한
Supplemental Channel을 위해서 확장되었다. 이것은 기본 속도집합의 xn의 형태
로 표시된다．
    이 절과 다음절에서는 IS-95의 Forw可d Reverse 채널을 공부할 것인데, 여기


                                   순방향 CDMA채널
                                  （기지국이 송신하는
                                 1. 23MHz대역의 신호）




                                                   동기 채널        Pilot ' 채넣
                                                    (32번）          (0번］ }




                                                   호출, 동기 , 파일럿 채널들은 논리채
                                                   널과 물리채널의 매핑 정보가 단말
                                                   기와 망 사이에 항상 공유되어야 하
                                                   므로 고정 Walsh 코드 값을 사용




                          （그림 乙22) CDMA Fo內yard 채널
       396                          7. 日ad山 Transmiss山n Technique
                                                                    口

에서는 RS1급을 기준으로 이야기를 하겠다. 또한 현재로서는 八4ulti-carrier 방식의
사용 여부가 현실성이 없으므로 SR3의 경우에 해당되는 항목들도 모두 거론하지
않겠다．
     Forw可d CI呱4A채널의 전체 구조를 나타내었다. Forw可dCI呱4A 채널은 Pilot
채널, 동기채널, 최대 7개까지의 호출채널, 그리고 여러 개의 Forward 트래픽 채널
로 구성된다. 이들 각각의 Code Channel들은 \Va1sh 함수에 의해서 직교 확산되며，
1.2288 Mcps로 고정 칩 속도를 가진 PN Code어］ 의해서 확산된다. 기지국에서는
복수의 Forward CI外江A채널을 사용하는 주파수 분할 다중화도 아울러서 사용된
다．
     할당된 64개의 Code Channel의 다른 구성으로는 호출채널 전부와 동기채널 1개
를 통화채널로 할당하여 1개의 P11毗채널과 63개의 통화채널로 구성할 수도 있다．
이 경우 호출채널과 동기채널은 할당되지 않는다．
     Forward 채널은 ＼人／alsh Code로 orthogonal 확산되어서 각각의 데이터들을
Code Channel로 분리하는 다중화小仙tiplexing) 방식을 사용하며, 기지국 신호를
나타내는 PN Short Code로 I, Q변조를 한다. Forward 채널에서 \Va1sh Code의
역할은 채널 구분용으로 Forw可（I 링크에서 사용하는 통화채널 이외의 Pu毗 채널
과 호출채널, 동기채널은 특정한 \V出sh로 변조되어서 전송된다. 즉 논리채널과 물
리채널의 매핑 정보가 단말기와 망 사이에 항상 공유되어야 하므로 고정 \Valsh
Code값을 사용한다. 그러므로 이 신호를 수신하는 단말기가 특별古 \Vaish Code
Channel의 정보를 수신하又 않아도 복조가 가능하다는 것이다. 이것은 단말기가 망
과의 별도의 상호작용을 거치지 않고 독자적으로 대기상태까지 진입할 수 있다는
이야기이며, 이것은 꺼꾸로 망은 단말기가 호를 시도하기 이전까지는 개별적인 단
말기의 관리를 하지 않는다는 이야기가 된다．

      7.5.1 Pilot 채널

     Pul毗 채널은 단말기가 특정 기지국 영역내에서 서비스를 제공받기 위해
coverage내의 단말기가 시스템어］ 동기를 맞춰 如丘ng및 Coherent 변조를 위한 위
상기준으로 사용하기             위한 기준채널로 무변조 확산（Unmodulated Spread
鈿玭trum) 신호이다. 무변조 확산 신호란 캐리어 신호 그 자체라는 의미이다. 즉
PN Short Code그 자체가 전송된다는 것이다. （그림 7-23）을 보면 알 수 있듯이
 7. Radio Transmission Technique



PN Short Code가 곱해지기 전까지 전혀 어떠한 신호도 없다. 최종적으로 PN
Short Code 자체만 전송되는 것을 확인할 수 있다．

                                                             Walsh Function 0

      Pilot 채널 (all 0's)

                                                                    1.2288Mcps




                卜채널 PN Sequence                     cos(2,vft)
                            1.228SMcps   Baseband                1(t)
                                           Filter



                                         Baseband
                                           川Iter                 Q('t)
                          1.2288Mcps
                      Q－채널 PN                       sin(2九兀口



                           （그림 下23) Pilot 채널의 구조도


 Pu야이라는 말의 사전적 의미는 "안내자" 혹은 "안내하다" 로서 가장 먼저 전송되
는 채널이라고 이해할 수 있다. CI呱4A에서 시간적으로 가장 먼저 수신되는 신호가
Pilot 신호는 아니다. 왜냐하면 모든 신호가 동시어］ 같은 대역으로 전송되기 때문이
다. 그러나 여기에서 Pu毗이라는 의미는 가장 먼저 전송되어서 가장 먼저 도착한다
는 의미보다는 가장 먼저 찾아지는 신호라는 의미일 것이다. 어쩌면 갇은 의미라고
도 생각할 수 있다. 알 수 없는 신호는 없는 것이나 마찬가지라고 생각한다면 가장
먼저 찾아지는 혹은 인지되어지는 신호가 가장 먼저 도착한 신호라고 이야기할 수
도 있을 것이다，
 우리가 사용하고 있는 PCS나 셀룰러 전화 시스템의 모든 기지국은 같은 주 斗수
채널을 사용하므로 Pilot Offset으로 구분되고 각 섹터 또는 셀을 구별하는 신호로
서 섹터 기지국인 경우어］ 3개 Omri 기지국인 경우에 1개를 할당한다．

 Pilot O竹set

 Pu毗채널은 각 기지국을 구별하기 위해서 각 기지국을 512개（2）의 옵셋 중 다
                                          7. Radio Transmission Technique
                                                                            1


른 값들로 설정되어 있다．
 I, Q 채널은 215召2768chip을 주기로 반복하고 1 ch如은 814nsec이므로 주기는
26.677msec이다. 이는 2초에 75회 반복되는 것이며 ，또한 정수배로 반복되는 것을
나타낸다. 때문어］ 우리는 언제나 짝수 초가 되는 시간에는 반드시 PN Short C어ie
가 시작하는 지점이라는 것을 알 수 있다. 64ch加을 하나의 옵셋 단위로 사용하므로
32768/64=512개의 옵셋을 갖는다．
 이 옵셋 인덱스는 0-offset pilot PN sequence(even sec）로부터 지연된 시간 차
이로 64chip을 하나의 옵셋으로 규정한다. 小offset pu毗 PN sequence 는 기지국
전송시간을 기준으로 매 짝수 초마다 출력되는 값을 시퀀스의 시작점으로 잡는다．
I와 Q 시퀀스어］ 대한 0尸offset pilot PN sequence의 시작점은 바로 이전의 15개 출
력값이 '0' 인 경우로 정의한다．
 Pu毗 PN 시퀀스 옵셋은 512대의 유일한 값을 가질 수 있다. 0-offset pilot PN
sequence로부터 주어진 p11毗 PN sequence어］ 대한 옵셋값은 인펙스어］ 64를 곱한
값과 같다.

 0非저I 7-1 Pilot PN Sequence Offset Index가 15인 Pilot의 시작점보다 얼마나
              지연되어있나2

  ,，풀0I , .   Pilot PN Sequence Offset = 15 X 64 = 960 PN chip
              Pilot PN Sequence의 시작시간은 기지국전송시간을 기준으로 매 짝
              수 초의 시작점으로부터 814[n sec] 乂 960[chip]=781.25?sec 이다．

 i距1三，느 12시 12분 12초 현재 Pilot Offset이 12인 신호를 수신하는 단말기는
              PN Short Code 의 몇 번째 Ch如을 수신하고 있는가2

：二！    ！「 현재 시간이 짝수 초이므로 단말기는 현재 기지국의 Pu毗옵셋의 人］
  it:：《，
              작점인 12X64 ch如을 수신하고 있다. 즉 768번째 ch如을 수신하고
              있다．


   7.5.2 동기채널

 동기채널은 기지국의 서비스 영역에서 단말기인 기지국과 초기시간 동기를 획득
하기 위해 사용되는 부호화, Interleaving, 대역확산 및 확산 변조된 스펙트럼 신호
이다. 동기채널어］ 대한 I 및 Q채널 Pilot PN 시퀀스는 해당 기지국의 Pilot 채널과
.
    7. Radio Transmission Technique                                                   399
                                                                                               I
같은 I꾜毗 PN 시퀀스 옵셋값을 사용한다. 단말기는 Pilot채널에서 Pilot PN동기를
맞추면, 동기채널의 동기화는 쉽게 할 수 있다. 이것은 동기채널과 그 밖의 모든 채
널들은 같은 Pilot PN시퀀스로 확산되고 동기채널어］ 있는 Frame 및 Interleaver
타이밍은 P11毗 PN시퀀스어］ 의해 정렬되기 때문이다. Forward 동기채널은 다음과
같이 형성된다．

                                               Modulation                Walsh Function 32
                      코드 Symbol                 Symb아




                                                                                  1.2288Mcps
     12Kbps             2.4Kbps                 也8Kbps            也8Kbps




                                                            cos(2,rl力
                                  quence
                                  1.2288M叩S                               끄t)
                                                 Baseband
                                                  Filter




                                                 Baseband
                                           卜      Filter
                                  1.2288M아）S
                                                                          Q(t)

                    Q-채널 PN Sequence                        sin(2,rft)


                              （그림 工24) 동기채널 형성


    채널의 구조

    동기채널은 동기채널 메시지를 1200bps로 전송하며 80ms길이의 슈퍼 Frame으
로 나누어진다. 각각의 동기채널 슈퍼 Frame은 길이가 26.666...ms인 서］ 개의
Frame으로 구성되어 있다. 동기채널 Frame은 iBit의 SSOMBit와 31 Bit의 동기
채널 加dy로 구성된다．
    동기채널 메시지 Capsule은 SOMBit를 제외한 동기채널 Frame body 만으로 구
성되며 기지국으로부터의 메시지를 담은 동기채널 메시지 부분과 통기채널 메시지
Capsule의 길이를 동기채널 슈퍼 Frame(8C吐ns）어］ 포함된 96 Bit 중 3개의 SOM을
뺀 93의 정수배가 되도록 하기 위한 오버해드 부분인 Padding으로 구성퇸다. 즉 가
변적인 길이의 메시지 몸체의 길이가 변경되는더］ 유동적으로 대처하기 위해서
    400                                                        7. Radio Transmission Technique
                                                                                                     1


Padding Bit가 추가되며, 이러한 Padding Bit는 모두 '0' 의 값을 갖는다．
 동기채널 메시지 Capsule은 S아d='l '인 동기채널 슈퍼Frame의 시작점에서만 시
작된다. SOMBit는 동기채널 메시지 Capsule의 시작（SOM='1'）과 동기채널 Frame
加dy를 구분（so入l='l '）하기 위해 사용퇸다．



          Sync Channel Super frame




     Sync Channel    Sync Channel    Sync Channel                               Sync Channel
        Frame           Frame                                                      Frame
                                        Frame     ，轟뵤
      Sync Channel       Sync Channel         Sync Channel                        Sync Channel
       Frame 加dy          Frame body           Frame body                         Frame body



                 Sync Channel Message Capsule                              Sync Ch. Msg Capsule

                                         93 X Ns bits
                                                                                               .，三


                          Sync channel Mes sage                            Padding

                           8 X MSG_LENGTI-I




     띠I   8b1t                  2사 1146 bit                  30 bit



                                    （그림 万25) 동기채널 구조


 동기채널 메시지는 길이필드와 메시지 몸체, CRC필드로 구성퇸다. 동기채널 머1
시지는 8 Bit의 八4SG工ENGTH 필드와 동기채널 메시지 몸체 그리고 CRC 필드로
이루어져있다．
 （그림 7-25）에서 Ns는 메시지전송어］ 필요한 동기채널의 슈피 Frame의 수이다．


   7.5.3 호출채널

 호출채널은 CDMA채널의 구성 중 하나로 통화채널이 할당되지 않은 단말기어］
system overhead ii寸ormation과 mobile Station specific message 등 제어정보를
전송하는데 사용된다．
    7. Radio Transmission Technique
U                                                                                                          臼I
                                                 Modulation                 Modulation          Walsh Function P
 호출     채널             코드 Symbol                  Symbol                     Symbol


                                                                                                      卜
 bits      Convolutional            Symbol                       注m卜，
             부호화기                  Repetition
            r=1!2. k=9                                       tote！니 난aver
                                                                                                    1.2288Mcps
                                                                                                      ,（
 9.6Kbps                   19.2Kbps                  19. 2Kbps               19.2Kbps
 4.8Kbps                   9.6Kbps
                                                                                                19.2Kbps

           호출 채널 P의 Long                    ,。                       1.2288Mcps
                                                                                         Decimator
           Code Mask                                                                 卜




                                                                            cos(2,r4t)
                     I-채널 PN Sequence
                               1      1.22881v1cp卜
                                                       Baseband
                                                         Filter


                                                       Baseband
                                                         Filter                          Q(t)
                                A 1.2288Mcps

                     Q-채널 PN Sequence


                                        （그림 刀26) 호출채널 형성


 호출채널의 전송속도는 sync channel 八/lessage의 Parameter PART가 0 혹은 1
로 설정됨에 따라서 앉洑0bps 혹은 4800bps로 고정 전송속도를 사용하게 되는데 동
일한 시스템（같은 SD）에서는 최대 7개(Walsh Code Channel 卜7）까지 사용할
수 있다. 그리고 Primary 호출채널은 \Walsh Code 1번을 부여한다. 호출채널은 다
음과 （그림 7-26）과 같이 형성퇸다．
 호출채널 데이터는 Block Interleaver를 거친 후 Long （뇨le발생기에서 생성된
데이터에 의해서 스크램블링된다. Long Code 발생기에 사용되는 Long Code
n追sk는 （그림 7-27）와 같다.

                                             2928     2423   2120                乂




                           11OOO11OO11O1 OOOOO PCN OOOOOOOOOOOO ｝가LOT_I칸나



                              （그림 石27) 호출채널 Long Code mask


    데이터 스크램블링은 Block Interleaver의 출력이 19Ksj羚이고 Long Code 발생
       402                                                                                    7. 日ad山 Transm治引on Te아｝nique
                                                                                                                                                        U


기의 출력이 1.2288Mcps이므로 Long Code발생기의 출력 중 64 PN chip마다 첫
번째 칩이 Block Interleaver의 출력과 moduo 2로 가산되어 스크램블링 한다．
 단말기에서는 단말기 유휴상태와 시스템 접속상태어］ 있을 때 이 호출채널을 통하
여 메시지를 수신한다．


  호출채널의 구조

  호출채널은 8劤T1S슬롯으로 나뉘어지고 2048개의 슬롯（163.84sec）이 최대 슬롯 사
이클을 구성한다. 각 최대 Slot 사이클은 亂ms단위의 시스템 시간을 2048로 나누었
을 때 나머지가 0인 Frame에서 시작한다. 각 8C竝ns Slot은 2아ns 길이의 4개 호출
채널 Frame으로 구성되며, 抑ns Frame은 lOms길이의 호출채널 반 Frame으로
나누어진다. 각 호출채널 반 Frame의 첫 Bit는 SCI(Synchronized Capsule
Indicator) Bit이다．



                      2048개의 Slot들로 구성되며168. 84초．163.84R bit                                            1


                                             Page Channel Sb1J                       Pa恥 ['hasrU
                                                    n                                      2047
                                                                                                             \\
                                                                                                                        8개의     호출        쟤널 half
                                                                                                                        frame들로        구성 되며80
                                                                                                                        me, 0.0811 bit.


   Page Channel half Page Channel half       Page Channel hull     ...            Page Channel half Page Channel half
        Frame             Fran쩌                   Frame                                Frame             Frame



   \                                                             1二느卜
          Page Channel Hal       Puge Channel Half                                                    \\\,                      Page Channel Half
            Frame 助as,             Frame助dy                      Page,
                                                                   Frame B。
                                                                          dy alf
                                                                         Chan쌉，             ···   「    Page
                                                                                                         Frame
                                                                                                            Ch,annel
                                                                                                                B。 dyIlaIf        Frame Body      三




                                   Page Channel Message Capsule                        Page Channel Message Capsule


                                                                                                                                            동기      된
   Si毗의      새로운                                                                          Page Channel Message               Padding        Capaule
   캡슐     시작이며，
   동기 된 캡슐
                                                                                            8X玉4SG_LENGTH             卜
                                Abutted messagea,
                                Unsynchronized

                    MSG小LENGTH                Message Body                                        메시지룔 채우고 남



                                                                     니
                                                                                                  는 영역이 생길 때


                        8 hit    +            2-   20。
                                                     2 hit                        3。hit
                                                                                                  사용됨．



                                                                                        R : 호출 채널 data rate (9600/4800bps)


                                                   （그림 工28) 호출채널 구조
    7. Radio Transmission Technique                        403
.


    호출채널 메시지 Capsule은 호출 채널상에서 전송되는 메시지들과 padding으로
구성된다. 호출채널 메시지의 길이 필드, 메시지 몸체, CRC필드로 구성된다. 길이
필드는 Octets 단위로 호출채널 메시지 전체를 나타낸다. 기지국에서 최대 호출채
널 메시지 길이를 148 옥텟, 즉 1184 Bit로 제한한다. 그러므로 길이 필드값은 148
옥텟을 초과하지 않는다. 메시지 몸체는 메시지 종류어］ 따라서 규정된 값들이 들어
가며, CRC 필드는 메시지 전송 후 단말기에서 오류를 검출하는데 사용된다．
    기지국은 동기 또는 비동기 메시지 Capsule을 전송할 수 있다. 동기 메시지
Capsule은 호출채널 반（牟） Frame의 두 번째 Bit에서 시작하여 시스템 시간과 정
렬이 가능한 Capsule을 말한다. 비동기 메시지 Capsule은 앞어］ 전송된 메시지 뒤를
따라서 바로 시작하는, 즉 시스템 시간과 정렬될 수 없는 Capsule을 말한다．
    일반적으로 호출채널의 메시지                   Capsule은 그것의   크기가 호출채널 반
Frame( l0ms）을 초과하는 경우가 많을 것이다. 그러므로 반 Fr跏ne의 시작 위치를
표시하는 SCI를 표시할 때 새로운 Capsule이 시작되는 경우에는 SCI를 1로 표시하
며, 그렇지 않으면 '0'으로 표시한다. 즉 동기 Capsule은 SCI가 1인 반 Frame의
SCI이후（즉 2번째 Bit）부터 시작되는 Capsule을 이야기한다．
    호출채널 메시지 후에 다음 SCI Bit가 시작할 때까지 8 Bit 이상 남아 있으면, 기
지국은 그 메시지 후어］ 비동기 메시지를 즉시 전송한다. 기지국은 비동기 호출채널
메시지가 뒤따르는 호출채널 메시지에는 padding Bit를 포함하지 않는다．
    호출채널 메시지 후에 다음 SCI Bit가 시작할 때까지 8 Bit 미만이 남았거나 호출
채널 메시지 Capsule 후어］ 뒤따라 전송할 비동기 메시지 Capsule이 없는 경우에 기
지국은 다음 SCI 앞까지 충분한 Padding Bit들을 포함시키고 SCI Bit 후에 동기
메시지 Capsule을 즉시 전송한다. 기지국은 모든 padding Bit들을 '0'으로 설정한다．
    기지국은 슬롯모드로 동작중인 단말기가 활성화된 후 곧바로 동기를 획득할 수
있도록 하기위하써 각각의 호출채널 Si毗에서 전송될 첫 번째 호출채널 메시지는
시스템 시간과 정렬이 가능하여 동기획득이 쉬운 동기 메시지 Capsule 형태로 전송
한다．

     7.5.4 Forward 통화채널

    Forward 통화채널은 통화중인 특정한 단말기어］ 제어신호 및 사용자 정보（음성정
보 혹은 데이터 정보）를 전송하는데 사용한다．
向                                                               7. Radio Transmission Technique
                                                                                                                            U



                                                                                   口Jnvolu t isnal
                                                         及茁i咆nCoder 「
                                                          Tail 8bit                         느’   c,   .   '卜    '   ]
                                               8.6Kbps                  9.6Kbps         r=   l
                                               4.0Kbps                  4 .8Kbps
                                               2．아伯PS                   2.4Kbps
                                               0.8Kbps                  1.2Kbps

                                                                                             （允de Syn巾이 H

                                                              PCB(800bps)
                             Modulat如n                                                       Walsh Fu ction P
                               ymb
               S V" 01bo i
             ii epe till On
  19.2Kbps                                                                                                     1.2288Mci冷
   9.6Kbps                     19.2Kbps
   4.8Kbps
   2.4Kbps
                                               Decimator         Decimator H 800Hz
                                  1.2288Mcps


                                  ++




               I-채널 PN Sequence                               口75(2九f刃                 Modulator
                                 1.2288Mcps




                                 I .2288Mcps                                                                            /
             七- Q；烈널 e上1 必（U1尹q드e                             e初似心略) _       -     m    /


                               （그림 万29) 日C倒 Forward 통화채널 형성



 지정된 Forw可d CI끄匹A채널에서 동시어］ 사용할 수 있는 최대 Forw可d 통화채
널의 수는 전체 Walsh Code의 개수 64에서 같은 Forw町d CDMA채널의 Pilot, 호
출채널과 동기채널의 개수를 뺀 것이다. 그렇다고 해서 한꺼번에 64개의 통화채널
을 쓸 수 있다는 것은 아니다. 여기에서 이야기하는 것은 어떤 Code Channel이 사
용될 수 있는 것인지어］ 대한 이야기이고 한꺼번에 쓰고 안 쓰고는 시스템의 혹은
채널의 용량문제로 다른 문제가 된다．
 이러한 통화채널은 （그림 7-29）과 같은 형태로 구성될 것이다. 이것은 RC1인 경
우를 나타내는 것이며, 이것은 IS-95B의 Supplemental Code Channel(SCCH :
Supplemental Code Channel)을 형성하기도 한다．
 다중화 과정에서 Decim毗아의 출력 속도가 8(X死七인 것은 전력제어 Bit를 천공
    7. Radio Transmission Technique
1                                                                                      405


하기 위한 타이밍을 제공하기 위해서 이다. 이것과 연계해서 전력제어 Bit의 결정도
8001七로 이루어지며, PCB는 800bps로 출력되어 다중화 된다．
    RC3의 경우 民rward Fundamental Channel과 Supplemental Channel의 구조
를 정리하면 （그림 7-30）과 같이 된다. 이것은 근본적으로 앞서 이야기한 RC1과는
현격한 차이가 있으며, 이것은 고속 데이터의 에러성능을 개선하는데 더욱 주력했
음을 볼 수 있다. 그것은 （그림 7-30）에서는 앞의 （그림 7-29）의 변조단과 텨ock
Interleaving 단 앞에 심볼 천공작업이 추가된다．
    여기에서 채널코딩을 할 때어］ 특정한 속도 이하, 즉 4배속 이하의 속도에서는 기
존의 Convolutional 부호화기를 사용하지만 그 이상의 속도에서는 터보 C（넋II坦으
로 연집 에러를 수정한다． RC3의 경우 전력제어 Bit를 다중화 하는 과정 Long
Coc妃를 다중화하는 과정은 （그림 7-29）의 다중화 과정과 동일하다.
                                                                                Modulation
                                                                                 Syn小아

                 ('ott rot Lit 003!                             1   L   1   ]
                      1    " l " urbu
                                                              ‘긴！사 리 n!
       業，
                    卜』 tt'oCl or
     Data Rate                                                                     Symb아



                                              烈卄
      lkbp引                N            Factor     Deletion   Symb이S              Rate (kbp引
        1.5               1/ 4                      I of 5      768                  38.4
        2.7               1/ 4                      I of 9      768                  38. 4
        毛8                1/ 4                      None        768                  38.4
        9. 6              1/ 4                      None        768                  38.4

                                          1
                                          l   X
        19.               1/ 4                      None        1,536                76.8
                                          1
                                          1   X
       38.4               1/ 4                      None        3,072               153.6
                                          1
                                          l   X
       76.8               1/ 4                      None       6,144                307그
                                          l   X
       153.6              1/ 4                      None       12. 288              614.4




      （그림 刀30) RC 3의 Fundament톄 ChanneIjlF Sup口en그ental Channe떽 형성


 （그림卜30）은 RC3 이상에서 사용되는 새로운 형태의 변조 기법을 보여준다. 이
책에서는 non-TD방식어］ 대해서만 이야기한다．
 （그림 7-30）어］서 \Valsh 함수는 +1(=0）과 Hl(=l）로 대응이 되며, QOFsign은 QOF
마스크에 곱해지는 부호를 나타낸다. 이것 역시 0일 때 양을 1일 때 음을 나타낸다．
WalShr。
      t는 0과 1로 표시되며, 0일 경우는 회전되지 않는 것이고 1인 경우 以尸회전
된 경우를 나타낸다. 이러한 상태에서 Null QOF는 기존의 Walsh Code에 0을 곱
하여（QOFsign=+1) 모든 요소들을 0으로 만들고, Walsh毗를 0으로 하여 회전하지
않는 것이다. 이것은 RC1, RC2의 형태로 변조할 때 사용한다. 즉 이러한 QOF와
   406                                      7. Radio Transmission Technique
                                                                              .


Walsh Code를 곱하면 \Valsh Code만 남게 되는 결과가 생기게 된다．
 지금까지 실제 사용되고 있는 Is小95의 Forw町d 채널들을 공부하였다. 이러한
Forw可d 채널은 일반적인 단말기가 망 내어］ 포함되기 위해서 Pilot채널과 동기채
널, 호출채널 등을 수신하여 처리한다. 물론 통화를 한다면 통화채널까지 복조 하는
기회가 있을 것이다. 이러한 일련의 채널들은 각각의 역할들이 있으며, 그것들은 서
로의 역할을 분담하여 그것의 목적을 수행하고 있는 것을 확인할 수 있다．
 우선 Pilot 채널은 그것이 단말기에 의해서 성공적으로 복조가 되게 되면 Pilot차1
널은 단말기에게 다음으로 찾게 될 동기채널의 주파수와 위상정보를 제공하게 된
다. 단말기는 Pil毗으로부터 제공받은 이러한 정보로 동기채널마저 복조할 수 있게
되고 여기에서는 호출채널을 성공적으로 복조하고 그것을 통해서 전송되는 각종 정
보들을 수신하기 위한 시간 조정 작업을 하게 된다. 즉 동기채널은 다단말기에게 시
스템 시간정보와 호출채널의 속도 등과 같은 호출채널 복조어］ 도움이 되는 정보들
을 제공한다.




   Yl
   Walsh
   함수



   QOF叱




           W키帥r아   U" ' 니나 " 니     11！
                                     弓四         stn(2可띠
                             PN1
                          F'＼日,


                     （그림 刀31) Modulator(l, 0 Mapping)


 이렇듯 각각의 채널들은 그것의 역할들이 서로 구분되어서 자음단계로 천이를 할
수 있게 한다. 물론 그것을 하나의 채널을 통해서 할 수 없지 않겠지만 어떻게 보면
그러한 기능들의 구분을 각각의 채널이 구분되는 계기가 된 거］ 아닌 가도 생각할
수 있을 것이다．
                                                                  H
         7. Radio Transmission Technique                 I-           I
     .                                                   [407
              Reverse 채널 구조
                                                                mmH
                                                                      )
         Reverse CDMA 채널은 /\ccess 채널과 통화채널로 구성되며, Is的C이후에는
Reverse P표毗채널도 추가로 사용되고 있다. 이러한 Pilot 채널은 Forward 채널과
마찬가지로 전송신호의 기준이 되는 신호의 역할을 하며, 따라서 Reverse도 이러한
pilot을 통해서 4장에서 설명한 것과 같은 Coherent detection을 할 수 있게 해 준
다．
     （그림 7-32）는 Reverse 채널의 신호들을 보여준다. 각각의 통화채널은 서로 구별
되는 사용자 긴 코드 시퀀스어］ 의해서 구별되고 각 /\ccess 채널은 서로 다른
Access 채널 긴 코드로 식별된다. 기지국은 다중화된 Reverse CI呱4A 채널들을
주파수 분할 다중화 방식어］ 의해 사용할 수 있다．



                                       역방향 CDMA채널
                                      （기지국이 수신되는
                                     1.23MHz디：
                                             1역의 신호）




            PCH loll
            대응되는
            ACH 1번




                         （그림 石32) CDMA 딕everse의 논리 채널들


         7.6.1 Access 채널

     Access 채널은 항상 4800bps로 전송하여 앉文刃bps보다 상대적으로 오류가 적게
발생한다. 따라서 입력되는 정보 Bit는 Frame당 98 Bit 된다. 이러한 /\ccess 채널
의 특징은 변조에서 Offset QPSK를 사용한다는 것과 \Va1sh Array 변조를 한다는
것이다．
     각 /\ccess 채널은 Access 채널이 전송하려고 하는 내용이 포함된 Capsule과
   408                                                            7. Radio Transmission Technique
                                                                                                    1


Access 채널의 검출 혹은 식별을 용이하게 하기 위한 Preamble로 구성된다．
Preamble은 1+PAM SZ개의 "0"을 전송하여 기지국에서 쉽게 인지할 수 있도록
한다. 또한 전송할 내용이 들어가게 되는 Capsu扼은 3小4A乂．CAP으로 정의되며，
여기에서 入'lAX_CAP size는 망에서 정의하게 되어 있다．
 이러한 Prea끄的le은 Reverse Pu야이 없는 상태에서 전송되는, 즉 RC1,2로 전송
되는 /iccess 채널 등은 Coherent detection을 할 수 없는 상태이고 이러한 이유로
초기어］ 기지국의 복조기가 채널의 Frame을 복조하기 위해서 동기를 맞추기 위한
시간이 필요한데 이것이 제공해주는 것이다. 따라서 이 I노eamble 역시 다중경로의
범위 내에서 알맞은 값으로 설정되어야 할 것이다．
 실지로 IS-95에서 사용하고 /\ccess 채널을 통해서 전송될 정보들의 양은 망이
발전하1 오면서（소위 말하는 IS弱A에서 IS-95B로 그리고 IS-95C 혹은 IS-2000으
로 발전하는 경우를 말함） 점점 많아지게 되었다. 따라서 망이 나타내고 있는
Protocol 개정번호에 따라서 이러한 八'lAX_CAP Size가 각기 다르게 관리되고 있
다. 예를 들면 Is弱A에서는 "1", IS-95B에서는 " 2", IS的C에서는 "3" 등이다．


                                                                         Modulation
    억세스                   코드 Symbol         반복된 Symbol                    Symbol
    채널
    bits


                                                             =J
     也8Kbps                 14.4Kb1冶         28.8Kbps                 28.8Kbps



                                        4.8Ksps(307.2Kcps)
                                                                         변조 심벌 (Walsh chip)

                                I-채널 PN Sequence                                 cos(2,r1Ot)


                                           1.2288Mcps             Baseband
                                                                   Filter


                                           1/2 PN chip Delay
                                               = 406.9ns
                   ['N chip
                   1.2288Mcps                                     Baseband
                                                   D
                                                                   Filter
           Long Co.                        l.2288Mcps
           Generato


               十
         Long Code Mask
                                Q채널 PN Sequence




                                （그림 下33) Access 채널 형성
    7. Radio Transmissi o n Technique                                                                                           409
1

    이러한 이유로 Pr毗ocol 개정번호어］ 타당하지 않는 入'TAX_CAP size가 제공된다
면 /\ccess 채널로 전송되는 메시지 내용의 일부가 소실되는 경우가 발생될 수 있으
며, 이것은 단말기의 Access 성공 율의 악화를 초래할 수 있다．
    이러한 사실은 실제 필드에서 나타나고 있는데 한국의 이동업체들은 여러 가지
이유로 인해서 IS-95B를 생략하고 Is-弱A에서 IS-95C로 발전해갔다. 물론 우리
는 IS-95B의 서비스인 MDR 서비스를 사용했으나, 이것은 엄밀히 말하면 IS-95B
가 아니라 Is小95A＋入'IDR망인 것이다. 문제는 여기어써 발생한다. Is小95C단말기는
Prot(乂ol 개정번호가 5인 지역, 즉 Is弱B지역어］들어가면 이어］ 합당한 Access 채
널을 구성하려고 할 것이다. 이것이 Backw町d comp砒小小ty이다. 그러나 한국의
이동업체의 경우 Pr야ocol 개정번호는 5이나 八IA)LCAP size는 1로 IS-95A의 형
태로 내려가므로 四円햐\.+MDR망이므로） IS-95C가 아닌 지역에서는 /\ccess 채
널의 메시지의 내용이 소실될 가능성이 높아지게 된다．

                                                                                                  0.02X(4+PAM SZ+MAX_CAP,,SZ) 초,
      120 mc, 96bit임                                                                              96X(4+ PAM_SZ+MAX_ CAP_SZ) bit 임
                                                           Acre卜5 ( 1      :                 i1

                                      1

         Acceaa Channel        1..        Access Channel         Acceaa Channel         Access Channel     Access Channel
             Frame                            Frame                  Frame                  Frame              Frame


                                                            \N
                                                                       Access Channel              Access Channel     Access Channel




                                                             /
                                                                        Frame Body                  Frame Body         Frame Body
          Page Channel Message Cap8uIe



        1+PAM SZ 개의
        Frame,    96 X
                                                                               Access Channel Message Capsu le
        (1+PAM_SZ)bit


                                                                                             88 X Nf bit


    Nf frame , 96 X Nf bit
    3+MAX小CAP_SZ룝       초과
    하지 않음．


                                                                                                                    머］시지를 채우고 남 !
                                                           8 X MSGLENGTII                                           뇬 영역이 섕길 n}1
                                                                                                                    人f붕 뇜 .

                              MSGJ皿NGTH                            Message Body                     CRC

                       卜 삐口小
                          I          Sb仕         1                  2- 842 bit               七늬
    Nf : 메시지 전송을 위한 Access Channel Frames 4.                                                               T : 부호화기 Tail Bit




                                                （그림 石34) Access 채널 구조
   410                                                    7. 日ad山 Transn기ss山n Technique
           1                                                                              1



 Access 채널의 전송
 Access 채널 메시지의 전송은 앞서 이야기되었듯이 /\ccess Probe를 통해서 전
송된다. 또한 그것의 전송 시작 시점은 다음과 같이 /\ccess Parameter들로 결정되
며, 그것의 resolution은 system time이 된다. 이러한 시작시점을 구체적으로 표시
하면 다음의 식과 같다．
         txmod(4+MAX_ CAP_ SZ+ PAM_ SZ)=0

 위의 식과 같이 t(System time）는 호출채널 moth切ring과 /\ccess 채널 전송시
점을 결정하는 중요한 시간요소이다．
 위의 식과 같은 시점어］ 전송이 시작되나 앞서 이야기한대로 r可idom Access를
위해서 실지로 메시지가 전송되는 시점은 임의의 지연（Randomization delay）이 있
은 후어］ 이루어진다. 이와 같은 내용은 （그림 7-35）어］ 나타나 있다.
 이상과 같은 절차는 매 /\ecess Probe를 전송할 때마다 발생하게 된다. RN
(PROBE_PN_RAM 이용）의 값은 ESN(Electronic Serial Number）을 이용한
hashing으로 값을 산출하며 실제적인 값은 0에서 511까지 분포된다. 이 PN
randomization delay는 단말기와 기지국간의 다중켱로의 경로의 크기와 연관될 수
있으며, 따라서 기지국 복조기（Searcher）의 Search Window의 크기어］ 따라서 유동




                                                      I
적으로 적용될 수 있다．
 PN Randomization Delay의 근본 목적은 Random Access 절차어］ 의해서 수행
되는 것이며, 이것은 각각의 다중접속 시도간의 충톨을 방지하기 위한 것이다. 이런
                                                      m
                  PN Randomization
                        '        i
                                     Delay
                                             =   RN
                                                 i
                  X 0.8138m




                                                                            TIme
                  전송시작시간 = t x mod(4+MAX_CAP_SZ + PAM_SZ) = 0



         （그림 石35) Randomization d이ay후 전송되는 Access 채널 Message
U.7. RadioTransmission
                  『印「nique                                         口月
의미에서 이것은 Preamble과는 그것의 의미가 다르다. 이러한 random delay로 인
하여 일종의 비동기 전송으로 볼 수 있다
 긴 코드에서 사용되는 마스크는 단말기에서 사용하는 채널 형태어］ 따라서 달라진
다. Access 채널을 통해서 전송되는 신호는（그림 7-35）와 같은 형태로 masking되
고 이러한 masking은 앞서 3장에서 이야기하였듯이 생성다항식의 초기값을 설정해
주는 역할을 하게 된다．


        41              3332   28 27   25 24         98            0

             110001111     ACN       PCN   BASE_ID        P比OT P


             ACN : 억 세스 채 널 Number

             PCN : 호출 채 녈 Number



                  （그림 石36) Access 채널 ZJ 코드 마스크


   7.6.2 Reverse 통화채널

 단말기는 Reverse 통화채널상으로 Forward과 동일한 데이터 속도 집합들로 전
송할 것이다. 그러나 IS-95C이후에는 약간의 변화가 있으나 기본적으로 그것의 소
도는 유사한 형태로 제공된다. 또한 Frame의 크기도 20ms로 사용하며, 5ms
Fran祀의 n血ni Frame도 있으나 이것은 특정한 규격에서 제안되고 있다．


 보코더 Frame 옵셋

 단말기는 스태거된 통화채널 Frame을 사용하게 된다. 이러한 보코더 Frame의
시간옵셋은 각종 Handoff 지시 메시지나 채널 할당 메시지 등을 통해서 FRAME_
OFFSET Parameter어］ 의해 규정퇸다. Reverse 통화채널 시간 옵셋은 F아ward
통화채널 시간 옵셋과 같은 것을 사용한다. 이것은 앞서 이야기한 것과 같이 시스템
의 보코더（Svc）의 시간 옵셋이다. 시간 옵셋이 0인 Reverse 통화채널 Fran犯은 시
스템 시간이 20ms의 정수배인 경우에만 시작되며, 스태거된 Frame은 0옵셋 통화
채널 Frame보다 1.25 X FRA1V1E. OFFSET ms만큼 늦계 시작한다. Reverse 통화
채널 Interleaver 블록은 Reverse 통화채널 Frame어］ 맞추어 정렬퇸다．
I      412                                                       7. Radio Transmission Technique
                                                                                                   U


 Reverse 통화채널은 /\ccess 채널과 마찬가지로 \Va1sh 변조를 6千ary Ortho
gona1 M以加1毗or를 사용하여 Forw可d과는 좀 다른 형태로 진행퇸다. 즉 ＼入／aish
인덱스 역할을 하는 6 Bit가 입력되면 그 인덱스에 해당되는 64 Bit가 출력되는 형
태로 처리된다. 즉 이것은 약 64/6의 코드율을 가진다고도 생각할 수 있으며, 때문
어］ 입력되는 정보가 28.8Kbps인 경우 출력은 307.2kcps가 된다. 이후 단은
OQPSK로 변조가 되며, 이때 1/2 PN chip만큼 지연이 필요하다.


    순방향 통화 채널
                                                     Add Encoder
    정보비트              >
                                            +          Tail 8bit
    (172.80,40,l6bpf)
                                        8.6Kbps                       9.6Kbps
                                        4.0Kbps                       48Kbps
                                        2．아小PS                        2.4Kbps
                                        0.8Kbps                       1.2Kbps
                                                                                     코드 Syn巾아
        28.8Kbps
        14.4Kbps
         7.2Kbps                          Modulat沁n
         3.6Kbps                       Symbol (Walsh chin)

               Symbol                                             64-ary           Data Burst
              Repetition                                      (i)rthogonal H+      Randomizer
                                                               Modulator
                           28.8Kbps             28.8Kbt瑁



                                I-채널 PN Sequence


                                          1.2288Mcps             Baseband
                                                                  Filter

                                           112 PH chip Delay
                                               = 406.9 na
                   I가너 chip
                   1.2288Mcps                                    Baseband
                                                1卜   D    +
                                                                  Filter
                                           l. 22S81Tcps


                                 Q－채널 PN Sequence                               sin(助打泣)

        Long Code Mask



                                 （그림 下37) RC1/2의 통화채널 구성


    이것 역시 RC3 이상의 형태에서 좀 다르게 변조가 되며, 그것의 대략은 다음과
같다. 여기에서도 마찬가지로 채널코딩을 다르게 적용하며, 다음 단은 \Va1sh 변조
단으로 앞서 설명한 64／뇨y 변조와는 다르게 적용이 되며, 그렇다고 다중화 개념의
Forward의 ＼사aish와는 또 다른 변조 방식이다．즉 이러한 Walsh 변조는 다중화의
    7. 日ad山 Transit기ss山n Technique
U

의미로 사용은 되나 단말기가 Reverse으로 전송하는 각종 채널들을 구분짓는 인자
로서 그것이 사용되며, 그것들의 내용은 （그림 7-41）어］ 나타난 것과 같다．

                                                                 Modulation
                                                                  Symbol
               Convolutional
 채널 Bi          휵은Turbo                                              w
                 Encoder




                      R mmm
    D카a Rate                                                     Symb이 Rate




                                     仙帥hnn
     (kbps)                                  1뇨키etion   Sym加Is     (kbp引
       1.5                                    1 of 5      768       38.4
       2.7                                    1 of 9      768       38.4
       4.8                                    None        768       38.4
       9.6                                    None        768       38.4
                                     n
      19.2          1/4                       None      1,536        76.8
     38.4           1/1                       None      3,072       153.6
      76.8          1/4                       None      6,144       307.2
     153.6          1/4                       None      12.288      614.4
     307.2          1/2                       None      12.288      614.4




 （그림 刀38) 日03의 日everse Fundament톄 Chann터과 Sul）이ement졔 Channe떽 구성


 또한 주의할 것은 Reverse 전력제어를 하기 위해서 PCB마다 전력제어 Bit를 전
송하는더］ Reverse의 경우 Pilot어］ 실어서 전송하며, 그것은 Forw町d의 천공 방식
과는 달리 Reverse Pilot어］ 다중화해서 전송하므로 Reverse의 R下F가 Forward과
비교하여 전력제어 Bit 천공 프로세스 등의 절차가 없다．

     7.6.3 Reverse Pilot 채널

 Reverse Pilot 채널은 IS-95C 이전에는 없던 것으로 이 채널은 RC3이상의 형상
에서만 변조될 수 있는 신호이다. 따라서 이것은 Reverse Supplemental Channel
등과 같은 95C용 채널이 전송될 때에만 전송이 되는 것이다. 또한 이 채널은
Forw可d Pu야과 마찬가지로 무 변조 신호로 \1alsh가 0번으로 변조되나 전력제어
Bit와 함께 다중화되어서 전송되게 된다. 그것의 구조는 （그림 7-39）와 같다.
 즉 Forw可d의 전력제어를 위한 정보를 Reverse Pilot의 정보에 다중화하여 전송
하게 된다. 이것은 Reverse 전력제어를 위해서 PCB를 전송하는 채널이 Forward
통화채널이고 이것을 천공하는 것과는 차이가 난다. 이러한 것을 볼 때 Forward 전
력제어는 Reverse의 전용 전력제어 채널을 사용하여 이루어진다고 볼 수 있다．
                                                  7. Radio Transmission Technique
   4 仁工
                                                                                    U



                                                     Pilot
     Pilot（모두 0) 1十
                               MUX. H                                    켜
                                                     384 Chip니
     전력제어비트 H竹
                                                      1536 Chip


                        （그림 万39) 日everse 전력제어 부채널과 P的t 채널


 Forward의 Pu毗은 이러한 용도로 사용할 수 없는 것이 특정한 단말의 전력제어
Bit를 전송할 수 없는 것이 Forw町d의 P11毗이기 때문이다. Forwardi꾜야은 기지국
을 식별하고 기지국의 모튼 단말들이 확인해야 할 공동의 채널이기 때문이다. 때문어］
개별적으로 관리되는 전력제어 Bit는 개별적으로 전송되는 통화채널로 전송될 수밖어］
없고 그것이 일반 통화채널의 정보를 잠식한다 할지라도 어쩔 수 없는 것이다．


     전송출력
                        20m. 통화 채널 프
          I             레임의 시작




                                        i
                                                                             time

              4긔UM_      PREAMBLE   .       .   2。
                                                 ms Frame            .
                      개위 선딕 又小거그눕       1




                               （그림 石40) 日everse 프리얻블


 Reverse Pu야은 Reverse 통화채널의 프리엠블을 제공하기도 한다. 이러한 프리
엠블들은 RC 可6의 Reverse Fundamental Channel이나 Reverse 전속채널이 전
송되기 전어］ 전력제어 그룹（1.25邸） 단위로 P11毗을 통해서 전송된다. 이러한 것은
단말기가 Hard Hando甘를 하게 될 때 통화채널 Frame을 보내기 전어］ Handoff 지
시 메시지에서 표시하고 있는 NT爪LPREAMBLE개의 전력제어 그룹의 시간을 프
리엠블로 사용한다. 즉 NUM_PREAMBLE X 1.25ms의 시간 이후에 통화 Frame
을 전송하게 된다. 이러한 Reverse Pu毗은 （그림 7-41）과 같이 변조가 이루어지며，
여기에서 기저대역의 모든 속도는 1.2288Mcps로 설정될 것이다．
 과거의 Is弱A의 경우 Reverse은 하나의 Code Channel이 하나의 개인코드가
              7. Radio Transmission Technique                                                         415
.                                                                                                [

되었다. 그러나 IS-9＆에서는 여러 개의 코드를 사용할 수 있게 되었다. 따라서 각
각의 채널에 대해서 각기 디른 \Valsh Code를 사용하여 구분지으며, 이러한 Walsh
（力de의 사용은 기지국에서 쉽게 복조할 수 있도록 하기 위해서 （그림 7-41）과 같이
미리 설정해 준다. 이러한 \Va1sh는 앞서 3장에서 이야기되었듯이 \Va1sh Code의
길이어］ 의해서 대역확장의 기능을 수행하게 되는데 이것은 단순히 대역을 더하여
대역확장을 하는 방식과는 차이를 둔다．

                    W訃尉i Cover
               (+＋小m) 혹은 (++H1나＋)




    忍
                 Pilot


         藕                                                                     口7s(2느i屯)



                  Walsh Cover
               (++++++++



         ；提
                                                                             기저대역겹
                                                                              필터 +
                                                                                           ,<)
                  Walsh Cover                                                                    「7
              (+ +++1小寸냐＋++H叫나
                                                                            邕， 李心

    据，
                                                                               sin('2域刃


                  Walsh Cover
                (+-) 혹은 (＋卜H




                  I-Channel PN Sequence                         Q-Channel PN Sequence

          Long
          Code
          加lask          I.｛나l日 ('ode rn m '
                                                    1 Chip 지연



                                               （그림 刀41) 日everse 변조
    8. IS-95 Call Flow
.




                               Is山95 Call Flo사




    깜깜한 방어］ 들어가서 스위치를 켜면 방 안이 환해진다. 또한 세탁실에 가서 세탁
기어］ 전원을 공급하고 스위치를 누르면 커다란 세탁기가 소리를 내면서 돌아간다．
그런데 내가 이러한 작용들을 위해서 무었을 했는가？ 단지 손가락어］ 약간의 힘을
주고 스위치를 ON한 것 이외에는 한 일이 없다. 그러나 엄청난 운동에너지의 행동
들이 이루어지는 것이다. 즉 내가 힘 안 들이고 스위치를 켜는 일은 상태의 변화 혹
은 천이를 위해서 동기부여를 한 것이다．
    또한 이러한 동기부여라는 측면에서 스위치를 손으로 ON, OFF 하는 것이 아니
라 리모콘으로 한다면 더욱 적은（운동）에너지로 동기부여를 할 수 있다. 더욱 세련
된 방법이겠지요. 이러한 동기부여를 하게 하는 것이 각각의 계층에서 이루어질 수
있으나 이 장에서는 주로 Layer 3, 즉 Signaling Layer에서 이루어지는 동기부여
어］ 대해서 공부할 것이다. 이러한 동기 부여는 주로 L3의 처리를 위하써 제공되는
Message 들이 될 것이다. 예를 들어서 Channel Ass塘nment 八/lessage가 전송되
고 어떠한 채널을 할당하겠다는 것은 실지로 단말기에게 망에서 상술퇸 내용의
Channel 자원을 할당하게 되는 것을 유발시켜 주는 것이다．
   418                                8. IS-95 Call Flow
                                                           1



     In川al Sta扼 처리
                                                           )
 단말기 초기화는 사용자가 단말기를 새롭게 켠다튼가 통화중이던 호가 어떠한 이
유로든 종료되었턴지, 혹은 IS-95에서 규정한 상태에서 상태유지가 되지 않을 때에
발생퇸다. 단말기는 이러한 초기 과정에서는 자신이 콴리하는 메모리（Flash
入4emory）어］ 미리 저장되어 있는 값들을 읽어 들이고 이후의 절차를 수행한다．
 단말기의 메모리어］ 저장되어 있는 값들 중어］ 단말기가 서비스받을 망어］ 대한 정
보들로 해당 망과 관련된 정보가 있으며, 이러한 정보는 단말기의 일방적인 정보가
아니라 망과는 여러 가지 다양한 형태로 공유되는 정보들이다.
 단말기는 다음의 （그림 斗1）과 같이 초기 상태에서는 4가지의 부 상태들로 구분
되어서 관리된다· 이러한 각 단계는 싯슨텔受，멨얏 채널 획득， 量갔채널 획득，
시간 변경 상태로 생각할 수 있다．


            전원 ON혹은 기타 다른
               상태에서 천이




                （그림 8-1) 단말기 초기화 과정
          8. IS-95 Call Flow                         419
      .


          이상의 과정에서는 단말기가 성공적으로 대기상태에 들어가서 지속적으로 해당
망의 정보를 수신하기 위한, 즉 통신하기 위한 준비 작업인 동기가 주요 작업이 퇸
 다．
           8.1.1 시스템 결정 상태 : 사용할 시스템 선택

          시스템 결정（System Determin毗幻n）은 단말기어］ 전원을 인가한 이후부터 시작
되며 필요한 시스템 정보를 단말기의 영구／반영구 메모리（E乍ROM）로부터 읽어와
 서 단말기어］ 필요한 Parameter를 설정한다．
          사용자가 단말기의 전원을 켜는 경우 단말기는 PC의 (i-MOS와 유사한 boot
sector에서 프로그램을 시작하여 RAM의 정상 동작 여부를 확인하고 전체 메모리
 영역어］ address 영역을 할당한다. 이후 단말기는 RAM어］ Interi끄I元 \Tect아를 형성
시키고 단말기의 기본 동작인 booting을 완료한다. 기본적인 환경설정이 완료되면
탄말기는 E2PRO八4에서 필요한 NAM Parameter를 RAM 영역어］ 확보하고 Flash
八4emory어］ 내장되어 있는 단말기 운영 소프트웨어, 즉 실행 코드인 Binary Files
 어］ 의해서 CDMA호 처리가 될 수 있도록 해당 S/W task를 동작시킨다. 이러한 사
 전 정보들은 단말기가 어떤 망에 /\ccess하햐 하는지를 결정하는 시스템 식별자
嬋땄）는 물론 그 시스템에서 실지로 신호를 수신하기 위해서 지정받을 채널인 1차
 채널（Primary 채널）과 2차 채널 등이 있다. 즉 1차 채널은 해당 망의 어느 지역어］
 가도 수신할 수 있는 채널이어야 할 것이며, 때문어］ 망을 설계할 때에도 1FA기지
국，즉 工캣읜숫팟숫맡量흐쁘：늪그잣굴읨－겻웃姓모트스m多芭又짼낱量童렬
을 하게 해야 한다. 실지로 운영되고 있는 기지국의 경우 가입자 용량에 따라서 이
 러한 FA를 증가 시켜가며, 이러한 구체적인 예를 튼다면 현재 PCS의 경우 도심지
  역의 기지국들은 4개의 주파수를 출력하고 있다．
          즉 단말기는 해당 Band Class어］ 해당되는 주파수에서 system을 결정하고
Primar3/ 채널로 이동하여 호 처리 준비를 한다. 예를 들면 PCS 대역에서 019시스
 템을 설정하고 019의 Primary 채널인 475로 복조기를 tuning한다. 만약 Primary
 채널이 실패할 경우 secondary 채널로 이동하여 동일한 작업을 수행한다. 또한 단
말기가 REDIRECTION 메시지를 수신하게 되면 다른 시스템 또는 다른 주파수 대
  역으로 이동하여 정의된 동작을 수행한다．


\ . RA, '1 .         的，破飢 ）竹라 刹한 ""?
                                   '「
                                          8. lS95 Call Flow
                                                              a


   8.1.2 Pilot 획득 상태1 :CDMA시스템의 Pilot 채널을 획득

 이 단계는 단말기가 서비스 받을 망으로부터，小 VV,，中 V ! .         하기 위해서 취
해지는 단계이다. 앞서 이야기한 시스템 결정 단계에서는 이 상태를 위해서 준비하
는 상태이다．
 IS-95에서는 기지국에서 송출되는 모든 신호의 대표격인 Pilot 채널을 수신하는
데어］ 추가적으로 상위 계층에서 Code Channel 등의 정보를 수신하지 않아도（수신
할 수도 없다） 복조할 수 있게 하기 위해서 특정한 Code Channel을 정하1 두어서
단말기에서 PN Code 수신 후 곧바로 복조할 수 있게 하였다. 이것은 비단 Pu야뿐
아니라 동기채널 및 호출채널도 마찬가지이다. 또한 Pu'야을 가장 먼저 수신（혹은
인식）하기 위해서 끄姓＼싶혼읜工쁘乞Qh4쁘르l呈更奭뇨끄뾰으로 하여 단말기에서
쁘工으奭量-r신하면 그것아 곧Pilot크툐이 되게 하였다． 따라서 단말기는
Prim可y 주파수 채널의 I亐lot 신호를 검색하면서 Code Channel은 0번으로 설정하
여 탐색한다. 결국 I亐lot 신호는 Code Channel이 0번이므로 Code Channel 변조를
By
 '月ss한 PN Code 그 자체가 되는 것이다．
 일반적으로 대역 확산 통신 시스템은 확산된 신호를 다시 복구하기 위해서는 확
산된 코드를 다시 곱하는 절차어］ 의해서 구해지며, 이러한 방식을 위해서는 수신단
에서는 송신단에서 출력한 확산 코드를 찾는 것이 중요하다. 이러한 방법어］ 대해서
는 상세하게 4장에서 공부하였다．
 이런 방식으로 탐색하던 단말기가 15초（T20m）초 내어］ Pilot 채널을 찾으면 동기채
넬브眠브언끄프므쁑잔星할쓰圭크삿스브型므燮부터 시작한다· 단말기
가 성공적으로 Pilot 채널을 찾으면 동기채널 획득 단계로 넘어가고, 동기채널을 수
신하면 이때부터 시스템 정보를 수신하여 단말기어］ 시간을 표시하고 PN C月e의
offset을 알 수 있는 것이다．

   8.1.3 동기 획득 상태

 동기 획득 상태는 CDMA시스템의 시스템 구성과 시간정보를 획득하는 단계이
다. 단말기는 Pilot 채널을 획득한 후 동기채널 획득 부 상태에서 시스템의 구성과
시간정보를 얻기 위하1 기지국이 보내는 동기채널 메시지를 수신하여 처리하게 된
다. 이때 단말기는 동기채널을 위하d 자신의 Code Channel(Walsh 32）을 설정한
       8. IS-95 Call Flow                             r H弓I
                                                      .1421 I
   .                                                  J      1

  다. 단말기가 이 상태에서 1초（ T21m) 이내어］ 유효한 동기채널 메시지를 받지 못하
   면 단말기는 시스템 결정 부 상태로 들어간다．1초 이내어］ 메시지를 받더라도 단말
  긴간삿昱한늪프론톳量7曜뽀혼（MO旦P－延攻F끄최굴인삿용하는 최손프론
  톤曼쓰쁘(1\小P프끄쁘크은볕 단말기는 사스템 결정 부 상태로 들어간
  다. 또한 PRAT 필드의 값이 단말기가 사용하는 프로토콜 개정번호（MOB_P_REV)
   어］ 의해서 예약되어 있는 경우에도 시스템 결정 상태로 돌아가게 퇸다．
       단말기는 I出毗을 획득하였으므로 Pilot어］ 실려오는 동기채널 정보를 복조하려고
  할 것이다. 이 채널 역시 IS 95에서는 Walsh채널 32번으로 고정하여 단말기가 초
   기단계에 32번 \N닒sh로 복조할 수 있게 미리 정해 두었다．
       동기채널은 단말기가 동작하는데 매우 중요한 정보가 있으므로 상대적으로
  C（月血g rate를 증가시킨 결과가 되는 1200bps로 전송되고 \Alalsh Code 32번으로
  수신한다. 이 동기채널은 Pilot 채널 획득을 통하1 맞춘 동기어］ 동기채널의 동기가
  맞추어져 있으므로 아무런 변동 없이 동기채널 메시지를 받을 수 있다. 시간적 관점
   에서 볼 때 Pilot 채널 주기의 시작점을 "Pilot PN ro끄over point"라고 한다.
       단말기가 Pu毗 채널을 수신한 다음 동기채널을 수신할 때 Pilot PN rollover
  帥nt에서 수신하게 된다. 즉 동기채널 메시지는 Pu毗 PN rollover point에서 시작
   되므로 복조의 기준점으로 사용한다. PN Code의 주기는 26.67ms이고 이것은 PN
  Short Ccx妃의 킬이가 되며, 이러한 3개의 Frame은 80ms로 1 super frame이 되며，
  이것은 CDMA시스템의 시스템 시간의 단위가 된다. 동기채널을 통해서 단말기가
  수신하는 정보들은 다음과 같다．
       므REV(pro加col revision level) - 현재 기지국이 서비스하고 있는 프로토콜의
   개정번호를 알려주며, 망은 이러한 정보를 자기의 서비스 영역어］ 들어온 단말기어］
   거］ 알려 주어서 어떠한 정도의 기지국인지를 알려준다. 이와 같이 기지국이 최소로
  지원할 수 있는 기지국의 프로토콜 개정번호인 八/llNPREV(minimum pr毗oc아
  revision level)도 같이 알려서 단말기의 MOB_P寸PEV과 조정하여 사용 가능한 프
  로토콜 개정번호를 사용할 수 있게 해준다．
       이러한 프로토콜 개정번호는 앝밭젖으론코으世늦I邑墮스곈옐이고포뽀奭꼐옇
  읕크흐등이 이어］ 해당된다· 최근어］ 서비스되고 있는 2.5세대망인 玗95C혹은
  玗2000（혹은 cdma2000）은흐坐坎1,프론톤골크정뽀호를 사용한다．
       또한 현재 단말기가 서비스받고 있는 망의 시스템 식별자인 SID(system

1. r:kt 쭈H '匕bn恤 ' 므｛e{1性   ‘   n   牛뇽t
                                    明邕 小六니 4:m 미a ,
              422                                                       8. IS-95 Call Flow
                     1                                                                       U



      identi如砒幻n）와 망 식별자인 l旺D(network identi如砒如n）를 표시하1 주어서 단말
      기가 올바르게 자신이 찾고 있는 망을 찾았는지를 확인시켜 준다. 이와 더불어서 해
      당 기지국의 끄峽量匙트量봇하여준다· 이 값은 앞서 Pilot 획득시어］ 결정된 값
      과 비교될 수 있을 것이다．
        가장 중요한 시간정보 수신은 LC_STATE(Long Code state), SYS_TIIVIE
      (system time), LP_SEC (leap second), LTM_OFF(offset of l兀al time) *1 9)
      다. 이러한 시스템 시간은 1980년의 첫 번째로 새로 시작하는 첫날인 1월6일 일요
      일 0시를기준으로PNSb.此Code와LongCod.를 시작하였4ii亘8叭'I屯의 대
      역폭으로 길이가 각각 242과 2巧인 되는 Long Code와 Short Code를 사용한다면 이
      것이 다시 만나서 1980년1월 6일 0시와 같은 상태, 즉 Long Code및 Short Code가
      같이 시작되는 상태가 되는 시점은 약 3700년이 지난 후에야 가능하다.
        여기서 이야기하고 있는 IS-95의 CDMA 시스템의 기준시간어］ 대한 시간경과어］
      따른 옵셋 정보를 동기채널로 수신하여 시간설정어］ 사용한다. 즉 LC小STATE는 시
      스템시간어］ 명시된 값을 Long Code의 상태로 이 필드를 표시한다. 이러한 Long
      Code는 앞으로 사용할 Long Code의 기준이 된다. SYSHT皿tIE은 시스템 시간을
      나타내며, LP_SEC는 시스템 시간이 시작한 이후 발생퇸 윤초의 수를 표시해주며，
      LTM_OFF는 시스템 시간과 지역시간의 차이를 나타내며, 현 지역 시간은 "SYSH
      TIME - LP_SEC + LTM_OFF"과 같다. 기지국은 이 필드를 30분 단위로 2의 보
      수형태어］ 이 필드로 설정한다．


                              년／월／일／시 MS SYNC CHANNEL messa解
                              Sync Channel Message
                                msgmtype : 1
                                仁rev : 5
                                 mml_p_rev : I
                                sid : 2190
                                nid : 17
                                pilot_pn : 384
                                Ic state : 0x488ea00c16
                                sys_ time : 0x1e2490ec2
山b' 執I) 吐이 U長                   Ip_sec : 13
                                ltm off: 18
                                daylt : 0
                                prat : 0 -> 9600bps
                                4 dma_freqfrequency assignment) : 575


                                         （그림 &2) 동기채널
 1 , 忖件忖D :    唯므4   ＼工＞ >.
    8. IS-95 Call Flow                                             거I
                                                             1,,m4231
口


 （그림 &2）는 동기채널의 실제 예이다. 이러한 동기채널은 고정 길이의 메시지 형
태로 다음과 같다．
 추가로 일광 절약 시간 표시자인 DAYLT(Daylight Savings Time）와 호출채널
의 데이티 율（PRAT）을 裝；00bps 또는 9600bps중 하나로 나타낸다．

     8.1.4 시간 변경 상태 : CDMA시스템과 동기를 맞춘다

 IS-弱는 동기식 CDMA의 Air규격이고, 이러한 동기식 CDMA방식에서는 동일
한 PN Code의 시간 옵셋을 사용하여 기지국간을 구별하게 된다. 따라서 시스템과
단말기가 동일한 시간으로 동기되어 있어야 한다. 이러한 시간이 system tin祀이며
단말기는 동기채널의 system time을 수신하여 내부 시간을 재조정하고, 이 값을 초
기값으로 하여 자체 발진소자로 시간을 계산한다. 즉 단말기는 자체 시계를 관리하
며 그 시계의 시간을 동기채널을 통해서 수신한 시간정보로 시계를 재설정한다．
 만약 단말기 내부적으로 恤ning이 어긋나게 되면 물리계층의 데이터 자체가 확실
하게 복조가 되지 않기 때문에 어떠한 정보도 수신할 수가 없다. 이것은 FM라디오
가 MBC주파수로 튜닝하1 놓고 KBS의 방송을 청취하려고 하는 것과 같은 이치가
된다. 이러한 System tim&은 기지국이 GPS(Global Positioning System) 위성정
보를 근거로 하여 단말기에게 제공된다.
 앞서 이야기 되었듯이 동기채널의 Frame은 26.67ms로 1개의 슈퍼 Frame이면서
시스템 시간의 단위가 되는 80ms내어］ 3개가 포함될 수 있다. 반면 통화채널이나 호

                                    동기 채널에서       정의된
                     26.67m         PN offset을 이용하여 수
       Zero Offsel
       의     파일럿     써 卜4e          신하는 메시지의 시작점


       rollover를
       보여주는 시
       스템 시간

                                                         p，可「Se
                                                             （니H
      동기 채널



                     H동기채널메시지니           H80m9니
                                                320 ms        IJ
                          （그림 8-3) 단말기 내부 타이밍
                                        8. IS-95 Call Flow
    424                                                 -U
 출채널의 Frame은 20ms로 4개가 80ms내에 포함될 것이다. 즉 현재 동기채널을 수
 신하여 시간 정보를 수신한 시점, 즉 시간을 확인한 시점이 이후어］ 복조하게 될 호
 출채널의 Frame과 정확하게 일치가 되지 않는다．
  따라서 동기채널과 호출채널의 Frame들이 같이 시작하는 시점까지 사간꼬연이
 있어야 한다. 그러므로 동기채널을 복조한 이후 그 슈퍼Fr帥e이 끝날 때까지 기다
 려야 한다. 이때 단말기는 수신한 시간정보를 가지고 자신이 지금 현재 어느 Frame
 의 시간적 위치어］ 있는 지를 가장 먼저 파악해야 할 것이다．.
  （그림 斗3）은 동기채널 메시지를 수신한 이후 단말기 내부적인 timing 도이다．
 26.67ms는 동기채널의 PN Short Code의 주기이며, 80ms는 동기채널의 슈퍼
 Frame이다．
  단말기는 동기채널 메시지를 수신한 후 내부적으로 관련 Parameter를 설정하고
 H/W를 제어한 다음 timing change를 수행한다. 이러한 동작을 위하여 충분한 시
 간인 4개의 슈퍼Fr8岫녀당하는4而勃 舡沁 따라서 단말기는유효한동
 기채널 메시지를 수신한 후 320노T1S 지난 뒤 호출채널 메시지 수신을 위해 timing
 change를 수행한다. 이때는 정리된 타이밍 정보를 가지고 Pilot 옵셋 등의 정보를
 가지고 해당 Pilot을 가지고 신호를 복조하게 된다．
  （그림 斗4）어］ 나타나 있듯이 단말기는 기지국으로부터 처음에는 Pu毗을 획득하
 기 위해서 local Pul毗 발생기어］ 의하써 P11毗을 찾고 이렇게 찾게 되면 동시어］ 동기
 채널을 복조할 수가 있게 된다. 즉 초기에 복조되는 동기채널은 타이밍 정보가 전혀
 없는 상태에서, 즉 P11야의 옵셋 정보가 없는 상태에서 찾게 된다. 이것은 시스템 시
 간정보가 아니라 기지국 신호정보에 의한 복조라고 할 수 있으며, zero offset어］ 의
 한 복조라고도 이야기할 수 있다．
  이렇게 찾은 후 복조퇸 동기채널을 통해서 시스템의 시간정보를 얻게 되면서 자
 신이 복조하고 있는 Pil야의 옵셋 정보를 규정할 수 있게 된다. 즉 이때는 단말기는
 시스템 시간정보로 자신이 가지고 있던 시간 정보들에게 옵셋을 가하1 줄 수 있게
 된다. 즉 시간을 새롭거］ 설정하게 된다．
  예를 들어서 무인도어］ 있던 로빈슨 크루소가 무인도에서 혼자만의 달력을 만들어
 서 각종 명절을 지내면서 잘 지내다가 구출되었을 때 그는 그의 모든 달력을 세상의
 달력과 시계에 다시 튜닝하게 될 것이다. 혼자 살기에는 혼자만의 달력으로 불편함
 이 없었으나 같이 살기에는 그러한 달력은 부적절하다.


\.m '4"如’ 斗m枷，,d용 .: 如年｝畔 如"力？
1
    8. IS-95 Call Flow
    小                                                                                      :L쯔；二1
                                                                                                   time


          Zero offset
          으로 복조한
          동조채널


                                      41+
                                                             동기 채널볼 포함한
                                      홍기 채널
                                                             최근의 슈퍼 프레임
          l寸on Zero                    프레임
          offset으로
          복조한 동기                                                  동기 채널 슈퍼 프레임 4개 +
          채널      +
                                                                  I   /\       I       I       I



                                                                      V
          호출 채널
          흑은 통화
          채널 ,.，느        1    i   i         1   I   :1   I    1            1       I   I   I
                             프레임 옵셋이 0이며， 임의의 파
                             일럿 옵셋으로 복조 되는 신호




                        （그림 &4) Forward CDMA 채널 P11아 PN 옵셋


    단말기도 망에서 독야청청할 수는 없으며, 다른 많은 단말기들과 같이 망을 인식
하고 있어야한다（한편으로는 망에 자신의 존재를 인식시켜야 한다）. 그러기 위해서
는 혼자만의 시간설정에서 모두 알고 있는 시간으로 설정하는 것이 필요하다. 우리
가 흔히 TV에서 볼 수 있는 전쟁영화 정면의 군사작전시어］ 작전개시에 앞서서 서
로의 시간을 맞추는 것과 같다．



    8.2     IdIe(Page) State 처리                                                                           )


    단말기는 여기어써 공부하게 될 대기상태어］ 머무는 시간이 일반적으로 가장 많게
되며, 이 기간은 단말기가 획득한 시스템어］ 대한 정보수집과 향후 상태 천이를 위한
준비를 하는 상태이다. 즉 단말기의 대기상태（k끄e st欲e）는 단말기가 자신이 지금
Serving 기지국으로 사용하고 있는 망의 상태를 파악하여 이동통신 서비스를 위한
환경조성 및 호출하는 전화를 받거나 전화통화를 시도할 수 있는 과정을 포함한다．
    단말기는 초기상태어］ 수신 복조된 동기채널에서 필요한 시간정보를 수신한 다음
망과의 통신을 위한 주파수 채널 선택 후 천이와 호출채널 및 Si毗 선택을 하여 하1
   426                                                                          8. IS-95 Cal l Flow
               1                                                                                      .


당 주파수 채널의 호출 Si야을 통하여 시스템 형상정보와 Access Parameter 정보
를 수신하고 갱신한다．


   8.2.1 Slotted Mode

 단말기어］ 표시되는 시간이 9시 뉴스시간어］ 제공되는 시보와 일치할까？ CDMA동
기식 시스템은 세상에서 가장 정확하다는 시각정보를 제공하는 GPS 위성을 통해서
시간을 제공받으니까 아마 일치할 것이다라고 생각하면 틀린 답이다. 물론 GPS로
부터 제공받는 시간정보를 가지고 단말기와 기지국이 통신하는 기준시간을 맞추어
서 사용한다. 그렇다면 왜 아닌지를 설명하겠다．

                                             Unit Slot Cycle

                                               늬 [q1
         1 I 1 I                                                                       1
         0         1   2        3                                                      2




         누叫1               1.   28 sec     11141     1.   28 sec

         I I IHIH                         I IHHI IH                        HI          1
         0 1 2 3 4 5 6 7 ... 1415 0 1 2 3 4 5 6 7 ... 1415                            2047




                                                          /\
                                                          띠H80 ms-b




                                         （그림 &5) 호출 듸아의 구성

                                                                   gby小O
 호출긔
   '널은호출긔
        '널SbO따부르는＼聊沙lot으로분할되며， "］러한Slot들은
특정한 단말기가 호출채녈을 감시하는 단위가 된다. 즉 단말기가 호출채널을 감시
하기 위해서 살아 있는 8C住ns 이외의 시간 동안은 단말기가 전력을 save할 수 있다．
그러나 이러한 Si야 Mode가 아닌 n이r없毗 入4ode로 동작할 때는 단말기는 항상 살
아 있으므로 전력을 save 할 수 없으나 모든 없ot을 감시할 수 있는 이점이 있다．
 Slot 八Tode로 동작하고 있는 단말기는 하나 혹은 두 개의 Slot Cycle 동안 호출
채널을 감시 할 수 있으며, registratio可origin毗ion/page response Message에서
    8. IS-95 Call Flow                                           427
.

단말기는 자신이 선취 하고 있는 Si야 Cycle을 규정한다. 80ms 킬이의 Slot이 16개
인 1.28 ms를 단위로 하는 Si毗 Cycle T는 2SLOT中CYCLE工江犯x 이다． 즉
SLOT_CYCLE皿口）EX가 1인 Slot Cycle T는 다음과 같다．

          T =1.28 sec[or 16 slot]x 2Sim-CrC1-!NL)EC               (8-1)

    위의 식에 의해서 SLOT_CYCLE皿DEX는0에서 7까지 있으므로 호출채널의
최소 Si毗 Cycle T는 20인 '1'로 1.28 sec(16 Slot)와 최대 Slot Cycled은 1.28
sec(16 Slot) X27 이다．
    玗95어］근거한 CDMA의 호출채널의 경우어］ 128口7)개의 호출채널 Cycle을 가
지고 있으며, 이러한 호출채널 Cycle은 16개의 Sl야으로 구성되어 있으므로， 모두
2048개의 Sl毗을 가지고 있다．
    일반적으로 한국의 이동통신 회사들은 Slot 八4ode를 2로 사용하며, 이 값은 업체
마다 다르게 운용할 수도 있다. 각각의 Si毗 Cycle Index어］ 따른 검색주기는 다음
의 ＜표 斗1＞과 같다．
    즉 망에서는 최소한 1.28sec마다 새로운 정보를 갱신해 주어야 한다는 것이다. 그
렇게 되면 51야 Cycle Index가 "0" 인 단말기는 갱신되는 신호를 효과적으로 받을
수 있으나, 나머지 Index로 동작되는 단말기는 어느 정도의 지연이 있은 후어］ 메시
지를 수신하게 될 것이다. 또한 non SbO仇出 Mode로 동작하는 단말기는 똑같은 메
시지를 16번 중복해서 받는 경우가 발생된다．


                         （표 8-1) Slot Cycle Index에 따른 검색주기

              Slot Cycle Index                        검색주기佃ec)
                         0                              1.28
                         1                               2.56
                         2                              5.12
                         3                              10.24
                         4                              20.48
                         5                              40.96
                         6                              81.92
                         7                              163.84
   428                                   8. IS-95 Call Flow
                                                              1


 어찌 되었든 단말기가 non Slotted 入4ode로 동작할 때는 단말기가 망으로부터 필
요한 정보를 얻기 위해서 사용하는 방법으로는 적합한 방법이라고는 할 수 없다. 때
문어］ 우리는 non Slotted Mode 단말기가 동작한다는 것은 단말기 자체의 문제를
해결하기 위한 방안, 이를테면 단말기가 망을 놓쳤다던가 해서 현재 정상적인 idle
상태가 아닐 때와 같은 때에 필요한 Mode일 것이다．
 여기어囚 주의할 것은 "SLOT_CYCLE皿口）EX가 '0'인 경우와 non Slot Mode
와는 다르다”는 것이다. 전자의 경우 단말기는 1.28초마다 80ms만 깨어나서 호출
채널 을 감시하는 반면 후자의 경우는 늘 깨어 호출채널 을 감시하는 것으로 non
Slot 八4（넜e가 SLOT_CYCLE_INDEX가 '0' 인 경우보다 16배 빠른 호출채널 감시
를 수행한다．
 그럼 처음의 문제어］ 대한 답으로 돌아가자 !
 단말기는 Power Save를 위해서 ii:兀E상태에서 위에서 언급한 것과 같이 특정한
시간에 만 깨어나는 Slot 入4ode로 동작하는 것이 일반적이다. 예를 들어서 Slot 2
Mode로 설정되어 있는 경우, Si야 2 八4ode의 한 주기는 5.12초이며, 호출채널 탐색
을 위해서 깨어 있는 시간은 80ms이다. 단말기에서 시간표시는 단말기가 호출채널
을 탐색하기 위해서 Sleep에서 깨어나 있는 동안어］ PCS폰 화면상의 I玉splay가 갱
신된다. 결과적으로 단말기가 호출채널을 탐색하기 위해서 Sleep에서 깨어나는 주
기인 Si야 Cyc把과 관계된다. 이때는 5.12초마다 한 번씩 시간이 바뀌는 것이 되며,
이것은 또한 시간표시의 최대 오차가 약 5초라는 것을 말한다. 이러한 것은 단말기
가 GPS로 수신한 시간을 자체 Clock으로 아주 정확한 시간을 가지고 일련의 처리
를 수행하지만 표시는 그렇게 하지 않는다는 것이다．
 또한 5초마다 한 번씩 돌아오는 단말기의 시간표시 기능이 단말기가 깨어 있는
80ms동안어］ 단말기의 수많은 다른 기능의 우선 순위어］ 밀려서 LCI）화면어］ 갱신퇸
시간표시가 실행되지 않는 경우도 시간이 정확하게 표시가 되지 않는 이유가 될 것
이다. 만약 단말기가 시간을 표시하는 기능이 최우선인 시계라면 아마 그렇지 않을
것이다. 정리하면 단말기어］ 표시퇸 시간은 51毗 Cycle의 정수배, 즉 5.12N초 이상의
오차를 나타낼 것이라고 생각할 수 있다.
 이상의 2가지의 이유로 단말기어］ 표시되는 시간이 일반 시계와 다를 수 있다. 그
러나 이렇게 시간이 틀리더라도 단말기 내의 Clock은 아주 정확하게 시간을 가리키
고 있다．
    8. IS寸95 Call F幻w
1

     8.2.2 호출채널 Monitor

    단말기는 초기상태에서 대기상태로 진입하면서 단말기어］ 이미 저장되어 있는
Primary 채널의 Prim可y 호출채널, 즉 \Va1sh Code 打로 변조되어 전송되는
CDMA Channel List 八lessage를 수신하여 현재 서비스받고 있는 기지국에서 제
공（출력）되고 있는 주파수 자원 중에서 단말기에 할당된 해당 주파수 채널
(Frequency Assignment）로 천이하게 된다. 이때 단말기의 전화번호（Nffl           :
Iv［아血e Identification Number）와 채널 list를 가지고 hashing하여 서비스 받을 주
파수 채널（FA）을 결정한다．
    서비스 주파수 채널로 이동한 단말기는 그 주파수 채널 가운데 Primary 호출채
널로 이동하여서 서비스받고 있는 기지국의 정보를 System Parameter Message
로 수신하고 그것의 내용 중 PAG且CHAN을 통해서 호출채널 범위에서 최대 호출
채널어］ 근거하여 호출채널 번호를 결정한다. 또한 실지로 단말기에게 부여된 호출
Si毗번호도 비슷한 방법으로 결정한다．
    이러한 호출채널 번호, Si야번호 및 사용 주파수 결정에는 뒤어］ 언급된다（이것은
자원을 균등하게 분배하기 위해서 사용되는 Hash 함수이다）.
    이렇듯 단말기가 정상적으로 대기상태어］ 진입하게 되면 앞서 이야기되었던
Slotted Mode혹은 non Slotted Mode로 망에서 내려오는 호출채널을 감시하게 된
다. 이러한 감시방법은 단말기어］ 미리 설정되어져 있는 N小I값 중 SCM(Station
Class M可k）어］ 의하써 결정되어 호출채널을 감시한다.
    만약 단말기가 정상적으로 대기상태에 머물지 못한다면, 단말기는 System
Parameter Message어］ 포함되어 있는 八4A乂SLOT_CYCLE上띠DEX와 '1' 중 작
은 값으로 읾otted 八lode를 결정하여 망을 감시한다.
    단말기가 호출채널 메시지 검색어］ 실패할 경우 다시 초기화 과정부터 시작하여야
한다. 이의 기준은 읾otted Mode와 non Slotted Mode가 다르게 적용된다. 욜lo旦gl
Mode인 경우는 정해진 Si毗 검색 시점에서 3초 동안 Frame어］ 오류가 있으면 초기
화 과정부터 시작하고, non Slotted 八4ode인 경우는 Frame 오류가 없는 Frame의
다음부터 3초 내어］ Frame 오류가 발생하는 경우 초기화 과정부터 다시 시작한다．
    Page Channel Message에서 3초 동안 valid Frame（오류가 없는 Frame）이 아닐
경우 초기화부터 다시 시작한다．
    430                                                      8. lS小95 Call Flow
                                                                                  .


                          （표 &2) Station （긔ass Mark

             Function            Bit(s)                    Setting
                                           Band Class0               아(XXXXXX
 Extended SCM Indicator            7
                                           Band Classi               1xxxxxxx
                                           CI呱4A only                x0xxxxxx
 Dual Mode                         6
                                           I允ai Mode                 x1xxxxxx
                                           Non-Si예ed                 xx0xxxxx
 Slotted Class                     5
                                           Slotted                   xx1xxxxx
 IS-54 Power Class                 4       항상 0                      xxx0xxxx
 25M也 Bandwidth                    3       항상 1                      xxxx1xxx
                                           Continuous                xxxxx0xx
 Transmission                      2
                                           Discontinuous             xxxxx1xx
                                           Class I                   xxxxxx00
 Power class for Band Class                Class II                  XXX)(XX01
                                  小1
 0 Analog Operation                        Class 皿                   xxxxxx10
                                           Reserved                  XX)OO(X11


 시스템 접속일 경우에도 Page Channel Message를 검색해야 하며 이때의 시간
기준은 1초이다. 즉 1초 동안 Frame어］ 오류가 있으면 시스템 접속을 중지하고 대기
상태(idle state）로 전환한다．
 Si毗 주기와 검색시점은 다음과 같은 식으로 산출된다．

          U仕PGSLOT)mo如xT)=0                                                (8- 2)


 여기에서 t는 System time, PGSLOT는 hashing어］ 의해서 구해진 Slot number
이고 L 兀J 는 x의 계산결과에서 소수점 이하를 버린 값이란 뜻이다. 또 T는 T=2i
로 1는 slot cycle ir넌ex이다．
 여기서 말하는 System time은 80ms 단위로 l叩date되고 호출채널은 20ms 단위
이므로 System time을 4로 나눈 값으로 설정된다. 그리고 Si毗 번호는                              [ t/4 i
mod 2048로 결정되므로 단말기는 쉽게 인식할 수 있다. (bottom down을 나타내는
 L 兀 ] ）는 소수점 이하를 버리는 것으로 깨어나야 할 시간과는 최대한 멀리 설정하
기 위해서이다． 예를 들면 (5220.陌ms）는 52520ms로 계산된다．
    8. IS-95 Call Flow                                 431
.


    Slot Cycle Index 값은 단말기의 EEPRO呱NAM 프로그램밍으로 입력）에도 저
장되어 있고， 호출채널의 시스템 Parameter 메시지에는 최태 Si毗 cycle Index를
포함하며， 단말기는 시스템에서 수신한 Si毗 Cycle Index 값과 저장된 값 중 작은
값으로 동작한다．
    Sl毗 Cycle Index 값은 망의 입장에서는 대기상태에 전송할 데이터의 양과 연관
이 있다. 즉 전송할 데이터가 많다면 단말기가 더욱 빈번하게 깨어나서 호출채널을
감시해 주어야 할 것이다. 이런 의미에서 망에서 이러한 Slot Cycle Index 값을 조
정할 수 있는 여지가 필요한 것이다.
    또한 단말기 입장에서 본 Sl毗 Cycle Index는 단말기의 소모전력과 연관퇸다. 자
주 깨어나게 되면 단말기는 대기상태어］ 더욱 많은 전력을 소모하게 될 것이다. 또한
얼마나 빨리 착신신호를 수신할 수 있는지에도 연관된다. 이러한 기타 등등의 이유
로 단말기에서도 위에서 이야기한 것같이 Si야 Cycle Jr넌ex을 제어하기 위해서 영
구 메모리에 저장하1 둔다．
    결국 단말기와 망과의 이러한 이해콴계의 합일점을 CDMA시스템에서는 2가지의
값 중에서 작은 값으로 하는 것으로 결정하여 운영하고 있다. 실지로 국내 망에서는
IS-95C 이전 단계에서는 말과 단말기가 합의한 Sl毗 Cycle Index 는 "2"로 사용하
였으나, IS-弱C가 되면서 Overhead Message의 크기가 증가하였고 메시지의 종류
도 증가하여 기존의 Sl毗 Cycle Index 2로는 그러한 모튼 메시지들을 처리하기가
어려움으로 망에서 SPM를 통해서 MAXeSLOT小CYCLE을 1로 전송하여 사용
Sl毗 Cycle Index를 1로 설정하여 사용한다．

     8.2.3 Overhead Messages update

    호출채널 구조는 앞장에서 설명되었듯이 l0ms의 Half Fra毗(full Fran祀＝20ms)
이 8개가 되어 호출채널 Si毗이 퇸다． Page Channel Message의 시작점은
SCI(Sync뇨onized Capsu把 Indicator) Bit를 기준으로 설정된다. SCI값이 '1'일 경
우는 새로운 Page Channel Message가 시작되고 '0'인 경우는 연속적인 메시지를
의미한다．
    만약 Half Frame을 단위로 Page Channel Message capsule이 설정될 경우는
"Synci寸이iized capsule"이라 하고, 임의의 Half Frame어］ Capsule이 설정될 경우
는 "Unsynci끄7onized capsule"이라 한다．
    432                                               8. IS-95 Call Flow
                                                                           .

 하나의 Page Channel Message Capsu1e은 Page Channel Message와 padding
으로 구성되며 하나의 Page Channel Message는 Message 길이, Message 몸체，
CRC로 구성된다. 여기에서 실제적인 메시지는 Message 몸체에 들어 있다. 구체적
인 구조는 7장을 상기하라！
 Page Channel Message는 시스템 정보전송, 호출정보, 채널정보, 인증요구 등의
메시지가 전송된다. 즉 호출채널은 시스템의 모든 상태가 전송되며 이러한 것들은
단말기가 시스템에 접속하기 위해서, 시스템에서 단말기를 관리하기 위해서 필요
한 정보들이라고 할 수 있다. 이 정보는 단말기의 이동 혹은 기지국 상황의 변동 등
에 의해서 값이 변할 때마다 단말기는 자신이 가지고 있는 값과 비교하여 갱신한다.
 Page Channel Message는 크거］ 전체 단말기가 수신하는 overhead Message와
각각의 단말기별（address field type으로 구분） 또는 특정 그룹의 단말기로 전송되
는 小rected 入4essage로 구분된다. 메시지어］ 공통적으로 포함되는 Address type은
다음의 표와 같다．


                          K표． 8-3) Address Type
          향목                   ADDR TYPE              ADDR LEN（옥텟）
        IMSI_S                      000                     5
         ESN                        001                     4
         IMSI                       010                   E5N7
         TMSI                       011                   2 싸 12
      BROANCAST                     101                    가변
          예약                   110, 100, 111


  시스템에서 호출채널을 통하여 전화호출, 인증요구, SMS 수신 등을 요구할 때는
각각의 단말기별로 행해진다. 이때 각 단말기를 구분하는 방법은 전화번호小IF나 :
Moble Indentification Number), ESN(Electronic Serial Number), 皿4SI(Inter
national 八4야血e Station Indentity), BROAI)CAST로 구분하여 사용하는데 이들
을 address type이라고 한다. 실제로 전화번호인 入41N은 IMSI어］ 포함되며 별도로
사용하는 이유는 MIN으로만 동작하는 기존의 단말기를 보호（9）하기 위해서이다．
  즉, 망에서 단말기를 호출할 때, 단말기 구분은 전화번호, ESN 등을 이용할 수
있다. 여기서는 八IN 혹은 皿4S1로 해도 상관없다. 入皿N과 IMSI는 망식별번호, 나
U
      8. lS-95 Call Flow
                                                             433
                                                                   I
라번호 등과 같이 좀더 넓은 의미의 식별정보를 포함하기 때문이며, 물론 IMSI에는
MIN을 포함하고 있다. 현재 대부분의 이동통시 업체득우 호춤의 경우 전학번古를
사용한다. BROADCAST는 SMS에서 방송용 메시지（cell broadcasting）를 전송하
는 address type이다. 이러한 address type은 Traffic state에서는 어떠한 address
type도 사용하지 않는다. 이것은 통화로가 열리게 되면, 통화로를 통해서 매시간 전
송되는 데이터들이 관리가 되고 있기 때문이다．
      이와 같이 생각할 때 예약되어있는 address type을 별도로 정의하여서 그러한
address ty光의 정보를 가지고 있는 단말기군이 있다면 특정한 단말기군 혹은 사용
자군을 형성하여 별도의 서비스를 제공할 수 있는 방법이 될 수도 있다．

 小；
                 동일한 전화번호를 저장하고 있으나 서로 다른 ESN을 사용하는 단
                 말기가 있을 때 망에서 전화번호로 호출한다면 전화기는 벨이 울릴
                 것인가？ 물론 한 대는 정상적으로 개통되어 있는 상태이나 나머지는
                 전화번호만을 저장한 상태이다．

                 전화벨은 한 대만 울린다. 전화벨이 울리는 시점은 통화채널이 완전
                 히 열린 상태이다. 물론 개통되지 않은 단말기도 호출어］ 응할 것이다．
                 그러나 호출어］ 응하는 Page Res 단계에서 ESN과 瓜'IS'를 대조하는
                 일종의 인증단계에서 거절당하기 때문에 호를 열수가 없다．
      호출채널 메시지 중에는 실제로 특정한 단말기가 아니라 모두 단말기가 수신하게
되는 방송개념의 overhead Message가 있다. 이것은 크게 현재 망의 형상과 관련된
Parameter를 전송해 주는 메시지와 망 접속시어］ 필요한 Parameter를 명시하1 주는
메시지들로 구분될 수 있다．
 \Configuration Parameter분 System Parameter, Neighbor List Message,
CDMA Channel List Message, Extended System Parameter Message, Global
서비스 Redirection 八/Iessage 등이며, 이것틀은 단말기에서 형상 정보 일련번호를
관리함으로 올바른 형상정보를 갱신하게 한다. 또한 /\ccess Parameter는 /\ccess
Parameter Message에서 제공되며, 이것 역시 /\ccess 형상 정보 일련번호를 통해
서 관리된다. 이 두 가지의 일련번호는 modulo 64로 관리퇸다．
      단말기는 이러한 메시지의 감시를 하나의 기지국어］ 대해서만 이루어지고 동시어］
2개 이상의 정보수신은 하지 않는다. 따라서 단말기가 수신한 Pilot 옵셋인
P凡OT_PNr 필드가 감시중인 호출채널의 Pilot 옵셋（PILOT_PNs) 단말기에 현재
            434                                       8. IS-95 Call Flow
                                                                           .


       저장되어 있는 Pilot 옵셋）와 같지 않은 임의의 메시지들은 무시한다．
        저장된 구성 메시지 일련번호（시스템 Parameter, 채널목록, 확장형 시스템
       Parameter, 서비스 방향설정 메시지의 일련번호）가 형상정보 메시지 일련번호
       (CONFIG_ 八4SG_SEQ）가 N띠1이 아니면서 같을 경우 그리고 단말기가 Parameter
       저장을 위해서 호출채널로 유효한 메시지를 최종적으로 수신한지가 Parameter 값
       들이 유효하다고 생각할 수 있는 최대 시간인 600초 이내일 때 단말기는 저장된 구
       성 Parameter가 현재 값이라고 간주하고 수신퇸 메시지를 처리한다．
        半 단말기가 각 호출 없ot에서 검색한 overhead Message의 데이터를 처리하는
          방법을 정리하면 다음과 같다．
        木 단말기는 모튼 Configuration Parameter 八/Iessage들어］ 들어 있는 Configura
            tion sequence number인 CONFIG小'ISG_SEQ를 검색하여 최근의 값보다 최
            신의 것이면 갱신하고 그렇지 않으면 무시한다. 이것은 /\ccess Parameter
            八/Iessage의 메시지 수신 시에도 마찬가지로 ACC小/ISG_SEQ를 사용하여 동
            일한 방법으로 처리한다．
        米 모튼 overhead Message에는 PILOT1PN이 전송되며 단말기는 이 PThOT
          PN이 동기채널에서 수신한 PThOTPN과 다를 경우 해당 overhead 八4essage
          를 무시한다.
        System Parameter Message는 시스템의 정보가 전송되며 등록, 전력제어，
       Handoff 등의 Parameter와 Extended System Parameter 등과 같은 추가 전송 머］
       시지들의 전송 여부 혹은 사용 여부를 표시한다. 또한 단말기가 없otted 八4ode로 동
       작하지 못할 때 망에서 제안하는 MAx_SLOT_CYCLE_il나DEX값 등도 포함되어
       있다．
        시스템 Parameter 메시지어］ 규정된 호출채널의 전체 수（PAG:巳CHAN）가 단말
       기가 저장하고 있는 값과 다르다면 새롭게 수신된 호출채녈 가운데에서 하나를 선
       택해야 한다. 이렇게 정해진 호출채널을 단말기는 저장하고 /\ccess Parameter 일
      ／少／         NULL로 설정하여 새롭게 시작한다·
///               「｝말기 7f: 1]롭게 '］스템부상태로천' ］되어 ' ］스템부상태로부터 ' 귀롭
                   하기 위해서 시스템 Parameter에 RESCAN뇔드들 enable시긴다．
                    :st Message는 overhead Message의 일종으로 현재 서비스받고 있는
                    ＼지국의 PN offset값과 그 기지국들의 형상정보를 전송한다. 이러한
    8. IS-95 Call Flow
U

형상정보는 단순히 Hando侄를 위한 간략한 정보, 즉 망 자원능력어］ 대한 정보들로
상세한 정보는 그 기지국의 System Parameter Message 등과 같이 상세한 정보
메시지를 수신할 수 있는 상황에서 그 메시지들을 수신하여야 한다. 따라서 단말기
는 이 메시지를 이용하여 Hando珏를 하기 위한 사전정보를 획득하게 퇸다．
 여기에서 PILOT_I寸C는 PILOT_PN offset의 증가 폭을 나타낸다. 이것은 인접
한 기지국에서 출력된 신호와 서비스를 받고 있는 기지국의 신호가 경로 지연으로
인하여 동일한 신호로 오인될 수 있는 것을 방지하기 위해서 할당하는 값이다. 이
값은 2, 4 등의 값들이 실지로 운용하는 망에서 사용된다．
 Access Parameter Message는 망에서 단말기가 망에 접속할 때 필요한
Parameter 혹은 값들을 정의해 주는 역할을 하며, 단말기는 이러한 정보를 수신할
때 일련번호를 관리함으로 가장 최근의 정보로 항상 유지하고 있어야 한다. 때문어］
이것의 일련번호는 시스템의 형상정보 일련번호와 더불어서 상당히 중요하게 관리
되어야 한다．
 CI呱4A Channel List Message는 이 메시지를 송출하는 기지국이 출력하고 있
는 서비스 채널（FA）을 나타낸다. 이 값들은 단말기가 서비스 주파수 채널을 찾을
때 사용되며, 이것들 중에서 하나의 주파수를 단말기를 선택하게 된다．
 Extended System Parameter Message는 System Parameter Message를 확장
한 개념으로 단말기의 preferred type과 cell broadcasting을 위한 호출채널 방송정
보 검색주기（broadcast Index）가 전송된다．


                             K표 8-4) Preferred MSID Type

     USE TMSI            PREF MSID TYPE                    설명
         0                     00           IMSI_S와 ESN
         0                     10           rMSI
         0                     11           IMSI와 ESN
         1                     10           할당된 呱4Sf가 vaild하면, TMSI
                                            할당된 呱4Sf가 vaild하면, TMSI
         1                     11
                                            TMSI가 할당되지 않았으면 皿4S1와 ESN



 또한 새로운 시스템 형상과 관련된 이를테면 /\ccess Han面妊관련 Parameter들
과 이와 연관퇸 Ec/l0 등의 정보, New MASHO 등의 Parameter도 함께 전송된다．
   436                                      8. IS-95 Call Flow
         r                                                       1


또한 Back ward compat小小ty를 위해서 동기채널로 전송된 Prot兀ol 개정번호를
다시 표시할 수 있다. 예를 들어서, 95B(P_REV=5）을 95C（므REV=6）로 업그레이
드중이라면, 95B망과 95C망이 같이 존재할 때 Sync Message에는 므REV을 5로
설정하고, ESP八'1에는 6으로 설정할 수 있는 방법이 있을 것이다．
 Broadcast Index는 단말기가 주기적으로 검색해야 할 Si毗 외어］ 방송용 정보를
수신할 때는 추가적으로 방송용 읾ot를 검색하햐 한다. 물론 이러한 단말기는 배터
리가 많이 소모되어 사용시간이 단축된다.


   8.2.4 Page Match Operation

 단말기는 대기（Idle）상태에서 앞서 공부한 overhead Message들을 수신하여 그
것이 내려주는 시스템 형상 정보와 망어］ Access 하기어］ 필요한 정보를 수신하여 단
말기가 저장하고 있으며, 또한 이어서 이 절에서 이야기할 명령 메시지와 이에 대한
응답처리와 더불어서 Page Match동작을 수행한다．
 Page 入hatch 단말기가 General Page 八hessage를 수신하게 될 때마다 수행하는
절차이다. 단말기는 그 메시지어］ 자신에게 할당된 瓜'IS' 또는 呱4S1가 포함되어 있는
지의 여부를 결정하기 위해서 각 메시지를 탐색한다. 이때 General page 八'lessage어］
포함된 정보가 탐색하던 단말기로 배달되는 정보라면, 단말기는 /\ccess 채널상으로
그 호출 메시지에 대한 Page Response Message를 전송한다．
 이것은 PAGE_CLASS와 PAGE_SUBCLASS의 값어］ 의해서 그것을 호출하는
IMSI, TMIS의 형태가 확인되어서 메시지의 내용어］ 대한 이후 이루어지는 동작이
확실해진다면 단말기는 Page 八'latch를 선언한다. 단말기는 이때 형상정보의 일련
번호（COI旺江G小'ISG寸SEQ）와 /\ccess Parameter 메시지 일련번호（ACC소4SG
SEQ）를 비교하여 일치하지 않으면 새로운 것으로 갱신한다. 즉 최신의 정보를 항
상 유지하겠다는 것이다．
 Page Match가 선언되면, 단말기는 호출 메시지를 수신한 후 단말기가 Page
Response Message로 응답하는 System Access 상태（정확히 皿：date overhead
Jr伽rn追tion부 상태）로 들어가며, 이러한 동작은 아무리 길어도 0.3초（T芻m) 이내어］
이루어져야 한다. Page match는 이러한 일련의 동작들을 말하며, 달리 표현하면 망
에서 단말기를 호출했을 때 그 호출어］ 부합되는 행동을 할 수 있다. 혹은 한다는 의
미일 것이다．
     8. IS-95 Call Flow
 1                                                                             437


      8.2.5 Broadcast Slot Monitoring

     Broadcast는 모든 단말기어］ 방송하는 형태로 호출채널의 data burst 入4essage를
이용하여 전송한다. 이 방식은 말 그대로의 의미로 볼 때 대기상태에서 망으로부터
호출채널을 이용하여 내려오는 모든 메시지들은 방송형이라고 말할 수 있겠으나
여기에서는 시스템 정보를 담고 있는 방송형이 아니라 부가서비스 형태 혹은
Application의 관점으로 이해해야 할 것이다. 물론 그러한 방송채널을 이용하여 어
떠한 부가서비스를 하고 있는지에 대한 이야기를 하려고 하는 것은 아니다．
 Broadcast Message는 호출채널과 Broadcasting Control 채널로 전송되며,
八4ult卜없야 Broadcast Message Tran帥小前on과 Periodic Broadcast 호출 의 2가
지방법으로 전송된다. 여기에서는 현재 사용되고 있지 않는 Broadcasting Control
채널로 전송되는 방송 메시지 전송 방법어］ 대해서는 거론하지 않겠다．
 각각의 방법은 방송형 메시지를 수신하기 위해서 slotted Mode혹은 Non-없야扼d
Mode로 동작하는 단말기에게 메시지를 전달한다. 호출채널상의 방송형 메시지는 방
송 address type을 가지는 data burst message이다. 읾otted Mode로 동작하는 단
말기는 호출채널 메시지를 수신하기 위해서 그것을 감시하는 별도의 없야이 할당된다．
 방송헝 호출은 방송형 address type을 가지는 general page message내의 recede
이다. 기지국은 앞서 결정된 일련의 없ot내에 전송되어질 것인 방송형 메시지인 그
si야을 감시하는 단말기에게 알려 주기 위해서 할당된 Si毗내에 방송호출을 전송할
것이다. 방송호출 이나 방송 메시지를 수신하기 위해서 단말기가 감시하는 Si야은
방송 Si毗으로 불려진다．


 다중 Slot 방송 전송방식
 이 방식은 Sl야 모드로 동작하고 있는 모튼 단말기들에게 Si毗의 구분없이 한번 순
간적으로 뿌려주는 방식이다. 이러한 이유들로 인해서 특수한 용도로 사용될 수 있다．
                                                       방송정보묠       가지고있뇬
                                                       data burst Messa只C는 ;
                                     7\
                                                       16 가四i 연속적 인 slot에
                                                       서 전송뙨다．




                /
        호출 채널 Slot            1.
                                   28초（16개Slot)   -늬
                          （그림 &6) 다중 Slot 방송 메시지 전송
                                                              8. IS-95 Call Flow
  438                                                                              a



 주기적 방송 호출 방식
 이 방법어］ 의하면, 단말기는 방송 메시지를 수신하기 위해서 상술된 방송 Si毗을
감시한다. 주기적인 방송호출 방식은 2가지로 방송 메시지를 전송한다. 모튼 메시지
가 방송호출 사이클의 첫 번째 si야내에 알맞게 전송퇸다면, 그것들은 이 방송 Slot
의 모든 전송일 것이다. 만약 단일 방송 메시지가 전송된다면, 그것은 이 방송 Slot
내에 전송을 시작할 것이다．
 또 다른 방법은 하나 혹은 그 이상의 방송호출이 방송호출 사이클의 첫 번째 사
이클 내에 전송될 것이다．
 각 방송호출은 연속적인 방송Si毗과 관련되어진다. 각각의 방송호출을 위하여, 관
련된 방송 메시지는 관련된 연속적인 방송 Slot어］ 전송될 것이다. 관련된 방송 메시
지의 방송Si毗은 방송호출 사이클의 첫 번째 없ot내의 GPM 전송내의 방송호출의
위치어］ 따라서 결정퇸다．



                                                                       33 34




        BroadcastBroadcastBroadcast   Broadcast Broadcast Broadcast
        Page #1   Page #2   Page #3    Msg #1    Msg #2    Msg #3

                    （그림 &7) Period匕 Broadcast 호출의 예



 （그림 斗7）은 방송 인덱스가 1로 설정된 주기 방송호출이다．
 GI丕4은 방송호출 사이클의 첫 번째 없毗으로 전송되는 3개의 방송호출을 포함한
다. 3개의 방송호출 각각을 위해서 DBM는 연속적인 Si毗내에서 전송된다．

 Slot 검색
 망은 단말기가 slotted mode로 동작하게 하기 위하써 2가지 종류의 slot ii닌ex를
전송한다. 하나는 앞서 이야기한 MAX_SLOT尸CYCLE工＼JDEX이고 또 다른 하나
는 BCAST皿寸DEX라는 방송형 메시지의 탐색을 위한 si毗 cycle정보이다. I光riodic
         8. IS-95 Call Flow
     1                                                     439


broadcast 호출방식으로 방송 메시지를 전송하는 경우에는 BCAST皿n死X를 근
거로 하여 주기적으로 단말기는 호출채널을 감시하게 된다．
         이것은 MAX나SLOT_CYCLE_H口）EX가 결국 시스템 정보일 수 있다는 측면
에서 시스템 Parameter 메시지에 포함되어 있었듯이 BCAST_INDEX(Broadcast
Monitoring Cycle）는 Extended System Parameter 入4essage어］서 포함되어 있
다．
     Broadcast Slot 주기는 다음의 식과 같이 나타낼 수 있다．

               B= 21x16, (05i57) i: BCAST그ND月x              他3)
         또한 Broadcast Sl야을 검색하는 시점은 임의의 호출채널에서 다음과 같다．

               U伽如*3), t:S少招m作me                            (8- 4)

     Broadcast Message를 처리하는 단말기는 고유의 검색 Sl야과는 별도로 broad
cast Sl야을 검색해야 한다. 이 경우어］ 추가적인 메시지를 수신하기 위해서 별도로
깨어나는 시간과 빈도가 증가함으로 배터리 소모량은 증가하게 될 것이다．
     일반적으로 BCAST工日DEX는 보통 5 이상을 할당하여 검색주기를 길게 한다．
이것은 일반적인 호출채널로 전송되는 호출을 포함한 overhead message정보들어］
비해서 방송채널로 전송되는 정보의 내용으로 볼 때 신속히 처리한다는 입장에서
보면 방송형이 상대적으로 낮은 점수를 받기 때문이다. 또한 방송 메시지의 갱신 빈
도보다는 일반적인 호출채널 메시지들의 갱신 빈도가 높기 때문어］ 검색주기를 길게
한디－.
     만약 일반 호출채널의 Slot Cycle Index가 2이고 Broadcast Monitoring Cycle
Index가 6일 때 이것의 구체적인 값을 （표 &1> S1야 Cycle Index어］ 따른 검색주
기에서 확인해 보면 방송탐색은 일반 호출채널 탐색이 16번 일어날 때 한번 일어나
게 된다. 밧뎨리 소모를 가지고 이야기한다면 기존보다는 약 6.25% 정도 더 소모될
것이다. 여기에서 주의해야 할 중요한 사항 한 가지 이상의 시나리오로 진행된다면
항상 방송채널은 일반 호출채널 탐색과 같은 시간어］ 이루어진다는 문제가 생기게
된다. 즉 그때는 방송 메시지로 인해서 다른 메시지들의 복조를 할 수 없을 수도 있
다는 이야기이다. 때문어］ 식 &4에서 나타난 것과 같이 3이라는 옵셋을 설정하게
된 것이다．
I    440
                                                                  8. IS-95 Call Flow



    8.2.6 （沁ick 호출채널

 앞서서 이야기된 단말기의 Slotted 入Iode는 단말기의 대기시간을 불연속적으로
하여 단말기의 전원을 Save하자는데 그 목적이 있다. 이 절에서 공부하게 될 伽ick
호출채널（QPCI引은 단말기의 대기시간을 향상시키기 위한 새로운 방식으로 IS-95C
에서 새롭게 제안된 Physical 채널이다. 단말기는 이 채널을 통해서 호출 Indica加rs
와 Configuration Change Indica切rs를 감시한다．
 QPCH는 QPCH 읾ot이라고 불리는 80ms의 시간간격을 가지는 Si毗들로 나뉘어
진다. 각 Si야은 （그림 斗8）과 같이 호출 Indicators(PI), Configuration Change
Indicators(CCI)와 Reserved Indicat아들로 구성된다．
 각각의 단말기에는 2개의 호출 Indicator가 할당이 되며, 하나는 QPCH 없毗의
첫 번째 40ms어］ 그리고 또 하나는 QPCH Slot의 두 번째 40吐ns어］ 있으며, 그것의
다음어］ 할당된 호출채널 Si毗을 감시할 컨지 말 건지의 정보를 가지고 있다. 기지국
은 QPCH_POWER_LEVEL_PAGE와 QPCHPOWERLEVEL小CONFIG의 P可a尸
meter들을 통해서 P1와 CCI bits를 위한 transmit-power level을 지시해야 한다．


    Page Channel   2047   0      1   1   2     3
                                                                     나
                                                                         i   比   쩌




    Quick Page
    Channel
                                              켜F- 호출 채널 Slot(80ms)

                                             Quick Page Channel
                                                 Slot(80ms)



           호출 채널 Slot B의 수신여             호출 채널 Si毗 C의 수신여
           부에 대한 정보를 포함                  부에 대한 정보를 포함


                              （그림 &8) Quic水 호출채널 구조



  각각의 단말기에는 2개의 호출 Indicat아가 할당이 되며, 하나는 QPCH Si毗의
 첫 번째 40吐TIS어］ 그리고 또 하나는 QPCH Si毗의 두 번째 40ms어］ 있으며, 그것의
다음어］ 할당된 호출채널 Si毗을 감시할 건지 말 건지의 정보를 가지고 있다. 기지국
    8. IS-95 Call Flow
1

은 QPCHPO人자ER나LEVEL_PAGE와 QPCH1POWER나LEVEL_CONFIG의 Para
meter들을 통하囚 PT와 CCI bits를 위한 transmit-p(叭ver level을 지시해야 한다．
  기지국은 시스템이 그것의 Configuration을 갱신할 때 최소한의 시간 주기가 T
(T = 2MAX_SLOT_CYCLE_INDEX）인 모든 단말기를 위한 호출 hi小cators를
turn on 할 것이다. Sec的r Configuration 갱신이 필요할 때 기지국은 Configuration
Change In小ca的rs를 T31쿄印）초） 안어］ turn on 할 것이다. 단말기는 일정한 주기
동안 단지 방문이 이루어진 기지국수만큼 CoT小guration을 저장하여야 한다. 저장
된（力nf迪uration의 기지국으로 Han面if 한 이후어］ 단말기는 CCI를 확인하고 즉각
적으로 Slotted 入4ode로 돌아갈지 말지를 결정해야 한다.


     8.2.7 명렁과 메시지 처리 동작

 단말기는 새로운 정보로의 Update, 확인을 요구하는 메시지어］ 확인절차와 더불
어서 명령과 메시지 처리 동작이 있다. 이것 역시 호출채널로 수신된 메시지 중에서
주소필드와 그에 대응되는 단말기 식별 데이터를 비교하여 address m毗ching이 이
루어지면 그 해당되는 메시지를 처리한다．
 단말기는 수신한 메시지들 가운데서 단말기가 가지고 있는 정보를 update하는 더］
에만 사용하는 메시지가 있고, 또한 수신 여부를 확인해 주는 것이 있고, 때로는 이
와 같이 구체적인 행동을 행하는 절차가 있다. 이러한 구체적인 행동들은 Order
Message어］ 포함된 명령코드와 명령 자격코드（OR均 : ORDer Qualification C어扼）
어］ 의한 것과 명령과 관련퇸 호출채널 메시지어］ 의해서 있는 것이 있다．


    명령 관련 메시지
    다음의 메시지들을 수신하면 각 메시지들이 내포하고 있는 해당 명령을 단말기는
수행한다．
    Authentication Ch에enge Message   단말기는 AUTHs값과 상관없이 유일시도 응
답 절차를 처리하고 인증시도 메시지로 응답한다. 단말기는 T32m초 이내에 명령／메
시지 응답표시와 함께 시스템 액세스 상태의 부가정보 갱신 부 상태로 들어간다．
    Channel Assignment Message   이 메시지의 ASIGNMODE에 호출채널 할당이
 통보되었을 때 단말기는 이것을 거부하든지 아니면 자신이 할당받을 호출채널의 주
 파수가 어떻게 되는지를 FREQ皿寸CL를 통해서 확인하고 새로운 호출채널 감시를
    442                                           8. IS-95 Cal l Flow



위한 작업을 한다. 이러한 ASSIGN MODE는 3Bit로 표현되며, 여기에서는
CDMA only 망에서 타당한 값에 대해서만 이야기한다. 이 값이 100, 이때는 통화
채널 할당을 하겠다는 말이며, 101일 때는 호출채널을 할당한다는 말이 된다．
 Extended Chann심 Assignment Message   이 메시지 역시 Channel Assignment
Message와 동일한 기능을 가지나 이 메시지에는 앞서 이야기한대로 채널 할당 단
계에서 소프트Han面if를 지원하기 위한 값틀이 전송되며, 이 메시지는IS-95C에서
추가된 메시지이다．
 PACA Message - PACA 서비스를 위해서 사용되는 메시지로 단말기는 이 메시
지를 수신하면 일련의 처리절차를 수행해야 한다．
 Dat（그 Burst Message   瓢1S를 전송하기 위한 메시지로 이 메시지를 수신하면 단
말기는 이 메시지어］ 따른 응답을 하고 처리를 한다．
 Order Message    각종 명령들을 수신하고 수행한다. 이 메시지들의 주요 내용을
간략히 요약하면 다음과 같다．
   水 Lock-Until Power Cycle 명령 H 단말기는 반영구적 메모리어］ Lock-Until
     Power cycle 명령어］ 대한 이유를 기록한다. 단말기가 이 명령을 수신한 후
     Unlock 명령을 받을 때까지 또는 단말기 전력 사이클링 후까지（예를 들어서
     단말기의 다음 파워업까지） 단말기는 시스템 /\ccess 상태로 들어가지 못한
     다. 이 조컨은 시스템 /\ccess 상태로 들어가게 되는 임의의 다른 단말기 조
     컨 중 먼저 시행된다. 단말기는 단말기 유휴상태로 빠져나올 수도 있고 잠김
     지시와 함께 단말기 초기상태 중의 시스템 결정 부 상태로 들어간다. 이렇게
     하면 단말기가 잠김상태 동안 선택동작모드에서 동작할 수 있다．
  永 잠금해제 명령 e 이 명령을 수신한 뒤에 단말기는 더 이상 잠금상태가 되지
     않는다. 단말기는 사용자에게 잠금상태가 제거되었음을 알려 주고, 단말기는
     잠금해제 지시와 함께 시스템 초기상태의 시스템 획득단계로 들어간다．
  永 유지요구 명령            단말기는 단말기의 반영구적 메모리어］ 유지요구 명령어］ 대
    한 이유를 기록한다. 단말기가 먼저 Lock-Until Power cycle 명령을 수신하
     면 단말기는 여전히 li兀k상태어］ 있다. 그렇지 않으면 단말기는 여전히
    unlock상태어］ 있다. 단말기는 사용자가 지속 필요 상태어］ 있는지를 알아야
    한다．
  米 등록거부 명령 1 이 명령은 보통의 서비스가 이 시스템에서 사용 가능하지
    8. IS-95 Call Flow                                  443
1


        않음을 나타낸다. 단말기는 등록거부 지시와 함께 단말기 초기상태의 시스템
        결정 부 상태로 들어간다．
      米 등록요구 명령           단말기는 등록 을 수행한다．
    Service Redirection Message   단말기는 저장하고 있던 RETURNJFFAIL값을
수신한 값으로 다시 설정하고 REDIRECTJEC값을 수신된 메시지로부터의 방향
전환한 레코드값으로 재설정한다．
    SSD Upd아e Message - SSD를 갱신한다．
 Status Request Mess（그ge - 단말기는 이 메시지를 처리한 후 상태 응답 메시지로
응답한다. 만약 어떤 정성적 정보（QUAL皿寸FO1TYPE값이 (xoooox）일 때）를 명
시하지 않았을 때 단말기는 상태 응답 메시지내의 요청정보 레코드를 포함한다. 만
약 메시지가 대역등급을 명시하면 (QUAL끄旺？O_TYPE값이 ()0000X끄일 때）, 단
말기는 상태응답 메시지내어］ 대역등급（BAND_CLASS）을 명시한다. 만약 메시지
가 대역등급과 동작모드를 명시한다면 (QUAL小INFO TYPE값이 ()0000010일 때）,
단말기는 상태 응답 메시지 내에 오직 대역등급（BAND_CLASS）과 동작모드
幻PMODE）을 명시하는 요청정보 레코드를 포함한다. 단말기는 T32m초 내어］ 명
령／메시지 응답지시와 함께 시스템 /\ccess 상태의 부가 정보갱신 부 상태로 들어
간다．


    명령 메시지의 명령코드와 ORDQ
 다음의 명령코드를 망으로부터 수신한다면 해당 명령을 단말기는 처리한다. 이러
한 ORDQ는 명령 메시지의 명령코드를 좀더 세부적으로 구분하여 좀더 구체적인
명령을 하기 위해서 사용된다．
 지금까지의 이야기들어］ 대해서 다음과 같이 우리의 일상 생활 가운데에서 일어날
수 있는 예로써 그것의 이해를 돕겠다. 즉 매일 아침 배달되는 신문이나 TV를 통해
서 우리는 사회에서 일어나고 있는 새로운 사건 사고 및 유용한 정보들을 습득하고
우리의 머리 속어］ 기억시킨다. 그리고 이러한 새로운 정보 혹은 유용한 정보를 우리
의 생활 속에서 활용한다. 또한 가끔은 우리가 얻게 된 정보들 중에서, 이를테면 친
구로부티 온 안부편지를 받았다면 잘 받았다고 회신을 해 줄 때도 있을 것이다. 더
나아가서 이렇게 얻게 된 정보 가운데서 수신자의 좀더 적극적인 행동을 필요로 할
때도 있을 것이다.
     444                                                           8. IS-95 Call 듸0小／
                                                                                        1

                       （표 &5) 명령 메시지의 명령코드와 아극D（그

 Order Code     ORDQ                                 이름／7陪
   000001      00:)0()000    Aabbre미毗ed 시ert Order
   000010      00000000     BS Challenge Confirm 명령
   000100      00000000     Reorder 명령
   000110      以xxx刃00      Audit 명령
   001001      00000000     Intercept Order
  010000       00000000     BS확인 Order
  010010      000lnnnn      Lock unlil P(기wer-Cycled Order（여기서 nnnn은 잠그는 이유임.)

  010010                    八4aintenance Requir以I Order（여기서 nnnn은 Maintenance하는
              0010nnnn
                            이유임.)
  010010      11111111      U川ock Order
  010101      00000000      Release Order
  010101      以xxx刃10       Release（명령（요구된 SO이 거절됨）
  011011      00000000      Rigistration Accepted Order(ROAIVI_INDI not included)
  011011      以xxx刃00       Rigistration Rejected Order
  011011      00000000      Rigis甘ation R由ected （뇨der
  011011      00mmm         Rigistration Rejected Order(delete TMSI)
  011011      00000000      Registraion Accepted Order(ROAM_INI)I included)
  011110      Nnnnnnnn      local Control order
  011111      00000000      Slotted Mode order
  100000      00000000      Retry order



 이렇듯 우리의 생활 가운데에서도 새로운 정보를 얻어서 처리하는 데에는 단순히
수신만 하는 정보, 수신 후 수신을 확인해 주는 정보, 나아가서 또 다른 행동을 하는
정보들이 있다．
 이렇듯 단말기도 그것이 서비스 받고 있는 망의 가운데에서 이러한 상호작용을
통히꺼 망에서 단말기의 존재를 인정받고 그어］ 상응하는 동작을 하는 것이다. 우리
의 생활방식은 예로부터 전해 오는 것이기에 아마도 이러한 절차는 사회의 행동양
식에서 본받아서 이러한 규격이 나왔을 것이다. （그림 斗9）는 대기상태에서 상태콴
리의 전체적인 정리를 순서도로 표시한 것이다．
8. IS-95 Call Flow



                PAGECHo = Code 채널
                PC data rate = PRATo
                  Tune to 호출 채널




                     Re帥tration수행

                                             NGHBR CONFIG = ,011"



                     와 이중화 MSG Check




                                               ///


                                                OVKD 정보에 대
                                                한 움 납 동작‘



                                                /
                                                               -No match -
                                                 MS Page Match
                                                 operation

                                                                        Mate"   기
                                                                                 1
                                                                   -




                                                                              1
                                                                       LUPC or ualock 小




                                                             ///


                                                              System Access싱태의
                                                              OVIID 정보 갱신




                                               서장된 파라몌터롤 갱
                                                                                 1
                                                                                System
                                       Yes   卜 신하고 또 다뵨 둥록                      Access
                                               처 리 절차 수행                         상태1




                              （그림 &9) 대기상태 정리




 8.3 Access Attempt State 처리                                                              )
 IS-95에서는 단말기가 대기상태에서 통화상태로 천이되기 위해서 이루어지는 일
련의 프로세스들을 시스템 /\ccess 상태로 규정하여 관리하고 있다. 이 상태는 분명
히 대기상태 및 통화상태와는 또 다른 처리를 할 것이다. 이 상태에서는 우선 망과
    446                                        8. IS-95 Call Flow
                                                                    .


상호교류를 통해서 망이 자신을 인식할 수 있는 처리과정이 필요할 것이며, 이와 동
시어］ 망에서 내려오는 호출채널을 통하써 자신의 /\ccess 채널이 정상적인지를 추
측하기위해서 대기상태의 호출채널 감시 기능도 아울러서 병행해야 할 것이다．
 구체적으로 이것과 관련해서 단말기는 부가정보갱신, Origination, Page Response,
Order瓜4essage response, 등록시도, 메시지 송출 등의 기능을 수행해야 하며, 이
것들은 각기 다른 부 상태들로 S/W로 관리되고 있다. 이러한 절차들은 공통적으로
다음의 Access 처리 과정과 같은 물리계층의 처리를 통해서 이루어진다．

   8.3.1 Access 쳐리

 단말기가 /\ccess 채널을 이용하여 기지국에 접속을 요구할 때는 호출채널에서
수신한 /\ccess Parameter 入4essage어］ 포함되어 있는 정보를 이용하여 접속한다．
Access Parameter Message는 open loop power를 설정하기 위한 Parameter, 설
정된 전력으로 출력하였으나 전송어］ 실패했을 경우 다음 단계의 송신전력 및 지연
시간, Capsule 사이즈 등이 전송된다．
 기본척으로 단말기가 망어］ Access 하는 경우는 망의 입장에서 볼 때는 예측을
전혀 할 수 없는 경우이다. N개의 단말기는 자신이 언제 망에 /\ccess를 할런지는
당사자만이 알 수 있고 전체적인 시스템의 입장에서는 N개의 Random변수가 존재
하는 것이다. 따라서 망의 입장에서는 기본적으로 단말기가 Access하는 것을
Random Access로 규정하고 통계처리만 할 수 있는 것이다. 이러한 관점에서 단말
기의 /\ccess 처리와 관련된 Parameter들이 결정되고 적용된다．
 단말기가 /\ccess 채널 번호를 설정할 때도 임의의 채널번호로 접속을 요구하고
실패할 경우 또한 임의의 채널번호를 사용한다. 이처럼 /\ccess 채널이 random한
것은 해당 기지국어］ 접속하는 단말기의 상태를 알 수 없고 그것이 확률분포함수로
표현될 수밖어］ 없기 때문에 이어］ 상응하는 확률분포함수로 처리하여 /\ccess 채널
간의 최대한 충돌을 방지하기 위해서 이다．
 즉 단말기가 기지국어］ 접속을 할 때 해당 /\ccess 채널에 다른 단말기가 이미 사
용할 수도 있고 기지국 상태 불량으로 사용할 수 없을 경우 등 접속에 실패할 경우
가 발생한다. 이러한 문제점을 해결하기 위해서 기지국어］ 접속할 1I 단말기는 채널
Access 프로토콜을 주어진 시간（time Slot) 동안 접속을 시도하며 접속에 실패할
경우 계속 임의의 시간이 지난 뒤어］ 재접속을 시도하는 방식인 Slotted ALOH\ 방
    8. IS-95 Call Flow                                 447
.

식과 유사하게 사용한다．




                   에게 전화할 수 있는       :＼노
                   Pcs 이므로 Random



                                    夕
                   Access
                                           /,y




                         （그림 8너0) 단말기의 Random Access


    각각의 /\ccess Probe가 기지국으로부터 A아（를 받지 못하는 주된 이유는 단말
기의 송신전력이 적거나 다른 /\ccess Probe들과 충돌어］ 의한 경우이다. 송신출력
어］ 의한 문제는 앞선 5장에서 이야기가 되었으며, 충돌어］ 의한 문제는 또 다른
Access의 장애요인이다. 때문어］ 각각의 /\ccess I노obe들 사이 그리고 /\ccess
Sequence 사이어］ 특정한 시간지연을 통해서 이러한 문제를 해결하고 있다.
    이러한 시간지연은 중요한 시스템 Parameter일 수 있는데 이러한 지연 값들이
너무 크다면 /\ccess상어］ Access 자체가 없어서 많은 지연이 초래될 것이며, 또한
너무 짧다면 잦은 충돌확률로 인해서 /\ccess가 또한 지연될 것이다. 랜덤 /\ccess
절차의 Parameter 대부분은 망으로부터 수신한 /\ccess Parameter 메시지로부터
제공받는다. 이것은 /\ccess 과정에서 발생될 수 있는 과다한 출력과 무질서한 접속
으로 인한 충돌을 방지하기 위해서이다.


    Access A1도, Probe, Probe Sequence

    단말기가 하나 이상의 메시지를 전송하고 그것어］ 대한 응답을 받는 과정을 통칭
하여 /\ccess Attempt라고 한다. 이러한 /\ccess Attempt는 몇 개의 /\ccess
까obe라는 Access의 실체（?）로 구성된다. 또한 이러한 /\ccess 까obe는 동일한
Access 채널번호를 사용하는 그룹을 /\ccess I노obe 시퀀스라고 별도로 구분한다．
5장의 （그림 5-3）과 4는 이러한 내용을 잘 설명하고 있다．
    단말기가 전송하고자 하는 정보를 /\ccess 채널로 전송할 때 /\ccess Probe를 통
해서 이루어지는데 동일한 Access Attem姚에서 사용되는 /\ccess Probe의 내용은
동일한 정보를 담고 있다. 단지 /\ccess Probe어］ 담겨 있는 정보의 전송을 성공하기
위해서 앞서 5장에서 공부한 Open Loop Power Control어］ 근거하여 조정된 출력
                                                                8. IS-95 Call Flow
                                                                                     1


값어］ 따라서 출력값만이 차이가 나는 것이다. 따라서 /\ccess Attempt의 첫
Access Probe는 개방 루프 전력제어에 의해서 결정되며 /\ccess의 성공확률을 높
이기 위해서 출력이 증가하는 방향으로 계속 변하게 퇸다．
 또한 이러한 /\ccess Probe에는 각종 Access 채널의 내용이 포함된 Capsule과
Access 채널의 검출 혹은 식별을 용이하게 하기 위한 I斗eamble로 구성된다. 이것
어］ 대해서는 7장에서 공부하였다．
  이상의 /\ccess I눈obe가 전송되기 위해서는 현재 단말기가 감시하고 있고
Access를 시도하려고 하는 대상이 되는 기지국이 출력하는（역으로 현재 감시하는
호출채널을 출력하는 기지국으로 /\ccess를 한다고 이야기할 수도 있다） 호출채널
과 연관하여 /\ccess 채널의 번호를 결정하게 된다（이렇게 결정퇸 /\ccess 채널 번
호 등은 Long Code Mask를 결정하는데 사용된다）. 이렇게 결정퇸 /\ccess 채널번
호는 하나의 /\ecess Probe 시퀀스에 동일하게 적용된다. 즉 동일한 /\ccess 채널로
전송되는 것을 Access Probe 시퀀스라고 한다. 즉 하나의 /\ccess Probe 시퀀스어］
서는 처음어］ 할당받은 /\ccess 채널 번호를 동일하게 적용해서 /\ccess Probe를 생
성한다는 것이다.


         억세스    채널
        ,Slot과 프레임
       ／의 경계

                              1개의 억세스 채널 Si毗

       寸H1    억세스 채널 Preamble                      억세스 채널        4
              (Modulation Symbol 0)              Message Capsule




         -H H- ,;l ,B Frame(2。rns)                                    System
                                                                      Ti1)mr)


                  1+PAM SZ             ＞寸13+MAXCAPUSZ 1
                 (1-16 Frame)               (3-10 Frame)
                           4+PAM SZ+MAX CAP SZ
                                (4-26 Frame)


                                             천
   +    4HPN Randomization Delay = PN X 0.8138 1is


                 （그림 &11) Access Probe의 구성과 랜덤화
    8. IS-95 Call Flow                               449
U


 각 Access Probe Sequence어］ 사용된 /\ccess 채널은 현재의 호출채널과 연관된
모든 /\ccess 채널 중에서 의사 랜덤하게 선택된다．
 단말기가 /\ccess 채널로 정보를 전송하는, 즉 /\ccess Probe를 출력하는 경우는
단말기 자체에서 특정한 요구（예를 들면 발신호나 등록 등）를 하는 경우와 망에서
요구하는 내용어］ 대한 응답으로 구분할 수 있다. 이러한 2가지는 망에서 /\ccess를
시도하는 단말기의 존재를 이미 알고 있다는 것（혹은 /\ccess를 예상하고 있다는
것）과 전혀 예상할 수 없다는 것의 차이라고 할 수 있다．
 정리하면 /\ccess Probe는 동일한 메시지를 전송하는 단위라고 할 수 있고
Access Probe Sequence는 동일한 Access 채널을 사용하는 /\ccess Probe의 그룹
이라고 정의할 수 있다．
 』麒野



 Access Timing

 Access Probe와 /\ccess 까obe Sequence의 타이밍은 /\ccess 채널의 Si야으로
표현되며, 이러한 Si毗은 /\ccess 채널상에서 구성되는 메시지 Capsule과 프리엠블
로 구성된다는 것은 이미 7장에서 공부한 적이 있다．
 임의의 Access시도에서 /\ccess 채널 출력의 정확한 타이밍은 PN 랜덤화라고
일컫는 절차어］ 의하1 결정된다. 각 /\ccess 시도에 대해서 단말기는 단말기의
ESN_S어］ 좌우되는 8.5.3장의 Hash 함수를 사용하여 0부터 " 2尸R（石且尸쏘R月R-1,' PN
ch如까지 지연 RN을 계산한다. 단말기는 RN개의 PN chip만큼 전송타이밍을 지연
한다. 이 전송 타이밍의 조정은 직접 Sequence확산 Long Code와 직교확산 I 및
P瓦OT_PN Sequence의 지연을 포함한다. 이 결과 단말기에서 기지국까지의 범위
로 효과적으로 증가시킬 수 있다（이렇게 하면 기지국이 같은 Access채널Si毗내의
많은 단말기로부터의 송출신호를 따로 구분하여 복조할 수 있을 것이다. PN 랜덤화
를 위한 비 랜덤 Algorithm의 사용으로 기지국은 PN 랜덤화와 단말기로부터의 실
제 전파지연과 분리할 수 있다. 따라서 기지국은 단말기로부터 Reverse 통화채널
전송의 타이밍을 정확하게 추정할 수 있다）. （그림 斗11）을 참고하라．
    Access Probe 시퀀스의 /\ccess I노obe의 전송 또한 의사랜덤어］ 의하써 출력된
다. 각 /\ccess Probe를 송출한 후 단말기는 그 읾ot의 끝으로부터 특정주기 TA=
(2+ACC_TMO) X 80ms 동안 기지국으로부터 확인을 기다린다. 확인이 수신되면
Access 시도는 종료되지만 그렇지 않다면, 0부터 PROB且BKOFF+1개의 Si毗까
   450                                                   8. IS-95 Call Flow
                                                                              U


지의 추가 백 오프 지연인 RT 이후 다음의 /\ccess Probe를 송출한다. 이 내용은
5장의 （그림 5-3）을 참고하라．
 Access Probe 시퀀스가 종료되고 다음 번 시퀀스가 시작되는, 즉 다음 번 시퀀스
의 첫 번째 Access Probe가 출력되는 시점 역시 랜덤한 값으로 구해진다. 이러한
랜덤값은 0부터 1 + BKOFF Slot까지의 범위를 가지는 백오프 지연인 RS이다. 이
러한 백오프 지연은 첫 번째와 두 번째 혹은 n번째와 n+1번째 시퀀스를 구분하기
위한 시간지연이라고 생각할 수 있다．




                                          - PP 十PD늬
    앞뒤의 /\l ｝니｛三
    구분하기     위한
    시간 간격             (a) Response         (b) Request


                   （그림 8너2) Request오＋ Response 경우의 Access

 그런데 단말기어］ 의해서 먼저 동기부여가 되는 요구 메시지들인 경우에는 백오프
지연 이외에 지속성 지연값을 결정하는 지속성 시험 PD의 사용으로 인해서 추가되
어야 한다. 이것은 망에서 Request를 위한 Access Probe의 메시지 도착 시간을 제
어할 수 없기 때문이다. 즉 기지국은 응답을 필요로 하는 메시지를 전송하는 속도를
조절함으로써 직접 응답 메시지의 도착속도를 제어할 수 있으므로 지속성 시험은
응답 Access시도어］ 필요하지 않다. 그러나 단말기에서 먼저 요구되어지는 경우 망
은 그것의 시점을 알 수 없으며, 따라서 /\ccess 채널번호를 할당하는 방법을 사용
해서 단말기들의 /\ecess 자체를 제한하며 랜덤 /\ccess의 효과적인 관리를 위해서
이러한 지속성 시험을 통해서 /\ccess를 순차적으로 진행할 수 있게 한다. 즉 식당
에서 음식을 기다리기 위해서 줄서 있는 것과 마찬가지의 원리이다．
 백오프 지연 RS후 각 읾ot어］ 대해 단말기는 단말기의 Access시도 및 /\ccess 과
부하 등급어］ 의한 Parameter로 의사랜덤 시험을 수행한다. 만일 그 시험이 통과하
면 그 Sequence의 첫 번째 /\ccess 다obe가 그 읾ot에서 시작된다. 그 시험이 실패
하면 APS는 최소한 다음 읾ot까지 지연된다．
    8. IS-95 Call Flow                               451
1



    Parameter 설정
    Access 시도 때마다 단말기는 8.5.1절에서 설명할 Hashing 기법을 사용하여 0부
터 2PROBE_PN_RAN -1까지의 수인 RN을 계산한다. Access 시도되는 동안어］
단말기는 Long （沁de I万rect S凹uence 확산과 I 및 Q채널 PILOT_PN Sequence
직교확산을 고려하여 송신 타이밍을 PN 칩만큼 지연한다．
    Access시도 단말기는 하나 이상의 Al冬를 송신한다. Access시도가 /\ccess 채
널 요구일 경우 단말기는 MAX_REQ_SEQ개의 APS를 송신한다. Access 시도가
Access 채널 응답일 경우 단말기는 八/[AX_RS므SEQ개의 APS를 송신한다．
    각 APS를 송신하기 전어］ 단말기는 8.5.4장의 랜덤번호 발생기에서 랜덤번호RA
(0- ACCHCH사m를 발생한다. 단말기는 이 번호 RA를 /\.PS의 모든 /\ccess Probe
를 위한 Access채널 긴 코드 마스크에서의 /\ccess 채널번호 ACN으로 사용한다．
    첫 번째 Al冬를 제외한 각 Al冬를 전송하기 전어］ 단말기는 랜덤 발생기 절차에
의거하써 0- i+BKOFF+1까지의 임의의 RS수를 발생한다. 단말기는 RS Slot 수
만큼 APS의 송신을 지연한다．
    Access시도가 /\ecess 채널 요구이면 각 APS의 첫 번째 /\ccess Probe를 송신
하기 전과 앞선 Al冬의 전송완료 후 RS 만큼의 지연이 끝난 후 단말기는 각
Access 채널 Slot어］ 대해 지속성 시험을 수행한다. 지속성 시험을 위해 단말기는
랜덤번호 발생 기법에 의하여 랜덤번호 RP (0 < RP < 1）를 발생한다. RP가
Access 시도의 종류어］ 따라서 P의 현재 값보다 작을 경우 지속성 시험은 통과하였
다고 본다. P값이 0이면 Access시도는 실패하고 이때 단말기는 /\ccess시도를 종
료한 후 등록변수를 갱신하고 Access 거부지시와 함께 단말기 초기화 상태 중 시스
템 결정 부 상태로 들어간다．
    앞서서 이야기되었듯이 단말기는 랜덤 /\ccess이며, 이러한 랜덤 Access라는 의
미는 아무렇게나 /\ccess 할 수 있다라는 의미와는 구별이 된다. 한번 발생된 Al冬
를 통해서 /\.ccess 후 그것이 성공하지 못했을 경우 새로운 /\ccess Probe
S因uence를 시작하기 위해서 단말기는 /\ccess Over Class(ACCOLC）에 따라서
"Congestion Control(혼잡제어）"을 한다. 이미 언급한 바와 같이 기지국에서 제어
되는 resp끄lse attem吼에는 적용되지 않고 단말기가 자체적으로 접속을 시도하는
request attem砒에만 적용된다.
                                                                                                                             8. IS-95 Call Flow



 이것은 단말기가 request attempt를 할 때 PD(Per前就ence Delay）로 결정되며，
이러한 과정을 硏｝rsistence test라고 한다. Persistence test는 단말기가 등록
(registration), 메시지 전송（MO SMS : 入4obile Originated SMS)）과 그 외의 경
우로 구분된다．
 등록인 경우 해당 단말기의 PSIST(0에서 15까지 할당되며 단말기의 ACCOLC어］
따라 결정됨）에 따라서 random delay 값이 결정된다. 이때 적용되는 값은 단말기의
PSIST와 Access Parame扼r Message어］ 있는 REG_PSIST이다. 그리고 메시지 전
송인 경우는 해당 단말기의 PSIST와 MSG_PSIST가 적용된다. 등록과 메시지 발신
이외의 request attempt는 단말기의 P51ST만 적용하여 delay 값을 켤정한다．


                     {
 Access 채널 요구가 등록일 경우 P는 아래와 같이 계산된다.
                          ,
                              2
                                  _
                                      PSJST
                                              (n)   /   "x
                                                                      2m, 1    's1
                                                                                     ', ,   " PSIST         (n)         63                 (8-5)
                          。                                              。therwise                   n =。,1, ..., 9
       p=
                     1。
                              ' "" " '                       x
                                                                 2-   REG_ PSJST
                                                                                                芽 PSIST（川 芒 7
       i7 =                                                                                                                                (8- 6)
                                               "'
                     jC   U                                              。t力erwise                n=10,11,...,15

 여기서 n은 단말기에 할당된 과부하 등급（ACCOLC）이고 PSIST(n）과 REG
PSIST는 /\ccess Parameter 메시지로부터 온 것이다．
 Access채널요구어］ 대한 메시지 송신이면 P는 아래와 같이 계산된다．

                              2 "" 釘" X x2出SG_PS싸                                           可PSIST(n）才63                                   (8中7)
       니，
                                                                          otherwise                  n= 0,1,...,9


       11=
                     j.   U 2           '     '"             "            ；二
                                                                          ,
                                                                            。therwise
                                                                       " ' ";      ,,‘          if   n= ILJ, 11, 7
                                                                                                     PS!ST      ...,D
                                                                                                                  (n)   :                  (8-8)



 여기서 n은 단말기어］ 할당퇸 과부하 등급이고 PSIST(n）과 八4SG_PSIST는
Access Parameter 메시지로부터 온 것이다．
 Access 채널 요구가 등록 또는 메시지 전송 이외인 경우 P는 아래와 같이 계산퇸다．


        //
             ,   -

                 e   )IJ 2 PSLT( ')/
                              -                                                             f PSIST   才 63
                                                                                                      (n)
                                                                                                                                           (8- 9)
                       [0                                              (7r/ier1V/Se
                                                                       otherwise                n =0,l,
                                                                                                     1, ...,
                                                                                                      ．··19
8. IS-95 Call Flow



                     2                                                     if PSJST(n) /7
                                          MSG_ PSIST
                                 x
            1。                       2-
                         '   "
                                                                                                (8- tO)
            J.
                 U                                     otherwise             n=10, 11. ....15
       0=
                                               시작



                                           PROBE=O
                                            SEQ=O



                                 ESN_S를 사용하여 hash
                                 하고 PROBE_PN_RAN으
                                    로 RN읕 얻는다




                                                                          Slot이 시작되었으면
                                                                            RP를 발생하라．


                                                           \\
                                                                  \
                                     Slot이 시작되었으면
                                                                      \
                                       RP를 발생하라．                      i
                                                                      J
                                                                  /
                                                                川｛)




                                     Slot이 시작되었으면
                                       RA를 발생하라．



                                     전송 전력을 초기화
                                         한다




                             시스템 타이밍에 RN Chip을
                             더한 시간에 엑세스 채널 RA
                              상에서 프로부를 송출한다．
                               그리고 TA를 설정한다．




                                  （그림 &13.1) Access 절차 0카 ]
   454                                                                8. IS-95 Call Flow
                                                                                             1




               [   Access성     ．“
                                    Yes




                                                                              PWR니STEP만
                                                                              큼 전력 증가
                                                                      0
                                                                                   十
                                                                              Wait RT Slot
                                                                                   A
                                              PROBE=PROBE+ 1
                               be가        그
                             Pr。                                                RT발생
                             NUM STEP
                             만큼 출력이

                                                                      Yes
   Wait RS Slot
               1
                                                                  小PROBE+ BKOFF+ ]     卜／
                             Sequence가                            의 범위인 임의의수
                             MA小REQSEQ(                           RT를 발생한다．
     RS발생                                       SEQ=SEQ+ 1
                             MAX_RSP_SEQ)
                             개 가 되었는가 ?



                                    Yes                                       Access 실패
         1
         11
          hH
               O싸I3KDFF+ 1의 법
               위인 임의의수 RS                                    단말기의 초기상     i
               롤 발생한다．                                       E가 중 시스템 결
                                                             정 상태르. 천이


                                    （그림 &13.2) Access 절차 예 2


 n은 단말기어］ 할당된 과부하 등급이고 PSIST(n）과 入4SG_PSIST는 /\ccess
Parameter 메시지로부터 온 것이다．
 각 /\ccess Probe 전송 후 단말기는 /\ccess 채널 Si毗의 마지막에서 TA= (2
+ ACC1TMO) X 80ms동안 기다린다. TA초 이내어］ 확인이 도착하지 않을 경우
단말기는 다음의 과정을 수행한다．
 NUMeSTEP또는 몇 개의 /\ccess I노obe가 /\ccess Probe가 APS에서 전달되면
단말기는 랜덤 절차를 사용하여 0 - PROBE_BKOFF+1 사이의 랜덤번호 RT를
발생시킨다. 단말기는 RT개의 추가 Access채녈 Si毗을 지연한 후 다음 /\ccess
    8. IS-95 Call Flow
1                                                                              455


Probe를 전송한다．
    그렇지 않을 경우 요구 Access에 대한 八/IAX_REQ卜SEQ또는 응답Access어］ 대
한 八/IAXHRSPSEQ보다 적은 수가 Access시도에서 송신된 경우 단말기는 또 다
른 APS를 위한 랜덤 절차를 수행한다．
    위와 같이 P값은 I光rsistence test를 수행하는 기준값이 되며 random 값인 RP를
지속적으로 생성하여 P값과 대조한다. 만약 RP값이 P보다 크면 persistence test를
계속 수행한다．
 Persistence test는 Si毗 단위로 설정되며 test어］ 성공하면 다음 APS는 현재
Slot어］ 시작되고 실패할 경우 ／뇌？S는 persistence test로 인하여 몇 개의 Slot이 지
연될 수 있다. 이와 같이 persistence test는 기지국어］ 접속하는 단말기의 상태를 알
수 없기 때문어］ 단말기 class별로 접속 지연을 이용하여 congestion contr이 역할을
한다．


    Access 채널의 Mask

 Access 채널은 Pu毗 채널과 함꼐 어떻게 보면 Pilot어］ 의해서 전송되는 것이 아
니다. 그러므로 특정한 기지국으로의 접속과 관련된 PN offset이 없이 망어］ 접속을
시도하게 된다. 따라서 수신 가능한 모든 기지국에서는 단말기에서 송신하는 신호
를 받을 수 있다. 즉 단말기가 Reverse으로 전송하는 신호들은 특정한 기지국의 정
보를 담고 있다고 하기 보다는 단말기의 정보로 변조되었기 때문이다. IS小95에서
사용하는 Long Code는 다음의 식과 같은 형태로 사용될 것이다．

            只功 = 伊＋少＋少＋尸나尤27+ 少＋少＋尹 +／나尸나尸뇩尸7
                 ＋尤쩌＋兀10＋尸＋兀6十t5＋兀3＋兀2＋尤＋1                                     (8- 11)




       41                   33 32   28 27     25 24        98              O

            110001111           ACN     PCN      BASE_ID        Pilot_PN


            ACN : 억 세스 채 널 번호

            PCN : 호출 채 널 번 호


                         （그림 &14) Access 채널 ZJ 코드 마스크
                                              8. IS-95 Call Flow
   456                                                             1


 긴 코드에서 사용되는 마스크는 단말기에서 사용하는 채널형태어］ 따라서 달라진
다. Access 채널을 통해서 전송되는 신호는 다음의 （그림 斗14）와 갇은 형태로
ma針ing되고 이러한 ma針dng은 앞서 3장어써 이야기하였듯이 식 (8尸11）의 초기
값을 설정해 주는 역할을 하게 된다．
 Reverse 통화채널의 데이터들은 또 다른 형태의 I力ng Code Mask를 사용한다．
여기에서 사용되는 mask는 공용 Long Code Mask라고도 하며, 개인용Long Code
八4ask라고도 한다. 이것은 이미 /\ccess할 대상이 설정이 끝난 통화상태어］ 이루어
지는 변조이므로 이 코드는 단말기만의 고유한 정보로 n追sk를 형성한다. 이것은
（그림 斗15）와 같이 八441부터 入432까지는 11oX끄i(x刃의 값으로 하고 나머지 32 Bit
는 그 단말기의 ESN_S를 사용해서 n追sk를 구성한다. 즉 CDMA단말기는 통화시
어］ ESN_S의 정보로 데이터를 변조하므로 각각의 단말기들은 모두 다른 mask를
사용하여 신호를 변조하게 퇸다. 따라서 이 신호를 복조하기 위해서는 단말기의
ESNS정보를 알고 있어야 한다. 이러한 이유에서 CDMA단말기의 신호의 도청이
불가능하다라는 말이 나온 것이다．
 즉 기지국은 Long Code 入4asking으로 초기값이 설정된 Long Code로 변조퇸 단
말기의 신호들을 찾는다. 이 값은 /\ccess 채널전송을 위해서 사용하는 I力ng Code
의 경우 그것의 값이 달라질 수가 있으나, Reverse 통화채널의 전송을 위해서 사용
되는 Long Code는 초기값 결정을 위한 mask를 구성할 때 단말기의 고유의 값인
ESN.mS을 사용하므로 언제나 같은 값이며 고유한 값이 된다．


  41                3231                                           0


       1100011000               ESN S의 조합

                （그림 &］듸 개인Long Code Mask 형태


  Access 채널 메시지는 등록, 발신, SMS 발신, 응답메시지 등이 있으며 address
type(ESN, MIN, IMSI）어］ 의하여 단말기가 구분된다. Access 채널 메시지는 다음
과 같이 6개 종류가 있다. 즉 등록 메시지, 명령 메시지, Data Burst 메시지, 발호
메시지, 호출응답 메시지, 인증 시도 응답 메시지들이다．
  단말기가 시스템 접속을 시도할 때 주어진 조건에서 연속적으로 접속어］ 실패할
 경우 재접속을 하지 않고 대기상태가 된다. 일부 단말기는 이를 보완하여 자동적으
    8. IS-95 Call Flow
口


로 재접속 시도를 하는 자동 재발신 기능을 가지고 있다．


     8.3.2 System Access의 Sub State

 단말기의 호 처리단계 중 대기상태에서 통화상태로 천이되기 직전에 관리되는 상
태가 System Access 상태란이야기는 이미 앞서 이야기되었다. 이러한 상태들의
종류와 이러한 상태들의 관리어］ 대해서 이 절에서 공부한다．
 단말기는 다음의 6가지의 sub state를 다음의 （그림 &16）과 같이 관리한다．


                                     대기상태에서 진입




                                     Overhead정보 갱
                                                   +
                                        신 부 상태



                          /Access\
                                               /
                                                                GPM를 수신
               확인 웅답을 요구                   /   사용자河 Data
               하는 명령이나 메               /       Burst 메시지를
               시지를 수신                 /        발생
                                                            사용자가 호
                                                            룰 시작




        MS 명령／메시지
         응답 부 상태                                   S SMS 전송玉甄
                                                    부 상태




                                                                          \
                대기상태로 돌아감．                                        통화 채널 상태로 천이 됨．

                         （그림 &16) System Access 상태 천이도


 단말기가 시스템어］ 접속을 시도할 때 항상 호출채널을 n아i-Slotted M以扼로 하
여 메시지를 수신한다. 만약 호출채널을 수신하지 못하면 시스템 접속을 중지하고
대기상태가 된다. 즉 통화를 시도할 때 등록을 시도할 때 등과 갇은 상황에서 단말
    458                                       8. lS-95 Call Flow
                                                                   U


기는 Slotted Mo扼와 같이 불연속적인 동작을 하는 것이 아니라 non小Slotted
八/Iode와 같이 연속적으로 망을 감시하고 있다．


  Update Overhead Information Sub state

  단발기는 /\ccess Attempt를 하기에 앞서서 현재 자신이 /\ccess를 시도할 기지
국 혹은 Pu야이 맞는지를 다시 확인해야 할 것이다. 이것은 단말기가 가장 최적의
기지국으로 /\ccess를 시도해야 하는데 엉뚱한 곳으로 /\ccess를 시도할 수 있기 때
문이다. 이러한 Access시도는 성공할 수 없을 뿐 아니라 실패를 위해서 소요되는
시간만 낭비하게 될 것이다. System Access 상태에서는 Access Attempt가 되는
다른 부 상태, 즉 발호, 호출응답, 등록시도, 명령／메시지 응답, 메시지 전송 등의 상
태로 천이되기 이전에 현재 저장하고 있는 정보가 타당한지어］ 대한 확인작업을 하
게 된다. 따라서 Update overhead information substate는 호출채널의 overhead
Message를 검색하며 상태 Parameter인 CONFIG_MSG_SEQ와 ACC小fSG_
SEQ를 수신하여 이전 값과 다를 경우 해당 메시지를 수신하여야 하며 동일한 값일
경우는 Access 상태를 수행한다. 이때 4초（ T41m) 동안 타당한 Overhead Message
를 수신하지 못하면 단말기는 초기화 과정부터 다시 시작한다. 이때 정의된 timer는
호출채널을 통해서 수신퇸 갱신 부가 메시지를 얻는데 컬리는 최대 시간을 측정하
는 것이며, 이때는 PAGED를 NO로 설정하여 더 이상의 호출을 받지 않는다. 여기
에서 수신하지 못하는 경우라는 것은 충분한 세기의 호출채널 신호가 없어서 그럴
수 있고, 호출채널을 잃어버렸을 경우일 수도 있다.
 System Access 상태에서 단말기는 필요어］ 따라서 호출채널의 6개 overhead
Message에 대하여 Configuration이 다를 경우 이 메시지를 수신하여 갱신하여야
한다. 만약 이러한 절차가 완료되지 못할 경우에는 사용자가 통화키를 눌러서 통화
를 시도하나 실지로 /\ccess Probe가 전송되지 않으며 （이것은 단말기가 발호 메시
지（Origin謫이1 八4essage）를 전송하지 못하는 상태임） 이러한 Overhead Message
를 모두 갱신할 때까지 기다리게 되므로 통화키를 눌러도 이 정도의 시간지연 후어］
발호 메시지가 전송되게 된다. 이러한 문제는 망에서 이러한 Overhead Message를
정확하게 빠뜨리지 않고 전송해 주어서 Non-sbO杭ed Mode로 동작하는 단말기어］
이러한 정보를 정상적인 없otted mode보다 신속하게 전해 주어야 한다．
    8. IS-95 Call Flow                                   459
.



    MS Origination Attempt Substate
    단말기가 발신할 경우 /\ccess 채널의 origination Message를 전송하며, 등록은
registration Message, 그리고 S八IS와 같은 메시지 전송은 data bur就 Message를
사용한다. 이 경우에도 단말기는 호출채널을 검색해야 하며 호출채널을 수신하지
못할 경우 대기상태로 천이한다. 이것은 앞서 이야기된 전력제어의 논리와 비슷하
다. 즉 Forw可d 채널을 통해서 Reverse 링크를 예측하는 것이다. 다시 말하면
Forward의 호출채널이 잘 수신되고 이상이 없다면 단말기는 자신이 송출하고 있는
Access 채널 역시 망어］ 잘 도착할 것이라고 믿어 의심치 않는 것이다. 역으로 호출
채널을 잃어버린다면 그민큼 채널환경이 좋지 않다는 이야기가 될 것이며, 따라서
Access 자체도 유실될 것이므로 지금 시도하는 /\ccess는 포기하고 다음의 좋은 때
를 기다리기 위해서 대기상태로 천이할 것이다．
    앞서 이야기된 오버해드 정보 갱신 부 상태에서 호출채널을 잃어버린 경우는 현
재 단말기가 가지고 있는 정보는 단말기가 대기상태를 유지하기에도 부족한 정보를
가지고 있게 되는 것이다. 대기상태라는 것이 단말기가 현재 처해있는 상태와 자신
이 행해야할 분명한 정보를 가지고 망의 부름을 기다리는 상태이기 때문이다. 따라
서 대기상태에서 단말기는 가장 싱싱한 오버해드정보를 가지고 있어야 하나 오버헤드
갱신상태에서 호출채널을 잃어 버린다면 그것마저도 되지 못하기 때문이다. 이렇듯 상
태가 만족되지 않아서 천이될 상태는 오버헤드 갱신 상태와 다음에 이야기될 /\ccess
Probe와 연관퇸 모튼 상태들에서는 당연히 이렇게 차이가 난다.
    이 상태에서는 단말기는 /\ccess Probe의 Capsule어］ Origination message를 전
송하게 된다. 이러한 발신 메시지는 발신 단말기의 정보와 착신을 원하는 단말기의
정보를 포함하고 있을 것이다. 단말기의 정보는 이 단말기가 서비스를 받을 수 있는
단말기인지를 식별해 주는 하나의 인증절차라고 볼 수 있다. 이것을 단말기의 전자
일련 번호인 ESN(Electric Serial Number）을 통한 인증절차라고 할 수 있다. 사실
이러한 절차를 인증이라고 이야기하지는 않는다. 우리가 인증이라고 이야기하는 인
증은 8.6절에서 새로 상세하게 공부하도록 하자. 그러나 발신단졔에서도 이러한
ESN 확인 이외어］ 인증절차가 이루어질 수도 있다．
    또한 여기에서는 자신이 원하는 호의 성격을 규정할 수 있으며, 이것은 Service
Option이나 Service 구성（Configuration) 등으로 표현되어져야 한다. 이러한 내용
    460                                              8. lS 95 Call Flow
                                                                          U


은 다음 절인 통화상태에서 공부하겠다. 단말기가 이 상태어］ 있는 동안은 어떠한 인
터럽트가 있어도 이 상태, 즉 발호상태보다 우선적으로 처리되지는 않는다．
 발호 메시지 이후에는 단말기는 망에서 내려주는 Channel Ass坦nment Message
혹은 Extended CAM을 기다리며, 이 메시지를 수신하면 단말기의 이러한 요구어］
의한 응답을 받은 것이 퇸다. 이와 비슷하게 인증이 Enable되어 있을 경우에는
Authentication Challenge Message, Base Station Challenge Confirm Order,
SSD Update Message들을 받을 것이며, 이러한 메시지들어］ 확인 응답이 포함되어
있지 않으면, 즉 자신의 요구어］ 대한 확인 메시지가 아니면 단말기는 Access 실패로
판단하고 System Access 상태 T如er을 T42m(12초）로 설정하고 타이머가 종료될
때까지 응답을 못 받으면 대기상태로 돌아간다. 발호 메시지어］ 대한 접속시도가 기지
국으로부터 응답을 받아서 종료되면 단말기는 등록어］ 관련된 변수를 저장한다．


 Page Response Substate

 Page response substate는 General Page 혹은 Slotted page Message를 수신하
여 자기의 address type과 일치가 될 때 응답을 수행하는 단계이다. 즉 Page
match와 address match가 이루어졌을 때 이루어지는 것이다. 이것은 앞서 이야기
한 발호상태와 모튼 것이 동일하나 이 상태로 진입하게 되는 trigger poi毗가 다른
것이다. 즉 사용자의 의지어］ 의해서 발신 호를 시도하는 발호 메시지어］ 의해서 이루
어지느냐, 아니면 망에서 호출어］ 의한 호출응답이냐 하는 것이 된다．
 우리가 한 가지 생각해 볼 것은 단말기의 /\ccess는 랜덤 Access라고 했으나 호
출은 발생 자체는 3자의 입장에서 보면 랜덤하지만 실지로 단말기는 자신이 계속해
서 감시하는 호출 없ot으로 들어오므로 랜덤이 아니다라고 이야기할 수 있다．


 \MS Order/Message Response Substate

 Order/Message Response Substate는 기본적으로 page response substate와
동일하다. 단지 해당 MSG_SEQ어］ 대한 응답을 ACK_SEQ로 전송하고 order tyl光
만 명시한다는 것이 차이가 나는 것이다. 이 메시지는 또 다시 ACK를 요구할 수
있다．
 이 상태에서 단말기는 기지국으로부터 받은 메시지어］ 대해 응답을 보내고 단말기
가 호출채널의 유실을 선언하면 단말기는 송신을 정지하고 대기상태로 돌아간다．
    8. IS-95 Call Flow                                            461
U


이 상태 동안 단말기가 보낸 메시지에 대한 응답을 받으면 단말기는 접속시도를 종료
한다. CAM, authentication challenge message, base station challenge confirm
order, SSD update message어］ 확인응답이 포함되어 있지 않으면 단말기는 대기상
태로 돌아간다．


 Registration Access Substate

 Registration Access substate는 단말기가 등록을 위하여 /\ccess 채널로 메시지
를 전송하는 것을 말한다. 이 상태에서는 호출이 오면 받아야 한다. 발신의 경우와는
달리 등록의 우선순위는 낮기 때문이다. 또한 등록 시도의 경우 발신시도 상태와는
달리 기지국어써 응답 메시지를 수신하며 이 상태가 종료되고 대기상태로 다시 들어
가게 된다. 이것은 다음 상태, 즉 Traffic 상태로 천이되는 발신상태와는 사뭇 다르다．
  이 상태에서 단말기는 기지국어］ 등록 메시지를 보내고 단말기가 호출채널 유실을
선언하면 단말기는 송신을 정지하고 Idle상태로 돌아간다. 이 상태 동안 단말기가
보낸 메시지어］ 대한 응답을 받으면 단말기는 접속시도를 종료한다．
  이때에도 발신이나 착신응답과 마찬가지로 인증이 행해질 수 있으며, 이때는
authentication challenge message, base station challenge confirm order, SSD
update message어］ 확인응답이 포함되어 있지 않으면 단말기는 대기상태로 돌아가
고, 등록접속이 사용자의 전원차단 지시로 시작된 경우 단말기는 등록어］ 관련된 변
수를 갱신하고 전원을 차단한다. 등록 메시지어］ 대한 접속시도가 기지국으로부터
확인응답을 받아 종료되면 단말기는 등록어］ 관련된 변수를 저장한다．
  단말기가 사용자로 하여금 발호를 하라는 지시를 받으면 단말기는 진행중인 접속
시도를 버리고 발호 부 상태로 들어간다. 즉 발호든 호출응답이튼 이 상태보다는 우
선순위가 높은 상태들이라고 볼 수 있다．

        hort) Message Transmission Substate

  이 상태에서는 우리가 흔히 말하는 단문 메시지, 즉 SMS 전송을 위한 상태이다．
이것은 IS-95에서 이러한 단문 서비스를 제공하기 위해서 설정퇸 Data Burst
入4essage를 통해서 이루어지며, 또 다른 하나의 방법으로는 정상적인 통화채널을
열기 위한 호 절차를 거쳐서, 즉 발호 메시지를 통해서 규정된 Service 師tion을 제
시하고 채녈을 할당받는 방법이 있으나 여기에서 말하고자 하는 방법은 음어］ 이야
   462                                                                         8. IS-95 Call Flow
                                                                                                    U

기한 D毗a Burst Message를 이용한 방법을 이야기하고자 한다．
 참고로 SMS와 관련해서 별도로 瓢4S의 메시지의 Fra工ne 구조와 전송 프로토콜
등을 규정한 규격이 Is寸637이며, 이것은 IS-96, IS-126/127 등과 같은 보코더 규격
이나, IS-707과 갇은 데이터 전송 규격과 갇은 단계의 규격으로 이해하면 될 것이


                                                                        //
                  0            1 40m내너igooa               I뇌 O               초기 상태의 시스
                                rran                                         템 결정 부 상태

                                Yes

                                 lL
                                 ii


                                 O


                                 口1,
                                 Li
                                                                      0VHD MSG 처리

                                 O
                                                                 /
                                 11,                                 Page match operation
                                 Li                                  과 Pa肛 response 지시

                                 0


                                 11
                                 Li
                                                                        Layer 2 처리

                                 0


                                                            -
                                                                 시스템 초기상태의 시스
                                                                 템 결정 부 상태

                      //
                                                            //／戶戶

                           MS 발신 시도                              OVHD 정보 갱신 부 상

                                              烈烈H 태
                           부 상태

                                               State timer expired


                                                                               !

                                              烈烈＝&。可／
                                                    "' " 7l ．태
                                             response혹은
                                         나 maintenance order



                                          "：露罕"eH 向aliza帥？ask
                      //

                      둥록 시도          부                      //
                      상태                        mode
                                          Assign」                Confirmation Initial
                                            = 011"               voice 채널 Task

                      /
                  ，흘츱 '］도 부                   娑＼芋翡 HH
                                              확인올 수신하고
                                                                               통화상태



              （그림 8너7) Sys也m Access 상태 정리
  8. IS-95 Call Flow                              463


다. 즉 IS-95를 기반으로 한 bear에 관련된 규격들이다. 이러한 규격들어］ 대한 이야
기는 앞의 1.7절을 다시 확인해 보시라！
 Access 상태에서 메시지를 전송할 때 호출채널을 통하여 釘4S는 수신하지만 수
신한 메시지의 응답은 전송하지 않는다. 또한 하나의 메시지가 전송 완료되지 않고
전송중일 경우에는 새로운 메시지를 전송하지 않는다．
 이 상태는 선택사항이며, 단말기는 기지국어］ Data Burst 八/lessage를 보낸다. 단
말기가 호출채널의 유실을 선언하면 단말기는 송신을 정지하고 대기상태로 돌아간
다. 이 상태 동안 단말기가 보낸 메시지어］ 대한 응답을 받으면 단말기는 접속시도를
종료한다. 단말기가 GPM를 수신하여 Page 入4atch가 이루어지면 진행중이던 접속
시도를 버리고 호출응답 상태로 천이한다．



       가affic State 처리                                  )
 이 상태는 단말기가 처해지는 통화상태를 나타내며 실지로 이 상태어써 단말기는
가장 많은 전력을 소모하고 가장 바쁘게 움직이게 되며, 가장 많은 정보를 수신하고
발신하는 상태가 된다. 또한 이 상태에서는 앞서 이야기퇸 전력제어나 Handoff 등
의 처리가 이루어지게 된다．

   8.4.1 Service Option

 시스템의 서비스 수용능력을 나타내는 말로서 Service Option은 음성, 데이터，
팩시밀리 등의 응용에 사용퇸다. 이러한 것의 구체적인 적용으로는 발호 메시지나
착호 메시지어］ Service Opti아l 필드이다. IS-95의 초기형태에서는 음성 호 이외어］
는 별다른 서비스가 없었으므로 또 다른 Service 伽tion들이 없었으나 보코더의 종
류도 다양해지며, 데이터호의 종류도 새롭게 정의되어야 할 필요가 있게 됨으로 이
러한 별도의 Service Option들을 정의하고 관리하는 별도의 규격이 정의되기어］ 이
르렀다. 이러한 이유에서 TSB-58, "TIA/EII\ 광대역 확산 스펙트럼 표준안을 위
한 Parameter 값 할당" 에서 Service Option의 목록 을 정의된다.
 TSB占8에서는 Service Option을 정의하기 위해서 다음의 （그림 斗18）과 갇이
각각을 나누어서 그것의 이름을 정의한다.
   464                                                          8. IS-95 Call Flow
                                                                                     1


                                  Service 이川on

          Proprietary                                       Base Service
                              Service Option Revision
          Indicaator                                        Option Numbor
            1 Bit                      3bits                   2 Bits

                    （그림 8-18) Service 야川on Number Format


 Proprietary Indicat아를 나타내는 iBit는 해당 Service Option이 특정한 회사어］
서 정의되어서 구별된 Service Opt幻n인지를 나타내는 것이다．


                （표 8-6) 표준 Service O［川on에 대한 번호할당

 Servk冶 야川on
                                                 설명
 번호 (10 진수）
      1             Basic Variable Rate Voice Service(8kbps)
      2             Mobile Station Loopback(8kbps)
      3             Enhanced Variable Rate Voice Service(8kbps)
      4             Asynchronous Data Service(9.6kbps)
      5             Group 3 Facsimile(9.6kbps)
      6             Short Message Services(Rate Set 1)
      7             Packet Data Service : Internet or ISO Pro切col Stack
      8             Packet Data Service: CDPD Protocol Stack
      9             Mobile Station Loopback(13 kbps)
     12             Asynchronous Data Service(14.4 or 9.6 kbps)
     13             Group 3 Facsimile(14.4 or 9.6 kbps)
     14             Short MessageServices(Rate Set 2)
     15             Packet Data Service : Internet or ISSOProtocol Stack(14.4 kbps)
     20             Group 3 An出og Facsimile (Rate Set 1)
     21             Group 3 Analog Facsimile (Rate Set 2)
                    High Speed Packet Data Service: Internet or ISO Protocol Stack
     22
                    (RS1 forw카d, RS1 reverse)
     32             Test Data Service Option(TDSO)
     33             144 kbps Packet Data Service, Internet or ISO Protocol Stack
    8. IS-95 Call Flow                                    465
1


    Service Option의 1번은 8K QCELP를 사용하는 음성 호이다. 이때까지만 해도
（그림 斗18）의 Service Option 숫자 형태에서 Base Service Option Nun的er만으
로 적용되었다. 여기에서 재미있는 것은 우리나라의 PcS 사업자들이 사용하는
13QCELP의 음성 호를 "000000000001" 의 1의 보수인 "100000000000", 즉 0X8000
으로 정의되었다．
    현재 IS寸弱를 기반으로 하는 우리나라의 이동통신에서 사용하고 있는 Service
O吼ion의 목 록 으 다음의 표와 같다. 물론 이것 이외에도 많은 Service Option들이
있으나 사용상의 문제 또는 기술상의 문제 등으로 여기에서는 생략하겠다．

     8.4.2 Service 구성

    단말기가 통화채널 상태로 동작하고 있을 때에는 단말기와 기지국은 Forw町d과
Reverse 통화채널의 Frame을 교환하면서 통신한다. 이러한 이유로 인해서 단말기
와 기지국은 이러한 Frame을 구성하고 해석할 수 있는 공통의 속성집합들을 공유
한다. 이러한 속성을 우리는 Service 구성이라고 한다. 이러한 속성들은 협상 가능
한 Parameter와 그렇지 못한 Parameter들로 구분퇸다．
    협상 가능한 Service 구성 Parameter들은 다음과 같은 것들로 구성된다．
 ,好띳嶝斟無虹


    다중화 옵션
    이것은 Forw可d와 Reverse 통화채널 frames을 신호, 1차, 2차 통화채널로 나눌
수 있도록 해준다. 즉 Frame의 구성형태를 다중화 옵션이 결정하는 것이다. 이러
한 다중화 옵션은 Frame의 구조와 천송속도를 나타내는 전송속도집합과 연관이 있
다． 이러한 다중화 옵션은 Forward과 Reverse이 같을 수 있다. 이러한 다중화옵션
은 7장을 확인해 보면 될 것이다．
 雄麟發難湘뇨



    채널 Configurations
    IS-95로 규정되는 CDM)\ 이동통신 시스템에서는 특별히 제공된 통화채널（FCH,
SCH）을 변조하기 위해 필요한 모든 정보를 채널 Configuration으로 정의한다. 이
것은 Rad그io Configurations, Frame Size, Interleaver Size, 그리고 Turb可
（노nvol毗ional 부호화의 내용을 나타낸다. 즉 CDMA의 RTT부분을 정의하는 것이
다． 여기에서 Rad由 （允nf坦uration은 （力de Rate, 데이터 전송률, Modulation/
    466                                         8. IS-95 Call Flow
                                                                     U


De跏dulati이l 형태, Symbol-Puncturing Pattern, 그리고 Spreading Rate을 정의
한다． 이러한 상세한 내용은 7장에서 공부한 내용을 참고하라. 이상과 같이 채널
Configuration은 채널의 형상어］ 대한 내용을 정의하는 것이다．


 통화채널 전송속도

 이것은 Forward/Reverse 통화채널을 위해서 실제로 사용되는 데이터 전송속도
이다. 이러한 Forward 통화채널의 전송속도는 통화채널에 지원되는 전송속도집합과
radio Configuration에서 지원되는 모든 전송률 을 말한다. 예를 들면 Fundamental
Channel의 경우 가변속도를 위해서 지원되는 1/2, 1/4, 1/8 속도 집합과 Full Rate
속도집합이 이러한 예들이다. 이와 같은 것은 Reverse에서도 동일한 개념으로 정의
되고 사용된다.
 이러한 전송속도는 Forw可d과 Reverse의 전송률은 각각 독립적으로 설정되고



 Service Option Connections

 Service Option으로 정의퇸 서비스가 사용되는 경우, Service Option 연결과 결
부된 것들을 확인해줄 수 있는 유일한 기준이며, 사용중인 서비스의 특정형태를 구
분하는 Service Option, Service Option 연결을 지원하기 위해 어떤 형태의
Forw可d 통화채널 통화가 사용되는지를 규정하는 Forw可d 통화채널의 통화 형태
와 Service Option 연결을 지원하기 위해 어떤 형태의 Reverse 통화채널 통화가
사용되는지를 규정하는 Reverse 통화채널 통화 형태 등이다．
 이러한 Set자ice Option은 통화상태어］ 제공되는 통화채널 상의 정보 전달매체 혹은
방식 등으로 협상된 특정한 Service 伽tion의 이름으로 제공되지만 초기통화 상태，
즉 채널 할당과정과 협상과정 등의 통화채널은 이러한 Service 伽tion이 필요 없다．
 각 Service Opt幻n과 관련된 것은 Service Opti이l, Forw可（l 통화채널의 통화 형
태, Reverse 통화 형태, Service Option 연결 기준 등이다. 콴련된 Service O吼幻n
은 통화 Bit가 단말기와 기지국어］ 의해서 처리되는 방법을 공식적으로 정의한다. 관
련퇸 Forward/Reverse 통화 형태는 Service Option을 지원하는데 사용된 통화 형
태를 규정한다. Service 伽tion은 특정한 통화 형태의 사용을 요구할 수 있거나 하
나 이상의 통화 형태를 받아들일 수 있다. Service Option은 단방향일 수 있는데,
    8. lS-95 Call Flow                                467
.


이 경우 恥rw可d 통화채널에서만 Reverse 통화채널에서만, 또는 Forward이나
Reverse 통화채널에서 지원될 수 있다. Service O砒ion이 양방향일 수 있는데, 이
경우 Forward/Reverse 동시어］ 지원될 수 있다. 관련된 Service Option 연결 기준
은 Service O砒幻n 연결을 유일하계 인식하기 위한 수단을 제공한다. 이 기준은 여
러 개의 Service O就ion 연결이 사용중일 때 혼란을 방지한다．
    단말기와 기지국이 공통으로 관리하는 Service 구성은 협상이 불가능한
Parameter로 있다. 이러한 non-negotiable Service 구성 Parameter는 기지국에서
단말기로 통보되는 Parameter들이며 다음과 같다. 협상 불가능한 항목이므로 단말
기는 기지국으로 이 항목들어］ 대해서 대안을 제시할 수 있는 사항이 아니다．


    Reverse Pilot Gating Rate

    이것은 Reverse Pilot의 Gating 속도를 제어하는데 사용되는 것으로 기지국은 서
비스 （노nnect Message어］ 사용하게 될 Reverse Pul毗의 gating rate을 표시한다．
이러한 내용은 Supplemental Code Channel과 Supplemental Channel의 할당과
관련된 General Handoff Direction 八4essage(GHIDM), Un如ersal Han耐I
Direction Message(UI끄呱1)에서도 이러한 정보를 포함한다．


    Forward과 Reverse 전력제뻐 Parameter

    전력제어, 즉 Forw可d Fundamental Channel 및 DCCH의 전력제어 모드와 외
부 루프 전력제어 Parameter와 다중화되는 전력제어 부채널 등의 정보로 구성되는
값이다．


    Logical to Physical Mapping

    이것은 논리채널을 물리채널로 대응하게 해주는 테이블의 내용을 말하며, 서비스
기준 식별자， 논리적 자원， 물리적 자원, Forward 및 Reverse I江ag 그리고 우선 순
위 등으로 구성되어 있다．


     8.4.3 Service 협상

    단말기는 호 발생시 Service O吼幻n과 관련된 디폴트 Service 구성을 요구할 수
있고 통화채널 동작 동안 새로운 Service 구성을 요청할 수 있다. 요청된 Service
    4亡）8                                                 8. IS-95 Call Flow
                                                                              .


구성은 그전의 것과 크게 다를 수 있거나 매우 비슷할 수 있다. 예를 들어서 단말기
는 모든 Service Option 구성이 현재구성과 다른 Service 구성을 요청할 수 있다．
또는 현재 Service Option 연결이 작은 변경만으로 유지되도록 Service 구성을 요
청할 수도 있다．
 이러한 Service Option은 초기어］ 발호 메시지나 호출응답 메시지에 의해서 제안
된 Service Option어］ 대해서 망이 대안을 제시하는 것으로 시작된다. 이러한 협상
여부에 대해서 IS-弱에서는 Ex扼nded Channel Assignment Message(ECM山 혹
은 Channel Assignment Message(CAM)의 ASSIGN_MODE와 GRANTED_
MODE의 값에 의해서 시작된다. ASSIGN소4ODE는 통화채널과 호출채널을 할당하
는데 사용되나 여기에서는 통화채널 할당어］ 대한 이야기만 하겠다. 즉 이 값이 '100'일
때 통화채널을 할당하겠다는 이야기가 된다. 나머지 필드는 Service 협상을 하기 위한
조건, 즉 협상시점과 협상을 위한 채널의 형상어］ 대해서 정보를 제공해 주는 필드이다．
 Service 협상과 관련된 사항을 다시 정리하면 초기 통화채널과 관련퇸 정보는
ECAM을 비롯한 CAM에서 제공되고 최종적으로 연결될 통화채널과 관련된 정보
는 Service Connection Completion Message어］서 이루어진다. CM匹의 ASSIGN1
MODE와 GRANTED_MODE에의한 사항을 정리하면 다음과 같다.


                        （표 &7) Defau仕 ConfI叩ration

 값（2진수）                          Detault Configuration
   000     Forward在teverse 통화채널을 위해 다중화 옵션1과 RC1
   001     Forward在teverse 통화채널을 위해 다중화 옵션2과 RC2
           Forw可d 통화채널을 위해1 다중화 옵션1과 RC1; Reverse 통화채널을 위해 다중
   010
           화 옵션2과 RC2
           Forw町（l 통화채널을 위해1 다중화 옵션2과 RC2; Reverse 통화채널을 위해 다중
   011
           화 옵션1과 RC1
           FOR_FCH_RC혹은 FOR_RC는 Forward Fundamental / De小cated Cont이
           채널을 위한 이 메시지에 포함되며， REV_FCI-LRC 혹은 REVHRC는 Reverse
           Fundamental / Dedicated Contr이 채널을 위한 이 메시지에 포함된다.20단말기
   100
           frame을 사용한다. 9600bps의 bit rate을 포함하는 radio Configuration을 위한
           다중화옵션1을 사용한다； 해서            14400bps의 bit rate을 포함하는 radio
           Co而guration을 위한 다중화옵션2을 사용한다．
                              Reserved
    n    1 rN   n   尸   r\   4 11   尸 1 =                 r
                                                               H   1
    0. I D-dO LiII                  now
1

    米 GRANTED소4ODE = '00' 혹은 '01' 인 ECAM을 수신하였다면, 단말기는 현
        재까지 자신이 가지고 있는 Configuration어］ 대한 Service 협상을 기지국이 서
        비스 Connect Message를 전송하기 이전어］ 시도하여야 한다．
    木 GRANTED소lODE = '10' 을 수신하였다면, 단말기는 현재까지 자신이 가지
        고 있는 Configuration어］ 대한 Service 협상을 기지국이 서비스 Connect
        八4essage를 전송하기 전에는 시도하지 않아야 한다．
    半 GRANTEI工MODE='00'인 경우어］, 단말기는 초기 Service 구성을 （표 &7)
        Default Configuration어］ 정의된 Default Configurations중 하나를 사용해야
        한다.
    求 GRANTED小IODE= '01' 혹은 '10' 인 경우, 단말기는 초기어］ 요구퇸 Service
        Option과 부합되는 Default 入lultiplex 伽tion과 Transm始sion Rates으로 구
        성된 초기 Service 구성을 사용해야 한다．
    Service 협상이 시작되는 시점이 언제인가라는 질문을 간혹 받는다. CAM이후
초기 통화채널 상태에서 서비스 Request/I扼sponse Message들을 사용해서 협상을
하는 것이 그것의 시작일 것이다. 그러나 어떤 의미에서는 Preferred Service
Option과 I노eferred Radio Configurations을 제안하는 Origination Message 혹은
Page Response 八4essage어］ 명시된 Sei刀ice Option이 Service 협상의 시작이라고
생각할 수도 있다．
    Service 협상은 Service Option협상과 RC, 다중화 옵션, Coding Scheme 등을
포함하는 서비스 Atti化ute 협상으로 나눌 수 있다. 이러한 Service 협상은 서로서로
연관되어 있으며, 하나 협상 절차에서 여러 단계로 진행될 수 있다. Service Option은
앞서서 이야기되었듯이 포괄적인 속성들을 포함하므로 모든 것이 바뀔 수도 있다．

    Service 협상 절차
    서비스 형상 속성（Atrribution) 협상은 Service O就ion 협상이 이루어지고 있는
동안에도 협상이 이루어질 수도 있다. 또한 단말기는 앞서 이야기된 Service
O야ion들어］ 대해서 Service Option의 속성들을 나타내는 Applicable Service 구성
/＼杭ributes (ASCA）을 관리해야 한다. 즉 Service Option은 이러한 속성들의 전체
를 나타내는 개념이라고 할 수 있다. 또한 Preferred Service Option과 연관된
Preferred 서비스-Conf地uration Attributes (SCA）을 선택하여 발신 호 혹은 착신
    470                                             8. IS-95 Cal l Flow
                                                                          U


응답 호를 시도한다．
 단말기에서 제공할 수 있는 Service Option으로 기지국이 단말기를 호출한다면
혹은 단말기가 기지국으로 요구한다면, 단말기는 기지국어］ 의해서 제안된 Service
Om幻n과 연관퇸 SCA를 확인하고 다음의 절차를 수행해야 한다．
 SCA내의 임의 값이 타당하지 않다면, 단말기는 ORDQ = '00000100'의 Mobile
Station Reject 아der를 전송하여 "메시지 필드가 타당한 범위가 아니다"라고 통보
한다．
 SCA Parameter들이 모두 ASCA에 있다면, 단말기는 제안퇸 속성들로 호를 설
정할 수 있으므로 서비스 제안을 수락한다. 반면 만약 SCA Parameter들이 타당하
나 그것들을 모두 적용할 수 없다면 단말기는 적용 가능한 항목은 선택하고 일부
속성을 수정하여 수정된 제안으로 응답한다. 예를 들어서 기지국이 "Service
Option = 33, RC = 3, Mux Option = 0x0911, FEC = Convolutional Code"로 요
구하였다면 단말기는 "Service (珀lion = 33, RC = 3, 入4ux Option = 0x0911, FEC
= Turbo Code" 로 응답하게 된다．
 만약 단말기가 지원하지 않는 Service Option으로 기지국이 호출된다면, 단말기
는 Service O吼ion 협상 규칙어］ 따른 Service O吼ion으로 응답해야 하며, 그
Service Option과 연관된 Preferred SCA를 선택하여야 한다.
 만약 협상 절차어］ SCA를 포함하지 않는다면, 단말기는 Default SCA를 선택하
여 사용해야 한다．


 Service 협상의 종료조건

  단말기는 기지국이 단말기의 입장에서 타당치 않는 서비스를 요구했을 때 단말기
가 이를 거절하고, 기지국이 如lion을 취할 때 까지 기다리고 있을 때 최종적으로
기지국이 호를 포기하기로 결정할 때어］ Service 협상은 종료된다．
  또한 기지국이 제안하는 Service Option들의 목록과 관련된 ASCA의 모든 것들
을 비교하였으나 더 이상의 대안이 없을 때, 단말기는 ORDQ='町刃0110'인 八/lobile
Station Reject Order를 전송하여 "가장 최근어］ 단말기어］ 의해서 제안될 수 있는
Capability를 요구"를 전송하게 된다. 이것 역시 협상이 종료되는 경우이다. 이러한
상태 이후어］ 기지국에서는 기지국은 호를 포기하거나 타당한 SCA를 다시 선택하
여 또 다른 Service 협상을 시작할지를 선택한다．
      8. IS尸95 Call Flo버／
 .                                                                         471




     Service Option 헙상규칙
     단말기와 기지국은 Service 구성 협상의 대체방식으로 Service 0砒幻n 협상을
사용한다. Service 0吼ion 협상은 Service 협상과 비슷하지만 Service 구성의 성분
들을 구체적으로 나타내는 기능이 없으El로 유동성이 떨어진다고 할 수 있다．
Service Option 협상 진행 중에는 기지국 혹은 단말기는 사용할 Service Option만
을 상술하여야 한다. Service Option과 연계된 Forward/Reverse 통화채널상에서
사용되는 다중화 옵션, Traffic Types 혹은 전송률 등을 구체적으로 상술하기 위한
형식이 없으나 묵시적인 Service 구성 성분들이 있다. 특별히 Forw可d/Reverse 다
중화 옵션과 전송률은 요구된 Service Option과 연계된 Default 入Iultiplex Options
과 Transmission Rates으로 가정되며, Forward/Reverse 통화채널 모두를 위한
Traffic Type은 Primaiy Traffic로 가정된다. 따라서 Service Option 협상을 사용
하여 형성퇸 Service 구성ion은 단일 Service Option Connection만 가질 수 있도
록 제한된다. 즉 Service 협상은 여러 개의 Service 0挑ion 협상의 결과를 가진다
고 할 수 있다．
     단말기는 발신과 착신에서 Service 협상을 할건지 Service Option 협상을 할컨
지를 Channel Assignment 八/Iessage어］ 의해서 할당되는 채널어］ 따라서 구별된다．
이것은 ASSIGN小'JUDE에 의해서 결정된다. ASSIGN소'JUDE에 Service 0姚ion
협상으로 이루어져야 할 통화채널이 할당되지 않는 E砒ended Channel Ass坦n
ment Message를 수신한 이후에는 항상 Service 협상만으로 서비스를 하여야 하며，
Hard Hando珏시 새로운 기지국과의 협상의 형태는 Ex扼nde可Gener川／ Universal
Handoff Direction Message 등과 같은 Handoff 메시지어］ 의해서 결정된다．
 단말기는 이러한 형태의 협상들을 제공하기 위해서 단말기가 최우선적으로 사용하
기를 원하는 Service Option인 Preferred Service Option을 가져야 하며, 이것어］ 따
라서 대치될 수 있는 Alternate Service Option의 목 룩 을 다음의 （표 斗8）과 구분해
서 관리한다．
                            （표 &8) Service 야川on Categories
          서비스 Type                   F가이erred So             ／싸ernate So
             Voice                        3                   l .OX 8000
        Low Data Rate                    15                       7
      八4e小urn Data Rate                  25                    22, 15, 7
        High data rate                   33                       33
   472                                     8. IS-95 Cal l Flow
                                                                 1


 이러한 방식의 경우 IS弱초기에는 지원되지 않았으나 망의 발전으로 인해서 서
비스의 형태가 다양하찌고 이러한 다앙한 형태의 서비스들을 최종적으로 망과 단말
기가 설정완료하기 위해서 Service Option들을 공통된 Category로 구분해서 관리
하는 방식이라고 이해할 수 있다．
 기지국이 단말기가 제안한 SO어］ 대한 응답으로 새로운 Service Option을 제안할
때 단말기가 지원하지 않는 SO으로 요구할 경우어］, 단말기는 Alternate 목록이 다 소
진될 때까지（협상 실패） 혹은 기지국이 단말기가 지원하는 Service Option으로 응답
할 때（협상 성공）까지 서비스 Tyl光을 Altei끄ate 목록상의 Service Option들로 계속
제안한다．
 단말기는 발신 호의 Service 伽tion과 관련된 default Service 구성을 요구할 수
있으며, 통화채널이 동작중일 때어］ 새로운 Service 구성S을 요구할 수 있다. 요구된
Service 구성은 그것의 앞의 Service 구성과 매우 유사할 수 있거나 혹은 엄청나게
다를 수도 있다. 예를 들어서, 단말기가 존재하는 Coi出guration의 Service Option
connecti아鳩의 Service 구성 요구할 수 있다. 혹은 전송률, Service Option
connection을 Forward/Reverse 통화채널 type으로 mappir增의 차이와 같은 사소
한 변화만 유지되는 Service Option c아mection이 존재하는 Service 구성을 단말
기는 요구할 수 있다．
 만약 단말기가 기지국이 수용할 수 있는 Service 구성을 요구한다면, 기지국과
단말기는 모두 새로운 Service 구성을 사용하기 시작할 것이다. 만약 단말기가 기
지국이 수용할 수 없는 Service 구성 을 요구한다면, 기지국은 제안퇸 Service 구성
을 거절하거나 alternative Service 구성을 제안할 것이다. 만약 기지국이
alternative Service 구성을 제안한다면, 단말기는 기지국의 제안된 Service 구성을
수용하거나 거절할 수 있으며, 혹은 또 다른 Service 구성을 제안할 수 있다. 이러
한 과정은 이름하여 Service 협상, 단말기와 기지국이 상호 수용할 수 있는 Service
구성을 찾거나 혹은 단말기든 기지국에서 또 다른 것어］ 의해서 제안된 것을 거절할
때에 종료된다．
 단말기는 Service 구성과 협상을 지원하기 위해서 서비스 부 기 능 들 을 수행한다．
이러한 부 기능들은 사용자와 기지국으로부터의 Service 구성 요청을 수행하는 정
규 서비스 부 기능과 서비스 요청 메시지와 서비스 응답메시지를 기다리는 서비스
요청／응답 부 기능, 서비스 연결 메시지를 기다리는 서비스 연결 부 기능, 새로운
    8. IS-95 Call Flow                             473
U


Service 구성과 관련된 활성시간 동안 대기한 후 서비스 연결 완료 메시지를 송신
하는 서비스 활성시간 부 기능을 수행한다．


     8.4.4 Service 구성과 협상을 지원하는 메시지

 이것을 지원하는 메시지들은 다음의 목록과 같이 정리될 수 있다．
 Service Request 八4essage는 기지국과 단말기는 이 메시지를 사용해서 Service
구성을 제안하거나 Service Resi刃nse 八/Iessage에서 제안퇸 Service 구성을 거절하
는데 사용할 수 있다. 이와 비슷한 기능을 하는 메시지가 Service Response
Message이며, 이 둘은 Service 협상을 하는데 제안하려는 서비스의 형상을 전송하
며 협상의 주도하는 메시지들이다.
 Service Connection Message는 위의 서비스 요구 및 응답 메시지에서 제안된
Service 구성을 기지국이 수용할 때 단말기에게 이러한 형상으로 Service 구성을
사용하자고 통보하는 메시지이다. 이때 단말기는 Service Connecti이i Compete
Message를 통해서 해당 Service 구성으로 전환되었음을 알리게 된다．
 추가적으로 Service Option의 특정기능을 발생하는데 사용하기 위해서 기지국과
단말기는 Service Option Control 八1essage를 사용하기도 한다.
 또한 기지국은 단말기의 상태를 확인하기 위해서 Status Request Message를 사
용하며, 단말기는 자신의 capability정보를 Status Response 八4essage로 전송하게
퇸다．
 이러한 상기의 메시지들은 통화채널상에서 Service 구성정보를 전송하여 협상을
지원하는 메시지들이다. 그러나 대기상태의 호출채널이나 /\ccess 채널을 통해서도
이러한 Service 구성은 제안되고 협상의 과정을 거친다. 다시 말해서 우리가
Service 협상이라는 개념을 통화상태에서 발생되눈 것이라고 제한하지 않는다면 발
신 메시지나 호출응답 메시지, 호출메시지, 채널 할당 메시지에서도 벌써 Service
구성어］ 대한 제안과 거절의 절차가 이루어지고 있음을 기억할 필요가 있다．


     8.4.5 Long Code 천이

 호를 처음 발의하는 호출 응답 메시지나 발신호 메시지어］ 음성비화 모드가
enable되어 있다면 기지국은 초기 통화채널 상태어］ 단말기로 개인용 Long Code
로 전의할 것을 요구하는 긴 코드 전의 요구명령幻RDQ山0000001）을 전송한다．
   474                                   8. IS-95 Cal l Flow
                                                               U


 이때 단말기가 개인용 긴 코드를 발생가능하고 단말기가 이 요구를 수행한다면
단말기는 0.2초（T56m) 내어］ 개인용 Long Code로 천이되어 사용한다는 응답명령
幻RDQ=00000(표1）을 보낸다. 이후 단말기는 Forw可d과 Reverse 통화채널어］ 개인
용 Long Code를 사용한다. 이러한 절차는 메시지어］ 규정된 실행시간 내어］ 이루어
진다. 그리고 단말기는 음성보안 모드가 활성된 것을 사용자에게 알려준다. 이때
Forward과 Reverse 통화채널은 개인용 긴 코드로 변조된다．
 기지국으로부터 그러한 요구가 있었으나 단말기가 개인용 긴 코드를 발생할 수 없
거나 그 요구를 혀락하지 않아서 수용할 수 없다면 단말기는 0.2초（T弱m) 이내어］ 공
용 Long Code를 사용하여 통신할 것이라는 Long Code 천이 응답명령（ORDQ=
00000010）을 전송한다. 이때 Forward 및 Reverse 통화채널은 공용 긴 코드를 사용
한다．
 역으로 기지국이 Long Code 천이 요구명령이 공용 Long Code의 천이를 요구
(ORDQ=00000000）하고 단말기가 이 요구를 수용한다면 단말기는 0.2초（T弱m) 내어］
긴 코드 천이 응답명령（ORDQ=0000X끄0）을 보낸다. 단말기는 음성보안 모드가 활성화
되지 않았음을 사용자에게 알려준다. 또한 기지국의 이러한 요구를 수용할 수 없을 때
단말기는 0.2초（T弱m) 내어］ Long Code천이 응답명령（ORDQ=00刃011）을 보낸다．


  8.4.6 통화 상태의 Sub State관리

 통화 상태에서도 부 상태들을 관리한다. 이 상태에서는 F아＼V町d과 Reverse 통화
채널을 사용하여 기지국과 통신하게 된다. 다음의 （그림 &19）과 같이 단말기의 제
어는 각각의 부 상태들로 이루어진다．
 단말기가 Forw可d 통화채널을 수신할 수 있고 Reverse 통화채널로 전력을 송출할
수 있는 기본단계를 설정하는 단졔인 초기 통화채널 상태와 Ale此 With Info珏nati아l
Message를 기다리는 명령 수신 대기 부 상태, 착신호인 경우 사용자가 응답하기를
기다리는 상태인 응답 대기 수신상태, 현재 Service 구성어］ 따라서 통화채널 Frame
을 기지국과 교환하는 대화상태 그리고 마지막으로 호를 절단했을 때인 해제상태로
구분되어 관리된다．


      널 초기 부 상티1
 이 상태에서 단말기는 Forw可d 통화채널을 수신할 수 있고 Reverse 통화채널로
 8. IS叫95 Call 디ow                                                      475




                단말기 斗신 호 상타回1 순빙향 통
                통해74 ：小I 국 확인 밍 령읖 수 :Ji




                                                        단딸기 빨且｝ 호 싱
                                                         어］ 순방향 통화
             Malntenance 명                              넉읕 봉해 之｝ 기
             Alert with info                            H; 확인 명 三寸，‘年
             加lessa昏샤나1                                  m} '겄다




                               芬단발기 사욤싸가 Call에 대a斗／'I

                           （그림 &19) 통화채널의 부 상태


전송을 시작할지를 확인해 주는 단계이다．
 구체적으로 이 상태에서 단말기는 등록관련 Parameter들을 초기화하고, 확인절
차를 Reset한다. 그리고 Forward 전력제어를 초기화한다. 이러한 것들은 새로운
상태로 진입하여서 맨 처음 단말기의 내부 데이터들을 정리하는 단계로 이해할 수
있다. 또한 단말기는 이 상태에 초기 Service 구성을 Access 상태의 채널 할당 메
시지의 GRANT小tIODE 필드를 통해서 다르게 구성하게 된다．
 즉 그 값이 '00'이면 초기의 Service 구성은 Forward 및 Reverse 통화채널 모두
다중화 옵션1과 전속속도를 RS1을 사용한다. 이러한 경우가 아닐 때인 GRANT
MODE 필드가 '01' 혹은 '10'이면 초기의 Service 구성은 단말기가 관련 메사지들
을 통해서 요구하는 Forward 및 Reverse 통화채널 다중화 옵션과 송신속도 사용
한다. 이러한 초기 Service 구성은 Service Option어］ 의한 접속을 말하는 것이 아
니다．
 이 상태에서 단말기는 새로운 상태에서 기지국으로부터 오는 색다른 신호어］ 대해
서 새롭게 수신할 수 있는 준비작업을 하게 퇸다. 즉 PILOT下N의 Pu毗을 통해서
Forw可d 통화채널을 지속적을 감시를 하게 되며, 할당된 CDMA 채널어］ 동조하며，
    476                                8. IS-95 Call Flow
                                                            .


이러한 Forward 통화채널로 자신의 Code Channel을 설정하게 된다. 그리고
For기刃可d과 Reverse 통화채널 Frame 옵셋을 FRAME OFFSET에 의해 결정된
할당 Frame옵셋으로 설정하면 단말기는 수신을 위한 기본적인 준비는 이루어진 것
이다. 그리고 Reverse 채널을 위해서 Forw可d Reverse 통화채넘 긴 코드 마스크
를 공용 Long Code 마스크를 설정한다．
  이렇게 단말기가 튜닝된 상태에서 정해진 시간 이내（T晟hn:l초）어］ 타당한 Frame
(N5m）이 연속적으로 양호하게 수신되는지 여부를 가지고 현재 수신하고있는 통화채
널이 안정적인지를 판단하게 된다. 여기에서 안정적이지 못한 상태로 판단되면 단
말기는 통화상태를 더 이상 유지할 수 없고 시스템 소실로 초기상태의 시스템 결정
상태로 빠지게 퇸다. 이것은 앞서서 모든 값들을 단말기가 초기화해버렸고 새롭게
시작하햐 하기에 초기상태로 천이되는 것이다．
 그렇지 않고 지금 수신하고 있는 통화채널이 안정적인 상태라고 판단할 수 있는
경우에는 전력제어어］ 의해서 정의된 전력으로 송신전력을 조정하며, Forward 통화
채널로 내려오는 통화채널 프리엠블을 수신하게 된다．
 이 상태에서 특정한 시간（T51m:2초） 이내어］ 기지국으로부터 확인명령（BS Ack
Order）을 수신하지 못하더라도 단말기는 초기상태로 빠지게 된다. 이러한 확인절차
는 단말기 혼자만의 상태가 아니라 망과의 상호 연동된 상태를 확인하기 위한 절차
로 이러한 확인이 되지 않는다면 단말기는 현재 단말기의 상태（Forw町（I 채널이 양
호한 경우）는 불문 Reverse이 문제가 되고 있다는 판단에서이다.
 이러한 상태에서 채널 할당 메시지가 Service 헙상을 필요로 한다면 정규 서비스
부 기능을 활성화시키고 협상이 필요 없다면 서비스 연결메시지 대기 부 기능을 활
성화시킨다. 또한 이러한 호가 발호인 경우는 대화 부 상태로 천이하고, 착 호인 경
우는 명령 대기 부 상태로 들어간다. 즉 링 백톤을 듣게 된다．


 명령 대기상태
 이 상태에서는 단말기는 모든 처리를 이 상태에서 메시지를 기다릴 수 있는 최대
시간 T52m(5초）만큼 기다리기 위해서 타이머를 설정한다. 이 기간은 /\Je此 with
Information Message의 수신 대기상태이며, 이 기간 중에도 단말기는 앞서 이야기
한 초기 통화채널 상태에서 수행하던 더 정확히 말하면 통화상태에서 이루어질 수
있는 전력제어와 Han（如ff 등을 수행한다．
    8. IS-95 Call Flow                                                                477
.

    특히 이 상태에서도 사용자어］ 의해서 제안된 서비스어］ 대해서 망과 협상하는 과
정이 있다. 이러한 필요가 있을 때에 단말기는 활성 서비스 부 기능어］ 의해서 이러
한 Service 협상을 수행하게 된다．
    좀더 구체적으로 이야기하면 서비스 제어 메시지를 통해서 Service Option의 특
정기능을 수행할 수도 있고 긴 코드 천이과정도 이루어질 수 있다. 물론 이 상태에
서 단말기 사용자어］ 의하써 전원이 꺼진다면 해제상태로 천이되어야 할 것이다．
    이 상태에서 인증시도가 있을 수 있으며 등록절차가 수행될 수도 있다. Pilot 측
정 요구에 의해서 측정 보고가 있을 수 있으며 ，상태요구에 의한 응답기능도 이 상
태에서 이루어져야 할 기능들이다.


    단말기 응답 대기상태1
    이 상태에서는 단말기는 모든 처리를 이 상태에서 메시지를 기다릴 수 있는 최대
시간인 T3m(5초）만큼 기다리기 위해서 타이머를 설정한다. 이 기간은 단말기가 착
호일 때 발생될 수 있는 상태로 착 호어］ 대한 응답대기 상태를 말한다．
    이 상태는 앞서 설명한 명령대기 상태와 유사하다. 다음의 （그림 斗20）은 단말기
응답대기 상태와 명령대기 상태를 시간별로 구별한 것이다．


                         SReqM   SRepM   SCM      SCCM    AWIM     Hang up

                                  A                A

                          V                                                      -




                   I 초기 통화상태             CAM : Channel Assignment Message
                                         SreqM : Service Request Message
                   I 명령 대기상태             SrepM : Service Response Message
                                         SCM : Service Connection Message
                     단말기 웅답 대기상태         SCCM : Service Connection Complete Message
                                         AWIM : Alert with Information Message
         H           통화 대화 상태


                                  （그림 &20) 시간정렬



    통화 대화 상태
    이 상태가 진정한 통화상태로 이 상태에는 협상으로 최종적으로 결정된 서비스
자원들로 서로 Frame을 교환하는 통신을 수행한다. 이 상태에서는 Hando卄와 전력
        478                                      8. IS-95 Call Flow
                                                                      1


 제어를 수행한다. 단말기가 발호 메시지로 호를 시도하였으나 다이얼 디지트를 모
두 전송하지 못했을 경우에는 o姮ination (노砒inuation Message를 사용해서 전
송하게 된다．
  사용자가 단문 메시지를 전송하려고 하면 이때 단말기는 data bt玎St message를
통해서 단문 메시지를 전송하게 된다. 이것은 통화중 전화번호를 전송한다튼가 하
는 경우라고 이해하면 된다. 또한 ARS 서비스 등에서 사용될 수 있는 DTMI구 전송
도 이루어질 수 있다．
  이 상태에서도 물론 새로운 서비스 형상을 위한 Service 협상도 지원이 되며, 음
성비화를 위해서 긴 코드의 사용을 선택할 수도 있다. 또한 사용자가 특별한
Service Option의 요구를 위해서 order를 전송할 수 있으며, 이때 사용하는 ORDQ
값은 원하는 Service Option번호로 설정한다．


  호 해제상태

  호 해제상태로 진입하면 2초간 동작 후 만료되는 상태 타이머 T爵TI을 작동시키
며， 이러한 시간이 지난 후에는 초기상태의 시스템 결정 부 상태로 천이된다．
  전원 차단에 의한 호의 해제인 경우 ORDQ＝以X00X끄의 release order를 전송하
며, 그렇지않고 기지국이나 단말기에 의해서 정상적으로호 해제인 경우는 ORDQ=
Dcx刃0000의 release order를 전송하여 호 해제를 구분한다．
  호 해제 부 상태에서는 전력제어와 Han面什를 여전히 수행하며 통화채널상에서
기지국과 단말기간의 연결을 유지하기 위해서 16개의 1과 8개의 0으로 구성된 Null
Tra佈c data를 12(）兀PS로 송신한다. 일종의 K叫）寸Alive 동작이라고 할 수 있다.
그리고 등록 타이머를 관리한다. 이 상태에서도 단말기는 기지국으로부터의 각종
명령 메시지를 처리한다．



  8.5    단맏:7 ' 식범과 보안
                                                                      1
   8.5.1 단말기의 식별

 CDMI\ 단말기를 CDMA망에서 식별하기 위해서 l5digit까지 사용할 수 있는
IMSI(International Mobile Station Iden蹴y）를 사용한다. 즉 idigit는 丁9까지 표
시될 수 있고 2진수로는 4 Bit가 필요하므로 IMSI는 모두 15자리의 16진수로 표시
    8. Is尸95 Call F幻w                                                                                479
.


될 수 있다. 이러한 IMSI는 다음의 （그림 &21）과 같이 표시된다．


                 15                13 12                11
                             MCC              MCC                              MSIN


                 =3digit
                                        十
                           MCC: Mobile Country Code
                                                                      NMSI
                                                              IMSI (15d泫卄이하）
                                                                                              :
                           MNC: M야川eN飢work Code
                           MSIN: Mobile Station Identification Number
                           NMSI: National Mobile Station Identity
                           IMSI: International Mobile Station Identity


                                                       （그림 &21) IMS떽 구조


    우리는 여기서 소위 말하는 전화번호에 해당되는 IMSLS를 생각해 본다. 이것은
IMSI에서 파생된 것으로 10 digit, 즉 34 Bit를 가지는 것이다．
    lOdigit의 IMSLS는 3digit와 7digit로 나뉘고 이를 각각 IMSLS2, 瓜4S1_S1이
라고 한다. 이것은 다음의 （그림 &22）어］ 나타나 있다．


                                                        첫 번째         두 번째         천 자리     마지막
          IMSI寸SI万git 寸Um1＝
                          卜                             3 Di죵It      3 Di포it       Digit   3 DigIt
                                                         xxx           xxx          x       xxx

          Bits                     H=   m1=   H=   +         10         10            4      10

          사용 번호 예 m1+                                        019       219            2     269

                                              （그림 &22) IMSI_S 이진 Ma口口ing



     8.5. 2 小'ISI_S의 부호화

    IMSI_S의 2진 八1appii培은 단순히 2진수로 변환이 아니라 암호화 가정으로 이루
어진다. 즉 lOdigit를 3, 3, 1, 3으로 구분하고 3Digit 식 나누어진 부분들은 다음과
같이 C어玉ng한다．
    非 3digit의 상위 digit부터 I万, D2, 1거이라고 나타내고, 그小git의 값이 0인 경우는
     10으로 생각한다．
   480                                              8. IS-95 Call Flow
                                                                         U


 米 3dig此는 (D3 x 1（刃＋D2X 10+1거）로 정리한 후 그 값어］ ill을 뺀다．
 水 이 결과치를 2진수로 변환한다. 이때 결과치가 10자리가 되지 않으면 상위의
   나머지 Bit들을 0으로 채운다．
 IMSI_Sip의 천 자리의 1 digit는 다음의 （표 斗9> BCD대응의 값들처럼 BCD변
환법어］ 의해서 4 Bit로 Mappii坦된다．


                           （표 &9) BCD대응

     십진수                이진수              십진수               이진수
         1              0001              6                 0110
         2              0010              7                 0111

         3              0011              8                 1000
         4              0100              9                 1001
         5              0101              0                 1010


             019-219-2269라는 1MSI_S는 어떻게 mappir堆되겠는가7

             첫벗째로019 : (loxloo+lxlo+9) -111 = 908 = 1110001100(2)
             이다. 즉 2진수 ()011 1000 1100로 표시되며 이 값은 出:38C 이다．
             그리고 219 : (2x100+1X 10+9) -ill   = 108 = 0001101100(2) 이며，
             2: 0010(2) 이다. 그리고 마지막으로 269: (2x100+6x10+9)-111
             =158 = 0010011110(2) 이다．
             즉 0192192269는 이진수 "0001 1011 0000 1000 1001 1110"로 표시
             되며, 이것을 Hexa (16진수）로 표시하면 0x1B089E이다．
             따라서 종합하면 IMSLS = IMSJ. S2p+ IMSI_Sip = （뇨：3＆그＆)8狙이다．

  8.5.3 Hash 함수

 일반적으로 단말기가 망어］ Access하거나 자원할당은 아주 랜덤하게 이루어진다．
이러한 이유로 망에서는 단말기가 /\ccess할 수 있는 자원의 배분을 아주 공평하게
하도록 해 주어야 한다. 특정한 주파수나 호출채널에만 단말기가 집중된다면 큰 문
제가 아닐 수 없을 것이다．
 이러한 문제를 해결하기 위해서 단말기는 주파수 채널, 호출채널, Access 채널을
    8. IS-95 Call Flow                                       481
.


할당받을 때 자원을 확률적으로 균일화시키는 함수인 Hash함수를 사용한다. 이러
한 hash함수는 이고 one way function으로 가역정리가 수행되지 않는伍4essage
digest function) 함수이다．
    이 함수는 단말기의 IMSI나 ESN中S, 서비스받을 수 있는 자원의 수N, 수정자
DEC아｛R을 변수로 사용하여 정수를 반환한다. 수정자는 같은 단말기로부터 여러
가지로 응용시어］ 얻어지는 값들간의 상관관꼐를 제거하는 역할을 한다.
    만일 해싱 함수가 액세스 채널의 PN랜덤화를 결정하고자 한다면 I끄＼SHJ(EY는
단말기의 ESN_S와 값이어야 한다. 만일 다른 목적어］ 사용되고자 한다면 HASH
KEY는 IMSI_S의 최하위 Bit와 갇아야 한다．
    Hash함수를 위해서 사용되는 HASYJ(EY는 다음과 같이 정의된다．
          HASY_ KEY=IMSImO_ S1+ 224xIMSI_ O_ S2의32LSB

    위 식에서 구하찐 값에서 L은 HASY KEY의 丁15 Bit까지이고, H는 HASY
KEY의 16-31 Bit까지이다. 또 JMSI_O_S2어］ 224을 곱하는 것은 16진수의 자리
수를 6자리 앞으로 당긴다는 의미로 IM釘j工S2를 IMSI巾O尸Si만큼의 자리옵셋을
보상하1 준 것이라고 볼 수 있다. 이렇게 해서 hash값 R은 다음과 같이 구해진다．

           R＝뇨｛伽曲的／7e毗CORR)}m0d2'6 1                          (8-12)
                    L                      2'"          J
    이렇게 구해진 hash값은 CDMA 채널 number, 호출채널 number Forward
common control 채널 number, Quick 호출채널 number, 호출 Si毗 number 등을
계산하는데 사용된다．
    또한 Quick 호출채널 indic毗아의 위치를 결정하는 hash 값은 또한 다음과 같이
정의된다. 이것은 伽ick 호출채널의 data rate어］ 따라서 달리 구해진다．

          R. - I ,",
          "D     Nx  V {40503x (L0 H今 DECCORR)}m0d2'6
           "'   -   L   "   八              216          _I
    4800bps인 경우

          R. =N+ 4+1-쯔仁쁘＋
            '                   LN+ 4i 2


          [(1 [쓴d片儡I(N+4
                      2 {40503
                            x(L H' 216
                                   DECCORR)
                                        }mod216
    482                                                       8. IS-95 Cal l Flow
               1                                                                    .


 9600bps인 경우


  心／冊七甘斗
     I / . I 2K. I '1N + 8 I 2K. I( N + 8   -.\ T40503 x (L0 H今 DECCORR)}mod 2比
     I I- I 11 I卜H1 -I-I 1e II H1           S I          "       .     '
     [\    [N+ 8]) 2       LN+8J      2       )                2'"



                          K표 8-10) Hash Function Modifier

  Apo:ocatopm                  N                     DEC아카극              Return 값
                   Ex扼nded 및 CEMA
                   Channel List Message
CI呱'I'\ 채널의 수
                   내어］ 포함되어 있는 채널
                   의 수
                   System Parameter
                   八4essage    내의   PAGEm
 호출 채널의 수                                    2XHASF尸KEY[0···1111           R+1
                   CHANs의 수
                   （이것은 7개까지 가능）

                   Extended System
                   Parameter
  Quick 호출         Message4         MCRR
                                             4XHASHJ(EY[0···111            R+1
   채널의 수           Parameter爪4essafe어］ 나
                   타난NU八'LQPCHs( 이 것
                   은 3개까지 가능）
 호출 읾ot의 수         2048                      6XHASI戶KEY[0···1111            R
                                            DECOR!?L Lt/MJ mod2'6
 호출 Indicator      앉刃0bps인 경우 376           1坦CORR1 나／64그 +1 mod2 '6
                                                                         Ri과 R2
     위치            4800bps인 경우 188
                                             여기서 t는 Frame의 시스템
                                             시간 임．
   For＼入／ard       八爪二RR Parameter
Common Control     Message어］ 나타난 NUM         2XHASH_KEY[0···11]            R- i
   채널의 수           FCCCHs(7개 까지 가능）
     8. IS-95 Call Flow                                           483
.


    叫I心多         전화번호가 0192192269에 대한 호출 Slot번호（PGSLOT）를 구하라·
                전화번호가 019-2四口269이므로 TMSI_O_S2p(019）와 IMSI_O_S1p
                는 각각 0x38C와 0x1B089E이다. 따라서 Hash Key는 다음과 같이
                구해진다．
                HASH나KI汀 = I｝江SI-U尸S2p + 224虹入4S1_O_S1p = 0x8C1B089E
                 여기에서 L, H, DECORR를 구하면
                 L : HASHJ(EY의 0에서 15번째 Bit = 0x089E
                 H : HASHJ(EY의 16어］서 31번째 Bit = 倣8C1B
                 DEC아｛R = 缸IIASH_KEY[0,1,        ,11] = 6x(小띠9E)=0x3B4 이다．
                 N : resource 개수（총 page Si毗 개수） = 2048
                 R : HASH 결과값 = PGSLOT
                 R = (N x ((40503 x (L ( H (DECORR) )mod216 )/216 (
                   = (2048 x ((40503 x (0x089E ( 0x8C1B ( 0x3B4)) mod
                          216)/216 (
                    = (20姻 x ((40503 x (0x8731)) mod 216)/216 (
                    = (2048 x ((0x1F698A93) mod 216)/216 (
                    = (2048 x (0x8A93) /216 (
                    = 0x9800
                 PGSLOT=R=0x1AA
                 Assigned Slot : ((t/4( -PGSLOT) mod(16xT)=0,
                 T=2SLOT끄DEX


       8.5.4 의사 랜덤 발생기

 IS中95규격에서 사용하는 의사린始 발생기는 모두 동일한 선형 발생기어］ 의하써
발생된다. 단말기와 기지국은 서로 같은 선형 필터들로 랜덤 발생기를 가지고 각각
    관리하고 있다. 이러한 의사，랜덤 발생기는 /\ccess 타이밍을 결정하는 값으로 사용
    되기어］ 각각이 가지고 있는 랜덤한 정보가 공유되어야 하기 때문이다. 다음은 현재
    정의되어 사용되고 있는 선형 발생기이다．
             Z, =axZ,,1modm                                         (8-13)
   484                                       8. IS-95 Call Flow
                                                                  U


 여기에서 a= 75=16807, rn=231-i=2147483647이며, z, 은 발생기의 출력이다. 여
기에서 사용되는 발생기는 앞서 3장에서 설명한 최장 코드의 일종으로 0과 m값이
없이 1부터 rn- i까지의 모든 수를 포함하는 전체 주기를 가지는 것이다．
 단말기가 초기화 상태에 있는 동안 단말기는 아래의 초기값을 사용한다．

         乙＝(ESN - S4）凡i入／DOM_ TJ兀IE )mod刃1                (8-14)

 여기에서 RANDOM什TI入'lB은 동기채널 메시지로부터 받아 저장한 SYSHTIJ\侄S
의 최하위Bit 32 Bit이다. 만일 이렇게 만들어진 초기값이 '0'이면 'i ' 로 대치된다. 단
말기는 연속 사용을 위해서 새로운 Zn을 계산해야 한다.
 2진분；= U (0< Un <1）이 필요한 경우에는 [/, = 乙／m값을 사용한다．
 작은 수 K,
       ,(0 드 K,, < 사1)이 필요한 경우에는 NX 乙／m값의 소수점을 제
외한 숫자를 사용한다.



 8.6 사용자 인증

  8.6.1 개요

 사용자 인증은 부정한 방법으로 서비스를 사용하는 불법 사용자로부터 원천적으
로 차단하는 방법이다. 앞서서 이야기되었듯이 /\ccess시어］ 사용되는 Long Code
Mask는 단말기의 고유한 전자일련（식별） 번호인 ESN으로 n追skii坦되어서 어느
정도의 보안을 유지할 수 있다. 그러나 동일한 ESN을 사용하는 전화기가 1대 이상
있다면, 즉 불법적인 전화기가 있다면, 보안이 유지될 수 없을 뿐 아니라 선의의 피
해자가 발생될 수 있다．
 이러한 이유로 또 다른 2차 보안장치가 인증 시스템인 것이다. 이것은 단말기만
가지고 있는, 즉 단말기만 일방적으로 가지고 있는 비밀정보（ESN）를 망과 공유하
는 또 다른 2차 비밀정보를 만들어서 호 시도시, 등록시, 착신시어］ 검증하도록 하는
방법이다．
 인증 관련 Parameter는 （표 &ii）과 같다．
    8. IS-95 Call Flow                                                       485
.

                         （표 8-11) Auth小Siqnature 입력 Param아er

            RANE CHA                                                     SAVE_REGIS
     절차                           ESN S        AUTH DATA      SSE AUTH
             LLENGE                                                         TERS

     등록        RAt皿无              ESN_ S力       IMSI Si        SSDA       FALSEE

             RAl江兀 및
    유일시도     IMSI_52의             ESN_ S力       IMSI_Si        SSD A      FALSEE
             최하위 8 Bit

     발신        RANDS              ESN_ S力         Digit        SSD A       TRUE


     착신        RANDs              ESN．中 S力      IMSI Si        SSD A       TRUE


    83 시도     RANDBS              ESN_ S力        flVISI_Si     SSD A      FALSEE




    Shared Secret Date(SSD : 공유 비밀 데이터）

    SSD는 단말기의 반영구적 메모리어］ 저장된 128 Bit 크기의 정보이다. 이러한
SSD는 다음의 （그림 斗23）과 같이 두 부분으로 나뉘어지는 더］ 각 부 분은 다른 처
리를 위해서 사용된다．

                              i
                                   ssI兀A(64)    三 SSDmB(64)

                                   （그림 &23) SSD의 구성


    여기에서 SSDA의 64 Bit는 인증절차어］ 사용되며, SSD_B의 64 Bit는 음성 보
안 및 메시지 암호화어］ 사용된다．


    Random Challenge Memory(RAND)

    기지국이 단말기로 호출채널을 통해서 전송한 최근의 /\ccess Parameter
Message중 32 Bit의 RAn）를 단말기는 보유하게 퇸다．


    Call History Parameter(COUNTs-p)

    단말기가 보유하는 八4odu1o 64 카운터로서 Parameter 갱신명령이 Forward 통화
I    486
                                                                    8. IS-95 Cal l 디0小／
                                                                                          1



채널을 통해서 수신되었을 때 단말기어］ 의해서 갱신된다．

     8.6.2 공유 비밀 데이터（SSD）의 갱신

    SSD는 SSD발생절차를 사용하여 갱신되며, 단말기 고유정보, 랜덤 데이터 및 단
말기가 미리 저장하고 있는 斗Key를 이용하여 초기화된다. 사용자가 인증 서비스
를 받는다는 것은 이러한 /v-Key를 할당받는다는 것을 의미하며, 이러한 /v-key는
단말기의 UI를 통해서 입력되는 것이 일반적이다. 또 다른 방법으로 입력되는 경우
는 OTA(Over The Air act如毗ion）를 통한 방법이다．


                   F1ANDSSD            ESNS

                 RANDSSD(56)        ESN_S(32)           A-Key(64)


                                          !
                                  SSD Generation
                                    Procedure

                                          !
                          SSD_ 뇨NEW(64)       SSD_B_NEW(64)


                              （그림 &24) SSD겨싼


    A-key는 64 Bit로 단말기어］ 지정되는 데이터로서 단말기의 영구보안 및 식별 머］
모리어］ 저장된다. A-Key는 단지 단말기와 시스템의 HLR, 그리고 인증센터（如C)
에서만 알 수 있고 관리된다. SSD갱신 절차는 다음과 갇다．


           RAND CHALLENG       ESN S           AUTH DATA        SSD AUTH

             RANDBS(32)       ESN_S(32)        IMSI_S1(24)    SSD_ A_NEW(64)



                                   Auth_SignaLure
                                     Procedure




                           （그림 &25) AUTHBS계산


    기지국은 호출채널이나 Forw可d 통화채널을 통해서 SSD갱신을 지시하며, 이것
은 SSD update 入'ISG를 통하써 이루어진다. 이 메시지에는 HLR/Au(二에서 SSD를
    8. IS-95 Call Flow                                                                          487
.

계산할 때 사용한 RANDSSD를 포함하고 있다．
    단말기가 SSD update 八/ISG를 수신하면 SSD 발생절차의 입력 Parameter값을
설정하고 SSD 발생절차를 수행하며, SSD寸／k_NEW와 SSD1B1NEW값을 설정한다．
    단말기는 하나의 32 Bit 난수 RAl나DBS를 선택하여 Access 채널 혹은 Reverse
통화채널로 Base Station Challenge Order어］ 실어 기지국어］ 전송한다．
    단말기와 기지국은 인증 절차의 입력 Parameter를 설정하고 인증 절차를 수행하
여 18 Bit의 AUTHBS를 설정한다. 단말기와 기지국은 SAVE_SI(코나ATUI扼의 입
력을 FALSE로 설정한다．
    기지국은 인증 절차의 결과인 18 Bit의 AUTHBS를 호출채널이나 Forw可（ii 통
화채널을 통해서 Base Station Challenge Confirmation Order어］ 실어서 단말기
어］ 보낸다．
    기지국 시도확인 명령을 수신한 단말기는 수신한 AUTHBS와 자신이 계산한
AUTHBS를 비교한다．

       Mobile Station                                                          Base Station

                         띠            SSD update order
                                         (RANDSSD)


      RANDSSD          A-Key                                     RANDSSD                A-Key



                                                                SSD Generation Pro



     SSDBNEW
           SSD A NEW
                                                               SSD_
                                    Base Station Challenge Order
                                                                      B_
                                                                           +   NEW   1
                                                                                 닥SD A NFW

                                             (RANDBS)




             AIJTHBS

                +
       AUT표BS = AUTHBS?        4   Base Station Challenge Order Confirmation
                                                   (AUTHBS)


                               SSD Update confirmation order (Success)
                               SSD Update Rejection order (failure)

                          （그림 &26) SSD U口date Message Flow
   488                                                        8. IS-95 Call Flow
                                                                                   .


 비교 결과 같으면 단말기는 SSD갱신절차를 수행하여 SSD_A, SSD_B를 각각
SSDANE＼사, ssI工BNE\\／로 설정하여 ssI) 갱신이 성공적으로 이루어졌음을
나타내는 SSD Update Confirmation Order를 기지국어］ 보낸다．
 비교 결과 틀리면 단말기는 SSD1A1NEW, SSDmB1NEW를 버리고 기지국으로
ssI) 갱신이 실패했음을 나타내는 성공적으로 이루어졌음을 나타내는 SSD Update
Reject Order를 기지국어］ 보낸다．
 SSD Update Confirmation 아der를 수신하면 기지국은 HLR/AuC로 부터 수신
한 값으로 SSD_A, SSI工B를 설정한다．


   8.6.3 단말기 등록인증

 인증절차는 Access Parameter Message의 AUTH 필드가 '01'로 설정되었을 때 수
행퇸다. 단말기는 /\ccess 채널로 Registration Message를 보내서 등 룩 을 시도한다．
 단말기는 다음의 （그림 斗27）과 같이 인증서명 절차의 입력 Parameter를 설정하
고 SAVE_REGISTERS를 FALSE로 설정한다．

         RAND CHALLENG    ESN S           AUTH DAT       SSD AUTH
           RANDBS(32)    ESN_ S(32)       IMSI S1(2引   SSD_ A_NEW(64)

                                      +
                              Auth,.Signature
                                Procedure




            （그림 8-27) 단말기 등록 인증을 위한 AUTHR계산


 단말기는 Registration Message의 AUTHI｛어］ 인증서명 절차의 결과값 AUTH小
SIC八ATTiRE로 설정하고 단말기어］ 저장되어 있는 RAI皿）C任｛An）의八4SB 8 Bit)
과 COUNT값을 Registration Message어］ 실어서 기지국으로 전송된다．
 기지국에서는 수신된 AUTHR값을 기지국에서 계산한 값과 비교하고 RAN]兀，
COU卜口는 내부어］ 저장퇸 값과 비교한다．
 비교값과 결과가 틀리면 기지국은 등록시도가 성공하지 못한 것으로 판단하고
Unique Challenge Response Procedure를 시작하거나 또는 SSD갱신절차를 수행
한다．
    8. IS-95 Call Flow                                                         489
1

     8.6.4 유일시도 응답（Unique Challenge Response I거rocedure)

    유일 시도 응답절차는 기지국에서 시작되며 호출채널 및 /\ccess 채널과
F야ward 통화채널 또는 Reverse 통화채널을 통해서 수행퇸다．
    기지국은 24 Bit의 RANDU를 발생시켜 Forward 통화채널이나 호출채널의
Authentication Challenge 入4essage어］ 실어서 단말기로 보낸다. Authentication
Challenge Message를 수신한 단말기는 （그림 斗28）과 같이 인증 서명 절차의 입
력 Parameter를 섣정하고 SAVE REGISTERS의 입력을 FALSE로 한다．


                RAND CHALLENG        ESN S      AUTH DATA       SSD AUTH

             RANDBS[ 24) IMS1_S2(8) ESN_S(32)   IMS! S1(24)   SSD_ A_NEW(64)



                                       Au t hS4三Bat끄re
              F\!Sf S2 이 LSB              Procedure
                 니 111 I: 01




                                         AUTHR( 1別

                        （그림 &28) 유일시도 응답을 위한 AUTHU겨싼


    단말기는 인증서명 절차를 수행하여 그 결과값 AUTHSIGNATURE을 A끄then
tication Challenge Response 八/lessage의 AUTHEJ 필드에 채워서 기지국으로 전
송된다．
    기지국에서는 자체적으로 계산한 값과 단말기에서 수신한 AUTHEJ값을 비교한다．
    비교값과 결과가 틀리면 기지국은 단말기로부터 더 이상 접속시도를 금지시키고
진행중인 호를 종료하거나 SSD 갱신절차를 시작한다．


     8.6.5 단말기 발호인증

    호출채널로 전송된 /\ccess Parameter Message의 AUTH 필드가 '01'이고 단말
기가 발호를 시도하면 이 인증절차가 수행퇸다．
    단말기는 （그림 斗29）와 같이 인증서명 절차의 입력 Parameter를 설정하고
SAVE_ REGISTER를 TRUE로 설정한다. 입력 Parameter 중 AUTILDATA에
는 발호 메시지의 CHARi의 필드어］ 포함퇸 최종 61玉git가 들어간다. 발호 메시지
내에 Digit 수가 6보다 적으면 나머지는 IMSI_Si의 최상위 Bit가 대신 들어간다．
      490                                                             8. lS-95 Call Flow
                                                                                           U


     단말기는 인증서명 절차를 수행하고 그 결과 AUTHSIGNATURE를 발호 메시
지의 AUTHR 필드어］ 채우고 RANDC와 COUNT 값은 단말기에 저장된 현재 값
으로 하여 기지국어］ 보낸다．

            RAND CHALLENG    ESN S          AUTH DATA         SSD AUTH

              RANDBS(32)    ESN_S(32)       DIGITS(24)        SSD_A(64)

                                        +
                                                         \1




                                Auth小Si；三nature
                                   Procedure

                                        1
                                  AUTHR(18)

                  （그림 &29) 단말기 발호인증을 위한 AUT니다． 계산



     기지국에서는 수신된 AUTHR값을 기지국에서 계산한 값과 비교하고 수신된
RANDC, COUNT는 내부어］ 저장된 값과 비교한다．
     비교 결과가 맞으면 기지국은 적절한 채널지정 절차를 개시하여 채널을 저장한
다음 기지국은 Forward 통화채널로 Par계Tleter 1珀date Order을 단말기로 보내 단
말기 내의 COUNTs-p값을 갱신한다．
     비교 결과가 틀리면 기지국은 서비스 제공을 거부하고 Unique Challenge
Response Procedure를 시작하거나 또는 SSI) 갱신절차를 수행한다．


      8.6.6 단말기 착 호 인증

     호출채널로 전송된 /\ccess Parameter Message의 AUTH 필드가 '01'이고
Access 채널에 실어보낸 호출응답 메시지어］ 단말기가 응답하면 이 인증절차가 수행퇸
다．
     단말기는 （그림 斗30）과 같이 인증서명 절차의 입력 Parameter를 설정하고
TRUE로 설정한다．
     단말기는 인증서명 절차를 수행하고 그 결과 AUTH小SIGNATURE를 Page
Response 入/Iessage의 AUTHI{ 필드어］ 채우고 RANDC와 COUNT 값은 단말기어］
저장된 현재 값으로 하여 기지국에 보낸다．
     기지국에서는 수신퇸 AUTHR값을 기지국에서 계산한 값과 비교하고 수신된
RANDC, COUNT는 내부어］ 저장된 값과 비교한다．
     8. IS-95 Call Flow                                               491
.


               RAND CHALLENG     ESN S       AUTFI DATA   SSD AUTH

                  RAND BS(32)   ESN_S(321   IMSI_S1(24)   SSD_A(64)



                                    Auth_Signature
                                      Proeedure



                                      AUTHR( 18)

                   （그림 &30) 단말기 착 호 인증을 위한 AUTHF{ 계산


    비교 결과가 맞으면 기지국은 적절한 채널지정 절차를 개시하여 채널을 저장한
다음 기지국은 Forw町d 통화채널로 Parameter Update Order을 단말기로 보내 단
말기 내의 COUNTs-p값을 갱신한다．
    비교 결과가 틀리면 기지국은 서비스 제공을 거부하고 Unique Challenge
Response Procedure를 시작하거나 또는 SSD 갱신절차를 수행한다．

      8.6.7 CAVE Algorithm

    앞에서 공부한 인증처리과정중에서 Auth_S坦niture Procedu丁e어］ 대한 공부를
이절에서 공부한다. 이것은 CAVE Algorithm이라는 절차를 통해서 그것의 Authen小
tication값을 얻게되는데 이 Algorithm은 널리 알려져 있다．
    CAVE Algorithm은 20byte의 입력을 가지며 CAVE Table이라고 하는 256byte
의 Table을 이용하여 난수를 발생한다. CAVE Algorithm을 통해서 생성되는
A毗hentication값은 총 24 Bit이며, 어떠한 Operation을 하느냐에 따라서 24 Bit를
사용하기도하고 18 Bit를 사용하기도 한다. 현재 여기에서 사용하고있는 것은 18
Bit이다.
    膊難難瓠

    REG(Register)2] bit Setting
    CAVE Algorithm의 입력 Parameter는 4byte의 LFSR과 l6byte의 REG（레지스
터）가 사용된다. 4byte의 LFSR중에서 상위ibyte가 Cave algorithm에 사용되며
LFSR은 별도의 Algorithm을 갖고 수행하는 LFSR cycle어］ 의해서 32 Bit를 결정한
1斗．
    LFSR의 최상위 8 Bit와 임의의 연속되는 REG 2byte(16 Bit）중 첫 번째 8 Bit와
Excius如eOR를 수행한다. LI구SR과 REG의 Excius如eOR를 통하囚 8 Bit의 결과
                                                          8. IS-95 Call Flow
                                                                               1


값 offset_i이 얻어진다. Offset_i이 나타내는 값만큼 offset된 cave table값을 읽어
들인다. cave table은 총254byte의 Data를 lb姓e 단위로 나누어 각각 丁255까지
                                        （刃이었다면 100에 해
可fset번흐를 부여한 Table을 말한다 만일 offset_i의 값이 1
당하는 cave table의 lbyte를 읽어들여 다음절차어］ 사용하게퇸다．
 Cave table로 부터 출력되는 8 Bit중 하위4 Bit와 offset 1을 생성하는데 사용되
었던 REG lbyte의 하위 4 Bit가 같은 지를 비교한다. 만일 같으면 LFSR cycle을
다시 반복하여 CAVE A坦orithm을 처음부터 다시 수행하며 LFSR cycle은 반복퇸
다. 이러한 반복은 Cave table로부터 출력되는 8 Bit중 하위4 Bit와 off s毗그을 생
성하는데 사용되었던 REG lbyte의 하위 4 Bit가 다를 때 까지 이루어진다．
 결국 다른값이 되면 그때 Cave table로 부터 출력되는 하위 4 Bit와 상위4 Bit 그
리고 임의로 연속되는 REG2byte중 두 번째 byte의 하위 4 Bit와 Exclusive OR를
수행한다. Exclusive OR의 출력 4 Bit는 Cave algorithm에 사용된 임의의 REG2
개의 byte중 첫 번째 byte의 하위 4 Bit어］ 채워진다. 이후 LFSR은 종료된다．


   L 100 :      LFSR                                              Reg(0시15)

                                             L HL H


    8b1t

                                                            L: Low bit
                                                            H : High bit
                       8b1t

                                    4bit
                                                                 EXIT

                                                                   十
                                                              LFSR_ Cyclej
  Offset 1


                                           Yes
                H                                         ＜二帥oL가＞
                                                                   A


                                                      1
             Cave table(256)                                  LFSR Cycle

                               （그림 &31) 하위 t기t Setting
          8. IS-95 Call Flow
      1                                                                                  493


          이과정을 모든 REG에 포함된 byte에 대하여 수행하며 마지막 16번째 byte어］ 대
한 Cave algorithm을 수행하여 LFSR cycle이 종료되었을 때 다음 단계를 수행한
 다．
          이것과 마찬가지로 상위bit를 가지고 REG의 값을 결정하는 방법도 있는톄 이것
은 하위bit setting과 마찬가지로 수행되지만 선택되는 bit를 상위의 4 Bit를 가지고
한다는 것이 차이가 있을 뿐이다. （그림 &31）과 （그림 &32）는 이러한 방법들을 설
명하고 있다．


           L 200 :       LFSR                                                  Reg(0-45)


           IlI"I I I                               L HL H


           8bit

                                                                     L : Low bit
                                                                     H : High bit
                                8bit

                                            4bit        4bit

                                                            +
                                                                           EXIT



          Offset 2                                      x아            LFSR Cycle




                      LH
                                               Yes


                                                        4bit
                                                            t    C
                                                                      GO
                                                                           t
                                                                               o   L_
                                                                                   A
                                                                                        200   >
                     Cave table(256)                                  LFSR_Cycle

                                       （그림 &32) 상위 bit Setting


      LFSR Cycle
      LFSR은 총 32byte로 수성되며, 그중 최상위 8 Bit가 Cave Algoi就hm어］ 사용된
다. LFSR Cycle은 1BitOi比ration에의해서 수행되는데 절차는 다음과같다．
      총32 Bit의 LFSR을 그림 斗33어］ 나타내었는데 LFSR cycle이 수행될때마다 각
bit들은 오른쪽으로 한 bit씩 Shift퇸다. 마지막 3bit와 10번째 bit와 Exclusive OR
I    494                                                          8. IS-95 Call Flow
                                                                                       1


를 수행하여 그 결과 값을 임시（Te聊）영역어］ 저장한다. 저장된 값은 LFSR cycle
이 반복 수행될 때 첫째 bit어］ 채워진다．


                                                                 1 bit




                                 （그림 8-33) LFS日 Cycle


    Au냔i CAVE

    인증어］ 사용되는 AURTH값은 Aut노Signature Procedure를 거친 18 Bit의 값
이다. 앞에서 다루었던 Cave Algori恤Ti은 LFSR Cycle과 Cave Table을 사용하여
REG의 16개 byte를 결정하는 것이다．
    여기에서는 LFSR Cycle과 Cave table을 통하여 결정된 REG에서 얻어지는
AUTH값 결정 절차를 다룬다 LFSR Cycle이 모든 REG에서 얻어지는 AUTH값


              R(O)      R(1)   R(2)                      R(13) R(14) R(15)




                8 bit                      8 bit                         8 bit
                                                   .. 하위 8 bit

           AUTH_CAVE
              24 bit


                               （그림 &34) AUTH_CAVE 생성
    8. IS-95 Call Flow                                    495
.


결정 절차를 다룬다. LFSR Cycle이 모든 REG에 대하여 EXIT되었을 때의 REG
값이 그림에 나타나 있다. REG의 16개 byte들 중에서 상위 3개의 byte와 하위 3개
byte가 각각 Exclusive OR를 거쳐 24 Bit의 A끄thHCAVE값을 채우게 된다．
    첫 번째 byte인 R(13）이 Exclusive OR을 수행하고 R(1）과 R(14), R(2）와 R(15)
가 각각 Ex如前veOR를 수행한다. 위의 과정을 통해서 얻어진 24 Bit의 /\uthH
CAVE값중 하위 18 Bit가 AUTH(AUTI표｛, AUTHBS, AUTHU）로 사용된다．



    8.7   확인절차                                                  )
    기지국과 단말기는 서로 메시지를 송수신함에 있어서 상대방이 정확하게 메시지
를 수신했음을 확인하기 위하여 확인절차를 별도로 사용한다. 이는 기지국과 단말
기간의 원활한 통신을 위한 것으로 L2와 L3의 확인으로 각각 분리될 수 도 있다．
    예를 들면 이 절에서 공부하게 될 공통필드를 사용하여 메시지를 확인하는 절차
는 L2 확인절차이며, 메시지의 내용 자체어］ 대한 확인 절차는 L3의 확인이라고 생
각할 수 있다．
    메시지확인을 위해서 사용되는 공통 필드들은 ACKTYPE, ACKSEQ, 八'ISG
SEQ, ACKREQ, VALIIJACI( 필드 등이 있다. 또한 이러한 확인절차는 대기상
태와 통화상태에서 이루어지나 그것의 진행 사항들이 약간 다르게 관리되고 진행된
다. 즉 공통필드의사용상에서도 통화 채널 상태에서는 이미 Frame에 태한 정보가
구체화되었으므로 ACKTYPE와 VALII工ACK 필드는 사용하지 않는다. 또한 머］
시지의 처리시간과 중복 메시지의 판별기준을 위한 timer도 다르게 관리된다．

     8.7.1 대기상태의 메시지 확인

    대기상태의 확인절차는 메시지의 공통 필드인 ACK_TYPE（확인 주소 형태）,
ACK_SEQ（확인 일련 번호）, 入[SG_SEQ（메시지 일련 번호）,ACK나REQ（확인 요
구 지시자）, VALII工ACK(유효 응답 지시자） 필드를 사용한다. 이러한 호출 채널
메시지의 확인작업은 /\ccess 채널로 이루어진다．
    ACKTYI下은 응답을 요구하는 메시지의 ad士ess type을 나타내며, 八/ISG
SEQ는 기지국 또는 단말기에서 메사지를 송신할 때 연속적으로 증가 시켜서 전송
      496                                       8. IS-95 Call Flow
                                                                     1


한다. ACK_SEQ는 수신한 메시지의 八'ISG_SEQ를 사용하며, ACK_REQ는 확인
을 요구할 때 사용하며 VALIDACK는 ACK1REQ에 대한 응답의 경우어］ 사용한
다. 즉 VAT끄工ACK는 응답을 포함하고 있다는 것을 나타낸다．
     따라서 지금 전송하고자 하는 메시지가 확인 요구가 있는 메시지어］ 태한 응답의
목적으로 전송할 때는 VALIII工ACK를 "1“로 설정하고 전송한다
                                     ． 그리고 ACK
TYPE과 ACK_SEQ 필드를 각각 호출 채널을 통해서 확인이 요구된 메시지의
ADDR니TYPE과 MSG_SEQ필드와 동일하게 설정하여 전송하게 될 이 메시지가
조금 전어］ 수신한 확인이 필요한 메시지에 대한 확인이라는 것을 명시한다．
     확인이 필요하지 않는 메시지를 송신할 때는 VALil工ACK를 "0" 로 설정하고,
ACKTYPE과 ACK나SEQ필드를 각각 호출 채널을 통해서 확인이 요구퇸 메시지
의 /\.DDRTYPE과 入'ISG_SEQ필드와 동일하게 설정한다. 이 같은 메시지가 없다
면, 시）DRTYPE을 "000'’로 ACK日TYPE을 "111”로 섣정한다．
     예를 들어서 호출 채널로 전송되는 임의의 메시지가 VAT끄工ACK=1이고 八4SGH
SEQ=2일 경우어］ 이 메시지어］ 대한 확인 메시지는 /\ccess 채널로 전송되는
ADDR TYPE이 동일하며 ACQSEQ=2인 메시지가 확인을 해주는 메시지가 된
다．
     단말기는 메시지（레코드）가 동일호출 채널로 수신되었고, 八4SG小SEQ, ACK
REQ필드에 동일한 값을 지니고, 단말기가 호출 채녈을 통하여 수신한 두개의 메시
지가 갇은 일련번호의 메시지를 나르는 갇은 신호라고 여겨질 수 있는 최소 기간인
2.2(T4m초 내에 수신되었고, 주소가 같을 I대 중복 메시지로 처리한다. 즉 망은
Si毗Index가 1인 Si毗 Mode 1인 경우를 최소로 하여 메시지를 전송한다는 이야기


                                           이 시간 간격 안에 동일한 호출
                        MSG_SEQ=k,         채널로 전송되는 MSG_ SEQ=k,
                        ACKREQ= a인         AC K_REQ= a인 메시지는 중복 메
                        메시지의 전송            시지로 판단한다．




                    7
                                     T4m                卜仄＼
                                                              T4m끝
            T4m시작

                （그림 &35) 반복 메시지 검출을 위한 시간 간격
    8. IS-95 Call Flow                                    497
口


가 된다. 앞의 （표 斗1) Si毗 Cycle Index어］ 따른 검색주기에서 알 수 있듯이 Si毗
八4ode 1인 경우 2.弱초이다．
 단말기는 호출 채널이 다른 기지국에서 전송되었거나, 다른 （노de Channel상 혹
은 다른 CDMA 채널상으로 전송될 때 호출 채널은 다른 것으로 간주한다．
 이러한 확인절차는 제어신호에만 적용되며 데이터 신호 전송에는 적용하지 않는
다. Signaling은 시스템과 기지국의 신뢰성 있는 신호 송수신이 되어야 하며, 음성
은 전송에 지연이 발생되지 않도록 FEC(Forw町d Error Correction）로 처리한다.
이러한 FEC방식은 앞의 7장에서 설명되었다．
 여기서 설명하고 있는 IS-95혹은 IS-2000 CAl Pr毗ocol은 OSI 7 layer의 layer
3까지를 규정하고있으며, 이 절에서 설명하고자 하는 확인절차는 Layer2에서 이루
어진다. Layer 2는 MAC/LAC layer로 에러정정 및 확인절차를 수행하는 계층이
다. 따라서 IS-95의 호 처리를 위해서 이루어지는 제어신호의 확인절차는 layer 2
에서 주로 이루어진다. 여기에서 이루어지는 확인절차도 L2 ack이다.
 （그림 斗36）어］ 나타났듯이 메시지의 확인은 우리가 전달하려고 하는 데이터를 포
장하는 과정, 즉 봉투어］ 표시된다. 원래 1ayer2의 역할이 이러한 확인절차를 나타내
는 것이다. 물론 메시지의 내용인 편지지에도 iayer3의 확인이 있다. 이 그림에서는
" 길동에게"라는 인사말이 될 것이다.



                                      i     지봉투의 받는 사람

                                      ! 咐甲빤쁘H
    킬동에게                                                 우표
    어쩌고 저쩌               서울시 금천구 독산동 145小 홍길동
    기타둥둥．..


                                      보내는 사람
                                      경기도 광명시 하안동 702번지 이도령

                         편지의 내용 : 'ayer 3
                         의 메시지 내용

                              （그림 &36) 메시지의 확인
   498                                      8. IS尸95 Call Flo니／
                                                                  .


 앞서 이야기퇸 ACK나SEQ, 入4SGSEQ, ACKJEQ, VAL표）1ACI豆 ACK小
TYPE필드들이 위의 그림의 편지봉투의 역할을 하는 필드들이다. 또한 layer 3의
확인은 메시지마다 어떠한 내용을 담고있느냐어］ 따라서 또한 이러한 L3 ack가 다
르게 나타날 것이다．
 즉 응답을 필요로 하는 메시지의 경우 각각의 필드들은 다음과 같이 정리된다．
 水 VALil工ACK=1
 木 ACK.eSEQ = ack를 필요로 하는 수신 메시지의 八4SG_SEQ
 水 ACK나TYPE= ack를 필요로 하는 수신 메시지의 ADDR TYT下
 또한 ACK가 필요 없는 메시지 수신 시 단말기는 다음과 같이 내부 Parameter를
설정한다．
 水 VALil工ACK = 0
 水 ACK나SEQ = 최근어］ 수신한 入41N을 가지고있는 메시지의 八4SG_SEQ로 하고
   그러한 메시지를 수신하지 못했을 때에는 111로 설정한다．
 水 ACK나TYPE= 000
 일반적으로 별도의 /\cknowledgement Procedui氾어］ 관련된 메시지를 사용하는
방법보다는 다음 메시지 처리 때, 즉 L3 Ack는 L2 Ack를 동반해서 대부분 사용하
고 있다. 그러나 단말기에서 응답할 메시지는 있고 다음 메시지가 없을 경우는
Mobile Station Order 八4essage를 이용하여 응답한다. 반대로 기지국에서 응답할
메시지가 있을 경우 Base Station Acknowledgement Order를 이용한다．
 수신측은 자신에게 지정된 메시지 수신 후 그어］ 해당한 응답메시지를 송신할 경
우 해당 메시지어］ A아（를 보내고 특별한 응답 메시지를 송신할 필요가 없는 경우
（단순히 메시지를 정상적으로 수신했다는 응답만 필요할 경우）에는 탄말기의 경우
八(IS Acknowledgement Order를 통하1 （기지국의 경우 BS Acknowledgement
Order)Ack를 송신한다．
 Ack_Req가 없은 GPM를 수신할 때는 PRM로 Ack를 한다．
 단말기가 /\ccess 채널을 통해서 메시지를 송신할 경우 기지국은 ACC TMOx
80ms내에 ack 메시지를 내려 주어야 하고 단말기는 TA=80X (2+ ACChTMO）이
내어］ Ack를 받지 못하면 재전송한다．
    8. IS-95 Call Flow                                           499
U


     8.7.2 통화상태

 통화상태에서도 확인절차가 필요하다. Forw可d과 Reverse 통화 채널에서 확인
을 요구하는 메시지어］ 대한 절차는 확인이 수신되지 않은 경우에만 메시지를 재 전
송하는 선택적 반복 기법이다. 통화 채널 메시지에서는 대기상태와는 달리 ACK
TYPE, VALII工ACK필드는 제외되며, ACK_REQ필드가 1로 설정되어 있을 때
확인윽 픽요로 한다．


 메시지 송신과 확인 수신
 계층2 프로토콜은 임의의 순서로 메시지를 전달하는 것을 보장하지 않는다. 단말
기가 기지국이 규정된 순서로 일련의 메시지를 수신하는 것이 필요하다면 단말기는
그 상태에서 다음 상태를 송신하기 전 각 메시지어］ 대한 확인을 기다려야 한다. 상
대적인 순서가 중요하지 않은 확인 요구 메시지에 대해 단말기는 첫 번째 메시지어］
대한 확인을 수신하기 전까지 송신할 수 있다．
 단말기는 확인恤SG_SEQ_ACK)요구 메시지어］ 태한 메시지 일련 번호를 저장한
다. 단말기는 Reverse 통화 채널 메시지 八띠ES卄SEQ 필드의 각 가능한 값에 대한
확인 상태 지시자（ACKWMTING[n], n은 O-7）를 저장한다. 단말기는 ACK
WAITING[(八'ISG_SEQ_ACK+4) mod 8］이 YES일 경우 확인을 요구하는 새로운


                                             단말기가 프레임처리롤 종
                                             료 . 확인이 수신되지않았다
                                             면, 메시지 재 전송을 위한
                         기지국에 의한 확인전송        처리작업을 시작한다．
                         확인 내용을 포함할 수
                         있는 마지막 프레임

    For砥咆rd 통
      화 채널


                             卜          'I뇨의 유효길이


                         =
    역방향 통화
                                         i
      채널

          단말기에 의한                메시지 전송의 끝이       T,, 타이머   :1
          메시지 전송                 면서 口Cm타이머의       의 만료시
                                 시작 시 점           (]




            （그림 &37) 日everse 통화 채널 메시지의 확인에 대한 시간제한
   500                                                  8. lS-95 Call Flow
                                                                             1


메시지를 송신하지 않는다．
 단말기는 확인을 수신한 메시지를 재전송하지 않는다．
 단말기가 메시지 송신 후 0.4초（Tim초）내어］ 확인을 수신하지 않으면, 단말기는 그
메시지를 그림 斗37과 같이 재 송신한다. 단말기가 메시지를 재 송신하는 경우, 단
말기는 재송신을 위하1 동일한 八心G_SEQ를 사용한다. 단말기는 갇은 메시지송신
후 Tim초 이내에 메시지를 재 송신하지 않는다．
 단말기는 확인을 요구하는 각 전송된 메시지어］ 대하여 재송신 카운터（RETRY놔
COU]寸T）를 저장한다. 단말기는 메시지의 첫 송신어］ 앞서 RETRYCOUNT를 0으
로 설정한다. 가 메시지 송신 후 단말기는 확인을 수신하지 못하면 RETRY_
COUNT를 증가시킨다. RETRYCOUNT가 3회(Nim）가되면 단말기는 확인실패를
나타낸다.


 메시지 수신과 확인 응답
 Forw町d 통화 채널로 수신된 메시지는 Reverse 통화 채널로 송신된 메시지와
같은 방법에 의하1 증가퇸 八心G_SEQ필드를 지닌다. 분리 일련번호는，확인을 요구하
는 Forward 통화 채널 메시지와 확인을 요구하지 않는 메시지를 위하여 유지된다．
 단말기는 수신된 메시지의 八4SG_SEQ 필드와 같이 설정된 ACKSEQ필드를 가
진 메시지를 송신함으로 수신된 메시지를 확인한다. 이런 방법으로 설정된 ACK日
SEQ필드를 가지고 송신퇸 메시지는 수신된 메시지의 확인을 포함함으로써 조회할


         기지국에1 의한                메시지전송의 끝이면서       ri, i而自희
         메시지 전송                  T2m타이머를 설정한다．       만료시점
     i              《




  For＼入yard 통
    화 채널

                                         T2m의 유효길이
  역방향 통화
    채널

                        단말기에 의한 확인 전송
                        확인 내용을 포함할 수 있   ！기지국이 프레임 처리를 舌       V
                        는 마지막 프레임        「 ii- 확인이 수신되지 않았다
                                           ',브， 메시지 재 전송을 위한
                                           처리작업을 시작한다.


           （그림 8-38) Forward 통화 채널 메시지의 확인에 대한 시간저탄
    8. lS-95 Call Flow
R                                                                        501


수 있다．
 확인요구 메시지를 수신할 때마다 단말기는 연속되는 Reverse 통화 채널 메시지
의 ACK뇨SEQ필드를 MSG_SEQ필드로 설정한다 메시지가 수신되지 않으면 단말
기는 이 필드를 '111'로 설정한다. 확인 요구 메시지를 수신한 후 단말기는 （그림
斗38）과 같이 T2m초 내에 확인을 포함하는 메시지를 송신한다．
 수신된 메시지가 확인을 요구하고 그 메시지가 수신퇸 후 T2m초 이내어］ 메시지가
이용되지 않는다면 단말기는 확인을 포함하는 단말기 확인명령을 송신한다. 단말기
확인명령은 확인을 요구하지 않는 메시지로서 송신되어진다．
 중복 메시지의 검출을 위해서 단말기는 Forw可d 통화 채널 메시지 八4SG_SEQ
필드（MSG_SEQRCVD［川, n은 小7）의 각 가능한 값어］ 대한 수신 상태 지시자를
저장한다．


          요구하지 않는 메시지
 ACKJEQ가 '0'으로 설정되어 있는 경우 통화 채널 메시지는 확인을 요구하지
않는다. 단말기는 확인을 요구하지 않는 메시지（ACK나SEQ_NOACK) 어］ 대해서 송
신되어질 다음의 메시지연속번호를 저장한다. 확인을 요구하지 않는 새로운 송신
메시지어］ 대하여 단말기는 메시지의 MSG_SEQ필드를 八4SG_SEQ_NOACK로 설
정하고 modulo 8로 MSG_SEQ_NOACK를 증가시킨다．
 （그림 斗38）는 이중으로 되어 같은 八心G叫SEQ번호를 가지고 확인을 요구하지 않
는 메시지를 T3m초 내어］ 수신한 경우를 고려한다. 단말기가 MSE_SEQ번호어］ 의해
결정된 것처럼 다중의 메시지 복제를 수신한다면 이중의 복제메시지는 폐기한다．


                                                   이 시간 간격 안에 동일한
                                                   호출    채널로     전송되는
                              MSG_SEQ=k,
                                                   MSG_SEQ=k, ACK_REQ=a
                              ACK_REQ=a 인
                                                   인 메시지는 중복 메시지로
                              메시지의 전송
                                                   판단한다．
    호출 채널

                    口
                                            'T3m
                         //
                                                                 卜＼
              T3m시작                                                   T3n,끝

 （그림 &39) 확인을 필요로 하지 않는 중복된 메시지를 검출하기 위한 시간 윈도우
                                                8. IS-95 Cal l Flow
   502                                                                U




  8.8 등록（Registr카向n)                                                  )
 등록은 단말기가 자신의 위치, 상태, Si毗 cycle 등의 개인정보를 기지국어］ 알림
으로써 기지국으로 하여금 효과적으로 단말기를 호출하도록 하기 위한 과정이다．
기지국은 단말기어］ 여러 가지 방법의 등 록 을 가능하게 할 수 있는데 이들 방법을
모두 사용하거나 일부만을 사용할 수 있다. 기지국이 각 등록방법을 모두 사용할 경
우 단말기의 정보를 항상 정확히 알 수는 있으나 지나치게 많은 메시지교환으로 시
스템부하를 가중시킬 수 있다．
 가지국은 시스템 Parameter 메시지를 통해서 단말기가 수행해야 할 등록의 종류
를 지정하고, 단말기는 해당등록조건이 맞을 경우 등록을 수행한다. 여러 등록 방법
중Power Up, Power Down, Timer Based, Distance Base, Zone Based 등록은
Roamir逗상태나 조컨어］ 따라서 기지국의 요구 없이 단말기 스스로 등록을 수행하
므로 Autonomous Registration이라고 한다．
 일반적으로 단말기의 등록은 대기상태에서 이루어지며, 초기상태에는 준비를 하
고 /\ccess 상태에서는 단말기가 송출한 등록, 발호, 호출응답 메시지에 대한 확인
을 수신하면 모든 등록 카운터를 초기화한다. 즉 모든 등록 관련퇸 값을 사용하지
않게 되고 등록의 필요성이 없어진다. 사실 등록의 의미는 개별적인 단말기의 존재
를 망에게 확인시켜주고 망과의 상호통신을 하기 위해서 이므로 /\ccess 상태나 통
화상태와 같이 망과 확실한 위치 정보 등으로 통신하는 가운데에는 이러한 별도의
등록절차는 의미가 없을 것이다．
 이렇듯 대기상태에서 이루어지는 등록은 다음과 갇은 종류가 있으며, 이것은 단
말기가 어디 있든지 망이 단말기의 위치파악이 될 수 있게끔 하기 위한 경우라고도
볼 수 있다．


      차단 둥록

 단말기가 사용자어］ 의해서 혹은 자연적으로 전원이 차단될 때 단말기는 망어］ 전
원이 차단되었음을 등록한다. 이것은 망의 입장에서 볼 때 단말기의 위치가 갑자기
사라져버리는 오류를 범하지 않게 하기 위해서 이다. 물론 전원 차단으로 인한 문
제, 즉 통화가 안 되는 것은 어쩔 수 없는 것이라고 할 수 있으나 망에서는 전원이
차단되어서 호출이 안 되는지 아니면 음영지역에 들어가서 인지가 분명해야 할 필
     8. IS-95 Call Flow
U


요가 있을 것이다．


 전원 공급 등록
 단말기에 새롭게 전원이 공급될 때 단말기는 새로운 위치등록을 해야 할 것이다．
이러한 경우 단말기의 공간적인 이동이 전원을 차단했을 때와 공급했을 때에 차이
가 없을 수도 있지만 엄청날 수도 있다. 즉 단말기에서는 그러한 사항을 알 수가 없
을 것이다. 때문어］ 망에서 알고있던 단말기의 최종위치정보와 단말기의 현재정보가
전혀 다른 곳일 수 있다. 때문어］ 망에서는 단말기를 호출할 수 없을 수도 있고 잘못
호출할 수도 있는 잘못을 범할 수도 있다. 때문에 이러한 등록절차는 반드시 필요하
다.




 Timer에 의한 둥록
 이것 역시 일정한 시간이 지난다면 단말기는 전혀 다른 지역으로 이동되어 있을
수 있다는 가정에서 이루어지는 등록절차로써 시간에 의해서 망이나 단말기의 상황
변화어］ 대한 갱신을 위한 등록절차 이다．
 단말기는 시스템 시간의 단위인 8（뇨IS단위로 카운터를 증가시키며 카운터의 값이
시스템 Parameter 메시지에서 명기된 등록주기를 초과하게 되면 등록을 수행하게
된다．
，寮饔裂無瓠

 거리에 의한 둥록
 단말기가 특정한 거리를 이동했을 때 이루어지는 것으로 거리이동, 즉 공간적인
변화로 인해서 시스템이나 단말기어］ 주어진 상황 변화에 대한 등록을 수행하는 과
정이다．
 단말기는 이전에 등록한 기지국의 위도, 경도 정보와 현재 기지국의 위도, 경도정
보를 피다고라스 정리에 의하써 거리를 계산한다 ．이렇게 측정된 거리는 시스템
Parameter에서 규정한 거리등록 기준보다 크다면 거리에 의한 위치등록을 수행한
다. 여기에서 거리는 단말기가 이동한 위치어］ 의한 정확한 거리가 아니라 단말기어］
게 서비스하고 있는 기지국간의 위치어］ 의하써 결정되어짐으로 단말기의 위, 경도
정보를 가지고 거리를 측정하는 것이 가장 정확하고 타당하다. 즉 단말기가 서비스
받고 있는 기지국이 어느정도 이상 거리가 떨어져있어서 망에서 단말기를 흐출하
                                         8. IS口95 Call 디ow
                                                             1


는데 필요한 정보를 갱신할 필요가 있을 수 있기 때문이다．


 Zone에 의한 등록

 하나의 등록 zone을 몇 개의 기지국으로 구성되고, 단말기가 새로운 지역으로 들
어갈 경우어］ 등록 을 수행한다. 그러나 단말기는 ZONE_LIST, Sil工｝皿)_LIST에
몇 개의 zone을 저장 관리하므로 저장되어있는, 즉 이전어］ 등록한 지역으로 들어칼
때는 수행하지않는다．
 이러한 ZON且끄ST는 7개（N帥）까지 가능하며 일한 숫자는 시스템 Parameter
의 TOTAL ZONE에 의해서 제한된다.


 Parameter 변경에 의한 등록

 기지국에서 수신한 시스템 Parameter 메시지에서 시스템 변경등록이 허용될 때
어］ 수행되며 단말기에서 관리하는 Si毗 cycle index정보와 단말기 등급 표시자
(SCM), 착신 호 enable 지시자（MOBHTERM）등의 정보가 변경되었을 때 망으로
보고하는 절차이다. 이 등록은 내부에서 REG_ENABLE과는 무관하게 등록이 수
행퇸다．


 명령에 의한 등록
 기지국으로부터 등록 요구를 받았을 경우어］ 수행되는 등록으로 기지국으로부터
전송되는 Registration Request Ord町어］ 의해서 이루어진다. 단말기는 이러한 명령
을 수신한 후 0.3초（T33m) 이내어］ 시스템 /\ccess 상태의 OVHD정보 갱신 부 상태
로 득어가서 등록을 위한 /\ccess를 준비해야 할 것이다．


 묵시적 등록
 단말기가 정상적으로 발호 메시지나 호출 응답 메시지를 전송하였고 이것으로 인
해서 망에서 단말기의 위치 정보 등을 갱신할 수 있는 기회가 주어진다면 이것은
등록이라는 이름보다는 호시도라고 볼 수 있으나 또 다른 형태의 등록이라고 볼 수
있으므로 이러한 것을 묵시적 등록이라고 한다．
    9. Vocoder                                        505
1




                                              Vocoder




    CDMA의 용량은 TI呱'IA, FDMA와는 달리 용량이 스펙트럼 효율 측면보다는
에러 성능 측면어］ 더욱 중요하게 의존하게 된다는 것어］ 대해서는 앞서서 이야기되
었다. CDMA 시스템의 효시라 할 수 있는 Qualcomm CI呱'IA 시스템을 고찰하1 보
면 Qualcoi列m의 시스템 엔지니어의 이러한 노력을 엿볼 수 있다．
    Qualc아nm CDMA의 CAI(Common Air Interface）를 정의한 IS-95의 경우 용
량 증대를 위해서 강력한 채널 코딩과 에러 성능이 뛰어난 변／복조 방식으로 대역
                              은 가변 데이터 율로 그 문제
을 희생시켰으며, 음성 부호화어］ 대해서 정의한 Is以；
의 해결책을 찾고 있다. 이 두 가지에서, 그것의 형태가 다르나 하나는 Eb/NO를 최
소화하는 것이며, 나머지 하나는 전체 대역의 전력감소를 통하1 용량 증대를 꾀하기
위함이다．
    Qualcomm CDMA에서 사용하는 Vocoder인 QCELI쁜 Cl呱'IA 시스템의 특성
어］ 부합되기 위해서 입력 뎨이터의 형태어］ 따라 변하는 가변 테이터 율로 전송된다.
이러한 QCELP은 선형 예측 필터어］ 여기（E斌ed) 신호로 특정한 벡티로 구성된
Codebook을 사용하는 CELP 구조를 기본으로 한다. 이것은 가변 데이터 율로 전송
   506                                            9. Vocoder
                                                               1


되므로 채널상에서 필요 없는 기본값들로 인한 간섭을 배제할 수 있어서 에러 성능
을 향상시키고, 전체적으로 시스템의 용량을 증대시킬 수 있다. 이것은 CDMA에서
는 시스템 용량이 단순한 주파수의 분할 측면이 아니라（결과는 같겠으나） power어］
기인퇸 것이라 할 수 있다．
 CDMA시스템에서 무선 인터페이스의 경우 Is-％에서 정의되었고 이러한 무선
인터페이스를 기반으로 전송되는 전송 데이터어］ 대한 내용은 별도의 기술 요구 사
항 등어］ 의해서 정의된다. 이러한 전송정보들은 크게 음성정보와 데이터 정보로 구
분할 수 있으며, 이것들은 전송되는 데이터의 특징어］ 따라서 약간의 차이를 가지면
서 정보의 구성방식, 전송방식 등과 같은 약속들이 정의된다．
 이 장과 다음 장에서는 이러한 （음성 및 비음성） 데이터들을 처리하는 방식 등어］
대해서 공부할 것이다. 특히 이 장에서는 음성정보 처리와 관련하여 새로운 형태의
Voice Sou丁ce （노小ng 방식인 V（乂oder의 A坦orithm을 분석하고 스펙트럼 효율과
관련될 수 있는 보다 저속의 \Tocod町에 대해서 공부한다．



      Voice Source Co비ng 방식                                        1
 음성의 디지털화 기술에는 파형 부호화, 음원 부호화 그리고 혼합방식이 있다．
PC八'I(Pulse Code 入'lodulation）이 파형 부호화의 대표적인 방식이며, Vocoder 방식
은 음원 부호화어］ 해당된다. Vocoder 방식은 음성의 파형을 분석하여 음성의 특징만
을 추출, 전송함으로써 파형 부호화어］ 비하여 전송 대역폭을 크게 감소시킬 수 있다．
 이러한 음성 부호화 시gorithm들은 다음과 같이 다시 정리될 수 있다．
 Waveform 부호화는 표본대 표본에 의하써 음성을 분석하고, 부흐화하고 재생한
다. 우리는 이러한 방법이 고품질의 음성을 생성할 수 있는 단순한 형태로 때때로 사
용하나 일반적으로 데이터의 속도를 16Kbps나 32Kbps 정도까지만 압축할 수 있다．
 Time-Domain Waveform Coder는 음성신호의 파형의 redundancy의 장점을
취할 수 있다. 유성음의 분절（segment）의 주기성과 인접한 음성 표본간의 상관성은
정보의 Bit율을 감소시키는데 사용된다．
 Frequency-Domain Waveform Coder는 주파수 영역에서 음성신호의 구조의
장점을 취한다. 음성의 포락선（Envelope）과 유성음 분절의 고조파 성분들은 정보의
Bit율을 감소시키는데 사용된다．
    9. Vocoder                                       507
1

    v (兀（xler는 \Ioice Cod町의 합성어로 사람의 발성기관들어］ 의해서 음성（소리）이
만들어지는 절차를 선형필터로 모델링하여 각각의 필터들의 Parameter를 생성하여
（즉 이 Parameter는 각각의 음성의 성격을 규정하는 Parameter들임）Parameter를
전송하는 방법이다        이러한 이유로 이러한 방법어］ 의해서 출력되는 데이터는
4Kbps 이하에서도 동작할 수 있다．
    이러한 Vocoder의 예로는 현재 힌국에서 서비스되고 있는 CI呱4A의 QCELP,
EVRC와 유럽의 GSM어］서 사용하고 있는 RPE-LTP 등이 그것들이다．
    Vocod町의 디지털 음성 부호화 Algorithm은 2가지 영역으로 구분할 수 있는데
그것은 부호화와 복호화이며 혹은 분석（／뇨ia1y前이과 합성（synthesis）이다. 디지털
음성 부호화 Algorithm은 표본화 과정을 거치면서 아날로그를 디지털로 변환하는
작업의 결과를 취하고, 음성의 필수적인 성분을 추출하여 양자화하여 전송채널로
전송하게 된다. 이러한 디지털 음성 복호화 Algorithm은 전송채널로 전송되는 bit
S甘earn을 수신하고, 부호화기에서 특징이 추출된 음성신호의 출력을 다시 만드는
과정이다．



                                  '1二十
                   Source Bit      수入］뒤 Bit



                                」《70;
        음성 입 력     ! Stream                   음성출력
                                                 p



                  （그림 9-1) 음성의 부호화와 복호화


    Vocoder의 압축기술은 음성을 합성할 수 있는 중요 Parameter를 분석을 통해서
추출하여 Parameter를 전송하는 방식이다. 즉 금고어］ 들어 있는 금괴를 주는 방법
은 금괴를 직접 줄 수도 있지만 그것의 열쇠를 주는 것도 한 가지 방법일 것이다．
이렇게 열쇠를 주는 방법은 상당히 간편한 방법이 될 수 있을 것이다. 이러한
Vocoder의 압축방식은 높은 상관성을 가지는 음성 정보원의 특성을 이용해서 수행
퇸다. 이것은 음성의 변화가 급격하지 않기 때문이며, 인접한 표본값에서 현재의 값
을 예측이 가능하다는 것이다. 이러한 특성은 음성의 Redundancy를 줄일 수 있는
다양한 압축의 방법들이 있을 수 있으나, 여기에서 공부하게 될 \Tocod町는 이러한
음성특성의 중요 Parameter들을 추출하여 압축의 효과를 내는 것이다．
    압축어］ 앞서서 음성이 짧은 시간（통상 10- 20ms) 동안 변화가 거의 없다는
Stationary한 상태라고 가정하며, 이러한 포락선의 정보는 10개 정도의（그 이상도
   508                                             9. Vocoder
                                                            1

가능） 계수로 표시가 가능하다. 또한 이러한 포락선 계수로 추출되지 못하는 좀더
고주파 성분의 추출은 음성의 피치（Pitch）어］ 나타나는 주기성을 찾아서 P可ameter
를 추출한다. 이러한 피치성분 추출 후에도 여전히 남아 있는 잔여 신호 성분들의
표현을 위해서 （力debo永으로 최종적으로 추출한다．



  9.2 발성의 원리                                                    \


 우리는 일반적으로 소리를 묘사할 때 파동인 소리를 생각한다. 이러한 가정에 의
해서 소리는 서1 가지의 주요 요소로 표현할 수 있다고 생각한다．
 첫 번째는 소리의 높낮이, 즉 고음과 저음의 구분이다. 소리의 높낮이는 1초 동안
몇 번의 진동을 하는가어］ 의해 결정되는데 진동수가 많으면 고음, 적으면 저음이다．
사람이 들을 수 있는 진동수의 범위는 1초어］ 20번에서 20,(X刃번 진동하는 파동들이다．
즉 사람의 가청 주파수는 20Hz - 2아cHZ어］ 이른다. 물론 사람마다 개인 차이는 있다.
 두 번째는 소리의 세기인데 소리의 세기는 단위면적당 공간을 지나가는 에너지의
크기와 관련해 비례한다. 이러한 소리의 세기는 소리를 표현할 때 진폭으로 표현된다．
 마지막으로 고려할 것은 소리의 질, 즉 음색인데 이러한 음색은 그 소리의 고조파
성분으로 기본 주파수의 진동수어］ 배가되어지는 소리들을 말한다. 이것은 기본 주
파수의 기본이 되는 진동을 좀더 색다르게 들리게 해 주어서 음의 색깔이라고 이야
기한다．




                          （甘＼
                         ．戶
               성［거 /,   「
                         「   ＼뇨폐로부E寸
                                       유입 되는 공71

                   （그림 아2) 사람의 발성 기관
    9. Vocoder                                         509
.


    우리가 말을 하는 것 혹은 노래하는 것 등과 같은 사람의 행동양식을 통상 발성（發
聲）이라고 이야기한다. 이러한 발성은 사람의 발성기관어］ 의해서 형성되게 된다. 이러
한 발성기관은 소리를 만들어낼 때 폐로부터 강하게 분출되는 공기에 의해서 자극되
며, 자극의 형태 및 자극의 종류어］ 의해서 소리는 유성음 혹은 무성음으로 구별된다．
    유성음은 폐로부티 강하게 바깥으로 유출되는 공기와 성대간의 복잡한 상호작용
어］ 의해서 만들어진다. 초기어］ 성대는 닫혀져 있다고 생각하자. 이때 폐로부터 밖으
로 분출되는 강한 공기어］ 의해서 공기압이 증가하여 성대가 열리고, 열려져 있는 성
대 사이로 공기가 강하게（혹은 빠르게） 흐를 때 Bernoulli 효과어］ 의해서 빠르게 움
직이는 공기 주변의 기압은 낮아지고 때문어］ 열려 있는 성대 근육을 닫히는 방향으
로 끌어당긴다. 성대가 닫혀 있을 때 폐로부터 분출되는 공기의 압력은 성대가 다시
열릴 때까지 증가된다. 이러한 동작은 스스로 반복되며, 이때 공기는 의사 주기 펄
스열을 생산한다.
    이러한 성대의 운동어］ 의해서 발생되는 펄스열의 기본 주파수는 음성의 pitch로
불려지며, 그것은 폐로부터 유출되는 공기 세기의 정도와 장력의 총합이 성대어］ 적
용되고 말하는 사람의 성대의 크기어］ 따라서 결정된다．
    무성음은 성도（vocal tract）의 임의의 지점에서 강하게 압축된 공기어］ 의해서 만
들어진다. 공기의 흐름은 성도어］ 의해서 여파되는 거친 잡음을 만드는 압축이다. 따
라서 성대의 진동이나 규칙적인 Pitch 성분은 없는 것이다．



                        공기의 빠른 흐름으로 주변
                        의 압력은 떨어지므로 바깥
                        에서 안으로 밀어서 성대를
                        닫으려고 함． PA> PB
                                              居기4 흐름

                                              員
                         (a) 성대 내／외부의 공기의 흐름과 압력




                 i으로 압력이 떨어 i
                  지는 十간．    i




                          (b) 성다1 내부의 압력그래프

                       （그림 아3) 공기의 흐름과 성대의 동작
                                                                        9. \/(:)（二（그der
   510                                                                                    .

 성도는 턱, 혀, 이, 그리고 연구개（목젖）의 형태어］ 의존하여 폭이 변할 때는 tube
로 모델링 된다. 일반적으로 성도의 길이는 17cm정도이므로 식 (9-1）어］ 의해서 기
하학적인 구조에 의존하는 자연 주파수（natural frequency), 즉 공진 주파수는 대략
500Hz이다. 이것의 제3고조파는 1印0Hz, 제5고조파는 25001七가 퇸다．

                                                                                    (9.1)
         t=       (2n+         V
                          1)
                                                         ..


                         4L
                                          0,
                                    ,n=        1,   2,
              =



 여기에서 V는 음속으로 일반적으로 상온에서는 약 340m/sec를 나타낸다. 그리고
L은 성도의 길이이다．

                                                              H
                          무성 음

                                                              >   LPC
                                   1 nh
                          유성 음                                H
                                          （그림 9-4) 소리의 합성／분석

 성도의 형태어］ 따라서 각각의 공진 주파수 혹은 Formant를 민들며, 다른 소리는 성도
가 유성음 흑은 무성음의 자극혀］ 의해서 자극되어질 때 만들어진다. 이상은 음성이
Vocoder에 의해서 합성되고 분석되는 것어］ 대한 기본적인 생각을 도식화해서 보여준다．
 일반적으로 사람의 소리는 （그림 9-4）와 같이 모형화된다. 즉 LPC는 정상적인
Frame 동안을 대표하는 주파수인 파형의 포락선을 결정지어 주고 세부적인 펄스열
의 지연과 이득 등을 Pitch필터로부터 얻어서 완전한 음을 만든다. 합성과 분석은
역프로서］스이며, QCELP(Qualcomm Code Exited Linear I斗edictive) CODEC은
선형 필터의 합으로 표현되므로 선형이고, 한 Frame어］서 시불변인 정상적인 상태
라고 한다면 LTI(Linear Time Invariant) 시스템으로 가역적인 특성이 있다.(2장
을 참고하라D. 따라서 가역적인 환경이므로 분석（／뇨rnlysi帥과 합성（Synthesis) 프
로세스는 동일한 처리과정으로 타당하다 할 수 있다. 다시 말해서 합성한 Frame이
선형시 불변한 시스템에서 처리퇸 프로세스이므로 이것의 가역적인 성격인분석 또
한 타당하다는 것이다．
    9. Vocoder                                                                51 1
.



    9.3 QCELP(Qua노omm Code Exited 니near F가edi에ye)

    Qualcomm에서는 CI呱4A다중접속에 부합되는 Vocoder로 CELP(Code Exited
Linear Pre小毗如e）를 사용하고 그것을 Qualc이ml형 CELP라고 해서 QCELP라고
명명하였다. 이것은 Is身；의 8KQCELP에서 출발해서 玗％A로 8KQCELP의 발
전형태로 소개되었으며, 힌국형 Pcs에서는 13QCELP로 데이터 속도를 높여서 코
딩하는 방식이 나오게 되었다．
    이 절에서는 13QCELP를 중심으로 소개하면서 이러한 variable rate Codec의
Algorithm 등어］ 대해서 공부한다．
    13K QCELP은 음성 활성량어］ 따라서 20ms 마다 13.3/6.2/2.7/1 Kbps중 한 가지
의 전송률을 선택하여 부호화하며, 분석／합성법을 사용한다. 이것은 음성의 활동성
(V여ce Act如ity）에 의해서 결정된다. 전송률은 배경잡음 에너지와 현재 Frame 어］
너지를 비교함으로써 결정되는데, 높은 전송률이 결정되면 LPC(Linear I노edictive
C以五ng) Parameter들은 낮은 전송률에서 보다 정확하게 전송된다． 또한 Pitch
Parameter와 Codebook P可ameter는 LPC어］ 비해서 빠르게 갱신된다.
                            Rate 1

                    LSP                           32

                   Pitch         11         11          11          11

                 Codeboo    12 12 12 12 12 12 12 12 12 12 12 12 12 12 12 12


                            Rate 1/ 2

                     LSP                          32

                   Pitch          11        11          11          11

                 Codeboo         12         12          12          12


                            Rate 1 /

                     LSP                          32

                   Pitch                           0

                 Codeboo                     4           4           4


                            Rate1/ 8

                     LSP                          32

                    Pitch                          0

                 Codeboo                           6


                                       （그림 아5) Bit 할당
   512                                                            9. Vocoder
                                                                               U


 1개의 Frame어］서 13K QCELP에서 전송하는 Packet의 형태는（그림 9-5）와 같
다. Full Rate인 경우 LSP는 20ms 마다 한 번씩 갱신되고, Pitch는 5ms마다 마지
막으로 Codebook은 1.25ms마다 갱신한다. 즉 Codebook으로 표시해 주는 음성의
성분이 LSP로 표현되는 음성의 성분보다 약 16배 정도 빠르게 변하는 성분을 표시
한다고 생각할 수 있다. 이러한 음성성분의 갱신속도는 그 해당 I뇽ameter가 추출
하는 성분이 고주파에 포함되어 있는 성분, 혹은 저주파어］ 포함된 성분에 따라서 결
정퇸다. 이와 갇은 경우 코드북어］ 의해서 추출되는 성분은 가장 고주파인 것이라고
할 수 있다.
 또한 Rate 1/4이나 Rate 1/8인 경우 피치성분이 없는 것을 볼 수 있는데, 이것은
피치성분이 없는 Frame을 전송하기 때문이다．
 8K QCELP의 경우와 비교했을 때 LPC P可ameter의 경우 낮은 전송률에서 더
욱 세믿해졌고, Pitch Parameter의 표현을 rough하게 표현했다. 이것은 낮은 전송
률에서는 음성의 재생에 Pitch보다 Formant 성분이 더 중요하게 취급하는 것이고,
또한 이러한 가변 Pitch 대신 Codebook을 더욱 강화하였다. 이것은 개량퇸
QCELP에서 무성음으로 간주되는 저속의 데이터들은 Pitch 성분이 없고, 비 주기
성 성분이 강하므로 그러한 특성을 충분히 반영한 형태로 수정을 가했을 것이라는
생각을 한다．
 QCELP의 구조는 （그림 9-6）과 같다．
 각각의 블록어］ 대한 대략의 기능은 다음과 갇다．
 Formant 필터 혹은 LPC 합성필터는 성도를 묘사한 장치이며, 성도（Vocal tract)




                                 P"(n)   F。rmant
                                                     y (ri)
                                                     1 卜 Fostfilter




                           :
                                     >    Filter


                                                              十    1汀（n)




             1     G      L& b            ai n/ ao



         \         입력 파라메터                     /

                                                              출력음성
                 （그림 9-6) QCELP DeCoder의 구조
.
    9. Vocoder                                     513
                                                         I
의 여파（Filter）어］ 의해서 발생된 원래 음성의 공진 주파수와 최대한 유사한 공진 주
파수를 구한다. 이것은 음성의 성분분석 중 가장 저주파 성분을 추출하는데 사용된다．
    Pitch 필터는 유성음인 경우 성대로부터 들어오는 주기적인 pulse열을 표현한다．
    Codebook은 무성음의 파열음과 무성음에서 성대가 자극되는 것을 표현한다. 배
경잡음이나 조용한 경우에 Codebook의 출력은 임의의 잡음으로 표현된다. 이것은
가장 고주파 성분들을 추출하는 것이다．
    Postfil扼r는 Parameter 양자화와 불완전한（力debook어］ 의해서 부가되는 양자화
잡음을 표현할 때 사용된다.
    Gain Con甘아은 Postfilter로 인한 전반적인 음량의 변화가 없게 하기 위해서 사
용된다．

     9.3.1 스펙트럼 분석 : LPC (Linear Predict加e Code)

    스펙트림 분석과정은 일반적으로 몇 가지의 과정들로 이루어진다. 창틀화 과정인
더］ 이것은 특정구간, 즉 Frame당 데이터를 처리하기 위해 데이터 스트림을 특정구
간 동안 선택하는 과정이라고 할 수 있다. 마치 기차킬 옆 오막살이집의 창문을 통
해서 지나가는 기차를 볼 때 창을 통해서 보면 지나가는 기차의 일부구간을 보는
것과 갇다．
    다음으로는 자기상콴 값을 계산하는 과정이 있다. 음성의 변동사항은 급변하지
않으므로 우리는 앞뒤상황을 통해서 선형적으로 예측할 수 있으며, 자기상콴 값은
이러한 예측을 위해서 자기상관을 계산한다. 이렇게 구해진 선형 예측 부호화化PC)
계수는 LSP로 양자화 된다．
    LPC 계수의 양자화를 위한 LSP 주파수로 변환과정과 LSP 주파수의 전송을 위
한 LSP 코드로 변환, 즉 양자화 과정이 마지막 처리과정이다．
    음성은 일반적으로 20Hz( 20KHz어］ 분포되어 있으며, 일반적인 전화의 경우 음
성 소스를 끄(I七로 대역 제한을 한다. 이것은 2장에서 공부한 Nyq毗t 이론어］ 의하1
서 8KHz의 펄스로 표본화함으로써 이루어지며, 또한 표본의 레벨을 14 Bit로 양자
화한다．
    음성신호에서 대부분의 모음은 15- -20吐'Is 구간 동안 거의 변하지 않는 정상상태
(stationary）이며, 스펙트럼 븐석은 이러한 20ms정도의 짧은 구간（Sho心Term)
신호를 Frame으로 정의하여 다음의 일련의 과정들을 수행한다. 음성을 분석할 때
   514                                                                                            9. Vocoder
                                                                                                               口

Frame으로 모든 과정이 이루어지므로 음성 표본틀 중 특정시간 위치에서 Frame을
정의해야 할 것이다. 그러나 여기에서는 정확한 Frame 단위 블록화로 인해서 발생
하는 스펙트럼의 변화현상을 제거하햐 한다. 이것을 위해서 Frame의 시작 부분과
끝 부분의 진폭을 영（zero）어］ 가깝게 처리하여 Frame화 했을 때 갑작스러운 표본
의 크기 변화를 완만하게 해줌으로 주파수 축에서 왜곡을 적어지게 하는 창틀화 작
업이 필요하다．
 윈도우 함수에 의해 음성파형을 곱하므로 Frame 경계에서 표본들의 안정성을
어느 정도 보장할 수 있고, 윈도우 함수의 Fourier 변환과 음성 스펙트럼 또는 스펙
트럼 영역에서 가중치 이동 평균어］ 대한 Convolution을 수행시킨다．
 QCELP에서는 이상과 갇은 특성을 충분히 가지며, 가장 널리 사용되는 Hamming
M及ndow를 사용한다. Hamming M及ndow 의 표현식은 (9.2）와 같다.

                  1                n
                  1 U.>4- U.4tcos(----)                  O 5nS1>9
                   '1   =   .   .1   .   戶   .       .   八     '       d   ＝   八




         WH(fl) -1               '159"                                                                    (9.2)
                  I          0                               otherwise

 음성신호의 시각 n에 있어서 표본치 S, 과 그 주변의 표본치와의 사이에는 강한
상관성이 있다. 시각 n어］ 대한 표본치 욱은, 예를 들면. 과거의 표본치 S，크, sn-2,
. , 욱-p에서 예측할 수 있다. 이것을 다시 말하면, 현재는 과거와 특정한 상관관계
어］ 의해서 이루어지고 예측될 수 있는 것이다라는 관념적인 내용을 내포하고 있으
리리寸 이러한 생각은 우리의 일상 생활 속에서도 흔히 응용된다. 다음의 예제를 풀
어보자．


             다음의 수열에서 빈칸어］ 틀어갈 수는 무엇인가 7
              순서            1            2       3       4         5               6    7    8       9    10
              수열            1            2       3       4         5               6    7    8       9     2


             답은 10이다. 그렇다면 왜 10인가 7
             이것은 우리가 직관적으로도 10이라고 알 수 있는데 여기에서 조금
             더 어려운 문제를 보자. 즉
              순서            1            2       3       4         5               6    7    8       9    10
              수열            1            2       4       7         11              16   22   29     37     7
.
    9. Vocoder                                             二） 겨 R

                                                                    I
                 답은 46이다. 이것도 직관적으로 알 수는 있겠으나, 우리가 46이란
                 답을 얻은 것은 각각의 값들의 상관성을 가지고 추측할 수 있었고，
                 그것의 변화가 예측 불가능하게 급격하지 않고 선형적으로 변한다고
                 생각했기 때문이다. 즉 n번째 수와 n+1번째 수의 변화량을 보고 n+2
                 번째의 값을 예측한 것이다. 다시 말하면 n번째 수가 n+1번째 시간
                 이 되었을 때어］ 변화된, 즉 자기상관값을 통해서 다음에 나타날 값을
                 알 수 있는 것이다. 앞의 2장에서 언급한 바와 같이 현재의 값은 과
                 거 시점에서는 미래의 값이었고 미래 시점에서는 과거의 값일 것이
                 다. 우리는 자기상관성을 계산함으로 미래의 값을 예측할 수 있는 것
                 이다. 이때 주의할 것은 그것의 변화가 선형적이어야 한다는 것이다．
                 이러한 선형적아라는 것은 일부 구간에서 선형이어도 된다. 여기에서
                 설명하고 있는 음성신호의 예측은 이러한 생각을 바탕에 두고 이루
                 어진다．
    어찌 되었든 QCELP에서는 17개의 자기상관 계수를 구함으로써 10개의 LPC계
수를 구할 수 있다. 이것은 다음의 과정들에서 보여준다. 예측치 g, 은 다음과 갇이
주어진다.

                 寸台
           了
                   q  S                                             =
           n
                                                                (9.3)


    식 (9-引에서 알 수 있듯이 현재의 예측치는 과거 n개의 값들어］ 가중계수를 곱한
선형적인 합으로 표현된다. 콴측치어］（실제 값） 대한 오차는 다음과 같다．

          e = S, -S, = S, -Z a1S，냐                              但4)

    여기어］서 ｛出는 선형 예측계수이다. 예측 오차를 최소화하는 { cli｝를 구하는 것이
여기에서의 목표이다. 식 (9-4)의 예측오차의 자승 평균치는 식 (9-5) 와 같다．

          E{e2, } = E{S, + a1S, 1 + a2s, 2 + ...+ cr,S。}        (9.5)

    식 (9旬으로부터           e2 , 을 최소로 하는 연립방정식으로부터 { a2｝를 구할 수 있다．
이것은 식 (9-旬를 { 耐로 편 미분을 하여 극한（최소）값을 구하면 된다. 이때 { a}
의 계수를 가지는 변수 { R,｝의 n개의 방정식으로부터 { 的를 구할 수 있다. 즉,
I11
       516                                                                                9. Vocoder
                                                                                                       U


                                                                                                  但6)
                       da.
      식 (9-이으로부터



                                      只 凡 R            尺 只 凡
                                                                          R          ／己

                             只 尺
                  R。                                                           a,
                                                                          ／亡   a,
                                                                                     R1
                                                                               (Z3   R2
                                                                                                  (9.7)
                             m        m                m
                  I亡.                 足l           R,_              ·．·   R(   （가    I乙

      여기에서，

             只＝s, ·S，냐                                                                            (9.8)

이다. 즉 玘는 S, 와 S,日의 자기상콴값이다．
      여기에서 음성 Frame어］ Hamming 윈도우를 씌운 Frame에서 생각하면, 玘는
Hamming 윈도우가 대칭적인 창이므로 （凡＝-R1)이 되며, 윈도우를 통과한 음성
표본들은 S,n （여기에서 n=0, 1, 2. .... l十1）으로 정의할 수 있다. 이것들의 자기상
관은 다음과 같다．

                                                                                                  (9功
             只＝                =“客’           s,   ,   ·   S州   '




      식 (9기에서 좌변의 행렬식이 자기상괸을 통하여 결정되면, 선형 예측계수들은 쉽
거］ 구해진다. 이것을 계산하기 위하여 Durbin의 Recursion이 사용된다. 참고로 13K
QCELP에서는 식 (9-기의 경우 n=10이며, 식 (9아의 N=17이다. 즉 0에서 16까지
의 표본들을 shift하여 17개의 자기상관을 계산하여 10개의 LPC계수들을 구한다．
      이러한 LPC 모델을 나타내는 선형필터의 전달함수를 구하기 위해서 식 (9-引를
万trai娼form하면 다음과 갇다．
                    (Z) = .1
             H(Z) =S
                                                                                                 (9.10)
                   e(Z) 1+乞a,Z
                             「'

      단시간 구간（short寸erm）에서 구한 LPC 계수들을 이용하여 전송 특성, 즉 음성
신호의 스펙트럼이 구해진다. 식 伯-10）의 시스템 함수는 전극（All pole) 함수이며，
이러한 극점틀은 해당 시스템의 자연 주파수어］ 해당되며, 여기에서는 음성 스펙트
 1
     9. Vocoder
                                                  517
                                                        I
럼의 Foimant어］ 대응된다. 시스템 함수의 분모를 "0"으로 두고, 실계수의 n차 방정
식을 풀어서 Fonnant 주파수 및 대역폭을 추정할 수 있다. 음성에서는 몇몇 개의
Foi끄追nt가 중요하며, Formant의 위치 관계나 시간 변화어］ 의해서 음성을 듣고 판
단한다. 이렇게 구해진 I丑z）의 근들은 주파수 영역에서의 필터 Parameter들이다．
음성의 선형 예측 분석에서는 n = 8 - 10 이 이용된다. 참고로 n은 성대의 진동을
동반하는 유성음을 8 - 10 정도로 생각하며, 여기에서는 10으로 설정하였다. 또한
창의 크기와 Frame Shift를 20ms로 하였다.
     선형 예측 분석에서는 음성신호의 자기상관에서 LP(二 계수가 얻어지고 이러한
LPC 계수는 계수감도가 좋고, 부호화할 때 충분한 계수 정밀도가 필요하다. 이러한
것들을 LPC계수는 만족하질 못한다. 때문어］ LPC어］ 기반을 둔 새로운 음향적인 구
조를 생각한다. 이것을 위하여 여기에서는 성문（성대 간격）에서의 경계조건을 성대
의 진동어］ 동반하여 개단（開端：札+1= 1) 또는 폐단（閉端：左, H=HD으로 생각해서
나온 Parameter인 LSP(Line Sp戈tral Pair）를 사용한다. LPC 계수들은 이러한
LSP 주파수를 사용하여 부호화되는데 이것은 LSP Parameter들이 양자화되기 쉽
고 안정하기 때문이다. 또한 이것은 Frame의 경계치의 연속성을 가질 수 있도록 보
간（Interpol砒ion）이 쉽다는 장점이 있다．
 인간의 성도는 많은 굴곡을 가지는 복잡한 음향학적 구조를 가지고 있다. 이를 서
로 다른 단면적을 갖는 무손실 음향관의 연속적인 형태로 가정할 수 있고 인간의
발성은 이러한 여러 개의 음향관들이 시간에 따라 각기 다른 모습으로 변화시켜 성
도의 특성을 변화시키는 것으로 볼 수 있다. 여기에서 h+1는 편자기 상관 계수
(PARC아｛: PARtial CORrelation）로 성도를 단면적이 다른 복수개의 음향관으로
근사화하였을 때 접속면에서 음파의 반사 계수와 같은 것이다. 음향관 양단에서 +1혹
은 1은 완전 무손실계를 나타내며, 여기에서 +1은 단면을 완전히 통과（Forw町d）하
는 것으로 생각되고, -1은 완전히 반사（Backw町d)하는 것으로 생각된다．
 原，+1= 士1의 조건에서 식 (9-11）의 시스템 함수 분모 다항식의 근을 구하면 그
것은 스펙트럼상에서 선 스펙트럼（LSP) 형태로 나타난다. 성도는 음파의 진행 방향
의 선형 필터와 반사어］ 의한 Reverse의（계수만 다른 동일한 형태의） 선형 필터의
양방향의 격자 필터로 （그림 아7）과 같이 모형화될 수 있다. 이것은 처리구간 내의
잔차 신호 A ,_ i S(2) 및 B,_1S(2）에서 상관기를 사용하여 左, 을 구하는 조작을
n=0에서부터 시작하여 최후로 전향 잔차 신호 e(Z）를 얻는다.
   518                                                           9. Vocoder
                                                                              .


      S(Z)       AQS(Z)       A1S(Z)             An-1S(Z)   AS(Z)=e(Z)




                 B0S(Z)       B1S(Z)            Bn 1S(Z)      BS(Z)

               A ,S(Z) : Forward Component
               B ,S(Z) : Backward Reflection Component

                           （그림 9-7) 격자형 분석 필터

 합성의 경우도 마찬가지로 （그림 9-7）이 가역적이므로 （그림 9-8）과 같이 나타낼
수 있다. 이러한 합성 필터에서 전향 잔차 신호, 또는 모델화한 구동 신호 e(Z）를 입
력하면 재합성 신호 S(2）를 얻는다．

         凡1(Z) = A (Z)+k屈－1(Z)
         B (Z) = Z ' [B, 1(Z) - k,A_1(Z)]                                (9.11)

 QCELP에서는 성도를 모델링할 때 편자기상관 계수 혹은 반사계수인 左, +1를 (1

으로 가정하였고, 따라서 Reverse 선형필터 B(Z）는 万（' +DA(Zb이다. 이상에서
성도의 전체 표현식은 A（刀를 左, +1이 +1일 때어］ 只2）로, 1일 때에 Q(Z）로 분리
할 수 있다. 즉

         P(Z) = A(Z) + Z '"'A(Z ')                                       (9.12)

         Q(Z) = A(Z) - Z ( "' 'A(Z ')                                    (9.13)

이다．
 식 (9-12), 식 付13）는 반사계수 虎, +1가 (1이므로 只2）와 Q(2）의 모든 근은 단
위 원상어］ 존재하며, 이것은 只2）와 Q(2）의 모든 근（root）들이 안정적이며，발진하
고 있다는 이야기가 된다. 이것은 只2）와 Q(2）의 표현 결과식인 식 (9-14), 식
僻15）를 고찰함으로써 더 명백해진다. 즉 근의 형태가 감쇠 없는（dampir垠계수가
cos 0형태인） I口가의 형태로 구성된다．
1
    9. Vocoder
                                                                           519
                                                                                 I
          P(Z) = (1+ Z ' )H(1- 2Z ' cos(2Jrw2j 1) + Z2)


          Q(Z) = (1叫 Z ')fl (1- 2Z ' cos(2冗o2j) + Z2)

    이것은 처음에 우리가 성도를 완전 반사계라고 가정한 것과 같은 결과이다. 또한
이것은 상호 분리적인 只刃와 QCZ）가 가지는 근들이 /(i) 의 형태이므로 口r，의 각
（角） 주파수들을 가지는 Sinusoidal신호가 음향관（성도）의 각각의 단면에서 새로운
필터 계수가 된다．
 LSP는 LPC에서 고려하지 않은 반사계수와 반사파어］ 대한 생각을 추가하여 주파
수 영역에서 불안정（Unstable) 할 수 있었던 LPC의 단점을 해소한 것이다. 그러나
LSP 역시도 그것을 쉽게 구하기 위해서 성도를 무손실로 가정하고 생각했으나 이
것은 아직까지 문제 거리로 남게 되며, 이러한 문제는 Forw可d과 Reverse 신호의
크기어］ 있으며, 이것은 LPC필터를 기본으로 하는 P(Z）와 Q(Z）어］ 가중치를 둠으로
해결될 수 있다．
 이렇게 LSP가 구해지며, 이것은 전송을 위하여 전송코드로 변환되어 전송된다. 각
각의 LSP 주파수들은 차동 양자화기를 사용하여 부호화된다. 먼저 바이어스가 감산
되는데 이 바이어스는 입력이 백색 잡음일 때 주파수어］ 추가된 값이다. 그런 다음에
바이어스를 뺀 결과로 나오는 값과 이전의 Frame어］ 기반하여 예측된 값간의 차이가
스칼라 양자화된다. 그리고 각각의 전송률어］ 대해서 서로 다른 스칼라 양자화기를 사
용하여 LSP 주파수 각각어］ 대해 서로 다른 양자화 범위와 양자화 간격을 가진다．

           Ae(Z)        An- e(Z)             A1e(Z)         A。
                                                             e(Z)   S(Z)




            BS(Z)       B , 1S(Z)            B1S(Z)         B。
                                                             S(Z)

                   AnS(Z) : Forward Component
                   B。S(Z) : Backward Reflection Component

                            （그림 아8) 격자형 합성필터
                                                      9. Vocoder
                                                                   1


 지금까지 단구간의 스펙트럼 분석에 대해서 생각했는데, 이러한 단기간 분석의
문제점을 생각해 보자. 음성신호의 중요한 정보들은 음성신호가 급격히 변화되는
구간어］ 포함되어 있는 경우가 많다. 폐쇄자음（p, b, k, g, t, d), 마찰음（1, v, 8), 유／
무성음의 천이구간 등이 그 대표적인 예이다. 그러나 단기간 분석방법의 경우 한
Frame내의 일부분에서 심한 변화가 생기면 Parameter를 정확하게 추정하1 낼 수
없다. 오차를 더 줄이기 위해 Frame의 이동간격을 더 작게 할 수 있으나, 이는 동일
한 크기의 시퀀스를 나타내기 위한 Parameter의 수를 증가시키는 단점이 있다. 또
Frame의 길이를 줄일 경우 데이터의 부족으로 인해 Parameter의 추정오차는 오히
려 증가할 수도 있다.


   9.3. 2 1才tch탐색

 Pitch검색은 불규칙 （力debook 내에서 최적의 코드 워드를 찾아내는 불규칙
Codebook 검색으로 QCELP 부호화기의 계산량어］ 큰 영향을 미치는 부분이다. 또
한 Pitch Parameter는 합성음의 음질어］ 매우 중요한 요소이다．

                    레벨




                                                  >
                                           샘플번호

                         （그림 9-9) 원음성 파형

 （그림 9-9) 시 （그림 9-11）어］ 보여진 것같이 음성신호는 음성의 Formant 주파수
를 추출하고 나면 잔차 신호는 평탄하게 된다. 그러나 무성음의 경우는 스펙트럼이
상당히 평탄하게 되나 유성음의 경우는 음성의 진동주기인 Pitch 주기가 잔존하고
있으므로 잔차 신호는 또 다른 해석으로 신호의 파라메타를 추출해야 한다．
 여기에서 행해지는 모형화는 （그림 9-10）의 잔차仕esidual) 신호를 （그림 9-11）과
같이 무성음원은 八4계열로, 유성음원을 Pitch주기의 펄스열로 표현하는 것이다．
     9. Vocoder                                                                        521
I



                   레벨




                             무성부             유성부




                                                                               >
                                                                        샘플번호

                               （그림 아］0) 예측 잔차


  이것은 잔차 신호의 장구간(long扼nfl) 상관성 분석을 기본으로 하여 분석
Frame마다 유성, 무성의 판정과 Pitch 추출을 수행함으로 쉽게 실현할 수 있다．


                  레벨




                       끄咽II Hmmm小lmnn { 1 U川m mnm i 1 U!mm   i
                                                                 i 1!
                                        무성구동                     유성구동
                                         신호                       신호




                                                                                   卜
                                                                          샘플번호


                         （그림 9-11) 잔차 신호의 모델화


     Pitch 검색기의 역할은 Pitch 필터의 구현에 필요한 2가지 Parameter인 Pitch 지
    연과 Pitch 이득을 구하는 것이다. Pitch 지연은 이전 Fr跏ne의 Pitch 필터 출력을
    이용하여 변형되어지는 확장적응 Codebook을 이용하여 현 Frame어］ 대한 최적의
    Pitch 필터 출력을 얻게 하는 값으로 결정한다．
     Pitch 필터는 다음과 같은 형태를 가진다．
    522                                                                       9. Vocoder
                                                                                           U



           1     1
                                                                                    (9.16)
          P(Z) 卜bZL

  여기에서 b는 "Pitch 이득"이며, L은 "Pitch 지연" 이다. Pitch 지연은 앞에서 이
야기했듯이 유성음이 발생될 때 성대를 밀고 밖으로 유출되는 공기가 형성하는 공
기의 펄스 주기와 같다. （그림 9-12）는 그것을 표시한 것이다．
 Pitch 지연은 Pitch가 갱신될 때마다 8 Bit를 사용해서 표현된다. 이것은 8K
QCELP의 경우 7 Bit를 사용되는 것과 비교된다. 이러한 차이는 8K QCELP의 경
우 Pitch 지연값을 설정할 때 17에서 143까지 1로 균일하게 레벨간격을 잡은 것과는 달
리 13K QCELP에서는 17에서 140까지의 값은 레벨간격을 0.5로 나머지는 1로 함
으로써 iBit가 늘어난 것이다. 이것은 8K QCELP에 비해 17N140의 Pitch지연을
더욱 세밀하게 표현한 것이다. 즉 8K QCELP 보다 Pitch 탐색 후의 잔차 신호 러］
벨이 작아지는 것을 기대할 수 있다．

                    A
              공기압




                            I,
                                 7]
                                      7
                                      ,   ?k
                                          .I,
                                                1   ,
                                                        7]
                                                             I
                                                                 i
                                                                     I   시간


                    （그림 9너2) 성대에서의 공기 펄스 열

 Pitch이득 b는 Pitch Parameter를 갱신할 때마다 3Bit로 스칼라 양자화된다．
Pitch이득의 레벨은 0에서 2.0이며, 0.25의 레벨간격을 가진다．
 최적의 I亐tch지연 및 이득을 얻을 때는 LPC 오차 가중 필터（Error Weighting
Filter）를 사용하여 평균 자승오차를 구함으로 청각 테스트시 최적인 Pitch 필티 출
력을 얻고자 하는 것이다. 이어］ 사용되는 필터는 다음과 같다．


                        1
      W(Z) = ,='
              加Z-
                                                                                   (9.17)
              刃2百'z니
    9. Vocoder                                                                      523
.

    이때 P는 스펙트럼 필터（LPC 필터）의 차수이고, a는 스펙트럼 필터의 계수이다．
식 (9-17）는 다음과 같이 쓸 수 있다．

              (Z) =
          W
                                    (Z)
                           A
                                                                                     (9.18)
                                                           )
                               .        .   L.
                           A       (-
    이때 ：는三 0과 1사이의 값이 일반적이며, 13K QCELP에서는 0.78이다．
    최적의 I거［tch이득 L' 와 Pitch 지연값 b' 의 결정시에는 최소 자승오차小4SE :
Mean Squared Error）를 계산하게 되는데, 이 경우에는 Formant 합성필터를 통과
한 신호, 즉 합성음성과 입력음성 신호의 차이를 가중 여파한 신호 兀（功과 Pitch 여］
측 필터의 예측값 勿노（功의 차이의 자승이 최소인 Pitch지연과 이득을 선택한다．



          MSE =       t{                         x   (n)       _   byL   (n)   }2    (9.19)

    여기에서 YL(功은 식 (9-20), 식 (9-21）과 같이 정의할 때，


          EL＝易的，(n)                                                                  (9.20)
            民         易向                                                             (9.21)   =




    식 (9-22）과 같이 되며, 이것을 최소화하는 L과 b를 순환적으로 구한다．

          - 2b民L 十b2E),YL                                                            (9.22)

    식 (9-22）의 최소값을 갖는 b를 찾기 위해서 b어］ 대해 미분하면 식 (9小23）과 같다．

                                                                                     (9.23)


    이것은 분석／합성법어］ 의해서 선택되며, 복잡도를 줄이기 위해서 순환적 Convo
뇨tion 기법이 사용퇸다. 순환적 （노nvolution은 이전의 부 Frame들과 현재 부
Frame의 Pitch 필터의 출력을 이용하며, 초기에는 부 Frame어］ 대한 출력이 결정
되지 않았으므로 스펙트럼 분석의 잔여 신호를 사용한다. 최적의 L과 b는 허용된
범위에서의 완전 탐색으로 결정퇸다. 이러한 구조는 Codebook 검색 구조도 마찬가
     524                                                                 9. Vocoder



지이다. 이것은 （그림 9-13）과 같다．
  이로써 최적의 Pitch지연을 결정할 수 있으며, 이때 최적 Pitch값은 상관값과 어］
너지의 비율이 된다. 이것을 적합값小4atched value) 이라 하며, 이것이 가장 큰 값
이 선택된다．
  이러한 Pitch Parameter들은 전송을 위해서 부호화되어야 한다. 각 Pitch 부
Frame에서, 선택된 최적의 Parameter들 b' 와 L' 는 전송 코드 PGAIN과 PLAG로
변환된다. 선택된 Pitch이득 b' 은, 0.25의 단계로 0과 2.0 사이에 세트 { 0, 0.25, ...,
2.0 ｝어］ 의해서 선형적으로 양자화된다. 선택된 최적이 Pitch지연 L' 은 {17, 17.5,
18, ..., 138.5, 139, 139.5, 140, 141, 142, 143｝의 요소들이다．


            s(n)                      azirin)      e(n)



                                                              'viz 江
                                                            시Z) /A(Z注9
                                                             후｝ 상대
                    (aj for current
                    pitch sub frame



                                                      byL(n)




                              I
                          For all
                          Le{17,17.5,18,18.5 . .. .139.5,
                                                            늬

                          140, 141, 142, 143)
                          be(0,0.25. ... .2.0)


                           （그림 9-13) 아oh탐색



 PLAG 값은 b' 와 L' 에 의존한다. 만약 b' 가 0이라면, 그때 PLAG는 0이다. 그렇
지 않다면, PLAG는 (L* - 16 - 0.5)PFRAC이다. 따라서, PLAG드｛0, 1, ·.., 127}
은 7 Bit를 사용하여 표현된다. Pitch지 연의 분수값은 Bit PFRAC를 사용하여 부호
화퇸다. PFRAC가 0이면 부호화된 Pitch는 정수이고, PFRAC가 1 이면 정수 Pitch
    9. Vocoder                                       525
U

어］ 0.5를 더한다．
 PGAIN의 값은 유일하게 b' 어］ 의존한다. 만약 b*=0라면, PLAG는 0이다. 그렇지
않다면, PGAII은 (b*/0.25 小 1）이다. 따라서 PGA]八은 3Bit를 사용하여 표현된다．
b*=0과 b*=0.25인 경우는 PGAIN=0 임을 주의하라. 이러한 두 경우에서, 첫 번째의
경우는 PLAG의 값이 0이고 두 번째 경우는 0이 아니므로 구별된다．
 결국 Pitch필터를 통과한 잔차 신호는 그것이 가지고 있던 긴 주기성분이 제거되
어 출력 신호는 좀더 평탄하게 된다．
 QCELP의 계산 시간 문제나 전송 데이터 율을 결정하기 위해서는 Pitch검색의
수정이 필요하다. 때문어］ Pitch검색의 경우 4개의 Pitch 부 Frame어］서 Pitch검색방
법을 홀수 Frame어］ 대하여는 모든 경우의 Pitch를 검색하고 짝수 Frame에서는 이
전 Frame의 Pitch 지연값을 기준으로 앞뒤로 전체 Frame 검색보다 작은 한정 범
위 내어］ 있는 값들어］ 대해서만 검색하는 적응형 방식을 생각할 수 있다. 이렇게 하
면, Pitch는 홀수 Frame의 경우 8 Bit, 짝수 Frame은 그 이하 Bit로 전송할 수 있
다. 이렇게 하면, Pitch탐색 시간뿐만 아니라 전송률도 감소시킬 수 있다.
 또한 적응 Codebook의 인접 코드 워드가 대부분의 표본값어］ 있어서 Pitch의 변
화가 급격하지 않으므로 특히 八4커갈수록 표본값만이 달라진 형태를 갖는다는 것을
이용하면, 계산량을 더욱 줄일 수 있다. 이때 최적 Pitch지연과 이득이 상관값과 어］
너지어］ 의해서 결정되어진다는 것을 이용한다. 상관값의 계산량보다는 에너지 항의
계산량이 더 큰 것이 일반적이므로 상관값을 이용 에너지 졔산 횟수를 줄이고자 하
는 것이 그 방법이다.

     9.3. 3 Codebo아（ 탐색

 Codebook 탐색은 스펙트럼 분석 후 잔차 신호의 비 주기성 성분을 추출하기 위
해서 행해진다. 즉 유성음의 경우 주기성분은 Pitch 검색으로 알려진 LTP에서 걸
러지고 유／무성음의 비 주기 성분은 （力debook Parameter로 추출된다．
 （力debook Parameter들로는 （力debook Inde奴I)와 이득（G）이 있다. Codebook
Index는 전체 C에ebook에서 Codebook 벡터의 거리와 관련되고， Codebook 이득
은 이러한 Codebo갸（ 벡터의 비례 축소어］ 해당한다. 때문어］ 이러한 Parameter들은
Pitch 탐색에서의 Pitch 지연과 Pitch 이득과 동일한 개념들이다．
 Codebook Index와 이득은 한 Frame어］ 대해 Full rate 전송시 최대 16번 갱신된
    526                                                                          9. Vocoder
                                                                                              1


다. I와 G는 순환적인 분석／합성법에 의해서 결정되며, Codebook을 갱신할 때마다 G
의 부호는 iBit를 사용해서 양자화되고 G는 로그(log）를 취한 후 3 - 4 Bit를 사용
해서 차동 부호화 된다. 그리고 Codebook Index는 7 Bit를 사용해서 양자화된다．
 13K QCELP에서는 Rate 1, Rate 1/2 경우는 불규칙 Codebook 검색을 통하여
（力debook 이득과 Index를 결정하고, Rate 1/4, Rate 1/8은 예측 잔차의 에너지로
부터 얻어지는 이득을 전송한다. Rate 1/4의 경우 여기（勵起）이득 Parameter는 5
번 갱신되며, Rate 1/8의 경우 여기 이득 신호는 한 Frame어］ 한번 사용된다．
 Codebook은 탐색 과정에서 얻어지는 것이 아니라 미리 구성을 해야 하며, 이것
은 잡음 신호와 같은 최종적인 잔차 신호를 여파한다는 측면에서 각 코드 워드를
영 평균, 단위 분석 백색 가우시안（Gausian) 불규칙 신호 열로 구성하고 이때 코드
워드 내의 표본 중 75%이상을 0의 값이 되도록 하는 것이다. 또 불규칙 （力debook
을 구성하는데, 완전 불규칙성을 부여하는 것이 아니라 인접 코드 워드간어］ 두 표본
값만 다르도록 하여 코드 워드간에 상관콴계를 부여함으로 계산량을 줄일 수 있도
록 구성한다.


          s(n)                                pam(n) dn느 e(n)

          L求 & 1:）串 for current
          pitch subframe H


                 {ai} for current
                 Codebook
                 subframe
                                                                          x(n)
                             cj(n)




                                 For all
                                 GE{8 a propriate values)




          For all
          IE{O,1.....127)
                                                                     V
                                                                1斗   &1   ( 1斗




                              （그림 9-14) Codebook 탐색
    9. Vocoder                                                            527
U

 （力debook의 크기는 Codebook 탐색시간을 결정짓는 주요 요소이므로 적당한 크
기가 필요하다. 여기에서는 128의 Codebook 2개를 Rate 1과 Rate 1/2어］ 각각 사용
한다．
 Codebook 검색구조에서도 Pitch검색구조와 마찬가지로 상관값과 에너지값을 이
용하여 적합한 값을 결정할 수 있는데, 불규칙 Codebook의 경우 Codebook 구성시
어］ 상관성을 고려하였O 口로, Pitch 검색구조와는 달리 코드 워드간의 에너지 값의
차가 크지 않으므로 상관값의 영향이 매우 커지게 된다.
 최적의 Codebook 이득 G' 와 Codebook Index 값 I ' 의 결정시에는 Pitch탐색과
마찬가지로 최소 자승오차를 계산하게 되는데, 이 경우에는 Pitch 합성필터를 통과
한 신호，즉 합성음성과 입력음성 신호의 차이를 가중 여파한 신호 的D과 Codebo아
                                              （
예측값 y1(功의 차이의 자승이 최소인 Codebook Index와 이득을 선택한다. 즉


          MSE       =브
                         n=O
                               {x   (n)       -   Gy1   (n)   }2           (9.24)

 여기에서 각각의 G에 대하여 y伽）은 G=1일 때 I번째의 가중된 합성음성의 코드
벡터이다．

          가（n) = h(n）水C1(n)for(）드n< L- 1                                   但25)

 여기에서 Codebook은 회퀴적인 구조이므로 Codebook의 표현식은 다음괴－ 같다．

          ,, . .         IC((n-1)m0d128                            n2I
          느UiJ = 5 /1. . 八，, .   .                                         (9.26)
                 I （八I乙?S+ (fl- 1)                                 n< 1

 이때 Codebook Index를 나타내는 I는 0에서 128까지의 범위이다．
 여기에서 식 (9.24）을 최소로 하는 I과 G를 순환적으로 구한다. 여기에서 다음을
정의하면，

                         HZ向
                           V/
                           n                      n
          且，   /=
                           工
                                                                           (9.27)


               瓦         易向               九
                                                                           (9.28)


    식 (9-24）은 식（9-29）과 같이 되고
          -2G且，/+G' 月yyI                                                   (9.29)
    528                                           9. Vocoder
                                                               1

  이것의 최소값을 구하기 위해 G에 대한 미분으로 그것을 구하면 퇸다. 결과는 주
어진 I어］ 따른 G의 값이다．

          G ＝勻                                          (9.30)
             E)
              ,y1
  이러한 방법은 분석／합성법에 의해서 선택되며, 복잡도를 줄이기 위해서 순환적
Convolution 기법이 사용된다. 순환적 Cony아ution은 이전의 부 Frame들과 현재
부 Frame의 Pitch 필터의 출력을 이용하며, 초기에는 부 Fr缸ne어］ 태한 출력이 결
정되지 않았으므로 스펙트럼 분석의 잔여 신호를 사용한다. 최적의 I와 G는 허용된
범위에서의 완전 탐색으로 결정퇸다. 이러한 구조는 Pitch 검색구조도 마찬가지이
다. 이것은 （그림 9-14）와 같다．
 지금까지는Rate 1, 1/2인 경우의 이야기였으며, 여기어｝서는 상대적으로 긴 지연
을 갖지 않는 Rate 1/4, 1/8의 경우는 이러한 Codebook 대신에 의사린帽 코드에 의
해서 여기된다. 이러한 이득 Parameter는 예측 잔차의 에너지로부터 얻어진다. 여］
측 잔차의 에너지는 예측 이득 비율에 입력음성 에너지의 곱으로 표현된다．


          尺（0)＝븜每'(n)                                   (9.31)


 여기에서 L七 Codebook 이득이 계산되고 있는 서브 Frame의 길이이다. 이것은
Rate 1/8인 경우는 160이고, Rate 1/4인 경우는 32이다. 최적의 Codebook 이득 (;'
는 다음과 같다．


             「ession和
            Su卯  『니臂                                    (9.32)


 Codebo아
       （Parameter의 양자화는 데이터 율어］ 따라 다르게 행해진다. Codebook
Index의 경우 入4=7인 Codebo아（을 사용하므로 Codebook Index(CBINDEX）가 필
요한 Rate 1, Rate 1/2는 7 Bit를 균일하게 할당된다．
 Codebook 이득의 경우는 좀더 다앙한 방법을 각각의 데이터 율어］ 따라 적용한
다. Rate 1, Rate 1/2의 경우 균일 양자화와 차동 양자화가 이루어지는데, 차동 양
자화는 Ratel인 경우 4의 배수 Frame에서만 이루어진다. Codebook 이득의 부호화
는 Codebook 이득의 부호（CBSIGN）와 크기（CBGAIN）로 부호화되는데, 부호의 경
우 iBit를 사용 하며, 0보다 크거나 갇으면 1로 작으면 1로 표현한다. Codebook
    9. Vocoder                                               529
.


이득 크기는 그것의 크기를 log scale로 바꾸는 연산의 스칼라 양자화기를 사용하
여 부호화한다. 이러한 스칼라 양자화기는 부 Frame의 수와 부호화 율에 의존하는
3-4 Bit의 선형 양자화기와 이득 예측필터로 구성된다. 즉 Codebook 이득은 Rate
1인 경우 16번 양자화되고 Rate 1/2인 경우 4번 양자화된다．
    Rate 1/4의 경우 이득을 4 Bit 균일 스칼라 양자화기로 부호화하며,. 이것은 음성
의 한 Frame 동안에 5번 양자화가 이루어진다. Rate 1/4는 부호화할 때 Codebook
대신 의사랜덤 코드를 사용하였으므로 Coclebook 색인과 이득은 필요가 없다. 의사
랜덤 코드 벡터는 전송단 부호기의 복호 영역에서와 수신단 복호기에서 있는 랜덤
숫자 발생기어］ 의하써 발생된다．
    Rate 1/8의 경우는 2 Bit의 균일 스칼라 양자화기를 사용하고, 음성의 한 Frame
어］ 한번 이루어진다, 또한 하나의 음성 Frame(20ms) 동안어］ 역시 한번 전송되는
랜덤코드 벡터 발생의 씨앗인 4 Bit의 CBSEED도 함께 전송한다．
    Codebook 검색 과정의 계산량을 결정하는 주요 Parameter는 Codebook의 크기
와 필터의 전달함수의 길이이다. Codebook의 크기는 탐색횟수를 증가시키는 요인
이 된다. 이것은 탐색횟수를 증가시키면（Codebo아혀 크기를 크거］ 하면） 더 많은 형
태의 잔차 신호도 여파할 수 있다는 장점이 있으나 시간이 많이 걸린다. 이러한 시
간을 해소하기 위해서는 탐색에서 적응적인 구조가 필요하나 이것은 시스템의 복잡
도를 증가시키는 요인이 된다．
    여파 과정어］ 의한 계산 시간은 계산의 복잡도가 다르다. 탐색의 경우는 단순한
비교 연산인 반면 이것은 convolution으로 이루어지므로 훨씬 복잡하다. 때문어］ 필
터의 길이가 상당히 중요하다. 일반적으로 Codebook 검색어］ 있어서 합성필터의 길
이는 무한 길이의 것을 사용해야 하나 실제로는 적절한 구간만을 잘라서 필터링시
사용한다. 이것은 음질과 관련되는 부분이며, 이것 역시 계산량과 음질을 동시어］ 고
려하여 어느 것어］ 더 가중치를 두어야 할지를 결정하여야 한다.



    9.4 전송률 결정

    음성신호를 유성음과 무성음으로 구분하는데는 일반적으로 에너지, 영교차 비
(zero寸crossing rate), 상관계수（correlation coefficient), 1차 반사계수, 2차 반사계
수 등 여러 가지 측정 방법을 사용한다. QCELP에서는 속도 결정 Algorithi可Rate
      530                                              9. Vocoder
                                                                    1


Decision Algoi就노Ti)을 2단계로 행하여 전송 Packet의 형태를 결정한다. 각 밴드
에서 다중 밴드 문턱 에너지를 이용하여 음성 활성 정도를 결정하는 첫째 단과 입력
음성의 통계치어］ 근거하는 부호화 율을 찾아내어 데이터 율을 감소시키는 둘째 단
으로 구성된다．

               （표 9너） 속도 감소를 위한 타당한 속도 수정

            Input Rate                  Cu巾Ut Rate
                1                        1, 1/2, 1/4
               1/2                        1/2, 1/4
               1/8                          1/8


     첫 번째 단에서는 배경잡음 에너지를 지속적으로 계산하고 배경잡음 에너지의 추
정치와 현재 Frame 에너지간의 차이어］ 따라 전송률 을 결정한다. 먼저 각 Frame어］
서 이전어］ 계산된 배경잡음 에너지의 추정치는 현재 Frame 에너지와 비교된다. 그
래서 이전의 에너지 추정치가 현재 Frame 에너지보다 크다면, 추정치는 현재
Frame 에너지로 교체되고 그렇지 않을 경우에는 그런 후어］ 전송률은 배경잡음 어］
너지의 추정치 위에서 추정치와 일정한 간격을 유지하며 활성 음성은 Ratel 과
Ratel/2로, 배경잡음은 Ratel/8로 결정한다．
     두 번째 단은 과중한 용량 증가를 위해서 속도 감소 작동을 요구하는 서비스 선
택제어 명령에 의해서 작동한다. 둘째 단에서의 속도 수정은（표 9-1>어］ 나타나 있
다
     여기에서는 음성을 6가지 형태로 나누어 부호화 모형을 검출한다. 영 교차와 규
준화 자기상관함수（NACF: Normalized Auto-correlation Function）는 유／무성음
분류어］ 사용되고, T町get..SNR은 QCELP 모델의 부호화 효율을 추정하는 데에 사
용된다. 그리고 예측 이득 미분치, LSP 미분치, NACF는 정상적이고 과도적인 음
성의 특징을 검출하는데 사용된다. 마지막으로, 평균下rame-에너지와 현재 Frame
에너지의 비와 LSP 미분치는 임시로 위장된 음성 Frame을 검출한다．
     이러한 6개의 문턱 값들은 다양한 부화화 형태를 결정하는데 사용된다. 문턱 값
은 배경잡음 에너지와 음성 활성화율의 원하는 평균 부호화 율어］ 근거하여 적응된
다．
    9. Vocoder                                                                  531
1



    9,5 겸론

    QCELP은 식 (9-10）과 같은 Open-loop 스펙트럼 Parameter 추정 방법의 LPC
필터와 LPC와는 달리 Open-loop와 Closed-loop탐색을 하는, 비교적 짧은 지연의
가중퇸 음성 잔차 예측인 I砒ch검색과 짧은 지연과 긴 지연의 가중된 음성 잔차 여］
측인 Codebook 검색의 과정으로 이루어진다. （그림 9-15）은 QCELP의 구조도이
다. 이것은 LPC 필터의 잔차 신호를 제거하기 위해 LTP롤 추가한 것으로 음질의
개선이나 계산 시간상의 문제는 거의 LTP라 할 수 있는 Pitch 탐색과 Codebook
탐색에서 일어난다．
    향후 개인 휴대통신에 사용될 음성 부호화기의 구조가 어떤 요인을 더 원하느냐
에 따라 그것의 구조가 바뀌어야 할 것이다. 그러나 지금 현재의 QCELP은 "음질",
" 계산 지연 시간", " 시스템의 복잡도" 등과 같은 3가지 항목이 trade-off의 관계가
있다．




       U               11
                     兄 h7 {T.n
                                 /／口二'7 =

                                            1+2；아 z니
                                                       r1’乙'7=       p
                                                                 l +2;（乂 Y Z기
                                                                    江i




                     （그림 아］5) QCELP의 구조


    이러한 3가지 요인을 모두 최적인 것으로 하기 위해서는 효과적인 Codebook 설
계와 더 적절한 Codebook의 적용방법이 더욱 필요할 것으로 생각한다. 이것은
QCELP이 사람의 음성신호의 특성을 선형 필터들로 모델링 한 것이라는 것에서，
사람의 음성신호의 또 다른 특성을 발견한다면 더 효과적인 음성 부호화기를 만들
수 있을 것이다．
                  八4U
                        색 인
                                                                                 1




回     Access Attempt 240
      Access Entry Handoff 344, 349
                                                  Cot싸oh凡ion 89, 앉II
                                                  Convolutional 47
      Access Handoff 287, 344                     Convo뇨tional 부호화 361
      Access Probe 239, 244, 346                  Correlation 68, 185
      Access Probe Handoff 344, 3印                Correlator 201
      Access Sequence 240                         Cross-Correl砒幻n 68
      Access 채널 345, 410                          CT 29
        Active Set 243, 289, 356
        ANSI 59                              r i Delay L<乂kl刃op 205
        Autocorrelation 49, 68, 70           니UDelay Spread 236
        AWGN 109, 110, 374                      Demodulation 260, 376, 466
                                                Dem어把la加r 177, 258

[j    Bandwidth   104                             Deskewer 213, 214
 ===Block Code 362                                Detect state 223
     Block Interleaving 378                       Doppler Spread 236
     미ocking Probabi血y 141                        Dummy Pilot 319
     BPSK 119, 122, 383                           Dwell state 225
                                                  Dynamic Threshold 310

［희    CAl 58, 305, 497, 505
      Candidate Frequency 326, 329
      Candidate Set 289, 298, 345            回    Effi 230, 249, 250, 251, 272
                                                  Erlang 141
      CAVE Algori仕m 15, 491                       Error 함수 105
      CDM 394                                     ESN 241, 410
      CDMA 43, 131
      CELP 505
      chip rate 132, 258, 391                回    FA 318, 320
                                                  Fading 144, 1凹, 212, 235
      Chip rate 49, 123                           Fast Rising Pilot 313
      Closed Loop Po＼入／er Cot北r이 231, 232,        FER 230
         242, 244                                 Filter 95
      Code Channel 356, 420                       Finger 198, 257
        Code Symbol 368, 378                      Formant 510, 523
        Codebook 505, 511, 512, 531               F야w町d 232
        Coherent 48, 178, 182, 185                Fourier Spectrum 81
          Coherent Detection 118                  Fourier Transform 83
          Coherent detection 124                  Frequency Hopping 117
                                                                                     '


                                                                       색 인         533
.

          Frequency Reuse Factor 40
                                                  ［히Open
                                                  -
                                                             Power
                                                     OQPSK 48, 388
                                                             Loop
                                                                         Control
                                                                                    238, 242


IT1 G刻ois Field 153                                    아thogonal 49, 70, 71
-   Gated Mode 252                                     Outer Loop Power Control 231, 266,
    GHDM 298, 325, 467                                     274
    Gold Code 119, 174                                 OVSF 173


n口） Hadam打d 入4atrix 173
-   Hash 480
                                                  （틔   Periodic Se可ch 326, 328
                                                       Phase Lock Loop 203
    hashing 410, 429, 430                              Pilot Beacon 319
          HLR 63                                       Pilot beacon 320
                                                       I꾜야 Set 288, 297, 311
口1 IMSI 432. 456. 479                                   Pilot strength 302
-  IMSI S 479                                           Pilot Strength 303
   Int三rleaver 373, 381                                 Pitch 507, 531
          Interleaving 378                              PN Code 166
          IS 57                                         PN Long Code 166
          IS-2000 245, 251, 408                         PN Short Code 166
          IS-95B 58, 139, 243, 287, 298, 308,           Power Control Group 245
              324, 344, 368, 404, 408                   Probe 447
          IS-95C 58, 245, 298, 368, 408                 Processing Gain 127, 133, 151, 360,
                                                           390

    fnLPC     510, 513
    =1口 LSI了II 166, 175, 391                       口人1 QCELP 465, 505. 511
                                                   니日 QIB 230, 250, 251, 272
    I 1 八AHFIO 288. 307. 317. 329                      QPSK 119, 122, 386
    니口d 八/Iatched Fil扼r 95                              Quick 호출채널 440
        MJI)R 58, 139, 409
        message capsule 346                        r i Radio Configuration 58, 320, 368, 465
          MN 432, 弱6                               H＝口 Rake 수신기 212
          Multipath Fading 213, 292                    Remaining Set 289, 339
          Multiple Access 49, 50, 129, 131, 393         Rician Fading 235
          Multiplexing 129, 393                         RIF 336
                                                        RTD방식 319
    ii1    Neighbor Configuration 341
    -      Neighbor Set 289, 354                   I ;1 Search Window 182. 217. 290
           N1) 422                                 느1日 Searcher 178, 180
           Non-Coherent 48, 186, 199                    Searcher정보 228
                                                        Service Option 57, 弱9, 463
    534      색 인
                                                                      1

    Service 구성 465
    Service 협상 324, 467                  回    변조
                                                   的， 108, 117, 124
    Serving Frequency 320, 324
    Shannon 112                          ri 人陪자인증 484
                                          m1 시노 447
    Single Search 327

                                         [히 얼랑 140
    Slam Operation 216
    Slotted mode 弱8                      뇨1d 열 잡음 108
    SMS 63, 432                              음영현상（Shadowing) 237
    SSD 443, 485                             인증 432, 441, 456, 459
    Supplemental Channel 59, 246, 249        임펄스 79, 85
    Supplemen出 Code Channel 139              임펄스 함수 87


回   target frequency 325, 326
    Tau( z- ) Dither Loop 210                잡음지수 109
    TRS 30                                   전력제어 부채널 246, 249, 250
    Turbo 363                                주파수 재사용 147
    UHDM 298

                                         囚 최자"코드
    Verify State 224
    Viterbi 365

                                         回 터보 373
    Voice Activity 145, 247, 252, 372,
       511
    Walsh Code 172, 261, 289, 305, 429           " 1론 97
                                         [司 표본화
    Walsh Code Channel 396, 401          뇨mH 필터 90
    Walsh채널 421
    WLL 26
                                         ［희 확산 변조     118, 123, 390
rE] 叩］벨 103
니m 능록 娼8, 502
   디지털 변조 48, 119, 382
                                인치




all that 's CDMA
초판 1쇄 인쇄 / 2002년 10월 20일
초판 1쇄 발행 / 2002년 10월 25일
 이인처         /
             /
                 옥윤 철
 은행행
                 김 갑용
             J
 지발발         /
                 진한도서
         r
         r



        /
        / /
         /
출판등록             제2-1557호
          /
등록일자             1993년 5월 25일

주     소 / 서울 중구 충무로 2가 21 서울중앙우체국 신관 엊）2호
           Tel. 02-319-3535 Fax. 02-319-3537
           http://www.jinhanbook.co.kr

ISBN 89-8432-087-0 93550
匣） 2002 Jirihan Books INC., Printed in Korea

                                       값 24,000원
